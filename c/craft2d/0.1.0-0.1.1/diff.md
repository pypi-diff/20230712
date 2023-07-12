# Comparing `tmp/craft2d-0.1.0.tar.gz` & `tmp/craft2d-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft2d-0.1.0.tar", max compression
+gzip compressed data, was "craft2d-0.1.1.tar", max compression
```

## Comparing `craft2d-0.1.0.tar` & `craft2d-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,30 @@
--rw-r--r--   0        0        0      472 2023-07-10 19:52:20.788976 craft2d-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.0/craft2d/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.0/craft2d/config/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.0/craft2d/env/__init__.py
--rw-r--r--   0        0        0    12324 2023-07-12 11:58:46.686133 craft2d-0.1.0/craft2d/env/environment.py
--rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.0/craft2d/render/__init__.py
--rw-r--r--   0        0        0     9438 2023-07-11 18:17:07.906805 craft2d-0.1.0/craft2d/render/render.py
--rw-r--r--   0        0        0      538 2023-07-11 18:36:38.388337 craft2d-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 craft2d-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      472 2023-07-10 19:52:20.788976 craft2d-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.1/craft2d/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.1/craft2d/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.1/craft2d/env/__init__.py
+-rw-r--r--   0        0        0    12324 2023-07-12 11:58:46.686133 craft2d-0.1.1/craft2d/env/environment.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.1/craft2d/render/__init__.py
+-rw-r--r--   0        0        0    10024 2023-07-12 12:28:33.746399 craft2d-0.1.1/craft2d/render/render.py
+-rw-r--r--   0        0        0     2193 2023-07-09 20:09:51.278818 craft2d-0.1.1/craft2d/resources/agent/agent-down.png
+-rw-r--r--   0        0        0     2111 2023-07-09 20:09:25.442353 craft2d-0.1.1/craft2d/resources/agent/agent-left.png
+-rw-r--r--   0        0        0     2153 2023-07-09 20:09:37.887138 craft2d-0.1.1/craft2d/resources/agent/agent-right.png
+-rw-r--r--   0        0        0     2103 2023-07-09 20:09:11.258794 craft2d-0.1.1/craft2d/resources/agent/agent-up.png
+-rw-r--r--   0        0        0     1797 2023-07-09 20:14:01.501432 craft2d-0.1.1/craft2d/resources/farm/plant-large.png
+-rw-r--r--   0        0        0     1219 2023-07-09 20:13:45.609907 craft2d-0.1.1/craft2d/resources/farm/plant-medium.png
+-rw-r--r--   0        0        0     1000 2023-07-09 20:13:26.261484 craft2d-0.1.1/craft2d/resources/farm/plant-small.png
+-rw-r--r--   0        0        0     1074 2023-07-09 20:15:44.310385 craft2d-0.1.1/craft2d/resources/objects/bridge.png
+-rw-r--r--   0        0        0     3400 2023-07-09 20:30:59.755816 craft2d-0.1.1/craft2d/resources/objects/crafting-table.png
+-rw-r--r--   0        0        0     5133 2023-07-10 19:33:45.377024 craft2d-0.1.1/craft2d/resources/objects/gem.png
+-rw-r--r--   0        0        0     1007 2023-07-09 20:29:41.393116 craft2d-0.1.1/craft2d/resources/objects/grass.png
+-rw-r--r--   0        0        0     3178 2023-07-10 16:32:23.402820 craft2d-0.1.1/craft2d/resources/objects/rope.png
+-rw-r--r--   0        0        0     3823 2023-07-10 16:31:28.142800 craft2d-0.1.1/craft2d/resources/objects/sticks.png
+-rw-r--r--   0        0        0     1364 2023-07-09 20:14:47.718624 craft2d-0.1.1/craft2d/resources/objects/stone.png
+-rw-r--r--   0        0        0     1840 2023-07-09 20:14:15.424009 craft2d-0.1.1/craft2d/resources/objects/tree.png
+-rw-r--r--   0        0        0     1423 2023-07-09 20:28:11.817175 craft2d-0.1.1/craft2d/resources/objects/weapon-advanced.png
+-rw-r--r--   0        0        0     1437 2023-07-09 20:18:43.082515 craft2d-0.1.1/craft2d/resources/objects/weapon-basic.png
+-rw-r--r--   0        0        0     1866 2023-07-09 20:15:14.696923 craft2d-0.1.1/craft2d/resources/objects/wood.png
+-rw-r--r--   0        0        0     1164 2023-07-09 20:11:48.365759 craft2d-0.1.1/craft2d/resources/terrain/grass.png
+-rw-r--r--   0        0        0     2474 2023-07-09 20:12:25.101611 craft2d-0.1.1/craft2d/resources/terrain/island.png
+-rw-r--r--   0        0        0     1019 2023-07-10 17:23:00.155464 craft2d-0.1.1/craft2d/resources/terrain/water.png
+-rw-r--r--   0        0        0      538 2023-07-12 12:31:12.704398 craft2d-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 craft2d-0.1.1/PKG-INFO
```

### Comparing `craft2d-0.1.0/craft2d/env/environment.py` & `craft2d-0.1.1/craft2d/env/environment.py`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.0/craft2d/render/render.py` & `craft2d-0.1.1/craft2d/render/render.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import importlib.util
 from itertools import product
+from pathlib import Path
 
 import numpy as np
 import pygame
 
 PLAYER_IMGS_PATH = [
     "resources/agent/agent-right.png",
     "resources/agent/agent-left.png",
@@ -21,14 +23,24 @@
 WEAPON_BASIC_IMG_PATH = "resources/objects/weapon-basic.png"
 ISLAND_IMG_PATH = "resources/terrain/island.png"
 WATER_IMG_PATH = "resources/terrain/water.png"
 GEM_IMG_PATH = "resources/objects/gem.png"
 WEAPON_ADV_IMG_PATH = "resources/objects/weapon-advanced.png"
 
 
+def get_file_path(file_name):
+    spec = importlib.util.find_spec("craft2d")
+    if spec is None:
+        raise ImportError("Package 'craft2d' not found.")
+
+    package_path = Path(spec.origin)
+    file_path = package_path.parent / file_name
+    return str(file_path)
+
+
 class Renderer:
     def __init__(
         self,
         n_rows: int,
         n_cols: int,
         env_objects: list[str],
         inv_objects: list[str],
@@ -44,29 +56,33 @@
         self.window_height = window_height
         self.cell_size = (
             self.window_width / (self.n_cols + 2),  # +2 for inventory
             self.window_height / self.n_rows,
         )
 
         # Load assets
-        self.background_image = self._load_image(BACKGROUND_IMG_PATH)
+        self.background_image = self._load_image(get_file_path(BACKGROUND_IMG_PATH))
         self.player_images = self._load_images(PLAYER_IMGS_PATH)
-        self.tree_image = self._load_image(TREE_IMG_PATH)
-        self.wood_image = self._load_image(WOOD_IMG_PATH)
-        self.stone_image = self._load_image(STONE_IMG_PATH)
-        self.grass_image = self._load_image(GRASS_IMG_PATH)
-        self.crafting_table_image = self._load_image(CRAFTING_TABLE_IMG_PATH)
-        self.sticks_image = self._load_image(STICKS_IMG_PATH)
-        self.rope_image = self._load_image(ROPE_IMG_PATH)
-        self.bridge_image = self._load_image(BRIDGE_IMG_PATH)
-        self.weapon_basic_image = self._load_image(WEAPON_BASIC_IMG_PATH)
-        self.island_image = self._load_image(ISLAND_IMG_PATH)
-        self.water_image = self._load_image(WATER_IMG_PATH)
-        self.gem_image = self._load_image(GEM_IMG_PATH)
-        self.weapon_advanced_image = self._load_image(WEAPON_ADV_IMG_PATH)
+        self.tree_image = self._load_image(get_file_path(TREE_IMG_PATH))
+        self.wood_image = self._load_image(get_file_path(WOOD_IMG_PATH))
+        self.stone_image = self._load_image(get_file_path(STONE_IMG_PATH))
+        self.grass_image = self._load_image(get_file_path(GRASS_IMG_PATH))
+        self.crafting_table_image = self._load_image(
+            get_file_path(CRAFTING_TABLE_IMG_PATH)
+        )
+        self.sticks_image = self._load_image(get_file_path(STICKS_IMG_PATH))
+        self.rope_image = self._load_image(get_file_path(ROPE_IMG_PATH))
+        self.bridge_image = self._load_image(get_file_path(BRIDGE_IMG_PATH))
+        self.weapon_basic_image = self._load_image(get_file_path(WEAPON_BASIC_IMG_PATH))
+        self.island_image = self._load_image(get_file_path(ISLAND_IMG_PATH))
+        self.water_image = self._load_image(get_file_path(WATER_IMG_PATH))
+        self.gem_image = self._load_image(get_file_path(GEM_IMG_PATH))
+        self.weapon_advanced_image = self._load_image(
+            get_file_path(WEAPON_ADV_IMG_PATH)
+        )
 
         # Initialise pygame
         pygame.init()
         self.clock = pygame.time.Clock()
 
     def _render_background(self, grid):
         for r, c in product(range(self.n_rows), range(self.n_cols)):
@@ -186,15 +202,15 @@
             pygame.image.load(path),
             self.cell_size,
         )
 
     def _load_images(self, paths):
         images = []
         for path in paths:
-            images.append(self._load_image(path))
+            images.append(self._load_image(get_file_path(path)))
         return images
 
 
 class HumanRenderer(Renderer):
     def __init__(
         self,
         n_rows: int,
```

### Comparing `craft2d-0.1.0/pyproject.toml` & `craft2d-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "craft2d"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Tristan Bester <tristanbester@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 numpy = "^1.25.1"
```

### Comparing `craft2d-0.1.0/PKG-INFO` & `craft2d-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft2d
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Tristan Bester
 Author-email: tristanbester@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

