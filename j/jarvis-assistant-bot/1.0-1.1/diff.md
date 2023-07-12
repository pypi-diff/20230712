# Comparing `tmp/jarvis_assistant_bot-1.0.tar.gz` & `tmp/jarvis_assistant_bot-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis_assistant_bot-1.0.tar", last modified: Wed Jul 12 20:32:18 2023, max compression
+gzip compressed data, was "jarvis_assistant_bot-1.1.tar", last modified: Wed Jul 12 21:02:55 2023, max compression
```

## Comparing `jarvis_assistant_bot-1.0.tar` & `jarvis_assistant_bot-1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 20:32:18.630553 jarvis_assistant_bot-1.0/
--rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-1.0/LICENSE
--rw-rw-rw-   0        0        0      689 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6070 2023-07-12 20:32:18.629554 jarvis_assistant_bot-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4909 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 20:32:18.558300 jarvis_assistant_bot-1.0/game/
--rw-rw-rw-   0        0        0    10624 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.0/game/game.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:32:18.576553 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/
--rw-rw-rw-   0        0        0     6070 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       72 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1081 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 20:32:18.630553 jarvis_assistant_bot-1.0/setup.cfg
--rw-rw-rw-   0        0        0      746 2023-07-12 20:31:31.000000 jarvis_assistant_bot-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:32:18.628558 jarvis_assistant_bot-1.0/src/
--rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-1.0/src/__init__.py
--rw-rw-rw-   0        0        0    13208 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.0/src/commands.py
--rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-1.0/src/common_functions.py
--rw-rw-rw-   0        0        0     5590 2023-07-12 12:45:11.000000 jarvis_assistant_bot-1.0/src/main.py
--rw-rw-rw-   0        0        0    18393 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.0/src/memory.py
--rw-rw-rw-   0        0        0     5186 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.0/src/notes_core.py
--rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.0/src/open_ai_input_assistent.py
--rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.0/src/save_load_books.py
--rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-1.0/src/sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 21:02:55.255920 jarvis_assistant_bot-1.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-1.1/LICENSE
+-rw-rw-rw-   0        0        0      784 2023-07-12 20:57:02.000000 jarvis_assistant_bot-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6070 2023-07-12 21:02:55.251913 jarvis_assistant_bot-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4909 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 21:02:55.216309 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/
+-rw-rw-rw-   0        0        0     6070 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-12 21:02:55.000000 jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-07-12 21:00:06.000000 jarvis_assistant_bot-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 21:02:55.255920 jarvis_assistant_bot-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-07-12 21:02:45.000000 jarvis_assistant_bot-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 21:02:55.250820 jarvis_assistant_bot-1.1/src/
+-rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-1.1/src/__init__.py
+-rw-rw-rw-   0        0        0    13213 2023-07-12 20:56:24.000000 jarvis_assistant_bot-1.1/src/commands.py
+-rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-1.1/src/common_functions.py
+-rw-rw-rw-   0        0        0    10652 2023-07-12 20:51:04.000000 jarvis_assistant_bot-1.1/src/goose_game.py
+-rw-rw-rw-   0        0        0     5590 2023-07-12 12:45:11.000000 jarvis_assistant_bot-1.1/src/main.py
+-rw-rw-rw-   0        0        0    18393 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.1/src/memory.py
+-rw-rw-rw-   0        0        0     5186 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.1/src/notes_core.py
+-rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.1/src/open_ai_input_assistent.py
+-rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.1/src/save_load_books.py
+-rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-1.1/src/sorter.py
```

### Comparing `jarvis_assistant_bot-1.0/LICENSE` & `jarvis_assistant_bot-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.0/MANIFEST.in` & `jarvis_assistant_bot-1.1/MANIFEST.in`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 tp_personal_assistant/
     src/
         __init__.py
         commands.py
         common_functions.py
         main.py
         memory.py
+        goose_game.py
         notes_core.py
         save_load_books.py
         open_ai_input_assistent.py
         sorter.py
-    game/
-        goose/
-            1-1.png
-            1-2.png
-            1-3.png
-            1-4.png
-            1-5.png
-        background.png
-        background2.png
-        bomb.png
-        bonus.png
-        bonus2.png
-        enemy.png
-        enemy2.png
-        game.py
-        goose_doose.jpg
-        player.png
+        game/
+            goose/
+                1-1.png
+                1-2.png
+                1-3.png
+                1-4.png
+                1-5.png
+            __init__.py
+            background.png
+            background2.png
+            bomb.png
+            bonus.png
+            bonus2.png
+            enemy.png
+            enemy2.png
+            goose_doose.jpg
+            player.png
     setup.py
     LICENSE
     MANIFEST.in
     CODE_OF_CONDUCT.md
     pyproject.toml
     README.md
```

### Comparing `jarvis_assistant_bot-1.0/PKG-INFO` & `jarvis_assistant_bot-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis_assistant_bot
-Version: 1.0
+Version: 1.1
 Summary: Jarvis is a personal assistant application that allows you to manage your address book with contacts. The application provides features to add, remove, change, save, and load contacts, making it easier to organize your personal or professional network. In addition, Jarvis integrates with ChatGPT, an AI language model, to provide interactive chat functionality. And to add some entertainment after a hard working day, Jarvis also includes a fun game about Bandera-goose.
 Home-page: https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654
 Author: Dmytro Filin, Illya Grygoriev, Dmytro Klymenko, Dmytro Paukov, Alexandr 
 Project-URL: Homepage, https://github.com/UkrainianEagleOwl/tp_personal_assistant
 Project-URL: Bug Tracker, https://github.com/UkrainianEagleOwl/tp_personal_assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jarvis_assistant_bot-1.0/README.md` & `jarvis_assistant_bot-1.1/README.md`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.0/game/game.py` & `jarvis_assistant_bot-1.1/src/goose_game.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,53 +21,53 @@
 
     FPS = pygame.time.Clock()
 
     screen = width, height = 1280, 720
 
     main_surface = pygame.display.set_mode(screen)
 
-    IMGS_PATH = 'game/goose'
+    IMGS_PATH = 'src/game/goose'
 
     # player = pygame.Surface((20, 20))
     # player.fill((WHITE))
     player_imgs = [pygame.image.load(IMGS_PATH + '/' + file).convert_alpha() for file in listdir(IMGS_PATH)]
     player = player_imgs[0]
     player_rect = player.get_rect()
     player_speed = 10
 
     def create_enemy():
         # enemy = pygame.Surface((20, 20))
         # enemy.fill((RED))
-        enemy = pygame.image.load('game/enemy2.png').convert_alpha()
+        enemy = pygame.image.load('src/game/enemy2.png').convert_alpha()
         enemy_rect = pygame.Rect(width + enemy.get_width(), random.randint(0, height - enemy.get_height()), *enemy.get_size())
         enemy_speed = random.randint(6,10)
         return [enemy, enemy_rect, enemy_speed]
 
     def create_bonus():
         # bonus = pygame.Surface((20, 20))
         # bonus.fill((GREEN))
-        bonus = pygame.image.load('game/bonus2.png').convert_alpha()
+        bonus = pygame.image.load('src/game/bonus2.png').convert_alpha()
         bonus_rect = pygame.Rect(random.randint(0, width - bonus.get_width()), -bonus.get_height(), *bonus.get_size())
         bonus_speed = random.randint(4,7)
         return [bonus, bonus_rect, bonus_speed]
 
     def create_bomb():
-        bomb = pygame.image.load('game/bomb.png').convert_alpha()
+        bomb = pygame.image.load('src/game/bomb.png').convert_alpha()
         bomb_rect = player_rect
         bomb_speed = random.randint(5,8)
         return [bomb, bomb_rect, bomb_speed]
 
     def handle_events():
         for event in pygame.event.get():
             if event.type == pygame.KEYDOWN:
                 if event.key == pygame.K_SPACE and bombs != 0:
                     bombss.append(create_bomb())
                     bombs -= 1
 
-    bg = pygame.transform.scale(pygame.image.load('game/background2.png').convert(), screen)
+    bg = pygame.transform.scale(pygame.image.load('src/game/background2.png').convert(), screen)
     bgX = 0
     bgX2 = bg.get_width()
     bg_speed = 5
 
     CREATE_ENEMY = pygame.USEREVENT + 1 
     pygame.time.set_timer(CREATE_ENEMY, 1000)
 
@@ -102,15 +102,15 @@
                     pygame.quit()
 
                 elif event.type == pygame.KEYDOWN:
                     if event.key == pygame.K_ESCAPE:
                         pygame.quit()
 
                         
-            custom_image = pygame.image.load('game/goose_doose.jpg').convert_alpha()
+            custom_image = pygame.image.load('src/game/goose_doose.jpg').convert_alpha()
             custom_image_rect = custom_image.get_rect(center=(width // 2, height // 2))
             main_surface.blit(custom_image, custom_image_rect)
             
             game_over_text = font.render("Гра закінчена!", True, WHITE)
             game_over_rect = game_over_text.get_rect(center=(width // 2 + 150, height // 2 - 100))
             main_surface.blit(game_over_text, game_over_rect)
             
@@ -126,15 +126,15 @@
         
     while start_screen:
         
         # Код для відображення початкового екрану
         main_surface.blit(bg, (0, 0))
         
         # Власна картинка та напис
-        custom_image = pygame.image.load('game/background.png').convert_alpha()
+        custom_image = pygame.image.load('src/game/background.png').convert_alpha()
         custom_image_rect = custom_image.get_rect(center=(width // 2, height // 2))
         main_surface.blit(custom_image, custom_image_rect)
 
         text = font.render("Натисніть будь-яку клавішу, щоб грати", True, BLACK)
         text_rect = text.get_rect(center=(width // 2, height // 2 + 100))
         main_surface.blit(text, text_rect)
```

### Comparing `jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/PKG-INFO` & `jarvis_assistant_bot-1.1/jarvis_assistant_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-assistant-bot
-Version: 1.0
+Version: 1.1
 Summary: Jarvis is a personal assistant application that allows you to manage your address book with contacts. The application provides features to add, remove, change, save, and load contacts, making it easier to organize your personal or professional network. In addition, Jarvis integrates with ChatGPT, an AI language model, to provide interactive chat functionality. And to add some entertainment after a hard working day, Jarvis also includes a fun game about Bandera-goose.
 Home-page: https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654
 Author: Dmytro Filin, Illya Grygoriev, Dmytro Klymenko, Dmytro Paukov, Alexandr 
 Project-URL: Homepage, https://github.com/UkrainianEagleOwl/tp_personal_assistant
 Project-URL: Bug Tracker, https://github.com/UkrainianEagleOwl/tp_personal_assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jarvis_assistant_bot-1.0/pyproject.toml` & `jarvis_assistant_bot-1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jarvis_assistant_bot"
-version = "1.0"
+version = "1.001"
 authors = [
   { name="Dmytro Filin"},
   { name="Illya Grygoriev"},
   { name="Dmytro Klymenko"},
   { name="Dmytro Paukov"},
   { name="Alexandr "}
 ]
```

### Comparing `jarvis_assistant_bot-1.0/setup.py` & `jarvis_assistant_bot-1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name='jarvis_assistant_bot',
-    version='1.0',
+    version='1.01',
     description='Welcome to Jarvis, your personal assistant! Jarvis is here to help you stay organized and manage your contacts, reminders, notes, and files efficiently.',
     author='Python Forces',
     url='https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654',
-    packages=['src','game'],
+    packages=['src'],
     
     entry_points={
         'console_scripts': [
             'Jarvis=src.main:main',
         ],
     },
     install_requires=[
```

### Comparing `jarvis_assistant_bot-1.0/src/commands.py` & `jarvis_assistant_bot-1.1/src/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from prompt_toolkit.completion import WordCompleter
 from colorama import Fore,Style
 from prettytable import PrettyTable
 from src.common_functions import STR_EPIC_COMMANDS
 from src.memory import Record,SetterValueIncorrect,AddressBook,Phone
 from src.notes_core import *
 from src.sorter import sort_files_in_this_path
-from game.game import *
+from src.goose_game import *
 import keyboard
 
 CHECK_SECOND_ARG_CHANGE_CONTACT = ("phone","email","birthday","address")
 CHECK_SECOND_ARG_CHANGE_NOTE = ("title","tag","description")
 
 def get_command_input_agree(Input_message=''):
     Input_value = None
```

### Comparing `jarvis_assistant_bot-1.0/src/common_functions.py` & `jarvis_assistant_bot-1.1/src/common_functions.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.0/src/main.py` & `jarvis_assistant_bot-1.1/src/main.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.0/src/memory.py` & `jarvis_assistant_bot-1.1/src/memory.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.0/src/notes_core.py` & `jarvis_assistant_bot-1.1/src/notes_core.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.0/src/open_ai_input_assistent.py` & `jarvis_assistant_bot-1.1/src/open_ai_input_assistent.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.0/src/save_load_books.py` & `jarvis_assistant_bot-1.1/src/save_load_books.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-1.0/src/sorter.py` & `jarvis_assistant_bot-1.1/src/sorter.py`

 * *Files identical despite different names*

