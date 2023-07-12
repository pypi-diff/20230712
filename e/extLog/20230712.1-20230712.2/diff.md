# Comparing `tmp/extLog-20230712.1.tar.gz` & `tmp/extLog-20230712.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extLog-20230712.1.tar", last modified: Wed Jul 12 12:02:34 2023, max compression
+gzip compressed data, was "extLog-20230712.2.tar", last modified: Wed Jul 12 12:34:50 2023, max compression
```

## Comparing `extLog-20230712.1.tar` & `extLog-20230712.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:02:34.245846 extLog-20230712.1/
--rw-rw-rw-   0        0        0      105 2023-07-12 12:02:34.244849 extLog-20230712.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 12:02:34.238868 extLog-20230712.1/extLog/
--rw-rw-rw-   0        0        0      893 2023-07-12 11:35:59.000000 extLog-20230712.1/extLog/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:02:34.243852 extLog-20230712.1/extLog.egg-info/
--rw-rw-rw-   0        0        0      105 2023-07-12 12:02:34.000000 extLog-20230712.1/extLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-07-12 12:02:34.000000 extLog-20230712.1/extLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:02:34.000000 extLog-20230712.1/extLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 12:02:34.000000 extLog-20230712.1/extLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 12:02:34.245846 extLog-20230712.1/setup.cfg
--rw-rw-rw-   0        0        0      220 2023-07-12 06:55:16.000000 extLog-20230712.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:34:50.500305 extLog-20230712.2/
+-rw-rw-rw-   0        0        0      105 2023-07-12 12:34:50.499309 extLog-20230712.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 12:34:50.494325 extLog-20230712.2/extLog/
+-rw-rw-rw-   0        0        0      991 2023-07-12 12:34:27.000000 extLog-20230712.2/extLog/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:34:50.499309 extLog-20230712.2/extLog.egg-info/
+-rw-rw-rw-   0        0        0      105 2023-07-12 12:34:50.000000 extLog-20230712.2/extLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-07-12 12:34:50.000000 extLog-20230712.2/extLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:34:50.000000 extLog-20230712.2/extLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 12:34:50.000000 extLog-20230712.2/extLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 12:34:50.500305 extLog-20230712.2/setup.cfg
+-rw-rw-rw-   0        0        0      220 2023-07-12 12:34:33.000000 extLog-20230712.2/setup.py
```

### Comparing `extLog-20230712.1/extLog/__init__.py` & `extLog-20230712.2/extLog/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: UTF-8 -*-
 # name = 'extLog'
 
-from logging import CRITICAL, DEBUG, ERROR, INFO, WARNING
+from logging import CRITICAL, DEBUG, ERROR, INFO, WARNING, Logger
 
 
-def genLogger(name=None, lvl=DEBUG):
+def genLogger(name: str = None, level: int = DEBUG, write_log: bool = False) -> Logger:
     import os
     from logging import getLogger, StreamHandler, FileHandler, Formatter
     from time import strftime
 
     logger = getLogger(name)
-
-    log_path = os.path.join(os.curdir, "Log", "")
-    os.makedirs(log_path, 777, True)
-    log_filename = log_path + f"{strftime('%m-%d')}.log"
+    logger.setLevel(level)
 
     # 输出日志到终端
     ch = StreamHandler()
     ch.setFormatter(Formatter("%(filename)12s:%(lineno)3d - %(levelname)5s: %(message)s"))
     logger.addHandler(ch)
 
     # 输出日志到文件
-    fh = FileHandler(log_filename, "a", encoding="UTF-8")
-    fh.setFormatter(Formatter("%(asctime)s %(filename)12s :%(lineno)3d - %(levelname)5s: %(message)s"))
-    logger.addHandler(fh)
+    if write_log:
+        log_path = os.path.join(os.curdir, "Log", "")
+        os.makedirs(log_path, 777, True)
+
+        log_file = log_path + f"{strftime('%m-%d')}.log"
+
+        fh = FileHandler(log_file, "a", encoding="UTF-8")
+        fh.setFormatter(Formatter("%(asctime)s %(filename)12s :%(lineno)3d - %(levelname)5s: %(message)s"))
+        logger.addHandler(fh)
 
-    logger.setLevel(lvl)
     return logger
```

