# Comparing `tmp/dpmt-1.0.2.tar.gz` & `tmp/dpmt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpmt-1.0.2.tar", last modified: Wed Jul 12 08:10:03 2023, max compression
+gzip compressed data, was "dpmt-1.0.3.tar", last modified: Wed Jul 12 08:11:58 2023, max compression
```

## Comparing `dpmt-1.0.2.tar` & `dpmt-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:10:03.547174 dpmt-1.0.2/
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2814 2023-07-12 08:10:03.547174 dpmt-1.0.2/PKG-INFO
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2348 2023-07-12 07:27:40.000000 dpmt-1.0.2/README.md
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      647 2023-07-12 08:09:33.000000 dpmt-1.0.2/pyproject.toml
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       38 2023-07-12 08:10:03.547174 dpmt-1.0.2/setup.cfg
-drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:10:03.543174 dpmt-1.0.2/src/
-drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:10:03.546174 dpmt-1.0.2/src/dpm/
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      143 2023-07-10 16:32:49.000000 dpmt-1.0.2/src/dpm/Colours.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     1697 2023-07-08 09:34:21.000000 dpmt-1.0.2/src/dpm/Menu.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     5776 2023-07-10 16:32:54.000000 dpmt-1.0.2/src/dpm/browse_library.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       92 2023-07-10 16:20:57.000000 dpmt-1.0.2/src/dpm/client.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       81 2023-07-08 09:41:05.000000 dpmt-1.0.2/src/dpm/cs.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     7031 2023-07-12 06:32:13.000000 dpmt-1.0.2/src/dpm/currently_playing.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      259 2023-07-10 16:33:18.000000 dpmt-1.0.2/src/dpm/info_panel.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2560 2023-07-12 05:18:08.000000 dpmt-1.0.2/src/dpm/main.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      991 2023-07-10 14:53:13.000000 dpmt-1.0.2/src/dpm/playlist.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     5262 2023-07-10 16:34:06.000000 dpmt-1.0.2/src/dpm/playlist_opt.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     3709 2023-07-10 16:34:47.000000 dpmt-1.0.2/src/dpm/search.py
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      218 2023-07-12 05:53:50.000000 dpmt-1.0.2/src/dpm/shuffle.py
-drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:10:03.547174 dpmt-1.0.2/src/dpmt.egg-info/
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2814 2023-07-12 08:10:03.000000 dpmt-1.0.2/src/dpmt.egg-info/PKG-INFO
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      459 2023-07-12 08:10:03.000000 dpmt-1.0.2/src/dpmt.egg-info/SOURCES.txt
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)        1 2023-07-12 08:10:03.000000 dpmt-1.0.2/src/dpmt.egg-info/dependency_links.txt
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       43 2023-07-12 08:10:03.000000 dpmt-1.0.2/src/dpmt.egg-info/entry_points.txt
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       17 2023-07-12 08:10:03.000000 dpmt-1.0.2/src/dpmt.egg-info/requires.txt
--rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)        4 2023-07-12 08:10:03.000000 dpmt-1.0.2/src/dpmt.egg-info/top_level.txt
+drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:11:58.822172 dpmt-1.0.3/
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2814 2023-07-12 08:11:58.822172 dpmt-1.0.3/PKG-INFO
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2348 2023-07-12 07:27:40.000000 dpmt-1.0.3/README.md
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      647 2023-07-12 08:11:49.000000 dpmt-1.0.3/pyproject.toml
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       38 2023-07-12 08:11:58.822172 dpmt-1.0.3/setup.cfg
+drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:11:58.818172 dpmt-1.0.3/src/
+drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:11:58.820172 dpmt-1.0.3/src/dpm/
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      143 2023-07-10 16:32:49.000000 dpmt-1.0.3/src/dpm/Colours.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     1697 2023-07-08 09:34:21.000000 dpmt-1.0.3/src/dpm/Menu.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     5776 2023-07-10 16:32:54.000000 dpmt-1.0.3/src/dpm/browse_library.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       92 2023-07-10 16:20:57.000000 dpmt-1.0.3/src/dpm/client.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       81 2023-07-08 09:41:05.000000 dpmt-1.0.3/src/dpm/cs.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     7031 2023-07-12 06:32:13.000000 dpmt-1.0.3/src/dpm/currently_playing.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      259 2023-07-10 16:33:18.000000 dpmt-1.0.3/src/dpm/info_panel.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2560 2023-07-12 05:18:08.000000 dpmt-1.0.3/src/dpm/main.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      991 2023-07-10 14:53:13.000000 dpmt-1.0.3/src/dpm/playlist.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     5262 2023-07-10 16:34:06.000000 dpmt-1.0.3/src/dpm/playlist_opt.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     3709 2023-07-10 16:34:47.000000 dpmt-1.0.3/src/dpm/search.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      218 2023-07-12 05:53:50.000000 dpmt-1.0.3/src/dpm/shuffle.py
+drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:11:58.821172 dpmt-1.0.3/src/dpmt.egg-info/
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2814 2023-07-12 08:11:58.000000 dpmt-1.0.3/src/dpmt.egg-info/PKG-INFO
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      459 2023-07-12 08:11:58.000000 dpmt-1.0.3/src/dpmt.egg-info/SOURCES.txt
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)        1 2023-07-12 08:11:58.000000 dpmt-1.0.3/src/dpmt.egg-info/dependency_links.txt
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       43 2023-07-12 08:11:58.000000 dpmt-1.0.3/src/dpmt.egg-info/entry_points.txt
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       17 2023-07-12 08:11:58.000000 dpmt-1.0.3/src/dpmt.egg-info/requires.txt
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)        4 2023-07-12 08:11:58.000000 dpmt-1.0.3/src/dpmt.egg-info/top_level.txt
```

### Comparing `dpmt-1.0.2/PKG-INFO` & `dpmt-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpmt
-Version: 1.0.2
+Version: 1.0.3
 Summary: TUI frontend for MPD
 Author-email: Shayan Naqvi <shayan.naqvi@icloud.com>
 Project-URL: Homepage, https://github.com/shayanaqvi/dpm
 Project-URL: Bug Tracker, https://github.com/shayanaqvi/dpm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dpmt-1.0.2/README.md` & `dpmt-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dpmt-1.0.2/pyproject.toml` & `dpmt-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpmt"
-version = "1.0.2"
+version = "1.0.3"
 dependencies = [
   "rich",
   "python-mpd2"
 ]
 authors = [
   { name="Shayan Naqvi", email="shayan.naqvi@icloud.com" },
 ]
```

### Comparing `dpmt-1.0.2/src/dpm/Menu.py` & `dpmt-1.0.3/src/dpm/Menu.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0.2/src/dpm/browse_library.py` & `dpmt-1.0.3/src/dpm/browse_library.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0.2/src/dpm/currently_playing.py` & `dpmt-1.0.3/src/dpm/currently_playing.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0.2/src/dpm/main.py` & `dpmt-1.0.3/src/dpm/main.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0.2/src/dpm/playlist.py` & `dpmt-1.0.3/src/dpm/playlist.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0.2/src/dpm/playlist_opt.py` & `dpmt-1.0.3/src/dpm/playlist_opt.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0.2/src/dpm/search.py` & `dpmt-1.0.3/src/dpm/search.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0.2/src/dpmt.egg-info/PKG-INFO` & `dpmt-1.0.3/src/dpmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpmt
-Version: 1.0.2
+Version: 1.0.3
 Summary: TUI frontend for MPD
 Author-email: Shayan Naqvi <shayan.naqvi@icloud.com>
 Project-URL: Homepage, https://github.com/shayanaqvi/dpm
 Project-URL: Bug Tracker, https://github.com/shayanaqvi/dpm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

