# Comparing `tmp/dummy_url_wrapper-0.0.4.tar.gz` & `tmp/dummy_url_wrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dummy_url_wrapper-0.0.4.tar", last modified: Tue Jul 11 12:22:50 2023, max compression
+gzip compressed data, was "dummy_url_wrapper-0.0.5.tar", last modified: Wed Jul 12 09:54:31 2023, max compression
```

## Comparing `dummy_url_wrapper-0.0.4.tar` & `dummy_url_wrapper-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 12:22:50.956954 dummy_url_wrapper-0.0.4/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-11 12:22:50.956954 dummy_url_wrapper-0.0.4/PKG-INFO
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 12:22:50.956954 dummy_url_wrapper-0.0.4/dummy_url_wrapper/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       67 2023-07-11 04:13:41.000000 dummy_url_wrapper-0.0.4/dummy_url_wrapper/__init__.py
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      690 2023-07-11 12:22:24.000000 dummy_url_wrapper-0.0.4/dummy_url_wrapper/mysdk.py
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-11 12:22:50.956954 dummy_url_wrapper-0.0.4/dummy_url_wrapper.egg-info/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-11 12:22:50.000000 dummy_url_wrapper-0.0.4/dummy_url_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      269 2023-07-11 12:22:50.000000 dummy_url_wrapper-0.0.4/dummy_url_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-11 12:22:50.000000 dummy_url_wrapper-0.0.4/dummy_url_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       23 2023-07-11 12:22:50.000000 dummy_url_wrapper-0.0.4/dummy_url_wrapper.egg-info/requires.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       18 2023-07-11 12:22:50.000000 dummy_url_wrapper-0.0.4/dummy_url_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-11 12:22:50.956954 dummy_url_wrapper-0.0.4/setup.cfg
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      886 2023-07-11 12:22:32.000000 dummy_url_wrapper-0.0.4/setup.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-12 09:54:31.833893 dummy_url_wrapper-0.0.5/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-12 09:54:31.833893 dummy_url_wrapper-0.0.5/PKG-INFO
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-12 09:54:31.829893 dummy_url_wrapper-0.0.5/dummy_url_wrapper/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       67 2023-07-11 04:13:41.000000 dummy_url_wrapper-0.0.5/dummy_url_wrapper/__init__.py
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      877 2023-07-12 09:46:43.000000 dummy_url_wrapper-0.0.5/dummy_url_wrapper/mysdk.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-12 09:54:31.833893 dummy_url_wrapper-0.0.5/dummy_url_wrapper.egg-info/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-12 09:54:31.000000 dummy_url_wrapper-0.0.5/dummy_url_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      269 2023-07-12 09:54:31.000000 dummy_url_wrapper-0.0.5/dummy_url_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-12 09:54:31.000000 dummy_url_wrapper-0.0.5/dummy_url_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       23 2023-07-12 09:54:31.000000 dummy_url_wrapper-0.0.5/dummy_url_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       18 2023-07-12 09:54:31.000000 dummy_url_wrapper-0.0.5/dummy_url_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-12 09:54:31.833893 dummy_url_wrapper-0.0.5/setup.cfg
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      886 2023-07-12 09:45:32.000000 dummy_url_wrapper-0.0.5/setup.py
```

### Comparing `dummy_url_wrapper-0.0.4/PKG-INFO` & `dummy_url_wrapper-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummy_url_wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package provides the wrapping of URLs for not exposing to clients
 Home-page: https://github.com/nk2909/Python-SDK.git
 Author: Nishant Kabariya
 Author-email: testurl@yopmail.com
 Keywords: python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `dummy_url_wrapper-0.0.4/dummy_url_wrapper.egg-info/PKG-INFO` & `dummy_url_wrapper-0.0.5/dummy_url_wrapper.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummy-url-wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package provides the wrapping of URLs for not exposing to clients
 Home-page: https://github.com/nk2909/Python-SDK.git
 Author: Nishant Kabariya
 Author-email: testurl@yopmail.com
 Keywords: python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `dummy_url_wrapper-0.0.4/setup.py` & `dummy_url_wrapper-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dummy_url_wrapper",
-    version="0.0.4",
+    version="0.0.5",
     description="This package provides the wrapping of URLs for not exposing to clients",
     url="https://github.com/nk2909/Python-SDK.git",
     author="Nishant Kabariya",
     author_email="testurl@yopmail.com",
     install_requires=["python-dotenv", "requests"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

