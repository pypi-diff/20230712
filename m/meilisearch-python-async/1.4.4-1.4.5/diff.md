# Comparing `tmp/meilisearch_python_async-1.4.4.tar.gz` & `tmp/meilisearch_python_async-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.4.4.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.4.5.tar", max compression
```

## Comparing `meilisearch_python_async-1.4.4.tar` & `meilisearch_python_async-1.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-07-02 20:09:22.080430 meilisearch_python_async-1.4.4/LICENSE
--rw-r--r--   0        0        0     5759 2023-07-02 20:09:22.080430 meilisearch_python_async-1.4.4/README.md
--rw-r--r--   0        0        0      151 2023-07-02 20:09:22.080430 meilisearch_python_async-1.4.4/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2759 2023-07-02 20:09:22.080430 meilisearch_python_async-1.4.4/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0     1441 2023-07-02 20:09:22.080430 meilisearch_python_async-1.4.4/meilisearch_python_async/_utils.py
--rw-r--r--   0        0        0       18 2023-07-02 20:09:22.080430 meilisearch_python_async-1.4.4/meilisearch_python_async/_version.py
--rw-r--r--   0        0        0    23120 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     2085 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    89322 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     4223 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0     1847 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1334 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0     3114 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    11932 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2243 2023-07-02 20:09:22.084430 meilisearch_python_async-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/LICENSE
+-rw-r--r--   0        0        0     5759 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/README.md
+-rw-r--r--   0        0        0      151 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2759 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0     1486 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/_utils.py
+-rw-r--r--   0        0        0       18 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/_version.py
+-rw-r--r--   0        0        0    22970 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     2085 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    89322 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     4223 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0     1847 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1334 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0     3114 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11932 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2243 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.5/PKG-INFO
```

### Comparing `meilisearch_python_async-1.4.4/LICENSE` & `meilisearch_python_async-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/README.md` & `meilisearch_python_async-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/_utils.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,10 +33,12 @@
     if isinstance(iso_date, datetime):
         return iso_date
 
     try:
         return datetime.strptime(iso_date, "%Y-%m-%dT%H:%M:%S.%fZ")
     except ValueError:
         split = iso_date.split(".")
+        if len(split) < 2:
+            raise
         reduce = len(split[1]) - 6
         reduced = f"{split[0]}.{split[1][:-reduce]}Z"
         return datetime.strptime(reduced, "%Y-%m-%dT%H:%M:%S.%fZ")
```

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/client.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,16 +383,14 @@
             >>>     key_info = KeyCreate(
             >>>         description="My new key",
             >>>         actions=["search"],
             >>>         indexes=["movies"],
             >>>     )
             >>>     keys = await client.create_key(key_info)
         """
-        # The json.loads(key.json()) is because Pydantic can't serialize a date in a Python dict,
-        # but can when converting to a json string.
         if is_pydantic_2():
             response = await self._http_requests.post("keys", json.loads(key.model_dump_json(by_alias=True)))  # type: ignore[attr-defined]
         else:  # pragma: no cover
             response = await self._http_requests.post("keys", json.loads(key.json(by_alias=True)))  # type: ignore[attr-defined]
 
         return Key(**response.json())
```

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/index.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/models/index.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/models/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/models/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/models/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/meilisearch_python_async/task.py` & `meilisearch_python_async-1.4.5/meilisearch_python_async/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.4/pyproject.toml` & `meilisearch_python_async-1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.4.4"
+version = "1.4.5"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
```

### Comparing `meilisearch_python_async-1.4.4/PKG-INFO` & `meilisearch_python_async-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.4.4
+Version: 1.4.5
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
```

