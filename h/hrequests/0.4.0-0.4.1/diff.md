# Comparing `tmp/hrequests-0.4.0.tar.gz` & `tmp/hrequests-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrequests-0.4.0.tar", max compression
+gzip compressed data, was "hrequests-0.4.1.tar", max compression
```

## Comparing `hrequests-0.4.0.tar` & `hrequests-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.4.0/hrequests/__init__.py
--rw-r--r--   0        0        0      143 2023-07-11 01:20:05.895609 hrequests-0.4.0/hrequests/__version__.py
--rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.4.0/hrequests/bin/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.4.0/hrequests/bin/LICENSE.txt
--rw-r--r--   0        0        0    23097 2023-07-08 02:07:11.879627 hrequests-0.4.0/hrequests/browser.py
--rw-r--r--   0        0        0     2771 2023-07-07 18:22:10.146220 hrequests-0.4.0/hrequests/cffi.py
--rw-r--r--   0        0        0    14008 2023-07-10 23:07:26.244002 hrequests-0.4.0/hrequests/client.py
--rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.4.0/hrequests/cookies.py
--rw-r--r--   0        0        0      723 2023-07-09 08:14:06.945274 hrequests-0.4.0/hrequests/exceptions.py
--rw-r--r--   0        0        0    19488 2023-07-09 08:47:23.150659 hrequests-0.4.0/hrequests/parser.py
--rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.4.0/hrequests/playwright_mock/__init__.py
--rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.4.0/hrequests/playwright_mock/context.py
--rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.4.0/hrequests/playwright_mock/element_handle.py
--rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.4.0/hrequests/playwright_mock/faker.py
--rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.4.0/hrequests/playwright_mock/frame.py
--rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.4.0/hrequests/playwright_mock/frame_locator.py
--rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.4.0/hrequests/playwright_mock/js_handle.py
--rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.4.0/hrequests/playwright_mock/locale.json
--rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.4.0/hrequests/playwright_mock/locator.py
--rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.4.0/hrequests/playwright_mock/mouse.py
--rw-r--r--   0        0        0    17529 2023-07-07 19:00:57.200997 hrequests-0.4.0/hrequests/playwright_mock/page.py
--rw-r--r--   0        0        0     1823 2023-07-08 02:07:11.739522 hrequests-0.4.0/hrequests/playwright_mock/playwright_mock.py
--rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.4.0/hrequests/playwright_mock/proxy_manager.py
--rw-r--r--   0        0        0    13766 2023-07-10 18:59:11.917298 hrequests-0.4.0/hrequests/reqs.py
--rw-r--r--   0        0        0     8573 2023-07-11 01:26:16.315730 hrequests-0.4.0/hrequests/response.py
--rw-r--r--   0        0        0    11808 2023-07-11 01:15:28.768157 hrequests-0.4.0/hrequests/session.py
--rw-r--r--   0        0        0     4715 2023-07-11 01:15:09.826071 hrequests-0.4.0/hrequests/toolbelt.py
--rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.4.0/LICENSE
--rw-r--r--   0        0        0     1022 2023-07-11 01:20:04.224146 hrequests-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    32506 2023-07-11 01:17:13.695947 hrequests-0.4.0/README.md
--rw-r--r--   0        0        0    32945 1970-01-01 00:00:00.000000 hrequests-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.4.1/hrequests/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-12 07:04:57.398235 hrequests-0.4.1/hrequests/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.4.1/hrequests/bin/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.4.1/hrequests/bin/LICENSE.txt
+-rw-r--r--   0        0        0    23097 2023-07-08 02:07:11.879627 hrequests-0.4.1/hrequests/browser.py
+-rw-r--r--   0        0        0     2771 2023-07-07 18:22:10.146220 hrequests-0.4.1/hrequests/cffi.py
+-rw-r--r--   0        0        0    13867 2023-07-12 07:02:34.366272 hrequests-0.4.1/hrequests/client.py
+-rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.4.1/hrequests/cookies.py
+-rw-r--r--   0        0        0      723 2023-07-09 08:14:06.945274 hrequests-0.4.1/hrequests/exceptions.py
+-rw-r--r--   0        0        0    19488 2023-07-09 08:47:23.150659 hrequests-0.4.1/hrequests/parser.py
+-rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.4.1/hrequests/playwright_mock/__init__.py
+-rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.4.1/hrequests/playwright_mock/context.py
+-rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.4.1/hrequests/playwright_mock/element_handle.py
+-rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.4.1/hrequests/playwright_mock/faker.py
+-rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.4.1/hrequests/playwright_mock/frame.py
+-rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.4.1/hrequests/playwright_mock/frame_locator.py
+-rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.4.1/hrequests/playwright_mock/js_handle.py
+-rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.4.1/hrequests/playwright_mock/locale.json
+-rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.4.1/hrequests/playwright_mock/locator.py
+-rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.4.1/hrequests/playwright_mock/mouse.py
+-rw-r--r--   0        0        0    17529 2023-07-07 19:00:57.200997 hrequests-0.4.1/hrequests/playwright_mock/page.py
+-rw-r--r--   0        0        0     1823 2023-07-08 02:07:11.739522 hrequests-0.4.1/hrequests/playwright_mock/playwright_mock.py
+-rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.4.1/hrequests/playwright_mock/proxy_manager.py
+-rw-r--r--   0        0        0    13766 2023-07-10 18:59:11.917298 hrequests-0.4.1/hrequests/reqs.py
+-rw-r--r--   0        0        0     8573 2023-07-11 01:26:16.315730 hrequests-0.4.1/hrequests/response.py
+-rw-r--r--   0        0        0    11917 2023-07-12 07:00:19.769672 hrequests-0.4.1/hrequests/session.py
+-rw-r--r--   0        0        0     4715 2023-07-11 01:15:09.826071 hrequests-0.4.1/hrequests/toolbelt.py
+-rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1022 2023-07-12 07:04:51.447345 hrequests-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    32580 2023-07-12 07:00:26.322650 hrequests-0.4.1/README.md
+-rw-r--r--   0        0        0    33018 1970-01-01 00:00:00.000000 hrequests-0.4.1/PKG-INFO
```

### Comparing `hrequests-0.4.0/hrequests/bin/LICENSE.txt` & `hrequests-0.4.1/hrequests/bin/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/browser.py` & `hrequests-0.4.1/hrequests/browser.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/cffi.py` & `hrequests-0.4.1/hrequests/cffi.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/client.py` & `hrequests-0.4.1/hrequests/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,21 +270,21 @@
         self.debug = debug
 
     def execute_request(
         self,
         method: str,
         url: str,
         data: Optional[Union[str, bytes, bytearray, dict]] = None,
-        headers: Optional[Union[dict, CaseInsensitiveDict]] = None,  # Optional[dict[str, str]]
-        cookies: Optional[Union[RequestsCookieJar, dict, list]] = None,  # Optional[dict[str, str]]
-        json: Optional[Union[dict, list, str]] = None,  # Optional[dict]
-        allow_redirects: Optional[bool] = False,
-        insecure_skip_verify: Optional[bool] = False,
-        timeout_seconds: int = 30,
-        proxy: Optional[dict] = None,  # Optional[dict[str, str]]
+        headers: Optional[Union[dict, CaseInsensitiveDict]] = None,
+        cookies: Optional[Union[RequestsCookieJar, dict, list]] = None,
+        json: Optional[Union[dict, list, str]] = None,
+        allow_redirects: bool = False,
+        verify: Optional[bool] = None,
+        timeout: Optional[int] = None,
+        proxy: Optional[dict] = None,
     ):
         # Prepare request body - build request body
         # Data has priority. JSON is only used if data is None.
         if data is None and json is not None:
             if type(json) in (dict, list):
                 json = dumps(json).decode('utf-8')
             request_body = json
@@ -341,25 +341,25 @@
             'sessionId': self._session_id,
             'followRedirects': allow_redirects,
             'forceHttp1': self.force_http1,
             'withDebug': self.debug,
             'catchPanics': self.catch_panics,
             'headers': dict(headers) if isinstance(headers, CaseInsensitiveDict) else headers,
             'headerOrder': self.header_order,
-            'insecureSkipVerify': insecure_skip_verify,
+            'insecureSkipVerify': not verify,
             'isByteRequest': is_byte_request,
             'additionalDecode': self.additional_decode,
             'proxyUrl': proxy,
             'requestUrl': url,
             'requestMethod': method,
             'requestBody': base64.b64encode(request_body).decode()
             if is_byte_request
             else request_body,
             'requestCookies': cookiejar_to_list(self.cookies),
-            'timeoutSeconds': timeout_seconds,
+            'timeoutSeconds': timeout,
         }
         if self.client_identifier is None:
             request_payload['customTlsClient'] = {
                 'ja3String': self.ja3_string,
                 'h2Settings': self.h2_settings,
                 'h2SettingsOrder': self.h2_settings_order,
                 'pseudoHeaderOrder': self.pseudo_header_order,
```

### Comparing `hrequests-0.4.0/hrequests/cookies.py` & `hrequests-0.4.1/hrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/exceptions.py` & `hrequests-0.4.1/hrequests/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/parser.py` & `hrequests-0.4.1/hrequests/parser.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/context.py` & `hrequests-0.4.1/hrequests/playwright_mock/context.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/element_handle.py` & `hrequests-0.4.1/hrequests/playwright_mock/element_handle.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/faker.py` & `hrequests-0.4.1/hrequests/playwright_mock/faker.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/frame.py` & `hrequests-0.4.1/hrequests/playwright_mock/frame.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/frame_locator.py` & `hrequests-0.4.1/hrequests/playwright_mock/frame_locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/locale.json` & `hrequests-0.4.1/hrequests/playwright_mock/locale.json`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/locator.py` & `hrequests-0.4.1/hrequests/playwright_mock/locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/mouse.py` & `hrequests-0.4.1/hrequests/playwright_mock/mouse.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/page.py` & `hrequests-0.4.1/hrequests/playwright_mock/page.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/playwright_mock.py` & `hrequests-0.4.1/hrequests/playwright_mock/playwright_mock.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/playwright_mock/proxy_manager.py` & `hrequests-0.4.1/hrequests/playwright_mock/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/reqs.py` & `hrequests-0.4.1/hrequests/reqs.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/response.py` & `hrequests-0.4.1/hrequests/response.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/hrequests/session.py` & `hrequests-0.4.1/hrequests/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     Args:
         browser (str): Browser to use [firefox, chrome, opera]
         client_identifier (str): Identifier for the client
         os (Literal['win', 'mac', 'lin'], optional): OS to use in header [win, mac, lin]
         headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
         temp (bool, optional): Indicates if session is temporary. Defaults to False.
         verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+        timeout (int, optional): Default timeout in seconds. Defaults to 30.
         ja3_string (str, optional): JA3 string. Defaults to None.
         h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
         additional_decode (str, optional): Additional decode. Defaults to None.
         pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
         priority_frames (list, optional): Priority frames. Defaults to None.
         header_order (list, optional): Header order. Defaults to None.
         force_http1 (bool, optional): Force HTTP/1. Defaults to False.
@@ -58,14 +59,15 @@
         self,
         client_identifier: str,
         browser: Literal['firefox', 'chrome', 'opera'],
         os: Optional[Literal['win', 'mac', 'lin']] = None,
         headers: Optional[dict] = None,
         temp: bool = False,
         verify: bool = True,
+        timeout: int = 30,
         *args,
         **kwargs,
     ):
         super().__init__(client_identifier=client_identifier, *args, **kwargs)
 
         # sync network methods
         self.get: partial = partial(get, session=self)
@@ -89,14 +91,15 @@
         self.render: partial = partial(hrequests.browser.render, session=self)
 
         self.temp: bool = temp  # indicate if session is temporary
         self._closed: bool = False  # indicate if session is closed
         self.browser: str = browser  # browser name
         self._os: str = os or rchoice(('win', 'mac', 'lin'))  # os name
         self.verify: bool = verify  # default to verifying certs
+        self.timeout: int = timeout  # default timeout
 
         # set headers
         if headers:
             self.headers = CaseInsensitiveDict(headers)
         else:
             self.resetHeaders(os=os)
 
@@ -132,16 +135,16 @@
         data: Optional[Union[str, bytes, bytearray, dict]] = None,
         files: Optional[dict] = None,
         headers: Optional[Union[dict, CaseInsensitiveDict]] = None,
         cookies: Optional[Union[RequestsCookieJar, dict, list]] = None,
         json: Optional[Union[dict, list, str]] = None,
         allow_redirects: bool = True,
         history: bool = False,
-        verify: bool = True,  # maps to insecure_skip_verify
-        timeout: int = 30,  # maps to timeout_seconds
+        verify: Optional[bool] = None,
+        timeout: Optional[int] = None,
         proxies: Optional[dict] = None,
     ) -> 'hrequests.response.Response':
         """
         Send a request with TLS client
 
         Args:
             method (str): Method of request (GET, POST, OPTIONS, HEAD, PUT, PATCH, DELETE)
@@ -156,29 +159,27 @@
             verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
             timeout (int, optional): Timeout in seconds. Defaults to 30.
             proxies (dict, optional): Dictionary of proxies. Defaults to None.
 
         Returns:
             hrequests.response.Response: Response object
         """
-        if verify is None:
-            verify = self.verify
         proc = ProcessResponse(
             session=self,
             method=method,
             url=url,
             data=data,
             files=files,
             headers=headers,
             cookies=cookies,
             json=json,
             allow_redirects=allow_redirects,
             chain=history,
-            insecure_skip_verify=not verify,
-            timeout_seconds=timeout,
+            verify=self.verify if verify is None else verify,
+            timeout=self.timeout if timeout is None else timeout,
             proxy=proxies,
         )
         proc.send()
         return proc.response
 
     def close(self):
         if not self._closed:
```

### Comparing `hrequests-0.4.0/hrequests/toolbelt.py` & `hrequests-0.4.1/hrequests/toolbelt.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/LICENSE` & `hrequests-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.0/pyproject.toml` & `hrequests-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hrequests"
-version = "0.4.0"
+version = "0.4.1"
 description = "Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library."
 authors = ["daijro <daijro.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/daijro/hrequests"
 keywords = ["tls", "client", "http", "scraping", "requests", "humans", "playwright"]
 classifiers = [
```

### Comparing `hrequests-0.4.0/README.md` & `hrequests-0.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,15 @@
 ```
 Parameters:
     browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'chrome'.
     version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
     os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+    timeout (int, optional): Default timeout in seconds. Defaults to 30.
     ja3_string (str, optional): JA3 string. Defaults to None.
     h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
     additional_decode (str, optional): Additional decode. Defaults to None.
     pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
     priority_frames (list, optional): Priority frames. Defaults to None.
     header_order (list, optional): Header order. Defaults to None.
     force_http1 (bool, optional): Force HTTP/1. Defaults to False.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope__7a6ep11_/tmpnw2210tt_TarContainer/0/29.md", line 1018, column 3: CDATA terminal not found*

 * *File "/tmp/diffoscope__7a6ep11_/tmpnw2210tt_TarContainer/0/29.md", line 1018, column 3: CDATA terminal not found*

```diff
@@ -68,17 +68,18 @@
 hrequests.Session('chrome', version=112) ```  Parameters ``` Parameters:
 browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use.
 Default is 'chrome'. version (int, optional): Version of the browser to use.
 Browser must be specified. Default is randomized. os (Literal['win', 'mac',
 'lin'], optional): OS to use in header. Default is randomized. headers (dict,
 optional): Dictionary of HTTP headers to send with the request. Default is
 generated from `browser` and `os`. verify (bool, optional): Verify the server's
-TLS certificate. Defaults to True. ja3_string (str, optional): JA3 string.
-Defaults to None. h2_settings (dict, optional): HTTP/2 settings. Defaults to
-None. additional_decode (str, optional): Additional decode. Defaults to None.
+TLS certificate. Defaults to True. timeout (int, optional): Default timeout in
+seconds. Defaults to 30. ja3_string (str, optional): JA3 string. Defaults to
+None. h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
+additional_decode (str, optional): Additional decode. Defaults to None.
 pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
 priority_frames (list, optional): Priority frames. Defaults to None.
 header_order (list, optional): Header order. Defaults to None. force_http1
 (bool, optional): Force HTTP/1. Defaults to False. catch_panics (bool,
 optional): Catch panics. Defaults to False. debug (bool, optional): Debug mode.
 Defaults to False. ```  Browsers can also be created through the `firefox`,
 `chrome`, and `opera` shortcuts: ```py >>> session = hrequests.firefox.Session
```

### Comparing `hrequests-0.4.0/PKG-INFO` & `hrequests-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrequests
-Version: 0.4.0
+Version: 0.4.1
 Summary: Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
 Home-page: https://github.com/daijro/hrequests
 License: Apache-2.0
 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro
 Author-email: daijro.dev@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -238,14 +238,15 @@
 ```
 Parameters:
     browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'chrome'.
     version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
     os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+    timeout (int, optional): Default timeout in seconds. Defaults to 30.
     ja3_string (str, optional): JA3 string. Defaults to None.
     h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
     additional_decode (str, optional): Additional decode. Defaults to None.
     pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
     priority_frames (list, optional): Priority frames. Defaults to None.
     header_order (list, optional): Header order. Defaults to None.
     force_http1 (bool, optional): Force HTTP/1. Defaults to False.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope__7a6ep11_/tmpnw2210tt_TarContainer/0/30", line 1058, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope__7a6ep11_/tmpnw2210tt_TarContainer/0/30", line 1058, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hrequests Version: 0.4.0 Summary: Hrequests (human
+Metadata-Version: 2.1 Name: hrequests Version: 0.4.1 Summary: Hrequests (human
 requests) is a simple, configurable, feature-rich, replacement for the Python
 requests library. Home-page: https://github.com/daijro/hrequests License:
 Apache-2.0 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro Author-email: daijro.dev@gmail.com Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -87,17 +87,18 @@
 hrequests.Session('chrome', version=112) ```  Parameters ``` Parameters:
 browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use.
 Default is 'chrome'. version (int, optional): Version of the browser to use.
 Browser must be specified. Default is randomized. os (Literal['win', 'mac',
 'lin'], optional): OS to use in header. Default is randomized. headers (dict,
 optional): Dictionary of HTTP headers to send with the request. Default is
 generated from `browser` and `os`. verify (bool, optional): Verify the server's
-TLS certificate. Defaults to True. ja3_string (str, optional): JA3 string.
-Defaults to None. h2_settings (dict, optional): HTTP/2 settings. Defaults to
-None. additional_decode (str, optional): Additional decode. Defaults to None.
+TLS certificate. Defaults to True. timeout (int, optional): Default timeout in
+seconds. Defaults to 30. ja3_string (str, optional): JA3 string. Defaults to
+None. h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
+additional_decode (str, optional): Additional decode. Defaults to None.
 pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
 priority_frames (list, optional): Priority frames. Defaults to None.
 header_order (list, optional): Header order. Defaults to None. force_http1
 (bool, optional): Force HTTP/1. Defaults to False. catch_panics (bool,
 optional): Catch panics. Defaults to False. debug (bool, optional): Debug mode.
 Defaults to False. ```  Browsers can also be created through the `firefox`,
 `chrome`, and `opera` shortcuts: ```py >>> session = hrequests.firefox.Session
```

