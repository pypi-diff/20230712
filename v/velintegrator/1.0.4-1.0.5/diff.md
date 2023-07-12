# Comparing `tmp/velintegrator-1.0.4.tar.gz` & `tmp/velintegrator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velintegrator-1.0.4.tar", last modified: Wed Jul 12 11:03:48 2023, max compression
+gzip compressed data, was "velintegrator-1.0.5.tar", last modified: Wed Jul 12 11:27:46 2023, max compression
```

## Comparing `velintegrator-1.0.4.tar` & `velintegrator-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 11:03:48.213129 velintegrator-1.0.4/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.0.4/MANIFEST.in
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 11:03:48.212979 velintegrator-1.0.4/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      742 2023-07-11 14:04:48.000000 velintegrator-1.0.4/README.md
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-12 11:03:48.213176 velintegrator-1.0.4/setup.cfg
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-07-12 11:03:02.000000 velintegrator-1.0.4/setup.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 11:03:48.212290 velintegrator-1.0.4/velintegrator/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.0.4/velintegrator/__init__.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     1031 2023-07-11 14:03:25.000000 velintegrator-1.0.4/velintegrator/handler.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3737 2023-07-12 11:02:41.000000 velintegrator-1.0.4/velintegrator/sdk.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 11:03:48.212836 velintegrator-1.0.4/velintegrator.egg-info/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 11:03:48.000000 velintegrator-1.0.4/velintegrator.egg-info/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-12 11:03:48.000000 velintegrator-1.0.4/velintegrator.egg-info/SOURCES.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-12 11:03:48.000000 velintegrator-1.0.4/velintegrator.egg-info/dependency_links.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-12 11:03:48.000000 velintegrator-1.0.4/velintegrator.egg-info/top_level.txt
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 11:27:46.206047 velintegrator-1.0.5/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.0.5/MANIFEST.in
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 11:27:46.205882 velintegrator-1.0.5/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      742 2023-07-11 14:04:48.000000 velintegrator-1.0.5/README.md
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-12 11:27:46.206088 velintegrator-1.0.5/setup.cfg
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-07-12 11:25:50.000000 velintegrator-1.0.5/setup.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 11:27:46.205022 velintegrator-1.0.5/velintegrator/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.0.5/velintegrator/__init__.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     1011 2023-07-12 11:27:20.000000 velintegrator-1.0.5/velintegrator/handler.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3737 2023-07-12 11:02:41.000000 velintegrator-1.0.5/velintegrator/sdk.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 11:27:46.205699 velintegrator-1.0.5/velintegrator.egg-info/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 11:27:46.000000 velintegrator-1.0.5/velintegrator.egg-info/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-12 11:27:46.000000 velintegrator-1.0.5/velintegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-12 11:27:46.000000 velintegrator-1.0.5/velintegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-12 11:27:46.000000 velintegrator-1.0.5/velintegrator.egg-info/top_level.txt
```

### Comparing `velintegrator-1.0.4/PKG-INFO` & `velintegrator-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.0.4
+Version: 1.0.5
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 Kafka Client for VELI.STORE
```

### Comparing `velintegrator-1.0.4/README.md` & `velintegrator-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `velintegrator-1.0.4/velintegrator/handler.py` & `velintegrator-1.0.5/velintegrator/handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from velikafkaclient.decorators import tracing
+from velikafkaclient.decorators import ctracing
 
 
 class BaseHandler:
     web_integrator = None
     ios_integrator = None
     android_integrator = None
     event_model = None
     params_methods_mapper = {}
     base_params_method = None
     params_method = None
-    tracing_id = None
 
     def __init__(self, event_name):
         self.event_name = event_name
         self.params_method = self.params_methods_mapper[event_name] if event_name in self.params_methods_mapper else \
             self.base_params_method
 
     def set_data(self, event_data, source):
         return self.event_model(**event_data)
 
-    @tracing
+    @ctracing
     async def send_data(self, event_data):
         event_data = event_data.dict()
         source = event_data.get('source')
         model = self.set_data(event_data, source)
         integrator_instances = {
             'web': self.web_integrator,
             'ios': self.ios_integrator,
```

### Comparing `velintegrator-1.0.4/velintegrator/sdk.py` & `velintegrator-1.0.5/velintegrator/sdk.py`

 * *Files identical despite different names*

### Comparing `velintegrator-1.0.4/velintegrator.egg-info/PKG-INFO` & `velintegrator-1.0.5/velintegrator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.0.4
+Version: 1.0.5
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 Kafka Client for VELI.STORE
```

