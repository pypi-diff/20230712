# Comparing `tmp/fedml_azure-2.0.1.dev0.tar.gz` & `tmp/fedml_azure-2.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedml_azure-2.0.1.dev0.tar", last modified: Tue Jul 11 21:18:53 2023, max compression
+gzip compressed data, was "fedml_azure-2.0.1.dev2.tar", last modified: Tue Jul 11 22:12:16 2023, max compression
```

## Comparing `fedml_azure-2.0.1.dev0.tar` & `fedml_azure-2.0.1.dev2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 21:18:53.995678 fedml_azure-2.0.1.dev0/
--rw-r--r--   0 I550585    (501) staff       (20)    11307 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/LICENSE.txt
--rw-r--r--   0 I550585    (501) staff       (20)      349 2023-07-11 21:18:53.995155 fedml_azure-2.0.1.dev0/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      103 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/pyproject.toml
--rw-r--r--   0 I550585    (501) staff       (20)       38 2023-07-11 21:18:53.995812 fedml_azure-2.0.1.dev0/setup.cfg
--rw-r--r--   0 I550585    (501) staff       (20)      757 2023-07-11 21:17:15.000000 fedml_azure-2.0.1.dev0/setup.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 21:18:53.973683 fedml_azure-2.0.1.dev0/src/
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 21:18:53.989743 fedml_azure-2.0.1.dev0/src/fedml_azure/
--rw-r--r--   0 I550585    (501) staff       (20)      182 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/__init__.py
--rw-r--r--   0 I550585    (501) staff       (20)    11107 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/compute_creation.py
--rw-r--r--   0 I550585    (501) staff       (20)    15864 2023-07-11 21:16:30.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/dbconnection.py
--rw-r--r--   0 I550585    (501) staff       (20)    16929 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/deployment.py
--rw-r--r--   0 I550585    (501) staff       (20)    14315 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/dwc_azureml.py
--rw-r--r--   0 I550585    (501) staff       (20)     4982 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/environment_creation.py
--rw-r--r--   0 I550585    (501) staff       (20)     1682 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/install_validate.sh
--rw-r--r--   0 I550585    (501) staff       (20)      380 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/internal_config.json
--rw-r--r--   0 I550585    (501) staff       (20)     7737 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/kyma_deploy.sh
--rw-r--r--   0 I550585    (501) staff       (20)     9867 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/kyma_deployment.py
--rw-r--r--   0 I550585    (501) staff       (20)      656 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/logger.py
--rw-r--r--   0 I550585    (501) staff       (20)     3112 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/resource_creation.py
--rw-r--r--   0 I550585    (501) staff       (20)     4949 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/script_generator.py
--rw-r--r--   0 I550585    (501) staff       (20)      652 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev0/src/fedml_azure/script_generator_helper.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 21:18:53.994253 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/
--rw-r--r--   0 I550585    (501) staff       (20)      349 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      707 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/SOURCES.txt
--rw-r--r--   0 I550585    (501) staff       (20)        1 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/dependency_links.txt
--rw-r--r--   0 I550585    (501) staff       (20)       19 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/requires.txt
--rw-r--r--   0 I550585    (501) staff       (20)       12 2023-07-11 21:18:53.000000 fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/top_level.txt
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 22:12:16.288956 fedml_azure-2.0.1.dev2/
+-rw-r--r--   0 I550585    (501) staff       (20)    11307 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/LICENSE.txt
+-rw-r--r--   0 I550585    (501) staff       (20)     1280 2023-07-11 22:12:16.288513 fedml_azure-2.0.1.dev2/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      890 2023-07-11 22:12:07.000000 fedml_azure-2.0.1.dev2/README.md
+-rw-r--r--   0 I550585    (501) staff       (20)      103 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/pyproject.toml
+-rw-r--r--   0 I550585    (501) staff       (20)       38 2023-07-11 22:12:16.289081 fedml_azure-2.0.1.dev2/setup.cfg
+-rw-r--r--   0 I550585    (501) staff       (20)      973 2023-07-11 22:11:50.000000 fedml_azure-2.0.1.dev2/setup.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 22:12:14.136155 fedml_azure-2.0.1.dev2/src/
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 22:12:16.281332 fedml_azure-2.0.1.dev2/src/fedml_azure/
+-rw-r--r--   0 I550585    (501) staff       (20)      182 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/__init__.py
+-rw-r--r--   0 I550585    (501) staff       (20)    11107 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/compute_creation.py
+-rw-r--r--   0 I550585    (501) staff       (20)    15864 2023-07-11 21:16:30.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/dbconnection.py
+-rw-r--r--   0 I550585    (501) staff       (20)    16929 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/deployment.py
+-rw-r--r--   0 I550585    (501) staff       (20)    14315 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/dwc_azureml.py
+-rw-r--r--   0 I550585    (501) staff       (20)     4982 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/environment_creation.py
+-rw-r--r--   0 I550585    (501) staff       (20)     1682 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/install_validate.sh
+-rw-r--r--   0 I550585    (501) staff       (20)      380 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/internal_config.json
+-rw-r--r--   0 I550585    (501) staff       (20)     7737 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/kyma_deploy.sh
+-rw-r--r--   0 I550585    (501) staff       (20)     9867 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/kyma_deployment.py
+-rw-r--r--   0 I550585    (501) staff       (20)      656 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/logger.py
+-rw-r--r--   0 I550585    (501) staff       (20)     3112 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/resource_creation.py
+-rw-r--r--   0 I550585    (501) staff       (20)     4949 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/script_generator.py
+-rw-r--r--   0 I550585    (501) staff       (20)      652 2023-07-11 21:14:08.000000 fedml_azure-2.0.1.dev2/src/fedml_azure/script_generator_helper.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-07-11 22:12:16.287753 fedml_azure-2.0.1.dev2/src/fedml_azure.egg-info/
+-rw-r--r--   0 I550585    (501) staff       (20)     1280 2023-07-11 22:12:14.000000 fedml_azure-2.0.1.dev2/src/fedml_azure.egg-info/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      717 2023-07-11 22:12:14.000000 fedml_azure-2.0.1.dev2/src/fedml_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 I550585    (501) staff       (20)        1 2023-07-11 22:12:14.000000 fedml_azure-2.0.1.dev2/src/fedml_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       19 2023-07-11 22:12:14.000000 fedml_azure-2.0.1.dev2/src/fedml_azure.egg-info/requires.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       12 2023-07-11 22:12:14.000000 fedml_azure-2.0.1.dev2/src/fedml_azure.egg-info/top_level.txt
```

### Comparing `fedml_azure-2.0.1.dev0/LICENSE.txt` & `fedml_azure-2.0.1.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/setup.py` & `fedml_azure-2.0.1.dev2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import setuptools
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="fedml_azure",
-    version="2.0.1.dev0",
+    version="2.0.1.dev2",
     author="SAP SE",
     description="A python library for building machine learning models on AzureML using a federated data source",
     license='Apache License 2.0',
     license_files = ['LICENSE.txt'],
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "hdbcli","ruamel.yaml"
     ],
```

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/compute_creation.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/compute_creation.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/dbconnection.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/dbconnection.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/deployment.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/deployment.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/dwc_azureml.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/dwc_azureml.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/environment_creation.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/environment_creation.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/install_validate.sh` & `fedml_azure-2.0.1.dev2/src/fedml_azure/install_validate.sh`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/kyma_deploy.sh` & `fedml_azure-2.0.1.dev2/src/fedml_azure/kyma_deploy.sh`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/kyma_deployment.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/kyma_deployment.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/logger.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/logger.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/resource_creation.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/resource_creation.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/script_generator.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/script_generator.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure/script_generator_helper.py` & `fedml_azure-2.0.1.dev2/src/fedml_azure/script_generator_helper.py`

 * *Files identical despite different names*

### Comparing `fedml_azure-2.0.1.dev0/src/fedml_azure.egg-info/SOURCES.txt` & `fedml_azure-2.0.1.dev2/src/fedml_azure.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.txt
+README.md
 pyproject.toml
 setup.py
 src/fedml_azure/__init__.py
 src/fedml_azure/compute_creation.py
 src/fedml_azure/dbconnection.py
 src/fedml_azure/deployment.py
 src/fedml_azure/dwc_azureml.py
```

