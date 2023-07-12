# Comparing `tmp/ergondata-executions-0.0.8.tar.gz` & `tmp/ergondata-executions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ergondata-executions-0.0.8.tar", last modified: Wed Jul 12 19:37:07 2023, max compression
+gzip compressed data, was "ergondata-executions-0.0.9.tar", last modified: Wed Jul 12 19:44:42 2023, max compression
```

## Comparing `ergondata-executions-0.0.8.tar` & `ergondata-executions-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-07-12 19:37:07.736604 ergondata-executions-0.0.8/
--rw-r--r--   0 daniel     (502) staff       (20)      308 2023-07-12 19:37:07.736357 ergondata-executions-0.0.8/PKG-INFO
-drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-07-12 19:37:07.734382 ergondata-executions-0.0.8/ergondata_executions/
--rw-r--r--   0 daniel     (502) staff       (20)       65 2023-03-24 20:47:01.000000 ergondata-executions-0.0.8/ergondata_executions/__init__.py
--rw-r--r--   0 daniel     (502) staff       (20)     7757 2023-07-12 19:34:13.000000 ergondata-executions-0.0.8/ergondata_executions/executions.py
-drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-07-12 19:37:07.735989 ergondata-executions-0.0.8/ergondata_executions.egg-info/
--rw-r--r--   0 daniel     (502) staff       (20)      308 2023-07-12 19:37:07.000000 ergondata-executions-0.0.8/ergondata_executions.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (502) staff       (20)      295 2023-07-12 19:37:07.000000 ergondata-executions-0.0.8/ergondata_executions.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (502) staff       (20)        1 2023-07-12 19:37:07.000000 ergondata-executions-0.0.8/ergondata_executions.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (502) staff       (20)       27 2023-07-12 19:37:07.000000 ergondata-executions-0.0.8/ergondata_executions.egg-info/requires.txt
--rw-r--r--   0 daniel     (502) staff       (20)       21 2023-07-12 19:37:07.000000 ergondata-executions-0.0.8/ergondata_executions.egg-info/top_level.txt
--rw-r--r--   0 daniel     (502) staff       (20)       38 2023-07-12 19:37:07.736690 ergondata-executions-0.0.8/setup.cfg
--rw-r--r--   0 daniel     (502) staff       (20)      430 2023-07-12 19:36:46.000000 ergondata-executions-0.0.8/setup.py
+drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-07-12 19:44:42.792914 ergondata-executions-0.0.9/
+-rw-r--r--   0 daniel     (502) staff       (20)      308 2023-07-12 19:44:42.792656 ergondata-executions-0.0.9/PKG-INFO
+drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-07-12 19:44:42.790607 ergondata-executions-0.0.9/ergondata_executions/
+-rw-r--r--   0 daniel     (502) staff       (20)       65 2023-03-24 20:47:01.000000 ergondata-executions-0.0.9/ergondata_executions/__init__.py
+-rw-r--r--   0 daniel     (502) staff       (20)     7757 2023-07-12 19:43:47.000000 ergondata-executions-0.0.9/ergondata_executions/executions.py
+drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-07-12 19:44:42.792183 ergondata-executions-0.0.9/ergondata_executions.egg-info/
+-rw-r--r--   0 daniel     (502) staff       (20)      308 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (502) staff       (20)      295 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (502) staff       (20)        1 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (502) staff       (20)       27 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/requires.txt
+-rw-r--r--   0 daniel     (502) staff       (20)       21 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (502) staff       (20)       38 2023-07-12 19:44:42.793000 ergondata-executions-0.0.9/setup.cfg
+-rw-r--r--   0 daniel     (502) staff       (20)      430 2023-07-12 19:44:38.000000 ergondata-executions-0.0.9/setup.py
```

### Comparing `ergondata-executions-0.0.8/ergondata_executions/executions.py` & `ergondata-executions-0.0.9/ergondata_executions/executions.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     message: str
     reason: NotRequired[str]
     data: NotRequired[object]
 
 
 class ExecutionsController:
 
-    # __ROOT_URL = "http://ergondata-django-api.us-east-1.elasticbeanstalk.com/api/"
-    __ROOT_URL = "http://127.0.0.1:8000/api/"
+    __ROOT_URL = "http://ergondata-django-api.us-east-1.elasticbeanstalk.com/api/"
+    # __ROOT_URL = "http://127.0.0.1:8000/api/"
     __AUTH_URL = "auth"
     __CREATE_EXECUTION_URL = "executions/create/execution"
     __UPDATE_EXECUTION_URL = "executions/update/execution"
     __CREATE_QUEUE_ITEM_URL = "executions/create/queue-item"
     __UPDATE_QUEUE_ITEM_URL = "executions/update/queue-item"
     __GET_QUEUE_ITEM_URL = "executions/get/queue-item"
     __GET_QUEUE_SIZE_URL = "executions/get/queue-size"
```

