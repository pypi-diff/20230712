# Comparing `tmp/cohere-sagemaker-0.6.3.tar.gz` & `tmp/cohere-sagemaker-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-sagemaker-0.6.3.tar", last modified: Tue May 30 19:55:42 2023, max compression
+gzip compressed data, was "cohere-sagemaker-0.7.0.tar", last modified: Wed Jul 12 17:22:52 2023, max compression
```

## Comparing `cohere-sagemaker-0.6.3.tar` & `cohere-sagemaker-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-30 19:55:42.723928 cohere-sagemaker-0.6.3/
--rw-r--r--   0 alexandre   (502) staff       (20)     1066 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/LICENSE
--rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-30 19:55:42.723780 cohere-sagemaker-0.6.3/PKG-INFO
--rw-r--r--   0 alexandre   (502) staff       (20)      948 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.3/README.md
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-30 19:55:42.722838 cohere-sagemaker-0.6.3/cohere_sagemaker/
--rw-r--r--   0 alexandre   (502) staff       (20)       57 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/__init__.py
--rw-r--r--   0 alexandre   (502) staff       (20)     1222 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/classification.py
--rw-r--r--   0 alexandre   (502) staff       (20)    19616 2023-05-30 19:55:02.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/client.py
--rw-r--r--   0 alexandre   (502) staff       (20)      623 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/embeddings.py
--rw-r--r--   0 alexandre   (502) staff       (20)      591 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/error.py
--rw-r--r--   0 alexandre   (502) staff       (20)      796 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/generation.py
--rw-r--r--   0 alexandre   (502) staff       (20)     2069 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/rerank.py
--rw-r--r--   0 alexandre   (502) staff       (20)      337 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/response.py
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-30 19:55:42.723544 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/
--rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 alexandre   (502) staff       (20)      460 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 alexandre   (502) staff       (20)        1 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       16 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/requires.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       17 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       38 2023-05-30 19:55:42.723978 cohere-sagemaker-0.6.3/setup.cfg
--rw-r--r--   0 alexandre   (502) staff       (20)     1525 2023-05-30 19:55:02.000000 cohere-sagemaker-0.6.3/setup.py
+drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1066 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/LICENSE
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1412 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/PKG-INFO
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      948 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/README.md
+drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/cohere_sagemaker/
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       57 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/__init__.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1222 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/classification.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)    21487 2023-07-12 17:22:44.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/client.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      623 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/embeddings.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      591 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/error.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      796 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/generation.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     2069 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/rerank.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      337 2023-07-11 10:58:17.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/response.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      491 2023-07-12 17:22:44.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/summary.py
+drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1412 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      488 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        1 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       16 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       17 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       38 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/setup.cfg
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1525 2023-07-12 17:22:44.000000 cohere-sagemaker-0.7.0/setup.py
```

### Comparing `cohere-sagemaker-0.6.3/LICENSE` & `cohere-sagemaker-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.3/PKG-INFO` & `cohere-sagemaker-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.6.3
+Version: 0.7.0
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.6.3/README.md` & `cohere-sagemaker-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.3/cohere_sagemaker/classification.py` & `cohere-sagemaker-0.7.0/cohere_sagemaker/classification.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.3/cohere_sagemaker/client.py` & `cohere-sagemaker-0.7.0/cohere_sagemaker/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from cohere_sagemaker.classification import Classification, Classifications
 from cohere_sagemaker.embeddings import Embeddings
 from cohere_sagemaker.error import CohereError
 from cohere_sagemaker.generation import (Generation, Generations,
                                          TokenLikelihood)
 from cohere_sagemaker.rerank import Reranking
+from cohere_sagemaker.summary import Summary
 
 
 class Client:
     def __init__(self, endpoint_name: Optional[str] = None, region_name: Optional[str] = None):
         """
         By default we assume region configured in AWS CLI (`aws configure get region`). You can change the region with
         `aws configure set region us-west-2` or override it with `region_name` parameter.
@@ -49,27 +50,27 @@
             raise CohereError(f"Endpoint {endpoint_name} does not exist.")
         self._endpoint_name = endpoint_name
 
     def _s3_models_dir_to_tarfile(self, s3_models_dir: str) -> str:
         """
         Compress an S3 folder which contains one or several fine-tuned models to a tar file.
         If the S3 folder contains only one fine-tuned model, it simply returns the path to that model.
-        If the S3 folder contains several fine-tuned models, it download all models, aggregates them into a single 
+        If the S3 folder contains several fine-tuned models, it download all models, aggregates them into a single
         tar.gz file.
 
         Args:
             s3_models_dir (str): S3 URI pointing to a folder
 
         Returns:
             str: S3 URI pointing to the `models.tar.gz` file
         """
 
         s3_models_dir = s3_models_dir + ("/" if not s3_models_dir.endswith("/") else "")
 
-        # Links of all fine-tuned models in s3_models_dir. Their format should be .tar.gz 
+        # Links of all fine-tuned models in s3_models_dir. Their format should be .tar.gz
         s3_tar_models = [
             s3_path
             for s3_path in S3Downloader.list(s3_models_dir, sagemaker_session=self._sess)
             if (
                 s3_path.endswith(".tar.gz")  # only .tar.gz files
                 and (s3_path.split("/")[-1] != "models.tar.gz")  # exclude the .tar.gz file we are creating
                 and (s3_path.rsplit("/", 1)[0] == s3_models_dir[:-1])  # only files at the root of s3_models_dir
@@ -89,15 +90,15 @@
 
             # Download and extract all fine-tuned models
             for s3_tar_model in s3_tar_models:
                 print(f"Adding fine-tuned model: {s3_tar_model}")
                 S3Downloader.download(s3_tar_model, local_tar_models_dir, sagemaker_session=self._sess)
                 with tarfile.open(os.path.join(local_tar_models_dir, s3_tar_model.split("/")[-1])) as tar:
                     tar.extractall(local_models_dir)
-                
+
             # Compress local_models_dir to a tar.gz file
             model_tar = os.path.join(tmpdir, "models.tar.gz")
             with tarfile.open(model_tar, "w:gz") as tar:
                 tar.add(local_models_dir, arcname=".")
 
             # Upload the new tarfile containing all models to s3
             # Very important to remove the trailing slash from s3_models_dir otherwise it just doesn't upload
@@ -125,15 +126,15 @@
                 (algorithm).
             endpoint_name (str): The name of the endpoint.
             s3_models_dir (str, optional): S3 URI pointing to the folder containing fine-tuned models. Defaults to None.
             instance_type (str, optional): The EC2 instance type to deploy the endpoint to. Defaults to "ml.g4dn.xlarge".
             n_instances (int, optional): Number of endpoint instances. Defaults to 1.
             recreate (bool, optional): Force re-creation of endpoint if it already exists. Defaults to False.
             rool (str, optional): The IAM role to use for the endpoint. If not provided, sagemaker.get_execution_role()
-                will be used to get the role. This should work when one uses the client inside SageMaker. If this errors 
+                will be used to get the role. This should work when one uses the client inside SageMaker. If this errors
                 out, the default role "ServiceRoleSagemaker" will be used, which generally works outside of SageMaker.
         """
         # First, check if endpoint already exists
         if self._does_endpoint_exist(endpoint_name):
             if recreate:
                 self.connect_to_endpoint(endpoint_name)
                 self.delete_endpoint()
@@ -162,29 +163,29 @@
                 role = sage.get_execution_role()
             except ValueError:
                 print("Using default role: 'ServiceRoleSagemaker'.")
                 role = "ServiceRoleSagemaker"
 
         model = sage.ModelPackage(
             role=role,
-            model_data=model_data, 
+            model_data=model_data,
             sagemaker_session=self._sess,  # makes sure the right region is used
             **kwargs
         )
 
         validation_params = dict(
-            model_data_download_timeout=2400, 
+            model_data_download_timeout=2400,
             container_startup_health_check_timeout=2400
         )
 
         try:
             model.deploy(
-                n_instances, 
-                instance_type, 
-                endpoint_name=endpoint_name, 
+                n_instances,
+                instance_type,
+                endpoint_name=endpoint_name,
                 **validation_params
             )
         except ParamValidationError:
             # For at least some versions of python 3.6, SageMaker SDK does not support the validation_params
             model.deploy(n_instances, instance_type, endpoint_name=endpoint_name)
         self.connect_to_endpoint(endpoint_name)
 
@@ -204,15 +205,16 @@
         stop_sequences: Optional[List[str]] = None,
         return_likelihoods: Optional[str] = None,
         truncate: Optional[str] = None,
         variant: Optional[str] = None
     ) -> Generations:
 
         if self._endpoint_name is None:
-            raise CohereError("No endpoint connected. Run connect_to_endpoint() first.")
+            raise CohereError("No endpoint connected. "
+                              "Run connect_to_endpoint() first.")
 
         json_params = {
             'prompt': prompt,
             'max_tokens': max_tokens,
             'temperature': temperature,
             'k': k,
             'p': p,
@@ -236,21 +238,21 @@
         try:
             result = self._client.invoke_endpoint(**params)
             response = json.loads(result['Body'].read().decode())
         except EndpointConnectionError as e:
             raise CohereError(str(e))
         except Exception as e:
             # TODO should be client error - distinct type from CohereError?
-            # ValidationError, e.g. when variant is bad 
+            # ValidationError, e.g. when variant is bad
             raise CohereError(str(e))
 
         generations: List[Generation] = []
         for gen in response['generations']:
             token_likelihoods = None
-                
+
             if 'token_likelihoods' in gen:
                 token_likelihoods = []
                 for likelihoods in gen['token_likelihoods']:
                     token_likelihood = likelihoods['likelihood'] if 'likelihood' in likelihoods else None
                     token_likelihoods.append(TokenLikelihood(likelihoods['token'], token_likelihood))
             generations.append(Generation(gen['text'], token_likelihoods))
         return Generations(generations)
@@ -259,15 +261,16 @@
         self,
         texts: List[str],
         truncate: Optional[str] = None,
         variant: Optional[str] = None
     ) -> Embeddings:
 
         if self._endpoint_name is None:
-            raise CohereError("No endpoint connected. Run connect_to_endpoint() first.")
+            raise CohereError("No endpoint connected. "
+                              "Run connect_to_endpoint() first.")
 
         json_params = {
             'texts': texts,
             'truncate': truncate
         }
         for key, value in list(json_params.items()):
             if value is None:
@@ -285,15 +288,15 @@
         try:
             result = self._client.invoke_endpoint(**params)
             response = json.loads(result['Body'].read().decode())
         except EndpointConnectionError as e:
             raise CohereError(str(e))
         except Exception as e:
             # TODO should be client error - distinct type from CohereError?
-            # ValidationError, e.g. when variant is bad 
+            # ValidationError, e.g. when variant is bad
             raise CohereError(str(e))
 
         return Embeddings(response['embeddings'])
 
     def rerank(self,
                query: str,
                documents: Union[List[str], List[Dict[str, Any]]],
@@ -305,15 +308,16 @@
             query (str): The search query
             documents (list[str], list[dict]): The documents to rerank
             top_n (int): (optional) The number of results to return, defaults to return all results
             max_chunks_per_doc (int): (optional) The maximum number of chunks derived from a document
         """
 
         if self._endpoint_name is None:
-            raise CohereError("No endpoint connected. Run connect_to_endpoint() first.")
+            raise CohereError("No endpoint connected. "
+                              "Run connect_to_endpoint() first.")
 
         parsed_docs = []
         for doc in documents:
             if isinstance(doc, str):
                 parsed_docs.append({'text': doc})
             elif isinstance(doc, dict) and 'text' in doc:
                 parsed_docs.append(doc)
@@ -344,23 +348,24 @@
             reranking = Reranking(response)
             for rank in reranking.results:
                 rank.document = parsed_docs[rank.index]
         except EndpointConnectionError as e:
             raise CohereError(str(e))
         except Exception as e:
             # TODO should be client error - distinct type from CohereError?
-            # ValidationError, e.g. when variant is bad 
+            # ValidationError, e.g. when variant is bad
             raise CohereError(str(e))
-        
+
         return reranking
 
     def classify(self, input: List[str], name: str) -> Classifications:
 
         if self._endpoint_name is None:
-            raise CohereError("No endpoint connected. Run connect_to_endpoint() first.")
+            raise CohereError("No endpoint connected. "
+                              "Run connect_to_endpoint() first.")
 
         json_params = {"texts": input, "model_id": name}
         json_body = json.dumps(json_params)
 
         params = {
             "EndpointName": self._endpoint_name,
             "ContentType": "application/json",
@@ -397,15 +402,15 @@
             name (str): The name to give to the fine-tuned model.
             train_data (str): An S3 path pointing to the training data.
             s3_models_dir (str): An S3 path pointing to the directory where the fine-tuned model will be saved.
             eval_data (str, optional): An S3 path pointing to the eval data. Defaults to None.
             instance_type (str, optional): The EC2 instance type to use for training. Defaults to "ml.g4dn.xlarge".
             training_parameters (Dict[str, Any], optional): Additional training parameters. Defaults to {}.
             rool (str, optional): The IAM role to use for the endpoint. If not provided, sagemaker.get_execution_role()
-                will be used to get the role. This should work when one uses the client inside SageMaker. If this errors 
+                will be used to get the role. This should work when one uses the client inside SageMaker. If this errors
                 out, the default role "ServiceRoleSagemaker" will be used, which generally works outside of SageMaker.
         """
         assert len(training_parameters) == 0, "training_parameters not yet supported."
         assert name != "model", "name cannot be 'model'"
         s3_models_dir = s3_models_dir + ("/" if not s3_models_dir.endswith("/") else "")
 
         if role is None:
@@ -445,22 +450,74 @@
         _, new_key = parse_s3_url(f"{s3_models_dir}{name}.tar.gz")
         s3_resource.Object(bucket, new_key).copy_from(CopySource={"Bucket": bucket, "Key": old_key})
 
         # Delete old dir
         bucket, old_short_key = parse_s3_url(s3_models_dir + job_name)
         s3_resource.Bucket(bucket).objects.filter(Prefix=old_short_key).delete()
 
+    def summarize(
+        self,
+        text: str,
+        length: Optional[str] = "auto",
+        format_: Optional[str] = "auto",
+        # Only summarize-xlarge is supported on Sagemaker
+        # model: Optional[str] = "summarize-xlarge",
+        extractiveness: Optional[str] = "auto",
+        temperature: Optional[float] = 1.0,
+        additional_command: Optional[str] = "",
+        variant: Optional[str] = None
+    ) -> Summary:
+
+        if self._endpoint_name is None:
+            raise CohereError("No endpoint connected. "
+                              "Run connect_to_endpoint() first.")
+
+        json_params = {
+            'text': text,
+            'length': length,
+            'format': format_,
+            'extractiveness': extractiveness,
+            'temperature': temperature,
+            'additional_command': additional_command,
+        }
+        for key, value in list(json_params.items()):
+            if value is None:
+                del json_params[key]
+        json_body = json.dumps(json_params)
+
+        params = {
+            'EndpointName': self._endpoint_name,
+            'ContentType': 'application/json',
+            'Body': json_body,
+        }
+        if variant is not None:
+            params['TargetVariant'] = variant
+
+        try:
+            result = self._client.invoke_endpoint(**params)
+            response = json.loads(result['Body'].read().decode())
+            summary = Summary(response)
+        except EndpointConnectionError as e:
+            raise CohereError(str(e))
+        except Exception as e:
+            # TODO should be client error - distinct type from CohereError?
+            # ValidationError, e.g. when variant is bad
+            raise CohereError(str(e))
+
+        return summary
+
+
     def delete_endpoint(self) -> None:
         if self._endpoint_name is None:
             raise CohereError("No endpoint connected.")
         try:
             self._service_client.delete_endpoint(EndpointName=self._endpoint_name)
         except:
             print("Endpoint not found, skipping deletion.")
-        
+
         try:
             self._service_client.delete_endpoint_config(EndpointConfigName=self._endpoint_name)
         except:
             print("Endpoint config not found, skipping deletion.")
 
     def close(self) -> None:
         try:
```

### Comparing `cohere-sagemaker-0.6.3/cohere_sagemaker/embeddings.py` & `cohere-sagemaker-0.7.0/cohere_sagemaker/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.3/cohere_sagemaker/error.py` & `cohere-sagemaker-0.7.0/cohere_sagemaker/error.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.3/cohere_sagemaker/generation.py` & `cohere-sagemaker-0.7.0/cohere_sagemaker/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.3/cohere_sagemaker/rerank.py` & `cohere-sagemaker-0.7.0/cohere_sagemaker/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/PKG-INFO` & `cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.6.3
+Version: 0.7.0
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.6.3/setup.py` & `cohere-sagemaker-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 
 setuptools.setup(name='cohere-sagemaker',
-                 version='0.6.3',
+                 version='0.7.0',
                  author='Cohere',
                  author_email='support@cohere.ai',
                  description='A Python library for the Cohere endpoints in AWS Sagemaker',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/cohere-ai/cohere-sagemaker',
                  packages=setuptools.find_packages(),
```

