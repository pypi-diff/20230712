# Comparing `tmp/pyexifwrangle-0.1.0.tar.gz` & `tmp/pyexifwrangle-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyexifwrangle-0.1.0.tar", last modified: Wed Jul  5 14:17:05 2023, max compression
+gzip compressed data, was "dist/pyexifwrangle-0.1.1.tar", last modified: Wed Jul 12 18:35:05 2023, max compression
```

## Comparing `pyexifwrangle-0.1.0.tar` & `pyexifwrangle-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/
--rw-r--r--   0 stephanie   (501) staff       (20)      589 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/PKG-INFO
--rw-r--r--   0 stephanie   (501) staff       (20)      609 2023-07-03 15:33:11.000000 pyexifwrangle-0.1.0/README.md
-drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/pyexifwrangle/
--rw-r--r--   0 stephanie   (501) staff       (20)      131 2023-07-05 14:05:22.000000 pyexifwrangle-0.1.0/pyexifwrangle/__init__.py
--rw-r--r--   0 stephanie   (501) staff       (20)     4155 2023-07-03 21:11:13.000000 pyexifwrangle-0.1.0/pyexifwrangle/wrangle.py
-drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/pyexifwrangle.egg-info/
--rw-r--r--   0 stephanie   (501) staff       (20)      589 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/pyexifwrangle.egg-info/PKG-INFO
--rw-r--r--   0 stephanie   (501) staff       (20)      253 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/pyexifwrangle.egg-info/SOURCES.txt
--rw-r--r--   0 stephanie   (501) staff       (20)        1 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/pyexifwrangle.egg-info/dependency_links.txt
--rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/pyexifwrangle.egg-info/requires.txt
--rw-r--r--   0 stephanie   (501) staff       (20)       14 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/pyexifwrangle.egg-info/top_level.txt
--rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-05 14:17:05.000000 pyexifwrangle-0.1.0/setup.cfg
--rw-r--r--   0 stephanie   (501) staff       (20)      915 2023-07-05 13:58:25.000000 pyexifwrangle-0.1.0/setup.py
+drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/
+-rw-r--r--   0 stephanie   (501) staff       (20)      589 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/PKG-INFO
+-rw-r--r--   0 stephanie   (501) staff       (20)      609 2023-07-03 15:33:11.000000 pyexifwrangle-0.1.1/README.md
+drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle/
+-rw-r--r--   0 stephanie   (501) staff       (20)      132 2023-07-12 18:27:14.000000 pyexifwrangle-0.1.1/pyexifwrangle/__init__.py
+-rw-r--r--   0 stephanie   (501) staff       (20)     2690 2023-07-12 18:15:44.000000 pyexifwrangle-0.1.1/pyexifwrangle/wrangle.py
+drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/
+-rw-r--r--   0 stephanie   (501) staff       (20)      589 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/PKG-INFO
+-rw-r--r--   0 stephanie   (501) staff       (20)      253 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/SOURCES.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)        1 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/dependency_links.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/requires.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)       14 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/pyexifwrangle.egg-info/top_level.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-12 18:35:05.000000 pyexifwrangle-0.1.1/setup.cfg
+-rw-r--r--   0 stephanie   (501) staff       (20)      915 2023-07-05 13:58:25.000000 pyexifwrangle-0.1.1/setup.py
```

### Comparing `pyexifwrangle-0.1.0/PKG-INFO` & `pyexifwrangle-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyexifwrangle
-Version: 0.1.0
+Version: 0.1.1
 Summary: A helper package for wrangling image EXIF data
 Home-page: https://github.com/stephaniereinders/pyexifwrangle
 Author: Stephanie Reinders
 Author-email: reinders.stephanie@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyexifwrangle-0.1.0/README.md` & `pyexifwrangle-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyexifwrangle-0.1.0/pyexifwrangle.egg-info/PKG-INFO` & `pyexifwrangle-0.1.1/pyexifwrangle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyexifwrangle
-Version: 0.1.0
+Version: 0.1.1
 Summary: A helper package for wrangling image EXIF data
 Home-page: https://github.com/stephaniereinders/pyexifwrangle
 Author: Stephanie Reinders
 Author-email: reinders.stephanie@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyexifwrangle-0.1.0/setup.py` & `pyexifwrangle-0.1.1/setup.py`

 * *Files identical despite different names*

