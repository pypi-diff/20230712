# Comparing `tmp/pylittle-0.0.1.tar.gz` & `tmp/pylittle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylittle-0.0.1.tar", last modified: Tue Jul 11 17:05:45 2023, max compression
+gzip compressed data, was "dist/pylittle-0.0.2.tar", last modified: Wed Jul 12 06:55:39 2023, max compression
```

## Comparing `pylittle-0.0.1.tar` & `pylittle-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-11 17:05:45.940961 pylittle-0.0.1/
--rw-rw-r--   0 gary      (1000) gary      (1000)     1443 2023-07-11 17:05:45.940961 pylittle-0.0.1/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)       12 2023-07-11 06:29:05.000000 pylittle-0.0.1/README.md
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-11 17:05:45.940961 pylittle-0.0.1/pylittle/
--rw-rw-r--   0 gary      (1000) gary      (1000)       81 2023-07-11 16:54:38.000000 pylittle-0.0.1/pylittle/__init__.py
--rw-rw-r--   0 gary      (1000) gary      (1000)       30 2023-07-11 16:54:09.000000 pylittle-0.0.1/pylittle/main.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-11 17:05:45.940961 pylittle-0.0.1/pylittle.egg-info/
--rw-rw-r--   0 gary      (1000) gary      (1000)     1443 2023-07-11 17:05:45.000000 pylittle-0.0.1/pylittle.egg-info/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)      250 2023-07-11 17:05:45.000000 pylittle-0.0.1/pylittle.egg-info/SOURCES.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-07-11 17:05:45.000000 pylittle-0.0.1/pylittle.egg-info/dependency_links.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       47 2023-07-11 17:05:45.000000 pylittle-0.0.1/pylittle.egg-info/entry_points.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       42 2023-07-11 17:05:45.000000 pylittle-0.0.1/pylittle.egg-info/requires.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        9 2023-07-11 17:05:45.000000 pylittle-0.0.1/pylittle.egg-info/top_level.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       38 2023-07-11 17:05:45.940961 pylittle-0.0.1/setup.cfg
--rw-rw-r--   0 gary      (1000) gary      (1000)     2090 2023-07-11 17:05:42.000000 pylittle-0.0.1/setup.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-12 06:55:39.984646 pylittle-0.0.2/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1443 2023-07-12 06:55:39.984646 pylittle-0.0.2/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)       12 2023-07-11 06:29:05.000000 pylittle-0.0.2/README.md
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-12 06:55:39.984646 pylittle-0.0.2/pylittle/
+-rw-rw-r--   0 gary      (1000) gary      (1000)      109 2023-07-12 06:35:28.000000 pylittle-0.0.2/pylittle/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)       30 2023-07-11 16:54:09.000000 pylittle-0.0.2/pylittle/main.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-12 06:55:39.984646 pylittle-0.0.2/pylittle.egg-info/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1443 2023-07-12 06:55:39.000000 pylittle-0.0.2/pylittle.egg-info/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)      250 2023-07-12 06:55:39.000000 pylittle-0.0.2/pylittle.egg-info/SOURCES.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-07-12 06:55:39.000000 pylittle-0.0.2/pylittle.egg-info/dependency_links.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       47 2023-07-12 06:55:39.000000 pylittle-0.0.2/pylittle.egg-info/entry_points.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       42 2023-07-12 06:55:39.000000 pylittle-0.0.2/pylittle.egg-info/requires.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        9 2023-07-12 06:55:39.000000 pylittle-0.0.2/pylittle.egg-info/top_level.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       38 2023-07-12 06:55:39.984646 pylittle-0.0.2/setup.cfg
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2090 2023-07-12 01:40:52.000000 pylittle-0.0.2/setup.py
```

### Comparing `pylittle-0.0.1/PKG-INFO` & `pylittle-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylittle
-Version: 0.0.1
+Version: 0.0.2
 Summary: pylittle test
 Home-page: https://www.pylittle.io/
 Author: pylittle Systems, Inc.
 Author-email: support@pylittle.io
 License: Proprietary License
 Project-URL: Homepage, https://www.pylittle.io/
 Project-URL: Documentation, https://www.pylittle.io/
```

### Comparing `pylittle-0.0.1/pylittle.egg-info/PKG-INFO` & `pylittle-0.0.2/pylittle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylittle
-Version: 0.0.1
+Version: 0.0.2
 Summary: pylittle test
 Home-page: https://www.pylittle.io/
 Author: pylittle Systems, Inc.
 Author-email: support@pylittle.io
 License: Proprietary License
 Project-URL: Homepage, https://www.pylittle.io/
 Project-URL: Documentation, https://www.pylittle.io/
```

### Comparing `pylittle-0.0.1/setup.py` & `pylittle-0.0.2/setup.py`

 * *Files identical despite different names*

