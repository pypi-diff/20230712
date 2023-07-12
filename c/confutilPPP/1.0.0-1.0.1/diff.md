# Comparing `tmp/confutilPPP-1.0.0.tar.gz` & `tmp/confutilPPP-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confutilPPP-1.0.0.tar", last modified: Tue Jul 11 17:29:03 2023, max compression
+gzip compressed data, was "confutilPPP-1.0.1.tar", last modified: Wed Jul 12 11:12:32 2023, max compression
```

## Comparing `confutilPPP-1.0.0.tar` & `confutilPPP-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:29:03.665279 confutilPPP-1.0.0/
--rw-rw-rw-   0        0        0      157 2023-07-11 17:29:03.664282 confutilPPP-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 17:29:03.655306 confutilPPP-1.0.0/confutilPPP/
--rw-rw-rw-   0        0        0      171 2023-07-11 08:18:03.000000 confutilPPP-1.0.0/confutilPPP/__init__.py
--rw-rw-rw-   0        0        0     2154 2023-07-11 17:14:17.000000 confutilPPP-1.0.0/confutilPPP/confutil.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:29:03.663285 confutilPPP-1.0.0/confutilPPP.egg-info/
--rw-rw-rw-   0        0        0      157 2023-07-11 17:29:03.000000 confutilPPP-1.0.0/confutilPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-07-11 17:29:03.000000 confutilPPP-1.0.0/confutilPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:29:03.000000 confutilPPP-1.0.0/confutilPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-11 17:29:03.000000 confutilPPP-1.0.0/confutilPPP.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 17:29:03.000000 confutilPPP-1.0.0/confutilPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 17:29:03.665279 confutilPPP-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-07-11 17:27:59.000000 confutilPPP-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:12:32.641007 confutilPPP-1.0.1/
+-rw-rw-rw-   0        0        0      157 2023-07-12 11:12:32.640007 confutilPPP-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2023-07-11 17:32:43.000000 confutilPPP-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 11:12:32.635449 confutilPPP-1.0.1/confutilPPP.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:12:32.641007 confutilPPP-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-07-12 10:58:48.000000 confutilPPP-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:12:32.628468 confutilPPP-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 11:12:32.638441 confutilPPP-1.0.1/src/confutilPPP/
+-rw-rw-rw-   0        0        0      203 2023-07-12 10:57:03.000000 confutilPPP-1.0.1/src/confutilPPP/__init__.py
+-rw-rw-rw-   0        0        0     2154 2023-07-11 17:14:17.000000 confutilPPP-1.0.1/src/confutilPPP/_confutil.py
```

### Comparing `confutilPPP-1.0.0/confutilPPP/confutil.py` & `confutilPPP-1.0.1/src/confutilPPP/_confutil.py`

 * *Files identical despite different names*

