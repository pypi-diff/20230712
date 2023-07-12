# Comparing `tmp/botocore-a-la-carte-lightsail-1.31.1.tar.gz` & `tmp/botocore-a-la-carte-lightsail-1.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-lightsail-1.31.1.tar", last modified: Sat Jul  8 01:42:31 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-lightsail-1.31.2.tar", last modified: Wed Jul 12 01:44:45 2023, max compression
```

## Comparing `botocore-a-la-carte-lightsail-1.31.1.tar` & `botocore-a-la-carte-lightsail-1.31.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:31.294949 botocore-a-la-carte-lightsail-1.31.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-08 01:42:31.000000 botocore-a-la-carte-lightsail-1.31.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-08 01:42:31.294949 botocore-a-la-carte-lightsail-1.31.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:31.294949 botocore-a-la-carte-lightsail-1.31.1/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:31.294949 botocore-a-la-carte-lightsail-1.31.1/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:31.294949 botocore-a-la-carte-lightsail-1.31.1/botocore/data/lightsail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:31.294949 botocore-a-la-carte-lightsail-1.31.1/botocore/data/lightsail/2016-11-28/
--rw-r--r--   0 runner    (1001) docker     (123)    17636 2023-07-08 01:41:59.000000 botocore-a-la-carte-lightsail-1.31.1/botocore/data/lightsail/2016-11-28/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 01:41:59.000000 botocore-a-la-carte-lightsail-1.31.1/botocore/data/lightsail/2016-11-28/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-08 01:41:59.000000 botocore-a-la-carte-lightsail-1.31.1/botocore/data/lightsail/2016-11-28/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   653497 2023-07-08 01:41:59.000000 botocore-a-la-carte-lightsail-1.31.1/botocore/data/lightsail/2016-11-28/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:31.294949 botocore-a-la-carte-lightsail-1.31.1/botocore_a_la_carte_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-08 01:42:31.000000 botocore-a-la-carte-lightsail-1.31.1/botocore_a_la_carte_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-08 01:42:31.000000 botocore-a-la-carte-lightsail-1.31.1/botocore_a_la_carte_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:42:31.000000 botocore-a-la-carte-lightsail-1.31.1/botocore_a_la_carte_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 01:42:31.000000 botocore-a-la-carte-lightsail-1.31.1/botocore_a_la_carte_lightsail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:42:31.294949 botocore-a-la-carte-lightsail-1.31.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 01:42:31.000000 botocore-a-la-carte-lightsail-1.31.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:45.627345 botocore-a-la-carte-lightsail-1.31.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-12 01:44:45.000000 botocore-a-la-carte-lightsail-1.31.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-12 01:44:45.627345 botocore-a-la-carte-lightsail-1.31.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:45.623345 botocore-a-la-carte-lightsail-1.31.2/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:45.623345 botocore-a-la-carte-lightsail-1.31.2/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:45.623345 botocore-a-la-carte-lightsail-1.31.2/botocore/data/lightsail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:45.623345 botocore-a-la-carte-lightsail-1.31.2/botocore/data/lightsail/2016-11-28/
+-rw-r--r--   0 runner    (1001) docker     (123)    17636 2023-07-12 01:44:12.000000 botocore-a-la-carte-lightsail-1.31.2/botocore/data/lightsail/2016-11-28/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 01:44:12.000000 botocore-a-la-carte-lightsail-1.31.2/botocore/data/lightsail/2016-11-28/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-12 01:44:12.000000 botocore-a-la-carte-lightsail-1.31.2/botocore/data/lightsail/2016-11-28/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   653497 2023-07-12 01:44:12.000000 botocore-a-la-carte-lightsail-1.31.2/botocore/data/lightsail/2016-11-28/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:45.627345 botocore-a-la-carte-lightsail-1.31.2/botocore_a_la_carte_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-12 01:44:45.000000 botocore-a-la-carte-lightsail-1.31.2/botocore_a_la_carte_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-12 01:44:45.000000 botocore-a-la-carte-lightsail-1.31.2/botocore_a_la_carte_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:44:45.000000 botocore-a-la-carte-lightsail-1.31.2/botocore_a_la_carte_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 01:44:45.000000 botocore-a-la-carte-lightsail-1.31.2/botocore_a_la_carte_lightsail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:44:45.627345 botocore-a-la-carte-lightsail-1.31.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-12 01:44:45.000000 botocore-a-la-carte-lightsail-1.31.2/setup.py
```

### Comparing `botocore-a-la-carte-lightsail-1.31.1/LICENSE.txt` & `botocore-a-la-carte-lightsail-1.31.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lightsail-1.31.1/PKG-INFO` & `botocore-a-la-carte-lightsail-1.31.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lightsail
-Version: 1.31.1
+Version: 1.31.2
 Summary: lightsail data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lightsail-1.31.1/botocore/data/lightsail/2016-11-28/endpoint-rule-set-1.json` & `botocore-a-la-carte-lightsail-1.31.2/botocore/data/lightsail/2016-11-28/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lightsail-1.31.1/botocore/data/lightsail/2016-11-28/paginators-1.json` & `botocore-a-la-carte-lightsail-1.31.2/botocore/data/lightsail/2016-11-28/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lightsail-1.31.1/botocore/data/lightsail/2016-11-28/service-2.json` & `botocore-a-la-carte-lightsail-1.31.2/botocore/data/lightsail/2016-11-28/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lightsail-1.31.1/botocore_a_la_carte_lightsail.egg-info/PKG-INFO` & `botocore-a-la-carte-lightsail-1.31.2/botocore_a_la_carte_lightsail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lightsail
-Version: 1.31.1
+Version: 1.31.2
 Summary: lightsail data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lightsail-1.31.1/setup.py` & `botocore-a-la-carte-lightsail-1.31.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-lightsail',
-    version="1.31.1",
+    version="1.31.2",
     description='lightsail data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/lightsail/*/*.json'],
```

