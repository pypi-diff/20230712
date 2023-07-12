# Comparing `tmp/mkdocs_calendar_plugin-0.2.2.tar.gz` & `tmp/mkdocs_calendar_plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_calendar_plugin-0.2.2.tar", max compression
+gzip compressed data, was "mkdocs_calendar_plugin-0.3.0.tar", max compression
```

## Comparing `mkdocs_calendar_plugin-0.2.2.tar` & `mkdocs_calendar_plugin-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       25 2023-07-12 11:48:58.907878 mkdocs_calendar_plugin-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-07-12 11:48:58.907878 mkdocs_calendar_plugin-0.2.2/mkdocs_calendar/__init__.py
--rw-r--r--   0        0        0     3255 2023-07-12 11:48:58.907878 mkdocs_calendar_plugin-0.2.2/mkdocs_calendar/plugin.py
--rw-r--r--   0        0        0     1124 2023-07-12 11:48:58.907878 mkdocs_calendar_plugin-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 mkdocs_calendar_plugin-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4801 2023-07-12 12:32:46.848452 mkdocs_calendar_plugin-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 12:32:46.848452 mkdocs_calendar_plugin-0.3.0/mkdocs_calendar/__init__.py
+-rw-r--r--   0        0        0     3293 2023-07-12 12:32:46.852452 mkdocs_calendar_plugin-0.3.0/mkdocs_calendar/plugin.py
+-rw-r--r--   0        0        0     1190 2023-07-12 12:32:46.852452 mkdocs_calendar_plugin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5877 1970-01-01 00:00:00.000000 mkdocs_calendar_plugin-0.3.0/PKG-INFO
```

### Comparing `mkdocs_calendar_plugin-0.2.2/mkdocs_calendar/plugin.py` & `mkdocs_calendar_plugin-0.3.0/mkdocs_calendar/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 class CalendarPluginConfig(BaseConfig):
     """Configuration options for the calendar plugin."""
 
     start = c.Optional(c.Type(date))
     end = c.Optional(c.Type(date))
-    tz = c.Choice(pytz.all_timezones, default="Europe/Zurich")
+    tz = c.Choice(pytz.all_timezones, default="UTC")
     week_names = c.Type(list, default=[])
     extra_key = c.Type(str, default="cal")
 
 
 # pylint: disable-next=too-few-public-methods
 class CalendarPlugin(BasePlugin[CalendarPluginConfig]):
     """Calendar plugin for MkDocs"""
@@ -71,20 +71,21 @@
             cal["academic_week"] = aw + 1
             if isinstance(week_names, Sequence) and 0 <= aw < len(week_names):
                 cal["academic_week_name"] = week_names[aw]
             else:
                 cal["academic_week_name"] = None
 
             cal["start"] = start_date
-            cal["delta"] = (now.date() - start_date).days
-            cal["delta_w"] = ((now.date() - start_date).days) / 7
+            cal["elapsed"] = (now.date() - start_date).days
+            cal["elapsed_weeks"] = cal["elapsed"] / 7
 
             cal["aw"] = cal["academic_week"]
             cal["awn"] = cal["academic_week_name"]
 
         if end_date is not None:
             cal["end"] = end_date
             cal["remaining"] = (end_date - now.date()).days
+            cal["remaining_weeks"] = cal["remaining"] / 7
 
         config.extra[self.config["extra_key"]] = cal
 
         return config
```

### Comparing `mkdocs_calendar_plugin-0.2.2/pyproject.toml` & `mkdocs_calendar_plugin-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mkdocs-calendar-plugin"
-version = "0.2.2"
-description = "An MkDocs plugin to ..."
+version = "0.3.0"
+description = "An MkDocs plugin to expose calendar information to the 'extra' configuration variable."
 authors = ["Jacques Supcik <jacques.supcik@hefr.ch>"]
-repository = "https://github.com/supcik/mkdocs-today-plugin"
+repository = "https://github.com/supcik/mkdocs-calendar-plugin"
 license = "Apache-2"
 readme = "README.md"
 packages = [{ include = "mkdocs_calendar" }]
 keywords = ["mkdocs", "python", "markdown", "wiki"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

