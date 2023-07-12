# Comparing `tmp/spatial_summarize_within-1.0.3.tar.gz` & `tmp/spatial_summarize_within-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_summarize_within-1.0.3.tar", last modified: Mon Jul 10 03:55:41 2023, max compression
+gzip compressed data, was "spatial_summarize_within-1.0.4.tar", last modified: Wed Jul 12 18:42:20 2023, max compression
```

## Comparing `spatial_summarize_within-1.0.3.tar` & `spatial_summarize_within-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-07-10 03:55:41.059357 spatial_summarize_within-1.0.3/
--rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-1.0.3/LICENSE
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-07-10 03:55:41.059238 spatial_summarize_within-1.0.3/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)     6819 2023-06-16 23:38:22.000000 spatial_summarize_within-1.0.3/README.md
--rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-07-10 03:55:41.059396 spatial_summarize_within-1.0.3/setup.cfg
--rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-07-10 03:52:47.000000 spatial_summarize_within-1.0.3/setup.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-07-10 03:55:41.058505 spatial_summarize_within-1.0.3/spatial_summarize_within/
--rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/__init__.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2370 2023-07-10 03:53:06.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/max_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2398 2023-07-10 03:53:06.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/mean_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2370 2023-07-10 03:53:06.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/min_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2357 2023-07-10 03:53:06.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/sum_within.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-07-10 03:55:41.059068 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/SOURCES.txt
--rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/dependency_links.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/requires.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/top_level.txt
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-07-12 18:42:20.207918 spatial_summarize_within-1.0.4/
+-rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-1.0.4/LICENSE
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-07-12 18:42:20.207780 spatial_summarize_within-1.0.4/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)     8993 2023-07-10 03:57:14.000000 spatial_summarize_within-1.0.4/README.md
+-rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-07-12 18:42:20.207961 spatial_summarize_within-1.0.4/setup.cfg
+-rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-07-12 01:04:17.000000 spatial_summarize_within-1.0.4/setup.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-07-12 18:42:20.206431 spatial_summarize_within-1.0.4/spatial_summarize_within/
+-rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-1.0.4/spatial_summarize_within/__init__.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2863 2023-07-12 18:37:27.000000 spatial_summarize_within-1.0.4/spatial_summarize_within/max_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2927 2023-07-12 18:34:19.000000 spatial_summarize_within-1.0.4/spatial_summarize_within/mean_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2898 2023-07-12 18:37:27.000000 spatial_summarize_within-1.0.4/spatial_summarize_within/min_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2864 2023-07-12 01:17:47.000000 spatial_summarize_within-1.0.4/spatial_summarize_within/sum_within.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-07-12 18:42:20.207115 spatial_summarize_within-1.0.4/spatial_summarize_within.egg-info/
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-07-12 18:42:20.000000 spatial_summarize_within-1.0.4/spatial_summarize_within.egg-info/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-07-12 18:42:20.000000 spatial_summarize_within-1.0.4/spatial_summarize_within.egg-info/SOURCES.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-07-12 18:42:20.000000 spatial_summarize_within-1.0.4/spatial_summarize_within.egg-info/dependency_links.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-07-12 18:42:20.000000 spatial_summarize_within-1.0.4/spatial_summarize_within.egg-info/requires.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-07-12 18:42:20.000000 spatial_summarize_within-1.0.4/spatial_summarize_within.egg-info/top_level.txt
```

### Comparing `spatial_summarize_within-1.0.3/LICENSE` & `spatial_summarize_within-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-1.0.3/spatial_summarize_within/max_within.py` & `spatial_summarize_within-1.0.4/spatial_summarize_within/mean_within.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,44 +4,57 @@
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
 # Function
-def max_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
+def mean_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
-    # Add area column to input geodataframe
+
+    # set same CRS
+    if input_summary_features.crs != input_shapefile.crs:
+        input_summary_features = input_summary_features.to_crs(input_shapefile.crs)
+
+    # set equal area projection
+    equal_area_crs = 'EPSG:6933'
+    input_summary_features = input_summary_features.to_crs(equal_area_crs)
+    input_shapefile = input_shapefile.to_crs(equal_area_crs)
+
+    # Add area column to input
     input_summary_features["area"] = input_summary_features.geometry.area
     # Intersect the input geodataframe with the entire overlay shapefile
     intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection', keep_geom_type=False)
     # Calculate the area of each polygon in intersect dataframe
     intersected["intersect_area"] = intersected.area
     # Calculate the percentage overlap of each polygon
     intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
     # Loop through each polygon in the overlay geodataframe
     for polygon in input_shapefile.itertuples():
         # Select intersected parts that belong to the current polygon
         temp_intersect = intersected.loc[intersected[key] == getattr(polygon, key)]
-        # Calculate the weighted value for each column
+        # Calculate the weighted mean
         for column in columns:
-            temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).max()
+            temp_intersect[column] = (temp_intersect[column] * temp_intersect["intersect_area"]).sum() / temp_intersect["intersect_area"].sum()
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
         # Group the results
-        temp_result = temp_intersect.groupby(key).max(numeric_only=True).reset_index()
+        temp_result = temp_intersect.groupby(key).mean(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
     result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
 
+    # Round relevant columns to 2 decimal places
+    result_gdf[columns + ['intersect_area', 'overlap_pct']] = result_gdf[columns + ['intersect_area', 'overlap_pct']].round(2)
+
     # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
-    return result_gdf
+    return result_gdf
```

### Comparing `spatial_summarize_within-1.0.3/spatial_summarize_within/mean_within.py` & `spatial_summarize_within-1.0.4/spatial_summarize_within/max_within.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,44 +4,57 @@
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
 # Function
-def mean_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
+def max_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
-    # Add area column to input geodataframe
+
+    # set same CRS
+    if input_summary_features.crs != input_shapefile.crs:
+        input_summary_features = input_summary_features.to_crs(input_shapefile.crs)
+
+    # set equal area projection
+    equal_area_crs = 'EPSG:6933'
+    input_summary_features = input_summary_features.to_crs(equal_area_crs)
+    input_shapefile = input_shapefile.to_crs(equal_area_crs)
+
+    # Add area column to input
     input_summary_features["area"] = input_summary_features.geometry.area
     # Intersect the input geodataframe with the entire overlay shapefile
     intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection', keep_geom_type=False)
     # Calculate the area of each polygon in intersect dataframe
     intersected["intersect_area"] = intersected.area
     # Calculate the percentage overlap of each polygon
     intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
     # Loop through each polygon in the overlay geodataframe
     for polygon in input_shapefile.itertuples():
         # Select intersected parts that belong to the current polygon
         temp_intersect = intersected.loc[intersected[key] == getattr(polygon, key)]
-        # Calculate the weighted mean
+        # Calculate the maximum value for each column
         for column in columns:
-            temp_intersect[column] = (temp_intersect[column] * temp_intersect["intersect_area"]).sum() / temp_intersect["intersect_area"].sum()
+            temp_intersect[column] = temp_intersect[column].max()
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
         # Group the results
-        temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
+        temp_result = temp_intersect.groupby(key).max(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
     result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
 
+    # Round relevant columns to 2 decimal places
+    result_gdf[columns + ['intersect_area', 'overlap_pct']] = result_gdf[columns + ['intersect_area', 'overlap_pct']].round(2)
+
     # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
-    return result_gdf
+    return result_gdf
```

### Comparing `spatial_summarize_within-1.0.3/spatial_summarize_within/min_within.py` & `spatial_summarize_within-1.0.4/spatial_summarize_within/min_within.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,25 @@
 
 # Function
 def min_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
-    # Add area column to input geodataframe
+
+    # set same CRS
+    if input_summary_features.crs != input_shapefile.crs:
+        input_summary_features = input_summary_features.to_crs(input_shapefile.crs)
+
+    # set equal area projection
+    equal_area_crs = 'EPSG:6933'
+    input_summary_features = input_summary_features.to_crs(equal_area_crs)
+    input_shapefile = input_shapefile.to_crs(equal_area_crs)
+
+    # Add area column to input
     input_summary_features["area"] = input_summary_features.geometry.area
     # Intersect the input geodataframe with the entire overlay shapefile
     intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection', keep_geom_type=False)
     # Calculate the area of each polygon in intersect dataframe
     intersected["intersect_area"] = intersected.area
     # Calculate the percentage overlap of each polygon
     intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
@@ -37,11 +47,14 @@
         temp_result = temp_intersect.groupby(key).min(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
     result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
 
+    # Round relevant columns to 2 decimal places
+    result_gdf[columns + ['intersect_area', 'overlap_pct']] = result_gdf[columns + ['intersect_area', 'overlap_pct']].round(2)
+
     # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
-    return result_gdf
+    return result_gdf
```

### Comparing `spatial_summarize_within-1.0.3/spatial_summarize_within/sum_within.py` & `spatial_summarize_within-1.0.4/spatial_summarize_within/sum_within.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,44 +3,58 @@
 import shapely
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
-# function
+# Function
 def sum_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
-        # Append suffix to key in input_summary_features
+        # Append suffix to key in input_summary_features if key match
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
-    # Add area column to input geodataframe
+
+    # set same CRS
+    if input_summary_features.crs != input_shapefile.crs:
+        input_summary_features = input_summary_features.to_crs(input_shapefile.crs)
+
+    # set equal area projection
+    equal_area_crs = 'EPSG:6933'
+    input_summary_features = input_summary_features.to_crs(equal_area_crs)
+    input_shapefile = input_shapefile.to_crs(equal_area_crs)
+
+    # Add area column to input
     input_summary_features["area"] = input_summary_features.geometry.area
-    # Intersect the input geodataframe with the entire overlay shapefile
+    # Intersect the summary features with the input shapefile
     intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection', keep_geom_type=False)
     # Calculate the area of each polygon in intersect dataframe
     intersected["intersect_area"] = intersected.area
     # Calculate the percentage overlap of each polygon
     intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
-    # Loop through each polygon in the overlay geodataframe
+    # Loop through each polygon in the overlay
     for polygon in input_shapefile.itertuples():
         # Select intersected parts that belong to current polygon
         temp_intersect = intersected.loc[intersected[key] == getattr(polygon, key)]
         # Calculate the weighted sum
         for column in columns:
-            temp_intersect.loc[:, column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
+            temp_intersect.loc[:, column] = temp_intersect[column] * temp_intersect["overlap_pct"]
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
         # Group the results
         temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
     result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
+
+    # Round relevant columns to 2 decimal places
+    result_gdf[columns + ['intersect_area', 'overlap_pct']] = result_gdf[columns + ['intersect_area', 'overlap_pct']].round(2)
+
     # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
-    return result_gdf
+    return result_gdf
```

