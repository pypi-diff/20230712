# Comparing `tmp/oqpy-0.3.0.tar.gz` & `tmp/oqpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqpy-0.3.0.tar", max compression
+gzip compressed data, was "oqpy-0.3.1.tar", max compression
```

## Comparing `oqpy-0.3.0.tar` & `oqpy-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1957 2023-06-20 21:22:31.425953 oqpy-0.3.0/CITATION.cff
--rw-r--r--   0        0        0    11328 2022-09-19 17:51:00.552588 oqpy-0.3.0/LICENSE
--rw-r--r--   0        0        0       71 2022-09-19 17:51:00.552909 oqpy-0.3.0/NOTICE
--rw-r--r--   0        0        0     6506 2023-06-20 21:22:31.426565 oqpy-0.3.0/README.md
--rw-r--r--   0        0        0     1011 2023-06-22 18:01:55.965412 oqpy-0.3.0/oqpy/__init__.py
--rw-r--r--   0        0        0    21295 2023-06-22 18:01:55.966357 oqpy-0.3.0/oqpy/base.py
--rw-r--r--   0        0        0    14289 2023-06-22 18:01:55.967309 oqpy-0.3.0/oqpy/classical_types.py
--rw-r--r--   0        0        0     5472 2023-06-22 18:01:55.968896 oqpy-0.3.0/oqpy/control_flow.py
--rw-r--r--   0        0        0    23815 2023-06-22 18:01:55.970221 oqpy-0.3.0/oqpy/program.py
--rw-r--r--   0        0        0     2702 2023-06-20 21:40:48.272150 oqpy-0.3.0/oqpy/pulse.py
--rw-r--r--   0        0        0     4435 2023-05-13 00:40:15.485776 oqpy-0.3.0/oqpy/quantum_types.py
--rw-r--r--   0        0        0     8337 2023-06-22 18:01:55.971346 oqpy-0.3.0/oqpy/subroutines.py
--rw-r--r--   0        0        0     3985 2023-06-22 18:01:55.972231 oqpy-0.3.0/oqpy/timing.py
--rw-r--r--   0        0        0     3663 2023-06-22 18:01:55.973559 oqpy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7945 1970-01-01 00:00:00.000000 oqpy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1957 2023-07-10 17:07:57.634999 oqpy-0.3.1/CITATION.cff
+-rw-r--r--   0        0        0    11328 2023-07-10 17:07:57.635282 oqpy-0.3.1/LICENSE
+-rw-r--r--   0        0        0       71 2023-07-10 17:07:57.635450 oqpy-0.3.1/NOTICE
+-rw-r--r--   0        0        0     6506 2023-07-10 17:07:57.635557 oqpy-0.3.1/README.md
+-rw-r--r--   0        0        0     1011 2023-07-11 21:42:26.697698 oqpy-0.3.1/oqpy/__init__.py
+-rw-r--r--   0        0        0    21295 2023-07-10 17:07:57.636548 oqpy-0.3.1/oqpy/base.py
+-rw-r--r--   0        0        0    14289 2023-07-11 18:44:55.227171 oqpy-0.3.1/oqpy/classical_types.py
+-rw-r--r--   0        0        0     5472 2023-07-10 17:07:57.636781 oqpy-0.3.1/oqpy/control_flow.py
+-rw-r--r--   0        0        0    24795 2023-07-11 21:42:26.698151 oqpy-0.3.1/oqpy/program.py
+-rw-r--r--   0        0        0     2702 2023-07-10 17:07:57.637125 oqpy-0.3.1/oqpy/pulse.py
+-rw-r--r--   0        0        0     4440 2023-07-11 21:42:26.698644 oqpy-0.3.1/oqpy/quantum_types.py
+-rw-r--r--   0        0        0     8678 2023-07-11 21:42:23.776313 oqpy-0.3.1/oqpy/subroutines.py
+-rw-r--r--   0        0        0     3985 2023-07-10 17:07:57.637542 oqpy-0.3.1/oqpy/timing.py
+-rw-r--r--   0        0        0     3663 2023-07-11 21:42:26.699276 oqpy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7945 1970-01-01 00:00:00.000000 oqpy-0.3.1/PKG-INFO
```

### Comparing `oqpy-0.3.0/CITATION.cff` & `oqpy-0.3.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `oqpy-0.3.0/LICENSE` & `oqpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oqpy-0.3.0/README.md` & `oqpy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `oqpy-0.3.0/oqpy/__init__.py` & `oqpy-0.3.1/oqpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 ############################################################################
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 from oqpy.classical_types import *
 from oqpy.control_flow import *
 from oqpy.program import *
 from oqpy.pulse import *
 from oqpy.quantum_types import *
 from oqpy.subroutines import *
 from oqpy.timing import *
```

### Comparing `oqpy-0.3.0/oqpy/base.py` & `oqpy-0.3.1/oqpy/base.py`

 * *Files identical despite different names*

### Comparing `oqpy-0.3.0/oqpy/classical_types.py` & `oqpy-0.3.1/oqpy/classical_types.py`

 * *Files identical despite different names*

### Comparing `oqpy-0.3.0/oqpy/control_flow.py` & `oqpy-0.3.1/oqpy/control_flow.py`

 * *Files identical despite different names*

### Comparing `oqpy-0.3.0/oqpy/program.py` & `oqpy-0.3.1/oqpy/program.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,15 @@
             tuple[tuple[str, ...], str, tuple[str, ...]], ast.CalibrationDefinition
         ] = {}
         self.subroutines: dict[str, ast.SubroutineDefinition] = {}
         self.externs: dict[str, ast.ExternDeclaration] = {}
         self.declared_vars: dict[str, Var] = {}
         self.undeclared_vars: dict[str, Var] = {}
         self.simplify_constants = simplify_constants
+        self.declared_subroutines: set[str] = set()
 
         if version is None or (
             len(version.split(".")) in [1, 2]
             and all([item.isnumeric() for item in version.split(".")])
         ):
             self.version = version
         else:
@@ -117,15 +118,18 @@
         if len(other.stack) > 1:
             raise RuntimeError("Cannot add subprogram with unclosed contextmanagers.")
         self._state.finalize_if_clause()
         self._state.body.extend(other._state.body)
         self._state.if_clause = other._state.if_clause
         self._state.finalize_if_clause()
         self.defcals.update(other.defcals)
-        self.subroutines.update(other.subroutines)
+        for name, subroutine_stmt in other.subroutines.items():
+            self._add_subroutine(
+                name, subroutine_stmt, needs_declaration=name not in other.declared_subroutines
+            )
         self.externs.update(other.externs)
         for var in other.declared_vars.values():
             self._mark_var_declared(var)
         for var in other.undeclared_vars.values():
             self._add_var(var)
         return self
 
@@ -202,20 +206,24 @@
                 encal=encal,
             )
 
     def _add_statement(self, stmt: ast.Statement) -> None:
         """Add a statment to the current context's program state."""
         self._state.add_statement(stmt)
 
-    def _add_subroutine(self, name: str, stmt: ast.SubroutineDefinition) -> None:
+    def _add_subroutine(
+        self, name: str, stmt: ast.SubroutineDefinition, needs_declaration: bool = True
+    ) -> None:
         """Register a subroutine which has been used.
 
         Subroutines are added to the top of the program upon conversion to ast.
         """
         self.subroutines[name] = stmt
+        if not needs_declaration:
+            self.declared_subroutines.add(name)
 
     def _add_defcal(
         self,
         qubit_names: list[str],
         name: str,
         arguments: list[str],
         stmt: ast.CalibrationDefinition,
@@ -266,30 +274,39 @@
             ignore_needs_declaration: If true, the field `_needs_declaration` of
                 undeclared variables is ignored and their declaration will not
                 be added to the AST
             encal_declarations: If true, when declaring undeclared variables,
                 if the variables have openpulse types, automatically wrap the
                 declarations in cal blocks.
         """
-        if not ignore_needs_declaration and self.undeclared_vars:
-            self.autodeclare(encal=encal_declarations)
+        mutating_prog = Program(self.version, self.simplify_constants)
+        mutating_prog += self
 
-        assert len(self.stack) == 1
-        self._state.finalize_if_clause()
-        if self._state.annotations:
-            warnings.warn(f"Annotation(s) {self._state.annotations} not applied to any statement")
+        if not ignore_needs_declaration and mutating_prog.undeclared_vars:
+            mutating_prog.autodeclare(encal=encal_declarations)
+
+        assert len(mutating_prog.stack) == 1
+        mutating_prog._state.finalize_if_clause()
+        if mutating_prog._state.annotations:
+            warnings.warn(
+                f"Annotation(s) {mutating_prog._state.annotations} not applied to any statement"
+            )
         statements = []
         if include_externs:
-            statements += self._make_externs_statements(encal_declarations)
-        statements += list(self.subroutines.values()) + self._state.body
+            statements += mutating_prog._make_externs_statements(encal_declarations)
+        statements += [
+            mutating_prog.subroutines[subroutine_name]
+            for subroutine_name in mutating_prog.subroutines
+            if subroutine_name not in mutating_prog.declared_subroutines
+        ] + mutating_prog._state.body
         if encal:
             statements = [ast.CalibrationStatement(statements)]
         if encal_declarations:
             statements = [ast.CalibrationGrammarDeclaration("openpulse")] + statements
-        prog = ast.Program(statements=statements, version=self.version)
+        prog = ast.Program(statements=statements, version=mutating_prog.version)
         if encal_declarations:
             MergeCalStatementsPass().visit(prog)
         return prog
 
     def to_qasm(
         self,
         encal: bool = False,
@@ -338,20 +355,26 @@
             else:
                 openqasm_vars.append(var)
 
         if to_beginning:
             openqasm_vars.reverse()
 
         for var in openqasm_vars:
-            stmt = var.make_declaration_statement(self)
+            if callable(var) and hasattr(var, "subroutine_declaration"):
+                name, stmt = var.subroutine_declaration  # type: ignore[attr-defined]
+                self._add_subroutine(name, stmt, needs_declaration=False)
+            else:
+                stmt = var.make_declaration_statement(self)
+                self._mark_var_declared(var)
+
             if to_beginning:
                 self._state.body.insert(0, stmt)
             else:
                 self._add_statement(stmt)
-            self._mark_var_declared(var)
+
         if openpulse_vars:
             cal_stmt = ast.CalibrationStatement([])
             for var in openpulse_vars:
                 stmt = var.make_declaration_statement(self)
                 cal_stmt.body.append(stmt)
                 self._mark_var_declared(var)
             if to_beginning:
```

### Comparing `oqpy-0.3.0/oqpy/pulse.py` & `oqpy-0.3.1/oqpy/pulse.py`

 * *Files identical despite different names*

### Comparing `oqpy-0.3.0/oqpy/quantum_types.py` & `oqpy-0.3.1/oqpy/quantum_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     program._push()
     if len(variables) > 1:
         yield variables
     elif len(variables) == 1:
         yield variables[0]
     else:
-        yield
+        yield None
     state = program._pop()
 
     stmt = ast.CalibrationDefinition(
         ast.Identifier(name),
         arguments_ast,
         [ast.Identifier(q.name) for q in qubits],
         return_type,
```

### Comparing `oqpy-0.3.0/oqpy/subroutines.py` & `oqpy-0.3.1/oqpy/subroutines.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,136 +26,145 @@
 
 import oqpy.program
 from oqpy.base import AstConvertible, OQPyExpression, make_annotations, to_ast
 from oqpy.classical_types import OQFunctionCall, _ClassicalVar
 from oqpy.quantum_types import Qubit
 from oqpy.timing import convert_float_to_duration
 
-__all__ = ["subroutine", "annotate_subroutine", "declare_extern", "declare_waveform_generator"]
+__all__ = ["subroutine", "declare_extern", "declare_waveform_generator"]
 
 SubroutineParams = [oqpy.Program, VarArg(AstConvertible)]
 
+FnType = TypeVar("FnType", bound=Callable[..., Any])
+
+
+def enable_decorator_arguments(f: FnType) -> Callable[..., FnType]:
+    @functools.wraps(f)
+    def decorator(*args, **kwargs):  # type: ignore[no-untyped-def]
+        if len(args) == 1 and len(kwargs) == 0 and callable(args[0]):
+            return f(args[0])
+        else:
+            return lambda realf: f(realf, *args, **kwargs)
 
+    return decorator
+
+
+@enable_decorator_arguments
 def subroutine(
-    func: Callable[[oqpy.Program, VarArg(AstConvertible)], AstConvertible | None]
+    func: Callable[[oqpy.Program, VarArg(AstConvertible)], AstConvertible | None],
+    annotations: Sequence[str | tuple[str, str]] = (),
 ) -> Callable[[oqpy.Program, VarArg(AstConvertible)], OQFunctionCall]:
     """Decorator to declare a subroutine.
 
     The function should take a program as well as any other arguments required.
     Note that the decorated function must include type hints for all arguments,
     and (other than the initial program) all of these type hints must be oqpy
     Variable types.
 
     .. code-block:: python
 
-        @subroutine
+        @subroutine(annotations=("optimize", "-O3"))
         def increment_variable(program: Program, i: IntVar):
             program.increment(i, 1)
 
         j = IntVar(0)
         increment_variable(j)
 
     This should generate the following OpenQASM:
 
     .. code-block:: qasm3
 
+        @optimize -O3
         def increment_variable(int[32] i) {
             i += 1;
         }
 
         int[32] j = 0;
         increment_variable(j);
 
+    Args:
+        func (Callable[[oqpy.Program, VarArg(AstConvertible)], AstConvertible | None]):
+            function to decorate. Its first argument must be an OQpy program.
+        annotations (Sequence[str | tuple[str, str]]): a collection of strings or
+            tuples of string that annotate the subroutine.
+
+    Returns:
+        Callable[[oqpy.Program, VarArg(AstConvertible)], AstConvertible | None]:
+            decorated function with added subroutine_declaration attribute.
     """
+    name = func.__name__
+    identifier = ast.Identifier(func.__name__)
+    argnames = list(inspect.signature(func).parameters.keys())
+    type_hints = get_type_hints(func)
+    inputs = {}  # used as inputs when calling the actual python function
+    arguments = []  # used in the ast definition of the subroutine
+    for argname in argnames[1:]:  # arg 0 should be program
+        if argname not in type_hints:
+            raise ValueError(f"No type hint provided for {argname} on subroutine {name}.")
+        input_ = inputs[argname] = type_hints[argname](name=argname)
+
+        if isinstance(input_, _ClassicalVar):
+            arguments.append(ast.ClassicalArgument(input_.type, ast.Identifier(argname)))
+        elif isinstance(input_, Qubit):
+            arguments.append(ast.QuantumArgument(ast.Identifier(input_.name), None))
+        else:
+            raise ValueError(
+                f"Type hint for {argname} on subroutine {name} is not an oqpy variable type."
+            )
+
+    inner_prog = oqpy.Program()
+    for input_val in inputs.values():
+        inner_prog._mark_var_declared(input_val)
+    output = func(inner_prog, **inputs)
+    inner_prog.autodeclare()
+    inner_prog._state.finalize_if_clause()
+    body = inner_prog._state.body
+    if isinstance(output, OQPyExpression):
+        return_type = output.type
+        body.append(ast.ReturnStatement(to_ast(inner_prog, output)))
+    elif output is None:
+        return_type = None
+        if type_hints.get("return", False):
+            return_hint = type_hints["return"]()
+            if isinstance(return_hint, _ClassicalVar):
+                return_type = return_hint.type
+            elif return_hint is not None:
+                raise ValueError(
+                    f"Type hint for return variable on subroutine {name} is not an oqpy classical type."
+                )
+    else:
+        raise ValueError("Output type of subroutine {name} was neither oqpy expression nor None.")
+    stmt = ast.SubroutineDefinition(
+        identifier,
+        arguments=arguments,
+        return_type=return_type,
+        body=body,
+    )
+    stmt.annotations = make_annotations(annotations)
 
     @functools.wraps(func)
     def wrapper(
         program: oqpy.Program,
         *args: AstConvertible,
-        annotations: Sequence[str | tuple[str, str]] = (),
     ) -> OQFunctionCall:
-        name = func.__name__
-        identifier = ast.Identifier(func.__name__)
-        argnames = list(inspect.signature(func).parameters.keys())
-        type_hints = get_type_hints(func)
-        inputs = {}  # used as inputs when calling the actual python function
-        arguments = []  # used in the ast definition of the subroutine
-        for argname in argnames[1:]:  # arg 0 should be program
-            if argname not in type_hints:
-                raise ValueError(f"No type hint provided for {argname} on subroutine {name}.")
-            input_ = inputs[argname] = type_hints[argname](name=argname)
-
-            if isinstance(input_, _ClassicalVar):
-                arguments.append(ast.ClassicalArgument(input_.type, ast.Identifier(argname)))
-            elif isinstance(input_, Qubit):
-                arguments.append(ast.QuantumArgument(ast.Identifier(input_.name), None))
-            else:
-                raise ValueError(
-                    f"Type hint for {argname} on subroutine {name} is not an oqpy variable type."
-                )
-
-        inner_prog = oqpy.Program()
-        for input_val in inputs.values():
-            inner_prog._mark_var_declared(input_val)
-        output = func(inner_prog, **inputs)
-        body = inner_prog._state.body
-        if isinstance(output, OQPyExpression):
-            return_type = output.type
-            body.append(ast.ReturnStatement(to_ast(inner_prog, output)))
-        elif output is None:
-            return_type = None
-            if type_hints.get("return", False):
-                return_hint = type_hints["return"]()
-                if isinstance(return_hint, _ClassicalVar):
-                    return_type = return_hint.type
-                elif return_hint is not None:
-                    raise ValueError(
-                        f"Type hint for return variable on subroutine {name} is not an oqpy classical type."
-                    )
-        else:
-            raise ValueError(
-                "Output type of subroutine {name} was neither oqpy expression nor None."
-            )
-        stmt = ast.SubroutineDefinition(
+        program.defcals.update(inner_prog.defcals)
+        for name, subroutine_stmt in inner_prog.subroutines.items():
+            program._add_subroutine(name, subroutine_stmt)
+        program.externs.update(inner_prog.externs)
+        return OQFunctionCall(
             identifier,
-            arguments=arguments,
-            return_type=return_type,
-            body=body,
+            args,
+            return_type,
+            subroutine_decl=stmt,
         )
-        stmt.annotations = make_annotations(annotations)
-        return OQFunctionCall(identifier, args, return_type, subroutine_decl=stmt)
 
+    setattr(wrapper, "subroutine_declaration", (name, stmt))
     return wrapper
 
 
-FnType = TypeVar("FnType", bound=Callable[..., Any])
-
-
-def annotate_subroutine(keyword: str, command: str | None = None) -> Callable[[FnType], FnType]:
-    """Add annotation to a subroutine."""
-
-    def annotate_subroutine_decorator(func: FnType) -> FnType:
-        @functools.wraps(func)
-        def wrapper(
-            program: oqpy.Program,
-            *args: AstConvertible,
-            annotations: Sequence[str | tuple[str, str]] = (),
-        ) -> OQFunctionCall:
-            new_ann: str | tuple[str, str]
-            if command is not None:
-                new_ann = keyword, command
-            else:
-                new_ann = keyword
-            return func(program, *args, annotations=list(annotations) + [new_ann])
-
-        return wrapper  # type: ignore[return-value]
-
-    return annotate_subroutine_decorator
-
-
 def declare_extern(
     name: str,
     args: list[tuple[str, ast.ClassicalType]],
     return_type: ast.ClassicalType,
     annotations: Sequence[str | tuple[str, str]] = (),
 ) -> Callable[..., OQFunctionCall]:
     """Declare an extern and return a callable which adds the extern.
```

### Comparing `oqpy-0.3.0/oqpy/timing.py` & `oqpy-0.3.1/oqpy/timing.py`

 * *Files identical despite different names*

### Comparing `oqpy-0.3.0/pyproject.toml` & `oqpy-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oqpy"
-version = "0.3.0"
+version = "0.3.1"
 description = "Generating OpenQASM 3 + OpenPulse in Python"
 authors = ["OQpy Contributors <oqpy-contributors@amazon.com>"]
 license = "Apache-2.0"
 include = ["CITATION.cff", "NOTICE"]
 readme = "README.md"
 repository = "https://github.com/openqasm/oqpy"
 keywords = ["openqasm", "quantum"]
```

### Comparing `oqpy-0.3.0/PKG-INFO` & `oqpy-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oqpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generating OpenQASM 3 + OpenPulse in Python
 Home-page: https://github.com/openqasm/oqpy
 License: Apache-2.0
 Keywords: openqasm,quantum
 Author: OQpy Contributors
 Author-email: oqpy-contributors@amazon.com
 Requires-Python: >=3.7,<4.0
```

