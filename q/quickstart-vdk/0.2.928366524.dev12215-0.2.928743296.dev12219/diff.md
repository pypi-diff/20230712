# Comparing `tmp/quickstart-vdk-0.2.928366524.dev12215.tar.gz` & `tmp/quickstart-vdk-0.2.928743296.dev12219.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.928366524.dev12215.tar", last modified: Wed Jul 12 04:31:09 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.928743296.dev12219.tar", last modified: Wed Jul 12 10:48:26 2023, max compression
```

## Comparing `quickstart-vdk-0.2.928366524.dev12215.tar` & `quickstart-vdk-0.2.928743296.dev12219.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 04:31:09.214179 quickstart-vdk-0.2.928366524.dev12215/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-07-12 04:31:09.214179 quickstart-vdk-0.2.928366524.dev12215/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-12 04:28:16.000000 quickstart-vdk-0.2.928366524.dev12215/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 04:31:09.214179 quickstart-vdk-0.2.928366524.dev12215/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-07-12 04:31:09.000000 quickstart-vdk-0.2.928366524.dev12215/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-12 04:31:09.000000 quickstart-vdk-0.2.928366524.dev12215/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 04:31:09.000000 quickstart-vdk-0.2.928366524.dev12215/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-12 04:31:09.000000 quickstart-vdk-0.2.928366524.dev12215/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-12 04:31:09.000000 quickstart-vdk-0.2.928366524.dev12215/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 04:31:09.214179 quickstart-vdk-0.2.928366524.dev12215/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-12 04:30:58.000000 quickstart-vdk-0.2.928366524.dev12215/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 04:31:09.214179 quickstart-vdk-0.2.928366524.dev12215/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-12 04:28:16.000000 quickstart-vdk-0.2.928366524.dev12215/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:48:26.603626 quickstart-vdk-0.2.928743296.dev12219/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-12 10:48:26.603626 quickstart-vdk-0.2.928743296.dev12219/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-12 10:48:12.000000 quickstart-vdk-0.2.928743296.dev12219/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:48:26.603626 quickstart-vdk-0.2.928743296.dev12219/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-12 10:48:26.000000 quickstart-vdk-0.2.928743296.dev12219/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-12 10:48:26.000000 quickstart-vdk-0.2.928743296.dev12219/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:48:26.000000 quickstart-vdk-0.2.928743296.dev12219/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-12 10:48:26.000000 quickstart-vdk-0.2.928743296.dev12219/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-12 10:48:26.000000 quickstart-vdk-0.2.928743296.dev12219/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:48:26.603626 quickstart-vdk-0.2.928743296.dev12219/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-12 10:48:16.000000 quickstart-vdk-0.2.928743296.dev12219/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:48:26.603626 quickstart-vdk-0.2.928743296.dev12219/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-12 10:48:12.000000 quickstart-vdk-0.2.928743296.dev12219/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.928366524.dev12215/PKG-INFO` & `quickstart-vdk-0.2.928743296.dev12219/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.928366524.dev12215
+Version: 0.2.928743296.dev12219
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.928366524.dev12215/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.928743296.dev12219/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.928366524.dev12215
+Version: 0.2.928743296.dev12219
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.928366524.dev12215/setup.py` & `quickstart-vdk-0.2.928743296.dev12219/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.928366524.dev12215"
+__version__ = "0.2.928743296.dev12219"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

