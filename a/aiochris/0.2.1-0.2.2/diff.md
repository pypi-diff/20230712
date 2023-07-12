# Comparing `tmp/aiochris-0.2.1.tar.gz` & `tmp/aiochris-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiochris-0.2.1.tar", max compression
+gzip compressed data, was "aiochris-0.2.2.tar", max compression
```

## Comparing `aiochris-0.2.1.tar` & `aiochris-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-07-07 17:16:46.450027 aiochris-0.2.1/LICENSE
--rw-r--r--   0        0        0     1738 2023-07-07 17:16:46.450027 aiochris-0.2.1/README.md
--rw-r--r--   0        0        0      574 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/__init__.py
--rw-r--r--   0        0        0     6243 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/admin.py
--rw-r--r--   0        0        0     1335 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/anon.py
--rw-r--r--   0        0        0     9627 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/authed.py
--rw-r--r--   0        0        0     3495 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/base.py
--rw-r--r--   0        0        0     1707 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/normal.py
--rw-r--r--   0        0        0     2284 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/examples.md
--rw-r--r--   0        0        0     4811 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/home.md
--rw-r--r--   0        0        0       97 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/collection_client.py
--rw-r--r--   0        0        0     4969 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/http.py
--rw-r--r--   0        0        0     4664 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/linked.py
--rw-r--r--   0        0        0     1450 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/metaprog.py
--rw-r--r--   0        0        0        0 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/__init__.py
--rw-r--r--   0        0        0     1638 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/collection_links.py
--rw-r--r--   0        0        0     2912 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/data.py
--rw-r--r--   0        0        0      644 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/enums.py
--rw-r--r--   0        0        0     5061 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/logged_in.py
--rw-r--r--   0        0        0      833 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/public.py
--rw-r--r--   0        0        0     3118 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/types.py
--rw-r--r--   0        0        0       31 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/util/__init__.py
--rw-r--r--   0        0        0      698 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/util/errors.py
--rw-r--r--   0        0        0     6920 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/util/search.py
--rw-r--r--   0        0        0      782 2023-07-07 17:16:46.450027 aiochris-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 aiochris-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 18:24:29.663271 aiochris-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1738 2023-07-12 18:24:29.663271 aiochris-0.2.2/README.md
+-rw-r--r--   0        0        0      574 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/__init__.py
+-rw-r--r--   0        0        0     6173 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/admin.py
+-rw-r--r--   0        0        0     1335 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/anon.py
+-rw-r--r--   0        0        0     9627 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/authed.py
+-rw-r--r--   0        0        0     3723 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/base.py
+-rw-r--r--   0        0        0     1707 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/client/normal.py
+-rw-r--r--   0        0        0     2284 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/examples.md
+-rw-r--r--   0        0        0     4811 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/home.md
+-rw-r--r--   0        0        0       97 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/collection_client.py
+-rw-r--r--   0        0        0     4969 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/http.py
+-rw-r--r--   0        0        0     4664 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/linked.py
+-rw-r--r--   0        0        0     1450 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/link/metaprog.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/__init__.py
+-rw-r--r--   0        0        0     1638 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/collection_links.py
+-rw-r--r--   0        0        0     2912 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/data.py
+-rw-r--r--   0        0        0      644 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/enums.py
+-rw-r--r--   0        0        0     5061 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/logged_in.py
+-rw-r--r--   0        0        0     1128 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/public.py
+-rw-r--r--   0        0        0     3118 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/models/types.py
+-rw-r--r--   0        0        0       31 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/util/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/util/errors.py
+-rw-r--r--   0        0        0     6920 2023-07-12 18:24:29.663271 aiochris-0.2.2/aiochris/util/search.py
+-rw-r--r--   0        0        0      782 2023-07-12 18:24:29.663271 aiochris-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 aiochris-0.2.2/PKG-INFO
```

### Comparing `aiochris-0.2.1/LICENSE` & `aiochris-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/README.md` & `aiochris-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/__init__.py` & `aiochris-0.2.2/aiochris/__init__.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/client/admin.py` & `aiochris-0.2.2/aiochris/client/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
     async def add_plugin(
         self,
         plugin_description: str | dict,
         compute_resources: str
         | ComputeResource
         | Iterable[ComputeResource | ComputeResourceName],
-        fname: str = "Plugin.json",
     ) -> Plugin:
         """
         Add a plugin to *CUBE*.
 
         Examples
         --------
 
@@ -95,22 +94,24 @@
         plugin_description: str | dict
             JSON description of a plugin.
             [spec](https://github.com/FNNDSC/CHRIS_docs/blob/5078aaf934bdbe313e85367f88aff7c14730a1d4/specs/ChRIS_Plugins.adoc#descriptor_file)
         compute_resources
             Compute resources to register the plugin to. Value can be either a comma-separated `str` of names,
             a `aiochris.models.public.ComputeResource`, a sequence of `aiochris.models.public.ComputeResource`,
             or a sequence of compute resource names as `str`.
-        fname: str
-            File name to send along in the multi-part POST request. Not important.
         """
         compute_names = _serialize_crs(compute_resources)
         if not isinstance(plugin_description, str):
             plugin_description = json.dumps(plugin_description)
         data = aiohttp.FormData()
-        data.add_field("fname", io.StringIO(plugin_description), filename=fname)
+        data.add_field(
+            "fname",
+            io.StringIO(plugin_description),
+            filename="aiochris_add_plugin.json",
+        )
         data.add_field("compute_names", compute_names)
         async with self.s.post(self.collection_links.admin, data=data) as res:
             await raise_for_status(res)
             return deserialize_linked(self, Plugin, await res.json())
 
     async def create_compute_resource(
         self,
```

### Comparing `aiochris-0.2.1/aiochris/client/anon.py` & `aiochris-0.2.2/aiochris/client/anon.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/client/authed.py` & `aiochris-0.2.2/aiochris/client/authed.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/client/base.py` & `aiochris-0.2.2/aiochris/client/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import abc
 from typing import AsyncContextManager, Generic, Optional, Callable, TypeVar
 
 import aiohttp
 from serde import from_dict
 
+from aiochris import Search
 from aiochris.link.collection_client import L, CollectionJsonApiClient
+from aiochris.models.public import PublicPlugin
 from aiochris.util.errors import raise_for_status
 
 CSelf = TypeVar(
     "CSelf", bound="BaseChrisClient"
 )  # can't wait for `Self` in Python 3.11!
 
 
@@ -92,7 +94,14 @@
         await self.close()
 
     async def close(self):
         """
         Close the HTTP session used by this client.
         """
         await self.s.close()
+
+    @abc.abstractmethod
+    def search_plugins(self, **query) -> Search[PublicPlugin]:
+        """
+        Search for plugins.
+        """
+        ...
```

### Comparing `aiochris-0.2.1/aiochris/client/normal.py` & `aiochris-0.2.2/aiochris/client/normal.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/examples.md` & `aiochris-0.2.2/aiochris/examples.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/home.md` & `aiochris-0.2.2/aiochris/home.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/link/collection_client.py` & `aiochris-0.2.2/aiochris/link/collection_client.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/link/http.py` & `aiochris-0.2.2/aiochris/link/http.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/link/linked.py` & `aiochris-0.2.2/aiochris/link/linked.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/link/metaprog.py` & `aiochris-0.2.2/aiochris/link/metaprog.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/models/collection_links.py` & `aiochris-0.2.2/aiochris/models/collection_links.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/models/data.py` & `aiochris-0.2.2/aiochris/models/data.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/models/enums.py` & `aiochris-0.2.2/aiochris/models/enums.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/models/logged_in.py` & `aiochris-0.2.2/aiochris/models/logged_in.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/models/types.py` & `aiochris-0.2.2/aiochris/models/types.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/util/errors.py` & `aiochris-0.2.2/aiochris/util/errors.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/aiochris/util/search.py` & `aiochris-0.2.2/aiochris/util/search.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.1/pyproject.toml` & `aiochris-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiochris"
-version = "0.2.1"
+version = "0.2.2"
 description = "ChRIS client built on aiohttp"
 authors = ["FNNDSC <dev@babyMRI.org>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `aiochris-0.2.1/PKG-INFO` & `aiochris-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiochris
-Version: 0.2.1
+Version: 0.2.2
 Summary: ChRIS client built on aiohttp
 License: MIT
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

