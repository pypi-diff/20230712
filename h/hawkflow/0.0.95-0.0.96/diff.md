# Comparing `tmp/hawkflow-0.0.95.tar.gz` & `tmp/hawkflow-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/felbus/github/hawkflow-py/dist/.tmp-x40173fj/hawkflow-0.0.95.tar", last modified: Thu Jul  6 08:54:39 2023, max compression
+gzip compressed data, was "/Users/felbus/github/hawkflow-py/dist/.tmp-75olkjrc/hawkflow-0.0.96.tar", last modified: Wed Jul 12 09:15:54 2023, max compression
```

## Comparing `hawkflow-0.0.95.tar` & `hawkflow-0.0.96.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:54:39.000000 hawkflow-0.0.95/
--rw-r--r--   0 felbus     (501) staff       (20)     1054 2023-02-20 15:32:46.000000 hawkflow-0.0.95/LICENSE
--rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-06 08:54:39.000000 hawkflow-0.0.95/PKG-INFO
--rw-r--r--   0 felbus     (501) staff       (20)     1264 2023-03-15 18:47:38.000000 hawkflow-0.0.95/README.md
--rw-r--r--   0 felbus     (501) staff       (20)      843 2023-07-06 08:54:26.000000 hawkflow-0.0.95/pyproject.toml
--rw-r--r--   0 felbus     (501) staff       (20)       38 2023-07-06 08:54:39.000000 hawkflow-0.0.95/setup.cfg
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:54:39.000000 hawkflow-0.0.95/src/
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:54:39.000000 hawkflow-0.0.95/src/hawkflow.egg-info/
--rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-06 08:54:39.000000 hawkflow-0.0.95/src/hawkflow.egg-info/PKG-INFO
--rw-r--r--   0 felbus     (501) staff       (20)      510 2023-07-06 08:54:39.000000 hawkflow-0.0.95/src/hawkflow.egg-info/SOURCES.txt
--rw-r--r--   0 felbus     (501) staff       (20)        1 2023-07-06 08:54:39.000000 hawkflow-0.0.95/src/hawkflow.egg-info/dependency_links.txt
--rw-r--r--   0 felbus     (501) staff       (20)       17 2023-07-06 08:54:39.000000 hawkflow-0.0.95/src/hawkflow.egg-info/requires.txt
--rw-r--r--   0 felbus     (501) staff       (20)       15 2023-07-06 08:54:39.000000 hawkflow-0.0.95/src/hawkflow.egg-info/top_level.txt
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:54:39.000000 hawkflow-0.0.95/src/hawkflowclient/
--rw-r--r--   0 felbus     (501) staff       (20)      199 2023-03-03 15:13:44.000000 hawkflow-0.0.95/src/hawkflowclient/__init__.py
--rw-r--r--   0 felbus     (501) staff       (20)      910 2023-07-06 07:19:23.000000 hawkflow-0.0.95/src/hawkflowclient/_endpoints.py
--rw-r--r--   0 felbus     (501) staff       (20)     1045 2023-02-20 15:32:46.000000 hawkflow-0.0.95/src/hawkflowclient/_hawkflow_exceptions.py
--rw-r--r--   0 felbus     (501) staff       (20)     4980 2023-07-06 07:19:23.000000 hawkflow-0.0.95/src/hawkflowclient/_validation.py
--rw-r--r--   0 felbus     (501) staff       (20)     2724 2023-07-06 07:19:23.000000 hawkflow-0.0.95/src/hawkflowclient/hawkflow_api.py
--rw-r--r--   0 felbus     (501) staff       (20)     1816 2023-02-20 15:32:46.000000 hawkflow-0.0.95/src/hawkflowclient/hawkflow_decorators.py
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:54:39.000000 hawkflow-0.0.95/src/hawkflowclient/tests/
--rw-r--r--   0 felbus     (501) staff       (20)        0 2023-02-20 15:32:46.000000 hawkflow-0.0.95/src/hawkflowclient/tests/__init__.py
--rw-r--r--   0 felbus     (501) staff       (20)     8702 2023-07-06 07:14:36.000000 hawkflow-0.0.95/src/hawkflowclient/tests/test_validation.py
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-12 09:15:54.000000 hawkflow-0.0.96/
+-rw-r--r--   0 felbus     (501) staff       (20)     1054 2023-02-20 15:32:46.000000 hawkflow-0.0.96/LICENSE
+-rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-12 09:15:54.000000 hawkflow-0.0.96/PKG-INFO
+-rw-r--r--   0 felbus     (501) staff       (20)     1264 2023-03-15 18:47:38.000000 hawkflow-0.0.96/README.md
+-rw-r--r--   0 felbus     (501) staff       (20)      843 2023-07-12 09:15:25.000000 hawkflow-0.0.96/pyproject.toml
+-rw-r--r--   0 felbus     (501) staff       (20)       38 2023-07-12 09:15:54.000000 hawkflow-0.0.96/setup.cfg
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-12 09:15:54.000000 hawkflow-0.0.96/src/
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-12 09:15:54.000000 hawkflow-0.0.96/src/hawkflow.egg-info/
+-rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-12 09:15:54.000000 hawkflow-0.0.96/src/hawkflow.egg-info/PKG-INFO
+-rw-r--r--   0 felbus     (501) staff       (20)      510 2023-07-12 09:15:54.000000 hawkflow-0.0.96/src/hawkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 felbus     (501) staff       (20)        1 2023-07-12 09:15:54.000000 hawkflow-0.0.96/src/hawkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 felbus     (501) staff       (20)       17 2023-07-12 09:15:54.000000 hawkflow-0.0.96/src/hawkflow.egg-info/requires.txt
+-rw-r--r--   0 felbus     (501) staff       (20)       15 2023-07-12 09:15:54.000000 hawkflow-0.0.96/src/hawkflow.egg-info/top_level.txt
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-12 09:15:54.000000 hawkflow-0.0.96/src/hawkflowclient/
+-rw-r--r--   0 felbus     (501) staff       (20)      199 2023-03-03 15:13:44.000000 hawkflow-0.0.96/src/hawkflowclient/__init__.py
+-rw-r--r--   0 felbus     (501) staff       (20)      910 2023-07-06 07:19:23.000000 hawkflow-0.0.96/src/hawkflowclient/_endpoints.py
+-rw-r--r--   0 felbus     (501) staff       (20)     1045 2023-02-20 15:32:46.000000 hawkflow-0.0.96/src/hawkflowclient/_hawkflow_exceptions.py
+-rw-r--r--   0 felbus     (501) staff       (20)     5009 2023-07-12 09:15:25.000000 hawkflow-0.0.96/src/hawkflowclient/_validation.py
+-rw-r--r--   0 felbus     (501) staff       (20)     2724 2023-07-06 07:19:23.000000 hawkflow-0.0.96/src/hawkflowclient/hawkflow_api.py
+-rw-r--r--   0 felbus     (501) staff       (20)     1816 2023-02-20 15:32:46.000000 hawkflow-0.0.96/src/hawkflowclient/hawkflow_decorators.py
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-12 09:15:54.000000 hawkflow-0.0.96/src/hawkflowclient/tests/
+-rw-r--r--   0 felbus     (501) staff       (20)        0 2023-02-20 15:32:46.000000 hawkflow-0.0.96/src/hawkflowclient/tests/__init__.py
+-rw-r--r--   0 felbus     (501) staff       (20)     8702 2023-07-06 07:14:36.000000 hawkflow-0.0.96/src/hawkflowclient/tests/test_validation.py
```

### Comparing `hawkflow-0.0.95/LICENSE` & `hawkflow-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.95/PKG-INFO` & `hawkflow-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hawkflow
-Version: 0.0.95
+Version: 0.0.96
 Summary: HawkFlow.ai
 License: LICENSE
 Project-URL: Homepage, https://github.com/hawkflow/hawkflow-py
 Keywords: hawkflow,hawkflowclient,monitoring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hawkflow-0.0.95/README.md` & `hawkflow-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.95/pyproject.toml` & `hawkflow-0.0.96/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="hawkflow"
-version="0.0.95"
+version="0.0.96"
 description="HawkFlow.ai"
 readme = "README.md"
 keywords=["hawkflow", "hawkflowclient", "monitoring"]
 license = {text = "LICENSE"}
 requires-python = ">=3.7"
 dependencies=[
     "requests>=2.25.1"
```

### Comparing `hawkflow-0.0.95/src/hawkflow.egg-info/PKG-INFO` & `hawkflow-0.0.96/src/hawkflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hawkflow
-Version: 0.0.95
+Version: 0.0.96
 Summary: HawkFlow.ai
 License: LICENSE
 Project-URL: Homepage, https://github.com/hawkflow/hawkflow-py
 Keywords: hawkflow,hawkflowclient,monitoring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hawkflow-0.0.95/src/hawkflowclient/_endpoints.py` & `hawkflow-0.0.96/src/hawkflowclient/_endpoints.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.95/src/hawkflowclient/_hawkflow_exceptions.py` & `hawkflow-0.0.96/src/hawkflowclient/_hawkflow_exceptions.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.95/src/hawkflowclient/_validation.py` & `hawkflow-0.0.96/src/hawkflowclient/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,26 +69,26 @@
     if process == "":
         raise HawkFlowDataTypesException("process parameter cannot be empty")
 
     if len(process) > 249:
         raise HawkFlowDataTypesException("process parameter exceeded max length of 250")
 
     if not re.match(PROCESS_REGEX, process):
-        raise HawkFlowDataTypesException("process parameter contains illegal characters")
+        raise HawkFlowDataTypesException(f"process parameter: {process} contains illegal characters")
 
 
 def _validate_meta(meta):
     if not isinstance(meta, str):
         raise HawkFlowDataTypesException("meta parameter must be type str")
 
     if len(meta) > 499:
         raise HawkFlowDataTypesException("meta parameter exceeded max length of 500")
 
     if not re.match(META_REGEX, meta):
-        raise HawkFlowDataTypesException("meta parameter contains illegal characters")
+        raise HawkFlowDataTypesException(f"meta parameter: {meta} contains illegal characters")
 
 
 def _validate_exception_text(exception_text):
     if not isinstance(exception_text, str):
         raise HawkFlowDataTypesException("exception_text parameter must be type str")
 
     if len(exception_text) > 15000:
@@ -105,15 +105,15 @@
         if not isinstance(key, str) or (not isinstance(items[key], int) and not isinstance(items[key], float)):
             raise HawkFlowDataTypesException(_metric_text)
 
         if key == "":
             raise HawkFlowDataTypesException("metric items parameter dictionary key cannot be empty")
 
         if not re.match(METRIC_KEY_REGEX, key):
-            raise HawkFlowDataTypesException("metric items parameter dictionary key contains illegal characters")
+            raise HawkFlowDataTypesException(f"metric items parameter dictionary key: {key} contains illegal characters")
 
 
 def _validate_metric_items_df(items):
     _metric_text = "metric items df parameter should be a dict {STR:{str:FLOAT or INT}, {str:FLOAT or INT}}"
 
     if not isinstance(items, dict):
         raise HawkFlowDataTypesException("metric items parameter must be type dict {STR:FLOAT or INT}")
```

### Comparing `hawkflow-0.0.95/src/hawkflowclient/hawkflow_api.py` & `hawkflow-0.0.96/src/hawkflowclient/hawkflow_api.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.95/src/hawkflowclient/hawkflow_decorators.py` & `hawkflow-0.0.96/src/hawkflowclient/hawkflow_decorators.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.95/src/hawkflowclient/tests/test_validation.py` & `hawkflow-0.0.96/src/hawkflowclient/tests/test_validation.py`

 * *Files identical despite different names*

