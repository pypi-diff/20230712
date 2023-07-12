# Comparing `tmp/systembridgegui-3.7.0.tar.gz` & `tmp/systembridgegui-3.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgegui-3.7.0.tar", last modified: Wed Jul 12 10:23:58 2023, max compression
+gzip compressed data, was "systembridgegui-3.7.0.dev1.tar", last modified: Mon Jul  3 08:35:32 2023, max compression
```

## Comparing `systembridgegui-3.7.0.tar` & `systembridgegui-3.7.0.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:58.568795 systembridgegui-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-12 10:23:58.568795 systembridgegui-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:23:58.568795 systembridgegui-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:58.564795 systembridgegui-3.7.0/systembridgegui/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/system_tray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:58.564795 systembridgegui-3.7.0/systembridgegui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/widgets/timed_message_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:58.564795 systembridgegui-3.7.0/systembridgegui/window/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/window/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/window/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-12 10:23:37.000000 systembridgegui-3.7.0/systembridgegui/window/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:23:58.564795 systembridgegui-3.7.0/systembridgegui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-12 10:23:58.000000 systembridgegui-3.7.0/systembridgegui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-12 10:23:58.000000 systembridgegui-3.7.0/systembridgegui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:23:58.000000 systembridgegui-3.7.0/systembridgegui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 10:23:58.000000 systembridgegui-3.7.0/systembridgegui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 10:23:58.000000 systembridgegui-3.7.0/systembridgegui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.581477 systembridgegui-3.7.0.dev1/systembridgegui/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-03 08:35:30.000000 systembridgegui-3.7.0.dev1/systembridgegui/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/system_tray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/systembridgegui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/widgets/timed_message_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/systembridgegui/window/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/window/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/window/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/window/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/top_level.txt
```

### Comparing `systembridgegui-3.7.0/pyproject.toml` & `systembridgegui-3.7.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0/setup.py` & `systembridgegui-3.7.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0/systembridgegui/__main__.py` & `systembridgegui-3.7.0.dev1/systembridgegui/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0/systembridgegui/icon.png` & `systembridgegui-3.7.0.dev1/systembridgegui/icon.png`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0/systembridgegui/system_tray.py` & `systembridgegui-3.7.0.dev1/systembridgegui/system_tray.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0/systembridgegui/widgets/timed_message_box.py` & `systembridgegui-3.7.0.dev1/systembridgegui/widgets/timed_message_box.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0/systembridgegui/window/main.py` & `systembridgegui-3.7.0.dev1/systembridgegui/window/main.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0/systembridgegui/window/notification.py` & `systembridgegui-3.7.0.dev1/systembridgegui/window/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0/systembridgegui/window/player.py` & `systembridgegui-3.7.0.dev1/systembridgegui/window/player.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0/systembridgegui.egg-info/SOURCES.txt` & `systembridgegui-3.7.0.dev1/systembridgegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

