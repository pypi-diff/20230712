# Comparing `tmp/mauritstestpackage2-3.0.0a14.tar.gz` & `tmp/mauritstestpackage2-3.0.0a15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mauritstestpackage2-3.0.0a14.tar", last modified: Wed Jul 12 15:59:00 2023, max compression
+gzip compressed data, was "mauritstestpackage2-3.0.0a15.tar", last modified: Wed Jul 12 17:58:05 2023, max compression
```

## Comparing `mauritstestpackage2-3.0.0a14.tar` & `mauritstestpackage2-3.0.0a15.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:59:00.593475 mauritstestpackage2-3.0.0a14/
--rw-r--r--   0 maurits    (501) staff       (20)     4387 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       61 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     5181 2023-07-12 15:59:00.593663 mauritstestpackage2-3.0.0a14/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      104 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:59:00.591163 mauritstestpackage2-3.0.0a14/mauritstestpackage/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/mauritstestpackage/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:59:00.589337 mauritstestpackage2-3.0.0a14/mauritstestpackage/locales/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:59:00.589441 mauritstestpackage2-3.0.0a14/mauritstestpackage/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:59:00.591428 mauritstestpackage2-3.0.0a14/mauritstestpackage/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:59:00.593169 mauritstestpackage2-3.0.0a14/mauritstestpackage2.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     5181 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/mauritstestpackage2.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      362 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/mauritstestpackage2.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/mauritstestpackage2.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/mauritstestpackage2.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       19 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/mauritstestpackage2.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-12 15:59:00.594227 mauritstestpackage2-3.0.0a14/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1194 2023-07-12 15:59:00.000000 mauritstestpackage2-3.0.0a14/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 17:58:05.435141 mauritstestpackage2-3.0.0a15/
+-rw-r--r--   0 maurits    (501) staff       (20)     4457 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       61 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     5251 2023-07-12 17:58:05.435271 mauritstestpackage2-3.0.0a15/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      104 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 17:58:05.432609 mauritstestpackage2-3.0.0a15/mauritstestpackage/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/mauritstestpackage/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 17:58:05.430291 mauritstestpackage2-3.0.0a15/mauritstestpackage/locales/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 17:58:05.430397 mauritstestpackage2-3.0.0a15/mauritstestpackage/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 17:58:05.433198 mauritstestpackage2-3.0.0a15/mauritstestpackage/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 17:58:05.434811 mauritstestpackage2-3.0.0a15/mauritstestpackage2.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     5251 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/mauritstestpackage2.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      362 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/mauritstestpackage2.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/mauritstestpackage2.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/mauritstestpackage2.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       19 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/mauritstestpackage2.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-12 17:58:05.435665 mauritstestpackage2-3.0.0a15/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1194 2023-07-12 17:58:05.000000 mauritstestpackage2-3.0.0a15/setup.py
```

### Comparing `mauritstestpackage2-3.0.0a14/CHANGES.rst` & `mauritstestpackage2-3.0.0a15/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+3.0.0a15 (2023-07-12)
+---------------------
+
+- Nothing changed yet.
+
+
 3.0.0a14 (2023-07-12)
 ---------------------
 
 - Nothing changed yet.
 
 
 3.0.0a13 (2023-07-12)
```

### Comparing `mauritstestpackage2-3.0.0a14/PKG-INFO` & `mauritstestpackage2-3.0.0a15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mauritstestpackage2
-Version: 3.0.0a14
+Version: 3.0.0a15
 Summary: Test package from Maurits for uploading to PyPI.
 Home-page: https://github.com/mauritsvanrees/mauritstestpackage
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL
 Keywords: test release pypi
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,20 @@
 
 Maurits van Rees
 
 
 Changelog
 =========
 
+3.0.0a15 (2023-07-12)
+---------------------
+
+- Nothing changed yet.
+
+
 3.0.0a14 (2023-07-12)
 ---------------------
 
 - Nothing changed yet.
 
 
 3.0.0a13 (2023-07-12)
```

### Comparing `mauritstestpackage2-3.0.0a14/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po` & `mauritstestpackage2-3.0.0a15/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po`

 * *Files identical despite different names*

### Comparing `mauritstestpackage2-3.0.0a14/mauritstestpackage2.egg-info/PKG-INFO` & `mauritstestpackage2-3.0.0a15/mauritstestpackage2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mauritstestpackage2
-Version: 3.0.0a14
+Version: 3.0.0a15
 Summary: Test package from Maurits for uploading to PyPI.
 Home-page: https://github.com/mauritsvanrees/mauritstestpackage
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL
 Keywords: test release pypi
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,20 @@
 
 Maurits van Rees
 
 
 Changelog
 =========
 
+3.0.0a15 (2023-07-12)
+---------------------
+
+- Nothing changed yet.
+
+
 3.0.0a14 (2023-07-12)
 ---------------------
 
 - Nothing changed yet.
 
 
 3.0.0a13 (2023-07-12)
```

### Comparing `mauritstestpackage2-3.0.0a14/setup.py` & `mauritstestpackage2-3.0.0a15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "3.0.0a14"
+version = "3.0.0a15"
 
 setup(
     name="mauritstestpackage2",
     version=version,
     description="Test package from Maurits for uploading to PyPI.",
     long_description=(open("README.rst").read() + "\n\n" + open("CHANGES.rst").read()),
     # Get strings from https://pypi.org/classifiers/
```

