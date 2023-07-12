# Comparing `tmp/inference_client-0.0.6.tar.gz` & `tmp/inference_client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference_client-0.0.6.tar", max compression
+gzip compressed data, was "inference_client-0.0.7.tar", max compression
```

## Comparing `inference_client-0.0.6.tar` & `inference_client-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-06-13 13:35:39.484234 inference_client-0.0.6/LICENSE
--rw-r--r--   0        0        0     5030 2023-06-13 13:35:39.484234 inference_client-0.0.6/README.md
--rw-r--r--   0        0        0      256 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/__init__.py
--rw-r--r--   0        0        0     2349 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/__version__.py
--rw-r--r--   0        0        0     1546 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/client.py
--rw-r--r--   0        0        0      719 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/config.py
--rw-r--r--   0        0        0     3129 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/helper.py
--rw-r--r--   0        0        0      250 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/logging.py
--rw-r--r--   0        0        0      551 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/model.py
--rw-r--r--   0        0        0     3541 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/caption.py
--rw-r--r--   0        0        0     5855 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/encode.py
--rw-r--r--   0        0        0     3664 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/generate.py
--rw-r--r--   0        0        0     2389 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/helper.py
--rw-r--r--   0        0        0     6174 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/rank.py
--rw-r--r--   0        0        0    13226 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/upscale.py
--rw-r--r--   0        0        0     3929 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/vqa.py
--rw-r--r--   0        0        0     1355 2023-06-13 13:35:39.536234 inference_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    17410 1970-01-01 00:00:00.000000 inference_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-12 03:21:39.450709 inference_client-0.0.7/LICENSE
+-rw-r--r--   0        0        0     5030 2023-07-12 03:21:39.450709 inference_client-0.0.7/README.md
+-rw-r--r--   0        0        0      256 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/__init__.py
+-rw-r--r--   0        0        0     2349 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/__version__.py
+-rw-r--r--   0        0        0     2062 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/client.py
+-rw-r--r--   0        0        0      719 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/config.py
+-rw-r--r--   0        0        0     3131 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/helper.py
+-rw-r--r--   0        0        0      250 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/logging.py
+-rw-r--r--   0        0        0      618 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/model.py
+-rw-r--r--   0        0        0     3541 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/caption.py
+-rw-r--r--   0        0        0    11314 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/encode.py
+-rw-r--r--   0        0        0     4141 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/generate.py
+-rw-r--r--   0        0        0     2426 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/helper.py
+-rw-r--r--   0        0        0     6174 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/rank.py
+-rw-r--r--   0        0        0    13226 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/upscale.py
+-rw-r--r--   0        0        0     3929 2023-07-12 03:21:39.510709 inference_client-0.0.7/inference_client/tasks/vqa.py
+-rw-r--r--   0        0        0     1355 2023-07-12 03:21:39.510709 inference_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    17410 1970-01-01 00:00:00.000000 inference_client-0.0.7/PKG-INFO
```

### Comparing `inference_client-0.0.6/LICENSE` & `inference_client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.6/README.md` & `inference_client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.6/inference_client/__version__.py` & `inference_client-0.0.7/inference_client/__version__.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.6/inference_client/client.py` & `inference_client-0.0.7/inference_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,25 +31,45 @@
     @lru_cache(maxsize=10)
     def get_model(
         self, model_name: Optional[str] = None, endpoint: Optional[str] = None
     ):
         """
         Get a model by name or endpoint. Returns a cached model if it exists.
 
+        Example:
+
+        ```python
+        from jina import Client
+
+        client = Client()
+
+        # get model by name
+        model = client.get_model('Salesforce/blip2-flan-t5-xl')
+
+        # or get model by endpoint
+        model = client.get_model('grpc://localhost:12345')
+        ```
+
         :param model_name: The name of the model.
         :param endpoint: The endpoint of the model.
         :return: The model.
         """
 
-        if not self._auth_token and not endpoint:
+        if not model_name and not endpoint:
             raise ValueError(
-                'Please provide an endpoint or a valid user token to access the model.'
+                'Please provide either a model name or endpoint to get a model.'
             )
 
-        if model_name:
+        from urllib.parse import urlparse
+
+        # Note: if endpoint is provided, model_name is ignored
+        o = urlparse(endpoint or model_name)
+        if o.scheme and o.netloc:
+            endpoint = endpoint or model_name
+        elif model_name:
             spec = get_model_spec(model_name, self._auth_token)
             endpoint = spec['endpoints']['grpc']
 
         return Model(
             model_name=model_name,
             token=self._auth_token,
             host=endpoint,
```

### Comparing `inference_client-0.0.6/inference_client/config.py` & `inference_client-0.0.7/inference_client/config.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.6/inference_client/helper.py` & `inference_client-0.0.7/inference_client/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     :param token: An optional token to use for authentication. If not set, it will try to login using the auth token
         in the env, or guide the user to login from a pop-out window
     :return: The validated token.
     """
     if token:
         os.environ['JINA_AUTH_TOKEN'] = token
         Auth.validate_token(token)
-        logger.info(f'successfully validated token: {token}')
+        logger.debug(f'successfully validated token: {token}')
         return token
     else:
         hubble.login()
         token = hubble.get_token()
-        logger.info(f'successfully logged in with token: {token}')
+        logger.debug(f'successfully logged in with token: {token}')
         return token
 
 
 @lru_cache(maxsize=10)
 def get_model_spec(model_name: str, token: str):
     """
     Retrieves the model spec for the specified model.
```

### Comparing `inference_client-0.0.6/inference_client/model.py` & `inference_client-0.0.7/inference_client/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from jina import Client
 
 from .tasks.caption import CaptionMixin
 from .tasks.encode import EncodeMixin
+from .tasks.generate import GenerationMixin
 from .tasks.rank import RankMixin
 from .tasks.upscale import UpscaleMixin
 from .tasks.vqa import VQAMixin
 
 
-class Model(CaptionMixin, EncodeMixin, RankMixin, UpscaleMixin, VQAMixin):
+class Model(
+    CaptionMixin, EncodeMixin, RankMixin, UpscaleMixin, VQAMixin, GenerationMixin
+):
     """
     The model to be used for inference.
     """
 
     def __init__(self, model_name: str, token: str, host: str, **kwargs):
         self.model_name = model_name
         self.token = token
```

### Comparing `inference_client-0.0.6/inference_client/tasks/caption.py` & `inference_client-0.0.7/inference_client/tasks/caption.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.6/inference_client/tasks/encode.py` & `inference_client-0.0.7/inference_client/tasks/rank.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,110 +6,103 @@
 
 from .helper import get_base_payload, iter_doc, load_plain_into_document
 
 if TYPE_CHECKING:
     from docarray.typing import ArrayType
 
 
-class EncodeMixin:
+class RankMixin:
     """
-    Mixin class for encoding documents.
+    Mixin class for ranking documents.
     """
 
     token: str
     client: Client
 
     @overload
-    def encode(self, *, text: Union[str, Iterable[str]], **kwargs):
+    def rank(
+        self,
+        *,
+        text: str,
+        candidates: Iterable[Union[str, bytes, 'ArrayType']],
+        **kwargs,
+    ):
         """
-        Encode plain text.
+        Rank the documents using the model.
 
-        :param text: the text to encode.
+        :param text: the reference text.
+        :param candidates: the candidates to be ranked, can be either a list of strings or a list of images.
         :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
-    def encode(
+    def rank(
         self,
         *,
-        image: Union[
-            str,
-            bytes,
-            'ArrayType',
-            Iterable[str],
-            Iterable[bytes],
-            Iterable['ArrayType'],
-        ],
+        image: Union[str, bytes, 'ArrayType'],
+        candidates: Iterable[Union[str, bytes, 'ArrayType']],
         **kwargs,
     ):
         """
-        Encode image.
+        Rank the documents using the model.
 
-        :param image: the image to encode, can be a `ndarray`, 'bytes' or uri of the image.
+        :param image: the reference image, can be a `ndarray`, 'bytes' or uri of the image.
+        :param candidates: the candidates to be ranked, can be either a list of strings or a list of images.
         :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
-    def encode(self, *, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
+    def rank(self, *, docs: Union[Iterable['Document'], 'DocumentArray'], **kwargs):
         """
-        Encode documents
+        Rank the documents using the model.
 
-        :param docs: the documents to encode
-        :param kwargs: additional arguments to pass to the model
+        :param docs: the documents to be ranked with candidates stored in the matches.
+        :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
-    def encode(
+    def rank(
         self,
         *,
         docs: Optional[Union[Iterable['Document'], 'DocumentArray']] = None,
-        text: Optional[Union[str, Iterable[str]]] = None,
-        image: Optional[
-            Union[
-                str,
-                bytes,
-                'ArrayType',
-                Iterable[str],
-                Iterable[bytes],
-                Iterable['ArrayType'],
-            ]
-        ] = None,
+        text: Optional[str] = None,
+        image: Optional[Union[str, bytes, 'ArrayType']] = None,
+        candidates: Optional[Iterable[Union[str, bytes, 'ArrayType']]] = None,
         **kwargs,
     ):
         """
-        Encode text, image, or documents using a pre-trained model.
+        Rank the documents using the model.
 
-        :param docs: the documents to encode. Default: None.
-        :param text: the text to encode. Default: None.
-        :param image: the image to encode, can be a `ndarray`, 'bytes' or uri of the image. Default: None.
+        :param docs: the documents to be ranked with candidates stored in the matches. Default: None.
+        :param text: the reference text. Default: None.
+        :param image: the reference image, can be a `ndarray`, 'bytes' or uri of the image. Default: None.
+        :param candidates: the candidates to be ranked, can be either a list of strings or a list of images. Default: None.
         :param kwargs: additional arguments to pass to the model.
         """
         ...
 
-    def encode(self, **kwargs):
+    def rank(self, **kwargs):
         """
-        Encode the documents using the model.
+        Rank the documents using the model.
 
         :param kwargs: additional arguments to pass to the model.
-        :return: encoded content.
+        :return: ranked content.
         """
-        payload, content_type, is_list = self._get_enocde_payload(**kwargs)
+        payload, content_type = self._get_rank_payload(**kwargs)
         result = self.client.post(**payload)
-        return self._unbox_encode_result(
+        return self._unbox_rank_result(
             result=result,
             content_type=content_type,
-            is_list=is_list,
         )
 
-    def _get_enocde_payload(self, **kwargs):
-        payload = get_base_payload('/encode', self.token, **kwargs)
-        is_list = False
+    def _get_rank_payload(self, **kwargs):
+        payload = get_base_payload('/rank', self.token, **kwargs)
 
         if 'docs' in kwargs:
             if 'text' in kwargs or 'image' in kwargs:
                 raise ValueError(
                     'More than one input type provided. Please provide only text, image or docs input.'
                 )
             content_type = 'docarray'
@@ -122,65 +115,63 @@
             payload.update(inputs=iter_doc(kwargs.pop('docs')))
 
         elif 'text' in kwargs:
             if 'image' in kwargs:
                 raise ValueError(
                     'Multi-modal input not supported. Please provide only text or image input.'
                 )
+            if 'candidates' not in kwargs:
+                raise ValueError(
+                    'Please provide candidates to rank against the text input.'
+                )
             content_type = 'plain'
             text_content = kwargs.pop('text')
             if isinstance(text_content, str):
-                is_list = False
                 text_doc = Document(text=text_content)
+                candidates = kwargs.pop('candidates')
+                text_doc.matches = DocumentArray(
+                    [load_plain_into_document(c) for c in candidates]
+                )
                 payload.update(inputs=DocumentArray([text_doc]))
                 payload.update(total_docs=1)
             else:
-                is_list = True
-                text_docs = DocumentArray([Document(text=c) for c in text_content])
-                payload.update(inputs=text_docs)
-                payload.update(total_docs=len(text_docs))
-                payload.update(results_in_order=True)
+                raise ValueError('Only single text input is supported.')
 
         elif 'image' in kwargs:
             if 'text' in kwargs:
                 raise ValueError(
                     'Multi-modal input not supported. Please provide only text or image input.'
                 )
+            if 'candidates' not in kwargs:
+                raise ValueError(
+                    'Please provide candidates to rank against the image input.'
+                )
             content_type = 'plain'
             image_content = kwargs.pop('image')
             if isinstance(image_content, (str, bytes, numpy.ndarray)):
-                is_list = False
                 image_doc = load_plain_into_document(image_content, mime_type='image')
+                candidates = kwargs.pop('candidates')
+                image_doc.matches = DocumentArray(
+                    [load_plain_into_document(c) for c in candidates]
+                )
                 payload.update(inputs=DocumentArray([image_doc]))
                 payload.update(total_docs=1)
             else:
-                is_list = True
-                image_docs = DocumentArray(
-                    [
-                        load_plain_into_document(c, mime_type='image')
-                        for c in image_content
-                    ]
-                )
-                payload.update(inputs=image_docs)
-                payload.update(total_docs=len(image_docs))
-                payload.update(results_in_order=True)
+                raise ValueError('Only single image input is supported.')
 
         else:
-            raise ValueError(
-                'Please provide either text, image or docs input to encode.'
-            )
+            raise ValueError('Please provide either text, image or docs input to rank.')
 
-        return payload, content_type, is_list
+        return payload, content_type
 
-    def _unbox_encode_result(
+    def _unbox_rank_result(
         self,
         result: 'DocumentArray' = None,
         content_type: str = 'docarray',
-        is_list: bool = False,
     ):
         if content_type == 'plain':
-            if is_list:
-                return result.embeddings
-            else:
-                return result[0].embedding
+            return [
+                (d.uri, d.scores) if d.uri else (d.content, d.scores)
+                for d in result[0].matches
+            ]
         else:
             return result
```

### Comparing `inference_client-0.0.6/inference_client/tasks/generate.py` & `inference_client-0.0.7/inference_client/tasks/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         do_sample: bool = False,
         temperature: float = 1.0,
         top_k: int = 1,
         top_p: float = 0.9,
         repetition_penalty: float = 1.0,
         length_penalty: float = 1.0,
         no_repeat_ngram_size: int = 0,
-        **kwargs
+        **kwargs,
     ):
         """Generate text from the given prompt.
 
         :param prompts: The prompt(s) to generate from.
         :param max_new_tokens: The maximum number of tokens to generate, not including the prompt.
         :param num_beams: Number of beams for beam search. 1 means no beam search.
         :param do_sample: Whether to use sampling instead of greedy decoding.
@@ -76,14 +76,31 @@
         """Generate text from the given prompt.
 
         :param prompts: The prompt(s) to generate from.
         :param kwargs: The arguments to pass to the model.
         :return: The generated text.
         """
         prompts = [prompts] if isinstance(prompts, str) else prompts
-        payload = get_base_payload('/generate', self.token, **kwargs)
+        payload = self._get_generate_payload(**kwargs)
         payload.update(
-            inputs=DocumentArray([Document(text=prompt) for prompt in prompts])
+            inputs=DocumentArray(
+                [Document(tags={'prompt': prompt}) for prompt in prompts]
+            )
         )
         result = self.client.post(**payload)
         text_out = [r.tags['generated_text'] or r.tags['response'] for r in result]
         return text_out if len(text_out) > 1 else text_out[0]
+
+    def _get_generate_payload(self, **kwargs):
+        """Get the payload for the generate endpoint.
+
+        :param kwargs: The arguments to pass to the model.
+        :return: The payload.
+        """
+        payload = get_base_payload('/generate', self.token, **kwargs)
+
+        if parameters := payload.get('parameters'):
+            parameters.update(kwargs)
+        else:
+            payload.update(parameters=kwargs)
+
+        return payload
```

### Comparing `inference_client-0.0.6/inference_client/tasks/helper.py` & `inference_client-0.0.7/inference_client/tasks/helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,15 +61,17 @@
 
     :param endpoint: the endpoint to send the request to
     :param token: user token
     :param kwargs: other parameters
     :return: a dict of payload containing the endpoint, token, request size and parameters
     """
     parameters = kwargs.pop('parameters', {})
-    parameters['drop_image_content'] = parameters.get('drop_image_content', True)
+
+    if endpoint != '/generate':
+        parameters['drop_image_content'] = parameters.get('drop_image_content', True)
     payload = dict(
         on=endpoint,
         request_size=kwargs.pop('request_size', 1),
         metadata=(('authorization', token),),
         parameters=parameters,
     )
     return payload
```

### Comparing `inference_client-0.0.6/inference_client/tasks/upscale.py` & `inference_client-0.0.7/inference_client/tasks/upscale.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.6/inference_client/tasks/vqa.py` & `inference_client-0.0.7/inference_client/tasks/vqa.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.6/pyproject.toml` & `inference_client-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inference_client"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python Client for Jina Inference API"
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
```

### Comparing `inference_client-0.0.6/PKG-INFO` & `inference_client-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-client
-Version: 0.0.6
+Version: 0.0.7
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
-Metadata-Version: 2.1 Name: inference-client Version: 0.0.6 Summary: Python
+Metadata-Version: 2.1 Name: inference-client Version: 0.0.7 Summary: Python
 Client for Jina Inference API Home-page: https://inference-api.jina.ai License:
 Apache-2.0 Keywords: jina,inference,api,client Author: Jina AI Author-email:
 hello@jina.ai Requires-Python: >=3.8,<4.0.0 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: pytorch
```

