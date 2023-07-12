# Comparing `tmp/wicked_expressions-0.8.0.tar.gz` & `tmp/wicked_expressions-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.8.0.tar", max compression
+gzip compressed data, was "wicked_expressions-0.8.1.tar", max compression
```

## Comparing `wicked_expressions-0.8.0.tar` & `wicked_expressions-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-07-10 19:15:59.395522 wicked_expressions-0.8.0/LICENSE
--rw-r--r--   0        0        0     2166 2023-07-10 19:15:59.395522 wicked_expressions-0.8.0/README.md
--rw-r--r--   0        0        0     1219 2023-07-10 19:17:39.854281 wicked_expressions-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      321 2023-07-10 19:17:39.838281 wicked_expressions-0.8.0/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      725 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     9084 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      305 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     1850 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      402 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8436 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0      375 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/rebindable.bolt
--rw-r--r--   0        0        0      596 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/safe_load.bolt
--rw-r--r--   0        0        0     3118 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1460 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     6454 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 wicked_expressions-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-12 04:48:26.629774 wicked_expressions-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2166 2023-07-12 04:48:26.629774 wicked_expressions-0.8.1/README.md
+-rw-r--r--   0        0        0     1219 2023-07-12 04:49:47.058801 wicked_expressions-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-07-12 04:49:47.042800 wicked_expressions-0.8.1/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      725 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     9084 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      305 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     1850 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      402 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8436 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0      375 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/rebindable.bolt
+-rw-r--r--   0        0        0      596 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/safe_load.bolt
+-rw-r--r--   0        0        0     3118 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1460 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     6454 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 wicked_expressions-0.8.1/PKG-INFO
```

### Comparing `wicked_expressions-0.8.0/LICENSE` & `wicked_expressions-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/README.md` & `wicked_expressions-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/pyproject.toml` & `wicked_expressions-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.8.0"
+version = "0.8.1"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
 
@@ -16,17 +16,17 @@
   "mcfunction",
 ]
 
 include = ["wicked_expressions/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-beet = ">=0.84.0"
-mecha = ">=0.67.0"
-bolt = ">=0.31.0"
+beet = ">=0.89.1"
+mecha = ">=0.73.0"
+bolt = ">=0.36.0"
 bolt-expressions = ">=0.12.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^22.10.0"
 isort = "^5.10.1"
 pytest-insta = ">=0.1.11,<0.3.0"
```

### Comparing `wicked_expressions-0.8.0/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.8.1/wicked_expressions/modules/api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.8.1/wicked_expressions/modules/comparison.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.8.1/wicked_expressions/modules/internal_api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.8.1/wicked_expressions/modules/raw_operations.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/wicked_expressions/modules/safe_load.bolt` & `wicked_expressions-0.8.1/wicked_expressions/modules/safe_load.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.8.1/wicked_expressions/modules/sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.8.1/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.8.1/wicked_expressions/modules/var.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.8.1/wicked_expressions/modules/var_sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.0/PKG-INFO` & `wicked_expressions-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.8.0
+Version: 0.8.1
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beet (>=0.84.0)
-Requires-Dist: bolt (>=0.31.0)
+Requires-Dist: beet (>=0.89.1)
+Requires-Dist: bolt (>=0.36.0)
 Requires-Dist: bolt-expressions (>=0.12.2)
-Requires-Dist: mecha (>=0.67.0)
+Requires-Dist: mecha (>=0.73.0)
 Description-Content-Type: text/markdown
 
 # wicked-expressions
 
 [![GitHub Actions](https://github.com/reapermc/wicked-expressions/workflows/CI/badge.svg)](https://github.com/reapermc/wicked-expressions/actions)
 
 > Extension of bolt-expressions written in Bolt.
```

