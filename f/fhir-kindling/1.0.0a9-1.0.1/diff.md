# Comparing `tmp/fhir_kindling-1.0.0a9.tar.gz` & `tmp/fhir_kindling-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir_kindling-1.0.0a9.tar", max compression
+gzip compressed data, was "fhir_kindling-1.0.1.tar", max compression
```

## Comparing `fhir_kindling-1.0.0a9.tar` & `fhir_kindling-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      133 2023-05-19 08:12:30.473185 fhir_kindling-1.0.0a9/fhir_kindling/__init__.py
--rw-r--r--   0        0        0       53 2023-06-12 10:49:45.354737 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/__init__.py
--rw-r--r--   0        0        0    13487 2023-06-14 11:50:22.471355 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/bench.py
--rw-r--r--   0        0        0     3435 2023-06-12 10:49:45.363362 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/constants.py
--rw-r--r--   0        0        0     8695 2023-06-12 10:49:45.363362 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/data.py
--rw-r--r--   0        0        0     3282 2023-06-13 21:22:44.886849 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/figures.py
--rw-r--r--   0        0        0     3957 2023-06-13 21:33:50.321717 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/results.py
--rw-r--r--   0        0        0      268 2023-05-19 08:12:30.487218 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/__init__.py
--rw-r--r--   0        0        0    13598 2023-06-12 10:49:45.376260 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/base.py
--rw-r--r--   0        0        0     9710 2023-05-19 08:12:30.488696 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_async.py
--rw-r--r--   0        0        0    10919 2023-05-19 08:12:30.489704 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_parameters.py
--rw-r--r--   0        0        0     7939 2023-05-19 08:12:30.490712 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_response.py
--rw-r--r--   0        0        0     9714 2023-05-19 08:12:30.491709 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_sync.py
--rw-r--r--   0        0        0       36 2023-05-19 08:12:30.494722 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/__init__.py
--rw-r--r--   0        0        0     3936 2023-05-19 08:12:30.495707 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/auth.py
--rw-r--r--   0        0        0    35574 2023-06-13 12:00:27.891209 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/fhir_server.py
--rw-r--r--   0        0        0     3736 2023-05-19 08:12:30.497707 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/server_responses.py
--rw-r--r--   0        0        0     2610 2023-05-19 08:12:30.498706 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/summary.py
--rw-r--r--   0        0        0     5712 2023-06-14 14:25:16.269949 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/transactions.py
--rw-r--r--   0        0        0     8894 2023-06-12 10:49:45.379382 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/transfer.py
--rw-r--r--   0        0        0       89 2023-05-19 08:12:30.503726 fhir_kindling-1.0.0a9/fhir_kindling/figures/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-19 08:12:30.507717 fhir_kindling-1.0.0a9/fhir_kindling/figures/resource_plots.py
--rw-r--r--   0        0        0      759 2023-05-19 08:12:30.507717 fhir_kindling-1.0.0a9/fhir_kindling/figures/summary.py
--rw-r--r--   0        0        0      203 2023-05-19 08:12:30.512721 fhir_kindling-1.0.0a9/fhir_kindling/generators/__init__.py
--rw-r--r--   0        0        0      174 2023-06-12 10:49:45.379382 fhir_kindling-1.0.0a9/fhir_kindling/generators/base.py
--rw-r--r--   0        0        0    20029 2023-06-12 10:49:45.379382 fhir_kindling-1.0.0a9/fhir_kindling/generators/dataset.py
--rw-r--r--   0        0        0     1530 2023-05-19 08:12:30.517471 fhir_kindling-1.0.0a9/fhir_kindling/generators/field_generator.py
--rw-r--r--   0        0        0     5019 2023-06-14 14:22:42.586944 fhir_kindling-1.0.0a9/fhir_kindling/generators/patient.py
--rw-r--r--   0        0        0     8165 2023-06-12 10:49:45.386430 fhir_kindling-1.0.0a9/fhir_kindling/generators/resource_generator.py
--rw-r--r--   0        0        0     5924 2023-06-12 10:49:45.386430 fhir_kindling-1.0.0a9/fhir_kindling/generators/time_series_generator.py
--rw-r--r--   0        0        0        0 2023-05-19 08:12:30.520468 fhir_kindling-1.0.0a9/fhir_kindling/privacy/__init__.py
--rw-r--r--   0        0        0     3774 2023-05-19 08:12:30.522454 fhir_kindling-1.0.0a9/fhir_kindling/privacy/k_anonymity.py
--rw-r--r--   0        0        0      103 2023-06-12 10:49:45.386430 fhir_kindling-1.0.0a9/fhir_kindling/serde/__init__.py
--rw-r--r--   0        0        0     4128 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/serde/flatten.py
--rw-r--r--   0        0        0      404 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/serde/json.py
--rw-r--r--   0        0        0        0 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/tests/__init__.py
--rw-r--r--   0        0        0      588 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/tests/server/__init__.py
--rw-r--r--   0        0        0     1031 2023-06-14 12:08:09.888924 fhir_kindling-1.0.0a9/fhir_kindling/tests/server/test_transfer.py
--rw-r--r--   0        0        0     1482 2023-05-19 08:12:30.539605 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_auth.py
--rw-r--r--   0        0        0      459 2023-06-14 14:28:11.503574 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_benchmark.py
--rw-r--r--   0        0        0    55630 2023-05-19 08:12:30.544612 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_fhir_query.py
--rw-r--r--   0        0        0    21796 2023-05-19 08:12:30.547611 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_fhir_server.py
--rw-r--r--   0        0        0    11123 2023-06-14 14:35:25.368258 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_generators.py
--rw-r--r--   0        0        0     1115 2023-05-19 08:12:30.555603 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_plots.py
--rw-r--r--   0        0        0     1024 2023-05-19 08:12:30.560617 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_privacy.py
--rw-r--r--   0        0        0     2082 2023-05-19 08:12:30.561622 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_serialization.py
--rw-r--r--   0        0        0     4810 2023-06-14 14:36:36.060848 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_util.py
--rw-r--r--   0        0        0       43 2023-05-19 08:12:30.563624 fhir_kindling-1.0.0a9/fhir_kindling/util/__init__.py
--rw-r--r--   0        0        0     4466 2023-05-19 08:12:30.564618 fhir_kindling-1.0.0a9/fhir_kindling/util/references.py
--rw-r--r--   0        0        0     1876 2023-05-19 08:12:30.565631 fhir_kindling-1.0.0a9/fhir_kindling/util/resources.py
--rw-r--r--   0        0        0     1071 2023-05-19 08:12:30.422025 fhir_kindling-1.0.0a9/LICENSE
--rw-r--r--   0        0        0     2788 2023-06-16 07:51:35.400997 fhir_kindling-1.0.0a9/pyproject.toml
--rw-r--r--   0        0        0    10041 2023-05-19 08:12:30.422025 fhir_kindling-1.0.0a9/README.md
--rw-r--r--   0        0        0    11720 1970-01-01 00:00:00.000000 fhir_kindling-1.0.0a9/setup.py
--rw-r--r--   0        0        0    11826 1970-01-01 00:00:00.000000 fhir_kindling-1.0.0a9/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2023-03-04 09:55:34.447847 fhir_kindling-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0    10041 2023-04-15 20:16:55.060230 fhir_kindling-1.0.1/README.md
+-rwxr-xr-x   0        0        0      133 2023-05-31 12:10:59.853995 fhir_kindling-1.0.1/fhir_kindling/__init__.py
+-rw-r--r--   0        0        0       53 2023-06-12 10:41:39.764673 fhir_kindling-1.0.1/fhir_kindling/benchmark/__init__.py
+-rw-r--r--   0        0        0    13487 2023-06-30 07:52:40.076501 fhir_kindling-1.0.1/fhir_kindling/benchmark/bench.py
+-rw-r--r--   0        0        0     3435 2023-06-12 10:41:39.764673 fhir_kindling-1.0.1/fhir_kindling/benchmark/constants.py
+-rw-r--r--   0        0        0     8695 2023-06-12 10:41:39.764673 fhir_kindling-1.0.1/fhir_kindling/benchmark/data.py
+-rw-r--r--   0        0        0     3282 2023-06-30 07:52:40.076501 fhir_kindling-1.0.1/fhir_kindling/benchmark/figures.py
+-rw-r--r--   0        0        0     3957 2023-06-30 07:52:40.076501 fhir_kindling-1.0.1/fhir_kindling/benchmark/results.py
+-rwxr-xr-x   0        0        0      268 2023-03-23 12:51:15.067324 fhir_kindling-1.0.1/fhir_kindling/fhir_query/__init__.py
+-rwxr-xr-x   0        0        0    13790 2023-07-09 11:04:22.677435 fhir_kindling-1.0.1/fhir_kindling/fhir_query/base.py
+-rwxr-xr-x   0        0        0    10481 2023-07-09 11:04:22.677435 fhir_kindling-1.0.1/fhir_kindling/fhir_query/query_async.py
+-rwxr-xr-x   0        0        0    10919 2023-03-23 00:16:03.459242 fhir_kindling-1.0.1/fhir_kindling/fhir_query/query_parameters.py
+-rwxr-xr-x   0        0        0     7939 2023-05-31 12:10:59.853995 fhir_kindling-1.0.1/fhir_kindling/fhir_query/query_response.py
+-rwxr-xr-x   0        0        0    10279 2023-07-09 11:04:22.677435 fhir_kindling-1.0.1/fhir_kindling/fhir_query/query_sync.py
+-rwxr-xr-x   0        0        0       36 2023-05-31 12:10:59.853995 fhir_kindling-1.0.1/fhir_kindling/fhir_server/__init__.py
+-rwxr-xr-x   0        0        0     3936 2023-03-23 00:16:03.319242 fhir_kindling-1.0.1/fhir_kindling/fhir_server/auth.py
+-rwxr-xr-x   0        0        0    38331 2023-07-12 10:06:42.416678 fhir_kindling-1.0.1/fhir_kindling/fhir_server/fhir_server.py
+-rwxr-xr-x   0        0        0     3736 2023-03-23 00:47:12.807135 fhir_kindling-1.0.1/fhir_kindling/fhir_server/server_responses.py
+-rwxr-xr-x   0        0        0     2610 2023-03-09 17:53:02.501330 fhir_kindling-1.0.1/fhir_kindling/fhir_server/summary.py
+-rwxr-xr-x   0        0        0     5712 2023-06-30 07:52:40.076501 fhir_kindling-1.0.1/fhir_kindling/fhir_server/transactions.py
+-rwxr-xr-x   0        0        0     8894 2023-06-12 10:41:39.764673 fhir_kindling-1.0.1/fhir_kindling/fhir_server/transfer.py
+-rwxr-xr-x   0        0        0       89 2023-03-04 09:55:34.717848 fhir_kindling-1.0.1/fhir_kindling/figures/__init__.py
+-rwxr-xr-x   0        0        0     1240 2023-03-04 09:55:34.717848 fhir_kindling-1.0.1/fhir_kindling/figures/resource_plots.py
+-rwxr-xr-x   0        0        0      759 2023-03-04 09:55:34.717848 fhir_kindling-1.0.1/fhir_kindling/figures/summary.py
+-rwxr-xr-x   0        0        0      203 2023-03-04 09:55:34.717848 fhir_kindling-1.0.1/fhir_kindling/generators/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-12 10:41:39.764673 fhir_kindling-1.0.1/fhir_kindling/generators/base.py
+-rwxr-xr-x   0        0        0    20029 2023-06-12 10:41:39.764673 fhir_kindling-1.0.1/fhir_kindling/generators/dataset.py
+-rwxr-xr-x   0        0        0     1530 2023-03-04 09:55:34.717848 fhir_kindling-1.0.1/fhir_kindling/generators/field_generator.py
+-rwxr-xr-x   0        0        0     5019 2023-06-30 07:52:40.076501 fhir_kindling-1.0.1/fhir_kindling/generators/patient.py
+-rwxr-xr-x   0        0        0     8165 2023-06-12 10:41:39.764673 fhir_kindling-1.0.1/fhir_kindling/generators/resource_generator.py
+-rw-r--r--   0        0        0     5924 2023-06-12 10:41:39.764673 fhir_kindling-1.0.1/fhir_kindling/generators/time_series_generator.py
+-rwxr-xr-x   0        0        0        0 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/privacy/__init__.py
+-rwxr-xr-x   0        0        0     3774 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/privacy/k_anonymity.py
+-rwxr-xr-x   0        0        0        1 2023-07-12 10:00:13.583113 fhir_kindling-1.0.1/fhir_kindling/serde/__init__.py
+-rwxr-xr-x   0        0        0     4128 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/serde/flatten.py
+-rwxr-xr-x   0        0        0      404 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/serde/json.py
+-rwxr-xr-x   0        0        0        0 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/tests/__init__.py
+-rwxr-xr-x   0        0        0      588 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/tests/conftest.py
+-rwxr-xr-x   0        0        0        0 2023-03-05 13:00:06.671372 fhir_kindling-1.0.1/fhir_kindling/tests/server/__init__.py
+-rwxr-xr-x   0        0        0     1034 2023-07-09 11:04:22.677435 fhir_kindling-1.0.1/fhir_kindling/tests/server/test_transfer.py
+-rwxr-xr-x   0        0        0     1482 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/tests/test_auth.py
+-rw-r--r--   0        0        0      459 2023-06-30 07:52:40.076501 fhir_kindling-1.0.1/fhir_kindling/tests/test_benchmark.py
+-rwxr-xr-x   0        0        0    55630 2023-07-09 14:36:46.653674 fhir_kindling-1.0.1/fhir_kindling/tests/test_fhir_query.py
+-rwxr-xr-x   0        0        0    21796 2023-05-23 15:03:19.828369 fhir_kindling-1.0.1/fhir_kindling/tests/test_fhir_server.py
+-rwxr-xr-x   0        0        0    11123 2023-06-30 07:52:40.076501 fhir_kindling-1.0.1/fhir_kindling/tests/test_generators.py
+-rwxr-xr-x   0        0        0     1115 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/tests/test_plots.py
+-rwxr-xr-x   0        0        0     1024 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/tests/test_privacy.py
+-rwxr-xr-x   0        0        0     2082 2023-05-31 12:10:59.853995 fhir_kindling-1.0.1/fhir_kindling/tests/test_serialization.py
+-rwxr-xr-x   0        0        0     5103 2023-07-09 11:04:22.677435 fhir_kindling-1.0.1/fhir_kindling/tests/test_util.py
+-rwxr-xr-x   0        0        0       43 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/util/__init__.py
+-rwxr-xr-x   0        0        0     4466 2023-03-23 00:16:03.399242 fhir_kindling-1.0.1/fhir_kindling/util/references.py
+-rwxr-xr-x   0        0        0     1876 2023-03-04 09:55:34.727848 fhir_kindling-1.0.1/fhir_kindling/util/resources.py
+-rw-r--r--   0        0        0     5183 2023-07-09 11:04:22.677435 fhir_kindling-1.0.1/fhir_kindling/util/retry_transport.py
+-rwxr-xr-x   0        0        0     2792 2023-07-12 10:04:30.231101 fhir_kindling-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11842 1970-01-01 00:00:00.000000 fhir_kindling-1.0.1/PKG-INFO
```

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/benchmark/bench.py` & `fhir_kindling-1.0.1/fhir_kindling/benchmark/bench.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/benchmark/constants.py` & `fhir_kindling-1.0.1/fhir_kindling/benchmark/constants.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/benchmark/data.py` & `fhir_kindling-1.0.1/fhir_kindling/benchmark/data.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/benchmark/figures.py` & `fhir_kindling-1.0.1/fhir_kindling/benchmark/figures.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/benchmark/results.py` & `fhir_kindling-1.0.1/fhir_kindling/benchmark/results.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/base.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_query/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
             FHIRResourceModel, fhir.resources.FHIRAbstractModel, str
         ] = None,
         query_parameters: FhirQueryParameters = None,
         auth: httpx.Auth = None,
         headers: dict = None,
         output_format: str = "json",
     ):
+        if base_url[-1] == "/":
+            base_url = base_url[:-1]
         self.base_url = base_url
 
         # Set up the requests session with auth and headers
         self.auth = auth
         self.headers = headers
 
         # initialize the resource and query parameters
@@ -261,14 +263,20 @@
         else:
             query_has_params = [added_has_param]
         self.query_parameters.has_parameters = query_has_params
 
         return self
 
     def _make_query_string(self) -> str:
+        """
+        Make the query string from the query parameters
+
+        Returns:
+            query string
+        """
         query_string = self.base_url + self.query_parameters.to_query_string()
 
         if not self._count:
             self._count = 5000
 
         if self._limit and self._limit < self._count:
             if query_string[-1] == "?":
```

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_async.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_query/query_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,33 @@
         query_parameters: FhirQueryParameters = None,
         auth: httpx.Auth = None,
         headers: dict = None,
         output_format: str = "json",
         client: httpx.AsyncClient = None,
         proxies: Union[str, dict] = None,
     ):
+        """Initialize an async FHIR query object.
+
+        Args:
+            base_url: Base URL of the FHIR server to query.
+            resource: Base resource to build the query on. Defaults to None.
+            query_parameters: Query parameters object that fully describes a FHIR query. Defaults to None.
+            auth: httpx auth object to authenticate the requests. Defaults to None.
+            headers: Optional additional headers to add to the request. Defaults to None.
+            output_format: Response format of the query. Defaults to "json".
+            client: httpx Client passed from the server. Defaults to None.
+            proxies: List of proxies to use. Defaults to None.
+        """
         super().__init__(
-            base_url, resource, query_parameters, auth, headers, output_format
+            base_url,
+            resource,
+            query_parameters,
+            auth,
+            headers,
+            output_format,
         )
         self.proxies = proxies
         # set up the async client instance
         self.client = None
         if client:
             self.client = client
         else:
```

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_parameters.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_query/query_parameters.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_response.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_query/query_response.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_sync.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_query/query_sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,18 +28,37 @@
         query_parameters: FhirQueryParameters = None,
         auth: httpx.Auth = None,
         headers: dict = None,
         client: httpx.Client = None,
         output_format: str = "json",
         proxies: Union[str, dict] = None,
     ):
+        """Initialize an sync FHIR query object.
+
+        Args:
+            base_url: Base URL of the FHIR server to query.
+            resource: Base resource to build the query on. Defaults to None.
+            query_parameters: Query parameters object that fully describes a FHIR query. Defaults to None.
+            auth: httpx auth object to authenticate the requests. Defaults to None.
+            headers: Optional additional headers to add to the request. Defaults to None.
+            output_format: Response format of the query. Defaults to "json".
+            client: httpx Client passed from the server. Defaults to None.
+            proxies: List of proxies to use. Defaults to None.
+        """
+
         super().__init__(
-            base_url, resource, query_parameters, auth, headers, output_format
+            base_url,
+            resource,
+            query_parameters,
+            auth,
+            headers,
+            output_format,
         )
         self.proxies = proxies
+        self.client = None
         if client:
             self.client = client
         else:
             self.client = self._setup_client()
 
     def all(
         self,
@@ -95,37 +114,37 @@
 
         """
         self._limit = 1
         return self._execute_query()
 
     def count(self) -> int:
         self._count = 0
-        with self._setup_client() as client:
-            response = client.get(self._make_query_string() + "&_summary=count")
+        response = self.client.get(self._make_query_string() + "&_summary=count")
         response.raise_for_status()
         return response.json()["total"]
 
     def _setup_client(self):
+        if self.client:
+            return self.client
         headers = self.headers if self.headers else {}
         headers["Content-Type"] = "application/fhir+json"
         client = httpx.Client(
             auth=self.auth, headers=headers, proxies=self.proxies, timeout=None
         )
         return client
 
     def _execute_query(
         self,
         page_callback: Union[
             Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
         ] = None,
         count: int = None,
     ) -> QueryResponse:
-        with self._setup_client() as client:
-            r = client.get(self.query_url)
-            r.raise_for_status()
+        r = self.client.get(self.query_url)
+        r.raise_for_status()
 
         response = self._resolve_response_pagination(r, page_callback, count)
         return response
 
     def _resolve_response_pagination(
         self,
         initial_response: httpx.Response,
@@ -158,55 +177,54 @@
         ] = None,
         count: int = None,
     ) -> dict:
         response_json = orjson.loads(initial_response.content)
         link = response_json.get("link", None)
         # If there is a link, get the next page otherwise return the response
 
-        with self._setup_client() as client:
-            if not link:
-                self.status_code = ResponseStatusCodes.OK
+        if not link:
+            self.status_code = ResponseStatusCodes.OK
+            return response_json
+        else:
+            entries = []
+            initial_entry = response_json.get("entry", None)
+            if not initial_entry:
+                self.status_code = ResponseStatusCodes.NOT_FOUND
                 return response_json
             else:
-                entries = []
-                initial_entry = response_json.get("entry", None)
-                if not initial_entry:
-                    self.status_code = ResponseStatusCodes.NOT_FOUND
-                    return response_json
-                else:
-                    self.status_code = ResponseStatusCodes.OK
+                self.status_code = ResponseStatusCodes.OK
+                response_entries = response_json["entry"]
+                entries.extend(response_entries)
+                self._execute_callback(response_entries, page_callback)
+            # if the limit is reached, stop resolving the pagination
+            if self._limit and len(entries) >= self._limit:
+                response_entries = response_json["entry"][: self._limit]
+                response_json["entry"] = response_entries
+                self._execute_callback(response_entries, page_callback)
+                return response_json
+            # query the linked page and add the entries to the response
+
+            while response_json.get("link", None):
+                if self._limit and len(entries) >= self._limit:
+                    break
+                next_page = next(
+                    (
+                        link
+                        for link in response_json["link"]
+                        if link.get("relation", None) == "next"
+                    ),
+                    None,
+                )
+                if next_page:
+                    response_json = self.client.get(next_page["url"]).json()
                     response_entries = response_json["entry"]
                     entries.extend(response_entries)
                     self._execute_callback(response_entries, page_callback)
-                # if the limit is reached, stop resolving the pagination
-                if self._limit and len(entries) >= self._limit:
-                    response_entries = response_json["entry"][: self._limit]
-                    response_json["entry"] = response_entries
-                    self._execute_callback(response_entries, page_callback)
-                    return response_json
-                # query the linked page and add the entries to the response
-
-                while response_json.get("link", None):
-                    if self._limit and len(entries) >= self._limit:
-                        break
-                    next_page = next(
-                        (
-                            link
-                            for link in response_json["link"]
-                            if link.get("relation", None) == "next"
-                        ),
-                        None,
-                    )
-                    if next_page:
-                        response_json = client.get(next_page["url"]).json()
-                        response_entries = response_json["entry"]
-                        entries.extend(response_entries)
-                        self._execute_callback(response_entries, page_callback)
-                    else:
-                        break
+                else:
+                    break
 
             response_json["entry"] = entries[: self._limit] if self._limit else entries
             return response_json
 
     def _resolve_xml_pagination(self, server_response: httpx.Response) -> str:
         # parse the xml response and extract the initial entries
         initial_response = xmltodict.parse(server_response.text)
```

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/auth.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_server/auth.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/fhir_server.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_server/fhir_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-from typing import List, Union
+from typing import Iterable, List, Union
 
 import fhir.resources
 import httpx
 from authlib.integrations.httpx_client import OAuth2Client
 from authlib.oauth2.rfc6749 import OAuth2Token
 from authlib.oauth2.rfc7523 import ClientSecretJWT
 from fhir.resources import FHIRAbstractModel, construct_fhir_element
@@ -31,32 +31,39 @@
 from fhir_kindling.fhir_server.transactions import (
     TransactionMethod,
     TransactionType,
     make_transaction_bundle,
 )
 from fhir_kindling.fhir_server.transfer import transfer
 from fhir_kindling.serde.json import json_dict
-from fhir_kindling.util.resources import valid_resource_name
+from fhir_kindling.util.retry_transport import RetryTransport
 
 
 class FhirServer:
     def __init__(
         self,
         api_address: str,
-        username: str = None,
-        password: str = None,
-        token: str = None,
-        client_id: str = None,
-        client_secret: str = None,
-        oidc_provider_url: str = None,
-        auth: httpx.Auth = None,
-        headers: dict = None,
-        proxies: Union[dict, str] = None,
-        timeout: int = None,
+        username: Union[str, None] = None,
+        password: Union[str, None] = None,
+        token: Union[str, None] = None,
+        client_id: Union[str, None] = None,
+        client_secret: Union[str, None] = None,
+        oidc_provider_url: Union[str, None] = None,
+        auth: Union[httpx.Auth, None] = None,
+        headers: Union[dict, None] = None,
+        proxies: Union[dict, str, None] = None,
+        timeout: Union[int, None] = None,
         fhir_server_type: str = "hapi",
+        retry_status_codes: Union[Iterable[int], None] = None,
+        retryable_methods: Union[Iterable[str], None] = None,
+        max_atttempts: int = 5,
+        max_backoff_wait: float = 60,
+        backoff_factor: float = 0.1,
+        jitter_ratio: float = 0.1,
+        respect_retry_after_header: bool = True,
     ):
         """
         Initialize a FHIR server connection
         Args:
             api_address: the base endpoint of the fhir server REST API
             username: username for basic auth
             password: password for basic auth
@@ -65,14 +72,17 @@
             client_secret: client secret for oauth2
             oidc_provider_url: provider url for oauth2
             auth: optional auth object to authenticate against a server
             headers: optional additional headers to be added to the session
             proxies: optional proxies to be added to the session
             timeout: optional timeout for the session default is None
             fhir_server_type: type of fhir server (hapi, blaze, etc.)
+            retry_status_codes: optional list of status codes to retry on
+            max_atttempts: optional number of times to retry
+            retry_wait: optional number of seconds to wait between retries
         """
 
         # server definition values
         self.fhir_server_type = fhir_server_type
         self.api_address = self._validate_api_address(api_address)
         self._meta_data = None
 
@@ -85,14 +95,23 @@
 
         # oauth2 auth vars
         self.client_id = client_id
         self.client_secret = client_secret
         self.oidc_provider_url = oidc_provider_url
         self.oauth_token: OAuth2Token = None
 
+        # retry vars
+        self.retry_status_codes = retry_status_codes
+        self.retryable_methods = retryable_methods
+        self.max_attempts = max_atttempts
+        self.max_backoff_wait = max_backoff_wait
+        self.backoff_factor = backoff_factor
+        self.jitter_ratio = jitter_ratio
+        self.respect_retry_after_header = respect_retry_after_header
+
         self._auth = auth
         self._headers = headers
         self._proxies = proxies
         self._timeout = timeout
 
     @classmethod
     def from_env(cls, no_auth: bool = False) -> "FhirServer":
@@ -150,90 +169,95 @@
 
         Returns:
             a FhirQuerySync object that can be further modified with filters and conditions before being executed
             against the server
         """
 
         self._validate_query_input(resource, query_parameters, query_string)
+        query_parameters = self._setup_query_parameters(
+            resource, query_string, query_parameters
+        )
 
-        if resource:
-            if isinstance(resource, str):
-                resource = valid_resource_name(resource)
-            # validate the given resource name
-            return FhirQuerySync(
-                base_url=self.api_address,
-                resource=resource,
-                auth=self.auth,
-                output_format=output_format,
-                proxies=self._proxies,
-                headers=self._headers,
-            )
-        elif query_string:
-            return self.raw_query(query_string, output_format)
+        query = FhirQuerySync(
+            base_url=self.api_address,
+            auth=self.auth,
+            query_parameters=query_parameters,
+            output_format=output_format,
+            proxies=self._proxies,
+            headers=self._headers,
+            client=self._sync_client(),
+        )
 
-        else:
-            return FhirQuerySync(
-                base_url=self.api_address,
-                auth=self.auth,
-                query_parameters=query_parameters,
-                output_format=output_format,
-                proxies=self._proxies,
-                headers=self._headers,
-            )
+        return query
 
     def query_async(
         self,
         resource: Union[Resource, FHIRAbstractModel, str] = None,
         query_string: str = None,
         query_parameters: FhirQueryParameters = None,
         output_format: str = "json",
     ) -> FhirQueryAsync:
         """
-        Initialize a FHIR query against the server with the given resource, query parameters or query string
+        Initialize an asynchronous FHIR query against the server with the given resource,
+        query parameters or query string
 
         Args:
             output_format: the output format to request from the fhir server (json or xml) defaults to json
             query_string: preformatted query string to execute against the servers REST API
             query_parameters: optionally pass in a query parameters object to use for the query
             resource: the FHIR resource to query from the server
 
         Returns:
             a FhirQueryAsync object that can be further modified with filters and conditions before being executed
             against the server
         """
 
         self._validate_query_input(resource, query_parameters, query_string)
+        query_parameters = self._setup_query_parameters(
+            resource, query_string, query_parameters
+        )
+
+        query = FhirQueryAsync(
+            self.api_address,
+            auth=self.auth,
+            headers=self._headers,
+            query_parameters=query_parameters,
+            output_format=output_format,
+            proxies=self._proxies,
+            client=self._async_client(),
+        )
+
+        return query
 
+    def _setup_query_parameters(
+        self,
+        resource: Union[Resource, FHIRAbstractModel, str] = None,
+        query_string: str = None,
+        query_parameters: FhirQueryParameters = None,
+    ) -> FhirQueryParameters:
+        """Initialize a FhirQueryParameters object from the given input
+
+        Args:
+            resource: Resource to use as base either string or model. Defaults to None.
+            query_string: Query string to transform into query parameters. Defaults to None.
+            query_parameters: Query parameters object that gets returned directly. Defaults to None.
+
+        Returns:
+            _description_
+        """
         if resource:
-            return FhirQueryAsync(
-                base_url=self.api_address,
-                resource=resource,
-                auth=self.auth,
-                output_format=output_format,
-                proxies=self._proxies,
-            )
+            if isinstance(resource, str):
+                query_parameters = FhirQueryParameters(resource=resource)
+            elif isinstance(resource, (Resource, FHIRAbstractModel)):
+                query_parameters = FhirQueryParameters(resource=resource.resource_type)
+
         elif query_string:
             query_parameters = FhirQueryParameters.from_query_string(query_string)
-            query = FhirQueryAsync(
-                self.api_address,
-                resource=query_parameters.resource,
-                query_parameters=query_parameters,
-                output_format=output_format,
-                proxies=self._proxies,
-            )
-            return query
 
-        else:
-            return FhirQueryAsync(
-                base_url=self.api_address,
-                auth=self.auth,
-                query_parameters=query_parameters,
-                output_format=output_format,
-                proxies=self._proxies,
-            )
+        return query_parameters
 
     def raw_query(
         self, query_string: str, output_format: str = "json"
     ) -> FhirQuerySync:
         """
         Execute a raw query string against the server
 
@@ -249,14 +273,15 @@
         query = FhirQuerySync(
             base_url=self.api_address,
             query_parameters=query_parameters,
             output_format=output_format,
             auth=self.auth,
             proxies=self._proxies,
             headers=self._headers,
+            client=self._sync_client(),
         )
         return query
 
     def raw_query_async(
         self, query_string: str, output_format: str = "json"
     ) -> FhirQueryAsync:
         """
@@ -275,14 +300,15 @@
         query = FhirQueryAsync(
             base_url=self.api_address,
             resource=query_parameters.resource,
             query_parameters=query_parameters,
             output_format=output_format,
             auth=self.auth,
             proxies=self._proxies,
+            client=self._async_client(),
         )
         return query
 
     def get(self, reference: Union[str, Reference]) -> FHIRAbstractModel:
         """
         Get a resource from the server specified by the given reference {ResourceType}/{id}
 
@@ -905,31 +931,68 @@
             except Exception as e:
                 print(r.text)
                 raise e
         response = r.json()
         self._meta_data = response
 
     def _sync_client(self) -> httpx.Client:
+        """Get a synchronous httpx client
+
+        Returns:
+            _httpx.Client: synchronous httpx client
+        """
+
+        transport = self._setup_transport()
         client = httpx.Client(
             headers=self.headers,
             auth=self.auth,
             proxies=self._proxies,
             timeout=self._timeout,
+            transport=transport,
         )
         return client
 
     def _async_client(self) -> httpx.AsyncClient:
+        transport = self._setup_transport(async_transport=True)
         client = httpx.AsyncClient(
             headers=self.headers,
             auth=self.auth,
             proxies=self._proxies,
             timeout=self._timeout,
+            transport=transport,
         )
         return client
 
+    def _setup_transport(
+        self, async_transport: bool = False
+    ) -> Union[RetryTransport, httpx.AsyncHTTPTransport, httpx.HTTPTransport]:
+        """Setup the transport for the httpx client if retryable methods or status codes are set
+        for the server the requests will be retried according to the configuration
+
+        Args:
+            async_transport: if True return an async transport
+        """
+
+        if self.retry_status_codes or self.retryable_methods:
+            return RetryTransport(
+                wrapped_transport=httpx.AsyncHTTPTransport()
+                if async_transport
+                else httpx.HTTPTransport(),
+                max_attempts=self.max_attempts,
+                backoff_factor=self.backoff_factor,
+                retry_status_codes=self.retry_status_codes,
+                retryable_methods=self.retryable_methods,
+                jitter_ratio=self.jitter_ratio,
+                max_backoff_wait=self.max_backoff_wait,
+            )
+        else:
+            return (
+                httpx.AsyncHTTPTransport() if async_transport else httpx.HTTPTransport()
+            )
+
     def _get_oidc_token(self):
         # get a new token if it is expired or not yet set
         if not self.oauth_token or self.oauth_token.is_expired():
             client = OAuth2Client(
                 client_id=self.client_id,
                 client_secret=self.client_secret,
                 token_endpoint_auth_method="client_secret_jwt",
```

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/server_responses.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_server/server_responses.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/summary.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_server/summary.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/transactions.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_server/transactions.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/transfer.py` & `fhir_kindling-1.0.1/fhir_kindling/fhir_server/transfer.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/figures/resource_plots.py` & `fhir_kindling-1.0.1/fhir_kindling/figures/resource_plots.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/figures/summary.py` & `fhir_kindling-1.0.1/fhir_kindling/figures/summary.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/generators/dataset.py` & `fhir_kindling-1.0.1/fhir_kindling/generators/dataset.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/generators/field_generator.py` & `fhir_kindling-1.0.1/fhir_kindling/generators/field_generator.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/generators/patient.py` & `fhir_kindling-1.0.1/fhir_kindling/generators/patient.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/generators/resource_generator.py` & `fhir_kindling-1.0.1/fhir_kindling/generators/resource_generator.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/generators/time_series_generator.py` & `fhir_kindling-1.0.1/fhir_kindling/generators/time_series_generator.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/privacy/k_anonymity.py` & `fhir_kindling-1.0.1/fhir_kindling/privacy/k_anonymity.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/serde/flatten.py` & `fhir_kindling-1.0.1/fhir_kindling/serde/flatten.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/conftest.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/server/test_transfer.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/server/test_transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 def test_transfer_resources(fhir_server):
     """
     Test the transfer resources
     """
     # get all conditions
     conditions = fhir_server.query("Condition").all().resource_list
 
-    target = FhirServer(api_address=os.getenv("TRANSFER_API_URL"))
+    target = FhirServer(api_address=os.getenv("TRANSFER_SERVER_URL"))
 
     response = transfer(source=fhir_server, target=target, resources=conditions)
 
     print(response)
     print(response.linkage)
     # save linkages
     response.save_linkage("linkage.json")
```

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_auth.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_fhir_query.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/test_fhir_query.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_fhir_server.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/test_fhir_server.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_generators.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_plots.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_privacy.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/test_privacy.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_serialization.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_util.py` & `fhir_kindling-1.0.1/fhir_kindling/tests/test_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -139,13 +139,23 @@
 def test_resource_contains_field(server):
     check_resource_contains_field("Patient", "birthDate")
     with pytest.raises(ValueError):
         check_resource_contains_field("Patient", "foo")
 
 
 def test_benchmark(server):
-    transfer_server = FhirServer(api_address=os.getenv("TRANSFER_API_URL"))
+    transfer_server = FhirServer(api_address=os.getenv("TRANSFER_SERVER_URL"))
     benchmark = ServerBenchmark(
         servers=[server, transfer_server], n_attempts=2, dataset_size=10
     )
     benchmark.run_suite(progress=False, save=False)
     # benchmark.plot()
+
+
+def test_retry_transport():
+    wrong_server_url = os.getenv("FHIR_API_URL") + "foo"
+    transfer_server = FhirServer(
+        api_address=wrong_server_url, retry_status_codes=[404], max_atttempts=3
+    )
+
+    with pytest.raises(Exception):
+        transfer_server.query("Patient").all()
```

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/util/references.py` & `fhir_kindling-1.0.1/fhir_kindling/util/references.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/fhir_kindling/util/resources.py` & `fhir_kindling-1.0.1/fhir_kindling/util/resources.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/LICENSE` & `fhir_kindling-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/pyproject.toml` & `fhir_kindling-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fhir-kindling"
-version = "1.0.0a9"
+version = "1.0.1"
 description = "Python library to simplify working with FHIR servers and resources."
 authors = ["Michael Graf <michael.graf3110@gmail.com>"]
 # todo add changelog when multiple readme bug is fixed
 readme = "README.md"
 packages = [{ include = "fhir_kindling" }]
 homepage = "https://migraf.github.io/fhir-kindling/"
 repository = "https://github.com/migraf/fhir-kindling"
@@ -33,15 +33,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 "fhir.resources" = "^6.0.0"
 pendulum = "*"
 tqdm = "*"
 orjson = "*"
 xmltodict = "*"
-pydantic = "*"
+pydantic = "^1.10.0"
 networkx = "*"
 httpx = "*"
 authlib = "*"
 pandas = { version = "*", optional = true }
 plotly = { version = "*", optional = true }
 faker = { version = "*", optional = true }
 matplotlib = { version = "*", optional = true }
```

### Comparing `fhir_kindling-1.0.0a9/README.md` & `fhir_kindling-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a9/setup.py` & `fhir_kindling-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,333 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fhir-kindling
+Version: 1.0.1
+Summary: Python library to simplify working with FHIR servers and resources.
+Home-page: https://migraf.github.io/fhir-kindling/
+License: MIT
+Keywords: python,fhir,hl7,client,medical records,healthcare,data
+Author: Michael Graf
+Author-email: michael.graf3110@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: demo
+Provides-Extra: ds
+Requires-Dist: RISE ; extra == "demo"
+Requires-Dist: authlib
+Requires-Dist: faker ; extra == "ds" or extra == "demo"
+Requires-Dist: fhir.resources (>=6.0.0,<7.0.0)
+Requires-Dist: httpx
+Requires-Dist: ipywidgets ; extra == "demo"
+Requires-Dist: kaleido (==0.2.1) ; extra == "ds" or extra == "demo"
+Requires-Dist: matplotlib ; extra == "ds" or extra == "demo"
+Requires-Dist: networkx
+Requires-Dist: notebook ; extra == "demo"
+Requires-Dist: orjson
+Requires-Dist: pandas ; extra == "ds" or extra == "demo"
+Requires-Dist: pendulum
+Requires-Dist: plotly ; extra == "ds" or extra == "demo"
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tqdm
+Requires-Dist: xmltodict
+Project-URL: Repository, https://github.com/migraf/fhir-kindling
+Description-Content-Type: text/markdown
+
+![Header](./docs/logo/kindling_header.png)
+
+[![CI](https://github.com/migraf/fhir-kindling/actions/workflows/main_ci.yml/badge.svg?branch=main)](https://github.com/migraf/fhir-kindling/actions/workflows/main_ci.yml)
+[![codecov](https://codecov.io/gh/migraf/fhir-kindling/branch/main/graph/badge.svg?token=FKQENFXACB)](https://codecov.io/gh/migraf/fhir-kindling)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Maintainability](https://api.codeclimate.com/v1/badges/3b83aa52724b6e75fc22/maintainability)](https://codeclimate.com/github/migraf/fhir-kindling/maintainability)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/fhir_kindling)
+![PyPI](https://img.shields.io/pypi/v/fhir_kindling)
+
+
+
+Python library for interacting with [HL7 FHIR](http://hl7.org/fhir/) servers and resources. Resource validation and parsing powered by
+[pydantic](https://github.com/samuelcolvin/pydantic) and the [fhir.resources](https://github.com/nazrulworld/fhir.resources) library.
+Provides a simple interface for synchronous and asynchronous CRUD operations for resources and bundles, 
+as well as resource transfer between servers.
+Datascience features include flattening of resources and bundles into tabular format (pandas dataframes) and plotting 
+methods for resources and bundles can optionally be included with the `ds` extra.
+
+Check out the [documentation](https://migraf.github.io/fhir-kindling/) for more information and a detailed user guide.
+
+
+Table of Contents
+=================
+
+- [Table of Contents](#table-of-contents)
+  - [Features](#features)
+  - [Installation](#installation)
+    - [Extras (optional)](#extras-optional)
+  - [Usage](#usage)
+    - [Connecting to a FHIR server](#connecting-to-a-fhir-server)
+    - [Query resources from the server](#query-resources-from-the-server)
+      - [Basic resource query](#basic-resource-query)
+      - [Query with filters](#query-with-filters)
+      - [Including related resources in the query](#including-related-resources-in-the-query)
+      - [Query resources by reference](#query-resources-by-reference)
+    - [Add resources to the server](#add-resources-to-the-server)
+    - [Deleting/Updating resources](#deletingupdating-resources)
+    - [Transfer resources between servers](#transfer-resources-between-servers)
+  - [Performance](#performance)
+  - [Contributing](#contributing)
+    - [Development](#development)
+    - [Tests](#tests)
+  - [Credits](#credits)
+
+## Features
+
+- Create, Read, Update, Delete resources using a FHIR server's REST API
+- Transfer resources between servers while maintaining referential integrity using server-given IDs
+- Bundle creation, validation and data management on a FHIR server via the REST API
+- Supports Hapi, Blaze and IBM FHIR servers
+- CSV serialization of query results
+- Synthetic data generation and
+
+
+
+<!-- Created by https://github.com/ekalinin/github-markdown-toc -->
+
+
+## Installation
+
+Install the package using pip:
+
+```shell
+pip install fhir-kindling --user
+```
+
+### Extras (optional)
+Fhir kindling can be used with the following extras:
+- `ds` for data science related features, such as flattening of resources into a tabular format
+
+```
+pip install fhir-kindling[ds] --user
+```
+
+## Usage
+
+### Connecting to a FHIR server
+
+```python
+from fhir_kindling import FhirServer
+
+# Connect with basic auth 
+basic_auth_server = FhirServer("https://fhir.server/fhir", username="admin", password="admin")
+# Connect with static token
+token_server = FhirServer("https://fhir.server/fhir", token="your_token")
+
+# Connect using oauth2/oidc
+oidc_server = FhirServer("https://fhir.server/fhir", client_id="client_id", client_secret="secret",
+                         oidc_provider_url="url")
+
+# Print the server's capability statement
+print(basic_auth_server.capabilities)
+
+```
+
+### Query resources from the server
+
+#### Basic resource query
+
+```python
+from fhir_kindling import FhirServer
+from fhir.resources.patient import Patient
+
+# Connect using oauth2/oidc
+oidc_server = FhirServer("https://fhir.server/fhir", client_id="client_id", client_secret="secret",
+                         oidc_provider_url="url")
+
+# query all patients on the server
+query = oidc_server.query(Patient, output_format="json").all()
+print(query.response)
+
+# Query resources based on name of resource
+query = oidc_server.query("Patient", output_format="json").all()
+print(query.response)
+```
+
+#### Query with filters
+
+Filtering the targeted resource is done using the `where` method on the query object. The filter is created by defining
+the target field, the comparison operator and the value to compare.
+
+```python
+from fhir_kindling import FhirServer
+
+server = FhirServer(api_address="https://fhir.server/fhir")
+
+query = server.query("Patient").where(field="birthDate", operator="gt", value="1980").all()
+```
+
+#### Including related resources in the query
+
+Resources that reference or are referenced by resources targeted by the query can be included in the response using
+the `include` method on the query object.
+
+```python
+# server initialization omitted
+# get the patients along with the queried conditions
+query_patient_condition = server.query("Condition").include(resource="Condition", reference_param="subject").all()
+
+# get the conditions for a patient
+query_patient_condition = server.query("Patient")
+query_patient_condition = query_patient_condition.include(resource="Condition", reference_param="subject", reverse=True)
+response = query_patient_condition.all()
+```
+
+#### Query resources by reference
+
+If you know the id and resource type of the resource you want to query, you can use the `get` method for a single
+reference
+for a list of references use `get_many`. The passed references should follow the format of `<resource_type>/<id>`.
+
+```python
+# server initialization omitted
+patient = server.get("Patient/123")
+
+patients = server.get_many(["Patient/123", "Patient/456"])
+
+```
+
+### Add resources to the server
+
+Resources can be added to the server using the `add` method on the server object. Lists of resources can be added using
+'add_all'.
+
+```python
+from fhir_kindling import FhirServer
+from fhir.resources.patient import Patient
+
+# Connect to the server
+server = FhirServer(api_address="https://fhir.server/fhir")
+
+# add a single resource
+patient = Patient(name=[{"family": "Smith", "given": ["John"]}])
+response = server.add(patient)
+
+# add multiple resources
+patients = [Patient(name=[{"family": f"Smith_{i}", "given": ["John"]}]) for i in range(10)]
+response = server.add_all(patients)
+```
+
+### Deleting/Updating resources
+
+Resources can be deleted from the server using the `delete` method on the server object, it takes as input either
+references to the resources or the resources itself.  
+Similarly the `update` method can be used to update the resources on the server, by passing a list of updated resources.
+
+```python
+from fhir_kindling import FhirServer
+from fhir.resources.patient import Patient
+
+# Connect to the server
+server = FhirServer(api_address="https://fhir.server/fhir")
+
+# add some patients
+patients = [Patient(name=[{"family": f"Smith_{i}", "given": ["John"]}]) for i in range(10)]
+response = server.add_all(patients)
+
+# change the name of the patients
+for patient in response.resources:
+    patient.name[0].given[0] = "Jane"
+
+# update the patients on the server
+updated_patients = server.update(resources=response.resources)
+
+# delete based on reference
+server.delete(references=response.references[:5])
+# delete based on resources
+server.delete(resources=response.resources[5:])
+```
+
+### Transfer resources between servers
+
+Transferring resources between servers is done using the `transfer` method on the server object. Using this method
+server assigned ids are used for transfer and referential integrity is maintained.  
+This method will also attempt to get all the resources that are referenced by the resources being transferred from the
+origin
+server and transfer them to the destination server as well.
+
+```python
+from fhir_kindling import FhirServer
+
+# initialize the two servers
+server_1 = FhirServer(api_address="https://fhir.server/fhir")
+server_2 = FhirServer(api_address="https://fhir.server/fhir")
+
+# query some resources from server 1
+conditions = server_1.query("Condition").limit(10)
+# transfer the resources to server 2
+response = server_1.transfer(server_2, resources=conditions.resources)
+
+```
+
+## Performance
+
+This library performs request at least 1.5 times faster than other popular python FHIR libraries.
+See [Benchmarks](benchmarks/README.md) for a more detailed description of the benchmarks.
+![Query Results](benchmarks/results/query_plot.png)
+
+
+## Contributing
+Contributions are very welcome and greatly appreciated! If you want to contribute to this project, please fork the 
+repository and make changes as you'd like. Pull requests are warmly welcome and credit will always be given.
+
+### Development
+
+To set up your environment to develop this package make sure you have [poetry](https://python-poetry.org/) installed and
+run the following commands:
+
+Install the dependencies:
+```bash
+poetry install --with dev --all-extras
+```
+
+Install pre-commit hooks:
+
+- Linting: [ruff](https://github.com/charliermarsh/ruff)
+- Formatting [black](https://black.readthedocs.io/en/stable/)
+
+```bash
+poetry run pre-commit install
+```
+
+### Tests
+To run the full test suit you need access to two FHIR servers (the second one is used for transfer tests).
+You can spin up two servers (one HAPI and one Blaze FHIR) using the compose file in the `testing` directory.
+```bash
+cd testing
+docker compose up
+```
+The servers will be available at `http://localhost:9090/fhir` and `http://localhost:9091/fhir` respectively.
+And the test should be configured to use them via the environment variables `FHIR_API_URL` and `TRANSFER_SERVER_URL` respectively.
+
+Run the tests:
+```bash
+poetry run pytest
+```
+
+
+## Credits
+
+This package was created with Cookiecutter and
+the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter) project template.
+
+
+
 
-packages = \
-['fhir_kindling',
- 'fhir_kindling.benchmark',
- 'fhir_kindling.fhir_query',
- 'fhir_kindling.fhir_server',
- 'fhir_kindling.figures',
- 'fhir_kindling.generators',
- 'fhir_kindling.privacy',
- 'fhir_kindling.serde',
- 'fhir_kindling.tests',
- 'fhir_kindling.tests.server',
- 'fhir_kindling.util']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['authlib',
- 'fhir.resources>=6.0.0,<7.0.0',
- 'httpx',
- 'networkx',
- 'orjson',
- 'pendulum',
- 'pydantic',
- 'tqdm',
- 'xmltodict']
-
-extras_require = \
-{'demo': ['pandas',
-          'plotly',
-          'faker',
-          'matplotlib',
-          'notebook',
-          'RISE',
-          'ipywidgets',
-          'kaleido==0.2.1'],
- 'ds': ['pandas', 'plotly', 'faker', 'matplotlib', 'kaleido==0.2.1']}
-
-setup_kwargs = {
-    'name': 'fhir-kindling',
-    'version': '1.0.0a9',
-    'description': 'Python library to simplify working with FHIR servers and resources.',
-    'long_description': '![Header](./docs/logo/kindling_header.png)\n\n[![CI](https://github.com/migraf/fhir-kindling/actions/workflows/main_ci.yml/badge.svg?branch=main)](https://github.com/migraf/fhir-kindling/actions/workflows/main_ci.yml)\n[![codecov](https://codecov.io/gh/migraf/fhir-kindling/branch/main/graph/badge.svg?token=FKQENFXACB)](https://codecov.io/gh/migraf/fhir-kindling)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Maintainability](https://api.codeclimate.com/v1/badges/3b83aa52724b6e75fc22/maintainability)](https://codeclimate.com/github/migraf/fhir-kindling/maintainability)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/fhir_kindling)\n![PyPI](https://img.shields.io/pypi/v/fhir_kindling)\n\n\n\nPython library for interacting with [HL7 FHIR](http://hl7.org/fhir/) servers and resources. Resource validation and parsing powered by\n[pydantic](https://github.com/samuelcolvin/pydantic) and the [fhir.resources](https://github.com/nazrulworld/fhir.resources) library.\nProvides a simple interface for synchronous and asynchronous CRUD operations for resources and bundles, \nas well as resource transfer between servers.\nDatascience features include flattening of resources and bundles into tabular format (pandas dataframes) and plotting \nmethods for resources and bundles can optionally be included with the `ds` extra.\n\nCheck out the [documentation](https://migraf.github.io/fhir-kindling/) for more information and a detailed user guide.\n\n\nTable of Contents\n=================\n\n- [Table of Contents](#table-of-contents)\n  - [Features](#features)\n  - [Installation](#installation)\n    - [Extras (optional)](#extras-optional)\n  - [Usage](#usage)\n    - [Connecting to a FHIR server](#connecting-to-a-fhir-server)\n    - [Query resources from the server](#query-resources-from-the-server)\n      - [Basic resource query](#basic-resource-query)\n      - [Query with filters](#query-with-filters)\n      - [Including related resources in the query](#including-related-resources-in-the-query)\n      - [Query resources by reference](#query-resources-by-reference)\n    - [Add resources to the server](#add-resources-to-the-server)\n    - [Deleting/Updating resources](#deletingupdating-resources)\n    - [Transfer resources between servers](#transfer-resources-between-servers)\n  - [Performance](#performance)\n  - [Contributing](#contributing)\n    - [Development](#development)\n    - [Tests](#tests)\n  - [Credits](#credits)\n\n## Features\n\n- Create, Read, Update, Delete resources using a FHIR server\'s REST API\n- Transfer resources between servers while maintaining referential integrity using server-given IDs\n- Bundle creation, validation and data management on a FHIR server via the REST API\n- Supports Hapi, Blaze and IBM FHIR servers\n- CSV serialization of query results\n- Synthetic data generation and\n\n\n\n<!-- Created by https://github.com/ekalinin/github-markdown-toc -->\n\n\n## Installation\n\nInstall the package using pip:\n\n```shell\npip install fhir-kindling --user\n```\n\n### Extras (optional)\nFhir kindling can be used with the following extras:\n- `ds` for data science related features, such as flattening of resources into a tabular format\n\n```\npip install fhir-kindling[ds] --user\n```\n\n## Usage\n\n### Connecting to a FHIR server\n\n```python\nfrom fhir_kindling import FhirServer\n\n# Connect with basic auth \nbasic_auth_server = FhirServer("https://fhir.server/fhir", username="admin", password="admin")\n# Connect with static token\ntoken_server = FhirServer("https://fhir.server/fhir", token="your_token")\n\n# Connect using oauth2/oidc\noidc_server = FhirServer("https://fhir.server/fhir", client_id="client_id", client_secret="secret",\n                         oidc_provider_url="url")\n\n# Print the server\'s capability statement\nprint(basic_auth_server.capabilities)\n\n```\n\n### Query resources from the server\n\n#### Basic resource query\n\n```python\nfrom fhir_kindling import FhirServer\nfrom fhir.resources.patient import Patient\n\n# Connect using oauth2/oidc\noidc_server = FhirServer("https://fhir.server/fhir", client_id="client_id", client_secret="secret",\n                         oidc_provider_url="url")\n\n# query all patients on the server\nquery = oidc_server.query(Patient, output_format="json").all()\nprint(query.response)\n\n# Query resources based on name of resource\nquery = oidc_server.query("Patient", output_format="json").all()\nprint(query.response)\n```\n\n#### Query with filters\n\nFiltering the targeted resource is done using the `where` method on the query object. The filter is created by defining\nthe target field, the comparison operator and the value to compare.\n\n```python\nfrom fhir_kindling import FhirServer\n\nserver = FhirServer(api_address="https://fhir.server/fhir")\n\nquery = server.query("Patient").where(field="birthDate", operator="gt", value="1980").all()\n```\n\n#### Including related resources in the query\n\nResources that reference or are referenced by resources targeted by the query can be included in the response using\nthe `include` method on the query object.\n\n```python\n# server initialization omitted\n# get the patients along with the queried conditions\nquery_patient_condition = server.query("Condition").include(resource="Condition", reference_param="subject").all()\n\n# get the conditions for a patient\nquery_patient_condition = server.query("Patient")\nquery_patient_condition = query_patient_condition.include(resource="Condition", reference_param="subject", reverse=True)\nresponse = query_patient_condition.all()\n```\n\n#### Query resources by reference\n\nIf you know the id and resource type of the resource you want to query, you can use the `get` method for a single\nreference\nfor a list of references use `get_many`. The passed references should follow the format of `<resource_type>/<id>`.\n\n```python\n# server initialization omitted\npatient = server.get("Patient/123")\n\npatients = server.get_many(["Patient/123", "Patient/456"])\n\n```\n\n### Add resources to the server\n\nResources can be added to the server using the `add` method on the server object. Lists of resources can be added using\n\'add_all\'.\n\n```python\nfrom fhir_kindling import FhirServer\nfrom fhir.resources.patient import Patient\n\n# Connect to the server\nserver = FhirServer(api_address="https://fhir.server/fhir")\n\n# add a single resource\npatient = Patient(name=[{"family": "Smith", "given": ["John"]}])\nresponse = server.add(patient)\n\n# add multiple resources\npatients = [Patient(name=[{"family": f"Smith_{i}", "given": ["John"]}]) for i in range(10)]\nresponse = server.add_all(patients)\n```\n\n### Deleting/Updating resources\n\nResources can be deleted from the server using the `delete` method on the server object, it takes as input either\nreferences to the resources or the resources itself.  \nSimilarly the `update` method can be used to update the resources on the server, by passing a list of updated resources.\n\n```python\nfrom fhir_kindling import FhirServer\nfrom fhir.resources.patient import Patient\n\n# Connect to the server\nserver = FhirServer(api_address="https://fhir.server/fhir")\n\n# add some patients\npatients = [Patient(name=[{"family": f"Smith_{i}", "given": ["John"]}]) for i in range(10)]\nresponse = server.add_all(patients)\n\n# change the name of the patients\nfor patient in response.resources:\n    patient.name[0].given[0] = "Jane"\n\n# update the patients on the server\nupdated_patients = server.update(resources=response.resources)\n\n# delete based on reference\nserver.delete(references=response.references[:5])\n# delete based on resources\nserver.delete(resources=response.resources[5:])\n```\n\n### Transfer resources between servers\n\nTransferring resources between servers is done using the `transfer` method on the server object. Using this method\nserver assigned ids are used for transfer and referential integrity is maintained.  \nThis method will also attempt to get all the resources that are referenced by the resources being transferred from the\norigin\nserver and transfer them to the destination server as well.\n\n```python\nfrom fhir_kindling import FhirServer\n\n# initialize the two servers\nserver_1 = FhirServer(api_address="https://fhir.server/fhir")\nserver_2 = FhirServer(api_address="https://fhir.server/fhir")\n\n# query some resources from server 1\nconditions = server_1.query("Condition").limit(10)\n# transfer the resources to server 2\nresponse = server_1.transfer(server_2, resources=conditions.resources)\n\n```\n\n## Performance\n\nThis library performs request at least 1.5 times faster than other popular python FHIR libraries.\nSee [Benchmarks](benchmarks/README.md) for a more detailed description of the benchmarks.\n![Query Results](benchmarks/results/query_plot.png)\n\n\n## Contributing\nContributions are very welcome and greatly appreciated! If you want to contribute to this project, please fork the \nrepository and make changes as you\'d like. Pull requests are warmly welcome and credit will always be given.\n\n### Development\n\nTo set up your environment to develop this package make sure you have [poetry](https://python-poetry.org/) installed and\nrun the following commands:\n\nInstall the dependencies:\n```bash\npoetry install --with dev --all-extras\n```\n\nInstall pre-commit hooks:\n\n- Linting: [ruff](https://github.com/charliermarsh/ruff)\n- Formatting [black](https://black.readthedocs.io/en/stable/)\n\n```bash\npoetry run pre-commit install\n```\n\n### Tests\nTo run the full test suit you need access to two FHIR servers (the second one is used for transfer tests).\nYou can spin up two servers (one HAPI and one Blaze FHIR) using the compose file in the `testing` directory.\n```bash\ncd testing\ndocker compose up\n```\nThe servers will be available at `http://localhost:9090/fhir` and `http://localhost:9091/fhir` respectively.\nAnd the test should be configured to use them via the environment variables `FHIR_API_URL` and `TRANSFER_SERVER_URL` respectively.\n\nRun the tests:\n```bash\npoetry run pytest\n```\n\n\n## Credits\n\nThis package was created with Cookiecutter and\nthe [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter) project template.\n\n\n\n\n\n',
-    'author': 'Michael Graf',
-    'author_email': 'michael.graf3110@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://migraf.github.io/fhir-kindling/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
 
 
-setup(**setup_kwargs)
```

