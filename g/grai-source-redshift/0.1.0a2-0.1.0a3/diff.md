# Comparing `tmp/grai_source_redshift-0.1.0a2.tar.gz` & `tmp/grai_source_redshift-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_redshift-0.1.0a2.tar", max compression
+gzip compressed data, was "grai_source_redshift-0.1.0a3.tar", max compression
```

## Comparing `grai_source_redshift-0.1.0a2.tar` & `grai_source_redshift-0.1.0a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-05-02 08:01:59.696812 grai_source_redshift-0.1.0a2/README.md
--rw-r--r--   0        0        0     1152 2023-06-30 17:13:40.681173 grai_source_redshift-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      175 2023-06-30 11:57:45.156662 grai_source_redshift-0.1.0a2/src/grai_source_redshift/__init__.py
--rw-r--r--   0        0        0     9040 2023-06-29 12:38:00.344732 grai_source_redshift-0.1.0a2/src/grai_source_redshift/adapters.py
--rw-r--r--   0        0        0     1058 2023-06-30 17:13:40.681405 grai_source_redshift-0.1.0a2/src/grai_source_redshift/base.py
--rw-r--r--   0        0        0     8092 2023-06-06 17:35:16.820909 grai_source_redshift-0.1.0a2/src/grai_source_redshift/loader.py
--rw-r--r--   0        0        0     5080 2023-06-06 17:35:16.821232 grai_source_redshift-0.1.0a2/src/grai_source_redshift/models.py
--rw-r--r--   0        0        0      199 2023-06-06 17:35:16.821468 grai_source_redshift-0.1.0a2/src/grai_source_redshift/package_definitions.py
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 grai_source_redshift-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-02 08:01:59.696812 grai_source_redshift-0.1.0a3/README.md
+-rw-r--r--   0        0        0     1152 2023-07-12 11:29:01.662558 grai_source_redshift-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-12 11:29:06.491842 grai_source_redshift-0.1.0a3/src/grai_source_redshift/__init__.py
+-rw-r--r--   0        0        0     9040 2023-07-12 10:52:48.739993 grai_source_redshift-0.1.0a3/src/grai_source_redshift/adapters.py
+-rw-r--r--   0        0        0     1058 2023-07-12 11:08:33.029031 grai_source_redshift-0.1.0a3/src/grai_source_redshift/base.py
+-rw-r--r--   0        0        0     8092 2023-06-06 17:35:16.820909 grai_source_redshift-0.1.0a3/src/grai_source_redshift/loader.py
+-rw-r--r--   0        0        0     5080 2023-06-06 17:35:16.821232 grai_source_redshift-0.1.0a3/src/grai_source_redshift/models.py
+-rw-r--r--   0        0        0      199 2023-06-06 17:35:16.821468 grai_source_redshift-0.1.0a3/src/grai_source_redshift/package_definitions.py
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 grai_source_redshift-0.1.0a3/PKG-INFO
```

### Comparing `grai_source_redshift-0.1.0a2/pyproject.toml` & `grai_source_redshift-0.1.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "grai_source_redshift"
-version = "0.1.0-alpha2"
+version = "0.1.0-alpha3"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_redshift", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-redshift"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-grai-client = {version = "^0.3.0a10", allow-prereleases = true}
+grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 multimethod = "^1.8"
 pydantic = {extras = ["dotenv"], version = "^1.10.7"}
 botocore = "^1.29.153"
 redshift-connector = "^2.0.911"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `grai_source_redshift-0.1.0a2/src/grai_source_redshift/adapters.py` & `grai_source_redshift-0.1.0a3/src/grai_source_redshift/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.1.0a2/src/grai_source_redshift/base.py` & `grai_source_redshift-0.1.0a3/src/grai_source_redshift/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.1.0a2/src/grai_source_redshift/loader.py` & `grai_source_redshift-0.1.0a3/src/grai_source_redshift/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.1.0a2/src/grai_source_redshift/models.py` & `grai_source_redshift-0.1.0a3/src/grai_source_redshift/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.1.0a2/PKG-INFO` & `grai_source_redshift-0.1.0a3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-source-redshift
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
 Requires-Dist: botocore (>=1.29.153,<2.0.0)
-Requires-Dist: grai-client (>=0.3.0a10,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
 Requires-Dist: redshift-connector (>=2.0.911,<3.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-redshift
 Description-Content-Type: text/markdown
```

