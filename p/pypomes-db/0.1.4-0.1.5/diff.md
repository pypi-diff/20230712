# Comparing `tmp/pypomes_db-0.1.4.tar.gz` & `tmp/pypomes_db-0.1.5.tar.gz`

## Comparing `pypomes_db-0.1.4.tar` & `pypomes_db-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12327 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12400 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.5/PKG-INFO
```

### Comparing `pypomes_db-0.1.4/src/pypomes_db/db_pomes.py` & `pypomes_db-0.1.5/src/pypomes_db/db_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,26 +65,28 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
     :param required: defines whether an empty search should be considered an error
     :return: tuple containing the search result, or None if there was an error, or if the search was empty
     """
-    # inicializa a variável de retorno
+    # inicialize the return variable
     result: tuple | None = None
 
     exc: bool = False
     try:
         with connect(__CONNECTION_KWARGS) as conn:
-            # obtem o cursor e executa a operação
+            # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
-                sel_stmt = sel_stmt.replace("SELECT", "SELECT TOP 1")
+                sel_stmt = sel_stmt.replace("SELECT", "SELECT TOP 1", 1)
                 cursor.execute(sel_stmt, where_vals)
-                # obtem a primeira tupla retornada pelo SELECT (None se nenhuma foi retornada)
-                result = cursor.fetchone()
+                # obtain the first tuple returned (None se no tuple was returned)
+                rec: Row = cursor.fetchone()
+                if rec is not None:
+                    result = tuple(rec)
     except Exception as e:
         exc = True
         errors.append(__db_except_msg(e))
 
     # o parâmetro 'required' foi definido e nenhum registro foi obtido?
     if required and not exc and result is None:
         # sim, reporte o erro
@@ -262,15 +264,15 @@
 
     return result
 
 
 def __db_except_msg(exception: Exception) -> str:
     """
     Formats and returns the error message corresponding to the exception raised
-    while accessing to the database.
+    while accessing the database.
 
     :param exception: the exception raised
     :return:the formatted error message
     """
     exc_msg: str = f"{exception}"
     exc_msg = exc_msg.replace('"', "'") \
                      .replace('\n', " ") \
@@ -279,15 +281,15 @@
     result = f"Error accessing {DB_NAME} at {DB_HOST}: {exc_msg}"
 
     return result
 
 
 def __db_required_msg(sel_stmt: str, where_vals: tuple) -> str:
     """
-    Formats and returns the message indicative of empty search.
+    Formats and returns the message indicative of an empty search.
 
     :param sel_stmt: the search command
     :param where_vals: values associated with the search criteria
     :return: message indicative of empty search
     """
     stmt: str = sel_stmt.replace('"', "'") \
                         .replace('\n', " ") \
```

### Comparing `pypomes_db-0.1.4/LICENSE` & `pypomes_db-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.1.4/pyproject.toml` & `pypomes_db-0.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (DB modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.1.4/PKG-INFO` & `pypomes_db-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_db
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of Python pomes, pennyeach (DB modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

