# Comparing `tmp/jarvis_assistant_bot-0.4.tar.gz` & `tmp/jarvis_assistant_bot-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis_assistant_bot-0.4.tar", last modified: Tue Jul 11 13:17:46 2023, max compression
+gzip compressed data, was "jarvis_assistant_bot-1.0.tar", last modified: Wed Jul 12 20:32:18 2023, max compression
```

## Comparing `jarvis_assistant_bot-0.4.tar` & `jarvis_assistant_bot-1.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 13:17:46.185434 jarvis_assistant_bot-0.4/
--rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-0.4/LICENSE
--rw-rw-rw-   0        0        0      311 2023-07-11 08:55:22.000000 jarvis_assistant_bot-0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4208 2023-07-11 13:17:46.185434 jarvis_assistant_bot-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3274 2023-07-11 13:12:08.000000 jarvis_assistant_bot-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 13:17:46.158870 jarvis_assistant_bot-0.4/jarvis_assistant_bot.egg-info/
--rw-rw-rw-   0        0        0     4208 2023-07-11 13:17:46.000000 jarvis_assistant_bot-0.4/jarvis_assistant_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-11 13:17:46.000000 jarvis_assistant_bot-0.4/jarvis_assistant_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 13:17:46.000000 jarvis_assistant_bot-0.4/jarvis_assistant_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-11 13:17:46.000000 jarvis_assistant_bot-0.4/jarvis_assistant_bot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-07-11 13:17:46.000000 jarvis_assistant_bot-0.4/jarvis_assistant_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-11 13:17:46.000000 jarvis_assistant_bot-0.4/jarvis_assistant_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2023-07-11 13:12:59.000000 jarvis_assistant_bot-0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 13:17:46.185434 jarvis_assistant_bot-0.4/setup.cfg
--rw-rw-rw-   0        0        0      541 2023-07-11 13:13:16.000000 jarvis_assistant_bot-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:17:46.183434 jarvis_assistant_bot-0.4/src/
--rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-0.4/src/__init__.py
--rw-rw-rw-   0        0        0    12611 2023-07-11 12:17:46.000000 jarvis_assistant_bot-0.4/src/commands.py
--rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-0.4/src/common_functions.py
--rw-rw-rw-   0        0        0     4148 2023-07-11 13:15:40.000000 jarvis_assistant_bot-0.4/src/main.py
--rw-rw-rw-   0        0        0    18396 2023-07-11 13:12:08.000000 jarvis_assistant_bot-0.4/src/memory.py
--rw-rw-rw-   0        0        0     5715 2023-07-11 12:16:24.000000 jarvis_assistant_bot-0.4/src/notes_core.py
--rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-0.4/src/save_load_books.py
--rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-0.4/src/sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:32:18.630553 jarvis_assistant_bot-1.0/
+-rw-rw-rw-   0        0        0     1091 2023-07-11 13:12:59.000000 jarvis_assistant_bot-1.0/LICENSE
+-rw-rw-rw-   0        0        0      689 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6070 2023-07-12 20:32:18.629554 jarvis_assistant_bot-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4909 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 20:32:18.558300 jarvis_assistant_bot-1.0/game/
+-rw-rw-rw-   0        0        0    10624 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.0/game/game.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:32:18.576553 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/
+-rw-rw-rw-   0        0        0     6070 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 20:32:18.000000 jarvis_assistant_bot-1.0/jarvis_assistant_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1081 2023-07-12 20:23:54.000000 jarvis_assistant_bot-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 20:32:18.630553 jarvis_assistant_bot-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      746 2023-07-12 20:31:31.000000 jarvis_assistant_bot-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:32:18.628558 jarvis_assistant_bot-1.0/src/
+-rw-rw-rw-   0        0        0        0 2023-07-09 17:18:59.000000 jarvis_assistant_bot-1.0/src/__init__.py
+-rw-rw-rw-   0        0        0    13208 2023-07-12 14:00:57.000000 jarvis_assistant_bot-1.0/src/commands.py
+-rw-rw-rw-   0        0        0     3147 2023-07-10 10:53:54.000000 jarvis_assistant_bot-1.0/src/common_functions.py
+-rw-rw-rw-   0        0        0     5590 2023-07-12 12:45:11.000000 jarvis_assistant_bot-1.0/src/main.py
+-rw-rw-rw-   0        0        0    18393 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.0/src/memory.py
+-rw-rw-rw-   0        0        0     5186 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.0/src/notes_core.py
+-rw-rw-rw-   0        0        0     2899 2023-07-12 10:27:50.000000 jarvis_assistant_bot-1.0/src/open_ai_input_assistent.py
+-rw-rw-rw-   0        0        0     2995 2023-07-11 13:12:08.000000 jarvis_assistant_bot-1.0/src/save_load_books.py
+-rw-rw-rw-   0        0        0     4339 2023-07-09 13:06:40.000000 jarvis_assistant_bot-1.0/src/sorter.py
```

### Comparing `jarvis_assistant_bot-0.4/LICENSE` & `jarvis_assistant_bot-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-0.4/jarvis_assistant_bot.egg-info/PKG-INFO` & `jarvis_assistant_bot-1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,13 @@
-Metadata-Version: 2.1
-Name: jarvis-assistant-bot
-Version: 0.4
-Summary: Welcome to Jarvis, your personal assistant! Jarvis is here to help you stay organized and manage your contacts, reminders, notes, and files efficiently. With Jarvis, you can easily handle your daily tasks and keep your information in one place.
-Home-page: https://github.com/UkrainianEagleOwl/tp_personal_assistant/tree/97c820e0779d54e488d5d824cce404b06bb4e654
-Author: Dmytro Filin, Illya Grygoriev, Dmytro Klymenko, Dmytro Paukov, Alexandr 
-Project-URL: Homepage, https://github.com/UkrainianEagleOwl/tp_personal_assistant
-Project-URL: Bug Tracker, https://github.com/UkrainianEagleOwl/tp_personal_assistant/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Sure! Here's the updated README with the additional information you provided:
 
 # Personal Assistant - Address Book (Jarvis)
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
-Welcome to Jarvis, your personal assistant! Jarvis is here to help you stay organized and manage your contacts, reminders, notes, and files efficiently. With Jarvis, you can easily handle your daily tasks and keep your information in one place.
+Welcome to Jarvis, your personal assistant! Jarvis is here to help you stay organized and manage your contacts, reminders, notes, and files efficiently. With Jarvis, you can easily handle your daily tasks and keep your information in one place.In addition, Jarvis integrates with ChatGPT, an AI language model, to provide interactive chat functionality. And to add some entertainment after a hard working day, Jarvis also includes a fun game about Bandera-goose.
 
 ## Table of Contents
 
 - [Features](#features)
 - [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
@@ -37,26 +21,26 @@
 
 - **Contact Book**: You can save and manage your contacts with names, addresses, phone numbers, email addresses, and birthdays. Jarvis securely stores this information, allowing you to easily access and update it whenever needed. It can also remind you of upcoming birthdays from your contact book.
 
 - **Notebook**: Jarvis provides a notebook feature where you can create and store text-based notes. These notes can contain important information, ideas, or anything you want to remember. You can search for specific notes using keywords or tags. Jarvis allows you to edit and delete notes, ensuring your information remains organized.
 
 - **File Sorting**: If you have files in a specified folder, Jarvis can help you sort them by categories such as images, documents, videos, and more. This feature ensures that your files are organized and easily accessible.
 
+- **NEW UPDATE**: *Interactive chat functionality with ChatGPT.*
+
+- **NEW UPDATE**: *Enjoy a fun game about Bandera-goose after a hard working day!*
+
 ## Getting Started
 
 To get started with Jarvis, follow these steps:
 
 ### Prerequisites
 
 - Python 3.x
-- Git
-- colorama 
-- prompt_toolkit
-- prettytable
-  
+- Git  
 
 ### Installation by clone from github
 
 1. Clone the repository.
    ```sh
    git clone https://github.com/UkrainianEagleOwl/tp_personal_assistant.git
    ```
@@ -80,22 +64,41 @@
 ## Usage
 
 1. Run the application.
    ```sh
    jarvis
    ```
 
-2. Follow the on-screen instructions to access and use Jarvis's various features, such as managing contacts, creating notes, and sorting files.
+2. Follow the on-screen instructions to access and use Jarvis's various features, such as managing contacts, creating notes, and sorting files. You can also interact with ChatGPT by typing messages. ChatGPT will respond to your inputs.
+
+## API Key
+
+In order to use the interactive chat functionality powered by ChatGPT, you will need an API key from OpenAI. Here's how you can obtain your API key:
+
+1. Visit the OpenAI website at [https://www.openai.com](https://www.openai.com).
+2. Create an account or log in to your existing account.
+3. Navigate to the API section and generate an API key for the GPT-3.5 model.
+4. Copy the API key to a secure location.
+
+When you run Jarvis for the first time, you will be prompted to enter your API key. Once entered, the key will be encrypted and saved on your computer for future usage. The encrypted key is used by the application to access the API and is only sent to OpenAI for processing your requests.
+
+## Privacy
+
+Jarvis takes privacy and data security seriously. The API key you provide is encrypted and stored locally on your computer. It is used solely for the purpose of accessing the OpenAI API to facilitate the interactive chat functionality. The key is not shared with any third parties or sent over the network. Your data and conversations are kept confidential.
+
+## Game
+
+Jarvis includes a fun game about Bandera-goose, designed to provide some entertainment after a hard working day. Interact with the game during your leisure time and enjoy the experience.
 
 ## Contacts
 
 Please feel free to reach out to any of the following team members if you have any questions, suggestions, or would like to contribute to this project:
 
 - Dmytro Filin - GitHub: [dmytrofilin](https://github.com/UkrainianEagleOwl) LinkedIn: [Dmytro Filin](https://www.linkedin.com/in/dmytro-filin-18716b198/) 
-- Illya Grygoriev - GitHub: [illyagrygoriev](https://github.com/Adentas)
+- Illya Hryhoriev - GitHub: [illyagrygoriev](https://github.com/Adentas)
 - Dmytro Klymenko - GitHub: [dmytroklymenko](https://github.com/leegosx)
 - Dmytro Paukov - GitHub: [dmytropaukov](https://github.com/paukdv)
 - Alexandr - GitHub: [alexandr](https://github.com/sanyashahter)
 
 Please ensure that you follow our [Code of Conduct](CODE_OF_CONDUCT.md) when interacting with team members.
 
 ## License
```

### Comparing `jarvis_assistant_bot-0.4/src/commands.py` & `jarvis_assistant_bot-1.0/src/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,29 @@
 from prompt_toolkit.completion import WordCompleter
 from colorama import Fore,Style
 from prettytable import PrettyTable
 from src.common_functions import STR_EPIC_COMMANDS
 from src.memory import Record,SetterValueIncorrect,AddressBook,Phone
 from src.notes_core import *
 from src.sorter import sort_files_in_this_path
+from game.game import *
+import keyboard
 
 CHECK_SECOND_ARG_CHANGE_CONTACT = ("phone","email","birthday","address")
 CHECK_SECOND_ARG_CHANGE_NOTE = ("title","tag","description")
 
+def get_command_input_agree(Input_message=''):
+    Input_value = None
+    while True:
+        Input_value = prompt(Input_message)
+        if (Input_value.lower() == 'yes') or (Input_value.lower() == 'no'):
+            return Input_value
+        else:
+            print("You can write only 'yes' or 'no'!")
+
 def get_command_input(Input_message='',check_class = None,need_comp = True, check_add_command = None, arg_number = None):
     Input_value = None
     while True:
         if need_comp:
             Input_value = prompt(Input_message, completer=completer)
         else:
             Input_value = prompt(Input_message)
@@ -207,34 +218,43 @@
     n_book.sort_notes_by_tag()
     return "Notes sorted by tags."
 
 def show_all_notes(*arg, a_book=AddressBook,n_book=Notebook):
     table = n_book.show_notes()
     return table
 
+def start_game(*arg,a_book = AddressBook,n_book = Notebook):
+    play()
+
 def ending(*arg,a_book = AddressBook,n_book = Notebook):
     return 'Goodbye!'
 
 input_variants = ['hello','hi','start','add contact','new contact','create contact','change contact','change phone','change contact details',"sort","sort files","need sort",
-                  'get contact','show contact','show person','show contacts','show address book','show all book','goodbye','close','end','search user','find contact','find user', "help","commands",
+                  'get contact', 'show contact','show person','show contacts','show address book','show all book','goodbye','close','end','search user','find contact','find user', "help","commands",
                   "need help",'remove note','delete note','get note out','add note', 'new note','create note','find notes', 'search notes','remove contact','delete contact','take out contact'
                   ,"edit note", "change note", "search by tag","sort by tag",'show all notes','show notebook','show notes','give me note',"find by tag","give me note by tag"
-                  ,"tag sorting","notebook sort by tag","remake note"]
+                  ,"tag sorting","notebook sort by tag","remake note", 'game', 'play', 'fun']
 # Ініціалізація автодоповнювача зі списком команд
 completer = WordCompleter(input_variants)
 
 # Define available commands
 commands = [
     {
         "name": "greet",
         "input view":["hello",'hi','start'],
         "arguments": [],
         "func":greetings
     },
     {
+        "name": "game",
+        "input view": ['game','play','fun'],
+        "arguments": [],
+        "func":start_game
+    },
+    {
         "name": "add new contact",
         "input view": ['add contact','new contact','create contact'],
         "arguments": ["name", "phone","birthday","email","address"],
         "func":add_new_contact
     },
     {
         "name": "change exist contact",
```

### Comparing `jarvis_assistant_bot-0.4/src/common_functions.py` & `jarvis_assistant_bot-1.0/src/common_functions.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-0.4/src/memory.py` & `jarvis_assistant_bot-1.0/src/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     if user_birthday.weekday() > 4:
                         greeting_day = days_week[0]
                     else:
                         greeting_day = days_week[user_birthday.weekday()]
                     user_info = {
                         'user_name': user_data.user_name.value,
                         'user_phones': ', '.join([str(x) for x in user_data.user_phones]),
-                        'user_birthday': user_data.user_birthday.value.strftime("%d.%m.%Y"),
+                        'user_birthday': user_data.user_birthday.value.strftime("%d %B"),
                         'day': '🎂' + ' ' + greeting_day
                     }
                     birthday_users.append(user_info)
 
         # Вивід списку користувачів за допомогою prettytable
         table = PrettyTable()
         table.field_names = ['Greeting Day', 'Name', 'Phone', 'Date of Birth']
```

### Comparing `jarvis_assistant_bot-0.4/src/notes_core.py` & `jarvis_assistant_bot-1.0/src/notes_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
-from prettytable import PrettyTable
-from colorama import init, Fore, Style
+from colorama import Fore, Style
 from src.memory import SetterValueIncorrect
 
 
 class Tag:
     def __init__(self, name):
         self._name = name
 
@@ -33,30 +32,18 @@
         self.description = description
 
     def __repr__(self):
         tags_str = ""
         if self.tags:
             tags_str = ", ".join(tag.name for tag in self.tags)
         return "Title: {}\nTags: {}\nDescription: {}".format(self.title, tags_str, self.description)
-
-    def to_dict(self):
-        notes_data = []
-        for note in self.notes:
-            # Сохраняем только имена тегов
-            tags_data = [tag.name for tag in note.tags]
-            notes_data.append({
-                'title': note.title,
-                'tags': tags_data,  # Используем сохраненные имена тегов
-                'description': note.description
-            })
-        return {'notes': notes_data}
     
     def change_note_info(self,change_field, new_info):
         if change_field == 'tag':
-            self.tags == new_info if isinstance(new_info, Tag) else Tag(new_info)
+            self.tags[-1] = new_info if isinstance(new_info, Tag) else Tag(new_info)
         elif change_field == 'title':
             self.title = new_info
         elif change_field == "description":
             self.description = new_info
 
     def add_tag(self,tag):
         self.tags.append(Tag(tag) if isinstance(tag, str) else tag)
```

### Comparing `jarvis_assistant_bot-0.4/src/save_load_books.py` & `jarvis_assistant_bot-1.0/src/save_load_books.py`

 * *Files identical despite different names*

### Comparing `jarvis_assistant_bot-0.4/src/sorter.py` & `jarvis_assistant_bot-1.0/src/sorter.py`

 * *Files identical despite different names*

