# Comparing `tmp/fh_fablib-1.0.20230705.tar.gz` & `tmp/fh_fablib-1.0.20230712.tar.gz`

## Comparing `fh_fablib-1.0.20230705.tar` & `fh_fablib-1.0.20230712.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.editorconfig
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20073 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/CHANGELOG.rst
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/bumpversion.sh
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0    26750 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/__init__.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/extract_js_gettext_strings.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/.editorconfig
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/.eslintrc.js
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/pyproject.toml
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/webpack.library.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.gitignore
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/LICENSE
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/README.rst
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/pyproject.toml
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/.editorconfig
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20205 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/CHANGELOG.rst
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/bumpversion.sh
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0    26750 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/fh_fablib/__init__.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/fh_fablib/extract_js_gettext_strings.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/fh_fablib/dotfiles/.editorconfig
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/fh_fablib/dotfiles/.eslintrc.js
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/fh_fablib/dotfiles/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/fh_fablib/dotfiles/pyproject.toml
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/fh_fablib/dotfiles/webpack.library.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/LICENSE
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/README.rst
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/pyproject.toml
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230712/PKG-INFO
```

### Comparing `fh_fablib-1.0.20230705/.pre-commit-config.yaml` & `fh_fablib-1.0.20230712/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     hooks:
       - id: absolufy-imports
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.277"
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.9-for-vscode
+    rev: v3.0.0
     hooks:
       - id: prettier
         args: [--list-different, --no-semi]
         exclude: "^conf/|.*\\.html$"
```

### Comparing `fh_fablib-1.0.20230705/CHANGELOG.rst` & `fh_fablib-1.0.20230712/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 ==========
 Change log
 ==========
 
 Next version
 ~~~~~~~~~~~~
 
+1.0.20230712
+~~~~~~~~~~~~
+
+- Updated the bundled pre-commit hooks, removed flake8-logging-format from the
+  default configuration.
+
 1.0.20230705
 ~~~~~~~~~~~~
 
 - Removed the unused ``config.app``.
 - Exposed all configuration values as ``FL_*`` environment values, for example
   ``FL_DOMAIN``.
```

### Comparing `fh_fablib-1.0.20230705/fh_fablib/__init__.py` & `fh_fablib-1.0.20230712/fh_fablib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fabric import Connection, task
 from invoke import Collection  # noqa, re-export
 from speckenv_django import django_database_url
 
 from fh_fablib.extract_js_gettext_strings import generate_strings
 
 
-__version__ = "1.0.20230705"
+__version__ = "1.0.20230712"
 
 
 # I don't care, in this context.
 warnings.simplefilter("ignore", category=ResourceWarning)
 
 
 def ansi(code):
```

### Comparing `fh_fablib-1.0.20230705/fh_fablib/extract_js_gettext_strings.py` & `fh_fablib-1.0.20230712/fh_fablib/extract_js_gettext_strings.py`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230705/fh_fablib/dotfiles/.pre-commit-config.yaml` & `fh_fablib-1.0.20230712/fh_fablib/dotfiles/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     hooks:
       - id: absolufy-imports
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.277"
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-eslint
     rev: v8.44.0
     hooks:
       - id: eslint
         args: [--fix]
@@ -60,15 +60,15 @@
           - "@babel/preset-env"
           - "@babel/preset-react"
           - "@babel/plugin-syntax-class-properties"
           - "@babel/plugin-syntax-decorators"
           - "@babel/plugin-syntax-jsx"
           - jest
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.9-for-vscode
+    rev: v3.0.0
     hooks:
       - id: prettier
         args: [--list-different, --no-semi]
         exclude: "^conf/|.*\\.html$|.*\\.json$"
   - repo: https://github.com/tox-dev/pyproject-fmt
     rev: 0.13.0
     hooks:
```

### Comparing `fh_fablib-1.0.20230705/fh_fablib/dotfiles/pyproject.toml` & `fh_fablib-1.0.20230712/fh_fablib/dotfiles/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -16,16 +16,14 @@
   "FBT",
   # flake8-bugbear
   "B",
   # flake8-comprehensions
   "C4",
   # flake8-django
   "DJ",
-  # flake8-logging-format
-  "G",
   # flake8-pie
   "PIE",
   # flake8-simplify
   "SIM",
   # flake8-gettext
   "INT",
   # pygrep-hooks
```

### Comparing `fh_fablib-1.0.20230705/fh_fablib/dotfiles/webpack.library.js` & `fh_fablib-1.0.20230712/fh_fablib/dotfiles/webpack.library.js`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230705/LICENSE` & `fh_fablib-1.0.20230712/LICENSE`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230705/README.rst` & `fh_fablib-1.0.20230712/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230705")
+       fl.require("1.0.20230712")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -90,15 +90,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230705")
+    fl.require("1.0.20230712")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20230705/pyproject.toml` & `fh_fablib-1.0.20230712/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -47,16 +47,14 @@
   "FBT",
   # flake8-bugbear
   "B",
   # flake8-comprehensions
   "C4",
   # flake8-django
   "DJ",
-  # flake8-logging-format
-  "G",
   # flake8-pie
   "PIE",
   # flake8-simplify
   "SIM",
   # flake8-gettext
   "INT",
   # pygrep-hooks
```

### Comparing `fh_fablib-1.0.20230705/PKG-INFO` & `fh_fablib-1.0.20230712/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fh-fablib
-Version: 1.0.20230705
+Version: 1.0.20230712
 Summary: fh-fablib
 Project-URL: Homepage, https://github.com/feinheit/fh-fablib/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9
@@ -28,15 +28,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230705")
+       fl.require("1.0.20230712")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -104,15 +104,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230705")
+    fl.require("1.0.20230712")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

