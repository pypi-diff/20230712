# Comparing `tmp/langchain_ray-0.0.4.tar.gz` & `tmp/langchain_ray-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_ray-0.0.4.tar", last modified: Sun Jul  9 03:21:52 2023, max compression
+gzip compressed data, was "langchain_ray-0.0.9.tar", last modified: Wed Jul 12 21:25:16 2023, max compression
```

## Comparing `langchain_ray-0.0.4.tar` & `langchain_ray-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,45 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 langchain_ray-0.0.4/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 langchain_ray-0.0.4/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      127 2023-07-07 04:36:43.000000 langchain_ray-0.0.4/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/langchain_ray/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     6244 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     3575 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/chains.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      984 2023-07-09 02:01:37.000000 langchain_ray-0.0.4/langchain_ray/imports.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/langchain_ray/pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     6120 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/pdf/chains.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     6485 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/pdf/utils.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/langchain_ray.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      496 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       48 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-07 03:48:41.000000 langchain_ray-0.0.4/langchain_ray.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       85 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       14 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      760 2023-07-09 03:21:30.000000 langchain_ray-0.0.4/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 langchain_ray-0.0.4/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:25:16.404264 langchain_ray-0.0.9/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 langchain_ray-0.0.9/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 langchain_ray-0.0.9/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-12 21:25:16.404264 langchain_ray-0.0.9/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      127 2023-07-07 04:36:43.000000 langchain_ray-0.0.9/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:25:16.400264 langchain_ray-0.0.9/langchain_ray/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    13942 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/_modidx.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:25:16.400264 langchain_ray-0.0.9/langchain_ray/api/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/api/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8428 2023-07-12 21:06:16.000000 langchain_ray-0.0.9/langchain_ray/api/app.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      154 2023-07-12 09:36:09.000000 langchain_ray-0.0.9/langchain_ray/api/app_deployment.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      426 2023-07-12 20:30:18.000000 langchain_ray-0.0.9/langchain_ray/api/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     7560 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/chains.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:25:16.400264 langchain_ray-0.0.9/langchain_ray/driver/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/driver/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     4094 2023-07-12 09:28:44.000000 langchain_ray-0.0.9/langchain_ray/driver/ingress_driver.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1825 2023-07-12 07:30:32.000000 langchain_ray-0.0.9/langchain_ray/driver/redis_kv_store.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1347 2023-07-12 18:43:57.000000 langchain_ray-0.0.9/langchain_ray/imports.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:25:16.404264 langchain_ray-0.0.9/langchain_ray/indexing/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/indexing/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     4933 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/indexing/chains.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2255 2023-07-12 21:18:18.000000 langchain_ray-0.0.9/langchain_ray/indexing/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:25:16.404264 langchain_ray-0.0.9/langchain_ray/ner/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/ner/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      861 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/ner/chains.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     4954 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/ner/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:25:16.404264 langchain_ray-0.0.9/langchain_ray/pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1712 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/pdf/chains.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     4172 2023-07-12 20:17:09.000000 langchain_ray-0.0.9/langchain_ray/pdf/ner.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2081 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/pdf/utils.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3205 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/remote_utils.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     4693 2023-07-12 21:18:19.000000 langchain_ray-0.0.9/langchain_ray/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-12 21:25:16.400264 langchain_ray-0.0.9/langchain_ray.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-12 21:25:16.000000 langchain_ray-0.0.9/langchain_ray.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      990 2023-07-12 21:25:16.000000 langchain_ray-0.0.9/langchain_ray.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-12 21:25:16.000000 langchain_ray-0.0.9/langchain_ray.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       48 2023-07-12 21:25:16.000000 langchain_ray-0.0.9/langchain_ray.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-07 03:48:41.000000 langchain_ray-0.0.9/langchain_ray.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      153 2023-07-12 21:25:16.000000 langchain_ray-0.0.9/langchain_ray.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       14 2023-07-12 21:25:16.000000 langchain_ray-0.0.9/langchain_ray.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      828 2023-07-12 21:15:17.000000 langchain_ray-0.0.9/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-07-12 21:25:16.404264 langchain_ray-0.0.9/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 langchain_ray-0.0.9/setup.py
```

### Comparing `langchain_ray-0.0.4/LICENSE` & `langchain_ray-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_ray-0.0.4/PKG-INFO` & `langchain_ray-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_ray
-Version: 0.0.4
+Version: 0.0.9
 Summary: LangChain leveraging Ray.
 Home-page: https://github.com/HamzaFarhan/langchain_ray
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langchain_ray-0.0.4/langchain_ray.egg-info/PKG-INFO` & `langchain_ray-0.0.9/langchain_ray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-ray
-Version: 0.0.4
+Version: 0.0.9
 Summary: LangChain leveraging Ray.
 Home-page: https://github.com/HamzaFarhan/langchain_ray
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langchain_ray-0.0.4/settings.ini` & `langchain_ray-0.0.9/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = langchain_ray
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.9
 min_python = 3.8
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = langchain_ray
 nbs_path = nbs
 recursive = True
@@ -22,9 +22,9 @@
 author_email = thehamza96@gmail.com
 copyright = 2023 onwards, %(author)s
 description = LangChain leveraging Ray.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = HamzaFarhan
-pip_requirements = "ray[air]" dreamai langchain transformers pypdf faiss-cpu sentence-transformers
+pip_requirements = "ray[air]" dreamai langchain transformers pypdf faiss-cpu sentence-transformers fastai accelerate demoji clean-text Unidecode tabulate redis setfit
```

### Comparing `langchain_ray-0.0.4/setup.py` & `langchain_ray-0.0.9/setup.py`

 * *Files identical despite different names*

