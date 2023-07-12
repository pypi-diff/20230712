# Comparing `tmp/afgutils-1.0.7.tar.gz` & `tmp/afgutils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afgutils-1.0.7.tar", last modified: Mon Jul  3 20:34:10 2023, max compression
+gzip compressed data, was "afgutils-1.0.8.tar", last modified: Wed Jul 12 18:01:46 2023, max compression
```

## Comparing `afgutils-1.0.7.tar` & `afgutils-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 20:34:10.786712 afgutils-1.0.7/
--rw-rw-rw-   0        0        0      224 2023-07-03 20:34:10.785710 afgutils-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 20:34:10.764711 afgutils-1.0.7/afgutils/
--rw-rw-rw-   0        0        0      264 2023-04-13 10:38:48.000000 afgutils-1.0.7/afgutils/__init__.py
--rw-rw-rw-   0        0        0      882 2023-05-04 15:08:56.000000 afgutils-1.0.7/afgutils/advanceai_util.py
--rw-rw-rw-   0        0        0     2634 2023-04-13 11:41:11.000000 afgutils-1.0.7/afgutils/credolab.py
--rw-rw-rw-   0        0        0     2950 2023-04-06 17:38:51.000000 afgutils-1.0.7/afgutils/db.py
--rw-rw-rw-   0        0        0      757 2023-04-06 17:33:13.000000 afgutils-1.0.7/afgutils/email.py
--rw-rw-rw-   0        0        0     1677 2023-04-13 11:41:11.000000 afgutils-1.0.7/afgutils/s3.py
--rw-rw-rw-   0        0        0     3903 2023-04-06 17:33:13.000000 afgutils-1.0.7/afgutils/trandata.py
--rw-rw-rw-   0        0        0     4200 2023-07-03 20:31:04.000000 afgutils-1.0.7/afgutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:34:10.784711 afgutils-1.0.7/afgutils.egg-info/
--rw-rw-rw-   0        0        0      224 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 20:34:10.786712 afgutils-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      633 2023-07-03 20:33:44.000000 afgutils-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:01:46.972493 afgutils-1.0.8/
+-rw-rw-rw-   0        0        0      224 2023-07-12 18:01:46.971493 afgutils-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 18:01:46.943494 afgutils-1.0.8/afgutils/
+-rw-rw-rw-   0        0        0      264 2023-04-13 10:38:48.000000 afgutils-1.0.8/afgutils/__init__.py
+-rw-rw-rw-   0        0        0      882 2023-05-04 15:08:56.000000 afgutils-1.0.8/afgutils/advanceai_util.py
+-rw-rw-rw-   0        0        0     2634 2023-04-13 11:41:11.000000 afgutils-1.0.8/afgutils/credolab.py
+-rw-rw-rw-   0        0        0     2950 2023-04-06 17:38:51.000000 afgutils-1.0.8/afgutils/db.py
+-rw-rw-rw-   0        0        0      757 2023-04-06 17:33:13.000000 afgutils-1.0.8/afgutils/email.py
+-rw-rw-rw-   0        0        0     1677 2023-04-13 11:41:11.000000 afgutils-1.0.8/afgutils/s3.py
+-rw-rw-rw-   0        0        0     3903 2023-04-06 17:33:13.000000 afgutils-1.0.8/afgutils/trandata.py
+-rw-rw-rw-   0        0        0     3768 2023-07-12 18:01:04.000000 afgutils-1.0.8/afgutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:01:46.969494 afgutils-1.0.8/afgutils.egg-info/
+-rw-rw-rw-   0        0        0      224 2023-07-12 18:01:46.000000 afgutils-1.0.8/afgutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-07-12 18:01:46.000000 afgutils-1.0.8/afgutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:01:46.000000 afgutils-1.0.8/afgutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-12 18:01:46.000000 afgutils-1.0.8/afgutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 18:01:46.000000 afgutils-1.0.8/afgutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 18:01:46.973495 afgutils-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      633 2023-07-12 17:59:19.000000 afgutils-1.0.8/setup.py
```

### Comparing `afgutils-1.0.7/afgutils/advanceai_util.py` & `afgutils-1.0.8/afgutils/advanceai_util.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.7/afgutils/credolab.py` & `afgutils-1.0.8/afgutils/credolab.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.7/afgutils/db.py` & `afgutils-1.0.8/afgutils/db.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.7/afgutils/email.py` & `afgutils-1.0.8/afgutils/email.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.7/afgutils/s3.py` & `afgutils-1.0.8/afgutils/s3.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.7/afgutils/trandata.py` & `afgutils-1.0.8/afgutils/trandata.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.7/afgutils/utils.py` & `afgutils-1.0.8/afgutils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import time
 from os import environ
 from .db import DB, sql
-from pandas import json_normalize
 from pandas import DataFrame
 
 session_token_cookie_name = "uwtool_session_token"
 
 
 def print_log(log_line):
     print(time.strftime('%Y-%m-%d %H:%M:%S'), log_line)
@@ -96,17 +95,14 @@
         pass
 
     else:
         raise TypeError("data_vector_to_sql_insert: data_vector must be a pandas.DataFrame or a dictionary")
 
     # text-serialize any embedded lists or dictionaries
     item_values = [str(item_value) if type(item_value) in (list, dict) else item_value for item_value in item_values]
-    # convert any string booleans to actual booleans
-    item_values = [_convert_string_to_boolean(item_value) if type(item_value) is str else item_value for item_value in
-                   item_values]
 
     # combine existing values with new values
     if type(existing_values) is list:
         result_items = existing_values + item_values
     elif existing_values is None:
         result_items = item_values
     else:
@@ -118,15 +114,7 @@
     elif insert_sql_tpl is None:
         result_sql = column_names_insert_text
     else:
         raise TypeError("data_vector_to_sql_insert: insert_sql_tpl must be a string or None")
 
     return result_items, result_sql
 
-
-def _convert_string_to_boolean(s: str) -> bool | str:
-    if s.lower() == 'true':
-        return True
-    elif s.lower() == 'false':
-        return False
-    else:
-        return s
```

### Comparing `afgutils-1.0.7/setup.py` & `afgutils-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 DESCRIPTION = 'Shared support functions'
 LONG_DESCRIPTION = 'Shared support functions'
 
 setup(
     name="afgutils",
     version=VERSION,
     description=DESCRIPTION,
```

