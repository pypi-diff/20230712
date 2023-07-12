# Comparing `tmp/dfm_tools-0.12.0.tar.gz` & `tmp/dfm_tools-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfm_tools-0.12.0.tar", last modified: Fri Jul  7 15:39:56 2023, max compression
+gzip compressed data, was "dfm_tools-0.13.0.tar", last modified: Wed Jul 12 14:47:17 2023, max compression
```

## Comparing `dfm_tools-0.12.0.tar` & `dfm_tools-0.13.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2353 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/dfm_tools/
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/bathymetry.py
--rw-r--r--   0 runner    (1001) docker     (122)     4140 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/coastlines.py
--rw-r--r--   0 runner    (1001) docker     (122)     4227 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    17494 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/energy_dissipation.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    28537 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/get_nc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9793 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/get_nc_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    21311 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/hydrolib_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    35184 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/interpolate_grid2bnd.py
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/linebuilder.py
--rw-r--r--   0 runner    (1001) docker     (122)    12273 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/meshkernel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/modelbuilder.py
--rw-r--r--   0 runner    (1001) docker     (122)    23929 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/modplot.py
--rw-r--r--   0 runner    (1001) docker     (122)    19385 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/xarray_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    17957 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/xugrid_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/dfm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15155 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/test_dfm_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/test_external_packages.py
--rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/test_meshkernel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:47:17.939365 dfm_tools-0.13.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-07-12 14:47:17.939365 dfm_tools-0.13.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:47:17.935365 dfm_tools-0.13.0/dfm_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/bathymetry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/coastlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8027 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4227 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18111 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/energy_dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28537 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/get_nc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9793 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/get_nc_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21311 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/hydrolib_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35184 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/interpolate_grid2bnd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/linebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12357 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/meshkernel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/modelbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23929 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/modplot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19385 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/xarray_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17957 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/dfm_tools/xugrid_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:47:17.939365 dfm_tools-0.13.0/dfm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-07-12 14:47:17.000000 dfm_tools-0.13.0/dfm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-12 14:47:17.000000 dfm_tools-0.13.0/dfm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 14:47:17.000000 dfm_tools-0.13.0/dfm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 14:47:17.000000 dfm_tools-0.13.0/dfm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-07-12 14:47:17.000000 dfm_tools-0.13.0/dfm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-12 14:47:17.000000 dfm_tools-0.13.0/dfm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-12 14:47:17.943365 dfm_tools-0.13.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:47:17.939365 dfm_tools-0.13.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/tests/test_coastlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13760 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/tests/test_dfm_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4051 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/tests/test_external_packages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-07-12 14:47:04.000000 dfm_tools-0.13.0/tests/test_meshkernel_helpers.py
```

### Comparing `dfm_tools-0.12.0/PKG-INFO` & `dfm_tools-0.13.0/dfm_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dfm_tools
-Version: 0.12.0
+Name: dfm-tools
+Version: 0.13.0
 Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
 Home-page: https://github.com/Deltares/dfm_tools
 Author: Jelmer Veenstra
 Author-email: Jelmer.Veenstra@Deltares.nl
 License: GNU General Public License v3 (GPLv3)
 Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 
 [![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
 [![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
 [![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
 [![pytest-py311](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml)
 [![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD?urlpath=/tree/docs/notebooks)
 [![Available on pypi](https://img.shields.io/pypi/v/dfm_tools.svg)](https://pypi.python.org/pypi/dfm_tools)
 [![Supported versions](https://img.shields.io/pypi/pyversions/dfm_tools.svg)](https://pypi.org/project/dfm_tools)
 [![Downloads](https://img.shields.io/pypi/dm/dfm_tools.svg)](https://pypistats.org/packages/dfm_tools)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7857393.svg)](https://doi.org/10.5281/zenodo.7857393)
 
 # dfm_tools
```

### Comparing `dfm_tools-0.12.0/README.md` & `dfm_tools-0.13.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
 [![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
 [![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
 [![pytest-py311](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml)
 [![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD?urlpath=/tree/docs/notebooks)
 [![Available on pypi](https://img.shields.io/pypi/v/dfm_tools.svg)](https://pypi.python.org/pypi/dfm_tools)
 [![Supported versions](https://img.shields.io/pypi/pyversions/dfm_tools.svg)](https://pypi.org/project/dfm_tools)
 [![Downloads](https://img.shields.io/pypi/dm/dfm_tools.svg)](https://pypistats.org/packages/dfm_tools)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7857393.svg)](https://doi.org/10.5281/zenodo.7857393)
 
 # dfm_tools
```

### Comparing `dfm_tools-0.12.0/dfm_tools/__init__.py` & `dfm_tools-0.13.0/dfm_tools/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 .. include:: ../README.md
 """
 
 __author__ = """Jelmer Veenstra"""
 __email__ = 'jelmer.veenstra@deltares.nl'
-__version__ = '0.12.0'
+__version__ = '0.13.0'
 
 from dfm_tools.deprecated import *
 from dfm_tools.errors import *
 from dfm_tools.download import *
 from dfm_tools.get_nc import *
 from dfm_tools.get_nc_helpers import *
 from dfm_tools.hydrolib_helpers import *
@@ -17,11 +17,12 @@
 from dfm_tools.linebuilder import *
 from dfm_tools.modplot import *
 from dfm_tools.xarray_helpers import *
 from dfm_tools.xugrid_helpers import *
 from dfm_tools.energy_dissipation import *
 from dfm_tools.bathymetry import *
 from dfm_tools.coastlines import *
+from dfm_tools import data
 #from dfm_tools.modelbuilder import * #commented since we do not want to expose these functions with hardcoded parameters
 
 import warnings
 warnings.filterwarnings('always',category=DeprecationWarning)
```

### Comparing `dfm_tools-0.12.0/dfm_tools/bathymetry.py` & `dfm_tools-0.13.0/dfm_tools/bathymetry.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/coastlines.py` & `dfm_tools-0.13.0/dfm_tools/coastlines.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 """
 Created on Mon Apr 24 03:46:44 2023
 
 @author: veenstra
 """
 
 import os
-import geopandas
+import geopandas as gpd
 import pandas as pd
+import datetime as dt
 
 
-def get_coastlines_gdb(res:str='h', bbox:tuple = (-180, -90, 180, 90), min_area:float = 0, crs:str = None, include_fields:list = ['area']) -> geopandas.geoseries.GeoSeries:
+def get_coastlines_gdb(res:str='h', bbox:tuple = (-180, -90, 180, 90), min_area:float = 0, crs:str = None, include_fields:list = ['area']) -> gpd.geoseries.GeoSeries:
     """
-    get coastlines from GSHHS database: https://www.ngdc.noaa.gov/mgg/shorelines/data/gshhg/latest/readme.txt
+    GSHHS coastlines: https://www.ngdc.noaa.gov/mgg/shorelines/data/gshhg/latest/readme.txt
     geopandas docs https://geopandas.org/en/stable/docs/reference/api/geopandas.read_file.html
     
     Parameters
     ----------
     res : str, optional
         f(ull), h(igh), i(ntermediate), l(ow), c(oarse) resolution. The default is 'h'.
     bbox : tuple, optional
@@ -30,40 +31,43 @@
 
     Returns
     -------
     coastlines_gdb : TYPE
         DESCRIPTION.
 
     """
-    #TODO: maybe download+unzip+load+cache from https://www.ngdc.noaa.gov/mgg/shorelines/
-    #TODO: add auto deciding of res/min_area based on bbox size (in WGS84 coords)
-    #TODO: maybe also add for rivers/borders?
     
     if res not in 'fhilc':
         raise KeyError(f'invalid res="{res}", resolution options are f(ull), h(igh), i(ntermediate), l(ow), c(oarse)')
     if crs is not None: #convert bbox from input crs to WGS84
-        bbox_points = geopandas.points_from_xy(x=[bbox[0],bbox[2]], y=[bbox[1],bbox[3]], crs=crs)
+        bbox_points = gpd.points_from_xy(x=[bbox[0],bbox[2]], y=[bbox[1],bbox[3]], crs=crs)
         bbox_points = bbox_points.to_crs('EPSG:4326') #convert to WGS84
         bbox = (bbox_points.x[0], bbox_points.y[0], bbox_points.x[1], bbox_points.y[1])
         
-    #L(evel)1 (coastlines except antarctica) and L6 (antarctic grounding line)
-    dir_GSHHS_shp = r'p:\1230882-emodnet_hrsm\data\landboundary_GSHHS\gshhg-shp-2.3.7\GSHHS_shp'
-    file_shp_L1 = os.path.join(dir_GSHHS_shp,res,f'GSHHS_{res}_L1.shp') #coastlines
-    file_shp_L6 = os.path.join(dir_GSHHS_shp,res,f'GSHHS_{res}_L6.shp') #Antarctic grounding-line polygons
-    file_shp_L2 = os.path.join(dir_GSHHS_shp,res,f'GSHHS_{res}_L2.shp') #lakes
-    file_shp_L3 = os.path.join(dir_GSHHS_shp,res,f'GSHHS_{res}_L3.shp') #islands-in-lakes
+    # download gshhs data if not present and return dir
+    from dfm_tools.data import gshhs_coastlines_shp # raises ImportError because of circular import when placed in top of script
+    dir_gshhs = gshhs_coastlines_shp()
+
+    file_shp_L1 = os.path.join(dir_gshhs,'GSHHS_shp',res,f'GSHHS_{res}_L1.shp') #coastlines
+    file_shp_L6 = os.path.join(dir_gshhs,'GSHHS_shp',res,f'GSHHS_{res}_L6.shp') #Antarctic grounding-line polygons
+    file_shp_L2 = os.path.join(dir_gshhs,'GSHHS_shp',res,f'GSHHS_{res}_L2.shp') #lakes
+    file_shp_L3 = os.path.join(dir_gshhs,'GSHHS_shp',res,f'GSHHS_{res}_L3.shp') #islands-in-lakes
     
-    coastlines_gdb_L1 = geopandas.read_file(file_shp_L1, include_fields=include_fields, where=f"area>{min_area}", bbox=bbox)
-    coastlines_gdb_L6 = geopandas.read_file(file_shp_L6, include_fields=include_fields, where=f"area>{min_area}", bbox=bbox)
+    print('>> reading coastlines: ',end='')
+    dtstart = dt.datetime.now()
+    coastlines_gdb_L1 = gpd.read_file(file_shp_L1, include_fields=include_fields, where=f"area>{min_area}", bbox=bbox)
+    coastlines_gdb_L6 = gpd.read_file(file_shp_L6, include_fields=include_fields, where=f"area>{min_area}", bbox=bbox)
     coastlines_gdb_list = [coastlines_gdb_L1,coastlines_gdb_L6]
-    if len(coastlines_gdb_L1)<2: #if max one L1 polygon is selected, automatically add lakes and islands-in-lakes
-        coastlines_gdb_L2 = geopandas.read_file(file_shp_L2, include_fields=include_fields, where=f"area>{min_area}", bbox=bbox)
-        coastlines_gdb_L3 = geopandas.read_file(file_shp_L3, include_fields=include_fields, where=f"area>{min_area}", bbox=bbox)
-        coastlines_gdb_list = [coastlines_gdb_L1,coastlines_gdb_L6,coastlines_gdb_L2,coastlines_gdb_L3]
+    if len(coastlines_gdb_L1)<2: #if only one L1 polygon is selected, automatically add lakes and islands-in-lakes
+        coastlines_gdb_L2 = gpd.read_file(file_shp_L2, include_fields=include_fields, where=f"area>{min_area}", bbox=bbox)
+        coastlines_gdb_list.append(coastlines_gdb_L2)
+        coastlines_gdb_L3 = gpd.read_file(file_shp_L3, include_fields=include_fields, where=f"area>{min_area}", bbox=bbox)
+        coastlines_gdb_list.append(coastlines_gdb_L3)
     coastlines_gdb = pd.concat(coastlines_gdb_list)
+    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
     
     if crs:
         coastlines_gdb = coastlines_gdb.to_crs(crs)
     
     return coastlines_gdb
```

### Comparing `dfm_tools-0.12.0/dfm_tools/deprecated.py` & `dfm_tools-0.13.0/dfm_tools/deprecated.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/download.py` & `dfm_tools-0.13.0/dfm_tools/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 from pathlib import Path
 import xarray as xr
 from pydap.client import open_url
 from pydap.cas.get_cookies import setup_session
 from dfm_tools.errors import OutOfRangeError
 import cdsapi
 import cftime
+import getpass
 
 
 def download_ERA5(varkey,
                   longitude_min, longitude_max, latitude_min, latitude_max, 
                   date_min, date_max,
                   dir_output='.', overwrite=False):
     """
     empty docstring
     """
     
     #TODO: describe something about the .cdsapirc file
     #TODO: make this function cdsapi generic, instead of ERA5 hardcoded (make flexible for product_type/name/name_output) (variables_dict is not used actively anymore, so this is possible)
     
+    # create $HOME/.cdsapirc if it does not exist
+    cds_credentials()
+    
     c = cdsapi.Client() # import cdsapi and create a Client instance # https://cds.climate.copernicus.eu/api-how-to
     
     #dictionary with ERA5 variables #this is not actively used
     variables_dict = {'ssr':'surface_net_solar_radiation',
                       'sst':'sea_surface_temperature',
                       'strd':'surface_thermal_radiation_downwards',
                       'slhf':'surface_latent_heat_flux',
@@ -82,27 +86,26 @@
         
         c.retrieve(name='reanalysis-era5-single-levels', request=request_dict, target=file_out)
 
 
 def download_CMEMS(varkey,
                    longitude_min, longitude_max, latitude_min, latitude_max, 
                    date_min, date_max, freq='D',
-                   dir_output='.', file_prefix='', overwrite=False,
-                   credentials=None):
+                   dir_output='.', file_prefix='', overwrite=False):
     """
     empty docstring
     """
 
     date_min, date_max = round_timestamp_to_outer_noon(date_min,date_max)
     
     global product #set product as global variable, so it only has to be retreived once per download run (otherwise once per variable)
     if 'product' not in globals():
         print('retrieving time range of CMEMS reanalysis and forecast products') #assuming here that physchem and bio reanalyisus/multiyear datasets have the same enddate, this seems safe
-        reanalysis_tstart, reanalysis_tstop = get_OPeNDAP_xr_ds_timerange(dataset_url='https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m', credentials=credentials)
-        forecast_tstart, forecast_tstop = get_OPeNDAP_xr_ds_timerange(dataset_url='https://nrt.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_anfc_0.083deg_P1D-m', credentials=credentials)
+        reanalysis_tstart, reanalysis_tstop = get_OPeNDAP_xr_ds_timerange(dataset_url='https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m')
+        forecast_tstart, forecast_tstop = get_OPeNDAP_xr_ds_timerange(dataset_url='https://nrt.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_anfc_0.083deg_P1D-m')
         if (date_min >= reanalysis_tstart) & (date_max <= reanalysis_tstop):
             product = 'reanalysis'
             print(f"The CMEMS '{product}' product will be used.")
         elif (date_min >= forecast_tstart) & (date_max <= forecast_tstop):
             product = 'analysisforecast'
             print(f"The CMEMS '{product}' product will be used.")
         else:
@@ -129,35 +132,80 @@
     #make sure the data fully covers the desired spatial extent. Download 2 additional grid cells (resolution is 1/12 degrees, but a bit more/less in alternating cells) in each direction
     longitude_min -= 2/12
     longitude_max += 2/12
     latitude_min  -= 2/12
     latitude_max  += 2/12
     
     download_OPeNDAP(dataset_url=dataset_url,
-                     credentials=credentials, #credentials=['username','password'], or create "%USERPROFILE%/CMEMS_credentials.txt" with username on line 1 and password on line 2. Register at: https://resources.marine.copernicus.eu/registration-form'
                      varkey=varkey,
                      longitude_min=longitude_min, longitude_max=longitude_max, latitude_min=latitude_min, latitude_max=latitude_max,
                      date_min=date_min, date_max=date_max,
                      dir_output=dir_output, file_prefix=file_prefix, overwrite=overwrite)
 
 
-def get_CMEMS_credentials():
+def cds_credentials():
+    """
+    create $HOME/.cdsapirc via getpass if necessary
+    """
+    #TODO: put this in a PR at https://github.com/ecmwf/cdsapi (https://github.com/ecmwf/cdsapi/blob/master/cdsapi/api.py#L303)
+    file_credentials = f'{os.path.expanduser("~")}/.cdsapirc'
+    if os.path.exists(file_credentials):
+        print('found CDS apikey')
+    else:
+        print("Downloading CDS/ERA5 data requires a CDS apikey, copy the key from https://cds.climate.copernicus.eu/api-how-to (first register and sign in) ")
+        apikey = getpass.getpass("Enter your CDS apikey: ")
+        with open(file_credentials,'w') as fc:
+            fc.write('url: https://cds.climate.copernicus.eu/api/v2\n')
+            fc.write(f'key: {apikey}')
+
+
+def copernicusmarine_credentials():
     """
-    parse file with CMEMS credentials to username/password
+    get CMEMS username/password from file or via getpass
     """
     file_credentials = f'{os.path.expanduser("~")}/CMEMS_credentials.txt'
-    if not os.path.exists(file_credentials):
-        raise FileNotFoundError(f'credentials argument not supplied and file_credentials not available ({file_credentials})')
-    with open(file_credentials) as fc:
-        username = fc.readline().strip()
-        password = fc.readline().strip()
+    if os.path.exists(file_credentials):
+        print('found CMEMS credentials')
+        with open(file_credentials) as fc:
+            username = fc.readline().strip()
+            password = fc.readline().strip()
+    else: #query username and password with getpass
+        print("Downloading CMEMS data requires a Copernicus Marine username and password, sign up for free at: https://data.marine.copernicus.eu/register.")
+        username = getpass.getpass("Enter your Copernicus Marine username: ")
+        password = getpass.getpass("Enter your Copernicus Marine password: ")
+        userpass_save = input("Do you want to save your credentials as plain text? [y/n]: ")
+        if userpass_save == 'y':
+            with open(file_credentials,'w') as fc:
+                fc.write(f'{username}\n{password}\n')
     return username, password
 
 
-def open_OPeNDAP_xr(dataset_url, credentials=None):
+def copernicusmarine_datastore(dataset_url):
+    """
+    Setting up a copernicus marine PydapDataStore with authentication via username and password.
+    """
+    if 'session' not in globals():
+        username, password = copernicusmarine_credentials()
+        #setting up a session and making the variable global so we do not have to repeat it
+        #https://help.marine.copernicus.eu/en/articles/5182598-how-to-consume-the-opendap-api-and-cas-sso-using-python
+        cas_url = 'https://cmems-cas.cls.fr/cas/login'
+        global session
+        session = setup_session(cas_url, username, password)
+    
+    cookies_dict = session.cookies.get_dict()
+    if 'CASTGC' not in cookies_dict.keys():
+        raise KeyError('CASTGC key missing from session cookies_dict, probably authentication failure')
+    session.cookies.set("CASTGC", cookies_dict['CASTGC'])
+    #TODO: add check for wrong dataset_id (now always "AttributeError: You cannot set the charset when no content-type is defined")
+    dap_dataset = open_url(dataset_url, session=session, user_charset='utf-8')
+    data_store = xr.backends.PydapDataStore(dap_dataset)
+    return data_store
+
+
+def open_OPeNDAP_xr(dataset_url):
     """
     How to get the opendap dataset_url (CMEMS example):
         - https://data.marine.copernicus.eu/products
         - go to the data access tab of a product, e.g.: https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/services
         - click the opendap link of the dataset of your choice
         - copy the dataset_url from the adress bar (excl .html), e.g.: https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m
     
@@ -166,44 +214,26 @@
         - Select a product and search for THREDDS, e.g.: https://www.hycom.org/dataserver/gofs-3pt1/analysis
         - find an opendap dataset_url, it depends per product/run where to find it.
         Some examples:
             https://tds.hycom.org/thredds/dodsC/GLBu0.08/expt_19.1/2010
             https://tds.hycom.org/thredds/dodsC/GLBy0.08/expt_93.0
 
     """
-    
-    def copernicusmarine_datastore(dataset_url, username, password):
-        #https://help.marine.copernicus.eu/en/articles/5182598-how-to-consume-the-opendap-api-and-cas-sso-using-python
-        cas_url = 'https://cmems-cas.cls.fr/cas/login'
-        session = setup_session(cas_url, username, password)
-        cookies_dict = session.cookies.get_dict()
-        if 'CASTGC' not in cookies_dict.keys():
-            raise KeyError('CASTGC key missing from session cookies_dict, probably authentication failure')
-        session.cookies.set("CASTGC", cookies_dict['CASTGC'])
-        #TODO: add check for wrong dataset_id (now always "AttributeError: You cannot set the charset when no content-type is defined")
-        dap_dataset = open_url(dataset_url, session=session, user_charset='utf-8')
-        data_store = xr.backends.PydapDataStore(dap_dataset)
-        return data_store
-    
+        
     if isinstance(dataset_url,list):
         dataset_url_one = dataset_url[0]
     else:
         dataset_url_one = dataset_url
     
     if 'cmems-du.eu' in dataset_url_one:
         if isinstance(dataset_url,list):
             raise TypeError('list not supported by opendap method used for cmems')
         
-        if credentials is None:
-            username, password = get_CMEMS_credentials() #parse file with CMEMS credentials to username/password
-        else:
-            username, password = credentials
-
         print(f'opening pydap connection to opendap dataset and opening with xarray: {dataset_url}.html')
-        data_store = copernicusmarine_datastore(dataset_url=dataset_url, username=username, password=password)
+        data_store = copernicusmarine_datastore(dataset_url=dataset_url)
         data_xr = xr.open_dataset(data_store)
     elif 'hycom.org' in dataset_url_one:
         if isinstance(dataset_url,list):
             print(f'xarray opening opendap dataset like: {dataset_url[0]}.html ({len(dataset_url)} urls/years)')
             data_xr = xr.open_mfdataset(dataset_url,decode_times=False) #TODO: for some reason decode_times does not work: "ValueError: unable to decode time units 'hours since analysis' with 'the default calendar'."
         else:
             print(f'xarray opening opendap dataset: {dataset_url}.html')
@@ -220,26 +250,25 @@
             data_xr = xr.open_dataset(dataset_url)
         if 'lon' in data_xr.dims:
             data_xr = data_xr.rename({'lon':'longitude','lat':'latitude'})
         
     return data_xr
 
 
-def download_OpenDAP_gettimes(dataset_url,credentials=None):
-    ds = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
+def download_OpenDAP_gettimes(dataset_url):
+    ds = open_OPeNDAP_xr(dataset_url=dataset_url)
     ds_time = ds.time.to_series()
     return ds_time
 
 
 def download_OPeNDAP(dataset_url,
                      varkey,
                      longitude_min, longitude_max, latitude_min, latitude_max, 
                      date_min, date_max, freq='D',
-                     dir_output='.', file_prefix='', overwrite=False,
-                     credentials=None):
+                     dir_output='.', file_prefix='', overwrite=False):
     """
     
 
     Parameters
     ----------
     dataset_url : TYPE
         DESCRIPTION.
@@ -261,31 +290,29 @@
         DESCRIPTION. The default is 'D'.
     dir_output : TYPE, optional
         DESCRIPTION. The default is '.'.
     file_prefix : TYPE, optional
         DESCRIPTION. The default is ''.
     overwrite : TYPE, optional
         DESCRIPTION. The default is False.
-    credentials : TYPE, optional
-        for CMEMS: credentials=['username','password'], or create "%USERPROFILE%/CMEMS_credentials.txt" with username on line 1 and password on line 2. Register at: https://resources.marine.copernicus.eu/registration-form'. The default is None.
-
+    
     Raises
     ------
     KeyError
         DESCRIPTION.
     OutOfRangeError
         DESCRIPTION.
 
     Returns
     -------
     None.
 
     """
     
-    data_xr = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
+    data_xr = open_OPeNDAP_xr(dataset_url=dataset_url)
     
     print(f'xarray subsetting data (variable \'{varkey}\' and lon/lat extents)')
     if varkey not in data_xr.data_vars:
         raise KeyError(f'"{varkey}" not found in dataset, available are: {list(data_xr.data_vars)}')
     data_xr_var = data_xr[[varkey]]
     data_xr_var = data_xr_var.sel(longitude=slice(longitude_min,longitude_max), #TODO: add depth selection?
                                   latitude=slice(latitude_min,latitude_max))
@@ -311,16 +338,16 @@
         data_xr_var_seltime = data_xr_var.sel(time=slice(date_str,date_str)) #+' 12:00:00', 
         
         print(f'xarray writing netcdf file: {name_output}')
         data_xr_var_seltime.to_netcdf(os.path.join(dir_output,name_output)) #TODO: add chunks={'time':1} or only possible with opening?
         data_xr_var_seltime.close()
 
 
-def get_OPeNDAP_xr_ds_timerange(dataset_url, credentials):
-    ds = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
+def get_OPeNDAP_xr_ds_timerange(dataset_url):
+    ds = open_OPeNDAP_xr(dataset_url=dataset_url)
     ds_times = ds.time.to_series()
     ds_tstart, ds_tstop = ds_times.iloc[0], ds_times.iloc[-1]
     return ds_tstart, ds_tstop
 
 
 def round_timestamp_to_outer_noon(date_min, date_max):
     """
```

### Comparing `dfm_tools-0.12.0/dfm_tools/energy_dissipation.py` & `dfm_tools-0.13.0/dfm_tools/energy_dissipation.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/get_nc.py` & `dfm_tools-0.13.0/dfm_tools/get_nc.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/get_nc_helpers.py` & `dfm_tools-0.13.0/dfm_tools/get_nc_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/hydrolib_helpers.py` & `dfm_tools-0.13.0/dfm_tools/hydrolib_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/interpolate_grid2bnd.py` & `dfm_tools-0.13.0/dfm_tools/interpolate_grid2bnd.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/linebuilder.py` & `dfm_tools-0.13.0/dfm_tools/linebuilder.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/modelbuilder.py` & `dfm_tools-0.13.0/dfm_tools/modelbuilder.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/modplot.py` & `dfm_tools-0.13.0/dfm_tools/modplot.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/xarray_helpers.py` & `dfm_tools-0.13.0/dfm_tools/xarray_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools/xugrid_helpers.py` & `dfm_tools-0.13.0/dfm_tools/xugrid_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.12.0/dfm_tools.egg-info/PKG-INFO` & `dfm_tools-0.13.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dfm-tools
-Version: 0.12.0
+Name: dfm_tools
+Version: 0.13.0
 Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
 Home-page: https://github.com/Deltares/dfm_tools
 Author: Jelmer Veenstra
 Author-email: Jelmer.Veenstra@Deltares.nl
 License: GNU General Public License v3 (GPLv3)
 Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 
 [![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
 [![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
 [![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
 [![pytest-py311](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml)
 [![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD?urlpath=/tree/docs/notebooks)
 [![Available on pypi](https://img.shields.io/pypi/v/dfm_tools.svg)](https://pypi.python.org/pypi/dfm_tools)
 [![Supported versions](https://img.shields.io/pypi/pyversions/dfm_tools.svg)](https://pypi.org/project/dfm_tools)
 [![Downloads](https://img.shields.io/pypi/dm/dfm_tools.svg)](https://pypistats.org/packages/dfm_tools)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7857393.svg)](https://doi.org/10.5281/zenodo.7857393)
 
 # dfm_tools
```

### Comparing `dfm_tools-0.12.0/dfm_tools.egg-info/SOURCES.txt` & `dfm_tools-0.13.0/dfm_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.cfg
 setup.py
 dfm_tools/__init__.py
 dfm_tools/bathymetry.py
 dfm_tools/coastlines.py
+dfm_tools/data.py
 dfm_tools/deprecated.py
 dfm_tools/download.py
 dfm_tools/energy_dissipation.py
 dfm_tools/errors.py
 dfm_tools/get_nc.py
 dfm_tools/get_nc_helpers.py
 dfm_tools/hydrolib_helpers.py
@@ -21,12 +22,14 @@
 dfm_tools.egg-info/PKG-INFO
 dfm_tools.egg-info/SOURCES.txt
 dfm_tools.egg-info/dependency_links.txt
 dfm_tools.egg-info/not-zip-safe
 dfm_tools.egg-info/requires.txt
 dfm_tools.egg-info/top_level.txt
 tests/__init__.py
+tests/test_coastlines.py
+tests/test_data.py
 tests/test_dfm_tools.py
 tests/test_download.py
+tests/test_examples.py
 tests/test_external_packages.py
-tests/test_meshkernel_helpers.py
-tests/utils.py
+tests/test_meshkernel_helpers.py
```

### Comparing `dfm_tools-0.12.0/setup.cfg` & `dfm_tools-0.13.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dfm_tools
-version = 0.12.0
+version = 0.13.0
 author = Jelmer Veenstra
 author_email = Jelmer.Veenstra@Deltares.nl
 description = dfm_tools are pre- and post-processing tools for Delft3D FM
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Deltares/dfm_tools
 keywords = dfm_tools, D-FlowFM, D-HYDRO, post-processing, pre-processing, mapfiles, hisfiles
@@ -28,14 +28,15 @@
 install_requires = 
 	scipy<1.10.0
 	numpy
 	matplotlib
 	pandas<2.0.0
 	shapely>=1.7.0
 	geopandas
+	fiona>=1.9
 	contextily
 	xarray
 	dask
 	netcdf4>=1.5.3
 	bottleneck
 	xugrid>=0.6.1
 	cdsapi
```

### Comparing `dfm_tools-0.12.0/tests/test_dfm_tools.py` & `dfm_tools-0.13.0/tests/test_dfm_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,56 @@
 #!/usr/bin/env python
 
-"""Tests for dfm_tools package environment"""
-
 import pytest
 import os
-import glob
 import dfm_tools as dfmt
 import numpy as np
 import hydrolib.core.dflowfm as hcdfm
 import pandas as pd
 
-from tests.utils import maybe_download_testdata
-
-dir_testinput = maybe_download_testdata()
-
-
-# ACCEPTANCE TESTS VIA EXAMPLE SCRIPTS, these are the ones who are only meant to generate output files
-
-dir_tests = os.path.dirname(__file__) #F9 doesnt work, only F5 (F5 also only method to reload external definition scripts)
-list_configfiles = glob.glob(os.path.join(dir_tests,'examples','*.py')) + glob.glob(os.path.join(dir_tests,'examples_workinprogress','*.py'))
-list_configfiles = [x for x in list_configfiles if 'workinprogress_xarray_performance' not in x] #ignore this slow script
-dir_output_general = os.path.join(dir_tests,'examples_output')
-os.makedirs(dir_output_general, exist_ok=True)
-
-@pytest.mark.requireslocaldata
-@pytest.mark.acceptance
-@pytest.mark.parametrize("file_config", [pytest.param(file_config, id=os.path.basename(file_config).replace('.py','')) for file_config in list_configfiles])
-def test_run_examples(file_config):
-    # 1. Set up test data
-    dir_output = os.path.join(dir_output_general,os.path.basename(file_config).replace('.py',''))
-    if not os.path.exists(dir_output):
-        os.mkdir(dir_output)
-    os.chdir(dir_output)
-    test = os.system(f'python {file_config}')#+ " & pause")
-    
-    if test:
-        raise OSError('execution did not finish properly')
-
 
-##### UNITTESTS AND SYSTEMTESTS
-
-@pytest.mark.parametrize("file_nc, expected_size", [pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0000_map.nc'), (5599,3,2), id='from 1 map partion Grevelingen'),
-                                                    pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen_FM_grid_20190603_net.nc'), (44804,4,2), id='fromnet Grevelingen')])
+@pytest.mark.parametrize("file_nc, expected_size", [pytest.param(dfmt.data.fm_grevelingen_map(return_filepath=True), (44796, 4, 2), id='from partitioned map Grevelingen'),
+                                                    pytest.param(dfmt.data.fm_curvedbend_map(return_filepath=True), (550, 4, 2), id='from map curvedbend'),
+                                                    pytest.param(dfmt.data.fm_grevelingen_net(return_filepath=True), (44804,4,2), id='fromnet Grevelingen')])
 @pytest.mark.systemtest
 def test_facenodecoordinates_shape(file_nc, expected_size):
     
     uds = dfmt.open_partitioned_dataset(file_nc)
     facenodecoordinates = uds.grid.face_node_coordinates
     
     assert facenodecoordinates.shape == expected_size
 
 
-@pytest.mark.parametrize("file_nc, varname, expected_size", [pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0*_map.nc'), 'mesh2d_sa1', (44796, 36), id='from partitioned map Grevelingen'),
-                                                             pytest.param(os.path.join(r'p:\archivedprojects\11203850-coastserv\06-Model\waq_model\simulations\run0_20200319\DFM_OUTPUT_kzn_waq', 'kzn_waq_0*_map.nc'), 'mesh2d_Chlfa', (17385, 39), id='from partitioned waq map coastserv'),
-                                                             #pytest.param(r'p:\11205258-006-kpp2020_rmm-g6\C_Work\01_Rooster\final_totaalmodel\rooster_rmm_v1p5_net.nc', 'mesh2d_face_x', (44804,), id='fromnet RMM'), #no time dimension
-                                                             ])
+@pytest.mark.unittest
+def test_getmapdata():
+    """
+    Checks whether ghost cells are properly taken care of (by asserting shape). And also whether varname can be found from attributes in case of Chlfa.
+    
+    """
+    file_nc = dfmt.data.fm_grevelingen_map(return_filepath=True)
+    expected_size = (44796, 36)
+    varname = 'mesh2d_sa1'
+    
+    data_xr_map = dfmt.open_partitioned_dataset(file_nc)
+    data_xr_map = dfmt.rename_waqvars(data_xr_map)
+    data_varsel = data_xr_map[varname].isel(time=2)
+    
+    assert data_varsel.shape == expected_size
+
+
 @pytest.mark.requireslocaldata
 @pytest.mark.unittest
-def test_getmapdata(file_nc, varname, expected_size):
+def test_getmapdata_waq():
     """
     Checks whether ghost cells are properly taken care of (by asserting shape). And also whether varname can be found from attributes in case of Chlfa.
     
-    file_nc = os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0*_map.nc')
-    expected_size = (44796,)
     """
+    file_nc = os.path.join(r'p:\archivedprojects\11203850-coastserv\06-Model\waq_model\simulations\run0_20200319\DFM_OUTPUT_kzn_waq', 'kzn_waq_0*_map.nc')
+    expected_size = (17385, 39)
+    varname = 'mesh2d_Chlfa'
     
     data_xr_map = dfmt.open_partitioned_dataset(file_nc)
     data_xr_map = dfmt.rename_waqvars(data_xr_map)
     data_varsel = data_xr_map[varname].isel(time=2)
     
     assert data_varsel.shape == expected_size
 
@@ -219,15 +202,15 @@
 
 @pytest.mark.unittest
 def test_intersect_edges():
     """
     ordering of xu.ugrid2d.intersect_edges return arrays is wrong, but we test it here since this test will fail once sorting is fixed in xugrid or numba.celltree. If so, depracate dfmt.intersect_edges_withsort()
     """
     
-    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D','cb_3d_map.nc') #sigmalayer
+    file_nc = dfmt.data.fm_curvedbend_map(return_filepath=True) #sigmalayer
                     
     line_array = np.array([[2084.67741935, 3353.02419355], #with linebend in cell en with line crossing same cell twice
                            [2255.79637097, 3307.15725806],
                            [2222.27822581, 3206.60282258],
                            [2128.78024194, 3266.58266129]])
     
     uds = dfmt.open_partitioned_dataset(file_nc)
@@ -241,15 +224,15 @@
 
 @pytest.mark.unittest
 def test_intersect_edges_withsort():
     """
     ordering of xu.ugrid2d.intersect_edges return arrays is wrong, so dfmt.intersect_edges_withsort() combines it with sorting. The line array clearly shows different ordering of the resulting face_index array
     """
     
-    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D','cb_3d_map.nc') #sigmalayer
+    file_nc = dfmt.data.fm_curvedbend_map(return_filepath=True) #sigmalayer
     
     line_array = np.array([[2084.67741935, 3353.02419355], #with linebend in cell en with line crossing same cell twice
                            [2255.79637097, 3307.15725806],
                            [2222.27822581, 3206.60282258],
                            [2128.78024194, 3266.58266129]])
     
     uds = dfmt.open_partitioned_dataset(file_nc)
@@ -259,15 +242,15 @@
     
     assert (edge_index == np.array([0, 0, 0, 1, 1, 1, 2, 2])).all()
     assert (face_index == np.array([ 91, 146, 147, 147, 202, 201, 201, 146])).all()
 
 
 @pytest.mark.unittest
 def test_zlayermodel_correct_layers():
-    file_nc = os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0*_map.nc') #zlayer
+    file_nc = dfmt.data.fm_grevelingen_map(return_filepath=True) #sigmalayer
     data_frommap_merged = dfmt.open_partitioned_dataset(file_nc)
     
     timestep = 3
     
     data_frommap_timesel = data_frommap_merged.isel(time=timestep) #select data for all layers
     data_frommap_merged_fullgrid = dfmt.reconstruct_zw_zcc_fromz(data_frommap_timesel)
     
@@ -278,18 +261,18 @@
     assert (np.abs(vals_zw_top-vals_wl)<1e-6).all()
     assert (np.abs(vals_zw_bot-vals_bl)<1e-6).all()
 
     
 @pytest.mark.requireslocaldata
 def test_timmodel_to_dataframe():
     
-    file_tim = os.path.join(dir_testinput,'Brouwerssluis_short.tim')
+    file_tim = r'p:\archivedprojects\11206811-002-d-hydro-grevelingen\simulaties\Jaarsom2017_dfm_006_zlayer\boundary_conditions\hist\jaarsom_2017\sources_sinks\FlakkeeseSpuisluis.tim'
     
     data_tim = hcdfm.TimModel(file_tim)
     
     refdate = '2016-01-01'
     tim_pd = dfmt.TimModel_to_DataFrame(data_tim, parse_column_labels=True, refdate=refdate)
     
     assert tim_pd.index[0] == pd.Timestamp('2016-01-01 00:00:00')
-    assert len(tim_pd) == 91
+    assert len(tim_pd) == 39603
     assert tim_pd.columns[-1] == 'Phaeocystis_P (g/m3)'
```

### Comparing `dfm_tools-0.12.0/tests/test_external_packages.py` & `dfm_tools-0.13.0/tests/test_external_packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,18 @@
 """
 Created on Mon Jun 19 22:03:43 2023
 
 @author: veenstra
 """
 
 import pytest
-import os
 import numpy as np
 import xarray as xr
 import xugrid as xu
-import warnings
-
-from tests.utils import maybe_download_testdata
-dir_testinput = maybe_download_testdata()
+import dfm_tools as dfmt
 
 
 @pytest.mark.unittest
 def test_import_shapely():
     """
     tests whether shapely can be imported successfully, this is a problem in some environments
     in that case 'import shapely' works, but import 'shapely.geometry' fails
@@ -27,21 +23,33 @@
     
 
 @pytest.mark.systemtest
 def test_xugrid_opendataset_ugridplot():
     """
     this one fails with xarray>=2023.3.0: https://github.com/Deltares/xugrid/issues/78
     """
-    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D/cb_3d_map.nc')
+    file_nc = dfmt.data.fm_curvedbend_map(return_filepath=True)
     
     uds = xu.open_dataset(file_nc,chunks={'time':1})
     
     uds['mesh2d_flowelem_bl'].ugrid.plot()
 
 
+@pytest.mark.systemtest
+def SKIP_test_xugrid_opendataset_ugridplot_contourf():
+    """
+    this one fails with xarray>=2023.3.0: https://github.com/Deltares/xugrid/issues/117
+    """
+    file_nc = dfmt.data.fm_curvedbend_map(return_filepath=True)
+    
+    uds = xu.open_dataset(file_nc,chunks={'time':1})
+    
+    uds['mesh2d_flowelem_bl'].ugrid.plot.contourf()
+
+
 @pytest.mark.unittest
 def test_xarray_pandas_resample():
     """
     this one fails with xarray<2023.3.0 (required for test_opendataset_ugridplot()) and pandas>1.5.3: https://github.com/Deltares/xugrid/issues/78#issuecomment-1597723955
     pandas 1.5.3 works with xarray<2023.3.0
     pandas 2.0.* fails with xarray<2023.3.0
     pandas 2.0.* works with xarray==2023.5.0
```

