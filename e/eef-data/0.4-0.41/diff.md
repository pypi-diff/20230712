# Comparing `tmp/eef-data-0.4.tar.gz` & `tmp/eef-data-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eef-data-0.4.tar", last modified: Wed Jul 12 12:06:47 2023, max compression
+gzip compressed data, was "eef-data-0.41.tar", last modified: Wed Jul 12 12:53:15 2023, max compression
```

## Comparing `eef-data-0.4.tar` & `eef-data-0.41.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:06:47.896579 eef-data-0.4/
--rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.4/LICENSE
--rw-rw-r--   0 linux     (1000) linux     (1000)    63160 2023-07-12 12:06:47.896579 eef-data-0.4/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)    62974 2023-07-10 13:29:48.000000 eef-data-0.4/README.md
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:06:47.892579 eef-data-0.4/eef_data.egg-info/
--rw-rw-r--   0 linux     (1000) linux     (1000)    63160 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/SOURCES.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/dependency_links.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/entry_points.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/requires.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 12:06:47.000000 eef-data-0.4/eef_data.egg-info/top_level.txt
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:06:47.892579 eef-data-0.4/eefdata/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.4/eefdata/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.4/eefdata/app.py
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:06:47.892579 eef-data-0.4/eefdata/src/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.4/eefdata/src/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.4/eefdata/src/attributeIDs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.4/eefdata/src/funcs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 12:06:47.896579 eef-data-0.4/setup.cfg
--rw-rw-r--   0 linux     (1000) linux     (1000)      684 2023-07-12 12:06:36.000000 eef-data-0.4/setup.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:53:15.946040 eef-data-0.41/
+-rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.41/LICENSE
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62755 2023-07-12 12:53:15.942040 eef-data-0.41/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62568 2023-07-12 12:51:45.000000 eef-data-0.41/README.md
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:53:15.938040 eef-data-0.41/eef_data.egg-info/
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62755 2023-07-12 12:53:15.000000 eef-data-0.41/eef_data.egg-info/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-12 12:53:15.000000 eef-data-0.41/eef_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-12 12:53:15.000000 eef-data-0.41/eef_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-12 12:53:15.000000 eef-data-0.41/eef_data.egg-info/entry_points.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-12 12:53:15.000000 eef-data-0.41/eef_data.egg-info/requires.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-12 12:53:15.000000 eef-data-0.41/eef_data.egg-info/top_level.txt
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:53:15.938040 eef-data-0.41/eefdata/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.41/eefdata/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   133960 2023-07-12 11:54:38.000000 eef-data-0.41/eefdata/app.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-12 12:53:15.942040 eef-data-0.41/eefdata/src/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.41/eefdata/src/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-03-28 21:02:40.000000 eef-data-0.41/eefdata/src/attributeIDs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   263013 2023-07-12 11:58:50.000000 eef-data-0.41/eefdata/src/funcs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-12 12:53:15.946040 eef-data-0.41/setup.cfg
+-rw-rw-r--   0 linux     (1000) linux     (1000)      685 2023-07-12 12:53:00.000000 eef-data-0.41/setup.py
```

### Comparing `eef-data-0.4/LICENSE` & `eef-data-0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `eef-data-0.4/PKG-INFO` & `eef-data-0.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,82 +1,60 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.4
+Version: 0.41
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align="center">
-
-EEF Datafile Extractor
-
-</h1>
-
-This command line application is designed to process data files from the [EEF](https://educationendowmentfoundation.org.uk/education-evidence/teaching-learning-toolkit?gclid=CjwKCAjwjMiiBhA4EiwAZe6jQ3WnUgowD16xFwcG_6hZySd_qiKcElx5wRI0BjJAdwj5RkFT_kzz1hoCS_MQAvD_BwE) Education Evidence Database. It allows you to extract specific dataframes required for data cleaning and analysis purposes. The database provides JSON files with nested structures, and this application simplifies the process of extracting the necessary data, making it easier to integrate into your broader data processing pipeline.
 
-## Dependencies
+[<img alt="" src="https://img.shields.io/pypi/v/eef-data?label=PyPI%20Package" />](https://pypi.org/project/eef-data/)
 
--   [Python](https://www.python.org/) 3.7 or higher
--   [numpy](https://github.com/numpy/numpy) 1.22.0
--   [pandas](https://github.com/pandas-dev/pandas) 1.5.0
--   [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) 3.0.30
--   [rich](https://github.com/Textualize/rich/tree/6d30ad0f30028210124c149811cbbe2b183711f9) 12.4.4
--   [toolz](https://github.com/pytoolz/toolz) 0.11.2
 
-Please make sure you have the above dependencies installed before running the application.
+<h1 align="center">
 
-## How to Run
+EEF Datafile Extractor
 
-To run the application, follow these steps.
+</h1>
 
-1.  Clone this repository:
+The EEF Datafile Extractor is an application designed to streamline the processing of data files from the [EEF](https://educationendowmentfoundation.org.uk/education-evidence/teaching-learning-toolkit?gclid=CjwKCAjwjMiiBhA4EiwAZe6jQ3WnUgowD16xFwcG_6hZySd_qiKcElx5wRI0BjJAdwj5RkFT_kzz1hoCS_MQAvD_BwE) Education Evidence Database. The database provides JSON files with complex, nested structures, and our toolkit simplifies the process of extracting the necessary data, making it easier to integrate into your broader data processing pipeline. We provide a collection of bespoke dataframes specifically tailored for data cleaning and analysis. In addition to the pre-built dataframes, the tool includes a custom dataframe builder. This feature empowers you to compile your own dataframes based on your specific research requirements.
 
-``` bash
->> git clone https://github.com/JonathanReardon/ToolkitExtraction
->> cd ToolkitExtraction
-```
+## Installing
 
-2.  Install the required dependencies by executing the following command:
+Install with `pip` or your favorite PyPI package manager.
 
 ``` bash
->> pip install -r requirements.txt
+>> pip install eef-data
 ```
 
-3.  Run the application:
+and simply run from the command line..
 
 ``` bash
->> python3 main.py
+>> eef-data
 ```
 
-To begin, you will need to input a data file. Once you have done so, press enter to proceed to the main menu.
+When you run eef-data, you will be asked to input a data file. Once you have done so, press enter to proceed to the main menu.
 
 <p align="center">
 
-<img src="/img/visual1.png"/>
+<img src="/eefdata/img/visual1.png"/>
 
 </p>
 
 When a selection is made, the newly created file location will be displayed in the "Output Files" box at the bottom of the display.
 
 <p align="center">
 
-<img src="/img/visual3.png"/>
+<img src="/eefdata/img/visual3.png"/>
 
 </p>
 
-All output dataframes will be saved within the 'output' directory, with the directory named after the original datafile. Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
-
-<p align="center">
-
-<img src="/img/visual2.png"/>
-
-</p>
+All output dataframes will be saved with the directory named after the original datafile. Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
 
 ## Dataframe 1: Study, Research and Design Variables
 
 This dataframe contains 'raw', 'ht', 'info', and 'CLEAN' data types.
 
 | Data Type | Description | Number of Columns |
 | --- | --- | :----: |
```

### Comparing `eef-data-0.4/README.md` & `eef-data-0.41/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,72 +1,50 @@
-<h1 align="center">
-
-EEF Datafile Extractor
-
-</h1>
-
-This command line application is designed to process data files from the [EEF](https://educationendowmentfoundation.org.uk/education-evidence/teaching-learning-toolkit?gclid=CjwKCAjwjMiiBhA4EiwAZe6jQ3WnUgowD16xFwcG_6hZySd_qiKcElx5wRI0BjJAdwj5RkFT_kzz1hoCS_MQAvD_BwE) Education Evidence Database. It allows you to extract specific dataframes required for data cleaning and analysis purposes. The database provides JSON files with nested structures, and this application simplifies the process of extracting the necessary data, making it easier to integrate into your broader data processing pipeline.
 
-## Dependencies
+[<img alt="" src="https://img.shields.io/pypi/v/eef-data?label=PyPI%20Package" />](https://pypi.org/project/eef-data/)
 
--   [Python](https://www.python.org/) 3.7 or higher
--   [numpy](https://github.com/numpy/numpy) 1.22.0
--   [pandas](https://github.com/pandas-dev/pandas) 1.5.0
--   [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) 3.0.30
--   [rich](https://github.com/Textualize/rich/tree/6d30ad0f30028210124c149811cbbe2b183711f9) 12.4.4
--   [toolz](https://github.com/pytoolz/toolz) 0.11.2
 
-Please make sure you have the above dependencies installed before running the application.
+<h1 align="center">
 
-## How to Run
+EEF Datafile Extractor
 
-To run the application, follow these steps.
+</h1>
 
-1.  Clone this repository:
+The EEF Datafile Extractor is an application designed to streamline the processing of data files from the [EEF](https://educationendowmentfoundation.org.uk/education-evidence/teaching-learning-toolkit?gclid=CjwKCAjwjMiiBhA4EiwAZe6jQ3WnUgowD16xFwcG_6hZySd_qiKcElx5wRI0BjJAdwj5RkFT_kzz1hoCS_MQAvD_BwE) Education Evidence Database. The database provides JSON files with complex, nested structures, and our toolkit simplifies the process of extracting the necessary data, making it easier to integrate into your broader data processing pipeline. We provide a collection of bespoke dataframes specifically tailored for data cleaning and analysis. In addition to the pre-built dataframes, the tool includes a custom dataframe builder. This feature empowers you to compile your own dataframes based on your specific research requirements.
 
-``` bash
->> git clone https://github.com/JonathanReardon/ToolkitExtraction
->> cd ToolkitExtraction
-```
+## Installing
 
-2.  Install the required dependencies by executing the following command:
+Install with `pip` or your favorite PyPI package manager.
 
 ``` bash
->> pip install -r requirements.txt
+>> pip install eef-data
 ```
 
-3.  Run the application:
+and simply run from the command line..
 
 ``` bash
->> python3 main.py
+>> eef-data
 ```
 
-To begin, you will need to input a data file. Once you have done so, press enter to proceed to the main menu.
+When you run eef-data, you will be asked to input a data file. Once you have done so, press enter to proceed to the main menu.
 
 <p align="center">
 
-<img src="/img/visual1.png"/>
+<img src="/eefdata/img/visual1.png"/>
 
 </p>
 
 When a selection is made, the newly created file location will be displayed in the "Output Files" box at the bottom of the display.
 
 <p align="center">
 
-<img src="/img/visual3.png"/>
+<img src="/eefdata/img/visual3.png"/>
 
 </p>
 
-All output dataframes will be saved within the 'output' directory, with the directory named after the original datafile. Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
-
-<p align="center">
-
-<img src="/img/visual2.png"/>
-
-</p>
+All output dataframes will be saved with the directory named after the original datafile. Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
 
 ## Dataframe 1: Study, Research and Design Variables
 
 This dataframe contains 'raw', 'ht', 'info', and 'CLEAN' data types.
 
 | Data Type | Description | Number of Columns |
 | --- | --- | :----: |
```

### Comparing `eef-data-0.4/eef_data.egg-info/PKG-INFO` & `eef-data-0.41/eef_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,82 +1,60 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.4
+Version: 0.41
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align="center">
-
-EEF Datafile Extractor
-
-</h1>
-
-This command line application is designed to process data files from the [EEF](https://educationendowmentfoundation.org.uk/education-evidence/teaching-learning-toolkit?gclid=CjwKCAjwjMiiBhA4EiwAZe6jQ3WnUgowD16xFwcG_6hZySd_qiKcElx5wRI0BjJAdwj5RkFT_kzz1hoCS_MQAvD_BwE) Education Evidence Database. It allows you to extract specific dataframes required for data cleaning and analysis purposes. The database provides JSON files with nested structures, and this application simplifies the process of extracting the necessary data, making it easier to integrate into your broader data processing pipeline.
 
-## Dependencies
+[<img alt="" src="https://img.shields.io/pypi/v/eef-data?label=PyPI%20Package" />](https://pypi.org/project/eef-data/)
 
--   [Python](https://www.python.org/) 3.7 or higher
--   [numpy](https://github.com/numpy/numpy) 1.22.0
--   [pandas](https://github.com/pandas-dev/pandas) 1.5.0
--   [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) 3.0.30
--   [rich](https://github.com/Textualize/rich/tree/6d30ad0f30028210124c149811cbbe2b183711f9) 12.4.4
--   [toolz](https://github.com/pytoolz/toolz) 0.11.2
 
-Please make sure you have the above dependencies installed before running the application.
+<h1 align="center">
 
-## How to Run
+EEF Datafile Extractor
 
-To run the application, follow these steps.
+</h1>
 
-1.  Clone this repository:
+The EEF Datafile Extractor is an application designed to streamline the processing of data files from the [EEF](https://educationendowmentfoundation.org.uk/education-evidence/teaching-learning-toolkit?gclid=CjwKCAjwjMiiBhA4EiwAZe6jQ3WnUgowD16xFwcG_6hZySd_qiKcElx5wRI0BjJAdwj5RkFT_kzz1hoCS_MQAvD_BwE) Education Evidence Database. The database provides JSON files with complex, nested structures, and our toolkit simplifies the process of extracting the necessary data, making it easier to integrate into your broader data processing pipeline. We provide a collection of bespoke dataframes specifically tailored for data cleaning and analysis. In addition to the pre-built dataframes, the tool includes a custom dataframe builder. This feature empowers you to compile your own dataframes based on your specific research requirements.
 
-``` bash
->> git clone https://github.com/JonathanReardon/ToolkitExtraction
->> cd ToolkitExtraction
-```
+## Installing
 
-2.  Install the required dependencies by executing the following command:
+Install with `pip` or your favorite PyPI package manager.
 
 ``` bash
->> pip install -r requirements.txt
+>> pip install eef-data
 ```
 
-3.  Run the application:
+and simply run from the command line..
 
 ``` bash
->> python3 main.py
+>> eef-data
 ```
 
-To begin, you will need to input a data file. Once you have done so, press enter to proceed to the main menu.
+When you run eef-data, you will be asked to input a data file. Once you have done so, press enter to proceed to the main menu.
 
 <p align="center">
 
-<img src="/img/visual1.png"/>
+<img src="/eefdata/img/visual1.png"/>
 
 </p>
 
 When a selection is made, the newly created file location will be displayed in the "Output Files" box at the bottom of the display.
 
 <p align="center">
 
-<img src="/img/visual3.png"/>
+<img src="/eefdata/img/visual3.png"/>
 
 </p>
 
-All output dataframes will be saved within the 'output' directory, with the directory named after the original datafile. Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
-
-<p align="center">
-
-<img src="/img/visual2.png"/>
-
-</p>
+All output dataframes will be saved with the directory named after the original datafile. Each individual dataframe will be labeled with the original datafile name as a prefix and a dataframe label suffix.
 
 ## Dataframe 1: Study, Research and Design Variables
 
 This dataframe contains 'raw', 'ht', 'info', and 'CLEAN' data types.
 
 | Data Type | Description | Number of Columns |
 | --- | --- | :----: |
```

### Comparing `eef-data-0.4/eefdata/app.py` & `eef-data-0.41/eefdata/app.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.4/eefdata/src/attributeIDs.py` & `eef-data-0.41/eefdata/src/attributeIDs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.4/eefdata/src/funcs.py` & `eef-data-0.41/eefdata/src/funcs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.4/setup.py` & `eef-data-0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='eef-data',
-    version='0.4',  # Remember to increment the version number
+    version='0.41',  # Remember to increment the version number
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy==1.22.0',
         'pandas==1.5.0',
         'prompt_toolkit==3.0.30',
         'rich==12.4.4',
```

