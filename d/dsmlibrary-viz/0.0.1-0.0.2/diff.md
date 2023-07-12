# Comparing `tmp/dsmlibrary_viz-0.0.1.tar.gz` & `tmp/dsmlibrary_viz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmlibrary_viz-0.0.1.tar", last modified: Wed Jul 12 14:22:47 2023, max compression
+gzip compressed data, was "dsmlibrary_viz-0.0.2.tar", last modified: Wed Jul 12 14:26:32 2023, max compression
```

## Comparing `dsmlibrary_viz-0.0.1.tar` & `dsmlibrary_viz-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-12 14:22:47.806380 dsmlibrary_viz-0.0.1/
--rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.1/LICENSE
--rw-r--r--   0 naii       (501) staff       (20)      715 2023-07-12 14:22:47.805641 dsmlibrary_viz-0.0.1/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)       16 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.1/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-12 14:22:47.800689 dsmlibrary_viz-0.0.1/dsmlibrary_viz/
--rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-12 12:12:47.000000 dsmlibrary_viz-0.0.1/dsmlibrary_viz/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.1/dsmlibrary_viz/base.py
--rw-r--r--   0 naii       (501) staff       (20)     1335 2023-07-12 14:19:49.000000 dsmlibrary_viz-0.0.1/dsmlibrary_viz/data_viz.py
--rw-r--r--   0 naii       (501) staff       (20)      232 2023-07-12 14:07:14.000000 dsmlibrary_viz-0.0.1/dsmlibrary_viz/utils.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-12 14:22:47.804890 dsmlibrary_viz-0.0.1/dsmlibrary_viz.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)      715 2023-07-12 14:22:47.000000 dsmlibrary_viz-0.0.1/dsmlibrary_viz.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      316 2023-07-12 14:22:47.000000 dsmlibrary_viz-0.0.1/dsmlibrary_viz.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-12 14:22:47.000000 dsmlibrary_viz-0.0.1/dsmlibrary_viz.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       27 2023-07-12 14:22:47.000000 dsmlibrary_viz-0.0.1/dsmlibrary_viz.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-12 14:22:47.000000 dsmlibrary_viz-0.0.1/dsmlibrary_viz.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-12 14:22:47.806553 dsmlibrary_viz-0.0.1/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1409 2023-07-12 14:20:23.000000 dsmlibrary_viz-0.0.1/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-12 14:26:32.471256 dsmlibrary_viz-0.0.2/
+-rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.2/LICENSE
+-rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-12 14:26:32.469952 dsmlibrary_viz-0.0.2/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      355 2023-07-12 14:26:15.000000 dsmlibrary_viz-0.0.2/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-12 14:26:32.452189 dsmlibrary_viz-0.0.2/dsmlibrary_viz/
+-rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-12 14:26:28.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz/base.py
+-rw-r--r--   0 naii       (501) staff       (20)     1335 2023-07-12 14:19:49.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz/data_viz.py
+-rw-r--r--   0 naii       (501) staff       (20)      232 2023-07-12 14:07:14.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz/utils.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-12 14:26:32.468687 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      316 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       28 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-12 14:26:32.471797 dsmlibrary_viz-0.0.2/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     1410 2023-07-12 14:24:27.000000 dsmlibrary_viz-0.0.2/setup.py
```

### Comparing `dsmlibrary_viz-0.0.1/LICENSE` & `dsmlibrary_viz-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.1/dsmlibrary_viz/base.py` & `dsmlibrary_viz-0.0.2/dsmlibrary_viz/base.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.1/dsmlibrary_viz/data_viz.py` & `dsmlibrary_viz-0.0.2/dsmlibrary_viz/data_viz.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.1/setup.py` & `dsmlibrary_viz-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,11 +36,11 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
 
     ],
     install_requires=[
         'requests',
         's3fs',
-        'duckdb'
+        'duckdb',
         'pandas'
     ],    
 )
```

