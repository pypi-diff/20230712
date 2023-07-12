# Comparing `tmp/fastapi-cors-0.0.5.tar.gz` & `tmp/fastapi-cors-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-cors-0.0.5.tar", last modified: Thu Jul  6 15:30:07 2023, max compression
+gzip compressed data, was "fastapi-cors-0.0.6.tar", last modified: Wed Jul 12 17:16:59 2023, max compression
```

## Comparing `fastapi-cors-0.0.5.tar` & `fastapi-cors-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/LICENSE
--rw-r--r--   0        0        0     2833 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/README.md
--rw-r--r--   0        0        0       55 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/fastapi_cors/__init__.py
--rw-r--r--   0        0        0      813 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/fastapi_cors/env.py
--rw-r--r--   0        0        0     2056 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/fastapi_cors/main.py
--rw-r--r--   0        0        0     2249 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 fastapi-cors-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-12 17:16:27.760172 fastapi-cors-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2833 2023-07-12 17:16:27.760172 fastapi-cors-0.0.6/README.md
+-rw-r--r--   0        0        0       55 2023-07-12 17:16:27.760172 fastapi-cors-0.0.6/fastapi_cors/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-12 17:16:27.760172 fastapi-cors-0.0.6/fastapi_cors/env.py
+-rw-r--r--   0        0        0     2056 2023-07-12 17:16:27.760172 fastapi-cors-0.0.6/fastapi_cors/main.py
+-rw-r--r--   0        0        0     2770 2023-07-12 17:16:27.760172 fastapi-cors-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 fastapi-cors-0.0.6/PKG-INFO
```

### Comparing `fastapi-cors-0.0.5/LICENSE` & `fastapi-cors-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.5/README.md` & `fastapi-cors-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.5/fastapi_cors/env.py` & `fastapi-cors-0.0.6/fastapi_cors/env.py`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.5/fastapi_cors/main.py` & `fastapi-cors-0.0.6/fastapi_cors/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.5/pyproject.toml` & `fastapi-cors-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 [project]
 name = "fastapi_cors"
 description = "Simple env support of CORS settings for Fastapi applications"
 authors = [
     { name = "Ian Cleary", email = "github@iancleary.me" },
 ]
 dynamic = []
-requires-python = ">=3.11"
+requires-python = ">=3.8"
 dependencies = [
     "environs>=9.5.0",
     "fastapi>=0.99.1",
 ]
 readme = "README.md"
-keywords = [
-    "cors",
-    "python",
-    "fastapi",
-    "environs",
-]
 classifiers = [
-    "Topic :: Software Development :: Code Generators",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: System Administrators",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python",
+    "Topic :: Internet",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Software Development",
+    "Typing :: Typed",
+    "Environment :: Web Environment",
+    "Framework :: FastAPI",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
+    "Topic :: Internet :: WWW/HTTP",
 ]
-version = "0.0.5"
+version = "0.0.6"
 
 [project.license]
 text = "MIT"
 
-[project.urls]
-Homepage = "https://github.com/iancleary/fastapi-cors"
-Repository = "https://github.com/iancleary/fastapi-cors"
-Documentation = "https://github.com/iancleary/fastapi-cors"
-
 [tool.pdm.version]
 source = "scm"
 write_to = "fastapi_cors/VERSION"
 write_template = "__version__ = '{}'"
 
 [tool.pdm.build]
 includes = [
@@ -119,10 +126,10 @@
 ignore_missing_imports = true
 exclude = [
     "docs/",
 ]
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-pep517>=1.0",
 ]
 build-backend = "pdm.pep517.api"
```

