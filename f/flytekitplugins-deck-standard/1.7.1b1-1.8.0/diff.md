# Comparing `tmp/flytekitplugins-deck-standard-1.7.1b1.tar.gz` & `tmp/flytekitplugins-deck-standard-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-deck-standard-1.7.1b1.tar", last modified: Tue Jun 27 22:00:53 2023, max compression
+gzip compressed data, was "flytekitplugins-deck-standard-1.8.0.tar", last modified: Tue Jul 11 22:07:15 2023, max compression
```

## Comparing `flytekitplugins-deck-standard-1.7.1b1.tar` & `flytekitplugins-deck-standard-1.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:53.520617 flytekitplugins-deck-standard-1.7.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-27 22:00:53.520617 flytekitplugins-deck-standard-1.7.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 22:00:35.000000 flytekitplugins-deck-standard-1.7.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:53.520617 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:53.520617 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-27 22:00:35.000000 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-27 22:00:35.000000 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:53.520617 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins_deck_standard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-27 22:00:53.000000 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins_deck_standard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-27 22:00:53.000000 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins_deck_standard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:53.000000 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins_deck_standard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 22:00:53.000000 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins_deck_standard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:53.000000 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins_deck_standard.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 22:00:53.000000 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins_deck_standard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:53.000000 flytekitplugins-deck-standard-1.7.1b1/flytekitplugins_deck_standard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:53.520617 flytekitplugins-deck-standard-1.7.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-27 22:00:50.000000 flytekitplugins-deck-standard-1.7.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:15.763673 flytekitplugins-deck-standard-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 22:07:15.763673 flytekitplugins-deck-standard-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 22:06:52.000000 flytekitplugins-deck-standard-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:15.763673 flytekitplugins-deck-standard-1.8.0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:15.763673 flytekitplugins-deck-standard-1.8.0/flytekitplugins/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 22:06:52.000000 flytekitplugins-deck-standard-1.8.0/flytekitplugins/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-11 22:06:52.000000 flytekitplugins-deck-standard-1.8.0/flytekitplugins/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:15.763673 flytekitplugins-deck-standard-1.8.0/flytekitplugins_deck_standard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 22:07:15.000000 flytekitplugins-deck-standard-1.8.0/flytekitplugins_deck_standard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 22:07:15.000000 flytekitplugins-deck-standard-1.8.0/flytekitplugins_deck_standard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:15.000000 flytekitplugins-deck-standard-1.8.0/flytekitplugins_deck_standard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 22:07:15.000000 flytekitplugins-deck-standard-1.8.0/flytekitplugins_deck_standard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:15.000000 flytekitplugins-deck-standard-1.8.0/flytekitplugins_deck_standard.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 22:07:15.000000 flytekitplugins-deck-standard-1.8.0/flytekitplugins_deck_standard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:15.000000 flytekitplugins-deck-standard-1.8.0/flytekitplugins_deck_standard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:15.763673 flytekitplugins-deck-standard-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-11 22:07:11.000000 flytekitplugins-deck-standard-1.8.0/setup.py
```

### Comparing `flytekitplugins-deck-standard-1.7.1b1/PKG-INFO` & `flytekitplugins-deck-standard-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-deck-standard
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: This Plugin provides more renderers to improve task visibility
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-deck-standard-1.7.1b1/flytekitplugins/deck/renderer.py` & `flytekitplugins-deck-standard-1.8.0/flytekitplugins/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-deck-standard-1.7.1b1/flytekitplugins_deck_standard.egg-info/PKG-INFO` & `flytekitplugins-deck-standard-1.8.0/flytekitplugins_deck_standard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-deck-standard
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: This Plugin provides more renderers to improve task visibility
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-deck-standard-1.7.1b1/setup.py` & `flytekitplugins-deck-standard-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "deck"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}-standard"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "markdown", "plotly", "ydata-profiling", "ipywidgets"]
 
-__version__ = "1.7.1b1"
+__version__ = "1.8.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This Plugin provides more renderers to improve task visibility",
```

