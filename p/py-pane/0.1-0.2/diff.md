# Comparing `tmp/py-pane-0.1.tar.gz` & `tmp/py-pane-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-pane-0.1.tar", last modified: Sat Jul  8 18:50:37 2023, max compression
+gzip compressed data, was "py-pane-0.2.tar", last modified: Tue Jul 11 22:56:10 2023, max compression
```

## Comparing `py-pane-0.1.tar` & `py-pane-0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-08 18:50:37.141142 py-pane-0.1/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2023-06-16 22:13:24.000000 py-pane-0.1/LICENSE.txt
--rw-r--r--   0 colin      (501) staff       (20)     4162 2023-07-08 18:50:37.141021 py-pane-0.1/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2186 2023-06-16 22:11:09.000000 py-pane-0.1/README.md
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-08 18:50:37.139996 py-pane-0.1/pane/
--rw-r--r--   0 colin      (501) staff       (20)    14873 2023-07-07 20:18:42.000000 py-pane-0.1/pane/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)    19195 2023-07-08 17:27:31.000000 py-pane-0.1/pane/convert.py
--rw-r--r--   0 colin      (501) staff       (20)     5260 2023-06-19 17:59:16.000000 py-pane-0.1/pane/field.py
--rw-r--r--   0 colin      (501) staff       (20)     6763 2023-06-08 19:22:13.000000 py-pane-0.1/pane/sketch.py
--rw-r--r--   0 colin      (501) staff       (20)     3583 2023-07-08 17:25:04.000000 py-pane-0.1/pane/test_converter.py
--rw-r--r--   0 colin      (501) staff       (20)     1132 2023-06-16 15:49:27.000000 py-pane-0.1/pane/test_field.py
--rw-r--r--   0 colin      (501) staff       (20)     1587 2023-06-19 15:52:18.000000 py-pane-0.1/pane/test_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3938 2023-06-19 17:37:20.000000 py-pane-0.1/pane/util.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-08 18:50:37.140594 py-pane-0.1/py_pane.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)     4162 2023-07-08 18:50:37.000000 py-pane-0.1/py_pane.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      344 2023-07-08 18:50:37.000000 py-pane-0.1/py_pane.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-08 18:50:37.000000 py-pane-0.1/py_pane.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)       35 2023-07-08 18:50:37.000000 py-pane-0.1/py_pane.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)        5 2023-07-08 18:50:37.000000 py-pane-0.1/py_pane.egg-info/top_level.txt
--rw-r--r--   0 colin      (501) staff       (20)      996 2023-07-08 18:50:17.000000 py-pane-0.1/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-08 18:50:37.141176 py-pane-0.1/setup.cfg
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-08 18:50:37.140705 py-pane-0.1/tests/
--rw-r--r--   0 colin      (501) staff       (20)     6693 2023-06-19 18:05:11.000000 py-pane-0.1/tests/test_pane.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-11 22:56:10.599717 py-pane-0.2/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2023-06-16 22:13:24.000000 py-pane-0.2/LICENSE.txt
+-rw-r--r--   0 colin      (501) staff       (20)     4182 2023-07-11 22:56:10.599592 py-pane-0.2/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2186 2023-06-16 22:11:09.000000 py-pane-0.2/README.md
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-11 22:56:10.598464 py-pane-0.2/pane/
+-rw-r--r--   0 colin      (501) staff       (20)    16253 2023-07-08 21:41:28.000000 py-pane-0.2/pane/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)    19184 2023-07-08 20:24:00.000000 py-pane-0.2/pane/convert.py
+-rw-r--r--   0 colin      (501) staff       (20)     5260 2023-06-19 17:59:16.000000 py-pane-0.2/pane/field.py
+-rw-r--r--   0 colin      (501) staff       (20)     6763 2023-06-08 19:22:13.000000 py-pane-0.2/pane/sketch.py
+-rw-r--r--   0 colin      (501) staff       (20)     3583 2023-07-08 17:25:04.000000 py-pane-0.2/pane/test_converter.py
+-rw-r--r--   0 colin      (501) staff       (20)     1132 2023-06-16 15:49:27.000000 py-pane-0.2/pane/test_field.py
+-rw-r--r--   0 colin      (501) staff       (20)     1587 2023-06-19 15:52:18.000000 py-pane-0.2/pane/test_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     4075 2023-07-11 21:59:06.000000 py-pane-0.2/pane/util.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-11 22:56:10.599201 py-pane-0.2/py_pane.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)     4182 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      344 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)       56 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)        5 2023-07-11 22:56:10.000000 py-pane-0.2/py_pane.egg-info/top_level.txt
+-rw-r--r--   0 colin      (501) staff       (20)     1060 2023-07-11 22:49:09.000000 py-pane-0.2/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-11 22:56:10.599753 py-pane-0.2/setup.cfg
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-11 22:56:10.599313 py-pane-0.2/tests/
+-rw-r--r--   0 colin      (501) staff       (20)     6847 2023-07-08 19:58:17.000000 py-pane-0.2/tests/test_pane.py
```

### Comparing `py-pane-0.1/LICENSE.txt` & `py-pane-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-pane-0.1/PKG-INFO` & `py-pane-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pane
-Version: 0.1
+Version: 0.2
 Summary: A modern dataclass & data conversion library, focused on speed and expressiveness.
 Author-email: Colin Gilgenbach <hexane@mit.edu>
 License: MIT License
         
         Copyright (c) 2023 Colin Gilgenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 # pane
 
 `pane` is a modern Python library for dataclasses and data conversion, aiming
 for speed and expressiveness.
```

### Comparing `py-pane-0.1/README.md` & `py-pane-0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-pane-0.1/pane/__init__.py` & `py-pane-0.2/pane/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import sys
-from dataclasses import dataclass, KW_ONLY, replace
+from dataclasses import dataclass, KW_ONLY, replace, FrozenInstanceError
 from inspect import Signature, Parameter
 from types import NotImplementedType
 import typing as t
 from typing_extensions import dataclass_transform, Self
 
 from .convert import DataType, IntoData, FromData, from_data, into_data, convert
 from .convert import Converter, make_converter, ConvertError
@@ -15,14 +15,15 @@
 
 
 ClassLayout = t.Literal['tuple', 'struct']
 T = t.TypeVar('T')
 
 
 PANE_FIELDS = '__pane_fields__'
+PANE_SET_FIELDS = '__pane_set__'
 PANE_SPECS = '__pane_specs__'
 PANE_BOUNDVARS = '__pane_boundvars__'
 PANE_OPTS = '__pane_opts__'
 POST_INIT = '__post_init__'
 
 
 @dataclass
@@ -52,14 +53,15 @@
     kw_only_default=False,
     field_specifiers=(FieldSpec, field),
 )
 class PaneBase:
     __pane_opts__: PaneOptions
     __pane_fields__: t.Sequence[Field]
     __pane_specs__: t.Dict[str, FieldSpec]
+    __pane_set__: t.Set[str]
 
     def __init_subclass__(
         cls,
         *args,
         name: t.Optional[str] = None,
         ser_format: t.Optional[ClassLayout] = None,
         de_format: t.Optional[t.Sequence[ClassLayout]] = None,
@@ -114,27 +116,52 @@
         })
         return bound
 
     def __repr__(self) -> str:
         inside = ", ".join(f"{field.name}={getattr(self, field.name)!r}" for field in self.__pane_fields__)
         return f"{self.__class__.__name__}({inside})"
 
+    def __setattr__(self, name: str, value: t.Any) -> None:
+        opts: PaneOptions = getattr(self, PANE_OPTS)
+        if opts.frozen:
+            raise FrozenInstanceError(f"cannot assign to field {name!r}")
+        super().__setattr__(name, value)
+        set_fields: t.Set[str] = getattr(self, PANE_SET_FIELDS)
+        set_fields.add(name)
+
+    def __delattr__(self, name: str, value: t.Any) -> None:
+        raise AttributeError(f"cannot delete field {name!r}")
+
+    @classmethod
+    def _converter(cls: t.Type[T], *args: t.Type[FromData],
+                   annotations: t.Optional[t.Tuple[t.Any, ...]] = None) -> Converter[T]:
+        return t.cast(Converter[T], PaneConverter(cls, annotations))
+
     @classmethod
     def from_data(cls, data: t.Any) -> Self:
-        conv: Converter = getattr(cls, '_converter')()
-        return conv.convert(data)
+        return from_data(data, cls)
 
-    def into_data(self) -> t.Any:
+    def into_data(self) -> DataType:
         opts: PaneOptions = getattr(self, PANE_OPTS)
         if opts.out_format == 'tuple':
             return tuple(into_data(getattr(self, field.name)) for field in getattr(self, PANE_FIELDS))
         elif opts.out_format == 'struct':
             return { field.out_name: into_data(getattr(self, field.name)) for field in getattr(self, PANE_FIELDS) }
         raise ValueError(f"Unknown 'out_format' '{opts.out_format}'")
 
+    def dict(self, set_only: bool = False) -> t.Dict[str, t.Any]:
+        """Return a dict of the fields in `self`."""
+        if set_only:
+            return {
+                k : getattr(self, k) for k in getattr(self, PANE_SET_FIELDS)
+            }
+        return {
+            field.name: getattr(self, field.name) for field in getattr(self, PANE_FIELDS)
+        }
+
     @classmethod
     def from_json(cls, f: FileOrPath) -> Self:
         import json
         with open_file(f) as f:
             obj = json.load(f)
         return cls.from_data(obj)
 
@@ -154,41 +181,51 @@
     def make_unchecked(cls, *args, **kwargs) -> Self:
         ...
 
 
 def _make_init(cls, fields: t.Sequence[Field]):
     params = []
     for field in fields:
+        if field.default is not _MISSING:
+            default = field.default
+        elif field.default_factory is not None:
+            default = field.default_factory()
+        else:
+            default = Parameter.empty
         kind = Parameter.KEYWORD_ONLY if field.kw_only else Parameter.POSITIONAL_OR_KEYWORD
-        default = field.default if field.default is not _MISSING else Parameter.empty
         annotation = field.type if field.type is not _MISSING else Parameter.empty
         params.append(Parameter(field.name, kind, default=default, annotation=annotation))
 
     sig = Signature(params, return_annotation=None)
 
     def __init__(self, *args, **kwargs):
         checked = kwargs.pop('_pane_checked', True)
         try:
             args = sig.bind(*args, **kwargs).arguments
         except TypeError as e:
             raise TypeError(*e.args) from None
 
+        set_fields = set()
+
         for field in t.cast(t.Sequence[Field], getattr(self, PANE_FIELDS)):
             if field.name in args:
                 val = args[field.name]
                 if checked:
                     val = convert(val, field.type)  # type: ignore
+                set_fields.add(field.name)
             elif field.default is not _MISSING:
                 val = field.default
             elif field.default_factory is not None:
                 val = field.default_factory()
             else:
                 raise RuntimeError()
             object.__setattr__(self, field.name, val)
 
+        object.__setattr__(self, PANE_SET_FIELDS, set_fields)
+
         if hasattr(self, POST_INIT):
             getattr(self, POST_INIT)()
 
     __init__.__signature__ = sig
     setattr(cls, '__init__', __init__)
     setattr(cls, '__signature__', sig)
```

### Comparing `py-pane-0.1/pane/convert.py` & `py-pane-0.2/pane/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,23 +441,23 @@
         self.expect = self.expect or self.from_type.__name__
         self.expect_plural = self.expect_plural or self.expect
 
     def expected(self, plural: bool = False) -> str:
         return t.cast(str, self.expect_plural if plural else self.expect)
 
     def try_convert(self, val: t.Any) -> T:
-        val = self.inner.convert(val)
+        val = self.inner.try_convert(val)
         try:
             return self.constructor(val)
         except Exception:
             raise ParseInterrupt from None
 
     def collect_errors(self, val: t.Any) -> t.Optional[ErrorNode]:
         try:
-            val = self.inner.convert(val)
+            val = self.inner.try_convert(val)
         except ParseInterrupt:
             return self.inner.collect_errors(val)
         try:
             self.constructor(val)
         except Exception as e:
             tb = e.__traceback__.tb_next  # type: ignore
             tb = traceback.TracebackException(type(e), e, tb)
@@ -537,15 +537,15 @@
     if not isinstance(val, DataTypes):
         raise TypeError(f"Type {type(val)} is not a valid data interchange type.")
 
     converter = make_converter(ty)
     return converter.convert(val)
 
 
-def convert(val: t.Union[IntoData, DataType], ty: t.Type[T]) -> T:
+def convert(val: IntoData, ty: t.Type[T]) -> T:
     data = into_data(val)
     return from_data(data, ty)
 
 __all__ = [
     'FromData', 'IntoData', 'DataType', 'ConvertError',
     'from_data', 'into_data', 'make_converter', 'convert',
 ]
```

### Comparing `py-pane-0.1/pane/field.py` & `py-pane-0.2/pane/field.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.1/pane/sketch.py` & `py-pane-0.2/pane/sketch.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.1/pane/test_converter.py` & `py-pane-0.2/pane/test_converter.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.1/pane/test_field.py` & `py-pane-0.2/pane/test_field.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.1/pane/test_util.py` & `py-pane-0.2/pane/test_util.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.1/pane/util.py` & `py-pane-0.2/pane/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 import sys
 from pathlib import Path
 from io import TextIOBase, IOBase, TextIOWrapper, BufferedIOBase
 from contextlib import AbstractContextManager, nullcontext
+from collections import OrderedDict
 from itertools import chain
 import typing as t
 
 
 FileOrPath = t.Union[str, Path, TextIOBase, t.TextIO]
 
 
@@ -52,29 +53,29 @@
         return f" {conj} ".join(words)
     return ", ".join(words[:-1]) + f", {conj} {words[-1]}"
 
 
 def _collect_typevars(d, ty):
     if isinstance(ty, type):
         pass
-    elif isinstance(ty, t.Sequence):
+    elif isinstance(ty, (tuple, t.Sequence)):
         for arg in ty:
             _collect_typevars(d, arg)
-    elif hasattr(ty, '__typing_subst__'):
-        d[ty] = None
+    elif hasattr(ty, '__typing_subst__') or isinstance(ty, (t.TypeVar, t.ParamSpec)):
+        d.setdefault(ty)
     else:
         for ty in getattr(ty, '__parameters__', ()):
-            d[ty] = None
+            d.setdefault(ty)
 
 
 def collect_typevars(args) -> tuple[t.Union[t.TypeVar, t.ParamSpec]]:
     # loosely based on typing._collect_parameters
-    d = {}
+    d = {}  # relies on dicts preserving insertion order
     _collect_typevars(d, args)
-    return tuple(d.keys())
+    return tuple(d)
 
 
 def _union_args(ty: t.Type) -> t.Sequence[t.Type]:
     base = t.get_origin(ty) or ty
     args = t.get_args(ty)
 
     if base is t.Union:
@@ -121,8 +122,8 @@
             value = type(None)
         if isinstance(value, str):
             value = t.ForwardRef(value, is_argument=False, is_class=True)
         # private access inside typing.
         value = t._eval_type(value, globalns, localns)  # type: ignore
         d[name] = value
 
-    return d
+    return d
```

### Comparing `py-pane-0.1/py_pane.egg-info/PKG-INFO` & `py-pane-0.2/py_pane.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pane
-Version: 0.1
+Version: 0.2
 Summary: A modern dataclass & data conversion library, focused on speed and expressiveness.
 Author-email: Colin Gilgenbach <hexane@mit.edu>
 License: MIT License
         
         Copyright (c) 2023 Colin Gilgenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 # pane
 
 `pane` is a modern Python library for dataclasses and data conversion, aiming
 for speed and expressiveness.
```

### Comparing `py-pane-0.1/pyproject.toml` & `py-pane-0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=51.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-pane"
-version = "0.1"
+version = "0.2"
 authors = [
 	{name = "Colin Gilgenbach", email = "hexane@mit.edu"},
 ]
 license = {file = "LICENSE.txt"}
 description = "A modern dataclass & data conversion library, focused on speed and expressiveness."
 readme = "README.md"
 keywords = ["dataclass", "validation", "parsing", "conversion"]
@@ -24,14 +24,19 @@
 
 requires-python = ">=3.10"
 dependencies = [
   'PyYAML >= 6.0',
   'typing_extensions ~= 4.5'  # frozen_default
 ]
 
+[project.optional-dependencies]
+dev = [
+  'pytest >= 6.2.4',
+]
+
 [project.urls]
 Repository = "https://github.com/hexane360/pane.git"
 
 [tool.setuptools]
 
 [tool.pyright]
 pythonVersion = "3.10"
```

### Comparing `py-pane-0.1/tests/test_pane.py` & `py-pane-0.2/tests/test_pane.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,25 +32,26 @@
 @pytest.mark.parametrize(('args', 'result'), [
     (f(), {'x': 3, 'y': 5.}),
     (f(4), {'x': 4, 'y': 5.}),
     (f(y=8), {'x': 3, 'y': 8.0}),
 ])
 def test_pane_construction(args, result):
     (args, kwargs) = args
-    assert TestClass(*args, **kwargs).__dict__ == result
+    assert TestClass(*args, **kwargs).dict() == result
 
 
-@pytest.mark.parametrize(('args', 'result'), [
-    (f(), {'x': 3, 'y': 5.}),
-    (f('st'), {'x': 'st', 'y': 5.}),
-    (f(y=None), {'x': 3, 'y': None}),
+@pytest.mark.parametrize(('args', 'result', 'set_only_result'), [
+    (f(), {'x': 3, 'y': 5.}, {}),
+    (f('st'), {'x': 'st', 'y': 5.}, {'x': 'st'}),
+    (f(y=None), {'x': 3, 'y': None}, {'y': None}),
 ])
-def test_pane_unchecked(args, result):
+def test_pane_unchecked(args, result, set_only_result):
     (args, kwargs) = args
-    assert TestClass.make_unchecked(*args, **kwargs).__dict__ == result
+    assert TestClass.make_unchecked(*args, **kwargs).dict() == result
+    assert TestClass.make_unchecked(*args, **kwargs).dict(set_only=True) == set_only_result
 
 
 @pytest.mark.parametrize(('args', 'result'), [
     (f(), "TestClass(x=3, y=5.0)"),
     (f(4), "TestClass(x=4, y=5.0)"),
     (f(y=8), "TestClass(x=3, y=8.0)"),
 ])
```

