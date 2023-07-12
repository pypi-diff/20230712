# Comparing `tmp/hyprshade-0.2.0.tar.gz` & `tmp/hyprshade-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.2.0.tar", max compression
+gzip compressed data, was "hyprshade-0.3.0.tar", max compression
```

## Comparing `hyprshade-0.2.0.tar` & `hyprshade-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.2.0/LICENSE
--rw-r--r--   0        0        0      719 2023-07-12 02:33:48.487461 hyprshade-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-10 23:35:03.452541 hyprshade-0.2.0/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.2.0/hyprshade/__main__.py
--rw-r--r--   0        0        0     2577 2023-07-11 08:22:08.168519 hyprshade-0.2.0/hyprshade/cli.py
--rw-r--r--   0        0        0     3349 2023-07-11 12:47:30.057291 hyprshade-0.2.0/hyprshade/config.py
--rw-r--r--   0        0        0      956 2023-07-11 02:46:20.738707 hyprshade-0.2.0/hyprshade/helpers.py
--rw-r--r--   0        0        0      808 2023-07-10 06:55:45.350472 hyprshade-0.2.0/hyprshade/utils.py
--rw-r--r--   0        0        0     1024 2023-07-12 02:50:48.862355 hyprshade-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.2.0/shaders/blue-light-filter.glsl
--rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.2.0/shaders/vibrance.glsl
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 hyprshade-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2311 2023-07-12 12:40:55.928150 hyprshade-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 10:22:13.964753 hyprshade-0.3.0/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.3.0/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2669 2023-07-12 12:44:09.002160 hyprshade-0.3.0/hyprshade/cli.py
+-rw-r--r--   0        0        0     3718 2023-07-12 12:36:54.366139 hyprshade-0.3.0/hyprshade/config.py
+-rw-r--r--   0        0        0      956 2023-07-11 02:46:20.738707 hyprshade-0.3.0/hyprshade/helpers.py
+-rw-r--r--   0        0        0      812 2023-07-12 12:09:47.053061 hyprshade-0.3.0/hyprshade/utils.py
+-rw-r--r--   0        0        0     1024 2023-07-12 12:44:55.348162 hyprshade-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.3.0/shaders/blue-light-filter.glsl
+-rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.3.0/shaders/vibrance.glsl
+-rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 hyprshade-0.3.0/PKG-INFO
```

### Comparing `hyprshade-0.2.0/LICENSE` & `hyprshade-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.2.0/hyprshade/cli.py` & `hyprshade-0.3.0/hyprshade/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,27 +64,31 @@
         return 0
 
     return on(shader_name_or_path)
 
 
 @app.command()
 def auto() -> int:
+    """Turn on/off screen shader based on schedule"""
+
     from hyprshade.config import Config
 
     t = datetime.now().time()
     schedule = Config().to_schedule()
     shade = schedule.find_shade(t)
 
     if shade is not None:
         return on(shade)
     return off()
 
 
 @app.command()
 def install() -> int:
+    """Instal systemd user units"""
+
     from hyprshade.config import Config
 
     schedule = Config().to_schedule()
 
     with open(path.join(systemd_user_config_home(), "hyprshade.service"), "w") as f:
         f.write(
             """[Unit]
```

### Comparing `hyprshade-0.2.0/hyprshade/config.py` & `hyprshade-0.3.0/hyprshade/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import os
 from collections.abc import Iterable
 from datetime import time
 from itertools import chain, pairwise
 from os import path
 from typing import Literal, NotRequired, TypedDict, cast
 
 import tomllib
-from more_itertools import nth, partition
+from more_itertools import first_true, nth, partition
 
-from hyprshade.utils import hyprshade_config_home, is_time_between
+from hyprshade.utils import hypr_config_home, hyprshade_config_home, is_time_between
 
 TimeInterval = tuple[time, time]
 
 
 class ShadeDict(TypedDict):
     name: str
     start_time: time
@@ -91,22 +92,29 @@
     """Parses config.toml into a dict"""
 
     _config_dict: ConfigDict
 
     def __init__(self, config_path: str | None = None):
         if config_path is None:
             config_path = Config.get_path()
+            if config_path is None:
+                raise FileNotFoundError("Config file not found")
 
         config_dict = Config._load(config_path)
         self._config_dict = cast(ConfigDict, config_dict)
 
     @staticmethod
     def _load(config_path: str) -> dict[str, object]:
         with open(config_path, "rb") as f:
             return tomllib.load(f)
 
     @staticmethod
-    def get_path() -> str:
-        return path.join(hyprshade_config_home(), "config.toml")
+    def get_path() -> str | None:
+        candidates = [
+            os.getenv("HYPRSHADE_CONFIG"),
+            path.join(hypr_config_home(), "hyprshade.toml"),
+            path.join(hyprshade_config_home(), "config.toml"),
+        ]
+        return first_true([c for c in candidates if c is not None], pred=path.isfile)
 
     def to_schedule(self) -> Schedule:
         return Schedule(self._config_dict)
```

### Comparing `hyprshade-0.2.0/hyprshade/helpers.py` & `hyprshade-0.3.0/hyprshade/helpers.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.2.0/hyprshade/utils.py` & `hyprshade-0.3.0/hyprshade/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     return path.join(xdg_config_home(), "hyprshade")
 
 
 def systemd_user_config_home():
     return path.join(xdg_config_home(), "systemd/user")
 
 
-def is_time_between(time: time, start_time: time, end_time: time) -> bool:
+def is_time_between(time_: time, start_time: time, end_time: time) -> bool:
     if end_time <= start_time:
-        return start_time <= time or time <= end_time
-    return start_time <= time <= end_time
+        return start_time <= time_ or time_ <= end_time
+    return start_time <= time_ <= end_time
```

### Comparing `hyprshade-0.2.0/pyproject.toml` & `hyprshade-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
 include = ["shaders"]
```

### Comparing `hyprshade-0.2.0/shaders/blue-light-filter.glsl` & `hyprshade-0.3.0/shaders/blue-light-filter.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.2.0/shaders/vibrance.glsl` & `hyprshade-0.3.0/shaders/vibrance.glsl`

 * *Files identical despite different names*

