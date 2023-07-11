# Comparing `tmp/fondat-4.1.5.tar.gz` & `tmp/fondat-4.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat-4.1.5.tar", max compression
+gzip compressed data, was "fondat-4.1.6.tar", max compression
```

## Comparing `fondat-4.1.5.tar` & `fondat-4.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.5/LICENSE
--rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.5/README.md
--rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.5/fondat/annotation.py
--rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.5/fondat/asgi.py
--rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.5/fondat/cache.py
--rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.5/fondat/codec.py
--rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.5/fondat/context.py
--rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.5/fondat/csv.py
--rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.5/fondat/data.py
--rw-r--r--   0        0        0     2444 2023-07-11 20:44:25.310120 fondat-4.1.5/fondat/error.py
--rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.5/fondat/file.py
--rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.5/fondat/http.py
--rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.5/fondat/lazy.py
--rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.5/fondat/memory.py
--rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.5/fondat/monitor.py
--rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.5/fondat/oauth.py
--rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.5/fondat/openapi.py
--rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.5/fondat/pagination.py
--rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.5/fondat/patch.py
--rw-r--r--   0        0        0    11552 2023-07-11 21:43:50.415822 fondat-4.1.5/fondat/resource.py
--rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.5/fondat/security.py
--rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.5/fondat/sql.py
--rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.5/fondat/sqlite.py
--rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.5/fondat/stream.py
--rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.5/fondat/string.py
--rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.5/fondat/types.py
--rw-r--r--   0        0        0    12794 2023-07-11 22:04:46.524331 fondat-4.1.5/fondat/validation.py
--rw-r--r--   0        0        0     1171 2023-07-11 22:13:45.993901 fondat-4.1.5/pyproject.toml
--rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 fondat-4.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.6/LICENSE
+-rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.6/README.md
+-rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.6/fondat/annotation.py
+-rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.6/fondat/asgi.py
+-rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.6/fondat/cache.py
+-rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.6/fondat/codec.py
+-rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.6/fondat/context.py
+-rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.6/fondat/csv.py
+-rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.6/fondat/data.py
+-rw-r--r--   0        0        0     2444 2023-07-11 20:44:25.310120 fondat-4.1.6/fondat/error.py
+-rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.6/fondat/file.py
+-rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.6/fondat/http.py
+-rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.6/fondat/lazy.py
+-rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.6/fondat/memory.py
+-rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.6/fondat/monitor.py
+-rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.6/fondat/oauth.py
+-rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.6/fondat/openapi.py
+-rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.6/fondat/pagination.py
+-rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.6/fondat/patch.py
+-rw-r--r--   0        0        0    11552 2023-07-11 21:43:50.415822 fondat-4.1.6/fondat/resource.py
+-rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.6/fondat/security.py
+-rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.6/fondat/sql.py
+-rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.6/fondat/sqlite.py
+-rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.6/fondat/stream.py
+-rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.6/fondat/string.py
+-rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.6/fondat/types.py
+-rw-r--r--   0        0        0    12790 2023-07-11 23:03:40.591314 fondat-4.1.6/fondat/validation.py
+-rw-r--r--   0        0        0     1171 2023-07-11 23:06:54.328556 fondat-4.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 fondat-4.1.6/PKG-INFO
```

### Comparing `fondat-4.1.5/LICENSE` & `fondat-4.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/README.md` & `fondat-4.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/annotation.py` & `fondat-4.1.6/fondat/annotation.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/asgi.py` & `fondat-4.1.6/fondat/asgi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/cache.py` & `fondat-4.1.6/fondat/cache.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/codec.py` & `fondat-4.1.6/fondat/codec.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/context.py` & `fondat-4.1.6/fondat/context.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/csv.py` & `fondat-4.1.6/fondat/csv.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/data.py` & `fondat-4.1.6/fondat/data.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/error.py` & `fondat-4.1.6/fondat/error.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/file.py` & `fondat-4.1.6/fondat/file.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/http.py` & `fondat-4.1.6/fondat/http.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/lazy.py` & `fondat-4.1.6/fondat/lazy.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/memory.py` & `fondat-4.1.6/fondat/memory.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/monitor.py` & `fondat-4.1.6/fondat/monitor.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/oauth.py` & `fondat-4.1.6/fondat/oauth.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/openapi.py` & `fondat-4.1.6/fondat/openapi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/pagination.py` & `fondat-4.1.6/fondat/pagination.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/patch.py` & `fondat-4.1.6/fondat/patch.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/resource.py` & `fondat-4.1.6/fondat/resource.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/security.py` & `fondat-4.1.6/fondat/security.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/sql.py` & `fondat-4.1.6/fondat/sql.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/sqlite.py` & `fondat-4.1.6/fondat/sqlite.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/stream.py` & `fondat-4.1.6/fondat/stream.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/string.py` & `fondat-4.1.6/fondat/string.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/types.py` & `fondat-4.1.6/fondat/types.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.5/fondat/validation.py` & `fondat-4.1.6/fondat/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import typing
 import wrapt
 
 from collections.abc import Callable, Iterable, Mapping
 from contextlib import contextmanager
 from fondat.types import is_instance, is_subclass, split_annotations
 from types import NoneType
-from typing import Any, TypeVar
+from typing import Any, Self, TypeVar
 
 
 class ValidationError(ValueError):
     """
     Error raised when a validation fails.
 
     Parameters:
@@ -87,38 +87,38 @@
         return bool(self.errors)
 
     def __iter__(self):
         return iter(self.errors)
 
     @classmethod
     @contextmanager
-    def collect(cls) -> Iterable["ValidationErrors"]:
+    def collect(cls) -> Self:
         """
-        Establish a context around a new ValidationErrors exception. Upon exit of the context,
-        if the ValidationErrors exception contains any ValidationError exceptions, the new
-        ValidationErrors exception will be raised.
+        Establish a context around a new ValidationErrors exception object. Upon exit of the
+        context, if the ValidationErrors exception object contains any ValidationError
+        exceptions, the new ValidationErrors exception object will be raised.
         """
-        validation_errors = ValidationErrors()
+        validation_errors = cls()
         yield validation_errors
         if validation_errors.errors:
             raise validation_errors
 
     @contextmanager
     def catch(self) -> Iterable[None]:
         """
         Establish a context to catch a ValidationError exception and add it to the
-        ValidationErrors exception. If an error is caught, it will be suppressed and execution
-        will continue outside of the context.
+        ValidationErrors exception object. If an error is caught, it will be suppressed, and
+        execution will continue outside of the context.
         """
         try:
             yield
         except ValidationError as ve:
             self.add(ve)
 
-    def add(self, error: "ValidationError") -> None:
+    def add(self, error: ValidationError) -> None:
         """Add a ValidationError exception to the ValidationErrors exception."""
         self.errors.append(error)
 
 
 class Validator:
     """Base class for type annotation that performs validation."""
```

### Comparing `fondat-4.1.5/pyproject.toml` & `fondat-4.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat"
-version = "4.1.5"
+version = "4.1.6"
 description = "A foundation for resource-oriented backend applications."
 readme = "README.md"
 authors = ["fondat authors"]
 homepage = "https://github.com/fondat/fondat/"
 documentation = "https://github.com/fondat/fondat/tree/main/docs"
 license = "MIT"
 keywords = ["asgi", "foundation", "resource", "openapi"]
@@ -22,15 +22,15 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 packages = [
     { include = "fondat" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 aiosqlite = "^0.19"
 iso8601 = "^2.0"
 multidict = "^6.0"
 wrapt = "^1.15"
 
 [tool.poetry.dev-dependencies]
 black = "^23.7"
```

### Comparing `fondat-4.1.5/PKG-INFO` & `fondat-4.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: fondat
-Version: 4.1.5
+Version: 4.1.6
 Summary: A foundation for resource-oriented backend applications.
 Home-page: https://github.com/fondat/fondat/
 License: MIT
 Keywords: asgi,foundation,resource,openapi
 Author: fondat authors
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: aiosqlite (>=0.19,<0.20)
 Requires-Dist: iso8601 (>=2.0,<3.0)
 Requires-Dist: multidict (>=6.0,<7.0)
 Requires-Dist: wrapt (>=1.15,<2.0)
 Project-URL: Documentation, https://github.com/fondat/fondat/tree/main/docs
```

