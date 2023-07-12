# Comparing `tmp/sqlapydantic-0.0.1.tar.gz` & `tmp/sqlapydantic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlapydantic-0.0.1.tar", max compression
+gzip compressed data, was "sqlapydantic-0.0.2.tar", max compression
```

## Comparing `sqlapydantic-0.0.1.tar` & `sqlapydantic-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-06-13 17:55:12.093655 sqlapydantic-0.0.1/LICENSE
--rw-r--r--   0        0        0     1418 2023-06-13 18:47:08.275813 sqlapydantic-0.0.1/README.md
--rw-r--r--   0        0        0      708 2023-06-13 18:55:56.950545 sqlapydantic-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      580 2023-06-13 18:37:45.917531 sqlapydantic-0.0.1/sqlapydantic/__init__.py
--rw-r--r--   0        0        0     9833 2023-06-13 18:33:03.429704 sqlapydantic-0.0.1/sqlapydantic/generator.py
--rw-r--r--   0        0        0      600 2023-06-13 18:32:20.460771 sqlapydantic-0.0.1/sqlapydantic/models.py
--rw-r--r--   0        0        0      732 2023-06-13 18:07:02.753138 sqlapydantic-0.0.1/sqlapydantic/utils.py
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 sqlapydantic-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-13 17:55:12.093655 sqlapydantic-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1418 2023-06-13 18:47:08.275813 sqlapydantic-0.0.2/README.md
+-rw-r--r--   0        0        0      762 2023-07-12 08:32:45.050244 sqlapydantic-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      833 2023-07-12 07:58:51.958331 sqlapydantic-0.0.2/sqlapydantic/__init__.py
+-rw-r--r--   0        0        0    11043 2023-07-12 08:30:35.173591 sqlapydantic-0.0.2/sqlapydantic/generator.py
+-rw-r--r--   0        0        0      722 2023-07-12 08:30:35.176278 sqlapydantic-0.0.2/sqlapydantic/models.py
+-rw-r--r--   0        0        0      732 2023-06-13 18:07:02.753138 sqlapydantic-0.0.2/sqlapydantic/utils.py
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 sqlapydantic-0.0.2/PKG-INFO
```

### Comparing `sqlapydantic-0.0.1/LICENSE` & `sqlapydantic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlapydantic-0.0.1/README.md` & `sqlapydantic-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlapydantic-0.0.1/pyproject.toml` & `sqlapydantic-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlapydantic"
-version = "0.0.1"
+version = "0.0.2"
 description = "Generate pydantic models from SQLAlchemy models"
 authors = ["maacck <c.mai@madainchina.com>"]
 readme = "README.md"
 homepage = "https://github.com/maacck/sqlapydantic"
 repository = "https://github.com/maacck/sqlapydantic"
 keywords = ["pydantic", "sqlalchemy"]
 packages = [{ include = "sqlapydantic" }]
@@ -14,14 +14,17 @@
 "BUG TRACKER" = "https://github.com/maacck/sqlapydantic/issues"
 
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 SQLAlchemy = "^2.0.13"
-pydantic = "^1.10.7"
+pydantic = "2.0.2"
 
 [tool.poetry.dev-dependencies]
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sqlapydantic-0.0.1/sqlapydantic/generator.py` & `sqlapydantic-0.0.2/sqlapydantic/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import inspect
 import sys
 from collections import defaultdict
 from importlib import import_module
 from textwrap import indent
-from typing import TypeVar, Any, ClassVar, Set
+from typing import Any, ClassVar, Set, TypeVar
 
 from pydantic import BaseModel
-from sqlalchemy.orm import DeclarativeBase, DeclarativeMeta
+from sqlalchemy import inspect
+from sqlalchemy.orm import DeclarativeBase, DeclarativeMeta, Relationship
 
-from sqlapydantic.models import ModelClass, ColumnAttribute
+from sqlapydantic.models import ColumnAttribute, ModelClass
 
 CustomBaseModel = TypeVar("CustomBaseModel", bound=BaseModel)
 
 IntPrimaryKey = int
 
 
 class GeneratorOptions(BaseModel):
@@ -28,26 +28,32 @@
 
     def __init__(
         self,
         base_model: CustomBaseModel = BaseModel,
         indentation: str = "    ",
         split_models: bool = False,
         restrict_fields: Set[str] = None,
+        strict_types: bool = False,
+        constraint_str_length: bool = True,
+        constraint_int_length: bool = True,
         **kwargs,
     ):
         self.base_model = base_model
         self.imports: dict[str, set[str]] = defaultdict(set)
         if type(self.base_model) != BaseModel:
             self.add_import(self.base_model)
         self.indentation = indentation
         if restrict_fields:
             self.restrict_fields = restrict_fields
         else:
             self.restrict_fields = {"id", "created_at", "updated_at"}
         self.split_models = split_models
+        self.strict_types = strict_types
+        self.constraint_str_length = constraint_str_length
+        self.constraint_int_length = constraint_int_length
 
     def add_import(self, obj: Any) -> None:
         # Don't store builtin imports
         if getattr(obj, "__module__", "builtins") == "builtins":
             return
 
         type_ = type(obj) if not isinstance(obj, type) else obj
@@ -97,27 +103,35 @@
         ]
 
     def parse_models(self, models_ins: list[DeclarativeBase]) -> list[ModelClass]:
         models: list[ModelClass] = []
         for model_in in models_ins:
             # Get Columns
             model = ModelClass(
-                name=model_in.__name__,
-                columns=[],
+                name=model_in.__name__, columns=[], relationship_classes=[]
             )
             for column in model_in.__table__.c:
                 model.columns.append(
                     ColumnAttribute(
                         optional=column.nullable is not False,
                         key=column.key,
                         python_type=column.type.python_type.__name__,
                         orm_column=column,
                     )
                 )
                 self.add_import(column.type.python_type)
+            # Get Relationships
+            # In Roadmap
+            """
+            model_relationships = inspect(model_in).relationships.items()
+            for rel in model_relationships:
+                rel_prop: Relationship = rel[1]
+                model.relationship_classes.append(rel_prop.mapper.class_)
+            """
+            # Split Models
             if self.split_models:
                 model_base = ModelClass(name=f"{model_in.__name__}Base", columns=[])
                 model_create = ModelClass(
                     name=f"{model_in.__name__}Create",
                     columns=[],
                     parent_class=model_base.name,
                 )
@@ -157,30 +171,44 @@
                         model_read.columns.append(col)
                 models.append(model_base)
                 models.append(model_create)
                 models.append(model_update)
                 models.append(model_read)
             else:
                 models.append(model)
-            # Get Relationships
-            """
-            model_relationships = inspect(model_in).relationships.items()
-            for rel in model_relationships:
-                rel_prop: Relationship = rel[1]
-                print(rel_prop.entity.columns)
-            """
 
         return models
 
     def render_column(self, col: ColumnAttribute, manual_optional: bool = False):
+        field_type = ""
         python_type = col.python_type
+        type_name = python_type.__class__.__name__
+        if isinstance(python_type, str) and self.constraint_str_length:
+            if (
+                hasattr(col.orm_column.type, "length")
+                and col.orm_column.type.length is not None
+            ):
+                self.add_literal_import("pydantic", "constr")
+                field_type = " = constr(max_length={})".format(
+                    col.orm_column.type.length
+                )
+        if self.strict_types and type_name in [
+            "int",
+            "str",
+            "bool",
+            "bytes",
+            "float",
+        ]:
+            strict_type = f"Strict{type_name.capitalize()}"
+            self.add_literal_import("pydantic", strict_type)
+            python_type = strict_type
         if col.optional is True or manual_optional is True:
-            python_type = f"Optional[{col.python_type}]"
+            python_type = f"Optional[{python_type}]"
             self.add_literal_import("typing", "Optional")
-        return f"{col.key}: {python_type}"
+        return f"{col.key}: {python_type}{field_type}"
 
     def render_class_declaration(self, model: ModelClass) -> str:
         model_name = self.base_model.__name__
         if model.parent_class:
             model_name = model.parent_class
         return f"class {model.name}({model_name}):"
```

### Comparing `sqlapydantic-0.0.1/sqlapydantic/utils.py` & `sqlapydantic-0.0.2/sqlapydantic/utils.py`

 * *Files identical despite different names*

### Comparing `sqlapydantic-0.0.1/PKG-INFO` & `sqlapydantic-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sqlapydantic
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate pydantic models from SQLAlchemy models
 Home-page: https://github.com/maacck/sqlapydantic
 Keywords: pydantic,sqlalchemy
 Author: maacck
 Author-email: c.mai@madainchina.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=2.0.13,<3.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (==2.0.2)
 Project-URL: BUG TRACKER, https://github.com/maacck/sqlapydantic/issues
 Project-URL: Repository, https://github.com/maacck/sqlapydantic
 Description-Content-Type: text/markdown
 
 # sqlapydantic
 
 Generate Pydantic Model from SQLAlchemy Model
```

