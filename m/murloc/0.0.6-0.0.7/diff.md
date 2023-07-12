# Comparing `tmp/murloc-0.0.6.tar.gz` & `tmp/murloc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murloc-0.0.6.tar", last modified: Wed Jul 12 02:29:44 2023, max compression
+gzip compressed data, was "murloc-0.0.7.tar", last modified: Wed Jul 12 02:37:41 2023, max compression
```

## Comparing `murloc-0.0.6.tar` & `murloc-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-12 02:29:44.634876 murloc-0.0.6/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-07-11 01:36:26.000000 murloc-0.0.6/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     1171 2023-07-12 02:29:44.634876 murloc-0.0.6/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     3722 2023-07-11 01:36:26.000000 murloc-0.0.6/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-12 02:29:44.633876 murloc-0.0.6/murloc/
--rw-rw-r--   0 chris     (1000) chris     (1000)      841 2023-07-12 02:06:09.000000 murloc-0.0.6/murloc/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2967 2023-07-12 02:04:15.000000 murloc-0.0.6/murloc/murloc.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-12 02:29:44.634876 murloc-0.0.6/murloc.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1171 2023-07-12 02:29:44.000000 murloc-0.0.6/murloc.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-07-12 02:29:44.000000 murloc-0.0.6/murloc.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-12 02:29:44.000000 murloc-0.0.6/murloc.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-07-12 02:29:44.000000 murloc-0.0.6/murloc.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-07-12 02:29:44.635876 murloc-0.0.6/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      527 2023-07-12 02:29:39.000000 murloc-0.0.6/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-12 02:37:41.441289 murloc-0.0.7/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-07-11 01:36:26.000000 murloc-0.0.7/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1214 2023-07-12 02:37:41.441289 murloc-0.0.7/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3722 2023-07-11 01:36:26.000000 murloc-0.0.7/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-12 02:37:41.440289 murloc-0.0.7/murloc/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      884 2023-07-12 02:36:55.000000 murloc-0.0.7/murloc/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2973 2023-07-12 02:37:34.000000 murloc-0.0.7/murloc/murloc.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-12 02:37:41.441289 murloc-0.0.7/murloc.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1214 2023-07-12 02:37:41.000000 murloc-0.0.7/murloc.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-07-12 02:37:41.000000 murloc-0.0.7/murloc.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-12 02:37:41.000000 murloc-0.0.7/murloc.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-07-12 02:37:41.000000 murloc-0.0.7/murloc.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-07-12 02:37:41.441289 murloc-0.0.7/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      527 2023-07-12 02:37:18.000000 murloc-0.0.7/setup.py
```

### Comparing `murloc-0.0.6/LICENSE` & `murloc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `murloc-0.0.6/PKG-INFO` & `murloc-0.0.7/murloc/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,50 @@
-Metadata-Version: 2.1
-Name: murloc
-Version: 0.0.6
-Summary: Extensible API server
-Home-page: 
-Author: Chris Varga
-Author-email: 
-Keywords: extensible api server
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
+"""
 Murloc is an extensible API server.
 
-To define API methods, use the route decorator like so:
+To define API methods, use the `route` decorator like so:
 
 ```python
-# file: main.py
+# main.py
 from murloc import Murloc
 
 app = Murloc()
 
 @app.route("/hello")
 def hello_world():
     return "hello, world!"
 
 @app.route("/echo")
 def echo_data(data):
     return data
 ```
 
-You can also specify `methods` directly as a dict() during Murloc initialization:
+You can also specify `methods` directly as a `dict()` during Murloc initialization:
 
 ```python
-# file: main.py
+# main.py
 from murloc import Murloc
 
 def hello_world():
     return "hello, world!"
 
 def echo_data(data):
     return data
 
 app = Murloc(methods={"/hello": hello_world, "/echo": echo_data})
 ```
 
-Run murloc with uvicorn like so:
+Run the murloc server with uvicorn like so:
 
+```bash
 $ uvicorn main:app
+```
 
 Or, with gunicorn (must support ASGI) like so:
 
+```bash
 $ gunicorn main:app --worker-class uvicorn.workers.UvicornWorker
+```
 
-Note: Assumes main.py and the Murloc variable `app`.
+> Note: These examples assume main.py and the Murloc variable `app`.
+"""
+from .murloc import Murloc
```

### Comparing `murloc-0.0.6/README.md` & `murloc-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `murloc-0.0.6/murloc/murloc.py` & `murloc-0.0.7/murloc/murloc.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         body = await read_body(receive)
         res = await handle_request(scope["path"], body.decode())
         await send(
             {
                 "type": "http.response.start",
                 "status": 200,
                 "headers": [
-                    (b"content-type", b"text/plain"),
+                    (b"content-type", b"application/json"),
                 ],
             }
         )
         await send(
             {
                 "type": "http.response.body",
                 "body": str(res).encode(),
```

### Comparing `murloc-0.0.6/setup.py` & `murloc-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import murloc
 from setuptools import setup, find_packages
 
 setup(
     name="murloc",
-    version="0.0.6",
+    version="0.0.7",
     author="Chris Varga",
     author_email="",
     description="Extensible API server",
     long_description=murloc.__doc__,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
```

