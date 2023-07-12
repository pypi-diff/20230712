# Comparing `tmp/BahnarTextAugmentation-1.0.0.tar.gz` & `tmp/BahnarTextAugmentation-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BahnarTextAugmentation-1.0.0.tar", last modified: Wed Jul 12 07:45:42 2023, max compression
+gzip compressed data, was "BahnarTextAugmentation-1.0.1.tar", last modified: Wed Jul 12 07:45:21 2023, max compression
```

## Comparing `BahnarTextAugmentation-1.0.0.tar` & `BahnarTextAugmentation-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:42.274589 BahnarTextAugmentation-1.0.0/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      128 2023-07-12 07:45:42.274589 BahnarTextAugmentation-1.0.0/PKG-INFO
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-11 06:49:41.000000 BahnarTextAugmentation-1.0.0/README.md
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       38 2023-07-12 07:45:42.274589 BahnarTextAugmentation-1.0.0/setup.cfg
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      778 2023-07-12 07:45:36.000000 BahnarTextAugmentation-1.0.0/setup.py
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:42.274589 BahnarTextAugmentation-1.0.0/src/
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:42.274589 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     5743 2023-07-12 06:59:53.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/EDA.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1757 2023-07-12 07:27:29.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/MTLCombination.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      929 2023-07-12 07:00:13.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/SentenceBoundary.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     4853 2023-07-12 07:27:20.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/Single.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     2117 2023-07-12 07:00:05.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/Word2Vec.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       20 2023-07-12 07:28:38.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/__init__.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1597 2023-07-12 07:34:06.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/utils.py
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:42.274589 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation.egg-info/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      128 2023-07-12 07:45:42.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation.egg-info/PKG-INFO
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      544 2023-07-12 07:45:42.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation.egg-info/SOURCES.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        1 2023-07-12 07:45:42.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation.egg-info/dependency_links.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      101 2023-07-12 07:45:42.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation.egg-info/requires.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       23 2023-07-12 07:45:42.000000 BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation.egg-info/top_level.txt
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      128 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/PKG-INFO
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-11 06:49:41.000000 BahnarTextAugmentation-1.0.1/README.md
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       38 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/setup.cfg
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      778 2023-07-12 07:44:58.000000 BahnarTextAugmentation-1.0.1/setup.py
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:21.392246 BahnarTextAugmentation-1.0.1/src/
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     5743 2023-07-12 06:59:53.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/EDA.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1757 2023-07-12 07:27:29.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/MTLCombination.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      929 2023-07-12 07:00:13.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/SentenceBoundary.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     4853 2023-07-12 07:27:20.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/Single.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     2117 2023-07-12 07:00:05.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/Word2Vec.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       20 2023-07-12 07:28:38.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/__init__.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1597 2023-07-12 07:34:06.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/utils.py
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      128 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/PKG-INFO
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      544 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/SOURCES.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        1 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/dependency_links.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      101 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/requires.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       23 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/top_level.txt
```

### Comparing `BahnarTextAugmentation-1.0.0/setup.py` & `BahnarTextAugmentation-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 setup(
     name='BahnarTextAugmentation',
-    version='1.0.0',
+    version='1.0.1',
     license='Apache License 2.0',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='Bahnar Text Augmentation',
     long_description=read('README.md'),
     install_requires=['pyvi', 
                       'simalign',
```

### Comparing `BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/EDA.py` & `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/EDA.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/MTLCombination.py` & `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/MTLCombination.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/SentenceBoundary.py` & `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/SentenceBoundary.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/Single.py` & `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/Single.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/Word2Vec.py` & `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/Word2Vec.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation/utils.py` & `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/utils.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.0/src/BahnarTextAugmentation.egg-info/SOURCES.txt` & `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

