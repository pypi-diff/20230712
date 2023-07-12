# Comparing `tmp/chatgpt-klient-0.0.5.tar.gz` & `tmp/chatgpt-klient-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-klient-0.0.5.tar", last modified: Tue Jul 11 11:28:06 2023, max compression
+gzip compressed data, was "chatgpt-klient-0.0.6.tar", last modified: Wed Jul 12 10:16:16 2023, max compression
```

## Comparing `chatgpt-klient-0.0.5.tar` & `chatgpt-klient-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 11:28:06.829171 chatgpt-klient-0.0.5/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-11 11:28:06.829171 chatgpt-klient-0.0.5/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.0.5/README.md
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-07-11 11:26:47.000000 chatgpt-klient-0.0.5/pyproject.toml
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-11 11:28:06.829171 chatgpt-klient-0.0.5/setup.cfg
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 11:28:06.821171 chatgpt-klient-0.0.5/src/
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 11:28:06.825171 chatgpt-klient-0.0.5/src/chatgpt_klient/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-07-11 11:26:56.000000 chatgpt-klient-0.0.5/src/chatgpt_klient/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5640 2023-07-11 11:26:05.000000 chatgpt-klient-0.0.5/src/chatgpt_klient/client.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt-klient-0.0.5/src/chatgpt_klient/consts.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-11 11:28:06.829171 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      322 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/requires.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-07-11 11:28:06.000000 chatgpt-klient-0.0.5/src/chatgpt_klient.egg-info/top_level.txt
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-12 10:16:16.702738 chatgpt-klient-0.0.6/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-12 10:16:16.702738 chatgpt-klient-0.0.6/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.0.6/README.md
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-07-12 10:12:59.000000 chatgpt-klient-0.0.6/pyproject.toml
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-12 10:16:16.702738 chatgpt-klient-0.0.6/setup.cfg
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-12 10:16:16.698738 chatgpt-klient-0.0.6/src/
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-12 10:16:16.698738 chatgpt-klient-0.0.6/src/chatgpt_klient/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-07-12 10:12:48.000000 chatgpt-klient-0.0.6/src/chatgpt_klient/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5594 2023-07-12 10:12:26.000000 chatgpt-klient-0.0.6/src/chatgpt_klient/client.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt-klient-0.0.6/src/chatgpt_klient/consts.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-12 10:16:16.702738 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      322 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/requires.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/top_level.txt
```

### Comparing `chatgpt-klient-0.0.5/src/chatgpt_klient/client.py` & `chatgpt-klient-0.0.6/src/chatgpt_klient/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,41 +42,39 @@
         )
 
     def clean_history(self):
         self.msg_history = {"messages": [], "tokens": []}
         self.last_prompt_tokens = 0
 
     def get_max_tokens_allowed(self):
-        return min(self.max_tokens, MAX_TOKENS[self.engine])
+        return min(self.max_tokens, MAX_TOKENS[self.engine]) - 10
 
     def send_prompt(self, text=None, max_tokens=None, no_history=False):
         response = "No response"
         if self.engine in ENGINES0:
             r = self.openai.Completion.create(
                 engine=self.engine,
                 prompt=text,
-                max_tokens=max_tokens or self.get_max_tokens_allowed(),
+                max_tokens=self.get_max_tokens_allowed(),
             )
             response = r["choices"][0]["text"]
         elif self.engine in ENGINES1:
             if text:
                 if no_history:
                     self.clean_history()
                 self.msg_history["messages"].append(
                     {
                         "role": "user",
                         "content": text,
                     }
                 )
                 self.msg_history["tokens"].append(len(self.encoding.encode(text)))
-            potential_tokens = (
-                self.msg_history["tokens"][-1] + self.last_prompt_tokens
-            ) + 10
+            potential_tokens = self.msg_history["tokens"][-1] + self.last_prompt_tokens
             logger.debug(f"Potential tokens: {potential_tokens}")
-            while potential_tokens > self.max_tokens:
+            while potential_tokens > self.get_max_tokens_allowed():
                 logger.warning("Too many tokens. Reducing history size")
                 aux = {"messages": [], "tokens": []}
                 first_user = True
                 first_assistant = True
                 for i in range(len(self.msg_history["messages"])):
                     if self.msg_history["messages"][i]["role"] == "user" and first_user:
                         first_user = False
@@ -92,15 +90,15 @@
                         aux["tokens"].append(self.msg_history["tokens"][i])
                 self.msg_history = aux
 
             try:
                 r = self.openai.ChatCompletion.create(
                     model=self.engine,
                     messages=self.msg_history["messages"],
-                    max_tokens=max_tokens or self.get_max_tokens_allowed(),
+                    max_tokens=self.get_max_tokens_allowed(),
                 )
                 logger.debug(r)
                 self.last_prompt_tokens = r["usage"]["total_tokens"]
                 response = r["choices"][0].message.content
             except openai.InvalidRequestError:
                 logger.exception("We shouldn't be getting here!")
```

### Comparing `chatgpt-klient-0.0.5/src/chatgpt_klient/consts.py` & `chatgpt-klient-0.0.6/src/chatgpt_klient/consts.py`

 * *Files identical despite different names*

