# Comparing `tmp/elody-0.0.6.tar.gz` & `tmp/elody-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elody-0.0.6.tar", last modified: Wed Jul 12 09:19:21 2023, max compression
+gzip compressed data, was "elody-0.0.7.tar", last modified: Wed Jul 12 10:02:15 2023, max compression
```

## Comparing `elody-0.0.6.tar` & `elody-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:19:21.605870 elody-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 09:19:06.000000 elody-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 09:19:21.605870 elody-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 09:19:06.000000 elody-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 09:19:06.000000 elody-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:19:21.605870 elody-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:19:21.601870 elody-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:19:21.601870 elody-0.0.6/src/elody/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:19:21.601870 elody-0.0.6/src/elody.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:02:15.411821 elody-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 10:02:01.000000 elody-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 10:02:15.411821 elody-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 10:02:01.000000 elody-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 10:02:01.000000 elody-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:02:15.411821 elody-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:02:15.411821 elody-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:02:15.411821 elody-0.0.7/src/elody/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 10:02:01.000000 elody-0.0.7/src/elody/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-12 10:02:01.000000 elody-0.0.7/src/elody/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 10:02:01.000000 elody-0.0.7/src/elody/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-12 10:02:01.000000 elody-0.0.7/src/elody/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-12 10:02:01.000000 elody-0.0.7/src/elody/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:02:15.411821 elody-0.0.7/src/elody.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 10:02:15.000000 elody-0.0.7/src/elody.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 10:02:15.000000 elody-0.0.7/src/elody.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:02:15.000000 elody-0.0.7/src/elody.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 10:02:15.000000 elody-0.0.7/src/elody.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 10:02:15.000000 elody-0.0.7/src/elody.egg-info/top_level.txt
```

### Comparing `elody-0.0.6/LICENSE` & `elody-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `elody-0.0.6/PKG-INFO` & `elody-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.6
+Version: 0.0.7
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `elody-0.0.6/README.md` & `elody-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `elody-0.0.6/pyproject.toml` & `elody-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elody"
-version = "0.0.6"
+version = "0.0.7"
 description = "elody SDK for Python"
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Intended Audience :: Developers",
```

### Comparing `elody-0.0.6/src/elody/client.py` & `elody-0.0.7/src/elody/client.py`

 * *Files identical despite different names*

### Comparing `elody-0.0.6/src/elody/loader.py` & `elody-0.0.7/src/elody/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import elody.util
 import os
-import util
 
 from importlib import import_module
 from inuits_policy_based_auth.exceptions import (
     PolicyFactoryException,
 )
```

### Comparing `elody-0.0.6/src/elody/util.py` & `elody-0.0.7/src/elody/util.py`

 * *Files identical despite different names*

### Comparing `elody-0.0.6/src/elody.egg-info/PKG-INFO` & `elody-0.0.7/src/elody.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.6
+Version: 0.0.7
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

