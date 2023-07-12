# Comparing `tmp/rankfmc-0.2.6.tar.gz` & `tmp/rankfmc-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankfmc-0.2.6.tar", last modified: Mon Jul 10 09:40:46 2023, max compression
+gzip compressed data, was "rankfmc-0.2.7.tar", last modified: Wed Jul 12 09:14:34 2023, max compression
```

## Comparing `rankfmc-0.2.6.tar` & `rankfmc-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:46.054237 rankfmc-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 09:40:32.000000 rankfmc-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 09:40:32.000000 rankfmc-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-07-10 09:40:46.054237 rankfmc-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-10 09:40:32.000000 rankfmc-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:46.054237 rankfmc-0.2.6/rankfmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:32.000000 rankfmc-0.2.6/rankfmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1052362 2023-07-10 09:40:45.000000 rankfmc-0.2.6/rankfmc/_rankfm.c
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-10 09:40:32.000000 rankfmc-0.2.6/rankfmc/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:46.054237 rankfmc-0.2.6/rankfmc/mt19937ar/
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-10 09:40:32.000000 rankfmc-0.2.6/rankfmc/mt19937ar/mt19937ar.c
--rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-07-10 09:40:32.000000 rankfmc-0.2.6/rankfmc/rankfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-10 09:40:32.000000 rankfmc-0.2.6/rankfmc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:40:46.054237 rankfmc-0.2.6/rankfmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-07-10 09:40:46.000000 rankfmc-0.2.6/rankfmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-10 09:40:46.000000 rankfmc-0.2.6/rankfmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:40:46.000000 rankfmc-0.2.6/rankfmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:40:46.000000 rankfmc-0.2.6/rankfmc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 09:40:46.000000 rankfmc-0.2.6/rankfmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 09:40:46.000000 rankfmc-0.2.6/rankfmc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:40:46.054237 rankfmc-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-10 09:40:32.000000 rankfmc-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:34.031236 rankfmc-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-12 09:14:17.000000 rankfmc-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-12 09:14:17.000000 rankfmc-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10339 2023-07-12 09:14:34.031236 rankfmc-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9746 2023-07-12 09:14:17.000000 rankfmc-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:34.031236 rankfmc-0.2.7/rankfmc/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1052362 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc/_rankfm.c
+-rw-r--r--   0 runner    (1001) docker     (122)     9296 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:34.031236 rankfmc-0.2.7/rankfmc/mt19937ar/
+-rw-r--r--   0 runner    (1001) docker     (122)     5923 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/mt19937ar/mt19937ar.c
+-rw-r--r--   0 runner    (1001) docker     (122)    21516 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/rankfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-07-12 09:14:17.000000 rankfmc-0.2.7/rankfmc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:14:34.031236 rankfmc-0.2.7/rankfmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10339 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-12 09:14:34.000000 rankfmc-0.2.7/rankfmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-12 09:14:33.000000 rankfmc-0.2.7/rankfmc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 09:14:34.031236 rankfmc-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-07-12 09:14:17.000000 rankfmc-0.2.7/setup.py
```

### Comparing `rankfmc-0.2.6/LICENSE` & `rankfmc-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.6/PKG-INFO` & `rankfmc-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: rankfmc
-Version: 0.2.6
+Version: 0.2.7
 Summary: a python implementation of the generic factorization machines model class adapted for collaborative filtering recommendation problems with implicit feedback user-item interaction data and (optionally) additional user/item side features
-Home-page: https://github.com/etlundquist/rankfmc
-Author: Eric Lundquist
-Author-email: e.t.lundquist@gmail.com
+Home-page: https://github.com/ErraticO/rankfmc
+Author: ErraticO
+Author-email: wyh123132@163.com
 License: GNU General Public License v3.0
 Keywords: machine,learning,recommendation,factorization,machines,implicit
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RankFM
 
 [![PyPI version](https://badge.fury.io/py/rankfm.svg)](https://badge.fury.io/py/rankfm)
 [![CircleCI](https://circleci.com/gh/etlundquist/rankfm.svg?style=shield)](https://circleci.com/gh/etlundquist/rankfm)
 [![Documentation Status](https://readthedocs.org/projects/rankfm/badge/?version=latest)](https://rankfm.readthedocs.io/en/latest/?badge=latest)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
+[[original author]](https://github.com/etlundquist/rankfm)
+
 RankFM is a python implementation of the general [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf) model class adapted for collaborative filtering recommendation/ranking problems with implicit feedback user/item interaction data. It uses [Bayesian Personalized Ranking (BPR)](https://arxiv.org/pdf/1205.2618.pdf) and a variant of [Weighted Approximate-Rank Pairwise (WARP)](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.587.3946&rep=rep1&type=pdf) loss to learn model weights via Stochastic Gradient Descent (SGD). It can (optionally) incorporate sample weights and user/item auxiliary features to augment the main interaction data.
 
 The core (training, prediction, recommendation) methods are written in [Cython](https://cython.org/), making it possible to scale to millions of user/item interactions. Designed for ease-of-use, RankFM accepts both `pd.DataFrame` and `np.ndarray` inputs - you do not have to convert your data to `scipy.sparse` matrices or re-map user/item identifiers prior to use. RankFM internally maps all user/item identifiers to zero-based integer indexes, but always converts its output back to the original user/item identifiers from your data, which can be arbitrary (non-zero-based, non-consecutive) integers or even strings.
 
 In addition to the familiar `fit()`, `predict()`, `recommend()` methods, RankFM includes additional utilities `similiar_users()` and `similar_items()` to find the most similar users/items to a given user/item based on latent factor space embeddings. A number of popular recommendation/ranking evaluation metric functions have been included in the separate `evaluation` module to streamline model tuning and validation.
 
 * see the **Quickstart** section below to get started with the basic functionality
 * see the `/examples` folder for more in-depth jupyter notebook walkthroughs with several popular open-source data sets
 * see the [Online Documentation](https://rankfm.readthedocs.io/en/latest/) for more comprehensive documentation on the main model class and separate evaluation module
 * see the [Medium Article](https://towardsdatascience.com/factorization-machines-for-item-recommendation-with-implicit-feedback-data-5655a7c749db) for contextual motivation and a detailed mathematical description of the algorithm
 
 ---
 ### Dependencies
-* Python 3.6+
+* Python 3.9+
 * numpy >= 1.15
 * pandas >= 1.5
 
 ### Installation
 
 #### Prerequisites
```

### Comparing `rankfmc-0.2.6/README.md` & `rankfmc-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # RankFM
 
 [![PyPI version](https://badge.fury.io/py/rankfm.svg)](https://badge.fury.io/py/rankfm)
 [![CircleCI](https://circleci.com/gh/etlundquist/rankfm.svg?style=shield)](https://circleci.com/gh/etlundquist/rankfm)
 [![Documentation Status](https://readthedocs.org/projects/rankfm/badge/?version=latest)](https://rankfm.readthedocs.io/en/latest/?badge=latest)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
+[[original author]](https://github.com/etlundquist/rankfm)
+
 RankFM is a python implementation of the general [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf) model class adapted for collaborative filtering recommendation/ranking problems with implicit feedback user/item interaction data. It uses [Bayesian Personalized Ranking (BPR)](https://arxiv.org/pdf/1205.2618.pdf) and a variant of [Weighted Approximate-Rank Pairwise (WARP)](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.587.3946&rep=rep1&type=pdf) loss to learn model weights via Stochastic Gradient Descent (SGD). It can (optionally) incorporate sample weights and user/item auxiliary features to augment the main interaction data.
 
 The core (training, prediction, recommendation) methods are written in [Cython](https://cython.org/), making it possible to scale to millions of user/item interactions. Designed for ease-of-use, RankFM accepts both `pd.DataFrame` and `np.ndarray` inputs - you do not have to convert your data to `scipy.sparse` matrices or re-map user/item identifiers prior to use. RankFM internally maps all user/item identifiers to zero-based integer indexes, but always converts its output back to the original user/item identifiers from your data, which can be arbitrary (non-zero-based, non-consecutive) integers or even strings.
 
 In addition to the familiar `fit()`, `predict()`, `recommend()` methods, RankFM includes additional utilities `similiar_users()` and `similar_items()` to find the most similar users/items to a given user/item based on latent factor space embeddings. A number of popular recommendation/ranking evaluation metric functions have been included in the separate `evaluation` module to streamline model tuning and validation.
 
 * see the **Quickstart** section below to get started with the basic functionality
 * see the `/examples` folder for more in-depth jupyter notebook walkthroughs with several popular open-source data sets
 * see the [Online Documentation](https://rankfm.readthedocs.io/en/latest/) for more comprehensive documentation on the main model class and separate evaluation module
 * see the [Medium Article](https://towardsdatascience.com/factorization-machines-for-item-recommendation-with-implicit-feedback-data-5655a7c749db) for contextual motivation and a detailed mathematical description of the algorithm
 
 ---
 ### Dependencies
-* Python 3.6+
+* Python 3.9+
 * numpy >= 1.15
 * pandas >= 1.5
 
 ### Installation
 
 #### Prerequisites
```

### Comparing `rankfmc-0.2.6/rankfmc/_rankfm.c` & `rankfmc-0.2.7/rankfmc/_rankfm.c`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.6/rankfmc/evaluation.py` & `rankfmc-0.2.7/rankfmc/evaluation.py`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.6/rankfmc/mt19937ar/mt19937ar.c` & `rankfmc-0.2.7/rankfmc/mt19937ar/mt19937ar.c`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.6/rankfmc/rankfm.py` & `rankfmc-0.2.7/rankfmc/rankfm.py`

 * *Files identical despite different names*

### Comparing `rankfmc-0.2.6/rankfmc.egg-info/PKG-INFO` & `rankfmc-0.2.7/rankfmc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: rankfmc
-Version: 0.2.6
+Version: 0.2.7
 Summary: a python implementation of the generic factorization machines model class adapted for collaborative filtering recommendation problems with implicit feedback user-item interaction data and (optionally) additional user/item side features
-Home-page: https://github.com/etlundquist/rankfmc
-Author: Eric Lundquist
-Author-email: e.t.lundquist@gmail.com
+Home-page: https://github.com/ErraticO/rankfmc
+Author: ErraticO
+Author-email: wyh123132@163.com
 License: GNU General Public License v3.0
 Keywords: machine,learning,recommendation,factorization,machines,implicit
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RankFM
 
 [![PyPI version](https://badge.fury.io/py/rankfm.svg)](https://badge.fury.io/py/rankfm)
 [![CircleCI](https://circleci.com/gh/etlundquist/rankfm.svg?style=shield)](https://circleci.com/gh/etlundquist/rankfm)
 [![Documentation Status](https://readthedocs.org/projects/rankfm/badge/?version=latest)](https://rankfm.readthedocs.io/en/latest/?badge=latest)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
+[[original author]](https://github.com/etlundquist/rankfm)
+
 RankFM is a python implementation of the general [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf) model class adapted for collaborative filtering recommendation/ranking problems with implicit feedback user/item interaction data. It uses [Bayesian Personalized Ranking (BPR)](https://arxiv.org/pdf/1205.2618.pdf) and a variant of [Weighted Approximate-Rank Pairwise (WARP)](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.587.3946&rep=rep1&type=pdf) loss to learn model weights via Stochastic Gradient Descent (SGD). It can (optionally) incorporate sample weights and user/item auxiliary features to augment the main interaction data.
 
 The core (training, prediction, recommendation) methods are written in [Cython](https://cython.org/), making it possible to scale to millions of user/item interactions. Designed for ease-of-use, RankFM accepts both `pd.DataFrame` and `np.ndarray` inputs - you do not have to convert your data to `scipy.sparse` matrices or re-map user/item identifiers prior to use. RankFM internally maps all user/item identifiers to zero-based integer indexes, but always converts its output back to the original user/item identifiers from your data, which can be arbitrary (non-zero-based, non-consecutive) integers or even strings.
 
 In addition to the familiar `fit()`, `predict()`, `recommend()` methods, RankFM includes additional utilities `similiar_users()` and `similar_items()` to find the most similar users/items to a given user/item based on latent factor space embeddings. A number of popular recommendation/ranking evaluation metric functions have been included in the separate `evaluation` module to streamline model tuning and validation.
 
 * see the **Quickstart** section below to get started with the basic functionality
 * see the `/examples` folder for more in-depth jupyter notebook walkthroughs with several popular open-source data sets
 * see the [Online Documentation](https://rankfm.readthedocs.io/en/latest/) for more comprehensive documentation on the main model class and separate evaluation module
 * see the [Medium Article](https://towardsdatascience.com/factorization-machines-for-item-recommendation-with-implicit-feedback-data-5655a7c749db) for contextual motivation and a detailed mathematical description of the algorithm
 
 ---
 ### Dependencies
-* Python 3.6+
+* Python 3.9+
 * numpy >= 1.15
 * pandas >= 1.5
 
 ### Installation
 
 #### Prerequisites
```

### Comparing `rankfmc-0.2.6/setup.py` & `rankfmc-0.2.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 import glob
 from setuptools import Extension, setup
 
 NAME = 'rankfmc'
-VERSION = '0.2.6'
+VERSION = '0.2.7'
 
 # define the extension packages to include
 # ----------------------------------------
 
 # prefer the generated C extensions when building
 if glob.glob('rankfmc/_rankfm.c'):
     print("building extensions with pre-generated C source...")
@@ -17,16 +17,19 @@
 else:
     print("re-generating C source with cythonize...")
     from Cython.Build import cythonize
     use_cython = True
     ext = 'pyx'
 
 # add compiler arguments to optimize machine code and ignore warnings
-disabled_warnings = ['-Wno-unused-function', '-Wno-uninitialized']
-compile_args = ['-O2', '-ffast-math'] + disabled_warnings
+if sys.platform == "linux":
+    disabled_warnings = ['-Wno-unused-function', '-Wno-uninitialized']
+    compile_args = ['-O2', '-ffast-math'] + disabled_warnings
+else:
+    compile_args = {'gcc': ['/Qstd=c99']}
 
 # define the _rankfm extension including the wrapped MT module
 extensions = [
     Extension(
         name='rankfmc._rankfm',
         sources=['rankfmc/_rankfm.{ext}'.format(ext=ext), 'rankfmc/mt19937ar/mt19937ar.c'],
         extra_compile_args=compile_args
@@ -48,17 +51,17 @@
 setup(
     name=NAME,
     version=VERSION,
     description='a python implementation of the generic factorization machines model class '
                 'adapted for collaborative filtering recommendation problems '
                 'with implicit feedback user-item interaction data '
                 'and (optionally) additional user/item side features',
-    author='Eric Lundquist',
-    author_email='e.t.lundquist@gmail.com',
-    url='https://github.com/etlundquist/rankfmc',
+    author='ErraticO',
+    author_email='wyh123132@163.com',
+    url='https://github.com/ErraticO/rankfmc',
     keywords=['machine', 'learning', 'recommendation', 'factorization', 'machines', 'implicit'],
     license='GNU General Public License v3.0',
     packages=['rankfmc'],
     ext_modules=extensions,
     zip_safe=False,
     python_requires='>=3.9',
     install_requires=['numpy>=1.15', 'pandas>=1.5'],
```

