# Comparing `tmp/typetype-1.1.0.tar.gz` & `tmp/typetype-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.1.0.tar", last modified: Tue Jul 11 21:46:40 2023, max compression
+gzip compressed data, was "typetype-1.1.1.tar", last modified: Tue Jul 11 23:51:32 2023, max compression
```

## Comparing `typetype-1.1.0.tar` & `typetype-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.443306 typetype-1.1.0/
--rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.1.0/MANIFEST.in
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-11 21:46:40.443154 typetype-1.1.0/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1358 2023-07-10 23:35:01.000000 typetype-1.1.0/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-11 21:46:40.443352 typetype-1.1.0/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      683 2023-07-11 21:45:24.000000 typetype-1.1.0/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.436918 typetype-1.1.0/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.1.0/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     9072 2023-07-11 21:45:25.000000 typetype-1.1.0/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.438493 typetype-1.1.0/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.1.0/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10372 2023-07-11 17:23:53.000000 typetype-1.1.0/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.1.0/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.439956 typetype-1.1.0/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-11 21:44:48.000000 typetype-1.1.0/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.1.0/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 21:46:40.437743 typetype-1.1.0/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1555 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      550 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/requires.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 21:46:40.000000 typetype-1.1.0/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.951542 typetype-1.1.1/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.1.1/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-11 23:51:32.951258 typetype-1.1.1/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1397 2023-07-11 23:50:53.000000 typetype-1.1.1/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-11 23:51:32.951611 typetype-1.1.1/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-11 23:51:11.000000 typetype-1.1.1/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.943723 typetype-1.1.1/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.1.1/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     9272 2023-07-11 23:49:26.000000 typetype-1.1.1/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.945297 typetype-1.1.1/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.1.1/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10372 2023-07-11 23:49:31.000000 typetype-1.1.1/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.1.1/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-11 23:49:32.000000 typetype-1.1.1/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.947387 typetype-1.1.1/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.1.1/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.1.1/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.1.1/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-11 22:27:26.000000 typetype-1.1.1/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.1.1/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-11 23:51:32.944423 typetype-1.1.1/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-11 23:51:32.000000 typetype-1.1.1/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.1.0/PKG-INFO` & `typetype-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: typetype
-Version: 1.1.0
-Summary: A command line typing game
-Home-page: https://github.com/ahmet8zer/typetype
-Author: Ahmet Ozer
-Description-Content-Type: text/markdown
-
 # typetype
 A Command Line Typing Game by Ahmet Ozer
 
 ## Installation
 To install typetype, use the following command:
  `pip install typetype`
 
@@ -32,13 +24,14 @@
 - Press the Enter key to confirm the selected mode.
 - Press the Delete key to go back to the previous game.
 - Press the Esc key to quit the game (only applicable on the first page).
 
 ### Inside The Game:
 - Simply start typing to play the game!
 - Press the Esc key to restart the game.
+- Press tab+enter to restart the game.
 - If the timer hasn't started yet, press * to return to the menu.
 
 ### Results/End Page:
 - Use the Esc key to quit the game.
```

### Comparing `typetype-1.1.0/README.md` & `typetype-1.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: typetype
+Version: 1.1.1
+Summary: A command line typing game
+Home-page: https://github.com/ahmet8zer/typetype
+Author: Ahmet Ozer
+Description-Content-Type: text/markdown
+
 # typetype
 A Command Line Typing Game by Ahmet Ozer
 
 ## Installation
 To install typetype, use the following command:
  `pip install typetype`
 
@@ -24,13 +32,14 @@
 - Press the Enter key to confirm the selected mode.
 - Press the Delete key to go back to the previous game.
 - Press the Esc key to quit the game (only applicable on the first page).
 
 ### Inside The Game:
 - Simply start typing to play the game!
 - Press the Esc key to restart the game.
+- Press tab+enter to restart the game.
 - If the timer hasn't started yet, press * to return to the menu.
 
 ### Results/End Page:
 - Use the Esc key to quit the game.
```

### Comparing `typetype-1.1.0/setup.py` & `typetype-1.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import sys
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='typetype',
-    version='1.1.0',
+    version='1.1.1',
     author='Ahmet Ozer',
     url="https://github.com/ahmet8zer/typetype",
     description='A command line typing game',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'typetype=typetype.ahmetsgame:callmain'
         ]
     },
     install_requires=[
-] + (['windows-curses','keyboard'] if sys.platform == 'win32' else ['keyboard'])
+] + (['windows-curses'] if sys.platform == 'win32' else [])
 )
```

### Comparing `typetype-1.1.0/typetype/ahmetsgame.py` & `typetype-1.1.1/typetype/ahmetsgame.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         cursor = True
     
     #start and setup colors and use the default terminal color as the background
     curses.start_color()
     curses.use_default_colors()
     stdscr.clear()
     #grey
-    curses.init_color(curses.COLOR_CYAN, 500, 500, 500)
-    curses.init_pair(1, curses.COLOR_CYAN, -1)
+    curses.init_pair(1, 245, -1)
     #white
     curses.init_pair(2, curses.COLOR_WHITE, -1)
     #(error)
     curses.init_pair(3, 160, -1)
     #(extra)
     #change color red to a greyish salmon color
     curses.init_color(curses.COLOR_RED, 300, 150, 150)
@@ -137,14 +136,18 @@
     while True:
         
         #allow the getch() function to timeout so we can refresh the screen every 0.3 seconds
         stdscr.timeout(300)
         
         #wait for an input key
         key = stdscr.getch()
+        #if tab+enter is pressed then restart the game (like esc)
+        if sys.platform == 'win32':
+            if (ctypes.windll.user32.GetKeyState(0x09) & 0x8000) and (ctypes.windll.user32.GetKeyState(0x0D) & 0x8000):
+                return start_game(stdscr, choices, cursor)
         try:
             char = chr(key)
         except:
             char = 'NA'
         
         #end the game if the timer has passed the time limit
         if timed!=0 and time_started:
@@ -257,8 +260,7 @@
 #used to call main
 def callmain():
     #this is to take away the escape delay
     os.environ.setdefault('ESCDELAY', '25')
     #run main
     curses.wrapper(main)
 
-callmain()
```

### Comparing `typetype-1.1.0/typetype/functions/game_selection.py` & `typetype-1.1.1/typetype/functions/game_selection.py`

 * *Files identical despite different names*

### Comparing `typetype-1.1.0/typetype/functions/refresh_update.py` & `typetype-1.1.1/typetype/functions/refresh_update.py`

 * *Files identical despite different names*

### Comparing `typetype-1.1.0/typetype/functions/setup_results.py` & `typetype-1.1.1/typetype/functions/setup_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 #setup the colors that will be used for the text and return the text for the user
 def setup(stdscr, choices):
 
     #choose sentence from sentences
     if choices[0] == 'x':
-        lines = open(os.path.dirname(os.path.dirname(__file__ ))+"/words/text.txt").readlines()
+        lines = open(os.path.dirname(os.path.dirname(__file__ ))+"/words/text.txt",'r',encoding='utf-8').readlines()
     elif choices[0] != 'x' and choices[1] == 'e':
         lines = open(os.path.dirname(os.path.dirname(__file__)) +"/words/200words.txt").readlines()
     elif choices[0] != 'x' and choices[1] == 'm':
         lines = open(os.path.dirname(os.path.dirname(__file__)) +"/words/5000words.txt").readlines()
     elif choices[0] != 'x' and choices[1] == 'h':
         lines = open(os.path.dirname(os.path.dirname(__file__)) +"/words/25000words.txt").readlines()
```

### Comparing `typetype-1.1.0/typetype/words/200words.txt` & `typetype-1.1.1/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.0/typetype/words/25000words.txt` & `typetype-1.1.1/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.0/typetype/words/5000words.txt` & `typetype-1.1.1/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.0/typetype/words/text.txt` & `typetype-1.1.1/typetype/words/text.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.1.0/typetype.egg-info/PKG-INFO` & `typetype-1.1.1/typetype.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.1.0
+Version: 1.1.1
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
@@ -32,13 +32,14 @@
 - Press the Enter key to confirm the selected mode.
 - Press the Delete key to go back to the previous game.
 - Press the Esc key to quit the game (only applicable on the first page).
 
 ### Inside The Game:
 - Simply start typing to play the game!
 - Press the Esc key to restart the game.
+- Press tab+enter to restart the game.
 - If the timer hasn't started yet, press * to return to the menu.
 
 ### Results/End Page:
 - Use the Esc key to quit the game.
```

### Comparing `typetype-1.1.0/typetype.egg-info/SOURCES.txt` & `typetype-1.1.1/typetype.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 setup.py
 typetype/__init__.py
 typetype/ahmetsgame.py
 typetype.egg-info/PKG-INFO
 typetype.egg-info/SOURCES.txt
 typetype.egg-info/dependency_links.txt
 typetype.egg-info/entry_points.txt
-typetype.egg-info/requires.txt
 typetype.egg-info/top_level.txt
 typetype/functions/__init__.py
 typetype/functions/game_selection.py
 typetype/functions/refresh_update.py
 typetype/functions/setup_results.py
 typetype/words/200words.txt
 typetype/words/25000words.txt
```

