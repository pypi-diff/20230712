# Comparing `tmp/taktile_client-1.0.7.tar.gz` & `tmp/taktile_client-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taktile_client-1.0.7.tar", max compression
+gzip compressed data, was "taktile_client-1.0.8.tar", max compression
```

## Comparing `taktile_client-1.0.7.tar` & `taktile_client-1.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1093 2023-03-03 14:58:43.588203 taktile_client-1.0.7/PYPI.md
--rw-r--r--   0        0        0     1320 2023-03-03 14:58:43.588203 taktile_client-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      281 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/__init__.py
--rw-r--r--   0        0        0       80 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/arrow/__init__.py
--rw-r--r--   0        0        0     2592 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/arrow/client.py
--rw-r--r--   0        0        0     3717 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/arrow/endpoint.py
--rw-r--r--   0        0        0      447 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/arrow/serialize/__init__.py
--rw-r--r--   0        0        0     1222 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/arrow/serialize/codecs.py
--rw-r--r--   0        0        0     2407 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/arrow/serialize/factory.py
--rw-r--r--   0        0        0     8347 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/arrow/serialize/serializer.py
--rw-r--r--   0        0        0     2146 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/arrow/serialize/utils.py
--rw-r--r--   0        0        0     3417 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/arrow/utils.py
--rw-r--r--   0        0        0     2644 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/client.py
--rw-r--r--   0        0        0     2085 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/config.py
--rw-r--r--   0        0        0     3159 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/deployment_api.py
--rw-r--r--   0        0        0      985 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/exceptions.py
--rw-r--r--   0        0        0     3366 2023-03-03 14:58:43.588203 taktile_client-1.0.7/taktile_client/http_client.py
--rw-r--r--   0        0        0      837 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/model.py
--rw-r--r--   0        0        0        0 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/py.typed
--rw-r--r--   0        0        0       77 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/__init__.py
--rw-r--r--   0        0        0     1048 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/client.py
--rw-r--r--   0        0        0     4637 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/endpoint.py
--rw-r--r--   0        0        0     3395 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/serialize/__init__.py
--rw-r--r--   0        0        0     1228 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/serialize/dataframe.py
--rw-r--r--   0        0        0     1172 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/serialize/numpy.py
--rw-r--r--   0        0        0      347 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/serialize/pydantic_model.py
--rw-r--r--   0        0        0     1189 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/serialize/series.py
--rw-r--r--   0        0        0      179 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/serialize/utils.py
--rw-r--r--   0        0        0     5142 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/rest/utils.py
--rw-r--r--   0        0        0     1259 2023-03-03 14:58:43.592203 taktile_client-1.0.7/taktile_client/version.py
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 taktile_client-1.0.7/setup.py
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 taktile_client-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-07-12 09:16:47.820286 taktile_client-1.0.8/PYPI.md
+-rw-r--r--   0        0        0     1327 2023-07-12 09:16:47.820286 taktile_client-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      281 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/__init__.py
+-rw-r--r--   0        0        0       80 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/arrow/__init__.py
+-rw-r--r--   0        0        0     2592 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/arrow/client.py
+-rw-r--r--   0        0        0     3717 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/arrow/endpoint.py
+-rw-r--r--   0        0        0      447 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/arrow/serialize/__init__.py
+-rw-r--r--   0        0        0     1222 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/arrow/serialize/codecs.py
+-rw-r--r--   0        0        0     2407 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/arrow/serialize/factory.py
+-rw-r--r--   0        0        0     8347 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/arrow/serialize/serializer.py
+-rw-r--r--   0        0        0     2146 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/arrow/serialize/utils.py
+-rw-r--r--   0        0        0     3417 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/arrow/utils.py
+-rw-r--r--   0        0        0     2644 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/client.py
+-rw-r--r--   0        0        0     2085 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/config.py
+-rw-r--r--   0        0        0     3159 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/deployment_api.py
+-rw-r--r--   0        0        0      985 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/exceptions.py
+-rw-r--r--   0        0        0     3366 2023-07-12 09:16:47.820286 taktile_client-1.0.8/taktile_client/http_client.py
+-rw-r--r--   0        0        0      837 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/model.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/py.typed
+-rw-r--r--   0        0        0       77 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/__init__.py
+-rw-r--r--   0        0        0     1048 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/client.py
+-rw-r--r--   0        0        0     4637 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/endpoint.py
+-rw-r--r--   0        0        0     3395 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/serialize/__init__.py
+-rw-r--r--   0        0        0     1228 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/serialize/dataframe.py
+-rw-r--r--   0        0        0     1172 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/serialize/numpy.py
+-rw-r--r--   0        0        0      347 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/serialize/pydantic_model.py
+-rw-r--r--   0        0        0     1189 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/serialize/series.py
+-rw-r--r--   0        0        0      179 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/serialize/utils.py
+-rw-r--r--   0        0        0     5110 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/rest/utils.py
+-rw-r--r--   0        0        0     1259 2023-07-12 09:16:47.824286 taktile_client-1.0.8/taktile_client/version.py
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 taktile_client-1.0.8/setup.py
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 taktile_client-1.0.8/PKG-INFO
```

### Comparing `taktile_client-1.0.7/PYPI.md` & `taktile_client-1.0.8/PYPI.md`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/pyproject.toml` & `taktile_client-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "taktile-client"
-version = "1.0.7"
+version = "1.0.8"
 description = "A lightweight client to call models deployed on Taktile."
 readme = 'PYPI.md'
 authors = ["Taktile GmbH <devops@taktile.com>"]
 license = "Apache-2.0"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26.0"
 pydantic = "^1.8.2"
 numpy = { version = "^1.23", optional = true }
-pandas = { version = "^1.4", optional = true }
+pandas = { version = ">=1.4, <3.0", optional = true }
 pyarrow = { version = ">=8, <=11", optional = true }
 certifi = { version = "2021.10.8", optional = true }
 taktile-types = ">=0.17.0, <1.0.0"
 tenacity = "^8.0.1"
 packaging = "^23.0"
 setuptools = ">=0.0.0"
```

### Comparing `taktile_client-1.0.7/taktile_client/arrow/client.py` & `taktile_client-1.0.8/taktile_client/arrow/client.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/arrow/endpoint.py` & `taktile_client-1.0.8/taktile_client/arrow/endpoint.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/arrow/serialize/codecs.py` & `taktile_client-1.0.8/taktile_client/arrow/serialize/codecs.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/arrow/serialize/factory.py` & `taktile_client-1.0.8/taktile_client/arrow/serialize/factory.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/arrow/serialize/serializer.py` & `taktile_client-1.0.8/taktile_client/arrow/serialize/serializer.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/arrow/serialize/utils.py` & `taktile_client-1.0.8/taktile_client/arrow/serialize/utils.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/arrow/utils.py` & `taktile_client-1.0.8/taktile_client/arrow/utils.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/client.py` & `taktile_client-1.0.8/taktile_client/client.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/config.py` & `taktile_client-1.0.8/taktile_client/config.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/deployment_api.py` & `taktile_client-1.0.8/taktile_client/deployment_api.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/exceptions.py` & `taktile_client-1.0.8/taktile_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/http_client.py` & `taktile_client-1.0.8/taktile_client/http_client.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/model.py` & `taktile_client-1.0.8/taktile_client/model.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/rest/client.py` & `taktile_client-1.0.8/taktile_client/rest/client.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/rest/endpoint.py` & `taktile_client-1.0.8/taktile_client/rest/endpoint.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/rest/serialize/__init__.py` & `taktile_client-1.0.8/taktile_client/rest/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/rest/serialize/dataframe.py` & `taktile_client-1.0.8/taktile_client/rest/serialize/dataframe.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/rest/serialize/numpy.py` & `taktile_client-1.0.8/taktile_client/rest/serialize/numpy.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/rest/serialize/series.py` & `taktile_client-1.0.8/taktile_client/rest/serialize/series.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/taktile_client/rest/utils.py` & `taktile_client-1.0.8/taktile_client/rest/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,18 +80,18 @@
                 retry_state.attempt_number,
             )
             return True
         return False
 
     @tenacity.retry(
         stop=my_stop,
-        retry=tenacity.retry_if_exception_type(  # type: ignore
+        retry=tenacity.retry_if_exception_type(
             exception_types=(APIClientExceptionRetryable,)
         ),
-        wait=tenacity.wait_random(min=0, max=1),  # type: ignore
+        wait=tenacity.wait_random(min=0, max=1),
         after=my_after,
         reraise=True,
     )
     def wrapped() -> t.Any:
         try:
             response = api.call(
                 verb="post",
```

### Comparing `taktile_client-1.0.7/taktile_client/version.py` & `taktile_client-1.0.8/taktile_client/version.py`

 * *Files identical despite different names*

### Comparing `taktile_client-1.0.7/setup.py` & `taktile_client-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
  'requests>=2.26.0,<3.0.0',
  'setuptools>=0.0.0',
  'taktile-types>=0.17.0,<1.0.0',
  'tenacity>=8.0.1,<9.0.0']
 
 extras_require = \
 {'arrow': ['numpy>=1.23,<2.0',
-           'pandas>=1.4,<2.0',
+           'pandas>=1.4,<3.0',
            'pyarrow>=8,<=11',
            'certifi==2021.10.8']}
 
 setup_kwargs = {
     'name': 'taktile-client',
-    'version': '1.0.7',
+    'version': '1.0.8',
     'description': 'A lightweight client to call models deployed on Taktile.',
     'long_description': '# Taktile Client\n\n[![pypi status](https://img.shields.io/pypi/v/taktile-client.svg)](https://pypi.python.org/pypi/taktile-client)\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)\n\nTaktile enables data science teams to industrialize, scale, and maintain machine learning models. Our ML development platform makes it easy to create your own end-to-end ML applications:\n\n- Turn models into auto-scaling APIs in a few lines of code\n- Easily add model tests\n- Create and share model explanations through the Taktile UI\n\n`taktile-client` is a stand-alone python client which can be used to make requests to Taktile deployments via REST or [Arrow Flight](https://arrow.apache.org/docs/format/Flight.html). If you require the full Taktile dev tooling, consider installing [taktile-cli](https://pypi.org/project/taktile-cli/) instead. Find more information in our [docs](https://docs.taktile.com).\n\nTo install the REST client only, run `pip install taktile-client`. For both REST and Arrow, run `pip install taktile-client\\[arrow]`.\n',
     'author': 'Taktile GmbH',
     'author_email': 'devops@taktile.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `taktile_client-1.0.7/PKG-INFO` & `taktile_client-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taktile-client
-Version: 1.0.7
+Version: 1.0.8
 Summary: A lightweight client to call models deployed on Taktile.
 License: Apache-2.0
 Author: Taktile GmbH
 Author-email: devops@taktile.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: arrow
 Requires-Dist: certifi (==2021.10.8) ; extra == "arrow"
 Requires-Dist: numpy (>=1.23,<2.0) ; extra == "arrow"
 Requires-Dist: packaging (>=23.0,<24.0)
-Requires-Dist: pandas (>=1.4,<2.0) ; extra == "arrow"
+Requires-Dist: pandas (>=1.4,<3.0) ; extra == "arrow"
 Requires-Dist: pyarrow (>=8,<=11) ; extra == "arrow"
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: setuptools (>=0.0.0)
 Requires-Dist: taktile-types (>=0.17.0,<1.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Description-Content-Type: text/markdown
```

