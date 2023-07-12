# Comparing `tmp/ufs_pyutils-0.1.1.tar.gz` & `tmp/ufs_pyutils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufs_pyutils-0.1.1.tar", last modified: Wed Jul 12 14:48:19 2023, max compression
+gzip compressed data, was "ufs_pyutils-0.1.2.tar", last modified: Wed Jul 12 14:53:31 2023, max compression
```

## Comparing `ufs_pyutils-0.1.1.tar` & `ufs_pyutils-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:19.431687 ufs_pyutils-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-12 14:48:08.000000 ufs_pyutils-0.1.1/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-12 14:48:08.000000 ufs_pyutils-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 14:48:19.431687 ufs_pyutils-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-12 14:48:08.000000 ufs_pyutils-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-12 14:48:19.431687 ufs_pyutils-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 14:48:08.000000 ufs_pyutils-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:19.427687 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:48:19.000000 ufs_pyutils-0.1.1/ufs_pyutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:31.240192 ufs_pyutils-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-12 14:53:21.000000 ufs_pyutils-0.1.2/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-12 14:53:21.000000 ufs_pyutils-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 14:53:31.240192 ufs_pyutils-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-12 14:53:21.000000 ufs_pyutils-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-12 14:53:31.240192 ufs_pyutils-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 14:53:21.000000 ufs_pyutils-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:31.240192 ufs_pyutils-0.1.2/ufs_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-12 14:53:31.000000 ufs_pyutils-0.1.2/ufs_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-12 14:53:31.000000 ufs_pyutils-0.1.2/ufs_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:53:31.000000 ufs_pyutils-0.1.2/ufs_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 14:53:31.000000 ufs_pyutils-0.1.2/ufs_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:53:31.000000 ufs_pyutils-0.1.2/ufs_pyutils.egg-info/top_level.txt
```

### Comparing `ufs_pyutils-0.1.1/INSTALL.md` & `ufs_pyutils-0.1.2/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ufs_pyutils-0.1.1/LICENSE` & `ufs_pyutils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ufs_pyutils-0.1.1/PKG-INFO` & `ufs_pyutils-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufs_pyutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Toolbox of API used for UFS applications.
 Home-page: https://github.com/HenryWinterbottom-NOAA/ufs_pyutils
 Author: "Henry R. Winterbottom"
 License: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ufs_pyutils-0.1.1/README.md` & `ufs_pyutils-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ufs_pyutils-0.1.1/setup.cfg` & `ufs_pyutils-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ufs_pyutils
-version = 0.1.1
+version = 0.1.2
 description = Python Toolbox of API used for UFS applications.
 long_description = file: INSTALL.md
 long_description_content_type = text/markdown
 author = "Henry R. Winterbottom"
 home_page = https://github.com/HenryWinterbottom-NOAA/ufs_pyutils
 license = GNU Lesser General Public License v2 (LGPLv2)
 classifiers =
```

### Comparing `ufs_pyutils-0.1.1/ufs_pyutils.egg-info/PKG-INFO` & `ufs_pyutils-0.1.2/ufs_pyutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufs-pyutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Toolbox of API used for UFS applications.
 Home-page: https://github.com/HenryWinterbottom-NOAA/ufs_pyutils
 Author: "Henry R. Winterbottom"
 License: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

