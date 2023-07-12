# Comparing `tmp/redis_om-0.1.2.tar.gz` & `tmp/redis_om-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_om-0.1.2.tar", max compression
+gzip compressed data, was "redis_om-0.1.3.tar", max compression
```

## Comparing `redis_om-0.1.2.tar` & `redis_om-0.1.3.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1071 2023-01-08 11:07:34.764057 redis_om-0.1.2/LICENSE
--rw-r--r--   0        0        0    12552 2023-01-08 11:07:34.764057 redis_om-0.1.2/README.md
--rw-r--r--   0        0        0      420 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/__init__.py
--rw-r--r--   0        0        0       35 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/async_redis.py
--rw-r--r--   0        0        0      751 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/checks.py
--rw-r--r--   0        0        0      524 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/connections.py
--rw-r--r--   0        0        0      180 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/__init__.py
--rw-r--r--   0        0        0        0 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/cli/__init__.py
--rw-r--r--   0        0        0      443 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/cli/migrate.py
--rw-r--r--   0        0        0     6537 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/encoders.py
--rw-r--r--   0        0        0        0 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/migrations/__init__.py
--rw-r--r--   0        0        0     5204 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/migrations/migrator.py
--rw-r--r--   0        0        0    64139 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/model.py
--rw-r--r--   0        0        0     2210 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/query_resolver.py
--rw-r--r--   0        0        0     2140 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/render_tree.py
--rw-r--r--   0        0        0      824 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/model/token_escaper.py
--rw-r--r--   0        0        0       13 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/sync_redis.py
--rw-r--r--   0        0        0      218 2023-01-08 11:07:34.764057 redis_om-0.1.2/aredis_om/util.py
--rw-r--r--   0        0        0     3717 2023-01-08 11:07:34.764057 redis_om-0.1.2/docs/connections.md
--rw-r--r--   0        0        0     6704 2023-01-08 11:07:34.764057 redis_om-0.1.2/docs/errors.md
--rw-r--r--   0        0        0     7510 2023-01-08 11:07:34.764057 redis_om-0.1.2/docs/fastapi_integration.md
--rw-r--r--   0        0        0    21901 2023-01-08 11:07:34.764057 redis_om-0.1.2/docs/getting_started.md
--rw-r--r--   0        0        0      973 2023-01-08 11:07:34.764057 redis_om-0.1.2/docs/index.md
--rw-r--r--   0        0        0    11595 2023-01-08 11:07:34.764057 redis_om-0.1.2/docs/models.md
--rw-r--r--   0        0        0     1674 2023-01-08 11:07:34.764057 redis_om-0.1.2/docs/redis_modules.md
--rw-r--r--   0        0        0     3688 2023-01-08 11:07:34.764057 redis_om-0.1.2/docs/validation.md
--rw-r--r--   0        0        0     3577 2023-01-08 11:07:34.764057 redis_om-0.1.2/images/logo.svg
--rw-r--r--   0        0        0     1828 2023-01-08 11:07:35.192068 redis_om-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      419 2023-01-08 11:08:45.565698 redis_om-0.1.2/redis_om/__init__.py
--rw-r--r--   0        0        0       35 2023-01-08 11:08:45.565698 redis_om-0.1.2/redis_om/async_redis.py
--rw-r--r--   0        0        0      714 2023-01-08 11:08:45.565698 redis_om-0.1.2/redis_om/checks.py
--rw-r--r--   0        0        0      524 2023-01-08 11:08:45.565698 redis_om-0.1.2/redis_om/connections.py
--rw-r--r--   0        0        0      180 2023-01-08 11:08:45.573698 redis_om-0.1.2/redis_om/model/__init__.py
--rw-r--r--   0        0        0        0 2023-01-08 11:08:45.629699 redis_om-0.1.2/redis_om/model/cli/__init__.py
--rw-r--r--   0        0        0      441 2023-01-08 11:08:45.629699 redis_om-0.1.2/redis_om/model/cli/migrate.py
--rw-r--r--   0        0        0     6537 2023-01-08 11:08:45.573698 redis_om-0.1.2/redis_om/model/encoders.py
--rw-r--r--   0        0        0        0 2023-01-08 11:08:45.629699 redis_om-0.1.2/redis_om/model/migrations/__init__.py
--rw-r--r--   0        0        0     5101 2023-01-08 11:08:45.633699 redis_om-0.1.2/redis_om/model/migrations/migrator.py
--rw-r--r--   0        0        0    63814 2023-01-08 11:08:45.629699 redis_om-0.1.2/redis_om/model/model.py
--rw-r--r--   0        0        0     2209 2023-01-08 11:08:45.573698 redis_om-0.1.2/redis_om/model/query_resolver.py
--rw-r--r--   0        0        0     2140 2023-01-08 11:08:45.577698 redis_om-0.1.2/redis_om/model/render_tree.py
--rw-r--r--   0        0        0      824 2023-01-08 11:08:45.573698 redis_om-0.1.2/redis_om/model/token_escaper.py
--rw-r--r--   0        0        0       13 2023-01-08 11:08:45.565698 redis_om-0.1.2/redis_om/sync_redis.py
--rw-r--r--   0        0        0      212 2023-01-08 11:08:45.565698 redis_om-0.1.2/redis_om/util.py
--rw-r--r--   0        0        0    14053 1970-01-01 00:00:00.000000 redis_om-0.1.2/setup.py
--rw-r--r--   0        0        0    14322 1970-01-01 00:00:00.000000 redis_om-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-12 10:27:59.001163 redis_om-0.1.3/LICENSE
+-rw-r--r--   0        0        0    13137 2023-07-12 10:27:59.001163 redis_om-0.1.3/README.md
+-rw-r--r--   0        0        0      463 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/_compat.py
+-rw-r--r--   0        0        0       35 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/async_redis.py
+-rw-r--r--   0        0        0      751 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/checks.py
+-rw-r--r--   0        0        0      524 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/connections.py
+-rw-r--r--   0        0        0      223 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/model/cli/__init__.py
+-rw-r--r--   0        0        0      448 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/cli/migrate.py
+-rw-r--r--   0        0        0     6513 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/encoders.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/migrations/__init__.py
+-rw-r--r--   0        0        0     5204 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/migrations/migrator.py
+-rw-r--r--   0        0        0    69588 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/model.py
+-rw-r--r--   0        0        0     2210 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/query_resolver.py
+-rw-r--r--   0        0        0     2140 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/render_tree.py
+-rw-r--r--   0        0        0      824 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/token_escaper.py
+-rw-r--r--   0        0        0       13 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/sync_redis.py
+-rw-r--r--   0        0        0      218 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/util.py
+-rw-r--r--   0        0        0     3717 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/connections.md
+-rw-r--r--   0        0        0     6704 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/errors.md
+-rw-r--r--   0        0        0     7510 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/fastapi_integration.md
+-rw-r--r--   0        0        0    21897 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/getting_started.md
+-rw-r--r--   0        0        0      973 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/index.md
+-rw-r--r--   0        0        0    11595 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/models.md
+-rw-r--r--   0        0        0     1674 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/redis_modules.md
+-rw-r--r--   0        0        0     3688 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/validation.md
+-rw-r--r--   0        0        0     3577 2023-07-12 10:27:59.005164 redis_om-0.1.3/images/logo.svg
+-rw-r--r--   0        0        0     1822 2023-07-12 10:27:59.489192 redis_om-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      462 2023-07-12 10:28:57.864638 redis_om-0.1.3/redis_om/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/_compat.py
+-rw-r--r--   0        0        0       35 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/async_redis.py
+-rw-r--r--   0        0        0      714 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/checks.py
+-rw-r--r--   0        0        0      524 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/connections.py
+-rw-r--r--   0        0        0      223 2023-07-12 10:28:57.940643 redis_om-0.1.3/redis_om/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:28:57.952644 redis_om-0.1.3/redis_om/model/cli/__init__.py
+-rw-r--r--   0        0        0      446 2023-07-12 10:28:57.952644 redis_om-0.1.3/redis_om/model/cli/migrate.py
+-rw-r--r--   0        0        0     6513 2023-07-12 10:28:57.940643 redis_om-0.1.3/redis_om/model/encoders.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:28:57.948643 redis_om-0.1.3/redis_om/model/migrations/__init__.py
+-rw-r--r--   0        0        0     5101 2023-07-12 10:28:57.948643 redis_om-0.1.3/redis_om/model/migrations/migrator.py
+-rw-r--r--   0        0        0    69263 2023-07-12 10:28:57.932643 redis_om-0.1.3/redis_om/model/model.py
+-rw-r--r--   0        0        0     2209 2023-07-12 10:28:57.864638 redis_om-0.1.3/redis_om/model/query_resolver.py
+-rw-r--r--   0        0        0     2140 2023-07-12 10:28:57.944643 redis_om-0.1.3/redis_om/model/render_tree.py
+-rw-r--r--   0        0        0      824 2023-07-12 10:28:57.864638 redis_om-0.1.3/redis_om/model/token_escaper.py
+-rw-r--r--   0        0        0       13 2023-07-12 10:28:57.856638 redis_om-0.1.3/redis_om/sync_redis.py
+-rw-r--r--   0        0        0      212 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/util.py
+-rw-r--r--   0        0        0    14617 1970-01-01 00:00:00.000000 redis_om-0.1.3/PKG-INFO
```

### Comparing `redis_om-0.1.2/LICENSE` & `redis_om-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/README.md` & `redis_om-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,21 +26,22 @@
   <summary><strong>Table of contents</strong></summary>
 
 span
 
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [💡 Why Redis OM?](#-why-redis-om)
+- [💻 Installation](#-installation)
+- [🏁 Getting started](#-getting-started)
 - [📇 Modeling Your Data](#-modeling-your-data)
 - [✓ Validating Data With Your Model](#-validating-data-with-your-model)
 - [🔎 Rich Queries and Embedded Models](#-rich-queries-and-embedded-models)
   - [Querying](#querying)
   - [Embedded Models](#embedded-models)
 - [Calling Other Redis Commands](#calling-other-redis-commands)
-- [💻 Installation](#-installation)
 - [📚 Documentation](#-documentation)
 - [⛏️ Troubleshooting](#️-troubleshooting)
 - [✨ So How Do You Get RediSearch and RedisJSON?](#-so-how-do-you-get-redisearch-and-redisjson)
 - [❤️ Contributing](#️-contributing)
 - [📝 License](#-license)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
@@ -53,14 +54,39 @@
 
 This **preview** release contains the following features:
 
 * Declarative object mapping for Redis objects
 * Declarative secondary-index generation
 * Fluent APIs for querying Redis
 
+## 💻 Installation
+
+Installation is simple with `pip`, Poetry, or Pipenv.
+
+```sh
+# With pip
+$ pip install redis-om
+
+# Or, using Poetry
+$ poetry add redis-om
+```
+
+## 🏁 Getting started
+
+### Starting Redis
+
+Before writing any code you'll need a Redis instance with the appropriate Redis modules! The quickest way to get this is with Docker:
+
+```sh
+docker run -p 6379:6379 -p 8001:8001 redis/redis-stack
+```
+
+This launches the [redis-stack](https://redis.io/docs/stack/) an extension of Redis that adds all manner of modern data structures to Redis. You'll also notice that if you open up http://localhost:8001 you'll have access to the redis-insight GUI, a GUI you can use to visualize and work with your data in Redis.
+
+
 ## 📇 Modeling Your Data
 
 Redis OM contains powerful declarative models that give you data validation, serialization, and persistence to Redis.
 
 Check out this example of modeling customer data with Redis OM. First, we create a `Customer` model:
 
 ```python
@@ -200,15 +226,15 @@
 
 from redis_om import (
     Field,
     HashModel,
     Migrator
 )
 
-                 
+
 class Customer(HashModel):
     first_name: str
     last_name: str = Field(index=True)
     email: EmailStr
     join_date: datetime.date
     age: int = Field(index=True)
     bio: Optional[str]
@@ -224,15 +250,15 @@
 
 # Find all customers with the last name "Brookins"
 Customer.find(Customer.last_name == "Brookins").all()
 
 # Find all customers that do NOT have the last name "Brookins"
 Customer.find(Customer.last_name != "Brookins").all()
 
-# Find all customers whose last name is "Brookins" OR whose age is 
+# Find all customers whose last name is "Brookins" OR whose age is
 # 100 AND whose last name is "Smith"
 Customer.find((Customer.last_name == "Brookins") | (
         Customer.age == 100
 ) & (Customer.last_name == "Smith")).all()
 ```
 
 These queries -- and more! -- are possible because **Redis OM manages indexes for you automatically**.
@@ -277,15 +303,15 @@
     bio: Optional[str] = Field(index=True, full_text_search=True,
                                default="")
 
     # Creates an embedded model.
     address: Address
 
 
-# With these two models and a Redis deployment with the RedisJSON 
+# With these two models and a Redis deployment with the RedisJSON
 # module installed, we can run queries like the following.
 
 # Before running queries, we need to run migrations to set up the
 # indexes that Redis OM will use. You can also use the `migrate`
 # CLI tool for this!
 Migrator().run()
 
@@ -322,26 +348,14 @@
 ```python
 from redis_om import get_redis_connection
 
 redis_conn = get_redis_connection()
 redis_conn.set("hello", "world")
 ```
 
-## 💻 Installation
-
-Installation is simple with `pip`, Poetry, or Pipenv.
-
-```sh
-# With pip
-$ pip install redis-om
-
-# Or, using Poetry
-$ poetry add redis-om
-```
-
 ## 📚 Documentation
 
 The Redis OM documentation is available [here](docs/index.md).
 
 ## ⛏️ Troubleshooting
 
 If you run into trouble or have any questions, we're here to help!
@@ -368,16 +382,16 @@
 
 Redis OM uses the [MIT license][license-url].
 
 <!-- Badges -->
 
 [version-svg]: https://img.shields.io/pypi/v/redis-om?style=flat-square
 [package-url]: https://pypi.org/project/redis-om/
-[ci-svg]: https://img.shields.io/github/workflow/status/redis/redis-om-python/CI?style=flat-square
-[ci-url]: https://github.com/redis/redis-om-python/actions/workflows/CI.yml
+[ci-svg]: https://img.shields.io/github/workflow/status/redis/redis-om-python/ci?style=flat-square
+[ci-url]: https://github.com/redis/redis-om-python/actions/workflows/ci.yml
 [license-image]: https://img.shields.io/badge/license-mit-green.svg?style=flat-square
 [license-url]: LICENSE
 <!-- Links -->
 
 [redis-om-website]: https://developer.redis.com
 [redis-om-js]: https://github.com/redis-om/redis-om-js
 [redis-om-dotnet]: https://github.com/redis-om/redis-om-dotnet
```

### Comparing `redis_om-0.1.2/aredis_om/checks.py` & `redis_om-0.1.3/aredis_om/checks.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/aredis_om/connections.py` & `redis_om-0.1.3/aredis_om/connections.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/aredis_om/model/encoders.py` & `redis_om-0.1.3/aredis_om/model/encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 import dataclasses
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-from pydantic import BaseModel
-from pydantic.json import ENCODERS_BY_TYPE
+from .._compat import ENCODERS_BY_TYPE, BaseModel
 
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
```

### Comparing `redis_om-0.1.2/aredis_om/model/migrations/migrator.py` & `redis_om-0.1.3/aredis_om/model/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/aredis_om/model/model.py` & `redis_om-0.1.3/aredis_om/model/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,36 +21,43 @@
     Type,
     TypeVar,
     Union,
     no_type_check,
 )
 
 from more_itertools import ichunked
-from pydantic import BaseModel, validator
-from pydantic.fields import FieldInfo as PydanticFieldInfo
-from pydantic.fields import ModelField, Undefined, UndefinedType
-from pydantic.main import ModelMetaclass, validate_model
-from pydantic.typing import NoArgAnyCallable
-from pydantic.utils import Representation
 from redis.commands.json.path import Path
 from redis.exceptions import ResponseError
 from typing_extensions import Protocol, get_args, get_origin
 from ulid import ULID
 
 from .. import redis
+from .._compat import BaseModel
+from .._compat import FieldInfo as PydanticFieldInfo
+from .._compat import (
+    ModelField,
+    ModelMetaclass,
+    NoArgAnyCallable,
+    Representation,
+    Undefined,
+    UndefinedType,
+    validate_model,
+    validator,
+)
 from ..checks import has_redis_json, has_redisearch
 from ..connections import get_redis_connection
 from ..util import ASYNC_MODE
 from .encoders import jsonable_encoder
 from .render_tree import render_tree
 from .token_escaper import TokenEscaper
 
 
 model_registry = {}
 _T = TypeVar("_T")
+Model = TypeVar("Model", bound="RedisModel")
 log = logging.getLogger(__name__)
 escaper = TokenEscaper()
 
 # For basic exact-match field types like an indexed string, we create a TAG
 # field in the RediSearch index. TAG is designed for multi-value fields
 # separated by a "separator" character. We're using the field for single values
 # (multi-value TAGs will be exposed as a separate field type), and we use the
@@ -147,14 +154,22 @@
         return {
             key.decode(encoding): value.decode(encoding) for key, value in obj.items()
         }
     elif isinstance(obj, bytes):
         return obj.decode(encoding)
 
 
+# TODO: replace with `str.removeprefix()` when only Python 3.9+ is supported
+def remove_prefix(value: str, prefix: str) -> str:
+    """Remove a prefix from a string."""
+    if value.startswith(prefix):
+        value = value[len(prefix) :]  # noqa: E203
+    return value
+
+
 class PipelineError(Exception):
     """A Redis pipeline error."""
 
 
 def verify_pipeline_response(
     response: List[Union[bytes, str]], expected_responses: int = 0
 ):
@@ -240,14 +255,32 @@
         return str(self.op)
 
     @property
     def tree(self):
         return render_tree(self)
 
 
+@dataclasses.dataclass
+class KNNExpression:
+    k: int
+    vector_field: ModelField
+    reference_vector: bytes
+
+    def __str__(self):
+        return f"KNN $K @{self.vector_field.name} $knn_ref_vector"
+
+    @property
+    def query_params(self) -> Dict[str, Union[str, bytes]]:
+        return {"K": str(self.k), "knn_ref_vector": self.reference_vector}
+
+    @property
+    def score_field(self) -> str:
+        return f"__{self.vector_field.name}_score"
+
+
 ExpressionOrNegated = Union[Expression, NegatedExpression]
 
 
 class ExpressionProxy:
     def __init__(self, field: ModelField, parents: List[Tuple[str, "RedisModel"]]):
         self.field = field
         self.parents = parents
@@ -337,36 +370,40 @@
 
 
 class FindQuery:
     def __init__(
         self,
         expressions: Sequence[ExpressionOrNegated],
         model: Type["RedisModel"],
+        knn: Optional[KNNExpression] = None,
         offset: int = 0,
-        limit: int = DEFAULT_PAGE_SIZE,
+        limit: Optional[int] = None,
         page_size: int = DEFAULT_PAGE_SIZE,
         sort_fields: Optional[List[str]] = None,
         nocontent: bool = False,
     ):
         if not has_redisearch(model.db()):
             raise RedisModelError(
                 "Your Redis instance does not have either the RediSearch module "
                 "or RedisJSON module installed. Querying requires that your Redis "
                 "instance has one of these modules installed."
             )
 
         self.expressions = expressions
         self.model = model
+        self.knn = knn
         self.offset = offset
-        self.limit = limit
+        self.limit = limit or (self.knn.k if self.knn else DEFAULT_PAGE_SIZE)
         self.page_size = page_size
         self.nocontent = nocontent
 
         if sort_fields:
             self.sort_fields = self.validate_sort_fields(sort_fields)
+        elif self.knn:
+            self.sort_fields = [self.knn.score_field]
         else:
             self.sort_fields = []
 
         self._expression = None
         self._query: Optional[str] = None
         self._pagination: List[str] = []
         self._model_cache: List[RedisModel] = []
@@ -413,19 +450,34 @@
 
         NOTE: We cache the resolved query string after generating it. This should be OK
         because all mutations of FindQuery through public APIs return a new FindQuery instance.
         """
         if self._query:
             return self._query
         self._query = self.resolve_redisearch_query(self.expression)
+        if self.knn:
+            self._query = (
+                self._query
+                if self._query.startswith("(") or self._query == "*"
+                else f"({self._query})"
+            ) + f"=>[{self.knn}]"
         return self._query
 
+    @property
+    def query_params(self):
+        params: List[Union[str, bytes]] = []
+        if self.knn:
+            params += [attr for kv in self.knn.query_params.items() for attr in kv]
+        return params
+
     def validate_sort_fields(self, sort_fields: List[str]):
         for sort_field in sort_fields:
             field_name = sort_field.lstrip("-")
+            if self.knn and field_name == self.knn.score_field:
+                continue
             if field_name not in self.model.__fields__:
                 raise QueryNotSupportedError(
                     f"You tried sort by {field_name}, but that field "
                     f"does not exist on the model {self.model}"
                 )
             field_proxy = getattr(self.model, field_name)
             if not getattr(field_proxy.field.field_info, "sortable", False):
@@ -716,18 +768,35 @@
 
         if encompassing_expression_is_negated:
             result = f"-({result})"
 
         return result
 
     async def execute(self, exhaust_results=True, return_raw_result=False):
-        args = ["ft.search", self.model.Meta.index_name, self.query, *self.pagination]
+        args: List[Union[str, bytes]] = [
+            "FT.SEARCH",
+            self.model.Meta.index_name,
+            self.query,
+            *self.pagination,
+        ]
         if self.sort_fields:
             args += self.resolve_redisearch_sort_fields()
 
+        if self.query_params:
+            args += ["PARAMS", str(len(self.query_params))] + self.query_params
+
+        if self.knn:
+            # Ensure DIALECT is at least 2
+            if "DIALECT" not in args:
+                args += ["DIALECT", "2"]
+            else:
+                i_dialect = args.index("DIALECT") + 1
+                if int(args[i_dialect]) < 2:
+                    args[i_dialect] = "2"
+
         if self.nocontent:
             args.append("NOCONTENT")
 
         # Reset the cache if we're executing from offset 0.
         if self.offset == 0:
             self._model_cache.clear()
 
@@ -905,32 +974,122 @@
 
 class FieldInfo(PydanticFieldInfo):
     def __init__(self, default: Any = Undefined, **kwargs: Any) -> None:
         primary_key = kwargs.pop("primary_key", False)
         sortable = kwargs.pop("sortable", Undefined)
         index = kwargs.pop("index", Undefined)
         full_text_search = kwargs.pop("full_text_search", Undefined)
+        vector_options = kwargs.pop("vector_options", None)
         super().__init__(default=default, **kwargs)
         self.primary_key = primary_key
         self.sortable = sortable
         self.index = index
         self.full_text_search = full_text_search
+        self.vector_options = vector_options
 
 
 class RelationshipInfo(Representation):
     def __init__(
         self,
         *,
         back_populates: Optional[str] = None,
         link_model: Optional[Any] = None,
     ) -> None:
         self.back_populates = back_populates
         self.link_model = link_model
 
 
+@dataclasses.dataclass
+class VectorFieldOptions:
+    class ALGORITHM(Enum):
+        FLAT = "FLAT"
+        HNSW = "HNSW"
+
+    class TYPE(Enum):
+        FLOAT32 = "FLOAT32"
+        FLOAT64 = "FLOAT64"
+
+    class DISTANCE_METRIC(Enum):
+        L2 = "L2"
+        IP = "IP"
+        COSINE = "COSINE"
+
+    algorithm: ALGORITHM
+    type: TYPE
+    dimension: int
+    distance_metric: DISTANCE_METRIC
+
+    # Common optional parameters
+    initial_cap: Optional[int] = None
+
+    # Optional parameters for FLAT
+    block_size: Optional[int] = None
+
+    # Optional parameters for HNSW
+    m: Optional[int] = None
+    ef_construction: Optional[int] = None
+    ef_runtime: Optional[int] = None
+    epsilon: Optional[float] = None
+
+    @staticmethod
+    def flat(
+        type: TYPE,
+        dimension: int,
+        distance_metric: DISTANCE_METRIC,
+        initial_cap: Optional[int] = None,
+        block_size: Optional[int] = None,
+    ):
+        return VectorFieldOptions(
+            algorithm=VectorFieldOptions.ALGORITHM.FLAT,
+            type=type,
+            dimension=dimension,
+            distance_metric=distance_metric,
+            initial_cap=initial_cap,
+            block_size=block_size,
+        )
+
+    @staticmethod
+    def hnsw(
+        type: TYPE,
+        dimension: int,
+        distance_metric: DISTANCE_METRIC,
+        initial_cap: Optional[int] = None,
+        m: Optional[int] = None,
+        ef_construction: Optional[int] = None,
+        ef_runtime: Optional[int] = None,
+        epsilon: Optional[float] = None,
+    ):
+        return VectorFieldOptions(
+            algorithm=VectorFieldOptions.ALGORITHM.HNSW,
+            type=type,
+            dimension=dimension,
+            distance_metric=distance_metric,
+            initial_cap=initial_cap,
+            m=m,
+            ef_construction=ef_construction,
+            ef_runtime=ef_runtime,
+            epsilon=epsilon,
+        )
+
+    @property
+    def schema(self):
+        attr = []
+        for k, v in vars(self).items():
+            if k == "algorithm" or v is None:
+                continue
+            attr.extend(
+                [
+                    k.upper() if k != "dimension" else "DIM",
+                    str(v) if not isinstance(v, Enum) else v.name,
+                ]
+            )
+
+        return " ".join([f"VECTOR {self.algorithm.name} {len(attr)}"] + attr)
+
+
 def Field(
     default: Any = Undefined,
     *,
     default_factory: Optional[NoArgAnyCallable] = None,
     alias: str = None,
     title: str = None,
     description: str = None,
@@ -952,14 +1111,15 @@
     max_length: int = None,
     allow_mutation: bool = True,
     regex: str = None,
     primary_key: bool = False,
     sortable: Union[bool, UndefinedType] = Undefined,
     index: Union[bool, UndefinedType] = Undefined,
     full_text_search: Union[bool, UndefinedType] = Undefined,
+    vector_options: Optional[VectorFieldOptions] = None,
     schema_extra: Optional[Dict[str, Any]] = None,
 ) -> Any:
     current_schema_extra = schema_extra or {}
     field_info = FieldInfo(
         default,
         default_factory=default_factory,
         alias=alias,
@@ -979,14 +1139,15 @@
         max_length=max_length,
         allow_mutation=allow_mutation,
         regex=regex,
         primary_key=primary_key,
         sortable=sortable,
         index=index,
         full_text_search=full_text_search,
+        vector_options=vector_options,
         **current_schema_extra,
     )
     field_info._validate()
     return field_info
 
 
 @dataclasses.dataclass
@@ -1071,14 +1232,18 @@
                 new_class.__annotations__[field_name] = ExpressionProxy
             # Check if this is our FieldInfo version with extended ORM metadata.
             if isinstance(field.field_info, FieldInfo):
                 if field.field_info.primary_key:
                     new_class._meta.primary_key = PrimaryKey(
                         name=field_name, field=field
                     )
+                if field.field_info.vector_options:
+                    score_attr = f"_{field_name}_score"
+                    setattr(new_class, score_attr, None)
+                    new_class.__annotations__[score_attr] = Union[float, None]
 
         if not getattr(new_class._meta, "global_key_prefix", None):
             new_class._meta.global_key_prefix = getattr(
                 base_meta, "global_key_prefix", ""
             )
         if not getattr(new_class._meta, "model_key_prefix", None):
             # Don't look at the base class for this.
@@ -1148,24 +1313,24 @@
     ) -> int:
         """Delete data at this key."""
         db = cls._get_db(pipeline)
 
         return await cls._delete(db, cls.make_primary_key(pk))
 
     @classmethod
-    async def get(cls, pk: Any) -> "RedisModel":
+    async def get(cls: Type["Model"], pk: Any) -> "Model":
         raise NotImplementedError
 
     async def update(self, **field_values):
         """Update this model instance with the specified key-value pairs."""
         raise NotImplementedError
 
     async def save(
-        self, pipeline: Optional[redis.client.Pipeline] = None
-    ) -> "RedisModel":
+        self: "Model", pipeline: Optional[redis.client.Pipeline] = None
+    ) -> "Model":
         raise NotImplementedError
 
     async def expire(
         self, num_seconds: int, pipeline: Optional[redis.client.Pipeline] = None
     ):
         db = self._get_db(pipeline)
 
@@ -1204,16 +1369,20 @@
         return cls.make_key(cls._meta.primary_key_pattern.format(pk=pk))
 
     @classmethod
     def db(cls):
         return cls._meta.database
 
     @classmethod
-    def find(cls, *expressions: Union[Any, Expression]) -> FindQuery:
-        return FindQuery(expressions=expressions, model=cls)
+    def find(
+        cls,
+        *expressions: Union[Any, Expression],
+        knn: Optional[KNNExpression] = None,
+    ) -> FindQuery:
+        return FindQuery(expressions=expressions, knn=knn, model=cls)
 
     @classmethod
     def from_redis(cls, res: Any):
         # TODO: Parsing logic copied from redisearch-py. Evaluate.
         def to_string(s):
             if isinstance(s, (str,)):
                 return s
@@ -1225,24 +1394,27 @@
         docs = []
         step = 2  # Because the result has content
         offset = 1  # The first item is the count of total matches.
 
         for i in range(1, len(res), step):
             if res[i + offset] is None:
                 continue
-            fields = dict(
+            fields: Dict[str, str] = dict(
                 zip(
                     map(to_string, res[i + offset][::2]),
                     map(to_string, res[i + offset][1::2]),
                 )
             )
             # $ means a json entry
             if fields.get("$"):
                 json_fields = json.loads(fields.pop("$"))
                 doc = cls(**json_fields)
+                for k, v in fields.items():
+                    if k.startswith("__") and k.endswith("_score"):
+                        setattr(doc, k[1:], float(v))
             else:
                 doc = cls(**fields)
 
             docs.append(doc)
         return docs
 
     @classmethod
@@ -1254,19 +1426,19 @@
             except AttributeError:
                 # object, at least, has no __annotations__ attribute.
                 pass
         return d
 
     @classmethod
     async def add(
-        cls,
-        models: Sequence["RedisModel"],
+        cls: Type["Model"],
+        models: Sequence["Model"],
         pipeline: Optional[redis.client.Pipeline] = None,
         pipeline_verifier: Callable[..., Any] = verify_pipeline_response,
-    ) -> Sequence["RedisModel"]:
+    ) -> Sequence["Model"]:
         db = cls._get_db(pipeline, bulk=True)
 
         for model in models:
             # save() just returns the model, we don't need that here.
             await model.save(pipeline=db)
 
         # If the user didn't give us a pipeline, then we need to execute
@@ -1333,42 +1505,38 @@
                 )
             elif dataclasses.is_dataclass(field.outer_type_):
                 raise RedisModelError(
                     f"HashModels cannot index dataclass fields. Field: {name}"
                 )
 
     async def save(
-        self, pipeline: Optional[redis.client.Pipeline] = None
-    ) -> "HashModel":
+        self: "Model", pipeline: Optional[redis.client.Pipeline] = None
+    ) -> "Model":
         self.check()
         db = self._get_db(pipeline)
 
         document = jsonable_encoder(self.dict())
         # TODO: Wrap any Redis response errors in a custom exception?
         await db.hset(self.key(), mapping=document)
         return self
 
     @classmethod
     async def all_pks(cls):  # type: ignore
         key_prefix = cls.make_key(cls._meta.primary_key_pattern.format(pk=""))
-        # TODO: We assume the key ends with the default separator, ":" -- when
-        #  we make the separator configurable, we need to update this as well.
-        #  ... And probably lots of other places ...
-        #
-        # TODO: Also, we need to decide how we want to handle the lack of
+        # TODO: We need to decide how we want to handle the lack of
         #  decode_responses=True...
         return (
-            key.split(":")[-1]
+            remove_prefix(key, key_prefix)
             if isinstance(key, str)
-            else key.decode(cls.Meta.encoding).split(":")[-1]
+            else remove_prefix(key.decode(cls.Meta.encoding), key_prefix)
             async for key in cls.db().scan_iter(f"{key_prefix}*", _type="HASH")
         )
 
     @classmethod
-    async def get(cls, pk: Any) -> "HashModel":
+    async def get(cls: Type["Model"], pk: Any) -> "Model":
         document = await cls.db().hgetall(cls.make_primary_key(pk))
         if not document:
             raise NotFoundError
         try:
             result = cls.parse_obj(document)
         except TypeError as e:
             log.warning(
@@ -1466,15 +1634,21 @@
                 log.warning(
                     "Model %s defined an empty list or tuple field: %s", cls, name
                 )
                 return ""
             embedded_cls = embedded_cls[0]
             schema = cls.schema_for_type(name, embedded_cls, field_info)
         elif any(issubclass(typ, t) for t in NUMERIC_TYPES):
-            schema = f"{name} NUMERIC"
+            vector_options: Optional[VectorFieldOptions] = getattr(
+                field_info, "vector_options", None
+            )
+            if vector_options:
+                schema = f"{name} {vector_options.schema}"
+            else:
+                schema = f"{name} NUMERIC"
         elif issubclass(typ, str):
             if getattr(field_info, "full_text_search", False) is True:
                 schema = (
                     f"{name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR} "
                     f"{name} AS {name}_fts TEXT"
                 )
             else:
@@ -1505,36 +1679,32 @@
             log.error(
                 "Your Redis instance does not have the RedisJson module "
                 "loaded. JsonModel depends on RedisJson."
             )
         super().__init__(*args, **kwargs)
 
     async def save(
-        self, pipeline: Optional[redis.client.Pipeline] = None
-    ) -> "JsonModel":
+        self: "Model", pipeline: Optional[redis.client.Pipeline] = None
+    ) -> "Model":
         self.check()
         db = self._get_db(pipeline)
 
         # TODO: Wrap response errors in a custom exception?
         await db.json().set(self.key(), Path.root_path(), json.loads(self.json()))
         return self
 
     @classmethod
     async def all_pks(cls):  # type: ignore
         key_prefix = cls.make_key(cls._meta.primary_key_pattern.format(pk=""))
-        # TODO: We assume the key ends with the default separator, ":" -- when
-        #  we make the separator configurable, we need to update this as well.
-        #  ... And probably lots of other places ...
-        #
-        # TODO: Also, we need to decide how we want to handle the lack of
+        # TODO: We need to decide how we want to handle the lack of
         #  decode_responses=True...
         return (
-            key.split(":")[-1]
+            remove_prefix(key, key_prefix)
             if isinstance(key, str)
-            else key.decode(cls.Meta.encoding).split(":")[-1]
+            else remove_prefix(key.decode(cls.Meta.encoding), key_prefix)
             async for key in cls.db().scan_iter(f"{key_prefix}*", _type="ReJSON-RL")
         )
 
     async def update(self, **field_values):
         validate_model_fields(self.__class__, field_values)
         for field, value in field_values.items():
             # Handle the simple update case first, e.g. city="Happy Valley"
@@ -1555,15 +1725,15 @@
 
             # Set the target field (the last "part" of the nested update
             # field name) to the target value.
             setattr(obj, target_field, value)
         await self.save()
 
     @classmethod
-    async def get(cls, pk: Any) -> "JsonModel":
+    async def get(cls: Type["Model"], pk: Any) -> "Model":
         document = json.dumps(await cls.db().json().get(cls.make_key(pk)))
         if document == "null":
             raise NotFoundError
         return cls.parse_raw(document)
 
     @classmethod
     def redisearch_schema(cls):
@@ -1619,18 +1789,30 @@
 
         try:
             field_is_model = issubclass(typ, RedisModel)
         except TypeError:
             # Not a class, probably a type annotation
             field_is_model = False
 
+        vector_options: Optional[VectorFieldOptions] = getattr(
+            field_info, "vector_options", None
+        )
+        try:
+            is_vector = vector_options and any(
+                issubclass(get_args(typ)[0], t) for t in NUMERIC_TYPES
+            )
+        except IndexError:
+            raise RedisModelError(
+                f"Vector field '{name}' must be annotated as a container type"
+            )
+
         # When we encounter a list or model field, we need to descend
         # into the values of the list or the fields of the model to
         # find any values marked as indexed.
-        if is_container_type:
+        if is_container_type and not is_vector:
             field_type = get_origin(typ)
             embedded_cls = get_args(typ)
             if not embedded_cls:
                 log.warning(
                     "Model %s defined an empty list or tuple field: %s", cls, name
                 )
                 return ""
@@ -1685,15 +1867,17 @@
             sortable_tag_error = RedisModelError(
                 "In this Preview release, TAG fields cannot "
                 f"be marked as sortable. Problem field: {name}. "
                 "See docs: TODO"
             )
 
             # TODO: GEO field
-            if parent_is_container_type or parent_is_model_in_container:
+            if is_vector and vector_options:
+                schema = f"{path} AS {index_field_name} {vector_options.schema}"
+            elif parent_is_container_type or parent_is_model_in_container:
                 if typ is not str:
                     raise RedisModelError(
                         "In this Preview release, list and tuple fields can only "
                         f"contain strings. Problem field: {name}. See docs: TODO"
                     )
                 if full_text_search is True:
                     raise RedisModelError(
```

### Comparing `redis_om-0.1.2/aredis_om/model/query_resolver.py` & `redis_om-0.1.3/aredis_om/model/query_resolver.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/aredis_om/model/render_tree.py` & `redis_om-0.1.3/aredis_om/model/render_tree.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/aredis_om/model/token_escaper.py` & `redis_om-0.1.3/aredis_om/model/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/docs/connections.md` & `redis_om-0.1.3/docs/connections.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/docs/errors.md` & `redis_om-0.1.3/docs/errors.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/docs/fastapi_integration.md` & `redis_om-0.1.3/docs/fastapi_integration.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/docs/getting_started.md` & `redis_om-0.1.3/docs/getting_started.md`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     $ docker run -d -p 6379:6379 redis
 
 ## Installing Redis OM
 
 The recommended way to install Redis OM is with [Poetry](https://python-poetry.org/docs/). You can install Redis OM using Poetry with the following command:
 
-    $ poetry install redis-om
+    $ poetry add redis-om
 
 If you're using Pipenv, the command is:
 
     $ pipenv install redis-om
 
 Finally, you can install Redis OM with `pip` by running the following command:
```

### Comparing `redis_om-0.1.2/docs/index.md` & `redis_om-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/docs/models.md` & `redis_om-0.1.3/docs/models.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/docs/redis_modules.md` & `redis_om-0.1.3/docs/redis_modules.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/docs/validation.md` & `redis_om-0.1.3/docs/validation.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/images/logo.svg` & `redis_om-0.1.3/images/logo.svg`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/pyproject.toml` & `redis_om-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-om"
-version = "0.1.2"
+version = "0.1.3"
 description = "Object mappings, and more, for Redis."
 authors = [ "Redis OSS <oss@redis.com>" ]
 maintainers = [ "Redis OSS <oss@redis.com>" ]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/redis/redis-om-python"
 classifiers = [
@@ -29,37 +29,36 @@
   [tool.poetry.urls]
   Code = "https://github.com/redis/redis-om-python"
   "Issue tracker" = "https://github.com/redis/redis-om-python/issues"
 
   [tool.poetry.dependencies]
   python = ">=3.7,<4.0"
   redis = ">=3.5.3,<5.0.0"
-  pydantic = "^1.10.2"
+  pydantic = ">=1.10.2,<2.1.0"
   click = "^8.0.1"
-  pptree = "^3.1"
   types-redis = ">=3.5.9,<5.0.0"
   python-ulid = "^1.0.3"
   typing-extensions = "^4.4.0"
-  hiredis = "^2.0.0"
-  more-itertools = "^8.14.0"
+  hiredis = "^2.2.3"
+  more-itertools = ">=8.14,<10.0"
 
   [tool.poetry.dev-dependencies]
   mypy = "^0.982"
   pytest = "^7.1.3"
   ipdb = "^0.13.9"
-  black = "^22.10"
+  black = "^23.1"
   isort = "^5.9.3"
   flake8 = "^5.0.4"
   bandit = "^1.7.4"
-  coverage = "^6.4"
+  coverage = "^7.1"
   pytest-cov = "^4.0.0"
-  pytest-xdist = "^2.5.0"
+  pytest-xdist = "^3.1.0"
   unasync = "^0.5.0"
-  pytest-asyncio = "^0.19.0"
-  email-validator = "^1.3.0"
+  pytest-asyncio = "^0.20.3"
+  email-validator = "^2.0.0"
   tox = "^3.26.0"
   tox-pyenv = "^1.1.0"
 
   [tool.poetry.scripts]
   migrate = "redis_om.model.cli.migrate:migrate"
 
 [build-system]
```

### Comparing `redis_om-0.1.2/redis_om/checks.py` & `redis_om-0.1.3/redis_om/checks.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/redis_om/connections.py` & `redis_om-0.1.3/redis_om/connections.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/redis_om/model/encoders.py` & `redis_om-0.1.3/redis_om/model/encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 import dataclasses
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-from pydantic import BaseModel
-from pydantic.json import ENCODERS_BY_TYPE
+from .._compat import ENCODERS_BY_TYPE, BaseModel
 
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
```

### Comparing `redis_om-0.1.2/redis_om/model/migrations/migrator.py` & `redis_om-0.1.3/redis_om/model/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/redis_om/model/model.py` & `redis_om-0.1.3/redis_om/model/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,36 +21,43 @@
     Type,
     TypeVar,
     Union,
     no_type_check,
 )
 
 from more_itertools import ichunked
-from pydantic import BaseModel, validator
-from pydantic.fields import FieldInfo as PydanticFieldInfo
-from pydantic.fields import ModelField, Undefined, UndefinedType
-from pydantic.main import ModelMetaclass, validate_model
-from pydantic.typing import NoArgAnyCallable
-from pydantic.utils import Representation
 from redis.commands.json.path import Path
 from redis.exceptions import ResponseError
 from typing_extensions import Protocol, get_args, get_origin
 from ulid import ULID
 
 from .. import redis
+from .._compat import BaseModel
+from .._compat import FieldInfo as PydanticFieldInfo
+from .._compat import (
+    ModelField,
+    ModelMetaclass,
+    NoArgAnyCallable,
+    Representation,
+    Undefined,
+    UndefinedType,
+    validate_model,
+    validator,
+)
 from ..checks import has_redis_json, has_redisearch
 from ..connections import get_redis_connection
 from ..util import ASYNC_MODE
 from .encoders import jsonable_encoder
 from .render_tree import render_tree
 from .token_escaper import TokenEscaper
 
 
 model_registry = {}
 _T = TypeVar("_T")
+Model = TypeVar("Model", bound="RedisModel")
 log = logging.getLogger(__name__)
 escaper = TokenEscaper()
 
 # For basic exact-match field types like an indexed string, we create a TAG
 # field in the RediSearch index. TAG is designed for multi-value fields
 # separated by a "separator" character. We're using the field for single values
 # (multi-value TAGs will be exposed as a separate field type), and we use the
@@ -147,14 +154,22 @@
         return {
             key.decode(encoding): value.decode(encoding) for key, value in obj.items()
         }
     elif isinstance(obj, bytes):
         return obj.decode(encoding)
 
 
+# TODO: replace with `str.removeprefix()` when only Python 3.9+ is supported
+def remove_prefix(value: str, prefix: str) -> str:
+    """Remove a prefix from a string."""
+    if value.startswith(prefix):
+        value = value[len(prefix) :]  # noqa: E203
+    return value
+
+
 class PipelineError(Exception):
     """A Redis pipeline error."""
 
 
 def verify_pipeline_response(
     response: List[Union[bytes, str]], expected_responses: int = 0
 ):
@@ -240,14 +255,32 @@
         return str(self.op)
 
     @property
     def tree(self):
         return render_tree(self)
 
 
+@dataclasses.dataclass
+class KNNExpression:
+    k: int
+    vector_field: ModelField
+    reference_vector: bytes
+
+    def __str__(self):
+        return f"KNN $K @{self.vector_field.name} $knn_ref_vector"
+
+    @property
+    def query_params(self) -> Dict[str, Union[str, bytes]]:
+        return {"K": str(self.k), "knn_ref_vector": self.reference_vector}
+
+    @property
+    def score_field(self) -> str:
+        return f"__{self.vector_field.name}_score"
+
+
 ExpressionOrNegated = Union[Expression, NegatedExpression]
 
 
 class ExpressionProxy:
     def __init__(self, field: ModelField, parents: List[Tuple[str, "RedisModel"]]):
         self.field = field
         self.parents = parents
@@ -337,36 +370,40 @@
 
 
 class FindQuery:
     def __init__(
         self,
         expressions: Sequence[ExpressionOrNegated],
         model: Type["RedisModel"],
+        knn: Optional[KNNExpression] = None,
         offset: int = 0,
-        limit: int = DEFAULT_PAGE_SIZE,
+        limit: Optional[int] = None,
         page_size: int = DEFAULT_PAGE_SIZE,
         sort_fields: Optional[List[str]] = None,
         nocontent: bool = False,
     ):
         if not has_redisearch(model.db()):
             raise RedisModelError(
                 "Your Redis instance does not have either the RediSearch module "
                 "or RedisJSON module installed. Querying requires that your Redis "
                 "instance has one of these modules installed."
             )
 
         self.expressions = expressions
         self.model = model
+        self.knn = knn
         self.offset = offset
-        self.limit = limit
+        self.limit = limit or (self.knn.k if self.knn else DEFAULT_PAGE_SIZE)
         self.page_size = page_size
         self.nocontent = nocontent
 
         if sort_fields:
             self.sort_fields = self.validate_sort_fields(sort_fields)
+        elif self.knn:
+            self.sort_fields = [self.knn.score_field]
         else:
             self.sort_fields = []
 
         self._expression = None
         self._query: Optional[str] = None
         self._pagination: List[str] = []
         self._model_cache: List[RedisModel] = []
@@ -413,19 +450,34 @@
 
         NOTE: We cache the resolved query string after generating it. This should be OK
         because all mutations of FindQuery through public APIs return a new FindQuery instance.
         """
         if self._query:
             return self._query
         self._query = self.resolve_redisearch_query(self.expression)
+        if self.knn:
+            self._query = (
+                self._query
+                if self._query.startswith("(") or self._query == "*"
+                else f"({self._query})"
+            ) + f"=>[{self.knn}]"
         return self._query
 
+    @property
+    def query_params(self):
+        params: List[Union[str, bytes]] = []
+        if self.knn:
+            params += [attr for kv in self.knn.query_params.items() for attr in kv]
+        return params
+
     def validate_sort_fields(self, sort_fields: List[str]):
         for sort_field in sort_fields:
             field_name = sort_field.lstrip("-")
+            if self.knn and field_name == self.knn.score_field:
+                continue
             if field_name not in self.model.__fields__:
                 raise QueryNotSupportedError(
                     f"You tried sort by {field_name}, but that field "
                     f"does not exist on the model {self.model}"
                 )
             field_proxy = getattr(self.model, field_name)
             if not getattr(field_proxy.field.field_info, "sortable", False):
@@ -716,18 +768,35 @@
 
         if encompassing_expression_is_negated:
             result = f"-({result})"
 
         return result
 
     def execute(self, exhaust_results=True, return_raw_result=False):
-        args = ["ft.search", self.model.Meta.index_name, self.query, *self.pagination]
+        args: List[Union[str, bytes]] = [
+            "FT.SEARCH",
+            self.model.Meta.index_name,
+            self.query,
+            *self.pagination,
+        ]
         if self.sort_fields:
             args += self.resolve_redisearch_sort_fields()
 
+        if self.query_params:
+            args += ["PARAMS", str(len(self.query_params))] + self.query_params
+
+        if self.knn:
+            # Ensure DIALECT is at least 2
+            if "DIALECT" not in args:
+                args += ["DIALECT", "2"]
+            else:
+                i_dialect = args.index("DIALECT") + 1
+                if int(args[i_dialect]) < 2:
+                    args[i_dialect] = "2"
+
         if self.nocontent:
             args.append("NOCONTENT")
 
         # Reset the cache if we're executing from offset 0.
         if self.offset == 0:
             self._model_cache.clear()
 
@@ -905,32 +974,122 @@
 
 class FieldInfo(PydanticFieldInfo):
     def __init__(self, default: Any = Undefined, **kwargs: Any) -> None:
         primary_key = kwargs.pop("primary_key", False)
         sortable = kwargs.pop("sortable", Undefined)
         index = kwargs.pop("index", Undefined)
         full_text_search = kwargs.pop("full_text_search", Undefined)
+        vector_options = kwargs.pop("vector_options", None)
         super().__init__(default=default, **kwargs)
         self.primary_key = primary_key
         self.sortable = sortable
         self.index = index
         self.full_text_search = full_text_search
+        self.vector_options = vector_options
 
 
 class RelationshipInfo(Representation):
     def __init__(
         self,
         *,
         back_populates: Optional[str] = None,
         link_model: Optional[Any] = None,
     ) -> None:
         self.back_populates = back_populates
         self.link_model = link_model
 
 
+@dataclasses.dataclass
+class VectorFieldOptions:
+    class ALGORITHM(Enum):
+        FLAT = "FLAT"
+        HNSW = "HNSW"
+
+    class TYPE(Enum):
+        FLOAT32 = "FLOAT32"
+        FLOAT64 = "FLOAT64"
+
+    class DISTANCE_METRIC(Enum):
+        L2 = "L2"
+        IP = "IP"
+        COSINE = "COSINE"
+
+    algorithm: ALGORITHM
+    type: TYPE
+    dimension: int
+    distance_metric: DISTANCE_METRIC
+
+    # Common optional parameters
+    initial_cap: Optional[int] = None
+
+    # Optional parameters for FLAT
+    block_size: Optional[int] = None
+
+    # Optional parameters for HNSW
+    m: Optional[int] = None
+    ef_construction: Optional[int] = None
+    ef_runtime: Optional[int] = None
+    epsilon: Optional[float] = None
+
+    @staticmethod
+    def flat(
+        type: TYPE,
+        dimension: int,
+        distance_metric: DISTANCE_METRIC,
+        initial_cap: Optional[int] = None,
+        block_size: Optional[int] = None,
+    ):
+        return VectorFieldOptions(
+            algorithm=VectorFieldOptions.ALGORITHM.FLAT,
+            type=type,
+            dimension=dimension,
+            distance_metric=distance_metric,
+            initial_cap=initial_cap,
+            block_size=block_size,
+        )
+
+    @staticmethod
+    def hnsw(
+        type: TYPE,
+        dimension: int,
+        distance_metric: DISTANCE_METRIC,
+        initial_cap: Optional[int] = None,
+        m: Optional[int] = None,
+        ef_construction: Optional[int] = None,
+        ef_runtime: Optional[int] = None,
+        epsilon: Optional[float] = None,
+    ):
+        return VectorFieldOptions(
+            algorithm=VectorFieldOptions.ALGORITHM.HNSW,
+            type=type,
+            dimension=dimension,
+            distance_metric=distance_metric,
+            initial_cap=initial_cap,
+            m=m,
+            ef_construction=ef_construction,
+            ef_runtime=ef_runtime,
+            epsilon=epsilon,
+        )
+
+    @property
+    def schema(self):
+        attr = []
+        for k, v in vars(self).items():
+            if k == "algorithm" or v is None:
+                continue
+            attr.extend(
+                [
+                    k.upper() if k != "dimension" else "DIM",
+                    str(v) if not isinstance(v, Enum) else v.name,
+                ]
+            )
+
+        return " ".join([f"VECTOR {self.algorithm.name} {len(attr)}"] + attr)
+
+
 def Field(
     default: Any = Undefined,
     *,
     default_factory: Optional[NoArgAnyCallable] = None,
     alias: str = None,
     title: str = None,
     description: str = None,
@@ -952,14 +1111,15 @@
     max_length: int = None,
     allow_mutation: bool = True,
     regex: str = None,
     primary_key: bool = False,
     sortable: Union[bool, UndefinedType] = Undefined,
     index: Union[bool, UndefinedType] = Undefined,
     full_text_search: Union[bool, UndefinedType] = Undefined,
+    vector_options: Optional[VectorFieldOptions] = None,
     schema_extra: Optional[Dict[str, Any]] = None,
 ) -> Any:
     current_schema_extra = schema_extra or {}
     field_info = FieldInfo(
         default,
         default_factory=default_factory,
         alias=alias,
@@ -979,14 +1139,15 @@
         max_length=max_length,
         allow_mutation=allow_mutation,
         regex=regex,
         primary_key=primary_key,
         sortable=sortable,
         index=index,
         full_text_search=full_text_search,
+        vector_options=vector_options,
         **current_schema_extra,
     )
     field_info._validate()
     return field_info
 
 
 @dataclasses.dataclass
@@ -1071,14 +1232,18 @@
                 new_class.__annotations__[field_name] = ExpressionProxy
             # Check if this is our FieldInfo version with extended ORM metadata.
             if isinstance(field.field_info, FieldInfo):
                 if field.field_info.primary_key:
                     new_class._meta.primary_key = PrimaryKey(
                         name=field_name, field=field
                     )
+                if field.field_info.vector_options:
+                    score_attr = f"_{field_name}_score"
+                    setattr(new_class, score_attr, None)
+                    new_class.__annotations__[score_attr] = Union[float, None]
 
         if not getattr(new_class._meta, "global_key_prefix", None):
             new_class._meta.global_key_prefix = getattr(
                 base_meta, "global_key_prefix", ""
             )
         if not getattr(new_class._meta, "model_key_prefix", None):
             # Don't look at the base class for this.
@@ -1148,24 +1313,24 @@
     ) -> int:
         """Delete data at this key."""
         db = cls._get_db(pipeline)
 
         return cls._delete(db, cls.make_primary_key(pk))
 
     @classmethod
-    def get(cls, pk: Any) -> "RedisModel":
+    def get(cls: Type["Model"], pk: Any) -> "Model":
         raise NotImplementedError
 
     def update(self, **field_values):
         """Update this model instance with the specified key-value pairs."""
         raise NotImplementedError
 
     def save(
-        self, pipeline: Optional[redis.client.Pipeline] = None
-    ) -> "RedisModel":
+        self: "Model", pipeline: Optional[redis.client.Pipeline] = None
+    ) -> "Model":
         raise NotImplementedError
 
     def expire(
         self, num_seconds: int, pipeline: Optional[redis.client.Pipeline] = None
     ):
         db = self._get_db(pipeline)
 
@@ -1204,16 +1369,20 @@
         return cls.make_key(cls._meta.primary_key_pattern.format(pk=pk))
 
     @classmethod
     def db(cls):
         return cls._meta.database
 
     @classmethod
-    def find(cls, *expressions: Union[Any, Expression]) -> FindQuery:
-        return FindQuery(expressions=expressions, model=cls)
+    def find(
+        cls,
+        *expressions: Union[Any, Expression],
+        knn: Optional[KNNExpression] = None,
+    ) -> FindQuery:
+        return FindQuery(expressions=expressions, knn=knn, model=cls)
 
     @classmethod
     def from_redis(cls, res: Any):
         # TODO: Parsing logic copied from redisearch-py. Evaluate.
         def to_string(s):
             if isinstance(s, (str,)):
                 return s
@@ -1225,24 +1394,27 @@
         docs = []
         step = 2  # Because the result has content
         offset = 1  # The first item is the count of total matches.
 
         for i in range(1, len(res), step):
             if res[i + offset] is None:
                 continue
-            fields = dict(
+            fields: Dict[str, str] = dict(
                 zip(
                     map(to_string, res[i + offset][::2]),
                     map(to_string, res[i + offset][1::2]),
                 )
             )
             # $ means a json entry
             if fields.get("$"):
                 json_fields = json.loads(fields.pop("$"))
                 doc = cls(**json_fields)
+                for k, v in fields.items():
+                    if k.startswith("__") and k.endswith("_score"):
+                        setattr(doc, k[1:], float(v))
             else:
                 doc = cls(**fields)
 
             docs.append(doc)
         return docs
 
     @classmethod
@@ -1254,19 +1426,19 @@
             except AttributeError:
                 # object, at least, has no __annotations__ attribute.
                 pass
         return d
 
     @classmethod
     def add(
-        cls,
-        models: Sequence["RedisModel"],
+        cls: Type["Model"],
+        models: Sequence["Model"],
         pipeline: Optional[redis.client.Pipeline] = None,
         pipeline_verifier: Callable[..., Any] = verify_pipeline_response,
-    ) -> Sequence["RedisModel"]:
+    ) -> Sequence["Model"]:
         db = cls._get_db(pipeline, bulk=True)
 
         for model in models:
             # save() just returns the model, we don't need that here.
             model.save(pipeline=db)
 
         # If the user didn't give us a pipeline, then we need to execute
@@ -1333,42 +1505,38 @@
                 )
             elif dataclasses.is_dataclass(field.outer_type_):
                 raise RedisModelError(
                     f"HashModels cannot index dataclass fields. Field: {name}"
                 )
 
     def save(
-        self, pipeline: Optional[redis.client.Pipeline] = None
-    ) -> "HashModel":
+        self: "Model", pipeline: Optional[redis.client.Pipeline] = None
+    ) -> "Model":
         self.check()
         db = self._get_db(pipeline)
 
         document = jsonable_encoder(self.dict())
         # TODO: Wrap any Redis response errors in a custom exception?
         db.hset(self.key(), mapping=document)
         return self
 
     @classmethod
     def all_pks(cls):  # type: ignore
         key_prefix = cls.make_key(cls._meta.primary_key_pattern.format(pk=""))
-        # TODO: We assume the key ends with the default separator, ":" -- when
-        #  we make the separator configurable, we need to update this as well.
-        #  ... And probably lots of other places ...
-        #
-        # TODO: Also, we need to decide how we want to handle the lack of
+        # TODO: We need to decide how we want to handle the lack of
         #  decode_responses=True...
         return (
-            key.split(":")[-1]
+            remove_prefix(key, key_prefix)
             if isinstance(key, str)
-            else key.decode(cls.Meta.encoding).split(":")[-1]
+            else remove_prefix(key.decode(cls.Meta.encoding), key_prefix)
             for key in cls.db().scan_iter(f"{key_prefix}*", _type="HASH")
         )
 
     @classmethod
-    def get(cls, pk: Any) -> "HashModel":
+    def get(cls: Type["Model"], pk: Any) -> "Model":
         document = cls.db().hgetall(cls.make_primary_key(pk))
         if not document:
             raise NotFoundError
         try:
             result = cls.parse_obj(document)
         except TypeError as e:
             log.warning(
@@ -1466,15 +1634,21 @@
                 log.warning(
                     "Model %s defined an empty list or tuple field: %s", cls, name
                 )
                 return ""
             embedded_cls = embedded_cls[0]
             schema = cls.schema_for_type(name, embedded_cls, field_info)
         elif any(issubclass(typ, t) for t in NUMERIC_TYPES):
-            schema = f"{name} NUMERIC"
+            vector_options: Optional[VectorFieldOptions] = getattr(
+                field_info, "vector_options", None
+            )
+            if vector_options:
+                schema = f"{name} {vector_options.schema}"
+            else:
+                schema = f"{name} NUMERIC"
         elif issubclass(typ, str):
             if getattr(field_info, "full_text_search", False) is True:
                 schema = (
                     f"{name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR} "
                     f"{name} AS {name}_fts TEXT"
                 )
             else:
@@ -1505,36 +1679,32 @@
             log.error(
                 "Your Redis instance does not have the RedisJson module "
                 "loaded. JsonModel depends on RedisJson."
             )
         super().__init__(*args, **kwargs)
 
     def save(
-        self, pipeline: Optional[redis.client.Pipeline] = None
-    ) -> "JsonModel":
+        self: "Model", pipeline: Optional[redis.client.Pipeline] = None
+    ) -> "Model":
         self.check()
         db = self._get_db(pipeline)
 
         # TODO: Wrap response errors in a custom exception?
         db.json().set(self.key(), Path.root_path(), json.loads(self.json()))
         return self
 
     @classmethod
     def all_pks(cls):  # type: ignore
         key_prefix = cls.make_key(cls._meta.primary_key_pattern.format(pk=""))
-        # TODO: We assume the key ends with the default separator, ":" -- when
-        #  we make the separator configurable, we need to update this as well.
-        #  ... And probably lots of other places ...
-        #
-        # TODO: Also, we need to decide how we want to handle the lack of
+        # TODO: We need to decide how we want to handle the lack of
         #  decode_responses=True...
         return (
-            key.split(":")[-1]
+            remove_prefix(key, key_prefix)
             if isinstance(key, str)
-            else key.decode(cls.Meta.encoding).split(":")[-1]
+            else remove_prefix(key.decode(cls.Meta.encoding), key_prefix)
             for key in cls.db().scan_iter(f"{key_prefix}*", _type="ReJSON-RL")
         )
 
     def update(self, **field_values):
         validate_model_fields(self.__class__, field_values)
         for field, value in field_values.items():
             # Handle the simple update case first, e.g. city="Happy Valley"
@@ -1555,15 +1725,15 @@
 
             # Set the target field (the last "part" of the nested update
             # field name) to the target value.
             setattr(obj, target_field, value)
         self.save()
 
     @classmethod
-    def get(cls, pk: Any) -> "JsonModel":
+    def get(cls: Type["Model"], pk: Any) -> "Model":
         document = json.dumps(cls.db().json().get(cls.make_key(pk)))
         if document == "null":
             raise NotFoundError
         return cls.parse_raw(document)
 
     @classmethod
     def redisearch_schema(cls):
@@ -1619,18 +1789,30 @@
 
         try:
             field_is_model = issubclass(typ, RedisModel)
         except TypeError:
             # Not a class, probably a type annotation
             field_is_model = False
 
+        vector_options: Optional[VectorFieldOptions] = getattr(
+            field_info, "vector_options", None
+        )
+        try:
+            is_vector = vector_options and any(
+                issubclass(get_args(typ)[0], t) for t in NUMERIC_TYPES
+            )
+        except IndexError:
+            raise RedisModelError(
+                f"Vector field '{name}' must be annotated as a container type"
+            )
+
         # When we encounter a list or model field, we need to descend
         # into the values of the list or the fields of the model to
         # find any values marked as indexed.
-        if is_container_type:
+        if is_container_type and not is_vector:
             field_type = get_origin(typ)
             embedded_cls = get_args(typ)
             if not embedded_cls:
                 log.warning(
                     "Model %s defined an empty list or tuple field: %s", cls, name
                 )
                 return ""
@@ -1685,15 +1867,17 @@
             sortable_tag_error = RedisModelError(
                 "In this Preview release, TAG fields cannot "
                 f"be marked as sortable. Problem field: {name}. "
                 "See docs: TODO"
             )
 
             # TODO: GEO field
-            if parent_is_container_type or parent_is_model_in_container:
+            if is_vector and vector_options:
+                schema = f"{path} AS {index_field_name} {vector_options.schema}"
+            elif parent_is_container_type or parent_is_model_in_container:
                 if typ is not str:
                     raise RedisModelError(
                         "In this Preview release, list and tuple fields can only "
                         f"contain strings. Problem field: {name}. See docs: TODO"
                     )
                 if full_text_search is True:
                     raise RedisModelError(
```

### Comparing `redis_om-0.1.2/redis_om/model/query_resolver.py` & `redis_om-0.1.3/redis_om/model/query_resolver.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/redis_om/model/render_tree.py` & `redis_om-0.1.3/redis_om/model/render_tree.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/redis_om/model/token_escaper.py` & `redis_om-0.1.3/redis_om/model/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.2/setup.py` & `redis_om-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,441 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: redis-om
+Version: 0.1.3
+Summary: Object mappings, and more, for Redis.
+Home-page: https://github.com/redis/redis-om-python
+License: BSD-3-Clause
+Author: Redis OSS
+Author-email: oss@redis.com
+Maintainer: Redis OSS
+Maintainer-email: oss@redis.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Requires-Dist: click (>=8.0.1,<9.0.0)
+Requires-Dist: hiredis (>=2.2.3,<3.0.0)
+Requires-Dist: more-itertools (>=8.14,<10.0)
+Requires-Dist: pydantic (>=1.10.2,<2.1.0)
+Requires-Dist: python-ulid (>=1.0.3,<2.0.0)
+Requires-Dist: redis (>=3.5.3,<5.0.0)
+Requires-Dist: types-redis (>=3.5.9,<5.0.0)
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Project-URL: Code, https://github.com/redis/redis-om-python
+Project-URL: Issue tracker, https://github.com/redis/redis-om-python/issues
+Project-URL: Repository, https://github.com/redis/redis-om-python
+Description-Content-Type: text/markdown
 
-packages = \
-['aredis_om',
- 'aredis_om.model',
- 'aredis_om.model.cli',
- 'aredis_om.model.migrations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.0.1,<9.0.0',
- 'hiredis>=2.0.0,<3.0.0',
- 'more-itertools>=8.14.0,<9.0.0',
- 'pptree>=3.1,<4.0',
- 'pydantic>=1.10.2,<2.0.0',
- 'python-ulid>=1.0.3,<2.0.0',
- 'redis>=3.5.3,<5.0.0',
- 'types-redis>=3.5.9,<5.0.0',
- 'typing-extensions>=4.4.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['migrate = redis_om.model.cli.migrate:migrate']}
-
-setup_kwargs = {
-    'name': 'redis-om',
-    'version': '0.1.2',
-    'description': 'Object mappings, and more, for Redis.',
-    'long_description': '<div align="center">\n  <br/>\n  <br/>\n  <img width="360" src="https://raw.githubusercontent.com/redis-developer/redis-om-python/main/images/logo.svg?token=AAAXXHUYL6RHPESRRAMBJOLBSVQXE" alt="Redis OM" />\n  <br/>\n  <br/>\n</div>\n\n<p align="center">\n    <p align="center">\n        Object mapping, and more, for Redis and Python\n    </p>\n</p>\n\n---\n\n[![Version][version-svg]][package-url]\n[![License][license-image]][license-url]\n[![Build Status][ci-svg]][ci-url]\n\n**Redis OM Python** makes it easy to model Redis data in your Python applications.\n\n[Redis OM .NET](https://github.com/redis/redis-om-dotnet) | [Redis OM Node.js](https://github.com/redis/redis-om-node) | [Redis OM Spring](https://github.com/redis/redis-om-spring) | **Redis OM Python**\n\n<details>\n  <summary><strong>Table of contents</strong></summary>\n\nspan\n\n<!-- DON\'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->\n\n- [💡 Why Redis OM?](#-why-redis-om)\n- [📇 Modeling Your Data](#-modeling-your-data)\n- [✓ Validating Data With Your Model](#-validating-data-with-your-model)\n- [🔎 Rich Queries and Embedded Models](#-rich-queries-and-embedded-models)\n  - [Querying](#querying)\n  - [Embedded Models](#embedded-models)\n- [Calling Other Redis Commands](#calling-other-redis-commands)\n- [💻 Installation](#-installation)\n- [📚 Documentation](#-documentation)\n- [⛏️ Troubleshooting](#️-troubleshooting)\n- [✨ So How Do You Get RediSearch and RedisJSON?](#-so-how-do-you-get-redisearch-and-redisjson)\n- [❤️ Contributing](#️-contributing)\n- [📝 License](#-license)\n\n<!-- END doctoc generated TOC please keep comment here to allow auto update -->\n\n</details>\n\n## 💡 Why Redis OM?\n\nRedis OM provides high-level abstractions that make it easy to model and query data in Redis with modern Python applications.\n\nThis **preview** release contains the following features:\n\n* Declarative object mapping for Redis objects\n* Declarative secondary-index generation\n* Fluent APIs for querying Redis\n\n## 📇 Modeling Your Data\n\nRedis OM contains powerful declarative models that give you data validation, serialization, and persistence to Redis.\n\nCheck out this example of modeling customer data with Redis OM. First, we create a `Customer` model:\n\n```python\nimport datetime\nfrom typing import Optional\n\nfrom pydantic import EmailStr\n\nfrom redis_om import HashModel\n\n\nclass Customer(HashModel):\n    first_name: str\n    last_name: str\n    email: EmailStr\n    join_date: datetime.date\n    age: int\n    bio: Optional[str]\n```\n\nNow that we have a `Customer` model, let\'s use it to save customer data to Redis.\n\n```python\nimport datetime\nfrom typing import Optional\n\nfrom pydantic import EmailStr\n\nfrom redis_om import HashModel\n\n\nclass Customer(HashModel):\n    first_name: str\n    last_name: str\n    email: EmailStr\n    join_date: datetime.date\n    age: int\n    bio: Optional[str]\n\n\n# First, we create a new `Customer` object:\nandrew = Customer(\n    first_name="Andrew",\n    last_name="Brookins",\n    email="andrew.brookins@example.com",\n    join_date=datetime.date.today(),\n    age=38,\n    bio="Python developer, works at Redis, Inc."\n)\n\n# The model generates a globally unique primary key automatically\n# without needing to talk to Redis.\nprint(andrew.pk)\n# > "01FJM6PH661HCNNRC884H6K30C"\n\n# We can save the model to Redis by calling `save()`:\nandrew.save()\n\n# Expire the model after 2 mins (120 seconds)\nandrew.expire(120)\n\n# To retrieve this customer with its primary key, we use `Customer.get()`:\nassert Customer.get(andrew.pk) == andrew\n```\n\n**Ready to learn more?** Check out the [getting started](docs/getting_started.md) guide.\n\nOr, continue reading to see how Redis OM makes data validation a snap.\n\n## ✓ Validating Data With Your Model\n\nRedis OM uses [Pydantic][pydantic-url] to validate data based on the type annotations you assign to fields in a model class.\n\nThis validation ensures that fields like `first_name`, which the `Customer` model marked as a `str`, are always strings. **But every Redis OM model is also a Pydantic model**, so you can use Pydantic validators like `EmailStr`, `Pattern`, and many more for complex validations!\n\nFor example, because we used the `EmailStr` type for the `email` field, we\'ll get a validation error if we try to create a `Customer` with an invalid email address:\n\n```python\nimport datetime\nfrom typing import Optional\n\nfrom pydantic import EmailStr, ValidationError\n\nfrom redis_om import HashModel\n\n\nclass Customer(HashModel):\n    first_name: str\n    last_name: str\n    email: EmailStr\n    join_date: datetime.date\n    age: int\n    bio: Optional[str]\n\n\ntry:\n    Customer(\n        first_name="Andrew",\n        last_name="Brookins",\n        email="Not an email address!",\n        join_date=datetime.date.today(),\n        age=38,\n        bio="Python developer, works at Redis, Inc."\n    )\nexcept ValidationError as e:\n    print(e)\n    """\n    pydantic.error_wrappers.ValidationError: 1 validation error for Customer\n     email\n       value is not a valid email address (type=value_error.email)\n    """\n```\n\n**Any existing Pydantic validator should work** as a drop-in type annotation with a Redis OM model. You can also write arbitrarily complex custom validations!\n\nTo learn more, see the [documentation on data validation](docs/validation.md).\n\n## 🔎 Rich Queries and Embedded Models\n\nData modeling, validation, and saving models to Redis all work regardless of how you run Redis.\n\nNext, we\'ll show you the **rich query expressions** and **embedded models** Redis OM provides when the [RediSearch][redisearch-url] and [RedisJSON][redis-json-url] modules are installed in your Redis deployment, or you\'re using [Redis Enterprise][redis-enterprise-url].\n\n**TIP**: *Wait, what\'s a Redis module?* If you aren\'t familiar with Redis modules, review the [So, How Do You Get RediSearch and RedisJSON?](#-so-how-do-you-get-redisearch-and-redisjson) section of this README.\n\n### Querying\n\nRedis OM comes with a rich query language that allows you to query Redis with Python expressions.\n\nTo show how this works, we\'ll make a small change to the `Customer` model we defined earlier. We\'ll add `Field(index=True)` to tell Redis OM that we want to index the `last_name` and `age` fields:\n\n```python\nimport datetime\nfrom typing import Optional\n\nfrom pydantic import EmailStr\n\nfrom redis_om import (\n    Field,\n    HashModel,\n    Migrator\n)\n\n                 \nclass Customer(HashModel):\n    first_name: str\n    last_name: str = Field(index=True)\n    email: EmailStr\n    join_date: datetime.date\n    age: int = Field(index=True)\n    bio: Optional[str]\n\n\n# Now, if we use this model with a Redis deployment that has the\n# RediSearch module installed, we can run queries like the following.\n\n# Before running queries, we need to run migrations to set up the\n# indexes that Redis OM will use. You can also use the `migrate`\n# CLI tool for this!\nMigrator().run()\n\n# Find all customers with the last name "Brookins"\nCustomer.find(Customer.last_name == "Brookins").all()\n\n# Find all customers that do NOT have the last name "Brookins"\nCustomer.find(Customer.last_name != "Brookins").all()\n\n# Find all customers whose last name is "Brookins" OR whose age is \n# 100 AND whose last name is "Smith"\nCustomer.find((Customer.last_name == "Brookins") | (\n        Customer.age == 100\n) & (Customer.last_name == "Smith")).all()\n```\n\nThese queries -- and more! -- are possible because **Redis OM manages indexes for you automatically**.\n\nQuerying with this index features a rich expression syntax inspired by the Django ORM, SQLAlchemy, and Peewee. We think you\'ll enjoy it!\n\n**Note:** Indexing only works for data stored in Redis logical database 0.  If you are using a different database number when connecting to Redis, you can expect the code to raise a `MigrationError` when you run the migrator.\n\n### Embedded Models\n\nRedis OM can store and query **nested models** like any document database, with the speed and power you get from Redis. Let\'s see how this works.\n\nIn the next example, we\'ll define a new `Address` model and embed it within the `Customer` model.\n\n```python\nimport datetime\nfrom typing import Optional\n\nfrom redis_om import (\n    EmbeddedJsonModel,\n    JsonModel,\n    Field,\n    Migrator,\n)\n\n\nclass Address(EmbeddedJsonModel):\n    address_line_1: str\n    address_line_2: Optional[str]\n    city: str = Field(index=True)\n    state: str = Field(index=True)\n    country: str\n    postal_code: str = Field(index=True)\n\n\nclass Customer(JsonModel):\n    first_name: str = Field(index=True)\n    last_name: str = Field(index=True)\n    email: str = Field(index=True)\n    join_date: datetime.date\n    age: int = Field(index=True)\n    bio: Optional[str] = Field(index=True, full_text_search=True,\n                               default="")\n\n    # Creates an embedded model.\n    address: Address\n\n\n# With these two models and a Redis deployment with the RedisJSON \n# module installed, we can run queries like the following.\n\n# Before running queries, we need to run migrations to set up the\n# indexes that Redis OM will use. You can also use the `migrate`\n# CLI tool for this!\nMigrator().run()\n\n# Find all customers who live in San Antonio, TX\nCustomer.find(Customer.address.city == "San Antonio",\n              Customer.address.state == "TX")\n```\n\n## Calling Other Redis Commands\n\nSometimes you\'ll need to run a Redis command directly.  Redis OM supports this through the `db` method on your model\'s class.  This returns a connected Redis client instance which exposes a function named for each Redis command.  For example, let\'s perform some basic set operations:\n\n```python\nfrom redis_om import HashModel\n\nclass Demo(HashModel):\n    some_field: str\n\nredis_conn = Demo.db()\n\nredis_conn.sadd("myset", "a", "b", "c", "d")\n\n# Prints False\nprint(redis_conn.sismember("myset", "e"))\n\n# Prints True\nprint(redis_conn.sismember("myset", "b"))\n```\n\nThe parameters expected by each command function are those documented on the command\'s page on [redis.io](https://redis.io/commands/).\n\nIf you don\'t want to get a Redis connection from a model class, you can also use `get_redis_connection`:\n\n```python\nfrom redis_om import get_redis_connection\n\nredis_conn = get_redis_connection()\nredis_conn.set("hello", "world")\n```\n\n## 💻 Installation\n\nInstallation is simple with `pip`, Poetry, or Pipenv.\n\n```sh\n# With pip\n$ pip install redis-om\n\n# Or, using Poetry\n$ poetry add redis-om\n```\n\n## 📚 Documentation\n\nThe Redis OM documentation is available [here](docs/index.md).\n\n## ⛏️ Troubleshooting\n\nIf you run into trouble or have any questions, we\'re here to help!\n\nHit us up on the [Redis Discord Server](http://discord.gg/redis) or [open an issue on GitHub](https://github.com/redis-developer/redis-om-python/issues/new).\n\n## ✨ So How Do You Get RediSearch and RedisJSON?\n\nSome advanced features of Redis OM rely on core features from two source available Redis modules: [RediSearch][redisearch-url] and [RedisJSON][redis-json-url].\n\nYou can run these modules in your self-hosted Redis deployment, or you can use [Redis Enterprise][redis-enterprise-url], which includes both modules.\n\nTo learn more, read [our documentation](docs/redis_modules.md).\n\n## ❤️ Contributing\n\nWe\'d love your contributions!\n\n**Bug reports** are especially helpful at this stage of the project. [You can open a bug report on GitHub](https://github.com/redis/redis-om-python/issues/new).\n\nYou can also **contribute documentation** -- or just let us know if something needs more detail. [Open an issue on GitHub](https://github.com/redis/redis-om-python/issues/new) to get started.\n\n## 📝 License\n\nRedis OM uses the [MIT license][license-url].\n\n<!-- Badges -->\n\n[version-svg]: https://img.shields.io/pypi/v/redis-om?style=flat-square\n[package-url]: https://pypi.org/project/redis-om/\n[ci-svg]: https://img.shields.io/github/workflow/status/redis/redis-om-python/CI?style=flat-square\n[ci-url]: https://github.com/redis/redis-om-python/actions/workflows/CI.yml\n[license-image]: https://img.shields.io/badge/license-mit-green.svg?style=flat-square\n[license-url]: LICENSE\n<!-- Links -->\n\n[redis-om-website]: https://developer.redis.com\n[redis-om-js]: https://github.com/redis-om/redis-om-js\n[redis-om-dotnet]: https://github.com/redis-om/redis-om-dotnet\n[redis-om-spring]: https://github.com/redis-om/redis-om-spring\n[redisearch-url]: https://redis.io/docs/stack/search/\n[redis-json-url]: https://redis.io/docs/stack/json/\n[pydantic-url]: https://github.com/samuelcolvin/pydantic\n[ulid-url]: https://github.com/ulid/spec\n[redis-enterprise-url]: https://redis.com/try-free/\n',
-    'author': 'Redis OSS',
-    'author_email': 'oss@redis.com',
-    'maintainer': 'Redis OSS',
-    'maintainer_email': 'oss@redis.com',
-    'url': 'https://github.com/redis/redis-om-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+<div align="center">
+  <br/>
+  <br/>
+  <img width="360" src="https://raw.githubusercontent.com/redis-developer/redis-om-python/main/images/logo.svg?token=AAAXXHUYL6RHPESRRAMBJOLBSVQXE" alt="Redis OM" />
+  <br/>
+  <br/>
+</div>
 
+<p align="center">
+    <p align="center">
+        Object mapping, and more, for Redis and Python
+    </p>
+</p>
+
+---
+
+[![Version][version-svg]][package-url]
+[![License][license-image]][license-url]
+[![Build Status][ci-svg]][ci-url]
+
+**Redis OM Python** makes it easy to model Redis data in your Python applications.
+
+[Redis OM .NET](https://github.com/redis/redis-om-dotnet) | [Redis OM Node.js](https://github.com/redis/redis-om-node) | [Redis OM Spring](https://github.com/redis/redis-om-spring) | **Redis OM Python**
+
+<details>
+  <summary><strong>Table of contents</strong></summary>
+
+span
+
+<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
+
+- [💡 Why Redis OM?](#-why-redis-om)
+- [💻 Installation](#-installation)
+- [🏁 Getting started](#-getting-started)
+- [📇 Modeling Your Data](#-modeling-your-data)
+- [✓ Validating Data With Your Model](#-validating-data-with-your-model)
+- [🔎 Rich Queries and Embedded Models](#-rich-queries-and-embedded-models)
+  - [Querying](#querying)
+  - [Embedded Models](#embedded-models)
+- [Calling Other Redis Commands](#calling-other-redis-commands)
+- [📚 Documentation](#-documentation)
+- [⛏️ Troubleshooting](#️-troubleshooting)
+- [✨ So How Do You Get RediSearch and RedisJSON?](#-so-how-do-you-get-redisearch-and-redisjson)
+- [❤️ Contributing](#️-contributing)
+- [📝 License](#-license)
+
+<!-- END doctoc generated TOC please keep comment here to allow auto update -->
+
+</details>
+
+## 💡 Why Redis OM?
+
+Redis OM provides high-level abstractions that make it easy to model and query data in Redis with modern Python applications.
+
+This **preview** release contains the following features:
+
+* Declarative object mapping for Redis objects
+* Declarative secondary-index generation
+* Fluent APIs for querying Redis
+
+## 💻 Installation
+
+Installation is simple with `pip`, Poetry, or Pipenv.
+
+```sh
+# With pip
+$ pip install redis-om
+
+# Or, using Poetry
+$ poetry add redis-om
+```
+
+## 🏁 Getting started
+
+### Starting Redis
+
+Before writing any code you'll need a Redis instance with the appropriate Redis modules! The quickest way to get this is with Docker:
+
+```sh
+docker run -p 6379:6379 -p 8001:8001 redis/redis-stack
+```
+
+This launches the [redis-stack](https://redis.io/docs/stack/) an extension of Redis that adds all manner of modern data structures to Redis. You'll also notice that if you open up http://localhost:8001 you'll have access to the redis-insight GUI, a GUI you can use to visualize and work with your data in Redis.
+
+
+## 📇 Modeling Your Data
+
+Redis OM contains powerful declarative models that give you data validation, serialization, and persistence to Redis.
+
+Check out this example of modeling customer data with Redis OM. First, we create a `Customer` model:
+
+```python
+import datetime
+from typing import Optional
+
+from pydantic import EmailStr
+
+from redis_om import HashModel
+
+
+class Customer(HashModel):
+    first_name: str
+    last_name: str
+    email: EmailStr
+    join_date: datetime.date
+    age: int
+    bio: Optional[str]
+```
+
+Now that we have a `Customer` model, let's use it to save customer data to Redis.
+
+```python
+import datetime
+from typing import Optional
+
+from pydantic import EmailStr
+
+from redis_om import HashModel
+
+
+class Customer(HashModel):
+    first_name: str
+    last_name: str
+    email: EmailStr
+    join_date: datetime.date
+    age: int
+    bio: Optional[str]
+
+
+# First, we create a new `Customer` object:
+andrew = Customer(
+    first_name="Andrew",
+    last_name="Brookins",
+    email="andrew.brookins@example.com",
+    join_date=datetime.date.today(),
+    age=38,
+    bio="Python developer, works at Redis, Inc."
+)
+
+# The model generates a globally unique primary key automatically
+# without needing to talk to Redis.
+print(andrew.pk)
+# > "01FJM6PH661HCNNRC884H6K30C"
+
+# We can save the model to Redis by calling `save()`:
+andrew.save()
+
+# Expire the model after 2 mins (120 seconds)
+andrew.expire(120)
+
+# To retrieve this customer with its primary key, we use `Customer.get()`:
+assert Customer.get(andrew.pk) == andrew
+```
+
+**Ready to learn more?** Check out the [getting started](docs/getting_started.md) guide.
+
+Or, continue reading to see how Redis OM makes data validation a snap.
+
+## ✓ Validating Data With Your Model
+
+Redis OM uses [Pydantic][pydantic-url] to validate data based on the type annotations you assign to fields in a model class.
+
+This validation ensures that fields like `first_name`, which the `Customer` model marked as a `str`, are always strings. **But every Redis OM model is also a Pydantic model**, so you can use Pydantic validators like `EmailStr`, `Pattern`, and many more for complex validations!
+
+For example, because we used the `EmailStr` type for the `email` field, we'll get a validation error if we try to create a `Customer` with an invalid email address:
+
+```python
+import datetime
+from typing import Optional
+
+from pydantic import EmailStr, ValidationError
+
+from redis_om import HashModel
+
+
+class Customer(HashModel):
+    first_name: str
+    last_name: str
+    email: EmailStr
+    join_date: datetime.date
+    age: int
+    bio: Optional[str]
+
+
+try:
+    Customer(
+        first_name="Andrew",
+        last_name="Brookins",
+        email="Not an email address!",
+        join_date=datetime.date.today(),
+        age=38,
+        bio="Python developer, works at Redis, Inc."
+    )
+except ValidationError as e:
+    print(e)
+    """
+    pydantic.error_wrappers.ValidationError: 1 validation error for Customer
+     email
+       value is not a valid email address (type=value_error.email)
+    """
+```
+
+**Any existing Pydantic validator should work** as a drop-in type annotation with a Redis OM model. You can also write arbitrarily complex custom validations!
+
+To learn more, see the [documentation on data validation](docs/validation.md).
+
+## 🔎 Rich Queries and Embedded Models
+
+Data modeling, validation, and saving models to Redis all work regardless of how you run Redis.
+
+Next, we'll show you the **rich query expressions** and **embedded models** Redis OM provides when the [RediSearch][redisearch-url] and [RedisJSON][redis-json-url] modules are installed in your Redis deployment, or you're using [Redis Enterprise][redis-enterprise-url].
+
+**TIP**: *Wait, what's a Redis module?* If you aren't familiar with Redis modules, review the [So, How Do You Get RediSearch and RedisJSON?](#-so-how-do-you-get-redisearch-and-redisjson) section of this README.
+
+### Querying
+
+Redis OM comes with a rich query language that allows you to query Redis with Python expressions.
+
+To show how this works, we'll make a small change to the `Customer` model we defined earlier. We'll add `Field(index=True)` to tell Redis OM that we want to index the `last_name` and `age` fields:
+
+```python
+import datetime
+from typing import Optional
+
+from pydantic import EmailStr
+
+from redis_om import (
+    Field,
+    HashModel,
+    Migrator
+)
+
+
+class Customer(HashModel):
+    first_name: str
+    last_name: str = Field(index=True)
+    email: EmailStr
+    join_date: datetime.date
+    age: int = Field(index=True)
+    bio: Optional[str]
+
+
+# Now, if we use this model with a Redis deployment that has the
+# RediSearch module installed, we can run queries like the following.
+
+# Before running queries, we need to run migrations to set up the
+# indexes that Redis OM will use. You can also use the `migrate`
+# CLI tool for this!
+Migrator().run()
+
+# Find all customers with the last name "Brookins"
+Customer.find(Customer.last_name == "Brookins").all()
+
+# Find all customers that do NOT have the last name "Brookins"
+Customer.find(Customer.last_name != "Brookins").all()
+
+# Find all customers whose last name is "Brookins" OR whose age is
+# 100 AND whose last name is "Smith"
+Customer.find((Customer.last_name == "Brookins") | (
+        Customer.age == 100
+) & (Customer.last_name == "Smith")).all()
+```
+
+These queries -- and more! -- are possible because **Redis OM manages indexes for you automatically**.
+
+Querying with this index features a rich expression syntax inspired by the Django ORM, SQLAlchemy, and Peewee. We think you'll enjoy it!
+
+**Note:** Indexing only works for data stored in Redis logical database 0.  If you are using a different database number when connecting to Redis, you can expect the code to raise a `MigrationError` when you run the migrator.
+
+### Embedded Models
+
+Redis OM can store and query **nested models** like any document database, with the speed and power you get from Redis. Let's see how this works.
+
+In the next example, we'll define a new `Address` model and embed it within the `Customer` model.
+
+```python
+import datetime
+from typing import Optional
+
+from redis_om import (
+    EmbeddedJsonModel,
+    JsonModel,
+    Field,
+    Migrator,
+)
+
+
+class Address(EmbeddedJsonModel):
+    address_line_1: str
+    address_line_2: Optional[str]
+    city: str = Field(index=True)
+    state: str = Field(index=True)
+    country: str
+    postal_code: str = Field(index=True)
+
+
+class Customer(JsonModel):
+    first_name: str = Field(index=True)
+    last_name: str = Field(index=True)
+    email: str = Field(index=True)
+    join_date: datetime.date
+    age: int = Field(index=True)
+    bio: Optional[str] = Field(index=True, full_text_search=True,
+                               default="")
+
+    # Creates an embedded model.
+    address: Address
+
+
+# With these two models and a Redis deployment with the RedisJSON
+# module installed, we can run queries like the following.
+
+# Before running queries, we need to run migrations to set up the
+# indexes that Redis OM will use. You can also use the `migrate`
+# CLI tool for this!
+Migrator().run()
+
+# Find all customers who live in San Antonio, TX
+Customer.find(Customer.address.city == "San Antonio",
+              Customer.address.state == "TX")
+```
+
+## Calling Other Redis Commands
+
+Sometimes you'll need to run a Redis command directly.  Redis OM supports this through the `db` method on your model's class.  This returns a connected Redis client instance which exposes a function named for each Redis command.  For example, let's perform some basic set operations:
+
+```python
+from redis_om import HashModel
+
+class Demo(HashModel):
+    some_field: str
+
+redis_conn = Demo.db()
+
+redis_conn.sadd("myset", "a", "b", "c", "d")
+
+# Prints False
+print(redis_conn.sismember("myset", "e"))
+
+# Prints True
+print(redis_conn.sismember("myset", "b"))
+```
+
+The parameters expected by each command function are those documented on the command's page on [redis.io](https://redis.io/commands/).
+
+If you don't want to get a Redis connection from a model class, you can also use `get_redis_connection`:
+
+```python
+from redis_om import get_redis_connection
+
+redis_conn = get_redis_connection()
+redis_conn.set("hello", "world")
+```
+
+## 📚 Documentation
+
+The Redis OM documentation is available [here](docs/index.md).
+
+## ⛏️ Troubleshooting
+
+If you run into trouble or have any questions, we're here to help!
+
+Hit us up on the [Redis Discord Server](http://discord.gg/redis) or [open an issue on GitHub](https://github.com/redis-developer/redis-om-python/issues/new).
+
+## ✨ So How Do You Get RediSearch and RedisJSON?
+
+Some advanced features of Redis OM rely on core features from two source available Redis modules: [RediSearch][redisearch-url] and [RedisJSON][redis-json-url].
+
+You can run these modules in your self-hosted Redis deployment, or you can use [Redis Enterprise][redis-enterprise-url], which includes both modules.
+
+To learn more, read [our documentation](docs/redis_modules.md).
+
+## ❤️ Contributing
+
+We'd love your contributions!
+
+**Bug reports** are especially helpful at this stage of the project. [You can open a bug report on GitHub](https://github.com/redis/redis-om-python/issues/new).
+
+You can also **contribute documentation** -- or just let us know if something needs more detail. [Open an issue on GitHub](https://github.com/redis/redis-om-python/issues/new) to get started.
+
+## 📝 License
+
+Redis OM uses the [MIT license][license-url].
+
+<!-- Badges -->
+
+[version-svg]: https://img.shields.io/pypi/v/redis-om?style=flat-square
+[package-url]: https://pypi.org/project/redis-om/
+[ci-svg]: https://img.shields.io/github/workflow/status/redis/redis-om-python/ci?style=flat-square
+[ci-url]: https://github.com/redis/redis-om-python/actions/workflows/ci.yml
+[license-image]: https://img.shields.io/badge/license-mit-green.svg?style=flat-square
+[license-url]: LICENSE
+<!-- Links -->
+
+[redis-om-website]: https://developer.redis.com
+[redis-om-js]: https://github.com/redis-om/redis-om-js
+[redis-om-dotnet]: https://github.com/redis-om/redis-om-dotnet
+[redis-om-spring]: https://github.com/redis-om/redis-om-spring
+[redisearch-url]: https://redis.io/docs/stack/search/
+[redis-json-url]: https://redis.io/docs/stack/json/
+[pydantic-url]: https://github.com/samuelcolvin/pydantic
+[ulid-url]: https://github.com/ulid/spec
+[redis-enterprise-url]: https://redis.com/try-free/
 
-setup(**setup_kwargs)
```

