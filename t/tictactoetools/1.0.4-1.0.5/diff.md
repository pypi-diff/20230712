# Comparing `tmp/tictactoetools-1.0.4.tar.gz` & `tmp/tictactoetools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictactoetools-1.0.4.tar", last modified: Tue Jul 11 20:43:26 2023, max compression
+gzip compressed data, was "tictactoetools-1.0.5.tar", last modified: Tue Jul 11 22:52:23 2023, max compression
```

## Comparing `tictactoetools-1.0.4.tar` & `tictactoetools-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:43:26.690092 tictactoetools-1.0.4/
--rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-1.0.4/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)     1722 2023-07-11 20:43:26.688947 tictactoetools-1.0.4/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)     1341 2023-07-11 20:31:43.000000 tictactoetools-1.0.4/README.md
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 20:43:26.690331 tictactoetools-1.0.4/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      593 2023-07-11 20:43:24.000000 tictactoetools-1.0.4/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:43:26.676184 tictactoetools-1.0.4/tictactoetools/
--rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-1.0.4/tictactoetools/__init__.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:43:26.685492 tictactoetools-1.0.4/tictactoetools/data/
--rw-r--r--   0 simon      (502) staff       (20)    24576 2023-07-11 19:12:05.000000 tictactoetools-1.0.4/tictactoetools/data/tic_tac_toe.db
--rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-1.0.4/tictactoetools/tictac_exceptions.py
--rw-r--r--   0 simon      (502) staff       (20)     9303 2023-07-11 20:36:27.000000 tictactoetools-1.0.4/tictactoetools/tictactoetools.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 20:43:26.682509 tictactoetools-1.0.4/tictactoetools.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)     1722 2023-07-11 20:43:26.000000 tictactoetools-1.0.4/tictactoetools.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      309 2023-07-11 20:43:26.000000 tictactoetools-1.0.4/tictactoetools.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 20:43:26.000000 tictactoetools-1.0.4/tictactoetools.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-11 20:43:26.000000 tictactoetools-1.0.4/tictactoetools.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 22:52:23.198272 tictactoetools-1.0.5/
+-rw-r--r--   0 simon      (502) staff       (20)     1071 2023-07-11 18:52:55.000000 tictactoetools-1.0.5/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)     1722 2023-07-11 22:52:23.196992 tictactoetools-1.0.5/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)     1341 2023-07-11 20:31:43.000000 tictactoetools-1.0.5/README.md
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-07-11 22:52:23.199531 tictactoetools-1.0.5/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      593 2023-07-11 22:52:08.000000 tictactoetools-1.0.5/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 22:52:23.188483 tictactoetools-1.0.5/tictactoetools/
+-rw-r--r--   0 simon      (502) staff       (20)        0 2023-07-11 18:46:11.000000 tictactoetools-1.0.5/tictactoetools/__init__.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 22:52:23.194200 tictactoetools-1.0.5/tictactoetools/data/
+-rw-r--r--   0 simon      (502) staff       (20)    24576 2023-07-11 22:51:57.000000 tictactoetools-1.0.5/tictactoetools/data/tic_tac_toe.db
+-rw-r--r--   0 simon      (502) staff       (20)      117 2023-07-11 18:51:40.000000 tictactoetools-1.0.5/tictactoetools/tictac_exceptions.py
+-rw-r--r--   0 simon      (502) staff       (20)     9303 2023-07-11 20:36:27.000000 tictactoetools-1.0.5/tictactoetools/tictactoetools.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-07-11 22:52:23.192874 tictactoetools-1.0.5/tictactoetools.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)     1722 2023-07-11 22:52:23.000000 tictactoetools-1.0.5/tictactoetools.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      309 2023-07-11 22:52:23.000000 tictactoetools-1.0.5/tictactoetools.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-07-11 22:52:23.000000 tictactoetools-1.0.5/tictactoetools.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)       15 2023-07-11 22:52:23.000000 tictactoetools-1.0.5/tictactoetools.egg-info/top_level.txt
```

### Comparing `tictactoetools-1.0.4/LICENSE` & `tictactoetools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tictactoetools-1.0.4/PKG-INFO` & `tictactoetools-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 1.0.4
+Version: 1.0.5
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tictactoetools-1.0.4/README.md` & `tictactoetools-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tictactoetools-1.0.4/setup.py` & `tictactoetools-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name="tictactoetools",
-    version="1.0.4",
+    version="1.0.5",
     author="Simon Valentino",
     author_email="simontvalentino@gmail.com",
     url="https://github.com/SimonValentino/tictactoetools.git",
     description="Creatively build Tic-Tac-Toe matches and store their data in a database of all users.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
```

### Comparing `tictactoetools-1.0.4/tictactoetools/data/tic_tac_toe.db` & `tictactoetools-1.0.5/tictactoetools/data/tic_tac_toe.db`

 * *Files 18% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -6,25 +6,19 @@
 	"player2_id"	INTEGER NOT NULL,
 	"start_time"	TEXT NOT NULL,
 	"end_time"	TEXT NOT NULL,
 	"board"	TEXT NOT NULL,
 	"winner_id"	INTEGER DEFAULT Null,
 	PRIMARY KEY("match_id" AUTOINCREMENT)
 );
-INSERT INTO matches VALUES(1,1,2,'2023-07-11 14:58:59','2023-07-11 14:59:00','{"board": [["X"]], "size": 1, "num_consecutive_to_win": 1}',1);
-INSERT INTO matches VALUES(2,1,3,'2023-07-11 15:07:15','2023-07-11 15:07:16','{"board": [["X"]], "size": 1, "num_consecutive_to_win": 1}',1);
-INSERT INTO matches VALUES(3,1,2,'2023-07-11 15:12:02','2023-07-11 15:12:05','{"board": [["X", " "], ["X", "O"]], "size": 2, "num_consecutive_to_win": 2}',1);
 CREATE TABLE IF NOT EXISTS "players" (
 	"player_id"	INTEGER NOT NULL UNIQUE,
 	"username"	VARCHAR(15) NOT NULL,
 	PRIMARY KEY("player_id" AUTOINCREMENT)
 );
-INSERT INTO players VALUES(1,'SIMON');
-INSERT INTO players VALUES(2,'FRANCIS');
-INSERT INTO players VALUES(3,'REGINALD');
 DELETE FROM sqlite_sequence;
 INSERT INTO sqlite_sequence VALUES('players',3);
 INSERT INTO sqlite_sequence VALUES('matches',3);
 CREATE VIEW player_stats_view AS
 SELECT p.player_id, p.username, COUNT(*) AS num_games,
        SUM(CASE WHEN m.winner_id = p.player_id THEN 1 ELSE 0 END) AS num_wins
 FROM players p
```

### Comparing `tictactoetools-1.0.4/tictactoetools/tictactoetools.py` & `tictactoetools-1.0.5/tictactoetools/tictactoetools.py`

 * *Files identical despite different names*

### Comparing `tictactoetools-1.0.4/tictactoetools.egg-info/PKG-INFO` & `tictactoetools-1.0.5/tictactoetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictactoetools
-Version: 1.0.4
+Version: 1.0.5
 Summary: Creatively build Tic-Tac-Toe matches and store their data in a database of all users.
 Home-page: https://github.com/SimonValentino/tictactoetools.git
 Author: Simon Valentino
 Author-email: simontvalentino@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

