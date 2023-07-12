# Comparing `tmp/soda-core-pandas-dask-3.0.44.tar.gz` & `tmp/soda-core-pandas-dask-3.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-pandas-dask-3.0.44.tar", last modified: Thu Jul  6 10:44:30 2023, max compression
+gzip compressed data, was "soda-core-pandas-dask-3.0.45.tar", last modified: Wed Jul 12 09:26:37 2023, max compression
```

## Comparing `soda-core-pandas-dask-3.0.44.tar` & `soda-core-pandas-dask-3.0.45.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:29.999172 soda-core-pandas-dask-3.0.44/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-06 10:44:29.999172 soda-core-pandas-dask-3.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 10:44:29.999172 soda-core-pandas-dask-3.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-07-06 10:44:10.000000 soda-core-pandas-dask-3.0.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:29.999172 soda-core-pandas-dask-3.0.44/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:29.999172 soda-core-pandas-dask-3.0.44/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-06 10:44:10.000000 soda-core-pandas-dask-3.0.44/soda/data_sources/dask_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-07-06 10:44:10.000000 soda-core-pandas-dask-3.0.44/soda/data_sources/dask_cursor.py
--rw-r--r--   0 runner    (1001) docker     (122)    13934 2023-07-06 10:44:10.000000 soda-core-pandas-dask-3.0.44/soda/data_sources/dask_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:29.999172 soda-core-pandas-dask-3.0.44/soda_core_pandas_dask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-06 10:44:29.000000 soda-core-pandas-dask-3.0.44/soda_core_pandas_dask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-06 10:44:29.000000 soda-core-pandas-dask-3.0.44/soda_core_pandas_dask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 10:44:29.000000 soda-core-pandas-dask-3.0.44/soda_core_pandas_dask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-06 10:44:29.000000 soda-core-pandas-dask-3.0.44/soda_core_pandas_dask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-06 10:44:29.000000 soda-core-pandas-dask-3.0.44/soda_core_pandas_dask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:29.999172 soda-core-pandas-dask-3.0.44/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-06 10:44:10.000000 soda-core-pandas-dask-3.0.44/tests/test_dask.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:37.105425 soda-core-pandas-dask-3.0.45/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-12 09:26:37.105425 soda-core-pandas-dask-3.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 09:26:37.105425 soda-core-pandas-dask-3.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-07-12 09:26:19.000000 soda-core-pandas-dask-3.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:37.101425 soda-core-pandas-dask-3.0.45/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:37.101425 soda-core-pandas-dask-3.0.45/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-12 09:26:19.000000 soda-core-pandas-dask-3.0.45/soda/data_sources/dask_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-07-12 09:26:19.000000 soda-core-pandas-dask-3.0.45/soda/data_sources/dask_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13934 2023-07-12 09:26:19.000000 soda-core-pandas-dask-3.0.45/soda/data_sources/dask_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:37.105425 soda-core-pandas-dask-3.0.45/soda_core_pandas_dask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-12 09:26:37.000000 soda-core-pandas-dask-3.0.45/soda_core_pandas_dask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-12 09:26:37.000000 soda-core-pandas-dask-3.0.45/soda_core_pandas_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:26:37.000000 soda-core-pandas-dask-3.0.45/soda_core_pandas_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-12 09:26:37.000000 soda-core-pandas-dask-3.0.45/soda_core_pandas_dask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 09:26:37.000000 soda-core-pandas-dask-3.0.45/soda_core_pandas_dask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:37.105425 soda-core-pandas-dask-3.0.45/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-12 09:26:19.000000 soda-core-pandas-dask-3.0.45/tests/test_dask.py
```

### Comparing `soda-core-pandas-dask-3.0.44/setup.py` & `soda-core-pandas-dask-3.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-pandas-dask"
-package_version = "3.0.44"
+package_version = "3.0.45"
 description = "Soda Core Dask Package"
 
 requires = [f"soda-core=={package_version}", "dask>=2022.10.0", "dask-sql>=2022.12.0,<2023.6.0"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-pandas-dask-3.0.44/soda/data_sources/dask_cursor.py` & `soda-core-pandas-dask-3.0.45/soda/data_sources/dask_cursor.py`

 * *Files identical despite different names*

### Comparing `soda-core-pandas-dask-3.0.44/soda/data_sources/dask_data_source.py` & `soda-core-pandas-dask-3.0.45/soda/data_sources/dask_data_source.py`

 * *Files identical despite different names*

