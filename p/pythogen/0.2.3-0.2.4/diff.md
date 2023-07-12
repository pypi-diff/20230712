# Comparing `tmp/pythogen-0.2.3.tar.gz` & `tmp/pythogen-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.2.3.tar", max compression
+gzip compressed data, was "pythogen-0.2.4.tar", max compression
```

## Comparing `pythogen-0.2.3.tar` & `pythogen-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-07-12 06:57:41.508891 pythogen-0.2.3/LICENSE
--rw-r--r--   0        0        0     2097 2023-07-12 06:57:41.508891 pythogen-0.2.3/README.md
--rw-r--r--   0        0        0     1567 2023-07-12 06:57:41.512891 pythogen-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1585 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/entrypoint.py
--rw-r--r--   0        0        0     7492 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/models.py
--rw-r--r--   0        0        0     2329 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3307 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/document.py
--rw-r--r--   0        0        0      576 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3239 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2132 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2437 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1074 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3512 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1810 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/response.py
--rw-r--r--   0        0        0    16516 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0    10343 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/renderer.py
--rw-r--r--   0        0        0      172 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/settings.py
--rw-r--r--   0        0        0     5149 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/client/httpx-method.j2
--rw-r--r--   0        0        0     1668 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/client/httpx-request-metrics.j2
--rw-r--r--   0        0        0    11127 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/httpx.j2
--rw-r--r--   0        0        0       33 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/init-py.j2
--rw-r--r--   0        0        0      312 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 09:47:38.443211 pythogen-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2097 2023-07-12 09:47:38.443211 pythogen-0.2.4/README.md
+-rw-r--r--   0        0        0     1567 2023-07-12 09:47:38.447211 pythogen-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1585 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/entrypoint.py
+-rw-r--r--   0        0        0     7531 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/models.py
+-rw-r--r--   0        0        0     2329 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3239 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-12 09:47:38.447211 pythogen-0.2.4/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    17663 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0    10011 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/renderer.py
+-rw-r--r--   0        0        0      172 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/settings.py
+-rw-r--r--   0        0        0     5149 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/client/httpx-method.j2
+-rw-r--r--   0        0        0     1668 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/client/httpx-request-metrics.j2
+-rw-r--r--   0        0        0    11127 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/httpx.j2
+-rw-r--r--   0        0        0       33 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/init-py.j2
+-rw-r--r--   0        0        0      312 2023-07-12 09:47:38.451211 pythogen-0.2.4/pythogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.4/PKG-INFO
```

### Comparing `pythogen-0.2.3/LICENSE` & `pythogen-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/README.md` & `pythogen-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pyproject.toml` & `pythogen-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.2.3"
+version = "0.2.4"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
```

### Comparing `pythogen-0.2.3/pythogen/entrypoint.py` & `pythogen-0.2.4/pythogen/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/models.py` & `pythogen-0.2.4/pythogen/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     required: list[str] | None
     enum: list[str] | None
     type: Type
     format: Format | None
     items: 'SchemaObject' | list['SchemaObject'] | None
     properties: list[SchemaProperty]
     description: str | None = None
+    additional_roperties: bool = False
 
     # Технические поля
     discriminator_base_class_schema: DiscriminatorBaseClassSchema | None = None
     is_fake: bool = False
 
     @property
     def required_properties(self) -> list[SchemaProperty]:
```

### Comparing `pythogen-0.2.3/pythogen/packager.py` & `pythogen-0.2.4/pythogen/packager.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/parsers/document.py` & `pythogen-0.2.4/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.4/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/parsers/operations.py` & `pythogen-0.2.4/pythogen/parsers/operations.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/parsers/parameters.py` & `pythogen-0.2.4/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/parsers/paths.py` & `pythogen-0.2.4/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/parsers/references.py` & `pythogen-0.2.4/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/parsers/request_body.py` & `pythogen-0.2.4/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/parsers/response.py` & `pythogen-0.2.4/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/parsers/schemas.py` & `pythogen-0.2.4/pythogen/parsers/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import logging
 import re
 from collections import defaultdict
 from typing import Any
 
 from pythogen import models
 from pythogen.parsers.inline_schemas_aggregator import InlineSchemasAggregator
 from pythogen.parsers.references import RefResolver
 
 
+logger = logging.getLogger(__name__)
+
+
 PRIMITIVE_TYPES = ('string', 'number', 'integer', 'boolean', 'null')
 
 
 class SchemaParser:
     """Парсер схемы
 
     Парсит схему из коллекции схем, расположенных в поле components -> schemas
@@ -377,14 +381,35 @@
                             properties=[],
                             title=None,
                             format=None,
                             items=None,
                             required=None,
                         )
                     )
+                elif models.Type(any_ref_any_type) is models.Type.object:
+                    additional_roperties = any_ref_item.get('additionalProperties', False)
+                    if additional_roperties:
+                        item_schema_id = f'{parent_schema_id}Item'
+                        items.append(
+                            models.SchemaObject(
+                                id=item_schema_id,
+                                type=models.Type.object,
+                                enum=None,
+                                properties=[],
+                                title=None,
+                                format=None,
+                                items=None,
+                                required=None,
+                                additional_roperties=True,
+                            )
+                        )
+                elif models.Type(any_ref_any_type) is models.Type.array:
+                    schema_id = f'<inline+{models.SchemaObject.__name__}>'
+                    schema = self.parse_item(schema_id, any_ref_item)
+                    items.append(schema)
                 else:
-                    items_schema_id = f'<inline+{models.SchemaObject.__name__}>'
-                    schema = self.parse_item(items_schema_id, items_schema_data)  # type: ignore
-                    self._inline_schema_aggregator.add(items_schema_id, schema)
+                    schema_id = f'<inline+{models.SchemaObject.__name__}>'
+                    schema = self.parse_item(schema_id, any_ref_item)  # type: ignore
+                    self._inline_schema_aggregator.add(schema_id, schema)
             return items
 
         return None
```

### Comparing `pythogen-0.2.3/pythogen/renderer.py` & `pythogen-0.2.4/pythogen/renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -214,86 +214,81 @@
         return f'{types[0]} | None'
     else:
         return ' | '.join(types)
 
 
 def j2_typerepr(schema: models.SchemaObject, document: models.Document | None = None) -> str:
     """Represent data type on j2 template"""
-    primitive_type_mapping = {
-        models.Type.integer: 'int',
-        models.Type.number: 'float',
-        models.Type.boolean: 'bool',
-        models.Type.string: 'str',
-        models.Type.null: 'None',
-    }
-    format_mapping = {
-        models.Format.binary: 'bytes',
-        models.Format.uri: 'HttpUrl',
-        models.Format.date: 'datetime.date',
-        models.Format.date_time: 'datetime.datetime',
-    }
-
     # TODO: всегда передавать document в функцию
     if document:
         schema = document.schemas.get(schema.id, schema)
 
     representation = 'dict'
 
-    if schema.type in primitive_type_mapping:
-        if schema.enum and schema.id == '<inline+SchemaObject>':
-            representation = f'Literal{schema.enum}'
-        elif schema.enum:
-            representation = schema.id
-        elif schema.format in format_mapping:
-            representation = format_mapping[schema.format]  # type: ignore
+    if schema.type in PRIMITIVE_TYPE_MAPPING:
+        if schema.enum:
+            if schema.id == '<inline+SchemaObject>':
+                representation = f'Literal{schema.enum}'
+            else:
+                representation = classname(schema.id)
+        elif schema.format in FORMAT_MAPPING:
+            representation = FORMAT_MAPPING[schema.format]  # type: ignore
         else:
-            representation = primitive_type_mapping[schema.type]
+            representation = PRIMITIVE_TYPE_MAPPING[schema.type]
 
     elif schema.type == models.Type.object and schema.id != '<inline+SchemaObject>':
         representation = classname(schema.id)
 
     elif schema.type == models.Type.array and schema.items:
         if schema.items.type is models.Type.any_of:  # type: ignore
-            class_items = []
-            primitive_items = []
-            for item in schema.items.items:  # type: ignore
-                if item.id:
-                    class_items.append(classname(item.id))
-                else:
-                    primitive_items.append(primitive_type_mapping[item.type])
-
-            class_items_str = ' | '.join([f'{class_item}' for class_item in class_items])
-            primitives_items_str = ' | '.join(primitive_items)
-
-            items = []
-            if class_items_str:
-                items.append(class_items_str)
-            if primitives_items_str:
-                items.append(primitives_items_str)
-
-            items_str = ' | '.join(items)
-            representation = f'list[{items_str}]'
+            list_items_repr = _repr_any_of_schema(schema.items.items)  # type: ignore
+            representation = f'list[{list_items_repr}]'
         else:
             item = j2_typerepr(schema.items)  # type: ignore
             representation = f'list[{item}]'
 
     elif schema.type is models.Type.any_of:
-        items = []
-        for item in schema.items:  # type: ignore
-            if item.id:
-                items.append(classname(item.id))
-            else:
-                if item.type is models.Type.null and not item.required:
-                    continue
-                items.append(primitive_type_mapping[item.type])
-        representation = ' | '.join(items)
+        representation = _repr_any_of_schema(schema.items)  # type: ignore
 
     return representation
 
 
+def _repr_any_of_schema(any_of_items: list[models.SchemaObject]) -> str:
+    items = []
+    for item in any_of_items:
+        if item.additional_roperties:
+            items.append('dict[Any, Any]')
+        elif item.type is models.Type.array and item.items:
+            repr = j2_typerepr(item)
+            items.append(repr)
+        elif item.id:
+            items.append(classname(item.id))
+        else:
+            if item.type is models.Type.null and not item.required:
+                continue
+            items.append(PRIMITIVE_TYPE_MAPPING[item.type])
+    return ' | '.join(items)
+
+
 def varname(value: str) -> str:
     return inflection.underscore(value)
 
 
 def classname(value: str) -> str:
     value = value.replace('.', '')
     return inflection.camelize(value)
+
+
+PRIMITIVE_TYPE_MAPPING = {
+    models.Type.integer: 'int',
+    models.Type.number: 'float',
+    models.Type.boolean: 'bool',
+    models.Type.string: 'str',
+    models.Type.null: 'None',
+}
+
+FORMAT_MAPPING = {
+    models.Format.binary: 'bytes',
+    models.Format.uri: 'HttpUrl',
+    models.Format.date: 'datetime.date',
+    models.Format.date_time: 'datetime.datetime',
+}
```

### Comparing `pythogen-0.2.3/pythogen/templates/client/httpx-method.j2` & `pythogen-0.2.4/pythogen/templates/client/httpx-method.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/templates/client/httpx-request-metrics.j2` & `pythogen-0.2.4/pythogen/templates/client/httpx-request-metrics.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/pythogen/templates/httpx.j2` & `pythogen-0.2.4/pythogen/templates/httpx.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.3/PKG-INFO` & `pythogen-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.2.3
+Version: 0.2.4
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.10,<4.0
```

