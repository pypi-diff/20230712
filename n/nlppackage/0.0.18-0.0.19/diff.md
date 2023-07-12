# Comparing `tmp/nlppackage-0.0.18.tar.gz` & `tmp/nlppackage-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlppackage-0.0.18.tar", last modified: Wed Jul  5 12:15:06 2023, max compression
+gzip compressed data, was "nlppackage-0.0.19.tar", last modified: Wed Jul 12 07:58:41 2023, max compression
```

## Comparing `nlppackage-0.0.18.tar` & `nlppackage-0.0.19.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:15:06.867544 nlppackage-0.0.18/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-05 12:14:40.000000 nlppackage-0.0.18/LICENSE
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-05 12:15:06.867544 nlppackage-0.0.18/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2696 2023-07-05 12:14:40.000000 nlppackage-0.0.18/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:15:06.866542 nlppackage-0.0.18/nlppackage/
--rw-rw-rw-   0 root         (0) root         (0)     4325 2023-07-05 12:14:40.000000 nlppackage-0.0.18/nlppackage/Class_NLP.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 12:14:40.000000 nlppackage-0.0.18/nlppackage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:15:06.867544 nlppackage-0.0.18/nlppackage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-05 12:15:06.000000 nlppackage-0.0.18/nlppackage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      252 2023-07-05 12:15:06.000000 nlppackage-0.0.18/nlppackage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 12:15:06.000000 nlppackage-0.0.18/nlppackage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-05 12:15:06.000000 nlppackage-0.0.18/nlppackage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-05 12:15:06.000000 nlppackage-0.0.18/nlppackage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-05 12:15:06.867544 nlppackage-0.0.18/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-07-05 12:14:40.000000 nlppackage-0.0.18/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 07:58:41.067463 nlppackage-0.0.19/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-12 07:58:16.000000 nlppackage-0.0.19/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-12 07:58:41.067463 nlppackage-0.0.19/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2696 2023-07-12 07:58:16.000000 nlppackage-0.0.19/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 07:58:41.066463 nlppackage-0.0.19/nlppackage/
+-rw-rw-rw-   0 root         (0) root         (0)     2982 2023-07-12 07:58:16.000000 nlppackage-0.0.19/nlppackage/Class_NLP.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 07:58:17.000000 nlppackage-0.0.19/nlppackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 07:58:41.067463 nlppackage-0.0.19/nlppackage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-12 07:58:41.000000 nlppackage-0.0.19/nlppackage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      252 2023-07-12 07:58:41.000000 nlppackage-0.0.19/nlppackage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 07:58:41.000000 nlppackage-0.0.19/nlppackage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-12 07:58:41.000000 nlppackage-0.0.19/nlppackage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-12 07:58:41.000000 nlppackage-0.0.19/nlppackage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-12 07:58:41.067463 nlppackage-0.0.19/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-07-12 07:58:16.000000 nlppackage-0.0.19/setup.py
```

### Comparing `nlppackage-0.0.18/LICENSE` & `nlppackage-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `nlppackage-0.0.18/README.md` & `nlppackage-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `nlppackage-0.0.18/setup.py` & `nlppackage-0.0.19/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="nlppackage",
     packages=['nlppackage'],
-    version="0.0.18",
+    version="0.0.19",
     author="Business & Décision",
     description="A package for NLP",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

