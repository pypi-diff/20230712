# Comparing `tmp/nginx-ldap-auth-service-2.0.2.tar.gz` & `tmp/nginx-ldap-auth-service-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-ldap-auth-service-2.0.2.tar", last modified: Tue Jul 11 23:19:43 2023, max compression
+gzip compressed data, was "nginx-ldap-auth-service-2.0.3.tar", last modified: Wed Jul 12 00:22:45 2023, max compression
```

## Comparing `nginx-ldap-auth-service-2.0.2.tar` & `nginx-ldap-auth-service-2.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.640298 nginx-ldap-auth-service-2.0.2/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1453 2023-05-26 19:55:10.000000 nginx-ldap-auth-service-2.0.2/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       54 2023-05-25 16:57:03.000000 nginx-ldap-auth-service-2.0.2/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     1674 2023-07-11 23:19:39.000000 nginx-ldap-auth-service-2.0.2/Makefile
--rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-11 23:19:43.640587 nginx-ldap-auth-service-2.0.2/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      568 2023-07-11 23:13:44.000000 nginx-ldap-auth-service-2.0.2/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.620288 nginx-ldap-auth-service-2.0.2/etc/
--rw-r--r--   0 cmalek     (501) admin       (80)      687 2023-07-10 16:45:02.000000 nginx-ldap-auth-service-2.0.2/etc/environment.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.621422 nginx-ldap-auth-service-2.0.2/etc/nginx/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.623150 nginx-ldap-auth-service-2.0.2/etc/nginx/certs/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1127 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.2/etc/nginx/certs/localhost.crt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1708 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.2/etc/nginx/certs/localhost.key
--rw-rw-r--   0 cmalek     (501) admin       (80)     4599 2023-07-11 20:39:31.000000 nginx-ldap-auth-service-2.0.2/etc/nginx/nginx.conf
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.628268 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/
--rw-rw-r--   0 cmalek     (501) admin       (80)      217 2023-07-11 23:19:39.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.632634 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2023-05-25 15:43:10.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2938 2023-07-10 22:42:15.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6600 2023-07-10 22:41:57.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/main.py
--rw-r--r--   0 cmalek     (501) admin       (80)     4706 2023-07-07 23:31:10.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/middleware.py
--rw-r--r--   0 cmalek     (501) admin       (80)     9652 2023-07-10 17:29:35.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/models.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.635592 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/
--rw-rw-r--   0 cmalek     (501) admin       (80)       74 2023-05-25 15:49:09.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      419 2023-07-10 16:58:38.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/cli.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2198 2023-07-10 23:42:20.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/server.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     3378 2023-07-08 00:06:11.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/ldap.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5010 2023-07-10 23:25:53.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/logging.py
--rw-r--r--   0 cmalek     (501) admin       (80)      179 2023-07-10 17:22:33.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/main.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4522 2023-07-11 20:24:02.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      147 2023-05-25 18:28:56.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/types.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-11 23:19:43.639792 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      865 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       62 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      270 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       16 2023-07-11 23:19:43.000000 nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      628 2023-05-26 19:08:43.000000 nginx-ldap-auth-service-2.0.2/requirements.dev.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      518 2023-07-11 23:19:43.643367 nginx-ldap-auth-service-2.0.2/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1927 2023-07-11 23:19:39.000000 nginx-ldap-auth-service-2.0.2/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.348319 nginx-ldap-auth-service-2.0.3/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1453 2023-05-26 19:55:10.000000 nginx-ldap-auth-service-2.0.3/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       54 2023-05-25 16:57:03.000000 nginx-ldap-auth-service-2.0.3/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1645 2023-07-12 00:22:38.000000 nginx-ldap-auth-service-2.0.3/Makefile
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-12 00:22:45.349052 nginx-ldap-auth-service-2.0.3/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      568 2023-07-11 23:13:44.000000 nginx-ldap-auth-service-2.0.3/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.307444 nginx-ldap-auth-service-2.0.3/etc/
+-rw-r--r--   0 cmalek     (501) admin       (80)      687 2023-07-12 00:20:30.000000 nginx-ldap-auth-service-2.0.3/etc/environment.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.308999 nginx-ldap-auth-service-2.0.3/etc/nginx/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.312670 nginx-ldap-auth-service-2.0.3/etc/nginx/certs/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1127 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.3/etc/nginx/certs/localhost.crt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1708 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.3/etc/nginx/certs/localhost.key
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4599 2023-07-11 20:39:31.000000 nginx-ldap-auth-service-2.0.3/etc/nginx/nginx.conf
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.325183 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      217 2023-07-12 00:22:38.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.332287 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/
+-rw-rw-r--   0 cmalek     (501) admin       (80)        0 2023-05-25 15:43:10.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3635 2023-07-12 00:14:38.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     7143 2023-07-12 00:14:51.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/main.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     4706 2023-07-07 23:31:10.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/middleware.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     9652 2023-07-12 00:21:31.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/models.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.338088 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       74 2023-05-25 15:49:09.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      419 2023-07-10 16:58:38.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/cli.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2198 2023-07-12 00:06:35.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/server.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3378 2023-07-08 00:06:11.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/ldap.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5010 2023-07-10 23:25:53.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/logging.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      179 2023-07-10 17:22:33.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/main.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4522 2023-07-11 20:24:02.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      147 2023-05-25 18:28:56.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/types.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.346622 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      865 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       62 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/entry_points.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      270 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       16 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      628 2023-05-26 19:08:43.000000 nginx-ldap-auth-service-2.0.3/requirements.dev.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      518 2023-07-12 00:22:45.355388 nginx-ldap-auth-service-2.0.3/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1927 2023-07-12 00:22:38.000000 nginx-ldap-auth-service-2.0.3/setup.py
```

### Comparing `nginx-ldap-auth-service-2.0.2/LICENSE.txt` & `nginx-ldap-auth-service-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/Makefile` & `nginx-ldap-auth-service-2.0.3/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-VERSION = 2.0.2
+VERSION = 2.0.3
 
 PACKAGE = nginx-ldap-auth-service
 
-DOCKER_REGISTRY = 131067624433.dkr.ecr.us-west-2.amazonaws.com/caltech-imss-ads
+DOCKER_REGISTRY = caltechads
 #======================================================================
 
 
 clean:
 	rm -rf *.tar.gz dist *.egg-info *.rpm
 	find . -name "*.pyc" -exec rm '{}' ';'
 
@@ -39,24 +39,24 @@
 dev-detached:
 	docker-compose up -d
 
 devdown:
 	docker-compose down
 
 restart:
-	docker-compose restart nginx_ldap_auth
+	docker-compose restart nginx-ldap-auth-service
 
 exec:
-	docker exec -it nginx_ldap_auth /bin/bash
+	docker exec -it nginx-ldap-auth-service /bin/sh
 
 release: dist
 	@twine upload dist/*
 
 log:
-	docker-compose logs -f nginx_ldap_auth
+	docker-compose logs -f nginx-ldap-auth-service
 
 logall:
 	docker-compose logs -f
 
 docker-clean:
 	docker stop $(shell docker ps -a -q)
 	docker rm $(shell docker ps -a -q)
```

### Comparing `nginx-ldap-auth-service-2.0.2/PKG-INFO` & `nginx-ldap-auth-service-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-ldap-auth-service
-Version: 2.0.2
+Version: 2.0.3
 Summary: A FastAPI app that authenticates users via LDAP and sets a cookie for nginx
 Home-page: https://github.com/caltechads/nginx-ldap-auth-service
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: nginx,ldap,auth,fastapi,devops
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nginx-ldap-auth-service-2.0.2/README.md` & `nginx-ldap-auth-service-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/etc/environment.txt` & `nginx-ldap-auth-service-2.0.3/etc/environment.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # REDIS_URL=redis://localhost
 # REDIS_PREFIX=nginx_ldap_auth.
 # LDAP_STARTTLS=True
 # LDAP_DISABLE_REFERRALS=False
 # LDAP_USERNAME_ATTRIBUTE=uid
 # LDAP_FULL_NAME_ATTRIBUTE=cn
 # LDAP_GET_USER_FILTER={username_attribute}={username}
-# LDAP_AUTHOIRZATION_FILTER=None
+# LDAP_AUTHORIZATION_FILTER=None
 # LDAP_TIMEOUT=15
 # LDAP_MIN_POOL_SIZE=1
 # LDAP_MAX_POOL_SIZE=30
 # LDAP_POOL_LIFETIME_SECONDS=20
 # STATSD_HOST=None
 # STATSD_PORT=8125
 # STATSD_PREFIX=nginx_ldap_auth.dev
```

### Comparing `nginx-ldap-auth-service-2.0.2/etc/nginx/certs/localhost.crt` & `nginx-ldap-auth-service-2.0.3/etc/nginx/certs/localhost.crt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/etc/nginx/certs/localhost.key` & `nginx-ldap-auth-service-2.0.3/etc/nginx/certs/localhost.key`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/etc/nginx/nginx.conf` & `nginx-ldap-auth-service-2.0.3/etc/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/main.py` & `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,16 +106,14 @@
         request: The request object
     """
     for key in list(request.session.keys()):
         del request.session[key]
     await get_session_handler(request).destroy()
 
 
-
-
 # --------------------------------------
 # Views
 # --------------------------------------
 
 @app.get("/auth/login", response_class=HTMLResponse, name="login")
 async def login(request: Request, service: str = "/"):
     """
@@ -204,22 +202,32 @@
     """
     Ensure the user is still authorized.  If the user is authorized, return
     200 OK, otherwise return 401 Unauthorized.
 
     The user is authorized if the cookie exists, the session the cookie refers
     to exists, and the ``username`` key in the settings is set.
 
+    Additionally, the user must still exist in LDAP, and if
+    :py:attr:`nginx_ldap_auth.settings.Settings.ldap_authorization_filter` is
+    not ``None``, the user must also match the filter.
+
     Args:
         request: The request object
         response: The response object
     """
     if request.cookies.get(settings.cookie_name):
         await load_session(request)
         if request.session.get("username"):
             # We have a valid session
+            if not await User.objects.get(request.session["username"]):
+                # The user does not exist in LDAP; log them out
+                await kill_session(request)
+            if not await User.objects.is_authorized(request.session["username"]):
+                # The user is not authorized
+                await kill_session(request)
             return {}
         else:
             # Destroy the session because it is not valid
             await kill_session(request)
     # Force the user to authenticate
     response.headers["Cache-Control"] = "no-cache"
     response.status_code = status.HTTP_401_UNAUTHORIZED
```

### Comparing `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/middleware.py` & `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/middleware.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/app/models.py` & `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/models.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/cli/server.py` & `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     '--keyfile', '-k',
     default=lambda: os.environ.get('SSL_KEYFILE', '/certs/server.key'),
     type=click.Path(exists=True, dir_okay=False),
     help="The path to the SSL key file."
 )
 @click.option(
     '--certfile', '-c',
-    default=lambda: os.environ.get('SSL_CERTFILE', '/certs/server.key'),
+    default=lambda: os.environ.get('SSL_CERTFILE', '/certs/server.crt'),
     type=click.Path(exists=True, dir_okay=False),
     help="The path to the SSL certificate file."
 )
 @click.option(
     '--workers', '-w',
     default=lambda: os.environ.get('WORKERS', 1),
     type=int,
```

### Comparing `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/ldap.py` & `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/ldap.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/logging.py` & `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/logging.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth/settings.py` & `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/settings.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/PKG-INFO` & `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-ldap-auth-service
-Version: 2.0.2
+Version: 2.0.3
 Summary: A FastAPI app that authenticates users via LDAP and sets a cookie for nginx
 Home-page: https://github.com/caltechads/nginx-ldap-auth-service
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: nginx,ldap,auth,fastapi,devops
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nginx-ldap-auth-service-2.0.2/nginx_ldap_auth_service.egg-info/SOURCES.txt` & `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/requirements.dev.txt` & `nginx-ldap-auth-service-2.0.3/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/setup.cfg` & `nginx-ldap-auth-service-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.2/setup.py` & `nginx-ldap-auth-service-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setup(
     name="nginx-ldap-auth-service",
-    version="2.0.2",
+    version="2.0.3",
     description="A FastAPI app that authenticates users via LDAP and sets a cookie for nginx",
     author="Caltech IMSS ADS",
     author_email="imss-ads-staff@caltech.edu",
     url="https://github.com/caltechads/nginx-ldap-auth-service",
     packages=find_packages(exclude=["bin"]),
     install_requires=[
         "aiodogstatsd==0.16.0.post0",
```

