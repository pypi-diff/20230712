# Comparing `tmp/geoinsight-0.5.4.tar.gz` & `tmp/geoinsight-0.5.6.tar.gz`

## Comparing `geoinsight-0.5.4.tar` & `geoinsight-0.5.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geoinsight-0.5.4/geoinsight/src/__init__.py
--rw-r--r--   0        0        0    75207 2020-02-02 00:00:00.000000 geoinsight-0.5.4/geoinsight/src/api.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.5.4/geoinsight/src/geoinsight.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.5.4/geoinsight/src/util.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 geoinsight-0.5.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.5.4/LICENSE
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 geoinsight-0.5.4/README.md
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 geoinsight-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 geoinsight-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geoinsight-0.5.6/geoinsight/src/__init__.py
+-rw-r--r--   0        0        0    75540 2020-02-02 00:00:00.000000 geoinsight-0.5.6/geoinsight/src/api.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.5.6/geoinsight/src/geoinsight.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.5.6/geoinsight/src/util.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 geoinsight-0.5.6/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.5.6/LICENSE
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 geoinsight-0.5.6/README.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 geoinsight-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 geoinsight-0.5.6/PKG-INFO
```

### Comparing `geoinsight-0.5.4/geoinsight/src/api.py` & `geoinsight-0.5.6/geoinsight/src/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,48 @@
+import os
 import requests
 import logging
 from auth0.authentication.token_verifier import TokenVerifier, AsymmetricSignatureVerifier
 
-AUTH0_DOMAIN = 'dev-pcpa2zpghqzahboo.eu.auth0.com'
-AUTH0_CLIENT_ID = 'KiQTUkMsTKEyCZfie0EPvQSDh4YDMndJ'
-
 class api(object):
     def __init__(self):
-        self.url = ""
+        self.AUTH0_DOMAIN = 'geoinsight.eu.auth0.com'
+        if os.environ['AUTH0_DOMAIN'] is not None:
+            self.AUTH0_DOMAIN = os.environ['AUTH0_DOMAIN']
+
+        self.AUTH0_CLIENT_ID = 'LVipjRM8ywtUFW0yGy5rQXj8Dgs8Uz8o'
+        if os.environ['AUTH0_CLIENT_ID'] is not None:
+            self.AUTH0_CLIENT_ID = os.environ['AUTH0_CLIENT_ID']
+
+        self.url = 'https://api.geoinsight.ai'
+        if os.environ['API_URL'] is not None:
+            self.url = os.environ['API_URL']
+
         self.headers = requests.structures.CaseInsensitiveDict()
         self.headers["Accept"] = "application/json"
         self.headers["Content-Type"] = "application/json"
         self.headers["Accept-Encoding"] = "gzip, deflate, br"
         self.headers["Connection"] = "keep-alive"
         self.headers["Authorization"] = ""
 
     def is_online(self):
         r = requests.get(self.url)
         if 200 <= r.status_code <= 299:
             return True
         else:
             return False
 
-    def set_access_token(self, _gpt, _apk, _apiurl="https://api.geoinsight.ai",):
-        body = {"grant_type": "refresh_token", "client_id": AUTH0_CLIENT_ID, "refresh_token": _gpt, "client_secret": _apk}
-        r = requests.post('https://{}/oauth/token'.format(AUTH0_DOMAIN), data=body)
-        self.url = _apiurl
+    def set_access_token(self, _gpt, _apk):
+        body = {"grant_type": "refresh_token", "client_id": self.AUTH0_CLIENT_ID, "refresh_token": _gpt, "client_secret": _apk}
+        r = requests.post('https://{}/oauth/token'.format(self.AUTH0_DOMAIN), data=body)
         if 200 <= r.status_code <= 299 and self.is_online():
-            jwks_url = 'https://{}/.well-known/jwks.json'.format(AUTH0_DOMAIN)
-            issuer = 'https://{}/'.format(AUTH0_DOMAIN)
+            jwks_url = 'https://{}/.well-known/jwks.json'.format(self.AUTH0_DOMAIN)
+            issuer = 'https://{}/'.format(self.AUTH0_DOMAIN)
             sv = AsymmetricSignatureVerifier(jwks_url)
-            tv = TokenVerifier(signature_verifier=sv, issuer=issuer, audience=AUTH0_CLIENT_ID)
+            tv = TokenVerifier(signature_verifier=sv, issuer=issuer, audience=self.AUTH0_CLIENT_ID)
             tv.verify(r.json()['id_token'])
             self.headers["Authorization"] = "Bearer " + '{token}'.format(token=r.json()['access_token'])
             logging.info('Access Token has been set')
         else:
             logging.error('An error occurred: {e}'.format(e=r.json()))
         return
```

### Comparing `geoinsight-0.5.4/geoinsight/src/geoinsight.py` & `geoinsight-0.5.6/geoinsight/src/geoinsight.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.4/geoinsight/src/util.py` & `geoinsight-0.5.6/geoinsight/src/util.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.4/.gitignore` & `geoinsight-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.4/README.md` & `geoinsight-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.4/PKG-INFO` & `geoinsight-0.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: geoinsight
-Version: 0.5.4
-Summary: GeoInsight python package
+Version: 0.5.6
+Summary: GeoInsight Python Package
 Author-email: GeoInsight <info@geoinsight.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

