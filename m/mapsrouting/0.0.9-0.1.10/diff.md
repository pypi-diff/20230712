# Comparing `tmp/mapsrouting-0.0.9-py3-none-any.whl.zip` & `tmp/mapsrouting-0.1.10-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,8 @@
-Zip file size: 1211 bytes, number of entries: 4
--rw-rw-rw-  2.0 fat      701 b- defN 23-Jul-12 12:29 mapsrouting-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 12:29 mapsrouting-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-12 12:29 mapsrouting-0.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      312 b- defN 23-Jul-12 12:29 mapsrouting-0.0.9.dist-info/RECORD
-4 files, 1106 bytes uncompressed, 597 bytes compressed:  46.0%
+Zip file size: 2687 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-12 13:01 maps/__init__.py
+-rw-rw-rw-  2.0 fat     2563 b- defN 23-Jul-12 13:01 maps/visualR.py
+-rw-rw-rw-  2.0 fat      702 b- defN 23-Jul-12 13:06 mapsrouting-0.1.10.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 13:06 mapsrouting-0.1.10.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-12 13:06 mapsrouting-0.1.10.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      459 b- defN 23-Jul-12 13:06 mapsrouting-0.1.10.dist-info/RECORD
+6 files, 3839 bytes uncompressed, 1851 bytes compressed:  51.8%
```

## zipnote {}

```diff
@@ -1,13 +1,19 @@
-Filename: mapsrouting-0.0.9.dist-info/METADATA
+Filename: maps/__init__.py
 Comment: 
 
-Filename: mapsrouting-0.0.9.dist-info/WHEEL
+Filename: maps/visualR.py
 Comment: 
 
-Filename: mapsrouting-0.0.9.dist-info/top_level.txt
+Filename: mapsrouting-0.1.10.dist-info/METADATA
 Comment: 
 
-Filename: mapsrouting-0.0.9.dist-info/RECORD
+Filename: mapsrouting-0.1.10.dist-info/WHEEL
+Comment: 
+
+Filename: mapsrouting-0.1.10.dist-info/top_level.txt
+Comment: 
+
+Filename: mapsrouting-0.1.10.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mapsrouting-0.0.9.dist-info/METADATA` & `mapsrouting-0.1.10.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapsrouting
-Version: 0.0.9
+Version: 0.1.10
 Summary: Visualize map paths implemented with Python
 Home-page: https://github.com/Dongguk-MAPS/Routing-Visualization
 Author: codusl100
 Author-email: codusl100@naver.com
 Keywords: codusl100,MAPS,route visualization,python route visualization
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

