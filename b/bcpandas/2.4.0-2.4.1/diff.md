# Comparing `tmp/bcpandas-2.4.0.tar.gz` & `tmp/bcpandas-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcpandas-2.4.0.tar", max compression
+gzip compressed data, was "bcpandas-2.4.1.tar", max compression
```

## Comparing `bcpandas-2.4.0.tar` & `bcpandas-2.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-04-08 02:50:35.706562 bcpandas-2.4.0/LICENSE
--rw-r--r--   0        0        0    16614 2023-04-08 02:50:35.706562 bcpandas-2.4.0/README.md
--rw-r--r--   0        0        0      563 2023-04-08 02:50:35.706562 bcpandas-2.4.0/bcpandas/__init__.py
--rw-r--r--   0        0        0     2339 2023-04-08 02:50:35.706562 bcpandas-2.4.0/bcpandas/constants.py
--rw-r--r--   0        0        0    16908 2023-04-08 02:50:35.706562 bcpandas-2.4.0/bcpandas/main.py
--rw-r--r--   0        0        0     7976 2023-04-08 02:50:35.706562 bcpandas-2.4.0/bcpandas/utils.py
--rw-r--r--   0        0        0     2493 2023-04-08 02:50:52.940438 bcpandas-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    17828 1970-01-01 00:00:00.000000 bcpandas-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-12 06:14:03.708241 bcpandas-2.4.1/LICENSE
+-rw-r--r--   0        0        0    16614 2023-07-12 06:14:03.708241 bcpandas-2.4.1/README.md
+-rw-r--r--   0        0        0      563 2023-07-12 06:14:03.708241 bcpandas-2.4.1/bcpandas/__init__.py
+-rw-r--r--   0        0        0     2339 2023-07-12 06:14:03.708241 bcpandas-2.4.1/bcpandas/constants.py
+-rw-r--r--   0        0        0    17016 2023-07-12 06:14:03.708241 bcpandas-2.4.1/bcpandas/main.py
+-rw-r--r--   0        0        0     8288 2023-07-12 06:14:03.708241 bcpandas-2.4.1/bcpandas/utils.py
+-rw-r--r--   0        0        0     2510 2023-07-12 06:14:20.780206 bcpandas-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0    17676 1970-01-01 00:00:00.000000 bcpandas-2.4.1/PKG-INFO
```

### Comparing `bcpandas-2.4.0/LICENSE` & `bcpandas-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bcpandas-2.4.0/README.md` & `bcpandas-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bcpandas-2.4.0/bcpandas/__init__.py` & `bcpandas-2.4.1/bcpandas/__init__.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.4.0/bcpandas/constants.py` & `bcpandas-2.4.1/bcpandas/constants.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.4.0/bcpandas/main.py` & `bcpandas-2.4.1/bcpandas/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,39 +67,42 @@
         driver_version: Optional[int] = None,
         port: int = 1433,
         odbc_kwargs: Optional[Dict[str, Union[str, int]]] = None,
     ):
         self.server = server
         self.database = database
         self.port = port
+        self.odbc_kwargs = odbc_kwargs
 
         if driver_version is None:
             all_drivers: List[str] = pyodbc.drivers()
             driver_candidates: List[str] = [
                 d.split("Driver ")[-1].split(" ")[0] for d in all_drivers if "SQL Server" in d
             ]
             new_driver_version: int = max(int(v) for v in driver_candidates if v.isnumeric())
             self.driver = f"{{ODBC Driver {new_driver_version} for SQL Server}}"
+            self.driver_version = new_driver_version  # simplifies copy construction
         else:
             self.driver = f"{{ODBC Driver {driver_version} for SQL Server}}"
+            self.driver_version = driver_version  # simplifies copy construction
 
         # Append a comma for use in connection strings (optionally blank)
         if port:
             port_str = f",{self.port}"
         else:
             port_str = ""
 
         db_url = (
             f"Driver={self.driver};Server=tcp:{self.server}{port_str};Database={self.database};"
         )
         if username and password:
             self.username = username
             self.password = password
             self.with_krb_auth = False
-            db_url += f"UID={username};PWD={password}"
+            db_url += f"UID={username};PWD={password};"
         else:
             self.username = ""
             self.password = ""
             self.with_krb_auth = True
             db_url += "Trusted_Connection=yes;"
 
         logger.info(f"Created creds:\t{self}")
@@ -404,17 +407,16 @@
     """
     # validation
     if df.shape[0] == 0 or df.shape[1] == 0:
         return
 
     _validate_args(df=df, sql_type=sql_type, if_exists=if_exists, batch_size=batch_size)
 
-    # TODO diff way to implement? could be big performance hit with big dataframe
     if index:
-        df = df.copy(deep=True).reset_index()
+        df = df.reset_index()
 
     delim = get_delimiter(df) if delimiter is None else delimiter
     _quotechar = get_quotechar(df) if quotechar is None else quotechar
 
     # save to temp path
     csv_file_path = get_temp_file(work_directory)
     # replace bools with 1 or 0, this is what pandas native does when writing to SQL Server
```

### Comparing `bcpandas-2.4.0/bcpandas/utils.py` & `bcpandas-2.4.1/bcpandas/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Created on Sat Aug  3 23:07:15 2019
 
 @author: ydima
 """
 
 import logging
+import sys
 from pathlib import Path
 import random
 import shlex
 import string
 from subprocess import PIPE, STDOUT, Popen
 import tempfile
 from typing import Dict, List, Optional, Tuple, Union
@@ -66,14 +67,20 @@
         )
 
     # auth
     if creds.with_krb_auth:
         auth = ["-T"]
     else:
         auth = ["-U", quote_this(creds.username), "-P", quote_this(creds.password)]
+    if creds.odbc_kwargs:
+        kwargs = {k.lower(): v for k, v in creds.odbc_kwargs.items()}
+        false_values = ("n", "no", "f", "false", "off", "0")
+
+        if sys.platform != "win32" and "encrypt" in kwargs:
+            auth += [f"-Y{'m' if kwargs['encrypt'] not in false_values else 'o'}"]
 
     # prepare SQL item string
     if sql_type == QUERY:
         # remove newlines for queries, otherwise messes up BCP
         sql_item_string = quote_this("".join(sql_item.splitlines()))
     else:
         sql_item_string = f"{schema}.{sql_item}"
```

### Comparing `bcpandas-2.4.0/pyproject.toml` & `bcpandas-2.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 description = "High-level wrapper around BCP for high performance data transfers between pandas and SQL Server. No knowledge of BCP required!!"
 keywords = ["bcp", "mssql", "pandas"]
 license = "MIT"
 maintainers = ["Oliver Borchert <me@borchero.com>"]
 name = "bcpandas"
 readme = "README.md"
 repository = "https://github.com/yehoshuadimarsky/bcpandas"
-version = "v2.4.0"
+version = "v2.4.1"
 
 [tool.poetry.plugins."pandas.sql.engine"]
 bcpandas = "bcpandas.main:to_sql"
 
 [tool.poetry.dependencies]
 pandas = ">=1.5"
 pyodbc = "*"
 python = ">=3.8.1"
 sqlalchemy = ">=1.0,<2.0"
 
 [tool.poetry.group.dev.dependencies]
+pre-commit = "*"
 black = "*"
 mypy = "*"
 ruff = "^0"
 types-setuptools = "*"
 
 [tool.poetry.group.test.dependencies]
 codetiming = "1.4.0"
```

### Comparing `bcpandas-2.4.0/PKG-INFO` & `bcpandas-2.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcpandas
-Version: 2.4.0
+Version: 2.4.1
 Summary: High-level wrapper around BCP for high performance data transfers between pandas and SQL Server. No knowledge of BCP required!!
 Home-page: https://github.com/yehoshuadimarsky/bcpandas
 License: MIT
 Keywords: bcp,mssql,pandas
 Author: yehoshuadimarsky
 Maintainer: Oliver Borchert
 Maintainer-email: me@borchero.com
@@ -12,18 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Requires-Dist: pandas (>=1.5)
 Requires-Dist: pyodbc
 Requires-Dist: sqlalchemy (>=1.0,<2.0)
 Project-URL: Repository, https://github.com/yehoshuadimarsky/bcpandas
 Description-Content-Type: text/markdown
```

