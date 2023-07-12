# Comparing `tmp/sdbsxwf-20220426.tar.gz` & `tmp/sdbsxwf-20230712.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdbsxwf-20220426.tar", last modified: Mon Apr 25 06:23:24 2022, max compression
+gzip compressed data, was "sdbsxwf-20230712.tar", last modified: Wed Jul 12 07:05:08 2023, max compression
```

## Comparing `sdbsxwf-20220426.tar` & `sdbsxwf-20230712.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-04-25 06:23:24.146033 sdbsxwf-20220426/
--rw-rw-rw-   0        0        0      860 2022-04-25 06:23:24.146033 sdbsxwf-20220426/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-04-25 06:23:24.146033 sdbsxwf-20220426/setup.cfg
--rw-rw-rw-   0        0        0     1298 2022-04-25 06:22:15.000000 sdbsxwf-20220426/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-25 06:23:24.132804 sdbsxwf-20220426/src/
-drwxrwxrwx   0        0        0        0 2022-04-25 06:23:24.135799 sdbsxwf-20220426/src/sdbsxwf/
--rw-rw-rw-   0        0        0      101 2022-04-25 06:23:19.000000 sdbsxwf-20220426/src/sdbsxwf/__init__.py
--rw-rw-rw-   0        0        0      109 2022-04-25 06:21:51.000000 sdbsxwf-20220426/src/sdbsxwf/main.py
--rw-rw-rw-   0        0        0       36 2022-04-25 05:23:40.000000 sdbsxwf-20220426/src/sdbsxwf/mk.py
-drwxrwxrwx   0        0        0        0 2022-04-25 06:23:24.144039 sdbsxwf-20220426/src/sdbsxwf.egg-info/
--rw-rw-rw-   0        0        0      860 2022-04-25 06:23:24.000000 sdbsxwf-20220426/src/sdbsxwf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2022-04-25 06:23:24.000000 sdbsxwf-20220426/src/sdbsxwf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-25 06:23:24.000000 sdbsxwf-20220426/src/sdbsxwf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-04-25 06:23:24.000000 sdbsxwf-20220426/src/sdbsxwf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-04-25 06:23:24.000000 sdbsxwf-20220426/src/sdbsxwf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 07:05:08.319249 sdbsxwf-20230712/
+-rw-rw-rw-   0        0        0      841 2023-07-12 07:05:08.319249 sdbsxwf-20230712/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 07:05:08.320266 sdbsxwf-20230712/setup.cfg
+-rw-rw-rw-   0        0        0     1332 2023-07-12 07:00:24.000000 sdbsxwf-20230712/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:05:08.310280 sdbsxwf-20230712/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 07:05:08.314265 sdbsxwf-20230712/src/sdbsxwf/
+-rw-rw-rw-   0        0        0      101 2022-04-25 06:23:19.000000 sdbsxwf-20230712/src/sdbsxwf/__init__.py
+-rw-rw-rw-   0        0        0      109 2022-04-25 06:21:51.000000 sdbsxwf-20230712/src/sdbsxwf/main.py
+-rw-rw-rw-   0        0        0       36 2022-04-25 05:23:40.000000 sdbsxwf-20230712/src/sdbsxwf/mk.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:05:08.318251 sdbsxwf-20230712/src/sdbsxwf.egg-info/
+-rw-rw-rw-   0        0        0      841 2023-07-12 07:05:08.000000 sdbsxwf-20230712/src/sdbsxwf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-07-12 07:05:08.000000 sdbsxwf-20230712/src/sdbsxwf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 07:05:08.000000 sdbsxwf-20230712/src/sdbsxwf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-12 07:05:08.000000 sdbsxwf-20230712/src/sdbsxwf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 07:05:08.000000 sdbsxwf-20230712/src/sdbsxwf.egg-info/top_level.txt
```

### Comparing `sdbsxwf-20220426/PKG-INFO` & `sdbsxwf-20230712/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sdbsxwf
-Version: 20220426
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: 
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 20230712
+Summary: 个人工具箱
+Home-page: 
+Author: xwf
+Author-email: 453211170@qq.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.5
 Classifier: Programming Language :: Python :: 2.6
@@ -19,8 +17,7 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Utilities
 
 试着改变世界
-
```

### Comparing `sdbsxwf-20220426/setup.py` & `sdbsxwf-20230712/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from distutils.core import setup
 from setuptools import find_packages
  
 setup(name = 'sdbsxwf',     # 包名
-      version = '20220426',  # 版本号
-      description = '',
+      version = '20230712',  # 版本号
+      description = '个人工具箱',
       long_description = '试着改变世界', 
-      author = '',
-      author_email = '',
+      author = 'xwf',
+      author_email = '453211170@qq.com',
       url = '',
       license = '',
       install_requires=[
         'six>=1.5.2',
         'parsel>=1.1',
     ], #申明依赖包
       classifiers = [
```

### Comparing `sdbsxwf-20220426/src/sdbsxwf.egg-info/PKG-INFO` & `sdbsxwf-20230712/src/sdbsxwf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sdbsxwf
-Version: 20220426
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: 
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 20230712
+Summary: 个人工具箱
+Home-page: 
+Author: xwf
+Author-email: 453211170@qq.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.5
 Classifier: Programming Language :: Python :: 2.6
@@ -19,8 +17,7 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Utilities
 
 试着改变世界
-
```

