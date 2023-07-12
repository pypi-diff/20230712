# Comparing `tmp/hmd_cli_transform_deploy-0.1.55-py3-none-any.whl.zip` & `tmp/hmd_cli_transform_deploy-0.1.56-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7106 bytes, number of entries: 7
--rw-rw-rw-  2.0 unx        0 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy/__init__.py
--rw-rw-rw-  2.0 unx     6704 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy/controller.py
--rw-rw-rw-  2.0 unx    11962 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
--rw-rw-rw-  2.0 unx     2804 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy-0.1.55.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy-0.1.55.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       25 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy-0.1.55.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      665 b- defN 23-Jul-11 14:18 hmd_cli_transform_deploy-0.1.55.dist-info/RECORD
-7 files, 22252 bytes uncompressed, 5900 bytes compressed:  73.5%
+Zip file size: 7150 bytes, number of entries: 7
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jul-12 14:27 hmd_cli_transform_deploy/__init__.py
+-rw-rw-rw-  2.0 unx     6885 b- defN 23-Jul-12 14:27 hmd_cli_transform_deploy/controller.py
+-rw-rw-rw-  2.0 unx    11962 b- defN 23-Jul-12 14:27 hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
+-rw-rw-rw-  2.0 unx     2804 b- defN 23-Jul-12 14:28 hmd_cli_transform_deploy-0.1.56.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Jul-12 14:28 hmd_cli_transform_deploy-0.1.56.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       25 b- defN 23-Jul-12 14:28 hmd_cli_transform_deploy-0.1.56.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      665 b- defN 23-Jul-12 14:28 hmd_cli_transform_deploy-0.1.56.dist-info/RECORD
+7 files, 22433 bytes uncompressed, 5944 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hmd_cli_transform_deploy/controller.py
 Comment: 
 
 Filename: hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.55.dist-info/METADATA
+Filename: hmd_cli_transform_deploy-0.1.56.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.55.dist-info/WHEEL
+Filename: hmd_cli_transform_deploy-0.1.56.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.55.dist-info/top_level.txt
+Filename: hmd_cli_transform_deploy-0.1.56.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.55.dist-info/RECORD
+Filename: hmd_cli_transform_deploy-0.1.56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_transform_deploy/controller.py

```diff
@@ -163,18 +163,22 @@
     )
     def run_transforms(self):
         load_hmd_env(override=False)
         hmd_region = self.app.pargs.hmd_region
         cust_code = self.app.pargs.customer_code
         environment = self.app.pargs.environment
         transform_names = self.app.pargs.transform_names
+        config_file = self.app.pargs.config_file
         run_params = self.app.pargs.run_params
 
         if run_params is not None:
             run_params = json.loads(run_params)
+        elif config_file is not None:
+            with open(config_file, "r") as cf:
+                run_params = json.load(cf)
 
         from .hmd_cli_transform_deploy import run_transforms as do_run_transforms
 
         result = do_run_transforms(
             hmd_region=hmd_region,
             cust_code=cust_code,
             environment=environment,
```

## Comparing `hmd_cli_transform_deploy-0.1.55.dist-info/METADATA` & `hmd_cli_transform_deploy-0.1.56.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-transform-deploy
-Version: 0.1.55
+Version: 0.1.56
 Summary: Command for deploying transforms
 Home-page: UNKNOWN
 Author: Kate Walls
 Author-email: kate.walls@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: acachecontrol (==0.3.5)
```

## Comparing `hmd_cli_transform_deploy-0.1.55.dist-info/RECORD` & `hmd_cli_transform_deploy-0.1.56.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 hmd_cli_transform_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hmd_cli_transform_deploy/controller.py,sha256=4UWXypCi-SOGm9u983yGUrqzvLY0jlk5yN0zSDtFaR8,6704
+hmd_cli_transform_deploy/controller.py,sha256=jbo6dnQcMG6fbDarF_fNzXp0KmIQnZjPun5jFb1EE3k,6885
 hmd_cli_transform_deploy/hmd_cli_transform_deploy.py,sha256=-Qcy3-d1Tq0I_opUl_MEfhe3fBHXdLLkGgno0NuApIw,11962
-hmd_cli_transform_deploy-0.1.55.dist-info/METADATA,sha256=3y4vjjDCvW69Bq8qNhtqaOjdeLetHU9F9KsJPPgGUyk,2804
-hmd_cli_transform_deploy-0.1.55.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
-hmd_cli_transform_deploy-0.1.55.dist-info/top_level.txt,sha256=DtG3sPNzAAQxAwWUR3qMTktl02xogyG5ckfqXQEDusU,25
-hmd_cli_transform_deploy-0.1.55.dist-info/RECORD,,
+hmd_cli_transform_deploy-0.1.56.dist-info/METADATA,sha256=AXmNkRKkHW8shzGRsAJk_5BghM_xV8Fuw6gXuXyy0eE,2804
+hmd_cli_transform_deploy-0.1.56.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
+hmd_cli_transform_deploy-0.1.56.dist-info/top_level.txt,sha256=DtG3sPNzAAQxAwWUR3qMTktl02xogyG5ckfqXQEDusU,25
+hmd_cli_transform_deploy-0.1.56.dist-info/RECORD,,
```

