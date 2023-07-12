# Comparing `tmp/mtng-0.7.0.tar.gz` & `tmp/mtng-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtng-0.7.0.tar", max compression
+gzip compressed data, was "mtng-0.7.1.tar", max compression
```

## Comparing `mtng-0.7.0.tar` & `mtng-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4820 2022-08-17 22:41:45.505290 mtng-0.7.0/README.md
--rw-r--r--   0        0        0      820 2023-07-12 09:42:26.506951 mtng-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       83 2022-08-11 10:46:06.387500 mtng-0.7.0/src/mtng/__init__.py
--rw-r--r--   0        0        0     6969 2023-07-12 09:28:26.387984 mtng-0.7.0/src/mtng/cli.py
--rw-r--r--   0        0        0     8250 2023-07-12 09:34:45.825269 mtng-0.7.0/src/mtng/collect.py
--rw-r--r--   0        0        0     1142 2023-07-12 09:04:23.800414 mtng-0.7.0/src/mtng/generate.py
--rw-r--r--   0        0        0     2244 2023-03-28 15:15:27.386088 mtng-0.7.0/src/mtng/spec.py
--rw-r--r--   0        0        0      437 2022-09-02 13:42:43.975478 mtng-0.7.0/src/mtng/template/base.tex
--rw-r--r--   0        0        0      119 2023-04-17 15:46:15.937707 mtng-0.7.0/src/mtng/template/item.tex
--rw-r--r--   0        0        0      261 2022-08-17 22:45:29.877915 mtng-0.7.0/src/mtng/template/item_context.tex
--rw-r--r--   0        0        0     2532 2023-04-17 15:59:47.711725 mtng-0.7.0/src/mtng/template/macros.tex
--rw-r--r--   0        0        0      725 2022-08-17 22:45:29.878621 mtng-0.7.0/src/mtng/template/main.tex
--rw-r--r--   0        0        0     3299 2022-09-02 13:55:37.778106 mtng-0.7.0/src/mtng/template/preamble.tex
--rw-r--r--   0        0        0      386 2022-09-02 13:54:57.808639 mtng-0.7.0/src/mtng/template/provides.tex
--rw-r--r--   0        0        0     3423 2023-07-12 09:04:23.800655 mtng-0.7.0/src/mtng/template/repo.tex
--rw-r--r--   0        0        0     5852 1970-01-01 00:00:00.000000 mtng-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4820 2022-08-17 22:41:45.505290 mtng-0.7.1/README.md
+-rw-r--r--   0        0        0      820 2023-07-12 09:44:20.462283 mtng-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       83 2022-08-11 10:46:06.387500 mtng-0.7.1/src/mtng/__init__.py
+-rw-r--r--   0        0        0     6969 2023-07-12 09:28:26.387984 mtng-0.7.1/src/mtng/cli.py
+-rw-r--r--   0        0        0     8250 2023-07-12 09:34:45.825269 mtng-0.7.1/src/mtng/collect.py
+-rw-r--r--   0        0        0     1142 2023-07-12 09:04:23.800414 mtng-0.7.1/src/mtng/generate.py
+-rw-r--r--   0        0        0     2244 2023-03-28 15:15:27.386088 mtng-0.7.1/src/mtng/spec.py
+-rw-r--r--   0        0        0      437 2022-09-02 13:42:43.975478 mtng-0.7.1/src/mtng/template/base.tex
+-rw-r--r--   0        0        0      119 2023-04-17 15:46:15.937707 mtng-0.7.1/src/mtng/template/item.tex
+-rw-r--r--   0        0        0      261 2022-08-17 22:45:29.877915 mtng-0.7.1/src/mtng/template/item_context.tex
+-rw-r--r--   0        0        0     2532 2023-04-17 15:59:47.711725 mtng-0.7.1/src/mtng/template/macros.tex
+-rw-r--r--   0        0        0      725 2022-08-17 22:45:29.878621 mtng-0.7.1/src/mtng/template/main.tex
+-rw-r--r--   0        0        0     3299 2022-09-02 13:55:37.778106 mtng-0.7.1/src/mtng/template/preamble.tex
+-rw-r--r--   0        0        0      386 2022-09-02 13:54:57.808639 mtng-0.7.1/src/mtng/template/provides.tex
+-rw-r--r--   0        0        0     3423 2023-07-12 09:04:23.800655 mtng-0.7.1/src/mtng/template/repo.tex
+-rw-r--r--   0        0        0     5852 1970-01-01 00:00:00.000000 mtng-0.7.1/PKG-INFO
```

### Comparing `mtng-0.7.0/README.md` & `mtng-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mtng-0.7.0/pyproject.toml` & `mtng-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mtng"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 packages = [
 { include = "mtng", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `mtng-0.7.0/src/mtng/cli.py` & `mtng-0.7.1/src/mtng/cli.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.0/src/mtng/collect.py` & `mtng-0.7.1/src/mtng/collect.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.0/src/mtng/generate.py` & `mtng-0.7.1/src/mtng/generate.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.0/src/mtng/spec.py` & `mtng-0.7.1/src/mtng/spec.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.0/src/mtng/template/macros.tex` & `mtng-0.7.1/src/mtng/template/macros.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.0/src/mtng/template/main.tex` & `mtng-0.7.1/src/mtng/template/main.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.0/src/mtng/template/preamble.tex` & `mtng-0.7.1/src/mtng/template/preamble.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.0/src/mtng/template/repo.tex` & `mtng-0.7.1/src/mtng/template/repo.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.0/PKG-INFO` & `mtng-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtng
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

