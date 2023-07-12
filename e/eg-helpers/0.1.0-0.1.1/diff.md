# Comparing `tmp/eg_helpers-0.1.0.tar.gz` & `tmp/eg_helpers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eg_helpers-0.1.0.tar", last modified: Wed Jul 12 15:41:41 2023, max compression
+gzip compressed data, was "eg_helpers-0.1.1.tar", last modified: Wed Jul 12 16:08:10 2023, max compression
```

## Comparing `eg_helpers-0.1.0.tar` & `eg_helpers-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:41:41.543037 eg_helpers-0.1.0/
--rw-rw-rw-   0        0        0      235 2023-07-12 15:41:41.543037 eg_helpers-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 15:41:41.537536 eg_helpers-0.1.0/eg_helpers/
--rw-rw-rw-   0        0        0        0 2023-06-16 21:42:46.000000 eg_helpers-0.1.0/eg_helpers/__init__.py
--rw-rw-rw-   0        0        0    22786 2023-07-12 14:57:48.000000 eg_helpers-0.1.0/eg_helpers/utils_debug.py
--rw-rw-rw-   0        0        0    58427 2023-07-12 14:57:56.000000 eg_helpers-0.1.0/eg_helpers/utils_debug_ascii_art.py
--rw-rw-rw-   0        0        0      611 2023-07-12 14:46:38.000000 eg_helpers-0.1.0/eg_helpers/utils_openai.py
--rw-rw-rw-   0        0        0     7806 2023-07-12 14:47:05.000000 eg_helpers-0.1.0/eg_helpers/utils_time.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:41:41.542534 eg_helpers-0.1.0/eg_helpers.egg-info/
--rw-rw-rw-   0        0        0      235 2023-07-12 15:41:41.000000 eg_helpers-0.1.0/eg_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-12 15:41:41.000000 eg_helpers-0.1.0/eg_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:41:41.000000 eg_helpers-0.1.0/eg_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-12 15:41:41.000000 eg_helpers-0.1.0/eg_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-12 15:41:41.000000 eg_helpers-0.1.0/eg_helpers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:41:41.544040 eg_helpers-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      469 2023-07-12 15:32:32.000000 eg_helpers-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:08:10.865938 eg_helpers-0.1.1/
+-rw-rw-rw-   0        0        0      235 2023-07-12 16:08:10.865938 eg_helpers-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 16:08:10.858432 eg_helpers-0.1.1/eg_helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-16 21:42:46.000000 eg_helpers-0.1.1/eg_helpers/__init__.py
+-rw-rw-rw-   0        0        0    22775 2023-07-12 16:07:28.000000 eg_helpers-0.1.1/eg_helpers/utils_debug.py
+-rw-rw-rw-   0        0        0    58427 2023-07-12 14:57:56.000000 eg_helpers-0.1.1/eg_helpers/utils_debug_ascii_art.py
+-rw-rw-rw-   0        0        0      611 2023-07-12 14:46:38.000000 eg_helpers-0.1.1/eg_helpers/utils_openai.py
+-rw-rw-rw-   0        0        0     7806 2023-07-12 14:47:05.000000 eg_helpers-0.1.1/eg_helpers/utils_time.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:08:10.864936 eg_helpers-0.1.1/eg_helpers.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:08:10.865938 eg_helpers-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      469 2023-07-12 16:06:04.000000 eg_helpers-0.1.1/setup.py
```

### Comparing `eg_helpers-0.1.0/eg_helpers/utils_debug.py` & `eg_helpers-0.1.1/eg_helpers/utils_debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,18 @@
 except UserError as e:
     print(f"UserError: {e}")
 """
 
 import tempfile 
 import shutil
 import datetime
-import sys
 import os
 import re
 import pandas as pd
-from utils_debug_ascii_art import get_random_art
+from .utils_debug_ascii_art import get_random_art
 
 
 ### this part is for internal troubleshooting / logging ... absurd, i know.. ###
 
 import logging
 import os
```

### Comparing `eg_helpers-0.1.0/eg_helpers/utils_debug_ascii_art.py` & `eg_helpers-0.1.1/eg_helpers/utils_debug_ascii_art.py`

 * *Files identical despite different names*

### Comparing `eg_helpers-0.1.0/eg_helpers/utils_openai.py` & `eg_helpers-0.1.1/eg_helpers/utils_openai.py`

 * *Files identical despite different names*

### Comparing `eg_helpers-0.1.0/eg_helpers/utils_time.py` & `eg_helpers-0.1.1/eg_helpers/utils_time.py`

 * *Files identical despite different names*

