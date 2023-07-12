# Comparing `tmp/bestPR1-0.6.10.tar.gz` & `tmp/bestPR1-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bestPR1-0.6.10.tar", last modified: Wed Jul 12 09:42:17 2023, max compression
+gzip compressed data, was "bestPR1-0.6.9.tar", last modified: Wed Jul 12 08:41:07 2023, max compression
```

## Comparing `bestPR1-0.6.10.tar` & `bestPR1-0.6.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 09:42:17.014415 bestPR1-0.6.10/
--rw-rw-rw-   0        0        0     1131 2023-07-12 09:42:17.013414 bestPR1-0.6.10/PKG-INFO
--rw-rw-rw-   0        0        0      683 2023-07-12 09:28:14.000000 bestPR1-0.6.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 09:42:16.989409 bestPR1-0.6.10/bestPR/
--rw-rw-rw-   0        0        0     1568 2023-07-12 07:40:56.000000 bestPR1-0.6.10/bestPR/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 09:42:17.012414 bestPR1-0.6.10/bestPR1.egg-info/
--rw-rw-rw-   0        0        0     1131 2023-07-12 09:42:16.000000 bestPR1-0.6.10/bestPR1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-07-12 09:42:16.000000 bestPR1-0.6.10/bestPR1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 09:42:16.000000 bestPR1-0.6.10/bestPR1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 09:42:16.000000 bestPR1-0.6.10/bestPR1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 09:42:16.000000 bestPR1-0.6.10/bestPR1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 09:42:17.014415 bestPR1-0.6.10/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-07-12 09:41:51.000000 bestPR1-0.6.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:07.359833 bestPR1-0.6.9/
+-rw-rw-rw-   0        0        0      345 2023-07-12 08:41:07.358834 bestPR1-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-12 05:08:05.000000 bestPR1-0.6.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:07.330825 bestPR1-0.6.9/bestPR/
+-rw-rw-rw-   0        0        0     1568 2023-07-12 07:40:56.000000 bestPR1-0.6.9/bestPR/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:07.355833 bestPR1-0.6.9/bestPR1.egg-info/
+-rw-rw-rw-   0        0        0      345 2023-07-12 08:41:07.000000 bestPR1-0.6.9/bestPR1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-07-12 08:41:07.000000 bestPR1-0.6.9/bestPR1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 08:41:07.000000 bestPR1-0.6.9/bestPR1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 08:41:07.000000 bestPR1-0.6.9/bestPR1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 08:41:07.000000 bestPR1-0.6.9/bestPR1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 08:41:07.359833 bestPR1-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-07-12 08:40:47.000000 bestPR1-0.6.9/setup.py
```

### Comparing `bestPR1-0.6.10/bestPR/__init__.py` & `bestPR1-0.6.9/bestPR/__init__.py`

 * *Files identical despite different names*

### Comparing `bestPR1-0.6.10/setup.py` & `bestPR1-0.6.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description =f.read()
 setup( name="bestPR1",
-       version="0.6.10",
-       description="see long description",
+       version="0.6.9",
        long_description=long_description,
        long_description_content_type="text/markdown",
        author="Ujjawal",
        url = "",
        author_email="ujjawald21@iitk.ac.in",
        packages=['bestPR'],
        install_requires=['scikit-learn'],
```

