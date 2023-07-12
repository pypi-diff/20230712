# Comparing `tmp/argus-rico-0.0.3.tar.gz` & `tmp/argus-rico-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argus-rico-0.0.3.tar", max compression
+gzip compressed data, was "argus-rico-0.0.4.tar", max compression
```

## Comparing `argus-rico-0.0.3.tar` & `argus-rico-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-05-24 01:07:47.899290 argus-rico-0.0.3/LICENSE
--rw-r--r--   0        0        0     1093 2023-06-27 22:00:39.860607 argus-rico-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2913 2023-06-27 22:01:41.485016 argus-rico-0.0.3/src/argus_rico/__init__.py
--rw-r--r--   0        0        0     1648 2023-06-12 16:35:31.667312 argus-rico-0.0.3/src/argus_rico/cli.py
--rw-r--r--   0        0        0      572 2023-06-05 21:00:52.783870 argus-rico-0.0.3/src/argus_rico/consumer.py
--rw-r--r--   0        0        0      792 2023-06-12 16:35:31.667436 argus-rico-0.0.3/src/argus_rico/efte_runner.py
--rw-r--r--   0        0        0     2060 2023-06-12 16:35:31.667549 argus-rico-0.0.3/src/argus_rico/heartbeat.py
--rw-r--r--   0        0        0     4960 2023-06-27 21:48:18.466470 argus-rico-0.0.3/src/argus_rico/images.py
--rw-r--r--   0        0        0      262 2023-06-12 16:35:31.667792 argus-rico-0.0.3/src/argus_rico/models/__init__.py
--rw-r--r--   0        0        0     8111 2023-06-12 16:35:31.667921 argus-rico-0.0.3/src/argus_rico/models/evr_image.py
--rw-r--r--   0        0        0     2740 2023-06-12 16:35:31.668047 argus-rico-0.0.3/src/argus_rico/producer.py
--rw-r--r--   0        0        0        0 2023-06-12 16:35:31.668081 argus-rico-0.0.3/src/argus_rico/py.typed
--rw-r--r--   0        0        0     2462 2023-06-12 16:35:31.668225 argus-rico-0.0.3/src/argus_rico/raw_streamer.py
--rw-r--r--   0        0        0     3597 2023-06-12 16:35:31.668377 argus-rico-0.0.3/src/argus_rico/schemas/raw_candidate.avsc
--rw-r--r--   0        0        0     6838 2023-06-12 16:35:31.668525 argus-rico-0.0.3/src/argus_rico/slack.py
--rw-r--r--   0        0        0     1417 2023-06-27 22:02:20.454635 argus-rico-0.0.3/setup.py
--rw-r--r--   0        0        0     1161 2023-06-27 22:02:20.454868 argus-rico-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-24 01:07:47.899290 argus-rico-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1115 2023-07-12 17:55:47.169576 argus-rico-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2913 2023-07-12 17:52:30.215011 argus-rico-0.0.4/src/argus_rico/__init__.py
+-rw-r--r--   0        0        0     1648 2023-06-12 16:35:31.667312 argus-rico-0.0.4/src/argus_rico/cli.py
+-rw-r--r--   0        0        0      572 2023-06-05 21:00:52.783870 argus-rico-0.0.4/src/argus_rico/consumer.py
+-rw-r--r--   0        0        0      792 2023-06-12 16:35:31.667436 argus-rico-0.0.4/src/argus_rico/efte_runner.py
+-rw-r--r--   0        0        0     2060 2023-06-12 16:35:31.667549 argus-rico-0.0.4/src/argus_rico/heartbeat.py
+-rw-r--r--   0        0        0     4960 2023-06-27 21:48:18.466470 argus-rico-0.0.4/src/argus_rico/images.py
+-rw-r--r--   0        0        0      262 2023-06-12 16:35:31.667792 argus-rico-0.0.4/src/argus_rico/models/__init__.py
+-rw-r--r--   0        0        0     8111 2023-06-12 16:35:31.667921 argus-rico-0.0.4/src/argus_rico/models/evr_image.py
+-rw-r--r--   0        0        0     2740 2023-06-12 16:35:31.668047 argus-rico-0.0.4/src/argus_rico/producer.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:31.668081 argus-rico-0.0.4/src/argus_rico/py.typed
+-rw-r--r--   0        0        0     2462 2023-06-12 16:35:31.668225 argus-rico-0.0.4/src/argus_rico/raw_streamer.py
+-rw-r--r--   0        0        0     3597 2023-06-12 16:35:31.668377 argus-rico-0.0.4/src/argus_rico/schemas/raw_candidate.avsc
+-rw-r--r--   0        0        0     6838 2023-06-12 16:35:31.668525 argus-rico-0.0.4/src/argus_rico/slack.py
+-rw-r--r--   0        0        0     1446 2023-07-12 17:55:59.072980 argus-rico-0.0.4/setup.py
+-rw-r--r--   0        0        0     1204 2023-07-12 17:55:59.073157 argus-rico-0.0.4/PKG-INFO
```

### Comparing `argus-rico-0.0.3/LICENSE` & `argus-rico-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/pyproject.toml` & `argus-rico-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "argus-rico"
-version = "0.0.3"
+version = "0.0.4"
 description = "Transient alert generation and database interaction for Argus and Evryscope"
 authors = ["Hank Corbett"]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.11"
 python-dotenv = "^0.19.0"
 fastavro = "^1.4.12"
@@ -23,14 +23,15 @@
 geojson-pydantic = "^0.6.2"
 numpy = "^1.24.3"
 ipython = "^8.14.0"
 sanitize-filename = "^1.2.0"
 pymongoarrow = "^0.7.0"
 pandas = "^2.0.2"
 qlsc = "^1.0.6"
+pre-commit = "^3.3.3"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 mypy = "^0.931"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
```

### Comparing `argus-rico-0.0.3/src/argus_rico/__init__.py` & `argus-rico-0.0.4/src/argus_rico/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Evryscope-Argus Transient Reporter."""
 
 __author__ = """Hank Corbett"""
 __email__ = "htc@unc.edu"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 __all__ = ["RicoHeartBeat", "RawStreamer", "EVRImageLoader"]
 
 import logging
 import os
 
 from dotenv import load_dotenv
```

### Comparing `argus-rico-0.0.3/src/argus_rico/cli.py` & `argus-rico-0.0.4/src/argus_rico/cli.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/src/argus_rico/consumer.py` & `argus-rico-0.0.4/src/argus_rico/consumer.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/src/argus_rico/efte_runner.py` & `argus-rico-0.0.4/src/argus_rico/efte_runner.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/src/argus_rico/heartbeat.py` & `argus-rico-0.0.4/src/argus_rico/heartbeat.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/src/argus_rico/images.py` & `argus-rico-0.0.4/src/argus_rico/images.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/src/argus_rico/models/evr_image.py` & `argus-rico-0.0.4/src/argus_rico/models/evr_image.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/src/argus_rico/producer.py` & `argus-rico-0.0.4/src/argus_rico/producer.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/src/argus_rico/raw_streamer.py` & `argus-rico-0.0.4/src/argus_rico/raw_streamer.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/src/argus_rico/schemas/raw_candidate.avsc` & `argus-rico-0.0.4/src/argus_rico/schemas/raw_candidate.avsc`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/src/argus_rico/slack.py` & `argus-rico-0.0.4/src/argus_rico/slack.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.3/setup.py` & `argus-rico-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
  'fastapi>=0.95.2,<0.96.0',
  'fastavro>=1.4.12,<2.0.0',
  'geojson-pydantic>=0.6.2,<0.7.0',
  'ipython>=8.14.0,<9.0.0',
  'numpy>=1.24.3,<2.0.0',
  'orjson>=3.8.13,<4.0.0',
  'pandas>=2.0.2,<3.0.0',
+ 'pre-commit>=3.3.3,<4.0.0',
  'pyarrow>=10.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'pymongo>=4.3.3,<5.0.0',
  'pymongoarrow>=0.7.0,<0.8.0',
  'python-dotenv>=0.19.0,<0.20.0',
  'qlsc>=1.0.6,<2.0.0',
  'rich>=13.3.5,<14.0.0',
@@ -34,15 +35,15 @@
  'slack-bolt>=1.18.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['rico = argus_rico.cli:main']}
 
 setup_kwargs = {
     'name': 'argus-rico',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Transient alert generation and database interaction for Argus and Evryscope',
     'long_description': None,
     'author': 'Hank Corbett',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `argus-rico-0.0.3/PKG-INFO` & `argus-rico-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argus-rico
-Version: 0.0.3
+Version: 0.0.4
 Summary: Transient alert generation and database interaction for Argus and Evryscope
 Author: Hank Corbett
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: astropy (>=5.3,<6.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
@@ -14,14 +14,15 @@
 Requires-Dist: fastapi (>=0.95.2,<0.96.0)
 Requires-Dist: fastavro (>=1.4.12,<2.0.0)
 Requires-Dist: geojson-pydantic (>=0.6.2,<0.7.0)
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: orjson (>=3.8.13,<4.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: pyarrow (>=10.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: pymongoarrow (>=0.7.0,<0.8.0)
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: qlsc (>=1.0.6,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
```

