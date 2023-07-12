# Comparing `tmp/mkdocs_calendar_plugin-0.2.1.tar.gz` & `tmp/mkdocs_calendar_plugin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_calendar_plugin-0.2.1.tar", max compression
+gzip compressed data, was "mkdocs_calendar_plugin-0.2.2.tar", max compression
```

## Comparing `mkdocs_calendar_plugin-0.2.1.tar` & `mkdocs_calendar_plugin-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       25 2023-07-10 18:49:47.627514 mkdocs_calendar_plugin-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-10 18:49:47.627514 mkdocs_calendar_plugin-0.2.1/mkdocs_calendar/__init__.py
--rw-r--r--   0        0        0     3230 2023-07-10 18:49:47.627514 mkdocs_calendar_plugin-0.2.1/mkdocs_calendar/plugin.py
--rw-r--r--   0        0        0     1124 2023-07-10 18:49:47.627514 mkdocs_calendar_plugin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 mkdocs_calendar_plugin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-12 11:48:58.907878 mkdocs_calendar_plugin-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 11:48:58.907878 mkdocs_calendar_plugin-0.2.2/mkdocs_calendar/__init__.py
+-rw-r--r--   0        0        0     3255 2023-07-12 11:48:58.907878 mkdocs_calendar_plugin-0.2.2/mkdocs_calendar/plugin.py
+-rw-r--r--   0        0        0     1124 2023-07-12 11:48:58.907878 mkdocs_calendar_plugin-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 mkdocs_calendar_plugin-0.2.2/PKG-INFO
```

### Comparing `mkdocs_calendar_plugin-0.2.1/mkdocs_calendar/plugin.py` & `mkdocs_calendar_plugin-0.2.2/mkdocs_calendar/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 # @attention   : SPDX-License-Identifier: MIT OR Apache-2.0
 ################################################################################
 
 """Calendar plugin for MkDocs"""
 
 import logging
 import time
+from collections.abc import Sequence
 from datetime import date, datetime
 
 import pytz
 from mkdocs.config import config_options as c
 from mkdocs.config.base import Config as BaseConfig
-from mkdocs.exceptions import PluginError
 from mkdocs.plugins import BasePlugin
 from pytz import timezone
 
 logger = logging.getLogger("mkdocs.plugins." + __name__)
 TAG = "[calendar] -"
 
 
 class CalendarPluginConfig(BaseConfig):
     """Configuration options for the calendar plugin."""
 
     start = c.Optional(c.Type(date))
     end = c.Optional(c.Type(date))
     tz = c.Choice(pytz.all_timezones, default="Europe/Zurich")
-    weeks_off = c.Type(list, default=[])
+    week_names = c.Type(list, default=[])
     extra_key = c.Type(str, default="cal")
 
 
 # pylint: disable-next=too-few-public-methods
 class CalendarPlugin(BasePlugin[CalendarPluginConfig]):
     """Calendar plugin for MkDocs"""
 
@@ -52,37 +52,38 @@
 
     def on_config(self, config):
         """Validate the configuration and add calendar entries to the config."""
         now = datetime.fromtimestamp(time.time(), tz=timezone(self.config["tz"]))
 
         start_date = self.get_xconfig(config, "start")
         end_date = self.get_xconfig(config, "end")
-        weeks_off = self.get_xconfig(config, "weeks_off") or []
+        week_names = self.get_xconfig(config, "week_names") or []
         cal = {
             "now": now,
             "today": now.date(),
             "weekday": now.weekday(),
             "week_number": now.isocalendar()[1],
             "iso_weekday": now.isoweekday(),
         }
 
         if start_date is not None:
-            academic_week = ((now.date() - start_date).days) // 7 + 1
-            try:
-                for i in weeks_off:
-                    if academic_week >= i:
-                        academic_week -= 1
-            except Exception as e:  # pylint: disable=invalid-name
-                raise PluginError(f"{TAG} : {e}") from e
+            # pylint: disable-next=invalid-name
+            aw = ((now.date() - start_date).days) // 7
+            cal["academic_week"] = aw + 1
+            if isinstance(week_names, Sequence) and 0 <= aw < len(week_names):
+                cal["academic_week_name"] = week_names[aw]
+            else:
+                cal["academic_week_name"] = None
 
             cal["start"] = start_date
             cal["delta"] = (now.date() - start_date).days
             cal["delta_w"] = ((now.date() - start_date).days) / 7
-            cal["academic_week"] = academic_week
-            cal["aw"] = academic_week
+
+            cal["aw"] = cal["academic_week"]
+            cal["awn"] = cal["academic_week_name"]
 
         if end_date is not None:
             cal["end"] = end_date
             cal["remaining"] = (end_date - now.date()).days
 
         config.extra[self.config["extra_key"]] = cal
```

### Comparing `mkdocs_calendar_plugin-0.2.1/pyproject.toml` & `mkdocs_calendar_plugin-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-calendar-plugin"
-version = "0.2.1"
+version = "0.2.2"
 description = "An MkDocs plugin to ..."
 authors = ["Jacques Supcik <jacques.supcik@hefr.ch>"]
 repository = "https://github.com/supcik/mkdocs-today-plugin"
 license = "Apache-2"
 readme = "README.md"
 packages = [{ include = "mkdocs_calendar" }]
 keywords = ["mkdocs", "python", "markdown", "wiki"]
```

### Comparing `mkdocs_calendar_plugin-0.2.1/PKG-INFO` & `mkdocs_calendar_plugin-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-calendar-plugin
-Version: 0.2.1
+Version: 0.2.2
 Summary: An MkDocs plugin to ...
 Home-page: https://github.com/supcik/mkdocs-today-plugin
 License: Apache-2
 Keywords: mkdocs,python,markdown,wiki
 Author: Jacques Supcik
 Author-email: jacques.supcik@hefr.ch
 Requires-Python: >=3.10,<4.0
```

