# Comparing `tmp/tagreader-4.2.2.tar.gz` & `tmp/tagreader-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagreader-4.2.2.tar", max compression
+gzip compressed data, was "tagreader-4.2.3.tar", max compression
```

## Comparing `tagreader-4.2.2.tar` & `tagreader-4.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.2.2/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-15 12:41:41.851734 tagreader-4.2.2/README.md
--rw-r--r--   0        0        0     1633 2023-07-12 09:12:52.054294 tagreader-4.2.2/pyproject.toml
--rw-r--r--   0        0        0      409 2023-07-12 09:12:52.054768 tagreader-4.2.2/tagreader/__init__.py
--rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.2.2/tagreader/__version__.py
--rw-r--r--   0        0        0    11751 2023-07-12 11:36:37.577799 tagreader-4.2.2/tagreader/cache.py
--rw-r--r--   0        0        0    22664 2023-07-12 11:46:17.055904 tagreader-4.2.2/tagreader/clients.py
--rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.2.2/tagreader/logger.py
--rw-r--r--   0        0        0    24973 2023-07-07 07:04:09.640569 tagreader-4.2.2/tagreader/odbc_handlers.py
--rw-r--r--   0        0        0     8193 2023-07-07 07:04:09.641056 tagreader-4.2.2/tagreader/utils.py
--rw-r--r--   0        0        0    32781 2023-07-07 07:04:09.641475 tagreader-4.2.2/tagreader/web_handlers.py
--rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 tagreader-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.2.3/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-15 12:41:41.851734 tagreader-4.2.3/README.md
+-rw-r--r--   0        0        0     1633 2023-07-12 11:49:21.921486 tagreader-4.2.3/pyproject.toml
+-rw-r--r--   0        0        0      409 2023-07-12 09:12:52.054768 tagreader-4.2.3/tagreader/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.2.3/tagreader/__version__.py
+-rw-r--r--   0        0        0    11751 2023-07-12 11:49:21.922116 tagreader-4.2.3/tagreader/cache.py
+-rw-r--r--   0        0        0    22664 2023-07-12 11:49:21.922743 tagreader-4.2.3/tagreader/clients.py
+-rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.2.3/tagreader/logger.py
+-rw-r--r--   0        0        0    24973 2023-07-07 07:04:09.640569 tagreader-4.2.3/tagreader/odbc_handlers.py
+-rw-r--r--   0        0        0     8193 2023-07-07 07:04:09.641056 tagreader-4.2.3/tagreader/utils.py
+-rw-r--r--   0        0        0    32781 2023-07-07 07:04:09.641475 tagreader-4.2.3/tagreader/web_handlers.py
+-rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 tagreader-4.2.3/PKG-INFO
```

### Comparing `tagreader-4.2.2/LICENSE` & `tagreader-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.2/README.md` & `tagreader-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.2/pyproject.toml` & `tagreader-4.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tagreader"
-version = "4.2.2"
+version = "4.2.3"
 description = "Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems."
 authors = ["Einar S. Idsø <eiids@equinor.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tagreader"}]
 keywords=["Aspen InfoPlus.21", "OSIsoft PI"]
 homepage = "https://github.com/equinor/tagreader-python"
```

### Comparing `tagreader-4.2.2/tagreader/cache.py` & `tagreader-4.2.3/tagreader/cache.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.2/tagreader/clients.py` & `tagreader-4.2.3/tagreader/clients.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.2/tagreader/odbc_handlers.py` & `tagreader-4.2.3/tagreader/odbc_handlers.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.2/tagreader/utils.py` & `tagreader-4.2.3/tagreader/utils.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.2/tagreader/web_handlers.py` & `tagreader-4.2.3/tagreader/web_handlers.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.2.2/PKG-INFO` & `tagreader-4.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagreader
-Version: 4.2.2
+Version: 4.2.3
 Summary: Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems.
 Home-page: https://github.com/equinor/tagreader-python
 License: MIT
 Keywords: Aspen InfoPlus.21,OSIsoft PI
 Author: Einar S. Idsø
 Author-email: eiids@equinor.com
 Requires-Python: >=3.8,<4.0
```

