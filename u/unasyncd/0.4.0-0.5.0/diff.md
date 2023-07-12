# Comparing `tmp/unasyncd-0.4.0.tar.gz` & `tmp/unasyncd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unasyncd-0.4.0.tar", max compression
+gzip compressed data, was "unasyncd-0.5.0.tar", max compression
```

## Comparing `unasyncd-0.4.0.tar` & `unasyncd-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-06-17 13:02:38.736694 unasyncd-0.4.0/LICENSE
--rw-r--r--   0        0        0    17844 2023-06-17 13:02:38.736694 unasyncd-0.4.0/README.md
--rw-r--r--   0        0        0      995 2023-06-17 13:02:38.736694 unasyncd-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 13:02:38.736694 unasyncd-0.4.0/unasyncd/__init__.py
--rw-r--r--   0        0        0     4089 2023-06-17 13:02:38.736694 unasyncd-0.4.0/unasyncd/cli.py
--rw-r--r--   0        0        0     2553 2023-06-17 13:02:38.736694 unasyncd-0.4.0/unasyncd/config.py
--rw-r--r--   0        0        0    10349 2023-06-17 13:02:38.736694 unasyncd-0.4.0/unasyncd/main.py
--rw-r--r--   0        0        0    38061 2023-06-17 13:02:38.736694 unasyncd-0.4.0/unasyncd/transformers.py
--rw-r--r--   0        0        0    18713 1970-01-01 00:00:00.000000 unasyncd-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-12 13:56:51.676885 unasyncd-0.5.0/LICENSE
+-rw-r--r--   0        0        0    17844 2023-07-12 13:56:51.676885 unasyncd-0.5.0/README.md
+-rw-r--r--   0        0        0      995 2023-07-12 13:56:51.676885 unasyncd-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 13:56:51.676885 unasyncd-0.5.0/unasyncd/__init__.py
+-rw-r--r--   0        0        0     4115 2023-07-12 13:56:51.676885 unasyncd-0.5.0/unasyncd/cli.py
+-rw-r--r--   0        0        0     2553 2023-07-12 13:56:51.680885 unasyncd-0.5.0/unasyncd/config.py
+-rw-r--r--   0        0        0    10349 2023-07-12 13:56:51.680885 unasyncd-0.5.0/unasyncd/main.py
+-rw-r--r--   0        0        0    40332 2023-07-12 13:56:51.680885 unasyncd-0.5.0/unasyncd/transformers.py
+-rw-r--r--   0        0        0    18713 1970-01-01 00:00:00.000000 unasyncd-0.5.0/PKG-INFO
```

### Comparing `unasyncd-0.4.0/LICENSE` & `unasyncd-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unasyncd-0.4.0/README.md` & `unasyncd-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 
 ### As a pre-commit hook
 
 Unasyncd is available as a pre-commit hook:
 
 ```yaml
 - repo: https://github.com/provinzkraut/unasyncd
-  rev: v0.2.1
+  rev: v0.4.0
   hooks:
     - id: unasyncd
 ```
 
 ### Configuration
 
 Unasyncd can be configured via a `pyproject.toml` file, a dedicated `.unasyncd.toml`
```

### Comparing `unasyncd-0.4.0/pyproject.toml` & `unasyncd-0.5.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "unasyncd"
-version = "0.4.0"
+version = "0.5.0"
 description = "A tool to transform asynchronous Python code to synchronous Python code."
 authors = ["Janek Nouvertné <j.a.nouvertne@posteo.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 libcst = "^1.0.0"
 click = "^8.1.3"
 rich = "^13.4.1"
 anyio = "^3.7.0"
-msgspec = "^0.16.0"
+msgspec = "^0.17.0"
 tomli-w = "^1.0.0"
 rich-click = "^1.6.1"
 ruff = {version = "*", optional = true}
 
 [tool.poetry.extras]
 ruff = ["ruff"]
```

### Comparing `unasyncd-0.4.0/unasyncd/cli.py` & `unasyncd-0.5.0/unasyncd/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         f"[blue]{files_unchanged}[/] {'would be ' if check_only else ''}"
         "left unchanged"
     )
 
     return files_changed > 0
 
 
-@click.command()
+@click.command()  # type: ignore[arg-type]
 @click.option(
     "--cache/--no-cache",
     is_flag=True,
     help="Cache transformation results",
     default=None,
 )
 @click.option(
```

### Comparing `unasyncd-0.4.0/unasyncd/config.py` & `unasyncd-0.5.0/unasyncd/config.py`

 * *Files identical despite different names*

### Comparing `unasyncd-0.4.0/unasyncd/main.py` & `unasyncd-0.5.0/unasyncd/main.py`

 * *Files identical despite different names*

### Comparing `unasyncd-0.4.0/unasyncd/transformers.py` & `unasyncd-0.5.0/unasyncd/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import dataclasses
 import itertools
 import re
 import subprocess
 import sys
 from collections import defaultdict
 from collections.abc import Iterable, Sequence
-from typing import Any, Callable, TypeVar, Union
+from typing import Any, Callable, TypeVar, Union, cast
 
 import libcst as cst
 import libcst.matchers as m
 from libcst import MetadataWrapper
 from libcst.metadata import QualifiedName, ScopeProvider
 from libcst.native import parse_module
 
@@ -132,17 +132,18 @@
         return val
 
     return None
 
 
 def _get_full_name_for_import_from(node: cst.ImportFrom) -> str:
     return (
-        cst.helpers.get_full_name_for_node_or_raise(node.module)
+        "." * len(node.relative)
+        + cst.helpers.get_full_name_for_node_or_raise(node.module)
         if node.module
-        else "." * len(node.relative)
+        else ""
     )
 
 
 def _create_import_from(module_name: str, names: Iterable[str]) -> cst.ImportFrom:
     relative: list[cst.Dot] = []
     if "." in module_name:
         orig_len = len(module_name)
@@ -426,17 +427,17 @@
         }
 
         self._scoped_node_imports: defaultdict[cst.CSTNode, ImportMeta] = defaultdict(
             lambda: ImportMeta(module_imports={}, from_imports={})
         )
 
         self._expressions_to_remove: set[cst.Expr] = set()
-        self._string_transformer = StringTransformer()
+        self._string_transformer = StringTransformer(self._name_replacements)
 
-        self._current_scop_name: tuple[str, ...] = tuple()
+        self._current_scope_name: tuple[str, ...] = tuple()
         self._scope_nodes: list[cst.CSTNode] = []
 
         self._if_type_checking_node: cst.If | None = None
         self._if_type_checking_imports: set[AnyImport] = set()
         self._in_if_type_checking_block: bool = False
         self._in_import = False
 
@@ -472,15 +473,15 @@
         """The parent node of the current scope (excludes comprehension scope)"""
         if self._scope_nodes:
             return self._scope_nodes[-1]
         return None
 
     @property
     def _should_transform_current_node(self) -> bool:
-        return self._current_scop_name not in self.meta.exclude
+        return self._current_scope_name not in self.meta.exclude
 
     def get_qualified_name(self, node: cst.CSTNode) -> str | None:
         """Get the fully qualified name of ``node``, relative to the current module."""
         try:
             if not (scope := self.get_metadata(ScopeProvider, node)):
                 return None
 
@@ -501,31 +502,31 @@
         return None
 
     def visit_Module(self, node: cst.Module) -> bool:
         self._scope_nodes.append(node)
         return True
 
     def visit_ClassDef(self, node: cst.ClassDef) -> bool | None:
-        self._current_scop_name = (*self._current_scop_name, node.name.value)
+        self._current_scope_name = (*self._current_scope_name, node.name.value)
         self._scope_nodes.append(node)
         return self._should_transform_current_node
 
     def leave_ClassDef(
         self, original_node: cst.ClassDef, updated_node: cst.ClassDef
     ) -> (
         cst.BaseStatement | cst.FlattenSentinel[cst.BaseStatement] | cst.RemovalSentinel
     ):
-        self._current_scop_name = self._current_scop_name[:-1]
+        self._current_scope_name = self._current_scope_name[:-1]
         self._scope_nodes = self._scope_nodes[:-1]
         if self._should_transform_docstrings and self._should_transform_current_node:
             updated_node = self._transform_docstring(updated_node)
         return updated_node
 
     def visit_FunctionDef(self, node: cst.FunctionDef) -> bool | None:
-        self._current_scop_name = (*self._current_scop_name, node.name.value)
+        self._current_scope_name = (*self._current_scope_name, node.name.value)
         self._scope_nodes.append(node)
         return self._should_transform_current_node
 
     def leave_FunctionDef(
         self, original_node: cst.FunctionDef, updated_node: cst.FunctionDef
     ) -> (
         cst.BaseStatement | cst.FlattenSentinel[cst.BaseStatement] | cst.RemovalSentinel
@@ -533,15 +534,15 @@
         if self._should_transform_current_node:
             if updated_node.asynchronous:
                 updated_node = updated_node.with_changes(asynchronous=None)
 
             if self._should_transform_docstrings:
                 updated_node = self._transform_docstring(updated_node)
 
-        self._current_scop_name = self._current_scop_name[:-1]
+        self._current_scope_name = self._current_scope_name[:-1]
         self._scope_nodes = self._scope_nodes[:-1]
         return updated_node
 
     def _transform_docstring(self, updated_node: ScopedNodeT) -> ScopedNodeT:
         if not (docstring_node := _get_docstring_node(updated_node.body)):
             return updated_node
 
@@ -791,14 +792,76 @@
 
         none_element = cst.SubscriptElement(slice=cst.Index(cst.Name("None")))
         updated_node = updated_node.with_changes(
             slice=[*updated_node.slice, none_element]
         )
         return updated_node
 
+    def leave_Assign(
+        self, original_node: cst.Assign, updated_node: cst.Assign
+    ) -> (
+        cst.BaseSmallStatement
+        | cst.FlattenSentinel[cst.BaseSmallStatement]
+        | cst.RemovalSentinel
+    ):
+        """Handle ``__all__`` and its imports"""
+
+        if not isinstance(self.current_scope_node, cst.Module):
+            return updated_node
+
+        if not m.matches(
+            updated_node, m.Assign(targets=[m.AssignTarget(target=m.Name("__all__"))])
+        ):
+            return updated_node
+
+        imported_names: dict[str, str] = {}
+        for module_name, import_ in self._scoped_node_imports[
+            self.current_scope_node
+        ].from_imports.items():
+            if isinstance(import_.names, cst.ImportStar):
+                continue
+
+            for name in import_.names:
+                full_name = name.evaluated_alias or name.evaluated_name
+                imported_names[
+                    full_name
+                ] = f"{_get_full_name_for_import_from(import_)}.{full_name}"
+
+        elements: list[cst.Element] = updated_node.value.elements  # type: ignore[attr-defined]  # noqa: E501
+        updated_elements: list[cst.Element] = []
+        for element in elements:
+            if not isinstance(element.value, cst.SimpleString):
+                continue
+
+            value = cast(str, element.value.evaluated_value)
+            if not (qualified_name := imported_names.get(value)):
+                continue
+
+            if not (replacement := self._name_replacements.get(qualified_name)):
+                continue
+
+            if "." in replacement:
+                module_name, attr = replacement.rsplit(".", 1)
+                self.meta.needs_from_import[module_name].add(attr)
+                replacement = attr
+            else:
+                self.meta.needs_module_import.add(replacement.rsplit(".", 1)[0])
+
+            quote = element.value.quote
+
+            updated_elements.append(
+                element.with_deep_changes(
+                    element.value, value=f"{quote}{replacement}{quote}"
+                )
+            )
+
+        return updated_node.with_deep_changes(
+            updated_node.value, elements=updated_elements
+        )
+
     def _find_first_non_import_line(self, updated_node: cst.Module) -> int:
         """Get the index of the first line of the module that is not an import,
         skipping module level docstrings and comments.
         """
         import_matcher = m.SimpleStatementLine(
             body=[m.AtLeastN(m.OneOf(m.Import(), m.ImportFrom()), n=1)]
         )
```

### Comparing `unasyncd-0.4.0/PKG-INFO` & `unasyncd-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: unasyncd
-Version: 0.4.0
+Version: 0.5.0
 Summary: A tool to transform asynchronous Python code to synchronous Python code.
 License: MIT
 Author: Janek Nouvertné
 Author-email: j.a.nouvertne@posteo.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ruff
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: libcst (>=1.0.0,<2.0.0)
-Requires-Dist: msgspec (>=0.16.0,<0.17.0)
+Requires-Dist: msgspec (>=0.17.0,<0.18.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Requires-Dist: ruff ; extra == "ruff"
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Unasync
@@ -428,15 +428,15 @@
 
 ### As a pre-commit hook
 
 Unasyncd is available as a pre-commit hook:
 
 ```yaml
 - repo: https://github.com/provinzkraut/unasyncd
-  rev: v0.2.1
+  rev: v0.4.0
   hooks:
     - id: unasyncd
 ```
 
 ### Configuration
 
 Unasyncd can be configured via a `pyproject.toml` file, a dedicated `.unasyncd.toml`
```

