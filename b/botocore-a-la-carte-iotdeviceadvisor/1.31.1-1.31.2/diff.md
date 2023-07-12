# Comparing `tmp/botocore-a-la-carte-iotdeviceadvisor-1.31.1.tar.gz` & `tmp/botocore-a-la-carte-iotdeviceadvisor-1.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-iotdeviceadvisor-1.31.1.tar", last modified: Sat Jul  8 01:42:21 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-iotdeviceadvisor-1.31.2.tar", last modified: Wed Jul 12 01:44:35 2023, max compression
```

## Comparing `botocore-a-la-carte-iotdeviceadvisor-1.31.1.tar` & `botocore-a-la-carte-iotdeviceadvisor-1.31.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:21.974653 botocore-a-la-carte-iotdeviceadvisor-1.31.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-08 01:42:21.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 01:42:21.974653 botocore-a-la-carte-iotdeviceadvisor-1.31.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:21.974653 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:21.974653 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:21.974653 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/data/iotdeviceadvisor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:21.974653 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/data/iotdeviceadvisor/2020-09-18/
--rw-r--r--   0 runner    (1001) docker     (123)    17680 2023-07-08 01:41:59.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/data/iotdeviceadvisor/2020-09-18/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 01:41:59.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/data/iotdeviceadvisor/2020-09-18/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 01:41:59.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/data/iotdeviceadvisor/2020-09-18/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    44174 2023-07-08 01:41:59.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/data/iotdeviceadvisor/2020-09-18/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:21.974653 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore_a_la_carte_iotdeviceadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 01:42:21.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore_a_la_carte_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-08 01:42:21.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore_a_la_carte_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:42:21.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore_a_la_carte_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 01:42:21.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore_a_la_carte_iotdeviceadvisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:42:21.974653 botocore-a-la-carte-iotdeviceadvisor-1.31.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-08 01:42:21.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:35.847241 botocore-a-la-carte-iotdeviceadvisor-1.31.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-12 01:44:35.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-12 01:44:35.847241 botocore-a-la-carte-iotdeviceadvisor-1.31.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:35.847241 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:35.847241 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:35.847241 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/data/iotdeviceadvisor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:35.847241 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/data/iotdeviceadvisor/2020-09-18/
+-rw-r--r--   0 runner    (1001) docker     (123)    17680 2023-07-12 01:44:12.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/data/iotdeviceadvisor/2020-09-18/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 01:44:12.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/data/iotdeviceadvisor/2020-09-18/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 01:44:12.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/data/iotdeviceadvisor/2020-09-18/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44174 2023-07-12 01:44:12.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/data/iotdeviceadvisor/2020-09-18/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:35.847241 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore_a_la_carte_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-12 01:44:35.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore_a_la_carte_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-12 01:44:35.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore_a_la_carte_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:44:35.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore_a_la_carte_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 01:44:35.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore_a_la_carte_iotdeviceadvisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:44:35.847241 botocore-a-la-carte-iotdeviceadvisor-1.31.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-12 01:44:35.000000 botocore-a-la-carte-iotdeviceadvisor-1.31.2/setup.py
```

### Comparing `botocore-a-la-carte-iotdeviceadvisor-1.31.1/LICENSE.txt` & `botocore-a-la-carte-iotdeviceadvisor-1.31.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotdeviceadvisor-1.31.1/PKG-INFO` & `botocore-a-la-carte-iotdeviceadvisor-1.31.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotdeviceadvisor
-Version: 1.31.1
+Version: 1.31.2
 Summary: iotdeviceadvisor data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/data/iotdeviceadvisor/2020-09-18/endpoint-rule-set-1.json` & `botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/data/iotdeviceadvisor/2020-09-18/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore/data/iotdeviceadvisor/2020-09-18/service-2.json` & `botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore/data/iotdeviceadvisor/2020-09-18/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotdeviceadvisor-1.31.1/botocore_a_la_carte_iotdeviceadvisor.egg-info/PKG-INFO` & `botocore-a-la-carte-iotdeviceadvisor-1.31.2/botocore_a_la_carte_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotdeviceadvisor
-Version: 1.31.1
+Version: 1.31.2
 Summary: iotdeviceadvisor data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotdeviceadvisor-1.31.1/setup.py` & `botocore-a-la-carte-iotdeviceadvisor-1.31.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-iotdeviceadvisor',
-    version="1.31.1",
+    version="1.31.2",
     description='iotdeviceadvisor data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/iotdeviceadvisor/*/*.json'],
```
