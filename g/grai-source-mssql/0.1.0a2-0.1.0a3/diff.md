# Comparing `tmp/grai_source_mssql-0.1.0a2.tar.gz` & `tmp/grai_source_mssql-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_mssql-0.1.0a2.tar", max compression
+gzip compressed data, was "grai_source_mssql-0.1.0a3.tar", max compression
```

## Comparing `grai_source_mssql-0.1.0a2.tar` & `grai_source_mssql-0.1.0a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1727 2023-05-02 08:01:59.696148 grai_source_mssql-0.1.0a2/README.md
--rw-r--r--   0        0        0     1032 2023-07-03 13:09:35.866648 grai_source_mssql-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      169 2023-06-30 11:57:03.825592 grai_source_mssql-0.1.0a2/src/grai_source_mssql/__init__.py
--rw-r--r--   0        0        0     8770 2023-06-29 12:17:13.063891 grai_source_mssql-0.1.0a2/src/grai_source_mssql/adapters.py
--rw-r--r--   0        0        0     1457 2023-06-30 17:13:40.677480 grai_source_mssql-0.1.0a2/src/grai_source_mssql/base.py
--rw-r--r--   0        0        0    12098 2023-06-29 12:17:13.150105 grai_source_mssql-0.1.0a2/src/grai_source_mssql/loader.py
--rw-r--r--   0        0        0     5032 2023-06-06 17:35:16.815992 grai_source_mssql-0.1.0a2/src/grai_source_mssql/models.py
--rw-r--r--   0        0        0      193 2023-06-06 17:35:16.816110 grai_source_mssql-0.1.0a2/src/grai_source_mssql/package_definitions.py
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 grai_source_mssql-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1727 2023-05-02 08:01:59.696148 grai_source_mssql-0.1.0a3/README.md
+-rw-r--r--   0        0        0     1032 2023-07-12 11:27:39.984362 grai_source_mssql-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-07-12 11:27:54.108908 grai_source_mssql-0.1.0a3/src/grai_source_mssql/__init__.py
+-rw-r--r--   0        0        0     8770 2023-07-12 10:52:48.719804 grai_source_mssql-0.1.0a3/src/grai_source_mssql/adapters.py
+-rw-r--r--   0        0        0     1457 2023-07-12 11:10:45.899843 grai_source_mssql-0.1.0a3/src/grai_source_mssql/base.py
+-rw-r--r--   0        0        0    12098 2023-07-12 10:52:48.720561 grai_source_mssql-0.1.0a3/src/grai_source_mssql/loader.py
+-rw-r--r--   0        0        0     5032 2023-06-06 17:35:16.815992 grai_source_mssql-0.1.0a3/src/grai_source_mssql/models.py
+-rw-r--r--   0        0        0      193 2023-06-06 17:35:16.816110 grai_source_mssql-0.1.0a3/src/grai_source_mssql/package_definitions.py
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 grai_source_mssql-0.1.0a3/PKG-INFO
```

### Comparing `grai_source_mssql-0.1.0a2/README.md` & `grai_source_mssql-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.1.0a2/pyproject.toml` & `grai_source_mssql-0.1.0a3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "grai_source_mssql"
-version = "0.1.0-alpha2"
+version = "0.1.0-alpha3"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_mssql", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-mssql"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a10", allow-prereleases = true}
+grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 multimethod = "^1.8"
 pyodbc = "^4.0.35"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
```

### Comparing `grai_source_mssql-0.1.0a2/src/grai_source_mssql/adapters.py` & `grai_source_mssql-0.1.0a3/src/grai_source_mssql/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.1.0a2/src/grai_source_mssql/base.py` & `grai_source_mssql-0.1.0a3/src/grai_source_mssql/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.1.0a2/src/grai_source_mssql/loader.py` & `grai_source_mssql-0.1.0a3/src/grai_source_mssql/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.1.0a2/src/grai_source_mssql/models.py` & `grai_source_mssql-0.1.0a3/src/grai_source_mssql/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.1.0a2/PKG-INFO` & `grai_source_mssql-0.1.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: grai-source-mssql
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: grai-client (>=0.3.0a10,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pyodbc (>=4.0.35,<5.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-mssql
 Description-Content-Type: text/markdown
```

