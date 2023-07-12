# Comparing `tmp/easy_ge-0.1.1.tar.gz` & `tmp/easy_ge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ge-0.1.1.tar", max compression
+gzip compressed data, was "easy_ge-0.1.2.tar", max compression
```

## Comparing `easy_ge-0.1.1.tar` & `easy_ge-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1059 2023-07-12 08:26:49.044542 easy_ge-0.1.1/LICENSE
--rw-r--r--   0        0        0     3781 2023-07-12 08:54:34.844225 easy_ge-0.1.1/README.md
--rw-r--r--   0        0        0       86 2023-07-12 09:36:20.503745 easy_ge-0.1.1/easy_ge/__init__.py
--rw-r--r--   0        0        0     5477 2023-07-12 09:41:47.853681 easy_ge-0.1.1/easy_ge/expectation_manager.py
--rw-r--r--   0        0        0     3997 2023-07-12 08:01:08.794839 easy_ge-0.1.1/easy_ge/helpers.py
--rw-r--r--   0        0        0     1821 2023-07-12 09:47:40.673614 easy_ge-0.1.1/easy_ge/main.py
--rw-r--r--   0        0        0      908 2023-07-11 19:54:36.830184 easy_ge-0.1.1/easy_ge/templates/checkpoint.tpl
--rw-r--r--   0        0        0     3287 2023-07-11 20:05:32.078164 easy_ge-0.1.1/easy_ge/templates/great_expectations.tpl
--rw-r--r--   0        0        0     4705 2023-07-11 19:59:36.076319 easy_ge-0.1.1/easy_ge/templates/schema.json
--rw-r--r--   0        0        0     1017 2023-07-12 10:08:10.613379 easy_ge-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4715 1970-01-01 00:00:00.000000 easy_ge-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-12 08:26:49.044542 easy_ge-0.1.2/LICENSE
+-rw-r--r--   0        0        0       86 2023-07-12 09:36:20.503745 easy_ge-0.1.2/easy_ge/__init__.py
+-rw-r--r--   0        0        0     5477 2023-07-12 09:41:47.853681 easy_ge-0.1.2/easy_ge/expectation_manager.py
+-rw-r--r--   0        0        0     3997 2023-07-12 08:01:08.794839 easy_ge-0.1.2/easy_ge/helpers.py
+-rw-r--r--   0        0        0     1821 2023-07-12 09:47:40.673614 easy_ge-0.1.2/easy_ge/main.py
+-rw-r--r--   0        0        0      908 2023-07-11 19:54:36.830184 easy_ge-0.1.2/easy_ge/templates/checkpoint.tpl
+-rw-r--r--   0        0        0     3287 2023-07-11 20:05:32.078164 easy_ge-0.1.2/easy_ge/templates/great_expectations.tpl
+-rw-r--r--   0        0        0     4705 2023-07-11 19:59:36.076319 easy_ge-0.1.2/easy_ge/templates/schema.json
+-rw-r--r--   0        0        0     1017 2023-07-12 10:14:49.073301 easy_ge-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 10:14:43.883302 easy_ge-0.1.2/readme.md
+-rw-r--r--   0        0        0      934 1970-01-01 00:00:00.000000 easy_ge-0.1.2/PKG-INFO
```

### Comparing `easy_ge-0.1.1/LICENSE` & `easy_ge-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.1/easy_ge/expectation_manager.py` & `easy_ge-0.1.2/easy_ge/expectation_manager.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.1/easy_ge/helpers.py` & `easy_ge-0.1.2/easy_ge/helpers.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.1/easy_ge/main.py` & `easy_ge-0.1.2/easy_ge/main.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.1/easy_ge/templates/checkpoint.tpl` & `easy_ge-0.1.2/easy_ge/templates/checkpoint.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.1/easy_ge/templates/great_expectations.tpl` & `easy_ge-0.1.2/easy_ge/templates/great_expectations.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.1/easy_ge/templates/schema.json` & `easy_ge-0.1.2/easy_ge/templates/schema.json`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.1/pyproject.toml` & `easy_ge-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "easy_ge"
-version = "0.1.1"
+version = "0.1.2"
 description = "A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases."
 authors = ["Elsayed91 <elsayed.is@outlook.com>"]
-readme = "README.md"
+readme = "readme.md"
 packages = [{include = "easy_ge"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 great-expectations = "^0.17.4"
 pyyaml = "^6.0"
 jsonschema = "^4.18.0"
```

