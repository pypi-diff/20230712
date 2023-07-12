# Comparing `tmp/c45-decision-tree-1.0.0.tar.gz` & `tmp/c45-decision-tree-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c45-decision-tree-1.0.0.tar", last modified: Wed Jul 12 15:34:29 2023, max compression
+gzip compressed data, was "c45-decision-tree-1.0.1.tar", last modified: Wed Jul 12 15:46:35 2023, max compression
```

## Comparing `c45-decision-tree-1.0.0.tar` & `c45-decision-tree-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:34:29.567898 c45-decision-tree-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-12 15:34:29.552260 c45-decision-tree-1.0.0/C45/
--rw-rw-rw-   0        0        0    13676 2023-07-12 15:30:23.000000 c45-decision-tree-1.0.0/C45/__init__.py
--rw-rw-rw-   0        0        0     3761 2023-07-12 15:34:29.567898 c45-decision-tree-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3329 2023-07-12 15:13:40.000000 c45-decision-tree-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 15:34:29.567898 c45-decision-tree-1.0.0/c45_decision_tree.egg-info/
--rw-rw-rw-   0        0        0     3761 2023-07-12 15:34:29.000000 c45-decision-tree-1.0.0/c45_decision_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-07-12 15:34:29.000000 c45-decision-tree-1.0.0/c45_decision_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:34:29.000000 c45-decision-tree-1.0.0/c45_decision_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-12 15:34:29.000000 c45-decision-tree-1.0.0/c45_decision_tree.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:34:29.567898 c45-decision-tree-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-07-12 15:23:13.000000 c45-decision-tree-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/C45/
+-rw-rw-rw-   0        0        0    13676 2023-07-12 15:30:23.000000 c45-decision-tree-1.0.1/C45/__init__.py
+-rw-rw-rw-   0        0        0     3836 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3404 2023-07-12 15:41:03.000000 c45-decision-tree-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/
+-rw-rw-rw-   0        0        0     3836 2023-07-12 15:46:35.000000 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-07-12 15:46:35.000000 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:46:35.000000 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-12 15:46:35.000000 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-07-12 15:39:27.000000 c45-decision-tree-1.0.1/setup.py
```

### Comparing `c45-decision-tree-1.0.0/C45/__init__.py` & `c45-decision-tree-1.0.1/C45/__init__.py`

 * *Files identical despite different names*

### Comparing `c45-decision-tree-1.0.0/PKG-INFO` & `c45-decision-tree-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c45-decision-tree
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for C4.5 Decision Tree Algorithm
 Home-page: https://github.com/novandikp/DecisionTreeC45
 Author: Novandi Kevin Pratama
 Author-email: kevinpret27@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,19 +22,24 @@
 ```
 where
 ```
 SplitInfo(S, A) = - sum ( |Sv| / |S| ) * log2 ( |Sv| / |S| )
 ```
 and Sv is the subset of S for which attribute A has value v.
 
+## Requirements
+- Python 3.6 or above
+- Pandas
+- Numpy
+
 ## Implementation
 
 ### Installation
 ```
-pip install c45
+pip install c45-decision-tree
 ```
 
 ### Train Model
 For training model, you need to prepare data in pandas dataframe format. For train model you need to can call `fit` method with 2 parameters, first is data and second is target. For example:
 ```python
 from C45 import C45Classifier
 import pandas as pd
```

### Comparing `c45-decision-tree-1.0.0/README.md` & `c45-decision-tree-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,24 @@
 ```
 where
 ```
 SplitInfo(S, A) = - sum ( |Sv| / |S| ) * log2 ( |Sv| / |S| )
 ```
 and Sv is the subset of S for which attribute A has value v.
 
+## Requirements
+- Python 3.6 or above
+- Pandas
+- Numpy
+
 ## Implementation
 
 ### Installation
 ```
-pip install c45
+pip install c45-decision-tree
 ```
 
 ### Train Model
 For training model, you need to prepare data in pandas dataframe format. For train model you need to can call `fit` method with 2 parameters, first is data and second is target. For example:
 ```python
 from C45 import C45Classifier
 import pandas as pd
```

### Comparing `c45-decision-tree-1.0.0/c45_decision_tree.egg-info/PKG-INFO` & `c45-decision-tree-1.0.1/c45_decision_tree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c45-decision-tree
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for C4.5 Decision Tree Algorithm
 Home-page: https://github.com/novandikp/DecisionTreeC45
 Author: Novandi Kevin Pratama
 Author-email: kevinpret27@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,19 +22,24 @@
 ```
 where
 ```
 SplitInfo(S, A) = - sum ( |Sv| / |S| ) * log2 ( |Sv| / |S| )
 ```
 and Sv is the subset of S for which attribute A has value v.
 
+## Requirements
+- Python 3.6 or above
+- Pandas
+- Numpy
+
 ## Implementation
 
 ### Installation
 ```
-pip install c45
+pip install c45-decision-tree
 ```
 
 ### Train Model
 For training model, you need to prepare data in pandas dataframe format. For train model you need to can call `fit` method with 2 parameters, first is data and second is target. For example:
 ```python
 from C45 import C45Classifier
 import pandas as pd
```

### Comparing `c45-decision-tree-1.0.0/setup.py` & `c45-decision-tree-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="c45-decision-tree",
-    version="1.0.0",
+    version="1.0.1",
     author="Novandi Kevin Pratama",
     author_email="kevinpret27@gmail.com",
     description="Library for C4.5 Decision Tree Algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novandikp/DecisionTreeC45",
     packages=setuptools.find_packages(),
```

