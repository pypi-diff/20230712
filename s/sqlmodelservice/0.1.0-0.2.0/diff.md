# Comparing `tmp/sqlmodelservice-0.1.0.tar.gz` & `tmp/sqlmodelservice-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodelservice-0.1.0.tar", max compression
+gzip compressed data, was "sqlmodelservice-0.2.0.tar", max compression
```

## Comparing `sqlmodelservice-0.1.0.tar` & `sqlmodelservice-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-07-12 09:20:54.866634 sqlmodelservice-0.1.0/LICENSE
--rw-r--r--   0        0        0      576 2023-07-12 11:17:33.572050 sqlmodelservice-0.1.0/README.md
--rw-r--r--   0        0        0     2262 2023-07-12 09:57:16.779986 sqlmodelservice-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 09:26:40.662529 sqlmodelservice-0.1.0/sqlmodelservice/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 09:26:53.250669 sqlmodelservice-0.1.0/sqlmodelservice/py.typed
--rw-r--r--   0        0        0     9318 2023-07-12 09:52:04.659296 sqlmodelservice-0.1.0/sqlmodelservice/service.py
--rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 sqlmodelservice-0.1.0/setup.py
--rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 sqlmodelservice-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-12 09:20:54.866634 sqlmodelservice-0.2.0/LICENSE
+-rw-r--r--   0        0        0      576 2023-07-12 11:17:33.572050 sqlmodelservice-0.2.0/README.md
+-rw-r--r--   0        0        0     2262 2023-07-12 11:21:36.700418 sqlmodelservice-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-07-12 11:21:21.352388 sqlmodelservice-0.2.0/sqlmodelservice/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:26:53.250669 sqlmodelservice-0.2.0/sqlmodelservice/py.typed
+-rw-r--r--   0        0        0     9318 2023-07-12 09:52:04.659296 sqlmodelservice-0.2.0/sqlmodelservice/service.py
+-rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 sqlmodelservice-0.2.0/setup.py
+-rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 sqlmodelservice-0.2.0/PKG-INFO
```

### Comparing `sqlmodelservice-0.1.0/LICENSE` & `sqlmodelservice-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodelservice-0.1.0/README.md` & `sqlmodelservice-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlmodelservice-0.1.0/pyproject.toml` & `sqlmodelservice-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [project.urls]
 Homepage = "https://github.com/volfpeter/sqlmodelservice"
 Documentation = "https://volfpeter.github.io/sqlmodelservice"
 
 [tool.poetry]
 name = "sqlmodelservice"
-version = "0.1.0"
+version = "0.2.0"
 description = "A generic service layer on top of SQLModel for conveniently creating APIs with frameworks like FastAPI."
 authors = ["Peter Volf <do.volfp@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sqlmodelservice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sqlmodelservice-0.1.0/sqlmodelservice/service.py` & `sqlmodelservice-0.2.0/sqlmodelservice/service.py`

 * *Files identical despite different names*

### Comparing `sqlmodelservice-0.1.0/setup.py` & `sqlmodelservice-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['sqlmodel>=0.0.8,<0.0.9']
 
 setup_kwargs = {
     'name': 'sqlmodelservice',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'A generic service layer on top of SQLModel for conveniently creating APIs with frameworks like FastAPI.',
     'long_description': '# SQLModelService\n\n`SQLModelService` is a generic service layer on top of `SQLModel` for conveniently creating APIs with frameworks like [FastAPI](https://fastapi.tiangolo.com/).\n\n## Installation\n\nThe library is available on PyPI and can be installed with:\n\n```console\n$ pip install sqlmodelservice\n```\n\n## Dependencies\n\nThe only direct dependency of the project -- as the name suggests -- is `SQLModel`.\n\n## Contributing\n\nContributions are welcome.\n\n## License\n\nThe library is open-sourced under the conditions of the [MIT license](https://choosealicense.com/licenses/mit/).\n',
     'author': 'Peter Volf',
     'author_email': 'do.volfp@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `sqlmodelservice-0.1.0/PKG-INFO` & `sqlmodelservice-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodelservice
-Version: 0.1.0
+Version: 0.2.0
 Summary: A generic service layer on top of SQLModel for conveniently creating APIs with frameworks like FastAPI.
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

