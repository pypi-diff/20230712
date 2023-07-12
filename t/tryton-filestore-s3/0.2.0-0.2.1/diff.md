# Comparing `tmp/tryton-filestore-s3-0.2.0.tar.gz` & `tmp/tryton-filestore-s3-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryton-filestore-s3-0.2.0.tar", last modified: Wed Oct 13 10:32:29 2021, max compression
+gzip compressed data, was "tryton-filestore-s3-0.2.1.tar", last modified: Wed Jul 12 06:39:35 2023, max compression
```

## Comparing `tryton-filestore-s3-0.2.0.tar` & `tryton-filestore-s3-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lukio     (1000) lukio     (1000)        0 2021-10-13 10:32:29.616634 tryton-filestore-s3-0.2.0/
--rw-rw-r--   0 lukio     (1000) lukio     (1000)      166 2021-10-13 10:17:02.000000 tryton-filestore-s3-0.2.0/CHANGELOG
--rw-rw-r--   0 lukio     (1000) lukio     (1000)      767 2021-10-13 10:20:47.000000 tryton-filestore-s3-0.2.0/COPYRIGHT
--rw-rw-r--   0 lukio     (1000) lukio     (1000)    35147 2021-10-13 10:00:57.000000 tryton-filestore-s3-0.2.0/LICENSE
--rw-rw-r--   0 lukio     (1000) lukio     (1000)       67 2021-10-13 10:00:57.000000 tryton-filestore-s3-0.2.0/MANIFEST.in
--rw-rw-r--   0 lukio     (1000) lukio     (1000)     1659 2021-10-13 10:32:29.616634 tryton-filestore-s3-0.2.0/PKG-INFO
--rw-rw-r--   0 lukio     (1000) lukio     (1000)      900 2021-10-13 10:00:57.000000 tryton-filestore-s3-0.2.0/README
--rw-rw-r--   0 lukio     (1000) lukio     (1000)       38 2021-10-13 10:32:29.616634 tryton-filestore-s3-0.2.0/setup.cfg
--rw-rw-r--   0 lukio     (1000) lukio     (1000)     1256 2021-10-13 10:21:38.000000 tryton-filestore-s3-0.2.0/setup.py
-drwxrwxr-x   0 lukio     (1000) lukio     (1000)        0 2021-10-13 10:32:29.616634 tryton-filestore-s3-0.2.0/tryton_filestore_s3.egg-info/
--rw-rw-r--   0 lukio     (1000) lukio     (1000)     1659 2021-10-13 10:32:29.000000 tryton-filestore-s3-0.2.0/tryton_filestore_s3.egg-info/PKG-INFO
--rw-rw-r--   0 lukio     (1000) lukio     (1000)      334 2021-10-13 10:32:29.000000 tryton-filestore-s3-0.2.0/tryton_filestore_s3.egg-info/SOURCES.txt
--rw-rw-r--   0 lukio     (1000) lukio     (1000)        1 2021-10-13 10:32:29.000000 tryton-filestore-s3-0.2.0/tryton_filestore_s3.egg-info/dependency_links.txt
--rw-rw-r--   0 lukio     (1000) lukio     (1000)        1 2021-10-13 10:32:29.000000 tryton-filestore-s3-0.2.0/tryton_filestore_s3.egg-info/not-zip-safe
--rw-rw-r--   0 lukio     (1000) lukio     (1000)       18 2021-10-13 10:32:29.000000 tryton-filestore-s3-0.2.0/tryton_filestore_s3.egg-info/requires.txt
--rw-rw-r--   0 lukio     (1000) lukio     (1000)       20 2021-10-13 10:32:29.000000 tryton-filestore-s3-0.2.0/tryton_filestore_s3.egg-info/top_level.txt
--rw-rw-r--   0 lukio     (1000) lukio     (1000)     1591 2021-10-13 10:15:38.000000 tryton-filestore-s3-0.2.0/tryton_filestore_s3.py
+drwxrwxr-x   0 lukio     (1000) lukio     (1000)        0 2023-07-12 06:39:35.377481 tryton-filestore-s3-0.2.1/
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)      259 2023-07-12 06:27:43.000000 tryton-filestore-s3-0.2.1/CHANGELOG
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)      801 2023-07-12 06:24:14.000000 tryton-filestore-s3-0.2.1/COPYRIGHT
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)    35147 2021-10-13 10:00:57.000000 tryton-filestore-s3-0.2.1/LICENSE
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)       67 2021-10-13 10:00:57.000000 tryton-filestore-s3-0.2.1/MANIFEST.in
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)     2072 2023-07-12 06:39:35.377481 tryton-filestore-s3-0.2.1/PKG-INFO
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)     1076 2023-07-12 06:20:58.000000 tryton-filestore-s3-0.2.1/README
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)       38 2023-07-12 06:39:35.377481 tryton-filestore-s3-0.2.1/setup.cfg
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)     1256 2023-07-12 06:27:24.000000 tryton-filestore-s3-0.2.1/setup.py
+drwxrwxr-x   0 lukio     (1000) lukio     (1000)        0 2023-07-12 06:39:35.377481 tryton-filestore-s3-0.2.1/tryton_filestore_s3.egg-info/
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)     2072 2023-07-12 06:39:35.000000 tryton-filestore-s3-0.2.1/tryton_filestore_s3.egg-info/PKG-INFO
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)      334 2023-07-12 06:39:35.000000 tryton-filestore-s3-0.2.1/tryton_filestore_s3.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)        1 2023-07-12 06:39:35.000000 tryton-filestore-s3-0.2.1/tryton_filestore_s3.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)        1 2023-07-12 06:39:35.000000 tryton-filestore-s3-0.2.1/tryton_filestore_s3.egg-info/not-zip-safe
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)       18 2023-07-12 06:39:35.000000 tryton-filestore-s3-0.2.1/tryton_filestore_s3.egg-info/requires.txt
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)       20 2023-07-12 06:39:35.000000 tryton-filestore-s3-0.2.1/tryton_filestore_s3.egg-info/top_level.txt
+-rw-rw-r--   0 lukio     (1000) lukio     (1000)     1831 2023-07-12 06:20:58.000000 tryton-filestore-s3-0.2.1/tryton_filestore_s3.py
```

### Comparing `tryton-filestore-s3-0.2.0/COPYRIGHT` & `tryton-filestore-s3-0.2.1/COPYRIGHT`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+Copyright (c) 2023 Cédric Krier.
 Copyright (c) 2021 Ningú.
 Copyright (c) 2018-2021 gcoop Cooperativa de Software Libre.
 Copyright (c) 2018-2021 Luciano Rossi.
 Copyright (c) 2018 Gotsho.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
```

### Comparing `tryton-filestore-s3-0.2.0/LICENSE` & `tryton-filestore-s3-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-filestore-s3-0.2.0/PKG-INFO` & `tryton-filestore-s3-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: tryton-filestore-s3
-Version: 0.2.0
+Version: 0.2.1
 Summary: Store Tryton files on S3 AWS Storage.
 Home-page: https://github.com/gcoop-libre/tryton-filestore-s3
 Author: gcoop
 Author-email: info@gcoop.coop
 License: GPL-3
+Description: Tryton FileStore S3 AWS Backend
+        ===============================
+        
+        S3 AWS backend for the Tryton application framework.
+        
+        In order to configure the S3 Amazon you should modify your trytond
+        configuration file to include the `tryton_filestore_s3.FileStoreS3` as class
+        of the database section. Also you need to specify the s3 credentials
+        with the s3_access_key, s3_secret_key and bucket values.
+        
+        An example configuration file looks like::
+        
+            [database]
+            class=tryton_filestore_s3.FileStoreS3
+            s3_access_key=access-key-s3
+            s3_secret_key=secret-key-s3
+            bucket=bucket-id-here
+        
+        Once you have specified the config file, everything should work out of the
+        box and you should see your attachments created on the S3 bucket.
+        
+        You can configure a different endpoint URL than the one generated for Amazon
+        with the configuration `s3_endpoint` (which must contain the scheme like
+        `https://`).
+        
+        Thanks
+        ------
+        This module was developed by gcoop in association with Gotsho. Thanks
+        Gotsho for sharing this feature.
+        
+        This code is based on the tryton-filestore-gs backend implementation.
+        
 Keywords: tryton s3 aws storage attachments
 Platform: Posix; MacOS X; Windows
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
-License-File: LICENSE
-
-Tryton FileStore S3 AWS Backend
-===============================
-
-S3 AWS backend for the Tryton application framework.
-
-In order to configure the S3 Amazon you should modify your trytond
-configuration file to include the `tryton_filestore_s3.FileStoreS3` as class
-of the database section. Also you need to specify the s3 credentials
-with the access_key, secret_key and bucket values.
-
-An example configuration file looks like::
-
-    [database]
-    class=tryton_filestore_s3.FileStoreS3
-    access_key=access-key-s3
-    secret_key=secret-key-s3
-    bucket=bucket-id-here
-
-Once you have specified the config file, everything should work out of the
-box and you should see your attachments created on the S3 bucket.
-
-Thanks
-------
-This module was developed by gcoop in association with Gotsho. Thanks
-Gotsho for sharing this feature.
-
-This code is based on the tryton-filestore-gs backend implementation.
-
-
```

### Comparing `tryton-filestore-s3-0.2.0/README` & `tryton-filestore-s3-0.2.1/README`

 * *Files 24% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 ===============================
 
 S3 AWS backend for the Tryton application framework.
 
 In order to configure the S3 Amazon you should modify your trytond
 configuration file to include the `tryton_filestore_s3.FileStoreS3` as class
 of the database section. Also you need to specify the s3 credentials
-with the access_key, secret_key and bucket values.
+with the s3_access_key, s3_secret_key and bucket values.
 
 An example configuration file looks like::
 
     [database]
     class=tryton_filestore_s3.FileStoreS3
-    access_key=access-key-s3
-    secret_key=secret-key-s3
+    s3_access_key=access-key-s3
+    s3_secret_key=secret-key-s3
     bucket=bucket-id-here
 
 Once you have specified the config file, everything should work out of the
 box and you should see your attachments created on the S3 bucket.
 
+You can configure a different endpoint URL than the one generated for Amazon
+with the configuration `s3_endpoint` (which must contain the scheme like
+`https://`).
+
 Thanks
 ------
 This module was developed by gcoop in association with Gotsho. Thanks
 Gotsho for sharing this feature.
 
 This code is based on the tryton-filestore-gs backend implementation.
```

### Comparing `tryton-filestore-s3-0.2.0/setup.py` & `tryton-filestore-s3-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
 
 
 setup(
     name='tryton-filestore-s3',
-    version='0.2.0',
+    version='0.2.1',
     author='gcoop',
     author_email='info@gcoop.coop',
     url='https://github.com/gcoop-libre/tryton-filestore-s3',
     description='Store Tryton files on S3 AWS Storage.',
     long_description=read('README'),
     py_modules=['tryton_filestore_s3'],
     zip_safe=False,
```

### Comparing `tryton-filestore-s3-0.2.0/tryton_filestore_s3.egg-info/PKG-INFO` & `tryton-filestore-s3-0.2.1/tryton_filestore_s3.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: tryton-filestore-s3
-Version: 0.2.0
+Version: 0.2.1
 Summary: Store Tryton files on S3 AWS Storage.
 Home-page: https://github.com/gcoop-libre/tryton-filestore-s3
 Author: gcoop
 Author-email: info@gcoop.coop
 License: GPL-3
+Description: Tryton FileStore S3 AWS Backend
+        ===============================
+        
+        S3 AWS backend for the Tryton application framework.
+        
+        In order to configure the S3 Amazon you should modify your trytond
+        configuration file to include the `tryton_filestore_s3.FileStoreS3` as class
+        of the database section. Also you need to specify the s3 credentials
+        with the s3_access_key, s3_secret_key and bucket values.
+        
+        An example configuration file looks like::
+        
+            [database]
+            class=tryton_filestore_s3.FileStoreS3
+            s3_access_key=access-key-s3
+            s3_secret_key=secret-key-s3
+            bucket=bucket-id-here
+        
+        Once you have specified the config file, everything should work out of the
+        box and you should see your attachments created on the S3 bucket.
+        
+        You can configure a different endpoint URL than the one generated for Amazon
+        with the configuration `s3_endpoint` (which must contain the scheme like
+        `https://`).
+        
+        Thanks
+        ------
+        This module was developed by gcoop in association with Gotsho. Thanks
+        Gotsho for sharing this feature.
+        
+        This code is based on the tryton-filestore-gs backend implementation.
+        
 Keywords: tryton s3 aws storage attachments
 Platform: Posix; MacOS X; Windows
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
-License-File: LICENSE
-
-Tryton FileStore S3 AWS Backend
-===============================
-
-S3 AWS backend for the Tryton application framework.
-
-In order to configure the S3 Amazon you should modify your trytond
-configuration file to include the `tryton_filestore_s3.FileStoreS3` as class
-of the database section. Also you need to specify the s3 credentials
-with the access_key, secret_key and bucket values.
-
-An example configuration file looks like::
-
-    [database]
-    class=tryton_filestore_s3.FileStoreS3
-    access_key=access-key-s3
-    secret_key=secret-key-s3
-    bucket=bucket-id-here
-
-Once you have specified the config file, everything should work out of the
-box and you should see your attachments created on the S3 bucket.
-
-Thanks
-------
-This module was developed by gcoop in association with Gotsho. Thanks
-Gotsho for sharing this feature.
-
-This code is based on the tryton-filestore-gs backend implementation.
-
-
```

### Comparing `tryton-filestore-s3-0.2.0/tryton_filestore_s3.py` & `tryton-filestore-s3-0.2.1/tryton_filestore_s3.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,16 +38,22 @@
 
 
 def name(id, prefix=''):
     return '/'.join(filter(None, [prefix, id]))
 
 
 def get_client():
-    access_key = config.get('database', 'access_key', default=None)
-    secret_key = config.get('database', 'secret_key', default=None)
+    access_key = config.get('database', 's3_access_key')
+    if access_key is None:
+        access_key = config.get('database', 'access_key')
+    secret_key = config.get('database', 's3_secret_key')
+    if secret_key is None:
+        secret_key = config.get('database', 'secret_key')
     bucket = config.get('database', 'bucket')
+    endpoint_url = config.get('database', 's3_endpoint')
     client = boto3.client(
         's3',
         aws_access_key_id=access_key,
         aws_secret_access_key=secret_key,
+        endpoint_url=endpoint_url,
     )
     return client, bucket
```

