# Comparing `tmp/grai_source_mysql-0.1.0a3.tar.gz` & `tmp/grai_source_mysql-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_mysql-0.1.0a3.tar", max compression
+gzip compressed data, was "grai_source_mysql-0.1.0a4.tar", max compression
```

## Comparing `grai_source_mysql-0.1.0a3.tar` & `grai_source_mysql-0.1.0a4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      130 2023-05-02 08:01:59.696306 grai_source_mysql-0.1.0a3/README.md
--rw-r--r--   0        0        0     1064 2023-07-03 13:21:08.072867 grai_source_mysql-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      169 2023-07-03 13:21:10.765158 grai_source_mysql-0.1.0a3/src/grai_source_mysql/__init__.py
--rw-r--r--   0        0        0     8646 2023-06-29 12:17:13.075447 grai_source_mysql-0.1.0a3/src/grai_source_mysql/adapters.py
--rw-r--r--   0        0        0     1054 2023-07-03 13:20:59.551801 grai_source_mysql-0.1.0a3/src/grai_source_mysql/base.py
--rw-r--r--   0        0        0     8955 2023-06-06 17:35:16.817542 grai_source_mysql-0.1.0a3/src/grai_source_mysql/loader.py
--rw-r--r--   0        0        0     4779 2023-06-06 17:35:16.817671 grai_source_mysql-0.1.0a3/src/grai_source_mysql/models.py
--rw-r--r--   0        0        0      193 2023-06-06 17:35:16.817772 grai_source_mysql-0.1.0a3/src/grai_source_mysql/package_definitions.py
--rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 grai_source_mysql-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0      130 2023-05-02 08:01:59.696306 grai_source_mysql-0.1.0a4/README.md
+-rw-r--r--   0        0        0     1064 2023-07-12 11:28:17.074456 grai_source_mysql-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-07-12 11:28:23.718780 grai_source_mysql-0.1.0a4/src/grai_source_mysql/__init__.py
+-rw-r--r--   0        0        0     8646 2023-07-12 10:52:48.726036 grai_source_mysql-0.1.0a4/src/grai_source_mysql/adapters.py
+-rw-r--r--   0        0        0     1054 2023-07-12 11:08:22.846990 grai_source_mysql-0.1.0a4/src/grai_source_mysql/base.py
+-rw-r--r--   0        0        0     8955 2023-06-06 17:35:16.817542 grai_source_mysql-0.1.0a4/src/grai_source_mysql/loader.py
+-rw-r--r--   0        0        0     4779 2023-06-06 17:35:16.817671 grai_source_mysql-0.1.0a4/src/grai_source_mysql/models.py
+-rw-r--r--   0        0        0      193 2023-06-06 17:35:16.817772 grai_source_mysql-0.1.0a4/src/grai_source_mysql/package_definitions.py
+-rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 grai_source_mysql-0.1.0a4/PKG-INFO
```

### Comparing `grai_source_mysql-0.1.0a3/pyproject.toml` & `grai_source_mysql-0.1.0a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "grai_source_mysql"
-version = "0.1.0-alpha3"
+version = "0.1.0-alpha4"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_mysql", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-mysql"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a10", allow-prereleases = true}
+grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 PyYAML = "^6.0"
 multimethod = "^1.8"
 mysql-connector-python = "^8.0.31"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
```

### Comparing `grai_source_mysql-0.1.0a3/src/grai_source_mysql/adapters.py` & `grai_source_mysql-0.1.0a4/src/grai_source_mysql/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_mysql-0.1.0a3/src/grai_source_mysql/base.py` & `grai_source_mysql-0.1.0a4/src/grai_source_mysql/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_mysql-0.1.0a3/src/grai_source_mysql/loader.py` & `grai_source_mysql-0.1.0a4/src/grai_source_mysql/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_mysql-0.1.0a3/src/grai_source_mysql/models.py` & `grai_source_mysql-0.1.0a4/src/grai_source_mysql/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_mysql-0.1.0a3/PKG-INFO` & `grai_source_mysql-0.1.0a4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-source-mysql
-Version: 0.1.0a3
+Version: 0.1.0a4
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
-Requires-Dist: grai-client (>=0.3.0a10,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: mysql-connector-python (>=8.0.31,<9.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-mysql
 Description-Content-Type: text/markdown
```

