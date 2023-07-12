# Comparing `tmp/mapsrouting-0.0.8-py3-none-any.whl.zip` & `tmp/mapsrouting-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1216 bytes, number of entries: 4
--rw-rw-rw-  2.0 fat      724 b- defN 23-Jul-12 12:27 mapsrouting-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 12:27 mapsrouting-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-12 12:27 mapsrouting-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      312 b- defN 23-Jul-12 12:27 mapsrouting-0.0.8.dist-info/RECORD
-4 files, 1129 bytes uncompressed, 602 bytes compressed:  46.7%
+Zip file size: 1211 bytes, number of entries: 4
+-rw-rw-rw-  2.0 fat      701 b- defN 23-Jul-12 12:29 mapsrouting-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 12:29 mapsrouting-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-12 12:29 mapsrouting-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      312 b- defN 23-Jul-12 12:29 mapsrouting-0.0.9.dist-info/RECORD
+4 files, 1106 bytes uncompressed, 597 bytes compressed:  46.0%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: mapsrouting-0.0.8.dist-info/METADATA
+Filename: mapsrouting-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: mapsrouting-0.0.8.dist-info/WHEEL
+Filename: mapsrouting-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: mapsrouting-0.0.8.dist-info/top_level.txt
+Filename: mapsrouting-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mapsrouting-0.0.8.dist-info/RECORD
+Filename: mapsrouting-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mapsrouting-0.0.8.dist-info/METADATA` & `mapsrouting-0.0.9.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: mapsrouting
-Version: 0.0.8
+Version: 0.0.9
 Summary: Visualize map paths implemented with Python
 Home-page: https://github.com/Dongguk-MAPS/Routing-Visualization
 Author: codusl100
 Author-email: codusl100@naver.com
 Keywords: codusl100,MAPS,route visualization,python route visualization
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
-Requires-Dist: urllib
 Requires-Dist: folium
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: osrm
 Requires-Dist: polyline
```

