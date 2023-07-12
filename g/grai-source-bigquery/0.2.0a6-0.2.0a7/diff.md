# Comparing `tmp/grai_source_bigquery-0.2.0a6.tar.gz` & `tmp/grai_source_bigquery-0.2.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.2.0a6.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.2.0a7.tar", max compression
```

## Comparing `grai_source_bigquery-0.2.0a6.tar` & `grai_source_bigquery-0.2.0a7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.2.0a6/README.md
--rw-r--r--   0        0        0     1123 2023-07-12 11:22:36.346381 grai_source_bigquery-0.2.0a6/pyproject.toml
--rw-r--r--   0        0        0      175 2023-07-12 11:22:42.500392 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     8786 2023-07-12 10:52:48.686859 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     1780 2023-07-12 11:10:32.464249 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0    14133 2023-07-12 10:52:48.688181 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     6222 2023-06-08 08:40:20.857764 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      199 2023-06-06 17:35:16.799326 grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 grai_source_bigquery-0.2.0a6/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.2.0a7/README.md
+-rw-r--r--   0        0        0     1123 2023-07-12 11:39:07.150675 grai_source_bigquery-0.2.0a7/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-12 11:39:11.251045 grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     8786 2023-07-12 10:52:48.686859 grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     1891 2023-07-12 11:38:41.594222 grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0    14133 2023-07-12 10:52:48.688181 grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     6222 2023-06-08 08:40:20.857764 grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      199 2023-06-06 17:35:16.799326 grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 grai_source_bigquery-0.2.0a7/PKG-INFO
```

### Comparing `grai_source_bigquery-0.2.0a6/pyproject.toml` & `grai_source_bigquery-0.2.0a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_bigquery"
-version = "0.2.0-alpha6"
+version = "0.2.0-alpha7"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_bigquery", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/base.py` & `grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,7 +48,12 @@
         return grai_nodes
 
     def edges(self):
         with self.connector.connect() as conn:
             connector_edges = conn.edges()
             grai_edges = adapt_to_client(connector_edges, self.source, self.version)
         return grai_edges
+
+    def ready(self) -> bool:
+        with self.connector.connect() as _:
+            pass
+        return True
```

### Comparing `grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/loader.py` & `grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.2.0a6/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.2.0a7/src/grai_source_bigquery/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.2.0a6/PKG-INFO` & `grai_source_bigquery-0.2.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-bigquery
-Version: 0.2.0a6
+Version: 0.2.0a7
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

