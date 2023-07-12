# Comparing `tmp/LongNet-0.3.2.tar.gz` & `tmp/LongNet-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.3.2.tar", last modified: Wed Jul 12 19:34:16 2023, max compression
+gzip compressed data, was "LongNet-0.3.4.tar", last modified: Wed Jul 12 20:32:48 2023, max compression
```

## Comparing `LongNet-0.3.2.tar` & `LongNet-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:34:16.872242 LongNet-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 19:34:07.000000 LongNet-0.3.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:34:16.872242 LongNet-0.3.2/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-12 19:34:07.000000 LongNet-0.3.2/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 19:34:07.000000 LongNet-0.3.2/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-12 19:34:07.000000 LongNet-0.3.2/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 19:34:07.000000 LongNet-0.3.2/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 19:34:07.000000 LongNet-0.3.2/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-12 19:34:07.000000 LongNet-0.3.2/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:34:16.872242 LongNet-0.3.2/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 19:34:16.000000 LongNet-0.3.2/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-12 19:34:16.000000 LongNet-0.3.2/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:34:16.000000 LongNet-0.3.2/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 19:34:16.000000 LongNet-0.3.2/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 19:34:16.000000 LongNet-0.3.2/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 19:34:16.872242 LongNet-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-12 19:34:07.000000 LongNet-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 19:34:16.872242 LongNet-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 19:34:07.000000 LongNet-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:34:16.872242 LongNet-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 19:34:07.000000 LongNet-0.3.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:32:48.056164 LongNet-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 20:32:38.000000 LongNet-0.3.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:32:48.056164 LongNet-0.3.4/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 20:32:38.000000 LongNet-0.3.4/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 20:32:38.000000 LongNet-0.3.4/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-12 20:32:38.000000 LongNet-0.3.4/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 20:32:38.000000 LongNet-0.3.4/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 20:32:38.000000 LongNet-0.3.4/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-12 20:32:38.000000 LongNet-0.3.4/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:32:48.056164 LongNet-0.3.4/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 20:32:48.000000 LongNet-0.3.4/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-12 20:32:48.000000 LongNet-0.3.4/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:32:48.000000 LongNet-0.3.4/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 20:32:48.000000 LongNet-0.3.4/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 20:32:48.000000 LongNet-0.3.4/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 20:32:48.056164 LongNet-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-12 20:32:38.000000 LongNet-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:32:48.056164 LongNet-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 20:32:38.000000 LongNet-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:32:48.056164 LongNet-0.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 20:32:38.000000 LongNet-0.3.4/test/test.py
```

### Comparing `LongNet-0.3.2/LICENSE` & `LongNet-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.2/LongNet/attend.py` & `LongNet-0.3.4/LongNet/attend.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.2/LongNet/attention.py` & `LongNet-0.3.4/LongNet/attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.2/LongNet/model.py` & `LongNet-0.3.4/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.2/LongNet/training.py` & `LongNet-0.3.4/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.2/LongNet/utils.py` & `LongNet-0.3.4/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.2/LongNet.egg-info/PKG-INFO` & `LongNet-0.3.4/LongNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.2
+Version: 0.3.4
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.2/PKG-INFO` & `LongNet-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.2
+Version: 0.3.4
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.2/README.md` & `LongNet-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.2/setup.py` & `LongNet-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.3.2',
+  version = '0.3.4',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.3.2/test/test.py` & `LongNet-0.3.4/test/test.py`

 * *Files identical despite different names*

