# Comparing `tmp/LongNet-0.3.5.tar.gz` & `tmp/LongNet-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.3.5.tar", last modified: Wed Jul 12 20:56:41 2023, max compression
+gzip compressed data, was "LongNet-0.3.6.tar", last modified: Wed Jul 12 21:06:08 2023, max compression
```

## Comparing `LongNet-0.3.5.tar` & `LongNet-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:56:41.846907 LongNet-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 20:56:30.000000 LongNet-0.3.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:56:41.846907 LongNet-0.3.5/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 20:56:30.000000 LongNet-0.3.5/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 20:56:30.000000 LongNet-0.3.5/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-12 20:56:30.000000 LongNet-0.3.5/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 20:56:30.000000 LongNet-0.3.5/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 20:56:30.000000 LongNet-0.3.5/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-12 20:56:30.000000 LongNet-0.3.5/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:56:41.846907 LongNet-0.3.5/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 20:56:41.000000 LongNet-0.3.5/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-12 20:56:41.000000 LongNet-0.3.5/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:56:41.000000 LongNet-0.3.5/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 20:56:41.000000 LongNet-0.3.5/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 20:56:41.000000 LongNet-0.3.5/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 20:56:41.846907 LongNet-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-12 20:56:30.000000 LongNet-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:56:41.846907 LongNet-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 20:56:30.000000 LongNet-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:56:41.846907 LongNet-0.3.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 20:56:30.000000 LongNet-0.3.5/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.932199 LongNet-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 21:05:54.000000 LongNet-0.3.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.928199 LongNet-0.3.6/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.932199 LongNet-0.3.6/LongNet/iterations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/BlocksparseDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/DilatedAttentionOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/DilatedAttentionOld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/DistributedDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/DynamicDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/MultiModal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.932199 LongNet-0.3.6/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 21:06:08.932199 LongNet-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-12 21:05:54.000000 LongNet-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:06:08.932199 LongNet-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 21:05:54.000000 LongNet-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.932199 LongNet-0.3.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 21:05:54.000000 LongNet-0.3.6/test/test.py
```

### Comparing `LongNet-0.3.5/LICENSE` & `LongNet-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.5/LongNet/attend.py` & `LongNet-0.3.6/LongNet/attend.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.5/LongNet/attention.py` & `LongNet-0.3.6/LongNet/attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.5/LongNet/model.py` & `LongNet-0.3.6/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.5/LongNet/training.py` & `LongNet-0.3.6/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.5/LongNet/utils.py` & `LongNet-0.3.6/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.5/LongNet.egg-info/PKG-INFO` & `LongNet-0.3.6/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.5
+Version: 0.3.6
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.5/PKG-INFO` & `LongNet-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.5
+Version: 0.3.6
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.5/README.md` & `LongNet-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.5/setup.py` & `LongNet-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.3.5',
+  version = '0.3.6',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.3.5/test/test.py` & `LongNet-0.3.6/test/test.py`

 * *Files identical despite different names*

