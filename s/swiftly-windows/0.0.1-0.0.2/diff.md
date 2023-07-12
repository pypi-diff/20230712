# Comparing `tmp/swiftly-windows-0.0.1.tar.gz` & `tmp/swiftly-windows-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-windows-0.0.1.tar", last modified: Wed Jul 12 20:30:28 2023, max compression
+gzip compressed data, was "swiftly-windows-0.0.2.tar", last modified: Wed Jul 12 20:44:55 2023, max compression
```

## Comparing `swiftly-windows-0.0.1.tar` & `swiftly-windows-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 20:30:28.079617 swiftly-windows-0.0.1/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-windows-0.0.1/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-12 20:30:28.079460 swiftly-windows-0.0.1/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 20:30:28.079702 swiftly-windows-0.0.1/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      165 2023-07-12 20:30:20.000000 swiftly-windows-0.0.1/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 20:30:28.078706 swiftly-windows-0.0.1/swiftly_windows/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-windows-0.0.1/swiftly_windows/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-windows-0.0.1/swiftly_windows/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-windows-0.0.1/swiftly_windows/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3299 2023-07-12 20:26:17.000000 swiftly-windows-0.0.1/swiftly_windows/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2172 2023-07-12 20:26:17.000000 swiftly-windows-0.0.1/swiftly_windows/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-windows-0.0.1/swiftly_windows/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 20:30:28.079279 swiftly-windows-0.0.1/swiftly_windows.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-12 20:30:28.000000 swiftly-windows-0.0.1/swiftly_windows.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      332 2023-07-12 20:30:28.000000 swiftly-windows-0.0.1/swiftly_windows.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 20:30:28.000000 swiftly-windows-0.0.1/swiftly_windows.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       16 2023-07-12 20:30:28.000000 swiftly-windows-0.0.1/swiftly_windows.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 20:44:55.732543 swiftly-windows-0.0.2/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-windows-0.0.2/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-12 20:44:55.732400 swiftly-windows-0.0.2/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 20:44:55.730420 swiftly-windows-0.0.2/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     7673 2023-07-12 20:27:39.000000 swiftly-windows-0.0.2/scripts/swiftly.ps1
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 20:44:55.732585 swiftly-windows-0.0.2/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      169 2023-07-12 20:44:48.000000 swiftly-windows-0.0.2/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 20:44:55.731712 swiftly-windows-0.0.2/swiftly_windows/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-windows-0.0.2/swiftly_windows/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-windows-0.0.2/swiftly_windows/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-windows-0.0.2/swiftly_windows/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3299 2023-07-12 20:26:17.000000 swiftly-windows-0.0.2/swiftly_windows/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2172 2023-07-12 20:26:17.000000 swiftly-windows-0.0.2/swiftly_windows/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-windows-0.0.2/swiftly_windows/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 20:44:55.732230 swiftly-windows-0.0.2/swiftly_windows.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-12 20:44:55.000000 swiftly-windows-0.0.2/swiftly_windows.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      352 2023-07-12 20:44:55.000000 swiftly-windows-0.0.2/swiftly_windows.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 20:44:55.000000 swiftly-windows-0.0.2/swiftly_windows.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       16 2023-07-12 20:44:55.000000 swiftly-windows-0.0.2/swiftly_windows.egg-info/top_level.txt
```

### Comparing `swiftly-windows-0.0.1/LICENSE` & `swiftly-windows-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-windows-0.0.1/swiftly_windows/gitignore.py` & `swiftly-windows-0.0.2/swiftly_windows/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-windows-0.0.1/swiftly_windows/init.py` & `swiftly-windows-0.0.2/swiftly_windows/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-windows-0.0.1/swiftly_windows/makeapp.py` & `swiftly-windows-0.0.2/swiftly_windows/makeapp.py`

 * *Files identical despite different names*

