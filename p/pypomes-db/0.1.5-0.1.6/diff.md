# Comparing `tmp/pypomes_db-0.1.5.tar.gz` & `tmp/pypomes_db-0.1.6.tar.gz`

## Comparing `pypomes_db-0.1.5.tar` & `pypomes_db-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12400 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12338 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/PKG-INFO
```

### Comparing `pypomes_db-0.1.5/src/pypomes_db/db_pomes.py` & `pypomes_db-0.1.6/src/pypomes_db/db_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,15 @@
         with connect(__CONNECTION_KWARGS) as conn:
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 cursor.execute(sel_stmt, where_vals)
                 # obtain the returned tuples
                 rows: list[Row] = cursor.fetchall()
                 for row in rows:
-                    values: list = [item for item in row]
-                    result.append(tuple(values))
+                    result.append(tuple(row))
     except Exception as e:
         exc = True
         errors.append(__db_except_msg(e))
 
     # no errors, the 'required' parameter has been defined, and the search is empty ?
     if required and not exc and len(result) == 0:
         # yes, report the error
```

### Comparing `pypomes_db-0.1.5/LICENSE` & `pypomes_db-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.1.5/pyproject.toml` & `pypomes_db-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (DB modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.1.5/PKG-INFO` & `pypomes_db-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_db
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of Python pomes, pennyeach (DB modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

