# Comparing `tmp/velintegrator-1.0.3.tar.gz` & `tmp/velintegrator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velintegrator-1.0.3.tar", last modified: Wed Jul 12 07:43:09 2023, max compression
+gzip compressed data, was "velintegrator-1.0.4.tar", last modified: Wed Jul 12 11:03:48 2023, max compression
```

## Comparing `velintegrator-1.0.3.tar` & `velintegrator-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 07:43:09.738017 velintegrator-1.0.3/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.0.3/MANIFEST.in
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 07:43:09.737881 velintegrator-1.0.3/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      742 2023-07-11 14:04:48.000000 velintegrator-1.0.3/README.md
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-12 07:43:09.738064 velintegrator-1.0.3/setup.cfg
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-07-12 07:37:48.000000 velintegrator-1.0.3/setup.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 07:43:09.737033 velintegrator-1.0.3/velintegrator/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.0.3/velintegrator/__init__.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     1031 2023-07-11 14:03:25.000000 velintegrator-1.0.3/velintegrator/handler.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3735 2023-07-12 07:39:28.000000 velintegrator-1.0.3/velintegrator/sdk.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 07:43:09.737727 velintegrator-1.0.3/velintegrator.egg-info/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 07:43:09.000000 velintegrator-1.0.3/velintegrator.egg-info/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-12 07:43:09.000000 velintegrator-1.0.3/velintegrator.egg-info/SOURCES.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-12 07:43:09.000000 velintegrator-1.0.3/velintegrator.egg-info/dependency_links.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-12 07:43:09.000000 velintegrator-1.0.3/velintegrator.egg-info/top_level.txt
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 11:03:48.213129 velintegrator-1.0.4/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.0.4/MANIFEST.in
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 11:03:48.212979 velintegrator-1.0.4/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      742 2023-07-11 14:04:48.000000 velintegrator-1.0.4/README.md
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-12 11:03:48.213176 velintegrator-1.0.4/setup.cfg
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-07-12 11:03:02.000000 velintegrator-1.0.4/setup.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 11:03:48.212290 velintegrator-1.0.4/velintegrator/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.0.4/velintegrator/__init__.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     1031 2023-07-11 14:03:25.000000 velintegrator-1.0.4/velintegrator/handler.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3737 2023-07-12 11:02:41.000000 velintegrator-1.0.4/velintegrator/sdk.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 11:03:48.212836 velintegrator-1.0.4/velintegrator.egg-info/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 11:03:48.000000 velintegrator-1.0.4/velintegrator.egg-info/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-12 11:03:48.000000 velintegrator-1.0.4/velintegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-12 11:03:48.000000 velintegrator-1.0.4/velintegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-12 11:03:48.000000 velintegrator-1.0.4/velintegrator.egg-info/top_level.txt
```

### Comparing `velintegrator-1.0.3/PKG-INFO` & `velintegrator-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 Kafka Client for VELI.STORE
```

### Comparing `velintegrator-1.0.3/README.md` & `velintegrator-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `velintegrator-1.0.3/velintegrator/handler.py` & `velintegrator-1.0.4/velintegrator/handler.py`

 * *Files identical despite different names*

### Comparing `velintegrator-1.0.3/velintegrator/sdk.py` & `velintegrator-1.0.4/velintegrator/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import re
-
 from requests import request
 from json import JSONDecodeError
-import logging
+from velilogger import logger
 
 
 class Integrator:
     absolute_url = None
     secret_key = None
     headers = {}
 
@@ -14,23 +12,23 @@
         self.data = self.set_data(model)
 
     @staticmethod
     def validate_response(response):
 
         if response.status_code not in [200, 201, 204]:
             message = "Invalid response, status code: " + str(response.status_code) + " " + str(response.json())
-            logging.info(message)
+            logger.info(message)
             return
         try:
             response_content = response.json().get('id', response.json())
             message = f"Success - {str(response.json())}"
         except JSONDecodeError:
             response_content = f"Response content: {response.content}, Response: {response}"
             message = response_content
-        logging.info(message)
+        logger.info(message)
         return response_content
 
     def set_data(self, model):
         return model.dict() if model else None
 
     def test(self):
         print(self.data)
```

### Comparing `velintegrator-1.0.3/velintegrator.egg-info/PKG-INFO` & `velintegrator-1.0.4/velintegrator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 Kafka Client for VELI.STORE
```

