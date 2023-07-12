# Comparing `tmp/eef-data-0.3.tar.gz` & `tmp/eef-data-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eef-data-0.3.tar", last modified: Wed Jul 12 11:59:27 2023, max compression
+gzip compressed data, was "eef-data-0.4.tar", last modified: Wed Jul 12 12:06:47 2023, max compression
```

## Comparing `eef-data-0.3.tar` & `eef-data-0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 11:59:27.463227 eef-data-0.3/
--rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.3/LICENSE
--rw-rw-r--   0 linux     (1000) linux     (1000)      153 2023-07-12 11:59:27.463227 eef-data-0.3/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)    62974 2023-07-10 13:29:48.000000 eef-data-0.3/README.md
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 11:59:27.459227 eef-data-0.3/eef_data.egg-info/
--rw-rw-r--   0 linux     (1000) linux     (1000)      153 2023-07-12 11:59:27.000000 eef-data-0.3/eef_data.egg-info/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 11:59:27.000000 eef-data-0.3/eef_data.egg-info/SOURCES.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 11:59:27.000000 eef-data-0.3/eef_data.egg-info/dependency_links.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 11:59:27.000000 eef-data-0.3/eef_data.egg-info/entry_points.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 11:59:27.000000 eef-data-0.3/eef_data.egg-info/requires.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 11:59:27.000000 eef-data-0.3/eef_data.egg-info/top_level.txt
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 11:59:27.459227 eef-data-0.3/eefdata/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.3/eefdata/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.3/eefdata/app.py
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 11:59:27.463227 eef-data-0.3/eefdata/src/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.3/eefdata/src/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.3/eefdata/src/attributeIDs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.3/eefdata/src/funcs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 11:59:27.463227 eef-data-0.3/setup.cfg
--rw-rw-r--   0 linux     (1000) linux     (1000)      424 2023-07-12 11:59:19.000000 eef-data-0.3/setup.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:06:47.896579 eef-data-0.4/
+-rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.4/LICENSE
+-rw-rw-r--   0 linux     (1000) linux     (1000)    63160 2023-07-12 12:06:47.896579 eef-data-0.4/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62974 2023-07-10 13:29:48.000000 eef-data-0.4/README.md
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:06:47.892579 eef-data-0.4/eef_data.egg-info/
+-rw-rw-r--   0 linux     (1000) linux     (1000)    63160 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/entry_points.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/requires.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/top_level.txt
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:06:47.892579 eef-data-0.4/eefdata/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.4/eefdata/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.4/eefdata/app.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:06:47.892579 eef-data-0.4/eefdata/src/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.4/eefdata/src/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.4/eefdata/src/attributeIDs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.4/eefdata/src/funcs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 12:06:47.896579 eef-data-0.4/setup.cfg
+-rw-rw-r--   0 linux     (1000) linux     (1000)      684 2023-07-12 12:06:36.000000 eef-data-0.4/setup.py
```

### Comparing `eef-data-0.3/LICENSE` & `eef-data-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eef-data-0.3/README.md` & `eef-data-0.4/README.md`

 * *Files identical despite different names*

### Comparing `eef-data-0.3/eefdata/app.py` & `eef-data-0.4/eefdata/app.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.3/eefdata/src/attributeIDs.py` & `eef-data-0.4/eefdata/src/attributeIDs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.3/eefdata/src/funcs.py` & `eef-data-0.4/eefdata/src/funcs.py`

 * *Files identical despite different names*

