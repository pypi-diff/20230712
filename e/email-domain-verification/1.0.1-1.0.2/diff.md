# Comparing `tmp/email_domain_verification-1.0.1.tar.gz` & `tmp/email_domain_verification-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email_domain_verification-1.0.1.tar", last modified: Wed Jul 12 07:46:28 2023, max compression
+gzip compressed data, was "email_domain_verification-1.0.2.tar", last modified: Wed Jul 12 07:47:16 2023, max compression
```

## Comparing `email_domain_verification-1.0.1.tar` & `email_domain_verification-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:46:28.180560 email_domain_verification-1.0.1/
--rw-r--r--   0 geek      (1000) geek      (1000)     3685 2023-07-12 07:46:28.177560 email_domain_verification-1.0.1/PKG-INFO
--rw-r--r--   0 geek      (1000) geek      (1000)       19 2023-07-11 15:17:07.000000 email_domain_verification-1.0.1/README.md
-drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:46:28.163560 email_domain_verification-1.0.1/email_domain_verification/
--rw-r--r--   0 geek      (1000) geek      (1000)       66 2023-07-12 06:04:32.000000 email_domain_verification-1.0.1/email_domain_verification/__init__.py
--rw-r--r--   0 geek      (1000) geek      (1000)      264 2023-07-11 18:04:28.000000 email_domain_verification-1.0.1/email_domain_verification/emails.py
--rw-r--r--   0 geek      (1000) geek      (1000)      670 2023-07-12 05:35:14.000000 email_domain_verification-1.0.1/email_domain_verification/interfaces.py
--rw-r--r--   0 geek      (1000) geek      (1000)      893 2023-07-12 05:46:35.000000 email_domain_verification-1.0.1/email_domain_verification/utils.py
--rw-r--r--   0 geek      (1000) geek      (1000)     4270 2023-07-12 05:42:09.000000 email_domain_verification-1.0.1/email_domain_verification/validators.py
--rw-r--r--   0 geek      (1000) geek      (1000)      885 2023-07-12 06:37:40.000000 email_domain_verification-1.0.1/email_domain_verification/verification.py
-drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:46:28.176560 email_domain_verification-1.0.1/email_domain_verification.egg-info/
--rw-r--r--   0 geek      (1000) geek      (1000)     3685 2023-07-12 07:46:27.000000 email_domain_verification-1.0.1/email_domain_verification.egg-info/PKG-INFO
--rw-r--r--   0 geek      (1000) geek      (1000)      493 2023-07-12 07:46:28.000000 email_domain_verification-1.0.1/email_domain_verification.egg-info/SOURCES.txt
--rw-r--r--   0 geek      (1000) geek      (1000)        1 2023-07-12 07:46:27.000000 email_domain_verification-1.0.1/email_domain_verification.egg-info/dependency_links.txt
--rw-r--r--   0 geek      (1000) geek      (1000)        9 2023-07-12 07:46:27.000000 email_domain_verification-1.0.1/email_domain_verification.egg-info/requires.txt
--rw-r--r--   0 geek      (1000) geek      (1000)       26 2023-07-12 07:46:27.000000 email_domain_verification-1.0.1/email_domain_verification.egg-info/top_level.txt
--rw-r--r--   0 geek      (1000) geek      (1000)       38 2023-07-12 07:46:28.180560 email_domain_verification-1.0.1/setup.cfg
--rw-r--r--   0 geek      (1000) geek      (1000)     4231 2023-07-12 07:46:23.000000 email_domain_verification-1.0.1/setup.py
+drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:47:16.678608 email_domain_verification-1.0.2/
+-rw-r--r--   0 geek      (1000) geek      (1000)     3685 2023-07-12 07:47:16.678608 email_domain_verification-1.0.2/PKG-INFO
+-rw-r--r--   0 geek      (1000) geek      (1000)       19 2023-07-11 15:17:07.000000 email_domain_verification-1.0.2/README.md
+drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:47:16.676608 email_domain_verification-1.0.2/email_domain_verification/
+-rw-r--r--   0 geek      (1000) geek      (1000)       66 2023-07-12 06:04:32.000000 email_domain_verification-1.0.2/email_domain_verification/__init__.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      264 2023-07-11 18:04:28.000000 email_domain_verification-1.0.2/email_domain_verification/emails.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      670 2023-07-12 05:35:14.000000 email_domain_verification-1.0.2/email_domain_verification/interfaces.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      893 2023-07-12 05:46:35.000000 email_domain_verification-1.0.2/email_domain_verification/utils.py
+-rw-r--r--   0 geek      (1000) geek      (1000)     4270 2023-07-12 05:42:09.000000 email_domain_verification-1.0.2/email_domain_verification/validators.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      885 2023-07-12 06:37:40.000000 email_domain_verification-1.0.2/email_domain_verification/verification.py
+drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:47:16.678608 email_domain_verification-1.0.2/email_domain_verification.egg-info/
+-rw-r--r--   0 geek      (1000) geek      (1000)     3685 2023-07-12 07:47:15.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/PKG-INFO
+-rw-r--r--   0 geek      (1000) geek      (1000)      493 2023-07-12 07:47:16.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/SOURCES.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)        1 2023-07-12 07:47:15.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/dependency_links.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)        9 2023-07-12 07:47:16.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/requires.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)       26 2023-07-12 07:47:16.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/top_level.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)       38 2023-07-12 07:47:16.678608 email_domain_verification-1.0.2/setup.cfg
+-rw-r--r--   0 geek      (1000) geek      (1000)     4231 2023-07-12 07:47:12.000000 email_domain_verification-1.0.2/setup.py
```

### Comparing `email_domain_verification-1.0.1/PKG-INFO` & `email_domain_verification-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email_domain_verification
-Version: 1.0.1
+Version: 1.0.2
 Summary: Can Verify All The Email Forms And Domains
 Home-page: https://github.com/khodnevis-app/development_tools
 Author: Mahdi Niknejad
 Author-email: mmahdiniknejad@gmail.com
 Project-URL: Documentation, https://github.com/khodnevis-app/development_tools
 Project-URL: Source, https://github.com/khodnevis-app/development_tools
 Project-URL: Tracker, https://github.com/khodnevis-app/development_tools/issues
@@ -125,11 +125,11 @@
     CustomValidator(10),
 ]
 
 verifier = EmailVerifier(email)
 verifier.verify(validators)
 
 
-#### Copyright (c) 2023, Khodnevisai.com (Mahdi Niknejad).
-
 ```
 
+#### Copyright (c) 2023, Khodnevisai.com (Mahdi Niknejad).
+
```

### Comparing `email_domain_verification-1.0.1/email_domain_verification/interfaces.py` & `email_domain_verification-1.0.2/email_domain_verification/interfaces.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-1.0.1/email_domain_verification/utils.py` & `email_domain_verification-1.0.2/email_domain_verification/utils.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-1.0.1/email_domain_verification/validators.py` & `email_domain_verification-1.0.2/email_domain_verification/validators.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-1.0.1/email_domain_verification/verification.py` & `email_domain_verification-1.0.2/email_domain_verification/verification.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-1.0.1/email_domain_verification.egg-info/PKG-INFO` & `email_domain_verification-1.0.2/email_domain_verification.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-domain-verification
-Version: 1.0.1
+Version: 1.0.2
 Summary: Can Verify All The Email Forms And Domains
 Home-page: https://github.com/khodnevis-app/development_tools
 Author: Mahdi Niknejad
 Author-email: mmahdiniknejad@gmail.com
 Project-URL: Documentation, https://github.com/khodnevis-app/development_tools
 Project-URL: Source, https://github.com/khodnevis-app/development_tools
 Project-URL: Tracker, https://github.com/khodnevis-app/development_tools/issues
@@ -125,11 +125,11 @@
     CustomValidator(10),
 ]
 
 verifier = EmailVerifier(email)
 verifier.verify(validators)
 
 
-#### Copyright (c) 2023, Khodnevisai.com (Mahdi Niknejad).
-
 ```
 
+#### Copyright (c) 2023, Khodnevisai.com (Mahdi Niknejad).
+
```

### Comparing `email_domain_verification-1.0.1/setup.py` & `email_domain_verification-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,25 +103,25 @@
     CustomValidator(10),
 ]
 
 verifier = EmailVerifier(email)
 verifier.verify(validators)
 
 
-#### Copyright (c) 2023, Khodnevisai.com (Mahdi Niknejad).
-
 ```
 
+#### Copyright (c) 2023, Khodnevisai.com (Mahdi Niknejad).
+
 """
 )
 
 if __name__ == "__main__":
     setuptools.setup(
         name="email_domain_verification",
-        version="1.0.1",
+        version="1.0.2",
         description="Can Verify All The Email Forms And Domains",
         author="Mahdi Niknejad",
         author_email="mmahdiniknejad@gmail.com",
         url="https://github.com/khodnevis-app/development_tools",
         project_urls={
             "Documentation": "https://github.com/khodnevis-app/development_tools",
             "Source": "https://github.com/khodnevis-app/development_tools",
```

