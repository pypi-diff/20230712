# Comparing `tmp/resource-id-1.0.0.tar.gz` & `tmp/resource-id-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resource-id-1.0.0.tar", last modified: Wed Aug  3 21:55:04 2022, max compression
+gzip compressed data, was "resource-id-1.1.1.tar", last modified: Wed Jul 12 15:57:00 2023, max compression
```

## Comparing `resource-id-1.0.0.tar` & `resource-id-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2022-08-03 21:55:04.311060 resource-id-1.0.0/
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2022-08-03 21:55:04.307779 resource-id-1.0.0/.github/
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2022-08-03 21:55:04.309710 resource-id-1.0.0/.github/workflows/
--rw-r--r--   0 charles    (501) staff       (20)      798 2022-08-03 19:18:47.000000 resource-id-1.0.0/.github/workflows/tox.yml
--rw-r--r--   0 charles    (501) staff       (20)       68 2022-08-03 21:40:24.000000 resource-id-1.0.0/.gitignore
--rw-r--r--   0 charles    (501) staff       (20)       43 2022-08-03 21:42:33.000000 resource-id-1.0.0/CHANGELOG.md
--rw-r--r--   0 charles    (501) staff       (20)     1055 2022-08-03 21:44:13.000000 resource-id-1.0.0/LICENSE.txt
--rw-r--r--   0 charles    (501) staff       (20)       20 2022-08-03 21:44:57.000000 resource-id-1.0.0/MANIFEST.in
--rw-r--r--   0 charles    (501) staff       (20)      929 2022-08-03 21:55:04.311169 resource-id-1.0.0/PKG-INFO
--rw-r--r--   0 charles    (501) staff       (20)     2079 2022-08-03 20:10:40.000000 resource-id-1.0.0/README.md
--rw-r--r--   0 charles    (501) staff       (20)      184 2022-08-03 16:07:41.000000 resource-id-1.0.0/pyproject.toml
--rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 15:42:00.000000 resource-id-1.0.0/pytest.ini
--rw-r--r--   0 charles    (501) staff       (20)      114 2022-08-03 21:39:13.000000 resource-id-1.0.0/requirements.txt
--rw-r--r--   0 charles    (501) staff       (20)     1081 2022-08-03 21:55:04.311570 resource-id-1.0.0/setup.cfg
--rw-r--r--   0 charles    (501) staff       (20)       38 2022-08-03 16:05:04.000000 resource-id-1.0.0/setup.py
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2022-08-03 21:55:04.307954 resource-id-1.0.0/src/
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2022-08-03 21:55:04.310037 resource-id-1.0.0/src/resource_id/
--rw-r--r--   0 charles    (501) staff       (20)      435 2022-08-03 18:32:10.000000 resource-id-1.0.0/src/resource_id/__init__.py
--rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 19:57:16.000000 resource-id-1.0.0/src/resource_id/py.typed
--rw-r--r--   0 charles    (501) staff       (20)     3397 2022-08-03 21:24:34.000000 resource-id-1.0.0/src/resource_id/resource_id.py
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2022-08-03 21:55:04.310674 resource-id-1.0.0/src/resource_id.egg-info/
--rw-r--r--   0 charles    (501) staff       (20)      929 2022-08-03 21:55:04.000000 resource-id-1.0.0/src/resource_id.egg-info/PKG-INFO
--rw-r--r--   0 charles    (501) staff       (20)      475 2022-08-03 21:55:04.000000 resource-id-1.0.0/src/resource_id.egg-info/SOURCES.txt
--rw-r--r--   0 charles    (501) staff       (20)        1 2022-08-03 21:55:04.000000 resource-id-1.0.0/src/resource_id.egg-info/dependency_links.txt
--rw-r--r--   0 charles    (501) staff       (20)       92 2022-08-03 21:55:04.000000 resource-id-1.0.0/src/resource_id.egg-info/requires.txt
--rw-r--r--   0 charles    (501) staff       (20)       12 2022-08-03 21:55:04.000000 resource-id-1.0.0/src/resource_id.egg-info/top_level.txt
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2022-08-03 21:55:04.310927 resource-id-1.0.0/tests/
--rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 15:44:50.000000 resource-id-1.0.0/tests/__init__.py
--rw-r--r--   0 charles    (501) staff       (20)     1576 2022-08-03 21:23:34.000000 resource-id-1.0.0/tests/test_resource_id.py
--rw-r--r--   0 charles    (501) staff       (20)      304 2022-08-03 20:06:17.000000 resource-id-1.0.0/tox.ini
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.396359 resource-id-1.1.1/
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.392509 resource-id-1.1.1/.github/
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.394767 resource-id-1.1.1/.github/workflows/
+-rw-r--r--   0 charles    (501) staff       (20)      798 2022-08-03 19:18:47.000000 resource-id-1.1.1/.github/workflows/tox.yml
+-rw-r--r--   0 charles    (501) staff       (20)       68 2022-08-03 21:40:24.000000 resource-id-1.1.1/.gitignore
+-rw-r--r--   0 charles    (501) staff       (20)      246 2023-07-12 15:41:47.000000 resource-id-1.1.1/CHANGELOG.md
+-rw-r--r--   0 charles    (501) staff       (20)     1055 2022-08-03 21:44:13.000000 resource-id-1.1.1/LICENSE.txt
+-rw-r--r--   0 charles    (501) staff       (20)       20 2022-08-03 21:44:57.000000 resource-id-1.1.1/MANIFEST.in
+-rw-r--r--   0 charles    (501) staff       (20)      929 2023-07-12 15:57:00.396460 resource-id-1.1.1/PKG-INFO
+-rw-r--r--   0 charles    (501) staff       (20)     2166 2023-07-12 15:52:32.000000 resource-id-1.1.1/README.md
+-rw-r--r--   0 charles    (501) staff       (20)      184 2022-08-03 16:07:41.000000 resource-id-1.1.1/pyproject.toml
+-rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 15:42:00.000000 resource-id-1.1.1/pytest.ini
+-rw-r--r--   0 charles    (501) staff       (20)      114 2022-08-03 21:39:13.000000 resource-id-1.1.1/requirements.txt
+-rw-r--r--   0 charles    (501) staff       (20)     1051 2023-07-12 15:57:00.396823 resource-id-1.1.1/setup.cfg
+-rw-r--r--   0 charles    (501) staff       (20)       38 2022-08-03 16:05:04.000000 resource-id-1.1.1/setup.py
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.392991 resource-id-1.1.1/src/
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.395197 resource-id-1.1.1/src/resource_id/
+-rw-r--r--   0 charles    (501) staff       (20)      435 2022-08-03 18:32:10.000000 resource-id-1.1.1/src/resource_id/__init__.py
+-rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 19:57:16.000000 resource-id-1.1.1/src/resource_id/py.typed
+-rw-r--r--   0 charles    (501) staff       (20)     4498 2023-07-12 15:26:10.000000 resource-id-1.1.1/src/resource_id/resource_id.py
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.395947 resource-id-1.1.1/src/resource_id.egg-info/
+-rw-r--r--   0 charles    (501) staff       (20)      929 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/PKG-INFO
+-rw-r--r--   0 charles    (501) staff       (20)      475 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/SOURCES.txt
+-rw-r--r--   0 charles    (501) staff       (20)        1 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/dependency_links.txt
+-rw-r--r--   0 charles    (501) staff       (20)       57 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/requires.txt
+-rw-r--r--   0 charles    (501) staff       (20)       12 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/top_level.txt
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.396221 resource-id-1.1.1/tests/
+-rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 15:44:50.000000 resource-id-1.1.1/tests/__init__.py
+-rw-r--r--   0 charles    (501) staff       (20)     2434 2023-07-12 14:30:12.000000 resource-id-1.1.1/tests/test_resource_id.py
+-rw-r--r--   0 charles    (501) staff       (20)      315 2023-07-12 15:31:01.000000 resource-id-1.1.1/tox.ini
```

### Comparing `resource-id-1.0.0/.github/workflows/tox.yml` & `resource-id-1.1.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `resource-id-1.0.0/LICENSE.txt` & `resource-id-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resource-id-1.0.0/PKG-INFO` & `resource-id-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-id
-Version: 1.0.0
+Version: 1.1.1
 Summary: Base62-encoded identifier.
 Home-page: https://github.com/declaresub/resource-id
 Author: Charles Yeomans
 Author-email: charles@declaresub.com
 License: MIT
 Keywords: identifier,url,base62
 Platform: any
```

### Comparing `resource-id-1.0.0/README.md` & `resource-id-1.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # ResourceId
 
 The resource-id package provides a ResourceId class implementing base62-encoded identifiers, suitable
 for URLs, URIs, and perhaps something else.
 
-ResourceId is written to work with [Pydantic](https://pydantic-docs.helpmanual.io), but does not depend on Pydantic.
+ResourceId is written to work with [Pydantic](https://pydantic-docs.helpmanual.io).
 In particular, it can be used with [FastAPI](https://fastapi.tiangolo.com) as a path parameter.
 
 ![tox](https://github.com/declaresub/resource-id/actions/workflows/tox.yml/badge.svg)
 
 
 ## Requirements
 
-Resource-id requires Python >= 3.7. For python <= 3.9, typing_extensions is required. For Python 3.7, 
-importlib-metadata is required.
+Resource-id requires Python >= 3.8. For python <= 3.9, typing_extensions is required.
+Version 1.1.0 adds support for pydantic 2, which in turn requires that pydantic be added 
+as a dependency.
 
 ## Installation
 
     pip install resource-id
 
 ## Usage
 
@@ -26,27 +27,29 @@
 
 Create a ResourceId:
 
     id = ResourceId(43)
     id1 = ResourceId('deadbeef')
     id2 = ResourceId(UUID(int=101))
 
+In fact a ResourceId can be created from any object that implements __int__,
+
 
 Create a URL path using a ResourceId:
 
     path = f"/api/foo/{ResourceId('deadbeef')}"
 
 Define a FastAPI request handler with a ResourceId:
 
     @app.get('/api/foo/{foo_id}')
     async def get_foo(foo_id: ResourceId):
         ...
 
 Here, FastAPI will validate the value of the path variable foo_id with Pydantic.  If validation fails, 
-FastAPI (unfortunately) returns 422 Unprocessable Entity.
+FastAPI returns 422 Unprocessable Entity.
 
     
 Convert a ResourceId to a UUID:
 
     res_id = ResourceId(43)
     id = res_id.uuid
```

### Comparing `resource-id-1.0.0/setup.cfg` & `resource-id-1.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 [options]
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	typing_extensions; python_version<"3.10"
-	importlib-metadata; python_version<"3.8"
+	pydantic<3
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = py.typed
```

### Comparing `resource-id-1.0.0/src/resource_id.egg-info/PKG-INFO` & `resource-id-1.1.1/src/resource_id.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-id
-Version: 1.0.0
+Version: 1.1.1
 Summary: Base62-encoded identifier.
 Home-page: https://github.com/declaresub/resource-id
 Author: Charles Yeomans
 Author-email: charles@declaresub.com
 License: MIT
 Keywords: identifier,url,base62
 Platform: any
```

