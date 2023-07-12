# Comparing `tmp/jtimer-0.1.3.tar.gz` & `tmp/jtimer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtimer-0.1.3.tar", max compression
+gzip compressed data, was "jtimer-0.1.4.tar", max compression
```

## Comparing `jtimer-0.1.3.tar` & `jtimer-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,25 @@
--rw-r--r--   0        0        0      697 2023-07-12 13:34:25.335708 jtimer-0.1.3/README.md
--rw-r--r--   0        0        0       38 2023-07-12 13:54:28.533999 jtimer-0.1.3/jtimer/__init__.py
--rw-r--r--   0        0        0      353 2023-07-12 12:22:04.706105 jtimer-0.1.3/jtimer/controller/__init__.py
--rw-r--r--   0        0        0     1122 2023-07-12 12:22:04.698105 jtimer-0.1.3/jtimer/controller/calc_utils.py
--rw-r--r--   0        0        0     3372 2023-07-12 13:04:11.170016 jtimer-0.1.3/jtimer/controller/timer_controller.py
--rw-r--r--   0        0        0     4187 2023-07-12 12:39:08.646493 jtimer-0.1.3/jtimer/dao/__init__.py
--rw-r--r--   0        0        0      859 2023-07-12 13:53:33.879010 jtimer-0.1.3/jtimer/main.py
--rw-r--r--   0        0        0        0 2023-07-02 23:23:52.197749 jtimer-0.1.3/jtimer/model/__init__.py
--rw-r--r--   0        0        0      467 2023-07-05 10:05:36.834824 jtimer-0.1.3/jtimer/model/time_event.py
--rw-r--r--   0        0        0      788 2023-07-12 12:21:41.349459 jtimer-0.1.3/jtimer/model/timer.py
--rw-r--r--   0        0        0      158 2023-07-05 08:39:15.858177 jtimer-0.1.3/jtimer/view/__init__.py
--rw-r--r--   0        0        0     1468 2023-07-12 12:19:22.753431 jtimer-0.1.3/jtimer/view/stats_view.py
--rw-r--r--   0        0        0     3379 2023-07-12 12:13:10.876234 jtimer-0.1.3/jtimer/view/timer_widget.py
--rw-r--r--   0        0        0     2345 2023-07-12 12:19:21.753401 jtimer-0.1.3/jtimer/view/timers_view.py
--rw-r--r--   0        0        0      735 2023-07-12 13:54:22.658104 jtimer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1644 2023-07-12 13:54:34.348152 jtimer-0.1.3/setup.py
--rw-r--r--   0        0        0     1222 2023-07-12 13:54:34.348348 jtimer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      697 2023-07-12 13:34:25.335708 jtimer-0.1.4/README.md
+-rw-r--r--   0        0        0   110370 2023-07-03 00:50:37.905521 jtimer-0.1.4/images/add.png
+-rw-r--r--   0        0        0     3023 2023-07-02 11:38:21.202742 jtimer-0.1.4/images/chart.png
+-rw-r--r--   0        0        0   185230 2023-07-03 00:47:33.188869 jtimer-0.1.4/images/delete.png
+-rw-r--r--   0        0        0    30477 2023-06-28 11:38:32.874181 jtimer-0.1.4/images/pause.png
+-rw-r--r--   0        0        0     3507 2023-06-28 11:43:04.759846 jtimer-0.1.4/images/pause2.png
+-rw-r--r--   0        0        0    40030 2023-06-28 11:33:57.440503 jtimer-0.1.4/images/play.png
+-rw-r--r--   0        0        0    53318 2023-06-28 11:43:04.739846 jtimer-0.1.4/images/play2.png
+-rw-r--r--   0        0        0       38 2023-07-12 14:44:20.004024 jtimer-0.1.4/jtimer/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-12 12:22:04.706105 jtimer-0.1.4/jtimer/controller/__init__.py
+-rw-r--r--   0        0        0     1122 2023-07-12 12:22:04.698105 jtimer-0.1.4/jtimer/controller/calc_utils.py
+-rw-r--r--   0        0        0     3372 2023-07-12 13:04:11.170016 jtimer-0.1.4/jtimer/controller/timer_controller.py
+-rw-r--r--   0        0        0     4241 2023-07-12 14:39:18.396294 jtimer-0.1.4/jtimer/dao/__init__.py
+-rw-r--r--   0        0        0      859 2023-07-12 13:53:33.879010 jtimer-0.1.4/jtimer/main.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:23:52.197749 jtimer-0.1.4/jtimer/model/__init__.py
+-rw-r--r--   0        0        0      467 2023-07-05 10:05:36.834824 jtimer-0.1.4/jtimer/model/time_event.py
+-rw-r--r--   0        0        0      788 2023-07-12 12:21:41.349459 jtimer-0.1.4/jtimer/model/timer.py
+-rw-r--r--   0        0        0      311 2023-07-12 14:41:27.196194 jtimer-0.1.4/jtimer/view/__init__.py
+-rw-r--r--   0        0        0     1468 2023-07-12 12:19:22.753431 jtimer-0.1.4/jtimer/view/stats_view.py
+-rw-r--r--   0        0        0     3379 2023-07-12 12:13:10.876234 jtimer-0.1.4/jtimer/view/timer_widget.py
+-rw-r--r--   0        0        0     2345 2023-07-12 12:19:21.753401 jtimer-0.1.4/jtimer/view/timers_view.py
+-rw-r--r--   0        0        0      698 2023-07-12 14:44:15.732029 jtimer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-07-05 10:16:26.043062 jtimer-0.1.4/resources/schema.sql
+-rw-r--r--   0        0        0     1534 2023-07-12 14:46:15.130725 jtimer-0.1.4/setup.py
+-rw-r--r--   0        0        0     1222 2023-07-12 14:46:15.130896 jtimer-0.1.4/PKG-INFO
```

### Comparing `jtimer-0.1.3/README.md` & `jtimer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.3/jtimer/controller/calc_utils.py` & `jtimer-0.1.4/jtimer/controller/calc_utils.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.3/jtimer/controller/timer_controller.py` & `jtimer-0.1.4/jtimer/controller/timer_controller.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.3/jtimer/dao/__init__.py` & `jtimer-0.1.4/jtimer/dao/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from datetime import date, datetime
 import sqlite3
-
+from importlib import resources
 from jtimer.model.time_event import TimeEvent, TimeEventType
 from jtimer.model.timer import Timer
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S.%f"
 
 
 class DAO:
     def __init__(self, db_name: str) -> None:
         self.db_name = db_name
         conn = self.connect()
         if not conn.execute(
             "SELECT name FROM sqlite_master WHERE name = 'timer'"
         ).fetchone():
-            with open("schema.sql", "r") as f:
+            with resources.open_text("resources", "schema.sql") as f:
                 conn.executescript(f.read())
             conn.commit()
         conn.close()
         self.next_id = 0
 
     def connect(self) -> sqlite3.Connection:
         return sqlite3.connect(self.db_name)
```

### Comparing `jtimer-0.1.3/jtimer/main.py` & `jtimer-0.1.4/jtimer/main.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.3/jtimer/model/timer.py` & `jtimer-0.1.4/jtimer/model/timer.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.3/jtimer/view/stats_view.py` & `jtimer-0.1.4/jtimer/view/stats_view.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.3/jtimer/view/timer_widget.py` & `jtimer-0.1.4/jtimer/view/timer_widget.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.3/jtimer/view/timers_view.py` & `jtimer-0.1.4/jtimer/view/timers_view.py`

 * *Files identical despite different names*

### Comparing `jtimer-0.1.3/pyproject.toml` & `jtimer-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 [tool.poetry]
 name = "jtimer"
-version = "0.1.3"
+version = "0.1.4"
 description = "John's Timer - desktop app for tracking time"
 authors = ["John Watson <jmwdev@pm.me>"]
 maintainers = ["John Watson <jmwdev@pm.me>"]
 license = "GNU GENERAL PUBLIC LICENSE V3"
 readme = "README.md"
 keywords = ["productivity"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
+include = ["resources", "images"]
+
 [tool.poetry.scripts]
 jtimer = "jtimer.main:start"
 
-packages = [
-    {include = "jtimer" },
-    {include = "schema.sql"}
-]
-
 [tool.poetry.dependencies]
 python = "^3.10.6"
 PyQt6 = "^6.5.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
```

### Comparing `jtimer-0.1.3/setup.py` & `jtimer-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyQt6>=6.5.1,<7.0.0']
 
 entry_points = \
-{'console_scripts': ['jtimer = jtimer.main:start',
-                     "packages = [{'include': 'jtimer'}, {'include': "
-                     "'schema.sql'}]"]}
+{'console_scripts': ['jtimer = jtimer.main:start']}
 
 setup_kwargs = {
     'name': 'jtimer',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': "John's Timer - desktop app for tracking time",
     'long_description': '# Timer App\n\nDEVELOPMENT IN PROGRESS\n\nDissatisfied with the selection of timer applications available in linux, I built my own.  It maintains a simple local db in /tmp\n\nThe application is fairly simple:\n    * user can specify a list of different timers.\n    * timers can be renamed.\n    * timers can be started / stopped concurrently.\n    * on startup the timers will resume the count from the last start.\n    * timers should not cross over days. automatic stop times at 23:59:59 for forgotten timers.\n    * daily statistics view\n\n\n\n## Installation\n```bash\npip install jtimer  # not timer\n```\n\n## Usage\n```bash\njtimer\n```\n\n## Planned Future developments\n\n* timer linked triggers\n* timer event view',
     'author': 'John Watson',
     'author_email': 'jmwdev@pm.me',
     'maintainer': 'John Watson',
     'maintainer_email': 'jmwdev@pm.me',
     'url': None,
```

### Comparing `jtimer-0.1.3/PKG-INFO` & `jtimer-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtimer
-Version: 0.1.3
+Version: 0.1.4
 Summary: John's Timer - desktop app for tracking time
 License: GNU GENERAL PUBLIC LICENSE V3
 Keywords: productivity
 Author: John Watson
 Author-email: jmwdev@pm.me
 Maintainer: John Watson
 Maintainer-email: jmwdev@pm.me
```

