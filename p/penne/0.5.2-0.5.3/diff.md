# Comparing `tmp/penne-0.5.2.tar.gz` & `tmp/penne-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penne-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "penne-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `penne-0.5.2.tar` & `penne-0.5.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1550 2023-07-12 15:53:26.029546 penne-0.5.2/README.md
--rw-r--r--   0        0        0      564 2023-07-12 15:53:26.205548 penne-0.5.2/penne/__init__.py
--rw-r--r--   0        0        0    13202 2023-07-12 15:53:26.205548 penne-0.5.2/penne/core.py
--rw-r--r--   0        0        0    44275 2023-07-12 15:53:26.205548 penne-0.5.2/penne/delegates.py
--rw-r--r--   0        0        0     4823 2023-07-12 15:53:26.205548 penne-0.5.2/penne/handlers.py
--rw-r--r--   0        0        0      893 2023-07-12 15:53:26.205548 penne-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 penne-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1550 2023-07-12 17:47:01.394371 penne-0.5.3/README.md
+-rw-r--r--   0        0        0      564 2023-07-12 17:47:01.610380 penne-0.5.3/penne/__init__.py
+-rw-r--r--   0        0        0    13204 2023-07-12 17:47:01.610380 penne-0.5.3/penne/core.py
+-rw-r--r--   0        0        0    44375 2023-07-12 17:47:01.610380 penne-0.5.3/penne/delegates.py
+-rw-r--r--   0        0        0     4823 2023-07-12 17:47:01.610380 penne-0.5.3/penne/handlers.py
+-rw-r--r--   0        0        0      893 2023-07-12 17:47:01.610380 penne-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 penne-0.5.3/PKG-INFO
```

### Comparing `penne-0.5.2/README.md` & `penne-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `penne-0.5.2/penne/__init__.py` & `penne-0.5.3/penne/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 Modules:
     core.py
     test_delegates.py
     handlers.py
     messages.py
 """
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 
 # Imports for easier user access
 from .core import Client
 from .delegates import *
```

### Comparing `penne-0.5.2/penne/core.py` & `penne-0.5.3/penne/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
             target_delegate = self.state[delegates.PlotID(*plot)]
         else:
             raise ValueError("Couldn't get delegate from context")
 
         return target_delegate
 
     def invoke_method(self, method: Union[delegates.MethodID, str], args: list = None,
-                      context: dict[str, tuple] = None, on_done=None):
+                      context: dict[str, tuple] = None, callback=None):
         """Invoke method on server
 
         Constructs a dictionary of arguments to use in send_message. The
         Dictionary follows the structure of an InvokeMethodMessage, but
         using a dictionary prevents from converting back and forth just
         before sending.
 
@@ -290,15 +290,15 @@
             method_id = method
 
         # Get invoke ID
         invoke_id = str(self._current_invoke)
         self._current_invoke += 1
 
         # Keep track of callback
-        self.callback_map[invoke_id] = on_done
+        self.callback_map[invoke_id] = callback
 
         # Construct message dict
         arg_dict = {
             "method": method_id,
             "args": args,
             "invoke_id": invoke_id
         }
```

### Comparing `penne-0.5.2/penne/delegates.py` & `penne-0.5.3/penne/delegates.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,17 @@
             the method's delegate
     """
 
     def __init__(self, object_delegate: Delegate, method_delegate: Method):
         self._obj_delegate = object_delegate
         self._method_delegate = method_delegate
 
-    def __call__(self, on_done=None, *arguments):
-        self._method_delegate.invoke(self._obj_delegate, list(arguments), callback=on_done)
+    def __call__(self, *args, **kwargs):
+        callback = kwargs.pop("callback", None)
+        self._method_delegate.invoke(self._obj_delegate, list(args), callback=callback)
 
 
 def inject_methods(delegate: Delegate, methods: List[MethodID]):
     """Inject methods into a delegate class
 
     Idea is to inject a method that is from the server to put into a delegate.
     Now it looks like the delegate has an instance method that actually calls what
@@ -738,15 +739,15 @@
             kind = "plot"
         elif isinstance(on_delegate, Entity):
             kind = "entity"
         else:
             raise ValueError("Invalid delegate context")
 
         context = {kind: on_delegate.id}
-        self.client.invoke_method(self.id, args, context=context, on_done=callback)
+        self.client.invoke_method(self.id, args, context=context, callback=callback)
 
     def __str__(self) -> str:
         """Custom string representation for methods"""
 
         rep = f"{self.name}:\n\t{self.doc}\n\tReturns: {self.return_doc}\n\tArgs:"
         for arg in self.arg_doc:
             rep += f"\n\t\t{arg.name}: {arg.doc}"
@@ -1110,27 +1111,27 @@
         self.signals = {
             "noo::tbl_reset": self._reset_table,
             "noo::tbl_rows_removed": self._remove_rows,
             "noo::tbl_updated": self._update_rows,
             "noo::tbl_selection_updated": self._update_selection
         }
 
-    def _on_table_init(self, init_info: dict, on_done=None):
+    def _on_table_init(self, init_info: dict, callback=None):
         """Creates table from server response info
 
         Args:
             init_info (Message Obj): 
                 Server response to subscribe which has columns, keys, data, 
                 and possibly selections
         """
 
         init = TableInitData(**init_info)
         logging.info(f"Table Initialized with cols: {init.columns} and row data: {init.data}")
-        if on_done:
-            on_done()
+        if callback:
+            callback()
 
     def _reset_table(self, init_info: dict = None):
         """Reset dataframe and selections to blank objects
 
         Method is linked to 'tbl_reset' signal
         """
 
@@ -1223,106 +1224,106 @@
         # Inject methods and signals
         if methods:
             inject_methods(self, methods)
         if signals:
             inject_signals(self, signals)
         self.relink_signals()
 
-    def subscribe(self, on_done: Callable = None):
+    def subscribe(self, callback: Callable = None):
         """Subscribe to this delegate's table
 
         Calls on_table_init as callback
 
         Args:
-              on_done (Callable): function to be called after table is subscribed to and initialized
+              callback (Callable): function to be called after table is subscribed to and initialized
 
         Raises:
             Exception: Could not subscribe to table
         """
 
         try:
             # Allow for callback after table init
-            self.tbl_subscribe(on_done=lambda data: self._on_table_init(data, on_done))
+            self.tbl_subscribe(callback=lambda data: self._on_table_init(data, callback))
         except Exception as e:
             raise Exception(f"Could not subscribe to table {self.id}...{e}")
 
-    def request_insert(self, row_list: List[List[int]], on_done=None):
+    def request_insert(self, row_list: List[List[int]], callback=None):
         """Add rows to end of table
 
         User endpoint for interacting with table and invoking method
         For input, row list is list of rows. Also note that tables have
         nine columns by default (x, y, z, r, g, b, sx, sy, sz).
         x, y, z -> coordinates
         r, g, b -> color values [0, 1]
         sx, sy, sz -> scaling factors, default size is 1 meter
 
         Row_list: [[1, 2, 3, 4, 5, 6, 7, 8, 9]]
 
         Args:
             row_list (list, optional): add rows using list of rows
-            on_done (function, optional): callback function
+            callback (function, optional): callback function
         """
 
-        self.tbl_insert(on_done, row_list)
+        self.tbl_insert(row_list, callback=callback)
 
-    def request_update(self, keys: List[int], rows: List[List[int]], on_done=None):
+    def request_update(self, keys: List[int], rows: List[List[int]], callback=None):
         """Update the table using a DataFrame
 
         User endpoint for interacting with table and invoking method
 
         Args:
             keys (list[int]):
                 list of keys to update
             rows (list[list[int]]):
                 list of new rows to update with
-            on_done (function, optional): 
+            callback (function, optional):
                 callback function called when complete
         """
 
-        self.tbl_update(on_done, keys, rows)
+        self.tbl_update(keys, rows, callback=callback)
 
-    def request_remove(self, keys: List[int], on_done=None):
+    def request_remove(self, keys: List[int], callback=None):
         """Remove rows from table by their keys
 
         User endpoint for interacting with table and invoking method
 
         Args:
             keys (list):
                 list of keys for rows to be removed
-            on_done (function, optional): 
+            callback (function, optional):
                 callback function called when complete
         """
 
-        self.tbl_remove(on_done, keys)
+        self.tbl_remove(keys, callback=callback)
 
-    def request_clear(self, on_done=None):
+    def request_clear(self, callback=None):
         """Clear the table
 
         User endpoint for interacting with table and invoking method
 
         Args:
-            on_done (function, optional): callback function called when complete
+            callback (function, optional): callback function called when complete
         """
-        self.tbl_clear(on_done)
+        self.tbl_clear(callback=callback)
 
-    def request_update_selection(self, name: str, keys: List[int], on_done=None):
+    def request_update_selection(self, name: str, keys: List[int], callback=None):
         """Update a selection object in the table
 
         User endpoint for interacting with table and invoking method
 
         Args:
             name (str):
                 name of the selection object to be updated
             keys (list):
                 list of keys to be in new selection
-            on_done (function, optional): 
+            callback (function, optional):
                 callback function called when complete
         """
         selection = Selection(name=name, rows=keys)
-        self.tbl_update_selection(on_done, selection.model_dump())
+        self.tbl_update_selection(selection.model_dump(), callback=callback)
 
     def show_methods(self):
         """Show methods available on the table"""
 
         if self.methods_list is None:
             message = "No methods available"
         else:
```

### Comparing `penne-0.5.2/penne/handlers.py` & `penne-0.5.3/penne/handlers.py`

 * *Files identical despite different names*

### Comparing `penne-0.5.2/pyproject.toml` & `penne-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `penne-0.5.2/PKG-INFO` & `penne-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penne
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python Client Library for NOODLES Protocol
 Keywords: noodles,cbor,Websockets,client,NOODLES
 Author: Alex Racapé
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

