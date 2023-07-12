# Comparing `tmp/re_action_template-2.1.2-py3-none-any.whl.zip` & `tmp/re_action_template-2.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 14523 bytes, number of entries: 8
+Zip file size: 14484 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 action_template/__init__.py
 -rwxr-xr-x  2.0 unx      156 b- defN 80-Jan-01 00:00 action_template/__main__.py
 -rw-r--r--  2.0 unx     2259 b- defN 80-Jan-01 00:00 action_template/main.py
--rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_action_template-2.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4308 b- defN 80-Jan-01 00:00 re_action_template-2.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_action_template-2.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 re_action_template-2.1.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      689 b- defN 16-Jan-01 00:00 re_action_template-2.1.2.dist-info/RECORD
-8 files, 38148 bytes uncompressed, 13305 bytes compressed:  65.1%
+-rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_action_template-2.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4229 b- defN 80-Jan-01 00:00 re_action_template-2.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_action_template-2.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 re_action_template-2.1.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      689 b- defN 16-Jan-01 00:00 re_action_template-2.1.3.dist-info/RECORD
+8 files, 38069 bytes uncompressed, 13266 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: action_template/__main__.py
 Comment: 
 
 Filename: action_template/main.py
 Comment: 
 
-Filename: re_action_template-2.1.2.dist-info/LICENSE
+Filename: re_action_template-2.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: re_action_template-2.1.2.dist-info/METADATA
+Filename: re_action_template-2.1.3.dist-info/METADATA
 Comment: 
 
-Filename: re_action_template-2.1.2.dist-info/WHEEL
+Filename: re_action_template-2.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: re_action_template-2.1.2.dist-info/entry_points.txt
+Filename: re_action_template-2.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: re_action_template-2.1.2.dist-info/RECORD
+Filename: re_action_template-2.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `re_action_template-2.1.2.dist-info/LICENSE` & `re_action_template-2.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `re_action_template-2.1.2.dist-info/METADATA` & `re_action_template-2.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-action-template
-Version: 2.1.2
+Version: 2.1.3
 Summary: 
 License: SSPL-1.0
 Author: Philipp Gayret
 Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -176,13 +176,11 @@
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

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: re-action-template Version: 2.1.2 Summary: License:
+Metadata-Version: 2.1 Name: re-action-template Version: 2.1.3 Summary: License:
 SSPL-1.0 Author: Philipp Gayret Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: Markdown (>=3.3.6,<4.0.0) Requires-
 Dist: fire (>=0.5.0,<0.6.0) Requires-Dist: jinja2 (>=3.0.3,<4.0.0) Requires-
 Dist: pyyaml (>=6.0,<7.0) Description-Content-Type: text/markdown  # release-
 engineers/action-template [![Status: Production ready](https://img.shields.io/
@@ -45,10 +45,9 @@
 {'level': 2, 'id': 'header-two', 'name': 'Header Two', 'children': [{'level':
 3, 'id': 'header-three', 'name': 'Header Three', 'children': []}, {'level': 3,
 'id': 'header-three-two', 'name': 'Header Three, Two', 'children': []}]}]}] ```
 ## Contributing This is a Python Poetry project using [Fire](https://
 github.com/google/python-fire). See [Poetry](https://python-poetry.org/) for
 more information. Development requires: - Bash - [Docker](https://
 www.docker.com/) - [Python](https://www.python.org/) - [Poetry](https://python-
-poetry.org/) See [`app.sh`](./app.sh) for building, running and releasing the
-application. ## Links This project was created using [template-poetry](https://
+poetry.org/) ## Links This project was created using [template-poetry](https://
 github.com/release-engineers/template-poetry).
```

