# Comparing `tmp/fcs-simple-endpoint-1.0.0.tar.gz` & `tmp/fcs-simple-endpoint-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcs-simple-endpoint-1.0.0.tar", last modified: Wed Jul 12 10:52:35 2023, max compression
+gzip compressed data, was "fcs-simple-endpoint-1.0.1.tar", last modified: Wed Jul 12 11:13:41 2023, max compression
```

## Comparing `fcs-simple-endpoint-1.0.0.tar` & `fcs-simple-endpoint-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:52:35.960217 fcs-simple-endpoint-1.0.0/
--rw-r--r--   0 koerner   (1000) koerner   (1000)     3281 2023-07-12 10:52:35.960217 fcs-simple-endpoint-1.0.0/PKG-INFO
--rw-r--r--   0 koerner   (1000) koerner   (1000)     2945 2023-07-12 10:51:40.000000 fcs-simple-endpoint-1.0.0/README.md
--rw-r--r--   0 koerner   (1000) koerner   (1000)      121 2023-01-27 12:46:04.000000 fcs-simple-endpoint-1.0.0/pyproject.toml
--rw-r--r--   0 koerner   (1000) koerner   (1000)     1741 2023-07-12 10:52:35.960217 fcs-simple-endpoint-1.0.0/setup.cfg
--rw-r--r--   0 koerner   (1000) koerner   (1000)       38 2023-01-27 12:44:38.000000 fcs-simple-endpoint-1.0.0/setup.py
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:52:35.950217 fcs-simple-endpoint-1.0.0/src/
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:52:35.960217 fcs-simple-endpoint-1.0.0/src/clarin/
--rw-r--r--   0 koerner   (1000) koerner   (1000)       65 2023-01-28 02:51:11.000000 fcs-simple-endpoint-1.0.0/src/clarin/__init__.py
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:52:35.960217 fcs-simple-endpoint-1.0.0/src/clarin/sru/
--rw-r--r--   0 koerner   (1000) koerner   (1000)       65 2023-01-28 02:49:27.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/__init__.py
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:52:35.960217 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/
--rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-28 02:02:28.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/__init__.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)     4849 2023-03-06 16:50:13.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/constants.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-28 02:50:16.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/py.typed
--rw-r--r--   0 koerner   (1000) koerner   (1000)     2390 2023-02-01 00:45:39.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/queryparser.py
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:52:35.960217 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/server/
--rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-02-02 14:43:11.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/server/__init__.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)    11237 2023-02-03 14:56:23.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/server/auth.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)    35690 2023-07-05 09:32:44.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/server/search.py
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:52:35.960217 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/xml/
--rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-28 02:02:15.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/xml/__init__.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)    27575 2023-07-05 09:51:41.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/xml/reader.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)    24661 2023-07-05 10:17:26.000000 fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/xml/writer.py
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:52:35.960217 fcs-simple-endpoint-1.0.0/src/fcs_simple_endpoint.egg-info/
--rw-r--r--   0 koerner   (1000) koerner   (1000)     3281 2023-07-12 10:52:35.000000 fcs-simple-endpoint-1.0.0/src/fcs_simple_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 koerner   (1000) koerner   (1000)      703 2023-07-12 10:52:35.000000 fcs-simple-endpoint-1.0.0/src/fcs_simple_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-07-12 10:52:35.000000 fcs-simple-endpoint-1.0.0/src/fcs_simple_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)      364 2023-07-12 10:52:35.000000 fcs-simple-endpoint-1.0.0/src/fcs_simple_endpoint.egg-info/requires.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)        7 2023-07-12 10:52:35.000000 fcs-simple-endpoint-1.0.0/src/fcs_simple_endpoint.egg-info/top_level.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-01-27 14:38:55.000000 fcs-simple-endpoint-1.0.0/src/fcs_simple_endpoint.egg-info/zip-safe
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:13:41.650198 fcs-simple-endpoint-1.0.1/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     3616 2023-07-12 11:13:41.650198 fcs-simple-endpoint-1.0.1/PKG-INFO
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     2945 2023-07-12 10:51:40.000000 fcs-simple-endpoint-1.0.1/README.md
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      121 2023-01-27 12:46:04.000000 fcs-simple-endpoint-1.0.1/pyproject.toml
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     2059 2023-07-12 11:13:41.650198 fcs-simple-endpoint-1.0.1/setup.cfg
+-rw-r--r--   0 koerner   (1000) koerner   (1000)       38 2023-01-27 12:44:38.000000 fcs-simple-endpoint-1.0.1/setup.py
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:13:41.640198 fcs-simple-endpoint-1.0.1/src/
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:13:41.640198 fcs-simple-endpoint-1.0.1/src/clarin/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)       65 2023-01-28 02:51:11.000000 fcs-simple-endpoint-1.0.1/src/clarin/__init__.py
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:13:41.640198 fcs-simple-endpoint-1.0.1/src/clarin/sru/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)       65 2023-01-28 02:49:27.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/__init__.py
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:13:41.650198 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-28 02:02:28.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/__init__.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     4849 2023-03-06 16:50:13.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/constants.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-28 02:50:16.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/py.typed
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     2390 2023-02-01 00:45:39.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/queryparser.py
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:13:41.650198 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/server/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-02-02 14:43:11.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/server/__init__.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)    11237 2023-02-03 14:56:23.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/server/auth.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)    35690 2023-07-05 09:32:44.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/server/search.py
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:13:41.650198 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/xml/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-28 02:02:15.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/xml/__init__.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)    27575 2023-07-05 09:51:41.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/xml/reader.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)    24661 2023-07-05 10:17:26.000000 fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/xml/writer.py
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:13:41.650198 fcs-simple-endpoint-1.0.1/src/fcs_simple_endpoint.egg-info/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     3616 2023-07-12 11:13:41.000000 fcs-simple-endpoint-1.0.1/src/fcs_simple_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      703 2023-07-12 11:13:41.000000 fcs-simple-endpoint-1.0.1/src/fcs_simple_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-07-12 11:13:41.000000 fcs-simple-endpoint-1.0.1/src/fcs_simple_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      364 2023-07-12 11:13:41.000000 fcs-simple-endpoint-1.0.1/src/fcs_simple_endpoint.egg-info/requires.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        7 2023-07-12 11:13:41.000000 fcs-simple-endpoint-1.0.1/src/fcs_simple_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-01-27 14:38:55.000000 fcs-simple-endpoint-1.0.1/src/fcs_simple_endpoint.egg-info/zip-safe
```

### Comparing `fcs-simple-endpoint-1.0.0/PKG-INFO` & `fcs-simple-endpoint-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: fcs-simple-endpoint
-Version: 1.0.0
+Version: 1.0.1
 Summary: "FCS SRU Simple Endpoint"
+Home-page: https://github.com/Querela/fcs-simple-endpoint-python/
 Author: Erik Körner
 Author-email: "Erik Körner" <koerner@saw-leipzig.de>
 License: MIT
+Project-URL: Source, https://github.com/Querela/fcs-simple-endpoint-python/
+Project-URL: Documentation, https://fcs-simple-endpoint-python.readthedocs.io/
+Project-URL: Issue Tracker, https://github.com/Querela/fcs-simple-endpoint-python/issues
+Keywords: SRU,FCS,CLARIN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: style
 Provides-Extra: docs
 Provides-Extra: build
```

### Comparing `fcs-simple-endpoint-1.0.0/README.md` & `fcs-simple-endpoint-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/constants.py` & `fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/constants.py`

 * *Files identical despite different names*

### Comparing `fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/queryparser.py` & `fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/queryparser.py`

 * *Files identical despite different names*

### Comparing `fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/server/auth.py` & `fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/server/auth.py`

 * *Files identical despite different names*

### Comparing `fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/server/search.py` & `fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/server/search.py`

 * *Files identical despite different names*

### Comparing `fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/xml/reader.py` & `fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/xml/reader.py`

 * *Files identical despite different names*

### Comparing `fcs-simple-endpoint-1.0.0/src/clarin/sru/fcs/xml/writer.py` & `fcs-simple-endpoint-1.0.1/src/clarin/sru/fcs/xml/writer.py`

 * *Files identical despite different names*

### Comparing `fcs-simple-endpoint-1.0.0/src/fcs_simple_endpoint.egg-info/PKG-INFO` & `fcs-simple-endpoint-1.0.1/src/fcs_simple_endpoint.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: fcs-simple-endpoint
-Version: 1.0.0
+Version: 1.0.1
 Summary: "FCS SRU Simple Endpoint"
+Home-page: https://github.com/Querela/fcs-simple-endpoint-python/
 Author: Erik Körner
 Author-email: "Erik Körner" <koerner@saw-leipzig.de>
 License: MIT
+Project-URL: Source, https://github.com/Querela/fcs-simple-endpoint-python/
+Project-URL: Documentation, https://fcs-simple-endpoint-python.readthedocs.io/
+Project-URL: Issue Tracker, https://github.com/Querela/fcs-simple-endpoint-python/issues
+Keywords: SRU,FCS,CLARIN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: style
 Provides-Extra: docs
 Provides-Extra: build
```

### Comparing `fcs-simple-endpoint-1.0.0/src/fcs_simple_endpoint.egg-info/SOURCES.txt` & `fcs-simple-endpoint-1.0.1/src/fcs_simple_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

