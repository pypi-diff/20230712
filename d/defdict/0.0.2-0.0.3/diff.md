# Comparing `tmp/defdict-0.0.2.tar.gz` & `tmp/defdict-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defdict-0.0.2.tar", last modified: Mon Jul  3 23:17:07 2023, max compression
+gzip compressed data, was "defdict-0.0.3.tar", last modified: Wed Jul 12 20:03:00 2023, max compression
```

## Comparing `defdict-0.0.2.tar` & `defdict-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 23:17:07.120406 defdict-0.0.2/
--rw-rw-rw-   0        0        0       26 2023-07-03 23:15:19.000000 defdict-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      390 2023-07-03 23:17:07.120406 defdict-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 23:17:07.121406 defdict-0.0.2/defdict/
--rw-rw-rw-   0        0        0    12243 2023-07-03 02:24:52.000000 defdict-0.0.2/defdict/DataFormat.py
--rw-rw-rw-   0        0        0    27850 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/DefDict.py
--rw-rw-rw-   0        0        0     4090 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/MapRule.py
--rw-rw-rw-   0        0        0     1981 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/SpaceDefinition.py
--rw-rw-rw-   0        0        0      400 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/SpeedTest.py
--rw-rw-rw-   0        0        0     6151 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/StdConversion.py
--rw-rw-rw-   0        0        0     2426 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/StdDefinitions.py
--rw-rw-rw-   0        0        0     3133 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/StdUnit.py
--rw-rw-rw-   0        0        0     2181 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/Tmat.py
--rw-rw-rw-   0        0        0    15323 2023-07-03 02:24:52.000000 defdict-0.0.2/defdict/UnitType.py
--rw-rw-rw-   0        0        0      331 2023-07-03 04:40:06.000000 defdict-0.0.2/defdict/__init__.py
--rw-rw-rw-   0        0        0       79 2023-07-03 23:17:07.121406 defdict-0.0.2/defdict/_static_version.py
--rw-rw-rw-   0        0        0     6071 2023-07-03 04:13:13.000000 defdict-0.0.2/defdict/_version.py
--rw-rw-rw-   0        0        0      165 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/system_keys.py
-drwxrwxrwx   0        0        0        0 2023-07-03 23:17:07.120406 defdict-0.0.2/defdict.egg-info/
--rw-rw-rw-   0        0        0      390 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       28 2023-07-03 02:55:19.000000 defdict-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 23:17:07.121406 defdict-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1690 2023-07-03 23:16:53.000000 defdict-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:03:00.628340 defdict-0.0.3/
+-rw-rw-rw-   0        0        0       26 2023-07-03 23:15:19.000000 defdict-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      448 2023-07-12 20:03:00.628340 defdict-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7482 2023-07-03 03:13:41.000000 defdict-0.0.3/ReadMe.md
+drwxrwxrwx   0        0        0        0 2023-07-12 20:03:00.629341 defdict-0.0.3/defdict/
+-rw-rw-rw-   0        0        0    12243 2023-07-03 02:24:52.000000 defdict-0.0.3/defdict/DataFormat.py
+-rw-rw-rw-   0        0        0    27915 2023-07-12 01:26:27.000000 defdict-0.0.3/defdict/DefDict.py
+-rw-rw-rw-   0        0        0     4090 2023-07-03 02:55:19.000000 defdict-0.0.3/defdict/MapRule.py
+-rw-rw-rw-   0        0        0     1981 2023-07-03 02:55:19.000000 defdict-0.0.3/defdict/SpaceDefinition.py
+-rw-rw-rw-   0        0        0      400 2023-07-03 02:55:19.000000 defdict-0.0.3/defdict/SpeedTest.py
+-rw-rw-rw-   0        0        0     6151 2023-07-03 02:55:19.000000 defdict-0.0.3/defdict/StdConversion.py
+-rw-rw-rw-   0        0        0     2426 2023-07-03 02:55:19.000000 defdict-0.0.3/defdict/StdDefinitions.py
+-rw-rw-rw-   0        0        0     3133 2023-07-03 02:55:19.000000 defdict-0.0.3/defdict/StdUnit.py
+-rw-rw-rw-   0        0        0     2181 2023-07-03 02:55:19.000000 defdict-0.0.3/defdict/Tmat.py
+-rw-rw-rw-   0        0        0    15323 2023-07-03 02:24:52.000000 defdict-0.0.3/defdict/UnitType.py
+-rw-rw-rw-   0        0        0      408 2023-07-05 02:31:24.000000 defdict-0.0.3/defdict/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-07-12 20:03:00.629341 defdict-0.0.3/defdict/_static_version.py
+-rw-rw-rw-   0        0        0     6071 2023-07-03 04:13:13.000000 defdict-0.0.3/defdict/_version.py
+-rw-rw-rw-   0        0        0      165 2023-07-03 02:55:19.000000 defdict-0.0.3/defdict/system_keys.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:03:00.628340 defdict-0.0.3/defdict.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-07-12 20:03:00.000000 defdict-0.0.3/defdict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-07-12 20:03:00.000000 defdict-0.0.3/defdict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 20:03:00.000000 defdict-0.0.3/defdict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-12 20:03:00.000000 defdict-0.0.3/defdict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 20:03:00.000000 defdict-0.0.3/defdict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       28 2023-07-03 02:55:19.000000 defdict-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 20:03:00.628340 defdict-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1759 2023-07-12 20:02:43.000000 defdict-0.0.3/setup.py
```

### Comparing `defdict-0.0.2/defdict/DataFormat.py` & `defdict-0.0.3/defdict/DataFormat.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.2/defdict/DefDict.py` & `defdict-0.0.3/defdict/DefDict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import logging
 import inspect
 import numpy as np
 from typing import Any
-from UnitType import UnitType
+from .UnitType import UnitType
 SEPARATOR = '.'
 
 class DefDict:
     reserved = ['get', 'set', 'keys', 'list', 'list_keys', 'ndtall']
     def __init__(self, definition=None, dtype=Any, name=None, prefixes=True, suffixes=True, format_rule=None, shape=None, rules=None, nested_def=True):
         self._definition = dict()
         self._data = dict()
@@ -89,15 +89,17 @@
     def list_keys(self):
         return list(self._data.keys())
 
     def get(self, key=None):
         if key is None:
             ret = self.list()[0]    # get the first element when no key has been specified
         else:
-            ret = self._data[key][0]
+            ret = self._data.get(key)
+            if ret is not None:
+                ret = ret[0]
         return ret
 
     def dict(self):
         ret = {}
         for k, v in self.data.items():
             if isinstance(v, DefDict):
                 ret[k] = v.dict()
```

### Comparing `defdict-0.0.2/defdict/MapRule.py` & `defdict-0.0.3/defdict/MapRule.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.2/defdict/SpaceDefinition.py` & `defdict-0.0.3/defdict/SpaceDefinition.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.2/defdict/StdConversion.py` & `defdict-0.0.3/defdict/StdConversion.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.2/defdict/StdDefinitions.py` & `defdict-0.0.3/defdict/StdDefinitions.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.2/defdict/StdUnit.py` & `defdict-0.0.3/defdict/StdUnit.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.2/defdict/Tmat.py` & `defdict-0.0.3/defdict/Tmat.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.2/defdict/UnitType.py` & `defdict-0.0.3/defdict/UnitType.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.2/defdict/_version.py` & `defdict-0.0.3/defdict/_version.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.2/setup.py` & `defdict-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,19 @@
 
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='defdict',
-    version='0.0.2',
+    version='0.0.3',
     cmdclass=cmdclass,
     description=get_metadata('description'),
     url=get_metadata("url"),
+    project_urls={'GitHub': 'https://github.com/Suke0811/DefDict'},
     author=get_metadata('author'),
     license='LGPLv3',
     packages=find_packages(include=['defdict', 'defdict.*']),
     install_requires=requirements,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Robot Framework',
```

