# Comparing `tmp/ufs_pyutils-0.0.1.tar.gz` & `tmp/ufs_pyutils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufs_pyutils-0.0.1.tar", last modified: Wed Jul 12 00:29:50 2023, max compression
+gzip compressed data, was "ufs_pyutils-0.1.0.tar", last modified: Wed Jul 12 01:58:39 2023, max compression
```

## Comparing `ufs_pyutils-0.0.1.tar` & `ufs_pyutils-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:29:50.274567 ufs_pyutils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-12 00:29:39.000000 ufs_pyutils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-12 00:29:50.274567 ufs_pyutils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-12 00:29:39.000000 ufs_pyutils-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-12 00:29:50.274567 ufs_pyutils-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 00:29:39.000000 ufs_pyutils-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:29:50.274567 ufs_pyutils-0.0.1/ufs_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-12 00:29:50.000000 ufs_pyutils-0.0.1/ufs_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-12 00:29:50.000000 ufs_pyutils-0.0.1/ufs_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:29:50.000000 ufs_pyutils-0.0.1/ufs_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 00:29:50.000000 ufs_pyutils-0.0.1/ufs_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:29:50.000000 ufs_pyutils-0.0.1/ufs_pyutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:58:39.714282 ufs_pyutils-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-12 01:58:29.000000 ufs_pyutils-0.1.0/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-12 01:58:29.000000 ufs_pyutils-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-12 01:58:39.714282 ufs_pyutils-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-12 01:58:29.000000 ufs_pyutils-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-12 01:58:39.718282 ufs_pyutils-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 01:58:29.000000 ufs_pyutils-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:58:39.714282 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/top_level.txt
```

### Comparing `ufs_pyutils-0.0.1/LICENSE` & `ufs_pyutils-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ufs_pyutils-0.0.1/PKG-INFO` & `ufs_pyutils-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,24 @@
-Metadata-Version: 2.1
-Name: ufs_pyutils
-Version: 0.0.1
-Summary: "API package containing Python utilities for UFS applications."
-Home-page: https://github.com/HenryWinterbottom-NOAA/ufs_pyutils
-Author: "Henry R. Winterbottom"
-License: GNU Lesser General Public License v2 (LGPLv2)
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Classifier: Typing :: Typed
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![License](https://img.shields.io/badge/License-LGPL_v2.1-black)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/blob/develop/LICENSE)
 ![Linux](https://img.shields.io/badge/Linux-ubuntu%7Ccentos-lightgrey)
 ![Python Version](https://img.shields.io/badge/Python-3.5|3.6|3.7|3.8|3.9-blue)
 [![Code style: black](https://img.shields.io/badge/Code%20Style-black-purple.svg)](https://github.com/psf/black)
+[![Documentation Status](https://img.shields.io/badge/Documentation-latest-gree)](https://ufs-pyutils.readthedocs.io/en/latest/?badge=latest)
 
 [![Build Tests](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/buildtest.yaml)
 [![Unit Tests](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/unittests.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/unittests.yaml)
 [![Python Coding Standards](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pycodestyle.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pycodestyle.yaml)
 [![Container Builds](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/containers.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/containers.yaml)
-[![Documentation Status](https://readthedocs.org/projects/ufs-pyutils/badge/?version=latest)](https://ufs-pyutils.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pypi.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pypi.yaml)
+
+# Installation
+
+~~~
+user@host:$ pip install ufs-pyutils
+~~~
 
 # Cloning
 
 This repository utilizes several sub-modules from various sources. To
 obtain the entire system, do as follows.
 
 ~~~
```

### Comparing `ufs_pyutils-0.0.1/setup.cfg` & `ufs_pyutils-0.1.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = ufs_pyutils
-version = 0.0.1
-description = "API package containing Python utilities for UFS applications."
-long_description = file: README.md
+version = 0.1.0
+description = "Python Toolbox API for UFS applications."
+long_description = file: INSTALL.md
 long_description_content_type = text/markdown
 author = "Henry R. Winterbottom"
 home_page = https://github.com/HenryWinterbottom-NOAA/ufs_pyutils
 license = GNU Lesser General Public License v2 (LGPLv2)
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
```

