# Comparing `tmp/soda-core-dremio-3.0.44.tar.gz` & `tmp/soda-core-dremio-3.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-dremio-3.0.44.tar", last modified: Thu Jul  6 10:44:42 2023, max compression
+gzip compressed data, was "soda-core-dremio-3.0.45.tar", last modified: Wed Jul 12 09:26:49 2023, max compression
```

## Comparing `soda-core-dremio-3.0.44.tar` & `soda-core-dremio-3.0.45.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:42.459488 soda-core-dremio-3.0.44/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 10:44:42.459488 soda-core-dremio-3.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 10:44:42.459488 soda-core-dremio-3.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-06 10:44:10.000000 soda-core-dremio-3.0.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:42.459488 soda-core-dremio-3.0.44/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:42.459488 soda-core-dremio-3.0.44/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-07-06 10:44:10.000000 soda-core-dremio-3.0.44/soda/data_sources/dremio_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:42.459488 soda-core-dremio-3.0.44/soda_core_dremio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 10:44:42.000000 soda-core-dremio-3.0.44/soda_core_dremio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-06 10:44:42.000000 soda-core-dremio-3.0.44/soda_core_dremio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 10:44:42.000000 soda-core-dremio-3.0.44/soda_core_dremio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-06 10:44:42.000000 soda-core-dremio-3.0.44/soda_core_dremio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-06 10:44:42.000000 soda-core-dremio-3.0.44/soda_core_dremio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:42.459488 soda-core-dremio-3.0.44/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-06 10:44:10.000000 soda-core-dremio-3.0.44/tests/test_dremio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:49.557786 soda-core-dremio-3.0.45/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:49.557786 soda-core-dremio-3.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 09:26:49.557786 soda-core-dremio-3.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-12 09:26:19.000000 soda-core-dremio-3.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:49.557786 soda-core-dremio-3.0.45/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:49.557786 soda-core-dremio-3.0.45/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-07-12 09:26:19.000000 soda-core-dremio-3.0.45/soda/data_sources/dremio_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:49.557786 soda-core-dremio-3.0.45/soda_core_dremio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:49.000000 soda-core-dremio-3.0.45/soda_core_dremio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-12 09:26:49.000000 soda-core-dremio-3.0.45/soda_core_dremio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:26:49.000000 soda-core-dremio-3.0.45/soda_core_dremio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-12 09:26:49.000000 soda-core-dremio-3.0.45/soda_core_dremio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 09:26:49.000000 soda-core-dremio-3.0.45/soda_core_dremio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:49.557786 soda-core-dremio-3.0.45/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-12 09:26:19.000000 soda-core-dremio-3.0.45/tests/test_dremio.py
```

### Comparing `soda-core-dremio-3.0.44/setup.py` & `soda-core-dremio-3.0.45/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-dremio"
-package_version = "3.0.44"
+package_version = "3.0.45"
 description = "Soda Core Dremio Package"
 
 requires = [f"soda-core=={package_version}", "pyodbc", "pyarrow"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-dremio-3.0.44/soda/data_sources/dremio_data_source.py` & `soda-core-dremio-3.0.45/soda/data_sources/dremio_data_source.py`

 * *Files identical despite different names*

