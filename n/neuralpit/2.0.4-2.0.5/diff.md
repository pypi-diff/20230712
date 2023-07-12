# Comparing `tmp/neuralpit-2.0.4.tar.gz` & `tmp/neuralpit-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-2.0.4.tar", last modified: Mon Jul 10 15:00:02 2023, max compression
+gzip compressed data, was "neuralpit-2.0.5.tar", last modified: Wed Jul 12 10:23:16 2023, max compression
```

## Comparing `neuralpit-2.0.4.tar` & `neuralpit-2.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:00:02.801541 neuralpit-2.0.4/
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 14:59:33.000000 neuralpit-2.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-10 15:00:02.801541 neuralpit-2.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-10 14:59:33.000000 neuralpit-2.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-10 14:59:33.000000 neuralpit-2.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 15:00:02.801541 neuralpit-2.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:00:02.797541 neuralpit-2.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:00:02.801541 neuralpit-2.0.4/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      586 2023-07-10 14:59:33.000000 neuralpit-2.0.4/src/neuralpit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:00:02.801541 neuralpit-2.0.4/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:59:33.000000 neuralpit-2.0.4/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3720 2023-07-10 14:59:33.000000 neuralpit-2.0.4/src/neuralpit/services/conversation.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-10 14:59:33.000000 neuralpit-2.0.4/src/neuralpit/services/conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:00:02.801541 neuralpit-2.0.4/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-10 15:00:02.000000 neuralpit-2.0.4/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-10 15:00:02.000000 neuralpit-2.0.4/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 15:00:02.000000 neuralpit-2.0.4/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-10 15:00:02.000000 neuralpit-2.0.4/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-10 15:00:02.000000 neuralpit-2.0.4/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 15:00:02.801541 neuralpit-2.0.4/test/
--rw-r--r--   0 root         (0) root         (0)      411 2023-07-10 14:59:33.000000 neuralpit-2.0.4/test/testCreateConversation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:22:45.000000 neuralpit-2.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-12 10:23:16.070674 neuralpit-2.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-12 10:22:45.000000 neuralpit-2.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-12 10:22:45.000000 neuralpit-2.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:23:16.070674 neuralpit-2.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.066674 neuralpit-2.0.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-12 10:22:45.000000 neuralpit-2.0.5/src/neuralpit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:22:45.000000 neuralpit-2.0.5/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-07-12 10:22:45.000000 neuralpit-2.0.5/src/neuralpit/services/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-12 10:22:45.000000 neuralpit-2.0.5/src/neuralpit/services/conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/test/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-07-12 10:22:45.000000 neuralpit-2.0.5/test/testCreateConversation.py
```

### Comparing `neuralpit-2.0.4/PKG-INFO` & `neuralpit-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.0.4
+Version: 2.0.5
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-2.0.4/pyproject.toml` & `neuralpit-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "2.0.4"
+version = "2.0.5"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-2.0.4/src/neuralpit/__init__.py` & `neuralpit-2.0.5/src/neuralpit/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.0.4/src/neuralpit/services/conversation.py` & `neuralpit-2.0.5/src/neuralpit/services/conversation.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,19 +58,19 @@
     def listConversationHistory(self, conversation_id):
         get_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/history')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
         get_call = requests.get(get_url, headers = headers)
         resp =  json.loads(get_call.content)
         return resp
     
-    def queryConversation(self, conversation_id, question):
+    def queryConversation(self, conversation_id, question, debug=False):
         post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/query')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
-        post_call = requests.post(post_url, headers = headers, json = {'question': question})
+        post_call = requests.post(post_url, headers = headers, json = {'question': question, 'debug': debug})
         resp =  json.loads(post_call.content)
         return resp
     
-    def summarizeDocument(self, conversation_id, document_id):
+    def summarizeDocument(self, conversation_id, document_id, debug=False):
         get_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/document/{document_id}/summarize')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
-        post_call = requests.get(get_url, headers = headers)
+        post_call = requests.get(get_url, headers = headers, json = {'debug': debug})
         return post_call.content
```

### Comparing `neuralpit-2.0.4/src/neuralpit/services/conversion.py` & `neuralpit-2.0.5/src/neuralpit/services/conversion.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.0.4/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-2.0.5/src/neuralpit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.0.4
+Version: 2.0.5
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

