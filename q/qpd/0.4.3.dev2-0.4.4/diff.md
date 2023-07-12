# Comparing `tmp/qpd-0.4.3.dev2.tar.gz` & `tmp/qpd-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpd-0.4.3.dev2.tar", last modified: Tue Jun  6 17:30:53 2023, max compression
+gzip compressed data, was "qpd-0.4.4.tar", last modified: Wed Jul 12 05:46:27 2023, max compression
```

## Comparing `qpd-0.4.3.dev2.tar` & `qpd-0.4.4.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.151713 qpd-0.4.3.dev2/_qpd_antlr/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/_qpd_antlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98636 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/_qpd_antlr/sqlLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)   785012 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/_qpd_antlr/sqlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    46840 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/_qpd_antlr/sqlVisitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/qpd/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/qpd/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/_parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/_parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38946 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/_parser/visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/qpd_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/qpd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-06 17:30:53.000000 qpd-0.4.3.dev2/qpd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-06 17:30:53.000000 qpd-0.4.3.dev2/qpd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:30:53.000000 qpd-0.4.3.dev2/qpd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-06 17:30:53.000000 qpd-0.4.3.dev2/qpd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 17:30:53.000000 qpd-0.4.3.dev2/qpd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/qpd_dask/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_dask/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/qpd_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_pandas/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/qpd_ray/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25424 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_ray/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/qpd_test/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_test/benchmark_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    51754 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_test/engine_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_test/sql_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_test/tests_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/qpd_version/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/qpd_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-06 17:30:53.155713 qpd-0.4.3.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-06 17:30:13.000000 qpd-0.4.3.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.601381 qpd-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 05:45:42.000000 qpd-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-12 05:46:27.601381 qpd-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-07-12 05:45:42.000000 qpd-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.597381 qpd-0.4.4/_qpd_antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-12 05:45:42.000000 qpd-0.4.4/_qpd_antlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98636 2023-07-12 05:45:42.000000 qpd-0.4.4/_qpd_antlr/sqlLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   785012 2023-07-12 05:45:42.000000 qpd-0.4.4/_qpd_antlr/sqlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46840 2023-07-12 05:45:42.000000 qpd-0.4.4/_qpd_antlr/sqlVisitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.597381 qpd-0.4.4/qpd/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.601381 qpd-0.4.4/qpd/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/_parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/_parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38946 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/_parser/visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/qpd_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.597381 qpd-0.4.4/qpd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-12 05:46:27.000000 qpd-0.4.4/qpd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-12 05:46:27.000000 qpd-0.4.4/qpd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:46:27.000000 qpd-0.4.4/qpd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 05:46:27.000000 qpd-0.4.4/qpd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 05:46:27.000000 qpd-0.4.4/qpd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.601381 qpd-0.4.4/qpd_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_dask/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.601381 qpd-0.4.4/qpd_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_pandas/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.601381 qpd-0.4.4/qpd_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25424 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_ray/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.601381 qpd-0.4.4/qpd_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_test/benchmark_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51754 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_test/engine_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_test/sql_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_test/tests_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:46:27.601381 qpd-0.4.4/qpd_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 05:45:42.000000 qpd-0.4.4/qpd_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-12 05:46:27.601381 qpd-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-12 05:45:42.000000 qpd-0.4.4/setup.py
```

### Comparing `qpd-0.4.3.dev2/LICENSE` & `qpd-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/PKG-INFO` & `qpd-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpd
-Version: 0.4.3.dev2
+Version: 0.4.4
 Summary: Query Pandas Using SQL
 Home-page: http://github.com/goodwanghan/qpd
 Author: Han Wang
 Author-email: goodwanghan@gmail.com
 License: Apache-2.0
 Description: # Query Pandas-like Dataframes Using SQL
         
@@ -119,14 +119,15 @@
         be guaranteed, but there will be no performance advantage. So for Spark, please use Spark SQL.
         If you use Fugue SQL on Spark backend, it will also directly use Spark to run the SQL statements.
         We don't see the value to make QPD run on Spark.
         
         
         ## Update History
         
+        * 0.4.4: Remove triad version constraint
         * 0.4.3: Fix packing issue
         * 0.4.2: Refactor to use the latest triad, fix packaging issues
         * 0.4.1: Make Pandas 2 compatible
         * 0.4.0: Support arbitrary column name
         * 0.2.6: Update pandas indexer import
         * 0.2.5: Update antlr to 4.9
         * 0.2.4: Fix a bug: set operations will alter the input dataframe to add columns
```

### Comparing `qpd-0.4.3.dev2/README.md` & `qpd-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 be guaranteed, but there will be no performance advantage. So for Spark, please use Spark SQL.
 If you use Fugue SQL on Spark backend, it will also directly use Spark to run the SQL statements.
 We don't see the value to make QPD run on Spark.
 
 
 ## Update History
 
+* 0.4.4: Remove triad version constraint
 * 0.4.3: Fix packing issue
 * 0.4.2: Refactor to use the latest triad, fix packaging issues
 * 0.4.1: Make Pandas 2 compatible
 * 0.4.0: Support arbitrary column name
 * 0.2.6: Update pandas indexer import
 * 0.2.5: Update antlr to 4.9
 * 0.2.4: Fix a bug: set operations will alter the input dataframe to add columns
```

### Comparing `qpd-0.4.3.dev2/_qpd_antlr/sqlLexer.py` & `qpd-0.4.4/_qpd_antlr/sqlLexer.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/_qpd_antlr/sqlParser.py` & `qpd-0.4.4/_qpd_antlr/sqlParser.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/_qpd_antlr/sqlVisitor.py` & `qpd-0.4.4/_qpd_antlr/sqlVisitor.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd/_parser/sql.py` & `qpd-0.4.4/qpd/_parser/sql.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd/_parser/utils.py` & `qpd-0.4.4/qpd/_parser/utils.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd/_parser/visitors.py` & `qpd-0.4.4/qpd/_parser/visitors.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd/constants.py` & `qpd-0.4.4/qpd/constants.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd/dataframe.py` & `qpd-0.4.4/qpd/dataframe.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd/qpd_engine.py` & `qpd-0.4.4/qpd/qpd_engine.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd/run.py` & `qpd-0.4.4/qpd/run.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd/specs.py` & `qpd-0.4.4/qpd/specs.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd/workflow.py` & `qpd-0.4.4/qpd/workflow.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd.egg-info/PKG-INFO` & `qpd-0.4.4/qpd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpd
-Version: 0.4.3.dev2
+Version: 0.4.4
 Summary: Query Pandas Using SQL
 Home-page: http://github.com/goodwanghan/qpd
 Author: Han Wang
 Author-email: goodwanghan@gmail.com
 License: Apache-2.0
 Description: # Query Pandas-like Dataframes Using SQL
         
@@ -119,14 +119,15 @@
         be guaranteed, but there will be no performance advantage. So for Spark, please use Spark SQL.
         If you use Fugue SQL on Spark backend, it will also directly use Spark to run the SQL statements.
         We don't see the value to make QPD run on Spark.
         
         
         ## Update History
         
+        * 0.4.4: Remove triad version constraint
         * 0.4.3: Fix packing issue
         * 0.4.2: Refactor to use the latest triad, fix packaging issues
         * 0.4.1: Make Pandas 2 compatible
         * 0.4.0: Support arbitrary column name
         * 0.2.6: Update pandas indexer import
         * 0.2.5: Update antlr to 4.9
         * 0.2.4: Fix a bug: set operations will alter the input dataframe to add columns
```

### Comparing `qpd-0.4.3.dev2/qpd.egg-info/SOURCES.txt` & `qpd-0.4.4/qpd.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 _qpd_antlr/__init__.py
 _qpd_antlr/sqlLexer.py
 _qpd_antlr/sqlParser.py
 _qpd_antlr/sqlVisitor.py
 qpd/__init__.py
 qpd/constants.py
 qpd/dataframe.py
+qpd/py.typed
 qpd/qpd_engine.py
 qpd/run.py
 qpd/specs.py
 qpd/workflow.py
 qpd.egg-info/PKG-INFO
 qpd.egg-info/SOURCES.txt
 qpd.egg-info/dependency_links.txt
```

### Comparing `qpd-0.4.3.dev2/qpd_dask/engine.py` & `qpd-0.4.4/qpd_dask/engine.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd_pandas/engine.py` & `qpd-0.4.4/qpd_pandas/engine.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd_ray/engine.py` & `qpd-0.4.4/qpd_ray/engine.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd_test/benchmark_suite.py` & `qpd-0.4.4/qpd_test/benchmark_suite.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd_test/engine_suite.py` & `qpd-0.4.4/qpd_test/engine_suite.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd_test/sql_suite.py` & `qpd-0.4.4/qpd_test/sql_suite.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd_test/tests_base.py` & `qpd-0.4.4/qpd_test/tests_base.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/qpd_test/utils.py` & `qpd-0.4.4/qpd_test/utils.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.3.dev2/setup.py` & `qpd-0.4.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,28 @@
     license="Apache-2.0",
     author="Han Wang",
     author_email="goodwanghan@gmail.com",
     keywords="pandas sql",
     url="http://github.com/goodwanghan/qpd",
     install_requires=[
         "pandas>=1.2.0",
-        "triad==0.9.0",
+        "triad>=0.9.0",
         "adagio",
         "antlr4-python3-runtime>=4.11.1,<4.12",
     ],
     extras_require={
         "dask": ["dask[dataframe,distributed]", "cloudpickle>=1.4.0"],
         # "ray": ["pandas>=1.1.2", "modin[ray]>=0.8.1.1"],
         "all": [
             "dask[dataframe,distributed]",
             "cloudpickle>=1.4.0",
             # "modin[ray]",
         ],
     },
+    package_data={"qpd": ["py.typed"]},
     classifiers=[
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
```

