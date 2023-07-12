# Comparing `tmp/lightning_rod-0.2.4.tar.gz` & `tmp/lightning_rod-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_rod-0.2.4.tar", max compression
+gzip compressed data, was "lightning_rod-0.2.5.tar", max compression
```

## Comparing `lightning_rod-0.2.4.tar` & `lightning_rod-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1061 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/LICENSE
--rw-r--r--   0        0        0     1389 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/README.md
--rw-r--r--   0        0        0      307 2023-07-05 19:29:24.543454 lightning_rod-0.2.4/lightning_rod/__init__.py
--rw-r--r--   0        0        0      667 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/advancement.bolt
--rw-r--r--   0        0        0      566 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/api.bolt
--rw-r--r--   0        0        0     4562 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/bossbar.bolt
--rw-r--r--   0        0        0       38 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/cancel_momentum.bolt
--rw-r--r--   0        0        0      314 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/clear.bolt
--rw-r--r--   0        0        0       85 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/comment.bolt
--rw-r--r--   0        0        0      144 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/config.bolt
--rw-r--r--   0        0        0     1593 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/effect.bolt
--rw-r--r--   0        0        0      569 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/gamemode.bolt
--rw-r--r--   0        0        0      157 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/give.bolt
--rw-r--r--   0        0        0       25 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/kill.bolt
--rw-r--r--   0        0        0     2521 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/math.bolt
--rw-r--r--   0        0        0       35 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/raw_cmd.bolt
--rw-r--r--   0        0        0       86 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/tag.bolt
--rw-r--r--   0        0        0     1029 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/time.bolt
--rw-r--r--   0        0        0      300 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/utils.bolt
--rw-r--r--   0        0        0     2175 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/xp.bolt
--rw-r--r--   0        0        0        0 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/py.typed
--rw-r--r--   0        0        0     1242 2023-07-05 19:29:24.559454 lightning_rod-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 lightning_rod-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1389 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/README.md
+-rw-r--r--   0        0        0      307 2023-07-12 04:55:00.041716 lightning_rod-0.2.5/lightning_rod/__init__.py
+-rw-r--r--   0        0        0      667 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/advancement.bolt
+-rw-r--r--   0        0        0      566 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/api.bolt
+-rw-r--r--   0        0        0     4562 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/bossbar.bolt
+-rw-r--r--   0        0        0       38 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/cancel_momentum.bolt
+-rw-r--r--   0        0        0      314 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/clear.bolt
+-rw-r--r--   0        0        0       85 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/comment.bolt
+-rw-r--r--   0        0        0      144 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/config.bolt
+-rw-r--r--   0        0        0     1593 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/effect.bolt
+-rw-r--r--   0        0        0      569 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/gamemode.bolt
+-rw-r--r--   0        0        0      157 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/give.bolt
+-rw-r--r--   0        0        0       25 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/kill.bolt
+-rw-r--r--   0        0        0     2521 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/math.bolt
+-rw-r--r--   0        0        0       35 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/raw_cmd.bolt
+-rw-r--r--   0        0        0       86 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/tag.bolt
+-rw-r--r--   0        0        0     1029 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/time.bolt
+-rw-r--r--   0        0        0      300 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/utils.bolt
+-rw-r--r--   0        0        0     2175 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/modules/xp.bolt
+-rw-r--r--   0        0        0        0 2023-07-12 04:54:17.061287 lightning_rod-0.2.5/lightning_rod/py.typed
+-rw-r--r--   0        0        0     1242 2023-07-12 04:55:00.061716 lightning_rod-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 lightning_rod-0.2.5/PKG-INFO
```

### Comparing `lightning_rod-0.2.4/LICENSE` & `lightning_rod-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/README.md` & `lightning_rod-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/lightning_rod/modules/advancement.bolt` & `lightning_rod-0.2.5/lightning_rod/modules/advancement.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/lightning_rod/modules/api.bolt` & `lightning_rod-0.2.5/lightning_rod/modules/api.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/lightning_rod/modules/bossbar.bolt` & `lightning_rod-0.2.5/lightning_rod/modules/bossbar.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/lightning_rod/modules/effect.bolt` & `lightning_rod-0.2.5/lightning_rod/modules/effect.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/lightning_rod/modules/gamemode.bolt` & `lightning_rod-0.2.5/lightning_rod/modules/gamemode.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/lightning_rod/modules/math.bolt` & `lightning_rod-0.2.5/lightning_rod/modules/math.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/lightning_rod/modules/time.bolt` & `lightning_rod-0.2.5/lightning_rod/modules/time.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/lightning_rod/modules/xp.bolt` & `lightning_rod-0.2.5/lightning_rod/modules/xp.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.4/pyproject.toml` & `lightning_rod-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightning_rod"
-version = "0.2.4"
+version = "0.2.5"
 description = "Function library for the Bolt scripting language."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/lightning-rod"
 readme = "README.md"
 
@@ -19,18 +19,18 @@
   "reapermc",
 ]
 
 include = ["lightning_rod/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-beet = ">=0.84.0"
-mecha = ">=0.67.0"
-bolt = ">=0.31.0"
-wicked-expressions = ">=0.6.0"
+beet = ">=0.89.1"
+mecha = ">=0.73.0"
+bolt = ">=0.36.0"
+wicked-expressions = ">=0.8.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^22.10.0"
 isort = "^5.10.1"
 pytest-insta = "^0.1.11"
 lectern = ">=0.25.0"
```

### Comparing `lightning_rod-0.2.4/PKG-INFO` & `lightning_rod-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lightning-rod
-Version: 0.2.4
+Version: 0.2.5
 Summary: Function library for the Bolt scripting language.
 Home-page: https://github.com/reapermc/lightning-rod
 License: MIT
 Keywords: beet,bolt,minecraft,datapack,minecraft-commands,mcfunction,library,reapermc
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beet (>=0.84.0)
-Requires-Dist: bolt (>=0.31.0)
-Requires-Dist: mecha (>=0.67.0)
-Requires-Dist: wicked-expressions (>=0.6.0)
+Requires-Dist: beet (>=0.89.1)
+Requires-Dist: bolt (>=0.36.0)
+Requires-Dist: mecha (>=0.73.0)
+Requires-Dist: wicked-expressions (>=0.8.1)
 Description-Content-Type: text/markdown
 
 # lightning-rod
 
 [![GitHub Actions](https://github.com/reapermc/lightning-rod/workflows/CI/badge.svg)](https://github.com/reapermc/lightning-rod/actions)
 
 > Function library for the Bolt scripting language.
```

