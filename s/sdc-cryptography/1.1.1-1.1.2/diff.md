# Comparing `tmp/sdc-cryptography-1.1.1.tar.gz` & `tmp/sdc-cryptography-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdc-cryptography-1.1.1.tar", last modified: Thu Oct 13 14:27:54 2022, max compression
+gzip compressed data, was "sdc-cryptography-1.1.2.tar", last modified: Wed Jul 12 07:52:29 2023, max compression
```

## Comparing `sdc-cryptography-1.1.1.tar` & `sdc-cryptography-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 14:27:54.730987 sdc-cryptography-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-10-13 14:27:54.730987 sdc-cryptography-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 14:27:54.730987 sdc-cryptography-1.1.1/sdc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 14:27:54.730987 sdc-cryptography-1.1.1/sdc/crypto/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/decrypter.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/jwe_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/jwt_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/key_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 14:27:54.730987 sdc-cryptography-1.1.1/sdc/crypto/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7013 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/sdc/crypto/scripts/generate_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 14:27:54.730987 sdc-cryptography-1.1.1/sdc_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-10-13 14:27:54.000000 sdc-cryptography-1.1.1/sdc_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-10-13 14:27:54.000000 sdc-cryptography-1.1.1/sdc_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 14:27:54.000000 sdc-cryptography-1.1.1/sdc_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-13 14:27:54.000000 sdc-cryptography-1.1.1/sdc_cryptography.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 14:27:54.000000 sdc-cryptography-1.1.1/sdc_cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-13 14:27:54.000000 sdc-cryptography-1.1.1/sdc_cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-13 14:27:54.000000 sdc-cryptography-1.1.1/sdc_cryptography.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-13 14:27:54.730987 sdc-cryptography-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-10-13 14:27:42.000000 sdc-cryptography-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:52:29.483512 sdc-cryptography-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-12 07:52:29.483512 sdc-cryptography-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:52:29.479512 sdc-cryptography-1.1.2/sdc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:52:29.483512 sdc-cryptography-1.1.2/sdc/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/jwe_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/jwt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/key_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:52:29.483512 sdc-cryptography-1.1.2/sdc/crypto/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7013 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/sdc/crypto/scripts/generate_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:52:29.483512 sdc-cryptography-1.1.2/sdc_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-12 07:52:29.000000 sdc-cryptography-1.1.2/sdc_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 07:52:29.000000 sdc-cryptography-1.1.2/sdc_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:52:29.000000 sdc-cryptography-1.1.2/sdc_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 07:52:29.000000 sdc-cryptography-1.1.2/sdc_cryptography.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:52:29.000000 sdc-cryptography-1.1.2/sdc_cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 07:52:29.000000 sdc-cryptography-1.1.2/sdc_cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 07:52:29.000000 sdc-cryptography-1.1.2/sdc_cryptography.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 07:52:29.483512 sdc-cryptography-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:52:29.483512 sdc-cryptography-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/tests/test_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/tests/test_encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/tests/test_from_rfc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/tests/test_generate_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/tests/test_invalid_token_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/tests/test_jwe_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/tests/test_jwt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-12 07:52:20.000000 sdc-cryptography-1.1.2/tests/test_key_store.py
```

### Comparing `sdc-cryptography-1.1.1/LICENSE` & `sdc-cryptography-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc-cryptography-1.1.1/PKG-INFO` & `sdc-cryptography-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdc-cryptography
-Version: 1.1.1
+Version: 1.1.2
 Summary: A shared library for SDC services that use JWT with JWE
 Home-page: https://github.com/ONSdigital/sdc-cryptography
 Author: ONS
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdc-cryptography-1.1.1/README.md` & `sdc-cryptography-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sdc-cryptography-1.1.1/sdc/crypto/decrypter.py` & `sdc-cryptography-1.1.2/sdc/crypto/decrypter.py`

 * *Files identical despite different names*

### Comparing `sdc-cryptography-1.1.1/sdc/crypto/encrypter.py` & `sdc-cryptography-1.1.2/sdc/crypto/encrypter.py`

 * *Files identical despite different names*

### Comparing `sdc-cryptography-1.1.1/sdc/crypto/helper.py` & `sdc-cryptography-1.1.2/sdc/crypto/helper.py`

 * *Files identical despite different names*

### Comparing `sdc-cryptography-1.1.1/sdc/crypto/jwe_helper.py` & `sdc-cryptography-1.1.2/sdc/crypto/jwe_helper.py`

 * *Files identical despite different names*

### Comparing `sdc-cryptography-1.1.1/sdc/crypto/jwt_helper.py` & `sdc-cryptography-1.1.2/sdc/crypto/jwt_helper.py`

 * *Files identical despite different names*

### Comparing `sdc-cryptography-1.1.1/sdc/crypto/key_store.py` & `sdc-cryptography-1.1.2/sdc/crypto/key_store.py`

 * *Files identical despite different names*

### Comparing `sdc-cryptography-1.1.1/sdc/crypto/scripts/generate_keys.py` & `sdc-cryptography-1.1.2/sdc/crypto/scripts/generate_keys.py`

 * *Files identical despite different names*

### Comparing `sdc-cryptography-1.1.1/sdc_cryptography.egg-info/PKG-INFO` & `sdc-cryptography-1.1.2/sdc_cryptography.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdc-cryptography
-Version: 1.1.1
+Version: 1.1.2
 Summary: A shared library for SDC services that use JWT with JWE
 Home-page: https://github.com/ONSdigital/sdc-cryptography
 Author: ONS
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdc-cryptography-1.1.1/setup.py` & `sdc-cryptography-1.1.2/setup.py`

 * *Files identical despite different names*

