# Comparing `tmp/eef-data-0.45.tar.gz` & `tmp/eef-data-0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eef-data-0.45.tar", last modified: Wed Jul 12 13:29:57 2023, max compression
+gzip compressed data, was "eef-data-0.46.tar", last modified: Wed Jul 12 13:33:47 2023, max compression
```

## Comparing `eef-data-0.45.tar` & `eef-data-0.46.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:29:57.231020 eef-data-0.45/
--rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.45/LICENSE
--rw-rw-r--   0 linux     (1000) linux     (1000)    62863 2023-07-12 13:29:57.227020 eef-data-0.45/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)    62474 2023-07-12 13:27:55.000000 eef-data-0.45/README.md
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:29:57.223020 eef-data-0.45/eef_data.egg-info/
--rw-rw-r--   0 linux     (1000) linux     (1000)    62863 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/SOURCES.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/dependency_links.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/entry_points.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/requires.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/top_level.txt
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:29:57.223020 eef-data-0.45/eefdata/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.45/eefdata/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.45/eefdata/app.py
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:29:57.227020 eef-data-0.45/eefdata/src/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.45/eefdata/src/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.45/eefdata/src/attributeIDs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.45/eefdata/src/funcs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 13:29:57.231020 eef-data-0.45/setup.cfg
--rw-rw-r--   0 linux     (1000) linux     (1000)      690 2023-07-12 13:29:44.000000 eef-data-0.45/setup.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:33:47.313778 eef-data-0.46/
+-rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.46/LICENSE
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62814 2023-07-12 13:33:47.309777 eef-data-0.46/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62474 2023-07-12 13:27:55.000000 eef-data-0.46/README.md
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:33:47.309777 eef-data-0.46/eef_data.egg-info/
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62814 2023-07-12 13:33:47.000000 eef-data-0.46/eef_data.egg-info/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 13:33:47.000000 eef-data-0.46/eef_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 13:33:47.000000 eef-data-0.46/eef_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 13:33:47.000000 eef-data-0.46/eef_data.egg-info/entry_points.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 13:33:47.000000 eef-data-0.46/eef_data.egg-info/requires.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 13:33:47.000000 eef-data-0.46/eef_data.egg-info/top_level.txt
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:33:47.309777 eef-data-0.46/eefdata/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.46/eefdata/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.46/eefdata/app.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:33:47.309777 eef-data-0.46/eefdata/src/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.46/eefdata/src/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.46/eefdata/src/attributeIDs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.46/eefdata/src/funcs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 13:33:47.313778 eef-data-0.46/setup.cfg
+-rw-rw-r--   0 linux     (1000) linux     (1000)      690 2023-07-12 13:33:42.000000 eef-data-0.46/setup.py
```

### Comparing `eef-data-0.45/LICENSE` & `eef-data-0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `eef-data-0.45/PKG-INFO` & `eef-data-0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.45
+Version: 0.46
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [<img alt="" src="https://img.shields.io/pypi/v/eef-data?label=PyPI%20Package" />](https://pypi.org/project/eef-data/)
 
-![PyPI](https://img.shields.io/pypi/v/eef-data)
-
 <h1 align="center">
 
 EEF Datafile Extractor
 
 </h1>
 
 The EEF Datafile Extractor is an application designed to streamline the processing of data files from the [EEF](https://educationendowmentfoundation.org.uk/education-evidence/teaching-learning-toolkit?gclid=CjwKCAjwjMiiBhA4EiwAZe6jQ3WnUgowD16xFwcG_6hZySd_qiKcElx5wRI0BjJAdwj5RkFT_kzz1hoCS_MQAvD_BwE) Education Evidence Database. The database provides JSON files with complex, nested structures, and our toolkit simplifies the process of extracting the necessary data, making it easier to integrate into your broader data processing pipeline. We provide a collection of bespoke dataframes specifically tailored for data cleaning and analysis. In addition to the pre-built dataframes, the tool includes a custom dataframe builder. This feature empowers you to compile your own dataframes based on your specific research requirements.
```

### Comparing `eef-data-0.45/README.md` & `eef-data-0.46/README.md`

 * *Files identical despite different names*

### Comparing `eef-data-0.45/eef_data.egg-info/PKG-INFO` & `eef-data-0.46/eef_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.45
+Version: 0.46
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [<img alt="" src="https://img.shields.io/pypi/v/eef-data?label=PyPI%20Package" />](https://pypi.org/project/eef-data/)
 
-![PyPI](https://img.shields.io/pypi/v/eef-data)
-
 <h1 align="center">
 
 EEF Datafile Extractor
 
 </h1>
 
 The EEF Datafile Extractor is an application designed to streamline the processing of data files from the [EEF](https://educationendowmentfoundation.org.uk/education-evidence/teaching-learning-toolkit?gclid=CjwKCAjwjMiiBhA4EiwAZe6jQ3WnUgowD16xFwcG_6hZySd_qiKcElx5wRI0BjJAdwj5RkFT_kzz1hoCS_MQAvD_BwE) Education Evidence Database. The database provides JSON files with complex, nested structures, and our toolkit simplifies the process of extracting the necessary data, making it easier to integrate into your broader data processing pipeline. We provide a collection of bespoke dataframes specifically tailored for data cleaning and analysis. In addition to the pre-built dataframes, the tool includes a custom dataframe builder. This feature empowers you to compile your own dataframes based on your specific research requirements.
```

### Comparing `eef-data-0.45/eefdata/app.py` & `eef-data-0.46/eefdata/app.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.45/eefdata/src/attributeIDs.py` & `eef-data-0.46/eefdata/src/attributeIDs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.45/eefdata/src/funcs.py` & `eef-data-0.46/eefdata/src/funcs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.45/setup.py` & `eef-data-0.46/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README_pypi.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='eef-data',
-    version='0.45',  # Remember to increment the version number
+    version='0.46',  # Remember to increment the version number
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy==1.22.0',
         'pandas==1.5.0',
         'prompt_toolkit==3.0.30',
         'rich==12.4.4',
```

