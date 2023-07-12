# Comparing `tmp/iotcore_api-1.1.5.tar.gz` & `tmp/iotcore_api-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotcore_api-1.1.5.tar", max compression
+gzip compressed data, was "iotcore_api-1.1.6.tar", max compression
```

## Comparing `iotcore_api-1.1.5.tar` & `iotcore_api-1.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.5/iotcoreapi/__init__.py
--rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.5/iotcoreapi/exceptions.py
--rw-r--r--   0        0        0    57644 2023-07-11 14:53:11.875194 iotcore_api-1.1.5/iotcoreapi/iotcoreapi.py
--rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.5/iotcoreapi/nan_treatment.py
--rw-r--r--   0        0        0      743 2023-07-11 14:55:54.845157 iotcore_api-1.1.5/pyproject.toml
--rw-r--r--   0        0        0    33781 2023-07-11 14:57:06.239918 iotcore_api-1.1.5/README.md
--rw-r--r--   0        0        0    34163 1970-01-01 00:00:00.000000 iotcore_api-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.6/iotcoreapi/__init__.py
+-rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.6/iotcoreapi/exceptions.py
+-rw-r--r--   0        0        0    57644 2023-07-11 14:53:11.875194 iotcore_api-1.1.6/iotcoreapi/iotcoreapi.py
+-rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.6/iotcoreapi/nan_treatment.py
+-rw-r--r--   0        0        0      865 2023-07-12 10:12:34.876701 iotcore_api-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0    33781 2023-07-11 14:57:06.239918 iotcore_api-1.1.6/README.md
+-rw-r--r--   0        0        0    34237 1970-01-01 00:00:00.000000 iotcore_api-1.1.6/PKG-INFO
```

### Comparing `iotcore_api-1.1.5/iotcoreapi/exceptions.py` & `iotcore_api-1.1.6/iotcoreapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.5/iotcoreapi/iotcoreapi.py` & `iotcore_api-1.1.6/iotcoreapi/iotcoreapi.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.5/iotcoreapi/nan_treatment.py` & `iotcore_api-1.1.6/iotcoreapi/nan_treatment.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.5/pyproject.toml` & `iotcore_api-1.1.6/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "iotcore-api"
-version = "1.1.5"
-description ="IoT core connection methods and utilities"
+version = "1.1.6"
+description ="IoT core connection methods and utilities in Python"
+authors = ["Ricardo Gomez-Aldaravi <ricardo.gomez.aldaravi@idrica.com>", "Laura Moreno <laura.moreno@idrica.com>"]
 readme = "README.md"
 packages = [
     {include = 'iotcoreapi/*.py'}
 ]
-authors = ["Idrica"]
 keywords = ["iotcoreapi", "goaigua"]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^2.0.1"
@@ -23,11 +23,12 @@
 mkdocs = "^1.4.2"
 mkdocstrings = "^0.20.0"
 mkdocs-material = "^9.1.3"
 mkdocstrings-python = "^0.8.3"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 mkdocs-pdf-export-plugin = "^0.5.10"
 pre-commit = "^3.3.2"
+toml = "^0.10.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `iotcore_api-1.1.5/README.md` & `iotcore_api-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.5/PKG-INFO` & `iotcore_api-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: iotcore-api
-Version: 1.1.5
-Summary: IoT core connection methods and utilities
+Version: 1.1.6
+Summary: IoT core connection methods and utilities in Python
 Keywords: iotcoreapi,goaigua
-Author: Idrica
+Author: Ricardo Gomez-Aldaravi
+Author-email: ricardo.gomez.aldaravi@idrica.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
```

