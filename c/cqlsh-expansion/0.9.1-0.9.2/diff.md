# Comparing `tmp/cqlsh-expansion-0.9.1.tar.gz` & `tmp/cqlsh-expansion-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cqlsh-expansion-0.9.1.tar", last modified: Thu Jun  1 14:38:53 2023, max compression
+gzip compressed data, was "cqlsh-expansion-0.9.2.tar", last modified: Wed Jul 12 17:39:05 2023, max compression
```

## Comparing `cqlsh-expansion-0.9.1.tar` & `cqlsh-expansion-0.9.2.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 srirangi   (505) staff       (20)        0 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/
--rw-r--r--   0 srirangi   (505) staff       (20)      927 2021-11-22 18:22:09.000000 cqlsh-expansion-0.9.1/LICENSE.txt
--rw-r--r--   0 srirangi   (505) staff       (20)    10215 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/PKG-INFO
--rw-r--r--   0 srirangi   (505) staff       (20)     9353 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/README.md
--rw-r--r--   0 srirangi   (505) staff       (20)    36491 2023-04-03 08:57:44.000000 cqlsh-expansion-0.9.1/THIRD-PARTY-LICENSES.txt
-drwxr-xr-x   0 srirangi   (505) staff       (20)        0 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/bin/
--rwxr-xr-x   0 srirangi   (505) staff       (20)     3062 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/bin/cqlsh
--rwxr-xr-x   0 srirangi   (505) staff       (20)     3072 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/bin/cqlsh-expansion
--rwxr-xr-x   0 srirangi   (505) staff       (20)    98937 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/bin/cqlsh-expansion.py
--rw-r--r--   0 srirangi   (505) staff       (20)    96814 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/bin/cqlsh.py
-drwxr-xr-x   0 srirangi   (505) staff       (20)        0 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/config/
--rw-r--r--   0 srirangi   (505) staff       (20)        5 2021-11-22 18:22:29.000000 cqlsh-expansion-0.9.1/config/__init__.py
--rw-r--r--   0 srirangi   (505) staff       (20)     7061 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/config/cqlshrc_template
--rw-r--r--   0 srirangi   (505) staff       (20)     2418 2023-04-03 11:55:02.000000 cqlsh-expansion-0.9.1/config/post_install.py
--rw-r--r--   0 srirangi   (505) staff       (20)     1468 2021-11-22 18:22:29.000000 cqlsh-expansion-0.9.1/config/sf-class2-root.crt
-drwxr-xr-x   0 srirangi   (505) staff       (20)        0 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/cqlsh_expansion.egg-info/
--rw-r--r--   0 srirangi   (505) staff       (20)    10215 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/cqlsh_expansion.egg-info/PKG-INFO
--rw-r--r--   0 srirangi   (505) staff       (20)      983 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/cqlsh_expansion.egg-info/SOURCES.txt
--rw-r--r--   0 srirangi   (505) staff       (20)        1 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/cqlsh_expansion.egg-info/dependency_links.txt
--rw-r--r--   0 srirangi   (505) staff       (20)       92 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/cqlsh_expansion.egg-info/entry_points.txt
--rw-r--r--   0 srirangi   (505) staff       (20)      114 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/cqlsh_expansion.egg-info/requires.txt
--rw-r--r--   0 srirangi   (505) staff       (20)       16 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/cqlsh_expansion.egg-info/top_level.txt
-drwxr-xr-x   0 srirangi   (505) staff       (20)        0 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/pylib/
-drwxr-xr-x   0 srirangi   (505) staff       (20)        0 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/
--rw-r--r--   0 srirangi   (505) staff       (20)      784 2023-04-03 09:08:39.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/__init__.py
--rw-r--r--   0 srirangi   (505) staff       (20)     7078 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/authproviderhandling.py
--rw-r--r--   0 srirangi   (505) staff       (20)   113001 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/copyutil.py
--rw-r--r--   0 srirangi   (505) staff       (20)    58090 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/cql3handling.py
--rw-r--r--   0 srirangi   (505) staff       (20)    13103 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/cqlhandling.py
--rw-r--r--   0 srirangi   (505) staff       (20)    10454 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/cqlshhandling.py
--rw-r--r--   0 srirangi   (505) staff       (20)     3977 2023-04-03 09:08:39.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/displaying.py
--rw-r--r--   0 srirangi   (505) staff       (20)    23470 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/formatting.py
--rw-r--r--   0 srirangi   (505) staff       (20)     4524 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/helptopics.py
--rw-r--r--   0 srirangi   (505) staff       (20)     8628 2023-06-01 14:35:23.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/legacydesc3x.py
--rw-r--r--   0 srirangi   (505) staff       (20)    18528 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/pylexotron.py
--rw-r--r--   0 srirangi   (505) staff       (20)     3429 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/saferscanner.py
--rw-r--r--   0 srirangi   (505) staff       (20)     3739 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/sslhandling.py
--rw-r--r--   0 srirangi   (505) staff       (20)     3403 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/tracing.py
--rw-r--r--   0 srirangi   (505) staff       (20)     5057 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/util.py
--rw-r--r--   0 srirangi   (505) staff       (20)    15865 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/pylib/cqlshlib/wcwidth.py
--rw-r--r--   0 srirangi   (505) staff       (20)     1356 2021-11-22 18:22:10.000000 cqlsh-expansion-0.9.1/pyproject.toml
--rw-r--r--   0 srirangi   (505) staff       (20)      973 2023-06-01 14:38:53.000000 cqlsh-expansion-0.9.1/setup.cfg
--rw-r--r--   0 srirangi   (505) staff       (20)      695 2023-05-17 17:23:50.000000 cqlsh-expansion-0.9.1/setup.py
+drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 17:39:05.550827 cqlsh-expansion-0.9.2/
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      927 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/LICENSE.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    10533 2023-07-12 17:39:05.551169 cqlsh-expansion-0.9.2/PKG-INFO
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     9363 2023-07-11 15:59:32.000000 cqlsh-expansion-0.9.2/README.md
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    36491 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/THIRD-PARTY-LICENSES.txt
+drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 17:39:05.523118 cqlsh-expansion-0.9.2/cqlsh_expansion/
+-rw-r--r--   0 mjraney  (197724063) staff       (20)        5 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/__init__.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      240 2023-07-11 15:41:00.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/__main__.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      260 2023-07-12 15:40:19.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/__main_expansion__.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    96838 2023-07-11 15:41:00.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/cqlsh.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    98469 2023-07-12 15:40:02.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/cqlsh_expansion.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     7067 2023-07-12 00:33:19.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/cqlshrc_template
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     1693 2023-07-11 16:14:58.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/describe_usage.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     3965 2023-07-12 15:53:34.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/post_install.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     1468 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/cqlsh_expansion/sf-class2-root.crt
+drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 17:39:05.529115 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/
+-rw-r--r--   0 mjraney  (197724063) staff       (20)    10533 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/PKG-INFO
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      984 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/SOURCES.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)        1 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/dependency_links.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      197 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/entry_points.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)       63 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/requires.txt
+-rw-r--r--   0 mjraney  (197724063) staff       (20)       25 2023-07-12 17:39:05.000000 cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/top_level.txt
+drwxr-xr-x   0 mjraney  (197724063) staff       (20)        0 2023-07-12 17:39:05.549950 cqlsh-expansion-0.9.2/cqlshlib/
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)      784 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/__init__.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     7078 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/authproviderhandling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)   113089 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/copyutil.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    58090 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/cql3handling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    13103 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/cqlhandling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    10454 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/cqlshhandling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    18263 2023-07-07 13:28:31.000000 cqlsh-expansion-0.9.2/cqlshlib/describe_function3x.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     3977 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/displaying.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    23471 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/formatting.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     4524 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/helptopics.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    18528 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/pylexotron.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     4167 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/saferscanner.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     3739 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/sslhandling.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     3403 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/tracing.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)     5057 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/util.py
+-rw-rw-r--   0 mjraney  (197724063) staff       (20)    15865 2023-07-05 15:08:20.000000 cqlsh-expansion-0.9.2/cqlshlib/wcwidth.py
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     1356 2021-12-09 21:36:37.000000 cqlsh-expansion-0.9.2/pyproject.toml
+-rw-r--r--   0 mjraney  (197724063) staff       (20)      106 2023-07-12 17:39:05.552198 cqlsh-expansion-0.9.2/setup.cfg
+-rw-r--r--   0 mjraney  (197724063) staff       (20)     2024 2023-07-12 17:37:49.000000 cqlsh-expansion-0.9.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cqlsh-expansion-0.9.1/LICENSE.txt` & `cqlsh-expansion-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/PKG-INFO` & `cqlsh-expansion-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: cqlsh-expansion
-Version: 0.9.1
-Summary: The cqlsh-expansion utility extends native cqlsh functionality to include parameters and capabilities specific to Amazon Keyspaces such as support for Sigv4 Authentication.
+Version: 0.9.2
+Summary: The cqlsh-expansion utility extends native cqlsh functionality to include cloud native capabilities
 Home-page: https://github.com/aws-samples/amazon-keyspaces-toolkit/tree/master/cqlsh-expansion
-Keywords: cql,cqlsh,cqlsh-expansion,amazon-keyspaces,ApacheCassandra
-Classifier: Development Status :: 4 - Beta
+Author: Michael Raney, Sri Rathan Rangisetti
+Keywords: cql,cqlsh,cqlsh-expansion,aws,keyspaces,cassandra,sigv4
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Requires-Python: <3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: THIRD-PARTY-LICENSES.txt
 License-File: LICENSE.txt
 
 
 # The Amazon Keyspaces (for Apache Cassandra) developer toolkit cqlsh-expansion script
 
@@ -76,20 +82,20 @@
 module = cassandra_sigv4.auth
 classname = SigV4AuthProvider
 region_name = us-east-1
 ```
 you can also set region as Environment variable
 
 ```
- export AWS_DEFAULT_REGION = us-east-1
+ export AWS_DEFAULT_REGION=us-east-1 
 ```
 
 To connect to Amazon Keyspaces with cqlsh-expansion using Sigv4 authenticator.  
 ```
-cqlsh-expansion cassandra.us-east-1.amazonaws.com 
+cqlsh-expansion cassandra.us-east-1.amazonaws.com 9142 --ssl 
 ```
 
 #### Connect with service-specific credentials
 
 You can create service-specific credentials that are similar to the traditional username and password that Cassandra uses for authentication and access management. AWS service-specific credentials are associated with a specific AWS Identity and Access Management (IAM) user and can only be used for the service they were created for. For more information, see [Using IAM with Amazon Keyspaces (for Apache Cassandra)](http://using%20iam%20with%20amazon%20keyspaces%20%28for%20apache%20cassandra%29/) in the IAM User Guide. To connect to Amazon Keyspaces using the cqlsh-expansion and IAM service-specific credentials you can use the command below. In this command we are connecting to us-east-1 region with service specific user *‘Sri-user-99’ *and service specific user password* ‘user-pass-01’. *You will need to replace these credentials with your own user name and password that were given to you when creating the service specific credentials.
```

### Comparing `cqlsh-expansion-0.9.1/README.md` & `cqlsh-expansion-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,20 +58,20 @@
 module = cassandra_sigv4.auth
 classname = SigV4AuthProvider
 region_name = us-east-1
 ```
 you can also set region as Environment variable
 
 ```
- export AWS_DEFAULT_REGION = us-east-1
+ export AWS_DEFAULT_REGION=us-east-1 
 ```
 
 To connect to Amazon Keyspaces with cqlsh-expansion using Sigv4 authenticator.  
 ```
-cqlsh-expansion cassandra.us-east-1.amazonaws.com 
+cqlsh-expansion cassandra.us-east-1.amazonaws.com 9142 --ssl 
 ```
 
 #### Connect with service-specific credentials
 
 You can create service-specific credentials that are similar to the traditional username and password that Cassandra uses for authentication and access management. AWS service-specific credentials are associated with a specific AWS Identity and Access Management (IAM) user and can only be used for the service they were created for. For more information, see [Using IAM with Amazon Keyspaces (for Apache Cassandra)](http://using%20iam%20with%20amazon%20keyspaces%20%28for%20apache%20cassandra%29/) in the IAM User Guide. To connect to Amazon Keyspaces using the cqlsh-expansion and IAM service-specific credentials you can use the command below. In this command we are connecting to us-east-1 region with service specific user *‘Sri-user-99’ *and service specific user password* ‘user-pass-01’. *You will need to replace these credentials with your own user name and password that were given to you when creating the service specific credentials.
```

### Comparing `cqlsh-expansion-0.9.1/THIRD-PARTY-LICENSES.txt` & `cqlsh-expansion-0.9.2/THIRD-PARTY-LICENSES.txt`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/bin/cqlsh-expansion.py` & `cqlsh-expansion-0.9.2/cqlsh_expansion/cqlsh_expansion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python3
+#!/usr/cqlsh_expansion/python3
 
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
@@ -32,15 +32,14 @@
 import traceback
 import warnings
 import webbrowser
 from contextlib import contextmanager
 from glob import glob
 from io import StringIO
 from uuid import UUID
-from ssl import SSLContext, PROTOCOL_TLSv1_2, CERT_REQUIRED
 
 if sys.version_info < (3, 6):
     sys.exit("\ncqlsh requires Python 3.6+\n")
 
 # see CASSANDRA-10428
 if platform.python_implementation().startswith('Jython'):
     sys.exit("\nCQL Shell does not run on Jython\n")
@@ -128,39 +127,39 @@
     sys.exit("\nPython Cassandra driver not installed, or not on PYTHONPATH.\n"
              'You might try "pip install cassandra-driver".\n\n'
              'Python: %s\n'
              'Module load path: %r\n\n'
              'Error: %s\n' % (sys.executable, sys.path, e))
 
 from cassandra.auth import PlainTextAuthProvider
-from cassandra.cluster import Cluster, ExecutionProfile, EXEC_PROFILE_DEFAULT
+from cassandra.cluster import Cluster
 from cassandra.cqltypes import cql_typename
 from cassandra.marshal import int64_unpack
 from cassandra.metadata import (ColumnMetadata, KeyspaceMetadata, TableMetadata)
 from cassandra.policies import WhiteListRoundRobinPolicy
 from cassandra.query import SimpleStatement, ordered_dict_factory, TraceUnavailable
 from cassandra.util import datetime_from_timestamp
 
 # cqlsh should run correctly when run out of a Cassandra source tree,
 # out of an unpacked Cassandra tarball, and after a proper package install.
 cqlshlibdir = os.path.join(CASSANDRA_PATH, 'pylib')
 if os.path.isdir(cqlshlibdir):
     sys.path.insert(0, cqlshlibdir)
 
-from cqlshlib import cql3handling, pylexotron, sslhandling, cqlshhandling, authproviderhandling, legacydesc3x
+from cqlshlib import cql3handling, pylexotron, sslhandling, cqlshhandling, authproviderhandling
 from cqlshlib.copyutil import ExportTask, ImportTask
 from cqlshlib.displaying import (ANSI_RESET, BLUE, COLUMN_NAME_COLORS, CYAN,
                                  RED, WHITE, FormattedValue, colorme)
 from cqlshlib.formatting import (DEFAULT_DATE_FORMAT, DEFAULT_NANOTIME_FORMAT,
                                  DEFAULT_TIMESTAMP_FORMAT, CqlType, DateTimeFormat,
                                  format_by_type)
 from cqlshlib.tracing import print_trace, print_trace_session
-from cqlshlib.util import get_file_encoding_bomsize, trim_if_present
+from cqlshlib.util import get_file_encoding_bomsize
 from cqlshlib.util import is_file_secure
-from cqlshlib.legacydesc3x import *
+from cqlshlib.describe_function3x import do_describe_3x
 
 DEFAULT_HOST = '127.0.0.1'
 DEFAULT_PORT = 9042
 DEFAULT_SSL = False
 DEFAULT_CONNECT_TIMEOUT_SECONDS = 5
 DEFAULT_REQUEST_TIMEOUT_SECONDS = 10
 
@@ -186,15 +185,15 @@
                                version='cqlsh ' + version)
 parser.add_option("-C", "--color", action='store_true', dest='color',
                   help='Always use color output')
 parser.add_option("--no-color", action='store_false', dest='color',
                   help='Never use color output')
 parser.add_option("--browser", dest='browser', help="""The browser to use to display CQL help, where BROWSER can be:
                                                     - one of the supported browsers in https://docs.python.org/3/library/webbrowser.html.
-                                                    - browser path followed by %s, example: /usr/bin/google-chrome-stable %s""")
+                                                    - browser path followed by %s, example: /usr/cqlsh_expansion/google-chrome-stable %s""")
 parser.add_option('--ssl', action='store_true', help='Use SSL', default=False)
 parser.add_option("-u", "--username", help="Authenticate as user.")
 parser.add_option("-p", "--password", help="Authenticate using password.")
 parser.add_option('-k', '--keyspace', help='Authenticate to the given keyspace.')
 parser.add_option("-f", "--file", help="Execute commands from FILE, then exit")
 parser.add_option('--debug', action='store_true',
                   help='Show additional debugging information')
@@ -472,32 +471,27 @@
                 self.auth_provider = PlainTextAuthProvider(username=auth_provider.username, password=password)
 
         self.keyspace = keyspace
         self.ssl = ssl
         self.tracing_enabled = tracing_enabled
         self.page_size = self.default_page_size
         self.expand_enabled = expand_enabled
-        Keypsaces_profile = ExecutionProfile(
-            consistency_level=cassandra.ConsistencyLevel.LOCAL_QUORUM,
-            request_timeout=request_timeout,   
-            row_factory = ordered_dict_factory,
-            load_balancing_policy=WhiteListRoundRobinPolicy([self.hostname]))
 
         if use_conn:
             self.conn = use_conn
         else:
             kwargs = {}
             if protocol_version is not None:
                 kwargs['protocol_version'] = protocol_version
             self.conn = Cluster(contact_points=(self.hostname,), port=self.port, cql_version=cqlver,
                                 auth_provider=self.auth_provider,
                                 ssl_options=sslhandling.ssl_settings(hostname, CONFIG_FILE) if ssl else None,
+                                load_balancing_policy=WhiteListRoundRobinPolicy([self.hostname]),
                                 control_connection_timeout=connect_timeout,
                                 connect_timeout=connect_timeout, 
-                                execution_profiles={EXEC_PROFILE_DEFAULT: Keypsaces_profile},
                                 **kwargs)
         self.owns_connection = not use_conn
 
 
         if keyspace:
             self.session = self.conn.connect(keyspace)
         else:
@@ -513,18 +507,17 @@
         self.display_date_format = display_date_format
 
         self.display_float_precision = display_float_precision
         self.display_double_precision = display_double_precision
 
         self.display_timezone = display_timezone
 
-        ##### These configurations are moved to EXEC_PROFILE_DEFAULT
-        # self.session.default_timeout = request_timeout
-        # self.session.row_factory = ordered_dict_factory
-        # self.session.default_consistency_level = cassandra.ConsistencyLevel.ONE
+        self.session.default_timeout = request_timeout
+        self.session.row_factory = ordered_dict_factory
+        self.session.default_consistency_level = cassandra.ConsistencyLevel.ONE
 
         self.get_connection_versions()
         self.set_expanded_cql_version(self.connection_versions['cql'])
 
         self.current_keyspace = keyspace
 
         self.max_trace_wait = max_trace_wait
@@ -633,14 +626,23 @@
         vers = {
             'build': result['release_version'],
             'protocol': self.conn.protocol_version,
             'cql': result['cql_version'],
         }
         self.connection_versions = vers
 
+    def get_keyspace_names(self):
+        return list(self.conn.metadata.keyspaces)
+
+    def get_columnfamily_names(self, ksname=None):
+        if ksname is None:
+            ksname = self.current_keyspace
+
+        return list(self.get_keyspace_meta(ksname).tables)
+
     def get_materialized_view_names(self, ksname=None):
         if ksname is None:
             ksname = self.current_keyspace
 
         return list(self.get_keyspace_meta(ksname).views)
 
     def get_index_names(self, ksname=None):
@@ -1360,24 +1362,19 @@
 
         DESCRIBE <objname>
 
           Output CQL commands that could be used to recreate the entire object schema,
           where object can be either a keyspace or a table or an index or a materialized
           view (in this order).
         """
-        """ 
-            For cqlsh > 6.0 DESCRIBE|DESC was moved to server side in Cassandra 4.0. As a consequence DESRIBE|DESC
-            will not work in cqlsh connected to Cassandra < 4.0.In cqlsh-expansion we have modified code to support describe statements for 
-            Cassandra 3.11  
-        """
         stmt = SimpleStatement(parsed.extract_orig(), consistency_level=cassandra.ConsistencyLevel.LOCAL_ONE, fetch_size=self.page_size if self.use_paging else None)
         future = self.session.execute_async(stmt)
 
         if self.connection_versions['build'][0] < '4':
-            do_describe_3x(self, parsed)
+            do_describe_3x(self, cqlruleset, parsed, self.query_out, cmd)
         else:
             try:
                 result = future.result()
                 what = parsed.matched[1][1].lower()
 
                 if what in ('columnfamilies', 'tables', 'types', 'functions', 'aggregates'):
                     self.describe_list(result)
@@ -1567,22 +1564,22 @@
         copyoptvals = list(map(self.cql_unprotect_value, parsed.get_binding('optvals', ())))
         opts = dict(list(zip(copyoptnames, copyoptvals)))
 
         direction = parsed.get_binding('dir').upper()
         if direction == 'FROM':
             self.show_consistencylevel()
             if self.consistency_level != cassandra.ConsistencyLevel.LOCAL_QUORUM:
-               raise SyntaxError("cqlsh-expansion.py 'COPY FROM' requires LOCAL_QUORUM consistency for writes")      
+               raise SyntaxError("cqlsh_expansion.py 'COPY FROM' requires LOCAL_QUORUM consistency for writes")
             task = ImportTask(self, ks, table, columns, fname, opts, self.conn.protocol_version, CONFIG_FILE)
         elif direction == 'TO':
             self.show_consistencylevel()
             if self.consistency_level != cassandra.ConsistencyLevel.LOCAL_QUORUM and \
             self.consistency_level != cassandra.ConsistencyLevel.LOCAL_ONE and \
             self.consistency_level != cassandra.ConsistencyLevel.ONE:
-               raise SyntaxError("cqlsh-expansion.py 'COPY TO' requires ONE, LOCAL_ONE, or LOCAL_QUORUM consistency for reads")            
+               raise SyntaxError("cqlsh_expansion.py 'COPY TO' requires ONE, LOCAL_ONE, or LOCAL_QUORUM consistency for reads")
             task = ExportTask(self, ks, table, columns, fname, opts, self.conn.protocol_version, CONFIG_FILE)
         else:
             raise SyntaxError("Unknown direction %s" % direction)
 
         task.run()
 
     def do_show(self, parsed):
@@ -2406,11 +2403,11 @@
         sys.exit(2)
 
 
 # always call this regardless of module name: when a sub-process is spawned
 # on Windows then the module name is not __main__, see CASSANDRA-9304 (Windows support was dropped in CASSANDRA-16956)
 insert_driver_hooks()
 
-if __name__ == '__main__':
+if __name__ == '__main_expansion__':
     main(*read_options(sys.argv[1:], os.environ))
 
-# vim: set ft=python et ts=4 sw=4 :
+# vim: set ft=python et ts=4 sw=4 :
```

### Comparing `cqlsh-expansion-0.9.1/bin/cqlsh.py` & `cqlsh-expansion-0.9.2/cqlsh_expansion/cqlsh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python3
+#!/usr/cqlsh_expansion/python3
 
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
@@ -185,15 +185,15 @@
                                version='cqlsh ' + version)
 parser.add_option("-C", "--color", action='store_true', dest='color',
                   help='Always use color output')
 parser.add_option("--no-color", action='store_false', dest='color',
                   help='Never use color output')
 parser.add_option("--browser", dest='browser', help="""The browser to use to display CQL help, where BROWSER can be:
                                                     - one of the supported browsers in https://docs.python.org/3/library/webbrowser.html.
-                                                    - browser path followed by %s, example: /usr/bin/google-chrome-stable %s""")
+                                                    - browser path followed by %s, example: /usr/cqlsh_expansion/google-chrome-stable %s""")
 parser.add_option('--ssl', action='store_true', help='Use SSL', default=False)
 parser.add_option("-u", "--username", help="Authenticate as user.")
 parser.add_option("-p", "--password", help="Authenticate using password.")
 parser.add_option('-k', '--keyspace', help='Authenticate to the given keyspace.')
 parser.add_option("-f", "--file", help="Execute commands from FILE, then exit")
 parser.add_option('--debug', action='store_true',
                   help='Show additional debugging information')
```

### Comparing `cqlsh-expansion-0.9.1/config/cqlshrc_template` & `cqlsh-expansion-0.9.2/cqlsh_expansion/cqlshrc_template`

 * *Files 2% similar despite different names*

```diff
@@ -80,18 +80,18 @@
 
 [connection]
 
 ;; The host to connect to
 hostname = 127.0.0.1
 
 ;; The port to connect to (9042 is the native protocol default)
-port = 9142
+port = 9042
 
 ;; Always connect using SSL - false by default
-ssl = true
+ssl = false
 
 ;; A timeout in seconds for opening new connections
 ; timeout = 10
 
 ;; A timeout in seconds for executing queries
 ; request_timeout = 10
 
@@ -109,15 +109,15 @@
 
 
 
 [ssl]
 certfile = ~/.cassandra/sf-class2-root.crt
 
 ;; Optional - true by default.
-;validate = true
+;validate = false
 
 ;; To be provided when require_client_auth=true
 ;userkey = ~/key.pem
 
 ;; To be provided when require_client_auth=true
 ;usercert = ~/cert.pem
 
@@ -157,15 +157,15 @@
 ;; COPY tasks.  Defaults to a max of 4 for COPY FROM and 16
 ;; for COPY TO.  However, at most (num_cores - 1) processes
 ;; will be created.
 numprocesses = 16
 
 ;; The maximum number of failed attempts to fetch a range of data (when using
 ;; COPY TO) or insert a chunk of data (when using COPY FROM) before giving up
-maxattempts = 25
+maxattempts = 1000
 
 ;; How often status updates are refreshed, in seconds
 ; reportfrequency = 0.25
 
 ;; An optional file to output rate statistics to
 ; ratefile =
 
@@ -210,15 +210,15 @@
 ;; A number of initial rows to skip
 ; skiprows = 0
 
 ;; A comma-separated list of column names to ignore
 ; skipcols =
 
 ;; The maximum global number of parsing errors to ignore, -1 means unlimited
-maxparseerrors = -1
+maxparseerrors = 1000
 
 ;; The maximum global number of insert errors to ignore, -1 means unlimited
 maxinserterrors = -1
 
 ;; A file to store all rows that could not be imported, by default this is
 ;; import_<ks>_<table>.err where <ks> is your keyspace and <table> is your table name.
 ; errfile =
```

### Comparing `cqlsh-expansion-0.9.1/config/sf-class2-root.crt` & `cqlsh-expansion-0.9.2/cqlsh_expansion/sf-class2-root.crt`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/cqlsh_expansion.egg-info/PKG-INFO` & `cqlsh-expansion-0.9.2/cqlsh_expansion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: cqlsh-expansion
-Version: 0.9.1
-Summary: The cqlsh-expansion utility extends native cqlsh functionality to include parameters and capabilities specific to Amazon Keyspaces such as support for Sigv4 Authentication.
+Version: 0.9.2
+Summary: The cqlsh-expansion utility extends native cqlsh functionality to include cloud native capabilities
 Home-page: https://github.com/aws-samples/amazon-keyspaces-toolkit/tree/master/cqlsh-expansion
-Keywords: cql,cqlsh,cqlsh-expansion,amazon-keyspaces,ApacheCassandra
-Classifier: Development Status :: 4 - Beta
+Author: Michael Raney, Sri Rathan Rangisetti
+Keywords: cql,cqlsh,cqlsh-expansion,aws,keyspaces,cassandra,sigv4
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Requires-Python: <3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: THIRD-PARTY-LICENSES.txt
 License-File: LICENSE.txt
 
 
 # The Amazon Keyspaces (for Apache Cassandra) developer toolkit cqlsh-expansion script
 
@@ -76,20 +82,20 @@
 module = cassandra_sigv4.auth
 classname = SigV4AuthProvider
 region_name = us-east-1
 ```
 you can also set region as Environment variable
 
 ```
- export AWS_DEFAULT_REGION = us-east-1
+ export AWS_DEFAULT_REGION=us-east-1 
 ```
 
 To connect to Amazon Keyspaces with cqlsh-expansion using Sigv4 authenticator.  
 ```
-cqlsh-expansion cassandra.us-east-1.amazonaws.com 
+cqlsh-expansion cassandra.us-east-1.amazonaws.com 9142 --ssl 
 ```
 
 #### Connect with service-specific credentials
 
 You can create service-specific credentials that are similar to the traditional username and password that Cassandra uses for authentication and access management. AWS service-specific credentials are associated with a specific AWS Identity and Access Management (IAM) user and can only be used for the service they were created for. For more information, see [Using IAM with Amazon Keyspaces (for Apache Cassandra)](http://using%20iam%20with%20amazon%20keyspaces%20%28for%20apache%20cassandra%29/) in the IAM User Guide. To connect to Amazon Keyspaces using the cqlsh-expansion and IAM service-specific credentials you can use the command below. In this command we are connecting to us-east-1 region with service specific user *‘Sri-user-99’ *and service specific user password* ‘user-pass-01’. *You will need to replace these credentials with your own user name and password that were given to you when creating the service specific credentials.
```

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/__init__.py` & `cqlsh-expansion-0.9.2/cqlshlib/__init__.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/authproviderhandling.py` & `cqlsh-expansion-0.9.2/cqlshlib/authproviderhandling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/copyutil.py` & `cqlsh-expansion-0.9.2/cqlshlib/copyutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,19 @@
 
 def printmsg(msg, eol='\n'):
     sys.stdout.write(msg)
     sys.stdout.write(eol)
     sys.stdout.flush()
 
 
+# Keep arguments in sync with printmsg
+def swallowmsg(msg, eol='\n'):
+    None
+
+
 class OneWayPipe(object):
     """
     A one way pipe protected by two process level locks, one for reading and one for writing.
     """
     def __init__(self):
         self.reader, self.writer = mp.Pipe(duplex=False)
         self.rlock = mp.Lock()
@@ -245,15 +250,15 @@
 
         # if cqlsh is invoked with --debug then set the global debug flag to True
         if shell.debug:
             global DEBUG
             DEBUG = True
 
         # do not display messages when exporting to STDOUT unless --debug is set
-        self.printmsg = printmsg if self.fname is not None or direction == 'from' or DEBUG else None
+        self.printmsg = printmsg if self.fname is not None or direction == 'from' or DEBUG else swallowmsg
         self.options = self.parse_options(opts, direction)
 
         self.num_processes = self.options.copy['numprocesses']
         self.encoding = self.options.copy['encoding']
         self.printmsg('Using %d child processes' % (self.num_processes,))
 
         if direction == 'from':
@@ -2734,8 +2739,8 @@
         if self.log_file:
             with open(self.log_file, "a") as f:
                 f.write(output + '\n')
 
     def get_total_records(self):
         self.update(time.time())
         self.log_message()
-        return self.total_records
+        return self.total_records
```

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/cql3handling.py` & `cqlsh-expansion-0.9.2/cqlshlib/cql3handling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/cqlhandling.py` & `cqlsh-expansion-0.9.2/cqlshlib/cqlhandling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/cqlshhandling.py` & `cqlsh-expansion-0.9.2/cqlshlib/cqlshhandling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/displaying.py` & `cqlsh-expansion-0.9.2/cqlshlib/displaying.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/formatting.py` & `cqlsh-expansion-0.9.2/cqlshlib/formatting.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
     return ''.join(builder)
 
 
 def append(builder, dividend, divisor, unit):
     if dividend == 0 or dividend < divisor:
         return dividend
 
-    builder.append(str(dividend / divisor))
+    builder.append(str(dividend // divisor))
     builder.append(unit)
     return dividend % divisor
 
 
 def decode_vint(buf):
     return decode_zig_zag_64(decode_unsigned_vint(buf))
```

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/helptopics.py` & `cqlsh-expansion-0.9.2/cqlshlib/helptopics.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/pylexotron.py` & `cqlsh-expansion-0.9.2/cqlshlib/pylexotron.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/sslhandling.py` & `cqlsh-expansion-0.9.2/cqlshlib/sslhandling.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/tracing.py` & `cqlsh-expansion-0.9.2/cqlshlib/tracing.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/util.py` & `cqlsh-expansion-0.9.2/cqlshlib/util.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pylib/cqlshlib/wcwidth.py` & `cqlsh-expansion-0.9.2/cqlshlib/wcwidth.py`

 * *Files identical despite different names*

### Comparing `cqlsh-expansion-0.9.1/pyproject.toml` & `cqlsh-expansion-0.9.2/pyproject.toml`

 * *Files identical despite different names*

