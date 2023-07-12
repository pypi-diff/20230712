# Comparing `tmp/unitxt-1.0.0.tar.gz` & `tmp/unitxt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitxt-1.0.0.tar", last modified: Mon Jul 10 13:08:10 2023, max compression
+gzip compressed data, was "unitxt-1.0.2.tar", last modified: Wed Jul 12 10:40:38 2023, max compression
```

## Comparing `unitxt-1.0.0.tar` & `unitxt-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-10 13:08:10.126247 unitxt-1.0.0/
--rw-rw-r--   0 elron    (605371) tslm      (3127)    11357 2023-06-19 13:07:43.000000 unitxt-1.0.0/LICENSE
--rw-rw-r--   0 elron    (605371) tslm      (3127)       33 2023-07-10 12:37:43.000000 unitxt-1.0.0/MANIFEST.in
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2204 2023-07-10 13:08:10.125508 unitxt-1.0.0/PKG-INFO
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1446 2023-07-10 12:46:11.000000 unitxt-1.0.0/README.md
--rw-rw-r--   0 elron    (605371) tslm      (3127)       56 2023-07-10 12:37:46.000000 unitxt-1.0.0/pyproject.toml
--rw-rw-r--   0 elron    (605371) tslm      (3127)       38 2023-07-10 13:08:10.126356 unitxt-1.0.0/setup.cfg
--rw-rw-r--   0 elron    (605371) tslm      (3127)      829 2023-07-10 12:37:52.000000 unitxt-1.0.0/setup.py
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-10 13:08:10.069353 unitxt-1.0.0/src/
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-10 13:08:10.120679 unitxt-1.0.0/src/unitxt/
--rw-rw-r--   0 elron    (605371) tslm      (3127)      164 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/__init__.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     5949 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/artifact.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1141 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/blocks.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      535 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/card.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2670 2023-07-10 12:59:31.000000 unitxt-1.0.0/src/unitxt/catalog.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      946 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/collections.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2933 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/common.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     3034 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/dataset.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/file_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      414 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/fusion.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1686 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/generator_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      656 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/instructions.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      658 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/load.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      668 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/loaders.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     4564 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/metric.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     4244 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/metrics.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      935 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/normalizers.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     8441 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/operator.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     7105 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/operators.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      201 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/processors.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      428 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/recipe.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      487 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/register.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2041 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/schema.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)    11071 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/split_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     3557 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/splitters.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6556 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/stream.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      567 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/task.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6351 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/templates.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6768 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/text_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1401 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/validate.py
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-10 13:08:10.124646 unitxt-1.0.0/src/unitxt.egg-info/
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2204 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/PKG-INFO
--rw-rw-r--   0 elron    (605371) tslm      (3127)      911 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/SOURCES.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)        1 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/dependency_links.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)       66 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/requires.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)        7 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/top_level.txt
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-12 10:40:38.786075 unitxt-1.0.2/
+-rw-rw-r--   0 elron    (605371) tslm      (3127)    11357 2023-07-11 12:24:16.000000 unitxt-1.0.2/LICENSE
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       33 2023-07-11 12:24:16.000000 unitxt-1.0.2/MANIFEST.in
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2242 2023-07-12 10:40:38.785474 unitxt-1.0.2/PKG-INFO
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1810 2023-07-12 07:15:30.000000 unitxt-1.0.2/README.md
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      118 2023-07-12 07:33:22.000000 unitxt-1.0.2/pyproject.toml
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       38 2023-07-12 10:40:38.786188 unitxt-1.0.2/setup.cfg
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      811 2023-07-12 10:40:35.000000 unitxt-1.0.2/setup.py
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-12 10:40:38.695540 unitxt-1.0.2/src/
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-12 10:40:38.777942 unitxt-1.0.2/src/unitxt/
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      129 2023-07-12 10:12:58.000000 unitxt-1.0.2/src/unitxt/__init__.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     5949 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/artifact.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      944 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/blocks.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      535 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/card.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2786 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/catalog.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/collections.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2948 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/common.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2831 2023-07-12 10:02:38.000000 unitxt-1.0.2/src/unitxt/dataset.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/file_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      399 2023-07-12 09:44:41.000000 unitxt-1.0.2/src/unitxt/fusion.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1686 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/generator_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      656 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/instructions.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      659 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/load.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      669 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/loaders.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     4579 2023-07-12 10:10:40.000000 unitxt-1.0.2/src/unitxt/metric.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     4244 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/metrics.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      935 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/normalizers.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     8441 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/operator.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     7075 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/operators.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      201 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/processors.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      428 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/recipe.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1384 2023-07-12 10:15:26.000000 unitxt-1.0.2/src/unitxt/register.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2041 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/schema.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)    11051 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/split_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     3556 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/splitters.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6556 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/stream.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      567 2023-07-12 07:30:16.000000 unitxt-1.0.2/src/unitxt/task.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6351 2023-07-12 07:58:27.000000 unitxt-1.0.2/src/unitxt/templates.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6768 2023-07-11 12:24:16.000000 unitxt-1.0.2/src/unitxt/text_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      246 2023-07-12 09:26:30.000000 unitxt-1.0.2/src/unitxt/utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1327 2023-07-12 09:48:17.000000 unitxt-1.0.2/src/unitxt/validate.py
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-12 10:40:38.784101 unitxt-1.0.2/src/unitxt.egg-info/
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2242 2023-07-12 10:40:38.779922 unitxt-1.0.2/src/unitxt.egg-info/PKG-INFO
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      931 2023-07-12 10:40:38.781000 unitxt-1.0.2/src/unitxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 elron    (605371) tslm      (3127)        1 2023-07-12 10:40:38.781620 unitxt-1.0.2/src/unitxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       66 2023-07-12 10:40:38.783545 unitxt-1.0.2/src/unitxt.egg-info/requires.txt
+-rw-rw-r--   0 elron    (605371) tslm      (3127)        7 2023-07-12 10:40:38.784195 unitxt-1.0.2/src/unitxt.egg-info/top_level.txt
```

### Comparing `unitxt-1.0.0/LICENSE` & `unitxt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.0/PKG-INFO` & `unitxt-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,43 @@
-Metadata-Version: 2.1
-Name: unitxt
-Version: 1.0.0
-Summary: Load any mixture of text to text data in one line of code
-Home-page: https://github.ibm.com/IBM-Research-AI/unitext
-Author: IBM Research
-Author-email: elron.bandel@ibm.com
-License: UNKNOWN
-Description: <div align="center">
-            <img src="./assets/banner.png" alt="Image Description" width="100%" />
-        </div>
-        
-        Unitxt is a python library for getting data fired up and set for utilization.
-        In one line of code, it preps a dataset or mixtures-of-datasets into an input-output format for training and evaluation.
-        We aspire to be simple, adaptable and transperant. 
-        
-        Unitxt builds on separation. Separation allows adding a dataset, without knowing anything about the models using it. Separation allows training without caring for preprocessing, switching models without loading the data differently and changing formats (instruction\ICL\etc.) without changing anything else. 
-        
-        # Installation 🦄
-        
-        Install with git clone:
-        
-        ```bash
-          pip install unitxt
-        ```
-        
-        # Usage 🦄
-        
-        ## Load a dataset
-        
-        ```python
-        from datasets import load_dataset
-        
-        dataset = load_dataset('unitxt/data', 'squad')
-        ```
-        
-        # Why Unitxt? 🦄
-        
-        Unitxt is construct in the light of the principles: (1) Simplicity (2) Adpatability (3) Transperancy
-        ### 🦄 Simplicity
-        Everything is unitxt is simple and designed to feel natural and self explenatory.
-        ### 🦄 Adaptability
-        Adding new datasets, loading recpepies, instructions and formattors is possible and encoureged!
-        ### 🦄 Transperancy
-        The reosurces and formators of Unitxt are stored as shared datasets and therfore can easily reviewed by the crowed. Moreover, when assembling dataset with Unitxt it is very clear to others whats in it. 
-        
-        #
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+<div align="center">
+    <img src="./assets/banner.png" alt="Image Description" width="100%" />
+</div>
+
+Unitxt is a python library for getting data fired up and set for utilization.
+In one line of code, it preps a dataset or mixtures-of-datasets into an input-output format for training and evaluation.
+We aspire to be simple, adaptable and transperant. 
+
+Unitxt builds on separation. Separation allows adding a dataset, without knowing anything about the models using it. Separation allows training without caring for preprocessing, switching models without loading the data differently and changing formats (instruction\ICL\etc.) without changing anything else. 
+
+# 
+[![version](https://img.shields.io/pypi/v/unitxt)](https://pypi.org/project/unitxt/)  ![license](https://img.shields.io/github/license/ibm/unitxt)  ![python](https://img.shields.io/badge/python-3.8%20|%203.9-blue)  ![tests](https://img.shields.io/github/actions/workflow/status/ibm/unitxt/tests.yml?branch=main&label=tests)
+![Read the Docs](https://img.shields.io/readthedocs/unitxt)
+
+
+# Installation 🦄
+
+```bash
+  pip install unitxt
+```
+
+# Usage 🦄
+
+## Load a dataset
+
+```python
+from datasets import load_dataset
+
+dataset = load_dataset('unitxt/data', 'squad')
+```
+
+# Why Unitxt? 🦄
+
+Unitxt is construct in the light of the principles: (1) Simplicity (2) Adpatability (3) Transperancy
+### 🦄 Simplicity
+Everything is unitxt is simple and designed to feel natural and self explenatory.
+### 🦄 Adaptability
+Adding new datasets, loading recpepies, instructions and formattors is possible and encoureged!
+### 🦄 Transperancy
+The reosurces and formators of Unitxt are stored as shared datasets and therfore can easily reviewed by the crowed. Moreover, when assembling dataset with Unitxt it is very clear to others whats in it. 
+
+#
+
```

### Comparing `unitxt-1.0.0/setup.py` & `unitxt-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
     long_description = fh.read()
     
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="unitxt",
-    version="1.0.0",
+    version="1.0.2",
     author="IBM Research",
     author_email="elron.bandel@ibm.com",
     description="Load any mixture of text to text data in one line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.ibm.com/IBM-Research-AI/unitext",
+    url="https://github.com/ibm/unitxt",
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
-    package_data={'unitext': ['catalog/*.json']},
+    package_data={'unitxt': ['catalog/*.json']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     install_requires=requirements,
 )
```

### Comparing `unitxt-1.0.0/src/unitxt/artifact.py` & `unitxt-1.0.2/src/unitxt/artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from dataclasses import dataclass, asdict, fields, field
-from abc import ABC, abstractmethod
-from typing import final
-import re
+import inspect
 import json
 import os
 import pkgutil
-import inspect
+import re
+from abc import ABC, abstractmethod
+from dataclasses import asdict, dataclass, field, fields
+from typing import final
 
 
 class AbstractField:
     pass
 
 
 from .text_utils import camel_to_snake_case, is_camel_case
```

### Comparing `unitxt-1.0.0/src/unitxt/card.py` & `unitxt-1.0.2/src/unitxt/card.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from typing import List, Optional, Union
+
 from .artifact import Artifact
-from .operator import StreamingOperator
-from .templates import TemplatesList, TemplatesDict
-from .instructions import InstructionsList, InstructionsDict
+from .instructions import InstructionsDict, InstructionsList
 from .loaders import Loader
+from .operator import StreamingOperator
 from .task import FormTask
-
-from typing import Union, List, Optional
+from .templates import TemplatesDict, TemplatesList
 
 
 class TaskCard(Artifact):
     loader: Loader
     task: FormTask
     preprocess_steps: Optional[List[StreamingOperator]] = None
     templates: Union[TemplatesList, TemplatesDict] = None
```

### Comparing `unitxt-1.0.0/src/unitxt/catalog.py` & `unitxt-1.0.2/src/unitxt/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+import os
+
 from .artifact import Artifact, Artifactory, register_atrifactory
 from .file_utils import get_all_files_in_dir
 
-import os
 
 class Catalog(Artifactory):
     name: str = None
     location: str = None
 
-catalog_path = os.path.dirname(__file__) + "/catalog"
+
+try:
+    import unitxt
+
+    catalog_path = os.path.dirname(unitxt.__file__) + "/catalog"
+except ImportError:
+    catalog_path = os.path.dirname(__file__) + "/catalog"
+
 
 class LocalCatalog(Catalog):
     name: str = "local"
     location: str = catalog_path
 
     @property
     def path_dict(self):
```

### Comparing `unitxt-1.0.0/src/unitxt/collections.py` & `unitxt-1.0.2/src/unitxt/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from .artifact import Artifact
-
+import random
 from abc import abstractmethod
-
 from dataclasses import field
-import random
+
+from .artifact import Artifact
 
 
 class Collection(Artifact):
     @abstractmethod
     def __getitem__(self, key):
         pass
```

### Comparing `unitxt-1.0.0/src/unitxt/common.py` & `unitxt-1.0.2/src/unitxt/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from .stream import MultiStream
-from .operator import SourceOperator
+from typing import Union
+
 from .card import TaskCard
-from .splitters import SliceSplit, SpreadSplit, RandomSampler
-from .recipe import SequentialRecipe, Recipe
 from .collections import ItemPicker, RandomPicker
-from .templates import RenderTemplatedICL
+from .operator import SourceOperator
+from .recipe import Recipe, SequentialRecipe
 from .schema import ToUnitxtGroup
-
-from typing import Union
+from .splitters import RandomSampler, SliceSplit, SpreadSplit
+from .stream import MultiStream
+from .templates import RenderTemplatedICL
 
 
 class CommonRecipe(Recipe, SourceOperator):
     card: TaskCard
     demos_pool_name: str = "demos_pool"
     demos_pool_size: int = None
     demos_field: str = "demos"
@@ -33,25 +33,25 @@
 
         steps.append(self.card.task)
 
         if self.demos_pool_size is not None:
             steps.append(
                 SliceSplit(
                     slices={
-                        self.demos_pool_name: f"train[:{self.demos_pool_size}]",
-                        "train": f"train[{self.demos_pool_size}:]",
+                        self.demos_pool_name: f"train[:{int(self.demos_pool_size)}]",
+                        "train": f"train[{int(self.demos_pool_size)}:]",
                         "validation": "validation",
                         "test": "test",
                     }
                 )
             )
 
         if self.num_demos is not None:
             if self.sampler_type == "random":
-                sampler = RandomSampler(sample_size=self.num_demos)
+                sampler = RandomSampler(sample_size=int(self.num_demos))
 
             steps.append(
                 SpreadSplit(
                     source_stream=self.demos_pool_name,
                     target_field=self.demos_field,
                     sampler=sampler,
                 )
```

### Comparing `unitxt-1.0.0/src/unitxt/dataset.py` & `unitxt-1.0.2/src/unitxt/dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,49 @@
-###############
-# `ls -1 src/unitxt | grep '\.py$' | grep -Ev 'dataset\.py|__init__\.py' | sort`:
-# artifact.py
-# blocks.py
-# card.py
-# catalog.py
-# collections.py
-# common.py
-# file_utils.py
-# fusion.py
-# generator_utils.py
-# instructions.py
-# loaders.py
-# load.py
-# metric.py
-# metrics.py
-# normalizers.py
-# operator.py
-# operators.py
-# processors.py
-# recipe.py
-# register.py
-# splitters.py
-# split_utils.py
-# stream.py
-# task.py
-# templates.py
-# text_utils.py
-# utilize.py
-# validate.py
-#####
-# imports for hf system:
-#####
+import datasets
+
+from .artifact import Artifact, UnitxtArtifactNotFoundError
 from .artifact import __file__ as _
+from .artifact import fetch_artifact
 from .blocks import __file__ as _
 from .card import __file__ as _
 from .catalog import __file__ as _
 from .collections import __file__ as _
 from .common import __file__ as _
 from .file_utils import __file__ as _
-
-# from .fusion import __file__
+from .fusion import __file__ as _
 from .generator_utils import __file__ as _
 from .instructions import __file__ as _
-from .loaders import __file__ as _
 from .load import __file__ as _
+from .loaders import __file__ as _
 from .metric import __file__ as _
 from .metrics import __file__ as _
 from .normalizers import __file__ as _
 from .operator import __file__ as _
 from .operators import __file__ as _
 from .processors import __file__ as _
 from .recipe import __file__ as _
 from .register import __file__ as _
+from .register import register_all_artifacts
 from .schema import __file__ as _
-from .splitters import __file__ as _
 from .split_utils import __file__ as _
+from .splitters import __file__ as _
 from .stream import __file__ as _
 from .task import __file__ as _
 from .templates import __file__ as _
 from .text_utils import __file__ as _
+from .utils import __file__ as _
+from .validate import __file__ as _
 
-# from .utilize import __file__ as _
-# from .validate import __file__ as _
-#############
 
-from .register import register_blocks
-from .artifact import Artifact
-
-import datasets
+def fetch(artifact_name):
+    try:
+        artifact, _ = fetch_artifact(artifact_name)
+        return artifact
+    except UnitxtArtifactNotFoundError:
+        return None
 
 
 def parse(query: str):
     """
     Parses a query of the form 'key1=value1,key2=value2,...' into a dictionary.
     """
     result = {}
@@ -83,28 +55,30 @@
             result[parts[0]] = float(parts[1])
 
         result[parts[0]] = parts[1]
 
     return result
 
 
-class Unitext(datasets.GeneratorBasedBuilder):
+class Dataset(datasets.GeneratorBasedBuilder):
     """TODO: Short description of my dataset."""
 
     VERSION = datasets.Version("1.1.1")
     builder_configs = {}
 
     @property
     def generators(self):
-        register_blocks()
+        register_all_artifacts()
         if not hasattr(self, "_generators") or self._generators is None:
-            args = parse(self.config.name)
-            if "type" not in args:
-                args["type"] = "common_recipe"
-            recipe = Artifact.from_dict(args)
+            recipe = fetch(self.config.name)
+            if recipe is None:
+                args = parse(self.config.name)
+                if "type" not in args:
+                    args["type"] = "common_recipe"
+                recipe = Artifact.from_dict(args)
             self._generators = recipe()
         return self._generators
 
     def _info(self):
         return datasets.DatasetInfo()
 
     def _split_generators(self, _):
```

### Comparing `unitxt-1.0.0/src/unitxt/file_utils.py` & `unitxt-1.0.2/src/unitxt/file_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.0/src/unitxt/generator_utils.py` & `unitxt-1.0.2/src/unitxt/generator_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.0/src/unitxt/instructions.py` & `unitxt-1.0.2/src/unitxt/instructions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .artifact import Artifact
-
 from abc import ABC, abstractmethod
 from typing import Dict
 
+from .artifact import Artifact
+
 
 class Instruction(Artifact):
     @abstractmethod
     def __call__(self) -> str:
         pass
```

### Comparing `unitxt-1.0.0/src/unitxt/load.py` & `unitxt-1.0.2/src/unitxt/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from .operator import StreamSource
-from datasets import DatasetDict
 from typing import Union
 
-from .catalog import LocalCatalog
+from datasets import DatasetDict
+
 from .artifact import Artifact
+from .catalog import LocalCatalog
+from .operator import StreamSource
 
 
 def load_stream(source_name_or_path: str) -> StreamSource:
     if Artifact.is_artifact_file(source_name_or_path):
         return Artifact.load(source_name_or_path)
     else:
         return LocalCatalog().load(source_name_or_path)
```

### Comparing `unitxt-1.0.0/src/unitxt/loaders.py` & `unitxt-1.0.2/src/unitxt/loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from .stream import MultiStream
-from .operator import SourceOperator
+from typing import Mapping, Optional, Sequence, Union
 
-from typing import Optional, Union, Sequence, Mapping
 from datasets import load_dataset as hf_load_dataset
 
+from .operator import SourceOperator
+from .stream import MultiStream
+
 
 class Loader(SourceOperator):
     pass
 
 
 class LoadHF(Loader):
     path: str
```

### Comparing `unitxt-1.0.0/src/unitxt/metric.py` & `unitxt-1.0.2/src/unitxt/metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,57 @@
-#####
-# imports for hf system:
-#####
+from dataclasses import field
+from typing import Any, Dict, Generator, Iterable, List, Optional, Union
+
+import datasets
+import evaluate
+from datasets import Features, Sequence, Value
+
 from .artifact import __file__ as _
 from .blocks import __file__ as _
 from .card import __file__ as _
 from .catalog import __file__ as _
 from .collections import __file__ as _
 from .common import __file__ as _
 from .file_utils import __file__ as _
-
-# from .fusion import __file__
+from .fusion import __file__ as _
 from .generator_utils import __file__ as _
 from .instructions import __file__ as _
-from .loaders import __file__ as _
 from .load import __file__ as _
+from .loaders import __file__ as _
 from .metrics import __file__ as _
 from .normalizers import __file__ as _
+from .operator import (
+    MultiStreamOperator,
+    SequntialOperator,
+    SequntialOperatorInitilizer,
+    StreamInitializerOperator,
+)
 from .operator import __file__ as _
+from .operators import (
+    ApplyStreamOperatorsField,
+    ApplyValueOperatorsField,
+    FlattenInstances,
+    MergeStreams,
+    SplitByValue,
+)
 from .operators import __file__ as _
 from .processors import __file__ as _
 from .recipe import __file__ as _
 from .register import __file__ as _
-from .splitters import __file__ as _
+from .register import register_all_artifacts
+from .schema import __file__ as _
 from .split_utils import __file__ as _
+from .splitters import __file__ as _
+from .stream import MultiStream, Stream
 from .stream import __file__ as _
 from .task import __file__ as _
 from .templates import __file__ as _
 from .text_utils import __file__ as _
-from .schema import __file__ as _
-
-# from .utilize import __file__ as _
-# from .validate import __file__ as _
-#############
-
-from .stream import MultiStream, Stream
-
-from .operator import SequntialOperator, SequntialOperatorInitilizer, MultiStreamOperator, StreamInitializerOperator
-
-from .operators import (
-    ApplyValueOperatorsField,
-    ApplyStreamOperatorsField,
-    SplitByValue,
-    MergeStreams,
-    FlattenInstances,
-)
-
-import evaluate
-import datasets
-
-from datasets import (
-    Features,
-    Value,
-    Sequence,
-)
-
-from dataclasses import field
-from typing import List, Union, Dict, Optional, Generator, Any, Iterable
+from .utils import __file__ as _
+from .validate import __file__ as _
 
 
 class MultiStreamScoreMean(MultiStreamOperator):
     def aggegate_results(self, multi_stream: MultiStream):
         scores = []
         for stream in multi_stream.values():
             instance = stream.peak()
@@ -96,14 +88,15 @@
 
 
 from .schema import UNITXT_DATASET_SCHEMA
 
 
 class MetricRecipe(SequntialOperatorInitilizer):
     def prepare(self):
+        register_all_artifacts()
         self.steps = [
             FromPredictionsAndOriginalData(),
             ApplyValueOperatorsField(
                 value_field="prediction", operators_field="processors", default_operators=["to_string"]
             ),
             SplitByValue(["group"]),
             ApplyStreamOperatorsField(
@@ -115,15 +108,15 @@
         ]
 
 
 UNITXT_METRIC_SCHEMA = Features({"predictions": Value("string"), "references": dict(UNITXT_DATASET_SCHEMA)})
 
 
 # @evaluate.utils.file_utils.add_start_docstrings(_DESCRIPTION, _KWARGS_DESCRIPTION)
-class UnitextMetric(evaluate.Metric):
+class Metric(evaluate.Metric):
     def _info(self):
         return evaluate.MetricInfo(
             description="_DESCRIPTION",
             citation="_CITATION",
             # inputs_description=_KWARGS_DESCRIPTION,
             features=UNITXT_METRIC_SCHEMA,
             codebase_urls=["https://"],
```

### Comparing `unitxt-1.0.0/src/unitxt/metrics.py` & `unitxt-1.0.2/src/unitxt/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from .stream import Stream
-from .operator import SingleStreamOperator, StreamInstanceOperator
+from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from abc import abstractmethod, ABC
+from typing import Any, Dict, List
 
-from typing import List, Dict, Any
+from .operator import SingleStreamOperator, StreamInstanceOperator
+from .stream import Stream
 
 
 def absrtact_factory():
     return {}
 
 
 def abstract_field():
```

### Comparing `unitxt-1.0.0/src/unitxt/operator.py` & `unitxt-1.0.2/src/unitxt/operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from .stream import MultiStream, Stream
-from .artifact import Artifact
-
 from abc import abstractmethod
-from typing import Optional, List, Dict, Generator, Union, Any
 from dataclasses import field
+from typing import Any, Dict, Generator, List, Optional, Union
+
+from .artifact import Artifact
+from .stream import MultiStream, Stream
 
 
 class Operator(Artifact):
     pass
 
 
 class OperatorError(Exception):
```

### Comparing `unitxt-1.0.0/src/unitxt/operators.py` & `unitxt-1.0.2/src/unitxt/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from .stream import MultiStream, Stream
+from dataclasses import field
+from typing import Any, Dict, Generator, Iterable, List, Optional, Union
+
 from .artifact import Artifact, fetch_artifact
 from .operator import (
-    StreamInstanceOperator,
+    MultiStream,
     MultiStreamOperator,
     SingleStreamOperator,
     SingleStreamReducer,
-    StreamInitializerOperator,
     Stream,
-    MultiStream,
+    StreamInitializerOperator,
+    StreamInstanceOperator,
 )
-
-from dataclasses import field
-from typing import List, Union, Dict, Optional, Generator, Any, Iterable
-
-from typing import Dict, Any
+from .stream import MultiStream, Stream
 
 
 class FromIterables(StreamInitializerOperator):
     def process(self, iterables: Dict[str, Iterable]) -> MultiStream:
         return MultiStream.from_iterables(iterables)
```

### Comparing `unitxt-1.0.0/src/unitxt/schema.py` & `unitxt-1.0.2/src/unitxt/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from datasets import Features, Sequence, Value
-from .operator import StreamInstanceOperatorValidator
+from dataclasses import field
+from typing import Any, Dict, List
 
-from typing import Dict, Any, List
+from datasets import Features, Sequence, Value
 
-from dataclasses import field
+from .operator import StreamInstanceOperatorValidator
 
 UNITXT_DATASET_SCHEMA = Features(
     {
         "source": Value("string"),
         "target": Value("string"),
         "references": Sequence(Value("string")),
         "metrics": Sequence(Value("string")),
```

### Comparing `unitxt-1.0.0/src/unitxt/split_utils.py` & `unitxt-1.0.2/src/unitxt/split_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import re
-import random
 import itertools
+import random
+import re
 
 from .generator_utils import ReusableGenerator
 
 
 def parse_random_mix_string(input_str):
     """
     Parses a string of format "source1[percentage1%]+source2[value2]+..." and returns a dictionary.
@@ -22,15 +22,15 @@
     Raises:
         ValueError: If the input string is not in the correct format.
 
     Example:
         >>> parse_random_mix_string("dale[90%]+oren[0.7]+mike")
             {'dale': 0.9, 'oren': 0.7, 'mike': 1.0}
     """
-    
+
     if not re.fullmatch(r"(([a-zA-Z]+\[\d*\.?\d*%?\]|[a-zA-Z]+)\+)*([a-zA-Z]+\[\d*\.?\d*%?\]|[a-zA-Z]+)", input_str):
         raise ValueError("Invalid input format")
 
     pattern = re.compile(r"([a-zA-Z]+)(\[\d*\.?\d*%?\])?")
     matches = pattern.findall(input_str)
 
     return {
@@ -59,15 +59,15 @@
     Raises:
         ValueError: If the input string is not in the correct format.
 
     Example:
         >>> parse_slices_string("oren[:50]+jake[24:]+test+oren[5:10]")
         {'oren': [(None, 50), (5, 10)], 'jake': [(24, None)], 'test': [(None, None)]}
     """
-    
+
     result_dict = {}
 
     # Split the input string into a list of sources
     sources = re.split("\+", input_str)
     for source in sources:
         # If the source has a slice, parse it
         match = re.fullmatch(r"(\w+)\[(\d*):(\d*)\]", source)
@@ -123,15 +123,15 @@
 
     Example:
         >>> old_streams = {"train": [1, 2, 3, 4, 5, 6, 7, 8, 9], "test": [10, 11, 12, 13, 14]}
         >>> mapping = {"new_train": {"train": [(None, 5), (7, 9)]}, "new_test": {"test": [(2, None)]}}
         >>> slice_streams(old_streams, mapping)
         {"new_train": [1, 2, 3, 4, 5, 8, 9], "new_test": [12, 13, 14]}
     """
-    
+
     new_streams = {}
     for new_stream, sources in mapping.items():
 
         def generator(new_stream, sources):
             for old_stream, slices in sources.items():
                 old_stream_content = input_streams[old_stream]
                 for start, end in slices:
@@ -174,15 +174,15 @@
                 }
             }
             stream_mapping = build_stream_mapping(mapping)
             print(stream_mapping)
             # Output: {'my_old_stream1': (['my_new_stream', 'my_new_stream2'], [0.6, 0.4]),
             #          'my_old_stream2': (['my_new_stream', 'my_new_stream2'], [0.2, 0.8])}
     """
-    
+
     stream_mapping = {}
 
     # Calculate total weight for each old stream
     total_weights = {}
     for new_stream, old_streams in mapping.items():
         for old_stream, weight in old_streams.items():
             if old_stream not in total_weights:
@@ -253,15 +253,15 @@
             }
             new_streams = create_streams(input_streams, mapping)
             for new_stream_name, new_stream in new_streams.items():
                 print(f"{new_stream_name}:")
                 for _, item in zip(range(10), new_stream):
                     print(item)
     """
-    
+
     new_streams = {}
 
     # Build stream routing
     stream_routing = build_stream_routing(mapping)
 
     rand = random.Random()
```

### Comparing `unitxt-1.0.0/src/unitxt/splitters.py` & `unitxt-1.0.2/src/unitxt/splitters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from .stream import MultiStream
-from .operator import MultiStreamOperator, InstanceOperatorWithGlobalAccess
-from .generator_utils import ReusableGenerator
-from .artifact import Artifact
-
-
-from typing import Optional, Dict, List
 from dataclasses import field
+from typing import Dict, List, Optional
+
+from .artifact import Artifact
+from .generator_utils import ReusableGenerator
+from .operator import InstanceOperatorWithGlobalAccess, MultiStreamOperator
+from .stream import MultiStream
 
 
 class Splitter(MultiStreamOperator):
     pass
 
 
 import random
 
 from .split_utils import (
     parse_random_mix_string,
-    random_mix_streams,
     parse_slices_string,
+    random_mix_streams,
     slice_streams,
 )
 
 
 class SplitRandomMix(Splitter):
     mix: Dict[str, str]
```

### Comparing `unitxt-1.0.0/src/unitxt/stream.py` & `unitxt-1.0.2/src/unitxt/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .generator_utils import ReusableGenerator
+from typing import Dict, Iterable
 
-from typing import Iterable, Dict
+from datasets import Dataset, DatasetDict, IterableDataset, IterableDatasetDict
 
-from datasets import IterableDatasetDict, IterableDataset, DatasetDict, Dataset
+from .generator_utils import ReusableGenerator
 
 
 class Stream:
     """A class for handling streaming data in a customizable way.
 
     This class provides methods for generating, caching, and manipulating streaming data.
```

### Comparing `unitxt-1.0.0/src/unitxt/task.py` & `unitxt-1.0.2/src/unitxt/task.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .operator import StreamInstanceOperator
+from typing import Any, Dict, List
 
-from typing import Dict, List, Any
+from .operator import StreamInstanceOperator
 
 
 class Tasker:
     pass
 
 
 class FormTask(Tasker, StreamInstanceOperator):
```

### Comparing `unitxt-1.0.0/src/unitxt/templates.py` & `unitxt-1.0.2/src/unitxt/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from .text_utils import split_words
-from .artifact import Artifact
-from .operator import StreamInstanceOperator, InstanceOperatorWithGlobalAccess
-from .instructions import Instruction
-
 import random
-from typing import Dict, Any, List
 from abc import ABC, abstractmethod
+from typing import Any, Dict, List
+
+from .artifact import Artifact
+from .instructions import Instruction
+from .operator import InstanceOperatorWithGlobalAccess, StreamInstanceOperator
+from .text_utils import split_words
 
 
 class Renderer(ABC):
     @abstractmethod
     def get_postprocessors(self) -> List[str]:
         pass
```

### Comparing `unitxt-1.0.0/src/unitxt/text_utils.py` & `unitxt-1.0.2/src/unitxt/text_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.0/src/unitxt.egg-info/PKG-INFO` & `unitxt-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.0.0
+Version: 1.0.2
 Summary: Load any mixture of text to text data in one line of code
-Home-page: https://github.ibm.com/IBM-Research-AI/unitext
+Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 License: UNKNOWN
-Description: <div align="center">
-            <img src="./assets/banner.png" alt="Image Description" width="100%" />
-        </div>
-        
-        Unitxt is a python library for getting data fired up and set for utilization.
-        In one line of code, it preps a dataset or mixtures-of-datasets into an input-output format for training and evaluation.
-        We aspire to be simple, adaptable and transperant. 
-        
-        Unitxt builds on separation. Separation allows adding a dataset, without knowing anything about the models using it. Separation allows training without caring for preprocessing, switching models without loading the data differently and changing formats (instruction\ICL\etc.) without changing anything else. 
-        
-        # Installation 🦄
-        
-        Install with git clone:
-        
-        ```bash
-          pip install unitxt
-        ```
-        
-        # Usage 🦄
-        
-        ## Load a dataset
-        
-        ```python
-        from datasets import load_dataset
-        
-        dataset = load_dataset('unitxt/data', 'squad')
-        ```
-        
-        # Why Unitxt? 🦄
-        
-        Unitxt is construct in the light of the principles: (1) Simplicity (2) Adpatability (3) Transperancy
-        ### 🦄 Simplicity
-        Everything is unitxt is simple and designed to feel natural and self explenatory.
-        ### 🦄 Adaptability
-        Adding new datasets, loading recpepies, instructions and formattors is possible and encoureged!
-        ### 🦄 Transperancy
-        The reosurces and formators of Unitxt are stored as shared datasets and therfore can easily reviewed by the crowed. Moreover, when assembling dataset with Unitxt it is very clear to others whats in it. 
-        
-        #
-        
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+    <img src="./assets/banner.png" alt="Image Description" width="100%" />
+</div>
+
+Unitxt is a python library for getting data fired up and set for utilization.
+In one line of code, it preps a dataset or mixtures-of-datasets into an input-output format for training and evaluation.
+We aspire to be simple, adaptable and transperant. 
+
+Unitxt builds on separation. Separation allows adding a dataset, without knowing anything about the models using it. Separation allows training without caring for preprocessing, switching models without loading the data differently and changing formats (instruction\ICL\etc.) without changing anything else. 
+
+# 
+[![version](https://img.shields.io/pypi/v/unitxt)](https://pypi.org/project/unitxt/)  ![license](https://img.shields.io/github/license/ibm/unitxt)  ![python](https://img.shields.io/badge/python-3.8%20|%203.9-blue)  ![tests](https://img.shields.io/github/actions/workflow/status/ibm/unitxt/tests.yml?branch=main&label=tests)
+![Read the Docs](https://img.shields.io/readthedocs/unitxt)
+
+
+# Installation 🦄
+
+```bash
+  pip install unitxt
+```
+
+# Usage 🦄
+
+## Load a dataset
+
+```python
+from datasets import load_dataset
+
+dataset = load_dataset('unitxt/data', 'squad')
+```
+
+# Why Unitxt? 🦄
+
+Unitxt is construct in the light of the principles: (1) Simplicity (2) Adpatability (3) Transperancy
+### 🦄 Simplicity
+Everything is unitxt is simple and designed to feel natural and self explenatory.
+### 🦄 Adaptability
+Adding new datasets, loading recpepies, instructions and formattors is possible and encoureged!
+### 🦄 Transperancy
+The reosurces and formators of Unitxt are stored as shared datasets and therfore can easily reviewed by the crowed. Moreover, when assembling dataset with Unitxt it is very clear to others whats in it. 
+
+#
+
+
+
```

### Comparing `unitxt-1.0.0/src/unitxt.egg-info/SOURCES.txt` & `unitxt-1.0.2/src/unitxt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,13 +28,14 @@
 src/unitxt/schema.py
 src/unitxt/split_utils.py
 src/unitxt/splitters.py
 src/unitxt/stream.py
 src/unitxt/task.py
 src/unitxt/templates.py
 src/unitxt/text_utils.py
+src/unitxt/utils.py
 src/unitxt/validate.py
 src/unitxt.egg-info/PKG-INFO
 src/unitxt.egg-info/SOURCES.txt
 src/unitxt.egg-info/dependency_links.txt
 src/unitxt.egg-info/requires.txt
 src/unitxt.egg-info/top_level.txt
```

