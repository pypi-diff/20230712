# Comparing `tmp/grai_source_flat_file-0.1.0a1.tar.gz` & `tmp/grai_source_flat_file-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_flat_file-0.1.0a1.tar", max compression
+gzip compressed data, was "grai_source_flat_file-0.1.0a4.tar", max compression
```

## Comparing `grai_source_flat_file-0.1.0a1.tar` & `grai_source_flat_file-0.1.0a4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      165 2023-05-19 11:07:12.932554 grai_source_flat_file-0.1.0a1/README.md
--rw-r--r--   0        0        0     1066 2023-06-30 03:30:27.619158 grai_source_flat_file-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      177 2023-06-30 03:30:27.624589 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/__init__.py
--rw-r--r--   0        0        0     6885 2023-06-29 15:34:52.425608 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/adapters.py
--rw-r--r--   0        0        0      997 2023-06-29 15:34:52.425750 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/base.py
--rw-r--r--   0        0        0     2843 2023-06-14 21:02:53.377068 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/loader.py
--rw-r--r--   0        0        0     1094 2023-06-29 15:34:52.426279 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/models.py
--rw-r--r--   0        0        0      201 2023-06-01 16:01:43.263838 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/package_definitions.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 grai_source_flat_file-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-05-02 08:01:59.695925 grai_source_flat_file-0.1.0a4/README.md
+-rw-r--r--   0        0        0     1067 2023-07-12 11:25:52.631073 grai_source_flat_file-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-07-12 11:26:03.096747 grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/__init__.py
+-rw-r--r--   0        0        0     6877 2023-07-12 10:52:48.708909 grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/adapters.py
+-rw-r--r--   0        0        0     1196 2023-07-12 11:10:40.549534 grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/base.py
+-rw-r--r--   0        0        0     2841 2023-07-12 10:52:48.709217 grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/loader.py
+-rw-r--r--   0        0        0     1094 2023-07-12 10:52:48.709758 grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/models.py
+-rw-r--r--   0        0        0      201 2023-06-06 17:35:16.812326 grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/package_definitions.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 grai_source_flat_file-0.1.0a4/PKG-INFO
```

### Comparing `grai_source_flat_file-0.1.0a1/pyproject.toml` & `grai_source_flat_file-0.1.0a4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "grai_source_flat_file"
-version = "0.1.0-alpha1"
+version = "0.1.0-alpha4"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_flat_file", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-flat-file"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a3", allow-prereleases = true}
+grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 PyYAML = "^6.0"
 multimethod = "^1.8"
 pandas = "^1.4.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
```

### Comparing `grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/adapters.py` & `grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
     Raises:
 
     """
     return [adapt_to_client(item, source, version) for item in objs]
 
 
 @adapt_to_client.register
-def adapt_sequence_to_client(objs: Sequence, source: SourceSpec, version: Literal["v1"]) -> List:
+def adapt_list_to_client(objs: List, source: SourceSpec, version: Literal["v1"]) -> List:
     """
 
     Args:
         objs (Sequence):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
```

### Comparing `grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/base.py` & `grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,36 @@
-from typing import List, Tuple
+import os
+from typing import List, Optional, Tuple
 
-from grai_client.endpoints.client import BaseClient
 from grai_client.integrations.base import (
     CombinedNodesAndEdgesMixin,
-    GraiIntegrationImplementationV1,
+    GraiIntegrationImplementation,
 )
 from grai_schemas.base import SourcedEdge, SourcedNode
+from grai_schemas.v1.source import SourceV1
 
 from grai_source_flat_file.adapters import adapt_to_client
-from grai_source_flat_file.loader import build_nodes_and_edges
+from grai_source_flat_file.loader import LOADER_MAP, build_nodes_and_edges
 
 
-class DbtIntegration(CombinedNodesAndEdgesMixin, GraiIntegrationImplementationV1):
-    def __init__(self, client: BaseClient, source_name: str, file_name: str, namespace: str):
-        super().__init__(client, source_name)
+class FlatFileIntegration(CombinedNodesAndEdgesMixin, GraiIntegrationImplementation):
+    def __init__(
+        self,
+        file_name: str,
+        namespace: str,
+        source: SourceV1,
+        version: Optional[str] = None,
+    ):
+        super().__init__(source, version)
 
         self.file_name = file_name
         self.namespace = namespace
 
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         nodes, edges = build_nodes_and_edges(self.file_name, self.namespace)
-        nodes = adapt_to_client(nodes, self.source, self.client.id)
-        edges = adapt_to_client(edges, self.source, self.client.id)
+        nodes = adapt_to_client(nodes, self.source, self.version)
+        edges = adapt_to_client(edges, self.source, self.version)
         return nodes, edges
+
+    def ready(self) -> bool:
+        file_ext = os.path.splitext(self.file_name)[-1]
+        return file_ext in LOADER_MAP
```

### Comparing `grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/loader.py` & `grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,29 +17,31 @@
 
     Raises:
 
     """
     return os.path.splitext(file_name)[0]
 
 
+LOADER_MAP = {".csv": pd.read_csv, ".parquet": pd.read_parquet, ".feather": pd.read_feather}
+
+
 def load_file(file_name: str) -> pd.DataFrame:
     """
 
     Args:
         file_name (str):
 
     Returns:
 
     Raises:
 
     """
-    loader_map = {".csv": pd.read_csv, ".parquet": pd.read_parquet, ".feather": pd.read_feather}
     file_ext = os.path.splitext(file_name)[-1]
-    assert file_ext in loader_map, f"{file_ext} not supported. Choose one of {set(loader_map.keys())}"
-    return loader_map[file_ext](file_name)
+    assert file_ext in LOADER_MAP, f"{file_ext} not supported. Choose one of {set(LOADER_MAP.keys())}"
+    return LOADER_MAP[file_ext](file_name)
 
 
 def map_pandas_types(dtype) -> str:
     """
 
     Args:
         dtype:
```

### Comparing `grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/models.py` & `grai_source_flat_file-0.1.0a4/src/grai_source_flat_file/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.1.0a1/PKG-INFO` & `grai_source_flat_file-0.1.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-source-flat-file
-Version: 0.1.0a1
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
-Requires-Dist: grai-client (>=0.3.0a3,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-flat-file
 Description-Content-Type: text/markdown
```

