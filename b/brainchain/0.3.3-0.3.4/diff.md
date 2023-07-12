# Comparing `tmp/brainchain-0.3.3.tar.gz` & `tmp/brainchain-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.3.3.tar", max compression
+gzip compressed data, was "brainchain-0.3.4.tar", max compression
```

## Comparing `brainchain-0.3.3.tar` & `brainchain-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.3/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.3/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.3/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.3/brainchain/__init__.py
--rw-r--r--   0        0        0     5886 2023-07-12 16:52:25.374976 brainchain-0.3.3/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.3/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.3/brainchain/coredata.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.3/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.3/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.3/brainchain/sales_intel.py
--rw-r--r--   0        0        0      531 2023-07-12 16:44:54.260915 brainchain-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.4/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.4/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.4/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.4/brainchain/__init__.py
+-rw-r--r--   0        0        0     5887 2023-07-12 17:03:15.378203 brainchain-0.3.4/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.4/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.4/brainchain/coredata.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.4/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.4/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.4/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      526 2023-07-12 18:01:46.777134 brainchain-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 brainchain-0.3.4/PKG-INFO
```

### Comparing `brainchain-0.3.3/brainchain/.aider.chat.history.md` & `brainchain-0.3.4/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.3/brainchain/.aider.input.history` & `brainchain-0.3.4/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.3/brainchain/README.md` & `brainchain-0.3.4/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.3/brainchain/brainchain.py` & `brainchain-0.3.4/brainchain/brainchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,18 @@
         params = {"query": query}
         response = requests.get(endpoint, headers=headers, params=params)
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
-    def search_results(self, query: str, additional_pages: int = 3):
+    def search_results(self, query: str, additional_pages: int = 10):
         return self.electrolaser(query, additional_pages=additional_pages)
 
-    def electrolaser(self, query: str, additional_pages: int = 90):
+    def electrolaser(self, query: str, additional_pages: int = 50):
         endpoint = self.services["electrolaser"][self.env]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         params = {"query": query, "additional_pages": additional_pages}
         response = requests.get(endpoint, headers=headers, params=params)
         if response.status_code == 200:
             return response.json()
         else:
```

### Comparing `brainchain-0.3.3/brainchain/carnivore.py` & `brainchain-0.3.4/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.3/brainchain/coredata.py` & `brainchain-0.3.4/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.3/brainchain/factcheck.py` & `brainchain-0.3.4/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.3/brainchain/requirements.txt` & `brainchain-0.3.4/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.3/brainchain/sales_intel.py` & `brainchain-0.3.4/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.3/pyproject.toml` & `brainchain-0.3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.3.3"
+version = "0.3.4"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
-promptlayer = "0.1.90"
+promptlayer = "^1.90"
 openai = "0.27.8"
-modal-client = "0.49.2437"
+modal-client = "^0.50"
 tiktoken = "0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `brainchain-0.3.3/PKG-INFO` & `brainchain-0.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.3.3
+Version: 0.3.4
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: modal-client (==0.49.2437)
+Requires-Dist: modal-client (>=0.50,<0.51)
 Requires-Dist: openai (==0.27.8)
-Requires-Dist: promptlayer (==0.1.90)
+Requires-Dist: promptlayer (>=1.90,<2.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: tiktoken (==0.4.0)
```

