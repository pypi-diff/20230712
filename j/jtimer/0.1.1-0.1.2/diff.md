# Comparing `tmp/jtimer-0.1.1.tar.gz` & `tmp/jtimer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtimer-0.1.1.tar", max compression
+gzip compressed data, was "jtimer-0.1.2.tar", max compression
```

## Comparing `jtimer-0.1.1.tar` & `jtimer-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      697 2023-07-12 13:34:25.335708 jtimer-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-07-05 12:32:42.025116 jtimer-0.1.1/jtimer/__init__.py
--rw-r--r--   0        0        0      353 2023-07-12 12:22:04.706105 jtimer-0.1.1/jtimer/controller/__init__.py
--rw-r--r--   0        0        0     1122 2023-07-12 12:22:04.698105 jtimer-0.1.1/jtimer/controller/calc_utils.py
--rw-r--r--   0        0        0     3372 2023-07-12 13:04:11.170016 jtimer-0.1.1/jtimer/controller/timer_controller.py
--rw-r--r--   0        0        0     4187 2023-07-12 12:39:08.646493 jtimer-0.1.1/jtimer/dao/__init__.py
--rw-r--r--   0        0        0      832 2023-07-12 12:52:40.395301 jtimer-0.1.1/jtimer/main.py
--rw-r--r--   0        0        0        0 2023-07-02 23:23:52.197749 jtimer-0.1.1/jtimer/model/__init__.py
--rw-r--r--   0        0        0      467 2023-07-05 10:05:36.834824 jtimer-0.1.1/jtimer/model/time_event.py
--rw-r--r--   0        0        0      788 2023-07-12 12:21:41.349459 jtimer-0.1.1/jtimer/model/timer.py
--rw-r--r--   0        0        0      158 2023-07-05 08:39:15.858177 jtimer-0.1.1/jtimer/view/__init__.py
--rw-r--r--   0        0        0     1468 2023-07-12 12:19:22.753431 jtimer-0.1.1/jtimer/view/stats_view.py
--rw-r--r--   0        0        0     3379 2023-07-12 12:13:10.876234 jtimer-0.1.1/jtimer/view/timer_widget.py
--rw-r--r--   0        0        0     2345 2023-07-12 12:19:21.753401 jtimer-0.1.1/jtimer/view/timers_view.py
--rw-r--r--   0        0        0      683 2023-07-12 13:35:57.804537 jtimer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      192 2023-07-05 10:16:26.043062 jtimer-0.1.1/schema.sql
--rw-r--r--   0        0        0     1480 2023-07-12 13:36:02.303944 jtimer-0.1.1/setup.py
--rw-r--r--   0        0        0     1222 2023-07-12 13:36:02.304149 jtimer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      697 2023-07-12 13:34:25.335708 jtimer-0.1.2/README.md
+-rw-r--r--   0        0        0       38 2023-07-12 13:39:39.101470 jtimer-0.1.2/jtimer/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-12 12:22:04.706105 jtimer-0.1.2/jtimer/controller/__init__.py
+-rw-r--r--   0        0        0     1122 2023-07-12 12:22:04.698105 jtimer-0.1.2/jtimer/controller/calc_utils.py
+-rw-r--r--   0        0        0     3372 2023-07-12 13:04:11.170016 jtimer-0.1.2/jtimer/controller/timer_controller.py
+-rw-r--r--   0        0        0     4187 2023-07-12 12:39:08.646493 jtimer-0.1.2/jtimer/dao/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-12 12:52:40.395301 jtimer-0.1.2/jtimer/main.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:23:52.197749 jtimer-0.1.2/jtimer/model/__init__.py
+-rw-r--r--   0        0        0      467 2023-07-05 10:05:36.834824 jtimer-0.1.2/jtimer/model/time_event.py
+-rw-r--r--   0        0        0      788 2023-07-12 12:21:41.349459 jtimer-0.1.2/jtimer/model/timer.py
+-rw-r--r--   0        0        0      158 2023-07-05 08:39:15.858177 jtimer-0.1.2/jtimer/view/__init__.py
+-rw-r--r--   0        0        0     1468 2023-07-12 12:19:22.753431 jtimer-0.1.2/jtimer/view/stats_view.py
+-rw-r--r--   0        0        0     3379 2023-07-12 12:13:10.876234 jtimer-0.1.2/jtimer/view/timer_widget.py
+-rw-r--r--   0        0        0     2345 2023-07-12 12:19:21.753401 jtimer-0.1.2/jtimer/view/timers_view.py
+-rw-r--r--   0        0        0      683 2023-07-12 13:39:36.669662 jtimer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-07-05 10:16:26.043062 jtimer-0.1.2/schema.sql
+-rw-r--r--   0        0        0     1480 2023-07-12 13:40:21.299773 jtimer-0.1.2/setup.py
+-rw-r--r--   0        0        0     1222 2023-07-12 13:40:21.300017 jtimer-0.1.2/PKG-INFO
```

### Comparing `jtimer-0.1.1/README.md` & `jtimer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.1/jtimer/controller/calc_utils.py` & `jtimer-0.1.2/jtimer/controller/calc_utils.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.1/jtimer/controller/timer_controller.py` & `jtimer-0.1.2/jtimer/controller/timer_controller.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.1/jtimer/dao/__init__.py` & `jtimer-0.1.2/jtimer/dao/__init__.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.1/jtimer/main.py` & `jtimer-0.1.2/jtimer/main.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.1/jtimer/model/timer.py` & `jtimer-0.1.2/jtimer/model/timer.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.1/jtimer/view/stats_view.py` & `jtimer-0.1.2/jtimer/view/stats_view.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.1/jtimer/view/timer_widget.py` & `jtimer-0.1.2/jtimer/view/timer_widget.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.1/jtimer/view/timers_view.py` & `jtimer-0.1.2/jtimer/view/timers_view.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.1/pyproject.toml` & `jtimer-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jtimer"
-version = "0.1.1"
+version = "0.1.2"
 description = "John's Timer - desktop app for tracking time"
 authors = ["John Watson <jmwdev@pm.me>"]
 maintainers = ["John Watson <jmwdev@pm.me>"]
 license = "GNU GENERAL PUBLIC LICENSE V3"
 readme = "README.md"
 keywords = ["productivity"]
 classifiers = [
```

### Comparing `jtimer-0.1.1/setup.py` & `jtimer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 modules = \
 ['schema']
 install_requires = \
 ['PyQt6>=6.5.1,<7.0.0']
 
 setup_kwargs = {
     'name': 'jtimer',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': "John's Timer - desktop app for tracking time",
     'long_description': '# Timer App\n\nDEVELOPMENT IN PROGRESS\n\nDissatisfied with the selection of timer applications available in linux, I built my own.  It maintains a simple local db in /tmp\n\nThe application is fairly simple:\n    * user can specify a list of different timers.\n    * timers can be renamed.\n    * timers can be started / stopped concurrently.\n    * on startup the timers will resume the count from the last start.\n    * timers should not cross over days. automatic stop times at 23:59:59 for forgotten timers.\n    * daily statistics view\n\n\n\n## Installation\n```bash\npip install jtimer  # not timer\n```\n\n## Usage\n```bash\njtimer\n```\n\n## Planned Future developments\n\n* timer linked triggers\n* timer event view',
     'author': 'John Watson',
     'author_email': 'jmwdev@pm.me',
     'maintainer': 'John Watson',
     'maintainer_email': 'jmwdev@pm.me',
     'url': None,
```

### Comparing `jtimer-0.1.1/PKG-INFO` & `jtimer-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtimer
-Version: 0.1.1
+Version: 0.1.2
 Summary: John's Timer - desktop app for tracking time
 License: GNU GENERAL PUBLIC LICENSE V3
 Keywords: productivity
 Author: John Watson
 Author-email: jmwdev@pm.me
 Maintainer: John Watson
 Maintainer-email: jmwdev@pm.me
```

