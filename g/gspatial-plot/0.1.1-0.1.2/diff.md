# Comparing `tmp/gspatial_plot-0.1.1.tar.gz` & `tmp/gspatial_plot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspatial_plot-0.1.1.tar", last modified: Sat Mar 18 21:55:01 2023, max compression
+gzip compressed data, was "gspatial_plot-0.1.2.tar", last modified: Wed Jul 12 05:04:50 2023, max compression
```

## Comparing `gspatial_plot-0.1.1.tar` & `gspatial_plot-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-18 21:55:01.548124 gspatial_plot-0.1.1/
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     1062 2023-01-24 13:48:22.000000 gspatial_plot-0.1.1/LICENSE
--rw-rw-r--   0 ambee     (1000) ambee     (1000)       43 2023-01-24 20:41:15.000000 gspatial_plot-0.1.1/MANIFEST.in
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     2670 2023-03-18 21:55:01.548124 gspatial_plot-0.1.1/PKG-INFO
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     2130 2023-02-28 08:11:29.000000 gspatial_plot-0.1.1/README.md
-drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-18 21:55:01.540124 gspatial_plot-0.1.1/gspatial_plot/
--rw-rw-r--   0 ambee     (1000) ambee     (1000)       20 2023-02-03 21:03:20.000000 gspatial_plot-0.1.1/gspatial_plot/__init__.py
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     1183 2023-02-04 09:15:27.000000 gspatial_plot-0.1.1/gspatial_plot/config.py
-drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-18 21:55:01.548124 gspatial_plot-0.1.1/gspatial_plot/datasets/
--rw-r--r--   0 ambee     (1000) ambee     (1000)        5 2021-08-01 17:23:46.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_admin_0_countries.cpg
--rwxr-xr-x   0 ambee     (1000) ambee     (1000)   786828 2022-05-09 04:46:19.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_admin_0_countries.dbf
--rwxr-xr-x   0 ambee     (1000) ambee     (1000)      143 2022-05-09 04:46:19.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_admin_0_countries.prj
--rwxr-xr-x   0 ambee     (1000) ambee     (1000)  1613020 2022-05-09 04:46:19.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_admin_0_countries.shp
--rwxr-xr-x   0 ambee     (1000) ambee     (1000)     2036 2022-05-09 04:46:19.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_admin_0_countries.shx
--rw-r--r--   0 ambee     (1000) ambee     (1000)        5 2021-08-31 07:43:04.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_geographic_lines.cpg
--rw-r--r--   0 ambee     (1000) ambee     (1000)    39112 2021-11-14 23:27:26.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_geographic_lines.dbf
--rw-r--r--   0 ambee     (1000) ambee     (1000)      145 2021-11-14 23:27:26.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_geographic_lines.prj
--rw-r--r--   0 ambee     (1000) ambee     (1000)    38836 2021-08-31 07:43:04.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_geographic_lines.shp
--rw-r--r--   0 ambee     (1000) ambee     (1000)      148 2021-08-31 07:43:04.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_geographic_lines.shx
--rw-r--r--   0 ambee     (1000) ambee     (1000)        5 2021-08-01 17:23:50.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_lakes.cpg
--rw-r--r--   0 ambee     (1000) ambee     (1000)  2994462 2021-11-29 04:07:23.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_lakes.dbf
--rw-r--r--   0 ambee     (1000) ambee     (1000)      145 2021-08-29 06:05:04.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_lakes.prj
--rw-r--r--   0 ambee     (1000) ambee     (1000)   339832 2021-11-23 07:23:19.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_lakes.shp
--rw-r--r--   0 ambee     (1000) ambee     (1000)     3396 2021-11-23 07:23:19.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_lakes.shx
--rw-r--r--   0 ambee     (1000) ambee     (1000)        5 2017-08-12 22:28:26.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_ocean.cpg
--rw-r--r--   0 ambee     (1000) ambee     (1000)      176 2017-10-16 01:22:56.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_ocean.dbf
--rw-r--r--   0 ambee     (1000) ambee     (1000)      143 2017-08-12 22:28:26.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_ocean.prj
--rw-r--r--   0 ambee     (1000) ambee     (1000)   978340 2017-10-16 01:22:56.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_ocean.shp
--rw-r--r--   0 ambee     (1000) ambee     (1000)      108 2017-10-16 01:22:56.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_ocean.shx
--rw-r--r--   0 ambee     (1000) ambee     (1000)        5 2021-08-01 17:23:50.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.cpg
--rw-r--r--   0 ambee     (1000) ambee     (1000)  3323764 2021-11-29 04:07:23.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.dbf
--rw-r--r--   0 ambee     (1000) ambee     (1000)      145 2021-08-01 17:23:50.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.prj
--rw-r--r--   0 ambee     (1000) ambee     (1000)   440568 2021-11-23 08:22:00.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shp
--rw-r--r--   0 ambee     (1000) ambee     (1000)     3924 2021-11-23 08:22:00.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shx
--rw-r--r--   0 ambee     (1000) ambee     (1000)   438813 2023-02-04 09:12:29.000000 gspatial_plot-0.1.1/gspatial_plot/datasets/us_states.geojson
--rw-rw-r--   0 ambee     (1000) ambee     (1000)    47384 2023-03-18 21:50:26.000000 gspatial_plot-0.1.1/gspatial_plot/plot.py
-drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-18 21:55:01.540124 gspatial_plot-0.1.1/gspatial_plot.egg-info/
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     2670 2023-03-18 21:55:01.000000 gspatial_plot-0.1.1/gspatial_plot.egg-info/PKG-INFO
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     1550 2023-03-18 21:55:01.000000 gspatial_plot-0.1.1/gspatial_plot.egg-info/SOURCES.txt
--rw-rw-r--   0 ambee     (1000) ambee     (1000)        1 2023-03-18 21:55:01.000000 gspatial_plot-0.1.1/gspatial_plot.egg-info/dependency_links.txt
--rw-rw-r--   0 ambee     (1000) ambee     (1000)      183 2023-03-18 21:55:01.000000 gspatial_plot-0.1.1/gspatial_plot.egg-info/requires.txt
--rw-rw-r--   0 ambee     (1000) ambee     (1000)       14 2023-03-18 21:55:01.000000 gspatial_plot-0.1.1/gspatial_plot.egg-info/top_level.txt
--rw-rw-r--   0 ambee     (1000) ambee     (1000)       79 2023-03-18 21:55:01.548124 gspatial_plot-0.1.1/setup.cfg
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     1279 2023-03-18 21:51:00.000000 gspatial_plot-0.1.1/setup.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.189175 gspatial_plot-0.1.2/
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1062 2023-01-24 13:48:22.000000 gspatial_plot-0.1.2/LICENSE
+-rwxr-xr-x   0 ambee      (501) staff       (20)       43 2023-01-24 20:41:15.000000 gspatial_plot-0.1.2/MANIFEST.in
+-rw-r--r--   0 ambee      (501) staff       (20)     2650 2023-07-12 05:04:50.189236 gspatial_plot-0.1.2/PKG-INFO
+-rwxr-xr-x   0 ambee      (501) staff       (20)     2130 2023-02-28 08:11:29.000000 gspatial_plot-0.1.2/README.md
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.180552 gspatial_plot-0.1.2/gspatial_plot/
+-rwxr-xr-x   0 ambee      (501) staff       (20)       20 2023-02-03 21:03:20.000000 gspatial_plot-0.1.2/gspatial_plot/__init__.py
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1183 2023-02-04 09:15:27.000000 gspatial_plot-0.1.2/gspatial_plot/config.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.188781 gspatial_plot-0.1.2/gspatial_plot/datasets/
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-01 17:23:46.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)   786828 2022-05-09 04:46:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      143 2022-05-09 04:46:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)  1613020 2022-05-09 04:46:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)     2036 2022-05-09 04:46:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-31 07:43:04.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)    39112 2021-11-14 23:27:26.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      145 2021-11-14 23:27:26.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)    38836 2021-08-31 07:43:04.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)      148 2021-08-31 07:43:04.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-01 17:23:50.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)  2994462 2021-11-29 04:07:23.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      145 2021-08-29 06:05:04.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)   339832 2021-11-23 07:23:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)     3396 2021-11-23 07:23:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2017-08-12 22:28:26.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)      176 2017-10-16 01:22:56.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      143 2017-08-12 22:28:26.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)   978340 2017-10-16 01:22:56.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)      108 2017-10-16 01:22:56.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-01 17:23:50.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)  3323764 2021-11-29 04:07:23.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      145 2021-08-01 17:23:50.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)   440568 2021-11-23 08:22:00.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)     3924 2021-11-23 08:22:00.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)   438813 2023-02-04 09:12:29.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/us_states.geojson
+-rwxr-xr-x   0 ambee      (501) staff       (20)    47404 2023-07-12 05:01:11.000000 gspatial_plot-0.1.2/gspatial_plot/plot.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.181168 gspatial_plot-0.1.2/gspatial_plot.egg-info/
+-rwxr-xr-x   0 ambee      (501) staff       (20)     2650 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/PKG-INFO
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1574 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/SOURCES.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)        1 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/dependency_links.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)      183 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/requires.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)       14 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/top_level.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)       79 2023-07-12 05:04:50.189423 gspatial_plot-0.1.2/setup.cfg
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1279 2023-07-12 05:01:28.000000 gspatial_plot-0.1.2/setup.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.189075 gspatial_plot-0.1.2/tests/
+-rwxr-xr-x   0 ambee      (501) staff       (20)      460 2023-01-24 19:47:35.000000 gspatial_plot-0.1.2/tests/test_functions.py
```

### Comparing `gspatial_plot-0.1.1/LICENSE` & `gspatial_plot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/PKG-INFO` & `gspatial_plot-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: gspatial_plot
-Version: 0.1.1
+Version: 0.1.2
 Summary: A geospatial plotting library built on top of geopandas.
 Home-page: https://github.com/ambeelabs/gspatial_plot/
 Author: Ambee
 License: MIT
 Keywords: geospatial plot geopandas maps plotting graph folium
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -107,9 +106,7 @@
 ```python
 gsp.offline_static_basemap()
 ```
 
 ```python
 gsp.offline_folium_basemap(crs="EPSG4326")
 ```
-
-
```

### Comparing `gspatial_plot-0.1.1/README.md` & `gspatial_plot-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/config.py` & `gspatial_plot-0.1.2/gspatial_plot/config.py`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_admin_0_countries.dbf` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.dbf`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_admin_0_countries.shp` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_admin_0_countries.shx` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.shx`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_geographic_lines.dbf` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.dbf`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_geographic_lines.shp` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_lakes.dbf` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.dbf`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_lakes.shp` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_lakes.shx` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.shx`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_ocean.shp` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.dbf` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.dbf`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shp` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shx` & `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shx`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/datasets/us_states.geojson` & `gspatial_plot-0.1.2/gspatial_plot/datasets/us_states.geojson`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.1/gspatial_plot/plot.py` & `gspatial_plot-0.1.2/gspatial_plot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -823,15 +823,15 @@
     if axis_on == True:
         ax.axis("on")
 
     if base is not None and point_data is True:
         ax = base.boundary.plot(
             color=boundarycolor, linewidth=boundary_linewidth, ax=ax
         )
-    else:
+    elif point_data is False:
         ax = data.boundary.plot(
             color=boundarycolor, linewidth=boundary_linewidth, ax=ax
         )
 
     plot_data = data.copy()
 
     if interpolate == True:
```

### Comparing `gspatial_plot-0.1.1/gspatial_plot.egg-info/PKG-INFO` & `gspatial_plot-0.1.2/gspatial_plot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: gspatial-plot
-Version: 0.1.1
+Version: 0.1.2
 Summary: A geospatial plotting library built on top of geopandas.
 Home-page: https://github.com/ambeelabs/gspatial_plot/
 Author: Ambee
 License: MIT
 Keywords: geospatial plot geopandas maps plotting graph folium
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -107,9 +106,7 @@
 ```python
 gsp.offline_static_basemap()
 ```
 
 ```python
 gsp.offline_folium_basemap(crs="EPSG4326")
 ```
-
-
```

### Comparing `gspatial_plot-0.1.1/gspatial_plot.egg-info/SOURCES.txt` & `gspatial_plot-0.1.2/gspatial_plot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 gspatial_plot/datasets/ne_50m_ocean.shp
 gspatial_plot/datasets/ne_50m_ocean.shx
 gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.cpg
 gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.dbf
 gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.prj
 gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shp
 gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shx
-gspatial_plot/datasets/us_states.geojson
+gspatial_plot/datasets/us_states.geojson
+tests/test_functions.py
```

### Comparing `gspatial_plot-0.1.1/setup.py` & `gspatial_plot-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 long_description = open(os.path.join(here, 'README.md')).read()
 
 setup(
     name="gspatial_plot",
     packages=find_packages(include=["gspatial_plot"]),
-    version="0.1.1",
+    version="0.1.2",
     author="Ambee",
     license="MIT",
     url='https://github.com/ambeelabs/gspatial_plot/',
     description="A geospatial plotting library built on top of geopandas.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     install_requires=[
```

