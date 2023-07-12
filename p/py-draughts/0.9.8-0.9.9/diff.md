# Comparing `tmp/py-draughts-0.9.8.tar.gz` & `tmp/py-draughts-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-0.9.8.tar", last modified: Tue Jul 11 20:04:44 2023, max compression
+gzip compressed data, was "py-draughts-0.9.9.tar", last modified: Wed Jul 12 10:11:51 2023, max compression
```

## Comparing `py-draughts-0.9.8.tar` & `py-draughts-0.9.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.241716 py-draughts-0.9.8/
--rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-0.9.8/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5460 2023-07-11 20:04:44.240737 py-draughts-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     4059 2023-07-11 19:54:28.000000 py-draughts-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.206715 py-draughts-0.9.8/draughts/
--rw-rw-rw-   0        0        0      945 2023-07-11 19:54:55.000000 py-draughts-0.9.8/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/american.py
--rw-rw-rw-   0        0        0     9140 2023-07-11 19:58:36.000000 py-draughts-0.9.8/draughts/base.py
--rw-rw-rw-   0        0        0      674 2023-07-11 19:49:33.000000 py-draughts-0.9.8/draughts/models.py
--rw-rw-rw-   0        0        0     4191 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/move.py
--rw-rw-rw-   0        0        0     5098 2023-07-11 19:36:47.000000 py-draughts-0.9.8/draughts/server.py
--rw-rw-rw-   0        0        0     5873 2023-07-11 19:34:13.000000 py-draughts-0.9.8/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.139998 py-draughts-0.9.8/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.208716 py-draughts-0.9.8/draughts/static/css/
--rw-rw-rw-   0        0        0     2782 2023-07-11 19:06:37.000000 py-draughts-0.9.8/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.212720 py-draughts-0.9.8/draughts/static/js/
--rw-rw-rw-   0        0        0     5824 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.219716 py-draughts-0.9.8/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2500 2023-07-11 19:06:02.000000 py-draughts-0.9.8/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.233714 py-draughts-0.9.8/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     5460 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-0.9.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 20:04:44.241716 py-draughts-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.238715 py-draughts-0.9.8/test/
--rw-rw-rw-   0        0        0     1123 2023-07-11 18:56:31.000000 py-draughts-0.9.8/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-11 18:56:31.000000 py-draughts-0.9.8/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.412134 py-draughts-0.9.9/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-11 18:05:22.000000 py-draughts-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6079 2023-07-12 10:11:51.411135 py-draughts-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4678 2023-07-12 10:10:58.000000 py-draughts-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.375137 py-draughts-0.9.9/draughts/
+-rw-rw-rw-   0        0        0      945 2023-07-12 10:11:28.000000 py-draughts-0.9.9/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-11 16:12:53.000000 py-draughts-0.9.9/draughts/american.py
+-rw-rw-rw-   0        0        0    10939 2023-07-12 10:06:21.000000 py-draughts-0.9.9/draughts/base.py
+-rw-rw-rw-   0        0        0      674 2023-07-12 09:24:29.000000 py-draughts-0.9.9/draughts/models.py
+-rw-rw-rw-   0        0        0     4191 2023-07-11 17:16:02.000000 py-draughts-0.9.9/draughts/move.py
+-rw-rw-rw-   0        0        0     5221 2023-07-12 10:03:55.000000 py-draughts-0.9.9/draughts/server.py
+-rw-rw-rw-   0        0        0     5989 2023-07-12 09:53:36.000000 py-draughts-0.9.9/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.334145 py-draughts-0.9.9/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.377135 py-draughts-0.9.9/draughts/static/css/
+-rw-rw-rw-   0        0        0     2782 2023-07-12 09:24:29.000000 py-draughts-0.9.9/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.378138 py-draughts-0.9.9/draughts/static/js/
+-rw-rw-rw-   0        0        0     5824 2023-07-11 15:13:38.000000 py-draughts-0.9.9/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.381136 py-draughts-0.9.9/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-0.9.9/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2500 2023-07-11 13:56:11.000000 py-draughts-0.9.9/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-11 13:47:51.000000 py-draughts-0.9.9/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.397138 py-draughts-0.9.9/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     6079 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 10:11:51.000000 py-draughts-0.9.9/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 17:26:06.000000 py-draughts-0.9.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 10:11:51.412134 py-draughts-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-07-11 17:45:47.000000 py-draughts-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:11:51.410136 py-draughts-0.9.9/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-11 16:12:53.000000 py-draughts-0.9.9/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-11 16:12:53.000000 py-draughts-0.9.9/test/test_board.py
```

### Comparing `py-draughts-0.9.8/LICENSE` & `py-draughts-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/PKG-INFO` & `py-draughts-0.9.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 0.9.8
+Version: 0.9.9
 Summary: A draughts library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -32,23 +32,30 @@
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
-
-
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
 
-## [Documentation](https://michalskibinski109.github.io/py-draughts/)
+## Key features
+1. Provides beautiful web interface for testing your engine/playing against AI.
+2. Supports multiple variants of the game (with different board size). `standard`, `american` etc.
+3. Follows international draughts standards. like `fen` `pdn` etc.
+4. Allows to easily create new variants of the game. by extending the `Board` class.
+5. Accurate documentation generated from code.
+
+
+
+### [Documentation](https://michalskibinski109.github.io/py-draughts/)
 
 ## Usage
 
 
 
 #### Displays simple ascii board
 
@@ -88,32 +95,36 @@
  . . . . . . . . . .
  . . . . . . . . . .
  w . . . w . w . w .
  . w . w . w . w . w
  w . w . w . w . w .
 ```
 
-### Generate legal moves and validate moves
+#### Generate legal moves and validate moves
 
 ```python
 >>> board.push_from_str("10x42")
 Move: 10->42 is correct, but not legal in given position.
  Legal moves are: [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
 
 >>> list(board.legal_moves)
 [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
 ```
 
-### Generate fen string
+#### Generate fen string and load board from fen string
+
 
 ```python
+>>> board =Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
+Board initialized with shape (10, 10). (base.py:109)
+>>> board.push_from_str("28-37")
 >>> board.fen
-[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]
+'[FEN "B:W4,11,31,K33,K34,37,38,40,K41,43,K44,45,K46,47:BK3,21,27"]'
 ```
-### American checkers
+#### American checkers
 
 ```python
 >>> from draughts.american import Board
 >>> board = Board()
 Board initialized with shape (8, 8). (base.py:108)
 >>> board
  . b . b . b . b
@@ -130,15 +141,15 @@
 ## UI
 
 ```python
 from draughts.server import Server
 Server().run()
 ```
 
-### Use for testing your engine.
+#### Use for testing your engine.
 
 _Example with simplest possible engine._
 
 ```python
 >>> server = Server(get_best_move_method=lambda board: np.random.choice(list(board.legal_moves)))
 >>> server.run()
 INFO:     Started server process [1617]
```

### Comparing `py-draughts-0.9.8/README.md` & `py-draughts-0.9.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,30 @@
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
-
-
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
 
-## [Documentation](https://michalskibinski109.github.io/py-draughts/)
+## Key features
+1. Provides beautiful web interface for testing your engine/playing against AI.
+2. Supports multiple variants of the game (with different board size). `standard`, `american` etc.
+3. Follows international draughts standards. like `fen` `pdn` etc.
+4. Allows to easily create new variants of the game. by extending the `Board` class.
+5. Accurate documentation generated from code.
+
+
+
+### [Documentation](https://michalskibinski109.github.io/py-draughts/)
 
 ## Usage
 
 
 
 #### Displays simple ascii board
 
@@ -59,32 +66,36 @@
  . . . . . . . . . .
  . . . . . . . . . .
  w . . . w . w . w .
  . w . w . w . w . w
  w . w . w . w . w .
 ```
 
-### Generate legal moves and validate moves
+#### Generate legal moves and validate moves
 
 ```python
 >>> board.push_from_str("10x42")
 Move: 10->42 is correct, but not legal in given position.
  Legal moves are: [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
 
 >>> list(board.legal_moves)
 [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
 ```
 
-### Generate fen string
+#### Generate fen string and load board from fen string
+
 
 ```python
+>>> board =Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
+Board initialized with shape (10, 10). (base.py:109)
+>>> board.push_from_str("28-37")
 >>> board.fen
-[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]
+'[FEN "B:W4,11,31,K33,K34,37,38,40,K41,43,K44,45,K46,47:BK3,21,27"]'
 ```
-### American checkers
+#### American checkers
 
 ```python
 >>> from draughts.american import Board
 >>> board = Board()
 Board initialized with shape (8, 8). (base.py:108)
 >>> board
  . b . b . b . b
@@ -101,15 +112,15 @@
 ## UI
 
 ```python
 from draughts.server import Server
 Server().run()
 ```
 
-### Use for testing your engine.
+#### Use for testing your engine.
 
 _Example with simplest possible engine._
 
 ```python
 >>> server = Server(get_best_move_method=lambda board: np.random.choice(list(board.legal_moves)))
 >>> server.run()
 INFO:     Started server process [1617]
```

### Comparing `py-draughts-0.9.8/draughts/__init__.py` & `py-draughts-0.9.9/draughts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A draughts library for Python, with move generation and validation,
 PDN parsing and writing. Supprots multiple variants of game.
 """
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 __author__ = "Michał Skibiński"
```

### Comparing `py-draughts-0.9.8/draughts/american.py` & `py-draughts-0.9.9/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/draughts/base.py` & `py-draughts-0.9.9/draughts/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from __future__ import annotations
 
 from abc import ABC
 from typing import Generator
 from collections import defaultdict
 import numpy as np
+import re
 
 from draughts.models import ENTITY_REPR, Color, Entity, SquareT
 from draughts.move import Move
 from draughts.utils import (
     logger,
     get_king_pseudo_legal_moves,
     get_man_pseudo_legal_moves,
@@ -106,14 +107,23 @@
         self.turn = Color.WHITE
         self._moves_stack: list[Move] = []
         logger.info(f"Board initialized with shape {self.shape}.")
 
     # @abstractmethod
     @property
     def legal_moves(self) -> Generator[Move, None, None]:
+        """
+        Return list legal moves for the current position.
+        *For every concrete variant of draughts this method should be overriden.*
+
+        .. warning::
+            Depending of implementation method can return generator or list.
+
+
+        """
         pass
 
     @property
     def position(self) -> np.ndarray:
         """Returns board position."""
         return self._pos
 
@@ -207,17 +217,45 @@
             ),
             '"]',
         ]
         return "".join(fen_components)
 
     @classmethod
     def from_fen(cls, fen: str) -> BaseBoard:
-        # [FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]
-        # remove everthing before W or B
-        raise NotImplementedError("Not implemented yet")
+        """
+        Creates a board from a FEN string by using regular expressions.
+        """
+        fen = fen.upper()
+        re_turn = re.compile(r"[WB]:")
+        re_white = re.compile(r"W[0-9K,]+")
+        re_black = re.compile(r"B[0-9K,]+")
+        turn = re_turn.search(fen).group(0)[0]
+        white = re_white.search(fen).group(0).replace("W", "")
+        black = re_black.search(fen).group(0).replace("B", "")
+        cls.STARTING_POSITION = np.zeros(cls.STARTING_POSITION.shape, dtype=np.int8)
+        if len(turn) != 1 or (len(white) == 0 and len(black) == 0):
+            raise ValueError(f"Wrong FEN: {fen}")
+        cls.__populate_from_list(white.split(","), Color.WHITE)
+        cls.__populate_from_list(black.split(","), Color.BLACK)
+        cls.turn = Color.WHITE if turn == "W" else Color.BLACK
+        return cls(starting_position=cls.STARTING_POSITION)
+
+    @classmethod
+    def __populate_from_list(cls, fen_list: list[str], color: Color) -> None:
+        board_range = range(1, cls.STARTING_POSITION.shape[0] + 1)
+        for sq in fen_list:
+            if sq.isdigit() and int(sq) in board_range:
+                cls.STARTING_POSITION[int(sq) - 1] = color.value
+            elif sq.startswith("K") and sq[1:].isdigit() and int(sq[1:]) in board_range:
+                cls.STARTING_POSITION[int(sq[1:]) - 1] = color.value * Entity.KING.value
+            else:
+                raise ValueError(
+                    f"Wrong FEN: invalid square value: {sq} for board with length\
+                        {cls.STARTING_POSITION.shape[0]}"
+                )
 
     @classmethod
     @property
     def info(cls) -> str:
         board_size = int(np.sqrt(cls.STARTING_POSITION.shape[0]))
         data = (
             f'[GameType "{cls.GAME_TYPE}"]\n'
@@ -256,19 +294,20 @@
             yield sq
 
     def __getitem__(self, key: SquareT) -> Entity:
         return self.position[key]
 
 
 if __name__ == "__main__":
-    board = BaseBoard(BaseBoard.STARTING_POSITION)
-    print(board)
-    # BaseBoard.from_fen(
-    #     '[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]'
-    # )
+    # board = BaseBoard(BaseBoard.STARTING_POSITION)
+    # print(board)
+    BaseBoard.from_fen(
+        '[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]'
+    )
+    BaseBoard.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 
 # print(board.info)
 #     m1 = Move([C3, B4])
 #     board.push(m1)
 
 #     m2 = Move([B6, A5])
 #     board.push(m2)
```

### Comparing `py-draughts-0.9.8/draughts/models.py` & `py-draughts-0.9.9/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/draughts/move.py` & `py-draughts-0.9.9/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/draughts/server.py` & `py-draughts-0.9.9/draughts/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         self.get_best_move_method = get_best_move_method
         if not get_best_move_method:
             self.get_best_move_method = lambda board: np.random.choice(
                 list(board.legal_moves)
             )
         self.templates = Jinja2Templates(directory=templates_dir)
         self.board = board
+        self.board = Board.from_fen(
+            "W:WK5,K6,12,K21,22,32,K46:B1,K3,18,29,K33,34,40,K42,45,K50"
+        )
         self.router = APIRouter()
         self.router.add_api_route("/", self.index)
         self.router.add_api_route("/set_board/{board_type}", self.set_board)
         self.router.add_api_route("/set_random_position", self.set_random_position)
         self.router.add_api_route("/random_move", self.get_best_move)
         self.router.add_api_route("/get_board_info", self.get_board_info)
         self.router.add_api_route("/get_legal_moves", self.get_legal_moves)
```

### Comparing `py-draughts-0.9.8/draughts/standard.py` & `py-draughts-0.9.9/draughts/standard.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,10 +146,11 @@
         return moves
 
 
 if __name__ == "__main__":
     board = Board()
     from pprint import pprint
 
-    pprint(board)
-    pprint(list(board.legal_moves))
-    print(board.fen)
+    Board.from_fen(
+        '[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]'
+    )
+    Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
```

### Comparing `py-draughts-0.9.8/draughts/static/css/style.css` & `py-draughts-0.9.9/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/draughts/static/js/script.js` & `py-draughts-0.9.9/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/draughts/templates/base.html` & `py-draughts-0.9.9/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/draughts/templates/index.html` & `py-draughts-0.9.9/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/draughts/utils.py` & `py-draughts-0.9.9/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/py_draughts.egg-info/PKG-INFO` & `py-draughts-0.9.9/py_draughts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 0.9.8
+Version: 0.9.9
 Summary: A draughts library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -32,23 +32,30 @@
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
-
-
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
 
-## [Documentation](https://michalskibinski109.github.io/py-draughts/)
+## Key features
+1. Provides beautiful web interface for testing your engine/playing against AI.
+2. Supports multiple variants of the game (with different board size). `standard`, `american` etc.
+3. Follows international draughts standards. like `fen` `pdn` etc.
+4. Allows to easily create new variants of the game. by extending the `Board` class.
+5. Accurate documentation generated from code.
+
+
+
+### [Documentation](https://michalskibinski109.github.io/py-draughts/)
 
 ## Usage
 
 
 
 #### Displays simple ascii board
 
@@ -88,32 +95,36 @@
  . . . . . . . . . .
  . . . . . . . . . .
  w . . . w . w . w .
  . w . w . w . w . w
  w . w . w . w . w .
 ```
 
-### Generate legal moves and validate moves
+#### Generate legal moves and validate moves
 
 ```python
 >>> board.push_from_str("10x42")
 Move: 10->42 is correct, but not legal in given position.
  Legal moves are: [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
 
 >>> list(board.legal_moves)
 [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
 ```
 
-### Generate fen string
+#### Generate fen string and load board from fen string
+
 
 ```python
+>>> board =Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
+Board initialized with shape (10, 10). (base.py:109)
+>>> board.push_from_str("28-37")
 >>> board.fen
-[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]
+'[FEN "B:W4,11,31,K33,K34,37,38,40,K41,43,K44,45,K46,47:BK3,21,27"]'
 ```
-### American checkers
+#### American checkers
 
 ```python
 >>> from draughts.american import Board
 >>> board = Board()
 Board initialized with shape (8, 8). (base.py:108)
 >>> board
  . b . b . b . b
@@ -130,15 +141,15 @@
 ## UI
 
 ```python
 from draughts.server import Server
 Server().run()
 ```
 
-### Use for testing your engine.
+#### Use for testing your engine.
 
 _Example with simplest possible engine._
 
 ```python
 >>> server = Server(get_best_move_method=lambda board: np.random.choice(list(board.legal_moves)))
 >>> server.run()
 INFO:     Started server process [1617]
```

### Comparing `py-draughts-0.9.8/py_draughts.egg-info/SOURCES.txt` & `py-draughts-0.9.9/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/setup.py` & `py-draughts-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/test/test_american_board.py` & `py-draughts-0.9.9/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.8/test/test_board.py` & `py-draughts-0.9.9/test/test_board.py`

 * *Files identical despite different names*

