# Comparing `tmp/elody-0.0.5.tar.gz` & `tmp/elody-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elody-0.0.5.tar", last modified: Wed Jul 12 08:45:01 2023, max compression
+gzip compressed data, was "elody-0.0.6.tar", last modified: Wed Jul 12 09:19:21 2023, max compression
```

## Comparing `elody-0.0.5.tar` & `elody-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:45:01.650711 elody-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 08:44:50.000000 elody-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 08:45:01.650711 elody-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 08:44:50.000000 elody-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-12 08:44:50.000000 elody-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 08:45:01.650711 elody-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:45:01.646711 elody-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:45:01.646711 elody-0.0.5/src/elody/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 08:44:50.000000 elody-0.0.5/src/elody/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-12 08:44:50.000000 elody-0.0.5/src/elody/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 08:44:50.000000 elody-0.0.5/src/elody/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-12 08:44:50.000000 elody-0.0.5/src/elody/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-12 08:44:50.000000 elody-0.0.5/src/elody/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:45:01.650711 elody-0.0.5/src/elody.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 08:45:01.000000 elody-0.0.5/src/elody.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 08:45:01.000000 elody-0.0.5/src/elody.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:45:01.000000 elody-0.0.5/src/elody.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-12 08:45:01.000000 elody-0.0.5/src/elody.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 08:45:01.000000 elody-0.0.5/src/elody.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:19:21.605870 elody-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 09:19:06.000000 elody-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 09:19:21.605870 elody-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 09:19:06.000000 elody-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 09:19:06.000000 elody-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:19:21.605870 elody-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:19:21.601870 elody-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:19:21.601870 elody-0.0.6/src/elody/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-12 09:19:06.000000 elody-0.0.6/src/elody/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:19:21.601870 elody-0.0.6/src/elody.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 09:19:21.000000 elody-0.0.6/src/elody.egg-info/top_level.txt
```

### Comparing `elody-0.0.5/LICENSE` & `elody-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `elody-0.0.5/PKG-INFO` & `elody-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.5
+Version: 0.0.6
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `elody-0.0.5/README.md` & `elody-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `elody-0.0.5/pyproject.toml` & `elody-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elody"
-version = "0.0.5"
+version = "0.0.6"
 description = "elody SDK for Python"
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Intended Audience :: Developers",
@@ -22,15 +22,15 @@
 ]
 keywords = ["elody", "SDK"]
 dependencies = [
   "certifi==2023.5.7",
   "charset-normalizer==3.2.0",
   "idna==3.4",
   "requests==2.31.0",
-  "urllib3==2.0.3",
+  "urllib3>=1.26.16",
 ]
 
 [project.optional-dependencies]
 loader = [
   "cloudevents==1.9.0",
   "inuits-policy-based-auth==4.1.0",
 ]
```

### Comparing `elody-0.0.5/src/elody/client.py` & `elody-0.0.6/src/elody/client.py`

 * *Files identical despite different names*

### Comparing `elody-0.0.5/src/elody/loader.py` & `elody-0.0.6/src/elody/loader.py`

 * *Files identical despite different names*

### Comparing `elody-0.0.5/src/elody/util.py` & `elody-0.0.6/src/elody/util.py`

 * *Files identical despite different names*

### Comparing `elody-0.0.5/src/elody.egg-info/PKG-INFO` & `elody-0.0.6/src/elody.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elody
-Version: 0.0.5
+Version: 0.0.6
 Summary: elody SDK for Python
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

