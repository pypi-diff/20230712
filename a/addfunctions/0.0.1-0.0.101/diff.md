# Comparing `tmp/addfunctions-0.0.1.tar.gz` & `tmp/addfunctions-0.0.101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addfunctions-0.0.1.tar", last modified: Wed Jul 12 11:48:54 2023, max compression
+gzip compressed data, was "addfunctions-0.0.101.tar", last modified: Wed Jul 12 11:58:17 2023, max compression
```

## Comparing `addfunctions-0.0.1.tar` & `addfunctions-0.0.101.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-12 11:48:54.867165 addfunctions-0.0.1/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-02-09 10:07:34.000000 addfunctions-0.0.1/LICENSE.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3898 2023-07-12 11:48:54.867165 addfunctions-0.0.1/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3314 2023-05-09 09:41:50.000000 addfunctions-0.0.1/README.md
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-12 11:48:54.867165 addfunctions-0.0.1/addfunctions.egg-info/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3898 2023-07-12 11:48:54.000000 addfunctions-0.0.1/addfunctions.egg-info/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      189 2023-07-12 11:48:54.000000 addfunctions-0.0.1/addfunctions.egg-info/SOURCES.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-07-12 11:48:54.000000 addfunctions-0.0.1/addfunctions.egg-info/dependency_links.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-07-12 11:48:54.000000 addfunctions-0.0.1/addfunctions.egg-info/top_level.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      549 2023-07-12 11:48:04.000000 addfunctions-0.0.1/pyproject.toml
--rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-07-12 11:48:54.867165 addfunctions-0.0.1/setup.cfg
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      660 2023-07-12 11:48:33.000000 addfunctions-0.0.1/setup.py
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-12 11:58:17.388798 addfunctions-0.0.101/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-02-09 10:07:34.000000 addfunctions-0.0.101/LICENSE.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      681 2023-07-12 11:58:17.388798 addfunctions-0.0.101/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)       95 2023-07-12 11:58:09.000000 addfunctions-0.0.101/README.md
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-12 11:58:17.388798 addfunctions-0.0.101/addfunctions.egg-info/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      681 2023-07-12 11:58:17.000000 addfunctions-0.0.101/addfunctions.egg-info/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      189 2023-07-12 11:58:17.000000 addfunctions-0.0.101/addfunctions.egg-info/SOURCES.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-07-12 11:58:17.000000 addfunctions-0.0.101/addfunctions.egg-info/dependency_links.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-07-12 11:58:17.000000 addfunctions-0.0.101/addfunctions.egg-info/top_level.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      551 2023-07-12 11:55:36.000000 addfunctions-0.0.101/pyproject.toml
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-07-12 11:58:17.388798 addfunctions-0.0.101/setup.cfg
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      662 2023-07-12 11:55:27.000000 addfunctions-0.0.101/setup.py
```

### Comparing `addfunctions-0.0.1/LICENSE.txt` & `addfunctions-0.0.101/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `addfunctions-0.0.1/pyproject.toml` & `addfunctions-0.0.101/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "addfunctions"
-version = "0.0.1"
+version = "0.0.101"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Additional functions for python scripts"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `addfunctions-0.0.1/setup.py` & `addfunctions-0.0.101/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "addfunctions",
-    version = "0.0.1",
+    version = "0.0.101",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
     description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/addfunctions",
     packages=setuptools.find_packages(),
```

