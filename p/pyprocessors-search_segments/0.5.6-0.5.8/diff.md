# Comparing `tmp/pyprocessors-search_segments-0.5.6.tar.gz` & `tmp/pyprocessors_search_segments-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors-search_segments-0.5.6.tar", last modified: Wed Jul 12 13:09:38 2023, max compression
+gzip compressed data, was "pyprocessors_search_segments-0.5.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprocessors-search_segments-0.5.6.tar` & `pyprocessors_search_segments-0.5.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       97 2021-04-14 09:32:17.791141 pyprocessors-search_segments-0.5.6/.dockerignore
--rw-r--r--   0        0        0      167 2023-04-27 11:09:38.051202 pyprocessors-search_segments-0.5.6/.gitignore
--rw-r--r--   0        0        0      448 2021-04-14 09:32:17.791141 pyprocessors-search_segments-0.5.6/Dockerfile
--rw-r--r--   0        0        0    10219 2023-07-12 11:36:24.468029 pyprocessors-search_segments-0.5.6/Jenkinsfile
--rw-r--r--   0        0        0      380 2022-02-22 13:26:31.568419 pyprocessors-search_segments-0.5.6/README.md
--rw-r--r--   0        0        0     1559 2022-04-08 12:08:36.518352 pyprocessors-search_segments-0.5.6/bumpversion.py
--rw-r--r--   0        0        0       55 2023-07-12 13:09:17.606149 pyprocessors-search_segments-0.5.6/pyprocessors_search_segments/__init__.py
--rw-r--r--   0        0        0     3244 2023-07-12 13:03:17.154363 pyprocessors-search_segments-0.5.6/pyprocessors_search_segments/kt_client.py
--rw-r--r--   0        0        0     4036 2023-07-12 12:24:56.103911 pyprocessors-search_segments-0.5.6/pyprocessors_search_segments/search_segments.py
--rw-r--r--   0        0        0     2589 2023-07-12 12:05:45.683264 pyprocessors-search_segments-0.5.6/pyproject.toml
--rw-r--r--   0        0        0        0 2021-03-25 07:15:30.426146 pyprocessors-search_segments-0.5.6/tests/__init__.py
--rw-r--r--   0        0        0    17492 2023-07-12 12:39:23.381960 pyprocessors-search_segments-0.5.6/tests/data/question_segments.json
--rw-r--r--   0        0        0      995 2023-07-12 12:39:31.369939 pyprocessors-search_segments-0.5.6/tests/test_search_segments.py
--rw-r--r--   0        0        0      951 2023-02-15 16:25:11.973559 pyprocessors-search_segments-0.5.6/tox.ini
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 pyprocessors-search_segments-0.5.6/setup.py
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 pyprocessors-search_segments-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-07-12 12:30:09.372448 pyprocessors_search_segments-0.5.8/.dockerignore
+-rw-r--r--   0        0        0      167 2023-07-12 12:30:09.372448 pyprocessors_search_segments-0.5.8/.gitignore
+-rw-r--r--   0        0        0      448 2023-07-12 12:30:09.373448 pyprocessors_search_segments-0.5.8/Dockerfile
+-rw-r--r--   0        0        0    10219 2023-07-12 12:30:09.373448 pyprocessors_search_segments-0.5.8/Jenkinsfile
+-rw-r--r--   0        0        0      380 2023-07-12 12:30:09.374448 pyprocessors_search_segments-0.5.8/README.md
+-rw-r--r--   0        0        0     1559 2023-07-12 12:30:09.374448 pyprocessors_search_segments-0.5.8/bumpversion.py
+-rw-r--r--   0        0        0       55 2023-07-12 17:01:07.102526 pyprocessors_search_segments-0.5.8/pyprocessors_search_segments/__init__.py
+-rw-r--r--   0        0        0     3244 2023-07-12 13:03:47.522274 pyprocessors_search_segments-0.5.8/pyprocessors_search_segments/kt_client.py
+-rw-r--r--   0        0        0     4036 2023-07-12 12:30:09.375448 pyprocessors_search_segments-0.5.8/pyprocessors_search_segments/search_segments.py
+-rw-r--r--   0        0        0     2589 2023-07-12 12:30:09.376448 pyprocessors_search_segments-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 12:30:09.377448 pyprocessors_search_segments-0.5.8/tests/__init__.py
+-rw-r--r--   0        0        0    17492 2023-07-12 12:40:04.152493 pyprocessors_search_segments-0.5.8/tests/data/question_segments.json
+-rw-r--r--   0        0        0      995 2023-07-12 12:40:04.153493 pyprocessors_search_segments-0.5.8/tests/test_search_segments.py
+-rw-r--r--   0        0        0      951 2023-07-12 12:30:09.378448 pyprocessors_search_segments-0.5.8/tox.ini
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 pyprocessors_search_segments-0.5.8/setup.py
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 pyprocessors_search_segments-0.5.8/PKG-INFO
```

### Comparing `pyprocessors-search_segments-0.5.6/Jenkinsfile` & `pyprocessors_search_segments-0.5.8/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors-search_segments-0.5.6/bumpversion.py` & `pyprocessors_search_segments-0.5.8/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-search_segments-0.5.6/pyprocessors_search_segments/kt_client.py` & `pyprocessors_search_segments-0.5.8/pyprocessors_search_segments/kt_client.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-search_segments-0.5.6/pyprocessors_search_segments/search_segments.py` & `pyprocessors_search_segments-0.5.8/pyprocessors_search_segments/search_segments.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-search_segments-0.5.6/pyproject.toml` & `pyprocessors_search_segments-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors-search_segments-0.5.6/tests/data/question_segments.json` & `pyprocessors_search_segments-0.5.8/tests/data/question_segments.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-search_segments-0.5.6/tests/test_search_segments.py` & `pyprocessors_search_segments-0.5.8/tests/test_search_segments.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-search_segments-0.5.6/tox.ini` & `pyprocessors_search_segments-0.5.8/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors-search_segments-0.5.6/setup.py` & `pyprocessors_search_segments-0.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
           'flask==2.1.3']}
 
 entry_points = \
 {'pyprocessors.plugins': ['search_segments = '
                           'pyprocessors_search_segments.search_segments:SearchSegmentsProcessor']}
 
 setup(name='pyprocessors-search_segments',
-      version='0.5.6',
+      version='0.5.8',
       description='Similar segments processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyprocessors-search_segments-0.5.6/PKG-INFO` & `pyprocessors_search_segments-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-search_segments
-Version: 0.5.6
+Version: 0.5.8
 Summary: Similar segments processor
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

