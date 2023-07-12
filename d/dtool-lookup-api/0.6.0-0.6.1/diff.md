# Comparing `tmp/dtool-lookup-api-0.6.0.tar.gz` & `tmp/dtool-lookup-api-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtool-lookup-api-0.6.0.tar", last modified: Wed Apr 26 10:26:10 2023, max compression
+gzip compressed data, was "dtool-lookup-api-0.6.1.tar", last modified: Wed Jul 12 09:14:57 2023, max compression
```

## Comparing `dtool-lookup-api-0.6.0.tar` & `dtool-lookup-api-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.739995 dtool-lookup-api-0.6.0/dtool_lookup_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/dtool_lookup_api/core/
--rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/core/LookupClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/test_dtool_lookup_api_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/test_dtool_lookup_api_synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:14:57.703156 dtool-lookup-api-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-12 09:14:57.703156 dtool-lookup-api-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:14:57.699156 dtool-lookup-api-0.6.1/dtool_lookup_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/dtool_lookup_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/dtool_lookup_api/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:14:57.699156 dtool-lookup-api-0.6.1/dtool_lookup_api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    22419 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/dtool_lookup_api/core/LookupClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/dtool_lookup_api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/dtool_lookup_api/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/dtool_lookup_api/synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-12 09:14:57.000000 dtool-lookup-api-0.6.1/dtool_lookup_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:14:57.699156 dtool-lookup-api-0.6.1/dtool_lookup_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-12 09:14:57.000000 dtool-lookup-api-0.6.1/dtool_lookup_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-12 09:14:57.000000 dtool-lookup-api-0.6.1/dtool_lookup_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:14:57.000000 dtool-lookup-api-0.6.1/dtool_lookup_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-12 09:14:57.000000 dtool-lookup-api-0.6.1/dtool_lookup_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 09:14:57.000000 dtool-lookup-api-0.6.1/dtool_lookup_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-12 09:14:57.703156 dtool-lookup-api-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:14:57.703156 dtool-lookup-api-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:14:57.695155 dtool-lookup-api-0.6.1/tests/dtool/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:14:57.703156 dtool-lookup-api-0.6.1/tests/dtool/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/tests/dtool/config/dtool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/tests/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/tests/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/tests/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/tests/test_dtool_lookup_api_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/tests/test_dtool_lookup_api_synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-12 09:14:28.000000 dtool-lookup-api-0.6.1/tests/utils.py
```

### Comparing `dtool-lookup-api-0.6.0/CHANGELOG.rst` & `dtool-lookup-api-0.6.1/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGELOG
 =========
 
+0.6.1 (12Jul23)
+---------------
+
+- New dependency graph request schema in use.
+
 0.6.0 (26Apr23)
 ---------------
 
 - Server-side pagination
 
 0.5.1 (23Oct22)
 ---------------
```

### Comparing `dtool-lookup-api-0.6.0/CONTRIBUTING.md` & `dtool-lookup-api-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/CONTRIBUTORS.rst` & `dtool-lookup-api-0.6.1/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/LICENSE.rst` & `dtool-lookup-api-0.6.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/PKG-INFO` & `dtool-lookup-api-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dtool-lookup-api
-Version: 0.6.0
+Version: 0.6.1
 Summary: This package offers both synchronous and asynchronous implementations of a standardized Python API to communicate with the dtool lookup server.
 Home-page: https://github.com/IMTEK-Simulation/dtool-lookup-api
-Download-URL: https://github.com/IMTEK-Simulation/dtool-lookup-api/tarball/0.6.0
+Download-URL: https://github.com/IMTEK-Simulation/dtool-lookup-api/tarball/0.6.1
 Author: Johannes Laurin Hoermann
 Author-email: johannes.hoermann@imtek.uni-freiburg.de
 License: MIT
 Provides-Extra: testing
 License-File: LICENSE.rst
 
 README
```

### Comparing `dtool-lookup-api-0.6.0/README.rst` & `dtool-lookup-api-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/dtool_lookup_api/__init__.py` & `dtool-lookup-api-0.6.1/dtool_lookup_api/__init__.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/dtool_lookup_api/asynchronous.py` & `dtool-lookup-api-0.6.1/dtool_lookup_api/asynchronous.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/dtool_lookup_api/core/LookupClient.py` & `dtool-lookup-api-0.6.1/dtool_lookup_api/core/LookupClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,21 +96,22 @@
     def header(self):
         return {'Authorization': f'Bearer {self.token}'}
 
     def _check_json(self, json):
         if isinstance(json, dict) and 'msg' in json:
             raise LookupServerError(json['msg'])
 
-    async def _get(self, route, headers=None):
+    async def _get(self, route, headers={}):
         """Return information from a specific route."""
         async with self.session.get(
                 f'{self.lookup_url}{route}',
-                headers=headers or self.header, ssl=self.verify_ssl) as r:
+                headers=self.header, ssl=self.verify_ssl) as r:
             json = await r.json()
             self._check_json(json)
+            headers.update(**r.headers)
             return json
 
     async def _post(self, route, json, method='json', headers={}):
         """Wrapper for http post methpod.
 
         Parameters
         ----------
@@ -139,17 +140,29 @@
             headers.update(**r.headers)
             return json
 
     async def summary(self):
         """Overall summary of datasets accessible to a user."""
         return await self._get('/dataset/summary')
 
-    async def all(self):
+    async def all(self, page_number=1, page_size=20, pagination={}):
         """List all registered datasets."""
-        return await self._get('/dataset/list')
+        headers = {}
+        dataset_list = await self._get(f'/dataset/list?page={page_number}&page_size={page_size}', headers=headers)
+
+        if 'X-Pagination' in headers:
+            p = json.loads(headers['X-Pagination'])
+            pagination.update(**p)
+        else:
+            logger = logging.getLogger(__name__)
+            logger.warning("Server returned no pagination information. Server version outdated.")
+
+        return dataset_list
+
+
 
     async def aggregate(self, aggregation, page_number=1, page_size=20, pagination={}):
 
         """
               Execute a direct MongoDB aggregation.
 
               Parameters
@@ -339,15 +352,15 @@
             if 'X-Pagination' in headers:
                 p = json.loads(headers['X-Pagination'])
                 pagination.update(p)
             else:
                 logger = logging.getLogger(__name__)
                 logger.warning("Server returned no pagination information. Server version outdated.")
         else:  # TODO: validity check on dependency key list
-            dependency_graph = await self._post(f'/graph/lookup/{uuid}', dependency_keys)
+            dependency_graph = await self._post(f'/graph/lookup/{uuid}', {"dependency_keys": dependency_keys})
 
         return dependency_graph
 
     async def readme(self, uri):
         """Request the README.yml of a dataset by URI."""
         return await self._post('/dataset/readme', dict(uri=uri))
```

### Comparing `dtool-lookup-api-0.6.0/dtool_lookup_api/core/__init__.py` & `dtool-lookup-api-0.6.1/dtool_lookup_api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/dtool_lookup_api/core/config.py` & `dtool-lookup-api-0.6.1/dtool_lookup_api/core/config.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/dtool_lookup_api/synchronous.py` & `dtool-lookup-api-0.6.1/dtool_lookup_api/synchronous.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/PKG-INFO` & `dtool-lookup-api-0.6.1/dtool_lookup_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dtool-lookup-api
-Version: 0.6.0
+Version: 0.6.1
 Summary: This package offers both synchronous and asynchronous implementations of a standardized Python API to communicate with the dtool lookup server.
 Home-page: https://github.com/IMTEK-Simulation/dtool-lookup-api
-Download-URL: https://github.com/IMTEK-Simulation/dtool-lookup-api/tarball/0.6.0
+Download-URL: https://github.com/IMTEK-Simulation/dtool-lookup-api/tarball/0.6.1
 Author: Johannes Laurin Hoermann
 Author-email: johannes.hoermann@imtek.uni-freiburg.de
 License: MIT
 Provides-Extra: testing
 License-File: LICENSE.rst
 
 README
```

### Comparing `dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/SOURCES.txt` & `dtool-lookup-api-0.6.1/dtool_lookup_api.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 dtool_lookup_api/core/config.py
 tests/conftest.py
 tests/environ.py
 tests/metadata.py
 tests/run.sh
 tests/test_dtool_lookup_api_basics.py
 tests/test_dtool_lookup_api_synchronous.py
-tests/utils.py
+tests/utils.py
+tests/dtool/config/dtool.json
```

### Comparing `dtool-lookup-api-0.6.0/setup.py` & `dtool-lookup-api-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/tests/conftest.py` & `dtool-lookup-api-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/tests/environ.py` & `dtool-lookup-api-0.6.1/tests/environ.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/tests/metadata.py` & `dtool-lookup-api-0.6.1/tests/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -152,19 +152,19 @@
         "utc_timestamp": False,
     }
 )
 
 # query
 
 DEFAULT_QUERY = {
-    'base_uri': 'smb://test-share',
+    'base_uri': 's3://test-bucket',
     'name': {'$regex': 'test'},
 }
-EXPECTED_DEFAULT_QUERY_RESPONSE = [ALL_METADTA[1]]
-EXPECTED_DEFAULT_QUERY_RESPONSE_IMMUTABLE_MARKER = [ALL_METADTA_IMMUTABLE_MARKER[1]]
+EXPECTED_DEFAULT_QUERY_RESPONSE = [ALL_METADTA[0]]
+EXPECTED_DEFAULT_QUERY_RESPONSE_IMMUTABLE_MARKER = [ALL_METADTA_IMMUTABLE_MARKER[0]]
 
 # readme
 
 DEFAULT_README_URI = 'smb://test-share/1a1f9fad-8589-413e-9602-5bbd66bfe675'
 EXPECTED_DEFAULT_README_RESPONSE = {
     "creation_date": "2020-11-08",
     "description": "testing description",
@@ -194,48 +194,41 @@
 DEFAULT_SEARCH_TEXT = "test"
 EXPECTED_DEFAULT_SEARCH_RESPONSE = ALL_METADTA
 EXPECTED_DEFAULT_SEARCH_RESPONSE_IMMUTABLE_MARKER = ALL_METADTA_IMMUTABLE_MARKER
 
 # config
 
 EXPECTED_CONFIG_RESPONSE = {
-    "dtool_lookup_server_dependency_graph_plugin": {
-        "dependency_keys": [
-            "readme.derived_from.uuid",
-            "annotations.source_dataset_uuid"
-        ],
-        "dynamic_dependency_keys": True,
-        "enable_dependency_view": True,
-        "force_rebuild_dependency_view": False,
-        "mongo_dependency_view_bookkeeping": "dep_views",
-        "mongo_dependency_view_cache_size": 10,
-        "mongo_dependency_view_prefix": "dep:",
-        "version": "0.1.3"
-    },
-    "dtool_lookup_server_direct_mongo_plugin": {
-        "allow_direct_aggregation": False,
-        "allow_direct_query": True,
-        "version": "0.1.2"
-    },
+    # dependency graph plugin
+    "dependency_keys": [
+        "readme.derived_from.uuid",
+        "annotations.source_dataset_uuid"
+    ],
+    "dynamic_dependency_keys": True,
+    "enable_dependency_view": True,
+    "force_rebuild_dependency_view": False,
+    "mongo_dependency_view_bookkeeping": "dep_views",
+    "mongo_dependency_view_cache_size": 10,
+    "mongo_dependency_view_prefix": "dep:",
+    # direct mongo plugin
+    "allow_direct_aggregation": True,
+    "allow_direct_query": True,
+    # other
     "jsonify_prettyprint_regular": True,
     "jwt_algorithm": "RS256",
     "jwt_header_name": "Authorization",
     "jwt_header_type": "Bearer",
     "jwt_public_key": "",
     "jwt_token_location": "headers",
     "sqlalchemy_track_modifications": False,
-    "version": "0.15.0"
 }
 
 EXPECTED_CONFIG_RESPONSE_IMMUTABLE_MARKER = _make_marker(EXPECTED_CONFIG_RESPONSE)
 EXPECTED_CONFIG_RESPONSE_IMMUTABLE_MARKER["jwt_public_key"] = False
-EXPECTED_CONFIG_RESPONSE_IMMUTABLE_MARKER["version"] = False
-EXPECTED_CONFIG_RESPONSE_IMMUTABLE_MARKER["dtool_lookup_server_dependency_graph_plugin"]["version"] = False
-EXPECTED_CONFIG_RESPONSE_IMMUTABLE_MARKER["dtool_lookup_server_direct_mongo_plugin"]["version"] = False
-EXPECTED_CONFIG_RESPONSE_IMMUTABLE_MARKER["dtool_lookup_server_direct_mongo_plugin"]["allow_direct_aggregation"] = False
+# EXPECTED_CONFIG_RESPONSE_IMMUTABLE_MARKER["dtool_lookup_server_direct_mongo_plugin"]["allow_direct_aggregation"] = False
 
 
 # user info
 
 DEFAULT_USER_INFO_USER_NAME = 'testuser'
 EXPECTED_DEFAULT_USER_INFO_RESPONSE = {
     'is_admin': True,
@@ -248,16 +241,14 @@
 
 # admin routes
 
 # list users
 
 EXPECTED_DEFAULT_LIST_USERS_RESPONSE = [{
     'is_admin': True,
-    'register_permissions_on_base_uris': [],
-    'search_permissions_on_base_uris': ['smb://test-share'],
     'username': 'testuser'
 }]
 EXPECTED_DEFAULT_LIST_USERS_RESPONSE_IMMUTABLE_MARKER = _make_marker(EXPECTED_DEFAULT_LIST_USERS_RESPONSE)
 
 # permission info
 DEFAULT_PERMISSION_INFO_BASE_URI = 'smb://test-share'
 EXPECTED_DEFAULT_PERMISSION_INFO_RESPONSE = {
```

### Comparing `dtool-lookup-api-0.6.0/tests/run.sh` & `dtool-lookup-api-0.6.1/tests/run.sh`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.6.0/tests/test_dtool_lookup_api_synchronous.py` & `dtool-lookup-api-0.6.1/tests/test_dtool_lookup_api_synchronous.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Test synchronous lookup api."""
 
 import logging
 import pytest
+import yaml
 
-from utils import _log_nested_dict, _compare
+from utils import _log_nested_dict, _compare, NoDatesSafeLoader
 
 # TODO: in need for more elegant way to outsource default queries and expected responses
 from metadata import (
     EXPECTED_DEFAULT_ALL_RESPONSE, EXPECTED_DEFAULT_ALL_RESPONSE_IMMUTABLE_MARKER,
     DEFAULT_AGGREGATION, EXPECTED_DEFAULT_AGGREGATION_RESPONSE, EXPECTED_DEFAULT_AGGREGATION_RESPONSE_IMMUTABLE_MARKER,
     EXPECTED_CONFIG_RESPONSE, EXPECTED_CONFIG_RESPONSE_IMMUTABLE_MARKER,
     DEFAULT_LOOKUP_UUID, EXPECTED_DEFAULT_LOOKUP_RESPONSE, EXPECTED_DEFAULT_LOOKUP_RESPONSE_IMMUTABLE_MARKER,
@@ -42,15 +43,15 @@
         EXPECTED_DEFAULT_ALL_RESPONSE_IMMUTABLE_MARKER,
     )
 
     assert compares
 
 
 @pytest.mark.usefixtures("dtool_lookup_server", "dtool_config")
-def test_defaut_aggregation():
+def test_default_aggregation():
     """Will send a direct mongo query request to the server."""
     from dtool_lookup_api.synchronous import aggregate
 
     logger = logging.getLogger(__name__)
 
     response = aggregate(DEFAULT_AGGREGATION)
     assert response is not None
@@ -87,15 +88,15 @@
         EXPECTED_CONFIG_RESPONSE_IMMUTABLE_MARKER,
     )
 
     assert compares
 
 
 @pytest.mark.usefixtures("dtool_lookup_server", "dtool_config")
-def test_defaut_lookup():
+def test_default_lookup():
     """Will send a direct mongo query request to the server."""
     from dtool_lookup_api.synchronous import lookup
 
     logger = logging.getLogger(__name__)
 
     response = lookup(DEFAULT_LOOKUP_UUID)
     assert response is not None
@@ -108,15 +109,15 @@
         EXPECTED_DEFAULT_LOOKUP_RESPONSE,
         EXPECTED_DEFAULT_LOOKUP_RESPONSE_IMMUTABLE_MARKER
     )
     assert compares
 
 
 @pytest.mark.usefixtures("dtool_lookup_server", "dtool_config")
-def test_defaut_manifest():
+def test_default_manifest():
     """Will send a direct mongo query request to the server."""
     from dtool_lookup_api.synchronous import manifest
 
     logger = logging.getLogger(__name__)
 
     response = manifest(DEFAULT_MANIFEST_URI)
     assert response is not None
@@ -129,15 +130,15 @@
         EXPECTED_DEFAULT_MANIFEST_RESPONSE,
         EXPECTED_DEFAULT_MANIFEST_RESPONSE_IMMUTABLE_MARKER
     )
     assert compares
 
 
 @pytest.mark.usefixtures("dtool_lookup_server", "dtool_config")
-def test_defaut_query():
+def test_default_query():
     """Will send a direct mongo query request to the server."""
     from dtool_lookup_api.synchronous import query
 
     logger = logging.getLogger(__name__)
 
     response = query(DEFAULT_QUERY)
     assert response is not None
@@ -162,18 +163,22 @@
 
     logger = logging.getLogger(__name__)
 
     response = readme(DEFAULT_README_URI)
     assert response is not None
 
     logger.debug("Response:")
-    _log_nested_dict(logger.debug, response)
+    logger.debug(response)
+
+    logger.debug("Parsed:")
+    parsed_readme = yaml.load(response, Loader=NoDatesSafeLoader)
+    _log_nested_dict(logger.debug, parsed_readme)
 
     compares = _compare(
-        response,
+        parsed_readme,
         EXPECTED_DEFAULT_README_RESPONSE,
         EXPECTED_DEFAULT_README_RESPONSE_IMMUTABLE_MARKER
     )
     assert compares
 
 
 @pytest.mark.usefixtures("dtool_lookup_server", "dtool_config")
@@ -246,43 +251,43 @@
         EXPECTED_DEFAULT_LIST_USERS_RESPONSE,
         EXPECTED_DEFAULT_LIST_USERS_RESPONSE_IMMUTABLE_MARKER
     )
     assert compares
 
 
 # TODO: clean up, i.e. delete users after use
-@pytest.mark.usefixtures("dtool_lookup_server", "dtool_config")
-def test_default_register_user():
-    """Will send a register user request to the server."""
-    from dtool_lookup_api.synchronous import register_user
-
-    logger = logging.getLogger(__name__)
-
-    # mimic https://github.com/jic-dtool/dtool-lookup-server/blob/12baba73eebc668b4998ae2c2ea43946dc3bf856/tests/test_admin_user_routes.py#L14
-    users = [
-        {"username": "evil-witch", "is_admin": True},
-        {"username": "dopey"}
-    ]
-
-    # TODO: check for nonexistence of not yet registered users on server
-
-    for user in users:
-        response = register_user(**user)
-        assert response == True
-        logger.debug("Response:")
-        _log_nested_dict(logger.debug, response)
-
-    # Ensure idempotent.
-    for user in users:
-        response = register_user(**user)
-        assert response == True
-        logger.debug("Response:")
-        _log_nested_dict(logger.debug, response)
-
-    # TODO: check for existence of registered users on server
+# @pytest.mark.usefixtures("dtool_lookup_server", "dtool_config")
+# def test_default_register_user():
+#    """Will send a register user request to the server."""
+#    from dtool_lookup_api.synchronous import register_user
+#
+#    logger = logging.getLogger(__name__)
+#
+#    # mimic https://github.com/jic-dtool/dtool-lookup-server/blob/12baba73eebc668b4998ae2c2ea43946dc3bf856/tests/test_admin_user_routes.py#L14
+#    users = [
+#        {"username": "evil-witch", "is_admin": True},
+#        {"username": "dopey"}
+#    ]
+#
+#    # TODO: check for nonexistence of not yet registered users on server
+#
+#    for user in users:
+#        response = register_user(**user)
+#        assert response == True
+#        logger.debug("Response:")
+#        _log_nested_dict(logger.debug, response)
+#
+#    # Ensure idempotent.
+#    for user in users:
+#        response = register_user(**user)
+#        assert response == True
+#        logger.debug("Response:")
+#        _log_nested_dict(logger.debug, response)
+#
+#    # TODO: check for existence of registered users on server
 
 
 # mark to run early in order to not have any other users registered in database by other tests
 @pytest.mark.first
 @pytest.mark.usefixtures("dtool_lookup_server", "dtool_config")
 def test_default_permission_info():
     """Will send a permission info request to the server."""
```

