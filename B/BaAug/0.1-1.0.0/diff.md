# Comparing `tmp/BaAug-0.1.tar.gz` & `tmp/BaAug-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BaAug-0.1.tar", last modified: Wed Jul 12 07:00:35 2023, max compression
+gzip compressed data, was "BaAug-1.0.0.tar", last modified: Wed Jul 12 07:28:51 2023, max compression
```

## Comparing `BaAug-0.1.tar` & `BaAug-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:00:35.490130 BaAug-0.1/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      104 2023-07-12 07:00:35.490130 BaAug-0.1/PKG-INFO
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-11 06:49:41.000000 BaAug-0.1/README.md
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       38 2023-07-12 07:00:35.490130 BaAug-0.1/setup.cfg
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      739 2023-07-12 04:15:58.000000 BaAug-0.1/setup.py
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:00:35.490130 BaAug-0.1/src/
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:00:35.490130 BaAug-0.1/src/BaAug/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     5743 2023-07-12 06:59:53.000000 BaAug-0.1/src/BaAug/EDA.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1717 2023-07-12 07:00:18.000000 BaAug-0.1/src/BaAug/MTLCombination.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      929 2023-07-12 07:00:13.000000 BaAug-0.1/src/BaAug/SentenceBoundary.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     4766 2023-07-12 06:59:59.000000 BaAug-0.1/src/BaAug/Single.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     2117 2023-07-12 07:00:05.000000 BaAug-0.1/src/BaAug/Word2Vec.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 06:59:47.000000 BaAug-0.1/src/BaAug/__init__.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1550 2023-07-12 04:56:59.000000 BaAug-0.1/src/BaAug/utils.py
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:00:35.490130 BaAug-0.1/src/BaAug.egg-info/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      104 2023-07-12 07:00:35.000000 BaAug-0.1/src/BaAug.egg-info/PKG-INFO
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      340 2023-07-12 07:00:35.000000 BaAug-0.1/src/BaAug.egg-info/SOURCES.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        1 2023-07-12 07:00:35.000000 BaAug-0.1/src/BaAug.egg-info/dependency_links.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       86 2023-07-12 07:00:35.000000 BaAug-0.1/src/BaAug.egg-info/requires.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        6 2023-07-12 07:00:35.000000 BaAug-0.1/src/BaAug.egg-info/top_level.txt
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:28:51.592549 BaAug-1.0.0/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      106 2023-07-12 07:28:51.592549 BaAug-1.0.0/PKG-INFO
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-11 06:49:41.000000 BaAug-1.0.0/README.md
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       38 2023-07-12 07:28:51.592549 BaAug-1.0.0/setup.cfg
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      756 2023-07-12 07:28:49.000000 BaAug-1.0.0/setup.py
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:28:51.588549 BaAug-1.0.0/src/
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:28:51.592549 BaAug-1.0.0/src/BaAug/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     5743 2023-07-12 06:59:53.000000 BaAug-1.0.0/src/BaAug/EDA.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1757 2023-07-12 07:27:29.000000 BaAug-1.0.0/src/BaAug/MTLCombination.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      929 2023-07-12 07:00:13.000000 BaAug-1.0.0/src/BaAug/SentenceBoundary.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     4853 2023-07-12 07:27:20.000000 BaAug-1.0.0/src/BaAug/Single.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     2117 2023-07-12 07:00:05.000000 BaAug-1.0.0/src/BaAug/Word2Vec.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       20 2023-07-12 07:28:38.000000 BaAug-1.0.0/src/BaAug/__init__.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1554 2023-07-12 07:27:52.000000 BaAug-1.0.0/src/BaAug/utils.py
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 07:28:51.592549 BaAug-1.0.0/src/BaAug.egg-info/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      106 2023-07-12 07:28:51.000000 BaAug-1.0.0/src/BaAug.egg-info/PKG-INFO
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      340 2023-07-12 07:28:51.000000 BaAug-1.0.0/src/BaAug.egg-info/SOURCES.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        1 2023-07-12 07:28:51.000000 BaAug-1.0.0/src/BaAug.egg-info/dependency_links.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      101 2023-07-12 07:28:51.000000 BaAug-1.0.0/src/BaAug.egg-info/requires.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        6 2023-07-12 07:28:51.000000 BaAug-1.0.0/src/BaAug.egg-info/top_level.txt
```

### Comparing `BaAug-0.1/setup.py` & `BaAug-1.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from setuptools import setup, find_packages
 
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 setup(
     name='BaAug',
-    version='0.1',
+    version='1.0.0',
     license='Apache License 2.0',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='Bahnar Augmentation',
     long_description=read('README.md'),
     install_requires=['pyvi', 
                       'simalign', 
                       'sentencepiece', 
                       'transformers', 
                       'sacremoses', 
                       'nltk', 
-                      'numpy', 
+                      'numpy>=1.22.0', 
                       'pandas',
-                      'gensim',
+                      'gensim>=4.3.0',
                       'openpyxl'
                       ],
 )
```

### Comparing `BaAug-0.1/src/BaAug/EDA.py` & `BaAug-1.0.0/src/BaAug/EDA.py`

 * *Files identical despite different names*

### Comparing `BaAug-0.1/src/BaAug/MTLCombination.py` & `BaAug-1.0.0/src/BaAug/MTLCombination.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import math
 import re
 
 
 def da_combine(proportion, keep_old=False):
   def wrap(sentences, loaded_alignments, ba_vi_dict):
     if len(loaded_alignments) < len(sentences):
-        loaded_alignments = build_aligner(sentences=sentences)
+        loaded_alignments.clear()
+        loaded_alignments.extend(build_aligner(sentences=sentences))
     da_pairs = []
     for i in range(len(sentences)):
       ttokens = custom_tokenize(sentences[i][1])
       stokens = custom_tokenize(sentences[i][0])
       alignment = loaded_alignments[i]
       
       n_words_replace = int(len(ttokens)*proportion)
```

### Comparing `BaAug-0.1/src/BaAug/SentenceBoundary.py` & `BaAug-1.0.0/src/BaAug/SentenceBoundary.py`

 * *Files identical despite different names*

### Comparing `BaAug-0.1/src/BaAug/Single.py` & `BaAug-1.0.0/src/BaAug/Single.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import re
 
 
 def da_replaceWord(proportion, keep_old=False):
     def wrap(sentences, loaded_alignments, ba_vi_dict):
         da_pairs = []
         if len(loaded_alignments) < len(sentences):
-            loaded_alignments = build_aligner(sentences=sentences)
+            loaded_alignments.clear()
+            loaded_alignments.extend(build_aligner(sentences=sentences))
         for i in range(len(sentences)):
             ttokens = custom_tokenize(sentences[i][1])
             stokens = custom_tokenize(sentences[i][0])
             alignment = loaded_alignments[i]
             
             n_words_replace=int(len(ttokens)*proportion)
             alg_positions = random.sample(range(len(ttokens)), n_words_replace)
@@ -38,15 +39,16 @@
             da_pairs.extend(sentences)
         return da_pairs
     return wrap
 
 def da_replaceToken(proportion, keep_old=False):
     def wrap(sentences, loaded_alignments, ba_vi_dict): 
         if len(loaded_alignments) < len(sentences):
-            loaded_alignments = build_aligner(sentences=sentences) 
+            loaded_alignments.clear()
+            loaded_alignments.extend(build_aligner(sentences=sentences))
         da_pairs = []
         for i in range(len(sentences)):
             ttokens = custom_tokenize(sentences[i][1])
             stokens = custom_tokenize(sentences[i][0])
             alignment = loaded_alignments[i]
             
             n_words_replace = int(len(ttokens)*proportion)
```

### Comparing `BaAug-0.1/src/BaAug/Word2Vec.py` & `BaAug-1.0.0/src/BaAug/Word2Vec.py`

 * *Files identical despite different names*

### Comparing `BaAug-0.1/src/BaAug/utils.py` & `BaAug-1.0.0/src/BaAug/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 def Sequential(*augMethods):
   def wrap(sentences, ba_vi_dict, loaded_alignments=None):
     # if not loaded_alignments:
     # if not ba_vi_dict:
     # loaded_alignments = []
-    if not loaded_alignments:
+    if loaded_alignments is None:
       checkReplaceFunction = reduce(lambda base, x: base or 'replace' in x.__name__ or 'da_combine' in x.__name__, augMethods, False)
       if checkReplaceFunction:
         loaded_alignments = build_aligner(sentences)
     return reduce(lambda x, y: y(x, loaded_alignments, ba_vi_dict), augMethods, sentences)
   return wrap
```

