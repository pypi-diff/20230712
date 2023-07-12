# Comparing `tmp/histeqkit-0.0.5.tar.gz` & `tmp/histeqkit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histeqkit-0.0.5.tar", last modified: Mon Jul 10 19:06:46 2023, max compression
+gzip compressed data, was "histeqkit-0.0.6.tar", last modified: Wed Jul 12 10:28:29 2023, max compression
```

## Comparing `histeqkit-0.0.5.tar` & `histeqkit-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 adityaraj   (501) staff       (20)        0 2023-07-10 19:06:46.344630 histeqkit-0.0.5/
--rw-r--r--   0 adityaraj   (501) staff       (20)        0 2023-07-10 17:38:45.000000 histeqkit-0.0.5/LICENSE
--rw-r--r--   0 adityaraj   (501) staff       (20)     2160 2023-07-10 19:06:46.344684 histeqkit-0.0.5/PKG-INFO
--rw-r--r--   0 adityaraj   (501) staff       (20)     1614 2023-07-10 19:05:03.000000 histeqkit-0.0.5/README.md
--rw-r--r--   0 adityaraj   (501) staff       (20)      103 2023-07-10 17:44:52.000000 histeqkit-0.0.5/pyproject.toml
--rw-r--r--   0 adityaraj   (501) staff       (20)      671 2023-07-10 19:06:46.344903 histeqkit-0.0.5/setup.cfg
-drwxr-xr-x   0 adityaraj   (501) staff       (20)        0 2023-07-10 19:06:46.342245 histeqkit-0.0.5/src/
-drwxr-xr-x   0 adityaraj   (501) staff       (20)        0 2023-07-10 19:06:46.344015 histeqkit-0.0.5/src/histeqkit/
--rw-r--r--   0 adityaraj   (501) staff       (20)       99 2023-07-10 18:22:08.000000 histeqkit-0.0.5/src/histeqkit/__init__.py
--rw-r--r--   0 adityaraj   (501) staff       (20)     1612 2023-07-10 16:54:55.000000 histeqkit-0.0.5/src/histeqkit/accuracyMeasure.py
--rw-r--r--   0 adityaraj   (501) staff       (20)    20009 2023-07-10 18:42:20.000000 histeqkit-0.0.5/src/histeqkit/algorithms.py
--rw-r--r--   0 adityaraj   (501) staff       (20)     4076 2023-07-10 16:49:25.000000 histeqkit-0.0.5/src/histeqkit/histogram.py
--rw-r--r--   0 adityaraj   (501) staff       (20)      470 2023-07-10 17:44:27.000000 histeqkit-0.0.5/src/histeqkit/main.py
--rw-r--r--   0 adityaraj   (501) staff       (20)     2382 2023-07-10 17:50:50.000000 histeqkit-0.0.5/src/histeqkit/utils.py
-drwxr-xr-x   0 adityaraj   (501) staff       (20)        0 2023-07-10 19:06:46.344523 histeqkit-0.0.5/src/histeqkit.egg-info/
--rw-r--r--   0 adityaraj   (501) staff       (20)     2160 2023-07-10 19:06:46.000000 histeqkit-0.0.5/src/histeqkit.egg-info/PKG-INFO
--rw-r--r--   0 adityaraj   (501) staff       (20)      349 2023-07-10 19:06:46.000000 histeqkit-0.0.5/src/histeqkit.egg-info/SOURCES.txt
--rw-r--r--   0 adityaraj   (501) staff       (20)        1 2023-07-10 19:06:46.000000 histeqkit-0.0.5/src/histeqkit.egg-info/dependency_links.txt
--rw-r--r--   0 adityaraj   (501) staff       (20)       10 2023-07-10 19:06:46.000000 histeqkit-0.0.5/src/histeqkit.egg-info/top_level.txt
+drwxr-xr-x   0 adityaraj   (501) staff       (20)        0 2023-07-12 10:28:29.534254 histeqkit-0.0.6/
+-rw-r--r--   0 adityaraj   (501) staff       (20)        0 2023-07-10 17:38:45.000000 histeqkit-0.0.6/LICENSE
+-rw-r--r--   0 adityaraj   (501) staff       (20)     2134 2023-07-12 10:28:29.534300 histeqkit-0.0.6/PKG-INFO
+-rw-r--r--   0 adityaraj   (501) staff       (20)     1588 2023-07-12 10:27:40.000000 histeqkit-0.0.6/README.md
+-rw-r--r--   0 adityaraj   (501) staff       (20)      103 2023-07-10 17:44:52.000000 histeqkit-0.0.6/pyproject.toml
+-rw-r--r--   0 adityaraj   (501) staff       (20)      671 2023-07-12 10:28:29.534503 histeqkit-0.0.6/setup.cfg
+drwxr-xr-x   0 adityaraj   (501) staff       (20)        0 2023-07-12 10:28:29.531407 histeqkit-0.0.6/src/
+drwxr-xr-x   0 adityaraj   (501) staff       (20)        0 2023-07-12 10:28:29.533409 histeqkit-0.0.6/src/histeqkit/
+-rw-r--r--   0 adityaraj   (501) staff       (20)       99 2023-07-10 18:22:08.000000 histeqkit-0.0.6/src/histeqkit/__init__.py
+-rw-r--r--   0 adityaraj   (501) staff       (20)     1612 2023-07-10 16:54:55.000000 histeqkit-0.0.6/src/histeqkit/accuracyMeasure.py
+-rw-r--r--   0 adityaraj   (501) staff       (20)    20009 2023-07-10 18:42:20.000000 histeqkit-0.0.6/src/histeqkit/algorithms.py
+-rw-r--r--   0 adityaraj   (501) staff       (20)     4076 2023-07-10 16:49:25.000000 histeqkit-0.0.6/src/histeqkit/histogram.py
+-rw-r--r--   0 adityaraj   (501) staff       (20)      470 2023-07-10 17:44:27.000000 histeqkit-0.0.6/src/histeqkit/main.py
+-rw-r--r--   0 adityaraj   (501) staff       (20)     2382 2023-07-10 17:50:50.000000 histeqkit-0.0.6/src/histeqkit/utils.py
+drwxr-xr-x   0 adityaraj   (501) staff       (20)        0 2023-07-12 10:28:29.534157 histeqkit-0.0.6/src/histeqkit.egg-info/
+-rw-r--r--   0 adityaraj   (501) staff       (20)     2134 2023-07-12 10:28:29.000000 histeqkit-0.0.6/src/histeqkit.egg-info/PKG-INFO
+-rw-r--r--   0 adityaraj   (501) staff       (20)      349 2023-07-12 10:28:29.000000 histeqkit-0.0.6/src/histeqkit.egg-info/SOURCES.txt
+-rw-r--r--   0 adityaraj   (501) staff       (20)        1 2023-07-12 10:28:29.000000 histeqkit-0.0.6/src/histeqkit.egg-info/dependency_links.txt
+-rw-r--r--   0 adityaraj   (501) staff       (20)       10 2023-07-12 10:28:29.000000 histeqkit-0.0.6/src/histeqkit.egg-info/top_level.txt
```

### Comparing `histeqkit-0.0.5/PKG-INFO` & `histeqkit-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histeqkit
-Version: 0.0.5
+Version: 0.0.6
 Summary: package for histogram equalization algorithms and image accuracy measures.
 Home-page: https://github.com/pypa/sampleproject
 Author: Aditya Raj
 Author-email: aditya2134.ar@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 HistEQKit is a Python package that provides a collection of histogram equalization algorithms and image accuracy measures for image enhancement and analysis tasks.
 
 ## Installation
 
 You can install HistEQKit using pip:
 
 ```shell
-pip install -i https://test.pypi.org/simple/ histeqkit
+pip install histeqkit==0.0.5
 ```
 
 HistEQKit requires Python 3.6 or higher.
 
 Usage
 
 To use HistEQKit, import the desired histogram equalization algorithms from the package,
```

### Comparing `histeqkit-0.0.5/README.md` & `histeqkit-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 HistEQKit is a Python package that provides a collection of histogram equalization algorithms and image accuracy measures for image enhancement and analysis tasks.
 
 ## Installation
 
 You can install HistEQKit using pip:
 
 ```shell
-pip install -i https://test.pypi.org/simple/ histeqkit
+pip install histeqkit==0.0.5
 ```
 
 HistEQKit requires Python 3.6 or higher.
 
 Usage
 
 To use HistEQKit, import the desired histogram equalization algorithms from the package,
```

### Comparing `histeqkit-0.0.5/setup.cfg` & `histeqkit-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = histeqkit
-version = 0.0.5
+version = 0.0.6
 author = Aditya Raj
 author_email = aditya2134.ar@gmail.com
 description = package for histogram equalization algorithms and image accuracy measures.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `histeqkit-0.0.5/src/histeqkit/accuracyMeasure.py` & `histeqkit-0.0.6/src/histeqkit/accuracyMeasure.py`

 * *Files identical despite different names*

### Comparing `histeqkit-0.0.5/src/histeqkit/algorithms.py` & `histeqkit-0.0.6/src/histeqkit/algorithms.py`

 * *Files identical despite different names*

### Comparing `histeqkit-0.0.5/src/histeqkit/histogram.py` & `histeqkit-0.0.6/src/histeqkit/histogram.py`

 * *Files identical despite different names*

### Comparing `histeqkit-0.0.5/src/histeqkit/utils.py` & `histeqkit-0.0.6/src/histeqkit/utils.py`

 * *Files identical despite different names*

### Comparing `histeqkit-0.0.5/src/histeqkit.egg-info/PKG-INFO` & `histeqkit-0.0.6/src/histeqkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histeqkit
-Version: 0.0.5
+Version: 0.0.6
 Summary: package for histogram equalization algorithms and image accuracy measures.
 Home-page: https://github.com/pypa/sampleproject
 Author: Aditya Raj
 Author-email: aditya2134.ar@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 HistEQKit is a Python package that provides a collection of histogram equalization algorithms and image accuracy measures for image enhancement and analysis tasks.
 
 ## Installation
 
 You can install HistEQKit using pip:
 
 ```shell
-pip install -i https://test.pypi.org/simple/ histeqkit
+pip install histeqkit==0.0.5
 ```
 
 HistEQKit requires Python 3.6 or higher.
 
 Usage
 
 To use HistEQKit, import the desired histogram equalization algorithms from the package,
```

