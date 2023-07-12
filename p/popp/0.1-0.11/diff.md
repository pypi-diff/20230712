# Comparing `tmp/popp-0.1.tar.gz` & `tmp/popp-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popp-0.1.tar", last modified: Wed Jul 12 03:00:46 2023, max compression
+gzip compressed data, was "popp-0.11.tar", last modified: Wed Jul 12 03:03:35 2023, max compression
```

## Comparing `popp-0.1.tar` & `popp-0.11.tar`

### file list

```diff
@@ -1,11 +1,19 @@
-drwxr-xr-x   0 hpc       (1000) hpc       (1000)        0 2023-07-12 03:00:46.964933 popp-0.1/
--rw-r--r--   0 hpc       (1000) hpc       (1000)       84 2023-07-12 02:54:32.000000 popp-0.1/MANIFEST.in
--rw-r--r--   0 hpc       (1000) hpc       (1000)      345 2023-07-12 03:00:46.964933 popp-0.1/PKG-INFO
--rwxrwxrwx   0 hpc       (1000) hpc       (1000)      155 2023-07-12 02:54:32.000000 popp-0.1/README.rst
-drwxr-xr-x   0 hpc       (1000) hpc       (1000)        0 2023-07-12 03:00:46.964933 popp-0.1/popp.egg-info/
--rw-r--r--   0 hpc       (1000) hpc       (1000)      345 2023-07-12 03:00:46.000000 popp-0.1/popp.egg-info/PKG-INFO
--rw-r--r--   0 hpc       (1000) hpc       (1000)      143 2023-07-12 03:00:46.000000 popp-0.1/popp.egg-info/SOURCES.txt
--rw-r--r--   0 hpc       (1000) hpc       (1000)        1 2023-07-12 03:00:46.000000 popp-0.1/popp.egg-info/dependency_links.txt
--rw-r--r--   0 hpc       (1000) hpc       (1000)        5 2023-07-12 03:00:46.000000 popp-0.1/popp.egg-info/top_level.txt
--rw-r--r--   0 hpc       (1000) hpc       (1000)       38 2023-07-12 03:00:46.964933 popp-0.1/setup.cfg
--rw-r--r--   0 hpc       (1000) hpc       (1000)     1474 2023-07-12 03:00:19.000000 popp-0.1/setup.py
+drwxr-xr-x   0 hpc       (1000) hpc       (1000)        0 2023-07-12 03:03:35.244908 popp-0.11/
+-rw-r--r--   0 hpc       (1000) hpc       (1000)       83 2023-07-12 03:02:52.000000 popp-0.11/MANIFEST.in
+-rw-r--r--   0 hpc       (1000) hpc       (1000)      346 2023-07-12 03:03:35.244908 popp-0.11/PKG-INFO
+-rwxrwxrwx   0 hpc       (1000) hpc       (1000)        5 2023-07-12 03:02:45.000000 popp-0.11/README.rst
+drwxr-xr-x   0 hpc       (1000) hpc       (1000)        0 2023-07-12 03:03:35.244908 popp-0.11/popp/
+-rw-r--r--   0 hpc       (1000) hpc       (1000)  1764572 2023-07-12 02:53:24.000000 popp-0.11/popp/Shortest-Path-Tour-Problem-with-Time-Windows-main.zip
+-rw-r--r--   0 hpc       (1000) hpc       (1000)   109441 2023-07-12 02:53:24.000000 popp-0.11/popp/The-label-correcting-algorithm-for-the-multi-objective-shortest-path-problem-main.zip
+-rw-r--r--   0 hpc       (1000) hpc       (1000)   466071 2023-07-12 02:53:23.000000 popp-0.11/popp/The-ripple-spreading-algorithm-for-the-fuzzy-multi-objective-path-optimization-problem-main.zip
+-rw-r--r--   0 hpc       (1000) hpc       (1000)   275979 2023-07-12 02:53:24.000000 popp-0.11/popp/The-shortest-path-problem-with-turn-restrictions-main.zip
+-rw-r--r--   0 hpc       (1000) hpc       (1000)    28658 2023-07-12 02:53:23.000000 popp-0.11/popp/public_emoa-main (1).zip
+-rw-r--r--   0 hpc       (1000) hpc       (1000)    25952 2023-07-12 02:53:23.000000 popp-0.11/popp/public_pymomapf-master.zip
+-rw-r--r--   0 hpc       (1000) hpc       (1000)   689338 2023-07-12 02:53:23.000000 popp-0.11/popp/s40747-022-00825-3.pdf
+drwxr-xr-x   0 hpc       (1000) hpc       (1000)        0 2023-07-12 03:03:35.244908 popp-0.11/popp.egg-info/
+-rw-r--r--   0 hpc       (1000) hpc       (1000)      346 2023-07-12 03:03:35.000000 popp-0.11/popp.egg-info/PKG-INFO
+-rw-r--r--   0 hpc       (1000) hpc       (1000)      547 2023-07-12 03:03:35.000000 popp-0.11/popp.egg-info/SOURCES.txt
+-rw-r--r--   0 hpc       (1000) hpc       (1000)        1 2023-07-12 03:03:35.000000 popp-0.11/popp.egg-info/dependency_links.txt
+-rw-r--r--   0 hpc       (1000) hpc       (1000)        5 2023-07-12 03:03:35.000000 popp-0.11/popp.egg-info/top_level.txt
+-rw-r--r--   0 hpc       (1000) hpc       (1000)       38 2023-07-12 03:03:35.244908 popp-0.11/setup.cfg
+-rw-r--r--   0 hpc       (1000) hpc       (1000)     1475 2023-07-12 03:03:32.000000 popp-0.11/setup.py
```

### Comparing `popp-0.1/setup.py` & `popp-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 setup(
     name='popp',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='0.1',
+    version='0.11',
 
     description='PPP',
     long_description='PPP',  #this is the
 
     # The project's main homepage.
 
     # Author details
```

