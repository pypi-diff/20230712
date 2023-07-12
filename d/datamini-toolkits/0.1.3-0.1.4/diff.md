# Comparing `tmp/datamini_toolkits-0.1.3.tar.gz` & `tmp/datamini_toolkits-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamini_toolkits-0.1.3.tar", last modified: Wed Jul 12 03:11:17 2023, max compression
+gzip compressed data, was "datamini_toolkits-0.1.4.tar", last modified: Wed Jul 12 03:12:51 2023, max compression
```

## Comparing `datamini_toolkits-0.1.3.tar` & `datamini_toolkits-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:11:17.444091 datamini_toolkits-0.1.3/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:11:17.443965 datamini_toolkits-0.1.3/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 16:08:35.000000 datamini_toolkits-0.1.3/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:11:17.441677 datamini_toolkits-0.1.3/datamini_toolkits/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.3/datamini_toolkits/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:11:17.442762 datamini_toolkits-0.1.3/datamini_toolkits/cmysql/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.3/datamini_toolkits/cmysql/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      348 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.3/datamini_toolkits/cmysql/agent.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1720 2023-07-04 11:51:19.000000 datamini_toolkits-0.1.3/datamini_toolkits/cmysql/cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-07-04 11:47:35.000000 datamini_toolkits-0.1.3/datamini_toolkits/cmysql/logs.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1243 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.3/datamini_toolkits/cmysql/prompts.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:11:17.443808 datamini_toolkits-0.1.3/datamini_toolkits/mock_data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.3/datamini_toolkits/mock_data/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6142 2023-07-12 03:10:09.000000 datamini_toolkits-0.1.3/datamini_toolkits/mock_data/agent.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1616 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.3/datamini_toolkits/mock_data/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2609 2023-07-12 03:10:51.000000 datamini_toolkits-0.1.3/datamini_toolkits/mock_data/cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.3/datamini_toolkits/mock_data/logs.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.3/datamini_toolkits/mock_data/prompts.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.3/datamini_toolkits/mock_data/test_tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.3/datamini_toolkits/mock_data/tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.3/datamini_toolkits/tests.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:11:17.442243 datamini_toolkits-0.1.3/datamini_toolkits.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:11:17.000000 datamini_toolkits-0.1.3/datamini_toolkits.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      757 2023-07-12 03:11:17.000000 datamini_toolkits-0.1.3/datamini_toolkits.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-07-12 03:11:17.000000 datamini_toolkits-0.1.3/datamini_toolkits.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      115 2023-07-12 03:11:17.000000 datamini_toolkits-0.1.3/datamini_toolkits.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-07-12 03:11:17.000000 datamini_toolkits-0.1.3/datamini_toolkits.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-07-12 03:11:17.444125 datamini_toolkits-0.1.3/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2023-07-12 03:11:16.000000 datamini_toolkits-0.1.3/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:12:51.168791 datamini_toolkits-0.1.4/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:12:51.168645 datamini_toolkits-0.1.4/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 16:08:35.000000 datamini_toolkits-0.1.4/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:12:51.165203 datamini_toolkits-0.1.4/datamini_toolkits/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.4/datamini_toolkits/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:12:51.166436 datamini_toolkits-0.1.4/datamini_toolkits/cmysql/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.4/datamini_toolkits/cmysql/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      348 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.4/datamini_toolkits/cmysql/agent.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1720 2023-07-04 11:51:19.000000 datamini_toolkits-0.1.4/datamini_toolkits/cmysql/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-07-04 11:47:35.000000 datamini_toolkits-0.1.4/datamini_toolkits/cmysql/logs.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1243 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.4/datamini_toolkits/cmysql/prompts.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:12:51.168309 datamini_toolkits-0.1.4/datamini_toolkits/mock_data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.4/datamini_toolkits/mock_data/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6142 2023-07-12 03:10:09.000000 datamini_toolkits-0.1.4/datamini_toolkits/mock_data/agent.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1616 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.4/datamini_toolkits/mock_data/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2608 2023-07-12 03:12:35.000000 datamini_toolkits-0.1.4/datamini_toolkits/mock_data/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.4/datamini_toolkits/mock_data/logs.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.4/datamini_toolkits/mock_data/prompts.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.4/datamini_toolkits/mock_data/test_tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.4/datamini_toolkits/mock_data/tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.4/datamini_toolkits/tests.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:12:51.165855 datamini_toolkits-0.1.4/datamini_toolkits.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:12:51.000000 datamini_toolkits-0.1.4/datamini_toolkits.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      757 2023-07-12 03:12:51.000000 datamini_toolkits-0.1.4/datamini_toolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-07-12 03:12:51.000000 datamini_toolkits-0.1.4/datamini_toolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      115 2023-07-12 03:12:51.000000 datamini_toolkits-0.1.4/datamini_toolkits.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-07-12 03:12:51.000000 datamini_toolkits-0.1.4/datamini_toolkits.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-07-12 03:12:51.168834 datamini_toolkits-0.1.4/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      417 2023-07-12 03:12:44.000000 datamini_toolkits-0.1.4/setup.py
```

### Comparing `datamini_toolkits-0.1.3/README.md` & `datamini_toolkits-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/cmysql/cli.py` & `datamini_toolkits-0.1.4/datamini_toolkits/cmysql/cli.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/cmysql/logs.py` & `datamini_toolkits-0.1.4/datamini_toolkits/cmysql/logs.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/cmysql/prompts.py` & `datamini_toolkits-0.1.4/datamini_toolkits/cmysql/prompts.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/mock_data/agent.py` & `datamini_toolkits-0.1.4/datamini_toolkits/mock_data/agent.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/mock_data/base.py` & `datamini_toolkits-0.1.4/datamini_toolkits/mock_data/base.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/mock_data/cli.py` & `datamini_toolkits-0.1.4/datamini_toolkits/mock_data/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 
 import sys,os
-#sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 print(sys.path)
 from agent import DataMakerAgentCreator
 from logs import log
 
 
 def get_args():
```

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/mock_data/logs.py` & `datamini_toolkits-0.1.4/datamini_toolkits/mock_data/logs.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/mock_data/prompts.py` & `datamini_toolkits-0.1.4/datamini_toolkits/mock_data/prompts.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/mock_data/test_tools.py` & `datamini_toolkits-0.1.4/datamini_toolkits/mock_data/test_tools.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits/mock_data/tools.py` & `datamini_toolkits-0.1.4/datamini_toolkits/mock_data/tools.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.3/datamini_toolkits.egg-info/SOURCES.txt` & `datamini_toolkits-0.1.4/datamini_toolkits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

