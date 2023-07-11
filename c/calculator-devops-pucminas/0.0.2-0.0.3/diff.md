# Comparing `tmp/calculator_devops_pucminas-0.0.2.tar.gz` & `tmp/calculator_devops_pucminas-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculator_devops_pucminas-0.0.2.tar", last modified: Tue Jul 11 22:25:55 2023, max compression
+gzip compressed data, was "calculator_devops_pucminas-0.0.3.tar", last modified: Tue Jul 11 23:18:07 2023, max compression
```

## Comparing `calculator_devops_pucminas-0.0.2.tar` & `calculator_devops_pucminas-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:25:55.479011 calculator_devops_pucminas-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 22:25:42.000000 calculator_devops_pucminas-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-11 22:25:55.479011 calculator_devops_pucminas-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 22:25:42.000000 calculator_devops_pucminas-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-11 22:25:42.000000 calculator_devops_pucminas-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 22:25:42.000000 calculator_devops_pucminas-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:25:55.479011 calculator_devops_pucminas-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:25:55.479011 calculator_devops_pucminas-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:25:55.479011 calculator_devops_pucminas-0.0.2/src/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:25:42.000000 calculator_devops_pucminas-0.0.2/src/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-11 22:25:42.000000 calculator_devops_pucminas-0.0.2/src/calculator/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:25:55.479011 calculator_devops_pucminas-0.0.2/src/calculator_devops_pucminas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-11 22:25:55.000000 calculator_devops_pucminas-0.0.2/src/calculator_devops_pucminas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-11 22:25:55.000000 calculator_devops_pucminas-0.0.2/src/calculator_devops_pucminas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:25:55.000000 calculator_devops_pucminas-0.0.2/src/calculator_devops_pucminas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 22:25:55.000000 calculator_devops_pucminas-0.0.2/src/calculator_devops_pucminas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 22:25:55.000000 calculator_devops_pucminas-0.0.2/src/calculator_devops_pucminas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:25:55.479011 calculator_devops_pucminas-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-11 22:25:42.000000 calculator_devops_pucminas-0.0.2/test/test_stringstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:18:07.807732 calculator_devops_pucminas-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 23:17:57.000000 calculator_devops_pucminas-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-11 23:18:07.807732 calculator_devops_pucminas-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 23:17:57.000000 calculator_devops_pucminas-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-11 23:17:57.000000 calculator_devops_pucminas-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 23:17:57.000000 calculator_devops_pucminas-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 23:18:07.807732 calculator_devops_pucminas-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:18:07.803732 calculator_devops_pucminas-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:18:07.807732 calculator_devops_pucminas-0.0.3/src/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 23:17:57.000000 calculator_devops_pucminas-0.0.3/src/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-11 23:17:57.000000 calculator_devops_pucminas-0.0.3/src/calculator/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:18:07.807732 calculator_devops_pucminas-0.0.3/src/calculator_devops_pucminas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-11 23:18:07.000000 calculator_devops_pucminas-0.0.3/src/calculator_devops_pucminas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-11 23:18:07.000000 calculator_devops_pucminas-0.0.3/src/calculator_devops_pucminas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 23:18:07.000000 calculator_devops_pucminas-0.0.3/src/calculator_devops_pucminas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 23:18:07.000000 calculator_devops_pucminas-0.0.3/src/calculator_devops_pucminas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 23:18:07.000000 calculator_devops_pucminas-0.0.3/src/calculator_devops_pucminas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:18:07.807732 calculator_devops_pucminas-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-11 23:17:57.000000 calculator_devops_pucminas-0.0.3/test/test_stringstd.py
```

### Comparing `calculator_devops_pucminas-0.0.2/LICENSE` & `calculator_devops_pucminas-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calculator_devops_pucminas-0.0.2/PKG-INFO` & `calculator_devops_pucminas-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calculator_devops_pucminas
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python calculator software
 Author-email: Sylvio Rubens <srjneto@hotmail.com>
 Project-URL: Homepage, https://github.com/SylvioRubens/devops_project
 Project-URL: Bug Tracker, https://github.com/SylvioRubens/devops_project/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `calculator_devops_pucminas-0.0.2/pyproject.toml` & `calculator_devops_pucminas-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calculator_devops_pucminas"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name="Sylvio Rubens", email="srjneto@hotmail.com"},
 ]
 description = "Python calculator software"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `calculator_devops_pucminas-0.0.2/src/calculator/calculator.py` & `calculator_devops_pucminas-0.0.3/src/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `calculator_devops_pucminas-0.0.2/src/calculator_devops_pucminas.egg-info/PKG-INFO` & `calculator_devops_pucminas-0.0.3/src/calculator_devops_pucminas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calculator-devops-pucminas
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python calculator software
 Author-email: Sylvio Rubens <srjneto@hotmail.com>
 Project-URL: Homepage, https://github.com/SylvioRubens/devops_project
 Project-URL: Bug Tracker, https://github.com/SylvioRubens/devops_project/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `calculator_devops_pucminas-0.0.2/test/test_stringstd.py` & `calculator_devops_pucminas-0.0.3/test/test_stringstd.py`

 * *Files identical despite different names*

