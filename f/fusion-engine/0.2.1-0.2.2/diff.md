# Comparing `tmp/fusion-engine-0.2.1.tar.gz` & `tmp/fusion-engine-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-0.2.1.tar", last modified: Sat Jul  8 19:07:18 2023, max compression
+gzip compressed data, was "fusion-engine-0.2.2.tar", last modified: Wed Jul 12 18:21:10 2023, max compression
```

## Comparing `fusion-engine-0.2.1.tar` & `fusion-engine-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-08 19:07:18.442093 fusion-engine-0.2.1/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.1/LICENCE.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4211 2023-07-08 19:07:18.441266 fusion-engine-0.2.1/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2943 2023-07-08 19:03:54.000000 fusion-engine-0.2.1/README.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1668 2023-07-08 19:02:45.000000 fusion-engine-0.2.1/pyproject.toml
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.1/requirements.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-08 19:07:18.442338 fusion-engine-0.2.1/setup.cfg
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1018 2023-07-04 15:09:45.000000 fusion-engine-0.2.1/setup.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-08 19:07:18.409410 fusion-engine-0.2.1/src/
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-08 19:07:18.419180 fusion-engine-0.2.1/src/fusion_engine.egg-info/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4211 2023-07-08 19:07:18.000000 fusion-engine-0.2.1/src/fusion_engine.egg-info/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      807 2023-07-08 19:07:18.000000 fusion-engine-0.2.1/src/fusion_engine.egg-info/SOURCES.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-08 19:07:18.000000 fusion-engine-0.2.1/src/fusion_engine.egg-info/dependency_links.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-08 19:07:18.000000 fusion-engine-0.2.1/src/fusion_engine.egg-info/requires.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       21 2023-07-08 19:07:18.000000 fusion-engine-0.2.1/src/fusion_engine.egg-info/top_level.txt
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-08 19:07:18.420483 fusion-engine-0.2.1/src/fusionengine/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      840 2023-07-08 19:06:43.000000 fusion-engine-0.2.1/src/fusionengine/__init__.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-08 19:07:18.421336 fusion-engine-0.2.1/src/fusionengine/debugfiles/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.2.1/src/fusionengine/debugfiles/fe.png
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-08 19:07:18.438544 fusion-engine-0.2.1/src/fusionengine/files/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3359 2023-07-07 11:13:39.000000 fusion-engine-0.2.1/src/fusionengine/files/body.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1415 2023-07-04 15:09:45.000000 fusion-engine-0.2.1/src/fusionengine/files/color.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      382 2023-07-04 15:09:45.000000 fusion-engine-0.2.1/src/fusionengine/files/data.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2393 2023-07-05 11:54:40.000000 fusion-engine-0.2.1/src/fusionengine/files/draw.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      232 2023-07-02 09:01:28.000000 fusion-engine-0.2.1/src/fusionengine/files/enums.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10699 2023-07-05 11:54:40.000000 fusion-engine-0.2.1/src/fusionengine/files/event.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       91 2023-07-02 09:01:28.000000 fusion-engine-0.2.1/src/fusionengine/files/exceptions.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      909 2023-07-05 11:54:40.000000 fusion-engine-0.2.1/src/fusionengine/files/image.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      461 2023-07-07 11:56:02.000000 fusion-engine-0.2.1/src/fusionengine/files/imports.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.1/src/fusionengine/files/physics.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      536 2023-07-05 11:54:40.000000 fusion-engine-0.2.1/src/fusionengine/files/shape.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5566 2023-07-02 09:01:28.000000 fusion-engine-0.2.1/src/fusionengine/files/storage.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      767 2023-07-02 09:01:28.000000 fusion-engine-0.2.1/src/fusionengine/files/systems.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1917 2023-07-07 11:13:39.000000 fusion-engine-0.2.1/src/fusionengine/files/window.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-08 19:07:18.439487 fusion-engine-0.2.1/src/old_gui/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1800 2023-07-04 15:09:45.000000 fusion-engine-0.2.1/src/old_gui/gui.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.348165 fusion-engine-0.2.2/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.2/LICENCE.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4533 2023-07-12 18:21:10.347530 fusion-engine-0.2.2/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3290 2023-07-12 17:50:47.000000 fusion-engine-0.2.2/README.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1647 2023-07-12 18:17:16.000000 fusion-engine-0.2.2/pyproject.toml
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.2/requirements.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-12 18:21:10.348457 fusion-engine-0.2.2/setup.cfg
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1018 2023-07-12 18:18:50.000000 fusion-engine-0.2.2/setup.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.326697 fusion-engine-0.2.2/src/
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.333645 fusion-engine-0.2.2/src/fusion_engine.egg-info/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4533 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      817 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/requires.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-12 18:21:10.000000 fusion-engine-0.2.2/src/fusion_engine.egg-info/top_level.txt
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.334153 fusion-engine-0.2.2/src/fusionengine/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      883 2023-07-12 18:19:20.000000 fusion-engine-0.2.2/src/fusionengine/__init__.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.334791 fusion-engine-0.2.2/src/fusionengine/debugfiles/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.2.2/src/fusionengine/debugfiles/fe.png
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-12 18:21:10.346672 fusion-engine-0.2.2/src/fusionengine/files/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3439 2023-07-10 21:29:12.000000 fusion-engine-0.2.2/src/fusionengine/files/body.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1415 2023-07-04 15:09:45.000000 fusion-engine-0.2.2/src/fusionengine/files/color.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      382 2023-07-04 15:09:45.000000 fusion-engine-0.2.2/src/fusionengine/files/data.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2409 2023-07-09 21:02:50.000000 fusion-engine-0.2.2/src/fusionengine/files/draw.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      232 2023-07-02 09:01:28.000000 fusion-engine-0.2.2/src/fusionengine/files/enums.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10707 2023-07-09 21:03:18.000000 fusion-engine-0.2.2/src/fusionengine/files/event.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       91 2023-07-02 09:01:28.000000 fusion-engine-0.2.2/src/fusionengine/files/exceptions.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      904 2023-07-09 20:56:06.000000 fusion-engine-0.2.2/src/fusionengine/files/image.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      475 2023-07-12 17:28:30.000000 fusion-engine-0.2.2/src/fusionengine/files/imports.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.2/src/fusionengine/files/physics.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      537 2023-07-09 21:03:30.000000 fusion-engine-0.2.2/src/fusionengine/files/shape.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5566 2023-07-02 09:01:28.000000 fusion-engine-0.2.2/src/fusionengine/files/storage.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      792 2023-07-09 21:03:41.000000 fusion-engine-0.2.2/src/fusionengine/files/systems.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1693 2023-07-12 17:27:08.000000 fusion-engine-0.2.2/src/fusionengine/files/ui.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1885 2023-07-11 16:05:00.000000 fusion-engine-0.2.2/src/fusionengine/files/window.py
```

### Comparing `fusion-engine-0.2.1/LICENCE.md` & `fusion-engine-0.2.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.1/PKG-INFO` & `fusion-engine-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.1
-Summary: This a fully custom engine based on Python and PySDL2, it's written in pure python and is using rust for ui.
+Version: 0.2.2
+Summary: This a fully custom engine based on Python and PySDL2, it's written in pure Python!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -86,22 +86,35 @@
   - [x] Draw images
   - [x] Input
   - [x] Storage system
   - [x] Rendering options
   - [x] Delta-Time
   - [x] Pip package and SetupTools
   - [ ] Physics system using PyMunk
-- [ ] UI (Rust)
+    - [x] Gravity
+    - [x] Rendering
+    - [ ] Collision system
+    - [ ] Physics shapes
+  - [ ] GUI library
+    - [x] Text
+    - [x] Drawing (Build in draw function)
+    - [ ] Buttons
+    - [ ] And more...
+  - [ ] Sound system
+    - [ ] Sound player
+    - [ ] File support
+    - [ ] And more...
+- [ ] UI (Using own GUI library)
   - [ ] Menu
   - [ ] Create project
   - [ ] Editor
   - [ ] Code editor build in
   - [ ] Run game
 
-- If you have more ideas, please tell us them in our discord group!
+- If you have more ideas, please tell us them in our [discord group](https://discord.gg/Smg3CK4ZMc)!
 
 ## 🗄️ About
 
 Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
 
 - PySDL2 is used for rendering and windowing
 - PySDL2-DLL is used by PySDL2 for SDL2 binaries
```

### Comparing `fusion-engine-0.2.1/README.md` & `fusion-engine-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -59,22 +59,35 @@
   - [x] Draw images
   - [x] Input
   - [x] Storage system
   - [x] Rendering options
   - [x] Delta-Time
   - [x] Pip package and SetupTools
   - [ ] Physics system using PyMunk
-- [ ] UI (Rust)
+    - [x] Gravity
+    - [x] Rendering
+    - [ ] Collision system
+    - [ ] Physics shapes
+  - [ ] GUI library
+    - [x] Text
+    - [x] Drawing (Build in draw function)
+    - [ ] Buttons
+    - [ ] And more...
+  - [ ] Sound system
+    - [ ] Sound player
+    - [ ] File support
+    - [ ] And more...
+- [ ] UI (Using own GUI library)
   - [ ] Menu
   - [ ] Create project
   - [ ] Editor
   - [ ] Code editor build in
   - [ ] Run game
 
-- If you have more ideas, please tell us them in our discord group!
+- If you have more ideas, please tell us them in our [discord group](https://discord.gg/Smg3CK4ZMc)!
 
 ## 🗄️ About
 
 Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
 
 - PySDL2 is used for rendering and windowing
 - PySDL2-DLL is used by PySDL2 for SDL2 binaries
```

### Comparing `fusion-engine-0.2.1/pyproject.toml` & `fusion-engine-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fusion-engine"
-description = "This a fully custom engine based on Python and PySDL2, it's written in pure python and is using rust for ui."
+description = "This a fully custom engine based on Python and PySDL2, it's written in pure Python!"
 requires-python = ">=3.7"
 license = {text = "LICENSE.md"}
 authors = [{name = "Dimkauzh", email = "uzhdimka@gmail.com"}]
 keywords = ["game", "python", "gamedev", "game-engine", "sdl2",
     "game-development", "pure-python", "sdl2-mixer", "sdl2-ttf", "sdl2-image",
     "python-game", "pysdl2", "sdl2-library", "python-game-library",
     "python-game-engine", "python-games"]
@@ -38,8 +38,8 @@
 dependencies = {file = "requirements.txt"}
 
 [tool.setuptools.package-data]
 fusionengine = ["**/*.png"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
-exclude = ["gui"]
+exclude = ["old_gui"]
```

### Comparing `fusion-engine-0.2.1/setup.py` & `fusion-engine-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.1/src/fusion_engine.egg-info/PKG-INFO` & `fusion-engine-0.2.2/src/fusion_engine.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.1
-Summary: This a fully custom engine based on Python and PySDL2, it's written in pure python and is using rust for ui.
+Version: 0.2.2
+Summary: This a fully custom engine based on Python and PySDL2, it's written in pure Python!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -86,22 +86,35 @@
   - [x] Draw images
   - [x] Input
   - [x] Storage system
   - [x] Rendering options
   - [x] Delta-Time
   - [x] Pip package and SetupTools
   - [ ] Physics system using PyMunk
-- [ ] UI (Rust)
+    - [x] Gravity
+    - [x] Rendering
+    - [ ] Collision system
+    - [ ] Physics shapes
+  - [ ] GUI library
+    - [x] Text
+    - [x] Drawing (Build in draw function)
+    - [ ] Buttons
+    - [ ] And more...
+  - [ ] Sound system
+    - [ ] Sound player
+    - [ ] File support
+    - [ ] And more...
+- [ ] UI (Using own GUI library)
   - [ ] Menu
   - [ ] Create project
   - [ ] Editor
   - [ ] Code editor build in
   - [ ] Run game
 
-- If you have more ideas, please tell us them in our discord group!
+- If you have more ideas, please tell us them in our [discord group](https://discord.gg/Smg3CK4ZMc)!
 
 ## 🗄️ About
 
 Fusion Engine is currently (6/14/2023) build with Python and some Python libraries:
 
 - PySDL2 is used for rendering and windowing
 - PySDL2-DLL is used by PySDL2 for SDL2 binaries
```

### Comparing `fusion-engine-0.2.1/src/fusion_engine.egg-info/SOURCES.txt` & `fusion-engine-0.2.2/src/fusion_engine.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 src/fusionengine/files/exceptions.py
 src/fusionengine/files/image.py
 src/fusionengine/files/imports.py
 src/fusionengine/files/physics.py
 src/fusionengine/files/shape.py
 src/fusionengine/files/storage.py
 src/fusionengine/files/systems.py
-src/fusionengine/files/window.py
-src/old_gui/gui.py
+src/fusionengine/files/ui.py
+src/fusionengine/files/window.py
```

### Comparing `fusion-engine-0.2.1/src/fusionengine/__init__.py` & `fusion-engine-0.2.2/src/fusionengine/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 __author__ = "Dimkauzh"
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 import fusionengine.files.data as data
 import fusionengine.files.systems as sysconfig
 
 from fusionengine.files.imports import *
 
 class Main:
     def __init__(self):
-        SDL_Init(SDL_INIT_VIDEO)
+        sdl2.SDL_Init(sdl2.SDL_INIT_VIDEO)
         self.window = window.Window()
         self.color = color.Colors()
         self.event = event.Event()
         self.keys = event.Keys()
         self.draw = draw.Draw()
         self.image = image.Image()
         self.body = body
         self.system = sysconfig.System()
         self.rendereroptions = sysconfig.RendererOptions()
         self.shape = shape.Shapes()
-        
+        self.ui = ui.UI()
+
         self.DEBUGIMAGE = "src/fusionengine/debugfiles/fe.png"
 
     def quit(self, window):
-        SDL_DestroyRenderer(window.renderer)
-        SDL_DestroyWindow(window.window)
+        sdl2.SDL_DestroyRenderer(window.renderer)
+        sdl2.SDL_DestroyWindow(window.window)
         del window
-        SDL_Quit()
+        sdl2.SDL_Quit()
```

### Comparing `fusion-engine-0.2.1/src/fusionengine/debugfiles/fe.png` & `fusion-engine-0.2.2/src/fusionengine/debugfiles/fe.png`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.1/src/fusionengine/files/body.py` & `fusion-engine-0.2.2/src/fusionengine/files/body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import fusionengine.files.data as data
 import fusionengine.files.window as window
 from fusionengine.files.enums import BodyType
 from fusionengine.files.imports import *
-import fusionengine.files.image as image
+import fusionengine.files.image as image_fe
+import fusionengine.files.draw as draw_fe
 
 class _RigidBody:
     def __init__(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
         self._body = data.DataBodies(window, x, y, width, height)
         self.window = window
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.body = self._body.body
         self.space = self._body.space
-        
+
 class _StaticBody:
     def __init__(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
         self._body = data.DataBodies(window, x, y, width, height)
         self.window = window
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.body = self._body.body
         self.space = self._body.space
-    
-class Entity: 
-    def __init__(self, bodytype: BodyType, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
+
+class Entity:
+    def __init__(self, bodytype: str, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
         self._addspace = []
-        self.image = None
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.window = window
         self.gravity = 0
-        
+        self.image_fe = image_fe.Image()
+        self.draw_fe = draw_fe.Draw()
+
         if bodytype == BodyType.RIGID_BODY:
             self.body = _RigidBody(self.window,
                                    self.x,
                                    self.y,
                                    self.width,
                                    self.height
                                    )
@@ -49,45 +51,45 @@
             self.body = _StaticBody(self.window,
                                     self.x,
                                     self.y,
                                     self.width,
                                     self.height
                                     )
             self._addspace.append(self.body.body)
-            
+
         self._set_body_data(self.x, self.y, self.width, self.height, self.body.space)
         self.box = pymunk.Poly.create_box(self.body.body)
         self._addspace.append(self.box)
-        
+
         self._addspaces()
 
-    def image(self, window: window._CustomRenderer, image: str, x: int, y: int, width: int, height: int) -> None:
-        drawimage = image.open_image(window, image, x, y, width, height)
-        image.draw_image(drawimage)
-        self.image = image
+    def image(self, window: window._CustomRenderer, image_path: str, x: int, y: int, width: int, height: int) -> None:
+        drawimage = self.image_fe.open_image(window, image, x, y, width, height)
+        self.image_fe.draw_image(drawimage)
+        self.image_path = image_path
         self.window = window
         self.x = x
         self.y = y
         self.width = width
         self.height = height
 
     def new_rect(self, window: window._CustomRenderer, color: tuple) -> None:
-        data.draw_rect(window,
+        self.draw_fe.draw_rect(window,
                       self.x,
                       self.y,
                       self.width,
                       self.height,
                       color
                       )
     def set_gravity(self, gravity: int) -> None:
         self.gravity = gravity
         self.body.space.gravity = self.gravity
-    
+
     def set_mass(self, mass: int) -> None:
         self.box.mass = mass
-    
+
     def _set_body_data(self, x, y, width, height, space) -> None:
         space.position = x, y
-    
+
     def _addspaces(self) -> None:
         for space in self._addspace:
-            self.body.space.add(space)
+            self.body.space.add(space)
```

### Comparing `fusion-engine-0.2.1/src/fusionengine/files/color.py` & `fusion-engine-0.2.2/src/fusionengine/files/color.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.1/src/fusionengine/files/event.py` & `fusion-engine-0.2.2/src/fusionengine/files/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def key_down(self, key: int, window: window._CustomRenderer) -> bool:
         event = window.event
         if event.type == sdl2.SDL_KEYDOWN:
             if event.key.keysym.sym == key:
                 return True
         return False
     def key_down_once(self, key: int, window: window._CustomRenderer) -> bool:
-        pass
+        return False
 
 
 class Keys:
     def __init__(self):
         self.KEY_UNKNOWN = sdl2.SDLK_UNKNOWN
         self.KEY_RETURN = sdl2.SDLK_RETURN
         self.KEY_ESCAPE = sdl2.SDLK_ESCAPE
```

### Comparing `fusion-engine-0.2.1/src/fusionengine/files/image.py` & `fusion-engine-0.2.2/src/fusionengine/files/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 class _CustomImage:
     def __init__(self, window: window._CustomRenderer, texture, rect: shape._CustomShape) -> None:
         self.window = window
         self.renderer = window.renderer
         self.texture = texture
         self.rect = rect
 
-class Image: 
+class Image:
     def open_image(self, window: window._CustomRenderer, image, x: int, y: int, width: int, height: int) -> _CustomImage:
         image = sdl2.ext.load_image(image)
         texture = sdl2.SDL_CreateTextureFromSurface(window.renderer, image)
         rect = sdl2.SDL_Rect(x, y, width, height)
         return _CustomImage(window, texture, rect)
-    
+
     def draw_image(self, image: _CustomImage) -> None:
         sdl2.SDL_RenderClear(image.renderer)
         sdl2.SDL_RenderCopy(image.renderer, image.texture, None, image.rect)
```

### Comparing `fusion-engine-0.2.1/src/fusionengine/files/shape.py` & `fusion-engine-0.2.2/src/fusionengine/files/shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 class _CustomShape:
     def __init__(self, x: int, y: int, width: int, height: int, color: tuple) -> None:
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.color = color
-        self.rect = SDL_Rect(x, y, width, height)
+        self.rect = sdl2.SDL_Rect(x, y, width, height)
 
 class Shapes:
     def __init__(self) -> None:
         pass
-    
+
     def new_rect(self, x: int, y: int, width: int, height: int, color: tuple) -> _CustomShape:
         return _CustomShape(x, y, width, height, color)
```

### Comparing `fusion-engine-0.2.1/src/fusionengine/files/storage.py` & `fusion-engine-0.2.2/src/fusionengine/files/storage.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.1/src/fusionengine/files/systems.py` & `fusion-engine-0.2.2/src/fusionengine/files/systems.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from fusionengine.files.enums import RendererFlag
 from fusionengine.files.imports import *
 
 class RendererOptions:
     def __init__(self) -> None:
-        self.rendererflag = SDL_RENDERER_ACCELERATED
+        self.rendererflag = sdl2.SDL_RENDERER_ACCELERATED
     def getSurfaceFromWindow(self, window):
         return window.surface
     def setRendererFlag(self, flag: RendererFlag) -> None:
         if flag == RendererFlag.PREVENT_SYNC:
-            self.rendererflag = SDL_RENDERER_PRESENTVSYNC
+            self.rendererflag = sdl2.SDL_RENDERER_PRESENTVSYNC
         elif flag == RendererFlag.SOFTWARE:
-            self.rendererflag = SDL_RENDERER_SOFTWARE
+            self.rendererflag = sdl2.SDL_RENDERER_SOFTWARE
         elif flag == RendererFlag.TARGET_TEXTURE:
-            self.rendererflag = SDL_RENDERER_TARGETTEXTURE
+            self.rendererflag = sdl2.SDL_RENDERER_TARGETTEXTURE
         else:
-            self.rendererflag = SDL_RENDERER_ACCELERATED
+            self.rendererflag = sdl2.SDL_RENDERER_ACCELERATED
 
 class System:
     def __init__(self):
         pass
```

### Comparing `fusion-engine-0.2.1/src/fusionengine/files/window.py` & `fusion-engine-0.2.2/src/fusionengine/files/draw.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 import fusionengine.files.systems as sysconfig
-from fusionengine.files.imports import *
+import fusionengine.files.window as window
 
-class _CustomRenderer:
-    def __init__(self, window: SDL_CreateWindow) -> None:
-        self.window = window
-        self.event = SDL_Event()
-        self.renderer = SDL_CreateRenderer(self.window, -1, sysconfig.RendererOptions().rendererflag)
+from fusionengine.files.imports import *
+import fusionengine.files.shape as shape
 
-class Window:
+class Draw:
     def __init__(self) -> None:
-        self.window = None
-        self._running = False
-        self._NOW = SDL_GetPerformanceCounter()
-        self._LAST = 0
-        self.DELTATIME = 0
-        self._entity = []
-    
-    def new_window(self, title: str, width: int, height: int) -> _CustomRenderer:
-        encoded_title = title.encode('utf-8')
-        self.window_window = SDL_CreateWindow(encoded_title,
-                                       SDL_WINDOWPOS_CENTERED,
-                                       SDL_WINDOWPOS_CENTERED,
-                                       width,
-                                       height,
-                                       SDL_WINDOW_SHOWN
-                                       )
-        self._running = True
-        self.window = _CustomRenderer(self.window_window)
-        return self.window
-    
-    def loop(self, your_loop):
-        while self.running(self.window):
-            your_loop()
-    
-    def running(self, window:_CustomRenderer) -> bool:
-        self._refresh(window)
-        return self._running
-    
-    def _refresh(self, window: _CustomRenderer) -> None:
-        SDL_UpdateWindowSurface(window.window)
-        SDL_RenderPresent(window.renderer)
-        
-        self._LAST = self._NOW
-        self._NOW = SDL_GetPerformanceCounter()
-
-        
-        
-        self.DELTATIME = (self._NOW - self._LAST)*1000 / SDL_GetPerformanceFrequency()
-               
-        if sdl2.SDL_PollEvent(window.event) != 0:
-            if window.event.type == sdl2.SDL_QUIT:
-                self._running = False
+        self.rendereroptions = sysconfig.RendererOptions()
+
+    def draw_line(self, window: window._CustomRenderer, x1: int, y1: int, x2: int, y2: int, color: tuple) -> None:
+        sdl2.SDL_SetRenderDrawColor(window.renderer,
+                               color[0],
+                               color[1],
+                               color[2],
+                               color[3]
+                               )
+
+        sdl2.SDL_RenderDrawLine(window.renderer, x1, y1, x2, y2)
+
+    def draw_line_rect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
+        rdr = window.renderer
+        self.draw_line(rdr, x, y, x + width, y, color)
+        self.draw_line(rdr, x, y + height, x + width, y + height, color)
+        self.draw_line(rdr, x, y, x, y + height, color)
+        self.draw_line(rdr, x + width, y, x + width, y + height, color)
+
+    def draw_rect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
+        sdl2.SDL_SetRenderDrawColor(window.renderer,
+                               color[0],
+                               color[1],
+                               color[2],
+                               color[3]
+                               )
+
+        rect = sdl2.SDL_Rect(x, y, width, height)
+        sdl2.SDL_RenderFillRect(window.renderer, rect)
+
+    def draw_own_rect(self, window: window._CustomRenderer, rect: shape._CustomShape) -> None:
+        sdl2.SDL_SetRenderDrawColor(window.renderer,
+                               rect.color[0],
+                               rect.color[1],
+                               rect.color[2],
+                               rect.color[3]
+                               )
+
+        sdl2.SDL_RenderFillRect(window.renderer, rect.rect)
+
+    def set_background_color(self, window: window._CustomRenderer, color: tuple) -> None:
+        sdl2.SDL_SetRenderDrawColor(window.renderer,
+                               color[0],
+                               color[1],
+                               color[2],
+                               color[3]
+                               )
 
-        
+        sdl2.SDL_RenderClear(window.renderer)
```

### Comparing `fusion-engine-0.2.1/src/old_gui/gui.py` & `fusion-engine-0.2.2/src/fusionengine/files/window.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,52 @@
-import tkinter as tk
+import fusionengine.files.systems as sysconfig
+from fusionengine.files.imports import *
 
-class CustomItems:
-    def __init__(self, window) -> None:
+class _CustomRenderer:
+    def __init__(self, window: sdl2.SDL_CreateWindow) -> None:
         self.window = window
-    
-    def new_label(self, text: str) -> tk.Label:
-        label = tk.Label(self.window, text=text)
-        label.pack()
-        return label
-    
-    def new_button(self, text: str, function) -> tk.Button:
-        button = tk.Button(self.window, text=text, function=function)
-        button.pack()
-        return button
+        self.event = sdl2.SDL_Event()
+        self.renderer = sdl2.SDL_CreateRenderer(self.window, -1, sysconfig.RendererOptions().rendererflag)
+
+class Window:
+    def __init__(self) -> None:
+        self._running = False
+        self._NOW = sdl2.SDL_GetPerformanceCounter()
+        self._LAST = 0
+        self.DELTATIME = 0
+        self._entity = []
+
+    def new_window(self, title: str, width: int, height: int) -> _CustomRenderer:
+        encoded_title = title.encode('utf-8')
+        self.window_window = sdl2.SDL_CreateWindow(encoded_title,
+                                       sdl2.SDL_WINDOWPOS_CENTERED,
+                                       sdl2.SDL_WINDOWPOS_CENTERED,
+                                       width,
+                                       height,
+                                       sdl2.SDL_WINDOW_SHOWN
+                                       )
+        self._running = True
+        self.window = _CustomRenderer(self.window_window)
+        return self.window
+
+    def loop(self, your_loop):
+        while self.running(self.window):
+            your_loop()
+
+    def running(self, window:_CustomRenderer) -> bool:
+        self._refresh(window)
+        return self._running
+
+    def _refresh(self, window: _CustomRenderer) -> None:
+        sdl2.SDL_UpdateWindowSurface(window.window)
+        sdl2.SDL_RenderPresent(window.renderer)
+
+        self._LAST = self._NOW
+        self._NOW = sdl2.SDL_GetPerformanceCounter()
+
 
-class MenuItems:
-    def __init__(self, window) -> None:
-        self.window = window
-    
-    def get_center_window(self):
-        # get the screen dimension
-        self.screen_width = self.window.winfo_screenwidth()
-        self.screen_height = self.window.winfo_screenheight()
-
-        # find the center point
-        center_x = int(self.screen_width/2 - self.screen_width / 2)
-        center_y = int(self.screen_height/2 - self.screen_height / 2)
-        
-        return center_x, center_y
-
-    def load_icon(self, file):
-        icon = tk.PhotoImage(file = file)
-        self.window.iconphoto(False, icon)
-
-class Menu:
-    def __init__(self):
-        self.window = tk.Tk()
-        self.labels = []
-        
-        self.ci = CustomItems(self.window)
-        self.mi = MenuItems(self.window)
-        
-        self.window_width = 800
-        self.window_height = 600
-        self.window_center = self.mi.get_center_window()
-        
-        self.start()
-        
-    def start(self):
-        self.window.geometry(f"{self.window_width}x{self.window_height}+{self.window_center[0]}+{self.window_center[1]}")
-        self.window.title('Fusion-Engine')
-        self.mi.load_icon("src/gui/assets/icon/fe.png")
-        
-        message = self.ci.new_label("Fusion-Engine")
-        
-        self.window.mainloop()
-        
 
-if __name__ == "__main__":
-    menu = Menu()
+        self.DELTATIME = (self._NOW - self._LAST)*1000 / sdl2.SDL_GetPerformanceFrequency()
+
+        if sdl2.SDL_PollEvent(window.event) != 0:
+            if window.event.type == sdl2.SDL_QUIT:
+                self._running = False
```

