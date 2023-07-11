# Comparing `tmp/doctran-0.0.7.tar.gz` & `tmp/doctran-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran-0.0.7.tar", max compression
+gzip compressed data, was "doctran-0.0.8.tar", max compression
```

## Comparing `doctran-0.0.7.tar` & `doctran-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.7/LICENSE
--rw-r--r--   0        0        0     8124 2023-07-07 20:26:59.304557 doctran-0.0.7/README.md
--rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.7/doctran/__init__.py
--rw-r--r--   0        0        0     7518 2023-07-11 00:11:18.356609 doctran-0.0.7/doctran/doctran.py
--rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.7/doctran/transformers/__init__.py
--rw-r--r--   0        0        0      413 2023-07-01 18:31:07.391598 doctran-0.0.7/doctran/transformers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      411 2023-07-11 00:16:06.632372 doctran-0.0.7/doctran/transformers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8900 2023-06-30 02:26:08.286700 doctran-0.0.7/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc
--rw-r--r--   0        0        0      462 2023-06-29 15:35:41.652339 doctran-0.0.7/doctran/transformers/__pycache__/prompts.cpython-310.pyc
--rw-r--r--   0        0        0    10859 2023-07-09 20:04:35.149795 doctran-0.0.7/doctran/transformers/__pycache__/transformers.cpython-310.pyc
--rw-r--r--   0        0        0    10892 2023-07-11 00:16:06.634804 doctran-0.0.7/doctran/transformers/__pycache__/transformers.cpython-38.pyc
--rw-r--r--   0        0        0    12087 2023-07-11 00:15:16.180171 doctran-0.0.7/doctran/transformers/transformers.py
--rw-r--r--   0        0        0      587 2023-07-11 00:17:30.635351 doctran-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8877 1970-01-01 00:00:00.000000 doctran-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.8/LICENSE
+-rw-r--r--   0        0        0     8124 2023-07-07 20:26:59.304557 doctran-0.0.8/README.md
+-rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.8/doctran/__init__.py
+-rw-r--r--   0        0        0     7295 2023-07-11 23:03:46.240318 doctran-0.0.8/doctran/doctran.py
+-rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.8/doctran/transformers/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-01 18:31:07.391598 doctran-0.0.8/doctran/transformers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      411 2023-07-11 00:16:06.632372 doctran-0.0.8/doctran/transformers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8900 2023-06-30 02:26:08.286700 doctran-0.0.8/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc
+-rw-r--r--   0        0        0      462 2023-06-29 15:35:41.652339 doctran-0.0.8/doctran/transformers/__pycache__/prompts.cpython-310.pyc
+-rw-r--r--   0        0        0    10859 2023-07-09 20:04:35.149795 doctran-0.0.8/doctran/transformers/__pycache__/transformers.cpython-310.pyc
+-rw-r--r--   0        0        0    10892 2023-07-11 00:16:06.634804 doctran-0.0.8/doctran/transformers/__pycache__/transformers.cpython-38.pyc
+-rw-r--r--   0        0        0    12087 2023-07-11 00:15:16.180171 doctran-0.0.8/doctran/transformers/transformers.py
+-rw-r--r--   0        0        0      587 2023-07-11 23:03:06.921593 doctran-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8877 1970-01-01 00:00:00.000000 doctran-0.0.8/PKG-INFO
```

### Comparing `doctran-0.0.7/LICENSE` & `doctran-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran-0.0.7/README.md` & `doctran-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `doctran-0.0.7/doctran/doctran.py` & `doctran-0.0.8/doctran/doctran.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,28 +157,23 @@
 
     def interrogate(self) -> 'DocumentTransformationBuilder':
         self.transformations.append((Transformation.interrogate, {}))
         return self
 
 
 class Doctran:
-    def __init__(self, openai_api_key: str = None, openai_model: str = "gpt-4", openai_token_limit: int = 8000):
+    def __init__(self, openai_api_key: str, openai_model: str = "gpt-4", openai_token_limit: int = 8000):
         self.config = DoctranConfig(
             openai_api_key=openai_api_key,
             openai_model=openai_model,
             openai_completions_url="https://api.openai.com/v1/completions",
             openai=openai,
             openai_token_limit=openai_token_limit
         )
-        if openai_api_key:
-            self.config.openai.api_key = openai_api_key
-        elif os.environ["OPENAI_API_KEY"]:
-            self.config.openai.api_key = os.environ["OPENAI_API_KEY"]
-        else:
-            raise Exception("No OpenAI API Key provided")
+        self.config.openai.api_key = openai_api_key
 
     def parse(self, *, content: str, content_type: ContentType = "text", uri: str = None, metadata: dict = None) -> Document:
         '''
         Parse raw text and apply different chunking schemes based on the content type.
 
         Returns:
             Document: the parsed content represented as a Doctran Document
```

### Comparing `doctran-0.0.7/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc` & `doctran-0.0.8/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `doctran-0.0.7/doctran/transformers/__pycache__/transformers.cpython-310.pyc` & `doctran-0.0.8/doctran/transformers/__pycache__/transformers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `doctran-0.0.7/doctran/transformers/__pycache__/transformers.cpython-38.pyc` & `doctran-0.0.8/doctran/transformers/__pycache__/transformers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `doctran-0.0.7/doctran/transformers/transformers.py` & `doctran-0.0.8/doctran/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `doctran-0.0.7/pyproject.toml` & `doctran-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doctran"
-version = "0.0.7"
+version = "0.0.8"
 description = "Document transformation framework for vector based retrieval"
 authors = ["Jason Fan <jason.wc.fan@gmail.com>", "Ayan Bandyopadhyay <ayanb9440@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pydantic = "^1.10.9"
```

### Comparing `doctran-0.0.7/PKG-INFO` & `doctran-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doctran
-Version: 0.0.7
+Version: 0.0.8
 Summary: Document transformation framework for vector based retrieval
 Author: Jason Fan
 Author-email: jason.wc.fan@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: doctran Version: 0.0.7 Summary: Document
+Metadata-Version: 2.1 Name: doctran Version: 0.0.8 Summary: Document
 transformation framework for vector based retrieval Author: Jason Fan Author-
 email: jason.wc.fan@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0) Requires-Dist: presidio-analyzer
 (>=2.2.33,<3.0.0) Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
```

