# Comparing `tmp/ProxyEater-1.5.2.tar.gz` & `tmp/ProxyEater-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProxyEater-1.5.2.tar", last modified: Thu Jul  6 06:57:23 2023, max compression
+gzip compressed data, was "ProxyEater-1.5.3.tar", last modified: Wed Jul 12 16:28:30 2023, max compression
```

## Comparing `ProxyEater-1.5.2.tar` & `ProxyEater-1.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/ProxyEater/
--rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/sources.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/ProxyEater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:28:30.649448 ProxyEater-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-12 16:28:18.000000 ProxyEater-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 16:28:18.000000 ProxyEater-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-12 16:28:30.649448 ProxyEater-1.5.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:28:30.649448 ProxyEater-1.5.3/ProxyEater/
+-rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-07-12 16:28:18.000000 ProxyEater-1.5.3/ProxyEater/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-07-12 16:28:18.000000 ProxyEater-1.5.3/ProxyEater/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-12 16:28:18.000000 ProxyEater-1.5.3/ProxyEater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-07-12 16:28:18.000000 ProxyEater-1.5.3/ProxyEater/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-12 16:28:18.000000 ProxyEater-1.5.3/ProxyEater/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:28:30.649448 ProxyEater-1.5.3/ProxyEater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-12 16:28:30.000000 ProxyEater-1.5.3/ProxyEater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 16:28:30.000000 ProxyEater-1.5.3/ProxyEater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:28:30.000000 ProxyEater-1.5.3/ProxyEater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 16:28:30.000000 ProxyEater-1.5.3/ProxyEater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-12 16:28:30.000000 ProxyEater-1.5.3/ProxyEater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 16:28:30.000000 ProxyEater-1.5.3/ProxyEater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-12 16:28:18.000000 ProxyEater-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-12 16:28:18.000000 ProxyEater-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:28:30.649448 ProxyEater-1.5.3/setup.cfg
```

### Comparing `ProxyEater-1.5.2/LICENSE` & `ProxyEater-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ProxyEater-1.5.2/PKG-INFO` & `ProxyEater-1.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: ProxyEater
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Python Proxy Scraper for gathering fresh proxies.
-Home-page: https://github.com/MPCodeWriter21/ProxyEater
-Author: CodeWriter21
-Author-email: CodeWriter21@gmail.com
+Author-email: "CodeWriter21 (MehardP21)" <CodeWriter21@gmail.com>
+License: Apache License 2.0
+Project-URL: Homepage, https://github.com/MPCodeWriter21/ProxyEater
+Project-URL: Donations, https://github.com/MPCodeWriter21/ProxyEater/blob/master/DONATE.md
+Project-URL: Source, https://github.com/MPCodeWriter21/ProxyEater
+Keywords: python,python3,proxy,proxylist,ProxyEater
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
-ProxyEater\[1.5.2\]
+ProxyEater\[1.5.3\]
 ===================
 
 ![version](https://img.shields.io/pypi/v/ProxyEater)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/ProxyEater)
 [![CodeFactor](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater/badge)](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater)
 
 A Python Proxy Scraper for gathering fresh proxies.
```

### Comparing `ProxyEater-1.5.2/ProxyEater/Proxy.py` & `ProxyEater-1.5.3/ProxyEater/Proxy.py`

 * *Files identical despite different names*

### Comparing `ProxyEater-1.5.2/ProxyEater/Scraper.py` & `ProxyEater-1.5.3/ProxyEater/Scraper.py`

 * *Files identical despite different names*

### Comparing `ProxyEater-1.5.2/ProxyEater/__main__.py` & `ProxyEater-1.5.3/ProxyEater/__main__.py`

 * *Files identical despite different names*

### Comparing `ProxyEater-1.5.2/ProxyEater/sources.json` & `ProxyEater-1.5.3/ProxyEater/sources.json`

 * *Files identical despite different names*

### Comparing `ProxyEater-1.5.2/ProxyEater.egg-info/PKG-INFO` & `ProxyEater-1.5.3/ProxyEater.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: ProxyEater
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Python Proxy Scraper for gathering fresh proxies.
-Home-page: https://github.com/MPCodeWriter21/ProxyEater
-Author: CodeWriter21
-Author-email: CodeWriter21@gmail.com
+Author-email: "CodeWriter21 (MehardP21)" <CodeWriter21@gmail.com>
+License: Apache License 2.0
+Project-URL: Homepage, https://github.com/MPCodeWriter21/ProxyEater
+Project-URL: Donations, https://github.com/MPCodeWriter21/ProxyEater/blob/master/DONATE.md
+Project-URL: Source, https://github.com/MPCodeWriter21/ProxyEater
+Keywords: python,python3,proxy,proxylist,ProxyEater
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
-ProxyEater\[1.5.2\]
+ProxyEater\[1.5.3\]
 ===================
 
 ![version](https://img.shields.io/pypi/v/ProxyEater)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/ProxyEater)
 [![CodeFactor](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater/badge)](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater)
 
 A Python Proxy Scraper for gathering fresh proxies.
```

### Comparing `ProxyEater-1.5.2/README.md` & `ProxyEater-1.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ProxyEater\[1.5.2\]
+ProxyEater\[1.5.3\]
 ===================
 
 ![version](https://img.shields.io/pypi/v/ProxyEater)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/ProxyEater)
 [![CodeFactor](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater/badge)](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater)
 
 A Python Proxy Scraper for gathering fresh proxies.
```

