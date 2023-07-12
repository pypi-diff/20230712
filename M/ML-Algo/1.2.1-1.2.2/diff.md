# Comparing `tmp/ML-Algo-1.2.1.tar.gz` & `tmp/ML-Algo-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML-Algo-1.2.1.tar", last modified: Wed Jul 12 12:51:40 2023, max compression
+gzip compressed data, was "ML-Algo-1.2.2.tar", last modified: Wed Jul 12 12:59:47 2023, max compression
```

## Comparing `ML-Algo-1.2.1.tar` & `ML-Algo-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:51:40.058014 ML-Algo-1.2.1/
-drwxrwxrwx   0        0        0        0 2023-07-12 12:51:40.037982 ML-Algo-1.2.1/ML-Algo/
--rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.1/ML-Algo/DataCleaning.py
--rw-rw-rw-   0        0        0     1621 2023-07-12 09:59:29.000000 ML-Algo-1.2.1/ML-Algo/FetchData.py
--rw-rw-rw-   0        0        0      653 2023-07-12 09:48:44.000000 ML-Algo-1.2.1/ML-Algo/Predictions.py
--rw-rw-rw-   0        0        0     2456 2023-07-12 09:47:02.000000 ML-Algo-1.2.1/ML-Algo/Series_Data.py
--rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.1/ML-Algo/Series_Time.py
--rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.1/ML-Algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:51:40.053004 ML-Algo-1.2.1/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0      164 2023-07-12 12:51:39.000000 ML-Algo-1.2.1/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-12 12:51:39.000000 ML-Algo-1.2.1/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:51:39.000000 ML-Algo-1.2.1/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 12:51:39.000000 ML-Algo-1.2.1/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 12:51:39.000000 ML-Algo-1.2.1/ML_Algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      164 2023-07-12 12:51:40.056005 ML-Algo-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 12:51:40.058014 ML-Algo-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      277 2023-07-12 12:51:18.000000 ML-Algo-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:59:47.732002 ML-Algo-1.2.2/
+drwxrwxrwx   0        0        0        0 2023-07-12 12:59:47.723077 ML-Algo-1.2.2/ML_Algo/
+-rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.2/ML_Algo/DataCleaning.py
+-rw-rw-rw-   0        0        0     1621 2023-07-12 09:59:29.000000 ML-Algo-1.2.2/ML_Algo/FetchData.py
+-rw-rw-rw-   0        0        0      653 2023-07-12 09:48:44.000000 ML-Algo-1.2.2/ML_Algo/Predictions.py
+-rw-rw-rw-   0        0        0     2456 2023-07-12 09:47:02.000000 ML-Algo-1.2.2/ML_Algo/Series_Data.py
+-rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.2/ML_Algo/Series_Time.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.2/ML_Algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:59:47.729367 ML-Algo-1.2.2/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0      164 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      164 2023-07-12 12:59:47.730990 ML-Algo-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 12:59:47.732002 ML-Algo-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      277 2023-07-12 12:59:11.000000 ML-Algo-1.2.2/setup.py
```

### Comparing `ML-Algo-1.2.1/ML-Algo/DataCleaning.py` & `ML-Algo-1.2.2/ML_Algo/DataCleaning.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.1/ML-Algo/FetchData.py` & `ML-Algo-1.2.2/ML_Algo/FetchData.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.1/ML-Algo/Predictions.py` & `ML-Algo-1.2.2/ML_Algo/Predictions.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.1/ML-Algo/Series_Data.py` & `ML-Algo-1.2.2/ML_Algo/Series_Data.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.1/ML-Algo/Series_Time.py` & `ML-Algo-1.2.2/ML_Algo/Series_Time.py`

 * *Files identical despite different names*

