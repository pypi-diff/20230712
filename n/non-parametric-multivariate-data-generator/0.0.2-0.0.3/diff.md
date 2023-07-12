# Comparing `tmp/non-parametric-multivariate-data-generator-0.0.2.tar.gz` & `tmp/non-parametric-multivariate-data-generator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "non-parametric-multivariate-data-generator-0.0.2.tar", last modified: Wed May 10 16:42:08 2023, max compression
+gzip compressed data, was "non-parametric-multivariate-data-generator-0.0.3.tar", last modified: Wed Jul 12 01:32:11 2023, max compression
```

## Comparing `non-parametric-multivariate-data-generator-0.0.2.tar` & `non-parametric-multivariate-data-generator-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 pablo.osorio   (504) staff       (20)        0 2023-05-10 16:42:08.363135 non-parametric-multivariate-data-generator-0.0.2/
--rw-r--r--   0 pablo.osorio   (504) staff       (20)     4571 2023-05-07 20:56:19.000000 non-parametric-multivariate-data-generator-0.0.2/LICENSE
--rw-r--r--   0 pablo.osorio   (504) staff       (20)     5788 2023-05-10 16:42:08.362316 non-parametric-multivariate-data-generator-0.0.2/PKG-INFO
--rw-r--r--   0 pablo.osorio   (504) staff       (20)     2668 2023-05-10 16:40:51.000000 non-parametric-multivariate-data-generator-0.0.2/README.md
--rw-r--r--   0 pablo.osorio   (504) staff       (20)      904 2023-05-10 16:40:49.000000 non-parametric-multivariate-data-generator-0.0.2/pyproject.toml
--rw-r--r--   0 pablo.osorio   (504) staff       (20)       38 2023-05-10 16:42:08.363246 non-parametric-multivariate-data-generator-0.0.2/setup.cfg
-drwxr-xr-x   0 pablo.osorio   (504) staff       (20)        0 2023-05-10 16:42:08.333010 non-parametric-multivariate-data-generator-0.0.2/src/
--rw-r--r--   0 pablo.osorio   (504) staff       (20)        0 2023-05-08 22:55:33.000000 non-parametric-multivariate-data-generator-0.0.2/src/__init__.py
-drwxr-xr-x   0 pablo.osorio   (504) staff       (20)        0 2023-05-10 16:42:08.336549 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric/
--rw-r--r--   0 pablo.osorio   (504) staff       (20)       65 2023-05-10 15:54:28.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric/__init__.py
--rw-r--r--   0 pablo.osorio   (504) staff       (20)      790 2023-05-09 23:31:26.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric/empirical_cumulative_distribution.py
--rw-r--r--   0 pablo.osorio   (504) staff       (20)      892 2023-05-09 23:31:26.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric/frequency_table.py
--rw-r--r--   0 pablo.osorio   (504) staff       (20)      451 2023-05-09 23:31:26.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric/plot_comparision.py
--rw-r--r--   0 pablo.osorio   (504) staff       (20)     2945 2023-05-10 16:27:53.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric/synthetic_data_generator.py
-drwxr-xr-x   0 pablo.osorio   (504) staff       (20)        0 2023-05-10 16:42:08.361184 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric_multivariate_data_generator.egg-info/
--rw-r--r--   0 pablo.osorio   (504) staff       (20)     5788 2023-05-10 16:42:08.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric_multivariate_data_generator.egg-info/PKG-INFO
--rw-r--r--   0 pablo.osorio   (504) staff       (20)      608 2023-05-10 16:42:08.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric_multivariate_data_generator.egg-info/SOURCES.txt
--rw-r--r--   0 pablo.osorio   (504) staff       (20)        1 2023-05-10 16:42:08.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric_multivariate_data_generator.egg-info/dependency_links.txt
--rw-r--r--   0 pablo.osorio   (504) staff       (20)      179 2023-05-10 16:42:08.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric_multivariate_data_generator.egg-info/requires.txt
--rw-r--r--   0 pablo.osorio   (504) staff       (20)       24 2023-05-10 16:42:08.000000 non-parametric-multivariate-data-generator-0.0.2/src/non_parametric_multivariate_data_generator.egg-info/top_level.txt
+drwxr-xr-x   0 pablo.osorio   (504) staff       (20)        0 2023-07-12 01:32:11.119171 non-parametric-multivariate-data-generator-0.0.3/
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)     4571 2023-07-12 00:54:43.000000 non-parametric-multivariate-data-generator-0.0.3/LICENSE
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)     5788 2023-07-12 01:32:11.118157 non-parametric-multivariate-data-generator-0.0.3/PKG-INFO
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)     2769 2023-07-12 01:30:54.000000 non-parametric-multivariate-data-generator-0.0.3/README.md
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)      856 2023-07-12 01:31:52.000000 non-parametric-multivariate-data-generator-0.0.3/pyproject.toml
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)       38 2023-07-12 01:32:11.119274 non-parametric-multivariate-data-generator-0.0.3/setup.cfg
+drwxr-xr-x   0 pablo.osorio   (504) staff       (20)        0 2023-07-12 01:32:11.099804 non-parametric-multivariate-data-generator-0.0.3/src/
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)        0 2023-07-12 00:55:51.000000 non-parametric-multivariate-data-generator-0.0.3/src/__init__.py
+drwxr-xr-x   0 pablo.osorio   (504) staff       (20)        0 2023-07-12 01:32:11.106863 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric/
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)       65 2023-07-12 00:56:33.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric/__init__.py
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)      790 2023-07-12 00:56:33.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric/empirical_cumulative_distribution.py
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)      892 2023-07-12 00:56:33.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric/frequency_table.py
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)      451 2023-07-12 00:56:33.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric/plot_comparision.py
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)     2985 2023-07-12 00:56:33.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric/synthetic_data_generator.py
+drwxr-xr-x   0 pablo.osorio   (504) staff       (20)        0 2023-07-12 01:32:11.115071 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric_multivariate_data_generator.egg-info/
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)     5788 2023-07-12 01:32:11.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric_multivariate_data_generator.egg-info/PKG-INFO
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)      629 2023-07-12 01:32:11.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric_multivariate_data_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)        1 2023-07-12 01:32:11.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric_multivariate_data_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)      145 2023-07-12 01:32:11.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric_multivariate_data_generator.egg-info/requires.txt
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)       24 2023-07-12 01:32:11.000000 non-parametric-multivariate-data-generator-0.0.3/src/non_parametric_multivariate_data_generator.egg-info/top_level.txt
+drwxr-xr-x   0 pablo.osorio   (504) staff       (20)        0 2023-07-12 01:32:11.116384 non-parametric-multivariate-data-generator-0.0.3/tests/
+-rw-r--r--   0 pablo.osorio   (504) staff       (20)      436 2023-07-12 01:30:23.000000 non-parametric-multivariate-data-generator-0.0.3/tests/test_shapes.py
```

### Comparing `non-parametric-multivariate-data-generator-0.0.2/LICENSE` & `non-parametric-multivariate-data-generator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `non-parametric-multivariate-data-generator-0.0.2/PKG-INFO` & `non-parametric-multivariate-data-generator-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: non-parametric-multivariate-data-generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: "Juan P. Restrepo" <jurest82@eafit.edu.co>, Pablo Osorio <osoriopabl@gmail.com>
 License: License text copyright © 2017 MariaDB Corporation Ab, All Rights Reserved.
         “Business Source License” is a trademark of MariaDB Corporation Ab.
         
         Licensed Work:        Non-parametric-multivariate-data-generator
```

### Comparing `non-parametric-multivariate-data-generator-0.0.2/README.md` & `non-parametric-multivariate-data-generator-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Non-parametric-multivariate-data-generator
 
 
-This repository contains the code for the Python3 implementation of the
-method explained in the following article:
-Restrepo L., J. Pablo; Rivera, J.C.; Laniado, H., Osorio, P; Becerra, O.
-[Nonparametric Generation of Synthetic Data Using Copulas. Electronics 2023, 12, 1601.](https://doi.org/10.3390/electronics12071601)
+This repository contains the code for the Python3 implementation of the method explained in the following article:
+Restrepo, J.P.; Rivera, J.C.; Laniado, H.; Osorio, P.; Becerra, O.A. Nonparametric Generation of Synthetic Data Using Copulas. Electronics 2023, 12, 1601. https://doi.org/10.3390/electronics12071601
 
 
 ## License
 
 This package is part of this stack will be "source available", not
 “open source”, although that will provide nearly all of the openness
 that users would typically get from an Apache 2.0 license:
@@ -60,22 +58,26 @@
 1  1.006849  0.695056  0.027386
 2  0.839067 -0.194327 -0.641318
 3 -0.955104 -0.384175  0.462385
 4 -0.197083  2.520539 -0.835229
 """
 ```
 
-## To install and test locally
+## To install, test locally and develop
 1. Create and activate a python virtual env
-1. `pip install -e .`
+1. `pip install -e ".[dev]"`
+1. `pytest`
+1. `pre-commit install`
+
 
 ## To install anywhere else
 1. Create and activate a python virtual env
 1. `python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple non-parametric-multivariate-data-generator`
 
 ## To deploy to pypi
 1. Create and activate a python virtual env
 1. `python3 -m pip install --upgrade pip`
 1. `python3 -m pip install --upgrade build`
 1. `python3 -m pip install --upgrade twine`
+1. Change project version property in `pyproject.toml`
 1. `python3 -m build`
 1. `python3 -m twine upload --repository testpypi dist/*`
```

### Comparing `non-parametric-multivariate-data-generator-0.0.2/pyproject.toml` & `non-parametric-multivariate-data-generator-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "non-parametric-multivariate-data-generator"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Juan P. Restrepo", email="jurest82@eafit.edu.co" },
   { name="Pablo Osorio", email="osoriopabl@gmail.com" },
 ]
 description = "A small example package"
 readme = "../README.md"
 requires-python = ">=3.9"
@@ -21,18 +21,16 @@
   "pandas>=1.3.5", "matplotlib>=3.2.2", "numpy>=1.21.6"
 ]
 
 [project.optional-dependencies]
 dev = [
     "jupyterlab>=3.2.1",
     "openpyxl==3.0.10",
-    "pre-commit>=3.11",
+    "pre-commit>=3.3",
     "pytest>=7.0",
-    "scikit-learn==1.0.2",
-    "scipy==1.7.3",
     "seaborn==0.11.2",
     "twine>=4.0.2",
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/jurest82/SyntheticDataCopulas"
```

### Comparing `non-parametric-multivariate-data-generator-0.0.2/src/non_parametric/empirical_cumulative_distribution.py` & `non-parametric-multivariate-data-generator-0.0.3/src/non_parametric/empirical_cumulative_distribution.py`

 * *Files identical despite different names*

### Comparing `non-parametric-multivariate-data-generator-0.0.2/src/non_parametric/frequency_table.py` & `non-parametric-multivariate-data-generator-0.0.3/src/non_parametric/frequency_table.py`

 * *Files identical despite different names*

### Comparing `non-parametric-multivariate-data-generator-0.0.2/src/non_parametric/synthetic_data_generator.py` & `non-parametric-multivariate-data-generator-0.0.3/src/non_parametric/synthetic_data_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from .frequency_table import frequency_table
 
 
 def generate_multivariate_data(X: pd.DataFrame, bins: int = 10, N: int = 1000):
     """This function generates new multivariate data respecting the dependency
     structures between variables.
 
-    Read the article Restrepo, Juan. P.; Rivera, J.C.; Laniado, H., Osorio, P; Becerra, O.
-    Nonparametric Generation of Synthetic Data Using Copulas. Electronics 2022, 1, 0. https://doi.org/
+    Read the article Restrepo, J.P.; Rivera, J.C.; Laniado, H.; Osorio,
+    P.; Becerra, O.A. 
+    Nonparametric Generation of Synthetic Data Using Copulas. 
+    Electronics 2023, 12, 1601. https://doi.org/10.3390/electronics12071601
     if you have any questions.
 
     -----------
     Parameters:
     X
       It is the original dataset
     bins
```

### Comparing `non-parametric-multivariate-data-generator-0.0.2/src/non_parametric_multivariate_data_generator.egg-info/PKG-INFO` & `non-parametric-multivariate-data-generator-0.0.3/src/non_parametric_multivariate_data_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: non-parametric-multivariate-data-generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: "Juan P. Restrepo" <jurest82@eafit.edu.co>, Pablo Osorio <osoriopabl@gmail.com>
 License: License text copyright © 2017 MariaDB Corporation Ab, All Rights Reserved.
         “Business Source License” is a trademark of MariaDB Corporation Ab.
         
         Licensed Work:        Non-parametric-multivariate-data-generator
```

### Comparing `non-parametric-multivariate-data-generator-0.0.2/src/non_parametric_multivariate_data_generator.egg-info/SOURCES.txt` & `non-parametric-multivariate-data-generator-0.0.3/src/non_parametric_multivariate_data_generator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,9 @@
 src/non_parametric/frequency_table.py
 src/non_parametric/plot_comparision.py
 src/non_parametric/synthetic_data_generator.py
 src/non_parametric_multivariate_data_generator.egg-info/PKG-INFO
 src/non_parametric_multivariate_data_generator.egg-info/SOURCES.txt
 src/non_parametric_multivariate_data_generator.egg-info/dependency_links.txt
 src/non_parametric_multivariate_data_generator.egg-info/requires.txt
-src/non_parametric_multivariate_data_generator.egg-info/top_level.txt
+src/non_parametric_multivariate_data_generator.egg-info/top_level.txt
+tests/test_shapes.py
```

