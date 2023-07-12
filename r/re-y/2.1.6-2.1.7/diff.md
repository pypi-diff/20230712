# Comparing `tmp/re_y-2.1.6-py3-none-any.whl.zip` & `tmp/re_y-2.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17896 bytes, number of entries: 9
+Zip file size: 17895 bytes, number of entries: 9
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 y/__init__.py
 -rwxr-xr-x  2.0 unx     2575 b- defN 80-Jan-01 00:00 y/__main__.py
 -rwxr-xr-x  2.0 unx    10305 b- defN 80-Jan-01 00:00 y/yinterpreter.py
 -rwxr-xr-x  2.0 unx     3962 b- defN 80-Jan-01 00:00 y/yreference.py
--rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_y-2.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     5130 b- defN 80-Jan-01 00:00 re_y-2.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_y-2.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 re_y-2.1.6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      659 b- defN 16-Jan-01 00:00 re_y-2.1.6.dist-info/RECORD
-9 files, 53339 bytes uncompressed, 16780 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_y-2.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5130 b- defN 80-Jan-01 00:00 re_y-2.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_y-2.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 re_y-2.1.7.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      659 b- defN 16-Jan-01 00:00 re_y-2.1.7.dist-info/RECORD
+9 files, 53339 bytes uncompressed, 16779 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: y/yinterpreter.py
 Comment: 
 
 Filename: y/yreference.py
 Comment: 
 
-Filename: re_y-2.1.6.dist-info/LICENSE
+Filename: re_y-2.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: re_y-2.1.6.dist-info/METADATA
+Filename: re_y-2.1.7.dist-info/METADATA
 Comment: 
 
-Filename: re_y-2.1.6.dist-info/WHEEL
+Filename: re_y-2.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: re_y-2.1.6.dist-info/entry_points.txt
+Filename: re_y-2.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: re_y-2.1.6.dist-info/RECORD
+Filename: re_y-2.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `re_y-2.1.6.dist-info/LICENSE` & `re_y-2.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `re_y-2.1.6.dist-info/METADATA` & `re_y-2.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: re-y
-Version: 2.1.6
+Version: 2.1.7
 Summary: 
 License: SSPL-1.0
 Author: Philipp Gayret
 Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lark (==1.1.5)
-Requires-Dist: ruamel.yaml (==0.17.21)
+Requires-Dist: ruamel.yaml (==0.17.32)
 Description-Content-Type: text/markdown
 
 <!-- README.md is auto-generated from README.md.template -->
 
 # release-engineers/y
 
 [![Status: Beta](https://img.shields.io/badge/status-beta-orange)](https://release-engineers.com/open-source-badges/)
```

## Comparing `re_y-2.1.6.dist-info/RECORD` & `re_y-2.1.7.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 y/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 y/__main__.py,sha256=H-bgfmFPaKa8KMp_MzqJbSEkoKxmYeTpZJTgf3LT3HE,2575
 y/yinterpreter.py,sha256=VjZvNQYyZ1yISTleo2hl1V-YmHrW2w_wweJzX61Yo-Y,10305
 y/yreference.py,sha256=Yqa_wVAUDoDkGWAALtBUdd0hGngzQzgZvxJEDFiFzag,3962
-re_y-2.1.6.dist-info/LICENSE,sha256=Jp0_6oDvg99Q72hGqp1nWkxHMRdlBra9z78CDwD4yLs,30583
-re_y-2.1.6.dist-info/METADATA,sha256=Len6CYENzpSQUyDmyaLuKREoLXeW4mQgIh7dIqbUzzc,5130
-re_y-2.1.6.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-re_y-2.1.6.dist-info/entry_points.txt,sha256=40UjBWjwL8Szi65DOA03p4EzqFIIj1GPUH1qw6eURpM,37
-re_y-2.1.6.dist-info/RECORD,,
+re_y-2.1.7.dist-info/LICENSE,sha256=Jp0_6oDvg99Q72hGqp1nWkxHMRdlBra9z78CDwD4yLs,30583
+re_y-2.1.7.dist-info/METADATA,sha256=6naWazMc7A1_2tgQ1-TzBjHsfjtIPmN2zJPyTPFvocg,5130
+re_y-2.1.7.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+re_y-2.1.7.dist-info/entry_points.txt,sha256=40UjBWjwL8Szi65DOA03p4EzqFIIj1GPUH1qw6eURpM,37
+re_y-2.1.7.dist-info/RECORD,,
```

