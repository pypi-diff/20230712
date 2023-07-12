# Comparing `tmp/upload-to-pypi-0.0.1.tar.gz` & `tmp/upload-to-pypi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upload-to-pypi-0.0.1.tar", last modified: Mon Jul 10 21:40:34 2023, max compression
+gzip compressed data, was "upload-to-pypi-0.0.2.tar", last modified: Wed Jul 12 19:55:10 2023, max compression
```

## Comparing `upload-to-pypi-0.0.1.tar` & `upload-to-pypi-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 ramgokul   (504) staff       (20)        0 2023-07-10 21:40:34.844790 upload-to-pypi-0.0.1/
--rw-r--r--   0 ramgokul   (504) staff       (20)      322 2023-07-10 21:40:34.844625 upload-to-pypi-0.0.1/PKG-INFO
--rw-r--r--   0 ramgokul   (504) staff       (20)        0 2023-07-10 21:38:04.000000 upload-to-pypi-0.0.1/README.md
--rw-r--r--   0 ramgokul   (504) staff       (20)       38 2023-07-10 21:40:34.844833 upload-to-pypi-0.0.1/setup.cfg
--rw-r--r--   0 ramgokul   (504) staff       (20)      587 2023-07-10 21:39:43.000000 upload-to-pypi-0.0.1/setup.py
-drwxr-xr-x   0 ramgokul   (504) staff       (20)        0 2023-07-10 21:40:34.844397 upload-to-pypi-0.0.1/upload_to_pypi.egg-info/
--rw-r--r--   0 ramgokul   (504) staff       (20)      322 2023-07-10 21:40:34.000000 upload-to-pypi-0.0.1/upload_to_pypi.egg-info/PKG-INFO
--rw-r--r--   0 ramgokul   (504) staff       (20)      170 2023-07-10 21:40:34.000000 upload-to-pypi-0.0.1/upload_to_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 ramgokul   (504) staff       (20)        1 2023-07-10 21:40:34.000000 upload-to-pypi-0.0.1/upload_to_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 ramgokul   (504) staff       (20)        1 2023-07-10 21:40:34.000000 upload-to-pypi-0.0.1/upload_to_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 ramgokul   (504) staff       (20)        0 2023-07-12 19:55:10.356644 upload-to-pypi-0.0.2/
+-rw-r--r--   0 ramgokul   (504) staff       (20)      322 2023-07-12 19:55:10.356500 upload-to-pypi-0.0.2/PKG-INFO
+-rw-r--r--   0 ramgokul   (504) staff       (20)        0 2023-07-10 21:38:04.000000 upload-to-pypi-0.0.2/README.md
+-rw-r--r--   0 ramgokul   (504) staff       (20)       38 2023-07-12 19:55:10.356691 upload-to-pypi-0.0.2/setup.cfg
+-rw-r--r--   0 ramgokul   (504) staff       (20)      587 2023-07-12 19:54:12.000000 upload-to-pypi-0.0.2/setup.py
+drwxr-xr-x   0 ramgokul   (504) staff       (20)        0 2023-07-12 19:55:10.356307 upload-to-pypi-0.0.2/upload_to_pypi.egg-info/
+-rw-r--r--   0 ramgokul   (504) staff       (20)      322 2023-07-12 19:55:10.000000 upload-to-pypi-0.0.2/upload_to_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 ramgokul   (504) staff       (20)      170 2023-07-12 19:55:10.000000 upload-to-pypi-0.0.2/upload_to_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 ramgokul   (504) staff       (20)        1 2023-07-12 19:55:10.000000 upload-to-pypi-0.0.2/upload_to_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 ramgokul   (504) staff       (20)        1 2023-07-12 19:55:10.000000 upload-to-pypi-0.0.2/upload_to_pypi.egg-info/top_level.txt
```

### Comparing `upload-to-pypi-0.0.1/setup.py` & `upload-to-pypi-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setuptools.setup(
     name="upload-to-pypi",
-    version="0.0.1",
+    version="0.0.2",
     author="pypi-tester-14",
     description="test",
     long_description="test",
     long_description_content_type="text/markdown",
     url="",
     classifiers=[
         "Programming Language :: Python :: 3",
```

