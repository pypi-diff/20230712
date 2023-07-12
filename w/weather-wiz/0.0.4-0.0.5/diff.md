# Comparing `tmp/weather_wiz-0.0.4.tar.gz` & `tmp/weather_wiz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_wiz-0.0.4.tar", last modified: Wed Jul 12 20:56:14 2023, max compression
+gzip compressed data, was "weather_wiz-0.0.5.tar", last modified: Wed Jul 12 20:59:39 2023, max compression
```

## Comparing `weather_wiz-0.0.4.tar` & `weather_wiz-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:56:14.306235 weather_wiz-0.0.4/
--rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 20:56:14.306235 weather_wiz-0.0.4/PKG-INFO
--rw-rw-r--   0 mine      (1000) mine      (1000)     1412 2023-07-12 16:35:40.000000 weather_wiz-0.0.4/README.md
--rw-rw-r--   0 mine      (1000) mine      (1000)       38 2023-07-12 20:56:14.306235 weather_wiz-0.0.4/setup.cfg
--rw-rw-r--   0 mine      (1000) mine      (1000)     1414 2023-07-12 20:56:08.000000 weather_wiz-0.0.4/setup.py
-drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:56:14.306235 weather_wiz-0.0.4/weather_wiz/
--rw-rw-r--   0 mine      (1000) mine      (1000)       36 2023-07-12 20:55:38.000000 weather_wiz-0.0.4/weather_wiz/__init__.py
--rw-rw-r--   0 mine      (1000) mine      (1000)     3160 2023-07-12 20:40:53.000000 weather_wiz-0.0.4/weather_wiz/weather_wiz.py
-drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:56:14.306235 weather_wiz-0.0.4/weather_wiz.egg-info/
--rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 20:56:14.000000 weather_wiz-0.0.4/weather_wiz.egg-info/PKG-INFO
--rw-rw-r--   0 mine      (1000) mine      (1000)      243 2023-07-12 20:56:14.000000 weather_wiz-0.0.4/weather_wiz.egg-info/SOURCES.txt
--rw-rw-r--   0 mine      (1000) mine      (1000)        1 2023-07-12 20:56:14.000000 weather_wiz-0.0.4/weather_wiz.egg-info/dependency_links.txt
--rw-rw-r--   0 mine      (1000) mine      (1000)      160 2023-07-12 20:56:14.000000 weather_wiz-0.0.4/weather_wiz.egg-info/requires.txt
--rw-rw-r--   0 mine      (1000) mine      (1000)       12 2023-07-12 20:56:14.000000 weather_wiz-0.0.4/weather_wiz.egg-info/top_level.txt
+drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:59:39.993016 weather_wiz-0.0.5/
+-rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 20:59:39.989016 weather_wiz-0.0.5/PKG-INFO
+-rw-rw-r--   0 mine      (1000) mine      (1000)     1412 2023-07-12 16:35:40.000000 weather_wiz-0.0.5/README.md
+-rw-rw-r--   0 mine      (1000) mine      (1000)       38 2023-07-12 20:59:39.993016 weather_wiz-0.0.5/setup.cfg
+-rw-rw-r--   0 mine      (1000) mine      (1000)     1414 2023-07-12 20:59:18.000000 weather_wiz-0.0.5/setup.py
+drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:59:39.989016 weather_wiz-0.0.5/weather_wiz/
+-rw-rw-r--   0 mine      (1000) mine      (1000)       36 2023-07-12 20:55:38.000000 weather_wiz-0.0.5/weather_wiz/__init__.py
+-rw-rw-r--   0 mine      (1000) mine      (1000)     3156 2023-07-12 20:58:08.000000 weather_wiz-0.0.5/weather_wiz/weather_wiz.py
+drwxrwxr-x   0 mine      (1000) mine      (1000)        0 2023-07-12 20:59:39.989016 weather_wiz-0.0.5/weather_wiz.egg-info/
+-rw-rw-r--   0 mine      (1000) mine      (1000)      934 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/PKG-INFO
+-rw-rw-r--   0 mine      (1000) mine      (1000)      243 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/SOURCES.txt
+-rw-rw-r--   0 mine      (1000) mine      (1000)        1 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/dependency_links.txt
+-rw-rw-r--   0 mine      (1000) mine      (1000)      160 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/requires.txt
+-rw-rw-r--   0 mine      (1000) mine      (1000)       12 2023-07-12 20:59:39.000000 weather_wiz-0.0.5/weather_wiz.egg-info/top_level.txt
```

### Comparing `weather_wiz-0.0.4/PKG-INFO` & `weather_wiz-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather_wiz
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get weather information from the command line
 Home-page: UNKNOWN
 Author: Pranjal Agarawal
 Author-email: prajesh.eleven118@gamil.com
 License: UNKNOWN
 Description: A package that allows you to get weather information from the command line using the OpenWeatherMap API.
 Keywords: python,weather,weather information,weather-wiz,weather-wiz package,weather-wiz python,OpenWeatherMap,OpenWeatherMap API,CLI,command line,command line interface,command line tool,tool,command line weather tool,command line weather information tool,command line weather information,command line weather
```

### Comparing `weather_wiz-0.0.4/README.md` & `weather_wiz-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `weather_wiz-0.0.4/setup.py` & `weather_wiz-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Get weather information from the command line'
 LONG_DESCRIPTION = 'A package that allows you to get weather information from the command line using the OpenWeatherMap API.'
 
 # Setting up
 setup(
     name="weather_wiz",
     version=VERSION,
```

### Comparing `weather_wiz-0.0.4/weather_wiz/weather_wiz.py` & `weather_wiz-0.0.5/weather_wiz/weather_wiz.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pyfiglet import Figlet
 from tabulate import tabulate
 from termcolor import colored
 from datetime import datetime
 from dotenv import load_dotenv
 load_dotenv()
 
-API_KEY = os.environ.get("OPEN_WEATHER_API_KEY")
+API_KEY = "45b11607ce8aa9c3a54c0a355e420441"
 API_URL = "https://api.openweathermap.org/data/2.5/weather?q={city}&appid={api_key}&units=metric"
 
 
 def get_weather(city):
     url = API_URL.format(city=city, api_key=API_KEY)
 
     response = requests.get(url)
```

### Comparing `weather_wiz-0.0.4/weather_wiz.egg-info/PKG-INFO` & `weather_wiz-0.0.5/weather_wiz.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-wiz
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get weather information from the command line
 Home-page: UNKNOWN
 Author: Pranjal Agarawal
 Author-email: prajesh.eleven118@gamil.com
 License: UNKNOWN
 Description: A package that allows you to get weather information from the command line using the OpenWeatherMap API.
 Keywords: python,weather,weather information,weather-wiz,weather-wiz package,weather-wiz python,OpenWeatherMap,OpenWeatherMap API,CLI,command line,command line interface,command line tool,tool,command line weather tool,command line weather information tool,command line weather information,command line weather
```

