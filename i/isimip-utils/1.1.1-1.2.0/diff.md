# Comparing `tmp/isimip_utils-1.1.1.tar.gz` & `tmp/isimip_utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isimip_utils-1.1.1.tar", last modified: Thu Jun  8 12:47:20 2023, max compression
+gzip compressed data, was "isimip_utils-1.2.0.tar", last modified: Wed Jul 12 11:42:19 2023, max compression
```

## Comparing `isimip_utils-1.1.1.tar` & `isimip_utils-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 jochen    (1000) jochen    (1000)        0 2023-06-08 12:47:20.877456 isimip_utils-1.1.1/
--rw-r--r--   0 jochen    (1000) jochen    (1000)     1102 2022-11-08 17:31:25.000000 isimip_utils-1.1.1/LICENSE
--rw-r--r--   0 jochen    (1000) jochen    (1000)     2553 2023-06-08 12:47:20.877456 isimip_utils-1.1.1/PKG-INFO
--rw-r--r--   0 jochen    (1000) jochen    (1000)     1800 2022-11-22 17:49:16.000000 isimip_utils-1.1.1/README.md
-drwxr-xr-x   0 jochen    (1000) jochen    (1000)        0 2023-06-08 12:47:20.877456 isimip_utils-1.1.1/isimip_utils/
--rw-r--r--   0 jochen    (1000) jochen    (1000)       32 2023-06-08 12:20:06.000000 isimip_utils-1.1.1/isimip_utils/__init__.py
--rw-r--r--   0 jochen    (1000) jochen    (1000)      486 2021-03-24 16:17:39.000000 isimip_utils-1.1.1/isimip_utils/checksum.py
--rw-r--r--   0 jochen    (1000) jochen    (1000)     2811 2023-06-08 12:19:33.000000 isimip_utils-1.1.1/isimip_utils/config.py
--rw-r--r--   0 jochen    (1000) jochen    (1000)      616 2022-11-16 16:57:11.000000 isimip_utils-1.1.1/isimip_utils/decorators.py
--rw-r--r--   0 jochen    (1000) jochen    (1000)       42 2022-11-08 16:34:22.000000 isimip_utils-1.1.1/isimip_utils/exceptions.py
--rw-r--r--   0 jochen    (1000) jochen    (1000)     4385 2023-02-09 17:18:18.000000 isimip_utils-1.1.1/isimip_utils/fetch.py
--rw-r--r--   0 jochen    (1000) jochen    (1000)     2118 2023-02-07 14:07:15.000000 isimip_utils-1.1.1/isimip_utils/netcdf.py
--rw-r--r--   0 jochen    (1000) jochen    (1000)     2565 2023-03-30 08:20:10.000000 isimip_utils-1.1.1/isimip_utils/patterns.py
--rw-r--r--   0 jochen    (1000) jochen    (1000)      669 2022-11-08 17:14:36.000000 isimip_utils-1.1.1/isimip_utils/utils.py
-drwxr-xr-x   0 jochen    (1000) jochen    (1000)        0 2023-06-08 12:47:20.877456 isimip_utils-1.1.1/isimip_utils.egg-info/
--rw-r--r--   0 jochen    (1000) jochen    (1000)     2553 2023-06-08 12:47:20.000000 isimip_utils-1.1.1/isimip_utils.egg-info/PKG-INFO
--rw-r--r--   0 jochen    (1000) jochen    (1000)      434 2023-06-08 12:47:20.000000 isimip_utils-1.1.1/isimip_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jochen    (1000) jochen    (1000)        1 2023-06-08 12:47:20.000000 isimip_utils-1.1.1/isimip_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jochen    (1000) jochen    (1000)       40 2023-06-08 12:47:20.000000 isimip_utils-1.1.1/isimip_utils.egg-info/requires.txt
--rw-r--r--   0 jochen    (1000) jochen    (1000)       13 2023-06-08 12:47:20.000000 isimip_utils-1.1.1/isimip_utils.egg-info/top_level.txt
--rw-r--r--   0 jochen    (1000) jochen    (1000)      896 2023-06-08 12:47:20.877456 isimip_utils-1.1.1/setup.cfg
--rw-r--r--   0 jochen    (1000) jochen    (1000)       38 2022-11-21 11:22:05.000000 isimip_utils-1.1.1/setup.py
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-07-12 11:42:19.484522 isimip_utils-1.2.0/
+-rw-r--r--   0 jochen    (1000) staff       (20)     1102 2022-12-14 15:31:47.000000 isimip_utils-1.2.0/LICENSE
+-rw-r--r--   0 jochen    (1000) staff       (20)     2553 2023-07-12 11:42:19.484596 isimip_utils-1.2.0/PKG-INFO
+-rw-r--r--   0 jochen    (1000) staff       (20)     1800 2022-12-14 15:31:47.000000 isimip_utils-1.2.0/README.md
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-07-12 11:42:19.483779 isimip_utils-1.2.0/isimip_utils/
+-rw-r--r--   0 jochen    (1000) staff       (20)       32 2023-07-12 11:42:10.000000 isimip_utils-1.2.0/isimip_utils/__init__.py
+-rw-r--r--   0 jochen    (1000) staff       (20)      486 2022-12-14 15:31:47.000000 isimip_utils-1.2.0/isimip_utils/checksum.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     1423 2023-06-30 07:44:28.000000 isimip_utils-1.2.0/isimip_utils/config.py
+-rw-r--r--   0 jochen    (1000) staff       (20)      616 2022-12-14 15:31:47.000000 isimip_utils-1.2.0/isimip_utils/decorators.py
+-rw-r--r--   0 jochen    (1000) staff       (20)       42 2022-12-14 15:31:47.000000 isimip_utils-1.2.0/isimip_utils/exceptions.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     4385 2023-02-27 16:09:14.000000 isimip_utils-1.2.0/isimip_utils/fetch.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     2118 2023-02-27 16:09:14.000000 isimip_utils-1.2.0/isimip_utils/netcdf.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     2041 2023-07-11 20:07:06.000000 isimip_utils-1.2.0/isimip_utils/parser.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     2565 2022-12-14 18:31:55.000000 isimip_utils-1.2.0/isimip_utils/patterns.py
+-rw-r--r--   0 jochen    (1000) staff       (20)      669 2022-12-14 15:31:47.000000 isimip_utils-1.2.0/isimip_utils/utils.py
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-07-12 11:42:19.484412 isimip_utils-1.2.0/isimip_utils.egg-info/
+-rw-r--r--   0 jochen    (1000) staff       (20)     2553 2023-07-12 11:42:19.000000 isimip_utils-1.2.0/isimip_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jochen    (1000) staff       (20)      457 2023-07-12 11:42:19.000000 isimip_utils-1.2.0/isimip_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)        1 2023-07-12 11:42:19.000000 isimip_utils-1.2.0/isimip_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)       40 2023-07-12 11:42:19.000000 isimip_utils-1.2.0/isimip_utils.egg-info/requires.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)       13 2023-07-12 11:42:19.000000 isimip_utils-1.2.0/isimip_utils.egg-info/top_level.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)      896 2023-07-12 11:42:19.484939 isimip_utils-1.2.0/setup.cfg
+-rw-r--r--   0 jochen    (1000) staff       (20)       38 2022-12-14 15:31:47.000000 isimip_utils-1.2.0/setup.py
```

### Comparing `isimip_utils-1.1.1/LICENSE` & `isimip_utils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isimip_utils-1.1.1/PKG-INFO` & `isimip_utils-1.2.0/isimip_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: isimip_utils
-Version: 1.1.1
+Name: isimip-utils
+Version: 1.2.0
 Summary: This package contains common functionality for different ISIMIP tools.
 Home-page: https://github.com/ISI-MIP/isimip-utils
 Author: Jochen Klar
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `isimip_utils-1.1.1/README.md` & `isimip_utils-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `isimip_utils-1.1.1/isimip_utils/decorators.py` & `isimip_utils-1.2.0/isimip_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `isimip_utils-1.1.1/isimip_utils/fetch.py` & `isimip_utils-1.2.0/isimip_utils/fetch.py`

 * *Files identical despite different names*

### Comparing `isimip_utils-1.1.1/isimip_utils/netcdf.py` & `isimip_utils-1.2.0/isimip_utils/netcdf.py`

 * *Files identical despite different names*

### Comparing `isimip_utils-1.1.1/isimip_utils/patterns.py` & `isimip_utils-1.2.0/isimip_utils/patterns.py`

 * *Files identical despite different names*

### Comparing `isimip_utils-1.1.1/isimip_utils/utils.py` & `isimip_utils-1.2.0/isimip_utils/utils.py`

 * *Files identical despite different names*

### Comparing `isimip_utils-1.1.1/isimip_utils.egg-info/PKG-INFO` & `isimip_utils-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: isimip-utils
-Version: 1.1.1
+Name: isimip_utils
+Version: 1.2.0
 Summary: This package contains common functionality for different ISIMIP tools.
 Home-page: https://github.com/ISI-MIP/isimip-utils
 Author: Jochen Klar
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `isimip_utils-1.1.1/setup.cfg` & `isimip_utils-1.2.0/setup.cfg`

 * *Files identical despite different names*

