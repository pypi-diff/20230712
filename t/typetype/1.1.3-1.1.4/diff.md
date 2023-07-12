# Comparing `tmp/typetype-1.1.3.tar.gz` & `tmp/typetype-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.1.3.tar", last modified: Wed Jul 12 00:54:59 2023, max compression
+gzip compressed data, was "typetype-1.1.4.tar", last modified: Wed Jul 12 01:37:53 2023, max compression
```

## Comparing `typetype-1.1.3.tar` & `typetype-1.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.851486 typetype-1.1.3/
--rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.1.3/MANIFEST.in
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-12 00:54:59.851365 typetype-1.1.3/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1397 2023-07-11 23:50:53.000000 typetype-1.1.3/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-12 00:54:59.851526 typetype-1.1.3/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-12 00:53:29.000000 typetype-1.1.3/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.846190 typetype-1.1.3/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.1.3/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     9674 2023-07-12 00:52:30.000000 typetype-1.1.3/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.847558 typetype-1.1.3/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.1.3/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10371 2023-07-12 00:18:12.000000 typetype-1.1.3/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.1.3/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-12 00:29:14.000000 typetype-1.1.3/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.849130 typetype-1.1.3/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.1.3/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.1.3/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.1.3/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-12 00:02:56.000000 typetype-1.1.3/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.1.3/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.846874 typetype-1.1.3/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 01:37:53.485977 typetype-1.1.4/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.1.4/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-12 01:37:53.485838 typetype-1.1.4/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1397 2023-07-11 23:50:53.000000 typetype-1.1.4/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-12 01:37:53.486026 typetype-1.1.4/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-12 01:29:41.000000 typetype-1.1.4/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 01:37:53.480052 typetype-1.1.4/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.1.4/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     9776 2023-07-12 01:36:13.000000 typetype-1.1.4/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 01:37:53.481549 typetype-1.1.4/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.1.4/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10371 2023-07-12 01:36:32.000000 typetype-1.1.4/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.1.4/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-12 00:29:14.000000 typetype-1.1.4/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 01:37:53.483401 typetype-1.1.4/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.1.4/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.1.4/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.1.4/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-12 01:36:37.000000 typetype-1.1.4/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.1.4/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 01:37:53.480720 typetype-1.1.4/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-12 01:37:53.000000 typetype-1.1.4/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-12 01:37:53.000000 typetype-1.1.4/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-12 01:37:53.000000 typetype-1.1.4/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-12 01:37:53.000000 typetype-1.1.4/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-12 01:37:53.000000 typetype-1.1.4/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.1.3/PKG-INFO` & `typetype-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.1.3
+Version: 1.1.4
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.1.3/README.md` & `typetype-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.1.3/setup.py` & `typetype-1.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='typetype',
-    version='1.1.3',
+    version='1.1.4',
     author='Ahmet Ozer',
     url="https://github.com/ahmet8zer/typetype",
     description='A command line typing game',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `typetype-1.1.3/typetype/ahmetsgame.py` & `typetype-1.1.4/typetype/ahmetsgame.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     curses.start_color()
     curses.use_default_colors()
     stdscr.clear()
     #grey
     if sys.platform == 'win32':
         curses.init_pair(1, 240, -1)
     else:
-        curses.init_pair(1, 235, -1)
+        curses.init_pair(1, 232, -1)
     #white
     curses.init_pair(2, curses.COLOR_WHITE, -1)
     #(error)
     curses.init_pair(3, 160, -1)
     #(extra)
     #change color red to a greyish salmon color
     curses.init_color(curses.COLOR_RED, 300, 150, 150)
@@ -152,18 +152,20 @@
                 return start_game(stdscr, choices, cursor)
         try:
             char = chr(key)
         except:
             char = 'NA'
             
         if sys.platform == 'win32':
-            if (ctypes.windll.user32.GetKeyState(0x27) & 0x8000):
-                char = "'"
-            elif (ctypes.windll.user32.GetKeyState(0x22) & 0x8000):
+            if (ctypes.windll.user32.GetKeyState(0xDE) & 0x8000) and (ctypes.windll.user32.GetKeyState(0x10) & 0x8000):
                 char = '"'
+                key = 0
+            elif (ctypes.windll.user32.GetKeyState(0xDE) & 0x8000):
+                char = "'"
+                key = 0
         
         #end the game if the timer has passed the time limit
         if timed!=0 and time_started:
             if time.time()-start_time>timed:
                 break
         
         #if the function times out, refresh the screen
```

### Comparing `typetype-1.1.3/typetype/functions/game_selection.py` & `typetype-1.1.4/typetype/functions/game_selection.py`

 * *Files identical despite different names*

### Comparing `typetype-1.1.3/typetype/functions/refresh_update.py` & `typetype-1.1.4/typetype/functions/refresh_update.py`

 * *Files identical despite different names*

### Comparing `typetype-1.1.3/typetype/functions/setup_results.py` & `typetype-1.1.4/typetype/functions/setup_results.py`

 * *Files identical despite different names*

### Comparing `typetype-1.1.3/typetype/words/200words.txt` & `typetype-1.1.4/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.3/typetype/words/25000words.txt` & `typetype-1.1.4/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.3/typetype/words/5000words.txt` & `typetype-1.1.4/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.3/typetype/words/text.txt` & `typetype-1.1.4/typetype/words/text.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.3/typetype.egg-info/PKG-INFO` & `typetype-1.1.4/typetype.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.1.3
+Version: 1.1.4
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.1.3/typetype.egg-info/SOURCES.txt` & `typetype-1.1.4/typetype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

