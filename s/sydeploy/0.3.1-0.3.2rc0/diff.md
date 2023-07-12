# Comparing `tmp/sydeploy-0.3.1-py3-none-any.whl.zip` & `tmp/sydeploy-0.3.2rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,18 @@
-Zip file size: 7541 bytes, number of entries: 18
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-11 12:25 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-11 12:25 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2326 b- defN 23-Jul-11 12:25 sydeploy/commands/authenticate/codeartifact.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     5227 b- defN 23-Jul-11 12:25 sydeploy/commands/build/python_package.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-11 12:25 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      291 b- defN 23-Jul-11 12:25 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:25 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx      807 b- defN 23-Jul-11 12:25 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      282 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1510 b- defN 23-Jul-11 12:25 sydeploy-0.3.1.dist-info/RECORD
-18 files, 12328 bytes uncompressed, 5019 bytes compressed:  59.3%
+Zip file size: 5926 bytes, number of entries: 16
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:39 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 07:39 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 07:39 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:39 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:39 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2813 b- defN 23-Jul-12 07:39 sydeploy/commands/authenticate/aws.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 07:39 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 07:39 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:39 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx     2031 b- defN 23-Jul-12 07:39 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      285 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1333 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/RECORD
+16 files, 8638 bytes uncompressed, 3690 bytes compressed:  57.3%
```

## zipnote {}

```diff
@@ -9,47 +9,41 @@
 
 Filename: sydeploy/commands/__init__.py
 Comment: 
 
 Filename: sydeploy/commands/authenticate/__init__.py
 Comment: 
 
-Filename: sydeploy/commands/authenticate/codeartifact.py
-Comment: 
-
-Filename: sydeploy/commands/build/__init__.py
-Comment: 
-
-Filename: sydeploy/commands/build/python_package.py
+Filename: sydeploy/commands/authenticate/aws.py
 Comment: 
 
 Filename: sydeploy/templates/meta.yaml.dist
 Comment: 
 
 Filename: sydeploy/templates/setup.py.dist
 Comment: 
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.3.1.dist-info/LICENSE
+Filename: sydeploy-0.3.2rc0.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.3.1.dist-info/METADATA
+Filename: sydeploy-0.3.2rc0.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.3.1.dist-info/WHEEL
+Filename: sydeploy-0.3.2rc0.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.3.1.dist-info/entry_points.txt
+Filename: sydeploy-0.3.2rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.3.1.dist-info/top_level.txt
+Filename: sydeploy-0.3.2rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.3.1.dist-info/RECORD
+Filename: sydeploy-0.3.2rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sydeploy/utils/simple.py

```diff
@@ -1,11 +1,13 @@
+import importlib
 from os import getcwd
 from os.path import expanduser, join, exists
 from sydeploy.errors import MissingSCIDCConfig
 from yaml import safe_load
+from inspect import getfullargspec
 
 
 def get_full_path(package_directory: str):
     if package_directory is None:
         return getcwd()
     if package_directory[0] == "~":
         package_directory = expanduser(package_directory)
@@ -18,7 +20,39 @@
     syd_path = join(package_directory, "syd.yaml")
     if not exists(syd_path):
         if not throw_error_on_missing:
             return None
         else:
             raise MissingSCIDCConfig(package_directory)
     return safe_load(open(syd_path, "r"))
+
+
+def run_function_if_valid_variables(function, local_variables: dict, syd_file_contents: dict):
+    if isinstance(function, str):
+        function_name = function.split(".")[-1]
+        function_path = ".".join(function.split(".")[0:-1])
+        try:
+            global_namespace = {}
+            exec(f"from {function_path} import {function_name}", global_namespace)
+            if function_name in global_namespace and callable(global_namespace.get(function_name)):
+                function = global_namespace[function_name]
+        except:
+            raise NotImplementedError(f"The function {function_name} does not exist.")
+    passed_arguments = {}
+    args = getfullargspec(function)
+    if hasattr(args, "args"):
+        args = args.args
+    else:
+        args = []
+    for arg in args:
+        if arg in local_variables:
+            passed_arguments[arg] = local_variables[arg]
+        elif arg in syd_file_contents:
+            passed_arguments[arg] = syd_file_contents[arg]
+
+    if len(passed_arguments) == len(args):
+        return function(**passed_arguments)
+    else:
+        raise f"All arguments {', '.join(args)} are required in the syd.yaml file."
+
+
+
```

## Comparing `sydeploy/commands/authenticate/codeartifact.py` & `sydeploy/commands/authenticate/aws.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,71 @@
+import os.path
 import sys
-import os
-from subprocess import run, check_call
+import shutil
 from impose_cli.decorators import impose
-
-
-def get_index_url():
-    pip = "pip" + str(sys.version_info[0])
-    return run(args=f"{pip} config get global.index-url", shell=True, capture_output=True).stdout.decode("utf-8").strip()
-
-
-def set_index_url(body, extra: bool = False):
-    pip = "pip" + str(sys.version_info[0])
-    index_url = "extra-index-url" if extra else "index-url"
-    check_call([pip, "config", "set", f"global.{index_url}", body])
+from subprocess import run, check_call
 
 
 @impose
-def pip(domain: str = None, repo: str = None, region: str = None):
-    if domain is None or repo is None:
-        raise Exception("A domain and a repo must be defined for CodeArtifact.")
-    region_string = "" if region is None else f"--region {region}"
+def _settings():
+    pass
 
-    account_id = run(args="aws sts get-caller-identity --query 'Account' --output text",
-                     shell=True, capture_output=True).stdout.decode("utf-8").strip()
 
-    res = run(args=f"aws codeartifact get-authorization-token --domain {domain} "
-                   f"--domain-owner {account_id} {region_string} --query  "
+def get_aws_account_id():
+    account_id_exec = run(args="aws sts get-caller-identity --query 'Account' --output text",
+                     shell=True, capture_output=True)
+    errors = account_id_exec.stderr.decode("utf-8").strip()
+    output = account_id_exec.stdout.decode("utf-8").strip()
+    if errors != "":
+        raise Exception(errors)
+    else:
+        return output
+
+
+def get_codeartifact_authentication_token(region: str, domain: str, repo: str):
+    account_id = get_aws_account_id()
+    auth_token_exec = run(args=f"aws codeartifact get-authorization-token --domain {domain} "
+                   f"--domain-owner {account_id} --region {region} --query  "
                    f"authorizationToken --output text", shell=True, capture_output=True)
-    res = res.stdout.decode("utf-8").strip()
+    errors = auth_token_exec.stderr.decode("utf-8").strip()
+    output = auth_token_exec.stdout.decode("utf-8").strip()
+    if errors != "":
+        raise Exception(errors)
+    else:
+        return output, account_id
+
+
+def authenticate_codeartifact_for_pip(region: str, domain: str, repo: str):
+    auth_token, account_id = get_codeartifact_authentication_token(region, domain, repo)
+    new_index_url = f"https://aws:{auth_token}@{domain}-{account_id}.d.codeartifact.{region}.amazonaws.com/pypi/{repo}/simple/"
+    pip = "pip" + str(sys.version[0])
+    check_call([pip, "config", "set", f"global.extra-index-url", new_index_url])
 
-    # By default, AWS CodeArtifact overrides the PIP config file
-    # I assume that this is a bug, but for the meantime, the solution
-    # is to take the remote host, save it temporarily,
-    # let aws replace it, and then switch it
-    new_index_url = f"https://aws:{res}@{domain}-{account_id}.d.codeartifact.{region}.amazonaws.com/pypi/{repo}/simple/"
-    set_index_url(new_index_url, extra=True)
 
-
-@impose
-def twine(domain: str = None, repo: str = None, region: str = None):
-    if domain is None or repo is None or region is None:
-        raise Exception("A domain, repository, and region must be defined for authentication with CodeArtifact.")
-    account_id = run(args="aws sts get-caller-identity --query 'Account' --output text",
-                     shell=True, capture_output=True).stdout.decode("utf-8").strip()
+def authenticate_codeartifact_for_twine(region: str, domain: str, repo: str):
+    account_id = get_aws_account_id()
     # Reauthenticate the KMS for CodeArtifact
-    run(args=f"aws codeartifact login --tool twine --domain {domain} "
+    twine_exec = run(args=f"aws codeartifact login --tool twine --domain {domain} "
              f"--domain-owner {account_id} --region {region} --repository {repo}", shell=True)
-    print("The repository's KMS was refreshed.")
+    output = twine_exec.stdout.decode("utf-8").strip()
+    errors = twine_exec.stderr.decode("utf-8").strip()
+    if errors != "":
+        raise Exception(errors)
+
+    if os.path.exists(os.path.expanduser("~/.pypirc")):
+        print("Writing to a temp file for CI/CD use.")
+        if not os.path.exists("/tmp"):
+            os.mkdir("/tmp")
+        shutil.copy2(os.path.expanduser("~/.pypirc"), "/tmp/.pypirc")
+    return output
+
+
+def authenticate_ecr_for_repo(region: str):
+    account_id = get_aws_account_id()
+    ecr_login_exec = run(args=f"aws ecr get-login-password --region {region} "
+                              f"| docker login --username AWS --password-stdin {account_id}.dkr.ecr.{region}.amazonaws.com")
+    output = ecr_login_exec.stdout.decode("utf-8").strip()
+    errors = ecr_login_exec.stderr.decode("utf-8").strip()
+    if errors != "":
+        raise Exception(errors)
+    else:
+        return output
```

## Comparing `sydeploy-0.3.1.dist-info/LICENSE` & `sydeploy-0.3.2rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.3.1.dist-info/RECORD` & `sydeploy-0.3.2rc0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 sydeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/commands/authenticate/codeartifact.py,sha256=1cILeh4sMS9aeB50Mit2QE5k_6JvVcEOQvuWw0w-sxM,2326
-sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/commands/build/python_package.py,sha256=6YnLodZ6NyrszcbBOcmA9MTDF_h_VxmzttW9kJWkOGE,5227
+sydeploy/commands/authenticate/aws.py,sha256=_rzQx_fvSQwmEZHvZM8SlvLuD78dsy2I1MmRBodLkCU,2813
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=0GlvFdAMVQNftMm3mpJkxhJCNn6vUXc2K9nUWIbNQq4,291
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/utils/simple.py,sha256=fabtM0DAnb9iF28FPIBzAax7isR-aEfTzcWPWyLqBjM,807
-sydeploy-0.3.1.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.3.1.dist-info/METADATA,sha256=nT1gn4PhRztciobbPeaK06BZ6i4A_48RDUYX-xoZYZU,282
-sydeploy-0.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.3.1.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.3.1.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.3.1.dist-info/RECORD,,
+sydeploy/utils/simple.py,sha256=PyKPFVZmqpnS5yXe6j3CO3h5PoIPg_TOqo71qnFIPgo,2031
+sydeploy-0.3.2rc0.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.3.2rc0.dist-info/METADATA,sha256=ze8dildN-uVTRfiex8xByPLOJ7awHVAN9ZHcUomAPy4,285
+sydeploy-0.3.2rc0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.3.2rc0.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.3.2rc0.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.3.2rc0.dist-info/RECORD,,
```

