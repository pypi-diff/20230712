# Comparing `tmp/anyjson2csv-0.0.1.tar.gz` & `tmp/anyjson2csv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyjson2csv-0.0.1.tar", last modified: Wed Jul 12 10:48:08 2023, max compression
+gzip compressed data, was "anyjson2csv-0.0.2.tar", last modified: Wed Jul 12 11:29:21 2023, max compression
```

## Comparing `anyjson2csv-0.0.1.tar` & `anyjson2csv-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 10:48:08.494524 anyjson2csv-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-07-12 08:57:26.000000 anyjson2csv-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      526 2023-07-12 10:48:08.492520 anyjson2csv-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-12 08:55:33.000000 anyjson2csv-0.0.1/README.md
--rw-rw-rw-   0        0        0      626 2023-07-12 10:46:45.000000 anyjson2csv-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 10:48:08.494524 anyjson2csv-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 10:48:08.394520 anyjson2csv-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 10:48:08.461524 anyjson2csv-0.0.1/src/anyjson2csv.egg-info/
--rw-rw-rw-   0        0        0      526 2023-07-12 10:48:08.000000 anyjson2csv-0.0.1/src/anyjson2csv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-07-12 10:48:08.000000 anyjson2csv-0.0.1/src/anyjson2csv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 10:48:08.000000 anyjson2csv-0.0.1/src/anyjson2csv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 10:48:08.000000 anyjson2csv-0.0.1/src/anyjson2csv.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 10:48:08.484522 anyjson2csv-0.0.1/src/json2csv/
--rw-rw-rw-   0        0        0       45 2023-07-12 08:51:33.000000 anyjson2csv-0.0.1/src/json2csv/__init__.py
--rw-rw-rw-   0        0        0     3446 2023-07-12 10:02:58.000000 anyjson2csv-0.0.1/src/json2csv/flatten_json.py
--rw-rw-rw-   0        0        0      686 2023-07-12 08:51:27.000000 anyjson2csv-0.0.1/src/json2csv/json_to_csv.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:29:21.447466 anyjson2csv-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-07-12 08:57:26.000000 anyjson2csv-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      526 2023-07-12 11:29:21.445469 anyjson2csv-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:55:33.000000 anyjson2csv-0.0.2/README.md
+-rw-rw-rw-   0        0        0      626 2023-07-12 11:27:35.000000 anyjson2csv-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:29:21.448465 anyjson2csv-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 11:29:21.378466 anyjson2csv-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 11:29:21.401467 anyjson2csv-0.0.2/src/anyjson2csv/
+-rw-rw-rw-   0        0        0        2 2023-07-12 11:27:26.000000 anyjson2csv-0.0.2/src/anyjson2csv/__init__.py
+-rw-rw-rw-   0        0        0     3446 2023-07-12 10:02:58.000000 anyjson2csv-0.0.2/src/anyjson2csv/flatten_json.py
+-rw-rw-rw-   0        0        0      686 2023-07-12 11:28:48.000000 anyjson2csv-0.0.2/src/anyjson2csv/json_to_csv.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:29:21.442460 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-07-12 11:29:21.000000 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-07-12 11:29:21.000000 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:29:21.000000 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 11:29:21.000000 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/top_level.txt
```

### Comparing `anyjson2csv-0.0.1/LICENSE.txt` & `anyjson2csv-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anyjson2csv-0.0.1/PKG-INFO` & `anyjson2csv-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyjson2csv
-Version: 0.0.1
+Version: 0.0.2
 Summary: JSON flatten to CSV for Python
 Author-email: BrainsLogic <info@brainslogic.com>
 Project-URL: Homepage, https://github.com/mehdiabidi/json2csv
 Project-URL: Bug Tracker, https://github.com/mehdiabidi/json2csv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anyjson2csv-0.0.1/pyproject.toml` & `anyjson2csv-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anyjson2csv"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="BrainsLogic", email="info@brainslogic.com" },
 ]
 description = "JSON flatten to CSV for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `anyjson2csv-0.0.1/src/anyjson2csv.egg-info/PKG-INFO` & `anyjson2csv-0.0.2/src/anyjson2csv.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyjson2csv
-Version: 0.0.1
+Version: 0.0.2
 Summary: JSON flatten to CSV for Python
 Author-email: BrainsLogic <info@brainslogic.com>
 Project-URL: Homepage, https://github.com/mehdiabidi/json2csv
 Project-URL: Bug Tracker, https://github.com/mehdiabidi/json2csv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anyjson2csv-0.0.1/src/json2csv/flatten_json.py` & `anyjson2csv-0.0.2/src/anyjson2csv/flatten_json.py`

 * *Files identical despite different names*

### Comparing `anyjson2csv-0.0.1/src/json2csv/json_to_csv.py` & `anyjson2csv-0.0.2/src/anyjson2csv/json_to_csv.py`

 * *Files identical despite different names*

