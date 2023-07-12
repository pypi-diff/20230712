# Comparing `tmp/Final2x-core-1.0.1.tar.gz` & `tmp/Final2x-core-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Final2x-core-1.0.1.tar", last modified: Sat Jul  8 03:06:40 2023, max compression
+gzip compressed data, was "Final2x-core-1.0.2.tar", last modified: Wed Jul 12 20:10:52 2023, max compression
```

## Comparing `Final2x-core-1.0.1.tar` & `Final2x-core-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.813253 Final2x-core-1.0.1/Final2x_core/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-08 03:06:16.000000 Final2x-core-1.0.1/Final2x_core/Final2x-core-pip.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.813253 Final2x-core-1.0.1/Final2x_core/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/Final2x_core/src/SRFactory/
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/REALCUGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/REALESRGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRBaseClass.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRFactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRMD.py
--rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/WAIFU2X.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRFactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/Final2x_core/src/SRncnn/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRncnn/REALCUGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRncnn/REALESRGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRncnn/SRMDncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/SRqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/Final2x_core/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/utils/getConfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/utils/progressLog.py
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-08 03:06:39.000000 Final2x-core-1.0.1/Final2x_core/src/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 03:06:40.813253 Final2x-core-1.0.1/Final2x_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7240 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-08 03:06:40.000000 Final2x-core-1.0.1/Final2x_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-08 03:06:16.000000 Final2x-core-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-08 03:06:16.000000 Final2x-core-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7240 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6534 2023-07-08 03:06:16.000000 Final2x-core-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-08 03:06:40.817253 Final2x-core-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-08 03:06:17.000000 Final2x-core-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-12 20:10:28.000000 Final2x-core-1.0.2/Final2x_core/Final2x-core-pip.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/src/SRFactory/
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/REALCUGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/REALESRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRBaseClass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRFactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRMD.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/WAIFU2X.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/src/SRncnn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRncnn/REALCUGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRncnn/REALESRGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRncnn/SRMDncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/utils/getConfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/utils/progressLog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7240 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-12 20:10:28.000000 Final2x-core-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-12 20:10:28.000000 Final2x-core-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7240 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6534 2023-07-12 20:10:28.000000 Final2x-core-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-12 20:10:29.000000 Final2x-core-1.0.2/setup.py
```

### Comparing `Final2x-core-1.0.1/Final2x_core/__main__.py` & `Final2x-core-1.0.2/Final2x_core/__main__.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/config.yaml` & `Final2x-core-1.0.2/Final2x_core/config.yaml`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRFactory/REALCUGAN.py` & `Final2x-core-1.0.2/Final2x_core/src/SRFactory/REALCUGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRFactory/REALESRGAN.py` & `Final2x-core-1.0.2/Final2x_core/src/SRFactory/REALESRGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRBaseClass.py` & `Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRBaseClass.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRFactory.py` & `Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRFactory.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRFactory/SRMD.py` & `Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRMD.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRFactory/WAIFU2X.py` & `Final2x-core-1.0.2/Final2x_core/src/SRFactory/WAIFU2X.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRFactory/__init__.py` & `Final2x-core-1.0.2/Final2x_core/src/SRFactory/__init__.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRncnn/REALCUGANncnn.py` & `Final2x-core-1.0.2/Final2x_core/src/SRncnn/REALCUGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRncnn/REALESRGANncnn.py` & `Final2x-core-1.0.2/Final2x_core/src/SRncnn/REALESRGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRncnn/SRMDncnn.py` & `Final2x-core-1.0.2/Final2x_core/src/SRncnn/SRMDncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/SRncnn/WAIFU2Xncnn.py` & `Final2x-core-1.0.2/Final2x_core/src/SRncnn/WAIFU2Xncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/utils/getConfig.py` & `Final2x-core-1.0.2/Final2x_core/src/utils/getConfig.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core/src/utils/progressLog.py` & `Final2x-core-1.0.2/Final2x_core/src/utils/progressLog.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/Final2x_core.egg-info/PKG-INFO` & `Final2x-core-1.0.2/Final2x_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Final2x-core
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/Tohrusky/Final2x-core
 Author: Tohrusky
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Final2x-core-1.0.1/Final2x_core.egg-info/SOURCES.txt` & `Final2x-core-1.0.2/Final2x_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/LICENSE` & `Final2x-core-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/PKG-INFO` & `Final2x-core-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Final2x-core
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/Tohrusky/Final2x-core
 Author: Tohrusky
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Final2x-core-1.0.1/README.md` & `Final2x-core-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.1/setup.py` & `Final2x-core-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-_version: str = "1.0.1"
+_version: str = "1.0.2"
 
 
 def My_find_packages(*tops):
     packages = []
     for d in tops:
         for root, dirs, files in os.walk(d, followlinks=True):
             packages.append(root)
```

