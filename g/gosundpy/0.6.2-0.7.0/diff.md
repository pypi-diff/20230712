# Comparing `tmp/gosundpy-0.6.2.tar.gz` & `tmp/gosundpy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gosundpy-0.6.2.tar", last modified: Wed Jan 18 01:43:03 2023, max compression
+gzip compressed data, was "gosundpy-0.7.0.tar", last modified: Wed Jul 12 00:30:25 2023, max compression
```

## Comparing `gosundpy-0.6.2.tar` & `gosundpy-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-01-18 01:43:03.580954 gosundpy-0.6.2/
--rw-r--r--   0 rabo       (501) staff       (20)     1073 2022-10-16 07:49:52.000000 gosundpy-0.6.2/LICENSE
--rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-01-18 01:43:03.580844 gosundpy-0.6.2/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)     1035 2022-11-27 06:20:19.000000 gosundpy-0.6.2/README.md
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-01-18 01:43:03.580065 gosundpy-0.6.2/gosundpy/
--rw-r--r--   0 rabo       (501) staff       (20)      645 2023-01-14 04:09:14.000000 gosundpy-0.6.2/gosundpy/__init__.py
--rw-r--r--   0 rabo       (501) staff       (20)     3357 2023-01-18 01:29:44.000000 gosundpy-0.6.2/gosundpy/device.py
--rw-r--r--   0 rabo       (501) staff       (20)      232 2023-01-17 09:35:40.000000 gosundpy-0.6.2/gosundpy/exceptions.py
--rw-r--r--   0 rabo       (501) staff       (20)     2480 2023-01-18 01:34:57.000000 gosundpy-0.6.2/gosundpy/gosund.py
--rw-r--r--   0 rabo       (501) staff       (20)      774 2023-01-18 01:33:20.000000 gosundpy-0.6.2/gosundpy/utils.py
--rw-r--r--   0 rabo       (501) staff       (20)       18 2023-01-18 01:43:00.000000 gosundpy-0.6.2/gosundpy/version.py
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-01-18 01:43:03.580676 gosundpy-0.6.2/gosundpy.egg-info/
--rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-01-18 01:43:03.000000 gosundpy-0.6.2/gosundpy.egg-info/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)      305 2023-01-18 01:43:03.000000 gosundpy-0.6.2/gosundpy.egg-info/SOURCES.txt
--rw-r--r--   0 rabo       (501) staff       (20)        1 2023-01-18 01:43:03.000000 gosundpy-0.6.2/gosundpy.egg-info/dependency_links.txt
--rw-r--r--   0 rabo       (501) staff       (20)       23 2023-01-18 01:43:03.000000 gosundpy-0.6.2/gosundpy.egg-info/requires.txt
--rw-r--r--   0 rabo       (501) staff       (20)        9 2023-01-18 01:43:03.000000 gosundpy-0.6.2/gosundpy.egg-info/top_level.txt
--rw-r--r--   0 rabo       (501) staff       (20)       38 2023-01-18 01:43:03.580993 gosundpy-0.6.2/setup.cfg
--rw-r--r--   0 rabo       (501) staff       (20)     1690 2022-10-16 07:49:52.000000 gosundpy-0.6.2/setup.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:30:25.685336 gosundpy-0.7.0/
+-rw-r--r--   0 rabo       (501) staff       (20)     1073 2022-10-16 07:49:52.000000 gosundpy-0.7.0/LICENSE
+-rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-07-12 00:30:25.685203 gosundpy-0.7.0/PKG-INFO
+-rw-r--r--   0 rabo       (501) staff       (20)     1035 2022-11-27 06:20:19.000000 gosundpy-0.7.0/README.md
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:30:25.684329 gosundpy-0.7.0/gosundpy/
+-rw-r--r--   0 rabo       (501) staff       (20)      645 2023-01-14 04:09:14.000000 gosundpy-0.7.0/gosundpy/__init__.py
+-rw-r--r--   0 rabo       (501) staff       (20)     3357 2023-01-18 01:29:44.000000 gosundpy-0.7.0/gosundpy/device.py
+-rw-r--r--   0 rabo       (501) staff       (20)      232 2023-01-17 09:35:40.000000 gosundpy-0.7.0/gosundpy/exceptions.py
+-rw-r--r--   0 rabo       (501) staff       (20)     2621 2023-07-12 00:07:52.000000 gosundpy-0.7.0/gosundpy/gosund.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1047 2023-07-12 00:07:04.000000 gosundpy-0.7.0/gosundpy/utils.py
+-rw-r--r--   0 rabo       (501) staff       (20)       18 2023-07-12 00:30:17.000000 gosundpy-0.7.0/gosundpy/version.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:30:25.684892 gosundpy-0.7.0/gosundpy.egg-info/
+-rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/PKG-INFO
+-rw-r--r--   0 rabo       (501) staff       (20)      305 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/SOURCES.txt
+-rw-r--r--   0 rabo       (501) staff       (20)        1 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/dependency_links.txt
+-rw-r--r--   0 rabo       (501) staff       (20)       23 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/requires.txt
+-rw-r--r--   0 rabo       (501) staff       (20)        9 2023-07-12 00:30:25.000000 gosundpy-0.7.0/gosundpy.egg-info/top_level.txt
+-rw-r--r--   0 rabo       (501) staff       (20)       38 2023-07-12 00:30:25.685381 gosundpy-0.7.0/setup.cfg
+-rw-r--r--   0 rabo       (501) staff       (20)     1690 2022-10-16 07:49:52.000000 gosundpy-0.7.0/setup.py
```

### Comparing `gosundpy-0.6.2/LICENSE` & `gosundpy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gosundpy-0.6.2/PKG-INFO` & `gosundpy-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gosundpy
-Version: 0.6.2
+Version: 0.7.0
 Summary: Python API for controling Gosund smart devices
 Home-page: https://github.com/purple4reina/gosundpy
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/gosundpy
 Project-URL: Bug Tracker, https://github.com/purple4reina/gosundpy/issues
```

### Comparing `gosundpy-0.6.2/README.md` & `gosundpy-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `gosundpy-0.6.2/gosundpy/__init__.py` & `gosundpy-0.7.0/gosundpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gosundpy-0.6.2/gosundpy/device.py` & `gosundpy-0.7.0/gosundpy/device.py`

 * *Files identical despite different names*

### Comparing `gosundpy-0.6.2/gosundpy/gosund.py` & `gosundpy-0.7.0/gosundpy/gosund.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from tuya_iot import TuyaOpenAPI, AuthType, TuyaDeviceManager, TuyaOpenMQ
 
 from .device import GosundDevice
 from .exceptions import assert_response_success, GosundException
-from .utils import cache_response
+from .utils import cache_response, wrap_session_timeout
 
 class Gosund(object):
 
     def __init__(self, username, password, access_id, access_key, country=1,
-            endpoint='https://openapi.tuyaus.com', status_cache_seconds=None):
+            endpoint='https://openapi.tuyaus.com', status_cache_seconds=None,
+            timeout=None):
         self.api = TuyaOpenAPI(endpoint, access_id, access_key,
                 auth_type=AuthType.CUSTOM)
+        if timeout is not None:
+            wrap_session_timeout(self.api.session, timeout)
+
         resp = self.api.connect(username, password, country)
         assert_response_success('connect to api', resp)
         self.manager = TuyaDeviceManager(self.api, TuyaOpenMQ(self.api))
         self._known_devices = {}
 
         self._status_caching = False
         if status_cache_seconds is not None:
```

### Comparing `gosundpy-0.6.2/gosundpy/utils.py` & `gosundpy-0.7.0/gosundpy/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,7 +24,15 @@
                 return cache.value
             cache.set(now, fn(*args, **kwargs))
             return cache.value
         cache = _timed_cache()
         _call.clear_cache = cache.reset
         return _call
     return _rate_limit
+
+def wrap_session_timeout(session, _timeout):
+    def _wrap(fn):
+        @functools.wraps(fn)
+        def _request(*args, timeout=None, **kwargs):
+            return fn(*args, timeout=_timeout, **kwargs)
+        return _request
+    session.request = _wrap(session.request)
```

### Comparing `gosundpy-0.6.2/gosundpy.egg-info/PKG-INFO` & `gosundpy-0.7.0/gosundpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gosundpy
-Version: 0.6.2
+Version: 0.7.0
 Summary: Python API for controling Gosund smart devices
 Home-page: https://github.com/purple4reina/gosundpy
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/gosundpy
 Project-URL: Bug Tracker, https://github.com/purple4reina/gosundpy/issues
```

### Comparing `gosundpy-0.6.2/setup.py` & `gosundpy-0.7.0/setup.py`

 * *Files identical despite different names*

