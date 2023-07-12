# Comparing `tmp/pylib_essentials-0.0.2.tar.gz` & `tmp/pylib_essentials-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylib_essentials-0.0.2.tar", last modified: Wed Jul 12 20:47:45 2023, max compression
+gzip compressed data, was "pylib_essentials-0.0.3.tar", last modified: Wed Jul 12 21:16:49 2023, max compression
```

## Comparing `pylib_essentials-0.0.2.tar` & `pylib_essentials-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 20:47:45.840634 pylib_essentials-0.0.2/
--rw-r--r--   0 feiye    (49086) vims     (50001)      218 2023-07-12 20:47:45.830634 pylib_essentials-0.0.2/PKG-INFO
--rw-r--r--   0 feiye    (49086) vims     (50001)      292 2023-06-12 21:54:20.000000 pylib_essentials-0.0.2/README.md
-drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 20:47:45.667633 pylib_essentials-0.0.2/pylib_essentials/
--rw-r--r--   0 feiye    (49086) vims     (50001)        0 2023-06-13 06:47:18.000000 pylib_essentials-0.0.2/pylib_essentials/__init__.py
--rw-r--r--   0 feiye    (49086) vims     (50001)   184895 2023-07-11 15:23:30.000000 pylib_essentials-0.0.2/pylib_essentials/schism_file.py
-drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 20:47:45.826634 pylib_essentials-0.0.2/pylib_essentials.egg-info/
--rw-r--r--   0 feiye    (49086) vims     (50001)      218 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/PKG-INFO
--rw-r--r--   0 feiye    (49086) vims     (50001)      278 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/SOURCES.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)        1 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/dependency_links.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)       42 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/requires.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)       17 2023-07-12 20:47:45.000000 pylib_essentials-0.0.2/pylib_essentials.egg-info/top_level.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)       38 2023-07-12 20:47:45.840634 pylib_essentials-0.0.2/setup.cfg
--rw-r--r--   0 feiye    (49086) vims     (50001)      391 2023-07-12 20:47:40.000000 pylib_essentials-0.0.2/setup.py
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 21:16:49.789196 pylib_essentials-0.0.3/
+-rw-r--r--   0 feiye    (49086) vims     (50001)      218 2023-07-12 21:16:49.788196 pylib_essentials-0.0.3/PKG-INFO
+-rw-r--r--   0 feiye    (49086) vims     (50001)      292 2023-06-12 21:54:20.000000 pylib_essentials-0.0.3/README.md
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 21:16:49.449194 pylib_essentials-0.0.3/pylib_essentials/
+-rw-r--r--   0 feiye    (49086) vims     (50001)        0 2023-06-13 06:47:18.000000 pylib_essentials-0.0.3/pylib_essentials/__init__.py
+-rw-r--r--   0 feiye    (49086) vims     (50001)   184978 2023-07-12 21:14:37.000000 pylib_essentials-0.0.3/pylib_essentials/schism_file.py
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 21:16:49.760196 pylib_essentials-0.0.3/pylib_essentials.egg-info/
+-rw-r--r--   0 feiye    (49086) vims     (50001)      218 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/PKG-INFO
+-rw-r--r--   0 feiye    (49086) vims     (50001)      278 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/SOURCES.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)        1 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/dependency_links.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       42 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/requires.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       17 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/top_level.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       38 2023-07-12 21:16:49.790196 pylib_essentials-0.0.3/setup.cfg
+-rw-r--r--   0 feiye    (49086) vims     (50001)      391 2023-07-12 21:15:35.000000 pylib_essentials-0.0.3/setup.py
```

### Comparing `pylib_essentials-0.0.2/pylib_essentials/schism_file.py` & `pylib_essentials-0.0.3/pylib_essentials/schism_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     tricontourf, tripcolor, colorbar, gca, gcf, plot, axis, xlim, ylim,\
     triplot, title, xlabel, ylabel, gca, gcf, setp, getp, close
 import matplotlib.cm as cm
 import matplotlib as mpl
 try:
     from pylib_utils.utility_functions import proj
 except:
-    print("projection module not found; install pylib_utils")
+    try:
+        from pylib.utility_functions import proj
+    except:
+        print("projection module not found; install pylib_utils or pylib")
 
 # for experimental features
 import numpy as np
 import pickle
 import pandas as pd
 import copy
 import scipy
```

