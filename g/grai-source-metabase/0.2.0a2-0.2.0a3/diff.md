# Comparing `tmp/grai_source_metabase-0.2.0a2.tar.gz` & `tmp/grai_source_metabase-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_metabase-0.2.0a2.tar", max compression
+gzip compressed data, was "grai_source_metabase-0.2.0a3.tar", max compression
```

## Comparing `grai_source_metabase-0.2.0a2.tar` & `grai_source_metabase-0.2.0a3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       28 2023-07-11 08:47:36.897894 grai_source_metabase-0.2.0a2/README.md
--rw-r--r--   0        0        0      797 2023-07-11 11:31:01.372995 grai_source_metabase-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0      156 2023-07-11 11:31:04.313661 grai_source_metabase-0.2.0a2/src/grai_source_metabase/__init__.py
--rw-r--r--   0        0        0    11025 2023-07-11 08:47:41.694755 grai_source_metabase-0.2.0a2/src/grai_source_metabase/adapters.py
--rw-r--r--   0        0        0     1730 2023-07-11 08:47:41.694831 grai_source_metabase-0.2.0a2/src/grai_source_metabase/base.py
--rw-r--r--   0        0        0    10514 2023-07-11 11:30:46.285459 grai_source_metabase-0.2.0a2/src/grai_source_metabase/loader.py
--rw-r--r--   0        0        0     3223 2023-07-11 08:47:41.695259 grai_source_metabase-0.2.0a2/src/grai_source_metabase/mock_tools.py
--rw-r--r--   0        0        0      783 2023-07-11 08:47:41.695829 grai_source_metabase-0.2.0a2/src/grai_source_metabase/models.py
--rw-r--r--   0        0        0      186 2023-07-11 08:47:41.697283 grai_source_metabase-0.2.0a2/src/grai_source_metabase/package_definitions.py
--rw-r--r--   0        0        0        0 2023-07-11 08:47:41.697516 grai_source_metabase-0.2.0a2/src/grai_source_metabase/py.typed
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 grai_source_metabase-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-07-12 10:52:48.711263 grai_source_metabase-0.2.0a3/README.md
+-rw-r--r--   0        0        0      797 2023-07-12 11:26:58.645780 grai_source_metabase-0.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-07-12 11:27:04.503039 grai_source_metabase-0.2.0a3/src/grai_source_metabase/__init__.py
+-rw-r--r--   0        0        0    11025 2023-07-12 10:52:48.713594 grai_source_metabase-0.2.0a3/src/grai_source_metabase/adapters.py
+-rw-r--r--   0        0        0     1479 2023-07-12 11:09:57.278686 grai_source_metabase-0.2.0a3/src/grai_source_metabase/base.py
+-rw-r--r--   0        0        0    10362 2023-07-12 10:52:48.714073 grai_source_metabase-0.2.0a3/src/grai_source_metabase/loader.py
+-rw-r--r--   0        0        0     3223 2023-07-11 15:52:49.389383 grai_source_metabase-0.2.0a3/src/grai_source_metabase/mock_tools.py
+-rw-r--r--   0        0        0      783 2023-07-11 08:47:41.695829 grai_source_metabase-0.2.0a3/src/grai_source_metabase/models.py
+-rw-r--r--   0        0        0      186 2023-07-11 08:47:41.697283 grai_source_metabase-0.2.0a3/src/grai_source_metabase/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-07-11 15:52:49.389459 grai_source_metabase-0.2.0a3/src/grai_source_metabase/py.typed
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 grai_source_metabase-0.2.0a3/PKG-INFO
```

### Comparing `grai_source_metabase-0.2.0a2/src/grai_source_metabase/adapters.py` & `grai_source_metabase-0.2.0a3/src/grai_source_metabase/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.2.0a2/src/grai_source_metabase/base.py` & `grai_source_metabase-0.2.0a3/src/grai_source_metabase/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Dict, List, Literal, Optional, Tuple, Union
+from typing import Dict, List, Optional, Union
 
-from grai_client.endpoints.client import BaseClient
-from grai_client.integrations.base import GraiIntegrationImplementation
-from grai_client.update import update
-from grai_schemas.base import Edge, Node, SourcedEdge, SourcedNode
+from grai_client.integrations.base import (
+    GraiIntegrationImplementation,
+    SeparateNodesAndEdgesMixin,
+)
+from grai_schemas.base import SourcedEdge, SourcedNode
 from grai_schemas.v1.source import SourceV1
 
 from grai_source_metabase.adapters import adapt_to_client
 from grai_source_metabase.loader import MetabaseConnector
 
 
-class MetabaseIntegration(GraiIntegrationImplementation):
+class MetabaseIntegration(SeparateNodesAndEdgesMixin, GraiIntegrationImplementation):
     def __init__(
         self,
         source: SourceV1,
         version: Optional[str] = None,
         metabase_namespace: Optional[str] = None,
         namespace_map: Optional[Union[str, Dict[int, str]]] = None,
         endpoint: Optional[str] = None,
@@ -28,23 +29,17 @@
             namespace_map=namespace_map,
             username=username,
             password=password,
             endpoint=endpoint,
         )
 
     def ready(self) -> bool:
-        try:
-            self.connector.authenticate()
-            return True
-        except Exception as e:
-            return False
+        self.connector.authenticate()
+        return True
 
     def nodes(self) -> List[SourcedNode]:
         nodes = adapt_to_client(self.connector.get_nodes(), self.source, self.version)
         return nodes
 
     def edges(self) -> List[SourcedEdge]:
         edges = adapt_to_client(self.connector.get_edges(), self.source, self.version)
         return edges
-
-    def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
-        return self.nodes(), self.edges()
```

### Comparing `grai_source_metabase-0.2.0a2/src/grai_source_metabase/loader.py` & `grai_source_metabase-0.2.0a3/src/grai_source_metabase/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import cached_property
 from itertools import chain
 from typing import Callable, Dict, List, Optional, TypedDict, Union
 
 import requests
 from pydantic import (
+    AnyHttpUrl,
     BaseModel,
     BaseSettings,
-    AnyHttpUrl,
     Json,
     SecretStr,
     parse_obj_as,
     validator,
 )
 from requests.exceptions import ConnectionError
 from retrying import retry
@@ -52,17 +52,15 @@
     ):
         passthrough_kwargs = {
             "username": username,
             "password": password,
             "endpoint": endpoint,
         }
 
-        self.config = MetabaseConfig(
-            **{k: v for k, v in passthrough_kwargs.items() if v is not None}
-        )
+        self.config = MetabaseConfig(**{k: v for k, v in passthrough_kwargs.items() if v is not None})
         self.api_endpoint = f"{self.config.endpoint}/api"
 
         self.session = requests.Session()
         self.session.headers.update({"Content-Type": "application/json"})
         self.session.headers.update(self.authenticate())
 
     @retry(stop_max_attempt_number=3, wait_fixed=5000)
@@ -154,17 +152,15 @@
             dict: The JSON response containing the list of collections.
 
         """
 
         pass
 
 
-def build_namespace_map(
-    default_map: Dict[int, str], dbs: Dict, metabase_namespace: str
-) -> Dict[int, str]:
+def build_namespace_map(default_map: Dict[int, str], dbs: Dict, metabase_namespace: str) -> Dict[int, str]:
     namespace_map = default_map.copy()
 
     for k, v in dbs.items():
         db_id_ns = f"{metabase_namespace}.{k}.{v['name']}"
         namespace_map.setdefault(k, db_id_ns)
 
     return namespace_map
@@ -220,50 +216,41 @@
 
         super().__init__(*args, **kwargs)
         self.base_namespace_map = namespace_map
         self.metabase_namespace = metabase_namespace
 
     @cached_property
     def namespace_map(self):
-        return build_namespace_map(
-            self.base_namespace_map, self.dbs_map, self.metabase_namespace
-        )
+        return build_namespace_map(self.base_namespace_map, self.dbs_map, self.metabase_namespace)
 
     @cached_property
     def tables(self) -> List[Dict]:
         # This line creates a list of tables by modifying each table dictionary obtained from the get_tables() method.
         # It replaces the "schema" key with a new key "schema_name" while preserving the other key-value pairs.
         # this is because the "schema" key is a reserved keyword in the pydantic.
-        return [
-            {**table, "schema_name": table.pop("schema")} for table in self.get_tables()
-        ]
+        return [{**table, "schema_name": table.pop("schema")} for table in self.get_tables()]
 
     @cached_property
     def tables_map(self) -> Dict:
         return {table["id"]: table for table in self.tables if table["active"]}
 
     @cached_property
     def dbs_map(self) -> Dict:
         return {db["id"]: db for db in self.get_dbs()["data"]}
 
     @cached_property
     def questions_map(self) -> Dict:
-        return {
-            question["id"]: question
-            for question in self.get_questions()
-            if question["archived"] is False
-        }
+        return {question["id"]: question for question in self.get_questions() if question["archived"] is False}
 
     @cached_property
     def question_table_map(self) -> Dict:
         return {
             question["id"]: question["table_id"]
             for question in self.questions_map.values()
-            if question["table_id"]
-            and self.tables_map.get(question["table_id"]) is not None
+            if question["table_id"] and self.tables_map.get(question["table_id"]) is not None
         }
 
     @cached_property
     def table_db_map(self) -> Dict:
         return {
             table["id"]: table["db_id"]
             for table in self.tables
@@ -281,17 +268,15 @@
 
         for question in self.questions_map.values():
             question["namespace"] = self.metabase_namespace
 
         for table in self.tables_map.values():
             table["namespace"] = self.namespace_map[self.table_db_map[table["id"]]]
 
-        verified_questions = [
-            Question(**question) for question in self.questions_map.values()
-        ]
+        verified_questions = [Question(**question) for question in self.questions_map.values()]
         verified_tables = [Table(**table) for table in self.tables_map.values()]
         nodes = chain(verified_questions, verified_tables)
 
         return list(nodes)
 
     def get_edges(self) -> List[Edge]:
         """
```

### Comparing `grai_source_metabase-0.2.0a2/src/grai_source_metabase/mock_tools.py` & `grai_source_metabase-0.2.0a3/src/grai_source_metabase/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.2.0a2/src/grai_source_metabase/models.py` & `grai_source_metabase-0.2.0a3/src/grai_source_metabase/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.2.0a2/PKG-INFO` & `grai_source_metabase-0.2.0a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: grai-source-metabase
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: 
 Author: Elseagle
 Author-email: dowolebolu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: grai-client (>=0.3.0-alpha18,<0.4.0)
-Requires-Dist: grai-schemas (>=0.2.0-alpha4,<0.3.0)
+Requires-Dist: grai-client (>=0.3.0-alpha21,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0-alpha5,<0.3.0)
 Requires-Dist: multimethod (>=1.9.1,<2.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: retrying (>=1.3.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Grai Metabase Integration
```

