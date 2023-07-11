# Comparing `tmp/replit-3.3.0.tar.gz` & `tmp/replit-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-3.3.0.tar", max compression
+gzip compressed data, was "replit-3.3.1.tar", max compression
```

## Comparing `replit-3.3.0.tar` & `replit-3.3.1.tar`

### file list

```diff
@@ -1,31 +1,41 @@
--rw-r--r--   0        0        0      720 2023-05-10 13:20:25.042796 replit-3.3.0/LICENSE
--rw-r--r--   0        0        0      673 2023-05-10 13:20:25.042796 replit-3.3.0/README.md
--rw-r--r--   0        0        0     1272 2023-05-11 18:14:08.517808 replit-3.3.0/pyproject.toml
--rw-r--r--   0        0        0      410 2023-05-10 13:20:25.050797 replit-3.3.0/src/replit/__init__.py
--rw-r--r--   0        0        0     2868 2023-05-10 13:20:25.050797 replit-3.3.0/src/replit/__main__.py
--rw-r--r--   0        0        0      171 2023-05-10 13:20:25.050797 replit-3.3.0/src/replit/audio/Makefile
--rw-r--r--   0        0        0    13226 2023-05-10 13:20:25.050797 replit-3.3.0/src/replit/audio/__init__.py
--rw-r--r--   0        0        0     1848 2023-05-10 13:20:25.050797 replit-3.3.0/src/replit/audio/test.py
--rw-r--r--   0        0        0     3687 2023-05-10 13:20:25.050797 replit-3.3.0/src/replit/audio/types.py
--rw-r--r--   0        0        0      426 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/database/__init__.py
--rw-r--r--   0        0        0    18699 2023-05-11 18:11:02.252075 replit-3.3.0/src/replit/database/database.py
--rw-r--r--   0        0        0      822 2023-05-11 18:11:29.114632 replit-3.3.0/src/replit/database/default_db.py
--rw-r--r--   0        0        0     2239 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/database/server.py
--rw-r--r--   0        0        0       33 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/goval/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/goval/api/__init__.py
--rw-r--r--   0        0        0     5198 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/goval/api/client_pb2.py
--rw-r--r--   0        0        0        0 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/goval/api/features/__init__.py
--rw-r--r--   0        0        0     1516 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/goval/api/features/features_pb2.py
--rw-r--r--   0        0        0        0 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/goval/api/repl/__init__.py
--rw-r--r--   0        0        0     3031 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/goval/api/repl/repl_pb2.py
--rw-r--r--   0        0        0     3563 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/goval/api/signing_pb2.py
--rw-r--r--   0        0        0      135 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/identity/__init__.py
--rw-r--r--   0        0        0      159 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/identity/exceptions.py
--rw-r--r--   0        0        0     9156 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/identity/verify.py
--rw-r--r--   0        0        0     2466 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/info.py
--rw-r--r--   0        0        0      352 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/web/__init__.py
--rw-r--r--   0        0        0     2589 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/web/app.py
--rw-r--r--   0        0        0     3329 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/web/user.py
--rw-r--r--   0        0        0     8552 2023-05-10 13:20:25.054797 replit-3.3.0/src/replit/web/utils.py
--rw-r--r--   0        0        0     1843 2023-05-11 18:14:30.144955 replit-3.3.0/setup.py
--rw-r--r--   0        0        0     1611 2023-05-11 18:14:30.145702 replit-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-05-10 13:20:25.042796 replit-3.3.1/LICENSE
+-rw-r--r--   0        0        0      673 2023-05-10 13:20:25.042796 replit-3.3.1/README.md
+-rw-r--r--   0        0        0     1297 2023-07-11 22:21:47.568581 replit-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0      410 2023-05-10 13:20:25.050797 replit-3.3.1/src/replit/__init__.py
+-rw-r--r--   0        0        0     2868 2023-05-10 13:20:25.050797 replit-3.3.1/src/replit/__main__.py
+-rw-r--r--   0        0        0      171 2023-05-10 13:20:25.050797 replit-3.3.1/src/replit/audio/Makefile
+-rw-r--r--   0        0        0    13226 2023-05-10 13:20:25.050797 replit-3.3.1/src/replit/audio/__init__.py
+-rw-r--r--   0        0        0    13821 2023-05-10 14:25:52.899007 replit-3.3.1/src/replit/audio/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2887 2023-05-10 14:25:52.903008 replit-3.3.1/src/replit/audio/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0        0        0     1848 2023-05-10 13:20:25.050797 replit-3.3.1/src/replit/audio/test.py
+-rw-r--r--   0        0        0     3687 2023-05-10 13:20:25.050797 replit-3.3.1/src/replit/audio/types.py
+-rw-r--r--   0        0        0      426 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/database/__init__.py
+-rw-r--r--   0        0        0      538 2023-05-10 14:00:56.919715 replit-3.3.1/src/replit/database/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    21623 2023-07-10 19:25:40.738619 replit-3.3.1/src/replit/database/__pycache__/database.cpython-310.pyc
+-rw-r--r--   0        0        0     1146 2023-07-10 19:18:36.935596 replit-3.3.1/src/replit/database/__pycache__/default_db.cpython-310.pyc
+-rw-r--r--   0        0        0     3270 2023-05-10 14:25:52.891007 replit-3.3.1/src/replit/database/__pycache__/server.cpython-310.pyc
+-rw-r--r--   0        0        0    19297 2023-07-10 19:25:07.682695 replit-3.3.1/src/replit/database/database.py
+-rw-r--r--   0        0        0      912 2023-07-10 12:45:23.845401 replit-3.3.1/src/replit/database/default_db.py
+-rw-r--r--   0        0        0     2239 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/database/server.py
+-rw-r--r--   0        0        0       33 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/goval/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/goval/api/__init__.py
+-rw-r--r--   0        0        0     5198 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/goval/api/client_pb2.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/goval/api/features/__init__.py
+-rw-r--r--   0        0        0     1516 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/goval/api/features/features_pb2.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/goval/api/repl/__init__.py
+-rw-r--r--   0        0        0     3031 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/goval/api/repl/repl_pb2.py
+-rw-r--r--   0        0        0     3563 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/goval/api/signing_pb2.py
+-rw-r--r--   0        0        0      135 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/identity/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/identity/exceptions.py
+-rw-r--r--   0        0        0     9156 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/identity/verify.py
+-rw-r--r--   0        0        0     2466 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/info.py
+-rw-r--r--   0        0        0      352 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/web/__init__.py
+-rw-r--r--   0        0        0      665 2023-05-10 14:00:56.915714 replit-3.3.1/src/replit/web/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3093 2023-05-10 14:00:56.915714 replit-3.3.1/src/replit/web/__pycache__/app.cpython-310.pyc
+-rw-r--r--   0        0        0     4871 2023-05-10 14:25:52.895007 replit-3.3.1/src/replit/web/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     8967 2023-05-10 14:25:52.895007 replit-3.3.1/src/replit/web/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2589 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/web/app.py
+-rw-r--r--   0        0        0     3329 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/web/user.py
+-rw-r--r--   0        0        0     8552 2023-05-10 13:20:25.054797 replit-3.3.1/src/replit/web/utils.py
+-rw-r--r--   0        0        0     1875 2023-07-11 22:23:20.156380 replit-3.3.1/setup.py
+-rw-r--r--   0        0        0     1657 2023-07-11 22:23:20.156691 replit-3.3.1/PKG-INFO
```

### Comparing `replit-3.3.0/LICENSE` & `replit-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/README.md` & `replit-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/pyproject.toml` & `replit-3.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit"
-version = "3.3.0"
+version = "3.3.1"
 description = "A library for interacting with features of repl.it"
 authors = ["Repl.it <contact@repl.it>", "mat <pypi@matdoes.dev>", "kennethreitz <me@kennethreitz.org>", "Scoder12 <pypi@scoder12.ml>", "AllAwesome497", ]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/replit/replit-py"
 homepage = "https://github.com/replit/replit-py"
 documentation = "https://replit-py.readthedocs.org/"
@@ -14,14 +14,15 @@
 typing_extensions = "^3.7.4"
 Flask = "^2.0.0"
 Werkzeug = "^2.0.0"
 aiohttp = "^3.6.2"
 requests = "^2.25.1"
 pyseto = "^1.6.11"
 protobuf = "^4.21.8"
+aiohttp-retry = "^2.8.3"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^3.8.3"
 darglint = "^1.5.2"
 flake8-bandit = "^2.1.2"
 flake8-bugbear = "^20.1.4"
 black = "^19.10b0"
```

### Comparing `replit-3.3.0/src/replit/__main__.py` & `replit-3.3.1/src/replit/__main__.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/audio/__init__.py` & `replit-3.3.1/src/replit/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/audio/test.py` & `replit-3.3.1/src/replit/audio/test.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/audio/types.py` & `replit-3.3.1/src/replit/audio/types.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/database/database.py` & `replit-3.3.1/src/replit/database/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,20 @@
     Iterator,
     List,
     Optional,
     Tuple,
     Union,
 )
 import urllib
-
+import time
+import asyncio
 import aiohttp
 import requests
-
+from requests.adapters import HTTPAdapter, Retry
+from aiohttp_retry import RetryClient, ExponentialRetry
 
 def to_primitive(o: Any) -> Any:
     """If object is an observed object, converts to primitve, otherwise returns it.
 
     Args:
         o (Any): Any object.
 
@@ -58,38 +60,45 @@
 
 _dumps = dumps
 
 
 class AsyncDatabase:
     """Async interface for Repl.it Database."""
 
-    __slots__ = ("db_url", "sess")
+    __slots__ = ("db_url", "sess", "client")
 
-    def __init__(self, db_url: str) -> None:
+    def __init__(self, db_url: str, retry_count: int = 5) -> None:
         """Initialize database. You shouldn't have to do this manually.
 
         Args:
             db_url (str): Database url to use.
         """
         self.db_url = db_url
         self.sess = aiohttp.ClientSession()
 
+        retry_options = ExponentialRetry(attempts=retry_count)
+        self.client = RetryClient(
+            client_session=self.sess,
+            retry_options=retry_options
+        )
+
     def update_db_url(self, db_url: str) -> None:
         """Update the database url.
 
         Args:
             db_url (str): Database url to use.
         """
         self.db_url = db_url
 
     async def __aenter__(self) -> "AsyncDatabase":
         return self
 
     async def __aexit__(self, exc_type: Any, exc_value: Any,
                         traceback: Any) -> None:
+        await self.client.close()
         await self.sess.close()
 
     async def get(self, key: str) -> str:
         """Return the value for key if key is in the database.
 
         This method will JSON decode the value. To disable this behavior, use the
         `get_raw` method instead.
@@ -110,16 +119,15 @@
 
         Raises:
             KeyError: Key is not set
 
         Returns:
             str: The value of the key
         """
-        async with self.sess.get(self.db_url + "/" +
-                                 urllib.parse.quote(key)) as response:
+        async with self.client.get(self.db_url + "/" + urllib.parse.quote(key)) as response:
             if response.status == 404:
                 raise KeyError(key)
             response.raise_for_status()
             return await response.text()
 
     async def set(self, key: str, value: Any) -> None:
         """Set a key in the database to the result of JSON encoding value.
@@ -150,43 +158,41 @@
 
     async def set_bulk_raw(self, values: Dict[str, str]) -> None:
         """Set multiple values in the database.
 
         Args:
             values (Dict[str, str]): The key-value pairs to set.
         """
-        async with self.sess.post(self.db_url, data=values) as response:
+        async with self.client.post(self.db_url, data=values) as response:
             response.raise_for_status()
 
     async def delete(self, key: str) -> None:
         """Delete a key from the database.
 
         Args:
             key (str): The key to delete
 
         Raises:
             KeyError: Key does not exist
         """
-        async with self.sess.delete(self.db_url + "/" +
+        async with self.client.delete(self.db_url + "/" +
                                     urllib.parse.quote(key)) as response:
             if response.status == 404:
                 raise KeyError(key)
             response.raise_for_status()
 
     async def list(self, prefix: str) -> Tuple[str, ...]:
         """List keys in the database which start with prefix.
-
         Args:
             prefix (str): The prefix keys must start with, blank not not check.
-
         Returns:
             Tuple[str]: The keys found.
         """
         params = {"prefix": prefix, "encode": "true"}
-        async with self.sess.get(self.db_url, params=params) as response:
+        async with self.client.get(self.db_url, params=params) as response:
             response.raise_for_status()
             text = await response.text()
             if not text:
                 return tuple()
             else:
                 return tuple(urllib.parse.unquote(k) for k in text.split("\n"))
 
@@ -414,22 +420,25 @@
 
     This interface will coerce all values everything to and from JSON. If you
     don't want this, use AsyncDatabase instead.
     """
 
     __slots__ = ("db_url", "sess")
 
-    def __init__(self, db_url: str) -> None:
+    def __init__(self, db_url: str, retry_count: int = 5) -> None:
         """Initialize database. You shouldn't have to do this manually.
 
         Args:
             db_url (str): Database url to use.
         """
         self.db_url = db_url
         self.sess = requests.Session()
+        retries = Retry(total=retry_count, backoff_factor=0.1, status_forcelist=[500, 502, 503, 504])
+        self.sess.mount("http://", HTTPAdapter(max_retries=retries))
+        self.sess.mount("https://", HTTPAdapter(max_retries=retries))
 
     def update_db_url(self, db_url: str) -> None:
         """Update the database url.
 
         Args:
             db_url (str): Database url to use.
         """
@@ -477,21 +486,18 @@
             Any: The the value for key if key is in the database, else default.
         """
         return super().get(key,
                            item_to_observed(_get_set_cb(self, key), default))
 
     def get_raw(self, key: str) -> str:
         """Look up the given key in the database and return the corresponding value.
-
         Args:
             key (str): The key to look up
-
         Raises:
             KeyError: The key is not in the database.
-
         Returns:
             str: The value of the key in the database.
         """
         r = self.sess.get(self.db_url + "/" + urllib.parse.quote(key))
         if r.status_code == 404:
             raise KeyError(key)
 
@@ -564,19 +570,16 @@
 
     def __len__(self) -> int:
         """The number of keys in the database."""
         return len(self.prefix(""))
 
     def prefix(self, prefix: str) -> Tuple[str, ...]:
         """Return all of the keys in the database that begin with the prefix.
-
         Args:
-            prefix (str): The prefix the keys must start with,
-                blank means anything.
-
+            prefix (str): The prefix the keys must start with, blank means anything.
         Returns:
             Tuple[str]: The keys found.
         """
         r = self.sess.get(f"{self.db_url}",
                           params={
                               "prefix": prefix,
                               "encode": "true"
```

### Comparing `replit-3.3.0/src/replit/database/default_db.py` & `replit-3.3.1/src/replit/database/default_db.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,10 +29,12 @@
 
 db: Optional[Database]
 db_url = get_db_url()
 if db_url:
     db = Database(db_url)
 else:
     # The user will see errors if they try to use the database.
+    print('Warning: error initializing database. Replit DB is not configured.')
     db = None
 
-refresh_db()
+if db:
+    refresh_db()
```

### Comparing `replit-3.3.0/src/replit/database/server.py` & `replit-3.3.1/src/replit/database/server.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/goval/api/client_pb2.py` & `replit-3.3.1/src/replit/goval/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/goval/api/features/features_pb2.py` & `replit-3.3.1/src/replit/goval/api/features/features_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/goval/api/repl/repl_pb2.py` & `replit-3.3.1/src/replit/goval/api/repl/repl_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/goval/api/signing_pb2.py` & `replit-3.3.1/src/replit/goval/api/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/identity/verify.py` & `replit-3.3.1/src/replit/identity/verify.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/info.py` & `replit-3.3.1/src/replit/info.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/web/app.py` & `replit-3.3.1/src/replit/web/app.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/web/user.py` & `replit-3.3.1/src/replit/web/user.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/src/replit/web/utils.py` & `replit-3.3.1/src/replit/web/utils.py`

 * *Files identical despite different names*

### Comparing `replit-3.3.0/setup.py` & `replit-3.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,27 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Flask>=2.0.0,<3.0.0',
  'Werkzeug>=2.0.0,<3.0.0',
+ 'aiohttp-retry>=2.8.3,<3.0.0',
  'aiohttp>=3.6.2,<4.0.0',
  'protobuf>=4.21.8,<5.0.0',
  'pyseto>=1.6.11,<2.0.0',
  'requests>=2.25.1,<3.0.0',
  'typing_extensions>=3.7.4,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['replit = replit.__main__:cli']}
 
 setup_kwargs = {
     'name': 'replit',
-    'version': '3.3.0',
+    'version': '3.3.1',
     'description': 'A library for interacting with features of repl.it',
     'long_description': '### `>>> import replit`\n\n![compute](https://github.com/kennethreitz42/replit-py/blob/kr-cleanup/ext/readme.gif?raw=true)\n\nThis repository is the home for the `replit` Python package, which provides:\n\n- A fully-featured database client for [Replit DB](https://docs.repl.it/misc/database).\n- A Flask–based application framework for accelerating development on the platform.\n- Replit user profile metadata retrieval (more coming here!).\n- A simple audio library that can play tones and audio files!\n\n### Open Source License\n\nThis library is licensed under the [ISC License](https://en.wikipedia.org/wiki/ISC_license) and is free for you to use, change, or even profit from!\n',
     'author': 'Repl.it',
     'author_email': 'contact@repl.it',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/replit/replit-py',
```

### Comparing `replit-3.3.0/PKG-INFO` & `replit-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: replit
-Version: 3.3.0
+Version: 3.3.1
 Summary: A library for interacting with features of repl.it
 Home-page: https://github.com/replit/replit-py
 License: ISC
 Author: Repl.it
 Author-email: contact@repl.it
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask (>=2.0.0,<3.0.0)
 Requires-Dist: Werkzeug (>=2.0.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.6.2,<4.0.0)
+Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0)
 Requires-Dist: protobuf (>=4.21.8,<5.0.0)
 Requires-Dist: pyseto (>=1.6.11,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: typing_extensions (>=3.7.4,<4.0.0)
 Project-URL: Documentation, https://replit-py.readthedocs.org/
 Project-URL: Repository, https://github.com/replit/replit-py
 Description-Content-Type: text/markdown
```

