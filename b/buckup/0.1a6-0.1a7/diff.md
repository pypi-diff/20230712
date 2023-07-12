# Comparing `tmp/buckup-0.1a6.tar.gz` & `tmp/buckup-0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buckup-0.1a6.tar", last modified: Wed May 24 09:50:40 2023, max compression
+gzip compressed data, was "buckup-0.1a7.tar", last modified: Wed Jul 12 13:49:05 2023, max compression
```

## Comparing `buckup-0.1a6.tar` & `buckup-0.1a7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-05-24 09:50:40.232460 buckup-0.1a6/
--rw-r--r--   0 jake      (1000) jake       (975)     1494 2023-03-15 10:25:28.000000 buckup-0.1a6/LICENSE
--rw-r--r--   0 jake      (1000) jake       (975)     3943 2023-05-24 09:50:40.232460 buckup-0.1a6/PKG-INFO
--rw-r--r--   0 jake      (1000) jake       (975)     3035 2023-05-24 09:41:31.000000 buckup-0.1a6/README.rst
-drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-05-24 09:50:40.229127 buckup-0.1a6/buckup/
--rw-r--r--   0 jake      (1000) jake       (975)       78 2023-05-24 09:42:01.000000 buckup-0.1a6/buckup/__init__.py
--rw-r--r--   0 jake      (1000) jake       (975)     9687 2023-05-24 09:41:31.000000 buckup-0.1a6/buckup/bucket_creator.py
--rw-r--r--   0 jake      (1000) jake       (975)     8995 2023-05-24 09:42:01.000000 buckup-0.1a6/buckup/command_line.py
--rw-r--r--   0 jake      (1000) jake       (975)      351 2023-03-15 10:25:28.000000 buckup-0.1a6/buckup/exceptions.py
--rw-r--r--   0 jake      (1000) jake       (975)      807 2023-03-15 10:25:28.000000 buckup-0.1a6/buckup/utils.py
-drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-05-24 09:50:40.232460 buckup-0.1a6/buckup.egg-info/
--rw-r--r--   0 jake      (1000) jake       (975)     3943 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/PKG-INFO
--rw-r--r--   0 jake      (1000) jake       (975)      323 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/SOURCES.txt
--rw-r--r--   0 jake      (1000) jake       (975)        1 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/dependency_links.txt
--rw-r--r--   0 jake      (1000) jake       (975)       52 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/entry_points.txt
--rw-r--r--   0 jake      (1000) jake       (975)        6 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/requires.txt
--rw-r--r--   0 jake      (1000) jake       (975)        7 2023-05-24 09:50:40.000000 buckup-0.1a6/buckup.egg-info/top_level.txt
--rw-r--r--   0 jake      (1000) jake       (975)      981 2023-05-24 09:50:40.235794 buckup-0.1a6/setup.cfg
--rw-r--r--   0 jake      (1000) jake       (975)      130 2023-03-15 10:25:28.000000 buckup-0.1a6/setup.py
+drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-07-12 13:49:05.133120 buckup-0.1a7/
+-rw-r--r--   0 jake      (1000) jake       (975)     1494 2023-03-15 10:25:28.000000 buckup-0.1a7/LICENSE
+-rw-r--r--   0 jake      (1000) jake       (975)     3943 2023-07-12 13:49:05.133120 buckup-0.1a7/PKG-INFO
+-rw-r--r--   0 jake      (1000) jake       (975)     3035 2023-05-24 09:41:31.000000 buckup-0.1a7/README.rst
+drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-07-12 13:49:05.129787 buckup-0.1a7/buckup/
+-rw-r--r--   0 jake      (1000) jake       (975)       78 2023-05-24 09:42:01.000000 buckup-0.1a7/buckup/__init__.py
+-rw-r--r--   0 jake      (1000) jake       (975)     9686 2023-07-12 13:47:01.000000 buckup-0.1a7/buckup/bucket_creator.py
+-rw-r--r--   0 jake      (1000) jake       (975)     8995 2023-05-24 09:42:01.000000 buckup-0.1a7/buckup/command_line.py
+-rw-r--r--   0 jake      (1000) jake       (975)      351 2023-03-15 10:25:28.000000 buckup-0.1a7/buckup/exceptions.py
+-rw-r--r--   0 jake      (1000) jake       (975)      807 2023-03-15 10:25:28.000000 buckup-0.1a7/buckup/utils.py
+drwxr-xr-x   0 jake      (1000) jake       (975)        0 2023-07-12 13:49:05.129787 buckup-0.1a7/buckup.egg-info/
+-rw-r--r--   0 jake      (1000) jake       (975)     3943 2023-07-12 13:49:05.000000 buckup-0.1a7/buckup.egg-info/PKG-INFO
+-rw-r--r--   0 jake      (1000) jake       (975)      323 2023-07-12 13:49:05.000000 buckup-0.1a7/buckup.egg-info/SOURCES.txt
+-rw-r--r--   0 jake      (1000) jake       (975)        1 2023-07-12 13:49:05.000000 buckup-0.1a7/buckup.egg-info/dependency_links.txt
+-rw-r--r--   0 jake      (1000) jake       (975)       52 2023-07-12 13:49:05.000000 buckup-0.1a7/buckup.egg-info/entry_points.txt
+-rw-r--r--   0 jake      (1000) jake       (975)        6 2023-07-12 13:49:05.000000 buckup-0.1a7/buckup.egg-info/requires.txt
+-rw-r--r--   0 jake      (1000) jake       (975)        7 2023-07-12 13:49:05.000000 buckup-0.1a7/buckup.egg-info/top_level.txt
+-rw-r--r--   0 jake      (1000) jake       (975)      981 2023-07-12 13:49:05.133120 buckup-0.1a7/setup.cfg
+-rw-r--r--   0 jake      (1000) jake       (975)      130 2023-03-15 10:25:28.000000 buckup-0.1a7/setup.py
```

### Comparing `buckup-0.1a6/LICENSE` & `buckup-0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `buckup-0.1a6/PKG-INFO` & `buckup-0.1a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckup
-Version: 0.1a6
+Version: 0.1a7
 Summary: Create S3 buckets in seconds from your command line to use on your website.
 Home-page: https://github.com/torchbox/buckup
 Author: Tomasz Knapik
 Author-email: tomasz.knapik@torchbox.com
 Maintainer: Torchbox
 Maintainer-email: info@torchbox.com
 License: BSD 3-Clause License
```

### Comparing `buckup-0.1a6/README.rst` & `buckup-0.1a7/README.rst`

 * *Files identical despite different names*

### Comparing `buckup-0.1a6/buckup/bucket_creator.py` & `buckup-0.1a7/buckup/bucket_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,27 @@
             )
         }
 
     def set_bucket_policy(self, bucket, user, allow_public_acls, public_get_object_paths=None):
         policy_statement = []
         public_access = bool(public_get_object_paths)
 
+        # NB: This API doesn't exist on a `Bucket`
+        self.s3_client.put_public_access_block(
+            Bucket=bucket.name,
+            PublicAccessBlockConfiguration={
+                "BlockPublicAcls": not allow_public_acls,
+                "IgnorePublicAcls": not allow_public_acls,
+                "BlockPublicPolicy": not public_access,
+                "RestrictPublicBuckets": not public_access
+            }
+        )
+        if public_access or allow_public_acls:
+            print('Configured public access to bucket.')
+
         if public_access:
             policy_statement.append(
                 self.get_bucket_policy_statement_for_get_object(
                     bucket, public_get_object_paths
                 )
             )
         policy_statement.extend(list(
@@ -122,28 +135,14 @@
                     time.sleep(5)
                     continue
                 raise e
             else:
                 break
         print('Bucket policy set.')
 
-        # NB: This API doesn't exist on a `Bucket`
-        self.s3_client.put_public_access_block(
-            Bucket=bucket.name,
-            PublicAccessBlockConfiguration={
-                "BlockPublicAcls": not allow_public_acls,
-                "IgnorePublicAcls": not allow_public_acls,
-                "BlockPublicPolicy": not public_access,
-                "RestrictPublicBuckets": not public_access
-            }
-        )
-
-        if public_access or allow_public_acls:
-            print('Configured public access to bucket.')
-
     def create_bucket(self, name, region):
         """
         Create bucket of name in the given region.
         """
         create_bucket_kwargs = {}
         create_bucket_config = {}
         # us-east-1 does not work with location specified.
```

### Comparing `buckup-0.1a6/buckup/command_line.py` & `buckup-0.1a7/buckup/command_line.py`

 * *Files identical despite different names*

### Comparing `buckup-0.1a6/buckup/utils.py` & `buckup-0.1a7/buckup/utils.py`

 * *Files identical despite different names*

### Comparing `buckup-0.1a6/buckup.egg-info/PKG-INFO` & `buckup-0.1a7/buckup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckup
-Version: 0.1a6
+Version: 0.1a7
 Summary: Create S3 buckets in seconds from your command line to use on your website.
 Home-page: https://github.com/torchbox/buckup
 Author: Tomasz Knapik
 Author-email: tomasz.knapik@torchbox.com
 Maintainer: Torchbox
 Maintainer-email: info@torchbox.com
 License: BSD 3-Clause License
```

### Comparing `buckup-0.1a6/setup.cfg` & `buckup-0.1a7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = buckup
-version = 0.1a6
+version = 0.1a7
 description = Create S3 buckets in seconds from your command line to use on your website.
 long-description = file: README.rst
 maintainer = Torchbox
 maintainer_email = info@torchbox.com
 author = Tomasz Knapik
 author_email = tomasz.knapik@torchbox.com
 url = https://github.com/torchbox/buckup
```

