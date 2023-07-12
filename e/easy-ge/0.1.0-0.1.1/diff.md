# Comparing `tmp/easy_ge-0.1.0.tar.gz` & `tmp/easy_ge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ge-0.1.0.tar", max compression
+gzip compressed data, was "easy_ge-0.1.1.tar", max compression
```

## Comparing `easy_ge-0.1.0.tar` & `easy_ge-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1059 2023-07-12 08:26:49.044542 easy_ge-0.1.0/LICENSE
--rw-r--r--   0        0        0     3781 2023-07-12 08:54:34.844225 easy_ge-0.1.0/README.md
--rw-r--r--   0        0        0       86 2023-07-12 09:36:20.503745 easy_ge-0.1.0/easy_ge/__init__.py
--rw-r--r--   0        0        0     5477 2023-07-12 09:41:47.853681 easy_ge-0.1.0/easy_ge/expectation_manager.py
--rw-r--r--   0        0        0     3997 2023-07-12 08:01:08.794839 easy_ge-0.1.0/easy_ge/helpers.py
--rw-r--r--   0        0        0     1821 2023-07-12 09:47:40.673614 easy_ge-0.1.0/easy_ge/main.py
--rw-r--r--   0        0        0      908 2023-07-11 19:54:36.830184 easy_ge-0.1.0/easy_ge/templates/checkpoint.tpl
--rw-r--r--   0        0        0     3287 2023-07-11 20:05:32.078164 easy_ge-0.1.0/easy_ge/templates/great_expectations.tpl
--rw-r--r--   0        0        0     4705 2023-07-11 19:59:36.076319 easy_ge-0.1.0/easy_ge/templates/schema.json
--rw-r--r--   0        0        0      949 2023-07-12 10:00:16.483464 easy_ge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4715 1970-01-01 00:00:00.000000 easy_ge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-12 08:26:49.044542 easy_ge-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3781 2023-07-12 08:54:34.844225 easy_ge-0.1.1/README.md
+-rw-r--r--   0        0        0       86 2023-07-12 09:36:20.503745 easy_ge-0.1.1/easy_ge/__init__.py
+-rw-r--r--   0        0        0     5477 2023-07-12 09:41:47.853681 easy_ge-0.1.1/easy_ge/expectation_manager.py
+-rw-r--r--   0        0        0     3997 2023-07-12 08:01:08.794839 easy_ge-0.1.1/easy_ge/helpers.py
+-rw-r--r--   0        0        0     1821 2023-07-12 09:47:40.673614 easy_ge-0.1.1/easy_ge/main.py
+-rw-r--r--   0        0        0      908 2023-07-11 19:54:36.830184 easy_ge-0.1.1/easy_ge/templates/checkpoint.tpl
+-rw-r--r--   0        0        0     3287 2023-07-11 20:05:32.078164 easy_ge-0.1.1/easy_ge/templates/great_expectations.tpl
+-rw-r--r--   0        0        0     4705 2023-07-11 19:59:36.076319 easy_ge-0.1.1/easy_ge/templates/schema.json
+-rw-r--r--   0        0        0     1017 2023-07-12 10:08:10.613379 easy_ge-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4715 1970-01-01 00:00:00.000000 easy_ge-0.1.1/PKG-INFO
```

### Comparing `easy_ge-0.1.0/LICENSE` & `easy_ge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.0/README.md` & `easy_ge-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.0/easy_ge/expectation_manager.py` & `easy_ge-0.1.1/easy_ge/expectation_manager.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.0/easy_ge/helpers.py` & `easy_ge-0.1.1/easy_ge/helpers.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.0/easy_ge/main.py` & `easy_ge-0.1.1/easy_ge/main.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.0/easy_ge/templates/checkpoint.tpl` & `easy_ge-0.1.1/easy_ge/templates/checkpoint.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.0/easy_ge/templates/great_expectations.tpl` & `easy_ge-0.1.1/easy_ge/templates/great_expectations.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.0/easy_ge/templates/schema.json` & `easy_ge-0.1.1/easy_ge/templates/schema.json`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.0/pyproject.toml` & `easy_ge-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "easy_ge"
-version = "0.1.0"
+version = "0.1.1"
 description = "A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases."
 authors = ["Elsayed91 <elsayed.is@outlook.com>"]
 readme = "README.md"
 packages = [{include = "easy_ge"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 great-expectations = "^0.17.4"
 pyyaml = "^6.0"
 jsonschema = "^4.18.0"
 jinja2 = "^3.1.2"
-google-cloud-storage = {version = "^2.10.0", extras = ["google"]}
-google-cloud-secret-manager = {version = "^2.16.2", extras = ["google"]}
+google-cloud-storage = {version = "^2.10.0", extras = ["google"], optional = true}
+google-cloud-secret-manager = {version = "^2.16.2", extras = ["google"], optional = true}
 pyarrow = "^12.0.1"
 fsspec = "^2023.6.0"
-gcsfs = {version = "^2023.6.0", extras = ["google"]}
-s3fs = {version = "^2023.6.0", extras = ["aws"]}
+gcsfs = {version = "^2023.6.0", extras = ["google"], optional = true}
+s3fs = {version = "^2023.6.0", extras = ["aws"], optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `easy_ge-0.1.0/PKG-INFO` & `easy_ge-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ge
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases.
 Author: Elsayed91
 Author-email: elsayed.is@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: easy-ge Version: 0.1.0 Summary: A package that
+Metadata-Version: 2.1 Name: easy-ge Version: 0.1.1 Summary: A package that
 abstracts the complexity of Great Expectations away. At least for straight
 forward use cases. Author: Elsayed91 Author-email: elsayed.is@outlook.com
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: fsspec (>=2023.6.0,<2024.0.0)
 Requires-Dist: gcsfs[google] (>=2023.6.0,<2024.0.0) Requires-Dist: google-
 cloud-secret-manager[google] (>=2.16.2,<3.0.0) Requires-Dist: google-cloud-
```

