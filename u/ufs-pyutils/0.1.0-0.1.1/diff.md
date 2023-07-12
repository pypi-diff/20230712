# Comparing `tmp/ufs_pyutils-0.1.0.tar.gz` & `tmp/ufs_pyutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufs_pyutils-0.1.0.tar", last modified: Wed Jul 12 01:58:39 2023, max compression
+gzip compressed data, was "ufs_pyutils-0.1.1.tar", last modified: Wed Jul 12 14:48:19 2023, max compression
```

## Comparing `ufs_pyutils-0.1.0.tar` & `ufs_pyutils-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:58:39.714282 ufs_pyutils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-12 01:58:29.000000 ufs_pyutils-0.1.0/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-12 01:58:29.000000 ufs_pyutils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-12 01:58:39.714282 ufs_pyutils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-12 01:58:29.000000 ufs_pyutils-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-12 01:58:39.718282 ufs_pyutils-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 01:58:29.000000 ufs_pyutils-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:58:39.714282 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:58:39.000000 ufs_pyutils-0.1.0/ufs_pyutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:19.431687 ufs_pyutils-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-12 14:48:08.000000 ufs_pyutils-0.1.1/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-12 14:48:08.000000 ufs_pyutils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 14:48:19.431687 ufs_pyutils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-12 14:48:08.000000 ufs_pyutils-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-12 14:48:19.431687 ufs_pyutils-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 14:48:08.000000 ufs_pyutils-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:19.427687 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/top_level.txt
```

### Comparing `ufs_pyutils-0.1.0/INSTALL.md` & `ufs_pyutils-0.1.1/INSTALL.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 
 [![Build Tests](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/buildtest.yaml)
 [![Unit Tests](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/unittests.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/unittests.yaml)
 [![Python Coding Standards](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pycodestyle.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pycodestyle.yaml)
 [![Container Builds](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/containers.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/containers.yaml)
 [![PyPI](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pypi.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pypi.yaml)
 
-# Purpose
+# Description
 
-This the `ufs_pyutils` package contains an API utilized by multiple
-[Unified Forecast System](https://ufscommunity.org/) (UFS)
-applications. However, it is not limited only to such applications and
-may be where the provided application interfaces are valid and/or
-useful.
+The `ufs_pyutils` package contains an toolbox of APIs for various
+workflow and diagnostic tool applications. Currently this utilized by
+multiple applications derived from the [Unified Forecast
+System](https://ufscommunity.org/) (UFS). However, it is not limited
+only to the UFS and may be useful and/or applicable to other such
+packages.
 
 # Installation
 
 The `ufs_pyutils` package may be installed as follows.
 
 ~~~
 user@host:$ pip install --user ufs-pyutils
 ~~~
 
-The available unit-tests for the available APIs may be executed as
-follows.
+The unit-tests for the available APIs may be executed as follows.
 
 ~~~
 user@host:$ cd /path/to/ufs_pyutils
 user@host:$ /path/to/pytest confs
 user@host:$ /path/to/pytest ioapps
 user@host:$ /path/to/pytest tools
 user@host:$ /path/to/pytest utils
```

### Comparing `ufs_pyutils-0.1.0/LICENSE` & `ufs_pyutils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ufs_pyutils-0.1.0/PKG-INFO` & `ufs_pyutils-0.1.1/ufs_pyutils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: ufs_pyutils
-Version: 0.1.0
-Summary: "Python Toolbox API for UFS applications."
+Name: ufs-pyutils
+Version: 0.1.1
+Summary: Python Toolbox of API used for UFS applications.
 Home-page: https://github.com/HenryWinterbottom-NOAA/ufs_pyutils
 Author: "Henry R. Winterbottom"
 License: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
@@ -31,32 +31,32 @@
 
 [![Build Tests](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/buildtest.yaml)
 [![Unit Tests](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/unittests.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/unittests.yaml)
 [![Python Coding Standards](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pycodestyle.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pycodestyle.yaml)
 [![Container Builds](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/containers.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/containers.yaml)
 [![PyPI](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pypi.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pypi.yaml)
 
-# Purpose
+# Description
 
-This the `ufs_pyutils` package contains an API utilized by multiple
-[Unified Forecast System](https://ufscommunity.org/) (UFS)
-applications. However, it is not limited only to such applications and
-may be where the provided application interfaces are valid and/or
-useful.
+The `ufs_pyutils` package contains an toolbox of APIs for various
+workflow and diagnostic tool applications. Currently this utilized by
+multiple applications derived from the [Unified Forecast
+System](https://ufscommunity.org/) (UFS). However, it is not limited
+only to the UFS and may be useful and/or applicable to other such
+packages.
 
 # Installation
 
 The `ufs_pyutils` package may be installed as follows.
 
 ~~~
 user@host:$ pip install --user ufs-pyutils
 ~~~
 
-The available unit-tests for the available APIs may be executed as
-follows.
+The unit-tests for the available APIs may be executed as follows.
 
 ~~~
 user@host:$ cd /path/to/ufs_pyutils
 user@host:$ /path/to/pytest confs
 user@host:$ /path/to/pytest ioapps
 user@host:$ /path/to/pytest tools
 user@host:$ /path/to/pytest utils
```

### Comparing `ufs_pyutils-0.1.0/README.md` & `ufs_pyutils-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ufs_pyutils-0.1.0/setup.cfg` & `ufs_pyutils-0.1.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = ufs_pyutils
-version = 0.1.0
-description = "Python Toolbox API for UFS applications."
+version = 0.1.1
+description = Python Toolbox of API used for UFS applications.
 long_description = file: INSTALL.md
 long_description_content_type = text/markdown
 author = "Henry R. Winterbottom"
 home_page = https://github.com/HenryWinterbottom-NOAA/ufs_pyutils
 license = GNU Lesser General Public License v2 (LGPLv2)
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `ufs_pyutils-0.1.0/ufs_pyutils.egg-info/PKG-INFO` & `ufs_pyutils-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: ufs-pyutils
-Version: 0.1.0
-Summary: "Python Toolbox API for UFS applications."
+Name: ufs_pyutils
+Version: 0.1.1
+Summary: Python Toolbox of API used for UFS applications.
 Home-page: https://github.com/HenryWinterbottom-NOAA/ufs_pyutils
 Author: "Henry R. Winterbottom"
 License: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
@@ -31,32 +31,32 @@
 
 [![Build Tests](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/buildtest.yaml)
 [![Unit Tests](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/unittests.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/unittests.yaml)
 [![Python Coding Standards](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pycodestyle.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pycodestyle.yaml)
 [![Container Builds](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/containers.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/containers.yaml)
 [![PyPI](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pypi.yaml/badge.svg)](https://github.com/HenryWinterbottom-NOAA/ufs_pyutils/actions/workflows/pypi.yaml)
 
-# Purpose
+# Description
 
-This the `ufs_pyutils` package contains an API utilized by multiple
-[Unified Forecast System](https://ufscommunity.org/) (UFS)
-applications. However, it is not limited only to such applications and
-may be where the provided application interfaces are valid and/or
-useful.
+The `ufs_pyutils` package contains an toolbox of APIs for various
+workflow and diagnostic tool applications. Currently this utilized by
+multiple applications derived from the [Unified Forecast
+System](https://ufscommunity.org/) (UFS). However, it is not limited
+only to the UFS and may be useful and/or applicable to other such
+packages.
 
 # Installation
 
 The `ufs_pyutils` package may be installed as follows.
 
 ~~~
 user@host:$ pip install --user ufs-pyutils
 ~~~
 
-The available unit-tests for the available APIs may be executed as
-follows.
+The unit-tests for the available APIs may be executed as follows.
 
 ~~~
 user@host:$ cd /path/to/ufs_pyutils
 user@host:$ /path/to/pytest confs
 user@host:$ /path/to/pytest ioapps
 user@host:$ /path/to/pytest tools
 user@host:$ /path/to/pytest utils
```

