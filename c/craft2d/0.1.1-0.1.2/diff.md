# Comparing `tmp/craft2d-0.1.1.tar.gz` & `tmp/craft2d-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft2d-0.1.1.tar", max compression
+gzip compressed data, was "craft2d-0.1.2.tar", max compression
```

## Comparing `craft2d-0.1.1.tar` & `craft2d-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      472 2023-07-10 19:52:20.788976 craft2d-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.1/craft2d/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.1/craft2d/config/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.1/craft2d/env/__init__.py
--rw-r--r--   0        0        0    12324 2023-07-12 11:58:46.686133 craft2d-0.1.1/craft2d/env/environment.py
--rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.1/craft2d/render/__init__.py
--rw-r--r--   0        0        0    10024 2023-07-12 12:28:33.746399 craft2d-0.1.1/craft2d/render/render.py
--rw-r--r--   0        0        0     2193 2023-07-09 20:09:51.278818 craft2d-0.1.1/craft2d/resources/agent/agent-down.png
--rw-r--r--   0        0        0     2111 2023-07-09 20:09:25.442353 craft2d-0.1.1/craft2d/resources/agent/agent-left.png
--rw-r--r--   0        0        0     2153 2023-07-09 20:09:37.887138 craft2d-0.1.1/craft2d/resources/agent/agent-right.png
--rw-r--r--   0        0        0     2103 2023-07-09 20:09:11.258794 craft2d-0.1.1/craft2d/resources/agent/agent-up.png
--rw-r--r--   0        0        0     1797 2023-07-09 20:14:01.501432 craft2d-0.1.1/craft2d/resources/farm/plant-large.png
--rw-r--r--   0        0        0     1219 2023-07-09 20:13:45.609907 craft2d-0.1.1/craft2d/resources/farm/plant-medium.png
--rw-r--r--   0        0        0     1000 2023-07-09 20:13:26.261484 craft2d-0.1.1/craft2d/resources/farm/plant-small.png
--rw-r--r--   0        0        0     1074 2023-07-09 20:15:44.310385 craft2d-0.1.1/craft2d/resources/objects/bridge.png
--rw-r--r--   0        0        0     3400 2023-07-09 20:30:59.755816 craft2d-0.1.1/craft2d/resources/objects/crafting-table.png
--rw-r--r--   0        0        0     5133 2023-07-10 19:33:45.377024 craft2d-0.1.1/craft2d/resources/objects/gem.png
--rw-r--r--   0        0        0     1007 2023-07-09 20:29:41.393116 craft2d-0.1.1/craft2d/resources/objects/grass.png
--rw-r--r--   0        0        0     3178 2023-07-10 16:32:23.402820 craft2d-0.1.1/craft2d/resources/objects/rope.png
--rw-r--r--   0        0        0     3823 2023-07-10 16:31:28.142800 craft2d-0.1.1/craft2d/resources/objects/sticks.png
--rw-r--r--   0        0        0     1364 2023-07-09 20:14:47.718624 craft2d-0.1.1/craft2d/resources/objects/stone.png
--rw-r--r--   0        0        0     1840 2023-07-09 20:14:15.424009 craft2d-0.1.1/craft2d/resources/objects/tree.png
--rw-r--r--   0        0        0     1423 2023-07-09 20:28:11.817175 craft2d-0.1.1/craft2d/resources/objects/weapon-advanced.png
--rw-r--r--   0        0        0     1437 2023-07-09 20:18:43.082515 craft2d-0.1.1/craft2d/resources/objects/weapon-basic.png
--rw-r--r--   0        0        0     1866 2023-07-09 20:15:14.696923 craft2d-0.1.1/craft2d/resources/objects/wood.png
--rw-r--r--   0        0        0     1164 2023-07-09 20:11:48.365759 craft2d-0.1.1/craft2d/resources/terrain/grass.png
--rw-r--r--   0        0        0     2474 2023-07-09 20:12:25.101611 craft2d-0.1.1/craft2d/resources/terrain/island.png
--rw-r--r--   0        0        0     1019 2023-07-10 17:23:00.155464 craft2d-0.1.1/craft2d/resources/terrain/water.png
--rw-r--r--   0        0        0      538 2023-07-12 12:31:12.704398 craft2d-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 craft2d-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-07-12 15:58:14.885516 craft2d-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.2/craft2d/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.2/craft2d/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.2/craft2d/env/__init__.py
+-rw-r--r--   0        0        0    12324 2023-07-12 16:06:09.446174 craft2d-0.1.2/craft2d/env/environment.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.2/craft2d/render/__init__.py
+-rw-r--r--   0        0        0    10024 2023-07-12 12:28:33.746399 craft2d-0.1.2/craft2d/render/render.py
+-rw-r--r--   0        0        0     2193 2023-07-09 20:09:51.278818 craft2d-0.1.2/craft2d/resources/agent/agent-down.png
+-rw-r--r--   0        0        0     2111 2023-07-09 20:09:25.442353 craft2d-0.1.2/craft2d/resources/agent/agent-left.png
+-rw-r--r--   0        0        0     2153 2023-07-09 20:09:37.887138 craft2d-0.1.2/craft2d/resources/agent/agent-right.png
+-rw-r--r--   0        0        0     2103 2023-07-09 20:09:11.258794 craft2d-0.1.2/craft2d/resources/agent/agent-up.png
+-rw-r--r--   0        0        0     1797 2023-07-09 20:14:01.501432 craft2d-0.1.2/craft2d/resources/farm/plant-large.png
+-rw-r--r--   0        0        0     1219 2023-07-09 20:13:45.609907 craft2d-0.1.2/craft2d/resources/farm/plant-medium.png
+-rw-r--r--   0        0        0     1000 2023-07-09 20:13:26.261484 craft2d-0.1.2/craft2d/resources/farm/plant-small.png
+-rw-r--r--   0        0        0     1074 2023-07-09 20:15:44.310385 craft2d-0.1.2/craft2d/resources/objects/bridge.png
+-rw-r--r--   0        0        0     3400 2023-07-09 20:30:59.755816 craft2d-0.1.2/craft2d/resources/objects/crafting-table.png
+-rw-r--r--   0        0        0     5133 2023-07-10 19:33:45.377024 craft2d-0.1.2/craft2d/resources/objects/gem.png
+-rw-r--r--   0        0        0     1007 2023-07-09 20:29:41.393116 craft2d-0.1.2/craft2d/resources/objects/grass.png
+-rw-r--r--   0        0        0     3178 2023-07-10 16:32:23.402820 craft2d-0.1.2/craft2d/resources/objects/rope.png
+-rw-r--r--   0        0        0     3823 2023-07-10 16:31:28.142800 craft2d-0.1.2/craft2d/resources/objects/sticks.png
+-rw-r--r--   0        0        0     1364 2023-07-09 20:14:47.718624 craft2d-0.1.2/craft2d/resources/objects/stone.png
+-rw-r--r--   0        0        0     1840 2023-07-09 20:14:15.424009 craft2d-0.1.2/craft2d/resources/objects/tree.png
+-rw-r--r--   0        0        0     1423 2023-07-09 20:28:11.817175 craft2d-0.1.2/craft2d/resources/objects/weapon-advanced.png
+-rw-r--r--   0        0        0     1437 2023-07-09 20:18:43.082515 craft2d-0.1.2/craft2d/resources/objects/weapon-basic.png
+-rw-r--r--   0        0        0     1866 2023-07-09 20:15:14.696923 craft2d-0.1.2/craft2d/resources/objects/wood.png
+-rw-r--r--   0        0        0     1164 2023-07-09 20:11:48.365759 craft2d-0.1.2/craft2d/resources/terrain/grass.png
+-rw-r--r--   0        0        0     2474 2023-07-09 20:12:25.101611 craft2d-0.1.2/craft2d/resources/terrain/island.png
+-rw-r--r--   0        0        0     1019 2023-07-10 17:23:00.155464 craft2d-0.1.2/craft2d/resources/terrain/water.png
+-rw-r--r--   0        0        0      538 2023-07-12 16:07:54.910818 craft2d-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 craft2d-0.1.2/PKG-INFO
```

### Comparing `craft2d-0.1.1/craft2d/env/environment.py` & `craft2d-0.1.2/craft2d/env/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 LEFT = 1
 UP = 2
 DOWN = 3
 USE = 4
 
 MAX_RESOURCE_COUNT = 3
 RESOURCE_COUNTS = {
-    "tree": 2,
-    "stone": 1,
-    "grass": 1,
+    "tree": 4,
+    "stone": 2,
+    "grass": 2,
     "gem": 1,
 }
 ENVIRONMENT_OBJECTS = (
     "tree",
     "stone",
     "grass",
     "crafting-table",
@@ -40,16 +40,16 @@
 )
 TASKS = {
     "get-wood": 0,
     "get-stone": 1,
     "get-grass": 2,
     "make-sticks": 3,
     "make-rope": 4,
-    "make-basic-weapon": 5,
-    "make-bridge": 6,
+    "make-bridge": 5,
+    "make-basic-weapon": 6,
     "get-gem": 7,
     "make-advanced-weapon": 8,
 }
 
 
 class Craft2dEnv(gym.Env):
     def __init__(
@@ -314,31 +314,31 @@
 
     def _handle_crafting_interaction(self):
         if self.inventory[6] > 0 and self.inventory[7] > 0:
             # Advanced weapon
             self.inventory[8] += 1
             self.inventory[6] -= 1
             self.inventory[7] -= 1
-        if self.inventory[3] > 0 and self.inventory[1] >= 1:
+        if self.inventory[3] > 0 and self.inventory[1] >= 2:
             # Weapon
             self.inventory[6] += 1
             self.inventory[3] -= 1
-            self.inventory[1] -= 1
+            self.inventory[1] -= 2
         elif self.inventory[3] > 0 and self.inventory[4] >= 1:
             # Bridge
             self.inventory[5] += 1
             self.inventory[3] -= 1
             self.inventory[4] -= 1
-        elif self.inventory[0] > 0:
+        elif self.inventory[0] > 1:
             # Sticks
-            self.inventory[0] -= 1
+            self.inventory[0] -= 2
             self.inventory[3] += 1
-        elif self.inventory[2] > 0:
+        elif self.inventory[2] > 1:
             # Rope
-            self.inventory[2] -= 1
+            self.inventory[2] -= 2
             self.inventory[4] += 1
 
     def _handle_water_interaction(self, itr_row, itr_col):
         # Place bridge on water if agent has bridge in inventory
         water_idx_env = ENVIRONMENT_OBJECTS.index("water")
         bridge_idx_env = ENVIRONMENT_OBJECTS.index("bridge")
         bridge_idx_inv = INVENTORY_OBJECTS.index("bridge")
```

### Comparing `craft2d-0.1.1/craft2d/render/render.py` & `craft2d-0.1.2/craft2d/render/render.py`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/agent/agent-down.png` & `craft2d-0.1.2/craft2d/resources/agent/agent-down.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/agent/agent-left.png` & `craft2d-0.1.2/craft2d/resources/agent/agent-left.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/agent/agent-right.png` & `craft2d-0.1.2/craft2d/resources/agent/agent-right.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/agent/agent-up.png` & `craft2d-0.1.2/craft2d/resources/agent/agent-up.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/farm/plant-large.png` & `craft2d-0.1.2/craft2d/resources/farm/plant-large.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/farm/plant-medium.png` & `craft2d-0.1.2/craft2d/resources/farm/plant-medium.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/farm/plant-small.png` & `craft2d-0.1.2/craft2d/resources/farm/plant-small.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/bridge.png` & `craft2d-0.1.2/craft2d/resources/objects/bridge.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/crafting-table.png` & `craft2d-0.1.2/craft2d/resources/objects/crafting-table.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/gem.png` & `craft2d-0.1.2/craft2d/resources/objects/gem.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/grass.png` & `craft2d-0.1.2/craft2d/resources/objects/grass.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/rope.png` & `craft2d-0.1.2/craft2d/resources/objects/rope.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/sticks.png` & `craft2d-0.1.2/craft2d/resources/objects/sticks.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/stone.png` & `craft2d-0.1.2/craft2d/resources/objects/stone.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/tree.png` & `craft2d-0.1.2/craft2d/resources/objects/tree.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/weapon-advanced.png` & `craft2d-0.1.2/craft2d/resources/objects/weapon-advanced.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/weapon-basic.png` & `craft2d-0.1.2/craft2d/resources/objects/weapon-basic.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/objects/wood.png` & `craft2d-0.1.2/craft2d/resources/objects/wood.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/terrain/grass.png` & `craft2d-0.1.2/craft2d/resources/terrain/grass.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/terrain/island.png` & `craft2d-0.1.2/craft2d/resources/terrain/island.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/craft2d/resources/terrain/water.png` & `craft2d-0.1.2/craft2d/resources/terrain/water.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.1/pyproject.toml` & `craft2d-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "craft2d"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Tristan Bester <tristanbester@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 numpy = "^1.25.1"
```

### Comparing `craft2d-0.1.1/PKG-INFO` & `craft2d-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft2d
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Tristan Bester
 Author-email: tristanbester@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,18 +20,18 @@
 ## Skills
 ### Easy
 1. Get wood: Tree 
 2. Get stone: Stone
 3. Get grass: Grass
 
 ### Medium
-1. Make sticks: Get wood + Use Crafting Table
-2. Make rope: Get grass + Use Crafting Table
+1. Make sticks: Get wood x 2 + Use Crafting Table
+2. Make rope: Get grass x 2 + Use Crafting Table
 
 ### Hard
-1. Make weapon: Sticks + Stone + Use Crafting Table
+1. Make weapon: Sticks x 1 + Stone x 2 + Use Crafting Table
 2. Make bridge: Rope + Sticks + Use Crafting Table
 
 ### Very Hard
 1. Get diamond: Bridge + water + collect diamond
 2. Make diamond weapon: Diamond + weapon + Use Crafting Table
 3. Plant & harvest before time runs out?
```

