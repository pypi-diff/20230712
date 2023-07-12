# Comparing `tmp/pylint_pydantic-0.2.0-py3-none-any.whl.zip` & `tmp/pylint_pydantic-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14910 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1857 b- defN 23-Jul-04 03:46 pylint_pydantic/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1833 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      511 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/RECORD
-6 files, 39458 bytes uncompressed, 13980 bytes compressed:  64.6%
+Zip file size: 14930 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1876 b- defN 23-Jul-12 01:41 pylint_pydantic/__init__.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1869 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      511 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/RECORD
+6 files, 39513 bytes uncompressed, 14000 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pylint_pydantic/__init__.py
 Comment: 
 
-Filename: pylint_pydantic-0.2.0.dist-info/LICENSE
+Filename: pylint_pydantic-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: pylint_pydantic-0.2.0.dist-info/METADATA
+Filename: pylint_pydantic-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: pylint_pydantic-0.2.0.dist-info/WHEEL
+Filename: pylint_pydantic-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: pylint_pydantic-0.2.0.dist-info/top_level.txt
+Filename: pylint_pydantic-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pylint_pydantic-0.2.0.dist-info/RECORD
+Filename: pylint_pydantic-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylint_pydantic/__init__.py

```diff
@@ -1,13 +1,13 @@
 import astroid
 from astroid import (MANAGER, Attribute, Call, ClassDef, FunctionDef, Name, nodes)
 from pylint.checkers.design_analysis import MisdesignChecker
 from pylint_plugin_utils import suppress_message
 
-VALIDATOR_METHOD_NAMES = {"validator", "root_validator", "field_validator"}
+VALIDATOR_METHOD_NAMES = {"validator", "root_validator", "field_validator", "model_validator"}
 
 
 def is_validator_method(node: FunctionDef):
 
     if not node.decorators:
         return False
```

## Comparing `pylint_pydantic-0.2.0.dist-info/LICENSE` & `pylint_pydantic-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylint_pydantic-0.2.0.dist-info/METADATA` & `pylint_pydantic-0.2.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-pydantic
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Pylint plugin to help Pylint understand the Pydantic
 Home-page: https://github.com/fcfangcc/pylint-pydantic
 Author: fcfangcc
 Author-email: swjfc22@163.com
 License: GPLv3
 Keywords: pylint,pydantic
 Platform: UNKNOWN
@@ -64,9 +64,10 @@
 If you have any questions, please create a issue.
 https://github.com/fcfangcc/pylint-pydantic/issues
 
 
 Changelog
 =====================
 - v0.2.0: support Pydantic V2
+- v0.2.1: support `model_validator`
```

