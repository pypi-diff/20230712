# Comparing `tmp/spendpoint-0.3.0.tar.gz` & `tmp/spendpoint-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spendpoint-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spendpoint-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spendpoint-0.3.0.tar` & `spendpoint-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      103 2023-04-04 10:46:28.100041 spendpoint-0.3.0/.dockerignore
--rw-r--r--   0        0        0      274 2023-04-04 10:46:28.100041 spendpoint-0.3.0/.editorconfig
--rw-r--r--   0        0        0      121 2023-05-16 13:05:47.269693 spendpoint-0.3.0/.gitignore
--rw-r--r--   0        0        0     2346 2023-05-16 13:05:47.269693 spendpoint-0.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      178 2023-04-04 10:46:28.100041 spendpoint-0.3.0/AUTHORS.rst
--rw-r--r--   0        0        0      387 2023-04-04 10:46:28.100041 spendpoint-0.3.0/Dockerfile
--rw-r--r--   0        0        0      408 2023-05-16 18:43:41.012519 spendpoint-0.3.0/HISTORY.rst
--rw-r--r--   0        0        0     1081 2023-04-04 10:46:28.100041 spendpoint-0.3.0/LICENSE
--rw-r--r--   0        0        0      957 2023-05-16 18:43:41.012519 spendpoint-0.3.0/README.rst
--rw-r--r--   0        0        0      495 2023-05-16 18:43:41.012519 spendpoint-0.3.0/data/configuration.toml
--rw-r--r--   0        0        0      315 2023-05-16 13:05:47.269693 spendpoint-0.3.0/default.nix
--rw-r--r--   0        0        0     1054 2023-04-04 10:46:28.104042 spendpoint-0.3.0/docs/templates/pyproject.toml
--rw-r--r--   0        0        0     1236 2023-05-16 18:43:41.012519 spendpoint-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      560 2023-05-16 18:43:41.012519 spendpoint-0.3.0/requirements.txt
--rw-r--r--   0        0        0      178 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/__init__.py
--rw-r--r--   0        0        0      776 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/__main__.py
--rw-r--r--   0        0        0     1492 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/bridge.py
--rw-r--r--   0        0        0      569 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/configuration.py
--rw-r--r--   0        0        0     8767 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/endpoint.py
--rw-r--r--   0        0        0      691 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/main.py
--rw-r--r--   0        0        0     4334 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/service.py
--rw-r--r--   0        0        0     3266 2023-05-16 13:05:47.269693 spendpoint-0.3.0/tasks.py
--rw-r--r--   0        0        0        0 2023-05-16 18:55:31.614071 spendpoint-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0       57 2023-04-04 10:46:28.104042 spendpoint-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-16 18:55:31.614071 spendpoint-0.3.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      116 2023-04-04 10:46:28.104042 spendpoint-0.3.0/tests/fixtures/state.py
--rw-r--r--   0        0        0     2590 2023-04-04 10:46:28.104042 spendpoint-0.3.0/tests/test_query_endpoint.py
--rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 spendpoint-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-04-04 10:46:28.100041 spendpoint-0.4.0/.dockerignore
+-rw-r--r--   0        0        0      268 2023-07-12 17:19:52.206269 spendpoint-0.4.0/.editorconfig
+-rw-r--r--   0        0        0      121 2023-05-16 13:05:47.269693 spendpoint-0.4.0/.gitignore
+-rw-r--r--   0        0        0     2346 2023-05-16 13:05:47.269693 spendpoint-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      178 2023-04-04 10:46:28.100041 spendpoint-0.4.0/AUTHORS.rst
+-rw-r--r--   0        0        0      424 2023-07-12 17:19:52.206269 spendpoint-0.4.0/Dockerfile
+-rw-r--r--   0        0        0      408 2023-05-16 18:43:41.012519 spendpoint-0.4.0/HISTORY.rst
+-rw-r--r--   0        0        0     1081 2023-04-04 10:46:28.100041 spendpoint-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1232 2023-07-12 17:19:52.206269 spendpoint-0.4.0/README.rst
+-rw-r--r--   0        0        0      551 2023-07-12 17:19:52.210270 spendpoint-0.4.0/data/configuration.toml
+-rw-r--r--   0        0        0      315 2023-05-16 13:05:47.269693 spendpoint-0.4.0/default.nix
+-rw-r--r--   0        0        0     1054 2023-04-04 10:46:28.104042 spendpoint-0.4.0/docs/templates/pyproject.toml
+-rw-r--r--   0        0        0     1236 2023-05-16 18:43:41.012519 spendpoint-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-05-16 18:43:41.012519 spendpoint-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      178 2023-07-12 17:19:52.210270 spendpoint-0.4.0/spendpoint/__init__.py
+-rw-r--r--   0        0        0      776 2023-05-16 18:43:41.016519 spendpoint-0.4.0/spendpoint/__main__.py
+-rw-r--r--   0        0        0     1511 2023-07-12 17:19:52.210270 spendpoint-0.4.0/spendpoint/bridge.py
+-rw-r--r--   0        0        0      569 2023-05-16 18:43:41.016519 spendpoint-0.4.0/spendpoint/configuration.py
+-rw-r--r--   0        0        0     8767 2023-05-16 18:43:41.016519 spendpoint-0.4.0/spendpoint/endpoint.py
+-rw-r--r--   0        0        0      691 2023-05-16 18:43:41.016519 spendpoint-0.4.0/spendpoint/main.py
+-rw-r--r--   0        0        0     4365 2023-07-12 17:19:52.210270 spendpoint-0.4.0/spendpoint/service.py
+-rw-r--r--   0        0        0     3266 2023-05-16 13:05:47.269693 spendpoint-0.4.0/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-12 17:32:03.513731 spendpoint-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-04 10:46:28.104042 spendpoint-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-12 17:32:03.513731 spendpoint-0.4.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-04 10:46:28.104042 spendpoint-0.4.0/tests/fixtures/state.py
+-rw-r--r--   0        0        0     2590 2023-04-04 10:46:28.104042 spendpoint-0.4.0/tests/test_query_endpoint.py
+-rw-r--r--   0        0        0     2734 1970-01-01 00:00:00.000000 spendpoint-0.4.0/PKG-INFO
```

### Comparing `spendpoint-0.3.0/.gitlab-ci.yml` & `spendpoint-0.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/LICENSE` & `spendpoint-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/docs/templates/pyproject.toml` & `spendpoint-0.4.0/docs/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/pyproject.toml` & `spendpoint-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/requirements.txt` & `spendpoint-0.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/spendpoint/__main__.py` & `spendpoint-0.4.0/spendpoint/__main__.py`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/spendpoint/bridge.py` & `spendpoint-0.4.0/spendpoint/bridge.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import requests
 from rdflib import Graph
 from typing import Union
 
 arklog.set_config_logging()
 
 
-def fetch_outliers(file_name: str, column: Union[str, int], iri: str, outlier_service_url: str) -> Graph:
+def fetch_outliers(file_name: str, column: Union[str, int], iri: str, outlier_service_url: str, timeout: int) -> Graph:
     """"""
     try:
         column = column if isinstance(column, int) else int(column)
     except ValueError as e:
         logging.error(f"Column '{column}' is not parseable to an integer.")
         raise
     parameters = {"iri": iri, "column" : column, "file" : file_name}
     try:
-        outliers_result = requests.post(outlier_service_url, json=parameters, timeout=60)
+        outliers_result = requests.post(outlier_service_url, json=parameters, timeout=timeout)
         outliers_result.raise_for_status()
     except requests.exceptions.InvalidSchema as e:
         logging.error(f"Invalid schema for '{outlier_service_url}'.")
         raise
     except requests.exceptions.ConnectTimeout as e:
         logging.error(f"Request for '{outlier_service_url}' timed out.")
         raise
```

### Comparing `spendpoint-0.3.0/spendpoint/configuration.py` & `spendpoint-0.4.0/spendpoint/configuration.py`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/spendpoint/endpoint.py` & `spendpoint-0.4.0/spendpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/spendpoint/main.py` & `spendpoint-0.4.0/spendpoint/main.py`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/spendpoint/service.py` & `spendpoint-0.4.0/spendpoint/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     :return:
     """
     logging.debug(f"Outlier service '{service_configuration.namespace}'.")
     file_name = str(_eval(part.expr.expr[0], eval_part.forget(ctx, _except=part.expr._vars)))
     column = str(_eval(part.expr.expr[1], eval_part.forget(ctx, _except=part.expr._vars)))
     iri = str(_eval(part.expr.expr[2], eval_part.forget(ctx, _except=part.expr._vars)))
     logging.info(f"Looking for outlier in '{file_name}' at column '{column}' for '{iri}'.")
-    outlier_graph = fetch_outliers(file_name, column, iri, service_configuration.endpoint)
+    outlier_graph = fetch_outliers(file_name, column, iri, service_configuration.endpoint, service_configuration.timeout)
     for stmt in outlier_graph:
         query_results.append(eval_part.merge({
             part.var: stmt[0],
             rdflib.term.Variable(part.var + "_relation") : stmt[1],
             rdflib.term.Variable(part.var + "_value") : stmt[2],
         }))
     logging.debug(f"{query_results=}")
```

### Comparing `spendpoint-0.3.0/tasks.py` & `spendpoint-0.4.0/tasks.py`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/tests/test_query_endpoint.py` & `spendpoint-0.4.0/tests/test_query_endpoint.py`

 * *Files identical despite different names*

### Comparing `spendpoint-0.3.0/PKG-INFO` & `spendpoint-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spendpoint
-Version: 0.3.0
+Version: 0.4.0
 Summary: SPARQL endpoint for ontologies.
 Keywords: spendpoint
 Author-email: Arkadiusz Michał Ryś <Arkadiusz.Michal.Rys@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,17 +40,19 @@
 Provides-Extra: test
 
 ##########
 SpEndPoint
 ##########
 
 Creates a SPARQL endpoint supporting custom services.
-Default access at `http://127.0.0.1:8000`.
+The default access point is at `http://127.0.0.1:8000`.
+This endpoint can be configured in the `configuration.toml <data/configuration.toml>`_ file.
+The docker image created uses uvicorn the host the application at `0.0.0.0:80`. Feel free to map this to any port of your liking.
 
-Currently supports 3 services:
+We currently support 3 services out of the box:
 
 .. code-block::
 
    dtf:outlier
    dtf:example
    dtf:conversion
 
@@ -69,12 +71,12 @@
 .. code-block:: shell
 
    pip install --index-url https://pip:glpat-m8mNfhxZAUnWvy7rLS1x@git.rys.one/api/v4/projects/262/packages/pypi/simple --no-deps spendpoint
 
 Configuration
 -------------
 
-A configuration file at `data/configuration.toml` holds all user configurable data.
+A configuration file at `configuration.toml <data/configuration.toml>`_ holds all user configurable data.
 You can set the `host` and `port` the server will listen on.
 A more advanced use is to import extra services.
 These services need to be defined in the `service.py` file as well.
```

