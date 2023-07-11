# Comparing `tmp/serm-1.0.2.tar.gz` & `tmp/serm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serm-1.0.2.tar", last modified: Tue Jul 11 22:39:34 2023, max compression
+gzip compressed data, was "serm-1.0.3.tar", last modified: Tue Jul 11 23:07:03 2023, max compression
```

## Comparing `serm-1.0.2.tar` & `serm-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:39:34.017427 serm-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 22:20:36.000000 serm-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 22:20:36.000000 serm-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-11 22:39:34.017427 serm-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-11 22:20:36.000000 serm-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 22:20:36.000000 serm-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:39:34.017427 serm-1.0.2/serm/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 22:20:36.000000 serm-1.0.2/serm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-07-11 22:20:36.000000 serm-1.0.2/serm/serm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-11 22:20:36.000000 serm-1.0.2/serm/sparseae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:39:34.017427 serm-1.0.2/serm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 22:39:33.000000 serm-1.0.2/serm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:39:34.017427 serm-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 22:20:36.000000 serm-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:07:03.856591 serm-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 22:51:24.000000 serm-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 22:51:24.000000 serm-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-11 23:07:03.856591 serm-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-11 22:51:25.000000 serm-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 22:51:25.000000 serm-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:07:03.856591 serm-1.0.3/serm/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 22:51:25.000000 serm-1.0.3/serm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-07-11 22:51:25.000000 serm-1.0.3/serm/serm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-11 22:51:25.000000 serm-1.0.3/serm/sparseae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:07:03.856591 serm-1.0.3/serm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 23:07:03.000000 serm-1.0.3/serm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 23:07:03.856591 serm-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 22:51:25.000000 serm-1.0.3/setup.py
```

### Comparing `serm-1.0.2/LICENSE` & `serm-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `serm-1.0.2/PKG-INFO` & `serm-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: serm
-Version: 1.0.2
+Version: 1.0.3
 Summary: SERM is a high-performance data-driven gene expression recovery framework.
 Home-page: https://github.com/xinglab-ai/self-consistent-expression-recovery-machine
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # self-consistent-expression-recovery-machine (SERM)
 SERM is a data-driven gene expression recovery framework. Using deep learning, SERM first learns from a subset of the noisy gene expression data to estimate the underlying data distribution. SERM then recovers the overall gene expression data by analytically imposing a self- consistency on the gene expression matrix, thus ensuring that the expression levels are similarly distributed in different parts of the matrix. SERM performs much better (in most cases >20% improvement than State-of-the-art) and is computationally at least 10 times faster than other analytical techniques. Here is an exmaple of its extra-ordinary performance:
 
-![image](im2.png)
+![image](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/blob/main/im1.png)
 Figure. Percent improvement in mean Pearson coefficient of the imputed data (in comparison to the observed data) by eight different techniques for cellular taxonomy  dataset. The sampling efficiencies (0.1%-10%) to create the observed data are shown in x-axis.
 
 # How to use SERM?
 
 ## Input data and parameters
 The gene expression data should be in matrix format (rows are cells and collumns are genes). There are a few parameters: 1) ROI length and width: SERM divides the whole matrix into a number of ROIs. The user can choose the size of the ROI that would be used by SERM. Good values for ROI height can be: cell number divided by 4 or 8 and ROI width can be gene number divided by 4 or 8. 2) Percent overlap: This parameter dictates how much overlap will be between two consecutive ROIs. The user can choose any value between 0.01 to 0.99. However, for small overlap, the consecutive windows would be disconnected and for large window size, more computation will be necessary. A value between 0.25 or 0.75 works well with SERM. The requirements of different packages in Python are described in requirements.txt. 
 
@@ -99,9 +99,9 @@
 out_SERM = srm.serm(dataObs,ROIsize,percOL,randomize=False) # If you want to randomize the rows and columns
 # of the data before applying SERM, please choose randomize=True
 print('Required time:',str(time.time()-t),'second')
 ```
 
 # Results:
 
-![image](im1.png)
+![image](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/blob/main/im1.png)
 Figure. Analysis of simulated scRNA-seq data with 5 classes. The histograms of the reference data, observed data (1% sampling efficiency), and imputed data by MAGIC, mcImpute, and SERM are shown in the first row of (a). Visualization of reference, observed,  and imputed data by t-SNE and UMAP are shown in the second and third rows, respectively. t-SNE and UMAP results from SERM imputed data are much better in separating the classes, whereas MAGIC degrades the data as a result of imputation. The clustering accuracy and cluster quality indices for UMAP visualizations of imputed data from different methods are shown in (b). Data are presented as mean values +/- standard deviation (SD). Error bars represent the standard deviation of the indices for n=1000 different initializations of k-means clustering.
```

### Comparing `serm-1.0.2/README.md` & `serm-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # self-consistent-expression-recovery-machine (SERM)
 SERM is a data-driven gene expression recovery framework. Using deep learning, SERM first learns from a subset of the noisy gene expression data to estimate the underlying data distribution. SERM then recovers the overall gene expression data by analytically imposing a self- consistency on the gene expression matrix, thus ensuring that the expression levels are similarly distributed in different parts of the matrix. SERM performs much better (in most cases >20% improvement than State-of-the-art) and is computationally at least 10 times faster than other analytical techniques. Here is an exmaple of its extra-ordinary performance:
 
-![image](im2.png)
+![image](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/blob/main/im1.png)
 Figure. Percent improvement in mean Pearson coefficient of the imputed data (in comparison to the observed data) by eight different techniques for cellular taxonomy  dataset. The sampling efficiencies (0.1%-10%) to create the observed data are shown in x-axis.
 
 # How to use SERM?
 
 ## Input data and parameters
 The gene expression data should be in matrix format (rows are cells and collumns are genes). There are a few parameters: 1) ROI length and width: SERM divides the whole matrix into a number of ROIs. The user can choose the size of the ROI that would be used by SERM. Good values for ROI height can be: cell number divided by 4 or 8 and ROI width can be gene number divided by 4 or 8. 2) Percent overlap: This parameter dictates how much overlap will be between two consecutive ROIs. The user can choose any value between 0.01 to 0.99. However, for small overlap, the consecutive windows would be disconnected and for large window size, more computation will be necessary. A value between 0.25 or 0.75 works well with SERM. The requirements of different packages in Python are described in requirements.txt. 
 
@@ -85,9 +85,9 @@
 out_SERM = srm.serm(dataObs,ROIsize,percOL,randomize=False) # If you want to randomize the rows and columns
 # of the data before applying SERM, please choose randomize=True
 print('Required time:',str(time.time()-t),'second')
 ```
 
 # Results:
 
-![image](im1.png)
+![image](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/blob/main/im1.png)
 Figure. Analysis of simulated scRNA-seq data with 5 classes. The histograms of the reference data, observed data (1% sampling efficiency), and imputed data by MAGIC, mcImpute, and SERM are shown in the first row of (a). Visualization of reference, observed,  and imputed data by t-SNE and UMAP are shown in the second and third rows, respectively. t-SNE and UMAP results from SERM imputed data are much better in separating the classes, whereas MAGIC degrades the data as a result of imputation. The clustering accuracy and cluster quality indices for UMAP visualizations of imputed data from different methods are shown in (b). Data are presented as mean values +/- standard deviation (SD). Error bars represent the standard deviation of the indices for n=1000 different initializations of k-means clustering.
```

### Comparing `serm-1.0.2/serm/serm.py` & `serm-1.0.3/serm/serm.py`

 * *Files identical despite different names*

### Comparing `serm-1.0.2/serm/sparseae.py` & `serm-1.0.3/serm/sparseae.py`

 * *Files identical despite different names*

### Comparing `serm-1.0.2/serm.egg-info/PKG-INFO` & `serm-1.0.3/serm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: serm
-Version: 1.0.2
+Version: 1.0.3
 Summary: SERM is a high-performance data-driven gene expression recovery framework.
 Home-page: https://github.com/xinglab-ai/self-consistent-expression-recovery-machine
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # self-consistent-expression-recovery-machine (SERM)
 SERM is a data-driven gene expression recovery framework. Using deep learning, SERM first learns from a subset of the noisy gene expression data to estimate the underlying data distribution. SERM then recovers the overall gene expression data by analytically imposing a self- consistency on the gene expression matrix, thus ensuring that the expression levels are similarly distributed in different parts of the matrix. SERM performs much better (in most cases >20% improvement than State-of-the-art) and is computationally at least 10 times faster than other analytical techniques. Here is an exmaple of its extra-ordinary performance:
 
-![image](im2.png)
+![image](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/blob/main/im1.png)
 Figure. Percent improvement in mean Pearson coefficient of the imputed data (in comparison to the observed data) by eight different techniques for cellular taxonomy  dataset. The sampling efficiencies (0.1%-10%) to create the observed data are shown in x-axis.
 
 # How to use SERM?
 
 ## Input data and parameters
 The gene expression data should be in matrix format (rows are cells and collumns are genes). There are a few parameters: 1) ROI length and width: SERM divides the whole matrix into a number of ROIs. The user can choose the size of the ROI that would be used by SERM. Good values for ROI height can be: cell number divided by 4 or 8 and ROI width can be gene number divided by 4 or 8. 2) Percent overlap: This parameter dictates how much overlap will be between two consecutive ROIs. The user can choose any value between 0.01 to 0.99. However, for small overlap, the consecutive windows would be disconnected and for large window size, more computation will be necessary. A value between 0.25 or 0.75 works well with SERM. The requirements of different packages in Python are described in requirements.txt. 
 
@@ -99,9 +99,9 @@
 out_SERM = srm.serm(dataObs,ROIsize,percOL,randomize=False) # If you want to randomize the rows and columns
 # of the data before applying SERM, please choose randomize=True
 print('Required time:',str(time.time()-t),'second')
 ```
 
 # Results:
 
-![image](im1.png)
+![image](https://github.com/xinglab-ai/self-consistent-expression-recovery-machine/blob/main/im1.png)
 Figure. Analysis of simulated scRNA-seq data with 5 classes. The histograms of the reference data, observed data (1% sampling efficiency), and imputed data by MAGIC, mcImpute, and SERM are shown in the first row of (a). Visualization of reference, observed,  and imputed data by t-SNE and UMAP are shown in the second and third rows, respectively. t-SNE and UMAP results from SERM imputed data are much better in separating the classes, whereas MAGIC degrades the data as a result of imputation. The clustering accuracy and cluster quality indices for UMAP visualizations of imputed data from different methods are shown in (b). Data are presented as mean values +/- standard deviation (SD). Error bars represent the standard deviation of the indices for n=1000 different initializations of k-means clustering.
```

### Comparing `serm-1.0.2/setup.py` & `serm-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="serm",
-    version="1.0.2",
+    version="1.0.3",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="SERM is a high-performance data-driven gene expression recovery framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/self-consistent-expression-recovery-machine",
     classifiers=[
```

