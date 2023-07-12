# Comparing `tmp/grai_source_postgres-0.2.0a3.tar.gz` & `tmp/grai_source_postgres-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_postgres-0.2.0a3.tar", max compression
+gzip compressed data, was "grai_source_postgres-0.2.0a4.tar", max compression
```

## Comparing `grai_source_postgres-0.2.0a3.tar` & `grai_source_postgres-0.2.0a4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      139 2023-05-02 08:01:59.696469 grai_source_postgres-0.2.0a3/README.md
--rw-r--r--   0        0        0     1118 2023-07-03 12:45:21.460147 grai_source_postgres-0.2.0a3/pyproject.toml
--rw-r--r--   0        0        0      175 2023-07-03 12:45:27.022653 grai_source_postgres-0.2.0a3/src/grai_source_postgres/__init__.py
--rw-r--r--   0        0        0     8780 2023-06-29 12:17:13.189092 grai_source_postgres-0.2.0a3/src/grai_source_postgres/adapters.py
--rw-r--r--   0        0        0     1069 2023-06-30 17:13:40.680269 grai_source_postgres-0.2.0a3/src/grai_source_postgres/base.py
--rw-r--r--   0        0        0    10194 2023-06-06 17:35:16.819070 grai_source_postgres-0.2.0a3/src/grai_source_postgres/loader.py
--rw-r--r--   0        0        0     5200 2023-06-06 17:35:16.819189 grai_source_postgres-0.2.0a3/src/grai_source_postgres/models.py
--rw-r--r--   0        0        0      199 2023-06-06 17:35:16.819399 grai_source_postgres-0.2.0a3/src/grai_source_postgres/package_definitions.py
--rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 grai_source_postgres-0.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0      139 2023-05-02 08:01:59.696469 grai_source_postgres-0.2.0a4/README.md
+-rw-r--r--   0        0        0     1119 2023-07-12 11:14:14.947138 grai_source_postgres-0.2.0a4/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-12 11:14:36.526720 grai_source_postgres-0.2.0a4/src/grai_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8780 2023-07-12 10:52:48.736364 grai_source_postgres-0.2.0a4/src/grai_source_postgres/adapters.py
+-rw-r--r--   0        0        0     1069 2023-07-12 11:11:31.476728 grai_source_postgres-0.2.0a4/src/grai_source_postgres/base.py
+-rw-r--r--   0        0        0    10194 2023-06-06 17:35:16.819070 grai_source_postgres-0.2.0a4/src/grai_source_postgres/loader.py
+-rw-r--r--   0        0        0     5200 2023-06-06 17:35:16.819189 grai_source_postgres-0.2.0a4/src/grai_source_postgres/models.py
+-rw-r--r--   0        0        0      199 2023-06-06 17:35:16.819399 grai_source_postgres-0.2.0a4/src/grai_source_postgres/package_definitions.py
+-rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 grai_source_postgres-0.2.0a4/PKG-INFO
```

### Comparing `grai_source_postgres-0.2.0a3/pyproject.toml` & `grai_source_postgres-0.2.0a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "grai_source_postgres"
-version = "0.2.0-alpha3"
+version = "0.2.0-alpha4"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_postgres", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-postgres"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a9", allow-prereleases = true}
+grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 PyYAML = "^6.0"
 multimethod = "^1.8"
 psycopg2 = "^2.9.5"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
```

### Comparing `grai_source_postgres-0.2.0a3/src/grai_source_postgres/adapters.py` & `grai_source_postgres-0.2.0a4/src/grai_source_postgres/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_postgres-0.2.0a3/src/grai_source_postgres/base.py` & `grai_source_postgres-0.2.0a4/src/grai_source_postgres/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_postgres-0.2.0a3/src/grai_source_postgres/loader.py` & `grai_source_postgres-0.2.0a4/src/grai_source_postgres/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_postgres-0.2.0a3/src/grai_source_postgres/models.py` & `grai_source_postgres-0.2.0a4/src/grai_source_postgres/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_postgres-0.2.0a3/PKG-INFO` & `grai_source_postgres-0.2.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-source-postgres
-Version: 0.2.0a3
+Version: 0.2.0a4
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
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: grai-client (>=0.3.0a9,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-postgres
 Description-Content-Type: text/markdown
```

