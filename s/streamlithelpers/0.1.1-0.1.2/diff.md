# Comparing `tmp/streamlithelpers-0.1.1.tar.gz` & `tmp/streamlithelpers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlithelpers-0.1.1.tar", last modified: Wed Jul 12 10:53:05 2023, max compression
+gzip compressed data, was "streamlithelpers-0.1.2.tar", last modified: Wed Jul 12 13:38:07 2023, max compression
```

## Comparing `streamlithelpers-0.1.1.tar` & `streamlithelpers-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:53:05.777004 streamlithelpers-0.1.1/
--rw-r--r--   0 adr27     (1415) adr27     (1415)     1063 2023-07-12 10:26:30.000000 streamlithelpers-0.1.1/LICENSE.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 10:53:05.777074 streamlithelpers-0.1.1/PKG-INFO
--rw-r--r--   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:16:18.000000 streamlithelpers-0.1.1/README.md
--rw-r--r--   0 adr27     (1415) adr27     (1415)       79 2023-07-12 10:53:05.779126 streamlithelpers-0.1.1/setup.cfg
--rw-r--r--   0 adr27     (1415) adr27     (1415)      806 2023-07-12 10:51:30.000000 streamlithelpers-0.1.1/setup.py
-drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:53:05.776133 streamlithelpers-0.1.1/streamlithelpers/
--rw-r--r--   0 adr27     (1415) adr27     (1415)      220 2023-07-12 10:51:30.000000 streamlithelpers-0.1.1/streamlithelpers/__init__.py
--rw-r--r--   0 adr27     (1415) adr27     (1415)    10198 2023-07-12 10:14:52.000000 streamlithelpers-0.1.1/streamlithelpers/streamlit_helpers.py
-drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 10:53:05.776901 streamlithelpers-0.1.1/streamlithelpers.egg-info/
--rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/PKG-INFO
--rw-rw-r--   0 adr27     (1415) adr27     (1415)      306 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/SOURCES.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)        1 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/dependency_links.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)       31 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/requires.txt
--rw-rw-r--   0 adr27     (1415) adr27     (1415)       17 2023-07-12 10:53:05.000000 streamlithelpers-0.1.1/streamlithelpers.egg-info/top_level.txt
+drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 13:38:07.439475 streamlithelpers-0.1.2/
+-rw-r--r--   0 adr27     (1415) adr27     (1415)     1063 2023-07-12 10:26:30.000000 streamlithelpers-0.1.2/LICENSE.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 13:38:07.439591 streamlithelpers-0.1.2/PKG-INFO
+-rw-r--r--   0 adr27     (1415) adr27     (1415)     2804 2023-07-12 13:37:07.000000 streamlithelpers-0.1.2/README.md
+-rw-r--r--   0 adr27     (1415) adr27     (1415)       79 2023-07-12 13:38:07.440012 streamlithelpers-0.1.2/setup.cfg
+-rw-r--r--   0 adr27     (1415) adr27     (1415)      806 2023-07-12 13:35:00.000000 streamlithelpers-0.1.2/setup.py
+drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 13:38:07.438549 streamlithelpers-0.1.2/streamlithelpers/
+-rw-r--r--   0 adr27     (1415) adr27     (1415)      220 2023-07-12 10:51:30.000000 streamlithelpers-0.1.2/streamlithelpers/__init__.py
+-rw-r--r--   0 adr27     (1415) adr27     (1415)    10198 2023-07-12 10:14:52.000000 streamlithelpers-0.1.2/streamlithelpers/streamlit_helpers.py
+drwxrwxr-x   0 adr27     (1415) adr27     (1415)        0 2023-07-12 13:38:07.439298 streamlithelpers-0.1.2/streamlithelpers.egg-info/
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)      561 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/PKG-INFO
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)      306 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)        1 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)       31 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/requires.txt
+-rw-rw-r--   0 adr27     (1415) adr27     (1415)       17 2023-07-12 13:38:07.000000 streamlithelpers-0.1.2/streamlithelpers.egg-info/top_level.txt
```

### Comparing `streamlithelpers-0.1.1/LICENSE.txt` & `streamlithelpers-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlithelpers-0.1.1/PKG-INFO` & `streamlithelpers-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlithelpers
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple utilities to help streamlit app development
 Home-page: https://github.com/andehr/streamlit-helpers
-Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.2.tar.gz
 Author: Andrew Robertson
 Author-email: 
 License: MIT
 Keywords: streamlit,utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `streamlithelpers-0.1.1/setup.py` & `streamlithelpers-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name='streamlithelpers',
     packages=['streamlithelpers'],
-    version='0.1.1',
+    version='0.1.2',
     license='MIT',
     description='Simple utilities to help streamlit app development',
     author='Andrew Robertson',
     author_email='',
     url='https://github.com/andehr/streamlit-helpers',
-    download_url='https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.1.tar.gz',
+    download_url='https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.2.tar.gz',
     keywords=['streamlit', 'utility'],
     install_requires=[
         'pandas',
         'streamlit',
         'streamlit-ace'
     ],
     classifiers=[
```

### Comparing `streamlithelpers-0.1.1/streamlithelpers/streamlit_helpers.py` & `streamlithelpers-0.1.2/streamlithelpers/streamlit_helpers.py`

 * *Files identical despite different names*

### Comparing `streamlithelpers-0.1.1/streamlithelpers.egg-info/PKG-INFO` & `streamlithelpers-0.1.2/streamlithelpers.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlithelpers
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple utilities to help streamlit app development
 Home-page: https://github.com/andehr/streamlit-helpers
-Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/andehr/streamlit-helpers/archive/refs/tags/v0.1.2.tar.gz
 Author: Andrew Robertson
 Author-email: 
 License: MIT
 Keywords: streamlit,utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

