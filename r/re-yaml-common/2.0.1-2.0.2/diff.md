# Comparing `tmp/re_yaml_common-2.0.1-py3-none-any.whl.zip` & `tmp/re_yaml_common-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15293 bytes, number of entries: 10
+Zip file size: 15325 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 yaml_common/__init__.py
 -rwxr-xr-x  2.0 unx      148 b- defN 80-Jan-01 00:00 yaml_common/__main__.py
 -rw-r--r--  2.0 unx     2190 b- defN 80-Jan-01 00:00 yaml_common/libcommon.py
 -rw-r--r--  2.0 unx     2110 b- defN 80-Jan-01 00:00 yaml_common/libmerge.py
 -rw-r--r--  2.0 unx      785 b- defN 80-Jan-01 00:00 yaml_common/main.py
--rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4589 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      817 b- defN 16-Jan-01 00:00 re_yaml_common-2.0.1.dist-info/RECORD
-10 files, 41367 bytes uncompressed, 13893 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4693 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 re_yaml_common-2.0.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      817 b- defN 16-Jan-01 00:00 re_yaml_common-2.0.2.dist-info/RECORD
+10 files, 41471 bytes uncompressed, 13925 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: yaml_common/libmerge.py
 Comment: 
 
 Filename: yaml_common/main.py
 Comment: 
 
-Filename: re_yaml_common-2.0.1.dist-info/LICENSE
+Filename: re_yaml_common-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: re_yaml_common-2.0.1.dist-info/METADATA
+Filename: re_yaml_common-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: re_yaml_common-2.0.1.dist-info/WHEEL
+Filename: re_yaml_common-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: re_yaml_common-2.0.1.dist-info/entry_points.txt
+Filename: re_yaml_common-2.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: re_yaml_common-2.0.1.dist-info/RECORD
+Filename: re_yaml_common-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `re_yaml_common-2.0.1.dist-info/LICENSE` & `re_yaml_common-2.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `re_yaml_common-2.0.1.dist-info/METADATA` & `re_yaml_common-2.0.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-yaml-common
-Version: 2.0.1
+Version: 2.0.2
 Summary: 
 License: SSPL-1.0
 Author: Philipp Gayret
 Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Description-Content-Type: text/markdown
 
 <!-- README.md is auto-generated from README.md.template -->
 
 # release-engineers/yaml-common
 
 [![Status: Production ready](https://img.shields.io/badge/status-production_ready-green)](https://release-engineers.com/open-source-badges/)
+[![PyPI version](https://badge.fury.io/py/re-yaml-common.svg)](https://badge.fury.io/py/re-yaml-common)
 
 Extracts and merges common parts of YAML from one set of files into a common file.
 Note that this project attempts to preserve comments and order of properties in your YAML files, but can not preserve formatting.
 
 ## Setup
 
 ```bash
```

