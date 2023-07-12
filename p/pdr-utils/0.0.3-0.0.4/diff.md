# Comparing `tmp/pdr-utils-0.0.3.tar.gz` & `tmp/pdr-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdr-utils-0.0.3.tar", last modified: Mon Jul 10 14:16:29 2023, max compression
+gzip compressed data, was "pdr-utils-0.0.4.tar", last modified: Wed Jul 12 13:09:37 2023, max compression
```

## Comparing `pdr-utils-0.0.3.tar` & `pdr-utils-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:16:29.191584 pdr-utils-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 14:16:19.000000 pdr-utils-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-10 14:16:29.191584 pdr-utils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 14:16:19.000000 pdr-utils-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:16:29.191584 pdr-utils-0.0.3/pdr_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-10 14:16:29.000000 pdr-utils-0.0.3/pdr_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-10 14:16:29.000000 pdr-utils-0.0.3/pdr_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:16:29.000000 pdr-utils-0.0.3/pdr_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:16:29.000000 pdr-utils-0.0.3/pdr_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 14:16:29.000000 pdr-utils-0.0.3/pdr_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:16:29.000000 pdr-utils-0.0.3/pdr_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:16:29.191584 pdr-utils-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-10 14:16:19.000000 pdr-utils-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:09:37.536529 pdr-utils-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 13:09:25.000000 pdr-utils-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-12 13:09:37.532529 pdr-utils-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 13:09:25.000000 pdr-utils-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:09:37.532529 pdr-utils-0.0.4/pdr_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:09:25.000000 pdr-utils-0.0.4/pdr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-12 13:09:25.000000 pdr-utils-0.0.4/pdr_utils/subgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:09:37.532529 pdr-utils-0.0.4/pdr_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-12 13:09:37.000000 pdr-utils-0.0.4/pdr_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-12 13:09:37.000000 pdr-utils-0.0.4/pdr_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:09:37.000000 pdr-utils-0.0.4/pdr_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:09:37.000000 pdr-utils-0.0.4/pdr_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-12 13:09:37.000000 pdr-utils-0.0.4/pdr_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 13:09:37.000000 pdr-utils-0.0.4/pdr_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:09:37.536529 pdr-utils-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-12 13:09:25.000000 pdr-utils-0.0.4/setup.py
```

### Comparing `pdr-utils-0.0.3/LICENSE` & `pdr-utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdr-utils-0.0.3/PKG-INFO` & `pdr-utils-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Predictoor utils lib.
 Home-page: https://github.com/oceanprotocol/pdr-utils
 Author: oceanprotocol
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pdr-utils-0.0.3/pdr_utils.egg-info/PKG-INFO` & `pdr-utils-0.0.4/pdr_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Predictoor utils lib.
 Home-page: https://github.com/oceanprotocol/pdr-utils
 Author: oceanprotocol
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pdr-utils-0.0.3/setup.py` & `pdr-utils-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 # Installed by pip install ocean-provider
 # or pip install -e .
 install_requirements = [
     "enforce_typing",
     "pylint",
     "bumpversion",
+    "requests",
+    "web3",
+    "coverage",
 ]
 
 # Required to run setup.py:
 setup_requirements = ["pytest-runner"]
 
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
@@ -43,11 +46,11 @@
         ]
     ),
     setup_requires=setup_requirements,
     test_suite="tests",
     url="https://github.com/oceanprotocol/pdr-utils",
     # fmt: off
     # bumpversion needs single quotes
-    version='0.0.3',
+    version='0.0.4',
     # fmt: on
     zip_safe=False,
 )
```

