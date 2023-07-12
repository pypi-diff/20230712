# Comparing `tmp/pyncos-module-0.0.1.tar.gz` & `tmp/pyncos-module-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncos-module-0.0.1.tar", last modified: Wed Jul 12 15:31:02 2023, max compression
+gzip compressed data, was "pyncos-module-0.0.2.tar", last modified: Wed Jul 12 15:46:40 2023, max compression
```

## Comparing `pyncos-module-0.0.1.tar` & `pyncos-module-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:31:02.837637 pyncos-module-0.0.1/
--rw-rw-rw-   0        0        0     1096 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      423 2023-07-12 15:31:02.837637 pyncos-module-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 15:31:02.825499 pyncos-module-0.0.1/module/
--rw-rw-rw-   0        0        0       23 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:31:02.826498 pyncos-module-0.0.1/module/commons/
--rw-rw-rw-   0        0        0      728 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/module/commons/__init__.py
--rw-rw-rw-   0        0        0     5776 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/module/module.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:31:02.829601 pyncos-module-0.0.1/module/networks/
--rw-rw-rw-   0        0        0        0 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/module/networks/__init__.py
--rw-rw-rw-   0        0        0     1642 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/module/networks/mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:31:02.831566 pyncos-module-0.0.1/module/utils/
--rw-rw-rw-   0        0        0      396 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/module/utils/__init__.py
--rw-rw-rw-   0        0        0     1437 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/module/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:31:02.836568 pyncos-module-0.0.1/pyncos_module.egg-info/
--rw-rw-rw-   0        0        0      423 2023-07-12 15:31:02.000000 pyncos-module-0.0.1/pyncos_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-07-12 15:31:02.000000 pyncos-module-0.0.1/pyncos_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:31:02.000000 pyncos-module-0.0.1/pyncos_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 15:31:02.000000 pyncos-module-0.0.1/pyncos_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:31:02.837637 pyncos-module-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-07-12 14:51:52.000000 pyncos-module-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:46:40.326191 pyncos-module-0.0.2/
+-rw-rw-rw-   0        0        0     1096 2023-07-12 14:51:52.000000 pyncos-module-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      423 2023-07-12 15:46:40.325192 pyncos-module-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-12 14:51:52.000000 pyncos-module-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 15:46:40.314127 pyncos-module-0.0.2/module/
+-rw-rw-rw-   0        0        0       23 2023-07-12 14:51:52.000000 pyncos-module-0.0.2/module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:46:40.315126 pyncos-module-0.0.2/module/commons/
+-rw-rw-rw-   0        0        0      728 2023-07-12 14:51:52.000000 pyncos-module-0.0.2/module/commons/__init__.py
+-rw-rw-rw-   0        0        0     5776 2023-07-12 14:51:52.000000 pyncos-module-0.0.2/module/module.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:46:40.317125 pyncos-module-0.0.2/module/networks/
+-rw-rw-rw-   0        0        0        0 2023-07-12 14:51:52.000000 pyncos-module-0.0.2/module/networks/__init__.py
+-rw-rw-rw-   0        0        0     1642 2023-07-12 14:51:52.000000 pyncos-module-0.0.2/module/networks/mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:46:40.319191 pyncos-module-0.0.2/module/utils/
+-rw-rw-rw-   0        0        0      396 2023-07-12 14:51:52.000000 pyncos-module-0.0.2/module/utils/__init__.py
+-rw-rw-rw-   0        0        0     1437 2023-07-12 14:51:52.000000 pyncos-module-0.0.2/module/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:46:40.324192 pyncos-module-0.0.2/pyncos_module.egg-info/
+-rw-rw-rw-   0        0        0      423 2023-07-12 15:46:40.000000 pyncos-module-0.0.2/pyncos_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-07-12 15:46:40.000000 pyncos-module-0.0.2/pyncos_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:46:40.000000 pyncos-module-0.0.2/pyncos_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 15:46:40.000000 pyncos-module-0.0.2/pyncos_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:46:40.326191 pyncos-module-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-07-12 15:46:35.000000 pyncos-module-0.0.2/setup.py
```

### Comparing `pyncos-module-0.0.1/LICENSE.txt` & `pyncos-module-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.1/module/commons/__init__.py` & `pyncos-module-0.0.2/module/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.1/module/module.py` & `pyncos-module-0.0.2/module/module.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.1/module/networks/mqtt.py` & `pyncos-module-0.0.2/module/networks/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.1/module/utils/logger.py` & `pyncos-module-0.0.2/module/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.1/setup.py` & `pyncos-module-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="pyncos-module", 
-    version="0.0.1",   
+    version="0.0.2",   
     author="xuwh",  
     author_email="xuwhdev@gmail.com", 
     description="", 
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://gitee.com/zwsjz/carbot-module-lib", 
     packages=setuptools.find_packages(),
```

