# Comparing `tmp/eef-data-0.44.tar.gz` & `tmp/eef-data-0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eef-data-0.44.tar", last modified: Wed Jul 12 13:10:19 2023, max compression
+gzip compressed data, was "eef-data-0.45.tar", last modified: Wed Jul 12 13:29:57 2023, max compression
```

## Comparing `eef-data-0.44.tar` & `eef-data-0.45.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:10:19.189026 eef-data-0.44/
--rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.44/LICENSE
--rw-rw-r--   0 linux     (1000) linux     (1000)    62847 2023-07-12 13:10:19.189026 eef-data-0.44/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)    62568 2023-07-12 12:57:42.000000 eef-data-0.44/README.md
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:10:19.185026 eef-data-0.44/eef_data.egg-info/
--rw-rw-r--   0 linux     (1000) linux     (1000)    62847 2023-07-12 13:10:19.000000 eef-data-0.44/eef_data.egg-info/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 13:10:19.000000 eef-data-0.44/eef_data.egg-info/SOURCES.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 13:10:19.000000 eef-data-0.44/eef_data.egg-info/dependency_links.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 13:10:19.000000 eef-data-0.44/eef_data.egg-info/entry_points.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 13:10:19.000000 eef-data-0.44/eef_data.egg-info/requires.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 13:10:19.000000 eef-data-0.44/eef_data.egg-info/top_level.txt
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:10:19.185026 eef-data-0.44/eefdata/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.44/eefdata/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.44/eefdata/app.py
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:10:19.185026 eef-data-0.44/eefdata/src/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.44/eefdata/src/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.44/eefdata/src/attributeIDs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.44/eefdata/src/funcs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 13:10:19.189026 eef-data-0.44/setup.cfg
--rw-rw-r--   0 linux     (1000) linux     (1000)      690 2023-07-12 13:10:13.000000 eef-data-0.44/setup.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:29:57.231020 eef-data-0.45/
+-rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.45/LICENSE
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62863 2023-07-12 13:29:57.227020 eef-data-0.45/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62474 2023-07-12 13:27:55.000000 eef-data-0.45/README.md
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:29:57.223020 eef-data-0.45/eef_data.egg-info/
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62863 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/entry_points.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/requires.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 13:29:57.000000 eef-data-0.45/eef_data.egg-info/top_level.txt
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:29:57.223020 eef-data-0.45/eefdata/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.45/eefdata/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.45/eefdata/app.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:29:57.227020 eef-data-0.45/eefdata/src/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.45/eefdata/src/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.45/eefdata/src/attributeIDs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.45/eefdata/src/funcs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 13:29:57.231020 eef-data-0.45/setup.cfg
+-rw-rw-r--   0 linux     (1000) linux     (1000)      690 2023-07-12 13:29:44.000000 eef-data-0.45/setup.py
```

### Comparing `eef-data-0.44/LICENSE` & `eef-data-0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `eef-data-0.44/PKG-INFO` & `eef-data-0.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.44
+Version: 0.45
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -35,23 +35,23 @@
 >> eef-data
 ```
 
 When you run eef-data, you will be asked to input a data file. Once you have done so, press enter to proceed to the main menu.
 
 <p align="center">
 
-![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual1.png?raw=true "visual1")
+![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/eefdata/img/visual1.png?raw=true "visual1")
 
 </p>
 
 When a selection is made, the newly created file location will be displayed in the "Output Files" box at the bottom of the display.
 
 <p align="center">
 
-![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual3.png?raw=true "visual2")
+![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/eefdata/img/visual2.png?raw=true "visual2")
 
 </p>
 
 Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
 
 ## Dataframe 1: Study, Research and Design Variables
```

### Comparing `eef-data-0.44/README.md` & `eef-data-0.45/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,28 +23,24 @@
 ``` bash
 >> eef-data
 ```
 
 When you run eef-data, you will be asked to input a data file. Once you have done so, press enter to proceed to the main menu.
 
 <p align="center">
-
 <img src="/eefdata/img/visual1.png"/>
-
 </p>
 
 When a selection is made, the newly created file location will be displayed in the "Output Files" box at the bottom of the display.
 
 <p align="center">
-
-<img src="/eefdata/img/visual3.png"/>
-
+<img src="/eefdata/img/visual2.png"/>
 </p>
 
-All output dataframes will be saved with the directory named after the original datafile. Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
+Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
 
 ## Dataframe 1: Study, Research and Design Variables
 
 This dataframe contains 'raw', 'ht', 'info', and 'CLEAN' data types.
 
 | Data Type | Description | Number of Columns |
 | --- | --- | :----: |
```

### Comparing `eef-data-0.44/eef_data.egg-info/PKG-INFO` & `eef-data-0.45/eef_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.44
+Version: 0.45
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -35,23 +35,23 @@
 >> eef-data
 ```
 
 When you run eef-data, you will be asked to input a data file. Once you have done so, press enter to proceed to the main menu.
 
 <p align="center">
 
-![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual1.png?raw=true "visual1")
+![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/eefdata/img/visual1.png?raw=true "visual1")
 
 </p>
 
 When a selection is made, the newly created file location will be displayed in the "Output Files" box at the bottom of the display.
 
 <p align="center">
 
-![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual3.png?raw=true "visual2")
+![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/eefdata/img/visual2.png?raw=true "visual2")
 
 </p>
 
 Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
 
 ## Dataframe 1: Study, Research and Design Variables
```

### Comparing `eef-data-0.44/eefdata/app.py` & `eef-data-0.45/eefdata/app.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.44/eefdata/src/attributeIDs.py` & `eef-data-0.45/eefdata/src/attributeIDs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.44/eefdata/src/funcs.py` & `eef-data-0.45/eefdata/src/funcs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.44/setup.py` & `eef-data-0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README_pypi.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='eef-data',
-    version='0.44',  # Remember to increment the version number
+    version='0.45',  # Remember to increment the version number
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy==1.22.0',
         'pandas==1.5.0',
         'prompt_toolkit==3.0.30',
         'rich==12.4.4',
```

