# Comparing `tmp/pympipool-0.5.1.tar.gz` & `tmp/pympipool-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.5.1.tar", last modified: Mon Jun 26 14:19:55 2023, max compression
+gzip compressed data, was "pympipool-0.5.2.tar", last modified: Wed Jul 12 00:54:24 2023, max compression
```

## Comparing `pympipool-0.5.1.tar` & `pympipool-0.5.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.113378 pympipool-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-26 14:19:49.000000 pympipool-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 14:19:49.000000 pympipool-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-06-26 14:19:55.113378 pympipool-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-26 14:19:49.000000 pympipool-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.113378 pympipool-0.5.1/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-26 14:19:55.113378 pympipool-0.5.1/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.109378 pympipool-0.5.1/pympipool/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/executor/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/executor/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.109378 pympipool-0.5.1/pympipool/share/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.109378 pympipool-0.5.1/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 14:19:55.113378 pympipool-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-26 14:19:54.000000 pympipool-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.113378 pympipool-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-26 14:19:49.000000 pympipool-0.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.716657 pympipool-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-12 00:54:21.000000 pympipool-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 00:54:21.000000 pympipool-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-12 00:54:24.716657 pympipool-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-12 00:54:21.000000 pympipool-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.716657 pympipool-0.5.2/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-12 00:54:24.716657 pympipool-0.5.2/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.712656 pympipool-0.5.2/pympipool/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/executor/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/executor/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.712656 pympipool-0.5.2/pympipool/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.712656 pympipool-0.5.2/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 00:54:24.716657 pympipool-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-12 00:54:24.000000 pympipool-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.716657 pympipool-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-12 00:54:21.000000 pympipool-0.5.2/versioneer.py
```

### Comparing `pympipool-0.5.1/LICENSE` & `pympipool-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/PKG-INFO` & `pympipool-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.1
+Version: 0.5.2
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.1/README.md` & `pympipool-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/pympipool/executor/mpipool.py` & `pympipool-0.5.2/pympipool/executor/mpipool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import pickle
 import sys
 
 import cloudpickle
 
+from pympipool.share.communication import (
+    connect_to_socket_interface,
+    send_result,
+    close_connection,
+    receive_instruction,
+)
 from pympipool.share.parallel import (
-    initialize_zmq,
     parse_arguments,
     parse_socket_communication,
 )
 
 
 def main():
     from mpi4py import MPI
@@ -20,31 +25,32 @@
     )
     from mpi4py.futures import MPIPoolExecutor
 
     future_dict = {}
     argument_dict = parse_arguments(argument_lst=sys.argv)
     with MPIPoolExecutor(int(argument_dict["total_cores"])) as executor:
         if executor is not None:
-            context, socket = initialize_zmq(
+            context, socket = connect_to_socket_interface(
                 host=argument_dict["host"], port=argument_dict["zmqport"]
             )
             while True:
                 output = parse_socket_communication(
                     executor=executor,
-                    input_dict=cloudpickle.loads(socket.recv()),
+                    input_dict=receive_instruction(socket=socket),
                     future_dict=future_dict,
                     cores_per_task=int(argument_dict["cores_per_task"]),
                 )
                 if "exit" in output.keys() and output["exit"]:
                     if "result" in output.keys():
-                        socket.send(cloudpickle.dumps({"result": output["result"]}))
+                        send_result(
+                            socket=socket, result_dict={"result": output["result"]}
+                        )
                     else:
-                        socket.send(cloudpickle.dumps({"result": True}))
-                    socket.close()
-                    context.term()
+                        send_result(socket=socket, result_dict={"result": True})
+                    close_connection(socket=socket, context=context)
                     break
                 elif isinstance(output, dict):
-                    socket.send(cloudpickle.dumps(output))
+                    send_result(socket=socket, result_dict=output)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pympipool-0.5.1/pympipool/share/communication.py` & `pympipool-0.5.2/pympipool/share/communication.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,7 +59,27 @@
         self._process.stdin.close()
         self._process.stderr.close()
         if wait:
             self._process.wait()
 
     def __del__(self):
         self.shutdown(wait=True)
+
+
+def connect_to_socket_interface(host, port):
+    context = zmq.Context()
+    socket = context.socket(zmq.PAIR)
+    socket.connect("tcp://" + host + ":" + port)
+    return context, socket
+
+
+def send_result(socket, result_dict):
+    socket.send(cloudpickle.dumps(result_dict))
+
+
+def receive_instruction(socket):
+    return cloudpickle.loads(socket.recv())
+
+
+def close_connection(socket, context):
+    socket.close()
+    context.term()
```

### Comparing `pympipool-0.5.1/pympipool/share/executor.py` & `pympipool-0.5.2/pympipool/share/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/pympipool/share/parallel.py` & `pympipool-0.5.2/pympipool/share/parallel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-import zmq
 from tqdm import tqdm
 
 
 def parse_arguments(argument_lst):
     argument_dict = {
         "total_cores": "--cores-total",
         "zmqport": "--zmqport",
@@ -17,21 +16,14 @@
             for k, v in argument_dict.items()
             if v in argument_lst
         }
     )
     return parse_dict
 
 
-def initialize_zmq(host, port):
-    context = zmq.Context()
-    socket = context.socket(zmq.PAIR)
-    socket.connect("tcp://" + host + ":" + port)
-    return context, socket
-
-
 def wrap(funct, number_of_cores_per_communicator=1):
     def functwrapped(*args, **kwargs):
         from mpi4py import MPI
 
         MPI.COMM_WORLD.Barrier()
         rank = MPI.COMM_WORLD.Get_rank()
         comm_new = MPI.COMM_WORLD.Split(
```

### Comparing `pympipool-0.5.1/pympipool/share/pool.py` & `pympipool-0.5.2/pympipool/share/pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/pympipool/share/serial.py` & `pympipool-0.5.2/pympipool/share/serial.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/pympipool.egg-info/PKG-INFO` & `pympipool-0.5.2/pympipool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.1
+Version: 0.5.2
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.1/pympipool.egg-info/SOURCES.txt` & `pympipool-0.5.2/pympipool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/setup.py` & `pympipool-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_communicator_split.py` & `pympipool-0.5.2/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_executor.py` & `pympipool-0.5.2/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_future.py` & `pympipool-0.5.2/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_interface.py` & `pympipool-0.5.2/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_multitask.py` & `pympipool-0.5.2/tests/test_multitask.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertEqual(f.result(), np.array(4))
 
     def test_pool_cancel(self):
-        with PoolExecutor(max_workers=2) as p:
+        with PoolExecutor(max_workers=2, sleep_interval=0) as p:
             fs1 = p.submit(sleep_one, i=2)
             fs2 = p.submit(sleep_one, i=2)
             fs3 = p.submit(sleep_one, i=2)
             fs4 = p.submit(sleep_one, i=2)
             sleep(1)
             fs1.cancel()
             fs2.cancel()
```

### Comparing `pympipool-0.5.1/tests/test_parse.py` & `pympipool-0.5.2/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_pool.py` & `pympipool-0.5.2/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_queue.py` & `pympipool-0.5.2/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_task.py` & `pympipool-0.5.2/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_worker.py` & `pympipool-0.5.2/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/tests/test_worker_memory.py` & `pympipool-0.5.2/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.1/versioneer.py` & `pympipool-0.5.2/versioneer.py`

 * *Files identical despite different names*

