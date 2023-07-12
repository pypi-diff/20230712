# Comparing `tmp/brainchain-0.3.1.tar.gz` & `tmp/brainchain-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.3.1.tar", max compression
+gzip compressed data, was "brainchain-0.3.3.tar", max compression
```

## Comparing `brainchain-0.3.1.tar` & `brainchain-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.1/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.1/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.1/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.1/brainchain/__init__.py
--rw-r--r--   0        0        0     4652 2023-07-11 23:19:08.256252 brainchain-0.3.1/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.1/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.1/brainchain/coredata.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.1/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.1/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.1/brainchain/sales_intel.py
--rw-r--r--   0        0        0      531 2023-07-11 23:18:28.733790 brainchain-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.3/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.3/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.3/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.3/brainchain/__init__.py
+-rw-r--r--   0        0        0     5886 2023-07-12 16:52:25.374976 brainchain-0.3.3/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.3/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.3/brainchain/coredata.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.3/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.3/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.3/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      531 2023-07-12 16:44:54.260915 brainchain-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.3.3/PKG-INFO
```

### Comparing `brainchain-0.3.1/brainchain/.aider.chat.history.md` & `brainchain-0.3.3/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.1/brainchain/.aider.input.history` & `brainchain-0.3.3/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.1/brainchain/README.md` & `brainchain-0.3.3/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.1/brainchain/brainchain.py` & `brainchain-0.3.3/brainchain/brainchain.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 class Brainchain:
     def __init__(self, env: str = "prod", api_key: str = os.environ["BRAINCHAIN_API_KEY"], service_url="https://brainchain--agent.modal.run/", salesintel_api_key=os.environ["SALESINTEL_API_KEY"]):
         self.api_key = api_key
         self.env = env
         self.fact_check_instance = FactCheck(environment=env)
         self.sales_intel_client = SalesIntel(salesintel_api_key)
-        self.search
         self.environments = ["prod", "dev"]
         self.services = {
             "agent": {
                 "prod": "https://brainchain--agent.modal.run/",
                 "dev": "https://brainchain--agent-dev.modal.run/"
             },
             "prompting": {
@@ -26,22 +25,49 @@
                 "prod": "https://brainchain--pdf-title.modal.run/",
                 "dev": "https://brainchain--pdf-title-dev.modal.run/"
             },
             "pdf_authors": {
                 "prod": "https://brainchain--pdf-authors.modal.run/",
                 "dev": "https://brainchain--pdf-authors-dev.modal.run/"
             },
-            "search": {}
+            "search": {
+                "prod": "https://brainchain--search.modal.run/",
+                "dev":  "https://brainchain--search-dev.modal.run/"
+            },
+            "electrolaser": {
+                "prod": "https://brainchain--electrolaser.modal.run/",
+                "dev": "https://brainchain--electrolaser-dev.modal.run/"
+            }
         }
 
     def fact_check(self, statement):
         return self.fact_check_instance.fact_check(statement)
 
     def search(self, query):
-        endpoint = self.services["search"]
+        endpoint = self.services["search"][self.env]
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+        params = {"query": query}
+        response = requests.get(endpoint, headers=headers, params=params)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            response.raise_for_status()
+
+    def search_results(self, query: str, additional_pages: int = 3):
+        return self.electrolaser(query, additional_pages=additional_pages)
+
+    def electrolaser(self, query: str, additional_pages: int = 90):
+        endpoint = self.services["electrolaser"][self.env]
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+        params = {"query": query, "additional_pages": additional_pages}
+        response = requests.get(endpoint, headers=headers, params=params)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            response.raise_for_status()
 
     def prompt(self, q, history=[], top_p=0.0, system="You are a multi-disciplinary research assistant who formulates, validates, and figures out correct answers. Your insights are ferocious and undeniable. You expand and digest new concepts and relate them to what you already know.", model="gpt-3.5-turbo-16k", presence_penalty=0.0, frequency_penalty=0.0, n=1):
         endpoint = self.services["prompting"][self.env]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         params = {"user_prompt": q, "history": history, "system_prompt": system, "model": model, "presence_penalty": float(
             presence_penalty), "frequency_penalty": float(frequency_penalty), "top_p": float(top_p)}
         response = requests.get(endpoint, headers=headers, params=params)
```

### Comparing `brainchain-0.3.1/brainchain/carnivore.py` & `brainchain-0.3.3/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.1/brainchain/coredata.py` & `brainchain-0.3.3/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.1/brainchain/factcheck.py` & `brainchain-0.3.3/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.1/brainchain/requirements.txt` & `brainchain-0.3.3/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.1/brainchain/sales_intel.py` & `brainchain-0.3.3/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.1/pyproject.toml` & `brainchain-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.3.1"
+version = "0.3.3"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.90"
```

### Comparing `brainchain-0.3.1/PKG-INFO` & `brainchain-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.3.1
+Version: 0.3.3
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

