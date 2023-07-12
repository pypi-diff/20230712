# Comparing `tmp/vban_cmd-2.3.0.tar.gz` & `tmp/vban_cmd-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.3.0.tar", max compression
+gzip compressed data, was "vban_cmd-2.3.1.tar", max compression
```

## Comparing `vban_cmd-2.3.0.tar` & `vban_cmd-2.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.3.0/LICENSE
--rw-r--r--   0        0        0      951 2023-07-11 17:25:21.228891 vban_cmd-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    12527 2023-07-11 18:49:38.369576 vban_cmd-2.3.0/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.3.0/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.3.0/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.3.0/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.3.0/vban_cmd/config.py
--rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.3.0/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.3.0/vban_cmd/event.py
--rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.3.0/vban_cmd/factory.py
--rw-r--r--   0        0        0     4115 2023-07-05 18:08:51.113607 vban_cmd-2.3.0/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.3.0/vban_cmd/kinds.py
--rw-r--r--   0        0        0     1150 2023-07-08 06:13:52.713834 vban_cmd-2.3.0/vban_cmd/macrobutton.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.3.0/vban_cmd/meta.py
--rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.3.0/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.3.0/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.3.0/vban_cmd/subject.py
--rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban_cmd-2.3.0/vban_cmd/util.py
--rw-r--r--   0        0        0     4320 2023-07-08 06:27:12.206963 vban_cmd-2.3.0/vban_cmd/vban.py
--rw-r--r--   0        0        0     7280 2023-07-11 17:55:51.111211 vban_cmd-2.3.0/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.3.0/vban_cmd/worker.py
--rw-r--r--   0        0        0    12664 1970-01-01 00:00:00.000000 vban_cmd-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.3.1/LICENSE
+-rw-r--r--   0        0        0      951 2023-07-12 03:49:01.207386 vban_cmd-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0    12527 2023-07-11 18:49:38.369576 vban_cmd-2.3.1/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.3.1/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.3.1/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.3.1/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.3.1/vban_cmd/config.py
+-rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.3.1/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.3.1/vban_cmd/event.py
+-rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.3.1/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4115 2023-07-05 18:08:51.113607 vban_cmd-2.3.1/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.3.1/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     1150 2023-07-08 06:13:52.713834 vban_cmd-2.3.1/vban_cmd/macrobutton.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.3.1/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.3.1/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.3.1/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.3.1/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.3.1/vban_cmd/util.py
+-rw-r--r--   0        0        0     4320 2023-07-08 06:27:12.206963 vban_cmd-2.3.1/vban_cmd/vban.py
+-rw-r--r--   0        0        0     7391 2023-07-12 03:47:07.637840 vban_cmd-2.3.1/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.3.1/vban_cmd/worker.py
+-rw-r--r--   0        0        0    12664 1970-01-01 00:00:00.000000 vban_cmd-2.3.1/PKG-INFO
```

### Comparing `vban_cmd-2.3.0/LICENSE` & `vban_cmd-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/pyproject.toml` & `vban_cmd-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.3.0"
+version = "2.3.1"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.3.0/README.md` & `vban_cmd-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/bus.py` & `vban_cmd-2.3.1/vban_cmd/bus.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/command.py` & `vban_cmd-2.3.1/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/config.py` & `vban_cmd-2.3.1/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/event.py` & `vban_cmd-2.3.1/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/factory.py` & `vban_cmd-2.3.1/vban_cmd/factory.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/iremote.py` & `vban_cmd-2.3.1/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/kinds.py` & `vban_cmd-2.3.1/vban_cmd/kinds.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/macrobutton.py` & `vban_cmd-2.3.1/vban_cmd/macrobutton.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/meta.py` & `vban_cmd-2.3.1/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/packet.py` & `vban_cmd-2.3.1/vban_cmd/packet.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/strip.py` & `vban_cmd-2.3.1/vban_cmd/strip.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/subject.py` & `vban_cmd-2.3.1/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/util.py` & `vban_cmd-2.3.1/vban_cmd/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,8 +69,22 @@
     for a, b in zip(t0, t1):
         if ((1 << 16) - 1) - b <= 7200:
             yield a == b
         else:
             yield True
 
 
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
+
+
 Socket = IntEnum("Socket", "register request response", start=0)
```

### Comparing `vban_cmd-2.3.0/vban_cmd/vban.py` & `vban_cmd-2.3.1/vban_cmd/vban.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/vban_cmd/vbancmd.py` & `vban_cmd-2.3.1/vban_cmd/vbancmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 import socket
 import time
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
 from queue import Queue
-from typing import Iterable, Optional, Union
+from typing import Iterable, Union
 
 from .error import VBANCMDError
 from .event import Event
 from .packet import RequestHeader
 from .subject import Subject
-from .util import Socket, script
+from .util import Socket, deep_merge, script
 from .worker import Producer, Subscriber, Updater
 
 logger = logging.getLogger(__name__)
 
 
 class VbanCmd(metaclass=ABCMeta):
     """Base class responsible for communicating with the VBAN RT Packet Service"""
@@ -190,22 +190,26 @@
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
             raise VBANCMDError(("\n").join(ERR_MSG)) from e
 
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
 
     def logout(self):
```

### Comparing `vban_cmd-2.3.0/vban_cmd/worker.py` & `vban_cmd-2.3.1/vban_cmd/worker.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.0/PKG-INFO` & `vban_cmd-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

