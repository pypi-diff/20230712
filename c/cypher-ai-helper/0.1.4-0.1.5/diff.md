# Comparing `tmp/cypher_ai_helper-0.1.4.tar.gz` & `tmp/cypher_ai_helper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypher_ai_helper-0.1.4.tar", max compression
+gzip compressed data, was "cypher_ai_helper-0.1.5.tar", max compression
```

## Comparing `cypher_ai_helper-0.1.4.tar` & `cypher_ai_helper-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1076 2023-06-28 13:38:18.205144 cypher_ai_helper-0.1.4/LICENSE
--rw-r--r--   0        0        0     2487 2023-06-28 13:38:18.205144 cypher_ai_helper-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-28 13:38:18.205144 cypher_ai_helper-0.1.4/cypher_ai_helper/__init__.py
--rw-r--r--   0        0        0     7304 2023-06-28 13:38:18.205144 cypher_ai_helper-0.1.4/cypher_ai_helper/main.py
--rw-r--r--   0        0        0     1008 2023-06-28 13:38:18.205144 cypher_ai_helper-0.1.4/cypher_ai_helper/system_prompt
--rw-r--r--   0        0        0       81 2023-06-28 13:38:18.205144 cypher_ai_helper-0.1.4/cypher_ai_helper/user_prompt
--rw-r--r--   0        0        0     5390 2023-06-28 13:38:18.205144 cypher_ai_helper-0.1.4/cypher_ai_helper/utils.py
--rw-r--r--   0        0        0      941 2023-06-28 13:38:36.541894 cypher_ai_helper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 cypher_ai_helper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-12 05:56:31.890503 cypher_ai_helper-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2487 2023-07-12 05:56:31.890503 cypher_ai_helper-0.1.5/README.md
+-rw-r--r--   0        0        0       81 2023-07-12 05:56:31.890503 cypher_ai_helper-0.1.5/cypher_ai_helper/__init__.py
+-rw-r--r--   0        0        0     7527 2023-07-12 05:56:31.890503 cypher_ai_helper-0.1.5/cypher_ai_helper/main.py
+-rw-r--r--   0        0        0     1008 2023-07-12 05:56:31.890503 cypher_ai_helper-0.1.5/cypher_ai_helper/system_prompt
+-rw-r--r--   0        0        0       81 2023-07-12 05:56:31.890503 cypher_ai_helper-0.1.5/cypher_ai_helper/user_prompt
+-rw-r--r--   0        0        0     5390 2023-07-12 05:56:31.890503 cypher_ai_helper-0.1.5/cypher_ai_helper/utils.py
+-rw-r--r--   0        0        0      837 2023-07-12 05:56:52.038700 cypher_ai_helper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 cypher_ai_helper-0.1.5/PKG-INFO
```

### Comparing `cypher_ai_helper-0.1.4/LICENSE` & `cypher_ai_helper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cypher_ai_helper-0.1.4/README.md` & `cypher_ai_helper-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cypher_ai_helper-0.1.4/cypher_ai_helper/main.py` & `cypher_ai_helper-0.1.5/cypher_ai_helper/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,18 +109,23 @@
     :param func: Function to use to test the query
     :return:
     """
     global query_cache
 
     if overwrite_cache:
         del query_cache[query_id]
-
+    _result_query = None
     if query_id in query_cache:
         logger.debug(f"Returning cached query for {query_id}")
-        return query_cache[query_id]
+        _result_query = query_cache[query_id]
+
+    if _result_query is not None and func:
+        return _result_query, func(query=_result_query)
+    elif _result_query is not None:
+        return _result_query, None
 
     with open(os.path.join(curdir, "system_prompt"), "r") as f:
         _system_prompt = f.read()
     with open(os.path.join(curdir, "user_prompt"), "r") as f:
         _prompt = f.read()
     _prompt = _prompt.replace("{{schema}}", schema)
     _prompt = _prompt.replace("{{instruction}}", instruction)
@@ -131,23 +136,25 @@
         {"role": "user", "content": _prompt},
     ]
     _functions = None
 
     _response_message = _send_chat_messages(_messages, _model=model, functions=_functions)
     _messages.append(json.loads(json.dumps(_response_message, ensure_ascii=False)))
     logger.debug(f"Messages: {_messages}")
+    _result_query = _response_message["content"]
     _follow_up_messages = _messages
+    query_cache[query_id] = _result_query
     if func:
         _new_messages = []
         _functions = [func_to_json(func)]
         assert len(_functions[0]["parameters"]) > 0, "Function must have at least one parameter"
         _new_messages.append(
             {
                 "role": "user",
-                "content": f"Execute the the following query: {_response_message['content']}\n\n"
+                "content": f"Execute the the following query: {_result_query}\n\n"
                            f"Do not attempt to generate values for placeholders, just execute the query as is.",
             }
         )
         _response_message = _send_chat_messages(_new_messages, _model=model, functions=_functions)
         _new_messages.append(json.loads(json.dumps(_response_message, ensure_ascii=False)))
         logger.debug(f"Messages: {_new_messages}")
         _follow_up_messages = _new_messages
@@ -179,9 +186,8 @@
                 "role": "user",
                 "content": "The query failed. Please consider the error and rewrite the query."
             })
             _response_message = _send_chat_messages(_follow_up_messages, _model=model, functions=_functions)
 
     logger.debug(f"Messages: {_follow_up_messages}")
     logger.debug(f"LLM Query Response: {_response_message}")
-    query_cache[query_id] = _response_message["content"]
     return _response_message["content"], None
```

### Comparing `cypher_ai_helper-0.1.4/cypher_ai_helper/system_prompt` & `cypher_ai_helper-0.1.5/cypher_ai_helper/system_prompt`

 * *Files identical despite different names*

### Comparing `cypher_ai_helper-0.1.4/cypher_ai_helper/utils.py` & `cypher_ai_helper-0.1.5/cypher_ai_helper/utils.py`

 * *Files identical despite different names*

### Comparing `cypher_ai_helper-0.1.4/PKG-INFO` & `cypher_ai_helper-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cypher-ai-helper
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple helper to create and execute Cypher queries for Neo4j
 License: MIT
 Author: Trayan Azarov
 Author-email: trayan.azarov@amikos.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

