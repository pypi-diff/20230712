# Comparing `tmp/sixth-python-0.1.5.tar.gz` & `tmp/sixth-python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-python-0.1.5.tar", last modified: Mon Jul 10 13:05:25 2023, max compression
+gzip compressed data, was "dist/sixth-python-0.1.6.tar", last modified: Wed Jul 12 00:23:41 2023, max compression
```

## Comparing `sixth-python-0.1.5.tar` & `sixth-python-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/
--rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-10 13:05:25.000000 sixth-python-0.1.5/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.5/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-10 13:05:25.000000 sixth-python-0.1.5/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3760 2023-07-10 13:05:20.000000 sixth-python-0.1.5/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth/
--rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.5/sixth/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.5/sixth/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-10 11:42:02.000000 sixth-python-0.1.5/sixth/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.5/sixth/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-10 11:42:02.000000 sixth-python-0.1.5/sixth/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     7024 2023-07-10 12:10:24.000000 sixth-python-0.1.5/sixth/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.5/sixth/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      143 2023-07-09 17:50:41.000000 sixth-python-0.1.5/sixth/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)      978 2023-07-10 11:22:10.000000 sixth-python-0.1.5/sixth/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4246 2023-07-10 13:04:35.000000 sixth-python-0.1.5/sixth/sdk.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.5/sixth/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.5/sixth/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.5/sixth/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 00:23:41.000000 sixth-python-0.1.6/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-12 00:23:41.000000 sixth-python-0.1.6/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.6/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-12 00:23:41.000000 sixth-python-0.1.6/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3760 2023-07-12 00:23:06.000000 sixth-python-0.1.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth/
+-rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.6/sixth/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.6/sixth/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-11 23:56:33.000000 sixth-python-0.1.6/sixth/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.6/sixth/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-11 23:56:33.000000 sixth-python-0.1.6/sixth/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     8228 2023-07-12 00:22:18.000000 sixth-python-0.1.6/sixth/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.6/sixth/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      143 2023-07-09 17:50:41.000000 sixth-python-0.1.6/sixth/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)     1201 2023-07-11 23:10:12.000000 sixth-python-0.1.6/sixth/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4246 2023-07-11 23:56:33.000000 sixth-python-0.1.6/sixth/sdk.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.6/sixth/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.6/sixth/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.6/sixth/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-12 00:23:41.000000 sixth-python-0.1.6/sixth_python.egg-info/top_level.txt
```

### Comparing `sixth-python-0.1.5/PKG-INFO` & `sixth-python-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.1.5/README.md` & `sixth-python-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.5/setup.py` & `sixth-python-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Sixth offical python package'
 LONG_DESCRIPTION = '''
 # **Sixth**
 
 
 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
```

### Comparing `sixth-python-0.1.5/sixth/middlewares/encryption_middleware.py` & `sixth-python-0.1.6/sixth/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.5/sixth/middlewares/six_base_http_middleware.py` & `sixth-python-0.1.6/sixth/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.5/sixth/middlewares/six_independent_rate_limiter.py` & `sixth-python-0.1.6/sixth/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.5/sixth/middlewares/six_rate_limiter_middleware.py` & `sixth-python-0.1.6/sixth/middlewares/six_rate_limiter_middleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,25 +21,29 @@
     def __init__(self, app: ASGIApp, apikey: str, fastapi_app: FastAPI, project_config: schemas.ProjectConfig):
         super().__init__(app)
         self._config = project_config
         self._log_dict = {}
         self._app = app
         self._apikey = apikey
         self._route_last_updated = {}
+        self._rate_limit_logs_sent = {}
+        
         for route in fastapi_app.router.routes:
             if type(route.app )== FastAPI:
                 for new_route in route.app.routes:
                     path = "/v"+str(route.app.version)+new_route.path
                     edited_route = re.sub(r'\W+', '~', path)
                     self._log_dict[str(edited_route)] = {}
                     self._route_last_updated[str(edited_route)] = time.time()
+                    self._rate_limit_logs_sent[str(edited_route)] = 0
             else:
                 edited_route = re.sub(r'\W+', '~', route.path)
                 self._log_dict[str(edited_route)] = {}
                 self._route_last_updated[str(edited_route)] = time.time()
+                self._rate_limit_logs_sent[str(edited_route)] = 0
                 
 
     async def set_body(self, request: Request, body: bytes):
         async def receive() -> Message:
             return {'type': 'http.request', 'body': body}
         request._receive = receive
         
@@ -69,29 +73,50 @@
         string = string.replace(' ', "")
         string = string.replace('true,', "True,")
         string = string.replace(",true", "True,")
         string = string.replace('false,', "False,")
         string = string.replace(",false", "False,")
         out=ast.literal_eval(string)
         return out
+    
+    async def _send_logs(self, route: str, header, body, query)-> None:
+        timestamp = time.time()
+        last_log_sent = self._rate_limit_logs_sent[route]
+        if timestamp - last_log_sent > 10:
+            print("called from here")
+            requests.post("https://backend.withsix.co/slack/send_message_to_slack_user", json=schemas.SlackMessageSchema(
+                header=header, 
+                user_id=self._apikey, 
+                body=str(body), 
+                query_args=str(query), 
+                timestamp=timestamp, 
+                attack_type="No Rate Limit Attack", 
+                cwe_link="https://cwe.mitre.org/data/definitions/770.html", 
+                status="MITIGATED", 
+                learn_more_link="https://en.wikipedia.org/wiki/Rate_limiting"
+            ).dict())
+            self._rate_limit_logs_sent[route]=timestamp
+            
+
         
     async def dispatch(self,request: Request,call_next) -> None:
         host = request.client.host
         route = request.scope["path"]
         route = re.sub(r'\W+', '~', route)
         headers = request.headers
         query_params = request.query_params
         rate_limit_resp = None
         status_code = 200
+
         
         
         #fail safe if there is an internal server error our servers are currenly in maintnance
         try:
-            if time.time() - self._route_last_updated[route] >5:
-                #update rate limit details every 5 seconds
+            if time.time() - self._route_last_updated[route] >60:
+                #update rate limit details every 60 seconds
                 rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
                 self._route_last_updated[route] = time.time()
                 status_code = rate_limit_resp.status_code
             body = None
 
             try:
                 body = await request.body()
@@ -125,32 +150,33 @@
                                 preferred_id = host
                         
 
                         if self._is_rate_limit_reached(preferred_id, route): 
                             _response = await call_next(request)
                             return _response
                         else:
+                            await self._send_logs(route=route, header=headers, body=body, query=query_params)
                             temp_payload = rate_limit.error_payload.values()
                             final = {}
                             for c in temp_payload:
                                 for keys in c:
                                     if keys != "uid":
                                         final[keys] = c[keys]
                             output= final
                             headers = MutableHeaders(headers={"content-length": str(len(str(output).encode())), 'content-type': 'application/json'})
                             return Response(json.dumps(output), status_code=420, headers=headers)
                     else:
                        
                         _response = await call_next(request)
                         return _response
                 except Exception as e:
-                   
+                    print(e)
                     _response = await call_next(request)
                     return _response
             else:
                 #fail safe if there is an internal server error our servers are currenly in maintnance
                 _response = await call_next(request)
                 return _response
         except Exception as e:
-            
+            print(e)
             _response = await call_next(request)
             return _response
```

### Comparing `sixth-python-0.1.5/sixth/sdk.py` & `sixth-python-0.1.6/sixth/sdk.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.5/sixth/utils/encryption_utils.py` & `sixth-python-0.1.6/sixth/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.5/sixth/utils/time_utils.py` & `sixth-python-0.1.6/sixth/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.5/sixth_python.egg-info/PKG-INFO` & `sixth-python-0.1.6/sixth_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.1.5/sixth_python.egg-info/SOURCES.txt` & `sixth-python-0.1.6/sixth_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.5/sixth_python.egg-info/requires.txt` & `sixth-python-0.1.6/sixth_python.egg-info/requires.txt`

 * *Files identical despite different names*

