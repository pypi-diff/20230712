# Comparing `tmp/mi-pyral-0.2.0.tar.gz` & `tmp/mi-pyral-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mi-pyral-0.2.0.tar", last modified: Wed Jul 12 01:10:47 2023, max compression
+gzip compressed data, was "mi-pyral-0.2.1.tar", last modified: Wed Jul 12 13:39:13 2023, max compression
```

## Comparing `mi-pyral-0.2.0.tar` & `mi-pyral-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 01:10:47.368620 mi-pyral-0.2.0/
--rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-04 22:05:28.000000 mi-pyral-0.2.0/LICENSE
--rw-r--r--   0 starr      (501) staff       (20)       27 2023-07-11 23:59:50.000000 mi-pyral-0.2.0/MANIFEST.in
--rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 01:10:47.368527 mi-pyral-0.2.0/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)      210 2022-10-08 18:13:55.000000 mi-pyral-0.2.0/README.md
--rw-r--r--   0 starr      (501) staff       (20)      910 2023-07-12 01:10:23.000000 mi-pyral-0.2.0/pyproject.toml
--rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-12 01:10:47.368650 mi-pyral-0.2.0/setup.cfg
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 01:10:47.366991 mi-pyral-0.2.0/src/
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 01:10:47.368028 mi-pyral-0.2.0/src/mi_pyral.egg-info/
--rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 01:10:47.000000 mi-pyral-0.2.0/src/mi_pyral.egg-info/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)      325 2023-07-12 01:10:47.000000 mi-pyral-0.2.0/src/mi_pyral.egg-info/SOURCES.txt
--rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-12 01:10:47.000000 mi-pyral-0.2.0/src/mi_pyral.egg-info/dependency_links.txt
--rw-r--r--   0 starr      (501) staff       (20)       47 2023-07-12 01:10:47.000000 mi-pyral-0.2.0/src/mi_pyral.egg-info/entry_points.txt
--rw-r--r--   0 starr      (501) staff       (20)       82 2023-07-12 01:10:47.000000 mi-pyral-0.2.0/src/mi_pyral.egg-info/requires.txt
--rw-r--r--   0 starr      (501) staff       (20)        6 2023-07-12 01:10:47.000000 mi-pyral-0.2.0/src/mi_pyral.egg-info/top_level.txt
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 01:10:47.368375 mi-pyral-0.2.0/src/pyral/
--rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-11 23:56:11.000000 mi-pyral-0.2.0/src/pyral/__init__.py
--rw-r--r--   0 starr      (501) staff       (20)     1453 2023-07-12 01:05:19.000000 mi-pyral-0.2.0/src/pyral/__main__.py
--rw-r--r--   0 starr      (501) staff       (20)      807 2023-07-12 00:44:58.000000 mi-pyral-0.2.0/src/pyral/log.conf
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 13:39:13.843759 mi-pyral-0.2.1/
+-rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/LICENSE
+-rw-r--r--   0 starr      (501) staff       (20)       66 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/MANIFEST.in
+-rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 13:39:13.843654 mi-pyral-0.2.1/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)      210 2022-10-08 18:13:55.000000 mi-pyral-0.2.1/README.md
+-rw-r--r--   0 starr      (501) staff       (20)      922 2023-07-12 13:38:58.000000 mi-pyral-0.2.1/pyproject.toml
+-rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-12 13:39:13.843795 mi-pyral-0.2.1/setup.cfg
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 13:39:13.841295 mi-pyral-0.2.1/src/
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 13:39:13.842283 mi-pyral-0.2.1/src/mi_pyral.egg-info/
+-rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)      479 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/SOURCES.txt
+-rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/dependency_links.txt
+-rw-r--r--   0 starr      (501) staff       (20)       47 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/entry_points.txt
+-rw-r--r--   0 starr      (501) staff       (20)       91 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/requires.txt
+-rw-r--r--   0 starr      (501) staff       (20)        6 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/top_level.txt
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 13:39:13.843507 mi-pyral-0.2.1/src/pyral/
+-rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-12 13:38:58.000000 mi-pyral-0.2.1/src/pyral/__init__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1453 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/__main__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1131 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/command.py
+-rw-r--r--   0 starr      (501) staff       (20)     2041 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/database.py
+-rw-r--r--   0 starr      (501) staff       (20)      726 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/exceptions.py
+-rw-r--r--   0 starr      (501) staff       (20)      807 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/log.conf
+-rw-r--r--   0 starr      (501) staff       (20)    25036 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/relation.py
+-rw-r--r--   0 starr      (501) staff       (20)    18344 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/relvar.py
+-rw-r--r--   0 starr      (501) staff       (20)      435 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/rtypes.py
+-rw-r--r--   0 starr      (501) staff       (20)     2104 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/transaction.py
```

### Comparing `mi-pyral-0.2.0/LICENSE` & `mi-pyral-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.0/PKG-INFO` & `mi-pyral-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mi-pyral
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyRAL Pythonic interface to TclRAL
 Author-email: Leon Starr <leon_starr@modelint.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Leon Starr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mi-pyral-0.2.0/pyproject.toml` & `mi-pyral-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mi-pyral"
-version = "0.2.0"
+version = "0.2.1"
 description = "PyRAL Pythonic interface to TclRAL"
 readme = "README.md"
 authors = [{ name = "Leon Starr", email = "leon_starr@modelint.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["relational", "tcl", "database", "cjdate", "darwen", "tutoriald", "thirdmanifesto"]
-dependencies = ['tomli; python_version < "3.11"']
+dependencies = ["tabulate", 'tomli; python_version < "3.11"']
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 build = ["build", "twine"]
 dev = ["bump2version", "pytest"]
 
 [project.scripts]
```

### Comparing `mi-pyral-0.2.0/src/mi_pyral.egg-info/PKG-INFO` & `mi-pyral-0.2.1/src/mi_pyral.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mi-pyral
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyRAL Pythonic interface to TclRAL
 Author-email: Leon Starr <leon_starr@modelint.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Leon Starr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mi-pyral-0.2.0/src/pyral/__main__.py` & `mi-pyral-0.2.1/src/pyral/__main__.py`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.0/src/pyral/log.conf` & `mi-pyral-0.2.1/src/pyral/log.conf`

 * *Files identical despite different names*

