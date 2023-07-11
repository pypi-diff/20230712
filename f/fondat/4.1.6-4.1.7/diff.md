# Comparing `tmp/fondat-4.1.6.tar.gz` & `tmp/fondat-4.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat-4.1.6.tar", max compression
+gzip compressed data, was "fondat-4.1.7.tar", max compression
```

## Comparing `fondat-4.1.6.tar` & `fondat-4.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.6/LICENSE
--rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.6/README.md
--rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.6/fondat/annotation.py
--rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.6/fondat/asgi.py
--rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.6/fondat/cache.py
--rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.6/fondat/codec.py
--rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.6/fondat/context.py
--rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.6/fondat/csv.py
--rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.6/fondat/data.py
--rw-r--r--   0        0        0     2444 2023-07-11 20:44:25.310120 fondat-4.1.6/fondat/error.py
--rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.6/fondat/file.py
--rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.6/fondat/http.py
--rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.6/fondat/lazy.py
--rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.6/fondat/memory.py
--rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.6/fondat/monitor.py
--rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.6/fondat/oauth.py
--rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.6/fondat/openapi.py
--rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.6/fondat/pagination.py
--rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.6/fondat/patch.py
--rw-r--r--   0        0        0    11552 2023-07-11 21:43:50.415822 fondat-4.1.6/fondat/resource.py
--rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.6/fondat/security.py
--rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.6/fondat/sql.py
--rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.6/fondat/sqlite.py
--rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.6/fondat/stream.py
--rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.6/fondat/string.py
--rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.6/fondat/types.py
--rw-r--r--   0        0        0    12790 2023-07-11 23:03:40.591314 fondat-4.1.6/fondat/validation.py
--rw-r--r--   0        0        0     1171 2023-07-11 23:06:54.328556 fondat-4.1.6/pyproject.toml
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 fondat-4.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.7/LICENSE
+-rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.7/README.md
+-rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.7/fondat/annotation.py
+-rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.7/fondat/asgi.py
+-rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.7/fondat/cache.py
+-rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.7/fondat/codec.py
+-rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.7/fondat/context.py
+-rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.7/fondat/csv.py
+-rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.7/fondat/data.py
+-rw-r--r--   0        0        0     2444 2023-07-11 20:44:25.310120 fondat-4.1.7/fondat/error.py
+-rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.7/fondat/file.py
+-rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.7/fondat/http.py
+-rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.7/fondat/lazy.py
+-rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.7/fondat/memory.py
+-rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.7/fondat/monitor.py
+-rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.7/fondat/oauth.py
+-rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.7/fondat/openapi.py
+-rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.7/fondat/pagination.py
+-rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.7/fondat/patch.py
+-rw-r--r--   0        0        0    11552 2023-07-11 21:43:50.415822 fondat-4.1.7/fondat/resource.py
+-rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.7/fondat/security.py
+-rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.7/fondat/sql.py
+-rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.7/fondat/sqlite.py
+-rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.7/fondat/stream.py
+-rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.7/fondat/string.py
+-rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.7/fondat/types.py
+-rw-r--r--   0        0        0    12793 2023-07-11 23:21:08.121362 fondat-4.1.7/fondat/validation.py
+-rw-r--r--   0        0        0     1171 2023-07-11 23:21:44.151545 fondat-4.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 fondat-4.1.7/PKG-INFO
```

### Comparing `fondat-4.1.6/LICENSE` & `fondat-4.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/README.md` & `fondat-4.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/annotation.py` & `fondat-4.1.7/fondat/annotation.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/asgi.py` & `fondat-4.1.7/fondat/asgi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/cache.py` & `fondat-4.1.7/fondat/cache.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/codec.py` & `fondat-4.1.7/fondat/codec.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/context.py` & `fondat-4.1.7/fondat/context.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/csv.py` & `fondat-4.1.7/fondat/csv.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/data.py` & `fondat-4.1.7/fondat/data.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/error.py` & `fondat-4.1.7/fondat/error.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/file.py` & `fondat-4.1.7/fondat/file.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/http.py` & `fondat-4.1.7/fondat/http.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/lazy.py` & `fondat-4.1.7/fondat/lazy.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/memory.py` & `fondat-4.1.7/fondat/memory.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/monitor.py` & `fondat-4.1.7/fondat/monitor.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/oauth.py` & `fondat-4.1.7/fondat/oauth.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/openapi.py` & `fondat-4.1.7/fondat/openapi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/pagination.py` & `fondat-4.1.7/fondat/pagination.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/patch.py` & `fondat-4.1.7/fondat/patch.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/resource.py` & `fondat-4.1.7/fondat/resource.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/security.py` & `fondat-4.1.7/fondat/security.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/sql.py` & `fondat-4.1.7/fondat/sql.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/sqlite.py` & `fondat-4.1.7/fondat/sqlite.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/stream.py` & `fondat-4.1.7/fondat/stream.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/string.py` & `fondat-4.1.7/fondat/string.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/types.py` & `fondat-4.1.7/fondat/types.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.6/fondat/validation.py` & `fondat-4.1.7/fondat/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,23 +87,23 @@
         return bool(self.errors)
 
     def __iter__(self):
         return iter(self.errors)
 
     @classmethod
     @contextmanager
-    def collect(cls) -> Self:
+    def collect(cls) -> Iterable[Self]:
         """
         Establish a context around a new ValidationErrors exception object. Upon exit of the
         context, if the ValidationErrors exception object contains any ValidationError
         exceptions, the new ValidationErrors exception object will be raised.
         """
         validation_errors = cls()
         yield validation_errors
-        if validation_errors.errors:
+        if validation_errors:
             raise validation_errors
 
     @contextmanager
     def catch(self) -> Iterable[None]:
         """
         Establish a context to catch a ValidationError exception and add it to the
         ValidationErrors exception object. If an error is caught, it will be suppressed, and
```

### Comparing `fondat-4.1.6/pyproject.toml` & `fondat-4.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat"
-version = "4.1.6"
+version = "4.1.7"
 description = "A foundation for resource-oriented backend applications."
 readme = "README.md"
 authors = ["fondat authors"]
 homepage = "https://github.com/fondat/fondat/"
 documentation = "https://github.com/fondat/fondat/tree/main/docs"
 license = "MIT"
 keywords = ["asgi", "foundation", "resource", "openapi"]
```

### Comparing `fondat-4.1.6/PKG-INFO` & `fondat-4.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fondat
-Version: 4.1.6
+Version: 4.1.7
 Summary: A foundation for resource-oriented backend applications.
 Home-page: https://github.com/fondat/fondat/
 License: MIT
 Keywords: asgi,foundation,resource,openapi
 Author: fondat authors
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

