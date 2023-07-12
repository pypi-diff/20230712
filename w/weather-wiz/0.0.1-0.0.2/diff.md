# Comparing `tmp/weather-wiz-0.0.1.tar.gz` & `tmp/weather-wiz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather-wiz-0.0.1.tar", last modified: Wed Jul 12 16:39:34 2023, max compression
+gzip compressed data, was "weather-wiz-0.0.2.tar", last modified: Wed Jul 12 20:42:52 2023, max compression
```

## Comparing `weather-wiz-0.0.1.tar` & `weather-wiz-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 16:39:34.356463 weather-wiz-0.0.1/
--rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 16:39:34.356463 weather-wiz-0.0.1/PKG-INFO
--rw-rw-r--   0 mine      (1000) mine      (1000)     1412 2023-07-12 16:35:40.000000 weather-wiz-0.0.1/README.md
--rw-rw-r--   0 mine      (1000) mine      (1000)       38 2023-07-12 16:39:34.356463 weather-wiz-0.0.1/setup.cfg
--rw-rw-r--   0 mine      (1000) mine      (1000)     1414 2023-07-12 16:37:48.000000 weather-wiz-0.0.1/setup.py
-drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 16:39:34.356463 weather-wiz-0.0.1/weather-wiz/
--rw-rw-r--   0 mine      (1000) mine      (1000)       51 2023-07-12 16:11:08.000000 weather-wiz-0.0.1/weather-wiz/__init__.py
--rw-rw-r--   0 mine      (1000) mine      (1000)     3160 2023-07-12 16:09:08.000000 weather-wiz-0.0.1/weather-wiz/weather_wiz.py
-drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 16:39:34.356463 weather-wiz-0.0.1/weather_wiz.egg-info/
--rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 16:39:34.000000 weather-wiz-0.0.1/weather_wiz.egg-info/PKG-INFO
--rw-rw-r--   0 mine      (1000) mine      (1000)      243 2023-07-12 16:39:34.000000 weather-wiz-0.0.1/weather_wiz.egg-info/SOURCES.txt
--rw-rw-r--   0 mine      (1000) mine      (1000)        1 2023-07-12 16:39:34.000000 weather-wiz-0.0.1/weather_wiz.egg-info/dependency_links.txt
--rw-rw-r--   0 mine      (1000) mine      (1000)      160 2023-07-12 16:39:34.000000 weather-wiz-0.0.1/weather_wiz.egg-info/requires.txt
--rw-rw-r--   0 mine      (1000) mine      (1000)       12 2023-07-12 16:39:34.000000 weather-wiz-0.0.1/weather_wiz.egg-info/top_level.txt
+drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:42:52.262312 weather-wiz-0.0.2/
+-rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 20:42:52.262312 weather-wiz-0.0.2/PKG-INFO
+-rw-rw-r--   0 mine      (1000) mine      (1000)     1412 2023-07-12 16:35:40.000000 weather-wiz-0.0.2/README.md
+-rw-rw-r--   0 mine      (1000) mine      (1000)       38 2023-07-12 20:42:52.262312 weather-wiz-0.0.2/setup.cfg
+-rw-rw-r--   0 mine      (1000) mine      (1000)     1414 2023-07-12 20:41:49.000000 weather-wiz-0.0.2/setup.py
+drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:42:52.262312 weather-wiz-0.0.2/weather_wiz/
+-rw-rw-r--   0 mine      (1000) mine      (1000)       51 2023-07-12 16:11:08.000000 weather-wiz-0.0.2/weather_wiz/__init__.py
+-rw-rw-r--   0 mine      (1000) mine      (1000)     3160 2023-07-12 20:40:53.000000 weather-wiz-0.0.2/weather_wiz/weather_wiz.py
+drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:42:52.262312 weather-wiz-0.0.2/weather_wiz.egg-info/
+-rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 20:42:52.000000 weather-wiz-0.0.2/weather_wiz.egg-info/PKG-INFO
+-rw-rw-r--   0 mine      (1000) mine      (1000)      243 2023-07-12 20:42:52.000000 weather-wiz-0.0.2/weather_wiz.egg-info/SOURCES.txt
+-rw-rw-r--   0 mine      (1000) mine      (1000)        1 2023-07-12 20:42:52.000000 weather-wiz-0.0.2/weather_wiz.egg-info/dependency_links.txt
+-rw-rw-r--   0 mine      (1000) mine      (1000)      160 2023-07-12 20:42:52.000000 weather-wiz-0.0.2/weather_wiz.egg-info/requires.txt
+-rw-rw-r--   0 mine      (1000) mine      (1000)       12 2023-07-12 20:42:52.000000 weather-wiz-0.0.2/weather_wiz.egg-info/top_level.txt
```

### Comparing `weather-wiz-0.0.1/PKG-INFO` & `weather-wiz-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-wiz
-Version: 0.0.1
+Version: 0.0.2
 Summary: Get weather information from the command line
 Home-page: UNKNOWN
 Author: Pranjal Agarawal
 Author-email: prajesh.eleven118@gamil.com
 License: UNKNOWN
 Description: A package that allows you to get weather information from the command line using the OpenWeatherMap API.
 Keywords: python,weather,weather information,weather-wiz,weather-wiz package,weather-wiz python,OpenWeatherMap,OpenWeatherMap API,CLI,command line,command line interface,command line tool,tool,command line weather tool,command line weather information tool,command line weather information,command line weather
```

### Comparing `weather-wiz-0.0.1/README.md` & `weather-wiz-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `weather-wiz-0.0.1/setup.py` & `weather-wiz-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Get weather information from the command line'
 LONG_DESCRIPTION = 'A package that allows you to get weather information from the command line using the OpenWeatherMap API.'
 
 # Setting up
 setup(
     name="weather-wiz",
     version=VERSION,
```

### Comparing `weather-wiz-0.0.1/weather-wiz/weather_wiz.py` & `weather-wiz-0.0.2/weather_wiz/weather_wiz.py`

 * *Files identical despite different names*

### Comparing `weather-wiz-0.0.1/weather_wiz.egg-info/PKG-INFO` & `weather-wiz-0.0.2/weather_wiz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-wiz
-Version: 0.0.1
+Version: 0.0.2
 Summary: Get weather information from the command line
 Home-page: UNKNOWN
 Author: Pranjal Agarawal
 Author-email: prajesh.eleven118@gamil.com
 License: UNKNOWN
 Description: A package that allows you to get weather information from the command line using the OpenWeatherMap API.
 Keywords: python,weather,weather information,weather-wiz,weather-wiz package,weather-wiz python,OpenWeatherMap,OpenWeatherMap API,CLI,command line,command line interface,command line tool,tool,command line weather tool,command line weather information tool,command line weather information,command line weather
```

