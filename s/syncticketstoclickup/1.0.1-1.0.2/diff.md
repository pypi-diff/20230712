# Comparing `tmp/syncticketstoclickup-1.0.1.tar.gz` & `tmp/syncticketstoclickup-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncticketstoclickup-1.0.1.tar", last modified: Wed Jul 12 17:56:57 2023, max compression
+gzip compressed data, was "syncticketstoclickup-1.0.2.tar", last modified: Wed Jul 12 18:42:28 2023, max compression
```

## Comparing `syncticketstoclickup-1.0.1.tar` & `syncticketstoclickup-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.658749 syncticketstoclickup-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/syncticketstoclickup/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/.env.example
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/clickup.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/zendesk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/zendesk_to_clickup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.359915 syncticketstoclickup-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.359915 syncticketstoclickup-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/syncticketstoclickup/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/.env.example
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/clickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/zendesk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/zendesk_to_clickup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/top_level.txt
```

### Comparing `syncticketstoclickup-1.0.1/.github/workflows/python-publish.yml` & `syncticketstoclickup-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.1/.gitignore` & `syncticketstoclickup-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.1/LICENSE` & `syncticketstoclickup-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.1/Makefile` & `syncticketstoclickup-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.1/PKG-INFO` & `syncticketstoclickup-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncticketstoclickup
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package that allows to sync tickets from Zendesk to ClickUp.
 Author: abrahamprz (Abraham Perez)
 Author-email: fcoabrahamprz@gmail.com
 Keywords: python,zendesk,clickup,ticket,task,sync,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -12,20 +12,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # zendesk-clickup
 Project that syncs all tickets from Zendesk to ClickUp. This is useful for teams that use them for managing customer support tickets and want to keep the ticket numbers consistent across both platforms.
 
-## Configuration
+## Installation
+This module is available on PyPI and can be installed using pip.
+```bash
+$ python -m pip install syncticketstoclickup
+```
+This module requires Python 3.10 or higher.
 
+## Configuration
 1. Duplicate the `.env.example` file and rename it to `.env`.
 2. Replace the placeholder values in the `.env` file with your actual configuration.
 
 ## Usage
 This is the basic usage of the module to sync all tickets from Zendesk to ClickUp.
-
 ```python
 from syncticketstoclickup.zendesk_to_clickup import ZendeskToClickUp
 
 ZendeskToClickUp().sync_zendesk_to_clickup()
 ```
```

### Comparing `syncticketstoclickup-1.0.1/README.md` & `syncticketstoclickup-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # zendesk-clickup
 Project that syncs all tickets from Zendesk to ClickUp. This is useful for teams that use them for managing customer support tickets and want to keep the ticket numbers consistent across both platforms.
 
-## Configuration
+## Installation
+This module is available on PyPI and can be installed using pip.
+```bash
+$ python -m pip install syncticketstoclickup
+```
+This module requires Python 3.10 or higher.
 
+## Configuration
 1. Duplicate the `.env.example` file and rename it to `.env`.
 2. Replace the placeholder values in the `.env` file with your actual configuration.
 
 ## Usage
 This is the basic usage of the module to sync all tickets from Zendesk to ClickUp.
-
 ```python
 from syncticketstoclickup.zendesk_to_clickup import ZendeskToClickUp
 
 ZendeskToClickUp().sync_zendesk_to_clickup()
 ```
```

### Comparing `syncticketstoclickup-1.0.1/setup.py` & `syncticketstoclickup-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.1/syncticketstoclickup/clickup.py` & `syncticketstoclickup-1.0.2/syncticketstoclickup/clickup.py`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.1/syncticketstoclickup/zendesk.py` & `syncticketstoclickup-1.0.2/syncticketstoclickup/zendesk.py`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.1/syncticketstoclickup/zendesk_to_clickup.py` & `syncticketstoclickup-1.0.2/syncticketstoclickup/zendesk_to_clickup.py`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/PKG-INFO` & `syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncticketstoclickup
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package that allows to sync tickets from Zendesk to ClickUp.
 Author: abrahamprz (Abraham Perez)
 Author-email: fcoabrahamprz@gmail.com
 Keywords: python,zendesk,clickup,ticket,task,sync,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -12,20 +12,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # zendesk-clickup
 Project that syncs all tickets from Zendesk to ClickUp. This is useful for teams that use them for managing customer support tickets and want to keep the ticket numbers consistent across both platforms.
 
-## Configuration
+## Installation
+This module is available on PyPI and can be installed using pip.
+```bash
+$ python -m pip install syncticketstoclickup
+```
+This module requires Python 3.10 or higher.
 
+## Configuration
 1. Duplicate the `.env.example` file and rename it to `.env`.
 2. Replace the placeholder values in the `.env` file with your actual configuration.
 
 ## Usage
 This is the basic usage of the module to sync all tickets from Zendesk to ClickUp.
-
 ```python
 from syncticketstoclickup.zendesk_to_clickup import ZendeskToClickUp
 
 ZendeskToClickUp().sync_zendesk_to_clickup()
 ```
```

### Comparing `syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/SOURCES.txt` & `syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

