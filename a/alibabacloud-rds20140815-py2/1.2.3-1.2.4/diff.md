# Comparing `tmp/alibabacloud_rds20140815_py2-1.2.3.tar.gz` & `tmp/alibabacloud_rds20140815_py2-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.2.3.tar", last modified: Tue Jul 11 15:08:44 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.2.4.tar", last modified: Wed Jul 12 15:10:08 2023, max compression
```

## Comparing `alibabacloud_rds20140815_py2-1.2.3.tar` & `alibabacloud_rds20140815_py2-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/
--rw-r--r--   0 root         (0) root         (0)     1830 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)   754958 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2570429 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2023-07-11 15:08:44.000000 alibabacloud_rds20140815_py2-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-07-12 15:10:07.000000 alibabacloud_rds20140815_py2-1.2.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-12 15:10:07.000000 alibabacloud_rds20140815_py2-1.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-12 15:10:07.000000 alibabacloud_rds20140815_py2-1.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-12 15:10:07.000000 alibabacloud_rds20140815_py2-1.2.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-12 15:10:07.000000 alibabacloud_rds20140815_py2-1.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 15:10:07.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   754958 2023-07-12 15:10:07.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2570429 2023-07-12 15:10:07.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 15:10:08.000000 alibabacloud_rds20140815_py2-1.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-07-12 15:10:07.000000 alibabacloud_rds20140815_py2-1.2.4/setup.py
```

### Comparing `alibabacloud_rds20140815_py2-1.2.3/ChangeLog.md` & `alibabacloud_rds20140815_py2-1.2.4/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-11 Version: 1.2.3
+- Fixed 500 for interface.
+
 2023-07-10 Version: 1.2.2
 - Fixed 500 for interface.
 
 2023-07-10 Version: 1.2.1
 - Add DescribeClassDetails Api.
 
 2023-07-09 Version: 1.2.0
```

### Comparing `alibabacloud_rds20140815_py2-1.2.3/LICENSE` & `alibabacloud_rds20140815_py2-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.2.3/PKG-INFO` & `alibabacloud_rds20140815_py2-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds20140815_py2
-Version: 1.2.3
+Version: 1.2.4
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.2.3/README-CN.md` & `alibabacloud_rds20140815_py2-1.2.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.2.3/README.md` & `alibabacloud_rds20140815_py2-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.2.3/alibabacloud_rds20140815_py2.egg-info/PKG-INFO` & `alibabacloud_rds20140815_py2-1.2.4/alibabacloud_rds20140815_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds20140815-py2
-Version: 1.2.3
+Version: 1.2.4
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.2.3/setup.py` & `alibabacloud_rds20140815_py2-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds20140815_py2.
 
-Created on 11/07/2023
+Created on 12/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds20140815"
 NAME = "alibabacloud_rds20140815_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds (20140815) SDK Library for Python2"
```

