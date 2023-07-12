# Comparing `tmp/vulcan-annotation-2.8.tar.gz` & `tmp/vulcan-annotation-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-annotation-2.8.tar", last modified: Tue Jul 11 14:07:35 2023, max compression
+gzip compressed data, was "vulcan-annotation-2.9.tar", last modified: Wed Jul 12 15:52:39 2023, max compression
```

## Comparing `vulcan-annotation-2.8.tar` & `vulcan-annotation-2.9.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 14:07:35.473443 vulcan-annotation-2.8/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-16 05:10:40.000000 vulcan-annotation-2.8/LICENSE
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      804 2023-07-11 14:07:35.473443 vulcan-annotation-2.8/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      328 2023-07-11 12:57:40.000000 vulcan-annotation-2.8/README.md
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-07-11 14:07:35.473443 vulcan-annotation-2.8/setup.cfg
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      841 2023-07-11 14:07:07.000000 vulcan-annotation-2.8/setup.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 14:07:35.473443 vulcan-annotation-2.8/vulcan_annotation/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       34 2023-07-11 13:20:33.000000 vulcan-annotation-2.8/vulcan_annotation/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)    10132 2023-07-11 14:06:46.000000 vulcan-annotation-2.8/vulcan_annotation/annotation.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 14:07:35.473443 vulcan-annotation-2.8/vulcan_annotation.egg-info/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      804 2023-07-11 14:07:35.000000 vulcan-annotation-2.8/vulcan_annotation.egg-info/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      292 2023-07-11 14:07:35.000000 vulcan-annotation-2.8/vulcan_annotation.egg-info/SOURCES.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-07-11 14:07:35.000000 vulcan-annotation-2.8/vulcan_annotation.egg-info/dependency_links.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       10 2023-07-11 14:07:35.000000 vulcan-annotation-2.8/vulcan_annotation.egg-info/requires.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       18 2023-07-11 14:07:35.000000 vulcan-annotation-2.8/vulcan_annotation.egg-info/top_level.txt
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-12 15:52:39.193508 vulcan-annotation-2.9/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-16 05:10:40.000000 vulcan-annotation-2.9/LICENSE
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      804 2023-07-12 15:52:39.193508 vulcan-annotation-2.9/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      328 2023-07-11 12:57:40.000000 vulcan-annotation-2.9/README.md
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-12 15:52:39.193508 vulcan-annotation-2.9/js/
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-12 15:52:39.193508 vulcan-annotation-2.9/js/src/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     7409 2023-04-29 16:40:26.000000 vulcan-annotation-2.9/js/src/va_dom.js
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)    13070 2023-07-11 14:05:04.000000 vulcan-annotation-2.9/js/src/vulcan_annotation.js
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-07-12 15:52:39.193508 vulcan-annotation-2.9/setup.cfg
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1108 2023-07-12 15:49:33.000000 vulcan-annotation-2.9/setup.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-12 15:52:39.193508 vulcan-annotation-2.9/vulcan_annotation/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      449 2023-07-12 15:47:06.000000 vulcan-annotation-2.9/vulcan_annotation/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)    10132 2023-07-11 14:06:46.000000 vulcan-annotation-2.9/vulcan_annotation/annotation.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-12 15:52:39.193508 vulcan-annotation-2.9/vulcan_annotation.egg-info/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      804 2023-07-12 15:52:39.000000 vulcan-annotation-2.9/vulcan_annotation.egg-info/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      341 2023-07-12 15:52:39.000000 vulcan-annotation-2.9/vulcan_annotation.egg-info/SOURCES.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-07-12 15:52:39.000000 vulcan-annotation-2.9/vulcan_annotation.egg-info/dependency_links.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       10 2023-07-12 15:52:39.000000 vulcan-annotation-2.9/vulcan_annotation.egg-info/requires.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       18 2023-07-12 15:52:39.000000 vulcan-annotation-2.9/vulcan_annotation.egg-info/top_level.txt
```

### Comparing `vulcan-annotation-2.8/LICENSE` & `vulcan-annotation-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-annotation-2.8/PKG-INFO` & `vulcan-annotation-2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-annotation
-Version: 2.8
+Version: 2.9
 Summary: Vulcan annotation for structured data.
 Home-page: https://github.com/vulcan-coalition/vulcan_annotation
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vulcan-annotation-2.8/vulcan_annotation/annotation.py` & `vulcan-annotation-2.9/vulcan_annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `vulcan-annotation-2.8/vulcan_annotation.egg-info/PKG-INFO` & `vulcan-annotation-2.9/vulcan_annotation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-annotation
-Version: 2.8
+Version: 2.9
 Summary: Vulcan annotation for structured data.
 Home-page: https://github.com/vulcan-coalition/vulcan_annotation
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

