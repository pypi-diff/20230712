# Comparing `tmp/macro_kit-0.4.5.tar.gz` & `tmp/macro_kit-0.4.6.tar.gz`

## Comparing `macro_kit-0.4.5.tar` & `macro_kit-0.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/__init__.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/_symbol.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/_validator.py
--rw-r--r--   0        0        0    17842 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/ast.py
--rw-r--r--   0        0        0    33045 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/expression.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/head.py
--rw-r--r--   0        0        0    33105 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/macro.py
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/mock.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/py.typed
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/type_map.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/utils.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/ipython/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/ipython/magic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/julia/__init__.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/julia/translate.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 macro_kit-0.4.5/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 macro_kit-0.4.5/LICENSE
--rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 macro_kit-0.4.5/README.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 macro_kit-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 macro_kit-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/__init__.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/_symbol.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/_validator.py
+-rw-r--r--   0        0        0    17973 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/ast.py
+-rw-r--r--   0        0        0    33045 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/expression.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/head.py
+-rw-r--r--   0        0        0    33105 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/macro.py
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/mock.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/py.typed
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/type_map.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/utils.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/ipython/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/ipython/magic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/julia/__init__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 macro_kit-0.4.6/macrokit/julia/translate.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 macro_kit-0.4.6/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 macro_kit-0.4.6/LICENSE
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 macro_kit-0.4.6/README.md
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 macro_kit-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 macro_kit-0.4.6/PKG-INFO
```

### Comparing `macro_kit-0.4.5/macrokit/__init__.py` & `macro_kit-0.4.6/macrokit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """macro-kit is a package for macro recording and metaprogramming in Python."""
 
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 __author__ = "Hanjin Liu"
 __email__ = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp"
 
 from macrokit._symbol import Symbol
 from macrokit.expression import (
     Expr,
     Head,
```

### Comparing `macro_kit-0.4.5/macrokit/_symbol.py` & `macro_kit-0.4.6/macrokit/_symbol.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/macrokit/_validator.py` & `macro_kit-0.4.6/macrokit/_validator.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/macrokit/ast.py` & `macro_kit-0.4.6/macrokit/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,14 +563,20 @@
 def _named_expr(ast_object: ast.NamedExpr):
     head = Head.walrus
     target = from_ast(ast_object.target)
     args = [target, from_ast(ast_object.value)]
     return Expr(head, args)
 
 
+# python < 3.9
+@from_ast.register
+def _index(ast_object: ast.Index):
+    return from_ast(ast_object.value)  # type: ignore
+
+
 def _nest_binop(op, values: "list[ast.expr]"):
     if len(values) == 2:
         return [op, from_ast(values[0]), from_ast(values[1])]
     else:
         return [op, from_ast(values[0]), Expr(Head.binop, _nest_binop(op, values[1:]))]
```

### Comparing `macro_kit-0.4.5/macrokit/expression.py` & `macro_kit-0.4.6/macrokit/expression.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/macrokit/head.py` & `macro_kit-0.4.6/macrokit/head.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/macrokit/macro.py` & `macro_kit-0.4.6/macrokit/macro.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/macrokit/mock.py` & `macro_kit-0.4.6/macrokit/mock.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/macrokit/type_map.py` & `macro_kit-0.4.6/macrokit/type_map.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/macrokit/utils.py` & `macro_kit-0.4.6/macrokit/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from typing import Any
 import inspect
+import warnings
 from macrokit._symbol import Symbol
 from macrokit.expression import Expr
+from typing_extensions import Literal
 
 
 class ExprCheckError(Exception):
     """Exception raised when expression check failed."""
 
     def __init__(self, msg: str, expr: Symbol | Expr, line: Symbol | Expr):
         super().__init__(msg)
@@ -18,35 +20,60 @@
         """Error description with the causes."""
         return f"{super().__str__()} (Caused by: `{self._expr}` in `{self._line}`)"
 
 
 _BUILTIN_FUNCTION_OR_METHOD = type(print)
 
 
+def _runtime_exc(
+    mode: Literal["ignore", "warn", "raise"],
+    e: Exception,
+    line: Expr,
+) -> None:
+    if mode == "ignore":
+        pass
+    elif mode == "warn":
+        warnings.warn(f"Unexpected exception in line {line}: {e}")
+    elif mode == "raise":
+        raise e
+    else:
+        raise ValueError(f"Invalid mode: {mode}")
+
+
 # TODO: import
-def check_attributes(code: Expr, ns: dict[str, Any] = {}) -> list[ExprCheckError]:
+def check_attributes(
+    code: Expr,
+    ns: dict[str, Any] = {},
+    runtime_errors: Literal["ignore", "warn", "raise"] = "warn",
+) -> list[ExprCheckError]:
     """Check if the given code contains undefined attributes."""
-    errors = list[ExprCheckError]()
+    errors: list[ExprCheckError] = []
     for line in code.iter_lines():
         if isinstance(line, Symbol):
             continue
         for expr in line.iter_getattr():
             try:
                 expr.eval(ns)
             except AttributeError as e:
                 errors.append(ExprCheckError(str(e), expr, line))
             except NameError:
                 # variables defined during the execution of the code.
                 pass
+            except Exception as e:
+                _runtime_exc(runtime_errors, e, line)
     return errors
 
 
-def check_call_args(code: Expr, ns: dict[str, Any] = {}) -> list[ExprCheckError]:
+def check_call_args(
+    code: Expr,
+    ns: dict[str, Any] = {},
+    runtime_errors: Literal["ignore", "warn", "raise"] = "warn",
+) -> list[ExprCheckError]:
     """Check if all the function calls in the given code are valid."""
-    errors = list[ExprCheckError]()
+    errors: list[ExprCheckError] = []
     for line in code.iter_lines():
         if isinstance(line, Symbol):
             continue
         for expr in line.iter_call():
             fexpr, args, kwargs = expr.split_call()
             _method = fexpr.eval(ns)
             if isinstance(_method, _BUILTIN_FUNCTION_OR_METHOD):
@@ -54,8 +81,10 @@
             try:
                 inspect.signature(_method).bind(*args, **kwargs)
             except TypeError as e:
                 errors.append(ExprCheckError(str(e), expr, line))
             except (ValueError, NameError):
                 # builtin classes such as `range`.
                 pass
+            except Exception as e:
+                _runtime_exc(runtime_errors, e, line)
     return errors
```

### Comparing `macro_kit-0.4.5/macrokit/ipython/magic.py` & `macro_kit-0.4.6/macrokit/ipython/magic.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/macrokit/julia/translate.py` & `macro_kit-0.4.6/macrokit/julia/translate.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/.gitignore` & `macro_kit-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/LICENSE` & `macro_kit-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/README.md` & `macro_kit-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.5/pyproject.toml` & `macro_kit-0.4.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 [project]
 name = "macro-kit"
 dynamic = ["version"]
 description = "Macro recording and metaprogramming in Python"
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 authors = [
     { name = "Hanjin Liu", email = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp" },
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "typing_extensions",
 ]
```

### Comparing `macro_kit-0.4.5/PKG-INFO` & `macro_kit-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macro-kit
-Version: 0.4.5
+Version: 0.4.6
 Summary: Macro recording and metaprogramming in Python
 Project-URL: Download, https://github.com/hanjinliu/macro-kit
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
@@ -32,18 +32,19 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # macro-kit
 
 `macro-kit` is a package for efficient macro recording and metaprogramming in Python using abstract syntax tree (AST).
```

