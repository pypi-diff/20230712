# Comparing `tmp/logPPP-1.0.2.tar.gz` & `tmp/logPPP-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logPPP-1.0.2.tar", last modified: Wed Jul 12 11:29:07 2023, max compression
+gzip compressed data, was "logPPP-1.0.3.tar", last modified: Wed Jul 12 11:34:35 2023, max compression
```

## Comparing `logPPP-1.0.2.tar` & `logPPP-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:29:07.139254 logPPP-1.0.2/
--rw-rw-rw-   0        0        0      126 2023-07-12 11:29:07.139254 logPPP-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-07-12 11:13:39.000000 logPPP-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 11:29:07.132273 logPPP-1.0.2/logPPP.egg-info/
--rw-rw-rw-   0        0        0      126 2023-07-12 11:29:07.000000 logPPP-1.0.2/logPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-12 11:29:07.000000 logPPP-1.0.2/logPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:29:07.000000 logPPP-1.0.2/logPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 11:29:07.000000 logPPP-1.0.2/logPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 11:29:07.140252 logPPP-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-07-12 11:22:50.000000 logPPP-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:29:07.125311 logPPP-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 11:29:07.137259 logPPP-1.0.2/src/logPPP/
--rw-rw-rw-   0        0        0      116 2023-07-11 14:54:45.000000 logPPP-1.0.2/src/logPPP/_ConsoleColors.py
--rw-rw-rw-   0        0        0     1404 2023-07-12 11:25:43.000000 logPPP-1.0.2/src/logPPP/__init__.py
--rw-rw-rw-   0        0        0      453 2023-07-11 14:15:21.000000 logPPP-1.0.2/src/logPPP/_util.py
--rw-rw-rw-   0        0        0      371 2023-07-11 14:39:27.000000 logPPP-1.0.2/src/logPPP/logPPPLevel.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.065303 logPPP-1.0.3/
+-rw-rw-rw-   0        0        0      126 2023-07-12 11:34:35.064333 logPPP-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-07-12 11:13:39.000000 logPPP-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.058323 logPPP-1.0.3/logPPP.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-07-12 11:34:34.000000 logPPP-1.0.3/logPPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-12 11:34:35.000000 logPPP-1.0.3/logPPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:34:34.000000 logPPP-1.0.3/logPPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 11:34:34.000000 logPPP-1.0.3/logPPP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:34:35.065303 logPPP-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-07-12 11:22:50.000000 logPPP-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.051378 logPPP-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.063337 logPPP-1.0.3/src/logPPP/
+-rw-rw-rw-   0        0        0      116 2023-07-11 14:54:45.000000 logPPP-1.0.3/src/logPPP/_ConsoleColors.py
+-rw-rw-rw-   0        0        0     1422 2023-07-12 11:34:34.000000 logPPP-1.0.3/src/logPPP/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-07-11 14:15:21.000000 logPPP-1.0.3/src/logPPP/_util.py
+-rw-rw-rw-   0        0        0      373 2023-07-12 11:34:15.000000 logPPP-1.0.3/src/logPPP/logPPPLevel.py
```

### Comparing `logPPP-1.0.2/src/logPPP/__init__.py` & `logPPP-1.0.3/src/logPPP/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import datetime
 
 from ._ConsoleColors import ConsoleColors
 from ._util import *
-from .logPPPLevel import logPLevel
+from .logPPPLevel import logPPPLevel
 
-__all__ = ['__version__', 'logPLevel', 'info', 'warning', 'error', 'debug', 'critical']
-__version__ = '1.0.2'
+__all__ = ['__version__', 'logPPPLevel', 'info', 'warning', 'error', 'debug', 'critical']
+__version__ = '1.0.3'
 # 等级
-level = logPLevel.INFO
+level = logPPPLevel.INFO
 
 
 # 日志输出
-def _base(args, sep=' ', end='\n', file=None, _level=logPLevel.INFO, color=ConsoleColors.RESET):
+def _base(args, sep=' ', end='\n', file=None, _level=logPPPLevel.INFO, color=ConsoleColors.RESET):
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     args = "{:<20} {:<8} {}  {}".format(timestamp, get_caller_file_basename_path(), _level['name'], args)
     args = f"{color}{args}{ConsoleColors.RESET}"
     if _level['level'] >= level['level']:
         print(args, sep=sep, end=end, file=file)
 
 
 # info等级
 def info(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPLevel.INFO, ConsoleColors.RESET)
+    _base(args, sep, end, file, logPPPLevel.INFO, ConsoleColors.RESET)
 
 
 # warning等级
 def warning(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPLevel.WARNING, ConsoleColors.YELLOW)
+    _base(args, sep, end, file, logPPPLevel.WARNING, ConsoleColors.YELLOW)
 
 
 # error等级
 def error(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPLevel.ERROR, ConsoleColors.RED)
+    _base(args, sep, end, file, logPPPLevel.ERROR, ConsoleColors.RED)
 
 
 # debug等级
 def debug(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPLevel.DEBUG, ConsoleColors.RED)
+    _base(args, sep, end, file, logPPPLevel.DEBUG, ConsoleColors.RED)
 
 
 # critical等级
 def critical(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPLevel.CRITICAL, ConsoleColors.RED)
+    _base(args, sep, end, file, logPPPLevel.CRITICAL, ConsoleColors.RED)
```

