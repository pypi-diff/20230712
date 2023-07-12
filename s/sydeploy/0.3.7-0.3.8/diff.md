# Comparing `tmp/sydeploy-0.3.7-py3-none-any.whl.zip` & `tmp/sydeploy-0.3.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 8159 bytes, number of entries: 18
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:08 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 09:08 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 09:08 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:08 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:08 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2867 b- defN 23-Jul-12 09:08 sydeploy/commands/authenticate/aws.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:08 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     6747 b- defN 23-Jul-12 09:08 sydeploy/commands/build/python_package.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 09:08 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 09:08 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:08 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx     2014 b- defN 23-Jul-12 09:08 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 09:08 sydeploy-0.3.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      282 b- defN 23-Jul-12 09:08 sydeploy-0.3.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 09:08 sydeploy-0.3.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 09:08 sydeploy-0.3.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 09:08 sydeploy-0.3.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1502 b- defN 23-Jul-12 09:08 sydeploy-0.3.7.dist-info/RECORD
-18 files, 15588 bytes uncompressed, 5655 bytes compressed:  63.7%
+Zip file size: 8151 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:23 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 09:23 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 09:23 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:23 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:23 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Jul-12 09:23 sydeploy/commands/authenticate/aws.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:23 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     6694 b- defN 23-Jul-12 09:23 sydeploy/commands/build/python_package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 09:23 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 09:23 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:23 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx     2014 b- defN 23-Jul-12 09:23 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 09:23 sydeploy-0.3.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      282 b- defN 23-Jul-12 09:23 sydeploy-0.3.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 09:23 sydeploy-0.3.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 09:23 sydeploy-0.3.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 09:23 sydeploy-0.3.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1502 b- defN 23-Jul-12 09:23 sydeploy-0.3.8.dist-info/RECORD
+18 files, 15535 bytes uncompressed, 5647 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.3.7.dist-info/LICENSE
+Filename: sydeploy-0.3.8.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.3.7.dist-info/METADATA
+Filename: sydeploy-0.3.8.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.3.7.dist-info/WHEEL
+Filename: sydeploy-0.3.8.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.3.7.dist-info/entry_points.txt
+Filename: sydeploy-0.3.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.3.7.dist-info/top_level.txt
+Filename: sydeploy-0.3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.3.7.dist-info/RECORD
+Filename: sydeploy-0.3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sydeploy/commands/build/python_package.py

```diff
@@ -30,15 +30,18 @@
 
     cleanup_function = clean_distribution
     if os.path.exists(os.path.join(package_directory, "setup.py")):
         delete_setup = False
     else:
         delete_setup = True
     try:
-        # STEP 1, WE WANT TO AUTHENTICATE
+        # Step1, we clean the last run
+        action = run_function_if_valid_variables(cleanup_function, locals(), syd_contents["meta"])
+
+        # STEP 2, WE WANT TO AUTHENTICATE
         if "registry" not in syd_contents['meta']:
             raise "A registry must be defined for a Python package to be built"
         if syd_contents["meta"]["registry"] not in AUTHENTICATION_MAPPING["build"]:
             raise NotImplementedError(f"Authentication for {syd_contents['meta']} is not currently supported.")
         build_function_name = AUTHENTICATION_MAPPING["build"][syd_contents["meta"]["registry"]]
         action = run_function_if_valid_variables(build_function_name, locals(), syd_contents["meta"])
 
@@ -96,43 +99,40 @@
         else:
             long_description = open(readme_files[0], "r").read()
 
         # Now we get the package_data
         result = [root for root, dirs, files in os.walk(os.path.join(package_directory, identifier)) if not any(file.endswith(".py") for file in files)]
         package_data = {identifier: ["{}/*".format(os.path.basename(x)) for x in result]}
 
-        version_formatted = f'"{version}'
-        long_description_formatted = f"""'{long_description}'"""
-        identifier_formatted = f'"{identifier}"'
         setup_contents = setup_contents.format(
-            name=identifier_formatted,
-            long_description=long_description_formatted,
-            version=version_formatted,
+            name=identifier,
+            long_description=long_description,
+            version=version,
             requirements=json.dumps(main_requirements),
             extra_requires=json.dumps(extra_requires),
             package_data=json.dumps(package_data)
         )
         open(os.path.join(package_directory, "setup.py"), "w").write(setup_contents)
     python_string = "python" + str(sys.version[0])
     print("Building the distribution now.")
     build_exec = run(args=f"{python_string} setup.py bdist_wheel", shell=True, cwd=package_directory, capture_output=True)
-    errors = build_exec.stderr.decode("utf-8").strip()
-    output = build_exec.stdout.decode("utf-8").strip()
-    if errors != "":
-        raise Exception(errors)
+    # Check if it worked
+    if not os.path.exists(os.path.join(package_directory, "dist")):
+        raise "Building the distribution failed."
+
     print("The distribution has been built.")
 
 
 def upload_distribution(package_directory: str, registry: str):
     package_directory = get_full_path(package_directory)
     config_path = "/tmp/.pypirc"
     if not os.path.exists("/tmp/.pypirc"):
         config_path = os.path.expanduser("~/.pypirc")
 
-    upload_exec = run(args=f"twine upload {registry} dist/* --config-file {config_path}", shell=True,
+    upload_exec = run(args=f"twine upload --repository {registry} dist/* --config-file {config_path}", shell=True,
                       capture_output=True, cwd=package_directory)
     errors = upload_exec.stderr.decode("utf-8").strip()
     output = upload_exec.stdout.decode("utf-8").strip()
     if errors != "":
         raise Exception(errors)
     print("Finished uploading to artifact repo.")
```

## Comparing `sydeploy-0.3.7.dist-info/LICENSE` & `sydeploy-0.3.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.3.7.dist-info/RECORD` & `sydeploy-0.3.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 sydeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/aws.py,sha256=C_1ZZz0aRID2nsZF6mtrv0SiFIjJR4SpqQqrdFryO64,2867
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/commands/build/python_package.py,sha256=0y1WCxYfi00f2tQjrlyec8dDgOfYwuortZcnxIu22KQ,6747
+sydeploy/commands/build/python_package.py,sha256=CEjOzwYsSYuJgKelVRhDCt_Didm_trSsBnaBKB59xiU,6694
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=0GlvFdAMVQNftMm3mpJkxhJCNn6vUXc2K9nUWIbNQq4,291
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/utils/simple.py,sha256=zzbHcF2XjYJZntAa3QTmHoLia_ACBPVQTsJtBpPt68Y,2014
-sydeploy-0.3.7.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.3.7.dist-info/METADATA,sha256=8bmVit1lWFvJGz4NhxoYUvzVlSrLbZlhzaltu3kqiTY,282
-sydeploy-0.3.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.3.7.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.3.7.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.3.7.dist-info/RECORD,,
+sydeploy-0.3.8.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.3.8.dist-info/METADATA,sha256=f7dx9h3J897OFgo1tUXsgQuOvKpQYc7ZhHuat6xch28,282
+sydeploy-0.3.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.3.8.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.3.8.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.3.8.dist-info/RECORD,,
```

