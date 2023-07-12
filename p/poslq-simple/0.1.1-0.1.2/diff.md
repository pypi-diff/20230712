# Comparing `tmp/poslq_simple-0.1.1.tar.gz` & `tmp/poslq_simple-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poslq_simple-0.1.1.tar", last modified: Wed Jul 12 20:14:20 2023, max compression
+gzip compressed data, was "poslq_simple-0.1.2.tar", last modified: Wed Jul 12 20:29:10 2023, max compression
```

## Comparing `poslq_simple-0.1.1.tar` & `poslq_simple-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 20:14:20.140205 poslq_simple-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-07-12 18:29:23.000000 poslq_simple-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3302 2023-07-12 20:14:20.139206 poslq_simple-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2778 2023-07-12 18:48:23.000000 poslq_simple-0.1.1/README.md
--rw-rw-rw-   0        0        0      602 2023-07-12 20:13:35.000000 poslq_simple-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 20:14:20.140205 poslq_simple-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 20:14:20.119676 poslq_simple-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 20:14:20.136693 poslq_simple-0.1.1/src/poslq_simple.egg-info/
--rw-rw-rw-   0        0        0     3302 2023-07-12 20:14:20.000000 poslq_simple-0.1.1/src/poslq_simple.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-07-12 20:14:20.000000 poslq_simple-0.1.1/src/poslq_simple.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 20:14:20.000000 poslq_simple-0.1.1/src/poslq_simple.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 20:14:20.000000 poslq_simple-0.1.1/src/poslq_simple.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 20:14:20.138200 poslq_simple-0.1.1/src/posql_simple/
--rw-rw-rw-   0        0        0        0 2023-07-12 18:18:07.000000 poslq_simple-0.1.1/src/posql_simple/__init__.py
--rw-rw-rw-   0        0        0     1831 2023-07-12 18:19:47.000000 poslq_simple-0.1.1/src/posql_simple/cypher.py
--rw-rw-rw-   0        0        0     5955 2023-07-12 18:19:15.000000 poslq_simple-0.1.1/src/posql_simple/w_out_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:29:10.569218 poslq_simple-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-12 18:29:23.000000 poslq_simple-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3302 2023-07-12 20:29:10.568218 poslq_simple-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2778 2023-07-12 18:48:23.000000 poslq_simple-0.1.2/README.md
+-rw-rw-rw-   0        0        0      611 2023-07-12 20:27:46.000000 poslq_simple-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 20:29:10.569218 poslq_simple-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 20:29:10.554550 poslq_simple-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 20:29:10.565143 poslq_simple-0.1.2/src/poslq_simple.egg-info/
+-rw-rw-rw-   0        0        0     3302 2023-07-12 20:29:10.000000 poslq_simple-0.1.2/src/poslq_simple.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-07-12 20:29:10.000000 poslq_simple-0.1.2/src/poslq_simple.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 20:29:10.000000 poslq_simple-0.1.2/src/poslq_simple.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 20:29:10.000000 poslq_simple-0.1.2/src/poslq_simple.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 20:29:10.567216 poslq_simple-0.1.2/src/posql_simple/
+-rw-rw-rw-   0        0        0        0 2023-07-12 18:18:07.000000 poslq_simple-0.1.2/src/posql_simple/__init__.py
+-rw-rw-rw-   0        0        0     1831 2023-07-12 18:19:47.000000 poslq_simple-0.1.2/src/posql_simple/cypher.py
+-rw-rw-rw-   0        0        0     5954 2023-07-12 20:19:04.000000 poslq_simple-0.1.2/src/posql_simple/w_out_sql.py
```

### Comparing `poslq_simple-0.1.1/LICENSE` & `poslq_simple-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poslq_simple-0.1.1/PKG-INFO` & `poslq_simple-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poslq_simple
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `poslq_simple-0.1.1/README.md` & `poslq_simple-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `poslq_simple-0.1.1/pyproject.toml` & `poslq_simple-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "poslq_simple"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="enyos", email="lebedevhh@outlook.fr" },
 ]
 description = "A simple nosql json storage for small projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `poslq_simple-0.1.1/src/poslq_simple.egg-info/PKG-INFO` & `poslq_simple-0.1.2/src/poslq_simple.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poslq-simple
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `poslq_simple-0.1.1/src/posql_simple/cypher.py` & `poslq_simple-0.1.2/src/posql_simple/cypher.py`

 * *Files identical despite different names*

### Comparing `poslq_simple-0.1.1/src/posql_simple/w_out_sql.py` & `poslq_simple-0.1.2/src/posql_simple/w_out_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import threading
 import time
 import uuid
 from os.path import exists, basename
 import os
-from cypher import  gen_cipher_file, gen_decypher_file
+from cypher import gen_cipher_file, gen_decypher_file
 from pathlib import Path
 
 LOCK = threading.Lock()
 
 # custom error class
 class InvalidFileExtensionError( Exception ):
     "File extension must be .pst"
```

