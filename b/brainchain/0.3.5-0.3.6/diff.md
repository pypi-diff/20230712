# Comparing `tmp/brainchain-0.3.5.tar.gz` & `tmp/brainchain-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.3.5.tar", max compression
+gzip compressed data, was "brainchain-0.3.6.tar", max compression
```

## Comparing `brainchain-0.3.5.tar` & `brainchain-0.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.5/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.5/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.5/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.5/brainchain/__init__.py
--rw-r--r--   0        0        0     5887 2023-07-12 17:03:15.378203 brainchain-0.3.5/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.5/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.5/brainchain/coredata.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.5/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.5/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.5/brainchain/sales_intel.py
--rw-r--r--   0        0        0      532 2023-07-12 18:05:54.407374 brainchain-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.6/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.6/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.6/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.6/brainchain/__init__.py
+-rw-r--r--   0        0        0     6227 2023-07-12 20:03:29.941305 brainchain-0.3.6/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.6/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.6/brainchain/coredata.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.6/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.6/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.6/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      532 2023-07-12 19:57:30.932222 brainchain-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.3.6/PKG-INFO
```

### Comparing `brainchain-0.3.5/brainchain/.aider.chat.history.md` & `brainchain-0.3.6/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.5/brainchain/.aider.input.history` & `brainchain-0.3.6/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.5/brainchain/README.md` & `brainchain-0.3.6/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.5/brainchain/brainchain.py` & `brainchain-0.3.6/brainchain/brainchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,25 +13,18 @@
         self.sales_intel_client = SalesIntel(salesintel_api_key)
         self.environments = ["prod", "dev"]
         self.services = {
             "agent": {
                 "prod": "https://brainchain--agent.modal.run/",
                 "dev": "https://brainchain--agent-dev.modal.run/"
             },
-            "prompting": {
-                "prod": "https://brainchain--prompting.modal.run/",
-                "dev": "https://brainchain--prompting-dev.modal.run/"
-            },
-            "pdf_title": {
-                "prod": "https://brainchain--pdf-title.modal.run/",
-                "dev": "https://brainchain--pdf-title-dev.modal.run/"
-            },
-            "pdf_authors": {
-                "prod": "https://brainchain--pdf-authors.modal.run/",
-                "dev": "https://brainchain--pdf-authors-dev.modal.run/"
+            "prompt-completion-service": {
+                "prompting": "https://brainchain--prompt-completion-service-fastapi-app.modal.run/prompting",
+                "get_pdf_title": "https://brainchain--prompt-completion-service-fastapi-app.modal.run/get_pdf_title",
+                "get_pdf_authors": "https://brainchain--prompt-completion-service-fastapi-app.modal.run/get_pdf_authors"
             },
             "search": {
                 "prod": "https://brainchain--search.modal.run/",
                 "dev":  "https://brainchain--search-dev.modal.run/"
             },
             "electrolaser": {
                 "prod": "https://brainchain--electrolaser.modal.run/",
@@ -61,50 +54,58 @@
         params = {"query": query, "additional_pages": additional_pages}
         response = requests.get(endpoint, headers=headers, params=params)
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
+    def bullet_point_summarizer(self, text: str, prompt=""):
+        endpoint = self.services["electrolaser"][self.env]
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+        params = {"query": query, "additional_pages": additional_pages}
+        response = requests.get(endpoint, headers=headers, params=params)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            response.raise_for_status()
+
     def prompt(self, q, history=[], top_p=0.0, system="You are a multi-disciplinary research assistant who formulates, validates, and figures out correct answers. Your insights are ferocious and undeniable. You expand and digest new concepts and relate them to what you already know.", model="gpt-3.5-turbo-16k", presence_penalty=0.0, frequency_penalty=0.0, n=1):
-        endpoint = self.services["prompting"][self.env]
+        endpoint = self.services["prompt-completion-service"]["prompting"]
         headers = {"Authorization": f"Bearer {self.api_key}"}
-        params = {"user_prompt": q, "history": history, "system_prompt": system, "model": model, "presence_penalty": float(
+        payload = {"user_prompt": q, "history": history, "system_prompt": system, "model": model, "presence_penalty": float(
             presence_penalty), "frequency_penalty": float(frequency_penalty), "top_p": float(top_p)}
-        response = requests.get(endpoint, headers=headers, params=params)
+        response = requests.post(endpoint, headers=headers, json=payload)
 
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
     def obtain_title(self, text_first_page: str = None):
-        endpoint = self.services["pdf_title"][self.env]
+        endpoint = self.services["prompt-completion-service"]["get_pdf_title"]
         payload = {}
 
         if text_first_page:
             payload["document_text"] = text_first_page
     
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.post(endpoint, headers=headers, json=payload)
         content = response.content.decode('utf-8')
-        print(content)
         return json.loads(content)
 
     def obtain_authors(self, text_first_page: str = None):
-        endpoint = self.services["pdf_authors"][self.env]
+        endpoint =  self.services["prompt-completion-service"]["get_pdf_authors"]
         payload = {}
 
         if text_first_page:
             payload["document_text"] = text_first_page
 
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.post(endpoint, headers=headers, json=payload)
         content = response.content.decode('utf-8')
-        print(content)
         return json.loads(content)
 
     def summon(self, prompt, agent_type="CCR", model="gpt-4-0613", max_tokens=2048, temperature=0.18, top_p=0.15, top_k=0.0, presence_penalty=1.0, frequency_penalty=1.0):
         endpoint = self.services["agent"][self.env]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         params = {
             "prompt": prompt,
```

### Comparing `brainchain-0.3.5/brainchain/carnivore.py` & `brainchain-0.3.6/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.5/brainchain/coredata.py` & `brainchain-0.3.6/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.5/brainchain/factcheck.py` & `brainchain-0.3.6/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.5/brainchain/requirements.txt` & `brainchain-0.3.6/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.5/brainchain/sales_intel.py` & `brainchain-0.3.6/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.5/pyproject.toml` & `brainchain-0.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.3.5"
+version = "0.3.6"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.92"
 openai = "0.27.8"
-modal-client = "0.50.2570"
+modal-client = "0.50.2627"
 tiktoken = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `brainchain-0.3.5/PKG-INFO` & `brainchain-0.3.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.3.5
+Version: 0.3.6
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: modal-client (==0.50.2570)
+Requires-Dist: modal-client (==0.50.2627)
 Requires-Dist: openai (==0.27.8)
 Requires-Dist: promptlayer (==0.1.92)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
```

