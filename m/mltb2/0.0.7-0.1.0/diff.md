# Comparing `tmp/mltb2-0.0.7.tar.gz` & `tmp/mltb2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltb2-0.0.7.tar", last modified: Thu Jul  6 20:19:41 2023, max compression
+gzip compressed data, was "mltb2-0.1.0.tar", last modified: Wed Jul 12 19:21:31 2023, max compression
```

## Comparing `mltb2-0.0.7.tar` & `mltb2-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:19:41.479008 mltb2-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-06 20:19:31.000000 mltb2-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:19:31.000000 mltb2-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-06 20:19:41.479008 mltb2-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-06 20:19:31.000000 mltb2-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:19:41.475008 mltb2-0.0.7/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-06 20:19:31.000000 mltb2-0.0.7/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:19:41.475008 mltb2-0.0.7/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 20:19:41.000000 mltb2-0.0.7/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-06 20:19:31.000000 mltb2-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 20:19:41.479008 mltb2-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-06 20:19:31.000000 mltb2-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:19:41.479008 mltb2-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-06 20:19:31.000000 mltb2-0.0.7/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:21:31.969387 mltb2-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-12 19:21:14.000000 mltb2-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 19:21:14.000000 mltb2-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-12 19:21:31.969387 mltb2-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-12 19:21:14.000000 mltb2-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:21:31.965387 mltb2-0.1.0/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-12 19:21:14.000000 mltb2-0.1.0/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-12 19:21:14.000000 mltb2-0.1.0/mltb2/fasttxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-12 19:21:14.000000 mltb2-0.1.0/mltb2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-07-12 19:21:14.000000 mltb2-0.1.0/mltb2/optuna_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-12 19:21:14.000000 mltb2-0.1.0/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-12 19:21:14.000000 mltb2-0.1.0/mltb2/somajo_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-12 19:21:14.000000 mltb2-0.1.0/mltb2/somajo_xformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-12 19:21:14.000000 mltb2-0.1.0/mltb2/xformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:21:31.965387 mltb2-0.1.0/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-12 19:21:31.000000 mltb2-0.1.0/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-12 19:21:31.000000 mltb2-0.1.0/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:21:31.000000 mltb2-0.1.0/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 19:21:31.000000 mltb2-0.1.0/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 19:21:31.000000 mltb2-0.1.0/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-12 19:21:14.000000 mltb2-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 19:21:31.969387 mltb2-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-12 19:21:14.000000 mltb2-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:21:31.969387 mltb2-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 19:21:14.000000 mltb2-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-12 19:21:14.000000 mltb2-0.1.0/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-12 19:21:14.000000 mltb2-0.1.0/tests/test_fasttxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-12 19:21:14.000000 mltb2-0.1.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-12 19:21:14.000000 mltb2-0.1.0/tests/test_optuna_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-12 19:21:14.000000 mltb2-0.1.0/tests/test_somajo_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-12 19:21:14.000000 mltb2-0.1.0/tests/test_somajo_xformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-12 19:21:14.000000 mltb2-0.1.0/tests/test_xformer.py
```

### Comparing `mltb2-0.0.7/LICENSE` & `mltb2-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.7/README.md` & `mltb2-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,67 @@
+Metadata-Version: 2.1
+Name: mltb2
+Version: 0.1.0
+Summary: Machine Learning Toolbox
+Home-page: https://github.com/telekom/mltb2
+Author: Philip May
+Author-email: philip@may.la
+Maintainer: Philip May
+Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
+Project-URL: Documentation, https://telekom.github.io/mltb2/
+Project-URL: Source Code, https://github.com/telekom/mltb2
+Keywords: optuna deep-learning ml ai machine-learning hyperparameter-optimization
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: files
+Provides-Extra: fasttext
+Provides-Extra: optuna
+Provides-Extra: plot
+Provides-Extra: somajo
+Provides-Extra: transformers
+Provides-Extra: somajo_transformers
+Provides-Extra: optional
+Provides-Extra: checking
+Provides-Extra: testing
+Provides-Extra: doc
+Provides-Extra: all
+License-File: LICENSE
+
 # Machine Learning Toolbox 2 - MLTB2
 
 [![MIT License](https://img.shields.io/github/license/telekom/mltb2)](https://github.com/telekom/mltb2/blob/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/mltb2)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/mltb2.svg)](https://pypi.python.org/pypi/mltb2)
 <br/>
 [![pytest](https://github.com/telekom/mltb2/actions/workflows/pytest.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/pytest.yml)
 [![Static Code Checks](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml)
 [![Build & Deploy Doc](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml)
 [![GitHub issues](https://img.shields.io/github/issues-raw/telekom/mltb2)](https://github.com/telekom/mltb2/issues)
 
 📦 A box of machine learning tools. 📦
 
-## Components and Documentation
-
 [Documentation Page](https://telekom.github.io/mltb2/)
 
-[`from mltb2.somajo import SoMaJoSentenceSplitter`](https://telekom.github.io/mltb2/api-reference/somajo.html#mltb2.somajo.SoMaJoSentenceSplitter)\
-Split texts into sentences. For German and English language.
-This is done with the [SoMaJo](https://github.com/tsproisl/SoMaJo) tool.
-
-[`from mltb2.somajo import JaccardSimilarity`](https://telekom.github.io/mltb2/api-reference/somajo.html#mltb2.somajo.JaccardSimilarity)\
-Calculate the [jaccard similarity](https://en.wikipedia.org/wiki/Jaccard_index).
-
-[`from mltb2.transformers import TransformersTokenCounter`](https://telekom.github.io/mltb2/api-reference/transformers.html#mltb2.transformers.TransformersTokenCounter)\
-Count tokens made by a [Transformers](https://github.com/huggingface/transformers) tokenizer.
-
-[`from mltb2.somajo_transformers import TextSplitter`](https://telekom.github.io/mltb2/api-reference/somajo_transformers.html#mltb2.somajo_transformers.TextSplitter)\
-Split the text into sections with a specified maximum token length.
-Does not divide words, but always whole sentences.
-
-[`from mltb2.optuna import SignificanceRepeatedTrainingPruner`](https://telekom.github.io/mltb2/api-reference/optuna.html#mltb2.optuna.SignificanceRepeatedTrainingPruner)\
-An [Optuna pruner](https://optuna.readthedocs.io/en/stable/reference/pruners.html)
-to use statistical significance (a t-test which serves as a heuristic) to stop
-unpromising trials early, avoiding unnecessary repeated training during cross validation.
-
 ## Installation
 
 MLTB2 is available at [the Python Package Index (PyPI)](https://pypi.org/project/mltb2/).
 It can be installed with pip:
 
 ```bash
 pip install mltb2
```

### Comparing `mltb2-0.0.7/mltb2/fasttext.py` & `mltb2-0.1.0/mltb2/fasttxt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""fastText specific functionality.
+"""fastText specific tools.
 
 This module is based on `fastText <https://fasttext.cc/docs/en/support.html>`_.
 Use pip to install the necessary dependencies for this module:
 ``pip install mltb2[fasttext]``
 """
 
 import os
```

### Comparing `mltb2-0.0.7/mltb2/files.py` & `mltb2-0.1.0/mltb2/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""File utils.
+"""File tools.
 
 Use pip to install the necessary dependencies for this module:
 ``pip install mltb2[files]``
 """
 
 
 import os
```

### Comparing `mltb2-0.0.7/mltb2/optuna.py` & `mltb2-0.1.0/mltb2/optuna_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2021 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""Optuna specific functionality.
+"""Optuna specific tools.
 
 This module is based on `Optuna <https://optuna.readthedocs.io/en/stable/>`_.
 Use pip to install the necessary dependencies for this module:
 ``pip install mltb2[optuna]``
 """
 
 
@@ -35,15 +35,15 @@
     once per epoch. In contrast, this pruner does not work on intermediate results but on the
     results of a cross validation or more precisely the results of the individual folds.
 
     Below is a minimalist example:
 
     .. testcode::
 
-        from mltb2.optuna import SignificanceRepeatedTrainingPruner
+        from mltb2.optuna_tool import SignificanceRepeatedTrainingPruner
         import logging
         import numpy as np
         import optuna
         from sklearn.datasets import load_iris
         from sklearn.model_selection import StratifiedKFold
         from sklearn.ensemble import RandomForestClassifier
         from sklearn.metrics import accuracy_score
```

### Comparing `mltb2-0.0.7/mltb2/plot.py` & `mltb2-0.1.0/mltb2/plot.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.7/mltb2/somajo.py` & `mltb2-0.1.0/mltb2/somajo_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""SoMaJo specific functionality.
+"""SoMaJo specific tools.
 
 This module is based on `SoMaJo <https://github.com/tsproisl/SoMaJo>`_.
 Use pip to install the necessary dependencies for this module:
 ``pip install mltb2[somajo]``
 """
 
 
 from abc import ABC
 from dataclasses import dataclass, field
-from typing import Container, Iterable, List, Optional, Set
+from typing import Container, Iterable, List, Optional, Set, Union
 
 from somajo import SoMaJo
 from tqdm import tqdm
 
 
 @dataclass
 class SoMaJoBaseClass(ABC):
@@ -155,18 +155,36 @@
 class TokenExtractor(SoMaJoBaseClass):
     """Extract tokens from text.
 
     Args:
         language: The language. ``de_CMC`` for German or ``en_PTB`` for English.
     """
 
-    def extract_url_set(self, text: str) -> Set[str]:
+    def extract_url_set(self, text: Union[Iterable, str]) -> Set[str]:
         """Extract URLs from text.
 
+        An example:
+
+        .. testcode::
+
+            from mltb2.somajo_tool import TokenExtractor
+
+            token_extractor = TokenExtractor("de_CMC")
+            url_set = token_extractor.extract_url_set("Das ist ein Link: http://github.com")
+            print(url_set)
+
+        Example output:
+
+        .. testoutput::
+
+            {'http://github.com'}
+
         Args:
             text: the text
         Returns:
             Set of extracted links.
         """
-        sentences = self.somajo.tokenize_text([text])
+        if isinstance(text, str):
+            text = [text]
+        sentences = self.somajo.tokenize_text(text)
         result = extract_token_class_set(sentences, keep_token_classes="URL")
         return result
```

### Comparing `mltb2-0.0.7/mltb2/somajo_transformers.py` & `mltb2-0.1.0/mltb2/somajo_xformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Copyright (c) 2023 Philip May
 # Copyright (c) 2023 Philip May, Deutsche Telekom AG
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""Hugging Face Transformers and SoMaJo specific functionality.
+"""Hugging Face Transformers and SoMaJo specific tools.
 
 This module is based on
 `Hugging Face Transformers <https://huggingface.co/docs/transformers/index>`_ and
 `SoMaJo <https://github.com/tsproisl/SoMaJo>`_.
 Use pip to install the necessary dependencies for this module:
 ``pip install mltb2[somajo_transformers]``
 """
 
 
 from dataclasses import dataclass
 from typing import List
 
 from tqdm import tqdm
 
-from mltb2.somajo import SoMaJoSentenceSplitter
-from mltb2.transformers import TransformersTokenCounter
+from mltb2.somajo_tool import SoMaJoSentenceSplitter
+from mltb2.xformer import TransformersTokenCounter
 
 
 @dataclass
 class TextSplitter:
     """Split the text into sections with a specified maximum token number.
 
     Does not divide words, but always whole sentences.
```

### Comparing `mltb2-0.0.7/mltb2/transformers.py` & `mltb2-0.1.0/mltb2/xformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""Hugging Face Transformers specific functionality.
+"""Hugging Face Transformers specific tools.
 
 This module is based on
 `Hugging Face Transformers <https://huggingface.co/docs/transformers/index>`_.
 Use pip to install the necessary dependencies for this module:
 ``pip install mltb2[transformers]``
 """
```

### Comparing `mltb2-0.0.7/mltb2.egg-info/SOURCES.txt` & `mltb2-0.1.0/mltb2.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 mltb2/__init__.py
-mltb2/fasttext.py
+mltb2/fasttxt.py
 mltb2/files.py
-mltb2/optuna.py
+mltb2/optuna_tool.py
 mltb2/plot.py
-mltb2/somajo.py
-mltb2/somajo_transformers.py
-mltb2/transformers.py
+mltb2/somajo_tool.py
+mltb2/somajo_xformer.py
+mltb2/xformer.py
 mltb2.egg-info/PKG-INFO
 mltb2.egg-info/SOURCES.txt
 mltb2.egg-info/dependency_links.txt
 mltb2.egg-info/requires.txt
 mltb2.egg-info/top_level.txt
 tests/__init__.py
 tests/test__init__.py
-tests/test_fasttext.py
+tests/test_fasttxt.py
 tests/test_files.py
-tests/test_optuna.py
-tests/test_somajo.py
-tests/test_somajo_transformers.py
-tests/test_transformers.py
+tests/test_optuna_tool.py
+tests/test_somajo_tool.py
+tests/test_somajo_xformer.py
+tests/test_xformer.py
```

### Comparing `mltb2-0.0.7/pyproject.toml` & `mltb2-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.7/setup.py` & `mltb2-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.7/tests/test_fasttext.py` & `mltb2-0.1.0/tests/test_fasttxt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 
-from mltb2.fasttext import FastTextLanguageIdentification
+from mltb2.fasttxt import FastTextLanguageIdentification
 
 
 def test_fasttext_language_identification_get_model_path_and_download():
     model_path = FastTextLanguageIdentification.get_model_path_and_download()
     assert model_path is not None
```

### Comparing `mltb2-0.0.7/tests/test_files.py` & `mltb2-0.1.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.7/tests/test_optuna.py` & `mltb2-0.1.0/tests/test_optuna_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) 2021 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 import pytest
 
-from mltb2.optuna import SignificanceRepeatedTrainingPruner
+from mltb2.optuna_tool import SignificanceRepeatedTrainingPruner
 
 
 def test_percentile_pruner_n_warmup_steps() -> None:
     SignificanceRepeatedTrainingPruner(n_warmup_steps=2)
     SignificanceRepeatedTrainingPruner(n_warmup_steps=0)
 
     with pytest.raises(ValueError):
```

### Comparing `mltb2-0.0.7/tests/test_somajo.py` & `mltb2-0.1.0/tests/test_somajo_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 from math import isclose
 
 from somajo import SoMaJo
 
-from mltb2.somajo import JaccardSimilarity, SoMaJoSentenceSplitter, TokenExtractor, detokenize, extract_token_class_set
+from mltb2.somajo_tool import (
+    JaccardSimilarity,
+    SoMaJoSentenceSplitter,
+    TokenExtractor,
+    detokenize,
+    extract_token_class_set,
+)
 
 
 def test_SoMaJoSentenceSplitter_call() -> None:
     """Test ``SoMaJoSentenceSplitter.call`` happy case."""
     splitter = SoMaJoSentenceSplitter("de_CMC")
     text = "Das ist der erste Satz. Das ist der 2. Satz."
     sentences = splitter(text)
@@ -57,26 +63,37 @@
     text2 = "Vollkommen anders!"
     jaccard_similarity = JaccardSimilarity("de_CMC")
     result = jaccard_similarity(text1, text2)
 
     assert isclose(result, 0.0)
 
 
-def test_TokenExtractor_call():
+def test_TokenExtractor_extract_url_set_with_str():
     url1 = "http://may.la"
     url2 = "github.com"
     text_with_url = f"{url1} Das ist ein Text. {url2} Er enthält eine URL."
     token_extractor = TokenExtractor("de_CMC")
     result = token_extractor.extract_url_set(text_with_url)
     assert len(result) == 2
     assert url1 in result
     assert url2 in result
 
 
-def test_TokenExtractor_call_no_url():
+def test_TokenExtractor_extract_url_set_with_list():
+    url1 = "http://may.la"
+    url2 = "github.com"
+    text_with_url = [f"{url1} Das ist ein Text.", f"{url2} Er enthält eine URL."]
+    token_extractor = TokenExtractor("de_CMC")
+    result = token_extractor.extract_url_set(text_with_url)
+    assert len(result) == 2
+    assert url1 in result
+    assert url2 in result
+
+
+def test_TokenExtractor_extract_url_set_no_url():
     text_with_url = "Das ist ein Text. Er enthält keine URLs."
     token_extractor = TokenExtractor("de_CMC")
     result = token_extractor.extract_url_set(text_with_url)
     assert len(result) == 0
 
 
 def test_extract_token_class_set_symbol():
```

### Comparing `mltb2-0.0.7/tests/test_somajo_transformers.py` & `mltb2-0.1.0/tests/test_somajo_xformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Copyright (c) 2023 Philip May, Deutsche Telekom AG
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 
 import pytest
 
-from mltb2.somajo import SoMaJoSentenceSplitter
-from mltb2.somajo_transformers import TextSplitter
-from mltb2.transformers import TransformersTokenCounter
+from mltb2.somajo_tool import SoMaJoSentenceSplitter
+from mltb2.somajo_xformer import TextSplitter
+from mltb2.xformer import TransformersTokenCounter
 
 
 def test_TextSplitter_call():
     somajo_sentence_splitter = SoMaJoSentenceSplitter("de_CMC")
     transformers_token_counter = TransformersTokenCounter("deepset/gbert-base")
     text_splitter = TextSplitter(
         max_token=12,
```

### Comparing `mltb2-0.0.7/tests/test_transformers.py` & `mltb2-0.1.0/tests/test_xformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 
-from mltb2.transformers import TransformersTokenCounter
+from mltb2.xformer import TransformersTokenCounter
 
 
 def test_TransformersTokenCounter_call_string():
     transformers_token_counter = TransformersTokenCounter("deepset/gbert-base")
     token_count = transformers_token_counter("Das ist ein Text.")
 
     assert token_count == 5
```

