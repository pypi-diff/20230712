# Comparing `tmp/pyvista-examples-0.1.1.tar.gz` & `tmp/pyvista-examples-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvista-examples-0.1.1.tar", last modified: Wed Jul 12 10:52:09 2023, max compression
+gzip compressed data, was "pyvista-examples-0.1.2.tar", last modified: Wed Jul 12 10:52:14 2023, max compression
```

## Comparing `pyvista-examples-0.1.1.tar` & `pyvista-examples-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:09.662714 pyvista-examples-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 10:52:09.662714 pyvista-examples-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:52:09.662714 pyvista-examples-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:09.654714 pyvista-examples-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:09.658714 pyvista-examples-0.1.1/src/pvexamples/
--rw-r--r--   0 runner    (1001) docker     (123)   463087 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/2k_earth_daymap.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      247 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    70751 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/airplane.ply
--rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/ant.ply
--rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/cells.py
--rw-r--r--   0 runner    (1001) docker     (123)   522284 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/channels.vti
--rw-r--r--   0 runner    (1001) docker     (123)   150745 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/gltf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/nut.ply
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/planets.py
--rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/sphere.ply
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/src/pvexamples/vrml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:09.658714 pyvista-examples-0.1.1/src/pyvista_examples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 10:52:09.000000 pyvista-examples-0.1.1/src/pyvista_examples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-12 10:52:09.000000 pyvista-examples-0.1.1/src/pyvista_examples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:52:09.000000 pyvista-examples-0.1.1/src/pyvista_examples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 10:52:09.000000 pyvista-examples-0.1.1/src/pyvista_examples.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:09.662714 pyvista-examples-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/tests/test_cell_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    26507 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/tests/test_download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/tests/test_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-12 10:51:59.000000 pyvista-examples-0.1.1/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:14.307446 pyvista-examples-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 10:52:14.307446 pyvista-examples-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:52:14.307446 pyvista-examples-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:14.299445 pyvista-examples-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:14.303446 pyvista-examples-0.1.2/src/pvexamples/
+-rw-r--r--   0 runner    (1001) docker     (123)   463087 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/2k_earth_daymap.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      247 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70751 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/airplane.ply
+-rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/ant.ply
+-rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)   522284 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/channels.vti
+-rw-r--r--   0 runner    (1001) docker     (123)   150745 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/nut.ply
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/planets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/sphere.ply
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/src/pvexamples/vrml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:14.303446 pyvista-examples-0.1.2/src/pyvista_examples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 10:52:14.000000 pyvista-examples-0.1.2/src/pyvista_examples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-12 10:52:14.000000 pyvista-examples-0.1.2/src/pyvista_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:52:14.000000 pyvista-examples-0.1.2/src/pyvista_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 10:52:14.000000 pyvista-examples-0.1.2/src/pyvista_examples.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:52:14.303446 pyvista-examples-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/tests/test_cell_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26507 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/tests/test_download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/tests/test_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-12 10:52:03.000000 pyvista-examples-0.1.2/tests/test_examples.py
```

### Comparing `pyvista-examples-0.1.1/LICENSE` & `pyvista-examples-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/2k_earth_daymap.jpg` & `pyvista-examples-0.1.2/src/pvexamples/2k_earth_daymap.jpg`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/_version.py` & `pyvista-examples-0.1.2/src/pvexamples/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 
 """
 import datetime
 
 now = datetime.datetime.now()
 
 # major, minor, patch
-version_info = 0, 1, 1
+version_info = 0, 1, 2
 
 # Nice string for the version
 __version__ = '.'.join(map(str, version_info))
```

### Comparing `pyvista-examples-0.1.1/src/pvexamples/airplane.ply` & `pyvista-examples-0.1.2/src/pvexamples/airplane.ply`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/ant.ply` & `pyvista-examples-0.1.2/src/pvexamples/ant.ply`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/cells.py` & `pyvista-examples-0.1.2/src/pvexamples/cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/channels.vti` & `pyvista-examples-0.1.2/src/pvexamples/channels.vti`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/downloads.py` & `pyvista-examples-0.1.2/src/pvexamples/downloads.py`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/examples.py` & `pyvista-examples-0.1.2/src/pvexamples/examples.py`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/gltf.py` & `pyvista-examples-0.1.2/src/pvexamples/gltf.py`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/nut.ply` & `pyvista-examples-0.1.2/src/pvexamples/nut.ply`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/planets.py` & `pyvista-examples-0.1.2/src/pvexamples/planets.py`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/sphere.ply` & `pyvista-examples-0.1.2/src/pvexamples/sphere.ply`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pvexamples/vrml.py` & `pyvista-examples-0.1.2/src/pvexamples/vrml.py`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/src/pyvista_examples.egg-info/SOURCES.txt` & `pyvista-examples-0.1.2/src/pyvista_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/tests/test_cell_examples.py` & `pyvista-examples-0.1.2/tests/test_cell_examples.py`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/tests/test_download_files.py` & `pyvista-examples-0.1.2/tests/test_download_files.py`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/tests/test_downloads.py` & `pyvista-examples-0.1.2/tests/test_downloads.py`

 * *Files identical despite different names*

### Comparing `pyvista-examples-0.1.1/tests/test_examples.py` & `pyvista-examples-0.1.2/tests/test_examples.py`

 * *Files identical despite different names*

