# Comparing `tmp/kanonym4text-0.2.4.tar.gz` & `tmp/kanonym4text-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanonym4text-0.2.4.tar", last modified: Sun Jul  9 22:36:46 2023, max compression
+gzip compressed data, was "kanonym4text-0.2.5.tar", last modified: Wed Jul 12 13:24:38 2023, max compression
```

## Comparing `kanonym4text-0.2.4.tar` & `kanonym4text-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 22:36:46.782323 kanonym4text-0.2.4/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-09 22:36:46.782323 kanonym4text-0.2.4/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     4896 2023-07-09 13:23:33.000000 kanonym4text-0.2.4/README.md
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 22:36:46.778324 kanonym4text-0.2.4/kanonym4text/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      119 2023-07-06 09:36:30.000000 kanonym4text-0.2.4/kanonym4text/__init__.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 22:36:46.782323 kanonym4text-0.2.4/kanonym4text/data/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    35592 2023-07-01 20:45:19.000000 kanonym4text-0.2.4/kanonym4text/data/5000_most_common_words_by_order.txt
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 22:36:46.782323 kanonym4text-0.2.4/kanonym4text/objects/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       52 2023-07-06 09:06:10.000000 kanonym4text-0.2.4/kanonym4text/objects/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8210 2023-07-09 14:14:56.000000 kanonym4text-0.2.4/kanonym4text/objects/kanonym.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 22:36:46.782323 kanonym4text-0.2.4/kanonym4text/utils/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-07-01 20:45:19.000000 kanonym4text-0.2.4/kanonym4text/utils/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13287 2023-07-06 10:50:11.000000 kanonym4text-0.2.4/kanonym4text/utils/anonym_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8723 2023-07-06 10:17:19.000000 kanonym4text-0.2.4/kanonym4text/utils/cluster_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6355 2023-07-09 14:30:42.000000 kanonym4text-0.2.4/kanonym4text/utils/llm_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      721 2023-07-05 07:09:39.000000 kanonym4text-0.2.4/kanonym4text/utils/models.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11168 2023-07-06 08:39:12.000000 kanonym4text-0.2.4/kanonym4text/utils/nlp_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3152 2023-07-06 08:40:32.000000 kanonym4text-0.2.4/kanonym4text/utils/utilization_utils.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 22:36:46.778324 kanonym4text-0.2.4/kanonym4text.egg-info/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-09 22:36:46.000000 kanonym4text-0.2.4/kanonym4text.egg-info/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      576 2023-07-09 22:36:46.000000 kanonym4text-0.2.4/kanonym4text.egg-info/SOURCES.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        1 2023-07-09 22:36:46.000000 kanonym4text-0.2.4/kanonym4text.egg-info/dependency_links.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      189 2023-07-09 22:36:46.000000 kanonym4text-0.2.4/kanonym4text.egg-info/requires.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       13 2023-07-09 22:36:46.000000 kanonym4text-0.2.4/kanonym4text.egg-info/top_level.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       38 2023-07-09 22:36:46.782323 kanonym4text-0.2.4/setup.cfg
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     1571 2023-07-09 22:36:15.000000 kanonym4text-0.2.4/setup.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-12 13:24:38.988110 kanonym4text-0.2.5/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-12 13:24:38.988110 kanonym4text-0.2.5/PKG-INFO
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     4896 2023-07-09 13:23:33.000000 kanonym4text-0.2.5/README.md
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-12 13:24:38.988110 kanonym4text-0.2.5/kanonym4text/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      119 2023-07-06 09:36:30.000000 kanonym4text-0.2.5/kanonym4text/__init__.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-12 13:24:38.988110 kanonym4text-0.2.5/kanonym4text/data/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    35592 2023-07-01 20:45:19.000000 kanonym4text-0.2.5/kanonym4text/data/5000_most_common_words_by_order.txt
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-12 13:24:38.988110 kanonym4text-0.2.5/kanonym4text/objects/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       52 2023-07-06 09:06:10.000000 kanonym4text-0.2.5/kanonym4text/objects/__init__.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8241 2023-07-12 13:18:58.000000 kanonym4text-0.2.5/kanonym4text/objects/kanonym.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-12 13:24:38.988110 kanonym4text-0.2.5/kanonym4text/utils/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-07-01 20:45:19.000000 kanonym4text-0.2.5/kanonym4text/utils/__init__.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13287 2023-07-06 10:50:11.000000 kanonym4text-0.2.5/kanonym4text/utils/anonym_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8723 2023-07-06 10:17:19.000000 kanonym4text-0.2.5/kanonym4text/utils/cluster_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6355 2023-07-09 14:30:42.000000 kanonym4text-0.2.5/kanonym4text/utils/llm_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      721 2023-07-05 07:09:39.000000 kanonym4text-0.2.5/kanonym4text/utils/models.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11183 2023-07-12 13:09:40.000000 kanonym4text-0.2.5/kanonym4text/utils/nlp_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3152 2023-07-06 08:40:32.000000 kanonym4text-0.2.5/kanonym4text/utils/utilization_utils.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-12 13:24:38.988110 kanonym4text-0.2.5/kanonym4text.egg-info/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-12 13:24:38.000000 kanonym4text-0.2.5/kanonym4text.egg-info/PKG-INFO
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      576 2023-07-12 13:24:38.000000 kanonym4text-0.2.5/kanonym4text.egg-info/SOURCES.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        1 2023-07-12 13:24:38.000000 kanonym4text-0.2.5/kanonym4text.egg-info/dependency_links.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      211 2023-07-12 13:24:38.000000 kanonym4text-0.2.5/kanonym4text.egg-info/requires.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       13 2023-07-12 13:24:38.000000 kanonym4text-0.2.5/kanonym4text.egg-info/top_level.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       38 2023-07-12 13:24:38.988110 kanonym4text-0.2.5/setup.cfg
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     1604 2023-07-12 13:24:31.000000 kanonym4text-0.2.5/setup.py
```

### Comparing `kanonym4text-0.2.4/PKG-INFO` & `kanonym4text-0.2.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: kanonym4text
-Version: 0.2.4
+Version: 0.2.5
 Summary: k-anonymity for texts
 Home-page: https://github.com/neumanh/K-anonymity-fot-texts
 Author: Lior Trieman, Hadas Neuman
 Author-email: liortr30@gmail.com, hadas.doron@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.4.tar.gz
+Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.5.tar.gz
 Description: A package that takes a dataframe with a corpus and return an anonymized corpus
 Keywords: python,k-anonymity,privacy,NLP
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `kanonym4text-0.2.4/README.md` & `kanonym4text-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.4/kanonym4text/data/5000_most_common_words_by_order.txt` & `kanonym4text-0.2.5/kanonym4text/data/5000_most_common_words_by_order.txt`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.4/kanonym4text/objects/kanonym.py` & `kanonym4text-0.2.5/kanonym4text/objects/kanonym.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
     def anonymize(self, df: pd.DataFrame, k: int, col: str = 'txt', plot: bool = False,
                   num_stop: int = 1000, n_jobs: int = 1, verbose: int = 0):
         """
         """
         self._init_logger(verbose)
-        logging.info(f'{os.path.basename(__file__)} WE pipeline')
+        logging.info(f'{os.path.basename(__file__)} WE pipeline. WE model: {self.wemodel_name}')
 
         logging.info(f'Number of documents: {df.shape[0]}')  # Logging
 
         # Collecting stopword list
         short_stopword_list, long_stopword_list = self._get_stop(num_stop)
         logging.info(f'Stopword list contains {len(long_stopword_list)} words')
```

### Comparing `kanonym4text-0.2.4/kanonym4text/utils/anonym_utils.py` & `kanonym4text-0.2.5/kanonym4text/utils/anonym_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.4/kanonym4text/utils/cluster_utils.py` & `kanonym4text-0.2.5/kanonym4text/utils/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.4/kanonym4text/utils/llm_utils.py` & `kanonym4text-0.2.5/kanonym4text/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.4/kanonym4text/utils/models.py` & `kanonym4text-0.2.5/kanonym4text/utils/models.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.4/kanonym4text/utils/nlp_utils.py` & `kanonym4text-0.2.5/kanonym4text/utils/nlp_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Imports
 import pandas as pd
 import numpy as np
 import re
 from nltk.corpus import stopwords
 from nltk.tokenize import word_tokenize
-import spacy
-import re
+# import spacy
 import bz2
 from collections import defaultdict
 import operator
 import logging
+import en_core_web_sm
 
 # Defining some global variables
 stopword_list = None
 
 short_stopword_list = None
 long_stopword_list = None
 
-nlp = spacy.load('en_core_web_sm', disable=['ner', 'parser'])  # disabling Named Entity Recognition for speed
-# we_model = models.we_model
+# nlp = spacy.load('en_core_web_sm', disable=['ner', 'parser'])  # disabling Named Entity Recognition for speed
+nlp = en_core_web_sm.load()
 
 def get_list_from_file(file_name, num):
     """"
     Reads a file with words (each word on different line) and returns a list of these words.
     """
     try:
         with open(file_name, 'r') as file:
```

### Comparing `kanonym4text-0.2.4/kanonym4text/utils/utilization_utils.py` & `kanonym4text-0.2.5/kanonym4text/utils/utilization_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.4/kanonym4text.egg-info/PKG-INFO` & `kanonym4text-0.2.5/kanonym4text.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: kanonym4text
-Version: 0.2.4
+Version: 0.2.5
 Summary: k-anonymity for texts
 Home-page: https://github.com/neumanh/K-anonymity-fot-texts
 Author: Lior Trieman, Hadas Neuman
 Author-email: liortr30@gmail.com, hadas.doron@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.4.tar.gz
+Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.5.tar.gz
 Description: A package that takes a dataframe with a corpus and return an anonymized corpus
 Keywords: python,k-anonymity,privacy,NLP
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `kanonym4text-0.2.4/kanonym4text.egg-info/SOURCES.txt` & `kanonym4text-0.2.5/kanonym4text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.4/setup.py` & `kanonym4text-0.2.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 DESCRIPTION = 'k-anonymity for texts'
 LONG_DESCRIPTION = 'A package that takes a dataframe with a corpus and return an anonymized corpus'
 
 # Setting up
 setup(
     name="kanonym4text",
     version=VERSION,
     author="Lior Trieman, Hadas Neuman",
     author_email="liortr30@gmail.com, hadas.doron@gmail.com",
     url='https://github.com/neumanh/K-anonymity-fot-texts',
 
-    download_url='https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.4.tar.gz',
+    download_url='https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.5.tar.gz',
 
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # package_dir={'kanonym4text': 'kanonym4text'},
     install_requires=[
@@ -26,15 +26,16 @@
         'gensim==4.3.1',
         'torch==2.0.1',
         'transformers==4.29.0',
         'sentence-transformers==2.2.2',
         'spacy==3.5.3',
         'nltk==3.8.1',
         'annoy==1.17.2',
-        'k-means-constrained==0.7.2'
+        'k-means-constrained==0.7.2',
+        'en_core_web_sm==3.6.0'
     ],
     keywords=['python', 'k-anonymity', 'privacy', 'NLP'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

