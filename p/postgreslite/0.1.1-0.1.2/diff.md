# Comparing `tmp/postgreslite-0.1.1.tar.gz` & `tmp/postgreslite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgreslite-0.1.1.tar", last modified: Tue Jul 11 23:39:43 2023, max compression
+gzip compressed data, was "postgreslite-0.1.2.tar", last modified: Wed Jul 12 00:25:24 2023, max compression
```

## Comparing `postgreslite-0.1.1.tar` & `postgreslite-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 23:39:43.504574 postgreslite-0.1.1/
--rw-rw-rw-   0        0        0     1090 2023-01-16 21:45:48.000000 postgreslite-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      179 2023-07-11 23:39:43.503569 postgreslite-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-01-16 21:45:48.000000 postgreslite-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 23:39:43.493889 postgreslite-0.1.1/postgreslite/
--rw-rw-rw-   0        0        0       86 2023-07-11 23:39:31.000000 postgreslite-0.1.1/postgreslite/__init__.py
--rw-rw-rw-   0        0        0     3002 2023-07-11 23:36:23.000000 postgreslite-0.1.1/postgreslite/handler.py
--rw-rw-rw-   0        0        0     4294 2023-07-11 23:39:01.000000 postgreslite-0.1.1/postgreslite/pool.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:39:43.502505 postgreslite-0.1.1/postgreslite.egg-info/
--rw-rw-rw-   0        0        0      179 2023-07-11 23:39:43.000000 postgreslite-0.1.1/postgreslite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-11 23:39:43.000000 postgreslite-0.1.1/postgreslite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 23:39:43.000000 postgreslite-0.1.1/postgreslite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-11 23:39:43.000000 postgreslite-0.1.1/postgreslite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 23:39:43.505081 postgreslite-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      446 2023-01-16 21:45:48.000000 postgreslite-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 00:25:24.265074 postgreslite-0.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-01-16 21:45:48.000000 postgreslite-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-07-12 00:25:24.263563 postgreslite-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-01-16 21:45:48.000000 postgreslite-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 00:25:24.242278 postgreslite-0.1.2/postgreslite/
+-rw-rw-rw-   0        0        0       86 2023-07-12 00:25:11.000000 postgreslite-0.1.2/postgreslite/__init__.py
+-rw-rw-rw-   0        0        0     3002 2023-07-11 23:36:23.000000 postgreslite-0.1.2/postgreslite/handler.py
+-rw-rw-rw-   0        0        0     4290 2023-07-12 00:25:04.000000 postgreslite-0.1.2/postgreslite/pool.py
+drwxrwxrwx   0        0        0        0 2023-07-12 00:25:24.262563 postgreslite-0.1.2/postgreslite.egg-info/
+-rw-rw-rw-   0        0        0      179 2023-07-12 00:25:24.000000 postgreslite-0.1.2/postgreslite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-12 00:25:24.000000 postgreslite-0.1.2/postgreslite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 00:25:24.000000 postgreslite-0.1.2/postgreslite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 00:25:24.000000 postgreslite-0.1.2/postgreslite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 00:25:24.265074 postgreslite-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      446 2023-01-16 21:45:48.000000 postgreslite-0.1.2/setup.py
```

### Comparing `postgreslite-0.1.1/LICENSE` & `postgreslite-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postgreslite-0.1.1/postgreslite/handler.py` & `postgreslite-0.1.2/postgreslite/handler.py`

 * *Files identical despite different names*

### Comparing `postgreslite-0.1.1/postgreslite/pool.py` & `postgreslite-0.1.2/postgreslite/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
         self._args = args
 
     @property
     def prepared(self) -> tuple:
         """ Prepare statements for SQLite with *args provided from earlier """
         arg_len = len(self._args)
 
-        print(self._args)
-
         if arg_len <= 0:
             return ()
         return self._args
 
 
 class PoolConnection:
     def __init__(
@@ -73,15 +71,15 @@
 
     async def _queue_manager(self):
         while True:
             query, args, future = await self._queue.get()
             try:
                 await self._background_task(query, *args, future=future)
             except Exception as e:
-                print(e)
+                print(f"PostgresLite error: {e}")
             self._queue.task_done()
 
     async def _background_task(self, query: str, *args: Any, future: asyncio.Future) -> None:
         prep = SQLStatements(*args)
 
         try:
             cursor: sqlite3.Cursor = await self.loop.run_in_executor(
```

