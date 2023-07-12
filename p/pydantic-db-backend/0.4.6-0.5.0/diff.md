# Comparing `tmp/pydantic_db_backend-0.4.6.tar.gz` & `tmp/pydantic_db_backend-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.4.6.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.5.0.tar", max compression
```

## Comparing `pydantic_db_backend-0.4.6.tar` & `pydantic_db_backend-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.4.6/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.4.6/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     6242 2023-07-11 07:48:12.508755 pydantic_db_backend-0.4.6/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.4.6/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0     6703 2023-07-11 13:02:38.177598 pydantic_db_backend-0.4.6/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.4.6/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.4.6/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.4.6/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0      996 2023-07-11 13:06:46.348152 pydantic_db_backend-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.5.0/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     6872 2023-07-12 12:03:04.958498 pydantic_db_backend-0.5.0/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.5.0/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0     7703 2023-07-12 12:59:36.806580 pydantic_db_backend-0.5.0/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.5.0/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.5.0/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0      617 2023-07-12 08:51:34.282543 pydantic_db_backend-0.5.0/pydantic_db_backend/indexes.py
+-rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.5.0/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0      996 2023-07-12 13:00:59.529502 pydantic_db_backend-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.5.0/PKG-INFO
```

### Comparing `pydantic_db_backend-0.4.6/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.5.0/pydantic_db_backend/backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 import contextlib
 import datetime
 import json
 import logging
 import re
 from contextvars import ContextVar
-from typing import Type, Dict, List
+from typing import Type, Dict, List, Tuple
 
 from dotenv import load_dotenv
 from pydantic import BaseModel, Field
 
+from pydantic_db_backend.indexes import Index
 from pydantic_db_backend.utils import uid, utcnow, str_to_datetime_if_parseable
 
 log = logging.getLogger(__name__)
 
 backend_context_var = ContextVar('backend_context_var')
 backend_alias_context_var = ContextVar('backend_alias_context_var', default='default')
 
@@ -61,16 +62,23 @@
 
     @classmethod
     def get_uids(cls, model: Type[BackendModel], skip: int = 0, limit: int = 0, query_filter: dict | None = None,
                  sort: List | None = None) -> List[str]:
         return cls.backend().get_uids(model=model, skip=skip, limit=limit, query_filter=query_filter, sort=sort)
 
     @classmethod
-    def get_instances(cls, model: Type[BackendModel], skip: int = 0, limit: int = 0, query_filter: dict | None = None,
-                      sort: List | None = None) -> List[BackendModel]:
+    def get_instances(
+        cls,
+        model: Type[BackendModel],
+        skip: int = 0,
+        limit: int = 0,
+        query_filter: dict | None = None,
+        sort: List | None = None,
+        max_results: bool | None = False
+    ) -> Tuple[List[BackendModel], int]:
         return cls.backend().get_instances(model=model, skip=skip, limit=limit, query_filter=query_filter, sort=sort)
 
     @classmethod
     def delete_uid(cls, model: Type[BackendModel], uid: str) -> None:
         return cls.backend().delete_uid(model=model, uid=uid)
 
     @classmethod
@@ -106,35 +114,42 @@
     def collection_name(cls, model: Type[BaseModel]) -> str:
         if model not in cls._collections:
             name = re.sub('([A-Z]+)', r'_\1', model.__name__).lower().removeprefix("_").removesuffix("_model")
             cls._collections[model] = name
         return cls._collections[model]
 
     @classmethod
-    def indexes(cls, model: Type[BaseModel], create_index_kwargs: dict | None, force_index_creation: bool = False) -> str:
+    def indexes(
+        cls,
+        model: Type[BaseModel],
+        create_index_kwargs: dict | None,
+        force_index_creation: bool = False
+    ) -> List[Index]:
         if model not in cls._indexes or force_index_creation:
-            index = cls.create_indexes(model, create_index_kwargs)
-            cls._indexes[model] = index
+            indexes = cls.create_indexes(model, create_index_kwargs)
+            cls._indexes[model] = indexes
         return cls._indexes[model]
 
     @classmethod
-    def create_indexes(cls, model: Type[BaseModel], create_index_kwargs: dict | None):
+    def create_indexes(cls, model: Type[BaseModel], create_index_kwargs: dict | None) -> List[Index]:
 
         if not hasattr(model, "Config"):
             return True
 
         if not hasattr(model.Config, "backend_indexes"):
             return True
 
-        for index_name, index_spec in model.Config.backend_indexes:
-            cls.create_index(cls.collection_name(model), index_name, index_spec, **create_index_kwargs)
+        indexes = model.Config.backend_indexes
+        for index in indexes:
+            cls.create_index(cls.collection_name(model), index, **create_index_kwargs)
+        return indexes
 
     @classmethod
-    def create_index(cls, collection_name: str, index_name: str, index_spec: list, **kwargs):
-        log.debug(f"[{collection_name}] Creating index {index_name}...")
+    def create_index(cls, collection_name: str, index: Index, **kwargs):
+        log.debug(f"[{collection_name}] Creating {index.type} index {index.name}...")
 
     @classmethod
     def to_db(cls, instance: BackendModel, json_dict: bool | None = True) -> dict:
         instance.updated_time = utcnow()
         return json.loads(instance.json()) if json_dict else instance.dict()
 
     @classmethod
@@ -146,22 +161,44 @@
         raise NotImplementedError
 
     @classmethod
     def post_instance(cls, instance: BackendModel) -> BackendModel:
         raise NotImplementedError
 
     @classmethod
-    def get_uids(cls, model: Type[BackendModel], skip: int = 0, limit: int = 0, query_filter: dict | None = None,
-                 sort: List | None = None) -> List[str]:
+    def get_uids(
+        cls,
+        model: Type[BackendModel],
+        skip: int = 0,
+        limit: int = 0,
+        query_filter: dict | None = None,
+        sort: List | None = None,
+        max_results: bool | None = False
+    ) -> Tuple[List[str], int]:
         raise NotImplementedError
 
     @classmethod
-    def get_instances(cls, model: Type[BackendModel], skip: int = 0, limit: int = 0, query_filter: dict | None = None,
-                      sort: List | None = None) -> List[BackendModel]:
-        raise NotImplementedError
+    def get_instances(
+        cls,
+        model: Type[BackendModel],
+        skip: int = 0,
+        limit: int = 0,
+        query_filter: dict = None,
+        sort: List = None,
+        max_results: bool = False,
+    ) -> Tuple[List[BackendModel], int]:
+        ids, max_results = cls.get_uids(
+            model=model,
+            skip=skip,
+            limit=limit,
+            query_filter=query_filter,
+            sort=sort,
+            max_results=max_results
+        )
+        return [cls.get_instance(model, uid=x) for x in ids], max_results
 
     @classmethod
     def delete_uid(cls, model: Type[BackendModel], uid: str) -> None:
         raise NotImplementedError
 
     @classmethod
     def delete_collection(cls, model: Type[BackendModel]) -> None:
```

### Comparing `pydantic_db_backend-0.4.6/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.5.0/pydantic_db_backend/backends/couchdb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
-from typing import Dict, Type, List
+from typing import Dict, Type, List, Tuple
 
 import pydash
 from couchdb import ResourceConflict, ServerError
 from pydantic import BaseModel, Field
 
 import couchdb
 from pydantic_db_backend.backend import BackendBase, BackendModel
 from pydantic_db_backend.exceptions import RevisionConflict, NotFound, AlreadyExists
+from pydantic_db_backend.indexes import Index, SortingIndex, AggregationIndex
 from pydantic_db_backend.utils import CustomJSONEncoder
 
 log = logging.getLogger(__name__)
 
 
 class CouchDbBackend(BackendBase):
     # _collections: Dict[Type[BaseModel], str] = {}
@@ -51,20 +52,55 @@
             },
             "_id", "_rev"
         )
         return super().from_db(model, document)
 
     # noinspection PyMethodOverriding
     @classmethod
-    def create_index(cls, collection_name: str, index_name: str, index_spec: list, db: couchdb.Database):
-        super().create_index(collection_name, index_name, index_spec)
-        i = (collection_name, index_name)
-        indexes = db.index()
-        if i not in indexes:
-            indexes[i] = index_spec
+    def create_index(cls, collection_name: str, index: Index, db: couchdb.Database):
+        super().create_index(collection_name, index)
+
+        if index.type == "sorting":
+            index: SortingIndex
+
+            i = (collection_name, index.name)
+            indexes = db.index()
+
+            # noinspection PyUnboundLocalVariable
+            if i not in indexes:
+                indexes[i] = index.sorting
+
+        elif index.type == "aggregation":
+            index: AggregationIndex
+            cls.view_from_aggregation_index(db, collection_name, index)
+
+
+        else:
+            pass
+
+    @classmethod
+    def view_from_aggregation_index(cls, db: couchdb.Database, collection_name: str, index: AggregationIndex):
+        design_document = f"_design/{collection_name}_{index.name}"
+        if design_document not in db:
+            field, func = next(iter(index.spec.items()))
+            map_function = f"function (doc) {{ emit(doc.{field}, 1); }}"
+            # reduce_function = f"function(keys, values, rereduce) {{ return sum(values); }}"
+            data = {
+                "_id": design_document,
+                "views": {
+                    (index.name): {
+                        "map": map_function,
+                        "reduce": func
+                    }
+                },
+                "language": "javascript",
+                "options": {"partitioned": False}
+            }
+            logging.info(f"creating view {collection_name}_{index.name}/{index.name}")
+            db.save(data)
 
     @classmethod
     def get_db(cls, model: Type[BackendModel]) -> couchdb.Database:
         db_name = cls.collection_name(model)
 
         with cls.alias() as alias:
             con = cls._connections[alias]
@@ -132,38 +168,40 @@
     @classmethod
     def get_uids(
         cls,
         model: Type[BackendModel],
         skip: int = 0,
         limit: int = 25,
         query_filter: dict = None,
-        sort: List = None
-    ) -> List[str]:
+        sort: List = None,
+        max_results: bool | None = False
+    ) -> Tuple[List[str], int]:
 
         # fix 0 limit, since couchdb does not know this
         limit = 9999999 if limit == 0 else limit
 
         if query_filter is None:
             query_filter = {}
 
         # convert to json and back again, to have iso datetime strings
         query_filter = json.loads(json.dumps(query_filter, cls=CustomJSONEncoder))
 
         db = cls.get_db(model)
 
-
         find_dict = {
             "selector": query_filter,
             "skip": skip,
             "limit": limit,
             "fields": ['_id']
         }
         if sort is not None:
             find_dict["sort"] = sort
 
+        max_results = 0
+
         try:
             find_result = db.find(find_dict)
         except ServerError as e:
 
             error_code = pydash.get(e, ["args", 0, 0])
 
             if error_code == 400:
@@ -171,27 +209,15 @@
                 # index cache and initiate a new get_db... and a loop
                 cls.indexes(model, dict(db=db), force_index_creation=True)
                 find_result = db.find(find_dict)
             else:
                 raise e
 
         result = [x["_id"] for x in find_result]
-        return result
-
-    @classmethod
-    def get_instances(
-        cls,
-        model: Type[BackendModel],
-        skip: int = 0,
-        limit: int = 0,
-        query_filter: dict = None,
-        sort: List = None
-    ) -> List[BackendModel]:
-        ids = cls.get_uids(model=model, skip=skip, limit=limit, query_filter=query_filter, sort=sort)
-        return [cls.get_instance(model, uid=x) for x in ids]
+        return result, max_results
 
     @classmethod
     def delete_collection(cls, model: Type[BackendModel]) -> None:
         with cls.alias() as alias:
             server = cls._connections[alias].server
             name = cls.collection_name(model)
             if name in server:
```

### Comparing `pydantic_db_backend-0.4.6/pydantic_db_backend/exceptions/__init__.py` & `pydantic_db_backend-0.5.0/pydantic_db_backend/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.6/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.5.0/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.4.6/pyproject.toml` & `pydantic_db_backend-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.4.6"
+version = "0.5.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^0.15.0"
```

### Comparing `pydantic_db_backend-0.4.6/PKG-INFO` & `pydantic_db_backend-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.4.6
+Version: 0.5.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
```

