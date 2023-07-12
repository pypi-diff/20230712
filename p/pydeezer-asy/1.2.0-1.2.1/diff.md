# Comparing `tmp/pydeezer_asy-1.2.0.tar.gz` & `tmp/pydeezer_asy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeezer_asy-1.2.0.tar", last modified: Wed Jul 12 11:20:39 2023, max compression
+gzip compressed data, was "pydeezer_asy-1.2.1.tar", last modified: Wed Jul 12 12:56:22 2023, max compression
```

## Comparing `pydeezer_asy-1.2.0.tar` & `pydeezer_asy-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:20:39.785443 pydeezer_asy-1.2.0/
--rw-rw-rw-   0        0        0      230 2023-07-12 11:20:39.785443 pydeezer_asy-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 11:20:39.725358 pydeezer_asy-1.2.0/deezer_asy/
--rw-rw-rw-   0        0        0    30354 2023-07-12 11:17:17.000000 pydeezer_asy-1.2.0/deezer_asy/DeezerAsy.py
--rw-rw-rw-   0        0        0      134 2023-07-07 16:55:48.000000 pydeezer_asy-1.2.0/deezer_asy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:20:39.744308 pydeezer_asy-1.2.0/deezer_asy/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/exceptions.py
--rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-1.2.0/deezer_asy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:20:39.782452 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/
--rw-rw-rw-   0        0        0      230 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 11:20:39.786440 pydeezer_asy-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      500 2023-07-12 11:20:28.000000 pydeezer_asy-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:56:22.773484 pydeezer_asy-1.2.1/
+-rw-rw-rw-   0        0        0     1662 2023-07-12 12:56:22.772487 pydeezer_asy-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1298 2023-07-12 12:53:05.000000 pydeezer_asy-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 12:56:22.625878 pydeezer_asy-1.2.1/deezer_asy/
+-rw-rw-rw-   0        0        0    30354 2023-07-12 11:17:17.000000 pydeezer_asy-1.2.1/deezer_asy/DeezerAsy.py
+-rw-rw-rw-   0        0        0      134 2023-07-07 16:55:48.000000 pydeezer_asy-1.2.1/deezer_asy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:56:22.661784 pydeezer_asy-1.2.1/deezer_asy/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/exceptions.py
+-rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-1.2.1/deezer_asy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:56:22.771531 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/
+-rw-rw-rw-   0        0        0     1662 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 12:56:22.775481 pydeezer_asy-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-12 12:56:15.000000 pydeezer_asy-1.2.1/setup.py
```

### Comparing `pydeezer_asy-1.2.0/deezer_asy/DeezerAsy.py` & `pydeezer_asy-1.2.1/deezer_asy/DeezerAsy.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.0/deezer_asy/constants/api_methods.py` & `pydeezer_asy-1.2.1/deezer_asy/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.0/deezer_asy/constants/track_formats.py` & `pydeezer_asy-1.2.1/deezer_asy/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.0/deezer_asy/util.py` & `pydeezer_asy-1.2.1/deezer_asy/util.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.0/pydeezer_asy.egg-info/SOURCES.txt` & `pydeezer_asy-1.2.1/pydeezer_asy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 deezer_asy/DeezerAsy.py
 deezer_asy/__init__.py
 deezer_asy/exceptions.py
 deezer_asy/util.py
 deezer_asy/constants/__init__.py
 deezer_asy/constants/api_methods.py
```

