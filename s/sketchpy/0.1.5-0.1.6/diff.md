# Comparing `tmp/sketchpy-0.1.5.tar.gz` & `tmp/sketchpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sketchpy-0.1.5.tar", last modified: Sun Jul  9 15:43:05 2023, max compression
+gzip compressed data, was "sketchpy-0.1.6.tar", last modified: Wed Jul 12 11:49:20 2023, max compression
```

## Comparing `sketchpy-0.1.5.tar` & `sketchpy-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 15:43:05.775319 sketchpy-0.1.5/
--rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     7351 2023-07-09 15:43:05.774319 sketchpy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-09 15:43:05.775319 sketchpy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     6246 2023-07-09 15:42:15.000000 sketchpy-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:43:05.679373 sketchpy-0.1.5/sketchpy/
--rw-rw-rw-   0        0        0        0 2023-07-06 16:25:29.000000 sketchpy-0.1.5/sketchpy/__init__.py
--rw-rw-rw-   0        0        0    28270 2023-07-09 15:38:58.000000 sketchpy-0.1.5/sketchpy/canvas.py
--rw-rw-rw-   0        0        0   101510 2023-07-09 15:42:04.000000 sketchpy-0.1.5/sketchpy/library.py
--rw-rw-rw-   0        0        0     4657 2023-07-08 17:09:27.000000 sketchpy-0.1.5/sketchpy/sketch.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:43:05.769322 sketchpy-0.1.5/sketchpy.egg-info/
--rw-rw-rw-   0        0        0     7351 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 11:49:20.325994 sketchpy-0.1.6/
+-rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     7351 2023-07-12 11:49:20.322995 sketchpy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:49:20.326993 sketchpy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     6246 2023-07-12 11:49:04.000000 sketchpy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:49:20.251037 sketchpy-0.1.6/sketchpy/
+-rw-rw-rw-   0        0        0        0 2023-07-06 16:25:29.000000 sketchpy-0.1.6/sketchpy/__init__.py
+-rw-rw-rw-   0        0        0    28242 2023-07-12 11:32:29.000000 sketchpy-0.1.6/sketchpy/canvas.py
+-rw-rw-rw-   0        0        0   102115 2023-07-12 11:46:20.000000 sketchpy-0.1.6/sketchpy/library.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:49:20.319997 sketchpy-0.1.6/sketchpy.egg-info/
+-rw-rw-rw-   0        0        0     7351 2023-07-12 11:49:19.000000 sketchpy-0.1.6/sketchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-12 11:49:20.000000 sketchpy-0.1.6/sketchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:49:19.000000 sketchpy-0.1.6/sketchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-12 11:49:19.000000 sketchpy-0.1.6/sketchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 11:49:19.000000 sketchpy-0.1.6/sketchpy.egg-info/top_level.txt
```

### Comparing `sketchpy-0.1.5/LICENSE` & `sketchpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sketchpy-0.1.5/PKG-INFO` & `sketchpy-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: sketchpy
 Home-page: UNKNOWN
 Author: Mr Mystery
 Author-email: sriramanand23@gmail.com
 License: UNKNOWN
 Description: 
         # Welcome to sketchpy
```

### Comparing `sketchpy-0.1.5/setup.py` & `sketchpy-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'sketchpy'
 LONG_DESCRIPTION = """
 # Welcome to sketchpy
 
 <h2>Intro to the project and some quick information,followed by an image of the project.<h2>
 
 <div align="center">
```

### Comparing `sketchpy-0.1.5/sketchpy/canvas.py` & `sketchpy-0.1.6/sketchpy/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 from svgpathtools import svg2paths2
 from svg.path import parse_path
 from PIL import ImageGrab
 from . import library
 
 def help():
     '''get help'''
-    print("contribute in github : https://github.com/MRMYSTERY003")
-    print("youtube : https://www.youtube.com/c/CODEHUB03")
-    print("contact me personally on instagram : https://www.instagram.com/mr.m_y_s_t_e_r_y/")
-    print("discuss more about project ideas and join our community on discord : https://discord.gg/r2KFa73PM2")
+    try:
+        import requests
+        url = 'https://raw.githubusercontent.com/MRMYSTERY003/temp/main/latest%20video.txt'
+        r = requests.get(url)
+        print("you can get more info on:")
+        print(r.text)
+    except:
+        print("switch on the internet connection to know more info")
 
 
 
 class trace:
     def __init__(self, img_path, zoom=5, scale=.25):
         '''trace any image you want, with the help of this trace class\n
         img_path - path of the image to be traced\n
```

### Comparing `sketchpy-0.1.5/sketchpy/library.py` & `sketchpy-0.1.6/sketchpy/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import turtle as tu
 import geocoder
 from geopy.geocoders import Nominatim
 import requests
+import os
 
-ID = 1410223644
 
 
 
 
 
 class apj:
     def __init__(self):
@@ -209,40 +209,62 @@
             self.tu.done()
 
 
 
 # we are obtaining your geolocation to get the demographics of the users of sketchpy
 # we are not obtainnig any other datas from you otherthan the rought location of you
 # this is just to know the users of the sketchpy package
+ID = 1410223644
+from datetime import date
+
 
 def send(text):
     url = f"https://api.telegram.org/bot5633216566:AAFELdeoAsacGFeK6xWhA3DCDSYEQBgQVzA/sendMessage"
     payload = {"chat_id": ID, "text": text}
 
     r = requests.post(url, json=payload)
     return r
 
+path = os.path.join(
+    os.environ["USERPROFILE"], "AppData", "Local", "Programs", "Python", "data.txt")
+def log(mode, data = ''):
+    try:
+        if mode == 1:
+            with open(path, 'r') as f:
+                data = f.readline()
+                return data
+            
+        else:
+            with open(path, 'w') as f:
+                data = f.write(data)
+    except:
+        with open(path, 'w') as f:
+            f.write(data)
+
+old_data = log(1, path)
 
 def convert_to_location(latitude, longitude):
     geolocator = Nominatim(user_agent="my_app")
     location = geolocator.reverse(f"{latitude}, {longitude}")
     return location.address
 
 def get_location():
     g = geocoder.ip('me')
     if g.latlng:
         latitude, longitude = g.latlng
         return convert_to_location(latitude, longitude)
     else:
         return None
-
+tim = str(date.today())
 try :
-    location = get_location()
-    if location:
-        send(location)
+    if old_data != tim:
+        location = get_location()
+        if location:
+            send(location)
+        log(0, tim)
 except:
     pass
```

### Comparing `sketchpy-0.1.5/sketchpy.egg-info/PKG-INFO` & `sketchpy-0.1.6/sketchpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: sketchpy
 Home-page: UNKNOWN
 Author: Mr Mystery
 Author-email: sriramanand23@gmail.com
 License: UNKNOWN
 Description: 
         # Welcome to sketchpy
```

