# Comparing `tmp/sqlapydantic-0.0.2.tar.gz` & `tmp/sqlapydantic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlapydantic-0.0.2.tar", max compression
+gzip compressed data, was "sqlapydantic-0.0.3.tar", max compression
```

## Comparing `sqlapydantic-0.0.2.tar` & `sqlapydantic-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-06-13 17:55:12.093655 sqlapydantic-0.0.2/LICENSE
--rw-r--r--   0        0        0     1418 2023-06-13 18:47:08.275813 sqlapydantic-0.0.2/README.md
--rw-r--r--   0        0        0      762 2023-07-12 08:32:45.050244 sqlapydantic-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      833 2023-07-12 07:58:51.958331 sqlapydantic-0.0.2/sqlapydantic/__init__.py
--rw-r--r--   0        0        0    11043 2023-07-12 08:30:35.173591 sqlapydantic-0.0.2/sqlapydantic/generator.py
--rw-r--r--   0        0        0      722 2023-07-12 08:30:35.176278 sqlapydantic-0.0.2/sqlapydantic/models.py
--rw-r--r--   0        0        0      732 2023-06-13 18:07:02.753138 sqlapydantic-0.0.2/sqlapydantic/utils.py
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 sqlapydantic-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-13 17:55:12.093655 sqlapydantic-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1418 2023-06-13 18:47:08.275813 sqlapydantic-0.0.3/README.md
+-rw-r--r--   0        0        0      762 2023-07-12 10:28:05.922966 sqlapydantic-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      833 2023-07-12 07:58:51.958331 sqlapydantic-0.0.3/sqlapydantic/__init__.py
+-rw-r--r--   0        0        0    11075 2023-07-12 10:27:19.351604 sqlapydantic-0.0.3/sqlapydantic/generator.py
+-rw-r--r--   0        0        0      722 2023-07-12 08:30:35.176278 sqlapydantic-0.0.3/sqlapydantic/models.py
+-rw-r--r--   0        0        0      732 2023-06-13 18:07:02.753138 sqlapydantic-0.0.3/sqlapydantic/utils.py
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 sqlapydantic-0.0.3/PKG-INFO
```

### Comparing `sqlapydantic-0.0.2/LICENSE` & `sqlapydantic-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlapydantic-0.0.2/README.md` & `sqlapydantic-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sqlapydantic-0.0.2/pyproject.toml` & `sqlapydantic-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlapydantic"
-version = "0.0.2"
+version = "0.0.3"
 description = "Generate pydantic models from SQLAlchemy models"
 authors = ["maacck <c.mai@madainchina.com>"]
 readme = "README.md"
 homepage = "https://github.com/maacck/sqlapydantic"
 repository = "https://github.com/maacck/sqlapydantic"
 keywords = ["pydantic", "sqlalchemy"]
 packages = [{ include = "sqlapydantic" }]
```

### Comparing `sqlapydantic-0.0.2/sqlapydantic/__init__.py` & `sqlapydantic-0.0.3/sqlapydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlapydantic-0.0.2/sqlapydantic/generator.py` & `sqlapydantic-0.0.3/sqlapydantic/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import sys
 from collections import defaultdict
 from importlib import import_module
 from textwrap import indent
 from typing import Any, ClassVar, Set, TypeVar
 
 from pydantic import BaseModel
-from sqlalchemy import inspect
+
+# from sqlalchemy import inspect as sa_inspect
+import inspect
 from sqlalchemy.orm import DeclarativeBase, DeclarativeMeta, Relationship
 
 from sqlapydantic.models import ColumnAttribute, ModelClass
 
 CustomBaseModel = TypeVar("CustomBaseModel", bound=BaseModel)
 
 IntPrimaryKey = int
```

### Comparing `sqlapydantic-0.0.2/sqlapydantic/models.py` & `sqlapydantic-0.0.3/sqlapydantic/models.py`

 * *Files identical despite different names*

### Comparing `sqlapydantic-0.0.2/sqlapydantic/utils.py` & `sqlapydantic-0.0.3/sqlapydantic/utils.py`

 * *Files identical despite different names*

### Comparing `sqlapydantic-0.0.2/PKG-INFO` & `sqlapydantic-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlapydantic
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate pydantic models from SQLAlchemy models
 Home-page: https://github.com/maacck/sqlapydantic
 Keywords: pydantic,sqlalchemy
 Author: maacck
 Author-email: c.mai@madainchina.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

