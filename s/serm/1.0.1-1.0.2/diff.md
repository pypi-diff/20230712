# Comparing `tmp/serm-1.0.1.tar.gz` & `tmp/serm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serm-1.0.1.tar", last modified: Tue Jul 11 22:11:45 2023, max compression
+gzip compressed data, was "serm-1.0.2.tar", last modified: Tue Jul 11 22:39:34 2023, max compression
```

## Comparing `serm-1.0.1.tar` & `serm-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:11:45.872105 serm-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 21:55:41.000000 serm-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 21:55:41.000000 serm-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-11 22:11:45.872105 serm-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-11 21:55:41.000000 serm-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 21:55:41.000000 serm-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:11:45.868105 serm-1.0.1/serm/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 21:55:41.000000 serm-1.0.1/serm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-07-11 21:55:41.000000 serm-1.0.1/serm/serm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-11 21:55:41.000000 serm-1.0.1/serm/sparseae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:11:45.872105 serm-1.0.1/serm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-11 22:11:45.000000 serm-1.0.1/serm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 22:11:45.000000 serm-1.0.1/serm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:11:45.000000 serm-1.0.1/serm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-11 22:11:45.000000 serm-1.0.1/serm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 22:11:45.000000 serm-1.0.1/serm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:11:45.872105 serm-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 21:55:41.000000 serm-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:39:34.017427 serm-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 22:20:36.000000 serm-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 22:20:36.000000 serm-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-11 22:39:34.017427 serm-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-11 22:20:36.000000 serm-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 22:20:36.000000 serm-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:39:34.017427 serm-1.0.2/serm/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 22:20:36.000000 serm-1.0.2/serm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-07-11 22:20:36.000000 serm-1.0.2/serm/serm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-11 22:20:36.000000 serm-1.0.2/serm/sparseae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:39:34.017427 serm-1.0.2/serm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:39:34.017427 serm-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 22:20:36.000000 serm-1.0.2/setup.py
```

### Comparing `serm-1.0.1/LICENSE` & `serm-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `serm-1.0.1/PKG-INFO` & `serm-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serm
-Version: 1.0.1
+Version: 1.0.2
 Summary: SERM is a high-performance data-driven gene expression recovery framework.
 Home-page: https://github.com/xinglab-ai/self-consistent-expression-recovery-machine
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 
 # Code Ocean capsule:
 
 You can run our reproducible code ocean capsule, where you just need to click once to obtain the results. Link to the capsule: https://doi.org/10.24433/CO.7874136.v1
 
 # Sample data
 
-To run the example code below, you will need to download the required data files. You can download them from [here](demo/data).
+To run the example code below, you will need to download the required data files. You can download them from [here](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/tree/main/demo/data).
 
 # Example code:
 
 ```python
 # Import all the necessary Python packages
 
 import scipy.io as sio
```

### Comparing `serm-1.0.1/README.md` & `serm-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # Code Ocean capsule:
 
 You can run our reproducible code ocean capsule, where you just need to click once to obtain the results. Link to the capsule: https://doi.org/10.24433/CO.7874136.v1
 
 # Sample data
 
-To run the example code below, you will need to download the required data files. You can download them from [here](demo/data).
+To run the example code below, you will need to download the required data files. You can download them from [here](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/tree/main/demo/data).
 
 # Example code:
 
 ```python
 # Import all the necessary Python packages
 
 import scipy.io as sio
```

### Comparing `serm-1.0.1/serm/serm.py` & `serm-1.0.2/serm/serm.py`

 * *Files identical despite different names*

### Comparing `serm-1.0.1/serm/sparseae.py` & `serm-1.0.2/serm/sparseae.py`

 * *Files identical despite different names*

### Comparing `serm-1.0.1/serm.egg-info/PKG-INFO` & `serm-1.0.2/serm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serm
-Version: 1.0.1
+Version: 1.0.2
 Summary: SERM is a high-performance data-driven gene expression recovery framework.
 Home-page: https://github.com/xinglab-ai/self-consistent-expression-recovery-machine
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 
 # Code Ocean capsule:
 
 You can run our reproducible code ocean capsule, where you just need to click once to obtain the results. Link to the capsule: https://doi.org/10.24433/CO.7874136.v1
 
 # Sample data
 
-To run the example code below, you will need to download the required data files. You can download them from [here](demo/data).
+To run the example code below, you will need to download the required data files. You can download them from [here](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/tree/main/demo/data).
 
 # Example code:
 
 ```python
 # Import all the necessary Python packages
 
 import scipy.io as sio
```

### Comparing `serm-1.0.1/setup.py` & `serm-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="serm",
-    version="1.0.1",
+    version="1.0.2",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="SERM is a high-performance data-driven gene expression recovery framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/self-consistent-expression-recovery-machine",
     classifiers=[
```

