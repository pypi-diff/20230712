# Comparing `tmp/elx-0.1.0a2.tar.gz` & `tmp/elx-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elx-0.1.0a2.tar", max compression
+gzip compressed data, was "elx-0.1.0a3.tar", max compression
```

## Comparing `elx-0.1.0a2.tar` & `elx-0.1.0a3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     2745 2023-07-12 16:49:28.422407 elx-0.1.0a2/README.md
--rw-r--r--   0        0        0      158 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/__init__.py
--rw-r--r--   0        0        0      533 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/catalog.py
--rw-r--r--   0        0        0      735 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/dagster.py
--rw-r--r--   0        0        0       92 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/exceptions.py
--rw-r--r--   0        0        0      933 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/json_temp_file.py
--rw-r--r--   0        0        0     2704 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/runner.py
--rw-r--r--   0        0        0     3587 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/singer.py
--rw-r--r--   0        0        0     4067 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/state.py
--rw-r--r--   0        0        0     2023 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/tap.py
--rw-r--r--   0        0        0      940 2023-07-12 16:49:28.422407 elx-0.1.0a2/elx/target.py
--rw-r--r--   0        0        0     1234 2023-07-12 16:49:28.426407 elx-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 elx-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     2745 2023-07-12 16:54:31.395640 elx-0.1.0a3/README.md
+-rw-r--r--   0        0        0      158 2023-07-12 16:54:31.395640 elx-0.1.0a3/elx/__init__.py
+-rw-r--r--   0        0        0      533 2023-07-12 16:54:31.395640 elx-0.1.0a3/elx/catalog.py
+-rw-r--r--   0        0        0       92 2023-07-12 16:54:31.395640 elx-0.1.0a3/elx/exceptions.py
+-rw-r--r--   0        0        0      933 2023-07-12 16:54:31.395640 elx-0.1.0a3/elx/json_temp_file.py
+-rw-r--r--   0        0        0     2704 2023-07-12 16:54:31.395640 elx-0.1.0a3/elx/runner.py
+-rw-r--r--   0        0        0     3587 2023-07-12 16:54:31.395640 elx-0.1.0a3/elx/singer.py
+-rw-r--r--   0        0        0     4067 2023-07-12 16:54:31.395640 elx-0.1.0a3/elx/state.py
+-rw-r--r--   0        0        0     2023 2023-07-12 16:54:31.395640 elx-0.1.0a3/elx/tap.py
+-rw-r--r--   0        0        0      940 2023-07-12 16:54:31.395640 elx-0.1.0a3/elx/target.py
+-rw-r--r--   0        0        0     1219 2023-07-12 16:54:31.399640 elx-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 elx-0.1.0a3/PKG-INFO
```

### Comparing `elx-0.1.0a2/README.md` & `elx-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `elx-0.1.0a2/elx/catalog.py` & `elx-0.1.0a3/elx/catalog.py`

 * *Files identical despite different names*

### Comparing `elx-0.1.0a2/elx/json_temp_file.py` & `elx-0.1.0a3/elx/json_temp_file.py`

 * *Files identical despite different names*

### Comparing `elx-0.1.0a2/elx/runner.py` & `elx-0.1.0a3/elx/runner.py`

 * *Files identical despite different names*

### Comparing `elx-0.1.0a2/elx/singer.py` & `elx-0.1.0a3/elx/singer.py`

 * *Files identical despite different names*

### Comparing `elx-0.1.0a2/elx/state.py` & `elx-0.1.0a3/elx/state.py`

 * *Files identical despite different names*

### Comparing `elx-0.1.0a2/elx/tap.py` & `elx-0.1.0a3/elx/tap.py`

 * *Files identical despite different names*

### Comparing `elx-0.1.0a2/elx/target.py` & `elx-0.1.0a3/elx/target.py`

 * *Files identical despite different names*

### Comparing `elx-0.1.0a2/pyproject.toml` & `elx-0.1.0a3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "elx"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = "A lightweight Python interface for extracting and loading using the Singer.io spec."
 authors = ["Jules Huisman <jules.huisman@quantile.nl>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.8,<4.0"
 pipx = "^1.2.0"
 smart-open = {version = "^6.3.0"}
 python-dotenv = "^1.0.0"
-dagster = "^1.3.13"
 pydantic = "1.10.11"
 azure-storage-blob = {version = "^12.0.0", optional = true}
 azure-common = {version = "^1.0.0", optional = true}
 azure-core = {version = "^1.0.0", optional = true}
 boto3 = {version = "^1.0.0", optional = true}
 google-cloud-storage = {version = "^2.6.0", optional = true}
 requests = {version = "^2.0.0", optional = true}
```

### Comparing `elx-0.1.0a2/PKG-INFO` & `elx-0.1.0a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: elx
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A lightweight Python interface for extracting and loading using the Singer.io spec.
 Author: Jules Huisman
 Author-email: jules.huisman@quantile.nl
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: gcs
 Provides-Extra: http
 Provides-Extra: ssh
 Requires-Dist: azure-common (>=1.0.0,<2.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: azure-core (>=1.0.0,<2.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: azure-storage-blob (>=12.0.0,<13.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: boto3 (>=1.0.0,<2.0.0) ; extra == "aws" or extra == "all"
-Requires-Dist: dagster (>=1.3.13,<2.0.0)
 Requires-Dist: google-cloud-storage (>=2.6.0,<3.0.0) ; extra == "gcs" or extra == "all"
 Requires-Dist: paramiko (>=2.0.0,<3.0.0) ; extra == "ssh" or extra == "all"
 Requires-Dist: pipx (>=1.2.0,<2.0.0)
 Requires-Dist: pydantic (==1.10.11)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.0.0,<3.0.0) ; extra == "http" or extra == "all"
 Requires-Dist: smart-open (>=6.3.0,<7.0.0)
```

