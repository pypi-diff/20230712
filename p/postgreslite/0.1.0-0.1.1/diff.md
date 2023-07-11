# Comparing `tmp/postgreslite-0.1.0.tar.gz` & `tmp/postgreslite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgreslite-0.1.0.tar", last modified: Tue Jul 11 23:37:31 2023, max compression
+gzip compressed data, was "postgreslite-0.1.1.tar", last modified: Tue Jul 11 23:39:43 2023, max compression
```

## Comparing `postgreslite-0.1.0.tar` & `postgreslite-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 23:37:31.290347 postgreslite-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-01-16 21:45:48.000000 postgreslite-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      179 2023-07-11 23:37:31.289342 postgreslite-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-01-16 21:45:48.000000 postgreslite-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 23:37:31.274677 postgreslite-0.1.0/postgreslite/
--rw-rw-rw-   0        0        0       86 2023-07-11 23:35:59.000000 postgreslite-0.1.0/postgreslite/__init__.py
--rw-rw-rw-   0        0        0     3002 2023-07-11 23:36:23.000000 postgreslite-0.1.0/postgreslite/handler.py
--rw-rw-rw-   0        0        0     4342 2023-07-11 23:33:33.000000 postgreslite-0.1.0/postgreslite/pool.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:37:31.287827 postgreslite-0.1.0/postgreslite.egg-info/
--rw-rw-rw-   0        0        0      179 2023-07-11 23:37:31.000000 postgreslite-0.1.0/postgreslite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-11 23:37:31.000000 postgreslite-0.1.0/postgreslite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 23:37:31.000000 postgreslite-0.1.0/postgreslite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-11 23:37:31.000000 postgreslite-0.1.0/postgreslite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 23:37:31.290347 postgreslite-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      446 2023-01-16 21:45:48.000000 postgreslite-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:39:43.504574 postgreslite-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-01-16 21:45:48.000000 postgreslite-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-07-11 23:39:43.503569 postgreslite-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-01-16 21:45:48.000000 postgreslite-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 23:39:43.493889 postgreslite-0.1.1/postgreslite/
+-rw-rw-rw-   0        0        0       86 2023-07-11 23:39:31.000000 postgreslite-0.1.1/postgreslite/__init__.py
+-rw-rw-rw-   0        0        0     3002 2023-07-11 23:36:23.000000 postgreslite-0.1.1/postgreslite/handler.py
+-rw-rw-rw-   0        0        0     4294 2023-07-11 23:39:01.000000 postgreslite-0.1.1/postgreslite/pool.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:39:43.502505 postgreslite-0.1.1/postgreslite.egg-info/
+-rw-rw-rw-   0        0        0      179 2023-07-11 23:39:43.000000 postgreslite-0.1.1/postgreslite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-11 23:39:43.000000 postgreslite-0.1.1/postgreslite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 23:39:43.000000 postgreslite-0.1.1/postgreslite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 23:39:43.000000 postgreslite-0.1.1/postgreslite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 23:39:43.505081 postgreslite-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      446 2023-01-16 21:45:48.000000 postgreslite-0.1.1/setup.py
```

### Comparing `postgreslite-0.1.0/LICENSE` & `postgreslite-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `postgreslite-0.1.0/postgreslite/handler.py` & `postgreslite-0.1.1/postgreslite/handler.py`

 * *Files identical despite different names*

### Comparing `postgreslite-0.1.0/postgreslite/pool.py` & `postgreslite-0.1.1/postgreslite/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,40 +29,38 @@
 class PoolConnection:
     def __init__(
         self,
         pool: sqlite3.Connection
     ):
         self._pool = pool
 
-    def _init_executor(self, query: str, arguments: list) -> sqlite3.Cursor:
+    def _init_executor(self, query: str, *args: Any) -> sqlite3.Cursor:
         """ Initialize SQL executor with args for 'Prepared Statements' """
-        prep = SQLStatements(arguments)
+        prep = SQLStatements(*args)
         data = self._pool.execute(query, prep.prepared)
         return data
 
     def execute(self, query: str, *args: Any) -> str:
         """ Execute SQL command with args for 'Prepared Statements' """
-        data = self._init_executor(query, args)
+        data = self._init_executor(query, *args)
 
         status_word = query.split(" ")[0].strip().upper()
         status_code = data.rowcount if data.rowcount > 0 else 0
         if status_word == "SELECT":
             status_code = len(data.fetchall())
 
         return f"{status_word} {status_code}"
 
     def fetch(self, query: str, *args: Any) -> list:
         """ Fetch DB data with args for 'Prepared Statements' """
-        data = self._init_executor(query, args).fetchall()
-        return data
+        return self._init_executor(query, *args).fetchall()
 
     def fetchrow(self, query: str, *args: Any) -> dict:
         """ Fetch DB row (one row only) with args for 'Prepared Statements' """
-        data = self._init_executor(query, args).fetchone()
-        return data
+        return self._init_executor(query, *args).fetchone()
 
 
 class AsyncPoolConnection(PoolConnection):
     def __init__(
         self,
         pool: sqlite3.Connection,
         loop: asyncio.AbstractEventLoop
```

