# Comparing `tmp/tictactoetools-1.0.5.tar.gz` & `tmp/tictactoetools-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictactoetools-1.0.5.tar", last modified: Tue Jul 11 22:52:23 2023, max compression
+gzip compressed data, was "tictactoetools-2.0.tar", last modified: Wed Jul 12 02:26:53 2023, max compression
```

## Comparing `tictactoetools-1.0.5.tar` & `tictactoetools-2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 22:52:23.198272 tictactoetools-1.0.5/
--rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-1.0.5/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)     1722 2023-07-11 22:52:23.196992 tictactoetools-1.0.5/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)     1341 2023-07-11 20:31:43.000000 tictactoetools-1.0.5/README.md
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 22:52:23.199531 tictactoetools-1.0.5/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      593 2023-07-11 22:52:08.000000 tictactoetools-1.0.5/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 22:52:23.188483 tictactoetools-1.0.5/tictactoetools/
--rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-1.0.5/tictactoetools/__init__.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 22:52:23.194200 tictactoetools-1.0.5/tictactoetools/data/
--rw-r--r--   0 simon      (502) staff       (20)    24576 2023-07-11 22:51:57.000000 tictactoetools-1.0.5/tictactoetools/data/tic_tac_toe.db
--rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-1.0.5/tictactoetools/tictac_exceptions.py
--rw-r--r--   0 simon      (502) staff       (20)     9303 2023-07-11 20:36:27.000000 tictactoetools-1.0.5/tictactoetools/tictactoetools.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 22:52:23.192874 tictactoetools-1.0.5/tictactoetools.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)     1722 2023-07-11 22:52:23.000000 tictactoetools-1.0.5/tictactoetools.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      309 2023-07-11 22:52:23.000000 tictactoetools-1.0.5/tictactoetools.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 22:52:23.000000 tictactoetools-1.0.5/tictactoetools.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-11 22:52:23.000000 tictactoetools-1.0.5/tictactoetools.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 02:26:53.624319 tictactoetools-2.0/
+-rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-2.0/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)     1707 2023-07-12 02:26:53.622921 tictactoetools-2.0/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)     1364 2023-07-12 02:26:12.000000 tictactoetools-2.0/README.md
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-12 02:26:53.624808 tictactoetools-2.0/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      516 2023-07-12 02:26:12.000000 tictactoetools-2.0/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 02:26:53.605567 tictactoetools-2.0/tests/
+-rw-r--r--   0 simon      (502) staff       (20)       56 2023-07-12 01:50:26.000000 tictactoetools-2.0/tests/test.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 02:26:53.611907 tictactoetools-2.0/tictactoetools/
+-rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-2.0/tictactoetools/__init__.py
+-rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-2.0/tictactoetools/tictac_exceptions.py
+-rw-r--r--   0 simon      (502) staff       (20)    10486 2023-07-12 02:26:12.000000 tictactoetools-2.0/tictactoetools/tictactoetools.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-12 02:26:53.620998 tictactoetools-2.0/tictactoetools.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)     1707 2023-07-12 02:26:53.000000 tictactoetools-2.0/tictactoetools.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      288 2023-07-12 02:26:53.000000 tictactoetools-2.0/tictactoetools.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-12 02:26:53.000000 tictactoetools-2.0/tictactoetools.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-12 02:26:53.000000 tictactoetools-2.0/tictactoetools.egg-info/top_level.txt
```

### Comparing `tictactoetools-1.0.5/LICENSE` & `tictactoetools-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tictactoetools-1.0.5/PKG-INFO` & `tictactoetools-2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 1.0.5
+Version: 2.0
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tictactoetools
 
 tictactoetools is a Python package that provides functionality for building games of Tic-Tac-Toe with customizable features
 and storing the data of matches in a database.
@@ -21,14 +19,16 @@
 
 ```
 pip install tictactoetools
 ```
 
 # Usage
 
+### Builtin functions
+
 The tictactoetools module within the package comes with a builtin play() method as an example for playing tic-tac-toe using
 the given features.
 
 The tictactoetools module also has functions for creating new users in the tictactoe.db database, logging matches in the
 database, starting new matches, and even prompting values from the user for playing Tic-Tac-Toe.
 
 ### Board Class
@@ -45,8 +45,7 @@
 
 Contributions to the tictactoetools package are welcome! If you encounter any issues or have suggestions for improvements,
 please create an issue on the GitHub repository.
 
 # License
 
 This package is licensed under the MIT License. See the LICENSE file for more information.
-
```

### Comparing `tictactoetools-1.0.5/README.md` & `tictactoetools-2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 ```
 pip install tictactoetools
 ```
 
 # Usage
 
+### Builtin functions
+
 The tictactoetools module within the package comes with a builtin play() method as an example for playing tic-tac-toe using
 the given features.
 
 The tictactoetools module also has functions for creating new users in the tictactoe.db database, logging matches in the
 database, starting new matches, and even prompting values from the user for playing Tic-Tac-Toe.
 
 ### Board Class
```

### Comparing `tictactoetools-1.0.5/setup.py` & `tictactoetools-2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name="tictactoetools",
-    version="1.0.5",
+    version="2.0",
     author="Simon Valentino",
     author_email="simontvalentino@gmail.com",
     url="https://github.com/SimonValentino/tictactoetools.git",
     description="Creatively build Tic-Tac-Toe matches and store their data in a database of all users.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
-    package_data={
-        "tictactoetools": ["data/tic_tac_toe.db"]
-    }
 )
```

### Comparing `tictactoetools-1.0.5/tictactoetools/tictactoetools.py` & `tictactoetools-2.0/tictactoetools/tictactoetools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import json
 import sqlite3
 from datetime import datetime
 from .tictac_exceptions import FullBoardError
 from dataclasses import dataclass
 import os
-
-__package_dir = os.path.dirname(__file__)
-__db_path = os.path.join(__package_dir, "data", "tic_tac_toe.db")
+import mysql.connector
 
 
 class Board:
     __BLANK_SPACE = " "
 
     def __init__(self, size: int = 3, num_consecutive_to_win: int = None) -> None:
         if size <= 0 or num_consecutive_to_win and num_consecutive_to_win <= 0:
@@ -229,64 +227,103 @@
     p1_id = get_player_id(match.p1)
     p2_id = get_player_id(match.p2)
     formatted_start_datetime = match.start_time.strftime("%Y-%m-%d %H:%M:%S")
     formatted_end_datetime = match.end_time.strftime("%Y-%m-%d %H:%M:%S")
     board_data = match.board._as_json()
     winner_id = get_player_id(match.winner) if match.winner else None
 
-    with sqlite3.connect(__db_path) as conn:
-        conn.execute("""
-        INSERT INTO matches (
-            player1_id,
-            player2_id,
-            start_time,
-            end_time,
-            board,
-            winner_id
-        )
-        VALUES (
-            ?,
-            ?,
-            ?,
-            ?,
-            ?,
-            ?
-        )
-        """, (p1_id, p2_id, formatted_start_datetime, formatted_end_datetime, json.dumps(board_data), winner_id))
+    with mysql.connector.connect(
+        host='sql9.freesqldatabase.com',
+        user='sql9632131',
+        password='iWCMKp7Q8R',
+        database='sql9632131'
+    ) as conn:
+        cursor = conn.cursor()
+        try:
+            cursor.execute("""
+            INSERT INTO matches (
+                player1_id,
+                player2_id,
+                start_time,
+                end_time,
+                board,
+                winner_id
+            )
+            VALUES (
+                %s,
+                %s,
+                %s,
+                %s,
+                %s,
+                %s
+            )
+            """, (p1_id, p2_id, formatted_start_datetime, formatted_end_datetime, json.dumps(board_data), winner_id))
+            conn.commit()
+        finally:
+            cursor.close()
 
 
 def get_player_id(username: str) -> int:
     if not username_exists(username):
         create_new_user(username)
 
-    with sqlite3.connect(__db_path) as conn:
+    with mysql.connector.connect(
+        host='sql9.freesqldatabase.com',
+        user='sql9632131',
+        password='iWCMKp7Q8R',
+        database='sql9632131'
+    ) as conn:
         cursor = conn.cursor()
-        cursor.execute("""
-            SELECT player_id
-            FROM players
-            WHERE username = ?
-            """, (username,))
-        row = cursor.fetchone()
-        return row[0]
+        try:
+            cursor.execute("""
+                SELECT player_id
+                FROM players
+                WHERE username = %s
+                """, (username,))
+            row = cursor.fetchone()
+            # Consume and discard any remaining unread results
+            cursor.fetchall()
+            return row[0]
+        finally:
+            cursor.close()
 
 
 def username_exists(username: str) -> bool:
-    with sqlite3.connect(__db_path) as conn:
+    with mysql.connector.connect(
+            host='sql9.freesqldatabase.com',
+            user='sql9632131',
+            password='iWCMKp7Q8R',
+            database='sql9632131'
+    ) as conn:
         cursor = conn.cursor()
-        cursor.execute("""
-        SELECT COUNT(username)
-        FROM players
-        WHERE username = ?
-        """, (username,))
-        row = cursor.fetchone()
-        return row[0] > 0
+        try:
+            cursor.execute("""
+            SELECT EXISTS(
+                SELECT 1 FROM players WHERE username = %s
+            ) AS username_exists
+            """, (username,))
+            exists = bool(cursor.fetchone()[0])
+            # Consume and discard any remaining unread results
+            cursor.fetchall()
+            return exists
+        finally:
+            cursor.close()
 
 
 def create_new_user(username: str) -> None:
-    with sqlite3.connect(__db_path) as conn:
-        conn.execute("""
-        INSERT INTO players (username)
-        VALUES (
-            ?
-        )
-        """, (username,))
-        conn.commit()
+    with mysql.connector.connect(
+            host='sql9.freesqldatabase.com',
+            user='sql9632131',
+            password='iWCMKp7Q8R',
+            database='sql9632131'
+    ) as conn:
+        cursor = conn.cursor()
+        try:
+            cursor.execute("""
+            INSERT INTO players (username)
+            VALUES (
+                %s
+            )
+            """, (username,))
+            conn.commit()
+        finally:
+            cursor.close()
```

### Comparing `tictactoetools-1.0.5/tictactoetools.egg-info/PKG-INFO` & `tictactoetools-2.0/tictactoetools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 1.0.5
+Version: 2.0
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tictactoetools
 
 tictactoetools is a Python package that provides functionality for building games of Tic-Tac-Toe with customizable features
 and storing the data of matches in a database.
@@ -21,14 +19,16 @@
 
 ```
 pip install tictactoetools
 ```
 
 # Usage
 
+### Builtin functions
+
 The tictactoetools module within the package comes with a builtin play() method as an example for playing tic-tac-toe using
 the given features.
 
 The tictactoetools module also has functions for creating new users in the tictactoe.db database, logging matches in the
 database, starting new matches, and even prompting values from the user for playing Tic-Tac-Toe.
 
 ### Board Class
@@ -45,8 +45,7 @@
 
 Contributions to the tictactoetools package are welcome! If you encounter any issues or have suggestions for improvements,
 please create an issue on the GitHub repository.
 
 # License
 
 This package is licensed under the MIT License. See the LICENSE file for more information.
-
```

