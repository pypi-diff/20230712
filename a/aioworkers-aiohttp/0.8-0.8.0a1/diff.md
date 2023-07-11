# Comparing `tmp/aioworkers_aiohttp-0.8.tar.gz` & `tmp/aioworkers_aiohttp-0.8.0a1.tar.gz`

## Comparing `aioworkers_aiohttp-0.8.tar` & `aioworkers_aiohttp-0.8.0a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/aioworkers_aiohttp/__init__.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/aioworkers_aiohttp/abc.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/aioworkers_aiohttp/app.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/aioworkers_aiohttp/plugin.ini
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/aioworkers_aiohttp/router.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/aioworkers_aiohttp/server.py
--rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/aioworkers_aiohttp/storage.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/aioworkers_aiohttp/supervisor.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/LICENSE
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/README.rst
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/pyproject.toml
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8/PKG-INFO
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/abc.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/app.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/plugin.ini
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/router.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/server.py
+-rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/storage.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/supervisor.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/LICENSE
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/README.rst
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/PKG-INFO
```

### Comparing `aioworkers_aiohttp-0.8/aioworkers_aiohttp/__init__.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict, Iterable, Tuple
 
 from aioworkers.core.plugin import Plugin
 
 from .server import WebServer
 
 
-__version__ = "0.8"
+__version__ = "0.8.0a1"
 
 BASE = Path(__file__).parent
 
 
 class plugin(Plugin):
     configs = (BASE / "plugin.ini",)
```

### Comparing `aioworkers_aiohttp-0.8/aioworkers_aiohttp/abc.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/abc.py`

 * *Files identical despite different names*

### Comparing `aioworkers_aiohttp-0.8/aioworkers_aiohttp/app.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/app.py`

 * *Files identical despite different names*

### Comparing `aioworkers_aiohttp-0.8/aioworkers_aiohttp/router.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/router.py`

 * *Files identical despite different names*

### Comparing `aioworkers_aiohttp-0.8/aioworkers_aiohttp/server.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/server.py`

 * *Files identical despite different names*

### Comparing `aioworkers_aiohttp-0.8/aioworkers_aiohttp/storage.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/storage.py`

 * *Files identical despite different names*

### Comparing `aioworkers_aiohttp-0.8/aioworkers_aiohttp/supervisor.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/supervisor.py`

 * *Files identical despite different names*

### Comparing `aioworkers_aiohttp-0.8/.gitignore` & `aioworkers_aiohttp-0.8.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `aioworkers_aiohttp-0.8/LICENSE` & `aioworkers_aiohttp-0.8.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioworkers_aiohttp-0.8/README.rst` & `aioworkers_aiohttp-0.8.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `aioworkers_aiohttp-0.8/pyproject.toml` & `aioworkers_aiohttp-0.8.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,26 +35,26 @@
     "aiohttp-apiset>=0.9.15",
     "aiohttp>=3.8",
     "aioworkers>0.20",
 ]
 [project.optional-dependencies]
 dev-test = [
     "aioworkers==0.21.1",
-    "aiohttp-apiset==0.9.16",
+    "aiohttp-apiset==0.9.15",
     "coverage[toml]==7.2.7",
-    "pytest==7.4.0",
+    "pytest==7.3.2",
     "pytest-aioworkers[aiohttp]==0.4",
     "pytest-mock==3.11.1",
     "pyyaml==6.0",
 ]
 dev-lint = [
-    "ruff==0.0.277",
+    "ruff==0.0.272",
     "isort==5.12.0",
-    "black==23.7.0",
-    "mypy==1.4.1",
+    "black==23.3.0",
+    "mypy==1.3.0",
 ]
 
 [project.entry-points.aioworkers]
 aiohttp = "aioworkers_aiohttp:plugin"
 
 [project.urls]
 Homepage = "https://github.com/aioworkers/aioworkers-aiohttp"
```

### Comparing `aioworkers_aiohttp-0.8/PKG-INFO` & `aioworkers_aiohttp-0.8.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioworkers-aiohttp
-Version: 0.8
+Version: 0.8.0a1
 Summary: Integrations aioworkers with aiohttp
 Project-URL: Homepage, https://github.com/aioworkers/aioworkers-aiohttp
 Project-URL: Documentation, https://github.com/aioworkers/aioworkers-aiohttp#readme
 Project-URL: Issues, https://github.com/aioworkers/aioworkers-aiohttp/issues
 Project-URL: Source, https://github.com/aioworkers/aioworkers-aiohttp
 Author-email: Alexander Malev <yttrium@somedev.ru>
 License-Expression: Apache-2.0
@@ -24,25 +24,25 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: aiohttp-apiset>=0.9.15
 Requires-Dist: aiohttp>=3.8
 Requires-Dist: aioworkers>0.20
 Provides-Extra: dev-lint
-Requires-Dist: black==23.7.0; extra == 'dev-lint'
+Requires-Dist: black==23.3.0; extra == 'dev-lint'
 Requires-Dist: isort==5.12.0; extra == 'dev-lint'
-Requires-Dist: mypy==1.4.1; extra == 'dev-lint'
-Requires-Dist: ruff==0.0.277; extra == 'dev-lint'
+Requires-Dist: mypy==1.3.0; extra == 'dev-lint'
+Requires-Dist: ruff==0.0.272; extra == 'dev-lint'
 Provides-Extra: dev-test
-Requires-Dist: aiohttp-apiset==0.9.16; extra == 'dev-test'
+Requires-Dist: aiohttp-apiset==0.9.15; extra == 'dev-test'
 Requires-Dist: aioworkers==0.21.1; extra == 'dev-test'
 Requires-Dist: coverage[toml]==7.2.7; extra == 'dev-test'
 Requires-Dist: pytest-aioworkers[aiohttp]==0.4; extra == 'dev-test'
 Requires-Dist: pytest-mock==3.11.1; extra == 'dev-test'
-Requires-Dist: pytest==7.4.0; extra == 'dev-test'
+Requires-Dist: pytest==7.3.2; extra == 'dev-test'
 Requires-Dist: pyyaml==6.0; extra == 'dev-test'
 Description-Content-Type: text/x-rst
 
 aioworkers-aiohttp
 ==================
 
 The package to integration aioworkers with aiohttp
```

