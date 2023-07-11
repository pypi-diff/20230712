# Comparing `tmp/motion_python-0.1.79.tar.gz` & `tmp/motion_python-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.79.tar", max compression
+gzip compressed data, was "motion_python-0.1.80.tar", max compression
```

## Comparing `motion_python-0.1.79.tar` & `motion_python-0.1.80.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3344 2023-07-08 00:46:41.015336 motion_python-0.1.79/README.md
--rw-r--r--   0        0        0      344 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/cli.py
--rw-r--r--   0        0        0    23355 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/component.py
--rw-r--r--   0        0        0     4623 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/dicts.py
--rw-r--r--   0        0        0    17213 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/execute.py
--rw-r--r--   0        0        0    13900 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/instance.py
--rw-r--r--   0        0        0     4882 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1153 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/route.py
--rw-r--r--   0        0        0     4953 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/server/update_task.py
--rw-r--r--   0        0        0     8661 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-07-08 00:47:00.723385 motion_python-0.1.79/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.79/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-11 22:32:47.862080 motion_python-0.1.80/README.md
+-rw-r--r--   0        0        0      344 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/cli.py
+-rw-r--r--   0        0        0    23989 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/component.py
+-rw-r--r--   0        0        0     4623 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/dicts.py
+-rw-r--r--   0        0        0    17368 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/execute.py
+-rw-r--r--   0        0        0    13507 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/instance.py
+-rw-r--r--   0        0        0     4882 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1153 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/route.py
+-rw-r--r--   0        0        0     4953 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/server/update_task.py
+-rw-r--r--   0        0        0     8661 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-07-11 22:33:13.239630 motion_python-0.1.80/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.80/PKG-INFO
```

### Comparing `motion_python-0.1.79/README.md` & `motion_python-0.1.80/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.79/motion/cli.py` & `motion_python-0.1.80/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.79/motion/component.py` & `motion_python-0.1.80/motion/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from motion.dicts import Params
 from motion.instance import ComponentInstance
 from motion.route import Route
-from motion.utils import random_passphrase, validate_args
+from motion.utils import DEFAULT_KEY_TTL, random_passphrase, validate_args
 
 
 class Component:
     """Component class for creating Motion components.
     Here are some examples:
 
     === "Basic"
@@ -111,36 +111,55 @@
         if __name__ == "__main__":
             c = MLMonitor() # Create instance
             c.run("predict", props={"features": YOUR_FEATURES_HERE})
             # Some alert may be fired in the background!
         ```
     """
 
-    def __init__(self, name: str, params: Dict[str, Any] = {}):
+    def __init__(
+        self,
+        name: str,
+        params: Dict[str, Any] = {},
+        cache_ttl: int = DEFAULT_KEY_TTL,
+    ):
         """Creates a new Motion component.
 
         Args:
             name (str):
                 Name of the component.
-                params (Dict[str, Any], optional):
-                    Parameters to be accessed by the component. Defaults to {}.
-                    Usage: `C.params["param_name"]` if C is the Component you
-                    have created.
+            params (Dict[str, Any], optional):
+                Parameters to be accessed by the component. Defaults to {}.
+                Usage: `C.params["param_name"]` if C is the Component you
+                have created.
+            cache_ttl (int, optional):
+                Time to live for cached serve results (seconds).
+                Defaults to 1 day. Set to 0 to disable caching.
         """
+        if cache_ttl is None or cache_ttl < 0:
+            raise ValueError(
+                "cache_ttl must be 0 (caching disabled) or a positive integer."
+            )
+
         self._name = name
         self._params = Params(params)
+        self._cache_ttl = cache_ttl
 
         # Set up routes
         self._serve_routes: Dict[str, Route] = {}
         self._update_routes: Dict[str, List[Route]] = {}
         self._init_state_func: Optional[Callable] = None
         self._save_state_func: Optional[Callable] = None
         self._load_state_func: Optional[Callable] = None
 
     @property
+    def cache_ttl(self) -> int:
+        """Time to live for cached serve results (seconds)."""
+        return self._cache_ttl
+
+    @property
     def name(self) -> str:
         """Name of the component.
 
         Example Usage:
         ```python
         from motion import Component
 
@@ -513,14 +532,15 @@
                 init_state_params=init_state_params,
                 save_state_func=self._save_state_func,
                 load_state_func=self._load_state_func,
                 serve_routes=self._serve_routes,
                 update_routes=self._update_routes,
                 logging_level=logging_level,
                 disabled=disabled,
+                cache_ttl=self._cache_ttl,
             )
         except RuntimeError:
             raise RuntimeError(
                 "Error creating component instance. Make sure the entry point "
                 + "of your program is protected, using `if __name__ == '__main__':`"
             )
```

### Comparing `motion_python-0.1.79/motion/dicts.py` & `motion_python-0.1.80/motion/dicts.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.79/motion/execute.py` & `motion_python-0.1.80/motion/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,23 +23,25 @@
 )
 
 
 class Executor:
     def __init__(
         self,
         instance_name: str,
+        cache_ttl: int,
         init_state_func: Optional[Callable],
         init_state_params: Dict[str, Any],
         save_state_func: Optional[Callable],
         load_state_func: Optional[Callable],
         serve_routes: Dict[str, Route],
         update_routes: Dict[str, List[Route]],
         disabled: bool = False,
     ):
         self._instance_name = instance_name
+        self._cache_ttl = cache_ttl
 
         self._init_state_func = init_state_func
         self._init_state_params = init_state_params
         self._load_state_func = load_state_func
         self._save_state_func = save_state_func
 
         self.running: Any = multiprocessing.Value("b", False)
@@ -324,14 +326,18 @@
             if not v:
                 raise ValueError(
                     f"Error loading state for {self._instance_name}."
                     + " No version found."
                 )
             self.version = int(v)
 
+        # If caching is disabled, return
+        if self._cache_ttl == 0:
+            return route_run, serve_result, props, None
+
         # Try hashing the value
         try:
             value_hash = hash_object(props)
         except TypeError:
             value_hash = None
 
         # Check if key is in cache if value can be hashed and
@@ -345,15 +351,14 @@
 
         return route_run, serve_result, props, value_hash
 
     def run(
         self,
         key: str,
         props: Dict[str, Any],
-        cache_ttl: int,
         ignore_cache: bool,
         force_refresh: bool,
         flush_update: bool,
     ) -> Any:
         route_hit = False
         serve_result = None
         props = Properties(props)
@@ -387,15 +392,15 @@
                 if value_hash:
                     cache_result_key = (
                         f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
                     )
                     self._redis_con.set(
                         cache_result_key,
                         cloudpickle.dumps(props),
-                        ex=cache_ttl,
+                        ex=self._cache_ttl,
                     )
 
         # Run the update routes
         # Enqueue results into update queues
         route_hit = self._enqueue_and_trigger_update(
             key, props, flush_update, route_hit
         )
@@ -405,15 +410,14 @@
 
         return serve_result
 
     async def arun(
         self,
         key: str,
         props: Dict[str, Any],
-        cache_ttl: int,
         ignore_cache: bool,
         force_refresh: bool,
         flush_update: bool,
     ) -> Any:
         route_hit = False
         serve_result = None
         props = Properties(props)
@@ -447,15 +451,15 @@
                 if value_hash:
                     cache_result_key = (
                         f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
                     )
                     self._redis_con.set(
                         cache_result_key,
                         cloudpickle.dumps(props),
-                        ex=cache_ttl,
+                        ex=self._cache_ttl,
                     )
 
         # Run the update routes
         # Enqueue results into update queues
         route_hit = self._enqueue_and_trigger_update(
             key, props, flush_update, route_hit
         )
```

### Comparing `motion_python-0.1.79/motion/instance.py` & `motion_python-0.1.80/motion/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         init_state_params: Optional[Dict[str, Any]],
         save_state_func: Optional[Callable],
         load_state_func: Optional[Callable],
         serve_routes: Dict[str, Route],
         update_routes: Dict[str, List[Route]],
         logging_level: str = "WARNING",
         disabled: bool = False,
+        cache_ttl: int = DEFAULT_KEY_TTL,
     ):
         """Creates a new instance of a Motion component.
 
         Args:
             component_name (str):
                 Name of the component we are creating an instance of.
             instance_id (str):
@@ -48,19 +49,21 @@
         # self._serverless = serverless
         # indicator = "serverless" if serverless else "local"
         logger.info(f"Creating local instance of {self._component_name}...")
         atexit.register(self.shutdown)
 
         # Create instance name
         self._instance_name = f"{self._component_name}__{instance_id}"
+        self._cache_ttl = cache_ttl
 
         self.running = False
         self.disabled = disabled
         self._executor = Executor(
             self._instance_name,
+            cache_ttl=self._cache_ttl,
             init_state_func=init_state_func,
             init_state_params=init_state_params if init_state_params else {},
             save_state_func=save_state_func,
             load_state_func=load_state_func,
             serve_routes=serve_routes,
             update_routes=update_routes,
             disabled=self.disabled,
@@ -257,15 +260,14 @@
         self._executor.flush_update(dataflow_key)
 
     def run(
         self,
         # *,
         dataflow_key: str,
         props: Dict[str, Any] = {},
-        cache_ttl: int = DEFAULT_KEY_TTL,
         ignore_cache: bool = False,
         force_refresh: bool = False,
         flush_update: bool = False,
     ) -> Any:
         """Runs the dataflow (serve and update ops) for the keyword argument
         passed in. If the key is not found to have any ops, an error
         is raised. Only one dataflow key should be passed in.
@@ -306,60 +308,55 @@
         ```
 
 
         Args:
             dataflow_key (str): Key of the dataflow to run.
             props (Dict[str, Any]): Keyword arguments to pass into the
                 dataflow ops, in addition to the state.
-            cache_ttl (int, optional):
-                How long the serveence result should live in a cache (in
-                seconds). Defaults to 1 day (60 * 60 * 24).
             ignore_cache (bool, optional):
                 If True, ignores the cache and runs the serve op. Does not
                 force refresh the state. Defaults to False.
             force_refresh (bool, optional): Read the latest value of the
-                state before running an serveence call, otherwise a stale
+                state before running an serve call, otherwise a stale
                 version of the state or a cached result may be used.
                 Defaults to False.
             flush_update (bool, optional):
                 If True, waits for the update op to finish executing before
                 returning. If the update queue hasn't reached batch_size
                 yet, the update op runs anyways. Force refreshes the
                 state after the update op completes. Defaults to False.
 
          Raises:
             ValueError: If more than one dataflow key-value pair is passed.
             RuntimeError:
                 If the component instance was initialized as disabled.
 
         Returns:
-            Any: Result of the serveence call. Might take a long time
+            Any: Result of the serve call. Might take a long time
             to run if `flush_update = True` and the update operation is
             computationally expensive.
         """
         if self.disabled:
             raise RuntimeError("Cannot run a disabled component instance.")
 
         serve_result = self._executor.run(
             key=dataflow_key,
             props=props,
-            cache_ttl=cache_ttl,
             ignore_cache=ignore_cache,
             force_refresh=force_refresh,
             flush_update=flush_update,
         )
 
         return serve_result
 
     async def arun(
         self,
         # *,
         dataflow_key: str,
         props: Dict[str, Any] = {},
-        cache_ttl: int = DEFAULT_KEY_TTL,
         ignore_cache: bool = False,
         force_refresh: bool = False,
         flush_update: bool = False,
     ) -> Awaitable[Any]:
         """Async version of run. Runs the dataflow (serve and update ops) for the
         specified key.
 
@@ -383,45 +380,41 @@
             asyncio.run(main())
         ```
 
         Args:
             dataflow_key (str): Key of the dataflow to run.
             props (Dict[str, Any]): Keyword arguments to pass into the
                 dataflow ops, in addition to the state.
-            cache_ttl (int, optional):
-                How long the serveence result should live in a cache (in
-                seconds). Defaults to 1 day (60 * 60 * 24).
             ignore_cache (bool, optional):
                 If True, ignores the cache and runs the serve op. Does not
                 force refresh the state. Defaults to False.
             force_refresh (bool, optional): Read the latest value of the
-                state before running an serveence call, otherwise a stale
+                state before running an serve call, otherwise a stale
                 version of the state or a cached result may be used.
                 Defaults to False.
             flush_update (bool, optional):
                 If True, waits for the update op to finish executing before
                 returning. If the update queue hasn't reached batch_size
                 yet, the update op runs anyways. Force refreshes the
                 state after the update op completes. Defaults to False.
 
         Raises:
             ValueError: If more than one dataflow key-value pair is passed.
             RuntimeError:
                 If the component instance was initialized as disabled.
 
         Returns:
-            Awaitable[Any]: Awaitable Result of the serveence call.
+            Awaitable[Any]: Awaitable Result of the serve call.
         """
         if self.disabled:
             raise RuntimeError("Cannot run a disabled component instance.")
 
         serve_result = await self._executor.arun(
             key=dataflow_key,
             props=props,
             # value=value,
-            cache_ttl=cache_ttl,
             ignore_cache=ignore_cache,
             force_refresh=force_refresh,
             flush_update=flush_update,
         )  # type: ignore
 
         return serve_result  # type: ignore
```

### Comparing `motion_python-0.1.79/motion/migrate.py` & `motion_python-0.1.80/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.79/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.80/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.79/motion/route.py` & `motion_python-0.1.80/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.79/motion/server/update_task.py` & `motion_python-0.1.80/motion/server/update_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.79/motion/utils.py` & `motion_python-0.1.80/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.79/pyproject.toml` & `motion_python-0.1.80/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.79"
+version = "0.1.80"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.79/PKG-INFO` & `motion_python-0.1.80/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.79
+Version: 0.1.80
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

