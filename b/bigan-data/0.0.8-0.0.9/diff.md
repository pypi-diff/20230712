# Comparing `tmp/bigan_data-0.0.8-py3-none-any.whl.zip` & `tmp/bigan_data-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1603 bytes, number of entries: 6
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 15:08 base/__init__.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jul-12 15:08 base/test.py
--rw-r--r--  2.0 unx      557 b- defN 23-Jul-12 15:08 bigan_data-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 15:08 bigan_data-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-12 15:08 bigan_data-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      445 b- defN 23-Jul-12 15:08 bigan_data-0.0.8.dist-info/RECORD
-6 files, 1160 bytes uncompressed, 789 bytes compressed:  32.0%
+Zip file size: 1644 bytes, number of entries: 6
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 15:16 bigan_data/__init__.py
+-rw-r--r--  2.0 unx       73 b- defN 23-Jul-12 15:16 bigan_data/bigan_data.py
+-rw-r--r--  2.0 unx      557 b- defN 23-Jul-12 15:17 bigan_data-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 15:17 bigan_data-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-12 15:17 bigan_data-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      464 b- defN 23-Jul-12 15:17 bigan_data-0.0.9.dist-info/RECORD
+6 files, 1197 bytes uncompressed, 794 bytes compressed:  33.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: base/__init__.py
+Filename: bigan_data/__init__.py
 Comment: 
 
-Filename: base/test.py
+Filename: bigan_data/bigan_data.py
 Comment: 
 
-Filename: bigan_data-0.0.8.dist-info/METADATA
+Filename: bigan_data-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: bigan_data-0.0.8.dist-info/WHEEL
+Filename: bigan_data-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: bigan_data-0.0.8.dist-info/top_level.txt
+Filename: bigan_data-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bigan_data-0.0.8.dist-info/RECORD
+Filename: bigan_data-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bigan_data-0.0.8.dist-info/METADATA` & `bigan_data-0.0.9.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigan-data
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bigan Trading Data Package
 Home-page: https://dev.azure.com/FutureFantasy/BiGan/_git/bigan-data
 Author: heian0224
 Author-email: heian0224@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://dev.azure.com/FutureFantasy/BiGan/_git/bigan-data/issues
 Platform: UNKNOWN
```

