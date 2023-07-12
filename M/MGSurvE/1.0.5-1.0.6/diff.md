# Comparing `tmp/MGSurvE-1.0.5.tar.gz` & `tmp/MGSurvE-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-1.0.5.tar", last modified: Tue Jun 27 16:35:10 2023, max compression
+gzip compressed data, was "MGSurvE-1.0.6.tar", last modified: Wed Jul 12 17:28:32 2023, max compression
```

## Comparing `MGSurvE-1.0.5.tar` & `MGSurvE-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-27 16:35:10.545185 MGSurvE-1.0.5/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.5/LICENSE
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-27 16:35:10.543669 MGSurvE-1.0.5/MGSurvE/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.5/MGSurvE/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-06-27 16:35:10.000000 MGSurvE-1.0.5/MGSurvE/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.5/MGSurvE/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.5/MGSurvE/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-05-11 16:34:41.000000 MGSurvE-1.0.5/MGSurvE/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.5/MGSurvE/kernels.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21376 2023-06-08 23:51:28.000000 MGSurvE-1.0.5/MGSurvE/landscape.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.5/MGSurvE/matrices.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.5/MGSurvE/network.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-1.0.5/MGSurvE/optimization.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.5/MGSurvE/optimizationPSO.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18240 2023-06-26 18:31:03.000000 MGSurvE-1.0.5/MGSurvE/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.5/MGSurvE/pointProcess.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-27 16:35:10.544821 MGSurvE-1.0.5/MGSurvE.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4525 2023-06-27 16:35:10.000000 MGSurvE-1.0.5/MGSurvE.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-06-27 16:35:10.000000 MGSurvE-1.0.5/MGSurvE.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-06-27 16:35:10.000000 MGSurvE-1.0.5/MGSurvE.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      221 2023-06-27 16:35:10.000000 MGSurvE-1.0.5/MGSurvE.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-06-27 16:35:10.000000 MGSurvE-1.0.5/MGSurvE.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4525 2023-06-27 16:35:10.545036 MGSurvE-1.0.5/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4093 2023-06-26 23:13:33.000000 MGSurvE-1.0.5/README.md
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-06-27 16:35:10.545237 MGSurvE-1.0.5/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-06-08 23:51:28.000000 MGSurvE-1.0.5/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-12 17:28:32.521221 MGSurvE-1.0.6/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/LICENSE
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-12 17:28:32.520027 MGSurvE-1.0.6/MGSurvE/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.6/MGSurvE/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-06-29 19:56:26.000000 MGSurvE-1.0.6/MGSurvE/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.6/MGSurvE/kernels.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21376 2023-07-12 17:23:52.000000 MGSurvE-1.0.6/MGSurvE/landscape.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/matrices.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/network.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/optimization.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.6/MGSurvE/optimizationPSO.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18240 2023-07-12 17:23:30.000000 MGSurvE-1.0.6/MGSurvE/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/pointProcess.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-12 17:28:32.520840 MGSurvE-1.0.6/MGSurvE.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      231 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-12 17:28:32.521074 MGSurvE-1.0.6/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4172 2023-06-29 18:04:52.000000 MGSurvE-1.0.6/README.md
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-12 17:28:32.521280 MGSurvE-1.0.6/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1441 2023-06-28 20:50:45.000000 MGSurvE-1.0.6/setup.py
```

### Comparing `MGSurvE-1.0.5/LICENSE` & `MGSurvE-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE/auxiliary.py` & `MGSurvE-1.0.6/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE/colors.py` & `MGSurvE-1.0.6/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE/constants.py` & `MGSurvE-1.0.6/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE/kernels.py` & `MGSurvE-1.0.6/MGSurvE/kernels.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE/landscape.py` & `MGSurvE-1.0.6/MGSurvE/landscape.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
             alphaMin=alphaMin, alphaAmplitude=alphaAmplitude,
             zorder=zorder, **kwargs
         )
         return (fig, ax)
     def plotTraps(self,
             fig, ax, 
             colors=cst.TRP_COLS, marker="X",
-            edgecolor='w', lws=(2, 0), ls=':',
+            edgecolor='w', lws=(2, 1), ls=':',
             size=300, zorders=(25, -5),
             **kwargs
         ):
         """Plots the traps locations.
         """
         (fig, ax) = plt.plotTraps(
             fig, ax,
```

### Comparing `MGSurvE-1.0.5/MGSurvE/matrices.py` & `MGSurvE-1.0.6/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE/network.py` & `MGSurvE-1.0.6/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE/optimization.py` & `MGSurvE-1.0.6/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE/optimizationPSO.py` & `MGSurvE-1.0.6/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE/plots.py` & `MGSurvE-1.0.6/MGSurvE/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     return (fig, ax)
 
 
 def plotTraps(
         fig, ax,
         trapsCoords, trapsTypes, trapsKernels, trapsFixed,
         colors=cst.TRP_COLS, marker="X",
-        edgecolors=('w', 'k'), lws=(2, 0), ls=':',
+        edgecolors=('w', 'k'), lws=(2, 1), ls=':',
         size=350, zorders=(25, -5), fill=True,
         transform=None, transparencyHex='DD',
         latlon=False, proj=None,
         **kwargs
     ):
     """ Plots the traps with the radii of effectiveness.
```

### Comparing `MGSurvE-1.0.5/MGSurvE/pointProcess.py` & `MGSurvE-1.0.6/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.5/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-1.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,23 @@
-Metadata-Version: 2.1
-Name: MGSurvE
-Version: 1.0.5
-Summary: MGSurvE
-Home-page: https://github.com/Chipdelmal/MGSurvE
-Author: Hector M. Sanchez C.
-Author-email: sanchez.hmsc@berkeley.edu
-License: GPLv3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # MGSurvE: Mosquito Gene SurveillancE
 
 MGSurvE is a project that optimizes mosquito traps' placement in complex heterogeneous landscapes in an effort to minimize the time to detection of genetic variants of interest.
 
 Please have a look at the [documentation](https://chipdelmal.github.io/MGSurvE/) for more info and our [pypi](https://pypi.org/project/MGSurvE/) package for detailed [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html), and [tutorials](https://chipdelmal.github.io/MGSurvE/build/html/demos.html).
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MGSurvE)](https://pypi.org/project/MGSurvE/)
 [![PyPI version](https://badge.fury.io/py/MGSurvE.svg)](https://badge.fury.io/py/MGSurvE)
 [![Unit Tests](https://github.com/chipdelmal/MGSurvE/actions/workflows/PyTests.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/tree/main/MGSurvE/test)
 [![Flake8](https://github.com/chipdelmal/MGSurvE/actions/workflows/Flake8.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Flake8.yml)
 [![Conda](https://github.com/chipdelmal/MGSurvE/actions/workflows/Anaconda.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Anaconda.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Chipdelmal/MGSurvE)
+[<img src="https://img.shields.io/badge/dockerhub-img-blue.svg?logo=docker">](https://hub.docker.com/r/chipdelmal/mgsurve)
+[<img src="https://img.shields.io/badge/ReadThe-docs-E40046.svg?logo=readthedocs">](https://chipdelmal.github.io/MGSurvE/)
 [![DOI](https://zenodo.org/badge/423533276.svg)](https://zenodo.org/badge/latestdoi/423533276)
-<!-- [![Docker](https://img.shields.io/docker/v/chipdelmal/mgsurve?color=success&label=docker%20img)](https://hub.docker.com/repository/docker/chipdelmal/mgsurve)-->
-
 
 
 To install the package's latest stable version run (usage of [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html) for environment management is strongly recommended):
 
 ```
 pip install MGSurvE
 ```
```

### Comparing `MGSurvE-1.0.5/PKG-INFO` & `MGSurvE-1.0.6/MGSurvE.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.5
+Version: 1.0.6
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,17 +22,17 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MGSurvE)](https://pypi.org/project/MGSurvE/)
 [![PyPI version](https://badge.fury.io/py/MGSurvE.svg)](https://badge.fury.io/py/MGSurvE)
 [![Unit Tests](https://github.com/chipdelmal/MGSurvE/actions/workflows/PyTests.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/tree/main/MGSurvE/test)
 [![Flake8](https://github.com/chipdelmal/MGSurvE/actions/workflows/Flake8.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Flake8.yml)
 [![Conda](https://github.com/chipdelmal/MGSurvE/actions/workflows/Anaconda.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Anaconda.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Chipdelmal/MGSurvE)
+[<img src="https://img.shields.io/badge/dockerhub-img-blue.svg?logo=docker">](https://hub.docker.com/r/chipdelmal/mgsurve)
+[<img src="https://img.shields.io/badge/ReadThe-docs-E40046.svg?logo=readthedocs">](https://chipdelmal.github.io/MGSurvE/)
 [![DOI](https://zenodo.org/badge/423533276.svg)](https://zenodo.org/badge/latestdoi/423533276)
-<!-- [![Docker](https://img.shields.io/docker/v/chipdelmal/mgsurve?color=success&label=docker%20img)](https://hub.docker.com/repository/docker/chipdelmal/mgsurve)-->
-
 
 
 To install the package's latest stable version run (usage of [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html) for environment management is strongly recommended):
 
 ```
 pip install MGSurvE
 ```
```

### Comparing `MGSurvE-1.0.5/README.md` & `MGSurvE-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,38 @@
+Metadata-Version: 2.1
+Name: MGSurvE
+Version: 1.0.6
+Summary: MGSurvE
+Home-page: https://github.com/Chipdelmal/MGSurvE
+Author: Hector M. Sanchez C.
+Author-email: sanchez.hmsc@berkeley.edu
+License: GPLv3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # MGSurvE: Mosquito Gene SurveillancE
 
 MGSurvE is a project that optimizes mosquito traps' placement in complex heterogeneous landscapes in an effort to minimize the time to detection of genetic variants of interest.
 
 Please have a look at the [documentation](https://chipdelmal.github.io/MGSurvE/) for more info and our [pypi](https://pypi.org/project/MGSurvE/) package for detailed [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html), and [tutorials](https://chipdelmal.github.io/MGSurvE/build/html/demos.html).
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MGSurvE)](https://pypi.org/project/MGSurvE/)
 [![PyPI version](https://badge.fury.io/py/MGSurvE.svg)](https://badge.fury.io/py/MGSurvE)
 [![Unit Tests](https://github.com/chipdelmal/MGSurvE/actions/workflows/PyTests.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/tree/main/MGSurvE/test)
 [![Flake8](https://github.com/chipdelmal/MGSurvE/actions/workflows/Flake8.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Flake8.yml)
 [![Conda](https://github.com/chipdelmal/MGSurvE/actions/workflows/Anaconda.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Anaconda.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Chipdelmal/MGSurvE)
+[<img src="https://img.shields.io/badge/dockerhub-img-blue.svg?logo=docker">](https://hub.docker.com/r/chipdelmal/mgsurve)
+[<img src="https://img.shields.io/badge/ReadThe-docs-E40046.svg?logo=readthedocs">](https://chipdelmal.github.io/MGSurvE/)
 [![DOI](https://zenodo.org/badge/423533276.svg)](https://zenodo.org/badge/latestdoi/423533276)
-<!-- [![Docker](https://img.shields.io/docker/v/chipdelmal/mgsurve?color=success&label=docker%20img)](https://hub.docker.com/repository/docker/chipdelmal/mgsurve)-->
-
 
 
 To install the package's latest stable version run (usage of [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html) for environment management is strongly recommended):
 
 ```
 pip install MGSurvE
 ```
```

### Comparing `MGSurvE-1.0.5/setup.py` & `MGSurvE-1.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
         'deap', 'numpy', 'scikit-learn', 'scipy', 'matplotlib', 'sympy',
         'ipython', 'jupyter', 'pandas', 'compress-pickle', 'dill', 
         'vincenty', 'haversine', 'networkx', 'pointpats', 'libpysal',
-        'geopandas', 'sympy'
+        'geopandas', 'sympy', 'termcolor'
     ],
     extras_require={
         'dev': [
             'pytest', 'ipykernel'
             'twine', 'wheel', 
             'sphinx', 'sphinx_rtd_theme', 'chardet'
         ],
```

