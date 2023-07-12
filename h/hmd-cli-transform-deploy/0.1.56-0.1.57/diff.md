# Comparing `tmp/hmd_cli_transform_deploy-0.1.56-py3-none-any.whl.zip` & `tmp/hmd_cli_transform_deploy-0.1.57-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7150 bytes, number of entries: 7
--rw-rw-rw-  2.0 unx        0 b- defN 23-Jul-12 14:27 hmd_cli_transform_deploy/__init__.py
--rw-rw-rw-  2.0 unx     6885 b- defN 23-Jul-12 14:27 hmd_cli_transform_deploy/controller.py
--rw-rw-rw-  2.0 unx    11962 b- defN 23-Jul-12 14:27 hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
--rw-rw-rw-  2.0 unx     2804 b- defN 23-Jul-12 14:28 hmd_cli_transform_deploy-0.1.56.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Jul-12 14:28 hmd_cli_transform_deploy-0.1.56.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       25 b- defN 23-Jul-12 14:28 hmd_cli_transform_deploy-0.1.56.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      665 b- defN 23-Jul-12 14:28 hmd_cli_transform_deploy-0.1.56.dist-info/RECORD
-7 files, 22433 bytes uncompressed, 5944 bytes compressed:  73.5%
+Zip file size: 7163 bytes, number of entries: 7
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jul-12 19:01 hmd_cli_transform_deploy/__init__.py
+-rw-rw-rw-  2.0 unx     6885 b- defN 23-Jul-12 19:01 hmd_cli_transform_deploy/controller.py
+-rw-rw-rw-  2.0 unx    11993 b- defN 23-Jul-12 19:01 hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
+-rw-rw-rw-  2.0 unx     2804 b- defN 23-Jul-12 19:01 hmd_cli_transform_deploy-0.1.57.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Jul-12 19:01 hmd_cli_transform_deploy-0.1.57.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       25 b- defN 23-Jul-12 19:01 hmd_cli_transform_deploy-0.1.57.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      665 b- defN 23-Jul-12 19:01 hmd_cli_transform_deploy-0.1.57.dist-info/RECORD
+7 files, 22464 bytes uncompressed, 5957 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hmd_cli_transform_deploy/controller.py
 Comment: 
 
 Filename: hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.56.dist-info/METADATA
+Filename: hmd_cli_transform_deploy-0.1.57.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.56.dist-info/WHEEL
+Filename: hmd_cli_transform_deploy-0.1.57.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.56.dist-info/top_level.txt
+Filename: hmd_cli_transform_deploy-0.1.57.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.56.dist-info/RECORD
+Filename: hmd_cli_transform_deploy-0.1.57.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_transform_deploy/hmd_cli_transform_deploy.py

```diff
@@ -28,15 +28,15 @@
 def run_image_sequence(img_seq: list):
     input_path = os.getcwd()
     output_path = os.getcwd()
 
     for img in img_seq:
         img_name = img["image_name"]
 
-        base_cmd = f"docker run -v {input_path}:/hmd_transform/input -v {output_path}:/hmd_transform/output -e HMD_AUTH_TOKEN={get_auth_token()} "
+        base_cmd = f"docker run --network neuronsphere_default -v {input_path}:/hmd_transform/input -v {output_path}:/hmd_transform/output -e HMD_AUTH_TOKEN={get_auth_token()} "
 
         for k, v in img["env"].items():
             if v == "default":
                 v = os.environ.get(k, v)
             base_cmd += f"-e {k}={v} "
 
         base_cmd += f"{img_name} "
```

## Comparing `hmd_cli_transform_deploy-0.1.56.dist-info/METADATA` & `hmd_cli_transform_deploy-0.1.57.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-transform-deploy
-Version: 0.1.56
+Version: 0.1.57
 Summary: Command for deploying transforms
 Home-page: UNKNOWN
 Author: Kate Walls
 Author-email: kate.walls@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: acachecontrol (==0.3.5)
```

