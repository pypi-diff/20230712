# Comparing `tmp/capsulecorp-0.1.1.tar.gz` & `tmp/capsulecorp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsulecorp-0.1.1.tar", last modified: Mon Jul 10 20:52:32 2023, max compression
+gzip compressed data, was "capsulecorp-0.1.2.tar", last modified: Wed Jul 12 13:54:57 2023, max compression
```

## Comparing `capsulecorp-0.1.1.tar` & `capsulecorp-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-10 20:52:32.645699 capsulecorp-0.1.1/
--rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.1/LICENSE
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-10 20:52:32.645088 capsulecorp-0.1.1/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.1/README.md
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-10 20:52:32.635673 capsulecorp-0.1.1/capsulecorp/
--rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.1/capsulecorp/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.1/capsulecorp/query_driver.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-10 20:52:32.643778 capsulecorp-0.1.1/capsulecorp/utilities/
--rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-10 14:36:34.000000 capsulecorp-0.1.1/capsulecorp/utilities/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     5882 2023-07-10 18:54:59.000000 capsulecorp-0.1.1/capsulecorp/utilities/databricks_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.1/capsulecorp/utilities/github_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.1/capsulecorp/utilities/slack_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.1/capsulecorp/utils.py
--rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-10 18:42:39.000000 capsulecorp-0.1.1/capsulecorp/version.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-10 20:52:32.639756 capsulecorp-0.1.1/capsulecorp.egg-info/
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-10 20:52:31.000000 capsulecorp-0.1.1/capsulecorp.egg-info/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-10 20:52:32.000000 capsulecorp-0.1.1/capsulecorp.egg-info/SOURCES.txt
--rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-10 20:52:31.000000 capsulecorp-0.1.1/capsulecorp.egg-info/dependency_links.txt
--rw-r--r--   0 daless383   (502) staff       (20)      100 2023-07-10 20:52:32.000000 capsulecorp-0.1.1/capsulecorp.egg-info/requires.txt
--rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-10 20:52:32.000000 capsulecorp-0.1.1/capsulecorp.egg-info/top_level.txt
--rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.1/pyproject.toml
--rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-10 20:52:32.645848 capsulecorp-0.1.1/setup.cfg
--rw-r--r--   0 daless383   (502) staff       (20)     6604 2023-07-10 18:43:29.000000 capsulecorp-0.1.1/setup.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-12 13:54:57.441418 capsulecorp-0.1.2/
+-rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.2/LICENSE
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-12 13:54:57.440772 capsulecorp-0.1.2/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.2/README.md
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-12 13:54:57.429823 capsulecorp-0.1.2/capsulecorp/
+-rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.2/capsulecorp/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.2/capsulecorp/query_driver.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-12 13:54:57.439509 capsulecorp-0.1.2/capsulecorp/utilities/
+-rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-10 14:36:34.000000 capsulecorp-0.1.2/capsulecorp/utilities/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     5882 2023-07-10 18:54:59.000000 capsulecorp-0.1.2/capsulecorp/utilities/databricks_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.2/capsulecorp/utilities/github_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.2/capsulecorp/utilities/slack_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.2/capsulecorp/utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-12 13:53:46.000000 capsulecorp-0.1.2/capsulecorp/version.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-12 13:54:57.434827 capsulecorp-0.1.2/capsulecorp.egg-info/
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-12 13:54:56.000000 capsulecorp-0.1.2/capsulecorp.egg-info/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-12 13:54:57.000000 capsulecorp-0.1.2/capsulecorp.egg-info/SOURCES.txt
+-rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-12 13:54:56.000000 capsulecorp-0.1.2/capsulecorp.egg-info/dependency_links.txt
+-rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-12 13:54:57.000000 capsulecorp-0.1.2/capsulecorp.egg-info/requires.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-12 13:54:57.000000 capsulecorp-0.1.2/capsulecorp.egg-info/top_level.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.2/pyproject.toml
+-rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-12 13:54:57.441630 capsulecorp-0.1.2/setup.cfg
+-rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.2/setup.py
```

### Comparing `capsulecorp-0.1.1/LICENSE` & `capsulecorp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.1/capsulecorp/query_driver.py` & `capsulecorp-0.1.2/capsulecorp/query_driver.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.1/capsulecorp/utilities/databricks_utils.py` & `capsulecorp-0.1.2/capsulecorp/utilities/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.1/capsulecorp/utilities/github_utils.py` & `capsulecorp-0.1.2/capsulecorp/utilities/github_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.1/capsulecorp/utilities/slack_utils.py` & `capsulecorp-0.1.2/capsulecorp/utilities/slack_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.1/capsulecorp/utils.py` & `capsulecorp-0.1.2/capsulecorp/utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.1/setup.py` & `capsulecorp-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,11 +62,12 @@
         'pandas',
         'boto3',
         'psycopg2-binary==2.9.3',
         'PyMySQL',
         'slack-sdk',
         'tabulate',
         'databricks-cli',
-        'PyGithub'
+        'PyGithub',
+        'scipy'
     ],
     include_package_data=True
 )
```

