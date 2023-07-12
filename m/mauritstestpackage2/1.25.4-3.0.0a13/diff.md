# Comparing `tmp/mauritstestpackage2-1.25.4.tar.gz` & `tmp/mauritstestpackage2-3.0.0a13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mauritstestpackage2-1.25.4.tar", last modified: Thu Sep  3 21:45:47 2020, max compression
+gzip compressed data, was "mauritstestpackage2-3.0.0a13.tar", last modified: Wed Jul 12 15:22:20 2023, max compression
```

## Comparing `mauritstestpackage2-1.25.4.tar` & `mauritstestpackage2-3.0.0a13.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/
--rw-r--r--   0 maurits    (501) staff       (20)     7522 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       65 2020-09-03 21:45:46.000000 mauritstestpackage2-1.25.4/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage/locales/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      554 2020-09-03 21:45:46.000000 mauritstestpackage2-1.25.4/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.mo
--rw-r--r--   0 maurits    (501) staff       (20)      767 2020-09-03 21:45:46.000000 mauritstestpackage2-1.25.4/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po
--rw-r--r--   0 maurits    (501) staff       (20)        2 2020-09-03 21:45:46.000000 mauritstestpackage2-1.25.4/mauritstestpackage/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1192 2020-09-03 21:45:46.000000 mauritstestpackage2-1.25.4/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      116 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/setup.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage2.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     7522 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage2.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage2.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      472 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage2.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)       37 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage2.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       19 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage2.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-09-03 21:45:47.000000 mauritstestpackage2-1.25.4/mauritstestpackage2.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      104 2020-09-03 21:45:46.000000 mauritstestpackage2-1.25.4/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3811 2020-09-03 21:45:46.000000 mauritstestpackage2-1.25.4/CHANGES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:22:20.948989 mauritstestpackage2-3.0.0a13/
+-rw-r--r--   0 maurits    (501) staff       (20)     4317 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     5111 2023-07-12 15:22:20.949112 mauritstestpackage2-3.0.0a13/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      104 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:22:20.946521 mauritstestpackage2-3.0.0a13/mauritstestpackage/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/mauritstestpackage/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:22:20.944236 mauritstestpackage2-3.0.0a13/mauritstestpackage/locales/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:22:20.944379 mauritstestpackage2-3.0.0a13/mauritstestpackage/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:22:20.946824 mauritstestpackage2-3.0.0a13/mauritstestpackage/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 15:22:20.948632 mauritstestpackage2-3.0.0a13/mauritstestpackage2.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     5111 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/mauritstestpackage2.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      362 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/mauritstestpackage2.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/mauritstestpackage2.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/mauritstestpackage2.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       19 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/mauritstestpackage2.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-12 15:22:20.949510 mauritstestpackage2-3.0.0a13/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1194 2023-07-12 15:22:20.000000 mauritstestpackage2-3.0.0a13/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mauritstestpackage2-1.25.4/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po` & `mauritstestpackage2-3.0.0a13/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po`

 * *Files identical despite different names*

### Comparing `mauritstestpackage2-1.25.4/setup.py` & `mauritstestpackage2-3.0.0a13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "1.25.4"
+version = "3.0.0a13"
 
 setup(
     name="mauritstestpackage2",
     version=version,
     description="Test package from Maurits for uploading to PyPI.",
     long_description=(open("README.rst").read() + "\n\n" + open("CHANGES.rst").read()),
     # Get strings from https://pypi.org/classifiers/
```

### Comparing `mauritstestpackage2-1.25.4/CHANGES.rst` & `mauritstestpackage2-3.0.0a13/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,52 @@
 Changelog
 =========
 
+3.0.0a13 (2023-07-12)
+---------------------
+
+- Nothing changed yet.
+
+
+3.0.0a12 (2022-12-09)
+---------------------
+
+- Nothing changed yet.
+
+
+3.0.0a11 (2022-03-15)
+---------------------
+
+- Nothing changed yet.
+
+
+3.0.0a10 (2022-02-10)
+---------------------
+
+- Nothing changed yet.
+
+
+3.0.0a9 (2021-11-01)
+--------------------
+
+- Nothing changed yet.
+
+
+3.0.0-alpha.8 (2021-10-29)
+--------------------------
+
+- Nothing changed yet.
+
+
+3.0.0-alpha7 (2021-10-29)
+-------------------------
+
+- Nothing changed yet.
+
+
 1.25.4 (2020-09-03)
 -------------------
 
 - Nothing changed yet.
 
 
 1.25.3 (2020-08-07)
```

