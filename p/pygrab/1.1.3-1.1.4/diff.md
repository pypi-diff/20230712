# Comparing `tmp/pygrab-1.1.3.tar.gz` & `tmp/pygrab-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-1.1.3.tar", last modified: Tue Jul 11 01:45:42 2023, max compression
+gzip compressed data, was "pygrab-1.1.4.tar", last modified: Wed Jul 12 02:26:43 2023, max compression
```

## Comparing `pygrab-1.1.3.tar` & `pygrab-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 01:45:42.476000 pygrab-1.1.3/
--rw-rw-rw-   0        0        0      183 2023-07-11 01:45:42.468000 pygrab-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 01:45:42.405000 pygrab-1.1.3/pygrab/
--rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.3/pygrab/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-07-07 04:12:12.000000 pygrab-1.1.3/pygrab/proxylist.py
--rw-rw-rw-   0        0        0    16578 2023-07-11 01:42:55.000000 pygrab-1.1.3/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-07-11 01:45:42.461000 pygrab-1.1.3/pygrab.egg-info/
--rw-rw-rw-   0        0        0      183 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 01:45:42.000000 pygrab-1.1.3/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 01:45:42.474000 pygrab-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      338 2023-07-11 01:43:23.000000 pygrab-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:26:43.621000 pygrab-1.1.4/
+-rw-rw-rw-   0        0        0     2163 2023-07-12 02:26:43.614000 pygrab-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1937 2023-07-12 02:15:21.000000 pygrab-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 02:26:43.550000 pygrab-1.1.4/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.4/pygrab/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-07-07 04:12:12.000000 pygrab-1.1.4/pygrab/proxylist.py
+-rw-rw-rw-   0        0        0    16578 2023-07-11 01:42:55.000000 pygrab-1.1.4/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:26:43.605000 pygrab-1.1.4/pygrab.egg-info/
+-rw-rw-rw-   0        0        0     2163 2023-07-12 02:26:43.000000 pygrab-1.1.4/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-12 02:26:43.000000 pygrab-1.1.4/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 02:26:43.000000 pygrab-1.1.4/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-12 02:26:43.000000 pygrab-1.1.4/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 02:26:43.000000 pygrab-1.1.4/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 02:26:43.619000 pygrab-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      616 2023-07-12 02:23:19.000000 pygrab-1.1.4/setup.py
```

### Comparing `pygrab-1.1.3/pygrab/proxylist.py` & `pygrab-1.1.4/pygrab/proxylist.py`

 * *Files identical despite different names*

### Comparing `pygrab-1.1.3/pygrab/pygrab.py` & `pygrab-1.1.4/pygrab/pygrab.py`

 * *Files identical despite different names*

