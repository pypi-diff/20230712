# Comparing `tmp/testdata-6.1.1.tar.gz` & `tmp/testdata-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdata-6.1.1.tar", last modified: Mon Mar 20 20:47:12 2023, max compression
+gzip compressed data, was "testdata-6.2.0.tar", last modified: Wed Jul 12 20:18:57 2023, max compression
```

## Comparing `testdata-6.1.1.tar` & `testdata-6.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:47:12.340786 testdata-6.1.1/
--rw-r--r--   0 jaymon     (501) staff       (20)     1080 2017-04-07 22:45:17.000000 testdata-6.1.1/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)    11736 2023-03-20 20:47:12.340594 testdata-6.1.1/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)    10967 2023-02-16 22:36:07.000000 testdata-6.1.1/README.md
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-03-20 20:47:12.340831 testdata-6.1.1/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     1766 2021-04-15 00:12:41.000000 testdata-6.1.1/setup.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:47:12.333607 testdata-6.1.1/testdata/
--rw-r--r--   0 jaymon     (501) staff       (20)     4469 2023-03-20 20:46:29.000000 testdata-6.1.1/testdata/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3048 2023-02-26 22:15:17.000000 testdata-6.1.1/testdata/base.py
--rw-r--r--   0 jaymon     (501) staff       (20)    15283 2023-02-16 22:42:02.000000 testdata-6.1.1/testdata/client.py
--rw-r--r--   0 jaymon     (501) staff       (20)      338 2023-02-16 01:11:44.000000 testdata-6.1.1/testdata/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1120 2023-02-16 22:56:53.000000 testdata-6.1.1/testdata/config.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:47:12.335837 testdata-6.1.1/testdata/data/
--rw-r--r--   0 jaymon     (501) staff       (20)    50131 2023-02-16 07:25:50.000000 testdata-6.1.1/testdata/data/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)      218 2019-08-08 04:23:32.000000 testdata-6.1.1/testdata/data/animated.gif
--rw-r--r--   0 jaymon     (501) staff       (20)     2438 2019-08-08 22:28:06.000000 testdata-6.1.1/testdata/data/favicon.ico
--rw-r--r--   0 jaymon     (501) staff       (20)      740 2019-07-27 01:14:03.000000 testdata-6.1.1/testdata/data/static.gif
--rw-r--r--   0 jaymon     (501) staff       (20)      305 2019-07-27 01:14:40.000000 testdata-6.1.1/testdata/data/static.jpg
--rw-r--r--   0 jaymon     (501) staff       (20)     1264 2019-08-09 04:19:10.000000 testdata-6.1.1/testdata/data/static.png
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:47:12.336708 testdata-6.1.1/testdata/data/usa/
--rw-r--r--   0 jaymon     (501) staff       (20)      195 2020-05-30 22:47:48.000000 testdata-6.1.1/testdata/data/usa/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)   146041 2020-05-30 22:45:38.000000 testdata-6.1.1/testdata/data/usa/cities.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5928 2020-05-30 22:43:32.000000 testdata-6.1.1/testdata/data/usa/states.py
--rw-r--r--   0 jaymon     (501) staff       (20)   471413 2020-05-30 22:46:08.000000 testdata-6.1.1/testdata/data/usa/zipcodes.py
--rw-r--r--   0 jaymon     (501) staff       (20)    14150 2023-02-16 07:56:48.000000 testdata-6.1.1/testdata/mocking.py
--rw-r--r--   0 jaymon     (501) staff       (20)    10612 2023-02-26 22:49:07.000000 testdata-6.1.1/testdata/output.py
--rw-r--r--   0 jaymon     (501) staff       (20)    30479 2023-02-16 22:43:04.000000 testdata-6.1.1/testdata/path.py
--rw-r--r--   0 jaymon     (501) staff       (20)     8373 2023-02-27 22:07:07.000000 testdata-6.1.1/testdata/server.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2158 2023-03-09 01:28:47.000000 testdata-6.1.1/testdata/service.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6815 2023-02-26 22:02:42.000000 testdata-6.1.1/testdata/test.py
--rw-r--r--   0 jaymon     (501) staff       (20)    10584 2023-02-16 01:06:35.000000 testdata-6.1.1/testdata/threading.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:47:12.337725 testdata-6.1.1/testdata/types/
--rw-r--r--   0 jaymon     (501) staff       (20)       26 2023-02-15 00:25:30.000000 testdata-6.1.1/testdata/types/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5761 2023-02-18 00:22:25.000000 testdata-6.1.1/testdata/types/datetime.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2082 2023-02-19 00:17:01.000000 testdata-6.1.1/testdata/types/mapping.py
--rw-r--r--   0 jaymon     (501) staff       (20)    12831 2023-03-18 21:11:47.000000 testdata-6.1.1/testdata/types/number.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2708 2023-03-18 21:12:54.000000 testdata-6.1.1/testdata/types/sequence.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11366 2023-03-07 07:03:34.000000 testdata-6.1.1/testdata/types/string.py
--rw-r--r--   0 jaymon     (501) staff       (20)    14185 2023-02-16 22:52:56.000000 testdata-6.1.1/testdata/user.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:47:12.334248 testdata-6.1.1/testdata.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)    11736 2023-03-20 20:47:12.000000 testdata-6.1.1/testdata.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     1108 2023-03-20 20:47:12.000000 testdata-6.1.1/testdata.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-03-20 20:47:12.000000 testdata-6.1.1/testdata.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-03-20 20:47:12.000000 testdata-6.1.1/testdata.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       15 2023-03-20 20:47:12.000000 testdata-6.1.1/testdata.egg-info/top_level.txt
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:47:12.340274 testdata-6.1.1/tests/
--rw-r--r--   0 jaymon     (501) staff       (20)      197 2023-02-15 01:00:57.000000 testdata-6.1.1/tests/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)      820 2023-02-26 20:39:42.000000 testdata-6.1.1/tests/base_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4197 2023-02-16 22:46:32.000000 testdata-6.1.1/tests/client_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     9285 2023-02-16 20:39:25.000000 testdata-6.1.1/tests/mocking_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4762 2023-02-26 22:47:57.000000 testdata-6.1.1/tests/output_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)    18376 2023-02-16 19:57:44.000000 testdata-6.1.1/tests/path_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3050 2023-02-16 19:59:45.000000 testdata-6.1.1/tests/server_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2889 2023-02-26 00:46:27.000000 testdata-6.1.1/tests/test_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1587 2023-02-16 19:57:20.000000 testdata-6.1.1/tests/testdata_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5487 2023-02-16 20:39:27.000000 testdata-6.1.1/tests/threading_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11416 2023-02-16 22:55:44.000000 testdata-6.1.1/tests/types_test.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3696 2023-02-16 22:53:13.000000 testdata-6.1.1/tests/user_test.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:18:57.797539 testdata-6.2.0/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1080 2017-04-07 22:45:17.000000 testdata-6.2.0/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)    11736 2023-07-12 20:18:57.797345 testdata-6.2.0/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)    10967 2023-02-16 22:36:07.000000 testdata-6.2.0/README.md
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-07-12 20:18:57.797579 testdata-6.2.0/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1766 2021-04-15 00:12:41.000000 testdata-6.2.0/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:18:57.791440 testdata-6.2.0/testdata/
+-rw-r--r--   0 jaymon     (501) staff       (20)     4469 2023-07-12 20:04:58.000000 testdata-6.2.0/testdata/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3048 2023-02-26 22:15:17.000000 testdata-6.2.0/testdata/base.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3565 2023-07-12 20:07:29.000000 testdata-6.2.0/testdata/client.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      338 2023-02-16 01:11:44.000000 testdata-6.2.0/testdata/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1120 2023-02-16 22:56:53.000000 testdata-6.2.0/testdata/config.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:18:57.792871 testdata-6.2.0/testdata/data/
+-rw-r--r--   0 jaymon     (501) staff       (20)    50131 2023-02-16 07:25:50.000000 testdata-6.2.0/testdata/data/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      218 2019-08-08 04:23:32.000000 testdata-6.2.0/testdata/data/animated.gif
+-rw-r--r--   0 jaymon     (501) staff       (20)     2438 2019-08-08 22:28:06.000000 testdata-6.2.0/testdata/data/favicon.ico
+-rw-r--r--   0 jaymon     (501) staff       (20)      740 2019-07-27 01:14:03.000000 testdata-6.2.0/testdata/data/static.gif
+-rw-r--r--   0 jaymon     (501) staff       (20)      305 2019-07-27 01:14:40.000000 testdata-6.2.0/testdata/data/static.jpg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1264 2019-08-09 04:19:10.000000 testdata-6.2.0/testdata/data/static.png
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:18:57.793765 testdata-6.2.0/testdata/data/usa/
+-rw-r--r--   0 jaymon     (501) staff       (20)      195 2020-05-30 22:47:48.000000 testdata-6.2.0/testdata/data/usa/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)   146041 2020-05-30 22:45:38.000000 testdata-6.2.0/testdata/data/usa/cities.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5928 2020-05-30 22:43:32.000000 testdata-6.2.0/testdata/data/usa/states.py
+-rw-r--r--   0 jaymon     (501) staff       (20)   471413 2020-05-30 22:46:08.000000 testdata-6.2.0/testdata/data/usa/zipcodes.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    14150 2023-02-16 07:56:48.000000 testdata-6.2.0/testdata/mocking.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    10786 2023-07-12 20:04:18.000000 testdata-6.2.0/testdata/output.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    30479 2023-07-11 23:50:10.000000 testdata-6.2.0/testdata/path.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     8380 2023-07-12 00:30:55.000000 testdata-6.2.0/testdata/server.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2158 2023-07-11 23:49:54.000000 testdata-6.2.0/testdata/service.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6815 2023-02-26 22:02:42.000000 testdata-6.2.0/testdata/test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6933 2023-07-12 20:14:01.000000 testdata-6.2.0/testdata/threading.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:18:57.795292 testdata-6.2.0/testdata/types/
+-rw-r--r--   0 jaymon     (501) staff       (20)       26 2023-02-15 00:25:30.000000 testdata-6.2.0/testdata/types/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5761 2023-02-18 00:22:25.000000 testdata-6.2.0/testdata/types/datetime.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2082 2023-02-19 00:17:01.000000 testdata-6.2.0/testdata/types/mapping.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    12831 2023-03-18 21:11:47.000000 testdata-6.2.0/testdata/types/number.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2708 2023-03-18 21:12:54.000000 testdata-6.2.0/testdata/types/sequence.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11366 2023-03-07 07:03:34.000000 testdata-6.2.0/testdata/types/string.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    14185 2023-02-16 22:52:56.000000 testdata-6.2.0/testdata/user.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:18:57.792119 testdata-6.2.0/testdata.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)    11736 2023-07-12 20:18:57.000000 testdata-6.2.0/testdata.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     1108 2023-07-12 20:18:57.000000 testdata-6.2.0/testdata.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-07-12 20:18:57.000000 testdata-6.2.0/testdata.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-07-12 20:18:57.000000 testdata-6.2.0/testdata.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       15 2023-07-12 20:18:57.000000 testdata-6.2.0/testdata.egg-info/top_level.txt
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-12 20:18:57.797162 testdata-6.2.0/tests/
+-rw-r--r--   0 jaymon     (501) staff       (20)      197 2023-02-15 01:00:57.000000 testdata-6.2.0/tests/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      820 2023-02-26 20:39:42.000000 testdata-6.2.0/tests/base_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1580 2023-07-12 19:40:38.000000 testdata-6.2.0/tests/client_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     9285 2023-02-16 20:39:25.000000 testdata-6.2.0/tests/mocking_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4762 2023-07-12 20:02:52.000000 testdata-6.2.0/tests/output_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    18376 2023-02-16 19:57:44.000000 testdata-6.2.0/tests/path_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3050 2023-02-16 19:59:45.000000 testdata-6.2.0/tests/server_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2889 2023-02-26 00:46:27.000000 testdata-6.2.0/tests/test_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1587 2023-02-16 19:57:20.000000 testdata-6.2.0/tests/testdata_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5124 2023-07-12 20:09:09.000000 testdata-6.2.0/tests/threading_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11416 2023-02-16 22:55:44.000000 testdata-6.2.0/tests/types_test.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3696 2023-02-16 22:53:13.000000 testdata-6.2.0/tests/user_test.py
```

### Comparing `testdata-6.1.1/LICENSE.txt` & `testdata-6.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/PKG-INFO` & `testdata-6.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testdata
-Version: 6.1.1
+Version: 6.2.0
 Summary: Easily generate random unicode test data among other things
 Home-page: http://github.com/Jaymon/testdata
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `testdata-6.1.1/README.md` & `testdata-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/setup.py` & `testdata-6.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/__init__.py` & `testdata-6.2.0/testdata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from .types.sequence import *
 from .types.mapping import *
 from .types.datetime import *
 from .user import *
 from .base import TestData
 
 
-__version__ = '6.1.1'
+__version__ = '6.2.0'
 
 
 # get rid of "No handler found" warnings (cribbed from requests)
 # DEPRECATED 7-15-2022, doesn't seem to be needed in python3
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `testdata-6.1.1/testdata/base.py` & `testdata-6.2.0/testdata/base.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/client.py` & `testdata-6.2.0/testdata/mocking.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,504 +1,377 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals, division, print_function, absolute_import
-import os
-import subprocess
+import types
+import inspect
 import sys
-import re
-import signal
-import time
-import logging
-
-from datatypes import (
-    HTTPClient as HTTP,
-    Dict,
-    make_list,
-)
+import importlib
+import os
+import copy
+import functools
 
 from .compat import *
-from .threading import Thread, Deque
 from .base import TestData
 
 
-logger = logging.getLogger(__name__)
-
-
-class Command(object):
-    """makes running a command from a non CLI environment easy peasy
-
-    This is handy when you need to test some CLI functionality of your python
-    modules.
-
-    c = Command("echo")
-    r = c.run("hello")
-    print(r) # hello
-    """
-
-    quiet = False
-    """this is the default quiet setting for running a script, it can be overriden in run()"""
-
-    bufsize = 1000
-    """how many lines to buffer of output, set to 0 to suppress all output"""
-
-    thread_class = Thread
-    """the threading class to use if run_async() is called instead of run()"""
-
-    @property
-    def returncode(self):
-        return self.process.returncode
-
-    @property
-    def cmd(self):
-        return self.process.cmd
-
-    @property
-    def buf(self):
-        return self.process.deque
-
-    @property
-    def environ(self):
-        environ = getattr(self, "_environ", None)
-        if not environ:
-            environ = dict(os.environ)
-
-        pythonpath = self.cwd
-        if "PYTHONPATH" in environ:
-            environ["PYTHONPATH"] += os.pathsep + pythonpath
-        else:
-            environ["PYTHONPATH"] = pythonpath
+###############################################################################
+# Supporting classes and methods
+###############################################################################
 
-        if os.getcwd() not in environ["PYTHONPATH"]:
-            environ["PYTHONPATH"] += os.pathsep + os.getcwd()
+class Mock(object):
+    """Do our very best to mock functionality
 
-        # make sure each value is a string
-        for k in environ.keys():
-            if not isinstance(environ[k], basestring):
-                environ[k] = String(environ[k])
-
-        self._environ = environ
-        return environ
-
-    @environ.setter
-    def environ(self, v):
-        self._environ = v
-
-    @environ.deleter
-    def environ(self):
-        del self._environ
-
-    def __init__(self, command, cwd="", environ=None, **kwargs):
-        self.cwd = os.path.realpath(cwd) if cwd else os.getcwd()
-        self.command = command
-        if environ:
-            self.environ.update(environ)
-
-        self.logger_prefix = kwargs.pop("logger_prefix", None)
-        logger = logging.getLogger("{}.Client".format(__name__))
-        if len(logger.handlers) == 0:
-            logger.setLevel(logging.INFO)
-            log_handler = logging.StreamHandler(stream=sys.stdout)
-            log_handler.setFormatter(logging.Formatter('%(message)s'))
-            logger.addHandler(log_handler)
-            logger.propagate = False
-        self.logger = logger
-
-        self.sudo = kwargs.pop("sudo", False)
-
-    def flush(self, line):
-        """flush the line to stdout"""
-        if self.logger_prefix is None:
-            self.logger_prefix = "{:0>5}: ".format(self.process.pid)
-
-        #self.logger.info("{:0>5}: {}".format(self.process.pid, line.rstrip()))
-        self.logger.info("{}{}".format(self.logger_prefix, line.rstrip()))
-        #sys.stdout.write(line)
-        #sys.stdout.flush()
-
-    def is_running(self):
-        return self.process.poll() is None
-
-    def create_cmd(self, command, arg_str):
-        if command:
-            if isinstance(command, basestring):
-                cmd = command
-                if arg_str:
-                    if isinstance(arg_str, basestring):
-                        cmd += " " + arg_str
-                    else:
-                        cmd += " ".join(arg_str)
+    This class tries to make it easy to mock an object, and can be used to quickly
+    get an object that can match a certain state, it isn't exhaustive and will fail
+    on things like isinstance checks, but it does it's very best to get you a mocked
+    up object that you can use for testing.
 
-            else:
-                cmd = list(command)
-                if arg_str:
-                    if isinstance(arg_str, basestring):
-                        cmd.append(arg_str)
-                    else:
-                        cmd.extend(arg_str)
+    If the given attribute doesn't exist then this will return an instance of self
+    so you can chain together objects of any depth with just the first object
 
-        else:
-            cmd = arg_str
-
-        if self.sudo:
-            if isinstance(cmd, basestring):
-                if not cmd.startswith("sudo"):
-                    cmd = "sudo " + cmd
+    At some point in the future this should extend this:
+        https://docs.python.org/dev/library/unittest.mock.html
 
-            else:
-                if not cmd[0] == "sudo":
-                    cmd.insert(0, "sudo")
+    :Example:
+        m = Mock(foo=1)
+        m.foo() # 1
+        m.foo # 1
+        m.bar.che.foo # 1
 
-        return cmd
+        m = Mock(foo=ValueError("the error you want to raise"))
+        m.foo(1, 2) # raises ValueError
+    """
+    def __init__(self, patches=None, **kwargs_patches):
+        self._patch(patches, **kwargs_patches)
 
-    def create_process(self, arg_str, **kwargs):
+    def __call__(self, *args, **kwargs):
+        """if the method doesn't exist then return self so you can do things like
+        `Mock(foo=1).bar().che().foo` and have it work similar to `Mock(foo=1).bar.che.foo`
         """
-        https://docs.python.org/3/library/subprocess.html
-        """
-        process = None
-        cmd = self.create_cmd(self.command, arg_str)
-
-        options = {}
-        options["quiet"] = quiet = kwargs.pop("quiet", self.quiet)
-
-        kwargs = Dict(kwargs)
-
-        retcode = kwargs.pops([
-            "code",
-            "ret_code",
-            "returncode",
-            "retcode",
-            "expected_ret_code",
-            "expected_returncode",
-            "codes",
-            "ret_codes",
-            "returncodes",
-            "retcodes",
-            "expected_ret_codes",
-            "expected_returncodes",
-        ], 0)
-        options["expected_returncodes"] = set(make_list(retcode))
-
-        # any kwargs with all capital letters should be considered environment
-        # variables
-        environ = self.environ
-        for k in list(kwargs.keys()):
-            if k.isupper():
-                environ[k] = kwargs.pop(k)
-
-        # we will allow overriding of these values
-        kwargs.setdefault("stderr", subprocess.STDOUT)
-
-        # we will not allow these to be overridden via kwargs
-        kwargs["shell"] = isinstance(cmd, basestring)
-        kwargs["stdout"] = subprocess.PIPE
-        kwargs["cwd"] = self.cwd
-        kwargs["env"] = environ
+        return self
 
+    def __getitem__(self, key):
         try:
-            process = subprocess.Popen(
-                cmd,
-                **kwargs
-            )
-
-        except subprocess.CalledProcessError as e:
-            process.returncode = e.returncode
-
-        finally:
-            if process:
-                process.options = options
-                process.cmd = cmd
-                process.deque = Deque(maxlen=self.bufsize)
+            v = super(Mock, self).__getattribute__(key)
 
-        self.process = process
-        return process
+        except AttributeError:
+            return self
 
-    def __iter__(self):
-        process = self.process
-        try:
-            # another round of links
-            # http://stackoverflow.com/a/17413045/5006 (what I used)
-            # http://stackoverflow.com/questions/2715847/
-            for line in iter(process.stdout.readline, b""):
-                line = line.decode("utf-8")
-                process.deque.append(line.rstrip())
-                if not process.options.get("quiet", False):
-                    self.flush(line)
-                yield line
-
-        finally:
-            if process:
-                process.stdout.close()
-
-    def quit(self, timeout=1):
-        """same as .terminate but uses signals"""
-        return self.finish("send_signal", timeout=timeout, args=(signal.SIGTERM,))
-        #self.process.send_signal(signal.SIGTERM)
-        #return self.wait(timeout)
-
-    def kill(self, timeout=1):
-        """kill -9 the script running asyncronously"""
-        return self.finish("kill", timeout=timeout)
-        #self.process.kill()
-        #return self.wait(timeout)
-
-    def terminate(self, timeout=1):
-        """terminate the script running asyncronously"""
-        return self.finish("terminate", timeout=timeout)
-        #self.process.terminate()
-        #return self.wait(timeout)
-
-    def murder(self, timeout=1):
-        cmd = self.create_cmd(["pkill", "-f", self.cmd], "")
-        logger.debug("Murdering {}".format(self.cmd))
-        if is_py2:
-            subprocess.call(cmd)
         else:
-            subprocess.run(cmd, check=False)
-        return self.wait(timeout)
-
-    def finish(self, method, timeout=1, maxcount=5, args=None, kwargs=None):
-        ret = ""
-
-        args = args or ()
-        kwargs = kwargs or {}
-
-        while self.is_running():
-            getattr(self.process, method)(*args, **kwargs)
-            ret = self.wait(timeout=timeout)
-            if ret.returncode is None:
-                count += 1
-                if count >= maxcount:
-                    ret = self.murder()
-
-        return ret
-
-    def wait(self, timeout=None):
-        ret = ""
-        if is_py2:
-            if timeout:
-                start = time.time()
-                stop = start
-                while self.is_running() and stop - start < timeout:
-                    time.sleep(0.1)
-                    stop = time.time()
+            self._raise_if_error(v)
+            #self.__dict__["_raise_if_error"](v)
+            return v
+
+    def __getattribute__(self, key):
+        # this makes sure the methods defined on this class get through this call
+        if key.startswith("_") and hasattr(type(self), key):
+            return super(Mock, self).__getattribute__(key)
 
-            else:
-                self.process.wait()
+        try:
+            v = super(Mock, self).__getattribute__(key)
 
-            ret = String("\n".join(self.buf))
+        except AttributeError:
+            # if the attribute doesn't exist then return self so you can do
+            # things like `Mock(foo=1).bar.che.foo` and have it work
+            return self
 
         else:
-            try:
-                self.process.wait(timeout=timeout)
-
-            except subprocess.TimeoutExpired:
-                pass
-
-            else:
-                ret = String("\n".join(self.buf))
+            if v is not None:
 
+                self._raise_if_error(v)
 
-        ret.returncode = self.returncode
-        return ret
-    join = wait
+                if not hasattr(v, "__call__"):
 
-    def run_async(self, arg_str="", **kwargs):
-        self.process = self.create_process(arg_str, **kwargs)
+                    frames = inspect.stack()
+                    frame = frames[1]
+                    loc = "\n".join(frame[4]) if frame[4] else ["REPL"]
+                    if ".{}(".format(key) in loc or ".{}".format(key) not in loc:
+
+                        # https://stackoverflow.com/questions/2172189/why-i-cant-extend-bool-in-python
+                        not_bool = (not self._is_instance(v, bool) and not self._is_subclass(v, bool))
+                        class_type = type(v) if not_bool else object 
+
+                        class MockAttr(class_type):
+                            def __new__(cls, *args, **kwargs):
+                                try:
+                                    return super(MockAttr, cls).__new__(cls, *args, **kwargs)
+                                except TypeError:
+                                    return super(MockAttr, cls).__new__(cls)
+
+                            def __call__(self, *args, **kwargs):
+                                return v
+
+                            def __bool__(self):
+                                return bool(v)
+                            __nonzero__ = __bool__
+
+                        return MockAttr(v)
+
+        return v
+
+    def _patch(self, patches=None, **kwargs_patches):
+        if not patches: patches = {}
+        patches.update(kwargs_patches)
+        for k, v in patches.items():
+            if "." in k:
+                k = k.split(".")[-1]
+            setattr(self, k, v)
+
+    def _raise_if_error(self, v):
+        if self._is_instance(v, Exception):
+            raise v
+        elif self._is_subclass(v, Exception):
+            raise v()
 
-        def target():
-            for line in self:
-                pass
-
-        t = self.thread_class(target=target)
-        t.daemon = True
-        t.start()
-        self.async_thread = t
-
-    def run(self, arg_str="", **kwargs):
-        """runs the passed in arguments
-
-        :param arg_str: string, the argument flags that will be passed to the command
-        :param **kwargs: These will be passed to subprocess or consumed
-        :returns: string, the string of the output and will have .returncode attribute
-        """
-        process = self.create_process(arg_str, **kwargs)
+    def _is_instance(self, v, class_types):
+        try:
+            if isinstance(v, class_types):
+                return True
 
-        for line in self: # consume all the output from the program
+        except TypeError:
             pass
+        return False
 
-        process.wait()
-
-        expected_retcodes = process.options["expected_returncodes"]
-        if process.returncode not in expected_retcodes:
-            raise RuntimeError("{} returned {}, expected {}".format(
-                self.process.cmd,
-                process.returncode,
-                expected_retcodes
-            ))
-
-        # we wrap the output in a String so we can set returncode
-        ret = String("\n".join(self.buf))
-        ret.returncode = process.returncode
-        return ret
-
-
-class ModuleCommand(Command):
-    """This sets the client up so you can just pass the module name and have everything
-    just work
+    def _is_subclass(self, v, class_types):
+        try:
+            if issubclass(v, class_types):
+                return True
 
-    :Example:
-        #You can setup this command 2 ways
+        except TypeError:
+            pass
+        return False
 
-        # 1 - pass in the module name
-        c = ModuleCommand("module_name")
 
-        # 2 - have the parent set it
-        class MyCommand(ModuleCommand):
-            name = "module_name"
-        c = MyCommand()
-    """
-    cmd_prefix = "{} -m".format(sys.executable)
-    """this is what will be used to invoke captain from the command line when run()
-    is called"""
+###############################################################################
+# testdata functions
+###############################################################################
+class MockData(TestData):
+    def patch_instance(self, mod, patches=None, **kwargs_patches):
+        """Helper function called from .patch() that will patch a class instance"""
+        if mod is None:
+            raise ValueError("mod is empty")
+
+        if not patches: patches = {}
+        patches.update(kwargs_patches) # combine both dicts
+
+        for name, patch in patches.items():
+            val = getattr(mod, name, None)
+            if inspect.isroutine(val):
+                # we first try and patch as is, if we fail then we wrap the patch in a
+                # lambda
+                try:
+                    setattr(mod, name, types.MethodType(patch, mod))
+
+                except TypeError:
+                    setattr(
+                        mod,
+                        name,
+                        types.MethodType(
+                            # lambda binding issue, see the explanation in patch_class
+                            # why I'm using partial here
+                            functools.partial(lambda *a, **kw: kw["__patch"], __patch=patch),
+                            mod
+                        )
+                    )
 
-    name = ""
-    """This is the module name you want to run"""
+            else:
+                if name in mod.__class__.__dict__ and inspect.isdatadescriptor(mod.__class__.__dict__[name]):
+                    # https://stackoverflow.com/a/30578922/5006
+                    monkey_class = self.patch_class(
+                        mod.__class__,
+                        **{name: patch}
+                    )
+                    mod.__class__ = monkey_class
+
+                else:
+                    setattr(mod, name, patch)
+
+        return mod
+
+    def patch_class(self, mod, patches=None, **kwargs_patches):
+        """Helper function called from .patch() that will patch a class type object"""
+        if not mod:
+            raise ValueError("mod is empty")
+
+        if not patches: patches = {}
+        patches.update(kwargs_patches) # combine both dicts
+
+        def copy_dict(mod):
+            d = {}
+            for k, v in mod.__dict__.items():
+                if k.startswith("__"):
+                    d[k] = v
+                else:
+                    if inspect.isroutine(v):
+                        d[k] = v
 
-    def __init__(self, name="", cwd="", environ=None):
-        if name:
-            self.name = name
+                    elif inspect.isdatadescriptor(v):
+                        d[k] = v
 
-        if not self.name:
-            raise ValueError("No name specified")
+                    else:
+                        d[k] = copy.deepcopy(v)
+            return d
 
-        super(ModuleCommand, self).__init__(None, cwd=cwd, environ=environ)
+        class_name = '{}Patched'.format(mod.__name__)
 
-    def create_cmd(self, command, arg_str):
-        if isinstance(command, basestring):
-            ret = "{} {} {}".format(self.cmd_prefix, self.name, command)
+        # http://stackoverflow.com/questions/9541025/how-to-copy-a-python-class
+        mod_patched = type(
+            class_name,
+            tuple([mod] + list(mod.__bases__)),
+            #{k: copy.deepcopy(v) for k, v in mod.__dict__.items()}
+            copy_dict(mod)
+        )
+        for name, patch in patches.items():
+            # make sure we have a callable if we need a callable
+            o = getattr(mod_patched, name, None)
+            if inspect.isroutine(o) and not inspect.isroutine(patch):
+                # so I ran into an issue with binding here, the value of patch was
+                # being changed on each iteration and so when I then called it the final
+                # value of patch was being returned instead of the value of patch
+                # when the lambda was created. a partial was the only way I could
+                # figure out how to make it work and return the correct value
+                patch = functools.partial(lambda *a, **kw: kw["__patch"], __patch=patch)
+
+            setattr(mod_patched, name, patch)
+
+        return mod_patched
+
+    def patch_module(self, mod, patches=None, **kwargs_patches):
+        """Helper function called from .patch() that will patch a module"""
+        if not mod:
+            raise ValueError("mod is empty")
+
+        if not patches: patches = {}
+        patches.update(kwargs_patches) # combine both dicts
+
+        # now we need to find the full module path so we can reload it
+        if inspect.ismodule(mod):
+            mod_name = mod.__name__
+            mpath = inspect.getsourcefile(mod)
+            mfile = mpath
 
         else:
-            ret = re.split(r"\s+", self.cmd_prefix)
-            ret.append(self.name)
-            if command:
-                ret.extend(command)
-
-        return super(ModuleCommand, self).create_cmd(ret, arg_str)
-
-
-class FileCommand(ModuleCommand):
-    """This will add the .py to a script so you don't have to
-
-    an example might be best to understand how the command gets put together
-
-    Let's say you wanted to run this path:
-
-        /foo/bar/program.py
-
-    You could configure this class like this:
-
-        class ProgamCommand(FileCommand):
-            script_prefix = "/foo/bar"
-            script_postfix = ".py"
-            name = "program"
-
-    Then when you need to run program.py, you only need to do:
-
-        p = ProgramCommand()
-        p.run() # runs "python /foo/bar/program.py"
-
-    But you also could run it:
-
-        p = FileCommand("/foo/bar/program.py")
+            mod_name = mod
 
-    or:
-        class ProgamCommand(FileCommand):
-            script_prefix = "/foo/bar"
+            # http://stackoverflow.com/questions/4907054/
+            def find_mod_path(p):
+                if '.' in p:
+                    p, m = p.rsplit('.', 1)
+                    imod_path = find_mod_path(p)
+                    mod_path = os.path.join(imod_path, m)
+
+                else:
+                    # we fudge the paths a bit to make sure current working directory is
+                    # also checked
+                    paths = [os.getcwd()]
+                    paths.extend(sys.path)
+                    # imp is deprecated in python 3, see:
+                    # https://stackoverflow.com/questions/35288021/what-is-the-equivalent-of-imp-find-module-in-importlib
+                    if is_py2:
+                        _, mod_path, _ = imp.find_module(p, paths)
 
-        p = ProgramCommand("program")
-    """
-    cmd_prefix = sys.executable
-    """If you have a space in the executable path that might be really bad"""
-
-    script_prefix = ""
-    """this will be prepended to the passed in script on initialization"""
-
-    script_postfix = ""
-    """this will be appended to the passed in script on initialization"""
-
-    def __init__(self, fileroot="", cwd="", environ=None):
-        if fileroot:
-            self.name = fileroot
-
-        if not self.name:
-            raise ValueError("no name found")
-
-        path = self.name
-        if self.script_prefix and not fileroot.startswith(self.script_prefix):
-            path = os.path.join(self.script_prefix.rstrip("/"), fileroot)
+                    else:
+                        spec = importlib.machinery.PathFinder().find_spec(p, paths)
+                        if spec.submodule_search_locations:
+                            mod_path = spec.submodule_search_locations[0]
+                        else:
+                            mod_path = spec.origin
+
+                return mod_path
+
+            mpath = find_mod_path(mod_name)
+
+            mfile = mpath
+            # figure out if we have a package or a module and set the appropriate file
+            if os.path.isdir(mpath):
+                mfile = os.path.join(mpath, '__init__.py')
 
-        if self.script_postfix and not path.endswith(self.script_postfix):
-            path += self.script_postfix
+            else:
+                if not mfile.endswith(".py"):
+                    mfile = '{}.py'.format(mpath)
 
-        super(FileCommand, self).__init__(path, cwd=cwd, environ=environ)
+        mname = self.get_module_name(prefix=mod_name)
+        #mname = '{}_{}'.format(mod_name, get_ascii(8))
+        if is_py2:
+            m = imp.load_source(mname, mfile)
+        else:
+            # ugh, this is deprecated in 3.4 (though it isn't throwing a warning
+            m = importlib.machinery.SourceFileLoader(mname, mfile).load_module()
+            # https://docs.python.org/3/library/importlib.html#importing-a-source-file-directly
+
+    #         loader = importlib.machinery.SourceFileLoader(mname, mfile)
+    #         loaded = types.ModuleType(loader.name)
+    #         m = loader.exec_module(loaded)
+
+        # go through and apply all the patches
+        for patch_name, patch in patches.items():
+            if "." in patch_name:
+                parts = patch_name.split(".")
+                sm = getattr(m, parts[0], None)
+                if sm:
+                    setattr(m, parts[0], self.patch_module(sm, {".".join(parts[1:]): patch}))
+                else:
+                    setattr(m, parts[0], Mock(**{parts[-1]: patch}))
+            else:
+                # if we're patching a function and patch isn't a function then make
+                # it a function
+                o = getattr(m, patch_name, None)
+                if inspect.isroutine(o) and not inspect.isroutine(patch):
+                    # lambda binding issue, see the explanation in patch_class why I'm
+                    # using partial here
+                    patch = functools.partial(lambda *a, **kw: kw["__patch"], __patch=patch)
+
+                setattr(m, patch_name, patch)
+
+        return m
+
+    def patch(self, mod, patches=None, **kwargs_patches):
+        """import module_name and apply the patches to it
+
+        :param mod: string|module|class|instance, the name of the thing you are patching
+        :param patches: dict, the keys are functions, classes, or modules that should be
+        patched in the module, the value is the patched value you want to replace the
+        key with
+        :returns: module|object, if you pass in an object, return the object, otherwise
+            return the module
+        """
+        if isinstance(mod, basestring):
+            m = self.patch_module(mod, patches=patches, **kwargs_patches)
 
+        elif inspect.ismodule(mod):
+            m = self.patch_module(mod, patches=patches, **kwargs_patches)
 
-###############################################################################
-# testdata functions
-###############################################################################
-class ClientData(TestData):
-    def run(self, cmd, arg_str="", cwd="", environ=None, **kwargs):
-        """Run a command on the command line
-
-        :param cmd: mixed, the command you want to run
-        :param arg_str: string, extra flags that will be appended to the cmd
-        :param **kwargs: allows you to pass into underlying Command.run() method
-        :returns: string, the output from the command
-        """
-        if hasattr(cmd, "run"):
-            ret = cmd.run(arg_str, cwd=cwd, environ=environ, **kwargs)
+        elif inspect.isclass(mod):
+            m = self.patch_class(mod, patches=patches, **kwargs_patches)
 
         else:
-            cmd = Command(cmd, cwd=cwd, environ=environ)
-            ret = cmd.run(arg_str, **kwargs)
+            m = self.patch_instance(mod, patches=patches, **kwargs_patches) 
 
-        return ret
+        return m
 
-    def fetch(self, url, body=None, query=None, **kwargs):
-        """fetch a url
+    def mock_class(self, name="", patches=None, **kwargs_patches):
+        """create a class with the given method and properties
 
-        :Example:
-            # make a simple get request
-            c = testdata.fetch("http://example.com/foo/bar")
+        :param name: string, the name of the class, default is just a random classname
+        :param patches: dict, keys are attributes mapped to their values 
+        :param **kwargs_patches: dict, keys will be attributes on the object
+        :returns: type, the object
+        """
+        if not patches: patches = {}
+        patches.update(kwargs_patches)
+        return type(self.get_classname(name=name), (Mock,), patches)
 
-            # make a request with a cookie
-            c = testdata.fetch("http://example.com/foo/bar", cookies={"foo": "1"})
+    def mock_instance(self, name="", patches=None, **kwargs_patches):
+        """This is the same as mock_class but returns an instance of that class
 
-            # make a request with a different method
-            c = testdata.fetch("http://example.com/foo/bar", method="PUT")
+        see mock_class() docs"""
+        return self.mock_class(name)(patches, **kwargs_patches)
 
-            # make a POST request
-            c = testdata.fetch("http://example.com/foo/bar", {"foo": 1})
+    def mock(self, patches=None, **kwargs_patches):
+        """Create a mocked object that tries to be really magical
 
-            # make a json POST request
-            c = testdata.fetch("http://example.com/foo/bar", {"foo": 1}, json=True)
+        This is different than mock_instance because it creates an object that uses a lot
+        of magic to try and be a jack of all trades
 
-        :param url: string, the full url you want to request
-        :param body: dict, the body you want to POST, pass None for GET request
-        :param query: dict, if you want to attach query params with ?
-        :param **kwargs: anything else you want to pass to the underlying HTTP object
-            method -- string, things like HEAD, or PUT
-            cookies -- dict, the cookies you want to pass to the server
-        :returns: HTTPResponse, has .code, .body, and other properties and methods
+        :returns: Mock instance
         """
-        c = HTTP(url, **kwargs)
-        method = kwargs.pop("method", "")
-        if method:
-            ret = c.fetch(method, url, query, body, **kwargs)
-
-        else:
-            if body is None:
-                ret = c.get(url, query, **kwargs)
-            else:
-                ret = c.post(url, body, query=query, **kwargs)
-
-        return ret
+        return Mock(patches, **kwargs_patches)
```

### Comparing `testdata-6.1.1/testdata/config.py` & `testdata-6.2.0/testdata/config.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/data/__init__.py` & `testdata-6.2.0/testdata/data/__init__.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/data/favicon.ico` & `testdata-6.2.0/testdata/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/data/static.gif` & `testdata-6.2.0/testdata/data/static.gif`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/data/static.png` & `testdata-6.2.0/testdata/data/static.png`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/data/usa/cities.py` & `testdata-6.2.0/testdata/data/usa/cities.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/data/usa/states.py` & `testdata-6.2.0/testdata/data/usa/states.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/data/usa/zipcodes.py` & `testdata-6.2.0/testdata/data/usa/zipcodes.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/output.py` & `testdata-6.2.0/testdata/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,22 +92,27 @@
         """create an instance of this stream capture class
 
         :param stream: file object, the stream this instance is wrapping, if this
             is passed in then this will save the string and also pass the string
             to this stream
         """
         self.heap = []
+        self.heaptimes = set()
         self.stream = stream
 
     def write(self, s):
-        # I originally was using time.time() and sometimes that would return the
-        # same value on subsequent calls
+        # I originally was using time.time_ns() and sometimes that would return
+        # the same value on subsequent calls
         # https://stackoverflow.com/questions/1938048/
         # https://stackoverflow.com/a/38256446
-        t = time.process_time_ns()
+        #t = time.process_time_ns()
+        t = time.time_ns()
+        while t in self.heaptimes:
+            t += 1
+        self.heaptimes.add(t)
         hpush(self.heap, (t, s))
         if self.stream:
             self.stream.write(s)
 
     def __iter__(self):
         for t, s in self.heap:
             yield s
@@ -267,32 +272,35 @@
 
 
 ###############################################################################
 # testdata functions
 ###############################################################################
 class OutputData(TestData):
     def basic_logging(self, **kwargs):
-        """Lots of times, in tests, I have to add a basic logger, it's basically the
-        same code over and over again, this will just make that a little easier to do
+        """Lots of times, in tests, I have to add a basic logger, it's basically
+        the same code over and over again, this will just make that a little
+        easier to do
 
         :example:
             import testdata
             testdata.basic_logging() # near top of file
 
-        :param **kwargs: key/val, these will be passed into logger.basicConfig method
+        :param **kwargs: key/val, these will be passed into logger.basicConfig
+            method
         """
         datatypes.logging.quick_config(**kwargs)
 
     def capture(stdout=True, stderr=True, loggers=True, *args, **kwargs):
         """Capture stdout and stderr so you can inspect it
 
-        this is handy for tests when you are trying to figure out if logging or whatnot
-        is doing the correct thing
+        this is handy for tests when you are trying to figure out if logging or
+        whatnot is doing the correct thing
 
-        I'd always wanted something similar to php's output buffering ob_start() method
+        I'd always wanted something similar to php's output buffering ob_start()
+        method
         http://www.php.net/manual/en/function.ob-start.php
 
         :example:
             with testdata.capture() as c:
                 print("foo")
             if "foo" in c:
                 print("foo was captured")
```

### Comparing `testdata-6.1.1/testdata/path.py` & `testdata-6.2.0/testdata/path.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/server.py` & `testdata-6.2.0/testdata/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         :example:
             s = WebServer("/some/path")
             print(s.url("foo.txt")) # http://localhost:PORT/foo.txt
 
         :param *parts: list, the path parts you will add to the scheme://netloc
         :returns: the full url scheme://netloc/parts
         """
-        # DEPRECATED? this extends Url so you can use al Url's helper methods
+        # DEPRECATED? this class extends Url so you can use all Url's helper methods
         return self.child(*parts, **kwargs)
 
 
 class CookieServer(CallbackServer):
     """This will write and read cookies to make sure a client is passing cookies
     correctly to the server
```

### Comparing `testdata-6.1.1/testdata/service.py` & `testdata-6.2.0/testdata/service.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/test.py` & `testdata-6.2.0/testdata/test.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/types/datetime.py` & `testdata-6.2.0/testdata/types/datetime.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/types/mapping.py` & `testdata-6.2.0/testdata/types/mapping.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/types/number.py` & `testdata-6.2.0/testdata/types/number.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/types/sequence.py` & `testdata-6.2.0/testdata/types/sequence.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/types/string.py` & `testdata-6.2.0/testdata/types/string.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata/user.py` & `testdata-6.2.0/testdata/user.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/testdata.egg-info/PKG-INFO` & `testdata-6.2.0/testdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testdata
-Version: 6.1.1
+Version: 6.2.0
 Summary: Easily generate random unicode test data among other things
 Home-page: http://github.com/Jaymon/testdata
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `testdata-6.1.1/testdata.egg-info/SOURCES.txt` & `testdata-6.2.0/testdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/tests/base_test.py` & `testdata-6.2.0/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/tests/mocking_test.py` & `testdata-6.2.0/tests/mocking_test.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/tests/output_test.py` & `testdata-6.2.0/tests/output_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,17 @@
         self.assertTrue("bar" in capture)
         self.assertTrue("foo\nbar" in capture)
 
     def test_capture_mixed(self):
         capture = Capture(loggers=False)
         with capture():
             print("foo stdout")
-            print('bar stderr', file=sys.stderr)
+            print("bar stderr", file=sys.stderr)
             print("baz stdout")
-            print('che stderr', file=sys.stderr)
+            print("che stderr", file=sys.stderr)
 
         output = "foo stdout\nbar stderr\nbaz stdout\nche stderr\n"
         self.assertTrue(output in capture)
         self.assertTrue(output == capture)
         self.assertFalse(output < capture)
         self.assertFalse(output > capture)
         self.assertFalse(output != capture)
```

### Comparing `testdata-6.1.1/tests/path_test.py` & `testdata-6.2.0/tests/path_test.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/tests/server_test.py` & `testdata-6.2.0/tests/server_test.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/tests/test_test.py` & `testdata-6.2.0/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/tests/testdata_test.py` & `testdata-6.2.0/tests/testdata_test.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/tests/threading_test.py` & `testdata-6.2.0/tests/threading_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,18 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals, division, print_function, absolute_import
 import time
 
-from testdata.threading import Thread, Deque, Tail
+from testdata.threading import Thread, Tail
 from testdata.compat import *
 from testdata.client import Command
 
 from . import TestCase, testdata
 
 
-class DequeTest(TestCase):
-    def test_lifecycle(self):
-        d = Deque(2)
-        self.assertEqual(0, len(d))
-
-        d.append(1)
-        self.assertEqual(1, len(d))
-
-        d.append(2)
-        self.assertEqual(2, len(d))
-
-        d.append(3)
-        self.assertEqual(2, len(d))
-
-        self.assertEqual(2, d[0])
-        self.assertEqual(3, d[1])
-
-
 class Thread3Test(TestCase):
     def setUp(self):
         # !!! this test can trigger a keyboard interrupt error, but I normally don't
         # need to do that so only comment out if needed
         self.skip_test()
         pass
```

### Comparing `testdata-6.1.1/tests/types_test.py` & `testdata-6.2.0/tests/types_test.py`

 * *Files identical despite different names*

### Comparing `testdata-6.1.1/tests/user_test.py` & `testdata-6.2.0/tests/user_test.py`

 * *Files identical despite different names*

