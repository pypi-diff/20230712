# Comparing `tmp/saracendb-0.1.tar.gz` & `tmp/saracendb-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saracendb-0.1.tar", last modified: Tue Jul 11 15:08:45 2023, max compression
+gzip compressed data, was "saracendb-1.0.tar", last modified: Wed Jul 12 14:19:17 2023, max compression
```

## Comparing `saracendb-0.1.tar` & `saracendb-1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:08:45.712320 saracendb-0.1/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      552 2023-07-11 15:08:45.712176 saracendb-0.1/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      125 2023-07-11 14:51:10.000000 saracendb-0.1/README.md
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:08:45.711159 saracendb-0.1/saracendb/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 14:52:10.000000 saracendb-0.1/saracendb/__init__.py
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     1674 2023-07-11 14:51:30.000000 saracendb-0.1/saracendb/main.py
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:08:45.711967 saracendb-0.1/saracendb.egg-info/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      552 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      222 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/SOURCES.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/dependency_links.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        8 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/requires.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/top_level.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-11 15:08:45.712364 saracendb-0.1/setup.cfg
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      914 2023-07-11 15:06:06.000000 saracendb-0.1/setup.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:19:17.450934 saracendb-1.0/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      444 2023-07-12 14:19:17.450802 saracendb-1.0/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       17 2023-07-12 14:19:13.000000 saracendb-1.0/README.md
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:19:17.450521 saracendb-1.0/saracendb.egg-info/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      444 2023-07-12 14:19:17.000000 saracendb-1.0/saracendb.egg-info/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      209 2023-07-12 14:19:17.000000 saracendb-1.0/saracendb.egg-info/SOURCES.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-12 14:19:17.000000 saracendb-1.0/saracendb.egg-info/dependency_links.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      113 2023-07-12 14:19:17.000000 saracendb-1.0/saracendb.egg-info/requires.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-12 14:19:17.000000 saracendb-1.0/saracendb.egg-info/top_level.txt
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:19:17.450645 saracendb-1.0/saracenpypacks/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:08:37.000000 saracendb-1.0/saracenpypacks/__init__.py
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-12 14:19:17.450969 saracendb-1.0/setup.cfg
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      990 2023-07-12 14:17:24.000000 saracendb-1.0/setup.py
```

### Comparing `saracendb-0.1/setup.py` & `saracendb-1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from setuptools import setup, find_packages
 import codecs
+import json
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1'
+with open("packages.json", "r") as f:
+    packages = json.load(f)
+
+VERSION = '1.0'
 DESCRIPTION = ''
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="saracendb",
     version=VERSION,
     author="Saracen Rhue",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['pymongo'],
+    install_requires=packages,
     keywords=['python', 'db'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

