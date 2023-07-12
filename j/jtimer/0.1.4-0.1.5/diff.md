# Comparing `tmp/jtimer-0.1.4.tar.gz` & `tmp/jtimer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtimer-0.1.4.tar", max compression
+gzip compressed data, was "jtimer-0.1.5.tar", max compression
```

## Comparing `jtimer-0.1.4.tar` & `jtimer-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      697 2023-07-12 13:34:25.335708 jtimer-0.1.4/README.md
--rw-r--r--   0        0        0   110370 2023-07-03 00:50:37.905521 jtimer-0.1.4/images/add.png
--rw-r--r--   0        0        0     3023 2023-07-02 11:38:21.202742 jtimer-0.1.4/images/chart.png
--rw-r--r--   0        0        0   185230 2023-07-03 00:47:33.188869 jtimer-0.1.4/images/delete.png
--rw-r--r--   0        0        0    30477 2023-06-28 11:38:32.874181 jtimer-0.1.4/images/pause.png
--rw-r--r--   0        0        0     3507 2023-06-28 11:43:04.759846 jtimer-0.1.4/images/pause2.png
--rw-r--r--   0        0        0    40030 2023-06-28 11:33:57.440503 jtimer-0.1.4/images/play.png
--rw-r--r--   0        0        0    53318 2023-06-28 11:43:04.739846 jtimer-0.1.4/images/play2.png
--rw-r--r--   0        0        0       38 2023-07-12 14:44:20.004024 jtimer-0.1.4/jtimer/__init__.py
--rw-r--r--   0        0        0      353 2023-07-12 12:22:04.706105 jtimer-0.1.4/jtimer/controller/__init__.py
--rw-r--r--   0        0        0     1122 2023-07-12 12:22:04.698105 jtimer-0.1.4/jtimer/controller/calc_utils.py
--rw-r--r--   0        0        0     3372 2023-07-12 13:04:11.170016 jtimer-0.1.4/jtimer/controller/timer_controller.py
--rw-r--r--   0        0        0     4241 2023-07-12 14:39:18.396294 jtimer-0.1.4/jtimer/dao/__init__.py
--rw-r--r--   0        0        0      859 2023-07-12 13:53:33.879010 jtimer-0.1.4/jtimer/main.py
--rw-r--r--   0        0        0        0 2023-07-02 23:23:52.197749 jtimer-0.1.4/jtimer/model/__init__.py
--rw-r--r--   0        0        0      467 2023-07-05 10:05:36.834824 jtimer-0.1.4/jtimer/model/time_event.py
--rw-r--r--   0        0        0      788 2023-07-12 12:21:41.349459 jtimer-0.1.4/jtimer/model/timer.py
--rw-r--r--   0        0        0      311 2023-07-12 14:41:27.196194 jtimer-0.1.4/jtimer/view/__init__.py
--rw-r--r--   0        0        0     1468 2023-07-12 12:19:22.753431 jtimer-0.1.4/jtimer/view/stats_view.py
--rw-r--r--   0        0        0     3379 2023-07-12 12:13:10.876234 jtimer-0.1.4/jtimer/view/timer_widget.py
--rw-r--r--   0        0        0     2345 2023-07-12 12:19:21.753401 jtimer-0.1.4/jtimer/view/timers_view.py
--rw-r--r--   0        0        0      698 2023-07-12 14:44:15.732029 jtimer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      192 2023-07-05 10:16:26.043062 jtimer-0.1.4/resources/schema.sql
--rw-r--r--   0        0        0     1534 2023-07-12 14:46:15.130725 jtimer-0.1.4/setup.py
--rw-r--r--   0        0        0     1222 2023-07-12 14:46:15.130896 jtimer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      673 2023-07-12 14:47:00.191841 jtimer-0.1.5/README.md
+-rw-r--r--   0        0        0   110370 2023-07-03 00:50:37.905521 jtimer-0.1.5/images/add.png
+-rw-r--r--   0        0        0     3023 2023-07-02 11:38:21.202742 jtimer-0.1.5/images/chart.png
+-rw-r--r--   0        0        0   185230 2023-07-03 00:47:33.188869 jtimer-0.1.5/images/delete.png
+-rw-r--r--   0        0        0    30477 2023-06-28 11:38:32.874181 jtimer-0.1.5/images/pause.png
+-rw-r--r--   0        0        0     3507 2023-06-28 11:43:04.759846 jtimer-0.1.5/images/pause2.png
+-rw-r--r--   0        0        0    40030 2023-06-28 11:33:57.440503 jtimer-0.1.5/images/play.png
+-rw-r--r--   0        0        0    53318 2023-06-28 11:43:04.739846 jtimer-0.1.5/images/play2.png
+-rw-r--r--   0        0        0       38 2023-07-12 14:48:29.947729 jtimer-0.1.5/jtimer/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-12 12:22:04.706105 jtimer-0.1.5/jtimer/controller/__init__.py
+-rw-r--r--   0        0        0     1122 2023-07-12 12:22:04.698105 jtimer-0.1.5/jtimer/controller/calc_utils.py
+-rw-r--r--   0        0        0     3372 2023-07-12 13:04:11.170016 jtimer-0.1.5/jtimer/controller/timer_controller.py
+-rw-r--r--   0        0        0     4241 2023-07-12 14:39:18.396294 jtimer-0.1.5/jtimer/dao/__init__.py
+-rw-r--r--   0        0        0      859 2023-07-12 13:53:33.879010 jtimer-0.1.5/jtimer/main.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:23:52.197749 jtimer-0.1.5/jtimer/model/__init__.py
+-rw-r--r--   0        0        0      467 2023-07-05 10:05:36.834824 jtimer-0.1.5/jtimer/model/time_event.py
+-rw-r--r--   0        0        0      788 2023-07-12 12:21:41.349459 jtimer-0.1.5/jtimer/model/timer.py
+-rw-r--r--   0        0        0      311 2023-07-12 14:41:27.196194 jtimer-0.1.5/jtimer/view/__init__.py
+-rw-r--r--   0        0        0     1468 2023-07-12 12:19:22.753431 jtimer-0.1.5/jtimer/view/stats_view.py
+-rw-r--r--   0        0        0     3379 2023-07-12 12:13:10.876234 jtimer-0.1.5/jtimer/view/timer_widget.py
+-rw-r--r--   0        0        0     2345 2023-07-12 12:19:21.753401 jtimer-0.1.5/jtimer/view/timers_view.py
+-rw-r--r--   0        0        0      698 2023-07-12 14:48:21.063741 jtimer-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-07-05 10:16:26.043062 jtimer-0.1.5/resources/schema.sql
+-rw-r--r--   0        0        0     1510 2023-07-12 14:49:04.663881 jtimer-0.1.5/setup.py
+-rw-r--r--   0        0        0     1198 2023-07-12 14:49:04.664084 jtimer-0.1.5/PKG-INFO
```

### Comparing `jtimer-0.1.4/README.md` & `jtimer-0.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Timer App
 
 DEVELOPMENT IN PROGRESS
 
 Dissatisfied with the selection of timer applications available in linux, I built my own.  It maintains a simple local db in /tmp
 
 The application is fairly simple:
-    * user can specify a list of different timers.
-    * timers can be renamed.
-    * timers can be started / stopped concurrently.
-    * on startup the timers will resume the count from the last start.
-    * timers should not cross over days. automatic stop times at 23:59:59 for forgotten timers.
-    * daily statistics view
+* user can specify a list of different timers.
+* timers can be renamed.
+* timers can be started / stopped concurrently.
+* on startup the timers will resume the count from the last start.
+* timers should not cross over days. automatic stop times at 23:59:59 for forgotten timers.
+* daily statistics view
 
 
 
 ## Installation
 ```bash
 pip install jtimer  # not timer
 ```
```

### Comparing `jtimer-0.1.4/images/add.png` & `jtimer-0.1.5/images/add.png`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/images/chart.png` & `jtimer-0.1.5/images/chart.png`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/images/delete.png` & `jtimer-0.1.5/images/delete.png`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/images/pause.png` & `jtimer-0.1.5/images/pause.png`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/images/pause2.png` & `jtimer-0.1.5/images/pause2.png`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/images/play.png` & `jtimer-0.1.5/images/play.png`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/images/play2.png` & `jtimer-0.1.5/images/play2.png`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/jtimer/controller/calc_utils.py` & `jtimer-0.1.5/jtimer/controller/calc_utils.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/jtimer/controller/timer_controller.py` & `jtimer-0.1.5/jtimer/controller/timer_controller.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/jtimer/dao/__init__.py` & `jtimer-0.1.5/jtimer/dao/__init__.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/jtimer/main.py` & `jtimer-0.1.5/jtimer/main.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/jtimer/model/timer.py` & `jtimer-0.1.5/jtimer/model/timer.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/jtimer/view/stats_view.py` & `jtimer-0.1.5/jtimer/view/stats_view.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/jtimer/view/timer_widget.py` & `jtimer-0.1.5/jtimer/view/timer_widget.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/jtimer/view/timers_view.py` & `jtimer-0.1.5/jtimer/view/timers_view.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.4/pyproject.toml` & `jtimer-0.1.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jtimer"
-version = "0.1.4"
+version = "0.1.5"
 description = "John's Timer - desktop app for tracking time"
 authors = ["John Watson <jmwdev@pm.me>"]
 maintainers = ["John Watson <jmwdev@pm.me>"]
 license = "GNU GENERAL PUBLIC LICENSE V3"
 readme = "README.md"
 keywords = ["productivity"]
 classifiers = [
```

### Comparing `jtimer-0.1.4/setup.py` & `jtimer-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['PyQt6>=6.5.1,<7.0.0']
 
 entry_points = \
 {'console_scripts': ['jtimer = jtimer.main:start']}
 
 setup_kwargs = {
     'name': 'jtimer',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': "John's Timer - desktop app for tracking time",
-    'long_description': '# Timer App\n\nDEVELOPMENT IN PROGRESS\n\nDissatisfied with the selection of timer applications available in linux, I built my own.  It maintains a simple local db in /tmp\n\nThe application is fairly simple:\n    * user can specify a list of different timers.\n    * timers can be renamed.\n    * timers can be started / stopped concurrently.\n    * on startup the timers will resume the count from the last start.\n    * timers should not cross over days. automatic stop times at 23:59:59 for forgotten timers.\n    * daily statistics view\n\n\n\n## Installation\n```bash\npip install jtimer  # not timer\n```\n\n## Usage\n```bash\njtimer\n```\n\n## Planned Future developments\n\n* timer linked triggers\n* timer event view',
+    'long_description': '# Timer App\n\nDEVELOPMENT IN PROGRESS\n\nDissatisfied with the selection of timer applications available in linux, I built my own.  It maintains a simple local db in /tmp\n\nThe application is fairly simple:\n* user can specify a list of different timers.\n* timers can be renamed.\n* timers can be started / stopped concurrently.\n* on startup the timers will resume the count from the last start.\n* timers should not cross over days. automatic stop times at 23:59:59 for forgotten timers.\n* daily statistics view\n\n\n\n## Installation\n```bash\npip install jtimer  # not timer\n```\n\n## Usage\n```bash\njtimer\n```\n\n## Planned Future developments\n\n* timer linked triggers\n* timer event view',
     'author': 'John Watson',
     'author_email': 'jmwdev@pm.me',
     'maintainer': 'John Watson',
     'maintainer_email': 'jmwdev@pm.me',
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `jtimer-0.1.4/PKG-INFO` & `jtimer-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtimer
-Version: 0.1.4
+Version: 0.1.5
 Summary: John's Timer - desktop app for tracking time
 License: GNU GENERAL PUBLIC LICENSE V3
 Keywords: productivity
 Author: John Watson
 Author-email: jmwdev@pm.me
 Maintainer: John Watson
 Maintainer-email: jmwdev@pm.me
@@ -18,20 +18,20 @@
 # Timer App
 
 DEVELOPMENT IN PROGRESS
 
 Dissatisfied with the selection of timer applications available in linux, I built my own.  It maintains a simple local db in /tmp
 
 The application is fairly simple:
-    * user can specify a list of different timers.
-    * timers can be renamed.
-    * timers can be started / stopped concurrently.
-    * on startup the timers will resume the count from the last start.
-    * timers should not cross over days. automatic stop times at 23:59:59 for forgotten timers.
-    * daily statistics view
+* user can specify a list of different timers.
+* timers can be renamed.
+* timers can be started / stopped concurrently.
+* on startup the timers will resume the count from the last start.
+* timers should not cross over days. automatic stop times at 23:59:59 for forgotten timers.
+* daily statistics view
 
 
 
 ## Installation
 ```bash
 pip install jtimer  # not timer
 ```
```

