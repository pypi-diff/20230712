# Comparing `tmp/pywinauto-supporter-0.0.2.tar.gz` & `tmp/pywinauto-supporter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywinauto-supporter-0.0.2.tar", last modified: Wed Jul 12 01:43:37 2023, max compression
+gzip compressed data, was "pywinauto-supporter-0.0.3.tar", last modified: Wed Jul 12 01:47:05 2023, max compression
```

## Comparing `pywinauto-supporter-0.0.2.tar` & `pywinauto-supporter-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 01:43:37.317979 pywinauto-supporter-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      923 2023-07-12 01:43:37.317979 pywinauto-supporter-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      656 2023-07-12 01:43:36.000000 pywinauto-supporter-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 01:43:37.316979 pywinauto-supporter-0.0.2/pywinauto_supporter/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 01:43:36.000000 pywinauto-supporter-0.0.2/pywinauto_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-12 01:43:36.000000 pywinauto-supporter-0.0.2/pywinauto_supporter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 01:43:37.317979 pywinauto-supporter-0.0.2/pywinauto_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      923 2023-07-12 01:43:37.000000 pywinauto-supporter-0.0.2/pywinauto_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      335 2023-07-12 01:43:37.000000 pywinauto-supporter-0.0.2/pywinauto_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 01:43:37.000000 pywinauto-supporter-0.0.2/pywinauto_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 01:43:37.000000 pywinauto-supporter-0.0.2/pywinauto_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-12 01:43:37.000000 pywinauto-supporter-0.0.2/pywinauto_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-12 01:43:37.000000 pywinauto-supporter-0.0.2/pywinauto_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 01:43:37.317979 pywinauto-supporter-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      609 2023-07-12 01:43:36.000000 pywinauto-supporter-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 01:47:05.873694 pywinauto-supporter-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-07-12 01:47:05.873694 pywinauto-supporter-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 01:47:05.871693 pywinauto-supporter-0.0.3/pywinauto_supporter/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/pywinauto_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/pywinauto_supporter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 01:47:05.872693 pywinauto-supporter-0.0.3/pywinauto_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/pywinauto_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/pywinauto_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/pywinauto_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/pywinauto_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/pywinauto_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/pywinauto_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 01:47:05.873694 pywinauto-supporter-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-12 01:47:05.000000 pywinauto-supporter-0.0.3/setup.py
```

### Comparing `pywinauto-supporter-0.0.2/PKG-INFO` & `pywinauto-supporter-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinauto-supporter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pywinauto supporter
 Home-page: https://github.com/automatethem/pywinauto-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `pywinauto-supporter-0.0.2/README.md` & `pywinauto-supporter-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pywinauto-supporter-0.0.2/pywinauto_supporter/utils.py` & `pywinauto-supporter-0.0.3/pywinauto_supporter/utils.py`

 * *Files identical despite different names*

### Comparing `pywinauto-supporter-0.0.2/pywinauto_supporter.egg-info/PKG-INFO` & `pywinauto-supporter-0.0.3/pywinauto_supporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinauto-supporter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pywinauto supporter
 Home-page: https://github.com/automatethem/pywinauto-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `pywinauto-supporter-0.0.2/setup.py` & `pywinauto-supporter-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='pywinauto-supporter',
-	version='0.0.2',
+	version='0.0.3',
 	description='Pywinauto supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/pywinauto-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

