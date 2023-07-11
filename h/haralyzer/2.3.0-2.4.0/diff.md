# Comparing `tmp/haralyzer-2.3.0.tar.gz` & `tmp/haralyzer-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haralyzer-2.3.0.tar", last modified: Thu Jun 15 07:40:00 2023, max compression
+gzip compressed data, was "haralyzer-2.4.0.tar", last modified: Tue Jul 11 22:00:07 2023, max compression
```

## Comparing `haralyzer-2.3.0.tar` & `haralyzer-2.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:40:00.141870 haralyzer-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-15 07:39:49.000000 haralyzer-2.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-15 07:40:00.141870 haralyzer-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 07:39:49.000000 haralyzer-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:40:00.141870 haralyzer-2.3.0/haralyzer/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33811 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/multihar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:40:00.141870 haralyzer-2.3.0/haralyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 07:40:00.000000 haralyzer-2.3.0/haralyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 07:40:00.141870 haralyzer-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-15 07:39:49.000000 haralyzer-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:00:07.344852 haralyzer-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-11 21:59:55.000000 haralyzer-2.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-11 22:00:07.344852 haralyzer-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-11 21:59:55.000000 haralyzer-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:00:07.344852 haralyzer-2.4.0/haralyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 21:59:55.000000 haralyzer-2.4.0/haralyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33811 2023-07-11 21:59:55.000000 haralyzer-2.4.0/haralyzer/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-11 21:59:55.000000 haralyzer-2.4.0/haralyzer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-11 21:59:55.000000 haralyzer-2.4.0/haralyzer/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-11 21:59:55.000000 haralyzer-2.4.0/haralyzer/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-11 21:59:55.000000 haralyzer-2.4.0/haralyzer/multihar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:00:07.344852 haralyzer-2.4.0/haralyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-11 22:00:07.000000 haralyzer-2.4.0/haralyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 22:00:07.000000 haralyzer-2.4.0/haralyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:00:07.000000 haralyzer-2.4.0/haralyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:00:07.000000 haralyzer-2.4.0/haralyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 22:00:07.000000 haralyzer-2.4.0/haralyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 22:00:07.000000 haralyzer-2.4.0/haralyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-11 22:00:07.344852 haralyzer-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-11 21:59:55.000000 haralyzer-2.4.0/setup.py
```

### Comparing `haralyzer-2.3.0/LICENSE.txt` & `haralyzer-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `haralyzer-2.3.0/PKG-INFO` & `haralyzer-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haralyzer
-Version: 2.3.0
+Version: 2.4.0
 Summary: A python framework for getting useful stuff out of HAR files
 Home-page: https://github.com/haralyzer/haralyzer
 Author: Justin Crown
 Author-email: justincrown1@gmail.com
 License: MIT
 Download-URL: https://github.com/haralyzer/haralyzer/releases/latest
 Project-URL: Changelog, https://github.com/haralyzer/haralyzer/blob/master/HISTORY.rst
```

### Comparing `haralyzer-2.3.0/README.rst` & `haralyzer-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `haralyzer-2.3.0/haralyzer/assets.py` & `haralyzer-2.4.0/haralyzer/assets.py`

 * *Files identical despite different names*

### Comparing `haralyzer-2.3.0/haralyzer/http.py` & `haralyzer-2.4.0/haralyzer/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,16 @@
     def text(self) -> Optional[str]:
         """
         :return: Request body
         :rtype: str
         """
         if "postData" not in self.raw_entry:
             return None
-        return self.raw_entry["postData"].get("text")
+        post_data = self.raw_entry["postData"]
+        return post_data.get("_textBase64", post_data.get("text"))
 
 
 class Response(HttpTransaction):
     """Response object for a HarEntry"""
 
     def __init__(self, url: str, entry: dict):
         """
```

### Comparing `haralyzer-2.3.0/haralyzer/mixins.py` & `haralyzer-2.4.0/haralyzer/mixins.py`

 * *Files identical despite different names*

### Comparing `haralyzer-2.3.0/haralyzer/multihar.py` & `haralyzer-2.4.0/haralyzer/multihar.py`

 * *Files identical despite different names*

### Comparing `haralyzer-2.3.0/haralyzer.egg-info/PKG-INFO` & `haralyzer-2.4.0/haralyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haralyzer
-Version: 2.3.0
+Version: 2.4.0
 Summary: A python framework for getting useful stuff out of HAR files
 Home-page: https://github.com/haralyzer/haralyzer
 Author: Justin Crown
 Author-email: justincrown1@gmail.com
 License: MIT
 Download-URL: https://github.com/haralyzer/haralyzer/releases/latest
 Project-URL: Changelog, https://github.com/haralyzer/haralyzer/blob/master/HISTORY.rst
```

### Comparing `haralyzer-2.3.0/setup.py` & `haralyzer-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 test_reqs = open("requirements-dev.txt").readlines()
 
 
 readme = open('README.rst').read()
 
 setup(
         name='haralyzer',
-        version='2.3.0',
+        version='2.4.0',
         description='A python framework for getting useful stuff out of HAR files',
         long_description=readme,
         long_description_content_type="text/x-rst",
         author='Justin Crown',
         author_email='justincrown1@gmail.com',
         url='https://github.com/haralyzer/haralyzer',
         download_url='https://github.com/haralyzer/haralyzer/releases/latest',
```

