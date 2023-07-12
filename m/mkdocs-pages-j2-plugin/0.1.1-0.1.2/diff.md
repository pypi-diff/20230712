# Comparing `tmp/mkdocs_pages_j2_plugin-0.1.1.tar.gz` & `tmp/mkdocs_pages_j2_plugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_pages_j2_plugin-0.1.1.tar", max compression
+gzip compressed data, was "mkdocs_pages_j2_plugin-0.1.2.tar", max compression
```

## Comparing `mkdocs_pages_j2_plugin-0.1.1.tar` & `mkdocs_pages_j2_plugin-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      257 2023-07-10 19:17:22.635501 mkdocs_pages_j2_plugin-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-10 19:17:22.635501 mkdocs_pages_j2_plugin-0.1.1/pagesj2/__init__.py
--rw-r--r--   0        0        0     2376 2023-07-10 19:17:22.635501 mkdocs_pages_j2_plugin-0.1.1/pagesj2/plugin.py
--rw-r--r--   0        0        0     1252 2023-07-10 19:17:22.635501 mkdocs_pages_j2_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 mkdocs_pages_j2_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      867 2023-07-12 13:45:49.713079 mkdocs_pages_j2_plugin-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:49.713079 mkdocs_pages_j2_plugin-0.1.2/pagesj2/__init__.py
+-rw-r--r--   0        0        0     2376 2023-07-12 13:45:49.713079 mkdocs_pages_j2_plugin-0.1.2/pagesj2/plugin.py
+-rw-r--r--   0        0        0     1256 2023-07-12 13:45:49.713079 mkdocs_pages_j2_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 mkdocs_pages_j2_plugin-0.1.2/PKG-INFO
```

### Comparing `mkdocs_pages_j2_plugin-0.1.1/pagesj2/plugin.py` & `mkdocs_pages_j2_plugin-0.1.2/pagesj2/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_pages_j2_plugin-0.1.1/pyproject.toml` & `mkdocs_pages_j2_plugin-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mkdocs-pages-j2-plugin"
-version = "0.1.1"
-description = "An MkDocs plugin to generate .pages from pages.j2"
+version = "0.1.2"
+description = "An MkDocs plugin to generate '.pages' from 'pages.j2'"
 authors = ["Jacques Supcik <jacques.supcik@hefr.ch>"]
 repository = "https://github.com/supcik/mkdocs-pages-j2-plugin"
 license = "Apache-2"
 readme = "README.md"
 packages = [{ include = "pagesj2" }]
 keywords = ["mkdocs", "python", "markdown", "wiki"]
 classifiers = [
```

### Comparing `mkdocs_pages_j2_plugin-0.1.1/PKG-INFO` & `mkdocs_pages_j2_plugin-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mkdocs-pages-j2-plugin
-Version: 0.1.1
-Summary: An MkDocs plugin to generate .pages from pages.j2
+Version: 0.1.2
+Summary: An MkDocs plugin to generate '.pages' from 'pages.j2'
 Home-page: https://github.com/supcik/mkdocs-pages-j2-plugin
 License: Apache-2
 Keywords: mkdocs,python,markdown,wiki
 Author: Jacques Supcik
 Author-email: jacques.supcik@hefr.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,20 +20,53 @@
 Requires-Dist: mkdocs (>=1.4.3,<2.0.0)
 Requires-Dist: mkdocs-awesome-pages-plugin (>=2.9.1,<3.0.0) ; extra == "test"
 Requires-Dist: mkdocs-macros-plugin (>=1.0.1,<2.0.0) ; extra == "test"
 Requires-Dist: mkdocs-material (>=9.1.15,<10.0.0) ; extra == "test"
 Project-URL: Repository, https://github.com/supcik/mkdocs-pages-j2-plugin
 Description-Content-Type: text/markdown
 
-# mkdocs-pages-j2-today
+# mkdocs-pages-j2-plugin
 
 This plugin builds `.pages` files from `.pages.j2` files, using Jinja2 to render the templates.
+This plugin is particularly useful when used together with the
+[mkdocs-awesome-pages-plugin](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin).
 
-```text
+## Installation
+
+Install the package with pip:
+
+```bash
+pip install mkdocs-pages-j2-plugin
+```
+
+Activate the plugin in `mkdocs.yml`:
+
+```yaml
+plugins:
+  - search
+  - pages-j2
+  - awesome-pages
+```
+
+## Usage
+
+Example of a `.pages.j2` file:
+
+```jinja2
 title: Page Title
 nav:
     - Welcome: index.md
 {%- for i in range(1,3) %}
     - My Page {{ i }}: p{{ i }}.md
 {%- endfor %}
 ```
 
+The plugin will render the _Jinja2_ template above and create a `.pages` file with the following content:
+
+```text
+title: Page Title
+nav:
+    - Welcome: index.md
+    - My Page 1: p1.md
+    - My Page 2: p2.md
+```
+
```

