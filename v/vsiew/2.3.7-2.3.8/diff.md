# Comparing `tmp/vsiew-2.3.7.tar.gz` & `tmp/vsiew-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.3.7.tar", last modified: Tue Jun 27 17:16:31 2023, max compression
+gzip compressed data, was "vsiew-2.3.8.tar", last modified: Wed Jul 12 16:22:14 2023, max compression
```

## Comparing `vsiew-2.3.7.tar` & `vsiew-2.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:31.038188 vsiew-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-27 17:16:09.000000 vsiew-2.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 17:16:31.038188 vsiew-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 17:16:09.000000 vsiew-2.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:16:31.038188 vsiew-2.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 17:16:09.000000 vsiew-2.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:31.038188 vsiew-2.3.7/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-27 17:16:09.000000 vsiew-2.3.7/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 17:16:09.000000 vsiew-2.3.7/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-27 17:16:09.000000 vsiew-2.3.7/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-27 17:16:09.000000 vsiew-2.3.7/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:31.038188 vsiew-2.3.7/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 17:16:31.000000 vsiew-2.3.7/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:22:14.186871 vsiew-2.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-12 16:21:46.000000 vsiew-2.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-12 16:22:14.186871 vsiew-2.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-12 16:21:46.000000 vsiew-2.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:22:14.186871 vsiew-2.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-12 16:21:46.000000 vsiew-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:22:14.182871 vsiew-2.3.8/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-12 16:21:46.000000 vsiew-2.3.8/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 16:21:46.000000 vsiew-2.3.8/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 16:21:46.000000 vsiew-2.3.8/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-12 16:21:46.000000 vsiew-2.3.8/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:22:14.186871 vsiew-2.3.8/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-12 16:22:14.000000 vsiew-2.3.8/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-12 16:22:14.000000 vsiew-2.3.8/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:22:14.000000 vsiew-2.3.8/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 16:22:14.000000 vsiew-2.3.8/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-12 16:22:14.000000 vsiew-2.3.8/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 16:22:14.000000 vsiew-2.3.8/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.3.7/LICENSE` & `vsiew-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.7/PKG-INFO` & `vsiew-2.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.7
+Version: 2.3.8
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.3.7/setup.py` & `vsiew-2.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.7/vsiew/__init__.py` & `vsiew-2.3.8/vsiew/__init__.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.7/vsiew/init.py` & `vsiew-2.3.8/vsiew/init.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.7/vsiew.egg-info/PKG-INFO` & `vsiew-2.3.8/vsiew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.7
+Version: 2.3.8
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

