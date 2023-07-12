# Comparing `tmp/weather_wiz-0.0.5.tar.gz` & `tmp/weather_wiz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_wiz-0.0.5.tar", last modified: Wed Jul 12 20:59:39 2023, max compression
+gzip compressed data, was "weather_wiz-0.0.6.tar", last modified: Wed Jul 12 21:03:23 2023, max compression
```

## Comparing `weather_wiz-0.0.5.tar` & `weather_wiz-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:59:39.993016 weather_wiz-0.0.5/
--rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 20:59:39.989016 weather_wiz-0.0.5/PKG-INFO
--rw-rw-r--   0 mine      (1000) mine      (1000)     1412 2023-07-12 16:35:40.000000 weather_wiz-0.0.5/README.md
--rw-rw-r--   0 mine      (1000) mine      (1000)       38 2023-07-12 20:59:39.993016 weather_wiz-0.0.5/setup.cfg
--rw-rw-r--   0 mine      (1000) mine      (1000)     1414 2023-07-12 20:59:18.000000 weather_wiz-0.0.5/setup.py
-drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:59:39.989016 weather_wiz-0.0.5/weather_wiz/
--rw-rw-r--   0 mine      (1000) mine      (1000)       36 2023-07-12 20:55:38.000000 weather_wiz-0.0.5/weather_wiz/__init__.py
--rw-rw-r--   0 mine      (1000) mine      (1000)     3156 2023-07-12 20:58:08.000000 weather_wiz-0.0.5/weather_wiz/weather_wiz.py
-drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:59:39.989016 weather_wiz-0.0.5/weather_wiz.egg-info/
--rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/PKG-INFO
--rw-rw-r--   0 mine      (1000) mine      (1000)      243 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/SOURCES.txt
--rw-rw-r--   0 mine      (1000) mine      (1000)        1 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/dependency_links.txt
--rw-rw-r--   0 mine      (1000) mine      (1000)      160 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/requires.txt
--rw-rw-r--   0 mine      (1000) mine      (1000)       12 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/top_level.txt
+drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 21:03:23.372155 weather_wiz-0.0.6/
+-rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 21:03:23.372155 weather_wiz-0.0.6/PKG-INFO
+-rw-rw-r--   0 mine      (1000) mine      (1000)     1412 2023-07-12 16:35:40.000000 weather_wiz-0.0.6/README.md
+-rw-rw-r--   0 mine      (1000) mine      (1000)       38 2023-07-12 21:03:23.372155 weather_wiz-0.0.6/setup.cfg
+-rw-rw-r--   0 mine      (1000) mine      (1000)     1414 2023-07-12 21:03:21.000000 weather_wiz-0.0.6/setup.py
+drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 21:03:23.368155 weather_wiz-0.0.6/weather_wiz/
+-rw-rw-r--   0 mine      (1000) mine      (1000)       36 2023-07-12 20:55:38.000000 weather_wiz-0.0.6/weather_wiz/__init__.py
+-rw-rw-r--   0 mine      (1000) mine      (1000)     3156 2023-07-12 20:58:08.000000 weather_wiz-0.0.6/weather_wiz/weather_wiz.py
+drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 21:03:23.372155 weather_wiz-0.0.6/weather_wiz.egg-info/
+-rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 21:03:23.000000 weather_wiz-0.0.6/weather_wiz.egg-info/PKG-INFO
+-rw-rw-r--   0 mine      (1000) mine      (1000)      243 2023-07-12 21:03:23.000000 weather_wiz-0.0.6/weather_wiz.egg-info/SOURCES.txt
+-rw-rw-r--   0 mine      (1000) mine      (1000)        1 2023-07-12 21:03:23.000000 weather_wiz-0.0.6/weather_wiz.egg-info/dependency_links.txt
+-rw-rw-r--   0 mine      (1000) mine      (1000)      160 2023-07-12 21:03:23.000000 weather_wiz-0.0.6/weather_wiz.egg-info/requires.txt
+-rw-rw-r--   0 mine      (1000) mine      (1000)       12 2023-07-12 21:03:23.000000 weather_wiz-0.0.6/weather_wiz.egg-info/top_level.txt
```

### Comparing `weather_wiz-0.0.5/PKG-INFO` & `weather_wiz-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather_wiz
-Version: 0.0.5
+Version: 0.0.6
 Summary: Get weather information from the command line
 Home-page: UNKNOWN
 Author: Pranjal Agarawal
 Author-email: prajesh.eleven118@gamil.com
 License: UNKNOWN
 Description: A package that allows you to get weather information from the command line using the OpenWeatherMap API.
 Keywords: python,weather,weather information,weather-wiz,weather-wiz package,weather-wiz python,OpenWeatherMap,OpenWeatherMap API,CLI,command line,command line interface,command line tool,tool,command line weather tool,command line weather information tool,command line weather information,command line weather
```

### Comparing `weather_wiz-0.0.5/README.md` & `weather_wiz-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `weather_wiz-0.0.5/setup.py` & `weather_wiz-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Get weather information from the command line'
 LONG_DESCRIPTION = 'A package that allows you to get weather information from the command line using the OpenWeatherMap API.'
 
 # Setting up
 setup(
     name="weather_wiz",
     version=VERSION,
```

### Comparing `weather_wiz-0.0.5/weather_wiz/weather_wiz.py` & `weather_wiz-0.0.6/weather_wiz/weather_wiz.py`

 * *Files identical despite different names*

