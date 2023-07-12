# Comparing `tmp/idds-common-1.2.9.tar.gz` & `tmp/idds-common-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-common-1.2.9.tar", last modified: Sat Apr 29 19:24:55 2023, max compression
+gzip compressed data, was "idds-common-1.3.0.tar", last modified: Wed Jul 12 16:01:35 2023, max compression
```

## Comparing `idds-common-1.2.9.tar` & `idds-common-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:55.947491 idds-common-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 19:24:44.000000 idds-common-1.2.9/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-29 19:24:55.947491 idds-common-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-29 19:24:44.000000 idds-common-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:55.943490 idds-common-1.2.9/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:55.947491 idds-common-1.2.9/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:55.947491 idds-common-1.2.9/lib/idds/common/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/dict_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:55.947491 idds-common-1.2.9/lib/idds/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/plugin/plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-04-29 19:24:44.000000 idds-common-1.2.9/lib/idds/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 19:24:53.000000 idds-common-1.2.9/lib/idds/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:55.947491 idds-common-1.2.9/lib/idds_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-29 19:24:55.000000 idds-common-1.2.9/lib/idds_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-29 19:24:55.000000 idds-common-1.2.9/lib/idds_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:24:55.000000 idds-common-1.2.9/lib/idds_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 19:24:55.000000 idds-common-1.2.9/lib/idds_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 19:24:55.000000 idds-common-1.2.9/lib/idds_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 19:24:55.947491 idds-common-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-29 19:24:44.000000 idds-common-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:55.947491 idds-common-1.2.9/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:55.947491 idds-common-1.2.9/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-29 19:24:53.000000 idds-common-1.2.9/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:35.765921 idds-common-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-12 16:01:25.000000 idds-common-1.3.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-12 16:01:35.765921 idds-common-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 16:01:25.000000 idds-common-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:35.761921 idds-common-1.3.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:35.765921 idds-common-1.3.0/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:35.765921 idds-common-1.3.0/lib/idds/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/dict_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:35.765921 idds-common-1.3.0/lib/idds/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/plugin/plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-07-12 16:01:25.000000 idds-common-1.3.0/lib/idds/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 16:01:34.000000 idds-common-1.3.0/lib/idds/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:35.765921 idds-common-1.3.0/lib/idds_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-12 16:01:35.000000 idds-common-1.3.0/lib/idds_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-12 16:01:35.000000 idds-common-1.3.0/lib/idds_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:01:35.000000 idds-common-1.3.0/lib/idds_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-12 16:01:35.000000 idds-common-1.3.0/lib/idds_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 16:01:35.000000 idds-common-1.3.0/lib/idds_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 16:01:35.765921 idds-common-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-12 16:01:25.000000 idds-common-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:35.761921 idds-common-1.3.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:35.765921 idds-common-1.3.0/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-12 16:01:34.000000 idds-common-1.3.0/tools/env/environment.yml
```

### Comparing `idds-common-1.2.9/LICENSE.rst` & `idds-common-1.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/lib/idds/common/authentication.py` & `idds-common-1.3.0/lib/idds/common/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import datetime
 import base64
 import json
 import jwt
 import os
 import re
 import requests
+import time
+
 
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
 try:
@@ -56,23 +58,53 @@
 
     if ssl_verify:
         return ssl_verify
 
     return True
 
 
-class BaseAuthentication(object):
+class Singleton(object):
+    _instance = None
+
+    def __new__(class_, *args, **kwargs):
+        if not isinstance(class_._instance, class_):
+            class_._instance = object.__new__(class_, *args, **kwargs)
+            class_._instance._initialized = False
+        return class_._instance
+
+
+class BaseAuthentication(Singleton):
     def __init__(self, timeout=None):
         self.timeout = timeout
         self.config = self.load_auth_server_config()
         self.max_expires_in = 60
+
+        self.cache = {}
+        self.cache_time = 3600 * 6
+
         if self.config and self.config.has_section('common'):
             if self.config.has_option('common', 'max_expires_in'):
                 self.max_expires_in = self.config.getint('common', 'max_expires_in')
 
+        if self.config and self.config.has_section('common'):
+            if self.config.has_option('common', 'cache_time'):
+                self.cache_time = self.config.getint('common', 'cache_time')
+
+    def get_cache_value(self, key):
+        if key in self.cache and self.cache[key]['time'] + self.cache_time > time.time():
+            return self.cache[key]['value']
+        return None
+
+    def set_cache_value(self, key, value):
+        cache_keys = list(self.cache.keys())
+        for k in cache_keys:
+            if self.cache[k]['time'] + self.cache_time <= time.time():
+                del self.cache[k]
+        self.cache[key] = {'time': time.time(), 'value': value}
+
     def load_auth_server_config(self):
         config = ConfigParser.ConfigParser()
         if os.environ.get('IDDS_AUTH_CONFIG', None):
             configfile = os.environ['IDDS_AUTH_CONFIG']
             if config.read(configfile) == [configfile]:
                 return config
 
@@ -106,14 +138,18 @@
 
 
 class OIDCAuthentication(BaseAuthentication):
     def __init__(self, timeout=None):
         super(OIDCAuthentication, self).__init__(timeout=timeout)
 
     def get_auth_config(self, vo):
+        ret = self.get_cache_value(vo)
+        if ret:
+            return ret
+
         ret = {'vo': vo, 'oidc_config_url': None, 'client_id': None,
                'client_secret': None, 'audience': None, 'no_verify': False}
 
         if self.config and self.config.has_section(vo):
             for name in ['oidc_config_url', 'client_id', 'client_secret', 'vo', 'audience']:
                 if self.config.has_option(vo, name):
                     ret[name] = self.config.get(vo, name)
@@ -131,23 +167,35 @@
 
     def get_endpoint_config(self, auth_config):
         content = self.get_http_content(auth_config['oidc_config_url'], no_verify=auth_config['no_verify'])
         endpoint_config = json.loads(content)
         # ret = {'token_endpoint': , 'device_authorization_endpoint': None}
         return endpoint_config
 
-    def get_oidc_sign_url(self, vo):
-        try:
+    def get_auth_endpoint_config(self, vo):
+        auth_config = self.get_cache_value(vo)
+        endpoint_config_key = vo + "_endpoint_config"
+        endpoint_config = self.get_cache_value(endpoint_config_key)
+
+        if not auth_config or not endpoint_config:
             allow_vos = self.get_allow_vos()
             if vo not in allow_vos:
                 return False, "VO %s is not allowed." % vo
 
             auth_config = self.get_auth_config(vo)
             endpoint_config = self.get_endpoint_config(auth_config)
 
+            self.set_cache_value(vo, auth_config)
+            self.set_cache_value(endpoint_config_key, endpoint_config)
+        return auth_config, endpoint_config
+
+    def get_oidc_sign_url(self, vo):
+        try:
+            auth_config, endpoint_config = self.get_auth_endpoint_config(vo)
+
             data = {'client_id': auth_config['client_id'],
                     'scope': "openid profile email offline_access",
                     'audience': auth_config['audience']}
 
             headers = {'content-type': 'application/x-www-form-urlencoded'}
 
             result = requests.session().post(endpoint_config['device_authorization_endpoint'],
@@ -167,20 +215,15 @@
         except requests.exceptions.ConnectionError as error:
             return False, 'Failed to get oidc sign in URL. ConnectionError: ' + str(error)
         except Exception as error:
             return False, 'Failed to get oidc sign in URL: ' + str(error)
 
     def get_id_token(self, vo, device_code, interval=5, expires_in=60):
         try:
-            allow_vos = self.get_allow_vos()
-            if vo not in allow_vos:
-                return False, "VO %s is not allowed." % vo
-
-            auth_config = self.get_auth_config(vo)
-            endpoint_config = self.get_endpoint_config(auth_config)
+            auth_config, endpoint_config = self.get_auth_endpoint_config(vo)
 
             data = {'client_id': auth_config['client_id'],
                     'client_secret': auth_config['client_secret'],
                     'grant_type': 'urn:ietf:params:oauth:grant-type:device_code',
                     'device_code': device_code}
 
             headers = {'content-type': 'application/x-www-form-urlencoded'}
@@ -209,20 +252,15 @@
             else:
                 return False, None
         except Exception as error:
             return False, 'Failed to get oidc token: ' + str(error)
 
     def refresh_id_token(self, vo, refresh_token):
         try:
-            allow_vos = self.get_allow_vos()
-            if vo not in allow_vos:
-                return False, "VO %s is not allowed." % vo
-
-            auth_config = self.get_auth_config(vo)
-            endpoint_config = self.get_endpoint_config(auth_config)
+            auth_config, endpoint_config = self.get_auth_endpoint_config(vo)
 
             data = {'client_id': auth_config['client_id'],
                     'client_secret': auth_config['client_secret'],
                     'grant_type': 'refresh_token',
                     'refresh_token': refresh_token}
 
             headers = {'content-type': 'application/x-www-form-urlencoded'}
@@ -248,36 +286,35 @@
 
     def get_public_key(self, token, jwks_uri, no_verify=False):
         headers = jwt.get_unverified_header(token)
         if headers is None or 'kid' not in headers:
             raise jwt.exceptions.InvalidTokenError('cannot extract kid from headers')
         kid = headers['kid']
 
-        jwks_content = self.get_http_content(jwks_uri, no_verify=no_verify)
-        jwks = json.loads(jwks_content)
+        jwks = self.get_cache_value(jwks_uri)
+        if not jwks:
+            jwks_content = self.get_http_content(jwks_uri, no_verify=no_verify)
+            jwks = json.loads(jwks_content)
+            self.set_cache_value(jwks_uri, jwks)
+
         jwk = None
         for j in jwks.get('keys', []):
             if j.get('kid') == kid:
                 jwk = j
         if jwk is None:
             raise jwt.exceptions.InvalidTokenError('JWK not found for kid={0}: {1}'.format(kid, str(jwks)))
 
         public_num = RSAPublicNumbers(n=decode_value(jwk['n']), e=decode_value(jwk['e']))
         public_key = public_num.public_key(default_backend())
         pem = public_key.public_bytes(encoding=serialization.Encoding.PEM, format=serialization.PublicFormat.SubjectPublicKeyInfo)
         return pem
 
     def verify_id_token(self, vo, token):
         try:
-            allow_vos = self.get_allow_vos()
-            if vo not in allow_vos:
-                return False, "VO %s is not allowed." % vo, None
-
-            auth_config = self.get_auth_config(vo)
-            endpoint_config = self.get_endpoint_config(auth_config)
+            auth_config, endpoint_config = self.get_auth_endpoint_config(vo)
 
             # check audience
             decoded_token = jwt.decode(token, verify=False, options={"verify_signature": False})
             audience = decoded_token['aud']
             if audience not in [auth_config['audience'], auth_config['client_id']]:
                 # discovery_endpoint = auth_config['oidc_config_url']
                 return False, "The audience %s of the token doesn't match vo configuration(client_id: %s)." % (audience, auth_config['client_id']), None
```

### Comparing `idds-common-1.2.9/lib/idds/common/cache.py` & `idds-common-1.3.0/lib/idds/common/cache.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/lib/idds/common/config.py` & `idds-common-1.3.0/lib/idds/common/config.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/lib/idds/common/constants.py` & `idds-common-1.3.0/lib/idds/common/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,15 @@
     Expiring = 16
     Expired = 17
     ToFinish = 18
     ToForceFinish = 19
     Terminating = 20
     Building = 21
     Built = 22
+    Throttling = 23
 
 
 class RequestLocking(IDDSEnum):
     Idle = 0
     Locking = 1
 
 
@@ -287,14 +288,15 @@
     FinalFailed = 4
     Lost = 5
     Deleted = 6
     Mapped = 7
     FakeAvailable = 8
     Missing = 9
     Cancelled = 10
+    Activated = 11
 
 
 class ContentLocking(IDDSEnum):
     Idle = 0
     Locking = 1
 
 
@@ -425,14 +427,15 @@
 
 
 class MessageStatus(IDDSEnum):
     New = 0
     Fetched = 1
     Delivered = 2
     Failed = 3
+    ConfirmDelivered = 4
 
 
 class MessageLocking(IDDSEnum):
     Idle = 0
     Locking = 1
 
 
@@ -480,14 +483,19 @@
     Transporter = 2
     Carrier = 3
     Conductor = 4
     Rest = 5
     Other = 6
 
 
+class ThrottlerStatus(IDDSEnum):
+    InActive = 0
+    Active = 1
+
+
 class ReturnCode(IDDSEnum):
     Ok = 0
     Failed = 255
     Locked = 1
 
 
 def get_work_status_from_transform_processing_status(status):
```

### Comparing `idds-common-1.2.9/lib/idds/common/dict_class.py` & `idds-common-1.3.0/lib/idds/common/dict_class.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/lib/idds/common/event.py` & `idds-common-1.3.0/lib/idds/common/event.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/lib/idds/common/exceptions.py` & `idds-common-1.3.0/lib/idds/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/lib/idds/common/plugin/plugin_base.py` & `idds-common-1.3.0/lib/idds/common/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/lib/idds/common/plugin/plugin_utils.py` & `idds-common-1.3.0/lib/idds/common/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/lib/idds/common/status_utils.py` & `idds-common-1.3.0/lib/idds/common/status_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/lib/idds/common/utils.py` & `idds-common-1.3.0/lib/idds/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import json
 import os
 import re
 import requests
 import subprocess
 import sys
 import tarfile
+import time
 # import traceback
 
 from enum import Enum
 from functools import wraps
 from packaging import version as packaging_version
 
 from idds.common.config import (config_has_section, config_has_option,
@@ -63,14 +64,15 @@
                                 format='%(asctime)s\t%(threadName)s\t%(name)s\t%(levelname)s\t%(message)s')
         else:
             logging.basicConfig(stream=sys.stdout, level=loglevel,
                                 format='%(asctime)s\t%(threadName)s\t%(name)s\t%(levelname)s\t%(message)s')
     else:
         logging.basicConfig(stream=stream, level=loglevel,
                             format='%(asctime)s\t%(threadName)s\t%(name)s\t%(levelname)s\t%(message)s')
+    logging.Formatter.converter = time.gmtime
 
 
 def get_logger(name, filename=None, loglevel=None):
     """
     Setup logging
     """
     if loglevel is None:
@@ -534,15 +536,15 @@
     for key in keys:
         if key in dict2:
             if key not in dict1 or dict1[key] is None:
                 dict1[key] = dict2[key]
             else:
                 if dict2[key] is None:
                     continue
-                elif isinstance(dict1[key], type(dict2[key])):
+                elif not isinstance(dict1[key], type(dict2[key])):
                     raise Exception("type of %s is different from %s, cannot merge" % (type(dict1[key]), type(dict2[key])))
                 elif dict1[key] == dict2[key]:
                     continue
                 elif type(dict1[key]) in (list, tuple, str):
                     dict1[key] = dict1[key] + dict2[key]
                 elif type(dict1[key]) in (int, float, complex):
                     dict1[key] = dict1[key] + dict2[key]
```

### Comparing `idds-common-1.2.9/lib/idds_common.egg-info/SOURCES.txt` & `idds-common-1.3.0/lib/idds_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.9/setup.py` & `idds-common-1.3.0/setup.py`

 * *Files identical despite different names*

