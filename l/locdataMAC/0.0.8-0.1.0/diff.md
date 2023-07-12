# Comparing `tmp/locdataMAC-0.0.8.tar.gz` & `tmp/locdataMAC-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locdataMAC-0.0.8.tar", last modified: Mon Jul  3 16:30:23 2023, max compression
+gzip compressed data, was "locdataMAC-0.1.0.tar", last modified: Wed Jul 12 15:42:32 2023, max compression
```

## Comparing `locdataMAC-0.0.8.tar` & `locdataMAC-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:30:23.773907 locdataMAC-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-03 16:30:23.773907 locdataMAC-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-03 16:30:23.773907 locdataMAC-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:30:23.769907 locdataMAC-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:30:23.769907 locdataMAC-0.0.8/src/locdataMAC/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/cutom_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-03 16:30:12.000000 locdataMAC-0.0.8/src/locdataMAC/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:30:23.773907 locdataMAC-0.0.8/src/locdataMAC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 16:30:23.000000 locdataMAC-0.0.8/src/locdataMAC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:42:32.489375 locdataMAC-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-12 15:42:32.489375 locdataMAC-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-12 15:42:32.489375 locdataMAC-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:42:32.485376 locdataMAC-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:42:32.489375 locdataMAC-0.1.0/src/locdataMAC/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/src/locdataMAC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/src/locdataMAC/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/src/locdataMAC/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/src/locdataMAC/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/src/locdataMAC/cutom_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/src/locdataMAC/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-12 15:42:17.000000 locdataMAC-0.1.0/src/locdataMAC/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:42:32.489375 locdataMAC-0.1.0/src/locdataMAC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-12 15:42:32.000000 locdataMAC-0.1.0/src/locdataMAC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-12 15:42:32.000000 locdataMAC-0.1.0/src/locdataMAC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:42:32.000000 locdataMAC-0.1.0/src/locdataMAC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 15:42:32.000000 locdataMAC-0.1.0/src/locdataMAC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 15:42:32.000000 locdataMAC-0.1.0/src/locdataMAC.egg-info/top_level.txt
```

### Comparing `locdataMAC-0.0.8/LICENSE` & `locdataMAC-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.8/PKG-INFO` & `locdataMAC-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locdataMAC
-Version: 0.0.8
+Version: 0.1.0
 Summary: A small python package
 Home-page: https://github.com/SachinMishra-ux/locdataMAC
 Author: SachinMishra-ux
 Author-email: sachin19566@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/SachinMishra-ux/locdataMAC/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `locdataMAC-0.0.8/README.md` & `locdataMAC-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.8/setup.py` & `locdataMAC-0.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import setuptools
+import io
 
-with open("README.md", "r", encoding="utf-8") as f:
+with io.open('README.md', encoding="utf-8") as f:
     long_description = f.read()
 
-__version__ = "0.0.8"
+__version__ = "0.1.0"
 
 REPO_NAME = "locdataMAC"
 AUTHOR_USER_NAME = "SachinMishra-ux"
 SRC_REPO = "locdataMAC"
 AUTHOR_EMAIL = "sachin19566@gmail.com"
 
 setuptools.setup(
```

### Comparing `locdataMAC-0.0.8/src/locdataMAC/activity.py` & `locdataMAC-0.1.0/src/locdataMAC/activity.py`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.8/src/locdataMAC/analytics.py` & `locdataMAC-0.1.0/src/locdataMAC/analytics.py`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.8/src/locdataMAC/charts.py` & `locdataMAC-0.1.0/src/locdataMAC/charts.py`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.8/src/locdataMAC/timer.py` & `locdataMAC-0.1.0/src/locdataMAC/timer.py`

 * *Files identical despite different names*

### Comparing `locdataMAC-0.0.8/src/locdataMAC.egg-info/PKG-INFO` & `locdataMAC-0.1.0/src/locdataMAC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locdataMAC
-Version: 0.0.8
+Version: 0.1.0
 Summary: A small python package
 Home-page: https://github.com/SachinMishra-ux/locdataMAC
 Author: SachinMishra-ux
 Author-email: sachin19566@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/SachinMishra-ux/locdataMAC/issues
 Classifier: Programming Language :: Python :: 3.7
```

