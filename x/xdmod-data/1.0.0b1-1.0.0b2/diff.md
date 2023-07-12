# Comparing `tmp/xdmod_data-1.0.0b1-py3-none-any.whl.zip` & `tmp/xdmod_data-1.0.0b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 16266 bytes, number of entries: 13
+Zip file size: 16268 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       37 b- defN 23-Jul-11 14:04 xdmod_data/__init__.py
--rw-r--r--  2.0 unx       54 b- defN 23-Jul-12 14:14 xdmod_data/__version__.py
+-rw-r--r--  2.0 unx       54 b- defN 23-Jul-12 14:21 xdmod_data/__version__.py
 -rw-r--r--  2.0 unx     2262 b- defN 23-Jul-11 14:04 xdmod_data/_descriptors.py
 -rw-r--r--  2.0 unx     5230 b- defN 23-Jul-11 14:04 xdmod_data/_http_requester.py
 -rw-r--r--  2.0 unx     4435 b- defN 23-Jul-11 14:04 xdmod_data/_response_processor.py
 -rw-r--r--  2.0 unx    10394 b- defN 23-Jul-11 14:04 xdmod_data/_validator.py
 -rw-r--r--  2.0 unx     3018 b- defN 23-Jul-11 14:04 xdmod_data/themes.py
 -rw-r--r--  2.0 unx    16931 b- defN 23-Jul-11 14:04 xdmod_data/warehouse.py
--rw-r--r--  2.0 unx     7652 b- defN 23-Jul-12 14:17 xdmod_data-1.0.0b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3552 b- defN 23-Jul-12 14:17 xdmod_data-1.0.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 14:17 xdmod_data-1.0.0b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-12 14:17 xdmod_data-1.0.0b1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1067 b- defN 23-Jul-12 14:17 xdmod_data-1.0.0b1.dist-info/RECORD
-13 files, 54735 bytes uncompressed, 14484 bytes compressed:  73.5%
+-rw-r--r--  2.0 unx     7652 b- defN 23-Jul-12 14:21 xdmod_data-1.0.0b2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3565 b- defN 23-Jul-12 14:21 xdmod_data-1.0.0b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 14:21 xdmod_data-1.0.0b2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-12 14:21 xdmod_data-1.0.0b2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1067 b- defN 23-Jul-12 14:21 xdmod_data-1.0.0b2.dist-info/RECORD
+13 files, 54748 bytes uncompressed, 14486 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: xdmod_data/themes.py
 Comment: 
 
 Filename: xdmod_data/warehouse.py
 Comment: 
 
-Filename: xdmod_data-1.0.0b1.dist-info/LICENSE
+Filename: xdmod_data-1.0.0b2.dist-info/LICENSE
 Comment: 
 
-Filename: xdmod_data-1.0.0b1.dist-info/METADATA
+Filename: xdmod_data-1.0.0b2.dist-info/METADATA
 Comment: 
 
-Filename: xdmod_data-1.0.0b1.dist-info/WHEEL
+Filename: xdmod_data-1.0.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: xdmod_data-1.0.0b1.dist-info/top_level.txt
+Filename: xdmod_data-1.0.0b2.dist-info/top_level.txt
 Comment: 
 
-Filename: xdmod_data-1.0.0b1.dist-info/RECORD
+Filename: xdmod_data-1.0.0b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xdmod_data/__version__.py

```diff
@@ -1,2 +1,2 @@
 __title__ = 'xdmod-data'
-__version__ = '1.0.0-beta.1'
+__version__ = '1.0.0-beta.2'
```

## Comparing `xdmod_data-1.0.0b1.dist-info/LICENSE` & `xdmod_data-1.0.0b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xdmod_data-1.0.0b1.dist-info/METADATA` & `xdmod_data-1.0.0b2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xdmod-data
-Version: 1.0.0b1
-Summary: Python driver for XDMoD
+Version: 1.0.0b2
+Summary: Python package for XDMoD data access
 Author: Aaron Weeden, Joseph P. White
 Maintainer: Aaron Weeden, Joseph P. White
 Project-URL: Source Code, https://github.com/ubccr/xdmod-data
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

## Comparing `xdmod_data-1.0.0b1.dist-info/RECORD` & `xdmod_data-1.0.0b2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 xdmod_data/__init__.py,sha256=e3S0EcDGJlWIp2hddSFjvt633jfeZ4W7VyAeLpfTWVM,37
-xdmod_data/__version__.py,sha256=j9K_YQ0EIq7Tnl7R50G5_cMz8X3F7ffmAQ1pT9PhUZE,54
+xdmod_data/__version__.py,sha256=bz7f9HabhHs5HR38K_H-vdFeq6-ygAL81-zUY7mbKjI,54
 xdmod_data/_descriptors.py,sha256=uUbC65oW5Vur-DhFEs__NrYTpCt5FrngTYVgu08FgwE,2262
 xdmod_data/_http_requester.py,sha256=7936UGqjrKrW4vY0bEsONRx0CYfPQojr-YEVieEkosg,5230
 xdmod_data/_response_processor.py,sha256=Vslz3-DtlhhoukJ11yJWcLi0wIcZSCIHMLlETzA9WEU,4435
 xdmod_data/_validator.py,sha256=GWHH_U5r_QVcZG9C_yo1xMGoxIFXmC__5l94-hqLcPE,10394
 xdmod_data/themes.py,sha256=eSD7_dJsFhiB3qrMW7FP54IFPXh9tr1XjHXIB6nvx-c,3018
 xdmod_data/warehouse.py,sha256=W7vMIAp_BiKEa15oipiRfZRmVBTfShqie4hFuj6TMdQ,16931
-xdmod_data-1.0.0b1.dist-info/LICENSE,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
-xdmod_data-1.0.0b1.dist-info/METADATA,sha256=v9cDkrdK8XDFbP0g2YuHfyT7T-ttdWRzlUr0anWrYBE,3552
-xdmod_data-1.0.0b1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-xdmod_data-1.0.0b1.dist-info/top_level.txt,sha256=ph-NOi5tK19CfM5XnNOGuId1orUYaKQPxOPiS-geLPk,11
-xdmod_data-1.0.0b1.dist-info/RECORD,,
+xdmod_data-1.0.0b2.dist-info/LICENSE,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
+xdmod_data-1.0.0b2.dist-info/METADATA,sha256=WhbreDE-73dxjd9tItVg2BLM0ywHFt8FCl3QenQSR70,3565
+xdmod_data-1.0.0b2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+xdmod_data-1.0.0b2.dist-info/top_level.txt,sha256=ph-NOi5tK19CfM5XnNOGuId1orUYaKQPxOPiS-geLPk,11
+xdmod_data-1.0.0b2.dist-info/RECORD,,
```

