# Comparing `tmp/easy_ge-0.1.2.tar.gz` & `tmp/easy_ge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ge-0.1.2.tar", max compression
+gzip compressed data, was "easy_ge-0.1.3.tar", max compression
```

## Comparing `easy_ge-0.1.2.tar` & `easy_ge-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1059 2023-07-12 08:26:49.044542 easy_ge-0.1.2/LICENSE
--rw-r--r--   0        0        0       86 2023-07-12 09:36:20.503745 easy_ge-0.1.2/easy_ge/__init__.py
--rw-r--r--   0        0        0     5477 2023-07-12 09:41:47.853681 easy_ge-0.1.2/easy_ge/expectation_manager.py
--rw-r--r--   0        0        0     3997 2023-07-12 08:01:08.794839 easy_ge-0.1.2/easy_ge/helpers.py
--rw-r--r--   0        0        0     1821 2023-07-12 09:47:40.673614 easy_ge-0.1.2/easy_ge/main.py
--rw-r--r--   0        0        0      908 2023-07-11 19:54:36.830184 easy_ge-0.1.2/easy_ge/templates/checkpoint.tpl
--rw-r--r--   0        0        0     3287 2023-07-11 20:05:32.078164 easy_ge-0.1.2/easy_ge/templates/great_expectations.tpl
--rw-r--r--   0        0        0     4705 2023-07-11 19:59:36.076319 easy_ge-0.1.2/easy_ge/templates/schema.json
--rw-r--r--   0        0        0     1017 2023-07-12 10:14:49.073301 easy_ge-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 10:14:43.883302 easy_ge-0.1.2/readme.md
--rw-r--r--   0        0        0      934 1970-01-01 00:00:00.000000 easy_ge-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-12 08:26:49.044542 easy_ge-0.1.3/LICENSE
+-rw-r--r--   0        0        0       86 2023-07-12 09:36:20.503745 easy_ge-0.1.3/easy_ge/__init__.py
+-rw-r--r--   0        0        0     5477 2023-07-12 09:41:47.853681 easy_ge-0.1.3/easy_ge/expectation_manager.py
+-rw-r--r--   0        0        0     3997 2023-07-12 08:01:08.794839 easy_ge-0.1.3/easy_ge/helpers.py
+-rw-r--r--   0        0        0     1821 2023-07-12 09:47:40.673614 easy_ge-0.1.3/easy_ge/main.py
+-rw-r--r--   0        0        0      908 2023-07-11 19:54:36.830184 easy_ge-0.1.3/easy_ge/templates/checkpoint.tpl
+-rw-r--r--   0        0        0     3287 2023-07-11 20:05:32.078164 easy_ge-0.1.3/easy_ge/templates/great_expectations.tpl
+-rw-r--r--   0        0        0     4705 2023-07-11 19:59:36.076319 easy_ge-0.1.3/easy_ge/templates/schema.json
+-rw-r--r--   0        0        0     1127 2023-07-12 10:28:29.473137 easy_ge-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 10:14:43.883302 easy_ge-0.1.3/readme.md
+-rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 easy_ge-0.1.3/PKG-INFO
```

### Comparing `easy_ge-0.1.2/LICENSE` & `easy_ge-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.2/easy_ge/expectation_manager.py` & `easy_ge-0.1.3/easy_ge/expectation_manager.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.2/easy_ge/helpers.py` & `easy_ge-0.1.3/easy_ge/helpers.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.2/easy_ge/main.py` & `easy_ge-0.1.3/easy_ge/main.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.2/easy_ge/templates/checkpoint.tpl` & `easy_ge-0.1.3/easy_ge/templates/checkpoint.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.2/easy_ge/templates/great_expectations.tpl` & `easy_ge-0.1.3/easy_ge/templates/great_expectations.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.2/easy_ge/templates/schema.json` & `easy_ge-0.1.3/easy_ge/templates/schema.json`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.2/pyproject.toml` & `easy_ge-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "easy_ge"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases."
 authors = ["Elsayed91 <elsayed.is@outlook.com>"]
 readme = "readme.md"
 packages = [{include = "easy_ge"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 great-expectations = "^0.17.4"
 pyyaml = "^6.0"
 jsonschema = "^4.18.0"
 jinja2 = "^3.1.2"
 google-cloud-storage = {version = "^2.10.0", extras = ["google"], optional = true}
 google-cloud-secret-manager = {version = "^2.16.2", extras = ["google"], optional = true}
 pyarrow = "^12.0.1"
@@ -19,14 +19,18 @@
 gcsfs = {version = "^2023.6.0", extras = ["google"], optional = true}
 s3fs = {version = "^2023.6.0", extras = ["aws"], optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 
+[tool.poetry.extras]
+aws = ["s3fs"]
+google = ["google-cloud-secret-manager", "google-cloud-storage", "gcsfs"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 filterwarnings = "ignore::DeprecationWarning"
 pythonpath = "."
```

### Comparing `easy_ge-0.1.2/PKG-INFO` & `easy_ge-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: easy-ge
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases.
 Author: Elsayed91
 Author-email: elsayed.is@outlook.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: aws
+Provides-Extra: google
 Requires-Dist: fsspec (>=2023.6.0,<2024.0.0)
-Requires-Dist: gcsfs[google] (>=2023.6.0,<2024.0.0)
-Requires-Dist: google-cloud-secret-manager[google] (>=2.16.2,<3.0.0)
-Requires-Dist: google-cloud-storage[google] (>=2.10.0,<3.0.0)
+Requires-Dist: gcsfs[google] (>=2023.6.0,<2024.0.0) ; extra == "google"
+Requires-Dist: google-cloud-secret-manager[google] (>=2.16.2,<3.0.0) ; extra == "google"
+Requires-Dist: google-cloud-storage[google] (>=2.10.0,<3.0.0) ; extra == "google"
 Requires-Dist: great-expectations (>=0.17.4,<0.18.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.18.0,<5.0.0)
 Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: s3fs[aws] (>=2023.6.0,<2024.0.0)
+Requires-Dist: s3fs[aws] (>=2023.6.0,<2024.0.0) ; extra == "aws"
 Description-Content-Type: text/markdown
```

