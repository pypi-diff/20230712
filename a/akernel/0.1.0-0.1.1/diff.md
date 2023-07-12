# Comparing `tmp/akernel-0.1.0.tar.gz` & `tmp/akernel-0.1.1.tar.gz`

## Comparing `akernel-0.1.0.tar` & `akernel-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 akernel-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 akernel-0.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/akernel.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/cache.py
--rw-r--r--   0        0        0     9111 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/code.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/connect.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/execution.py
--rw-r--r--   0        0        0    17853 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/kernel.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/kernelspec.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/message.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/traceback.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/IPython/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/IPython/core/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/IPython/core/getipython.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/IPython/core/interactiveshell.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/comm/__init__.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/comm/comm.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/comm/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/display/__init__.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/display/display.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/conftest.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/test_async_code.py
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/test_execution.py
--rw-r--r--   0        0        0     6748 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/test_kernel.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/test_react_code.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 akernel-0.1.0/binder/environment.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 akernel-0.1.0/binder/postBuild
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 akernel-0.1.0/examples/reactivity.ipynb
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 akernel-0.1.0/share/jupyter/kernels/akernel/kernel.json
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 akernel-0.1.0/LICENSE
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 akernel-0.1.0/README.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 akernel-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 akernel-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 akernel-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 akernel-0.1.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/akernel.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/cache.py
+-rw-r--r--   0        0        0     9111 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/code.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/connect.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/execution.py
+-rw-r--r--   0        0        0    17853 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/kernel.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/kernelspec.py
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/message.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/traceback.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/IPython/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/IPython/core/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/IPython/core/getipython.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/IPython/core/interactiveshell.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/comm/__init__.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/comm/comm.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/comm/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/display/__init__.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/display/display.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/conftest.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/test_async_code.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/test_execution.py
+-rw-r--r--   0        0        0     6748 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/test_kernel.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/test_react_code.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 akernel-0.1.1/binder/environment.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 akernel-0.1.1/binder/postBuild
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 akernel-0.1.1/examples/reactivity.ipynb
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 akernel-0.1.1/share/jupyter/kernels/akernel/kernel.json
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 akernel-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 akernel-0.1.1/README.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 akernel-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 akernel-0.1.1/PKG-INFO
```

### Comparing `akernel-0.1.0/.github/workflows/main.yml` & `akernel-0.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/akernel.py` & `akernel-0.1.1/akernel/akernel.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/code.py` & `akernel-0.1.1/akernel/code.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/connect.py` & `akernel-0.1.1/akernel/connect.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/execution.py` & `akernel-0.1.1/akernel/execution.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/kernel.py` & `akernel-0.1.1/akernel/kernel.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/kernelspec.py` & `akernel-0.1.1/akernel/kernelspec.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/message.py` & `akernel-0.1.1/akernel/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 protocol_version_info = (5, 3)
 protocol_version = "%i.%i" % protocol_version_info
 
 DELIM = b"<IDS|MSG>"
 
 
 def date_to_str(obj: Dict[str, Any]):
-    if "date" in obj and type(obj["date"]) != str:
+    if obj is not None and "date" in obj and type(obj["date"]) != str:
         obj["date"] = obj["date"].isoformat().replace("+00:00", "Z")
     return obj
 
 
 def utcnow() -> datetime:
     return datetime.utcnow().replace(tzinfo=timezone.utc)
```

### Comparing `akernel-0.1.0/akernel/traceback.py` & `akernel-0.1.1/akernel/traceback.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/comm/comm.py` & `akernel-0.1.1/akernel/comm/comm.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/tests/conftest.py` & `akernel-0.1.1/akernel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/tests/test_async_code.py` & `akernel-0.1.1/akernel/tests/test_async_code.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/tests/test_execution.py` & `akernel-0.1.1/akernel/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/tests/test_kernel.py` & `akernel-0.1.1/akernel/tests/test_kernel.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/akernel/tests/test_react_code.py` & `akernel-0.1.1/akernel/tests/test_react_code.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/examples/reactivity.ipynb` & `akernel-0.1.1/examples/reactivity.ipynb`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/LICENSE` & `akernel-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/README.md` & `akernel-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/pyproject.toml` & `akernel-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akernel-0.1.0/PKG-INFO` & `akernel-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akernel
-Version: 0.1.0
+Version: 0.1.1
 Summary: An asynchronous Python Jupyter kernel
 Project-URL: Homepage, https://github.com/davidbrochart/akernel
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: jupyter
 Classifier: Development Status :: 4 - Beta
```

