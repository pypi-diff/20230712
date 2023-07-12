# Comparing `tmp/re_y-2.0.0-py3-none-any.whl.zip` & `tmp/re_y-2.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17937 bytes, number of entries: 9
+Zip file size: 17895 bytes, number of entries: 9
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 y/__init__.py
 -rwxr-xr-x  2.0 unx     2575 b- defN 80-Jan-01 00:00 y/__main__.py
 -rwxr-xr-x  2.0 unx    10305 b- defN 80-Jan-01 00:00 y/yinterpreter.py
 -rwxr-xr-x  2.0 unx     3962 b- defN 80-Jan-01 00:00 y/yreference.py
--rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_y-2.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5209 b- defN 80-Jan-01 00:00 re_y-2.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_y-2.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 re_y-2.0.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      659 b- defN 16-Jan-01 00:00 re_y-2.0.0.dist-info/RECORD
-9 files, 53418 bytes uncompressed, 16821 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_y-2.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5130 b- defN 80-Jan-01 00:00 re_y-2.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_y-2.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 re_y-2.1.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      659 b- defN 16-Jan-01 00:00 re_y-2.1.2.dist-info/RECORD
+9 files, 53339 bytes uncompressed, 16779 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: y/yinterpreter.py
 Comment: 
 
 Filename: y/yreference.py
 Comment: 
 
-Filename: re_y-2.0.0.dist-info/LICENSE
+Filename: re_y-2.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: re_y-2.0.0.dist-info/METADATA
+Filename: re_y-2.1.2.dist-info/METADATA
 Comment: 
 
-Filename: re_y-2.0.0.dist-info/WHEEL
+Filename: re_y-2.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: re_y-2.0.0.dist-info/entry_points.txt
+Filename: re_y-2.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: re_y-2.0.0.dist-info/RECORD
+Filename: re_y-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `re_y-2.0.0.dist-info/LICENSE` & `re_y-2.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `re_y-2.0.0.dist-info/METADATA` & `re_y-2.1.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-y
-Version: 2.0.0
+Version: 2.1.2
 Summary: 
 License: SSPL-1.0
 Author: Philipp Gayret
 Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -103,13 +103,11 @@
 Development requires:
 
 - Bash
 - [Docker](https://www.docker.com/)
 - [Python](https://www.python.org/)
 - [Poetry](https://python-poetry.org/)
 
-See [`app.sh`](./app.sh) for building, running and releasing the application.
-
 ## Links
 
 This project was created using [template-poetry](https://github.com/release-engineers/template-poetry).
```

