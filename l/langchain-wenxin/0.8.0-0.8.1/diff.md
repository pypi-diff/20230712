# Comparing `tmp/langchain_wenxin-0.8.0.tar.gz` & `tmp/langchain_wenxin-0.8.1.tar.gz`

## Comparing `langchain_wenxin-0.8.0.tar` & `langchain_wenxin-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/examples/Langchain_wenxin_retrieval_qa_compared.ipynb
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/src/langchain_wenxin/__about__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/src/langchain_wenxin/__init__.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/src/langchain_wenxin/chat_models.py
--rw-r--r--   0        0        0    11065 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/src/langchain_wenxin/client.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/src/langchain_wenxin/embeddings.py
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/src/langchain_wenxin/llms.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/src/langchain_wenxin/retrievers.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/integration_tests/chat_models/__init__.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/integration_tests/chat_models/test_wenxin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/integration_tests/embeddings/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/integration_tests/embeddings/test_wenxin.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/integration_tests/llms/__init__.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/integration_tests/llms/test_wenxin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/tools/__init__.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/tests/tools/test_callbacks.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/README.md
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/examples/Langchain_wenxin_retrieval_qa_compared.ipynb
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/src/langchain_wenxin/__about__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/src/langchain_wenxin/__init__.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/src/langchain_wenxin/chat_models.py
+-rw-r--r--   0        0        0    11065 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/src/langchain_wenxin/client.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/src/langchain_wenxin/embeddings.py
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/src/langchain_wenxin/llms.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/src/langchain_wenxin/retrievers.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/integration_tests/chat_models/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/integration_tests/chat_models/test_wenxin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/integration_tests/embeddings/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/integration_tests/embeddings/test_wenxin.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/integration_tests/llms/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/integration_tests/llms/test_wenxin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/tools/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/tests/tools/test_callbacks.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/LICENSE.txt
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/README.md
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.1/PKG-INFO
```

### Comparing `langchain_wenxin-0.8.0/examples/Langchain_wenxin_retrieval_qa_compared.ipynb` & `langchain_wenxin-0.8.1/examples/Langchain_wenxin_retrieval_qa_compared.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/src/langchain_wenxin/chat_models.py` & `langchain_wenxin-0.8.1/src/langchain_wenxin/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/src/langchain_wenxin/client.py` & `langchain_wenxin-0.8.1/src/langchain_wenxin/client.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/src/langchain_wenxin/embeddings.py` & `langchain_wenxin-0.8.1/src/langchain_wenxin/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/src/langchain_wenxin/llms.py` & `langchain_wenxin-0.8.1/src/langchain_wenxin/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/src/langchain_wenxin/retrievers.py` & `langchain_wenxin-0.8.1/src/langchain_wenxin/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/tests/integration_tests/chat_models/test_wenxin.py` & `langchain_wenxin-0.8.1/tests/integration_tests/chat_models/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/tests/integration_tests/embeddings/test_wenxin.py` & `langchain_wenxin-0.8.1/tests/integration_tests/embeddings/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/tests/integration_tests/llms/test_wenxin.py` & `langchain_wenxin-0.8.1/tests/integration_tests/llms/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/tests/tools/test_callbacks.py` & `langchain_wenxin-0.8.1/tests/tools/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/.gitignore` & `langchain_wenxin-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/LICENSE.txt` & `langchain_wenxin-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/README.md` & `langchain_wenxin-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/pyproject.toml` & `langchain_wenxin-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.0/PKG-INFO` & `langchain_wenxin-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-wenxin
-Version: 0.8.0
+Version: 0.8.1
 Project-URL: Documentation, https://github.com/ninehills/langchain-wenxin#readme
 Project-URL: Issues, https://github.com/ninehills/langchain-wenxin/issues
 Project-URL: Source, https://github.com/ninehills/langchain-wenxin
 Author-email: Tao Yang <swulling@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

