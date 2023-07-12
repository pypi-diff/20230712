# Comparing `tmp/python-pbxonline-0.2.0.tar.gz` & `tmp/python-pbxonline-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pbxonline-0.2.0.tar", last modified: Wed Jul 12 08:35:54 2023, max compression
+gzip compressed data, was "python-pbxonline-0.2.1.tar", last modified: Wed Jul 12 11:23:26 2023, max compression
```

## Comparing `python-pbxonline-0.2.0.tar` & `python-pbxonline-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.685196 python-pbxonline-0.2.0/
--rw-rw-rw-   0        0        0    35821 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      798 2023-07-12 08:35:54.686195 python-pbxonline-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 11:33:48.000000 python-pbxonline-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.602851 python-pbxonline-0.2.0/pbxonline/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/__init__.py
--rw-rw-rw-   0        0        0     8155 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/api.py
--rw-rw-rw-   0        0        0     4506 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/auth_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.604861 python-pbxonline-0.2.0/pbxonline/cache/
--rw-rw-rw-   0        0        0        0 2023-04-24 08:42:27.000000 python-pbxonline-0.2.0/pbxonline/cache/__init__.py
--rw-rw-rw-   0        0        0     3352 2023-07-07 08:51:00.000000 python-pbxonline-0.2.0/pbxonline/cache_handler.py
--rw-rw-rw-   0        0        0      173 2023-07-07 08:50:19.000000 python-pbxonline-0.2.0/pbxonline/config.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.610852 python-pbxonline-0.2.0/pbxonline/constants/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/constants/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-24 08:35:02.000000 python-pbxonline-0.2.0/pbxonline/constants/constants.py
--rw-rw-rw-   0        0        0      105 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/constants/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.620714 python-pbxonline-0.2.0/pbxonline/endpoints/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/endpoints/__init__.py
--rw-rw-rw-   0        0        0     1455 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/endpoints/action.py
--rw-rw-rw-   0        0        0      141 2023-04-24 12:47:39.000000 python-pbxonline-0.2.0/pbxonline/endpoints/base.py
--rw-rw-rw-   0        0        0     1023 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/endpoints/pbx.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.628716 python-pbxonline-0.2.0/pbxonline/models/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.0/pbxonline/models/__init__.py
--rw-rw-rw-   0        0        0     1346 2023-04-27 06:19:09.000000 python-pbxonline-0.2.0/pbxonline/models/base.py
--rw-rw-rw-   0        0        0      165 2023-07-07 08:33:02.000000 python-pbxonline-0.2.0/pbxonline/models/errors.py
--rw-rw-rw-   0        0        0     2484 2023-07-10 14:21:16.000000 python-pbxonline-0.2.0/pbxonline/models/utils.py
--rw-rw-rw-   0        0        0      185 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/pbxonline/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.677198 python-pbxonline-0.2.0/python_pbxonline.egg-info/
--rw-rw-rw-   0        0        0      798 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 08:35:54.000000 python-pbxonline-0.2.0/python_pbxonline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-12 08:35:54.693193 python-pbxonline-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1269 2023-07-12 08:35:47.000000 python-pbxonline-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:54.684196 python-pbxonline-0.2.0/tests/
--rw-rw-rw-   0        0        0      614 2023-07-12 08:11:45.000000 python-pbxonline-0.2.0/tests/test_action.py
--rw-rw-rw-   0        0        0      266 2023-07-07 08:50:49.000000 python-pbxonline-0.2.0/tests/test_auth.py
--rw-rw-rw-   0        0        0      410 2023-07-07 12:53:43.000000 python-pbxonline-0.2.0/tests/test_pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:23:26.758660 python-pbxonline-0.2.1/
+-rw-rw-rw-   0        0        0    35821 2023-04-21 13:50:30.000000 python-pbxonline-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-04-21 13:50:30.000000 python-pbxonline-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      798 2023-07-12 11:23:26.759638 python-pbxonline-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:33:48.000000 python-pbxonline-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 11:23:26.700482 python-pbxonline-0.2.1/pbxonline/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.1/pbxonline/__init__.py
+-rw-rw-rw-   0        0        0     8903 2023-07-12 11:21:55.000000 python-pbxonline-0.2.1/pbxonline/api.py
+-rw-rw-rw-   0        0        0     4506 2023-07-12 08:35:47.000000 python-pbxonline-0.2.1/pbxonline/auth_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:23:26.702241 python-pbxonline-0.2.1/pbxonline/cache/
+-rw-rw-rw-   0        0        0        0 2023-04-24 08:42:27.000000 python-pbxonline-0.2.1/pbxonline/cache/__init__.py
+-rw-rw-rw-   0        0        0     3352 2023-07-07 08:51:00.000000 python-pbxonline-0.2.1/pbxonline/cache_handler.py
+-rw-rw-rw-   0        0        0      173 2023-07-07 08:50:19.000000 python-pbxonline-0.2.1/pbxonline/config.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:23:26.705291 python-pbxonline-0.2.1/pbxonline/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.1/pbxonline/constants/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 08:35:02.000000 python-pbxonline-0.2.1/pbxonline/constants/constants.py
+-rw-rw-rw-   0        0        0      105 2023-04-21 13:50:30.000000 python-pbxonline-0.2.1/pbxonline/constants/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:23:26.711248 python-pbxonline-0.2.1/pbxonline/endpoints/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.1/pbxonline/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     1455 2023-07-12 08:35:47.000000 python-pbxonline-0.2.1/pbxonline/endpoints/action.py
+-rw-rw-rw-   0        0        0      141 2023-04-24 12:47:39.000000 python-pbxonline-0.2.1/pbxonline/endpoints/base.py
+-rw-rw-rw-   0        0        0     1023 2023-07-12 08:35:47.000000 python-pbxonline-0.2.1/pbxonline/endpoints/pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:23:26.712280 python-pbxonline-0.2.1/pbxonline/models/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.2.1/pbxonline/models/__init__.py
+-rw-rw-rw-   0        0        0     1346 2023-04-27 06:19:09.000000 python-pbxonline-0.2.1/pbxonline/models/base.py
+-rw-rw-rw-   0        0        0      165 2023-07-07 08:33:02.000000 python-pbxonline-0.2.1/pbxonline/models/errors.py
+-rw-rw-rw-   0        0        0     2484 2023-07-10 14:21:16.000000 python-pbxonline-0.2.1/pbxonline/models/utils.py
+-rw-rw-rw-   0        0        0      185 2023-07-12 08:35:47.000000 python-pbxonline-0.2.1/pbxonline/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:23:26.742715 python-pbxonline-0.2.1/python_pbxonline.egg-info/
+-rw-rw-rw-   0        0        0      798 2023-07-12 11:23:26.000000 python-pbxonline-0.2.1/python_pbxonline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      833 2023-07-12 11:23:26.000000 python-pbxonline-0.2.1/python_pbxonline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:23:26.000000 python-pbxonline-0.2.1/python_pbxonline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-12 11:23:26.000000 python-pbxonline-0.2.1/python_pbxonline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 11:23:26.000000 python-pbxonline-0.2.1/python_pbxonline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-12 11:23:26.765121 python-pbxonline-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2023-07-12 11:23:18.000000 python-pbxonline-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:23:26.756161 python-pbxonline-0.2.1/tests/
+-rw-rw-rw-   0        0        0      614 2023-07-12 11:17:01.000000 python-pbxonline-0.2.1/tests/test_action.py
+-rw-rw-rw-   0        0        0      266 2023-07-07 08:50:49.000000 python-pbxonline-0.2.1/tests/test_auth.py
+-rw-rw-rw-   0        0        0      331 2023-07-12 11:20:21.000000 python-pbxonline-0.2.1/tests/test_endcall.py
+-rw-rw-rw-   0        0        0      410 2023-07-07 12:53:43.000000 python-pbxonline-0.2.1/tests/test_pbx.py
+-rw-rw-rw-   0        0        0      518 2023-07-12 11:15:45.000000 python-pbxonline-0.2.1/tests/test_startcall.py
```

### Comparing `python-pbxonline-0.2.0/LICENSE.txt` & `python-pbxonline-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.2.0/PKG-INFO` & `python-pbxonline-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-pbxonline
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wrapper for PBX Online API
 Home-page: https://github.com/alexanderlhsglobal/python-pbxonline
-Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.2.0.tar.gz
+Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.2.1.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@hotmail.com
 License: GPL-3.0-or-later
 Keywords: pbxonline
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python-pbxonline-0.2.0/pbxonline/api.py` & `python-pbxonline-0.2.1/pbxonline/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,17 +64,33 @@
 
     def _parse_response_content(self, response: requests.Response) -> dict | str:
         """ Parses the response content to a dict if the response is JSON, otherwise returns the response content as a string. """
         
         response_type = response.headers.get('Content-Type', '')
         response_content_decoded = response.content.decode('utf-8')
         
-        # Remove the first part of the response if it's not JSON
-        # Sometimes the API returns a response that starts with html. To get a valid JSON response, we need to remove the html part.
-        resp_content = response_content_decoded[response_content_decoded.find('{'):]
+        if 'text/json' in response_type:
+            
+            # Remove the first part of the response if it's not JSON
+            # Sometimes the API returns a response that starts with html. To get a valid JSON response, we need to remove the html part.
+    
+            # Find the index of the first square bracket or curly bracket
+            # If the square bracket is before the curly bracket, use that index. Otherwise, use the curly bracket index.
+            square_brackets_index = response_content_decoded.find('[')
+            curly_brackets_index = response_content_decoded.find('{')
+            if(square_brackets_index < curly_brackets_index and square_brackets_index != -1):
+                index = square_brackets_index
+            elif(curly_brackets_index != -1):
+                index = curly_brackets_index
+            else:
+                index = 0
+            
+            resp_content = response_content_decoded[index:]
+        else:
+            resp_content = response_content_decoded
         
         # If the response is JSON, parse it to a dict
         resp_content = json.loads(resp_content) if 'text/json' in response_type else resp_content
         
         return resp_content
 
     def _do_request(self, method: Literal['GET', 'POST', 'PUT'], url: str, data: Optional[dict] = None, headers: Optional[dict] = None, prepend_base_to_url: Optional[bool] = True) -> requests.Response:
```

### Comparing `python-pbxonline-0.2.0/pbxonline/auth_handler.py` & `python-pbxonline-0.2.1/pbxonline/auth_handler.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.2.0/pbxonline/cache_handler.py` & `python-pbxonline-0.2.1/pbxonline/cache_handler.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.2.0/pbxonline/endpoints/action.py` & `python-pbxonline-0.2.1/pbxonline/endpoints/action.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.2.0/pbxonline/endpoints/pbx.py` & `python-pbxonline-0.2.1/pbxonline/endpoints/pbx.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.2.0/pbxonline/models/base.py` & `python-pbxonline-0.2.1/pbxonline/models/base.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.2.0/pbxonline/models/utils.py` & `python-pbxonline-0.2.1/pbxonline/models/utils.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.2.0/python_pbxonline.egg-info/PKG-INFO` & `python-pbxonline-0.2.1/python_pbxonline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-pbxonline
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wrapper for PBX Online API
 Home-page: https://github.com/alexanderlhsglobal/python-pbxonline
-Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.2.0.tar.gz
+Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.2.1.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@hotmail.com
 License: GPL-3.0-or-later
 Keywords: pbxonline
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python-pbxonline-0.2.0/python_pbxonline.egg-info/SOURCES.txt` & `python-pbxonline-0.2.1/python_pbxonline.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,8 +24,10 @@
 python_pbxonline.egg-info/PKG-INFO
 python_pbxonline.egg-info/SOURCES.txt
 python_pbxonline.egg-info/dependency_links.txt
 python_pbxonline.egg-info/requires.txt
 python_pbxonline.egg-info/top_level.txt
 tests/test_action.py
 tests/test_auth.py
-tests/test_pbx.py
+tests/test_endcall.py
+tests/test_pbx.py
+tests/test_startcall.py
```

### Comparing `python-pbxonline-0.2.0/setup.py` & `python-pbxonline-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'python-pbxonline',         
   packages=['pbxonline', 'pbxonline.models', 'pbxonline.constants', 'pbxonline.endpoints', 'pbxonline.cache'],
-  version = '0.2.0',
+  version = '0.2.1',
   license='GPL-3.0-or-later',
   description = 'Wrapper for PBX Online API',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@hotmail.com',
   url = 'https://github.com/alexanderlhsglobal/python-pbxonline',
-  download_url = 'https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.2.0.tar.gz',
+  download_url = 'https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.2.1.tar.gz',
   keywords = ['pbxonline'],
   install_requires=[
           'requests',
           'requests_oauthlib'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

### Comparing `python-pbxonline-0.2.0/tests/test_action.py` & `python-pbxonline-0.2.1/tests/test_action.py`

 * *Files identical despite different names*

