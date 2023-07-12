# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521.tar", last modified: Wed Jul 12 08:06:26 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818.tar", last modified: Wed Jul 12 08:29:19 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-12 08:06:21.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15055 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-12 08:05:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:06:26.249400 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-12 08:06:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:29:19.294409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-12 08:29:19.294409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 08:29:19.294409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-12 08:29:14.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:29:19.290409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:29:19.290409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15654 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:29:19.294409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230712080521
+Version: 1.0.0.dev20230712082818
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -310,14 +310,19 @@
         keys = self.__s3.list_objects(
             bucket_name=self.__output_bucket,
             prefix=prefix,
             access_key_id=self.__output_bucket_access_key,
             secret_access_key=self.__output_bucket_secret_access_key
         )
         for key in keys:
+            # TODO: Fails here with unauthorized credentials. Try testing writing and deleting
+            #  object to the 'noaa-wcsd-zarr-pds' bucket to see if you have the same problem.
+            #  Once this is working again, the echofish-aws-raw-to-zarr-lambda should be working
+            #  fully. I simplified the echofish-aws-cloudformation project by turning off some features
+            #  they need to be turned back on...
             self.__s3.delete_object(
                 bucket_name=self.__output_bucket,
                 key=key,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
             )
         print('Removing existing s3 objects done')
@@ -377,14 +382,16 @@
         self.__create_local_zarr_store(
             raw_file_name=input_file_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
             output_zarr_prefix=output_zarr_prefix,
             store_name=store_name
         )
+        # TODO: problem here, this is the first use of the NOAA-NODD credentials and for some reason
+        # those credentials can write but cannot delete???
         self.__remove_existing_s3_objects(
             prefix=os.path.join(output_zarr_prefix, store_name)
         )
         self.__upload_files(store_name, output_zarr_prefix)
         self.__update_processing_status(
             cruise_name=cruise_name,
             file_name=input_file_name,
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230712080521
+Version: 1.0.0.dev20230712082818
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712080521/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

