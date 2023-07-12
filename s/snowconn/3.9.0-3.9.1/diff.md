# Comparing `tmp/snowconn-3.9.0.tar.gz` & `tmp/snowconn-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snowconn-3.9.0.tar", last modified: Wed Jul  6 07:55:04 2022, max compression
+gzip compressed data, was "dist/snowconn-3.9.1.tar", last modified: Thu Oct 27 16:20:24 2022, max compression
```

## Comparing `snowconn-3.9.0.tar` & `snowconn-3.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-06 07:55:04.000000 snowconn-3.9.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1066 2022-07-06 07:54:53.000000 snowconn-3.9.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11860 2022-07-06 07:55:04.000000 snowconn-3.9.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11507 2022-07-06 07:54:53.000000 snowconn-3.9.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-07-06 07:55:04.000000 snowconn-3.9.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1120 2022-07-06 07:54:53.000000 snowconn-3.9.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-06 07:55:04.000000 snowconn-3.9.0/snowconn/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       30 2022-07-06 07:54:53.000000 snowconn-3.9.0/snowconn/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13733 2022-07-06 07:54:53.000000 snowconn-3.9.0/snowconn/connect.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-06 07:55:04.000000 snowconn-3.9.0/snowconn.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11860 2022-07-06 07:55:04.000000 snowconn-3.9.0/snowconn.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      226 2022-07-06 07:55:04.000000 snowconn-3.9.0/snowconn.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-07-06 07:55:04.000000 snowconn-3.9.0/snowconn.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      270 2022-07-06 07:55:04.000000 snowconn-3.9.0/snowconn.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2022-07-06 07:55:04.000000 snowconn-3.9.0/snowconn.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-27 16:20:24.000000 snowconn-3.9.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1066 2022-10-27 16:20:12.000000 snowconn-3.9.1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11860 2022-10-27 16:20:24.000000 snowconn-3.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11507 2022-10-27 16:20:12.000000 snowconn-3.9.1/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-10-27 16:20:24.000000 snowconn-3.9.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1150 2022-10-27 16:20:12.000000 snowconn-3.9.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-27 16:20:24.000000 snowconn-3.9.1/snowconn/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       30 2022-10-27 16:20:12.000000 snowconn-3.9.1/snowconn/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13733 2022-10-27 16:20:12.000000 snowconn-3.9.1/snowconn/connect.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-27 16:20:24.000000 snowconn-3.9.1/snowconn.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11860 2022-10-27 16:20:24.000000 snowconn-3.9.1/snowconn.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      226 2022-10-27 16:20:24.000000 snowconn-3.9.1/snowconn.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-10-27 16:20:24.000000 snowconn-3.9.1/snowconn.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2022-10-27 16:20:24.000000 snowconn-3.9.1/snowconn.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2022-10-27 16:20:24.000000 snowconn-3.9.1/snowconn.egg-info/top_level.txt
```

### Comparing `snowconn-3.9.0/LICENSE` & `snowconn-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snowconn-3.9.0/PKG-INFO` & `snowconn-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowconn
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python utilities for connection to the Snowflake data warehouse
 Home-page: https://github.com/Daltix/snowconn
 Author: Daltix NV
 Author-email: snowconn@daltix.com
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 Provides-Extra: storage
```

### Comparing `snowconn-3.9.0/README.md` & `snowconn-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `snowconn-3.9.0/setup.py` & `snowconn-3.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 readme_path = path.join(this_directory, 'README.md')
 
 with open(readme_path, encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='snowconn',
-    version='3.9.0',
+    version='3.9.1',
     description='Python utilities for connection to the Snowflake data '
                 'warehouse',
     url='https://github.com/Daltix/snowconn',
     author='Daltix NV',
     author_email='snowconn@daltix.com',
     packages=['snowconn'],
     install_requires=[
         'six',
         'snowflake-connector-python==2.7.9',
         'snowflake-sqlalchemy>=1.3, <1.4',
+        'sqlalchemy<=1.4.41',
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     extras_require={
         "pandas": [
             "snowflake-connector-python[pandas]==2.7.9",
```

### Comparing `snowconn-3.9.0/snowconn/connect.py` & `snowconn-3.9.1/snowconn/connect.py`

 * *Files identical despite different names*

### Comparing `snowconn-3.9.0/snowconn.egg-info/PKG-INFO` & `snowconn-3.9.1/snowconn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowconn
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python utilities for connection to the Snowflake data warehouse
 Home-page: https://github.com/Daltix/snowconn
 Author: Daltix NV
 Author-email: snowconn@daltix.com
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 Provides-Extra: storage
```

