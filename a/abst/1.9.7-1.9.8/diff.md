# Comparing `tmp/abst-1.9.7.tar.gz` & `tmp/abst-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abst-1.9.7.tar", last modified: Fri May 26 12:50:25 2023, max compression
+gzip compressed data, was "abst-1.9.8.tar", last modified: Wed Jul 12 12:16:20 2023, max compression
```

## Comparing `abst-1.9.7.tar` & `abst-1.9.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 12:50:14.000000 abst-1.9.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-26 12:50:25.687347 abst-1.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-26 12:50:14.000000 abst-1.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/abst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:14.000000 abst-1.9.7/abst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-26 12:50:14.000000 abst-1.9.7/abst/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/abst/bastion_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:14.000000 abst-1.9.7/abst/bastion_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-26 12:50:14.000000 abst-1.9.7/abst/bastion_support/bastion_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22747 2023-05-26 12:50:14.000000 abst-1.9.7/abst/bastion_support/oci_bastion.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-26 12:50:14.000000 abst-1.9.7/abst/cfg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-26 12:50:14.000000 abst-1.9.7/abst/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-26 12:50:14.000000 abst-1.9.7/abst/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-05-26 12:50:14.000000 abst-1.9.7/abst/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/abst/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:14.000000 abst-1.9.7/abst/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-26 12:50:14.000000 abst-1.9.7/abst/notifier/version_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-26 12:50:14.000000 abst-1.9.7/abst/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 12:50:14.000000 abst-1.9.7/abst/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/abst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:50:25.687347 abst-1.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 12:50:14.000000 abst-1.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 12:50:14.000000 abst-1.9.7/tests/test_sample_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.750786 abst-1.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 12:16:10.000000 abst-1.9.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-12 12:16:20.750786 abst-1.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-12 12:16:10.000000 abst-1.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.742786 abst-1.9.8/abst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:10.000000 abst-1.9.8/abst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-12 12:16:10.000000 abst-1.9.8/abst/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.746786 abst-1.9.8/abst/bastion_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:10.000000 abst-1.9.8/abst/bastion_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-12 12:16:10.000000 abst-1.9.8/abst/bastion_support/bastion_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22990 2023-07-12 12:16:10.000000 abst-1.9.8/abst/bastion_support/oci_bastion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-12 12:16:10.000000 abst-1.9.8/abst/cfg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-12 12:16:10.000000 abst-1.9.8/abst/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-12 12:16:10.000000 abst-1.9.8/abst/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-07-12 12:16:10.000000 abst-1.9.8/abst/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.746786 abst-1.9.8/abst/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:10.000000 abst-1.9.8/abst/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-12 12:16:10.000000 abst-1.9.8/abst/notifier/version_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-12 12:16:10.000000 abst-1.9.8/abst/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-12 12:16:10.000000 abst-1.9.8/abst/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.746786 abst-1.9.8/abst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:16:20.000000 abst-1.9.8/abst.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:16:20.750786 abst-1.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-12 12:16:10.000000 abst-1.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:16:20.750786 abst-1.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-12 12:16:10.000000 abst-1.9.8/tests/test_sample_dict.py
```

### Comparing `abst-1.9.7/LICENSE.md` & `abst-1.9.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/PKG-INFO` & `abst-1.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.7
+Version: 1.9.8
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.7/README.md` & `abst-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/abst/bastion_support/bastion_scheduler.py` & `abst-1.9.8/abst/bastion_support/bastion_scheduler.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/abst/bastion_support/oci_bastion.py` & `abst-1.9.8/abst/bastion_support/oci_bastion.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         self.current_status = "creating bastion session"
         try:
             res = self.create_bastion_ssh_session_managed(creds)
         except subprocess.CalledProcessError as ex:
             logging.debug(f"Exception {ex}")
             rich.print(f"[red]Invalid Config in abst {self.get_print_name()}[/red]")
             exit(1)
-            return  # Just for Pycharm
 
         bid, response = self.load_response(res)
 
         if bid is None:
             rich.print(
                 f"Failed to Create Bastion {self.get_print_name()} with response"
                 f" '{response}'")
@@ -469,17 +468,23 @@
 
         :param ssh_tunnel_arg_str: String for ssh tunnel creation
         :param shell: If you use shell environment (can have different impacts on MAC and
          LINUX)
         :return:
         """
         args_split = self.process_args(already_split, shell, ssh_tunnel_arg_str)
+        try:
+            p = subprocess.Popen(args_split, stdout=subprocess.PIPE,
+                                 stderr=subprocess.STDOUT, shell=shell)
+        except FileNotFoundError:
+            self.connected = False
+            rich.print("Failed to establish SSH tunnel due to different setting os shell terminal, [red]try to run "
+                       "again with --shell[/red]")
+            return True
 
-        p = subprocess.Popen(args_split, stdout=subprocess.PIPE,
-                             stderr=subprocess.STDOUT, shell=shell)
         self.active_tunnel = p
         tries = 3
         while p.poll() is None and tries >= 0:
             line = p.stdout.readline().decode("utf-8").strip()
             line_err = None
 
             if p.stderr:
```

### Comparing `abst-1.9.7/abst/cfg_func.py` & `abst-1.9.8/abst/cfg_func.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/abst/config.py` & `abst-1.9.8/abst/config.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/abst/dialogs.py` & `abst-1.9.8/abst/dialogs.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/abst/main.py` & `abst-1.9.8/abst/main.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/abst/notifier/version_notifier.py` & `abst-1.9.8/abst/notifier/version_notifier.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/abst/tools.py` & `abst-1.9.8/abst/tools.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/abst/wrappers.py` & `abst-1.9.8/abst/wrappers.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/abst.egg-info/PKG-INFO` & `abst-1.9.8/abst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.7
+Version: 1.9.8
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.7/abst.egg-info/SOURCES.txt` & `abst-1.9.8/abst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abst-1.9.7/setup.py` & `abst-1.9.8/setup.py`

 * *Files identical despite different names*

