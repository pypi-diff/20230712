# Comparing `tmp/hyprshade-0.1.2.tar.gz` & `tmp/hyprshade-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.1.2.tar", max compression
+gzip compressed data, was "hyprshade-0.2.0.tar", max compression
```

## Comparing `hyprshade-0.1.2.tar` & `hyprshade-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.1.2/LICENSE
--rw-r--r--   0        0        0       44 2023-07-05 23:37:20.434170 hyprshade-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-10 23:35:03.452541 hyprshade-0.1.2/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.1.2/hyprshade/__main__.py
--rw-r--r--   0        0        0     2577 2023-07-11 08:22:08.168519 hyprshade-0.1.2/hyprshade/cli.py
--rw-r--r--   0        0        0     3349 2023-07-11 12:47:30.057291 hyprshade-0.1.2/hyprshade/config.py
--rw-r--r--   0        0        0      956 2023-07-11 02:46:20.738707 hyprshade-0.1.2/hyprshade/helpers.py
--rw-r--r--   0        0        0      808 2023-07-10 06:55:45.350472 hyprshade-0.1.2/hyprshade/utils.py
--rw-r--r--   0        0        0     1002 2023-07-11 12:52:04.437286 hyprshade-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 hyprshade-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.2.0/LICENSE
+-rw-r--r--   0        0        0      719 2023-07-12 02:33:48.487461 hyprshade-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 23:35:03.452541 hyprshade-0.2.0/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.2.0/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2577 2023-07-11 08:22:08.168519 hyprshade-0.2.0/hyprshade/cli.py
+-rw-r--r--   0        0        0     3349 2023-07-11 12:47:30.057291 hyprshade-0.2.0/hyprshade/config.py
+-rw-r--r--   0        0        0      956 2023-07-11 02:46:20.738707 hyprshade-0.2.0/hyprshade/helpers.py
+-rw-r--r--   0        0        0      808 2023-07-10 06:55:45.350472 hyprshade-0.2.0/hyprshade/utils.py
+-rw-r--r--   0        0        0     1024 2023-07-12 02:50:48.862355 hyprshade-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.2.0/shaders/blue-light-filter.glsl
+-rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.2.0/shaders/vibrance.glsl
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 hyprshade-0.2.0/PKG-INFO
```

### Comparing `hyprshade-0.1.2/LICENSE` & `hyprshade-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.2/hyprshade/cli.py` & `hyprshade-0.2.0/hyprshade/cli.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.2/hyprshade/config.py` & `hyprshade-0.2.0/hyprshade/config.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.2/hyprshade/helpers.py` & `hyprshade-0.2.0/hyprshade/helpers.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.2/hyprshade/utils.py` & `hyprshade-0.2.0/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.1.2/pyproject.toml` & `hyprshade-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
+include = ["shaders"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typer = { extras = ["all"], version = "^0.9.0" }
 more-itertools = "^9.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

