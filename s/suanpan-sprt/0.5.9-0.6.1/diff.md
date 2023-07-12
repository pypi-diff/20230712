# Comparing `tmp/suanpan-sprt-0.5.9.tar.gz` & `tmp/suanpan-sprt-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.5.9.tar", last modified: Tue Jun 20 09:56:04 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.6.1.tar", last modified: Wed Jul 12 09:43:26 2023, max compression
```

## Comparing `suanpan-sprt-0.5.9.tar` & `suanpan-sprt-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.9/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.9/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.9/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5251 2023-06-20 09:26:42.000000 suanpan-sprt-0.5.9/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.9/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.9/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.9/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5353 2023-06-20 09:26:42.000000 suanpan-sprt-0.5.9/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.9/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-06-20 09:56:03.000000 suanpan-sprt-0.5.9/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.6.1/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.6.1/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.6.1/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4249 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.6.1/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.6.1/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5622 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2082 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.6.1/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6628 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.6.1/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-12 09:25:29.000000 suanpan-sprt-0.6.1/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.5.9/setup.py` & `suanpan-sprt-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.9/sprt/__main__.py` & `suanpan-sprt-0.6.1/sprt/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import sys
 import signal
 import asyncio
 import click
+import pathlib
 from hypercorn.asyncio import serve
 from hypercorn.config import Config
 from logging.config import dictConfig
 from . import server, envs, exceptions
 
 
 @click.command()
 @click.option('-h', '--host', default='localhost', envvar='RT_HOST', help='Runtime host')
-@click.option('-p', '--port', default=9988, envvar='RT_PORT', help='Runtime port')
+@click.option('-p', '--port', default=19900, envvar='RT_PORT', help='Runtime port')
 @click.option('-l', '--log-level', default='debug', envvar='RT_LOG_LEVEL', help='runtime logging level')
 @click.option('-f', '--log-file', default='runtime.log', envvar='RT_LOG_FILE', help='runtime logging file')
 @click.option('--new-log', default=False, envvar='RT_NEW_LOG', help='component with new log')
 @click.option('-w', '--working-dir', default='.', envvar='RT_WORKING_DIR', help='working dir')
 def main(host, port, log_level: str, log_file: str, new_log: bool, working_dir: str):
+    pathlib.Path(log_file).parent.mkdir(parents=True, exist_ok=True)
     if log_level.upper() in ('CRITICAL', 'FATAL', 'ERROR', 'WARN', 'WARNING', 'INFO', 'DEBUG'):
         dictConfig({
             'version': 1,
             'root': {
                 'level': log_level.upper(),
                 'handlers': ['console']
             },
@@ -34,40 +36,27 @@
                     'level': 'DEBUG',
                     'formatter': 'std_out',
                     'class': 'logging.handlers.RotatingFileHandler',
                     'filename': log_file,
                     'encoding': 'utf8',
                     'maxBytes': 10000000,
                     'backupCount': 1,
-                },
-                'logkit': {
-                    'class': 'sprt.log.LogkitHandler',
-                    'level': 'INFO',
-                    'uri': envs.logkitUri,
-                    'namespace': envs.logkitNamespace,
-                    'socketio_path': envs.logkitPath,
-                    'event': envs.logkitEventsAppend
                 }
             },
             'formatters': {
                 'std_out': {
                     'format': '%(asctime)s :: [%(levelname)-8s] %(message)s',
                     # 'datefmt': '%Y-%m-%d %H:%M:%S'
                 },
             },
             'loggers': {
                 'sprt.server': {
                     'level': log_level.upper(),
                     'handlers': ['rotate_file'],
                     'propagate': False
-                },
-                'logkit': {
-                    'level': envs.logkitLogsLevel.upper(),
-                    'handlers': ['console', 'logkit'],
-                    'propagate': False
                 }
             },
         })
 
     signal.signal(signal.SIGTERM, receive_signal)
     signal.signal(signal.SIGINT, receive_signal)
     app = server.create_app(working_dir, log_file, new_log)
@@ -98,36 +87,23 @@
             },
             'handlers': {
                 'console': {
                     'class': 'sprt.log.NodeStreamHandler',
                     'level': 'DEBUG',
                     'formatter': 'std_out',
                     'stream': sys.stdout
-                },
-                'logkit': {
-                    'class': 'sprt.log.LogkitHandler',
-                    'level': 'INFO',
-                    'uri': envs.logkitUri,
-                    'namespace': envs.logkitNamespace,
-                    'socketio_path': envs.logkitPath,
-                    'event': envs.logkitEventsAppend
                 }
             },
             'formatters': {
                 'std_out': {
                     'format': '%(asctime)s :: [%(levelname)-8s] %(message)s',
                     # 'datefmt': '%Y-%m-%d %H:%M:%S'
                 },
             },
             'loggers': {
-                'logkit': {
-                    'level': envs.logkitLogsLevel.upper(),
-                    'handlers': ['console', 'logkit'],
-                    'propagate': False
-                }
             },
         })
 
     try:
         resp = asyncio.run(server.handle_event(event, working_dir=working_dir))
         return resp
     except exceptions.RequestSchemaValidationError as e:
```

### Comparing `suanpan-sprt-0.5.9/sprt/arguments.py` & `suanpan-sprt-0.6.1/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.9/sprt/envs.py` & `suanpan-sprt-0.6.1/sprt/envs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 
-userId = os.environ.get('SP_USER_ID')
-appId = os.environ.get('SP_APP_ID')
+userId = None
+appId = None
 nodeId = None
 
 # Api
 host = os.environ.get('SP_HOST')
 accessSecret = os.environ.get('SP_ACCESS_SECRET')
 userIdHeaderField = os.environ.get('SP_USER_ID_HEADER_FIELD', 'x-sp-user-id')
 userSignatureHeaderField = os.environ.get('SP_USER_SIGNATURE_HEADER_FIELD', 'x-sp-signature')
 userSignVersionHeaderField = os.environ.get('SP_USER_SIGN_VERSION_HEADER_FIELD', 'x-sp-sign-version')
 
-# Logkit
+# Logkit, only for testing
 logkitUri = os.environ.get('SP_LOGKIT_URI', '')
 logkitNamespace = os.environ.get('SP_LOGKIT_NAMESPACE', '/logkit')
 logkitPath = os.environ.get('SP_LOGKIT_PATH', '')
 logkitEventsAppend = os.environ.get('SP_LOGKIT_EVENTS_APPEND', 'append')
 logkitLogsLevel = os.environ.get('SP_LOGKIT_LOGS_LEVEL', 'warning')
 
 # storage
```

### Comparing `suanpan-sprt-0.5.9/sprt/log.py` & `suanpan-sprt-0.6.1/sprt/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime, timezone
 from urllib.parse import urljoin
 from . import master, envs
 
 
 class NodeStreamHandler(logging.StreamHandler):
     def __init__(self, stream=None):
-        super().__init__()
+        super().__init__(stream=stream)
 
     def get_stream(self):
         return sys.stdout
 
     def set_stream(self, _value):
         ...
```

### Comparing `suanpan-sprt-0.5.9/sprt/master.py` & `suanpan-sprt-0.6.1/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.9/sprt/server.py` & `suanpan-sprt-0.6.1/sprt/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,80 +9,108 @@
 from quart import Quart
 from quart_schema import QuartSchema, validate_request, validate_response, RequestSchemaValidationError
 from quart_schema import validation
 from . import loader, envs, exceptions, utils
 
 
 @dataclasses.dataclass
+class LogkitInfo:
+    uri: str
+    path: str
+    namespace: typing.Optional[str] = "/logkit"
+    events_append: typing.Optional[str] = "append"
+    logs_level: typing.Optional[str] = "warning"
+
+
+@dataclasses.dataclass
 class FunctionContext:
     request_id: str
+    user_id: str
+    app_id: str
     node_id: str
     # 右面板参数
     params: typing.Optional[dict]
     # 输入桩参数
     args: dict
 
 
 @dataclasses.dataclass
 class FunctionParams:
     id: str
     file: str
     working_dir: typing.Optional[str]
     context: FunctionContext
+    logkit: LogkitInfo
     function: typing.Optional[str] = "main"
 
 
 @dataclasses.dataclass
 class FunctionResponse:
     id: str
     success: bool
     error: typing.Optional[str] = None
     data: typing.Optional[dict] = None
 
 
-def acquire_resource(node_id):
+@dataclasses.dataclass
+class FunctionReleaseParams:
+    app_id: str
+
+
+@dataclasses.dataclass
+class FunctionReleaseResponse:
+    success: bool
+
+
+def acquire_resource(user_id, app_id, node_id):
+    envs.userId = user_id
+    envs.appId = app_id
     envs.nodeId = node_id
-    return node_id
+    return user_id, app_id, node_id
 
 
 def release_resource(ctx):
+    envs.userId = None
+    envs.appId = None
     envs.nodeId = None
 
 
 @contextmanager
 def node_context(*args, **kwargs):
     resource = acquire_resource(*args, **kwargs)
     try:
         yield resource
     finally:
         release_resource(resource)
 
 
 def create_app(working_dir='.', log_file='', new_log=False):
-    log_path = pathlib.Path(log_file).parent
-    filename = pathlib.Path(log_file).name
-    logfile_prefix = filename.split('-')[0:2]
+    log_path = pathlib.Path(log_file).parent.parent
     app = Quart(__name__)
     QuartSchema(app)
 
     @app.post("/")
     @validate_request(FunctionParams)
     @validate_response(FunctionResponse)
-    async def handle_post(data: FunctionParams) -> FunctionResponse:
+    async def function_invoke(data: FunctionParams) -> FunctionResponse:
+        user_id = data.context.user_id
+        app_id = data.context.app_id
         node_id = data.context.node_id
         if new_log:
-            log_dir = log_path / f'{logfile_prefix[0]}-{logfile_prefix[1]}-{node_id}'
+            log_dir = log_path / f'{app_id}-{user_id}-{node_id}'
             log_dir.mkdir(parents=True, exist_ok=True)
-            log_name = log_dir / f'app-{logfile_prefix[0]}-{node_id}'
+            log_name = log_dir / f'app-{app_id}-{node_id}'
         else:
-            log_name = log_path / node_id
+            log_dir = log_path / app_id
+            log_dir.mkdir(parents=True, exist_ok=True)
+            log_name = log_dir / node_id
         if utils.should_log_rollover(str(log_name)):
             utils.do_log_rollover(str(log_name))
-        with open(log_path / node_id, 'a', encoding='utf8') as f:
-            with redirect_stdout(f), redirect_stderr(f), node_context(node_id):
+        with open(log_name, 'a', encoding='utf8') as f:
+            with redirect_stdout(f), redirect_stderr(f), node_context(user_id, app_id, node_id):
                 function = None
                 try:
                     logging.debug(f'event: {data.context.args}')
                     function = load(data, working_dir)
                     ret = await function.call_func(data.context.request_id, data.context.args, data.context.params)
                     logging.debug(f'response: {ret}')
                     out_data = {key: value for key, value in ret.items() if
@@ -102,14 +130,26 @@
         if isinstance(error.validation_error, TypeError):
             err = str(error.validation_error)
         else:
             err = error.validation_error.json()
 
         return {"errors": err}, 400
 
+    @app.post("/function/release")
+    @validate_request(FunctionReleaseParams)
+    @validate_response(FunctionReleaseResponse)
+    async def function_release(data: FunctionReleaseParams) -> FunctionReleaseResponse:
+        for node_id in list(module_imported):
+            node_function = module_imported[node_id]
+            if node_function.context.app_id == data.app_id:
+                logging.info(f'node {node_id} release')
+                del module_imported[node_id]
+
+        return FunctionReleaseResponse(success=True)
+
     @app.get("/health/liveness")
     async def liveness():
         return "OK"
 
     @app.get("/health/readiness")
     async def readiness():
         return "OK"
@@ -117,25 +157,28 @@
     return app
 
 
 module_imported = {}
 
 
 def load(data: FunctionParams, default_dir):
+    user_id = data.context.user_id
+    app_id = data.context.app_id
     node_id = data.context.node_id
     working_dir = data.working_dir if data.working_dir else default_dir
     filename = data.file
     function = data.function
 
     node_function = module_imported.get(node_id)
     if not node_function:
         logging.info(f'node {node_id} import function {function} from {filename}')
-        node_function = loader.NodeFunction(node_id, working_dir, filename, function)
+        node_function = loader.NodeFunction(user_id, app_id, node_id, working_dir, filename, function)
         module_imported[node_id] = node_function
 
+    node_function.update_logkit(data.logkit)
     return node_function
 
 
 async def handle_event(event_data, working_dir='.'):
     model_class = validation._to_pydantic_model(FunctionParams)
     try:
         json_data = json.loads(event_data)
```

### Comparing `suanpan-sprt-0.5.9/sprt/storage.py` & `suanpan-sprt-0.6.1/sprt/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import abc
 import logging
 import pathlib
 import functools
 import minio
 from . import master, envs, utils
 
-logger = logging.getLogger('logkit')
-
 
 class Storage(abc.ABC):
     CONTENT_MD5 = "Content-MD5"
     _instance = None
 
     def __init__(self, endpoint, bucket, access_id, access_secret, root_path='', temp_store='', global_store=''):
         self.endpoint = endpoint
@@ -136,15 +134,15 @@
     def auto_refresh_token(self, func):
         @functools.wraps(func)
         def _dec(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except minio.error.S3Error as e:
                 if e.code == "AccessDenied":
-                    logger.warning("Minio access denied, refreshing access key.")
+                    logging.warning("Minio access denied, refreshing access key.")
                     self.client = self._connect_client()
                     return func(*args, **kwargs)
                 raise e
 
         return _dec
 
     def download(self, key, path=None, bucket=None):
```

### Comparing `suanpan-sprt-0.5.9/sprt/testing.py` & `suanpan-sprt-0.6.1/sprt/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,40 +31,27 @@
                     'level': 'DEBUG',
                     'formatter': 'std_out',
                     'class': 'logging.handlers.RotatingFileHandler',
                     'filename': 'sprt.server.log',
                     'encoding': 'utf8',
                     'maxBytes': 10000000,
                     'backupCount': 1,
-                },
-                'logkit': {
-                    'class': 'sprt.log.LogkitHandler',
-                    'level': 'INFO',
-                    'uri': envs.logkitUri,
-                    'namespace': envs.logkitNamespace,
-                    'socketio_path': envs.logkitPath,
-                    'event': envs.logkitEventsAppend
                 }
             },
             'formatters': {
                 'std_out': {
                     'format': '%(asctime)s :: [%(levelname)-8s] %(message)s',
                     # 'datefmt': '%Y-%m-%d %H:%M:%S'
                 },
             },
             'loggers': {
                 'sprt.server': {
                     'level': 'DEBUG',
                     'handlers': ['rotate_file'],
                     'propagate': False
-                },
-                'logkit': {
-                    'level': envs.logkitLogsLevel.upper(),
-                    'handlers': ['console', 'logkit'],
-                    'propagate': False
                 }
             },
         })
 
     def set_params(self, **kwargs):
         for key, value in kwargs.items():
             if isinstance(value, str):
@@ -91,13 +78,22 @@
         ret = {
             'id': self.id,
             'file': self.file,
             'working_dir': self.working_dir,
             'function': self.function,
             'context': {
                 'request_id': uuid.uuid4().hex,
+                'user_id': 'test_user',
+                'app_id': 'test_app',
                 'node_id': self.node_id,
                 'params': self.params,
                 'args': _args
+            },
+            'logkit': {
+                'uri': envs.logkitUri,
+                'path': envs.logkitPath,
+                'namespace': envs.logkitNamespace,
+                'events_append': envs.logkitEventsAppend,
+                'logs_level': envs.logkitLogsLevel
             }
         }
         return ret
```

### Comparing `suanpan-sprt-0.5.9/sprt/utils.py` & `suanpan-sprt-0.6.1/sprt/utils.py`

 * *Files identical despite different names*

