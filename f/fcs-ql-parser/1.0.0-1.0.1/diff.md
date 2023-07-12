# Comparing `tmp/fcs-ql-parser-1.0.0.tar.gz` & `tmp/fcs-ql-parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcs-ql-parser-1.0.0.tar", last modified: Wed Jul 12 10:45:18 2023, max compression
+gzip compressed data, was "fcs-ql-parser-1.0.1.tar", last modified: Wed Jul 12 11:19:31 2023, max compression
```

## Comparing `fcs-ql-parser-1.0.0.tar` & `fcs-ql-parser-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:45:18.430224 fcs-ql-parser-1.0.0/
--rw-r--r--   0 koerner   (1000) koerner   (1000)     4582 2023-07-12 10:45:18.430224 fcs-ql-parser-1.0.0/PKG-INFO
--rw-r--r--   0 koerner   (1000) koerner   (1000)     3558 2023-07-12 10:44:32.000000 fcs-ql-parser-1.0.0/README.md
--rw-r--r--   0 koerner   (1000) koerner   (1000)      185 2023-01-23 15:29:52.000000 fcs-ql-parser-1.0.0/pyproject.toml
--rw-r--r--   0 koerner   (1000) koerner   (1000)     2472 2023-07-12 10:45:18.440224 fcs-ql-parser-1.0.0/setup.cfg
--rw-r--r--   0 koerner   (1000) koerner   (1000)       38 2023-01-23 14:56:58.000000 fcs-ql-parser-1.0.0/setup.py
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:45:18.420224 fcs-ql-parser-1.0.0/src/
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:45:18.430224 fcs-ql-parser-1.0.0/src/fcs_ql_parser.egg-info/
--rw-r--r--   0 koerner   (1000) koerner   (1000)     4582 2023-07-12 10:45:18.000000 fcs-ql-parser-1.0.0/src/fcs_ql_parser.egg-info/PKG-INFO
--rw-r--r--   0 koerner   (1000) koerner   (1000)      571 2023-07-12 10:45:18.000000 fcs-ql-parser-1.0.0/src/fcs_ql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-07-12 10:45:18.000000 fcs-ql-parser-1.0.0/src/fcs_ql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)      345 2023-07-12 10:45:18.000000 fcs-ql-parser-1.0.0/src/fcs_ql_parser.egg-info/requires.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)        6 2023-07-12 10:45:18.000000 fcs-ql-parser-1.0.0/src/fcs_ql_parser.egg-info/top_level.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-01-23 15:08:33.000000 fcs-ql-parser-1.0.0/src/fcs_ql_parser.egg-info/zip-safe
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:45:18.430224 fcs-ql-parser-1.0.0/src/fcsql/
--rw-r--r--   0 koerner   (1000) koerner   (1000)     2597 2023-01-23 15:02:28.000000 fcs-ql-parser-1.0.0/src/fcsql/FCSLexer.g4
--rw-r--r--   0 koerner   (1000) koerner   (1000)     8881 2023-01-23 17:11:02.000000 fcs-ql-parser-1.0.0/src/fcsql/FCSLexer.interp
--rw-r--r--   0 koerner   (1000) koerner   (1000)     9195 2023-01-23 17:11:02.000000 fcs-ql-parser-1.0.0/src/fcsql/FCSLexer.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)      459 2023-01-23 17:11:02.000000 fcs-ql-parser-1.0.0/src/fcsql/FCSLexer.tokens
--rw-r--r--   0 koerner   (1000) koerner   (1000)     2234 2023-01-23 15:02:28.000000 fcs-ql-parser-1.0.0/src/fcsql/FCSParser.g4
--rw-r--r--   0 koerner   (1000) koerner   (1000)     7523 2023-01-23 17:11:10.000000 fcs-ql-parser-1.0.0/src/fcsql/FCSParser.interp
--rw-r--r--   0 koerner   (1000) koerner   (1000)    60870 2023-01-23 17:11:10.000000 fcs-ql-parser-1.0.0/src/fcsql/FCSParser.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)      459 2023-01-23 17:11:10.000000 fcs-ql-parser-1.0.0/src/fcsql/FCSParser.tokens
--rw-r--r--   0 koerner   (1000) koerner   (1000)     6893 2023-01-23 17:11:10.000000 fcs-ql-parser-1.0.0/src/fcsql/FCSParserListener.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)     1547 2023-01-31 21:53:02.000000 fcs-ql-parser-1.0.0/src/fcsql/__init__.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)    52040 2023-03-09 22:09:44.000000 fcs-ql-parser-1.0.0/src/fcsql/parser.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-31 22:26:33.000000 fcs-ql-parser-1.0.0/src/fcsql/py.typed
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:19:31.790192 fcs-ql-parser-1.0.1/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     4881 2023-07-12 11:19:31.790192 fcs-ql-parser-1.0.1/PKG-INFO
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     3558 2023-07-12 10:44:32.000000 fcs-ql-parser-1.0.1/README.md
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      185 2023-01-23 15:29:52.000000 fcs-ql-parser-1.0.1/pyproject.toml
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     2755 2023-07-12 11:19:31.800192 fcs-ql-parser-1.0.1/setup.cfg
+-rw-r--r--   0 koerner   (1000) koerner   (1000)       38 2023-01-23 14:56:58.000000 fcs-ql-parser-1.0.1/setup.py
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:19:31.790192 fcs-ql-parser-1.0.1/src/
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:19:31.790192 fcs-ql-parser-1.0.1/src/fcs_ql_parser.egg-info/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     4881 2023-07-12 11:19:31.000000 fcs-ql-parser-1.0.1/src/fcs_ql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      571 2023-07-12 11:19:31.000000 fcs-ql-parser-1.0.1/src/fcs_ql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-07-12 11:19:31.000000 fcs-ql-parser-1.0.1/src/fcs_ql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      345 2023-07-12 11:19:31.000000 fcs-ql-parser-1.0.1/src/fcs_ql_parser.egg-info/requires.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        6 2023-07-12 11:19:31.000000 fcs-ql-parser-1.0.1/src/fcs_ql_parser.egg-info/top_level.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-01-23 15:08:33.000000 fcs-ql-parser-1.0.1/src/fcs_ql_parser.egg-info/zip-safe
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:19:31.790192 fcs-ql-parser-1.0.1/src/fcsql/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     2597 2023-01-23 15:02:28.000000 fcs-ql-parser-1.0.1/src/fcsql/FCSLexer.g4
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     8881 2023-01-23 17:11:02.000000 fcs-ql-parser-1.0.1/src/fcsql/FCSLexer.interp
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     9195 2023-01-23 17:11:02.000000 fcs-ql-parser-1.0.1/src/fcsql/FCSLexer.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      459 2023-01-23 17:11:02.000000 fcs-ql-parser-1.0.1/src/fcsql/FCSLexer.tokens
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     2234 2023-01-23 15:02:28.000000 fcs-ql-parser-1.0.1/src/fcsql/FCSParser.g4
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     7523 2023-01-23 17:11:10.000000 fcs-ql-parser-1.0.1/src/fcsql/FCSParser.interp
+-rw-r--r--   0 koerner   (1000) koerner   (1000)    60870 2023-01-23 17:11:10.000000 fcs-ql-parser-1.0.1/src/fcsql/FCSParser.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      459 2023-01-23 17:11:10.000000 fcs-ql-parser-1.0.1/src/fcsql/FCSParser.tokens
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     6893 2023-01-23 17:11:10.000000 fcs-ql-parser-1.0.1/src/fcsql/FCSParserListener.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     1547 2023-01-31 21:53:02.000000 fcs-ql-parser-1.0.1/src/fcsql/__init__.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)    52040 2023-03-09 22:09:44.000000 fcs-ql-parser-1.0.1/src/fcsql/parser.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-31 22:26:33.000000 fcs-ql-parser-1.0.1/src/fcsql/py.typed
```

### Comparing `fcs-ql-parser-1.0.0/PKG-INFO` & `fcs-ql-parser-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: fcs-ql-parser
-Version: 1.0.0
+Version: 1.0.1
 Summary: "FCS-QL (CLARIN-FCS Core 2.0 Query Language) Grammar and Parser"
+Home-page: https://github.com/Querela/fcs-ql-python/
 Author: Erik Körner
 Author-email: "Erik Körner" <koerner@saw-leipzig.de>
 License: MIT
+Project-URL: Source, https://github.com/Querela/fcs-ql-python/
+Project-URL: Documentation, https://fcs-ql-python.readthedocs.io/
+Project-URL: Issue Tracker, https://github.com/Querela/fcs-ql-python/issues
+Keywords: FCS,FCS-QL,CLARIN,Query Parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `fcs-ql-parser-1.0.0/README.md` & `fcs-ql-parser-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/setup.cfg` & `fcs-ql-parser-1.0.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = fcs-ql-parser
-version = 1.0.0
+version = 1.0.1
 author = Erik Körner
 author_email = "Erik Körner" <koerner@saw-leipzig.de>
 description = "FCS-QL (CLARIN-FCS Core 2.0 Query Language) Grammar and Parser"
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers = 
@@ -20,14 +20,24 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Text Processing :: General
 	Topic :: Utilities
+keywords = 
+	FCS
+	FCS-QL
+	CLARIN
+	Query Parser
+url = https://github.com/Querela/fcs-ql-python/
+project_urls = 
+	Source = https://github.com/Querela/fcs-ql-python/
+	Documentation = https://fcs-ql-python.readthedocs.io/
+	Issue Tracker = https://github.com/Querela/fcs-ql-python/issues
 
 [options]
 zip_safe = True
 include_package_data = True
 package_dir = 
 	=src
 packages = fcsql
```

### Comparing `fcs-ql-parser-1.0.0/src/fcs_ql_parser.egg-info/PKG-INFO` & `fcs-ql-parser-1.0.1/src/fcs_ql_parser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: fcs-ql-parser
-Version: 1.0.0
+Version: 1.0.1
 Summary: "FCS-QL (CLARIN-FCS Core 2.0 Query Language) Grammar and Parser"
+Home-page: https://github.com/Querela/fcs-ql-python/
 Author: Erik Körner
 Author-email: "Erik Körner" <koerner@saw-leipzig.de>
 License: MIT
+Project-URL: Source, https://github.com/Querela/fcs-ql-python/
+Project-URL: Documentation, https://fcs-ql-python.readthedocs.io/
+Project-URL: Issue Tracker, https://github.com/Querela/fcs-ql-python/issues
+Keywords: FCS,FCS-QL,CLARIN,Query Parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `fcs-ql-parser-1.0.0/src/fcs_ql_parser.egg-info/SOURCES.txt` & `fcs-ql-parser-1.0.1/src/fcs_ql_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/src/fcsql/FCSLexer.g4` & `fcs-ql-parser-1.0.1/src/fcsql/FCSLexer.g4`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/src/fcsql/FCSLexer.interp` & `fcs-ql-parser-1.0.1/src/fcsql/FCSLexer.interp`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/src/fcsql/FCSLexer.py` & `fcs-ql-parser-1.0.1/src/fcsql/FCSLexer.py`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/src/fcsql/FCSParser.g4` & `fcs-ql-parser-1.0.1/src/fcsql/FCSParser.g4`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/src/fcsql/FCSParser.interp` & `fcs-ql-parser-1.0.1/src/fcsql/FCSParser.interp`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/src/fcsql/FCSParser.py` & `fcs-ql-parser-1.0.1/src/fcsql/FCSParser.py`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/src/fcsql/FCSParserListener.py` & `fcs-ql-parser-1.0.1/src/fcsql/FCSParserListener.py`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/src/fcsql/__init__.py` & `fcs-ql-parser-1.0.1/src/fcsql/__init__.py`

 * *Files identical despite different names*

### Comparing `fcs-ql-parser-1.0.0/src/fcsql/parser.py` & `fcs-ql-parser-1.0.1/src/fcsql/parser.py`

 * *Files identical despite different names*

