# Comparing `tmp/fusion-engine-0.2.2.tar.gz` & `tmp/fusion-engine-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-0.2.2.tar", last modified: Wed Jul 12 18:21:10 2023, max compression
+gzip compressed data, was "fusion-engine-0.2.3.tar", last modified: Wed Jul 12 19:32:05 2023, max compression
```

## Comparing `fusion-engine-0.2.2.tar` & `fusion-engine-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.348165 fusion-engine-0.2.2/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.2/LICENCE.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4533 2023-07-12 18:21:10.347530 fusion-engine-0.2.2/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3290 2023-07-12 17:50:47.000000 fusion-engine-0.2.2/README.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1647 2023-07-12 18:17:16.000000 fusion-engine-0.2.2/pyproject.toml
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.2/requirements.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-12 18:21:10.348457 fusion-engine-0.2.2/setup.cfg
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1018 2023-07-12 18:18:50.000000 fusion-engine-0.2.2/setup.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.326697 fusion-engine-0.2.2/src/
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.333645 fusion-engine-0.2.2/src/fusion_engine.egg-info/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4533 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      817 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/SOURCES.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/dependency_links.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/requires.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/top_level.txt
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.334153 fusion-engine-0.2.2/src/fusionengine/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      883 2023-07-12 18:19:20.000000 fusion-engine-0.2.2/src/fusionengine/__init__.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.334791 fusion-engine-0.2.2/src/fusionengine/debugfiles/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.2.2/src/fusionengine/debugfiles/fe.png
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.346672 fusion-engine-0.2.2/src/fusionengine/files/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3439 2023-07-10 21:29:12.000000 fusion-engine-0.2.2/src/fusionengine/files/body.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1415 2023-07-04 15:09:45.000000 fusion-engine-0.2.2/src/fusionengine/files/color.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      382 2023-07-04 15:09:45.000000 fusion-engine-0.2.2/src/fusionengine/files/data.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2409 2023-07-09 21:02:50.000000 fusion-engine-0.2.2/src/fusionengine/files/draw.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      232 2023-07-02 09:01:28.000000 fusion-engine-0.2.2/src/fusionengine/files/enums.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10707 2023-07-09 21:03:18.000000 fusion-engine-0.2.2/src/fusionengine/files/event.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       91 2023-07-02 09:01:28.000000 fusion-engine-0.2.2/src/fusionengine/files/exceptions.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      904 2023-07-09 20:56:06.000000 fusion-engine-0.2.2/src/fusionengine/files/image.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      475 2023-07-12 17:28:30.000000 fusion-engine-0.2.2/src/fusionengine/files/imports.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.2/src/fusionengine/files/physics.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      537 2023-07-09 21:03:30.000000 fusion-engine-0.2.2/src/fusionengine/files/shape.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5566 2023-07-02 09:01:28.000000 fusion-engine-0.2.2/src/fusionengine/files/storage.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      792 2023-07-09 21:03:41.000000 fusion-engine-0.2.2/src/fusionengine/files/systems.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1693 2023-07-12 17:27:08.000000 fusion-engine-0.2.2/src/fusionengine/files/ui.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1885 2023-07-11 16:05:00.000000 fusion-engine-0.2.2/src/fusionengine/files/window.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 19:32:05.782372 fusion-engine-0.2.3/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.3/LICENCE.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4743 2023-07-12 19:32:05.781733 fusion-engine-0.2.3/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3500 2023-07-12 19:31:53.000000 fusion-engine-0.2.3/README.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1647 2023-07-12 18:17:16.000000 fusion-engine-0.2.3/pyproject.toml
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.3/requirements.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-12 19:32:05.782527 fusion-engine-0.2.3/setup.cfg
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1018 2023-07-12 18:18:50.000000 fusion-engine-0.2.3/setup.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 19:32:05.753315 fusion-engine-0.2.3/src/
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 19:32:05.763708 fusion-engine-0.2.3/src/fusion_engine.egg-info/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4743 2023-07-12 19:32:05.000000 fusion-engine-0.2.3/src/fusion_engine.egg-info/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      817 2023-07-12 19:32:05.000000 fusion-engine-0.2.3/src/fusion_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-12 19:32:05.000000 fusion-engine-0.2.3/src/fusion_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-12 19:32:05.000000 fusion-engine-0.2.3/src/fusion_engine.egg-info/requires.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-12 19:32:05.000000 fusion-engine-0.2.3/src/fusion_engine.egg-info/top_level.txt
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 19:32:05.764621 fusion-engine-0.2.3/src/fusionengine/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      883 2023-07-12 19:31:27.000000 fusion-engine-0.2.3/src/fusionengine/__init__.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 19:32:05.765426 fusion-engine-0.2.3/src/fusionengine/debugfiles/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.2.3/src/fusionengine/debugfiles/fe.png
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 19:32:05.780587 fusion-engine-0.2.3/src/fusionengine/files/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3439 2023-07-10 21:29:12.000000 fusion-engine-0.2.3/src/fusionengine/files/body.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1415 2023-07-04 15:09:45.000000 fusion-engine-0.2.3/src/fusionengine/files/color.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      382 2023-07-04 15:09:45.000000 fusion-engine-0.2.3/src/fusionengine/files/data.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2409 2023-07-09 21:02:50.000000 fusion-engine-0.2.3/src/fusionengine/files/draw.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      232 2023-07-02 09:01:28.000000 fusion-engine-0.2.3/src/fusionengine/files/enums.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10707 2023-07-09 21:03:18.000000 fusion-engine-0.2.3/src/fusionengine/files/event.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       91 2023-07-02 09:01:28.000000 fusion-engine-0.2.3/src/fusionengine/files/exceptions.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      904 2023-07-09 20:56:06.000000 fusion-engine-0.2.3/src/fusionengine/files/image.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      475 2023-07-12 17:28:30.000000 fusion-engine-0.2.3/src/fusionengine/files/imports.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.3/src/fusionengine/files/physics.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      537 2023-07-09 21:03:30.000000 fusion-engine-0.2.3/src/fusionengine/files/shape.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5566 2023-07-02 09:01:28.000000 fusion-engine-0.2.3/src/fusionengine/files/storage.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      792 2023-07-09 21:03:41.000000 fusion-engine-0.2.3/src/fusionengine/files/systems.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1693 2023-07-12 17:27:08.000000 fusion-engine-0.2.3/src/fusionengine/files/ui.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1869 2023-07-12 19:17:58.000000 fusion-engine-0.2.3/src/fusionengine/files/window.py
```

### Comparing `fusion-engine-0.2.2/LICENCE.md` & `fusion-engine-0.2.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/PKG-INFO` & `fusion-engine-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.2
+Version: 0.2.3
 Summary: This a fully custom engine based on Python and PySDL2, it's written in pure Python!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -29,14 +29,18 @@
 
 ![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
 
 Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
 rendering graphics, and handling user input. It is and engine to create
 games fast and easy!
 
+### 🌐 Website
+
+We have our own website with our docs on it. Things like information could be a little outdated, but the docs are hosted there. [See here](https://dimkauzh.github.io/fusion-engine/)
+
 ### 💻 Development
 
 Keep in mind that this project is in work, so if you want to see code,
 then it is in dev branch but there is no 'full version' of this project!
 We working hard to make first alpha version of it!
 
 ## 💾 Installation
@@ -70,15 +74,15 @@
 
 - Zenthm (Contributing)
 - XCarCedo (Contributing)
 - FBS_Gamer (Discord server)
 
 ## 📃 Documentation
 
-See at [The wiki of the project](https://github.com/dimkauzh/fusion-engine/wiki) (Still in work!)
+See at [The wiki of the project](https://dimkauzh.github.io/fusion-engine/wiki/wiki.html) (Still in work!)
 
 ## 📯 Coming features
 
 We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
 
 - [x] Engine
   - [x] Create window
```

### Comparing `fusion-engine-0.2.2/README.md` & `fusion-engine-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 ![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
 
 Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
 rendering graphics, and handling user input. It is and engine to create
 games fast and easy!
 
+### 🌐 Website
+
+We have our own website with our docs on it. Things like information could be a little outdated, but the docs are hosted there. [See here](https://dimkauzh.github.io/fusion-engine/)
+
 ### 💻 Development
 
 Keep in mind that this project is in work, so if you want to see code,
 then it is in dev branch but there is no 'full version' of this project!
 We working hard to make first alpha version of it!
 
 ## 💾 Installation
@@ -43,15 +47,15 @@
 
 - Zenthm (Contributing)
 - XCarCedo (Contributing)
 - FBS_Gamer (Discord server)
 
 ## 📃 Documentation
 
-See at [The wiki of the project](https://github.com/dimkauzh/fusion-engine/wiki) (Still in work!)
+See at [The wiki of the project](https://dimkauzh.github.io/fusion-engine/wiki/wiki.html) (Still in work!)
 
 ## 📯 Coming features
 
 We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
 
 - [x] Engine
   - [x] Create window
```

### Comparing `fusion-engine-0.2.2/pyproject.toml` & `fusion-engine-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/setup.py` & `fusion-engine-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusion_engine.egg-info/PKG-INFO` & `fusion-engine-0.2.3/src/fusion_engine.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.2
+Version: 0.2.3
 Summary: This a fully custom engine based on Python and PySDL2, it's written in pure Python!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -29,14 +29,18 @@
 
 ![logo](https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png)
 
 Fusion is a game engine for creating graphical applications using the PySDL2 library and the programming language Python. It provides a simple coding interface for creating windows,
 rendering graphics, and handling user input. It is and engine to create
 games fast and easy!
 
+### 🌐 Website
+
+We have our own website with our docs on it. Things like information could be a little outdated, but the docs are hosted there. [See here](https://dimkauzh.github.io/fusion-engine/)
+
 ### 💻 Development
 
 Keep in mind that this project is in work, so if you want to see code,
 then it is in dev branch but there is no 'full version' of this project!
 We working hard to make first alpha version of it!
 
 ## 💾 Installation
@@ -70,15 +74,15 @@
 
 - Zenthm (Contributing)
 - XCarCedo (Contributing)
 - FBS_Gamer (Discord server)
 
 ## 📃 Documentation
 
-See at [The wiki of the project](https://github.com/dimkauzh/fusion-engine/wiki) (Still in work!)
+See at [The wiki of the project](https://dimkauzh.github.io/fusion-engine/wiki/wiki.html) (Still in work!)
 
 ## 📯 Coming features
 
 We are working hard to implement very basic and complex stuff so our engine becomes more rigid. These features are worked on or will be worked on:
 
 - [x] Engine
   - [x] Create window
```

### Comparing `fusion-engine-0.2.2/src/fusion_engine.egg-info/SOURCES.txt` & `fusion-engine-0.2.3/src/fusion_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/__init__.py` & `fusion-engine-0.2.3/src/fusionengine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Dimkauzh"
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 import fusionengine.files.data as data
 import fusionengine.files.systems as sysconfig
 
 from fusionengine.files.imports import *
 
 class Main:
```

### Comparing `fusion-engine-0.2.2/src/fusionengine/debugfiles/fe.png` & `fusion-engine-0.2.3/src/fusionengine/debugfiles/fe.png`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/body.py` & `fusion-engine-0.2.3/src/fusionengine/files/body.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/color.py` & `fusion-engine-0.2.3/src/fusionengine/files/color.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/draw.py` & `fusion-engine-0.2.3/src/fusionengine/files/draw.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/event.py` & `fusion-engine-0.2.3/src/fusionengine/files/event.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/image.py` & `fusion-engine-0.2.3/src/fusionengine/files/image.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/shape.py` & `fusion-engine-0.2.3/src/fusionengine/files/shape.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/storage.py` & `fusion-engine-0.2.3/src/fusionengine/files/storage.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/systems.py` & `fusion-engine-0.2.3/src/fusionengine/files/systems.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/ui.py` & `fusion-engine-0.2.3/src/fusionengine/files/ui.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.2/src/fusionengine/files/window.py` & `fusion-engine-0.2.3/src/fusionengine/files/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,10 +43,9 @@
         self._LAST = self._NOW
         self._NOW = sdl2.SDL_GetPerformanceCounter()
 
 
 
         self.DELTATIME = (self._NOW - self._LAST)*1000 / sdl2.SDL_GetPerformanceFrequency()
 
-        if sdl2.SDL_PollEvent(window.event) != 0:
-            if window.event.type == sdl2.SDL_QUIT:
-                self._running = False
+        if sdl2.SDL_PollEvent(window.event) != 0 and window.event.type == sdl2.SDL_QUIT:
+            self._running = False
```

