# Comparing `tmp/miniature_lighting_desk-0.2.0.tar.gz` & `tmp/miniature_lighting_desk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniature_lighting_desk-0.2.0.tar", max compression
+gzip compressed data, was "miniature_lighting_desk-0.3.0.tar", max compression
```

## Comparing `miniature_lighting_desk-0.2.0.tar` & `miniature_lighting_desk-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.2.0/LICENSE
--rw-r--r--   0        0        0       43 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.2.0/miniature_lighting_desk/__init__.py
--rw-r--r--   0        0        0    10130 2023-07-10 21:44:26.485799 miniature_lighting_desk-0.2.0/miniature_lighting_desk/async_hal.py
--rw-r--r--   0        0        0     1089 2023-07-10 21:50:30.169129 miniature_lighting_desk-0.2.0/miniature_lighting_desk/cli.py
--rw-r--r--   0        0        0     3000 2023-07-10 21:46:19.949131 miniature_lighting_desk-0.2.0/miniature_lighting_desk/local_gui.py
--rw-r--r--   0        0        0     4404 2023-07-10 21:52:08.892461 miniature_lighting_desk-0.2.0/miniature_lighting_desk/server.py
--rw-r--r--   0        0        0      815 2023-07-11 21:03:17.451758 miniature_lighting_desk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 miniature_lighting_desk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.3.0/LICENSE
+-rw-r--r--   0        0        0       43 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.3.0/miniature_lighting_desk/__init__.py
+-rw-r--r--   0        0        0    10677 2023-07-11 22:48:36.988372 miniature_lighting_desk-0.3.0/miniature_lighting_desk/async_hal.py
+-rw-r--r--   0        0        0     2506 2023-07-11 22:51:31.421704 miniature_lighting_desk-0.3.0/miniature_lighting_desk/cli.py
+-rw-r--r--   0        0        0     3000 2023-07-10 21:46:19.949131 miniature_lighting_desk-0.3.0/miniature_lighting_desk/local_gui.py
+-rw-r--r--   0        0        0     4404 2023-07-10 21:52:08.892461 miniature_lighting_desk-0.3.0/miniature_lighting_desk/server.py
+-rw-r--r--   0        0        0      815 2023-07-11 23:11:04.385027 miniature_lighting_desk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 miniature_lighting_desk-0.3.0/PKG-INFO
```

### Comparing `miniature_lighting_desk-0.2.0/LICENSE` & `miniature_lighting_desk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.2.0/miniature_lighting_desk/async_hal.py` & `miniature_lighting_desk-0.3.0/miniature_lighting_desk/async_hal.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,24 @@
         """Queue getting brightness."""
         future = self.submit_async(
             partial(self._async_get_brightness, channel), block=True
         )
         return self.unscale_brightness(future.result())
 
 
+class WifiControllerABC(ControllerABC):
+    @abstractmethod
+    def wifi(self, ssid: str, password: str) -> dict:
+        """Connect controller to wifi network."""
+
+    @abstractmethod
+    def wifi_status(self) -> dict:
+        """Get controller wifi status."""
+
+
 class MockController(ControllerABC):
     def __init__(self, *args, no_channels=8, **kwargs):
         self.no_channels = no_channels
         self.vals = [0] * no_channels
         self.max_brightness = 100
         super().__init__(*args, **kwargs)
 
@@ -182,23 +192,25 @@
     def scale_brightness(self, unscaled: int) -> int:
         return self.max_brightness - unscaled
 
     def unscale_brightness(self, scaled: int) -> int:
         return self.max_brightness - scaled
 
 
-class SerialRpcController(ControllerABC):
+class SerialRpcController(WifiControllerABC):
     def __init__(self, *args, port="/dev/ttyUSB0", **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.serial = AioSerial(port=port, baudrate=460800)
         self.lock = asyncio.Lock()
-        future = self.submit_async(partial(self.call, "channel_count"), block=True)
-        self.no_channels = future.result()
-        future = self.submit_async(partial(self.call, "max_brightness"), block=True)
-        self.max_brightness = future.result()
+        self.no_channels = self.sync_call("channel_count")
+        self.max_brightness = self.sync_call("max_brightness")
+
+    def sync_call(self, method: str, **kwargs):
+        future = self.submit_async(partial(self.call, method, **kwargs), block=True)
+        return future.result()
 
     async def call(self, method: str, **kwargs):
         async with self.lock:  # dunno, might be needed...
             cmd = request_json(method, params=kwargs).encode()
             await self.serial.write_async(cmd)
             await self.serial.write_async(b"\n\r")
             resp = await self.serial.readline_async()
@@ -211,14 +223,23 @@
     async def _async_set_brightness(
         self, channel: int, brightness: int, pause: float = 0
     ) -> None:
         return await self.call("set_brightness", channel=channel, brightness=brightness)
 
     scale_brightness = unscale_brightness = lambda s, x: x
 
+    def wifi(self, ssid: str, password: str):
+        return self.sync_call("wifi_connect", ssid=ssid, key=password)
+
+    def wifi_status(self):
+        return self.sync_call("wifi_status")
+
+    def repl(self):
+        return self.sync_call("repl")
+
 
 class Channel:
     """Class to represent a particular channel on the controller."""
 
     def __init__(
         self,
         controller: ControllerABC,
```

### Comparing `miniature_lighting_desk-0.2.0/miniature_lighting_desk/local_gui.py` & `miniature_lighting_desk-0.3.0/miniature_lighting_desk/local_gui.py`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.2.0/miniature_lighting_desk/server.py` & `miniature_lighting_desk-0.3.0/miniature_lighting_desk/server.py`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.2.0/pyproject.toml` & `miniature_lighting_desk-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miniature-lighting-desk"
-version = "0.2.0"
+version = "0.3.0"
 description = "Desk software for Miniature Lighting Controller"
 authors = ["John Maximilian <2e0byo@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyusb = "^1.2.1"
```

### Comparing `miniature_lighting_desk-0.2.0/PKG-INFO` & `miniature_lighting_desk-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniature-lighting-desk
-Version: 0.2.0
+Version: 0.3.0
 Summary: Desk software for Miniature Lighting Controller
 License: MIT
 Author: John Maximilian
 Author-email: 2e0byo@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

