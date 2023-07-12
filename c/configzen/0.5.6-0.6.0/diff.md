# Comparing `tmp/configzen-0.5.6.tar.gz` & `tmp/configzen-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.5.6.tar", max compression
+gzip compressed data, was "configzen-0.6.0.tar", max compression
```

## Comparing `configzen-0.5.6.tar` & `configzen-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      536 2023-06-29 17:13:35.607166 configzen-0.5.6/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.5.6/configzen/__main__.py
--rw-r--r--   0        0        0     1681 2023-07-03 13:55:18.269988 configzen-0.5.6/configzen/_isolation.py
--rw-r--r--   0        0        0     3375 2023-07-01 12:22:23.319430 configzen-0.5.6/configzen/_setup.py
--rw-r--r--   0        0        0    78116 2023-07-04 17:12:24.284924 configzen-0.5.6/configzen/config.py
--rw-r--r--   0        0        0     5206 2023-07-04 17:07:03.452372 configzen-0.5.6/configzen/decorators.py
--rw-r--r--   0        0        0     4434 2023-07-03 13:55:18.493989 configzen-0.5.6/configzen/errors.py
--rw-r--r--   0        0        0      491 2023-07-04 19:06:00.928709 configzen-0.5.6/configzen/field.py
--rw-r--r--   0        0        0     6740 2023-07-04 09:58:16.042313 configzen-0.5.6/configzen/interpolation.py
--rw-r--r--   0        0        0    26250 2023-07-03 13:16:45.908317 configzen-0.5.6/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.5.6/configzen/py.typed
--rw-r--r--   0        0        0     4704 2023-07-03 13:21:43.983660 configzen-0.5.6/configzen/route.py
--rw-r--r--   0        0        0     1197 2023-07-03 12:44:27.155689 configzen-0.5.6/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.5.6/LICENSE
--rw-r--r--   0        0        0     1474 2023-07-04 19:06:29.565837 configzen-0.5.6/pyproject.toml
--rw-r--r--   0        0        0    14350 2023-06-29 18:06:31.120725 configzen-0.5.6/README.md
--rw-r--r--   0        0        0    14870 1970-01-01 00:00:00.000000 configzen-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      560 2023-07-12 17:05:42.365663 configzen-0.6.0/configzen/__init__.py
+-rw-r--r--   0        0        0      901 2023-07-06 04:46:24.689646 configzen-0.6.0/configzen/__main__.py
+-rw-r--r--   0        0        0     1677 2023-07-12 16:47:13.813568 configzen-0.6.0/configzen/_detach.py
+-rw-r--r--   0        0        0     3295 2023-07-12 15:49:28.622492 configzen-0.6.0/configzen/_setup.py
+-rw-r--r--   0        0        0     4997 2023-07-06 04:46:31.747498 configzen-0.6.0/configzen/decorators.py
+-rw-r--r--   0        0        0     4294 2023-07-06 04:46:34.678790 configzen-0.6.0/configzen/errors.py
+-rw-r--r--   0        0        0      475 2023-07-06 04:46:37.882744 configzen-0.6.0/configzen/field.py
+-rw-r--r--   0        0        0    14453 2023-07-12 17:06:16.632311 configzen-0.6.0/configzen/interpolation.py
+-rw-r--r--   0        0        0    77237 2023-07-12 17:17:27.067524 configzen-0.6.0/configzen/model.py
+-rw-r--r--   0        0        0     3752 2023-07-12 16:47:14.105134 configzen-0.6.0/configzen/module.py
+-rw-r--r--   0        0        0    25405 2023-07-06 04:46:48.597531 configzen-0.6.0/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.6.0/configzen/py.typed
+-rw-r--r--   0        0        0     4568 2023-07-06 04:47:00.398626 configzen-0.6.0/configzen/route.py
+-rw-r--r--   0        0        0     1160 2023-07-06 04:46:57.057284 configzen-0.6.0/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1683 2023-07-12 17:18:17.998544 configzen-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    14309 2023-07-12 17:20:51.907213 configzen-0.6.0/README.md
+-rw-r--r--   0        0        0    15240 1970-01-01 00:00:00.000000 configzen-0.6.0/PKG-INFO
```

### Comparing `configzen-0.5.6/configzen/__main__.py` & `configzen-0.6.0/configzen/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import argparse
-
-from configzen import ConfigMeta, ConfigModel
-from configzen.config import get_context
-
-
-class Store(ConfigModel):
-    class Config(ConfigMeta):
-        extra = ConfigMeta.Extra.allow
-
-
-if __name__ == "__main__":
-    p = argparse.ArgumentParser()
-    p.add_argument("--source", help="file to load from")
-    p.add_argument("dest", help="file to save into")
-    p.add_argument("--async", dest="use_async", action="store_true", help="use async")
-
-    opt = p.parse_args()
-
-    if opt.use_async:
-        import asyncio
-
-        store = asyncio.run(Store.load_async(opt.source))
-        print(store)
-        context = get_context(store)
-        context.agent.resource = opt.dest
-        asyncio.run(store.save_async())
-    else:
-        store = Store.load(opt.source)
-        print(store)
-        context = get_context(store)
-        context.agent.resource = opt.dest
-        store.save()
+import argparse
+
+from configzen import ConfigMeta, ConfigModel
+from configzen.model import get_context
+
+
+class Store(ConfigModel):
+    class Config(ConfigMeta):
+        extra = ConfigMeta.Extra.allow
+
+
+if __name__ == "__main__":
+    p = argparse.ArgumentParser()
+    p.add_argument("--source", help="file to load from")
+    p.add_argument("dest", help="file to save into")
+    p.add_argument("--async", dest="use_async", action="store_true", help="use async")
+
+    opt = p.parse_args()
+
+    if opt.use_async:
+        import asyncio
+
+        store = asyncio.run(Store.load_async(opt.source))
+        print(store)
+        context = get_context(store)
+        context.agent.resource = opt.dest
+        asyncio.run(store.save_async())
+    else:
+        store = Store.load(opt.source)
+        print(store)
+        context = get_context(store)
+        context.agent.resource = opt.dest
+        store.save()
```

### Comparing `configzen-0.5.6/configzen/_isolation.py` & `configzen-0.6.0/configzen/_detach.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from __future__ import annotations
-
-import asyncio
-import contextvars
-import functools
-from collections.abc import Callable, Coroutine
-from typing import Any, cast
-
-from configzen.typedefs import P, T
-
-
-def isolation_runner(
-    func: Callable[P, T],
-) -> Callable[P, T]:
-    """
-    Decorator to copy a function call context automatically (context isolation)
-    to prevent collisions.
-
-    This decorator will copy the current context and run the function
-    in this new isolated context.
-    """
-    if isinstance(func, (classmethod, staticmethod)):
-        return type(func)(isolation_runner(func.__func__))
-
-    if asyncio.iscoroutinefunction(func):
-
-        @functools.wraps(func)
-        def _isolating_async_wrapper(*args: Any, **kwargs: Any) -> asyncio.Task[T]:
-            return isolate_await(
-                cast(Callable[P, Coroutine[Any, Any, T]], func), *args, **kwargs
-            )
-
-        return cast(Callable[P, T], _isolating_async_wrapper)
-
-    @functools.wraps(func)
-    def _isolating_wrapper(*args: Any, **kwargs: Any) -> T:
-        return isolate_run(func, *args, **kwargs)
-
-    return _isolating_wrapper
-
-
-def isolate_run(
-    func: Callable[..., T],
-    *args: Any,
-    **kwargs: Any,
-) -> T:
-    """Utility for running a function in an isolated context."""
-    context = contextvars.copy_context()
-    return context.run(func, *args, **kwargs)
-
-
-def isolate_await(
-    func: Callable[..., Coroutine[Any, Any, T]],
-    *args: Any,
-    **kwargs: Any,
-) -> asyncio.Task[T]:
-    """Utility for awaiting a coroutine in an isolated context."""
-    return asyncio.create_task(func(*args, **kwargs))
+from __future__ import annotations
+
+import asyncio
+import contextvars
+import functools
+from collections.abc import Callable, Coroutine
+from typing import Any, cast
+
+from configzen.typedefs import P, T
+
+
+def detached_context_function(
+    func: Callable[P, T],
+) -> Callable[P, T]:
+    """
+    Decorator to copy a function call context automatically (context isolation)
+    to prevent collisions.
+
+    This decorator will copy the current context and run the function
+    in this new isolated context.
+    """
+    if isinstance(func, (classmethod, staticmethod)):
+        return type(func)(detached_context_function(func.__func__))
+
+    if asyncio.iscoroutinefunction(func):
+
+        @functools.wraps(func)
+        def _detaching_async_wrapper(*args: Any, **kwargs: Any) -> asyncio.Task[T]:
+            return detached_context_await(
+                cast(Callable[P, Coroutine[Any, Any, T]], func), *args, **kwargs
+            )
+
+        return cast(Callable[P, T], _detaching_async_wrapper)
+
+    @functools.wraps(func)
+    def _detaching_wrapper(*args: Any, **kwargs: Any) -> T:
+        return detached_context_run(func, *args, **kwargs)
+
+    return _detaching_wrapper
+
+
+def detached_context_run(
+    func: Callable[..., T],
+    *args: Any,
+    **kwargs: Any,
+) -> T:
+    """Utility for running a function in an isolated context."""
+    context = contextvars.copy_context()
+    return context.run(func, *args, **kwargs)
+
+
+def detached_context_await(
+    func: Callable[..., Coroutine[Any, Any, T]],
+    *args: Any,
+    **kwargs: Any,
+) -> asyncio.Task[T]:
+    """Utility for awaiting a coroutine in an isolated context."""
+    return asyncio.create_task(func(*args, **kwargs))
```

### Comparing `configzen-0.5.6/configzen/_setup.py` & `configzen-0.6.0/configzen/_setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,128 @@
-"""
-Convenience hooks for quicker development with _configzen_.
-
-For advanced use cases, you can prevent this module from executing
-by setting the environment variable ``CONFIGZEN_SETUP`` to ``0``.
-"""
-
-from __future__ import annotations
-
-import ast
-import ipaddress
-import pathlib
-from collections.abc import Mapping
-from typing import TYPE_CHECKING, Any
-
-from pydantic.json import ENCODERS_BY_TYPE
-
-from configzen.config import ConfigModel, export_hook, field_hook
-
-if TYPE_CHECKING:
-    from configzen.typedefs import ConfigModelT
-
-for obj_type, obj_encoder in ENCODERS_BY_TYPE.items():
-    export_hook.register(obj_type, obj_encoder)
-
-
-@export_hook.register(pathlib.WindowsPath)
-@export_hook.register(pathlib.PureWindowsPath)
-def _export_windows_path(obj: pathlib.WindowsPath | pathlib.PureWindowsPath) -> str:
-    """
-    This hook makes non-absolute paths in configurations cross-platform.
-
-    Parameters
-    ----------
-    obj
-        The path to convert.
-
-    Returns
-    -------
-    The converted path.
-    """
-    return obj.as_posix()
-
-
-@export_hook.register(list)
-def _export_list(obj: list[Any]) -> list[Any]:
-    return [export_hook(item) for item in obj]
-
-
-@export_hook.register(Mapping)
-def _export_mapping(obj: Mapping[Any, Any]) -> dict[Any, Any]:
-    return {k: export_hook(v) for k, v in obj.items()}
-
-
-@field_hook.register(dict)
-@field_hook.register(list)
-def _eval_literals(cls: type[Any], value: Any) -> Any:
-    """
-    Load a dict/list using literal evaluation.
-    Solves nested dictionaries problem in INI files.
-
-    Parameters
-    ----------
-    cls
-        The type to load the value into.
-
-    value
-        The value to load.
-
-    Returns
-    -------
-    The loaded value.
-    """
-    if isinstance(value, str):
-        try:
-            data = ast.literal_eval(value)
-        except (SyntaxError, ValueError):
-            # There might be some following validator, let it be like that
-            return value
-        else:
-            return cls(data)
-    return value
-
-
-@field_hook.register(ipaddress.IPv4Address)
-@field_hook.register(ipaddress.IPv6Address)
-def _eval_ipaddress(
-    cls: type[ipaddress.IPv4Address | ipaddress.IPv6Address], value: Any
-) -> ipaddress.IPv4Address | ipaddress.IPv6Address | Any:
-    if isinstance(value, str) and value.casefold() == "localhost":
-        if issubclass(cls, ipaddress.IPv6Address):
-            return cls("::1")
-        return cls("127.0.0.1")
-    return value
-
-
-@field_hook.register(ConfigModel)
-def _eval_model(cls: type[ConfigModelT], value: Any) -> ConfigModelT | Any:
-    """
-    Load a model using dict literal evaluation.
-    Solves nested dictionaries problem in INI files.
-
-    Parameters
-    ----------
-    cls
-        The type to load the value into.
-
-    value
-        The value to load.
-
-    Returns
-    -------
-    The loaded value.
-    """
-    data = value
-    if isinstance(value, str):
-        try:
-            data = ast.literal_eval(value)
-        except (SyntaxError, ValueError):
-            # Note: Strings resembling models is probably not intended
-            # to be used with automatic pickle/JSON parsing.
-            # return cls.parse_raw(value)
-            return data
-        else:
-            return cls.parse_obj(data)
-    return data
+"""
+Convenience hooks for quicker workflow with _configzen_.
+
+For advanced use cases, you can prevent this module from executing
+by setting the environment variable ``CONFIGZEN_SETUP`` to ``0``.
+"""
+
+from __future__ import annotations
+
+import ast
+import ipaddress
+import pathlib
+from collections.abc import Mapping
+from typing import TYPE_CHECKING, Any
+
+from pydantic.json import ENCODERS_BY_TYPE
+
+from configzen.model import ConfigModel, export_hook, field_hook
+
+if TYPE_CHECKING:
+    from configzen.typedefs import ConfigModelT
+
+for obj_type, obj_encoder in ENCODERS_BY_TYPE.items():
+    export_hook.register(obj_type, obj_encoder)
+
+
+@export_hook.register(pathlib.WindowsPath)
+@export_hook.register(pathlib.PureWindowsPath)
+def _export_windows_path(obj: pathlib.WindowsPath | pathlib.PureWindowsPath) -> str:
+    """
+    This hook makes non-absolute paths in configurations cross-platform.
+
+    Parameters
+    ----------
+    obj
+        The path to convert.
+
+    Returns
+    -------
+    The converted path.
+    """
+    return obj.as_posix()
+
+
+@export_hook.register(list)
+def _export_list(obj: list[Any]) -> list[Any]:
+    return [export_hook(item) for item in obj]
+
+
+@export_hook.register(Mapping)
+def _export_mapping(obj: Mapping[Any, Any]) -> dict[Any, Any]:
+    return {k: export_hook(v) for k, v in obj.items()}
+
+
+@field_hook.register(dict)
+@field_hook.register(list)
+@field_hook.register(set)
+@field_hook.register(tuple)
+def _eval_literals(cls: type[Any], value: Any) -> Any:
+    """
+    Load a value using literal evaluation.
+    Solves nested dictionaries problem in INI files.
+
+    Parameters
+    ----------
+    cls
+        The type to load the value into.
+
+    value
+        The value to load.
+
+    Returns
+    -------
+    The loaded value.
+    """
+    if isinstance(value, str):
+        try:
+            data = ast.literal_eval(value)
+        except (SyntaxError, ValueError):
+            # There might be some following validator, let it be like that
+            return value
+        else:
+            return cls(data)
+    return value
+
+
+@field_hook.register(ipaddress.IPv4Address)
+@field_hook.register(ipaddress.IPv6Address)
+def _eval_ipaddress(
+    cls: type[ipaddress.IPv4Address | ipaddress.IPv6Address], value: Any
+) -> ipaddress.IPv4Address | ipaddress.IPv6Address | Any:
+    if isinstance(value, str) and value.casefold() == "localhost":
+        if issubclass(cls, ipaddress.IPv6Address):
+            return cls("::1")
+        return cls("127.0.0.1")
+    return value
+
+
+@field_hook.register(ConfigModel)
+def _eval_model(cls: type[ConfigModelT], value: Any) -> ConfigModelT | Any:
+    """
+    Load a model using dict literal evaluation.
+    Solves nested dictionaries problem in INI files.
+
+    Parameters
+    ----------
+    cls
+        The type to load the value into.
+
+    value
+        The value to load.
+
+    Returns
+    -------
+    The loaded value.
+    """
+    data = value
+    if isinstance(value, str):
+        try:
+            data = ast.literal_eval(value)
+        except (SyntaxError, ValueError):
+            # Note: Strings resembling models is probably not intended
+            # to be used with automatic pickle/JSON parsing.
+            # return cls.parse_raw(value)
+            return data
+        else:
+            return cls.parse_obj(data)
+    return data
```

### Comparing `configzen-0.5.6/configzen/config.py` & `configzen-0.6.0/configzen/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,2453 +1,2513 @@
-"""
-The main module of the configzen library.
-
-This module provides an API to manage configuration files and resources
-in a consistent way. It also provides tools to load and save configuration
-files in various formats and within a number of advanced methods.
-
-.. code-block:: python
-
-    from configzen import ConfigModel, ConfigField, ConfigMeta
-
-    class DatabaseConfig(ConfigModel):
-        host: str
-        port: int
-        user: str
-        password: str = ConfigField(exclude=True)
-
-        class Config(ConfigMeta):
-            resource = "examples/database.json"
-
-    db_config = DatabaseConfig.load()
-    db_config.host = "newhost"
-    db_config.port = 5432
-
-    db_config.save()
-
-    db_config = DatabaseConfig.load()
-    print(db_config.host)
-    print(db_config.port)
-
-    # Output:
-    # newhost
-    # 5432
-
-    db_config.host = "otherhost"
-    db_config.port = 5433
-
-    db_config.at("host").save()
-
-    print(db_config.host)
-    print(db_config.port)
-
-    # Output:
-    # otherhost
-    # 5432  # <- not 5433, because we saved only host
-
-    db_config.host = "anotherhost"
-    db_config.at("port").reload()
-
-    print(db_config.host)
-    print(db_config.port)
-
-    # Output:
-    # otherhost  # <- not anotherhost, because we reloaded only port
-    # 5432
-"""
-
-from __future__ import annotations
-
-import abc
-import asyncio
-import contextvars
-import copy
-import dataclasses
-import functools
-import importlib
-import io
-import os
-import pathlib
-import urllib.parse
-import urllib.request
-from collections.abc import (
-    Callable,
-    Mapping,
-    Iterator,
-)
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    ClassVar,
-    Generic,
-    Literal,
-    Optional,
-    cast,
-    get_origin,
-    no_type_check,
-    overload,
-)
-
-import anyconfig
-import pydantic
-from anyconfig.utils import filter_options, is_dict_like, is_list_like
-from pydantic.fields import make_generic_validator  # type: ignore[attr-defined]
-from pydantic.fields import ModelField, Undefined
-from pydantic.main import BaseModel, ModelMetaclass
-from pydantic.utils import ROOT_KEY
-
-from configzen._isolation import isolate_run, isolate_await, isolation_runner
-from configzen.errors import (
-    ConfigAccessError,
-    ResourceLookupError,
-    UnavailableParserError,
-    UnspecifiedParserError,
-    InterpolationLookupError,
-    InterpolationError,
-)
-from configzen.interpolation import (
-    NAMESPACE_TOKEN,
-    INTERPOLATOR,
-    BaseInterpolator,
-    include_const,
-    interpolate,
-    include,
-    AT_TOKEN,
-)
-from configzen.processor import EXPORT, DirectiveContext, Processor
-from configzen.route import ConfigRoute
-from configzen.typedefs import (
-    AsyncConfigIO,
-    ConfigIO,
-    ConfigModelT,
-    ConfigRouteLike,
-    IncludeExcludeT,
-    NormalizedResourceT,
-    RawResourceT,
-    T,
-)
-
-try:
-    import aiofiles
-
-    AIOFILES_AVAILABLE = True
-except ImportError:
-    aiofiles = None  # type: ignore[assignment]
-    AIOFILES_AVAILABLE = False
-
-__all__ = (
-    "ConfigAgent",
-    "ConfigAt",
-    "ConfigModel",
-    "ConfigMeta",
-    "export_hook",
-    "field_hook",
-    "export_model",
-    "export_model_async",
-)
-
-ALL_URL_SCHEMES: set[str] = set(
-    urllib.parse.uses_relative + urllib.parse.uses_netloc + urllib.parse.uses_params
-) - {""}
-
-CONTEXT: str = "__context__"
-TOKEN: str = "__context_token__"
-LOCAL: str = "__local__"
-
-INTERPOLATION_TRACKER: str = "__interpolation_tracker__"
-INTERPOLATION_INCLUSIONS: str = "__interpolation_inclusions__"
-
-current_context: contextvars.ContextVar[
-    BaseContext[Any] | None
-] = contextvars.ContextVar("current_context", default=None)
-
-current_interpolation_tracker: contextvars.ContextVar[
-    dict[str, Any] | None
-] = contextvars.ContextVar("current_interpolation_tracker", default=None)
-
-_exporting: contextvars.ContextVar[bool] = contextvars.ContextVar(
-    "_exporting", default=False
-)
-
-
-def _get_defaults_from_model_class(
-    model: type[pydantic.BaseModel],
-) -> dict[str, Any]:
-    defaults = {}
-    for field in model.__fields__.values():
-        default = field.default
-        if not field.field_info.exclude and not field.required:
-            if isinstance(default, pydantic.BaseModel):
-                default = default.dict()
-            defaults[field.alias] = default
-    return defaults
-
-
-def _get_object_state(obj: Any) -> dict[str, Any]:
-    state = obj
-    if not isinstance(obj, dict):
-        state = obj.__dict__  # avoidance of vars() is intended
-    return cast(dict[str, Any], state)
-
-
-@functools.singledispatch
-def export_hook(obj: Any) -> Any:
-    """
-    Convert a value to a format that can be safely serialized.
-
-    This function is used to convert values that are not supported by
-    `anyconfig` to a format that can be safely serialized. It is used
-    internally by `ConfigModel` and `AsyncConfigModel` to convert
-    values before saving them to a file.
-
-    Parameters
-    ----------
-    obj
-        The value to convert.
-
-    Returns
-    -------
-    Any
-    """
-    if dataclasses.is_dataclass(obj):
-        return export_hook(dataclasses.asdict(obj))
-    if isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields"):
-        return _export_namedtuple(obj)
-    return obj
-
-
-@functools.singledispatch
-def _export_namedtuple(obj: tuple[Any, ...]) -> Any:
-    # Initially I wanted it to be export_hook(obj._asdict()), but
-    # pydantic doesn't seem to be friends with custom NamedTuple-s.
-    return export_hook(list(obj))
-
-
-field_hook_registrars: Any = functools.singledispatch(lambda _cls, value: value)
-
-if TYPE_CHECKING:
-
-    class _FieldHookType:
-        def __call__(self, cls: type[T], value: Any) -> Any:
-            ...
-
-        def register(
-            self,
-            cls: type[T],
-            func: Callable[[type[T], Any], Any] | None = None,
-        ) -> Callable[
-            [Callable[[type[T], Any], Any]],
-            Callable[[type[T] | Any, Any], Any],
-        ]:
-            ...
-
-        def dispatch(self, cls: type[T]) -> Callable[[type[T] | Any, Any], Any]:
-            ...
-
-    field_hook: _FieldHookType = _FieldHookType()
-
-else:
-
-    def field_hook(cls: type[Any], value: Any) -> Any:
-        """
-        Automatically registered pre-validator for values in fields
-        where the outer type is `cls`.
-
-        This function is used to load values that are not supported by
-        `anyconfig` to a format that can be used at runtime. It is used
-        by pydantic while performing validation.
-
-        Parameters
-        ----------
-        cls
-            The type to load the value into.
-
-        value
-            The value to load.
-
-        Returns
-        -------
-        The loaded value.
-        """
-        origin = get_origin(cls)
-        try:
-            if isinstance(value, origin or cls):
-                return value
-        except TypeError:
-            return value
-        if origin:
-            cls = origin
-        try:
-            cast_func = field_hook_registrars.dispatch(cls)
-        except KeyError:
-            return value
-        return cast_func(cls, value)
-
-    field_hook.register = field_hook_registrars.register
-
-
-@functools.singledispatch
-def export_model(obj: Any, **kwargs: Any) -> dict[str, Any]:
-    """
-    Export a ConfigModel to a safely-serializable format.
-    Register a custom exporter for a type using the `with_exporter` decorator,
-    which can help to exclude particular values from the export if needed.
-
-    Parameters
-    ----------
-    obj
-    """
-    if isinstance(obj, ConfigModel) and not _exporting.get():
-        return obj.export(**kwargs)
-    return cast(dict[str, Any], obj.dict(**kwargs))
-
-
-@functools.singledispatch
-async def export_model_async(obj: Any, **kwargs: Any) -> dict[str, Any]:
-    """
-    Export a ConfigModel to a safely-serializable format.
-    Register a custom exporter for a type using the `with_exporter` decorator,
-    which can help to exclude particular values from the export if needed.
-
-    Parameters
-    ----------
-    obj
-    """
-    if isinstance(obj, ConfigModel) and not _exporting.get():
-        return await obj.export_async(**kwargs)
-    return cast(dict[str, Any], await obj.dict_async(**kwargs))
-
-
-def _delegate_ac_options(
-    load_options: dict[str, Any], dump_options: dict[str, Any], options: dict[str, Any]
-) -> None:
-    for key, value in options.items():
-        if key.startswith("dump_"):
-            actual_key = key.removeprefix("dump_")
-            targets = [dump_options]
-        elif key.startswith("load_"):
-            actual_key = key.removeprefix("load_")
-            targets = [load_options]
-        else:
-            actual_key = key
-            targets = [load_options, dump_options]
-        for target in targets:
-            if actual_key in target:
-                msg = (
-                    f"Option {key}={value!r} overlaps with "
-                    f"defined {actual_key}={target[actual_key]!r}"
-                )
-                raise ValueError(msg)
-            target[actual_key] = value
-
-
-class ConfigAgent(Generic[ConfigModelT]):
-    """
-    Configuration resource agent: loader and saver.
-
-    This class is used to broke between the model and the home resource, which
-    can be a file, a URL, or a file-like object. It is used internally
-    by `ConfigModel` and `AsyncConfigModel` to load and save
-    configuration files.
-
-    Parameters
-    ----------
-    resource
-        The resource to load the configuration from.
-    processor
-        The resource processor to use. If not specified, the processor used will
-        be :class:`DefaultProcessor`.
-    parser_name
-        The name of the engines to use for loading and saving the
-        configuration. If not specified, the processor will be guessed
-        from the file extension.
-    create_if_missing
-        Whether to create the file if it doesn't exist.
-    use_pydantic_json
-        Whether to use pydantic's JSON serialization for saving the
-        configuration. This is useful for preserving the type of
-        values that are not supported by `anyconfig`.
-    kwargs
-        Additional options to pass to `anyconfig` API functions.
-
-    Attributes
-    ----------
-    create_if_missing
-        Whether to create the file if it doesn't exist.
-    parser_name
-        The name of the engines to use for loading and saving the
-        configuration. If not specified, the processor will be guessed
-        from the file extension.
-    allowed_url_schemes
-        The URL schemes that are allowed to be used.
-
-    Raises
-    ------
-    ValueError
-    """
-
-    processor_class: type[Processor[ConfigModelT]]
-    create_if_missing: bool
-    is_relative: bool = False
-    allowed_url_schemes: set[str]
-    use_pydantic_json: bool = True
-    default_load_options: dict[str, Any] = {}
-    default_dump_options: dict[str, Any] = {
-        # These are usually desirable for configuration files.
-        # If you want to change them, you can do so by monkey-patching
-        # these variables. You can also change `load_options` and
-        # `dump_options` instance attributes to make a local change.
-        "allow_unicode": True,
-        "ensure_ascii": False,
-        "indent": 2,
-    }
-    _resource: NormalizedResourceT
-
-    predefined_default_kwargs: ClassVar[dict[str, Any]] = {"encoding": "UTF-8"}
-    default_allowed_url_schemes: ClassVar[set[str]] = {"file", "http", "https"}
-
-    OPEN_KWARGS: ClassVar[set[str]] = {
-        "mode",
-        "buffering",
-        "encoding",
-        "errors",
-        "newline",
-    }
-    URLOPEN_KWARGS: ClassVar[set[str]] = {
-        "data",
-        "timeout",
-        "cafile",
-        "capath",
-        "cadefault",
-        "context",
-    }
-    JSON_KWARGS: ClassVar[set[str]] = {
-        "skipkeys",
-        "ensure_ascii",
-        "check_circular",
-        "allow_nan",
-        "cls",
-        "indent",
-        "separators",
-        "default",
-        "sort_keys",
-    }
-    EXPORT_KWARGS: ClassVar[set[str]] = {
-        "by_alias",
-        "include",
-        "exclude",
-        "exclude_unset",
-        "exclude_defaults",
-        "exclude_none",
-    }
-    EXTRA_FILE_EXTENSIONS: ClassVar[dict[str, str]] = {
-        "yml": "yaml",
-        "conf": "ini",
-        "cfg": "ini",
-        # Note: CBOR (RFC 7049) is deprecated, use CBOR (RFC 8949) instead.
-        "cbor": "cbor2",
-        # https://github.com/msgpack/msgpack/issues/291#issuecomment-1370526984
-        "mpk": "msgpack",
-        "pkl": "pickle",
-    }
-    BINARY_DATA_PARSERS: ClassVar[set[str]] = {
-        "ion",
-        "bson",
-        "cbor",
-        "cbor2",
-        "msgpack",
-        "pickle",
-    }
-    SUPPORTED_PARSERS: list[str] = anyconfig.list_types()
-
-    def __init__(
-        self,
-        resource: RawResourceT,
-        parser_name: str | None = None,
-        processor_class: type[Processor[ConfigModelT]] | None = None,
-        *,
-        create_if_missing: bool = False,
-        **kwargs: Any,
-    ) -> None:
-        """Parameters
-        ----------
-        resource
-            The URL to the configuration file, or a file-like object.
-        parser_name
-            The name of the anyconfig parser to use
-            for loading and saving the configuration.
-        create_if_missing
-            Whether to automatically create missing keys when loading the configuration.
-        default_kwargs
-            Default keyword arguments to pass while opening the resource.
-        use_pydantic_json
-            Whether to use Pydantic's JSON encoder/decoder instead of the default
-            anyconfig one.
-        uses_binary_data
-            Whether to treat the data as binary.
-            Defaults to True for formats listed in `ConfigAgent.BINARY_DATA_PARSERS`.
-        **kwargs
-            Additional keyword arguments to pass to
-            `anyconfig.loads()` and `anyconfig.dumps()`.
-        """
-        self._parser_name = None
-        self._uses_binary_data = kwargs.get("uses_binary_data", False)
-
-        if processor_class is None:
-            processor_class = Processor[ConfigModelT]
-
-        self.processor_class = processor_class
-        self.parser_name = parser_name
-
-        if isinstance(resource, (str, os.PathLike)) and not (
-            isinstance(resource, str)
-            and urllib.parse.urlparse(str(resource)).scheme in ALL_URL_SCHEMES
-        ):
-            raw_path = os.fspath(resource)
-            resource = pathlib.Path(raw_path)
-            if (
-                raw_path.startswith(".")
-                and resource.parts
-                and not resource.parts[0].startswith(".")
-            ):
-                self.is_relative = True
-
-        self.resource = resource
-        self.create_if_missing = create_if_missing
-        self.use_pydantic_json = kwargs.pop("use_pydantic_json", True)
-        self.default_kwargs = kwargs.pop(
-            "default_kwargs", self.predefined_default_kwargs.copy()
-        )
-        self.allowed_url_schemes = kwargs.pop(
-            "allowed_url_schemes", self.default_allowed_url_schemes.copy()
-        )
-
-        self.load_options = self.default_load_options.copy()
-        self.dump_options = self.default_dump_options.copy()
-
-        _delegate_ac_options(self.load_options, self.dump_options, kwargs)
-
-    @property
-    def resource(self) -> NormalizedResourceT:
-        """
-        The resource of the configuration.
-
-        This can be a file path, a URL, or a file-like object.
-
-        Returns
-        -------
-        The resource of the configuration.
-        """
-        return self._resource
-
-    @resource.setter
-    def resource(self, value: NormalizedResourceT) -> None:
-        """
-        The resource of the configuration.
-
-        This can be a file path, a URL, or a file-like object.
-
-        .. note::
-            If the resource is a file path, the processor will be guessed
-            from the file extension.
-
-        Returns
-        -------
-        The resource of the configuration.
-        """
-        self._resource = value
-        if self.parser_name is None:
-            self.parser_name = self._guess_parser_name()
-
-    @property
-    def parser_name(self) -> str | None:
-        return self._parser_name
-
-    @parser_name.setter
-    def parser_name(self, value: str | None) -> None:
-        if value is not None:
-            value = value.casefold()
-        self._parser_name = value
-
-    def _guess_parser_name(self) -> str | None:
-        parser_name = None
-        if isinstance(self.resource, pathlib.Path):
-            suffix = self.resource.suffix[1:].casefold()
-            supported_parsers = self.SUPPORTED_PARSERS
-            if not suffix:
-                recognized_file_extensions = supported_parsers + [
-                    alias + "(-> " + actual_parser_name + ")"
-                    for alias, actual_parser_name in self.EXTRA_FILE_EXTENSIONS.items()
-                    if actual_parser_name in supported_parsers
-                ]
-                msg = (
-                    "Could not guess the anyconfig parser to use for "
-                    f"{self.resource!r}.\n"
-                    f"Recognized file extensions: {recognized_file_extensions}"
-                )
-                raise UnspecifiedParserError(msg)
-            parser_name = self.EXTRA_FILE_EXTENSIONS.get(suffix, suffix)
-            if (
-                parser_name == "cbor2"
-                and "cbor2" not in supported_parsers
-                and "cbor" in supported_parsers
-            ):
-                parser_name = "cbor"
-        return parser_name
-
-    def load_into(
-        self,
-        config_class: type[ConfigModelT],
-        blob: str | bytes,
-        parser_name: str | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Load the configuration into a `ConfigModel` subclass.
-
-        Parameters
-        ----------
-        config_class
-            The `ConfigModel` subclass to load the configuration into.
-        blob
-            The configuration to load.
-        parser_name
-            The name of the engines to use for loading the configuration.
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.loads()`.
-
-        Returns
-        -------
-        The loaded configuration.
-        """
-        dict_config = self.load_dict(blob, parser_name=parser_name, **kwargs)
-        if dict_config is None:
-            dict_config = {}
-        return config_class.parse_obj(dict_config)
-
-    async def async_load_into(
-        self,
-        config_class: type[ConfigModelT],
-        blob: str | bytes,
-        parser_name: str | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Load the configuration into a `ConfigModel` subclass asynchronously.
-
-        Parameters
-        ----------
-        config_class
-            The `ConfigModel` subclass to load the configuration into.
-        blob
-            The configuration to load.
-        parser_name
-            The name of the engines to use for loading the configuration.
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.loads()`.
-
-        Returns
-        -------
-        The loaded configuration.
-        """
-        dict_config = await self.load_dict_async(
-            blob, parser_name=parser_name, **kwargs
-        )
-        if dict_config is None:
-            dict_config = {}
-        return config_class.parse_obj(dict_config)
-
-    def _load_dict_impl(
-        self,
-        blob: str | bytes,
-        parser_name: str | None = None,
-        **kwargs: Any,
-    ) -> dict[str, Any]:
-        parser_name = parser_name or self.parser_name or self._guess_parser_name()
-        if parser_name is None:
-            msg = "Cannot read configuration because `parser_name` was not specified"
-            raise UnspecifiedParserError(msg)
-        kwargs = self.load_options | kwargs
-        try:
-            loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
-                blob, ac_parser=parser_name, **kwargs
-            )
-        except anyconfig.UnknownParserTypeError as exc:
-            raise UnavailableParserError(str(exc).split()[-1], self) from exc
-        if not isinstance(loaded, Mapping):
-            msg = (
-                f"Expected a mapping as a result of loading {self.resource}, "
-                f"got {type(loaded).__name__}."
-            )
-            raise TypeError(msg)
-        return dict(loaded)
-
-    def load_dict(
-        self,
-        blob: str | bytes,
-        parser_name: str | None = None,
-        *,
-        preprocess: bool = True,
-        **kwargs: Any,
-    ) -> dict[str, Any]:
-        """
-        Load the configuration into a dictionary. The dictionary is
-        usually used to initialize a `ConfigModel` subclass. If the
-        configuration is empty, None might be returned instead of a dictionary.
-
-        Parameters
-        ----------
-        blob
-            The configuration to load.
-        parser_name
-            The name of the anyconfig parser to use for loading the configuration.
-        preprocess
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.loads()`.
-
-        Returns
-        -------
-        The loaded configuration dictionary.
-        """
-        loaded = self._load_dict_impl(blob, parser_name=parser_name, **kwargs)
-        if preprocess:
-            loaded = self.processor_class(self, loaded).preprocess()
-        return loaded
-
-    async def load_dict_async(
-        self,
-        blob: str | bytes,
-        parser_name: str | None = None,
-        *,
-        preprocess: bool = True,
-        **kwargs: Any,
-    ) -> dict[str, Any]:
-        """
-        Load the configuration into a dictionary asynchronously.
-
-        Parameters
-        ----------
-        blob
-            The configuration to load.
-        parser_name
-            The name of the anyconfig parser to use for loading the configuration.
-        preprocess
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.loads()`.
-
-        Returns
-        -------
-        The loaded configuration dictionary.
-        """
-        loaded = self._load_dict_impl(blob, parser_name, **kwargs)
-        if preprocess:
-            loaded = await self.processor_class(self, loaded).preprocess_async()
-        return loaded
-
-    def dump_config(
-        self,
-        config: ConfigModelT,
-        parser_name: str | None = None,
-        **kwargs: Any,
-    ) -> str:
-        """
-        Dump the configuration to a string.
-
-        Parameters
-        ----------
-        config
-            The configuration to dump.
-        parser_name
-            The name of the anyconfig parser to use for saving the configuration.
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.dumps()`.
-
-        Returns
-        -------
-        The dumped configuration.
-        """
-        if parser_name is None:
-            parser_name = self.parser_name
-        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
-        if parser_name == "json" and self.use_pydantic_json:
-            export_kwargs |= filter_options(
-                self.JSON_KWARGS, self.dump_options | kwargs
-            )
-            _exporting.set(True)  # noqa: FBT003
-            return isolate_run(config.json, **export_kwargs)
-        data = export_model(config, **export_kwargs)
-        return self.dump_data(data, parser_name=parser_name, **kwargs)
-
-    async def dump_config_async(
-        self,
-        config: ConfigModelT,
-        parser_name: str | None = None,
-        **kwargs: Any,
-    ) -> str:
-        """
-        Dump the configuration to a string.
-
-        Parameters
-        ----------
-        config
-            The configuration to dump.
-        parser_name
-            The name of the anyconfig parser to use for saving the configuration.
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.dumps()`.
-
-        Returns
-        -------
-        The dumped configuration.
-        """
-        if parser_name is None:
-            parser_name = self.parser_name
-        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
-        if parser_name == "json" and self.use_pydantic_json:
-            export_kwargs |= filter_options(
-                self.JSON_KWARGS, self.dump_options | kwargs
-            )
-            _exporting.set(True)  # noqa: FBT003
-            return await isolate_await(config.json_async, **export_kwargs)
-        data = await export_model_async(config, **export_kwargs)
-        return self.dump_data(data, parser_name=parser_name, **kwargs)
-
-    def dump_data(
-        self,
-        data: dict[str, Any],
-        parser_name: str | None = None,
-        **kwargs: Any,
-    ) -> str:
-        """
-        Dump data to a string.
-
-        Parameters
-        ----------
-        data
-            The data to dump.
-        parser_name
-            The name of the anyconfig parser to use for saving the configuration.
-        kwargs
-            Additional keyword arguments to pass to `anyconfig.dumps()`.
-
-        Returns
-        -------
-        The dumped configuration.
-        """
-        if parser_name is None:
-            parser_name = self.parser_name
-        if parser_name is None:
-            msg = (
-                "Cannot write configuration because `parser_name` was not specified"
-                f"for agent {self}"
-            )
-            raise UnspecifiedParserError(msg)
-        kwargs = self.dump_options | kwargs
-        return anyconfig.dumps(export_hook(data), ac_parser=parser_name, **kwargs)
-
-    @property
-    def is_url(self) -> bool:
-        """
-        Whether the resource is a URL.
-
-        This simply checks if the resource object is a string, since local paths
-        are converted into `pathlib.Path` objects.
-        """
-        return isinstance(self.resource, str)
-
-    @property
-    def uses_binary_data(self) -> bool:
-        """
-        Whether the resource uses bytes for storing data, not str.
-        """
-        return self._uses_binary_data or self.parser_name in self.BINARY_DATA_PARSERS
-
-    def open_resource(self, **kwds: Any) -> ConfigIO:
-        """
-        Open the configuration file.
-
-        Parameters
-        ----------
-        **kwds
-            Keyword arguments to pass to the opening routine.
-            For URLs, these are passed to ``urllib.request.urllib.request.urlopen()``.
-            For local files, these are passed to ``builtins.open()``.
-
-        Returns
-        -------
-        The opened resource.
-        """
-        if self.resource is None:
-            if self.uses_binary_data:
-                return io.BytesIO()
-            return io.StringIO()
-        if self.is_url:
-            url = urllib.parse.urlparse(cast(str, self.resource))
-            if url.scheme not in self.allowed_url_schemes:
-                msg = (
-                    f"URL scheme {url.scheme!r} is not allowed, "
-                    f"must be one of {self.allowed_url_schemes!r}"
-                )
-                raise ValueError(msg)
-            kwds = filter_options(self.URLOPEN_KWARGS, kwds)
-            request = urllib.request.Request(url.geturl())
-            return cast(ConfigIO, urllib.request.urlopen(request, **kwds))  # noqa: S310
-        if isinstance(self.resource, (int, pathlib.Path)):
-            kwds = filter_options(self.OPEN_KWARGS, kwds)
-            if isinstance(self.resource, int):
-                return cast(
-                    ConfigIO,
-                    # We intentionally do not use the context manager here
-                    # because we do not want to close the file.
-                    # Moreover, we want to allow the file to be opened
-                    # from a file descriptor, not supported by Path().
-                    open(self.resource, **kwds),  # noqa: PTH123, SIM115
-                )
-            return cast(ConfigIO, pathlib.Path(self.resource).open(**kwds))
-        return cast(ConfigIO, self.resource)
-
-    def open_resource_async(self, **kwds: Any) -> AsyncConfigIO:
-        """
-        Open the configuration file asynchronously.
-
-        Parameters
-        ----------
-        **kwds
-            Keyword arguments to pass to the opening routine.
-
-        Returns
-        -------
-        The opened resource.
-        """
-        if self.is_url:
-            msg = "Asynchronous URL opening is not supported"
-            raise NotImplementedError(msg)
-        if not AIOFILES_AVAILABLE:
-            msg = (
-                "Aiofiles is not available, cannot open file "
-                "asynchronously (install with `pip install aiofiles`)"
-            )
-            raise RuntimeError(msg)
-        if isinstance(self.resource, (int, pathlib.Path)):
-            kwds = filter_options(self.OPEN_KWARGS, kwds)
-            return aiofiles.open(self.resource, **kwds)
-        raise RuntimeError("cannot open resource asynchronously")
-
-    def processor_open_resource(self, **kwargs: Any) -> ConfigIO:
-        """
-        Called by the processor to open a configuration resource
-        with the reading intention.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the opening routine.
-            For URLs, these are passed to ``urllib.request.urlopen()``.
-            For local files, these are passed to ``builtins.open()``.
-
-        Returns
-        -------
-        The opened resource.
-        """
-        kwargs = self._get_default_kwargs("read", kwargs)
-        return self.open_resource(**kwargs)
-
-    def processor_open_resource_async(self, **kwargs: Any) -> AsyncConfigIO:
-        """
-        Called by the processor to open a configuration resource asynchronously
-        with the reading intention.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the opening routine.
-            For URLs, these are passed to ``urllib.request.urlopen()``.
-            For local files, these are passed to ``builtins.open()``.
-
-        Returns
-        -------
-        The opened resource.
-        """
-        kwargs = self._get_default_kwargs("read", kwargs)
-        return self.open_resource_async(**kwargs)
-
-    def _get_default_kwargs(
-        self,
-        method: Literal["read", "write"],
-        kwargs: dict[str, Any] | None = None,
-    ) -> dict[str, Any]:
-        if not kwargs:
-            kwargs = self.default_kwargs
-        new_kwargs = cast(dict[str, Any], kwargs).copy()
-        if not self.is_url:
-            if method == "read":
-                new_kwargs.setdefault("mode", "rb" if self.uses_binary_data else "r")
-            elif method == "write":
-                new_kwargs.setdefault("mode", "wb" if self.uses_binary_data else "w")
-            else:
-                msg = f"Invalid resource access method: {method!r}"
-                raise ValueError(msg)
-        if self.uses_binary_data:
-            new_kwargs.pop("encoding", None)
-        return new_kwargs
-
-    def read(
-        self,
-        *,
-        config_class: type[ConfigModelT],
-        create_kwargs: dict[str, Any] | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Read the configuration file.
-
-        Parameters
-        ----------
-        config_class
-            The configuration model class to load the configuration into.
-        create_kwargs
-            Keyword arguments to pass to the open method
-            when optionally creating the file.
-        **kwargs
-            Keyword arguments to pass to the open method.
-
-        Returns
-        -------
-        The loaded configuration.
-        """
-        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
-        try:
-            with self.open_resource(**kwargs) as fp:
-                blob = fp.read()
-        except FileNotFoundError:
-            if self.create_if_missing:
-                defaults = _get_defaults_from_model_class(config_class)
-                blob = self.dump_data(defaults)
-                self.write(blob, **(create_kwargs or {}))
-            else:
-                raise
-        return self.load_into(config_class, blob, **self.load_options)
-
-    def write(self, blob: str | bytes, **kwargs: Any) -> int:
-        """
-        Write the configuration file.
-
-        Parameters
-        ----------
-        blob
-            The string/bytes to write into the resource.
-        kwargs
-            Keyword arguments to pass to the opening routine.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
-        with self.open_resource(**kwargs) as fp:
-            return fp.write(cast(str, blob))
-
-    async def read_async(
-        self,
-        *,
-        config_class: type[ConfigModelT],
-        create_kwargs: dict[str, Any] | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Read the configuration file asynchronously.
-
-        Parameters
-        ----------
-        config_class
-            The configuration model class to load the configuration into.
-        create_kwargs
-            Keyword arguments to pass to the open method
-            when optionally creating the file.
-        **kwargs
-            Keyword arguments to pass to the open method.
-
-        Returns
-        -------
-        The loaded configuration.
-        """
-        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
-        try:
-            async with self.open_resource_async(**kwargs) as fp:
-                blob = await fp.read()
-        except FileNotFoundError:
-            if self.create_if_missing:
-                defaults = _get_defaults_from_model_class(config_class)
-                blob = self.dump_data(defaults)
-                await self.write_async(blob, **(create_kwargs or {}))
-        return await self.async_load_into(config_class, blob, **self.load_options)
-
-    async def write_async(
-        self,
-        blob: str | bytes,
-        **kwargs: Any,
-    ) -> int:
-        """
-        Write the configuration file asynchronously.
-
-        Parameters
-        ----------
-        blob
-            The string/bytes to write into the resource.
-        kwargs
-            Keyword arguments to pass to the opening routine.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
-        async with self.open_resource_async(**kwargs) as fp:
-            # Technically those might be also bytes,
-            # todo(bswck): type hint it properly...
-            return await fp.write(cast(str, blob))
-
-    @classmethod
-    def from_directive_context(
-        cls,
-        ctx: DirectiveContext,
-        /,
-        route_separator: str = ":",
-        route_class: type[ConfigRoute] | None = None,
-    ) -> tuple[ConfigAgent[ConfigModelT], ConfigRouteLike | None]:
-        """
-        Create a configuration agent from a preprocessor directive context.
-        Return an optional scope that the context points to.
-
-        Parameters
-        ----------
-        route_class
-        route_separator
-        ctx
-
-        Returns
-        -------
-        The configuration agent.
-        """
-        if route_class is None:
-            route_class = ConfigRoute
-        route: ConfigRouteLike | None = None
-        args: list[Any] = []
-        kwargs: dict[str, Any] = {}
-        if isinstance(ctx.snippet, str):
-            path, _, route = ctx.snippet.partition(route_separator)
-            route = ConfigRoute(
-                route.strip().replace(route_separator, route_class.TOK_DOT)
-            )
-            args.append(path)
-        elif isinstance(ctx.snippet, int):
-            args.append(ctx.snippet)
-        elif is_dict_like(ctx.snippet):
-            kwargs |= ctx.snippet
-        elif is_list_like(ctx.snippet):
-            args += list(ctx.snippet)
-        else:
-            msg = (
-                f"Invalid snippet for the {ctx.directive!r} directive: {ctx.snippet!r}"
-            )
-            raise ValueError(msg)
-        return cls(*args, **kwargs), str(route)
-
-    @classmethod
-    def register_file_extension(
-        cls,
-        file_extension: str,
-        *,
-        parser_name: str,
-    ) -> None:
-        """
-        Register a file extension with the proper anyconfig parser to use.
-
-        Parameters
-        ----------
-        file_extension
-        parser_name
-
-        Returns
-        -------
-        """
-        cls.EXTRA_FILE_EXTENSIONS[file_extension] = parser_name
-
-    def __repr__(self) -> str:
-        resource = self.resource
-        return f"{type(self).__name__}({resource=!r})"
-
-
-def at(
-    mapping: Any,
-    route: ConfigRouteLike,
-    converter_func: Callable[[Any], dict[str, Any]] = _get_object_state,
-    agent: ConfigAgent[ConfigModelT] | None = None,
-) -> Any:
-    """
-    Get an item at a route.
-
-    Parameters
-    ----------
-    mapping
-        The mapping to use.
-    route
-        The route to the item.
-    converter_func
-    agent
-
-    Returns
-    -------
-    The item at the route.
-    """
-    route = ConfigRoute(route)
-    route_here = []
-    scope = _get_object_state(mapping)
-    try:
-        for part in route:
-            route_here.append(part)
-            scope = converter_func(scope)[part]
-    except KeyError:
-        raise ResourceLookupError(agent, route_here) from None
-    return scope
-
-
-@dataclasses.dataclass(frozen=True)
-class ConfigAt(Generic[ConfigModelT]):
-    """
-    A configuration item at a specific location.
-
-    Attributes
-    ----------
-    owner
-        The configuration model instance.
-    mapping
-        The mapping to use.
-    route
-        The route to the item.
-    """
-
-    owner: ConfigModelT
-    mapping: dict[str, Any] | None
-    route: ConfigRouteLike
-
-    def get(
-        self, route: ConfigRouteLike | None = None, default: Any = Undefined
-    ) -> Any:
-        """
-        Get the value of the item.
-
-        Parameters
-        ----------
-        route
-            The route to the item. If not given, the sole route of this item is used.
-            If given, the route is appended to the sole route of this item.
-        default
-            The default value to return if the item is not found.
-
-        Returns
-        -------
-        The value of the item.
-        """
-        base_route = ConfigRoute(self.route)
-        if route is None:
-            route = base_route
-        else:
-            route = base_route.enter(ConfigRoute(route, allow_empty=True))
-        try:
-            scope = at(self.mapping or self.owner, route)
-        except ResourceLookupError as err:
-            if default is Undefined:
-                route_here = err.route
-                raise ConfigAccessError(self.owner, route_here) from None
-            scope = default
-        return scope
-
-    def update(self, value: Any) -> Any:
-        """
-        Update the value of the item with regard to this item mapping.
-
-        Parameters
-        ----------
-        value
-            The new value.
-
-        Returns
-        -------
-        The updated mapping.
-        """
-        route = list(ConfigRoute(self.route))
-        mapping = self.mapping or self.owner
-        key = route.pop()
-        scope = _get_object_state(mapping)
-        route_here = []
-        try:
-            for part in route:
-                route_here.append(part)
-                scope = _get_object_state(scope[part])
-            scope[key] = value
-        except KeyError:
-            raise ConfigAccessError(self.owner, route_here) from None
-        return mapping
-
-    async def save_async(self, **kwargs: Any) -> int:
-        """
-        Save the configuration asynchronously.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the saving function.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        return await _save_async(self, **kwargs)
-
-    def save(self, **kwargs: Any) -> int:
-        """
-        Save the configuration.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the saving function.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        return _save(self, **kwargs)
-
-    async def reload_async(self, **kwargs: Any) -> Any:
-        """
-        Reload the configuration asynchronously.
-
-        Parameters
-        ----------
-        kwargs
-            Keyword arguments to pass to the reloading function.
-
-        Returns
-        -------
-        The reloaded configuration or its belonging item.
-        """
-        return await _reload_async(self, **kwargs)
-
-    def reload(self, **kwargs: Any) -> Any:
-        """
-        Reload the configuration.
-
-        Parameters
-        ----------
-        kwargs
-            Keyword arguments to pass to the reloading function.
-
-        Returns
-        -------
-        The reloaded configuration or its belonging item.
-        """
-        return _reload(self, **kwargs)
-
-
-def _save(
-    section: ConfigModelT | ConfigAt[ConfigModelT],
-    write_kwargs: dict[str, Any] | None = None,
-    **kwargs: Any,
-) -> int:
-    if isinstance(section, ConfigModel):
-        config = section
-        return config.save(write_kwargs=write_kwargs, **kwargs)
-
-    if write_kwargs is None:
-        write_kwargs = {}
-
-    config = section.owner
-    data = config.initial_state
-    scope = ConfigAt(config, data, section.route)
-    data = scope.update(section.get())
-    context = get_context(config)
-    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
-    result = config.write(blob, **write_kwargs)
-    context.initial_state = data
-    return result
-
-
-async def _save_async(
-    section: ConfigModelT | ConfigAt[ConfigModelT],
-    write_kwargs: dict[str, Any] | None = None,
-    **kwargs: Any,
-) -> int:
-    if isinstance(section, ConfigModel):
-        config = section
-        return await config.save_async(write_kwargs=write_kwargs, **kwargs)
-
-    if write_kwargs is None:
-        write_kwargs = {}
-
-    config = section.owner
-    data = config.initial_state
-    scope = ConfigAt(config, data, section.route)
-    data = scope.update(section.get())
-    context = get_context(config)
-    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
-    result = await config.write_async(blob, **write_kwargs)
-    context.initial_state = data
-    return result
-
-
-def _reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
-    if isinstance(section, ConfigModel):
-        config = section
-        return config.reload()
-
-    config = section.owner
-    context = get_context(config)
-    state = config.__dict__
-    newest = context.agent.read(config_class=type(config), **kwargs)
-    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
-    ConfigAt(config, state, section.route).update(section_data)
-    return section_data
-
-
-async def _reload_async(
-    section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any
-) -> Any:
-    if isinstance(section, ConfigModel):
-        config = section
-        return await config.reload_async()
-
-    config = section.owner
-    context = get_context(config)
-    state = config.__dict__
-    newest = await context.agent.read_async(config_class=type(config), **kwargs)
-    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
-    ConfigAt(config, state, section.route).update(section_data)
-    return section_data
-
-
-class BaseContext(abc.ABC, Generic[ConfigModelT]):
-    """
-    The base class for configuration context.
-    Contexts are used to
-    - store configuration resource information,
-    - link configuration items to the configuration models they belong to,
-    - keep track of the route leading to particular configuration
-      items that are also ConfigModel subclasses.
-
-    Attributes
-    ----------
-    initial_state
-        The initial configuration state.
-
-    """
-
-    initial_state: dict[str, Any]
-    interpolation_namespace: dict[str, Any]
-
-    @abc.abstractmethod
-    def trace_route(self) -> Iterator[str]:
-        """Trace the route to where the configuration subcontext points to."""
-
-    @property
-    def route(self) -> ConfigRoute:
-        """The route to where the configuration subcontext points to."""
-        return ConfigRoute(list(self.trace_route()))
-
-    @overload
-    def enter(self: BaseContext[ConfigModelT], part: None) -> BaseContext[ConfigModelT]:
-        ...
-
-    @overload
-    def enter(self, part: str) -> Subcontext[ConfigModelT]:
-        ...
-
-    def enter(
-        self, part: str | None
-    ) -> Subcontext[ConfigModelT] | BaseContext[ConfigModelT]:
-        """
-        Enter a subcontext.
-
-        Parameters
-        ----------
-        part
-            The name of the item nested in the item this context points to.
-
-        Returns
-        -------
-        The new subcontext.
-        """
-        if part is None:
-            return self
-        return Subcontext(self, part, self.interpolation_namespace.setdefault(part, {}))
-
-    @property
-    @abc.abstractmethod
-    def agent(self) -> ConfigAgent[ConfigModelT]:
-        """The configuration agent responsible for loading and saving."""
-
-    @property
-    @abc.abstractmethod
-    def toplevel_interpolation_namespace(self) -> dict[str, Any]:
-        """Top-level interpolation namespace."""
-
-    @property
-    @abc.abstractmethod
-    def owner(self) -> ConfigModelT | None:
-        """
-        The top-level configuration model instance,
-        holding all adjacent contexts.
-        """
-
-    @property
-    @abc.abstractmethod
-    def at(self) -> ConfigModelT | ConfigAt[ConfigModelT] | None:
-        """
-        The configuration model instance or the configuration item
-        this context points to.
-        """
-
-
-class Context(BaseContext[ConfigModelT], Generic[ConfigModelT]):
-    """
-    The context of a configuration model.
-
-    Parameters
-    ----------
-    agent
-        The configuration resource agent.
-    owner
-        The top-level configuration model instance,
-        holding all belonging subcontexts.
-    """
-
-    _initial_state: dict[str, Any]
-
-    def __init__(
-        self,
-        agent: ConfigAgent[ConfigModelT],
-        owner: ConfigModelT | None = None,
-    ) -> None:
-        self._initial_state = {}
-        self._owner = None
-        self._agent = agent
-        self.interpolation_namespace = {}
-        self.owner = owner
-
-    def trace_route(self) -> Iterator[str]:
-        yield from ()
-
-    @property
-    def agent(self) -> ConfigAgent[ConfigModelT]:
-        return self._agent
-
-    @property
-    def toplevel_interpolation_namespace(self) -> dict[str, Any]:
-        return self.interpolation_namespace
-
-    @property
-    def at(self) -> ConfigModelT | None:
-        return self.owner
-
-    @property
-    def owner(self) -> ConfigModelT | None:
-        return self._owner
-
-    @owner.setter
-    def owner(self, config: ConfigModelT | None) -> None:
-        if config is None:
-            return
-        self._owner = config
-
-    @property
-    def initial_state(self) -> dict[str, Any]:
-        return copy.deepcopy(self._initial_state)
-
-    @initial_state.setter
-    def initial_state(self, initial_state: dict[str, Any]) -> None:
-        self._initial_state = copy.deepcopy(initial_state)
-
-    def __repr__(self) -> str:
-        agent = self.agent
-        return (
-            f"<{type(self).__name__} "
-            f"of {type(self.owner).__name__!r} configuration "
-            f"({agent=})>"
-        )
-
-
-class Subcontext(BaseContext[ConfigModelT], Generic[ConfigModelT]):
-    """
-    The subcontext of a configuration model.
-
-    Parameters
-    ----------
-    parent
-        The parent context.
-    part
-        The name of the item nested in the item the parent context points to.
-    """
-
-    __slots__ = ("_parent", "_part", "_interpolation_namespace")
-
-    def __init__(
-        self,
-        parent: BaseContext[ConfigModelT],
-        part: str,
-        interpolation_namespace: dict[str, Any],
-    ) -> None:
-        self._parent = parent
-        self._part = part
-        self.interpolation_namespace = interpolation_namespace
-
-    @property
-    def agent(self) -> ConfigAgent[ConfigModelT]:
-        return self._parent.agent
-
-    @property
-    def toplevel_interpolation_namespace(self) -> dict[str, Any]:
-        return self._parent.toplevel_interpolation_namespace
-
-    def trace_route(self) -> Iterator[str]:
-        yield from self._parent.trace_route()
-        yield self._part
-
-    @property
-    def at(self) -> ConfigAt[ConfigModelT]:
-        if self.owner is None:
-            msg = "Cannot get at() of a model without parent model"
-            raise ValueError(msg)
-        return ConfigAt(self.owner, None, self.route)
-
-    @property
-    def owner(self) -> ConfigModelT | None:
-        return self._parent.owner
-
-    @property
-    def initial_state(self) -> dict[str, Any]:
-        return self._parent.initial_state
-
-    @initial_state.setter
-    def initial_state(self, value: dict[str, Any]) -> None:
-        data = self._parent.initial_state
-        data[self._part] = copy.deepcopy(value)
-        self._parent.initial_state = data
-
-    def __repr__(self) -> str:
-        agent = self.agent
-        route = self.route
-        return (
-            f"<{type(self).__name__} "
-            f"of {type(self.owner).__name__ + '.' + str(route)!r} configuration "
-            f"({agent=})>"
-        )
-
-
-def get_context(config: ConfigModelT) -> BaseContext[ConfigModelT]:
-    """
-    Get the context of the configuration model.
-
-    Parameters
-    ----------
-    config
-        The configuration model instance.
-
-    Returns
-    -------
-    The context of the configuration model.
-    """
-    context = get_context_or_none(config)
-    if context is None:
-        raise RuntimeError(
-            "This model is either inside a list "
-            "or was not loaded by a configuration agent."
-        )
-    return context
-
-
-def get_context_or_none(config: ConfigModelT) -> BaseContext[ConfigModelT] | None:
-    """
-    Get the context of the configuration model safely.
-
-    Parameters
-    ----------
-    config
-        The configuration model instance.
-
-    Returns
-    -------
-    The context of the configuration model.
-    """
-    return cast(
-        Optional[BaseContext[ConfigModelT]], getattr(config, LOCAL).get(current_context)
-    )
-
-
-# noinspection PyUnusedLocal
-@make_generic_validator
-def _common_field_validator(
-    cls: type[ConfigModelT],
-    v: Any,
-    values: dict[str, Any],
-    field: pydantic.fields.ModelField,
-    config: pydantic.BaseConfig,
-) -> Any:
-    post_hook_value = field_hook(field.outer_type_, v)
-    disallow_interpolation = getattr(config, "disallow_interpolation", False)
-    disallowed_interpolation_fields = set()
-
-    interpolation_tracker = current_interpolation_tracker.get()
-
-    if interpolation_tracker is None:
-        interpolation_tracker = {}
-        current_interpolation_tracker.set(interpolation_tracker)
-
-    if not isinstance(disallow_interpolation, bool):
-        disallowed_interpolation_fields = set(disallow_interpolation)
-    if (
-        field.field_info.extra.get("interpolate", True)
-        and field.alias not in disallowed_interpolation_fields
-    ):
-        old_value = post_hook_value
-        try:
-            interpolated = interpolate(
-                post_hook_value,
-                cls,
-                values.copy(),
-                field.outer_type_,
-            )
-        except InterpolationError as err:
-            err.message += f" (encountered in {cls.__qualname__}.{field.alias})"
-            raise
-
-        new_value = field_hook(field.outer_type_, interpolated)
-        if old_value != new_value:
-            interpolation_tracker[field.alias] = (old_value, copy.copy(new_value))
-        post_hook_value = new_value
-    return post_hook_value
-
-
-def _json_encoder(model_encoder: Callable[..., Any], value: Any, **kwargs: Any) -> Any:
-    initial_state_type = type(value)
-    converted_value = export_hook(value)
-    if isinstance(converted_value, initial_state_type):
-        return model_encoder(value, **kwargs)
-    return converted_value
-
-
-class ConfigModelMetaclass(ModelMetaclass):
-    def __new__(
-        cls,
-        name: str,
-        bases: tuple[type, ...],
-        namespace: dict[str, Any],
-        **kwargs: Any,
-    ) -> type:
-        namespace |= dict.fromkeys(
-            (EXPORT, CONTEXT, LOCAL, TOKEN), pydantic.PrivateAttr()
-        ) | {INTERPOLATION_TRACKER: pydantic.PrivateAttr(default_factory=dict)}
-
-        if namespace.get(INTERPOLATION_INCLUSIONS) is None:
-            namespace[INTERPOLATION_INCLUSIONS] = {}
-
-        if namespace.get(INTERPOLATOR) is None:
-            namespace[INTERPOLATOR] = BaseInterpolator()
-
-        if kwargs.pop("root", None):
-            return type.__new__(cls, name, bases, namespace, **kwargs)
-
-        model = super().__new__(cls, name, bases, namespace, **kwargs)
-        for field in model.__fields__.values():
-            if field.pre_validators is None:
-                field.pre_validators = []
-            field.pre_validators[:] = [_common_field_validator, *field.pre_validators]
-            if type(field.outer_type_) is ConfigModelMetaclass:
-                validator = make_generic_validator(
-                    field.outer_type_.__field_setup__  # type: ignore[attr-defined]
-                )
-                field.pre_validators[:] = [
-                    _common_field_validator,
-                    validator,
-                    *field.pre_validators,
-                ]
-        model_encoder = model.__json_encoder__
-        model.__json_encoder__ = functools.partial(_json_encoder, model_encoder)
-        return cast(type, model)
-
-
-class ConfigMeta(pydantic.BaseSettings.Config):
-    """
-    Meta-configuration for configuration models.
-
-    See https://docs.pydantic.dev/latest/usage/model_config/ for more information
-    on model configurations.
-
-    Attributes
-    ----------
-    resource
-        The configuration resource to read from/write to.
-
-        If a string, it will be interpreted as a path to a file.
-
-    parser_name
-        The anyconfig parser to use.
-
-    autoupdate_forward_refs
-        Whether to automatically update forward references
-        when `ConfigModel.load()` or `ConfigModel.load_async()`
-        methods are called. For convenience, defaults to `True`.
-
-    And all other attributes from `pydantic.BaseSettings.Config`.
-    """
-
-    resource: ConfigAgent[ConfigModel] | RawResourceT | None = None
-    parser_name: str | None = None
-    validate_assignment: bool = True
-    autoupdate_forward_refs: bool = True
-
-    Extra = pydantic.Extra
-
-
-class ConfigModel(
-    pydantic.BaseSettings,
-    metaclass=ConfigModelMetaclass,
-    root=True,
-):
-    """The base class for configuration models."""
-
-    __config__ = ConfigMeta
-
-    def __init__(self, **kwargs: Any) -> None:
-        # Set private attributes via the constructor
-        # to allow preprocessor-related instances to exist.
-        for private_attr in self.__private_attributes__:
-            value = kwargs.pop(private_attr, Undefined)
-            if value is not Undefined:
-                if private_attr == CONTEXT:
-                    context = current_context.get()
-                    if context:
-                        value = context
-                    current_context.set(value)
-                object.__setattr__(self, private_attr, value)
-        super().__init__(**kwargs)
-
-    def __deepcopy__(
-        self: ConfigModelT, memodict: dict[Any, Any] | None = None
-    ) -> ConfigModelT:
-        state = dict(self._iter(to_dict=False))
-        state.pop(LOCAL, None)
-        state.pop(TOKEN, None)
-        clone = copy.deepcopy(state)
-        return type(self).parse_obj(
-            {
-                field.alias: clone[field_name]
-                for field_name, field in self.__fields__.items()
-            }
-        )
-
-    def __setattr__(self, key: str, value: Any) -> None:
-        getattr(self, LOCAL).run(super().__setattr__, key, value)
-
-    def _init_private_attributes(self) -> None:
-        super()._init_private_attributes()
-        local = contextvars.copy_context()
-        object.__setattr__(self, LOCAL, local)
-        tok = getattr(self, TOKEN, None)
-        if tok:
-            context = current_context.get()
-            if context is not None:
-                context.interpolation_namespace |= self.dict()
-            current_context.reset(tok)
-
-    def export(self, **kwargs: Any) -> dict[str, Any]:
-        """
-        Export the configuration model.
-
-        Returns
-        -------
-        The exported configuration model.
-        """
-        _exporting.set(True)  # noqa: FBT003
-        return isolate_run(self.dict, **kwargs)
-
-    async def export_async(self, **kwargs: Any) -> dict[str, Any]:
-        """
-        Export the configuration model.
-
-        Returns
-        -------
-        The exported configuration model.
-        """
-        _exporting.set(True)  # noqa: FBT003
-        return await isolate_await(self.dict_async, **kwargs)
-
-    async def dict_async(self, **kwargs: Any) -> dict[str, Any]:
-        """
-        Get the dictionary representation of the configuration model.
-
-        Returns
-        -------
-        The dictionary representation of the configuration model.
-        """
-        return dict(await self._iter_async(to_dict=True, **kwargs))
-
-    # noinspection PyShadowingNames
-    async def json_async(  # noqa: PLR0913
-        self,
-        include: IncludeExcludeT = None,
-        exclude: IncludeExcludeT = None,
-        *,
-        by_alias: bool = False,
-        exclude_unset: bool = False,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-        encoder: Callable[[Any], Any] | None = None,
-        models_as_dict: bool = True,
-        **dumps_kwargs: Any,
-    ) -> str:
-        encoder = cast(Callable[[Any], Any], encoder or self.__json_encoder__)
-        data = dict(
-            await self._iter_async(
-                to_dict=models_as_dict,
-                by_alias=by_alias,
-                include=include,
-                exclude=exclude,
-                exclude_unset=exclude_unset,
-                exclude_defaults=exclude_defaults,
-                exclude_none=exclude_none,
-            )
-        )
-        if self.__custom_root_type__:
-            data = data[ROOT_KEY]
-        return self.__config__.json_dumps(data, default=encoder, **dumps_kwargs)
-
-    def _iter(  # type: ignore[override]
-        self, **kwargs: Any
-    ) -> Iterator[tuple[str, Any]]:
-        if kwargs.get("to_dict", False) and _exporting.get():
-            state: dict[str, Any] = {}
-            for key, value in super()._iter(**kwargs):
-                state |= [self._export_iter_hook(key, value)]
-            metadata = getattr(self, EXPORT, None)
-            if metadata:
-                context = get_context(self)
-                context.agent.processor_class.export(state, metadata=metadata)
-            yield from state.items()
-        else:
-            yield from super()._iter(**kwargs)
-
-    async def _iter_async(self, **kwargs: Any) -> Iterator[tuple[str, Any]]:
-        if kwargs.get("to_dict", False) and _exporting.get():
-            state: dict[str, Any] = {}
-            for key, value in super()._iter(**kwargs):
-                state |= [self._export_iter_hook(key, value)]
-            metadata = getattr(self, EXPORT, None)
-            if metadata:
-                context = get_context(self)
-                await context.agent.processor_class.export_async(
-                    state, metadata=metadata
-                )
-            return ((key, value) for key, value in state.items())
-        return super()._iter(**kwargs)
-
-    def _export_iter_hook(
-        self,
-        key: str,
-        value: Any,
-    ) -> tuple[str, Any]:
-        interpolation_tracker = getattr(self, LOCAL).get(current_interpolation_tracker)
-        field = self.__fields__.get(key)
-        actual_key = field.alias if field else key
-        if interpolation_tracker:
-            interpolation_track = interpolation_tracker.get(actual_key)
-            if interpolation_track:
-                old_value, new_value = interpolation_track
-                # if value != new_value:
-                #     raise InterpolationError(
-                #         f"Cannot restore the value of {actual_key!r} "
-                #         "before interpolation."
-                #     )
-                value = old_value
-        return actual_key, value
-
-    @classmethod
-    @no_type_check
-    def _get_value(cls, value: Any, *, to_dict: bool, **kwds: Any) -> Any:
-        if _exporting.get():
-            exporter = export_model.dispatch(type(value))
-            if (
-                isinstance(value, BaseModel)
-                or exporter != export_model.dispatch(object)
-            ) and to_dict:
-                value_dict = export_model(value, **kwds)
-                if ROOT_KEY in value_dict:
-                    return value_dict[ROOT_KEY]
-                return value_dict
-        return super()._get_value(value, to_dict=to_dict, **kwds)
-
-    @classmethod
-    def _resolve_agent(
-        cls,
-        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
-        *,
-        create_if_missing: bool | None = None,
-        parser_name: str | None = None,
-    ) -> ConfigAgent[ConfigModelT]:
-        if resource is None:
-            resource = getattr(cls.__config__, "resource", None)
-        if resource is None:
-            raise ValueError("No resource specified")
-        if parser_name is None:
-            parser_name = getattr(cls.__config__, "parser_name", None)
-        agent: ConfigAgent[ConfigModelT]
-        if isinstance(resource, ConfigAgent):
-            agent = resource
-        else:
-            agent = ConfigAgent(
-                resource,
-                parser_name=parser_name,
-            )
-        if create_if_missing is not None:
-            agent.create_if_missing = create_if_missing
-        if parser_name is not None:
-            agent.parser_name = cast(str, parser_name)
-        return agent
-
-    @property
-    def initial_state(self) -> dict[str, Any]:
-        """
-        The initial configuration state.
-
-        It is a copy of the configuration state
-        at the last time of loading, reloading or saving.
-        """
-        return get_context(self).initial_state
-
-    def at(
-        self: ConfigModelT,
-        route: ConfigRouteLike | None = None,
-    ) -> ConfigModelT | ConfigAt[ConfigModelT]:
-        """
-        Lazily point to a specific item in the configuration.
-
-        Parameters
-        ----------
-        route
-            The access route to the item in this configuration.
-            If None, the whole configuration is returned.
-
-        Returns
-        -------
-        The configuration accessor.
-        """
-        if route is None:
-            context = get_context_or_none(self)
-            self_at = None
-            if context is not None:
-                self_at = context.at
-            if self_at is not None:
-                return self_at
-            return self
-        return ConfigAt(self, None, route)
-
-    @overload
-    def get(self: ConfigModelT, route: None = None, default: Any = ...) -> ConfigModelT:
-        ...
-
-    @overload
-    def get(
-        self: ConfigModelT, route: ConfigRouteLike = ..., default: Any = ...
-    ) -> Any:
-        ...
-
-    def get(
-        self, route: ConfigRouteLike | None = None, default: Any = Undefined
-    ) -> Any:
-        """
-        Get a value from the configuration.
-
-        Parameters
-        ----------
-        route
-            Route to access the item. If None, the whole configuration is returned.
-        default
-        """
-        if route is None:
-            return self
-        return self.at(route).get(default=default)
-
-    def update(self, kwargs: dict[str, Any]) -> None:
-        """
-        Update the configuration with new values, in-place.
-
-        Parameters
-        ----------
-        kwargs
-            The new values to update the configuration with.
-
-        Returns
-        -------
-        None
-        """
-        # Crucial difference to self.__dict__.update():
-        # self.__dict__.update() would not trigger the validation
-        # of the new values.
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
-    def rollback(self) -> None:
-        """
-        Rollback the configuration to its initial state.
-
-        Returns
-        -------
-        None
-        """
-        context = get_context(self)
-        self.__dict__.update(context.initial_state)
-
-    @classmethod
-    def load(
-        cls: type[ConfigModelT],
-        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
-        *,
-        create_if_missing: bool | None = None,
-        parser_name: str | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Load the configuration file.
-        To reload the configuration, use the `reload()` method.
-
-        Parameters
-        ----------
-        resource
-            The configuration resource to read from/write to.
-        parser_name
-            The anyconfig parser to use.
-        create_if_missing
-            Whether to create the configuration file if it does not exist.
-        **kwargs
-            Keyword arguments to pass to the read method.
-
-        Returns
-        -------
-        self
-        """
-        agent = cls._resolve_agent(
-            resource,
-            parser_name=parser_name,
-            create_if_missing=create_if_missing,
-        )
-        current_context.set(Context(agent))
-        local = contextvars.copy_context()
-        if getattr(
-            cls.__config__,
-            "autoupdate_forward_refs",
-            ConfigMeta.autoupdate_forward_refs,
-        ):
-            cls.update_forward_refs()
-        config = local.run(agent.read, config_class=cls, **kwargs)
-        object.__setattr__(config, LOCAL, local)
-        context = cast(Context[ConfigModelT], local.get(current_context))
-        context.owner = config
-        context.initial_state = config.__dict__
-        return config
-
-    def reload(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
-        """
-        Reload the configuration file.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the read method.
-
-        Returns
-        -------
-        self
-        """
-        context = get_context(self)
-        current_context.set(get_context(context.owner))
-        if context.owner is self:
-            changed = context.agent.read(config_class=type(self), **kwargs)
-        else:
-            changed = _reload(cast(ConfigModelT, context.at), **kwargs)
-        state = changed.__dict__
-        context.initial_state = state
-        self.update(state)
-        return self
-
-    def save(
-        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
-    ) -> int:
-        """
-        Save the configuration to the configuration file.
-
-        Parameters
-        ----------
-        write_kwargs
-            Keyword arguments to pass to the write method.
-        **kwargs
-            Keyword arguments to pass to the dumping method.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        context = get_context(self)
-        if context.owner is self:
-            if write_kwargs is None:
-                write_kwargs = {}
-            blob = context.agent.dump_config(self, **kwargs)
-            result = self.write(blob, **write_kwargs)
-            context.initial_state = self.__dict__
-            return result
-        return _save(
-            cast(ConfigAt[ConfigModelT], context.at),
-            write_kwargs=write_kwargs,
-            **kwargs,
-        )
-
-    def write(self, blob: str | bytes, **kwargs: Any) -> int:
-        """
-        Overwrite the configuration file with the given string or bytes.
-
-        Parameters
-        ----------
-        blob
-            The blob to write to the configuration file.
-        **kwargs
-            Keyword arguments to pass to the open method.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        context = get_context(self)
-        if context.agent.is_url:
-            msg = "Writing to URLs is not yet supported"
-            raise NotImplementedError(msg)
-        return context.agent.write(blob, **kwargs)
-
-    @classmethod
-    async def load_async(
-        cls: type[ConfigModelT],
-        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
-        *,
-        parser_name: str | None = None,
-        create_if_missing: bool | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Load the configuration file asynchronously.
-        To reload the configuration, use the `reload_async()` method.
-
-        Parameters
-        ----------
-        resource
-            The configuration resource.
-        parser_name
-            The anyconfig parser to use.
-        create_if_missing
-            Whether to create the configuration file if it does not exist.
-        **kwargs
-            Keyword arguments to pass to the read method.
-
-        Returns
-        -------
-        self
-        """
-        agent = cls._resolve_agent(
-            resource, create_if_missing=create_if_missing, parser_name=parser_name
-        )
-        current_context.set(Context(agent))
-        local = contextvars.copy_context()
-        if getattr(
-            cls.__config__,
-            "autoupdate_forward_refs",
-            ConfigMeta.autoupdate_forward_refs,
-        ):
-            cls.update_forward_refs()
-        reader = local.run(
-            asyncio.create_task, agent.read_async(config_class=cls, **kwargs)
-        )
-        config = await reader
-        object.__setattr__(config, LOCAL, local)
-        context = cast(Context[ConfigModelT], local.get(current_context))
-        context.owner = config
-        return config
-
-    async def reload_async(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
-        """
-        Reload the configuration file asynchronously.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the read method.
-
-        Returns
-        -------
-        self
-        """
-        context = get_context(self)
-        current_context.set(get_context(context.owner))
-        if context.owner is self:
-            changed = await context.agent.read_async(config_class=type(self), **kwargs)
-        else:
-            changed = await _reload_async(
-                cast(ConfigAt[ConfigModelT], context.at), **kwargs
-            )
-        state = changed.__dict__
-        context.initial_state = state
-        self.update(state)
-        return self
-
-    async def save_async(
-        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
-    ) -> int:
-        """
-        Save the configuration to the configuration file asynchronously.
-
-        Parameters
-        ----------
-        write_kwargs
-            Keyword arguments to pass to the write method.
-        **kwargs
-            Keyword arguments to pass to the dumping method.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        context = get_context(self)
-        if context.owner is self:
-            if write_kwargs is None:
-                write_kwargs = {}
-            _exporting.set(True)  # noqa: FBT003
-            blob = await context.agent.dump_config_async(self, **kwargs)
-            result = await self.write_async(blob, **write_kwargs)
-            context.initial_state = self.__dict__
-            return result
-        return await _save_async(
-            cast(ConfigAt[ConfigModelT], context.at),
-            write_kwargs=write_kwargs,
-            **kwargs,
-        )
-
-    async def write_async(self, blob: str | bytes, **kwargs: Any) -> int:
-        """
-        Overwrite the configuration file asynchronously with the given string or bytes.
-
-        Parameters
-        ----------
-        blob
-            The blob to write to the configuration file.
-        **kwargs
-            Keyword arguments to pass to the open method.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        context = get_context(self)
-        if context.agent.is_url:
-            msg = "Saving to URLs is not yet supported"
-            raise NotImplementedError(msg)
-        return await context.agent.write_async(blob, **kwargs)
-
-    @classmethod
-    def _evaluate_interpolation_namespaces(cls) -> dict[str | None, dict[str, Any]]:
-        inclusions = getattr(cls, INTERPOLATION_INCLUSIONS)
-        return {
-            namespace_id: evaluate_namespace()
-            for namespace_id, evaluate_namespace in inclusions.items()
-        }
-
-    @classmethod
-    def get_interpolation_namespace(
-        cls,
-        identifiers: set[str],
-        closest_namespace: dict[str, Any],
-    ) -> dict[str, Any]:
-        """Get the interpolation namespace according to requested identifiers."""
-        context = current_context.get()
-        interpolation_context = {}
-
-        namespaces = cls._evaluate_interpolation_namespaces()
-        if context is not None:
-            namespaces.setdefault(None, {}).update(
-                context.toplevel_interpolation_namespace
-            )
-        for identifier in identifiers:
-            (
-                namespace_identifier,
-                specifies_namespace,
-                raw_route,
-            ) = identifier.rpartition(NAMESPACE_TOKEN)
-            namespace = namespaces.get(None, {})
-            if specifies_namespace:
-                try:
-                    namespace |= namespaces[namespace_identifier]
-                except KeyError:
-                    raise InterpolationLookupError(namespace_identifier) from None
-            else:
-                namespace |= closest_namespace
-
-            owner, has_at, raw_route = raw_route.rpartition(AT_TOKEN)
-
-            lookup_identifier = owner if has_at else raw_route
-            try:
-                value = at(namespace, lookup_identifier)
-            except ResourceLookupError:
-                if not specifies_namespace:
-                    raise
-                value = at(closest_namespace, lookup_identifier)
-
-            if has_at:
-                owner = value
-                if not isinstance(owner, ConfigModel):
-                    raise InterpolationError(
-                        f"Cannot @-interpolate with {type(owner).__name__!r} objects"
-                    )
-                value = owner.at(raw_route)
-
-            interpolation_context[identifier] = value
-            if raw_route not in closest_namespace:
-                interpolation_context[raw_route] = value
-
-        return interpolation_context
-
-    @classmethod
-    def __field_setup__(cls, value: dict[str, Any], field: ModelField) -> Any:
-        """
-        Called when this configuration model is being initialized as a field
-        of some other configuration model.
-        """
-        context = current_context.get()
-        if context is not None:
-            subcontext = context.enter(field.name)
-            tok = current_context.set(subcontext)
-            return _get_object_state(value) | {
-                TOKEN: tok,
-                LOCAL: contextvars.copy_context(),
-            }
-        return value
-
-    if not TYPE_CHECKING:
-        load = isolation_runner(load)
-        load_async = isolation_runner(load_async)
-        reload = isolation_runner(reload)
-        reload_async = isolation_runner(reload_async)
-        save = isolation_runner(save)
-        save_async = isolation_runner(save_async)
-        export = isolation_runner(export)
-        export_async = isolation_runner(export_async)
-
-
-setattr(ConfigModel, INTERPOLATION_INCLUSIONS, None)
-include.register(ConfigModel, include_const)
-
-if os.getenv("CONFIGZEN_SETUP") != "0":
-    importlib.import_module("._setup", package=__package__)
+"""
+The main module of the configzen library.
+
+This module provides an API to manage configuration files and resources
+in a consistent way. It also provides tools to load and save configuration
+files in various formats and within a number of advanced methods.
+
+```python
+from configzen import ConfigModel, ConfigField, ConfigMeta
+
+class DatabaseConfig(ConfigModel):
+    host: str
+    port: int
+    user: str
+    password: str = ConfigField(exclude=True)
+
+    class Config(ConfigMeta):
+        resource = "examples/database.json"
+
+db_config = DatabaseConfig.load()
+db_config.host = "newhost"
+db_config.port = 5432
+
+db_config.save()
+
+db_config = DatabaseConfig.load()
+print(db_config.host)
+print(db_config.port)
+
+# Output:
+# newhost
+# 5432
+
+db_config.host = "otherhost"
+db_config.port = 5433
+
+db_config.at("host").save()
+
+print(db_config.host)
+print(db_config.port)
+
+# Output:
+# otherhost
+# 5432  # <- not 5433, because we saved only host
+
+db_config.host = "anotherhost"
+db_config.at("port").reload()
+
+print(db_config.host)
+print(db_config.port)
+
+# Output:
+# otherhost  # <- not anotherhost, because we reloaded only port
+# 5432
+```
+"""
+
+from __future__ import annotations
+
+import abc
+import asyncio
+import contextvars
+import copy
+import dataclasses
+import functools
+import importlib
+import inspect
+import io
+import itertools
+import os
+import pathlib
+import sys
+import types
+import urllib.parse
+import urllib.request
+from collections.abc import (
+    Callable,
+    Mapping,
+    Iterator,
+)
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    ClassVar,
+    Generic,
+    Literal,
+    Optional,
+    Union,
+    cast,
+    get_args,
+    get_origin,
+    no_type_check,
+    overload,
+)
+
+import anyconfig
+import pydantic
+from anyconfig.utils import filter_options, is_dict_like, is_list_like
+from pydantic.fields import make_generic_validator  # type: ignore[attr-defined]
+from pydantic.fields import ModelField, Undefined
+from pydantic.main import BaseModel, ModelMetaclass
+from pydantic.utils import ROOT_KEY
+
+from configzen._detach import (
+    detached_context_run,
+    detached_context_await,
+    detached_context_function,
+)
+from configzen.errors import (
+    ConfigAccessError,
+    ResourceLookupError,
+    UnavailableParserError,
+    UnspecifiedParserError,
+    InterpolationError,
+)
+from configzen.interpolation import (
+    EVALUATION_ENGINE,
+    INTERPOLATOR,
+    BaseInterpolator,
+    include_const,
+    interpolate,
+    include,
+    BaseEvaluationEngine,
+)
+from configzen.module import MODULE, ConfigModule
+from configzen.processor import EXPORT, DirectiveContext, Processor
+from configzen.route import ConfigRoute
+from configzen.typedefs import (
+    AsyncConfigIO,
+    ConfigIO,
+    ConfigModelT,
+    ConfigRouteLike,
+    IncludeExcludeT,
+    NormalizedResourceT,
+    RawResourceT,
+    T,
+)
+
+try:
+    import aiofiles
+
+    AIOFILES_AVAILABLE = True
+except ImportError:
+    aiofiles = None  # type: ignore[assignment]
+    AIOFILES_AVAILABLE = False
+
+__all__ = (
+    "ConfigAgent",
+    "ConfigAt",
+    "ConfigModel",
+    "ConfigMeta",
+    "export_hook",
+    "field_hook",
+    "export_model",
+    "export_model_async",
+)
+
+ALL_URL_SCHEMES: set[str] = set(
+    urllib.parse.uses_relative + urllib.parse.uses_netloc + urllib.parse.uses_params
+) - {""}
+
+CONTEXT: str = "__context__"
+TOKEN: str = "__context_token__"
+LOCAL: str = "__local__"
+
+INTERPOLATION_TRACKER: str = "__interpolation_tracker__"
+INTERPOLATION_INCLUSIONS: str = "__interpolation_inclusions__"
+
+current_context: contextvars.ContextVar[
+    BaseContext[Any] | None
+    ] = contextvars.ContextVar("current_context", default=None)
+
+current_interpolation_tracker: contextvars.ContextVar[
+    dict[str, Any] | None
+    ] = contextvars.ContextVar("current_interpolation_tracker", default=None)
+
+_exporting: contextvars.ContextVar[bool] = contextvars.ContextVar(
+    "_exporting", default=False
+)
+
+
+def _get_defaults_from_model_class(
+    model: type[pydantic.BaseModel],
+) -> dict[str, Any]:
+    defaults = {}
+    for field in model.__fields__.values():
+        default = field.default
+        if not field.field_info.exclude and not field.required:
+            if isinstance(default, pydantic.BaseModel):
+                default = default.dict()
+            defaults[field.alias] = default
+    return defaults
+
+
+def _get_object_state(obj: Any) -> dict[str, Any]:
+    state = obj
+    if not isinstance(obj, dict):
+        state = obj.__dict__  # avoidance of vars() is intended
+    return cast(dict[str, Any], state)
+
+
+@functools.singledispatch
+def export_hook(obj: Any) -> Any:
+    """
+    Convert a value to a format that can be safely serialized.
+
+    This function is used to convert values that are not supported by
+    `anyconfig` to a format that can be safely serialized. It is used
+    internally by `ConfigModel` and `AsyncConfigModel` to convert
+    values before saving them to a file.
+
+    Parameters
+    ----------
+    obj
+        The value to convert.
+
+    Returns
+    -------
+    Any
+    """
+    if dataclasses.is_dataclass(obj):
+        return export_hook(dataclasses.asdict(obj))
+    if isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields"):
+        return _export_namedtuple(obj)
+    return obj
+
+
+@functools.singledispatch
+def _export_namedtuple(obj: tuple[Any, ...]) -> Any:
+    # Initially I wanted it to be export_hook(obj._asdict()), but
+    # pydantic doesn't seem to be friends with custom NamedTuple-s.
+    return export_hook(list(obj))
+
+
+field_hook_registrars: Any = functools.singledispatch(lambda _cls, value: value)
+
+if TYPE_CHECKING:
+
+    class _FieldHookType:
+        def __call__(self, cls: type[T], value: Any) -> Any:
+            ...
+
+        def register(
+            self,
+            cls: type[T],
+            func: Callable[[type[T], Any], Any] | None = None,
+        ) -> Callable[
+            [Callable[[type[T], Any], Any]],
+            Callable[[type[T] | Any, Any], Any],
+        ]:
+            ...
+
+        def dispatch(self, cls: type[T]) -> Callable[[type[T] | Any, Any], Any]:
+            ...
+
+
+    field_hook: _FieldHookType = _FieldHookType()
+
+else:
+
+    def field_hook(cls: type[Any], value: Any) -> Any:
+        """
+        Automatically registered pre-validator for values in fields
+        where the outer type is `cls`.
+
+        This function is used to load values that are not supported by
+        `anyconfig` to a format that can be used at runtime. It is used
+        by pydantic while performing validation.
+
+        Parameters
+        ----------
+        cls
+            The type to load the value into.
+
+        value
+            The value to load.
+
+        Returns
+        -------
+        The loaded value.
+        """
+        origin = get_origin(cls)
+        if origin in [Union] + (
+            [types.UnionType] if sys.version_info >= (3, 10) else []
+        ):
+            for result in itertools.starmap(
+                field_hook, zip(get_args(cls), itertools.repeat(value))
+            ):
+                if result != value:
+                    return result
+            return value
+        try:
+            if isinstance(value, origin or cls):
+                return value
+        except TypeError:
+            return value
+        if origin:
+            cls = origin
+
+        try:
+            cast_func = field_hook_registrars.dispatch(cls)
+        except KeyError:
+            return value
+        return cast_func(cls, value)
+
+
+    field_hook.register = field_hook_registrars.register
+
+
+@functools.singledispatch
+def export_model(obj: Any, **kwargs: Any) -> dict[str, Any]:
+    """
+    Export a ConfigModel to a safely-serializable format.
+    Register a custom exporter for a type using the `with_exporter` decorator,
+    which can help to exclude particular values from the export if needed.
+
+    Parameters
+    ----------
+    obj
+    """
+    if isinstance(obj, ConfigModel) and not _exporting.get():
+        return obj.export(**kwargs)
+    return cast(dict[str, Any], obj.dict(**kwargs))
+
+
+@functools.singledispatch
+async def export_model_async(obj: Any, **kwargs: Any) -> dict[str, Any]:
+    """
+    Export a ConfigModel to a safely-serializable format.
+    Register a custom exporter for a type using the `with_exporter` decorator,
+    which can help to exclude particular values from the export if needed.
+
+    Parameters
+    ----------
+    obj
+    """
+    if isinstance(obj, ConfigModel) and not _exporting.get():
+        return await obj.export_async(**kwargs)
+    return cast(dict[str, Any], await obj.dict_async(**kwargs))
+
+
+def _delegate_ac_options(
+    load_options: dict[str, Any], dump_options: dict[str, Any], options: dict[str, Any]
+) -> None:
+    for key, value in options.items():
+        if key.startswith("dump_"):
+            actual_key = key.removeprefix("dump_")
+            targets = [dump_options]
+        elif key.startswith("load_"):
+            actual_key = key.removeprefix("load_")
+            targets = [load_options]
+        else:
+            actual_key = key
+            targets = [load_options, dump_options]
+        for target in targets:
+            if actual_key in target:
+                msg = (
+                    f"Option {key}={value!r} overlaps with "
+                    f"defined {actual_key}={target[actual_key]!r}"
+                )
+                raise ValueError(msg)
+            target[actual_key] = value
+
+
+class ConfigAgent(Generic[ConfigModelT]):
+    """
+    Configuration resource agent: loader and saver.
+
+    This class is used to broke between the model and the home resource, which
+    can be a file, a URL, or a file-like object. It is used internally
+    by `ConfigModel` and `AsyncConfigModel` to load and save
+    configuration files.
+
+    Attributes
+    ----------
+    create_if_missing
+        Whether to create the file if it doesn't exist.
+    parser_name
+        The name of the engines to use for loading and saving the
+        configuration. If not specified, the processor will be guessed
+        from the file extension.
+    allowed_url_schemes
+        The URL schemes that are allowed to be used.
+
+    Raises
+    ------
+    ValueError
+    """
+
+    processor_class: type[Processor[ConfigModelT]]
+    create_if_missing: bool
+    is_relative: bool = False
+    allowed_url_schemes: set[str]
+    use_pydantic_json: bool = True
+    default_load_options: dict[str, Any] = {}
+    default_dump_options: dict[str, Any] = {
+        # These are usually desirable for configuration files.
+        # If you want to change them, you can do so by monkey-patching
+        # these variables. You can also change `load_options` and
+        # `dump_options` instance attributes to make a local change.
+        "allow_unicode": True,
+        "ensure_ascii": False,
+        "indent": 2,
+    }
+    _resource: NormalizedResourceT
+
+    predefined_default_kwargs: ClassVar[dict[str, Any]] = {"encoding": "UTF-8"}
+    default_allowed_url_schemes: ClassVar[set[str]] = {"file", "http", "https"}
+
+    OPEN_KWARGS: ClassVar[set[str]] = {
+        "mode",
+        "buffering",
+        "encoding",
+        "errors",
+        "newline",
+    }
+    URLOPEN_KWARGS: ClassVar[set[str]] = {
+        "data",
+        "timeout",
+        "cafile",
+        "capath",
+        "cadefault",
+        "context",
+    }
+    JSON_KWARGS: ClassVar[set[str]] = {
+        "skipkeys",
+        "ensure_ascii",
+        "check_circular",
+        "allow_nan",
+        "cls",
+        "indent",
+        "separators",
+        "default",
+        "sort_keys",
+    }
+    EXPORT_KWARGS: ClassVar[set[str]] = {
+        "by_alias",
+        "include",
+        "exclude",
+        "exclude_unset",
+        "exclude_defaults",
+        "exclude_none",
+    }
+    EXTRA_FILE_EXTENSIONS: ClassVar[dict[str, str]] = {
+        "yml": "yaml",
+        "conf": "ini",
+        "cfg": "ini",
+        # Note: CBOR (RFC 7049) is deprecated, use CBOR (RFC 8949) instead.
+        "cbor": "cbor2",
+        # https://github.com/msgpack/msgpack/issues/291#issuecomment-1370526984
+        "mpk": "msgpack",
+        "pkl": "pickle",
+    }
+    BINARY_DATA_PARSERS: ClassVar[set[str]] = {
+        "ion",
+        "bson",
+        "cbor",
+        "cbor2",
+        "msgpack",
+        "pickle",
+    }
+    SUPPORTED_PARSERS: list[str] = anyconfig.list_types()
+
+    def __init__(
+        self,
+        resource: RawResourceT,
+        parser_name: str | None = None,
+        processor_class: type[Processor[ConfigModelT]] | None = None,
+        *,
+        create_if_missing: bool = False,
+        **kwargs: Any,
+    ) -> None:
+        """Parameters
+        ----------
+        resource
+            The URL to the configuration file, or a file-like object.
+        parser_name
+            The name of the anyconfig parser to use
+            for loading and saving the configuration.
+        create_if_missing
+            Whether to automatically create missing keys when loading the configuration.
+        default_kwargs
+            Default keyword arguments to pass while opening the resource.
+        use_pydantic_json
+            Whether to use Pydantic's JSON encoder/decoder instead of the default
+            anyconfig one.
+        uses_binary_data
+            Whether to treat the data as binary.
+            Defaults to True for formats listed in `ConfigAgent.BINARY_DATA_PARSERS`.
+        **kwargs
+            Additional keyword arguments to pass to
+            `anyconfig.loads()` and `anyconfig.dumps()`.
+        """
+        self._parser_name = None
+        self._uses_binary_data = kwargs.get("uses_binary_data", False)
+
+        if processor_class is None:
+            processor_class = Processor[ConfigModelT]
+
+        self.processor_class = processor_class
+        self.parser_name = parser_name
+
+        if isinstance(resource, (str, os.PathLike)) and not (
+            isinstance(resource, str)
+            and urllib.parse.urlparse(str(resource)).scheme in ALL_URL_SCHEMES
+        ):
+            raw_path = os.fspath(resource)
+            resource = pathlib.Path(raw_path)
+            if (
+                raw_path.startswith(".")
+                and resource.parts
+                and not resource.parts[0].startswith(".")
+            ):
+                self.is_relative = True
+
+        self.resource = resource
+        self.create_if_missing = create_if_missing
+        self.use_pydantic_json = kwargs.pop("use_pydantic_json", True)
+        self.default_kwargs = kwargs.pop(
+            "default_kwargs", self.predefined_default_kwargs.copy()
+        )
+        self.allowed_url_schemes = kwargs.pop(
+            "allowed_url_schemes", self.default_allowed_url_schemes.copy()
+        )
+
+        self.load_options = self.default_load_options.copy()
+        self.dump_options = self.default_dump_options.copy()
+
+        _delegate_ac_options(self.load_options, self.dump_options, kwargs)
+
+    @property
+    def resource(self) -> NormalizedResourceT:
+        """
+        The resource of the configuration.
+
+        This can be a file path, a URL, or a file-like object.
+
+        Returns
+        -------
+        The resource of the configuration.
+        """
+        return self._resource
+
+    @resource.setter
+    def resource(self, value: NormalizedResourceT) -> None:
+        """
+        The resource of the configuration.
+
+        This can be a file path, a URL, or a file-like object.
+
+        .. note::
+            If the resource is a file path, the processor will be guessed
+            from the file extension.
+
+        Returns
+        -------
+        The resource of the configuration.
+        """
+        self._resource = value
+        if self.parser_name is None:
+            self.parser_name = self._guess_parser_name()
+
+    @property
+    def parser_name(self) -> str | None:
+        return self._parser_name
+
+    @parser_name.setter
+    def parser_name(self, value: str | None) -> None:
+        if value is not None:
+            value = value.casefold()
+        self._parser_name = value
+
+    def _guess_parser_name(self) -> str | None:
+        parser_name = None
+        if isinstance(self.resource, pathlib.Path):
+            suffix = self.resource.suffix[1:].casefold()
+            supported_parsers = self.SUPPORTED_PARSERS
+            if not suffix:
+                recognized_file_extensions = supported_parsers + [
+                    alias + "(-> " + actual_parser_name + ")"
+                    for alias, actual_parser_name in self.EXTRA_FILE_EXTENSIONS.items()
+                    if actual_parser_name in supported_parsers
+                ]
+                msg = (
+                    "Could not guess the anyconfig parser to use for "
+                    f"{self.resource!r}.\n"
+                    f"Recognized file extensions: {recognized_file_extensions}"
+                )
+                raise UnspecifiedParserError(msg)
+            parser_name = self.EXTRA_FILE_EXTENSIONS.get(suffix, suffix)
+            if (
+                parser_name == "cbor2"
+                and "cbor2" not in supported_parsers
+                and "cbor" in supported_parsers
+            ):
+                parser_name = "cbor"
+        return parser_name
+
+    def load_into(
+        self,
+        config_class: type[ConfigModelT],
+        blob: str | bytes,
+        parser_name: str | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Load the configuration into a `ConfigModel` subclass.
+
+        Parameters
+        ----------
+        config_class
+            The `ConfigModel` subclass to load the configuration into.
+        blob
+            The configuration to load.
+        parser_name
+            The name of the engines to use for loading the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
+        dict_config = self.load_dict(blob, parser_name=parser_name, **kwargs)
+        if dict_config is None:
+            dict_config = {}
+        return config_class.parse_obj(dict_config)
+
+    async def async_load_into(
+        self,
+        config_class: type[ConfigModelT],
+        blob: str | bytes,
+        parser_name: str | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Load the configuration into a `ConfigModel` subclass asynchronously.
+
+        Parameters
+        ----------
+        config_class
+            The `ConfigModel` subclass to load the configuration into.
+        blob
+            The configuration to load.
+        parser_name
+            The name of the engines to use for loading the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
+        dict_config = await self.load_dict_async(
+            blob, parser_name=parser_name, **kwargs
+        )
+        if dict_config is None:
+            dict_config = {}
+        return config_class.parse_obj(dict_config)
+
+    def _load_dict_impl(
+        self,
+        blob: str | bytes,
+        parser_name: str | None = None,
+        **kwargs: Any,
+    ) -> dict[str, Any]:
+        parser_name = parser_name or self.parser_name or self._guess_parser_name()
+        if parser_name is None:
+            msg = "Cannot read configuration because `parser_name` was not specified"
+            raise UnspecifiedParserError(msg)
+        kwargs = self.load_options | kwargs
+        try:
+            loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
+                blob, ac_parser=parser_name, **kwargs
+            )
+        except anyconfig.UnknownParserTypeError as exc:
+            raise UnavailableParserError(str(exc).split()[-1], self) from exc
+        if not isinstance(loaded, Mapping):
+            msg = (
+                f"Expected a mapping as a result of loading {self.resource}, "
+                f"got {type(loaded).__name__}."
+            )
+            raise TypeError(msg)
+        return dict(loaded)
+
+    def load_dict(
+        self,
+        blob: str | bytes,
+        parser_name: str | None = None,
+        *,
+        preprocess: bool = True,
+        **kwargs: Any,
+    ) -> dict[str, Any]:
+        """
+        Load the configuration into a dictionary. The dictionary is
+        usually used to initialize a `ConfigModel` subclass. If the
+        configuration is empty, None might be returned instead of a dictionary.
+
+        Parameters
+        ----------
+        blob
+            The configuration to load.
+        parser_name
+            The name of the anyconfig parser to use for loading the configuration.
+        preprocess
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration dictionary.
+        """
+        loaded = self._load_dict_impl(blob, parser_name=parser_name, **kwargs)
+        if preprocess:
+            loaded = self.processor_class(self, loaded).preprocess()
+        return loaded
+
+    async def load_dict_async(
+        self,
+        blob: str | bytes,
+        parser_name: str | None = None,
+        *,
+        preprocess: bool = True,
+        **kwargs: Any,
+    ) -> dict[str, Any]:
+        """
+        Load the configuration into a dictionary asynchronously.
+
+        Parameters
+        ----------
+        blob
+            The configuration to load.
+        parser_name
+            The name of the anyconfig parser to use for loading the configuration.
+        preprocess
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration dictionary.
+        """
+        loaded = self._load_dict_impl(blob, parser_name, **kwargs)
+        if preprocess:
+            loaded = await self.processor_class(self, loaded).preprocess_async()
+        return loaded
+
+    def dump_config(
+        self,
+        config: ConfigModelT,
+        parser_name: str | None = None,
+        **kwargs: Any,
+    ) -> str:
+        """
+        Dump the configuration to a string.
+
+        Parameters
+        ----------
+        config
+            The configuration to dump.
+        parser_name
+            The name of the anyconfig parser to use for saving the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.dumps()`.
+
+        Returns
+        -------
+        The dumped configuration.
+        """
+        if parser_name is None:
+            parser_name = self.parser_name
+        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
+        if parser_name == "json" and self.use_pydantic_json:
+            export_kwargs |= filter_options(
+                self.JSON_KWARGS, self.dump_options | kwargs
+            )
+            _exporting.set(True)  # noqa: FBT003
+            return detached_context_run(config.json, **export_kwargs)
+        data = export_model(config, **export_kwargs)
+        return self.dump_data(data, parser_name=parser_name, **kwargs)
+
+    async def dump_config_async(
+        self,
+        config: ConfigModelT,
+        parser_name: str | None = None,
+        **kwargs: Any,
+    ) -> str:
+        """
+        Dump the configuration to a string.
+
+        Parameters
+        ----------
+        config
+            The configuration to dump.
+        parser_name
+            The name of the anyconfig parser to use for saving the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.dumps()`.
+
+        Returns
+        -------
+        The dumped configuration.
+        """
+        if parser_name is None:
+            parser_name = self.parser_name
+        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
+        if parser_name == "json" and self.use_pydantic_json:
+            export_kwargs |= filter_options(
+                self.JSON_KWARGS, self.dump_options | kwargs
+            )
+            _exporting.set(True)  # noqa: FBT003
+            return await detached_context_await(config.json_async, **export_kwargs)
+        data = await export_model_async(config, **export_kwargs)
+        return self.dump_data(data, parser_name=parser_name, **kwargs)
+
+    def dump_data(
+        self,
+        data: dict[str, Any],
+        parser_name: str | None = None,
+        **kwargs: Any,
+    ) -> str:
+        """
+        Dump data to a string.
+
+        Parameters
+        ----------
+        data
+            The data to dump.
+        parser_name
+            The name of the anyconfig parser to use for saving the configuration.
+        kwargs
+            Additional keyword arguments to pass to `anyconfig.dumps()`.
+
+        Returns
+        -------
+        The dumped configuration.
+        """
+        if parser_name is None:
+            parser_name = self.parser_name
+        if parser_name is None:
+            msg = (
+                "Cannot write configuration because `parser_name` was not specified"
+                f"for agent {self}"
+            )
+            raise UnspecifiedParserError(msg)
+        kwargs = self.dump_options | kwargs
+        return anyconfig.dumps(export_hook(data), ac_parser=parser_name, **kwargs)
+
+    @property
+    def is_url(self) -> bool:
+        """
+        Whether the resource is a URL.
+
+        This simply checks if the resource object is a string, since local paths
+        are converted into `pathlib.Path` objects.
+        """
+        return isinstance(self.resource, str)
+
+    @property
+    def uses_binary_data(self) -> bool:
+        """
+        Whether the resource uses bytes for storing data, not str.
+        """
+        return self._uses_binary_data or self.parser_name in self.BINARY_DATA_PARSERS
+
+    def open_resource(self, **kwds: Any) -> ConfigIO:
+        """
+        Open the configuration file.
+
+        Parameters
+        ----------
+        **kwds
+            Keyword arguments to pass to the opening routine.
+            For URLs, these are passed to ``urllib.request.urllib.request.urlopen()``.
+            For local files, these are passed to ``builtins.open()``.
+
+        Returns
+        -------
+        The opened resource.
+        """
+        if self.resource is None:
+            if self.uses_binary_data:
+                return io.BytesIO()
+            return io.StringIO()
+        if self.is_url:
+            url = urllib.parse.urlparse(cast(str, self.resource))
+            if url.scheme not in self.allowed_url_schemes:
+                msg = (
+                    f"URL scheme {url.scheme!r} is not allowed, "
+                    f"must be one of {self.allowed_url_schemes!r}"
+                )
+                raise ValueError(msg)
+            kwds = filter_options(self.URLOPEN_KWARGS, kwds)
+            request = urllib.request.Request(url.geturl())
+            return cast(ConfigIO, urllib.request.urlopen(request, **kwds))  # noqa: S310
+        if isinstance(self.resource, (int, pathlib.Path)):
+            kwds = filter_options(self.OPEN_KWARGS, kwds)
+            if isinstance(self.resource, int):
+                return cast(
+                    ConfigIO,
+                    # We intentionally do not use the context manager here
+                    # because we do not want to close the file.
+                    # Moreover, we want to allow the file to be opened
+                    # from a file descriptor, not supported by Path().
+                    open(self.resource, **kwds),  # noqa: PTH123, SIM115
+                )
+            return cast(ConfigIO, pathlib.Path(self.resource).open(**kwds))
+        return cast(ConfigIO, self.resource)
+
+    def open_resource_async(self, **kwds: Any) -> AsyncConfigIO:
+        """
+        Open the configuration file asynchronously.
+
+        Parameters
+        ----------
+        **kwds
+            Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The opened resource.
+        """
+        if self.is_url:
+            msg = "Asynchronous URL opening is not supported"
+            raise NotImplementedError(msg)
+        if not AIOFILES_AVAILABLE:
+            msg = (
+                "Aiofiles is not available, cannot open file "
+                "asynchronously (install with `pip install aiofiles`)"
+            )
+            raise RuntimeError(msg)
+        if isinstance(self.resource, (int, pathlib.Path)):
+            kwds = filter_options(self.OPEN_KWARGS, kwds)
+            return aiofiles.open(self.resource, **kwds)
+        raise RuntimeError("cannot open resource asynchronously")
+
+    def processor_open_resource(self, **kwargs: Any) -> ConfigIO:
+        """
+        Called by the processor to open a configuration resource
+        with the reading intention.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the opening routine.
+            For URLs, these are passed to ``urllib.request.urlopen()``.
+            For local files, these are passed to ``builtins.open()``.
+
+        Returns
+        -------
+        The opened resource.
+        """
+        kwargs = self._get_default_kwargs("read", kwargs)
+        return self.open_resource(**kwargs)
+
+    def processor_open_resource_async(self, **kwargs: Any) -> AsyncConfigIO:
+        """
+        Called by the processor to open a configuration resource asynchronously
+        with the reading intention.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the opening routine.
+            For URLs, these are passed to ``urllib.request.urlopen()``.
+            For local files, these are passed to ``builtins.open()``.
+
+        Returns
+        -------
+        The opened resource.
+        """
+        kwargs = self._get_default_kwargs("read", kwargs)
+        return self.open_resource_async(**kwargs)
+
+    def _get_default_kwargs(
+        self,
+        method: Literal["read", "write"],
+        kwargs: dict[str, Any] | None = None,
+    ) -> dict[str, Any]:
+        if not kwargs:
+            kwargs = self.default_kwargs
+        new_kwargs = cast(dict[str, Any], kwargs).copy()
+        if not self.is_url:
+            if method == "read":
+                new_kwargs.setdefault("mode", "rb" if self.uses_binary_data else "r")
+            elif method == "write":
+                new_kwargs.setdefault("mode", "wb" if self.uses_binary_data else "w")
+            else:
+                msg = f"Invalid resource access method: {method!r}"
+                raise ValueError(msg)
+        if self.uses_binary_data:
+            new_kwargs.pop("encoding", None)
+        return new_kwargs
+
+    def read(
+        self,
+        *,
+        config_class: type[ConfigModelT],
+        create_kwargs: dict[str, Any] | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Read the configuration file.
+
+        Parameters
+        ----------
+        config_class
+            The configuration model class to load the configuration into.
+        create_kwargs
+            Keyword arguments to pass to the open method
+            when optionally creating the file.
+        **kwargs
+            Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
+        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
+        try:
+            with self.open_resource(**kwargs) as fp:
+                blob = fp.read()
+        except FileNotFoundError:
+            if self.create_if_missing:
+                defaults = _get_defaults_from_model_class(config_class)
+                blob = self.dump_data(defaults)
+                self.write(blob, **(create_kwargs or {}))
+            else:
+                raise
+        return self.load_into(config_class, blob, **self.load_options)
+
+    def write(self, blob: str | bytes, **kwargs: Any) -> int:
+        """
+        Write the configuration file.
+
+        Parameters
+        ----------
+        blob
+            The string/bytes to write into the resource.
+        kwargs
+            Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
+        with self.open_resource(**kwargs) as fp:
+            return fp.write(cast(str, blob))
+
+    async def read_async(
+        self,
+        *,
+        config_class: type[ConfigModelT],
+        create_kwargs: dict[str, Any] | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Read the configuration file asynchronously.
+
+        Parameters
+        ----------
+        config_class
+            The configuration model class to load the configuration into.
+        create_kwargs
+            Keyword arguments to pass to the open method
+            when optionally creating the file.
+        **kwargs
+            Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
+        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
+        try:
+            async with self.open_resource_async(**kwargs) as fp:
+                blob = await fp.read()
+        except FileNotFoundError:
+            if self.create_if_missing:
+                defaults = _get_defaults_from_model_class(config_class)
+                blob = self.dump_data(defaults)
+                await self.write_async(blob, **(create_kwargs or {}))
+        return await self.async_load_into(config_class, blob, **self.load_options)
+
+    async def write_async(
+        self,
+        blob: str | bytes,
+        **kwargs: Any,
+    ) -> int:
+        """
+        Write the configuration file asynchronously.
+
+        Parameters
+        ----------
+        blob
+            The string/bytes to write into the resource.
+        kwargs
+            Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
+        async with self.open_resource_async(**kwargs) as fp:
+            # Technically those might be also bytes,
+            # todo(bswck): type hint it properly...
+            return await fp.write(cast(str, blob))
+
+    @classmethod
+    def from_directive_context(
+        cls,
+        ctx: DirectiveContext,
+        /,
+        route_separator: str = ":",
+        route_class: type[ConfigRoute] | None = None,
+    ) -> tuple[ConfigAgent[ConfigModelT], ConfigRouteLike | None]:
+        """
+        Create a configuration agent from a preprocessor directive context.
+        Return an optional scope that the context points to.
+
+        Parameters
+        ----------
+        route_class
+        route_separator
+        ctx
+
+        Returns
+        -------
+        The configuration agent.
+        """
+        if route_class is None:
+            route_class = ConfigRoute
+        route: ConfigRouteLike | None = None
+        args: list[Any] = []
+        kwargs: dict[str, Any] = {}
+        if isinstance(ctx.snippet, str):
+            path, _, route = ctx.snippet.partition(route_separator)
+            route = ConfigRoute(
+                route.strip().replace(route_separator, route_class.TOK_DOT)
+            )
+            args.append(path)
+        elif isinstance(ctx.snippet, int):
+            args.append(ctx.snippet)
+        elif is_dict_like(ctx.snippet):
+            kwargs |= ctx.snippet
+        elif is_list_like(ctx.snippet):
+            args += list(ctx.snippet)
+        else:
+            msg = (
+                f"Invalid snippet for the {ctx.directive!r} directive: {ctx.snippet!r}"
+            )
+            raise ValueError(msg)
+        return cls(*args, **kwargs), str(route)
+
+    @classmethod
+    def register_file_extension(
+        cls,
+        file_extension: str,
+        *,
+        parser_name: str,
+    ) -> None:
+        """
+        Register a file extension with the proper anyconfig parser to use.
+
+        Parameters
+        ----------
+        file_extension
+        parser_name
+
+        Returns
+        -------
+        """
+        cls.EXTRA_FILE_EXTENSIONS[file_extension] = parser_name
+
+    def __repr__(self) -> str:
+        resource = self.resource
+        return f"{type(self).__name__}({resource=!r})"
+
+
+def at(
+    mapping: Any,
+    route: ConfigRouteLike,
+    converter_func: Callable[[Any], dict[str, Any]] = _get_object_state,
+    agent: ConfigAgent[ConfigModelT] | None = None,
+) -> Any:
+    """
+    Get an item at a route.
+
+    Parameters
+    ----------
+    mapping
+        The mapping to use.
+    route
+        The route to the item.
+    converter_func
+    agent
+
+    Returns
+    -------
+    The item at the route.
+    """
+    route = ConfigRoute(route)
+    route_here = []
+    scope = converter_func(mapping)
+    try:
+        for part in route:
+            route_here.append(part)
+            scope = converter_func(scope)[part]
+    except KeyError:
+        raise ResourceLookupError(agent, route_here) from None
+    return scope
+
+
+@dataclasses.dataclass(frozen=True)
+class ConfigAt(Generic[ConfigModelT]):
+    """
+    A configuration item at a specific location.
+
+    Attributes
+    ----------
+    owner
+        The configuration model instance.
+    mapping
+        The mapping to use.
+    route
+        The route to the item.
+    """
+
+    owner: ConfigModelT
+    mapping: dict[str, Any] | None
+    route: ConfigRouteLike
+
+    def get(
+        self, route: ConfigRouteLike | None = None, default: Any = Undefined
+    ) -> Any:
+        """
+        Get the value of the item.
+
+        Parameters
+        ----------
+        route
+            The route to the item. If not given, the sole route of this item is used.
+            If given, the route is appended to the sole route of this item.
+        default
+            The default value to return if the item is not found.
+
+        Returns
+        -------
+        The value of the item.
+        """
+        base_route = ConfigRoute(self.route)
+        if route is None:
+            route = base_route
+        else:
+            route = base_route.enter(ConfigRoute(route, allow_empty=True))
+        try:
+            scope = at(self.mapping or self.owner, route)
+        except ResourceLookupError as err:
+            if default is Undefined:
+                route_here = err.route
+                raise ConfigAccessError(self.owner, route_here) from None
+            scope = default
+        return scope
+
+    def update(self, value: Any) -> Any:
+        """
+        Update the value of the item with regard to this item mapping.
+
+        Parameters
+        ----------
+        value
+            The new value.
+
+        Returns
+        -------
+        The updated mapping.
+        """
+        route = list(ConfigRoute(self.route))
+        mapping = self.mapping or self.owner
+        key = route.pop()
+        scope = _get_object_state(mapping)
+        route_here = []
+        try:
+            for part in route:
+                route_here.append(part)
+                scope = _get_object_state(scope[part])
+            scope[key] = value
+        except KeyError:
+            raise ConfigAccessError(self.owner, route_here) from None
+        return mapping
+
+    async def save_async(self, **kwargs: Any) -> int:
+        """
+        Save the configuration asynchronously.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the saving function.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        return await _partial_save_async(self, **kwargs)
+
+    def save(self, **kwargs: Any) -> int:
+        """
+        Save the configuration.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the saving function.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        return _partial_save(self, **kwargs)
+
+    async def reload_async(self, **kwargs: Any) -> Any:
+        """
+        Reload the configuration asynchronously.
+
+        Parameters
+        ----------
+        kwargs
+            Keyword arguments to pass to the reloading function.
+
+        Returns
+        -------
+        The reloaded configuration or its belonging item.
+        """
+        return await _partial_reload_async(self, **kwargs)
+
+    def reload(self, **kwargs: Any) -> Any:
+        """
+        Reload the configuration.
+
+        Parameters
+        ----------
+        kwargs
+            Keyword arguments to pass to the reloading function.
+
+        Returns
+        -------
+        The reloaded configuration or its belonging item.
+        """
+        return _partial_reload(self, **kwargs)
+
+
+def _partial_save(
+    section: ConfigModelT | ConfigAt[ConfigModelT],
+    write_kwargs: dict[str, Any] | None = None,
+    **kwargs: Any,
+) -> int:
+    if isinstance(section, ConfigModel):
+        config = section
+        return config.save(write_kwargs=write_kwargs, **kwargs)
+
+    if write_kwargs is None:
+        write_kwargs = {}
+
+    config = section.owner
+    data = config.initial_state
+    scope = ConfigAt(config, data, section.route)
+    data = scope.update(section.get())
+    context = get_context(config)
+    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
+    result = config.write(blob, **write_kwargs)
+    context.initial_state = data
+    return result
+
+
+async def _partial_save_async(
+    section: ConfigModelT | ConfigAt[ConfigModelT],
+    write_kwargs: dict[str, Any] | None = None,
+    **kwargs: Any,
+) -> int:
+    if isinstance(section, ConfigModel):
+        config = section
+        return await config.save_async(write_kwargs=write_kwargs, **kwargs)
+
+    if write_kwargs is None:
+        write_kwargs = {}
+
+    config = section.owner
+    data = config.initial_state
+    scope = ConfigAt(config, data, section.route)
+    data = scope.update(section.get())
+    context = get_context(config)
+    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
+    result = await config.write_async(blob, **write_kwargs)
+    context.initial_state = data
+    return result
+
+
+def _partial_reload(
+    section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any
+) -> Any:
+    if isinstance(section, ConfigModel):
+        config = section
+        return config.reload()
+
+    config = section.owner
+    context = get_context(config)
+    state = config.__dict__
+    newest = context.agent.read(config_class=type(config), **kwargs)
+    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
+    ConfigAt(config, state, section.route).update(section_data)
+    return section_data
+
+
+async def _partial_reload_async(
+    section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any
+) -> Any:
+    if isinstance(section, ConfigModel):
+        config = section
+        return await config.reload_async()
+
+    config = section.owner
+    context = get_context(config)
+    state = config.__dict__
+    newest = await context.agent.read_async(config_class=type(config), **kwargs)
+    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
+    ConfigAt(config, state, section.route).update(section_data)
+    return section_data
+
+
+class BaseContext(abc.ABC, Generic[ConfigModelT]):
+    """
+    The base class for configuration context.
+    Contexts are used to
+    - store configuration resource information,
+    - link configuration items to the configuration models they belong to,
+    - keep track of the route leading to particular configuration
+      items that are also ConfigModel subclasses.
+
+    Attributes
+    ----------
+    initial_state
+        The initial configuration state.
+
+    """
+
+    initial_state: dict[str, Any]
+    interpolation_namespace: dict[str, Any]
+
+    @abc.abstractmethod
+    def trace_route(self) -> Iterator[str]:
+        """Trace the route to where the configuration subcontext points to."""
+
+    @property
+    def route(self) -> ConfigRoute:
+        """The route to where the configuration subcontext points to."""
+        return ConfigRoute(list(self.trace_route()))
+
+    @overload
+    def enter(self: BaseContext[ConfigModelT], part: None) -> BaseContext[ConfigModelT]:
+        ...
+
+    @overload
+    def enter(self, part: str) -> Subcontext[ConfigModelT]:
+        ...
+
+    def enter(
+        self, part: str | None
+    ) -> Subcontext[ConfigModelT] | BaseContext[ConfigModelT]:
+        """
+        Enter a subcontext.
+
+        Parameters
+        ----------
+        part
+            The name of the item nested in the item this context points to.
+
+        Returns
+        -------
+        The new subcontext.
+        """
+        if part is None:
+            return self
+        return Subcontext(self, part, self.interpolation_namespace.setdefault(part, {}))
+
+    @property
+    @abc.abstractmethod
+    def agent(self) -> ConfigAgent[ConfigModelT]:
+        """The configuration agent responsible for loading and saving."""
+
+    @property
+    @abc.abstractmethod
+    def toplevel_interpolation_namespace(self) -> dict[str, Any]:
+        """Top-level interpolation namespace."""
+
+    @property
+    @abc.abstractmethod
+    def owner(self) -> ConfigModelT | None:
+        """
+        The top-level configuration model instance,
+        holding all adjacent contexts.
+        """
+
+    @property
+    @abc.abstractmethod
+    def at(self) -> ConfigModelT | ConfigAt[ConfigModelT] | None:
+        """
+        The configuration model instance or the configuration item
+        this context points to.
+        """
+
+
+class Context(BaseContext[ConfigModelT], Generic[ConfigModelT]):
+    """
+    The context of a configuration model.
+
+    Parameters
+    ----------
+    agent
+        The configuration resource agent.
+    owner
+        The top-level configuration model instance,
+        holding all belonging subcontexts.
+    """
+
+    _initial_state: dict[str, Any]
+
+    def __init__(
+        self,
+        agent: ConfigAgent[ConfigModelT],
+        owner: ConfigModelT | None = None,
+    ) -> None:
+        self._initial_state = {}
+        self._owner = None
+        self._agent = agent
+        self.interpolation_namespace = {}
+        self.owner = owner
+
+    def trace_route(self) -> Iterator[str]:
+        yield from ()
+
+    @property
+    def agent(self) -> ConfigAgent[ConfigModelT]:
+        return self._agent
+
+    @property
+    def toplevel_interpolation_namespace(self) -> dict[str, Any]:
+        return self.interpolation_namespace
+
+    @property
+    def at(self) -> ConfigModelT | None:
+        return self.owner
+
+    @property
+    def owner(self) -> ConfigModelT | None:
+        return self._owner
+
+    @owner.setter
+    def owner(self, config: ConfigModelT | None) -> None:
+        if config is None:
+            return
+        self._owner = config
+
+    @property
+    def initial_state(self) -> dict[str, Any]:
+        return copy.deepcopy(self._initial_state)
+
+    @initial_state.setter
+    def initial_state(self, initial_state: dict[str, Any]) -> None:
+        self._initial_state = copy.deepcopy(initial_state)
+
+    def __repr__(self) -> str:
+        agent = self.agent
+        return (
+            f"<{type(self).__name__} "
+            f"of {type(self.owner).__name__!r} configuration "
+            f"({agent=})>"
+        )
+
+
+class Subcontext(BaseContext[ConfigModelT], Generic[ConfigModelT]):
+    """
+    The subcontext of a configuration model.
+
+    Parameters
+    ----------
+    parent
+        The parent context.
+    part
+        The name of the item nested in the item the parent context points to.
+    """
+
+    __slots__ = ("_parent", "_part", "_interpolation_namespace")
+
+    def __init__(
+        self,
+        parent: BaseContext[ConfigModelT],
+        part: str,
+        interpolation_namespace: dict[str, Any],
+    ) -> None:
+        self._parent = parent
+        self._part = part
+        self.interpolation_namespace = interpolation_namespace
+
+    @property
+    def agent(self) -> ConfigAgent[ConfigModelT]:
+        return self._parent.agent
+
+    @property
+    def toplevel_interpolation_namespace(self) -> dict[str, Any]:
+        return self._parent.toplevel_interpolation_namespace
+
+    def trace_route(self) -> Iterator[str]:
+        yield from self._parent.trace_route()
+        yield self._part
+
+    @property
+    def at(self) -> ConfigAt[ConfigModelT]:
+        if self.owner is None:
+            msg = "Cannot get at() of a model without parent model"
+            raise ValueError(msg)
+        return ConfigAt(self.owner, None, self.route)
+
+    @property
+    def owner(self) -> ConfigModelT | None:
+        return self._parent.owner
+
+    @property
+    def initial_state(self) -> dict[str, Any]:
+        return self._parent.initial_state
+
+    @initial_state.setter
+    def initial_state(self, value: dict[str, Any]) -> None:
+        data = self._parent.initial_state
+        data[self._part] = copy.deepcopy(value)
+        self._parent.initial_state = data
+
+    def __repr__(self) -> str:
+        agent = self.agent
+        route = self.route
+        return (
+            f"<{type(self).__name__} "
+            f"of {type(self.owner).__name__ + '.' + str(route)!r} configuration "
+            f"({agent=})>"
+        )
+
+
+def get_context(config: ConfigModelT) -> BaseContext[ConfigModelT]:
+    """
+    Get the context of the configuration model.
+
+    Parameters
+    ----------
+    config
+        The configuration model instance.
+
+    Returns
+    -------
+    The context of the configuration model.
+    """
+    context = get_context_or_none(config)
+    if context is None:
+        raise RuntimeError(
+            "This model is either inside a list "
+            "or was not loaded by a configuration agent."
+        )
+    return context
+
+
+def get_context_or_none(config: ConfigModelT) -> BaseContext[ConfigModelT] | None:
+    """
+    Get the context of the configuration model safely.
+
+    Parameters
+    ----------
+    config
+        The configuration model instance.
+
+    Returns
+    -------
+    The context of the configuration model.
+    """
+    return cast(
+        Optional[BaseContext[ConfigModelT]], getattr(config, LOCAL).get(current_context)
+    )
+
+
+# noinspection PyUnusedLocal
+@make_generic_validator
+def _common_field_validator(
+    cls: type[ConfigModelT],
+    v: Any,
+    values: dict[str, Any],
+    field: pydantic.fields.ModelField,
+    config: pydantic.BaseConfig,
+) -> Any:
+    post_hook_value = field_hook(field.outer_type_, v)
+    disallow_interpolation = getattr(config, "disallow_interpolation", False)
+    disallowed_interpolation_fields = set()
+
+    interpolation_tracker = current_interpolation_tracker.get()
+
+    if interpolation_tracker is None:
+        interpolation_tracker = {}
+        current_interpolation_tracker.set(interpolation_tracker)
+
+    if not isinstance(disallow_interpolation, bool):
+        disallowed_interpolation_fields = set(disallow_interpolation)
+    if (
+        field.field_info.extra.get("interpolate", True)
+        and field.alias not in disallowed_interpolation_fields
+    ):
+        old_value = post_hook_value
+        try:
+            interpolated = interpolate(
+                post_hook_value,
+                cls,
+                values.copy(),
+                field.outer_type_,
+            )
+        except InterpolationError as err:
+            err.message += f" (encountered in {cls.__qualname__}.{field.alias})"
+            raise
+
+        new_value = field_hook(field.outer_type_, interpolated)
+        if old_value != new_value:
+            interpolation_tracker[field.alias] = (old_value, copy.copy(new_value))
+        post_hook_value = new_value
+
+    return post_hook_value
+
+
+def _json_encoder(model_encoder: Callable[..., Any], value: Any, **kwargs: Any) -> Any:
+    initial_state_type = type(value)
+    converted_value = export_hook(value)
+    if isinstance(converted_value, initial_state_type):
+        return model_encoder(value, **kwargs)
+    return converted_value
+
+
+class ConfigModelMetaclass(ModelMetaclass):
+    def __new__(
+        cls,
+        name: str,
+        bases: tuple[type, ...],
+        namespace: dict[str, Any],
+        **kwargs: Any,
+    ) -> type:
+        namespace |= dict.fromkeys(
+            (EXPORT, CONTEXT, LOCAL, TOKEN, MODULE), pydantic.PrivateAttr()
+        ) | {INTERPOLATION_TRACKER: pydantic.PrivateAttr(default_factory=dict)}
+
+        if namespace.get(INTERPOLATION_INCLUSIONS) is None:
+            namespace[INTERPOLATION_INCLUSIONS] = {}
+
+        if namespace.get(INTERPOLATOR) is None:
+            namespace[INTERPOLATOR] = BaseInterpolator()
+
+        if namespace.get(EVALUATION_ENGINE) is None:
+            namespace[EVALUATION_ENGINE] = BaseEvaluationEngine()
+
+        if kwargs.pop("root", None):
+            return type.__new__(cls, name, bases, namespace, **kwargs)
+
+        model = super().__new__(cls, name, bases, namespace, **kwargs)
+        for field in model.__fields__.values():
+            if field.pre_validators is None:
+                field.pre_validators = []
+            field.pre_validators[:] = [_common_field_validator, *field.pre_validators]
+            if type(field.outer_type_) is ConfigModelMetaclass:
+                validator = make_generic_validator(
+                    field.outer_type_.__field_setup__  # type: ignore[attr-defined]
+                )
+                field.pre_validators[:] = [
+                    _common_field_validator,
+                    validator,
+                    *field.pre_validators,
+                ]
+        model_encoder = model.__json_encoder__
+        model.__json_encoder__ = functools.partial(_json_encoder, model_encoder)
+        return cast(type, model)
+
+
+class ConfigMeta(pydantic.BaseSettings.Config):
+    """
+    Meta-configuration for configuration models.
+
+    See https://docs.pydantic.dev/latest/usage/model_config/ for more information
+    on model configurations.
+
+    Attributes
+    ----------
+    resource
+        The configuration resource to read from/write to.
+
+        If a string, it will be interpreted as a path to a file.
+
+    parser_name
+        The anyconfig parser to use.
+
+    autoupdate_forward_refs
+        Whether to automatically update forward references
+        when `ConfigModel.load()` or `ConfigModel.load_async()`
+        methods are called. For convenience, defaults to `True`.
+
+    And all other attributes from `pydantic.BaseSettings.Config`.
+    """
+
+    resource: ConfigAgent[ConfigModel] | RawResourceT | None = None
+    parser_name: str | None = None
+    validate_assignment: bool = True
+    autoupdate_forward_refs: bool = True
+
+    Extra = pydantic.Extra
+
+
+class ConfigModel(
+    pydantic.BaseSettings,
+    metaclass=ConfigModelMetaclass,
+    root=True,
+):
+    """The base class for configuration models."""
+
+    __config__ = ConfigMeta
+
+    module_wrapper_class: ClassVar[type[ConfigModule[ConfigModel]]] = ConfigModule
+
+    def __init__(self, **kwargs: Any) -> None:
+        # Set private attributes via the constructor
+        # to allow preprocessor-related instances to exist.
+        for private_attr in self.__private_attributes__:
+            value = kwargs.pop(private_attr, Undefined)
+            if value is not Undefined:
+                if private_attr == CONTEXT:
+                    context = current_context.get()
+                    if context:
+                        value = context
+                    current_context.set(value)
+                object.__setattr__(self, private_attr, value)
+        super().__init__(**kwargs)
+
+    def __deepcopy__(
+        self: ConfigModelT, memodict: dict[Any, Any] | None = None
+    ) -> ConfigModelT:
+        state = dict(self._iter(to_dict=False))
+        state.pop(LOCAL, None)
+        state.pop(TOKEN, None)
+        clone = copy.deepcopy(state)
+        return type(self).parse_obj(
+            {
+                field.alias: clone[field_name]
+                for field_name, field in self.__fields__.items()
+            }
+        )
+
+    def __setattr__(self, key: str, value: Any) -> None:
+        getattr(self, LOCAL).run(super().__setattr__, key, value)
+
+    def _init_private_attributes(self) -> None:
+        super()._init_private_attributes()
+        local = contextvars.copy_context()
+        object.__setattr__(self, LOCAL, local)
+        tok = getattr(self, TOKEN, None)
+        if tok:
+            context = current_context.get()
+            if context is not None:
+                context.interpolation_namespace |= self.dict()
+            current_context.reset(tok)
+
+    def export(self, **kwargs: Any) -> dict[str, Any]:
+        """
+        Export the configuration model.
+
+        Returns
+        -------
+        The exported configuration model.
+        """
+        _exporting.set(True)  # noqa: FBT003
+        return detached_context_run(self.dict, **kwargs)
+
+    async def export_async(self, **kwargs: Any) -> dict[str, Any]:
+        """
+        Export the configuration model.
+
+        Returns
+        -------
+        The exported configuration model.
+        """
+        _exporting.set(True)  # noqa: FBT003
+        return await detached_context_await(self.dict_async, **kwargs)
+
+    async def dict_async(self, **kwargs: Any) -> dict[str, Any]:
+        """
+        Get the dictionary representation of the configuration model.
+
+        Returns
+        -------
+        The dictionary representation of the configuration model.
+        """
+        return dict(await self._iter_async(to_dict=True, **kwargs))
+
+    # noinspection PyShadowingNames
+    async def json_async(  # noqa: PLR0913
+        self,
+        include: IncludeExcludeT = None,
+        exclude: IncludeExcludeT = None,
+        *,
+        by_alias: bool = False,
+        exclude_unset: bool = False,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        encoder: Callable[[Any], Any] | None = None,
+        models_as_dict: bool = True,
+        **dumps_kwargs: Any,
+    ) -> str:
+        encoder = cast(Callable[[Any], Any], encoder or self.__json_encoder__)
+        data = dict(
+            await self._iter_async(
+                to_dict=models_as_dict,
+                by_alias=by_alias,
+                include=include,
+                exclude=exclude,
+                exclude_unset=exclude_unset,
+                exclude_defaults=exclude_defaults,
+                exclude_none=exclude_none,
+            )
+        )
+        if self.__custom_root_type__:
+            data = data[ROOT_KEY]
+        return self.__config__.json_dumps(data, default=encoder, **dumps_kwargs)
+
+    def _iter(  # type: ignore[override]
+        self, **kwargs: Any
+    ) -> Iterator[tuple[str, Any]]:
+        if kwargs.get("to_dict", False) and _exporting.get():
+            state: dict[str, Any] = {}
+            for key, value in super()._iter(**kwargs):
+                state |= [self._export_iter_hook(key, value)]
+            metadata = getattr(self, EXPORT, None)
+            if metadata:
+                context = get_context(self)
+                context.agent.processor_class.export(state, metadata=metadata)
+            yield from state.items()
+        else:
+            yield from super()._iter(**kwargs)
+
+    async def _iter_async(self, **kwargs: Any) -> Iterator[tuple[str, Any]]:
+        if kwargs.get("to_dict", False) and _exporting.get():
+            state: dict[str, Any] = {}
+            for key, value in super()._iter(**kwargs):
+                state |= [self._export_iter_hook(key, value)]
+            metadata = getattr(self, EXPORT, None)
+            if metadata:
+                context = get_context(self)
+                await context.agent.processor_class.export_async(
+                    state, metadata=metadata
+                )
+            return ((key, value) for key, value in state.items())
+        return super()._iter(**kwargs)
+
+    def _export_iter_hook(
+        self,
+        key: str,
+        value: Any,
+    ) -> tuple[str, Any]:
+        interpolation_tracker = getattr(self, LOCAL).get(current_interpolation_tracker)
+        field = self.__fields__.get(key)
+        actual_key = field.alias if field else key
+        if interpolation_tracker:
+            interpolation_track = interpolation_tracker.get(actual_key)
+            if interpolation_track:
+                old_value, new_value = interpolation_track
+                # if value != new_value:
+                #     raise InterpolationError(
+                #         f"Cannot restore the value of {actual_key!r} "
+                #         "before interpolation."
+                #     )
+                value = old_value
+        return actual_key, value
+
+    @classmethod
+    @no_type_check
+    def _get_value(cls, value: Any, *, to_dict: bool, **kwds: Any) -> Any:
+        if _exporting.get():
+            exporter = export_model.dispatch(type(value))
+            if (
+                isinstance(value, BaseModel)
+                or exporter != export_model.dispatch(object)
+            ) and to_dict:
+                value_dict = export_model(value, **kwds)
+                if ROOT_KEY in value_dict:
+                    return value_dict[ROOT_KEY]
+                return value_dict
+        return super()._get_value(value, to_dict=to_dict, **kwds)
+
+    @classmethod
+    def _resolve_agent(
+        cls,
+        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
+        *,
+        create_if_missing: bool | None = None,
+        parser_name: str | None = None,
+    ) -> ConfigAgent[ConfigModelT]:
+        if resource is None:
+            resource = getattr(cls.__config__, "resource", None)
+        if resource is None:
+            raise ValueError("No resource specified")
+        if parser_name is None:
+            parser_name = getattr(cls.__config__, "parser_name", None)
+        agent: ConfigAgent[ConfigModelT]
+        if isinstance(resource, ConfigAgent):
+            agent = resource
+        else:
+            agent = ConfigAgent(
+                resource,
+                parser_name=parser_name,
+            )
+        if create_if_missing is not None:
+            agent.create_if_missing = create_if_missing
+        if parser_name is not None:
+            agent.parser_name = cast(str, parser_name)
+        return agent
+
+    @property
+    def initial_state(self) -> dict[str, Any]:
+        """
+        The initial configuration state.
+
+        It is a copy of the configuration state
+        at the last time of loading, reloading or saving.
+        """
+        return get_context(self).initial_state
+
+    def at(
+        self: ConfigModelT,
+        route: ConfigRouteLike | None = None,
+    ) -> ConfigModelT | ConfigAt[ConfigModelT]:
+        """
+        Lazily point to a specific item in the configuration.
+
+        Parameters
+        ----------
+        route
+            The access route to the item in this configuration.
+            If None, the whole configuration is returned.
+
+        Returns
+        -------
+        The configuration accessor.
+        """
+        if route is None:
+            context = get_context_or_none(self)
+            self_at = None
+            if context is not None:
+                self_at = context.at
+            if self_at is not None:
+                return self_at
+            return self
+        return ConfigAt(self, None, route)
+
+    @overload
+    def get(self: ConfigModelT, route: None = None, default: Any = ...) -> ConfigModelT:
+        ...
+
+    @overload
+    def get(
+        self: ConfigModelT, route: ConfigRouteLike = ..., default: Any = ...
+    ) -> Any:
+        ...
+
+    def get(
+        self, route: ConfigRouteLike | None = None, default: Any = Undefined
+    ) -> Any:
+        """
+        Get a value from the configuration.
+
+        Parameters
+        ----------
+        route
+            Route to access the item. If None, the whole configuration is returned.
+        default
+        """
+        if route is None:
+            return self
+        return self.at(route).get(default=default)
+
+    def update(self, kwargs: dict[str, Any]) -> None:
+        """
+        Update the configuration with new values, in-place.
+
+        Parameters
+        ----------
+        kwargs
+            The new values to update the configuration with.
+
+        Returns
+        -------
+        None
+        """
+        # Crucial difference to self.__dict__.update():
+        # self.__dict__.update() would not trigger the validation
+        # of the new values.
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+    def rollback(self) -> None:
+        """
+        Rollback the configuration to its initial state.
+
+        Returns
+        -------
+        None
+        """
+        context = get_context(self)
+        self.__dict__.update(context.initial_state)
+
+    @classmethod
+    def load(
+        cls: type[ConfigModelT],
+        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
+        *,
+        create_if_missing: bool | None = None,
+        parser_name: str | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Load the configuration file.
+        To reload the configuration, use the `reload()` method.
+
+        Parameters
+        ----------
+        resource
+            The configuration resource to read from/write to.
+        parser_name
+            The anyconfig parser to use.
+        create_if_missing
+            Whether to create the configuration file if it does not exist.
+        **kwargs
+            Keyword arguments to pass to the read method.
+
+        Returns
+        -------
+        self
+        """
+        agent = cls._resolve_agent(
+            resource,
+            parser_name=parser_name,
+            create_if_missing=create_if_missing,
+        )
+        current_context.set(Context(agent))
+        local = contextvars.copy_context()
+        if getattr(
+            cls.__config__,
+            "autoupdate_forward_refs",
+            ConfigMeta.autoupdate_forward_refs,
+        ):
+            cls.update_forward_refs()
+        config = local.run(agent.read, config_class=cls, **kwargs)
+        object.__setattr__(config, LOCAL, local)
+        context = cast(Context[ConfigModelT], local.get(current_context))
+        context.owner = config
+        context.initial_state = config.__dict__
+        return config
+
+    @classmethod
+    async def load_async(
+        cls: type[ConfigModelT],
+        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
+        *,
+        parser_name: str | None = None,
+        create_if_missing: bool | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Load the configuration file asynchronously.
+        To reload the configuration, use the `reload_async()` method.
+
+        Parameters
+        ----------
+        resource
+            The configuration resource.
+        parser_name
+            The anyconfig parser to use.
+        create_if_missing
+            Whether to create the configuration file if it does not exist.
+        **kwargs
+            Keyword arguments to pass to the read method.
+
+        Returns
+        -------
+        self
+        """
+        agent = cls._resolve_agent(
+            resource, create_if_missing=create_if_missing, parser_name=parser_name
+        )
+        current_context.set(Context(agent))
+        local = contextvars.copy_context()
+        if getattr(
+            cls.__config__,
+            "autoupdate_forward_refs",
+            ConfigMeta.autoupdate_forward_refs,
+        ):
+            cls.update_forward_refs()
+        reader = local.run(
+            asyncio.create_task, agent.read_async(config_class=cls, **kwargs)
+        )
+        config = await reader
+        object.__setattr__(config, LOCAL, local)
+        context = cast(Context[ConfigModelT], local.get(current_context))
+        context.owner = config
+        return config
+
+    def reload(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
+        """
+        Reload the configuration file.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the read method.
+
+        Returns
+        -------
+        self
+        """
+        try:
+            context = get_context(self)
+        except RuntimeError:
+            wrapped_module = getattr(self, MODULE, None)
+            if wrapped_module is None:
+                raise
+            importlib.reload(wrapped_module)
+            self.update(
+                {
+                    key: value
+                    for key, value in wrapped_module.__dict__.items()
+                    if key in self.__fields__
+                }
+            )
+            return self
+        current_context.set(get_context(context.owner))
+        if context.owner is self:
+            changed = context.agent.read(config_class=type(self), **kwargs)
+        else:
+            changed = _partial_reload(cast(ConfigModelT, context.at), **kwargs)
+        state = changed.__dict__
+        context.initial_state = state
+        self.update(state)
+        return self
+
+    async def reload_async(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
+        """
+        Reload the configuration file asynchronously.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the read method.
+
+        Returns
+        -------
+        self
+        """
+        context = get_context(self)
+        current_context.set(get_context(context.owner))
+        if context.owner is self:
+            changed = await context.agent.read_async(config_class=type(self), **kwargs)
+        else:
+            changed = await _partial_reload_async(
+                cast(ConfigAt[ConfigModelT], context.at), **kwargs
+            )
+        state = changed.__dict__
+        context.initial_state = state
+        self.update(state)
+        return self
+
+    def save(
+        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
+    ) -> int:
+        """
+        Save the configuration to the configuration file.
+
+        Parameters
+        ----------
+        write_kwargs
+            Keyword arguments to pass to the write method.
+        **kwargs
+            Keyword arguments to pass to the dumping method.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        context = get_context(self)
+        if context.owner is self:
+            if write_kwargs is None:
+                write_kwargs = {}
+            blob = context.agent.dump_config(self, **kwargs)
+            result = self.write(blob, **write_kwargs)
+            context.initial_state = self.__dict__
+            return result
+        return _partial_save(
+            cast(ConfigAt[ConfigModelT], context.at),
+            write_kwargs=write_kwargs,
+            **kwargs,
+        )
+
+    async def save_async(
+        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
+    ) -> int:
+        """
+        Save the configuration to the configuration file asynchronously.
+
+        Parameters
+        ----------
+        write_kwargs
+            Keyword arguments to pass to the write method.
+        **kwargs
+            Keyword arguments to pass to the dumping method.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        context = get_context(self)
+        if context.owner is self:
+            if write_kwargs is None:
+                write_kwargs = {}
+            _exporting.set(True)  # noqa: FBT003
+            blob = await context.agent.dump_config_async(self, **kwargs)
+            result = await self.write_async(blob, **write_kwargs)
+            context.initial_state = self.__dict__
+            return result
+        return await _partial_save_async(
+            cast(ConfigAt[ConfigModelT], context.at),
+            write_kwargs=write_kwargs,
+            **kwargs,
+        )
+
+    def write(self, blob: str | bytes, **kwargs: Any) -> int:
+        """
+        Overwrite the configuration file with the given string or bytes.
+
+        Parameters
+        ----------
+        blob
+            The blob to write to the configuration file.
+        **kwargs
+            Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        context = get_context(self)
+        if context.agent.is_url:
+            msg = "Writing to URLs is not yet supported"
+            raise NotImplementedError(msg)
+        return context.agent.write(blob, **kwargs)
+
+    async def write_async(self, blob: str | bytes, **kwargs: Any) -> int:
+        """
+        Overwrite the configuration file asynchronously with the given string or bytes.
+
+        Parameters
+        ----------
+        blob
+            The blob to write to the configuration file.
+        **kwargs
+            Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        context = get_context(self)
+        if context.agent.is_url:
+            msg = "Saving to URLs is not yet supported"
+            raise NotImplementedError(msg)
+        return await context.agent.write_async(blob, **kwargs)
+
+    @classmethod
+    def _evaluate_interpolation_namespaces(cls) -> dict[str | None, dict[str, Any]]:
+        inclusions = getattr(cls, INTERPOLATION_INCLUSIONS)
+        return {
+            namespace_id: evaluate_namespace()
+            for namespace_id, evaluate_namespace in inclusions.items()
+        }
+
+    @classmethod
+    def _evaluate_interpolation_expression(
+        cls,
+        expression: str,
+        *,
+        result_namespace: dict[str, Any],
+        namespaces: dict[str | None, dict[str, Any]],
+        closest_namespace: dict[str, Any],
+        target_type: type[Any],
+    ) -> Any:
+        evaluation_engine: BaseEvaluationEngine = getattr(cls, EVALUATION_ENGINE)
+        return evaluation_engine.evaluate_expression(
+            expression=expression,
+            result_namespace=result_namespace,
+            namespaces=namespaces,
+            closest_namespace=closest_namespace,
+            target_type=target_type,
+        )
+
+    @classmethod
+    def wrap_module(
+        cls: type[ConfigModelT],
+        module_name: str | types.ModuleType,
+        /,
+        **values: Any,
+    ) -> ConfigModelT:
+        module_vars = None
+        if isinstance(module_name, str):
+            module_name = module_name
+            if module_name not in sys.modules:
+                package = None
+                if module_name.startswith("."):
+                    current_frame = inspect.currentframe()
+                    assert current_frame is not None
+                    frame_back = current_frame.f_back
+                    assert frame_back is not None
+                    package = frame_back.f_globals["__package__"]
+                module_vars = vars(
+                    importlib.import_module(module_name, package=package)
+                )
+        else:
+            module_name = module_name.__name__
+        config_module = cls.module_wrapper_class.wrap_module(
+            module_name, cls, module_vars, **values
+        )
+        return cast(ConfigModelT, config_module.get_model())
+
+    @classmethod
+    def wrap_this_module(
+        cls: type[ConfigModelT],
+        **values: Any,
+    ) -> ConfigModelT:
+        current_frame = inspect.currentframe()
+        assert current_frame is not None
+        frame_back = current_frame.f_back
+        assert frame_back is not None
+        return cls.wrap_module(
+            frame_back.f_globals["__name__"],
+            **values
+        )
+
+    @classmethod
+    def get_interpolation_namespace(
+        cls,
+        expressions: set[str],
+        closest_namespace: dict[str, Any],
+        target_type: type[Any],
+    ) -> dict[str, Any]:
+        """Get the interpolation namespace according to occuring expressions."""
+        context = current_context.get()
+        result_namespace: dict[str, Any] = {}
+
+        namespaces = cls._evaluate_interpolation_namespaces()
+        if context is not None:
+            namespaces.setdefault(None, {}).update(
+                context.toplevel_interpolation_namespace
+            )
+
+        for expression in expressions:
+            value = cls._evaluate_interpolation_expression(
+                expression=expression,
+                result_namespace=result_namespace,
+                namespaces=namespaces,
+                closest_namespace=closest_namespace,
+                target_type=target_type,
+            )
+            result_namespace[expression] = value
+
+        return result_namespace
+
+    @classmethod
+    def __field_setup__(cls, value: dict[str, Any], field: ModelField) -> Any:
+        """
+        Called when this configuration model is being initialized as a field
+        of some other configuration model.
+        """
+        context = current_context.get()
+        if context is not None:
+            subcontext = context.enter(field.name)
+            tok = current_context.set(subcontext)
+            return _get_object_state(value) | {
+                TOKEN: tok,
+                LOCAL: contextvars.copy_context(),
+            }
+        return value
+
+    if not TYPE_CHECKING:
+        load = detached_context_function(load)
+        load_async = detached_context_function(load_async)
+        reload = detached_context_function(reload)
+        reload_async = detached_context_function(reload_async)
+        save = detached_context_function(save)
+        save_async = detached_context_function(save_async)
+        export = detached_context_function(export)
+        export_async = detached_context_function(export_async)
+
+
+setattr(ConfigModel, INTERPOLATION_INCLUSIONS, None)
+include.register(ConfigModel, include_const)
+
+if os.getenv("CONFIGZEN_SETUP") != "0":
+    importlib.import_module("._setup", package=__package__)
```

### Comparing `configzen-0.5.6/configzen/decorators.py` & `configzen-0.6.0/configzen/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-from __future__ import annotations
-
-import contextlib
-import functools
-from collections.abc import Callable, Iterator, Coroutine
-from typing import TYPE_CHECKING, Any, cast, overload
-
-from configzen.config import export_hook, export_model, export_model_async, field_hook
-
-if TYPE_CHECKING:
-    from configzen.typedefs import ConfigModelT, T
-
-__all__ = (
-    "with_exporter",
-    "with_async_exporter",
-    "with_field_hook",
-    "with_export_hook",
-)
-
-
-@overload
-def with_export_hook(
-    func: Callable[[T], Any],
-    cls: None = None,
-) -> functools.partial[type[T]]:
-    ...
-
-
-@overload
-def with_export_hook(
-    func: Callable[[T], Any],
-    cls: type[T],
-) -> type[T]:
-    ...
-
-
-def with_export_hook(
-    func: Callable[[T], Any], cls: type[T] | None = None
-) -> type[T] | functools.partial[type[T]]:
-    """
-    Register a pre-serialization converter function for a type.
-
-    Parameters
-    ----------
-    func
-        The converter function.
-
-    cls
-        The type to register the converter for.
-        Optional for the decoration syntax.
-
-    Returns
-    -------
-    The conversion result class.
-
-    Usage
-    -----
-    .. code-block:: python
-
-        @with_export_hook(converter_func)
-        class MyClass:
-            ...
-
-    """
-    if cls is None:
-        return functools.partial(with_export_hook, func)
-
-    export_hook.register(cls, func)
-
-    if not hasattr(cls, "__get_validators__"):
-
-        def validator_gen() -> Iterator[Callable[[Any], Any]]:
-            hook_func = field_hook.dispatch(cls)
-            yield lambda value: hook_func(cls, value)
-
-        with contextlib.suppress(TypeError):
-            cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
-
-    return cls
-
-
-@overload
-def with_field_hook(
-    func: Callable[[type[T], Any], T],
-    cls: type[T],
-) -> type[T]:
-    ...
-
-
-@overload
-def with_field_hook(
-    func: Callable[[type[T], Any], T],
-    cls: None = None,
-) -> functools.partial[type[T]]:
-    ...
-
-
-def with_field_hook(
-    func: Callable[[type[T], Any], T], cls: type[T] | None = None
-) -> type[T] | functools.partial[type[T]]:
-    """
-    Register a field hook for a type.
-
-    Parameters
-    ----------
-    func
-        The loader function.
-    cls
-        The type to register the loader for.
-
-    Returns
-    -------
-    The loading result class.
-    """
-
-    if cls is None:
-        return functools.partial(with_field_hook, func)
-
-    field_hook.register(cls, func)
-    return cls
-
-
-def with_exporter(
-    func: Callable[[ConfigModelT], Any] | None = None,
-    cls: type[ConfigModelT] | None = None,
-    **predefined_kwargs: Any,
-) -> type[ConfigModelT] | Any:
-    """
-    Register a custom exporter for a configuration model class.
-
-    Parameters
-    ----------
-    func
-        The exporter function.
-    cls
-        The type to register the exporter for.
-    """
-    if cls is None:
-        return functools.partial(with_exporter, func)
-
-    if func and predefined_kwargs:
-        raise NotImplementedError(
-            "specifying both a function and predefined kwargs is not supported"
-        )
-
-    if func is None:
-
-        def func(obj: Any, **kwargs: Any) -> Any:
-            kwargs |= predefined_kwargs
-            return obj.export(**kwargs)
-
-        export_model.register(cls, func)
-
-        if export_model_async.dispatch(cls) is export_model_async:
-
-            async def default_async_func(obj: Any, **kwargs: Any) -> Any:
-                kwargs |= predefined_kwargs
-                return await obj.export_async(**kwargs)
-
-            export_model_async.register(cls, default_async_func)
-    else:
-        export_model.register(cls, func)
-        if export_model_async.dispatch(cls) is export_model_async:
-
-            async def default_async_func(obj: Any, **kwargs: Any) -> Any:
-                nonlocal func
-                if TYPE_CHECKING:
-                    func = cast(Callable[..., dict[str, Any]], func)
-
-                return func(obj, **kwargs)
-
-            export_model_async.register(cls, default_async_func)
-    return cls
-
-
-def with_async_exporter(
-    func: Callable[[ConfigModelT], Coroutine[Any, Any, Any]] | None = None,
-    cls: type[ConfigModelT] | None = None,
-    **predefined_kwargs: Any,
-) -> type[ConfigModelT] | Any:
-    """
-    Register a custom exporter for a configuration model class.
-
-    Parameters
-    ----------
-    func
-        The exporter function.
-    cls
-        The type to register the exporter for.
-    """
-    if cls is None:
-        return functools.partial(with_exporter, func)
-
-    if func and predefined_kwargs:
-        raise NotImplementedError(
-            "specifying both a function and default kwargs is not supported"
-        )
-
-    if func is None:
-
-        async def default_async_func(obj: Any, **kwargs: Any) -> Any:
-            kwargs |= predefined_kwargs
-            return await obj.export_async(**kwargs)
-
-        export_model_async.register(cls, default_async_func)
-    else:
-        export_model_async.register(cls, func)
-    return cls
+from __future__ import annotations
+
+import contextlib
+import functools
+from collections.abc import Callable, Iterator, Coroutine
+from typing import TYPE_CHECKING, Any, cast, overload
+
+from configzen.model import export_hook, export_model, export_model_async, field_hook
+
+if TYPE_CHECKING:
+    from configzen.typedefs import ConfigModelT, T
+
+__all__ = (
+    "with_exporter",
+    "with_async_exporter",
+    "with_field_hook",
+    "with_export_hook",
+)
+
+
+@overload
+def with_export_hook(
+    func: Callable[[T], Any],
+    cls: None = None,
+) -> functools.partial[type[T]]:
+    ...
+
+
+@overload
+def with_export_hook(
+    func: Callable[[T], Any],
+    cls: type[T],
+) -> type[T]:
+    ...
+
+
+def with_export_hook(
+    func: Callable[[T], Any], cls: type[T] | None = None
+) -> type[T] | functools.partial[type[T]]:
+    """
+    Register a pre-serialization converter function for a type.
+
+    Parameters
+    ----------
+    func
+        The converter function.
+
+    cls
+        The type to register the converter for.
+        Optional for the decoration syntax.
+
+    Returns
+    -------
+    The conversion result class.
+
+    Usage
+    -----
+    .. code-block:: python
+
+        @with_export_hook(converter_func)
+        class MyClass:
+            ...
+
+    """
+    if cls is None:
+        return functools.partial(with_export_hook, func)
+
+    export_hook.register(cls, func)
+
+    if not hasattr(cls, "__get_validators__"):
+
+        def validator_gen() -> Iterator[Callable[[Any], Any]]:
+            hook_func = field_hook.dispatch(cls)
+            yield lambda value: hook_func(cls, value)
+
+        with contextlib.suppress(TypeError):
+            cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
+
+    return cls
+
+
+@overload
+def with_field_hook(
+    func: Callable[[type[T], Any], T],
+    cls: type[T],
+) -> type[T]:
+    ...
+
+
+@overload
+def with_field_hook(
+    func: Callable[[type[T], Any], T],
+    cls: None = None,
+) -> functools.partial[type[T]]:
+    ...
+
+
+def with_field_hook(
+    func: Callable[[type[T], Any], T], cls: type[T] | None = None
+) -> type[T] | functools.partial[type[T]]:
+    """
+    Register a field hook for a type.
+
+    Parameters
+    ----------
+    func
+        The loader function.
+    cls
+        The type to register the loader for.
+
+    Returns
+    -------
+    The loading result class.
+    """
+
+    if cls is None:
+        return functools.partial(with_field_hook, func)
+
+    field_hook.register(cls, func)
+    return cls
+
+
+def with_exporter(
+    func: Callable[[ConfigModelT], Any] | None = None,
+    cls: type[ConfigModelT] | None = None,
+    **predefined_kwargs: Any,
+) -> type[ConfigModelT] | Any:
+    """
+    Register a custom exporter for a configuration model class.
+
+    Parameters
+    ----------
+    func
+        The exporter function.
+    cls
+        The type to register the exporter for.
+    """
+    if cls is None:
+        return functools.partial(with_exporter, func)
+
+    if func and predefined_kwargs:
+        raise NotImplementedError(
+            "specifying both a function and predefined kwargs is not supported"
+        )
+
+    if func is None:
+
+        def func(obj: Any, **kwargs: Any) -> Any:
+            kwargs |= predefined_kwargs
+            return obj.export(**kwargs)
+
+        export_model.register(cls, func)
+
+        if export_model_async.dispatch(cls) is export_model_async:
+
+            async def default_async_func(obj: Any, **kwargs: Any) -> Any:
+                kwargs |= predefined_kwargs
+                return await obj.export_async(**kwargs)
+
+            export_model_async.register(cls, default_async_func)
+    else:
+        export_model.register(cls, func)
+        if export_model_async.dispatch(cls) is export_model_async:
+
+            async def default_async_func(obj: Any, **kwargs: Any) -> Any:
+                nonlocal func
+                if TYPE_CHECKING:
+                    func = cast(Callable[..., dict[str, Any]], func)
+
+                return func(obj, **kwargs)
+
+            export_model_async.register(cls, default_async_func)
+    return cls
+
+
+def with_async_exporter(
+    func: Callable[[ConfigModelT], Coroutine[Any, Any, Any]] | None = None,
+    cls: type[ConfigModelT] | None = None,
+    **predefined_kwargs: Any,
+) -> type[ConfigModelT] | Any:
+    """
+    Register a custom exporter for a configuration model class.
+
+    Parameters
+    ----------
+    func
+        The exporter function.
+    cls
+        The type to register the exporter for.
+    """
+    if cls is None:
+        return functools.partial(with_exporter, func)
+
+    if func and predefined_kwargs:
+        raise NotImplementedError(
+            "specifying both a function and default kwargs is not supported"
+        )
+
+    if func is None:
+
+        async def default_async_func(obj: Any, **kwargs: Any) -> Any:
+            kwargs |= predefined_kwargs
+            return await obj.export_async(**kwargs)
+
+        export_model_async.register(cls, default_async_func)
+    else:
+        export_model_async.register(cls, func)
+    return cls
```

### Comparing `configzen-0.5.6/configzen/errors.py` & `configzen-0.6.0/configzen/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-"""This module contains all the custom errors raised by _configzen_."""
-
-from __future__ import annotations
-
-import contextlib
-from collections.abc import Iterator
-from typing import TYPE_CHECKING, Any
-
-if TYPE_CHECKING:
-    from configzen.config import ConfigAgent
-    from configzen.typedefs import ConfigModelT
-
-
-class ConfigError(Exception):
-    """An error occurred while loading a configuration."""
-
-    def __init__(self, message: str) -> None:
-        self._message = message
-        super().__init__(message)
-
-    @property
-    def message(self) -> str:
-        """The error message."""
-        return self._message
-
-    @message.setter
-    def message(self, value: str) -> None:
-        self._message = value
-        super().__init__(self.message)
-
-
-class InterpolationError(ConfigError):
-    """An error occurred with regard to interpolating a configuration."""
-
-
-class InterpolationLookupError(ConfigError, LookupError):
-    """An error occurred with regard to interpolating a configuration."""
-
-    def __init__(self, message: str) -> None:
-        super().__init__(repr(message))
-
-
-class IncorrectConfigError(ConfigError):
-    """An error occurred while loading a configuration."""
-
-
-class InternalSyntaxError(ConfigError):
-    """Syntax error in a _configzen_ component."""
-
-    def __init__(
-        self,
-        message: str,
-        index: Any = None,
-        prefix: str = "",
-        suffix: str = "",
-    ) -> None:
-        super().__init__(message)
-        self.index = index
-        self.prefix = prefix
-        self.suffix = suffix
-
-
-class ConfigSyntaxError(ConfigError):
-    """An error occurred while parsing arguments."""
-
-
-@contextlib.contextmanager
-def formatted_syntax_error(
-    source: str, error_cls: type[ConfigSyntaxError] = ConfigSyntaxError
-) -> Iterator[None]:
-    """Raise a SyntaxError with a message and a source."""
-    try:
-        yield
-    except InternalSyntaxError as exc:
-        idx = len(exc.prefix) + exc.index + 1
-        charlist = [" "] * len(exc.prefix + repr(source) + exc.suffix)
-        charlist[idx] = "^"
-        indicator = "".join(charlist)
-        msg = "\n".join(
-            map(str, (exc, exc.prefix + repr(source) + exc.suffix, indicator))
-        )
-        raise error_cls(msg) from None
-
-
-class UnspecifiedParserError(ConfigError):
-    """Could not determine the parser to use."""
-
-
-class UnavailableParserError(ConfigError):
-    MISSING_DEPENDENCIES: dict[str, str] = {
-        "yaml": "pyyaml (or ruamel.yaml)",
-        "toml": "toml",
-        "ion": "anyconfig-ion-backend",
-        "bson": "anyconfig-bson-backend",
-        "msgpack": "anyconfig-msgpack-backend",
-        "cbor": "anyconfig-cbor2-backend (or anyconfig-cbor-backend)",
-        "configobj": "anyconfig-configobj-backend",
-    }
-
-    def __init__(self, parser_name: str, agent: ConfigAgent[ConfigModelT]) -> None:
-        missing_dependency: str = self.MISSING_DEPENDENCIES.get(
-            parser_name, f"<the proper anyconfig backend for {parser_name!r} files>"
-        )
-        super().__init__(
-            f"The {parser_name!r} parser required to load configuration "
-            f"for agent {agent} is not available.\n"
-            f"Install it with `pip install {missing_dependency}`."
-        )
-
-
-class ConfigAccessError(ConfigError, LookupError):
-    """An error occurred while accessing configuration part."""
-
-    def __init__(self, config: ConfigModelT, route: str | list[str]) -> None:
-        if not isinstance(route, str):
-            route = ".".join(route)
-        self.route = route
-        super().__init__(
-            f"Could not access {type(config).__name__}.{route}",
-        )
-
-
-class ConfigProcessorError(ConfigError):
-    """An error occurred while preprocessing/exporting a configuration."""
-
-
-class ResourceLookupError(ConfigError, LookupError):
-    """An error occurred while looking up a resource."""
-
-    def __init__(
-        self, resource: ConfigAgent[ConfigModelT] | None, route: list[str]
-    ) -> None:
-        resource_name = resource.resource if resource else "the provided resource"
-        self.route = route
-        super().__init__(f"{route} not found in {resource_name}")
-
-
-class ConfigPreprocessingError(ConfigProcessorError, ValueError):
-    """An error occurred while preprocessing a configuration value."""
+"""This module contains all the custom errors raised by _configzen_."""
+
+from __future__ import annotations
+
+import contextlib
+from collections.abc import Iterator
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from configzen.model import ConfigAgent
+    from configzen.typedefs import ConfigModelT
+
+
+class ConfigError(Exception):
+    """An error occurred while loading a configuration."""
+
+    def __init__(self, message: str) -> None:
+        self._message = message
+        super().__init__(message)
+
+    @property
+    def message(self) -> str:
+        """The error message."""
+        return self._message
+
+    @message.setter
+    def message(self, value: str) -> None:
+        self._message = value
+        super().__init__(self.message)
+
+
+class InterpolationError(ConfigError):
+    """An error occurred with regard to interpolating a configuration."""
+
+
+class InterpolationLookupError(ConfigError, LookupError):
+    """An error occurred with regard to interpolating a configuration."""
+
+    def __init__(self, message: str) -> None:
+        super().__init__(repr(message))
+
+
+class IncorrectConfigError(ConfigError):
+    """An error occurred while loading a configuration."""
+
+
+class InternalSyntaxError(ConfigError):
+    """Syntax error in a _configzen_ component."""
+
+    def __init__(
+        self,
+        message: str,
+        index: Any = None,
+        prefix: str = "",
+        suffix: str = "",
+    ) -> None:
+        super().__init__(message)
+        self.index = index
+        self.prefix = prefix
+        self.suffix = suffix
+
+
+class ConfigSyntaxError(ConfigError):
+    """An error occurred while parsing arguments."""
+
+
+@contextlib.contextmanager
+def formatted_syntax_error(
+    source: str, error_cls: type[ConfigSyntaxError] = ConfigSyntaxError
+) -> Iterator[None]:
+    """Raise a SyntaxError with a message and a source."""
+    try:
+        yield
+    except InternalSyntaxError as exc:
+        idx = len(exc.prefix) + exc.index + 1
+        charlist = [" "] * len(exc.prefix + repr(source) + exc.suffix)
+        charlist[idx] = "^"
+        indicator = "".join(charlist)
+        msg = "\n".join(
+            map(str, (exc, exc.prefix + repr(source) + exc.suffix, indicator))
+        )
+        raise error_cls(msg) from None
+
+
+class UnspecifiedParserError(ConfigError):
+    """Could not determine the parser to use."""
+
+
+class UnavailableParserError(ConfigError):
+    MISSING_DEPENDENCIES: dict[str, str] = {
+        "yaml": "pyyaml (or ruamel.yaml)",
+        "toml": "toml",
+        "ion": "anyconfig-ion-backend",
+        "bson": "anyconfig-bson-backend",
+        "msgpack": "anyconfig-msgpack-backend",
+        "cbor": "anyconfig-cbor2-backend (or anyconfig-cbor-backend)",
+        "configobj": "anyconfig-configobj-backend",
+    }
+
+    def __init__(self, parser_name: str, agent: ConfigAgent[ConfigModelT]) -> None:
+        missing_dependency: str = self.MISSING_DEPENDENCIES.get(
+            parser_name, f"<the proper anyconfig backend for {parser_name!r} files>"
+        )
+        super().__init__(
+            f"The {parser_name!r} parser required to load configuration "
+            f"for agent {agent} is not available.\n"
+            f"Install it with `pip install {missing_dependency}`."
+        )
+
+
+class ConfigAccessError(ConfigError, LookupError):
+    """An error occurred while accessing configuration part."""
+
+    def __init__(self, config: ConfigModelT, route: str | list[str]) -> None:
+        if not isinstance(route, str):
+            route = ".".join(route)
+        self.route = route
+        super().__init__(
+            f"Could not access {type(config).__name__}.{route}",
+        )
+
+
+class ConfigProcessorError(ConfigError):
+    """An error occurred while preprocessing/exporting a configuration."""
+
+
+class ResourceLookupError(ConfigError, LookupError):
+    """An error occurred while looking up a resource."""
+
+    def __init__(
+        self, resource: ConfigAgent[ConfigModelT] | None, route: list[str]
+    ) -> None:
+        resource_name = resource.resource if resource else "the provided resource"
+        self.route = route
+        super().__init__(f"{route} not found in {resource_name}")
+
+
+class ConfigPreprocessingError(ConfigProcessorError, ValueError):
+    """An error occurred while preprocessing a configuration value."""
```

### Comparing `configzen-0.5.6/configzen/processor.py` & `configzen-0.6.0/configzen/processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,838 +1,838 @@
-from __future__ import annotations
-
-import asyncio
-import copy
-import dataclasses
-import enum
-import pathlib
-from collections.abc import Callable
-from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
-
-from anyconfig.utils import is_dict_like, is_list_like
-from pydantic.fields import Undefined
-
-from configzen.errors import ConfigPreprocessingError
-from configzen.typedefs import ConfigModelT, ConfigRouteLike
-
-if TYPE_CHECKING:
-    from configzen.config import BaseContext, ConfigAgent
-
-__all__ = (
-    "DirectiveContext",
-    "directive",
-    "Processor",
-)
-
-DirectiveT = TypeVar("DirectiveT")
-
-EXPORT: str = "__configzen_export__"
-EXECUTES_DIRECTIVES: str = "__configzen_executes_directives__"
-EXECUTES_DIRECTIVES_ASYNC: str = "__configzen_executes_directives_async__"
-
-
-def directive(
-    name: str | enum.Enum,
-    *,
-    asynchronous: bool | None = None,
-) -> Callable[..., Any]:
-    """
-    Decorator for creating processor directives.
-
-    Parameters
-    ----------
-    name
-        The name of the directive.
-    asynchronous
-        Whether the decorated directive function is asynchronous.
-
-    Returns
-    -------
-    The decorated function.
-    """
-    if isinstance(name, enum.Enum):
-        name = name.value.casefold()
-
-    def decorator(func: Any) -> Any:
-        nonlocal asynchronous
-        if asynchronous is None:
-            asynchronous = asyncio.iscoroutinefunction(func)
-        attr = EXECUTES_DIRECTIVES_ASYNC if asynchronous else EXECUTES_DIRECTIVES
-        if not hasattr(func, attr):
-            setattr(func, attr, set())
-        getattr(func, attr).add(name)
-        return func
-
-    return decorator
-
-
-@dataclasses.dataclass
-class DirectiveContext:
-    """
-    Context for processor directives.
-
-    Attributes
-    ----------
-    directive
-        The directive.
-    key
-        The key of the directive.
-    prefix
-        The prefix of the directive.
-    snippet
-        The config snippet where this directive was invoked.
-    container
-        The dictionary that contains the :attr:`dict`.
-
-    """
-
-    directive: str
-    key: str
-    prefix: str
-    snippet: dict[str, Any]
-    container: dict[str, Any]
-
-
-def parse_directive_call(
-    prefix: str,
-    directive_name: str,
-) -> str:
-    if directive_name.startswith(prefix):
-        directive_name = directive_name[len(prefix) :].casefold()
-
-        if not directive_name.isidentifier():
-            msg = f"Invalid directive name: {directive_name}"
-            raise ConfigPreprocessingError(msg)
-
-    return directive_name
-
-
-if TYPE_CHECKING:
-
-    class ExportMetadata(TypedDict, Generic[ConfigModelT]):
-        route: str | None
-        context: BaseContext[ConfigModelT]
-        key_order: list[str]
-        preprocess: bool
-
-else:
-
-    class ExportMetadata(TypedDict):
-        """
-        Metadata for exporting.
-
-        Attributes
-        ----------
-        route
-            The route to import from.
-        context
-            The context attached to the import.
-        """
-
-        route: str | None
-        context: BaseContext[ConfigModelT]
-        key_order: list[str]
-        preprocess: bool
-
-
-class BaseProcessor(Generic[ConfigModelT]):
-    """
-    Processor that executes directives.
-
-    Attributes
-    ----------
-    dict_config
-        The dictionary config to parse and update.
-    directive_prefix
-        The prefix for directives.
-    """
-
-    _directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
-    _async_directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
-    directive_prefix: ClassVar[str]
-    extension_prefix: ClassVar[str]
-
-    def __init__(
-        self,
-        agent: ConfigAgent[ConfigModelT],
-        dict_config: dict[str, Any],
-    ) -> None:
-        self.agent = agent
-        self.dict_config = dict_config
-
-    @classmethod
-    def export(
-        cls,
-        state: Any,
-        *,
-        metadata: ExportMetadata[ConfigModelT] | None = None,
-    ) -> None:
-        """
-        Export the state.
-
-        Parameters
-        ----------
-        state
-            The state to export.
-        metadata
-            The metadata of the substitution.
-        """
-        if is_dict_like(state):
-            if metadata is None:
-                from configzen.config import CONTEXT
-
-                state.pop(CONTEXT, None)
-                metadata = state.pop(EXPORT, None)
-            if metadata:
-                cls._export(state, metadata)
-            else:
-                cls.export(list(state.values()))
-        elif is_list_like(state):
-            for item in state:
-                cls.export(item)
-
-    @classmethod
-    async def export_async(
-        cls,
-        state: Any,
-        *,
-        metadata: ExportMetadata[ConfigModelT] | None = None,
-    ) -> None:
-        """
-        Export the state asynchronously.
-
-        Parameters
-        ----------
-        state
-            The state to export.
-        metadata
-            The metadata of the substitution.
-        """
-        if is_dict_like(state):
-            if metadata is None:
-                from configzen.config import CONTEXT
-
-                state.pop(CONTEXT, None)
-                metadata = state.pop(EXPORT, None)
-            if metadata:
-                await cls._export_async(state, metadata)
-            else:
-                await cls.export_async(list(state.values()))
-        elif is_list_like(state):
-            for item in state:
-                await cls.export_async(item)
-
-    @classmethod
-    def _export(
-        cls,
-        state: Any,
-        metadata: ExportMetadata[ConfigModelT],
-    ) -> None:
-        raise NotImplementedError
-
-    @classmethod
-    async def _export_async(
-        cls,
-        state: Any,
-        metadata: ExportMetadata[ConfigModelT],
-    ) -> None:
-        raise NotImplementedError
-
-    async def preprocess_async(self) -> dict[str, Any]:
-        """
-        Parse the dictionary config and return the parsed config,
-        ready for instantiating the model.
-
-        Returns
-        -------
-        The parsed config.
-        """
-        return cast(dict[str, Any], await self._preprocess_async(self.dict_config))
-
-    def preprocess(self) -> dict[str, Any]:
-        """
-        Parse the dictionary config and return the parsed config,
-        ready for instantiating the model.
-
-        Returns
-        -------
-        The parsed config.
-        """
-        return cast(dict[str, Any], self._preprocess(self.dict_config))
-
-    def _preprocess(self, container: Any) -> Any:
-        if not is_dict_like(container):
-            if is_list_like(container):
-                return [self._preprocess(v) for v in container]
-            return container
-
-        result: dict[str, Any] = {}
-
-        for key, value in sorted(
-            cast(dict[str, Any], container).items(),
-            key=lambda item: item[0] == self.directive_prefix,
-        ):
-            if key.startswith(self.extension_prefix):
-                actual_key = key.lstrip(self.extension_prefix)
-                overridden = result.get(actual_key, {})
-                if not is_dict_like(overridden):
-                    raise ConfigPreprocessingError(
-                        f"{self.extension_prefix} can be used only for overriding "
-                        f"dictionary sections but item at {actual_key!r} "
-                        f"is not a dictionary"
-                    )
-                replacement = overridden | value
-                result[actual_key] = self._preprocess(replacement)
-            elif key.startswith(self.directive_prefix):
-                directive_name = parse_directive_call(self.directive_prefix, key)
-                context_container = container.copy()
-                del context_container[key]
-                context = DirectiveContext(
-                    directive=directive_name,
-                    key=key,
-                    prefix=self.directive_prefix,
-                    snippet=value,
-                    container=context_container,
-                )
-                self._call_directive(context)
-                new_container = self._preprocess(context.container)
-                result |= new_container
-            else:
-                result[key] = self._preprocess(value)
-        return result
-
-    async def _preprocess_async(self, container: Any) -> Any:
-        if not is_dict_like(container):
-            if is_list_like(container):
-                return [await self._preprocess_async(v) for v in container]
-            return container
-
-        result: dict[str, Any] = {}
-
-        for key, value in sorted(
-            cast(dict[str, Any], container).items(),
-            key=lambda item: item[0] == self.directive_prefix,
-        ):
-            if key.startswith(self.extension_prefix):
-                actual_key = key.lstrip(self.extension_prefix)
-                overridden = result.get(actual_key, {})
-                if not is_dict_like(overridden):
-                    raise ConfigPreprocessingError(
-                        f"{self.extension_prefix} can be used only for overriding "
-                        f"dictionary sections but item at {actual_key!r} "
-                        f"is not a dictionary"
-                    )
-                replacement = overridden | value
-                result[actual_key] = await self._preprocess_async(replacement)
-            elif key.startswith(self.directive_prefix):
-                directive_name = parse_directive_call(self.directive_prefix, key)
-                context_container = container.copy()
-                del context_container[key]
-                context = DirectiveContext(
-                    directive=directive_name,
-                    key=key,
-                    prefix=self.directive_prefix,
-                    snippet=value,
-                    container=context_container,
-                )
-                await self._call_directive_async(context)
-                new_container = await self._preprocess_async(context.container)
-                result |= new_container
-            else:
-                result[key] = await self._preprocess_async(value)
-        return result
-
-    def _call_directive(self, context: DirectiveContext) -> None:
-        handler = self._directive_handlers.get(context.directive)
-        if handler is None:
-            raise ConfigPreprocessingError(
-                f"unknown preprocessing directive: {context.directive!r}"
-            )
-        handler(self, context)
-
-    async def _call_directive_async(self, context: DirectiveContext) -> None:
-        handler = self._async_directive_handlers.get(context.directive)
-        if handler is None:
-            raise ConfigPreprocessingError(
-                f"unknown preprocessing directive: {context.directive!r}"
-            )
-        await handler(self, context)
-
-    def __init_subclass__(cls, **kwargs: Any) -> None:
-        super().__init_subclass__(**kwargs)
-        if cls._directive_handlers is None:
-            cls._directive_handlers = {}
-        else:
-            cls._directive_handlers = cls._directive_handlers.copy()
-        if cls._async_directive_handlers is None:
-            cls._async_directive_handlers = {}
-        else:
-            cls._async_directive_handlers = cls._async_directive_handlers.copy()
-        for _name, func in cls.__dict__.items():
-            if hasattr(func, EXECUTES_DIRECTIVES):
-                for directive_name in getattr(func, EXECUTES_DIRECTIVES):
-                    cls._directive_handlers[directive_name] = func
-            elif hasattr(func, EXECUTES_DIRECTIVES_ASYNC):
-                for directive_name in getattr(func, EXECUTES_DIRECTIVES_ASYNC):
-                    cls._async_directive_handlers[directive_name] = func
-
-    @classmethod
-    def register_directive(cls, name: str, func: Any) -> None:
-        if cls._directive_handlers is None:
-            cls._directive_handlers = {}
-        cls._directive_handlers[name] = func
-
-    @classmethod
-    def directive(cls, directive_name: str) -> str:
-        """
-        Create a directive call.
-
-        Parameters
-        ----------
-        directive_name
-            The name of the directive.
-
-        Returns
-        -------
-        The directive call.
-        """
-        if isinstance(directive_name, enum.Enum):
-            directive_name = directive_name.value
-
-        return cls.directive_prefix + directive_name
-
-
-class Directives(str, enum.Enum):
-    EXTEND = "extend"
-    INCLUDE = "include"
-    COPY = "copy"
-
-
-class Processor(BaseProcessor[ConfigModelT]):
-    directive_prefix = "^"
-    extension_prefix = "+"
-    route_separator: ClassVar[str] = ":"
-
-    @directive(Directives.EXTEND)
-    def extend(self, ctx: DirectiveContext) -> None:
-        """
-        Extend a configuration with another configuration.
-        Recursively preprocess the referenced configuration.
-        Preserve information about the referenced configuration.
-
-        Visual example
-        --------------
-
-        With `base.yaml` containing:
-        ```yaml
-        section:
-          foo: 1
-          bar: 2
-        ```
-
-        and `config.yaml` containing:
-
-        ```yaml
-        ^extend: base.yaml
-        +section:
-          foo: 3
-        ```
-
-        -> `load()` -> `save()` ->
-
-        ```yaml
-        ^extend: base.yaml
-        +section:
-          foo: 3
-        ```
-        """
-        self._substitute(ctx, preprocess=True, preserve=True)
-
-    @directive(Directives.INCLUDE)
-    def include(self, ctx: DirectiveContext) -> None:
-        """
-        Include a configuration in another configuration.
-        Recursively preprocess the referenced configuration.
-        Do not preserve information about the referenced configuration.
-
-        Visual example
-        --------------
-        With `biz.yaml` containing:
-
-        ```yaml
-        section:
-          biz: 3
-        ```
-
-        and `base.yaml` containing:
-
-        ```yaml
-        ^extend: biz.yaml
-        +section:
-          foo: 1
-          bar: 2
-        ```
-
-        and `config.yaml` containing:
-
-        ```yaml
-        ^include: base.yaml
-        +section:
-          foo: 3
-        ```
-
-        -> `load()` -> `save()` ->
-
-        ```yaml
-        ^extend: biz.yaml
-        +section:
-          bar: 2
-          foo: 3
-        ```
-        """
-        self._substitute(ctx, preprocess=True, preserve=False)
-
-    @directive(Directives.COPY)
-    def copy(self, ctx: DirectiveContext) -> None:
-        """
-        Copy a configuration and paste into another configuration.
-        This is just a literal copy-paste.
-        Do not preprocess the referenced configuration.
-        Do not preserve information about the referenced configuration.
-
-        Visual example
-        --------------
-        With `base.yaml` containing:
-
-        ```yaml
-        section:
-          foo: 1
-          bar: 2
-        ```
-
-        and `config.yaml` containing:
-
-        ```yaml
-        ^copy: base.yaml
-        +section:
-          foo: 3
-        ```
-
-        -> `load()` -> `save()` ->
-
-        ```yaml
-        section:
-          foo: 3
-          bar: 2
-        ```
-        """
-        self._substitute(ctx, preprocess=False, preserve=False)
-
-    @directive(Directives.EXTEND)
-    async def extend_async(self, ctx: DirectiveContext) -> None:
-        """
-        Extend a configuration with another configuration asynchronously.
-        For more information see `extend`.
-        """
-        await self._substitute_async(ctx, preprocess=True, preserve=True)
-
-    @directive(Directives.INCLUDE)
-    async def include_async(self, ctx: DirectiveContext) -> None:
-        """
-        Include a configuration in another configuration asynchronously.
-        For more information see `include`.
-        """
-        await self._substitute_async(ctx, preprocess=True, preserve=False)
-
-    @directive(Directives.COPY)
-    async def copy_async(self, ctx: DirectiveContext) -> None:
-        """
-        Copy a configuration and paste into another configuration asynchronously.
-        For more information see `copy`.
-        """
-        await self._substitute_async(ctx, preprocess=False, preserve=False)
-
-    def _get_substitution_means(
-        self, ctx: DirectiveContext  # , *, preserve: bool
-    ) -> tuple[
-        ConfigAgent[ConfigModelT], ConfigAgent[ConfigModelT], ConfigRouteLike | None
-    ]:
-        agent_class = type(self.agent)
-
-        # todo(bswck): raise on include and extend combined
-        # if preserve and ???:
-        #     msg = (
-        #         "Using more than one ??? directive "
-        #         "in the same scope is not allowed"
-        #     )
-        #     raise ConfigPreprocessingError(msg)
-
-        agent, route = agent_class.from_directive_context(
-            ctx, route_separator=self.route_separator
-        )
-
-        if agent.resource == self.agent.resource:
-            raise ConfigPreprocessingError(
-                f"{agent.resource} tried to {ctx.directive!r} on itself"
-            )
-
-        actual_agent = agent
-        if agent.is_relative:
-            parent = cast(pathlib.Path, self.agent.resource).parent
-            child = cast(pathlib.Path, agent.resource)
-
-            actual_agent = copy.copy(agent)
-            actual_agent.resource = parent / child
-
-        return actual_agent, agent, route
-
-    def _substitute(
-        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
-    ) -> None:
-        agent, orig_agent, route = self._get_substitution_means(ctx)
-
-        with agent.processor_open_resource() as reader:
-            source = orig_agent.load_dict(reader.read(), preprocess=preprocess)
-
-        self._substitute_impl(
-            ctx,
-            route,
-            source=source,
-            agent=orig_agent,
-            preprocess=preprocess,
-            preserve=preserve,
-        )
-
-    async def _substitute_async(
-        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
-    ) -> None:
-        agent, orig_agent, route = self._get_substitution_means(ctx)
-
-        async with agent.processor_open_resource_async() as reader:
-            source = orig_agent.load_dict(await reader.read(), preprocess=preprocess)
-
-        self._substitute_impl(
-            ctx,
-            route,
-            source=source,
-            agent=orig_agent,
-            preprocess=preprocess,
-            preserve=preserve,
-        )
-
-    @staticmethod
-    def _substitute_impl(  # noqa: PLR0913
-        ctx: DirectiveContext,
-        route: ConfigRouteLike | None,
-        *,
-        source: dict[str, Any],
-        agent: ConfigAgent[ConfigModelT],
-        preprocess: bool,
-        preserve: bool,
-    ) -> None:
-        from configzen.config import CONTEXT, Context, at
-
-        if route:
-            source = at(source, route, agent=agent)
-            if not is_dict_like(source):
-                raise ConfigPreprocessingError(
-                    f"imported item {route!r} "
-                    f"from {agent.resource} is not a dictionary"
-                )
-
-        context: Context[ConfigModelT] = Context(agent)
-        ctx.container = source | ctx.container
-
-        if preserve:
-            ctx.container |= {
-                CONTEXT: context,
-                EXPORT: ExportMetadata(
-                    route=str(route),
-                    context=context,
-                    preprocess=preprocess,
-                    key_order=list(ctx.container),
-                ),
-            }
-
-    @classmethod
-    def _export(  # noqa: C901
-        cls,
-        state: dict[str, Any],
-        metadata: ExportMetadata[ConfigModelT],
-    ) -> None:
-        """
-        Exports model state preserving substition directive calls in the model state.
-
-        Parameters
-        ----------
-        metadata
-        state
-        """
-        from configzen.config import CONTEXT, at, export_hook
-
-        overrides = {}
-
-        route = metadata["route"]
-        context = metadata["context"]
-        key_order = metadata["key_order"]
-        agent = context.agent
-
-        with agent.processor_open_resource() as reader:
-            # Here we intentionally always preprocess the loaded configuration.
-            loaded = agent.load_dict(reader.read())
-
-            if route:
-                loaded = at(loaded, route, agent=agent)
-
-        substituted_values = loaded.copy()
-
-        for key, value in loaded.items():
-            counterpart_value = state.pop(key, Undefined)
-            if counterpart_value is Undefined:
-                continue
-            counterpart_value = export_hook(counterpart_value)
-
-            if is_dict_like(value):
-                if EXPORT in value:
-                    value.pop(CONTEXT, None)
-                    cls.export(value, metadata=value.pop(EXPORT))
-                overrides_for_key = {
-                    sub_key: comp
-                    for sub_key, comp in counterpart_value.items()
-                    if (
-                        (orig := value.get(sub_key, Undefined)) is Undefined
-                        or orig != comp
-                    )
-                }
-                if overrides_for_key:
-                    export_key = agent.processor_class.extension_prefix + key
-                    overrides[export_key] = overrides_for_key
-
-            elif is_list_like(value):
-                cls.export(value)
-                if value != counterpart_value:
-                    overrides[key] = counterpart_value
-
-            elif value != counterpart_value:
-                overrides[key] = counterpart_value
-                del substituted_values[key]
-
-        for value in state.values():
-            cls.export(value)
-
-        cls._export_finalize(
-            context=context,
-            state=state,
-            overrides=overrides,
-            values=substituted_values,
-            route=route,
-            key_order=key_order,
-        )
-
-    @classmethod
-    async def _export_async(  # noqa: C901
-        cls,
-        state: dict[str, Any],
-        metadata: ExportMetadata[ConfigModelT],
-    ) -> None:
-        """
-        Exports model state preserving substition directive calls in the model state.
-
-        Parameters
-        ----------
-        metadata
-        state
-        """
-        from configzen.config import CONTEXT, at, export_hook
-
-        overrides = {}
-
-        route = metadata["route"]
-        context = metadata["context"]
-        key_order = metadata["key_order"]
-        agent = context.agent
-
-        async with agent.processor_open_resource_async() as reader:
-            # Here we intentionally always preprocess the loaded configuration.
-            loaded = await agent.load_dict_async(await reader.read())
-
-            if route:
-                loaded = at(loaded, route, agent=agent)
-
-        substituted_values = loaded.copy()
-
-        for key, value in loaded.items():
-            counterpart_value = state.pop(key, Undefined)
-            if counterpart_value is Undefined:
-                continue
-            counterpart_value = export_hook(counterpart_value)
-
-            if is_dict_like(value):
-                if EXPORT in value:
-                    value.pop(CONTEXT, None)
-                    await cls.export_async(value, metadata=value.pop(EXPORT))
-                overrides_for_key = {
-                    sub_key: comp
-                    for sub_key, comp in counterpart_value.items()
-                    if (
-                        (orig := value.get(sub_key, Undefined)) is Undefined
-                        or orig != comp
-                    )
-                }
-                if overrides_for_key:
-                    export_key = agent.processor_class.extension_prefix + key
-                    overrides[export_key] = overrides_for_key
-
-            elif is_list_like(value):
-                await cls.export_async(value)
-                if value != counterpart_value:
-                    overrides[key] = counterpart_value
-
-            elif counterpart_value != value:
-                overrides[key] = counterpart_value
-                del substituted_values[key]
-
-        for value in state.values():
-            await cls.export_async(value)
-
-        cls._export_finalize(
-            context=context,
-            state=state,
-            overrides=overrides,
-            values=substituted_values,
-            route=route,
-            key_order=key_order,
-        )
-
-    @classmethod
-    def _export_finalize(  # noqa: PLR0913
-        cls,
-        context: BaseContext[ConfigModelT],
-        *,
-        state: dict[str, Any],
-        overrides: dict[str, Any],
-        values: dict[str, Any],
-        route: str | None,
-        key_order: list[str],
-    ) -> None:
-        from configzen.config import export_hook
-
-        state |= overrides
-        extras: dict[str, Any] = {
-            key: state.pop(key) for key in set(state) if key not in key_order
-        }
-
-        if values:
-            substitution_directive = cls.directive(Directives.EXTEND)
-            resource = str(export_hook(context.agent.resource))
-            if route:
-                resource = cls.route_separator.join((resource, route))
-            # Put the substitution directive at the beginning of the state in-place.
-            state |= {substitution_directive: resource} | {
-                key: state.pop(key) for key in set(state)
-            }
-
-        # Preserve the order of keys in the original configuration.
-        for key in filter(state.__contains__, key_order):
-            state[key] = state.pop(key)
-
-        state |= extras
+from __future__ import annotations
+
+import asyncio
+import copy
+import dataclasses
+import enum
+import pathlib
+from collections.abc import Callable
+from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
+
+from anyconfig.utils import is_dict_like, is_list_like
+from pydantic.fields import Undefined
+
+from configzen.errors import ConfigPreprocessingError
+from configzen.typedefs import ConfigModelT, ConfigRouteLike
+
+if TYPE_CHECKING:
+    from configzen.model import BaseContext, ConfigAgent
+
+__all__ = (
+    "DirectiveContext",
+    "directive",
+    "Processor",
+)
+
+DirectiveT = TypeVar("DirectiveT")
+
+EXPORT: str = "__configzen_export__"
+EXECUTES_DIRECTIVES: str = "__configzen_executes_directives__"
+EXECUTES_DIRECTIVES_ASYNC: str = "__configzen_executes_directives_async__"
+
+
+def directive(
+    name: str | enum.Enum,
+    *,
+    asynchronous: bool | None = None,
+) -> Callable[..., Any]:
+    """
+    Decorator for creating processor directives.
+
+    Parameters
+    ----------
+    name
+        The name of the directive.
+    asynchronous
+        Whether the decorated directive function is asynchronous.
+
+    Returns
+    -------
+    The decorated function.
+    """
+    if isinstance(name, enum.Enum):
+        name = name.value.casefold()
+
+    def decorator(func: Any) -> Any:
+        nonlocal asynchronous
+        if asynchronous is None:
+            asynchronous = asyncio.iscoroutinefunction(func)
+        attr = EXECUTES_DIRECTIVES_ASYNC if asynchronous else EXECUTES_DIRECTIVES
+        if not hasattr(func, attr):
+            setattr(func, attr, set())
+        getattr(func, attr).add(name)
+        return func
+
+    return decorator
+
+
+@dataclasses.dataclass
+class DirectiveContext:
+    """
+    Context for processor directives.
+
+    Attributes
+    ----------
+    directive
+        The directive.
+    key
+        The key of the directive.
+    prefix
+        The prefix of the directive.
+    snippet
+        The config snippet where this directive was invoked.
+    container
+        The dictionary that contains the :attr:`dict`.
+
+    """
+
+    directive: str
+    key: str
+    prefix: str
+    snippet: dict[str, Any]
+    container: dict[str, Any]
+
+
+def parse_directive_call(
+    prefix: str,
+    directive_name: str,
+) -> str:
+    if directive_name.startswith(prefix):
+        directive_name = directive_name[len(prefix) :].casefold()
+
+        if not directive_name.isidentifier():
+            msg = f"Invalid directive name: {directive_name}"
+            raise ConfigPreprocessingError(msg)
+
+    return directive_name
+
+
+if TYPE_CHECKING:
+
+    class ExportMetadata(TypedDict, Generic[ConfigModelT]):
+        route: str | None
+        context: BaseContext[ConfigModelT]
+        key_order: list[str]
+        preprocess: bool
+
+else:
+
+    class ExportMetadata(TypedDict):
+        """
+        Metadata for exporting.
+
+        Attributes
+        ----------
+        route
+            The route to import from.
+        context
+            The context attached to the import.
+        """
+
+        route: str | None
+        context: BaseContext[ConfigModelT]
+        key_order: list[str]
+        preprocess: bool
+
+
+class BaseProcessor(Generic[ConfigModelT]):
+    """
+    Processor that executes directives.
+
+    Attributes
+    ----------
+    dict_config
+        The dictionary config to parse and update.
+    directive_prefix
+        The prefix for directives.
+    """
+
+    _directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
+    _async_directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
+    directive_prefix: ClassVar[str]
+    extension_prefix: ClassVar[str]
+
+    def __init__(
+        self,
+        agent: ConfigAgent[ConfigModelT],
+        dict_config: dict[str, Any],
+    ) -> None:
+        self.agent = agent
+        self.dict_config = dict_config
+
+    @classmethod
+    def export(
+        cls,
+        state: Any,
+        *,
+        metadata: ExportMetadata[ConfigModelT] | None = None,
+    ) -> None:
+        """
+        Export the state.
+
+        Parameters
+        ----------
+        state
+            The state to export.
+        metadata
+            The metadata of the substitution.
+        """
+        if is_dict_like(state):
+            if metadata is None:
+                from configzen.model import CONTEXT
+
+                state.pop(CONTEXT, None)
+                metadata = state.pop(EXPORT, None)
+            if metadata:
+                cls._export(state, metadata)
+            else:
+                cls.export(list(state.values()))
+        elif is_list_like(state):
+            for item in state:
+                cls.export(item)
+
+    @classmethod
+    async def export_async(
+        cls,
+        state: Any,
+        *,
+        metadata: ExportMetadata[ConfigModelT] | None = None,
+    ) -> None:
+        """
+        Export the state asynchronously.
+
+        Parameters
+        ----------
+        state
+            The state to export.
+        metadata
+            The metadata of the substitution.
+        """
+        if is_dict_like(state):
+            if metadata is None:
+                from configzen.model import CONTEXT
+
+                state.pop(CONTEXT, None)
+                metadata = state.pop(EXPORT, None)
+            if metadata:
+                await cls._export_async(state, metadata)
+            else:
+                await cls.export_async(list(state.values()))
+        elif is_list_like(state):
+            for item in state:
+                await cls.export_async(item)
+
+    @classmethod
+    def _export(
+        cls,
+        state: Any,
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        raise NotImplementedError
+
+    @classmethod
+    async def _export_async(
+        cls,
+        state: Any,
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        raise NotImplementedError
+
+    async def preprocess_async(self) -> dict[str, Any]:
+        """
+        Parse the dictionary config and return the parsed config,
+        ready for instantiating the model.
+
+        Returns
+        -------
+        The parsed config.
+        """
+        return cast(dict[str, Any], await self._preprocess_async(self.dict_config))
+
+    def preprocess(self) -> dict[str, Any]:
+        """
+        Parse the dictionary config and return the parsed config,
+        ready for instantiating the model.
+
+        Returns
+        -------
+        The parsed config.
+        """
+        return cast(dict[str, Any], self._preprocess(self.dict_config))
+
+    def _preprocess(self, container: Any) -> Any:
+        if not is_dict_like(container):
+            if is_list_like(container):
+                return [self._preprocess(v) for v in container]
+            return container
+
+        result: dict[str, Any] = {}
+
+        for key, value in sorted(
+            cast(dict[str, Any], container).items(),
+            key=lambda item: item[0] == self.directive_prefix,
+        ):
+            if key.startswith(self.extension_prefix):
+                actual_key = key.lstrip(self.extension_prefix)
+                overridden = result.get(actual_key, {})
+                if not is_dict_like(overridden):
+                    raise ConfigPreprocessingError(
+                        f"{self.extension_prefix} can be used only for overriding "
+                        f"dictionary sections but item at {actual_key!r} "
+                        f"is not a dictionary"
+                    )
+                replacement = overridden | value
+                result[actual_key] = self._preprocess(replacement)
+            elif key.startswith(self.directive_prefix):
+                directive_name = parse_directive_call(self.directive_prefix, key)
+                context_container = container.copy()
+                del context_container[key]
+                context = DirectiveContext(
+                    directive=directive_name,
+                    key=key,
+                    prefix=self.directive_prefix,
+                    snippet=value,
+                    container=context_container,
+                )
+                self._call_directive(context)
+                new_container = self._preprocess(context.container)
+                result |= new_container
+            else:
+                result[key] = self._preprocess(value)
+        return result
+
+    async def _preprocess_async(self, container: Any) -> Any:
+        if not is_dict_like(container):
+            if is_list_like(container):
+                return [await self._preprocess_async(v) for v in container]
+            return container
+
+        result: dict[str, Any] = {}
+
+        for key, value in sorted(
+            cast(dict[str, Any], container).items(),
+            key=lambda item: item[0] == self.directive_prefix,
+        ):
+            if key.startswith(self.extension_prefix):
+                actual_key = key.lstrip(self.extension_prefix)
+                overridden = result.get(actual_key, {})
+                if not is_dict_like(overridden):
+                    raise ConfigPreprocessingError(
+                        f"{self.extension_prefix} can be used only for overriding "
+                        f"dictionary sections but item at {actual_key!r} "
+                        f"is not a dictionary"
+                    )
+                replacement = overridden | value
+                result[actual_key] = await self._preprocess_async(replacement)
+            elif key.startswith(self.directive_prefix):
+                directive_name = parse_directive_call(self.directive_prefix, key)
+                context_container = container.copy()
+                del context_container[key]
+                context = DirectiveContext(
+                    directive=directive_name,
+                    key=key,
+                    prefix=self.directive_prefix,
+                    snippet=value,
+                    container=context_container,
+                )
+                await self._call_directive_async(context)
+                new_container = await self._preprocess_async(context.container)
+                result |= new_container
+            else:
+                result[key] = await self._preprocess_async(value)
+        return result
+
+    def _call_directive(self, context: DirectiveContext) -> None:
+        handler = self._directive_handlers.get(context.directive)
+        if handler is None:
+            raise ConfigPreprocessingError(
+                f"unknown preprocessing directive: {context.directive!r}"
+            )
+        handler(self, context)
+
+    async def _call_directive_async(self, context: DirectiveContext) -> None:
+        handler = self._async_directive_handlers.get(context.directive)
+        if handler is None:
+            raise ConfigPreprocessingError(
+                f"unknown preprocessing directive: {context.directive!r}"
+            )
+        await handler(self, context)
+
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if cls._directive_handlers is None:
+            cls._directive_handlers = {}
+        else:
+            cls._directive_handlers = cls._directive_handlers.copy()
+        if cls._async_directive_handlers is None:
+            cls._async_directive_handlers = {}
+        else:
+            cls._async_directive_handlers = cls._async_directive_handlers.copy()
+        for _name, func in cls.__dict__.items():
+            if hasattr(func, EXECUTES_DIRECTIVES):
+                for directive_name in getattr(func, EXECUTES_DIRECTIVES):
+                    cls._directive_handlers[directive_name] = func
+            elif hasattr(func, EXECUTES_DIRECTIVES_ASYNC):
+                for directive_name in getattr(func, EXECUTES_DIRECTIVES_ASYNC):
+                    cls._async_directive_handlers[directive_name] = func
+
+    @classmethod
+    def register_directive(cls, name: str, func: Any) -> None:
+        if cls._directive_handlers is None:
+            cls._directive_handlers = {}
+        cls._directive_handlers[name] = func
+
+    @classmethod
+    def directive(cls, directive_name: str) -> str:
+        """
+        Create a directive call.
+
+        Parameters
+        ----------
+        directive_name
+            The name of the directive.
+
+        Returns
+        -------
+        The directive call.
+        """
+        if isinstance(directive_name, enum.Enum):
+            directive_name = directive_name.value
+
+        return cls.directive_prefix + directive_name
+
+
+class Directives(str, enum.Enum):
+    EXTEND = "extend"
+    INCLUDE = "include"
+    COPY = "copy"
+
+
+class Processor(BaseProcessor[ConfigModelT]):
+    directive_prefix = "^"
+    extension_prefix = "+"
+    route_separator: ClassVar[str] = ":"
+
+    @directive(Directives.EXTEND)
+    def extend(self, ctx: DirectiveContext) -> None:
+        """
+        Extend a configuration with another configuration.
+        Recursively preprocess the referenced configuration.
+        Preserve information about the referenced configuration.
+
+        Visual example
+        --------------
+
+        With `base.yaml` containing:
+        ```yaml
+        section:
+          foo: 1
+          bar: 2
+        ```
+
+        and `config.yaml` containing:
+
+        ```yaml
+        ^extend: base.yaml
+        +section:
+          foo: 3
+        ```
+
+        -> `load()` -> `save()` ->
+
+        ```yaml
+        ^extend: base.yaml
+        +section:
+          foo: 3
+        ```
+        """
+        self._substitute(ctx, preprocess=True, preserve=True)
+
+    @directive(Directives.INCLUDE)
+    def include(self, ctx: DirectiveContext) -> None:
+        """
+        Include a configuration in another configuration.
+        Recursively preprocess the referenced configuration.
+        Do not preserve information about the referenced configuration.
+
+        Visual example
+        --------------
+        With `biz.yaml` containing:
+
+        ```yaml
+        section:
+          biz: 3
+        ```
+
+        and `base.yaml` containing:
+
+        ```yaml
+        ^extend: biz.yaml
+        +section:
+          foo: 1
+          bar: 2
+        ```
+
+        and `config.yaml` containing:
+
+        ```yaml
+        ^include: base.yaml
+        +section:
+          foo: 3
+        ```
+
+        -> `load()` -> `save()` ->
+
+        ```yaml
+        ^extend: biz.yaml
+        +section:
+          bar: 2
+          foo: 3
+        ```
+        """
+        self._substitute(ctx, preprocess=True, preserve=False)
+
+    @directive(Directives.COPY)
+    def copy(self, ctx: DirectiveContext) -> None:
+        """
+        Copy a configuration and paste into another configuration.
+        This is just a literal copy-paste.
+        Do not preprocess the referenced configuration.
+        Do not preserve information about the referenced configuration.
+
+        Visual example
+        --------------
+        With `base.yaml` containing:
+
+        ```yaml
+        section:
+          foo: 1
+          bar: 2
+        ```
+
+        and `config.yaml` containing:
+
+        ```yaml
+        ^copy: base.yaml
+        +section:
+          foo: 3
+        ```
+
+        -> `load()` -> `save()` ->
+
+        ```yaml
+        section:
+          foo: 3
+          bar: 2
+        ```
+        """
+        self._substitute(ctx, preprocess=False, preserve=False)
+
+    @directive(Directives.EXTEND)
+    async def extend_async(self, ctx: DirectiveContext) -> None:
+        """
+        Extend a configuration with another configuration asynchronously.
+        For more information see `extend`.
+        """
+        await self._substitute_async(ctx, preprocess=True, preserve=True)
+
+    @directive(Directives.INCLUDE)
+    async def include_async(self, ctx: DirectiveContext) -> None:
+        """
+        Include a configuration in another configuration asynchronously.
+        For more information see `include`.
+        """
+        await self._substitute_async(ctx, preprocess=True, preserve=False)
+
+    @directive(Directives.COPY)
+    async def copy_async(self, ctx: DirectiveContext) -> None:
+        """
+        Copy a configuration and paste into another configuration asynchronously.
+        For more information see `copy`.
+        """
+        await self._substitute_async(ctx, preprocess=False, preserve=False)
+
+    def _get_substitution_means(
+        self, ctx: DirectiveContext  # , *, preserve: bool
+    ) -> tuple[
+        ConfigAgent[ConfigModelT], ConfigAgent[ConfigModelT], ConfigRouteLike | None
+    ]:
+        agent_class = type(self.agent)
+
+        # todo(bswck): raise on include and extend combined
+        # if preserve and ???:
+        #     msg = (
+        #         "Using more than one ??? directive "
+        #         "in the same scope is not allowed"
+        #     )
+        #     raise ConfigPreprocessingError(msg)
+
+        agent, route = agent_class.from_directive_context(
+            ctx, route_separator=self.route_separator
+        )
+
+        if agent.resource == self.agent.resource:
+            raise ConfigPreprocessingError(
+                f"{agent.resource} tried to {ctx.directive!r} on itself"
+            )
+
+        actual_agent = agent
+        if agent.is_relative:
+            parent = cast(pathlib.Path, self.agent.resource).parent
+            child = cast(pathlib.Path, agent.resource)
+
+            actual_agent = copy.copy(agent)
+            actual_agent.resource = parent / child
+
+        return actual_agent, agent, route
+
+    def _substitute(
+        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
+    ) -> None:
+        agent, orig_agent, route = self._get_substitution_means(ctx)
+
+        with agent.processor_open_resource() as reader:
+            source = orig_agent.load_dict(reader.read(), preprocess=preprocess)
+
+        self._substitute_impl(
+            ctx,
+            route,
+            source=source,
+            agent=orig_agent,
+            preprocess=preprocess,
+            preserve=preserve,
+        )
+
+    async def _substitute_async(
+        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
+    ) -> None:
+        agent, orig_agent, route = self._get_substitution_means(ctx)
+
+        async with agent.processor_open_resource_async() as reader:
+            source = orig_agent.load_dict(await reader.read(), preprocess=preprocess)
+
+        self._substitute_impl(
+            ctx,
+            route,
+            source=source,
+            agent=orig_agent,
+            preprocess=preprocess,
+            preserve=preserve,
+        )
+
+    @staticmethod
+    def _substitute_impl(  # noqa: PLR0913
+        ctx: DirectiveContext,
+        route: ConfigRouteLike | None,
+        *,
+        source: dict[str, Any],
+        agent: ConfigAgent[ConfigModelT],
+        preprocess: bool,
+        preserve: bool,
+    ) -> None:
+        from configzen.model import CONTEXT, Context, at
+
+        if route:
+            source = at(source, route, agent=agent)
+            if not is_dict_like(source):
+                raise ConfigPreprocessingError(
+                    f"imported item {route!r} "
+                    f"from {agent.resource} is not a dictionary"
+                )
+
+        context: Context[ConfigModelT] = Context(agent)
+        ctx.container = source | ctx.container
+
+        if preserve:
+            ctx.container |= {
+                CONTEXT: context,
+                EXPORT: ExportMetadata(
+                    route=str(route),
+                    context=context,
+                    preprocess=preprocess,
+                    key_order=list(ctx.container),
+                ),
+            }
+
+    @classmethod
+    def _export(  # noqa: C901
+        cls,
+        state: dict[str, Any],
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        """
+        Exports model state preserving substition directive calls in the model state.
+
+        Parameters
+        ----------
+        metadata
+        state
+        """
+        from configzen.model import CONTEXT, at, export_hook
+
+        overrides = {}
+
+        route = metadata["route"]
+        context = metadata["context"]
+        key_order = metadata["key_order"]
+        agent = context.agent
+
+        with agent.processor_open_resource() as reader:
+            # Here we intentionally always preprocess the loaded configuration.
+            loaded = agent.load_dict(reader.read())
+
+            if route:
+                loaded = at(loaded, route, agent=agent)
+
+        substituted_values = loaded.copy()
+
+        for key, value in loaded.items():
+            counterpart_value = state.pop(key, Undefined)
+            if counterpart_value is Undefined:
+                continue
+            counterpart_value = export_hook(counterpart_value)
+
+            if is_dict_like(value):
+                if EXPORT in value:
+                    value.pop(CONTEXT, None)
+                    cls.export(value, metadata=value.pop(EXPORT))
+                overrides_for_key = {
+                    sub_key: comp
+                    for sub_key, comp in counterpart_value.items()
+                    if (
+                        (orig := value.get(sub_key, Undefined)) is Undefined
+                        or orig != comp
+                    )
+                }
+                if overrides_for_key:
+                    export_key = agent.processor_class.extension_prefix + key
+                    overrides[export_key] = overrides_for_key
+
+            elif is_list_like(value):
+                cls.export(value)
+                if value != counterpart_value:
+                    overrides[key] = counterpart_value
+
+            elif value != counterpart_value:
+                overrides[key] = counterpart_value
+                del substituted_values[key]
+
+        for value in state.values():
+            cls.export(value)
+
+        cls._export_finalize(
+            context=context,
+            state=state,
+            overrides=overrides,
+            values=substituted_values,
+            route=route,
+            key_order=key_order,
+        )
+
+    @classmethod
+    async def _export_async(  # noqa: C901
+        cls,
+        state: dict[str, Any],
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        """
+        Exports model state preserving substition directive calls in the model state.
+
+        Parameters
+        ----------
+        metadata
+        state
+        """
+        from configzen.model import CONTEXT, at, export_hook
+
+        overrides = {}
+
+        route = metadata["route"]
+        context = metadata["context"]
+        key_order = metadata["key_order"]
+        agent = context.agent
+
+        async with agent.processor_open_resource_async() as reader:
+            # Here we intentionally always preprocess the loaded configuration.
+            loaded = await agent.load_dict_async(await reader.read())
+
+            if route:
+                loaded = at(loaded, route, agent=agent)
+
+        substituted_values = loaded.copy()
+
+        for key, value in loaded.items():
+            counterpart_value = state.pop(key, Undefined)
+            if counterpart_value is Undefined:
+                continue
+            counterpart_value = export_hook(counterpart_value)
+
+            if is_dict_like(value):
+                if EXPORT in value:
+                    value.pop(CONTEXT, None)
+                    await cls.export_async(value, metadata=value.pop(EXPORT))
+                overrides_for_key = {
+                    sub_key: comp
+                    for sub_key, comp in counterpart_value.items()
+                    if (
+                        (orig := value.get(sub_key, Undefined)) is Undefined
+                        or orig != comp
+                    )
+                }
+                if overrides_for_key:
+                    export_key = agent.processor_class.extension_prefix + key
+                    overrides[export_key] = overrides_for_key
+
+            elif is_list_like(value):
+                await cls.export_async(value)
+                if value != counterpart_value:
+                    overrides[key] = counterpart_value
+
+            elif counterpart_value != value:
+                overrides[key] = counterpart_value
+                del substituted_values[key]
+
+        for value in state.values():
+            await cls.export_async(value)
+
+        cls._export_finalize(
+            context=context,
+            state=state,
+            overrides=overrides,
+            values=substituted_values,
+            route=route,
+            key_order=key_order,
+        )
+
+    @classmethod
+    def _export_finalize(  # noqa: PLR0913
+        cls,
+        context: BaseContext[ConfigModelT],
+        *,
+        state: dict[str, Any],
+        overrides: dict[str, Any],
+        values: dict[str, Any],
+        route: str | None,
+        key_order: list[str],
+    ) -> None:
+        from configzen.model import export_hook
+
+        state |= overrides
+        extras: dict[str, Any] = {
+            key: state.pop(key) for key in set(state) if key not in key_order
+        }
+
+        if values:
+            substitution_directive = cls.directive(Directives.EXTEND)
+            resource = str(export_hook(context.agent.resource))
+            if route:
+                resource = cls.route_separator.join((resource, route))
+            # Put the substitution directive at the beginning of the state in-place.
+            state |= {substitution_directive: resource} | {
+                key: state.pop(key) for key in set(state)
+            }
+
+        # Preserve the order of keys in the original configuration.
+        for key in filter(state.__contains__, key_order):
+            state[key] = state.pop(key)
+
+        state |= extras
```

### Comparing `configzen-0.5.6/configzen/typedefs.py` & `configzen-0.6.0/configzen/typedefs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import contextlib
-import os
-import pathlib
-import sys
-from collections.abc import Mapping, Set
-from typing import TYPE_CHECKING, Any, Optional, TextIO, TypeVar, Union
-
-if sys.version_info >= (3, 10):
-    from typing import ParamSpec, TypeAlias
-else:
-    from typing_extensions import ParamSpec, TypeAlias
-
-if TYPE_CHECKING:
-    from aiofiles.base import AiofilesContextManager
-    from aiofiles.threadpool.text import AsyncTextIOWrapper
-
-    # noinspection PyUnresolvedReferences
-    from configzen.config import ConfigModel
-    from configzen.route import ConfigRoute
-
-T = TypeVar("T")
-P = ParamSpec("P")
-
-ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
-ConfigRouteLike: TypeAlias = Union[str, list[str], "ConfigRoute"]
-
-ConfigIO: TypeAlias = contextlib.AbstractContextManager[TextIO]
-AsyncConfigIO: TypeAlias = "AiofilesContextManager[None, None, AsyncTextIOWrapper]"
-RawResourceT: TypeAlias = Union[ConfigIO, str, int, os.PathLike, pathlib.Path]
-NormalizedResourceT: TypeAlias = Union[ConfigIO, str, int, pathlib.Path]
-IncludeExcludeT: TypeAlias = Optional[
-    Union[
-        Set[Union[int, str]],
-        Mapping[Union[int, str], Any],
-    ]
-]
+import contextlib
+import os
+import pathlib
+import sys
+from collections.abc import Mapping, Set
+from typing import TYPE_CHECKING, Any, Optional, TextIO, TypeVar, Union
+
+if sys.version_info >= (3, 10):
+    from typing import ParamSpec, TypeAlias
+else:
+    from typing_extensions import ParamSpec, TypeAlias
+
+if TYPE_CHECKING:
+    from aiofiles.base import AiofilesContextManager
+    from aiofiles.threadpool.text import AsyncTextIOWrapper
+
+    # noinspection PyUnresolvedReferences
+    from configzen.model import ConfigModel
+    from configzen.route import ConfigRoute
+
+T = TypeVar("T")
+P = ParamSpec("P")
+
+ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
+ConfigRouteLike: TypeAlias = Union[str, list[str], "ConfigRoute"]
+
+ConfigIO: TypeAlias = contextlib.AbstractContextManager[TextIO]
+AsyncConfigIO: TypeAlias = "AiofilesContextManager[None, None, AsyncTextIOWrapper]"
+RawResourceT: TypeAlias = Union[ConfigIO, str, int, os.PathLike, pathlib.Path]
+NormalizedResourceT: TypeAlias = Union[ConfigIO, str, int, pathlib.Path]
+IncludeExcludeT: TypeAlias = Optional[
+    Union[
+        Set[Union[int, str]],
+        Mapping[Union[int, str], Any],
+    ]
+]
```

### Comparing `configzen-0.5.6/LICENSE` & `configzen-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.5.6/pyproject.toml` & `configzen-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,62 @@
-[tool.poetry]
-name = "configzen"
-version = "0.5.6"
-description = "The easiest way to manage configuration files in Python"
-authors = ["bswck <bswck.dev@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/bswck/configzen"
-
-[tool.poetry.dependencies]
-python = "^3.9"
-pydantic = "^1.10.10"
-anyconfig = "^0.13.0"
-typing-extensions = { version = "^4.5.0", python = ">=3.9,<3.11" }
-aiofiles = { version = "^23.1.0" }
-pyyaml = { version = "^6.0" }
-toml = { version = "^0.10.2" }
-
-[tool.poetry.group.dev.dependencies]
-ruff = "^0.0.267"
-mypy = "^1.3.0"
-black = "^23.3.0"
-pytest = "^7.3.1"
-mkdocs = "^1.4.3"
-mkdocstrings = "^0.22.0"
-pylint = "^2.17.4"
-anyconfig-ion-backend = "^0.1.1"
-anyconfig-bson-backend = "^0.1.2"
-anyconfig-cbor2-backend = "^0.1.2"
-anyconfig-cbor-backend = "^0.1.2"
-anyconfig-configobj-backend = "^0.1.4"
-anyconfig-msgpack-backend = "^0.1.1"
-
-[tool.ruff]
-target-version = "py39"
-select = [
-    "F", "E", "W", "I", "UP", "N", "S", "C", "B", "A", "T", "Q", "RUF", "YTT", "BLE", "ANN", "FBT", "PL", "TRY", "RSE",
-    "SLF", "DTZ", "EXE", "ISC", "ICN", "G", "INP", "PIE", "RET", "SIM", "TID", "TCH", "ARG", "PTH"
-]
-ignore = [
-    "DTZ005", "INP001", "TCH003", "ANN101", "ANN102", "ANN401", "I001", "TID252", "T201", "B905", "S101", "TRY003",
-    "PLR2004"
-]
-fix = true
-exclude = ["examples/", "tests/"]
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "configzen"
+version = "0.6.0"
+description = "The easiest way to manage configuration files in Python"
+authors = ["bswck <bswck.dev@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/bswck/configzen"
+
+[tool.poetry.dependencies]
+python = "^3.9"
+pydantic = "^1.10.10"
+anyconfig = "^0.13.0"
+typing-extensions = { version = "^4.5.0", python = ">=3.9,<3.11" }
+aiofiles = { version = "^23.1.0" }
+pyyaml = { version = "^6.0" }
+toml = { version = "^0.10.2" }
+click = "^8.1.3"
+pytest = "^7.4.0"
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.267"
+mypy = "^1.3.0"
+black = "^23.3.0"
+pytest = "^7.3.1"
+mkdocs = "^1.4.3"
+mkdocstrings = "^0.22.0"
+pylint = "^2.17.4"
+anyconfig-ion-backend = "^0.1.1"
+anyconfig-bson-backend = "^0.1.2"
+anyconfig-cbor2-backend = "^0.1.2"
+anyconfig-cbor-backend = "^0.1.2"
+anyconfig-configobj-backend = "^0.1.4"
+anyconfig-msgpack-backend = "^0.1.1"
+
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.18"
+mkdocstrings = "^0.22.0"
+mkdocstrings-python = "^1.1.2"
+jinja2 = "<3.1.0"
+
+[tool.ruff]
+target-version = "py39"
+select = [
+    "F", "E", "W", "I", "UP", "N", "S", "C", "B", "A", "T", "Q", "RUF", "YTT", "BLE", "ANN", "FBT", "PL", "TRY", "RSE",
+    "SLF", "DTZ", "EXE", "ISC", "ICN", "G", "INP", "PIE", "RET", "SIM", "TID", "TCH", "ARG", "PTH"
+]
+ignore = [
+    "DTZ005", "INP001", "TCH003", "ANN101", "ANN102", "ANN401", "I001", "TID252", "T201", "B905", "S101", "TRY003",
+    "PLR2004"
+]
+fix = true
+exclude = ["examples/", "tests/"]
+
+#[tool.poetry.scripts]
+#configzen = "configzen.__main__:main"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `configzen-0.5.6/README.md` & `configzen-0.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,334 +1,402 @@
-# configzen
-
-_configzen_ – easily create and maintain complex, statically-typed configurations with validation in Python.
-
-## What is this?
-
-_configzen_ is a good choice if you need to create complex configurations with schemas.
-Being based on [pydantic](https://docs.pydantic.dev/latest/), this tool will allow you to create _configuration models_
-for your configuration files, and then load, modify and save them with scope control.
-To see roughly how it works, check out the [Features](#features) section.
-
-### Preprocessing
-
-_configzen_ provides built-in preprocessing directives to your configuration files,
-offering features such as extending configuration files directly from other configuration files (without writing any
-code).
-You might think of it as something that is analogous
-to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
-broadened to any from the supported configuration file formats (see [Supported file formats](#supported-file-formats)).
-The directive `^copy` may also be handy in quick conversions between the mentioned formats.
-See [Preprocessing directives](#preprocessing-directives) for more information.
-
-## Supported file formats
-
-_configzen_ uses [anyconfig](https://pypi.org/project/anyconfig/) to serialize and deserialize data and does not operate on any protocol-specific entities.
-As an example result, comments in your configuration files are lost on save[^1], but you can exchange file formats without any hassle.
-
-The following table shows the supported file formats, their requirements, file extensions, and the backend libraries used to accomplish this goal.
-
-| File Format                                                                         | To use, install:              | Recognized File Extension(s) | Backend Library                                                                                         |
-|-------------------------------------------------------------------------------------|-------------------------------|------------------------------|---------------------------------------------------------------------------------------------------------|
-| [JSON](https://en.wikipedia.org/wiki/JSON)                                          | -                             | `json`                       | [json](https://docs.python.org/3/library/json.html) (standard library)                                  |
-| [INI](https://en.wikipedia.org/wiki/INI_file)                                       | -                             | `ini`, `cfg`, `conf`         | [configparser](https://docs.python.org/3/library/configparser.html) (standard library)                  |
-| [TOML](https://en.wikipedia.org/wiki/TOML)                                          | -                             | `toml`                       | [toml](https://pypi.python.org/pypi/toml)                                                               |
-| [YAML](https://yaml.org)                                                            | -                             | `yaml`, `yml`                | [pyyaml](https://pypi.python.org/pypi/PyYAML) / [ruamel.yml](https://pypi.python.org/pypi/ruamel.yml) |
-| [XML](https://en.wikipedia.org/wiki/XML)                                            | -                             | `xml`                        | [xml](https://docs.python.org/3/library/xml.html) (standard library)                                    |
-| [BSON](https://en.wikipedia.org/wiki/BSON)                                          | `anyconfig-bson-backend`      | `bson`                       | [bson](https://pypi.org/project/bson/)                                                                  |
-| [CBOR](https://cbor.io/) ([RFC 8949](https://www.rfc-editor.org/rfc/rfc8949))       | `anyconfig-cbor2-backend`     | `cbor`, `cbor2`              | [cbor2](https://pypi.org/project/cbor2/)                                                                |
-| CBOR (deprecated, [RFC 7049](https://www.rfc-editor.org/rfc/rfc7049))               | `anyconfig-cbor-backend`      | `cbor`                       | [cbor](https://pypi.org/project/cbor/)                                                                  |
-| properties                                                                          | -                             | `properties`                 | (native)                                                                                                |
-| shellvars                                                                           | -                             | `shellvars`                  | (native)                                                                                                |
-
-[//]: # (| [ConfigObj]&#40;https://configobj.readthedocs.io/en/latest/configobj.html#introduction&#41; | `anyconfig-configobj-backend` | `configobj`                  | [configobj]&#40;https://pypi.org/project/configobj/&#41;                                                        |)
-[//]: # (| [Amazon Ion]&#40;https://en.wikipedia.org/wiki/Ion_&#40;serialization_format&#41;&#41;              | `anyconfig-ion-backend`       | `ion`                        | [ion]&#40;https://pypi.org/project/amazon.ion/&#41;                                                             |)
-[//]: # (| [MessagePack]&#40;https://en.wikipedia.org/wiki/MessagePack&#41;                            | `anyconfig-msgpack-backend`   | `msgpack`, `mpk`             | [msgpack]&#40;https://pypi.org/project/msgpack/&#41;                                                            |)
-
-If your file extension is not recognized, you can register your own file extension by calling `ConfigAgent.register_file_extension(file_extension, parser_name)`.
-
-If your favorite backend library is not supported, please let me know by reporting it as an issue.
-Using custom backends is to be supported in the future.
-
-[^1]: A suggested alternative for comments is to use the `description` parameter in your configuration models' fields: `ConfigField(description=...)`.
-The provided field descriptions are included in JSON schemas generated by the default implementation of the `ConfigModel.schema()` method.
-
-## Features
-
-### Managing content
-
-Having a YAML configuration file like this:
-
-```yaml
-# database.yml
-host: 127.0.0.1
-port: 5432
-user: postgres
-```
-
-You can create a _configzen_ configuration model for it like this:
-
-```python
-# config.py
-from ipaddress import IPv4Address, IPv6Address
-from configzen import ConfigModel, ConfigMeta, ConfigField
-
-
-class DatabaseConfig(ConfigModel):
-    host: IPv4Address | IPv6Address
-    port: int
-    user: str
-    password: str = ConfigField(exclude=True)
-
-    class Config(ConfigMeta):
-        resource = "database.yml"
-        env_prefix = "DB_"
-
-
-db_config = DatabaseConfig.load()
-```
-
-With this code written, you can load your configuration from a file as well as from the environment variables
-`DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with
-the option `exclude=True`, it will not be included in the configuration's exported data: that
-guarantees that your password does never leak into `database.yml` on save – but you may still pass it
-through an environment variable (here – the mentioned `DB_PASSWORD`). Secret files are also supported,
-see [the pydantic documentation](https://docs.pydantic.dev/latest/usage/settings/#secret-support) section
-for more information.
-
-[pydantic](https://docs.pydantic.dev/latest/) will naturally take care of parsing and validating the loaded data.
-Configuration models inherit from the `pydantic.BaseSettings` class, so you can use all of its features:
-schema generation, type conversion, validation, etc.
-
-There are additional features brought to you by _configzen_ worth checking out, though.
-
-You can use the `db_config` object defined above to access the configuration values:
-
-```python
->>> db_config.host
-IPv4Address('127.0.0.1')
-```
-
-modify them, if the pydantic model validation allows
-it ([`<Your model>.Config.validate_assignment`](https://docs.pydantic.dev/latest/usage/model_config/#options) will
-be `True` by default):
-
-```python
->>> db_config.host = "0.0.0.0"
->>> db_config.host
-IPv4Address('0.0.0.0')
-```
-
-as well as reload particular values, without touching the rest of the configuration:
-
-```python
->>> db_config.at("port").reload()
-5432
->>> db_config
-DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
->>> db_config.at("host").reload()
-IPv4Address('127.0.0.1')
->>> db_config
-DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
-```
-
-or reload the whole configuration:
-
-```python
->>> db_config.port = 1234
->>> db_config.reload()
-DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
-```
-
-or save a particular value, without touching the rest of the configuration:
-
-```python
->>> db_config.host = "0.0.0.0"
->>> db_config.port = 443
->>> db_config
-DatabaseConfig(host=IPv4Address('0.0.0.0'), port=443, user='postgres', password='password')
->>> db_config.at("host").save()
-40
->>> db_config.reload()
-DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
-```
-
-or save the whole configuration:
-
-```python
->>> db_config.save()
-39
-```
-
-### Preprocessing
-
-To see supported preprocessing directives,
-see [Supported preprocessing directives](#supported-preprocessing-directives).
-
-#### Basic usage
-
-Having a base configuration file like this (`base.json`):
-
-```json
-{
-  "i18n": {
-    "language": "en",
-    "timezone": "UTC"
-  },
-  "app": {
-    "debug": true,
-    "expose": 8000
-  }
-}
-```
-
-create another configuration file like this, overriding desired sections as needed:
-
-```yaml
-# production.yml
-^extend: base.json
-
-+app:
-  debug: false
-```
-
-and load the `production.yml` configuration file. No explicit changes to the code indicating the use of the `base.json`
-file are needed.
-
-_Note: Using `+` in front of a key will update the section already defined at that key,
-instead of replacing it._
-
-Notice how configuration file formats do not matter in _configzen_: you can
-extend JSON configurations with YAML, but that might be as well any other format
-among the supported ones (see the [Supported file formats](#supported-file-formats) section).
-
-The above example is equivalent to as if you used:
-
-```yaml
-# production.yml
-i18n:
-  language: en
-  timezone: UTC
-app:
-  debug: false
-  expose: 8000
-```
-
-but with a significant difference: when you save the above configuration, the `^extend` relation to the base
-configuration file `base.json` is preserved.
-This basically means that changes made in the base configuration file will apply to the configuration model instance
-loaded from the `^extend`-ing configuration file.
-Any changes made locally to the model will result in `+` sections being automatically added to the exported
-configuration data.
-
-#### Supported preprocessing directives
-
-| Directive  | Is the referenced file preprocessed? | Is the directive preserved on export? |
-|------------|--------------------------------------|---------------------------------------|
-| `^extend`  | Yes                                  | Yes                                   |
-| `^include` | Yes                                  | No                                    |
-| `^copy`    | No                                   | No                                    |
-
-
-### Interpolation
-
-#### Basic interpolation
-
-You can use interpolation in your configuration files:
-
-```yaml
-cpu:
-  cores: 4
-num_workers: ${cpu.cores}
-```
-
-```python
->>> from configzen import ConfigModel
-...
->>> class CPUConfig(ConfigModel):
-...     cores: int
-...
->>> class AppConfig(ConfigModel):
-...     cpu: CPUConfig
-...     num_workers: int
-...
->>> app_config = AppConfig.load("app.yml")
->>> app_config
-AppConfig(cpu=CPUConfig(cores=4), num_workers=4)
-```
-
-
-#### Reusable configuration with namespaces
-
-You can share independent configuration models as namespaces through inclusion:
-
-```yaml
-# database.yml
-host: ${app_config::db_host}
-port: ${app_config::expose}
-```
-
-```yaml
-# app.yml
-db_host: localhost
-expose: 8000
-```
-
-```python
->>> from configzen import ConfigModel, include
->>> from ipaddress import IPv4Address
->>>
->>> @include("app_config")
-... class DatabaseConfig(ConfigModel):
-...     host: IPv4Address
-...     port: int
-...
->>> class AppConfig(ConfigModel):
-...     db_host: str
-...     expose: int
-...
->>> app_config = AppConfig.load("app.yml")
->>> app_config
-AppConfig(db_host='localhost', expose=8000)
->>> db_config = DatabaseConfig.load("database.yml")
->>> db_config
-DatabaseConfig(host=IPv4Address('127.0.0.1'), port=8000)
->>> db_config.dict()
-{'host': IPv4Address('127.0.0.1'), 'port': 8000}
->>> db_config.export()  # used when saving
-{'host': '${app_config::db_host}', 'port': '${app_config::expose}'}
-```
-
-You do not have to pass a variable name to `@include`, though. `@include` lets you overwrite the main interpolation namespace
-or one with a separate name (here: `app_config`) with configuration models, dictionaries and their factories.
-
-## Setup
-
-In order to use _configzen_ in your project, install it with your package manager, for example `pip`:
-
-```bash
-pip install configzen
-```
-
-If you are willing to contribute to the project, which is awesome, simply clone the repository and install its
-dependencies with [poetry](https://python-poetry.org/):
-
-```bash
-poetry install --with dev
-```
-
-## License
-
-[MIT License](https://choosealicense.com/licenses/mit/)
-
-## Contributing
-
-Contributions are welcome! Feel free to [open an issue](https://github.com/bswck/configzen/issues/new/choose)
-or [submit a pull request](https://github.com/bswck/configzen/compare).
-
-## Credits
-
-* [@Lunarmagpie](https://github.com/Lunarmagpie) for _crucial_ design tips and ideas.
-
-## Author
-
-* [bswck](https://github.com/bswck) (contact: bswck.dev@gmail.com or via [Discord](https://discord.com/) `bswck#8238`)
+# configzen
+
+_configzen_ – easily create and maintain complex, statically-typed configurations with validation in Python.
+
+## Features
+
+### Managing content
+
+Having a YAML configuration file like this:
+
+```yaml
+# database.yml
+host: 127.0.0.1
+port: 5432
+user: postgres
+```
+
+You can create a _configzen_ configuration model for it like this:
+
+```python
+# model.py
+from ipaddress import IPv4Address, IPv6Address
+from configzen import ConfigModel, ConfigMeta, ConfigField
+
+
+class DatabaseConfig(ConfigModel):
+    host: IPv4Address | IPv6Address
+    port: int
+    user: str
+    password: str = ConfigField(exclude=True)
+
+    class Config(ConfigMeta):
+        resource = "database.yml"
+        env_prefix = "DB_"
+
+
+db_config = DatabaseConfig.load()
+```
+
+And you can load your configuration from a file as well as from the environment variables
+`DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with
+the option `exclude=True`, it will not be included in the configuration's exported data: that
+guarantees that your password does never leak into `database.yml` on save – but you may still pass it
+through an environment variable (here – the mentioned `DB_PASSWORD`). Secret files are also supported,
+see [the pydantic documentation](https://docs.pydantic.dev/latest/usage/settings/#secret-support)
+for more information.
+
+[pydantic](https://docs.pydantic.dev/latest/) will naturally take care of parsing and validating the loaded data.
+Configuration models inherit from the `pydantic.BaseSettings` class, so you can use all of its features:
+schema generation, type conversion, validation, etc.
+
+There are additional features brought to you by _configzen_ worth checking out, though.
+
+You can use the `db_config` object defined above to access the configuration values:
+
+```python
+>>> db_config.host
+IPv4Address('127.0.0.1')
+```
+
+modify them, if the pydantic model validation allows
+it ([`<Your model>.Config.validate_assignment`](https://docs.pydantic.dev/latest/usage/model_config/#options) will
+be `True` by default):
+
+```python
+>>> db_config.host = "0.0.0.0"
+>>> db_config.host
+IPv4Address('0.0.0.0')
+```
+
+as well as reload particular values, without touching the rest of the configuration:
+
+```python
+>>> db_config.at("port").reload()
+5432
+>>> db_config
+DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
+>>> db_config.at("host").reload()
+IPv4Address('127.0.0.1')
+>>> db_config
+DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
+```
+
+or reload the whole configuration:
+
+```python
+>>> db_config.port = 1234
+>>> db_config.reload()
+DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
+```
+
+or save a particular value, without touching the rest of the configuration:
+
+```python
+>>> db_config.host = "0.0.0.0"
+>>> db_config.port = 443
+>>> db_config
+DatabaseConfig(host=IPv4Address('0.0.0.0'), port=443, user='postgres', password='password')
+>>> db_config.at("host").save()
+40
+>>> db_config.reload()
+DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
+```
+
+or save the whole configuration:
+
+```python
+>>> db_config.save()
+39
+```
+
+### Preprocessing
+
+To see supported preprocessing directives,
+see [Supported preprocessing directives](#supported-preprocessing-directives).
+
+#### Basic usage
+
+Having a base configuration file like this (`base.json`):
+
+```json
+{
+  "i18n": {
+    "language": "en",
+    "timezone": "UTC"
+  },
+  "app": {
+    "debug": true,
+    "expose": 8000
+  }
+}
+```
+
+create another configuration file like this, overriding desired sections as needed:
+
+```yaml
+# production.yml
+^extend: base.json
+
++app:
+  debug: false
+```
+
+and load the `production.yml` configuration file. No explicit changes to the code indicating the use of the `base.json`
+file are needed.
+
+_Note: Using `+` in front of a key will update the section already defined at that key,
+instead of replacing it._
+
+Notice how configuration file formats do not matter in _configzen_: you can
+extend JSON configurations with YAML, but that might be as well any other format
+among the supported ones (see the [Supported file formats](#supported-file-formats) section).
+
+The above example is equivalent to as if you used:
+
+```yaml
+# production.yml
+i18n:
+  language: en
+  timezone: UTC
+app:
+  debug: false
+  expose: 8000
+```
+
+but with a significant difference: when you save the above configuration, the `^extend` relation to the base
+configuration file `base.json` is preserved.
+This basically means that changes made in the base configuration file will apply to the configuration model instance
+loaded from the `^extend`-ing configuration file.
+Any changes made locally to the model will result in `+` sections being automatically added to the exported
+configuration data.
+
+#### Supported preprocessing directives
+
+| Directive  | Is the referenced file preprocessed? | Is the directive preserved on export? |
+|------------|--------------------------------------|---------------------------------------|
+| `^extend`  | Yes                                  | Yes                                   |
+| `^include` | Yes                                  | No                                    |
+| `^copy`    | No                                   | No                                    |
+
+
+### Interpolation
+
+#### Basic interpolation
+
+You can use interpolation in your configuration files:
+
+```yaml
+cpu:
+  cores: 4
+num_workers: ${cpu.cores}
+```
+
+```python
+>>> from configzen import ConfigModel
+...
+>>> class CPUConfig(ConfigModel):
+...     cores: int
+...
+>>> class AppConfig(ConfigModel):
+...     cpu: CPUConfig
+...     num_workers: int
+...
+>>> app_config = AppConfig.load("app.yml")
+>>> app_config
+AppConfig(cpu=CPUConfig(cores=4), num_workers=4)
+```
+
+
+#### Reusable configuration with namespaces
+
+You can share independent configuration models as namespaces through inclusion:
+
+```yaml
+# database.yml
+host: ${app_config::db_host}
+port: ${app_config::expose}
+```
+
+```yaml
+# app.yml
+db_host: localhost
+expose: 8000
+```
+
+```python
+>>> from configzen import ConfigModel, include
+>>> from ipaddress import IPv4Address
+>>>
+>>> @include("app_config")
+... class DatabaseConfig(ConfigModel):
+...     host: IPv4Address
+...     port: int
+...
+>>> class AppConfig(ConfigModel):
+...     db_host: str
+...     expose: int
+...
+>>> app_config = AppConfig.load("app.yml")
+>>> app_config
+AppConfig(db_host='localhost', expose=8000)
+>>> db_config = DatabaseConfig.load("database.yml")
+>>> db_config
+DatabaseConfig(host=IPv4Address('127.0.0.1'), port=8000)
+>>> db_config.dict()
+{'host': IPv4Address('127.0.0.1'), 'port': 8000}
+>>> db_config.export()  # used when saving
+{'host': '${app_config::db_host}', 'port': '${app_config::expose}'}
+```
+
+You do not have to pass a variable name to `@include`, though. `@include` lets you overwrite the main interpolation namespace
+or one with a separate name (here: `app_config`) with configuration models, dictionaries and their factories.
+
+
+### Modular configuration
+
+#### Wrapping modules in-place
+
+You can wrap modules in-place with configuration models:
+
+
+1) Without writing a model class:
+
+```python
+# config.py
+from configzen import ConfigModule
+
+HOST: str = "localhost"
+PORT: int = 8000
+
+ConfigModule.wrap_this_module()
+```
+
+2) With a model class:
+
+```python
+# config.py
+from configzen import ConfigModel
+
+class AppConfig(ConfigModel):
+    HOST: str = "localhost"
+    PORT: int = 8000
+    
+AppConfig.wrap_this_module()
+```
+
+Now values `HOST` and `PORT` will be validated as `str` and `int` data types, respectively:
+
+```python
+>>> import config  # <configuration module 'config' from 'config.py'>
+>>> config.HOST
+'localhost'
+>>> config.PORT
+8000
+>>> config.PORT = "8000"
+>>> config.PORT
+8000
+>>> config.PORT = "abc"
+Traceback (most recent call last):
+  ...
+```
+
+#### Wrapping interchangeable modules
+
+You can wrap modules outside them with configuration models:
+
+```python
+# setup.py
+from configzen import ConfigModel
+
+class AppConfig(ConfigModel):
+    HOST: str = "localhost"
+    PORT: int = 8000
+
+config_model = AppConfig.wrap_module("config")
+```
+
+```py
+# config.py
+HOST: str = "0.0.0.0"
+PORT: int = 443
+```
+
+```python
+>>> from setup import config_model
+>>> config_model.HOST
+'0.0.0.0'
+>>> config_model.PORT
+443
+>>> config_model.PORT = "8000"
+>>> config_model.PORT
+8000
+>>> import config
+>>> config.HOST
+'0.0.0.0'
+>>> config.PORT
+8000
+```
+
+## Supported file formats
+
+_configzen_ uses [anyconfig](https://pypi.org/project/anyconfig/) to serialize and deserialize data and does not operate on any protocol-specific entities.
+As an example result, comments in your configuration files are lost on save[^1], but you can exchange file formats without any hassle.
+
+The following table shows the supported file formats, their requirements, file extensions, and the backend libraries used to accomplish this goal.
+
+| File Format                                                                         | To use, install:              | Recognized File Extension(s) | Backend Library                                                                                         |
+|-------------------------------------------------------------------------------------|-------------------------------|------------------------------|---------------------------------------------------------------------------------------------------------|
+| [JSON](https://en.wikipedia.org/wiki/JSON)                                          | -                             | `json`                       | [json](https://docs.python.org/3/library/json.html) (standard library)                                  |
+| [INI](https://en.wikipedia.org/wiki/INI_file)                                       | -                             | `ini`, `cfg`, `conf`         | [configparser](https://docs.python.org/3/library/configparser.html) (standard library)                  |
+| [TOML](https://en.wikipedia.org/wiki/TOML)                                          | -                             | `toml`                       | [toml](https://pypi.python.org/pypi/toml)                                                               |
+| [YAML](https://yaml.org)                                                            | -                             | `yaml`, `yml`                | [pyyaml](https://pypi.python.org/pypi/PyYAML) / [ruamel.yml](https://pypi.python.org/pypi/ruamel.yml) |
+| [XML](https://en.wikipedia.org/wiki/XML)                                            | -                             | `xml`                        | [xml](https://docs.python.org/3/library/xml.html) (standard library)                                    |
+| [BSON](https://en.wikipedia.org/wiki/BSON)                                          | `anyconfig-bson-backend`      | `bson`                       | [bson](https://pypi.org/project/bson/)                                                                  |
+| [CBOR](https://cbor.io/) ([RFC 8949](https://www.rfc-editor.org/rfc/rfc8949))       | `anyconfig-cbor2-backend`     | `cbor`, `cbor2`              | [cbor2](https://pypi.org/project/cbor2/)                                                                |
+| CBOR (deprecated, [RFC 7049](https://www.rfc-editor.org/rfc/rfc7049))               | `anyconfig-cbor-backend`      | `cbor`                       | [cbor](https://pypi.org/project/cbor/)                                                                  |
+| properties                                                                          | -                             | `properties`                 | (native)                                                                                                |
+| shellvars                                                                           | -                             | `shellvars`                  | (native)                                                                                                |
+
+[//]: # (| [ConfigObj]&#40;https://configobj.readthedocs.io/en/latest/configobj.html#introduction&#41; | `anyconfig-configobj-backend` | `configobj`                  | [configobj]&#40;https://pypi.org/project/configobj/&#41;                                                        |)
+[//]: # (| [Amazon Ion]&#40;https://en.wikipedia.org/wiki/Ion_&#40;serialization_format&#41;&#41;              | `anyconfig-ion-backend`       | `ion`                        | [ion]&#40;https://pypi.org/project/amazon.ion/&#41;                                                             |)
+[//]: # (| [MessagePack]&#40;https://en.wikipedia.org/wiki/MessagePack&#41;                            | `anyconfig-msgpack-backend`   | `msgpack`, `mpk`             | [msgpack]&#40;https://pypi.org/project/msgpack/&#41;                                                            |)
+
+If your file extension is not recognized, you can register your own file extension by calling `ConfigAgent.register_file_extension(file_extension, parser_name)`.
+
+If your favorite backend library is not supported, please let me know by reporting it as an issue.
+Using custom backends is to be supported in the future.
+
+[^1]: A suggested alternative for comments is to use the `description` parameter in your configuration models' fields: `ConfigField(description=...)`.
+The provided field descriptions are included in JSON schemas generated by the default implementation of the `ConfigModel.schema()` method.
+
+## Setup
+
+In order to use _configzen_ in your project, install it with your package manager, for example `pip`:
+
+```bash
+pip install configzen
+```
+
+If you are willing to contribute to the project, which is awesome, simply clone the repository and install its
+dependencies with [poetry](https://python-poetry.org/):
+
+```bash
+poetry install --with dev
+```
+
+## License
+
+[MIT License](https://choosealicense.com/licenses/mit/)
+
+## Contributing
+
+Contributions are welcome! Feel free to [open an issue](https://github.com/bswck/configzen/issues/new/choose)
+or [submit a pull request](https://github.com/bswck/configzen/compare).
+
+## Credits
+
+* [@Lunarmagpie](https://github.com/Lunarmagpie) for _crucial_ design tips and ideas.
+
+## Author
+
+* [bswck](https://github.com/bswck) (contact: bswck.dev@gmail.com or via [Discord](https://discord.com/) `bswck#8238`)
```

### Comparing `configzen-0.5.6/PKG-INFO` & `configzen-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,35 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.5.6
+Version: 0.6.0
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: anyconfig (>=0.13.0,<0.14.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pydantic (>=1.10.10,<2.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version >= "3.9" and python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # configzen
 
 _configzen_ – easily create and maintain complex, statically-typed configurations with validation in Python.
 
-## What is this?
-
-_configzen_ is a good choice if you need to create complex configurations with schemas.
-Being based on [pydantic](https://docs.pydantic.dev/latest/), this tool will allow you to create _configuration models_
-for your configuration files, and then load, modify and save them with scope control.
-To see roughly how it works, check out the [Features](#features) section.
-
-### Preprocessing
-
-_configzen_ provides built-in preprocessing directives to your configuration files,
-offering features such as extending configuration files directly from other configuration files (without writing any
-code).
-You might think of it as something that is analogous
-to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
-broadened to any from the supported configuration file formats (see [Supported file formats](#supported-file-formats)).
-The directive `^copy` may also be handy in quick conversions between the mentioned formats.
-See [Preprocessing directives](#preprocessing-directives) for more information.
-
-## Supported file formats
-
-_configzen_ uses [anyconfig](https://pypi.org/project/anyconfig/) to serialize and deserialize data and does not operate on any protocol-specific entities.
-As an example result, comments in your configuration files are lost on save[^1], but you can exchange file formats without any hassle.
-
-The following table shows the supported file formats, their requirements, file extensions, and the backend libraries used to accomplish this goal.
-
-| File Format                                                                         | To use, install:              | Recognized File Extension(s) | Backend Library                                                                                         |
-|-------------------------------------------------------------------------------------|-------------------------------|------------------------------|---------------------------------------------------------------------------------------------------------|
-| [JSON](https://en.wikipedia.org/wiki/JSON)                                          | -                             | `json`                       | [json](https://docs.python.org/3/library/json.html) (standard library)                                  |
-| [INI](https://en.wikipedia.org/wiki/INI_file)                                       | -                             | `ini`, `cfg`, `conf`         | [configparser](https://docs.python.org/3/library/configparser.html) (standard library)                  |
-| [TOML](https://en.wikipedia.org/wiki/TOML)                                          | -                             | `toml`                       | [toml](https://pypi.python.org/pypi/toml)                                                               |
-| [YAML](https://yaml.org)                                                            | -                             | `yaml`, `yml`                | [pyyaml](https://pypi.python.org/pypi/PyYAML) / [ruamel.yml](https://pypi.python.org/pypi/ruamel.yml) |
-| [XML](https://en.wikipedia.org/wiki/XML)                                            | -                             | `xml`                        | [xml](https://docs.python.org/3/library/xml.html) (standard library)                                    |
-| [BSON](https://en.wikipedia.org/wiki/BSON)                                          | `anyconfig-bson-backend`      | `bson`                       | [bson](https://pypi.org/project/bson/)                                                                  |
-| [CBOR](https://cbor.io/) ([RFC 8949](https://www.rfc-editor.org/rfc/rfc8949))       | `anyconfig-cbor2-backend`     | `cbor`, `cbor2`              | [cbor2](https://pypi.org/project/cbor2/)                                                                |
-| CBOR (deprecated, [RFC 7049](https://www.rfc-editor.org/rfc/rfc7049))               | `anyconfig-cbor-backend`      | `cbor`                       | [cbor](https://pypi.org/project/cbor/)                                                                  |
-| properties                                                                          | -                             | `properties`                 | (native)                                                                                                |
-| shellvars                                                                           | -                             | `shellvars`                  | (native)                                                                                                |
-
-[//]: # (| [ConfigObj]&#40;https://configobj.readthedocs.io/en/latest/configobj.html#introduction&#41; | `anyconfig-configobj-backend` | `configobj`                  | [configobj]&#40;https://pypi.org/project/configobj/&#41;                                                        |)
-[//]: # (| [Amazon Ion]&#40;https://en.wikipedia.org/wiki/Ion_&#40;serialization_format&#41;&#41;              | `anyconfig-ion-backend`       | `ion`                        | [ion]&#40;https://pypi.org/project/amazon.ion/&#41;                                                             |)
-[//]: # (| [MessagePack]&#40;https://en.wikipedia.org/wiki/MessagePack&#41;                            | `anyconfig-msgpack-backend`   | `msgpack`, `mpk`             | [msgpack]&#40;https://pypi.org/project/msgpack/&#41;                                                            |)
-
-If your file extension is not recognized, you can register your own file extension by calling `ConfigAgent.register_file_extension(file_extension, parser_name)`.
-
-If your favorite backend library is not supported, please let me know by reporting it as an issue.
-Using custom backends is to be supported in the future.
-
-[^1]: A suggested alternative for comments is to use the `description` parameter in your configuration models' fields: `ConfigField(description=...)`.
-The provided field descriptions are included in JSON schemas generated by the default implementation of the `ConfigModel.schema()` method.
-
 ## Features
 
 ### Managing content
 
 Having a YAML configuration file like this:
 
 ```yaml
@@ -86,15 +38,15 @@
 port: 5432
 user: postgres
 ```
 
 You can create a _configzen_ configuration model for it like this:
 
 ```python
-# config.py
+# model.py
 from ipaddress import IPv4Address, IPv6Address
 from configzen import ConfigModel, ConfigMeta, ConfigField
 
 
 class DatabaseConfig(ConfigModel):
     host: IPv4Address | IPv6Address
     port: int
@@ -105,20 +57,20 @@
         resource = "database.yml"
         env_prefix = "DB_"
 
 
 db_config = DatabaseConfig.load()
 ```
 
-With this code written, you can load your configuration from a file as well as from the environment variables
+And you can load your configuration from a file as well as from the environment variables
 `DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with
 the option `exclude=True`, it will not be included in the configuration's exported data: that
 guarantees that your password does never leak into `database.yml` on save – but you may still pass it
 through an environment variable (here – the mentioned `DB_PASSWORD`). Secret files are also supported,
-see [the pydantic documentation](https://docs.pydantic.dev/latest/usage/settings/#secret-support) section
+see [the pydantic documentation](https://docs.pydantic.dev/latest/usage/settings/#secret-support)
 for more information.
 
 [pydantic](https://docs.pydantic.dev/latest/) will naturally take care of parsing and validating the loaded data.
 Configuration models inherit from the `pydantic.BaseSettings` class, so you can use all of its features:
 schema generation, type conversion, validation, etc.
 
 There are additional features brought to you by _configzen_ worth checking out, though.
@@ -319,14 +271,132 @@
 >>> db_config.export()  # used when saving
 {'host': '${app_config::db_host}', 'port': '${app_config::expose}'}
 ```
 
 You do not have to pass a variable name to `@include`, though. `@include` lets you overwrite the main interpolation namespace
 or one with a separate name (here: `app_config`) with configuration models, dictionaries and their factories.
 
+
+### Modular configuration
+
+#### Wrapping modules in-place
+
+You can wrap modules in-place with configuration models:
+
+
+1) Without writing a model class:
+
+```python
+# config.py
+from configzen import ConfigModule
+
+HOST: str = "localhost"
+PORT: int = 8000
+
+ConfigModule.wrap_this_module()
+```
+
+2) With a model class:
+
+```python
+# config.py
+from configzen import ConfigModel
+
+class AppConfig(ConfigModel):
+    HOST: str = "localhost"
+    PORT: int = 8000
+    
+AppConfig.wrap_this_module()
+```
+
+Now values `HOST` and `PORT` will be validated as `str` and `int` data types, respectively:
+
+```python
+>>> import config  # <configuration module 'config' from 'config.py'>
+>>> config.HOST
+'localhost'
+>>> config.PORT
+8000
+>>> config.PORT = "8000"
+>>> config.PORT
+8000
+>>> config.PORT = "abc"
+Traceback (most recent call last):
+  ...
+```
+
+#### Wrapping interchangeable modules
+
+You can wrap modules outside them with configuration models:
+
+```python
+# setup.py
+from configzen import ConfigModel
+
+class AppConfig(ConfigModel):
+    HOST: str = "localhost"
+    PORT: int = 8000
+
+config_model = AppConfig.wrap_module("config")
+```
+
+```py
+# config.py
+HOST: str = "0.0.0.0"
+PORT: int = 443
+```
+
+```python
+>>> from setup import config_model
+>>> config_model.HOST
+'0.0.0.0'
+>>> config_model.PORT
+443
+>>> config_model.PORT = "8000"
+>>> config_model.PORT
+8000
+>>> import config
+>>> config.HOST
+'0.0.0.0'
+>>> config.PORT
+8000
+```
+
+## Supported file formats
+
+_configzen_ uses [anyconfig](https://pypi.org/project/anyconfig/) to serialize and deserialize data and does not operate on any protocol-specific entities.
+As an example result, comments in your configuration files are lost on save[^1], but you can exchange file formats without any hassle.
+
+The following table shows the supported file formats, their requirements, file extensions, and the backend libraries used to accomplish this goal.
+
+| File Format                                                                         | To use, install:              | Recognized File Extension(s) | Backend Library                                                                                         |
+|-------------------------------------------------------------------------------------|-------------------------------|------------------------------|---------------------------------------------------------------------------------------------------------|
+| [JSON](https://en.wikipedia.org/wiki/JSON)                                          | -                             | `json`                       | [json](https://docs.python.org/3/library/json.html) (standard library)                                  |
+| [INI](https://en.wikipedia.org/wiki/INI_file)                                       | -                             | `ini`, `cfg`, `conf`         | [configparser](https://docs.python.org/3/library/configparser.html) (standard library)                  |
+| [TOML](https://en.wikipedia.org/wiki/TOML)                                          | -                             | `toml`                       | [toml](https://pypi.python.org/pypi/toml)                                                               |
+| [YAML](https://yaml.org)                                                            | -                             | `yaml`, `yml`                | [pyyaml](https://pypi.python.org/pypi/PyYAML) / [ruamel.yml](https://pypi.python.org/pypi/ruamel.yml) |
+| [XML](https://en.wikipedia.org/wiki/XML)                                            | -                             | `xml`                        | [xml](https://docs.python.org/3/library/xml.html) (standard library)                                    |
+| [BSON](https://en.wikipedia.org/wiki/BSON)                                          | `anyconfig-bson-backend`      | `bson`                       | [bson](https://pypi.org/project/bson/)                                                                  |
+| [CBOR](https://cbor.io/) ([RFC 8949](https://www.rfc-editor.org/rfc/rfc8949))       | `anyconfig-cbor2-backend`     | `cbor`, `cbor2`              | [cbor2](https://pypi.org/project/cbor2/)                                                                |
+| CBOR (deprecated, [RFC 7049](https://www.rfc-editor.org/rfc/rfc7049))               | `anyconfig-cbor-backend`      | `cbor`                       | [cbor](https://pypi.org/project/cbor/)                                                                  |
+| properties                                                                          | -                             | `properties`                 | (native)                                                                                                |
+| shellvars                                                                           | -                             | `shellvars`                  | (native)                                                                                                |
+
+[//]: # (| [ConfigObj]&#40;https://configobj.readthedocs.io/en/latest/configobj.html#introduction&#41; | `anyconfig-configobj-backend` | `configobj`                  | [configobj]&#40;https://pypi.org/project/configobj/&#41;                                                        |)
+[//]: # (| [Amazon Ion]&#40;https://en.wikipedia.org/wiki/Ion_&#40;serialization_format&#41;&#41;              | `anyconfig-ion-backend`       | `ion`                        | [ion]&#40;https://pypi.org/project/amazon.ion/&#41;                                                             |)
+[//]: # (| [MessagePack]&#40;https://en.wikipedia.org/wiki/MessagePack&#41;                            | `anyconfig-msgpack-backend`   | `msgpack`, `mpk`             | [msgpack]&#40;https://pypi.org/project/msgpack/&#41;                                                            |)
+
+If your file extension is not recognized, you can register your own file extension by calling `ConfigAgent.register_file_extension(file_extension, parser_name)`.
+
+If your favorite backend library is not supported, please let me know by reporting it as an issue.
+Using custom backends is to be supported in the future.
+
+[^1]: A suggested alternative for comments is to use the `description` parameter in your configuration models' fields: `ConfigField(description=...)`.
+The provided field descriptions are included in JSON schemas generated by the default implementation of the `ConfigModel.schema()` method.
+
 ## Setup
 
 In order to use _configzen_ in your project, install it with your package manager, for example `pip`:
 
 ```bash
 pip install configzen
 ```
```

