# Comparing `tmp/cubicweb-leaflet-0.9.0.tar.gz` & `tmp/cubicweb-leaflet-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-leaflet-0.9.0.tar", last modified: Mon Mar 28 13:29:54 2022, max compression
+gzip compressed data, was "cubicweb-leaflet-1.0.0.tar", last modified: Wed Jul 12 12:38:21 2023, max compression
```

## Comparing `cubicweb-leaflet-0.9.0.tar` & `cubicweb-leaflet-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 13:29:54.389923 cubicweb-leaflet-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      308 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      530 2022-03-28 13:29:54.385923 cubicweb-leaflet-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 13:29:54.377923 cubicweb-leaflet-0.9.0/cubicweb_leaflet/
--rw-rw-rw-   0 root         (0) root         (0)       93 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 13:29:54.381923 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/
--rw-rw-rw-   0 root         (0) root         (0)      360 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/cubes.leaflet.css
--rw-rw-rw-   0 root         (0) root         (0)     8609 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/cubes.leaflet.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 13:29:54.385923 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     2898 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/layers-2x.png
--rw-rw-rw-   0 root         (0) root         (0)     1502 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/layers.png
--rw-rw-rw-   0 root         (0) root         (0)     2519 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-blue-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1221 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-green-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     4033 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-icon-2x.png
--rw-rw-rw-   0 root         (0) root         (0)     1747 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1337 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-red-icon.png
--rw-rw-rw-   0 root         (0) root         (0)      797 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-shadow.png
--rw-rw-rw-   0 root         (0) root         (0)    10161 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leaflet.css
--rw-rw-rw-   0 root         (0) root         (0)   125410 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leaflet.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 13:29:54.385923 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leafletcluster/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leafletcluster/MarkerCluster.Default.css
--rw-rw-rw-   0 root         (0) root         (0)      438 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leafletcluster/MarkerCluster.Default.ie.css
--rw-rw-rw-   0 root         (0) root         (0)      366 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leafletcluster/MarkerCluster.css
--rw-rw-rw-   0 root         (0) root         (0)    58364 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leafletcluster/leaflet.markercluster-src.js
--rw-rw-rw-   0 root         (0) root         (0)    28286 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leafletcluster/leaflet.markercluster.js
--rw-rw-rw-   0 root         (0) root         (0)     1028 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/uiprops.py
--rw-rw-rw-   0 root         (0) root         (0)    13143 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 13:29:54.381923 cubicweb-leaflet-0.9.0/cubicweb_leaflet.egg-info/
--rw-r--r--   0 root         (0) root         (0)      530 2022-03-28 13:29:53.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1279 2022-03-28 13:29:54.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-28 13:29:53.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-03-28 13:29:53.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-28 13:29:53.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2022-03-28 13:29:53.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-03-28 13:29:53.000000 cubicweb-leaflet-0.9.0/cubicweb_leaflet.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-28 13:29:54.389923 cubicweb-leaflet-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2667 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 13:29:54.385923 cubicweb-leaflet-0.9.0/test/
--rw-rw-rw-   0 root         (0) root         (0)     1774 2022-03-28 13:29:20.000000 cubicweb-leaflet-0.9.0/test/test_leaflet.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 12:38:21.480962 cubicweb-leaflet-1.0.0/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      308 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/MANIFEST.in
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      510 2023-07-12 12:38:21.480962 cubicweb-leaflet-1.0.0/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       64 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/README.rst
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 12:38:21.476962 cubicweb-leaflet-1.0.0/cubicweb_leaflet/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       93 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/__init__.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      706 2023-07-07 11:59:43.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/__pkginfo__.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 12:38:21.476962 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      360 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/cubes.leaflet.css
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     8609 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/cubes.leaflet.js
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 12:38:21.480962 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2898 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/layers-2x.png
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1502 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/layers.png
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2519 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-blue-icon.png
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1221 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-green-icon.png
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     4033 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-icon-2x.png
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1747 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-icon.png
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1337 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-red-icon.png
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      797 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-shadow.png
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    10161 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leaflet.css
+-rw-r--r--   0 fferry    (1000) fferry    (1000)   125410 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leaflet.js
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 12:38:21.480962 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leafletcluster/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1287 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leafletcluster/MarkerCluster.Default.css
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      438 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leafletcluster/MarkerCluster.Default.ie.css
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      366 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leafletcluster/MarkerCluster.css
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    58364 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leafletcluster/leaflet.markercluster-src.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    28286 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leafletcluster/leaflet.markercluster.js
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1010 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/uiprops.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)    12973 2023-07-07 11:59:08.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet/views.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 12:38:21.476962 cubicweb-leaflet-1.0.0/cubicweb_leaflet.egg-info/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      510 2023-07-12 12:38:21.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet.egg-info/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1279 2023-07-12 12:38:21.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet.egg-info/SOURCES.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-07-12 12:38:21.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet.egg-info/dependency_links.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       44 2023-07-12 12:38:21.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet.egg-info/entry_points.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-07-03 14:05:52.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet.egg-info/not-zip-safe
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       50 2023-07-12 12:38:21.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet.egg-info/requires.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       17 2023-07-12 12:38:21.000000 cubicweb-leaflet-1.0.0/cubicweb_leaflet.egg-info/top_level.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       38 2023-07-12 12:38:21.480962 cubicweb-leaflet-1.0.0/setup.cfg
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2596 2023-07-07 11:59:08.000000 cubicweb-leaflet-1.0.0/setup.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-12 12:38:21.480962 cubicweb-leaflet-1.0.0/test/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1737 2023-07-03 13:54:31.000000 cubicweb-leaflet-1.0.0/test/test_leaflet.py
```

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/cubes.leaflet.js` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/cubes.leaflet.js`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/layers-2x.png` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/layers.png` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/layers.png`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-blue-icon.png` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-blue-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-green-icon.png` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-green-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-icon-2x.png` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-icon.png` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-red-icon.png` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-red-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/images/marker-shadow.png` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leaflet.css` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leaflet.css`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leaflet.js` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leaflet.js`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leafletcluster/MarkerCluster.Default.css` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leafletcluster/MarkerCluster.Default.css`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leafletcluster/leaflet.markercluster-src.js` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leafletcluster/leaflet.markercluster-src.js`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/data/leafletcluster/leaflet.markercluster.js` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/data/leafletcluster/leaflet.markercluster.js`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/uiprops.py` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/uiprops.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -11,12 +10,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
-JAVASCRIPTS += [data('cubes.leaflet.js'),]
+JAVASCRIPTS += [
+    data("cubes.leaflet.js"),
+]
 
-GMARKER_BLUE_ICON = data('images/marker-blue-icon.png')
-GMARKER_RED_ICON = data('images/marker-red-icon.png')
-GMARKER_GREEN_ICON = data('images/marker-green-icon.png')
+GMARKER_BLUE_ICON = data("images/marker-blue-icon.png")
+GMARKER_RED_ICON = data("images/marker-red-icon.png")
+GMARKER_GREEN_ICON = data("images/marker-green-icon.png")
```

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet/views.py` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -11,328 +10,346 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 """cubicweb-leaflet views/forms/actions/components for web ui"""
-from __future__ import absolute_import
 
 import six
-from six.moves import range
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb import _
 from cubicweb.utils import js_dumps, make_uid, JSString
 from cubicweb.predicates import multi_columns_rset, adaptable
-from cubicweb.view import AnyRsetView
+from cubicweb_web.view import AnyRsetView
 
 
 #############################################################################
 # LEAFLET OBJECT ############################################################
 #############################################################################
-class LeafletMap(object):
+class LeafletMap:
     """widget class to render leaflet map
 
     Typical usage is::
 
         leaflet_map = LeafletMap()
         self.w(leaflet_map.render(self._cw, my_list_of_markers))
 
     The list of markers can either a python list or a url to a json file
     """
+
     default_settings = {
-        'divid': 'map-geo',
-        'width': '940px',
-        'height': '400px',
-        'minZoom': 1,
-        'maxZoom': 18,
-        'initialZoom': 2,  # if unset, leaflet will be asked to fit all markers
-        'provider': 'osm',
-        'map_options': {},  # see http://leafletjs.com/reference.html#map-options
-        }
+        "divid": "map-geo",
+        "width": "940px",
+        "height": "400px",
+        "minZoom": 1,
+        "maxZoom": 18,
+        "initialZoom": 2,  # if unset, leaflet will be asked to fit all markers
+        "provider": "osm",
+        "map_options": {},  # see http://leafletjs.com/reference.html#map-options
+    }
 
     providers = {
-        'osm': {
-            'url': 'https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',
-            'attribution': (
+        "osm": {
+            "url": "https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",
+            "attribution": (
                 '&copy; <a href="http://openstreetmap.org">OpenStreetMap</a> contributors, '
-                'data under '
+                "data under "
                 '<a href="https://opendatacommons.org/licenses/odbl/">Open Database License</a>'
             ),
         },
-        'wikimedia': {
-            'url': 'https://maps.wikimedia.org/osm-intl/{z}/{x}/{y}.png',
-            'attribution': (
+        "wikimedia": {
+            "url": "https://maps.wikimedia.org/osm-intl/{z}/{x}/{y}.png",
+            "attribution": (
                 '<a href="https://wikimediafoundation.org/wiki/Maps_Terms_of_Use">Wikimedia maps</a> '
                 '| Map data © <a href="http://openstreetmap.org/copyright">OpenStreetMap '
-                'contributors</a>'
+                "contributors</a>"
+            ),
+        },
+        "esri-topomap": {
+            "url": "https://server.arcgisonline.com/ArcGIS/rest/services/World_Topo_Map/MapServer/"
+            "tile/{z}/{y}/{x}",
+            "attribution": (
+                "Esri &mdash; Sources: Esri, HERE, Garmin, Intermap, increment P Corp., GEBCO, "
+                "USGS, FAO, NPS, NRCAN, GeoBase, IGN, Kadaster NL, Ordnance Survey, "
+                "Esri Japan, METI, Esri China (Hong Kong), (c) OpenStreetMap contributors, "
+                "and the GIS User Community "
             ),
         },
-        'esri-topomap': {
-            'url':
-            'https://server.arcgisonline.com/ArcGIS/rest/services/World_Topo_Map/MapServer/'
-            'tile/{z}/{y}/{x}',
-            'attribution': ('Esri &mdash; Sources: Esri, HERE, Garmin, Intermap, increment P Corp., GEBCO, '
-                            'USGS, FAO, NPS, NRCAN, GeoBase, IGN, Kadaster NL, Ordnance Survey, '
-                            'Esri Japan, METI, Esri China (Hong Kong), (c) OpenStreetMap contributors, '
-                            'and the GIS User Community ')
+        "esri-imagery": {
+            "url": "https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/"
+            "tile/{z}/{y}/{x}",
+            "attribution": (
+                "Esri &mdash; Source: Esri, Maxar, GeoEye, Earthstar Geographics, CNES/Airbus DS,"
+                "USDA, USGS, AeroGRID, IGN, and the GIS User Community"
+            ),
         },
-        'esri-imagery': {
-            'url':
-            'https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/'
-            'tile/{z}/{y}/{x}',
-            'attribution': ('Esri &mdash; Source: Esri, Maxar, GeoEye, Earthstar Geographics, CNES/Airbus DS,'
-                            'USDA, USGS, AeroGRID, IGN, and the GIS User Community')
-        }
     }
 
     def __init__(self, custom_settings=None):
         settings = self.get_settings(custom_settings)
-        if isinstance(settings['provider'], six.string_types):
-            settings['provider'] = self.providers[settings['provider']]
+        if isinstance(settings["provider"], str):
+            settings["provider"] = self.providers[settings["provider"]]
         self.settings = settings
 
     def get_settings(self, custom_settings=None):
         settings = self.default_settings.copy()
         settings.update(custom_settings or {})
         return settings
 
     def render(self, req, datasource, use_cdn=True):
-        req.add_js('cubes.leaflet.js')
-        req.add_css('cubes.leaflet.css')
+        req.add_js("cubes.leaflet.js")
+        req.add_css("cubes.leaflet.css")
         if use_cdn:
-            req.add_js('https://cdnjs.cloudflare.com/ajax/libs/leaflet/0.7.3/leaflet.js',
-                       localfile=False)
-            req.add_css('https://cdnjs.cloudflare.com/ajax/libs/leaflet/0.7.3/leaflet.css',
-                        localfile=False)
+            req.add_js(
+                "https://cdnjs.cloudflare.com/ajax/libs/leaflet/0.7.3/leaflet.js",
+                localfile=False,
+            )
+            req.add_css(
+                "https://cdnjs.cloudflare.com/ajax/libs/leaflet/0.7.3/leaflet.css",
+                localfile=False,
+            )
         else:
-            req.add_js('leaflet.js')
-            req.add_css('leaflet.css')
-        if self.settings.get('cluster'):
-            req.add_js('leafletcluster/leaflet.markercluster.js')
-            req.add_js('leafletcluster/leaflet.markercluster-src.js')
-            req.add_css(('leafletcluster/MarkerCluster.css',
-                         'leafletcluster/MarkerCluster.Default.css'))
+            req.add_js("leaflet.js")
+            req.add_css("leaflet.css")
+        if self.settings.get("cluster"):
+            req.add_js("leafletcluster/leaflet.markercluster.js")
+            req.add_js("leafletcluster/leaflet.markercluster-src.js")
+            req.add_css(
+                (
+                    "leafletcluster/MarkerCluster.css",
+                    "leafletcluster/MarkerCluster.Default.css",
+                )
+            )
         self._call_js_onload(req, datasource)
         return self.div_holder()
 
     def _call_js_onload(self, req, datasource):
-        """ Call the JS function """
-        req.add_onload("""
-function initMap() {
+        """Call the JS function"""
+        req.add_onload(
+            """
+function initMap() {{
     // this should check if your leaflet is available or wait if not.
-    if (typeof L === "undefined") {
+    if (typeof L === "undefined") {{
         window.setTimeout(initMap, 100);
         return;
-    }
-    cw.cubes.leaflet.renderLeafLetMap(%s, %s);
-};
-initMap();""" % (js_dumps(datasource), js_dumps(self.settings)))
+    }}
+    cw.cubes.leaflet.renderLeafLetMap({}, {});
+}};
+initMap();""".format(
+                js_dumps(datasource), js_dumps(self.settings)
+            )
+        )
 
     def div_holder(self):
-        style = u''
-        width = self.settings.get('width', 940)
+        style = ""
+        width = self.settings.get("width", 940)
         if width:
             if isinstance(width, int):
-                width = '%spx' % width
-            style += 'width: %s;' % width
-        height = self.settings.get('height', 400)
+                width = f"{width}px"
+            style += f"width: {width};"
+        height = self.settings.get("height", 400)
         if height:
             if isinstance(height, int):
-                height = '%spx' % height
-            style += 'height: %s;' % height
-        return u'<div id="%s" style="%s"></div>' % (self.settings['divid'], style)
+                height = f"{height}px"
+            style += f"height: {height};"
+        return f"<div id=\"{self.settings['divid']}\" style=\"{style}\"></div>"
 
 
 class LeafletMultiPolygon(LeafletMap):
-    """ LeafletMap class for plotting multipolygon.
+    """LeafletMap class for plotting multipolygon.
     Should be used in a view.
     """
 
-    js_plotter = 'cw.cubes.leaflet.plotMap'
+    js_plotter = "cw.cubes.leaflet.plotMap"
 
     def _call_js_onload(self, req, datasource):
-        req.add_onload('cw.cubes.leaflet.initMap(%s)' % js_dumps(self.settings))
-        req.add_onload('%s(%s, %s)' % (self.js_plotter,
-                                       js_dumps(datasource),
-                                       js_dumps(self.settings)))
+        req.add_onload(f"cw.cubes.leaflet.initMap({js_dumps(self.settings)})")
+        req.add_onload(
+            f"{self.js_plotter}({js_dumps(datasource)}, {js_dumps(self.settings)})"
+        )
 
 
 class LeafletMultiPolygonValues(LeafletMultiPolygon):
-    """ LeafletMap class for plotting multipolygon with associated values.
+    """LeafletMap class for plotting multipolygon with associated values.
     Should be used in a view.
     """
 
     default_settings = {
-        'legend_visibility': True,
-        'legend_position': 'bottomright',
-        'info_visibility': True,
-        'info_position': 'topright',
+        "legend_visibility": True,
+        "legend_position": "bottomright",
+        "info_visibility": True,
+        "info_position": "topright",
     }
 
-    js_plotter = 'cw.cubes.leaflet.plotMapValues'
+    js_plotter = "cw.cubes.leaflet.plotMapValues"
 
     def get_settings(self, custom_settings=None):
-        settings = super(LeafletMultiPolygonValues, self).default_settings.copy()
+        settings = super().default_settings.copy()
         settings.update(self.default_settings)
         settings.update(custom_settings or {})
         return settings
 
 
 #############################################################################
 # LEAFLET VIEWS #############################################################
 #############################################################################
 
+
 class AbstractLeafletView(AnyRsetView):
     __abstract__ = True
-    __regid__ = 'leaflet'
-    title = _('Leaflet')
+    __regid__ = "leaflet"
+    title = _("Leaflet")
     paginable = False
     plotclass = LeafletMap
 
     def call(self, custom_settings=None, use_cdn=True):
-        """ View call """
+        """View call"""
         markers = self.build_markers()
         settings = self._update_settings(custom_settings)
         geomap = self.plotclass(settings)
         self.w(geomap.render(self._cw, datasource=markers, use_cdn=use_cdn))
 
     def _update_settings(self, custom_settings):
-        """ Update the default settings with custom settings and form"""
+        """Update the default settings with custom settings and form"""
         settings = custom_settings.copy() if custom_settings else {}
-        for attr, value in six.iteritems(self._cw.form):
+        for attr, value in self._cw.form.items():
             if attr in settings:
                 settings[attr] = value
-        if 'cluster' in self._cw.form:
-            settings['cluster'] = True
+        if "cluster" in self._cw.form:
+            settings["cluster"] = True
         return settings
 
     def build_markers(self):
-        """ Build the markers from the current cw_rset """
+        """Build the markers from the current cw_rset"""
         markers = []
         for rownum, _ in enumerate(self.cw_rset.rows):
             marker = self._build_markers_from_row(rownum)
             if marker:
                 markers.append(marker)
         return markers
 
     def _build_markers_from_row(self, rownum):
-        """ Build the markers from the ``rownum`` of the current cw_rset """
+        """Build the markers from the ``rownum`` of the current cw_rset"""
         raise NotImplementedError
 
 
 class IGeocodableLeafletView(AbstractLeafletView):
-    """ Simple leaflet view for IGeocodable entities.
-    """
-    __select__ = AbstractLeafletView.__select__ & adaptable('IGeocodable')
+    """Simple leaflet view for IGeocodable entities."""
+
+    __select__ = AbstractLeafletView.__select__ & adaptable("IGeocodable")
 
     def _build_markers_from_row(self, rownum):
-        """ Build a marker from an igeocodable entity """
+        """Build a marker from an igeocodable entity"""
         entity = self.cw_rset.get_entity(rownum, 0)
-        igeocodable = entity.cw_adapt_to('IGeocodable')
+        igeocodable = entity.cw_adapt_to("IGeocodable")
         if not igeocodable.latitude or not igeocodable.longitude:
             return
         marker = {}
-        marker['eid'] = entity.eid
-        marker['latitude'] = igeocodable.latitude
-        marker['longitude'] = igeocodable.longitude
-        marker['title'] = entity.dc_title()
-        marker['url'] = entity.absolute_url()
-        marker['description'] = entity.dc_description(format='text/html') or ''
-        marker['icon_options'] = {'iconUrl': self.marker_icon(entity)}
-        marker['popup'] = '<h3><a href="{url}">{title}</a></h3>{description}'
+        marker["eid"] = entity.eid
+        marker["latitude"] = igeocodable.latitude
+        marker["longitude"] = igeocodable.longitude
+        marker["title"] = entity.dc_title()
+        marker["url"] = entity.absolute_url()
+        marker["description"] = entity.dc_description(format="text/html") or ""
+        marker["icon_options"] = {"iconUrl": self.marker_icon(entity)}
+        marker["popup"] = '<h3><a href="{url}">{title}</a></h3>{description}'
         return marker
 
     def marker_icon(self, entity):
-        return entity.cw_adapt_to('IGeocodable').marker_icon
+        return entity.cw_adapt_to("IGeocodable").marker_icon
 
 
 class RowLeafletView(AbstractLeafletView):
-    """ Simple leaflet view that try to convert the first column to latitude
+    """Simple leaflet view that try to convert the first column to latitude
     and the second column to longitude.
     """
+
     __select__ = AbstractLeafletView.__select__ & multi_columns_rset(2)
 
     def _build_markers_from_row(self, rownum):
-        """ Build a marker from the ``rownum`` of the current cw_rset,
+        """Build a marker from the ``rownum`` of the current cw_rset,
         probably floats"""
         marker = {}
-        marker['eid'] = make_uid('marker')
+        marker["eid"] = make_uid("marker")
         row = self.cw_rset[rownum]
         if not len(row) >= 2 or not row[0] or not row[1]:
             return
         try:
-            marker['latitude'] = float(row[0])
-            marker['longitude'] = float(row[1])
+            marker["latitude"] = float(row[0])
+            marker["longitude"] = float(row[1])
         except (TypeError, ValueError):
             return
         data = []
         for i in range(2, len(row)):
-            if rset.description[rownum][i] == 'String' and row[i]:
+            if rset.description[rownum][i] == "String" and row[i]:
                 data.append(xml_escape(row[i]))
         if data:
-            marker['title'] = data[0]
-            marker['notes'] = data[1:]
-            _d = [d for d in data if d.startswith('http://')]
+            marker["title"] = data[0]
+            marker["notes"] = data[1:]
+            _d = [d for d in data if d.startswith("http://")]
             if _d:
-                marker['url'] = _d[0]
+                marker["url"] = _d[0]
         return marker
 
 
 #############################################################################
 # LEAFLET POLYGON VIEW ######################################################
 #############################################################################
 class GeoJsonView(AbstractLeafletView):
-    """ Leaflet view that work on a single column rset.
+    """Leaflet view that work on a single column rset.
     It expects GeoJson on the single column and will plot Multipolygon
     based on this GeoJson. This should be used with the postgis cube
     and the 'ASJSON' RQL function
     """
-    title = _('GeoJson')
-    __regid__ = 'leaflet-geojson'
+
+    title = _("GeoJson")
+    __regid__ = "leaflet-geojson"
     paginable = False
     __select__ = AbstractLeafletView.__select__ & multi_columns_rset(1)
     plotclass = LeafletMultiPolygon
 
     def build_markers(self):
-        """ Build the markers from an rset """
-        return JSString('[%s]' % ', '.join(row[0] for row in self.cw_rset.rows))
+        """Build the markers from an rset"""
+        return JSString(f"[{', '.join(row[0] for row in self.cw_rset.rows)}]")
 
 
 class GeoJsonValuesView(AbstractLeafletView):
     """Leaflet view that works on a multicolumns rset.
 
     It expects GeoJson on the first column. It will plot Multipolygon
     based on this GeoJson. This should be used with the postgis cube
     and the 'ASJSON' RQL function.
 
     If the second column contains numbers, they are used to colorize
     geometries. Otherwize, the row index is used to colorize the
     geometry.
     """
-    title = _('GeoJson')
-    __regid__ = 'leaflet-geojson'
+
+    title = _("GeoJson")
+    __regid__ = "leaflet-geojson"
     paginable = False
-    __select__ = (AbstractLeafletView.__select__ &
-                  multi_columns_rset())
+    __select__ = AbstractLeafletView.__select__ & multi_columns_rset()
 
     plotclass = LeafletMultiPolygonValues
 
     def _get_geo(self, row):
         return row[0]
 
     def _get_data(self, row):
         return js_dumps(row[1:])
 
     def build_markers(self):
-        """ Build the markers from an rset """
-        datafmt = ('{"type": "Feature", '
-                   ' "id": %(id)s, '
-                   ' "properties": %(vals)s, '
-                   ' "geometry": %(geo)s}')
-        data = ', '.join(datafmt % {'id': i,
-                                    'vals': self._get_data(row),
-                                    'geo': self._get_geo(row)}
-                         for i, row in enumerate(self.cw_rset))
+        """Build the markers from an rset"""
+        datafmt = (
+            '{"type": "Feature", '
+            ' "id": %(id)s, '
+            ' "properties": %(vals)s, '
+            ' "geometry": %(geo)s}'
+        )
+        data = ", ".join(
+            datafmt % {"id": i, "vals": self._get_data(row), "geo": self._get_geo(row)}
+            for i, row in enumerate(self.cw_rset)
+        )
         return JSString('{"type": "FeatureCollection","features": [%s]}' % data)
```

### Comparing `cubicweb-leaflet-0.9.0/cubicweb_leaflet.egg-info/SOURCES.txt` & `cubicweb-leaflet-1.0.0/cubicweb_leaflet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-leaflet-0.9.0/setup.py` & `cubicweb-leaflet-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,66 +18,64 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with CubicWeb.  If not, see <http://www.gnu.org/licenses/>.
 """cubicweb_leaflet setup module using data from
 cubicweb_leaflet/__pkginfo__.py file
 """
 
-from __future__ import absolute_import
 from os.path import join, dirname
 
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_leaflet', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_leaflet", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, 'README.rst')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-                    for d, v in requires.items()]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'leaflet=cubicweb_leaflet',
+        "cubicweb.cubes": [
+            "leaflet=cubicweb_leaflet",
         ],
     },
     zip_safe=False,
 )
```

### Comparing `cubicweb-leaflet-0.9.0/test/test_leaflet.py` & `cubicweb-leaflet-1.0.0/test/test_leaflet.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,19 @@
             return set(('My', 'Cube', 'Entity', 'Types'))
 
         def list_startup_views(self):
             '''only test startup views of the returned identifiers'''
             return ('some', 'startup', 'views')
 """
 
-from __future__ import absolute_import
 from cubicweb.devtools import testlib
 
+
 class DefaultTC(testlib.CubicWebTC):
     def test_something(self):
-        self.skipTest('this cube has no test')
+        self.skipTest("this cube has no test")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from logilab.common.testlib import unittest_main
+
     unittest_main()
```

