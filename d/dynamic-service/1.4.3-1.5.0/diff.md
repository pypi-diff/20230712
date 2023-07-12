# Comparing `tmp/dynamic-service-1.4.3.tar.gz` & `tmp/dynamic-service-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.4.3.tar", last modified: Mon Jul 10 07:19:45 2023, max compression
+gzip compressed data, was "dynamic-service-1.5.0.tar", last modified: Wed Jul 12 13:02:51 2023, max compression
```

## Comparing `dynamic-service-1.4.3.tar` & `dynamic-service-1.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.756045 dynamic-service-1.4.3/
--rw-rw-rw-   0        0        0      236 2023-07-10 07:19:44.000000 dynamic-service-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-10 07:19:45.755541 dynamic-service-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/build.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.696094 dynamic-service-1.4.3/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.738286 dynamic-service-1.4.3/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.4.3/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     8954 2023-07-08 15:55:29.000000 dynamic-service-1.4.3/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.4.3/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.4.3/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.748915 dynamic-service-1.4.3/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    20624 2023-07-10 07:19:23.000000 dynamic-service-1.4.3/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.4.3/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.686496 dynamic-service-1.4.3/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.686496 dynamic-service-1.4.3/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.753427 dynamic-service-1.4.3/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.710348 dynamic-service-1.4.3/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-10 07:19:44.000000 dynamic-service-1.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.4.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.4.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 07:19:45.756045 dynamic-service-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-07-10 07:19:39.000000 dynamic-service-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.079254 dynamic-service-1.5.0/
+-rw-rw-rw-   0        0        0      236 2023-07-12 13:02:48.000000 dynamic-service-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-12 13:02:51.079254 dynamic-service-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.017291 dynamic-service-1.5.0/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.062075 dynamic-service-1.5.0/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.5.0/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     8954 2023-07-08 15:55:29.000000 dynamic-service-1.5.0/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.5.0/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.5.0/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.072245 dynamic-service-1.5.0/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    20656 2023-07-12 13:02:21.000000 dynamic-service-1.5.0/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.5.0/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.006088 dynamic-service-1.5.0/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.007088 dynamic-service-1.5.0/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.077256 dynamic-service-1.5.0/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.031104 dynamic-service-1.5.0/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-07-12 13:02:48.000000 dynamic-service-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.5.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 13:02:51.079254 dynamic-service-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-07-12 13:02:34.000000 dynamic-service-1.5.0/setup.py
```

### Comparing `dynamic-service-1.4.3/PKG-INFO` & `dynamic-service-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.4.3
+Version: 1.5.0
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.4.3/README.md` & `dynamic-service-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/build.py` & `dynamic-service-1.5.0/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/dynamic_service/base.py` & `dynamic-service-1.5.0/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/dynamic_service/endpoints/data.py` & `dynamic-service-1.5.0/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/dynamic_service/endpoints/engine.py` & `dynamic-service-1.5.0/dynamic_service/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.5.0/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/dynamic_service/endpoints/process.py` & `dynamic-service-1.5.0/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/dynamic_service/service/rest.py` & `dynamic-service-1.5.0/dynamic_service/service/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,14 +583,16 @@
         if not self.created:
             self.create(
                 host=host, port=port, silent=silent,
                 daemon=daemon
             )
         # end if
 
+        self._serving = True
+
         self._serving_process.start()
     # end start_serving
 
     def run(
             self,
             serve: Optional[bool] = True,
             host: Optional[Host] = None,
```

### Comparing `dynamic-service-1.4.3/dynamic_service/service/sockets.py` & `dynamic-service-1.5.0/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.5.0/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.5.0/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.5.0/dynamic_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.4.3
+Version: 1.5.0
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.4.3/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.5.0/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.3/pyproject.toml` & `dynamic-service-1.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.4.3'
+version = '1.5.0'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.4.3/setup.py` & `dynamic-service-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.4.3',
+        version='1.5.0',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

