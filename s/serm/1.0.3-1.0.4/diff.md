# Comparing `tmp/serm-1.0.3.tar.gz` & `tmp/serm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serm-1.0.3.tar", last modified: Tue Jul 11 23:07:03 2023, max compression
+gzip compressed data, was "serm-1.0.4.tar", last modified: Wed Jul 12 01:08:53 2023, max compression
```

## Comparing `serm-1.0.3.tar` & `serm-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:07:03.856591 serm-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 22:51:24.000000 serm-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 22:51:24.000000 serm-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-11 23:07:03.856591 serm-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-11 22:51:25.000000 serm-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 22:51:25.000000 serm-1.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:07:03.856591 serm-1.0.3/serm/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 22:51:25.000000 serm-1.0.3/serm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-07-11 22:51:25.000000 serm-1.0.3/serm/serm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-11 22:51:25.000000 serm-1.0.3/serm/sparseae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:07:03.856591 serm-1.0.3/serm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 23:07:03.856591 serm-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 22:51:25.000000 serm-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:08:53.679705 serm-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 00:52:20.000000 serm-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 00:52:20.000000 serm-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-12 01:08:53.679705 serm-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-07-12 00:52:20.000000 serm-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 00:52:21.000000 serm-1.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:08:53.679705 serm-1.0.4/serm/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 00:52:21.000000 serm-1.0.4/serm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-07-12 00:52:21.000000 serm-1.0.4/serm/serm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-12 00:52:21.000000 serm-1.0.4/serm/sparseae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:08:53.679705 serm-1.0.4/serm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-12 01:08:53.000000 serm-1.0.4/serm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-12 01:08:53.000000 serm-1.0.4/serm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:08:53.000000 serm-1.0.4/serm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-12 01:08:53.000000 serm-1.0.4/serm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 01:08:53.000000 serm-1.0.4/serm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:08:53.679705 serm-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-12 00:52:21.000000 serm-1.0.4/setup.py
```

### Comparing `serm-1.0.3/LICENSE` & `serm-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `serm-1.0.3/PKG-INFO` & `serm-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serm
-Version: 1.0.3
+Version: 1.0.4
 Summary: SERM is a high-performance data-driven gene expression recovery framework.
 Home-page: https://github.com/xinglab-ai/self-consistent-expression-recovery-machine
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -39,66 +39,62 @@
 
 # Code Ocean capsule:
 
 You can run our reproducible code ocean capsule, where you just need to click once to obtain the results. Link to the capsule: https://doi.org/10.24433/CO.7874136.v1
 
 # Sample data
 
-To run the example code below, you will need to download the required data files. You can download them from [here](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/tree/main/demo/data).
+To run the example code below, you will need to download the required data files. You can download them from [here](https://drive.google.com/drive/folders/13diFWPuZpncZE27OGQ0lplElsVCaSYog).
 
 # Example code:
 
 ```python
 # Import all the necessary Python packages
 
 import scipy.io as sio
 import serm as srm
 import random
 import time
 
 # Load the reference data, the observed data, and the data labels
-# The raw data is from the work of Baryawno et al. 
-# Reference: Baryawno, Ninib, et al. "A cellular taxonomy 
+# The raw data is from the work of Baryawno et al.
+# Reference: Baryawno, Ninib, et al. "A cellular taxonomy
 # of the bone marrow stroma in homeostasis and leukemia." Cell 177.7 (2019): 1915-1932.
-# The data from the authors contains 23092 cells and 27998 genes. 
-# The raw data is added in 'data' folder of this capsule. Following Huang et al 
-# (Nature Methods 15, 539–542 (2018)), we choose 12,162 cells and 2,422 genes with 
+# The data from the authors contains 23092 cells and 27998 genes.
+# The raw data is added in 'data' folder of this capsule. Following Huang et al
+# (Nature Methods 15, 539–542 (2018)), we choose 12,162 cells and 2,422 genes with
 # high expression to create a reference dataset.
-# 
-# The following two code lines read the reference data 
-a=sio.loadmat('demo/data/data_reference.mat')
+
+# The following two code lines read the reference data
+a=sio.loadmat('data_reference.mat')
 dataRef=a['data_reference']
 
-# The observed data were generated from the reference data by simulating efficiency loss that introduces zeros 
+# The observed data were generated from the reference data by simulating efficiency loss that introduces zeros
 # following the work of Huang et al.
 # The following three code lines were used from Huang et al to create observed data with 10%
 # sampling efficiency: (detail code (demo_creation_observedData.R) is also added in the 'code' folder
 # of this capsule)
 # alpha <- rgamma(ncol(data.filt), 10, 100)
 # data_observed <- t(apply(sweep(data.filt, 2, alpha, "*"), 1, function(data)
 #  rpois(length(data), data)))
 
 # The following two code lines read the observed data for 10% sampling efficiency
-a=sio.loadmat('demo/data/data_observed_10perc.mat')
+a=sio.loadmat('data_observed_10perc.mat')
 dataObs=a['data_observed']
 
-# Load data labels 
-a=sio.loadmat('demo/data/data_label.mat')
-dataLabel=a['data_label']
-
 # Selection of the size of the region of interest (ROI)
 # We choose ROI size in such a way that the expression matrix
 # is divided into 4 (i.e. 2 by 2) ROIs. However, other ROI sizes are also
-# fine as SERM is generally very robust against the ROI size. 
+# fine as SERM is generally very robust against the ROI size.
 ROIsize = [6100,1250]
-# Selection of percent of overlap between successive ROIs. The default value is 50%, but other 
+# Selection of percent of overlap between successive ROIs. The default value is 50%, but other
 # values can be chosen
 percOL = 0.5
 t=time.time() # For keeping record of computational time
-random.seed(0) # Setting the random number generator seed to 0. 
+random.seed(0) # Setting the random number generator seed to 0.
 # Run SERM
 out_SERM = srm.serm(dataObs,ROIsize,percOL,randomize=False) # If you want to randomize the rows and columns
 # of the data before applying SERM, please choose randomize=True
 print('Required time:',str(time.time()-t),'second')
 ```
 
 # Results:
```

### Comparing `serm-1.0.3/README.md` & `serm-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,66 +25,62 @@
 
 # Code Ocean capsule:
 
 You can run our reproducible code ocean capsule, where you just need to click once to obtain the results. Link to the capsule: https://doi.org/10.24433/CO.7874136.v1
 
 # Sample data
 
-To run the example code below, you will need to download the required data files. You can download them from [here](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/tree/main/demo/data).
+To run the example code below, you will need to download the required data files. You can download them from [here](https://drive.google.com/drive/folders/13diFWPuZpncZE27OGQ0lplElsVCaSYog).
 
 # Example code:
 
 ```python
 # Import all the necessary Python packages
 
 import scipy.io as sio
 import serm as srm
 import random
 import time
 
 # Load the reference data, the observed data, and the data labels
-# The raw data is from the work of Baryawno et al. 
-# Reference: Baryawno, Ninib, et al. "A cellular taxonomy 
+# The raw data is from the work of Baryawno et al.
+# Reference: Baryawno, Ninib, et al. "A cellular taxonomy
 # of the bone marrow stroma in homeostasis and leukemia." Cell 177.7 (2019): 1915-1932.
-# The data from the authors contains 23092 cells and 27998 genes. 
-# The raw data is added in 'data' folder of this capsule. Following Huang et al 
-# (Nature Methods 15, 539–542 (2018)), we choose 12,162 cells and 2,422 genes with 
+# The data from the authors contains 23092 cells and 27998 genes.
+# The raw data is added in 'data' folder of this capsule. Following Huang et al
+# (Nature Methods 15, 539–542 (2018)), we choose 12,162 cells and 2,422 genes with
 # high expression to create a reference dataset.
-# 
-# The following two code lines read the reference data 
-a=sio.loadmat('demo/data/data_reference.mat')
+
+# The following two code lines read the reference data
+a=sio.loadmat('data_reference.mat')
 dataRef=a['data_reference']
 
-# The observed data were generated from the reference data by simulating efficiency loss that introduces zeros 
+# The observed data were generated from the reference data by simulating efficiency loss that introduces zeros
 # following the work of Huang et al.
 # The following three code lines were used from Huang et al to create observed data with 10%
 # sampling efficiency: (detail code (demo_creation_observedData.R) is also added in the 'code' folder
 # of this capsule)
 # alpha <- rgamma(ncol(data.filt), 10, 100)
 # data_observed <- t(apply(sweep(data.filt, 2, alpha, "*"), 1, function(data)
 #  rpois(length(data), data)))
 
 # The following two code lines read the observed data for 10% sampling efficiency
-a=sio.loadmat('demo/data/data_observed_10perc.mat')
+a=sio.loadmat('data_observed_10perc.mat')
 dataObs=a['data_observed']
 
-# Load data labels 
-a=sio.loadmat('demo/data/data_label.mat')
-dataLabel=a['data_label']
-
 # Selection of the size of the region of interest (ROI)
 # We choose ROI size in such a way that the expression matrix
 # is divided into 4 (i.e. 2 by 2) ROIs. However, other ROI sizes are also
-# fine as SERM is generally very robust against the ROI size. 
+# fine as SERM is generally very robust against the ROI size.
 ROIsize = [6100,1250]
-# Selection of percent of overlap between successive ROIs. The default value is 50%, but other 
+# Selection of percent of overlap between successive ROIs. The default value is 50%, but other
 # values can be chosen
 percOL = 0.5
 t=time.time() # For keeping record of computational time
-random.seed(0) # Setting the random number generator seed to 0. 
+random.seed(0) # Setting the random number generator seed to 0.
 # Run SERM
 out_SERM = srm.serm(dataObs,ROIsize,percOL,randomize=False) # If you want to randomize the rows and columns
 # of the data before applying SERM, please choose randomize=True
 print('Required time:',str(time.time()-t),'second')
 ```
 
 # Results:
```

### Comparing `serm-1.0.3/serm/serm.py` & `serm-1.0.4/serm/serm.py`

 * *Files identical despite different names*

### Comparing `serm-1.0.3/serm/sparseae.py` & `serm-1.0.4/serm/sparseae.py`

 * *Files identical despite different names*

### Comparing `serm-1.0.3/serm.egg-info/PKG-INFO` & `serm-1.0.4/serm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serm
-Version: 1.0.3
+Version: 1.0.4
 Summary: SERM is a high-performance data-driven gene expression recovery framework.
 Home-page: https://github.com/xinglab-ai/self-consistent-expression-recovery-machine
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -39,66 +39,62 @@
 
 # Code Ocean capsule:
 
 You can run our reproducible code ocean capsule, where you just need to click once to obtain the results. Link to the capsule: https://doi.org/10.24433/CO.7874136.v1
 
 # Sample data
 
-To run the example code below, you will need to download the required data files. You can download them from [here](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/tree/main/demo/data).
+To run the example code below, you will need to download the required data files. You can download them from [here](https://drive.google.com/drive/folders/13diFWPuZpncZE27OGQ0lplElsVCaSYog).
 
 # Example code:
 
 ```python
 # Import all the necessary Python packages
 
 import scipy.io as sio
 import serm as srm
 import random
 import time
 
 # Load the reference data, the observed data, and the data labels
-# The raw data is from the work of Baryawno et al. 
-# Reference: Baryawno, Ninib, et al. "A cellular taxonomy 
+# The raw data is from the work of Baryawno et al.
+# Reference: Baryawno, Ninib, et al. "A cellular taxonomy
 # of the bone marrow stroma in homeostasis and leukemia." Cell 177.7 (2019): 1915-1932.
-# The data from the authors contains 23092 cells and 27998 genes. 
-# The raw data is added in 'data' folder of this capsule. Following Huang et al 
-# (Nature Methods 15, 539–542 (2018)), we choose 12,162 cells and 2,422 genes with 
+# The data from the authors contains 23092 cells and 27998 genes.
+# The raw data is added in 'data' folder of this capsule. Following Huang et al
+# (Nature Methods 15, 539–542 (2018)), we choose 12,162 cells and 2,422 genes with
 # high expression to create a reference dataset.
-# 
-# The following two code lines read the reference data 
-a=sio.loadmat('demo/data/data_reference.mat')
+
+# The following two code lines read the reference data
+a=sio.loadmat('data_reference.mat')
 dataRef=a['data_reference']
 
-# The observed data were generated from the reference data by simulating efficiency loss that introduces zeros 
+# The observed data were generated from the reference data by simulating efficiency loss that introduces zeros
 # following the work of Huang et al.
 # The following three code lines were used from Huang et al to create observed data with 10%
 # sampling efficiency: (detail code (demo_creation_observedData.R) is also added in the 'code' folder
 # of this capsule)
 # alpha <- rgamma(ncol(data.filt), 10, 100)
 # data_observed <- t(apply(sweep(data.filt, 2, alpha, "*"), 1, function(data)
 #  rpois(length(data), data)))
 
 # The following two code lines read the observed data for 10% sampling efficiency
-a=sio.loadmat('demo/data/data_observed_10perc.mat')
+a=sio.loadmat('data_observed_10perc.mat')
 dataObs=a['data_observed']
 
-# Load data labels 
-a=sio.loadmat('demo/data/data_label.mat')
-dataLabel=a['data_label']
-
 # Selection of the size of the region of interest (ROI)
 # We choose ROI size in such a way that the expression matrix
 # is divided into 4 (i.e. 2 by 2) ROIs. However, other ROI sizes are also
-# fine as SERM is generally very robust against the ROI size. 
+# fine as SERM is generally very robust against the ROI size.
 ROIsize = [6100,1250]
-# Selection of percent of overlap between successive ROIs. The default value is 50%, but other 
+# Selection of percent of overlap between successive ROIs. The default value is 50%, but other
 # values can be chosen
 percOL = 0.5
 t=time.time() # For keeping record of computational time
-random.seed(0) # Setting the random number generator seed to 0. 
+random.seed(0) # Setting the random number generator seed to 0.
 # Run SERM
 out_SERM = srm.serm(dataObs,ROIsize,percOL,randomize=False) # If you want to randomize the rows and columns
 # of the data before applying SERM, please choose randomize=True
 print('Required time:',str(time.time()-t),'second')
 ```
 
 # Results:
```

### Comparing `serm-1.0.3/setup.py` & `serm-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="serm",
-    version="1.0.3",
+    version="1.0.4",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="SERM is a high-performance data-driven gene expression recovery framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/self-consistent-expression-recovery-machine",
     classifiers=[
```

