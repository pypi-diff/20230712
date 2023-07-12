# Comparing `tmp/fastapi-serve-0.0.2.dev4.tar.gz` & `tmp/fastapi-serve-0.0.2.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.2.dev4.tar", last modified: Tue Jul 11 16:57:39 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.2.dev6.tar", last modified: Wed Jul 12 08:15:47 2023, max compression
```

## Comparing `fastapi-serve-0.0.2.dev4.tar` & `fastapi-serve-0.0.2.dev6.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.190368 fastapi-serve-0.0.2.dev4/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 16:57:38.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:39.190368 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 16:57:39.000000 fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:57:39.194368 fastapi-serve-0.0.2.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-11 16:57:34.000000 fastapi-serve-0.0.2.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.600761 fastapi-serve-0.0.2.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 08:15:47.596761 fastapi-serve-0.0.2.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.592761 fastapi-serve-0.0.2.dev6/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.596761 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.596761 fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.596761 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 08:15:47.600761 fastapi-serve-0.0.2.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/setup.py
```

### Comparing `fastapi-serve-0.0.2.dev4/LICENSE` & `fastapi-serve-0.0.2.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev4/PKG-INFO` & `fastapi-serve-0.0.2.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.2.dev4
+Version: 0.0.2.dev6
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev4 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev6 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.2.dev4/README.md` & `fastapi-serve-0.0.2.dev6/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             url='https://api.hubble.jina.ai/v2/executor/getMeta',
             params={'id': name, 'secret': secret},
         ).status_code
         == HTTPStatus.OK
     )
 
 
-def get_uri(id: str, tag: str):
+def get_jinaai_uri(id: str, tag: str):
     import requests
     from hubble import Auth
 
     r = requests.get(
         f"https://apihubble.jina.ai/v2/executor/getMeta?id={id}&tag={tag}",
         headers={"Authorization": f"token {Auth.get_auth_token()}"},
     )
@@ -40,26 +40,25 @@
         print(f'Could not find image with id {id} and tag {tag}')
         return
     _image_name = _json['data']['name']
     _user_name = _json['meta']['owner']['name']
     return f'jinaai+docker://{_user_name}/{_image_name}:{tag}'
 
 
-def get_module_dir(app_str: str, app_dir: str = None) -> Tuple[str, bool]:
+def get_app_dir(app_str: str, app_dir: str = None) -> Tuple[str, bool]:
     sys.path.insert(0, os.getcwd())
 
-    fastapi_app, _module = load_fastapi_app(app_str)
-    _is_websocket = any_websocket_route_in_app(fastapi_app)
-    _module_dir = get_parent_dir(modname=app_str, filename=_module.__file__)
+    _fastapi_app, _module = load_fastapi_app(app_str)
+    _is_websocket = any_websocket_route_in_app(_fastapi_app)
 
     # if app_dir is not None, return it
     if app_dir is not None:
         return app_dir, _is_websocket
-
-    return _module_dir, _is_websocket
+    else:
+        return get_parent_dir(modname=app_str, filename=_module.__file__), _is_websocket
 
 
 def _remove_fastapi_serve(tmpdir: str) -> None:
     _requirements_txt = 'requirements.txt'
     _pyproject_toml = 'pyproject.toml'
 
     # Remove fastapi-serve itself from the requirements list as a fixed version might break things
@@ -229,30 +228,32 @@
     )
     with EnvironmentVarCtxtManager(push_envs):
         gateway_id = HubIO(args).push().get('id')
         return gateway_id + ':' + tag
 
 
 def push_app_to_hubble(
-    module_dir: str,
-    image_name=None,
+    app: str,
+    app_dir: str = None,
+    image_name: str = None,
     tag: str = 'latest',
     requirements: Tuple[str] = None,
     version: str = 'latest',
     platform: str = None,
     verbose: Optional[bool] = False,
     public: Optional[bool] = False,
 ) -> str:
     tmpdir = mkdtemp()
+    app_dir, _ = get_app_dir(app_str=app, app_dir=app_dir)
 
     # Copy appdir to tmpdir
-    copytree(module_dir, tmpdir, dirs_exist_ok=True)
+    copytree(app_dir, tmpdir, dirs_exist_ok=True)
     # Copy fastapi_serve to tmpdir
     copytree(
-        os.path.dirname(__file__),
+        os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
         os.path.join(tmpdir, 'fastapi_serve'),
         dirs_exist_ok=True,
     )
 
     if image_name is None:
         image_name = get_random_name()
     _handle_dependencies(requirements, tmpdir)
```

### Comparing `fastapi-serve-0.0.2.dev4/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import os
 import sys
 import uuid
 from functools import wraps
 from typing import TYPE_CHECKING, Tuple
 
 if TYPE_CHECKING:
     from types import ModuleType
```

### Comparing `fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev4/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
             shared_data.last_reported_time = current_time
 
 
 class MetricsMiddleware:
     def __init__(
         self,
-        app: ASGIApp,
+        app: "ASGIApp",
         duration_counter: Optional["Counter"] = None,
         request_counter: Optional["Counter"] = None,
     ):
         self.app = app
         self.duration_counter = duration_counter
         self.request_counter = request_counter
         # TODO: figure out solution for static assets
@@ -121,15 +121,15 @@
             "/openapi.json",
             "/healthz",
             "/dry_run",
             "/metrics",
             "/favicon.ico",
         ]
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
+    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
         # Not all Scope objs have path key, e.g., lifespan type of scope
         path = scope.get("path")
         if path and path not in self.skip_routes:
             timer = Timer(5)
             shared_data = timer.SharedData(last_reported_time=time.perf_counter())
             send_duration_task = asyncio.create_task(
                 timer.send_duration_periodically(
@@ -150,28 +150,28 @@
                         1, {"route": path, "protocol": scope["type"]}
                     )
         else:
             await self.app(scope, receive, send)
 
 
 class LoggingMiddleware:
-    def __init__(self, app: ASGIApp, logger: "JinaLogger"):
+    def __init__(self, app: "ASGIApp", logger: "JinaLogger"):
         self.app = app
         self.logger = logger
         self.skip_routes = [
             "/docs",
             "/redoc",
             "/openapi.json",
             "/healthz",
             "/dry_run",
             "/metrics",
             "/favicon.ico",
         ]
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
+    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
         # Not all Scope objs have path key, e.g., lifespan type of scope
         path = scope.get("path")
         if path and path not in self.skip_routes:
             # Get IP address, use X-Forwarded-For if set else use scope['client'][0]
             ip_address = scope.get("client")[0] if scope.get("client") else None
             if scope.get("headers"):
                 for header in scope["headers"]:
```

### Comparing `fastapi-serve-0.0.2.dev4/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.2.dev4
+Version: 0.0.2.dev6
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev4 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev6 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.2.dev4/setup.py` & `fastapi-serve-0.0.2.dev6/setup.py`

 * *Files identical despite different names*

