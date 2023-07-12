# Comparing `tmp/pythogen-0.2.2.tar.gz` & `tmp/pythogen-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.2.2.tar", max compression
+gzip compressed data, was "pythogen-0.2.3.tar", max compression
```

## Comparing `pythogen-0.2.2.tar` & `pythogen-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-07-11 12:27:36.792956 pythogen-0.2.2/LICENSE
--rw-r--r--   0        0        0     2097 2023-07-11 12:27:36.792956 pythogen-0.2.2/README.md
--rw-r--r--   0        0        0     1567 2023-07-11 12:27:36.796956 pythogen-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1585 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/entrypoint.py
--rw-r--r--   0        0        0     7474 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/models.py
--rw-r--r--   0        0        0     2329 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3307 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/document.py
--rw-r--r--   0        0        0      576 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3239 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2132 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2437 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1074 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3512 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1810 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/parsers/response.py
--rw-r--r--   0        0        0    16508 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0     9987 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/renderer.py
--rw-r--r--   0        0        0      172 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/settings.py
--rw-r--r--   0        0        0     5149 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/client/httpx-method.j2
--rw-r--r--   0        0        0     1668 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/client/httpx-request-metrics.j2
--rw-r--r--   0        0        0    11404 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/httpx.j2
--rw-r--r--   0        0        0       33 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/init-py.j2
--rw-r--r--   0        0        0      312 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 06:57:41.508891 pythogen-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2097 2023-07-12 06:57:41.508891 pythogen-0.2.3/README.md
+-rw-r--r--   0        0        0     1567 2023-07-12 06:57:41.512891 pythogen-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1585 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/entrypoint.py
+-rw-r--r--   0        0        0     7492 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/models.py
+-rw-r--r--   0        0        0     2329 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3239 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-12 06:57:41.512891 pythogen-0.2.3/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    16516 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0    10343 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/renderer.py
+-rw-r--r--   0        0        0      172 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/settings.py
+-rw-r--r--   0        0        0     5149 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/client/httpx-method.j2
+-rw-r--r--   0        0        0     1668 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/client/httpx-request-metrics.j2
+-rw-r--r--   0        0        0    11127 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/httpx.j2
+-rw-r--r--   0        0        0       33 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/init-py.j2
+-rw-r--r--   0        0        0      312 2023-07-12 06:57:41.516891 pythogen-0.2.3/pythogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.3/PKG-INFO
```

### Comparing `pythogen-0.2.2/LICENSE` & `pythogen-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/README.md` & `pythogen-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pyproject.toml` & `pythogen-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.2.2"
+version = "0.2.3"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
```

### Comparing `pythogen-0.2.2/pythogen/entrypoint.py` & `pythogen-0.2.3/pythogen/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/models.py` & `pythogen-0.2.3/pythogen/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 class Type(Enum):
     string = 'string'
     number = 'number'
     integer = 'integer'
     boolean = 'boolean'
     array = 'array'
     object = 'object'
+    null = 'null'
 
     # TODO: refactor
     any_of = 'any_of'
 
 
 @dataclass
 class SchemaProperty:
```

### Comparing `pythogen-0.2.2/pythogen/packager.py` & `pythogen-0.2.3/pythogen/packager.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/parsers/document.py` & `pythogen-0.2.3/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.3/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/parsers/operations.py` & `pythogen-0.2.3/pythogen/parsers/operations.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/parsers/parameters.py` & `pythogen-0.2.3/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/parsers/paths.py` & `pythogen-0.2.3/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/parsers/references.py` & `pythogen-0.2.3/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/parsers/request_body.py` & `pythogen-0.2.3/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/parsers/response.py` & `pythogen-0.2.3/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/parsers/schemas.py` & `pythogen-0.2.3/pythogen/parsers/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 
 from pythogen import models
 from pythogen.parsers.inline_schemas_aggregator import InlineSchemasAggregator
 from pythogen.parsers.references import RefResolver
 
 
-PRIMITIVE_TYPES = ('string', 'number', 'integer', 'boolean')
+PRIMITIVE_TYPES = ('string', 'number', 'integer', 'boolean', 'null')
 
 
 class SchemaParser:
     """Парсер схемы
 
     Парсит схему из коллекции схем, расположенных в поле components -> schemas
     OpenAPI-спеки (https://swagger.io/specification/#schema-object)
```

### Comparing `pythogen-0.2.2/pythogen/renderer.py` & `pythogen-0.2.3/pythogen/renderer.py`

 * *Files 5% similar despite different names*

```diff
@@ -219,14 +219,15 @@
 def j2_typerepr(schema: models.SchemaObject, document: models.Document | None = None) -> str:
     """Represent data type on j2 template"""
     primitive_type_mapping = {
         models.Type.integer: 'int',
         models.Type.number: 'float',
         models.Type.boolean: 'bool',
         models.Type.string: 'str',
+        models.Type.null: 'None',
     }
     format_mapping = {
         models.Format.binary: 'bytes',
         models.Format.uri: 'HttpUrl',
         models.Format.date: 'datetime.date',
         models.Format.date_time: 'datetime.datetime',
     }
@@ -271,16 +272,24 @@
 
             items_str = ' | '.join(items)
             representation = f'list[{items_str}]'
         else:
             item = j2_typerepr(schema.items)  # type: ignore
             representation = f'list[{item}]'
 
-    elif schema.type == models.Type.any_of:
-        representation = classname(schema.id)
+    elif schema.type is models.Type.any_of:
+        items = []
+        for item in schema.items:  # type: ignore
+            if item.id:
+                items.append(classname(item.id))
+            else:
+                if item.type is models.Type.null and not item.required:
+                    continue
+                items.append(primitive_type_mapping[item.type])
+        representation = ' | '.join(items)
 
     return representation
 
 
 def varname(value: str) -> str:
     return inflection.underscore(value)
```

### Comparing `pythogen-0.2.2/pythogen/templates/client/httpx-method.j2` & `pythogen-0.2.3/pythogen/templates/client/httpx-method.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/templates/client/httpx-request-metrics.j2` & `pythogen-0.2.3/pythogen/templates/client/httpx-request-metrics.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.2/pythogen/templates/httpx.j2` & `pythogen-0.2.3/pythogen/templates/httpx.j2`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 import httpx
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import field_validator
 from pydantic import FieldValidationInfo
 from pydantic import ConfigDict
 from pydantic import HttpUrl
-from pydantic import RootModel
 import logging
 from functools import wraps
 
 
 # backward compatibility for httpx<0.18.2
 try:
     DEFAULT_AUTH = httpx.USE_CLIENT_DEFAULT
@@ -216,28 +215,14 @@
         return v
 {%- endfor %}
 
 
 {%- for model in models %}
 
 {%- if model.type.value == "any_of"  %}
-class {{ classname(model.id) }}(RootModel):
-    root: list[
-    {% set pipe = joiner(" | ") %}
-    {%- for item in model.items %}
-        {{ pipe() }}{{ item.id }}
-    {%- endfor %}
-    ]
-
-    def __iter__(self):
-        return iter(self.root)
-
-    def __getitem__(self, item):
-        return self.root[item]
-
 {%- else %}
 class {{ classname(model.id) }}(BaseModel):
     """
     {{ model.title }}
     """
     model_config = ConfigDict(
         populate_by_name=True,  # Addressing by field name, even if there is an alias.
@@ -374,10 +359,13 @@
             except:
                 continue
 
         raise Exception("Can't parse \"{item}\"")
 
 
 
-{% for model in models -%}
+{% for model in models %}
+{%- if model.type.value != "any_of" %}
 {{ classname(model.id) }}.model_rebuild()
+{%- else %}
+{%- endif -%}
 {% endfor %}
```

### Comparing `pythogen-0.2.2/PKG-INFO` & `pythogen-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.2.2
+Version: 0.2.3
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.10,<4.0
```

