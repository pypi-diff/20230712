# Comparing `tmp/py2js-1.1.8.tar.gz` & `tmp/py2js-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2js-1.1.8.tar", last modified: Thu Mar 16 00:29:45 2023, max compression
+gzip compressed data, was "py2js-1.2.1.tar", last modified: Wed Jul 12 14:45:39 2023, max compression
```

## Comparing `py2js-1.1.8.tar` & `py2js-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 00:29:45.363613 py2js-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-16 00:29:32.000000 py2js-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-03-16 00:29:45.363613 py2js-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-03-16 00:29:32.000000 py2js-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 00:29:45.363613 py2js-1.1.8/py2js/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-16 00:29:32.000000 py2js-1.1.8/py2js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23495 2023-03-16 00:29:32.000000 py2js-1.1.8/py2js/py2js.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-16 00:29:32.000000 py2js-1.1.8/py2js/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 00:29:45.363613 py2js-1.1.8/py2js.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-03-16 00:29:45.000000 py2js-1.1.8/py2js.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-16 00:29:45.000000 py2js-1.1.8/py2js.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 00:29:45.000000 py2js-1.1.8/py2js.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-16 00:29:45.000000 py2js-1.1.8/py2js.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 00:29:45.363613 py2js-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-16 00:29:32.000000 py2js-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:45:39.319767 py2js-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-12 14:45:30.000000 py2js-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-12 14:45:39.319767 py2js-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-12 14:45:30.000000 py2js-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:45:39.315767 py2js-1.2.1/py2js/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 14:45:30.000000 py2js-1.2.1/py2js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27792 2023-07-12 14:45:30.000000 py2js-1.2.1/py2js/py2js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-12 14:45:30.000000 py2js-1.2.1/py2js/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:45:39.319767 py2js-1.2.1/py2js.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-12 14:45:39.000000 py2js-1.2.1/py2js.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-12 14:45:39.000000 py2js-1.2.1/py2js.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:45:39.000000 py2js-1.2.1/py2js.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 14:45:39.000000 py2js-1.2.1/py2js.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:45:39.319767 py2js-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-12 14:45:30.000000 py2js-1.2.1/setup.py
```

### Comparing `py2js-1.1.8/LICENSE` & `py2js-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py2js-1.1.8/PKG-INFO` & `py2js-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: py2js
-Version: 1.1.8
+Version: 1.2.1
 Summary: Write javascript in python with python syntax
 Home-page: https://github.com/am230/py2js
 Author: am230
 Author-email: am.230@outlook.jp
 License: MIT Licence
 Keywords: javascript,convert,translator
 Platform: any
 Requires: jsbeautifier
-Requires: strbuilder
+Requires: strinpy
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Python to Javascript translator
 ===============================
 
 .. image:: https://img.shields.io/github/license/mashape/apistatus.svg
```

### Comparing `py2js-1.1.8/README.rst` & `py2js-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `py2js-1.1.8/py2js/py2js.py` & `py2js-1.2.1/py2js/py2js.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,49 @@
+from pathlib import Path
 import ast
 import enum
 import inspect
 import re
 import types
 from dataclasses import dataclass, field
 from functools import reduce
-from typing import Any, List, Dict, Optional, Union, Callable
+from typing import List, Dict, Optional, Union, Callable
 
 import jsbeautifier
-from strbuilder import Builder, SurroundBuilder
+import strinpy
 
 from .visitor import Visitor, VisitorContext
 
 
 class JSScope(enum.Enum):
     MODULE = 0
     CLASS_FIELD = 1
     FUNCTION_FIELD = 2
     ARGUMENT = 3
     F_STRING = 4
-    FOR_LOOP = 5
+    JOINED_STR = 5
+    FOR_LOOP = 6
 
 
 @dataclass
 class JSVisitorContext(VisitorContext):
     variables: List[str] = field(default_factory=list)
     global_variables: list[str] = field(default_factory=list)
     scope: JSScope = field(default=JSScope.MODULE)
     break_suffix: str = field(default='')
-    parent: ast.AST = field(default=None)
-    node: ast.AST = field(default=None)
+    parent: Optional[ast.AST] = field(default=None)
+    node: Optional[ast.AST] = field(default=None)
     has_yield: bool = field(default=False)
 
     def is_existed(self, name: str) -> bool:
         return name in self.variables or name in self.global_variables
 
     def copy(
         self,
-        variables: Dict[str, Any] = None,
+        variables: Optional[List[str]] = None,
         node: Optional[ast.AST] = None,
         scope: Optional[JSScope] = None,
         break_suffix: Optional[str] = None,
         has_yield: Optional[bool] = None,
         root: Optional['JSVisitorContext'] = None
     ) -> 'JSVisitorContext':
         return JSVisitorContext(
@@ -51,18 +53,14 @@
             break_suffix=self.break_suffix if break_suffix is None else break_suffix,
             parent=self.node,
             node=node or self.node,
             has_yield=self.has_yield if has_yield is None else has_yield
         )
 
 
-class ConstantConsumer:
-    def __call__(self, value: Any, ctx: JSVisitorContext) -> str: ...
-
-
 class CodeGen(Visitor[JSVisitorContext]):
     BOOL_OP_TABLE: Dict[type, str] = {
         ast.Or: '||',
         ast.And: '&&'
     }
 
     UNARY_OP_TABLE: Dict[type, str] = {
@@ -96,217 +94,261 @@
         ast.Mod: '%',
         ast.Mult: '*',
         ast.Pow: '**',
         ast.RShift: '>>',
         ast.Sub: '-',
     }
 
-    CONSTANT_CONSUMER_TABLE: Dict[type, ConstantConsumer] = {
+    CONSTANT_CONSUMER_TABLE: Dict[type, Callable] = {
         bool: lambda value, ctx: 'true' if value else 'false',
-        str: lambda value, ctx: ('%s' if ctx.scope == JSScope.F_STRING else f'`%s`') % value.replace('`', '\\`').replace('$', '\\$'),
+        # str: lambda value, ctx: ("'%s'" if ctx.scope == JSScope.F_STRING else f'`%s`') % value.replace('`', '\\`').replace('$', '\\$'),
+        str: lambda value, ctx: value.replace('\\', '\\\\').replace('$', '\\$').replace('`', '\\`') if ctx.scope == JSScope.JOINED_STR else "'{}'".format(value.replace('\\', '\\\\').replace('\'', '\\\'')) if ctx.scope == JSScope.F_STRING else '\'{}\''.format(value.replace('\\', '\\\\').replace("'", "\\'")),
         int: lambda value, ctx: str(value),
         float: lambda value, ctx: str(value),
+        bytes: lambda value, ctx: f'new Uint8Array([{",".join(str(b) for b in value)}])',
         type(None): lambda _, ctx: 'null',
         type(...): lambda _, ctx: 'ellipsis'
     }
 
-    def __init__(self, python_compatible: bool = False) -> None:
-        self.python_compatible = python_compatible
+    def __init__(self, compatible: bool = False) -> None:
+        self.compatible = compatible
         super().__init__(JSVisitorContext)
 
-    def sperator(self, ast: Union[List[ast.AST], ast.AST], context: Optional[JSVisitorContext] = None):
+    def sperator(self, ast: Union[List[ast.AST], ast.AST], context: JSVisitorContext):
         if context.scope == JSScope.ARGUMENT:
             return ','
         return ';'
 
     def visit_Module(self, node: ast.Module, ctx: JSVisitorContext):
         return self.visit(node.body, ctx)
 
     def visit_Import(self, node: ast.Import, ctx: JSVisitorContext):
-        return [f'import * as {x.asname} from "{x.name}"' if x.asname else f'import "{x.name}"' for x in node.names]
+        items = []
+        for item in node.names:
+            if item.asname:
+                items.append(f'import * as {item.asname} from "{item.name}"')
+            else:
+                items.append(f'import "{item.name}"')
+        return ';'.join(items)
 
     def visit_ImportFrom(self, node: ast.ImportFrom, ctx: JSVisitorContext):
-        builder = Builder(separator=',')
+        items = []
         for item in node.names:
             if item.name == '*':
-                builder.write(f'/* Wildcard import not supported: {node.module} */')
+                items.append(f'/* Wildcard import not supported: {node.module} */')
                 continue
-            builder.write(f'{item.name} as {item.asname}' if item.asname else item.name)
-        dir = '"../"'
-        return f'import {{{builder.build()}}} from {node.module or dir}'
+            items.append(f'{item.name} as {item.asname}' if item.asname else item.name)
+
+        return strinpy.build([
+            'import ',
+            ['{',
+                ', '.join(items),
+             '}',],
+            f' from ',
+            node.module or '"../"'
+        ])
 
     def visit_ClassDef(self, node: ast.ClassDef, ctx: JSVisitorContext):
         context = ctx.copy(scope=JSScope.CLASS_FIELD)
 
-        body = node.body
-        name = ast.Name(node.name)
-        builder = Builder()\
-            .write(f'let {node.name} = class')\
-            .write(SurroundBuilder(surround='{}')
-                   .write_if(self.python_compatible, lambda: '''constructor(...args) {if ('__init__' in this) this.__init__(...args); return new Proxy(this, { apply: (target, self, args) => target.__call__(...args), get: (target, key) => target.__getitem__(key) })}''')
-                   .write(self.visit(filter(lambda node: isinstance(node, ast.FunctionDef), body), context))
-                   .write(self.visit(filter(lambda node: not isinstance(node, ast.FunctionDef), body), context))
-                   )\
-            .write_if(node.bases, lambda: (f'''Object.getOwnPropertyNames({base}.prototype).forEach(name => {{if (name !== 'constructor') {{{node.name}.prototype[name] = {base}.prototype[name];}}}});''' for base in map(lambda base: self.visit(base, ctx), node.bases)))\
-            .write(f'{node.name} = new Proxy({node.name}, {{ apply: (clazz, thisValue, args) => new clazz(...args) }});')\
-            .write_if(node.decorator_list, lambda: (f'{node.name} = ', reduce(lambda value, element: f'{element}({value})', map(lambda decorator: self.visit(decorator, ctx), node.decorator_list), node.name), ';'))
-
-        return builder.build()
+        return strinpy.build([
+            f'let {node.name} = class',
+            ['{',
+                self.compatible and '''constructor(...args) {if ('__init__' in this) this.__init__(...args); return new Proxy(this, { apply: (target, self, args) => target.__call__(...args), get: (target, key) => target[key] || target.__getitem__(key) })}''',
+                self.visit(filter(lambda node: not isinstance(node, ast.FunctionDef), node.body), context),
+                ';',
+                self.visit(filter(lambda node: isinstance(node, ast.FunctionDef), node.body), context),
+             '}'],
+            node.bases and [f'''Object.getOwnPropertyNames({base}.prototype).forEach(name => {{if (name !== 'constructor') {{{node.name}.prototype[name] = {base}.prototype[name];}}}});''' for base in map(lambda base: self.visit(base, ctx), node.bases)],
+            f'{node.name} = new Proxy({node.name}, {{ apply: (clazz, thisValue, args) => new clazz(...args) }});',
+            node.decorator_list and (f'{node.name} = ', reduce(lambda value, element: f'{element}({value})', map(lambda decorator: self.visit(decorator, ctx), node.decorator_list), node.name), ';'),
+        ])
 
     def visit_FunctionDef(self, node: ast.FunctionDef, ctx: JSVisitorContext):
         context = ctx.copy(scope=JSScope.FUNCTION_FIELD)
 
+        constructor = node.name == '__init__'
+
         body = self.visit(node.body, context)
         if ctx.scope == JSScope.CLASS_FIELD:
-            builder = Builder()
-            builder.write_if(context.has_yield, '*')
-            builder.write(node.name)
-            if self.python_compatible:
-                (
-                    builder
-                    .write('=(...__args)=>{')
-                    .write(f'({self.visit(node.args, ctx)} =>')
-                    .write(SurroundBuilder(surround='{}')
-                           .write(body))
-                    .write(')(this,...__args)}')
-                )
+            if self.compatible:
+                code = [
+                    context.has_yield and '*',
+                    node.name,
+                    node.decorator_list and '=',
+                    [[self.visit(decorator, ctx), '('] for decorator in node.decorator_list],
+                    '(...__args)',
+                    node.decorator_list and '=>',
+                    '{',
+                    f'({self.visit(node.args, ctx)}',
+                    '=>'
+                    '{', body, '}',
+                    ')(this,...__args)}',
+                    [[')'] for decorator in node.decorator_list],
+                ]
+                return strinpy.build(code)
             else:
-                (
-                    builder
-                    .write(self.visit(node.args, ctx))
-                    .write(SurroundBuilder(surround='{}')
-                           .write(body))
-                )
-            return builder.build()
-        builder = Builder()\
-            .write_if(not ctx.is_existed(node.name), 'let')\
-            .write(node.name)\
-            .write('=')\
-            .write_if(context.has_yield, 'function*')\
-            .write(f'{self.visit(node.args, ctx)}')\
-            .write_if(not context.has_yield, '=>')\
-            .write(SurroundBuilder(surround='{}')
-                   .write(body))
+                return strinpy.build([
+                    context.has_yield and '*',
+                    node.name,
+                    node.decorator_list and '=',
+                    [[self.visit(decorator, ctx), '('] for decorator in node.decorator_list],
+                    self.visit(node.args, ctx),
+                    node.decorator_list and '=>',
+                    '{', body, '}',
+                    [[')'] for decorator in node.decorator_list],
+                ])
+
+        code = [
+            not ctx.is_existed(node.name) and 'let',
+            f' {node.name}',
+            '=',
+            # decorator
+            [[self.visit(decorator, ctx), '('] for decorator in node.decorator_list],
+            context.has_yield and 'function*',
+            self.visit(node.args, ctx),
+            not context.has_yield and '=>',
+            '{', body, '}',
+            [[')'] for decorator in node.decorator_list],
+        ]
         ctx.variables.append(node.name)
-        return builder.build()
+
+        return strinpy.build(code)
 
     def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef, ctx: JSVisitorContext):
         context = ctx.copy(scope=JSScope.FUNCTION_FIELD)
 
         body = self.visit(node.body, context)
 
         if ctx.scope == JSScope.CLASS_FIELD:
-            return Builder()\
-                .write_if(context.has_yield, '*')\
-                .write(node.name)\
-                .write(f'{self.visit(node.args, ctx)}')\
-                .write(SurroundBuilder(surround='{}')
-                       .write(body))\
-                .build()
-        builder = Builder()\
-            .write_if(not ctx.is_existed(node.name), 'let')\
-            .write(node.name)\
-            .write('=')\
-            .write_if(context.has_yield, 'async function*', or_else='async')\
-            .write(f'{self.visit(node.args, ctx)}')\
-            .write_if(not context.has_yield, '=>')\
-            .write(SurroundBuilder(surround='{}')
-                   .write(body))
+            return strinpy.build([
+                context.has_yield and '*',
+                node.name,
+                self.visit(node.args, ctx),
+                '{', body, '}',
+            ])
+
+        code = strinpy.build([
+            not ctx.is_existed(node.name) and 'let',
+            node.name,
+            '=',
+            'async function*' if context.has_yield else 'async',
+            self.visit(node.args, ctx),
+            not context.has_yield and '=>',
+            '{', body, '}',
+        ])
         ctx.variables.append(node.name)
-        return builder.build()
+        return code
 
     def visit_Yield(self, node: ast.Yield, ctx: JSVisitorContext):
         ctx.has_yield = True
         return f'yield {self.visit(node.value, ctx)}'
 
     def visit_YieldFrom(self, node: ast.YieldFrom, ctx: JSVisitorContext):
         ctx.has_yield = True
         return f'yield* {self.visit(node.value, ctx)}'
 
     def visit_If(self, node: ast.If, ctx: JSVisitorContext):
-        return Builder('if').write(SurroundBuilder(surround='()').write(self.visit(node.test, ctx))).write(SurroundBuilder(surround='{}').write(self.visit(node.body, ctx))).build()
+        return strinpy.build([
+            'if',
+            '(', self.visit(node.test, ctx), ')',
+            '{', self.visit(node.body, ctx), '}',
+            node.orelse and [
+                'else',
+                '{', self.visit(node.orelse, ctx), '}',
+            ],
+        ])
 
     def visit_Compare(self, node: ast.Compare, ctx: JSVisitorContext):
-        ops = Builder()
+        ops = []
         invert = False
         for op in node.ops:
             op_type = type(op)
-            ops.write(self.COMPARE_OP_TABLE[op_type])
+            ops.append(self.COMPARE_OP_TABLE[op_type])
             if op_type == ast.NotIn:
                 invert = True
 
-        builder = Builder(self.visit(node.left, ctx))
+        code = [self.visit(node.left, ctx)]
         comparators = node.comparators
         while comparators:
-            builder.write(ops.pop(0))
-            builder.write(self.visit(comparators.pop(0)))
-        if not invert:
-            return builder.build()
-        return f'!({builder.build()})'
+            code.append(ops.pop(0))
+            code.append(self.visit(comparators.pop(0)))
+        if invert:
+            return strinpy.build(['!(', code, ')'])
+        return strinpy.build(code)
 
     def visit_Name(self, node: ast.Name, ctx: JSVisitorContext):
         return node.id
 
     def visit_Constant(self, node: ast.Constant, ctx: JSVisitorContext):
         return self.CONSTANT_CONSUMER_TABLE[type(node.value)](node.value, ctx)
 
     def visit_Assign(self, node: ast.Assign, ctx: JSVisitorContext):
-        builder = Builder(separator=';')
+        code = []
 
         defines = [target.id for target in node.targets if isinstance(target, ast.Name) and not ctx.is_existed(target.id)]
         ctx.variables.extend(defines)
 
         if ctx.scope != JSScope.CLASS_FIELD:
             if len(node.targets) == len(defines):
-                builder.write(f'let {", ".join(defines)} = {self.visit(node.value, ctx)}')
-                return builder.build()
+                code.append(f'let {", ".join(defines)} = {self.visit(node.value, ctx)}')
+                return strinpy.build(code)
             elif defines:
-                builder.write(f'let {", ".join(defines)}')
-        builder.write(f'{self.visit(node.targets, ctx)} = {self.visit(node.value, ctx)}')
-        return builder.build()
-        # return Builder().write_if(node.targets in ctx.variables and ctx.scope != JSScope.CLASS_FIELD and not any(map(lambda target: isinstance(target, ast.Attribute), node.targets)), 'let').write(f'{self.visit(node.targets, ctx)} = {self.visit(node.value, ctx)}').build()
+                code.append(f'let {", ".join(defines)}')
+        code.append(f'{self.visit(node.targets, ctx)} = {self.visit(node.value, ctx)}')
+        return strinpy.build(code)
 
     def visit_Call(self, node: ast.Call, ctx: JSVisitorContext):
         context = ctx.copy(scope=JSScope.ARGUMENT)
 
         starreds = tuple(filter(lambda arg: isinstance(arg, ast.Starred), node.args))
-        args = filter(lambda arg: not isinstance(arg, ast.Starred), node.args)
+        args = list(filter(lambda arg: not isinstance(arg, ast.Starred), node.args))
 
-        return Builder(f'{self.visit(node.func, ctx)}')\
-            .write(SurroundBuilder(surround='()', separator=',')
-                   .write_if(args, lambda: self.visit(args, context))
-                   .write_if(node.keywords, lambda: SurroundBuilder(surround='{}', separator=',')
-                                 .write(self.visit(filter(lambda kw: kw.arg is not None, node.keywords), context))
-                                 .write(self.visit(filter(lambda kw: kw.arg is None, node.keywords), context)))
-                   .write_if(starreds, lambda: self.visit(starreds, context))
-                   ).build()
+        code = [
+            self.visit(node.func, ctx),
+            '(',
+            args and [self.visit(args, context)],
+            node.keywords and [
+                args and ', ',
+                '{',
+                self.visit(filter(lambda kw: kw.arg is not None, node.keywords), context),
+                self.visit(filter(lambda kw: kw.arg is None, node.keywords), context),
+                '}',
+            ],
+            starreds and self.visit(starreds, context),
+            ')',
+        ]
+        return strinpy.build(code)
 
     def visit_keyword(self, node: ast.keyword, ctx: JSVisitorContext):
         return f'{node.arg}:{self.visit(node.value)}' if node.arg is not None else f'...{self.visit(node.value)}'
 
     def visit_arguments(self, node: ast.arguments, ctx: JSVisitorContext):
         context = ctx.copy(scope=JSScope.ARGUMENT)
 
         kwlen = len(node.defaults)
         kwargs = node.args[-kwlen:]
         args = node.args[:len(node.args)-kwlen]
         keywords = dict(zip(kwargs, node.defaults))
 
-        return SurroundBuilder(surround='()')\
-            .write(
-            Builder(separator=',')
-            .write_if(node.args, self.visit(args, context))
-            .write_if(node.kwarg or node.defaults, lambda:
-                      SurroundBuilder(surround='{}', separator=',')
-                      .write_if(keywords, lambda: (f'{self.visit(key, context)}={self.visit(value, context)}' for key,  value in keywords.items()))
-                      .write_if(node.kwarg, lambda: f'...{self.visit(node.kwarg, context)}')
-                      .build() + '={}')
-            .write_if(node.vararg, lambda: f'...{self.visit(node.vararg, context)}')
-            .build()
-        ).build()
+        code = [
+            strinpy.build(args and self.visit(args, context)),
+            strinpy.build(bool(node.kwarg or node.defaults) and [
+                '{',
+                bool(keywords) and [f'{self.visit(key, context)}={self.visit(value, context)}' for key,  value in keywords.items()],
+                node.kwarg and [bool(keywords) and ',', f'...{self.visit(node.kwarg, context)}'],
+                '}',
+            ]),
+            strinpy.build(node.vararg and [f'...{self.visit(node.vararg, context)}']),
+        ]
+        return strinpy.build([
+            '(',
+            ', '.join(filter(None, code)),
+            ')',
+        ])
 
     def visit_Attribute(self, node: ast.Attribute, ctx: JSVisitorContext):
         return f'{self.visit(node.value, ctx)}.{node.attr}'
 
     def visit_Expr(self, node: ast.Expr, ctx: JSVisitorContext):
         return self.visit(node.value, ctx)
 
@@ -316,77 +358,133 @@
     def visit_arg(self, node: ast.arg, ctx: JSVisitorContext):
         return node.arg
 
     def visit_Return(self, node: ast.Return, ctx: JSVisitorContext):
         return f'return {self.visit(node.value, ctx)}'
 
     def visit_List(self, node: ast.List, ctx: JSVisitorContext):
-        return SurroundBuilder(surround='[]', separator=',').write(map(lambda item: self.visit(item, ctx), node.elts)).build()
+        return strinpy.build([
+            '[',
+            ', '.join(map(lambda item: self.visit(item, ctx), node.elts)),
+            ']',
+        ])
 
     def visit_Tuple(self, *args):
         return f'/*tuple*/{self.visit_List(*args)}'
 
     def visit_Dict(self, node: ast.Dict, ctx: JSVisitorContext):
-        return '{%s}' % ', '.join(f'{self.visit(key, ctx.copy(scope=JSScope.F_STRING))}: {self.visit(value, ctx)}' for key, value in zip(node.keys, node.values))
+        return '{%s}' % ', '.join(f'{self.visit(key, ctx.copy(scope=JSScope.F_STRING)) if isinstance(key, ast.Constant) else "["+self.visit(key, ctx.copy(scope=JSScope.F_STRING))+"]"}: {self.visit(value, ctx)}' for key, value in zip(node.keys, node.values))
+
+    def visit_Set(self, node: ast.Set, ctx: JSVisitorContext):
+        return f'new Set([{", ".join(map(lambda x: self.visit(x, ctx), node.elts))}])'
 
     def visit_Lambda(self, node: ast.Lambda, ctx: JSVisitorContext):
-        return f'{self.visit(node.args, ctx)}=> {{return {self.visit(node.body, ctx)}}}'
+        f'{self.visit(node.args, ctx)}=> {{return {self.visit(node.body, ctx)}}}'
+        return strinpy.build([
+            '(',
+            self.visit(node.args, ctx),
+            '=>{',
+            self.visit(node.body, ctx),
+            '}',
+            ')',
+        ])
 
     def visit_For(self, node: ast.For, ctx: JSVisitorContext):
-        target = Builder()
+        # target = Builder()
+        # if isinstance(node.target, ast.Name):
+        #     if not ctx.is_existed(node.target.id):
+        #         target.write(f'let')
+        # target.write(self.visit(node.target, ctx))
+
+        # return (
+        #     Builder()
+        #     .write_if(node.orelse, '__else: {')
+        #     .write(f'for ({target.build()} of {self.visit(node.iter, ctx)})')
+        #     .write(f"{{{self.visit(node.body, ctx.copy(break_suffix='__else' if node.orelse else ''))}}}")
+        #     .write_if(node.orelse, f'{self.visit(node.orelse, ctx)} }}')
+        # ).build()
+        target = []
         if isinstance(node.target, ast.Name):
             if not ctx.is_existed(node.target.id):
-                target.write(f'let')
-        target.write(self.visit(node.target, ctx))
+                target.append(f'let')
+        target.append(self.visit(node.target, ctx))
 
-        return (
-            Builder()
-            .write_if(node.orelse, '__else: {')
-            .write(f'for ({target.build()} of {self.visit(node.iter, ctx)})')
-            .write(f"{{{self.visit(node.body, ctx.copy(break_suffix='__else' if node.orelse else ''))}}}")
-            .write_if(node.orelse, f'{self.visit(node.orelse, ctx)} }}')
-        ).build()
+        code = [
+            node.orelse and '__else: {',
+            'for (',
+            ' '.join(target),
+            ' of ',
+            self.visit(node.iter, ctx),
+            ')',
+            '{',
+            self.visit(node.body, ctx.copy(break_suffix='__else' if node.orelse else '')),
+            '}',
+            node.orelse and f'{self.visit(node.orelse, ctx)} }}',
+        ]
+        return strinpy.build(code)
 
     def visit_AsyncFor(self, node: ast.AsyncFor, ctx: JSVisitorContext):
-        return (
-            Builder()
-            .write_if(node.orelse, '__else: {')
-            .write(f'for await ({self.visit(node.target, ctx)} of {self.visit(node.iter, ctx)})')
-            .write(f"{{{self.visit(node.body, ctx.copy(break_suffix='__else' if node.orelse else ''))}}}")
-            .write_if(node.orelse, f'{self.visit(node.orelse, ctx)} }}')
-        ).build()
+        # return (
+        #     Builder()
+        #     .write_if(node.orelse, '__else: {')
+        #     .write(f'for await ({self.visit(node.target, ctx)} of {self.visit(node.iter, ctx)})')
+        #     .write(f"{{{self.visit(node.body, ctx.copy(break_suffix='__else' if node.orelse else ''))}}}")
+        #     .write_if(node.orelse, f'{self.visit(node.orelse, ctx)} }}')
+        # ).build()
+        return strinpy.build([
+            node.orelse and '__else: {',
+            'for await (',
+            self.visit(node.target, ctx),
+            'of',
+            self.visit(node.iter, ctx),
+            ')',
+            '{',
+            self.visit(node.body, ctx.copy(break_suffix='__else' if node.orelse else '')),
+            '}',
+            node.orelse and f'{self.visit(node.orelse, ctx)} }}',
+        ])
 
     def visit_Await(self, node: ast.Await, ctx: JSVisitorContext):
         return f'await {self.visit(node.value, ctx)}'
 
     def visit_BoolOp(self, node: ast.BoolOp, ctx: JSVisitorContext):
         return self.BOOL_OP_TABLE[type(node.op)].join(map(lambda value: self.visit(value, ctx), node.values))
 
     def visit_UnaryOp(self, node: ast.UnaryOp, ctx: JSVisitorContext):
         return f'{self.UNARY_OP_TABLE[type(node.op)]}{self.visit(node.operand, ctx)}'
 
     def visit_ListComp(self, node: ast.ListComp, ctx: JSVisitorContext):
-        ctx.parent = node
-        return f'{self.visit(node.generators, ctx)}'
+        context = ctx.copy()
+        context.parent = node
+        return f'{self.visit(node.generators, context)}'
 
     def visit_DictComp(self, node: ast.DictComp, ctx: JSVisitorContext):
-        "Object.fromEntries([1,2,3].map(n=>[n,1]))"
-        return f'Object.fromEntries({self.visit(node.generators, ctx)})'
+        context = ctx.copy()
+        context.parent = node
+        return f'Object.fromEntries({self.visit(node.generators, context)})'
+
+    def visit_SetComp(self, node: ast.SetComp, ctx: JSVisitorContext):
+        context = ctx.copy()
+        context.parent = node
+        return f'new Set({self.visit(node.generators, context)})'
 
     def visit_comprehension(self, node: ast.comprehension, ctx: JSVisitorContext):
-        builder = Builder(f'{self.visit(node.iter, ctx)}')
-        target = self.visit(node.target, ctx)
-        builder.write_if(node.ifs, (f'.filter({target}=>{self.visit(x, ctx)})' for x in node.ifs))
-
-        if isinstance(ctx.parent, ast.DictComp):
-            builder.write(f'.map(({target})=>[{self.visit(ctx.parent.key, ctx)}, {self.visit(ctx.parent.value, ctx)}])')
-        else:
-            builder.write(f'.map(({target})=>{self.visit(ctx.parent.elt, ctx)})')
-
-        return builder.build()
+        code = [
+            self.visit(node.iter, ctx),
+            node.ifs and [f'.filter({self.visit(node.target, ctx)}=>{self.visit(x, ctx)})' for x in node.ifs],
+            f'.map(({self.visit(node.target, ctx)})=>[{self.visit(ctx.parent.key, ctx)}, {self.visit(ctx.parent.value, ctx)}])'
+            if isinstance(ctx.parent, ast.DictComp) else
+            f'.map(({self.visit(node.target, ctx)})=>{self.visit(ctx.parent.elt, ctx)})',  # type: ignore
+        ]
+        return strinpy.build(code)
+
+    def visit_GeneratorExp(self, node: ast.GeneratorExp, ctx: JSVisitorContext):
+        context = ctx.copy()
+        context.parent = node
+        return self.visit(node.generators, context)
 
     def visit_IfExp(self, node: ast.IfExp, ctx: JSVisitorContext):
         return f'{self.visit(node.test, ctx)} ? {self.visit(node.body, ctx)} : {self.visit(node.orelse, ctx)}'
 
     def visit_Starred(self, node: ast.Starred, ctx: JSVisitorContext):
         return f'...{self.visit(node.value, ctx)}'
 
@@ -396,45 +494,64 @@
         if op_type == ast.FloorDiv:
             return f'(({expr}) >> 0)'
         return f'({expr})'
 
     def visit_AnnAssign(self, node: ast.AnnAssign, ctx: JSVisitorContext):
         if isinstance(node.target, ast.Name):
             ctx.variables.append(node.target.id)
-        return (
-            Builder()
-            .write_if(not isinstance(node.target, ast.Attribute) and ctx.scope != JSScope.CLASS_FIELD, 'let')
-            .write(f'{self.visit(node.target, ctx)}')
-            .write_if(node.value is not None, lambda: f'={self.visit(node.value, ctx)}')
-        ).build()
+        # return (
+        #     Builder()
+        #     .write_if(not isinstance(node.target, ast.Attribute) and ctx.scope != JSScope.CLASS_FIELD, 'let')
+        #     .write(f'{self.visit(node.target, ctx)}')
+        #     .write_if(node.value is not None, lambda: f'={self.visit(node.value, ctx)}')
+        # ).build()
+        return strinpy.build([
+            not isinstance(node.target, ast.Attribute) and ctx.scope != JSScope.CLASS_FIELD and 'let',
+            self.visit(node.target, ctx),
+            node.value is not None and f'={self.visit(node.value, ctx)}',
+        ])
 
     def visit_Pass(self, node: ast.Pass, ctx: JSVisitorContext):
         return '/* pass */'
 
     def visit_With(self, node: ast.With, ctx: JSVisitorContext):
-        builder = SurroundBuilder(surround='{}', separator=';')
-        builder.write(
-            Builder('let')
-            .write(SurroundBuilder(surround='[]', separator=',')
-                   .write(f'__with_{i}' for i, expr in enumerate(node.items)))
-            .write('=')
-            .write(SurroundBuilder(surround='[]', separator=',').write(f'{self.visit(expr.context_expr)}' for expr in node.items))
-        )\
-            .write(Builder(separator=';').write(Builder().write_if(expr.optional_vars, f'{self.visit(expr.optional_vars)}=').write(f'__with_{i}.__enter__()') for i, expr in enumerate(node.items)))\
-            .write(self.visit(node.body))\
-            .write(Builder(separator=';').write(Builder().write_if(expr.optional_vars, f'{self.visit(expr.optional_vars)}=').write(f'__with_{i}.__exit__()') for i, expr in enumerate(node.items)))
-
-        return builder.build()
+        return strinpy.build([
+            '{ let [',
+            [f'__with_{i}' for i, expr in enumerate(node.items)],
+            '] = [',
+            [f'{self.visit(expr.context_expr)}' for expr in node.items],
+            '];',
+            [f'{self.visit(expr.optional_vars)}=__with_{i}.__enter__()' for i, expr in enumerate(node.items)], ';',
+            self.visit(node.body),
+            ';', [f'{self.visit(expr.optional_vars)}=__with_{i}.__exit__()' for i, expr in enumerate(node.items)],
+            '}'
+        ])
+
+    def visit_AsyncWith(self, node: ast.AsyncWith, ctx: JSVisitorContext):
+        return strinpy.build([
+            '{ let [',
+            [f'__with_{i}' for i, expr in enumerate(node.items)],
+            '] = [',
+            [f'{self.visit(expr.context_expr)}' for expr in node.items],
+            '];',
+            [f'{self.visit(expr.optional_vars)}=await __with_{i}.__aenter__()' for i, expr in enumerate(node.items)], ';',
+            self.visit(node.body),
+            ';', [f'await __with_{i}.__aexit__()' for i, expr in enumerate(node.items)],
+            '}'
+        ])
 
     def visit_JoinedStr(self, node: ast.JoinedStr, ctx: JSVisitorContext):
-        context = ctx.copy(scope=JSScope.F_STRING)
-        return '`{}`'.format(''.join(map(lambda item: self.visit(item, context), node.values)))
+        context = ctx.copy(scope=JSScope.JOINED_STR)
+        a = '`{}`'.format(''.join(map(lambda item: self.visit(item, context), node.values)))
+        return a
 
     def visit_FormattedValue(self, node: ast.FormattedValue, ctx: JSVisitorContext):
-        return f'${{{self.visit(node.value, ctx)}}}'
+        context = ctx.copy(scope=JSScope.F_STRING)
+        a = f'${{{self.visit(node.value, context)}}}'
+        return a
 
     def visit_Delete(self, node: ast.Delete, ctx: JSVisitorContext):
         return ';'.join(map(lambda target: f'delete {self.visit(target, ctx)}', node.targets))
 
     def visit_AugAssign(self, node: ast.AugAssign, ctx: JSVisitorContext):
         op_type = type(node.op)
         target = self.visit(node.target, ctx)
@@ -466,87 +583,136 @@
     def visit_Continue(self, node: ast.Continue, ctx: JSVisitorContext):
         return 'continue'
 
     def visit_Assert(self, node: ast.Assert, ctx: JSVisitorContext):
         return f'console.assert({self.visit(node.test, ctx)})'
 
     def visit_Try(self, node: ast.Try, ctx: JSVisitorContext):
-        return (
-            Builder(separator='')
-            .write_if(node.orelse, '__else: {')
-            .write(f'try {{{self.visit(node.body, ctx)}}}')
-            .write_if(node.handlers, "catch(__err) {%s}" % '\n'.join(
-                Builder()
-                .write_if(handler.type, lambda: f'if (__err instanceof {self.visit(handler.type, ctx)})')
-                .write(SurroundBuilder(surround='{}', separator=';')
-                       .write_if(handler.name, f'{handler.name} = __err')
-                       .write(self.visit(handler.body, ctx))
-                       .write_if(node.orelse, 'break __else')
-                       )
-                .build()
-                for handler in node.handlers
-            ))
-            .write_if(node.finalbody, Builder(f'finally {{{self.visit(node.finalbody, ctx)}').write('}'))
-            .write_if(node.orelse, f'{self.visit(node.orelse, ctx)}}}')
-        ).build()
+        code = [
+            node.orelse and '__else: {',
+            'try {',
+            self.visit(node.body, ctx),
+            '}',
+            node.handlers and [
+                'catch(__err) {',
+                [[
+                    handler.type and f'if (__err instanceof {self.visit(handler.type, ctx)})',
+                    # SurroundBuilder(surround='{}', separator=';').write_if(handler.name, f'{handler.name} = __err').write(self.visit(handler.body, ctx)).write_if(node.orelse, 'break __else')
+                    '{',
+                    [
+                        handler.name and f'{handler.name} = __err;',
+                        self.visit(handler.body, ctx),
+                        node.orelse and ';break __else',
+                    ],
+                    '}',
+                ] for handler in node.handlers],
+                '}',
+            ],
+            node.finalbody and [
+                'finally {',
+                self.visit(node.finalbody, ctx),
+                '}',
+            ],
+            node.orelse and [
+                self.visit(node.orelse, ctx),
+                '}',
+            ]
+        ]
+        return strinpy.build(code)
 
     def visit_Match(self, node: ast.Match, ctx: JSVisitorContext):
         return '/*@deprecated match not supported */'
 
     def visit_Global(self, node: ast.Global, ctx: JSVisitorContext):
         ctx.global_variables.extend(node.names)
         return f'var {",".join(node.names)}'
-    
+
     def visit_NoneType(self, null: None, ctx: JSVisitorContext):
         return 'null'
 
 
-space_regex = re.compile('\s+')
+SUPPORTED_TYPES = types.FunctionType | types.ModuleType | Callable
 
 
-def js(func: Optional[Callable] = None, as_function: bool = False, python_compatible: bool = False) -> str:
-    def wrapper(func):
-        lines = inspect.getsourcelines(func)[0]
-
-        if not as_function:
-            while lines:
-                line = lines[0].strip()
-                if line.startswith('@'):
-                    lines.pop(0)
-                elif line.startswith('def'):
-                    lines.pop(0)
-                    break
-                else:
-                    break
+def get_source(source: SUPPORTED_TYPES) -> str:
+    lines = inspect.getsourcelines(source)[0]
 
-        if not lines:
-            return ''
+    if isinstance(source, types.FunctionType):
+        while lines:
+            line = lines[0].strip()
+            if line.startswith('@'):
+                lines.pop(0)
+            elif line.startswith('def'):
+                lines.pop(0)
+                break
+            else:
+                break
 
-        match = space_regex.match(lines[0]).group() if lines[0].startswith(' ') else ''
-        if match:
-            spaces = len(match)
-            lines = list(map(lambda line: line[spaces:], lines))
+    if not lines:
+        return ''
 
-        return convert(''.join(lines), python_compatible=python_compatible)
+    match = re.match(r'\s+', lines[0]) if lines[0].startswith(' ') else ''
+    if match:
+        spaces = len(match.group())
+        lines = list(map(lambda line: line[spaces:], lines))
+
+    return ''.join(lines)
+
+
+def compatible(source: SUPPORTED_TYPES) -> str:
+    return convert(source, compatible=True)
+
+
+def track_imports(target: Path) -> List[Path]:
+    imports = set([target])
+    visited = imports.copy()
+
+    def check_import(path: Path):
+        path = path.resolve()
+        if path in visited:
+            return
+        visited.add(path)
+        if path.exists() and path.is_file():
+            imports.add(path)
+            track_imports(path)
+
+    def track_imports(target: Path):
+        module = ast.parse(target.read_text(encoding='utf-8'))
+        for node in ast.walk(module):
+            if isinstance(node, ast.ImportFrom):
+                if node.module:
+                    path = target.parent / node.module.replace('.', '/')
+                    check_import(path.with_suffix('.py'))
+                    check_import(path / '__init__.py')
+                else:
+                    path = target.parent
+                for alias in node.names:
+                    check_import(
+                        path / ('../' * (node.level - 1)) / f'{alias.name}.py'
+                    )
+            elif isinstance(node, ast.Import):
+                for alias in node.names:
+                    path = target.parent / alias.name.replace('.', '/')
+                    check_import(path.with_suffix('.py'))
+                    check_import(path / '__init__.py')
 
-    if func is None:
-        return wrapper
+    track_imports(target)
 
-    return wrapper(func)
+    return list(imports)
 
 
 def convert(
-    source: Union[str, ast.AST, types.ModuleType, types.FunctionType],
-    formatter: Optional[Callable[[str], str]] = jsbeautifier.beautify,
+    source: Union[str, ast.AST, SUPPORTED_TYPES],
+    formatter: Callable[[str], str] = jsbeautifier.beautify,
     code_gen: Optional[Visitor] = None,
-    python_compatible: bool = False
-):
-    generator = code_gen or CodeGen(python_compatible=python_compatible)
+    compatible: bool = False
+) -> str:
+    generator = code_gen or CodeGen(compatible=compatible)
 
     if isinstance(source, ast.AST):
         parsed = source
     elif isinstance(source, str):
         parsed = ast.parse(source)
     else:
-        parsed = ast.parse(inspect.getsource(source))
+        parsed = ast.parse(get_source(source))
 
     return formatter(generator.visit(parsed))
```

### Comparing `py2js-1.1.8/py2js/visitor.py` & `py2js-1.2.1/py2js/visitor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 import ast
-import functools
 import inspect
 from typing import Callable, Generic, List, Optional, Self, TypeVar, Union
 
 
 class VisitorContext:
     parent: ast.AST
     node: ast.AST
 
 
 T = TypeVar('T', bound=VisitorContext)
 
 
+AST_TYPES = ast.AST | List[ast.AST] | list[ast.stmt] | list[ast.expr] | list[ast.comprehension] | list | filter | tuple | None
+
+
 class VisitorMethod:
-    def __call__(self: Self, node: ast.AST, context: VisitorContext) -> str:
-        pass
+    __name__: str
+
+    def __call__(self: Self, node: AST_TYPES, context: VisitorContext) -> str:
+        raise NotImplementedError
 
 
 class Visitor(Generic[T]):
     def __init__(self, context_factory_or_default: Union[T, Callable[[], T]]) -> None:
         self.create_context = context_factory_or_default if callable(context_factory_or_default) else lambda: context_factory_or_default
+        self.visitors = {}
 
-    @functools.cache
     def get_visitor(self, node) -> Optional[VisitorMethod]:
+        if node.__class__ in self.visitors:
+            return self.visitors[node.__class__]
         field_name: str = 'visit_' + node.__class__.__name__
+        func = None
         if hasattr(self, field_name):
-            return getattr(self, field_name)
+            func = getattr(self, field_name)
         elif hasattr(self, field_name := field_name.lower()):
-            return getattr(self, field_name)
+            func = getattr(self, field_name)
+        if func is None:
+            raise NotImplementedError(f'{node.__class__.__name__} is not implemented.')
+        self.visitors[node.__class__] = func
+        return func
 
-    def transform(self, node: ast.AST, context: Optional[T] = None):
+    def transform(self, node: AST_TYPES, context: Optional[T] = None):
         context = context or self.create_context()
 
         method = self.get_visitor(node)
         if method is None:
             return f"/* {node.__class__.__name__} translator not found. */"
 
         visited = method(node, context)
@@ -41,18 +52,18 @@
             raise ValueError(f'{method.__name__} returned null!\n{inspect.getsourcefile(method)}:{inspect.getsourcelines(method)[1]}')
 
         if isinstance(visited, (list, tuple, map, filter, set)):
             return ';'.join(visited)
         else:
             return visited
 
-    def sperator(self, ast: Union[List[ast.AST], ast.AST], context: Optional[T] = None):
+    def sperator(self, ast: AST_TYPES, context: Optional[T] = None):
         return ';'
 
-    def visit(self, ast: Union[List[ast.AST], ast.AST], context: Optional[T] = None) -> List[str]:
+    def visit(self, ast: AST_TYPES, context: Optional[T] = None) -> str:
         if context is None:
             context = self.create_context()
 
         if not isinstance(ast, (list, tuple, set, map, filter)):
             return self.transform(ast, context=context)
         else:
             return self.sperator(ast, context=context).join(map(lambda x: self.transform(x, context=context), ast))
```

### Comparing `py2js-1.1.8/py2js.egg-info/PKG-INFO` & `py2js-1.2.1/py2js.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: py2js
-Version: 1.1.8
+Version: 1.2.1
 Summary: Write javascript in python with python syntax
 Home-page: https://github.com/am230/py2js
 Author: am230
 Author-email: am.230@outlook.jp
 License: MIT Licence
 Keywords: javascript,convert,translator
 Platform: any
 Requires: jsbeautifier
-Requires: strbuilder
+Requires: strinpy
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Python to Javascript translator
 ===============================
 
 .. image:: https://img.shields.io/github/license/mashape/apistatus.svg
```

### Comparing `py2js-1.1.8/setup.py` & `py2js-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 author = 'am230'
 name = 'py2js'
 py_modules = [name]
 
 setup(
     name=name,
-    version="1.1.8",
-    keywords=("javascript", "convert", "translator"),
+    version="1.2.1",
+    keywords=["javascript", "convert", "translator"],
     description="Write javascript in python with python syntax",
     long_description=long_description,
-    requires=['jsbeautifier', 'strbuilder'],
+    requires=['jsbeautifier', 'strinpy'],
     license="MIT Licence",
     long_description_content_type='text/x-rst',
     packages=find_packages(),
     url=f"https://github.com/{author}/{name}",
     author=author,
     author_email="am.230@outlook.jp",
     py_modules=py_modules,
```

