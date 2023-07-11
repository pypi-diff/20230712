# Comparing `tmp/fondat-4.1.4.tar.gz` & `tmp/fondat-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat-4.1.4.tar", max compression
+gzip compressed data, was "fondat-4.1.5.tar", max compression
```

## Comparing `fondat-4.1.4.tar` & `fondat-4.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.4/LICENSE
--rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.4/README.md
--rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.4/fondat/annotation.py
--rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.4/fondat/asgi.py
--rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.4/fondat/cache.py
--rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.4/fondat/codec.py
--rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.4/fondat/context.py
--rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.4/fondat/csv.py
--rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.4/fondat/data.py
--rw-r--r--   0        0        0     2444 2022-09-25 17:46:57.851193 fondat-4.1.4/fondat/error.py
--rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.4/fondat/file.py
--rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.4/fondat/http.py
--rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.4/fondat/lazy.py
--rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.4/fondat/memory.py
--rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.4/fondat/monitor.py
--rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.4/fondat/oauth.py
--rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.4/fondat/openapi.py
--rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.4/fondat/pagination.py
--rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.4/fondat/patch.py
--rw-r--r--   0        0        0    11398 2023-05-28 15:08:56.067124 fondat-4.1.4/fondat/resource.py
--rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.4/fondat/security.py
--rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.4/fondat/sql.py
--rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.4/fondat/sqlite.py
--rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.4/fondat/stream.py
--rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.4/fondat/string.py
--rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.4/fondat/types.py
--rw-r--r--   0        0        0    10948 2022-09-30 06:16:57.338274 fondat-4.1.4/fondat/validation.py
--rw-r--r--   0        0        0     1172 2023-06-22 07:22:32.061609 fondat-4.1.4/pyproject.toml
--rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 fondat-4.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.5/LICENSE
+-rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.5/README.md
+-rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.5/fondat/annotation.py
+-rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.5/fondat/asgi.py
+-rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.5/fondat/cache.py
+-rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.5/fondat/codec.py
+-rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.5/fondat/context.py
+-rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.5/fondat/csv.py
+-rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.5/fondat/data.py
+-rw-r--r--   0        0        0     2444 2023-07-11 20:44:25.310120 fondat-4.1.5/fondat/error.py
+-rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.5/fondat/file.py
+-rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.5/fondat/http.py
+-rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.5/fondat/lazy.py
+-rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.5/fondat/memory.py
+-rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.5/fondat/monitor.py
+-rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.5/fondat/oauth.py
+-rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.5/fondat/openapi.py
+-rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.5/fondat/pagination.py
+-rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.5/fondat/patch.py
+-rw-r--r--   0        0        0    11552 2023-07-11 21:43:50.415822 fondat-4.1.5/fondat/resource.py
+-rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.5/fondat/security.py
+-rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.5/fondat/sql.py
+-rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.5/fondat/sqlite.py
+-rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.5/fondat/stream.py
+-rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.5/fondat/string.py
+-rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.5/fondat/types.py
+-rw-r--r--   0        0        0    12794 2023-07-11 22:04:46.524331 fondat-4.1.5/fondat/validation.py
+-rw-r--r--   0        0        0     1171 2023-07-11 22:13:45.993901 fondat-4.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 fondat-4.1.5/PKG-INFO
```

### Comparing `fondat-4.1.4/LICENSE` & `fondat-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/README.md` & `fondat-4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/annotation.py` & `fondat-4.1.5/fondat/annotation.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/asgi.py` & `fondat-4.1.5/fondat/asgi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/cache.py` & `fondat-4.1.5/fondat/cache.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/codec.py` & `fondat-4.1.5/fondat/codec.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/context.py` & `fondat-4.1.5/fondat/context.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/csv.py` & `fondat-4.1.5/fondat/csv.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/data.py` & `fondat-4.1.5/fondat/data.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/error.py` & `fondat-4.1.5/fondat/error.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/file.py` & `fondat-4.1.5/fondat/file.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/http.py` & `fondat-4.1.5/fondat/http.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/lazy.py` & `fondat-4.1.5/fondat/lazy.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/memory.py` & `fondat-4.1.5/fondat/memory.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/monitor.py` & `fondat-4.1.5/fondat/monitor.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/oauth.py` & `fondat-4.1.5/fondat/oauth.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/openapi.py` & `fondat-4.1.5/fondat/openapi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/pagination.py` & `fondat-4.1.5/fondat/pagination.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/patch.py` & `fondat-4.1.5/fondat/patch.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/resource.py` & `fondat-4.1.5/fondat/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 or property would have a return type as a class decorated with @resource. 
 
 For information on how security policies are evaluated, see the `authorize` function.
 """
 
 import asyncio
 import fondat.context as context
+import fondat.error
 import fondat.monitor as monitor
 import functools
 import inspect
 import logging
 import types
 import wrapt
 
 from collections.abc import Callable, Iterable, Mapping
 from contextlib import contextmanager, suppress
 from fondat.cache import CacheResource, hash_json
 from fondat.codec import JSONCodec
-from fondat.error import BadRequestError, ForbiddenError, NotFoundError, UnauthorizedError
 from fondat.lazy import LazySimpleNamespace
 from fondat.security import Policy
 from fondat.types import literal_values
-from fondat.validation import ValidationError, validate_arguments
+from fondat.validation import validate_arguments
 from typing import Any, Literal, TypeVar
 
 
 T = TypeVar("T")
 
 
 _logger = logging.getLogger(__name__)
@@ -72,18 +72,18 @@
     is raised if encountered, otherwise the first UnauthorizedError exception is raised.
     """
     exception = None
     for policy in policies or ():
         try:
             await policy.apply()
             return  # security policy authorized the operation
-        except ForbiddenError as fe:
-            if not isinstance(exception, ForbiddenError):
+        except fondat.error.ForbiddenError as fe:
+            if not isinstance(exception, fondat.error.ForbiddenError):
                 exception = fe
-        except UnauthorizedError as ue:
+        except fondat.error.UnauthorizedError as ue:
             if not exception:
                 exception = ue
         except:
             raise
     if exception:
         raise exception
 
@@ -142,15 +142,15 @@
 
     When an operation is called:
     • its arguments are copied to prevent side effects
     • its arguments are validated against their type hints
 
     Exceptions that an operation should raise:
     • fondat.error.Error (e.g. BadRequestError)
-    • fondat.validation.ValidationError (automatically reraised as a BadRequestError)
+    • ValueError (automatically reraised as a fondat.error.BadRequestError)
 
     The cache is a resource that exposes cache entry resources. A MemoryResource can serve as
     an operation cache resource out of the box. It is safe for a single cache resource to be
     shared by multiple operations.
     """
 
     if wrapped is None:
@@ -216,22 +216,26 @@
                 name="operation_invocations", tags=tags, status="status"
             ):
                 async with monitor.timer(name="operation_duration", tags=tags):
                     await authorize(operation.policies)
                     if cache:
                         cache_args = JSONCodec.get(Any).encode(defaults | arguments)
                         cache_entry = cache[tags | {"arguments": cache_args}]
-                        with suppress(NotFoundError):
+                        with suppress(fondat.error.NotFoundError):
                             result = JSONCodec.get(returns).decode(await cache_entry.get())
                             _logger.debug("returning cached result")
                             return result
                     try:
                         result = await wrapped(*args, **kwargs)
-                    except ValidationError as ve:
-                        raise BadRequestError from ve
+                    except fondat.error.Error:
+                        raise
+                    except ValueError as ve:
+                        raise fondat.error.BadRequestError from ve
+                    except Exception as ex:
+                        raise fondat.error.InternalServerError from ex
                     if cache:
                         await cache_entry.put(JSONCodec.get(returns).encode(result))
                     return result
 
     wrapped._fondat_operation = types.SimpleNamespace(
         method=method,
         type=type,
```

### Comparing `fondat-4.1.4/fondat/security.py` & `fondat-4.1.5/fondat/security.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/sql.py` & `fondat-4.1.5/fondat/sql.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/sqlite.py` & `fondat-4.1.5/fondat/sqlite.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/stream.py` & `fondat-4.1.5/fondat/stream.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/string.py` & `fondat-4.1.5/fondat/string.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/types.py` & `fondat-4.1.5/fondat/types.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.4/fondat/validation.py` & `fondat-4.1.5/fondat/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,32 +13,40 @@
 from contextlib import contextmanager
 from fondat.types import is_instance, is_subclass, split_annotations
 from types import NoneType
 from typing import Any, TypeVar
 
 
 class ValidationError(ValueError):
-    """Error raised when validation fails."""
+    """
+    Error raised when a validation fails.
 
-    __slots__ = {"message", "path"}
-
-    def __init__(self, message: str | None = None, path: list[str | int] | None = None):
+    Parameters:
+    • message: human-readable error message
+    • path: path to the attribute that is the subject of the validation error
+    • code: machine-readable error code
+    """
+
+    __slots__ = {"message", "path", "code"}
+
+    def __init__(
+        self,
+        message: str | None = None,
+        path: list[str | int] | None = None,
+        code: str | None = None,
+    ):
         self.message = message
         self.path = path
+        self.code = code
 
     def __repr__(self):
-        return f"{self.__class__.__name__}({self.message!r}, {self.path!r})"
+        return f"{self.__class__.__name__}({self.message!r}, {self.path!r}, {self.code!r})"
 
     def __str__(self):
-        result = []
-        if self.message is not None:
-            result.append(str(self.message))
-        if self.path:
-            result.append(f"({'.'.join((str(a) for a in self.path))})")
-        return " ".join(result)
+        return self.message or self.code
 
     @staticmethod
     @contextmanager
     def path_on_error(path: list[str | int] | str | int):
         """Context manager to specify error path in the event that a DecodeError is raised."""
         try:
             yield
@@ -49,14 +57,72 @@
                 case str() | int():
                     ve.path.insert(0, path)
                 case list():
                     ve.path = path + ve.path
             raise
 
 
+class ValidationErrors(ValueError):
+    """
+    Error that collects multiple validation errors, to be raised together.
+
+    Parameters and attributes:
+    • errors: collected validation errors
+    """
+
+    __slots__ = {"errors"}
+
+    def __init__(self, *errors):
+        self.errors = list(errors)
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}{', '.join(self.errors)!r})"
+
+    def __str__(self):
+        return ", ".join(str(e) for e in self.errors)
+
+    def __len__(self):
+        return len(self.errors)
+
+    def __bool__(self):
+        return bool(self.errors)
+
+    def __iter__(self):
+        return iter(self.errors)
+
+    @classmethod
+    @contextmanager
+    def collect(cls) -> Iterable["ValidationErrors"]:
+        """
+        Establish a context around a new ValidationErrors exception. Upon exit of the context,
+        if the ValidationErrors exception contains any ValidationError exceptions, the new
+        ValidationErrors exception will be raised.
+        """
+        validation_errors = ValidationErrors()
+        yield validation_errors
+        if validation_errors.errors:
+            raise validation_errors
+
+    @contextmanager
+    def catch(self) -> Iterable[None]:
+        """
+        Establish a context to catch a ValidationError exception and add it to the
+        ValidationErrors exception. If an error is caught, it will be suppressed and execution
+        will continue outside of the context.
+        """
+        try:
+            yield
+        except ValidationError as ve:
+            self.add(ve)
+
+    def add(self, error: "ValidationError") -> None:
+        """Add a ValidationError exception to the ValidationErrors exception."""
+        self.errors.append(error)
+
+
 class Validator:
     """Base class for type annotation that performs validation."""
 
     def validate(self, value: Any) -> None:
         raise NotImplementedError
```

### Comparing `fondat-4.1.4/pyproject.toml` & `fondat-4.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat"
-version = "4.1.4" 
+version = "4.1.5"
 description = "A foundation for resource-oriented backend applications."
 readme = "README.md"
 authors = ["fondat authors"]
 homepage = "https://github.com/fondat/fondat/"
 documentation = "https://github.com/fondat/fondat/tree/main/docs"
 license = "MIT"
 keywords = ["asgi", "foundation", "resource", "openapi"]
@@ -24,23 +24,23 @@
 packages = [
     { include = "fondat" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiosqlite = "^0.19"
-iso8601 = "^1.1"
+iso8601 = "^2.0"
 multidict = "^6.0"
 wrapt = "^1.15"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3"
+black = "^23.7"
 isort = "^5.12"
 pre-commit = "^3.3"
-pytest = "^7.3"
+pytest = "^7.4"
 pytest-asyncio = "^0.21"
 pytest-cov = "^4.1"
 
 [tool.isort]
 profile = "black"
 lexicographical = true
 lines_after_imports = 2
```

### Comparing `fondat-4.1.4/PKG-INFO` & `fondat-4.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fondat
-Version: 4.1.4
+Version: 4.1.5
 Summary: A foundation for resource-oriented backend applications.
 Home-page: https://github.com/fondat/fondat/
 License: MIT
 Keywords: asgi,foundation,resource,openapi
 Author: fondat authors
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: aiosqlite (>=0.19,<0.20)
-Requires-Dist: iso8601 (>=1.1,<2.0)
+Requires-Dist: iso8601 (>=2.0,<3.0)
 Requires-Dist: multidict (>=6.0,<7.0)
 Requires-Dist: wrapt (>=1.15,<2.0)
 Project-URL: Documentation, https://github.com/fondat/fondat/tree/main/docs
 Description-Content-Type: text/markdown
 
 # fondat
```

