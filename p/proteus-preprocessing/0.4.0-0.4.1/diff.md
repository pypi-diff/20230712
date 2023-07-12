# Comparing `tmp/proteus_preprocessing-0.4.0.tar.gz` & `tmp/proteus_preprocessing-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_preprocessing-0.4.0.tar", max compression
+gzip compressed data, was "proteus_preprocessing-0.4.1.tar", max compression
```

## Comparing `proteus_preprocessing-0.4.0.tar` & `proteus_preprocessing-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0       43 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/deck/__init__.py
--rw-r--r--   0        0        0      909 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/deck/ecl_deck.py
--rw-r--r--   0        0        0     8837 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/deck/runspec.py
--rw-r--r--   0        0        0     2999 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/deck/section.py
--rw-r--r--   0        0        0        0 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/modular/__init__.py
--rw-r--r--   0        0        0      548 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/modular/dat.py
--rw-r--r--   0        0        0    16684 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/modular/data.py
--rw-r--r--   0        0        0      415 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/modular/egrid.py
--rw-r--r--   0        0        0      365 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/modular/grdecl.py
--rw-r--r--   0        0        0     2123 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/modular/init.py
--rw-r--r--   0        0        0     5402 2023-07-12 09:24:02.308837 proteus_preprocessing-0.4.0/preprocessing/modular/s.py
--rw-r--r--   0        0        0      178 2023-07-12 09:24:02.312837 proteus_preprocessing-0.4.0/preprocessing/modular/x.py
--rw-r--r--   0        0        0      221 2023-07-12 09:24:02.312837 proteus_preprocessing-0.4.0/preprocessing/patches.py
--rw-r--r--   0        0        0       71 2023-07-12 09:24:02.312837 proteus_preprocessing-0.4.0/preprocessing/utils/__init__.py
--rw-r--r--   0        0        0     1062 2023-07-12 09:24:02.312837 proteus_preprocessing-0.4.0/preprocessing/utils/expand_dates.py
--rw-r--r--   0        0        0      901 2023-07-12 09:24:02.312837 proteus_preprocessing-0.4.0/preprocessing/utils/expand_wcon.py
--rw-r--r--   0        0        0     1526 2023-07-12 09:24:02.312837 proteus_preprocessing-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 proteus_preprocessing-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/deck/__init__.py
+-rw-r--r--   0        0        0      909 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/deck/ecl_deck.py
+-rw-r--r--   0        0        0     8837 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/deck/runspec.py
+-rw-r--r--   0        0        0     2999 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/deck/section.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/facilities/__init__.py
+-rw-r--r--   0        0        0     2509 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/facilities/flowline.py
+-rw-r--r--   0        0        0     1461 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/facilities/network.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/modular/__init__.py
+-rw-r--r--   0        0        0      548 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/dat.py
+-rw-r--r--   0        0        0    16684 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/data.py
+-rw-r--r--   0        0        0      415 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/egrid.py
+-rw-r--r--   0        0        0      365 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/grdecl.py
+-rw-r--r--   0        0        0     2123 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/init.py
+-rw-r--r--   0        0        0     5402 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/s.py
+-rw-r--r--   0        0        0      178 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/x.py
+-rw-r--r--   0        0        0      221 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/patches.py
+-rw-r--r--   0        0        0       71 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/utils/__init__.py
+-rw-r--r--   0        0        0     1062 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/utils/expand_dates.py
+-rw-r--r--   0        0        0      901 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/utils/expand_wcon.py
+-rw-r--r--   0        0        0     1572 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 proteus_preprocessing-0.4.1/PKG-INFO
```

### Comparing `proteus_preprocessing-0.4.0/preprocessing/deck/ecl_deck.py` & `proteus_preprocessing-0.4.1/preprocessing/deck/ecl_deck.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.0/preprocessing/deck/runspec.py` & `proteus_preprocessing-0.4.1/preprocessing/deck/runspec.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.0/preprocessing/deck/section.py` & `proteus_preprocessing-0.4.1/preprocessing/deck/section.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.0/preprocessing/modular/dat.py` & `proteus_preprocessing-0.4.1/preprocessing/modular/dat.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.0/preprocessing/modular/data.py` & `proteus_preprocessing-0.4.1/preprocessing/modular/data.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.0/preprocessing/modular/init.py` & `proteus_preprocessing-0.4.1/preprocessing/modular/init.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.0/preprocessing/modular/s.py` & `proteus_preprocessing-0.4.1/preprocessing/modular/s.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.0/preprocessing/utils/expand_dates.py` & `proteus_preprocessing-0.4.1/preprocessing/utils/expand_dates.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.0/preprocessing/utils/expand_wcon.py` & `proteus_preprocessing-0.4.1/preprocessing/utils/expand_wcon.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.0/pyproject.toml` & `proteus_preprocessing-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "proteus-preprocessing"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = []
 packages = [
     { include = "preprocessing/modular" },
     { include = "preprocessing/deck" },
+    { include = "preprocessing/facilities" },
     { include = "preprocessing/utils" },
     { include = "preprocessing/patches.py" },
     { include = "preprocessing/__init__.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `proteus_preprocessing-0.4.0/PKG-INFO` & `proteus_preprocessing-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteus-preprocessing
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

