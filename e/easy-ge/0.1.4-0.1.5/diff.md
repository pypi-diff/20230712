# Comparing `tmp/easy_ge-0.1.4.tar.gz` & `tmp/easy_ge-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ge-0.1.4.tar", max compression
+gzip compressed data, was "easy_ge-0.1.5.tar", max compression
```

## Comparing `easy_ge-0.1.4.tar` & `easy_ge-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1059 2023-07-12 08:26:49.044542 easy_ge-0.1.4/LICENSE
--rw-r--r--   0        0        0       86 2023-07-12 09:36:20.503745 easy_ge-0.1.4/easy_ge/__init__.py
--rw-r--r--   0        0        0     5477 2023-07-12 09:41:47.853681 easy_ge-0.1.4/easy_ge/expectation_manager.py
--rw-r--r--   0        0        0     3997 2023-07-12 08:01:08.794839 easy_ge-0.1.4/easy_ge/helpers.py
--rw-r--r--   0        0        0     1821 2023-07-12 09:47:40.673614 easy_ge-0.1.4/easy_ge/main.py
--rw-r--r--   0        0        0      908 2023-07-11 19:54:36.830184 easy_ge-0.1.4/easy_ge/templates/checkpoint.tpl
--rw-r--r--   0        0        0     3287 2023-07-11 20:05:32.078164 easy_ge-0.1.4/easy_ge/templates/great_expectations.tpl
--rw-r--r--   0        0        0     4705 2023-07-11 19:59:36.076319 easy_ge-0.1.4/easy_ge/templates/schema.json
--rw-r--r--   0        0        0     1046 2023-07-12 10:36:09.153049 easy_ge-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 10:14:43.883302 easy_ge-0.1.4/readme.md
--rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 easy_ge-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-12 08:26:49.044542 easy_ge-0.1.5/LICENSE
+-rw-r--r--   0        0        0       86 2023-07-12 09:36:20.503745 easy_ge-0.1.5/easy_ge/__init__.py
+-rw-r--r--   0        0        0     5477 2023-07-12 09:41:47.853681 easy_ge-0.1.5/easy_ge/expectation_manager.py
+-rw-r--r--   0        0        0     3997 2023-07-12 08:01:08.794839 easy_ge-0.1.5/easy_ge/helpers.py
+-rw-r--r--   0        0        0     1821 2023-07-12 09:47:40.673614 easy_ge-0.1.5/easy_ge/main.py
+-rw-r--r--   0        0        0      908 2023-07-11 19:54:36.830184 easy_ge-0.1.5/easy_ge/templates/checkpoint.tpl
+-rw-r--r--   0        0        0     3287 2023-07-11 20:05:32.078164 easy_ge-0.1.5/easy_ge/templates/great_expectations.tpl
+-rw-r--r--   0        0        0     4705 2023-07-11 19:59:36.076319 easy_ge-0.1.5/easy_ge/templates/schema.json
+-rw-r--r--   0        0        0     1047 2023-07-12 10:37:57.203031 easy_ge-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 10:14:43.883302 easy_ge-0.1.5/readme.md
+-rw-r--r--   0        0        0     1025 1970-01-01 00:00:00.000000 easy_ge-0.1.5/PKG-INFO
```

### Comparing `easy_ge-0.1.4/LICENSE` & `easy_ge-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.4/easy_ge/expectation_manager.py` & `easy_ge-0.1.5/easy_ge/expectation_manager.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.4/easy_ge/helpers.py` & `easy_ge-0.1.5/easy_ge/helpers.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.4/easy_ge/main.py` & `easy_ge-0.1.5/easy_ge/main.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.4/easy_ge/templates/checkpoint.tpl` & `easy_ge-0.1.5/easy_ge/templates/checkpoint.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.4/easy_ge/templates/great_expectations.tpl` & `easy_ge-0.1.5/easy_ge/templates/great_expectations.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.4/easy_ge/templates/schema.json` & `easy_ge-0.1.5/easy_ge/templates/schema.json`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.4/PKG-INFO` & `easy_ge-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: easy-ge
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases.
 Author: Elsayed91
 Author-email: elsayed.is@outlook.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: aws
 Provides-Extra: google
 Requires-Dist: fsspec (>=2023.6.0,<2024.0.0)
 Requires-Dist: gcsfs (>=2023.6.0,<2024.0.0) ; extra == "google"
 Requires-Dist: google-cloud-secret-manager (>=2.16.2,<3.0.0) ; extra == "google"
```

