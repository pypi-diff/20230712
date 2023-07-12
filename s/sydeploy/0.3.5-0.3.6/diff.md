# Comparing `tmp/sydeploy-0.3.5-py3-none-any.whl.zip` & `tmp/sydeploy-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 8212 bytes, number of entries: 18
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 08:55 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 08:55 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2834 b- defN 23-Jul-12 08:55 sydeploy/commands/authenticate/aws.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     6552 b- defN 23-Jul-12 08:55 sydeploy/commands/build/python_package.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 08:55 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 08:55 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx     2388 b- defN 23-Jul-12 08:55 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      282 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1502 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/RECORD
-18 files, 15734 bytes uncompressed, 5708 bytes compressed:  63.7%
+Zip file size: 8104 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:58 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 08:58 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 08:58 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:58 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:58 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2834 b- defN 23-Jul-12 08:58 sydeploy/commands/authenticate/aws.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:58 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     6552 b- defN 23-Jul-12 08:58 sydeploy/commands/build/python_package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 08:58 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 08:58 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:58 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx     2014 b- defN 23-Jul-12 08:58 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 08:59 sydeploy-0.3.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      282 b- defN 23-Jul-12 08:59 sydeploy-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 08:59 sydeploy-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 08:59 sydeploy-0.3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 08:59 sydeploy-0.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1502 b- defN 23-Jul-12 08:59 sydeploy-0.3.6.dist-info/RECORD
+18 files, 15360 bytes uncompressed, 5600 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.3.5.dist-info/LICENSE
+Filename: sydeploy-0.3.6.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.3.5.dist-info/METADATA
+Filename: sydeploy-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.3.5.dist-info/WHEEL
+Filename: sydeploy-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.3.5.dist-info/entry_points.txt
+Filename: sydeploy-0.3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.3.5.dist-info/top_level.txt
+Filename: sydeploy-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.3.5.dist-info/RECORD
+Filename: sydeploy-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sydeploy/utils/simple.py

```diff
@@ -1,8 +1,7 @@
-import importlib
 from os import getcwd
 from os.path import expanduser, join, exists
 from sydeploy.errors import MissingSCIDCConfig
 from yaml import safe_load
 from inspect import getfullargspec
 
 
@@ -22,34 +21,23 @@
         if not throw_error_on_missing:
             return None
         else:
             raise MissingSCIDCConfig(package_directory)
     return safe_load(open(syd_path, "r"))
 
 
-def safe_import(function_path, function_name):
-    """Imports a function from a module without using exec."""
-    try:
-        module = importlib.import_module(function_path)
-        function = getattr(module, function_name)
-    except ImportError:
-        function = None
-    return function
-
-
 def run_function_if_valid_variables(function, local_variables: dict, syd_file_contents: dict):
     if isinstance(function, str):
         function_name = function.split(".")[-1]
         function_path = ".".join(function.split(".")[0:-1])
         try:
-            # global_namespace = {}
-            # exec(f"from {function_path} import {function_name}", global_namespace)
-            # if function_name in global_namespace and callable(global_namespace.get(function_name)):
-            #     function = global_namespace[function_name]
-            safe_import(function_path, function_name)
+            global_namespace = {}
+            exec(f"from {function_path} import {function_name}", global_namespace)
+            if function_name in global_namespace and callable(global_namespace.get(function_name)):
+                function = global_namespace[function_name]
         except:
             raise NotImplementedError(f"The function {function_name} does not exist.")
     passed_arguments = {}
     args = getfullargspec(function)
     if hasattr(args, "args"):
         args = args.args
     else:
```

## Comparing `sydeploy-0.3.5.dist-info/LICENSE` & `sydeploy-0.3.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.3.5.dist-info/RECORD` & `sydeploy-0.3.6.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/aws.py,sha256=mvg4jSe0C3B54vc74vOqkrLP17jb2cd--NXXUyNVxk8,2834
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/build/python_package.py,sha256=HUMbdUMidmQwpjzC44nrjTyTX5R0r4Vc72EIftSlzVk,6552
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=0GlvFdAMVQNftMm3mpJkxhJCNn6vUXc2K9nUWIbNQq4,291
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/utils/simple.py,sha256=OWzsI3lBLhuCB-Ju4tdYd2SZHmImbgES4qyRCD1bz5g,2388
-sydeploy-0.3.5.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.3.5.dist-info/METADATA,sha256=k0GbrbUP8txBJ6nEV80w0v4ERIrrKsujrp3jyGt18r4,282
-sydeploy-0.3.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.3.5.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.3.5.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.3.5.dist-info/RECORD,,
+sydeploy/utils/simple.py,sha256=zzbHcF2XjYJZntAa3QTmHoLia_ACBPVQTsJtBpPt68Y,2014
+sydeploy-0.3.6.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.3.6.dist-info/METADATA,sha256=u37z5Wp14rBx6JDHEEfss3lP6AaRrvCcRldz64LjfnY,282
+sydeploy-0.3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.3.6.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.3.6.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.3.6.dist-info/RECORD,,
```

