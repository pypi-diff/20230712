# Comparing `tmp/duet-0.2.9.dev20230622135328.tar.gz` & `tmp/duet-0.2.9.dev20230712233414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duet-0.2.9.dev20230622135328.tar", last modified: Thu Jun 22 20:53:28 2023, max compression
+gzip compressed data, was "duet-0.2.9.dev20230712233414.tar", last modified: Wed Jul 12 21:34:14 2023, max compression
```

## Comparing `duet-0.2.9.dev20230622135328.tar` & `duet-0.2.9.dev20230712233414.tar`

### file list

```diff
@@ -1,39 +1,29 @@
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-06-22 20:53:28.898888 duet-0.2.9.dev20230622135328/
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-06-22 20:53:28.894888 duet-0.2.9.dev20230622135328/.github/
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-06-22 20:53:28.894888 duet-0.2.9.dev20230622135328/.github/workflows/
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3138 2023-03-02 23:41:07.000000 duet-0.2.9.dev20230622135328/.github/workflows/ci.yml
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1819 2021-10-20 18:54:16.000000 duet-0.2.9.dev20230622135328/.gitignore
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      383 2023-02-27 20:10:50.000000 duet-0.2.9.dev20230622135328/.mypy.ini
--rw-r-----   0 maffoo   (237528) primarygroup (89939)      945 2021-02-10 21:37:09.000000 duet-0.2.9.dev20230622135328/.pylintrc
--rw-r-----   0 maffoo   (237528) primarygroup (89939)      296 2021-02-06 15:18:23.000000 duet-0.2.9.dev20230622135328/AUTHORS
--rw-r-----   0 maffoo   (237528) primarygroup (89939)     1103 2021-02-05 22:48:38.000000 duet-0.2.9.dev20230622135328/CONTRIBUTING.md
--rw-r-----   0 maffoo   (237528) primarygroup (89939)    11357 2021-02-05 22:48:38.000000 duet-0.2.9.dev20230622135328/LICENSE
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)       70 2023-02-27 20:10:50.000000 duet-0.2.9.dev20230622135328/MANIFEST.in
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1974 2023-06-22 20:53:28.898888 duet-0.2.9.dev20230622135328/PKG-INFO
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1496 2021-10-20 18:54:16.000000 duet-0.2.9.dev20230622135328/README.md
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-06-22 20:53:28.894888 duet-0.2.9.dev20230622135328/dev/
--rwxr-x---   0 maffoo   (237528) primarygroup (89939)      688 2021-09-30 08:10:16.000000 duet-0.2.9.dev20230622135328/dev/build
--rwxr-x---   0 maffoo   (237528) primarygroup (89939)       80 2021-02-10 21:37:09.000000 duet-0.2.9.dev20230622135328/dev/check
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)       95 2023-05-25 17:12:37.000000 duet-0.2.9.dev20230622135328/dev/requirements.txt
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-06-22 20:53:28.898888 duet-0.2.9.dev20230622135328/duet/
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2247 2023-05-25 17:12:37.000000 duet-0.2.9.dev20230622135328/duet/__init__.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      608 2023-05-19 23:58:22.000000 duet-0.2.9.dev20230622135328/duet/_version.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3543 2021-10-20 18:54:16.000000 duet-0.2.9.dev20230622135328/duet/aitertools.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)    17205 2023-05-19 23:58:22.000000 duet-0.2.9.dev20230622135328/duet/api.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)    19623 2023-02-27 20:10:50.000000 duet-0.2.9.dev20230622135328/duet/api_test.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     6252 2023-06-22 20:51:07.000000 duet-0.2.9.dev20230622135328/duet/futuretools.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1824 2023-06-22 20:51:07.000000 duet-0.2.9.dev20230622135328/duet/futuretools_test.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)    15991 2023-05-25 17:12:37.000000 duet-0.2.9.dev20230622135328/duet/impl.py
--rw-r-----   0 maffoo   (237528) primarygroup (89939)     2486 2021-02-10 21:37:09.000000 duet-0.2.9.dev20230622135328/duet/impl_test.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)       59 2021-10-20 18:54:16.000000 duet-0.2.9.dev20230622135328/duet/py.typed
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3297 2023-02-27 20:10:50.000000 duet-0.2.9.dev20230622135328/duet/typing.py
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-06-22 20:53:28.898888 duet-0.2.9.dev20230622135328/duet.egg-info/
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1974 2023-06-22 20:53:28.000000 duet-0.2.9.dev20230622135328/duet.egg-info/PKG-INFO
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      527 2023-06-22 20:53:28.000000 duet-0.2.9.dev20230622135328/duet.egg-info/SOURCES.txt
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)        1 2023-06-22 20:53:28.000000 duet-0.2.9.dev20230622135328/duet.egg-info/dependency_links.txt
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      148 2023-06-22 20:53:28.000000 duet-0.2.9.dev20230622135328/duet.egg-info/requires.txt
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)        5 2023-06-22 20:53:28.000000 duet-0.2.9.dev20230622135328/duet.egg-info/top_level.txt
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      247 2023-02-27 20:10:50.000000 duet-0.2.9.dev20230622135328/pyproject.toml
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)       53 2023-05-19 23:58:22.000000 duet-0.2.9.dev20230622135328/requirements.txt
--rw-r-----   0 maffoo   (237528) primarygroup (89939)       73 2023-06-22 20:53:28.898888 duet-0.2.9.dev20230622135328/setup.cfg
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2387 2023-02-27 20:10:50.000000 duet-0.2.9.dev20230622135328/setup.py
+drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-07-12 21:34:14.609426 duet-0.2.9.dev20230712233414/
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)    11357 2022-05-04 07:11:02.000000 duet-0.2.9.dev20230712233414/LICENSE
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)       70 2023-04-08 17:31:34.000000 duet-0.2.9.dev20230712233414/MANIFEST.in
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1994 2023-07-12 21:34:14.609426 duet-0.2.9.dev20230712233414/PKG-INFO
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1496 2022-05-04 07:11:02.000000 duet-0.2.9.dev20230712233414/README.md
+drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-07-12 21:34:14.609426 duet-0.2.9.dev20230712233414/dev/
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)      101 2023-06-23 00:28:45.000000 duet-0.2.9.dev20230712233414/dev/requirements.txt
+drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-07-12 21:34:14.609426 duet-0.2.9.dev20230712233414/duet/
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2247 2023-05-20 03:58:59.000000 duet-0.2.9.dev20230712233414/duet/__init__.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)      608 2023-05-20 03:59:07.000000 duet-0.2.9.dev20230712233414/duet/_version.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3543 2023-07-12 21:33:21.000000 duet-0.2.9.dev20230712233414/duet/aitertools.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)    17205 2023-06-23 00:28:38.000000 duet-0.2.9.dev20230712233414/duet/api.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)    19623 2023-04-08 17:31:34.000000 duet-0.2.9.dev20230712233414/duet/api_test.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     6406 2023-07-12 21:33:31.000000 duet-0.2.9.dev20230712233414/duet/futuretools.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1824 2023-06-23 00:28:45.000000 duet-0.2.9.dev20230712233414/duet/futuretools_test.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)    15991 2023-05-20 03:59:07.000000 duet-0.2.9.dev20230712233414/duet/impl.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2486 2022-05-04 07:11:02.000000 duet-0.2.9.dev20230712233414/duet/impl_test.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)       59 2022-05-04 07:11:02.000000 duet-0.2.9.dev20230712233414/duet/py.typed
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3297 2023-04-08 17:31:34.000000 duet-0.2.9.dev20230712233414/duet/typing.py
+drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-07-12 21:34:14.609426 duet-0.2.9.dev20230712233414/duet.egg-info/
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1994 2023-07-12 21:34:14.000000 duet-0.2.9.dev20230712233414/duet.egg-info/PKG-INFO
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)      427 2023-07-12 21:34:14.000000 duet-0.2.9.dev20230712233414/duet.egg-info/SOURCES.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)        1 2023-07-12 21:34:14.000000 duet-0.2.9.dev20230712233414/duet.egg-info/dependency_links.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)      154 2023-07-12 21:34:14.000000 duet-0.2.9.dev20230712233414/duet.egg-info/requires.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)        5 2023-07-12 21:34:14.000000 duet-0.2.9.dev20230712233414/duet.egg-info/top_level.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)      247 2023-04-08 17:31:34.000000 duet-0.2.9.dev20230712233414/pyproject.toml
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)       53 2023-06-23 00:28:38.000000 duet-0.2.9.dev20230712233414/requirements.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)       73 2023-07-12 21:34:14.613426 duet-0.2.9.dev20230712233414/setup.cfg
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2387 2023-04-08 17:31:34.000000 duet-0.2.9.dev20230712233414/setup.py
```

### Comparing `duet-0.2.9.dev20230622135328/LICENSE` & `duet-0.2.9.dev20230712233414/LICENSE`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/PKG-INFO` & `duet-0.2.9.dev20230712233414/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: duet
-Version: 0.2.9.dev20230622135328
+Version: 0.2.9.dev20230712233414
 Summary: A simple future-based async library for python.
 Home-page: http://github.com/google/duet
 Author: The Duet Authors
 Author-email: maffoo@google.com
 License: Apache 2
+Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev_env
 License-File: LICENSE
 
 This is a development version of Duet and may be unstable.
 
@@ -47,7 +48,9 @@
 ```
 pip install duet
 ```
 
 ## Note
 
 duet is not an official Google project.
+
+
```

### Comparing `duet-0.2.9.dev20230622135328/README.md` & `duet-0.2.9.dev20230712233414/README.md`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet/__init__.py` & `duet-0.2.9.dev20230712233414/duet/__init__.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet/_version.py` & `duet-0.2.9.dev20230712233414/duet/_version.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet/aitertools.py` & `duet-0.2.9.dev20230712233414/duet/aitertools.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet/api.py` & `duet-0.2.9.dev20230712233414/duet/api.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet/api_test.py` & `duet-0.2.9.dev20230712233414/duet/api_test.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet/futuretools.py` & `duet-0.2.9.dev20230712233414/duet/futuretools.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
     def add_done_callback(self, fn: Callable[["FutureLike[T]"], Any]) -> None:
         ...
 
     def cancel(self) -> bool:
         ...
 
+    def cancelled(self) -> bool:
+        ...
+
 
 class AwaitableFuture(Future, Generic[T]):
     """A Future that can be awaited."""
 
     # This is an internal variable in the Future class.
     # We add an annotation here so mypy will let us use it.
     _condition: threading.Condition
@@ -63,19 +66,22 @@
         awaitable = AwaitableFuture[T]()
 
         def cancel(awaitable_future: Future):
             if awaitable_future.cancelled():
                 future.cancel()
 
         def callback(future: FutureLike[T]):
-            error = future.exception()
-            if error is None:
-                awaitable.try_set_result(future.result())
+            if future.cancelled():
+                awaitable.cancel()
             else:
-                awaitable.try_set_exception(error)
+                error = future.exception()
+                if error is None:
+                    awaitable.try_set_result(future.result())
+                else:
+                    awaitable.try_set_exception(error)
 
         awaitable.add_done_callback(cancel)
         future.add_done_callback(callback)
         return awaitable
 
     def __await__(self) -> Generator["AwaitableFuture[T]", None, T]:
         yield self
```

### Comparing `duet-0.2.9.dev20230622135328/duet/futuretools_test.py` & `duet-0.2.9.dev20230712233414/duet/futuretools_test.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet/impl.py` & `duet-0.2.9.dev20230712233414/duet/impl.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet/impl_test.py` & `duet-0.2.9.dev20230712233414/duet/impl_test.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet/typing.py` & `duet-0.2.9.dev20230712233414/duet/typing.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.9.dev20230622135328/duet.egg-info/PKG-INFO` & `duet-0.2.9.dev20230712233414/duet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: duet
-Version: 0.2.9.dev20230622135328
+Version: 0.2.9.dev20230712233414
 Summary: A simple future-based async library for python.
 Home-page: http://github.com/google/duet
 Author: The Duet Authors
 Author-email: maffoo@google.com
 License: Apache 2
+Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev_env
 License-File: LICENSE
 
 This is a development version of Duet and may be unstable.
 
@@ -47,7 +48,9 @@
 ```
 pip install duet
 ```
 
 ## Note
 
 duet is not an official Google project.
+
+
```

### Comparing `duet-0.2.9.dev20230622135328/setup.py` & `duet-0.2.9.dev20230712233414/setup.py`

 * *Files identical despite different names*

