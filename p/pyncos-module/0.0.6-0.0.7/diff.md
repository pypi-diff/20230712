# Comparing `tmp/pyncos-module-0.0.6.tar.gz` & `tmp/pyncos-module-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncos-module-0.0.6.tar", last modified: Wed Jul 12 16:17:55 2023, max compression
+gzip compressed data, was "pyncos-module-0.0.7.tar", last modified: Wed Jul 12 16:21:15 2023, max compression
```

## Comparing `pyncos-module-0.0.6.tar` & `pyncos-module-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 16:17:55.583600 pyncos-module-0.0.6/
--rw-rw-rw-   0        0        0     1096 2023-07-12 14:51:52.000000 pyncos-module-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      423 2023-07-12 16:17:55.582599 pyncos-module-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-12 14:51:52.000000 pyncos-module-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 16:17:55.570530 pyncos-module-0.0.6/ncos/
--rw-rw-rw-   0        0        0       23 2023-07-12 16:12:11.000000 pyncos-module-0.0.6/ncos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:17:55.571531 pyncos-module-0.0.6/ncos/commons/
--rw-rw-rw-   0        0        0      728 2023-07-12 14:51:52.000000 pyncos-module-0.0.6/ncos/commons/__init__.py
--rw-rw-rw-   0        0        0     5862 2023-07-12 16:17:34.000000 pyncos-module-0.0.6/ncos/module.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:17:55.573531 pyncos-module-0.0.6/ncos/networks/
--rw-rw-rw-   0        0        0        0 2023-07-12 14:51:52.000000 pyncos-module-0.0.6/ncos/networks/__init__.py
--rw-rw-rw-   0        0        0     1647 2023-07-12 16:11:50.000000 pyncos-module-0.0.6/ncos/networks/mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:17:55.575533 pyncos-module-0.0.6/ncos/utils/
--rw-rw-rw-   0        0        0      406 2023-07-12 16:11:58.000000 pyncos-module-0.0.6/ncos/utils/__init__.py
--rw-rw-rw-   0        0        0     1437 2023-07-12 14:51:52.000000 pyncos-module-0.0.6/ncos/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:17:55.581601 pyncos-module-0.0.6/pyncos_module.egg-info/
--rw-rw-rw-   0        0        0      423 2023-07-12 16:17:55.000000 pyncos-module-0.0.6/pyncos_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-07-12 16:17:55.000000 pyncos-module-0.0.6/pyncos_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 16:17:55.000000 pyncos-module-0.0.6/pyncos_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 16:17:55.000000 pyncos-module-0.0.6/pyncos_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 16:17:55.583600 pyncos-module-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-07-12 16:17:25.000000 pyncos-module-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:21:15.107322 pyncos-module-0.0.7/
+-rw-rw-rw-   0        0        0     1096 2023-07-12 14:51:52.000000 pyncos-module-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      423 2023-07-12 16:21:15.107322 pyncos-module-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-12 14:51:52.000000 pyncos-module-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 16:21:15.094788 pyncos-module-0.0.7/ncos/
+-rw-rw-rw-   0        0        0       23 2023-07-12 16:12:11.000000 pyncos-module-0.0.7/ncos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:21:15.096819 pyncos-module-0.0.7/ncos/commons/
+-rw-rw-rw-   0        0        0      698 2023-07-12 16:20:56.000000 pyncos-module-0.0.7/ncos/commons/__init__.py
+-rw-rw-rw-   0        0        0     5862 2023-07-12 16:17:34.000000 pyncos-module-0.0.7/ncos/module.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:21:15.098824 pyncos-module-0.0.7/ncos/networks/
+-rw-rw-rw-   0        0        0        0 2023-07-12 14:51:52.000000 pyncos-module-0.0.7/ncos/networks/__init__.py
+-rw-rw-rw-   0        0        0     1647 2023-07-12 16:11:50.000000 pyncos-module-0.0.7/ncos/networks/mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:21:15.101350 pyncos-module-0.0.7/ncos/utils/
+-rw-rw-rw-   0        0        0      406 2023-07-12 16:11:58.000000 pyncos-module-0.0.7/ncos/utils/__init__.py
+-rw-rw-rw-   0        0        0     1437 2023-07-12 14:51:52.000000 pyncos-module-0.0.7/ncos/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:21:15.105324 pyncos-module-0.0.7/pyncos_module.egg-info/
+-rw-rw-rw-   0        0        0      423 2023-07-12 16:21:15.000000 pyncos-module-0.0.7/pyncos_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-12 16:21:15.000000 pyncos-module-0.0.7/pyncos_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:21:15.000000 pyncos-module-0.0.7/pyncos_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 16:21:15.000000 pyncos-module-0.0.7/pyncos_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:21:15.107322 pyncos-module-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-07-12 16:21:09.000000 pyncos-module-0.0.7/setup.py
```

### Comparing `pyncos-module-0.0.6/LICENSE.txt` & `pyncos-module-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.6/ncos/commons/__init__.py` & `pyncos-module-0.0.7/ncos/commons/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 #
 LOGS_ENABLE                           = False
 LOGS_PATH                             = os.path.join('.','logs')
 
 #DATA DUMPS
 DATA_ROOT_PATH                        = os.path.join('.', 'data')
-DATA_LOCAL_FILE                       = os.path.join(DATA_ROOT_PATH, 'local')
+DATA_LOCAL_FILE                       = 'local'
```

### Comparing `pyncos-module-0.0.6/ncos/module.py` & `pyncos-module-0.0.7/ncos/module.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.6/ncos/networks/mqtt.py` & `pyncos-module-0.0.7/ncos/networks/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.6/ncos/utils/logger.py` & `pyncos-module-0.0.7/ncos/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.6/setup.py` & `pyncos-module-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="pyncos-module", 
-    version="0.0.6",   
+    version="0.0.7",   
     author="xuwh",  
     author_email="xuwhdev@gmail.com", 
     description="", 
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://gitee.com/zwsjz/carbot-module-lib", 
     packages=setuptools.find_packages(),
```

