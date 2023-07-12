# Comparing `tmp/cmem_plugin_kaggle-1.0.2.tar.gz` & `tmp/cmem_plugin_kaggle-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_kaggle-1.0.2.tar", max compression
+gzip compressed data, was "cmem_plugin_kaggle-2.0.0.tar", max compression
```

## Comparing `cmem_plugin_kaggle-1.0.2.tar` & `cmem_plugin_kaggle-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      401 2023-04-28 12:01:29.654392 cmem_plugin_kaggle-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0    11334 2023-04-28 12:01:29.654392 cmem_plugin_kaggle-1.0.2/LICENSE
--rw-r--r--   0        0        0      359 2023-04-28 12:01:29.654392 cmem_plugin_kaggle-1.0.2/README-public.md
--rw-r--r--   0        0        0        0 2023-04-28 12:01:29.654392 cmem_plugin_kaggle-1.0.2/cmem_plugin_kaggle/__init__.py
--rw-r--r--   0        0        0    12669 2023-04-28 12:01:29.654392 cmem_plugin_kaggle-1.0.2/cmem_plugin_kaggle/kaggle_import.py
--rw-r--r--   0        0        0     1771 2023-04-28 12:01:55.943128 cmem_plugin_kaggle-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 cmem_plugin_kaggle-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      532 2023-07-12 09:14:18.466703 cmem_plugin_kaggle-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11334 2023-07-12 09:14:18.466703 cmem_plugin_kaggle-2.0.0/LICENSE
+-rw-r--r--   0        0        0      359 2023-07-12 09:14:18.466703 cmem_plugin_kaggle-2.0.0/README-public.md
+-rw-r--r--   0        0        0        0 2023-07-12 09:14:18.466703 cmem_plugin_kaggle-2.0.0/cmem_plugin_kaggle/__init__.py
+-rw-r--r--   0        0        0    12669 2023-07-12 09:14:18.466703 cmem_plugin_kaggle-2.0.0/cmem_plugin_kaggle/kaggle_import.py
+-rw-r--r--   0        0        0     1790 2023-07-12 09:14:40.206860 cmem_plugin_kaggle-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 cmem_plugin_kaggle-2.0.0/PKG-INFO
```

### Comparing `cmem_plugin_kaggle-1.0.2/LICENSE` & `cmem_plugin_kaggle-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kaggle-1.0.2/cmem_plugin_kaggle/kaggle_import.py` & `cmem_plugin_kaggle-2.0.0/cmem_plugin_kaggle/kaggle_import.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kaggle-1.0.2/pyproject.toml` & `cmem_plugin_kaggle-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-kaggle"
-version = "1.0.2"
+version = "2.0.0"
 license = "Apache-2.0"
 description = "Import dataset resources from Kaggle."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -16,26 +16,27 @@
     "eccenca Corporate Memory", "plugin", "kaggle", "dataset"
 ]
 homepage = "https://github.com/eccenca/cmem-plugin-kaggle"
 include = ["CHANGELOG.md"]
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
-cmem-plugin-base = "^3.1.0"
+python = "^3.11"
+cmem-plugin-base = "^4.0.0"
 kaggle = "^1.5.13"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.3"
 defusedxml = "^0.7.1"
 flake8-formatter-junit-xml = "^0.0.6"
 genbadge = "^1.1.0"
 mypy = "^1.2.0"
+pillow = "^9.5.0"
 pylint-junit = "^0.3.2"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-memray = "^1.4.0"
 safety = "^1.10.3"
 typed-ast = "^1.5.4"
 wheel = "^0.38.4"
```

### Comparing `cmem_plugin_kaggle-1.0.2/PKG-INFO` & `cmem_plugin_kaggle-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-kaggle
-Version: 1.0.2
+Version: 2.0.0
 Summary: Import dataset resources from Kaggle.
 Home-page: https://github.com/eccenca/cmem-plugin-kaggle
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,kaggle,dataset
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cmem-plugin-base (>=3.1.0,<4.0.0)
+Requires-Dist: cmem-plugin-base (>=4.0.0,<5.0.0)
 Requires-Dist: kaggle (>=1.5.13,<2.0.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-kaggle
 
 Import dataset resources from [Kaggle](https://www.kaggle.com/).
```

