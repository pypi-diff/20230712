# Comparing `tmp/grai_source_snowflake-0.1.0a2.tar.gz` & `tmp/grai_source_snowflake-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_snowflake-0.1.0a2.tar", max compression
+gzip compressed data, was "grai_source_snowflake-0.1.0a3.tar", max compression
```

## Comparing `grai_source_snowflake-0.1.0a2.tar` & `grai_source_snowflake-0.1.0a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      144 2023-05-02 08:01:59.696972 grai_source_snowflake-0.1.0a2/README.md
--rw-r--r--   0        0        0     1114 2023-07-03 13:11:40.788304 grai_source_snowflake-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      177 2023-06-30 11:58:01.630475 grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/__init__.py
--rw-r--r--   0        0        0     8707 2023-06-29 12:17:13.225985 grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/adapters.py
--rw-r--r--   0        0        0     1184 2023-06-30 17:13:40.683025 grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/base.py
--rw-r--r--   0        0        0    10107 2023-06-06 17:35:16.823894 grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/loader.py
--rw-r--r--   0        0        0     5973 2023-06-06 17:35:16.824028 grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/models.py
--rw-r--r--   0        0        0      201 2023-06-06 17:35:16.824210 grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/package_definitions.py
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 grai_source_snowflake-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      144 2023-05-02 08:01:59.696972 grai_source_snowflake-0.1.0a3/README.md
+-rw-r--r--   0        0        0     1114 2023-07-12 11:29:35.481766 grai_source_snowflake-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-07-12 11:29:39.667753 grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/__init__.py
+-rw-r--r--   0        0        0     8707 2023-07-12 10:52:48.743077 grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/adapters.py
+-rw-r--r--   0        0        0     1184 2023-07-12 11:08:28.542931 grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/base.py
+-rw-r--r--   0        0        0    10107 2023-06-06 17:35:16.823894 grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/loader.py
+-rw-r--r--   0        0        0     5973 2023-06-06 17:35:16.824028 grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/models.py
+-rw-r--r--   0        0        0      201 2023-06-06 17:35:16.824210 grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/package_definitions.py
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 grai_source_snowflake-0.1.0a3/PKG-INFO
```

### Comparing `grai_source_snowflake-0.1.0a2/pyproject.toml` & `grai_source_snowflake-0.1.0a3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_snowflake"
-version = "0.1.0-alpha2"
+version = "0.1.0-alpha3"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "ELv2"
 packages = [
     { include = "grai_source_snowflake", from = "src" },
 ]
 readme = "README.md"
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 PyYAML = "^6.0"
 multimethod = "^1.8"
 snowflake-connector-python = "^3.0.0"
-grai-client = {version = "^0.3.0a10", allow-prereleases = true}
+grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.10.1"
 pytest = "^7.2.0"
```

### Comparing `grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/adapters.py` & `grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/base.py` & `grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/loader.py` & `grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_snowflake-0.1.0a2/src/grai_source_snowflake/models.py` & `grai_source_snowflake-0.1.0a3/src/grai_source_snowflake/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_snowflake-0.1.0a2/PKG-INFO` & `grai_source_snowflake-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-source-snowflake
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: 
 Home-page: https://www.grai.io/
 License: ELv2
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
-Requires-Dist: grai-client (>=0.3.0a10,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: snowflake-connector-python (>=3.0.0,<4.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-snowflake
 Description-Content-Type: text/markdown
```

