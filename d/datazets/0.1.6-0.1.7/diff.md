# Comparing `tmp/datazets-0.1.6.tar.gz` & `tmp/datazets-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazets-0.1.6.tar", last modified: Fri May 26 18:19:42 2023, max compression
+gzip compressed data, was "datazets-0.1.7.tar", last modified: Wed Jul 12 08:54:01 2023, max compression
```

## Comparing `datazets-0.1.6.tar` & `datazets-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 18:19:42.059783 datazets-0.1.6/
--rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4613 2023-05-26 18:19:42.059783 datazets-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 18:19:42.043962 datazets-0.1.6/datazets/
--rw-rw-rw-   0        0        0      765 2023-05-26 18:14:25.000000 datazets-0.1.6/datazets/__init__.py
--rw-rw-rw-   0        0        0    19064 2023-05-26 18:19:14.000000 datazets-0.1.6/datazets/datazets.py
--rw-rw-rw-   0        0        0     1069 2023-05-26 18:19:02.000000 datazets-0.1.6/datazets/examples.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:19:42.058398 datazets-0.1.6/datazets/utils/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.6/datazets/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:19:42.056793 datazets-0.1.6/datazets.egg-info/
--rw-rw-rw-   0        0        0     4613 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 18:19:42.060797 datazets-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1382 2023-05-26 18:14:10.000000 datazets-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:54:01.469649 datazets-0.1.7/
+-rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4613 2023-07-12 08:54:01.468557 datazets-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 08:54:01.456222 datazets-0.1.7/datazets/
+-rw-rw-rw-   0        0        0      739 2023-07-12 08:53:35.000000 datazets-0.1.7/datazets/__init__.py
+-rw-rw-rw-   0        0        0    19174 2023-07-12 08:50:16.000000 datazets-0.1.7/datazets/datazets.py
+-rw-rw-rw-   0        0        0     1216 2023-07-12 08:52:18.000000 datazets-0.1.7/datazets/examples.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:54:01.467561 datazets-0.1.7/datazets/utils/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.7/datazets/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:54:01.466562 datazets-0.1.7/datazets.egg-info/
+-rw-rw-rw-   0        0        0     4613 2023-07-12 08:54:01.000000 datazets-0.1.7/datazets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-12 08:54:01.000000 datazets-0.1.7/datazets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 08:54:01.000000 datazets-0.1.7/datazets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-12 08:54:01.000000 datazets-0.1.7/datazets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 08:54:01.000000 datazets-0.1.7/datazets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 08:54:01.469649 datazets-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1382 2023-05-26 18:14:10.000000 datazets-0.1.7/setup.py
```

### Comparing `datazets-0.1.6/LICENSE` & `datazets-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datazets-0.1.6/PKG-INFO` & `datazets-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.6
+Version: 0.1.7
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.6.tar.gz
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.7.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `datazets-0.1.6/README.md` & `datazets-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `datazets-0.1.6/datazets/__init__.py` & `datazets-0.1.7/datazets/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from datazets.datazets import get, get_dataproperties, download_from_url, unzip, listdir, url2disk
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 
 # module level doc-string
 __doc__ = """
 datazets
 =====================================================================
 
-Description
------------
 Datazets is a python package to import well known example data sets.
 
 Example
 -------
 >>> # Import library
 >>> import datazets as dz
 >>> #
```

### Comparing `datazets-0.1.6/datazets/datazets.py` & `datazets-0.1.7/datazets/datazets.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 import logging
 import zipfile
 import fnmatch
 from io import BytesIO
 from urllib.parse import urlparse
 
 logger = logging.getLogger('')
-for handler in logger.handlers[:]:
-    logger.removeHandler(handler)
+[logger.removeHandler(handler) for handler in logger.handlers[:]]
 console = logging.StreamHandler()
 formatter = logging.Formatter('[datazets] >%(levelname)s> %(message)s')
 console.setFormatter(formatter)
 logger.addHandler(console)
 logger = logging.getLogger(__name__)
 
 
@@ -59,22 +58,22 @@
             * 'census_income'
             * 'ads'
         Continous data sets:
             * 'breast_cancer'
             * 'cancer'
             * 'auto_mpg'
             * 'iris'
-        Images
+        Images:
             * 'faces'
             * 'mnist'
-        files:
-            * 'southern_nebula' (images)
-            * 'flowers' (images)
-            * 'scenes' (images)
-            * 'cat_and_dog' (images)
+        Images (files):
+            * 'southern_nebula'
+            * 'flowers'
+            * 'scenes'
+            * 'cat_and_dog'
         Text data sets:
             * 'marketing_retail'
             * 'malicious_urls'
             * 'grocery_products'
         Time series:
             * 'bitcoin'
             * 'meta'
@@ -139,15 +138,15 @@
         df = _generate_data(dataproperties['filename'], **args)
     elif dataproperties['type']=='DAG':
         df = _extract_files(dataproperties, targetdir=os.path.join(dataproperties['curpath'], dataproperties['input']), ext='*')
         # PATH_TO_DATA = download_from_url(dataproperties['filename'], url=dataproperties['url'], dataproperties=dataproperties)
     else:
         PATH_TO_DATA = download_from_url(dataproperties['filename'], url=dataproperties['url'])
         df = pd.read_csv(PATH_TO_DATA, sep=dataproperties['sep'])
-    
+
     df = _set_dtypes(df, dataproperties)
     # Return
     return df
 
 
 # %%
 def _set_dtypes(df, dataproperties):
@@ -209,31 +208,32 @@
 
 # %% Get the correct url name.
 def get_dataproperties(data, sep=None, url=None):
     inputname, datatype = data, None
     if data is not None:
         data = data.lower()
         # Set datatype for imges
-        if data=='flowers' or data=='scenes' or data=='southern_nebula':
+        if data=='flowers' or data=='scenes' or data=='southern_nebula' or data=='cat_and_dog':
             datatype='files'
             if data=='flowers': data = 'flower_images.zip'
             if data=='scenes': data = 'scenes.zip'
-            # if data=='cat_and_dog': data = 'cat_and_dog.zip'
-            # if data=='southern_nebula': data = 'southern_nebula.zip'
+            if data=='cat_and_dog': data = 'cat_and_dog.zip'
+            if data=='southern_nebula': data = 'southern_nebula.zip'
         elif data=='alarm' or data=='andes' or data=='asia' or data=='sachs' or data=='water':
             datatype='DAG'
             if os.path.splitext(data)[1]=='':
                 sep=','
                 data = data + '.zip'
         elif data=='random_discrete':
             datatype='synthetic'
         else:
             datatype='various'
             # Rename to correct filename
             if data=='titanic': data, sep ='titanic_train.zip', ','
+            if data=='ds_salaries': data, sep ='ds_salaries.zip', ','
             if data=='student': data, sep ='student_train.zip', ','
             if data=='cancer': data, sep = 'cancer_dataset.zip', ','
             if data=='fifa': data, sep = 'FIFA_2018.zip', ','
             if data=='ads': data, sep = 'ads_data.zip', ','
             if data=='bitcoin': data, sep = 'BTCUSDT.zip', ','
             if data=='meta': data, sep = 'facebook_stocks.zip', ','
             if data=='energy': data, sep = 'energy_source_target_value.zip', ','
@@ -374,14 +374,15 @@
             zip_ref = zipfile.ZipFile(path_to_zip, 'r')
             zip_ref.extractall(pathname)
             zip_ref.close()
             getpath = path_to_zip.replace('.zip', '')
             if not os.path.isdir(getpath):
                 logger.error('Extraction failed.')
                 getpath = None
+                raise Exception('Extraction failed')
     else:
         logger.warning('Input is not a zip file: [%s]', path_to_zip)
     # Return
     return getpath
 
 
 # %%
```

### Comparing `datazets-0.1.6/datazets/examples.py` & `datazets-0.1.7/datazets/examples.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # %%
 import datazets as dz
-df = dz.get(data='ds_salaries', overwrite=True)
+IMG = dz.get(data='faces', overwrite=True)
 
 
 # %%
 import datazets as dz
 url='https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data'
 df = dz.get(url=url, sep=',')
 df.shape
 
 # %%
 import datazets as dz
 df = dz.get(data='auto_mpg')
 # df.shape
 
 # %% New
+import datazets as dz
+IMAGES = ['faces', 'mnist', 'southern_nebula', 'flowers', 'scenes', 'cat_and_dog']
 
 # %% test
 datasets = ['census_income',
             'stormofswords',
             'sprinkler',
             'titanic',
             'student',
@@ -40,10 +42,15 @@
             'malicious_urls',
             'waterpump',
             'elections',
             'tips',
             'predictive_maintenance',
             ]
 
+datasets = datasets + IMAGES
+
+# %%
 for data in datasets:
     df = dz.get(data=data)
-    print(df.shape)
+    print(len(df))
+
+# %%
```

### Comparing `datazets-0.1.6/datazets.egg-info/PKG-INFO` & `datazets-0.1.7/datazets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.6
+Version: 0.1.7
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.6.tar.gz
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.7.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `datazets-0.1.6/setup.py` & `datazets-0.1.7/setup.py`

 * *Files identical despite different names*

