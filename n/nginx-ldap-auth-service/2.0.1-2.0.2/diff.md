# Comparing `tmp/nginx-ldap-auth-service-2.0.1.tar.gz` & `tmp/nginx-ldap-auth-service-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-ldap-auth-service-2.0.1.tar", last modified: Tue Jul 11 23:15:15 2023, max compression
+gzip compressed data, was "nginx-ldap-auth-service-2.0.2.tar", last modified: Tue Jul 11 23:19:43 2023, max compression
```

## Comparing `nginx-ldap-auth-service-2.0.1.tar` & `nginx-ldap-auth-service-2.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:15:15.188347 nginx-ldap-auth-service-2.0.1/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1453 2023-05-26 19:55:10.000000 nginx-ldap-auth-service-2.0.1/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       54 2023-05-25 16:57:03.000000 nginx-ldap-auth-service-2.0.1/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     1674 2023-07-11 23:15:11.000000 nginx-ldap-auth-service-2.0.1/Makefile
--rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-11 23:15:15.188571 nginx-ldap-auth-service-2.0.1/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      568 2023-07-11 23:13:44.000000 nginx-ldap-auth-service-2.0.1/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:15:15.168818 nginx-ldap-auth-service-2.0.1/etc/
--rw-r--r--   0 cmalek     (501) admin       (80)      687 2023-07-10 16:45:02.000000 nginx-ldap-auth-service-2.0.1/etc/environment.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:15:15.169900 nginx-ldap-auth-service-2.0.1/etc/nginx/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:15:15.171523 nginx-ldap-auth-service-2.0.1/etc/nginx/certs/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1127 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.1/etc/nginx/certs/localhost.crt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1708 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.1/etc/nginx/certs/localhost.key
--rw-rw-r--   0 cmalek     (501) admin       (80)     4599 2023-07-11 20:39:31.000000 nginx-ldap-auth-service-2.0.1/etc/nginx/nginx.conf
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:15:15.176224 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/
--rw-rw-r--   0 cmalek     (501) admin       (80)      217 2023-07-11 23:15:11.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:15:15.180796 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2023-05-25 15:43:10.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2938 2023-07-10 22:42:15.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6600 2023-07-10 22:41:57.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/main.py
--rw-r--r--   0 cmalek     (501) admin       (80)     4706 2023-07-07 23:31:10.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/middleware.py
--rw-r--r--   0 cmalek     (501) admin       (80)     9652 2023-07-10 17:29:35.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/models.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:15:15.183949 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/cli/
--rw-rw-r--   0 cmalek     (501) admin       (80)       74 2023-05-25 15:49:09.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/cli/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      419 2023-07-10 16:58:38.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/cli/cli.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2198 2023-07-10 23:42:20.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/cli/server.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     3378 2023-07-08 00:06:11.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/ldap.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5010 2023-07-10 23:25:53.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/logging.py
--rw-r--r--   0 cmalek     (501) admin       (80)      179 2023-07-10 17:22:33.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/main.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4522 2023-07-11 20:24:02.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      147 2023-05-25 18:28:56.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/types.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:15:15.187854 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth_service.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-11 23:15:15.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth_service.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      865 2023-07-11 23:15:15.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth_service.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-11 23:15:15.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth_service.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       62 2023-07-11 23:15:15.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth_service.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      287 2023-07-11 23:15:15.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth_service.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       16 2023-07-11 23:15:15.000000 nginx-ldap-auth-service-2.0.1/nginx_ldap_auth_service.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      628 2023-05-26 19:08:43.000000 nginx-ldap-auth-service-2.0.1/requirements.dev.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      518 2023-07-11 23:15:15.189480 nginx-ldap-auth-service-2.0.1/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1955 2023-07-11 23:15:11.000000 nginx-ldap-auth-service-2.0.1/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.640298 nginx-ldap-auth-service-2.0.2/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1453 2023-05-26 19:55:10.000000 nginx-ldap-auth-service-2.0.2/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       54 2023-05-25 16:57:03.000000 nginx-ldap-auth-service-2.0.2/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1674 2023-07-11 23:19:39.000000 nginx-ldap-auth-service-2.0.2/Makefile
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-11 23:19:43.640587 nginx-ldap-auth-service-2.0.2/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      568 2023-07-11 23:13:44.000000 nginx-ldap-auth-service-2.0.2/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.620288 nginx-ldap-auth-service-2.0.2/etc/
+-rw-r--r--   0 cmalek     (501) admin       (80)      687 2023-07-10 16:45:02.000000 nginx-ldap-auth-service-2.0.2/etc/environment.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.621422 nginx-ldap-auth-service-2.0.2/etc/nginx/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.623150 nginx-ldap-auth-service-2.0.2/etc/nginx/certs/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1127 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.2/etc/nginx/certs/localhost.crt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1708 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.2/etc/nginx/certs/localhost.key
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4599 2023-07-11 20:39:31.000000 nginx-ldap-auth-service-2.0.2/etc/nginx/nginx.conf
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.628268 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      217 2023-07-11 23:19:39.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.632634 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/
+-rw-rw-r--   0 cmalek     (501) admin       (80)        0 2023-05-25 15:43:10.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2938 2023-07-10 22:42:15.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     6600 2023-07-10 22:41:57.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/main.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     4706 2023-07-07 23:31:10.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/middleware.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     9652 2023-07-10 17:29:35.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/models.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.635592 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       74 2023-05-25 15:49:09.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      419 2023-07-10 16:58:38.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/cli.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2198 2023-07-10 23:42:20.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/server.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3378 2023-07-08 00:06:11.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/ldap.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5010 2023-07-10 23:25:53.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/logging.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      179 2023-07-10 17:22:33.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/main.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4522 2023-07-11 20:24:02.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      147 2023-05-25 18:28:56.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/types.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.639792 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      865 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       62 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/entry_points.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      270 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       16 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      628 2023-05-26 19:08:43.000000 nginx-ldap-auth-service-2.0.2/requirements.dev.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      518 2023-07-11 23:19:43.643367 nginx-ldap-auth-service-2.0.2/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1927 2023-07-11 23:19:39.000000 nginx-ldap-auth-service-2.0.2/setup.py
```

### Comparing `nginx-ldap-auth-service-2.0.1/LICENSE.txt` & `nginx-ldap-auth-service-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/Makefile` & `nginx-ldap-auth-service-2.0.2/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = 2.0.1
+VERSION = 2.0.2
 
 PACKAGE = nginx-ldap-auth-service
 
 DOCKER_REGISTRY = 131067624433.dkr.ecr.us-west-2.amazonaws.com/caltech-imss-ads
 #======================================================================
```

### Comparing `nginx-ldap-auth-service-2.0.1/PKG-INFO` & `nginx-ldap-auth-service-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-ldap-auth-service
-Version: 2.0.1
+Version: 2.0.2
 Summary: A FastAPI app that authenticates users via LDAP and sets a cookie for nginx
 Home-page: https://github.com/caltechads/nginx-ldap-auth-service
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: nginx,ldap,auth,fastapi,devops
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nginx-ldap-auth-service-2.0.1/README.md` & `nginx-ldap-auth-service-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/etc/environment.txt` & `nginx-ldap-auth-service-2.0.2/etc/environment.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/etc/nginx/certs/localhost.crt` & `nginx-ldap-auth-service-2.0.2/etc/nginx/certs/localhost.crt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/etc/nginx/certs/localhost.key` & `nginx-ldap-auth-service-2.0.2/etc/nginx/certs/localhost.key`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/etc/nginx/nginx.conf` & `nginx-ldap-auth-service-2.0.2/etc/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/forms.py` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/forms.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/main.py` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/main.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/middleware.py` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/middleware.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/app/models.py` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/models.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/cli/server.py` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/server.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/ldap.py` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/ldap.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/logging.py` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/logging.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth/settings.py` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/settings.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth_service.egg-info/PKG-INFO` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-ldap-auth-service
-Version: 2.0.1
+Version: 2.0.2
 Summary: A FastAPI app that authenticates users via LDAP and sets a cookie for nginx
 Home-page: https://github.com/caltechads/nginx-ldap-auth-service
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: nginx,ldap,auth,fastapi,devops
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nginx-ldap-auth-service-2.0.1/nginx_ldap_auth_service.egg-info/SOURCES.txt` & `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/requirements.dev.txt` & `nginx-ldap-auth-service-2.0.2/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/setup.cfg` & `nginx-ldap-auth-service-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.1/setup.py` & `nginx-ldap-auth-service-2.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setup(
     name="nginx-ldap-auth-service",
-    version="2.0.1",
+    version="2.0.2",
     description="A FastAPI app that authenticates users via LDAP and sets a cookie for nginx",
     author="Caltech IMSS ADS",
     author_email="imss-ads-staff@caltech.edu",
     url="https://github.com/caltechads/nginx-ldap-auth-service",
     packages=find_packages(exclude=["bin"]),
     install_requires=[
         "aiodogstatsd==0.16.0.post0",
         "fastapi>=0.95.0",
         "uvicorn[standard]==0.21.1",
-        "gunicorn==22.0.1",
         "bonsai==1.5.1",
         "pydantic-settings",
         "pydantic>=1.9.0",
         "structlog==23.1.0",
         "tabulate>=0.8.9",
         "click>=8.0",
         "sentry-sdk>=1.1.0",
```

