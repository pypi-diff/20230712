# Comparing `tmp/modal-0.50.2627-py3-none-any.whl.zip` & `tmp/modal-0.50.2632-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1223 bytes, number of entries: 4
--rw-r--r--  2.0 unx      517 b- defN 23-Jul-11 21:46 modal-0.50.2627.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 21:46 modal-0.50.2627.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-11 21:46 modal-0.50.2627.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      304 b- defN 23-Jul-11 21:46 modal-0.50.2627.dist-info/RECORD
-4 files, 914 bytes uncompressed, 625 bytes compressed:  31.6%
+Zip file size: 1221 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      517 b- defN 23-Jul-12 20:03 modal-0.50.2632.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 20:03 modal-0.50.2632.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-12 20:03 modal-0.50.2632.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      304 b- defN 23-Jul-12 20:03 modal-0.50.2632.dist-info/RECORD
+4 files, 914 bytes uncompressed, 623 bytes compressed:  31.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: modal-0.50.2627.dist-info/METADATA
+Filename: modal-0.50.2632.dist-info/METADATA
 Comment: 
 
-Filename: modal-0.50.2627.dist-info/WHEEL
+Filename: modal-0.50.2632.dist-info/WHEEL
 Comment: 
 
-Filename: modal-0.50.2627.dist-info/top_level.txt
+Filename: modal-0.50.2632.dist-info/top_level.txt
 Comment: 
 
-Filename: modal-0.50.2627.dist-info/RECORD
+Filename: modal-0.50.2632.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `modal-0.50.2627.dist-info/METADATA` & `modal-0.50.2632.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: modal
-Version: 0.50.2627
+Version: 0.50.2632
 Summary: Dummy alias that requires modal-client
 Author: Modal Labs
 Author-email: erik@modal.com
 Project-URL: Homepage, https://modal.com
 Description-Content-Type: text/markdown
-Requires-Dist: modal-client (==0.50.2627)
+Requires-Dist: modal-client (==0.50.2632)
 
 This package is a dummy package that just requires the modal-client package.
 If you're looking for the active learning framework [modAL](https://modal-python.readthedocs.io/en/latest/),
 it's now available using the package name `modAL-python`.
```
