# Comparing `tmp/qiskit_hangyul-0.4.0.tar.gz` & `tmp/qiskit_hangyul-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_hangyul-0.4.0.tar", last modified: Wed Jul 12 06:53:55 2023, max compression
+gzip compressed data, was "qiskit_hangyul-0.5.0.tar", last modified: Wed Jul 12 07:18:13 2023, max compression
```

## Comparing `qiskit_hangyul-0.4.0.tar` & `qiskit_hangyul-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-12 06:53:55.152935 qiskit_hangyul-0.4.0/
--rw-r--r--   0 hangyulson   (501) staff       (20)      334 2023-07-12 06:53:55.153030 qiskit_hangyul-0.4.0/PKG-INFO
--rw-r--r--   0 hangyulson   (501) staff       (20)       26 2023-04-08 21:37:34.000000 qiskit_hangyul-0.4.0/README.md
-drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-12 06:53:55.151823 qiskit_hangyul-0.4.0/qiskit_hangyul/
--rw-r--r--   0 hangyulson   (501) staff       (20)       54 2023-07-12 03:16:51.000000 qiskit_hangyul-0.4.0/qiskit_hangyul/__init__.py
--rw-r--r--   0 hangyulson   (501) staff       (20)     5019 2023-07-12 06:51:36.000000 qiskit_hangyul-0.4.0/qiskit_hangyul/quantier.py
-drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-12 06:53:55.152798 qiskit_hangyul-0.4.0/qiskit_hangyul.egg-info/
--rw-r--r--   0 hangyulson   (501) staff       (20)      334 2023-07-12 06:53:55.000000 qiskit_hangyul-0.4.0/qiskit_hangyul.egg-info/PKG-INFO
--rw-r--r--   0 hangyulson   (501) staff       (20)      271 2023-07-12 06:53:55.000000 qiskit_hangyul-0.4.0/qiskit_hangyul.egg-info/SOURCES.txt
--rw-r--r--   0 hangyulson   (501) staff       (20)        1 2023-07-12 06:53:55.000000 qiskit_hangyul-0.4.0/qiskit_hangyul.egg-info/dependency_links.txt
--rw-r--r--   0 hangyulson   (501) staff       (20)       18 2023-07-12 06:53:55.000000 qiskit_hangyul-0.4.0/qiskit_hangyul.egg-info/requires.txt
--rw-r--r--   0 hangyulson   (501) staff       (20)       15 2023-07-12 06:53:55.000000 qiskit_hangyul-0.4.0/qiskit_hangyul.egg-info/top_level.txt
--rw-r--r--   0 hangyulson   (501) staff       (20)       38 2023-07-12 06:53:55.153382 qiskit_hangyul-0.4.0/setup.cfg
--rw-r--r--   0 hangyulson   (501) staff       (20)      624 2023-07-12 06:53:46.000000 qiskit_hangyul-0.4.0/setup.py
+drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-12 07:18:13.486441 qiskit_hangyul-0.5.0/
+-rw-r--r--   0 hangyulson   (501) staff       (20)      334 2023-07-12 07:18:13.486501 qiskit_hangyul-0.5.0/PKG-INFO
+-rw-r--r--   0 hangyulson   (501) staff       (20)       26 2023-04-08 21:37:34.000000 qiskit_hangyul-0.5.0/README.md
+drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-12 07:18:13.485427 qiskit_hangyul-0.5.0/qiskit_hangyul/
+-rw-r--r--   0 hangyulson   (501) staff       (20)       55 2023-07-12 07:17:48.000000 qiskit_hangyul-0.5.0/qiskit_hangyul/__init__.py
+-rw-r--r--   0 hangyulson   (501) staff       (20)     5019 2023-07-12 06:51:36.000000 qiskit_hangyul-0.5.0/qiskit_hangyul/quantier.py
+drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-12 07:18:13.486331 qiskit_hangyul-0.5.0/qiskit_hangyul.egg-info/
+-rw-r--r--   0 hangyulson   (501) staff       (20)      334 2023-07-12 07:18:13.000000 qiskit_hangyul-0.5.0/qiskit_hangyul.egg-info/PKG-INFO
+-rw-r--r--   0 hangyulson   (501) staff       (20)      271 2023-07-12 07:18:13.000000 qiskit_hangyul-0.5.0/qiskit_hangyul.egg-info/SOURCES.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)        1 2023-07-12 07:18:13.000000 qiskit_hangyul-0.5.0/qiskit_hangyul.egg-info/dependency_links.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)       18 2023-07-12 07:18:13.000000 qiskit_hangyul-0.5.0/qiskit_hangyul.egg-info/requires.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)       15 2023-07-12 07:18:13.000000 qiskit_hangyul-0.5.0/qiskit_hangyul.egg-info/top_level.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)       38 2023-07-12 07:18:13.486751 qiskit_hangyul-0.5.0/setup.cfg
+-rw-r--r--   0 hangyulson   (501) staff       (20)      624 2023-07-12 07:17:58.000000 qiskit_hangyul-0.5.0/setup.py
```

### Comparing `qiskit_hangyul-0.4.0/qiskit_hangyul/quantier.py` & `qiskit_hangyul-0.5.0/qiskit_hangyul/quantier.py`

 * *Files identical despite different names*

### Comparing `qiskit_hangyul-0.4.0/setup.py` & `qiskit_hangyul-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qiskit_hangyul",
-    version="0.4.0",
+    version="0.5.0",
     description="A quantum provider for Qiskit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["qiskit_hangyul"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

