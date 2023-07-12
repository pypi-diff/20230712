# Comparing `tmp/skytek-utils-0.6.0.tar.gz` & `tmp/skytek-utils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytek-utils-0.6.0.tar", last modified: Mon Jul 10 07:53:14 2023, max compression
+gzip compressed data, was "skytek-utils-0.7.0.tar", last modified: Wed Jul 12 10:21:39 2023, max compression
```

## Comparing `skytek-utils-0.6.0.tar` & `skytek-utils-0.7.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:14.130519 skytek-utils-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-10 07:53:14.130519 skytek-utils-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:14.126519 skytek-utils-0.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:53:14.130519 skytek-utils-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:14.126519 skytek-utils-0.6.0/skytek_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 07:53:05.000000 skytek-utils-0.6.0/skytek_utils/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:14.130519 skytek-utils-0.6.0/skytek_utils/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/django/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:14.130519 skytek-utils-0.6.0/skytek_utils/interconnect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/interconnect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:14.130519 skytek-utils-0.6.0/skytek_utils/interconnect/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/interconnect/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/interconnect/api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/interconnect/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/interconnect/api/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/interconnect/api/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/interconnect/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/interconnect/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/skytek_utils/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:14.130519 skytek-utils-0.6.0/skytek_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-10 07:53:14.000000 skytek-utils-0.6.0/skytek_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-10 07:53:14.000000 skytek-utils-0.6.0/skytek_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:53:14.000000 skytek-utils-0.6.0/skytek_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:53:13.000000 skytek-utils-0.6.0/skytek_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 07:53:14.000000 skytek-utils-0.6.0/skytek_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 07:53:14.000000 skytek-utils-0.6.0/skytek_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:14.130519 skytek-utils-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-10 07:53:03.000000 skytek-utils-0.6.0/tests/test_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:39.344329 skytek-utils-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-12 10:21:39.344329 skytek-utils-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:39.332329 skytek-utils-0.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:21:39.344329 skytek-utils-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:39.336329 skytek-utils-0.7.0/skytek_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 10:21:30.000000 skytek-utils-0.7.0/skytek_utils/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:39.340329 skytek-utils-0.7.0/skytek_utils/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/django/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:39.340329 skytek-utils-0.7.0/skytek_utils/interconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/interconnect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:39.344329 skytek-utils-0.7.0/skytek_utils/interconnect/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/interconnect/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/interconnect/api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/interconnect/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/interconnect/api/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/interconnect/api/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/interconnect/api/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/interconnect/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/interconnect/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/skytek_utils/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:39.340329 skytek-utils-0.7.0/skytek_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-12 10:21:39.000000 skytek-utils-0.7.0/skytek_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 10:21:39.000000 skytek-utils-0.7.0/skytek_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:21:39.000000 skytek-utils-0.7.0/skytek_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:21:39.000000 skytek-utils-0.7.0/skytek_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 10:21:39.000000 skytek-utils-0.7.0/skytek_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 10:21:39.000000 skytek-utils-0.7.0/skytek_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:21:39.344329 skytek-utils-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 10:21:28.000000 skytek-utils-0.7.0/tests/test_iter.py
```

### Comparing `skytek-utils-0.6.0/LICENSE` & `skytek-utils-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.6.0/PKG-INFO` & `skytek-utils-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.6.0
+Version: 0.7.0
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.6.0/setup.py` & `skytek-utils-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.6.0/skytek_utils/celery.py` & `skytek-utils-0.7.0/skytek_utils/celery.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.6.0/skytek_utils/datetime.py` & `skytek-utils-0.7.0/skytek_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.6.0/skytek_utils/django/shortcuts.py` & `skytek-utils-0.7.0/skytek_utils/django/shortcuts.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.6.0/skytek_utils/interconnect/api/authentication.py` & `skytek-utils-0.7.0/skytek_utils/interconnect/api/authentication.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.6.0/skytek_utils/interconnect/api/client.py` & `skytek-utils-0.7.0/skytek_utils/interconnect/api/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import requests
-from django.conf import settings
 
+from .conf import settings
 from .jwt import generate_jwt
 
 
 class Client:
     def __init__(self, remote_module: str) -> None:
         self.remote_module = remote_module
 
     def _get_host(self):
         environment_domain = settings.INTERCONNECT_ENVIRONMENT_DOMAIN
         return f"{self.remote_module}.{environment_domain}"
 
     def _make_url(self, path: str):
         host = self._get_host()
-        protocol = (
-            "https" if getattr(settings, "INTERCONNECT_USE_SSL", True) else "http"
-        )
+        protocol = "https" if settings.INTERCONNECT_USE_SSL else "http"
         if not path.startswith("/"):
             path = f"/{path}"
         return f"{protocol}://{host}{path}"
 
     def _call_api_by_path(self, method, path, *args, **kwargs):
         url = self._make_url(path)
         return self._call_api(method, url, *args, **kwargs)
```

### Comparing `skytek-utils-0.6.0/skytek_utils/interconnect/api/jwt.py` & `skytek-utils-0.7.0/skytek_utils/interconnect/api/jwt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime, timedelta
 from typing import Optional
 
 import jwt
-from django.conf import settings
 
+from .conf import settings
 from .user import ModuleUser
 
 
 def jwt_to_module_user(token: str) -> Optional[ModuleUser]:
     key = settings.INTERCONNECT_JWT_ENCODE_KEY
     if not key:
         return None
```

### Comparing `skytek-utils-0.6.0/skytek_utils/interconnect/api/mixins.py` & `skytek-utils-0.7.0/skytek_utils/interconnect/api/mixins.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.6.0/skytek_utils/interconnect/api/permissions.py` & `skytek-utils-0.7.0/skytek_utils/interconnect/api/permissions.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.6.0/skytek_utils/monitoring.py` & `skytek-utils-0.7.0/skytek_utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.6.0/skytek_utils.egg-info/PKG-INFO` & `skytek-utils-0.7.0/skytek_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.6.0
+Version: 0.7.0
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.6.0/skytek_utils.egg-info/SOURCES.txt` & `skytek-utils-0.7.0/skytek_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 skytek_utils/django/forms.py
 skytek_utils/django/models.py
 skytek_utils/django/shortcuts.py
 skytek_utils/interconnect/__init__.py
 skytek_utils/interconnect/api/__init__.py
 skytek_utils/interconnect/api/authentication.py
 skytek_utils/interconnect/api/client.py
+skytek_utils/interconnect/api/conf.py
 skytek_utils/interconnect/api/jwt.py
 skytek_utils/interconnect/api/mixins.py
 skytek_utils/interconnect/api/permissions.py
 skytek_utils/interconnect/api/user.py
 tests/test_iter.py
```

### Comparing `skytek-utils-0.6.0/tests/test_iter.py` & `skytek-utils-0.7.0/tests/test_iter.py`

 * *Files identical despite different names*

