# Comparing `tmp/dynamic-sh-0.0.1a1.tar.gz` & `tmp/dynamic-sh-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-sh-0.0.1a1.tar", last modified: Tue Jul 11 22:09:38 2023, max compression
+gzip compressed data, was "dynamic-sh-0.0.2.tar", last modified: Tue Jul 11 22:14:41 2023, max compression
```

## Comparing `dynamic-sh-0.0.1a1.tar` & `dynamic-sh-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:09:38.470033 dynamic-sh-0.0.1a1/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      518 2023-07-11 22:09:38.469911 dynamic-sh-0.0.1a1/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/README.md
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:09:38.467998 dynamic-sh-0.0.1a1/dynamic/
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1400 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:09:38.468470 dynamic-sh-0.0.1a1/dynamic/classes/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/classes/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1280 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/classes/agent.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      133 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/classes/chain.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/classes/logger.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-sh-0.0.1a1/dynamic/classes/message.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:09:38.468769 dynamic-sh-0.0.1a1/dynamic/protocols/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/protocols/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)    10102 2023-07-11 18:24:11.000000 dynamic-sh-0.0.1a1/dynamic/protocols/server.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1419 2023-07-11 18:24:11.000000 dynamic-sh-0.0.1a1/dynamic/protocols/ws.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:09:38.468877 dynamic-sh-0.0.1a1/dynamic/request/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/request/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:09:38.468957 dynamic-sh-0.0.1a1/dynamic/response/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/response/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:09:38.469281 dynamic-sh-0.0.1a1/dynamic/router/
--rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/router/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/router/get_file_routes.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2113 2023-07-08 22:39:44.000000 dynamic-sh-0.0.1a1/dynamic/router/router.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:09:38.469765 dynamic-sh-0.0.1a1/dynamic_sh.egg-info/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      518 2023-07-11 22:09:38.000000 dynamic-sh-0.0.1a1/dynamic_sh.egg-info/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)      545 2023-07-11 22:09:38.000000 dynamic-sh-0.0.1a1/dynamic_sh.egg-info/SOURCES.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-11 22:09:38.000000 dynamic-sh-0.0.1a1/dynamic_sh.egg-info/dependency_links.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)        8 2023-07-11 22:09:38.000000 dynamic-sh-0.0.1a1/dynamic_sh.egg-info/top_level.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)      560 2023-07-11 22:09:28.000000 dynamic-sh-0.0.1a1/pyproject.toml
--rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-11 22:09:38.470067 dynamic-sh-0.0.1a1/setup.cfg
--rw-r--r--   0 omarwaseem   (501) staff       (20)      713 2023-07-11 22:09:32.000000 dynamic-sh-0.0.1a1/setup.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.670680 dynamic-sh-0.0.2/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      516 2023-07-11 22:14:41.670542 dynamic-sh-0.0.2/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/README.md
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.667348 dynamic-sh-0.0.2/dynamic/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1400 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.668379 dynamic-sh-0.0.2/dynamic/classes/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/classes/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1280 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/classes/agent.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      133 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/classes/chain.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/classes/logger.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-sh-0.0.2/dynamic/classes/message.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.668954 dynamic-sh-0.0.2/dynamic/protocols/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/protocols/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)    10102 2023-07-11 18:24:11.000000 dynamic-sh-0.0.2/dynamic/protocols/server.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1419 2023-07-11 18:24:11.000000 dynamic-sh-0.0.2/dynamic/protocols/ws.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.669096 dynamic-sh-0.0.2/dynamic/request/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/request/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.669185 dynamic-sh-0.0.2/dynamic/response/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/response/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.669559 dynamic-sh-0.0.2/dynamic/router/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/router/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/router/get_file_routes.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2113 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/router/router.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.670343 dynamic-sh-0.0.2/dynamic_sh.egg-info/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      516 2023-07-11 22:14:41.000000 dynamic-sh-0.0.2/dynamic_sh.egg-info/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      545 2023-07-11 22:14:41.000000 dynamic-sh-0.0.2/dynamic_sh.egg-info/SOURCES.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-11 22:14:41.000000 dynamic-sh-0.0.2/dynamic_sh.egg-info/dependency_links.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        8 2023-07-11 22:14:41.000000 dynamic-sh-0.0.2/dynamic_sh.egg-info/top_level.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      553 2023-07-11 22:13:47.000000 dynamic-sh-0.0.2/pyproject.toml
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-11 22:14:41.670727 dynamic-sh-0.0.2/setup.cfg
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      840 2023-07-11 22:14:34.000000 dynamic-sh-0.0.2/setup.py
```

### Comparing `dynamic-sh-0.0.1a1/PKG-INFO` & `dynamic-sh-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-sh
-Version: 0.0.1a1
+Version: 0.0.2
 Author: 
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dynamic-sh-0.0.1a1/dynamic/__init__.py` & `dynamic-sh-0.0.2/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.1a1/dynamic/classes/agent.py` & `dynamic-sh-0.0.2/dynamic/classes/agent.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.1a1/dynamic/classes/message.py` & `dynamic-sh-0.0.2/dynamic/classes/message.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.1a1/dynamic/protocols/server.py` & `dynamic-sh-0.0.2/dynamic/protocols/server.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.1a1/dynamic/protocols/ws.py` & `dynamic-sh-0.0.2/dynamic/protocols/ws.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.1a1/dynamic/router/get_file_routes.py` & `dynamic-sh-0.0.2/dynamic/router/get_file_routes.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.1a1/dynamic/router/router.py` & `dynamic-sh-0.0.2/dynamic/router/router.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.1a1/dynamic_sh.egg-info/PKG-INFO` & `dynamic-sh-0.0.2/dynamic_sh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-sh
-Version: 0.0.1a1
+Version: 0.0.2
 Author: 
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dynamic-sh-0.0.1a1/dynamic_sh.egg-info/SOURCES.txt` & `dynamic-sh-0.0.2/dynamic_sh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.1a1/pyproject.toml` & `dynamic-sh-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynamic-sh"
-version = "0.0.1-alpha1"
+version = "0.0.2"
 description = ""
 authors = [
     "Furqan Rydhan <furqan.rydhan@gmail.com>",
     "Aman Ibrahim <amanmibra@gmail.com>"
 ]
 readme = "README.md"
 keywords = ["llm", "langchain"]
```

### Comparing `dynamic-sh-0.0.1a1/setup.py` & `dynamic-sh-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
-setup(
-    name='dynamic-sh',
-    version='0.0.1-alpha1',
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

