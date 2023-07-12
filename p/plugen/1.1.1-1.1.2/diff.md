# Comparing `tmp/plugen-1.1.1.tar.gz` & `tmp/plugen-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugen-1.1.1.tar", last modified: Wed Jul 12 19:06:24 2023, max compression
+gzip compressed data, was "plugen-1.1.2.tar", last modified: Wed Jul 12 19:07:10 2023, max compression
```

## Comparing `plugen-1.1.1.tar` & `plugen-1.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.281000 plugen-1.1.1/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4017 2023-07-12 19:06:24.281000 plugen-1.1.1/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     3761 2023-07-12 19:04:47.000000 plugen-1.1.1/README.md
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.277000 plugen-1.1.1/plugen/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       19 2023-07-10 05:15:24.000000 plugen-1.1.1/plugen/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.281000 plugen-1.1.1/plugen/lib/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-1.1.1/plugen/lib/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-1.1.1/plugen/lib/build.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      256 2023-07-12 05:01:03.000000 plugen-1.1.1/plugen/lib/init.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1968 2023-07-09 18:38:01.000000 plugen-1.1.1/plugen/lib/plugin.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-1.1.1/plugen/lib/serve.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-1.1.1/plugen/lib/utils.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1927 2023-07-12 05:01:40.000000 plugen-1.1.1/plugen/main.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.281000 plugen-1.1.1/plugen/plugins/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.1/plugen/plugins/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.281000 plugen-1.1.1/plugen/plugins/copydest/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.1/plugen/plugins/copydest/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      677 2023-07-12 05:19:15.000000 plugen-1.1.1/plugen/plugins/copydest/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.281000 plugen-1.1.1/plugen/plugins/hotreload/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.1/plugen/plugins/hotreload/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-1.1.1/plugen/plugins/hotreload/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.281000 plugen-1.1.1/plugen/plugins/imagecompressor/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.1/plugen/plugins/imagecompressor/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-1.1.1/plugen/plugins/imagecompressor/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.281000 plugen-1.1.1/plugen/plugins/sass/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.1/plugen/plugins/sass/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-1.1.1/plugen/plugins/sass/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.281000 plugen-1.1.1/plugen/plugins/tailwind/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.1/plugen/plugins/tailwind/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1356 2023-07-12 05:25:42.000000 plugen-1.1.1/plugen/plugins/tailwind/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:06:24.281000 plugen-1.1.1/plugen.egg-info/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4017 2023-07-12 19:06:24.000000 plugen-1.1.1/plugen.egg-info/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      792 2023-07-12 19:06:24.000000 plugen-1.1.1/plugen.egg-info/SOURCES.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-12 19:06:24.000000 plugen-1.1.1/plugen.egg-info/dependency_links.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-12 19:06:24.000000 plugen-1.1.1/plugen.egg-info/entry_points.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       18 2023-07-12 19:06:24.000000 plugen-1.1.1/plugen.egg-info/requires.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-12 19:06:24.000000 plugen-1.1.1/plugen.egg-info/top_level.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-12 19:06:24.281000 plugen-1.1.1/setup.cfg
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      643 2023-07-12 19:06:21.000000 plugen-1.1.1/setup.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4017 2023-07-12 19:07:10.917056 plugen-1.1.2/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     3761 2023-07-12 19:04:47.000000 plugen-1.1.2/README.md
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/plugen/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       19 2023-07-10 05:15:24.000000 plugen-1.1.2/plugen/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/plugen/lib/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-1.1.2/plugen/lib/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-1.1.2/plugen/lib/build.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      256 2023-07-12 05:01:03.000000 plugen-1.1.2/plugen/lib/init.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1968 2023-07-09 18:38:01.000000 plugen-1.1.2/plugen/lib/plugin.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-1.1.2/plugen/lib/serve.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-1.1.2/plugen/lib/utils.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1927 2023-07-12 05:01:40.000000 plugen-1.1.2/plugen/main.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/plugen/plugins/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.2/plugen/plugins/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/plugen/plugins/copydest/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.2/plugen/plugins/copydest/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      677 2023-07-12 05:19:15.000000 plugen-1.1.2/plugen/plugins/copydest/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/plugen/plugins/hotreload/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.2/plugen/plugins/hotreload/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-1.1.2/plugen/plugins/hotreload/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/plugen/plugins/imagecompressor/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.2/plugen/plugins/imagecompressor/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-1.1.2/plugen/plugins/imagecompressor/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/plugen/plugins/sass/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.2/plugen/plugins/sass/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-1.1.2/plugen/plugins/sass/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/plugen/plugins/tailwind/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.2/plugen/plugins/tailwind/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1356 2023-07-12 05:25:42.000000 plugen-1.1.2/plugen/plugins/tailwind/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:07:10.917056 plugen-1.1.2/plugen.egg-info/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4017 2023-07-12 19:07:10.000000 plugen-1.1.2/plugen.egg-info/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      792 2023-07-12 19:07:10.000000 plugen-1.1.2/plugen.egg-info/SOURCES.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-12 19:07:10.000000 plugen-1.1.2/plugen.egg-info/dependency_links.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-12 19:07:10.000000 plugen-1.1.2/plugen.egg-info/entry_points.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       18 2023-07-12 19:07:10.000000 plugen-1.1.2/plugen.egg-info/requires.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-12 19:07:10.000000 plugen-1.1.2/plugen.egg-info/top_level.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-12 19:07:10.917056 plugen-1.1.2/setup.cfg
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      693 2023-07-12 19:07:08.000000 plugen-1.1.2/setup.py
```

### Comparing `plugen-1.1.1/PKG-INFO` & `plugen-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugen
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/aclarembeau/plugen
 Author: Clarembeau Alexis
 Author-email: alexis.clarembeau@gmail.com
 License: MIT
 Keywords: static website generator
 Description-Content-Type: text/markdown
```

### Comparing `plugen-1.1.1/README.md` & `plugen-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen/lib/build.py` & `plugen-1.1.2/plugen/lib/build.py`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen/lib/plugin.py` & `plugen-1.1.2/plugen/lib/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen/lib/serve.py` & `plugen-1.1.2/plugen/lib/serve.py`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen/lib/utils.py` & `plugen-1.1.2/plugen/lib/utils.py`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen/main.py` & `plugen-1.1.2/plugen/main.py`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen/plugins/copydest/plugin.py` & `plugen-1.1.2/plugen/plugins/copydest/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen/plugins/hotreload/plugin.py` & `plugen-1.1.2/plugen/plugins/hotreload/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen/plugins/sass/plugin.py` & `plugen-1.1.2/plugen/plugins/sass/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen/plugins/tailwind/plugin.py` & `plugen-1.1.2/plugen/plugins/tailwind/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/plugen.egg-info/PKG-INFO` & `plugen-1.1.2/plugen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugen
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/aclarembeau/plugen
 Author: Clarembeau Alexis
 Author-email: alexis.clarembeau@gmail.com
 License: MIT
 Keywords: static website generator
 Description-Content-Type: text/markdown
```

### Comparing `plugen-1.1.1/plugen.egg-info/SOURCES.txt` & `plugen-1.1.2/plugen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plugen-1.1.1/setup.py` & `plugen-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 setup(
     entry_points={
         'console_scripts': [
             'plugen = plugen:main',
         ],
     },
     name='plugen',
-    version='1.1.1',
+    version='1.1.2',
     license='MIT',
+    site="https://github.com/aclarembeau/plugen",
     author="Clarembeau Alexis",
     author_email='alexis.clarembeau@gmail.com',
     packages=find_packages('./'),
     package_dir={'': './'},
     url='https://github.com/aclarembeau/plugen',
     keywords='static website generator',
     install_requires=['PyYAML', 'websockets'],
```

