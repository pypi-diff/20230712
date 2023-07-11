# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831.tar", last modified: Tue Jul 11 21:19:31 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025.tar", last modified: Tue Jul 11 21:41:26 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:19:31.591630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 21:19:31.591630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 21:19:31.591630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 21:19:27.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:19:31.587630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:19:31.587630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15083 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3375 2023-07-11 21:18:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:19:31.591630 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 21:19:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 21:41:22.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:41:26.418817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15056 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711211831
+Version: 1.0.0.dev20230711214025
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230711211831",
+  version="1.0.0.dev20230711214025",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -298,22 +298,22 @@
             start_time=start_time,
             end_time=end_time,
             frequencies=frequencies,
             channels=channels
         )
 
     ############################################################################
-    def __remove_existing_s3_objects(  # "delete_remote_objects"
+    def __remove_existing_s3_objects(
             self,
-            output_zarr_prefix
+            prefix
     ):
-        print(f'Removing existing s3 objects from: {self.__output_bucket} with prefix {output_zarr_prefix}')
+        print(f'Removing existing s3 objects from: {self.__output_bucket} with prefix {prefix}')
         keys = self.__s3.list_objects(
             bucket_name=self.__output_bucket,
-            prefix=output_zarr_prefix,
+            prefix=prefix,
             access_key_id=self.__output_bucket_access_key,
             secret_access_key=self.__output_bucket_secret_access_key
         )
         for key in keys:
             self.__s3.delete_object(
                 bucket_name=self.__output_bucket,
                 key=key,
@@ -377,15 +377,17 @@
         self.__create_local_zarr_store(
             raw_file_name=input_file_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
             output_zarr_prefix=output_zarr_prefix,
             store_name=store_name
         )
-        self.__remove_existing_s3_objects(output_zarr_prefix=output_zarr_prefix)
+        self.__remove_existing_s3_objects(
+            prefix=os.path.join(output_zarr_prefix, store_name)
+        )
         self.__upload_files(store_name, output_zarr_prefix)
         self.__update_processing_status(
             cruise_name=cruise_name,
             file_name=input_file_name,
             new_status='SUCCESS'
         )
         self.__delete_all_local_raw_and_zarr_files()
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 from .s3_operations import S3Operations
 from .dynamo_operations import DynamoOperations
 
 input_bucket = os.environ['INPUT_BUCKET']
 output_bucket = os.environ['OUTPUT_BUCKET']
 table_name = os.environ['TABLE_NAME']
 
-if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
-    output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
-
-if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
-    output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
+# if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
+#     output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
+#
+# if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
+#     output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
 
 executor = LambdaExecutor(
     s3_operations=S3Operations(),
     dynamo_operations=DynamoOperations(),
     input_bucket=input_bucket,
     output_bucket=output_bucket,
     table_name=table_name,
     output_bucket_access_key=os.getenv('OUTPUT_BUCKET_ACCESS_KEY'),
     output_bucket_secret_access_key=os.getenv('OUTPUT_BUCKET_SECRET_ACCESS_KEY')
 )
 
 
 def handler(sns_event, context):
-    print(os.environ['TABLE_NAME'])
-    print(os.environ['INPUT_BUCKET'])
-    print(os.environ['OUTPUT_BUCKET'])
+    print(f"table name: {os.environ['TABLE_NAME']}")
+    print(f"input bucket: {os.environ['INPUT_BUCKET']}")
+    print(f"output bucket: {os.environ['OUTPUT_BUCKET']}")
     if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
         print(os.environ['OUTPUT_BUCKET_ACCESS_KEY'])
     if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
         print(os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY'])
     #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,15 +77,22 @@
     def delete_object(
             self,
             bucket_name,
             key,
             access_key_id=None,
             secret_access_key=None
     ):
+        print(access_key_id)
+        print(type(access_key_id))
+        print(secret_access_key)
+        print(type(secret_access_key))
+        print('key')
+        print(key)
         s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
+        print(f"Deleting item: Bucket={bucket_name}, Key={key}")
         s3_client.delete_object(Bucket=bucket_name, Key=key)
 
     #####################################################################
     def upload_file(
             self,
             file_name,
             bucket_name,
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711211831
+Version: 1.0.0.dev20230711214025
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711211831/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

