# Comparing `tmp/dropstackframe-0.1.0.tar.gz` & `tmp/dropstackframe-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dropstackframe-0.1.0.tar", max compression
+gzip compressed data, was "dropstackframe-0.1.0a7.tar", max compression
```

## Comparing `dropstackframe-0.1.0.tar` & `dropstackframe-0.1.0a7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-07-12 16:37:20.003827 dropstackframe-0.1.0/LICENSE
--rw-r--r--   0        0        0     3495 2023-07-12 16:37:20.003827 dropstackframe-0.1.0/README.md
--rw-r--r--   0        0        0      309 2023-07-12 16:37:20.003827 dropstackframe-0.1.0/dropstackframe/__init__.py
--rw-r--r--   0        0        0     2553 2023-07-12 16:37:20.003827 dropstackframe-0.1.0/dropstackframe/dropstackframe.py
--rw-r--r--   0        0        0        0 2023-07-12 16:37:20.003827 dropstackframe-0.1.0/dropstackframe/py.typed
--rw-r--r--   0        0        0     2679 2023-07-12 16:37:58.535889 dropstackframe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4371 1970-01-01 00:00:00.000000 dropstackframe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-12 16:27:11.699984 dropstackframe-0.1.0a7/LICENSE
+-rw-r--r--   0        0        0     3495 2023-07-12 16:27:11.699984 dropstackframe-0.1.0a7/README.md
+-rw-r--r--   0        0        0      309 2023-07-12 16:27:11.699984 dropstackframe-0.1.0a7/dropstackframe/__init__.py
+-rw-r--r--   0        0        0     2553 2023-07-12 16:27:11.699984 dropstackframe-0.1.0a7/dropstackframe/dropstackframe.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:27:11.699984 dropstackframe-0.1.0a7/dropstackframe/py.typed
+-rw-r--r--   0        0        0     2682 2023-07-12 16:27:31.100270 dropstackframe-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 dropstackframe-0.1.0a7/PKG-INFO
```

### Comparing `dropstackframe-0.1.0/LICENSE` & `dropstackframe-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `dropstackframe-0.1.0/README.md` & `dropstackframe-0.1.0a7/README.md`

 * *Files identical despite different names*

### Comparing `dropstackframe-0.1.0/dropstackframe/dropstackframe.py` & `dropstackframe-0.1.0a7/dropstackframe/dropstackframe.py`

 * *Files identical despite different names*

### Comparing `dropstackframe-0.1.0/pyproject.toml` & `dropstackframe-0.1.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dropstackframe"
-version = "0.1.0"
+version = "0.1.0-a7"
 description = "A python package for removing stack frames from stack traces."
 authors = [ "Jesper Nielsen <jespernielsen1982+dropstackframe@gmail.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jesnie/dropstackframe"
 repository = "https://github.com/jesnie/dropstackframe"
 classifiers = [ "Development Status :: 4 - Beta", "Intended Audience :: Developers", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11", "Typing :: Typed",]
```

### Comparing `dropstackframe-0.1.0/PKG-INFO` & `dropstackframe-0.1.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropstackframe
-Version: 0.1.0
+Version: 0.1.0a7
 Summary: A python package for removing stack frames from stack traces.
 Home-page: https://github.com/jesnie/dropstackframe
 License: MIT
 Author: Jesper Nielsen
 Author-email: jespernielsen1982+dropstackframe@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

