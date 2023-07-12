# Comparing `tmp/inference_client-0.0.7.tar.gz` & `tmp/inference_client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference_client-0.0.7.tar", max compression
+gzip compressed data, was "inference_client-0.0.8.tar", max compression
```

## Comparing `inference_client-0.0.7.tar` & `inference_client-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-12 03:21:39.450709 inference_client-0.0.7/LICENSE
--rw-r--r--   0        0        0     5030 2023-07-12 03:21:39.450709 inference_client-0.0.7/README.md
--rw-r--r--   0        0        0      256 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/__init__.py
--rw-r--r--   0        0        0     2349 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/__version__.py
--rw-r--r--   0        0        0     2062 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/client.py
--rw-r--r--   0        0        0      719 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/config.py
--rw-r--r--   0        0        0     3131 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/helper.py
--rw-r--r--   0        0        0      250 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/logging.py
--rw-r--r--   0        0        0      618 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/model.py
--rw-r--r--   0        0        0     3541 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/caption.py
--rw-r--r--   0        0        0    11314 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/encode.py
--rw-r--r--   0        0        0     4141 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/generate.py
--rw-r--r--   0        0        0     2426 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/helper.py
--rw-r--r--   0        0        0     6174 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/rank.py
--rw-r--r--   0        0        0    13226 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/upscale.py
--rw-r--r--   0        0        0     3929 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/vqa.py
--rw-r--r--   0        0        0     1355 2023-07-12 03:21:39.510709 inference_client-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    17410 1970-01-01 00:00:00.000000 inference_client-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-12 04:27:40.256550 inference_client-0.0.8/LICENSE
+-rw-r--r--   0        0        0     5030 2023-07-12 04:27:40.256550 inference_client-0.0.8/README.md
+-rw-r--r--   0        0        0      256 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/__init__.py
+-rw-r--r--   0        0        0     2349 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/__version__.py
+-rw-r--r--   0        0        0     2062 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/client.py
+-rw-r--r--   0        0        0      719 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/config.py
+-rw-r--r--   0        0        0     3131 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/helper.py
+-rw-r--r--   0        0        0      250 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/logging.py
+-rw-r--r--   0        0        0      618 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/model.py
+-rw-r--r--   0        0        0     3541 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/tasks/caption.py
+-rw-r--r--   0        0        0    11314 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/tasks/encode.py
+-rw-r--r--   0        0        0     4191 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/tasks/generate.py
+-rw-r--r--   0        0        0     2426 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/tasks/helper.py
+-rw-r--r--   0        0        0     6174 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/tasks/rank.py
+-rw-r--r--   0        0        0    13226 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/tasks/upscale.py
+-rw-r--r--   0        0        0     3929 2023-07-12 04:27:40.316550 inference_client-0.0.8/inference_client/tasks/vqa.py
+-rw-r--r--   0        0        0     1355 2023-07-12 04:27:40.316550 inference_client-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    17410 1970-01-01 00:00:00.000000 inference_client-0.0.8/PKG-INFO
```

### Comparing `inference_client-0.0.7/LICENSE` & `inference_client-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/README.md` & `inference_client-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/__version__.py` & `inference_client-0.0.8/inference_client/__version__.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/client.py` & `inference_client-0.0.8/inference_client/client.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/config.py` & `inference_client-0.0.8/inference_client/config.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/helper.py` & `inference_client-0.0.8/inference_client/helper.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/model.py` & `inference_client-0.0.8/inference_client/model.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/tasks/caption.py` & `inference_client-0.0.8/inference_client/tasks/caption.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/tasks/encode.py` & `inference_client-0.0.8/inference_client/tasks/encode.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/tasks/generate.py` & `inference_client-0.0.8/inference_client/tasks/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,18 @@
         payload = self._get_generate_payload(**kwargs)
         payload.update(
             inputs=DocumentArray(
                 [Document(tags={'prompt': prompt}) for prompt in prompts]
             )
         )
         result = self.client.post(**payload)
-        text_out = [r.tags['generated_text'] or r.tags['response'] for r in result]
+        text_out = [
+            r.tags.get('generated_text', '') or r.tags.get('response', '')
+            for r in result
+        ]
         return text_out if len(text_out) > 1 else text_out[0]
 
     def _get_generate_payload(self, **kwargs):
         """Get the payload for the generate endpoint.
 
         :param kwargs: The arguments to pass to the model.
         :return: The payload.
```

### Comparing `inference_client-0.0.7/inference_client/tasks/helper.py` & `inference_client-0.0.8/inference_client/tasks/helper.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/tasks/rank.py` & `inference_client-0.0.8/inference_client/tasks/rank.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/tasks/upscale.py` & `inference_client-0.0.8/inference_client/tasks/upscale.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/inference_client/tasks/vqa.py` & `inference_client-0.0.8/inference_client/tasks/vqa.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.7/pyproject.toml` & `inference_client-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inference_client"
-version = "0.0.7"
+version = "0.0.8"
 description = "Python Client for Jina Inference API"
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
```

### Comparing `inference_client-0.0.7/PKG-INFO` & `inference_client-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python Client for Jina Inference API
 Home-page: https://inference-api.jina.ai
 License: Apache-2.0
 Keywords: jina,inference,api,client
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inference-client Version: 0.0.7 Summary: Python
+Metadata-Version: 2.1 Name: inference-client Version: 0.0.8 Summary: Python
 Client for Jina Inference API Home-page: https://inference-api.jina.ai License:
 Apache-2.0 Keywords: jina,inference,api,client Author: Jina AI Author-email:
 hello@jina.ai Requires-Python: >=3.8,<4.0.0 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: pytorch
```

