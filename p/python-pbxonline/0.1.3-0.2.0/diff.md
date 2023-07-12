# Comparing `tmp/python-pbxonline-0.1.3.tar.gz` & `tmp/python-pbxonline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pbxonline-0.1.3.tar", last modified: Mon Jul 10 14:23:03 2023, max compression
+gzip compressed data, was "python-pbxonline-0.2.0.tar", last modified: Wed Jul 12 08:35:54 2023, max compression
```

## Comparing `python-pbxonline-0.1.3.tar` & `python-pbxonline-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 14:23:03.486323 python-pbxonline-0.1.3/
--rw-rw-rw-   0        0        0    35821 2023-04-21 13:50:30.000000 python-pbxonline-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-04-21 13:50:30.000000 python-pbxonline-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      798 2023-07-10 14:23:03.486323 python-pbxonline-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 11:33:48.000000 python-pbxonline-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 14:23:03.426715 python-pbxonline-0.1.3/pbxonline/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.3/pbxonline/__init__.py
--rw-rw-rw-   0        0        0     8283 2023-07-10 14:22:55.000000 python-pbxonline-0.1.3/pbxonline/api.py
--rw-rw-rw-   0        0        0     3451 2023-07-07 09:09:45.000000 python-pbxonline-0.1.3/pbxonline/auth_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:23:03.426715 python-pbxonline-0.1.3/pbxonline/cache/
--rw-rw-rw-   0        0        0        0 2023-04-24 08:42:27.000000 python-pbxonline-0.1.3/pbxonline/cache/__init__.py
--rw-rw-rw-   0        0        0     3352 2023-07-07 08:51:00.000000 python-pbxonline-0.1.3/pbxonline/cache_handler.py
--rw-rw-rw-   0        0        0      173 2023-07-07 08:50:19.000000 python-pbxonline-0.1.3/pbxonline/config.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:23:03.433232 python-pbxonline-0.1.3/pbxonline/constants/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.3/pbxonline/constants/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-24 08:35:02.000000 python-pbxonline-0.1.3/pbxonline/constants/constants.py
--rw-rw-rw-   0        0        0      105 2023-04-21 13:50:30.000000 python-pbxonline-0.1.3/pbxonline/constants/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:23:03.439850 python-pbxonline-0.1.3/pbxonline/endpoints/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.3/pbxonline/endpoints/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-07-10 14:22:55.000000 python-pbxonline-0.1.3/pbxonline/endpoints/action.py
--rw-rw-rw-   0        0        0      141 2023-04-24 12:47:39.000000 python-pbxonline-0.1.3/pbxonline/endpoints/base.py
--rw-rw-rw-   0        0        0      658 2023-07-07 12:11:14.000000 python-pbxonline-0.1.3/pbxonline/endpoints/pbx.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:23:03.444829 python-pbxonline-0.1.3/pbxonline/models/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.3/pbxonline/models/__init__.py
--rw-rw-rw-   0        0        0     1346 2023-04-27 06:19:09.000000 python-pbxonline-0.1.3/pbxonline/models/base.py
--rw-rw-rw-   0        0        0      165 2023-07-07 08:33:02.000000 python-pbxonline-0.1.3/pbxonline/models/errors.py
--rw-rw-rw-   0        0        0     2484 2023-07-10 14:21:16.000000 python-pbxonline-0.1.3/pbxonline/models/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:23:03.479248 python-pbxonline-0.1.3/python_pbxonline.egg-info/
--rw-rw-rw-   0        0        0      798 2023-07-10 14:23:03.000000 python-pbxonline-0.1.3/python_pbxonline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2023-07-10 14:23:03.000000 python-pbxonline-0.1.3/python_pbxonline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 14:23:03.000000 python-pbxonline-0.1.3/python_pbxonline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-10 14:23:03.000000 python-pbxonline-0.1.3/python_pbxonline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 14:23:03.000000 python-pbxonline-0.1.3/python_pbxonline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-10 14:23:03.496032 python-pbxonline-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1269 2023-07-10 14:22:55.000000 python-pbxonline-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:23:03.485323 python-pbxonline-0.1.3/tests/
--rw-rw-rw-   0        0        0      366 2023-07-10 14:18:23.000000 python-pbxonline-0.1.3/tests/test_action.py
--rw-rw-rw-   0        0        0      266 2023-07-07 08:50:49.000000 python-pbxonline-0.1.3/tests/test_auth.py
--rw-rw-rw-   0        0        0      410 2023-07-07 12:53:43.000000 python-pbxonline-0.1.3/tests/test_pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.685196 python-pbxonline-0.2.0/
+-rw-rw-rw-   0        0        0    35821 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      798 2023-07-12 08:35:54.686195 python-pbxonline-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:33:48.000000 python-pbxonline-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.602851 python-pbxonline-0.2.0/pbxonline/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/__init__.py
+-rw-rw-rw-   0        0        0     8155 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/api.py
+-rw-rw-rw-   0        0        0     4506 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/auth_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.604861 python-pbxonline-0.2.0/pbxonline/cache/
+-rw-rw-rw-   0        0        0        0 2023-04-24 08:42:27.000000 python-pbxonline-0.2.0/pbxonline/cache/__init__.py
+-rw-rw-rw-   0        0        0     3352 2023-07-07 08:51:00.000000 python-pbxonline-0.2.0/pbxonline/cache_handler.py
+-rw-rw-rw-   0        0        0      173 2023-07-07 08:50:19.000000 python-pbxonline-0.2.0/pbxonline/config.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.610852 python-pbxonline-0.2.0/pbxonline/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/constants/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 08:35:02.000000 python-pbxonline-0.2.0/pbxonline/constants/constants.py
+-rw-rw-rw-   0        0        0      105 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/constants/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.620714 python-pbxonline-0.2.0/pbxonline/endpoints/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     1455 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/endpoints/action.py
+-rw-rw-rw-   0        0        0      141 2023-04-24 12:47:39.000000 python-pbxonline-0.2.0/pbxonline/endpoints/base.py
+-rw-rw-rw-   0        0        0     1023 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/endpoints/pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.628716 python-pbxonline-0.2.0/pbxonline/models/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/models/__init__.py
+-rw-rw-rw-   0        0        0     1346 2023-04-27 06:19:09.000000 python-pbxonline-0.2.0/pbxonline/models/base.py
+-rw-rw-rw-   0        0        0      165 2023-07-07 08:33:02.000000 python-pbxonline-0.2.0/pbxonline/models/errors.py
+-rw-rw-rw-   0        0        0     2484 2023-07-10 14:21:16.000000 python-pbxonline-0.2.0/pbxonline/models/utils.py
+-rw-rw-rw-   0        0        0      185 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.677198 python-pbxonline-0.2.0/python_pbxonline.egg-info/
+-rw-rw-rw-   0        0        0      798 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-12 08:35:54.693193 python-pbxonline-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.684196 python-pbxonline-0.2.0/tests/
+-rw-rw-rw-   0        0        0      614 2023-07-12 08:11:45.000000 python-pbxonline-0.2.0/tests/test_action.py
+-rw-rw-rw-   0        0        0      266 2023-07-07 08:50:49.000000 python-pbxonline-0.2.0/tests/test_auth.py
+-rw-rw-rw-   0        0        0      410 2023-07-07 12:53:43.000000 python-pbxonline-0.2.0/tests/test_pbx.py
```

### Comparing `python-pbxonline-0.1.3/LICENSE.txt` & `python-pbxonline-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.3/PKG-INFO` & `python-pbxonline-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-pbxonline
-Version: 0.1.3
+Version: 0.2.0
 Summary: Wrapper for PBX Online API
 Home-page: https://github.com/alexanderlhsglobal/python-pbxonline
-Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.3.tar.gz
+Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.2.0.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@hotmail.com
 License: GPL-3.0-or-later
 Keywords: pbxonline
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python-pbxonline-0.1.3/pbxonline/api.py` & `python-pbxonline-0.2.0/pbxonline/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import json
 from typing import Tuple, Optional, Literal
+import re
 
 from . import config
 from .auth_handler import AuthHandler
 from .cache_handler import CacheHandler
 
 from pbxonline.endpoints.pbx import PBXEndpoint
 from pbxonline.endpoints.action import ActionEndpoint
@@ -57,14 +58,29 @@
         :rtype: dict
         """
         
         tmp_headers = self._headers.copy()
         tmp_headers.update(headers)
         return tmp_headers
 
+    def _parse_response_content(self, response: requests.Response) -> dict | str:
+        """ Parses the response content to a dict if the response is JSON, otherwise returns the response content as a string. """
+        
+        response_type = response.headers.get('Content-Type', '')
+        response_content_decoded = response.content.decode('utf-8')
+        
+        # Remove the first part of the response if it's not JSON
+        # Sometimes the API returns a response that starts with html. To get a valid JSON response, we need to remove the html part.
+        resp_content = response_content_decoded[response_content_decoded.find('{'):]
+        
+        # If the response is JSON, parse it to a dict
+        resp_content = json.loads(resp_content) if 'text/json' in response_type else resp_content
+        
+        return resp_content
+
     def _do_request(self, method: Literal['GET', 'POST', 'PUT'], url: str, data: Optional[dict] = None, headers: Optional[dict] = None, prepend_base_to_url: Optional[bool] = True) -> requests.Response:
         """ Makes a request to the given url, with the given method and data; updates headers with new values if given.
         By default, the BASE_URL is prepended to the URL. If the arg "prepend_base_to_url" is set to False, it will not be prepended.
         
         :param method: the HTTP method to use for the request.
         :type method: Literal['GET', 'POST', 'PUT']
         :param url: the URL to make the request to.
@@ -115,41 +131,25 @@
         """
         
         # Check the headers for appropriate tokens before we make a request
         self._check_header_tokens()
 
         # Make the request
         response = self._do_request(method, url, data, headers, **kwargs)
-        response_type = response.headers.get('Content-Type', '')
-        resp_content = response.json() if 'text/json' in response_type else response.content
+        resp_content = self._parse_response_content(response)
         
         # Unauthorized, token is not valid anymore
-        if response.status_code == 401: 
-            refresh_token = self._auth_handler.get_token_from_cache('refresh_token')
+        if response.status_code == 401:
             
-            # If we have a refresh token, get a new access token with it
-            if refresh_token:
-                auth_tokens = self._auth_handler._get_tokens_from_refresh_token(refresh_token)
-                
-                if not auth_tokens:
-                    # Delete cache and get new tokens
-                    # This will force new tokens without the cached refresh token
-                    self._cache_handler.delete(self._api_id)
-                    auth_tokens = self._auth_handler.get_tokens()
-            else:
-                # No refresh token, get new tokens with username and password
-                auth_tokens = self._auth_handler.get_tokens()
-
-            # Set the new token in the headers
-            self._set_token_header(auth_tokens.get('token'))
+            # Force new tokens
+            self._auth_handler.refresh_tokens()
             
             # Resend request after forcing new tokens
             response = self._do_request(method, url, data, headers, **kwargs)
-            response_type = response.headers.get('Content-Type', '')
-            resp_content = response.json() if 'text/json' in response_type else response.content
+            resp_content = self._parse_response_content(response)
             
         return response.status_code, response.headers, resp_content
     
     def get(self, url: str, data: Optional[dict] = None, headers: Optional[dict] = None, **kwargs: dict) -> Tuple[int, dict, dict]:
         """ Makes a GET request to the given URL, with the given data and headers. """
         status, headers, response = self._request('GET', url, data, headers, **kwargs)
         return status, headers, response
```

### Comparing `python-pbxonline-0.1.3/pbxonline/cache_handler.py` & `python-pbxonline-0.2.0/pbxonline/cache_handler.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.3/pbxonline/endpoints/pbx.py` & `python-pbxonline-0.2.0/pbxonline/endpoints/pbx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from typing import Optional
 
 from pbxonline.models.base import ObjectListModel, BaseModel
 from .base import APIEndpoint
 from pbxonline.models.utils import construct_object_from_data, construct_error_from_data
+from pbxonline.utils import request_not_succesful
 
 class PBXEndpoint(APIEndpoint):
     
     def __init__(self, api: object) -> None:
         endpoint = 'pbx'
         super().__init__(api, endpoint)
         
     def get_sip_accounts(self) -> ObjectListModel:
         
         status, headers, resp_json = self.api.get( f'{self.endpoint}/sipaccount')
-        if status > 299: return construct_error_from_data(resp_json)
+        if request_not_succesful(status): return construct_error_from_data(resp_json)
+
+        return construct_object_from_data(resp_json['results'])
+    
+    def get_did_numbers(self) -> ObjectListModel:
+        
+        status, headers, resp_json = self.api.get( f'{self.endpoint}/did')
+        if request_not_succesful(status): return construct_error_from_data(resp_json)
 
         return construct_object_from_data(resp_json['results'])
```

### Comparing `python-pbxonline-0.1.3/pbxonline/models/base.py` & `python-pbxonline-0.2.0/pbxonline/models/base.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.3/pbxonline/models/utils.py` & `python-pbxonline-0.2.0/pbxonline/models/utils.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.3/python_pbxonline.egg-info/PKG-INFO` & `python-pbxonline-0.2.0/python_pbxonline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-pbxonline
-Version: 0.1.3
+Version: 0.2.0
 Summary: Wrapper for PBX Online API
 Home-page: https://github.com/alexanderlhsglobal/python-pbxonline
-Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.3.tar.gz
+Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.2.0.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@hotmail.com
 License: GPL-3.0-or-later
 Keywords: pbxonline
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python-pbxonline-0.1.3/python_pbxonline.egg-info/SOURCES.txt` & `python-pbxonline-0.2.0/python_pbxonline.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 pbxonline/__init__.py
 pbxonline/api.py
 pbxonline/auth_handler.py
 pbxonline/cache_handler.py
 pbxonline/config.py
+pbxonline/utils.py
 pbxonline/cache/__init__.py
 pbxonline/constants/__init__.py
 pbxonline/constants/constants.py
 pbxonline/constants/errors.py
 pbxonline/endpoints/__init__.py
 pbxonline/endpoints/action.py
 pbxonline/endpoints/base.py
```

### Comparing `python-pbxonline-0.1.3/setup.py` & `python-pbxonline-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'python-pbxonline',         
   packages=['pbxonline', 'pbxonline.models', 'pbxonline.constants', 'pbxonline.endpoints', 'pbxonline.cache'],
-  version = '0.1.3',
+  version = '0.2.0',
   license='GPL-3.0-or-later',
   description = 'Wrapper for PBX Online API',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@hotmail.com',
   url = 'https://github.com/alexanderlhsglobal/python-pbxonline',
-  download_url = 'https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.3.tar.gz',
+  download_url = 'https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.2.0.tar.gz',
   keywords = ['pbxonline'],
   install_requires=[
           'requests',
           'requests_oauthlib'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

