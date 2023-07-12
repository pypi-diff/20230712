# Comparing `tmp/lcwc-0.7.tar.gz` & `tmp/lcwc-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcwc-0.7.tar", last modified: Sun Jul  9 20:05:33 2023, max compression
+gzip compressed data, was "lcwc-0.8.tar", last modified: Wed Jul 12 15:51:20 2023, max compression
```

## Comparing `lcwc-0.7.tar` & `lcwc-0.8.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.259806 lcwc-0.7/
--rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.7/LICENSE
--rw-rw-rw-   0        0        0     2325 2023-07-09 20:05:33.259306 lcwc-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1671 2023-06-10 14:58:54.000000 lcwc-0.7/README.md
--rw-rw-rw-   0        0        0      802 2023-07-09 20:05:21.000000 lcwc-0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-09 20:05:33.260306 lcwc-0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.215306 lcwc-0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.233306 lcwc-0.7/src/lcwc/
--rw-rw-rw-   0        0        0      124 2023-07-09 20:01:56.000000 lcwc-0.7/src/lcwc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.243308 lcwc-0.7/src/lcwc/arcgis/
--rw-rw-rw-   0        0        0       72 2023-06-30 18:00:38.000000 lcwc-0.7/src/lcwc/arcgis/__init__.py
--rw-rw-rw-   0        0        0     6502 2023-07-09 20:01:56.000000 lcwc-0.7/src/lcwc/arcgis/client.py
--rw-rw-rw-   0        0        0      769 2023-07-07 07:11:12.000000 lcwc-0.7/src/lcwc/arcgis/incident.py
--rw-rw-rw-   0        0        0      326 2023-06-24 14:32:45.000000 lcwc-0.7/src/lcwc/category.py
--rw-rw-rw-   0        0        0      318 2023-06-30 18:02:43.000000 lcwc-0.7/src/lcwc/client.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.246306 lcwc-0.7/src/lcwc/feed/
--rw-rw-rw-   0        0        0       68 2023-06-30 17:57:06.000000 lcwc-0.7/src/lcwc/feed/__init__.py
--rw-rw-rw-   0        0        0     4468 2023-06-30 18:37:18.000000 lcwc-0.7/src/lcwc/feed/client.py
--rw-rw-rw-   0        0        0      241 2023-07-05 13:46:18.000000 lcwc-0.7/src/lcwc/feed/incident.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.248806 lcwc-0.7/src/lcwc/feed/utils/
--rw-rw-rw-   0        0        0     2373 2023-06-30 18:38:10.000000 lcwc-0.7/src/lcwc/feed/utils/__init__.py
--rw-rw-rw-   0        0        0      651 2023-07-01 15:08:06.000000 lcwc-0.7/src/lcwc/incident.py
--rw-rw-rw-   0        0        0      330 2023-07-09 20:02:44.000000 lcwc-0.7/src/lcwc/unit.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.253308 lcwc-0.7/src/lcwc/utils/
--rw-rw-rw-   0        0        0      668 2023-07-09 06:50:55.000000 lcwc-0.7/src/lcwc/utils/__init__.py
--rw-rw-rw-   0        0        0     1737 2023-07-07 07:17:11.000000 lcwc-0.7/src/lcwc/utils/encoding.py
--rw-rw-rw-   0        0        0     4286 2023-07-05 15:08:28.000000 lcwc-0.7/src/lcwc/utils/restadapter.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.258306 lcwc-0.7/src/lcwc/web/
--rw-rw-rw-   0        0        0       64 2023-06-30 17:55:06.000000 lcwc-0.7/src/lcwc/web/__init__.py
--rw-rw-rw-   0        0        0     3972 2023-06-30 18:34:22.000000 lcwc-0.7/src/lcwc/web/client.py
--rw-rw-rw-   0        0        0      232 2023-06-30 20:31:48.000000 lcwc-0.7/src/lcwc/web/incident.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.239806 lcwc-0.7/src/lcwc.egg-info/
--rw-rw-rw-   0        0        0     2325 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      637 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 15:51:20.619824 lcwc-0.8/
+-rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.8/LICENSE
+-rw-rw-rw-   0        0        0     2325 2023-07-12 15:51:20.619323 lcwc-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1671 2023-06-10 14:58:54.000000 lcwc-0.8/README.md
+-rw-rw-rw-   0        0        0      802 2023-07-12 15:51:11.000000 lcwc-0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:51:20.619824 lcwc-0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 15:51:20.523824 lcwc-0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 15:51:20.576823 lcwc-0.8/src/lcwc/
+-rw-rw-rw-   0        0        0      192 2023-07-12 15:14:30.000000 lcwc-0.8/src/lcwc/__init__.py
+-rw-rw-rw-   0        0        0      849 2023-07-12 15:14:30.000000 lcwc-0.8/src/lcwc/agency.py
+-rw-rw-rw-   0        0        0     4011 2023-07-12 15:14:30.000000 lcwc-0.8/src/lcwc/agencyclient.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:51:20.602323 lcwc-0.8/src/lcwc/arcgis/
+-rw-rw-rw-   0        0        0       72 2023-06-30 18:00:38.000000 lcwc-0.8/src/lcwc/arcgis/__init__.py
+-rw-rw-rw-   0        0        0     6502 2023-07-12 15:13:32.000000 lcwc-0.8/src/lcwc/arcgis/client.py
+-rw-rw-rw-   0        0        0      769 2023-07-07 07:11:12.000000 lcwc-0.8/src/lcwc/arcgis/incident.py
+-rw-rw-rw-   0        0        0      326 2023-06-24 14:32:45.000000 lcwc-0.8/src/lcwc/category.py
+-rw-rw-rw-   0        0        0      318 2023-06-30 18:02:43.000000 lcwc-0.8/src/lcwc/client.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:51:20.606323 lcwc-0.8/src/lcwc/feed/
+-rw-rw-rw-   0        0        0       68 2023-06-30 17:57:06.000000 lcwc-0.8/src/lcwc/feed/__init__.py
+-rw-rw-rw-   0        0        0     4468 2023-06-30 18:37:18.000000 lcwc-0.8/src/lcwc/feed/client.py
+-rw-rw-rw-   0        0        0      241 2023-07-05 13:46:18.000000 lcwc-0.8/src/lcwc/feed/incident.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:51:20.607324 lcwc-0.8/src/lcwc/feed/utils/
+-rw-rw-rw-   0        0        0     2373 2023-06-30 18:38:10.000000 lcwc-0.8/src/lcwc/feed/utils/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-07-01 15:08:06.000000 lcwc-0.8/src/lcwc/incident.py
+-rw-rw-rw-   0        0        0      330 2023-07-09 20:02:44.000000 lcwc-0.8/src/lcwc/unit.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:51:20.612823 lcwc-0.8/src/lcwc/utils/
+-rw-rw-rw-   0        0        0     2598 2023-07-12 15:14:30.000000 lcwc-0.8/src/lcwc/utils/__init__.py
+-rw-rw-rw-   0        0        0     1737 2023-07-07 07:17:11.000000 lcwc-0.8/src/lcwc/utils/encoding.py
+-rw-rw-rw-   0        0        0     4286 2023-07-05 15:08:28.000000 lcwc-0.8/src/lcwc/utils/restadapter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:51:20.618323 lcwc-0.8/src/lcwc/web/
+-rw-rw-rw-   0        0        0       64 2023-06-30 17:55:06.000000 lcwc-0.8/src/lcwc/web/__init__.py
+-rw-rw-rw-   0        0        0     3972 2023-06-30 18:34:22.000000 lcwc-0.8/src/lcwc/web/client.py
+-rw-rw-rw-   0        0        0      232 2023-06-30 20:31:48.000000 lcwc-0.8/src/lcwc/web/incident.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:51:20.593823 lcwc-0.8/src/lcwc.egg-info/
+-rw-rw-rw-   0        0        0     2325 2023-07-12 15:51:20.000000 lcwc-0.8/src/lcwc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-07-12 15:51:20.000000 lcwc-0.8/src/lcwc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:51:20.000000 lcwc-0.8/src/lcwc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-12 15:51:20.000000 lcwc-0.8/src/lcwc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 15:51:20.000000 lcwc-0.8/src/lcwc.egg-info/top_level.txt
```

### Comparing `lcwc-0.7/LICENSE` & `lcwc-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/PKG-INFO` & `lcwc-0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.7
+Version: 0.8
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lcwc-0.7/README.md` & `lcwc-0.8/README.md`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/pyproject.toml` & `lcwc-0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lcwc"
-version = "0.7"
+version = "0.8"
 authors = [
   { name="Nate Shoffner", email="nate.shoffner@gmail.com" },
 ]
 description = "Python library for fetching the Lancaster County-Wide Communications live incident list."
 keywords = ["lcwc", "lancaster", "police", "fire", "ems", "dispatch", "911", "incident"]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `lcwc-0.7/src/lcwc/arcgis/client.py` & `lcwc-0.8/src/lcwc/arcgis/client.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/src/lcwc/arcgis/incident.py` & `lcwc-0.8/src/lcwc/arcgis/incident.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/src/lcwc/feed/client.py` & `lcwc-0.8/src/lcwc/feed/client.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/src/lcwc/feed/utils/__init__.py` & `lcwc-0.8/src/lcwc/feed/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/src/lcwc/incident.py` & `lcwc-0.8/src/lcwc/incident.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/src/lcwc/utils/encoding.py` & `lcwc-0.8/src/lcwc/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/src/lcwc/utils/restadapter.py` & `lcwc-0.8/src/lcwc/utils/restadapter.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/src/lcwc/web/client.py` & `lcwc-0.8/src/lcwc/web/client.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.7/src/lcwc.egg-info/PKG-INFO` & `lcwc-0.8/src/lcwc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.7
+Version: 0.8
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lcwc-0.7/src/lcwc.egg-info/SOURCES.txt` & `lcwc-0.8/src/lcwc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 src/lcwc/__init__.py
+src/lcwc/agency.py
+src/lcwc/agencyclient.py
 src/lcwc/category.py
 src/lcwc/client.py
 src/lcwc/incident.py
 src/lcwc/unit.py
 src/lcwc.egg-info/PKG-INFO
 src/lcwc.egg-info/SOURCES.txt
 src/lcwc.egg-info/dependency_links.txt
```

