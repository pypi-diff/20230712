# Comparing `tmp/read5-1.1.3.tar.gz` & `tmp/read5-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read5-1.1.3.tar", last modified: Wed Jul 12 13:01:17 2023, max compression
+gzip compressed data, was "read5-1.1.5.tar", last modified: Wed Jul 12 13:10:41 2023, max compression
```

## Comparing `read5-1.1.3.tar` & `read5-1.1.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:01:17.915694 read5-1.1.3/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    35149 2023-04-26 15:37:10.000000 read5-1.1.3/LICENSE
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       22 2023-04-26 15:39:17.000000 read5-1.1.3/MANIFEST.in
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      749 2023-07-12 13:01:17.919694 read5-1.1.3/PKG-INFO
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2540 2023-07-12 12:54:27.000000 read5-1.1.3/README.md
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:01:17.927694 read5-1.1.3/read5/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    20135 2023-07-12 12:37:48.000000 read5-1.1.3/read5/AbstractFileReader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      773 2023-05-02 14:53:52.000000 read5-1.1.3/read5/Exceptions.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    13183 2023-07-12 12:39:21.000000 read5-1.1.3/read5/Fast5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    11653 2023-07-12 12:38:39.000000 read5-1.1.3/read5/Pod5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      980 2023-07-12 12:52:52.000000 read5-1.1.3/read5/Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     8605 2023-07-12 12:39:08.000000 read5-1.1.3/read5/Slow5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      148 2023-07-12 12:47:33.000000 read5-1.1.3/read5/__init__.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      497 2023-07-12 13:01:17.927694 read5-1.1.3/read5/_version.py
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:01:17.899694 read5-1.1.3/read5.egg-info/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      749 2023-07-12 13:01:17.000000 read5-1.1.3/read5.egg-info/PKG-INFO
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      393 2023-07-12 13:01:17.000000 read5-1.1.3/read5.egg-info/SOURCES.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        1 2023-07-12 13:01:17.000000 read5-1.1.3/read5.egg-info/dependency_links.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       62 2023-07-12 13:01:17.000000 read5-1.1.3/read5.egg-info/requires.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        6 2023-07-12 13:01:17.000000 read5-1.1.3/read5.egg-info/top_level.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      208 2023-07-12 13:01:17.923694 read5-1.1.3/setup.cfg
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1239 2023-07-12 13:00:17.000000 read5-1.1.3/setup.py
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:01:17.907694 read5-1.1.3/tests/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    54377 2023-07-12 12:51:42.000000 read5-1.1.3/tests/test_FileReader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    68611 2023-04-26 15:39:17.000000 read5-1.1.3/versioneer.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:10:41.818770 read5-1.1.5/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    35149 2023-04-26 15:37:10.000000 read5-1.1.5/LICENSE
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       22 2023-04-26 15:39:17.000000 read5-1.1.5/MANIFEST.in
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2210 2023-07-12 13:10:41.818770 read5-1.1.5/PKG-INFO
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2634 2023-07-12 13:03:46.000000 read5-1.1.5/README.md
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1459 2023-07-12 13:09:27.000000 read5-1.1.5/README.rst
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:10:41.830770 read5-1.1.5/read5/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    20135 2023-07-12 12:37:48.000000 read5-1.1.5/read5/AbstractFileReader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      773 2023-05-02 14:53:52.000000 read5-1.1.5/read5/Exceptions.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    13183 2023-07-12 12:39:21.000000 read5-1.1.5/read5/Fast5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    11653 2023-07-12 12:38:39.000000 read5-1.1.5/read5/Pod5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      980 2023-07-12 12:52:52.000000 read5-1.1.5/read5/Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     8605 2023-07-12 12:39:08.000000 read5-1.1.5/read5/Slow5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      148 2023-07-12 12:47:33.000000 read5-1.1.5/read5/__init__.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      497 2023-07-12 13:10:41.830770 read5-1.1.5/read5/_version.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:10:41.794770 read5-1.1.5/read5.egg-info/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2210 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/PKG-INFO
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      404 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/SOURCES.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        1 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/dependency_links.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       62 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/requires.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        6 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/top_level.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      208 2023-07-12 13:10:41.826770 read5-1.1.5/setup.cfg
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1350 2023-07-12 13:09:49.000000 read5-1.1.5/setup.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:10:41.806770 read5-1.1.5/tests/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    54377 2023-07-12 12:51:42.000000 read5-1.1.5/tests/test_FileReader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    68611 2023-04-26 15:39:17.000000 read5-1.1.5/versioneer.py
```

### Comparing `read5-1.1.3/LICENSE` & `read5-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `read5-1.1.3/README.md` & `read5-1.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # ![Alt text](figures/logo.png)
 
 Read5 is a python wrapper to read fast5, slow5/blow5 and pod5 files using the same overloaded functions from different APIs.
 
-[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-teal.svg)](https://www.gnu.org/licenses/gpl-3.0)![Python3.9](https://img.shields.io/badge/Language-Python_3.9-darkred.svg)![conda](https://img.shields.io/badge/Uses-conda-green.svg)
+[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-teal.svg)](https://www.gnu.org/licenses/gpl-3.0)
+![Python3](https://img.shields.io/badge/Language-Python_3-darkred.svg)
 
-[![Anaconda-Server Badge](https://anaconda.org/jannessp/read5/badges/version.svg)](https://anaconda.org/jannessp/read5) ![Conda](https://img.shields.io/conda/dn/jannessp/read5)
-[![Conda package](https://anaconda.org/jannessp/read5/badges/latest_release_date.svg)](https://anaconda.org/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/platforms.svg)](https://anaconda.org/jannessp/read5)
+[![PyPI version](https://badge.fury.io/py/read5.svg)](https://badge.fury.io/py/read5)
+
+<!-- ![conda](https://img.shields.io/badge/Uses-conda-green.svg) [![Anaconda-Server Badge](https://anaconda.org/jannessp/read5/badges/version.svg)](https://anaconda.org/jannessp/read5) ![Conda](https://img.shields.io/conda/dn/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/latest_release_date.svg)](https://anaconda.org/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/platforms.svg)](https://anaconda.org/jannessp/read5) -->
  
 [![DOI](https://zenodo.org/badge/633012569.svg)](https://zenodo.org/badge/latestdoi/633012569)
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/Ja_Spangenberg)](https://twitter.com/Ja_Spangenberg)
 ___
 ## Table of Content
 1.  [Installation](#installation)
```

### Comparing `read5-1.1.3/read5/AbstractFileReader.py` & `read5-1.1.5/read5/AbstractFileReader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.3/read5/Exceptions.py` & `read5-1.1.5/read5/Exceptions.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.3/read5/Fast5Reader.py` & `read5-1.1.5/read5/Fast5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.3/read5/Pod5Reader.py` & `read5-1.1.5/read5/Pod5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.3/read5/Reader.py` & `read5-1.1.5/read5/Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.3/read5/Slow5Reader.py` & `read5-1.1.5/read5/Slow5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.3/setup.py` & `read5-1.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,19 +7,23 @@
     # 'ont_vbz_hdf_plugin>=1.0',
     'vbz-h5py-plugin>=1.0', # same as ont_vbz but in pipy
     'pyslow5>=1.0',
     'numpy',
     'pod5>=0.2.3', # currently only avaible via pipy
 ]
 
+with open("README.rst", "r") as rst:
+    long_description = rst.read()
+
 setup(
     name='read5',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description="Wrapper to read fast5, slow5, blow5 and pod5 files.",
+    long_description=long_description,
     license="GNU General Public License v3",
     author="Jannes Spangenberg",
     author_email='jannes.spangenberg@uni-jena.de',
     url='https://github.com/JannesSP/read5',
     packages=find_packages(),
     install_requires=requirements,
     keywords=['read5', 'slow5', 'blow5', 'fast5', 'pod5', 'ONT', 'Oxford Nanopore Technologies', 'Nanopore', 'raw data', 'wrapper'],
```

### Comparing `read5-1.1.3/tests/test_FileReader.py` & `read5-1.1.5/tests/test_FileReader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.3/versioneer.py` & `read5-1.1.5/versioneer.py`

 * *Files identical despite different names*

