# Comparing `tmp/adafri-0.0.11.tar.gz` & `tmp/adafri-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.11.tar", last modified: Tue Jul 11 22:02:38 2023, max compression
+gzip compressed data, was "adafri-0.0.12.tar", last modified: Tue Jul 11 22:42:58 2023, max compression
```

## Comparing `adafri-0.0.11.tar` & `adafri-0.0.12.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.406222 adafri-0.0.11/
--rw-r--r--   0 ibrahima   (502) staff       (20)      552 2023-07-11 22:02:38.405889 adafri-0.0.11/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.391914 adafri-0.0.11/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       50 2023-07-11 19:48:50.000000 adafri-0.0.11/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.397325 adafri-0.0.11/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       79 2023-07-11 21:48:50.000000 adafri-0.0.11/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1114 2023-07-11 21:45:31.000000 adafri-0.0.11/adafri/utils/firebase_collection.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.11/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    12814 2023-07-11 19:22:02.000000 adafri-0.0.11/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.398171 adafri-0.0.11/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       40 2023-07-11 21:48:14.000000 adafri-0.0.11/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.398941 adafri-0.0.11/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       42 2023-07-11 19:50:47.000000 adafri-0.0.11/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.401030 adafri-0.0.11/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:36:21.000000 adafri-0.0.11/adafri/v1/auth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5254 2023-07-11 19:45:53.000000 adafri-0.0.11/adafri/v1/auth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4321 2023-07-11 19:45:25.000000 adafri-0.0.11/adafri/v1/auth/models/client_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.402119 adafri-0.0.11/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)       21 2023-07-11 21:22:03.000000 adafri-0.0.11/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.404636 adafri-0.0.11/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-11 21:47:06.000000 adafri-0.0.11/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     8801 2023-07-11 21:51:21.000000 adafri-0.0.11/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4519 2023-07-11 19:25:49.000000 adafri-0.0.11/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:02:38.394114 adafri-0.0.11/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      552 2023-07-11 22:02:38.000000 adafri-0.0.11/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)      537 2023-07-11 22:02:38.000000 adafri-0.0.11/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-11 22:02:38.000000 adafri-0.0.11/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-11 22:02:38.000000 adafri-0.0.11/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-11 22:02:38.406365 adafri-0.0.11/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)     1000 2023-07-11 22:02:24.000000 adafri-0.0.11/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.510805 adafri-0.0.12/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      552 2023-07-11 22:42:58.510368 adafri-0.0.12/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.499457 adafri-0.0.12/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       50 2023-07-11 19:48:50.000000 adafri-0.0.12/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.504249 adafri-0.0.12/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       79 2023-07-11 21:48:50.000000 adafri-0.0.12/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1040 2023-07-11 22:40:50.000000 adafri-0.0.12/adafri/utils/firebase_collection.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.12/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    12814 2023-07-11 19:22:02.000000 adafri-0.0.12/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.504847 adafri-0.0.12/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       40 2023-07-11 21:48:14.000000 adafri-0.0.12/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.505443 adafri-0.0.12/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       42 2023-07-11 19:50:47.000000 adafri-0.0.12/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.507214 adafri-0.0.12/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-11 19:36:21.000000 adafri-0.0.12/adafri/v1/auth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5254 2023-07-11 19:45:53.000000 adafri-0.0.12/adafri/v1/auth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4321 2023-07-11 19:45:25.000000 adafri-0.0.12/adafri/v1/auth/models/client_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.507825 adafri-0.0.12/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       21 2023-07-11 21:22:03.000000 adafri-0.0.12/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.509562 adafri-0.0.12/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-11 21:47:06.000000 adafri-0.0.12/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     8801 2023-07-11 21:51:21.000000 adafri-0.0.12/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4519 2023-07-11 19:25:49.000000 adafri-0.0.12/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-11 22:42:58.501975 adafri-0.0.12/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      552 2023-07-11 22:42:58.000000 adafri-0.0.12/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)      537 2023-07-11 22:42:58.000000 adafri-0.0.12/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-11 22:42:58.000000 adafri-0.0.12/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-11 22:42:58.000000 adafri-0.0.12/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-11 22:42:58.511001 adafri-0.0.12/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1000 2023-07-11 22:42:53.000000 adafri-0.0.12/setup.py
```

### Comparing `adafri-0.0.11/PKG-INFO` & `adafri-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adafri
-Version: 0.0.11
+Version: 0.0.12
 Summary: Adafri python module
 Home-page: UNKNOWN
 Author: Ibrahima Touré
 Author-email: ibrahima.toure.dev@gmail.com
 License: UNKNOWN
 Description: Adafri python module
 Keywords: python,first package
```

### Comparing `adafri-0.0.11/adafri/utils/response.py` & `adafri-0.0.12/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.11/adafri/utils/utils.py` & `adafri-0.0.12/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.11/adafri/v1/auth/models/client.py` & `adafri-0.0.12/adafri/v1/auth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.11/adafri/v1/auth/models/client_fields.py` & `adafri-0.0.12/adafri/v1/auth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.11/adafri/v1/user/models/user.py` & `adafri-0.0.12/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.11/adafri/v1/user/models/user_fields.py` & `adafri-0.0.12/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.11/adafri.egg-info/PKG-INFO` & `adafri-0.0.12/adafri.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adafri
-Version: 0.0.11
+Version: 0.0.12
 Summary: Adafri python module
 Home-page: UNKNOWN
 Author: Ibrahima Touré
 Author-email: ibrahima.toure.dev@gmail.com
 License: UNKNOWN
 Description: Adafri python module
 Keywords: python,first package
```

### Comparing `adafri-0.0.11/adafri.egg-info/SOURCES.txt` & `adafri-0.0.12/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.11/setup.py` & `adafri-0.0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.11' 
+VERSION = '0.0.12' 
 DESCRIPTION = 'Adafri python module'
 LONG_DESCRIPTION = 'Adafri python module'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="adafri",
```

