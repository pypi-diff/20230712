# Comparing `tmp/pymulticore-0.1.1.tar.gz` & `tmp/pymulticore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymulticore-0.1.1.tar", last modified: Wed Jul 12 00:46:45 2023, max compression
+gzip compressed data, was "pymulticore-0.1.3.tar", last modified: Wed Jul 12 01:03:37 2023, max compression
```

## Comparing `pymulticore-0.1.1.tar` & `pymulticore-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 00:46:45.801000 pymulticore-0.1.1/
--rw-rw-rw-   0        0        0      200 2023-07-12 00:46:45.794000 pymulticore-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-08 18:57:14.000000 pymulticore-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 00:46:45.728000 pymulticore-0.1.1/pymulticore/
--rw-rw-rw-   0        0        0       26 2023-07-09 15:44:29.000000 pymulticore-0.1.1/pymulticore/__init__.py
--rw-rw-rw-   0        0        0    14335 2023-07-11 16:31:20.000000 pymulticore-0.1.1/pymulticore/pymulticore.py
-drwxrwxrwx   0        0        0        0 2023-07-12 00:46:45.785000 pymulticore-0.1.1/pymulticore.egg-info/
--rw-rw-rw-   0        0        0      200 2023-07-12 00:46:45.000000 pymulticore-0.1.1/pymulticore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-12 00:46:45.000000 pymulticore-0.1.1/pymulticore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 00:46:45.000000 pymulticore-0.1.1/pymulticore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 00:46:45.000000 pymulticore-0.1.1/pymulticore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 00:46:45.000000 pymulticore-0.1.1/pymulticore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 00:46:45.799000 pymulticore-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      420 2023-07-11 16:34:22.000000 pymulticore-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:03:37.186000 pymulticore-0.1.3/
+-rw-rw-rw-   0        0        0     2663 2023-07-12 01:03:37.178000 pymulticore-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2418 2023-07-12 01:01:48.000000 pymulticore-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 01:03:37.110000 pymulticore-0.1.3/pymulticore/
+-rw-rw-rw-   0        0        0       26 2023-07-09 15:44:29.000000 pymulticore-0.1.3/pymulticore/__init__.py
+-rw-rw-rw-   0        0        0    14335 2023-07-11 16:31:20.000000 pymulticore-0.1.3/pymulticore/pymulticore.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:03:37.169000 pymulticore-0.1.3/pymulticore.egg-info/
+-rw-rw-rw-   0        0        0     2663 2023-07-12 01:03:36.000000 pymulticore-0.1.3/pymulticore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-12 01:03:37.000000 pymulticore-0.1.3/pymulticore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 01:03:36.000000 pymulticore-0.1.3/pymulticore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 01:03:36.000000 pymulticore-0.1.3/pymulticore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 01:03:36.000000 pymulticore-0.1.3/pymulticore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 01:03:37.184000 pymulticore-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-07-12 01:02:31.000000 pymulticore-0.1.3/setup.py
```

### Comparing `pymulticore-0.1.1/pymulticore/pymulticore.py` & `pymulticore-0.1.3/pymulticore/pymulticore.py`

 * *Files identical despite different names*

