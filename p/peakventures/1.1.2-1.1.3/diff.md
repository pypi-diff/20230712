# Comparing `tmp/peakventures-1.1.2.tar.gz` & `tmp/peakventures-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakventures-1.1.2.tar", max compression
+gzip compressed data, was "peakventures-1.1.3.tar", max compression
```

## Comparing `peakventures-1.1.2.tar` & `peakventures-1.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.1.2/peakventures/__init__.py
--rw-r--r--   0        0        0     2041 2023-05-26 10:51:38.348267 peakventures-1.1.2/peakventures/api.py
--rw-r--r--   0        0        0     1153 2023-05-26 10:31:37.185812 peakventures-1.1.2/peakventures/credentials.py
--rw-r--r--   0        0        0     1336 2023-05-26 10:32:19.525020 peakventures-1.1.2/peakventures/storage.py
--rw-r--r--   0        0        0      376 2023-05-26 10:51:47.258190 peakventures-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 peakventures-1.1.2/setup.py
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 peakventures-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.1.3/peakventures/__init__.py
+-rw-r--r--   0        0        0     1813 2023-07-12 17:49:47.662944 peakventures-1.1.3/peakventures/api.py
+-rw-r--r--   0        0        0     1153 2023-05-26 10:31:37.185812 peakventures-1.1.3/peakventures/credentials.py
+-rw-r--r--   0        0        0     1336 2023-05-26 10:32:19.525020 peakventures-1.1.3/peakventures/storage.py
+-rw-r--r--   0        0        0      376 2023-07-12 17:50:29.928161 peakventures-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 peakventures-1.1.3/setup.py
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 peakventures-1.1.3/PKG-INFO
```

### Comparing `peakventures-1.1.2/peakventures/api.py` & `peakventures-1.1.3/peakventures/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import functools
 
 import requests
 from tenacity import retry, wait_exponential, stop_after_attempt
 
 from peakventures.credentials import get_credentials_json, API_CREDENTIALS_NAME
 
-BASE_URL_V1 = "https://api.peakventures.co"
 BASE_URL_V2 = "https://live.adtechapi.xyz"
 
 
 @functools.lru_cache(maxsize=1)
 def _get_session() -> requests.Session:
     credentials = get_credentials_json(API_CREDENTIALS_NAME)
 
@@ -39,27 +38,20 @@
 
 
 @retry(wait=wait_exponential(1), stop=stop_after_attempt(3))
 def update_sellside_keywords_weights(topic: str, weights: dict) -> None:
     """Update sellside weights."""
     session = _get_session()
 
-    v1_response = session.put(f"{BASE_URL_V1}/topics/{topic}/keywords", json={
+    response = session.put(f"{BASE_URL_V2}/topics/{topic}/keywords", json={
         "type": "sellside",
         "weights": weights
     })
 
-    v1_response.raise_for_status()
-
-    v2_response = session.put(f"{BASE_URL_V2}/topics/{topic}/keywords", json={
-        "type": "sellside",
-        "weights": weights
-    })
-
-    v2_response.raise_for_status()
+    response.raise_for_status()
 
 
 @retry(wait=wait_exponential(1), stop=stop_after_attempt(3))
 def get_topic_afd_domains(topic: str) -> list:
     """Get topic AFD domains."""
     session = _get_session()
```

### Comparing `peakventures-1.1.2/peakventures/credentials.py` & `peakventures-1.1.3/peakventures/credentials.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.1.2/peakventures/storage.py` & `peakventures-1.1.3/peakventures/storage.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.1.2/setup.py` & `peakventures-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['azure-storage-blob>=12.16.0,<13.0.0',
  'boto3>=1.26.141,<2.0.0',
  'tenacity>=8.2.2,<9.0.0']
 
 setup_kwargs = {
     'name': 'peakventures',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': 'PeakVentures Python Utilities for DataBricks',
     'long_description': 'None',
     'author': 'Volodymyr Smirnov',
     'author_email': 'volodymyr@peakventures.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `peakventures-1.1.2/PKG-INFO` & `peakventures-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakventures
-Version: 1.1.2
+Version: 1.1.3
 Summary: PeakVentures Python Utilities for DataBricks
 Author: Volodymyr Smirnov
 Author-email: volodymyr@peakventures.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

