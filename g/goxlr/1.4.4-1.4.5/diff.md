# Comparing `tmp/goxlr-1.4.4.tar.gz` & `tmp/goxlr-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.4.4.tar", last modified: Wed Jul 12 12:20:16 2023, max compression
+gzip compressed data, was "goxlr-1.4.5.tar", last modified: Wed Jul 12 15:33:53 2023, max compression
```

## Comparing `goxlr-1.4.4.tar` & `goxlr-1.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.103587 goxlr-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-12 12:20:06.000000 goxlr-1.4.4/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 12:20:06.000000 goxlr-1.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-12 12:20:16.103587 goxlr-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-12 12:20:06.000000 goxlr-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.099587 goxlr-1.4.4/goxlr/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.103587 goxlr-1.4.4/goxlr/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    26580 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/commands/goxlr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.103587 goxlr-1.4.4/goxlr/types/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/types/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-12 12:20:06.000000 goxlr-1.4.4/goxlr/types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:16.099587 goxlr-1.4.4/goxlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 12:20:16.000000 goxlr-1.4.4/goxlr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 12:20:06.000000 goxlr-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 12:20:16.103587 goxlr-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-12 12:20:06.000000 goxlr-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.472806 goxlr-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-12 15:33:41.000000 goxlr-1.4.5/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 15:33:41.000000 goxlr-1.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-12 15:33:53.472806 goxlr-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-12 15:33:41.000000 goxlr-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.468806 goxlr-1.4.5/goxlr/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.472806 goxlr-1.4.5/goxlr/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26580 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/commands/goxlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23933 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.472806 goxlr-1.4.5/goxlr/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.472806 goxlr-1.4.5/goxlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 15:33:41.000000 goxlr-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 15:33:53.472806 goxlr-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-12 15:33:41.000000 goxlr-1.4.5/setup.py
```

### Comparing `goxlr-1.4.4/LICENSE-3RD-PARTY.txt` & `goxlr-1.4.5/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.4/LICENSE.txt` & `goxlr-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.4/PKG-INFO` & `goxlr-1.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.4
+Version: 1.4.5
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.4/README.md` & `goxlr-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.4/goxlr/commands/daemon.py` & `goxlr-1.4.5/goxlr/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.4/goxlr/commands/goxlr.py` & `goxlr-1.4.5/goxlr/commands/goxlr.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.4/goxlr/commands/status.py` & `goxlr-1.4.5/goxlr/commands/status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Union
 from ..error import DaemonError, MixerNotFoundError
 from ..types.models import *
 
 
 class StatusCommands:
     """
     Used to retrieve information from the GoXLR Utility daemon.
@@ -609,16 +610,58 @@
         return self.get_settings().mute_hold_duration
 
     def is_vc_mute_also_mute_cm(self) -> bool:
         return self.get_settings().vc_mute_also_mute_cm
 
     # Button down
 
-    def get_button_down(self) -> Dict[Button, bool]:
-        return self.mixer.button_down
+    def get_button_down(self, button: Button) -> bool:
+        return self.mixer.button_down[button]
+
+    async def wait_for_button(
+        self,
+        buttons: Union[List[Button], Dict[Button, bool]],
+        all_values: bool = False,
+        invert: bool = False,
+    ) -> Dict[Button, bool]:
+        """
+        Waits for the specified button states to be achieved.
+
+        :param buttons: List of buttons or dictionary specifying the button states to wait for.
+                        - If a list, all buttons are assumed to have the desired state as True (down).
+                        - If a dictionary, Key: Button, Value: Desired button state (True for down, False for up).
+        :param all: Whether to wait for all (instead of any) of the buttons to achieve the desired state.
+        :param invert: Whether to check for the opposite button states.
+        """
+        if isinstance(buttons, dict):
+            button_states = buttons
+        else:
+            button_states = {button: True for button in buttons}
+
+        if invert:
+            button_states = {
+                button: not state for button, state in button_states.items()
+            }
+
+        if all_values:
+            while not all(
+                self.get_button_down(button) == state
+                for button, state in button_states.items()
+            ):
+                await self.receive_patch()
+        else:
+            while not any(
+                self.get_button_down(button) == state
+                for button, state in button_states.items()
+            ):
+                await self.receive_patch()
+
+        await self.update()  # be sure it's up to date
+
+        return {button: self.get_button_down(button) for button in button_states.keys()}
 
     # Profile name
 
     def get_profile_name(self) -> str:
         return self.mixer.profile_name
 
     def get_mic_profile_name(self) -> str:
```

### Comparing `goxlr-1.4.4/goxlr/socket.py` & `goxlr-1.4.5/goxlr/socket.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.4/goxlr/types/enums.py` & `goxlr-1.4.5/goxlr/types/enums.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.4/goxlr/types/models.py` & `goxlr-1.4.5/goxlr/types/models.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.4/goxlr.egg-info/PKG-INFO` & `goxlr-1.4.5/goxlr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.4
+Version: 1.4.5
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.4/setup.py` & `goxlr-1.4.5/setup.py`

 * *Files identical despite different names*

