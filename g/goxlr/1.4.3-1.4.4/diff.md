# Comparing `tmp/goxlr-1.4.3.tar.gz` & `tmp/goxlr-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.4.3.tar", last modified: Tue Jul 11 16:57:57 2023, max compression
+gzip compressed data, was "goxlr-1.4.4.tar", last modified: Wed Jul 12 12:20:16 2023, max compression
```

## Comparing `goxlr-1.4.3.tar` & `goxlr-1.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.344742 goxlr-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-11 16:57:45.000000 goxlr-1.4.3/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 16:57:45.000000 goxlr-1.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 16:57:57.344742 goxlr-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-11 16:57:45.000000 goxlr-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.340742 goxlr-1.4.3/goxlr/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.344742 goxlr-1.4.3/goxlr/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/commands/goxlr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.344742 goxlr-1.4.3/goxlr/types/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/types/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.340742 goxlr-1.4.3/goxlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 16:57:45.000000 goxlr-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 16:57:57.344742 goxlr-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 16:57:45.000000 goxlr-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.103587 goxlr-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-12 12:20:06.000000 goxlr-1.4.4/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 12:20:06.000000 goxlr-1.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-12 12:20:16.103587 goxlr-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-12 12:20:06.000000 goxlr-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.099587 goxlr-1.4.4/goxlr/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.103587 goxlr-1.4.4/goxlr/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26580 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/commands/goxlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.103587 goxlr-1.4.4/goxlr/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.099587 goxlr-1.4.4/goxlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 12:20:06.000000 goxlr-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 12:20:16.103587 goxlr-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-12 12:20:06.000000 goxlr-1.4.4/setup.py
```

### Comparing `goxlr-1.4.3/LICENSE-3RD-PARTY.txt` & `goxlr-1.4.4/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.3/LICENSE.txt` & `goxlr-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.3/PKG-INFO` & `goxlr-1.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.3
+Version: 1.4.4
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.3/README.md` & `goxlr-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.3/goxlr/commands/daemon.py` & `goxlr-1.4.4/goxlr/commands/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from ..types import LogLevel, PathType
 
 
 class DaemonCommands:
+    """
+    Used to send commands to the GoXLR daemon.
+    """
+
     async def __send_daemon(self, payload):
         payload = {"Daemon": payload}
         return await self.send(payload)
 
     async def open_ui(self):
         return await self.__send_daemon("OpenUi")
```

### Comparing `goxlr-1.4.3/goxlr/commands/goxlr.py` & `goxlr-1.4.4/goxlr/commands/goxlr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import ctypes
 
+from ..error import MissingFeatureError
+
 from ..types.models import Colours
 from ..types.enums import *
 
 
 class GoXLRCommands:
-    # GoXLR commands
+    """
+    GoXLR-specific commands.
+    """
 
     async def __send_command(self, payload, serial=None):
         payload = {"Command": [serial or self.serial, payload]}
         return await self.send(payload)
 
     async def set_shutdown_commands(self, *methods) -> dict | str:
         """
@@ -169,14 +173,28 @@
 
     # DeEss
     async def set_deesser(self, deesser: ctypes.c_uint8):
         return await self.__send_command({"SetDeesser": deesser})
 
     # Colour Related Settings
     async def set_animation_mode(self, animation_mode: AnimationMode):
+        """
+        Set the animation mode of the device.
+
+        :param animation_mode: The animation mode to set.
+        :type animation_mode: AnimationMode
+
+        :raises MissingFeatureError: If the animation mode is not supported on the GoXLR Mini.
+        """
+        if (
+            animation_mode == AnimationMode.Ripple
+            and self.get_device_type() == DeviceType.Mini
+        ):
+            raise MissingFeatureError("Ripple animation is not supported on the Mini")
+
         return await self.__send_command(
             {
                 "SetAnimationMode": "None"
                 if animation_mode is AnimationMode.NONE
                 else animation_mode.name
             }
         )
```

### Comparing `goxlr-1.4.3/goxlr/commands/status.py` & `goxlr-1.4.4/goxlr/commands/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from ..error import DaemonError, MixerNotFoundError
 from ..types.models import *
 
 
 class StatusCommands:
     """
-    Commands related to getting the status of the GoXLR.
-    I decided to split this into its own file because there's
-    already enough code in goxlr.py.
+    Used to retrieve information from the GoXLR Utility daemon.
     """
 
     async def get_status(self) -> Status:
         """
         Returns the status of the GoXLR.
 
         :return: The status of the GoXLR.
```

### Comparing `goxlr-1.4.3/goxlr/socket.py` & `goxlr-1.4.4/goxlr/socket.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.uri = f"ws://{self.host}:{self.port}/api/websocket"
         self.socket = None
         self.heartbeat_interval = 5
         self.heartbeat_task = None
         self.heartbeat_payload = {"id": 0, "data": "Ping"}
         self.response_queue = []
 
-    async def connect(self):
+    async def open(self):
         """
         Connects to the daemon and starts the heartbeat task.
 
         :return: True if the connection was successful, False otherwise.
         """
         self.socket = await websockets.connect(self.uri)
         self.heartbeat_task = asyncio.create_task(self.__send_heartbeat())
@@ -125,34 +125,42 @@
         :return: The patch from the daemon.
         """
         response = await self.receive(IDType.Patch)
         patches = response.get("data").get("Patch")
 
         return [Patch(p) for p in patches]
 
-    async def open(self):
-        """
-        Alias for `connect()`.
-
-        :return: True if the connection was successful, False otherwise.
-        """
-        return await self.connect()
-
     async def close(self):
         """
         Closes the connection to the daemon.
 
         :return: True if the connection was closed, False otherwise.
         """
         await self.socket.close()
         self.heartbeat_task.cancel()
         return self.socket.closed
 
+    async def connect(self):
+        """
+        Alias for `open()`.
+
+        :return: True if the connection was successful, False otherwise.
+        """
+        return await self.open()
+
+    async def disconnect(self):
+        """
+        Alias for `close()`.
+
+        :return: True if the connection was closed, False otherwise.
+        """
+        return await self.close()
+
     async def __aenter__(self):
-        await self.connect()
+        await self.open()
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
 
 
 class GoXLR(Socket, DaemonCommands, GoXLRCommands, StatusCommands):
@@ -240,21 +248,29 @@
             serial = next(iter(self.status.mixers))
 
         self.serial = serial
         self.mixer = self.status.mixers.get(self.serial)
 
         return self.mixer
 
-    async def connect(self):
+    async def open(self):
         """
         Connects to the GoXLR Utility daemon and gets the latest data.
 
         :return: True if the connection was successful, False otherwise.
 
         :raises DaemonError: If no mixers are found.
         """
-        connected = await super().connect()
+        connected = await super().open()
         if connected:
             await self.update()
             self.select_mixer()  # select the first mixer by default
 
         return connected
+
+    async def connect(self):
+        """
+        Alias for `open()`.
+
+        :return: True if the connection was successful, False otherwise.
+        """
+        return await self.open()
```

### Comparing `goxlr-1.4.3/goxlr/types/enums.py` & `goxlr-1.4.4/goxlr/types/enums.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.3/goxlr/types/models.py` & `goxlr-1.4.4/goxlr/types/models.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.3/goxlr.egg-info/PKG-INFO` & `goxlr-1.4.4/goxlr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.3
+Version: 1.4.4
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.3/setup.py` & `goxlr-1.4.4/setup.py`

 * *Files identical despite different names*

