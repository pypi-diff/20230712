# Comparing `tmp/tahoma_gpt-0.0.3.tar.gz` & `tmp/tahoma_gpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma_gpt-0.0.3.tar", last modified: Wed Jul 12 01:53:52 2023, max compression
+gzip compressed data, was "tahoma_gpt-0.0.4.tar", last modified: Wed Jul 12 01:59:56 2023, max compression
```

## Comparing `tahoma_gpt-0.0.3.tar` & `tahoma_gpt-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:53:52.979690 tahoma_gpt-0.0.3/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma_gpt-0.0.3/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      148 2023-07-12 01:27:33.000000 tahoma_gpt-0.0.3/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 01:53:52.979789 tahoma_gpt-0.0.3/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:59.000000 tahoma_gpt-0.0.3/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:25.000000 tahoma_gpt-0.0.3/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1212 2023-07-12 01:24:52.000000 tahoma_gpt-0.0.3/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 01:52:47.000000 tahoma_gpt-0.0.3/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-07-12 01:53:52.980116 tahoma_gpt-0.0.3/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma_gpt-0.0.3/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:53:52.976291 tahoma_gpt-0.0.3/tahoma_gpt/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      138 2023-07-12 01:21:46.000000 tahoma_gpt-0.0.3/tahoma_gpt/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 01:53:38.000000 tahoma_gpt-0.0.3/tahoma_gpt/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 01:45:52.000000 tahoma_gpt-0.0.3/tahoma_gpt/__version__.py~
--rwxrwx---   0 neptune   (1000) neptune   (1000)    37481 2023-07-12 01:25:54.000000 tahoma_gpt-0.0.3/tahoma_gpt/tahoma_gpt.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:53:52.979385 tahoma_gpt-0.0.3/tahoma_gpt/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma_gpt-0.0.3/tahoma_gpt/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma_gpt-0.0.3/tahoma_gpt/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:53:52.978598 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      454 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       58 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       11 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:59:56.991402 tahoma_gpt-0.0.4/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma_gpt-0.0.4/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      148 2023-07-12 01:27:33.000000 tahoma_gpt-0.0.4/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 01:59:56.991543 tahoma_gpt-0.0.4/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:59.000000 tahoma_gpt-0.0.4/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:25.000000 tahoma_gpt-0.0.4/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1212 2023-07-12 01:24:52.000000 tahoma_gpt-0.0.4/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 01:52:47.000000 tahoma_gpt-0.0.4/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-07-12 01:59:56.991900 tahoma_gpt-0.0.4/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma_gpt-0.0.4/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:59:56.987850 tahoma_gpt-0.0.4/tahoma_gpt/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      138 2023-07-12 01:21:46.000000 tahoma_gpt-0.0.4/tahoma_gpt/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 01:59:32.000000 tahoma_gpt-0.0.4/tahoma_gpt/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 01:53:38.000000 tahoma_gpt-0.0.4/tahoma_gpt/__version__.py~
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    37464 2023-07-12 01:59:04.000000 tahoma_gpt-0.0.4/tahoma_gpt/tahoma_gpt.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:59:56.991048 tahoma_gpt-0.0.4/tahoma_gpt/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma_gpt-0.0.4/tahoma_gpt/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma_gpt-0.0.4/tahoma_gpt/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:59:56.990178 tahoma_gpt-0.0.4/tahoma_gpt.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 01:59:56.000000 tahoma_gpt-0.0.4/tahoma_gpt.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      454 2023-07-12 01:59:56.000000 tahoma_gpt-0.0.4/tahoma_gpt.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-07-12 01:59:56.000000 tahoma_gpt-0.0.4/tahoma_gpt.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       58 2023-07-12 01:59:56.000000 tahoma_gpt-0.0.4/tahoma_gpt.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 01:59:56.000000 tahoma_gpt-0.0.4/tahoma_gpt.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       11 2023-07-12 01:59:56.000000 tahoma_gpt-0.0.4/tahoma_gpt.egg-info/top_level.txt
```

### Comparing `tahoma_gpt-0.0.3/LICENSE` & `tahoma_gpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.3/PKG-INFO` & `tahoma_gpt-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma_gpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma-gpt
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma-gpt/issues
 Keywords: tahoma_gpt,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tahoma_gpt-0.0.3/PYPI_README.md` & `tahoma_gpt-0.0.4/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.3/README.md` & `tahoma_gpt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.3/pyproject.toml` & `tahoma_gpt-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.3/tahoma_gpt/tahoma_gpt.py` & `tahoma_gpt-0.0.4/tahoma_gpt/tahoma_gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 import openai
 import datetime
 import os
 import requests
 import subprocess
 import asyncio
-import pyoverkiz
 import time
 from inputimeout import inputimeout, TimeoutOccurred
 
 
 import sys
 from tahoma_gpt import __version__
```

### Comparing `tahoma_gpt-0.0.3/tahoma_gpt.egg-info/PKG-INFO` & `tahoma_gpt-0.0.4/tahoma_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma-gpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma-gpt
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma-gpt/issues
 Keywords: tahoma_gpt,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

