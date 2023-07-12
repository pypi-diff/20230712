# Comparing `tmp/soda-core-denodo-3.0.44.tar.gz` & `tmp/soda-core-denodo-3.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-denodo-3.0.44.tar", last modified: Thu Jul  6 10:44:39 2023, max compression
+gzip compressed data, was "soda-core-denodo-3.0.45.tar", last modified: Wed Jul 12 09:26:46 2023, max compression
```

## Comparing `soda-core-denodo-3.0.44.tar` & `soda-core-denodo-3.0.45.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:39.755424 soda-core-denodo-3.0.44/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 10:44:39.755424 soda-core-denodo-3.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 10:44:39.755424 soda-core-denodo-3.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-07-06 10:44:10.000000 soda-core-denodo-3.0.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:39.755424 soda-core-denodo-3.0.44/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:39.755424 soda-core-denodo-3.0.44/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-07-06 10:44:10.000000 soda-core-denodo-3.0.44/soda/data_sources/denodo_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:39.755424 soda-core-denodo-3.0.44/soda_core_denodo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 10:44:39.000000 soda-core-denodo-3.0.44/soda_core_denodo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-06 10:44:39.000000 soda-core-denodo-3.0.44/soda_core_denodo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 10:44:39.000000 soda-core-denodo-3.0.44/soda_core_denodo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-06 10:44:39.000000 soda-core-denodo-3.0.44/soda_core_denodo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-06 10:44:39.000000 soda-core-denodo-3.0.44/soda_core_denodo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-07-12 09:26:19.000000 soda-core-denodo-3.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-07-12 09:26:19.000000 soda-core-denodo-3.0.45/soda/data_sources/denodo_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/top_level.txt
```

### Comparing `soda-core-denodo-3.0.44/setup.py` & `soda-core-denodo-3.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-denodo"
-package_version = "3.0.44"
+package_version = "3.0.45"
 # TODO Add proper description
 description = "Soda Core Denodo Package"
 
 requires = [f"soda-core=={package_version}", f"soda-core-postgres=={package_version}"]
 # TODO Fix the params
 setup(
     name=package_name,
```

### Comparing `soda-core-denodo-3.0.44/soda/data_sources/denodo_data_source.py` & `soda-core-denodo-3.0.45/soda/data_sources/denodo_data_source.py`

 * *Files identical despite different names*

