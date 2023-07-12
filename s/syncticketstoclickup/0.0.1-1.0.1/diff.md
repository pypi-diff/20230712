# Comparing `tmp/syncticketstoclickup-0.0.1.tar.gz` & `tmp/syncticketstoclickup-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncticketstoclickup-0.0.1.tar", last modified: Wed Jul 12 17:13:07 2023, max compression
+gzip compressed data, was "syncticketstoclickup-1.0.1.tar", last modified: Wed Jul 12 17:56:57 2023, max compression
```

## Comparing `syncticketstoclickup-0.0.1.tar` & `syncticketstoclickup-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:13:07.989059 syncticketstoclickup-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 17:12:56.000000 syncticketstoclickup-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-12 17:13:07.989059 syncticketstoclickup-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 17:12:56.000000 syncticketstoclickup-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:13:07.989059 syncticketstoclickup-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-12 17:12:56.000000 syncticketstoclickup-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:13:07.989059 syncticketstoclickup-0.0.1/syncticketstoclickup/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 17:12:56.000000 syncticketstoclickup-0.0.1/syncticketstoclickup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-12 17:12:56.000000 syncticketstoclickup-0.0.1/syncticketstoclickup/clickup.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 17:12:56.000000 syncticketstoclickup-0.0.1/syncticketstoclickup/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 17:12:56.000000 syncticketstoclickup-0.0.1/syncticketstoclickup/zendesk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-12 17:12:56.000000 syncticketstoclickup-0.0.1/syncticketstoclickup/zendesk_to_clickup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:13:07.989059 syncticketstoclickup-0.0.1/syncticketstoclickup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-12 17:13:07.000000 syncticketstoclickup-0.0.1/syncticketstoclickup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-12 17:13:07.000000 syncticketstoclickup-0.0.1/syncticketstoclickup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:13:07.000000 syncticketstoclickup-0.0.1/syncticketstoclickup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 17:13:07.000000 syncticketstoclickup-0.0.1/syncticketstoclickup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 17:13:07.000000 syncticketstoclickup-0.0.1/syncticketstoclickup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.658749 syncticketstoclickup-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/syncticketstoclickup/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/.env.example
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/clickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/zendesk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-12 17:56:43.000000 syncticketstoclickup-1.0.1/syncticketstoclickup/zendesk_to_clickup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:56:57.662749 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 17:56:57.000000 syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/top_level.txt
```

### Comparing `syncticketstoclickup-0.0.1/LICENSE` & `syncticketstoclickup-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-0.0.1/PKG-INFO` & `syncticketstoclickup-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: syncticketstoclickup
-Version: 0.0.1
+Version: 1.0.1
 Summary: A package that allows to sync tickets from Zendesk to ClickUp.
 Author: abrahamprz (Abraham Perez)
-Author-email: <fcoabrahamprz@gmail.com>
+Author-email: fcoabrahamprz@gmail.com
 Keywords: python,zendesk,clickup,ticket,task,sync,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # zendesk-clickup
 Project that syncs all tickets from Zendesk to ClickUp. This is useful for teams that use them for managing customer support tickets and want to keep the ticket numbers consistent across both platforms.
 
 ## Configuration
```

### Comparing `syncticketstoclickup-0.0.1/README.md` & `syncticketstoclickup-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-0.0.1/setup.py` & `syncticketstoclickup-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from setuptools import setup, find_packages
 
-
-VERSION = "0.0.1"
 DESCRIPTION = "A package that allows to sync tickets from Zendesk to ClickUp."
 
 # Read the contents of the README.md file
-with open('README.md', 'r', encoding='utf-8') as f:
+with open("README.md", "r", encoding="utf-8") as f:
     md_long_description = f.read()
 
 # Setting up
 setup(
     name="syncticketstoclickup",
-    version=VERSION,
+    use_scm_version=True,
+    setup_requires=["setuptools_scm"],
     author="abrahamprz (Abraham Perez)",
-    author_email="<fcoabrahamprz@gmail.com>",
+    author_email="fcoabrahamprz@gmail.com",
     description=DESCRIPTION,
     long_description=md_long_description,  # Use the contents of README.md as the long description
-    long_description_content_type='text/markdown',  # Specify the content type as Markdown
+    long_description_content_type="text/markdown",  # Specify the content type as Markdown
     packages=find_packages(),
     install_requires=["requests", "tqdm", "python-dotenv"],
     keywords=["python", "zendesk", "clickup", "ticket", "task", "sync", "requests"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
+        # "Operating System :: MacOS :: MacOS X",
+        # "Operating System :: Microsoft :: Windows",
+        "License :: OSI Approved :: MIT License",
     ],
     # entry_points={
     #     'console_scripts': [
     #         'sync-zendesk-to-clickup=syncticketstoclickup.main:main'
     #     ]
     # },
 )
```

### Comparing `syncticketstoclickup-0.0.1/syncticketstoclickup/clickup.py` & `syncticketstoclickup-1.0.1/syncticketstoclickup/clickup.py`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-0.0.1/syncticketstoclickup/zendesk.py` & `syncticketstoclickup-1.0.1/syncticketstoclickup/zendesk.py`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-0.0.1/syncticketstoclickup/zendesk_to_clickup.py` & `syncticketstoclickup-1.0.1/syncticketstoclickup/zendesk_to_clickup.py`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-0.0.1/syncticketstoclickup.egg-info/PKG-INFO` & `syncticketstoclickup-1.0.1/syncticketstoclickup.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: syncticketstoclickup
-Version: 0.0.1
+Version: 1.0.1
 Summary: A package that allows to sync tickets from Zendesk to ClickUp.
 Author: abrahamprz (Abraham Perez)
-Author-email: <fcoabrahamprz@gmail.com>
+Author-email: fcoabrahamprz@gmail.com
 Keywords: python,zendesk,clickup,ticket,task,sync,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # zendesk-clickup
 Project that syncs all tickets from Zendesk to ClickUp. This is useful for teams that use them for managing customer support tickets and want to keep the ticket numbers consistent across both platforms.
 
 ## Configuration
```

