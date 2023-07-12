# Comparing `tmp/ns_asphalt9-0.1.2.tar.gz` & `tmp/ns_asphalt9-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ns_asphalt9-0.1.2.tar", last modified: Mon Jul 10 16:06:38 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.1.3.tar", last modified: Wed Jul 12 06:20:30 2023, max compression
```

## Comparing `ns_asphalt9-0.1.2.tar` & `ns_asphalt9-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/
--rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.1.2/LICENSE
--rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/MANIFEST.in
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.1.2/README.md
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/
--rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/
--rw-r--r--   0 sunhao     (501) staff       (20)      258 2023-07-09 10:58:05.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)      589 2023-07-09 10:57:49.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 sunhao     (501) staff       (20)     4652 2023-07-10 14:21:56.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3917 2023-07-02 12:56:49.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 sunhao     (501) staff       (20)     4241 2023-07-10 15:55:00.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/cache.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2828 2023-07-10 15:07:50.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/consts.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/controller.py
--rw-r--r--   0 sunhao     (501) staff       (20)      638 2023-07-10 14:11:06.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)    23653 2023-07-10 14:18:29.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/
--rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/ocr.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1843 2023-07-10 14:15:27.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 sunhao     (501) staff       (20)    13412 2023-07-10 15:27:10.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/pages.py
--rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2686 2023-07-10 14:02:34.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/fetch_cars.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 sunhao     (501) staff       (20)     5517 2023-07-10 14:14:54.000000 ns_asphalt9-0.1.2/ns_asphalt9/main.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/setup.cfg
--rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:30.688006 ns_asphalt9-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-12 06:20:30.688006 ns_asphalt9-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:30.684007 ns_asphalt9-0.1.3/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:30.688006 ns_asphalt9-0.1.3/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:30.688006 ns_asphalt9-0.1.3/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:30.688006 ns_asphalt9-0.1.3/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:30.688006 ns_asphalt9-0.1.3/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:30.688006 ns_asphalt9-0.1.3/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/utils/fetch_tracks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:30.684007 ns_asphalt9-0.1.3/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-12 06:20:30.000000 ns_asphalt9-0.1.3/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-12 06:20:30.000000 ns_asphalt9-0.1.3/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 06:20:30.000000 ns_asphalt9-0.1.3/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 06:20:30.000000 ns_asphalt9-0.1.3/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 06:20:30.000000 ns_asphalt9-0.1.3/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 06:20:30.000000 ns_asphalt9-0.1.3/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 06:20:30.000000 ns_asphalt9-0.1.3/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-12 06:20:30.692007 ns_asphalt9-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:20:30.688006 ns_asphalt9-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-12 06:20:21.000000 ns_asphalt9-0.1.3/tests/test_ocr.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ns_asphalt9-0.1.2/LICENSE` & `ns_asphalt9-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/PKG-INFO` & `ns_asphalt9-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
-Description: # ns_asphalt9 
-        
-        基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
-        
-        
-        ### 硬件依赖
-            
-        1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
-           
-           用于switch画面输入到虚拟机
-        
-        2. **蓝牙(必选)**
-           
-           用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
-        
-        3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
-           
-           同时输出switch到显示器和采集卡，方便debug
-        
-        
-        ### 使用教程
-        
-        [Wiki](https://github.com/codehai/ns_asphalt9/wiki)
-        
-        
-        ### 免责声明
-        
-        ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
-        
-        
-        ### 许可证
-        
-        ![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
-        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >= 3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ns_asphalt9 
+
+基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
+
+
+### 硬件依赖
+    
+1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
+   
+   用于switch画面输入到虚拟机
+
+2. **蓝牙(必选)**
+   
+   用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
+
+3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
+   
+   同时输出switch到显示器和采集卡，方便debug
+
+
+### 使用教程
+
+[Wiki](https://github.com/codehai/ns_asphalt9/wiki)
+
+
+### 免责声明
+
+ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
+
+
+### 许可证
+
+![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
```

### Comparing `ns_asphalt9-0.1.2/README.md` & `ns_asphalt9-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/actions/common.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/globals.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,12 +34,13 @@
 DIVISION = ""
 
 # 选车次数
 SELECT_COUNT = {
     consts.mp1_zh: 0,
     consts.mp2_zh: 0,
     consts.mp3_zh: 0,
-    consts.car_hunt_zh: 0
+    consts.car_hunt_zh: 0,
+    consts.legendary_hunt_zh: 0
 }
 
 # 比赛中
 RACING = 0
```

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/gui/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
             try:
                 if self.settings_data and "传奇寻车" in self.settings_data:
                     option1.set(self.settings_data["传奇寻车"]["车库位置"][r]["row"])
                     option2.set(self.settings_data["传奇寻车"]["车库位置"][r]["col"])
             except IndexError:
                 pass
 
-            self.setting_modules["寻车"]["车库位置"].append({"row": option1, "col": option2})
+            self.setting_modules["传奇寻车"]["车库位置"].append({"row": option1, "col": option2})
 
         # 多人三配置
         mp3_settings_frame = customtkinter.CTkFrame(self.settings, width=340)
         mp3_settings_frame.grid(
             row=6, column=1, columnspan=2, padx=(20, 0), pady=(20, 0), sticky="nsew"
         )
```

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.1.3/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.1.3/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.1.3/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.1.3/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/pages.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.1.3/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9/main.py` & `ns_asphalt9-0.1.3/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.1.3/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
-Description: # ns_asphalt9 
-        
-        基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
-        
-        
-        ### 硬件依赖
-            
-        1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
-           
-           用于switch画面输入到虚拟机
-        
-        2. **蓝牙(必选)**
-           
-           用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
-        
-        3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
-           
-           同时输出switch到显示器和采集卡，方便debug
-        
-        
-        ### 使用教程
-        
-        [Wiki](https://github.com/codehai/ns_asphalt9/wiki)
-        
-        
-        ### 免责声明
-        
-        ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
-        
-        
-        ### 许可证
-        
-        ![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
-        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >= 3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ns_asphalt9 
+
+基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
+
+
+### 硬件依赖
+    
+1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
+   
+   用于switch画面输入到虚拟机
+
+2. **蓝牙(必选)**
+   
+   用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
+
+3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
+   
+   同时输出switch到显示器和采集卡，方便debug
+
+
+### 使用教程
+
+[Wiki](https://github.com/codehai/ns_asphalt9/wiki)
+
+
+### 免责声明
+
+ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
+
+
+### 许可证
+
+![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
```

### Comparing `ns_asphalt9-0.1.2/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.1.3/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,9 +31,11 @@
 ns_asphalt9/core/gui/images/help.png
 ns_asphalt9/core/gui/images/home.png
 ns_asphalt9/core/gui/images/logo.png
 ns_asphalt9/core/gui/images/settings.png
 ns_asphalt9/core/utils/__init__.py
 ns_asphalt9/core/utils/decorator.py
 ns_asphalt9/core/utils/fetch_cars.py
+ns_asphalt9/core/utils/fetch_tracks.py
 ns_asphalt9/core/utils/log.py
-ns_asphalt9/core/utils/timer.py
+ns_asphalt9/core/utils/timer.py
+tests/test_ocr.py
```

### Comparing `ns_asphalt9-0.1.2/setup.cfg` & `ns_asphalt9-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.1.2
+version = 0.1.3
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

