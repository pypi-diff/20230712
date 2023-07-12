# Comparing `tmp/dpmt-1.0.tar.gz` & `tmp/dpmt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "dpmt-1.0.1.tar", last modified: Wed Jul 12 08:07:38 2023, max compression
```

## Comparing `dpmt-1.0.tar` & `dpmt-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 dpmt-1.0/LISENCE
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/Colours.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/Menu.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/TODO.md
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/browse_library.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/client.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/cs.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/currently_playing.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/info_panel.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/main.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/playlist.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/playlist_opt.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/search.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/shuffle.py
--rw-r--r--   0        0        0  1019851 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/screenshots/browse_albums.png
--rw-r--r--   0        0        0   991599 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/screenshots/browse_artist.png
--rw-r--r--   0        0        0   926646 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/screenshots/browse_title.png
--rw-r--r--   0        0        0  1205757 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/screenshots/currently_playing.png
--rw-r--r--   0        0        0   884329 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/screenshots/main_menu.png
--rw-r--r--   0        0        0   895950 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/screenshots/playlist_options.png
--rw-r--r--   0        0        0  1281334 2020-02-02 00:00:00.000000 dpmt-1.0/src/dpm/screenshots/search_results.png
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 dpmt-1.0/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 dpmt-1.0/pyproject.toml
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 dpmt-1.0/PKG-INFO
+drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:07:38.327177 dpmt-1.0.1/
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2813 2023-07-12 08:07:38.327177 dpmt-1.0.1/PKG-INFO
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2348 2023-07-12 07:27:40.000000 dpmt-1.0.1/README.md
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      641 2023-07-12 08:07:23.000000 dpmt-1.0.1/pyproject.toml
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       38 2023-07-12 08:07:38.327177 dpmt-1.0.1/setup.cfg
+drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:07:38.323177 dpmt-1.0.1/src/
+drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:07:38.326177 dpmt-1.0.1/src/dpm/
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      143 2023-07-10 16:32:49.000000 dpmt-1.0.1/src/dpm/Colours.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     1697 2023-07-08 09:34:21.000000 dpmt-1.0.1/src/dpm/Menu.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     5776 2023-07-10 16:32:54.000000 dpmt-1.0.1/src/dpm/browse_library.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       92 2023-07-10 16:20:57.000000 dpmt-1.0.1/src/dpm/client.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       81 2023-07-08 09:41:05.000000 dpmt-1.0.1/src/dpm/cs.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     7031 2023-07-12 06:32:13.000000 dpmt-1.0.1/src/dpm/currently_playing.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      259 2023-07-10 16:33:18.000000 dpmt-1.0.1/src/dpm/info_panel.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2560 2023-07-12 05:18:08.000000 dpmt-1.0.1/src/dpm/main.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      991 2023-07-10 14:53:13.000000 dpmt-1.0.1/src/dpm/playlist.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     5262 2023-07-10 16:34:06.000000 dpmt-1.0.1/src/dpm/playlist_opt.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     3709 2023-07-10 16:34:47.000000 dpmt-1.0.1/src/dpm/search.py
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      218 2023-07-12 05:53:50.000000 dpmt-1.0.1/src/dpm/shuffle.py
+drwxr-xr-x   0 shayanaqvi  (1000) shayanaqvi  (1000)        0 2023-07-12 08:07:38.327177 dpmt-1.0.1/src/dpmt.egg-info/
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)     2813 2023-07-12 08:07:38.000000 dpmt-1.0.1/src/dpmt.egg-info/PKG-INFO
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)      459 2023-07-12 08:07:38.000000 dpmt-1.0.1/src/dpmt.egg-info/SOURCES.txt
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)        1 2023-07-12 08:07:38.000000 dpmt-1.0.1/src/dpmt.egg-info/dependency_links.txt
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       38 2023-07-12 08:07:38.000000 dpmt-1.0.1/src/dpmt.egg-info/entry_points.txt
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)       17 2023-07-12 08:07:38.000000 dpmt-1.0.1/src/dpmt.egg-info/requires.txt
+-rw-r--r--   0 shayanaqvi  (1000) shayanaqvi  (1000)        4 2023-07-12 08:07:38.000000 dpmt-1.0.1/src/dpmt.egg-info/top_level.txt
```

### Comparing `dpmt-1.0/src/dpm/Menu.py` & `dpmt-1.0.1/src/dpm/Menu.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0/src/dpm/browse_library.py` & `dpmt-1.0.1/src/dpm/browse_library.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0/src/dpm/currently_playing.py` & `dpmt-1.0.1/src/dpm/currently_playing.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0/src/dpm/main.py` & `dpmt-1.0.1/src/dpm/main.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0/src/dpm/playlist.py` & `dpmt-1.0.1/src/dpm/playlist.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0/src/dpm/playlist_opt.py` & `dpmt-1.0.1/src/dpm/playlist_opt.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0/src/dpm/search.py` & `dpmt-1.0.1/src/dpm/search.py`

 * *Files identical despite different names*

### Comparing `dpmt-1.0/README.md` & `dpmt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dpmt-1.0/PKG-INFO` & `dpmt-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dpmt
-Version: 1.0
+Version: 1.0.1
 Summary: TUI frontend for MPD
+Author-email: Shayan Naqvi <shayan.naqvi@icloud.com>
 Project-URL: Homepage, https://github.com/shayanaqvi/dpm
 Project-URL: Bug Tracker, https://github.com/shayanaqvi/dpm/issues
-Author-email: Shayan Naqvi <shayan.naqvi@icloud.com>
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # dpm
 dpm is a TUI frontend to MPD
 ## Features
 The feature set, at present, is somewhat limited. Right now, it can:
```

