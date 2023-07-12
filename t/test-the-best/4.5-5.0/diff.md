# Comparing `tmp/test_the_best-4.5.tar.gz` & `tmp/test_the_best-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_the_best-4.5.tar", last modified: Tue Jul 11 16:12:44 2023, max compression
+gzip compressed data, was "test_the_best-5.0.tar", last modified: Wed Jul 12 10:39:41 2023, max compression
```

## Comparing `test_the_best-4.5.tar` & `test_the_best-5.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 16:12:44.124621 test_the_best-4.5/
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-11 16:09:10.000000 test_the_best-4.5/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      321 2023-07-11 16:12:44.124621 test_the_best-4.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      131 2023-07-11 16:03:59.000000 test_the_best-4.5/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-11 16:12:44.124621 test_the_best-4.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      433 2023-07-11 16:09:39.000000 test_the_best-4.5/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 16:12:44.120620 test_the_best-4.5/test_the_best/
--rw-r--r--   0 runner    (1000) runner    (1000)      471 2023-07-11 15:45:02.000000 test_the_best-4.5/test_the_best/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-11 16:12:44.124621 test_the_best-4.5/test_the_best.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      321 2023-07-11 16:12:43.000000 test_the_best-4.5/test_the_best.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      246 2023-07-11 16:12:43.000000 test_the_best-4.5/test_the_best.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 16:12:43.000000 test_the_best-4.5/test_the_best.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-4.5/test_the_best.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-11 16:12:43.000000 test_the_best-4.5/test_the_best.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 10:39:41.838867 test_the_best-5.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-11 16:09:10.000000 test_the_best-5.0/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-12 10:36:56.000000 test_the_best-5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)      454 2023-07-12 10:39:41.838867 test_the_best-5.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      131 2023-07-11 16:03:59.000000 test_the_best-5.0/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-12 10:39:41.838867 test_the_best-5.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      457 2023-07-12 10:37:11.000000 test_the_best-5.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 10:39:41.838867 test_the_best-5.0/test_the_best/
+-rw-r--r--   0 runner    (1000) runner    (1000)      471 2023-07-11 15:45:02.000000 test_the_best-5.0/test_the_best/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 10:39:41.838867 test_the_best-5.0/test_the_best.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      454 2023-07-12 10:39:41.000000 test_the_best-5.0/test_the_best.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      258 2023-07-12 10:39:41.000000 test_the_best-5.0/test_the_best.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 10:39:41.000000 test_the_best-5.0/test_the_best.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-11 14:16:45.000000 test_the_best-5.0/test_the_best.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-07-12 10:39:41.000000 test_the_best-5.0/test_the_best.egg-info/top_level.txt
```

### Comparing `test_the_best-4.5/LICENSE` & `test_the_best-5.0/LICENSE`

 * *Files identical despite different names*

