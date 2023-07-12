# Comparing `tmp/sydeploy-0.3.4-py3-none-any.whl.zip` & `tmp/sydeploy-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 8216 bytes, number of entries: 18
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 08:51 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 08:51 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2813 b- defN 23-Jul-12 08:51 sydeploy/commands/authenticate/aws.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     6552 b- defN 23-Jul-12 08:51 sydeploy/commands/build/python_package.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 08:51 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 08:51 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:51 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx     2388 b- defN 23-Jul-12 08:51 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      282 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1502 b- defN 23-Jul-12 08:51 sydeploy-0.3.4.dist-info/RECORD
-18 files, 15713 bytes uncompressed, 5712 bytes compressed:  63.6%
+Zip file size: 8212 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 08:55 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 08:55 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2834 b- defN 23-Jul-12 08:55 sydeploy/commands/authenticate/aws.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     6552 b- defN 23-Jul-12 08:55 sydeploy/commands/build/python_package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 08:55 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 08:55 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 08:55 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx     2388 b- defN 23-Jul-12 08:55 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      282 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1502 b- defN 23-Jul-12 08:55 sydeploy-0.3.5.dist-info/RECORD
+18 files, 15734 bytes uncompressed, 5708 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.3.4.dist-info/LICENSE
+Filename: sydeploy-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.3.4.dist-info/METADATA
+Filename: sydeploy-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.3.4.dist-info/WHEEL
+Filename: sydeploy-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.3.4.dist-info/entry_points.txt
+Filename: sydeploy-0.3.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.3.4.dist-info/top_level.txt
+Filename: sydeploy-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.3.4.dist-info/RECORD
+Filename: sydeploy-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sydeploy/commands/authenticate/aws.py

```diff
@@ -41,15 +41,15 @@
     check_call([pip, "config", "set", f"global.extra-index-url", new_index_url])
 
 
 def authenticate_codeartifact_for_twine(region: str, domain: str, repo: str):
     account_id = get_aws_account_id()
     # Reauthenticate the KMS for CodeArtifact
     twine_exec = run(args=f"aws codeartifact login --tool twine --domain {domain} "
-             f"--domain-owner {account_id} --region {region} --repository {repo}", shell=True)
+             f"--domain-owner {account_id} --region {region} --repository {repo}", shell=True, capture_output=True)
     output = twine_exec.stdout.decode("utf-8").strip()
     errors = twine_exec.stderr.decode("utf-8").strip()
     if errors != "":
         raise Exception(errors)
 
     if os.path.exists(os.path.expanduser("~/.pypirc")):
         print("Writing to a temp file for CI/CD use.")
```

## Comparing `sydeploy-0.3.4.dist-info/LICENSE` & `sydeploy-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.3.4.dist-info/RECORD` & `sydeploy-0.3.5.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 sydeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/commands/authenticate/aws.py,sha256=_rzQx_fvSQwmEZHvZM8SlvLuD78dsy2I1MmRBodLkCU,2813
+sydeploy/commands/authenticate/aws.py,sha256=mvg4jSe0C3B54vc74vOqkrLP17jb2cd--NXXUyNVxk8,2834
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/build/python_package.py,sha256=HUMbdUMidmQwpjzC44nrjTyTX5R0r4Vc72EIftSlzVk,6552
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=0GlvFdAMVQNftMm3mpJkxhJCNn6vUXc2K9nUWIbNQq4,291
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/utils/simple.py,sha256=OWzsI3lBLhuCB-Ju4tdYd2SZHmImbgES4qyRCD1bz5g,2388
-sydeploy-0.3.4.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.3.4.dist-info/METADATA,sha256=uXnJHre467S9Pevy12LRt24zf-x01PJLPYDZzPa7CDk,282
-sydeploy-0.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.3.4.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.3.4.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.3.4.dist-info/RECORD,,
+sydeploy-0.3.5.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.3.5.dist-info/METADATA,sha256=k0GbrbUP8txBJ6nEV80w0v4ERIrrKsujrp3jyGt18r4,282
+sydeploy-0.3.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.3.5.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.3.5.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.3.5.dist-info/RECORD,,
```

