# Comparing `tmp/pycrispr-1.0.1.tar.gz` & `tmp/pycrispr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrispr-1.0.1.tar", last modified: Fri Jul  7 11:49:27 2023, max compression
+gzip compressed data, was "pycrispr-1.2.0.tar", last modified: Wed Jul 12 07:09:24 2023, max compression
```

## Comparing `pycrispr-1.0.1.tar` & `pycrispr-1.2.0.tar`

### file list

```diff
@@ -1,51 +1,59 @@
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-07 11:49:27.664035 pycrispr-1.0.1/
--rw-rw-r--   0 niek      (1000) niek      (1000)     1849 2023-06-21 08:40:56.000000 pycrispr-1.0.1/.gitignore
--rw-rw-r--   0 niek      (1000) niek      (1000)      335 2023-06-02 09:16:34.000000 pycrispr-1.0.1/CITATION.cff
--rw-rw-r--   0 niek      (1000) niek      (1000)    35149 2023-06-02 09:16:34.000000 pycrispr-1.0.1/LICENSE
--rw-rw-r--   0 niek      (1000) niek      (1000)      251 2023-07-07 10:38:46.000000 pycrispr-1.0.1/MANIFEST.in
--rw-rw-r--   0 niek      (1000) niek      (1000)      879 2023-07-07 11:49:27.664035 pycrispr-1.0.1/PKG-INFO
--rw-rw-r--   0 niek      (1000) niek      (1000)      123 2023-06-02 09:16:34.000000 pycrispr-1.0.1/README.md
--rw-rw-r--   0 niek      (1000) niek      (1000)      247 2023-07-07 11:41:49.000000 pycrispr-1.0.1/README.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)        0 2023-07-07 09:26:39.000000 pycrispr-1.0.1/__init__.py
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-07 11:49:27.660035 pycrispr-1.0.1/docs/
--rw-rw-r--   0 niek      (1000) niek      (1000)      638 2023-06-02 09:16:34.000000 pycrispr-1.0.1/docs/Makefile
--rw-rw-r--   0 niek      (1000) niek      (1000)      804 2023-06-02 09:16:34.000000 pycrispr-1.0.1/docs/make.bat
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-07 11:49:27.660035 pycrispr-1.0.1/docs/source/
--rw-rw-r--   0 niek      (1000) niek      (1000)      955 2023-07-05 13:55:11.000000 pycrispr-1.0.1/docs/source/conf.py
--rw-rw-r--   0 niek      (1000) niek      (1000)     1050 2023-07-07 09:50:16.000000 pycrispr-1.0.1/docs/source/index.rst
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-07 11:49:27.660035 pycrispr-1.0.1/pycrispr/
--rw-rw-r--   0 niek      (1000) niek      (1000)        0 2023-07-07 09:21:22.000000 pycrispr-1.0.1/pycrispr/__init__.py
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-07 11:49:27.660035 pycrispr-1.0.1/pycrispr/scripts/
--rw-rw-r--   0 niek      (1000) niek      (1000)        0 2023-07-07 09:21:29.000000 pycrispr-1.0.1/pycrispr/scripts/__init__.py
--rw-r--r--   0 niek      (1000) niek      (1000)     6025 2023-07-07 11:49:06.000000 pycrispr-1.0.1/pycrispr/scripts/pycrispr.py
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-07 11:49:27.664035 pycrispr-1.0.1/pycrispr/scripts/src/
--rw-rw-r--   0 niek      (1000) niek      (1000)      111 2023-07-06 09:36:57.000000 pycrispr-1.0.1/pycrispr/scripts/src/count.yaml
--rw-rw-r--   0 niek      (1000) niek      (1000)     2320 2023-06-15 07:36:30.000000 pycrispr-1.0.1/pycrispr/scripts/src/flute.R
--rw-r--r--   0 niek      (1000) niek      (1000)      180 2023-07-03 14:48:04.000000 pycrispr-1.0.1/pycrispr/scripts/src/flute.yaml
--rw-r--r--   0 niek      (1000) niek      (1000)       80 2023-07-06 09:37:41.000000 pycrispr-1.0.1/pycrispr/scripts/src/join.yaml
--rw-r--r--   0 niek      (1000) niek      (1000)      112 2023-07-06 09:37:54.000000 pycrispr-1.0.1/pycrispr/scripts/src/mageck.yaml
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-07 11:49:27.664035 pycrispr-1.0.1/pycrispr/scripts/src/python/
--rw-r--r--   0 niek      (1000) niek      (1000)     1213 2023-06-20 21:04:06.000000 pycrispr-1.0.1/pycrispr/scripts/src/python/join.py
--rw-r--r--   0 niek      (1000) niek      (1000)     2598 2023-06-20 21:17:15.000000 pycrispr-1.0.1/pycrispr/scripts/src/python/plot.py
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-07 11:49:27.664035 pycrispr-1.0.1/pycrispr/scripts/src/report/
--rw-rw-r--   0 niek      (1000) niek      (1000)       15 2023-06-19 10:11:24.000000 pycrispr-1.0.1/pycrispr/scripts/src/report/alignment-rates.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       27 2023-06-19 10:51:05.000000 pycrispr-1.0.1/pycrispr/scripts/src/report/dot-plot_neg.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       27 2023-06-19 10:49:49.000000 pycrispr-1.0.1/pycrispr/scripts/src/report/dot-plot_pos.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       13 2023-06-19 10:53:22.000000 pycrispr-1.0.1/pycrispr/scripts/src/report/mageck.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       12 2023-06-19 10:11:15.000000 pycrispr-1.0.1/pycrispr/scripts/src/report/multiqc.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       33 2023-06-19 10:11:39.000000 pycrispr-1.0.1/pycrispr/scripts/src/report/plot-coverage.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       22 2023-06-19 10:19:19.000000 pycrispr-1.0.1/pycrispr/scripts/src/report/report.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       15 2023-06-19 10:50:28.000000 pycrispr-1.0.1/pycrispr/scripts/src/report/sgrank.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       12 2023-06-19 10:51:18.000000 pycrispr-1.0.1/pycrispr/scripts/src/report/volcano.rst
--rw-r--r--   0 niek      (1000) niek      (1000)     7519 2023-06-23 06:59:44.000000 pycrispr-1.0.1/pycrispr/scripts/src/snakefile
--rw-r--r--   0 niek      (1000) niek      (1000)      110 2023-07-06 09:35:08.000000 pycrispr-1.0.1/pycrispr/scripts/src/trim.yaml
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-07 11:49:27.660035 pycrispr-1.0.1/pycrispr.egg-info/
--rw-rw-r--   0 niek      (1000) niek      (1000)      879 2023-07-07 11:49:27.000000 pycrispr-1.0.1/pycrispr.egg-info/PKG-INFO
--rw-r--r--   0 niek      (1000) niek      (1000)     1115 2023-07-07 11:49:27.000000 pycrispr-1.0.1/pycrispr.egg-info/SOURCES.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)        1 2023-07-07 11:49:27.000000 pycrispr-1.0.1/pycrispr.egg-info/dependency_links.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)       59 2023-07-07 11:49:27.000000 pycrispr-1.0.1/pycrispr.egg-info/entry_points.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)       26 2023-07-07 11:49:27.000000 pycrispr-1.0.1/pycrispr.egg-info/requires.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)        9 2023-07-07 11:49:27.000000 pycrispr-1.0.1/pycrispr.egg-info/top_level.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)        0 2023-06-02 09:16:34.000000 pycrispr-1.0.1/pyproject.toml
--rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-07 11:49:27.664035 pycrispr-1.0.1/setup.cfg
--rw-r--r--   0 niek      (1000) niek      (1000)     1198 2023-07-07 11:48:53.000000 pycrispr-1.0.1/setup.py
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-12 07:09:24.693450 pycrispr-1.2.0/
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1833 2023-07-11 12:36:21.000000 pycrispr-1.2.0/.gitignore
+-rw-rw-r--   0 niek      (1000) niek      (1000)      756 2023-07-11 11:38:39.000000 pycrispr-1.2.0/CITATION.cff
+-rw-rw-r--   0 niek      (1000) niek      (1000)    35149 2023-06-02 09:16:34.000000 pycrispr-1.2.0/LICENSE
+-rw-rw-r--   0 niek      (1000) niek      (1000)      251 2023-07-07 10:38:46.000000 pycrispr-1.2.0/MANIFEST.in
+-rw-rw-r--   0 niek      (1000) niek      (1000)      879 2023-07-12 07:09:24.693450 pycrispr-1.2.0/PKG-INFO
+-rw-rw-r--   0 niek      (1000) niek      (1000)      123 2023-06-02 09:16:34.000000 pycrispr-1.2.0/README.md
+-rw-rw-r--   0 niek      (1000) niek      (1000)      247 2023-07-07 11:41:49.000000 pycrispr-1.2.0/README.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)        0 2023-07-07 09:26:39.000000 pycrispr-1.2.0/__init__.py
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-12 07:09:24.689450 pycrispr-1.2.0/docs/
+-rw-rw-r--   0 niek      (1000) niek      (1000)      638 2023-06-02 09:16:34.000000 pycrispr-1.2.0/docs/Makefile
+-rw-rw-r--   0 niek      (1000) niek      (1000)      804 2023-06-02 09:16:34.000000 pycrispr-1.2.0/docs/make.bat
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-12 07:09:24.689450 pycrispr-1.2.0/docs/source/
+-rw-rw-r--   0 niek      (1000) niek      (1000)      955 2023-07-05 13:55:11.000000 pycrispr-1.2.0/docs/source/conf.py
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1050 2023-07-07 09:50:16.000000 pycrispr-1.2.0/docs/source/index.rst
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-12 07:09:24.689450 pycrispr-1.2.0/pycrispr/
+-rw-rw-r--   0 niek      (1000) niek      (1000)        0 2023-07-07 09:21:22.000000 pycrispr-1.2.0/pycrispr/__init__.py
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-12 07:09:24.689450 pycrispr-1.2.0/pycrispr/scripts/
+-rw-rw-r--   0 niek      (1000) niek      (1000)        0 2023-07-07 09:21:29.000000 pycrispr-1.2.0/pycrispr/scripts/__init__.py
+-rw-r--r--   0 niek      (1000) niek      (1000)     6522 2023-07-11 08:21:55.000000 pycrispr-1.2.0/pycrispr/scripts/pycrispr.py
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-12 07:09:24.693450 pycrispr-1.2.0/pycrispr/scripts/src/
+-rw-rw-r--   0 niek      (1000) niek      (1000)      111 2023-07-06 09:36:57.000000 pycrispr-1.2.0/pycrispr/scripts/src/count.yaml
+-rw-rw-r--   0 niek      (1000) niek      (1000)     2320 2023-06-15 07:36:30.000000 pycrispr-1.2.0/pycrispr/scripts/src/flute.R
+-rw-r--r--   0 niek      (1000) niek      (1000)      180 2023-07-03 14:48:04.000000 pycrispr-1.2.0/pycrispr/scripts/src/flute.yaml
+-rw-r--r--   0 niek      (1000) niek      (1000)       80 2023-07-06 09:37:41.000000 pycrispr-1.2.0/pycrispr/scripts/src/join.yaml
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-12 07:09:24.693450 pycrispr-1.2.0/pycrispr/scripts/src/python/
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1620 2023-07-11 08:35:49.000000 pycrispr-1.2.0/pycrispr/scripts/src/python/bagel2bf.py
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1027 2023-07-10 14:27:35.000000 pycrispr-1.2.0/pycrispr/scripts/src/python/bagel2fc.py
+-rw-rw-r--   0 niek      (1000) niek      (1000)      793 2023-07-11 07:25:14.000000 pycrispr-1.2.0/pycrispr/scripts/src/python/bagel2pr.py
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1971 2023-07-10 09:53:48.000000 pycrispr-1.2.0/pycrispr/scripts/src/python/convert_count_table.py
+-rw-r--r--   0 niek      (1000) niek      (1000)     1213 2023-06-20 21:04:06.000000 pycrispr-1.2.0/pycrispr/scripts/src/python/join.py
+-rw-r--r--   0 niek      (1000) niek      (1000)     2597 2023-07-11 08:15:44.000000 pycrispr-1.2.0/pycrispr/scripts/src/python/plot.py
+-rw-rw-r--   0 niek      (1000) niek      (1000)      596 2023-07-11 08:34:05.000000 pycrispr-1.2.0/pycrispr/scripts/src/python/plot_bf.py
+-rw-rw-r--   0 niek      (1000) niek      (1000)      538 2023-07-11 08:25:24.000000 pycrispr-1.2.0/pycrispr/scripts/src/python/plot_pr.py
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-12 07:09:24.693450 pycrispr-1.2.0/pycrispr/scripts/src/report/
+-rw-rw-r--   0 niek      (1000) niek      (1000)       15 2023-06-19 10:11:24.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/alignment-rates.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       13 2023-07-11 08:40:10.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/bagel2.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       19 2023-07-11 08:43:33.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/bagel2_plots.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       27 2023-06-19 10:51:05.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/dot-plot_neg.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       27 2023-06-19 10:49:49.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/dot-plot_pos.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       13 2023-06-19 10:53:22.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/mageck.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       12 2023-06-19 10:11:15.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/multiqc.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       33 2023-06-19 10:11:39.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/plot-coverage.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       22 2023-06-19 10:19:19.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/report.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       15 2023-06-19 10:50:28.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/sgrank.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       12 2023-06-19 10:51:18.000000 pycrispr-1.2.0/pycrispr/scripts/src/report/volcano.rst
+-rw-r--r--   0 niek      (1000) niek      (1000)    11200 2023-07-11 09:09:25.000000 pycrispr-1.2.0/pycrispr/scripts/src/snakefile
+-rw-r--r--   0 niek      (1000) niek      (1000)      224 2023-07-11 07:05:44.000000 pycrispr-1.2.0/pycrispr/scripts/src/stats.yaml
+-rw-r--r--   0 niek      (1000) niek      (1000)      110 2023-07-06 09:35:08.000000 pycrispr-1.2.0/pycrispr/scripts/src/trim.yaml
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-12 07:09:24.689450 pycrispr-1.2.0/pycrispr.egg-info/
+-rw-rw-r--   0 niek      (1000) niek      (1000)      879 2023-07-12 07:09:24.000000 pycrispr-1.2.0/pycrispr.egg-info/PKG-INFO
+-rw-r--r--   0 niek      (1000) niek      (1000)     1447 2023-07-12 07:09:24.000000 pycrispr-1.2.0/pycrispr.egg-info/SOURCES.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)        1 2023-07-12 07:09:24.000000 pycrispr-1.2.0/pycrispr.egg-info/dependency_links.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)       59 2023-07-12 07:09:24.000000 pycrispr-1.2.0/pycrispr.egg-info/entry_points.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)       26 2023-07-12 07:09:24.000000 pycrispr-1.2.0/pycrispr.egg-info/requires.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)        9 2023-07-12 07:09:24.000000 pycrispr-1.2.0/pycrispr.egg-info/top_level.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)        0 2023-06-02 09:16:34.000000 pycrispr-1.2.0/pyproject.toml
+-rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-12 07:09:24.693450 pycrispr-1.2.0/setup.cfg
+-rw-r--r--   0 niek      (1000) niek      (1000)     1198 2023-07-11 08:21:47.000000 pycrispr-1.2.0/setup.py
```

### Comparing `pycrispr-1.0.1/.gitignore` & `pycrispr-1.2.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 *~
 .Rhistory
 .gitignore
 .vscode/
-experiment.yaml
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `pycrispr-1.0.1/LICENSE` & `pycrispr-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrispr-1.0.1/PKG-INFO` & `pycrispr-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrispr
-Version: 1.0.1
+Version: 1.2.0
 Summary: A package for CRISPR-Cas9 screen analysis
 Author: Niek Wit
 Author-email: nw416@cam.ac.uk
 License: GPL-3.0 license
 Project-URL: Documentation, https://pycrispr.readthedocs.io/
 Project-URL: Source, https://github.com/niekwit/pycrispr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycrispr-1.0.1/docs/Makefile` & `pycrispr-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycrispr-1.0.1/docs/make.bat` & `pycrispr-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pycrispr-1.0.1/docs/source/conf.py` & `pycrispr-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pycrispr-1.0.1/docs/source/index.rst` & `pycrispr-1.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pycrispr-1.0.1/pycrispr/scripts/pycrispr.py` & `pycrispr-1.2.0/pycrispr/scripts/pycrispr.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,26 +50,32 @@
               is_flag=True,
               help="Disable jobs from running in a Conda environment (not recommended)")
 @click.option("-d","--dryrun", 
               is_flag=True,
               help="Dry run for running pipeline (helpful for testing if pipeline works)")
 @click.option("-r","--cleanup", 
               is_flag=True,
-              help="Cleanup unused conda environments and packages")
+              help="Clean up unused conda environments and packages")
 @click.option("-v","--verbose", 
               show_default=True,
               is_flag=True,
               help="Increase verbosity")
 
 
 def analysis(threads,slurm,background,noconda,dryrun,cleanup,verbose):
     
     ''' Run CRISPR-Cas9 screen analysis pipeline
     '''
+    #load experiment settings
+    config = loadYaml()
+    stats = config["stats"]["type"]
+    
+    
     if cleanup:
+        
         click.secho("Cleaning up unused Conda packages and environment...",fg="green")
         subprocess.run("snakemake --cores 1 --conda-cleanup-envs --conda-cleanup-pkgs cache", shell=True)
         click.secho("Done!",fg="green")
         sys.exit(0)
     
     click.secho("CRISPR-Cas9 screen analysis with pycrispr",fg="green")
     
@@ -88,90 +94,118 @@
     shutil.copyfile(flute_file,flute_dest)
     
     #copy Python scripts to work_dir
     python_files = glob.glob(os.path.join(script_dir,"src","python","*.py"))
     [shutil.copyfile(x,os.path.join(work_dir,"scripts",os.path.basename(x))) for x in python_files]
     
     #plot DAG
-    if not os.path.exists("dag.pdf"):
-        click.echo("Plotting snakemake DAG")
-        dag = "snakemake --forceall --dag | grep -v '\-> 0\|0\[label = \"all\"' |dot -Tpdf > dag.pdf"
-        process=subprocess.check_output(dag,shell=True)
+    if stats == "mageck":
+        
+        file = "dag-mageck.pdf"
+    
+    elif stats == "bagel2":
         
+        file = "dag-bagel2.pdf"    
+            
+    if not os.path.exists(file):
+        
+        click.echo(f"Plotting snakemake DAG for {stats}...")
+        dag = f"snakemake --forceall --dag | grep -v '\-> 0\|0\[label = \"all\"' |dot -Tpdf > {file}" 
+        process=subprocess.check_output(dag,shell=True)
+         
     #construct snakemake command
     snakemake = "snakemake --output-wait 20" 
+    
     if not noconda:
+        
         snakemake = f"{snakemake} --use-conda" 
+    
     if verbose:
+        
         snakemake = f"{snakemake} -p" #prints shell commands
+    
     if dryrun:
+        
         click.echo("Dry run only")
         snakemake = f"{snakemake} -n"
+    
     if slurm:
-        click.echo("Submitting pipeline to Slurm workload manager")
+        
+        click.echo("Submitting jobs to Slurm workload manager...")
         #load slurm default resources
-        slurm = loadYaml()
-        account = slurm["resources"]["account"]
-        partition = slurm["resources"]["partition"]
-        max_jobs = slurm["resources"]["max_jobs"]
+        account = config["resources"]["account"]
+        partition = config["resources"]["partition"]
+        max_jobs = config["resources"]["max_jobs"]
         
         snakemake = f"{snakemake} --slurm -j {max_jobs} --default-resources slurm_account={account} slurm_partition={partition}" #run snakemake in background with nohup
+    
     else:
+        
         snakemake = f"{snakemake} --cores {threads}"
     
     #copy conda envs yamls to work_dir
     conda_envs = glob.glob(os.path.join(script_dir,"src","*.yaml"))
     os.makedirs("envs",exist_ok = True)
     [shutil.copyfile(x,os.path.join(work_dir,"envs",os.path.basename(x))) for x in conda_envs]
         
     #run snakemake command    
     if not os.path.isdir(".snakemake/"): #this dir does not exist before first run
+        
         if background: #check if it needs to run in the background (nohup)
+            
             os.makedirs("logs", exist_ok=True)
             snakemake = f"nohup {snakemake} >> logs/terminal.log &"
             bg_msg()
         subprocess.run(snakemake, shell=True)
+    
     else: #if it has run before, it probably failed at some step so rerun all failed rules
         snakemake = f"{snakemake} --rerun-incomplete"
+        
         if background:
+            
             os.makedirs("logs", exist_ok=True)
             snakemake = f"nohup {snakemake} >> logs/terminal.log &"
             bg_msg()
+        
         subprocess.run(snakemake, shell=True)
 
 
 @click.command(name='report')
 
 def report():
     
     ''' Create HTML report of analysis
     '''
+    #load experiment settings
+    config = loadYaml()
+    stats = config["stats"]["type"]
+    
     #create report for previous pipeline run
     click.secho("Creating report of analysis...",fg="green")
     
     #copy report files to work_dir
     shutil.copytree(os.path.join(script_dir,"src","report"),
                     os.path.join(work_dir,"report"), 
                     dirs_exist_ok=True)
         
     #create command
-    report = "snakemake --report pycrispr-report.html"
+    report = f"snakemake --report pycrispr_{stats}-report.html"
     
     #run command
     subprocess.run(report, shell=True)
     return
 
 
 @click.command(name='version')
 
 def version():
     
     ''' Display version of pycrispr
     '''
-    version = "1.0.1"
+    version = "1.2.0"
     
     #create report for previous pipeline run
     click.secho(f"pycrispr v{version}",fg="green")
     
     return
            
 #add subparsers
```

### Comparing `pycrispr-1.0.1/pycrispr/scripts/src/flute.R` & `pycrispr-1.2.0/pycrispr/scripts/src/flute.R`

 * *Files identical despite different names*

### Comparing `pycrispr-1.0.1/pycrispr/scripts/src/python/join.py` & `pycrispr-1.2.0/pycrispr/scripts/src/python/join.py`

 * *Files identical despite different names*

### Comparing `pycrispr-1.0.1/pycrispr/scripts/src/python/plot.py` & `pycrispr-1.2.0/pycrispr/scripts/src/python/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     '''General plotting function
     '''
     sns.set_style("white")
     sns.set_style("ticks")
     sns.barplot(x=list(df.keys())[0],
                     y=list(df.keys())[1],
                     data=df,
-                    color="royalblue",
+                    color="seagreen",
                     edgecolor="black",
                     linewidth=1)
     plt.ylabel(y_label)
     plt.xticks(rotation = 'vertical')
     plt.xlabel("")
     plt.tight_layout()
     sns.despine()
```

### Comparing `pycrispr-1.0.1/pycrispr/scripts/src/snakefile` & `pycrispr-1.2.0/pycrispr/scripts/src/snakefile`

 * *Files 21% similar despite different names*

```diff
@@ -8,68 +8,93 @@
 configfile: "experiment.yaml"
 
 #load variables
 library = config["library"]
 fasta = config["lib_info"][library]["fasta"]
 index = config["lib_info"][library]["index"]
 sg_length = config["lib_info"][library]["sg_length"]
+stats = config["stats"]["type"]
 
 #check if read files need to be renamed
 if "rename" in config and not os.path.exists("rename.done"):
+    
     OLD_FILES = list(config["rename"].keys())
     NEW_FILES = list(config["rename"].values())
 
     #create sample names
     SAMPLES = [x.replace(".fq.gz","") for x in NEW_FILES]
 else:
+    
     #create sample names
     SAMPLES = [os.path.basename(x).replace(".fq.gz","") for x in glob.glob("reads/*fq.gz")]
     #remove any pre-existing trimmed fq files from this list
     SAMPLES = [x for x in SAMPLES if not "_trimmed" in x]
 
-#load mageck settings
-COMPARISONS = [value.replace(",","-") for (key,value) in config["stats"]["comparisons"].items()]
+#load stats comparisons
+COMPARISONS = [value.replace(",","-") for (key,value) in config["stats"]["comparisons"].items()] #commas are not compatible with snakemake report
+
+if stats == "bagel2": #remove comparisons with pooled control samples (not supported by BAGEL2)
+    
+    COMPARISONS = [x for x in COMPARISONS if not "-" in x.split("_vs_")[1]]
+
 
 #set targets for target rule
 TARGETS = [expand("qc/fastqc/{sample}.html", sample=SAMPLES),
-        expand("qc/fastqc/{sample}_fastqc.zip", sample=SAMPLES),
-        "qc/multiqc.html",
-        "count/alignment-rates.pdf",
-        "count/sequence-coverage.pdf",
+            expand("qc/fastqc/{sample}_fastqc.zip", sample=SAMPLES),
+            "qc/multiqc.html",
+            "count/alignment-rates.pdf",
+            "count/sequence-coverage.pdf"
+            ]
+
+if stats == "mageck":
+    
+    TARGETS.extend([
         expand("mageck/{comparison}.gene_summary.txt", comparison=COMPARISONS),
         expand("mageck/{comparison}.sgrna_summary.txt", comparison=COMPARISONS),
         expand("mageck_flute/{comparison}.volcano.pdf", comparison=COMPARISONS),
         expand("mageck_flute/{comparison}.dot_pos.pdf", comparison=COMPARISONS),
         expand("mageck_flute/{comparison}.dot_neg.pdf", comparison=COMPARISONS),
         expand("mageck_flute/{comparison}.sgrank.pdf", comparison=COMPARISONS)
-        ]
+    ])
+
+elif stats == "bagel2":
+    TARGETS.extend([
+       "count/counts-aggregated-bagel2.tsv",
+        expand("bagel2/{comparison}.foldchange", comparison=COMPARISONS),
+        expand("bagel2/{comparison}.bf", comparison=COMPARISONS),
+        expand("bagel2/{comparison}.pr", comparison=COMPARISONS),
+        expand("bagel2_plots/{comparison}.bf.pdf", comparison=COMPARISONS),
+        expand("bagel2_plots/{comparison}.pr.pdf", comparison=COMPARISONS),
+    ])
 
 
 
 ####SNAKEMAKE RULES####
 
 #report location
 report: "report/report.rst"
 
 #rules to be run on login node instead of compute node when running on HPC (only very small jobs)
-localrules: all, rename, join, plot_alignment_rate, plot_coverage  
+localrules: all, rename, join, plot_alignment_rate, plot_coverage, plot_bf, plot_pr
 
 #extend TARGETS with renamed files if required
 if "rename" in config and not os.path.exists("rename.done"):
+    
     TARGETS.extend(expand("reads/{new_file}", new_file=NEW_FILES)),
     TARGETS.append("rename.done")
 
 
 #set target rule
 rule all:
     input:
         TARGETS
 
 
 if "rename" in config and not os.path.exists("rename.done"):
+    
     rule rename:
         input:
             expand("reads/{old_file}", old_file=OLD_FILES)
         output:
             f=expand("reads/{new_file}", new_file=NEW_FILES),
             t=touch("rename.done"),
         run:
@@ -113,15 +138,15 @@
 rule trim:
     input:
         "reads/{sample}.fq.gz"
     output:
         temp("reads/{sample}_trimmed.fq.gz")
     params:
         sgl=sg_length,
-        lt=config["left_trim"],
+        lt=config["lib_info"][library]["left_trim"],
     threads: config["resources"]["trim"]["cpu"]
     conda:
         "envs/trim.yaml"
     log:
         "logs/trim/{sample}.log",
     resources:
         runtime=config["resources"]["trim"]["time"]
@@ -156,54 +181,148 @@
         "count/counts-aggregated.tsv"
     params:
         fa=fasta,
     script:
         "scripts/join.py"
 
 
-rule mageck:
-    input: 
-        "count/counts-aggregated.tsv"
-    output:
-        "mageck/{comparison}_summary.Rnw",
-        report("mageck/{comparison}.gene_summary.txt", caption="report/mageck.rst", category="MAGeCK"),
-        "mageck/{comparison}.log",
-        "mageck/{comparison}.R",
-        #"mageck/{comparison}.report.Rmd",
-        "mageck/{comparison}.sgrna_summary.txt",
-        "mageck/{comparison}.normalized.txt"
-    resources:
-        runtime=config["resources"]["mageck"]["time"]
-    conda:
-        "envs/mageck.yaml"
-    log:
-        "logs/mageck/{comparison}.log"
-    shell:
-        '''
-        mageck test --normcounts-to-file -k {input} -t $(echo "{wildcards.comparison}" | sed 's/_vs_.*//' | sed 's/-/,/') -c $(echo "{wildcards.comparison}" | sed 's/^[^_vs_]*_vs_//' | sed 's/-/,/') -n mageck/{wildcards.comparison} 2> {log}
-        '''
+if stats == "mageck":
+    
+    rule mageck:
+        input: 
+            "count/counts-aggregated.tsv"
+        output:
+            "mageck/{comparison}_summary.Rnw",
+            report("mageck/{comparison}.gene_summary.txt", caption="report/mageck.rst", category="MAGeCK"),
+            "mageck/{comparison}.log",
+            "mageck/{comparison}.R",
+            "mageck/{comparison}.sgrna_summary.txt",
+            "mageck/{comparison}.normalized.txt"
+        resources:
+            runtime=config["resources"]["stats"]["time"]
+        conda:
+            "envs/stats.yaml"
+        log:
+            "logs/mageck/{comparison}.log"
+        shell:
+            '''
+            mageck test --normcounts-to-file -k {input} -t $(echo "{wildcards.comparison}" | sed 's/_vs_.*//' | sed 's/-/,/') -c $(echo "{wildcards.comparison}" | sed 's/^[^_vs_]*_vs_//' | sed 's/-/,/') -n mageck/{wildcards.comparison} 2> {log}
+            '''
 
 
-rule mageck_flute:
-    input:
-        "mageck/{comparison}.gene_summary.txt",
-        "mageck/{comparison}.sgrna_summary.txt"
-    output:
-        report("mageck_flute/{comparison}.volcano.pdf", caption="report/volcano.rst", category="MAGeCK Flute", subcategory="{comparison}", labels={"Comparison":"{comparison}","Figure": "volcano plot"}),
-        report("mageck_flute/{comparison}.dot_pos.pdf", caption="report/dot-plot_pos.rst", category="MAGeCK Flute", subcategory="{comparison}", labels={"Comparison":"{comparison}","Figure": "dot plot enriched genes"}),
-        report("mageck_flute/{comparison}.dot_neg.pdf", caption="report/dot-plot_neg.rst", category="MAGeCK Flute", subcategory="{comparison}", labels={"Comparison":"{comparison}","Figure": "dot plot depleted genes"}),
-        report("mageck_flute/{comparison}.sgrank.pdf", caption="report/sgrank.rst", category="MAGeCK Flute", subcategory="{comparison}", labels={"Comparison":"{comparison}","Figure": "sgRNA rank"}),
-    params:
-        spc=config["lib_info"][library]["species"],
-    resources:
-        runtime=config["resources"]["mageck"]["time"]
-    conda:
-        "envs/flute.yaml"
-    script:
-        "scripts/flute.R"
+    rule mageck_flute:
+        input:
+            "mageck/{comparison}.gene_summary.txt",
+            "mageck/{comparison}.sgrna_summary.txt"
+        output:
+            report("mageck_flute/{comparison}.volcano.pdf", caption="report/volcano.rst", category="MAGeCK Flute", subcategory="{comparison}", labels={"Comparison":"{comparison}","Figure": "volcano plot"}),
+            report("mageck_flute/{comparison}.dot_pos.pdf", caption="report/dot-plot_pos.rst", category="MAGeCK Flute", subcategory="{comparison}", labels={"Comparison":"{comparison}","Figure": "dot plot enriched genes"}),
+            report("mageck_flute/{comparison}.dot_neg.pdf", caption="report/dot-plot_neg.rst", category="MAGeCK Flute", subcategory="{comparison}", labels={"Comparison":"{comparison}","Figure": "dot plot depleted genes"}),
+            report("mageck_flute/{comparison}.sgrank.pdf", caption="report/sgrank.rst", category="MAGeCK Flute", subcategory="{comparison}", labels={"Comparison":"{comparison}","Figure": "sgRNA rank"}),
+        params:
+            spc=config["lib_info"][library]["species"]
+        resources:
+            runtime=config["resources"]["stats"]["time"]
+        conda:
+            "envs/flute.yaml"
+        script:
+            "scripts/flute.R"
+
+
+elif stats == "bagel2":
+    
+    rule convert_count_table:
+        input:
+            "count/counts-aggregated.tsv"
+        output:
+            "count/counts-aggregated-bagel2.tsv"
+        params:
+            fa=fasta,
+            b2dir=config["stats"]["bagel2_dir"]
+        resources:
+            runtime=config["resources"]["stats"]["time"]
+        conda:
+            "envs/stats.yaml"
+        script:
+            "scripts/convert_count_table.py"
+    
+    
+    rule bagel2fc:
+        input:
+            "count/counts-aggregated-bagel2.tsv"
+        output:
+            "bagel2/{comparison}.foldchange"
+        params:
+            b2dir=config["stats"]["bagel2_dir"]
+        resources:
+            runtime=config["resources"]["stats"]["time"]
+        conda:
+            "envs/stats.yaml"
+        log:
+            "logs/bagel2/fc_{comparison}.log"
+        script:
+            "scripts/bagel2fc.py"
+
+
+    rule bagel2bf:
+        input:
+            "bagel2/{comparison}.foldchange"
+        output:
+            "bagel2/{comparison}.bf"
+        params:
+            b2dir=config["stats"]["bagel2_dir"],
+            species=config["lib_info"][library]["species"],
+        resources:
+            runtime=config["resources"]["stats"]["time"]
+        conda:
+            "envs/stats.yaml"
+        log:
+            "logs/bagel2/bf_{comparison}.log"
+        script:
+            "scripts/bagel2bf.py"
+
+
+    rule bagel2pr:
+        input:
+            "bagel2/{comparison}.bf"
+        output:
+            report("bagel2/{comparison}.pr", caption="report/bagel2.rst", category="BAGEL2")
+        params:
+            b2dir=config["stats"]["bagel2_dir"],
+            species=config["lib_info"][library]["species"]
+        resources:
+            runtime=config["resources"]["stats"]["time"]
+        conda:
+            "envs/stats.yaml"
+        log:
+            "logs/bagel2/pr_{comparison}.log"
+        script:
+            "scripts/bagel2pr.py"
+
+
+    rule plot_bf:
+        input:
+            "bagel2/{comparison}.bf"
+        output:
+            report("bagel2_plots/{comparison}.bf.pdf", caption="report/bagel2_plots.rst", category="BAGEL2 plots", subcategory="{comparison}", labels={"Comparison":"{comparison}", "Figure":"BF plot"})
+        conda:
+            "envs/stats.yaml"
+        script:
+            "scripts/plot_bf.py"
+
+
+    rule plot_pr:
+        input:
+            "bagel2/{comparison}.pr"
+        output:
+            report("bagel2_plots/{comparison}.pr.pdf", caption="report/bagel2_plots.rst", category="BAGEL2 plots", subcategory="{comparison}", labels={"Comparison":"{comparison}", "Figure":"Precision-recall plot"})
+        conda:
+            "envs/stats.yaml"
+        script:
+            "scripts/plot_pr.py"
 
 
 rule plot_alignment_rate:
     input:
         expand("logs/count/{sample}.log", sample=SAMPLES)
     output:
         report("count/alignment-rates.pdf", caption="report/alignment-rates.rst", category="Alignment rates")
@@ -211,15 +330,15 @@
         name="plot_alignment_rate",
     script:
         "scripts/plot.py"
 
 
 rule plot_coverage:
     input:
-        "count/counts-aggregated.tsv",
+        "count/counts-aggregated.tsv"
     params:
         name="plot_coverage",
         fa=fasta,
     output:
         report("count/sequence-coverage.pdf", caption="report/plot-coverage.rst", category="Sequence coverage")
     script:
         "scripts/plot.py"
```

### Comparing `pycrispr-1.0.1/pycrispr.egg-info/PKG-INFO` & `pycrispr-1.2.0/pycrispr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrispr
-Version: 1.0.1
+Version: 1.2.0
 Summary: A package for CRISPR-Cas9 screen analysis
 Author: Niek Wit
 Author-email: nw416@cam.ac.uk
 License: GPL-3.0 license
 Project-URL: Documentation, https://pycrispr.readthedocs.io/
 Project-URL: Source, https://github.com/niekwit/pycrispr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycrispr-1.0.1/pycrispr.egg-info/SOURCES.txt` & `pycrispr-1.2.0/pycrispr.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,20 +20,28 @@
 pycrispr.egg-info/top_level.txt
 pycrispr/scripts/__init__.py
 pycrispr/scripts/pycrispr.py
 pycrispr/scripts/src/count.yaml
 pycrispr/scripts/src/flute.R
 pycrispr/scripts/src/flute.yaml
 pycrispr/scripts/src/join.yaml
-pycrispr/scripts/src/mageck.yaml
 pycrispr/scripts/src/snakefile
+pycrispr/scripts/src/stats.yaml
 pycrispr/scripts/src/trim.yaml
+pycrispr/scripts/src/python/bagel2bf.py
+pycrispr/scripts/src/python/bagel2fc.py
+pycrispr/scripts/src/python/bagel2pr.py
+pycrispr/scripts/src/python/convert_count_table.py
 pycrispr/scripts/src/python/join.py
 pycrispr/scripts/src/python/plot.py
+pycrispr/scripts/src/python/plot_bf.py
+pycrispr/scripts/src/python/plot_pr.py
 pycrispr/scripts/src/report/alignment-rates.rst
+pycrispr/scripts/src/report/bagel2.rst
+pycrispr/scripts/src/report/bagel2_plots.rst
 pycrispr/scripts/src/report/dot-plot_neg.rst
 pycrispr/scripts/src/report/dot-plot_pos.rst
 pycrispr/scripts/src/report/mageck.rst
 pycrispr/scripts/src/report/multiqc.rst
 pycrispr/scripts/src/report/plot-coverage.rst
 pycrispr/scripts/src/report/report.rst
 pycrispr/scripts/src/report/sgrank.rst
```

### Comparing `pycrispr-1.0.1/setup.py` & `pycrispr-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name='pycrispr',
-    version='1.0.1',
+    version='1.2.0',
     py_modules=['pycrispr'], 
     description='A package for CRISPR-Cas9 screen analysis',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     project_urls={
         'Documentation': 'https://pycrispr.readthedocs.io/',
         'Source': 'https://github.com/niekwit/pycrispr',
```

