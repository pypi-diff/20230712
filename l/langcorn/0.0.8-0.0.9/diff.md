# Comparing `tmp/langcorn-0.0.8.tar.gz` & `tmp/langcorn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcorn-0.0.8.tar", max compression
+gzip compressed data, was "langcorn-0.0.9.tar", max compression
```

## Comparing `langcorn-0.0.8.tar` & `langcorn-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1088 2023-05-15 11:37:09.280660 langcorn-0.0.8/LICENSE
--rw-r--r--   0        0        0     7377 2023-05-15 11:37:09.280660 langcorn-0.0.8/Readme.md
--rw-r--r--   0        0        0       77 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/__init__.py
--rw-r--r--   0        0        0      489 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/__main__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/server/__init__.py
--rw-r--r--   0        0        0     4648 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/server/api.py
--rw-r--r--   0        0        0      999 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/server/test_api.py
--rw-r--r--   0        0        0      981 2023-05-15 11:37:09.280660 langcorn-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     8388 1970-01-01 00:00:00.000000 langcorn-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-15 11:46:53.076266 langcorn-0.0.9/LICENSE
+-rw-r--r--   0        0        0     7377 2023-05-15 11:46:53.076266 langcorn-0.0.9/Readme.md
+-rw-r--r--   0        0        0       77 2023-05-15 11:46:53.076266 langcorn-0.0.9/langcorn/__init__.py
+-rw-r--r--   0        0        0      484 2023-05-15 11:46:53.076266 langcorn-0.0.9/langcorn/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:46:53.076266 langcorn-0.0.9/langcorn/server/__init__.py
+-rw-r--r--   0        0        0     4643 2023-05-15 11:46:53.076266 langcorn-0.0.9/langcorn/server/api.py
+-rw-r--r--   0        0        0      999 2023-05-15 11:46:53.076266 langcorn-0.0.9/langcorn/server/test_api.py
+-rw-r--r--   0        0        0      981 2023-05-15 11:46:53.076266 langcorn-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8388 1970-01-01 00:00:00.000000 langcorn-0.0.9/PKG-INFO
```

### Comparing `langcorn-0.0.8/LICENSE` & `langcorn-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.8/Readme.md` & `langcorn-0.0.9/Readme.md`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.8/langcorn/server/api.py` & `langcorn-0.0.9/langcorn/server/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         return LangResponse(output=output, error="", memory=memory)
 
     return handler
 
 
 def create_service(*lc_apps, auth_token: str = "", app: FastAPI = None):
     # Make local modules discoverable
-    sys.path.append(os.path.dirname(__file__))
+    sys.path.append(os.path.dirname("."))
     logger.info("Creating service")
     app = app or FastAPI()
     endpoints = ["/docs"]
 
     _authenticate_or_401 = Depends(authenticate_or_401(auth_token=auth_token))
     if lc_apps and isinstance(import_from_string(lc_apps[0]), FastAPI):
         raise RuntimeError(
```

### Comparing `langcorn-0.0.8/langcorn/server/test_api.py` & `langcorn-0.0.9/langcorn/server/test_api.py`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.8/pyproject.toml` & `langcorn-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langcorn"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Python package creating rest api interface for LangChain"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = [
     "Alexander Miasoiedov <msoedov@gmail.com>",
 ]
 repository = "https://github.com/msoedov/langcorn"
 license = "MIT"
```

### Comparing `langcorn-0.0.8/PKG-INFO` & `langcorn-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langcorn
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package creating rest api interface for LangChain
 Home-page: https://github.com/msoedov/langcorn
 License: MIT
 Keywords: nlp,langchain,openai,gpt,fastapi
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
```

