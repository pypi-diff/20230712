# Comparing `tmp/pyncos-module-0.0.4.tar.gz` & `tmp/pyncos-module-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncos-module-0.0.4.tar", last modified: Wed Jul 12 15:58:42 2023, max compression
+gzip compressed data, was "pyncos-module-0.0.5.tar", last modified: Wed Jul 12 16:12:41 2023, max compression
```

## Comparing `pyncos-module-0.0.4.tar` & `pyncos-module-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:58:42.323829 pyncos-module-0.0.4/
--rw-rw-rw-   0        0        0     1096 2023-07-12 14:51:52.000000 pyncos-module-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      423 2023-07-12 15:58:42.322811 pyncos-module-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-12 14:51:52.000000 pyncos-module-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 15:58:42.311700 pyncos-module-0.0.4/ncos/
--rw-rw-rw-   0        0        0       23 2023-07-12 14:51:52.000000 pyncos-module-0.0.4/ncos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:58:42.312699 pyncos-module-0.0.4/ncos/commons/
--rw-rw-rw-   0        0        0      728 2023-07-12 14:51:52.000000 pyncos-module-0.0.4/ncos/commons/__init__.py
--rw-rw-rw-   0        0        0     5856 2023-07-12 15:58:31.000000 pyncos-module-0.0.4/ncos/module.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:58:42.314700 pyncos-module-0.0.4/ncos/networks/
--rw-rw-rw-   0        0        0        0 2023-07-12 14:51:52.000000 pyncos-module-0.0.4/ncos/networks/__init__.py
--rw-rw-rw-   0        0        0     1642 2023-07-12 14:51:52.000000 pyncos-module-0.0.4/ncos/networks/mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:58:42.316702 pyncos-module-0.0.4/ncos/utils/
--rw-rw-rw-   0        0        0      396 2023-07-12 14:51:52.000000 pyncos-module-0.0.4/ncos/utils/__init__.py
--rw-rw-rw-   0        0        0     1437 2023-07-12 14:51:52.000000 pyncos-module-0.0.4/ncos/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:58:42.321810 pyncos-module-0.0.4/pyncos_module.egg-info/
--rw-rw-rw-   0        0        0      423 2023-07-12 15:58:42.000000 pyncos-module-0.0.4/pyncos_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-07-12 15:58:42.000000 pyncos-module-0.0.4/pyncos_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:58:42.000000 pyncos-module-0.0.4/pyncos_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 15:58:42.000000 pyncos-module-0.0.4/pyncos_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:58:42.324811 pyncos-module-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-07-12 15:58:18.000000 pyncos-module-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:12:41.241567 pyncos-module-0.0.5/
+-rw-rw-rw-   0        0        0     1096 2023-07-12 14:51:52.000000 pyncos-module-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      423 2023-07-12 16:12:41.240570 pyncos-module-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-12 14:51:52.000000 pyncos-module-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 16:12:41.228433 pyncos-module-0.0.5/ncos/
+-rw-rw-rw-   0        0        0       23 2023-07-12 16:12:11.000000 pyncos-module-0.0.5/ncos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:12:41.229536 pyncos-module-0.0.5/ncos/commons/
+-rw-rw-rw-   0        0        0      728 2023-07-12 14:51:52.000000 pyncos-module-0.0.5/ncos/commons/__init__.py
+-rw-rw-rw-   0        0        0     5871 2023-07-12 16:11:38.000000 pyncos-module-0.0.5/ncos/module.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:12:41.231534 pyncos-module-0.0.5/ncos/networks/
+-rw-rw-rw-   0        0        0        0 2023-07-12 14:51:52.000000 pyncos-module-0.0.5/ncos/networks/__init__.py
+-rw-rw-rw-   0        0        0     1647 2023-07-12 16:11:50.000000 pyncos-module-0.0.5/ncos/networks/mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:12:41.234534 pyncos-module-0.0.5/ncos/utils/
+-rw-rw-rw-   0        0        0      406 2023-07-12 16:11:58.000000 pyncos-module-0.0.5/ncos/utils/__init__.py
+-rw-rw-rw-   0        0        0     1437 2023-07-12 14:51:52.000000 pyncos-module-0.0.5/ncos/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:12:41.239569 pyncos-module-0.0.5/pyncos_module.egg-info/
+-rw-rw-rw-   0        0        0      423 2023-07-12 16:12:41.000000 pyncos-module-0.0.5/pyncos_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-12 16:12:41.000000 pyncos-module-0.0.5/pyncos_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:12:41.000000 pyncos-module-0.0.5/pyncos_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 16:12:41.000000 pyncos-module-0.0.5/pyncos_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:12:41.241567 pyncos-module-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-07-12 16:12:37.000000 pyncos-module-0.0.5/setup.py
```

### Comparing `pyncos-module-0.0.4/LICENSE.txt` & `pyncos-module-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.4/ncos/commons/__init__.py` & `pyncos-module-0.0.5/ncos/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.4/ncos/module.py` & `pyncos-module-0.0.5/ncos/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #-*- coding:utf-8 -*- 
 
 from abc import abstractmethod
 import os
 from uuid import uuid4
-from networks.mqtt import MqttClient
+from ncos.networks.mqtt import MqttClient
 from json import dumps, loads
-from utils import LOG_DEBUG, LOG_ERROR
-from commons import *
+from ncos.utils import LOG_DEBUG, LOG_ERROR
+from ncos.commons import *
 
 class ModuleBase:
   
 
   __slot_name__ = ''
   '''
     The name of slot which to register
```

### Comparing `pyncos-module-0.0.4/ncos/networks/mqtt.py` & `pyncos-module-0.0.5/ncos/networks/mqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf-8 -*-
 
 from paho.mqtt import client as mqtt_client
 from uuid import uuid4
 
-from utils import LOG_DEBUG
+from ncos.utils import LOG_DEBUG
 
 
 class MqttClient:
   
   
   def __on_messaged__(self, client, userdata, msg):
     if self.on_messaged:
```

### Comparing `pyncos-module-0.0.4/ncos/utils/logger.py` & `pyncos-module-0.0.5/ncos/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyncos-module-0.0.4/setup.py` & `pyncos-module-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="pyncos-module", 
-    version="0.0.4",   
+    version="0.0.5",   
     author="xuwh",  
     author_email="xuwhdev@gmail.com", 
     description="", 
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://gitee.com/zwsjz/carbot-module-lib", 
     packages=setuptools.find_packages(),
```

