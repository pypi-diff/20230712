# Comparing `tmp/opack-0.0.1.tar.gz` & `tmp/opack-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opack-0.0.1.tar", last modified: Wed Jul 12 07:41:56 2023, max compression
+gzip compressed data, was "opack-0.1.0.tar", last modified: Wed Jul 12 10:26:06 2023, max compression
```

## Comparing `opack-0.0.1.tar` & `opack-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:41:56.171057 opack-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 07:41:41.000000 opack-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-12 07:41:56.171057 opack-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 07:41:41.000000 opack-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:41:56.167056 opack-0.0.1/opack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:41:41.000000 opack-0.0.1/opack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 07:41:41.000000 opack-0.0.1/opack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-12 07:41:41.000000 opack-0.0.1/opack/object_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 07:41:41.000000 opack-0.0.1/opack/opack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-12 07:41:41.000000 opack-0.0.1/opack/opack_construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:41:56.171057 opack-0.0.1/opack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-12 07:41:56.000000 opack-0.0.1/opack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 07:41:56.000000 opack-0.0.1/opack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:41:56.000000 opack-0.0.1/opack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 07:41:56.000000 opack-0.0.1/opack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 07:41:56.000000 opack-0.0.1/opack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 07:41:56.000000 opack-0.0.1/opack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-12 07:41:41.000000 opack-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 07:41:41.000000 opack-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 07:41:56.171057 opack-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:41:56.171057 opack-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-12 07:41:41.000000 opack-0.0.1/tests/test_opack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:26:06.603904 opack-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 10:25:49.000000 opack-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-12 10:26:06.603904 opack-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 10:25:49.000000 opack-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:26:06.603904 opack-0.1.0/opack/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 10:25:49.000000 opack-0.1.0/opack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 10:25:49.000000 opack-0.1.0/opack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-12 10:25:49.000000 opack-0.1.0/opack/object_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 10:25:49.000000 opack-0.1.0/opack/opack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-12 10:25:49.000000 opack-0.1.0/opack/opack_construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:26:06.603904 opack-0.1.0/opack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-12 10:26:06.000000 opack-0.1.0/opack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 10:26:06.000000 opack-0.1.0/opack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:26:06.000000 opack-0.1.0/opack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 10:26:06.000000 opack-0.1.0/opack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 10:26:06.000000 opack-0.1.0/opack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 10:26:06.000000 opack-0.1.0/opack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-12 10:25:49.000000 opack-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 10:25:49.000000 opack-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:26:06.603904 opack-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:26:06.603904 opack-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-12 10:25:49.000000 opack-0.1.0/tests/test_opack.py
```

### Comparing `opack-0.0.1/LICENSE` & `opack-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opack-0.0.1/PKG-INFO` & `opack-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opack
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python library for parsing the opack format
 Author-email: lori <loriwittdev@gmail.com>
 Maintainer-email: lori <loriwittdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 loriwitt
```

### Comparing `opack-0.0.1/opack/object_types.py` & `opack-0.1.0/opack/object_types.py`

 * *Files identical despite different names*

### Comparing `opack-0.0.1/opack/opack_construct.py` & `opack-0.1.0/opack/opack_construct.py`

 * *Files identical despite different names*

### Comparing `opack-0.0.1/opack.egg-info/PKG-INFO` & `opack-0.1.0/opack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opack
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python library for parsing the opack format
 Author-email: lori <loriwittdev@gmail.com>
 Maintainer-email: lori <loriwittdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 loriwitt
```

### Comparing `opack-0.0.1/pyproject.toml` & `opack-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "opack"
-version = "0.0.1"
+version = "0.1.0"
 description = "Python library for parsing the opack format"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "opack", "plist", "cli", "parser"]
 authors = [
     { name = "lori", email = "loriwittdev@gmail.com" }
```

### Comparing `opack-0.0.1/tests/test_opack.py` & `opack-0.1.0/tests/test_opack.py`

 * *Files identical despite different names*

