# Comparing `tmp/typetype-1.1.1.tar.gz` & `tmp/typetype-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.1.1.tar", last modified: Tue Jul 11 23:51:32 2023, max compression
+gzip compressed data, was "typetype-1.1.3.tar", last modified: Wed Jul 12 00:54:59 2023, max compression
```

## Comparing `typetype-1.1.1.tar` & `typetype-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.951542 typetype-1.1.1/
--rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.1.1/MANIFEST.in
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-11 23:51:32.951258 typetype-1.1.1/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1397 2023-07-11 23:50:53.000000 typetype-1.1.1/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-11 23:51:32.951611 typetype-1.1.1/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-11 23:51:11.000000 typetype-1.1.1/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.943723 typetype-1.1.1/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.1.1/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     9272 2023-07-11 23:49:26.000000 typetype-1.1.1/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.945297 typetype-1.1.1/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.1.1/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10372 2023-07-11 23:49:31.000000 typetype-1.1.1/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.1.1/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-11 23:49:32.000000 typetype-1.1.1/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.947387 typetype-1.1.1/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.1.1/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.1.1/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.1.1/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-11 22:27:26.000000 typetype-1.1.1/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.1.1/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.944423 typetype-1.1.1/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.851486 typetype-1.1.3/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.1.3/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-12 00:54:59.851365 typetype-1.1.3/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1397 2023-07-11 23:50:53.000000 typetype-1.1.3/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-12 00:54:59.851526 typetype-1.1.3/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-12 00:53:29.000000 typetype-1.1.3/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.846190 typetype-1.1.3/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.1.3/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     9674 2023-07-12 00:52:30.000000 typetype-1.1.3/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.847558 typetype-1.1.3/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.1.3/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10371 2023-07-12 00:18:12.000000 typetype-1.1.3/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.1.3/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-12 00:29:14.000000 typetype-1.1.3/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.849130 typetype-1.1.3/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.1.3/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.1.3/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.1.3/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-12 00:02:56.000000 typetype-1.1.3/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.1.3/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 00:54:59.846874 typetype-1.1.3/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-12 00:54:59.000000 typetype-1.1.3/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.1.1/PKG-INFO` & `typetype-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.1.1
+Version: 1.1.3
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.1.1/README.md` & `typetype-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.1.1/setup.py` & `typetype-1.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='typetype',
-    version='1.1.1',
+    version='1.1.3',
     author='Ahmet Ozer',
     url="https://github.com/ahmet8zer/typetype",
     description='A command line typing game',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `typetype-1.1.1/typetype/ahmetsgame.py` & `typetype-1.1.3/typetype/ahmetsgame.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,29 @@
         cursor = True
     
     #start and setup colors and use the default terminal color as the background
     curses.start_color()
     curses.use_default_colors()
     stdscr.clear()
     #grey
-    curses.init_pair(1, 245, -1)
+    if sys.platform == 'win32':
+        curses.init_pair(1, 240, -1)
+    else:
+        curses.init_pair(1, 235, -1)
     #white
     curses.init_pair(2, curses.COLOR_WHITE, -1)
     #(error)
     curses.init_pair(3, 160, -1)
     #(extra)
     #change color red to a greyish salmon color
     curses.init_color(curses.COLOR_RED, 300, 150, 150)
-    curses.init_pair(4, curses.COLOR_RED, -1)
+    if sys.platform == 'win32':
+        curses.init_pair(4, 88, -1)
+    else:
+        curses.init_pair(4, curses.COLOR_RED, -1)
     #magenta
     curses.init_pair(5, curses.COLOR_MAGENTA, -1)
     
     #prompt user for what type of game they want
     choices = get_game(stdscr)
     if choices == 'q':
         return 
@@ -144,14 +150,20 @@
         if sys.platform == 'win32':
             if (ctypes.windll.user32.GetKeyState(0x09) & 0x8000) and (ctypes.windll.user32.GetKeyState(0x0D) & 0x8000):
                 return start_game(stdscr, choices, cursor)
         try:
             char = chr(key)
         except:
             char = 'NA'
+            
+        if sys.platform == 'win32':
+            if (ctypes.windll.user32.GetKeyState(0x27) & 0x8000):
+                char = "'"
+            elif (ctypes.windll.user32.GetKeyState(0x22) & 0x8000):
+                char = '"'
         
         #end the game if the timer has passed the time limit
         if timed!=0 and time_started:
             if time.time()-start_time>timed:
                 break
         
         #if the function times out, refresh the screen
```

### Comparing `typetype-1.1.1/typetype/functions/game_selection.py` & `typetype-1.1.3/typetype/functions/game_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
                 return choice + '1'
             elif active == 2:
                 return choice + '2'
             elif active == 3:
                 return choice + '3'
             elif active == 4 and choice[0] == 't':
                 return get_mode(stdscr, get_diff(stdscr, choice[:-1]))
-            elif active == 14 and choice[0] == 'w':
+            elif active == 4 and choice[0] == 'w':
                 return choice + '4'
             elif active == 5:
                 return get_mode(stdscr, get_diff(stdscr, choice[:-1]))
         #delete
         elif key == 127 or key == 8:
             return get_mode(stdscr, get_diff(stdscr, choice[:-1]))
```

### Comparing `typetype-1.1.1/typetype/functions/refresh_update.py` & `typetype-1.1.3/typetype/functions/refresh_update.py`

 * *Files identical despite different names*

### Comparing `typetype-1.1.1/typetype/functions/setup_results.py` & `typetype-1.1.3/typetype/functions/setup_results.py`

 * *Files identical despite different names*

### Comparing `typetype-1.1.1/typetype/words/200words.txt` & `typetype-1.1.3/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.1/typetype/words/25000words.txt` & `typetype-1.1.3/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.1/typetype/words/5000words.txt` & `typetype-1.1.3/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.1/typetype/words/text.txt` & `typetype-1.1.3/typetype/words/text.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.1/typetype.egg-info/PKG-INFO` & `typetype-1.1.3/typetype.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.1.1
+Version: 1.1.3
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.1.1/typetype.egg-info/SOURCES.txt` & `typetype-1.1.3/typetype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

