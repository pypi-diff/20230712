# Comparing `tmp/postgreslite-0.1.2.tar.gz` & `tmp/postgreslite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgreslite-0.1.2.tar", last modified: Wed Jul 12 00:25:24 2023, max compression
+gzip compressed data, was "postgreslite-0.1.3.tar", last modified: Wed Jul 12 09:44:04 2023, max compression
```

## Comparing `postgreslite-0.1.2.tar` & `postgreslite-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 00:25:24.265074 postgreslite-0.1.2/
--rw-rw-rw-   0        0        0     1090 2023-01-16 21:45:48.000000 postgreslite-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      179 2023-07-12 00:25:24.263563 postgreslite-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-01-16 21:45:48.000000 postgreslite-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 00:25:24.242278 postgreslite-0.1.2/postgreslite/
--rw-rw-rw-   0        0        0       86 2023-07-12 00:25:11.000000 postgreslite-0.1.2/postgreslite/__init__.py
--rw-rw-rw-   0        0        0     3002 2023-07-11 23:36:23.000000 postgreslite-0.1.2/postgreslite/handler.py
--rw-rw-rw-   0        0        0     4290 2023-07-12 00:25:04.000000 postgreslite-0.1.2/postgreslite/pool.py
-drwxrwxrwx   0        0        0        0 2023-07-12 00:25:24.262563 postgreslite-0.1.2/postgreslite.egg-info/
--rw-rw-rw-   0        0        0      179 2023-07-12 00:25:24.000000 postgreslite-0.1.2/postgreslite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-12 00:25:24.000000 postgreslite-0.1.2/postgreslite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 00:25:24.000000 postgreslite-0.1.2/postgreslite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 00:25:24.000000 postgreslite-0.1.2/postgreslite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 00:25:24.265074 postgreslite-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      446 2023-01-16 21:45:48.000000 postgreslite-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:44:04.970401 postgreslite-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2023-01-16 21:45:48.000000 postgreslite-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-07-12 09:44:04.968889 postgreslite-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-01-16 21:45:48.000000 postgreslite-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 09:44:04.963321 postgreslite-0.1.3/postgreslite/
+-rw-rw-rw-   0        0        0       86 2023-07-12 08:32:58.000000 postgreslite-0.1.3/postgreslite/__init__.py
+-rw-rw-rw-   0        0        0     3128 2023-07-12 09:29:37.000000 postgreslite-0.1.3/postgreslite/handler.py
+-rw-rw-rw-   0        0        0     4564 2023-07-12 09:39:01.000000 postgreslite-0.1.3/postgreslite/pool.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:44:04.968889 postgreslite-0.1.3/postgreslite.egg-info/
+-rw-rw-rw-   0        0        0      179 2023-07-12 09:44:04.000000 postgreslite-0.1.3/postgreslite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-12 09:44:04.000000 postgreslite-0.1.3/postgreslite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 09:44:04.000000 postgreslite-0.1.3/postgreslite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 09:44:04.000000 postgreslite-0.1.3/postgreslite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 09:44:04.970401 postgreslite-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      446 2023-01-16 21:45:48.000000 postgreslite-0.1.3/setup.py
```

### Comparing `postgreslite-0.1.2/LICENSE` & `postgreslite-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postgreslite-0.1.2/postgreslite/handler.py` & `postgreslite-0.1.3/postgreslite/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 from datetime import datetime, date
 
 __all__ = (
     "PostgresLite",
 )
 
 
+class CustomCursor(sqlite3.Cursor):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
 def dict_factory(cursor: sqlite3.Cursor, row: list) -> dict:
     """ Convert SQLite3 data to dict """
     d = {}
     for index, col in enumerate(cursor.description):
         d[col[0]] = row[index]
     return d
```

### Comparing `postgreslite-0.1.2/postgreslite/pool.py` & `postgreslite-0.1.3/postgreslite/pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         data = self._pool.execute(query, prep.prepared)
         return data
 
     def execute(self, query: str, *args: Any) -> str:
         """ Execute SQL command with args for 'Prepared Statements' """
         data = self._init_executor(query, *args)
 
-        status_word = query.split(" ")[0].strip().upper()
+        status_word = query.strip().split(" ")[0].upper()
         status_code = data.rowcount if data.rowcount > 0 else 0
         if status_word == "SELECT":
             status_code = len(data.fetchall())
 
         return f"{status_word} {status_code}"
 
     def fetch(self, query: str, *args: Any) -> list:
@@ -68,64 +68,82 @@
 
         self._queue = asyncio.Queue()
         self._task: asyncio.Task = None
 
     async def _queue_manager(self):
         while True:
             query, args, future = await self._queue.get()
+
             try:
                 await self._background_task(query, *args, future=future)
-            except Exception as e:
-                print(f"PostgresLite error: {e}")
+            except Exception:
+                pass
+
             self._queue.task_done()
 
     async def _background_task(self, query: str, *args: Any, future: asyncio.Future) -> None:
         prep = SQLStatements(*args)
 
         try:
             cursor: sqlite3.Cursor = await self.loop.run_in_executor(
                 None,
                 self._pool.execute,
                 query,
                 prep.prepared
             )
+
             future.set_result(cursor)
         except Exception as e:
             future.set_exception(e)
 
     async def _init_executor(self, query: str, *args: Any) -> sqlite3.Cursor:
         """ Initialize SQL executor with args for 'Prepared Statements' """
         future = self.loop.create_future()
         await self._queue.put((query, args, future))
-        return await future
+
+        try:
+            return await future
+        except Exception:
+            raise future.exception()
 
     @property
     def queue_size(self) -> int:
         """ Get the size of the queue """
         return self._queue.qsize()
 
     async def close(self) -> None:
         """ Close the connection """
         await self._queue.join()
         self._task.cancel()
         self._pool.close()
 
     async def execute(self, query: str, *args: Any) -> str:
         """ Execute SQL command with args for 'Prepared Statements' """
-        data = await self._init_executor(query, *args)
+        try:
+            data = await self._init_executor(query, *args)
+        except Exception as e:
+            raise e
 
-        status_word = query.split(" ")[0].strip().upper()
+        status_word = query.strip().split(" ")[0].upper()
         status_code = data.rowcount if data.rowcount > 0 else 0
         if status_word == "SELECT":
             status_code = len(data.fetchall())
 
         return f"{status_word} {status_code}"
 
     async def fetch(self, query: str, *args: Any) -> list:
         """ Fetch DB data with args for 'Prepared Statements' """
-        data = await self._init_executor(query, *args)
+        try:
+            data = await self._init_executor(query, *args)
+        except Exception as e:
+            raise e
+
         return data.fetchall()
 
     async def fetchrow(self, query: str, *args: Any) -> dict:
         """ Fetch DB row (one row only) with args for 'Prepared Statements' """
-        data = await self._init_executor(query, *args)
+        try:
+            data = await self._init_executor(query, *args)
+        except Exception as e:
+            raise e
+
         return data.fetchone()
```

