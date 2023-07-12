# Comparing `tmp/getSequence-1.51.tar.gz` & `tmp/getSequence-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getSequence-1.51.tar", last modified: Tue Jun 20 15:21:00 2023, max compression
+gzip compressed data, was "getSequence-1.6.tar", last modified: Wed Jul 12 17:33:24 2023, max compression
```

## Comparing `getSequence-1.51.tar` & `getSequence-1.6.tar`

### file list

```diff
@@ -1,59 +1,56 @@
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.160869 getSequence-1.51/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      257 2022-02-07 14:17:58.000000 getSequence-1.51/.codecov.yml
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.155893 getSequence-1.51/.github/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2257 2022-02-07 14:17:58.000000 getSequence-1.51/.github/CONTRIBUTING.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      224 2022-02-07 14:17:58.000000 getSequence-1.51/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156033 getSequence-1.51/.github/workflows/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2049 2022-03-09 18:03:44.000000 getSequence-1.51/.github/workflows/CI.yaml
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1403 2023-06-14 13:39:19.000000 getSequence-1.51/.gitignore
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      328 2022-02-07 14:17:58.000000 getSequence-1.51/.lgtm.yml
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3556 2022-02-07 14:17:58.000000 getSequence-1.51/CODE_OF_CONDUCT.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1072 2022-02-07 14:17:58.000000 getSequence-1.51/LICENSE
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      145 2022-02-07 14:17:58.000000 getSequence-1.51/MANIFEST.in
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6036 2023-06-20 15:21:00.160929 getSequence-1.51/PKG-INFO
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5724 2022-07-08 16:41:31.000000 getSequence-1.51/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156276 getSequence-1.51/devtools/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3518 2022-02-07 14:17:58.000000 getSequence-1.51/devtools/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156402 getSequence-1.51/devtools/conda-envs/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      208 2022-02-07 14:17:58.000000 getSequence-1.51/devtools/conda-envs/test_env.yaml
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156553 getSequence-1.51/devtools/legacy-miniconda-setup/
--rwxr-xr-x   0 ryanemenecker   (501) staff       (20)     1344 2022-02-07 14:17:58.000000 getSequence-1.51/devtools/legacy-miniconda-setup/before_install.sh
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156698 getSequence-1.51/devtools/scripts/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3860 2022-02-07 14:17:58.000000 getSequence-1.51/devtools/scripts/create_conda_env.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.157582 getSequence-1.51/docs/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      608 2022-02-07 14:17:58.000000 getSequence-1.51/docs/Makefile
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      590 2022-02-07 14:17:58.000000 getSequence-1.51/docs/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.157738 getSequence-1.51/docs/_static/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      507 2022-02-07 14:17:58.000000 getSequence-1.51/docs/_static/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.157881 getSequence-1.51/docs/_templates/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      470 2022-02-07 14:17:58.000000 getSequence-1.51/docs/_templates/README.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5343 2022-02-07 14:17:58.000000 getSequence-1.51/docs/conf.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1472 2022-03-09 18:25:45.000000 getSequence-1.51/docs/getting_started.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      536 2022-03-09 18:03:00.000000 getSequence-1.51/docs/index.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      779 2022-02-07 14:17:58.000000 getSequence-1.51/docs/make.bat
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.158184 getSequence-1.51/docs/usage/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3433 2022-03-09 17:56:01.000000 getSequence-1.51/docs/usage/command-line.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1620 2022-03-09 17:55:47.000000 getSequence-1.51/docs/usage/using-in-python.rst
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.161283 getSequence-1.51/getSequence/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      306 2022-03-09 17:44:54.000000 getSequence-1.51/getSequence/__init__.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      497 2023-06-20 15:21:00.161314 getSequence-1.51/getSequence/_version.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)   523968 2023-06-20 15:18:03.000000 getSequence-1.51/getSequence/get_sequence.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1681 2023-06-20 15:18:01.000000 getSequence-1.51/getSequence/getseq.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       47 2022-03-09 16:51:05.000000 getSequence-1.51/getSequence/getsequence_exceptions.py
--rw-------   0 ryanemenecker   (501) staff       (20)  1154428 2022-11-22 16:52:54.000000 getSequence-1.51/getSequence/screenshot.png
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.160565 getSequence-1.51/getSequence/tests/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      113 2022-02-07 14:17:58.000000 getSequence-1.51/getSequence/tests/__init__.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      319 2022-02-07 14:17:58.000000 getSequence-1.51/getSequence/tests/test_getSequence.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     4366 2023-06-14 13:39:26.000000 getSequence-1.51/getSequence/vis_sequence.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.160326 getSequence-1.51/getSequence.egg-info/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6036 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/PKG-INFO
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1005 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/SOURCES.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)        1 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/dependency_links.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       17 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/requires.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       12 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/top_level.txt
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.160784 getSequence-1.51/scripts/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1460 2022-07-08 16:37:31.000000 getSequence-1.51/scripts/getseq
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1342 2022-11-22 20:02:42.000000 getSequence-1.51/scripts/visseq
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      360 2023-06-20 15:21:00.161157 getSequence-1.51/setup.cfg
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2299 2022-11-22 19:56:28.000000 getSequence-1.51/setup.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    68611 2022-02-07 14:17:58.000000 getSequence-1.51/versioneer.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.537137 getSequence-1.6/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      257 2022-02-07 14:17:58.000000 getSequence-1.6/.codecov.yml
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.532534 getSequence-1.6/.github/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2257 2022-02-07 14:17:58.000000 getSequence-1.6/.github/CONTRIBUTING.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      224 2022-02-07 14:17:58.000000 getSequence-1.6/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.532680 getSequence-1.6/.github/workflows/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2049 2022-03-09 18:03:44.000000 getSequence-1.6/.github/workflows/CI.yaml
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1403 2023-06-14 13:39:19.000000 getSequence-1.6/.gitignore
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      328 2022-02-07 14:17:58.000000 getSequence-1.6/.lgtm.yml
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3556 2022-02-07 14:17:58.000000 getSequence-1.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1072 2022-02-07 14:17:58.000000 getSequence-1.6/LICENSE
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      145 2022-02-07 14:17:58.000000 getSequence-1.6/MANIFEST.in
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5996 2023-07-12 17:33:24.537195 getSequence-1.6/PKG-INFO
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5724 2022-07-08 16:41:31.000000 getSequence-1.6/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.532928 getSequence-1.6/devtools/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3518 2022-02-07 14:17:58.000000 getSequence-1.6/devtools/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.533083 getSequence-1.6/devtools/conda-envs/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      208 2022-02-07 14:17:58.000000 getSequence-1.6/devtools/conda-envs/test_env.yaml
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.533232 getSequence-1.6/devtools/legacy-miniconda-setup/
+-rwxr-xr-x   0 ryanemenecker   (501) staff       (20)     1344 2022-02-07 14:17:58.000000 getSequence-1.6/devtools/legacy-miniconda-setup/before_install.sh
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.533383 getSequence-1.6/devtools/scripts/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3860 2022-02-07 14:17:58.000000 getSequence-1.6/devtools/scripts/create_conda_env.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.534416 getSequence-1.6/docs/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      608 2022-02-07 14:17:58.000000 getSequence-1.6/docs/Makefile
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      590 2022-02-07 14:17:58.000000 getSequence-1.6/docs/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.534577 getSequence-1.6/docs/_static/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      507 2022-02-07 14:17:58.000000 getSequence-1.6/docs/_static/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.534726 getSequence-1.6/docs/_templates/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      470 2022-02-07 14:17:58.000000 getSequence-1.6/docs/_templates/README.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5343 2022-02-07 14:17:58.000000 getSequence-1.6/docs/conf.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1472 2022-03-09 18:25:45.000000 getSequence-1.6/docs/getting_started.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      536 2022-03-09 18:03:00.000000 getSequence-1.6/docs/index.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      779 2022-02-07 14:17:58.000000 getSequence-1.6/docs/make.bat
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.535079 getSequence-1.6/docs/usage/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3433 2022-03-09 17:56:01.000000 getSequence-1.6/docs/usage/command-line.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1620 2022-03-09 17:55:47.000000 getSequence-1.6/docs/usage/using-in-python.rst
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.537553 getSequence-1.6/getSequence/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      306 2022-03-09 17:44:54.000000 getSequence-1.6/getSequence/__init__.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      496 2023-07-12 17:33:24.537583 getSequence-1.6/getSequence/_version.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)   523969 2023-07-12 17:31:11.000000 getSequence-1.6/getSequence/get_sequence.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1042 2023-07-12 17:31:23.000000 getSequence-1.6/getSequence/getseq.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       47 2023-07-12 17:31:24.000000 getSequence-1.6/getSequence/getsequence_exceptions.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.536899 getSequence-1.6/getSequence/tests/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      113 2022-02-07 14:17:58.000000 getSequence-1.6/getSequence/tests/__init__.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      319 2022-02-07 14:17:58.000000 getSequence-1.6/getSequence/tests/test_getSequence.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.536646 getSequence-1.6/getSequence.egg-info/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5996 2023-07-12 17:33:24.000000 getSequence-1.6/getSequence.egg-info/PKG-INFO
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      935 2023-07-12 17:33:24.000000 getSequence-1.6/getSequence.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)        1 2023-07-12 17:33:24.000000 getSequence-1.6/getSequence.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       17 2023-07-12 17:33:24.000000 getSequence-1.6/getSequence.egg-info/requires.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       12 2023-07-12 17:33:24.000000 getSequence-1.6/getSequence.egg-info/top_level.txt
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-07-12 17:33:24.537033 getSequence-1.6/scripts/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1460 2022-07-08 16:37:31.000000 getSequence-1.6/scripts/getseq
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      360 2023-07-12 17:33:24.537444 getSequence-1.6/setup.cfg
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2269 2023-07-12 17:29:05.000000 getSequence-1.6/setup.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    68611 2022-02-07 14:17:58.000000 getSequence-1.6/versioneer.py
```

### Comparing `getSequence-1.51/.github/CONTRIBUTING.md` & `getSequence-1.6/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/.github/workflows/CI.yaml` & `getSequence-1.6/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/.gitignore` & `getSequence-1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/CODE_OF_CONDUCT.md` & `getSequence-1.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/LICENSE` & `getSequence-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/PKG-INFO` & `getSequence-1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: getSequence
-Version: 1.51
+Version: 1.6
 Summary: A CLI to get a uniprot sequence returned to terminal
-Home-page: UNKNOWN
 Author: Ryan Emenecker
 Author-email: remenecker@wustl.edu
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 getSequence
 ==============================
 
@@ -128,9 +126,7 @@
 Copyright (c) 2022, Ryan Emenecker
 
 
 #### Acknowledgements
  
 Project based on the 
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.6.
-
-
```

### Comparing `getSequence-1.51/README.md` & `getSequence-1.6/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/devtools/README.md` & `getSequence-1.6/devtools/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/devtools/legacy-miniconda-setup/before_install.sh` & `getSequence-1.6/devtools/legacy-miniconda-setup/before_install.sh`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/devtools/scripts/create_conda_env.py` & `getSequence-1.6/devtools/scripts/create_conda_env.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/docs/Makefile` & `getSequence-1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/docs/README.md` & `getSequence-1.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/docs/conf.py` & `getSequence-1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/docs/getting_started.rst` & `getSequence-1.6/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/docs/index.rst` & `getSequence-1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/docs/make.bat` & `getSequence-1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/docs/usage/command-line.rst` & `getSequence-1.6/docs/usage/command-line.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/docs/usage/using-in-python.rst` & `getSequence-1.6/docs/usage/using-in-python.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/getSequence/get_sequence.py` & `getSequence-1.6/getSequence/get_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,11 +177,11 @@
         split_by_lines = seq_to_use.split('\n')
         header = split_by_lines[0].lower()
         for chars in split_by_lines[1:]:
             temp_seq+=chars
         final_vals = [header, temp_seq]
         return final_vals
 
-    # if we have still failed... well eff.
+    # if we have still failed... well darn.
     raise Exception('Unable to find sequence.')
```

### Comparing `getSequence-1.51/getSequence.egg-info/PKG-INFO` & `getSequence-1.6/getSequence.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: getSequence
-Version: 1.51
+Version: 1.6
 Summary: A CLI to get a uniprot sequence returned to terminal
-Home-page: UNKNOWN
 Author: Ryan Emenecker
 Author-email: remenecker@wustl.edu
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 getSequence
 ==============================
 
@@ -128,9 +126,7 @@
 Copyright (c) 2022, Ryan Emenecker
 
 
 #### Acknowledgements
  
 Project based on the 
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.6.
-
-
```

### Comparing `getSequence-1.51/getSequence.egg-info/SOURCES.txt` & `getSequence-1.6/getSequence.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,15 @@
 docs/usage/command-line.rst
 docs/usage/using-in-python.rst
 getSequence/__init__.py
 getSequence/_version.py
 getSequence/get_sequence.py
 getSequence/getseq.py
 getSequence/getsequence_exceptions.py
-getSequence/screenshot.png
-getSequence/vis_sequence.py
 getSequence.egg-info/PKG-INFO
 getSequence.egg-info/SOURCES.txt
 getSequence.egg-info/dependency_links.txt
 getSequence.egg-info/requires.txt
 getSequence.egg-info/top_level.txt
 getSequence/tests/__init__.py
 getSequence/tests/test_getSequence.py
-scripts/getseq
-scripts/visseq
+scripts/getseq
```

### Comparing `getSequence-1.51/scripts/getseq` & `getSequence-1.6/scripts/getseq`

 * *Files identical despite different names*

### Comparing `getSequence-1.51/setup.py` & `getSequence-1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     # Optional include package data to ship with your package
     # Customize MANIFEST.in if the general case does not suit your needs
     # Comment out this line to prevent the files from being packaged with your software
     include_package_data=True,
 
     # Allows `setup.py test` to work correctly with pytest
     setup_requires=[] + pytest_runner,
-    scripts=['scripts/getseq',
-            'scripts/visseq'],
+    scripts=['scripts/getseq'],
 
     # Additional entries you may want simply uncomment the lines you want and fill in the data
     # url='http://www.my_package.com',  # Website
     install_requires=['urllib3',
                     'requests'],              # Required packages, pulls from pip if needed; do not use for Conda deployment
     # platforms=['Linux',
     #            'Mac OS-X',
```

### Comparing `getSequence-1.51/versioneer.py` & `getSequence-1.6/versioneer.py`

 * *Files identical despite different names*

