# Comparing `tmp/vban_cmd-2.3.1.tar.gz` & `tmp/vban_cmd-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.3.1.tar", max compression
+gzip compressed data, was "vban_cmd-2.3.2.tar", max compression
```

## Comparing `vban_cmd-2.3.1.tar` & `vban_cmd-2.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.3.1/LICENSE
--rw-r--r--   0        0        0      951 2023-07-12 03:49:01.207386 vban_cmd-2.3.1/pyproject.toml
--rw-r--r--   0        0        0    12527 2023-07-11 18:49:38.369576 vban_cmd-2.3.1/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.3.1/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.3.1/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.3.1/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.3.1/vban_cmd/config.py
--rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.3.1/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.3.1/vban_cmd/event.py
--rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.3.1/vban_cmd/factory.py
--rw-r--r--   0        0        0     4115 2023-07-05 18:08:51.113607 vban_cmd-2.3.1/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban_cmd-2.3.1/vban_cmd/kinds.py
--rw-r--r--   0        0        0     1150 2023-07-08 06:13:52.713834 vban_cmd-2.3.1/vban_cmd/macrobutton.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.3.1/vban_cmd/meta.py
--rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.3.1/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.3.1/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.3.1/vban_cmd/subject.py
--rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.3.1/vban_cmd/util.py
--rw-r--r--   0        0        0     4320 2023-07-08 06:27:12.206963 vban_cmd-2.3.1/vban_cmd/vban.py
--rw-r--r--   0        0        0     7391 2023-07-12 03:47:07.637840 vban_cmd-2.3.1/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.3.1/vban_cmd/worker.py
--rw-r--r--   0        0        0    12664 1970-01-01 00:00:00.000000 vban_cmd-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.3.2/LICENSE
+-rw-r--r--   0        0        0      951 2023-07-12 08:49:24.959188 vban_cmd-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0    12527 2023-07-11 18:49:38.369576 vban_cmd-2.3.2/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.3.2/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.3.2/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.3.2/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.3.2/vban_cmd/config.py
+-rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.3.2/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.3.2/vban_cmd/event.py
+-rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.3.2/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4115 2023-07-05 18:08:51.113607 vban_cmd-2.3.2/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2202 2023-07-12 04:34:54.220984 vban_cmd-2.3.2/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     1150 2023-07-08 06:13:52.713834 vban_cmd-2.3.2/vban_cmd/macrobutton.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.3.2/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.3.2/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.3.2/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.3.2/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.3.2/vban_cmd/util.py
+-rw-r--r--   0        0        0     5996 2023-07-12 09:23:28.333915 vban_cmd-2.3.2/vban_cmd/vban.py
+-rw-r--r--   0        0        0     7391 2023-07-12 03:47:07.637840 vban_cmd-2.3.2/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.3.2/vban_cmd/worker.py
+-rw-r--r--   0        0        0    12664 1970-01-01 00:00:00.000000 vban_cmd-2.3.2/PKG-INFO
```

### Comparing `vban_cmd-2.3.1/LICENSE` & `vban_cmd-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/pyproject.toml` & `vban_cmd-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.3.1"
+version = "2.3.2"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.3.1/README.md` & `vban_cmd-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/bus.py` & `vban_cmd-2.3.2/vban_cmd/bus.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/command.py` & `vban_cmd-2.3.2/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/config.py` & `vban_cmd-2.3.2/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/event.py` & `vban_cmd-2.3.2/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/factory.py` & `vban_cmd-2.3.2/vban_cmd/factory.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/iremote.py` & `vban_cmd-2.3.2/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/kinds.py` & `vban_cmd-2.3.2/vban_cmd/kinds.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,31 +58,31 @@
 
 
 @dataclass
 class BasicMap(KindMapClass):
     name: str
     ins: tuple = (2, 1)
     outs: tuple = (1, 1)
-    vban: tuple = (4, 4)
+    vban: tuple = (4, 4, 1, 1)
 
 
 @dataclass
 class BananaMap(KindMapClass):
     name: str
     ins: tuple = (3, 2)
     outs: tuple = (3, 2)
-    vban: tuple = (8, 8)
+    vban: tuple = (8, 8, 1, 1)
 
 
 @dataclass
 class PotatoMap(KindMapClass):
     name: str
     ins: tuple = (5, 3)
     outs: tuple = (5, 3)
-    vban: tuple = (8, 8)
+    vban: tuple = (8, 8, 1, 1)
 
 
 def kind_factory(kind_id):
     match kind_id:
         case "basic":
             _kind_map = BasicMap
         case "banana":
```

### Comparing `vban_cmd-2.3.1/vban_cmd/macrobutton.py` & `vban_cmd-2.3.2/vban_cmd/macrobutton.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/meta.py` & `vban_cmd-2.3.2/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/packet.py` & `vban_cmd-2.3.2/vban_cmd/packet.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/strip.py` & `vban_cmd-2.3.2/vban_cmd/strip.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/subject.py` & `vban_cmd-2.3.2/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/util.py` & `vban_cmd-2.3.2/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/vban.py` & `vban_cmd-2.3.2/vban_cmd/vban.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import abstractmethod
 
 from .iremote import IRemote
+from .kinds import kinds_all
 
 
 class VbanStream(IRemote):
     """
     Implements the common interface
 
     Defines concrete implementation for vban stream
@@ -129,14 +130,29 @@
         return
 
     @property
     def bit(self) -> int:
         return
 
 
+class VbanAudioInstream(VbanInstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
+class VbanMidiInstream(VbanInstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
+class VbanTextInstream(VbanInstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
 class VbanOutstream(VbanStream):
     """
     class representing a vban outstream
 
     Subclasses VbanStream
     """
 
@@ -144,26 +160,70 @@
         return f"{type(self).__name__}{self._remote.kind}{self.index}"
 
     @property
     def direction(self) -> str:
         return "out"
 
 
+class VbanAudioOutstream(VbanOutstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
+class VbanMidiOutstream(VbanOutstream):
+    def __str__(self):
+        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+
+
+def _make_stream_pair(remote, kind):
+    num_instream, num_outstream, num_midi, num_text = kind.vban
+
+    def _generate_streams(i, dir):
+        """generator function for creating instream/outstream tuples"""
+        if dir == "in":
+            if i < num_instream:
+                yield VbanAudioInstream
+            elif i < num_instream + num_midi:
+                yield VbanMidiInstream
+            else:
+                yield VbanTextInstream
+        else:
+            if i < num_outstream:
+                yield VbanAudioOutstream
+            else:
+                yield VbanMidiOutstream
+
+    return (
+        tuple(
+            cls(remote, i)
+            for i in range(num_instream + num_midi + num_text)
+            for cls in _generate_streams(i, "in")
+        ),
+        tuple(
+            cls(remote, i)
+            for i in range(num_outstream + num_midi)
+            for cls in _generate_streams(i, "out")
+        ),
+    )
+
+
+def _make_stream_pairs(remote):
+    return {kind.name: _make_stream_pair(remote, kind) for kind in kinds_all}
+
+
 class Vban:
     """
     class representing the vban module
 
     Contains two tuples, one for each stream type
     """
 
     def __init__(self, remote):
         self.remote = remote
-        num_instream, num_outstream = remote.kind.vban
-        self.instream = tuple(VbanInstream(remote, i) for i in range(num_instream))
-        self.outstream = tuple(VbanOutstream(remote, i) for i in range(num_outstream))
+        self.instream, self.outstream = _make_stream_pairs(remote)[remote.kind.name]
 
     def enable(self):
         """if VBAN disabled there can be no communication with it"""
 
     def disable(self):
         self.remote._set_rt("vban.Enable", 0)
```

### Comparing `vban_cmd-2.3.1/vban_cmd/vbancmd.py` & `vban_cmd-2.3.2/vban_cmd/vbancmd.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/vban_cmd/worker.py` & `vban_cmd-2.3.2/vban_cmd/worker.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.1/PKG-INFO` & `vban_cmd-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.3.1
+Version: 2.3.2
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

