# Comparing `tmp/re_yaml_common-2.0.3-py3-none-any.whl.zip` & `tmp/re_yaml_common-2.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15324 bytes, number of entries: 10
+Zip file size: 15287 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 yaml_common/__init__.py
 -rwxr-xr-x  2.0 unx      148 b- defN 80-Jan-01 00:00 yaml_common/__main__.py
 -rw-r--r--  2.0 unx     2190 b- defN 80-Jan-01 00:00 yaml_common/libcommon.py
 -rw-r--r--  2.0 unx     2110 b- defN 80-Jan-01 00:00 yaml_common/libmerge.py
 -rw-r--r--  2.0 unx      785 b- defN 80-Jan-01 00:00 yaml_common/main.py
--rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4693 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      817 b- defN 16-Jan-01 00:00 re_yaml_common-2.0.3.dist-info/RECORD
-10 files, 41471 bytes uncompressed, 13924 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4614 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      817 b- defN 16-Jan-01 00:00 re_yaml_common-2.0.4.dist-info/RECORD
+10 files, 41392 bytes uncompressed, 13887 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: yaml_common/libmerge.py
 Comment: 
 
 Filename: yaml_common/main.py
 Comment: 
 
-Filename: re_yaml_common-2.0.3.dist-info/LICENSE
+Filename: re_yaml_common-2.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: re_yaml_common-2.0.3.dist-info/METADATA
+Filename: re_yaml_common-2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: re_yaml_common-2.0.3.dist-info/WHEEL
+Filename: re_yaml_common-2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: re_yaml_common-2.0.3.dist-info/entry_points.txt
+Filename: re_yaml_common-2.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: re_yaml_common-2.0.3.dist-info/RECORD
+Filename: re_yaml_common-2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `re_yaml_common-2.0.3.dist-info/LICENSE` & `re_yaml_common-2.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `re_yaml_common-2.0.3.dist-info/METADATA` & `re_yaml_common-2.0.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-yaml-common
-Version: 2.0.3
+Version: 2.0.4
 Summary: 
 License: SSPL-1.0
 Author: Philipp Gayret
 Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -197,13 +197,11 @@
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

## Comparing `re_yaml_common-2.0.3.dist-info/RECORD` & `re_yaml_common-2.0.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 yaml_common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 yaml_common/__main__.py,sha256=re0xzAbZwMzgQVZtDssRF4p3svJbEgf8m3CeOuuODdw,148
 yaml_common/libcommon.py,sha256=SxwkAC3r4t3fOOoIQ0xBd7ZtWLKxKx00_ydVa3tptbY,2190
 yaml_common/libmerge.py,sha256=Kwiq5_oDtZSyXkDJHHJ5K4duEQYiHz3gJfE3_DRVC1U,2110
 yaml_common/main.py,sha256=wxl-okiSn4VU_z3A0e5WYLzpLtlR-umUoVY3CeFGv6Q,785
-re_yaml_common-2.0.3.dist-info/LICENSE,sha256=Jp0_6oDvg99Q72hGqp1nWkxHMRdlBra9z78CDwD4yLs,30583
-re_yaml_common-2.0.3.dist-info/METADATA,sha256=FNA_DIe2KJnJqYoStOHMWKXbVzE5GSUfe8k0IFS0esk,4693
-re_yaml_common-2.0.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-re_yaml_common-2.0.3.dist-info/entry_points.txt,sha256=mvvDourzPiSQLF2FrOOFispRrzVwoHHtv2aTpaVEYwg,57
-re_yaml_common-2.0.3.dist-info/RECORD,,
+re_yaml_common-2.0.4.dist-info/LICENSE,sha256=Jp0_6oDvg99Q72hGqp1nWkxHMRdlBra9z78CDwD4yLs,30583
+re_yaml_common-2.0.4.dist-info/METADATA,sha256=Fy_jHkQvVXGVQfUrHAvTEcnztJRnEnniSEM7hF74MTc,4614
+re_yaml_common-2.0.4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+re_yaml_common-2.0.4.dist-info/entry_points.txt,sha256=mvvDourzPiSQLF2FrOOFispRrzVwoHHtv2aTpaVEYwg,57
+re_yaml_common-2.0.4.dist-info/RECORD,,
```

