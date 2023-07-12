# Comparing `tmp/soda-core-duckdb-3.0.44.tar.gz` & `tmp/soda-core-duckdb-3.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-duckdb-3.0.44.tar", last modified: Thu Jul  6 10:44:45 2023, max compression
+gzip compressed data, was "soda-core-duckdb-3.0.45.tar", last modified: Wed Jul 12 09:26:52 2023, max compression
```

## Comparing `soda-core-duckdb-3.0.44.tar` & `soda-core-duckdb-3.0.45.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:45.263563 soda-core-duckdb-3.0.44/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 10:44:45.263563 soda-core-duckdb-3.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 10:44:45.263563 soda-core-duckdb-3.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-07-06 10:44:10.000000 soda-core-duckdb-3.0.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:45.259564 soda-core-duckdb-3.0.44/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:45.263563 soda-core-duckdb-3.0.44/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     5504 2023-07-06 10:44:10.000000 soda-core-duckdb-3.0.44/soda/data_sources/duckdb_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:45.263563 soda-core-duckdb-3.0.44/soda_core_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 10:44:45.000000 soda-core-duckdb-3.0.44/soda_core_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-06 10:44:45.000000 soda-core-duckdb-3.0.44/soda_core_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 10:44:45.000000 soda-core-duckdb-3.0.44/soda_core_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-06 10:44:45.000000 soda-core-duckdb-3.0.44/soda_core_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-06 10:44:45.000000 soda-core-duckdb-3.0.44/soda_core_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:45.263563 soda-core-duckdb-3.0.44/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-07-06 10:44:10.000000 soda-core-duckdb-3.0.44/tests/test_duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:52.401868 soda-core-duckdb-3.0.45/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:52.401868 soda-core-duckdb-3.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 09:26:52.401868 soda-core-duckdb-3.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-07-12 09:26:19.000000 soda-core-duckdb-3.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:52.397868 soda-core-duckdb-3.0.45/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:52.397868 soda-core-duckdb-3.0.45/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5504 2023-07-12 09:26:19.000000 soda-core-duckdb-3.0.45/soda/data_sources/duckdb_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:52.401868 soda-core-duckdb-3.0.45/soda_core_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:52.000000 soda-core-duckdb-3.0.45/soda_core_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-12 09:26:52.000000 soda-core-duckdb-3.0.45/soda_core_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:26:52.000000 soda-core-duckdb-3.0.45/soda_core_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-12 09:26:52.000000 soda-core-duckdb-3.0.45/soda_core_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 09:26:52.000000 soda-core-duckdb-3.0.45/soda_core_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:52.401868 soda-core-duckdb-3.0.45/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-07-12 09:26:19.000000 soda-core-duckdb-3.0.45/tests/test_duckdb.py
```

### Comparing `soda-core-duckdb-3.0.44/setup.py` & `soda-core-duckdb-3.0.45/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-duckdb"
-package_version = "3.0.44"
+package_version = "3.0.45"
 description = "Soda Core Duckdb Package"
 
 requires = [f"soda-core=={package_version}", "duckdb<=0.8"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-duckdb-3.0.44/soda/data_sources/duckdb_data_source.py` & `soda-core-duckdb-3.0.45/soda/data_sources/duckdb_data_source.py`

 * *Files identical despite different names*

### Comparing `soda-core-duckdb-3.0.44/tests/test_duckdb.py` & `soda-core-duckdb-3.0.45/tests/test_duckdb.py`

 * *Files identical despite different names*

