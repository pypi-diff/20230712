# Comparing `tmp/pinject_design-0.1.92.tar.gz` & `tmp/pinject_design-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinject_design-0.1.92.tar", max compression
+gzip compressed data, was "pinject_design-0.1.93.tar", max compression
```

## Comparing `pinject_design-0.1.92.tar` & `pinject_design-0.1.93.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinject_design-0.1.92/LICENSE
--rw-r--r--   0        0        0      170 2022-12-05 13:41:50.000000 pinject_design-0.1.92/pinject_design/__init__.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinject_design-0.1.92/pinject_design/di/__init__.py
--rw-r--r--   0        0        0     1786 2022-10-12 04:28:37.000000 pinject_design-0.1.92/pinject_design/di/app_designed.py
--rw-r--r--   0        0        0     2442 2023-05-06 03:52:35.678286 pinject_design-0.1.92/pinject_design/di/app_injected.py
--rw-r--r--   0        0        0      640 2022-10-09 04:01:27.000000 pinject_design-0.1.92/pinject_design/di/applicative.py
--rw-r--r--   0        0        0     6671 2023-05-08 06:26:47.063185 pinject_design-0.1.92/pinject_design/di/ast.py
--rw-r--r--   0        0        0     7338 2023-05-04 06:32:55.349238 pinject_design-0.1.92/pinject_design/di/design.py
--rw-r--r--   0        0        0     1943 2023-05-09 04:27:42.242474 pinject_design-0.1.92/pinject_design/di/designed.py
--rw-r--r--   0        0        0     1341 2022-11-10 03:41:15.000000 pinject_design-0.1.92/pinject_design/di/dynamic_proxy.py
--rw-r--r--   0        0        0    28337 2023-07-04 16:13:18.254578 pinject_design-0.1.92/pinject_design/di/graph.py
--rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinject_design-0.1.92/pinject_design/di/implicit_globals.py
--rw-r--r--   0        0        0    31694 2023-07-11 15:15:09.600147 pinject_design-0.1.92/pinject_design/di/injected.py
--rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinject_design-0.1.92/pinject_design/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinject_design-0.1.92/pinject_design/di/permissioned/__init__.py
--rw-r--r--   0        0        0     7815 2023-05-24 05:53:54.289323 pinject_design-0.1.92/pinject_design/di/permissioned/blueprint.py
--rw-r--r--   0        0        0      147 2023-07-02 07:30:07.430121 pinject_design-0.1.92/pinject_design/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject_design-0.1.92/pinject_design/di/provider.py
--rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinject_design-0.1.92/pinject_design/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinject_design-0.1.92/pinject_design/di/session.py
--rw-r--r--   0        0        0     2069 2022-10-12 04:28:37.000000 pinject_design-0.1.92/pinject_design/di/sessioned.py
--rw-r--r--   0        0        0     5730 2023-05-08 04:41:16.885893 pinject_design-0.1.92/pinject_design/di/static_proxy.py
--rw-r--r--   0        0        0      151 2022-10-12 04:42:16.000000 pinject_design-0.1.92/pinject_design/di/test_ast.py
--rw-r--r--   0        0        0      995 2022-10-08 11:27:55.000000 pinject_design-0.1.92/pinject_design/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1505 2022-10-09 04:19:51.000000 pinject_design-0.1.92/pinject_design/di/test_graph.py
--rw-r--r--   0        0        0     2249 2023-04-19 08:08:57.197957 pinject_design-0.1.92/pinject_design/di/test_injected.py
--rw-r--r--   0        0        0      705 2022-10-12 04:28:37.000000 pinject_design-0.1.92/pinject_design/di/test_proxiable.py
--rw-r--r--   0        0        0    28581 2023-07-11 04:43:03.271241 pinject_design-0.1.92/pinject_design/di/util.py
--rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinject_design-0.1.92/pinject_design/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinject_design-0.1.92/pinject_design/global_configs
--rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinject_design-0.1.92/pinject_design/global_configs.py
--rw-r--r--   0        0        0     1316 2023-06-15 09:48:02.404293 pinject_design-0.1.92/pinject_design/graph_inspection.py
--rw-r--r--   0        0        0     1612 2023-07-11 12:13:24.402905 pinject_design-0.1.92/pinject_design/helper_structure.py
--rw-r--r--   0        0        0     6272 2023-07-11 12:13:24.403516 pinject_design-0.1.92/pinject_design/helpers.py
--rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinject_design-0.1.92/pinject_design/module_inspector.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinject_design-0.1.92/pinject_design/nx_graph_util.py
--rw-r--r--   0        0        0      467 2023-05-29 00:14:18.924421 pinject_design-0.1.92/pinject_design/pinject_design.iml
--rw-r--r--   0        0        0    20791 2023-07-11 12:13:24.404826 pinject_design-0.1.92/pinject_design/run_config_utils.py
--rw-r--r--   0        0        0     1590 2023-07-11 12:13:24.405223 pinject_design-0.1.92/pinject_design/run_config_utils_v2.py
--rw-r--r--   0        0        0      938 2023-07-11 12:13:24.405644 pinject_design-0.1.92/pinject_design/test_package/__init__.py
--rw-r--r--   0        0        0      234 2023-07-11 12:13:24.406011 pinject_design-0.1.92/pinject_design/test_package/child/__init__.py
--rw-r--r--   0        0        0      284 2023-07-11 12:13:24.406483 pinject_design-0.1.92/pinject_design/test_package/child/module1.py
--rw-r--r--   0        0        0    19827 2023-07-11 15:01:19.140665 pinject_design-0.1.92/pinject_design/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinject_design-0.1.92/pinject_design/viz/__init__.py
--rw-r--r--   0        0        0       78 2022-04-27 03:51:47.000000 pinject_design-0.1.92/pinject_design/viz/graph.py
--rw-r--r--   0        0        0      639 2023-07-11 15:15:15.334477 pinject_design-0.1.92/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pinject_design-0.1.92/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinject_design-0.1.93/LICENSE
+-rw-r--r--   0        0        0      170 2022-12-05 13:41:50.000000 pinject_design-0.1.93/pinject_design/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinject_design-0.1.93/pinject_design/di/__init__.py
+-rw-r--r--   0        0        0     1786 2022-10-12 04:28:37.000000 pinject_design-0.1.93/pinject_design/di/app_designed.py
+-rw-r--r--   0        0        0     2536 2023-07-12 07:11:32.777696 pinject_design-0.1.93/pinject_design/di/app_injected.py
+-rw-r--r--   0        0        0      640 2022-10-09 04:01:27.000000 pinject_design-0.1.93/pinject_design/di/applicative.py
+-rw-r--r--   0        0        0     6671 2023-05-08 06:26:47.063185 pinject_design-0.1.93/pinject_design/di/ast.py
+-rw-r--r--   0        0        0     7402 2023-07-12 06:48:32.126362 pinject_design-0.1.93/pinject_design/di/design.py
+-rw-r--r--   0        0        0     1943 2023-05-09 04:27:42.242474 pinject_design-0.1.93/pinject_design/di/designed.py
+-rw-r--r--   0        0        0     1341 2022-11-10 03:41:15.000000 pinject_design-0.1.93/pinject_design/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    29448 2023-07-12 06:36:42.176942 pinject_design-0.1.93/pinject_design/di/graph.py
+-rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinject_design-0.1.93/pinject_design/di/implicit_globals.py
+-rw-r--r--   0        0        0    32106 2023-07-12 06:06:44.180482 pinject_design-0.1.93/pinject_design/di/injected.py
+-rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinject_design-0.1.93/pinject_design/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinject_design-0.1.93/pinject_design/di/permissioned/__init__.py
+-rw-r--r--   0        0        0     7815 2023-05-24 05:53:54.289323 pinject_design-0.1.93/pinject_design/di/permissioned/blueprint.py
+-rw-r--r--   0        0        0      147 2023-07-02 07:30:07.430121 pinject_design-0.1.93/pinject_design/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject_design-0.1.93/pinject_design/di/provider.py
+-rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinject_design-0.1.93/pinject_design/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinject_design-0.1.93/pinject_design/di/session.py
+-rw-r--r--   0        0        0     2069 2022-10-12 04:28:37.000000 pinject_design-0.1.93/pinject_design/di/sessioned.py
+-rw-r--r--   0        0        0     5730 2023-05-08 04:41:16.885893 pinject_design-0.1.93/pinject_design/di/static_proxy.py
+-rw-r--r--   0        0        0      151 2022-10-12 04:42:16.000000 pinject_design-0.1.93/pinject_design/di/test_ast.py
+-rw-r--r--   0        0        0      995 2022-10-08 11:27:55.000000 pinject_design-0.1.93/pinject_design/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1505 2022-10-09 04:19:51.000000 pinject_design-0.1.93/pinject_design/di/test_graph.py
+-rw-r--r--   0        0        0     2249 2023-04-19 08:08:57.197957 pinject_design-0.1.93/pinject_design/di/test_injected.py
+-rw-r--r--   0        0        0      705 2022-10-12 04:28:37.000000 pinject_design-0.1.93/pinject_design/di/test_proxiable.py
+-rw-r--r--   0        0        0    28581 2023-07-11 04:43:03.271241 pinject_design-0.1.93/pinject_design/di/util.py
+-rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinject_design-0.1.93/pinject_design/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinject_design-0.1.93/pinject_design/global_configs
+-rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinject_design-0.1.93/pinject_design/global_configs.py
+-rw-r--r--   0        0        0     1316 2023-06-15 09:48:02.404293 pinject_design-0.1.93/pinject_design/graph_inspection.py
+-rw-r--r--   0        0        0     1612 2023-07-11 12:13:24.402905 pinject_design-0.1.93/pinject_design/helper_structure.py
+-rw-r--r--   0        0        0     6272 2023-07-11 12:13:24.403516 pinject_design-0.1.93/pinject_design/helpers.py
+-rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinject_design-0.1.93/pinject_design/module_inspector.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinject_design-0.1.93/pinject_design/nx_graph_util.py
+-rw-r--r--   0        0        0      467 2023-05-29 00:14:18.924421 pinject_design-0.1.93/pinject_design/pinject_design.iml
+-rw-r--r--   0        0        0    20791 2023-07-11 12:13:24.404826 pinject_design-0.1.93/pinject_design/run_config_utils.py
+-rw-r--r--   0        0        0     1590 2023-07-11 12:13:24.405223 pinject_design-0.1.93/pinject_design/run_config_utils_v2.py
+-rw-r--r--   0        0        0      938 2023-07-11 12:13:24.405644 pinject_design-0.1.93/pinject_design/test_package/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-11 12:13:24.406011 pinject_design-0.1.93/pinject_design/test_package/child/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-11 12:13:24.406483 pinject_design-0.1.93/pinject_design/test_package/child/module1.py
+-rw-r--r--   0        0        0    17998 2023-07-12 06:05:41.275007 pinject_design-0.1.93/pinject_design/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinject_design-0.1.93/pinject_design/viz/__init__.py
+-rw-r--r--   0        0        0       78 2022-04-27 03:51:47.000000 pinject_design-0.1.93/pinject_design/viz/graph.py
+-rw-r--r--   0        0        0      639 2023-07-12 11:40:58.814948 pinject_design-0.1.93/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pinject_design-0.1.93/PKG-INFO
```

### Comparing `pinject_design-0.1.92/LICENSE` & `pinject_design-0.1.93/LICENSE`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/app_designed.py` & `pinject_design-0.1.93/pinject_design/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/app_injected.py` & `pinject_design-0.1.93/pinject_design/di/app_injected.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from typing import Set
 
 from pinject_design import Injected
 from pinject_design.di.applicative import Applicative
-from pinject_design.di.injected import InjectedPure, InjectedFunction
+from pinject_design.di.injected import InjectedPure, InjectedFunction,InjectedByName
 from pinject_design.di.proxiable import T, DelegatedVar
 from pinject_design.di.static_proxy import eval_app, ast_proxy, \
     AstProxyContextImpl
 from pinject_design.di.ast import Expr, Object, show_expr
 
 
 class ApplicativeInjectedImpl(Applicative[Injected]):
@@ -57,18 +57,20 @@
         case Object(InjectedFunction(func, kwargs)):
             reduced = reduce_injected_expr(Object(kwargs))
             return f"{func.__name__}({reduced})"
         case Object(DelegatedVar() as dv):
             return reduce_injected_expr(Object(dv.eval()))
         case Object(EvaledInjected() as ei):
             return ei.repr_ast()
+        case Object(InjectedByName(name)):
+            return f"$('{name}')"
         case Object(Injected() as i):
             return f"<{i.__class__.__name__}>"
-        case Object(x):
-            return f"???:{type(x)}"
+        # case Object(x):
+        #     return f"Unknown:{x}"
 
 
 def eval_injected(expr: Expr[Injected]) -> EvaledInjected:
     return EvaledInjected(eval_app(expr, ApplicativeInjected), expr)
 
 
 def injected_proxy(injected: Injected) -> DelegatedVar[Injected]:
```

### Comparing `pinject_design-0.1.92/pinject_design/di/applicative.py` & `pinject_design-0.1.93/pinject_design/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/ast.py` & `pinject_design-0.1.93/pinject_design/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/design.py` & `pinject_design-0.1.93/pinject_design/di/design.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,19 +119,22 @@
         d_kwargs = {k: None for k in deleted}
         return f(**called_kwargs, **d_kwargs)
 
     return create_function(sig, impl)
 
 
 def bind_to_injected(bind: Bind):
-    if isinstance(bind, PinjectBind) and "to_class" in bind.kwargs:
-        cls = bind.kwargs["to_class"]
-        return Injected.bind(cls)
-    elif isinstance(bind, InjectedProvider):
-        return bind.src
+    match bind:
+        case PinjectBind(kwargs={"to_class": cls}):
+            return Injected.bind(cls)
+        case InjectedProvider(src):
+            return src
+        case PinjectBind(kwargs={"to_instance": instance}):
+            return Injected.pure(instance)
+
     pb = bind.to_pinject_binding()
     provider = pinject_to_provider(pb)
     provider = remove_kwargs_from_func(provider, ["self"])
     return Injected.bind(provider)
 
 
 # jetbrains://idea/navigate/reference?project=archpainter&path=notes/organized/mac/check_fid_and_generated.ipynb
@@ -229,13 +232,15 @@
 
     def __hash__(self):
         return hash(frozendict(**self.kwargs))
 
     def to_pinject_binding(self) -> Union[PinjectConfigure, PinjectProvider]:
         return PinjectConfigure(self.kwargs)
 
+
 @dataclass
 class MetaBind(Bind):
-    src:Bind
-    metadata:dict
+    src: Bind
+    metadata: dict
+
     def to_pinject_binding(self) -> Union[PinjectConfigure, PinjectProvider]:
         return self.src.to_pinject_binding()
```

### Comparing `pinject_design-0.1.92/pinject_design/di/designed.py` & `pinject_design-0.1.93/pinject_design/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/dynamic_proxy.py` & `pinject_design-0.1.93/pinject_design/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/graph.py` & `pinject_design-0.1.93/pinject_design/di/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,19 @@
         pass
 
     @property
     @abstractmethod
     def design(self):
         pass
 
+    @property
+    @abstractmethod
+    def resolver(self)->"DependencyResolver":
+        pass
+
 
 # using async was not a good Idea since all the function needs to be assumed a coroutine.
 # we don't assume the provider function is a coroutine.
 
 class IScope:
     @abstractmethod
     def provide(self, key, provider_func: Callable[[], Any], trace: List) -> Any:
@@ -212,14 +217,33 @@
         return self.cache[key]
 
     def __contains__(self, item):
         return item in self.cache or item in self.parent
 
 
 @dataclass
+class OverridingScope(IScope):
+    """
+    This class overrides a given scope with a given set of keys.
+    The overriden values will be returned if asked, instead of the original scope.
+    """
+    src: IScope
+    overrides: Dict[str, Any]
+
+    def provide(self, key, provider_func: Callable[[], Any], trace: List) -> Any:
+        if key in self.overrides:
+            return self.overrides[key]
+        else:
+            return self.src.provide(key, provider_func, trace)
+
+    def __contains__(self, item):
+        return item in self.overrides or item in self.src
+
+
+@dataclass
 class DependencyResolver:
     """
     okey I want to make a variant that uses IMPLICIT_BINDINGS when the target is not in the mapping.
     what we need is actually a str->Injected mapping.
     """
     src: "Design"
 
@@ -246,16 +270,20 @@
 
         @lru_cache()
         def _memoized_provider(tgt: str):
             return self.mapping[tgt].get_provider()
 
         self.memoized_provider = _memoized_provider
 
+        predefined = {"__final_target__"}
+
         @lru_cache()
         def _memoized_deps(tgt: str):
+            if tgt in predefined:
+                return []
             if tgt not in self.mapping:
                 raise KeyError(f"target {tgt} is not in the dependency injection mapping.")
             return self.mapping[tgt].dependencies()
 
         self.memoized_deps = _memoized_deps
 
     def _dfs(self, tgt: str, visited: set[str] = None):
@@ -291,21 +319,20 @@
                 return Success({providable: self._dependency_tree(providable)})
             case _:
                 tgt: Injected = self._to_injected(providable)
 
                 return Success({t: self._dependency_tree(t) for t in tgt.dependencies()})
 
     @staticmethod
-    def unresult_tree(tree:Result[Dict[str, Result], Exception])->Dict:
+    def unresult_tree(tree: Result[Dict[str, Result], Exception]) -> Dict:
         if isinstance(tree, Failure):
             return dict(error=tree)
         else:
             return {k: DependencyResolver.unresult_tree(v) for k, v in tree.unwrap().items()}
 
-
     def find_failures(self, tree: Result[Dict[str, Result], Exception]):
         """
         recursively dig into the tree and find all failures
         :param tree:
         :return:
         """
 
@@ -347,14 +374,18 @@
         return res
 
     def provide(self, providable: Providable, scope: IScope):
         # I need to make this based on Threaded Future rather than asyncio
         # because asyncio does not support creating new loop in a thread
         # which means that we cannot use asyncio.run in a cooruntine
         tgt: Injected = self._to_injected(providable)
+        # TODO I want to bind a special key that is only available in this 'provide' scope.
+        scope = OverridingScope(scope, overrides=dict(
+            __final_target__=tgt,
+        ))
 
         def provide_injected(tgt: Injected, key: str):
             assert isinstance(tgt, Injected), f"tgt must be Injected. got {tgt} of type {type(tgt)}"
             assert isinstance(key, str), f"key must be str. got {key} of type {type(key)}"
             provider = tgt.get_provider()
 
             # TODO handle the case where this provider raises an exception
@@ -364,15 +395,15 @@
                 values = [self._provide(d, scope, [key, d]) for d in tgt.dependencies()]
                 kwargs = dict(zip(deps, values))
                 try:
                     return provider(**kwargs)
                 except Exception as e:
                     logger.error(f"failed to provide {key} with {kwargs} \n -> {e}")
                     raise e
-                    #raise RuntimeError(f"failed to provide {key} due to an exception!") from e
+                    # raise RuntimeError(f"failed to provide {key} due to an exception!") from e
                 # I think we need to give a unique name to this injected so that the value will be cached
                 # check if we are in the loop or not
 
             return scope.provide(key, get_result, trace=[key])
 
         match tgt:
             case InjectedByName(key):
@@ -409,15 +440,17 @@
         # one way to prevent this from happening is to use a thread for each provider.
         return res
 
     def child(self, session_provider, overrides: 'Design' = None):
         if overrides is None:
             from pinject_design import Design
             overrides = Design()
-        child_design = self.src + overrides.bind_provider(session=session_provider)
+        child_design = self.src + overrides.bind_provider(
+            session=session_provider
+        )
         child_resolver = DependencyResolver(child_design)
         return child_resolver
 
 
 def run_coroutine_in_new_thread(coroutine):
     # Future to store the result of the coroutine
     future = Future()
@@ -457,32 +490,38 @@
     line_number = caller_info.lineno
 
     return file_name, line_number
 
 
 @dataclass
 class MyObjectGraph(IObjectGraph):
-    resolver: DependencyResolver
+    _resolver: DependencyResolver
     src_design: "Design"
     scope: IScope
 
     def __post_init__(self):
         assert isinstance(self.resolver, DependencyResolver) or self.resolver is None
 
     @property
+    def resolver(self) ->"DependencyResolver":
+        return self._resolver
+
+    @property
     def factory(self) -> IObjectGraphFactory:
         return OGFactoryByDesign(self.src_design)
 
     @staticmethod
     def root(design: "Design") -> "MyObjectGraph":
         scope = MScope()
         graph = MyObjectGraph(None, design, scope)
-        design = design.bind_instance(session=graph)
+        design = design.bind_instance(
+            session=graph
+        )
         resolver = DependencyResolver(design)
-        graph.resolver = resolver
+        graph._resolver = resolver
         return graph
 
     def provide(self, target: Providable, level: int = 2):
         """
         :param target:
         :param level: 2 when you are direcly calling. set increased number to show the callee
         :return:
@@ -516,14 +555,15 @@
         return child_graph
 
     @property
     def design(self):
         return self.src_design
 
 
+
 class ExtendedObjectGraph(IObjectGraph):
     """
     an object graph which can also provide instances based on its name not only from class object.
     TODO I need to change the implementation to not to use pinject, so that I can provide async providers
     """
 
     @property
```

### Comparing `pinject_design-0.1.92/pinject_design/di/injected.py` & `pinject_design-0.1.93/pinject_design/di/injected.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 import functools
 import hashlib
 import inspect
 import sys
 from copy import copy
 from dataclasses import dataclass, field
-from typing import List, Generic, Union, Callable, TypeVar, Tuple, Set, Dict
+from typing import List, Generic, Union, Callable, TypeVar, Tuple, Set, Dict, Any
 
 from makefun import create_function
 
 from pinject_design.di.implicit_globals import IMPLICIT_BINDINGS
 from pinject_design.di.injected_analysis import get_instance_origin
 from pinject_design.di.proxiable import DelegatedVar
 from loguru import logger
@@ -424,14 +424,15 @@
 @dataclass
 class InjectedCache(Injected[T]):
     cache: Injected[Dict]
     program: Injected[T]
     program_dependencies: List[Injected]
 
     def __post_init__(self):
+        self.program = Injected.ensure_injected(self.program)
         def impl(session, cache: Dict, *deps):
             logger.info(f"Checking for cache with deps:{deps}")
             sha256_key = hashlib.sha256(str(deps).encode()).hexdigest()
             hash_key = sha256_key
             if hash_key not in cache:
                 logger.info(f"Cache miss for {deps}")
                 data = session[self.program]
@@ -445,14 +446,16 @@
         self.impl = Injected.list(
             Injected.by_name("session"),
             self.cache,
             *self.program_dependencies
         ).map(
             lambda t: impl(*t)
         )
+        assert isinstance(self.impl, Injected)
+        assert isinstance(self.program, Injected)
 
     def get_provider(self):
         return self.impl.get_provider()
 
     def dependencies(self) -> Set[str]:
         return self.impl.dependencies()
 
@@ -833,7 +836,15 @@
 
 def injected_class(cls):
     return injected_function(cls)
 
 
 def injected(name: str):
     return Injected.by_name(name).proxy
+
+def add_viz_metadata(metadata: Dict[str, Any]):
+    def impl(tgt:Injected):
+        if not hasattr(tgt, '__viz_metadata__'):
+            tgt.__viz_metadata__ = dict()
+        tgt.__viz_metadata__.update(metadata)
+        return tgt
+    return impl
```

### Comparing `pinject_design-0.1.92/pinject_design/di/injected_analysis.py` & `pinject_design-0.1.93/pinject_design/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/permissioned/blueprint.py` & `pinject_design-0.1.93/pinject_design/di/permissioned/blueprint.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/proxiable.py` & `pinject_design-0.1.93/pinject_design/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/session.py` & `pinject_design-0.1.93/pinject_design/di/session.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/sessioned.py` & `pinject_design-0.1.93/pinject_design/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/static_proxy.py` & `pinject_design-0.1.93/pinject_design/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/test_dynamic_proxy.py` & `pinject_design-0.1.93/pinject_design/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/test_graph.py` & `pinject_design-0.1.93/pinject_design/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/test_injected.py` & `pinject_design-0.1.93/pinject_design/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/test_proxiable.py` & `pinject_design-0.1.93/pinject_design/di/test_proxiable.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/di/util.py` & `pinject_design-0.1.93/pinject_design/di/util.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/exceptions.py` & `pinject_design-0.1.93/pinject_design/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/graph_inspection.py` & `pinject_design-0.1.93/pinject_design/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/helper_structure.py` & `pinject_design-0.1.93/pinject_design/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/helpers.py` & `pinject_design-0.1.93/pinject_design/helpers.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/module_inspector.py` & `pinject_design-0.1.93/pinject_design/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/nx_graph_util.py` & `pinject_design-0.1.93/pinject_design/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/run_config_utils.py` & `pinject_design-0.1.93/pinject_design/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/run_config_utils_v2.py` & `pinject_design-0.1.93/pinject_design/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/test_package/__init__.py` & `pinject_design-0.1.93/pinject_design/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.92/pinject_design/visualize_di.py` & `pinject_design-0.1.93/pinject_design/visualize_di.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,15 +94,16 @@
                 return Injected.bind(self.implicit_mappings[src]).dynamic_dependencies()
             elif src in self.pinject_mappings:
                 pp: PinProvider = self.pinject_mappings[src]
                 deps = [d for d in Injected.bind(pp.src).dynamic_dependencies() if
                         d not in pp.non_injectables.value_or([])]
                 return deps
             elif src in self.multi_mappings:
-                return list(set(chain(*[Injected.bind(tgt).dynamic_dependencies() for tgt in self.multi_mappings[src]])))
+                return list(
+                    set(chain(*[Injected.bind(tgt).dynamic_dependencies() for tgt in self.multi_mappings[src]])))
             elif src in self.direct_injected:
                 di = self.direct_injected[src]
                 return self.resolve_injected(di)
             else:
                 raise RuntimeError(f"key not found!:{src}")
 
         self.deps_impl = deps_impl
@@ -276,46 +277,16 @@
                 return ("injected", desc, "mzipped")
             case InjectedByName(name):
                 desc = f"{name}"
                 return ("injected", desc, "by_name")
             case Injected() as injected:
                 desc = f"{injected.__class__.__name__}"
                 return ("injected", desc, str(injected))
-        #
-        # return match(tgt,
-        #              InjectedWithDefaultDesign, lambda iwdd: self.parse_injected(iwdd.src),
-        #              InjectedFunction,
-        #              lambda injected: ("injected",
-        #                                f"Injected:{safe(getattr)(injected.target_function, '__name__').value_or(repr(injected.target_function))}",
-        #                                self.get_source(injected.target_function)),
-        #              InjectedPure,
-        #              lambda injected: (
-        #                  "injected",
-        #                  f"Pure:{injected.value}",
-        #                  self.get_source(injected.value)
-        #                  if isinstance(injected, Callable)
-        #                  else str(injected.value)
-        #              ),
-        #              PartialInjectedFunction,
-        #              lambda injected: ("injected", f"partial=>{injected.src.target_function.__name__}",
-        #                                self.get_source(injected.src.target_function)),
-        #              MappedInjected,
-        #              lambda injected: ("injected", f"{injected.__class__.__name__}", self.get_source(injected.f)),
-        #              ZippedInjected,
-        #              lambda injected: ("injected", f"{injected.__class__.__name__}", "zipped"),
-        #              MZippedInjected,
-        #              lambda injected: ("injected", f"{injected.__class__.__name__}", "mzipped"),
-        #              # IArtifactObject,
-        #              # lambda injected: ("injected", f"artifact:{injected.metadata.identifier}", str(injected)),
-        #              InjectedByName,
-        #              lambda injected: (
-        #                  "injected", f"name:{injected.name}", f"injected by name:{injected.name}"),
-        #              Injected,
-        #              lambda injected: ("injected", f"{injected.__class__.__name__}", str(injected)),
-        #              )
+            case unknown:
+                raise ValueError(f"unknown injected type {unknown}")
 
     def create_dependency_digraph_rooted(self, root: Injected, root_name="__root__",
                                          replace_missing=True
                                          ) -> NxGraphUtil:
         tmp_design = self.src.bind_provider(**{root_name: root})
         return DIGraph(tmp_design) \
             .create_dependency_digraph(
@@ -335,29 +306,35 @@
         self.stylize_graph(nx_graph, replace_missing=replace_missing)
         return NxGraphUtil(nx_graph)
 
     def get_node_to_sl(self, nx_graph, replace_missing):
         @memoize
         def node_to_sl(n):
             def parse(tgt):
-                return match(tgt,
-                             Injected, self.parse_injected,
-                             InjectedProvider(Injected), self.parse_injected,
-                             PinjectProviderBind, lambda ppb: ("function", ppb.f.__name__, self.get_source(ppb.f)),
-                             DirectPinjectProvider,
-                             lambda dpp: ("method", dpp.method.__name__, self.get_source(dpp.method)),
-                             PinjectBind({"to_instance": callable}), lambda i: ("instance", str(i), self.get_source(i)),
-                             PinjectBind({"to_instance": Any}),
-                             lambda i: ("instance", str(i), f"instance:{pformat(i)}"),
-                             PinjectBind({"to_class": Any}), lambda i: ("class", i.__name__, self.get_source(i)),
-                             type, lambda cls: ("class", cls.__name__, self.get_source(cls)),
-                             list, lambda providers: ("multi_binding", repr(providers), repr(providers)),
-                             # MetaBind, lambda mb: (mb.metadata["src"],parse(mb.src)[1],mb.metadata["src"]),
-                             Any, lambda a: ("unknown", str(a), f"unknown-type:{type(a)}=>{a}")
-                             )
+                match tgt:
+                    case Injected():
+                        return self.parse_injected(tgt)
+                    case InjectedProvider(Injected() as _tgt):
+                        return self.parse_injected(_tgt)
+                    case PinjectProviderBind():
+                        return ("function", tgt.f.__name__, self.get_source(tgt.f))
+                    case DirectPinjectProvider():
+                        return ("method", tgt.method.__name__, self.get_source(tgt.method))
+                    case PinjectBind({"to_instance": callable_ob}) if callable(callable_ob):
+                        return ("instance", str(tgt.to_instance), self.get_source(callable_ob))
+                    case PinjectBind({"to_instance": any}):
+                        return ("instance", str(any), f"instance:{pformat(any)}")
+                    case PinjectBind({"to_class": cls}):
+                        return ("class", cls.__name__, self.get_source(cls))
+                    case cls if isinstance(cls, type):
+                        return ("class", cls.__name__, self.get_source(cls))
+                    case [*providers]:
+                        return ("multi_binding", repr(providers), repr(providers))
+                    case _:
+                        return ("unknown", repr(tgt), repr(tgt))
 
             if replace_missing and not is_successful(safe(self.__getitem__)(n)):
                 group, short, long = "missing", f"missing_{n}", f"missing_{n}"
             else:
                 group, short, long = parse(self[n])
             short = str(short).replace("<", "").replace(">", "")[:100]
             n_edges = len(list(nx_graph.neighbors(n))) + safe(self.dependencies_of)(n).map(len).value_or(0)
```

### Comparing `pinject_design-0.1.92/pyproject.toml` & `pinject_design-0.1.93/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinject-design"
-version = "0.1.92"
+version = "0.1.93"
 description = "immutable wrapper for pinject"
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 makefun = "*"
```

### Comparing `pinject_design-0.1.92/PKG-INFO` & `pinject_design-0.1.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinject-design
-Version: 0.1.92
+Version: 0.1.93
 Summary: immutable wrapper for pinject
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

