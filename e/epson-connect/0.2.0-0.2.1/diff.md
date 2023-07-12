# Comparing `tmp/epson_connect-0.2.0.tar.gz` & `tmp/epson_connect-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epson_connect-0.2.0.tar", max compression
+gzip compressed data, was "epson_connect-0.2.1.tar", max compression
```

## Comparing `epson_connect-0.2.0.tar` & `epson_connect-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1119 2023-07-09 20:45:17.736792 epson_connect-0.2.0/LICENSE
--rw-r--r--   0        0        0      704 2023-07-10 05:14:45.827382 epson_connect-0.2.0/README.md
--rw-r--r--   0        0        0     1340 2023-07-10 17:07:54.467052 epson_connect-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       41 2023-07-10 04:04:57.289077 epson_connect-0.2.0/src/epson_connect/__init__.py
--rw-r--r--   0        0        0     3560 2023-07-10 04:07:20.223607 epson_connect-0.2.0/src/epson_connect/authenticate.py
--rw-r--r--   0        0        0     1154 2023-07-09 05:46:28.548782 epson_connect-0.2.0/src/epson_connect/client.py
--rw-r--r--   0        0        0     4349 2023-07-10 04:46:00.519043 epson_connect-0.2.0/src/epson_connect/printer.py
--rw-r--r--   0        0        0     4924 2023-07-10 04:09:53.041881 epson_connect-0.2.0/src/epson_connect/printer_settings.py
--rw-r--r--   0        0        0     2435 2023-07-10 04:19:47.452482 epson_connect-0.2.0/src/epson_connect/scanner.py
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 epson_connect-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-07-09 20:45:17.736792 epson_connect-0.2.1/LICENSE
+-rw-r--r--   0        0        0      763 2023-07-12 19:25:52.875427 epson_connect-0.2.1/README.md
+-rw-r--r--   0        0        0     1339 2023-07-12 19:24:10.856304 epson_connect-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-07-10 04:04:57.289077 epson_connect-0.2.1/src/epson_connect/__init__.py
+-rw-r--r--   0        0        0     3984 2023-07-12 19:21:10.575014 epson_connect-0.2.1/src/epson_connect/authenticate.py
+-rw-r--r--   0        0        0     1154 2023-07-09 05:46:28.548782 epson_connect-0.2.1/src/epson_connect/client.py
+-rw-r--r--   0        0        0     4465 2023-07-12 19:19:38.422590 epson_connect-0.2.1/src/epson_connect/printer.py
+-rw-r--r--   0        0        0     4924 2023-07-10 04:09:53.041881 epson_connect-0.2.1/src/epson_connect/printer_settings.py
+-rw-r--r--   0        0        0     2450 2023-07-12 19:25:30.140848 epson_connect-0.2.1/src/epson_connect/scanner.py
+-rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 epson_connect-0.2.1/PKG-INFO
```

### Comparing `epson_connect-0.2.0/LICENSE` & `epson_connect-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.0/README.md` & `epson_connect-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Epson Connect
 
 This library provides a wrapper for the Epson Connect API.
 
-NB: This library is very must still in alpha.
+NB: This library is very much still in beta.
 
 ## Install
 
 ```
 pip install epson-connect
 ```
 
@@ -23,15 +23,19 @@
 
 # Or with these enviornment variables defined...
 # export ESPON_CONNECT_API_PRINTER_EMAIL=<an email address for the device>
 # export ESPON_CONNECT_API_CLIENT_ID=<client id>
 # export ESPON_CONNECT_API_CLIENT_SECRET=<client secret>
 # ec = espon_connect.Client()
 
+# Print a PDF.
 job_id = ec.printer.print('./path/to/file.pdf')
+
+# List scan destinations.
+ec.scanner.list()
 ```
 
 ### Tests
 
 ```
 tox
 ```
```

### Comparing `epson_connect-0.2.0/pyproject.toml` & `epson_connect-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "epson-connect"
-version = "0.2.0"
+version = "0.2.1"
 description = "Bindings for the Espon Connect API"
 license = "MIT"
 authors = ["Paul Logston <paul.logston@gmail.com>"]
 maintainers = ["Paul Logston <paul.logston@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/epson-connect/"
 repository = "https://github.com/logston/epson-connect"
 keywords = ["epson", "connect", "api"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Topic :: Internet",
     "Topic :: Printing",
     "Topic :: Software Development :: Libraries",
```

### Comparing `epson_connect-0.2.0/src/epson_connect/authenticate.py` & `epson_connect-0.2.1/src/epson_connect/authenticate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 import os
 from datetime import datetime, timedelta
 
 import requests
 from requests.auth import HTTPBasicAuth
 
+logger = logging.getLogger(__name__)
+
 
 class AuthCtx:
     def __init__(
             self,
             base_url: str,
             printer_email: str,
             client_id: str,
@@ -46,15 +49,15 @@
         else:
             data = {
                 'grant_type': 'refresh_token',
                 'refresh_token': self._refresh_token,
             }
 
         try:
-            body = self.send(method, path, data, headers=headers, auth=auth)
+            body = self.send(method, path, data=data, headers=headers, auth=auth)
         except ApiError as e:
             raise AuthenticationError(e)
 
         error = body.get('error')
         if error:
             raise AuthenticationError(error)
 
@@ -70,28 +73,41 @@
         """
         Cancel authentication.
         """
         method = 'DELETE'
         path = f'/api/1/printing/printers/{self._subject_id}'
         self.send(method, path)
 
-    def send(self, method, path, data=None, headers=None, auth=None) -> dict:
+    def send(self, method, path, data=None, json=None, headers=None, auth=None) -> dict:
         # auth is only set when we are authenticating with Client ID and Client Secret.
         # In this scenario, we do not want to call self._auth again as that
         # would cause a recursion exception.
         if not auth:
             self._auth()
 
+        headers = headers or self.default_headers
+
+        logger.debug(f'{method} {path} data={data} json={json} headers={headers} auth={bool(auth)}')
+
         resp = requests.request(
             method=method,
             url=self._base_url + path,
-            headers=headers or self.default_headers,
+            headers=headers,
             data=data,
+            json=json,
             auth=auth,
-        ).json()
+        )
+
+        # Assume JSON and fall back to raw bytes.
+        try:
+            resp = resp.json()
+        except Exception:
+            resp = {'code': resp.content.decode()}
+
+        logger.debug(f'resp={resp}')
 
         error = resp.get('code')
         if error:
             raise ApiError(error)
 
         return resp
```

### Comparing `epson_connect-0.2.0/src/epson_connect/client.py` & `epson_connect-0.2.1/src/epson_connect/client.py`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.0/src/epson_connect/printer.py` & `epson_connect-0.2.1/src/epson_connect/printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         'docx',
         'xls',
         'xlsx',
         'ppt',
         'pptx',
         'pdf',
         'jpeg',
+        'jpg',
         'bmp',
         'gif',
         'png',
         'tiff',
     }
 
     VALID_OPERATORS = {
@@ -45,29 +46,33 @@
     def _print_setting(self, settings) -> dict:
         """
         Create a print job.
         """
         method = 'POST'
         path = f'/api/1/printing/printers/{self.device_id}/jobs'
 
-        return self._auth_ctx.send(method, path, settings)
+        return self._auth_ctx.send(method, path, json=settings)
 
     def _upload_file(self, upload_uri: str, file_path: str, print_mode: str) -> None:
         """
         Upload file to be printed.
         """
         # Get extension from file path.
         extension = pathlib.Path(file_path).suffix.lower()
         if extension[1:] not in self.VALID_EXTENSIONS:
             raise PrinterError(f'{extension} is not a valid printing extension.')
 
         o = urlparse(upload_uri)
         q_dict = parse_qs(o.query)
-        q_dict['File'] = [f'1{extension}']
-        path = o._replace(query=urlencode(q_dict)).geturl()
+        q_dict = {
+            'Key': q_dict['Key'][0],
+            'File': f'1{extension}',
+        }
+        o = o._replace(query=urlencode(q_dict))
+        path = o.path + '?' + o.query
 
         content_type = 'application/octet-stream'
         if print_mode == 'photo':
             content_type = 'image/jpeg'
 
         with open(file_path, 'rb') as fp:
             data = fp.read()
@@ -116,15 +121,15 @@
         if job_status not in ('pending', 'pending_held'):
             raise PrinterError(f'Can not cancel job with status {job_status}')
 
         data = {
             'operated_by': operated_by,
         }
 
-        self._auth_ctx.send(method, path, data)
+        self._auth_ctx.send(method, path, json=data)
 
     def job_info(self, job_id):
         """
         Get print job information.
         """
         method = 'GET'
         path = f'/api/1/printing/printers/{self.device_id}/jobs/{job_id}'
@@ -146,12 +151,12 @@
         path = f'/api/1/printing/printers/{self.device_id}/settings/notifications'
 
         data = {
             'notification': enabled,
             'callback_uri': callback_uri,
         }
 
-        return self._auth_ctx.send(method, path, data)
+        return self._auth_ctx.send(method, path, json=data)
 
 
 class PrinterError(ValueError):
     pass
```

### Comparing `epson_connect-0.2.0/src/epson_connect/printer_settings.py` & `epson_connect-0.2.1/src/epson_connect/printer_settings.py`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.0/src/epson_connect/scanner.py` & `epson_connect-0.2.1/src/epson_connect/scanner.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         data = {
             'alias_name': name,
             'type': type_,
             'destination': destination,
         }
 
-        resp = self._auth_ctx.send(method, self._path, data)
+        resp = self._auth_ctx.send(method, self._path, json=data)
         self._destination_cache[resp['id']] = resp
         return resp
 
     def update(self, id_, name=None, destination=None, type_=None):
         """
         Update scan destination.
         """
@@ -52,29 +52,29 @@
         data = {
             'id': id_,
             'alias_name': name if name else dest_cache['alias_name'],
             'type': type_ if type_ else dest_cache['type'],
             'destination': destination if destination else dest_cache['destination'],
         }
 
-        resp = self._auth_ctx.send(method, self._path, data)
+        resp = self._auth_ctx.send(method, self._path, json=data)
         self._destination_cache[id_] = resp
         return resp
 
     def remove(self, id_):
         """
         Update scan destination.
         """
         method = 'DELETE'
 
         data = {
             'id': id_,
         }
 
-        self._auth_ctx.send(method, self._path, data)
+        self._auth_ctx.send(method, self._path, json=data)
 
         del self._destination_cache[id_]
 
     def _validate_destination(self, name, destination, type_):
         if len(name) < 1 or len(name) > 32:
             raise ScannerError('Scan destination name too long.')
```

### Comparing `epson_connect-0.2.0/PKG-INFO` & `epson_connect-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: epson-connect
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bindings for the Espon Connect API
 Home-page: https://pypi.org/project/epson-connect/
 License: MIT
 Keywords: epson,connect,api
 Author: Paul Logston
 Author-email: paul.logston@gmail.com
 Maintainer: Paul Logston
 Maintainer-email: paul.logston@gmail.com
 Requires-Python: >=3.9
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -27,15 +27,15 @@
 Project-URL: Repository, https://github.com/logston/epson-connect
 Description-Content-Type: text/markdown
 
 # Epson Connect
 
 This library provides a wrapper for the Epson Connect API.
 
-NB: This library is very must still in alpha.
+NB: This library is very much still in beta.
 
 ## Install
 
 ```
 pip install epson-connect
 ```
 
@@ -52,15 +52,19 @@
 
 # Or with these enviornment variables defined...
 # export ESPON_CONNECT_API_PRINTER_EMAIL=<an email address for the device>
 # export ESPON_CONNECT_API_CLIENT_ID=<client id>
 # export ESPON_CONNECT_API_CLIENT_SECRET=<client secret>
 # ec = espon_connect.Client()
 
+# Print a PDF.
 job_id = ec.printer.print('./path/to/file.pdf')
+
+# List scan destinations.
+ec.scanner.list()
 ```
 
 ### Tests
 
 ```
 tox
 ```
```

