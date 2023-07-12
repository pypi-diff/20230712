# Comparing `tmp/penne-0.5.1.tar.gz` & `tmp/penne-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penne-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "penne-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `penne-0.5.1.tar` & `penne-0.5.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1550 2023-07-10 17:15:24.171165 penne-0.5.1/README.md
--rw-r--r--   0        0        0      564 2023-07-10 17:15:24.347167 penne-0.5.1/penne/__init__.py
--rw-r--r--   0        0        0    12998 2023-07-10 17:15:24.347167 penne-0.5.1/penne/core.py
--rw-r--r--   0        0        0    44214 2023-07-10 17:15:24.347167 penne-0.5.1/penne/delegates.py
--rw-r--r--   0        0        0     4581 2023-07-10 17:15:24.351167 penne-0.5.1/penne/handlers.py
--rw-r--r--   0        0        0      893 2023-07-10 17:15:24.351167 penne-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 penne-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1550 2023-07-12 15:53:26.029546 penne-0.5.2/README.md
+-rw-r--r--   0        0        0      564 2023-07-12 15:53:26.205548 penne-0.5.2/penne/__init__.py
+-rw-r--r--   0        0        0    13202 2023-07-12 15:53:26.205548 penne-0.5.2/penne/core.py
+-rw-r--r--   0        0        0    44275 2023-07-12 15:53:26.205548 penne-0.5.2/penne/delegates.py
+-rw-r--r--   0        0        0     4823 2023-07-12 15:53:26.205548 penne-0.5.2/penne/handlers.py
+-rw-r--r--   0        0        0      893 2023-07-12 15:53:26.205548 penne-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 penne-0.5.2/PKG-INFO
```

### Comparing `penne-0.5.1/README.md` & `penne-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `penne-0.5.1/penne/__init__.py` & `penne-0.5.2/penne/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 Modules:
     core.py
     test_delegates.py
     handlers.py
     messages.py
 """
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 
 # Imports for easier user access
 from .core import Client
 from .delegates import *
```

### Comparing `penne-0.5.1/penne/core.py` & `penne-0.5.2/penne/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,18 @@
             mapping message type to corresponding id
         server_messages (dict):
             mapping message id's to handle info
         _current_invoke (str):
             id for next method invoke
         callback_map (dict):
             mapping invoke_id to callback function
+        callback_queue (queue):
+            queue for storing callback functions, useful for polling and running in the main thread
+        is_active (bool):
+            flag for whether client is active
     """
 
     def __init__(self, url: str, custom_delegate_hash: dict[Type[delegates.Delegate], Type[delegates.Delegate]] = None,
                  on_connected=None, strict=False, json=None):
         """Constructor for the Client Class
 
         Args:
```

### Comparing `penne-0.5.1/penne/delegates.py` & `penne-0.5.2/penne/delegates.py`

 * *Files 0% similar despite different names*

```diff
@@ -761,15 +761,15 @@
         name: Name of the signal
         doc: Documentation for the signal
         arg_doc: Documentation for the arguments
     """
     id: SignalID
     name: str
     doc: Optional[str] = None
-    arg_doc: List[MethodArg] = None
+    arg_doc: List[MethodArg] = []
 
 
 class Entity(Delegate):
     """Container for other entities, possibly renderable, has associated methods and signals
 
     Attributes:
         id: ID for the entity
@@ -875,18 +875,18 @@
         name: Name of the buffer
         size: Size of the buffer in bytes
         inline_bytes: Bytes of the buffer
         uri_bytes: URI for the bytes
     """
     id: BufferID
     name: Optional[str] = "Unnamed Buffer Delegate"
-    size: int = None
+    size: int
 
-    inline_bytes: bytes = None
-    uri_bytes: str = None
+    inline_bytes: Optional[bytes] = None
+    uri_bytes: Optional[str] = None
 
     @model_validator(mode="after")
     def one_of(cls, model):
         if bool(model.inline_bytes) != bool(model.uri_bytes):
             return model
         else:
             raise ValueError("One plot type must be specified")
@@ -969,16 +969,16 @@
         name: Name of the image
         buffer_source: Buffer that the image is stored in
         uri_source: URI for the bytes if they are hosted externally
     """
     id: ImageID
     name: Optional[str] = "Unnamed Image Delegate"
 
-    buffer_source: BufferID = None
-    uri_source: str = None
+    buffer_source: Optional[BufferID] = None
+    uri_source: Optional[str] = None
 
     @model_validator(mode="after")
     def one_of(cls, model):
         if bool(model.buffer_source) != bool(model.uri_source):
             return model
         else:
             raise ValueError("One plot type must be specified")
@@ -1034,17 +1034,17 @@
     """
     id: LightID
     name: Optional[str] = "Unnamed Light Delegate"
 
     color: Optional[Color] = Color('white')
     intensity: Optional[float] = 1.0
 
-    point: PointLight = None
-    spot: SpotLight = None
-    directional: DirectionalLight = None
+    point: Optional[PointLight] = None
+    spot: Optional[SpotLight] = None
+    directional: Optional[DirectionalLight] = None
 
     @field_validator("color", mode='before')
     def check_color_rgb(cls, value):
 
         # Raise warning if format is wrong
         if len(value) != 3:
             logging.warning(f"Color is not RGB in Light: {value}")
```

### Comparing `penne-0.5.1/penne/handlers.py` & `penne-0.5.2/penne/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,21 @@
         component_id (ID):
             ID of the component to be updated
     """
 
     delegate = client.get_delegate(component_id)
     current_state = delegate.model_dump()
     current_state.update(message)
+    updated_model = type(delegate).model_validate(current_state)  # Validate and coerce input
 
-    delegate_type = type(delegate)
-    client.state[component_id] = delegate_type(**current_state)
+    # Merge into old model
+    for field, value in updated_model:
+        setattr(delegate, field, value)
+    for field, value in delegate.__pydantic_extra__.items():  # Hack for now waiting for new release
+        setattr(delegate, field, value)
 
 
 def handle(client, message_id, message: dict[str, Any]):
     """Handle message from server
 
     'Handle' uses the ID attached to message to get handling info, and uses this info 
     to take proper course of action with message. The function has 5 main sections
```

### Comparing `penne-0.5.1/pyproject.toml` & `penne-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `penne-0.5.1/PKG-INFO` & `penne-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penne
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python Client Library for NOODLES Protocol
 Keywords: noodles,cbor,Websockets,client,NOODLES
 Author: Alex Racapé
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

