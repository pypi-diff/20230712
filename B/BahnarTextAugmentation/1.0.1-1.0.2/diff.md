# Comparing `tmp/BahnarTextAugmentation-1.0.1.tar.gz` & `tmp/BahnarTextAugmentation-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BahnarTextAugmentation-1.0.1.tar", last modified: Wed Jul 12 07:45:21 2023, max compression
+gzip compressed data, was "BahnarTextAugmentation-1.0.2.tar", last modified: Wed Jul 12 08:04:17 2023, max compression
```

## Comparing `BahnarTextAugmentation-1.0.1.tar` & `BahnarTextAugmentation-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      128 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/PKG-INFO
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-11 06:49:41.000000 BahnarTextAugmentation-1.0.1/README.md
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       38 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/setup.cfg
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      778 2023-07-12 07:44:58.000000 BahnarTextAugmentation-1.0.1/setup.py
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:21.392246 BahnarTextAugmentation-1.0.1/src/
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     5743 2023-07-12 06:59:53.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/EDA.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1757 2023-07-12 07:27:29.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/MTLCombination.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      929 2023-07-12 07:00:13.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/SentenceBoundary.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     4853 2023-07-12 07:27:20.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/Single.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     2117 2023-07-12 07:00:05.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/Word2Vec.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       20 2023-07-12 07:28:38.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/__init__.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1597 2023-07-12 07:34:06.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/utils.py
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:45:21.396247 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      128 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/PKG-INFO
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      544 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/SOURCES.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        1 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/dependency_links.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      101 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/requires.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       23 2023-07-12 07:45:21.000000 BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/top_level.txt
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 08:04:17.832200 BahnarTextAugmentation-1.0.2/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      128 2023-07-12 08:04:17.832200 BahnarTextAugmentation-1.0.2/PKG-INFO
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-11 06:49:41.000000 BahnarTextAugmentation-1.0.2/README.md
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       38 2023-07-12 08:04:17.832200 BahnarTextAugmentation-1.0.2/setup.cfg
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      778 2023-07-12 08:04:12.000000 BahnarTextAugmentation-1.0.2/setup.py
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 08:04:17.832200 BahnarTextAugmentation-1.0.2/src/
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 08:04:17.832200 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     5743 2023-07-12 06:59:53.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/EDA.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1779 2023-07-12 07:56:32.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/MTLCombination.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      929 2023-07-12 07:00:13.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/SentenceBoundary.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     4885 2023-07-12 07:56:17.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/Single.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     2117 2023-07-12 07:00:05.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/Word2Vec.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       45 2023-07-12 08:02:09.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/__init__.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       41 2023-07-12 08:03:59.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/_version.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1598 2023-07-12 07:57:40.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/utils.py
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 08:04:17.832200 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation.egg-info/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      128 2023-07-12 08:04:17.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation.egg-info/PKG-INFO
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      583 2023-07-12 08:04:17.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation.egg-info/SOURCES.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        1 2023-07-12 08:04:17.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation.egg-info/dependency_links.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      101 2023-07-12 08:04:17.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation.egg-info/requires.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       23 2023-07-12 08:04:17.000000 BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation.egg-info/top_level.txt
```

### Comparing `BahnarTextAugmentation-1.0.1/setup.py` & `BahnarTextAugmentation-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 setup(
     name='BahnarTextAugmentation',
-    version='1.0.1',
+    version='1.0.2',
     license='Apache License 2.0',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='Bahnar Text Augmentation',
     long_description=read('README.md'),
     install_requires=['pyvi', 
                       'simalign',
```

### Comparing `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/EDA.py` & `BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/EDA.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/MTLCombination.py` & `BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/MTLCombination.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 import numpy as np
 import math
 import re
 
 
 def da_combine(proportion, keep_old=False):
-  def wrap(sentences, loaded_alignments, ba_vi_dict):
+  def da_combine_wrap(sentences, loaded_alignments, ba_vi_dict):
     if len(loaded_alignments) < len(sentences):
         loaded_alignments.clear()
         loaded_alignments.extend(build_aligner(sentences=sentences))
     da_pairs = []
     for i in range(len(sentences)):
       ttokens = custom_tokenize(sentences[i][1])
       stokens = custom_tokenize(sentences[i][0])
@@ -43,9 +43,9 @@
       s_out_str = ' '.join(stokens)
       da_pairs.append([s_out_str, t_out_str])
     if keep_old:
       loaded_alignments.extend(loaded_alignments)
       da_pairs.extend(sentences)
     return da_pairs
   
-  return wrap
+  return da_combine_wrap
```

### Comparing `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/SentenceBoundary.py` & `BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/SentenceBoundary.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/Single.py` & `BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/Single.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 import numpy as np
 import math
 import re
 
 
 def da_replaceWord(proportion, keep_old=False):
-    def wrap(sentences, loaded_alignments, ba_vi_dict):
+    def replace_wrap(sentences, loaded_alignments, ba_vi_dict):
         da_pairs = []
         if len(loaded_alignments) < len(sentences):
             loaded_alignments.clear()
             loaded_alignments.extend(build_aligner(sentences=sentences))
         for i in range(len(sentences)):
             ttokens = custom_tokenize(sentences[i][1])
             stokens = custom_tokenize(sentences[i][0])
@@ -34,18 +34,18 @@
             t_out_str = ' '.join(ttokens)
             s_out_str = ' '.join(stokens)
             da_pairs.append([s_out_str, t_out_str])
         if keep_old:
             loaded_alignments.extend(loaded_alignments)
             da_pairs.extend(sentences)
         return da_pairs
-    return wrap
+    return replace_wrap
 
 def da_replaceToken(proportion, keep_old=False):
-    def wrap(sentences, loaded_alignments, ba_vi_dict): 
+    def replace_wrap(sentences, loaded_alignments, ba_vi_dict): 
         if len(loaded_alignments) < len(sentences):
             loaded_alignments.clear()
             loaded_alignments.extend(build_aligner(sentences=sentences))
         da_pairs = []
         for i in range(len(sentences)):
             ttokens = custom_tokenize(sentences[i][1])
             stokens = custom_tokenize(sentences[i][0])
@@ -73,15 +73,15 @@
             t_out_str = ' '.join(ttokens)
             s_out_str = ' '.join(stokens)
             da_pairs.append([s_out_str, t_out_str])
         if keep_old:
             loaded_alignments.extend(loaded_alignments)
             da_pairs.extend(sentences)
         return da_pairs
-    return wrap
+    return replace_wrap
 
 def da_swap(proportion, keep_old=False):
     def wrap(sentences, *args):
         #NOTE loaded alignments and ba_vi_dict are not used
         da_pairs = []
         for i in range(len(sentences)):
             moved_pos=set()
```

### Comparing `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/Word2Vec.py` & `BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/Word2Vec.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation/utils.py` & `BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,14 @@
   def wrap(sentences, ba_vi_dict, loaded_alignments=None):
     # if not loaded_alignments:
     # if not ba_vi_dict:
     # loaded_alignments = []
     if loaded_alignments is None:
       print("Starting build aligner...")
       checkReplaceFunction = reduce(lambda base, x: base or ('replace' in x.__name__ or 'da_combine' in x.__name__), augMethods, False)
+
       if checkReplaceFunction:
         loaded_alignments = build_aligner(sentences)
     return reduce(lambda x, y: y(x, loaded_alignments, ba_vi_dict), augMethods, sentences)
   return wrap
```

### Comparing `BahnarTextAugmentation-1.0.1/src/BahnarTextAugmentation.egg-info/SOURCES.txt` & `BahnarTextAugmentation-1.0.2/src/BahnarTextAugmentation.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,13 +2,14 @@
 setup.py
 src/BahnarTextAugmentation/EDA.py
 src/BahnarTextAugmentation/MTLCombination.py
 src/BahnarTextAugmentation/SentenceBoundary.py
 src/BahnarTextAugmentation/Single.py
 src/BahnarTextAugmentation/Word2Vec.py
 src/BahnarTextAugmentation/__init__.py
+src/BahnarTextAugmentation/_version.py
 src/BahnarTextAugmentation/utils.py
 src/BahnarTextAugmentation.egg-info/PKG-INFO
 src/BahnarTextAugmentation.egg-info/SOURCES.txt
 src/BahnarTextAugmentation.egg-info/dependency_links.txt
 src/BahnarTextAugmentation.egg-info/requires.txt
 src/BahnarTextAugmentation.egg-info/top_level.txt
```

