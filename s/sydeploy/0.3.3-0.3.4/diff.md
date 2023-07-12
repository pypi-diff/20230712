# Comparing `tmp/sydeploy-0.3.3-py3-none-any.whl.zip` & `tmp/sydeploy-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 8113 bytes, number of entries: 18
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 07:56 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 07:56 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2813 b- defN 23-Jul-12 07:56 sydeploy/commands/authenticate/aws.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     6552 b- defN 23-Jul-12 07:56 sydeploy/commands/build/python_package.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 07:56 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 07:56 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx     2031 b- defN 23-Jul-12 07:56 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      282 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1502 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/RECORD
-18 files, 15356 bytes uncompressed, 5609 bytes compressed:  63.5%
+Zip file size: 8216 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 08:51 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 08:51 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2813 b- defN 23-Jul-12 08:51 sydeploy/commands/authenticate/aws.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     6552 b- defN 23-Jul-12 08:51 sydeploy/commands/build/python_package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 08:51 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 08:51 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx     2388 b- defN 23-Jul-12 08:51 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      282 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1502 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/RECORD
+18 files, 15713 bytes uncompressed, 5712 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.3.3.dist-info/LICENSE
+Filename: sydeploy-0.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.3.3.dist-info/METADATA
+Filename: sydeploy-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.3.3.dist-info/WHEEL
+Filename: sydeploy-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.3.3.dist-info/entry_points.txt
+Filename: sydeploy-0.3.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.3.3.dist-info/top_level.txt
+Filename: sydeploy-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.3.3.dist-info/RECORD
+Filename: sydeploy-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sydeploy/commands/build/python_package.py

```diff
@@ -7,18 +7,18 @@
 from subprocess import run
 from impose_cli.decorators import impose
 from sydeploy.utils.simple import read_syd_yaml_file, get_full_path, run_function_if_valid_variables
 
 
 AUTHENTICATION_MAPPING = {
     "build": {
-        "codeartifact": "sydeploy.commands2.authenticate.aws.authenticate_codeartifact_for_pip"
+        "codeartifact": "sydeploy.commands.authenticate.aws.authenticate_codeartifact_for_twine"
     },
-    "upload": {
-        "codeartifact": "sydeploy.commands2.authenticate.aws.authenticate_codeartifact_for_twine"
+    "download": {
+        "codeartifact": "sydeploy.commands.authenticate.aws.authenticate_codeartifact_for_pip"
     }
 }
 
 
 @impose
 def _settings():
     pass
@@ -104,15 +104,15 @@
             name=identifier_formatted,
             long_description=long_description_formatted,
             version=version_formatted,
             requirements=json.dumps(main_requirements),
             extra_requires=json.dumps(extra_requires),
             package_data=json.dumps(package_data)
         )
-        open(os.path.join(package_directory, identifier), "w").write(setup_contents)
+        open(os.path.join(package_directory, "setup.py"), "w").write(setup_contents)
     python_string = "python" + str(sys.version[0])
     print("Building the distribution now.")
     build_exec = run(args=f"{python_string} setup.py bdist_wheel", shell=True, cwd=package_directory)
     errors = build_exec.stderr.decode("utf-8").strip()
     output = build_exec.stdout.decode("utf-8").strip()
     if errors != "":
         raise Exception(errors)
```

## sydeploy/utils/simple.py

```diff
@@ -22,23 +22,34 @@
         if not throw_error_on_missing:
             return None
         else:
             raise MissingSCIDCConfig(package_directory)
     return safe_load(open(syd_path, "r"))
 
 
+def safe_import(function_path, function_name):
+    """Imports a function from a module without using exec."""
+    try:
+        module = importlib.import_module(function_path)
+        function = getattr(module, function_name)
+    except ImportError:
+        function = None
+    return function
+
+
 def run_function_if_valid_variables(function, local_variables: dict, syd_file_contents: dict):
     if isinstance(function, str):
         function_name = function.split(".")[-1]
         function_path = ".".join(function.split(".")[0:-1])
         try:
-            global_namespace = {}
-            exec(f"from {function_path} import {function_name}", global_namespace)
-            if function_name in global_namespace and callable(global_namespace.get(function_name)):
-                function = global_namespace[function_name]
+            # global_namespace = {}
+            # exec(f"from {function_path} import {function_name}", global_namespace)
+            # if function_name in global_namespace and callable(global_namespace.get(function_name)):
+            #     function = global_namespace[function_name]
+            safe_import(function_path, function_name)
         except:
             raise NotImplementedError(f"The function {function_name} does not exist.")
     passed_arguments = {}
     args = getfullargspec(function)
     if hasattr(args, "args"):
         args = args.args
     else:
```

## Comparing `sydeploy-0.3.3.dist-info/LICENSE` & `sydeploy-0.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.3.3.dist-info/RECORD` & `sydeploy-0.3.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 sydeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/aws.py,sha256=_rzQx_fvSQwmEZHvZM8SlvLuD78dsy2I1MmRBodLkCU,2813
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/commands/build/python_package.py,sha256=Mhjbl8wAcZXCPTgK6vBuqihgldCns049viPPfhBFXqY,6552
+sydeploy/commands/build/python_package.py,sha256=HUMbdUMidmQwpjzC44nrjTyTX5R0r4Vc72EIftSlzVk,6552
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=0GlvFdAMVQNftMm3mpJkxhJCNn6vUXc2K9nUWIbNQq4,291
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/utils/simple.py,sha256=PyKPFVZmqpnS5yXe6j3CO3h5PoIPg_TOqo71qnFIPgo,2031
-sydeploy-0.3.3.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.3.3.dist-info/METADATA,sha256=5rh8qCSfoOyCQX8bAeu0PLWYuJSdcu0zZrQoVdpBs-0,282
-sydeploy-0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.3.3.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.3.3.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.3.3.dist-info/RECORD,,
+sydeploy/utils/simple.py,sha256=OWzsI3lBLhuCB-Ju4tdYd2SZHmImbgES4qyRCD1bz5g,2388
+sydeploy-0.3.4.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.3.4.dist-info/METADATA,sha256=uXnJHre467S9Pevy12LRt24zf-x01PJLPYDZzPa7CDk,282
+sydeploy-0.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.3.4.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.3.4.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.3.4.dist-info/RECORD,,
```

