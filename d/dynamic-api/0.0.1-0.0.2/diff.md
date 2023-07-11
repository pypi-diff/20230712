# Comparing `tmp/dynamic-api-0.0.1.tar.gz` & `tmp/dynamic-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-api-0.0.1.tar", last modified: Tue Jul 11 22:02:09 2023, max compression
+gzip compressed data, was "dynamic-api-0.0.2.tar", last modified: Tue Jul 11 22:14:41 2023, max compression
```

## Comparing `dynamic-api-0.0.1.tar` & `dynamic-api-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:02:09.575732 dynamic-api-0.0.1/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      517 2023-07-11 22:02:09.575569 dynamic-api-0.0.1/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/README.md
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:02:09.572696 dynamic-api-0.0.1/dynamic-sh/
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1400 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:02:09.573580 dynamic-api-0.0.1/dynamic-sh/classes/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/classes/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1280 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/classes/agent.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      133 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/classes/chain.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/classes/logger.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-api-0.0.1/dynamic-sh/classes/message.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:02:09.574169 dynamic-api-0.0.1/dynamic-sh/protocols/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/protocols/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)    10102 2023-07-11 18:24:11.000000 dynamic-api-0.0.1/dynamic-sh/protocols/server.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1419 2023-07-11 18:24:11.000000 dynamic-api-0.0.1/dynamic-sh/protocols/ws.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:02:09.574397 dynamic-api-0.0.1/dynamic-sh/request/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/request/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:02:09.574538 dynamic-api-0.0.1/dynamic-sh/response/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/response/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:02:09.574940 dynamic-api-0.0.1/dynamic-sh/router/
--rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/router/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/router/get_file_routes.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2113 2023-07-08 22:39:44.000000 dynamic-api-0.0.1/dynamic-sh/router/router.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:02:09.575413 dynamic-api-0.0.1/dynamic_api.egg-info/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      517 2023-07-11 22:02:09.000000 dynamic-api-0.0.1/dynamic_api.egg-info/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)      591 2023-07-11 22:02:09.000000 dynamic-api-0.0.1/dynamic_api.egg-info/SOURCES.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-11 22:02:09.000000 dynamic-api-0.0.1/dynamic_api.egg-info/dependency_links.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)       11 2023-07-11 22:02:09.000000 dynamic-api-0.0.1/dynamic_api.egg-info/top_level.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)      553 2023-07-11 18:51:44.000000 dynamic-api-0.0.1/pyproject.toml
--rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-11 22:02:09.575774 dynamic-api-0.0.1/setup.cfg
--rw-r--r--   0 omarwaseem   (501) staff       (20)      707 2023-07-11 22:02:05.000000 dynamic-api-0.0.1/setup.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.735797 dynamic-api-0.0.2/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      517 2023-07-11 22:14:41.735692 dynamic-api-0.0.2/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/README.md
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.734026 dynamic-api-0.0.2/dynamic/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1400 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.734465 dynamic-api-0.0.2/dynamic/classes/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/classes/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1280 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/classes/agent.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      133 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/classes/chain.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/classes/logger.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-api-0.0.2/dynamic/classes/message.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.734731 dynamic-api-0.0.2/dynamic/protocols/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/protocols/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)    10102 2023-07-11 18:24:11.000000 dynamic-api-0.0.2/dynamic/protocols/server.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1419 2023-07-11 18:24:11.000000 dynamic-api-0.0.2/dynamic/protocols/ws.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.734820 dynamic-api-0.0.2/dynamic/request/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/request/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.734892 dynamic-api-0.0.2/dynamic/response/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/response/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.735161 dynamic-api-0.0.2/dynamic/router/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/router/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/router/get_file_routes.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2113 2023-07-08 22:39:44.000000 dynamic-api-0.0.2/dynamic/router/router.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.735555 dynamic-api-0.0.2/dynamic_api.egg-info/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      517 2023-07-11 22:14:41.000000 dynamic-api-0.0.2/dynamic_api.egg-info/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      549 2023-07-11 22:14:41.000000 dynamic-api-0.0.2/dynamic_api.egg-info/SOURCES.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-11 22:14:41.000000 dynamic-api-0.0.2/dynamic_api.egg-info/dependency_links.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        8 2023-07-11 22:14:41.000000 dynamic-api-0.0.2/dynamic_api.egg-info/top_level.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      553 2023-07-11 22:13:47.000000 dynamic-api-0.0.2/pyproject.toml
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-11 22:14:41.735830 dynamic-api-0.0.2/setup.cfg
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      840 2023-07-11 22:14:34.000000 dynamic-api-0.0.2/setup.py
```

### Comparing `dynamic-api-0.0.1/PKG-INFO` & `dynamic-api-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-api
-Version: 0.0.1
+Version: 0.0.2
 Author: 
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dynamic-api-0.0.1/dynamic-sh/__init__.py` & `dynamic-api-0.0.2/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamic-api-0.0.1/dynamic-sh/classes/agent.py` & `dynamic-api-0.0.2/dynamic/classes/agent.py`

 * *Files identical despite different names*

### Comparing `dynamic-api-0.0.1/dynamic-sh/classes/message.py` & `dynamic-api-0.0.2/dynamic/classes/message.py`

 * *Files identical despite different names*

### Comparing `dynamic-api-0.0.1/dynamic-sh/protocols/server.py` & `dynamic-api-0.0.2/dynamic/protocols/server.py`

 * *Files identical despite different names*

### Comparing `dynamic-api-0.0.1/dynamic-sh/protocols/ws.py` & `dynamic-api-0.0.2/dynamic/protocols/ws.py`

 * *Files identical despite different names*

### Comparing `dynamic-api-0.0.1/dynamic-sh/router/get_file_routes.py` & `dynamic-api-0.0.2/dynamic/router/get_file_routes.py`

 * *Files identical despite different names*

### Comparing `dynamic-api-0.0.1/dynamic-sh/router/router.py` & `dynamic-api-0.0.2/dynamic/router/router.py`

 * *Files identical despite different names*

### Comparing `dynamic-api-0.0.1/dynamic_api.egg-info/PKG-INFO` & `dynamic-api-0.0.2/dynamic_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-api
-Version: 0.0.1
+Version: 0.0.2
 Author: 
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dynamic-api-0.0.1/pyproject.toml` & `dynamic-api-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynamic-sh"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = [
     "Furqan Rydhan <furqan.rydhan@gmail.com>",
     "Aman Ibrahim <amanmibra@gmail.com>"
 ]
 readme = "README.md"
 keywords = ["llm", "langchain"]
```

### Comparing `dynamic-api-0.0.1/setup.py` & `dynamic-api-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
-setup(
-    name='dynamic-api',
-    version='0.0.1',
-    description='',
-    author='',
-    author_email='',
-    packages=find_packages(),
-    install_requires=[
-        # List of package dependencies
-    ],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
+for name in ['dynamic-sh', 'dynamic-llm', 'dynamic-api']:
+    setup(
+        name=name,
+        version='0.0.2',
+        description='',
+        author='',
+        author_email='',
+        packages=find_packages(),
+        install_requires=[
+            # List of package dependencies
+        ],
+        classifiers=[
+            'Development Status :: 3 - Alpha',
+            'Intended Audience :: Developers',
+            'License :: OSI Approved :: MIT License',
+            'Programming Language :: Python :: 3',
+            'Programming Language :: Python :: 3.6',
+            'Programming Language :: Python :: 3.7',
+            'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
+        ],
 )
```

