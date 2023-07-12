# Comparing `tmp/langfuse-0.0.2.tar.gz` & `tmp/langfuse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfuse-0.0.2.tar", max compression
+gzip compressed data, was "langfuse-0.0.3.tar", max compression
```

## Comparing `langfuse-0.0.2.tar` & `langfuse-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     3693 2023-07-12 11:28:38.262604 langfuse-0.0.2/README.md
--rw-r--r--   0        0        0      152 2023-07-12 11:28:38.839985 langfuse-0.0.2/langfuse/__init__.py
--rw-r--r--   0        0        0       47 2023-07-12 11:28:38.302195 langfuse-0.0.2/langfuse/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.307846 langfuse-0.0.2/langfuse/api/event/__init__.py
--rw-r--r--   0        0        0     4794 2023-07-12 11:28:38.860217 langfuse-0.0.2/langfuse/api/event/event_create.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.319025 langfuse-0.0.2/langfuse/api/generations/__init__.py
--rw-r--r--   0        0        0     4557 2023-07-12 11:28:38.871136 langfuse-0.0.2/langfuse/api/generations/generations_log.py
--rw-r--r--   0        0        0     4713 2023-07-12 11:28:38.863639 langfuse-0.0.2/langfuse/api/generations/generations_update.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.320137 langfuse-0.0.2/langfuse/api/score/__init__.py
--rw-r--r--   0        0        0     4790 2023-07-12 11:28:38.867895 langfuse-0.0.2/langfuse/api/score/score_create.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.320737 langfuse-0.0.2/langfuse/api/span/__init__.py
--rw-r--r--   0        0        0     4761 2023-07-12 11:28:38.866173 langfuse-0.0.2/langfuse/api/span/span_create.py
--rw-r--r--   0        0        0     4774 2023-07-12 11:28:38.871407 langfuse-0.0.2/langfuse/api/span/span_update.py
--rw-r--r--   0        0        0        0 2023-07-12 11:28:38.321803 langfuse-0.0.2/langfuse/api/trace/__init__.py
--rw-r--r--   0        0        0     4790 2023-07-12 11:28:38.881219 langfuse-0.0.2/langfuse/api/trace/trace_create.py
--rw-r--r--   0        0        0     2817 2023-07-12 11:28:38.860072 langfuse-0.0.2/langfuse/client.py
--rw-r--r--   0        0        0      470 2023-07-12 11:28:38.866826 langfuse-0.0.2/langfuse/errors.py
--rw-r--r--   0        0        0     1457 2023-07-12 11:56:10.548759 langfuse-0.0.2/langfuse/langfuse.py
--rw-r--r--   0        0        0     1728 2023-07-12 11:28:38.301226 langfuse-0.0.2/langfuse/models/__init__.py
--rw-r--r--   0        0        0     5412 2023-07-12 11:28:38.897239 langfuse-0.0.2/langfuse/models/create_event_request.py
--rw-r--r--   0        0        0     9118 2023-07-12 11:28:38.937787 langfuse-0.0.2/langfuse/models/create_log.py
--rw-r--r--   0        0        0     1725 2023-07-12 11:28:38.883101 langfuse-0.0.2/langfuse/models/create_log_model_parameters.py
--rw-r--r--   0        0        0     3071 2023-07-12 11:28:38.902369 langfuse-0.0.2/langfuse/models/create_score_request.py
--rw-r--r--   0        0        0     6087 2023-07-12 11:28:38.916905 langfuse-0.0.2/langfuse/models/create_span_request.py
--rw-r--r--   0        0        0     2334 2023-07-12 11:28:38.891619 langfuse-0.0.2/langfuse/models/create_trace_request.py
--rw-r--r--   0        0        0     4004 2023-07-12 11:28:38.902333 langfuse-0.0.2/langfuse/models/event.py
--rw-r--r--   0        0        0     2232 2023-07-12 11:28:38.886603 langfuse-0.0.2/langfuse/models/llm_usage.py
--rw-r--r--   0        0        0     7657 2023-07-12 11:28:38.920966 langfuse-0.0.2/langfuse/models/log.py
--rw-r--r--   0        0        0     1692 2023-07-12 11:28:38.895920 langfuse-0.0.2/langfuse/models/log_model_parameters.py
--rw-r--r--   0        0        0      214 2023-07-12 11:28:38.605234 langfuse-0.0.2/langfuse/models/observation_level_event.py
--rw-r--r--   0        0        0      219 2023-07-12 11:28:38.604669 langfuse-0.0.2/langfuse/models/observation_level_generation.py
--rw-r--r--   0        0        0      213 2023-07-12 11:28:38.597789 langfuse-0.0.2/langfuse/models/observation_level_span.py
--rw-r--r--   0        0        0     2723 2023-07-12 11:28:38.903995 langfuse-0.0.2/langfuse/models/score.py
--rw-r--r--   0        0        0     4686 2023-07-12 11:28:38.928970 langfuse-0.0.2/langfuse/models/span.py
--rw-r--r--   0        0        0     2716 2023-07-12 11:28:38.918702 langfuse-0.0.2/langfuse/models/trace.py
--rw-r--r--   0        0        0      168 2023-07-12 11:28:38.594692 langfuse-0.0.2/langfuse/models/trace_id_type.py
--rw-r--r--   0        0        0      173 2023-07-12 11:28:38.597198 langfuse-0.0.2/langfuse/models/trace_id_type_event.py
--rw-r--r--   0        0        0      179 2023-07-12 11:28:38.590702 langfuse-0.0.2/langfuse/models/trace_id_type_generations.py
--rw-r--r--   0        0        0      172 2023-07-12 11:28:38.599195 langfuse-0.0.2/langfuse/models/trace_id_type_span.py
--rw-r--r--   0        0        0     7379 2023-07-12 11:28:38.939815 langfuse-0.0.2/langfuse/models/update_generation_request.py
--rw-r--r--   0        0        0     1798 2023-07-12 11:28:38.911989 langfuse-0.0.2/langfuse/models/update_generation_request_model_parameters.py
--rw-r--r--   0        0        0     3908 2023-07-12 11:28:38.930144 langfuse-0.0.2/langfuse/models/update_span_request.py
--rw-r--r--   0        0        0       25 2023-07-12 11:28:38.260242 langfuse-0.0.2/langfuse/py.typed
--rw-r--r--   0        0        0      993 2023-07-12 11:28:38.912136 langfuse-0.0.2/langfuse/types.py
--rw-r--r--   0        0        0      652 2023-07-12 11:56:30.780190 langfuse-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4234 1970-01-01 00:00:00.000000 langfuse-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3693 2023-07-12 11:28:38.262604 langfuse-0.0.3/README.md
+-rw-r--r--   0        0        0      152 2023-07-12 11:28:38.839985 langfuse-0.0.3/langfuse/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-12 11:28:38.302195 langfuse-0.0.3/langfuse/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:28:38.307846 langfuse-0.0.3/langfuse/api/event/__init__.py
+-rw-r--r--   0        0        0     4794 2023-07-12 11:28:38.860217 langfuse-0.0.3/langfuse/api/event/event_create.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:28:38.319025 langfuse-0.0.3/langfuse/api/generations/__init__.py
+-rw-r--r--   0        0        0     4557 2023-07-12 11:28:38.871136 langfuse-0.0.3/langfuse/api/generations/generations_log.py
+-rw-r--r--   0        0        0     4713 2023-07-12 11:28:38.863639 langfuse-0.0.3/langfuse/api/generations/generations_update.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:28:38.320137 langfuse-0.0.3/langfuse/api/score/__init__.py
+-rw-r--r--   0        0        0     4790 2023-07-12 11:28:38.867895 langfuse-0.0.3/langfuse/api/score/score_create.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:28:38.320737 langfuse-0.0.3/langfuse/api/span/__init__.py
+-rw-r--r--   0        0        0     4761 2023-07-12 11:28:38.866173 langfuse-0.0.3/langfuse/api/span/span_create.py
+-rw-r--r--   0        0        0     4774 2023-07-12 11:28:38.871407 langfuse-0.0.3/langfuse/api/span/span_update.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:28:38.321803 langfuse-0.0.3/langfuse/api/trace/__init__.py
+-rw-r--r--   0        0        0     4790 2023-07-12 11:28:38.881219 langfuse-0.0.3/langfuse/api/trace/trace_create.py
+-rw-r--r--   0        0        0     2817 2023-07-12 11:28:38.860072 langfuse-0.0.3/langfuse/client.py
+-rw-r--r--   0        0        0      470 2023-07-12 11:28:38.866826 langfuse-0.0.3/langfuse/errors.py
+-rw-r--r--   0        0        0     1447 2023-07-12 11:58:40.886141 langfuse-0.0.3/langfuse/langfuse.py
+-rw-r--r--   0        0        0     1728 2023-07-12 11:28:38.301226 langfuse-0.0.3/langfuse/models/__init__.py
+-rw-r--r--   0        0        0     5412 2023-07-12 11:28:38.897239 langfuse-0.0.3/langfuse/models/create_event_request.py
+-rw-r--r--   0        0        0     9118 2023-07-12 11:28:38.937787 langfuse-0.0.3/langfuse/models/create_log.py
+-rw-r--r--   0        0        0     1725 2023-07-12 11:28:38.883101 langfuse-0.0.3/langfuse/models/create_log_model_parameters.py
+-rw-r--r--   0        0        0     3071 2023-07-12 11:28:38.902369 langfuse-0.0.3/langfuse/models/create_score_request.py
+-rw-r--r--   0        0        0     6087 2023-07-12 11:28:38.916905 langfuse-0.0.3/langfuse/models/create_span_request.py
+-rw-r--r--   0        0        0     2334 2023-07-12 11:28:38.891619 langfuse-0.0.3/langfuse/models/create_trace_request.py
+-rw-r--r--   0        0        0     4004 2023-07-12 11:28:38.902333 langfuse-0.0.3/langfuse/models/event.py
+-rw-r--r--   0        0        0     2232 2023-07-12 11:28:38.886603 langfuse-0.0.3/langfuse/models/llm_usage.py
+-rw-r--r--   0        0        0     7657 2023-07-12 11:28:38.920966 langfuse-0.0.3/langfuse/models/log.py
+-rw-r--r--   0        0        0     1692 2023-07-12 11:28:38.895920 langfuse-0.0.3/langfuse/models/log_model_parameters.py
+-rw-r--r--   0        0        0      214 2023-07-12 11:28:38.605234 langfuse-0.0.3/langfuse/models/observation_level_event.py
+-rw-r--r--   0        0        0      219 2023-07-12 11:28:38.604669 langfuse-0.0.3/langfuse/models/observation_level_generation.py
+-rw-r--r--   0        0        0      213 2023-07-12 11:28:38.597789 langfuse-0.0.3/langfuse/models/observation_level_span.py
+-rw-r--r--   0        0        0     2723 2023-07-12 11:28:38.903995 langfuse-0.0.3/langfuse/models/score.py
+-rw-r--r--   0        0        0     4686 2023-07-12 11:28:38.928970 langfuse-0.0.3/langfuse/models/span.py
+-rw-r--r--   0        0        0     2716 2023-07-12 11:28:38.918702 langfuse-0.0.3/langfuse/models/trace.py
+-rw-r--r--   0        0        0      168 2023-07-12 11:28:38.594692 langfuse-0.0.3/langfuse/models/trace_id_type.py
+-rw-r--r--   0        0        0      173 2023-07-12 11:28:38.597198 langfuse-0.0.3/langfuse/models/trace_id_type_event.py
+-rw-r--r--   0        0        0      179 2023-07-12 11:28:38.590702 langfuse-0.0.3/langfuse/models/trace_id_type_generations.py
+-rw-r--r--   0        0        0      172 2023-07-12 11:28:38.599195 langfuse-0.0.3/langfuse/models/trace_id_type_span.py
+-rw-r--r--   0        0        0     7379 2023-07-12 11:28:38.939815 langfuse-0.0.3/langfuse/models/update_generation_request.py
+-rw-r--r--   0        0        0     1798 2023-07-12 11:28:38.911989 langfuse-0.0.3/langfuse/models/update_generation_request_model_parameters.py
+-rw-r--r--   0        0        0     3908 2023-07-12 11:28:38.930144 langfuse-0.0.3/langfuse/models/update_span_request.py
+-rw-r--r--   0        0        0       25 2023-07-12 11:28:38.260242 langfuse-0.0.3/langfuse/py.typed
+-rw-r--r--   0        0        0      993 2023-07-12 11:28:38.912136 langfuse-0.0.3/langfuse/types.py
+-rw-r--r--   0        0        0      652 2023-07-12 11:59:34.496749 langfuse-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4234 1970-01-01 00:00:00.000000 langfuse-0.0.3/PKG-INFO
```

### Comparing `langfuse-0.0.2/README.md` & `langfuse-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/api/event/event_create.py` & `langfuse-0.0.3/langfuse/api/event/event_create.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/api/generations/generations_log.py` & `langfuse-0.0.3/langfuse/api/generations/generations_log.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/api/generations/generations_update.py` & `langfuse-0.0.3/langfuse/api/generations/generations_update.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/api/score/score_create.py` & `langfuse-0.0.3/langfuse/api/score/score_create.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/api/span/span_create.py` & `langfuse-0.0.3/langfuse/api/span/span_create.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/api/span/span_update.py` & `langfuse-0.0.3/langfuse/api/span/span_update.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/api/trace/trace_create.py` & `langfuse-0.0.3/langfuse/api/trace/trace_create.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/client.py` & `langfuse-0.0.3/langfuse/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/langfuse.py` & `langfuse-0.0.3/langfuse/langfuse.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from langfuse.client import Client
 from langfuse.langfuse import client
 from langfuse.models.create_trace_request import CreateTraceRequest
 from langfuse.api.trace import trace_create
 
 @attr.s(auto_attribs=True)
-class AuthenticatedClient:
+class ApiClient:
     """A Client which has been authenticated for use on secured endpoints"""
 
     client: Client
     promises: list[Coroutine] = attr.ib(factory=list)
 
     def __init__(self, public_key: str, secret_key: str, base_url: Optional[str]):
         self.base_url = base_url if base_url else 'https://cloud.langfuse.com'
```

### Comparing `langfuse-0.0.2/langfuse/models/__init__.py` & `langfuse-0.0.3/langfuse/models/__init__.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/create_event_request.py` & `langfuse-0.0.3/langfuse/models/create_event_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/create_log.py` & `langfuse-0.0.3/langfuse/models/create_log.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/create_log_model_parameters.py` & `langfuse-0.0.3/langfuse/models/create_log_model_parameters.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/create_score_request.py` & `langfuse-0.0.3/langfuse/models/create_score_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/create_span_request.py` & `langfuse-0.0.3/langfuse/models/create_span_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/create_trace_request.py` & `langfuse-0.0.3/langfuse/models/create_trace_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/event.py` & `langfuse-0.0.3/langfuse/models/event.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/llm_usage.py` & `langfuse-0.0.3/langfuse/models/llm_usage.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/log.py` & `langfuse-0.0.3/langfuse/models/log.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/log_model_parameters.py` & `langfuse-0.0.3/langfuse/models/log_model_parameters.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/score.py` & `langfuse-0.0.3/langfuse/models/score.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/span.py` & `langfuse-0.0.3/langfuse/models/span.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/trace.py` & `langfuse-0.0.3/langfuse/models/trace.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/update_generation_request.py` & `langfuse-0.0.3/langfuse/models/update_generation_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/update_generation_request_model_parameters.py` & `langfuse-0.0.3/langfuse/models/update_generation_request_model_parameters.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/models/update_span_request.py` & `langfuse-0.0.3/langfuse/models/update_span_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/langfuse/types.py` & `langfuse-0.0.3/langfuse/types.py`

 * *Files identical despite different names*

### Comparing `langfuse-0.0.2/pyproject.toml` & `langfuse-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langfuse"
-version = "0.0.2"
+version = "0.0.3"
 description = "A client library for accessing langfuse"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "langfuse"},
```

### Comparing `langfuse-0.0.2/PKG-INFO` & `langfuse-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfuse
-Version: 0.0.2
+Version: 0.0.3
 Summary: A client library for accessing langfuse
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

