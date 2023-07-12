# Comparing `tmp/mopinion-1.0.0.tar.gz` & `tmp/mopinion-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mopinion-1.0.0.tar", last modified: Fri Mar  4 12:04:54 2022, max compression
+gzip compressed data, was "mopinion-1.0.1.tar", last modified: Wed Jul 12 07:40:15 2023, max compression
```

## Comparing `mopinion-1.0.0.tar` & `mopinion-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2022-03-04 12:04:54.633236 mopinion-1.0.0/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1363 2022-03-04 09:44:06.000000 mopinion-1.0.0/CHANGES.rst
--rw-rw-r--   0 jose      (1000) jose      (1000)     1075 2021-02-13 00:37:58.000000 mopinion-1.0.0/LICENSE
--rw-rw-r--   0 jose      (1000) jose      (1000)       58 2021-02-13 00:37:58.000000 mopinion-1.0.0/MANIFEST.in
--rw-rw-r--   0 jose      (1000) jose      (1000)     5902 2022-03-04 12:04:54.633236 mopinion-1.0.0/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)     2824 2022-02-23 10:24:57.000000 mopinion-1.0.0/README.rst
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2022-03-04 12:04:54.633236 mopinion-1.0.0/mopinion/
--rw-rw-r--   0 jose      (1000) jose      (1000)       43 2021-02-13 00:37:58.000000 mopinion-1.0.0/mopinion/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    21697 2022-02-23 10:06:54.000000 mopinion-1.0.0/mopinion/client.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     3319 2022-02-23 10:06:54.000000 mopinion-1.0.0/mopinion/dataclasses.py
--rw-rw-r--   0 jose      (1000) jose      (1000)      345 2022-02-23 10:06:54.000000 mopinion-1.0.0/mopinion/settings.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2022-03-04 12:04:54.633236 mopinion-1.0.0/mopinion.egg-info/
--rw-rw-r--   0 jose      (1000) jose      (1000)     5902 2022-03-04 12:04:54.000000 mopinion-1.0.0/mopinion.egg-info/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)      371 2022-03-04 12:04:54.000000 mopinion-1.0.0/mopinion.egg-info/SOURCES.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2022-03-04 12:04:54.000000 mopinion-1.0.0/mopinion.egg-info/dependency_links.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       20 2022-03-04 12:04:54.000000 mopinion-1.0.0/mopinion.egg-info/entry_points.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2021-02-13 00:38:16.000000 mopinion-1.0.0/mopinion.egg-info/not-zip-safe
--rw-rw-r--   0 jose      (1000) jose      (1000)      124 2022-03-04 12:04:54.000000 mopinion-1.0.0/mopinion.egg-info/requires.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        9 2022-03-04 12:04:54.000000 mopinion-1.0.0/mopinion.egg-info/top_level.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)      332 2022-03-04 12:04:54.633236 mopinion-1.0.0/setup.cfg
--rw-rw-r--   0 jose      (1000) jose      (1000)     1351 2022-03-04 09:44:06.000000 mopinion-1.0.0/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-12 07:40:15.752846 mopinion-1.0.1/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1483 2023-07-12 07:10:58.000000 mopinion-1.0.1/CHANGES.rst
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1075 2023-07-09 08:13:57.000000 mopinion-1.0.1/LICENSE
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2023-07-09 08:13:57.000000 mopinion-1.0.1/MANIFEST.in
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4769 2023-07-12 07:40:15.752846 mopinion-1.0.1/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2023-07-12 07:10:58.000000 mopinion-1.0.1/README.rst
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-12 07:40:15.752846 mopinion-1.0.1/mopinion/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       43 2023-07-09 08:13:57.000000 mopinion-1.0.1/mopinion/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    21798 2023-07-12 07:10:58.000000 mopinion-1.0.1/mopinion/client.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3319 2023-07-11 10:05:45.000000 mopinion-1.0.1/mopinion/dataclasses.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      345 2023-07-11 07:13:04.000000 mopinion-1.0.1/mopinion/settings.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-12 07:40:15.752846 mopinion-1.0.1/mopinion.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4769 2023-07-12 07:40:15.000000 mopinion-1.0.1/mopinion.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      336 2023-07-12 07:40:15.000000 mopinion-1.0.1/mopinion.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-12 07:40:15.000000 mopinion-1.0.1/mopinion.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-12 07:40:15.000000 mopinion-1.0.1/mopinion.egg-info/not-zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      124 2023-07-12 07:40:15.000000 mopinion-1.0.1/mopinion.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        9 2023-07-12 07:40:15.000000 mopinion-1.0.1/mopinion.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2023-07-12 07:40:15.752846 mopinion-1.0.1/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1355 2023-07-12 07:14:56.000000 mopinion-1.0.1/setup.py
```

### Comparing `mopinion-1.0.0/CHANGES.rst` & `mopinion-1.0.1/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Changelog
 ========================================================
 
 
+1.0.1 (2023-07-11)
+-------------------
+- Fix issue where query parameters are not properly set for iterable responses.
+
 1.0.0 (2022-03-04)
 -------------------
 
 - Released stable version.
 
 
 0.0.7 (2022-02-23)
```

### Comparing `mopinion-1.0.0/LICENSE` & `mopinion-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mopinion-1.0.0/PKG-INFO` & `mopinion-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,177 @@
 Metadata-Version: 2.1
 Name: mopinion
-Version: 1.0.0
+Version: 1.0.1
 Summary: A client library for the Mopinion Data API
-Home-page: https://github.com/mopinion/mopinion-python-api
+Home-page: https://github.com/Mopinion-com/mopinion-python-api
 Author: Mopinion
 Author-email: 
 License: MIT License
-Description: Mopinion API - Python Client
-        ==========================================
-        
-        .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
-            :target: https://github.com/mopinion/mopinion-python-api/blob/master/LICENSE
-            :alt: License-MIT
-        
-        .. image:: https://readthedocs.org/projects/mopinion-python-api/badge/?version=latest
-            :target: https://mopinion-python-api.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://github.com/mopinion/mopinion-python-api/workflows/Test%20Suite/badge.svg/
-            :alt: GitHub Actions
-        
-        .. image:: https://badge.fury.io/py/mopinion.svg/
-            :target: https://badge.fury.io/py/mopinion/
-            :alt: Badge PyPi
-        
-        
-        A client library for the `Mopinion Data API <https://developer.mopinion.com/api/>`_.
-        
-        Our Mopinion Client provides functionality for authentication, authorization and requesting resources.
-        It comes with an easy, beautiful, and elegant way of interacting with our API.
-        
-        `Read the docs <https://mopinion-python-api.readthedocs.io/en/latest/>`_ for further information.
-        
-        Installation
-        -------------
-        
-        Install using ``pip``::
-        
-            pip install mopinion
-        
-        
-        Example
-        --------
-        
-        .. code:: python
-        
-            >>> from mopinion import MopinionClient
-            >>> client = MopinionClient(public_key=PUBLIC_KEY, private_key=PRIVATE_KEY)
-            >>> assert client.is_available()
-            >>> response = client.resource("account")
-            >>> response = client.resource("deployments")
-            >>>
-            >>> response = client.get_account()
-            >>>
-            >>> response = client.get_deployments()
-            >>> response = client.get_deployments("abc")
-            >>>
-            >>> response = client.get_reports(report_id=123)
-            >>> response = client.get_reports_fields(report_id=123)
-            >>> response = client.get_reports_feedback(report_id=123)
-            >>>
-            >>> response = client.get_datasets(dataset_id=123)
-            >>> response = client.get_datasets_feedback(dataset_id=123)
-            >>> response = client.get_datasets_fields(dataset_id=123)
-            >>>
-            >>> client.close()
-            >>>
-            >>> with MopinionClient(public_key=YOUR_PUBLIC_KEY, private_key=YOUR_PRIVATE_KEY) as client:
-            ...     response = client.get_account()
-            ...     assert response.json()["_meta"]["code"] == 200
-        
-        Documentation
-        ---------------
-        
-        You can find here at `Read the docs <https://mopinion-python-api.readthedocs.io/en/latest/>`_ the complete documentation.
-        
-        
-        About Mopinion
-        ---------------
-        
-        `Mopinion <https://mopinion.com/>`_ is a leading all-in-one user feedback platform that helps digital enterprises listen, understand,
-        and act across all digital touchpoints (web, mobile, and email). Join some of the most forward-thinking
-        digital teams from companies such as T-mobile, eBay, TSB Bank, Walmart, Hotels.com, Decathlon, Ahold,
-        Mediacorp Ltd, and many more.
-        
-        Please visit the website for more information about the product: https://mopinion.com
-        
-        
-        Changelog
-        ========================================================
-        
-        
-        1.0.0 (2022-03-04)
-        -------------------
-        
-        - Released stable version.
-        
-        
-        0.0.7 (2022-02-23)
-        -------------------
-        
-        - Fixes in documentation.
-        
-        - Implement `__enter__()` and `__exit__()` methods.
-        
-        - Added methods: `get_account`, `get_deployments`,
-          `get_datasets`, `get_datasets_fields`,
-          `get_datasets_feedback`, `get_reports`,
-          `get_reports_fields`, `get_reports_feedback`.
-        
-        - Increased compatibility from Python 3.6 to 3.10.
-        
-        
-        0.0.6 (2021-02-11)
-        -------------------
-        
-        - Fixes in documentation.
-        
-        - Added pre-commit configuration to project.
-        
-        - Added new endpoint for `/deployments/<str_id>`.
-        
-        
-        0.0.5 (2021-01-22)
-        -------------------
-        
-        - Several fixes in documentation.
-        
-        
-        0.0.4 (2021-01-22)
-        -------------------
-        
-        - Fixed in documentation.
-        
-        - Added examples for `query_params` in the doc examples.
-        
-        - Updated directory name from `mopinion_client` to `mopinion`.
-        
-        - Implemented About in Docs and Readme.
-        
-        0.0.3 (2021-01-20)
-        -------------------
-        
-        - Fixed typing in method `get_token`. Return `bytes` instead of `str`.
-        
-        0.0.2 (2021-01-20)
-        -------------------
-        
-        - Fixed in documentation.
-        
-        - Removed travis ci. Integrated GitHub Actions.
-        
-        - Added coverage into GitHub actions.
-        
-        0.0.1 (2021-01-20)
-        -------------------
-        
-        - Initial project structure.
-        
-        - Client implementation.
-        
-        - Test suite.
-        
-        - Request examples.
-        
 Keywords: mopinion
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Provides-Extra: test
+License-File: LICENSE
+
+Mopinion API - Python Client
+==========================================
+
+.. image:: https://img.shields.io/badge/License-MIT-yellow.svg
+    :target: https://github.com/Mopinion-com/mopinion-python-api/blob/master/LICENSE
+    :alt: License-MIT
+
+.. image:: https://readthedocs.org/projects/mopinion-python-api/badge/?version=latest
+    :target: https://mopinion-python-api.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://github.com/Mopinion-com/mopinion-python-api/workflows/Test%20Suite/badge.svg/
+    :alt: GitHub Actions
+
+.. image:: https://badge.fury.io/py/mopinion.svg/
+    :target: https://badge.fury.io/py/mopinion/
+    :alt: Badge PyPi
+
+
+A client library for the `Mopinion Data API <https://developer.mopinion.com/api/>`_.
+
+Our Mopinion Client provides functionality for authentication, authorization and requesting resources.
+It comes with an easy, beautiful, and elegant way of interacting with our API.
+
+`Read the docs <https://mopinion-python-api.readthedocs.io/en/latest/>`_ for further information.
+
+Installation
+-------------
+
+Install using ``pip``::
+
+    pip install mopinion
+
+
+Example
+--------
+
+.. code:: python
+
+    >>> from mopinion import MopinionClient
+    >>> client = MopinionClient(public_key=PUBLIC_KEY, private_key=PRIVATE_KEY)
+    >>> assert client.is_available()
+    >>> response = client.resource("account")
+    >>> response = client.resource("deployments")
+    >>>
+    >>> response = client.get_account()
+    >>>
+    >>> response = client.get_deployments()
+    >>> response = client.get_deployments("abc")
+    >>>
+    >>> response = client.get_reports(report_id=123)
+    >>> response = client.get_reports_fields(report_id=123)
+    >>> response = client.get_reports_feedback(report_id=123)
+    >>>
+    >>> response = client.get_datasets(dataset_id=123)
+    >>> response = client.get_datasets_feedback(dataset_id=123)
+    >>> response = client.get_datasets_fields(dataset_id=123)
+    >>>
+    >>> client.close()
+    >>>
+    >>> with MopinionClient(public_key=YOUR_PUBLIC_KEY, private_key=YOUR_PRIVATE_KEY) as client:
+    ...     response = client.get_account()
+    ...     assert response.json()["_meta"]["code"] == 200
+
+Documentation
+---------------
+
+You can find here at `Read the docs <https://mopinion-python-api.readthedocs.io/en/latest/>`_ the complete documentation.
+
+
+About Mopinion
+---------------
+
+`Mopinion <https://mopinion.com/>`_ is a leading all-in-one user feedback platform that helps digital enterprises listen, understand,
+and act across all digital touchpoints (web, mobile, and email). Join some of the most forward-thinking
+digital teams from companies such as T-mobile, eBay, TSB Bank, Walmart, Hotels.com, Decathlon, Ahold,
+Mediacorp Ltd, and many more.
+
+Please visit the website for more information about the product: https://mopinion.com
+
+
+Changelog
+========================================================
+
+
+1.0.1 (2023-07-11)
+-------------------
+- Fix issue where query parameters are not properly set for iterable responses.
+
+1.0.0 (2022-03-04)
+-------------------
+
+- Released stable version.
+
+
+0.0.7 (2022-02-23)
+-------------------
+
+- Fixes in documentation.
+
+- Implement `__enter__()` and `__exit__()` methods.
+
+- Added methods: `get_account`, `get_deployments`,
+  `get_datasets`, `get_datasets_fields`,
+  `get_datasets_feedback`, `get_reports`,
+  `get_reports_fields`, `get_reports_feedback`.
+
+- Increased compatibility from Python 3.6 to 3.10.
+
+
+0.0.6 (2021-02-11)
+-------------------
+
+- Fixes in documentation.
+
+- Added pre-commit configuration to project.
+
+- Added new endpoint for `/deployments/<str_id>`.
+
+
+0.0.5 (2021-01-22)
+-------------------
+
+- Several fixes in documentation.
+
+
+0.0.4 (2021-01-22)
+-------------------
+
+- Fixed in documentation.
+
+- Added examples for `query_params` in the doc examples.
+
+- Updated directory name from `mopinion_client` to `mopinion`.
+
+- Implemented About in Docs and Readme.
+
+0.0.3 (2021-01-20)
+-------------------
+
+- Fixed typing in method `get_token`. Return `bytes` instead of `str`.
+
+0.0.2 (2021-01-20)
+-------------------
+
+- Fixed in documentation.
+
+- Removed travis ci. Integrated GitHub Actions.
+
+- Added coverage into GitHub actions.
+
+0.0.1 (2021-01-20)
+-------------------
+
+- Initial project structure.
+
+- Client implementation.
+
+- Test suite.
+
+- Request examples.
```

### Comparing `mopinion-1.0.0/README.rst` & `mopinion-1.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Mopinion API - Python Client
 ==========================================
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
-    :target: https://github.com/mopinion/mopinion-python-api/blob/master/LICENSE
+    :target: https://github.com/Mopinion-com/mopinion-python-api/blob/master/LICENSE
     :alt: License-MIT
 
 .. image:: https://readthedocs.org/projects/mopinion-python-api/badge/?version=latest
     :target: https://mopinion-python-api.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://github.com/mopinion/mopinion-python-api/workflows/Test%20Suite/badge.svg/
+.. image:: https://github.com/Mopinion-com/mopinion-python-api/workflows/Test%20Suite/badge.svg/
     :alt: GitHub Actions
 
 .. image:: https://badge.fury.io/py/mopinion.svg/
     :target: https://badge.fury.io/py/mopinion/
     :alt: Badge PyPi
```

### Comparing `mopinion-1.0.0/mopinion/client.py` & `mopinion-1.0.1/mopinion/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 API Client library for the Mopinion Data API.
 For more information, see: https://developer.mopinion.com/api/
 """
-
+import urllib.parse
 from base64 import b64encode
 from collections.abc import Iterator
 from mopinion import settings
 from mopinion.dataclasses import Credentials
 from mopinion.dataclasses import EndPoint
 from mopinion.dataclasses import RequestArguments
 from mopinion.dataclasses import ResourceUri
@@ -106,17 +106,15 @@
           private_key (str):
           verbosity (str): Defaults to normal.
           version (str): If no version provided, default to latest.
           content_negotiation (str): Defaults to application/json.
           max_retries (int): Defaults to 3.
           backoff_factor (int): Defaults to 1.
         """
-        self.credentials = Credentials(
-            public_key=public_key, private_key=private_key
-        )
+        self.credentials = Credentials(public_key=public_key, private_key=private_key)
         self.session = requests.Session()
         retries = Retry(total=max_retries, backoff_factor=backoff_factor)
         adapter = HTTPAdapter(max_retries=retries)
         self.session.mount(settings.BASE_URL, adapter=adapter)
         self.signature_token = self._get_signature_token(self.credentials)
         self.content_negotiation = content_negotiation
         self.verbosity = verbosity
@@ -369,20 +367,23 @@
 
         if iterator:
             return self._get_iterator(resource_uri.endpoint, **params)
         else:
             return self.request(endpoint=resource_uri.endpoint, **params)
 
     def _get_iterator(self, endpoint: str, **params):
-        next_uri = endpoint
-        # yield messages till next (uri) == False
-        while next_uri:
-            response = self.request(endpoint=next_uri, **params)
+        while True:
+            response = self.request(endpoint=endpoint, **params)
             yield response
-            next_uri = response.json()["_meta"]["next"]
+
+            if not response.json()["_meta"]["has_more"]:
+                break
+
+            next_uri = urllib.parse.urlparse(response.json()["_meta"]["next"])
+            params["query_params"] = dict(urllib.parse.parse_qsl(next_uri.query))
 
     # GET methods
     def get_account(self, **kwargs):
         """
         Get your account.
 
         Args:
```

### Comparing `mopinion-1.0.0/mopinion/dataclasses.py` & `mopinion-1.0.1/mopinion/dataclasses.py`

 * *Files identical despite different names*

### Comparing `mopinion-1.0.0/mopinion.egg-info/PKG-INFO` & `mopinion-1.0.1/mopinion.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,177 @@
 Metadata-Version: 2.1
 Name: mopinion
-Version: 1.0.0
+Version: 1.0.1
 Summary: A client library for the Mopinion Data API
-Home-page: https://github.com/mopinion/mopinion-python-api
+Home-page: https://github.com/Mopinion-com/mopinion-python-api
 Author: Mopinion
 Author-email: 
 License: MIT License
-Description: Mopinion API - Python Client
-        ==========================================
-        
-        .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
-            :target: https://github.com/mopinion/mopinion-python-api/blob/master/LICENSE
-            :alt: License-MIT
-        
-        .. image:: https://readthedocs.org/projects/mopinion-python-api/badge/?version=latest
-            :target: https://mopinion-python-api.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://github.com/mopinion/mopinion-python-api/workflows/Test%20Suite/badge.svg/
-            :alt: GitHub Actions
-        
-        .. image:: https://badge.fury.io/py/mopinion.svg/
-            :target: https://badge.fury.io/py/mopinion/
-            :alt: Badge PyPi
-        
-        
-        A client library for the `Mopinion Data API <https://developer.mopinion.com/api/>`_.
-        
-        Our Mopinion Client provides functionality for authentication, authorization and requesting resources.
-        It comes with an easy, beautiful, and elegant way of interacting with our API.
-        
-        `Read the docs <https://mopinion-python-api.readthedocs.io/en/latest/>`_ for further information.
-        
-        Installation
-        -------------
-        
-        Install using ``pip``::
-        
-            pip install mopinion
-        
-        
-        Example
-        --------
-        
-        .. code:: python
-        
-            >>> from mopinion import MopinionClient
-            >>> client = MopinionClient(public_key=PUBLIC_KEY, private_key=PRIVATE_KEY)
-            >>> assert client.is_available()
-            >>> response = client.resource("account")
-            >>> response = client.resource("deployments")
-            >>>
-            >>> response = client.get_account()
-            >>>
-            >>> response = client.get_deployments()
-            >>> response = client.get_deployments("abc")
-            >>>
-            >>> response = client.get_reports(report_id=123)
-            >>> response = client.get_reports_fields(report_id=123)
-            >>> response = client.get_reports_feedback(report_id=123)
-            >>>
-            >>> response = client.get_datasets(dataset_id=123)
-            >>> response = client.get_datasets_feedback(dataset_id=123)
-            >>> response = client.get_datasets_fields(dataset_id=123)
-            >>>
-            >>> client.close()
-            >>>
-            >>> with MopinionClient(public_key=YOUR_PUBLIC_KEY, private_key=YOUR_PRIVATE_KEY) as client:
-            ...     response = client.get_account()
-            ...     assert response.json()["_meta"]["code"] == 200
-        
-        Documentation
-        ---------------
-        
-        You can find here at `Read the docs <https://mopinion-python-api.readthedocs.io/en/latest/>`_ the complete documentation.
-        
-        
-        About Mopinion
-        ---------------
-        
-        `Mopinion <https://mopinion.com/>`_ is a leading all-in-one user feedback platform that helps digital enterprises listen, understand,
-        and act across all digital touchpoints (web, mobile, and email). Join some of the most forward-thinking
-        digital teams from companies such as T-mobile, eBay, TSB Bank, Walmart, Hotels.com, Decathlon, Ahold,
-        Mediacorp Ltd, and many more.
-        
-        Please visit the website for more information about the product: https://mopinion.com
-        
-        
-        Changelog
-        ========================================================
-        
-        
-        1.0.0 (2022-03-04)
-        -------------------
-        
-        - Released stable version.
-        
-        
-        0.0.7 (2022-02-23)
-        -------------------
-        
-        - Fixes in documentation.
-        
-        - Implement `__enter__()` and `__exit__()` methods.
-        
-        - Added methods: `get_account`, `get_deployments`,
-          `get_datasets`, `get_datasets_fields`,
-          `get_datasets_feedback`, `get_reports`,
-          `get_reports_fields`, `get_reports_feedback`.
-        
-        - Increased compatibility from Python 3.6 to 3.10.
-        
-        
-        0.0.6 (2021-02-11)
-        -------------------
-        
-        - Fixes in documentation.
-        
-        - Added pre-commit configuration to project.
-        
-        - Added new endpoint for `/deployments/<str_id>`.
-        
-        
-        0.0.5 (2021-01-22)
-        -------------------
-        
-        - Several fixes in documentation.
-        
-        
-        0.0.4 (2021-01-22)
-        -------------------
-        
-        - Fixed in documentation.
-        
-        - Added examples for `query_params` in the doc examples.
-        
-        - Updated directory name from `mopinion_client` to `mopinion`.
-        
-        - Implemented About in Docs and Readme.
-        
-        0.0.3 (2021-01-20)
-        -------------------
-        
-        - Fixed typing in method `get_token`. Return `bytes` instead of `str`.
-        
-        0.0.2 (2021-01-20)
-        -------------------
-        
-        - Fixed in documentation.
-        
-        - Removed travis ci. Integrated GitHub Actions.
-        
-        - Added coverage into GitHub actions.
-        
-        0.0.1 (2021-01-20)
-        -------------------
-        
-        - Initial project structure.
-        
-        - Client implementation.
-        
-        - Test suite.
-        
-        - Request examples.
-        
 Keywords: mopinion
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Provides-Extra: test
+License-File: LICENSE
+
+Mopinion API - Python Client
+==========================================
+
+.. image:: https://img.shields.io/badge/License-MIT-yellow.svg
+    :target: https://github.com/Mopinion-com/mopinion-python-api/blob/master/LICENSE
+    :alt: License-MIT
+
+.. image:: https://readthedocs.org/projects/mopinion-python-api/badge/?version=latest
+    :target: https://mopinion-python-api.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://github.com/Mopinion-com/mopinion-python-api/workflows/Test%20Suite/badge.svg/
+    :alt: GitHub Actions
+
+.. image:: https://badge.fury.io/py/mopinion.svg/
+    :target: https://badge.fury.io/py/mopinion/
+    :alt: Badge PyPi
+
+
+A client library for the `Mopinion Data API <https://developer.mopinion.com/api/>`_.
+
+Our Mopinion Client provides functionality for authentication, authorization and requesting resources.
+It comes with an easy, beautiful, and elegant way of interacting with our API.
+
+`Read the docs <https://mopinion-python-api.readthedocs.io/en/latest/>`_ for further information.
+
+Installation
+-------------
+
+Install using ``pip``::
+
+    pip install mopinion
+
+
+Example
+--------
+
+.. code:: python
+
+    >>> from mopinion import MopinionClient
+    >>> client = MopinionClient(public_key=PUBLIC_KEY, private_key=PRIVATE_KEY)
+    >>> assert client.is_available()
+    >>> response = client.resource("account")
+    >>> response = client.resource("deployments")
+    >>>
+    >>> response = client.get_account()
+    >>>
+    >>> response = client.get_deployments()
+    >>> response = client.get_deployments("abc")
+    >>>
+    >>> response = client.get_reports(report_id=123)
+    >>> response = client.get_reports_fields(report_id=123)
+    >>> response = client.get_reports_feedback(report_id=123)
+    >>>
+    >>> response = client.get_datasets(dataset_id=123)
+    >>> response = client.get_datasets_feedback(dataset_id=123)
+    >>> response = client.get_datasets_fields(dataset_id=123)
+    >>>
+    >>> client.close()
+    >>>
+    >>> with MopinionClient(public_key=YOUR_PUBLIC_KEY, private_key=YOUR_PRIVATE_KEY) as client:
+    ...     response = client.get_account()
+    ...     assert response.json()["_meta"]["code"] == 200
+
+Documentation
+---------------
+
+You can find here at `Read the docs <https://mopinion-python-api.readthedocs.io/en/latest/>`_ the complete documentation.
+
+
+About Mopinion
+---------------
+
+`Mopinion <https://mopinion.com/>`_ is a leading all-in-one user feedback platform that helps digital enterprises listen, understand,
+and act across all digital touchpoints (web, mobile, and email). Join some of the most forward-thinking
+digital teams from companies such as T-mobile, eBay, TSB Bank, Walmart, Hotels.com, Decathlon, Ahold,
+Mediacorp Ltd, and many more.
+
+Please visit the website for more information about the product: https://mopinion.com
+
+
+Changelog
+========================================================
+
+
+1.0.1 (2023-07-11)
+-------------------
+- Fix issue where query parameters are not properly set for iterable responses.
+
+1.0.0 (2022-03-04)
+-------------------
+
+- Released stable version.
+
+
+0.0.7 (2022-02-23)
+-------------------
+
+- Fixes in documentation.
+
+- Implement `__enter__()` and `__exit__()` methods.
+
+- Added methods: `get_account`, `get_deployments`,
+  `get_datasets`, `get_datasets_fields`,
+  `get_datasets_feedback`, `get_reports`,
+  `get_reports_fields`, `get_reports_feedback`.
+
+- Increased compatibility from Python 3.6 to 3.10.
+
+
+0.0.6 (2021-02-11)
+-------------------
+
+- Fixes in documentation.
+
+- Added pre-commit configuration to project.
+
+- Added new endpoint for `/deployments/<str_id>`.
+
+
+0.0.5 (2021-01-22)
+-------------------
+
+- Several fixes in documentation.
+
+
+0.0.4 (2021-01-22)
+-------------------
+
+- Fixed in documentation.
+
+- Added examples for `query_params` in the doc examples.
+
+- Updated directory name from `mopinion_client` to `mopinion`.
+
+- Implemented About in Docs and Readme.
+
+0.0.3 (2021-01-20)
+-------------------
+
+- Fixed typing in method `get_token`. Return `bytes` instead of `str`.
+
+0.0.2 (2021-01-20)
+-------------------
+
+- Fixed in documentation.
+
+- Removed travis ci. Integrated GitHub Actions.
+
+- Added coverage into GitHub actions.
+
+0.0.1 (2021-01-20)
+-------------------
+
+- Initial project structure.
+
+- Client implementation.
+
+- Test suite.
+
+- Request examples.
```

### Comparing `mopinion-1.0.0/setup.py` & `mopinion-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 import os
 
 
-version = "1.0.0"
+version = "1.0.1"
 
 long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read()])
 
 install_requires = [
     "requests",
     "dataclasses; python_version < '3.7.0'",
 ]
@@ -35,15 +35,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords=["mopinion"],
     author="Mopinion",
     author_email="",
-    url="https://github.com/mopinion/mopinion-python-api",
+    url="https://github.com/Mopinion-com/mopinion-python-api",
     license="MIT License",
     packages=["mopinion"],
     include_package_data=True,
     zip_safe=False,
     install_requires=install_requires,
     tests_require=tests_require,
     python_requires=">=3.6",
```

