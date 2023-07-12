# Comparing `tmp/voicemeeter_api-2.3.0.tar.gz` & `tmp/voicemeeter_api-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.3.0.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.3.1.tar", max compression
```

## Comparing `voicemeeter_api-2.3.0.tar` & `voicemeeter_api-2.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.0/LICENSE
--rw-r--r--   0        0        0     1102 2023-07-11 17:25:08.856740 voicemeeter_api-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    18140 2023-07-11 17:21:40.302191 voicemeeter_api-2.3.0/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.0/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.3.0/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4207 2023-07-10 19:16:03.423527 voicemeeter_api-2.3.0/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.3.0/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.3.0/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.3.0/voicemeeterlib/device.py
--rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.0/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.0/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.3.0/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.3.0/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.3.0/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.3.0/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.3.0/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.0/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-10 14:28:38.873267 voicemeeter_api-2.3.0/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.0/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    12109 2023-07-11 16:45:26.140521 voicemeeter_api-2.3.0/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.3.0/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.3.0/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2978 2023-07-10 02:00:50.034407 voicemeeter_api-2.3.0/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     1971 2023-06-30 17:58:26.046029 voicemeeter_api-2.3.0/voicemeeterlib/util.py
--rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.3.0/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    17953 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.1/LICENSE
+-rw-r--r--   0        0        0     1102 2023-07-12 03:48:54.989633 voicemeeter_api-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0    18156 2023-07-11 18:43:59.775001 voicemeeter_api-2.3.1/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.1/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.3.1/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4207 2023-07-10 19:16:03.423527 voicemeeter_api-2.3.1/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.3.1/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.3.1/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.3.1/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.1/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.1/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.3.1/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.3.1/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.3.1/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.3.1/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.3.1/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.1/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-10 14:28:38.873267 voicemeeter_api-2.3.1/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.1/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    12243 2023-07-12 03:43:21.313261 voicemeeter_api-2.3.1/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.3.1/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.3.1/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2978 2023-07-10 02:00:50.034407 voicemeeter_api-2.3.1/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     2449 2023-07-12 01:53:12.508493 voicemeeter_api-2.3.1/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.3.1/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    17969 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.1/PKG-INFO
```

### Comparing `voicemeeter_api-2.3.0/LICENSE` & `voicemeeter_api-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/pyproject.toml` & `voicemeeter_api-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.3.0"
+version = "2.3.1"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [{ include = "voicemeeterlib" }]
```

### Comparing `voicemeeter_api-2.3.0/README.md` & `voicemeeter_api-2.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -687,16 +687,16 @@
     }
 )
 ```
 
 Or for each class you may do:
 
 ```python
-vm.strip[0].apply(mute: True, gain: 3.2, A1: True)
-vm.vban.outstream[0].apply(on: True, name: 'streamname', bit: 24)
+vm.strip[0].apply({"mute": True, "gain": 3.2, "A1": True})
+vm.vban.outstream[0].apply({"on": True, "name": "streamname", "bit": 24})
 ```
 
 ## Config Files
 
 `vm.apply_config(configname)`
 
 You may load config files in TOML format.
```

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/bus.py` & `voicemeeter_api-2.3.1/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.3.1/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/command.py` & `voicemeeter_api-2.3.1/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/config.py` & `voicemeeter_api-2.3.1/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/device.py` & `voicemeeter_api-2.3.1/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/error.py` & `voicemeeter_api-2.3.1/voicemeeterlib/error.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/event.py` & `voicemeeter_api-2.3.1/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/factory.py` & `voicemeeter_api-2.3.1/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/inst.py` & `voicemeeter_api-2.3.1/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/iremote.py` & `voicemeeter_api-2.3.1/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/kinds.py` & `voicemeeter_api-2.3.1/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.3.1/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/meta.py` & `voicemeeter_api-2.3.1/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/misc.py` & `voicemeeter_api-2.3.1/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/recorder.py` & `voicemeeter_api-2.3.1/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/remote.py` & `voicemeeter_api-2.3.1/voicemeeterlib/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import ctypes as ct
 import logging
 import time
 from abc import abstractmethod
 from queue import Queue
 from typing import Iterable, NoReturn, Optional, Union
 
@@ -9,15 +10,15 @@
 from .error import CAPIError, VMError
 from .event import Event
 from .inst import bits
 from .kinds import KindId
 from .misc import Midi, VmGui
 from .subject import Subject
 from .updater import Producer, Updater
-from .util import grouper, polling, script
+from .util import deep_merge, grouper, polling, script
 
 logger = logging.getLogger(__name__)
 
 
 class Remote(CBindings):
     """Base class responsible for wrapping the C Remote API"""
 
@@ -302,22 +303,26 @@
     def apply_config(self, name):
         """applies a config from memory"""
         ERR_MSG = (
             f"No config with name '{name}' is loaded into memory",
             f"Known configs: {list(self.configs.keys())}",
         )
         try:
-            config = self.configs[name].copy()
+            config = self.configs[name]
         except KeyError as e:
             self.logger.error(("\n").join(ERR_MSG))
             raise VMError(("\n").join(ERR_MSG)) from e
 
         if "extends" in config:
-            extended = config.pop("extends")
-            config = self.configs[extended] | config
+            extended = config["extends"]
+            config = {
+                k: v
+                for k, v in deep_merge(self.configs[extended], config)
+                if k not in ("extends")
+            }
             self.logger.debug(
                 f"profile '{name}' extends '{extended}', profiles merged.."
             )
         self.apply(config)
         self.logger.info(f"Profile '{name}' applied!")
 
     def logout(self) -> NoReturn:
```

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/strip.py` & `voicemeeter_api-2.3.1/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/subject.py` & `voicemeeter_api-2.3.1/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/updater.py` & `voicemeeter_api-2.3.1/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/util.py` & `voicemeeter_api-2.3.1/voicemeeterlib/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import functools
 from itertools import zip_longest
 from typing import Iterator
 
 
 def polling(func):
     """
@@ -66,7 +67,21 @@
 
 def grouper(n, iterable, fillvalue=None):
     """
     Group elements of an iterable by sets of n length
     """
     args = [iter(iterable)] * n
     return zip_longest(fillvalue=fillvalue, *args)
+
+
+def deep_merge(dict1, dict2):
+    """Generator function for deep merging two dicts"""
+    for k in set(dict1) | set(dict2):
+        if k in dict1 and k in dict2:
+            if isinstance(dict1[k], dict) and isinstance(dict2[k], dict):
+                yield k, dict(deep_merge(dict1[k], dict2[k]))
+            else:
+                yield k, dict2[k]
+        elif k in dict1:
+            yield k, dict1[k]
+        else:
+            yield k, dict2[k]
```

### Comparing `voicemeeter_api-2.3.0/voicemeeterlib/vban.py` & `voicemeeter_api-2.3.1/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.0/PKG-INFO` & `voicemeeter_api-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.3.0
+Version: 2.3.1
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -704,16 +704,16 @@
     }
 )
 ```
 
 Or for each class you may do:
 
 ```python
-vm.strip[0].apply(mute: True, gain: 3.2, A1: True)
-vm.vban.outstream[0].apply(on: True, name: 'streamname', bit: 24)
+vm.strip[0].apply({"mute": True, "gain": 3.2, "A1": True})
+vm.vban.outstream[0].apply({"on": True, "name": "streamname", "bit": 24})
 ```
 
 ## Config Files
 
 `vm.apply_config(configname)`
 
 You may load config files in TOML format.
```

