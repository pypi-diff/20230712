# Comparing `tmp/cqlsh-expansion-0.9.2.tar.gz` & `tmp/cqlsh-expansion-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlsh-expansion-0.9.2.tar", last modified: Wed Jul 12 17:39:05 2023, max compression
+gzip compressed data, was "cqlsh-expansion-0.9.3.tar", last modified: Wed Jul 12 18:57:22 2023, max compression
```

## Comparing `cqlsh-expansion-0.9.2.tar` & `cqlsh-expansion-0.9.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 17:39:05.550827 cqlsh-expansion-0.9.2/
--rw-r--r--   0 mjraney  (197724063) staff       (20)      927 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/LICENSE.txt
--rw-r--r--   0 mjraney  (197724063) staff       (20)    10533 2023-07-12 17:39:05.551169 cqlsh-expansion-0.9.2/PKG-INFO
--rw-r--r--   0 mjraney  (197724063) staff       (20)     9363 2023-07-11 15:59:32.000000 cqlsh-expansion-0.9.2/README.md
--rw-r--r--   0 mjraney  (197724063) staff       (20)    36491 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/THIRD-PARTY-LICENSES.txt
-drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 17:39:05.523118 cqlsh-expansion-0.9.2/cqlsh_expansion/
--rw-r--r--   0 mjraney  (197724063) staff       (20)        5 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/__init__.py
--rw-r--r--   0 mjraney  (197724063) staff       (20)      240 2023-07-11 15:41:00.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/__main__.py
--rw-r--r--   0 mjraney  (197724063) staff       (20)      260 2023-07-12 15:40:19.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/__main_expansion__.py
--rw-r--r--   0 mjraney  (197724063) staff       (20)    96838 2023-07-11 15:41:00.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/cqlsh.py
--rw-r--r--   0 mjraney  (197724063) staff       (20)    98469 2023-07-12 15:40:02.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/cqlsh_expansion.py
--rw-r--r--   0 mjraney  (197724063) staff       (20)     7067 2023-07-12 00:33:19.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/cqlshrc_template
--rw-r--r--   0 mjraney  (197724063) staff       (20)     1693 2023-07-11 16:14:58.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/describe_usage.py
--rw-r--r--   0 mjraney  (197724063) staff       (20)     3965 2023-07-12 15:53:34.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/post_install.py
--rw-r--r--   0 mjraney  (197724063) staff       (20)     1468 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/sf-class2-root.crt
-drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 17:39:05.529115 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/
--rw-r--r--   0 mjraney  (197724063) staff       (20)    10533 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/PKG-INFO
--rw-r--r--   0 mjraney  (197724063) staff       (20)      984 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/SOURCES.txt
--rw-r--r--   0 mjraney  (197724063) staff       (20)        1 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/dependency_links.txt
--rw-r--r--   0 mjraney  (197724063) staff       (20)      197 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/entry_points.txt
--rw-r--r--   0 mjraney  (197724063) staff       (20)       63 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/requires.txt
--rw-r--r--   0 mjraney  (197724063) staff       (20)       25 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/top_level.txt
-drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 17:39:05.549950 cqlsh-expansion-0.9.2/cqlshlib/
--rw-rw-r--   0 mjraney  (197724063) staff       (20)      784 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/__init__.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)     7078 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/authproviderhandling.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)   113089 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/copyutil.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)    58090 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/cql3handling.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)    13103 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/cqlhandling.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)    10454 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/cqlshhandling.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)    18263 2023-07-07 13:28:31.000000 cqlsh-expansion-0.9.2/cqlshlib/describe_function3x.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)     3977 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/displaying.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)    23471 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/formatting.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)     4524 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/helptopics.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)    18528 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/pylexotron.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)     4167 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/saferscanner.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)     3739 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/sslhandling.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)     3403 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/tracing.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)     5057 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/util.py
--rw-rw-r--   0 mjraney  (197724063) staff       (20)    15865 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/wcwidth.py
--rw-r--r--   0 mjraney  (197724063) staff       (20)     1356 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/pyproject.toml
--rw-r--r--   0 mjraney  (197724063) staff       (20)      106 2023-07-12 17:39:05.552198 cqlsh-expansion-0.9.2/setup.cfg
--rw-r--r--   0 mjraney  (197724063) staff       (20)     2024 2023-07-12 17:37:49.000000 cqlsh-expansion-0.9.2/setup.py
+drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 18:57:22.603635 cqlsh-expansion-0.9.3/
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      927 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.3/LICENSE.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    10533 2023-07-12 18:57:22.604177 cqlsh-expansion-0.9.3/PKG-INFO
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     9363 2023-07-11 15:59:32.000000 cqlsh-expansion-0.9.3/README.md
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    36491 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.3/THIRD-PARTY-LICENSES.txt
+drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 18:57:22.574426 cqlsh-expansion-0.9.3/cqlsh_expansion/
+-rw-r--r--   0 mjraney  (197724063) staff       (20)        5 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.3/cqlsh_expansion/__init__.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      240 2023-07-11 15:41:00.000000 cqlsh-expansion-0.9.3/cqlsh_expansion/__main__.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      260 2023-07-12 15:40:19.000000 cqlsh-expansion-0.9.3/cqlsh_expansion/__main_expansion__.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    96838 2023-07-11 15:41:00.000000 cqlsh-expansion-0.9.3/cqlsh_expansion/cqlsh.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    98469 2023-07-12 15:40:02.000000 cqlsh-expansion-0.9.3/cqlsh_expansion/cqlsh_expansion.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     7067 2023-07-12 00:33:19.000000 cqlsh-expansion-0.9.3/cqlsh_expansion/cqlshrc_template
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     1693 2023-07-11 16:14:58.000000 cqlsh-expansion-0.9.3/cqlsh_expansion/describe_usage.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     3965 2023-07-12 15:53:34.000000 cqlsh-expansion-0.9.3/cqlsh_expansion/post_install.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     1468 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.3/cqlsh_expansion/sf-class2-root.crt
+drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 18:57:22.579427 cqlsh-expansion-0.9.3/cqlsh_expansion.egg-info/
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    10533 2023-07-12 18:57:22.000000 cqlsh-expansion-0.9.3/cqlsh_expansion.egg-info/PKG-INFO
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      984 2023-07-12 18:57:22.000000 cqlsh-expansion-0.9.3/cqlsh_expansion.egg-info/SOURCES.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)        1 2023-07-12 18:57:22.000000 cqlsh-expansion-0.9.3/cqlsh_expansion.egg-info/dependency_links.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      197 2023-07-12 18:57:22.000000 cqlsh-expansion-0.9.3/cqlsh_expansion.egg-info/entry_points.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)       58 2023-07-12 18:57:22.000000 cqlsh-expansion-0.9.3/cqlsh_expansion.egg-info/requires.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)       25 2023-07-12 18:57:22.000000 cqlsh-expansion-0.9.3/cqlsh_expansion.egg-info/top_level.txt
+drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 18:57:22.602507 cqlsh-expansion-0.9.3/cqlshlib/
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)      784 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/__init__.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     7078 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/authproviderhandling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)   113089 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/copyutil.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    58090 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/cql3handling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    13103 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/cqlhandling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    10454 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/cqlshhandling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    18263 2023-07-07 13:28:31.000000 cqlsh-expansion-0.9.3/cqlshlib/describe_function3x.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     3977 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/displaying.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    23471 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/formatting.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     4524 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/helptopics.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    18528 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/pylexotron.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     4167 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/saferscanner.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     3739 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/sslhandling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     3403 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/tracing.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     5057 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/util.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    15865 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.3/cqlshlib/wcwidth.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     1356 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.3/pyproject.toml
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      106 2023-07-12 18:57:22.605585 cqlsh-expansion-0.9.3/setup.cfg
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     2019 2023-07-12 18:53:50.000000 cqlsh-expansion-0.9.3/setup.py
```

### Comparing `cqlsh-expansion-0.9.2/LICENSE.txt` & `cqlsh-expansion-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/PKG-INFO` & `cqlsh-expansion-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqlsh-expansion
-Version: 0.9.2
+Version: 0.9.3
 Summary: The cqlsh-expansion utility extends native cqlsh functionality to include cloud native capabilities
 Home-page: https://github.com/aws-samples/amazon-keyspaces-toolkit/tree/master/cqlsh-expansion
 Author: Michael Raney, Sri Rathan Rangisetti
 Keywords: cql,cqlsh,cqlsh-expansion,aws,keyspaces,cassandra,sigv4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cqlsh-expansion-0.9.2/README.md` & `cqlsh-expansion-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/THIRD-PARTY-LICENSES.txt` & `cqlsh-expansion-0.9.3/THIRD-PARTY-LICENSES.txt`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlsh_expansion/cqlsh.py` & `cqlsh-expansion-0.9.3/cqlsh_expansion/cqlsh.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlsh_expansion/cqlsh_expansion.py` & `cqlsh-expansion-0.9.3/cqlsh_expansion/cqlsh_expansion.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlsh_expansion/cqlshrc_template` & `cqlsh-expansion-0.9.3/cqlsh_expansion/cqlshrc_template`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlsh_expansion/describe_usage.py` & `cqlsh-expansion-0.9.3/cqlsh_expansion/describe_usage.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlsh_expansion/post_install.py` & `cqlsh-expansion-0.9.3/cqlsh_expansion/post_install.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlsh_expansion/sf-class2-root.crt` & `cqlsh-expansion-0.9.3/cqlsh_expansion/sf-class2-root.crt`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/PKG-INFO` & `cqlsh-expansion-0.9.3/cqlsh_expansion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqlsh-expansion
-Version: 0.9.2
+Version: 0.9.3
 Summary: The cqlsh-expansion utility extends native cqlsh functionality to include cloud native capabilities
 Home-page: https://github.com/aws-samples/amazon-keyspaces-toolkit/tree/master/cqlsh-expansion
 Author: Michael Raney, Sri Rathan Rangisetti
 Keywords: cql,cqlsh,cqlsh-expansion,aws,keyspaces,cassandra,sigv4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/SOURCES.txt` & `cqlsh-expansion-0.9.3/cqlsh_expansion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/__init__.py` & `cqlsh-expansion-0.9.3/cqlshlib/__init__.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/authproviderhandling.py` & `cqlsh-expansion-0.9.3/cqlshlib/authproviderhandling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/copyutil.py` & `cqlsh-expansion-0.9.3/cqlshlib/copyutil.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/cql3handling.py` & `cqlsh-expansion-0.9.3/cqlshlib/cql3handling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/cqlhandling.py` & `cqlsh-expansion-0.9.3/cqlshlib/cqlhandling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/cqlshhandling.py` & `cqlsh-expansion-0.9.3/cqlshlib/cqlshhandling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/describe_function3x.py` & `cqlsh-expansion-0.9.3/cqlshlib/describe_function3x.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/displaying.py` & `cqlsh-expansion-0.9.3/cqlshlib/displaying.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/formatting.py` & `cqlsh-expansion-0.9.3/cqlshlib/formatting.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/helptopics.py` & `cqlsh-expansion-0.9.3/cqlshlib/helptopics.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/pylexotron.py` & `cqlsh-expansion-0.9.3/cqlshlib/pylexotron.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/saferscanner.py` & `cqlsh-expansion-0.9.3/cqlshlib/saferscanner.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/sslhandling.py` & `cqlsh-expansion-0.9.3/cqlshlib/sslhandling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/tracing.py` & `cqlsh-expansion-0.9.3/cqlshlib/tracing.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/util.py` & `cqlsh-expansion-0.9.3/cqlshlib/util.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/cqlshlib/wcwidth.py` & `cqlsh-expansion-0.9.3/cqlshlib/wcwidth.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/pyproject.toml` & `cqlsh-expansion-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.2/setup.py` & `cqlsh-expansion-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # Get the long description from the README file
 long_description = (pathlib.Path(__file__).parent.resolve() / 'README.md').read_text(encoding='utf-8')
 
 
 # Setting up
 setup(
     name="cqlsh-expansion",
-    version='0.9.2',
+    version='0.9.3',
     description='The cqlsh-expansion utility extends native cqlsh functionality to include cloud native capabilities',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url = 'https://github.com/aws-samples/amazon-keyspaces-toolkit/tree/master/cqlsh-expansion',
     python_requires='>=3.6',
     install_requires=[
-        "six>1.14.0",
+        "six>=1.12.0",
         "cassandra-driver",
-        "boto3>=1.16",
+        "boto3",
         "cassandra-sigv4>=4.0.2",
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
```

