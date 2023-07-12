# Comparing `tmp/refunc-cli-1.2.2.tar.gz` & `tmp/refunc-cli-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refunc-cli-1.2.2.tar", last modified: Fri Apr 28 05:23:23 2023, max compression
+gzip compressed data, was "refunc-cli-1.2.3.tar", last modified: Wed Jul 12 10:17:01 2023, max compression
```

## Comparing `refunc-cli-1.2.2.tar` & `refunc-cli-1.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/MANIFEST.in
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      494 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/README.md
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:23:23.499520 refunc-cli-1.2.2/refunc_cli.egg-info/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      600 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/entry_points.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/not-zip-safe
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      114 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/requires.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/top_level.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      113 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/requirements.txt
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/rfctl/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2432 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/__main__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1561 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/awslocal.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3738 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/build.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/rfctl/client/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       33 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/client/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1449 2023-04-28 05:20:56.000000 refunc-cli-1.2.2/rfctl/client/client.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      841 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/create.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/create_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/delete.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/delete_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/get.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/get_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3152 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/init.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1458 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/init_source.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/schema.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      680 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/update_code.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      645 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/update_config.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/setup.cfg
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2023-04-28 05:22:41.000000 refunc-cli-1.2.2/setup.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-07-12 10:17:01.988620 refunc-cli-1.2.3/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/MANIFEST.in
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-07-12 10:17:01.988620 refunc-cli-1.2.3/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      494 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/README.md
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-07-12 10:17:01.980620 refunc-cli-1.2.3/refunc_cli.egg-info/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-07-12 10:17:01.000000 refunc-cli-1.2.3/refunc_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      600 2023-07-12 10:17:01.000000 refunc-cli-1.2.3/refunc_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-07-12 10:17:01.000000 refunc-cli-1.2.3/refunc_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2023-07-12 10:17:01.000000 refunc-cli-1.2.3/refunc_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-07-12 10:17:01.000000 refunc-cli-1.2.3/refunc_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      114 2023-07-12 10:17:01.000000 refunc-cli-1.2.3/refunc_cli.egg-info/requires.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2023-07-12 10:17:01.000000 refunc-cli-1.2.3/refunc_cli.egg-info/top_level.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      113 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/requirements.txt
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-07-12 10:17:01.988620 refunc-cli-1.2.3/rfctl/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2432 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/__main__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1561 2023-07-12 10:13:25.000000 refunc-cli-1.2.3/rfctl/awslocal.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3738 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/build.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-07-12 10:17:01.988620 refunc-cli-1.2.3/rfctl/client/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       33 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/client/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1557 2023-07-12 10:14:57.000000 refunc-cli-1.2.3/rfctl/client/client.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      841 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/create.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/create_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/delete.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/delete_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/get.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/get_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3152 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/init.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1458 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/init_source.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/schema.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      680 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/update_code.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      645 2023-04-28 05:17:10.000000 refunc-cli-1.2.3/rfctl/update_config.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-07-12 10:17:01.988620 refunc-cli-1.2.3/setup.cfg
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2023-07-12 10:15:04.000000 refunc-cli-1.2.3/setup.py
```

### Comparing `refunc-cli-1.2.2/refunc_cli.egg-info/SOURCES.txt` & `refunc-cli-1.2.3/refunc_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/rfctl/__main__.py` & `refunc-cli-1.2.3/rfctl/__main__.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/rfctl/awslocal.py` & `refunc-cli-1.2.3/rfctl/awslocal.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/rfctl/build.py` & `refunc-cli-1.2.3/rfctl/build.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/rfctl/create.py` & `refunc-cli-1.2.3/rfctl/create.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/rfctl/init.py` & `refunc-cli-1.2.3/rfctl/init.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/rfctl/init_source.py` & `refunc-cli-1.2.3/rfctl/init_source.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/rfctl/schema.py` & `refunc-cli-1.2.3/rfctl/schema.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/rfctl/update_code.py` & `refunc-cli-1.2.3/rfctl/update_code.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/rfctl/update_config.py` & `refunc-cli-1.2.3/rfctl/update_config.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.2/setup.py` & `refunc-cli-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 os.chdir(os.path.dirname(sys.argv[0]) or ".")
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup_args = dict(
     name='refunc-cli',
-    version='1.2.2',
+    version='1.2.3',
     description='refunc command line tools',
     author='arvin',
     license='MIT',
     url='https://github.com/refunc/refunc-cli',
     author_email='arvintian8@gamil.com',
     packages=find_packages(),
     include_package_data=True,
```

