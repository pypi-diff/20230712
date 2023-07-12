# Comparing `tmp/brainchain-0.3.4.tar.gz` & `tmp/brainchain-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.3.4.tar", max compression
+gzip compressed data, was "brainchain-0.3.5.tar", max compression
```

## Comparing `brainchain-0.3.4.tar` & `brainchain-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.4/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.4/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.4/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.4/brainchain/__init__.py
--rw-r--r--   0        0        0     5887 2023-07-12 17:03:15.378203 brainchain-0.3.4/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.4/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.4/brainchain/coredata.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.4/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.4/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.4/brainchain/sales_intel.py
--rw-r--r--   0        0        0      526 2023-07-12 18:01:46.777134 brainchain-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 brainchain-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.5/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.5/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.5/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.5/brainchain/__init__.py
+-rw-r--r--   0        0        0     5887 2023-07-12 17:03:15.378203 brainchain-0.3.5/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.5/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.5/brainchain/coredata.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.5/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.5/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.5/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      532 2023-07-12 18:05:54.407374 brainchain-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.3.5/PKG-INFO
```

### Comparing `brainchain-0.3.4/brainchain/.aider.chat.history.md` & `brainchain-0.3.5/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.4/brainchain/.aider.input.history` & `brainchain-0.3.5/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.4/brainchain/README.md` & `brainchain-0.3.5/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.4/brainchain/brainchain.py` & `brainchain-0.3.5/brainchain/brainchain.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.4/brainchain/carnivore.py` & `brainchain-0.3.5/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.4/brainchain/coredata.py` & `brainchain-0.3.5/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.4/brainchain/factcheck.py` & `brainchain-0.3.5/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.4/brainchain/requirements.txt` & `brainchain-0.3.5/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.4/brainchain/sales_intel.py` & `brainchain-0.3.5/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.4/pyproject.toml` & `brainchain-0.3.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.3.4"
+version = "0.3.5"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
-promptlayer = "^1.90"
+promptlayer = "0.1.92"
 openai = "0.27.8"
-modal-client = "^0.50"
-tiktoken = "0.4.0"
+modal-client = "0.50.2570"
+tiktoken = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

