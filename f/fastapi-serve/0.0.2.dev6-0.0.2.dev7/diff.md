# Comparing `tmp/fastapi-serve-0.0.2.dev6.tar.gz` & `tmp/fastapi-serve-0.0.2.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.2.dev6.tar", last modified: Wed Jul 12 08:15:47 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.2.dev7.tar", last modified: Wed Jul 12 14:42:22 2023, max compression
```

## Comparing `fastapi-serve-0.0.2.dev6.tar` & `fastapi-serve-0.0.2.dev7.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.600761 fastapi-serve-0.0.2.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 08:15:47.596761 fastapi-serve-0.0.2.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.592761 fastapi-serve-0.0.2.dev6/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.596761 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.596761 fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:15:47.596761 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 08:15:47.000000 fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 08:15:47.600761 fastapi-serve-0.0.2.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 08:15:42.000000 fastapi-serve-0.0.2.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:42:22.080227 fastapi-serve-0.0.2.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 14:42:22.080227 fastapi-serve-0.0.2.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:42:22.076227 fastapi-serve-0.0.2.dev7/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 14:42:21.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:42:22.076227 fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:42:22.080227 fastapi-serve-0.0.2.dev7/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:42:22.076227 fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 14:42:22.000000 fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-12 14:42:22.000000 fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:42:22.000000 fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 14:42:22.000000 fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:42:22.000000 fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 14:42:22.000000 fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 14:42:22.000000 fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:42:22.080227 fastapi-serve-0.0.2.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 14:42:17.000000 fastapi-serve-0.0.2.dev7/setup.py
```

### Comparing `fastapi-serve-0.0.2.dev6/LICENSE` & `fastapi-serve-0.0.2.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev6/PKG-INFO` & `fastapi-serve-0.0.2.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.2.dev6
+Version: 0.0.2.dev7
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
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev6 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev7 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.2.dev6/README.md` & `fastapi-serve-0.0.2.dev7/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 import requests
 import yaml
 
 from fastapi_serve.cloud.helper import (
     any_websocket_route_in_app,
     get_parent_dir,
-    get_random_name,
     load_fastapi_app,
 )
+from fastapi_serve.helper import get_random_name
 
 
 def hubble_exists(name: str, secret: Optional[str] = None) -> bool:
     return (
         requests.get(
             url='https://api.hubble.jina.ai/v2/executor/getMeta',
             params={'id': name, 'secret': secret},
@@ -40,25 +40,25 @@
         print(f'Could not find image with id {id} and tag {tag}')
         return
     _image_name = _json['data']['name']
     _user_name = _json['meta']['owner']['name']
     return f'jinaai+docker://{_user_name}/{_image_name}:{tag}'
 
 
-def get_app_dir(app_str: str, app_dir: str = None) -> Tuple[str, bool]:
+def get_app_dir(app: str, app_dir: str = None) -> Tuple[str, bool]:
     sys.path.insert(0, os.getcwd())
 
-    _fastapi_app, _module = load_fastapi_app(app_str)
+    _fastapi_app, _module = load_fastapi_app(app)
     _is_websocket = any_websocket_route_in_app(_fastapi_app)
 
     # if app_dir is not None, return it
     if app_dir is not None:
         return app_dir, _is_websocket
     else:
-        return get_parent_dir(modname=app_str, filename=_module.__file__), _is_websocket
+        return get_parent_dir(modname=app, filename=_module.__file__), _is_websocket
 
 
 def _remove_fastapi_serve(tmpdir: str) -> None:
     _requirements_txt = 'requirements.txt'
     _pyproject_toml = 'pyproject.toml'
 
     # Remove fastapi-serve itself from the requirements list as a fixed version might break things
@@ -193,15 +193,15 @@
 
 def _push_to_hubble(
     tmpdir: str, name: str, tag: str, platform: str, verbose: bool, public: bool
 ) -> str:
     from hubble.executor.hubio import HubIO
     from hubble.executor.parsers import set_hub_push_parser
 
-    from fastapi_serve.gateway.helper import EnvironmentVarCtxtManager
+    from fastapi_serve.helper import EnvironmentVarCtxtManager
 
     secret = secrets.token_hex(8)
     args_list = [
         tmpdir,
         '--tag',
         tag,
         '--no-usage',
@@ -239,15 +239,15 @@
     requirements: Tuple[str] = None,
     version: str = 'latest',
     platform: str = None,
     verbose: Optional[bool] = False,
     public: Optional[bool] = False,
 ) -> str:
     tmpdir = mkdtemp()
-    app_dir, _ = get_app_dir(app_str=app, app_dir=app_dir)
+    app_dir, _ = get_app_dir(app=app, app_dir=app_dir)
 
     # Copy appdir to tmpdir
     copytree(app_dir, tmpdir, dirs_exist_ok=True)
     # Copy fastapi_serve to tmpdir
     copytree(
         os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
         os.path.join(tmpdir, 'fastapi_serve'),
```

### Comparing `fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,32 @@
 from fastapi_serve.cloud.errors import (
     InvalidAutoscaleMaxError,
     InvalidAutoscaleMinError,
     InvalidDiskSizeError,
     InvalidInstanceError,
 )
 
+# jcloud args
 INSTANCE = 'instance'
 AUTOSCALE_MIN = 'autoscale_min'
 AUTOSCALE_MAX = 'autoscale_max'
 DISK_SIZE = 'disk_size'
+
+# config file
 JCloudConfigFile = 'jcloud_config.yml'
+
+# default values
 DEFAULT_TIMEOUT = 120
 DEFAULT_DISK_SIZE = '1G'
+DEFAULT_LABEL = 'fastapi-serve'
+APP_NAME = 'fastapi'
+JINA_VERSION = '3.18.0'
+DOCARRAY_VERSION = '0.21.0'
+APP_LOGS_URL = "[https://cloud.jina.ai/](https://cloud.jina.ai/user/flows?action=detail&id={app_id}&tab=logs)"
+PRICING_URL = "****{cph}**** ([Read about pricing here](https://github.com/jina-ai/langchain-serve#-pricing))"
 
 
 @dataclass
 class Defaults:
     instance: str = 'C3'
     autoscale_min: int = 1
     autoscale_max: int = 10
```

### Comparing `fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev6/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.2.dev7/fastapi_serve/cloud/options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 import click
 
 from fastapi_serve.cloud.config import DEFAULT_TIMEOUT, validate_jcloud_config_callback
 
+_common_options = [
+    click.argument(
+        'app',
+        type=str,
+        required=True,
+    ),
+    click.option(
+        '--app-dir',
+        type=str,
+        required=False,
+        help='Base directory to be used for the FastAPI app.',
+    ),
+]
+
 _hubble_push_options = [
     click.option(
         '--image-name',
         type=str,
         required=False,
         help='Name of the image to be pushed.',
     ),
@@ -24,24 +38,24 @@
     ),
     click.option(
         '--requirements',
         default=None,
         type=str,
         help='''Pass either
 
-            1) multiple requirements or,
-            2) a path to a requirements.txt/pyproject.toml file or,
-            3) a directory containing requirements.txt/pyproject.toml file.''',
+1) multiple requirements or,
+2) a path to a requirements.txt/pyproject.toml file or,
+3) a directory containing requirements.txt/pyproject.toml file.''',
         multiple=True,
     ),
     click.option(
         '--version',
         type=str,
         default='latest',
-        help='Version of serving gateway to be used.',
+        help='Version of fastapi-serve to be used.',
         show_default=False,
     ),
     click.option(
         '--verbose',
         is_flag=True,
         help='Verbose mode.',
         show_default=True,
@@ -51,93 +65,65 @@
         is_flag=True,
         help='Push the image publicly.',
         default=False,
         show_default=True,
     ),
 ]
 
-
-_jcloud_shared_options = [
+_jcloud_only_options = [
     click.option(
         '--app-id',
         type=str,
         default=None,
         help='AppID of the deployed agent to be updated.',
         show_default=True,
     ),
     click.option(
-        '--requirements',
-        default=None,
-        type=str,
-        help='''Pass either 
-        1) multiple requirements or,
-        2) a path to a requirements.txt/pyproject.toml file or,
-        3) a directory containing requirements.txt/pyproject.toml file.''',
-        multiple=True,
-    ),
-    click.option(
-        '--version',
-        type=str,
-        default='latest',
-        help='Version of serving gateway to be used.',
-        show_default=False,
-    ),
-    click.option(
         '--timeout',
         type=int,
         default=DEFAULT_TIMEOUT,
         help='Total request timeout in seconds.',
         show_default=True,
     ),
     click.option(
-        '--platform',
-        type=str,
-        default=None,
-        help='Platform of Docker image needed for the deployment is built on.',
-        show_default=False,
-    ),
-    click.option(
         '--config',
         type=click.Path(exists=True),
         help='Path to the config file',
         callback=validate_jcloud_config_callback,
         show_default=False,
     ),
     click.option(
         '--env',
+        '--envs',
         type=click.Path(exists=True),
-        help='Path to the environment file',
+        help='Path to the environment file (should be a .env file)',
+        show_default=False,
+    ),
+    click.option(
+        '--secret',
+        '--secrets',
+        type=click.Path(exists=True),
+        help='Path to the secrets file (should be a .env file)',
         show_default=False,
     ),
     click.option(
         '--cors',
         is_flag=True,
         help='Enable CORS.',
         default=True,
         show_default=True,
     ),
-    click.option(
-        '--verbose',
-        is_flag=True,
-        help='Verbose mode.',
-        show_default=True,
-    ),
-    click.option(
-        '--public',
-        is_flag=True,
-        help='Push the image publicly.',
-        default=False,
-        show_default=True,
-    ),
 ]
 
 
-def hubble_shared_options(func):
-    for option in reversed(_hubble_push_options):
+def hubble_options(func):
+    for option in reversed(_common_options + _hubble_push_options):
         func = option(func)
     return func
 
 
-def jcloud_shared_options(func):
-    for option in reversed(_jcloud_shared_options):
+def jcloud_options(func):
+    for option in reversed(
+        _common_options + _jcloud_only_options + _hubble_push_options
+    ):
         func = option(func)
     return func
```

### Comparing `fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.2.dev7/fastapi_serve/gateway/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from jina.serve.runtimes.gateway.http.fastapi import FastAPIBaseGateway
 
 from fastapi_serve.gateway.helper import (
     APPDIR,
-    EnvironmentVarCtxtManager,
     LoggingMiddleware,
     MetricsMiddleware,
     import_from_string,
 )
+from fastapi_serve.helper import EnvironmentVarCtxtManager
 
 if TYPE_CHECKING:
     from fastapi import FastAPI
 
 
 class FastAPIServeGateway(FastAPIBaseGateway):
-    def __init__(self, app_str: str, *args, **kwargs):
+    def __init__(self, app: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._app_str = app_str
+        self._app_str = app
         self._app: "FastAPI" = None
         self._fix_sys_path()
         self._init_fastapi_app()
         self._configure_cors()
         self._register_healthz()
         self._setup_metrics()
         self._setup_logging()
```

### Comparing `fastapi-serve-0.0.2.dev6/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.2.dev7/fastapi_serve/gateway/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,41 +46,14 @@
         raise ImportFromStringError(
             message.format(attrs_str=attrs_str, module_str=module_str)
         )
 
     return app, module
 
 
-class EnvironmentVarCtxtManager:
-    """a class to wrap env vars"""
-
-    def __init__(self, envs: Dict):
-        """
-        :param envs: a dictionary of environment variables
-        """
-        self._env_keys_added: Dict = envs
-        self._env_keys_old: Dict = {}
-
-    def __enter__(self):
-        for key, val in self._env_keys_added.items():
-            # Store the old value, if it exists
-            if key in os.environ:
-                self._env_keys_old[key] = os.environ[key]
-            # Update the environment variable with the new value
-            os.environ[key] = str(val)
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        # Restore the old values of updated environment variables
-        for key, val in self._env_keys_old.items():
-            os.environ[key] = str(val)
-        # Remove any newly added environment variables
-        for key in self._env_keys_added.keys():
-            os.unsetenv(key)
-
-
 class Timer:
     class SharedData:
         def __init__(self, last_reported_time):
             self.last_reported_time = last_reported_time
 
     def __init__(self, interval: int):
         self.interval = interval
```

### Comparing `fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.2.dev6
+Version: 0.0.2.dev7
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
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev6 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev7 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.2.dev6/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.2.dev7/fastapi_serve.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 fastapi_serve/__init__.py
 fastapi_serve/__main__.py
 fastapi_serve/config.yml
+fastapi_serve/helper.py
 fastapi_serve.egg-info/PKG-INFO
 fastapi_serve.egg-info/SOURCES.txt
 fastapi_serve.egg-info/dependency_links.txt
 fastapi_serve.egg-info/entry_points.txt
 fastapi_serve.egg-info/not-zip-safe
 fastapi_serve.egg-info/requires.txt
 fastapi_serve.egg-info/top_level.txt
```

### Comparing `fastapi-serve-0.0.2.dev6/setup.py` & `fastapi-serve-0.0.2.dev7/setup.py`

 * *Files identical despite different names*

