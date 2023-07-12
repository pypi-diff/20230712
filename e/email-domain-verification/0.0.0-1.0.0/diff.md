# Comparing `tmp/email_domain_verification-0.0.0.tar.gz` & `tmp/email_domain_verification-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email_domain_verification-0.0.0.tar", last modified: Wed Jul 12 06:47:06 2023, max compression
+gzip compressed data, was "email_domain_verification-1.0.0.tar", last modified: Wed Jul 12 07:39:07 2023, max compression
```

## Comparing `email_domain_verification-0.0.0.tar` & `email_domain_verification-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 06:47:06.039563 email_domain_verification-0.0.0/
--rw-r--r--   0 geek      (1000) geek      (1000)     1166 2023-07-12 06:47:06.039563 email_domain_verification-0.0.0/PKG-INFO
--rw-r--r--   0 geek      (1000) geek      (1000)       19 2023-07-11 15:17:07.000000 email_domain_verification-0.0.0/README.md
-drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 06:47:06.037563 email_domain_verification-0.0.0/email_domain_verification/
--rw-r--r--   0 geek      (1000) geek      (1000)       66 2023-07-12 06:04:32.000000 email_domain_verification-0.0.0/email_domain_verification/__init__.py
--rw-r--r--   0 geek      (1000) geek      (1000)      264 2023-07-11 18:04:28.000000 email_domain_verification-0.0.0/email_domain_verification/emails.py
--rw-r--r--   0 geek      (1000) geek      (1000)      670 2023-07-12 05:35:14.000000 email_domain_verification-0.0.0/email_domain_verification/interfaces.py
--rw-r--r--   0 geek      (1000) geek      (1000)      893 2023-07-12 05:46:35.000000 email_domain_verification-0.0.0/email_domain_verification/utils.py
--rw-r--r--   0 geek      (1000) geek      (1000)     4270 2023-07-12 05:42:09.000000 email_domain_verification-0.0.0/email_domain_verification/validators.py
--rw-r--r--   0 geek      (1000) geek      (1000)      885 2023-07-12 06:37:40.000000 email_domain_verification-0.0.0/email_domain_verification/verification.py
-drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 06:47:06.038563 email_domain_verification-0.0.0/email_domain_verification.egg-info/
--rw-r--r--   0 geek      (1000) geek      (1000)     1166 2023-07-12 06:47:04.000000 email_domain_verification-0.0.0/email_domain_verification.egg-info/PKG-INFO
--rw-r--r--   0 geek      (1000) geek      (1000)      493 2023-07-12 06:47:06.000000 email_domain_verification-0.0.0/email_domain_verification.egg-info/SOURCES.txt
--rw-r--r--   0 geek      (1000) geek      (1000)        1 2023-07-12 06:47:04.000000 email_domain_verification-0.0.0/email_domain_verification.egg-info/dependency_links.txt
--rw-r--r--   0 geek      (1000) geek      (1000)        9 2023-07-12 06:47:05.000000 email_domain_verification-0.0.0/email_domain_verification.egg-info/requires.txt
--rw-r--r--   0 geek      (1000) geek      (1000)       26 2023-07-12 06:47:05.000000 email_domain_verification-0.0.0/email_domain_verification.egg-info/top_level.txt
--rw-r--r--   0 geek      (1000) geek      (1000)       38 2023-07-12 06:47:06.039563 email_domain_verification-0.0.0/setup.cfg
--rw-r--r--   0 geek      (1000) geek      (1000)     1631 2023-07-11 20:02:21.000000 email_domain_verification-0.0.0/setup.py
+drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:39:07.208122 email_domain_verification-1.0.0/
+-rw-r--r--   0 geek      (1000) geek      (1000)     3623 2023-07-12 07:39:07.207122 email_domain_verification-1.0.0/PKG-INFO
+-rw-r--r--   0 geek      (1000) geek      (1000)       19 2023-07-11 15:17:07.000000 email_domain_verification-1.0.0/README.md
+drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:39:07.205122 email_domain_verification-1.0.0/email_domain_verification/
+-rw-r--r--   0 geek      (1000) geek      (1000)       66 2023-07-12 06:04:32.000000 email_domain_verification-1.0.0/email_domain_verification/__init__.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      264 2023-07-11 18:04:28.000000 email_domain_verification-1.0.0/email_domain_verification/emails.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      670 2023-07-12 05:35:14.000000 email_domain_verification-1.0.0/email_domain_verification/interfaces.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      893 2023-07-12 05:46:35.000000 email_domain_verification-1.0.0/email_domain_verification/utils.py
+-rw-r--r--   0 geek      (1000) geek      (1000)     4270 2023-07-12 05:42:09.000000 email_domain_verification-1.0.0/email_domain_verification/validators.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      885 2023-07-12 06:37:40.000000 email_domain_verification-1.0.0/email_domain_verification/verification.py
+drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:39:07.207122 email_domain_verification-1.0.0/email_domain_verification.egg-info/
+-rw-r--r--   0 geek      (1000) geek      (1000)     3623 2023-07-12 07:39:06.000000 email_domain_verification-1.0.0/email_domain_verification.egg-info/PKG-INFO
+-rw-r--r--   0 geek      (1000) geek      (1000)      493 2023-07-12 07:39:07.000000 email_domain_verification-1.0.0/email_domain_verification.egg-info/SOURCES.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)        1 2023-07-12 07:39:06.000000 email_domain_verification-1.0.0/email_domain_verification.egg-info/dependency_links.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)        9 2023-07-12 07:39:06.000000 email_domain_verification-1.0.0/email_domain_verification.egg-info/requires.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)       26 2023-07-12 07:39:06.000000 email_domain_verification-1.0.0/email_domain_verification.egg-info/top_level.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)       38 2023-07-12 07:39:07.209122 email_domain_verification-1.0.0/setup.cfg
+-rw-r--r--   0 geek      (1000) geek      (1000)     4169 2023-07-12 07:39:02.000000 email_domain_verification-1.0.0/setup.py
```

### Comparing `email_domain_verification-0.0.0/email_domain_verification/interfaces.py` & `email_domain_verification-1.0.0/email_domain_verification/interfaces.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-0.0.0/email_domain_verification/utils.py` & `email_domain_verification-1.0.0/email_domain_verification/utils.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-0.0.0/email_domain_verification/validators.py` & `email_domain_verification-1.0.0/email_domain_verification/validators.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-0.0.0/email_domain_verification/verification.py` & `email_domain_verification-1.0.0/email_domain_verification/verification.py`

 * *Files identical despite different names*

