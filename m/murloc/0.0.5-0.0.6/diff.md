# Comparing `tmp/murloc-0.0.5.tar.gz` & `tmp/murloc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murloc-0.0.5.tar", last modified: Thu Jun  1 02:41:24 2023, max compression
+gzip compressed data, was "murloc-0.0.6.tar", last modified: Wed Jul 12 02:29:44 2023, max compression
```

## Comparing `murloc-0.0.5.tar` & `murloc-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-01 02:41:24.564990 murloc-0.0.5/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-05-26 21:19:51.000000 murloc-0.0.5/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     4086 2023-06-01 02:41:24.564990 murloc-0.0.5/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     3722 2023-06-01 02:38:30.000000 murloc-0.0.5/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-01 02:41:24.563990 murloc-0.0.5/murloc/
--rw-rw-r--   0 chris     (1000) chris     (1000)       25 2023-05-26 20:30:24.000000 murloc-0.0.5/murloc/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5058 2023-06-01 02:19:05.000000 murloc-0.0.5/murloc/murloc.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-01 02:41:24.564990 murloc-0.0.5/murloc.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     4086 2023-06-01 02:41:24.000000 murloc-0.0.5/murloc.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-06-01 02:41:24.000000 murloc-0.0.5/murloc.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-01 02:41:24.000000 murloc-0.0.5/murloc.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-06-01 02:41:24.000000 murloc-0.0.5/murloc.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-06-01 02:41:24.564990 murloc-0.0.5/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-06-01 01:31:57.000000 murloc-0.0.5/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-12 02:29:44.634876 murloc-0.0.6/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-07-11 01:36:26.000000 murloc-0.0.6/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1171 2023-07-12 02:29:44.634876 murloc-0.0.6/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3722 2023-07-11 01:36:26.000000 murloc-0.0.6/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-12 02:29:44.633876 murloc-0.0.6/murloc/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      841 2023-07-12 02:06:09.000000 murloc-0.0.6/murloc/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2967 2023-07-12 02:04:15.000000 murloc-0.0.6/murloc/murloc.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-12 02:29:44.634876 murloc-0.0.6/murloc.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1171 2023-07-12 02:29:44.000000 murloc-0.0.6/murloc.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-07-12 02:29:44.000000 murloc-0.0.6/murloc.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-12 02:29:44.000000 murloc-0.0.6/murloc.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-07-12 02:29:44.000000 murloc-0.0.6/murloc.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-07-12 02:29:44.635876 murloc-0.0.6/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      527 2023-07-12 02:29:39.000000 murloc-0.0.6/setup.py
```

### Comparing `murloc-0.0.5/LICENSE` & `murloc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `murloc-0.0.5/PKG-INFO` & `murloc-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: murloc
-Version: 0.0.5
-Summary: extensible api server
-Home-page: 
-Author: Chris Varga
-Author-email: 
-Keywords: extensible api server
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Murloc
 Extensible api server
 
 ## Example usage
 ```python
 import murloc
```

### Comparing `murloc-0.0.5/setup.py` & `murloc-0.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,17 @@
+import murloc
 from setuptools import setup, find_packages
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
 setup(
     name="murloc",
-    version="0.0.5",
+    version="0.0.6",
     author="Chris Varga",
     author_email="",
-    description="extensible api server",
-    long_description=long_description,
+    description="Extensible API server",
+    long_description=murloc.__doc__,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

