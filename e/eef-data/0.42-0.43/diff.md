# Comparing `tmp/eef-data-0.42.tar.gz` & `tmp/eef-data-0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eef-data-0.42.tar", last modified: Wed Jul 12 13:02:56 2023, max compression
+gzip compressed data, was "eef-data-0.43.tar", last modified: Wed Jul 12 13:06:22 2023, max compression
```

## Comparing `eef-data-0.42.tar` & `eef-data-0.43.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:02:56.507639 eef-data-0.42/
--rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.42/LICENSE
--rw-rw-r--   0 linux     (1000) linux     (1000)    62871 2023-07-12 13:02:56.507639 eef-data-0.42/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)    62568 2023-07-12 12:57:42.000000 eef-data-0.42/README.md
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:02:56.503639 eef-data-0.42/eef_data.egg-info/
--rw-rw-r--   0 linux     (1000) linux     (1000)    62871 2023-07-12 13:02:56.000000 eef-data-0.42/eef_data.egg-info/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 13:02:56.000000 eef-data-0.42/eef_data.egg-info/SOURCES.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 13:02:56.000000 eef-data-0.42/eef_data.egg-info/dependency_links.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 13:02:56.000000 eef-data-0.42/eef_data.egg-info/entry_points.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 13:02:56.000000 eef-data-0.42/eef_data.egg-info/requires.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 13:02:56.000000 eef-data-0.42/eef_data.egg-info/top_level.txt
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:02:56.507639 eef-data-0.42/eefdata/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.42/eefdata/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.42/eefdata/app.py
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:02:56.507639 eef-data-0.42/eefdata/src/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.42/eefdata/src/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.42/eefdata/src/attributeIDs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.42/eefdata/src/funcs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 13:02:56.507639 eef-data-0.42/setup.cfg
--rw-rw-r--   0 linux     (1000) linux     (1000)      690 2023-07-12 13:02:52.000000 eef-data-0.42/setup.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:06:22.498146 eef-data-0.43/
+-rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.43/LICENSE
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62889 2023-07-12 13:06:22.498146 eef-data-0.43/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62568 2023-07-12 12:57:42.000000 eef-data-0.43/README.md
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:06:22.494145 eef-data-0.43/eef_data.egg-info/
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62889 2023-07-12 13:06:22.000000 eef-data-0.43/eef_data.egg-info/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 13:06:22.000000 eef-data-0.43/eef_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 13:06:22.000000 eef-data-0.43/eef_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 13:06:22.000000 eef-data-0.43/eef_data.egg-info/entry_points.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 13:06:22.000000 eef-data-0.43/eef_data.egg-info/requires.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 13:06:22.000000 eef-data-0.43/eef_data.egg-info/top_level.txt
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:06:22.494145 eef-data-0.43/eefdata/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.43/eefdata/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.43/eefdata/app.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 13:06:22.498146 eef-data-0.43/eefdata/src/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.43/eefdata/src/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.43/eefdata/src/attributeIDs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.43/eefdata/src/funcs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 13:06:22.498146 eef-data-0.43/setup.cfg
+-rw-rw-r--   0 linux     (1000) linux     (1000)      690 2023-07-12 13:06:18.000000 eef-data-0.43/setup.py
```

### Comparing `eef-data-0.42/LICENSE` & `eef-data-0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `eef-data-0.42/PKG-INFO` & `eef-data-0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.42
+Version: 0.43
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,23 +34,23 @@
 >> eef-data
 ```
 
 When you run eef-data, you will be asked to input a data file. Once you have done so, press enter to proceed to the main menu.
 
 <p align="center">
 
-![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual1.png "visual1")
+![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual1.png?raw=true "visual1")
 
 </p>
 
 When a selection is made, the newly created file location will be displayed in the "Output Files" box at the bottom of the display.
 
 <p align="center">
 
-![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual3.png "visual1")
+![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual3.png?raw=true "visual2")
 
 </p>
 
 All output dataframes will be saved with the directory named after the original datafile. Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
 
 ## Dataframe 1: Study, Research and Design Variables
```

### Comparing `eef-data-0.42/README.md` & `eef-data-0.43/README.md`

 * *Files identical despite different names*

### Comparing `eef-data-0.42/eef_data.egg-info/PKG-INFO` & `eef-data-0.43/eef_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.42
+Version: 0.43
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,23 +34,23 @@
 >> eef-data
 ```
 
 When you run eef-data, you will be asked to input a data file. Once you have done so, press enter to proceed to the main menu.
 
 <p align="center">
 
-![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual1.png "visual1")
+![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual1.png?raw=true "visual1")
 
 </p>
 
 When a selection is made, the newly created file location will be displayed in the "Output Files" box at the bottom of the display.
 
 <p align="center">
 
-![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual3.png "visual1")
+![](https://github.com/JonathanReardon/ToolkitExtraction/blob/master/img/visual3.png?raw=true "visual2")
 
 </p>
 
 All output dataframes will be saved with the directory named after the original datafile. Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
 
 ## Dataframe 1: Study, Research and Design Variables
```

### Comparing `eef-data-0.42/eefdata/app.py` & `eef-data-0.43/eefdata/app.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.42/eefdata/src/attributeIDs.py` & `eef-data-0.43/eefdata/src/attributeIDs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.42/eefdata/src/funcs.py` & `eef-data-0.43/eefdata/src/funcs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.42/setup.py` & `eef-data-0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README_pypi.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='eef-data',
-    version='0.42',  # Remember to increment the version number
+    version='0.43',  # Remember to increment the version number
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy==1.22.0',
         'pandas==1.5.0',
         'prompt_toolkit==3.0.30',
         'rich==12.4.4',
```

