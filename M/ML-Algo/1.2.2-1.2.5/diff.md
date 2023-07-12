# Comparing `tmp/ML-Algo-1.2.2.tar.gz` & `tmp/ML-Algo-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML-Algo-1.2.2.tar", last modified: Wed Jul 12 12:59:47 2023, max compression
+gzip compressed data, was "ML-Algo-1.2.5.tar", last modified: Wed Jul 12 13:33:22 2023, max compression
```

## Comparing `ML-Algo-1.2.2.tar` & `ML-Algo-1.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:59:47.732002 ML-Algo-1.2.2/
-drwxrwxrwx   0        0        0        0 2023-07-12 12:59:47.723077 ML-Algo-1.2.2/ML_Algo/
--rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.2/ML_Algo/DataCleaning.py
--rw-rw-rw-   0        0        0     1621 2023-07-12 09:59:29.000000 ML-Algo-1.2.2/ML_Algo/FetchData.py
--rw-rw-rw-   0        0        0      653 2023-07-12 09:48:44.000000 ML-Algo-1.2.2/ML_Algo/Predictions.py
--rw-rw-rw-   0        0        0     2456 2023-07-12 09:47:02.000000 ML-Algo-1.2.2/ML_Algo/Series_Data.py
--rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.2/ML_Algo/Series_Time.py
--rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.2/ML_Algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:59:47.729367 ML-Algo-1.2.2/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0      164 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 12:59:47.000000 ML-Algo-1.2.2/ML_Algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      164 2023-07-12 12:59:47.730990 ML-Algo-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 12:59:47.732002 ML-Algo-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      277 2023-07-12 12:59:11.000000 ML-Algo-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:33:22.768912 ML-Algo-1.2.5/
+drwxrwxrwx   0        0        0        0 2023-07-12 13:33:22.753914 ML-Algo-1.2.5/ML_Algo/
+-rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.5/ML_Algo/DataCleaning.py
+-rw-rw-rw-   0        0        0     1629 2023-07-12 13:17:21.000000 ML-Algo-1.2.5/ML_Algo/FetchData.py
+-rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.2.5/ML_Algo/Predictions.py
+-rw-rw-rw-   0        0        0     2487 2023-07-12 13:21:48.000000 ML-Algo-1.2.5/ML_Algo/Series_Data.py
+-rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.5/ML_Algo/Series_Time.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.5/ML_Algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:33:22.765777 ML-Algo-1.2.5/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0      164 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      164 2023-07-12 13:33:22.767892 ML-Algo-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 13:33:22.768912 ML-Algo-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      288 2023-07-12 13:32:40.000000 ML-Algo-1.2.5/setup.py
```

### Comparing `ML-Algo-1.2.2/ML_Algo/DataCleaning.py` & `ML-Algo-1.2.5/ML_Algo/DataCleaning.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.2/ML_Algo/FetchData.py` & `ML-Algo-1.2.5/ML_Algo/FetchData.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import json
 import pandas as pd
-from Series_Time import *
+from ML_Algo.Series_Time import *
 
 def getData(date):  
     url =  'http://192.168.0.35:5060/ldat'
     param =  {
         "id": "10751",
         "reqdate": date
          # 04-06-2023
```

### Comparing `ML-Algo-1.2.2/ML_Algo/Series_Data.py` & `ML-Algo-1.2.5/ML_Algo/Series_Data.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 def combine_json_data(json_files):
     combined_df = pd.DataFrame()
 
     for index, json_data in enumerate(json_files):
         data = json_data['data']['10751']
         df = pd.DataFrame(data)
-        df['ts'] = pd.to_datetime(df['ts'])
+        df['ts'] = pd.to_datetime(df['ts'], format="%m/%d/%Y %I:%M:%S %p")
         df['ts'] = df['ts'].dt.strftime('%H:%M')
         df = df.drop('status', axis=1)
         
         cols = df.columns.tolist()
         cols = ['ts'] + [col for col in cols if col != 'ts']
         df = df[cols]
```

### Comparing `ML-Algo-1.2.2/ML_Algo/Series_Time.py` & `ML-Algo-1.2.5/ML_Algo/Series_Time.py`

 * *Files identical despite different names*

