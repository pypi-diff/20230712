# Comparing `tmp/pypomes_db-0.1.3.tar.gz` & `tmp/pypomes_db-0.1.4.tar.gz`

## Comparing `pypomes_db-0.1.3.tar` & `pypomes_db-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12327 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/PKG-INFO
```

### Comparing `pypomes_db-0.1.3/LICENSE` & `pypomes_db-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.1.3/pyproject.toml` & `pypomes_db-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (DB modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,15 +18,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=23.1.2",
     "psycopg2-binary>=2.9.6",
     "pyodbc>=4.0.39",
-    "pypomes_core>=0.1.1",
+    "pypomes_core>=0.1.4",
     "setuptools>=68.0.0",
     "wheel>=0.40.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.1.3/PKG-INFO` & `pypomes_db-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pypomes_db
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of Python pomes, pennyeach (DB modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=23.1.2
 Requires-Dist: psycopg2-binary>=2.9.6
 Requires-Dist: pyodbc>=4.0.39
-Requires-Dist: pypomes-core>=0.1.1
+Requires-Dist: pypomes-core>=0.1.4
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.40.0
```

