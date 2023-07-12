# Comparing `tmp/cql-parser-1.0.0.tar.gz` & `tmp/cql-parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cql-parser-1.0.0.tar", last modified: Wed Jul 12 10:21:20 2023, max compression
+gzip compressed data, was "cql-parser-1.0.1.tar", last modified: Wed Jul 12 11:22:50 2023, max compression
```

## Comparing `cql-parser-1.0.0.tar` & `cql-parser-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:21:20.530254 cql-parser-1.0.0/
--rw-r--r--   0 koerner   (1000) koerner   (1000)     3555 2023-07-12 10:21:20.530254 cql-parser-1.0.0/PKG-INFO
--rw-r--r--   0 koerner   (1000) koerner   (1000)     2745 2023-07-12 09:34:05.000000 cql-parser-1.0.0/README.md
--rw-r--r--   0 koerner   (1000) koerner   (1000)      478 2023-07-12 10:16:15.000000 cql-parser-1.0.0/pyproject.toml
--rw-r--r--   0 koerner   (1000) koerner   (1000)     1839 2023-07-12 10:21:20.530254 cql-parser-1.0.0/setup.cfg
--rw-r--r--   0 koerner   (1000) koerner   (1000)       38 2023-01-21 18:34:20.000000 cql-parser-1.0.0/setup.py
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:21:20.530254 cql-parser-1.0.0/src/
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:21:20.530254 cql-parser-1.0.0/src/cql/
--rw-r--r--   0 koerner   (1000) koerner   (1000)     1311 2023-07-12 09:30:34.000000 cql-parser-1.0.0/src/cql/__init__.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)     2295 2023-01-23 11:41:45.000000 cql-parser-1.0.0/src/cql/__main__.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)     3114 2023-07-12 09:29:32.000000 cql-parser-1.0.0/src/cql/lexer.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)    29451 2023-07-12 09:36:30.000000 cql-parser-1.0.0/src/cql/parser.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-24 17:24:03.000000 cql-parser-1.0.0/src/cql/py.typed
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:21:20.530254 cql-parser-1.0.0/src/cql_parser.egg-info/
--rw-r--r--   0 koerner   (1000) koerner   (1000)     3555 2023-07-12 10:21:20.000000 cql-parser-1.0.0/src/cql_parser.egg-info/PKG-INFO
--rw-r--r--   0 koerner   (1000) koerner   (1000)      507 2023-07-12 10:21:20.000000 cql-parser-1.0.0/src/cql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-07-12 10:21:20.000000 cql-parser-1.0.0/src/cql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)      131 2023-07-12 10:21:20.000000 cql-parser-1.0.0/src/cql_parser.egg-info/requires.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)        4 2023-07-12 10:21:20.000000 cql-parser-1.0.0/src/cql_parser.egg-info/top_level.txt
--rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-01-21 18:38:05.000000 cql-parser-1.0.0/src/cql_parser.egg-info/zip-safe
-drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 10:21:20.530254 cql-parser-1.0.0/tests/
--rw-r--r--   0 koerner   (1000) koerner   (1000)     1968 2023-01-23 11:36:22.000000 cql-parser-1.0.0/tests/test_init.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)    23517 2023-01-22 16:42:34.000000 cql-parser-1.0.0/tests/test_parser_cqlstandard.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)     1400 2023-01-22 17:34:54.000000 cql-parser-1.0.0/tests/test_parser_errors.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)      745 2023-01-22 16:25:14.000000 cql-parser-1.0.0/tests/test_parser_queries.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)    10371 2023-01-23 11:36:22.000000 cql-parser-1.0.0/tests/test_toCQL.py
--rw-r--r--   0 koerner   (1000) koerner   (1000)      827 2023-01-21 19:14:05.000000 cql-parser-1.0.0/tests/test_toXCQL.py
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:22:50.090190 cql-parser-1.0.1/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     4802 2023-07-12 11:22:50.090190 cql-parser-1.0.1/PKG-INFO
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     3775 2023-07-12 10:32:43.000000 cql-parser-1.0.1/README.md
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      478 2023-07-12 10:16:15.000000 cql-parser-1.0.1/pyproject.toml
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     2050 2023-07-12 11:22:50.090190 cql-parser-1.0.1/setup.cfg
+-rw-r--r--   0 koerner   (1000) koerner   (1000)       38 2023-01-21 18:34:20.000000 cql-parser-1.0.1/setup.py
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:22:50.090190 cql-parser-1.0.1/src/
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:22:50.090190 cql-parser-1.0.1/src/cql/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     1311 2023-07-12 09:30:34.000000 cql-parser-1.0.1/src/cql/__init__.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     2295 2023-01-23 11:41:45.000000 cql-parser-1.0.1/src/cql/__main__.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     3114 2023-07-12 09:29:32.000000 cql-parser-1.0.1/src/cql/lexer.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)    29451 2023-07-12 09:36:30.000000 cql-parser-1.0.1/src/cql/parser.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        0 2023-01-24 17:24:03.000000 cql-parser-1.0.1/src/cql/py.typed
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:22:50.090190 cql-parser-1.0.1/src/cql_parser.egg-info/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     4802 2023-07-12 11:22:50.000000 cql-parser-1.0.1/src/cql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      507 2023-07-12 11:22:50.000000 cql-parser-1.0.1/src/cql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-07-12 11:22:50.000000 cql-parser-1.0.1/src/cql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      131 2023-07-12 11:22:50.000000 cql-parser-1.0.1/src/cql_parser.egg-info/requires.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        4 2023-07-12 11:22:50.000000 cql-parser-1.0.1/src/cql_parser.egg-info/top_level.txt
+-rw-r--r--   0 koerner   (1000) koerner   (1000)        1 2023-01-21 18:38:05.000000 cql-parser-1.0.1/src/cql_parser.egg-info/zip-safe
+drwxr-xr-x   0 koerner   (1000) koerner   (1000)        0 2023-07-12 11:22:50.090190 cql-parser-1.0.1/tests/
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     1968 2023-01-23 11:36:22.000000 cql-parser-1.0.1/tests/test_init.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)    23517 2023-01-22 16:42:34.000000 cql-parser-1.0.1/tests/test_parser_cqlstandard.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)     1400 2023-01-22 17:34:54.000000 cql-parser-1.0.1/tests/test_parser_errors.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      745 2023-01-22 16:25:14.000000 cql-parser-1.0.1/tests/test_parser_queries.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)    10371 2023-01-23 11:36:22.000000 cql-parser-1.0.1/tests/test_toCQL.py
+-rw-r--r--   0 koerner   (1000) koerner   (1000)      827 2023-01-21 19:14:05.000000 cql-parser-1.0.1/tests/test_toXCQL.py
```

### Comparing `cql-parser-1.0.0/PKG-INFO` & `cql-parser-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: cql-parser
-Version: 1.0.0
+Version: 1.0.1
 Summary: "CQL (Contextual Query Language) Parser"
+Home-page: https://github.com/Querela/cql-python/
 Author: Erik Körner
 Author-email: "Erik Körner" <koerner@saw-leipzig.de>
 License: MIT
+Project-URL: Source, https://github.com/Querela/cql-python/
+Project-URL: Issue Tracker, https://github.com/Querela/cql-python/issues
+Keywords: CQL,CLARIN,Query Parser
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -20,14 +24,26 @@
 Provides-Extra: test
 Provides-Extra: style
 Provides-Extra: vendor
 Provides-Extra: build
 
 # CQL (Contextual Query Language) Parser (for Python)
 
+<!-- START: BADGES -->
+[![cql-parser @ PyPI](https://img.shields.io/pypi/v/cql-parser)](https://pypi.python.org/pypi/cql-parser)
+[![](https://img.shields.io/github/last-commit/Querela/cql-python)](https://github.com/Querela/cql-python/commits/main)
+[![Github Actions: Python package](https://github.com/Querela/cql-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/Querela/cql-python/actions/workflows/python-package.yml)
+
+[![](https://img.shields.io/badge/%20code%20style-black-000000)](https://github.com/psf/black)
+[![](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)
+[![](https://img.shields.io/badge/linting-flake8-yellowgreen)](https://github.com/PyCQA/flake8)  
+[![](https://img.shields.io/badge/%20doc%20style-sphinx-0a507a.svg)](https://www.sphinx-doc.org/en/master/usage/index.html)
+[![](https://img.shields.io/badge/%20doc%20style-google-3666d6.svg)](https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings)
+<!-- END: BADGES -->
+
 * [Grammar and Specification](http://www.loc.gov/standards/sru/cql/spec.html)
 
 ## Notice
 
 Prefix parsing and resolution is still work-in-progress!
 Test cases mostly check out but it definitely needs to be finished before
 using in real world scenarios.
```

### Comparing `cql-parser-1.0.0/README.md` & `cql-parser-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # CQL (Contextual Query Language) Parser (for Python)
 
+<!-- START: BADGES -->
+[![cql-parser @ PyPI](https://img.shields.io/pypi/v/cql-parser)](https://pypi.python.org/pypi/cql-parser)
+[![](https://img.shields.io/github/last-commit/Querela/cql-python)](https://github.com/Querela/cql-python/commits/main)
+[![Github Actions: Python package](https://github.com/Querela/cql-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/Querela/cql-python/actions/workflows/python-package.yml)
+
+[![](https://img.shields.io/badge/%20code%20style-black-000000)](https://github.com/psf/black)
+[![](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)
+[![](https://img.shields.io/badge/linting-flake8-yellowgreen)](https://github.com/PyCQA/flake8)  
+[![](https://img.shields.io/badge/%20doc%20style-sphinx-0a507a.svg)](https://www.sphinx-doc.org/en/master/usage/index.html)
+[![](https://img.shields.io/badge/%20doc%20style-google-3666d6.svg)](https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings)
+<!-- END: BADGES -->
+
 * [Grammar and Specification](http://www.loc.gov/standards/sru/cql/spec.html)
 
 ## Notice
 
 Prefix parsing and resolution is still work-in-progress!
 Test cases mostly check out but it definitely needs to be finished before
 using in real world scenarios.
```

### Comparing `cql-parser-1.0.0/setup.cfg` & `cql-parser-1.0.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = cql-parser
-version = 1.0.0
+version = 1.0.1
 author = Erik Körner
 author_email = "Erik Körner" <koerner@saw-leipzig.de>
 description = "CQL (Contextual Query Language) Parser"
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers = 
@@ -17,14 +17,22 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: YACC
 	Topic :: Text Processing :: General
 	Topic :: Utilities
+keywords = 
+	CQL
+	CLARIN
+	Query Parser
+url = https://github.com/Querela/cql-python/
+project_urls = 
+	Source = https://github.com/Querela/cql-python/
+	Issue Tracker = https://github.com/Querela/cql-python/issues
 
 [options]
 zip_safe = True
 include_package_data = True
 package_dir = 
 	=src
 packages = cql
```

### Comparing `cql-parser-1.0.0/src/cql/__init__.py` & `cql-parser-1.0.1/src/cql/__init__.py`

 * *Files identical despite different names*

### Comparing `cql-parser-1.0.0/src/cql/__main__.py` & `cql-parser-1.0.1/src/cql/__main__.py`

 * *Files identical despite different names*

### Comparing `cql-parser-1.0.0/src/cql/lexer.py` & `cql-parser-1.0.1/src/cql/lexer.py`

 * *Files identical despite different names*

### Comparing `cql-parser-1.0.0/src/cql/parser.py` & `cql-parser-1.0.1/src/cql/parser.py`

 * *Files identical despite different names*

### Comparing `cql-parser-1.0.0/src/cql_parser.egg-info/PKG-INFO` & `cql-parser-1.0.1/src/cql_parser.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: cql-parser
-Version: 1.0.0
+Version: 1.0.1
 Summary: "CQL (Contextual Query Language) Parser"
+Home-page: https://github.com/Querela/cql-python/
 Author: Erik Körner
 Author-email: "Erik Körner" <koerner@saw-leipzig.de>
 License: MIT
+Project-URL: Source, https://github.com/Querela/cql-python/
+Project-URL: Issue Tracker, https://github.com/Querela/cql-python/issues
+Keywords: CQL,CLARIN,Query Parser
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -20,14 +24,26 @@
 Provides-Extra: test
 Provides-Extra: style
 Provides-Extra: vendor
 Provides-Extra: build
 
 # CQL (Contextual Query Language) Parser (for Python)
 
+<!-- START: BADGES -->
+[![cql-parser @ PyPI](https://img.shields.io/pypi/v/cql-parser)](https://pypi.python.org/pypi/cql-parser)
+[![](https://img.shields.io/github/last-commit/Querela/cql-python)](https://github.com/Querela/cql-python/commits/main)
+[![Github Actions: Python package](https://github.com/Querela/cql-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/Querela/cql-python/actions/workflows/python-package.yml)
+
+[![](https://img.shields.io/badge/%20code%20style-black-000000)](https://github.com/psf/black)
+[![](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)
+[![](https://img.shields.io/badge/linting-flake8-yellowgreen)](https://github.com/PyCQA/flake8)  
+[![](https://img.shields.io/badge/%20doc%20style-sphinx-0a507a.svg)](https://www.sphinx-doc.org/en/master/usage/index.html)
+[![](https://img.shields.io/badge/%20doc%20style-google-3666d6.svg)](https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings)
+<!-- END: BADGES -->
+
 * [Grammar and Specification](http://www.loc.gov/standards/sru/cql/spec.html)
 
 ## Notice
 
 Prefix parsing and resolution is still work-in-progress!
 Test cases mostly check out but it definitely needs to be finished before
 using in real world scenarios.
```

### Comparing `cql-parser-1.0.0/tests/test_init.py` & `cql-parser-1.0.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `cql-parser-1.0.0/tests/test_parser_cqlstandard.py` & `cql-parser-1.0.1/tests/test_parser_cqlstandard.py`

 * *Files identical despite different names*

### Comparing `cql-parser-1.0.0/tests/test_parser_errors.py` & `cql-parser-1.0.1/tests/test_parser_errors.py`

 * *Files identical despite different names*

### Comparing `cql-parser-1.0.0/tests/test_parser_queries.py` & `cql-parser-1.0.1/tests/test_parser_queries.py`

 * *Files identical despite different names*

### Comparing `cql-parser-1.0.0/tests/test_toCQL.py` & `cql-parser-1.0.1/tests/test_toCQL.py`

 * *Files identical despite different names*

### Comparing `cql-parser-1.0.0/tests/test_toXCQL.py` & `cql-parser-1.0.1/tests/test_toXCQL.py`

 * *Files identical despite different names*

