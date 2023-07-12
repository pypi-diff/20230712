# Comparing `tmp/systembridgecli-3.7.0.tar.gz` & `tmp/systembridgecli-3.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgecli-3.7.0.tar", last modified: Wed Jul 12 10:22:37 2023, max compression
+gzip compressed data, was "systembridgecli-3.7.0.dev1.tar", last modified: Mon Jul  3 08:34:21 2023, max compression
```

## Comparing `systembridgecli-3.7.0.tar` & `systembridgecli-3.7.0.dev1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:22:37.384273 systembridgecli-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-12 10:22:37.384273 systembridgecli-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 10:22:24.000000 systembridgecli-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:22:37.384273 systembridgecli-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-12 10:22:24.000000 systembridgecli-3.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:22:37.380273 systembridgecli-3.7.0/systembridgecli/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 10:22:24.000000 systembridgecli-3.7.0/systembridgecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-12 10:22:24.000000 systembridgecli-3.7.0/systembridgecli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-12 10:22:24.000000 systembridgecli-3.7.0/systembridgecli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:22:37.384273 systembridgecli-3.7.0/systembridgecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-12 10:22:37.000000 systembridgecli-3.7.0/systembridgecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-12 10:22:37.000000 systembridgecli-3.7.0/systembridgecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:22:37.000000 systembridgecli-3.7.0/systembridgecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 10:22:37.000000 systembridgecli-3.7.0/systembridgecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 10:22:37.000000 systembridgecli-3.7.0/systembridgecli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:21.088980 systembridgecli-3.7.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 08:34:21.088980 systembridgecli-3.7.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 08:33:59.000000 systembridgecli-3.7.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:34:21.088980 systembridgecli-3.7.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-03 08:33:59.000000 systembridgecli-3.7.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:21.088980 systembridgecli-3.7.0.dev1/systembridgecli/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 08:33:59.000000 systembridgecli-3.7.0.dev1/systembridgecli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-03 08:33:59.000000 systembridgecli-3.7.0.dev1/systembridgecli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-03 08:34:19.000000 systembridgecli-3.7.0.dev1/systembridgecli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:21.088980 systembridgecli-3.7.0.dev1/systembridgecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 08:34:21.000000 systembridgecli-3.7.0.dev1/systembridgecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-03 08:34:21.000000 systembridgecli-3.7.0.dev1/systembridgecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:34:21.000000 systembridgecli-3.7.0.dev1/systembridgecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 08:34:21.000000 systembridgecli-3.7.0.dev1/systembridgecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 08:34:21.000000 systembridgecli-3.7.0.dev1/systembridgecli.egg-info/top_level.txt
```

### Comparing `systembridgecli-3.7.0/pyproject.toml` & `systembridgecli-3.7.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgecli-3.7.0/setup.py` & `systembridgecli-3.7.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgecli-3.7.0/systembridgecli/__main__.py` & `systembridgecli-3.7.0.dev1/systembridgecli/__main__.py`

 * *Files identical despite different names*

