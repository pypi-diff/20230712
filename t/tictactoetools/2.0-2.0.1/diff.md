# Comparing `tmp/tictactoetools-2.0.tar.gz` & `tmp/tictactoetools-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictactoetools-2.0.tar", last modified: Wed Jul 12 02:26:53 2023, max compression
+gzip compressed data, was "tictactoetools-2.0.1.tar", last modified: Wed Jul 12 17:54:37 2023, max compression
```

## Comparing `tictactoetools-2.0.tar` & `tictactoetools-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 02:26:53.624319 tictactoetools-2.0/
--rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-2.0/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)     1707 2023-07-12 02:26:53.622921 tictactoetools-2.0/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)     1364 2023-07-12 02:26:12.000000 tictactoetools-2.0/README.md
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-12 02:26:53.624808 tictactoetools-2.0/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      516 2023-07-12 02:26:12.000000 tictactoetools-2.0/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 02:26:53.605567 tictactoetools-2.0/tests/
--rw-r--r--   0 simon      (502) staff       (20)       56 2023-07-12 01:50:26.000000 tictactoetools-2.0/tests/test.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 02:26:53.611907 tictactoetools-2.0/tictactoetools/
--rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-2.0/tictactoetools/__init__.py
--rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-2.0/tictactoetools/tictac_exceptions.py
--rw-r--r--   0 simon      (502) staff       (20)    10486 2023-07-12 02:26:12.000000 tictactoetools-2.0/tictactoetools/tictactoetools.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 02:26:53.620998 tictactoetools-2.0/tictactoetools.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)     1707 2023-07-12 02:26:53.000000 tictactoetools-2.0/tictactoetools.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      288 2023-07-12 02:26:53.000000 tictactoetools-2.0/tictactoetools.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-12 02:26:53.000000 tictactoetools-2.0/tictactoetools.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-12 02:26:53.000000 tictactoetools-2.0/tictactoetools.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 17:54:37.218325 tictactoetools-2.0.1/
+-rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-2.0.1/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)     2726 2023-07-12 17:54:37.215617 tictactoetools-2.0.1/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)     2381 2023-07-12 17:43:35.000000 tictactoetools-2.0.1/README.md
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-12 17:54:37.218630 tictactoetools-2.0.1/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      518 2023-07-12 17:54:20.000000 tictactoetools-2.0.1/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 17:54:37.202525 tictactoetools-2.0.1/tests/
+-rw-r--r--   0 simon      (502) staff       (20)      110 2023-07-12 17:25:13.000000 tictactoetools-2.0.1/tests/test.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 17:54:37.207860 tictactoetools-2.0.1/tictactoetools/
+-rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-2.0.1/tictactoetools/__init__.py
+-rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-2.0.1/tictactoetools/tictac_exceptions.py
+-rw-r--r--   0 simon      (502) staff       (20)    13453 2023-07-12 17:28:05.000000 tictactoetools-2.0.1/tictactoetools/tictactoetools.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 17:54:37.213924 tictactoetools-2.0.1/tictactoetools.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)     2726 2023-07-12 17:54:37.000000 tictactoetools-2.0.1/tictactoetools.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      288 2023-07-12 17:54:37.000000 tictactoetools-2.0.1/tictactoetools.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-12 17:54:37.000000 tictactoetools-2.0.1/tictactoetools.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-12 17:54:37.000000 tictactoetools-2.0.1/tictactoetools.egg-info/top_level.txt
```

### Comparing `tictactoetools-2.0/LICENSE` & `tictactoetools-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tictactoetools-2.0/PKG-INFO` & `tictactoetools-2.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 2.0
+Version: 2.0.1
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,30 +19,53 @@
 
 ```
 pip install tictactoetools
 ```
 
 # Usage
 
-### Builtin functions
+## Builtin Functions
 
-The tictactoetools module within the package comes with a builtin play() method as an example for playing tic-tac-toe using
-the given features.
+The package includes several built-in functions that facilitate the gameplay and interaction with the Tic-Tac-Toe game.
+These functions provide functionality for playing matches, creating new matches, prompting user input, managing player moves,
+and handling rematch options. There are also builtin functions for working with the database (see "Database")
 
-The tictactoetools module also has functions for creating new users in the tictactoe.db database, logging matches in the
-database, starting new matches, and even prompting values from the user for playing Tic-Tac-Toe.
+The builtin play() function is an example of how all the functions can work together to make a Tic-Tac-Toe game, as well
+as logging data on the database.
 
-### Board Class
+## Database
 
-The Board class represents the Tic-Tac-Toe game board. It provides methods for displaying the board, marking cells with
-any symbol, checking for a winner, and more.
+The tictactoetools package includes several built-in functions that facilitate working with the database, such as logging
+matches, retrieving player IDs, checking username existence, creating new users, and fetching player and match statistics.
 
-### Match Class
+The database for this package consists of the following tables:
 
-The Match class is a data class responsible for storing information about the players, start and end times of a match,
+### Table: players
+
+- `player_id`: Unique identifier for each player.
+- `username`: The username of the player.
+
+### Table: matches
+
+- `match_id`: Unique identifier for each match.
+- `player1_id`: The ID of the first player in the match.
+- `player2_id`: The ID of the second player in the match.
+- `start_time`: The start time of the match.
+- `end_time`: The end time of the match.
+- `board`: The game board data for the match.
+- `winner_id`: The ID of the player who won the match.
+
+## Board Class
+
+The `Board` class represents the internal Tic Tac Toe game board. It provides functionality to manage and display the board
+state, check for a winner, mark cells with player symbols, and perform other board-related operations.
+
+## Match Class
+
+The `Match` class is a data class responsible for storing information about the players, start and end times of a match,
 the board configuration, and the winner.
 
 # Contributing
 
 Contributions to the tictactoetools package are welcome! If you encounter any issues or have suggestions for improvements,
 please create an issue on the GitHub repository.
```

### Comparing `tictactoetools-2.0/setup.py` & `tictactoetools-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name="tictactoetools",
-    version="2.0",
+    version="2.0.1",
     author="Simon Valentino",
     author_email="simontvalentino@gmail.com",
     url="https://github.com/SimonValentino/tictactoetools.git",
     description="Creatively build Tic-Tac-Toe matches and store their data in a database of all users.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
```

### Comparing `tictactoetools-2.0/tictactoetools.egg-info/PKG-INFO` & `tictactoetools-2.0.1/tictactoetools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 2.0
+Version: 2.0.1
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,30 +19,53 @@
 
 ```
 pip install tictactoetools
 ```
 
 # Usage
 
-### Builtin functions
+## Builtin Functions
 
-The tictactoetools module within the package comes with a builtin play() method as an example for playing tic-tac-toe using
-the given features.
+The package includes several built-in functions that facilitate the gameplay and interaction with the Tic-Tac-Toe game.
+These functions provide functionality for playing matches, creating new matches, prompting user input, managing player moves,
+and handling rematch options. There are also builtin functions for working with the database (see "Database")
 
-The tictactoetools module also has functions for creating new users in the tictactoe.db database, logging matches in the
-database, starting new matches, and even prompting values from the user for playing Tic-Tac-Toe.
+The builtin play() function is an example of how all the functions can work together to make a Tic-Tac-Toe game, as well
+as logging data on the database.
 
-### Board Class
+## Database
 
-The Board class represents the Tic-Tac-Toe game board. It provides methods for displaying the board, marking cells with
-any symbol, checking for a winner, and more.
+The tictactoetools package includes several built-in functions that facilitate working with the database, such as logging
+matches, retrieving player IDs, checking username existence, creating new users, and fetching player and match statistics.
 
-### Match Class
+The database for this package consists of the following tables:
 
-The Match class is a data class responsible for storing information about the players, start and end times of a match,
+### Table: players
+
+- `player_id`: Unique identifier for each player.
+- `username`: The username of the player.
+
+### Table: matches
+
+- `match_id`: Unique identifier for each match.
+- `player1_id`: The ID of the first player in the match.
+- `player2_id`: The ID of the second player in the match.
+- `start_time`: The start time of the match.
+- `end_time`: The end time of the match.
+- `board`: The game board data for the match.
+- `winner_id`: The ID of the player who won the match.
+
+## Board Class
+
+The `Board` class represents the internal Tic Tac Toe game board. It provides functionality to manage and display the board
+state, check for a winner, mark cells with player symbols, and perform other board-related operations.
+
+## Match Class
+
+The `Match` class is a data class responsible for storing information about the players, start and end times of a match,
 the board configuration, and the winner.
 
 # Contributing
 
 Contributions to the tictactoetools package are welcome! If you encounter any issues or have suggestions for improvements,
 please create an issue on the GitHub repository.
```

