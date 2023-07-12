# Comparing `tmp/modelicalang-0.1.0a0.tar.gz` & `tmp/modelicalang-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelicalang-0.1.0a0.tar", max compression
+gzip compressed data, was "modelicalang-0.1.0a1.tar", max compression
```

## Comparing `modelicalang-0.1.0a0.tar` & `modelicalang-0.1.0a1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-01-31 05:12:56.433055 modelicalang-0.1.0a0/LICENSE
--rw-r--r--   0        0        0      139 2023-02-01 07:58:45.993579 modelicalang-0.1.0a0/README.md
--rw-r--r--   0        0        0     1337 2023-02-01 07:58:45.993579 modelicalang-0.1.0a0/modelicalang/__init__.py
--rw-r--r--   0        0        0     2272 2023-02-01 07:58:45.993579 modelicalang-0.1.0a0/modelicalang/_backend.py
--rw-r--r--   0        0        0        0 2023-02-01 07:58:45.993579 modelicalang-0.1.0a0/modelicalang/py.typed
--rw-r--r--   0        0        0    56944 2023-02-01 07:58:45.993579 modelicalang-0.1.0a0/modelicalang/v3_4.py
--rw-r--r--   0        0        0    58157 2023-02-01 07:58:45.993579 modelicalang-0.1.0a0/modelicalang/v3_5.py
--rw-r--r--   0        0        0     1774 2023-02-01 07:58:45.993579 modelicalang-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 modelicalang-0.1.0a0/setup.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 modelicalang-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-01-31 05:12:56.433055 modelicalang-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0      139 2023-02-02 08:31:28.517139 modelicalang-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1483 2023-07-12 07:19:30.267264 modelicalang-0.1.0a1/modelicalang/__init__.py
+-rw-r--r--   0        0        0     3545 2023-07-12 07:19:30.267264 modelicalang-0.1.0a1/modelicalang/_backend.py
+-rw-r--r--   0        0        0       52 2023-07-12 07:19:30.267264 modelicalang-0.1.0a1/modelicalang/exceptions.py
+-rw-r--r--   0        0        0        0 2023-02-01 07:58:45.993579 modelicalang-0.1.0a1/modelicalang/py.typed
+-rw-r--r--   0        0        0    56944 2023-02-01 07:58:45.993579 modelicalang-0.1.0a1/modelicalang/v3_4.py
+-rw-r--r--   0        0        0    58157 2023-02-01 07:58:45.993579 modelicalang-0.1.0a1/modelicalang/v3_5.py
+-rw-r--r--   0        0        0     1784 2023-07-12 07:19:30.267264 modelicalang-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 modelicalang-0.1.0a1/PKG-INFO
```

### Comparing `modelicalang-0.1.0a0/LICENSE` & `modelicalang-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `modelicalang-0.1.0a0/modelicalang/__init__.py` & `modelicalang-0.1.0a1/modelicalang/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+from __future__ import annotations
+
 __all__ = (
     "ModelicaVersion",
     "get_syntax_type",
     "ParsingExpressionLike",
     "returns_parsing_expression",
+    "ModelicaLangInternalWarning",
     "v3_4",
     "v3_5",
     "latest",
 )
 
 import enum
 from functools import lru_cache
 from typing import TYPE_CHECKING, Dict, Optional, Type, Union
 
-from typing_extensions import TypeAlias
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
+
+from .exceptions import ModelicaLangInternalWarning
 
 if TYPE_CHECKING:
     from arpeggio import _ParsingExpressionLike  # noqa: F401
 
 from . import v3_4, v3_5
 from ._backend import returns_parsing_expression
```

### Comparing `modelicalang-0.1.0a0/modelicalang/v3_4.py` & `modelicalang-0.1.0a1/modelicalang/v3_4.py`

 * *Files identical despite different names*

### Comparing `modelicalang-0.1.0a0/modelicalang/v3_5.py` & `modelicalang-0.1.0a1/modelicalang/v3_5.py`

 * *Files identical despite different names*

### Comparing `modelicalang-0.1.0a0/pyproject.toml` & `modelicalang-0.1.0a1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ModelicaLang"
-version = "0.1.0a0"
+version = "0.1.0a1"
 description = "Modelica parser and class representation for Python"
 repository = "https://github.com/ijknabla/ModelicaLanguageForPython"
 documentation = "https://ijknabla.github.io/ModelicaLanguageForPython/"
 authors = ["ijknabla <ijknabla@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
@@ -14,35 +14,36 @@
 packages = [
     { include = "modelicalang"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Arpeggio = ">=0.8"
-typing-extensions = ">=3.10"
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^22", python = ">=3.6.2"}
 isort = "^5.8"
 astunparse = {version = "^1.6.3", python = "<3.9"}
 
 [tool.poetry.group.document.dependencies]
 sphinx = "^5"
 sphinx-autobuild = "^2021.3.14"
 sphinx-rtd-theme = "^1.1.1"
 pygments-modelicapeg-plugin = {git = "https://github.com/ijknabla/pygments-modelicapeg-plugin.git", rev = "main"}
 
-[tool.poetry.group.test.dependencies]
+[tool.poetry.group.lint.dependencies]
 mypy = "^0.971"
 pyproject-flake8 = "^0.0.1-alpha.2"
-pytest = "^6.2.5"
-pytest-cov = "^4.0.0"
 types-setuptools = "^57.4.11"
 types-arpeggio = {git = "https://github.com/ijknabla/types-arpeggio.git", rev = "main"}
 
+[tool.poetry.group.test.dependencies]
+pytest = "^6.2.5"
+pytest-cov = "^4.0.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
```

### Comparing `modelicalang-0.1.0a0/PKG-INFO` & `modelicalang-0.1.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelicalang
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Modelica parser and class representation for Python
 Home-page: https://github.com/ijknabla/ModelicaLanguageForPython
 License: MIT
 Author: ijknabla
 Author-email: ijknabla@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: Arpeggio (>=0.8)
-Requires-Dist: typing-extensions (>=3.10)
 Project-URL: Documentation, https://ijknabla.github.io/ModelicaLanguageForPython/
 Project-URL: Repository, https://github.com/ijknabla/ModelicaLanguageForPython
 Description-Content-Type: text/markdown
 
 # ModelicaLang
 
 Modelica parser and class representation for Python
```

