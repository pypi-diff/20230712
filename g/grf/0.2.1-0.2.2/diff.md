# Comparing `tmp/grf-0.2.1.tar.gz` & `tmp/grf-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grf-0.2.1.tar", last modified: Wed Feb  1 23:17:47 2023, max compression
+gzip compressed data, was "grf-0.2.2.tar", last modified: Tue Jul 11 22:50:11 2023, max compression
```

## Comparing `grf-0.2.1.tar` & `grf-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxrwxr-x   0 dp        (1000) dp        (1000)        0 2023-02-01 23:17:47.492176 grf-0.2.1/
--rw-r--r--   0 dp        (1000) dp        (1000)    35149 2023-02-01 18:45:53.000000 grf-0.2.1/LICENSE
--rw-rw-r--   0 dp        (1000) dp        (1000)      156 2023-02-01 23:17:47.492176 grf-0.2.1/PKG-INFO
--rw-r--r--   0 dp        (1000) dp        (1000)     3070 2023-02-01 18:45:53.000000 grf-0.2.1/README.md
-drwxrwxr-x   0 dp        (1000) dp        (1000)        0 2023-02-01 23:17:47.492176 grf-0.2.1/grf/
--rw-rw-r--   0 dp        (1000) dp        (1000)      604 2023-02-01 19:10:22.000000 grf-0.2.1/grf/__init__.py
--rw-rw-r--   0 dp        (1000) dp        (1000)    79235 2023-02-01 19:05:55.000000 grf-0.2.1/grf/actions.py
--rw-r--r--   0 dp        (1000) dp        (1000)    13076 2023-02-01 18:45:53.000000 grf-0.2.1/grf/common.py
--rw-rw-r--   0 dp        (1000) dp        (1000)       38 2023-02-01 19:10:28.000000 grf-0.2.1/grf/constants.py
--rwxr-xr-x   0 dp        (1000) dp        (1000)    59628 2023-02-01 18:45:53.000000 grf-0.2.1/grf/decompile.py
--rw-rw-r--   0 dp        (1000) dp        (1000)    23459 2023-02-01 18:45:53.000000 grf-0.2.1/grf/grf.py
--rw-rw-r--   0 dp        (1000) dp        (1000)    26449 2023-02-01 18:45:53.000000 grf-0.2.1/grf/lib.py
--rw-r--r--   0 dp        (1000) dp        (1000)    20614 2023-02-01 18:45:53.000000 grf-0.2.1/grf/parser.py
--rw-r--r--   0 dp        (1000) dp        (1000)    11396 2023-02-01 18:45:53.000000 grf-0.2.1/grf/parsetab.py
--rw-r--r--   0 dp        (1000) dp        (1000)    13838 2023-02-01 21:19:31.000000 grf-0.2.1/grf/sprites.py
--rw-r--r--   0 dp        (1000) dp        (1000)     5818 2023-02-01 18:45:53.000000 grf-0.2.1/grf/strings.py
--rw-r--r--   0 dp        (1000) dp        (1000)    20258 2023-02-01 18:45:53.000000 grf-0.2.1/grf/va2vars.py
--rw-r--r--   0 dp        (1000) dp        (1000)     7485 2023-02-01 18:45:53.000000 grf-0.2.1/grf/vox.py
-drwxrwxr-x   0 dp        (1000) dp        (1000)        0 2023-02-01 23:17:47.492176 grf-0.2.1/grf.egg-info/
--rw-r--r--   0 dp        (1000) dp        (1000)      156 2023-02-01 23:17:47.000000 grf-0.2.1/grf.egg-info/PKG-INFO
--rw-r--r--   0 dp        (1000) dp        (1000)      402 2023-02-01 23:17:47.000000 grf-0.2.1/grf.egg-info/SOURCES.txt
--rw-r--r--   0 dp        (1000) dp        (1000)        1 2023-02-01 23:17:47.000000 grf-0.2.1/grf.egg-info/dependency_links.txt
--rw-rw-r--   0 dp        (1000) dp        (1000)       47 2023-02-01 23:17:47.000000 grf-0.2.1/grf.egg-info/entry_points.txt
--rw-r--r--   0 dp        (1000) dp        (1000)       55 2023-02-01 23:17:47.000000 grf-0.2.1/grf.egg-info/requires.txt
--rw-r--r--   0 dp        (1000) dp        (1000)        4 2023-02-01 23:17:47.000000 grf-0.2.1/grf.egg-info/top_level.txt
--rw-r--r--   0 dp        (1000) dp        (1000)       85 2023-02-01 18:45:53.000000 grf-0.2.1/pyproject.toml
--rw-r--r--   0 dp        (1000) dp        (1000)      103 2023-02-01 23:17:47.492176 grf-0.2.1/setup.cfg
--rw-r--r--   0 dp        (1000) dp        (1000)      523 2023-02-01 22:42:15.000000 grf-0.2.1/setup.py
+drwxrwxr-x   0 dp        (1000) dp        (1000)        0 2023-07-11 22:50:11.090004 grf-0.2.2/
+-rw-rw-r--   0 dp        (1000) dp        (1000)    18002 2023-06-24 08:11:42.000000 grf-0.2.2/LICENSE
+-rw-rw-r--   0 dp        (1000) dp        (1000)      156 2023-07-11 22:50:11.090004 grf-0.2.2/PKG-INFO
+-rw-rw-r--   0 dp        (1000) dp        (1000)     3071 2023-06-24 08:11:42.000000 grf-0.2.2/README.md
+drwxrwxr-x   0 dp        (1000) dp        (1000)        0 2023-07-11 22:50:11.086004 grf-0.2.2/grf/
+-rw-rw-r--   0 dp        (1000) dp        (1000)      698 2023-06-25 15:14:08.000000 grf-0.2.2/grf/__init__.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)    84307 2023-07-11 20:04:43.000000 grf-0.2.2/grf/actions.py
+-rw-r--r--   0 dp        (1000) dp        (1000)    13521 2023-07-07 20:59:43.000000 grf-0.2.2/grf/common.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)      831 2023-06-24 08:11:42.000000 grf-0.2.2/grf/constants.py
+-rwxrwxr-x   0 dp        (1000) dp        (1000)    59636 2023-06-24 08:11:42.000000 grf-0.2.2/grf/decompile.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)    26860 2023-07-07 21:59:20.000000 grf-0.2.2/grf/grf.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)    45781 2023-07-11 19:34:25.000000 grf-0.2.2/grf/lib.py
+-rw-r--r--   0 dp        (1000) dp        (1000)    20766 2023-07-07 13:47:59.000000 grf-0.2.2/grf/parser.py
+-rw-r--r--   0 dp        (1000) dp        (1000)    11857 2023-07-04 23:04:57.000000 grf-0.2.2/grf/parsetab.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)    14723 2023-07-05 16:08:59.000000 grf-0.2.2/grf/sprites.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)     6035 2023-06-24 08:11:42.000000 grf-0.2.2/grf/strings.py
+-rw-r--r--   0 dp        (1000) dp        (1000)    20258 2023-02-01 18:45:53.000000 grf-0.2.2/grf/va2vars.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)    16054 2023-06-24 08:11:42.000000 grf-0.2.2/grf/vox.py
+drwxrwxr-x   0 dp        (1000) dp        (1000)        0 2023-07-11 22:50:11.086004 grf-0.2.2/grf.egg-info/
+-rw-r--r--   0 dp        (1000) dp        (1000)      156 2023-07-11 22:50:11.000000 grf-0.2.2/grf.egg-info/PKG-INFO
+-rw-r--r--   0 dp        (1000) dp        (1000)      579 2023-07-11 22:50:11.000000 grf-0.2.2/grf.egg-info/SOURCES.txt
+-rw-r--r--   0 dp        (1000) dp        (1000)        1 2023-07-11 22:50:11.000000 grf-0.2.2/grf.egg-info/dependency_links.txt
+-rw-rw-r--   0 dp        (1000) dp        (1000)       47 2023-07-11 22:50:11.000000 grf-0.2.2/grf.egg-info/entry_points.txt
+-rw-r--r--   0 dp        (1000) dp        (1000)       65 2023-07-11 22:50:11.000000 grf-0.2.2/grf.egg-info/requires.txt
+-rw-r--r--   0 dp        (1000) dp        (1000)        4 2023-07-11 22:50:11.000000 grf-0.2.2/grf.egg-info/top_level.txt
+-rw-r--r--   0 dp        (1000) dp        (1000)       85 2023-06-19 19:17:46.000000 grf-0.2.2/pyproject.toml
+-rw-r--r--   0 dp        (1000) dp        (1000)      103 2023-07-11 22:50:11.090004 grf-0.2.2/setup.cfg
+-rw-rw-r--   0 dp        (1000) dp        (1000)      742 2023-07-07 14:25:20.000000 grf-0.2.2/setup.py
+drwxrwxr-x   0 dp        (1000) dp        (1000)        0 2023-07-11 22:50:11.086004 grf-0.2.2/tests/
+-rw-rw-r--   0 dp        (1000) dp        (1000)     1809 2023-07-02 16:37:55.000000 grf-0.2.2/tests/test_action0.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)     1225 2023-07-04 23:11:32.000000 grf-0.2.2/tests/test_action2.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)     3916 2023-07-07 18:21:39.000000 grf-0.2.2/tests/test_lib_purchase_order.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)     3011 2023-07-09 19:58:29.000000 grf-0.2.2/tests/test_lib_rv_properties_cb.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)     3191 2023-07-07 18:24:01.000000 grf-0.2.2/tests/test_lib_train_properties_cb.py
+-rw-rw-r--   0 dp        (1000) dp        (1000)       31 2023-07-02 14:40:42.000000 grf-0.2.2/tests/test_newgrf_class.py
```

### Comparing `grf-0.2.1/README.md` & `grf-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
 pip install --upgrade pip
 pip install --upgrade setuptools
 python setup.py install
 ```
 
 # Licensing
 
-Currently grf-py is licensed under GPL v3 which basically means any GRF you make with it should be licensed under GPL as well. In part this is due to it importing nml library which is also licensed under GPL. But I do plan to change the lincense to more permissive in future and allow importing grf-py in closed source projects as well. So if you need a more permissive license or have some other suggestions feel free to contact me (dP) via issues or discord.
+Currently grf-py is licensed under GPL v2+ which basically means any GRF you make with it should be licensed under GPL as well. In part this is due to it importing nml library which is also licensed under GPL. But I do plan to change the lincense to more permissive in future and allow importing grf-py in closed source projects as well. So if you need a more permissive license or have some other suggestions feel free to contact me (dP) via issues or discord.
 
 This also means that if you plan to make any contributions to grf-py please explicitly license them under some non-restrictive license so I won't have to undo them later when I decide to change the license. Preferably use public domain or CC-0, but BSD or MIT should also be fine.
```

### Comparing `grf-0.2.1/grf/actions.py` & `grf-0.2.2/grf/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import textwrap
 import struct
 import pprint
 from collections.abc import Iterable
 
-from .common import Feature, hex_str, utoi32, VEHICLE_FEATURES, date_to_days, ANY_LANGUAGE, DataReader, to_bytes, read_dword, days_to_date
+from .common import Feature, hex_str, utoi32, VEHICLE_FEATURES, date_to_days, ANY_LANGUAGE, \
+                    DataReader, to_bytes, read_dword, read_word, days_to_date, read_extended_byte, encode_extended_byte
 from .common import TRAIN, RV, SHIP, AIRCRAFT, STATION, RIVER, CANAL, BRIDGE, HOUSE, GLOBAL_VAR, \
                     INDUSTRY_TILE, INDUSTRY, CARGO, SOUND_EFFECT, AIRPORT, SIGNAL, OBJECT, RAILTYPE, \
                     AIRPORT_TILE, ROADTYPE, TRAMTYPE, NO_CLIMATE, ALL_CLIMATES, TEMPERATE, ARCTIC, TROPICAL, TOYLAND
 
 from .parser import Node, Expr, Value, Var, Temp, Perm, Call, parse_code, OP_INIT, SPRITE_FLAGS
 from .sprites import BaseSprite, LazyBaseSprite, SoundSprite, IntermediateSprite
 
@@ -25,14 +26,47 @@
         return f'Ref({self.ref_id})'
 
     __repr__ = __str__
 
     def __int__(self):
         return self.value
 
+    def __eq__(self, ref):
+        return (
+            isinstance(ref, Ref) and
+            self.value == ref.value and
+            self.is_callback == ref.is_callback and
+            self.ref_id == ref.ref_id
+        )
+
+
+def get_ref_id(ref_obj):
+    if isinstance(ref_obj, Ref):
+        return ref_obj.value
+    if isinstance(ref_obj, int):
+        return ref_obj | 0x8000
+    if isinstance(ref_obj, SoundSprite):
+        return ref_obj.id | 0x8000
+    return ref_obj.ref_id
+
+
+def ref_eq(a, b):
+    return get_ref_id(a) == get_ref_id(b)
+
+
+def ref_dict_eq(a, b):
+    if len(a) != len(b):
+        return False
+    for k, v in a.items():
+        if k not in b:
+            return False
+        if get_ref_id(v) != get_ref_id(b[k]):
+            return False
+    return True
+
 
 class CB(Ref):
     def __init__(self, value):
         super().__init__(value | 0x8000)
 
 
 class Range:
@@ -45,14 +79,22 @@
         if self.low == self.high:
             return f'{self.low} -> {self.ref}'
         return f'{self.low}..{self.high} -> {self.ref}'
 
     def __repr__(self):
         return f'Range({self.low}, {self.high}, {self.ref})'
 
+    def __eq__(self, r):
+        return (
+            isinstance(r, Range) and
+            get_ref_id(self.ref) == get_ref_id(r.ref) and
+            self.low == r.low and
+            self.high == r.high
+        )
+
 
 def _py_dict(data, key_func, value_func, indent=12):
     indent_str = ' ' * indent
     res = ''
     it = data.items() if isinstance(data, dict) else data
     for k, v in it:
         kstr = key_func(k)
@@ -99,24 +141,14 @@
 
     def _format_ref(self, context, ref):
         if isinstance(ref, ReferenceableAction):
             return ref.py_ref()
         return repr(ref)
 
 
-def get_ref_id(ref_obj):
-    if isinstance(ref_obj, Ref):
-        return ref_obj.value
-    if isinstance(ref_obj, int):
-        return ref_obj | 0x8000
-    if isinstance(ref_obj, SoundSprite):
-        return ref_obj.id | 0x8000
-    return ref_obj.ref_id
-
-
 class SpriteRef:
     def __init__(self, id, pal=0, is_global=True, use_recolour=False, always_transparent=False, no_transparent=False):
         assert id <= 0x3fff, id
         assert pal <= 0x3fff, pal
         self.id = id
         self.pal = pal
         self.is_global = is_global
@@ -180,14 +212,45 @@
 
     def encode(cls, value):
         if isinstance(value, datetime.date):
             value = date_to_days(value)
         return struct.pack('<I', value)
 
 
+class IDProperty(Property):
+    def __init__(self, *, extended=False):
+        self.extended = extended
+
+    def _resolve(self, value):
+        if isinstance(value, int):
+            return value
+        if hasattr(value, 'id'):
+            return value.id
+        return None
+
+    def validate(self, value):
+        value = self._resolve(value)
+        if not isinstance(value, int):
+            raise ValueError(f'int or object with id expected')
+
+    def read(self, data, ofs):
+        if self.extended:
+            value, ofs = read_extended_byte(data, ofs)
+        else:
+            value, ofs = read_word(data, ofs)
+        return value, ofs
+
+    def encode(self, value):
+        value = self._resolve(value)
+        if self.extended:
+            return encode_extended_byte(value)
+        else:
+            return struct.pack('<H', value)
+
+
 class ClimateProperty(Property):
     def validate(cls, value):
         if not (0 <= value <= ALL_CLIMATES):
             raise ValueError(f'Expected value between NO_CLIMATE(0) and ALL_CLIMATES({ALL_CLIMATES})')
 
     def read(cls, data, ofs):
         return data[ofs], ofs + 1
@@ -249,44 +312,45 @@
     0x05: ('track_type', 'B'),  # Track type (see below)  should be same as front
     0x08: ('ai_special_flag', 'B'),  # AI special flag: set to 1 if engine is 'optimized' for passenger service (AI won't use it for other cargo), 0 otherwise     no
     0x09: ('max_speed', 'W'),  # Speed in mph*1.6 (see below)    no
     0x0B: ('power', 'W'),  # Power (0 for wagons)    should be zero
     0x0D: ('running_cost_factor', 'B'),  # Running cost factor (0 for wagons)  should be zero
     0x0E: ('running_cost_base', 'D'),  # Running cost base, see below    should be zero
     0x12: ('sprite_id', 'B'),  # Sprite ID (FD for new graphics)     yes
-    0x13: ('is_dual_headed', 'B'),  # Dual-headed flag; 1 if dual-headed engine, 0 otherwise  should be zero also for front
+    0x13: ('dual_headed', 'B'),  # Dual-headed flag; 1 if dual-headed engine, 0 otherwise  should be zero also for front
     0x14: ('cargo_capacity', 'B'),  # Cargo capacity  yes
     0x15: ('default_cargo_type', 'B'),  # Cargo type, see CargoTypes
-    0x16: ('weight', 'B'),  # Weight in tons  should be zero
+    0x16: ('weight_low', 'B'),  # Weight in tons  should be zero
     0x17: ('cost_factor', 'B'),  # Cost factor     should be zero
     0x18: ('ai_engine_rank', 'B'),  # Engine rank for the AI (AI selects the highest-rank engine of those it can buy)     no
     0x19: ('engine_class', 'B'),  # Engine traction type (see below)    no
-    0x1A: ('sort_purchase_list', 'B*'), # Not a property, but an action: sort the purchase list.  no
+    0x1A: ('sort_purchase_list', IDProperty(extended=True)), # Not a property, but an action: sort the purchase list.  no
     0x1B: ('extra_power_per_wagon', 'W'),  # Power added by each wagon connected to this engine, see below   should be zero
     0x1C: ('refit_cost', 'B'),  # Refit cost, using 50% of the purchase price cost base   yes
     0x1D: ('refittable_cargo_types', 'D'),  # Bit mask of cargo types available for refitting, see column 2 (bit value) in CargoTypes     yes
     0x1E: ('cb_flags', 'B'),  # Callback flags bit mask, see below  yes
     0x1F: ('tractive_effort_coefficient', 'B'),  # Coefficient of tractive effort  should be zero
     0x20: ('air_drag_coefficient', 'B'),  # Coefficient of air drag     should be zero
     0x21: ('shorten_by', 'B'),  # Make vehicle shorter by this amount, see below  yes
     0x22: ('visual_effect_and_powered', 'B'),  # Set visual effect type (steam/smoke/sparks) as well as position, see below  yes
-    0x23: ('extra_weight_per_wagon_low', 'B'),  # Set how much weight is added by making wagons powered (i.e. weight of engine), see below    should be zero
-    0x24: ('extra_weight_per_wagon_high', 'B'),  # High byte of vehicle weight, weight will be prop.24*256+prop.16     should be zero
+    0x23: ('extra_weight_per_wagon', 'B'),  # Set how much weight is added by making wagons powered (i.e. weight of engine), see below    should be zero
+    0x24: ('weight_high', 'B'),  # High byte of vehicle weight, weight will be prop.24*256+prop.16     should be zero
     0x25: ('bitmask_vehicle_info', 'B'),  # User-defined bit mask to set when checking veh. var. 42     yes
     0x26: ('retire_early', 'b'),  # Retire vehicle early, this many years before the end of phase 2 (see Action0General)    no
     0x27: ('misc_flags', 'B'),  # Miscellaneous flags     partly
     0x28: ('refittable_cargo_classes', 'W'),  # Refittable cargo classes    yes
     0x29: ('non_refittable_cargo_classes', 'W'),  # Non-refittable cargo classes    yes
     0x2A: ('introduction_date', DateProperty()),  # Long format introduction date   no
     0x2B: ('cargo_age_period', 'W'),  # period  yes
     0x2C: ('cargo_allow_refit', 'n*B'), # refittable cargo types   yes
     0x2D: ('cargo_disallow_refit', 'n*B'),  # refittable cargo types    yes
     0x2E: ('curve_speed_mod', 'W'),  # speed modifier    yes
-    0x2F: ('variant_group', 'W'),  # Vehicle variant group
+    0x2F: ('variant_group', IDProperty()),  # Vehicle variant group
     0x30: ('extra_flags', 'D'),  # extra flags
+    0x31: ('extra_cb_flags', 'B'),  # extra callback flags
 }
 
 ACTION0_RV_PROPS = {
     **ACTION0_COMMON_VEHICLE_PROPS,
     0x05: ('road_type', 'B'),  # Roadtype / tramtype (see below)     should be same as front
     0x08: ('precise_max_speed', 'B'),  # Speed in mph*3.2    no
     0x09: ('running_cost_factor', 'B'),  # Running cost factor     should be zero
@@ -305,51 +369,53 @@
     0x19: ('air_drag_coefficient', 'B'),  # Coefficient of air drag     should be zero
     0x1A: ('refit_cost', 'B'),  # Refit cost, using 25% of the purchase price cost base   yes
     0x1B: ('retire_early', 'b'),  # Retire vehicle early, this many years before the end of phase 2 (see Action0General)    no
     0x1C: ('misc_flags', 'B'),  # Miscellaneous vehicle flags     partly ("tram" should be same as front)
     0x1D: ('refittable_cargo_classes', 'W'),  # Refittable cargo classes, see train prop. 28    yes
     0x1E: ('non_refittable_cargo_classes', 'W'),  # Non-refittable cargo classes, see train prop. 29    yes
     0x1F: ('introduction_date', DateProperty()),  # Long format introduction date   no
-    0x20: ('sort_purchase_list', 'B*'), # Sort the purchase list  no
+    0x20: ('sort_purchase_list', IDProperty(extended=True)), # Sort the purchase list  no
     0x21: ('visual_effect', 'B'),  # Visual effect   yes
     0x22: ('cargo_age_period', 'W'),  # Custom cargo ageing period  yes
     0x23: ('shorten_by', 'B'),  # Make vehicle shorter, see train property 21     yes
-    0x24: ('cargo_allow_refit', 'B n*B'),  # List of always refittable cargo types, see train property 2C    yes
-    0x25: ('cargo_disallow_refit', 'B n*B'),  # List of never refittable cargo types, see train property 2D     yes
-    0x26: ('variant_group', 'W'),  # Vehicle variant group
+    0x24: ('cargo_allow_refit', 'n*B'),  # List of always refittable cargo types, see train property 2C    yes
+    0x25: ('cargo_disallow_refit', 'n*B'),  # List of never refittable cargo types, see train property 2D     yes
+    0x26: ('variant_group', IDProperty()),  # Vehicle variant group
     0x27: ('extra_flags', 'D'),  # extra flags
+    0x28: ('extra_cb_flags', 'B'),  # extra callback flags
 }
 
 ACTION0_SHIP_PROPS = {
     **ACTION0_COMMON_VEHICLE_PROPS,
     0x08: ('sprite_id', 'B'),  # Sprite (FF for new graphics)
     0x09: ('is_refittable', 'B'),  # Refittable (0 no, 1 yes)
     0x0A: ('cost_factor', 'B'),  # Cost factor
-    0x0B: ('speed', 'B'),  # Speed in mph*3.2
-    0x0C: ('cargo_type', 'B'),  # Cargo type, see CargoTypes
-    0x0D: ('capacity', 'W'),  # Capacity
+    0x0B: ('max_speed', 'B'),  # Speed in mph*3.2
+    0x0C: ('default_cargo_type', 'B'),  # Cargo type, see CargoTypes
+    0x0D: ('cargo_capacity', 'W'),  # Capacity
     0x0F: ('running_cost_factor', 'B'),  # Running cost factor
-    0x10: ('sound', 'B'),  # Sound effect type (4=cargo ship, 5=passenger ship)
+    0x10: ('sound_effect', 'B'),  # Sound effect type (4=cargo ship, 5=passenger ship)
     0x11: ('refittable_cargo_types', 'D'),  # v≥1     Bit mask of cargo types available for refitting, see column 2 (bit values) in CargoTypes
     0x12: ('cb_flags', 'B'),  # Callback flags bit mask, see below
     0x13: ('refit_cost', 'B'),  #  Refit cost, using 1/32 of the default refit cost base
-    0x14: ('ocean_speed', 'B'),  # Ocean speed fraction, sets fraction of top speed available in the ocean; e.g. 00=100%, 80=50%, FF=0.4%
-    0x15: ('canal_speed', 'B'),  # Canal speed fraction, same as above but for canals and rivers
+    0x14: ('ocean_speed_fraction', 'B'),  # Ocean speed fraction, sets fraction of top speed available in the ocean; e.g. 00=100%, 80=50%, FF=0.4%
+    0x15: ('canal_speed_fraction', 'B'),  # Canal speed fraction, same as above but for canals and rivers
     0x16: ('retire_early', 'b'),  # Retire vehicle early, this many years before the end of phase 2 (see Action0General)
-    0x17: ('flags', 'B'),  # Miscellaneous vehicle flags
-    0x18: ('refit_classes', 'W'),  # Refittable cargo classes, see train prop. 28
-    0x19: ('non_refit_classes', 'W'),  # Non-refittable cargo classes, see train prop. 29
+    0x17: ('misc_flags', 'B'),  # Miscellaneous vehicle flags
+    0x18: ('refittable_cargo_classes', 'W'),  # Refittable cargo classes, see train prop. 28
+    0x19: ('non_refittable_cargo_classes', 'W'),  # Non-refittable cargo classes, see train prop. 29
     0x1A: ('introduction_date', DateProperty()),  # Long format introduction date
-    0x1B: ('sort_purchase_list', 'B*'), # Sort the purchase list
+    0x1B: ('sort_purchase_list', IDProperty(extended=True)), # Sort the purchase list
     0x1C: ('visual_effect', 'B'),  # Visual effect
     0x1D: ('cargo_age_period', 'W'),  # Custom cargo ageing period
-    0x1E: ('cargo_allow_refit', 'B n*B'),  # List of always refittable cargo types, see train property 2C
-    0x1F: ('cargo_disallow_refit', 'B n*B'),  # List of never refittable cargo types, see train property 2D
-    0x20: ('variant_group', 'W'),  # Vehicle variant group
+    0x1E: ('cargo_allow_refit', 'n*B'),  # List of always refittable cargo types, see train property 2C
+    0x1F: ('cargo_disallow_refit', 'n*B'),  # List of never refittable cargo types, see train property 2D
+    0x20: ('variant_group', IDProperty()),  # Vehicle variant group
     0x21: ('extra_flags', 'D'),  # extra flags
+    0x22: ('extra_cb_flags', 'B'),  # extra callback flags
 }
 
 ACTION0_AIRCRAFT_PROPS = {
     **ACTION0_COMMON_VEHICLE_PROPS,
     0x08: ('sprite_id', 'B'),  # Sprite (FF for new graphics)
     0x09: ('is_helicopter', 'B'),  # Is helicopter? 2=no, 0=yes
     0x0A: ('is_large', 'B'),  # Is large? 0=no, 1=yes (i.e. can't safely land on small airports)
@@ -364,21 +430,22 @@
     0x14: ('cb_flags', 'B'),  # Callback flags bit mask, see below
     0x15: ('refit_cost', 'B'),  # Refit cost, using 1/32 of the default refit cost base
     0x16: ('retire_early', 'b'),  # Retire vehicle early, this many years before the end of phase 2 (see Action0General)
     0x17: ('misc_flags', 'B'),  # Miscellaneous vehicle flags
     0x18: ('refittable_cargo_classes', 'W'),  # Refittable cargo classes, see train prop. 28
     0x19: ('non_refittable_cargo_classes', 'W'),  # Non-refittable cargo classes, see train prop. 29
     0x1A: ('introduction_date', DateProperty()),  # Long format introduction date
-    0x1B: ('sort_purchase_list', 'B*'),  # Sort the purchase list
+    0x1B: ('sort_purchase_list', IDProperty(extended=True)),  # Sort the purchase list
     0x1C: ('cargo_age_period', 'W'),  # Custom cargo ageing period
-    0x1D: ('cargo_allow_refit', 'B n*B'),  # List of always refittable cargo types, see train property 2C
-    0x1E: ('cargo_disallow_refit', 'B n*B'),  # List of never refittable cargo types, see train property 2D
+    0x1D: ('cargo_allow_refit', 'n*B'),  # List of always refittable cargo types, see train property 2C
+    0x1E: ('cargo_disallow_refit', 'n*B'),  # List of never refittable cargo types, see train property 2D
     0x1F: ('range', 'W'),  # Aircraft range in tiles. Distance is euclidean, a value of 0 means range is unlimited
-    0x20: ('variant_group', 'W'),  # Vehicle variant group
+    0x20: ('variant_group', IDProperty()),  # Vehicle variant group
     0x21: ('extra_flags', 'D'),  # extra flags
+    0x22: ('extra_cb_flags', 'B'),  # extra callback flags
 }
 
 
 class BaseSpriteData:
     def __init__(self, sprite, *, flags=None, registers=None):
         assert isinstance(sprite, SpriteRef)
         self.sprite = sprite
@@ -905,16 +972,36 @@
     0x14: ('speed_limit', 'W'),  # Speed limit
     0x15: ('acceleration_model', 'B'),  # Acceleration model
     0x18: ('requires_railtype_list', 'n*L'),  # Introduction required rail type list[2]
     0x19: ('introduces_railtype_list', 'n*L'),  # Introduced rail type list[2]
     0x1D: ('alternative_railtype_list', 'n*L'),  # Alternate rail type labels that shall be "redirected" to this rail type
 }
 
+ACTION0_ROADTYPE_PROPS = {
+    0x08: ('label', 'L'),  # Road type label
+    0x09: ('toolbar_caption', 'W'),  # StringID: Build road toolbar caption
+    0x0A: ('menu_text', 'W'),  # StringID: Road construction dropdown text
+    0x0B: ('build_window_caption', 'W'),  # StringID: Build vehicle window caption
+    0x0C: ('autoreplace_text', 'W'),  # StringID: Autoreplace text
+    0x0D: ('new_engine_text', 'W'),  # StringID: New engine text
+    0x0F: ('powered_roadtype_list', 'n*L'),  # Powered road type list[1]
+    0x10: ('roadtype_flags', 'B'),  # Road type flags
+    0x13: ('construction_cost', 'W'),  # Construction costs
+    0x14: ('speed_limit', 'W'),  # Speed limit
+    0x16: ('map_colour', 'B'),  # Minimap colour
+    0x17: ('introduction_date', DateProperty()), # Introduction date
+    0x18: ('requires_roadtype_list', 'n*L'),  # Introduction required road type list[1]
+    0x19: ('introduces_roadtype_list', 'n*L'),  # Introduced road type list[1]
+    0x1A: ('sort_order', 'B'),  # Sort order
+    0x1B: ('name', 'W'),  # StringID: Road type name
+    0x1C: ('maintenance_cost', 'W'),  # Infrastructure maintenance cost factor
+    0x1D: ('alternative_roadtype_list', 'n*L'),  # Alternate road type labels that shall be "redirected" to this road type
+}
+
 # TODO airport_tile
-# TODO road_type
 # TODO tram_type
 
 ACTION0_PROPS = {
     TRAIN: ACTION0_TRAIN_PROPS,
     RV: ACTION0_RV_PROPS,
     SHIP: ACTION0_SHIP_PROPS,
     AIRCRAFT: ACTION0_AIRCRAFT_PROPS,
@@ -924,14 +1011,15 @@
     GLOBAL_VAR: ACTION0_GLOBAL_PROPS,
     INDUSTRY_TILE: ACTION0_INDUSTRY_TILE_PROPS,
     INDUSTRY: ACTION0_INDUSTRY_PROPS,
     CARGO: ACTION0_CARGO_PROPS,
     SOUND_EFFECT: ACTION0_SOUND_EFFECT_PROPS,
     OBJECT: ACTION0_OBJECT_PROPS,
     RAILTYPE: ACTION0_RAILTYPE_PROPS,
+    ROADTYPE: ACTION0_ROADTYPE_PROPS,
 }
 
 ACTION0_PROP_DICT = {
     feature: {name: (id, size) for id, (name, size, *_) in fdict.items()}
     for feature, fdict in ACTION0_PROPS.items()
 }
 
@@ -949,34 +1037,60 @@
     RESERVED_1 = 0x4  # reserved, do not use
     RESERVED_2 = 0x8  # reserved, do not use
     AUTOREFIT = 0x10  # Auto-refitting is enabled for refits where callback 15E allows it or prop 1A specifies zero cost.
     USE_CARGO_MULT = 0x20  # Use cargo multiplier for default cargo. See page about vehicle refitting.
     NO_BREAKDOWN_SMOKE = 0x40  # Disable breakdown smoke effect.
     USE_SPRITE_STACK = 0x80  # Compose vehicle from multiple sprites.
 
+
 class TrainFlags:
     TILT = 0x1
     USE_2CC = 0x2
     MULTIPLE_UNIT = 0x4
     ALLOW_FLIPPING = 0x8
     AUTOREFIT = 0x10
     USE_CARGO_MULT = 0x20
     NO_BREAKDOWN_SMOKE = 0x40
     USE_SPRITE_STACK = 0x80
 
+class AIFlags:
+    CARGO = 0x00
+    PASSENGER = 0x01
+
+
+class TrainRunningCost:
+    STEAM = 0x4C30
+    DIESEL = 0x4C36
+    ELECTRIC = 0x4C3C
+    ROADVEH = 0x4C48
+    NONE = 0x0000
+
+
+class TrainVisualEffect:
+    DEFAULT = 0x00
+    STEAM = 0x10
+    DIESEL = 0x20
+    ELECTRIC = 0x30
+    DISABLE = 0x40
+
 
 def train_hpi(value):
     return value
 
+
 def train_ton(value):
     return value
 
+
 def nml_te(value):
     return int(float(value) * 255 + 0.5)
 
+def nml_drag(value):
+    return int(float(value) * 255 + 0.5)
+
 
 class CargoClass:
     PASSENGERS = 0x1  # passengers, also tourists (ECS)
     MAIL = 0x2  # mail
     EXPRESS = 0x4  # express goods, also tourists (ECS)
     ARMOURED = 0x8  # valuables, diamonds, gold and alike
     BULK = 0x10  # coal, ore, grain,...
@@ -1060,14 +1174,23 @@
             feature={self.feature},
             first_id={self.first_id},
             count={self.count},
             props={propstr}
         )
         '''
 
+    def __eq__(self, action):
+        return (
+            isinstance(action, DefineMultiple) and
+            self.feature == action.feature and
+            self.first_id == action.first_id and
+            self.count == action.count and
+            self.props == action.props
+        )
+
 
 class Define(DefineMultiple):
     def __init__(self, *, feature, id, props):
         multi_props = {k: [v] for k, v in props.items()}
         super().__init__(feature=feature, first_id=id, count=1, props=multi_props)
 
     @property
@@ -1244,15 +1367,15 @@
 class ExtendedSpriteLayout(AdvancedSpriteLayout):
     # Not implemented yet
     def __init__(self, *args, **kw):
         super().__init__(*args, has_flags=False, **kw)
 
 
 class Switch(LazyBaseSprite, ReferenceableAction, ReferencingAction):
-    def __init__(self, ranges, default, code, *, feature=None, ref_id=None, related_scope=False):
+    def __init__(self, code, ranges, default, *, feature=None, ref_id=None, related_scope=False):
         super().__init__()
         self.feature = feature
         self.ref_id = ref_id
         self.related_scope = related_scope
 
         self._ranges = []
         if isinstance(ranges, dict):
@@ -1335,14 +1458,25 @@
             feature={self.feature},{self._py_ref_id(context)}
             related_scope={self.related_scope},
             code={code_str},
             ranges={ranges_str},
             default={default_str},
         )'''
 
+    def __eq__(self, action):
+        return (
+            isinstance(action, Switch) and
+            self.feature == action.feature and
+            self.ref_id == action.ref_id and
+            self.related_scope == action.related_scope and
+            self.code == action.code and
+            self._ranges == action._ranges and
+            ref_eq(self.default, action.default)
+        )
+
 
 class RandomSwitch(LazyBaseSprite, ReferenceableAction, ReferencingAction):
     def __init__(self, *, scope, triggers, cmp_all, lowest_bit, groups, count=None, feature=None, ref_id=None):
         if scope == 'relative' and feature in VEHICLE_FEATURES:
             assert count is not None
         else:
             assert count is None
@@ -1486,14 +1620,24 @@
             feature={self.feature},
             wagon_override={self.wagon_override},
             ids={self.ids!r},
             maps={_py_ref_dict(self.maps, value_func)},
             default={self._format_ref(context, self.default)},
         )'''
 
+    def __eq__(self, action):
+        return (
+            isinstance(action, Action3) and
+            self.feature == action.feature and
+            self.ids == action.ids and
+            ref_dict_eq(self.maps, action.maps) and
+            ref_eq(self.default, action.default) and
+            self.wagon_override == action.wagon_override
+        )
+
 
 class Map(Action3):
     def __init__(self, definition, maps, default):
         assert isinstance(definition, DefineMultiple)
         super().__init__(
             feature=definition.feature,
             ids=[definition.first_id],
@@ -1559,14 +1703,23 @@
             feature={self.feature},
             lang={self.lang},
             offset={offset_str},
             is_generic_offset={self.is_generic_offset},
             strings=''' + pformat(self.strings, indent_first=0, indent=10 + 8) + '''
         )'''
 
+    def __eq__(self, action):
+        return (
+            isinstance(action, DefineStrings) and
+            self.feature == action.feature and
+            self.lang == action.lang and
+            self.offset == action.offset and
+            self.is_generic_offset == action.is_generic_offset and
+            self.strings == action.strings
+        )
 
 # Action 5
 
 class ReplaceNewSprites(LazyBaseSprite):
     def __init__(self, set_type, count, *, offset=None):
         assert isinstance(set_type, int)
         assert isinstance(count, int)
```

### Comparing `grf-0.2.1/grf/common.py` & `grf-0.2.2/grf/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,24 +159,35 @@
 
 class FeatureMeta(type):
     def __call__(cls, feature):
         return cls.FEATURES[feature]
 
 
 class Feature(metaclass=FeatureMeta):
+    _FROM_NAME = {}
+
     def __init__(self, id, name):
         self.id = id
         self.name = name
         self.constant = name.upper()
 
     def __repr__(self):
         return self.constant
 
+    @classmethod
+    def from_name(cls, name):
+        return cls._FROM_NAME[name]
+
+    @classmethod
+    def from_constant(cls, constant):
+        cls.from_name(constant.lower())
+
+
 
-FeatureMeta.FEATURES = [None] * 0x14
+FeatureMeta.FEATURES = [None] * 0x15
 for k, n in ((0x00, 'train'),
              (0x01, 'rv'),
              (0x02, 'ship'),
              (0x03, 'aircraft'),
              (0x04, 'station'),
              (0x05, 'canal'),
              (0x06, 'bridge'),
@@ -188,41 +199,52 @@
              (0x0c, 'sound_effect'),
              (0x0d, 'airport'),
              (0x0e, 'signal'),
              (0x0f, 'object'),
              (0x10, 'railtype'),
              (0x11, 'airport_tile'),
              (0x12, 'roadtype'),
-             (0x13, 'Tramtype'),
+             (0x13, 'tramtype'),
+             (0x14, 'road_stop'),
             ):
-    FeatureMeta.FEATURES[k] = type.__call__(Feature, k, n)
+    obj = type.__call__(Feature, k, n)
+    FeatureMeta.FEATURES[k] = obj
+    Feature._FROM_NAME[n] = obj
 
 TRAIN, RV, SHIP, AIRCRAFT, STATION, RIVER, BRIDGE, HOUSE, GLOBAL_VAR, INDUSTRY_TILE, INDUSTRY, CARGO, \
-SOUND_EFFECT, AIRPORT, SIGNAL, OBJECT, RAILTYPE, AIRPORT_TILE, ROADTYPE, TRAMTYPE = FeatureMeta.FEATURES
+SOUND_EFFECT, AIRPORT, SIGNAL, OBJECT, RAILTYPE, AIRPORT_TILE, ROADTYPE, TRAMTYPE, ROAD_STOP = FeatureMeta.FEATURES
 
 CANAL = RIVER
 
 VEHICLE_FEATURES = (TRAIN, RV, SHIP, AIRCRAFT)
 
 
 def read_extended_byte(data, offset):
     res = data[offset]
     if res != 0xff:
         return res, offset + 1
     return data[offset + 1] | (data[offset + 2] << 8), offset + 3
 
 
+def encode_extended_byte(value):
+    if value < 255:
+        return struct.pack('<B', value)
+    else:
+        return struct.pack('<BH', 255, value)
+
+
 def read_word(data, offset):
     return data[offset] | (data[offset + 1] << 8), offset + 2
 
 
 def read_dword(data, offset):
     return data[offset] | (data[offset + 1] << 8) | (data[offset + 2] << 16) | (data[offset + 3] << 24), offset + 4
 
 
+
 class DataReader:
     def __init__(self, data, offset=0):
         self.data = data
         self.offset = offset
 
     def get_byte(self):
         self.offset += 1
```

### Comparing `grf-0.2.1/grf/decompile.py` & `grf-0.2.2/grf/decompile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1088,18 +1088,18 @@
     if grf_type == 0xff:
         data = f.read(l)
         if l == 1:  # Some NewGRF files have "empty" pseudo-sprites which are 1 byte long.
             return True, [], None
         # print(f'{nfo_line}: Sprite({l}, {grf_type_str}) <{data[0]:02x}>: {hex_str(data, 100)}')
         context.count_action(data[0], l + size_bytes * 2 + 1)
         res.append(PyComment(f'{nfo_line}: Sprite({l}, {grf_type_str}) <{data[0]:02x}>: {hex_str(data, 100)}'))
-        if container == 1:
-            sprite = RealRemapSprite(context.get_v1_sprite_id(), data)
-            res.append(SpritePlaceholder(sprite.id))
-            return True, res, sprite
+        # if container == 1:
+        #     sprite = RealRemapSprite(context.get_v1_sprite_id(), data)
+        #     res.append(SpritePlaceholder(sprite.id))
+        #     return True, res, sprite
         try:
             res.extend(decode_pseudo_sprite(data, context))
         except Exception as e:
             res.append(PyComment(f'Error decoding sprite:'))
             estr = traceback.format_exc()
             for l in estr.split('\n'):
                 res.append(PyComment(l))
```

### Comparing `grf-0.2.1/grf/grf.py` & `grf-0.2.2/grf/grf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 import heapq
 import inspect
+import json
 import struct
 import time
 import textwrap
 from collections import defaultdict
 
 from PIL import Image, ImageDraw
 import nml.spriteencoder
@@ -16,15 +17,15 @@
                      IndustryProductionCallback, Action3, Map, DefineStrings, ReplaceNewSprites, \
                      ModifySprites, If, SetDescription, ReplaceOldSprites, ErrorMessage, Comment, \
                      ComputeParameters, Label, SoundEffects, ImportSound, Translations, SetProperties
 from .parser import Node, Expr, Value, Var, Temp, Perm, Call, parse_code, OP_INIT, SPRITE_FLAGS, GenericVar
 from .common import Feature, hex_str, utoi32, FeatureMeta, to_bytes, GLOBAL_VAR
 from .common import PALETTE
 from .sprites import BaseSprite, GraphicsSprite, SoundSprite, RealSprite, LazyBaseSprite, IntermediateSprite, \
-                     PaletteRemap
+                     PaletteRemap, AlternativeSprites
 from .strings import StringManager
 
 
 # def map_rgb_image(self, im):
 #     assert im.mode == 'RGB', im.mode
 #     data = np.array(im)
 
@@ -147,20 +148,27 @@
         print(f'   Graphics loading time: {self.loading_time:.02f}')
         print(f'   Graphics conversion time: {self.conversion_time:.02f}')
         print(f'   Graphics composing time: {self.composing_time:.02f}')
         print(f'   Graphics compression time: {self.compression_time:.02f}')
 
 
 class BaseNewGRF:
-    def __init__(self):
+    def __init__(self, *, id_map_file=None):
         self.generators = []
         self._next_sound_id = 73
         self._sounds = {}
         self.strings = StringManager()
         self._sprite_encoder = SpriteEncoder()
+        self._id_map = IDMap(id_map_file)
+
+    def reserve_ids(self, feature, ids):
+        self._id_map.reserve_ids(feature, ids)
+
+    def resolve_id(self, feature, value, *, articulated=False):
+        return self._id_map.resolve(feature, value, articulated=articulated)
 
     def _add_sound(self, s):
         assert isinstance(s, SoundSprite)
 
         if s.id is not None:
             return
 
@@ -174,35 +182,23 @@
             self._next_sound_id += 1
             self._sounds[h] = s
 
     def _add(self, l, *sprites):
         if not sprites:
             return
 
-        # Unfold real sprite tuple if it was passed as a single arg
-        if isinstance(sprites[0], (tuple, list)):
-            assert len(sprites) == 1
-            sprites = sprites[0]
-            assert len(sprites) >= 1
-            assert isinstance(sprites[0], GraphicsSprite), type(sprites[0])
+        # TODO assert all(isinstance(s, (BaseSprite, SpriteGenerator, PyComment)) for s in sprites), sprites
 
         if isinstance(sprites[0], RealSprite):
             if isinstance(sprites[0], SoundSprite):
                 for s in sprites:
                     self._add_sound(s)
                 return
-            elif isinstance(sprites[0], PaletteRemap):
-                l.append((sprites[0],))
-                return
-            assert(all(isinstance(s, GraphicsSprite) for s in sprites)), sprites
-            assert(len(set((s.zoom, s.bpp) for s in sprites)) == len(sprites)), sprites
 
-            l.append(tuple(sprites))
-        else:
-            l.extend(sprites)
+        l.extend(sprites)
 
     def add(self, *sprites):
         self._add(self.generators, *sprites)
 
     def _write_pseudo_sprite(self, f, data, grf_type=0xff):
         f.write(struct.pack('<IB', len(data), grf_type))
         f.write(data)
@@ -280,17 +276,18 @@
         def resolve(s, i):
             # Action can reference other actions, resolve all the references
             if isinstance(s, ReferencingAction):
                 for r in s.get_refs():
                     if isinstance(r, Ref):
                         if r.is_callback:
                             continue
-                        r = refids.get(r.ref_id)
-                        if r is None:
-                            raise RuntimeError(f'Unresolved direct reference {r} in action {s}')
+                        robj = refids.get(r.ref_id)
+                        if robj is None:
+                            raise RuntimeError(f'Unresolved direct reference {r} in action {s.py(None)}')
+                        r = robj
                         ref_count[id(r)] += 1
                         continue
 
                     if not isinstance(r, ReferenceableAction):
                         if isinstance(r, SoundSprite):
                             self._add_sound(r)
                         continue
@@ -411,91 +408,176 @@
 
         t.log(f'Resolving action references')
         sprites = self.resolve_refs(sprites)
 
         t.log(f'Adding sounds')
         if self._sounds:
             sprites.append(SoundEffects(len(self._sounds)))
-            for s in self._sounds.values():
-                sprites.append((s,))
+            sprites.extend(self._sounds.values())
 
         t.log(f'Adding strings')
         sprites.extend(self.strings.get_actions())
 
         t.log(f'Enumerating {len(sprites)} real sprites')
         data_offset = 14
         next_sprite_id = 1
         for s in sprites:
-            if isinstance(s, tuple):
-                for x in s:
-                    x.sprite_id = next_sprite_id
+            if isinstance(s, (AlternativeSprites, RealSprite)):
+                s.sprite_id = next_sprite_id
                 next_sprite_id += 1
-                s = s[0]
             data_offset += s.get_data_size() + 5
 
         with open(filename, 'wb') as f:
             t.log(f'Writing pseudo sprites')
             f.write(b'\x00\x00GRF\x82\x0d\x0a\x1a\x0a')  # file header
             f.write(struct.pack('<I', data_offset))
             f.write(b'\x00')  # compression(1)
             # f.write(b'\x04\x00\x00\x00')  # num(4)
             # f.write(b'\xFF')  # grf_type(1)
             # f.write(b'\xb0\x01\x00\x00')  # num + 0xff -> recoloursprites() (257 each)
             self._write_pseudo_sprite(f, b'\x02\x00\x00\x00')
 
             for s in sprites:
-                if isinstance(s, tuple):
-                    self._write_pseudo_sprite(f, s[0].get_data(), grf_type=0xfd)
+                if isinstance(s, (AlternativeSprites, RealSprite)):
+                    self._write_pseudo_sprite(f, s.get_data(), grf_type=0xfd)
                 else:
                     self._write_pseudo_sprite(f, s.get_data(), grf_type=0xff)
             f.write(b'\x00\x00\x00\x00')
 
             t.log(f'Writing real sprites')
             written_sprites = set()
             for sl in sprites:
-                if not isinstance(sl, tuple):
-                    continue
-                for s in sl:
-                    if s in written_sprites:
+                if isinstance(sl, RealSprite):
+                    if sl in written_sprites:
                         continue
-                    f.write(s.get_real_data(self._sprite_encoder))
-                    written_sprites.add(s)
+                    # print('data', sl.get_real_data(self._sprite_encoder), flush=True)
+                    f.write(sl.get_real_data(self._sprite_encoder))
+                    written_sprites.add(sl)
+                elif isinstance(sl, AlternativeSprites):
+                    for s in sl.sprites:
+                        if s in written_sprites:
+                            continue
+                        f.write(s.get_real_data(self._sprite_encoder))
+                        written_sprites.add(s)
 
             f.write(b'\x00\x00\x00\x00')
 
+        self._id_map.save()
         t.stop()
         self._sprite_encoder.print_time_report()
 
     def wrap(self, func):
         def wrapper(*args, **kw):
             obj = func(*args, **kw)
             self.add(obj)
             return obj
         return wrapper
 
     def bind(self, cls):
-
-        @functools.wraps(cls)
-        def wrapper(*args, **kw):
-            gen = cls(*args, **kw)
-            self.add(gen)
-            return gen
-
-        # Expose attributes on the wrapper
-        for name in dir(cls):
-            obj = getattr(cls, name)
-            if not name.startswith('__'):
-                setattr(wrapper, name, obj)
-
-        return wrapper
+        def constructor(obj_self, *args, **kw):
+            cls.__init__(obj_self, *args, **kw)
+            self.add(obj_self)
+
+        return type(
+            'Bound' + cls.__name__,
+            (cls,),
+            {
+                'bound_newgrf': self,
+                '__init__': constructor,
+            },
+        )
+
+
+class IDMap:
+    MIN_ID = 300
+
+    def __init__(self, path=None):
+        self.path = path
+        self._loaded = False
+        self._index = {}
+        self._next_id = {}
+        self._auto_ids = set()
+        self._manual_ids = set()
+
+    def _check_path(self):
+        if self.path is None:
+            self.path = 'id_map.json'
+            print(f'WARNING: ID index is not configured, using default "{self.path}"')
+            print('Set id index path by passing id_map_file to NewGRF constructor.')
+
+    def _load(self):
+        if self._loaded: return
+        self._check_path()
+
+        try:
+            data = json.load(open(self.path))
+        except FileNotFoundError:
+            # TODO link docs on how to create empty index
+            # Creating index automatically is dangerous as it may mask the error.
+            raise RuntimeError(f'ERROR: ID index file is not found in "{self.path}".')
+
+        assert data['version'] == 1
+
+        # Load into temporaries first in case of exception
+        index = {}
+        next_id = {}
+        used_ids = set()
+        for feature_name, feature_index in data['index'].items():
+            feature = Feature.from_name(feature_name)
+            for name, fid in feature_index.items():
+                key = (feature, name)
+                index[key] = fid
+                used_ids.add(key)
+                next_id[feature] = max(next_id.get(feature, 0), fid)
+        self._loaded = True
+        self._index = index
+        self._next_id = next_id
+        self._auto_ids = used_ids
+
+    def save(self):
+        self._check_path()
+        index = {}
+        for (feature, name), value in self._index.items():
+            index.setdefault(feature.name, {})[name] = value
+        data = {
+            'version': 1,
+            'index': index,
+        }
+        jdata = json.dumps(data, indent=4)
+        with open(self.path, 'w') as f:
+            f.write(jdata)
+
+    def reserve_ids(self, ids):
+        self._manual_ids.update(ids)
+
+    def resolve(self, feature, value, *, articulated=False):
+        self._load()
+        key = (feature, value)
+        if isinstance(value, int):
+            if key in self._auto_ids:
+                raise RuntimeError(f'ID {value} can''t be used for feature {feature!r} as it was previously auto-assigned.')
+            self._manual_ids.add(key)
+            return value
+
+        assert isinstance(value, str), type(value)
+        i = self._index.get(key)
+        # TODO use separate articulated range
+        if i is None:
+            i = self._next_id.get(feature, self.MIN_ID)
+            while (feature, i) in self._manual_ids:
+                i += 1
+            self._next_id[feature] = i + 1
+            self._index[key] = i
+            self._auto_ids.add((feature, i))
+        return i
 
 
 class NewGRF(BaseNewGRF):
-    def __init__(self, *, grfid, name, description, version=None, min_compatible_version=None, format_version=8, url=None):
-        super().__init__()
+    def __init__(self, *, grfid, name, description, version=None, min_compatible_version=None, format_version=8, url=None, id_map_file=None):
+        super().__init__(id_map_file=id_map_file)
 
         if isinstance(grfid, str):
             grfid = grfid.encode('utf-8')
 
         if len(grfid) != 4:
             raise ValueError(f'Expected 4 symbols for GRFID, found {len(grfid)}: {grfid}')
 
@@ -518,24 +600,42 @@
         self._cargo_table = None
         self._railtype_table = None
         self.grfid = grfid
         self.name = name
         self.description = description
         self.format_version = format_version
 
+    @property
+    def grfid_value(self):
+        return struct.unpack('<I', self.grfid)[0]
+
+    def add_railtype(self, *railtype_list):
+        if self._railtype_table is None:
+            self._railtype_table = {}
+
+        if railtype_list and isinstance(railtype_list[0], (tuple, list)):
+            railtype_list = railtype_list[0]
+
+        rt_id = len(self._railtype_table)
+
+        if isinstance(railtype_list, (list, tuple)):
+            rtb = to_bytes(railtype_list[0])
+            self._railtype_table[rtb] = (rt_id, tuple(map(to_bytes, railtype_list)))
+        else:
+            rtb = to_bytes(railtype_list)
+            self._railtype_table[rtb] = (rt_id, None)
+
+        return rt_id
+
     def set_railtype_table(self, railtype_list):
         self._railtype_table = {}
+        res = []
         for i, rt in enumerate(railtype_list):
-            if isinstance(rt, (list, tuple)):
-                rtb = to_bytes(rt[0])
-                self._railtype_table[rtb] = (i, tuple(map(to_bytes, rt)))
-            else:
-                rtb = to_bytes(rt)
-                self._railtype_table[rtb] = (i, None)
-        return tuple(range(len(self._railtype_table)))
+            res.append(self.add_railtype(rt))
+        return res
 
     def get_railtype_id(self, railtype):
         rtbytes = to_bytes(railtype)
         if rtbytes not in self._railtype_table:
             raise ValueError(f'Unknown railtype `{railtype}`')
         return self._railtype_table[rtbytes][0]
```

### Comparing `grf-0.2.1/grf/parser.py` & `grf-0.2.2/grf/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,22 @@
 
 def hex_str(s):
     if isinstance(s, (bytes, memoryview)):
         return ':'.join('{:02x}'.format(b) for b in s)
     return ':'.join('{:02x}'.format(ord(c)) for c in s)
 
 
+def get_constant(value, error):
+    if isinstance(value, int):
+        return value
+    if isinstance(value, Value):
+        return value.value
+    raise RuntimeError(error)
+
+
 class Node:
     def __init__(self):
         pass
 
     def _make_node(self, value):
         if isinstance(value, int):
             return Value(value)
@@ -292,33 +300,28 @@
     def compile(self, register, shift=0, and_mask=0xffffffff):
         and_mask &= self.and_mask >> shift
         shift += self.shift
         assert shift < 0x20, shift
         assert and_mask <= 0xffffffff, and_mask
         if self.param is not None:
             # TODO dynamic param (var 7B)
-            if not isinstance(self.param, int):
-                self.param = 0
-            return True, struct.pack('<BBBI', self.var, self.param, 0x20 | shift, and_mask)
+            param = get_constant(self.param, 'Parameter should be a constant')
+            return True, struct.pack('<BBBI', self.var, param, 0x20 | shift, and_mask)
         else:
             return True, struct.pack('<BBI', self.var, 0x20 | shift, and_mask)
 
 
 class Temp(Node):
     def __init__(self, register):
         assert isinstance(register, (int, Node)), type(register)
         super().__init__()
         self.register = register
 
     def get_index(self):
-        if isinstance(self.register, int):
-            return self.register
-        if isinstance(self.register, Value):
-            return self.register.value
-        raise RuntimeError('Register number should be a simple value, not expression')
+        return get_constant(self.register, 'Register number should be a simple value, not expression')
 
     def format(self, parent_priority=0):
         if isinstance(self.register, int):
             return  f'TEMP[0x{self.register:02x}]'
         return  f'TEMP[{self.register.format()}]'
 
     def compile(self, register, shift=0, and_mask=0xffffffff):
@@ -608,14 +611,15 @@
     assert op is not None, t[1]
     t[0] = Expr(op, t[3], t[5])
 
 
 def p_expression_call3(t):
     #                1     2      3     4      5     6         7     8     9     10   11      12   13    14      15     16  17   18      19     20
     '''expression : NAME LPAREN NUMBER COMMA NAME ASSIGN     NUMBER COMMA NAME ASSIGN NUMBER RPAREN
+                  | NAME LPAREN NUMBER COMMA NAME ASSIGN     NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN
                   | NAME LPAREN NUMBER COMMA NAME ASSIGN expression COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN
                   | NAME LPAREN NUMBER COMMA NAME ASSIGN     NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN
     '''
     assert t[1] == 'var'
     if len(t) > 17:
         assert t[5] == 'shift' and t[9] == 'and'
         assert t[13] == 'add'
```

### Comparing `grf-0.2.1/grf/parsetab.py` & `grf-0.2.2/grf/parsetab.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # parsetab.py
 # This file is automatically generated. Do not edit.
 # pylint: disable=W,C,R
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'leftLTGTLEGEEQNEQleftSHRUSHRSHLleftBINORleftBINXORleftBINANDleftADDSUBleftMULrightUMINUSADD ASSIGN BINAND BINOR BINXOR COMMA EQ GE GT LBRACKET LE LPAREN LT MUL NAME NEQ NEWLINE NUMBER RBRACKET RPAREN SHL SHR SHRU SUBlines : line\n             | expression\n             | lines line\n    line : expression NEWLINE\n            | NEWLINE\n    expression : expression ADD expression\n                  | expression SUB expression\n                  | expression MUL expression\n                  | expression BINAND expression\n                  | expression BINOR expression\n                  | expression BINXOR expression\n                  | expression SHRU expression\n                  | expression SHR expression\n                  | expression SHL expression\n                  | expression LT expression\n                  | expression GT expression\n                  | expression LE expression\n                  | expression GE expression\n                  | expression EQ expression\n                  | expression NEQ expression\n    expression : NAME LBRACKET NUMBER RBRACKET ASSIGN expressionexpression : NAME LPAREN NUMBER RPARENexpression : NAME LPAREN expression COMMA expression RPARENexpression : NAME LPAREN NUMBER COMMA NAME ASSIGN     NUMBER COMMA NAME ASSIGN NUMBER RPAREN\n                  | NAME LPAREN NUMBER COMMA NAME ASSIGN expression COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN\n                  | NAME LPAREN NUMBER COMMA NAME ASSIGN     NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN\n    expression : LPAREN expression RPARENexpression : NAME LBRACKET NUMBER RBRACKETexpression : NUMBER\n                  | SUB NUMBER %prec UMINUS\n    expression : NAME'
+_lr_signature = 'leftLTGTLEGEEQNEQleftSHRUSHRSHLleftBINORleftBINXORleftBINANDleftADDSUBleftMULrightUMINUSADD ASSIGN BINAND BINOR BINXOR COMMA EQ GE GT LBRACKET LE LPAREN LT MUL NAME NEQ NEWLINE NUMBER RBRACKET RPAREN SHL SHR SHRU SUBlines : line\n             | expression\n             | lines line\n    line : expression NEWLINE\n            | NEWLINE\n    expression : expression ADD expression\n                  | expression SUB expression\n                  | expression MUL expression\n                  | expression BINAND expression\n                  | expression BINOR expression\n                  | expression BINXOR expression\n                  | expression SHRU expression\n                  | expression SHR expression\n                  | expression SHL expression\n                  | expression LT expression\n                  | expression GT expression\n                  | expression LE expression\n                  | expression GE expression\n                  | expression EQ expression\n                  | expression NEQ expression\n    expression : NAME LBRACKET NUMBER RBRACKET ASSIGN expressionexpression : NAME LPAREN NUMBER RPARENexpression : NAME LPAREN expression COMMA expression RPARENexpression : NAME LPAREN NUMBER COMMA NAME ASSIGN     NUMBER COMMA NAME ASSIGN NUMBER RPAREN\n                  | NAME LPAREN NUMBER COMMA NAME ASSIGN     NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN\n                  | NAME LPAREN NUMBER COMMA NAME ASSIGN expression COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN\n                  | NAME LPAREN NUMBER COMMA NAME ASSIGN     NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN\n    expression : LPAREN expression RPARENexpression : NAME LBRACKET NUMBER RBRACKETexpression : NUMBER\n                  | SUB NUMBER %prec UMINUS\n    expression : NAME'
     
-_lr_action_items = {'NEWLINE':([0,1,2,3,4,6,7,9,10,11,27,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,57,59,71,80,84,],[4,4,-1,11,-5,-31,-29,-3,11,-4,-30,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-27,-28,-22,-21,-23,-24,-25,-26,]),'NAME':([0,1,2,3,4,6,7,8,9,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,29,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,52,53,54,57,58,59,62,63,70,71,72,79,80,84,],[6,6,-1,-2,-5,-31,-29,6,-3,-4,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,-30,6,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-27,-28,-22,55,6,6,-21,6,-23,64,65,73,-24,74,81,-25,-26,]),'LPAREN':([0,1,2,3,4,6,7,8,9,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,29,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,53,54,57,58,59,71,80,84,],[8,8,-1,-2,-5,29,-29,8,-3,-4,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,-30,8,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-27,-28,-22,8,8,-21,8,-23,-24,-25,-26,]),'NUMBER':([0,1,2,3,4,5,6,7,8,9,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,53,54,57,58,59,66,67,71,75,76,80,82,84,],[7,7,-1,-2,-5,27,-31,-29,7,-3,-4,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,-30,46,47,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-27,-28,-22,7,7,-21,60,-23,68,69,-24,77,78,-25,83,-26,]),'SUB':([0,1,2,3,4,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,53,54,56,57,58,59,60,61,71,80,84,],[5,5,-1,13,-5,-31,-29,5,-3,13,-4,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,-30,5,13,-6,-7,-8,13,13,13,13,13,13,13,13,13,13,13,13,-29,13,-27,-28,-22,5,5,13,13,5,-23,-29,13,-24,-25,-26,]),'$end':([1,2,3,4,6,7,9,11,27,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,57,59,71,80,84,],[0,-1,-2,-5,-31,-29,-3,-4,-30,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-27,-28,-22,-21,-23,-24,-25,-26,]),'ADD':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[12,-31,-29,12,-30,12,-6,-7,-8,12,12,12,12,12,12,12,12,12,12,12,12,-29,12,-27,-28,-22,12,12,-23,-29,12,-24,-25,-26,]),'MUL':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[14,-31,-29,14,-30,14,14,14,-8,14,14,14,14,14,14,14,14,14,14,14,14,-29,14,-27,-28,-22,14,14,-23,-29,14,-24,-25,-26,]),'BINAND':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[15,-31,-29,15,-30,15,-6,-7,-8,-9,15,15,15,15,15,15,15,15,15,15,15,-29,15,-27,-28,-22,15,15,-23,-29,15,-24,-25,-26,]),'BINOR':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[16,-31,-29,16,-30,16,-6,-7,-8,-9,-10,-11,16,16,16,16,16,16,16,16,16,-29,16,-27,-28,-22,16,16,-23,-29,16,-24,-25,-26,]),'BINXOR':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[17,-31,-29,17,-30,17,-6,-7,-8,-9,17,-11,17,17,17,17,17,17,17,17,17,-29,17,-27,-28,-22,17,17,-23,-29,17,-24,-25,-26,]),'SHRU':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[18,-31,-29,18,-30,18,-6,-7,-8,-9,-10,-11,-12,-13,-14,18,18,18,18,18,18,-29,18,-27,-28,-22,18,18,-23,-29,18,-24,-25,-26,]),'SHR':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[19,-31,-29,19,-30,19,-6,-7,-8,-9,-10,-11,-12,-13,-14,19,19,19,19,19,19,-29,19,-27,-28,-22,19,19,-23,-29,19,-24,-25,-26,]),'SHL':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[20,-31,-29,20,-30,20,-6,-7,-8,-9,-10,-11,-12,-13,-14,20,20,20,20,20,20,-29,20,-27,-28,-22,20,20,-23,-29,20,-24,-25,-26,]),'LT':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[21,-31,-29,21,-30,21,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-29,21,-27,-28,-22,21,21,-23,-29,21,-24,-25,-26,]),'GT':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[22,-31,-29,22,-30,22,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-29,22,-27,-28,-22,22,22,-23,-29,22,-24,-25,-26,]),'LE':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[23,-31,-29,23,-30,23,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-29,23,-27,-28,-22,23,23,-23,-29,23,-24,-25,-26,]),'GE':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[24,-31,-29,24,-30,24,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-29,24,-27,-28,-22,24,24,-23,-29,24,-24,-25,-26,]),'EQ':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[25,-31,-29,25,-30,25,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-29,25,-27,-28,-22,25,25,-23,-29,25,-24,-25,-26,]),'NEQ':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,84,],[26,-31,-29,26,-30,26,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-29,26,-27,-28,-22,26,26,-23,-29,26,-24,-25,-26,]),'LBRACKET':([6,],[28,]),'RPAREN':([6,7,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,49,50,51,56,57,59,68,71,78,80,83,84,],[-31,-29,-30,49,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,51,-27,-28,-22,59,-21,-23,71,-24,80,-25,84,-26,]),'COMMA':([6,7,27,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,57,59,60,61,68,69,71,77,80,84,],[-31,-29,-30,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,52,53,-27,-28,-22,-21,-23,62,63,70,72,-24,79,-25,-26,]),'RBRACKET':([46,],[50,]),'ASSIGN':([50,55,64,65,73,74,81,],[54,58,66,67,75,76,82,]),}
+_lr_action_items = {'NEWLINE':([0,1,2,3,4,6,7,9,10,11,27,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,57,59,71,80,81,85,],[4,4,-1,11,-5,-32,-30,-3,11,-4,-31,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-28,-29,-22,-21,-23,-24,-25,-26,-27,]),'NAME':([0,1,2,3,4,6,7,8,9,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,29,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,52,53,54,57,58,59,62,63,70,71,72,79,80,81,85,],[6,6,-1,-2,-5,-32,-30,6,-3,-4,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,-31,6,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-28,-29,-22,55,6,6,-21,6,-23,64,65,73,-24,74,82,-25,-26,-27,]),'LPAREN':([0,1,2,3,4,6,7,8,9,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,29,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,53,54,57,58,59,71,80,81,85,],[8,8,-1,-2,-5,29,-30,8,-3,-4,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,-31,8,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-28,-29,-22,8,8,-21,8,-23,-24,-25,-26,-27,]),'NUMBER':([0,1,2,3,4,5,6,7,8,9,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,53,54,57,58,59,66,67,71,75,76,80,81,83,85,],[7,7,-1,-2,-5,27,-32,-30,7,-3,-4,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,-31,46,47,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-28,-29,-22,7,7,-21,60,-23,68,69,-24,77,78,-25,-26,84,-27,]),'SUB':([0,1,2,3,4,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,53,54,56,57,58,59,60,61,71,80,81,85,],[5,5,-1,13,-5,-32,-30,5,-3,13,-4,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,-31,5,13,-6,-7,-8,13,13,13,13,13,13,13,13,13,13,13,13,-30,13,-28,-29,-22,5,5,13,13,5,-23,-30,13,-24,-25,-26,-27,]),'$end':([1,2,3,4,6,7,9,11,27,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,49,50,51,57,59,71,80,81,85,],[0,-1,-2,-5,-32,-30,-3,-4,-31,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-28,-29,-22,-21,-23,-24,-25,-26,-27,]),'ADD':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[12,-32,-30,12,-31,12,-6,-7,-8,12,12,12,12,12,12,12,12,12,12,12,12,-30,12,-28,-29,-22,12,12,-23,-30,12,-24,-25,-26,-27,]),'MUL':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[14,-32,-30,14,-31,14,14,14,-8,14,14,14,14,14,14,14,14,14,14,14,14,-30,14,-28,-29,-22,14,14,-23,-30,14,-24,-25,-26,-27,]),'BINAND':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[15,-32,-30,15,-31,15,-6,-7,-8,-9,15,15,15,15,15,15,15,15,15,15,15,-30,15,-28,-29,-22,15,15,-23,-30,15,-24,-25,-26,-27,]),'BINOR':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[16,-32,-30,16,-31,16,-6,-7,-8,-9,-10,-11,16,16,16,16,16,16,16,16,16,-30,16,-28,-29,-22,16,16,-23,-30,16,-24,-25,-26,-27,]),'BINXOR':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[17,-32,-30,17,-31,17,-6,-7,-8,-9,17,-11,17,17,17,17,17,17,17,17,17,-30,17,-28,-29,-22,17,17,-23,-30,17,-24,-25,-26,-27,]),'SHRU':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[18,-32,-30,18,-31,18,-6,-7,-8,-9,-10,-11,-12,-13,-14,18,18,18,18,18,18,-30,18,-28,-29,-22,18,18,-23,-30,18,-24,-25,-26,-27,]),'SHR':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[19,-32,-30,19,-31,19,-6,-7,-8,-9,-10,-11,-12,-13,-14,19,19,19,19,19,19,-30,19,-28,-29,-22,19,19,-23,-30,19,-24,-25,-26,-27,]),'SHL':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[20,-32,-30,20,-31,20,-6,-7,-8,-9,-10,-11,-12,-13,-14,20,20,20,20,20,20,-30,20,-28,-29,-22,20,20,-23,-30,20,-24,-25,-26,-27,]),'LT':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[21,-32,-30,21,-31,21,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-30,21,-28,-29,-22,21,21,-23,-30,21,-24,-25,-26,-27,]),'GT':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[22,-32,-30,22,-31,22,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-30,22,-28,-29,-22,22,22,-23,-30,22,-24,-25,-26,-27,]),'LE':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[23,-32,-30,23,-31,23,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-30,23,-28,-29,-22,23,23,-23,-30,23,-24,-25,-26,-27,]),'GE':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[24,-32,-30,24,-31,24,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-30,24,-28,-29,-22,24,24,-23,-30,24,-24,-25,-26,-27,]),'EQ':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[25,-32,-30,25,-31,25,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-30,25,-28,-29,-22,25,25,-23,-30,25,-24,-25,-26,-27,]),'NEQ':([3,6,7,10,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,56,57,59,60,61,71,80,81,85,],[26,-32,-30,26,-31,26,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,-30,26,-28,-29,-22,26,26,-23,-30,26,-24,-25,-26,-27,]),'LBRACKET':([6,],[28,]),'RPAREN':([6,7,27,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,49,50,51,56,57,59,68,71,77,78,80,81,84,85,],[-32,-30,-31,49,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,51,-28,-29,-22,59,-21,-23,71,-24,80,81,-25,-26,85,-27,]),'COMMA':([6,7,27,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,47,48,49,50,51,57,59,60,61,68,69,71,77,80,81,85,],[-32,-30,-31,-6,-7,-8,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-20,52,53,-28,-29,-22,-21,-23,62,63,70,72,-24,79,-25,-26,-27,]),'RBRACKET':([46,],[50,]),'ASSIGN':([50,55,64,65,73,74,82,],[54,58,66,67,75,76,83,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
       _lr_action[_x][_k] = _y
 del _lr_action_items
@@ -23,39 +23,40 @@
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
 _lr_productions = [
   ("S' -> lines","S'",1,None,None,None),
-  ('lines -> line','lines',1,'p_lines','parser.py',467),
-  ('lines -> expression','lines',1,'p_lines','parser.py',468),
-  ('lines -> lines line','lines',2,'p_lines','parser.py',469),
-  ('line -> expression NEWLINE','line',2,'p_line','parser.py',483),
-  ('line -> NEWLINE','line',1,'p_line','parser.py',484),
-  ('expression -> expression ADD expression','expression',3,'p_expression_binop','parser.py',511),
-  ('expression -> expression SUB expression','expression',3,'p_expression_binop','parser.py',512),
-  ('expression -> expression MUL expression','expression',3,'p_expression_binop','parser.py',513),
-  ('expression -> expression BINAND expression','expression',3,'p_expression_binop','parser.py',514),
-  ('expression -> expression BINOR expression','expression',3,'p_expression_binop','parser.py',515),
-  ('expression -> expression BINXOR expression','expression',3,'p_expression_binop','parser.py',516),
-  ('expression -> expression SHRU expression','expression',3,'p_expression_binop','parser.py',517),
-  ('expression -> expression SHR expression','expression',3,'p_expression_binop','parser.py',518),
-  ('expression -> expression SHL expression','expression',3,'p_expression_binop','parser.py',519),
-  ('expression -> expression LT expression','expression',3,'p_expression_binop','parser.py',520),
-  ('expression -> expression GT expression','expression',3,'p_expression_binop','parser.py',521),
-  ('expression -> expression LE expression','expression',3,'p_expression_binop','parser.py',522),
-  ('expression -> expression GE expression','expression',3,'p_expression_binop','parser.py',523),
-  ('expression -> expression EQ expression','expression',3,'p_expression_binop','parser.py',524),
-  ('expression -> expression NEQ expression','expression',3,'p_expression_binop','parser.py',525),
-  ('expression -> NAME LBRACKET NUMBER RBRACKET ASSIGN expression','expression',6,'p_expression_assign','parser.py',572),
-  ('expression -> NAME LPAREN NUMBER RPAREN','expression',4,'p_expression_call1','parser.py',585),
-  ('expression -> NAME LPAREN expression COMMA expression RPAREN','expression',6,'p_expression_call2','parser.py',591),
-  ('expression -> NAME LPAREN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN','expression',12,'p_expression_call3','parser.py',606),
-  ('expression -> NAME LPAREN NUMBER COMMA NAME ASSIGN expression COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN','expression',16,'p_expression_call3','parser.py',607),
-  ('expression -> NAME LPAREN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN','expression',20,'p_expression_call3','parser.py',608),
-  ('expression -> LPAREN expression RPAREN','expression',3,'p_expression_group','parser.py',633),
-  ('expression -> NAME LBRACKET NUMBER RBRACKET','expression',4,'p_expression_storage','parser.py',638),
-  ('expression -> NUMBER','expression',1,'p_expression_number','parser.py',646),
-  ('expression -> SUB NUMBER','expression',2,'p_expression_number','parser.py',647),
-  ('expression -> NAME','expression',1,'p_expression_name','parser.py',656),
+  ('lines -> line','lines',1,'p_lines','parser.py',477),
+  ('lines -> expression','lines',1,'p_lines','parser.py',478),
+  ('lines -> lines line','lines',2,'p_lines','parser.py',479),
+  ('line -> expression NEWLINE','line',2,'p_line','parser.py',493),
+  ('line -> NEWLINE','line',1,'p_line','parser.py',494),
+  ('expression -> expression ADD expression','expression',3,'p_expression_binop','parser.py',521),
+  ('expression -> expression SUB expression','expression',3,'p_expression_binop','parser.py',522),
+  ('expression -> expression MUL expression','expression',3,'p_expression_binop','parser.py',523),
+  ('expression -> expression BINAND expression','expression',3,'p_expression_binop','parser.py',524),
+  ('expression -> expression BINOR expression','expression',3,'p_expression_binop','parser.py',525),
+  ('expression -> expression BINXOR expression','expression',3,'p_expression_binop','parser.py',526),
+  ('expression -> expression SHRU expression','expression',3,'p_expression_binop','parser.py',527),
+  ('expression -> expression SHR expression','expression',3,'p_expression_binop','parser.py',528),
+  ('expression -> expression SHL expression','expression',3,'p_expression_binop','parser.py',529),
+  ('expression -> expression LT expression','expression',3,'p_expression_binop','parser.py',530),
+  ('expression -> expression GT expression','expression',3,'p_expression_binop','parser.py',531),
+  ('expression -> expression LE expression','expression',3,'p_expression_binop','parser.py',532),
+  ('expression -> expression GE expression','expression',3,'p_expression_binop','parser.py',533),
+  ('expression -> expression EQ expression','expression',3,'p_expression_binop','parser.py',534),
+  ('expression -> expression NEQ expression','expression',3,'p_expression_binop','parser.py',535),
+  ('expression -> NAME LBRACKET NUMBER RBRACKET ASSIGN expression','expression',6,'p_expression_assign','parser.py',582),
+  ('expression -> NAME LPAREN NUMBER RPAREN','expression',4,'p_expression_call1','parser.py',595),
+  ('expression -> NAME LPAREN expression COMMA expression RPAREN','expression',6,'p_expression_call2','parser.py',601),
+  ('expression -> NAME LPAREN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN','expression',12,'p_expression_call3','parser.py',616),
+  ('expression -> NAME LPAREN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN','expression',16,'p_expression_call3','parser.py',617),
+  ('expression -> NAME LPAREN NUMBER COMMA NAME ASSIGN expression COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN','expression',16,'p_expression_call3','parser.py',618),
+  ('expression -> NAME LPAREN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER COMMA NAME ASSIGN NUMBER RPAREN','expression',20,'p_expression_call3','parser.py',619),
+  ('expression -> LPAREN expression RPAREN','expression',3,'p_expression_group','parser.py',644),
+  ('expression -> NAME LBRACKET NUMBER RBRACKET','expression',4,'p_expression_storage','parser.py',649),
+  ('expression -> NUMBER','expression',1,'p_expression_number','parser.py',657),
+  ('expression -> SUB NUMBER','expression',2,'p_expression_number','parser.py',658),
+  ('expression -> NAME','expression',1,'p_expression_name','parser.py',667),
 ]
```

### Comparing `grf-0.2.1/grf/sprites.py` & `grf-0.2.2/grf/sprites.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,14 +109,43 @@
     def get_data(self):
         return struct.pack('<I', self.sprite_id)
 
     def get_real_data(self, encoder):
         raise NotImplementedError
 
 
+class AlternativeSprites(RealSprite):
+    def __init__(self, *sprites):
+        assert all(isinstance(s, GraphicsSprite) for s in sprites), sprites
+        assert len(set((s.zoom, s.bpp) for s in sprites)) == len(sprites), sprites
+
+        self.sprites = sprites
+        super().__init__()
+        self._sprite_id = None
+
+    @property
+    def sprite_id(self):
+        return self._sprite_id
+
+    @sprite_id.setter
+    def sprite_id(self, value):
+        self._sprite_id = value
+        for s in self.sprites:
+            s.sprite_id = value
+
+    def get_real_data(self, encoder):
+        return b''.join(s.get_real_data(encoder) for s in self.sprites)
+
+    def get_zoom(self, zoom):
+        for s in self.sprites:
+            if s.zoom == zoom:
+                return s
+        return None
+
+
 class SoundSprite(RealSprite):
     def __init__(self):
         super().__init__()
         self.id = None
 
     def get_hash(self):
         raise NotImplemented
@@ -279,61 +308,61 @@
             if self.bpp == BPP_8:
                 npimg = npimg[crop_y: crop_y + h, crop_x: crop_x + w]
             else:
                 npimg = npimg[crop_y: crop_y + h, crop_x: crop_x + w, :]
 
         info_byte = 0x40
         if self.bpp == BPP_24 or self.bpp == BPP_32:
-            stack = [npimg]
-
             if self.bpp == BPP_32:
-                npimg.reshape((w * h, 4))
+                npimg = npimg.reshape(w * h, 4)
                 rbpp = 4
                 info_byte |= 0x1 | 0x2  # rgb, alph
 
                 if npalpha is not None:
                     npimg = npimg[:, :3]
-                    npalpha.reshape((w * h, 1))
+                    npalpha = npalpha.reshape(w * h, 1)
                     stack = [npimg, npalpha]
+                else:
+                    stack = [npimg]
             else:
-                npimg.reshape((w * h, 3))
+                npimg = npimg.reshape(w * h, 3)
                 rbpp = 3
                 info_byte = 0x1  # rgb
 
                 if npalpha is not None:
-                    npalpha.reshape((w * h, 1))
-                    stack.append(npalpha)
+                    npalpha = npalpha.reshape(w * h, 1)
+                    stack = [npimg, npalpha]
                     rbpp += 1
                     info_byte |= 0x2  # alpha
-
+                else:
+                    stack = [npimg]
 
             if self.mask is not None:
                 mask_file, mxofs, myofs = self.mask
                 mask_img, mask_bpp = self.get_mask_image()
                 if mask_bpp != BPP_8:
                     raise RuntimeError(f'Mask {mask_file.path} is not an 8bpp image')
                 mxofs, myofs = self.x + mxofs + crop_x, self.y + myofs + crop_y
                 mask_img = mask_img.crop((mxofs, myofs, mxofs + w, myofs + h))
                 mask_img = fix_palette(mask_img, f'{mask_file.path} {mxofs},{myofs} {w}x{h}')
                 npmask = np.asarray(mask_img)
-                npmask.reshape((w * h, 1))
+                npmask = npmask.reshape(w * h, 1)
                 stack.append(npmask)
                 rbpp += 1
                 info_byte |= 0x4  # mask
 
             if len(stack) > 1:
                 raw_data = np.concatenate(stack, axis=1)
             else:
                 raw_data = stack[0]
-            raw_data.reshape(w * h * rbpp, order='c')
+            raw_data = raw_data.reshape(w * h * rbpp)
 
         else:
             info_byte |= 0x4  # pal/mask
-            raw_data = npimg
-            raw_data.reshape(w * h, order='c')
+            raw_data = npimg.reshape(w * h)
 
         encoder.count_composing(time.time() - t0)
         data = encoder.sprite_compress(np.ascontiguousarray(raw_data))
         return struct.pack(
             '<IIBBHHhh',
             self.sprite_id,
             len(data) + 10,
```

### Comparing `grf-0.2.1/grf/strings.py` & `grf-0.2.2/grf/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,17 @@
     def __getitem__(self, name):
         full_name = 'STR_' + name
         if full_name not in self._default_lang.strings:
             raise KeyError(name)
         return StringRef(self, nml.expression.Identifier(full_name, None), hash(full_name))
 
     def add(self, value, name=None):
+        if isinstance(value, StringRef):
+            assert name is None
+            return value
         if name is None:
             name = self._named_strings.get(value)
             if name is None:
                 name = f'GRFPY_{self._next_string_id}'
                 self._next_string_id += 1
                 self._named_strings[value] = name
                 self._default_lang.handle_text(name, None, value, None)
@@ -125,14 +128,20 @@
 
 class StringRef:
     def __init__(self, manager, nmlexpr, hash):
         self.manager = manager
         self.nmlexpr = nmlexpr
         self.hash = hash
 
+    def __hash__(self):
+        return self.hash
+
+    def __eq__(self, value):
+        return self.hash == value.hash
+
     @property
     def string_nmlexpr(self):
         if isinstance(self.nmlexpr, nml.expression.String):
             return self.nmlexpr
         return nml.expression.String([self.nmlexpr], None)
 
     def eval(self, *args):
```

### Comparing `grf-0.2.1/grf/va2vars.py` & `grf-0.2.2/grf/va2vars.py`

 * *Files identical despite different names*

### Comparing `grf-0.2.1/setup.py` & `grf-0.2.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
+from pathlib import Path
+
+root_path = Path(__file__).parent
 
 install_requires = [
-    'nml==0.6.1',
-    'numpy==1.22.0',
-    'Pillow==8.4.0',
+    'nml==0.7.4',
+    'numpy==1.25.0',
+    'Pillow==9.4.0',
+    'ply==3.11',
     'spectra==0.0.11',
 ]
 
 setup(
     name='grf',
-    version='0.2.1',
+    setuptools_git_versioning={
+        "enabled": True,
+        "version_file": root_path / "VERSION",
+    },
     description='Framework for making OpenTTD NewGRF files',
     author='dP',
     packages=find_packages(include=['grf']),
     entry_points={
         'console_scripts': [
             'grftopy = grf.decompile:main',
         ]
     },
     install_requires=install_requires,
     python_requires=">=3.6.9",
+    setup_requires=["setuptools-git-versioning<2"],
 )
```

