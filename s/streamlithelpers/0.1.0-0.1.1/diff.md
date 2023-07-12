# Comparing `tmp/streamlithelpers-0.1.0.tar.gz` & `tmp/streamlithelpers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlithelpers-0.1.0.tar", last modified: Wed Jul 12 10:43:27 2023, max compression
+gzip compressed data, was "streamlithelpers-0.1.1.tar", last modified: Wed Jul 12 10:53:05 2023, max compression
```

## Comparing `streamlithelpers-0.1.0.tar` & `streamlithelpers-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:43:27.185052 streamlithelpers-0.1.0/
--rw-r--r--   0 adr27     (1415) adr27     (1415)     1063 2023-07-12 10:26:30.000000 streamlithelpers-0.1.0/LICENSE.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 10:43:27.185124 streamlithelpers-0.1.0/PKG-INFO
--rw-r--r--   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:16:18.000000 streamlithelpers-0.1.0/README.md
--rw-r--r--   0 adr27     (1415) adr27     (1415)       79 2023-07-12 10:43:27.185479 streamlithelpers-0.1.0/setup.cfg
--rw-r--r--   0 adr27     (1415) adr27     (1415)      806 2023-07-12 10:42:46.000000 streamlithelpers-0.1.0/setup.py
-drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:43:27.184169 streamlithelpers-0.1.0/streamlithelpers/
--rw-r--r--   0 adr27     (1415) adr27     (1415)      218 2023-07-12 10:14:52.000000 streamlithelpers-0.1.0/streamlithelpers/__init__.py
--rw-r--r--   0 adr27     (1415) adr27     (1415)    10198 2023-07-12 10:14:52.000000 streamlithelpers-0.1.0/streamlithelpers/streamlit_helpers.py
-drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:43:27.184934 streamlithelpers-0.1.0/streamlithelpers.egg-info/
--rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 10:43:27.000000 streamlithelpers-0.1.0/streamlithelpers.egg-info/PKG-INFO
--rw-rw-r--   0 adr27     (1415) adr27     (1415)      306 2023-07-12 10:43:27.000000 streamlithelpers-0.1.0/streamlithelpers.egg-info/SOURCES.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)        1 2023-07-12 10:43:27.000000 streamlithelpers-0.1.0/streamlithelpers.egg-info/dependency_links.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)       31 2023-07-12 10:43:27.000000 streamlithelpers-0.1.0/streamlithelpers.egg-info/requires.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)       17 2023-07-12 10:43:27.000000 streamlithelpers-0.1.0/streamlithelpers.egg-info/top_level.txt
+drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:53:05.777004 streamlithelpers-0.1.1/
+-rw-r--r--   0 adr27     (1415) adr27     (1415)     1063 2023-07-12 10:26:30.000000 streamlithelpers-0.1.1/LICENSE.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 10:53:05.777074 streamlithelpers-0.1.1/PKG-INFO
+-rw-r--r--   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:16:18.000000 streamlithelpers-0.1.1/README.md
+-rw-r--r--   0 adr27     (1415) adr27     (1415)       79 2023-07-12 10:53:05.779126 streamlithelpers-0.1.1/setup.cfg
+-rw-r--r--   0 adr27     (1415) adr27     (1415)      806 2023-07-12 10:51:30.000000 streamlithelpers-0.1.1/setup.py
+drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:53:05.776133 streamlithelpers-0.1.1/streamlithelpers/
+-rw-r--r--   0 adr27     (1415) adr27     (1415)      220 2023-07-12 10:51:30.000000 streamlithelpers-0.1.1/streamlithelpers/__init__.py
+-rw-r--r--   0 adr27     (1415) adr27     (1415)    10198 2023-07-12 10:14:52.000000 streamlithelpers-0.1.1/streamlithelpers/streamlit_helpers.py
+drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:53:05.776901 streamlithelpers-0.1.1/streamlithelpers.egg-info/
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/PKG-INFO
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)      306 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)        1 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)       31 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/requires.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)       17 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/top_level.txt
```

### Comparing `streamlithelpers-0.1.0/LICENSE.txt` & `streamlithelpers-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlithelpers-0.1.0/PKG-INFO` & `streamlithelpers-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlithelpers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple utilities to help streamlit app development
 Home-page: https://github.com/andehr/streamlit-helpers
-Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.1.tar.gz
 Author: Andrew Robertson
 Author-email: 
 License: MIT
 Keywords: streamlit,utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `streamlithelpers-0.1.0/setup.py` & `streamlithelpers-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name='streamlithelpers',
     packages=['streamlithelpers'],
-    version='0.1.0',
+    version='0.1.1',
     license='MIT',
     description='Simple utilities to help streamlit app development',
     author='Andrew Robertson',
     author_email='',
     url='https://github.com/andehr/streamlit-helpers',
-    download_url='https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.0.tar.gz',
+    download_url='https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.1.tar.gz',
     keywords=['streamlit', 'utility'],
     install_requires=[
         'pandas',
         'streamlit',
         'streamlit-ace'
     ],
     classifiers=[
```

### Comparing `streamlithelpers-0.1.0/streamlithelpers/streamlit_helpers.py` & `streamlithelpers-0.1.1/streamlithelpers/streamlit_helpers.py`

 * *Files identical despite different names*

### Comparing `streamlithelpers-0.1.0/streamlithelpers.egg-info/PKG-INFO` & `streamlithelpers-0.1.1/streamlithelpers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlithelpers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple utilities to help streamlit app development
 Home-page: https://github.com/andehr/streamlit-helpers
-Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.1.tar.gz
 Author: Andrew Robertson
 Author-email: 
 License: MIT
 Keywords: streamlit,utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

