# Comparing `tmp/cmem_plugin_parameters-1.0.2.tar.gz` & `tmp/cmem_plugin_parameters-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_parameters-1.0.2.tar", max compression
+gzip compressed data, was "cmem_plugin_parameters-2.0.0.tar", max compression
```

## Comparing `cmem_plugin_parameters-1.0.2.tar` & `cmem_plugin_parameters-2.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11334 2023-04-28 10:30:21.343782 cmem_plugin_parameters-1.0.2/LICENSE
--rw-r--r--   0        0        0      364 2023-04-28 10:30:21.343782 cmem_plugin_parameters-1.0.2/README-public.md
--rw-r--r--   0        0        0     3301 2023-04-28 10:30:21.343782 cmem_plugin_parameters-1.0.2/cmem_plugin_parameters/__init__.py
--rw-r--r--   0        0        0     1653 2023-04-28 10:30:55.846243 cmem_plugin_parameters-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 cmem_plugin_parameters-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-07-12 11:25:21.952555 cmem_plugin_parameters-2.0.0/LICENSE
+-rw-r--r--   0        0        0      364 2023-07-12 11:25:21.952555 cmem_plugin_parameters-2.0.0/README-public.md
+-rw-r--r--   0        0        0     3301 2023-07-12 11:25:21.952555 cmem_plugin_parameters-2.0.0/cmem_plugin_parameters/__init__.py
+-rw-r--r--   0        0        0     1672 2023-07-12 11:25:51.709695 cmem_plugin_parameters-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 cmem_plugin_parameters-2.0.0/PKG-INFO
```

### Comparing `cmem_plugin_parameters-1.0.2/LICENSE` & `cmem_plugin_parameters-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_parameters-1.0.2/cmem_plugin_parameters/__init__.py` & `cmem_plugin_parameters-2.0.0/cmem_plugin_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_parameters-1.0.2/pyproject.toml` & `cmem_plugin_parameters-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-parameters"
-version = "1.0.2"
+version = "2.0.0"
 license = "Apache-2.0"
 description = "Set or overwrite parameters of a task."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
@@ -13,26 +13,27 @@
 keywords = [
     "eccenca Corporate Memory", "plugin", "yaml", "parameters"
 ]
 homepage = "https://github.com/eccenca/cmem-plugin-parameters"
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
-cmem-plugin-base = "^3.1.0"
+python = "^3.11"
+cmem-plugin-base = "^4.0.0"
 PyYAML = "^6.0"
 
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

### Comparing `cmem_plugin_parameters-1.0.2/PKG-INFO` & `cmem_plugin_parameters-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-parameters
-Version: 1.0.2
+Version: 2.0.0
 Summary: Set or overwrite parameters of a task.
 Home-page: https://github.com/eccenca/cmem-plugin-parameters
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,yaml,parameters
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: cmem-plugin-base (>=3.1.0,<4.0.0)
+Requires-Dist: cmem-plugin-base (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-parameters
 
 eccenca Corporate Memory Workflow plugin for parameter input
 
 This is a plugin for [eccenca](https://eccenca.com) [Corporate Memory](https://documentation.eccenca.com).
```

