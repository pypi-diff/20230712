# Comparing `tmp/igrafx_mining_sdk-2.24.4.tar.gz` & `tmp/igrafx_mining_sdk-2.24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igrafx_mining_sdk-2.24.4.tar", last modified: Wed Jul 12 08:57:57 2023, max compression
+gzip compressed data, was "igrafx_mining_sdk-2.24.5.tar", last modified: Wed Jul 12 09:48:41 2023, max compression
```

## Comparing `igrafx_mining_sdk-2.24.4.tar` & `igrafx_mining_sdk-2.24.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:57:57.432300 igrafx_mining_sdk-2.24.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-12 08:57:57.432300 igrafx_mining_sdk-2.24.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:57:57.428300 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/column_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/workgroup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:57:57.428300 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-12 08:57:57.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-12 08:57:57.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:57:57.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 08:57:57.000000 igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 08:57:57.432300 igrafx_mining_sdk-2.24.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 08:57:37.000000 igrafx_mining_sdk-2.24.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:57:57.428300 igrafx_mining_sdk-2.24.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_column_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-12 08:57:35.000000 igrafx_mining_sdk-2.24.4/tests/test_workgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:48:41.660194 igrafx_mining_sdk-2.24.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-12 09:48:41.660194 igrafx_mining_sdk-2.24.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:48:41.656194 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/workgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:48:41.660194 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-12 09:48:41.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-12 09:48:41.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:48:41.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 09:48:41.000000 igrafx_mining_sdk-2.24.5/igrafx_mining_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:48:41.660194 igrafx_mining_sdk-2.24.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 09:48:22.000000 igrafx_mining_sdk-2.24.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:48:41.660194 igrafx_mining_sdk-2.24.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/tests/test_column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/tests/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-12 09:48:18.000000 igrafx_mining_sdk-2.24.5/tests/test_workgroup.py
```

### Comparing `igrafx_mining_sdk-2.24.4/LICENSE` & `igrafx_mining_sdk-2.24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/PKG-INFO` & `igrafx_mining_sdk-2.24.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igrafx_mining_sdk
-Version: 2.24.4
+Version: 2.24.5
 Summary: The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects.
 Home-page: https://www.logpickr.com/fr/accueil.html
 Author: iGrafx
 Author-email: contact@igrafx.com
 License: Apache License 2.0
 Description:
```

### Comparing `igrafx_mining_sdk-2.24.4/README.md` & `igrafx_mining_sdk-2.24.5/README.md`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/__init__.py` & `igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/api_connector.py` & `igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/api_connector.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/column_mapping.py` & `igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/datasource.py` & `igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/datasource.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/graph.py` & `igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/graph.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/project.py` & `igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/project.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk/workgroup.py` & `igrafx_mining_sdk-2.24.5/igrafx_mining_sdk/workgroup.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/PKG-INFO` & `igrafx_mining_sdk-2.24.5/igrafx_mining_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igrafx-mining-sdk
-Version: 2.24.4
+Version: 2.24.5
 Summary: The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects.
 Home-page: https://www.logpickr.com/fr/accueil.html
 Author: iGrafx
 Author-email: contact@igrafx.com
 License: Apache License 2.0
 Description:
```

### Comparing `igrafx_mining_sdk-2.24.4/igrafx_mining_sdk.egg-info/SOURCES.txt` & `igrafx_mining_sdk-2.24.5/igrafx_mining_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/pyproject.toml` & `igrafx_mining_sdk-2.24.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/setup.py` & `igrafx_mining_sdk-2.24.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 }
 
 # Extract requirements
 requirements = list(pyproject_data['tool']['poetry']['dependencies'].values())
 
 setup(
     name="igrafx_mining_sdk",
-    version='2.24.4',
+    version='2.24.5',
     description=package_infos['__doc__'],
     long_description=open("README.md", 'r').read(),
     long_description_content_type='text/markdown',
     url="https://www.logpickr.com/fr/accueil.html",
     author=package_infos['__author__'],
     author_email=package_infos['__email__'],
     packages=find_packages(),
```

### Comparing `igrafx_mining_sdk-2.24.4/tests/test_column_mapping.py` & `igrafx_mining_sdk-2.24.5/tests/test_column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/tests/test_datasource.py` & `igrafx_mining_sdk-2.24.5/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/tests/test_graph.py` & `igrafx_mining_sdk-2.24.5/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/tests/test_project.py` & `igrafx_mining_sdk-2.24.5/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.4/tests/test_workgroup.py` & `igrafx_mining_sdk-2.24.5/tests/test_workgroup.py`

 * *Files identical despite different names*

