# Comparing `tmp/whyshift-0.0.1.tar.gz` & `tmp/whyshift-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyshift-0.0.1.tar", last modified: Tue Jul 11 11:44:01 2023, max compression
+gzip compressed data, was "dist/whyshift-0.0.2.tar", last modified: Wed Jul 12 14:57:49 2023, max compression
```

## Comparing `whyshift-0.0.1.tar` & `whyshift-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:44:01.517617 whyshift-0.0.1/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:02:02.000000 whyshift-0.0.1/LICENSE
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-11 11:44:01.517617 whyshift-0.0.1/PKG-INFO
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       52 2023-07-11 11:01:00.000000 whyshift-0.0.1/README.md
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       38 2023-07-11 11:44:01.517617 whyshift-0.0.1/setup.cfg
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      879 2023-07-11 11:13:14.000000 whyshift-0.0.1/setup.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:44:01.513617 whyshift-0.0.1/whyshift/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      123 2023-07-11 11:42:26.000000 whyshift-0.0.1/whyshift/__init__.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    14392 2023-07-11 11:09:30.000000 whyshift-0.0.1/whyshift/dataset.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:44:01.517617 whyshift-0.0.1/whyshift/folktables/
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      165 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/__init__.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8357 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/acs.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      747 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/dataset.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      987 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/exceptions.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4568 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/folktables.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8782 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/load_acs.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:44:01.517617 whyshift-0.0.1/whyshift/folktables/utils/
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/utils/__init__.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4043 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/utils/download_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      998 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/utils/files_resources.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1443 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables/utils/load_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     7466 2023-07-11 11:01:26.000000 whyshift-0.0.1/whyshift/folktables_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4547 2023-07-11 11:10:30.000000 whyshift-0.0.1/whyshift/utils.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:44:01.513617 whyshift-0.0.1/whyshift.egg-info/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-11 11:44:01.000000 whyshift-0.0.1/whyshift.egg-info/PKG-INFO
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-11 11:44:01.000000 whyshift-0.0.1/whyshift.egg-info/SOURCES.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        1 2023-07-11 11:44:01.000000 whyshift-0.0.1/whyshift.egg-info/dependency_links.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       26 2023-07-11 11:44:01.000000 whyshift-0.0.1/whyshift.egg-info/requires.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        9 2023-07-11 11:44:01.000000 whyshift-0.0.1/whyshift.egg-info/top_level.txt
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift/
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift/folktables/
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8357 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/acs.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4568 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/folktables.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      987 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/exceptions.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      747 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/dataset.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8782 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/load_acs.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift/folktables/utils/
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      998 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/utils/files_resources.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1443 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/utils/load_utils.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4043 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/utils/download_utils.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/utils/__init__.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      165 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/__init__.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     7466 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables_utils.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    13969 2023-07-12 14:48:26.000000 whyshift-0.0.2/whyshift/dataset.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4547 2023-07-11 11:10:30.000000 whyshift-0.0.2/whyshift/utils.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      123 2023-07-12 14:56:36.000000 whyshift-0.0.2/whyshift/__init__.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     9551 2023-07-12 14:52:42.000000 whyshift-0.0.2/README.md
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      879 2023-07-12 14:57:24.000000 whyshift-0.0.2/setup.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      664 2023-07-12 14:57:49.000000 whyshift-0.0.2/PKG-INFO
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       26 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/requires.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      622 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      664 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/PKG-INFO
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        1 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        9 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/top_level.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       38 2023-07-12 14:57:49.000000 whyshift-0.0.2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `whyshift-0.0.1/PKG-INFO` & `whyshift-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: whyshift
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data
 Home-page: https://github.com/namkoong-lab/whyshift
 Author: Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong
 Author-email: liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu
+License: UNKNOWN
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3
-License-File: LICENSE
```

### Comparing `whyshift-0.0.1/setup.py` & `whyshift-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='whyshift',
-    version='0.0.1',    
+    version='0.0.2',    
     description='A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data',
     url='https://github.com/namkoong-lab/whyshift',
     author='Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong',
     author_email='liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu',
     packages=find_packages(),
     install_requires=['pandas',
                       'numpy',
```

### Comparing `whyshift-0.0.1/whyshift/dataset.py` & `whyshift-0.0.2/whyshift/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     df = data 
     df = df[df["AGEP"] > 18]
     df = df[df["AGEP"] < 35]
     return df
 
 def get_USAccident(state, need_preprocess, root_dir='./datasets/USAccident/US_Accidents_Dec21_updated.csv'):
     if not state in ['CA', 'TX', 'FL', 'OR', 'MN', 'VA', 'SC', 'NY', 'PA', 'NC', 'TN', 'MI', 'MO']:
-        raise NotImplementedError(f"{state} is not supported in this dataset")
+        raise NotImplementedError(f"{state} is not supported in this dataset!")
 
     raw_X = preprocess(root_dir)
     data = raw_X[raw_X["State"]==state]
 
     y_sample = data["Severity"]
     X_sample = data.drop(["Severity", "State", "Start_Lat", "Start_Lng"], axis=1).values
 
@@ -113,29 +113,17 @@
         
     df = df[(df.trip_duration < 5900)]
     df = df[(df.pickup_longitude > -110)]
     df = df[(df.pickup_latitude < 50)]
     df.drop(['store_and_fwd_flag'], axis=1, inplace=True)
     df.drop(['vendor_id'], axis=1, inplace=True)
     df['pickup_datetime'] = pd.to_datetime(df.pickup_datetime)
-    df['dropoff_datetime'] = pd.to_datetime(df.dropoff_datetime)
-    df['dp_month'] = df.dropoff_datetime.dt.month
-    df['dp_week'] = df.dropoff_datetime.dt.week
-    df['dp_weekday'] = df.dropoff_datetime.dt.weekday
-    df['dp_hour'] = df.dropoff_datetime.dt.hour
-    df['dp_minute'] = df.dropoff_datetime.dt.minute
-    df['dp_minute_oftheday'] = df['dp_hour'] * 60 + df['dp_minute']
-    df.drop(['dp_minute'], axis=1, inplace=True)
-
-
-
     df.drop(['dropoff_datetime'], axis=1, inplace=True) 
-
     df['month'] = df.pickup_datetime.dt.month
-    df['week'] = df.pickup_datetime.dt.week
+    df['week'] = df.pickup_datetime.dt.isocalendar().week
     df['weekday'] = df.pickup_datetime.dt.weekday
     df['hour'] = df.pickup_datetime.dt.hour
     df['minute'] = df.pickup_datetime.dt.minute
     df['minute_oftheday'] = df['hour'] * 60 + df['minute']
     df.drop(['minute'], axis=1, inplace=True)
```

### Comparing `whyshift-0.0.1/whyshift/folktables/acs.py` & `whyshift-0.0.2/whyshift/folktables/acs.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift/folktables/dataset.py` & `whyshift-0.0.2/whyshift/folktables/dataset.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift/folktables/exceptions.py` & `whyshift-0.0.2/whyshift/folktables/exceptions.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift/folktables/folktables.py` & `whyshift-0.0.2/whyshift/folktables/folktables.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift/folktables/load_acs.py` & `whyshift-0.0.2/whyshift/folktables/load_acs.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift/folktables/utils/download_utils.py` & `whyshift-0.0.2/whyshift/folktables/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift/folktables/utils/files_resources.py` & `whyshift-0.0.2/whyshift/folktables/utils/files_resources.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift/folktables/utils/load_utils.py` & `whyshift-0.0.2/whyshift/folktables/utils/load_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift/folktables_utils.py` & `whyshift-0.0.2/whyshift/folktables_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift/utils.py` & `whyshift-0.0.2/whyshift/utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.1/whyshift.egg-info/PKG-INFO` & `whyshift-0.0.2/whyshift.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: whyshift
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data
 Home-page: https://github.com/namkoong-lab/whyshift
 Author: Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong
 Author-email: liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu
+License: UNKNOWN
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3
-License-File: LICENSE
```

### Comparing `whyshift-0.0.1/whyshift.egg-info/SOURCES.txt` & `whyshift-0.0.2/whyshift.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 whyshift/__init__.py
 whyshift/dataset.py
 whyshift/folktables_utils.py
 whyshift/utils.py
 whyshift.egg-info/PKG-INFO
```

