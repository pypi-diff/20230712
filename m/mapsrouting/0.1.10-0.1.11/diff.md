# Comparing `tmp/mapsrouting-0.1.10-py3-none-any.whl.zip` & `tmp/mapsrouting-0.1.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2687 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-12 13:01 maps/__init__.py
+Zip file size: 2685 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-12 13:17 maps/__init__.py
 -rw-rw-rw-  2.0 fat     2563 b- defN 23-Jul-12 13:01 maps/visualR.py
--rw-rw-rw-  2.0 fat      702 b- defN 23-Jul-12 13:06 mapsrouting-0.1.10.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 13:06 mapsrouting-0.1.10.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-12 13:06 mapsrouting-0.1.10.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      459 b- defN 23-Jul-12 13:06 mapsrouting-0.1.10.dist-info/RECORD
-6 files, 3839 bytes uncompressed, 1851 bytes compressed:  51.8%
+-rw-rw-rw-  2.0 fat      681 b- defN 23-Jul-12 13:17 mapsrouting-0.1.11.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 13:17 mapsrouting-0.1.11.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-12 13:17 mapsrouting-0.1.11.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      459 b- defN 23-Jul-12 13:17 mapsrouting-0.1.11.dist-info/RECORD
+6 files, 3818 bytes uncompressed, 1849 bytes compressed:  51.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: maps/__init__.py
 Comment: 
 
 Filename: maps/visualR.py
 Comment: 
 
-Filename: mapsrouting-0.1.10.dist-info/METADATA
+Filename: mapsrouting-0.1.11.dist-info/METADATA
 Comment: 
 
-Filename: mapsrouting-0.1.10.dist-info/WHEEL
+Filename: mapsrouting-0.1.11.dist-info/WHEEL
 Comment: 
 
-Filename: mapsrouting-0.1.10.dist-info/top_level.txt
+Filename: mapsrouting-0.1.11.dist-info/top_level.txt
 Comment: 
 
-Filename: mapsrouting-0.1.10.dist-info/RECORD
+Filename: mapsrouting-0.1.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## maps/__init__.py

```diff
@@ -1 +1 @@
-version = '0.1.10'
+version = '0.1.11'
```

## Comparing `mapsrouting-0.1.10.dist-info/METADATA` & `mapsrouting-0.1.11.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mapsrouting
-Version: 0.1.10
+Version: 0.1.11
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
 Requires-Dist: folium
 Requires-Dist: pandas
 Requires-Dist: numpy
-Requires-Dist: osrm
 Requires-Dist: polyline
```

