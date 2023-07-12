# Comparing `tmp/chlorophyll-0.3.1.tar.gz` & `tmp/chlorophyll-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chlorophyll-0.3.1.tar", last modified: Fri Apr 21 14:00:48 2023, max compression
+gzip compressed data, was "chlorophyll-0.4.0.tar", last modified: Wed Jul 12 14:24:22 2023, max compression
```

## Comparing `chlorophyll-0.3.1.tar` & `chlorophyll-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:48.670071 chlorophyll-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-21 14:00:48.666072 chlorophyll-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:48.666072 chlorophyll-0.3.1/chlorophyll/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/codeview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:48.666072 chlorophyll-0.3.1/chlorophyll/colorschemes/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/ayu-dark.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/ayu-light.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/dracula.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/mariana.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/colorschemes/monokai.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/chlorophyll/schemeparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:48.666072 chlorophyll-0.3.1/chlorophyll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 14:00:48.000000 chlorophyll-0.3.1/chlorophyll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:00:48.670071 chlorophyll-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-21 14:00:38.000000 chlorophyll-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:22.995867 chlorophyll-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-12 14:24:22.991866 chlorophyll-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:22.991866 chlorophyll-0.4.0/chlorophyll/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/codeview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:22.991866 chlorophyll-0.4.0/chlorophyll/colorschemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/ayu-dark.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/ayu-light.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/dracula.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/mariana.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/monokai.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/schemeparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:22.991866 chlorophyll-0.4.0/chlorophyll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:24:22.995867 chlorophyll-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/setup.py
```

### Comparing `chlorophyll-0.3.1/LICENSE` & `chlorophyll-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.1/PKG-INFO` & `chlorophyll-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.3.1
+Version: 0.4.0
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
 Home-page: https://gitlab.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Chlorophyll</h1>
```

### Comparing `chlorophyll-0.3.1/README.md` & `chlorophyll-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.1/chlorophyll/codeview.py` & `chlorophyll-0.4.0/chlorophyll/codeview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 from __future__ import annotations
 
+import inspect
 from contextlib import suppress
 from pathlib import Path
 from tkinter import BaseWidget, Event, Misc, TclError, Text, ttk
 from tkinter.font import Font
-from typing import Any
+from typing import Any, Callable, Type, Union
 
-from pygments import lex
+import pygments
 import pygments.lexers
+import toml
 from pyperclip import copy
 from tklinenums import TkLineNumbers
-from toml import load
 
 from .schemeparser import _parse_scheme
 
 color_schemes_dir = Path(__file__).parent / "colorschemes"
 
+LexerType = Union[Type[pygments.lexer.Lexer], pygments.lexer.Lexer]
+
 
 class CodeView(Text):
     _w: str
     _builtin_color_schemes = {"ayu-dark", "ayu-light", "dracula", "mariana", "monokai"}
 
     def __init__(
         self,
         master: Misc | None = None,
-        lexer: pygments.lexers.Lexer = pygments.lexers.TextLexer,
+        lexer: LexerType = pygments.lexers.TextLexer,
         color_scheme: dict[str, dict[str, str | int]] | str | None = None,
         tab_width: int = 4,
+        linenums_theme: Callable[[], tuple[str, str]] | tuple[str, str] | None = None,
         **kwargs,
     ) -> None:
         self._frame = ttk.Frame(master)
         self._frame.grid_rowconfigure(0, weight=1)
         self._frame.grid_columnconfigure(1, weight=1)
 
         kwargs.setdefault("wrap", "none")
         kwargs.setdefault("font", ("monospace", 11))
 
         super().__init__(self._frame, **kwargs)
         super().grid(row=0, column=1, sticky="nswe")
 
-        self._line_numbers = TkLineNumbers(self._frame, self, justify=kwargs.get("justify", "left"))
+        self._line_numbers = TkLineNumbers(
+            self._frame, self, justify=kwargs.get("justify", "left"), colors=linenums_theme
+        )
         self._vs = ttk.Scrollbar(self._frame, orient="vertical", command=self.yview)
         self._hs = ttk.Scrollbar(self._frame, orient="horizontal", command=self.xview)
 
         self._line_numbers.grid(row=0, column=0, sticky="ns")
         self._vs.grid(row=0, column=2, sticky="ns")
         self._hs.grid(row=1, column=1, sticky="we")
 
@@ -56,14 +62,15 @@
         contmand = "Command" if self._windowingsystem == "aqua" else "Control"
 
         super().bind(f"<{contmand}-c>", self._copy, add=True)
         super().bind(f"<{contmand}-v>", self._paste, add=True)
         super().bind(f"<{contmand}-a>", self._select_all, add=True)
         super().bind(f"<{contmand}-Shift-Z>", self.redo, add=True)
         super().bind("<<ContentChanged>>", self.scroll_line_update, add=True)
+        super().bind("<Button-1>", self._line_numbers.redraw, add=True)
 
         self._orig = f"{self._w}_widget"
         self.tk.call("rename", self._w, self._orig)
         self.tk.createcommand(self._w, self._cmd_proxy)
 
         self._set_lexer(lexer)
         self._set_color_scheme(color_scheme)
@@ -142,15 +149,15 @@
         for tag in self.tag_names(index=None):
             if tag.startswith("Token"):
                 self.tag_remove(tag, f"{line_num}.0", f"{line_num}.end")
 
         line_text = self.get(f"{line_num}.0", f"{line_num}.end")
         start_col = 0
 
-        for token, text in lex(line_text, self._lexer()):
+        for token, text in pygments.lex(line_text, self._lexer):
             token = str(token)
             end_col = start_col + len(text)
             if token not in {"Token.Text.Whitespace", "Token.Text"}:
                 self.tag_add(token, f"{line_num}.{start_col}", f"{line_num}.{end_col}")
             start_col = end_col
 
     def highlight_all(self) -> None:
@@ -158,53 +165,52 @@
             if tag.startswith("Token"):
                 self.tag_remove(tag, "1.0", "end")
 
         lines = self.get("1.0", "end")
         line_offset = lines.count("\n") - lines.lstrip().count("\n")
         start_index = str(self.tk.call(self._orig, "index", f"1.0 + {line_offset} lines"))
 
-        for token, text in lex(lines, self._lexer()):
+        for token, text in pygments.lex(lines, self._lexer):
             token = str(token)
             end_index = self.index(f"{start_index} + {len(text)} chars")
             if token not in {"Token.Text.Whitespace", "Token.Text"}:
                 self.tag_add(token, start_index, end_index)
             start_index = end_index
 
     def highlight_area(self, start_line: int | None = None, end_line: int | None = None) -> None:
         for tag in self.tag_names(index=None):
             if tag.startswith("Token"):
                 self.tag_remove(tag, f"{start_line}.0", f"{end_line}.end")
 
         text = self.get(f"{start_line}.0", f"{end_line}.end")
         line_offset = text.count("\n") - text.lstrip().count("\n")
         start_index = str(self.tk.call(self._orig, "index", f"{start_line}.0 + {line_offset} lines"))
-        for token, text in lex(text, self._lexer()):
+        for token, text in pygments.lex(text, self._lexer):
             token = str(token)
             end_index = self.index(f"{start_index} + {len(text)} indices")
             if token not in {"Token.Text.Whitespace", "Token.Text"}:
                 self.tag_add(token, start_index, end_index)
             start_index = end_index
 
     def _set_color_scheme(self, color_scheme: dict[str, dict[str, str | int]] | str | None) -> None:
         if isinstance(color_scheme, str) and color_scheme in self._builtin_color_schemes:
-            color_scheme = load(color_schemes_dir / f"{color_scheme}.toml")
+            color_scheme = toml.load(color_schemes_dir / f"{color_scheme}.toml")
         elif color_scheme is None:
-            color_scheme = load(color_schemes_dir / "dracula.toml")
+            color_scheme = toml.load(color_schemes_dir / "dracula.toml")
 
         assert isinstance(color_scheme, dict), "Must be a dictionary or a built-in color scheme"
 
         config, tags = _parse_scheme(color_scheme)
         self.configure(**config)
         self._setup_tags(tags)
 
         self.highlight_all()
 
-    def _set_lexer(self, lexer: pygments.lexers.Lexer) -> None:
-        self._lexer = lexer
-
+    def _set_lexer(self, lexer: LexerType) -> None:
+        self._lexer = lexer() if inspect.isclass(lexer) else lexer
         self.highlight_all()
 
     def __setitem__(self, key: str, value) -> None:
         self.configure(**{key: value})
 
     def __getitem__(self, key: str) -> Any:
         return self.cget(key)
```

### Comparing `chlorophyll-0.3.1/chlorophyll/colorschemes/ayu-dark.toml` & `chlorophyll-0.4.0/chlorophyll/colorschemes/ayu-dark.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.1/chlorophyll/colorschemes/ayu-light.toml` & `chlorophyll-0.4.0/chlorophyll/colorschemes/ayu-light.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.1/chlorophyll/colorschemes/dracula.toml` & `chlorophyll-0.4.0/chlorophyll/colorschemes/dracula.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.1/chlorophyll/colorschemes/mariana.toml` & `chlorophyll-0.4.0/chlorophyll/colorschemes/mariana.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.1/chlorophyll/colorschemes/monokai.toml` & `chlorophyll-0.4.0/chlorophyll/colorschemes/monokai.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.3.1/chlorophyll/schemeparser.py` & `chlorophyll-0.4.0/chlorophyll/schemeparser.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,19 @@
     "inactiveselectbackground": "inactive_select_bg",
     "insertbackground": "caret",
     "insertwidth": "caret_width",
     "borderwidth": "border_width",
     "highlightthickness": "focus_border_width",
 }
 
+_extras = {
+    "Error": "error",
+    "Literal.Date": "date",
+}
+
 _keywords = {
     "Keyword.Constant": "constant",
     "Keyword.Declaration": "declaration",
     "Keyword.Namespace": "namespace",
     "Keyword.Pseudo": "pseudo",
     "Keyword.Reserved": "reserved",
     "Keyword.Type": "type",
@@ -40,14 +45,15 @@
     "Name.Variable.Global": "global_variable",
     "Name.Variable.Instance": "instance_variable",
     "Name.Variable.Magic": "magic_variable",
 }
 
 _strings = {
     "Literal.String.Affix": "affix",
+    "Literal.String.Backtick": "backtick",
     "Literal.String.Char": "char",
     "Literal.String.Delimeter": "delimeter",
     "Literal.String.Doc": "doc",
     "Literal.String.Double": "double",
     "Literal.String.Escape": "escape",
     "Literal.String.Heredoc": "heredoc",
     "Literal.String.Interpol": "interpol",
@@ -70,14 +76,22 @@
     "Comment.Multiline": "multiline",
     "Comment.Preproc": "preproc",
     "Comment.PreprocFile": "preprocfile",
     "Comment.Single": "single",
     "Comment.Special": "special",
 }
 
+_generic = {
+    "Generic.Emph": "emphasis",
+    "Generic.Error": "error",
+    "Generic.Heading": "heading",
+    "Generic.Strong": "strong",
+    "Generic.Subheading": "subheading",
+}
+
 
 def _parse_table(
     source: dict[str, str | int] | None,
     map_: dict[str, str],
     fallback: str | int | None = None,
 ) -> dict[str, str | int | None]:
     result: dict[str, str | int | None] = {}
@@ -132,9 +146,11 @@
             color_scheme.get("operator"),
             {"Operator": "symbol", "Operator.Word": "word"},
         )
     )
     tags.update(**_parse_table(color_scheme.get("string"), _strings, general_string))
     tags.update(**_parse_table(color_scheme.get("number"), _numbers))
     tags.update(**_parse_table(color_scheme.get("comment"), _comments, general_comment))
+    tags.update(**_parse_table(color_scheme.get("generic"), _generic))
+    tags.update(**_parse_table(color_scheme.get("extras"), _extras))
 
     return editor, tags
```

### Comparing `chlorophyll-0.3.1/chlorophyll.egg-info/PKG-INFO` & `chlorophyll-0.4.0/chlorophyll.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.3.1
+Version: 0.4.0
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
 Home-page: https://gitlab.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Chlorophyll</h1>
```

### Comparing `chlorophyll-0.3.1/setup.py` & `chlorophyll-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 
 setup(
     name="chlorophyll",
-    version="0.3.1",
+    version="0.4.0",
     description="A module that fills your code with color - syntax highlighted text box widget for Tkinter.",
     author="rdbende",
     author_email="rdbende@gmail.com",
     url="https://gitlab.com/rdbende/chlorophyll",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["pygments", "toml", "tklinenums", "pyperclip"],
@@ -22,12 +22,13 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
     packages=["chlorophyll"],
     package_data={"chlorophyll": ["colorschemes/*"]},
 )
```

