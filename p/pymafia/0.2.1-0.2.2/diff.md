# Comparing `tmp/pymafia-0.2.1.tar.gz` & `tmp/pymafia-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymafia-0.2.1.tar", max compression
+gzip compressed data, was "pymafia-0.2.2.tar", max compression
```

## Comparing `pymafia-0.2.1.tar` & `pymafia-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0     1068 2023-04-27 18:27:20.603026 pymafia-0.2.1/LICENSE
--rw-r--r--   0        0        0     1964 2023-04-27 18:27:20.603026 pymafia-0.2.1/README.md
--rw-r--r--   0        0        0     1283 2023-04-27 18:27:59.203652 pymafia-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      390 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/__init__.py
--rw-r--r--   0        0        0      283 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/ash/__init__.py
--rw-r--r--   0        0        0     3193 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/ash/conversion.py
--rw-r--r--   0        0        0     1421 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/ash/library.py
--rw-r--r--   0        0        0     3315 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/combat.py
--rw-r--r--   0        0        0     1449 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/__init__.py
--rw-r--r--   0        0        0     2442 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/bounty.py
--rw-r--r--   0        0        0     1836 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/class_.py
--rw-r--r--   0        0        0     2464 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/coinmaster.py
--rw-r--r--   0        0        0     2526 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/effect.py
--rw-r--r--   0        0        0     2653 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/element.py
--rw-r--r--   0        0        0     6826 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/familiar.py
--rw-r--r--   0        0        0    11495 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/item.py
--rw-r--r--   0        0        0     5338 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/location.py
--rw-r--r--   0        0        0     6712 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/monster.py
--rw-r--r--   0        0        0     1976 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/path.py
--rw-r--r--   0        0        0     2772 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/phylum.py
--rw-r--r--   0        0        0     2765 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/servant.py
--rw-r--r--   0        0        0     3160 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/skill.py
--rw-r--r--   0        0        0     2542 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/slot.py
--rw-r--r--   0        0        0     1314 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/stat.py
--rw-r--r--   0        0        0     2610 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/thrall.py
--rw-r--r--   0        0        0     2889 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/vykea.py
--rw-r--r--   0        0        0      545 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/__init__.py
--rw-r--r--   0        0        0      583 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/barrel_god.py
--rw-r--r--   0        0        0      890 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/boxing_daycare.py
--rw-r--r--   0        0        0     1350 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/cartography.py
--rw-r--r--   0        0        0     1030 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/cosplay_saber.py
--rw-r--r--   0        0        0     1784 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/crimbo_shrub.py
--rw-r--r--   0        0        0     1286 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/god_lobster.py
--rw-r--r--   0        0        0     1569 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/love_tunnel.py
--rw-r--r--   0        0        0     1044 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/mumming_trunk.py
--rw-r--r--   0        0        0     3518 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/pantogram.py
--rw-r--r--   0        0        0     1597 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/protonic_pack.py
--rw-r--r--   0        0        0     1139 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/snojo.py
--rw-r--r--   0        0        0     1299 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/songboom.py
--rw-r--r--   0        0        0      670 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/stomping_boots.py
--rw-r--r--   0        0        0     1408 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/witchess.py
--rw-r--r--   0        0        0      125 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/kolmafia/__init__.py
--rw-r--r--   0        0        0     1759 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/kolmafia/kolmafia.py
--rw-r--r--   0        0        0     1572 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/kolmafia/patch.py
--rw-r--r--   0        0        0     1682 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/player.py
--rw-r--r--   0        0        0     1148 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/preference.py
--rw-r--r--   0        0        0     1277 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/utils.py
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 pymafia-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-12 19:04:30.209512 pymafia-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5241 2023-07-12 19:04:30.209512 pymafia-0.2.2/README.md
+-rw-r--r--   0        0        0     1283 2023-07-12 19:05:15.994309 pymafia-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      390 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/__init__.py
+-rw-r--r--   0        0        0      283 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/ash/__init__.py
+-rw-r--r--   0        0        0     3251 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/ash/conversion.py
+-rw-r--r--   0        0        0     1421 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/ash/library.py
+-rw-r--r--   0        0        0     3315 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/combat.py
+-rw-r--r--   0        0        0     1527 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/datatypes/__init__.py
+-rw-r--r--   0        0        0     2442 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/datatypes/bounty.py
+-rw-r--r--   0        0        0     1836 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/datatypes/class_.py
+-rw-r--r--   0        0        0     2464 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/coinmaster.py
+-rw-r--r--   0        0        0     2526 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/effect.py
+-rw-r--r--   0        0        0     2653 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/element.py
+-rw-r--r--   0        0        0     6826 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/familiar.py
+-rw-r--r--   0        0        0    11495 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/item.py
+-rw-r--r--   0        0        0     5338 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/location.py
+-rw-r--r--   0        0        0     1813 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/modifier.py
+-rw-r--r--   0        0        0     6712 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/monster.py
+-rw-r--r--   0        0        0     1976 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/path.py
+-rw-r--r--   0        0        0     2772 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/phylum.py
+-rw-r--r--   0        0        0     2765 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/servant.py
+-rw-r--r--   0        0        0     3160 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/skill.py
+-rw-r--r--   0        0        0     2542 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/slot.py
+-rw-r--r--   0        0        0     1314 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/stat.py
+-rw-r--r--   0        0        0     2610 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/thrall.py
+-rw-r--r--   0        0        0     2889 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/vykea.py
+-rw-r--r--   0        0        0      545 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/barrel_god.py
+-rw-r--r--   0        0        0      890 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/boxing_daycare.py
+-rw-r--r--   0        0        0     1350 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/cartography.py
+-rw-r--r--   0        0        0     1030 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/cosplay_saber.py
+-rw-r--r--   0        0        0     1784 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/crimbo_shrub.py
+-rw-r--r--   0        0        0     1286 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/god_lobster.py
+-rw-r--r--   0        0        0     1569 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/love_tunnel.py
+-rw-r--r--   0        0        0     1044 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/mumming_trunk.py
+-rw-r--r--   0        0        0     3518 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/pantogram.py
+-rw-r--r--   0        0        0     1597 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/protonic_pack.py
+-rw-r--r--   0        0        0     1139 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/snojo.py
+-rw-r--r--   0        0        0     1299 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/songboom.py
+-rw-r--r--   0        0        0      670 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/stomping_boots.py
+-rw-r--r--   0        0        0     1408 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/witchess.py
+-rw-r--r--   0        0        0      125 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/kolmafia/__init__.py
+-rw-r--r--   0        0        0     1397 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/kolmafia/kolmafia.py
+-rw-r--r--   0        0        0     1572 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/kolmafia/patch.py
+-rw-r--r--   0        0        0     1682 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/player.py
+-rw-r--r--   0        0        0     1148 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/preference.py
+-rw-r--r--   0        0        0     1277 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/utils.py
+-rw-r--r--   0        0        0     5913 1970-01-01 00:00:00.000000 pymafia-0.2.2/PKG-INFO
```

### Comparing `pymafia-0.2.1/LICENSE` & `pymafia-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/pyproject.toml` & `pymafia-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymafia"
-version = "0.2.1"  # This is the standard placeholder for poetry-dynamic-versioning
+version = "0.2.2"  # This is the standard placeholder for poetry-dynamic-versioning
 description = "A Python module and bridge for reflecting KoLmafia's Java environment"
 license = "MIT"
 authors = ["MrFizzyBubbs <MrFizzyBubbs@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MrFizzyBubbs/pymafia"
 
 [tool.poetry.dependencies]
```

### Comparing `pymafia-0.2.1/src/pymafia/ash/conversion.py` & `pymafia-0.2.2/src/pymafia/ash/conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Class,
     Coinmaster,
     Effect,
     Element,
     Familiar,
     Item,
     Location,
+    Modifier,
     Monster,
     Path,
     Phylum,
     Servant,
     Skill,
     Slot,
     Stat,
@@ -47,14 +48,15 @@
     km.DataTypes.COINMASTER_TYPE: Coinmaster,
     km.DataTypes.PHYLUM_TYPE: Phylum,
     km.DataTypes.BOUNTY_TYPE: Bounty,
     km.DataTypes.THRALL_TYPE: Thrall,
     km.DataTypes.SERVANT_TYPE: Servant,
     km.DataTypes.VYKEA_TYPE: Vykea,
     km.DataTypes.PATH_TYPE: Path,
+    km.DataTypes.MODIFIER_TYPE: Modifier,
 }
 
 
 def to_java(obj: Any) -> Any:
     """Convert a Python object to a KoLmafia Value or PluralValue."""
     if isinstance(obj, (bool, int, float, str)):
         return km.Value(obj)
```

### Comparing `pymafia-0.2.1/src/pymafia/ash/library.py` & `pymafia-0.2.2/src/pymafia/ash/library.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/combat.py` & `pymafia-0.2.2/src/pymafia/combat.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/__init__.py` & `pymafia-0.2.2/src/pymafia/datatypes/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     "Effect",
     "EffectQuality",
     "Element",
     "Familiar",
     "Item",
     "CandyType",
     "Location",
+    "Modifier",
     "Monster",
     "Path",
     "Phylum",
     "Servant",
     "Skill",
     "Slot",
     "Stat",
@@ -28,14 +29,15 @@
 from pymafia.datatypes.class_ import Class
 from pymafia.datatypes.coinmaster import Coinmaster
 from pymafia.datatypes.effect import Effect, EffectQuality
 from pymafia.datatypes.element import Element
 from pymafia.datatypes.familiar import Familiar
 from pymafia.datatypes.item import CandyType, Item
 from pymafia.datatypes.location import Location
+from pymafia.datatypes.modifier import Modifier
 from pymafia.datatypes.monster import Monster
 from pymafia.datatypes.path import Path
 from pymafia.datatypes.phylum import Phylum
 from pymafia.datatypes.servant import Servant
 from pymafia.datatypes.skill import Skill
 from pymafia.datatypes.slot import Slot
 from pymafia.datatypes.stat import Stat
@@ -56,8 +58,9 @@
     Coinmaster,
     Phylum,
     Bounty,
     Thrall,
     Servant,
     Vykea,
     Path,
+    Modifier,
 )
```

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/bounty.py` & `pymafia-0.2.2/src/pymafia/datatypes/bounty.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/class_.py` & `pymafia-0.2.2/src/pymafia/datatypes/class_.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/coinmaster.py` & `pymafia-0.2.2/src/pymafia/datatypes/coinmaster.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/effect.py` & `pymafia-0.2.2/src/pymafia/datatypes/effect.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/element.py` & `pymafia-0.2.2/src/pymafia/datatypes/element.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/familiar.py` & `pymafia-0.2.2/src/pymafia/datatypes/familiar.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/item.py` & `pymafia-0.2.2/src/pymafia/datatypes/item.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/location.py` & `pymafia-0.2.2/src/pymafia/datatypes/location.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/monster.py` & `pymafia-0.2.2/src/pymafia/datatypes/monster.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/path.py` & `pymafia-0.2.2/src/pymafia/datatypes/path.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/phylum.py` & `pymafia-0.2.2/src/pymafia/datatypes/phylum.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/servant.py` & `pymafia-0.2.2/src/pymafia/datatypes/servant.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/skill.py` & `pymafia-0.2.2/src/pymafia/datatypes/skill.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/slot.py` & `pymafia-0.2.2/src/pymafia/datatypes/slot.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/stat.py` & `pymafia-0.2.2/src/pymafia/datatypes/stat.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/thrall.py` & `pymafia-0.2.2/src/pymafia/datatypes/thrall.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/datatypes/vykea.py` & `pymafia-0.2.2/src/pymafia/datatypes/vykea.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/__init__.py` & `pymafia-0.2.2/src/pymafia/iotms/__init__.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/barrel_god.py` & `pymafia-0.2.2/src/pymafia/iotms/barrel_god.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/boxing_daycare.py` & `pymafia-0.2.2/src/pymafia/iotms/boxing_daycare.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/cartography.py` & `pymafia-0.2.2/src/pymafia/iotms/cartography.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/cosplay_saber.py` & `pymafia-0.2.2/src/pymafia/iotms/cosplay_saber.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/crimbo_shrub.py` & `pymafia-0.2.2/src/pymafia/iotms/crimbo_shrub.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/god_lobster.py` & `pymafia-0.2.2/src/pymafia/iotms/god_lobster.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/love_tunnel.py` & `pymafia-0.2.2/src/pymafia/iotms/love_tunnel.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/mumming_trunk.py` & `pymafia-0.2.2/src/pymafia/iotms/mumming_trunk.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/pantogram.py` & `pymafia-0.2.2/src/pymafia/iotms/pantogram.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/protonic_pack.py` & `pymafia-0.2.2/src/pymafia/iotms/protonic_pack.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/snojo.py` & `pymafia-0.2.2/src/pymafia/iotms/snojo.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/songboom.py` & `pymafia-0.2.2/src/pymafia/iotms/songboom.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/stomping_boots.py` & `pymafia-0.2.2/src/pymafia/iotms/stomping_boots.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/iotms/witchess.py` & `pymafia-0.2.2/src/pymafia/iotms/witchess.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/kolmafia/kolmafia.py` & `pymafia-0.2.2/src/pymafia/kolmafia/kolmafia.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,29 @@
-import json
 import os
 import re
 import urllib.request
 import zipfile
 from typing import Any, Iterable
 
 import jpype
 
 import pymafia.kolmafia.patch as patch
+import pymafia_config
 
-GITHUB_RELEASE_URL = "https://api.github.com/repos/kolmafia/kolmafia/releases/"
 GITHUB_DOWNLOAD_URL = "https://github.com/kolmafia/kolmafia/releases/download/"
 JAVA_PATTERN = "(net\\/sourceforge\\/kolmafia.*\\/([^\\$]*))\\.class"
 
 
-def latest_revision() -> str:
-    with urllib.request.urlopen(GITHUB_RELEASE_URL + "latest") as response:
-        data = json.loads(response.read().decode())
-        return data["name"]
-
-
-def download_kolmafia(revision: str, location: str):
+def download_kolmafia(revision: int, location: str):
     jar_url = GITHUB_DOWNLOAD_URL + f"r{revision}/KoLmafia-{revision}.jar"
     urllib.request.urlretrieve(jar_url, filename=location)
 
 
 class KoLmafia:
-    def __init__(self, revision: str):
-        revision = latest_revision() if revision == "latest" else revision
+    def __init__(self, revision: int):
         location = f"KoLmafia-{revision}.jar"
 
         if not os.path.isfile(location):
             download_kolmafia(revision, location)
 
         jpype.startJVM(classpath=location, convertStrings=True)
         patch.apply()
@@ -47,8 +39,8 @@
 
     def __getattr__(self, name: str) -> Any:
         if name in self.classes:
             return jpype.JClass(self.classes[name])
         return super().__getattribute__(name)
 
 
-km = KoLmafia(os.environ.get("KOLMAFIA_REVISION", "27335"))
+km = KoLmafia(pymafia_config.revision)
```

### Comparing `pymafia-0.2.1/src/pymafia/kolmafia/patch.py` & `pymafia-0.2.2/src/pymafia/kolmafia/patch.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/player.py` & `pymafia-0.2.2/src/pymafia/player.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/preference.py` & `pymafia-0.2.2/src/pymafia/preference.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.1/src/pymafia/utils.py` & `pymafia-0.2.2/src/pymafia/utils.py`

 * *Files identical despite different names*

