# Comparing `tmp/grai_source_fivetran-0.1.0a5.tar.gz` & `tmp/grai_source_fivetran-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.1.0a5.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.1.0a6.tar", max compression
```

## Comparing `grai_source_fivetran-0.1.0a5.tar` & `grai_source_fivetran-0.1.0a6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      420 2023-05-30 08:16:23.842412 grai_source_fivetran-0.1.0a5/README.md
--rw-r--r--   0        0        0     1178 2023-07-06 09:26:32.110948 grai_source_fivetran-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0      149 2023-07-06 09:26:59.661765 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     9006 2023-07-06 08:19:52.348308 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     2402 2023-07-06 08:19:52.348811 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-17 18:10:50.922218 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0   451222 2023-06-06 17:35:16.808504 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    69211 2023-06-06 17:35:16.809499 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    16682 2023-07-06 08:19:52.349407 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     2173 2023-06-06 17:35:16.809859 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     5452 2023-06-06 17:35:16.809979 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      199 2023-06-06 17:35:16.810077 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-17 18:10:50.924423 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 grai_source_fivetran-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-05-30 08:16:23.842412 grai_source_fivetran-0.1.0a6/README.md
+-rw-r--r--   0        0        0     1178 2023-07-12 11:24:59.655178 grai_source_fivetran-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-07-12 11:25:04.214489 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     9006 2023-07-12 10:52:48.704547 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     2513 2023-07-12 11:08:11.044481 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-17 18:10:50.922218 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0   451222 2023-06-06 17:35:16.808504 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    69211 2023-06-06 17:35:16.809499 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    17360 2023-07-12 10:52:48.704959 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     2173 2023-06-06 17:35:16.809859 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     5452 2023-06-06 17:35:16.809979 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      199 2023-06-06 17:35:16.810077 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-17 18:10:50.924423 grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 grai_source_fivetran-0.1.0a6/PKG-INFO
```

### Comparing `grai_source_fivetran-0.1.0a5/pyproject.toml` & `grai_source_fivetran-0.1.0a6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.1.0-alpha5"
+version = "0.1.0-alpha6"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
 readme = "README.md"
@@ -12,15 +12,15 @@
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran"
 documentation = "https://docs.grai.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.9.13"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a19", allow-prereleases = true}
+grai-client = {version = "^0.3.0a21", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 multimethod = "^1.8"
 fivetran = "^0.7.0"
 requests = "^2.28.1"
 python-dotenv = "^0.21.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/adapters.py` & `grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/base.py` & `grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,21 @@
             parallelization=parallelization,
             api_key=api_key,
             api_secret=api_secret,
             endpoint=endpoint,
             limit=limit,
         )
 
-    def validate_nodes_and_edges(self, nodes: List[SourcedNode], edges: List[SourcedEdge]):
+    def ready(self) -> bool:
+        self.connector.has_query_permissions()
+        return True
+
+    def validate_nodes_and_edges(
+        self, nodes: List[SourcedNode], edges: List[SourcedEdge]
+    ):
         """
 
         Args:
             nodes (List[Node]):
             edges (List[Edge]):
 
         Returns:
```

### Comparing `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/main.py` & `grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/fivetran_api/main.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/loader.py` & `grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Tuple,
     TypedDict,
     TypeVar,
     Union,
 )
 
 import requests
-from pydantic import BaseModel, BaseSettings, SecretStr, validator
+from pydantic import BaseModel, BaseSettings, Json, SecretStr, validator
 
 from grai_source_fivetran.fivetran_api.api_models import (
     ColumnMetadataResponse,
     ConnectorResponse,
     GroupResponse,
     SchemaMetadataResponse,
     TableMetadataResponse,
@@ -117,15 +117,15 @@
     def make_request(
         self,
         request: Callable[..., requests.Response],
         url: str,
         headers: Optional[Dict] = None,
         params: Optional[Dict] = None,
         **kwargs,
-    ) -> Dict:
+    ) -> Tuple[Dict, requests.Response]:
         """
 
         Args:
             request:
             url:
             headers:  (Default value = None)
             params:  (Default value = None)
@@ -434,63 +434,44 @@
     source: str
     destination: str
 
 
 NamespaceTypes = Union[Dict[str, Union[str, SourceDestinationDict]], str]
 
 
-def build_namespace_map(
-    connectors: Dict, namespace_map: Union[str, Optional[NamespaceTypes]], default_namespace: Optional[str]
+def process_base_namespace_map(
+    namespace_map: Optional[Union[str, Dict[str, Union[str, SourceDestinationDict]]]]
 ) -> Dict[str, NamespaceIdentifier]:
-    """
-
-    Args:
-        connectors (Dict):
-        namespace_map (Union[str, Optional[NamespaceTypes]]):
-        default_namespace (Optional[str]):
-
-    Returns:
-
-    Raises:
-
-    """
-    if namespace_map is None and default_namespace is None:
-        message = (
-            f"The FivetranGraiMapper requires a not null value for `default_namespace` and/or `namespaces. "
-            f"These values are used to identify which Fivetran connection id's belong to which associated "
-            f"Grai namespace. `default_namespace` will map a single namespace to ALL connection id's."
-            "This behavior can be overridden by `namespaces` which maps {connection_id -> "
-            "namespace} or {connection_id -> {source: namespace, destination: namespace}}"
-        )
-        raise ValueError(message)
-    elif isinstance(namespace_map, str):
-        namespace_map = json.loads(namespace_map)
-
     if namespace_map is None:
         namespace_map = {}
-    else:
+    elif isinstance(namespace_map, str):
+        try:
+            namespace_map = json.loads(namespace_map)
+        except:
+            message = f"The provided JSON string was invalid and could not be successfully parsed."
+            raise Exception(message)
+    elif isinstance(namespace_map, dict):
         message = (
             "The namespaces object should be a dictionary whose id's are Fivetran connector id's and whose values "
             "identify the Grai namespace associated with either the source or destination of the connector. "
             "The values can either be provided as a dictionary with the keys 'source' and 'destination' or ",
             "as strings identifying the Grai namespace you'd like to associate with both the source "
             "and destination.",
         )
         assert all(isinstance(v, (dict, str)) for v in namespace_map.values()), message
         assert all("source" in v and "destination" in v for v in namespace_map.values() if isinstance(v, dict)), message
+    else:
+        raise ValueError(f"namespace_map must be either a JSON string, a dictionary not {type(namespace_map)}")
+
+    result: Dict[str, NamespaceIdentifier] = {}
 
-    if default_namespace is not None:
-        namespace_map = namespace_map.copy()  # avoid modifying the users original argument
-        for k in connectors.keys():
-            namespace_map.setdefault(k, default_namespace)
-
-    return {
-        k: NamespaceIdentifier(source=v, destination=v) if isinstance(v, str) else NamespaceIdentifier(**v)
-        for k, v in namespace_map.items()
-    }
+    for k, v in namespace_map.items():
+        result[k] = NamespaceIdentifier(source=v, destination=v) if isinstance(v, str) else NamespaceIdentifier(**v)
+
+    return result
 
 
 class FivetranConnector(FivetranAPI):
     """ """
 
     def __init__(
         self,
@@ -501,30 +482,61 @@
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.parallelization = parallelization
         self.semaphore = asyncio.Semaphore(self.parallelization)
         self.http_runner = parallelize_http(self.semaphore)
         self.default_namespace = default_namespace
+        self._namespace_map_base = process_base_namespace_map(namespaces)
 
-        self.connectors = {conn.id: conn for conn in self.get_connectors() if conn.id is not None}
-        self.namespace_map = build_namespace_map(self.connectors, namespaces, self.default_namespace)
-        if self.default_namespace is None:
-            self.connectors = {k: v for k, v in self.connectors.items() if k in self.namespace_map}
+        self._namespace_map: Optional[Dict[str, NamespaceIdentifier]] = None
+        self._connectors: Optional[Dict[str, ConnectorResponse]] = None
 
         self.table_to_conn_map: Dict[str, str] = {}
         self.column_to_conn_map: Dict[str, str] = {}
         self.schemas: Dict[str, SchemaMetadataResponse] = {}
         self.tables: Dict[str, TableMetadataResponse] = {}
         self.columns: Dict[str, ColumnMetadataResponse] = {}
 
         self._nodes = None
         self._edges = None
         self.lineage_ready = False
 
+    def has_query_permissions(self):
+        try:
+            # Should check all of the required endpoints here since the API key can be scoped
+            self.get_all_groups(limit=1)
+            return True
+        except Exception as e:
+            return False
+
+    @property
+    def connectors(self) -> Dict[str, ConnectorResponse]:
+        if self._connectors is None:
+            self._connectors = {conn.id: conn for conn in self.get_connectors() if conn.id is not None}
+        return self._connectors
+
+    @property
+    def namespace_map(self):
+        if self._namespace_map is None:
+            namespace_map = self._namespace_map_base.copy()  # avoid modifying the users original argument
+            if self.default_namespace is not None:
+                identifier = NamespaceIdentifier(source=self.default_namespace, destination=self.default_namespace)
+                for k in self.connectors.keys():
+                    namespace_map.setdefault(k, identifier.copy())
+            else:
+                for k in self.connectors.keys():
+                    source_namespace = f"fivetran-{k}-source"
+                    destination_namespace = f"fivetran-{k}-destination"
+                    identifier = NamespaceIdentifier(source=source_namespace, destination=destination_namespace)
+                    namespace_map.setdefault(k, identifier)
+            self._namespace_map = namespace_map
+
+        return self._namespace_map
+
     def build_lineage(self):
         """ """
         connector_ids = [[conn_id] for conn_id in self.connectors.keys()]
         schemas = self.http_runner(self.get_schemas, arg_list=connector_ids)
         tables = self.http_runner(self.get_tables, arg_list=connector_ids)
         columns = self.http_runner(self.get_columns, arg_list=connector_ids)
```

### Comparing `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.1.0a6/src/grai_source_fivetran/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a5/PKG-INFO` & `grai_source_fivetran-0.1.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: grai-source-fivetran
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fivetran (>=0.7.0,<0.8.0)
-Requires-Dist: grai-client (>=0.3.0a19,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran
```

