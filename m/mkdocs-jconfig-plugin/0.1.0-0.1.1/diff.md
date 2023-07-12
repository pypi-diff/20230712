# Comparing `tmp/mkdocs_jconfig_plugin-0.1.0.tar.gz` & `tmp/mkdocs_jconfig_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_jconfig_plugin-0.1.0.tar", max compression
+gzip compressed data, was "mkdocs_jconfig_plugin-0.1.1.tar", max compression
```

## Comparing `mkdocs_jconfig_plugin-0.1.0.tar` & `mkdocs_jconfig_plugin-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       24 2023-07-10 21:18:02.076045 mkdocs_jconfig_plugin-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-10 21:18:02.076045 mkdocs_jconfig_plugin-0.1.0/mkdocs_jconfig/__init__.py
--rw-r--r--   0        0        0     2707 2023-07-10 21:18:02.076045 mkdocs_jconfig_plugin-0.1.0/mkdocs_jconfig/plugin.py
--rw-r--r--   0        0        0     1104 2023-07-10 21:18:02.076045 mkdocs_jconfig_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 mkdocs_jconfig_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1181 2023-07-12 14:14:27.020051 mkdocs_jconfig_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 14:14:27.020051 mkdocs_jconfig_plugin-0.1.1/mkdocs_jconfig/__init__.py
+-rw-r--r--   0        0        0     2707 2023-07-12 14:14:27.020051 mkdocs_jconfig_plugin-0.1.1/mkdocs_jconfig/plugin.py
+-rw-r--r--   0        0        0     1174 2023-07-12 14:14:27.020051 mkdocs_jconfig_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 mkdocs_jconfig_plugin-0.1.1/PKG-INFO
```

### Comparing `mkdocs_jconfig_plugin-0.1.0/mkdocs_jconfig/plugin.py` & `mkdocs_jconfig_plugin-0.1.1/mkdocs_jconfig/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_jconfig_plugin-0.1.0/pyproject.toml` & `mkdocs_jconfig_plugin-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mkdocs-jconfig-plugin"
-version = "0.1.0"
-description = "An MkDocs plugin to ..."
+version = "0.1.1"
+description = "An MkDocs plugin to process configuration items with Jinja2"
 authors = ["Jacques Supcik <jacques.supcik@hefr.ch>"]
 repository = "https://github.com/supcik/mkdocs-jconfig-plugin"
 license = "Apache-2"
 readme = "README.md"
 packages = [{ include = "mkdocs_jconfig" }]
 keywords = ["mkdocs", "python", "markdown", "wiki"]
 classifiers = [
@@ -25,14 +25,15 @@
 test = ["mkdocs-material", "mkdocs-macros-plugin"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pylint = "^2.17.4"
 isort = "^5.12.0"
 pre-commit = "^3.3.3"
+mkdocs-calendar-plugin = "^0.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins]
```

