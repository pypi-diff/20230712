# Comparing `tmp/optim_esm_tools-0.4.0.tar.gz` & `tmp/optim_esm_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-0.4.0.tar", last modified: Mon Jul 10 06:59:24 2023, max compression
+gzip compressed data, was "optim_esm_tools-0.5.0.tar", last modified: Wed Jul 12 12:47:32 2023, max compression
```

## Comparing `optim_esm_tools-0.4.0.tar` & `optim_esm_tools-0.5.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-10 06:59:24.927272 optim_esm_tools-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.919272 optim_esm_tools-0.4.0/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/_test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/calculate_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    23233 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/tipping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/xarray_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/optim_esm_tools/cmip_files/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/cmip_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/optim_esm_conf.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/optim_esm_tools/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/plotting/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/synda_files/format_synda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.919272 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 06:59:24.927272 optim_esm_tools-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_pangeo_download.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.691658 optim_esm_tools-0.5.0/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/calculate_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/query_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25466 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/tipping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools/cmip_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/cmip_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/optim_esm_conf.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/plotting/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/plotting/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/synda_files/format_synda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 12:47:32.699658 optim_esm_tools-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_area_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_pangeo_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-0.4.0/PKG-INFO` & `optim_esm_tools-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim_esm_tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,25 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        0.5.0 / 2023-07-07
+        ------------------
+        **Last release before refactoring pre-processing**
+        *Next release will use CDO tools instead of xMip tools to do pre-processing for reliability reasons*
+        
+        * Lon and lat coords for clustering by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/79
+        * Queriable area field by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/80
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.4.0...v0.5.0
+        
         0.4.0 / 2023-07-07
         ------------------
         *  Technical release related to the setup of the package relating to the config
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.3.0...v0.4.0
```

### Comparing `optim_esm_tools-0.4.0/README.md` & `optim_esm_tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/_test_utils.py` & `optim_esm_tools-0.5.0/optim_esm_tools/_test_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,15 +32,19 @@
 
     ddict = search.to_dataset_dict(
         xarray_open_kwargs={'use_cftime': True},
     )
     data = list(ddict.values())[0]
 
     data = data.mean(set(data.dims) - {'x', 'y', 'lat', 'lon', 'time'})
-
+    if query['variable_id'] != 'tas':
+        raise ValueError(
+            'Only tas for now as only areacella is hardcoded (see line below)'
+        )
+    data.attrs.update(dict(external_variables='areacella'))
     os.makedirs(dest_folder, exist_ok=True)
     data.to_netcdf(write_to)
     return write_to
 
 
 def year_means(path, refresh=True):
     new_dir = os.path.split(path.replace('Amon', 'AYear'))[0]
@@ -54,14 +58,15 @@
     data = oet.cmip_files.io.load_glob(path)
 
     data = data.groupby('time.year').mean('time')
     data = data.rename(year='time')
     data['time'] = [cftime.DatetimeNoLeap(y, 1, 1) for y in data['time']]
 
     os.makedirs(new_dir, exist_ok=True)
+    assert os.path.exists(new_dir)
     data.to_netcdf(new_dest)
     return new_dest
 
 
 def get_synda_loc():
     return os.path.join(
         os.environ.get('ST_HOME', os.path.join(os.path.abspath('.'), 'cmip')), 'data'
```

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/analyze/clustering.py` & `optim_esm_tools-0.5.0/optim_esm_tools/analyze/clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from optim_esm_tools.utils import tqdm, timed
+from optim_esm_tools.config import get_logger
 import typing as ty
 from warnings import warn
 import numba
 from math import sin, cos, sqrt, atan2, radians
 
 
 @timed()
@@ -75,16 +76,16 @@
 
     return return_masks
 
 
 @timed()
 def build_cluster_mask(
     global_mask: np.ndarray,
-    x_coord: np.array,
-    y_coord: np.array,
+    lon_coord: np.array,
+    lat_coord: np.array,
     show_tqdm: bool = False,
     max_distance_km: ty.Union[str, float, int] = 'infer',
     **kw,
 ) -> ty.Tuple[ty.List[np.ndarray], ty.List[np.ndarray]]:
     """Build set of clusters and masks based on the global mask, basically a utility wrapper arround build_clusters'
 
     Args:
@@ -96,103 +97,109 @@
             provided, make a guess based on the distance between grid cells.
             Defaults to 'infer'.
         show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
 
     Returns:
         ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
     """
-
-    _check_input(global_mask, x_coord, y_coord)
-    xm, ym = np.meshgrid(x_coord, y_coord)
-    xy_data = np.array([xm[global_mask.T], ym[global_mask.T]])
+    lon, lat = _check_input(global_mask, lon_coord, lat_coord)
+    xy_data = np.array([lon[global_mask], lat[global_mask]])
 
     if len(xy_data.T) <= 2:
         warn(f'No data from this mask {xy_data}!')
         return [], []
 
     if max_distance_km == 'infer':
-        max_distance_km = _infer_max_step_size(x_coord, y_coord)
+        max_distance_km = _infer_max_step_size(lon_coord.flatten(), lat_coord.flatten())
 
     masks, clusters = _build_cluster_with_kw(
-        x_coord,
-        y_coord,
+        lon_coord,
+        lat_coord,
         coordinates_deg=xy_data,
         show_tqdm=show_tqdm,
         max_distance_km=max_distance_km,
         **kw,
     )
 
     return masks, clusters
 
 
 @timed()
 def build_weighted_cluster(
     weights: np.ndarray,
-    x_coord: np.array,
-    y_coord: np.array,
+    lon_coord: np.array,
+    lat_coord: np.array,
     show_tqdm: bool = False,
     threshold=0.99,
     max_distance_km: ty.Union[str, float, int] = 'infer',
     **kw,
 ) -> ty.Tuple[ty.List[np.ndarray], ty.List[np.ndarray]]:
     """Build set of clusters and masks based on the weights (which should be a grid)'
 
     Args:
         weights (np.ndarray): normalized score data (values in [0,1])
-        x_coord (np.array): all x values
-        y_coord (np.array): all y values
+        lon_coord (np.array): all lon values
+        lat_coord (np.array): all lat values
         max_distance_km (ty.Union[str, float, int]): find an appropriate distance
             threshold for build_clusters' max_distance_km argument. If nothing is
             provided, make a guess based on the distance between grid cells.
             Defaults to 'infer'.
         show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
 
     Returns:
         ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
     """
 
-    _check_input(weights, x_coord, y_coord)
-    xm, ym = np.meshgrid(x_coord, y_coord)
-    xy_data = np.array([xm.flatten(), ym.flatten()])
+    lon, lat = _check_input(weights, lon_coord, lat_coord)
+    xy_data = np.array([lon.flatten(), lat.flatten()])
 
     if max_distance_km == 'infer':
-        max_distance_km = _infer_max_step_size(x_coord, y_coord)
+        max_distance_km = _infer_max_step_size(lon.flatten(), lat.flatten())
 
     flat_weights = weights.T.flatten()
     mask = flat_weights > threshold
     masks, clusters = _build_cluster_with_kw(
-        x_coord,
-        y_coord,
+        lon,
+        lat,
         coordinates_deg=xy_data[:, mask],
         weights=flat_weights[mask],
         show_tqdm=show_tqdm,
         max_distance_km=max_distance_km,
         **kw,
     )
 
     return masks, clusters
 
 
-def _check_input(data, x_coord, y_coord):
-    if data.shape != (len(x_coord), len(y_coord)):
-        message = f'Wrong input {data.shape} != {len(x_coord), len(y_coord)}'
+def _check_input(data, lon_coord, lat_coord):
+    if len(lon_coord.shape) <= 1:
+        get_logger.warning('Expected lon and lat values, but got x, y values')
+        # seperate x, y values, bad practice?
+        lon, lat = np.meshgrid(lon_coord, lat_coord)
+    else:
+        lon, lat = lon_coord, lat_coord
+
+    if data.shape != lon.shape or data.shape != lat.shape:
+        message = f'Wrong input {data.shape} != {lon.shape, lat.shape}'
         raise ValueError(message)
+    return lon, lat
 
 
-def _build_cluster_with_kw(x_coord, y_coord, show_tqdm=False, **cluster_kw):
+def _build_cluster_with_kw(lon, lat, show_tqdm=False, **cluster_kw):
     masks = []
     clusters = [np.rad2deg(cluster) for cluster in build_clusters(**cluster_kw)]
-
+    if lat.shape != lon.shape:
+        raise ValueError(f'Got inconsistent input {lat.shape} != {lon.shape}')
     for cluster in clusters:
-        mask = np.zeros((len(y_coord), len(x_coord)), np.bool_)
+        mask = np.zeros(lat.shape, np.bool_)
         for s_x, s_y in tqdm(cluster, desc='fill_mask', disable=not show_tqdm):
             # This is a bit blunt, but it's fast enough to regain the indexes such that we can build a 2d masked array.
-            x_i = np.argwhere(np.isclose(x_coord, s_x))[0]
-            y_i = np.argwhere(np.isclose(y_coord, s_y))[0]
-            mask[y_i, x_i] = 1
+            mask_x = np.isclose(lon, s_x)
+            mask_y = np.isclose(lat, s_y)
+            mask |= mask_x & mask_y
         masks.append(mask)
     return masks, clusters
 
 
 def _infer_max_step_size(xs, ys):
     ys = ys[ys > 0]
     # coords = [[[xs[0], ys[0]], [xs[0], ys[1]]], [[xs[0], ys[0]], [xs[1], ys[0]]]]
@@ -202,19 +209,21 @@
     return 2 * max(_distance(c) for c in coords)
 
 
 def _distance(coords, force_math=False):
     """Wrapper for if geopy is not installed"""
     if not force_math:
         try:
-            import geopy.distance
+            from geopy.distance import geodesic
 
-            return geopy.distance.geodesic(*coords).km
+            return geodesic(*coords).km
         except (ImportError, ModuleNotFoundError):
             pass
+    if len(coords) != 4:
+        coords = [c for cc in coords for c in cc]
     return _distance_bf_coord(*coords)
 
 
 @numba.njit
 def _distance_bf_coord(lat1, lon1, lat2, lon2):
     lat1 = radians(lat1)
     lon1 = radians(lon1)
```

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/analyze/cmip_handler.py` & `optim_esm_tools-0.5.0/optim_esm_tools/analyze/cmip_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,26 +22,34 @@
     variable_of_interest: ty.Tuple[str] = ('tas',),
     max_time: ty.Optional[ty.Tuple[int, int, int]] = (2100, 1, 1),
     min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
     strict: bool = True,
     _time_var='time',
     _detrend_type='linear',
     _ma_window: int = 10,
-):
+) -> xr.Dataset:
     """Transform the dataset to get it ready for handling in optim_esm_tools
 
     Args:
         ds (xr.Dataset): input dataset
+        calculate_conditions (ty.Tuple[tipping_criteria._Condition], optional): Calculate the results of these tipping conditions. Defaults to None.
+        condition_kwargs (ty.Mapping, optional): kwargs for the tipping conditions. Defaults to None.
         variable_of_interest (ty.Tuple[str], optional): Variables to handle. Defaults to ('tas',).
         max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to (2100, 1, 1).
         min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to None.
         strict (bool, optional): raise errors on loading, if any. Defaults to True.
         _time_var (str, optional): Name of the time dimention. Defaults to 'time'.
         _detrend_type (str, optional): Type of detrending applied. Defaults to 'linear'.
         _ma_window (int, optional): Moving average window (assumed to be years). Defaults to 10.
+
+    Raises:
+        ValueError: If there are multiple tipping conditions with the same short_description
+
+    Returns:
+        xr.Dataset: The fully initiallized dataset
     """
     if calculate_conditions is None:
         calculate_conditions = (
             tipping_criteria.StartEndDifference,
             tipping_criteria.StdDetrended,
             tipping_criteria.MaxJump,
             tipping_criteria.MaxDerivitive,
@@ -83,29 +91,33 @@
 @oet.utils.timed()
 def read_ds(
     base: str,
     variable_of_interest: ty.Tuple[str] = ('tas',),
     max_time: ty.Optional[ty.Tuple[int, int, int]] = (2100, 1, 1),
     min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
     apply_transform: bool = True,
+    add_area: bool = True,
+    area_query_kwargs: ty.Optional[ty.Mapping] = None,
     strict: bool = True,
-    load: bool = True,
+    load: bool = False,
     _ma_window: int = 10,
     _cache: bool = True,
     _file_name: str = 'merged.nc',
     **kwargs,
 ) -> xr.Dataset:
     """Read a dataset from a folder called "base".
 
     Args:
         base (str): Folder to load the data from
         variable_of_interest (ty.Tuple[str], optional): Variables to handle. Defaults to ('tas',).
         max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to (2100, 1, 1).
         min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to None.
-        transform_ds: (boolm optional): Apply analysis specific postprocessing algoritms. Defaults to True.
+        apply_transform: (bool, optional): Apply analysis specific postprocessing algoritms. Defaults to True.
+        add_area (bool, optional): Search for cell area information. Defaults to True.
+        area_query_kwargs (ty.Mapping, optional): additionall keyword arguments for searching.
         strict (bool, optional): raise errors on loading, if any. Defaults to True.
         load (bool, optional): apply dataset.load to dataset directly. Defaults to False.
         _ma_window (int, optional): Moving average window (assumed to be years). Defaults to 10.
         _cache (bool, optional): cache the dataset with it's extra fields to alow faster (re)loading. Defaults to True.
 
     kwargs:
         any kwargs are passed onto transfor_ds.
@@ -139,14 +151,17 @@
         if strict:
             raise FileNotFoundError(message)
         warn(message)
         return None
 
     data_set = oet.analyze.io.load_glob(data_path, load=load)
     data_set = oet.analyze.io.recast(data_set)
+    if add_area:
+        area_query_kwargs = area_query_kwargs or dict()
+        data_set = _add_area(data_set, strict, path=data_path, **area_query_kwargs)
 
     if apply_transform:
         data_set = transform_ds(
             data_set,
             variable_of_interest=variable_of_interest,
             max_time=max_time,
             min_time=min_time,
@@ -167,14 +182,48 @@
 
     if _cache:
         oet.config.get_logger().info(f'Write {post_processed_file}')
         data_set.to_netcdf(post_processed_file)
     return data_set
 
 
+def _add_area(
+    data_set,
+    strict,
+    _change_logging=True,
+    **kw,
+):
+    import logging
+    import numpy as np
+
+    data_set = data_set.copy()
+    shape = len(data_set['y']), len(data_set['x'])
+
+    data_set['cell_area'] = (
+        ('y', 'x'),
+        np.ones(shape) * 180 * 360 / np.product(shape),
+    )
+    return data_set
+
+    if _change_logging:
+        # Intake-esm is so verbose...
+        logging.getLogger().setLevel(logging.ERROR)
+    try:
+        data_set = oet.analyze.query_metric.add_area_to_ds(data_set, **kw)
+    except oet.analyze.query_metric.NoMatchFoundError:
+        if strict:
+            # If you are really desperate pass method='brute_force'
+            raise
+    finally:
+        from optim_esm_tools.config import config
+
+        logging.getLogger().setLevel(config['log']['logging_level'].upper())
+    return data_set
+
+
 def _name_cache_file(
     base,
     variable_of_interest,
     min_time,
     max_time,
     _ma_window,
     version,
```

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/analyze/find_matches.py` & `optim_esm_tools-0.5.0/optim_esm_tools/analyze/find_matches.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,40 +26,47 @@
     activity_id='ScenarioMIP',
     institution_id='*',
     source_id='*',
     experiment_id='ssp585',
     variant_label='*',
     domain='Ayear',
     variable_id='tas',
-    grid='*',
+    grid_label='*',
     version='*',
     max_versions: int = 1,
     max_members: int = 1,
     required_file='merged.nc',
+    # Depricated arg
+    grid=None,
 ) -> list:
     """Follow synda folder format to find matches
 
     Args:
         base (str): where start looking for matches
         activity_id (str, optional): As synda convention. Defaults to 'ScenarioMIP'.
         institution_id (str, optional): As synda convention. Defaults to '*'.
         source_id (str, optional): As synda convention. Defaults to '*'.
         experiment_id (str, optional): As synda convention. Defaults to 'ssp585'.
         variant_label (str, optional): As synda convention. Defaults to '*'.
         domain (str, optional): As synda convention. Defaults to 'Ayear'.
         variable_id (str, optional): As synda convention. Defaults to 'tas'.
-        grid (str, optional): As synda convention. Defaults to '*'.
+        grid_label (str, optional): As synda convention. Defaults to '*'.
         version (str, optional): As synda convention. Defaults to '*'.
         max_versions (int, optional): Max mumber of different versions that match. Defaults to 1.
         max_members (int, optional): Max mumber of different members that match. Defaults to 1.
         required_file (str, optional): Filename to match. Defaults to 'merged.nc'.
 
     Returns:
         list: of matches corresponding to the query
     """
+    if grid is not None:
+        get_logger().warning(
+            f'grid argument for find_matches is depricated, use grid_label'
+        )
+        grid_label = grid
     if max_versions is None:
         max_versions = int(9e9)
     if max_members is None:
         max_members = int(9e9)
     variantes = sorted(
         glob.glob(
             os.path.join(
@@ -67,15 +74,15 @@
                 activity_id,
                 institution_id,
                 source_id,
                 experiment_id,
                 variant_label,
                 domain,
                 variable_id,
-                grid,
+                grid_label,
                 version,
             )
         ),
         key=_variant_label_id_and_version,
     )
     seen = dict()
     for candidate in variantes:
@@ -162,7 +169,17 @@
     if folders[-1][0] == 'v' and len(folders[-1]) == len('v20190731'):
         return {
             k: folders[-i - 1]
             for i, k in enumerate(config['CMIP_files']['folder_fmt'].split()[::-1])
         }
         # great
     raise NotImplementedError(f'folder {path} does not end with a version')
+
+
+def base_from_path(path, look_back_extra=0):
+    path = _get_head(path)
+    return os.path.join(
+        os.sep,
+        *path.split(os.sep)[
+            : -len(config['CMIP_files']['folder_fmt'].split()) - look_back_extra
+        ],
+    )
```

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/analyze/io.py` & `optim_esm_tools-0.5.0/optim_esm_tools/analyze/io.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 import xarray as xr
 import numpy as np
 import os
 from optim_esm_tools.utils import add_load_kw
-from optim_esm_tools.analyze.calculate_metric import add_grid_area_field
 
 
 @add_load_kw
 def load_glob(
     pattern: str,
     **kw,
 ) -> xr.Dataset:
@@ -41,17 +40,18 @@
         broadcast_lonlat,
         _drop_coords,
         correct_coordinates,
         correct_lon,
         correct_units,
         parse_lon_lat_bounds,
         sort_vertex_order,
-        maybe_convert_bounds_to_vertex,
-        maybe_convert_vertex_to_bounds,
-        fix_metadata,
+        replace_x_y_nominal_lat_lon,
+        # maybe_convert_bounds_to_vertex,
+        # maybe_convert_vertex_to_bounds,
+        # fix_metadata,
     )
 
     ds = data_set.copy()
     # See https://github.com/jbusecke/xMIP/issues/299
     for k, v in {'longitude': 'lon', 'latitude': 'lat'}.items():
         if k in ds and v not in ds:
             ds = ds.rename({k: v})
@@ -60,58 +60,43 @@
     # promote empty dims to actual coordinates
     ds = promote_empty_dims(ds)
     # demote coordinates from data_variables
     ds = correct_coordinates(ds)
     # broadcast lon/lat
     ds = broadcast_lonlat(ds)
     # shift all lons to consistent 0-360
-    ds = correct_lon(ds)
+    # Breaks some grids!
+    # ds = correct_lon(ds)
     # fix the units
     ds = correct_units(ds)
     # rename the `bounds` according to their style (bound or vertex)
     ds = parse_lon_lat_bounds(ds)
     # sort verticies in a consistent manner
     ds = sort_vertex_order(ds)
     # convert vertex into bounds and vice versa, so both are available
-    ds = maybe_convert_bounds_to_vertex(ds)
-    ds = maybe_convert_vertex_to_bounds(ds)
+    # ds = maybe_convert_bounds_to_vertex(ds)
+    # ds = maybe_convert_vertex_to_bounds(ds)
 
     # Not really sure if we need this, it raises key errors since we aren't xmip
     # ds = fix_metadata(ds)
-    ds = ds.drop_vars(_drop_coords, errors='ignore')
+    # ds = ds.drop_vars(_drop_coords, errors='ignore')
 
-    # Add grid field (associate km2 to each x,y value)
-    add_grid_area_field(ds)
+    import xmip.preprocessing
+
+    xmip.preprocessing._interp_nominal_lon = _interp_nominal_lon_new
+    # # remove unphyisical cell area
+    # mask = ds['cell_area'] == 0
+    # ds['lat'][mask] = 0
+    # ds['lon'][mask] = 0
+    ds = replace_x_y_nominal_lat_lon(ds)
     return ds
 
 
-# Keeping this arround for sake of the old times
-# def _interp_nominal_lon_new(lon_1d):
-#     from optim_esm_tools.config import get_logger
-#     get_logger().debug('Using altered version _interp_nominal_lon_new')
-#     x = np.arange(len(lon_1d))
-#     idx = np.isnan(lon_1d)
-#     # TODO assume that longitudes are cyclic see https://github.com/jbusecke/xMIP/issues/299
-#     ret = np.interp(x, x[~idx], lon_1d[~idx], period=len(lon_1d))
-#     return ret
-
-# def recast(data_set):
-#     from xmip.preprocessing import (
-#         promote_empty_dims,
-#         replace_x_y_nominal_lat_lon,
-#         rename_cmip6,
-#         broadcast_lonlat,
-#     )
-
-#     ds = data_set.copy()
-#     # See https://github.com/jbusecke/xMIP/issues/299
-#     for k, v in {'longitude': 'lon', 'latitude': 'lat'}.items():
-#         if k in ds and v not in ds:
-#             ds = ds.rename({k: v})
-#     ds = rename_cmip6(ds)
-#     ds = promote_empty_dims(ds)
-#     ds = broadcast_lonlat(ds)
-#     import xmip.preprocessing
-
-#     xmip.preprocessing._interp_nominal_lon = _interp_nominal_lon_new
-#     ds = replace_x_y_nominal_lat_lon(ds)
-#     return ds
+def _interp_nominal_lon_new(lon_1d):
+    from optim_esm_tools.config import get_logger
+
+    get_logger().debug('Using altered version _interp_nominal_lon_new')
+    x = np.arange(len(lon_1d))
+    idx = np.isnan(lon_1d)
+    # TODO assume that longitudes are cyclic see https://github.com/jbusecke/xMIP/issues/299
+    ret = np.interp(x, x[~idx], lon_1d[~idx], period=len(lon_1d))
+    return ret
```

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/analyze/region_finding.py` & `optim_esm_tools-0.5.0/optim_esm_tools/analyze/region_finding.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from optim_esm_tools.analyze.cmip_handler import transform_ds, read_ds
 from optim_esm_tools.analyze.clustering import (
     build_cluster_mask,
     build_weighted_cluster,
 )
 from optim_esm_tools.plotting.plot import setup_map, _show
 from optim_esm_tools.analyze.tipping_criteria import var_to_perc, rank2d
+from optim_esm_tools.analyze.find_matches import base_from_path
 
 
 import os
 
 import numpy as np
 import xarray as xr
 
@@ -41,14 +42,19 @@
         message = (
             f'Spurious coordinate {spurious_dim} dropping for safety. Keep {no_drop}'
         )
         oet.config.get_logger().warn(message)
         data_set = data_set.mean(spurious_dim)
     for k, data_array in data_set.data_vars.items():
         if all(dim in list(data_array.dims) for dim in masked_dims):
+            # First dim is time?
+            if 'time' == data_array.dims[0] and data_array.shape[1:] == da_mask.T.shape:
+                da_mask = da_mask.T
+            elif data_array.shape == da_mask.T.shape:
+                da_mask = da_mask.T
             da = data_set[k].where(da_mask, drop=False)
             da = da.assign_attrs(ds_start[k].attrs)
             data_set[k] = da
     data_set = data_set.assign_attrs(ds_start.attrs)
     return data_set
 
 
@@ -116,14 +122,15 @@
                     f'Best is to start {self.__class__.__name__} from a synda path'
                 )
                 self.data_set = transform_ds(data_set)
             else:
                 self.data_set = data_set
         else:
             self.data_set = read_ds(path, **read_ds_kw)
+
         if save_kw is None:
             save_kw = dict(
                 save_in='./',
                 file_types=(
                     'png',
                     'pdf',
                 ),
@@ -155,15 +162,15 @@
 
     @plt_show
     def plot_basic_map(self):
         self._plot_basic_map()
         self.save(f'{self.title_label}_global_map')
 
     def _plot_basic_map(self):
-        raise NotImplementedError(f'{self.__class__.__class__} has no _plot_basic_map')
+        raise NotImplementedError(f'{self.__class__.__name__} has no _plot_basic_map')
 
     def save(self, name):
         assert self.__class__.__name__ in name
         oet.utils.save_fig(name, **self.save_kw)
 
     @property
     def title(self):
@@ -178,19 +185,23 @@
             if mask is None or not np.sum(mask):
                 return 0
         except Exception as e:
             print(mask)
             raise ValueError(
                 mask,
             ) from e
-        return self.data_set['cell_area'].values[mask].sum()
+        if self.data_set['cell_area'].shape == mask.shape:
+            return self.data_set['cell_area'].values[mask]
+        if self.data_set['cell_area'].shape == mask.T.shape:
+            return self.data_set['cell_area'].values[mask.T]
+        raise ValueError
 
     @apply_options
-    def mask_is_large_enough(self, mask, min_area_km_sq=0):
-        return self.mask_area(mask) >= min_area_km_sq
+    def mask_is_large_enough(self, mask, min_area_sq=0):
+        return self.mask_area(mask).sum() >= min_area_sq
 
     def filter_masks_and_clusters(self, masks_and_clusters):
         if not len(masks_and_clusters[0]):
             return [], []
         ret_m = []
         ret_c = []
         for m, c in zip(*masks_and_clusters):
@@ -310,63 +321,76 @@
 
 class Percentiles(RegionExtractor):
     @oet.utils.check_accepts(
         accepts=immutabledict.immutabledict(cluster_method=('weighted', 'masked'))
     )
     @apply_options
     def get_masks(self, cluster_method='masked') -> dict:
-        """Get mask for max of ii and iii and a box arround that"""
         if cluster_method == 'weighted':
-            return self._get_masks_weighted()
-        return self._get_masks_masked()
+            masks, clusters = self._get_masks_weighted()
+        else:
+            masks, clusters = self._get_masks_masked()
+        if len(masks) and masks[0].shape == self.data_set['cell_area'].values.T.shape:
+            masks = [m.T for m in masks]
+        return masks, clusters
 
     @apply_options
-    def _get_masks_weighted(self, min_weight=0.95):
+    def _get_masks_weighted(
+        self,
+        min_weight=0.95,
+        lon_lat_dim=('lon', 'lat'),
+    ):
         labels = [crit.short_description for crit in self.criteria]
 
         sums = []
         for lab in labels:
-            vals = self.data_set[lab].values.T
+            vals = self.data_set[lab].values
             vals = rank2d(vals)
             vals[np.isnan(vals)] = 0
             sums.append(vals)
 
         tot_sum = np.zeros_like(sums[0])
         for s in sums:
             tot_sum += s
         tot_sum /= len(sums)
 
+        if tot_sum.T.shape == self.data_set[lon_lat_dim[0]].shape:
+            tot_sum = tot_sum.T
         masks, clusters = build_weighted_cluster(
             weights=tot_sum,
-            x_coord=self.data_set['x'].values,
-            y_coord=self.data_set['y'].values,
+            lon_coord=self.data_set[lon_lat_dim[0]].values,
+            lat_coord=self.data_set[lon_lat_dim[1]].values,
             threshold=min_weight,
         )
         return masks, clusters
 
     @apply_options
     def _get_masks_masked(
         self,
         percentiles=_two_sigma_percent,
+        lon_lat_dim=('lon', 'lat'),
     ):
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         for lab in labels:
-            arr = self.data_set[lab].values.T
+            arr = self.data_set[lab].values
             arr_no_nan = arr[~np.isnan(arr)]
             thr = np.percentile(arr_no_nan, percentiles)
             masks.append(arr >= thr)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
-
+        if all_mask.T.shape == self.data_set[lon_lat_dim[0]].shape:
+            all_mask = all_mask.T
         masks, clusters = build_cluster_mask(
-            all_mask, self.data_set['x'].values, self.data_set['y'].values
+            all_mask,
+            lon_coord=self.data_set[lon_lat_dim[0]].values,
+            lat_coord=self.data_set[lon_lat_dim[1]].values,
         )
         return masks, clusters
 
     @plt_show
     def plot_masks(self, masks_and_clusters, ax=None, legend=True):
         if not len(masks_and_clusters[0]):
             self.log.warning('No clusters found!')
@@ -384,31 +408,31 @@
         masks_and_clusters,
         scatter_medians=True,
         ax=None,
         legend=True,
         mask_cbar_kw=None,
         cluster_kw=None,
     ):
+        ds_dummy = self.data_set.copy()
         masks, clusters = masks_and_clusters
-        all_masks = np.zeros(masks[0].shape, np.float64)
+        all_masks = np.zeros(ds_dummy['cell_area'].shape, np.float64)
         all_masks[:] = np.nan
-        ds_dummy = self.data_set.copy()
-        area = ds_dummy['cell_area'].values
-        for m, c in zip(masks, clusters):
-            a = area[m].sum()
-            all_masks[m] = a
+        for m, _ in zip(masks, clusters):
+            if all_masks.shape == m.T.shape:
+                m = m.T
+            all_masks[m] = self.mask_area(m).sum()
 
         if ax is None:
             setup_map()
             ax = plt.gca()
         if mask_cbar_kw is None:
             mask_cbar_kw = dict(extend='neither', label='Area per cluster [km$^2$]')
         mask_cbar_kw.setdefault('orientation', 'horizontal')
 
-        ds_dummy['area_square'] = (('y', 'x'), all_masks)
+        ds_dummy['area_square'] = (ds_dummy['cell_area'].dims, all_masks)
 
         ds_dummy['area_square'].plot(cbar_kwargs=mask_cbar_kw, vmin=0, extend='neither')
         plt.title('')
         if scatter_medians:
             if cluster_kw is None:
                 cluster_kw = dict()
             for m_i, cluster in enumerate(clusters):
@@ -497,57 +521,67 @@
                 ax.legend(**legend_kw)
         plt.suptitle(f'Clusters {self.title}', y=0.95)
 
 
 class PercentilesHistory(Percentiles):
     @apply_options
     def get_masks(
-        self, percentiles_historical=_two_sigma_percent, read_ds_kw=None
+        self,
+        percentiles_historical=_two_sigma_percent,
+        read_ds_kw=None,
+        lon_lat_dim=('lon', 'lat'),
     ) -> dict:
         if read_ds_kw is None:
             read_ds_kw = dict()
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
 
         historical_ds = self.get_historical_ds(read_ds_kw=read_ds_kw)
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         for lab in labels:
-            arr = self.data_set[lab].values.T
-            arr_historical = historical_ds[lab].values.T
+            arr = self.data_set[lab].values
+            arr_historical = historical_ds[lab].values
             thr = np.percentile(
                 arr_historical[~np.isnan(arr_historical)], percentiles_historical
             )
             masks.append(arr >= thr)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
+        if all_mask.T.shape == self.data_set[lon_lat_dim[0]].shape:
+            all_mask = all_mask.T
+        assert all_mask.shape == self.data_set[lon_lat_dim[0]].shape, (
+            all_mask.shape,
+            self.data_set[lon_lat_dim[0]].shape,
+        )
         masks, clusters = build_cluster_mask(
-            all_mask, self.data_set['x'].values, self.data_set['y'].values
+            all_mask,
+            lon_coord=self.data_set[lon_lat_dim[0]].values,
+            lat_coord=self.data_set[lon_lat_dim[1]].values,
         )
+        if len(masks) and masks[0].shape == self.data_set['cell_area'].values.T.shape:
+            masks = [m.T for m in masks]
         return masks, clusters
 
     @apply_options
     def find_historical(
         self,
         match_to='piControl',
-        look_back_extra=1,
+        look_back_extra=0,
         query_updates=None,
         search_kw=None,
     ):
         from optim_esm_tools.config import config
 
-        base = os.path.join(
-            os.sep,
-            *self.data_set.attrs['path'].split(os.sep)[
-                : -len(config['CMIP_files']['folder_fmt'].split()) - look_back_extra
-            ],
+        base = base_from_path(
+            self.data_set.attrs['path'], look_back_extra=look_back_extra
         )
 
         search = oet.cmip_files.find_matches.folder_to_dict(self.data_set.attrs['path'])
         search['activity_id'] = 'CMIP'
         if search['experiment_id'] == match_to:
             raise NotImplementedError()
         search['experiment_id'] = match_to
@@ -555,15 +589,15 @@
             search.update(search_kw)
         if query_updates is None:
             query_updates = [
                 dict(),
                 dict(variant_label='*'),
                 dict(version='*'),
                 # can lead to funny behavior as grid differences may cause breaking compares
-                dict(grid='*'),
+                dict(grid_label='*'),
             ]
 
         for try_n, update_query in enumerate(query_updates):
             if try_n:
                 self.log.warning(
                     f'No results after {try_n} try, retying with {update_query}'
                 )
@@ -589,85 +623,103 @@
     @oet.utils.check_accepts(
         accepts=immutabledict.immutabledict(cluster_method=('weighted', 'masked'))
     )
     @apply_options
     def get_masks(self, cluster_method='masked') -> dict:
         """Get mask for max of ii and iii and a box arround that"""
         if cluster_method == 'weighted':
-            return self._get_masks_weighted()
-        return self._get_masks_masked()
+            masks, clusters = self._get_masks_weighted()
+        else:
+            masks, clusters = self._get_masks_masked()
+        if len(masks) and masks[0].shape == self.data_set['cell_area'].values.T.shape:
+            masks = [m.T for m in masks]
+        return masks, clusters
 
     @apply_options
-    def _get_masks_weighted(self, min_weight=0.95):
+    def _get_masks_weighted(self, min_weight=0.95, lon_lat_dim=('lon', 'lat')):
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         ds = self.data_set.copy()
         combined_score = np.ones_like(ds[labels[0]].values)
+
         for label in labels:
             combined_score *= rank2d(ds[label].values)
 
-        combined_score = combined_score.T
-
+        if combined_score.T.shape == self.data_set[lon_lat_dim[0]].shape:
+            combined_score = combined_score.T
         masks, clusters = build_weighted_cluster(
             weights=combined_score,
-            x_coord=self.data_set['x'].values,
-            y_coord=self.data_set['y'].values,
+            lon_coord=self.data_set[lon_lat_dim[0]].values,
+            lat_coord=self.data_set[lon_lat_dim[1]].values,
             threshold=min_weight,
         )
         return masks, clusters
 
     @apply_options
-    def _get_masks_masked(self, product_percentiles=_two_sigma_percent) -> dict:
+    def _get_masks_masked(
+        self, product_percentiles=_two_sigma_percent, lon_lat_dim=('lon', 'lat')
+    ) -> dict:
         """Get mask for max of ii and iii and a box arround that"""
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         ds = self.data_set.copy()
         combined_score = np.ones_like(ds[labels[0]].values)
         for label in labels:
             combined_score *= rank2d(ds[label].values)
 
         # Combined score is fraction, not percent!
-        all_mask = (combined_score > (product_percentiles / 100)).T
+        all_mask = combined_score > (product_percentiles / 100)
+
+        if all_mask.T.shape == self.data_set[lon_lat_dim[0]].shape:
+            all_mask = all_mask.T
 
         masks, clusters = build_cluster_mask(
-            all_mask, self.data_set['x'].values, self.data_set['y'].values
+            all_mask,
+            lon_coord=self.data_set[lon_lat_dim[0]].values,
+            lat_coord=self.data_set[lon_lat_dim[1]].values,
         )
         return masks, clusters
 
 
 class LocalHistory(PercentilesHistory):
     @apply_options
-    def get_masks(self, n_times_historical=4, read_ds_kw=None) -> dict:
+    def get_masks(
+        self, n_times_historical=4, read_ds_kw=None, lon_lat_dim=('lon', 'lat')
+    ) -> dict:
         if read_ds_kw is None:
             read_ds_kw = dict()
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
 
         historical_ds = self.get_historical_ds(read_ds_kw=read_ds_kw)
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         for lab in labels:
-            arr = self.data_set[lab].values.T
-            arr_historical = historical_ds[lab].values.T
+            arr = self.data_set[lab].values
+            arr_historical = historical_ds[lab].values
             mask_divide = arr / arr_historical > n_times_historical
             # If arr_historical is 0, the devision is going to get a nan assigned,
             # despite this being the most interesting region (no historical
             # changes, only in the scenario's)!
             mask_no_std = (arr_historical == 0) & (arr > 0)
             masks.append(mask_divide | mask_no_std)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
+        if all_mask.T.shape == self.data_set[lon_lat_dim[0]].shape:
+            all_mask = all_mask.T
         masks, clusters = build_cluster_mask(
-            all_mask, self.data_set['x'].values, self.data_set['y'].values
+            all_mask,
+            lon_coord=self.data_set[lon_lat_dim[0]].values,
+            lat_coord=self.data_set[lon_lat_dim[1]].values,
         )
         return masks, clusters
 
     @apply_options
     def _plot_basic_map(self, normalizations=None, read_ds_kw=None):
         if read_ds_kw is None:
             read_ds_kw = dict()
```

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/analyze/tipping_criteria.py` & `optim_esm_tools-0.5.0/optim_esm_tools/analyze/tipping_criteria.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,17 +135,15 @@
 
         combined_score = np.ones_like(da_1.values)
         for da, label in zip(
             [da_1, da_2], [super_1.short_description, super_2.short_description]
         ):
             _name = f'percentile {label}'
             combined_score *= var_to_perc(da, _name, None)
-        return xr.DataArray(
-            combined_score, dims=('y', 'x'), name=self.short_description
-        )
+        return xr.DataArray(combined_score, dims=da_1.dims, name=self.short_description)
 
 
 @timed
 @apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
 def running_mean_diff(
     data_set: xr.Dataset,
```

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/analyze/xarray_tools.py` & `optim_esm_tools-0.5.0/optim_esm_tools/analyze/xarray_tools.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/config.py` & `optim_esm_tools-0.5.0/optim_esm_tools/config.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/optim_esm_conf.ini` & `optim_esm_tools-0.5.0/optim_esm_tools/optim_esm_conf.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ## Config file with defaults for optim_esm_tools
 
 [constants]
 # 365.25 * 24 * 3600
 seconds_to_year = 31557600
 
 [versions]
-cmip_handler = 0.3.1-prealpha_4
+cmip_handler = 0.3.5-13.patch-area
 
 [display]
 progress_bar = True
 
 [CMIP_files]
-folder_fmt = institution_id source_id experiment_id variant_label domain variable_id grid version
+folder_fmt = activity_id institution_id source_id experiment_id variant_label domain variable_id grid_label version
 excluded =
         # This one only has a dataset which is 5 years long, rendering it quite useless for 10yr running means
         E3SM-Project       E3SM-1-1-ECA     piControl   r1i1p1f1  *        *  gr  v20201204
 
         # Bad data https://errata.es-doc.org/static/index.html?experiment=ssp585&institute=thu&project=cmip6&source=ciesm
         THU                CIESM            ssp585      r1i1p1f1  *        *  *   v20200417
 
@@ -35,14 +35,19 @@
         #  Verify if this exclusions are correct
         # Something wrong happened with the lon/lat coords.
         NCAR               CESM2            ssp370      r4i1p1f1  siconc   *  gn  v20200528
 
         # Projection fails
         DKRZ               MPI-ESM1-2-LR    ssp119      r1i1p1f1  siconc   *  *   v20210901
 
+
+        # areacello uses non conformal indexing for lat/lon (one iterator i for x and y)
+        MPI-M              ICON-ESM-LR      *           *         Ofx     *   gn  v20210215
+        MPI-M              ICON-ESM-LR      *           *         fx      *   gn  v20220111
+
 [log]
-logging_level=WARNING
+logging_level=ERROR
 
 # For the wrapper that monitors real time of functions (@timed)
 [time_tool]
 min_seconds=10
 reporter=warning
```

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/plotting/map_maker.py` & `optim_esm_tools-0.5.0/optim_esm_tools/plotting/map_maker.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/synda_files/format_synda.py` & `optim_esm_tools-0.5.0/optim_esm_tools/synda_files/format_synda.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-0.5.0/optim_esm_tools/synda_files/synda_files.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools/utils.py` & `optim_esm_tools-0.5.0/optim_esm_tools/utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools.egg-info/PKG-INFO` & `optim_esm_tools-0.5.0/optim_esm_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim-esm-tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,25 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        0.5.0 / 2023-07-07
+        ------------------
+        **Last release before refactoring pre-processing**
+        *Next release will use CDO tools instead of xMip tools to do pre-processing for reliability reasons*
+        
+        * Lon and lat coords for clustering by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/79
+        * Queriable area field by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/80
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.4.0...v0.5.0
+        
         0.4.0 / 2023-07-07
         ------------------
         *  Technical release related to the setup of the package relating to the config
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.3.0...v0.4.0
```

### Comparing `optim_esm_tools-0.4.0/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-0.5.0/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 optim_esm_tools/analyze/__init__.py
 optim_esm_tools/analyze/calculate_metric.py
 optim_esm_tools/analyze/clustering.py
 optim_esm_tools/analyze/cmip_handler.py
 optim_esm_tools/analyze/find_matches.py
 optim_esm_tools/analyze/globals.py
 optim_esm_tools/analyze/io.py
+optim_esm_tools/analyze/query_metric.py
 optim_esm_tools/analyze/region_finding.py
 optim_esm_tools/analyze/tipping_criteria.py
 optim_esm_tools/analyze/xarray_tools.py
 optim_esm_tools/cmip_files/__init__.py
 optim_esm_tools/plotting/__init__.py
 optim_esm_tools/plotting/map_maker.py
 optim_esm_tools/plotting/plot.py
 optim_esm_tools/synda_files/__init__.py
 optim_esm_tools/synda_files/format_synda.py
 optim_esm_tools/synda_files/synda_files.py
+test/test_area_query.py
 test/test_basics.py
 test/test_clustering.py
 test/test_find_matches.py
 test/test_pangeo_download.py
 test/test_plotting.py
 test/test_region_finding.py
 test/test_utils.py
```

### Comparing `optim_esm_tools-0.4.0/setup.py` & `optim_esm_tools-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='0.4.0',
+    version='0.5.0',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
     packages=setuptools.find_packages(),
     package_dir={
```

### Comparing `optim_esm_tools-0.4.0/test/test_clustering.py` & `optim_esm_tools-0.5.0/test/test_clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 
 def test_clustering_empty():
     ds = optim_esm_tools._test_utils.minimal_xr_ds().copy()
     ds['var'] = (ds['var'].dims, np.zeros_like(ds['var']))
     ds = ds.isel(time=0)
     assert np.all(np.shape(ds['var']) > np.array([2, 2]))
-
-    clusters, masks = clustering.build_cluster_mask(ds['var'] > 0, ds['x'], ds['y'])
+    lat, lon = np.meshgrid(ds['y'], ds['x'])
+    clusters, masks = clustering.build_cluster_mask(ds['var'] > 0, lon, lat)
     assert len(clusters) == len(masks) == 0
 
 
 def test_clustering_double_blob(npoints=100, res_x=3, res_y=3):
     ds = optim_esm_tools._test_utils.minimal_xr_ds().copy()
     ds = ds.isel(time=0)
 
@@ -28,19 +28,19 @@
             np.clip(np.random.normal(y, res_y, npoints).astype(int), 0, len_y),
         ):
             arr[x_i][y_i] += 1
 
     assert np.sum(arr) == 2 * npoints
     ds['var'] = (ds['var'].dims, arr)
     assert np.all(np.shape(ds['var']) > np.array([2, 2]))
-
+    lat, lon = np.meshgrid(ds['y'], ds['x'])
     clusters, masks = clustering.build_cluster_mask(
         ds['var'] > 1,
-        ds['x'],
-        ds['y'],
+        lon,
+        lat,
         max_distance_km=1000,
         min_samples=2,
     )
     assert len(clusters) == len(masks)
     assert len(clusters) == 2
```

### Comparing `optim_esm_tools-0.4.0/test/test_find_matches.py` & `optim_esm_tools-0.5.0/test/test_find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/test/test_region_finding.py` & `optim_esm_tools-0.5.0/test/test_region_finding.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import optim_esm_tools._test_utils
 from optim_esm_tools.analyze import region_finding
 import tempfile
 import os
 
 
 class Work(unittest.TestCase):
+    """
+    Note of caution! cache=True can lead to funky behavoir!
+    """
+
     @classmethod
     def setUpClass(cls):
         for data_name in ['ssp585', 'piControl']:
             cls.get_path(data_name)
 
     @staticmethod
     def get_path(data_name, refresh=True):
@@ -38,22 +42,26 @@
             save_kw = dict(
                 save_in=temp_dir,
                 sub_dir=None,
                 file_types=('png',),
                 dpi=25,
                 skip=skip_save,
             )
+            ## REMEMBER THE CACHE = TRUE!
             region_finder = cls(
                 path=head,
-                read_ds_kw=dict(_file_name=tail),
+                read_ds_kw=dict(
+                    _file_name=tail, _cache=os.environ.get('_CACHE_TRUE', 0)
+                ),
                 transform=True,
                 save_kw=save_kw,
                 extra_opt=extra_opt,
             )
             region_finder.show = False
+            ## REMEMBER THE CACHE = TRUE!
             region_finder.workflow()
             return region_finder
 
     def test_max_region_wo_time_series(self):
         self.test_max_region('MaxRegion', new_opt=dict(time_series_joined=False))
 
     def test_percentiles(self):
```

### Comparing `optim_esm_tools-0.4.0/test/test_utils.py` & `optim_esm_tools-0.5.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/test/test_viewer.py` & `optim_esm_tools-0.5.0/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/test/test_workflow.py` & `optim_esm_tools-0.5.0/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.4.0/test/test_xarray_tools.py` & `optim_esm_tools-0.5.0/test/test_xarray_tools.py`

 * *Files identical despite different names*

