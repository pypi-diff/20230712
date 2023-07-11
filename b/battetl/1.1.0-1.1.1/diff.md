# Comparing `tmp/battetl-1.1.0.tar.gz` & `tmp/battetl-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battetl-1.1.0.tar", last modified: Tue Jul 11 18:50:37 2023, max compression
+gzip compressed data, was "battetl-1.1.1.tar", last modified: Tue Jul 11 22:26:33 2023, max compression
```

## Comparing `battetl-1.1.0.tar` & `battetl-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.135462 battetl-1.1.0/
--rw-r--r--   0 Benjamin   (502) staff       (20)     1066 2023-07-10 18:08:18.000000 battetl-1.1.0/LICENSE
--rw-r--r--   0 Benjamin   (502) staff       (20)    16509 2023-07-11 18:50:37.134989 battetl-1.1.0/PKG-INFO
--rw-r--r--   0 Benjamin   (502) staff       (20)    15958 2023-07-11 18:30:14.000000 battetl-1.1.0/README.md
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.125758 battetl-1.1.0/battetl/
--rw-r--r--   0 Benjamin   (502) staff       (20)     7528 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/BattETL.py
--rw-r--r--   0 Benjamin   (502) staff       (20)      155 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/__init__.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     6971 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/battetl_quick.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     9627 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/constants.py
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.129643 battetl-1.1.0/battetl/extract/
--rw-r--r--   0 Benjamin   (502) staff       (20)    26560 2023-07-10 18:08:18.000000 battetl-1.1.0/battetl/extract/Extractor.py
--rw-r--r--   0 Benjamin   (502) staff       (20)       33 2023-07-10 18:08:18.000000 battetl-1.1.0/battetl/extract/__init__.py
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.132503 battetl-1.1.0/battetl/load/
--rw-r--r--   0 Benjamin   (502) staff       (20)    39804 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/load/Loader.py
--rw-r--r--   0 Benjamin   (502) staff       (20)      115 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/load/__init__.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     7341 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/load/batt_db_test_helper.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     3201 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/load/quick_loader.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     1677 2023-07-10 18:08:18.000000 battetl-1.1.0/battetl/logger.py
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.134052 battetl-1.1.0/battetl/transform/
--rw-r--r--   0 Benjamin   (502) staff       (20)    29328 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/transform/Transformer.py
--rw-r--r--   0 Benjamin   (502) staff       (20)       37 2023-07-10 18:08:18.000000 battetl-1.1.0/battetl/transform/__init__.py
--rw-r--r--   0 Benjamin   (502) staff       (20)    13584 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/utils.py
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.128158 battetl-1.1.0/battetl.egg-info/
--rw-r--r--   0 Benjamin   (502) staff       (20)    16509 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/PKG-INFO
--rw-r--r--   0 Benjamin   (502) staff       (20)      533 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/SOURCES.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)        1 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/dependency_links.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)      171 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/requires.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)        8 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/top_level.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)       38 2023-07-11 18:50:37.135569 battetl-1.1.0/setup.cfg
--rw-r--r--   0 Benjamin   (502) staff       (20)      886 2023-07-11 18:30:14.000000 battetl-1.1.0/setup.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.686521 battetl-1.1.1/
+-rw-r--r--   0 Benjamin   (502) staff       (20)     1066 2023-07-10 18:08:18.000000 battetl-1.1.1/LICENSE
+-rw-r--r--   0 Benjamin   (502) staff       (20)    16509 2023-07-11 22:26:33.685912 battetl-1.1.1/PKG-INFO
+-rw-r--r--   0 Benjamin   (502) staff       (20)    15958 2023-07-11 18:30:14.000000 battetl-1.1.1/README.md
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.674062 battetl-1.1.1/battetl/
+-rw-r--r--   0 Benjamin   (502) staff       (20)     7528 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/BattETL.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)      155 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/__init__.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     6971 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/battetl_quick.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     9627 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/constants.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.678755 battetl-1.1.1/battetl/extract/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    26584 2023-07-11 22:24:08.000000 battetl-1.1.1/battetl/extract/Extractor.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)       33 2023-07-10 18:08:18.000000 battetl-1.1.1/battetl/extract/__init__.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.683109 battetl-1.1.1/battetl/load/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    39804 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/load/Loader.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)      115 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/load/__init__.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     7341 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/load/batt_db_test_helper.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     3201 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/load/quick_loader.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     1677 2023-07-10 18:08:18.000000 battetl-1.1.1/battetl/logger.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.685073 battetl-1.1.1/battetl/transform/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    29382 2023-07-11 22:24:08.000000 battetl-1.1.1/battetl/transform/Transformer.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)       37 2023-07-10 18:08:18.000000 battetl-1.1.1/battetl/transform/__init__.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)    13584 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/utils.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.676650 battetl-1.1.1/battetl.egg-info/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    16509 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/PKG-INFO
+-rw-r--r--   0 Benjamin   (502) staff       (20)      533 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/SOURCES.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)        1 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/dependency_links.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)      171 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/requires.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)        8 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/top_level.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)       38 2023-07-11 22:26:33.686728 battetl-1.1.1/setup.cfg
+-rw-r--r--   0 Benjamin   (502) staff       (20)      886 2023-07-11 22:24:08.000000 battetl-1.1.1/setup.py
```

### Comparing `battetl-1.1.0/LICENSE` & `battetl-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/PKG-INFO` & `battetl-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battetl
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python module for extracting, transforming, and loading battery data to a database.
 Home-page: https://github.com/BattGenie/battetl
 Author: Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak
 Author-email: info@battgenie.life
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battetl-1.1.0/README.md` & `battetl-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/battetl/BattETL.py` & `battetl-1.1.1/battetl/BattETL.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/battetl/battetl_quick.py` & `battetl-1.1.1/battetl/battetl_quick.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/battetl/constants.py` & `battetl-1.1.1/battetl/constants.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/battetl/extract/Extractor.py` & `battetl-1.1.1/battetl/extract/Extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 class Extractor:
     def __init__(self):
         """
         An interface to extract battery test data from raw data files. 
         """
         self.raw_test_data_meta_data = []
         self.raw_cycle_stats_meta_data = []
-        self.raw_test_data = pd.DataFrame()
-        self.raw_cycle_stats = pd.DataFrame()
+        self.raw_test_data = pd.DataFrame(dtype=object)
+        self.raw_cycle_stats = pd.DataFrame(dtype=object)
         self.cycler_make = ''
 
         self.schedule = {
             'schedule': DashOrderedDict(),
             'file_name': '',
             'steps': {'chg': [], 'dsg': [], 'rst': []}
         }
```

### Comparing `battetl-1.1.0/battetl/load/Loader.py` & `battetl-1.1.1/battetl/load/Loader.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/battetl/load/batt_db_test_helper.py` & `battetl-1.1.1/battetl/load/batt_db_test_helper.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/battetl/load/quick_loader.py` & `battetl-1.1.1/battetl/load/quick_loader.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/battetl/logger.py` & `battetl-1.1.1/battetl/logger.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/battetl/transform/Transformer.py` & `battetl-1.1.1/battetl/transform/Transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         self.user_transform_test_data = user_transform_test_data
         self.user_transform_cycle_stats = user_transform_cycle_stats
         if self.user_transform_test_data:
             logger.info('User defined transform_test_data function found')
         if self.user_transform_cycle_stats:
             logger.info('User defined transform_cycle_stats function found')
 
-        self.test_data = pd.DataFrame()
-        self.cycle_stats = pd.DataFrame()
+        self.test_data = pd.DataFrame(dtype=object)
+        self.cycle_stats = pd.DataFrame(dtype=object)
 
     def transform_test_data(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Transforms test data to conform to BattETL naming and data conventions
 
         Parameters
         ----------
@@ -76,15 +76,15 @@
 
         df = self.__consolidate_temps(df)
 
         # Apply user defined transformation
         if self.user_transform_test_data:
             df = self.user_transform_test_data(df)
 
-        self.test_data = df
+        self.test_data = df.astype(object)
         return df
 
     def transform_cycle_stats(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Transforms cycle stats to conform to BattETL naming and data conventions
 
         Parameters
@@ -112,15 +112,15 @@
         if cycleMake == Constants.MAKE_MACCOR and dataType == Constants.DATA_TYPE_CYCLE_STATS:
             df = self.__transform_maccor_cycle_stats(df)
 
         # Apply user defined transformation
         if self.user_transform_cycle_stats:
             df = self.user_transform_cycle_stats(df)
 
-        self.cycle_stats = df
+        self.cycle_stats = df.astype(object)
         return df
 
     def __transform_arbin_test_data(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Transforms Arbin test data to conform to BattETL naming and data conventions
         1. Rename columns
         2. Convert to milli
```

### Comparing `battetl-1.1.0/battetl/utils.py` & `battetl-1.1.1/battetl/utils.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/battetl.egg-info/PKG-INFO` & `battetl-1.1.1/battetl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battetl
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python module for extracting, transforming, and loading battery data to a database.
 Home-page: https://github.com/BattGenie/battetl
 Author: Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak
 Author-email: info@battgenie.life
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battetl-1.1.0/battetl.egg-info/SOURCES.txt` & `battetl-1.1.1/battetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `battetl-1.1.0/setup.py` & `battetl-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="battetl",
-    version="1.1.0",
+    version="1.1.1",
     author="Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak",
     author_email="info@battgenie.life",
     description="A Python module for extracting, transforming, and loading battery data to a database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BattGenie/battetl",
     packages=setuptools.find_packages(),
```

