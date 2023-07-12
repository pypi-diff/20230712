# Comparing `tmp/drf-jsonschema-serializer-1.0.0.tar.gz` & `tmp/drf-jsonschema-serializer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-jsonschema-serializer-1.0.0.tar", last modified: Wed Feb 15 09:44:44 2023, max compression
+gzip compressed data, was "drf-jsonschema-serializer-2.0.0.tar", last modified: Wed Jul 12 09:35:50 2023, max compression
```

## Comparing `drf-jsonschema-serializer-1.0.0.tar` & `drf-jsonschema-serializer-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:44:44.916459 drf-jsonschema-serializer-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-02-15 09:44:44.916459 drf-jsonschema-serializer-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:44:44.912459 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:44:44.912459 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-02-15 09:44:44.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-15 09:44:44.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 09:44:44.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 09:44:44.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-15 09:44:44.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-15 09:44:44.000000 drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-02-15 09:44:44.916459 drf-jsonschema-serializer-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:44:44.912459 drf-jsonschema-serializer-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    32608 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-15 09:44:38.000000 drf-jsonschema-serializer-1.0.0/tests/test_model_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:35:50.310596 drf-jsonschema-serializer-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-12 09:35:50.310596 drf-jsonschema-serializer-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:35:50.306596 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:35:50.310596 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-12 09:35:50.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-12 09:35:50.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:35:50.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:35:50.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-12 09:35:50.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 09:35:50.000000 drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-12 09:35:50.310596 drf-jsonschema-serializer-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:35:50.310596 drf-jsonschema-serializer-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    32608 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-12 09:35:45.000000 drf-jsonschema-serializer-2.0.0/tests/test_model_serializer.py
```

### Comparing `drf-jsonschema-serializer-1.0.0/LICENSE` & `drf-jsonschema-serializer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-serializer-1.0.0/PKG-INFO` & `drf-jsonschema-serializer-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: drf-jsonschema-serializer
-Version: 1.0.0
+Version: 2.0.0
 Summary: JSON Schema support for Django REST Framework
 Home-page: https://github.com/maykinmedia/drf-jsonschema-serializer
 Author: ISProjects, Maykin Media
 Author-email: support@maykinmedia.nl
 License: BSD
 Project-URL: Documentation, http://drf-jsonschema-serializer.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/drf-jsonschema-serializer/blob/main/docs/changelog.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/drf-jsonschema-serializer/issues
 Project-URL: Source Code, https://github.com/maykinmedia/drf-jsonschema-serializer
 Keywords: django,rest,polymorphic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all-format-validators
 Provides-Extra: tests
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 =========================================
 Django REST Framework JSON Schema support
 =========================================
 
-:Version: 1.0.0
+:Version: 2.0.0
 :Source: https://github.com/maykinmedia/drf-jsonschema-serializer
 :Keywords: django, rest, jsonschema
 
 |build-status| |coverage| |linting| |black| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `drf-jsonschema-serializer-1.0.0/README.rst` & `drf-jsonschema-serializer-2.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =========================================
 Django REST Framework JSON Schema support
 =========================================
 
-:Version: 1.0.0
+:Version: 2.0.0
 :Source: https://github.com/maykinmedia/drf-jsonschema-serializer
 :Keywords: django, rest, jsonschema
 
 |build-status| |coverage| |linting| |black| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer/convert.py` & `drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer/convert.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer/converters.py` & `drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer/converters.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer/fields.py` & `drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer/fields.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer.egg-info/PKG-INFO` & `drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: drf-jsonschema-serializer
-Version: 1.0.0
+Version: 2.0.0
 Summary: JSON Schema support for Django REST Framework
 Home-page: https://github.com/maykinmedia/drf-jsonschema-serializer
 Author: ISProjects, Maykin Media
 Author-email: support@maykinmedia.nl
 License: BSD
 Project-URL: Documentation, http://drf-jsonschema-serializer.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/drf-jsonschema-serializer/blob/main/docs/changelog.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/drf-jsonschema-serializer/issues
 Project-URL: Source Code, https://github.com/maykinmedia/drf-jsonschema-serializer
 Keywords: django,rest,polymorphic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all-format-validators
 Provides-Extra: tests
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 =========================================
 Django REST Framework JSON Schema support
 =========================================
 
-:Version: 1.0.0
+:Version: 2.0.0
 :Source: https://github.com/maykinmedia/drf-jsonschema-serializer
 :Keywords: django, rest, jsonschema
 
 |build-status| |coverage| |linting| |black| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `drf-jsonschema-serializer-1.0.0/drf_jsonschema_serializer.egg-info/SOURCES.txt` & `drf-jsonschema-serializer-2.0.0/drf_jsonschema_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-serializer-1.0.0/setup.cfg` & `drf-jsonschema-serializer-2.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-jsonschema-serializer
-version = 1.0.0
+version = 2.0.0
 description = JSON Schema support for Django REST Framework
 long_description = file: README.rst
 url = https://github.com/maykinmedia/drf-jsonschema-serializer
 project_urls = 
 	Documentation = http://drf-jsonschema-serializer.readthedocs.io/en/latest/
 	Changelog = https://github.com/maykinmedia/drf-jsonschema-serializer/blob/main/docs/changelog.rst
 	Bug Tracker = https://github.com/maykinmedia/drf-jsonschema-serializer/issues
@@ -13,24 +13,25 @@
 author = ISProjects, Maykin Media
 author_email = support@maykinmedia.nl
 keywords = django, rest, polymorphic
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires =
```

### Comparing `drf-jsonschema-serializer-1.0.0/tests/test_convert.py` & `drf-jsonschema-serializer-2.0.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-serializer-1.0.0/tests/test_fields.py` & `drf-jsonschema-serializer-2.0.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-serializer-1.0.0/tests/test_model_serializer.py` & `drf-jsonschema-serializer-2.0.0/tests/test_model_serializer.py`

 * *Files identical despite different names*

