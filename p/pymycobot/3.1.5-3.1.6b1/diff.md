# Comparing `tmp/pymycobot-3.1.5.tar.gz` & `tmp/pymycobot-3.1.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.1.5.tar", last modified: Thu Jul  6 03:10:49 2023, max compression
+gzip compressed data, was "pymycobot-3.1.6b1.tar", last modified: Wed Jul 12 07:38:37 2023, max compression
```

## Comparing `pymycobot-3.1.5.tar` & `pymycobot-3.1.6b1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 03:10:49.008346 pymycobot-3.1.5/
--rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.5/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0    59799 2023-07-06 03:10:49.007334 pymycobot-3.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 03:10:48.970371 pymycobot-3.1.5/pymycobot/
--rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.5/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     1627 2023-07-06 02:42:11.000000 pymycobot-3.1.5/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.5/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    12339 2023-07-06 02:36:59.000000 pymycobot-3.1.5/pymycobot/common.py
--rw-rw-rw-   0        0        0     9159 2023-07-05 06:05:50.000000 pymycobot-3.1.5/pymycobot/elephantrobot.py
--rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.5/pymycobot/error.py
--rw-rw-rw-   0        0        0    34521 2023-07-06 02:36:43.000000 pymycobot-3.1.5/pymycobot/generate.py
--rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.5/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.5/pymycobot/log.py
--rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.5/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     9080 2023-06-27 03:24:18.000000 pymycobot-3.1.5/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    13314 2023-06-27 03:24:50.000000 pymycobot-3.1.5/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.5/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.5/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.5/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     7725 2023-07-06 02:40:02.000000 pymycobot-3.1.5/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.5/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     8707 2023-07-06 02:41:09.000000 pymycobot-3.1.5/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.5/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0    19696 2023-06-27 03:25:03.000000 pymycobot-3.1.5/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.5/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:10:49.005329 pymycobot-3.1.5/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    59799 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 03:10:49.009351 pymycobot-3.1.5/setup.cfg
--rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:38:37.013070 pymycobot-3.1.6b1/
+-rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.6b1/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.6b1/MANIFEST.in
+-rw-rw-rw-   0        0        0    59801 2023-07-12 07:38:37.011678 pymycobot-3.1.6b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.6b1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 07:38:36.972582 pymycobot-3.1.6b1/pymycobot/
+-rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.6b1/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     1681 2023-07-12 07:37:42.000000 pymycobot-3.1.6b1/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.6b1/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0      201 2023-07-12 07:37:01.000000 pymycobot-3.1.6b1/pymycobot/cobotx.py
+-rw-rw-rw-   0        0        0    12339 2023-07-06 06:16:02.000000 pymycobot-3.1.6b1/pymycobot/common.py
+-rw-rw-rw-   0        0        0     9159 2023-07-05 06:05:50.000000 pymycobot-3.1.6b1/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.6b1/pymycobot/error.py
+-rw-rw-rw-   0        0        0    34521 2023-07-06 02:36:43.000000 pymycobot-3.1.6b1/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.6b1/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.6b1/pymycobot/log.py
+-rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.6b1/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     9080 2023-06-27 03:24:18.000000 pymycobot-3.1.6b1/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    13314 2023-06-27 03:24:50.000000 pymycobot-3.1.6b1/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.6b1/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.6b1/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.6b1/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     7725 2023-07-06 02:40:02.000000 pymycobot-3.1.6b1/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.6b1/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     8707 2023-07-06 02:41:09.000000 pymycobot-3.1.6b1/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.6b1/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0    19696 2023-06-27 03:25:03.000000 pymycobot-3.1.6b1/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.6b1/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:38:37.009201 pymycobot-3.1.6b1/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    59801 2023-07-12 07:38:36.000000 pymycobot-3.1.6b1/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-07-12 07:38:36.000000 pymycobot-3.1.6b1/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 07:38:36.000000 pymycobot-3.1.6b1/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 07:38:36.000000 pymycobot-3.1.6b1/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 07:38:36.000000 pymycobot-3.1.6b1/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.6b1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 07:38:37.013070 pymycobot-3.1.6b1/setup.cfg
+-rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.6b1/setup.py
```

### Comparing `pymycobot-3.1.5/LICENSE` & `pymycobot-3.1.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/PKG-INFO` & `pymycobot-3.1.6b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.5
+Version: 3.1.6b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `pymycobot-3.1.5/README.md` & `pymycobot-3.1.6b1/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/Interface.py` & `pymycobot-3.1.6b1/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/__init__.py` & `pymycobot-3.1.6b1/pymycobot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pymycobot import utils
 from pymycobot.mybuddysocket import MyBuddySocket
 from pymycobot.ultraArm import ultraArm
 from pymycobot.mybuddybluetooth import MyBuddyBlueTooth
 from pymycobot.mypalletizersocket import MyPalletizerSocket
 from pymycobot.myarm import MyArm
 from pymycobot.elephantrobot import ElephantRobot
+from pymycobot.cobotx import CobotX
 
 __all__ = [
     "MyCobot",
     "MyCobotCommandGenerator",
     "Angle",
     "Coord",
     "utils",
@@ -32,23 +33,24 @@
     "MyBuddy",
     "MyBuddySocket",
     "MyBuddyBlueTooth",
     "ultraArm",
     "MyPalletizerSocket",
     "MechArm",
     "MyArm",
-    "ElephantRobot"
+    "ElephantRobot",
+    "CobotX"
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.1.5"
+__version__ = "3.1.6b1"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.1.5/pymycobot/bluet.py` & `pymycobot-3.1.6b1/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/common.py` & `pymycobot-3.1.6b1/pymycobot/common.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/elephantrobot.py` & `pymycobot-3.1.6b1/pymycobot/elephantrobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/error.py` & `pymycobot-3.1.6b1/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/generate.py` & `pymycobot-3.1.6b1/pymycobot/generate.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/log.py` & `pymycobot-3.1.6b1/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/myarm.py` & `pymycobot-3.1.6b1/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/mybuddy.py` & `pymycobot-3.1.6b1/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/mybuddybluetooth.py` & `pymycobot-3.1.6b1/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/mybuddyemoticon.py` & `pymycobot-3.1.6b1/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/mybuddysocket.py` & `pymycobot-3.1.6b1/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/mycobot.py` & `pymycobot-3.1.6b1/pymycobot/mycobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/mycobotsocket.py` & `pymycobot-3.1.6b1/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/mypalletizer.py` & `pymycobot-3.1.6b1/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/mypalletizersocket.py` & `pymycobot-3.1.6b1/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/ultraArm.py` & `pymycobot-3.1.6b1/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot/utils.py` & `pymycobot-3.1.6b1/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.5/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.1.6b1/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.5
+Version: 3.1.6b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `pymycobot-3.1.5/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.1.6b1/pymycobot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 pymycobot/Interface.py
 pymycobot/__init__.py
 pymycobot/bluet.py
+pymycobot/cobotx.py
 pymycobot/common.py
 pymycobot/elephantrobot.py
 pymycobot/error.py
 pymycobot/generate.py
 pymycobot/genre.py
 pymycobot/log.py
 pymycobot/mecharm.py
```

### Comparing `pymycobot-3.1.5/setup.py` & `pymycobot-3.1.6b1/setup.py`

 * *Files identical despite different names*

