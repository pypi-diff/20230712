# Comparing `tmp/shrt-0.1.9.tar.gz` & `tmp/shrt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrt-0.1.9.tar", max compression
+gzip compressed data, was "shrt-0.2.0.tar", max compression
```

## Comparing `shrt-0.1.9.tar` & `shrt-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1087 2022-08-15 04:46:01.511863 shrt-0.1.9/LICENSE
--rw-r--r--   0        0        0      506 2022-08-15 04:46:01.511863 shrt-0.1.9/README.md
--rw-r--r--   0        0        0      846 2022-08-15 04:46:50.484136 shrt-0.1.9/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/__init__.py
--rw-r--r--   0        0        0       33 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/__main__.py
--rw-r--r--   0        0        0      178 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/app.py
--rw-r--r--   0        0        0        0 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/cli/__init__.py
--rw-r--r--   0        0        0       29 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/cli/__main__.py
--rw-r--r--   0        0        0      187 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/cli/main.py
--rw-r--r--   0        0        0     2645 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/cli/url.py
--rw-r--r--   0        0        0      874 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/database.py
--rw-r--r--   0        0        0      271 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/schemas.py
--rw-r--r--   0        0        0      862 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/settings.py
--rw-r--r--   0        0        0      111 2022-08-15 04:46:01.512863 shrt-0.1.9/shrt/utils/__init__.py
--rw-r--r--   0        0        0     1183 2022-08-15 04:46:01.513863 shrt-0.1.9/shrt/utils/cache.py
--rw-r--r--   0        0        0      191 2022-08-15 04:46:01.513863 shrt-0.1.9/shrt/utils/strings.py
--rw-r--r--   0        0        0        0 2022-08-15 04:46:01.513863 shrt-0.1.9/shrt/views/__init__.py
--rw-r--r--   0        0        0     1011 2022-08-15 04:46:01.513863 shrt-0.1.9/shrt/views/redirect.py
--rw-r--r--   0        0        0      113 2022-08-15 04:46:01.513863 shrt-0.1.9/shrt/views/status.py
--rw-r--r--   0        0        0      556 2022-08-15 04:46:01.513863 shrt-0.1.9/shrt/web.py
--rw-r--r--   0        0        0     1560 2022-08-15 04:46:51.160046 shrt-0.1.9/setup.py
--rw-r--r--   0        0        0     1423 2022-08-15 04:46:51.160413 shrt-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-12 13:24:41.452965 shrt-0.2.0/LICENSE
+-rw-r--r--   0        0        0      554 2023-07-12 13:24:41.452965 shrt-0.2.0/README.md
+-rw-r--r--   0        0        0      851 2023-07-12 13:24:55.988951 shrt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 13:24:41.475965 shrt-0.2.0/shrt/__init__.py
+-rw-r--r--   0        0        0       33 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/__main__.py
+-rw-r--r--   0        0        0      178 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/app.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:24:41.475965 shrt-0.2.0/shrt/cli/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/cli/__main__.py
+-rw-r--r--   0        0        0      187 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/cli/main.py
+-rw-r--r--   0        0        0     3042 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/cli/url.py
+-rw-r--r--   0        0        0      874 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/database.py
+-rw-r--r--   0        0        0      271 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/schemas.py
+-rw-r--r--   0        0        0      862 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/settings.py
+-rw-r--r--   0        0        0      133 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/utils/__init__.py
+-rw-r--r--   0        0        0     1414 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/utils/cache.py
+-rw-r--r--   0        0        0      191 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/utils/strings.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:24:41.476965 shrt-0.2.0/shrt/views/__init__.py
+-rw-r--r--   0        0        0     1011 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/views/redirect.py
+-rw-r--r--   0        0        0      113 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/views/status.py
+-rw-r--r--   0        0        0      634 2023-07-12 13:24:41.453965 shrt-0.2.0/shrt/web.py
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 shrt-0.2.0/PKG-INFO
```

### Comparing `shrt-0.1.9/LICENSE` & `shrt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shrt-0.1.9/pyproject.toml` & `shrt-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "shrt"
-version = "0.1.9"
+version = "0.2.0"
 description = "Shorten URLs"
 authors = ["Yehuda Deutsch <yeh@uda.co.il>"]
 maintainers = ["Yehuda Deutsch <yeh@uda.co.il>"]
 readme = "README.md"
 repository = "https://gitlab.com/uda/shrt"
 license = "MIT"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://gitlab.com/uda/shrt/-/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fastapi = { extras = ["all"], version = "^0.79.0" }
-typer = "^0.6.1"
+fastapi = { extras = ["all"], version = "^0.99.0" }
+typer = "^0.9.0"
 fastapi-jinja = "^0.2.0"
 SQLAlchemy = "^1.4.40"
-databases = { extras = ["aiosqlite"], version = "^0.6.0" }
-tabulate = "^0.8.10"
-redis = {version = "^4.3.4", optional = true}
-
-[tool.poetry.dev-dependencies]
-dunamai = "^1.12.0"
+databases = { extras = ["aiosqlite"], version = "^0.7.0" }
+tabulate = "^0.9.0"
+redis = {version = "^4.6.0", optional = true}
 
 [tool.poetry.extras]
 cache = ["redis"]
 
 [tool.poetry.scripts]
 shrt = 'shrt.cli.main:cli'
 
+[tool.poetry.group.dev.dependencies]
+dunamai = "^1.17.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shrt-0.1.9/shrt/cli/url.py` & `shrt-0.2.0/shrt/cli/url.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,11 +67,21 @@
 
 
 @app.command(name='get')
 def cmd_get(path: str):
     with database.engine.connect() as conn:
         result = conn.execute(redirects.select().where(redirects.c.path == path)).fetchone()
         if not result:
-            typer.echo('No URL found', err=True)
+            typer.echo(f'No URL found for path "{path}"', err=True)
             raise typer.Exit(code=1)
         result = {k: getattr(result, k) for k in redirects.c.keys()}
         typer.echo(tabulate([result], headers='keys'))
+
+
+@app.command(name='delete')
+def cmd_delete(path: str):
+    with database.engine.connect() as conn:
+        result = conn.execute(redirects.delete().where(redirects.c.path == path))
+        if not result.rowcount:
+            typer.echo(f'No URL found for path "{path}"', err=True)
+            raise typer.Exit(code=1)
+        typer.echo(f'Deleted redirect for path "{path}"')
```

### Comparing `shrt-0.1.9/shrt/database.py` & `shrt-0.2.0/shrt/database.py`

 * *Files identical despite different names*

### Comparing `shrt-0.1.9/shrt/settings.py` & `shrt-0.2.0/shrt/settings.py`

 * *Files identical despite different names*

### Comparing `shrt-0.1.9/shrt/utils/cache.py` & `shrt-0.2.0/shrt/utils/cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,36 +2,47 @@
 Assuming here we are using Redis
 Assuming connection pool is initiated by the server
 """
 import asyncio
 
 from pydantic import RedisDsn
 try:
-    from redis import asyncio as aioredis
+    from redis.asyncio import ConnectionPool, Redis
     redis_installed = True
 except ImportError:
     redis_installed = False
+    ConnectionPool, Redis = None, None
 
 MAX_CLIENTS = 10000
 
-redis_pool: aioredis.ConnectionPool = None
-redis_conn: aioredis.Redis = None
+redis_pool: ConnectionPool = None
+redis_conn: Redis = None
 
 # Allow some space for rogue connections, so we don't fail desired connections
 _redis_semaphore = asyncio.Semaphore(int(MAX_CLIENTS * 0.9))
 
 
 def redis_init(url: str | RedisDsn):
     if not redis_installed:
         return None
     global redis_pool, redis_conn
     if not redis_pool:
-        redis_pool = aioredis.ConnectionPool.from_url(url, max_connections=MAX_CLIENTS)
+        redis_pool = ConnectionPool.from_url(url, max_connections=MAX_CLIENTS)
     if not redis_conn:
-        redis_conn = aioredis.Redis(connection_pool=redis_pool)
+        redis_conn = Redis(connection_pool=redis_pool)
+
+
+async def redis_disconnect():
+    if not redis_installed:
+        return None
+    global redis_pool, redis_conn
+    if redis_conn:
+        await redis_conn.close()
+        redis_conn = None
+        redis_pool = None
 
 
 async def get_cache(key: str) -> str | None:
     if not redis_installed:
         return None
     async with _redis_semaphore:
         return await redis_conn.get(key)
```

### Comparing `shrt-0.1.9/shrt/views/redirect.py` & `shrt-0.2.0/shrt/views/redirect.py`

 * *Files identical despite different names*

### Comparing `shrt-0.1.9/shrt/web.py` & `shrt-0.2.0/shrt/web.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .app import app, settings
 from .database import database, init_engine
-from .utils import redis_init
+from .utils import redis_init, redis_disconnect
 from .views import status, redirect
 
 app.include_router(status.router, prefix='/status', include_in_schema=False)
 app.include_router(redirect.router, prefix='', tags=['redirect'], include_in_schema=True)
 
 
 @app.on_event("startup")
@@ -14,7 +14,9 @@
     if settings.use_cache:
         redis_init(url=settings.redis_url)
 
 
 @app.on_event("shutdown")
 async def shutdown():
     await database.disconnect()
+    if settings.use_cache:
+        await redis_disconnect()
```

### Comparing `shrt-0.1.9/PKG-INFO` & `shrt-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: shrt
-Version: 0.1.9
+Version: 0.2.0
 Summary: Shorten URLs
 Home-page: https://gitlab.com/uda/shrt
 License: MIT
 Author: Yehuda Deutsch
 Author-email: yeh@uda.co.il
 Maintainer: Yehuda Deutsch
 Maintainer-email: yeh@uda.co.il
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cache
 Requires-Dist: SQLAlchemy (>=1.4.40,<2.0.0)
-Requires-Dist: databases[aiosqlite] (>=0.6.0,<0.7.0)
+Requires-Dist: databases[aiosqlite] (>=0.7.0,<0.8.0)
 Requires-Dist: fastapi-jinja (>=0.2.0,<0.3.0)
-Requires-Dist: fastapi[all] (>=0.79.0,<0.80.0)
-Requires-Dist: redis (>=4.3.4,<5.0.0); extra == "cache"
-Requires-Dist: tabulate (>=0.8.10,<0.9.0)
-Requires-Dist: typer (>=0.6.1,<0.7.0)
+Requires-Dist: fastapi[all] (>=0.99.0,<0.100.0)
+Requires-Dist: redis (>=4.6.0,<5.0.0) ; extra == "cache"
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://gitlab.com/uda/shrt/-/issues
 Project-URL: Repository, https://gitlab.com/uda/shrt
 Description-Content-Type: text/markdown
 
 # SHRT - Shortened URL service
 
 An MVP to serve shortened URLs
@@ -45,9 +46,11 @@
 shrt url add https://x59.us
 # Create a custom short path
 shrt url add https://x59.co --path x59
 # Create a new short path, even if the target exists in the DB
 shrt url add https://x59.co --create-new
 # Get details for a given short path
 shrt url get x59
+# Delete a given short path
+shrt url delete x59
 ```
```

