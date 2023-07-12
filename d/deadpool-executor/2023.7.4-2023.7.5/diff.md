# Comparing `tmp/deadpool_executor-2023.7.4.tar.gz` & `tmp/deadpool_executor-2023.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadpool_executor-2023.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deadpool_executor-2023.7.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deadpool_executor-2023.7.4.tar` & `deadpool_executor-2023.7.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/.coveragerc
--rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.4/LICENSE
--rw-r--r--   0        0        0    22826 2023-07-10 00:05:36.185684 deadpool_executor-2023.7.4/README.rst
--rw-r--r--   0        0        0       86 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/covstart.pth
--rw-r--r--   0        0        0    23912 2023-07-11 09:24:29.569757 deadpool_executor-2023.7.4/deadpool.py
--rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/examples/callbacks.py
--rw-r--r--   0        0        0      751 2023-07-09 23:58:41.948872 deadpool_executor-2023.7.4/examples/entrypoint.py
--rw-r--r--   0        0        0      961 2023-07-11 08:20:11.089233 deadpool_executor-2023.7.4/examples/leftover.py
--rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/examples/priorities.py
--rw-r--r--   0        0        0     1168 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/noxfile.py
--rw-r--r--   0        0        0     1289 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.4/pyproject.toml
--rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/tests/conftest.py
--rw-r--r--   0        0        0    11381 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.4/tests/test_deadpool.py
--rw-r--r--   0        0        0    23905 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.5/.coveragerc
+-rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.5/LICENSE
+-rw-r--r--   0        0        0    23161 2023-07-12 20:43:26.395603 deadpool_executor-2023.7.5/README.rst
+-rw-r--r--   0        0        0       86 2023-07-12 11:42:09.927732 deadpool_executor-2023.7.5/covstart.pth
+-rw-r--r--   0        0        0    24234 2023-07-12 20:43:46.151456 deadpool_executor-2023.7.5/deadpool.py
+-rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.5/examples/callbacks.py
+-rw-r--r--   0        0        0      751 2023-07-09 23:58:41.948872 deadpool_executor-2023.7.5/examples/entrypoint.py
+-rw-r--r--   0        0        0      961 2023-07-12 14:22:32.777642 deadpool_executor-2023.7.5/examples/leftover.py
+-rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.5/examples/priorities.py
+-rw-r--r--   0        0        0     1230 2023-07-12 20:43:26.399603 deadpool_executor-2023.7.5/noxfile.py
+-rw-r--r--   0        0        0     1335 2023-07-12 20:43:26.399603 deadpool_executor-2023.7.5/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.5/tests/conftest.py
+-rw-r--r--   0        0        0    10238 2023-07-12 20:43:26.399603 deadpool_executor-2023.7.5/tests/test_deadpool.py
+-rw-r--r--   0        0        0    24240 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.5/PKG-INFO
```

### Comparing `deadpool_executor-2023.7.4/LICENSE` & `deadpool_executor-2023.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.4/README.rst` & `deadpool_executor-2023.7.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -548,27 +548,42 @@
 
 To run the tests:
 
 .. code-block:: shell
 
    $ nox -s tests
 
+To run tests for a particular version, and say with coverage:
+
+.. code-block:: shell
+
+   $ nox -s testcov-3.11
+
+To pass additional arguments to pytest, use the ``--`` separator:
+
+.. code-block:: shell
+
+   $ nox -s testcov-3.11 -- -k test_deadpool -s <etc>
+
+This is nonstandard above, but I customized the ``noxfile.py`` to
+allow this.
+
 style
 ^^^^^
 
 To apply style fixes, and check for any remaining lints,
 
 .. code-block:: shell
 
    $ nox -t style
 
 docs
 ^^^^
 
-The only docs currently are this README, which uses RST. Github 
+The only docs currently are this README, which uses RST. Github
 uses `docutils <https://docutils.sourceforge.io/docs/ref/rst/directives.html>`_
 to render RST.
 
 release
 ^^^^^^^
 
 This project uses flit to release the package to pypi. The whole
```

### Comparing `deadpool_executor-2023.7.4/deadpool.py` & `deadpool_executor-2023.7.5/deadpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 import pickle
 import signal
 import sys
 import threading
 import traceback
 import typing
 import weakref
+import atexit
 from concurrent.futures import CancelledError, Executor, InvalidStateError, as_completed
 from dataclasses import dataclass, field
 from multiprocessing.connection import Connection
 from queue import Empty, PriorityQueue, Queue, SimpleQueue
 from typing import Callable, Optional, Tuple
 
 import psutil
 
-__version__ = "2023.7.4"
+__version__ = "2023.7.5"
 __all__ = [
     "Deadpool",
     "Future",
     "CancelledError",
     "TimeoutError",
     "ProcessError",
     "PoolClosed",
@@ -79,17 +80,14 @@
         initargs=(),
         finalizer=None,
         finargs=(),
         daemon=True,
         mp_context="forkserver",
         malloc_trim_rss_memory_threshold_bytes=None,
     ):
-        if isinstance(mp_context, str):
-            mp_context = mp.get_context(mp_context)
-
         # For the process to send info OUT OF the process
         conn_receiver, conn_sender = mp.Pipe(duplex=False)
         # For sending work INTO the process
         conn_receiver2, conn_sender2 = mp.Pipe(duplex=False)
         p = mp_context.Process(
             daemon=daemon,
             target=raw_runner2,
@@ -534,23 +532,61 @@
             job = priority_item.item
             *_, fut = job
             fut.cancel()
         except Empty:
             break
 
 
+# Taken from
+# https://psutil.readthedocs.io/en/latest/index.html?highlight=children#kill-process-tree
+def kill_proc_tree(
+    pid,
+    sig=signal.SIGTERM,
+    include_parent=True,
+    timeout=None,
+    on_terminate=None,
+    allow_kill_self=False,
+):  # pragma: no cover
+    """Kill a process tree (including grandchildren) with signal
+    "sig" and return a (gone, still_alive) tuple.
+    "on_terminate", if specified, is a callback function which is
+    called as soon as a child terminates.
+    """
+    if not allow_kill_self and pid == os.getpid():
+        raise ValueError("Won't kill myself")
+
+    try:
+        parent = psutil.Process(pid)
+    except psutil.NoSuchProcess:
+        return
+
+    children = parent.children(recursive=True)
+    if include_parent:
+        children.append(parent)
+
+    for p in children:
+        try:
+            p.send_signal(sig)
+        except psutil.NoSuchProcess:
+            pass
+
+    gone, alive = psutil.wait_procs(children, timeout=timeout, callback=on_terminate)
+    return (gone, alive)
+
+
 def raw_runner2(
     conn: Connection,
     conn_receiver: Connection,
     parent_pid,
     initializer,
     initargs,
     finitializer: Optional[Callable] = None,
     finitargs: Optional[Tuple] = None,
     mem_clear_threshold_bytes: Optional[int] = None,
+    kill_proc_tree=kill_proc_tree,
 ):
     # This event is used to signal that the "parent"
     # monitor thread should be deactivated.
     evt = threading.Event()
 
     def self_destruct_if_parent_disappers():
         """Poll every 5 seconds to see whether the parent is still
@@ -559,16 +595,19 @@
         while True:
             if evt.wait(2.0):
                 return
 
             if not psutil.pid_exists(parent_pid):
                 logger.warning(f"Parent {parent_pid} is gone, self-destructing.")
                 evt.set()
-                kill_proc_tree(pid, sig=signal.SIGKILL, allow_kill_self=True)
-                return
+                atexit._run_exitfuncs()
+                kill_proc_tree(
+                    pid, sig=signal.SIGKILL, allow_kill_self=True
+                )  # pragma: no cover
+                return  # pragma: no cover
 
     tparent = threading.Thread(target=self_destruct_if_parent_disappers, daemon=True)
     tparent.start()
 
     def deactivate_parentless_self_destruct():
         evt.set()
 
@@ -587,34 +626,39 @@
         """Action to fire when the timeout given to ``threading.Timer``
         is reached. It kills this process with SIGKILL."""
         # First things first. Set a self-destruct timer for ourselves.
         # If we don't finish up in time, boom.
         deactivate_parentless_self_destruct()
         conn_send_safe(TimeoutError(f"Process {pid} timed out, self-destructing."))
         # kill_proc_tree_in_process_daemon(pid, signal.SIGKILL)
-        kill_proc_tree(pid, sig=signal.SIGKILL, allow_kill_self=True)
+        atexit._run_exitfuncs()
+        kill_proc_tree(
+            pid, sig=signal.SIGKILL, allow_kill_self=True
+        )  # pragma: no cover
 
     if initializer:
         initargs = initargs or ()
         try:
             initializer(*initargs)
         except Exception:
             logger.exception("Initializer failed")
 
     while True:
         # Wait for some work.
         try:
+            logger.debug("Waiting for work...")
             job = conn_receiver.recv()
+            logger.debug("Got a job")
         except EOFError:
             logger.debug("Received EOF, exiting.")
             break
-        except KeyboardInterrupt:
+        except KeyboardInterrupt:  # pragma: no cover
             logger.debug("Received KeyboardInterrupt, exiting.")
             break
-        except BaseException:
+        except BaseException:  # pragma: no cover
             logger.exception("Received unexpected exception, exiting.")
             break
 
         if job is None:
             logger.debug("Received None, exiting.")
             break
 
@@ -671,56 +715,20 @@
     # to exit, which we don't have. However, we do have a kill
     # switch. Since this process worker will process no more
     # work, and since we've already fun the finalizer, we may
     # as well just nuke it. That will remove its memory space
     # and all its threads too.
     deactivate_parentless_self_destruct()
     logger.debug(f"Deleting worker {pid=}")
-    kill_proc_tree(pid, sig=signal.SIGKILL, allow_kill_self=True)
+    atexit._run_exitfuncs()
+    kill_proc_tree(pid, sig=signal.SIGKILL, allow_kill_self=True)  # pragma: no cover
 
 
 def kill_proc_tree_in_process_daemon(pid, sig):  # pragma: no cover
     mp.Process(target=kill_proc_tree, args=(pid, sig), daemon=True).start()
 
 
-# Taken from
-# https://psutil.readthedocs.io/en/latest/index.html?highlight=children#kill-process-tree
-def kill_proc_tree(
-    pid,
-    sig=signal.SIGTERM,
-    include_parent=True,
-    timeout=None,
-    on_terminate=None,
-    allow_kill_self=False,
-):  # pragma: no cover
-    """Kill a process tree (including grandchildren) with signal
-    "sig" and return a (gone, still_alive) tuple.
-    "on_terminate", if specified, is a callback function which is
-    called as soon as a child terminates.
-    """
-    if not allow_kill_self and pid == os.getpid():
-        raise ValueError("Won't kill myself")
-
-    try:
-        parent = psutil.Process(pid)
-    except psutil.NoSuchProcess:
-        return
-
-    children = parent.children(recursive=True)
-    if include_parent:
-        children.append(parent)
-
-    for p in children:
-        try:
-            p.send_signal(sig)
-        except psutil.NoSuchProcess:
-            pass
-
-    gone, alive = psutil.wait_procs(children, timeout=timeout, callback=on_terminate)
-    return (gone, alive)
-
-
 def trim_memory() -> None:
     """Tell malloc to give all the unused memory back to the OS."""
     if sys.platform == "linux":
         libc = ctypes.CDLL("libc.so.6")
         libc.malloc_trim(0)
```

### Comparing `deadpool_executor-2023.7.4/examples/entrypoint.py` & `deadpool_executor-2023.7.5/examples/entrypoint.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.4/examples/leftover.py` & `deadpool_executor-2023.7.5/examples/leftover.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.4/examples/priorities.py` & `deadpool_executor-2023.7.5/examples/priorities.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.4/noxfile.py` & `deadpool_executor-2023.7.5/noxfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,19 +22,20 @@
         "3.10",
         "3.11",
     ]
 )
 def testcov(session):
     session.install(".")
     session.install("pytest", "pytest-html", "coverage")
+    EXTRA_PYTEST = " ".join(session.posargs)
     session.run(
         *shlex.split(
-            "coverage run --concurrency=multiprocessing,thread "
-            "-m pytest "
-            " --html=report.html --self-contained-html"
+            f"coverage run --concurrency=multiprocessing,thread "
+            f"-m pytest {EXTRA_PYTEST}"
+            f" --html=report.html --self-contained-html"
         )
     )
     session.run(*shlex.split("coverage combine"))
     session.run(*shlex.split("coverage report"))
     session.run(*shlex.split("coverage html"))
```

### Comparing `deadpool_executor-2023.7.4/pyproject.toml` & `deadpool_executor-2023.7.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -48,7 +48,10 @@
 [tool.black]
 include = '\.pyi?$'
 extend-exclude = '''
 (
     ^/venv.*
 )
 '''
+
+[tool.pyright]
+useLibraryCodeForTypes = true
```

### Comparing `deadpool_executor-2023.7.4/tests/test_deadpool.py` & `deadpool_executor-2023.7.5/tests/test_deadpool.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,67 +21,14 @@
 
 
 async def test_func():
     await asyncio.sleep(0.1)
     return 42
 
 
-class TestDeadPool(unittest.TestCase):
-    async def test_acquire(self):
-        async with deadpool.DeadPool(size=2) as pool:
-            fut1 = pool.acquire()
-            fut2 = pool.acquire()
-            await asyncio.sleep(0.1)  # ensure both workers are running
-            self.assertEqual(pool.num_workers(), 2)
-            pool.release(await fut1)
-            pool.release(await fut2)
-        self.assertEqual(pool.num_workers(), 0)
-
-    async def test_concurrent_tasks(self):
-        async with deadpool.DeadPool(size=2) as pool:
-            results = await asyncio.gather(
-                pool.run_in_executor(test_func), pool.run_in_executor(test_func)
-            )
-            self.assertEqual(len(results), 2)
-            self.assertIn(42, results)
-
-    async def test_oversubscription(self):
-        async with deadpool.DeadPool(size=2) as pool:
-            fut1 = pool.acquire()
-            fut2 = pool.acquire()
-            fut3 = pool.acquire()
-            await asyncio.sleep(0.1)  # ensure all workers are running
-            self.assertEqual(pool.num_workers(), 2)
-            pool.release(await fut1)
-            pool.release(await fut2)
-            pool.release(await fut3)
-        self.assertEqual(pool.num_workers(), 0)
-
-    async def test_closed_pool(self):
-        pool = deadpool.DeadPool(size=2)
-        await pool.acquire()
-        await pool.acquire()
-        pool.close()
-        with self.assertRaises(RuntimeError):
-            await pool.acquire()
-
-    async def test_worker_exceptions(self):
-        async def failing_func():
-            await asyncio.sleep(0.1)
-            raise ValueError("failed")
-
-        async with deadpool.DeadPool(size=2) as pool:
-            results = await asyncio.gather(
-                pool.run_in_executor(failing_func), pool.run_in_executor(test_func)
-            )
-            self.assertEqual(len(results), 2)
-            self.assertIn(42, results)
-            self.assertIsInstance(results[0], ValueError)
-
-
 def f():
     return 123
 
 
 def t(duration=10.0):
     time.sleep(duration)
     return duration
@@ -107,18 +54,18 @@
 
 
 @pytest.mark.parametrize("malloc_threshold", [None, 0, 1_000_000])
 def test_simple(malloc_threshold):
     with deadpool.Deadpool(
         malloc_trim_rss_memory_threshold_bytes=malloc_threshold
     ) as exe:
-        fut = exe.submit(t, 0.5)
+        fut = exe.submit(t, 0.05)
         result = fut.result()
 
-    assert result == 0.5
+    assert result == 0.05
 
     # Outside the context manager, no new tasks
     # can be submitted.
     with pytest.raises(deadpool.PoolClosed):
         exe.submit(f)
 
 
@@ -126,14 +73,43 @@
     with deadpool.Deadpool(max_workers=1, initializer=logging_initializer) as exe:
         futs = [exe.submit(t, 0.1) for _ in range(2)]
         results = [fut.result() for fut in futs]
 
     assert results == [0.1] * 2
 
 
+@pytest.mark.parametrize("ctx", ["spawn", "forkserver", "fork"])
+def test_ctx(logging_initializer, ctx):
+    with deadpool.Deadpool(mp_context=ctx, initializer=logging_initializer) as exe:
+        fut = exe.submit(t, 0.05)
+        result = fut.result()
+
+    assert result == 0.05
+
+
+def tsk(*args):
+    return os.getpid()
+
+
+@pytest.mark.parametrize(
+    "max_tasks_per_child,pid_count",
+    [
+        (100, 1),
+        (1, 10),
+    ],
+)
+def test_max_tasks_per_child(logging_initializer, max_tasks_per_child, pid_count):
+    kwargs = dict(max_workers=1, max_tasks_per_child=max_tasks_per_child)
+    with deadpool.Deadpool(initializer=logging_initializer, **kwargs) as exe:
+        futs = [exe.submit(tsk, 0) for _ in range(10)]
+        pids = set(fut.result() for fut in deadpool.as_completed(futs))
+
+    assert len(pids) == pid_count
+
+
 @pytest.mark.parametrize("wait", [True, False])
 @pytest.mark.parametrize("cancel_futures", [True, False])
 def test_shutdown(logging_initializer, wait, cancel_futures):
     with deadpool.Deadpool(
         max_workers=1,
         shutdown_wait=wait,
         shutdown_cancel_futures=cancel_futures,
```

### Comparing `deadpool_executor-2023.7.4/PKG-INFO` & `deadpool_executor-2023.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpool-executor
-Version: 2023.7.4
+Version: 2023.7.5
 Summary: Deadpool
 Author-email: Caleb Hattingh <caleb.hattingh@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
@@ -573,27 +573,42 @@
 
 To run the tests:
 
 .. code-block:: shell
 
    $ nox -s tests
 
+To run tests for a particular version, and say with coverage:
+
+.. code-block:: shell
+
+   $ nox -s testcov-3.11
+
+To pass additional arguments to pytest, use the ``--`` separator:
+
+.. code-block:: shell
+
+   $ nox -s testcov-3.11 -- -k test_deadpool -s <etc>
+
+This is nonstandard above, but I customized the ``noxfile.py`` to
+allow this.
+
 style
 ^^^^^
 
 To apply style fixes, and check for any remaining lints,
 
 .. code-block:: shell
 
    $ nox -t style
 
 docs
 ^^^^
 
-The only docs currently are this README, which uses RST. Github 
+The only docs currently are this README, which uses RST. Github
 uses `docutils <https://docutils.sourceforge.io/docs/ref/rst/directives.html>`_
 to render RST.
 
 release
 ^^^^^^^
 
 This project uses flit to release the package to pypi. The whole
```

