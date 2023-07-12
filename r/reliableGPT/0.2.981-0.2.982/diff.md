# Comparing `tmp/reliableGPT-0.2.981.tar.gz` & `tmp/reliableGPT-0.2.982.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.981.tar", last modified: Sat Jul  8 03:29:31 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.982.tar", last modified: Wed Jul 12 21:27:02 2023, max compression
```

## Comparing `reliableGPT-0.2.981.tar` & `reliableGPT-0.2.982.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:29:31.329740 reliableGPT-0.2.981/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.981/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 03:29:31.329597 reliableGPT-0.2.981/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8377 2023-07-08 02:45:37.000000 reliableGPT-0.2.981/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.981/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:29:31.328010 reliableGPT-0.2.981/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      366 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-08 03:29:31.000000 reliableGPT-0.2.981/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-08 03:29:31.329391 reliableGPT-0.2.981/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.981/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    18415 2023-07-08 02:52:42.000000 reliableGPT-0.2.981/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.981/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.981/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5208 2023-07-08 03:25:36.000000 reliableGPT-0.2.981/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.981/reliablegpt/reliableQuery.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-08 03:29:31.329808 reliableGPT-0.2.981/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-08 03:29:10.000000 reliableGPT-0.2.981/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:27:02.973633 reliableGPT-0.2.982/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.982/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-12 21:27:02.973507 reliableGPT-0.2.982/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8557 2023-07-11 03:10:54.000000 reliableGPT-0.2.982/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.982/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:27:02.971946 reliableGPT-0.2.982/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      337 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       63 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-12 21:27:02.000000 reliableGPT-0.2.982/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-12 21:27:02.973155 reliableGPT-0.2.982/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-07 02:48:09.000000 reliableGPT-0.2.982/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    19026 2023-07-12 21:23:16.000000 reliableGPT-0.2.982/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.982/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-08 03:07:22.000000 reliableGPT-0.2.982/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5325 2023-07-12 21:22:05.000000 reliableGPT-0.2.982/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-12 21:27:02.973683 reliableGPT-0.2.982/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      418 2023-07-12 21:26:48.000000 reliableGPT-0.2.982/setup.py
```

### Comparing `reliableGPT-0.2.981/LICENSE` & `reliableGPT-0.2.982/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.981/README.md` & `reliableGPT-0.2.982/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-# 💪 reliableGPT: Stop OpenAI Errors in Production 🚀
+# 💪 reliableGPT: Stop failing customer requests for your LLM App 🚀
+[![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
 
 ⚡️ Get 0 dropped requests for your LLM app in production ⚡️
 
-**Schedule a ReliableGPT onboarding meeting with the builders: [Meeting Scheduling Link](https://calendly.com/d/yr3-9zt-yy4/reliablegpt?month=2023-07)**
-
 When a request to your llm app fails, reliableGPT handles it by:
 * Retrying with an alternate model - GPT-4, GPT3.5, GPT3.5 16k, text-davinci-003
 * Retrying with a larger context window model for Context Window Errors
 * Sending a Cached Response (using semantic similarity)
 * Retry with a fallback API key for Invalid API Key errors 
 
+## Community 
+* Join us on [Discord](https://discord.gg/WXFfTeEXRh) or Email us at ishaan@berri.ai & krrish@berri.ai
+* **Talk to Founders: Learn more / get help onboarding: [Meeting Scheduling Link](https://calendly.com/d/yr3-9zt-yy4/reliablegpt?month=2023-07)**
+
+
 # Getting Started
 ## Step 1. pip install package
 ```
 pip install reliableGPT
 ```
 ## Step 2. The core package is 1 line of code
 Integrating with OpenAI, Azure OpenAI, Langchain, LlamaIndex
@@ -23,15 +27,14 @@
 ```
 
 ## Troubleshooting
 If you experience failure, try 
 ```
 pip install reliableGPT==0.2.976
 ```
-Call/Text Ishaan at +14126186238
 
 ## 👉 Code Examples
 * [reliableGPT Getting Started](https://colab.research.google.com/drive/1za1eU6EXLlW4UjHy_YYSc7veDeGTvLON?usp=sharing)
 * [reliableGPT (Advanced) OpenAI Key Manager](https://colab.research.google.com/drive/1xW-fTKjIQyVvhPLo5MWFCY7YlaMxBy_v?usp=sharing)
 
 ![ezgif com-optimize](https://github.com/BerriAI/reliableGPT/assets/17561003/017046b0-0044-4df3-a740-d5edd9e23738)
```

### Comparing `reliableGPT-0.2.981/reliablegpt/Alerting.py` & `reliableGPT-0.2.982/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.981/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.982/reliablegpt/IndividualRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,55 +7,61 @@
 import traceback
 from uuid import uuid4
 from waitress import serve
 from flask import Flask, request
 from uuid import uuid4
 import traceback
 from threading import active_count
+import random 
+
+## for testing
+class CustomError(Exception):
+    def __init__(self, error):
+        self.error = error
+
 
 class IndividualRequest:
   """A brief description of the class."""
 
   def __init__(self,
                model=None,
-               app: Flask=None,
                fallback_strategy=[
                  'gpt-3.5-turbo', 'text-davinci-003', 'gpt-4',
                  'text-davinci-002'
                ],
+               azure_fallback_strategy=None,
                graceful_string="Sorry, the OpenAI API is currently down",
                user_email="",
                user_token="",
                send_notification=False,
                logging_fn=None,
                backup_openai_key="",
                caching=False,
                alerting=None,
                max_threads=None,
+               _test=False,
                verbose=False):
     # Initialize instance variables
     self.model = model
     self.model_function = model.get_model_function()
     self.verbose = verbose
     self.graceful_string = graceful_string
     self.fallback_strategy = fallback_strategy
     self.user_email = user_email
     self.user_token = user_token
     self.save_request = logging_fn
     self.backup_openai_key = backup_openai_key
+    self._test = _test
     self.print_verbose(f"INIT fallback strategy {self.fallback_strategy}")
     self.caching = caching
     self.max_threads = max_threads
     self.print_verbose(f"INIT with threads {self.max_threads} {self.caching} {max_threads}")
     self.alerting = alerting
-    self.app = app
-    if self.app:
-      self.app.register_error_handler(Exception, self.handle_unhandled_exception)
-      self.app.register_error_handler(500, self.handle_unhandled_exception)
-  
+    self.azure_fallback_strategy = azure_fallback_strategy
+
   def handle_unhandled_exception(self, e):
     self.print_verbose(colored("UNHANDLED EXCEPTION OCCURRED", "red"))
     if self.alerting:
       self.alerting.add_error(error_type="Unhandled Exception", error_description=traceback.format_exc())
 
   def print_verbose(self, print_statement):
     if self.verbose:
@@ -63,25 +69,29 @@
 
   ## Code that handles / wraps openai calls
   def __call__(self, *args, **kwargs):
     try:
       self.print_verbose(f"calling model function: {self.model_function}")
       self.print_verbose(f"these are the kwargs: {kwargs}")
       self.print_verbose(f"this is the openai api base: {openai.api_base}")
+      self.print_verbose(f"testing enabled: {self._test}")
       try:
         # this should never block running the openai call
         # [TODO] make this into a threaded call to reduce impact on latency
         self.save_request(
           user_email=self.user_email,
           graceful_string=self.graceful_string,
           posthog_event='reliableGPT.request',
         )
       except:
         print("ReliableGPT error occured during saving request")
       self.print_verbose(f"max threads: {self.max_threads}, caching: {self.caching}")
+      if self._test:
+        error = {"type": "RandomError"}
+        raise CustomError(error)
       if self.max_threads and self.caching:
         self.print_verbose(f'current util: {active_count()/self.max_threads}')
         thread_utilization = active_count()/self.max_threads
         self.print_verbose(f"Thread utilization: {thread_utilization}")
         if thread_utilization > 0.8: # over 80% utilization of threads, start returning cached responses
           if "messages" in kwargs and self.caching:
             print(kwargs["messages"])
@@ -192,14 +202,22 @@
       ) > 0:  # user passed in a backup key for the raw openai endpoint
         # switch to the raw openai model instead of using azure.
         new_kwargs["openai2"] = openai.__dict__.copy(
         )  # preserve the azure endpoint details
         if "Embedding" in str(self.model_function):
           fallback_strategy = ["text-embedding-ada-002"]
 
+      if self.azure_fallback_strategy: # try backup azure models
+        for engine in self.azure_fallback_strategy:
+          new_kwargs["engine"] = engine
+          self.print_verbose(f"new azure engine: {new_kwargs}")
+          result = self.make_LLM_request(new_kwargs)
+          if result != None:
+            return result
+        
       for model in fallback_strategy:
         new_kwargs['model'] = model  # Update the model
         result = self.make_LLM_request(new_kwargs)
         if result != None:
           return result
       return None
     except:
@@ -208,14 +226,16 @@
 
   def make_LLM_request(self, new_kwargs):
     embedding_model = self.model.get_original_embeddings()
     chat_model = self.model.get_original_chat()
     completion_model = self.model.get_original_completion()
     try:
       self.print_verbose(f"{new_kwargs.keys()}")
+      if "engine" in new_kwargs:
+        return chat_model(**new_kwargs)
       if "openai2" in new_kwargs:
         openai.api_type = "openai"
         openai.api_base = "https://api.openai.com/v1"
         openai.api_version = None
         openai.api_key = self.backup_openai_key
         new_kwargs_except_openai_attributes = {
           k: v
```

### Comparing `reliableGPT-0.2.981/reliablegpt/Model.py` & `reliableGPT-0.2.982/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.981/reliablegpt/main.py` & `reliableGPT-0.2.982/reliablegpt/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,25 +86,26 @@
         alerting.add_error(error)
       # send_emails_task(self.user_email, posthog_metadata, self.send_notification)
   except:
     return  # safe function, should not impact error handling if logging fails
 
 
 def reliableGPT(openai_create_function,
-            app: Flask=None,
            fallback_strategy=[
              'gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'
            ],
+           azure_fallback_strategy=None,
            graceful_string="Sorry, the OpenAI API is currently down",
            user_email="",
            user_token="",
            send_notification=True,
            caching=False,
            max_threads=None,
            backup_openai_key=None,
+           _test=False,
            verbose=False):
   """Determine if an instantiation is calling the rate limit handler or the individual request wrapper directly and return the correct object"""
 
   primary_email = ""  # which api key management is mapped to
   ## Add email for alerting
   if isinstance(user_email, str):
     if user_email == "":
@@ -116,19 +117,20 @@
     primary_email = user_email[0]
     for email in user_email:
       alerting.add_emails(email)
 
   model = Model(openai_create_function)
   ## Route to the right object
   return IndividualRequest(model,
-                            app=app,
                             fallback_strategy=fallback_strategy,
+                            azure_fallback_strategy=azure_fallback_strategy,
                             graceful_string=graceful_string,
                             user_email=primary_email,
                             user_token=user_token,
                             logging_fn=save_request,
                             send_notification=send_notification,
                             backup_openai_key=backup_openai_key, 
                             caching=caching,
                             max_threads=max_threads,
                             alerting=alerting,
+                            _test=_test,
                             verbose=verbose)
```

