# Comparing `tmp/onedata_lambda_utils-0.1.2.tar.gz` & `tmp/onedata_lambda_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onedata_lambda_utils-0.1.2.tar", last modified: Wed Feb 22 21:51:21 2023, max compression
+gzip compressed data, was "onedata_lambda_utils-0.2.0.tar", last modified: Wed Jul 12 16:31:41 2023, max compression
```

## Comparing `onedata_lambda_utils-0.1.2.tar` & `onedata_lambda_utils-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 rwidzisz  (1000) rwidzisz  (1000)        0 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)     1256 2023-02-22 21:49:26.000000 onedata_lambda_utils-0.1.2/setup.py
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)      223 2023-02-22 21:49:26.000000 onedata_lambda_utils-0.1.2/README.md
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)       24 2023-02-22 21:49:26.000000 onedata_lambda_utils-0.1.2/MANIFEST.in
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)       38 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/setup.cfg
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)     1102 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/PKG-INFO
-drwxrwxr-x   0 rwidzisz  (1000) rwidzisz  (1000)        0 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils.egg-info/
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)      406 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)       21 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils.egg-info/top_level.txt
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)       25 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils.egg-info/requires.txt
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)     1102 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils.egg-info/PKG-INFO
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)        1 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils.egg-info/dependency_links.txt
-drwxrwxr-x   0 rwidzisz  (1000) rwidzisz  (1000)        0 2023-02-22 21:51:21.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils/
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)        0 2023-02-22 21:50:56.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils/py.typed
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)     1618 2023-02-22 21:50:56.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils/stats.py
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)        0 2023-02-22 21:50:56.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils/__init__.py
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)     5891 2023-02-22 21:50:56.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils/types.py
--rw-rw-r--   0 rwidzisz  (1000) rwidzisz  (1000)     1186 2023-02-22 21:50:56.000000 onedata_lambda_utils-0.1.2/onedata_lambda_utils/streaming.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:31:41.125808 onedata_lambda_utils-0.2.0/
+-rw-rw-r--   0 root         (0) root         (0)     1158 2023-02-03 12:50:29.000000 onedata_lambda_utils-0.2.0/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-02-22 21:49:26.000000 onedata_lambda_utils-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-07-12 16:31:41.125808 onedata_lambda_utils-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      595 2023-07-12 08:06:59.000000 onedata_lambda_utils-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:31:41.125808 onedata_lambda_utils-0.2.0/onedata_lambda_utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-02-22 21:50:56.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2328 2023-07-07 09:28:19.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils/logging.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-02-22 21:50:56.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils/py.typed
+-rw-rw-r--   0 root         (0) root         (0)     1618 2023-02-22 21:50:56.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils/stats.py
+-rw-rw-r--   0 root         (0) root         (0)     1228 2023-07-06 14:36:39.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils/streaming.py
+-rw-rw-r--   0 root         (0) root         (0)     5904 2023-07-06 14:36:39.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:31:41.125808 onedata_lambda_utils-0.2.0/onedata_lambda_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-07-12 16:31:41.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-12 16:31:41.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 16:31:41.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-12 16:31:41.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 16:31:41.000000 onedata_lambda_utils-0.2.0/onedata_lambda_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 16:31:41.125808 onedata_lambda_utils-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1256 2023-07-10 13:24:54.000000 onedata_lambda_utils-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `onedata_lambda_utils-0.1.2/setup.py` & `onedata_lambda_utils-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="onedata_lambda_utils",
-    version="0.1.2",
+    version="0.2.0",
     python_requires=">=3.7",
     description="Python Library containing utility functions for use in OpenFaaS lambda implementations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rafal Widziszewski",
     license="MIT",
     classifiers=[
```

### Comparing `onedata_lambda_utils-0.1.2/PKG-INFO` & `onedata_lambda_utils-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: onedata_lambda_utils
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python Library containing utility functions for use in OpenFaaS lambda implementations
-Home-page: UNKNOWN
 Author: Rafal Widziszewski
 License: MIT
-Description: onedata-lambda-utils
-        ========================
-        Python Library containing utility functions for use in OpenFaaS lambda implementations
-        
-        ## Installation
-        
-        Installation:
-        ```bash
-           python -m pip install onedata_lambda_utils
-        ```
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+onedata-lambda-utils
+========================
+Python Library containing utility functions for use in OpenFaaS lambda implementations
+
+## Installation
+
+Installation:
+```bash
+   python -m pip install onedata_lambda_utils
+```
+
+## Compatibility
+
+Specific `onedata-lambda-utils` releases are intended to be used only with compatible Oneprovider versions:
+
+| Oneprovider version | Compatible python library versions |
+|---------------------|------------------------------------|
+| `21.02.3`+          | `0.2.x`                            |
+| `21.02.1 - 21.02.2` | `0.1.x`                            |
```

### Comparing `onedata_lambda_utils-0.1.2/onedata_lambda_utils.egg-info/PKG-INFO` & `onedata_lambda_utils-0.2.0/onedata_lambda_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: onedata-lambda-utils
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python Library containing utility functions for use in OpenFaaS lambda implementations
-Home-page: UNKNOWN
 Author: Rafal Widziszewski
 License: MIT
-Description: onedata-lambda-utils
-        ========================
-        Python Library containing utility functions for use in OpenFaaS lambda implementations
-        
-        ## Installation
-        
-        Installation:
-        ```bash
-           python -m pip install onedata_lambda_utils
-        ```
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+onedata-lambda-utils
+========================
+Python Library containing utility functions for use in OpenFaaS lambda implementations
+
+## Installation
+
+Installation:
+```bash
+   python -m pip install onedata_lambda_utils
+```
+
+## Compatibility
+
+Specific `onedata-lambda-utils` releases are intended to be used only with compatible Oneprovider versions:
+
+| Oneprovider version | Compatible python library versions |
+|---------------------|------------------------------------|
+| `21.02.3`+          | `0.2.x`                            |
+| `21.02.1 - 21.02.2` | `0.1.x`                            |
```

### Comparing `onedata_lambda_utils-0.1.2/onedata_lambda_utils/stats.py` & `onedata_lambda_utils-0.2.0/onedata_lambda_utils/stats.py`

 * *Files identical despite different names*

### Comparing `onedata_lambda_utils-0.1.2/onedata_lambda_utils/types.py` & `onedata_lambda_utils-0.2.0/onedata_lambda_utils/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     rootFileDeleted: bool
     protectionFlags: List[ProtectionFlag]
     effectiveProtectionFlags: List[ProtectionFlag]
     creationTime: int
     archiveCount: int
 
 
-class AtmFile(TypedDict):
+class AtmFile(TypedDict, total=False):
     """
     JSON object describing a file in Onedata filesystem.
 
     Refer to the API specification for more information:
     https://onedata.org/#/home/api/latest/oneprovider?anchor=operation/get_attrs
     """
```

### Comparing `onedata_lambda_utils-0.1.2/onedata_lambda_utils/streaming.py` & `onedata_lambda_utils-0.2.0/onedata_lambda_utils/streaming.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,11 +28,14 @@
 
         super().__init__()
 
     def stream_item(self, item: T) -> None:
         self.stream_items([item])
 
     def stream_items(self, items: Iterable[T]) -> None:
+        if not items:
+            return
+
         with self._synchronized_context, open(f"/out/{self.result_name}", "a") as f:
             for item in items:
                 json.dump(item, f)
                 f.write("\n")
```

