# Comparing `tmp/logPPP-1.0.1.tar.gz` & `tmp/logPPP-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logPPP-1.0.1.tar", last modified: Tue Jul 11 17:17:04 2023, max compression
+gzip compressed data, was "logPPP-1.0.2.tar", last modified: Wed Jul 12 11:29:07 2023, max compression
```

## Comparing `logPPP-1.0.1.tar` & `logPPP-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:17:04.028008 logPPP-1.0.1/
--rw-rw-rw-   0        0        0      126 2023-07-11 17:17:04.028008 logPPP-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 17:17:04.019032 logPPP-1.0.1/logPPP/
--rw-rw-rw-   0        0        0      116 2023-07-11 14:54:45.000000 logPPP-1.0.1/logPPP/ConsoleColors.py
--rw-rw-rw-   0        0        0     1288 2023-07-11 15:00:15.000000 logPPP-1.0.1/logPPP/__init__.py
--rw-rw-rw-   0        0        0      371 2023-07-11 14:39:27.000000 logPPP-1.0.1/logPPP/logPLevel.py
--rw-rw-rw-   0        0        0      453 2023-07-11 14:15:21.000000 logPPP-1.0.1/logPPP/util.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:17:04.026013 logPPP-1.0.1/logPPP.egg-info/
--rw-rw-rw-   0        0        0      126 2023-07-11 17:17:03.000000 logPPP-1.0.1/logPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-07-11 17:17:03.000000 logPPP-1.0.1/logPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:17:03.000000 logPPP-1.0.1/logPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 17:17:03.000000 logPPP-1.0.1/logPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 17:17:04.029005 logPPP-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-07-11 17:17:01.000000 logPPP-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:29:07.139254 logPPP-1.0.2/
+-rw-rw-rw-   0        0        0      126 2023-07-12 11:29:07.139254 logPPP-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-07-12 11:13:39.000000 logPPP-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 11:29:07.132273 logPPP-1.0.2/logPPP.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-07-12 11:29:07.000000 logPPP-1.0.2/logPPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-12 11:29:07.000000 logPPP-1.0.2/logPPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:29:07.000000 logPPP-1.0.2/logPPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 11:29:07.000000 logPPP-1.0.2/logPPP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:29:07.140252 logPPP-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-07-12 11:22:50.000000 logPPP-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:29:07.125311 logPPP-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 11:29:07.137259 logPPP-1.0.2/src/logPPP/
+-rw-rw-rw-   0        0        0      116 2023-07-11 14:54:45.000000 logPPP-1.0.2/src/logPPP/_ConsoleColors.py
+-rw-rw-rw-   0        0        0     1404 2023-07-12 11:25:43.000000 logPPP-1.0.2/src/logPPP/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-07-11 14:15:21.000000 logPPP-1.0.2/src/logPPP/_util.py
+-rw-rw-rw-   0        0        0      371 2023-07-11 14:39:27.000000 logPPP-1.0.2/src/logPPP/logPPPLevel.py
```

### Comparing `logPPP-1.0.1/logPPP/__init__.py` & `logPPP-1.0.2/src/logPPP/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
 
-from .ConsoleColors import ConsoleColors
-from .logPLevel import logPLevel
-from .util import *
+from ._ConsoleColors import ConsoleColors
+from ._util import *
+from .logPPPLevel import logPLevel
 
+__all__ = ['__version__', 'logPLevel', 'info', 'warning', 'error', 'debug', 'critical']
+__version__ = '1.0.2'
 # 等级
 level = logPLevel.INFO
 
 
 # 日志输出
 def _base(args, sep=' ', end='\n', file=None, _level=logPLevel.INFO, color=ConsoleColors.RESET):
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
```

