# Comparing `tmp/mcemtools-0.4.0.tar.gz` & `tmp/mcemtools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.4.0.tar", last modified: Tue Jul 11 11:10:54 2023, max compression
+gzip compressed data, was "mcemtools-0.5.0.tar", last modified: Wed Jul 12 04:56:10 2023, max compression
```

## Comparing `mcemtools-0.4.0.tar` & `mcemtools-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:54.493888 mcemtools-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 11:10:41.000000 mcemtools-0.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-11 11:10:41.000000 mcemtools-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-11 11:10:41.000000 mcemtools-0.4.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 11:10:41.000000 mcemtools-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-11 11:10:41.000000 mcemtools-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-11 11:10:54.493888 mcemtools-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-11 11:10:41.000000 mcemtools-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:54.493888 mcemtools-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 11:10:41.000000 mcemtools-0.4.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:54.493888 mcemtools-0.4.0/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 11:10:41.000000 mcemtools-0.4.0/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-11 11:10:41.000000 mcemtools-0.4.0/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-11 11:10:41.000000 mcemtools-0.4.0/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-11 11:10:41.000000 mcemtools-0.4.0/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-11 11:10:41.000000 mcemtools-0.4.0/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-07-11 11:10:41.000000 mcemtools-0.4.0/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-11 11:10:41.000000 mcemtools-0.4.0/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:54.493888 mcemtools-0.4.0/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-11 11:10:54.000000 mcemtools-0.4.0/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 11:10:54.000000 mcemtools-0.4.0/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:10:54.000000 mcemtools-0.4.0/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 11:10:54.000000 mcemtools-0.4.0/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:10:54.000000 mcemtools-0.4.0/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 11:10:54.000000 mcemtools-0.4.0/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 11:10:54.000000 mcemtools-0.4.0/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 11:10:41.000000 mcemtools-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 11:10:54.493888 mcemtools-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 11:10:41.000000 mcemtools-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:54.493888 mcemtools-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 11:10:41.000000 mcemtools-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-11 11:10:41.000000 mcemtools-0.4.0/tests/test_mcemtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 04:55:58.000000 mcemtools-0.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-12 04:55:58.000000 mcemtools-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-12 04:55:58.000000 mcemtools-0.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 04:55:58.000000 mcemtools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-12 04:55:58.000000 mcemtools-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-12 04:56:10.543545 mcemtools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-12 04:55:58.000000 mcemtools-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 04:55:58.000000 mcemtools-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 04:56:10.543545 mcemtools-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-12 04:55:58.000000 mcemtools-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 04:55:58.000000 mcemtools-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-12 04:55:58.000000 mcemtools-0.5.0/tests/test_mcemtools.py
```

### Comparing `mcemtools-0.4.0/CONTRIBUTING.rst` & `mcemtools-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.4.0/LICENSE` & `mcemtools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.4.0/PKG-INFO` & `mcemtools-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.4.0
+Version: 0.5.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -85,7 +85,11 @@
 * Tests are increasing in number
 * init includes import of mcemtools
 
 0.4.0 (2023-07-11)
 ------------------
 
 * Many small bugs are fixed
+
+0.5.0 (2023-07-12)
+------------------
+* Added binning to transforms
```

### Comparing `mcemtools-0.4.0/README.rst` & `mcemtools-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.4.0/docs/Makefile` & `mcemtools-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.4.0/docs/conf.py` & `mcemtools-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.4.0/docs/installation.rst` & `mcemtools-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.4.0/docs/make.bat` & `mcemtools-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.4.0/mcemtools/masking.py` & `mcemtools-0.5.0/mcemtools/masking.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import matplotlib.pyplot as plt
 from matplotlib.widgets import RangeSlider, Slider
 from lognflow import select_file
 import numpy as np
 
+def mask2D_to_4D(mask2D, data4D_shape):
+    n_x, n_y, n_r, n_c = data4D_shape
+    assert len(mask2D.shape) == 2, 'mask should be 2d'
+    assert mask2D.shape[0] == n_r, 'mask should have same shape as patterns'
+    assert mask2D.shape[1] == n_c, 'mask should have same shape as patterns'
+        
+    _mask4D = np.array([np.array([mask2D.copy()])])
+    _mask4D = np.tile(_mask4D, (n_x, n_y, 1, 1))
+    return _mask4D
+
 def annular_mask(image_shape : tuple, 
                  center:tuple = None, radius:float=None, in_radius:float=None):
     """make a circle bianry pattern in a given window
     This simple function makes a circle filled with ones for where the circle is
     in a window and leaves the rest of the elements to remain zero.
     Parameters
     ----------
```

### Comparing `mcemtools-0.4.0/mcemtools/tensor_svd.py` & `mcemtools-0.5.0/mcemtools/tensor_svd.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     1. Roughly estimate noise level and determine the number of iterations to use in HOOI algorithm.
     2. Atuomatically determine denoising ranks from eigenvalues.
     """
     # Case when SVD ranks are fed in the input, call svd_HO function to denoise
 
     if len(data.shape) == 3:  # hyperspectral data case, directly feed data to svd_HO function
         [X, _, _] = svd_HO(data, rank)
-    if len(data.shape) == 4:    # Original 4D STEM data case, unfold reciprocal space dimensions into one dimension then feed to svd_HO function
+    if len(data.shape) == 4:
         data = np.reshape(data, [data.shape[0], data.shape[1], data.shape[2]*data.shape[3]])
         [X, _, _] = svd_HO(data, rank)
     
     return X
```

### Comparing `mcemtools-0.4.0/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.5.0/mcemtools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.4.0
+Version: 0.5.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -85,7 +85,11 @@
 * Tests are increasing in number
 * init includes import of mcemtools
 
 0.4.0 (2023-07-11)
 ------------------
 
 * Many small bugs are fixed
+
+0.5.0 (2023-07-12)
+------------------
+* Added binning to transforms
```

### Comparing `mcemtools-0.4.0/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.5.0/mcemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcemtools-0.4.0/setup.py` & `mcemtools-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
```

