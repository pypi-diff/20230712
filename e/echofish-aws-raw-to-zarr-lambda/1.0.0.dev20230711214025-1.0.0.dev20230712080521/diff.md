# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025.tar", last modified: Tue Jul 11 21:41:26 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521.tar", last modified: Wed Jul 12 08:06:26 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-11 21:41:22.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:41:26.418817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15056 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-07-11 21:40:20.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 21:41:26.422817 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 21:41:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-12 08:06:21.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15055 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711214025
+Version: 1.0.0.dev20230712080521
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230711214025",
+  version="1.0.0.dev20230712080521",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             self,
             s3_operations,
             dynamo_operations,
             input_bucket,
             output_bucket,
             table_name,
             output_bucket_access_key,
-            output_bucket_secret_access_key
+            output_bucket_secret_access_key,
     ):
         self.__s3 = s3_operations
         self.__dynamo = dynamo_operations
         self.__input_bucket = input_bucket
         self.__output_bucket = output_bucket
         self.__table_name = table_name
         self.__output_bucket_access_key = output_bucket_access_key
@@ -316,15 +316,15 @@
         for key in keys:
             self.__s3.delete_object(
                 bucket_name=self.__output_bucket,
                 key=key,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
             )
-        # print('Removing existing s3 objects done')
+        print('Removing existing s3 objects done')
 
     ############################################################################
     def __upload_files(
             self,
             local_directory,
             object_prefix
     ):
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 # lambda_handler.py
 import os
 import json
 from .lambda_executor import LambdaExecutor
 from .s3_operations import S3Operations
 from .dynamo_operations import DynamoOperations
 
+
 input_bucket = os.environ['INPUT_BUCKET']
 output_bucket = os.environ['OUTPUT_BUCKET']
 table_name = os.environ['TABLE_NAME']
 
-# if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
-#     output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
-#
-# if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
-#     output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
-
 executor = LambdaExecutor(
     s3_operations=S3Operations(),
     dynamo_operations=DynamoOperations(),
     input_bucket=input_bucket,
     output_bucket=output_bucket,
     table_name=table_name,
     output_bucket_access_key=os.getenv('OUTPUT_BUCKET_ACCESS_KEY'),
     output_bucket_secret_access_key=os.getenv('OUTPUT_BUCKET_SECRET_ACCESS_KEY')
 )
 
-
 def handler(sns_event, context):
     print(f"table name: {os.environ['TABLE_NAME']}")
     print(f"input bucket: {os.environ['INPUT_BUCKET']}")
     print(f"output bucket: {os.environ['OUTPUT_BUCKET']}")
     if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
         print(os.environ['OUTPUT_BUCKET_ACCESS_KEY'])
     if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
         print(os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY'])
     #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
-    # There should only ever be one message at a time.
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
         executor.execute(message)
         print("Done Message : " + str(message))
     print("Done Event : " + str(sns_event))
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         session = boto3.Session()
         if access_key_id:
             s3_client = session.client(
                 service_name='s3',
                 aws_access_key_id=access_key_id,
                 aws_secret_access_key=secret_access_key
             )
+            print('NODD Authenticated')
         else:
             s3_client = session.client(service_name='s3')
         return s3_client
 
     #####################################################################
     def __chunked(
             self,
@@ -77,18 +78,14 @@
     def delete_object(
             self,
             bucket_name,
             key,
             access_key_id=None,
             secret_access_key=None
     ):
-        print(access_key_id)
-        print(type(access_key_id))
-        print(secret_access_key)
-        print(type(secret_access_key))
         print('key')
         print(key)
         s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
         print(f"Deleting item: Bucket={bucket_name}, Key={key}")
         s3_client.delete_object(Bucket=bucket_name, Key=key)
 
     #####################################################################
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230711214025
+Version: 1.0.0.dev20230712080521
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230711214025/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

