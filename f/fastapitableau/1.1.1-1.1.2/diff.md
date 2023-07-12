# Comparing `tmp/fastapitableau-1.1.1.tar.gz` & `tmp/fastapitableau-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapitableau-1.1.1.tar", last modified: Wed Feb 23 19:57:49 2022, max compression
+gzip compressed data, was "fastapitableau-1.1.2.tar", last modified: Tue Jul 11 21:31:09 2023, max compression
```

## Comparing `fastapitableau-1.1.1.tar` & `fastapitableau-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxr-xr-x   0 toph       (501) staff       (20)        0 2022-02-23 19:57:49.685658 fastapitableau-1.1.1/
--rw-r--r--   0 toph       (501) staff       (20)       78 2021-09-16 15:20:23.000000 fastapitableau-1.1.1/MANIFEST.in
--rw-r--r--   0 toph       (501) staff       (20)     8804 2022-02-23 19:57:49.685854 fastapitableau-1.1.1/PKG-INFO
--rw-r--r--   0 toph       (501) staff       (20)     8005 2022-02-23 19:41:14.000000 fastapitableau-1.1.1/README.md
-drwxr-xr-x   0 toph       (501) staff       (20)        0 2022-02-23 19:57:49.677666 fastapitableau-1.1.1/fastapitableau/
--rw-r--r--   0 toph       (501) staff       (20)       55 2021-10-28 22:37:22.000000 fastapitableau-1.1.1/fastapitableau/__init__.py
--rw-r--r--   0 toph       (501) staff       (20)     3501 2021-10-28 22:37:22.000000 fastapitableau-1.1.1/fastapitableau/applications.py
--rw-r--r--   0 toph       (501) staff       (20)     1544 2021-09-27 15:23:28.000000 fastapitableau-1.1.1/fastapitableau/exception_handlers.py
--rw-r--r--   0 toph       (501) staff       (20)     1420 2021-10-28 22:37:22.000000 fastapitableau-1.1.1/fastapitableau/logger.py
--rw-r--r--   0 toph       (501) staff       (20)     1756 2021-10-28 22:37:22.000000 fastapitableau-1.1.1/fastapitableau/middleware.py
--rw-r--r--   0 toph       (501) staff       (20)     6060 2021-10-28 22:37:22.000000 fastapitableau-1.1.1/fastapitableau/openapi.py
--rw-r--r--   0 toph       (501) staff       (20)     3834 2021-10-28 22:37:22.000000 fastapitableau-1.1.1/fastapitableau/pages.py
--rw-r--r--   0 toph       (501) staff       (20)     5668 2021-10-28 22:37:22.000000 fastapitableau-1.1.1/fastapitableau/routing.py
--rw-r--r--   0 toph       (501) staff       (20)     7221 2022-02-23 19:41:14.000000 fastapitableau-1.1.1/fastapitableau/rstudio_connect.py
-drwxr-xr-x   0 toph       (501) staff       (20)        0 2022-02-23 19:57:49.669026 fastapitableau-1.1.1/fastapitableau/statics/
-drwxr-xr-x   0 toph       (501) staff       (20)        0 2022-02-23 19:57:49.681895 fastapitableau-1.1.1/fastapitableau/statics/css/
--rw-r--r--   0 toph       (501) staff       (20)    21241 2021-09-27 15:23:28.000000 fastapitableau-1.1.1/fastapitableau/statics/css/styles.css
-drwxr-xr-x   0 toph       (501) staff       (20)        0 2022-02-23 19:57:49.685291 fastapitableau-1.1.1/fastapitableau/templates/
--rw-r--r--   0 toph       (501) staff       (20)    32886 2021-09-27 15:23:28.000000 fastapitableau-1.1.1/fastapitableau/templates/index.html
--rw-r--r--   0 toph       (501) staff       (20)      727 2021-09-23 14:09:48.000000 fastapitableau-1.1.1/fastapitableau/templates/param_table.html
--rw-r--r--   0 toph       (501) staff       (20)     5506 2021-09-28 19:43:10.000000 fastapitableau-1.1.1/fastapitableau/templates/setup_tableau.html
--rw-r--r--   0 toph       (501) staff       (20)     2518 2021-09-27 15:23:28.000000 fastapitableau-1.1.1/fastapitableau/templates/tableau_usage.html
--rw-r--r--   0 toph       (501) staff       (20)     1787 2021-09-27 15:23:28.000000 fastapitableau-1.1.1/fastapitableau/templates/user_guide.html
--rw-r--r--   0 toph       (501) staff       (20)     3710 2021-09-28 19:43:10.000000 fastapitableau-1.1.1/fastapitableau/user_guide.py
--rw-r--r--   0 toph       (501) staff       (20)     1058 2021-10-06 21:17:32.000000 fastapitableau-1.1.1/fastapitableau/utils.py
-drwxr-xr-x   0 toph       (501) staff       (20)        0 2022-02-23 19:57:49.681077 fastapitableau-1.1.1/fastapitableau.egg-info/
--rw-r--r--   0 toph       (501) staff       (20)     8804 2022-02-23 19:57:49.000000 fastapitableau-1.1.1/fastapitableau.egg-info/PKG-INFO
--rw-r--r--   0 toph       (501) staff       (20)      834 2022-02-23 19:57:49.000000 fastapitableau-1.1.1/fastapitableau.egg-info/SOURCES.txt
--rw-r--r--   0 toph       (501) staff       (20)        1 2022-02-23 19:57:49.000000 fastapitableau-1.1.1/fastapitableau.egg-info/dependency_links.txt
--rw-r--r--   0 toph       (501) staff       (20)       59 2022-02-23 19:57:49.000000 fastapitableau-1.1.1/fastapitableau.egg-info/requires.txt
--rw-r--r--   0 toph       (501) staff       (20)       15 2022-02-23 19:57:49.000000 fastapitableau-1.1.1/fastapitableau.egg-info/top_level.txt
--rw-r--r--   0 toph       (501) staff       (20)        1 2021-08-26 16:09:32.000000 fastapitableau-1.1.1/fastapitableau.egg-info/zip-safe
--rw-r--r--   0 toph       (501) staff       (20)      201 2021-10-19 19:46:31.000000 fastapitableau-1.1.1/pyproject.toml
--rw-r--r--   0 toph       (501) staff       (20)     1365 2022-02-23 19:57:49.687215 fastapitableau-1.1.1/setup.cfg
--rw-r--r--   0 toph       (501) staff       (20)       74 2021-08-26 15:41:17.000000 fastapitableau-1.1.1/setup.py
+drwxr-xr-x   0 toph       (502) staff       (20)        0 2023-07-11 21:31:09.923467 fastapitableau-1.1.2/
+-rw-r--r--   0 toph       (502) staff       (20)       78 2021-09-16 15:20:23.000000 fastapitableau-1.1.2/MANIFEST.in
+-rw-r--r--   0 toph       (502) staff       (20)     8784 2023-07-11 21:31:09.923542 fastapitableau-1.1.2/PKG-INFO
+-rw-r--r--   0 toph       (502) staff       (20)     8005 2022-02-23 19:41:14.000000 fastapitableau-1.1.2/README.md
+drwxr-xr-x   0 toph       (502) staff       (20)        0 2023-07-11 21:31:09.919467 fastapitableau-1.1.2/fastapitableau/
+-rw-r--r--   0 toph       (502) staff       (20)       55 2021-10-28 22:37:22.000000 fastapitableau-1.1.2/fastapitableau/__init__.py
+-rw-r--r--   0 toph       (502) staff       (20)     3501 2021-10-28 22:37:22.000000 fastapitableau-1.1.2/fastapitableau/applications.py
+-rw-r--r--   0 toph       (502) staff       (20)     1544 2021-09-27 15:23:28.000000 fastapitableau-1.1.2/fastapitableau/exception_handlers.py
+-rw-r--r--   0 toph       (502) staff       (20)     1446 2023-07-11 21:26:24.000000 fastapitableau-1.1.2/fastapitableau/logger.py
+-rw-r--r--   0 toph       (502) staff       (20)     1756 2021-10-28 22:37:22.000000 fastapitableau-1.1.2/fastapitableau/middleware.py
+-rw-r--r--   0 toph       (502) staff       (20)     6058 2023-07-11 21:26:24.000000 fastapitableau-1.1.2/fastapitableau/openapi.py
+-rw-r--r--   0 toph       (502) staff       (20)     3834 2021-10-28 22:37:22.000000 fastapitableau-1.1.2/fastapitableau/pages.py
+-rw-r--r--   0 toph       (502) staff       (20)     5678 2023-07-11 21:26:24.000000 fastapitableau-1.1.2/fastapitableau/routing.py
+-rw-r--r--   0 toph       (502) staff       (20)     7233 2023-07-11 21:26:24.000000 fastapitableau-1.1.2/fastapitableau/rstudio_connect.py
+drwxr-xr-x   0 toph       (502) staff       (20)        0 2023-07-11 21:31:09.916170 fastapitableau-1.1.2/fastapitableau/statics/
+drwxr-xr-x   0 toph       (502) staff       (20)        0 2023-07-11 21:31:09.920666 fastapitableau-1.1.2/fastapitableau/statics/css/
+-rw-r--r--   0 toph       (502) staff       (20)    21241 2021-09-27 15:23:28.000000 fastapitableau-1.1.2/fastapitableau/statics/css/styles.css
+drwxr-xr-x   0 toph       (502) staff       (20)        0 2023-07-11 21:31:09.921858 fastapitableau-1.1.2/fastapitableau/templates/
+-rw-r--r--   0 toph       (502) staff       (20)    32886 2021-09-27 15:23:28.000000 fastapitableau-1.1.2/fastapitableau/templates/index.html
+-rw-r--r--   0 toph       (502) staff       (20)      727 2021-09-23 14:09:48.000000 fastapitableau-1.1.2/fastapitableau/templates/param_table.html
+-rw-r--r--   0 toph       (502) staff       (20)     5506 2021-09-28 19:43:10.000000 fastapitableau-1.1.2/fastapitableau/templates/setup_tableau.html
+-rw-r--r--   0 toph       (502) staff       (20)     2518 2021-09-27 15:23:28.000000 fastapitableau-1.1.2/fastapitableau/templates/tableau_usage.html
+-rw-r--r--   0 toph       (502) staff       (20)     1787 2021-09-27 15:23:28.000000 fastapitableau-1.1.2/fastapitableau/templates/user_guide.html
+-rw-r--r--   0 toph       (502) staff       (20)     3710 2021-09-28 19:43:10.000000 fastapitableau-1.1.2/fastapitableau/user_guide.py
+-rw-r--r--   0 toph       (502) staff       (20)     1058 2021-10-06 21:17:32.000000 fastapitableau-1.1.2/fastapitableau/utils.py
+drwxr-xr-x   0 toph       (502) staff       (20)        0 2023-07-11 21:31:09.920398 fastapitableau-1.1.2/fastapitableau.egg-info/
+-rw-r--r--   0 toph       (502) staff       (20)     8784 2023-07-11 21:31:09.000000 fastapitableau-1.1.2/fastapitableau.egg-info/PKG-INFO
+-rw-r--r--   0 toph       (502) staff       (20)     1002 2023-07-11 21:31:09.000000 fastapitableau-1.1.2/fastapitableau.egg-info/SOURCES.txt
+-rw-r--r--   0 toph       (502) staff       (20)        1 2023-07-11 21:31:09.000000 fastapitableau-1.1.2/fastapitableau.egg-info/dependency_links.txt
+-rw-r--r--   0 toph       (502) staff       (20)       67 2023-07-11 21:31:09.000000 fastapitableau-1.1.2/fastapitableau.egg-info/requires.txt
+-rw-r--r--   0 toph       (502) staff       (20)       15 2023-07-11 21:31:09.000000 fastapitableau-1.1.2/fastapitableau.egg-info/top_level.txt
+-rw-r--r--   0 toph       (502) staff       (20)        1 2021-08-26 16:09:32.000000 fastapitableau-1.1.2/fastapitableau.egg-info/zip-safe
+-rw-r--r--   0 toph       (502) staff       (20)      201 2021-10-19 19:46:31.000000 fastapitableau-1.1.2/pyproject.toml
+-rw-r--r--   0 toph       (502) staff       (20)     1374 2023-07-11 21:31:09.923876 fastapitableau-1.1.2/setup.cfg
+-rw-r--r--   0 toph       (502) staff       (20)       74 2021-08-26 15:41:17.000000 fastapitableau-1.1.2/setup.py
+drwxr-xr-x   0 toph       (502) staff       (20)        0 2023-07-11 21:31:09.923310 fastapitableau-1.1.2/tests/
+-rw-r--r--   0 toph       (502) staff       (20)     3296 2021-10-06 21:17:32.000000 fastapitableau-1.1.2/tests/test_applications.py
+-rw-r--r--   0 toph       (502) staff       (20)      961 2021-10-28 22:37:22.000000 fastapitableau-1.1.2/tests/test_logging.py
+-rw-r--r--   0 toph       (502) staff       (20)    13687 2021-09-28 19:43:10.000000 fastapitableau-1.1.2/tests/test_openapi.py
+-rw-r--r--   0 toph       (502) staff       (20)     1502 2023-07-11 21:26:24.000000 fastapitableau-1.1.2/tests/test_routing.py
+-rw-r--r--   0 toph       (502) staff       (20)      457 2021-09-22 15:59:10.000000 fastapitableau-1.1.2/tests/test_rstudio_connect.py
+-rw-r--r--   0 toph       (502) staff       (20)      688 2021-09-28 19:43:10.000000 fastapitableau-1.1.2/tests/test_user_guide.py
+-rw-r--r--   0 toph       (502) staff       (20)      380 2021-09-28 19:43:10.000000 fastapitableau-1.1.2/tests/test_utils.py
```

### Comparing `fastapitableau-1.1.1/PKG-INFO` & `fastapitableau-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fastapitableau
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package for writing FastAPI apps that you can call from Tableau.
 Home-page: https://github.com/rstudio/fastapitableau
 Author: Toph Allen, James Blair, Bill Sager
 Author-email: toph@rstudio.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -160,9 +159,7 @@
 
 - You must turn off "Aggregate Measures" under the "Analysis" menu for Tableau to pass the correct values to the extension. If this setting is on, Tableau will send aggregated data to the extension, which may cause inaccuracies in computations.
 - With this value off, calculated fields don't allow you to pass raw values directly to an extension. Those values must be wrapped in an aggregating function. Since we've turned "Aggregate Measures" off, these functions won't actually aggregate the data. We've had success using `ATTR([VALUE_NAME])`.
 
 ## Debug logging
 
 To enable verbose debug logging, set the environment variable `FASTAPITABLEAU_LOG_LEVEL` to `DEBUG`.
-
-
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: fastapitableau Version: 1.1.1 Summary: A Python
+Metadata-Version: 2.1 Name: fastapitableau Version: 1.1.2 Summary: A Python
 package for writing FastAPI apps that you can call from Tableau. Home-page:
 https://github.com/rstudio/fastapitableau Author: Toph Allen, James Blair, Bill
-Sager Author-email: toph@rstudio.com License: MIT Platform: UNKNOWN Classifier:
-Environment :: Web Environment Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3.7 Classifier: Topic :: Internet :: WWW/HTTP
-:: Dynamic Content Classifier: Topic :: Software Development :: Libraries ::
-Python Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: test
+Sager Author-email: toph@rstudio.com License: MIT Classifier: Environment ::
+Web Environment Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3.7 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+test
                                [FastAPI Tableau]
                          [Coverage] [Package_version]
 # FastAPI Tableau --- **Documentation**: [https://rstudio.github.io/
 fastapitableau](https://rstudio.github.io/fastapitableau) **Source Code**:
 [https://github.com/rstudio/fastapitableau](https://github.com/rstudio/
 fastapitableau) --- FastAPI Tableau lets you call external Python code from
 Tableau workbooks via [Tableau Analytics Extensions](https://tableau.github.io/
```

### Comparing `fastapitableau-1.1.1/README.md` & `fastapitableau-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/applications.py` & `fastapitableau-1.1.2/fastapitableau/applications.py`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/exception_handlers.py` & `fastapitableau-1.1.2/fastapitableau/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/logger.py` & `fastapitableau-1.1.2/fastapitableau/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,17 @@
         else:
             correlation_id = get_correlation_id(extra["scope"])
             kwargs["extra"]["correlation_id"] = correlation_id
             prefix = f"[{correlation_id}] " if correlation_id is not None else ""
             return prefix + msg, kwargs
 
 
-def get_correlation_id(scope: Scope = None, headers: Headers = None) -> Optional[str]:
+def get_correlation_id(
+    scope: Optional[Scope] = None, headers: Optional[Headers] = None
+) -> Optional[str]:
     headers = Headers(scope=scope, headers=headers)
     correlation_id_keys = ["x-rs-correlation-id", "x-correlation-id"]
     for key in correlation_id_keys:
         if key in headers.keys():
             return headers[key]
     return None
```

### Comparing `fastapitableau-1.1.1/fastapitableau/middleware.py` & `fastapitableau-1.1.2/fastapitableau/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/openapi.py` & `fastapitableau-1.1.2/fastapitableau/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     openapi = deepcopy(openapi)
     schemas = openapi["components"]["schemas"]
 
     if rewrite_paths is None:
         rewrite_paths = list(openapi["paths"].keys())
 
     for path_name in rewrite_paths:
-
         path = openapi["paths"][path_name]
         request_body = path.get("post").get("requestBody")
 
         if request_body is None:
             continue  # We skip rewriting functions that just take the whole request
 
         path_schema = request_body["content"]["application/json"]["schema"]
@@ -92,15 +91,14 @@
     openapi_url: str,
     title: str,
     swagger_js_url: str = "https://cdn.jsdelivr.net/npm/swagger-ui-dist@3/swagger-ui-bundle.js",
     swagger_css_url: str = "https://cdn.jsdelivr.net/npm/swagger-ui-dist@3/swagger-ui.css",
     swagger_favicon_url: str = "https://fastapi.tiangolo.com/img/favicon.png",
     home_url: str,
 ) -> HTMLResponse:
-
     html = f"""
 <!DOCTYPE html>
     <html>
     <head>
     <link type="text/css" rel="stylesheet" href="{swagger_css_url}">
     <link rel="shortcut icon" href="{swagger_favicon_url}">
     <link rel="stylesheet" type="text/css" href="static/css/styles.css">
```

### Comparing `fastapitableau-1.1.1/fastapitableau/pages.py` & `fastapitableau-1.1.2/fastapitableau/pages.py`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/routing.py` & `fastapitableau-1.1.2/fastapitableau/routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             _request = Request(request.scope, _receive)
 
             return await original_route_handler(_request)
 
         return custom_route_handler
 
     async def ensure_request_body(
-        self, body: Dict, scope: MutableMapping = None
+        self, body: Dict, scope: Optional[MutableMapping] = None
     ) -> Dict:
         # Here, we only want to operate on Tableau requests. We have a few options.
         # 1. Duck typing, which is what the main branch does right now. It checks to see if this a dict and contains the keys "script" and "data".
         # 2. Validate. Try to process the body with FastAPI's args and see if it works. If it doesn't, try this method.
         # 3. Use headers.
         body_will_validate = await self.body_will_validate(body)
         if body_will_validate:
```

### Comparing `fastapitableau-1.1.1/fastapitableau/rstudio_connect.py` & `fastapitableau-1.1.2/fastapitableau/rstudio_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         messages = "\n\n---\n\n".join(message_list)
         return messages
 
     try:
         # Call RStudio Connect API to get server settings
         use_http = environ.get("FASTAPITABLEAU_USE_HTTP", "False").title() == "True"
         if use_http:
-            connect_server = urlparse(connect_server)._replace(scheme="http").geturl()  # type: ignore[arg-type]
+            connect_server = urlparse(connect_server)._replace(scheme="http").geturl()  # type: ignore[arg-type, assignment]
         settings_url = str(connect_server) + "__api__/server_settings"
         headers = {"Authorization": "Key " + str(connect_api_key)}
         response = requests.get(settings_url, headers=headers, verify=not use_http)
     except Exception as e:
         logger.warning(
             "Unable to access RStudio Connect settings API due to error: %s", e
         )
```

### Comparing `fastapitableau-1.1.1/fastapitableau/statics/css/styles.css` & `fastapitableau-1.1.2/fastapitableau/statics/css/styles.css`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/templates/index.html` & `fastapitableau-1.1.2/fastapitableau/templates/index.html`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/templates/param_table.html` & `fastapitableau-1.1.2/fastapitableau/templates/param_table.html`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/templates/setup_tableau.html` & `fastapitableau-1.1.2/fastapitableau/templates/setup_tableau.html`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/templates/tableau_usage.html` & `fastapitableau-1.1.2/fastapitableau/templates/tableau_usage.html`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/templates/user_guide.html` & `fastapitableau-1.1.2/fastapitableau/templates/user_guide.html`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/user_guide.py` & `fastapitableau-1.1.2/fastapitableau/user_guide.py`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau/utils.py` & `fastapitableau-1.1.2/fastapitableau/utils.py`

 * *Files identical despite different names*

### Comparing `fastapitableau-1.1.1/fastapitableau.egg-info/PKG-INFO` & `fastapitableau-1.1.2/fastapitableau.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fastapitableau
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package for writing FastAPI apps that you can call from Tableau.
 Home-page: https://github.com/rstudio/fastapitableau
 Author: Toph Allen, James Blair, Bill Sager
 Author-email: toph@rstudio.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -160,9 +159,7 @@
 
 - You must turn off "Aggregate Measures" under the "Analysis" menu for Tableau to pass the correct values to the extension. If this setting is on, Tableau will send aggregated data to the extension, which may cause inaccuracies in computations.
 - With this value off, calculated fields don't allow you to pass raw values directly to an extension. Those values must be wrapped in an aggregating function. Since we've turned "Aggregate Measures" off, these functions won't actually aggregate the data. We've had success using `ATTR([VALUE_NAME])`.
 
 ## Debug logging
 
 To enable verbose debug logging, set the environment variable `FASTAPITABLEAU_LOG_LEVEL` to `DEBUG`.
-
-
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: fastapitableau Version: 1.1.1 Summary: A Python
+Metadata-Version: 2.1 Name: fastapitableau Version: 1.1.2 Summary: A Python
 package for writing FastAPI apps that you can call from Tableau. Home-page:
 https://github.com/rstudio/fastapitableau Author: Toph Allen, James Blair, Bill
-Sager Author-email: toph@rstudio.com License: MIT Platform: UNKNOWN Classifier:
-Environment :: Web Environment Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3.7 Classifier: Topic :: Internet :: WWW/HTTP
-:: Dynamic Content Classifier: Topic :: Software Development :: Libraries ::
-Python Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: test
+Sager Author-email: toph@rstudio.com License: MIT Classifier: Environment ::
+Web Environment Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3.7 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+test
                                [FastAPI Tableau]
                          [Coverage] [Package_version]
 # FastAPI Tableau --- **Documentation**: [https://rstudio.github.io/
 fastapitableau](https://rstudio.github.io/fastapitableau) **Source Code**:
 [https://github.com/rstudio/fastapitableau](https://github.com/rstudio/
 fastapitableau) --- FastAPI Tableau lets you call external Python code from
 Tableau workbooks via [Tableau Analytics Extensions](https://tableau.github.io/
```

### Comparing `fastapitableau-1.1.1/setup.cfg` & `fastapitableau-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fastapitableau
-version = 1.1.1
+version = 1.1.2
 url = https://github.com/rstudio/fastapitableau
 license = MIT
 license_files = LICENSE.txt
 author = Toph Allen, James Blair, Bill Sager
 author_email = toph@rstudio.com
 description = A Python package for writing FastAPI apps that you can call from Tableau.
 long_description = file:README.md
@@ -17,15 +17,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3.7
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 install_requires = 
-	fastapi
+	fastapi <=0.88.0
 	aiofiles
 	commonmark
 	requests
 	jinja2
 setup_requires = setuptools
 packages = fastapitableau
 python_requires = >=3.7
```

