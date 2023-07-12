# Comparing `tmp/velintegrator-1.0.2.tar.gz` & `tmp/velintegrator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velintegrator-1.0.2.tar", last modified: Tue Jul 11 14:05:07 2023, max compression
+gzip compressed data, was "velintegrator-1.0.3.tar", last modified: Wed Jul 12 07:43:09 2023, max compression
```

## Comparing `velintegrator-1.0.2.tar` & `velintegrator-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 14:05:07.115619 velintegrator-1.0.2/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.0.2/MANIFEST.in
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-11 14:05:07.115498 velintegrator-1.0.2/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      742 2023-07-11 14:04:48.000000 velintegrator-1.0.2/README.md
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-11 14:05:07.115652 velintegrator-1.0.2/setup.cfg
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-07-11 14:03:39.000000 velintegrator-1.0.2/setup.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 14:05:07.114825 velintegrator-1.0.2/velintegrator/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.0.2/velintegrator/__init__.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     1031 2023-07-11 14:03:25.000000 velintegrator-1.0.2/velintegrator/handler.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3608 2023-07-11 12:42:19.000000 velintegrator-1.0.2/velintegrator/sdk.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 14:05:07.115366 velintegrator-1.0.2/velintegrator.egg-info/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-11 14:05:07.000000 velintegrator-1.0.2/velintegrator.egg-info/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-11 14:05:07.000000 velintegrator-1.0.2/velintegrator.egg-info/SOURCES.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-11 14:05:07.000000 velintegrator-1.0.2/velintegrator.egg-info/dependency_links.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-11 14:05:07.000000 velintegrator-1.0.2/velintegrator.egg-info/top_level.txt
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 07:43:09.738017 velintegrator-1.0.3/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.0.3/MANIFEST.in
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 07:43:09.737881 velintegrator-1.0.3/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      742 2023-07-11 14:04:48.000000 velintegrator-1.0.3/README.md
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-12 07:43:09.738064 velintegrator-1.0.3/setup.cfg
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-07-12 07:37:48.000000 velintegrator-1.0.3/setup.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 07:43:09.737033 velintegrator-1.0.3/velintegrator/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.0.3/velintegrator/__init__.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     1031 2023-07-11 14:03:25.000000 velintegrator-1.0.3/velintegrator/handler.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3735 2023-07-12 07:39:28.000000 velintegrator-1.0.3/velintegrator/sdk.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-12 07:43:09.737727 velintegrator-1.0.3/velintegrator.egg-info/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-12 07:43:09.000000 velintegrator-1.0.3/velintegrator.egg-info/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-12 07:43:09.000000 velintegrator-1.0.3/velintegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-12 07:43:09.000000 velintegrator-1.0.3/velintegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-12 07:43:09.000000 velintegrator-1.0.3/velintegrator.egg-info/top_level.txt
```

### Comparing `velintegrator-1.0.2/PKG-INFO` & `velintegrator-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 Kafka Client for VELI.STORE
```

### Comparing `velintegrator-1.0.2/README.md` & `velintegrator-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `velintegrator-1.0.2/velintegrator/handler.py` & `velintegrator-1.0.3/velintegrator/handler.py`

 * *Files identical despite different names*

### Comparing `velintegrator-1.0.2/velintegrator/sdk.py` & `velintegrator-1.0.3/velintegrator/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,19 @@
 
         if response.status_code not in [200, 201, 204]:
             message = "Invalid response, status code: " + str(response.status_code) + " " + str(response.json())
             logging.info(message)
             return
         try:
             response_content = response.json().get('id', response.json())
+            message = f"Success - {str(response.json())}"
         except JSONDecodeError:
             response_content = f"Response content: {response.content}, Response: {response}"
+            message = response_content
+        logging.info(message)
         return response_content
 
     def set_data(self, model):
         return model.dict() if model else None
 
     def test(self):
         print(self.data)
```

### Comparing `velintegrator-1.0.2/velintegrator.egg-info/PKG-INFO` & `velintegrator-1.0.3/velintegrator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 Kafka Client for VELI.STORE
```

