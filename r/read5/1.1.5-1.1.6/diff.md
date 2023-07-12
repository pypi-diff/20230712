# Comparing `tmp/read5-1.1.5.tar.gz` & `tmp/read5-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read5-1.1.5.tar", last modified: Wed Jul 12 13:10:41 2023, max compression
+gzip compressed data, was "read5-1.1.6.tar", last modified: Wed Jul 12 21:34:07 2023, max compression
```

## Comparing `read5-1.1.5.tar` & `read5-1.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:10:41.818770 read5-1.1.5/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    35149 2023-04-26 15:37:10.000000 read5-1.1.5/LICENSE
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       22 2023-04-26 15:39:17.000000 read5-1.1.5/MANIFEST.in
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2210 2023-07-12 13:10:41.818770 read5-1.1.5/PKG-INFO
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2634 2023-07-12 13:03:46.000000 read5-1.1.5/README.md
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1459 2023-07-12 13:09:27.000000 read5-1.1.5/README.rst
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:10:41.830770 read5-1.1.5/read5/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    20135 2023-07-12 12:37:48.000000 read5-1.1.5/read5/AbstractFileReader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      773 2023-05-02 14:53:52.000000 read5-1.1.5/read5/Exceptions.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    13183 2023-07-12 12:39:21.000000 read5-1.1.5/read5/Fast5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    11653 2023-07-12 12:38:39.000000 read5-1.1.5/read5/Pod5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      980 2023-07-12 12:52:52.000000 read5-1.1.5/read5/Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     8605 2023-07-12 12:39:08.000000 read5-1.1.5/read5/Slow5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      148 2023-07-12 12:47:33.000000 read5-1.1.5/read5/__init__.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      497 2023-07-12 13:10:41.830770 read5-1.1.5/read5/_version.py
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:10:41.794770 read5-1.1.5/read5.egg-info/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2210 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/PKG-INFO
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      404 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/SOURCES.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        1 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/dependency_links.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       62 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/requires.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        6 2023-07-12 13:10:41.000000 read5-1.1.5/read5.egg-info/top_level.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      208 2023-07-12 13:10:41.826770 read5-1.1.5/setup.cfg
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1350 2023-07-12 13:09:49.000000 read5-1.1.5/setup.py
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 13:10:41.806770 read5-1.1.5/tests/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    54377 2023-07-12 12:51:42.000000 read5-1.1.5/tests/test_FileReader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    68611 2023-04-26 15:39:17.000000 read5-1.1.5/versioneer.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 21:34:07.435057 read5-1.1.6/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    35149 2023-04-26 15:37:10.000000 read5-1.1.6/LICENSE
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       22 2023-04-26 15:39:17.000000 read5-1.1.6/MANIFEST.in
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2328 2023-07-12 21:34:07.435057 read5-1.1.6/PKG-INFO
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3382 2023-07-12 21:30:22.000000 read5-1.1.6/README.md
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1459 2023-07-12 13:09:27.000000 read5-1.1.6/README.rst
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 21:34:07.451057 read5-1.1.6/read5/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    20135 2023-07-12 12:37:48.000000 read5-1.1.6/read5/AbstractFileReader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      773 2023-07-12 15:11:37.000000 read5-1.1.6/read5/Exceptions.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    13183 2023-07-12 12:39:21.000000 read5-1.1.6/read5/Fast5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    11653 2023-07-12 12:38:39.000000 read5-1.1.6/read5/Pod5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      980 2023-07-12 12:52:52.000000 read5-1.1.6/read5/Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     8605 2023-07-12 12:39:08.000000 read5-1.1.6/read5/Slow5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      148 2023-07-12 12:47:33.000000 read5-1.1.6/read5/__init__.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      497 2023-07-12 21:34:07.451057 read5-1.1.6/read5/_version.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 21:34:07.415057 read5-1.1.6/read5.egg-info/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2328 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/PKG-INFO
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      404 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/SOURCES.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        1 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/dependency_links.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       88 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/requires.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        6 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/top_level.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      208 2023-07-12 21:34:07.443057 read5-1.1.6/setup.cfg
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1519 2023-07-12 21:25:01.000000 read5-1.1.6/setup.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 21:34:07.423057 read5-1.1.6/tests/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    54377 2023-07-12 12:51:42.000000 read5-1.1.6/tests/test_FileReader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    68611 2023-04-26 15:39:17.000000 read5-1.1.6/versioneer.py
```

### Comparing `read5-1.1.5/LICENSE` & `read5-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `read5-1.1.5/PKG-INFO` & `read5-1.1.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: read5
-Version: 1.1.5
+Version: 1.1.6
 Summary: Wrapper to read fast5, slow5, blow5 and pod5 files.
 Home-page: https://github.com/JannesSP/read5
 Author: Jannes Spangenberg
 Author-email: jannes.spangenberg@uni-jena.de
 License: GNU General Public License v3
 Keywords: read5,slow5,blow5,fast5,pod5,ONT,Oxford Nanopore Technologies,Nanopore,raw data,wrapper
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE
 
 Installation
 ------------
 
 Pod5 is not available via conda (27.06.2023). Read5 Currently available
 via pipy.
```

### Comparing `read5-1.1.5/README.md` & `read5-1.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 # ![Alt text](figures/logo.png)
 
 Read5 is a python wrapper to read fast5, slow5/blow5 and pod5 files using the same overloaded functions from different APIs.
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-teal.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![Python3](https://img.shields.io/badge/Language-Python_3-darkred.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/read5)
 
-[![PyPI version](https://badge.fury.io/py/read5.svg)](https://badge.fury.io/py/read5)
+[![PyPI version](https://badge.fury.io/py/read5.svg)](https://badge.fury.io/py/read5) ![PyPI - Downloads](https://img.shields.io/pypi/dm/read5) ![PyPI - Status](https://img.shields.io/pypi/status/read5)
 
-<!-- ![conda](https://img.shields.io/badge/Uses-conda-green.svg) [![Anaconda-Server Badge](https://anaconda.org/jannessp/read5/badges/version.svg)](https://anaconda.org/jannessp/read5) ![Conda](https://img.shields.io/conda/dn/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/latest_release_date.svg)](https://anaconda.org/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/platforms.svg)](https://anaconda.org/jannessp/read5) -->
+
+[![Anaconda-Server Badge](https://anaconda.org/jannessp/read5/badges/version.svg)](https://anaconda.org/jannessp/read5) ![Conda](https://img.shields.io/conda/dn/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/latest_release_date.svg)](https://anaconda.org/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/platforms.svg)](https://anaconda.org/jannessp/read5)
  
 [![DOI](https://zenodo.org/badge/633012569.svg)](https://zenodo.org/badge/latestdoi/633012569)
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/Ja_Spangenberg)](https://twitter.com/Ja_Spangenberg)
 ___
 ## Table of Content
 1.  [Installation](#installation)
 2.  [Usage](#usage)
 3.  [Full Documentation](https://jannessp.github.io/read5.github.io/)
 ___
 ## Installation
 
-Pod5 is not available via conda (27.06.2023).
-Read5 Currently available via pipy.
-
+### Pypi/pip
 ```bash
 pip install read5
 ```
+### Conda
+Pod5 is currently not available via conda (27.06.2023). Please install it using pip in your conda environment.
+```bash
+conda install mamba
+mamba create -n read5 -c jannessp read5
+conda activate read5
+pip install pod5 # needed as no pod5 conda package available yet
+```
 ___
 ## Usage
 
 [Click here to see a full documentation about the classes and function.](https://jannessp.github.io/read5.github.io/)
 
 *my_file* can be a fast5, slow5, blow5 or pod5 file. The wrapper detects the file format depending on the file extension.
 
-Small example:
+### Small example:
 
 ```python
 from read5 import read # or from read5.Reader import read
 
 r5 = read(my_file) # file with on of these extensions: .fast5, .slow5, .blow5, .pod5
 for readid in r5:
     signal = r5.getSignal(readid)
@@ -45,18 +52,34 @@
     channel = r5.getChannelNumber(readid)
     sampleid = r5.getSampleID(readid)
     runid = r5.getSampleID(readid)
 
 readid_list = r5.getReads()
 ```
 
+### File Reader Classes
 If you want to use the file readers you can import the corresponding class like this:
 
 ```python
 from read5.Fast5Reader import Fast5Reader # contains the Fast5 Reader class
 from read5.Slow5Reader import Slow5Reader # contains the Slow5 Reader class
 from read5.Pod5Reader import Pod5Reader # contains the Pod5 Reader class
 ```
 
+### Abstract File Reader Class
+
+```python
+from read5.AbstractFileReader import AbstractFileReader
+```
+
+### Possible Exceptions
+
+```python
+from read5.Exceptions import UnknownFileFormatException, UnknownNormalizationMode
+```
+
+- UnknownFileFormatException: is raised, when the file extension does not match one of ['.fast5', '.slow5', '.blow5', 'pod5']
+- UnknownNormalizationMode: is raised, when an unknown mode is provided for the signal normalization function
+
 ## Full Documentation
 Created with [pdoc3](https://pdoc3.github.io/pdoc/).
 Can be found [here](https://jannessp.github.io/read5.github.io/).
```

### Comparing `read5-1.1.5/README.rst` & `read5-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `read5-1.1.5/read5/AbstractFileReader.py` & `read5-1.1.6/read5/AbstractFileReader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.5/read5/Exceptions.py` & `read5-1.1.6/read5/Exceptions.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.5/read5/Fast5Reader.py` & `read5-1.1.6/read5/Fast5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.5/read5/Pod5Reader.py` & `read5-1.1.6/read5/Pod5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.5/read5/Reader.py` & `read5-1.1.6/read5/Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.5/read5/Slow5Reader.py` & `read5-1.1.6/read5/Slow5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.5/read5.egg-info/PKG-INFO` & `read5-1.1.6/read5.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: read5
-Version: 1.1.5
+Version: 1.1.6
 Summary: Wrapper to read fast5, slow5, blow5 and pod5 files.
 Home-page: https://github.com/JannesSP/read5
 Author: Jannes Spangenberg
 Author-email: jannes.spangenberg@uni-jena.de
 License: GNU General Public License v3
 Keywords: read5,slow5,blow5,fast5,pod5,ONT,Oxford Nanopore Technologies,Nanopore,raw data,wrapper
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE
 
 Installation
 ------------
 
 Pod5 is not available via conda (27.06.2023). Read5 Currently available
 via pipy.
```

### Comparing `read5-1.1.5/setup.py` & `read5-1.1.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from setuptools import setup, find_packages
 import versioneer
 
+# conda
+# requirements = [
+#     'python',
+#     'h5py>=3.8',
+#     'ont_vbz_hdf_plugin>=1.0',
+#     'pyslow5>=1.0.0',
+#     'numpy>=1.20',
+# ]
+
+# pipy
 requirements = [
-    # package requirements go here
+    'python>=3.8,<3.11',
     'h5py>=3.0',
-    # 'ont_vbz_hdf_plugin>=1.0',
-    'vbz-h5py-plugin>=1.0', # same as ont_vbz but in pipy
-    'pyslow5>=1.0',
-    'numpy',
-    'pod5>=0.2.3', # currently only avaible via pipy
+    'vbz-h5py-plugin>=1.0',
+    'pyslow5>=1.0.0',
+    'numpy>=1.20',
+    'pod5>=0.2.3',
 ]
 
 with open("README.rst", "r") as rst:
     long_description = rst.read()
 
 setup(
     name='read5',
@@ -24,16 +33,18 @@
     author="Jannes Spangenberg",
     author_email='jannes.spangenberg@uni-jena.de',
     url='https://github.com/JannesSP/read5',
     packages=find_packages(),
     install_requires=requirements,
     keywords=['read5', 'slow5', 'blow5', 'fast5', 'pod5', 'ONT', 'Oxford Nanopore Technologies', 'Nanopore', 'raw data', 'wrapper'],
     classifiers=[
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
+        'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
+        'Topic :: Scientific/Engineering :: Bio-Informatics',
     ]
 )
```

### Comparing `read5-1.1.5/tests/test_FileReader.py` & `read5-1.1.6/tests/test_FileReader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.5/versioneer.py` & `read5-1.1.6/versioneer.py`

 * *Files identical despite different names*

