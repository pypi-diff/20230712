# Comparing `tmp/reliableGPT-0.2.982.tar.gz` & `tmp/reliableGPT-0.2.983.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.982.tar", last modified: Wed Jul 12 21:27:02 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.983.tar", last modified: Wed Jul 12 21:29:17 2023, max compression
```

## Comparing `reliableGPT-0.2.982.tar` & `reliableGPT-0.2.983.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:27:02.973633 reliableGPT-0.2.982/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.982/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-12 21:27:02.973507 reliableGPT-0.2.982/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.982/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.982/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:27:02.971946 reliableGPT-0.2.982/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:27:02.973155 reliableGPT-0.2.982/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.982/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    19026 2023-07-12 21:23:16.000000 reliableGPT-0.2.982/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.982/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.982/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5325 2023-07-12 21:22:05.000000 reliableGPT-0.2.982/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-12 21:27:02.973683 reliableGPT-0.2.982/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-12 21:26:48.000000 reliableGPT-0.2.982/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:29:17.454407 reliableGPT-0.2.983/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.983/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-12 21:29:17.454288 reliableGPT-0.2.983/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.983/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.983/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:29:17.452586 reliableGPT-0.2.983/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-12 21:29:17.000000 reliableGPT-0.2.983/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:29:17.454078 reliableGPT-0.2.983/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.983/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    19026 2023-07-12 21:23:16.000000 reliableGPT-0.2.983/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.983/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.983/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5272 2023-07-12 21:28:58.000000 reliableGPT-0.2.983/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-12 21:29:17.454450 reliableGPT-0.2.983/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-12 21:29:14.000000 reliableGPT-0.2.983/setup.py
```

### Comparing `reliableGPT-0.2.982/LICENSE` & `reliableGPT-0.2.983/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.982/README.md` & `reliableGPT-0.2.983/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.982/reliablegpt/Alerting.py` & `reliableGPT-0.2.983/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.982/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.983/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.982/reliablegpt/Model.py` & `reliableGPT-0.2.983/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.982/reliablegpt/main.py` & `reliableGPT-0.2.983/reliablegpt/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # # Prod Imports
 from reliablegpt.IndividualRequest import IndividualRequest
 from reliablegpt.Model import Model
 from reliablegpt.Alerting import Alerting
-from reliablegpt.reliableQuery import reliable_query
 import requests
 
 # # Dev Imports
 # from IndividualRequest import IndividualRequest
 # from Model import Model
 # from Alerting import Alerting
```

