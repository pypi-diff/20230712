# Comparing `tmp/outbox-encryption-1.1.1.tar.gz` & `tmp/outbox-encryption-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outbox-encryption-1.1.1.tar", last modified: Fri Feb 24 16:21:05 2023, max compression
+gzip compressed data, was "outbox-encryption-1.1.2.tar", last modified: Wed Jul 12 12:47:28 2023, max compression
```

## Comparing `outbox-encryption-1.1.1.tar` & `outbox-encryption-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:21:05.770599 outbox-encryption-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-24 16:20:57.000000 outbox-encryption-1.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-24 16:20:57.000000 outbox-encryption-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-02-24 16:21:05.766599 outbox-encryption-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-02-24 16:20:57.000000 outbox-encryption-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:21:05.766599 outbox-encryption-1.1.1/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)    33295 2023-02-24 16:20:57.000000 outbox-encryption-1.1.1/encryption/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:21:05.766599 outbox-encryption-1.1.1/outbox_encryption.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-02-24 16:21:05.000000 outbox-encryption-1.1.1/outbox_encryption.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-24 16:21:05.000000 outbox-encryption-1.1.1/outbox_encryption.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 16:21:05.000000 outbox-encryption-1.1.1/outbox_encryption.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-24 16:21:05.000000 outbox-encryption-1.1.1/outbox_encryption.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 16:21:05.000000 outbox-encryption-1.1.1/outbox_encryption.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 16:21:05.770599 outbox-encryption-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-02-24 16:20:57.000000 outbox-encryption-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:28.936049 outbox-encryption-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-12 12:47:16.000000 outbox-encryption-1.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 12:47:16.000000 outbox-encryption-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-07-12 12:47:28.936049 outbox-encryption-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-12 12:47:16.000000 outbox-encryption-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:28.932049 outbox-encryption-1.1.2/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)    33295 2023-07-12 12:47:16.000000 outbox-encryption-1.1.2/encryption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:28.932049 outbox-encryption-1.1.2/outbox_encryption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-07-12 12:47:28.000000 outbox-encryption-1.1.2/outbox_encryption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-12 12:47:28.000000 outbox-encryption-1.1.2/outbox_encryption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:47:28.000000 outbox-encryption-1.1.2/outbox_encryption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-12 12:47:28.000000 outbox-encryption-1.1.2/outbox_encryption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 12:47:28.000000 outbox-encryption-1.1.2/outbox_encryption.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:47:28.936049 outbox-encryption-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-12 12:47:16.000000 outbox-encryption-1.1.2/setup.py
```

### Comparing `outbox-encryption-1.1.1/LICENSE.md` & `outbox-encryption-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `outbox-encryption-1.1.1/PKG-INFO` & `outbox-encryption-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outbox-encryption
-Version: 1.1.1
+Version: 1.1.2
 Summary: DJANGO OUTBOX ENCRYPTION
 Home-page: https://github.com/PROJECT-OUTBOX/django_lib_outbox_encryption.git
 Author-email: suratiwan03@gmail.com
 Keywords: encrypt,decrypt,environment,django,settings
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `outbox-encryption-1.1.1/README.md` & `outbox-encryption-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `outbox-encryption-1.1.1/encryption/__init__.py` & `outbox-encryption-1.1.2/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `outbox-encryption-1.1.1/outbox_encryption.egg-info/PKG-INFO` & `outbox-encryption-1.1.2/outbox_encryption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outbox-encryption
-Version: 1.1.1
+Version: 1.1.2
 Summary: DJANGO OUTBOX ENCRYPTION
 Home-page: https://github.com/PROJECT-OUTBOX/django_lib_outbox_encryption.git
 Author-email: suratiwan03@gmail.com
 Keywords: encrypt,decrypt,environment,django,settings
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `outbox-encryption-1.1.1/setup.py` & `outbox-encryption-1.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="1.1.1",    # 1.0.21 (versi akhir sebelum rombak rule)
+    version="1.1.2",    # 1.0.21 (versi akhir sebelum rombak rule)
 
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
@@ -32,16 +32,18 @@
     # EITHER py_modules OR packages should be present.
     packages=find_packages(exclude="tests"),
 
     # agar file manifest .in dieksekusi
     include_package_data = True,
 
     # dependencies
+    # pastikan versi cryptography == 38.0.1
+    # jika tidak maka akan error
     install_requires=[
-        'cryptography',
+        'cryptography==38.0.1',
         'python-decouple',
     ],
 
     # The description that will be shown on PyPI.
     # Keep it short and concise
     # This field is OPTIONAL
     description="DJANGO OUTBOX ENCRYPTION",
```

