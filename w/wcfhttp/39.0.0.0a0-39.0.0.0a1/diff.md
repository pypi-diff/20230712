# Comparing `tmp/wcfhttp-39.0.0.0a0.tar.gz` & `tmp/wcfhttp-39.0.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-39.0.0.0a0.tar", last modified: Wed Jul 12 04:11:01 2023, max compression
+gzip compressed data, was "wcfhttp-39.0.0.0a1.tar", last modified: Wed Jul 12 07:46:58 2023, max compression
```

## Comparing `wcfhttp-39.0.0.0a0.tar` & `wcfhttp-39.0.0.0a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 04:11:01.322278 wcfhttp-39.0.0.0a0/
--rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0     1830 2023-07-12 04:11:01.306656 wcfhttp-39.0.0.0a0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 04:11:01.322278 wcfhttp-39.0.0.0a0/setup.cfg
--rw-rw-rw-   0        0        0     1423 2023-07-12 03:00:09.000000 wcfhttp-39.0.0.0a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:11:01.306656 wcfhttp-39.0.0.0a0/wcfhttp/
--rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a0/wcfhttp/__init__.py
--rw-rw-rw-   0        0        0    14705 2023-07-12 04:06:57.000000 wcfhttp-39.0.0.0a0/wcfhttp/core.py
--rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a0/wcfhttp/main.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:11:01.306656 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/
--rw-rw-rw-   0        0        0     1830 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 07:46:58.297585 wcfhttp-39.0.0.0a1/
+-rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1830 2023-07-12 07:46:58.297585 wcfhttp-39.0.0.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 07:46:58.297585 wcfhttp-39.0.0.0a1/setup.cfg
+-rw-rw-rw-   0        0        0     1423 2023-07-12 07:46:37.000000 wcfhttp-39.0.0.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:46:58.281964 wcfhttp-39.0.0.0a1/wcfhttp/
+-rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a1/wcfhttp/__init__.py
+-rw-rw-rw-   0        0        0    14705 2023-07-12 07:46:44.000000 wcfhttp-39.0.0.0a1/wcfhttp/core.py
+-rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a1/wcfhttp/main.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:46:58.297585 wcfhttp-39.0.0.0a1/wcfhttp.egg-info/
+-rw-rw-rw-   0        0        0     1830 2023-07-12 07:46:58.000000 wcfhttp-39.0.0.0a1/wcfhttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-12 07:46:58.000000 wcfhttp-39.0.0.0a1/wcfhttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 07:46:58.000000 wcfhttp-39.0.0.0a1/wcfhttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-12 07:46:58.000000 wcfhttp-39.0.0.0a1/wcfhttp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-07-12 07:46:58.000000 wcfhttp-39.0.0.0a1/wcfhttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 07:46:58.000000 wcfhttp-39.0.0.0a1/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-39.0.0.0a0/PKG-INFO` & `wcfhttp-39.0.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 39.0.0.0a0
+Version: 39.0.0.0a1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

### Comparing `wcfhttp-39.0.0.0a0/setup.py` & `wcfhttp-39.0.0.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             'wcfhttp=wcfhttp.main:main'
         ]
     },
     install_requires=[
         "setuptools",
         "fastapi",
         "uvicorn[standard]",
-        "wcferry==39.0.0.0a2",
+        "wcferry==39.0.0.0a1",
     ],
     classifiers=[
         "Environment :: Win32 (MS Windows)",
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Topic :: Communications :: Chat",
         "Operating System :: Microsoft :: Windows",
```

### Comparing `wcfhttp-39.0.0.0a0/wcfhttp/core.py` & `wcfhttp-39.0.0.0a1/wcfhttp/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any
 
 import requests
 from fastapi import Body, FastAPI
 from pydantic import BaseModel
 from wcferry import Wcf, WxMsg
 
-__version__ = "39.0.0.0a0"
+__version__ = "39.0.0.0a1"
 
 
 class Msg(BaseModel):
     id: str
     type: int
     xml: str
     sender: str
```

### Comparing `wcfhttp-39.0.0.0a0/wcfhttp/main.py` & `wcfhttp-39.0.0.0a1/wcfhttp/main.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-39.0.0.0a0/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-39.0.0.0a1/wcfhttp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 39.0.0.0a0
+Version: 39.0.0.0a1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

