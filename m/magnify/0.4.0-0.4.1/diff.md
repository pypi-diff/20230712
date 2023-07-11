# Comparing `tmp/magnify-0.4.0.tar.gz` & `tmp/magnify-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.4.0.tar", max compression
+gzip compressed data, was "magnify-0.4.1.tar", max compression
```

## Comparing `magnify-0.4.0.tar` & `magnify-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.4.0/README.md
--rw-r--r--   0        0        0     1631 2023-07-07 23:46:24.157858 magnify-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      243 2023-07-07 23:46:31.718016 magnify-0.4.0/src/magnify/__init__.py
--rw-r--r--   0        0        0     3656 2023-07-07 23:13:15.436352 magnify-0.4.0/src/magnify/filter.py
--rw-r--r--   0        0        0    26165 2023-07-11 19:47:47.845868 magnify-0.4.0/src/magnify/find.py
--rw-r--r--   0        0        0     7516 2023-07-07 19:57:46.832323 magnify-0.4.0/src/magnify/identify.py
--rw-r--r--   0        0        0     1278 2023-07-07 22:23:16.867076 magnify-0.4.0/src/magnify/pipeline.py
--rw-r--r--   0        0        0      318 2023-07-07 19:04:45.491234 magnify-0.4.0/src/magnify/plot/__init__.py
--rw-r--r--   0        0        0     2345 2023-07-07 19:04:45.527235 magnify-0.4.0/src/magnify/plot/image.py
--rw-r--r--   0        0        0     1856 2023-07-07 19:04:45.511235 magnify-0.4.0/src/magnify/plot/ndplot.py
--rw-r--r--   0        0        0     2501 2023-07-07 19:04:45.551236 magnify-0.4.0/src/magnify/plot/relation.py
--rw-r--r--   0        0        0      694 2023-07-07 19:04:45.503235 magnify-0.4.0/src/magnify/plot/style.py
--rw-r--r--   0        0        0      445 2023-07-07 23:40:28.478446 magnify-0.4.0/src/magnify/postprocess.py
--rw-r--r--   0        0        0     1180 2023-07-07 19:09:00.448530 magnify-0.4.0/src/magnify/preprocess.py
--rw-r--r--   0        0        0    14930 2023-07-07 19:50:07.354563 magnify-0.4.0/src/magnify/reader.py
--rw-r--r--   0        0        0     2926 2023-07-07 23:43:18.929994 magnify-0.4.0/src/magnify/registry.py
--rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.4.0/src/magnify/stitch.py
--rw-r--r--   0        0        0     2639 2023-07-07 19:50:21.414864 magnify-0.4.0/src/magnify/utils.py
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 magnify-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.4.1/README.md
+-rw-r--r--   0        0        0     1631 2023-07-11 23:24:24.576990 magnify-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-07-11 23:24:31.489126 magnify-0.4.1/src/magnify/__init__.py
+-rw-r--r--   0        0        0     3692 2023-07-11 23:24:08.976685 magnify-0.4.1/src/magnify/filter.py
+-rw-r--r--   0        0        0    26165 2023-07-11 19:47:47.845868 magnify-0.4.1/src/magnify/find.py
+-rw-r--r--   0        0        0     7516 2023-07-07 19:57:46.832323 magnify-0.4.1/src/magnify/identify.py
+-rw-r--r--   0        0        0     1278 2023-07-07 22:23:16.867076 magnify-0.4.1/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      318 2023-07-07 19:04:45.491234 magnify-0.4.1/src/magnify/plot/__init__.py
+-rw-r--r--   0        0        0     2345 2023-07-07 19:04:45.527235 magnify-0.4.1/src/magnify/plot/image.py
+-rw-r--r--   0        0        0     1856 2023-07-07 19:04:45.511235 magnify-0.4.1/src/magnify/plot/ndplot.py
+-rw-r--r--   0        0        0     2501 2023-07-07 19:04:45.551236 magnify-0.4.1/src/magnify/plot/relation.py
+-rw-r--r--   0        0        0      694 2023-07-07 19:04:45.503235 magnify-0.4.1/src/magnify/plot/style.py
+-rw-r--r--   0        0        0      445 2023-07-07 23:40:28.478446 magnify-0.4.1/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1180 2023-07-07 19:09:00.448530 magnify-0.4.1/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    14930 2023-07-11 23:23:45.940234 magnify-0.4.1/src/magnify/reader.py
+-rw-r--r--   0        0        0     2926 2023-07-07 23:43:18.929994 magnify-0.4.1/src/magnify/registry.py
+-rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.4.1/src/magnify/stitch.py
+-rw-r--r--   0        0        0     2639 2023-07-07 19:50:21.414864 magnify-0.4.1/src/magnify/utils.py
+-rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 magnify-0.4.1/PKG-INFO
```

### Comparing `magnify-0.4.0/pyproject.toml` & `magnify-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.4.0"
+version = "0.4.1"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 opencv-python = [
```

### Comparing `magnify-0.4.0/src/magnify/filter.py` & `magnify-0.4.1/src/magnify/filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import cv2 as cv
 import numpy as np
 import xarray as xr
 
 from magnify import utils
 import magnify.registry as registry
```

### Comparing `magnify-0.4.0/src/magnify/find.py` & `magnify-0.4.1/src/magnify/find.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/identify.py` & `magnify-0.4.1/src/magnify/identify.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/pipeline.py` & `magnify-0.4.1/src/magnify/pipeline.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/plot/image.py` & `magnify-0.4.1/src/magnify/plot/image.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/plot/ndplot.py` & `magnify-0.4.1/src/magnify/plot/ndplot.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/plot/relation.py` & `magnify-0.4.1/src/magnify/plot/relation.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/plot/style.py` & `magnify-0.4.1/src/magnify/plot/style.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/preprocess.py` & `magnify-0.4.1/src/magnify/preprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/reader.py` & `magnify-0.4.1/src/magnify/reader.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/registry.py` & `magnify-0.4.1/src/magnify/registry.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/stitch.py` & `magnify-0.4.1/src/magnify/stitch.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/src/magnify/utils.py` & `magnify-0.4.1/src/magnify/utils.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.0/PKG-INFO` & `magnify-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnify
-Version: 0.4.0
+Version: 0.4.1
 Summary: A microscopy image processing toolkit.
 Author: Karl Krauth
 Author-email: karl.krauth@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

