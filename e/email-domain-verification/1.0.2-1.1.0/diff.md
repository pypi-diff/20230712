# Comparing `tmp/email_domain_verification-1.0.2.tar.gz` & `tmp/email_domain_verification-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email_domain_verification-1.0.2.tar", last modified: Wed Jul 12 07:47:16 2023, max compression
+gzip compressed data, was "email_domain_verification-1.1.0.tar", last modified: Wed Jul 12 08:39:49 2023, max compression
```

## Comparing `email_domain_verification-1.0.2.tar` & `email_domain_verification-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:47:16.678608 email_domain_verification-1.0.2/
--rw-r--r--   0 geek      (1000) geek      (1000)     3685 2023-07-12 07:47:16.678608 email_domain_verification-1.0.2/PKG-INFO
--rw-r--r--   0 geek      (1000) geek      (1000)       19 2023-07-11 15:17:07.000000 email_domain_verification-1.0.2/README.md
-drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:47:16.676608 email_domain_verification-1.0.2/email_domain_verification/
--rw-r--r--   0 geek      (1000) geek      (1000)       66 2023-07-12 06:04:32.000000 email_domain_verification-1.0.2/email_domain_verification/__init__.py
--rw-r--r--   0 geek      (1000) geek      (1000)      264 2023-07-11 18:04:28.000000 email_domain_verification-1.0.2/email_domain_verification/emails.py
--rw-r--r--   0 geek      (1000) geek      (1000)      670 2023-07-12 05:35:14.000000 email_domain_verification-1.0.2/email_domain_verification/interfaces.py
--rw-r--r--   0 geek      (1000) geek      (1000)      893 2023-07-12 05:46:35.000000 email_domain_verification-1.0.2/email_domain_verification/utils.py
--rw-r--r--   0 geek      (1000) geek      (1000)     4270 2023-07-12 05:42:09.000000 email_domain_verification-1.0.2/email_domain_verification/validators.py
--rw-r--r--   0 geek      (1000) geek      (1000)      885 2023-07-12 06:37:40.000000 email_domain_verification-1.0.2/email_domain_verification/verification.py
-drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 07:47:16.678608 email_domain_verification-1.0.2/email_domain_verification.egg-info/
--rw-r--r--   0 geek      (1000) geek      (1000)     3685 2023-07-12 07:47:15.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/PKG-INFO
--rw-r--r--   0 geek      (1000) geek      (1000)      493 2023-07-12 07:47:16.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/SOURCES.txt
--rw-r--r--   0 geek      (1000) geek      (1000)        1 2023-07-12 07:47:15.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/dependency_links.txt
--rw-r--r--   0 geek      (1000) geek      (1000)        9 2023-07-12 07:47:16.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/requires.txt
--rw-r--r--   0 geek      (1000) geek      (1000)       26 2023-07-12 07:47:16.000000 email_domain_verification-1.0.2/email_domain_verification.egg-info/top_level.txt
--rw-r--r--   0 geek      (1000) geek      (1000)       38 2023-07-12 07:47:16.678608 email_domain_verification-1.0.2/setup.cfg
--rw-r--r--   0 geek      (1000) geek      (1000)     4231 2023-07-12 07:47:12.000000 email_domain_verification-1.0.2/setup.py
+drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 08:39:49.649607 email_domain_verification-1.1.0/
+-rw-r--r--   0 geek      (1000) geek      (1000)     3742 2023-07-12 08:39:49.648607 email_domain_verification-1.1.0/PKG-INFO
+-rw-r--r--   0 geek      (1000) geek      (1000)     2473 2023-07-12 08:37:36.000000 email_domain_verification-1.1.0/README.md
+drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 08:39:49.646607 email_domain_verification-1.1.0/email_domain_verification/
+-rw-r--r--   0 geek      (1000) geek      (1000)       66 2023-07-12 08:37:36.000000 email_domain_verification-1.1.0/email_domain_verification/__init__.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      264 2023-07-12 08:37:36.000000 email_domain_verification-1.1.0/email_domain_verification/emails.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      670 2023-07-12 08:37:36.000000 email_domain_verification-1.1.0/email_domain_verification/interfaces.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      893 2023-07-12 08:37:36.000000 email_domain_verification-1.1.0/email_domain_verification/utils.py
+-rw-r--r--   0 geek      (1000) geek      (1000)     4270 2023-07-12 08:37:36.000000 email_domain_verification-1.1.0/email_domain_verification/validators.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      885 2023-07-12 08:37:36.000000 email_domain_verification-1.1.0/email_domain_verification/verification.py
+drwxr-xr-x   0 geek      (1000) geek      (1000)        0 2023-07-12 08:39:49.648607 email_domain_verification-1.1.0/email_domain_verification.egg-info/
+-rw-r--r--   0 geek      (1000) geek      (1000)     3742 2023-07-12 08:39:48.000000 email_domain_verification-1.1.0/email_domain_verification.egg-info/PKG-INFO
+-rw-r--r--   0 geek      (1000) geek      (1000)      493 2023-07-12 08:39:49.000000 email_domain_verification-1.1.0/email_domain_verification.egg-info/SOURCES.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)        1 2023-07-12 08:39:48.000000 email_domain_verification-1.1.0/email_domain_verification.egg-info/dependency_links.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)        9 2023-07-12 08:39:49.000000 email_domain_verification-1.1.0/email_domain_verification.egg-info/requires.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)       26 2023-07-12 08:39:49.000000 email_domain_verification-1.1.0/email_domain_verification.egg-info/top_level.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)       38 2023-07-12 08:39:49.649607 email_domain_verification-1.1.0/setup.cfg
+-rw-r--r--   0 geek      (1000) geek      (1000)     4288 2023-07-12 08:39:45.000000 email_domain_verification-1.1.0/setup.py
```

### Comparing `email_domain_verification-1.0.2/PKG-INFO` & `email_domain_verification-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: email_domain_verification
-Version: 1.0.2
-Summary: Can Verify All The Email Forms And Domains
-Home-page: https://github.com/khodnevis-app/development_tools
-Author: Mahdi Niknejad
+Version: 1.1.0
+Summary: Email Validator
+Home-page: https://github.com/Khodnevis-Research-Lab/email-domain-verification
+Author: Mahdi Niknejad, Khodnevisai.com
 Author-email: mmahdiniknejad@gmail.com
-Project-URL: Documentation, https://github.com/khodnevis-app/development_tools
-Project-URL: Source, https://github.com/khodnevis-app/development_tools
-Project-URL: Tracker, https://github.com/khodnevis-app/development_tools/issues
+Project-URL: Documentation, https://github.com/Khodnevis-Research-Lab/email-domain-verification
+Project-URL: Source, https://github.com/Khodnevis-Research-Lab/email-domain-verification
+Project-URL: Tracker, https://github.com/Khodnevis-Research-Lab/email-domain-verification/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # Email Domain Verification Package
 this package can provide some email validators with which users can validate their project emails far easily
 
 ## Installation
```

### Comparing `email_domain_verification-1.0.2/email_domain_verification/interfaces.py` & `email_domain_verification-1.1.0/email_domain_verification/interfaces.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-1.0.2/email_domain_verification/utils.py` & `email_domain_verification-1.1.0/email_domain_verification/utils.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-1.0.2/email_domain_verification/validators.py` & `email_domain_verification-1.1.0/email_domain_verification/validators.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-1.0.2/email_domain_verification/verification.py` & `email_domain_verification-1.1.0/email_domain_verification/verification.py`

 * *Files identical despite different names*

### Comparing `email_domain_verification-1.0.2/email_domain_verification.egg-info/PKG-INFO` & `email_domain_verification-1.1.0/email_domain_verification.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: email-domain-verification
-Version: 1.0.2
-Summary: Can Verify All The Email Forms And Domains
-Home-page: https://github.com/khodnevis-app/development_tools
-Author: Mahdi Niknejad
+Version: 1.1.0
+Summary: Email Validator
+Home-page: https://github.com/Khodnevis-Research-Lab/email-domain-verification
+Author: Mahdi Niknejad, Khodnevisai.com
 Author-email: mmahdiniknejad@gmail.com
-Project-URL: Documentation, https://github.com/khodnevis-app/development_tools
-Project-URL: Source, https://github.com/khodnevis-app/development_tools
-Project-URL: Tracker, https://github.com/khodnevis-app/development_tools/issues
+Project-URL: Documentation, https://github.com/Khodnevis-Research-Lab/email-domain-verification
+Project-URL: Source, https://github.com/Khodnevis-Research-Lab/email-domain-verification
+Project-URL: Tracker, https://github.com/Khodnevis-Research-Lab/email-domain-verification/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # Email Domain Verification Package
 this package can provide some email validators with which users can validate their project emails far easily
 
 ## Installation
```

### Comparing `email_domain_verification-1.0.2/setup.py` & `email_domain_verification-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -113,23 +113,23 @@
 
 """
 )
 
 if __name__ == "__main__":
     setuptools.setup(
         name="email_domain_verification",
-        version="1.0.2",
-        description="Can Verify All The Email Forms And Domains",
-        author="Mahdi Niknejad",
+        version="1.1.0",
+        description="Email Validator",
+        author="Mahdi Niknejad, Khodnevisai.com",
         author_email="mmahdiniknejad@gmail.com",
-        url="https://github.com/khodnevis-app/development_tools",
+        url="https://github.com/Khodnevis-Research-Lab/email-domain-verification",
         project_urls={
-            "Documentation": "https://github.com/khodnevis-app/development_tools",
-            "Source": "https://github.com/khodnevis-app/development_tools",
-            "Tracker": "https://github.com/khodnevis-app/development_tools/issues",
+            "Documentation": "https://github.com/Khodnevis-Research-Lab/email-domain-verification",
+            "Source": "https://github.com/Khodnevis-Research-Lab/email-domain-verification",
+            "Tracker": "https://github.com/Khodnevis-Research-Lab/email-domain-verification/issues",
         },
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=["email_domain_verification"],
         package_data={"email_domain_verification": ["py.typed", "*.pyi"]},
         classifiers=[
             "Development Status :: 5 - Production/Stable",
@@ -142,12 +142,12 @@
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "Topic :: Software Development",
         ],
-        python_requires=">=3.10",
+        python_requires=">=3.7",
         install_requires=[
             "requests",
         ],
     )
```

