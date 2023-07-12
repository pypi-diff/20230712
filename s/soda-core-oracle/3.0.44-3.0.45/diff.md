# Comparing `tmp/soda-core-oracle-3.0.44.tar.gz` & `tmp/soda-core-oracle-3.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-oracle-3.0.44.tar", last modified: Thu Jul  6 10:44:50 2023, max compression
+gzip compressed data, was "soda-core-oracle-3.0.45.tar", last modified: Wed Jul 12 09:26:57 2023, max compression
```

## Comparing `soda-core-oracle-3.0.44.tar` & `soda-core-oracle-3.0.45.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:50.487697 soda-core-oracle-3.0.44/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 10:44:50.487697 soda-core-oracle-3.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 10:44:50.487697 soda-core-oracle-3.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-06 10:44:10.000000 soda-core-oracle-3.0.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:50.487697 soda-core-oracle-3.0.44/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:50.487697 soda-core-oracle-3.0.44/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     9209 2023-07-06 10:44:10.000000 soda-core-oracle-3.0.44/soda/data_sources/oracle_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:44:50.487697 soda-core-oracle-3.0.44/soda_core_oracle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 10:44:50.000000 soda-core-oracle-3.0.44/soda_core_oracle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-06 10:44:50.000000 soda-core-oracle-3.0.44/soda_core_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 10:44:50.000000 soda-core-oracle-3.0.44/soda_core_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-06 10:44:50.000000 soda-core-oracle-3.0.44/soda_core_oracle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-06 10:44:50.000000 soda-core-oracle-3.0.44/soda_core_oracle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:57.858028 soda-core-oracle-3.0.45/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:57.858028 soda-core-oracle-3.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 09:26:57.858028 soda-core-oracle-3.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-12 09:26:19.000000 soda-core-oracle-3.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:57.854028 soda-core-oracle-3.0.45/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:57.858028 soda-core-oracle-3.0.45/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     9209 2023-07-12 09:26:19.000000 soda-core-oracle-3.0.45/soda/data_sources/oracle_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:57.858028 soda-core-oracle-3.0.45/soda_core_oracle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:57.000000 soda-core-oracle-3.0.45/soda_core_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-12 09:26:57.000000 soda-core-oracle-3.0.45/soda_core_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:26:57.000000 soda-core-oracle-3.0.45/soda_core_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-12 09:26:57.000000 soda-core-oracle-3.0.45/soda_core_oracle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 09:26:57.000000 soda-core-oracle-3.0.45/soda_core_oracle.egg-info/top_level.txt
```

### Comparing `soda-core-oracle-3.0.44/setup.py` & `soda-core-oracle-3.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-oracle"
-package_version = "3.0.44"
+package_version = "3.0.45"
 # TODO Add proper description
 description = "Soda Core Oracle Package"
 
 requires = [f"soda-core=={package_version}", "oracledb==1.1.1"]
 # TODO Fix the params
 setup(
     name=package_name,
```

### Comparing `soda-core-oracle-3.0.44/soda/data_sources/oracle_data_source.py` & `soda-core-oracle-3.0.45/soda/data_sources/oracle_data_source.py`

 * *Files identical despite different names*

