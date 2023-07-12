# Comparing `tmp/grai_source_bigquery-0.2.0a5.tar.gz` & `tmp/grai_source_bigquery-0.2.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.2.0a5.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.2.0a6.tar", max compression
```

## Comparing `grai_source_bigquery-0.2.0a5.tar` & `grai_source_bigquery-0.2.0a6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.2.0a5/README.md
--rw-r--r--   0        0        0     1122 2023-06-30 16:51:59.727823 grai_source_bigquery-0.2.0a5/pyproject.toml
--rw-r--r--   0        0        0      175 2023-06-30 16:52:04.348881 grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     8786 2023-06-29 08:12:22.800613 grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     1780 2023-06-30 16:19:05.042165 grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0    14133 2023-06-30 08:35:34.231658 grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     6222 2023-06-08 08:40:20.857764 grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      199 2023-06-06 17:35:16.799326 grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 grai_source_bigquery-0.2.0a5/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.2.0a6/README.md
+-rw-r--r--   0        0        0     1123 2023-07-12 11:22:36.346381 grai_source_bigquery-0.2.0a6/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-12 11:22:42.500392 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     8786 2023-07-12 10:52:48.686859 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     1780 2023-07-12 11:10:32.464249 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0    14133 2023-07-12 10:52:48.688181 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     6222 2023-06-08 08:40:20.857764 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      199 2023-06-06 17:35:16.799326 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 grai_source_bigquery-0.2.0a6/PKG-INFO
```

### Comparing `grai_source_bigquery-0.2.0a5/pyproject.toml` & `grai_source_bigquery-0.2.0a6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "grai_source_bigquery"
-version = "0.2.0-alpha5"
+version = "0.2.0-alpha6"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_bigquery", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-bigquery"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a9", allow-prereleases = true}
+grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 multimethod = "^1.8"
 google-cloud-bigquery = "^3.5.0"
 setuptools = "^67.1.0"
 google-cloud-logging = "^3.5.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/base.py` & `grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/loader.py` & `grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.2.0a5/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.2.0a5/PKG-INFO` & `grai_source_bigquery-0.2.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-source-bigquery
-Version: 0.2.0a5
+Version: 0.2.0a6
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-cloud-bigquery (>=3.5.0,<4.0.0)
 Requires-Dist: google-cloud-logging (>=3.5.0,<4.0.0)
-Requires-Dist: grai-client (>=0.3.0a9,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: setuptools (>=67.1.0,<68.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-bigquery
 Description-Content-Type: text/markdown
```

