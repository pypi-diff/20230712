# Comparing `tmp/faasmctl-0.3.3.tar.gz` & `tmp/faasmctl-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.3.3.tar", last modified: Tue Jul 11 19:07:07 2023, max compression
+gzip compressed data, was "faasmctl-0.3.4.tar", last modified: Wed Jul 12 10:32:54 2023, max compression
```

## Comparing `faasmctl-0.3.3.tar` & `faasmctl-0.3.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.218190 faasmctl-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-11 19:03:24.000000 faasmctl-0.3.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 19:07:07.218190 faasmctl-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-11 19:03:24.000000 faasmctl-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.214190 faasmctl-0.3.3/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.218190 faasmctl-0.3.3/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.218190 faasmctl-0.3.3/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.218190 faasmctl-0.3.3/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-11 19:06:58.000000 faasmctl-0.3.3/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-11 19:06:58.000000 faasmctl-0.3.3/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 19:03:24.000000 faasmctl-0.3.3/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:07:07.214190 faasmctl-0.3.3/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 19:07:07.000000 faasmctl-0.3.3/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-11 19:03:24.000000 faasmctl-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:07:07.218190 faasmctl-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.481671 faasmctl-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-12 10:29:59.000000 faasmctl-0.3.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-12 10:32:54.481671 faasmctl-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-12 10:29:59.000000 faasmctl-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.473671 faasmctl-0.3.4/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.477671 faasmctl-0.3.4/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.481671 faasmctl-0.3.4/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.481671 faasmctl-0.3.4/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-12 10:32:38.000000 faasmctl-0.3.4/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-12 10:32:38.000000 faasmctl-0.3.4/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.477671 faasmctl-0.3.4/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-12 10:29:59.000000 faasmctl-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:32:54.481671 faasmctl-0.3.4/setup.cfg
```

### Comparing `faasmctl-0.3.3/LICENSE.md` & `faasmctl-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/PKG-INFO` & `faasmctl-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.3
+Version: 0.3.4
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.3
+pip install faasmctl==0.3.4
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.3/README.md` & `faasmctl-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.3
+pip install faasmctl==0.3.4
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.3/faasmctl/tasks/cli.py` & `faasmctl-0.3.4/faasmctl/tasks/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from faasmctl.util.compose import run_compose_cmd
 from faasmctl.util.config import (
     BACKEND_INI_STRING,
     get_faasm_ini_file,
     get_faasm_ini_value,
 )
 from invoke import task
+from os.path import abspath
 
 
 def do_run_cmd(cli, cmd, ini_file):
     if not ini_file:
         ini_file = get_faasm_ini_file()
 
     backend = get_faasm_ini_value(ini_file, "Faasm", BACKEND_INI_STRING)
@@ -19,17 +20,24 @@
             "running on a '{}' backend".format(COMPOSE_BACKEND)
         )
 
     # First, start the container once to avoid recreating it multiple times
     up_cmd = "up -d --no-recreate {}".format(cli)
     run_compose_cmd(ini_file, up_cmd)
 
-    # Second, actually run the requested command
+    # Second, copy the the ini file inside the container
+    ini_file = abspath(ini_file)
+    ini_file_ctr_path = "/tmp/faasm.ini"
+    cp_cmd = "cp {} {}:{}".format(ini_file, cli, ini_file_ctr_path)
+    run_compose_cmd(ini_file, cp_cmd)
+
+    # Lastly, actually run the requested command
     compose_cmd = [
         "exec",
+        "-e FAASM_INI_FILE={}".format(ini_file_ctr_path),
         "-it" if not cmd else "",
         cli,
         "bash" if not cmd else cmd,
     ]
     compose_cmd = " ".join(compose_cmd)
     run_compose_cmd(ini_file, compose_cmd)
```

### Comparing `faasmctl-0.3.3/faasmctl/tasks/delete.py` & `faasmctl-0.3.4/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/tasks/deploy.py` & `faasmctl-0.3.4/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/tasks/flush.py` & `faasmctl-0.3.4/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/tasks/invoke.py` & `faasmctl-0.3.4/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/tasks/logs.py` & `faasmctl-0.3.4/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/tasks/status.py` & `faasmctl-0.3.4/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/compose.py` & `faasmctl-0.3.4/faasmctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/config.py` & `faasmctl-0.3.4/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/deploy.py` & `faasmctl-0.3.4/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/docker.py` & `faasmctl-0.3.4/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/flush.py` & `faasmctl-0.3.4/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.3.4/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.3.4/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/invoke.py` & `faasmctl-0.3.4/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/planner.py` & `faasmctl-0.3.4/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl/util/upload.py` & `faasmctl-0.3.4/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.3.4/faasmctl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.3
+Version: 0.3.4
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.3
+pip install faasmctl==0.3.4
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.3/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.3.4/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.3/pyproject.toml` & `faasmctl-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

