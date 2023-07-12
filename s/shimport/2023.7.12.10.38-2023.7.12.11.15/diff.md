# Comparing `tmp/shimport-2023.7.12.10.38.tar.gz` & `tmp/shimport-2023.7.12.11.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shimport-2023.7.12.10.38.tar", last modified: Wed Jul 12 10:38:25 2023, max compression
+gzip compressed data, was "shimport-2023.7.12.11.15.tar", last modified: Wed Jul 12 11:15:45 2023, max compression
```

## Comparing `shimport-2023.7.12.10.38.tar` & `shimport-2023.7.12.11.15.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:38:25.728232 shimport-2023.7.12.10.38/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-12 10:38:25.728232 shimport-2023.7.12.10.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-12 10:38:25.732232 shimport-2023.7.12.10.38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:38:25.720231 shimport-2023.7.12.10.38/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:38:25.724232 shimport-2023.7.12.10.38/src/shimport/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 10:38:21.000000 shimport-2023.7.12.10.38/src/shimport/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:38:25.728232 shimport-2023.7.12.10.38/src/shimport/abcs/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/abcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/abcs/attrdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/abcs.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-12 10:38:14.000000 shimport-2023.7.12.10.38/src/shimport/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/module.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:38:25.728232 shimport-2023.7.12.10.38/src/shimport/util/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 10:37:32.000000 shimport-2023.7.12.10.38/src/shimport/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 10:38:14.000000 shimport-2023.7.12.10.38/src/shimport/util/lme.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-12 10:38:14.000000 shimport-2023.7.12.10.38/src/shimport/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:38:25.728232 shimport-2023.7.12.10.38/src/shimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-12 10:38:25.000000 shimport-2023.7.12.10.38/src/shimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 10:38:25.000000 shimport-2023.7.12.10.38/src/shimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:38:25.000000 shimport-2023.7.12.10.38/src/shimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:38:25.000000 shimport-2023.7.12.10.38/src/shimport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 10:38:25.000000 shimport-2023.7.12.10.38/src/shimport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 10:38:25.000000 shimport-2023.7.12.10.38/src/shimport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:15:45.525638 shimport-2023.7.12.11.15/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 11:15:45.525638 shimport-2023.7.12.11.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-12 11:15:45.525638 shimport-2023.7.12.11.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:15:45.521638 shimport-2023.7.12.11.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:15:45.521638 shimport-2023.7.12.11.15/src/shimport/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 11:15:40.000000 shimport-2023.7.12.11.15/src/shimport/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:15:45.525638 shimport-2023.7.12.11.15/src/shimport/abcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/abcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/abcs/attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/abcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-12 11:15:34.000000 shimport-2023.7.12.11.15/src/shimport/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:15:45.525638 shimport-2023.7.12.11.15/src/shimport/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 11:14:50.000000 shimport-2023.7.12.11.15/src/shimport/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-12 11:15:34.000000 shimport-2023.7.12.11.15/src/shimport/util/lme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-12 11:15:34.000000 shimport-2023.7.12.11.15/src/shimport/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:15:45.525638 shimport-2023.7.12.11.15/src/shimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 11:15:45.000000 shimport-2023.7.12.11.15/src/shimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 11:15:45.000000 shimport-2023.7.12.11.15/src/shimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:15:45.000000 shimport-2023.7.12.11.15/src/shimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:15:45.000000 shimport-2023.7.12.11.15/src/shimport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 11:15:45.000000 shimport-2023.7.12.11.15/src/shimport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 11:15:45.000000 shimport-2023.7.12.11.15/src/shimport.egg-info/top_level.txt
```

### Comparing `shimport-2023.7.12.10.38/PKG-INFO` & `shimport-2023.7.12.11.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: shimport
-Version: 2023.7.12.10.38
-Summary: Autodocs for python projects
+Version: 2023.7.12.11.15
+Summary: Import tools for python projects
 Home-page: https://github.com/elo-enterprises/shimport/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/shimport/
 Project-URL: Source, https://github.com/elo-enterprises/shimport/
 Project-URL: Download, https://github.com/elo-enterprises/shimport/#files
 Platform: any
 Classifier: Programming Language :: Python
-Requires-Python: >3.6
+Requires-Python: >3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: testing
 Provides-Extra: lint
 Provides-Extra: publish
 
 See the project README
```

### Comparing `shimport-2023.7.12.10.38/setup.cfg` & `shimport-2023.7.12.11.15/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shimport
-description = Autodocs for python projects
+description = Import tools for python projects
 author = elo
 platforms = any
 license = MIT
 license_files = LICENSE.txt
 long_description = See the project README
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/elo-enterprises/shimport/
@@ -18,15 +18,15 @@
 [options]
 zip_safe = False
 zip_ok = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
-python_requires = >3.6
+python_requires = >3.7
 install_requires = 
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `shimport-2023.7.12.10.38/setup.py` & `shimport-2023.7.12.11.15/setup.py`

 * *Files identical despite different names*

### Comparing `shimport-2023.7.12.10.38/src/shimport/__init__.py` & `shimport-2023.7.12.11.15/src/shimport/__init__.py`

 * *Files identical despite different names*

### Comparing `shimport-2023.7.12.10.38/src/shimport/abcs/__init__.py` & `shimport-2023.7.12.11.15/src/shimport/abcs/__init__.py`

 * *Files identical despite different names*

### Comparing `shimport-2023.7.12.10.38/src/shimport/abcs/attrdict.py` & `shimport-2023.7.12.11.15/src/shimport/abcs/attrdict.py`

 * *Files identical despite different names*

### Comparing `shimport-2023.7.12.10.38/src/shimport/abcs.py` & `shimport-2023.7.12.11.15/src/shimport/abcs.py`

 * *Files identical despite different names*

### Comparing `shimport-2023.7.12.10.38/src/shimport/models.py` & `shimport-2023.7.12.11.15/src/shimport/models.py`

 * *Files identical despite different names*

### Comparing `shimport-2023.7.12.10.38/src/shimport/module.py` & `shimport-2023.7.12.11.15/src/shimport/module.py`

 * *Files identical despite different names*

### Comparing `shimport-2023.7.12.10.38/src/shimport/util/lme.py` & `shimport-2023.7.12.11.15/src/shimport/util/lme.py`

 * *Files identical despite different names*

### Comparing `shimport-2023.7.12.10.38/src/shimport/util/typing.py` & `shimport-2023.7.12.11.15/src/shimport/util/typing.py`

 * *Files identical despite different names*

### Comparing `shimport-2023.7.12.10.38/src/shimport.egg-info/PKG-INFO` & `shimport-2023.7.12.11.15/src/shimport.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: shimport
-Version: 2023.7.12.10.38
-Summary: Autodocs for python projects
+Version: 2023.7.12.11.15
+Summary: Import tools for python projects
 Home-page: https://github.com/elo-enterprises/shimport/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/shimport/
 Project-URL: Source, https://github.com/elo-enterprises/shimport/
 Project-URL: Download, https://github.com/elo-enterprises/shimport/#files
 Platform: any
 Classifier: Programming Language :: Python
-Requires-Python: >3.6
+Requires-Python: >3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: testing
 Provides-Extra: lint
 Provides-Extra: publish
 
 See the project README
```

### Comparing `shimport-2023.7.12.10.38/src/shimport.egg-info/SOURCES.txt` & `shimport-2023.7.12.11.15/src/shimport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

