# Comparing `tmp/click_schema_config-0.1.5.tar.gz` & `tmp/click_schema_config-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_schema_config-0.1.5.tar", max compression
+gzip compressed data, was "click_schema_config-0.2.0.tar", max compression
```

## Comparing `click_schema_config-0.1.5.tar` & `click_schema_config-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rwxr-xr-x   0        0        0     1069 2022-09-29 16:32:25.000000 click_schema_config-0.1.5/LICENSE
--rwxr-xr-x   0        0        0     2738 2023-06-11 10:45:17.093552 click_schema_config-0.1.5/README.md
--rwxr-xr-x   0        0        0      145 2023-06-10 13:51:53.856876 click_schema_config-0.1.5/click_schema_config/__init__.py
--rwxr-xr-x   0        0        0     2477 2023-06-11 12:54:52.091190 click_schema_config-0.1.5/click_schema_config/click.py
--rwxr-xr-x   0        0        0     3259 2023-06-11 12:55:24.787473 click_schema_config-0.1.5/click_schema_config/config.py
--rw-r--r--   0        0        0        0 2023-06-25 09:20:09.658441 click_schema_config-0.1.5/click_schema_config/py.typed
--rw-r--r--   0        0        0      353 2023-06-11 13:01:07.886461 click_schema_config-0.1.5/click_schema_config/types.py
--rwxr-xr-x   0        0        0      476 2023-06-25 10:04:24.790178 click_schema_config-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 click_schema_config-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-12 09:20:50.939061 click_schema_config-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     5255 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/README.md
+-rwxr-xr-x   0        0        0      150 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/__init__.py
+-rwxr-xr-x   0        0        0     2318 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/click.py
+-rw-r--r--   0        0        0     3320 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/commands/codegen.py
+-rw-r--r--   0        0        0       69 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/commands/templates/__init__.py.jinja
+-rw-r--r--   0        0        0      768 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/commands/templates/dataclass.py.jinja
+-rw-r--r--   0        0        0        0 2023-07-12 09:20:50.947061 click_schema_config-0.2.0/click_schema_config/py.typed
+-rwxr-xr-x   0        0        0     3585 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/read_config.py
+-rw-r--r--   0        0        0      408 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/types.py
+-rwxr-xr-x   0        0        0      681 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5844 1970-01-01 00:00:00.000000 click_schema_config-0.2.0/PKG-INFO
```

### Comparing `click_schema_config-0.1.5/LICENSE` & `click_schema_config-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.1.5/click_schema_config/click.py` & `click_schema_config-0.2.0/click_schema_config/click.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Protocol
 from click.decorators import FC
 from .types import FileLike
 
 import builtins
 
 import click
-from .config import read_configs
+from .read_config import read_configs
 
 
 class Decorator(Protocol):
     def __call__(self, func: FC) -> FC:
         ...
 
 
@@ -35,35 +35,31 @@
     if isinstance(files, str):
         files = [files]
 
     config = read_configs(files)
 
     def decorator(func: FC) -> FC:
         # We use reverse-order so that the options are added in the order they appear in the file
-        for section, options in reversed(config.items()):
-            for variable_name, d in reversed(options.items()):
-                option_name = (
-                    f"{f'{section}.' if section != 'DEFAULT' else ''}{variable_name}"
-                )
-
+        for section in reversed(config.values()):
+            for d in reversed(section.values()):
                 type_evalled = d.type
                 if type_evalled is not None:
                     if insecure_eval:
                         try:
                             type_evalled = eval(type_evalled)
                         except Exception:
                             type_evalled = None
                     else:
                         type_evalled = getattr(builtins, type_evalled, None)
 
                 func = click.option(
-                    f"--{option_name}"
+                    f"--{d.option_name}"
                     if type_evalled is not bool
-                    else f"--{option_name}/--no-{option_name}",
-                    option_name.replace(".", "__"),
+                    else f"--{d.option_name}/--no-{d.option_name}",
+                    d.programmatic_name,
                     **(
                         dict(
                             type=type_evalled,
                             default=d.value,
                             required=d.required,
                             help=f"\n{d.description or ''}".replace("\n", "\b\n"),
                             show_default=True,
```

### Comparing `click_schema_config-0.1.5/click_schema_config/config.py` & `click_schema_config-0.2.0/click_schema_config/read_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,32 +16,32 @@
     variable: re.Pattern[str]
 
 
 regexes = Regexes(
     section=re.compile(r"^\[(?P<section>.*)\](#.*)?$"),
     comment=re.compile(r"^[#;]\s?(?P<comment>.*)$"),
     variable=re.compile(
-        r"^(?P<name>\w+)\s*(:\s*(?P<type>\w+))?\s*((?P<not_required>=)\s*(?P<value>.*))?\s*([#;].*)?$"
+        r"^(?P<name>\w+(-\w+)*)\s*(:\s*(?P<type>\w+))?\s*((?P<not_required>=)\s*(?P<value>.*))?\s*([#;].*)?$"
     ),
 )
 
 
 def read_config(config: FileLike, preconfig: Config | None = None) -> Config:
     if isinstance(config, str):
         with open(config) as file:
             return read_config(file, preconfig)
-    result: Config = dict(**(preconfig or {}))
-    result.setdefault("DEFAULT", {})
+    result: Config = (preconfig or {}).copy()
+    result.setdefault(None, {})
 
     @dataclass
     class Current:
-        section: str
+        section: str | None
         description: list[str]
 
-    current = Current(section="DEFAULT", description=[])
+    current = Current(section=None, description=[])
     for i in config:
         match i.strip():
             case "":
                 current.description = []
 
             case i if m := regexes.section.match(i):
                 current.section = m.group("section")
@@ -56,16 +56,22 @@
                 variable_value = ast.literal_eval(m.group("value") or "None")
                 variable_exact_type = m.group("type")
                 variable_inferred_type = variable_exact_type or (
                     typename
                     if (typename := type(variable_value).__name__) != "NoneType"
                     else None
                 )
+
+                option_name = f"{f'{current.section}.' if current.section is not None else ''}{variable_name}"
+                programmatic_name = option_name.replace(".", "__").replace("-", "_")
                 current_variable = result[current.section].get(
-                    variable_name, Variable()
+                    variable_name,
+                    Variable(
+                        option_name=option_name, programmatic_name=programmatic_name
+                    ),
                 )
 
                 result[current.section][variable_name] = dataclasses.replace(
                     current_variable,
                     value=variable_value,
                     required=m.group("not_required") is None,
                     **(
@@ -90,15 +96,15 @@
 
     return result
 
 
 def read_configs(
     filenames: FileLike | list[FileLike], preconfig: Config | None = None
 ) -> Config:
-    result = dict(**(preconfig or {}))
+    result = (preconfig or {}).copy()
     if not isinstance(filenames, list):
         filenames = [filenames]
 
     for file in filenames:
         result = read_config(file, result)
 
     return result
```

