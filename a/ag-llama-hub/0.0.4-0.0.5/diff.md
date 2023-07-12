# Comparing `tmp/ag_llama_hub-0.0.4.tar.gz` & `tmp/ag_llama_hub-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_hub-0.0.4.tar", last modified: Wed Jul 12 13:49:59 2023, max compression
+gzip compressed data, was "dist\ag_llama_hub-0.0.5.tar", last modified: Wed Jul 12 14:18:08 2023, max compression
```

## Comparing `ag_llama_hub-0.0.4.tar` & `ag_llama_hub-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 13:49:59.106413 ag_llama_hub-0.0.4/
--rw-rw-rw-   0        0        0      832 2023-07-12 13:49:59.105416 ag_llama_hub-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 13:49:59.091451 ag_llama_hub-0.0.4/ag_llama_hub/
--rw-rw-rw-   0        0        0     2113 2023-07-12 13:31:26.000000 ag_llama_hub-0.0.4/ag_llama_hub/__init__.py
--rw-rw-rw-   0        0        0     4691 2023-07-12 13:32:06.000000 ag_llama_hub-0.0.4/ag_llama_hub/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.4/ag_llama_hub/choice.py
--rw-rw-rw-   0        0        0    16256 2023-07-04 11:44:01.000000 ag_llama_hub-0.0.4/ag_llama_hub/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.4/ag_llama_hub/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:49:59.100428 ag_llama_hub-0.0.4/ag_llama_hub.egg-info/
--rw-rw-rw-   0        0        0      832 2023-07-12 13:49:58.000000 ag_llama_hub-0.0.4/ag_llama_hub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-12 13:49:59.000000 ag_llama_hub-0.0.4/ag_llama_hub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 13:49:58.000000 ag_llama_hub-0.0.4/ag_llama_hub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-07-12 13:49:58.000000 ag_llama_hub-0.0.4/ag_llama_hub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 13:49:58.000000 ag_llama_hub-0.0.4/ag_llama_hub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 13:49:59.107409 ag_llama_hub-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2567 2023-07-12 13:13:29.000000 ag_llama_hub-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:49:59.103419 ag_llama_hub-0.0.4/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.4/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.4/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:18:08.487662 ag_llama_hub-0.0.5/
+-rw-rw-rw-   0        0        0      832 2023-07-12 14:18:08.486666 ag_llama_hub-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 14:18:08.471705 ag_llama_hub-0.0.5/ag_llama_hub/
+-rw-rw-rw-   0        0        0     2113 2023-07-12 13:31:26.000000 ag_llama_hub-0.0.5/ag_llama_hub/__init__.py
+-rw-rw-rw-   0        0        0     4702 2023-07-12 14:18:03.000000 ag_llama_hub-0.0.5/ag_llama_hub/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.5/ag_llama_hub/choice.py
+-rw-rw-rw-   0        0        0    16256 2023-07-04 11:44:01.000000 ag_llama_hub-0.0.5/ag_llama_hub/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.5/ag_llama_hub/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:18:08.481680 ag_llama_hub-0.0.5/ag_llama_hub.egg-info/
+-rw-rw-rw-   0        0        0      832 2023-07-12 14:18:08.000000 ag_llama_hub-0.0.5/ag_llama_hub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-12 14:18:08.000000 ag_llama_hub-0.0.5/ag_llama_hub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 14:18:08.000000 ag_llama_hub-0.0.5/ag_llama_hub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-07-12 14:18:08.000000 ag_llama_hub-0.0.5/ag_llama_hub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 14:18:08.000000 ag_llama_hub-0.0.5/ag_llama_hub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 14:18:08.487662 ag_llama_hub-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2567 2023-07-12 13:13:29.000000 ag_llama_hub-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:18:08.484672 ag_llama_hub-0.0.5/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.5/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.5/utils/render.py
```

### Comparing `ag_llama_hub-0.0.4/PKG-INFO` & `ag_llama_hub-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_hub
-Version: 0.0.4
+Version: 0.0.5
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub-0.0.4/ag_llama_hub/__init__.py` & `ag_llama_hub-0.0.5/ag_llama_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.4/ag_llama_hub/__main__.py` & `ag_llama_hub-0.0.5/ag_llama_hub/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 from . import COMPLETION_MAX_PROMPT
 from . import COMPLETION_MAX_TOKENS
 from . import COMPLETION_MAX_N
 from . import COMPLETION_MAX_LOGPROBS
 
 # Load the language model to be served.
 stream_model = None
-def load_stream_model():
+def load_stream_model(model=MODEL):
     global stream_model
     stream_model = load_model(
-        name_or_path=MODEL,
+        name_or_path=model,
         revision=MODEL_REVISION,
         cache_dir=MODEL_CACHE_DIR,
         load_in_8bit=MODEL_LOAD_IN_8BIT,
         load_in_4bit=MODEL_LOAD_IN_4BIT,
         local_files_only=MODEL_LOCAL_FILES_ONLY,
         trust_remote_code=MODEL_TRUST_REMOTE_CODE,
         half_precision=MODEL_HALF_PRECISION,
```

### Comparing `ag_llama_hub-0.0.4/ag_llama_hub/choice.py` & `ag_llama_hub-0.0.5/ag_llama_hub/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.4/ag_llama_hub/model.py` & `ag_llama_hub-0.0.5/ag_llama_hub/model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.4/ag_llama_hub/tokenizer.py` & `ag_llama_hub-0.0.5/ag_llama_hub/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.4/ag_llama_hub.egg-info/PKG-INFO` & `ag_llama_hub-0.0.5/ag_llama_hub.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-hub
-Version: 0.0.4
+Version: 0.0.5
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub-0.0.4/setup.py` & `ag_llama_hub-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.4/utils/download.py` & `ag_llama_hub-0.0.5/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.4/utils/render.py` & `ag_llama_hub-0.0.5/utils/render.py`

 * *Files identical despite different names*

