# Comparing `tmp/superannotate_databricks_connector-0.0.1.dev2.tar.gz` & `tmp/superannotate_databricks_connector-0.0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superannotate_databricks_connector-0.0.1.dev2.tar", last modified: Wed Jun 28 05:56:02 2023, max compression
+gzip compressed data, was "superannotate_databricks_connector-0.0.2.dev1.tar", last modified: Wed Jul 12 14:48:13 2023, max compression
```

## Comparing `superannotate_databricks_connector-0.0.1.dev2.tar` & `superannotate_databricks_connector-0.0.2.dev1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 05:56:02.733801 superannotate_databricks_connector-0.0.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-06-28 05:56:02.733801 superannotate_databricks_connector-0.0.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-28 05:56:02.733801 superannotate_databricks_connector-0.0.1.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 05:56:02.725800 superannotate_databricks_connector-0.0.1.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 05:56:02.729800 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 05:56:02.729800 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/comment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2803 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/shapes.py
--rw-r--r--   0 runner    (1001) docker     (122)      898 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/tag.py
--rw-r--r--   0 runner    (1001) docker     (122)     1875 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/text_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2673 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/vector_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/video_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/text.py
--rw-r--r--   0 runner    (1001) docker     (122)     6218 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 05:56:02.729800 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-06-28 05:56:02.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      939 2023-06-28 05:56:02.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-28 05:56:02.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-28 05:56:02.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-28 05:56:02.000000 superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 05:56:02.729800 superannotate_databricks_connector-0.0.1.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-06-28 05:55:50.000000 superannotate_databricks_connector-0.0.1.dev2/tests/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:48:13.659658 superannotate_databricks_connector-0.0.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3931 2023-07-12 14:48:13.655658 superannotate_databricks_connector-0.0.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 14:48:13.659658 superannotate_databricks_connector-0.0.2.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:48:13.651657 superannotate_databricks_connector-0.0.2.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:48:13.651657 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:48:13.655658 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/comment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2803 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      898 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1875 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/text_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2673 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/vector_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6218 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:48:13.655658 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3931 2023-07-12 14:48:13.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-12 14:48:13.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 14:48:13.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-12 14:48:13.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-07-12 14:48:13.000000 superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 14:48:13.655658 superannotate_databricks_connector-0.0.2.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-07-12 14:48:02.000000 superannotate_databricks_connector-0.0.2.dev1/tests/test_vector.py
```

### Comparing `superannotate_databricks_connector-0.0.1.dev2/LICENSE.txt` & `superannotate_databricks_connector-0.0.2.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superannotate_databricks_connector-0.0.1.dev2/pyproject.toml` & `superannotate_databricks_connector-0.0.2.dev1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 
-name = "superannotate_databricks_connector"  # Required
+name = "superannotate_databricks_connector"  
 
-version = "0.0.1dev2"
+version = "0.0.2dev1"
 
 description = "Custom functions to work with SuperAnnotate in Databricks"
 
-readme = "README.md"
+readme = "readme.md"
 
 requires-python = ">=3.8"
 
 license = { file = "LICENSE.txt" }
 
 keywords = ["superannotate_databricks_connector", "superannotate"]
```

### Comparing `superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/comment.py` & `superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/comment.py`

 * *Files identical despite different names*

### Comparing `superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/shapes.py` & `superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/shapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         StructField("x1", FloatType(), True),
         StructField("y1", FloatType(), True),
         StructField("x2", FloatType(), True),
         StructField("y2", FloatType(), True),
         StructField("x3", FloatType(), True),
         StructField("y3", FloatType(), True),
         StructField("x4", FloatType(), True),
-        StructField("y5", FloatType(), True)
+        StructField("y4", FloatType(), True)
     ])
 
 
 def get_point_schema():
     """
     Defines the schema of a point
 
@@ -91,15 +91,15 @@
     Returns:
         StructType: Schema of an ellipse
     """
     return StructType([
         StructField("cx", FloatType(), True),
         StructField("cy", FloatType(), True),
         StructField("rx", FloatType(), True),
-        StructField("ty", FloatType(), True),
+        StructField("ry", FloatType(), True),
         StructField("angle", FloatType(), True)
     ])
 
 
 def get_polygon_schema():
     """
     Defines the schema of a polygon. It contains a shell as well
```

### Comparing `superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/tag.py` & `superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/tag.py`

 * *Files identical despite different names*

### Comparing `superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/text_schema.py` & `superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/text_schema.py`

 * *Files identical despite different names*

### Comparing `superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/schemas/vector_schema.py` & `superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/schemas/vector_schema.py`

 * *Files identical despite different names*

### Comparing `superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/text.py` & `superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/text.py`

 * *Files identical despite different names*

### Comparing `superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector/vector.py` & `superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector/vector.py`

 * *Files identical despite different names*

### Comparing `superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector.egg-info/PKG-INFO` & `superannotate_databricks_connector-0.0.2.dev1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: superannotate-databricks-connector
-Version: 0.0.1.dev2
+Name: superannotate_databricks_connector
+Version: 0.0.2.dev1
 Summary: Custom functions to work with SuperAnnotate in Databricks
 Author-email: Leo Lindén <leo@superannotate.com>
 Maintainer-email: Leo Lindén <leo@superannotate.com>
 License: MIT License
         
         Copyright (c) 2023 SuperAnnotate AI Inc.
         
@@ -38,7 +38,69 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
+
+# Superannotate Databricks Connector
+SuperAnnotate is the cornerstone of your data labeling pipeline. It brings you a cutting-edge annotation tool for all types of data including image, video, text, LiDAR, audio, and more.
+
+This Python package provides a set of utilities for working with SuperAnnotate data on Databricks. It includes functionality to process SuperAnnotate data and save it to Delta tables.
+
+
+### Features
+Convert superannotate annotation data to Apache Spark&trade; Data Frames. 
+Project types supported:
+    - Vector
+    - Text
+
+
+
+### Example notebooks.
+Copy the notebooks in the demo folder to your databricks workspace to get started with SuperAnnotate quickly!
+
+### Installation
+```bash
+pip install superannotate_databricks_connector
+``` 
+
+### Tests
+
+Run tests by building the Dockerfile.test file using
+
+```bash
+docker build -f Dockerfile.test -t test_package .
+```
+
+If you are running the tests for the first you first have to build the base dockerfile containing pyspark.
+
+```bash
+docker build -f Dockerfile.spark -t spark_docker_base .
+```
+
+### Build package
+
+In the main directory, run the following to generate a .whl file. 
+
+```bash
+python -m build
+```
+
+### Usage
+First import the required function
+
+```python
+from superannotate_databricks_conector.vector import get_vector_dataframe
+from superannotate import SAClient
+```
+
+You can then convert your annotations to a spark dataframe
+
+```python
+sa = SAClient(token="<TOKEN>")
+annotations = sa.get_annotations("<PROJECT_NAME>)
+df = get_vector_dataframe(annotations, spark)
+```
+
+
```

### Comparing `superannotate_databricks_connector-0.0.1.dev2/src/superannotate_databricks_connector.egg-info/SOURCES.txt` & `superannotate_databricks_connector-0.0.2.dev1/src/superannotate_databricks_connector.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE.txt
 pyproject.toml
+readme.md
 src/superannotate_databricks_connector/__init__.py
 src/superannotate_databricks_connector/text.py
 src/superannotate_databricks_connector/vector.py
 src/superannotate_databricks_connector.egg-info/PKG-INFO
 src/superannotate_databricks_connector.egg-info/SOURCES.txt
 src/superannotate_databricks_connector.egg-info/dependency_links.txt
 src/superannotate_databricks_connector.egg-info/requires.txt
 src/superannotate_databricks_connector.egg-info/top_level.txt
 src/superannotate_databricks_connector/schemas/__init__.py
 src/superannotate_databricks_connector/schemas/comment.py
 src/superannotate_databricks_connector/schemas/shapes.py
 src/superannotate_databricks_connector/schemas/tag.py
 src/superannotate_databricks_connector/schemas/text_schema.py
 src/superannotate_databricks_connector/schemas/vector_schema.py
-src/superannotate_databricks_connector/schemas/video_schema.py
 tests/test_text.py
 tests/test_vector.py
```

### Comparing `superannotate_databricks_connector-0.0.1.dev2/tests/test_text.py` & `superannotate_databricks_connector-0.0.2.dev1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `superannotate_databricks_connector-0.0.1.dev2/tests/test_vector.py` & `superannotate_databricks_connector-0.0.2.dev1/tests/test_vector.py`

 * *Files identical despite different names*

