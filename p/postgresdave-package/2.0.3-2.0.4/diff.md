# Comparing `tmp/postgresdave_package-2.0.3.tar.gz` & `tmp/postgresdave_package-2.0.4.tar.gz`

## Comparing `postgresdave_package-2.0.3.tar` & `postgresdave_package-2.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/01) create the database.sql
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/02) create the schemas.sql
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/03) create roles.sql
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/04) grant usage.sql
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/05) create the users.sql
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/06) Admin Queries.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/07) CancelQueries.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/08) CREATE TABLE AS.sql
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/09) pk_fk_example.sql
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/10) SELECT LAG LEAD RANK.sql
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/11) tables.ddl
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/12) Levenshtein.ddl
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/13) Database Profiling.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/14) Iterative, Dynamic SQL.md
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/Backup.md
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/Basics.md
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/QuickStart.md
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/backup.bat
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/methods.md
--rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/restore.bat
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/src/postgresdave_package/.querylog
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/src/postgresdave_package/__init__.py
--rw-r--r--   0        0        0    16758 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/src/postgresdave_package/postgresdave.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/src/postgresdave_package/testcase1.csv
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/.schemawiz_config1
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/.schemawiz_config3
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/Test_Connect.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/Test_SQLite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/local_sqlite_db
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/LICENSE
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/README.md
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/01) create the database.sql
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/02) create the schemas.sql
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/03) create roles.sql
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/04) grant usage.sql
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/05) create the users.sql
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/06) Admin Queries.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/07) CancelQueries.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/08) CREATE TABLE AS.sql
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/09) pk_fk_example.sql
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/10) SELECT LAG LEAD RANK.sql
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/11) tables.ddl
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/12) Levenshtein.ddl
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/13) Database Profiling.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/14) Iterative, Dynamic SQL.md
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/Backup.md
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/Basics.md
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/QuickStart.md
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/backup.bat
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/methods.md
+-rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/restore.bat
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/src/postgresdave_package/.querylog
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/src/postgresdave_package/__init__.py
+-rw-r--r--   0        0        0    16758 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/src/postgresdave_package/postgresdave.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/src/postgresdave_package/testcase1.csv
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/test/.schemawiz_config1
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/test/.schemawiz_config3
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/test/Test_Connect.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/test/Test_SQLite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/test/local_sqlite_db
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/LICENSE
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/README.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 postgresdave_package-2.0.4/PKG-INFO
```

### Comparing `postgresdave_package-2.0.3/04) grant usage.sql` & `postgresdave_package-2.0.4/04) grant usage.sql`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/06) Admin Queries.md` & `postgresdave_package-2.0.4/06) Admin Queries.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/07) CancelQueries.md` & `postgresdave_package-2.0.4/07) CancelQueries.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/09) pk_fk_example.sql` & `postgresdave_package-2.0.4/09) pk_fk_example.sql`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/12) Levenshtein.ddl` & `postgresdave_package-2.0.4/12) Levenshtein.ddl`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/13) Database Profiling.md` & `postgresdave_package-2.0.4/13) Database Profiling.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/14) Iterative, Dynamic SQL.md` & `postgresdave_package-2.0.4/14) Iterative, Dynamic SQL.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/Backup.md` & `postgresdave_package-2.0.4/Backup.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/QuickStart.md` & `postgresdave_package-2.0.4/QuickStart.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/backup.bat` & `postgresdave_package-2.0.4/backup.bat`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/methods.md` & `postgresdave_package-2.0.4/methods.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/restore.bat` & `postgresdave_package-2.0.4/restore.bat`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/src/postgresdave_package/.querylog` & `postgresdave_package-2.0.4/src/postgresdave_package/.querylog`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/src/postgresdave_package/postgresdave.py` & `postgresdave_package-2.0.4/src/postgresdave_package/postgresdave.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import psycopg2 
 from datetime import *
 import time
 from garbledave_package.garbledave import garbledave 
 
 def main():
-	mydb = postgres_db('thisone')
+	mydb = postgres_db('new one')
 	mydb.connect()
 	mydb = postgres_db('that one')
 	mydb.connect()
 	print(mydb.dbstr())	
 
 	#print(mydb.does_table_exist('projectbuckets'))
 	#mydb.enable_logging = True
```

### Comparing `postgresdave_package-2.0.3/LICENSE` & `postgresdave_package-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `postgresdave_package-2.0.3/pyproject.toml` & `postgresdave_package-2.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["hatchling","psycopg2","garbledave_package"]
+requires = ["hatchling","psycopg2-binary","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "postgresdave_package"
-version = "2.0.3"
+version = "2.0.4"
 dependencies = [
-  'psycopg2 >= 2.9.5',
+  'psycopg2-binary >= 2.9.5',
   'garbledave_package >= 1.0.0'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
 description = "A wrapper for simplified Postgres usage using psycopg2."
 readme = "README.md"
```

### Comparing `postgresdave_package-2.0.3/PKG-INFO` & `postgresdave_package-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: postgresdave_package
-Version: 2.0.3
+Version: 2.0.4
 Summary: A wrapper for simplified Postgres usage using psycopg2.
 Project-URL: Homepage, https://github.com/daveskura/postgresdave
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: garbledave-package>=1.0.0
-Requires-Dist: psycopg2>=2.9.5
+Requires-Dist: psycopg2-binary>=2.9.5
 Description-Content-Type: text/markdown
 
 # postgresdave
 A simple wrapper on psycopg2 to access Postgres
 
 ### install with pip
 pip install postgresdave_package
```

