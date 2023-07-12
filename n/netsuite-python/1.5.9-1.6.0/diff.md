# Comparing `tmp/netsuite_python-1.5.9.tar.gz` & `tmp/netsuite_python-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.5.9.tar", last modified: Mon Jun 26 17:16:53 2023, max compression
+gzip compressed data, was "netsuite_python-1.6.0.tar", last modified: Wed Jul 12 18:57:23 2023, max compression
```

## Comparing `netsuite_python-1.5.9.tar` & `netsuite_python-1.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.847256 netsuite_python-1.5.9/
--rw-rw-rw-   0        0        0     5438 2023-06-26 17:16:53.847256 netsuite_python-1.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     5108 2023-04-25 19:14:38.000000 netsuite_python-1.5.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.814255 netsuite_python-1.5.9/netsuite/
--rw-rw-rw-   0        0        0    12080 2023-06-26 17:14:03.000000 netsuite_python-1.5.9/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.823256 netsuite_python-1.5.9/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.5.9/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.828255 netsuite_python-1.5.9/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.5.9/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.5.9/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2579 2023-05-19 19:55:49.000000 netsuite_python-1.5.9/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.5.9/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.5.9/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.5.9/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.831255 netsuite_python-1.5.9/netsuite/netsuite_rest_client/
--rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.5.9/netsuite/netsuite_rest_client/__init__.py
--rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.5.9/netsuite/netsuite_rest_client/rest_api_client.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.833255 netsuite_python-1.5.9/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0    12245 2023-06-26 17:12:39.000000 netsuite_python-1.5.9/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.5.9/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.841255 netsuite_python-1.5.9/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.846255 netsuite_python-1.5.9/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0     5438 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 17:16:53.847256 netsuite_python-1.5.9/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-06-26 17:15:56.000000 netsuite_python-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.461783 netsuite_python-1.6.0/
+-rw-rw-rw-   0        0        0     5438 2023-07-12 18:57:23.460783 netsuite_python-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5108 2023-04-25 19:14:38.000000 netsuite_python-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.430466 netsuite_python-1.6.0/netsuite/
+-rw-rw-rw-   0        0        0    12080 2023-06-26 17:14:03.000000 netsuite_python-1.6.0/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.438783 netsuite_python-1.6.0/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.6.0/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.443783 netsuite_python-1.6.0/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.6.0/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.6.0/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2579 2023-05-19 19:55:49.000000 netsuite_python-1.6.0/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.6.0/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.6.0/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.6.0/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.445783 netsuite_python-1.6.0/netsuite/netsuite_rest_client/
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.6.0/netsuite/netsuite_rest_client/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.6.0/netsuite/netsuite_rest_client/rest_api_client.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.448783 netsuite_python-1.6.0/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12245 2023-06-26 17:12:39.000000 netsuite_python-1.6.0/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6403 2023-07-12 18:56:42.000000 netsuite_python-1.6.0/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.455783 netsuite_python-1.6.0/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.459782 netsuite_python-1.6.0/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0     5438 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 18:57:23.461783 netsuite_python-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-07-12 18:56:53.000000 netsuite_python-1.6.0/setup.py
```

### Comparing `netsuite_python-1.5.9/PKG-INFO` & `netsuite_python-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.5.9
+Version: 1.6.0
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.5.9/README.md` & `netsuite_python-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/Netsuite.py` & `netsuite_python-1.6.0/netsuite/Netsuite.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.6.0/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.6.0/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/api_clients/api_client.py` & `netsuite_python-1.6.0/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/api_clients/configuration.py` & `netsuite_python-1.6.0/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/api_clients/rest.py` & `netsuite_python-1.6.0/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/module_loading.py` & `netsuite_python-1.6.0/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/scripts/cli.py` & `netsuite_python-1.6.0/netsuite/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/settings.py` & `netsuite_python-1.6.0/netsuite/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,18 @@
         getattr(settings, 'NETSUITE', {})
         django_imported = True
     except ImproperlyConfigured as e:
         settings = None
 except ImportError as e:
     settings = None
 
-BASE_DIR = Path(__file__).parent.parent.parent.parent.parent.parent.resolve()
+if os.environ.get('BASE_DIR')is not None:
+    BASE_DIR = Path(os.environ.get('BASE_DIR'))
+else:
+    BASE_DIR = Path(__file__).parent.parent.parent.parent.parent.parent.resolve()
 BASE_CONFIG_DIR = Path.joinpath(BASE_DIR, 'config')
 NETSUITE_CONFIG_DIR = Path.joinpath(BASE_CONFIG_DIR, 'netsuite')
 NETSUITE_TOKENS_DIR = Path.joinpath(BASE_CONFIG_DIR, 'tokens')
 PACKAGE_DIR = Path(__file__).parent.resolve()
 NETSUITE_CLIENT_DIR = Path.joinpath(BASE_DIR, 'netsuite_rest_client')
 
 if not os.path.exists(NETSUITE_CONFIG_DIR):
```

### Comparing `netsuite_python-1.5.9/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.6.0/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite/storages/JSONStorage.py` & `netsuite_python-1.6.0/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.6.0/netsuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.5.9
+Version: 1.6.0
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.5.9/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.6.0/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.9/setup.py` & `netsuite_python-1.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.5.9',
+    version='1.6.0',
     description='Python SDK for Netsuite API with Flask Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

