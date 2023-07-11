# Comparing `tmp/superagent_py-0.0.31.tar.gz` & `tmp/superagent_py-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.0.31.tar", max compression
+gzip compressed data, was "superagent_py-0.0.32.tar", max compression
```

## Comparing `superagent_py-0.0.31.tar` & `superagent_py-0.0.32.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1073 2023-07-07 07:40:13.841999 superagent_py-0.0.31/LICENSE
--rw-r--r--   0        0        0     3169 2023-07-07 07:40:13.841999 superagent_py-0.0.31/README.md
--rw-r--r--   0        0        0      380 2023-07-07 07:40:13.841999 superagent_py-0.0.31/pyproject.toml
--rw-r--r--   0        0        0      589 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/__init__.py
--rw-r--r--   0        0        0     2963 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/py.typed
--rw-r--r--   0        0        0      343 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    13371 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/agent_documents/__init__.py
--rw-r--r--   0        0        0     8622 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/agent_documents/client.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/agent_tools/__init__.py
--rw-r--r--   0        0        0     8494 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/agent_tools/client.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     7900 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     5563 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0     9401 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10077 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0     8745 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2048 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-07-07 07:40:13.841999 superagent_py-0.0.31/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     3990 2023-07-07 07:40:13.845999 superagent_py-0.0.31/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-07-07 07:40:13.845999 superagent_py-0.0.31/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-07-07 07:40:13.845999 superagent_py-0.0.31/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-07-07 07:40:13.845999 superagent_py-0.0.31/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-07 07:40:13.845999 superagent_py-0.0.31/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3680 1970-01-01 00:00:00.000000 superagent_py-0.0.31/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-11 22:05:21.111118 superagent_py-0.0.32/LICENSE
+-rw-r--r--   0        0        0     3169 2023-07-11 22:05:21.111118 superagent_py-0.0.32/README.md
+-rw-r--r--   0        0        0      380 2023-07-11 22:05:21.111118 superagent_py-0.0.32/pyproject.toml
+-rw-r--r--   0        0        0      589 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/__init__.py
+-rw-r--r--   0        0        0     2963 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/py.typed
+-rw-r--r--   0        0        0      343 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    13371 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent_documents/__init__.py
+-rw-r--r--   0        0        0     8622 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent_documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent_tools/__init__.py
+-rw-r--r--   0        0        0     8494 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent_tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     7900 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     5563 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0     9401 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10077 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0     8745 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2048 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     3990 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3680 1970-01-01 00:00:00.000000 superagent_py-0.0.32/PKG-INFO
```

### Comparing `superagent_py-0.0.31/LICENSE` & `superagent_py-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/README.md` & `superagent_py-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/__init__.py` & `superagent_py-0.0.32/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/client.py` & `superagent_py-0.0.32/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/core/datetime_utils.py` & `superagent_py-0.0.32/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.0.32/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/agent/client.py` & `superagent_py-0.0.32/src/superagent/resources/agent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/agent_documents/client.py` & `superagent_py-0.0.32/src/superagent/resources/agent_documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/agent_tools/client.py` & `superagent_py-0.0.32/src/superagent/resources/agent_tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/api_token/client.py` & `superagent_py-0.0.32/src/superagent/resources/api_token/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/auth/client.py` & `superagent_py-0.0.32/src/superagent/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/documents/client.py` & `superagent_py-0.0.32/src/superagent/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/prompts/client.py` & `superagent_py-0.0.32/src/superagent/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/tools/client.py` & `superagent_py-0.0.32/src/superagent/resources/tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/traces/client.py` & `superagent_py-0.0.32/src/superagent/resources/traces/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/resources/user/client.py` & `superagent_py-0.0.32/src/superagent/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/types/http_validation_error.py` & `superagent_py-0.0.32/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/src/superagent/types/validation_error.py` & `superagent_py-0.0.32/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.31/PKG-INFO` & `superagent_py-0.0.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.0.31
+Version: 0.0.32
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

