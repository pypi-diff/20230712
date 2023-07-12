# Comparing `tmp/click_schema_config-0.2.1.tar.gz` & `tmp/click_schema_config-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_schema_config-0.2.1.tar", max compression
+gzip compressed data, was "click_schema_config-0.2.2.tar", max compression
```

## Comparing `click_schema_config-0.2.1.tar` & `click_schema_config-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1069 2023-07-12 10:09:59.473612 click_schema_config-0.2.1/LICENSE
--rwxr-xr-x   0        0        0     5255 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/README.md
--rwxr-xr-x   0        0        0      150 2023-07-12 10:09:59.477612 click_schema_config-0.2.1/click_schema_config/__init__.py
--rwxr-xr-x   0        0        0     2318 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/click.py
--rw-r--r--   0        0        0     3320 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/commands/codegen.py
--rw-r--r--   0        0        0       69 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/commands/templates/__init__.py.jinja
--rw-r--r--   0        0        0      768 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/commands/templates/dataclass.py.jinja
--rw-r--r--   0        0        0        0 2023-07-12 10:09:59.473612 click_schema_config-0.2.1/click_schema_config/py.typed
--rwxr-xr-x   0        0        0     3585 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/read_config.py
--rw-r--r--   0        0        0      408 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/types.py
--rwxr-xr-x   0        0        0      698 2023-07-12 10:09:59.485612 click_schema_config-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5883 1970-01-01 00:00:00.000000 click_schema_config-0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-12 10:09:59.473612 click_schema_config-0.2.2/LICENSE
+-rwxr-xr-x   0        0        0     5255 2023-07-12 10:09:59.481612 click_schema_config-0.2.2/README.md
+-rwxr-xr-x   0        0        0      150 2023-07-12 10:09:59.477612 click_schema_config-0.2.2/click_schema_config/__init__.py
+-rwxr-xr-x   0        0        0     2478 2023-07-12 12:58:19.321843 click_schema_config-0.2.2/click_schema_config/click.py
+-rw-r--r--   0        0        0     3344 2023-07-12 12:39:05.946883 click_schema_config-0.2.2/click_schema_config/commands/codegen.py
+-rw-r--r--   0        0        0       69 2023-07-12 10:09:59.481612 click_schema_config-0.2.2/click_schema_config/commands/templates/__init__.py.jinja
+-rw-r--r--   0        0        0      768 2023-07-12 10:09:59.481612 click_schema_config-0.2.2/click_schema_config/commands/templates/dataclass.py.jinja
+-rw-r--r--   0        0        0        0 2023-07-12 10:09:59.473612 click_schema_config-0.2.2/click_schema_config/py.typed
+-rwxr-xr-x   0        0        0     3585 2023-07-12 10:09:59.481612 click_schema_config-0.2.2/click_schema_config/read_config.py
+-rw-r--r--   0        0        0      408 2023-07-12 10:09:59.481612 click_schema_config-0.2.2/click_schema_config/types.py
+-rwxr-xr-x   0        0        0      698 2023-07-12 12:59:35.574299 click_schema_config-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 click_schema_config-0.2.2/PKG-INFO
```

### Comparing `click_schema_config-0.2.1/LICENSE` & `click_schema_config-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.1/README.md` & `click_schema_config-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.1/click_schema_config/click.py` & `click_schema_config-0.2.2/click_schema_config/click.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 __all__ = ["schema_from_inis"]
 
-from typing import Any, Protocol
-from click.decorators import FC
+from _typeshed import IdentityFunction
+from typing import Any, Callable
 from .types import FileLike
 
 import builtins
 
 import click
 from .read_config import read_configs
 
-
-class Decorator(Protocol):
-    def __call__(self, func: FC) -> FC:
-        ...
+FC = Callable[..., Any]
 
 
 def schema_from_inis(
     files: list[FileLike] | FileLike = ["config.default.ini", "config.ini"],
     insecure_eval: bool = False,
     **kwargs: Any,
-) -> Decorator:
+) -> IdentityFunction:
     """Decorate a click command to load options from a config file.
 
     Parameters
     ----------
     filenames : list[FileLike] | files, optional
         List of files (either open file-pointers or filenames) to load, by default ["config.default.ini", "config.ini"]
     insecure_eval : bool, optional
@@ -33,15 +30,15 @@
     """
 
     if isinstance(files, str):
         files = [files]
 
     config = read_configs(files)
 
-    def decorator(func: FC) -> FC:
+    def decorator(func: FC, /) -> FC:
         # We use reverse-order so that the options are added in the order they appear in the file
         for section in reversed(config.values()):
             for d in reversed(section.values()):
                 type_evalled = d.type
                 if type_evalled is not None:
                     if insecure_eval:
                         try:
@@ -53,21 +50,25 @@
 
                 func = click.option(
                     f"--{d.option_name}"
                     if type_evalled is not bool
                     else f"--{d.option_name}/--no-{d.option_name}",
                     d.programmatic_name,
                     **(
-                        dict(
+                        dict(  # type: ignore[arg-type]
                             type=type_evalled,
                             default=d.value,
                             required=d.required,
                             help=f"\n{d.description or ''}".replace("\n", "\b\n"),
                             show_default=True,
                         )
                         | kwargs
                     ),
-                )(func)
+                )(
+                    func  # type: ignore[arg-type]
+                )
 
         return func
 
-    return decorator
+    # Seems to be a mypy bug?
+    # https://github.com/python/mypy/issues/9810
+    return decorator  # type: ignore[return-value]
```

### Comparing `click_schema_config-0.2.1/click_schema_config/commands/codegen.py` & `click_schema_config-0.2.2/click_schema_config/commands/codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import contextlib
 import re
 import typing
 import click
-from halo import Halo
+from halo import Halo  # type: ignore[import]
 
 import pathlib
 import yaml
 from pydantic import BaseModel
 
 import jinja2
```

### Comparing `click_schema_config-0.2.1/click_schema_config/commands/templates/dataclass.py.jinja` & `click_schema_config-0.2.2/click_schema_config/commands/templates/dataclass.py.jinja`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.1/click_schema_config/read_config.py` & `click_schema_config-0.2.2/click_schema_config/read_config.py`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.1/pyproject.toml` & `click_schema_config-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "click-schema-config"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Joy Void Joy <joy.void.joy@gmail.com>"]
 readme = "README.md"
 packages = [{include = "click_schema_config"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.4"
 pyyaml = "^6.0"
 pydantic = "^2.0.2"
 jinja2 = "^3.1.2"
 black = {version = "^22.8.0", allow-prereleases = true}
-types-click = "^7.1.8"
 halo = "^0.0.31"
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.3.0"
+mypy = "^1.4.1"
 ipython = "^8.14.0"
 halo = "^0.0.31"
 types-pyyaml = "^6.0.12.10"
+types-click = "^7.1.8"
 
 [tool.poetry.scripts]
 codegen-ini = "click_schema_config.commands.codegen:codegen"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `click_schema_config-0.2.1/PKG-INFO` & `click_schema_config-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: click-schema-config
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Joy Void Joy
 Author-email: joy.void.joy@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=22.8.0,<23.0.0)
 Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: types-click (>=7.1.8,<8.0.0)
 Description-Content-Type: text/markdown
 
 # click-schema-config
 
 click-schema-config allows you to add settings from a config file. Those will be automatically pulled into your program description without having to repeat them. Comments will be used as helper text for click.
 
 # Is this project necessary?
```

