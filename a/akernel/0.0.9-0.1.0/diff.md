# Comparing `tmp/akernel-0.0.9.tar.gz` & `tmp/akernel-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akernel-0.0.9.tar", last modified: Mon Jul 26 06:54:36 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `akernel-0.0.9.tar` & `akernel-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,34 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.725235 akernel-0.0.9/
--rw-rw-r--   0 david     (1000) david     (1000)     1081 2021-05-17 08:49:04.000000 akernel-0.0.9/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       16 2021-05-17 08:49:04.000000 akernel-0.0.9/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     2979 2021-07-26 06:54:36.725235 akernel-0.0.9/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     2020 2021-07-26 06:53:50.000000 akernel-0.0.9/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.725235 akernel-0.0.9/akernel/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.725235 akernel-0.0.9/akernel/IPython/
--rw-rw-r--   0 david     (1000) david     (1000)       49 2021-07-03 21:29:50.000000 akernel-0.0.9/akernel/IPython/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.725235 akernel-0.0.9/akernel/IPython/core/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-07-03 21:29:50.000000 akernel-0.0.9/akernel/IPython/core/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      304 2021-07-25 18:29:32.000000 akernel-0.0.9/akernel/IPython/core/getipython.py
--rw-rw-r--   0 david     (1000) david     (1000)       24 2021-06-17 06:15:57.000000 akernel-0.0.9/akernel/IPython/core/interactiveshell.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-17 05:19:53.000000 akernel-0.0.9/akernel/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)       72 2021-07-26 06:53:03.000000 akernel-0.0.9/akernel/_version.py
--rw-rw-r--   0 david     (1000) david     (1000)      569 2021-06-02 21:05:39.000000 akernel-0.0.9/akernel/akernel.py
--rw-rw-r--   0 david     (1000) david     (1000)     2435 2021-07-25 18:29:32.000000 akernel-0.0.9/akernel/code.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.725235 akernel-0.0.9/akernel/comm/
--rw-rw-r--   0 david     (1000) david     (1000)       72 2021-06-17 20:38:19.000000 akernel-0.0.9/akernel/comm/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4228 2021-07-10 22:06:30.000000 akernel-0.0.9/akernel/comm/comm.py
--rw-rw-r--   0 david     (1000) david     (1000)     1985 2021-07-04 14:05:57.000000 akernel-0.0.9/akernel/comm/manager.py
--rw-rw-r--   0 david     (1000) david     (1000)      680 2021-06-05 17:38:31.000000 akernel-0.0.9/akernel/connect.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.725235 akernel-0.0.9/akernel/display/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-06-16 16:37:26.000000 akernel-0.0.9/akernel/display/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      469 2021-06-29 09:01:30.000000 akernel-0.0.9/akernel/display/display.py
--rw-rw-r--   0 david     (1000) david     (1000)    15464 2021-07-25 18:29:32.000000 akernel-0.0.9/akernel/kernel.py
--rw-rw-r--   0 david     (1000) david     (1000)      516 2021-05-17 09:05:15.000000 akernel-0.0.9/akernel/kernelspec.py
--rw-rw-r--   0 david     (1000) david     (1000)     4145 2021-07-10 22:06:30.000000 akernel-0.0.9/akernel/message.py
--rw-rw-r--   0 david     (1000) david     (1000)     1235 2021-07-25 18:29:32.000000 akernel-0.0.9/akernel/traceback.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.725235 akernel-0.0.9/akernel.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     2979 2021-07-26 06:54:36.000000 akernel-0.0.9/akernel.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      704 2021-07-26 06:54:36.000000 akernel-0.0.9/akernel.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2021-07-26 06:54:36.000000 akernel-0.0.9/akernel.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       49 2021-07-26 06:54:36.000000 akernel-0.0.9/akernel.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)      120 2021-07-26 06:54:36.000000 akernel-0.0.9/akernel.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2021-07-26 06:54:36.000000 akernel-0.0.9/akernel.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2021-07-26 06:54:36.725235 akernel-0.0.9/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1478 2021-07-10 22:09:09.000000 akernel-0.0.9/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.721235 akernel-0.0.9/share/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.721235 akernel-0.0.9/share/jupyter/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.721235 akernel-0.0.9/share/jupyter/kernels/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-26 06:54:36.725235 akernel-0.0.9/share/jupyter/kernels/akernel/
--rw-rw-r--   0 david     (1000) david     (1000)      161 2021-06-03 16:13:13.000000 akernel-0.0.9/share/jupyter/kernels/akernel/kernel.json
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 akernel-0.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 akernel-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/akernel.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/cache.py
+-rw-r--r--   0        0        0     9111 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/code.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/connect.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/execution.py
+-rw-r--r--   0        0        0    17853 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/kernel.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/kernelspec.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/message.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/traceback.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/IPython/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/IPython/core/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/IPython/core/getipython.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/IPython/core/interactiveshell.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/comm/__init__.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/comm/comm.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/comm/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/display/__init__.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/display/display.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/conftest.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/test_async_code.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/test_execution.py
+-rw-r--r--   0        0        0     6748 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/test_kernel.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 akernel-0.1.0/akernel/tests/test_react_code.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 akernel-0.1.0/binder/environment.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 akernel-0.1.0/binder/postBuild
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 akernel-0.1.0/examples/reactivity.ipynb
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 akernel-0.1.0/share/jupyter/kernels/akernel/kernel.json
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 akernel-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 akernel-0.1.0/README.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 akernel-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 akernel-0.1.0/PKG-INFO
```

### Comparing `akernel-0.0.9/LICENSE` & `akernel-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `akernel-0.0.9/akernel/kernel.py` & `akernel-0.1.0/akernel/kernel.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,87 +2,105 @@
 import platform
 import asyncio
 import json
 from io import StringIO
 from contextvars import ContextVar
 from typing import Dict, Any, List, Optional, Union, Awaitable, cast
 
-from zmq.sugar.socket import Socket
+from zmq.asyncio import Socket
 
-from akernel.comm import comm
+import comm  # type: ignore
 from akernel.comm.manager import CommManager
 from akernel.display import display
 import akernel.IPython
 from akernel.IPython import core
 from .connect import connect_channel
 from .message import receive_message, send_message, create_message, check_message
-from .code import make_async
+from .execution import pre_execute, cache_execution
 from .traceback import get_traceback
-from ._version import __version__
+from . import __version__
 
 
-PARENT_HEADER_VAR: ContextVar = ContextVar("parent_header")
+PARENT_VAR: ContextVar = ContextVar("parent")
+IDENTS_VAR: ContextVar = ContextVar("idents")
 
 KERNEL: "Kernel"
 
 
-sys.modules["ipykernel.comm"] = comm
 sys.modules["IPython.display"] = display
 sys.modules["IPython"] = akernel.IPython
 sys.modules["IPython.core"] = core
 
 
 class Kernel:
-
     shell_channel: Socket
     iopub_channel: Socket
     control_channel: Socket
+    stdin_channel: Socket
     connection_cfg: Dict[str, Union[str, int]]
     stop: asyncio.Event
     restart: bool
     key: str
     comm_manager: CommManager
-    kernel_name: str
+    kernel_mode: str
     running_cells: Dict[int, asyncio.Task]
     task_i: int
     execution_count: int
     execution_state: str
-    globals: Dict[str, Any]
-    locals: Dict[str, Any]
+    globals: Dict[str, Dict[str, Any]]
+    locals: Dict[str, Dict[str, Any]]
+    _multi_kernel: Optional[bool]
+    _cache_kernel: Optional[bool]
+    _react_kernel: Optional[bool]
+    kernel_initialized: List[str]
+    cache: Optional[Dict[str, Any]]
 
     def __init__(
         self,
-        kernel_name: str,
+        kernel_mode: str,
+        cache_dir: Optional[str],
         connection_file: str,
     ):
         global KERNEL
         KERNEL = self
         self.comm_manager = CommManager()
+
+        def get_comm_manager():
+            return self.comm_manager
+
+        comm.get_comm_manager = get_comm_manager
         self.loop = asyncio.get_event_loop()
-        self.kernel_name = kernel_name
+        self.kernel_mode = kernel_mode
+        self.cache_dir = cache_dir
+        self._multi_kernel = None
+        self._cache_kernel = None
+        self._react_kernel = None
+        self.kernel_initialized = []
+        self.globals = {}
+        self.locals = {}
         self.running_cells = {}
         self.task_i = 0
         self.execution_count = 1
         self.execution_state = "starting"
-        self.globals = {
-            "asyncio": asyncio,
-            "print": self.print,
-            "__task__": self.task,
-            "_": None,
-        }
-        self.locals = {}
         with open(connection_file) as f:
             self.connection_cfg = json.load(f)
         self.key = cast(str, self.connection_cfg["key"])
         self.restart = False
         self.interrupted = False
         self.msg_cnt = 0
+        if self.cache_kernel:
+            from .cache import cache
+
+            self.cache = cache(cache_dir)
+        else:
+            self.cache = None
         self.shell_channel = connect_channel("shell", self.connection_cfg)
         self.iopub_channel = connect_channel("iopub", self.connection_cfg)
         self.control_channel = connect_channel("control", self.connection_cfg)
+        self.stdin_channel = connect_channel("stdin", self.connection_cfg)
         msg = self.create_message(
             "status", content={"execution_state": self.execution_state}
         )
         send_message(msg, self.iopub_channel, self.key)
         self.execution_state = "idle"
         self.stop = asyncio.Event()
         while True:
@@ -93,14 +111,59 @@
             else:
                 if not self.restart:
                     break
             finally:
                 self.shell_task.cancel()
                 self.control_task.cancel()
 
+    @property
+    def multi_kernel(self):
+        if self._multi_kernel is None:
+            self._multi_kernel = "multi" in self.kernel_mode
+        return self._multi_kernel
+
+    @property
+    def cache_kernel(self):
+        if self._cache_kernel is None:
+            self._cache_kernel = "cache" in self.kernel_mode
+        return self._cache_kernel
+
+    @property
+    def react_kernel(self):
+        if self._react_kernel is None:
+            self._react_kernel = "react" in self.kernel_mode
+        return self._react_kernel
+
+    def init_kernel(self, namespace):
+        if namespace in self.kernel_initialized:
+            return
+
+        self.globals[namespace] = {
+            "ainput": self.ainput,
+            "asyncio": asyncio,
+            "print": self.print,
+            "__task__": self.task,
+            "_": None,
+        }
+        self.locals[namespace] = {}
+        if self.react_kernel:
+            code = (
+                "import ipyx, ipywidgets;"
+                "globals().update({'ipyx': ipyx, 'ipywidgets': ipywidgets})"
+            )
+            exec(code, self.globals[namespace], self.locals[namespace])
+
+        self.kernel_initialized.append(namespace)
+
+    def get_namespace(self, parent_header):
+        if self.multi_kernel:
+            return parent_header["session"]
+
+        return "namespace"
+
     def interrupt(self):
         self.interrupted = True
         for task in self.running_cells.values():
             task.cancel()
         self.running_cells = {}
 
     async def main(self) -> None:
@@ -126,14 +189,15 @@
             if self.interrupted and not await check_message(self.shell_channel):
                 self.interrupted = False
             res = await receive_message(self.shell_channel)
             assert res is not None
             idents, msg = res
             msg_type = msg["header"]["msg_type"]
             parent_header = msg["header"]
+            parent = msg
             if msg_type == "kernel_info_request":
                 msg = self.create_message(
                     "kernel_info_reply",
                     parent_header=parent_header,
                     content={
                         "status": "ok",
                         "protocol_version": "5.5",
@@ -169,35 +233,49 @@
                     continue
                 msg = self.create_message(
                     "execute_input",
                     parent_header=parent_header,
                     content={"code": code, "execution_count": self.execution_count},
                 )
                 send_message(msg, self.iopub_channel, self.key)
-                return_value, async_code = make_async(code)
-                try:
-                    exec(async_code, self.globals, self.locals)
-                except Exception as e:
+                namespace = self.get_namespace(parent_header)
+                self.init_kernel(namespace)
+                traceback, exception, cache_info = pre_execute(
+                    code,
+                    self.globals[namespace],
+                    self.locals[namespace],
+                    self.execution_count,
+                    react=self.react_kernel,
+                    cache=self.cache,
+                )
+                if cache_info["cached"]:
+                    self.finish_execution(
+                        idents,
+                        parent_header,
+                        self.execution_count,
+                        result=cache_info["result"],
+                    )
+                    self.execution_count += 1
+                elif traceback:
                     self.finish_execution(
                         idents,
                         parent_header,
                         self.execution_count,
-                        exception=e,
-                        code=code,
-                        return_value=return_value,
+                        traceback=traceback,
+                        exception=exception,
                     )
                 else:
                     task = asyncio.create_task(
-                        self.execute_code(
+                        self.execute_and_finish(
                             idents,
-                            parent_header,
+                            parent,
                             self.task_i,
                             self.execution_count,
                             code,
-                            return_value,
+                            cache_info,
                         )
                     )
                     self.running_cells[self.task_i] = task
                     self.task_i += 1
                     self.execution_count += 1
             elif msg_type == "comm_info_request":
                 self.execution_state = "busy"
@@ -244,57 +322,41 @@
                 msg = self.create_message(
                     "shutdown_reply",
                     parent_header=parent_header,
                     content={"restart": self.restart},
                 )
                 send_message(msg, self.control_channel, self.key, idents[0])
                 if self.restart:
-                    self.globals = {
-                        "asyncio": asyncio,
-                        "print": self.print,
-                        "__task__": self.task,
-                        "_": None,
-                    }
-                    self.locals = {}
                     self.execution_count = 1
                 self.stop.set()
 
-    async def execute_code(
+    async def execute_and_finish(
         self,
         idents: List[bytes],
-        parent_header: Dict[str, Any],
+        parent: Dict[str, Any],
         task_i: int,
         execution_count: int,
         code: str,
-        return_value: bool,
+        cache_info: Dict[str, Any],
     ) -> None:
-        PARENT_HEADER_VAR.set(parent_header)
-        traceback, exception = None, None
+        PARENT_VAR.set(parent)
+        IDENTS_VAR.set(idents)
+        parent_header = parent["header"]
+        traceback, exception = [], None
+        namespace = self.get_namespace(parent_header)
         try:
-            result = await self.locals["__async_cell__"]()
+            result = await self.locals[namespace]["__async_cell__"]()
         except KeyboardInterrupt:
             self.interrupt()
         except Exception as e:
             exception = e
-            traceback = get_traceback(code, return_value)
+            traceback = get_traceback(code, e, execution_count)
         else:
-            if result is not None:
-                self.globals["_"] = result
-                if getattr(result, "_repr_mimebundle_", None) is not None:
-                    data = result._repr_mimebundle_()
-                    display.display(data, raw=True)
-                elif getattr(result, "_ipython_display_", None) is not None:
-                    result._ipython_display_()
-                else:
-                    msg = self.create_message(
-                        "stream",
-                        parent_header=parent_header,
-                        content={"name": "stdout", "text": f"{repr(result)}\n"},
-                    )
-                    send_message(msg, self.iopub_channel, self.key)
+            self.show_result(result, self.globals[namespace], parent_header)
+            cache_execution(self.cache, cache_info, self.globals[namespace], result)
         finally:
             self.finish_execution(
                 idents,
                 parent_header,
                 execution_count,
                 exception=exception,
                 traceback=traceback,
@@ -305,60 +367,38 @@
     def finish_execution(
         self,
         idents: List[bytes],
         parent_header: Dict[str, Any],
         execution_count: Optional[int],
         exception: Optional[Exception] = None,
         no_exec: bool = False,
-        traceback: Optional[List[str]] = None,
-        code: Optional[str] = None,
-        return_value: bool = False,
+        traceback: List[str] = [],
+        result=None,
     ) -> None:
+        if result:
+            namespace = self.get_namespace(parent_header)
+            self.show_result(result, self.globals[namespace], parent_header)
         if no_exec:
             status = "aborted"
         else:
-            if traceback is None and exception is None:
-                status = "ok"
-            else:
+            if traceback:
                 status = "error"
                 assert exception is not None
-                assert exception.args is not None
-                if type(exception) is SyntaxError:
-                    assert exception.lineno is not None
-                    assert exception.text is not None
-                    assert exception.offset is not None
-                    if exception.filename == "<string>":
-                        assert code is not None
-                        code_lines = code.splitlines()
-                        lineno = exception.lineno - 2
-                        if return_value and lineno == len(code_lines) + 1:
-                            lineno -= 1
-                        text = code_lines[lineno - 1].rstrip()
-                        offset = exception.offset - 5
-                    else:
-                        lineno = exception.lineno
-                        text = exception.text.rstrip()
-                        offset = exception.offset - 1
-                    traceback = [
-                        f"File {exception.filename}, line {lineno}:",
-                        text,
-                        offset * " " + "^",
-                    ]
-                assert traceback is not None
                 msg = create_message(
                     "error",
                     parent_header=parent_header,
                     content={
                         "ename": type(exception).__name__,
                         "evalue": exception.args[0],
-                        "traceback": traceback
-                        + [f"{type(exception).__name__}: {exception.args[0]}"],
+                        "traceback": traceback,
                     },
                 )
                 send_message(msg, self.iopub_channel, self.key)
+            else:
+                status = "ok"
         msg = self.create_message(
             "execute_reply",
             parent_header=parent_header,
             content={"status": status, "execution_count": execution_count},
         )
         send_message(msg, self.shell_channel, self.key, idents[0])
         self.execution_state = "idle"
@@ -374,14 +414,30 @@
             i = self.task_i - 1 + cell_i
         else:
             i = cell_i
         if i in self.running_cells:
             return self.running_cells[i]
         return asyncio.sleep(0)
 
+    async def ainput(self, prompt: str = "") -> Any:
+        parent = PARENT_VAR.get()
+        idents = IDENTS_VAR.get()
+        if parent["content"]["allow_stdin"]:
+            msg = self.create_message(
+                "input_request",
+                parent_header=parent["header"],
+                content={"prompt": prompt, "password": False},
+            )
+            send_message(msg, self.stdin_channel, self.key, idents[0])
+            res = await receive_message(self.stdin_channel)
+            assert res is not None
+            idents, msg = res
+            if msg["content"]["status"] == "ok":
+                return msg["content"]["value"]
+
     def print(
         self,
         *objects,
         sep: str = " ",
         end: str = "\n",
         file=sys.stdout,
         flush: bool = False,
@@ -395,15 +451,15 @@
             return
         f = StringIO()
         print(*objects, sep=sep, end=end, file=f, flush=True)
         text = f.getvalue()
         f.close()
         msg = self.create_message(
             "stream",
-            parent_header=PARENT_HEADER_VAR.get(),
+            parent_header=PARENT_VAR.get()["header"],
             content={"name": name, "text": text},
         )
         send_message(msg, self.iopub_channel, self.key)
 
     def create_message(
         self,
         msg_type: str,
@@ -411,7 +467,32 @@
         parent_header: Dict[str, Any] = {},
     ) -> Dict[str, Any]:
         msg = create_message(
             msg_type, content=content, parent_header=parent_header, msg_cnt=self.msg_cnt
         )
         self.msg_cnt += 1
         return msg
+
+    def show_result(self, result, globals_, parent_header):
+        if result is not None:
+            globals_["_"] = result
+            send_stream = True
+            if getattr(result, "_repr_mimebundle_", None) is not None:
+                try:
+                    data = result._repr_mimebundle_()
+                    display.display(data, raw=True)
+                    send_stream = False
+                except Exception:
+                    pass
+            elif getattr(result, "_ipython_display_", None) is not None:
+                try:
+                    result._ipython_display_()
+                    send_stream = False
+                except Exception:
+                    pass
+            if send_stream:
+                msg = self.create_message(
+                    "stream",
+                    parent_header=parent_header,
+                    content={"name": "stdout", "text": f"{repr(result)}\n"},
+                )
+                send_message(msg, self.iopub_channel, self.key)
```

### Comparing `akernel-0.0.9/akernel/message.py` & `akernel-0.1.0/akernel/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 import hmac
 import hashlib
 from datetime import datetime, timezone
-from typing import List, Dict, Tuple, Any, Optional
+from typing import List, Dict, Tuple, Any, Optional, cast
 
 from zmq.utils import jsonapi
-from zmq.sugar.socket import Socket
+from zmq.asyncio import Socket
 from dateutil.parser import parse as dateutil_parse  # type: ignore
 
 
 protocol_version_info = (5, 3)
 protocol_version = "%i.%i" % protocol_version_info
 
 DELIM = b"<IDS|MSG>"
@@ -108,23 +108,23 @@
     for buf in buffers:
         if isinstance(buf, memoryview):
             view = buf
         else:
             view = memoryview(buf)
         assert view.contiguous
     to_send += buffers
-    return sock.send_multipart(to_send, copy=True)
+    sock.send_multipart(to_send, copy=True)
 
 
 def pack(obj: Dict[str, Any]) -> bytes:
     return jsonapi.dumps(obj)
 
 
 def unpack(s: bytes) -> Dict[str, Any]:
-    return jsonapi.loads(s)
+    return cast(Dict[str, Any], jsonapi.loads(s))
 
 
 def sign(msg_list: List[bytes], key: str) -> bytes:
     auth = hmac.new(key.encode("ascii"), digestmod=hashlib.sha256)
     h = auth.copy()
     for m in msg_list:
         h.update(m)
@@ -146,9 +146,9 @@
     message["parent_header"] = str_to_date(unpack(msg_list[2]))
     message["metadata"] = unpack(msg_list[3])
     message["content"] = unpack(msg_list[4])
     message["buffers"] = [memoryview(b) for b in msg_list[5:]]
     return message
 
 
-async def check_message(sock: Socket) -> bool:
+async def check_message(sock: Socket) -> int:
     return await sock.poll(0)
```

