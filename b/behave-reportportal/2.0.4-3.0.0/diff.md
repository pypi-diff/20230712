# Comparing `tmp/behave-reportportal-2.0.4.tar.gz` & `tmp/behave-reportportal-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behave-reportportal-2.0.4.tar", last modified: Mon Jun 12 12:11:33 2023, max compression
+gzip compressed data, was "behave-reportportal-3.0.0.tar", last modified: Wed Jul 12 13:35:30 2023, max compression
```

## Comparing `behave-reportportal-2.0.4.tar` & `behave-reportportal-3.0.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/behave_reportportal/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/behave_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/behave_agent.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/behave_reportportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:35:30.921695 behave-reportportal-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-07-12 13:35:30.921695 behave-reportportal-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:35:30.921695 behave-reportportal-3.0.0/behave_reportportal/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/behave_reportportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/behave_reportportal/behave_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/behave_reportportal/behave_agent.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/behave_reportportal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/behave_reportportal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:35:30.921695 behave-reportportal-3.0.0/behave_reportportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-07-12 13:35:30.000000 behave-reportportal-3.0.0/behave_reportportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-12 13:35:30.000000 behave-reportportal-3.0.0/behave_reportportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:35:30.000000 behave-reportportal-3.0.0/behave_reportportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 13:35:30.000000 behave-reportportal-3.0.0/behave_reportportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 13:35:30.000000 behave-reportportal-3.0.0/behave_reportportal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-12 13:35:30.921695 behave-reportportal-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-12 13:35:25.000000 behave-reportportal-3.0.0/setup.py
```

### Comparing `behave-reportportal-2.0.4/LICENSE` & `behave-reportportal-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `behave-reportportal-2.0.4/PKG-INFO` & `behave-reportportal-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: behave-reportportal
-Version: 2.0.4
+Version: 3.0.0
 Summary: Agent for reporting Behave results to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-behave
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,behave
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 agent-python-behave
 ===================
```

### Comparing `behave-reportportal-2.0.4/README.rst` & `behave-reportportal-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `behave-reportportal-2.0.4/behave_reportportal/__init__.py` & `behave-reportportal-3.0.0/behave_reportportal/__init__.py`

 * *Files identical despite different names*

### Comparing `behave-reportportal-2.0.4/behave_reportportal/behave_agent.py` & `behave-reportportal-3.0.0/behave_reportportal/behave_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
             project=cfg.project,
             api_key=cfg.api_key,
             is_skipped_an_issue=cfg.is_skipped_an_issue,
             launch_id=cfg.launch_id,
             retries=cfg.retries,
             mode="DEBUG" if cfg.debug_mode else "DEFAULT",
             log_batch_size=cfg.log_batch_size,
-            log_batch_payload_size=cfg.log_batch_payload_size
+            log_batch_payload_size=cfg.log_batch_payload_size,
+            launch_uuid_print=cfg.launch_uuid_print,
+            print_output=cfg.launch_uuid_print_output
         )
 
 
 class BehaveAgent(metaclass=Singleton):
     """Functionality for integration of Behave tests with Report Portal."""
 
     def __init__(self, cfg, rp_service=None):
```

### Comparing `behave-reportportal-2.0.4/behave_reportportal/behave_agent.pyi` & `behave-reportportal-3.0.0/behave_reportportal/behave_agent.pyi`

 * *Files identical despite different names*

### Comparing `behave-reportportal-2.0.4/behave_reportportal/utils.py` & `behave-reportportal-3.0.0/behave_reportportal/utils.py`

 * *Files identical despite different names*

### Comparing `behave-reportportal-2.0.4/behave_reportportal.egg-info/PKG-INFO` & `behave-reportportal-3.0.0/behave_reportportal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: behave-reportportal
-Version: 2.0.4
+Version: 3.0.0
 Summary: Agent for reporting Behave results to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-behave
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,behave
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 agent-python-behave
 ===================
```

### Comparing `behave-reportportal-2.0.4/setup.py` & `behave-reportportal-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Config for setup package behave agent."""
 
 import os
 
 from setuptools import setup
 
-__version__ = '2.0.4'
+__version__ = '3.0.0'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Filename to be read
     :return: File content
@@ -29,14 +29,14 @@
     packages=['behave_reportportal'],
     package_data={'behave_reportportal': ['*.pyi']},
     python_requires='>=3.6',
     install_requires=read_file('requirements.txt').splitlines(),
     license='Apache 2.0',
     keywords=['testing', 'reporting', 'reportportal', 'behave'],
     classifiers=[
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ]
 )
```

