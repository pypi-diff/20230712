# Comparing `tmp/netsuite_python-1.6.0.tar.gz` & `tmp/netsuite_python-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.6.0.tar", last modified: Wed Jul 12 18:57:23 2023, max compression
+gzip compressed data, was "netsuite_python-1.6.1.tar", last modified: Wed Jul 12 19:43:02 2023, max compression
```

## Comparing `netsuite_python-1.6.0.tar` & `netsuite_python-1.6.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.461783 netsuite_python-1.6.0/
--rw-rw-rw-   0        0        0     5438 2023-07-12 18:57:23.460783 netsuite_python-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     5108 2023-04-25 19:14:38.000000 netsuite_python-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.430466 netsuite_python-1.6.0/netsuite/
--rw-rw-rw-   0        0        0    12080 2023-06-26 17:14:03.000000 netsuite_python-1.6.0/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.438783 netsuite_python-1.6.0/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.6.0/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.443783 netsuite_python-1.6.0/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.6.0/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.6.0/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2579 2023-05-19 19:55:49.000000 netsuite_python-1.6.0/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.6.0/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.6.0/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.6.0/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.445783 netsuite_python-1.6.0/netsuite/netsuite_rest_client/
--rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.6.0/netsuite/netsuite_rest_client/__init__.py
--rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.6.0/netsuite/netsuite_rest_client/rest_api_client.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.448783 netsuite_python-1.6.0/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0    12245 2023-06-26 17:12:39.000000 netsuite_python-1.6.0/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6403 2023-07-12 18:56:42.000000 netsuite_python-1.6.0/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.455783 netsuite_python-1.6.0/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.6.0/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:57:23.459782 netsuite_python-1.6.0/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0     5438 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 18:57:23.000000 netsuite_python-1.6.0/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 18:57:23.461783 netsuite_python-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-07-12 18:56:53.000000 netsuite_python-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:02.015762 netsuite_python-1.6.1/
+-rw-rw-rw-   0        0        0     5674 2023-07-12 19:43:02.014763 netsuite_python-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5344 2023-07-12 18:58:16.000000 netsuite_python-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:01.997763 netsuite_python-1.6.1/netsuite/
+-rw-rw-rw-   0        0        0    12080 2023-06-26 17:14:03.000000 netsuite_python-1.6.1/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.6.1/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.6.1/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:02.001765 netsuite_python-1.6.1/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.6.1/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:02.003763 netsuite_python-1.6.1/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.6.1/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.6.1/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2579 2023-05-19 19:55:49.000000 netsuite_python-1.6.1/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.6.1/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.6.1/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.6.1/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.6.1/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.6.1/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:02.004764 netsuite_python-1.6.1/netsuite/netsuite_rest_client/
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.6.1/netsuite/netsuite_rest_client/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.6.1/netsuite/netsuite_rest_client/rest_api_client.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:02.006763 netsuite_python-1.6.1/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.6.1/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12245 2023-06-26 17:12:39.000000 netsuite_python-1.6.1/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6679 2023-07-12 19:42:58.000000 netsuite_python-1.6.1/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:02.009763 netsuite_python-1.6.1/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.6.1/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.6.1/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.6.1/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.6.1/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:43:02.013765 netsuite_python-1.6.1/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0     5674 2023-07-12 19:43:01.000000 netsuite_python-1.6.1/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-07-12 19:43:01.000000 netsuite_python-1.6.1/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:43:01.000000 netsuite_python-1.6.1/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-12 19:43:01.000000 netsuite_python-1.6.1/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2023-07-12 19:43:01.000000 netsuite_python-1.6.1/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 19:43:01.000000 netsuite_python-1.6.1/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:43:02.015762 netsuite_python-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-07-12 19:42:58.000000 netsuite_python-1.6.1/setup.py
```

### Comparing `netsuite_python-1.6.0/PKG-INFO` & `netsuite_python-1.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -26,14 +26,15 @@
 
 # QUICK START #
 
 ## Prerequisite  Setup ##
     1. Enable Services
         * Restlets
         * Rest Web Services
+        * OAUTH 2.0
     2. Create a role for the integration with the following permissions:
         * Access Token Management
         * Log in using Access Tokens	
         * Log in using OAuth 2.0 Access Tokens	
         * OAuth 2.0 Authorized Applications Management	
         * REST Web Services	
         * SuiteApp Deployment	
@@ -41,14 +42,17 @@
         * User Access Tokens	
     3. Create an integration record 
         * Check Client Credentials ( MAchine to Machine Grant)
         * Under Scope Select 
             * Restlets
             * Rest Web Services
         * STORE THE CLIENT ID 
+    4. Create and upload the certificate
+        * with dev environment setup, run ```netsuite generate-certificate```
+        * upload the public cert to Netsuite under Setup -> Integrations -> Manage Oauth 2.0
 
 
 ## Setup The Easy Way  ##
 run ``` netsuite initialize ```
 * Follow the prompts
 
 * Docs will be located in the generated "netsuite_rest_client folder" at the rot of the project
```

### Comparing `netsuite_python-1.6.0/README.md` & `netsuite_python-1.6.1/netsuite_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: netsuite-python
+Version: 1.6.1
+Summary: Python SDK for Netsuite API with Flask Integration
+Home-page: https://bitbucket.org/theapiguys/netsuite_python
+Author: Will @ TheAPIGuys
+Author-email: will@theapiguys.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # README #
 
 
 This library makes it easy to set up a Netsuite authorization without needing a frontend client using CLI utilities.
 
 ### Docs ###
 [Netsuite API Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158022624537.html)
@@ -15,14 +26,15 @@
 
 # QUICK START #
 
 ## Prerequisite  Setup ##
     1. Enable Services
         * Restlets
         * Rest Web Services
+        * OAUTH 2.0
     2. Create a role for the integration with the following permissions:
         * Access Token Management
         * Log in using Access Tokens	
         * Log in using OAuth 2.0 Access Tokens	
         * OAuth 2.0 Authorized Applications Management	
         * REST Web Services	
         * SuiteApp Deployment	
@@ -30,14 +42,17 @@
         * User Access Tokens	
     3. Create an integration record 
         * Check Client Credentials ( MAchine to Machine Grant)
         * Under Scope Select 
             * Restlets
             * Rest Web Services
         * STORE THE CLIENT ID 
+    4. Create and upload the certificate
+        * with dev environment setup, run ```netsuite generate-certificate```
+        * upload the public cert to Netsuite under Setup -> Integrations -> Manage Oauth 2.0
 
 
 ## Setup The Easy Way  ##
 run ``` netsuite initialize ```
 * Follow the prompts
 
 * Docs will be located in the generated "netsuite_rest_client folder" at the rot of the project
@@ -134,7 +149,9 @@
     * Use the defaults or repeat the info used above for
         * Path to Netsuite Credentials
     * Confirm the app name to be refreshed, if single app, just use default
 * That's it! You should now have a valid token to use with the Netsuite API.
 
 
 
+
+
```

### Comparing `netsuite_python-1.6.0/netsuite/Netsuite.py` & `netsuite_python-1.6.1/netsuite/Netsuite.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.6.1/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.6.1/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite/api_clients/api_client.py` & `netsuite_python-1.6.1/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite/api_clients/configuration.py` & `netsuite_python-1.6.1/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite/api_clients/rest.py` & `netsuite_python-1.6.1/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite/module_loading.py` & `netsuite_python-1.6.1/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite/scripts/cli.py` & `netsuite_python-1.6.1/netsuite/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite/settings.py` & `netsuite_python-1.6.1/netsuite/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,16 +32,23 @@
     settings = None
 
 if os.environ.get('BASE_DIR')is not None:
     BASE_DIR = Path(os.environ.get('BASE_DIR'))
 else:
     BASE_DIR = Path(__file__).parent.parent.parent.parent.parent.parent.resolve()
 BASE_CONFIG_DIR = Path.joinpath(BASE_DIR, 'config')
-NETSUITE_CONFIG_DIR = Path.joinpath(BASE_CONFIG_DIR, 'netsuite')
-NETSUITE_TOKENS_DIR = Path.joinpath(BASE_CONFIG_DIR, 'tokens')
+if os.environ.get("NETSUITE_CONFIG_DIR") is not None:
+    NETSUITE_CONFIG_DIR = Path(os.environ.get("NETSUITE_CONFIG_DIR"))
+else:
+    NETSUITE_CONFIG_DIR = Path.joinpath(BASE_CONFIG_DIR, 'netsuite')
+
+if os.environ.get("NETSUITE_TOKENS_DIR") is not None:
+    NETSUITE_TOKENS_DIR = Path(os.environ.get("NETSUITE_TOKENS_DIR"))
+else:
+    NETSUITE_TOKENS_DIR = Path.joinpath(BASE_CONFIG_DIR, 'tokens')
 PACKAGE_DIR = Path(__file__).parent.resolve()
 NETSUITE_CLIENT_DIR = Path.joinpath(BASE_DIR, 'netsuite_rest_client')
 
 if not os.path.exists(NETSUITE_CONFIG_DIR):
     os.makedirs(NETSUITE_CONFIG_DIR)
 if not os.path.exists(NETSUITE_TOKENS_DIR):
     os.makedirs(NETSUITE_TOKENS_DIR)
```

### Comparing `netsuite_python-1.6.0/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.6.1/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite/storages/JSONStorage.py` & `netsuite_python-1.6.1/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: netsuite-python
-Version: 1.6.0
-Summary: Python SDK for Netsuite API with Flask Integration
-Home-page: https://bitbucket.org/theapiguys/netsuite_python
-Author: Will @ TheAPIGuys
-Author-email: will@theapiguys.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # README #
 
 
 This library makes it easy to set up a Netsuite authorization without needing a frontend client using CLI utilities.
 
 ### Docs ###
 [Netsuite API Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158022624537.html)
@@ -26,14 +15,15 @@
 
 # QUICK START #
 
 ## Prerequisite  Setup ##
     1. Enable Services
         * Restlets
         * Rest Web Services
+        * OAUTH 2.0
     2. Create a role for the integration with the following permissions:
         * Access Token Management
         * Log in using Access Tokens	
         * Log in using OAuth 2.0 Access Tokens	
         * OAuth 2.0 Authorized Applications Management	
         * REST Web Services	
         * SuiteApp Deployment	
@@ -41,14 +31,17 @@
         * User Access Tokens	
     3. Create an integration record 
         * Check Client Credentials ( MAchine to Machine Grant)
         * Under Scope Select 
             * Restlets
             * Rest Web Services
         * STORE THE CLIENT ID 
+    4. Create and upload the certificate
+        * with dev environment setup, run ```netsuite generate-certificate```
+        * upload the public cert to Netsuite under Setup -> Integrations -> Manage Oauth 2.0
 
 
 ## Setup The Easy Way  ##
 run ``` netsuite initialize ```
 * Follow the prompts
 
 * Docs will be located in the generated "netsuite_rest_client folder" at the rot of the project
@@ -145,9 +138,7 @@
     * Use the defaults or repeat the info used above for
         * Path to Netsuite Credentials
     * Confirm the app name to be refreshed, if single app, just use default
 * That's it! You should now have a valid token to use with the Netsuite API.
 
 
 
-
-
```

### Comparing `netsuite_python-1.6.0/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.6.1/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.6.0/setup.py` & `netsuite_python-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.6.0',
+    version='1.6.1',
     description='Python SDK for Netsuite API with Flask Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

