# Comparing `tmp/common-task-system-client-1.1.3.tar.gz` & `tmp/common-task-system-client-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-task-system-client-1.1.3.tar", last modified: Thu May 25 05:22:27 2023, max compression
+gzip compressed data, was "common-task-system-client-1.1.4.tar", last modified: Wed Jul 12 07:43:04 2023, max compression
```

## Comparing `common-task-system-client-1.1.3.tar` & `common-task-system-client-1.1.4.tar`

### file list

```diff
@@ -1,51 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.755390 common-task-system-client-1.1.3/
--rw-rw-rw-   0        0        0     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      302 2023-05-25 05:22:27.754390 common-task-system-client-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-20 07:10:46.000000 common-task-system-client-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.736548 common-task-system-client-1.1.3/common_task_system_client.egg-info/
--rw-rw-rw-   0        0        0      302 2023-05-25 05:22:27.000000 common-task-system-client-1.1.3/common_task_system_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1499 2023-05-25 05:22:27.000000 common-task-system-client-1.1.3/common_task_system_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 05:22:27.000000 common-task-system-client-1.1.3/common_task_system_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-25 05:22:27.000000 common-task-system-client-1.1.3/common_task_system_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-25 05:22:27.000000 common-task-system-client-1.1.3/common_task_system_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 05:22:27.755390 common-task-system-client-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-05-25 05:14:28.000000 common-task-system-client-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.738554 common-task-system-client-1.1.3/task_system_client/
--rw-rw-rw-   0        0        0        0 2023-02-20 07:12:05.000000 common-task-system-client-1.1.3/task_system_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.739555 common-task-system-client-1.1.3/task_system_client/callback/
--rw-rw-rw-   0        0        0       42 2023-03-17 05:21:49.000000 common-task-system-client-1.1.3/task_system_client/callback/__init__.py
--rw-rw-rw-   0        0        0      490 2023-03-17 06:56:57.000000 common-task-system-client-1.1.3/task_system_client/callback/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.740554 common-task-system-client-1.1.3/task_system_client/callback/callbacks/
--rw-rw-rw-   0        0        0        0 2023-03-17 03:52:57.000000 common-task-system-client-1.1.3/task_system_client/callback/callbacks/__init__.py
--rw-rw-rw-   0        0        0      701 2023-03-23 01:18:51.000000 common-task-system-client-1.1.3/task_system_client/callback/callbacks/upload_log.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.742554 common-task-system-client-1.1.3/task_system_client/executor/
--rw-rw-rw-   0        0        0      193 2023-03-14 03:27:53.000000 common-task-system-client-1.1.3/task_system_client/executor/__init__.py
--rw-rw-rw-   0        0        0      711 2023-05-25 01:59:12.000000 common-task-system-client-1.1.3/task_system_client/executor/base.py
--rw-rw-rw-   0        0        0     1854 2023-05-23 09:53:37.000000 common-task-system-client-1.1.3/task_system_client/executor/executor.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.743555 common-task-system-client-1.1.3/task_system_client/handler/
--rw-rw-rw-   0        0        0      277 2023-04-21 03:33:18.000000 common-task-system-client-1.1.3/task_system_client/handler/__init__.py
--rw-rw-rw-   0        0        0      166 2023-04-21 03:13:13.000000 common-task-system-client-1.1.3/task_system_client/handler/base.py
--rw-rw-rw-   0        0        0      732 2023-04-21 08:24:39.000000 common-task-system-client-1.1.3/task_system_client/handler/exception.py
--rw-rw-rw-   0        0        0      382 2023-03-16 03:20:59.000000 common-task-system-client-1.1.3/task_system_client/main.py
--rw-rw-rw-   0        0        0     1888 2023-04-21 05:42:56.000000 common-task-system-client-1.1.3/task_system_client/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.745554 common-task-system-client-1.1.3/task_system_client/subscriber/
--rw-rw-rw-   0        0        0      541 2023-04-21 03:36:06.000000 common-task-system-client-1.1.3/task_system_client/subscriber/__init__.py
--rw-rw-rw-   0        0        0     4009 2023-05-25 05:21:41.000000 common-task-system-client-1.1.3/task_system_client/subscriber/base.py
--rw-rw-rw-   0        0        0     4656 2023-05-22 06:58:46.000000 common-task-system-client-1.1.3/task_system_client/subscriber/threaded.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.746554 common-task-system-client-1.1.3/task_system_client/task_center/
--rw-rw-rw-   0        0        0      130 2023-02-22 05:09:58.000000 common-task-system-client-1.1.3/task_system_client/task_center/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.747777 common-task-system-client-1.1.3/task_system_client/task_center/dispatch/
--rw-rw-rw-   0        0        0      286 2023-02-27 02:22:48.000000 common-task-system-client-1.1.3/task_system_client/task_center/dispatch/__init__.py
--rw-rw-rw-   0        0        0      857 2023-03-17 09:28:16.000000 common-task-system-client-1.1.3/task_system_client/task_center/dispatch/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.751390 common-task-system-client-1.1.3/task_system_client/task_center/subscription/
--rw-rw-rw-   0        0        0      487 2023-02-27 02:22:30.000000 common-task-system-client-1.1.3/task_system_client/task_center/subscription/__init__.py
--rw-rw-rw-   0        0        0     1132 2023-05-22 06:58:46.000000 common-task-system-client-1.1.3/task_system_client/task_center/subscription/base.py
--rw-rw-rw-   0        0        0     1218 2023-05-22 06:58:46.000000 common-task-system-client-1.1.3/task_system_client/task_center/subscription/http.py
--rw-rw-rw-   0        0        0      553 2023-05-22 06:58:46.000000 common-task-system-client-1.1.3/task_system_client/task_center/subscription/redis.py
--rw-rw-rw-   0        0        0      659 2023-05-22 06:58:46.000000 common-task-system-client-1.1.3/task_system_client/task_center/subscription/sql.py
--rw-rw-rw-   0        0        0     2254 2023-05-25 05:15:00.000000 common-task-system-client-1.1.3/task_system_client/task_center/task.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:22:27.753390 common-task-system-client-1.1.3/task_system_client/utils/
--rw-rw-rw-   0        0        0        0 2023-02-20 09:58:14.000000 common-task-system-client-1.1.3/task_system_client/utils/__init__.py
--rw-rw-rw-   0        0        0      428 2023-02-22 03:46:05.000000 common-task-system-client-1.1.3/task_system_client/utils/class_loader.py
--rw-rw-rw-   0        0        0     2627 2023-02-27 01:52:51.000000 common-task-system-client-1.1.3/task_system_client/utils/db_utils.py
--rw-rw-rw-   0        0        0     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.1.3/task_system_client/utils/module_loading.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:04.100700 common-task-system-client-1.1.4/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.1.4/LICENSE
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      288 2023-07-12 07:43:04.097334 common-task-system-client-1.1.4/PKG-INFO
+-rwxrwxrwx   0 cone      (1000) cone      (1000)       24 2023-02-20 07:10:46.000000 common-task-system-client-1.1.4/README.md
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:02.683238 common-task-system-client-1.1.4/common_task_system_client.egg-info/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      288 2023-07-12 07:43:01.000000 common-task-system-client-1.1.4/common_task_system_client.egg-info/PKG-INFO
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1780 2023-07-12 07:43:02.000000 common-task-system-client-1.1.4/common_task_system_client.egg-info/SOURCES.txt
+-rwxrwxrwx   0 cone      (1000) cone      (1000)        1 2023-07-12 07:43:01.000000 common-task-system-client-1.1.4/common_task_system_client.egg-info/dependency_links.txt
+-rwxrwxrwx   0 cone      (1000) cone      (1000)       89 2023-07-12 07:43:01.000000 common-task-system-client-1.1.4/common_task_system_client.egg-info/entry_points.txt
+-rwxrwxrwx   0 cone      (1000) cone      (1000)       15 2023-07-12 07:43:01.000000 common-task-system-client-1.1.4/common_task_system_client.egg-info/requires.txt
+-rwxrwxrwx   0 cone      (1000) cone      (1000)       19 2023-07-12 07:43:01.000000 common-task-system-client-1.1.4/common_task_system_client.egg-info/top_level.txt
+-rwxrwxrwx   0 cone      (1000) cone      (1000)       38 2023-07-12 07:43:04.101698 common-task-system-client-1.1.4/setup.cfg
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      578 2023-07-12 07:42:08.000000 common-task-system-client-1.1.4/setup.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:02.760565 common-task-system-client-1.1.4/task_system_client/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-02-20 07:12:05.000000 common-task-system-client-1.1.4/task_system_client/__init__.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:02.828603 common-task-system-client-1.1.4/task_system_client/callback/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)       42 2023-03-17 05:21:49.000000 common-task-system-client-1.1.4/task_system_client/callback/__init__.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      405 2023-06-15 08:34:51.000000 common-task-system-client-1.1.4/task_system_client/callback/base.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:02.912162 common-task-system-client-1.1.4/task_system_client/callback/callbacks/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-03-17 03:52:57.000000 common-task-system-client-1.1.4/task_system_client/callback/callbacks/__init__.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      701 2023-03-23 01:18:51.000000 common-task-system-client-1.1.4/task_system_client/callback/callbacks/upload_log.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:03.033239 common-task-system-client-1.1.4/task_system_client/executor/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      252 2023-06-15 09:39:15.000000 common-task-system-client-1.1.4/task_system_client/executor/__init__.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1170 2023-06-15 09:02:43.000000 common-task-system-client-1.1.4/task_system_client/executor/base.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1900 2023-06-28 09:41:22.000000 common-task-system-client-1.1.4/task_system_client/executor/executor.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:03.286194 common-task-system-client-1.1.4/task_system_client/executor/system/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)       34 2023-06-29 01:30:31.000000 common-task-system-client-1.1.4/task_system_client/executor/system/__init__.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      161 2023-06-29 08:32:09.000000 common-task-system-client-1.1.4/task_system_client/executor/system/base.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     5762 2023-06-29 01:38:35.000000 common-task-system-client-1.1.4/task_system_client/executor/system/custom_program.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      899 2023-06-29 03:37:01.000000 common-task-system-client-1.1.4/task_system_client/executor/system/shell.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1403 2023-06-29 03:37:01.000000 common-task-system-client-1.1.4/task_system_client/executor/system/sql.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:03.408884 common-task-system-client-1.1.4/task_system_client/handler/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      277 2023-04-21 03:33:18.000000 common-task-system-client-1.1.4/task_system_client/handler/__init__.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      166 2023-04-21 03:13:13.000000 common-task-system-client-1.1.4/task_system_client/handler/base.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      732 2023-04-21 08:24:39.000000 common-task-system-client-1.1.4/task_system_client/handler/exception.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1504 2023-06-28 09:57:01.000000 common-task-system-client-1.1.4/task_system_client/main.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     3494 2023-06-29 03:30:38.000000 common-task-system-client-1.1.4/task_system_client/settings.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:03.531818 common-task-system-client-1.1.4/task_system_client/subscriber/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      541 2023-04-21 03:36:06.000000 common-task-system-client-1.1.4/task_system_client/subscriber/__init__.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     4053 2023-06-29 03:53:46.000000 common-task-system-client-1.1.4/task_system_client/subscriber/base.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     4656 2023-05-22 06:58:46.000000 common-task-system-client-1.1.4/task_system_client/subscriber/threaded.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:03.607125 common-task-system-client-1.1.4/task_system_client/task_center/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      130 2023-02-22 05:09:58.000000 common-task-system-client-1.1.4/task_system_client/task_center/__init__.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:03.694177 common-task-system-client-1.1.4/task_system_client/task_center/dispatch/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      519 2023-06-28 10:01:37.000000 common-task-system-client-1.1.4/task_system_client/task_center/dispatch/__init__.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     4596 2023-06-29 01:56:42.000000 common-task-system-client-1.1.4/task_system_client/task_center/dispatch/dispatcher.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:03.917072 common-task-system-client-1.1.4/task_system_client/task_center/subscription/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      487 2023-02-27 02:22:30.000000 common-task-system-client-1.1.4/task_system_client/task_center/subscription/__init__.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1132 2023-05-22 06:58:46.000000 common-task-system-client-1.1.4/task_system_client/task_center/subscription/base.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1218 2023-06-15 08:32:17.000000 common-task-system-client-1.1.4/task_system_client/task_center/subscription/http.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      553 2023-05-22 06:58:46.000000 common-task-system-client-1.1.4/task_system_client/task_center/subscription/redis.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      657 2023-06-15 08:32:17.000000 common-task-system-client-1.1.4/task_system_client/task_center/subscription/sql.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1726 2023-06-15 08:56:19.000000 common-task-system-client-1.1.4/task_system_client/task_center/task.py
+drwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-07-12 07:43:04.064821 common-task-system-client-1.1.4/task_system_client/utils/
+-rwxrwxrwx   0 cone      (1000) cone      (1000)        0 2023-02-20 09:58:14.000000 common-task-system-client-1.1.4/task_system_client/utils/__init__.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)      428 2023-02-22 03:46:05.000000 common-task-system-client-1.1.4/task_system_client/utils/class_loader.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     2625 2023-06-15 08:42:58.000000 common-task-system-client-1.1.4/task_system_client/utils/db_utils.py
+-rwxrwxrwx   0 cone      (1000) cone      (1000)     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.1.4/task_system_client/utils/module_loading.py
```

### Comparing `common-task-system-client-1.1.3/LICENSE` & `common-task-system-client-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.3/common_task_system_client.egg-info/SOURCES.txt` & `common-task-system-client-1.1.4/common_task_system_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 LICENSE
 README.md
 setup.py
 common_task_system_client.egg-info/PKG-INFO
 common_task_system_client.egg-info/SOURCES.txt
 common_task_system_client.egg-info/dependency_links.txt
+common_task_system_client.egg-info/entry_points.txt
 common_task_system_client.egg-info/requires.txt
 common_task_system_client.egg-info/top_level.txt
 task_system_client/__init__.py
 task_system_client/main.py
 task_system_client/settings.py
 task_system_client/callback/__init__.py
 task_system_client/callback/base.py
 task_system_client/callback/callbacks/__init__.py
 task_system_client/callback/callbacks/upload_log.py
 task_system_client/executor/__init__.py
 task_system_client/executor/base.py
 task_system_client/executor/executor.py
+task_system_client/executor/system/__init__.py
+task_system_client/executor/system/base.py
+task_system_client/executor/system/custom_program.py
+task_system_client/executor/system/shell.py
+task_system_client/executor/system/sql.py
 task_system_client/handler/__init__.py
 task_system_client/handler/base.py
 task_system_client/handler/exception.py
 task_system_client/subscriber/__init__.py
 task_system_client/subscriber/base.py
 task_system_client/subscriber/threaded.py
 task_system_client/task_center/__init__.py
```

### Comparing `common-task-system-client-1.1.3/task_system_client/callback/callbacks/upload_log.py` & `common-task-system-client-1.1.4/task_system_client/callback/callbacks/upload_log.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.3/task_system_client/executor/executor.py` & `common-task-system-client-1.1.4/task_system_client/executor/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from task_system_client.task_center.task import TaskSchedule
-from .base import ExecuteStatus
+from task_system_client.executor.base import ExecuteStatus
 from task_system_client.callback import Callback
 import time
 
 
 class BaseExecutor(object):
     category = None
+    parent = None
     name = None
 
     def __init__(self, schedule: TaskSchedule):
         self.schedule = schedule
         self.task = schedule.task
         self.result = {
             'generator': self.schedule.generator,
```

### Comparing `common-task-system-client-1.1.3/task_system_client/handler/exception.py` & `common-task-system-client-1.1.4/task_system_client/handler/exception.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.3/task_system_client/subscriber/__init__.py` & `common-task-system-client-1.1.4/task_system_client/subscriber/__init__.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.3/task_system_client/subscriber/base.py` & `common-task-system-client-1.1.4/task_system_client/subscriber/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,18 @@
         self.subscription = create_subscription(self.SUBSCRIPTION or SUBSCRIPTION)
         self.exception_handler = None
         if ExceptionHandler is not None:
             self.exception_handler: BaseHandler = ExceptionHandler()
 
     def run_synchronous(self, executor):
         try:
-            executor.run()
+            executor.result['logs'] = executor.run()
         except EmptyResult:
             executor.execute_status = ExecuteStatus.EMPTY
-        except NoRetryException as e:
+        except (NoRetryException, NotImplementedError) as e:
             executor.execute_status = ExecuteStatus.ERROR_BUT_NO_RETRY
             executor.result['error'] = str(e)
         except TimeoutException as e:
             executor.execute_status = ExecuteStatus.TIMEOUT
             executor.result['error'] = str(e)
         except Exception as e:
             executor.execute_status = ExecuteStatus.FAILED
@@ -95,15 +95,15 @@
                 if not schedule:
                     time.sleep(1)
                     continue
                 executor = dispatch(schedule)
                 if self.is_executable(executor):
                     self.run_executor(executor)
                 else:
-                    self.subscription.put(executor.schedule)
+                    subscription.put(executor.schedule)
             except Exception as e:
                 self.on_exception(e)
 
     def start(self):
         self._state.set()
         self.run()
```

### Comparing `common-task-system-client-1.1.3/task_system_client/subscriber/threaded.py` & `common-task-system-client-1.1.4/task_system_client/subscriber/threaded.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.3/task_system_client/task_center/subscription/base.py` & `common-task-system-client-1.1.4/task_system_client/task_center/subscription/base.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.3/task_system_client/task_center/subscription/http.py` & `common-task-system-client-1.1.4/task_system_client/task_center/subscription/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 except ImportError:
     raise ImportError('requests is required for http subscription, please install requests first')
 
 import logging
 import time
 from sys import stdout
 from typing import Union
-
 from .base import BaseSubscription
 from ..task import TaskSchedule
 
 logger = logging.getLogger(__name__)
 
 
 class HttpSubscription(BaseSubscription):
@@ -28,8 +27,8 @@
             stdout.write('[%s]no more schedule now, wait 1 second...\r' % time.strftime('%Y-%m-%d %H:%M:%S'))
             stdout.flush()
         else:
             # 有可能存在500情况是被nginx代理的，所以输出response.text不会错
             stdout.write('[%s]get schedule error, status code: %s\n' % (
                 time.strftime('%Y-%m-%d %H:%M:%S'), response.text))
             stdout.flush()
-        return None
+        return None
```

### Comparing `common-task-system-client-1.1.3/task_system_client/task_center/subscription/redis.py` & `common-task-system-client-1.1.4/task_system_client/task_center/subscription/redis.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.1.3/task_system_client/task_center/subscription/sql.py` & `common-task-system-client-1.1.4/task_system_client/task_center/subscription/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,7 @@
 
     def request(self):
         self.cursor.execute(self.schedule)
         return self.cursor.fetchall()
 
     def stop(self):
         self.connection.close()
-
```

### Comparing `common-task-system-client-1.1.3/task_system_client/task_center/task.py` & `common-task-system-client-1.1.4/task_system_client/task_center/task.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,38 +17,21 @@
 
 
 class Task:
 
     def __init__(self, task):
         self.id = task['id']
         self.name = task['name']
-        self.category = Category(task['category'])
+        self.category = Category(task['category']) if task.get('category') else None
         self.config = task.get('config') or {}
         self.parent = Task(task['parent']) if task.get('parent') else None
         self.content = task
 
-        parent = self.parent
-        names = [self.name]
-        while parent:
-            names.append(parent.name)
-            parent = parent.parent
-        self.unique_name = '-'.join(reversed(names))
-
-        if self.category:
-            names = [self.category.name]
-            parent = self.category.parent
-            while parent:
-                names.append(parent.name)
-                parent = parent.parent
-            self.unique_category = '-'.join(reversed(names))
-        else:
-            self.unique_category = None
-
     def __str__(self):
-        return 'Task(id=%s, name=%s)' % (self.id, self.unique_name)
+        return 'Task(id=%s, name=%s)' % (self.id, self.name)
 
     __repr__ = __str__
 
 
 class TaskSchedule:
 
     def __init__(self, schedule):
```

### Comparing `common-task-system-client-1.1.3/task_system_client/utils/db_utils.py` & `common-task-system-client-1.1.4/task_system_client/utils/db_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,7 @@
         except Exception as e:
             logger.exception("delete failed: %s, cmd is %s" % (e, cmd))
             return 0
     conn.commit()
     conn.close()
     logger.debug("delete %s rows from %s where %s" % (r, table, ' and '.join(children)))
     return r
-
```

### Comparing `common-task-system-client-1.1.3/task_system_client/utils/module_loading.py` & `common-task-system-client-1.1.4/task_system_client/utils/module_loading.py`

 * *Files identical despite different names*

