# Comparing `tmp/pubpypack-harmony-lawrence-laugesen-0.0.1.tar.gz` & `tmp/pubpypack-harmony-lawrence-laugesen-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubpypack-harmony-lawrence-laugesen-0.0.1.tar", last modified: Tue Jul 11 11:11:25 2023, max compression
+gzip compressed data, was "pubpypack-harmony-lawrence-laugesen-0.0.2.tar", last modified: Wed Jul 12 10:47:27 2023, max compression
```

## Comparing `pubpypack-harmony-lawrence-laugesen-0.0.1.tar` & `pubpypack-harmony-lawrence-laugesen-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 lawrencelaugesen   (501) staff       (20)        0 2023-07-11 11:11:25.529557 pubpypack-harmony-lawrence-laugesen-0.0.1/
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)       50 2023-06-21 10:51:07.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/MANIFEST.in
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      496 2023-07-11 11:11:25.529770 pubpypack-harmony-lawrence-laugesen-0.0.1/PKG-INFO
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      133 2023-06-20 11:43:09.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/README.md
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      131 2023-07-03 21:00:40.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/pyproject.toml
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)     1684 2023-07-11 11:11:25.531430 pubpypack-harmony-lawrence-laugesen-0.0.1/setup.cfg
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      175 2023-06-27 12:01:44.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/setup.py
-drwxr-xr-x   0 lawrencelaugesen   (501) staff       (20)        0 2023-07-11 11:11:25.516906 pubpypack-harmony-lawrence-laugesen-0.0.1/src/
-drwxr-xr-x   0 lawrencelaugesen   (501) staff       (20)        0 2023-07-11 11:11:25.522105 pubpypack-harmony-lawrence-laugesen-0.0.1/src/first_python_package.egg-info/
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      441 2023-07-10 10:56:07.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/first_python_package.egg-info/PKG-INFO
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      579 2023-07-10 10:56:07.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/first_python_package.egg-info/SOURCES.txt
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)        1 2023-07-10 10:56:07.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/first_python_package.egg-info/dependency_links.txt
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)       47 2023-07-10 10:56:07.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/first_python_package.egg-info/entry_points.txt
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)       20 2023-07-10 10:56:07.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/first_python_package.egg-info/requires.txt
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)        6 2023-07-10 10:56:07.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/first_python_package.egg-info/top_level.txt
-drwxr-xr-x   0 lawrencelaugesen   (501) staff       (20)        0 2023-07-11 11:11:25.525404 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)        0 2023-06-21 10:24:26.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/__init__.py
-drwxr-xr-x   0 lawrencelaugesen   (501) staff       (20)        0 2023-07-11 11:11:25.525725 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/__pycache__/
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      452 2023-06-26 11:42:09.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/__pycache__/harmonic_mean.cpython-310.pyc
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)        0 2023-06-21 10:42:19.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/data.json
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)   198761 2023-06-26 11:43:09.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/harmonic_mean.c
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)       77 2023-06-26 11:42:44.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/harmonic_mean.pyx
--rwxr-xr-x   0 lawrencelaugesen   (501) staff       (20)      700 2023-07-10 10:55:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/harmony.py
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)        0 2023-06-21 10:24:36.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/hello.py
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)        0 2023-07-03 20:23:55.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/py.typed
-drwxr-xr-x   0 lawrencelaugesen   (501) staff       (20)        0 2023-07-11 11:11:25.528552 pubpypack-harmony-lawrence-laugesen-0.0.1/src/pubpypack_harmony_lawrence_laugesen.egg-info/
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      496 2023-07-11 11:11:25.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/pubpypack_harmony_lawrence_laugesen.egg-info/PKG-INFO
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      959 2023-07-11 11:11:25.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/pubpypack_harmony_lawrence_laugesen.egg-info/SOURCES.txt
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)        1 2023-07-11 11:11:25.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/pubpypack_harmony_lawrence_laugesen.egg-info/dependency_links.txt
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)       47 2023-07-11 11:11:25.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/pubpypack_harmony_lawrence_laugesen.egg-info/entry_points.txt
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)       20 2023-07-11 11:11:25.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/pubpypack_harmony_lawrence_laugesen.egg-info/requires.txt
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)        6 2023-07-11 11:11:25.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/src/pubpypack_harmony_lawrence_laugesen.egg-info/top_level.txt
-drwxr-xr-x   0 lawrencelaugesen   (501) staff       (20)        0 2023-07-11 11:11:25.529067 pubpypack-harmony-lawrence-laugesen-0.0.1/test/
--rw-r--r--   0 lawrencelaugesen   (501) staff       (20)      467 2023-07-10 10:56:05.000000 pubpypack-harmony-lawrence-laugesen-0.0.1/test/test_harmonic_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:27.277079 pubpypack-harmony-lawrence-laugesen-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-12 10:47:27.277079 pubpypack-harmony-lawrence-laugesen-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-12 10:47:27.281079 pubpypack-harmony-lawrence-laugesen-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:27.269079 pubpypack-harmony-lawrence-laugesen-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:27.273079 pubpypack-harmony-lawrence-laugesen-0.0.2/src/first_python_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/first_python_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/first_python_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/first_python_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/first_python_package.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/first_python_package.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/first_python_package.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:27.277079 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:27.277079 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/__pycache__/harmonic_mean.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)   198761 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/harmonic_mean.c
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/harmonic_mean.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/harmony.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:27.277079 pubpypack-harmony-lawrence-laugesen-0.0.2/src/pubpypack_harmony_lawrence_laugesen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-12 10:47:27.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/pubpypack_harmony_lawrence_laugesen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-12 10:47:27.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/pubpypack_harmony_lawrence_laugesen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:47:27.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/pubpypack_harmony_lawrence_laugesen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 10:47:27.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/pubpypack_harmony_lawrence_laugesen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 10:47:27.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/pubpypack_harmony_lawrence_laugesen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 10:47:27.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/src/pubpypack_harmony_lawrence_laugesen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:47:27.277079 pubpypack-harmony-lawrence-laugesen-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-12 10:47:12.000000 pubpypack-harmony-lawrence-laugesen-0.0.2/test/test_harmonic_mean.py
```

### Comparing `pubpypack-harmony-lawrence-laugesen-0.0.1/setup.cfg` & `pubpypack-harmony-lawrence-laugesen-0.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pubpypack-harmony-lawrence-laugesen
-version = 0.0.1
+version = 0.0.2
 author = Laugesen
 author_email = "Laugesen" <laugesen@email.com>
 url = https://github.com/laugesen11/first_python_package
 description = This package is silly
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

### Comparing `pubpypack-harmony-lawrence-laugesen-0.0.1/src/first_python_package.egg-info/SOURCES.txt` & `pubpypack-harmony-lawrence-laugesen-0.0.2/src/first_python_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/harmonic_mean.c` & `pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/harmonic_mean.c`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-lawrence-laugesen-0.0.1/src/impkg/harmony.py` & `pubpypack-harmony-lawrence-laugesen-0.0.2/src/impkg/harmony.py`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-lawrence-laugesen-0.0.1/src/pubpypack_harmony_lawrence_laugesen.egg-info/SOURCES.txt` & `pubpypack-harmony-lawrence-laugesen-0.0.2/src/pubpypack_harmony_lawrence_laugesen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

