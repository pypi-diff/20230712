# Comparing `tmp/robocorp_storage-0.2.0.tar.gz` & `tmp/robocorp_storage-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_storage-0.2.0.tar", max compression
+gzip compressed data, was "robocorp_storage-0.3.0.tar", max compression
```

## Comparing `robocorp_storage-0.2.0.tar` & `robocorp_storage-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0      388 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/README.md
--rw-r--r--   0        0        0      801 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5321 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/src/robocorp/storage/__init__.py
--rw-r--r--   0        0        0     6642 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/src/robocorp/storage/_requests.py
--rw-r--r--   0        0        0     3739 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/src/robocorp/storage/_storage.py
--rw-r--r--   0        0        0        0 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/src/robocorp/storage/py.typed
--rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 robocorp_storage-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      385 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/README.md
+-rw-r--r--   0        0        0      801 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7283 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/__init__.py
+-rw-r--r--   0        0        0     6044 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_client.py
+-rw-r--r--   0        0        0     2354 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_environment.py
+-rw-r--r--   0        0        0     6343 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_requests.py
+-rw-r--r--   0        0        0     1904 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_types.py
+-rw-r--r--   0        0        0      170 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/py.typed
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 robocorp_storage-0.3.0/PKG-INFO
```

### Comparing `robocorp_storage-0.2.0/pyproject.toml` & `robocorp_storage-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-storage"
-version = "0.2.0"
+version = "0.3.0"
 description = "Robocorp Asset Storage library"
 authors = [
 	"Cosmin P. <cosmin@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
```

### Comparing `robocorp_storage-0.2.0/src/robocorp/storage/_requests.py` & `robocorp_storage-0.3.0/src/robocorp/storage/_requests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import logging
 import os
 import random
 import time
-import urllib.parse as urlparse
+import urllib.parse
 from typing import Callable, Optional
 
 import requests
-from requests.exceptions import HTTPError
+from requests.exceptions import HTTPError as _HTTPError
 from tenacity import (
     before_sleep_log,
     retry,
     retry_if_exception,
     stop_after_attempt,
     wait_random_exponential,
 )
@@ -27,15 +27,15 @@
     # 400 - payload is bad and needs to be changed
     # 401 - missing auth bearer token
     # 403 - auth is in place, but not allowed (insufficient privileges)
     # 404 - resource does not exist
     # 409 - payload not good for the affected resource
     no_retry_codes = [400, 401, 403, 404, 409]
 
-    if isinstance(exc, RequestsHTTPError):
+    if isinstance(exc, HTTPError):
         if exc.status_code in no_retry_codes:
             return False
 
         if exc.status_code == 429:
             # We hit the rate limiter, so sleep extra before retrying.
             seconds = round(random.uniform(1, 3), 2)
             LOGGER.warning("Rate limit hit, sleeping %.2fs...", seconds)
@@ -54,78 +54,79 @@
 
     # Monkeypatch inner logging function so it produces an exhaustive log when
     # used under the before-sleep logging utility in `tenacity`.
     LOGGER.log = extensive_log
     return before_sleep_log(LOGGER, logging.DEBUG, exc_info=True)
 
 
-class RequestsHTTPError(HTTPError):
-    """Custom `requests` HTTP error with status code and message."""
+# Exported for ease-of-use
+Response = requests.Response
 
-    def __init__(
-        self,
-        *args,
-        status_code: int = 0,
-        status_message: str = "Error",
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
 
+class HTTPError(_HTTPError):
+    """Custom `requests` HTTP error with status code and reason"""
+
+    def __init__(self, message: str, status_code: int, reason: str):
+        super().__init__(message)
+        self.message = message
         self.status_code = status_code
-        self.status_message = status_message
+        self.reason = reason
+
+    def __str__(self):
+        return f"{self.status_code} {self.reason} - {self.message}"
 
 
 class Requests:
     """Wrapper over `requests` 3rd-party with error handling and retrying support."""
 
-    def __init__(self, route_prefix: str, default_headers: Optional[dict] = None):
+    def __init__(self, route_prefix: str = "", default_headers: Optional[dict] = None):
         self._route_prefix = route_prefix
         self._default_headers = default_headers
 
     def handle_error(self, response: requests.Response):
-        resp_status_code = response.status_code
-        log_func = LOGGER.critical if resp_status_code // 100 == 5 else LOGGER.debug
-        log_func("API response: %s %r", resp_status_code, response.reason)
+        http_status = f"{response.status_code} {response.reason!r}"
+        if 500 <= response.status_code < 600:
+            LOGGER.critical("Server error: %s", http_status)
+        elif 400 <= response.status_code < 500:
+            LOGGER.info("Client error: %s", http_status)
+        else:
+            LOGGER.debug("Response: %s", http_status)
 
         if response.ok:
             return
 
-        fields = {}
+        # Fallback values
+        status_code = response.status_code
+        reason = response.reason
+        message = response.text
+
         try:
             fields = response.json()
+
+            # For some reason we might still get a string from the deserialized
+            # JSON payload, possible due to some double encoding bug in CR
             while not isinstance(fields, dict):
-                # For some reason we might still get a string from the deserialized
-                # retrieved JSON payload. If a dictionary couldn't be obtained at all,
-                # it will end up raising `RequestsHTTPError`.
                 fields = json.loads(fields)
-        except (json.JSONDecodeError, ValueError, TypeError):
-            # No `fields` dictionary can be obtained at all.
-            LOGGER.critical("No fields were returned by the server")
-            try:
-                response.raise_for_status()
-            except Exception as exc:
-                LOGGER.exception(exc)
-                raise RequestsHTTPError(exc, status_code=resp_status_code) from exc
 
-        err_status_code = 0
-        status_message = "Error"
-        try:
-            err_status_code = int(fields.get("status", resp_status_code))
-            status_message = fields.get("code") or fields.get("error", {}).get(
-                "code", "Error"
-            )
-            reason = fields.get("message") or fields.get("error", {}).get(
-                "message", response.reason
-            )
-            raise HTTPError(f"{err_status_code} {status_message}: {reason}")
+            if "status" in fields:
+                status_code = int(fields["status"])
+
+            if "code" in fields:
+                reason = fields["code"]
+            elif "error" in fields and "code" in fields["error"]:
+                reason = fields["error"]["code"]
+
+            if "message" in fields:
+                message = fields["message"]
+            elif "error" in fields and "message" in fields["error"]:
+                message = fields["error"]["message"]
         except Exception as exc:
-            LOGGER.exception(exc)
-            raise RequestsHTTPError(
-                str(fields), status_code=err_status_code, status_message=status_message
-            ) from exc
+            LOGGER.critical("Failed to parse error response: %r", exc)
+
+        raise HTTPError(message, status_code=status_code, reason=reason)
 
     @retry(
         # Retry until either succeed or trying for the fifth time and still failing.
         # So sleep and retry for 4 times at most.
         stop=stop_after_attempt(5),
         # If the exception is no worth retrying or the number of tries is depleted,
         # then re-raise the last raised exception.
@@ -147,41 +148,36 @@
         url: str,
         *args,
         _handle_error: Optional[Callable[[requests.Response], None]] = None,
         _sensitive: bool = False,
         headers: Optional[dict] = None,
         **kwargs,
     ) -> requests.Response:
-        # Absolute URLs override the prefix, so they are safe to be sent as they'll be
-        # the same after joining.
-        url = urlparse.urljoin(self._route_prefix, url)
+        # Absolute URLs override the prefix, so they are safe to be sent
+        # as they'll be the same after joining.
+        url = urllib.parse.urljoin(self._route_prefix, url)
         headers = headers if headers is not None else self._default_headers
         handle_error = _handle_error or self.handle_error
 
-        url_for_log = url
+        log_url = url
         if _sensitive:
             # Omit query from the URL since might contain sensitive info.
-            split = urlparse.urlsplit(url_for_log)
-            url_for_log = urlparse.urlunsplit(
-                [split.scheme, split.netloc, split.path, "", split.fragment]
-            )
+            split = urllib.parse.urlsplit(log_url)
+            split = split._replace(query="")
+            log_url = urllib.parse.urlunsplit(split)
 
-        LOGGER.debug("%s %r", verb.__name__.upper(), url_for_log)
+        LOGGER.debug("%s %r", verb.__name__.upper(), log_url)
         response = verb(url, *args, headers=headers, **kwargs)
         handle_error(response)
         return response
 
-    # CREATE
     def post(self, *args, **kwargs) -> requests.Response:
         return self._request(requests.post, *args, **kwargs)
 
-    # RETRIEVE
     def get(self, *args, **kwargs) -> requests.Response:
         return self._request(requests.get, *args, **kwargs)
 
-    # UPDATE
     def put(self, *args, **kwargs) -> requests.Response:
         return self._request(requests.put, *args, **kwargs)
 
-    # DELETE
     def delete(self, *args, **kwargs) -> requests.Response:
         return self._request(requests.delete, *args, **kwargs)
```

### Comparing `robocorp_storage-0.2.0/PKG-INFO` & `robocorp_storage-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-storage
-Version: 0.2.0
+Version: 0.3.0
 Summary: Robocorp Asset Storage library
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Cosmin P.
 Author-email: cosmin@robocorp.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,19 +21,18 @@
 Description-Content-Type: text/markdown
 
 # Robocorp Control Room Asset Storage API library
 
 `robocorp-storage` is a library which provides read and write access to the
 *Asset Storage* in Robocorp **Control Room**.
 
-
 ## Usage
 
 ```python
 from robocorp import storage
 
 def store_email():
-    storage.set_asset("cosmin", "cosmin@robocorp.com")
-    print("E-mail:", storage.get_asset("cosmin"))
+    storage.set_text("cosmin", "cosmin@robocorp.com")
+    print("E-mail:", storage.get_text("cosmin"))
     storage.delete_asset("cosmin")
 ```
```

