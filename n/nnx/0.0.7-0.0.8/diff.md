# Comparing `tmp/nnx-0.0.7.tar.gz` & `tmp/nnx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnx-0.0.7.tar", max compression
+gzip compressed data, was "nnx-0.0.8.tar", max compression
```

## Comparing `nnx-0.0.7.tar` & `nnx-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1072 2023-07-05 17:41:51.529317 nnx-0.0.7/LICENSE
--rw-r--r--   0        0        0    21250 2023-07-10 14:57:54.628800 nnx-0.0.7/README.md
--rw-r--r--   0        0        0     1410 2023-07-10 15:00:29.396804 nnx-0.0.7/nnx/__init__.py
--rw-r--r--   0        0        0     5241 2023-07-10 15:00:28.184804 nnx-0.0.7/nnx/containers.py
--rw-r--r--   0        0        0     5417 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/contextlib.py
--rw-r--r--   0        0        0     4512 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/dataclasses.py
--rw-r--r--   0        0        0       45 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/errors.py
--rw-r--r--   0        0        0     4345 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/helpers.py
--rw-r--r--   0        0        0     1832 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/ids.py
--rw-r--r--   0        0        0    26625 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/module.py
--rw-r--r--   0        0        0        0 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nn/__init__.py
--rw-r--r--   0        0        0      763 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nn/activations.py
--rw-r--r--   0        0        0     2763 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nn/dtypes.py
--rw-r--r--   0        0        0     2147 2023-07-08 19:31:09.240551 nnx-0.0.7/nnx/nn/initializers.py
--rw-r--r--   0        0        0    16022 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/nn/linear.py
--rw-r--r--   0        0        0    13511 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/nn/normalization.py
--rw-r--r--   0        0        0     2281 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nn/stochastic.py
--rw-r--r--   0        0        0      348 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/nodes.py
--rw-r--r--   0        0        0     2037 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/partitioning.py
--rw-r--r--   0        0        0     8738 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/pytreelib.py
--rw-r--r--   0        0        0     2313 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/reprlib.py
--rw-r--r--   0        0        0    13718 2023-07-08 19:31:09.240551 nnx-0.0.7/nnx/spmd.py
--rw-r--r--   0        0        0     5103 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/state.py
--rw-r--r--   0        0        0     2412 2023-07-05 17:41:51.533316 nnx-0.0.7/nnx/tracers.py
--rw-r--r--   0        0        0    22437 2023-07-10 14:57:54.632800 nnx-0.0.7/nnx/transforms.py
--rw-r--r--   0        0        0      764 2023-07-10 15:09:18.980819 nnx-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    22353 1970-01-01 00:00:00.000000 nnx-0.0.7/setup.py
--rw-r--r--   0        0        0    21733 1970-01-01 00:00:00.000000 nnx-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-12 16:43:43.251031 nnx-0.0.8/LICENSE
+-rw-r--r--   0        0        0    21250 2023-07-12 16:43:43.251031 nnx-0.0.8/README.md
+-rw-r--r--   0        0        0     1410 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/__init__.py
+-rw-r--r--   0        0        0     5241 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/containers.py
+-rw-r--r--   0        0        0     5417 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/contextlib.py
+-rw-r--r--   0        0        0     4512 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/dataclasses.py
+-rw-r--r--   0        0        0       45 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/errors.py
+-rw-r--r--   0        0        0     4345 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/helpers.py
+-rw-r--r--   0        0        0     1832 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/ids.py
+-rw-r--r--   0        0        0    26625 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/module.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/nn/__init__.py
+-rw-r--r--   0        0        0      763 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/nn/activations.py
+-rw-r--r--   0        0        0     2763 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/nn/dtypes.py
+-rw-r--r--   0        0        0     2147 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/nn/initializers.py
+-rw-r--r--   0        0        0    16022 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/nn/linear.py
+-rw-r--r--   0        0        0    13511 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/nn/normalization.py
+-rw-r--r--   0        0        0     2281 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/nn/stochastic.py
+-rw-r--r--   0        0        0      348 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/nodes.py
+-rw-r--r--   0        0        0     2037 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/partitioning.py
+-rw-r--r--   0        0        0     8738 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/pytreelib.py
+-rw-r--r--   0        0        0     2313 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/reprlib.py
+-rw-r--r--   0        0        0    13718 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/spmd.py
+-rw-r--r--   0        0        0     5103 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/state.py
+-rw-r--r--   0        0        0     2412 2023-07-12 16:43:43.255031 nnx-0.0.8/nnx/tracers.py
+-rw-r--r--   0        0        0    26223 2023-07-12 16:43:43.259031 nnx-0.0.8/nnx/transforms.py
+-rw-r--r--   0        0        0      764 2023-07-12 16:43:43.259031 nnx-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    21733 1970-01-01 00:00:00.000000 nnx-0.0.8/PKG-INFO
```

### Comparing `nnx-0.0.7/LICENSE` & `nnx-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/README.md` & `nnx-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/__init__.py` & `nnx-0.0.8/nnx/__init__.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/containers.py` & `nnx-0.0.8/nnx/containers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/contextlib.py` & `nnx-0.0.8/nnx/contextlib.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/dataclasses.py` & `nnx-0.0.8/nnx/dataclasses.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/helpers.py` & `nnx-0.0.8/nnx/helpers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/ids.py` & `nnx-0.0.8/nnx/ids.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/module.py` & `nnx-0.0.8/nnx/module.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/nn/activations.py` & `nnx-0.0.8/nnx/nn/activations.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/nn/dtypes.py` & `nnx-0.0.8/nnx/nn/dtypes.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/nn/initializers.py` & `nnx-0.0.8/nnx/nn/initializers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/nn/linear.py` & `nnx-0.0.8/nnx/nn/linear.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/nn/normalization.py` & `nnx-0.0.8/nnx/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/nn/stochastic.py` & `nnx-0.0.8/nnx/nn/stochastic.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/partitioning.py` & `nnx-0.0.8/nnx/partitioning.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/pytreelib.py` & `nnx-0.0.8/nnx/pytreelib.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/reprlib.py` & `nnx-0.0.8/nnx/reprlib.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/spmd.py` & `nnx-0.0.8/nnx/spmd.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/state.py` & `nnx-0.0.8/nnx/state.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/tracers.py` & `nnx-0.0.8/nnx/tracers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.7/nnx/transforms.py` & `nnx-0.0.8/nnx/transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+import dataclasses
 import functools
 import typing as tp
 from types import MappingProxyType
+from typing import Any
 
 import jax
 import jax.numpy as jnp
 import jax.stages
 import jax.tree_util as jtu
 
 from nnx import containers, contextlib, partitioning, spmd, tracers
-from nnx.module import CallableProxy, DelayedAccessor, Module, ModuleDef, PureModule
+from nnx.module import (
+    CallableProxy,
+    DelayedAccessor,
+    Module,
+    ModuleDef,
+    ModuleMeta,
+    PureModule,
+)
 from nnx.state import State
 
 A = tp.TypeVar("A")
 C = tp.TypeVar("C")
+B = tp.TypeVar("B")
 F = tp.TypeVar("F", bound=tp.Callable[..., tp.Any])
 G = tp.TypeVar("G", bound=tp.Callable[..., tp.Any])
 M = tp.TypeVar("M", bound=Module)
 
 AxisName = tp.Hashable
 Leaf = tp.Any
 Leaves = tp.List[Leaf]
@@ -239,130 +249,105 @@
         reduce_axes=reduce_axes,
     )
     ref_grad = functools.wraps(fun)(ref_grad)
     # _update_decorator_fields(ref_grad, fun)
     return ref_grad
 
 
-# NOTE: I don't understand why variable_broadcasts exists. Passing them as
-# captures to `scan_fn` makes it impossible to propagate state updates from
-# them. Maybe, there should only be `variable_carry` and `variable_axes`.
-class Scan(Module, tp.Generic[M]):
-    def __init__(
+@dataclasses.dataclass
+class ScanOptions:
+    variable_axes: tp.Mapping[partitioning.Filter, int]
+    variable_broadcast: partitioning.Filter
+    variable_carry: partitioning.Filter
+    split_rngs: contextlib.RngFilter
+    in_axes: tp.Any
+    out_axes: tp.Any
+    length: tp.Optional[int]
+    reverse: bool
+    unroll: int
+    data_transform: tp.Optional[tp.Callable[..., tp.Any]]
+    metadata_params: tp.Mapping[tp.Any, tp.Any]
+
+
+class ScanMeta(ModuleMeta):
+    def __call__(
         self,
+        module_constructor: tp.Callable[..., M],
         *,
+        variable_axes: tp.Mapping[partitioning.Filter, int] = MappingProxyType({}),
+        variable_broadcast: partitioning.Filter = None,
+        variable_carry: partitioning.Filter = ...,
+        split_rngs: contextlib.RngFilter = None,
+        in_axes: tp.Any = 0,
+        out_axes: tp.Any = 0,
+        length: tp.Optional[int] = None,
+        reverse: bool = False,
+        unroll: int = 1,
+        data_transform: tp.Optional[tp.Callable[..., tp.Any]] = None,
+        metadata_params: tp.Mapping[tp.Any, tp.Any] = {},
+    ) -> tp.Callable[..., "Scan[M]"]:
+        super_call = super().__call__
+
+        def _create_scan(*args, **kwargs) -> Scan[M]:
+            return super_call(
+                module_constructor=module_constructor,
+                module_init_args=args,
+                module_init_kwargs=kwargs,
+                variable_axes=variable_axes,
+                variable_broadcast=variable_broadcast,
+                variable_carry=variable_carry,
+                split_rngs=split_rngs,
+                in_axes=in_axes,
+                out_axes=out_axes,
+                length=length,
+                reverse=reverse,
+                unroll=unroll,
+                data_transform=data_transform,
+                metadata_params=metadata_params,
+            )
+
+        return _create_scan
+
+
+class Scan(Module, tp.Generic[M], metaclass=ScanMeta):
+    def __init__(
+        self,
         module_constructor: tp.Callable[..., M],
+        *,
+        variable_axes: tp.Mapping[partitioning.Filter, int] = MappingProxyType({}),
+        variable_broadcast: partitioning.Filter = None,
+        variable_carry: partitioning.Filter = ...,
+        split_rngs: contextlib.RngFilter = None,
+        in_axes: tp.Any = 0,
+        out_axes: tp.Any = 0,
+        length: tp.Optional[int] = None,
+        reverse: bool = False,
+        unroll: int = 1,
+        data_transform: tp.Optional[tp.Callable[..., tp.Any]] = None,
+        metadata_params: tp.Mapping[tp.Any, tp.Any] = MappingProxyType({}),
         module_init_args: tp.Tuple[tp.Any, ...],
         module_init_kwargs: tp.Dict[str, tp.Any],
-        variable_axes: tp.Mapping[partitioning.Filter, int],
-        variable_broadcast: partitioning.Filter,
-        variable_carry: partitioning.Filter,
-        split_rngs: contextlib.RngFilter,
-        in_axes: tp.Any,
-        out_axes: tp.Any,
-        length: tp.Optional[int],
-        reverse: bool,
-        unroll: int,
-        data_transform: tp.Optional[tp.Callable[..., tp.Any]],
-        metadata_params: tp.Mapping[tp.Any, tp.Any],
     ):
         self.module_constructor = module_constructor
-        self.variable_axes = variable_axes
-        self.variable_broadcast = variable_broadcast
-        self.variable_carry = variable_carry
-        self.split_rngs = split_rngs
-        self.in_axes = in_axes
-        self.out_axes = out_axes
-        self.length = length
-        self.reverse = reverse
-        self.unroll = unroll
-        self.data_transform = data_transform
-        self.metadata_params = metadata_params
-        self.scan_module = self.create_module(*module_init_args, **module_init_kwargs)
-
-    def create_module(
-        self: "Scan[M]", *args, ctx: tp.Optional[contextlib.Context] = None, **kwargs
-    ) -> M:
-        if self.variable_axes and self.length is None:
-            raise ValueError("Cannot use variable_axes without specifying a length")
-
-        key_values = []
-
-        if ctx is not None:
-            if not isinstance(ctx, contextlib.Context):
-                raise TypeError(f"Expected a Context, got {type(ctx).__name__}")
-
-            keys, ctxdef = ctx.partition()
-            split_predicate = contextlib.to_rng_predicate(self.split_rngs)
-
-            key_axes = []
-            key_names = tuple(keys.keys())
-
-            for name, key in keys.items():
-                if split_predicate(name):
-                    if self.length is None:
-                        raise ValueError(
-                            "Cannot split RNGs without specifying a length"
-                        )
-                    key = jax.random.split(key, self.length)
-                    key_axes.append(0)
-                else:
-                    key_axes.append(None)
-                key_values.append(key)
-        else:
-            key_names = None
-            ctxdef = None
-            key_axes = None
-
-        init_out_axes = (*self.variable_axes.values(), None, None)
-        moduledef: tp.Optional[ModuleDef[M]] = None
-
-        def _init_state(*key_values):
-            nonlocal moduledef
-
-            if ctxdef is not None:
-                assert key_names is not None
-                keys = dict(zip(key_names, key_values))
-                ctx = ctxdef.merge(keys)
-                kwargs["ctx"] = ctx
-
-            module = self.module_constructor(*args, **kwargs)
-
-            # lift module
-            filters = (
-                *self.variable_axes.keys(),
-                self.variable_broadcast,
-                self.variable_carry,
-            )
-
-            states, moduledef = module.partition(*filters)
-
-            return states
-
-        if ctxdef is not None or self.variable_axes:
-            _init_state = jax.vmap(
-                _init_state,
-                in_axes=key_axes,
-                out_axes=init_out_axes,
-                axis_size=self.length,
-            )
-
-        *axes_states, broadcast_state, carry_state = _init_state(*key_values)
-        moduledef = tp.cast(ModuleDef[M], moduledef)
-
-        # add additional axis name to Variable.sharding
-        if spmd.PARTITION_NAME in self.metadata_params:
-            axes_states = [
-                spmd.add_axis(state, index, self.metadata_params)
-                for state, index in zip(axes_states, self.variable_axes.values())
-            ]
-
-        module = moduledef.merge(*axes_states, broadcast_state, carry_state)
-
-        return module
+        self.options = ScanOptions(
+            variable_axes=variable_axes,
+            variable_broadcast=variable_broadcast,
+            variable_carry=variable_carry,
+            split_rngs=split_rngs,
+            in_axes=in_axes,
+            out_axes=out_axes,
+            length=length,
+            reverse=reverse,
+            unroll=unroll,
+            data_transform=data_transform,
+            metadata_params=metadata_params,
+        )
+        self.scan_module = scan_init(
+            self.options, module_constructor, module_init_args, module_init_kwargs
+        )
 
     def __call__(
         self,
         carry_arg: C,
         axes_arg,
         *broadcast_args,
         ctx: tp.Optional[contextlib.Context] = None,
@@ -377,236 +362,409 @@
         accessesor = DelayedAccessor()
 
         def _context(
             accessesor,
             carry_arg: C,
             axes_arg,
             *broadcast_args,
-            ctx: tp.Optional[contextlib.Context] = None,
             **broadcast_kwargs,
         ) -> tp.Tuple[C, tp.Any]:
-            # split module state
-            filters = (
-                *self.variable_axes.keys(),
-                self.variable_broadcast,
-                self.variable_carry,
-            )
-            (
-                *axes_states,
-                broadcast_state,
-                carry_state,
-            ), moduledef = self.scan_module.partition(*filters)
-
-            # transpose axes state
-            axes_states = tuple(
-                jax.tree_map(lambda x: jnp.moveaxis(x, axis, 0), axes_state)
-                for axes_state, axis in zip(axes_states, self.variable_axes.values())
-            )
-            # transpose axes arg
-            axes_arg = tree_map_upto_left(
-                lambda axis, node: jax.tree_map(
-                    lambda x: jnp.moveaxis(x, axis, 0), node
-                ),
-                self.in_axes,
+            def _apply(module, *args, **kwargs):
+                return accessesor(module)(*args, **kwargs)
+
+            return scan_apply(
+                self.options,
+                _apply,
+                self.scan_module,
+                carry_arg,
                 axes_arg,
+                broadcast_args,
+                broadcast_kwargs,
             )
 
-            # infer length
-            lengths: tp.Set[int] = set(
-                x.shape[0] for x in jax.tree_util.tree_leaves((axes_states, axes_arg))
-            )
+        return CallableProxy(_context, accessesor)  # type: ignore
 
-            if len(lengths) > 1:
-                raise ValueError(
-                    f"Inconsistent lengths between variable_axes states and "
-                    f"axes_arg: {lengths}"
-                )
-            elif len(lengths) == 0:
-                if self.length is None:
-                    raise ValueError(
-                        "Cannot infer length from variable_axes states or axes_arg, "
-                        "please specify `length`"
-                    )
-                length = self.length
-            else:
-                length = lengths.pop()
-                if self.length is not None and self.length != length:
-                    raise ValueError(
-                        f"Specified length {self.length} is the same as the inferred "
-                        f"length {length}"
-                    )
-
-            # split rng state
-            axes_keys: tp.Optional[tp.Dict[str, jax.Array]]
-            broadcast_keys: tp.Optional[tp.Dict[str, jax.Array]]
-
-            if ctx is not None:
-                if not isinstance(ctx, contextlib.Context):
-                    raise TypeError(f"Expected a Context, got {type(ctx).__name__}")
-
-                axes_keys = {}
-                broadcast_keys = {}
-
-                keys, ctxdef = ctx.partition()
-                split_predicate = contextlib.to_rng_predicate(self.split_rngs)
-
-                for name, key in keys.items():
-                    if split_predicate(name):
-                        axes_keys[name] = jax.random.split(key, length)
-                    else:
-                        broadcast_keys[name] = key
+
+class ScanCall(tp.Protocol, tp.Generic[C, A, B]):
+    def __call__(
+        self,
+        module: Module,
+        carry_arg: C,
+        axes_arg: A,
+        *broadcast_args: tp.Any,
+        **broadcast_kwargs: tp.Any,
+    ) -> tp.Tuple[C, B]:
+        ...
+
+
+def scan_init(
+    options: ScanOptions,
+    module_constructor: tp.Callable[..., M],
+    module_init_args: tp.Tuple[tp.Any, ...],
+    module_init_kwargs: tp.Dict[str, tp.Any],
+) -> M:
+    if options.variable_axes and options.length is None:
+        raise ValueError("Cannot use variable_axes without specifying a length")
+
+    ctx = module_init_kwargs.pop("ctx", None)
+
+    if ctx is not None and not isinstance(ctx, contextlib.Context):
+        raise TypeError(f"Expected a Context, got {type(ctx).__name__}")
+
+    key_values = []
+
+    if ctx is not None:
+        if not isinstance(ctx, contextlib.Context):
+            raise TypeError(f"Expected a Context, got {type(ctx).__name__}")
+
+        keys, ctxdef = ctx.partition()
+        split_predicate = contextlib.to_rng_predicate(options.split_rngs)
+
+        key_axes = []
+        key_names = tuple(keys.keys())
+
+        for name, key in keys.items():
+            if split_predicate(name):
+                if options.length is None:
+                    raise ValueError("Cannot split RNGs without specifying a length")
+                key = jax.random.split(key, options.length)
+                key_axes.append(0)
             else:
-                ctxdef = None
-                axes_keys = None
-                broadcast_keys = None
-
-            carry = (carry_state, carry_arg)
-            axes = (axes_keys, axes_states, axes_arg)
-
-            def scan_fn(
-                carry: tp.Tuple[State, tp.Any],
-                axes: tp.Tuple[
-                    tp.Optional[tp.Dict[str, jax.Array]], tp.Tuple[State, ...], tp.Any
-                ],
-            ):
-                carry_state, carry_arg = carry
-                axes_keys, axes_states, axes_arg = axes
-
-                # merge rng state
-                if ctxdef is not None:
-                    assert axes_keys is not None and broadcast_keys is not None
-                    ctx = ctxdef.merge({**axes_keys, **broadcast_keys})
-                    broadcast_kwargs["ctx"] = ctx
-
-                # remove metadata axis name from Variable.sharding
-                if spmd.PARTITION_NAME in self.metadata_params:
-                    axes_states = [
-                        spmd.remove_axis(state, index, self.metadata_params)
-                        for state, index in zip(
-                            axes_states, self.variable_axes.values()
-                        )
-                    ]
-
-                # merge module state
-                module = moduledef.merge(*axes_states, broadcast_state, carry_state)
-
-                fn = accessesor(module)
-                (carry_out, axes_out) = fn(
-                    carry_arg, axes_arg, *broadcast_args, **broadcast_kwargs
-                )
-
-                # split module state
-                (*axes_states, _broadcast_state, carry_state), _ = module.partition(
-                    *filters
-                )
-
-                # add metadata axis name to Variable.sharding
-                if spmd.PARTITION_NAME in self.metadata_params:
-                    axes_states = [
-                        spmd.add_axis(state, index, self.metadata_params)
-                        for state, index in zip(
-                            axes_states, self.variable_axes.values()
-                        )
-                    ]
-
-                carry = (carry_state, carry_out)
-                out = (axes_states, axes_out)
-
-                return carry, out
-
-            carry, scan_out = jax.lax.scan(
-                scan_fn,
-                carry,
-                axes,
-                length=length,
-                reverse=self.reverse,
-                unroll=self.unroll,
-            )
-            carry_state, carry_out = carry
-            axes_states, out = scan_out
+                key_axes.append(None)
+            key_values.append(key)
+    else:
+        key_names = None
+        ctxdef = None
+        key_axes = None
+
+    init_out_axes = (*options.variable_axes.values(), None, None)
+    moduledef: tp.Optional[ModuleDef[M]] = None
+
+    def _init_state(*key_values):
+        nonlocal moduledef
+
+        if ctxdef is not None:
+            assert key_names is not None
+            keys = dict(zip(key_names, key_values))
+            ctx = ctxdef.merge(keys)
+            module_init_kwargs["ctx"] = ctx
+
+        module = module_constructor(*module_init_args, **module_init_kwargs)
+
+        # lift module
+        filters = (
+            *options.variable_axes.keys(),
+            options.variable_broadcast,
+            options.variable_carry,
+        )
+
+        states, moduledef = module.partition(*filters)
+
+        return states
+
+    if ctxdef is not None or options.variable_axes:
+        _init_state = jax.vmap(
+            _init_state,
+            in_axes=key_axes,
+            out_axes=init_out_axes,
+            axis_size=options.length,
+        )
+
+    *axes_states, broadcast_state, carry_state = _init_state(*key_values)
+    moduledef = tp.cast(ModuleDef[M], moduledef)
 
-            # transpose axes state
-            axes_states = tuple(
-                jax.tree_map(lambda x: jnp.moveaxis(x, 0, axis), axes_state)
-                for axes_state, axis in zip(axes_states, self.variable_axes.values())
+    # add additional axis name to Variable.sharding
+    if spmd.PARTITION_NAME in options.metadata_params:
+        axes_states = [
+            spmd.add_axis(state, index, options.metadata_params)
+            for state, index in zip(axes_states, options.variable_axes.values())
+        ]
+
+    module = moduledef.merge(*axes_states, broadcast_state, carry_state)
+
+    return module
+
+
+def scan_apply(
+    options: ScanOptions,
+    f: ScanCall[C, A, B],
+    module: Module,
+    carry_arg: C,
+    axes_arg: A,
+    broadcast_args: tuple[tp.Any, ...],
+    broadcast_kwargs: dict[str, tp.Any],
+) -> tp.Tuple[C, B]:
+    # split module state
+    filters = (
+        *options.variable_axes.keys(),
+        options.variable_broadcast,
+        options.variable_carry,
+    )
+    (
+        *axes_states,
+        broadcast_state,
+        carry_state,
+    ), moduledef = module.partition(*filters)
+
+    # transpose axes state
+    axes_states = tuple(
+        jax.tree_map(lambda x: jnp.moveaxis(x, axis, 0), axes_state)
+        for axes_state, axis in zip(axes_states, options.variable_axes.values())
+    )
+    # transpose axes arg
+    axes_arg = tree_map_upto_left(
+        lambda axis, node: jax.tree_map(lambda x: jnp.moveaxis(x, axis, 0), node),
+        options.in_axes,
+        axes_arg,
+    )
+
+    # infer length
+    lengths: tp.Set[int] = set(
+        x.shape[0] for x in jax.tree_util.tree_leaves((axes_states, axes_arg))
+    )
+
+    if len(lengths) > 1:
+        raise ValueError(
+            f"Inconsistent lengths between variable_axes states and "
+            f"axes_arg: {lengths}"
+        )
+    elif len(lengths) == 0:
+        if options.length is None:
+            raise ValueError(
+                "Cannot infer length from variable_axes states or axes_arg, "
+                "please specify `length`"
             )
-            # transpose axes arg
-            out = tree_map_upto_left(
-                lambda axis, node: jax.tree_map(
-                    lambda x: jnp.moveaxis(x, 0, axis), node
-                ),
-                self.out_axes,
-                out,
+        length = options.length
+    else:
+        length = lengths.pop()
+        if options.length is not None and options.length != length:
+            raise ValueError(
+                f"Specified length {options.length} is the same as the inferred "
+                f"length {length}"
             )
 
-            self.scan_module.update_state((*axes_states, carry_state))
+    # split rng state
+    axes_keys: tp.Optional[tp.Dict[str, jax.Array]]
+    broadcast_keys: tp.Optional[tp.Dict[str, jax.Array]]
+
+    ctx = broadcast_kwargs.pop("ctx", None)
+    if ctx is not None:
+        if not isinstance(ctx, contextlib.Context):
+            raise TypeError(f"Expected a Context, got {type(ctx).__name__}")
+
+        axes_keys = {}
+        broadcast_keys = {}
+
+        keys, ctxdef = ctx.partition()
+        split_predicate = contextlib.to_rng_predicate(options.split_rngs)
+
+        for name, key in keys.items():
+            if split_predicate(name):
+                axes_keys[name] = jax.random.split(key, length)
+            else:
+                broadcast_keys[name] = key
+    else:
+        ctxdef = None
+        axes_keys = None
+        broadcast_keys = None
+
+    carry = (carry_state, carry_arg)
+    axes = (axes_keys, axes_states, axes_arg)
+
+    def scan_fn(
+        carry: tp.Tuple[State, tp.Any],
+        axes: tp.Tuple[
+            tp.Optional[tp.Dict[str, jax.Array]], tp.Tuple[State, ...], tp.Any
+        ],
+    ):
+        carry_state, carry_arg = carry
+        axes_keys, axes_states, axes_arg = axes
+
+        # merge rng state
+        if ctxdef is not None:
+            assert axes_keys is not None and broadcast_keys is not None
+            ctx = ctxdef.merge({**axes_keys, **broadcast_keys})
+            broadcast_kwargs["ctx"] = ctx
+
+        # remove metadata axis name from Variable.sharding
+        if spmd.PARTITION_NAME in options.metadata_params:
+            axes_states = [
+                spmd.remove_axis(state, index, options.metadata_params)
+                for state, index in zip(axes_states, options.variable_axes.values())
+            ]
+
+        # merge module state
+        module = moduledef.merge(*axes_states, broadcast_state, carry_state)
 
-            return carry_out, out
+        (carry_out, axes_out) = f(
+            module, carry_arg, axes_arg, *broadcast_args, **broadcast_kwargs
+        )
 
-        return CallableProxy(_context, accessesor)  # type: ignore
+        # split module state
+        (*axes_states, _broadcast_state, carry_state), _ = module.partition(*filters)
+
+        # add metadata axis name to Variable.sharding
+        if spmd.PARTITION_NAME in options.metadata_params:
+            axes_states = [
+                spmd.add_axis(state, index, options.metadata_params)
+                for state, index in zip(axes_states, options.variable_axes.values())
+            ]
+
+        carry = (carry_state, carry_out)
+        out = (axes_states, axes_out)
+
+        return carry, out
+
+    carry, scan_out = jax.lax.scan(
+        scan_fn,
+        carry,
+        axes,
+        length=length,
+        reverse=options.reverse,
+        unroll=options.unroll,
+    )
+    carry_state, carry_out = carry
+    axes_states, out = scan_out
+
+    # transpose axes state
+    axes_states = tuple(
+        jax.tree_map(lambda x: jnp.moveaxis(x, 0, axis), axes_state)
+        for axes_state, axis in zip(axes_states, options.variable_axes.values())
+    )
+    # transpose axes arg
+    out = tree_map_upto_left(
+        lambda axis, node: jax.tree_map(lambda x: jnp.moveaxis(x, 0, axis), node),
+        options.out_axes,
+        out,
+    )
+
+    module.update_state((*axes_states, carry_state))
+
+    return carry_out, out
 
 
 def scan(
-    module_constructor: tp.Callable[..., M],
+    f: F,
+    *,
     variable_axes: tp.Mapping[partitioning.Filter, int] = MappingProxyType({}),
     variable_broadcast: partitioning.Filter = None,
     variable_carry: partitioning.Filter = ...,
     split_rngs: contextlib.RngFilter = None,
     in_axes: tp.Any = 0,
     out_axes: tp.Any = 0,
     length: tp.Optional[int] = None,
     reverse: bool = False,
     unroll: int = 1,
     data_transform: tp.Optional[tp.Callable[..., tp.Any]] = None,
     metadata_params: tp.Mapping[tp.Any, tp.Any] = {},
-) -> tp.Callable[..., Scan[M]]:
-    def _create_scan(*args, **kwargs) -> Scan[M]:
-        return Scan(
-            module_constructor=module_constructor,
-            module_init_args=args,
-            module_init_kwargs=kwargs,
-            variable_axes=variable_axes,
-            variable_broadcast=variable_broadcast,
-            variable_carry=variable_carry,
-            split_rngs=split_rngs,
-            in_axes=in_axes,
-            out_axes=out_axes,
-            length=length,
-            reverse=reverse,
-            unroll=unroll,
-            data_transform=data_transform,
-            metadata_params=metadata_params,
-        )
+    is_init: tp.Optional[bool] = None,
+) -> F:
+    if is_init is None:
+        is_init = f.__name__ == "__init__"
+
+    options = ScanOptions(
+        variable_axes=variable_axes,
+        variable_broadcast=variable_broadcast,
+        variable_carry=variable_carry,
+        split_rngs=split_rngs,
+        in_axes=in_axes,
+        out_axes=out_axes,
+        length=length,
+        reverse=reverse,
+        unroll=unroll,
+        data_transform=data_transform,
+        metadata_params=metadata_params,
+    )
+
+    if is_init:
+
+        @functools.wraps(f)
+        def init_wrapper(module: Module, *args, **kwargs):
+            def module_constructor(*args, **kwargs):
+                f(module, *args, **kwargs)
+                return module
+
+            lifted_module = scan_init(options, module_constructor, args, kwargs)
+            module.update_state(lifted_module)
+
+        wrapper = init_wrapper
+
+    else:
+
+        @functools.wraps(f)
+        def apply_wrapper(
+            module: Module, carry_arg: C, axes_arg, *args, **kwargs
+        ) -> tuple[C, tp.Any]:
+            return scan_apply(options, f, module, carry_arg, axes_arg, args, kwargs)
+
+        wrapper = apply_wrapper
+
+    return wrapper  # type: ignore
+
+
+class RematMeta(ModuleMeta):
+    def __call__(
+        self,
+        module_constructor: tp.Callable[..., M],
+        # variables: lift.CollectionFilter = True,
+        # rngs: lift.PRNGSequenceFilter = True,
+        prevent_cse: bool = True,
+        static_argnums: tp.Union[int, tuple[int, ...]] = (),
+        policy: tp.Optional[tp.Callable[..., bool]] = None,
+    ) -> tp.Callable[..., "Remat[M]"]:
+        super_call = super().__call__
+
+        def create_remat(*args, **kwargs) -> Remat[M]:
+            return super_call(
+                module_constructor=module_constructor,
+                module_init_args=args,
+                module_init_kwargs=kwargs,
+                prevent_cse=prevent_cse,
+                static_argnums=static_argnums,
+                policy=policy,
+            )
+
+        return create_remat
+
 
-    return _create_scan
+@dataclasses.dataclass
+class RematOptions:
+    # variables: lift.CollectionFilter,
+    # rngs: lift.PRNGSequenceFilter,
+    prevent_cse: bool
+    static_argnums: tp.Union[int, tuple[int, ...]]
+    policy: tp.Optional[tp.Callable[..., bool]]
+
+    def __post_init__(self):
+        if isinstance(self.static_argnums, int):
+            self.static_argnums = (self.static_argnums,)
+
+        # add 2 as an offset to account for state and keys
+        self.static_argnums = tuple(x + 2 if x >= 0 else x for x in self.static_argnums)
 
 
-class Remat(Module, tp.Generic[M]):
+class Remat(Module, tp.Generic[M], metaclass=RematMeta):
     def __init__(
         self,
         *,
         module_constructor: tp.Callable[..., M],
-        module_init_args: tp.Tuple[tp.Any, ...],
-        module_init_kwargs: tp.Dict[str, tp.Any],
         # variables: lift.CollectionFilter,
         # rngs: lift.PRNGSequenceFilter,
-        prevent_cse: bool,
-        static_argnums: tp.Union[int, tuple[int, ...]],
-        policy: tp.Optional[tp.Callable[..., bool]],
+        prevent_cse: bool = True,
+        static_argnums: tp.Union[int, tuple[int, ...]] = (),
+        policy: tp.Optional[tp.Callable[..., bool]] = None,
+        module_init_args: tp.Tuple[tp.Any, ...],
+        module_init_kwargs: tp.Dict[str, tp.Any],
     ):
-        if isinstance(static_argnums, int):
-            static_argnums = (static_argnums,)
-
-        # add 2 as an offset to account for state and keys
-        static_argnums = tuple(x + 2 if x >= 0 else x for x in static_argnums)
-
+        self.options = RematOptions(
+            prevent_cse=prevent_cse,
+            static_argnums=static_argnums,
+            policy=policy,
+        )
         self.module_constructor = module_constructor
-        self.prevent_cse = prevent_cse
-        self.static_argnums = static_argnums
-        self.policy = policy
         self.remat_module = self.module_constructor(
             *module_init_args, **module_init_kwargs
         )
 
     def __call__(
         self,
         *args,
@@ -617,73 +775,107 @@
     @property
     def call(self) -> M:
         accessesor = DelayedAccessor()
 
         def _call(
             accessesor, *args, ctx: tp.Optional[contextlib.Context] = None
         ) -> tp.Tuple[tp.Any]:
-            state, moduledef = self.remat_module.partition()
+            def _apply(module, *args, **kwargs):
+                return accessesor(module)(*args, **kwargs)
 
-            if ctx is not None:
-                keys, ctxdef = ctx.partition()
-            else:
-                keys = None
-                ctxdef = None
+            return remat_apply(
+                self.options,
+                _apply,
+                self.remat_module,
+                args,
+                ctx,
+            )
 
-            def _remat_fn(
-                state: State,
-                keys: tp.Optional[tp.Dict[str, jax.Array]],
-                *args,
-            ) -> tp.Tuple[State, tp.Any]:
-                kwargs = {}
-                if keys is not None:
-                    assert ctxdef is not None
-                    kwargs["ctx"] = ctxdef.merge(keys)
-
-                module = moduledef.merge(state)
-                fn = accessesor(module)
-                out = fn(*args, **kwargs)
-
-                state, _ = module.partition()
-
-                return state, out
-
-            state, out = jax.checkpoint(
-                _remat_fn,
-                prevent_cse=self.prevent_cse,
-                static_argnums=self.static_argnums,
-                policy=self.policy,
-            )(state, keys, *args)
+        return CallableProxy(_call, accessesor)  # type: ignore
 
-            self.remat_module.update_state(state)
 
-            return out
+class RematCall(tp.Protocol):
+    def __call__(self, *args, ctx: tp.Optional[contextlib.Context]) -> tp.Any:
+        ...
+
+
+def remat_apply(
+    options: RematOptions,
+    f: RematCall,
+    module: Module,
+    args: tp.Tuple[tp.Any, ...],
+    ctx: tp.Optional[contextlib.Context],
+):
+    state, moduledef = module.partition()
 
-        return CallableProxy(_call, accessesor)  # type: ignore
+    if ctx is not None:
+        keys, ctxdef = ctx.partition()
+    else:
+        keys = None
+        ctxdef = None
+
+    def _remat_fn(
+        state: State,
+        keys: tp.Optional[tp.Dict[str, jax.Array]],
+        *args,
+    ) -> tp.Tuple[State, tp.Any]:
+        kwargs = {}
+        if keys is not None:
+            assert ctxdef is not None
+            kwargs["ctx"] = ctxdef.merge(keys)
+
+        module = moduledef.merge(state)
+        out = f(module, *args, **kwargs)
+
+        state, _ = module.partition()
+
+        return state, out
+
+    state, out = jax.checkpoint(
+        _remat_fn,
+        prevent_cse=options.prevent_cse,
+        static_argnums=options.static_argnums,
+        policy=options.policy,
+    )(state, keys, *args)
+
+    module.update_state(state)
+
+    return out
 
 
 def remat(
-    module_constructor: tp.Callable[..., M],
-    # variables: lift.CollectionFilter = True,
-    # rngs: lift.PRNGSequenceFilter = True,
+    f: F,
+    *,
+    # variables: lift.CollectionFilter,
+    # rngs: lift.PRNGSequenceFilter,
     prevent_cse: bool = True,
     static_argnums: tp.Union[int, tuple[int, ...]] = (),
     policy: tp.Optional[tp.Callable[..., bool]] = None,
-) -> tp.Callable[..., Remat[M]]:
-    def create_remat(*args, **kwargs) -> Remat[M]:
-        return Remat(
-            module_constructor=module_constructor,
-            module_init_args=args,
-            module_init_kwargs=kwargs,
-            prevent_cse=prevent_cse,
-            static_argnums=static_argnums,
-            policy=policy,
-        )
+    is_init: tp.Optional[bool] = None,
+) -> F:
+    if is_init is None:
+        is_init = f.__name__ == "__init__"
+
+    options = RematOptions(
+        # variables=variables,
+        # rngs=rngs,
+        prevent_cse=prevent_cse,
+        static_argnums=static_argnums,
+        policy=policy,
+    )
+
+    if is_init:
+        return f
+    else:
+
+        @functools.wraps(f)
+        def wrapper(module: Module, *args, ctx: tp.Optional[contextlib.Context] = None):
+            return remat_apply(options, f, module, args, ctx)
 
-    return create_remat
+        return wrapper  # type: ignore
 
 
 def tree_map_upto_left(
     f: tp.Callable[[tp.Any, tp.Any], tp.Any], left: tp.Any, right: tp.Any
 ) -> tp.Any:
     leaves_left, treedef = jtu.tree_flatten(left)
     leaves_right = treedef.flatten_up_to(right)
```

### Comparing `nnx-0.0.7/pyproject.toml` & `nnx-0.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nnx"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["Cristian Garcia <cgarcia.e88@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 jax = "*"
```

### Comparing `nnx-0.0.7/setup.py` & `nnx-0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,469 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nnx
+Version: 0.0.8
+Summary: 
+Author: Cristian Garcia
+Author-email: cgarcia.e88@gmail.com
+Requires-Python: >=3.9,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: jax
+Requires-Dist: jaxlib
+Requires-Dist: optax
+Requires-Dist: typing-extensions
+Description-Content-Type: text/markdown
 
-packages = \
-['nnx', 'nnx.nn']
+[![codecov](https://codecov.io/gh/cgarciae/nnx/branch/main/graph/badge.svg?token=VqJjL474Z7)](https://codecov.io/gh/cgarciae/nnx)
 
-package_data = \
-{'': ['*']}
+# NNX
 
-install_requires = \
-['jax', 'jaxlib', 'optax', 'typing-extensions']
-
-setup_kwargs = {
-    'name': 'nnx',
-    'version': '0.0.7',
-    'description': '',
-    'long_description': '[![codecov](https://codecov.io/gh/cgarciae/nnx/branch/main/graph/badge.svg?token=VqJjL474Z7)](https://codecov.io/gh/cgarciae/nnx)\n\n# NNX\n\n_**N**eural **N**etworks for JA**X**_\n\nNNX is a Neural Networks library for JAX that provides a simple yet powerful module system that adheres to standard Python semantics. Its aim is to combine the robustness of [Flax](https://flax.readthedocs.io/en/latest/) with a simplified, Pythonic API akin to that of [PyTorch](https://pytorch.org/).\n\n* **Pythonic**: Modules are just regular python classes, they contain their own state, are fully mutable, and allow sharing references between Modules.\n* **Compatible**: Easily convert back and forth between Modules and pytrees using the Functional API to integrate with any JAX API.\n* **Safe**: NNX incorporates mechanisms to try to prevent tracer leakage, avoid stale RNGs, and ensure proper state propagation in order to help produce correct JAX programs.\n* **Semantic**: Partition a Module\'s state into different semantic collections, allowing for fine-grained control when applying JAX transformations.\n\n#### Table of Contents\n* [Installation](#installation)\n* [Getting Started](#getting-started)\n* [FAQs](#faqs)\n* [Examples](#examples)\n* [User Guide](#user-guide)\n\n## Installation\n\nTo get started with `nnx`, install the package via pip:\n\n```\npip install nnx\n```\nFor the most recent version, install directly from our GitHub repository:\n\n```\npip install git+https://github.com/cgarciae/nnx\n```\n\n## Getting Started\n\nThe following example guides you through creating a basic `Linear` model with NNX and executing a forward pass. It also demonstrate how handle mutable state by showing how to keep track of the number of times the model has been called.\n\n```python\nimport nnx\nimport jax\nimport jax.numpy as jnp\n\nclass Count(nnx.Variable): pass\n\nclass Linear(nnx.Module):\n    def __init__(self, din: int, dout: int, *, ctx: nnx.Context):\n        key = ctx.make_rng("params")\n        self.w = nnx.Param(jax.random.uniform(key, (din, dout)))\n        self.b = nnx.Param(jnp.zeros((dout,)))\n        self.count = Count(0)  # track the number of calls\n\n    def __call__(self, x):\n        self.count += 1\n        return x @ self.w + self.b\n\nmodel = Linear(din=12, dout=2, ctx=nnx.context(0))\n\n# Forward pass and verify the call count\nx = jnp.ones((8, 12))\ny = model(x)\nassert model.count == 1\n```\n\nIn this example `nnx.context(0)` create a `PRNGKey` for `params` with seed `0`, this is used by `make_rng`\ninside `__init__` to generate a random key to initialize the parameters.\n\n### Training with the Functional API\n\nThe [Functional API](#functional-api) converts an NNX Module python semantics into pure pytree object with functional semantics. It is the recommended way to use NNX as it provides tight control over the state, allows you to use regular JAX transformations, and it minimizes overhead. In this example the model will be trained using Stochastic Gradient Descent (SGD).\n\n```python\n(params, counts), moduledef = model.partition(nnx.Param, Count)\n\n@jax.jit\ndef train_step(params, counts, x, y):\n    def loss_fn(params):\n        y_pred, (updates, _) = moduledef.apply(params, counts)(x)\n        loss = jax.numpy.mean((y_pred - y) ** 2)\n        return loss, updates.filter(Count)\n\n    # compute gradient\n    grads, counts = jax.grad(loss_fn, has_aux=True)(params)\n    # SGD update\n    params = jax.tree_map(lambda w, g: w - 0.1 * g, params, grads)\n\n    return params, counts\n\n# execute the training step\nparams, counts = train_step(params, counts, x, y)\nmodel = moduledef.merge(params, counts)\nassert model.count == 2\n```\n\n### Training with Lifted Transforms\n\n[Lifted Transforms](#lifted-transforms) provide a convenient way interact with NNX Modules. In this example, we use the `nnx.jit` and `nnx.grad` lifted transforms to define the training step. The model is trained using Stochastic Gradient Descent (SGD). Because lifted transforms automatically update the Module\'s state, `train_step` doesn\'t require a return statement.\n\n```python\n@nnx.jit\ndef train_step(model, x, y):\n    def loss_fn(model):\n        y_pred = model(x)\n        return jax.numpy.mean((y_pred - y) ** 2)\n    \n    # compute gradient\n    grads: nnx.State = nnx.grad(loss_fn, wrt=nnx.Param)(model)\n    # SGD update\n    model.update_state(\n        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter(nnx.Param), grads)\n    )\n\n# execute the training step\ntrain_step(model, x, y)\nassert model.count == 2\n```\n\n**Note**: Using `nnx.jit` introduces some overhead when compared to using `jax.jit` directly. Use `nnx.jit` for simple prototypes, but for production code use `jax.jit` directly.\n\n## Examples\n\n* [Using the Functional API](https://github.com/cgarciae/nnx/blob/main/examples/01_functional_api.py): Shows how to train a simple model using the functional API.\n* [Using Lifted Transforms](https://github.com/cgarciae/nnx/blob/main/examples/02_lifted_transforms.py): Shows how to train a simple model using lifted transforms.\n* [Using TrainState](https://github.com/cgarciae/nnx/blob/main/examples/03_train_state.py): Shows how to train a simple model using the functional API with the help of `TrainState`.\n* [Using PureModule](https://github.com/cgarciae/nnx/blob/main/examples/04_pure.py) (experimental): Shows how to train a simple model using the functional API and leveraging `PureModule` to simplify the code.\n* [Training a VAE](https://github.com/cgarciae/nnx/blob/main/examples/05_vae.py): Shows how to train a VAE on the binarized MNIST dataset, uses the functional API, `TrainState`, and shows how to use capture intermediate values to retrieve `kl_loss`.\n* [Scan over layers](https://github.com/cgarciae/nnx/blob/main/examples/06_scan_over_layers.py): An contrived example that implements scan over layers with dropout and a share BatcNorm layer to showcase how lifted transforms can be implemented. It uses the functional API along with `jax.vmap` and `jax.lax.scan`.\n* [Creating a Transformer](https://github.com/cgarciae/nnx/blob/main/examples/07_transformer.py): Shows how to create a Transformer with an auto-regressive decoder that uses scan over layers and a kv-cache for fast inference. Credits to @levskaya.\n\n## FAQs\n\n### Status\nNNX is still in early development so expect bugs and breaking changes. That said, current API is the result of months of experimentation and we don\'t expect any major changes in the near future.\n\n### How is it different from Flax?\nNNX takes the best features that allow Flax to scale to large projects and integrates them into a much simpler Module system with pythonic semantics. \n\nOne place in which NNX strongly deviates from Flax is that (currently) it avoids shape inference in favor of static initialization. It is not a technical limitation but rather a design choice. This design both simplifies the internal implementation and makes it easier to reason about the code for the user, at the cost of being more verbose at times. On the other hand, Pytorch users will feel right at home.\n\n### How is it different from Equinox?\nWhile they might look similar at a surface-level, NNX\'s Module system is more powerful and flexible than Equinox\'s, it contains the following additional features:\n\n* Uses regular python classes (no mandatory dataclass behavior).\n* Modules are mutable\n* Reference sharing between Modules is allowed\n* Mutable state lives inside the Module (no need for a separate [State container](https://docs.kidger.site/equinox/examples/stateful/)).\n* Supports node metadata and semantic partitioning.\n\nOne major difference between the two frameworks is that, by design, NNX Modules are not Pytrees. This adds a safety layer as it prevents state updates from being lost by accident due to referential transparency. It also removes the need of threading a separate [State container](https://docs.kidger.site/equinox/examples/stateful/) throughout the code in order to propagate state. In NNX state updates are either always preserved or explicitly discarded by the user.\n\n## User Guide\n\n### Modules\n\nNNX Modules are normal python classes, they obey regular python semantics such as mutability and reference sharing, including reference cycles. They can contain 2 types of attributes: node attributes and static attributes. Node attributes include NNX `Variable`s (e.g. `nnx.Param`), Numpy arrays, JAX arrays, submodules Modules, and other NNX types. All other types are treated as static attributes.\n\n```python\nclass Foo(nnx.Module):\n    def __init__(self, ctx: nnx.Context):\n        # node attributes\n        self.variable = nnx.Param(jnp.array(1))\n        self.np_buffer = np.array(2)\n        self.jax_buffer = jnp.array(3)\n        self.node = nnx.Node([4, 5])\n        self.submodule = nnx.Linear(2, 4, ctx=ctx)\n        # static attributes\n        self.int = 1\n        self.float = 2.0\n        self.str = "hello"\n        self.list = [1, 2, 3]\n\nmodel = Foo(din=12, dout=2, ctx=nnx.context(0))\n```\nAs shown above, python container types such as `list`, `tuple`, and `dict` are treated as static attributes, if similar functionality is needed, NNX provides the `Sequence` and `Dict` Modules.\n\n### Functional API\n\nNNX Modules are not pytrees so they cannot be passed to JAX transformations. In order to interact with JAX, a Module must be partitioned into a `State` and `ModuleDef` objects. The `State` object is a flat dictionary-like pytree structure that contains all the deduplicated node attributes, and the `ModuleDef` contains the static attributes and structural information needed to reconstruct the Module.\n\n```python\nstate, moduledef = model.partition()\n```\n```\nState({\n  (\'jax_buffer\',): Array(3),\n  (\'node\',): Node(value=[4, 5]),\n  (\'np_buffer\',): array(2),\n  (\'submodule\', \'bias\'): Param(value=Array(...)),\n  (\'submodule\', \'kernel\'): Param(value=Array(...)),\n  (\'variable\',): Param(value=Array(1))\n})\n```\n\n`State` and `ModuleDef` are pytrees so they can be passed to JAX transformations. More over, `ModuleDef` provides 2 very important methods: `merge` and `apply`. The `merge` method can be used to create a new `Module` from a `State` object:\n\n```python\nmodel = moduledef.merge(state)\n```\nThis can be use to e.g. recreate a module inside a JAX transformation. The `apply` provides a functional interface to the module, it can be used call any method or submodule and get the output and the updated state:\n\n```python\n# run __call__\ny, (state, moduledef) = moduledef.apply(state)(x)\n# run some_method\ny, (state, moduledef) = moduledef.apply(state).some_method(x)\n# run submodule\ny, (state, moduledef) = moduledef.apply(state).submodule(x)\n```\n\n`apply` can call any nested method or submodule as long as it can be accessed via the `.` or `[]` operators.\n\n### Partitioning State\nIn NNX you can filter based on any node type, most commonly you will want to filter based on `nnx.Variable` subclasses such as `nnx.Param` or `nnx.BatchStat`.\n\nHere are various examples of how you can use the `partition` method to split a module into multiple substates:\n\n```python\n# partition the module into the state with all the nodes and the moduledef\nstate, moduledef = model.partition()\n# verify that the state contains only params, else raise an error\nparams, moduledef = model.partition(nnx.Param)\n# split the state into params and batch_stats, verify no nodes are left\n(params, batch_stats), moduledef = model.partition(nnx.Param, nnx.BatchStat)\n# if there are any nodes left, use the `...` filter to capture them\n(params, batch_stats, rest), moduledef = model.partition(nnx.Param, nnx.BatchStat, ...)\n# using `...` as the only filter is equivalent to not passing any filters\nmodel.partition(...) = model.partition()\n```\n`partition` will make sure all nodes are match by atleast one filter, else it will raise an error. If you have non-`Variable` nodes like `nnx.Node`, `jax.Array`, or `numpy.ndarray` attributes, you can use the `...` filter which will match any node. For a more general filter you can pass a predicate function of the form:\n\n```python\n(path: Tuple[str, ...], value: Any) -> bool\n```\n\nTo reconstruct the module from a set of substates, you can use `merge` as usual but passing the substates as additional arguments:\n\n```python\nmodel = moduledef.merge(params, batch_stats, rest)\n```\n\nThe same is true for `apply`.\n\n```python\ny, (state, moduledef) = moduledef.apply(params, batch_stats, rest)(x)\n```\n\n Note that `apply` will return a single `state` object, if you need to re-partition the state you can use `State`\'s own `partition` method:\n\n```python\nparams, batch_stats, rest = state.partition(nnx.Param, nnx.BatchStat, ...)\n```\n\nAlternatively, if you are just interested in a subset of partitions, you can use the `State.filter` method which will not raise an error if some nodes are not matched by any filter:\n\n```python\n# only get params\nparams = state.filter(nnx.Param)\n# get params and batch_stats\nparams, batch_stats = state.filter(nnx.Param, nnx.BatchStat)\n```\n\n### Filters\n\nFilters let you select subsets of nodes based on some criteria. These are use throughout the API in method like `partition`, `filter`, and `pop_state`. There are 4 types of filters:\n\n* `type`: matches all node instances of the given type.\n* `...`: matches all nodes.\n* `(path, any) -> bool`: a predicate function that takes a node path and value and returns a boolean.\n* `Tuple[Filter, ...]`: a tuple of filters, matches all nodes that match any of the filters.\n\nNNX also provides the following custom filters:\n\n* `nnx.Not(filter)`: matches all nodes that do not match the given filter\n* `nnx.buffers`: matches all `numpy.ndarray` and `jax.Array` nodes\n\nHere is an example of how to use `Not` and `buffers`:\n```python\nrest = module.filter(nnx.Not(nnx.Param))\nbuffers = module.filter(nnx.buffers)\n```\n\n\n### Capturing Intermediate Values\nIn NNX you can easily propagate intemediate values by simply assigning them to an attribute at runtime. For convenience, you should assign them to a `Variable` attribute with a `collection` name by using `nnx.var` so you can easily retrieve them later.\n\nHere is an example of how to create a `Linear` module that captures its output into a `Variable` attribute with the `intermediates` collection name:\n\n```python\nclass Linear(nnx.Module):\n    def __init__(self, din: int, dout: int, *, ctx: nnx.Context):\n        key = ctx.make_rng("params")\n        self.w = nnx.Param(jax.random.uniform(key, (din, dout)))\n        self.b = nnx.Param(jnp.zeros((dout,)))\n\n    def __call__(self, x):\n        y = x @ self.w + self.b\n        self.y = nnx.Intermediate(y)\n        return y\n\nmodel = Linear(12, 2, ctx=nnx.context(0))\n```\nSince `y` is only created when the module is called, it is not available upon initialization. However, once you call the module `y` will be created. It is recommended that you use `pop_state` to retrieve temporary collections like `Intermediate`:\n\n```python\ny = model(jnp.ones((8, 12)))\nintermediates = model.pop_state(nnx.Intermediate)\n```\n`pop_state` will return a `State` object with the nodes that match the given filter and remove them from the module\'s attributes.\n\n```\nState({\n  (\'y\',): Intermediate(\n    value=Array(...)\n  )\n})\n```\n\nIf you use the functional API to call the module instead, the `Intermediate` nodes will be present in the output `state`. To retrieve the `intermediates` nodes and optionally separate them from the output `state` you can use `State.partition`:\n\n```python\nstate, moduledef = model.partition()\ny, (state, moduledef) = moduledef.apply(state)(jnp.ones((8, 12)))\n# "pop" the intermediates from the state\nintermediates, state = state.partition("intermediates", ...)\n```\n\nAlternatively, you can use `State.filter` to retrieve the `intermediates` nodes without removing them from the `state`.\n\n\n\n### Lifted Transforms\n\nNNX lifted transforms analogous versions of JAX transforms but they know how to work with Modules. They usually perform the following tasks:\n\n* Handle the Module\'s substates and Context\'s RNG streams according to the transform\'s semantics.\n* Properly propagating state in and out of the transform, including updating the input Module\'s state with updates that happen inside the transform.\n\nHere\'s a diagram illustrating how lifted transformations work:\n\n![lifted-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)\n\nCurrently NNX provides the `jit`, `grad`, and `scan` lifted transforms.\n\n#### Manual Lifting\n\nIn case you want to use JAX transforms directly you can always use the functional API\nto manually lift your Modules. \n\nHere we will create an example of how to implement an MLP that uses "scan over layers" to efficiently process a sequence of inputs assuming that each layer has the same parameters and input/output dimensions. The first thing we need to do is create a `Block` module that represents a single layer, this block with just contain a `Linear` layer, a `Dropout` layer, and a `GELU` activation function:\n\n```python\nclass Block(nnx.Module):\n    def __init__(self, dim: int, *, ctx: nnx.Context):\n        self.linear = nnx.Linear(dim, dim, ctx=ctx)\n        self.dropout = nnx.Dropout(0.5)\n\n    def __call__(self, x: jax.Array, *, train: bool, ctx: nnx.Context) -> jax.Array:\n        x = self.linear(x)\n        x = self.dropout(x, deterministic=not train, ctx=ctx)\n        x = jax.nn.gelu(x)\n        return x\n```\n\nNow we will define `ScanMLP`. During `__init__`, instead of creating a list of `Block`s, we will use `jax.vmap` to create a single `Block` whose parameters have an addtional `layer` axis. This will allow us to pass the parameters as inputs to scan so it will apply a layer at each step.\n\n```python\nclass ScanMLP(nnx.Module):\n    def __init__(self, dim: int, *, n_layers: int, ctx: nnx.Context):\n        params_key = jax.random.split(ctx.make_rng("params"), n_layers)\n        self.n_layers = n_layers\n        self.layers = jax.vmap(\n            lambda key: Block(dim, ctx=nnx.context(params=key)).partition()\n        )(params_key).merge()\n\n```\nNote that we split the `params` key into `n_layers` keys so each layer has different parameters.\n\nNow we will define `__call__`. Here we need to split the `dropout` key into `n_layers` keys so each layer has a different dropout mask, and `partition` the layers to get their `params`. Both `params` and `dropout_key` will be passed as inputs, `x` will be the carry value. Inside the `scan_fn` we will merge the `params` back into a `Block` module and\napply it to the input `x`, passing the sliced `dropout_key` as part of the `Context`.\n\n\n```python\n    def __call__(self, x: jax.Array, *, train: bool, ctx: nnx.Context) -> jax.Array:\n        dropout_key = jax.random.split(ctx.make_rng("dropout"), self.n_layers)\n        params, moduledef = self.layers.partition(nnx.Param)\n\n        def scan_fn(x: inputs):\n            params, dropout_key = inputs\n            module = moduledef.merge(params)\n            x = module(x, train=train, ctx=nnx.context(dropout=dropout_key))\n            return x, module.filter(nnx.Param)\n\n        x, params = jax.lax.scan(scan_fn, x, (params, dropout_key))\n        self.layers.update_state(params)\n        return x\n```\nFinally we apply `jax.lax.scan`, update the `layers` state with the new `params`, and return the final `x` value.\n\nHere is a simple way to test our `ScanMLP`:\n\n```python\nmodel = ScanMLP(10, n_layers=5, ctx=nnx.context(0))\n\nx = jnp.ones((3, 10))\ny = model(x, train=True, ctx=nnx.context(dropout=1))\n```\n\nFor a more robust implementation with comments take a look at the [Scan over layers](https://github.com/cgarciae/nnx/blob/main/examples/06_scan_over_layers.py) example.\n\n### Case Studies\n#### Shared State\n\nIn NNX, you can create modules that share state between them. This is useful when designing complex neural network architectures, as it allows you to reuse certain layers and reduce the number of learnable parameters.\n\nHere\'s an example of creating a module with shared state:\n\n```python\nclass Block(nnx.Module):\n    def __init__(self, linear: nnx.Linear, *, ctx: nnx.Context):\n        self.linear = linear\n        self.bn = nnx.BatchNorm(2, ctx=ctx)\n\n    def __call__(self, x, *, ctx: nnx.Context):\n        x = self.linear(x)\n        x = self.bn(x, ctx=ctx)\n        x = nnx.relu(x)\n        return x\n\nclass Model(nnx.Module):\n    def __init__(self, *, ctx: nnx.Context):\n        shared = nnx.Linear(2, 2, ctx=ctx)\n        self.block1 = Block(shared, ctx=ctx)\n        self.block2 = Block(shared, ctx=ctx)\n\n    def __call__(self, x, *, ctx: nnx.Context):\n        x = self.block1(x, ctx=ctx)\n        x = self.block2(x, ctx=ctx)\n        return x\n```\n\nIn this example, the `Model` module contains two instances of the `Block` module. Each instance shares the same `nnx.Linear` module. To run the model, you can use the Context `flags` argument to set the `use_running_average` flag for all `BatchNorm` modules.\n\nHere\'s an example of computing the loss for a `Model` instance:\n\n```python\ndef loss_fn(model: Model, x: jax.Array, y: jax.Array):\n    ctx = nnx.context(flags=dict(use_running_average=True))\n    y_pred = model(x, ctx=ctx)\n    return jnp.mean((y - y_pred) ** 2)\n```\n\nIt\'s important to note that the state for the shared `nnx.Linear` module will be kept in sync at all times on both `Block` instances, including during gradient updates.\n',
-    'author': 'Cristian Garcia',
-    'author_email': 'cgarcia.e88@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.12',
-}
+_**N**eural **N**etworks for JA**X**_
 
+NNX is a Neural Networks library for JAX that provides a simple yet powerful module system that adheres to standard Python semantics. Its aim is to combine the robustness of [Flax](https://flax.readthedocs.io/en/latest/) with a simplified, Pythonic API akin to that of [PyTorch](https://pytorch.org/).
+
+* **Pythonic**: Modules are just regular python classes, they contain their own state, are fully mutable, and allow sharing references between Modules.
+* **Compatible**: Easily convert back and forth between Modules and pytrees using the Functional API to integrate with any JAX API.
+* **Safe**: NNX incorporates mechanisms to try to prevent tracer leakage, avoid stale RNGs, and ensure proper state propagation in order to help produce correct JAX programs.
+* **Semantic**: Partition a Module's state into different semantic collections, allowing for fine-grained control when applying JAX transformations.
+
+#### Table of Contents
+* [Installation](#installation)
+* [Getting Started](#getting-started)
+* [FAQs](#faqs)
+* [Examples](#examples)
+* [User Guide](#user-guide)
+
+## Installation
+
+To get started with `nnx`, install the package via pip:
+
+```
+pip install nnx
+```
+For the most recent version, install directly from our GitHub repository:
+
+```
+pip install git+https://github.com/cgarciae/nnx
+```
+
+## Getting Started
+
+The following example guides you through creating a basic `Linear` model with NNX and executing a forward pass. It also demonstrate how handle mutable state by showing how to keep track of the number of times the model has been called.
+
+```python
+import nnx
+import jax
+import jax.numpy as jnp
+
+class Count(nnx.Variable): pass
+
+class Linear(nnx.Module):
+    def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
+        key = ctx.make_rng("params")
+        self.w = nnx.Param(jax.random.uniform(key, (din, dout)))
+        self.b = nnx.Param(jnp.zeros((dout,)))
+        self.count = Count(0)  # track the number of calls
+
+    def __call__(self, x):
+        self.count += 1
+        return x @ self.w + self.b
+
+model = Linear(din=12, dout=2, ctx=nnx.context(0))
+
+# Forward pass and verify the call count
+x = jnp.ones((8, 12))
+y = model(x)
+assert model.count == 1
+```
+
+In this example `nnx.context(0)` create a `PRNGKey` for `params` with seed `0`, this is used by `make_rng`
+inside `__init__` to generate a random key to initialize the parameters.
+
+### Training with the Functional API
+
+The [Functional API](#functional-api) converts an NNX Module python semantics into pure pytree object with functional semantics. It is the recommended way to use NNX as it provides tight control over the state, allows you to use regular JAX transformations, and it minimizes overhead. In this example the model will be trained using Stochastic Gradient Descent (SGD).
+
+```python
+(params, counts), moduledef = model.partition(nnx.Param, Count)
+
+@jax.jit
+def train_step(params, counts, x, y):
+    def loss_fn(params):
+        y_pred, (updates, _) = moduledef.apply(params, counts)(x)
+        loss = jax.numpy.mean((y_pred - y) ** 2)
+        return loss, updates.filter(Count)
+
+    # compute gradient
+    grads, counts = jax.grad(loss_fn, has_aux=True)(params)
+    # SGD update
+    params = jax.tree_map(lambda w, g: w - 0.1 * g, params, grads)
+
+    return params, counts
+
+# execute the training step
+params, counts = train_step(params, counts, x, y)
+model = moduledef.merge(params, counts)
+assert model.count == 2
+```
+
+### Training with Lifted Transforms
+
+[Lifted Transforms](#lifted-transforms) provide a convenient way interact with NNX Modules. In this example, we use the `nnx.jit` and `nnx.grad` lifted transforms to define the training step. The model is trained using Stochastic Gradient Descent (SGD). Because lifted transforms automatically update the Module's state, `train_step` doesn't require a return statement.
+
+```python
+@nnx.jit
+def train_step(model, x, y):
+    def loss_fn(model):
+        y_pred = model(x)
+        return jax.numpy.mean((y_pred - y) ** 2)
+    
+    # compute gradient
+    grads: nnx.State = nnx.grad(loss_fn, wrt=nnx.Param)(model)
+    # SGD update
+    model.update_state(
+        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter(nnx.Param), grads)
+    )
+
+# execute the training step
+train_step(model, x, y)
+assert model.count == 2
+```
+
+**Note**: Using `nnx.jit` introduces some overhead when compared to using `jax.jit` directly. Use `nnx.jit` for simple prototypes, but for production code use `jax.jit` directly.
+
+## Examples
+
+* [Using the Functional API](https://github.com/cgarciae/nnx/blob/main/examples/01_functional_api.py): Shows how to train a simple model using the functional API.
+* [Using Lifted Transforms](https://github.com/cgarciae/nnx/blob/main/examples/02_lifted_transforms.py): Shows how to train a simple model using lifted transforms.
+* [Using TrainState](https://github.com/cgarciae/nnx/blob/main/examples/03_train_state.py): Shows how to train a simple model using the functional API with the help of `TrainState`.
+* [Using PureModule](https://github.com/cgarciae/nnx/blob/main/examples/04_pure.py) (experimental): Shows how to train a simple model using the functional API and leveraging `PureModule` to simplify the code.
+* [Training a VAE](https://github.com/cgarciae/nnx/blob/main/examples/05_vae.py): Shows how to train a VAE on the binarized MNIST dataset, uses the functional API, `TrainState`, and shows how to use capture intermediate values to retrieve `kl_loss`.
+* [Scan over layers](https://github.com/cgarciae/nnx/blob/main/examples/06_scan_over_layers.py): An contrived example that implements scan over layers with dropout and a share BatcNorm layer to showcase how lifted transforms can be implemented. It uses the functional API along with `jax.vmap` and `jax.lax.scan`.
+* [Creating a Transformer](https://github.com/cgarciae/nnx/blob/main/examples/07_transformer.py): Shows how to create a Transformer with an auto-regressive decoder that uses scan over layers and a kv-cache for fast inference. Credits to @levskaya.
+
+## FAQs
+
+### Status
+NNX is still in early development so expect bugs and breaking changes. That said, current API is the result of months of experimentation and we don't expect any major changes in the near future.
+
+### How is it different from Flax?
+NNX takes the best features that allow Flax to scale to large projects and integrates them into a much simpler Module system with pythonic semantics. 
+
+One place in which NNX strongly deviates from Flax is that (currently) it avoids shape inference in favor of static initialization. It is not a technical limitation but rather a design choice. This design both simplifies the internal implementation and makes it easier to reason about the code for the user, at the cost of being more verbose at times. On the other hand, Pytorch users will feel right at home.
+
+### How is it different from Equinox?
+While they might look similar at a surface-level, NNX's Module system is more powerful and flexible than Equinox's, it contains the following additional features:
+
+* Uses regular python classes (no mandatory dataclass behavior).
+* Modules are mutable
+* Reference sharing between Modules is allowed
+* Mutable state lives inside the Module (no need for a separate [State container](https://docs.kidger.site/equinox/examples/stateful/)).
+* Supports node metadata and semantic partitioning.
+
+One major difference between the two frameworks is that, by design, NNX Modules are not Pytrees. This adds a safety layer as it prevents state updates from being lost by accident due to referential transparency. It also removes the need of threading a separate [State container](https://docs.kidger.site/equinox/examples/stateful/) throughout the code in order to propagate state. In NNX state updates are either always preserved or explicitly discarded by the user.
+
+## User Guide
+
+### Modules
+
+NNX Modules are normal python classes, they obey regular python semantics such as mutability and reference sharing, including reference cycles. They can contain 2 types of attributes: node attributes and static attributes. Node attributes include NNX `Variable`s (e.g. `nnx.Param`), Numpy arrays, JAX arrays, submodules Modules, and other NNX types. All other types are treated as static attributes.
+
+```python
+class Foo(nnx.Module):
+    def __init__(self, ctx: nnx.Context):
+        # node attributes
+        self.variable = nnx.Param(jnp.array(1))
+        self.np_buffer = np.array(2)
+        self.jax_buffer = jnp.array(3)
+        self.node = nnx.Node([4, 5])
+        self.submodule = nnx.Linear(2, 4, ctx=ctx)
+        # static attributes
+        self.int = 1
+        self.float = 2.0
+        self.str = "hello"
+        self.list = [1, 2, 3]
+
+model = Foo(din=12, dout=2, ctx=nnx.context(0))
+```
+As shown above, python container types such as `list`, `tuple`, and `dict` are treated as static attributes, if similar functionality is needed, NNX provides the `Sequence` and `Dict` Modules.
+
+### Functional API
+
+NNX Modules are not pytrees so they cannot be passed to JAX transformations. In order to interact with JAX, a Module must be partitioned into a `State` and `ModuleDef` objects. The `State` object is a flat dictionary-like pytree structure that contains all the deduplicated node attributes, and the `ModuleDef` contains the static attributes and structural information needed to reconstruct the Module.
+
+```python
+state, moduledef = model.partition()
+```
+```
+State({
+  ('jax_buffer',): Array(3),
+  ('node',): Node(value=[4, 5]),
+  ('np_buffer',): array(2),
+  ('submodule', 'bias'): Param(value=Array(...)),
+  ('submodule', 'kernel'): Param(value=Array(...)),
+  ('variable',): Param(value=Array(1))
+})
+```
+
+`State` and `ModuleDef` are pytrees so they can be passed to JAX transformations. More over, `ModuleDef` provides 2 very important methods: `merge` and `apply`. The `merge` method can be used to create a new `Module` from a `State` object:
+
+```python
+model = moduledef.merge(state)
+```
+This can be use to e.g. recreate a module inside a JAX transformation. The `apply` provides a functional interface to the module, it can be used call any method or submodule and get the output and the updated state:
+
+```python
+# run __call__
+y, (state, moduledef) = moduledef.apply(state)(x)
+# run some_method
+y, (state, moduledef) = moduledef.apply(state).some_method(x)
+# run submodule
+y, (state, moduledef) = moduledef.apply(state).submodule(x)
+```
+
+`apply` can call any nested method or submodule as long as it can be accessed via the `.` or `[]` operators.
+
+### Partitioning State
+In NNX you can filter based on any node type, most commonly you will want to filter based on `nnx.Variable` subclasses such as `nnx.Param` or `nnx.BatchStat`.
+
+Here are various examples of how you can use the `partition` method to split a module into multiple substates:
+
+```python
+# partition the module into the state with all the nodes and the moduledef
+state, moduledef = model.partition()
+# verify that the state contains only params, else raise an error
+params, moduledef = model.partition(nnx.Param)
+# split the state into params and batch_stats, verify no nodes are left
+(params, batch_stats), moduledef = model.partition(nnx.Param, nnx.BatchStat)
+# if there are any nodes left, use the `...` filter to capture them
+(params, batch_stats, rest), moduledef = model.partition(nnx.Param, nnx.BatchStat, ...)
+# using `...` as the only filter is equivalent to not passing any filters
+model.partition(...) = model.partition()
+```
+`partition` will make sure all nodes are match by atleast one filter, else it will raise an error. If you have non-`Variable` nodes like `nnx.Node`, `jax.Array`, or `numpy.ndarray` attributes, you can use the `...` filter which will match any node. For a more general filter you can pass a predicate function of the form:
+
+```python
+(path: Tuple[str, ...], value: Any) -> bool
+```
+
+To reconstruct the module from a set of substates, you can use `merge` as usual but passing the substates as additional arguments:
+
+```python
+model = moduledef.merge(params, batch_stats, rest)
+```
+
+The same is true for `apply`.
+
+```python
+y, (state, moduledef) = moduledef.apply(params, batch_stats, rest)(x)
+```
+
+ Note that `apply` will return a single `state` object, if you need to re-partition the state you can use `State`'s own `partition` method:
+
+```python
+params, batch_stats, rest = state.partition(nnx.Param, nnx.BatchStat, ...)
+```
+
+Alternatively, if you are just interested in a subset of partitions, you can use the `State.filter` method which will not raise an error if some nodes are not matched by any filter:
+
+```python
+# only get params
+params = state.filter(nnx.Param)
+# get params and batch_stats
+params, batch_stats = state.filter(nnx.Param, nnx.BatchStat)
+```
+
+### Filters
+
+Filters let you select subsets of nodes based on some criteria. These are use throughout the API in method like `partition`, `filter`, and `pop_state`. There are 4 types of filters:
+
+* `type`: matches all node instances of the given type.
+* `...`: matches all nodes.
+* `(path, any) -> bool`: a predicate function that takes a node path and value and returns a boolean.
+* `Tuple[Filter, ...]`: a tuple of filters, matches all nodes that match any of the filters.
+
+NNX also provides the following custom filters:
+
+* `nnx.Not(filter)`: matches all nodes that do not match the given filter
+* `nnx.buffers`: matches all `numpy.ndarray` and `jax.Array` nodes
+
+Here is an example of how to use `Not` and `buffers`:
+```python
+rest = module.filter(nnx.Not(nnx.Param))
+buffers = module.filter(nnx.buffers)
+```
+
+
+### Capturing Intermediate Values
+In NNX you can easily propagate intemediate values by simply assigning them to an attribute at runtime. For convenience, you should assign them to a `Variable` attribute with a `collection` name by using `nnx.var` so you can easily retrieve them later.
+
+Here is an example of how to create a `Linear` module that captures its output into a `Variable` attribute with the `intermediates` collection name:
+
+```python
+class Linear(nnx.Module):
+    def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
+        key = ctx.make_rng("params")
+        self.w = nnx.Param(jax.random.uniform(key, (din, dout)))
+        self.b = nnx.Param(jnp.zeros((dout,)))
+
+    def __call__(self, x):
+        y = x @ self.w + self.b
+        self.y = nnx.Intermediate(y)
+        return y
+
+model = Linear(12, 2, ctx=nnx.context(0))
+```
+Since `y` is only created when the module is called, it is not available upon initialization. However, once you call the module `y` will be created. It is recommended that you use `pop_state` to retrieve temporary collections like `Intermediate`:
+
+```python
+y = model(jnp.ones((8, 12)))
+intermediates = model.pop_state(nnx.Intermediate)
+```
+`pop_state` will return a `State` object with the nodes that match the given filter and remove them from the module's attributes.
+
+```
+State({
+  ('y',): Intermediate(
+    value=Array(...)
+  )
+})
+```
+
+If you use the functional API to call the module instead, the `Intermediate` nodes will be present in the output `state`. To retrieve the `intermediates` nodes and optionally separate them from the output `state` you can use `State.partition`:
+
+```python
+state, moduledef = model.partition()
+y, (state, moduledef) = moduledef.apply(state)(jnp.ones((8, 12)))
+# "pop" the intermediates from the state
+intermediates, state = state.partition("intermediates", ...)
+```
+
+Alternatively, you can use `State.filter` to retrieve the `intermediates` nodes without removing them from the `state`.
+
+
+
+### Lifted Transforms
+
+NNX lifted transforms analogous versions of JAX transforms but they know how to work with Modules. They usually perform the following tasks:
+
+* Handle the Module's substates and Context's RNG streams according to the transform's semantics.
+* Properly propagating state in and out of the transform, including updating the input Module's state with updates that happen inside the transform.
+
+Here's a diagram illustrating how lifted transformations work:
+
+![lifted-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
+
+Currently NNX provides the `jit`, `grad`, and `scan` lifted transforms.
+
+#### Manual Lifting
+
+In case you want to use JAX transforms directly you can always use the functional API
+to manually lift your Modules. 
+
+Here we will create an example of how to implement an MLP that uses "scan over layers" to efficiently process a sequence of inputs assuming that each layer has the same parameters and input/output dimensions. The first thing we need to do is create a `Block` module that represents a single layer, this block with just contain a `Linear` layer, a `Dropout` layer, and a `GELU` activation function:
+
+```python
+class Block(nnx.Module):
+    def __init__(self, dim: int, *, ctx: nnx.Context):
+        self.linear = nnx.Linear(dim, dim, ctx=ctx)
+        self.dropout = nnx.Dropout(0.5)
+
+    def __call__(self, x: jax.Array, *, train: bool, ctx: nnx.Context) -> jax.Array:
+        x = self.linear(x)
+        x = self.dropout(x, deterministic=not train, ctx=ctx)
+        x = jax.nn.gelu(x)
+        return x
+```
+
+Now we will define `ScanMLP`. During `__init__`, instead of creating a list of `Block`s, we will use `jax.vmap` to create a single `Block` whose parameters have an addtional `layer` axis. This will allow us to pass the parameters as inputs to scan so it will apply a layer at each step.
+
+```python
+class ScanMLP(nnx.Module):
+    def __init__(self, dim: int, *, n_layers: int, ctx: nnx.Context):
+        params_key = jax.random.split(ctx.make_rng("params"), n_layers)
+        self.n_layers = n_layers
+        self.layers = jax.vmap(
+            lambda key: Block(dim, ctx=nnx.context(params=key)).partition()
+        )(params_key).merge()
+
+```
+Note that we split the `params` key into `n_layers` keys so each layer has different parameters.
+
+Now we will define `__call__`. Here we need to split the `dropout` key into `n_layers` keys so each layer has a different dropout mask, and `partition` the layers to get their `params`. Both `params` and `dropout_key` will be passed as inputs, `x` will be the carry value. Inside the `scan_fn` we will merge the `params` back into a `Block` module and
+apply it to the input `x`, passing the sliced `dropout_key` as part of the `Context`.
+
+
+```python
+    def __call__(self, x: jax.Array, *, train: bool, ctx: nnx.Context) -> jax.Array:
+        dropout_key = jax.random.split(ctx.make_rng("dropout"), self.n_layers)
+        params, moduledef = self.layers.partition(nnx.Param)
+
+        def scan_fn(x: inputs):
+            params, dropout_key = inputs
+            module = moduledef.merge(params)
+            x = module(x, train=train, ctx=nnx.context(dropout=dropout_key))
+            return x, module.filter(nnx.Param)
+
+        x, params = jax.lax.scan(scan_fn, x, (params, dropout_key))
+        self.layers.update_state(params)
+        return x
+```
+Finally we apply `jax.lax.scan`, update the `layers` state with the new `params`, and return the final `x` value.
+
+Here is a simple way to test our `ScanMLP`:
+
+```python
+model = ScanMLP(10, n_layers=5, ctx=nnx.context(0))
+
+x = jnp.ones((3, 10))
+y = model(x, train=True, ctx=nnx.context(dropout=1))
+```
+
+For a more robust implementation with comments take a look at the [Scan over layers](https://github.com/cgarciae/nnx/blob/main/examples/06_scan_over_layers.py) example.
+
+### Case Studies
+#### Shared State
+
+In NNX, you can create modules that share state between them. This is useful when designing complex neural network architectures, as it allows you to reuse certain layers and reduce the number of learnable parameters.
+
+Here's an example of creating a module with shared state:
+
+```python
+class Block(nnx.Module):
+    def __init__(self, linear: nnx.Linear, *, ctx: nnx.Context):
+        self.linear = linear
+        self.bn = nnx.BatchNorm(2, ctx=ctx)
+
+    def __call__(self, x, *, ctx: nnx.Context):
+        x = self.linear(x)
+        x = self.bn(x, ctx=ctx)
+        x = nnx.relu(x)
+        return x
+
+class Model(nnx.Module):
+    def __init__(self, *, ctx: nnx.Context):
+        shared = nnx.Linear(2, 2, ctx=ctx)
+        self.block1 = Block(shared, ctx=ctx)
+        self.block2 = Block(shared, ctx=ctx)
+
+    def __call__(self, x, *, ctx: nnx.Context):
+        x = self.block1(x, ctx=ctx)
+        x = self.block2(x, ctx=ctx)
+        return x
+```
+
+In this example, the `Model` module contains two instances of the `Block` module. Each instance shares the same `nnx.Linear` module. To run the model, you can use the Context `flags` argument to set the `use_running_average` flag for all `BatchNorm` modules.
+
+Here's an example of computing the loss for a `Model` instance:
+
+```python
+def loss_fn(model: Model, x: jax.Array, y: jax.Array):
+    ctx = nnx.context(flags=dict(use_running_average=True))
+    y_pred = model(x, ctx=ctx)
+    return jnp.mean((y - y_pred) ** 2)
+```
+
+It's important to note that the state for the shared `nnx.Linear` module will be kept in sync at all times on both `Block` instances, including during gradient updates.
 
-setup(**setup_kwargs)
```

