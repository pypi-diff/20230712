# Comparing `tmp/eg_helpers-0.1.1.tar.gz` & `tmp/eg_helpers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eg_helpers-0.1.1.tar", last modified: Wed Jul 12 16:08:10 2023, max compression
+gzip compressed data, was "eg_helpers-0.1.2.tar", last modified: Wed Jul 12 16:17:27 2023, max compression
```

## Comparing `eg_helpers-0.1.1.tar` & `eg_helpers-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 16:08:10.865938 eg_helpers-0.1.1/
--rw-rw-rw-   0        0        0      235 2023-07-12 16:08:10.865938 eg_helpers-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 16:08:10.858432 eg_helpers-0.1.1/eg_helpers/
--rw-rw-rw-   0        0        0        0 2023-06-16 21:42:46.000000 eg_helpers-0.1.1/eg_helpers/__init__.py
--rw-rw-rw-   0        0        0    22775 2023-07-12 16:07:28.000000 eg_helpers-0.1.1/eg_helpers/utils_debug.py
--rw-rw-rw-   0        0        0    58427 2023-07-12 14:57:56.000000 eg_helpers-0.1.1/eg_helpers/utils_debug_ascii_art.py
--rw-rw-rw-   0        0        0      611 2023-07-12 14:46:38.000000 eg_helpers-0.1.1/eg_helpers/utils_openai.py
--rw-rw-rw-   0        0        0     7806 2023-07-12 14:47:05.000000 eg_helpers-0.1.1/eg_helpers/utils_time.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:08:10.864936 eg_helpers-0.1.1/eg_helpers.egg-info/
--rw-rw-rw-   0        0        0      235 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-12 16:08:10.000000 eg_helpers-0.1.1/eg_helpers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 16:08:10.865938 eg_helpers-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      469 2023-07-12 16:06:04.000000 eg_helpers-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:17:27.830079 eg_helpers-0.1.2/
+-rw-rw-rw-   0        0        0      235 2023-07-12 16:17:27.829079 eg_helpers-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 16:17:27.824079 eg_helpers-0.1.2/eg_helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-16 21:42:46.000000 eg_helpers-0.1.2/eg_helpers/__init__.py
+-rw-rw-rw-   0        0        0    22775 2023-07-12 16:07:28.000000 eg_helpers-0.1.2/eg_helpers/utils_debug.py
+-rw-rw-rw-   0        0        0    58427 2023-07-12 14:57:56.000000 eg_helpers-0.1.2/eg_helpers/utils_debug_ascii_art.py
+-rw-rw-rw-   0        0        0      611 2023-07-12 14:46:38.000000 eg_helpers-0.1.2/eg_helpers/utils_openai.py
+-rw-rw-rw-   0        0        0     7807 2023-07-12 16:15:16.000000 eg_helpers-0.1.2/eg_helpers/utils_time.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:17:27.828079 eg_helpers-0.1.2/eg_helpers.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-07-12 16:17:27.000000 eg_helpers-0.1.2/eg_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-12 16:17:27.000000 eg_helpers-0.1.2/eg_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:17:27.000000 eg_helpers-0.1.2/eg_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-12 16:17:27.000000 eg_helpers-0.1.2/eg_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-12 16:17:27.000000 eg_helpers-0.1.2/eg_helpers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:17:27.830079 eg_helpers-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      469 2023-07-12 16:17:13.000000 eg_helpers-0.1.2/setup.py
```

### Comparing `eg_helpers-0.1.1/eg_helpers/utils_debug.py` & `eg_helpers-0.1.2/eg_helpers/utils_debug.py`

 * *Files identical despite different names*

### Comparing `eg_helpers-0.1.1/eg_helpers/utils_debug_ascii_art.py` & `eg_helpers-0.1.2/eg_helpers/utils_debug_ascii_art.py`

 * *Files identical despite different names*

### Comparing `eg_helpers-0.1.1/eg_helpers/utils_openai.py` & `eg_helpers-0.1.2/eg_helpers/utils_openai.py`

 * *Files identical despite different names*

### Comparing `eg_helpers-0.1.1/eg_helpers/utils_time.py` & `eg_helpers-0.1.2/eg_helpers/utils_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #File: utils_time.py
 import datetime
-from utils_debug import debugging_prints
+from .utils_debug import debugging_prints
 import pytz
 import regex as re
 
 debug_level = 2
 
 def dprint(msg, level=2, log_timestamps=True, *args):
     debugging_prints(msg, level, debug_level, log_timestamps, *args)
```

