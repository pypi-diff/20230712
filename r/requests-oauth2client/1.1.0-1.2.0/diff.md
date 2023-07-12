# Comparing `tmp/requests_oauth2client-1.1.0.tar.gz` & `tmp/requests_oauth2client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_oauth2client-1.1.0.tar", max compression
+gzip compressed data, was "requests_oauth2client-1.2.0.tar", max compression
```

## Comparing `requests_oauth2client-1.1.0.tar` & `requests_oauth2client-1.2.0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0      586 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/LICENSE
--rw-r--r--   0        0        0    33609 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/README.md
--rw-r--r--   0        0        0     2326 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1817 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/__init__.py
--rw-r--r--   0        0        0    20404 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/api_client.py
--rw-r--r--   0        0        0    12715 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/auth.py
--rw-r--r--   0        0        0    21329 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/authorization_request.py
--rw-r--r--   0        0        0     5233 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/backchannel_authentication.py
--rw-r--r--   0        0        0    45451 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/client.py
--rw-r--r--   0        0        0    13768 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/client_authentication.py
--rw-r--r--   0        0        0     4369 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/device_authorization.py
--rw-r--r--   0        0        0     2700 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/discovery.py
--rw-r--r--   0        0        0     5834 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/exceptions.py
--rw-r--r--   0        0        0      180 2022-08-02 11:41:28.988904 requests_oauth2client-1.1.0/requests_oauth2client/flask/__init__.py
--rw-r--r--   0        0        0     2841 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/requests_oauth2client/flask/auth.py
--rw-r--r--   0        0        0     3411 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/requests_oauth2client/pooling.py
--rw-r--r--   0        0        0        0 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/requests_oauth2client/py.typed
--rw-r--r--   0        0        0     8926 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/requests_oauth2client/tokens.py
--rw-r--r--   0        0        0     2412 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/requests_oauth2client/utils.py
--rw-r--r--   0        0        0      272 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/requests_oauth2client/vendor_specific/__init__.py
--rw-r--r--   0        0        0     3313 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/requests_oauth2client/vendor_specific/auth0.py
--rw-r--r--   0        0        0      550 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/.coveragerc
--rw-r--r--   0        0        0        0 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0    19411 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     3476 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/test_authorization_code.py
--rw-r--r--   0        0        0     2069 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/test_client_credentials.py
--rw-r--r--   0        0        0     4881 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/test_device_authorization.py
--rw-r--r--   0        0        0     2048 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/test_refresh_token.py
--rw-r--r--   0        0        0     5774 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/test_token_exchange.py
--rw-r--r--   0        0        0        0 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/__init__.py
--rw-r--r--   0        0        0    14476 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/conftest.py
--rw-r--r--   0        0        0    11738 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_api_client.py
--rw-r--r--   0        0        0     7036 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_auth.py
--rw-r--r--   0        0        0     1592 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_auth0.py
--rw-r--r--   0        0        0     4662 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_authorization_request.py
--rw-r--r--   0        0        0     9758 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_backchannel_authentication.py
--rw-r--r--   0        0        0    45509 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_client.py
--rw-r--r--   0        0        0     5866 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_client_authentication.py
--rw-r--r--   0        0        0     7791 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_device_authorization.py
--rw-r--r--   0        0        0     2029 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_discovery.py
--rw-r--r--   0        0        0     2592 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_flask.py
--rw-r--r--   0        0        0     1516 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_pkce.py
--rw-r--r--   0        0        0    10279 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_tokens.py
--rw-r--r--   0        0        0      857 2022-08-02 11:41:28.992905 requests_oauth2client-1.1.0/tests/unit_tests/test_utils.py
--rw-r--r--   0        0        0    35261 2022-08-02 11:42:30.292103 requests_oauth2client-1.1.0/setup.py
--rw-r--r--   0        0        0    34633 2022-08-02 11:42:30.294360 requests_oauth2client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-07-12 07:28:00.815487 requests_oauth2client-1.2.0/LICENSE
+-rw-r--r--   0        0        0    40327 2023-07-12 07:28:00.815487 requests_oauth2client-1.2.0/README.md
+-rw-r--r--   0        0        0     2565 2023-07-12 07:28:00.815487 requests_oauth2client-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1951 2023-07-12 07:28:00.815487 requests_oauth2client-1.2.0/requests_oauth2client/__init__.py
+-rw-r--r--   0        0        0    20449 2023-07-12 07:28:00.815487 requests_oauth2client-1.2.0/requests_oauth2client/api_client.py
+-rw-r--r--   0        0        0    13247 2023-07-12 07:28:00.815487 requests_oauth2client-1.2.0/requests_oauth2client/auth.py
+-rw-r--r--   0        0        0    28868 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/authorization_request.py
+-rw-r--r--   0        0        0     5244 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/backchannel_authentication.py
+-rw-r--r--   0        0        0    57384 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/client.py
+-rw-r--r--   0        0        0    15046 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/client_authentication.py
+-rw-r--r--   0        0        0     4369 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/device_authorization.py
+-rw-r--r--   0        0        0     2700 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/discovery.py
+-rw-r--r--   0        0        0     8336 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/exceptions.py
+-rw-r--r--   0        0        0      180 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/flask/__init__.py
+-rw-r--r--   0        0        0     2841 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/flask/auth.py
+-rw-r--r--   0        0        0     3411 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/pooling.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/py.typed
+-rw-r--r--   0        0        0    17930 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/tokens.py
+-rw-r--r--   0        0        0     2412 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/utils.py
+-rw-r--r--   0        0        0      301 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/vendor_specific/__init__.py
+-rw-r--r--   0        0        0     3960 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/vendor_specific/auth0.py
+-rw-r--r--   0        0        0     2199 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/requests_oauth2client/vendor_specific/ping.py
+-rw-r--r--   0        0        0      550 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/.coveragerc
+-rw-r--r--   0        0        0        0 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    19661 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     3506 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/test_authorization_code.py
+-rw-r--r--   0        0        0     2068 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/test_client_credentials.py
+-rw-r--r--   0        0        0     4880 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/test_device_authorization.py
+-rw-r--r--   0        0        0     2048 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/test_refresh_token.py
+-rw-r--r--   0        0        0     5774 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/test_token_exchange.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/__init__.py
+-rw-r--r--   0        0        0    16858 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/conftest.py
+-rw-r--r--   0        0        0    11738 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_api_client.py
+-rw-r--r--   0        0        0     7034 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_auth.py
+-rw-r--r--   0        0        0     7745 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_authorization_request.py
+-rw-r--r--   0        0        0     9752 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_backchannel_authentication.py
+-rw-r--r--   0        0        0    51244 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_client.py
+-rw-r--r--   0        0        0     6135 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_client_authentication.py
+-rw-r--r--   0        0        0     7789 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_device_authorization.py
+-rw-r--r--   0        0        0     2029 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_discovery.py
+-rw-r--r--   0        0        0     2592 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_flask.py
+-rw-r--r--   0        0        0    20850 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_oidc.py
+-rw-r--r--   0        0        0     1516 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_pkce.py
+-rw-r--r--   0        0        0    10671 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_tokens.py
+-rw-r--r--   0        0        0      857 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/test_utils.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/vendor_specific/__init__.py
+-rw-r--r--   0        0        0     1727 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/vendor_specific/test_auth0.py
+-rw-r--r--   0        0        0     1827 2023-07-12 07:28:00.819487 requests_oauth2client-1.2.0/tests/unit_tests/vendor_specific/test_ping.py
+-rw-r--r--   0        0        0    41340 1970-01-01 00:00:00.000000 requests_oauth2client-1.2.0/PKG-INFO
```

### Comparing `requests_oauth2client-1.1.0/LICENSE` & `requests_oauth2client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/README.md` & `requests_oauth2client-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,61 @@
-`requests_oauth2client` is a OAuth 2.x client for Python, able to obtain, refresh and revoke tokens from any OAuth2.x/OIDC
-compliant Authorization Server. It sits upon and extends the famous [requests] HTTP client module.
+Metadata-Version: 2.1
+Name: requests-oauth2client
+Version: 1.2.0
+Summary: An OAuth2.x Client based on requests.
+Home-page: https://github.com/guillp/requests_oauth2client
+License: Apache-2.0
+Author: Guillaume Pujol
+Author-email: guill.p.linux@gmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Security
+Provides-Extra: doc
+Provides-Extra: test
+Requires-Dist: binapy (>=0.6.1)
+Requires-Dist: furl (>=2.1.2)
+Requires-Dist: jwskate (>=0.8)
+Requires-Dist: requests (>=2.19.0)
+Description-Content-Type: text/markdown
+
+`requests_oauth2client` is an OAuth 2.x client for Python, able to obtain, refresh and revoke tokens from any
+OAuth2.x/OIDC compliant Authorization Server. It sits upon and extends the famous [requests] HTTP client module.
 
 It can act as an [OAuth 2.0](https://tools.ietf.org/html/rfc6749) /
 [2.1](https://datatracker.ietf.org/doc/draft-ietf-oauth-v2-1) client, to automatically get and renew Access Tokens,
 based on the
-[Client Credentials](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-03.html#name-client-credentials),
-[Authorization Code](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-03.html#name-authorization-code),
-[Refresh token](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-03.html#name-refresh-token),
+[Client Credentials](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-07.html#name-client-credentials),
+[Authorization Code](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-07.html#name-authorization-code),
+[Refresh token](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-07.html#name-refresh-token),
 [Token Exchange](https://www.rfc-editor.org/rfc/rfc8693.html),
-[Device Authorization](https://www.rfc-editor.org/rfc/rfc8628.html), or
-[CIBA](https://openid.net/specs/openid-client-initiated-backchannel-authentication-core-1_0.html) grants.
+[JWT Bearer](https://www.rfc-editor.org/rfc/rfc7523.html#section-2.1),
+[Device Authorization](https://www.rfc-editor.org/rfc/rfc8628.html),
+[Resource Owner Password](https://www.rfc-editor.org/rfc/rfc6749#section-4.3) or
+[CIBA](https://openid.net/specs/openid-client-initiated-backchannel-authentication-core-1_0.html) grants. Additional
+grant types are easy to add if needed.
 
 It also supports [OpenID Connect 1.0](https://openid.net/specs/openid-connect-core-1_0.html),
 [PKCE](https://www.rfc-editor.org/rfc/rfc7636.html),
-[Client Assertions](https://www.rfc-editor.org/rfc/rfc7523.html),
-[Token Revocation](https://www.rfc-editor.org/rfc/rfc7009.html),
-and [Introspection](https://www.rfc-editor.org/rfc/rfc7662.html),
+[Client Assertions](https://www.rfc-editor.org/rfc/rfc7523.html#section-2.2),
+[Token Revocation](https://www.rfc-editor.org/rfc/rfc7009.html), and
+[Introspection](https://www.rfc-editor.org/rfc/rfc7662.html),
 [Resource Indicators](https://www.rfc-editor.org/rfc/rfc8707.html),
 [JWT-secured Authorization Requests](https://datatracker.ietf.org/doc/rfc9101/),
 [Pushed Authorization Requests](https://datatracker.ietf.org/doc/rfc9126/),
-[Authorization Server Issuer Identification](https://www.rfc-editor.org/rfc/rfc9207.html)
-as well as using custom params to any endpoint, and other important features that are often overlooked in other client
-libraries.
+[Authorization Server Issuer Identification](https://www.rfc-editor.org/rfc/rfc9207.html), as well as using custom
+params to any endpoint, and other important features that are often overlooked in other client libraries.
 
 And it also includes a [wrapper][apiclient] around [requests.Session] that makes it super easy to use REST-style APIs,
 with or without OAuth 2.x.
 
 Please note that despite the name, this library has no relationship with Google
 [oauth2client](https://github.com/googleapis/oauth2client) library.
 
@@ -39,98 +69,119 @@
 
 # Documentation
 
 Full module documentation is available at https://guillp.github.io/requests_oauth2client/
 
 # Installation
 
-`requests_oauth2client` is [available from PyPi](https://pypi.org/project/requests-oauth2client/), so installing it is as easy as:
+`requests_oauth2client` is [available from PyPi](https://pypi.org/project/requests-oauth2client/), so installing it is
+as easy as:
 
 ```shell
 pip install requests_oauth2client
 ```
 
 # Usage
 
 Everything from `requests_oauth2client` is available from the root module, so you can import it like this:
 
 ```python
 from requests_oauth2client import *
 ```
 
-Note that this automatically imports `requests`, so no need to import it yourself.
+Or you can import individual objects from this package as usual. Note that importing `*` automatically imports
+`requests`, so no need to import it yourself.
 
 ## Calling APIs with Access Tokens
 
-If you already managed to obtain an access token, you can simply use the [BearerAuth] Auth Handler for [requests]:
+If you already managed to obtain an access token for the API you want to call, you can simply use the [BearerAuth] Auth
+Handler for [requests]:
 
 ```python
 import requests
-from requests_oauth2client import BearerToken
+from requests_oauth2client import BearerAuth
 
 token = "an_access_token"
 resp = requests.get("https://my.protected.api/endpoint", auth=BearerAuth(token))
 ```
 
-This authentication handler will add a properly formatted `Authorization` header in the request, with your access token
-according to [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1).
+This authentication handler will add a properly formatted `Authorization: Bearer <access_token>` header in the request,
+with your access token according to [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1).
 
 ## Using an OAuth2Client
 
 [OAuth2Client] offers several methods that implement the communication to the various endpoints that are standardised by
 OAuth 2.0 and its extensions. Those endpoints include the Token Endpoint, the Revocation, Introspection, UserInfo,
-BackChannel Authentication and Device Authorization Endpoints. You only have to provide those if you intend to use them.
+BackChannel Authentication and Device Authorization Endpoints.
+
+You have to provide the URLs for those endpoints if you intend to use them. Otherwise, only the Token Endpoint is
+mandatory to initialize an `OAuth2Client`.
 
-To initialize an [OAuth2Client], you only need a Token Endpoint URI, and the credentials for your application, which are
-often a `client_id` and a `client_secret`:
+To initialize an [OAuth2Client], you only need a Token Endpoint URI from your AS, and the credentials for your
+application, which are often a `client_id` and a `client_secret`, usually also provided by the AS:
 
 ```python
 from requests_oauth2client import OAuth2Client
 
 oauth2client = OAuth2Client(
-    token_endpoint="https://myas.local/token_endpoint",
-    auth=("client_id", "client_secret"),
+    token_endpoint="https://url.to.the/token_endpoint",
+    client_id="my_client_id",
+    client_secret="my_client_secret",
 )
 ```
 
 The Token Endpoint is the only endpoint that is mandatory to obtain tokens. Credentials are used to authenticate the
 client everytime it sends a request to its Authorization Server. Usually, those are a static Client ID and Secret, which
 are the direct equivalent of a username and a password, but meant for an application instead of for a human user. The
 default authentication method used by `OAuth2Client` is *Client Secret Post*, but other standardised methods such as
 *Client Secret Basic*, *Client Secret JWT* or *Private Key JWT* are supported as well. See
 [more about client authentication methods below](#supported-client-authentication-methods).
 
 ## Obtaining tokens
 
-[OAuth2Client] has methods to send requests to the Token Endpoint using the different standardised (and/or custom)
-grants. Since the token endpoint and authentication method are already declared for the client at init time, the only
-required parameters are those that will be sent in the request to the Token Endpoint.
+[OAuth2Client] has dedicated methods to send requests to the Token Endpoint using the different standardised (and/or
+custom) grants. Since the Token Endpoint URL and Client Authentication Method to use are already declared for the client
+at init time, the only required parameters for those methods are those that will be sent in the request to the Token
+Endpoint.
 
 Those methods directly return a [BearerToken] if the request is successful, or raise an exception if it fails.
-[BearerToken] will manage the token expiration, will contain the eventual refresh token that matches the access token,
-and will keep track of other associated metadata as well. You can create such a [BearerToken] yourself if you need:
+[BearerToken] contains all the data as returned by the Token Endpoint, including the Access Token. It will:
+
+- keep track of the Access Token expiration date (based on the `expires_in` hint as returned by the AS). This date is
+  accessible with the `expires_at` attribute.
+- contain the Refresh Token, if returned by the AS, accessible with the `refresh_token` attribute.
+- contain the ID Token, if returned by the AS, accessible with the `ìd_token` attribute (when using the Authorization
+  Code flow).
+- keep track of other associated metadata as well, also accessible as attributes with the same name:
+  `token.custom_attr`, or with subscription syntax `token["my.custom.attr"]`.
+
+You can create such a [BearerToken] yourself if you need:
 
 ```python
 from requests_oauth2client import BearerToken
 
 bearer_token = BearerToken(access_token="an_access_token", expires_in=60)
 print(bearer_token)
 # {'access_token': 'an_access_token',
 #  'expires_in': 55,
 #  'token_type': 'Bearer'}
 print(bearer_token.expires_at)
 # datetime.datetime(2021, 8, 20, 9, 56, 59, 498793)
 assert not bearer_token.is_expired()
+
+print(bearer_token.expires_in)
+# 40
 ```
 
-Note that the `expires_in` indicator here is not static. It keeps track of the token lifetime and is calculated as the
-time flies. The actual static expiration date is accessible with the `expires_at` property. You can check if a token is
-expired with [bearer_token.is_expired()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.tokens.BearerToken.is_expired).
+Note that the `expires_in` indicator here is not static. It keeps track of the token lifetime, in seconds, and is
+calculated as the time flies. The actual static expiration date is accessible with the `expires_at` property. You can
+check if a token is expired with
+[bearer_token.is_expired()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.tokens.BearerToken.is_expired).
 
-You can use a [BearerToken] instance anywhere you can supply an access_token as string.
+You can use a [BearerToken] instance anywhere you can use an access_token as string.
 
 ### Using OAuth2Client as a requests Auth Handler
 
 While using [OAuth2Client] directly is great for testing or debugging OAuth2.x flows, it is not a viable option for
 actual applications where tokens must be obtained, used during their lifetime then obtained again or refreshed once they
 are expired. `requests_oauth2client` contains several [requests] compatible Auth Handlers (as subclasses of
 [requests.auth.AuthBase](https://requests.readthedocs.io/en/latest/user/advanced/#custom-authentication)), that will
@@ -141,132 +192,170 @@
 ### Client Credentials grant
 
 To send a request using the Client Credentials grant, use the aptly named
 [.client_credentials()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.client_credentials)
 method, with the parameters to send in the token request as keyword parameters:
 
 ```python
+from requests_oauth2client import OAuth2Client
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    auth=("client_id", "client_secret"),
+)
+
+token = oauth2client.client_credentials(scope="myscope")
+# or, if your AS uses resource indicator:
 token = oauth2client.client_credentials(scope="myscope", resource="https://myapi.local")
+# or, if your AS uses 'audience' as parameter to identify the requested API (Auth0 style):
+token = oauth2client.client_credentials(audience="https://myapi.local")
+# or, if your AS uses custom parameters:
+token = oauth2client.client_credentials(scope="myscope", custom_param="custom_value")
 ```
 
-Parameters such as `scope`, `resource` or `audience` that may be required by the AS can be passed as keyword
-parameters. Those will be included in the token request that is sent to the AS.
+Parameters such as `scope`, `resource` or `audience` or any other parameter that may be required by the AS can be passed
+as keyword parameters. Those will be included in the token request that is sent to the AS. `scope` is not mandatory at
+client level (but it might be required by your AS to serve your request).
 
 #### As Auth Handler
 
 You can use the
 [OAuth2ClientCredentialsAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2ClientCredentialsAuth)
 auth handler. It takes an [OAuth2Client] as parameter, and the additional kwargs to pass to the token endpoint:
 
 ```python
 import requests
+from requests_oauth2client import OAuth2Client, OAuth2ClientCredentialsAuth
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    auth=("client_id", "client_secret"),
+)
 
 auth = OAuth2ClientCredentialsAuth(
     oauth2client, scope="myscope", resource="https://myapi.local"
 )
 
 # use it like this:
 requests.get("https://myapi.local/resource", auth=auth)
 
-# or
+# or like this:
 session = requests.Session()
 session.auth = auth
 
 resp = session.get("https://myapi.local/resource")
 ```
 
 Once again, extra parameters such as `scope`, `resource` or `audience` are allowed if required.
 
-When you send your first request, [OAuth2ClientCredentialsAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2ClientCredentialsAuth)
+When you send your first request,
+[OAuth2ClientCredentialsAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2ClientCredentialsAuth)
 will automatically retrieve an access token from the AS using the Client Credentials grant, then will include it in the
 request. Next requests will use the same token, as long as it is valid. A new token will be automatically retrieved once
 the previous one is expired.
 
 ### Authorization Code Grant
 
 Obtaining tokens with the Authorization code grant is made in 3 steps:
 
-1. your application must open specific url called the *Authentication Request* in a browser.
+1. your application must open a specific url called the *Authentication Request* in a browser.
 
 2. your application must obtain and validate the *Authorization Response*, which is a redirection back to your
-   application that contains an *Authorization Code* as parameter.
+   application that contains an *Authorization Code* as parameter. This redirect back (often called "callback") is
+   initiated by the Authorization Server after any necessary interaction with the user is complete (Registration, Login,
+   Profile completion, Multi-Factor Authentication, Authorization, Consent, etc.)
 
 3. your application must then exchange this Authorization Code for an *Access Token*, with a request to the Token
    Endpoint.
 
-[OAuth2Client] doesn't implement anything that is related to the Authorization Request or Response. It is only able to
-exchange the Authorization Code for a Token in step 3. But `requests_oauth2client` has other classes to help you with
-steps 1 and 2, as described below:
+`requests_oauth2client`, and more specifically [OAuth2Client] will help you with all those steps, as described below.
 
 #### Generating Authorization Requests
 
-You can generate valid authorization requests with the
-[AuthorizationRequest](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.authorization_request.AuthorizationRequest)
-class:
+To be able to use the Authorization Code grant, you need two urls:
 
-```python
-auth_request = AuthorizationRequest(
-    authorization_endpoint,
-    client_id,
-    redirect_uri=redirect_uri,
-    scope=scope,
-    resource=resource,  # extra parameters can be included as well if required by your AS
-)
-print(auth_request)  # redirect the user to that URL to get a code
-```
-
-This request will look like this (with line breaks for display purposes only):
+- the URL for Authorization Endpoint, which is the url where you must send your Authorization Requests
+- the Redirect URI, which is the url pointing to your application, where the Authorization Server will reply with
+  Authorization Response
 
-```
-https://myas.local/authorize
-?client_id=my_client_id
-&redirect_uri=http%3A%2F%2Flocalhost%2Fcallback
-&response_type=code
-&state=kHWL4VwcbUbtPR4mtht6yMAGG_S-ZcBh5RxI_IGDmJc
-&nonce=mSGOS1M3LYU9ncTvvutoqUR4n1EtmaC_sQ3db4dyMAc
-&scope=openid+email+profile
-&code_challenge=Dk11ttaDb_Hyq1dObMqQcTIlfYYRVblFMC9lFM3UWW8
-&code_challenge_method=S256
-&resource=https%3A%2F%2Fmy.resource.local%2Fapi
-```
+You can declare those urls when initializing your OAuth2Client instance. Then you can generate valid Authorization
+Requests by calling the method `.authorization_request()`:
 
-[AuthorizationRequest] supports PKCE and uses it by default. You can avoid it by passing `code_challenge_method=None` to
-[AuthorizationRequest]. You can obtain the generated code_verifier from `auth_request.code_verifier`.
+```python
+from requests_oauth2client import OAuth2Client
 
-Redirecting or otherwise sending the user to this url is your application responsibility, as well as obtaining the
-Authorization Response url.
+client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endoint",
+    authorization_endpoint="https://url.to.the/authorization_endpoint",
+    redirect_uri="https://url.to.my.application/redirect_uri",
+    client_id="client_id",
+    client_secret="client_secret",
+)
+
+az_request = client.authorization_request(scope="openid email profile")
+
+print(az_request)
+# this will look like this, with line feeds for display purposes only:
+# https://url.to.the/authorization_endpoint
+# ?client_id=client_id
+# &redirect_uri=https%3A%2F%2Furl.to.my.application%2Fredirect_uri
+# &response_type=code
+# &scope=openid+email+profile
+# &state=FBx9mWeLwoKGgG76vhi6v61-4mgxmgZhtWIa7aTffdY
+# &nonce=iHZJokhkGOAojff1tdknRyz9mPZyy5vq9JDlVaUHyqk
+# &code_challenge=TG7qgdyKnwUPuoQ6NNJRlLMoHbeVmJlB8g0VOcfQEkc
+# &code_challenge_method=S256
+
+# you can send the user to that url with:
+import webbrowser
+
+webbrowser.open(az_request.uri)
+```
+
+Note that the `state`, `nonce` and `code_challenge` parameters are generated with secure random values by default.
+Should you wish to use your own values, you can pass them as parameters to `OAuth2Client.authorization_request()`. For
+PKCE, you need to pass your generated `code_verifier`, and the `code_challenge` will automatically be derived from it.
+If you don't want to use PKCE, you can pass `code_challenge_method=None` when initializing your `OAuth2Client`.
 
 #### Validating the Authorization Response
 
-Once the user is successfully authenticated and authorized, the AS will respond with a redirection to your redirect_uri.
-That is the *Authorization Response*. It contains several parameters that must be retrieved by your client. The
-authorization code is one of those parameters, but you must also validate that the *state* matches your request. You can
-do this with:
+Once you have redirected the user browser to the Authorization Request URI, and after the user is successfully
+authenticated and authorized, plus any other extra interactive step is complete, the AS will respond with a redirection
+to your redirect_uri. That is the *Authorization Response*. It contains several parameters that must be retrieved by
+your client. The *Authorization Code* is one of those parameters, but you must also validate that the *state* matches
+your request. You can do this with:
 
 ```python
+# using the `az_request` as defined above
+
 response_uri = input(
     "Please enter the full url and/or params obtained on the redirect_uri: "
 )
-auth_response = auth_request.validate_callback(response_uri)
+az_response = az_request.validate_callback(response_uri)
 ```
 
+This auth_response is an `AuthorizationResponse` instance and contains everything that is needed for your application to
+complete the authentication and get its tokens from the AS.
+
 #### Exchanging code for tokens
 
+Once you have obtained the AS response, containing an authorization code, your application must exchange it for actual
+Token(s).
+
 To exchange a code for Access and/or ID tokens, use the
 [OAuth2Client.authorization_code()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.authorization_code)
 method. If you have obtained an AuthorizationResponse as described above, you can simply do:
 
 ```python
-token = oauth2client.authorization_code(auth_response)
+token = oauth2client.authorization_code(az_response)
 ```
 
-This will automatically include the `code`, `redirect_uri` and `code_verifier` parameters in the Token Request,
-as expected by the AS.
-
-If you managed another way to obtain an Authorization Code, you can manually pass those parameters like this:
+This will automatically include the `code`, `redirect_uri` and `code_verifier` parameters in the Token Request, as
+expected by the AS. You may include extra parameters if required, or you may pass your own parameters, without using an
+`AuthorizationResponse` instance, like this:
 
 ```python
 token = oauth2client.authorization_code(
     code=code,
     code_verifier=code_verifier,
     redirect_uri=redirect_uri,
     custom_param=custom_value,
@@ -277,152 +366,186 @@
 
 The
 [OAuth2AuthorizationCodeAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2AuthorizationCodeAuth)
 handler takes an [OAuth2Client] and an authorization code as parameter, plus whatever additional keyword parameters are
 required by your Authorization Server:
 
 ```python
+from requests_oauth2client import OAuth2Client, ApiClient, OAuth2AuthorizationCodeAuth
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    authorization_endpoint="https://url.to.the/authorization_endpoint",
+    auth=("client_id", "client_secret"),
+)
+
 api_client = ApiClient(
     "https://your.protected.api/endpoint",
     auth=OAuth2AuthorizationCodeAuth(
-        client,
-        code,
-        code_verifier=auth_request.code_verifier,
-        redirect_uri=redirect_uri,
+        oauth2client,
+        "my_authorization_code",
     ),
 )
 
-resp = api_client.post(
-    data={...}
-)  # first call will exchange the code for an initial access/refresh tokens
+# any request using api_client will trigger exchanging the code for an access_token, which is then cached, and refreshed later if needed
+resp = api_client.post(data={...})
 ```
 
 [OAuth2AuthorizationCodeAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2AuthorizationCodeAuth)
 will take care of refreshing the token automatically once it is expired, using the refresh token, if available.
 
+### Note on AuthorizationRequest
+
+Authorization Requests generated by `OAuth2Client.authorization_request()` are instance of the class
+[`AuthorizationRequest`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.authorization_request.AuthorizationRequest).
+You can also use that class directly to generate your requests, but in that case you need to supply your Authorization
+Endpoint URI, your `client_id`, `redirect_uri`, etc. You can access every parameter from an `AuthorizationRequest`
+instance, as well as the generated `code_verifier`, as attributes of this instance. Once an Authorization Request URL is
+generated, it your application responsibility to redirect or otherwise send the user to that URL. You may use the
+`webbrowser` module from Python standard library to do so. Here is an example for generating Authorization Requests:
+
+```python
+from requests_oauth2client import AuthorizationRequest
+
+az_request = AuthorizationRequest(
+    "https://url.to.the/authorization_endpoint",
+    client_id="my_client_id",
+    redirect_uri="http://localhost/callback",  # this redirect_uri is specific to your app
+    scope="openid email profile",
+    # extra parameters such as `resource` can be included as well if required by your AS
+    resource="https://my.resource.local/api",
+)
+print(
+    az_request
+)  # this request will look like this, with line breaks for display purposes only
+# https://url.to.the/authorization_endpoint
+# ?client_id=my_client_id
+# &redirect_uri=http%3A%2F%2Flocalhost%callback
+# &response_type=code
+# &state=kHWL4VwcbUbtPR4mtht6yMAGG_S-ZcBh5RxI_IGDmJc
+# &nonce=mSGOS1M3LYU9ncTvvutoqUR4n1EtmaC_sQ3db4dyMAc
+# &scope=openid+email+profile
+# &code_challenge=W3n02f6xUKoDVbmhWEWz3h780b-Ci6ucnBS_d7nogmQ
+# &code_challenge_method=S256
+# &resource=https%3A%2F%2Fmy.resource.local%2Fapi
+
+print(az_request.code_verifier)
+# 'gYK-ZnQfoat2bghwed7oEz--wvn4D70ksJ5GuWO9sXXygZ7PMnUlSpBmMCcNRHxdgTS9m_roYwGxF6HQxIqZVwXmxRJUziFHUFxDrNuUIjCJCx6gBhPlpFbUXulB1fo2'
+```
+
 ### Device Authorization Grant
 
-Helpers for the Device Authorization Grant are also included. To get device and user codes:
+Helpers for the Device Authorization Grant are also included. To get device and user codes, read the response attributes
+(including Device Code, User Code, Verification URI, etc.), then pooling the Token Endpoint:
 
 ```python
+from requests_oauth2client import (
+    OAuth2Client,
+    DeviceAuthorizationPoolingJob,
+    BearerToken,
+)
+
 client = OAuth2Client(
-    token_endpoint="https://myas.local/token",
-    device_authorization_endpoint="https://myas.local/device",
-    auth=(client_id, client_secret),
+    token_endpoint="https://url.to.the/token_endpoint",
+    device_authorization_endpoint="https://url.to.the/device_authorization_endpoint",
+    auth=("client_id", "client_secret"),
 )
 
 da_resp = client.authorize_device()
-```
-
-`da_resp` contains the Device Code, User Code, Verification URI and other info returned by the AS:
 
-```python
+# `da_resp` contains the Device Code, User Code, Verification URI and other info returned by the AS:
 da_resp.device_code
 da_resp.user_code
 da_resp.verification_uri
 da_resp.verification_uri_complete
 da_resp.expires_at  # just like for BearerToken, expiration is tracked by requests_oauth2client
 da_resp.interval
-```
-
-Send/show the Verification Uri and User Code to the user. He must use a browser to visit that url, authenticate and
-input the User Code. You can then request the Token endpoint to check if the user successfully authorized you using an
-[OAuth2Client]:
-
-```python
-token = client.device_code(da_resp.device_code)
-```
 
-This will raise an exception, either
-[AuthorizationPending](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.exceptions.AuthorizationPending),
-[SlowDown](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.exceptions.SlowDown),
-[ExpiredToken](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.exceptions.ExpiredToken), or
-[AccessDenied](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.exceptions.AccessDenied) if the
-user did not yet finish authorizing your device, if you should increase your pooling period, or if the device code is no
-longer valid, or the user finally denied your access, respectively. Other exceptions may be raised depending on the
-error code that the AS responds with. If the user did finish authorizing successfully, `token` will contain your access
-token.
+# Send/show the Verification Uri and User Code to the user. He must use a browser to visit that url, authenticate and
+# input the User Code.
 
-To make pooling easier, you can use a
-[DeviceAuthorizationPoolingJob](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.device_authorization.DeviceAuthorizationPoolingJob)
-like this:
-
-```python
-pool_job = DeviceAuthorizationPoolingJob(
-    client, device_auth_resp.device_code, interval=device_auth_resp.interval
-)
+# You can then request the Token endpoint to check if the user successfully authorized your device like this:
+pool_job = DeviceAuthorizationPoolingJob(client, da_resp)
 
 resp = None
 while resp is None:
     resp = pool_job()
 
 assert isinstance(resp, BearerToken)
 ```
 
 [DeviceAuthorizationPoolingJob](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.device_authorization.DeviceAuthorizationPoolingJob)
-will automatically obey the pooling period. Everytime you call pool_job(), it will wait the appropriate number of
+will automatically obey the pooling period. Everytime you call `pool_job()`, it will wait the appropriate number of
 seconds as indicated by the AS, and will apply slow_down requests.
 
 #### As Auth Handler
 
 Use
 [OAuth2DeviceCodeAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2DeviceCodeAuth)
 as auth handler to exchange a device code for an access token:
 
 ```python
+from requests_oauth2client import ApiClient, OAuth2DeviceCodeAuth, OAuth2Client
+
+client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    device_authorization_endpoint="https://url.to.the/device_authorization_endpoint",
+    auth=("client_id", "client_secret"),
+)
+
+device_auth_resp = client.authorize_device()
+
+# expose user_code and verification_uri or verification_uri_complete to the user
+device_auth_resp.user_code
+device_auth_resp.verification_uri
+device_auth_resp.verification_uri_complete
+
+# then try to send your request with a OAuth2DeviceCodeAuth handler
+# this will pool the token endpoint until the user authorize the device
 api_client = ApiClient(
     "https://your.protected.api/endpoint",
-    auth=OAuth2DeviceCodeAuth(
-        client,
-        device_auth_resp.device_code,
-        interval=device_auth_resp.interval,
-        expires_in=device_auth_resp.expires_in,
-    ),
+    auth=OAuth2DeviceCodeAuth(client, device_auth_resp),
 )
 
 resp = api_client.post(
     data={...}
 )  # first call will hang until the user authorizes your app and the token endpoint returns a token.
 ```
 
 ### Client-Initiated BackChannel Authentication (CIBA)
 
-To initiate a BackChannel Authentication against the dedicated endpoint:
+To initiate a BackChannel Authentication against the dedicated endpoint, read the response attributes, and pool the
+Token Endpoint until the end-user successfully authenticates:
 
 ```python
+from requests_oauth2client import (
+    OAuth2Client,
+    BearerToken,
+    BackChannelAuthenticationPoolingJob,
+)
+
 client = OAuth2Client(
-    token_endpoint="https://myas.local/token",
-    backchannel_authentication_endpoint="https://myas.local/backchannel_authorize",
-    auth=(client_id, client_secret),
+    token_endpoint="https://url.to.the/token_endpoint",
+    backchannel_authentication_endpoint="https://url.to.the/backchannel_authorization_endpoint",
+    auth=("client_id", "client_secret"),
 )
 
 ba_resp = client.backchannel_authentication_request(
     scope="openid email profile",
     login_hint="user@example.net",
 )
-```
-
-`ba_resp` will contain the response attributes as returned by the AS, including an `auth_req_id`:
 
-```python
+# `ba_resp` will contain the response attributes as returned by the AS, including an `auth_req_id`:
 ba_resp.auth_req_id
 ba_resp.expires_in  # decreases as times fly
 ba_resp.expires_at  # a datetime to keep track of the expiration date, based on the "expires_in" returned by the AS
 ba_resp.interval  # the pooling interval indicated by the AS
 ba_resp.custom  # if the AS respond with additional attributes, they are also accessible
-```
 
-To pool the Token Endpoint until the end-user successfully authenticates:
-
-```python
-pool_job = BackChannelAuthenticationPoolingJob(
-    client=client,
-    auth_req_id=ba_resp.auth_req_id,
-    interval=bca_resp.interval,
-)
+pool_job = BackChannelAuthenticationPoolingJob(client, ba_resp)
 
 resp = None
 while resp is None:
     resp = pool_job()
 
 assert isinstance(resp, BearerToken)
 ```
@@ -432,15 +555,20 @@
 ### Token Exchange
 
 To send a token exchange request, use the
 [OAuth2Client.token_exchange()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.token_exchange)
 method:
 
 ```python
-client = OAuth2Client(token_endpoint, auth=...)
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
 token = client.token_exchange(
     subject_token="your_token_value",
     subject_token_type="urn:ietf:params:oauth:token-type:access_token",
 )
 ```
 
 As with the other grant-type specific methods, you may specify additional keyword parameters, that will be passed to the
@@ -455,14 +583,21 @@
     actor_token_type="id_token",  # will be automatically replaced by "urn:ietf:params:oauth:token-type:id_token"
 )
 ```
 
 Or to make it even easier, types can be guessed based on the supplied subject or actor token:
 
 ```python
+from requests_oauth2client import BearerToken, ClientSecretJwt, IdToken, OAuth2Client
+
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
+
 token = client.token_exchange(
     subject_token=BearerToken(
         "your_token_value"
     ),  # subject_token_type will be "urn:ietf:params:oauth:token-type:access_token"
     actor_token=IdToken(
         "your_actor_token"
     ),  # actor_token_type will be "urn:ietf:params:oauth:token-type:id_token"
@@ -474,61 +609,81 @@
 `requests_oauth2client` supports several client authentication methods, as defined in multiple OAuth2.x standards. You
 select the appropriate method to use when initializing your [OAuth2Client], with the `auth` parameter. Once initialized,
 a client will automatically use the configured authentication method every time it sends a requested to an endpoint that
 requires client authentication. You don't have anything else to do afterwards.
 
 ### Client Secret Basic
 
-With **client_secret_basic**, `client_id` and `client_secret` are included in clear-text in the `Authorization` header when sending requests to the Token Endpoint. To use
-it, just pass a
+With **client_secret_basic**, `client_id` and `client_secret` are included in clear-text in the `Authorization` header
+when sending requests to the Token Endpoint. To use it, just pass a
 [`ClientSecretBasic(client_id, client_secret)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.ClientSecretBasic)
 as `auth` parameter:
 
 ```python
 from requests_oauth2client import OAuth2Client, ClientSecretBasic
 
-client = OAuth2Client(token_endpoint, auth=ClientSecretBasic(client_id, client_secret))
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretBasic("client_id", "client_secret"),
+)
 ```
 
 ### Client Secret Post
 
-With **client_secret_post**, `client_id` and `client_secret` are included as part of the body form data. To use it, pass a
+With **client_secret_post**, `client_id` and `client_secret` are included as part of the body form data. To use it, pass
+a
 [`ClientSecretPost(client_id, client_secret)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.ClientSecretPost)
-as `auth` parameter. This is the default when you pass a tuple `(client_id, client_secret)` as
-`auth` when initializing an `OAuth2Client`:
+as `auth` parameter. This is the default when you pass a tuple `(client_id, client_secret)` as `auth` when initializing
+an `OAuth2Client`:
 
 ```python
 from requests_oauth2client import OAuth2Client, ClientSecretPost
 
-client = OAuth2Client(token_endpoint, auth=ClientSecretPost(client_id, client_secret))
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretPost("client_id", "client_secret"),
+)
+# or
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint", auth=("client_id", "client_secret")
+)
 # or
-client = OAuth2Client(token_endpoint, auth=(client_id, client_secret))
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    client_id="my_client_id",
+    client_secret="my_client_secret",
+)
 ```
 
 ### Client Secret JWT
 
-With **client_secret_jwt**, the client generates an ephemeral JWT assertion including information about itself (client_id), the
-AS (url of the endpoint), and an expiration date a few seconds in the future. To use it, pass a
+With **client_secret_jwt**, the client generates an ephemeral JWT assertion including information about itself
+(client_id), the AS (url of the endpoint), and an expiration date a few seconds in the future. To use it, pass a
 [`ClientSecretJwt(client_id, client_secret)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.ClientSecretJwt)
 as `auth` parameter. Assertion generation is entirely automatic, you don't have anything to do:
 
 ```python
 from requests_oauth2client import OAuth2Client, ClientSecretJwt
 
-client = OAuth2Client(token_endpoint, auth=ClientSecretJwt(client_id, client_secret))
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
 ```
 
-This method is more secure than the 2 previous, because only ephemeral credentials are transmitted, which limits the possibility for interception and replay of the Client Secret.
-But that Client Secret still needs to be shared between the AS and Client owner(s).
+This method is more secure than the 2 previous, because only ephemeral credentials are transmitted, which limits the
+possibility for interception and replay of the Client Secret. But that Client Secret still needs to be shared between
+the AS and Client owner(s).
 
 ### Private Key JWT
 
-With **private_key_jwt**, client uses a JWT assertion that is just like _client_secret_jwt_, but it is signed with an _asymmetric_ key.
-To use it, you need a private signing key, in a `dict` that matches the JWK format, or as an instance of `jwskate.Jwk`. The matching public key must be
-registered for your client on AS side. Once you have that, using this auth method is simple with the
+With **private_key_jwt**, client uses a JWT assertion that is just like the one for _client_secret_jwt_, but it is
+signed with an _asymmetric_ key. To use it, you need a private signing key, in a `dict` that matches the JWK format, or
+as an instance of `jwskate.Jwk`. The matching public key must be registered for your client on AS side. Once you have
+that, using this auth method is simple with the
 [`PrivateKeyJwt(client_id, private_jwk)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.PrivateKeyJwt)
 auth handler:
 
 ```python
 from requests_oauth2client import OAuth2Client, PrivateKeyJwt
 
 private_jwk = {
@@ -541,143 +696,154 @@
     "q": "...",
     "dp": "...",
     "dq": "...",
     "qi": "...",
 }
 
 client = OAuth2Client(
-    "https://myas.local/token", auth=PrivateKeyJwt(client_id, private_jwk)
+    "https://url.to.the/token_endpoint", auth=PrivateKeyJwt("client_id", private_jwk)
 )
 # or
-client = OAuth2Client(token_endpoint, auth=(client_id, private_jwk))
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint", auth=("client_id", private_jwk)
+)
+# or
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint", client_id="client_id", private_jwk=private_jwk
+)
 ```
 
-This method can be considered more secure than those relying on a client secret, because only ephemeral credentials are sent over the wire, and it uses asymetric cryptography: the signing key is generated by the client, and only the public key is known by the AS.
-Transmitting that public key between owner(s) of the client and of the AS is much easier than transmitting the Client Secret, which is a shared key that must be considered as confidential.
+This method can be considered more secure than those relying on a client secret, because only ephemeral credentials are
+sent over the wire, and it uses asymmetric cryptography: the signing key is generated by the client, and only the public
+key is known by the AS. Transmitting that public key between owner(s) of the client and of the AS is much easier than
+transmitting the Client Secret, which is a shared key that must be considered as confidential.
 
 ### None
 
-The latest Client Authentication Method, **none**, is for Public Clients which do not authenticate to the Token Endpoint.
-Those clients only include their `client_id` in body form data, without any authentication credentials. Use
+The latest Client Authentication Method, **none**, is for Public Clients which do not authenticate to the Token
+Endpoint. Those clients only include their `client_id` in body form data, without any authentication credentials. Use
 [`PublicApp(client_id)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.PublicApp):
 
 ```python
 from requests_oauth2client import OAuth2Client, PublicApp
 
-client = OAuth2Client(token_endpoint, auth=PublicApp(client_id, client_secret))
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint", auth=PublicApp("app_client_id")
+)
 ```
 
 ## Token Revocation
 
 [OAuth2Client] can send revocation requests to a Revocation Endpoint. You need to provide a Revocation Endpoint URI when
-creating the [OAuth2Client] :
-
-```python
-oauth2client = OAuth2Client(
-    token_endpoint,
-    revocation_endpoint=revocation_endpoint,
-    auth=ClientSecretJwt("client_id", "client_secret"),
-)
-```
-
-The
+creating the [OAuth2Client]. The
 [OAuth2Client.revoke_token()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.revoke_token)
 method and its specialized aliases
 [.revoke_access_token()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.revoke_access_token)
 and
 [.revoke_refresh_token()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.revoke_refresh_token)
 are then available:
 
 ```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    revocation_endpoint="https://url.to.the/revocation_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
+
 oauth2client.revoke_token("mytoken", token_type_hint="access_token")
 oauth2client.revoke_access_token(
     "mytoken"
 )  # will automatically add token_type_hint=access_token
 oauth2client.revoke_refresh_token(
     "mytoken"
 )  # will automatically add token_type_hint=refresh_token
 ```
 
 Because Revocation Endpoints usually don't return meaningful responses, those methods return a boolean. This boolean
-indicates that a request was successfully sent and no error was returned. If the Authorization Server actually returns a
-standardised error, an exception will be raised instead.
+indicates that a request was successfully sent and no error was returned. If the Authorization Server returns a
+non-successful HTTP code, but no standardised error message, it will return `False`. If the Authorization Server
+actually returns a standardised error, an exception will be raised instead, like the other methods from `OAuth2Client`.
 
 ## Token Introspection
 
 [OAuth2Client] can send requests to a Token Introspection Endpoint. You need to provide an Introspection Endpoint URI
-when creating the `OAuth2Client`:
+when creating the `OAuth2Client`. The
+[OAuth2Client.introspect_token()](<https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.instrospect_token()>)
+method is then available:
 
 ```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
 oauth2client = OAuth2Client(
-    token_endpoint,
-    introspection_endpoint=introspection_endpoint,
+    token_endpoint="https://url.to.the/token_endpoint",
+    introspection_endpoint="https://url.to.the/introspection_endpoint",
     auth=ClientSecretJwt("client_id", "client_secret"),
 )
-```
 
-The
-[OAuth2Client.introspect_token()](<https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.instrospect_token()>)
-method is then available:
-
-```python
 resp = oauth2client.introspect_token("mytoken", token_type_hint="access_token")
 ```
 
 It returns whatever data is returned by the introspection endpoint (if it is a JSON, its content is returned decoded).
 
 ## UserInfo Requests
 
 [OAuth2Client] can send requests to an UserInfo Endpoint. You need to provide an UserInfo Endpoint URI when creating the
-`OAuth2Client`:
+`OAuth2Client`. The
+[OAuth2Client.userinfo()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.userinfo))
+method is then available:
 
 ```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
 oauth2client = OAuth2Client(
-    token_endpoint,
-    userinfo_endpoint=userinfo_endpoint,
+    token_endpoint="https://url.to.the/token_endpoint",
+    userinfo_endpoint="https://url.to.the/userinfo_endpoint",
     auth=ClientSecretJwt("client_id", "client_secret"),
 )
-```
-
-The
-[OAuth2Client.userinfo()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.userinfo))
-method is then available:
-
-```python
 resp = oauth2client.userinfo("mytoken")
 ```
 
 It returns whatever data is returned by the userinfo endpoint (if it is a JSON, its content is returned decoded).
 
 ## Initializing an OAuth2Client from a discovery document
 
 You can initialize an [OAuth2Client] with the endpoint URIs mentioned in a standardised discovery document with the
 [OAuth2Client.from_discovery_endpoint()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.from_discovery_document)
 class method:
 
 ```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
 oauth2client = OAuth2Client.from_discovery_endpoint(
-    "https://myas.local/.well-known/openid-configuration"
+    "https://url.to.the/.well-known/openid-configuration",
+    auth=ClientSecretJwt("client_id", "client_secret"),
 )
 ```
 
 This will fetch the document from the specified URI, then will decode it and initialize an [OAuth2Client] pointing to
 the appropriate endpoint URIs.
 
 ## Specialized API Client
 
 Using APIs usually involves multiple endpoints under the same root url, with a common authentication method. To make it
-easier, `requests_oauth2client` includes a [requests.Session] wrapper called [ApiClient], which takes the
-root API url as parameter on initialization. You can then send requests to different endpoints by passing their relative
-path instead of the full url. [ApiClient] also accepts an `auth` parameter with an AuthHandler. You can pass any of the
-OAuth2 Auth Handler from this module, or any [requests]-compatible
-[Authentication Handler](https://requests.readthedocs.io/en/latest/user/advanced/#custom-authentication). Which makes
-it very easy to call APIs that are protected with an OAuth2 Client Credentials Grant:
+easier, `requests_oauth2client` includes a [requests.Session] wrapper called [ApiClient], which takes the root API url
+as parameter on initialization. You can then send requests to different endpoints by passing their relative path instead
+of the full url. [ApiClient] also accepts an `auth` parameter with an AuthHandler. You can pass any of the OAuth2 Auth
+Handler from this module, or any [requests]-compatible
+[Authentication Handler](https://requests.readthedocs.io/en/latest/user/advanced/#custom-authentication). Which makes it
+very easy to call APIs that are protected with an OAuth2 Client Credentials Grant:
 
 ```python
-oauth2client = OAuth2Client("https://myas.local/token", (client_id, client_secret))
+from requests_oauth2client import OAuth2Client, ApiClient, OAuth2ClientCredentialsAuth
+
+oauth2client = OAuth2Client(
+    "https://url.to.the/token_endpoint", ("client_id", "client_secret")
+)
 api = ApiClient(
     "https://myapi.local/root", auth=OAuth2ClientCredentialsAuth(oauth2client)
 )
 
 # will actually send a GET to https://myapi.local/root/resource/foo
 resp = api.get("/resource/foo")
 ```
@@ -703,30 +869,34 @@
 You can also use a syntax based on `__getattr__` or `__getitem__`:
 
 ```python
 api.resource.get()  # will send a GET to https://myapi.local/root/resource
 api["my-resource"].get()  # will send a GET to https://myapi.local/root/my-resource
 ```
 
-Both `__getattr__` and `__getitem__` return a new `ApiClient` initialised on the new base_url.
-So you can easily call multiple sub-resources on the same API this way:
+Both `__getattr__` and `__getitem__` return a new `ApiClient` initialised on the new base_url. So you can easily call
+multiple sub-resources on the same API this way:
 
 ```python
+from requests_oauth2client import ApiClient
+
 api = ApiClient("https://myapi.local")
 users_api = api.users
 user = users_api.get("userid")  # GET https://myapi.local/users/userid
 other_user = users_api.get("other_userid")  # GET https://myapi.local/users/other_userid
 resources_api = api.resources
 resources = resources_api.get()  # GET https://myapi.local/resources
 ```
 
 [ApiClient] will, by default, raise exceptions whenever a request returns an error status. You can disable that by
 passing `raise_for_status=False` when initializing your [ApiClient]:
 
 ```python
+from requests_oauth2client import ApiClient
+
 api = ApiClient(
     "http://httpstat.us", raise_for_status=False
 )  # raise_for_status defaults to True
 resp = api.get("500")
 assert resp is not None
 # without raise_for_status=False, a requests.exceptions.HTTPError exception would be raised instead
 ```
@@ -734,46 +904,49 @@
 You may override this at request time:
 
 ```python
 # raise_for_status at request-time overrides the value defined at init-time
 resp = api.get("500", raise_for_status=True)
 ```
 
-You can access the underlying `requests.Session` with the session attribute, and you can provide an already existing and configured `Session` instance at init time:
+You can access the underlying `requests.Session` with the session attribute, and you can provide an already existing and
+configured `Session` instance at init time:
 
 ```python
 import requests
+from requests_oauth2client import ApiClient
 
 session = requests.Session()
 session.proxies = {"https": "http://localhost:3128"}
 api = ApiClient("https://myapi.local/resource", session=session)
 assert api.session == session
 ```
 
 ## Vendor-Specific clients
 
 `requests_oauth2client` being flexible enough to handle most use cases, you should be able to use any AS by any vendor
 as long as it supports OAuth 2.0.
 
 You can however create a subclass of [OAuth2Client] or [ApiClient] to make it easier to use with specific Authorization
-Servers or APIs. The sub-module `requests_oauth2client.vendor_specific` includes such classes for [Auth0](https://auth0.com):
+Servers or APIs. The sub-module `requests_oauth2client.vendor_specific` includes such classes for
+[Auth0](https://auth0.com):
 
 ```python
-from requests_oauth2client.vendor_specific import Auth0Client
+from requests_oauth2client.vendor_specific import Auth0Client, Auth0ManagementApiClient
 
-a0client = Auth0Client("mytenant.eu", (client_id, client_secret))
+a0client = Auth0Client("mytenant.eu", ("client_id", "client_secret"))
 # this will automatically initialize the token endpoint to https://mytenant.eu.auth0.com/oauth/token
 # and other endpoints accordingly
 token = a0client.client_credentials(audience="audience")
 
 # this is a wrapper around Auth0 Management API
-a0mgmt = Auth0ManagementApiClient("mytenant.eu", (client_id, client_secret))
+a0mgmt = Auth0ManagementApiClient("mytenant.eu", ("client_id", "client_secret"))
 myusers = a0mgmt.get("users")
 ```
 
 [apiclient]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.api_client.ApiClient
-[authorizationrequest]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.authorization_request.AuthorizationRequest
 [bearerauth]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.BearerAuth
 [bearertoken]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.tokens.BearerToken
 [oauth2client]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client
 [requests]: https://requests.readthedocs.io/en/latest/
 [requests.session]: https://requests.readthedocs.io/en/latest/api/#requests.Session
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `requests_oauth2client-1.1.0/pyproject.toml` & `requests_oauth2client-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool]
 [tool.poetry]
 name = "requests_oauth2client"
-version = "1.1.0"
+version = "1.2.0"
 homepage = "https://github.com/guillp/requests_oauth2client"
 description = "An OAuth2.x Client based on requests."
 authors = ["Guillaume Pujol <guill.p.linux@gmail.com>"]
 readme = "README.md"
-license =  "Apache-2.0"
-classifiers=[
+license = "Apache-2.0"
+classifiers = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Security',
     'License :: OSI Approved :: Apache Software License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
@@ -22,49 +22,50 @@
 ]
 packages = [
     { include = "requests_oauth2client" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8,<3.12"
 
 requests = ">=2.19.0"
-binapy = "^0.6"
+binapy = ">=0.6.1"
 furl = ">=2.1.2"
-jwskate = "^0.3.0"
+jwskate = ">=0.8"
+
 
 [tool.poetry.dev-dependencies]
-black  = ">=22.1.0"
+black = ">=22.10.0"
 coverage = ">=6.3.1"
-isort  = ">=5.9.3"
+isort = ">=5.9.3"
 flask = ">=2.0.1"
 livereload = ">=2.6.3"
-mypy = ">=0.931"
-mkdocs  = ">=1.3.1"
+mypy = ">=1.4"
+mkdocs = ">=1.3.1"
 mkdocs-autorefs = ">=0.3.0"
-mkdocs-include-markdown-plugin  = ">=3.2.3"
-mkdocs-material  = ">=8.2.1"
-mkdocs-material-extensions  = ">=1.0.1"
+mkdocs-include-markdown-plugin = ">=3.2.3"
+mkdocs-material = ">=8.2.1"
+mkdocs-material-extensions = ">=1.0.1"
 mkdocstrings = { version = ">=0.18.0", extras = ["python"] }
 pre-commit = ">=2.12.0"
-pytest  = ">=7.0.1"
-pytest-cov  = ">=3.0.0"
+pytest = ">=7.0.1"
+pytest-cov = ">=3.0.0"
 pytest-mypy = ">=0.9.1"
 requests-mock = ">=1.9.3"
 toml = ">=0.10.2"
-tox  = ">=3.20.1"
+tox = ">=4"
 types-requests = ">=2.25.10"
 types-cryptography = ">=3.3.15"
-virtualenv  = ">=20.2.2"
+virtualenv = ">=20.2.2"
 pytest-freezegun = "^0.4.2"
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-cov"]
-doc = ["mkdocs", "mkdocs-autorefs", "mkdocs-include-markdown-plugin", "mkdocs-material", "mkdocs-material-extensions", "mkdocstrings"]
+doc = ["mdformat", "mkdocs", "mkdocs-autorefs", "mkdocs-include-markdown-plugin", "mkdocs-material", "mkdocs-material-extensions", "mkdocstrings"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 96
@@ -90,7 +91,17 @@
 show_error_context = true
 show_column_numbers = true
 show_error_codes = true
 pretty = true
 warn_unused_configs = true
 warn_unused_ignores = true
 warn_redundant_casts = true
+
+
+[tool.pytest.ini_options]
+requests_mock_case_sensitive = true
+markers = [
+    "slow: marks tests as slow"
+]
+filterwarnings = [
+    "ignore::DeprecationWarning: distutils Version classes are deprecated. Use packaging.version instead."
+]
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/__init__.py` & `requests_oauth2client-1.2.0/requests_oauth2client/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     OAuth2AccessTokenAuth,
     OAuth2AuthorizationCodeAuth,
     OAuth2ClientCredentialsAuth,
     OAuth2DeviceCodeAuth,
 )
 from .authorization_request import (
     AuthorizationRequest,
+    AuthorizationRequestSerializer,
     AuthorizationResponse,
     PkceUtils,
     RequestUriParameterAuthorizationRequest,
 )
 from .backchannel_authentication import (
     BackChannelAuthenticationPoolingJob,
     BackChannelAuthenticationResponse,
@@ -49,23 +50,27 @@
     ConsentRequired,
     DeviceAuthorizationError,
     EndpointError,
     ExpiredAccessToken,
     ExpiredToken,
     InteractionRequired,
     InvalidBackChannelAuthenticationResponse,
+    InvalidClient,
     InvalidDeviceAuthorizationResponse,
     InvalidGrant,
     InvalidIdToken,
+    InvalidPushedAuthorizationResponse,
+    InvalidRequest,
     InvalidScope,
     InvalidTokenResponse,
     LoginRequired,
     MismatchingIssuer,
     MismatchingState,
     MissingAuthCode,
+    MissingIssuer,
     OAuth2Error,
     ServerError,
     SessionSelectionRequired,
     SlowDown,
     UnauthorizedClient,
     UnknownIntrospectionError,
     UnknownTokenEndpointError,
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/api_client.py` & `requests_oauth2client-1.2.0/requests_oauth2client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 from typing import (
     IO,
     Any,
     Callable,
     Iterable,
+    List,
     Mapping,
     MutableMapping,
     Optional,
     Tuple,
     Union,
 )
 from urllib.parse import quote as urlencode
@@ -93,20 +94,21 @@
 
     def request(  # noqa: C901
         self,
         method: str,
         url: Union[None, str, bytes, Iterable[Union[str, bytes, int]]] = None,
         params: Union[None, bytes, MutableMapping[str, str]] = None,
         data: Union[
-            None,
+            Iterable[bytes],
             str,
             bytes,
-            Mapping[str, Any],
-            Iterable[Tuple[str, Optional[str]]],
-            IO[Any],
+            List[Tuple[Any, Any]],
+            Tuple[Tuple[Any, Any], ...],
+            Mapping[Any, Any],
+            None,
         ] = None,
         headers: Optional[MutableMapping[str, str]] = None,
         cookies: Union[None, RequestsCookieJar, MutableMapping[str, str]] = None,
         files: Optional[MutableMapping[str, IO[Any]]] = None,
         auth: Union[
             None,
             Tuple[str, str],
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/auth.py` & `requests_oauth2client-1.2.0/requests_oauth2client/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """This module contains requests-compatible Auth Handlers that implement OAuth 2.0."""
 
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 import requests
 
+from .authorization_request import AuthorizationResponse
 from .device_authorization import DeviceAuthorizationResponse
 from .exceptions import ExpiredAccessToken
 from .tokens import BearerToken
 
 if TYPE_CHECKING:  # pragma: no cover
     from .client import OAuth2Client
 
 
 class BearerAuth(requests.auth.AuthBase):
-    """An Auth Handler that includes a Bearer Token in API calls.
+    """An Auth Handler that includes a Bearer Token in API calls, as defined in [RFC6750$2.1].
 
-    Thus is as defined in [RFC6750$2.1](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1).
+    As a prerequisite to using this `AuthBase`, you have to obtain an access token manually.
+    You most likely don't want do to that by yourself, but instead use an instance of
+    [OAuth2Client][requests_oauth2client.client.OAuth2Client] to do that for you.
+    See the others Auth Handlers in this module, which will automatically obtain access tokens from an OAuth 2.x server.
 
-    As a prerequisite to using this AuthBase, you have to obtain an access token manually.
-    You most likely don't want do to that by yourself. See the others Auth Handlers in this module,
-    that will automatically obtain access tokens from an OAuth 2.x server.
+    [RFC6750$2.1]: https://datatracker.ietf.org/doc/html/rfc6750#section-2.1
 
     Usage:
         ```python
         auth = BearerAuth("my_access_token")
         resp = requests.get("https://my.api.local/resource", auth=auth)
         ```
 
@@ -39,15 +41,15 @@
     """
 
     def __init__(self, token: Optional[Union[str, BearerToken]] = None) -> None:
         self.token = token  # type: ignore[assignment] # until https://github.com/python/mypy/issues/3004 is fixed
 
     @property
     def token(self) -> Optional[BearerToken]:
-        """Return the token that is used for authorization against the API.
+        """Return the [BearerToken] that is used for authorization against the API.
 
         Returns:
             the configured [BearerToken][requests_oauth2client.tokens.BearerToken] used with this AuthHandler.
         """
         return self._token
 
     @token.setter
@@ -65,15 +67,15 @@
 
     def __call__(self, request: requests.PreparedRequest) -> requests.PreparedRequest:
         """Implement the usage of Bearer Tokens in requests.
 
         This will add a properly formatted `Authorization: Bearer <token>` header in
         the request.
 
-        If the configuerd token is a instance of BearerToken with an expires_at attribute,
+        If the configured token is a instance of BearerToken with an expires_at attribute,
         raises [ExpiredAccessToken][requests_oauth2client.exceptions.ExpiredAccessToken] once the access token is expired.
 
         Args:
             request: a [PreparedRequest][requests.PreparedRequest]
 
         Returns:
             a [PreparedRequest][requests.PreparedRequest] with an Access Token added in Authorization Header
@@ -210,17 +212,22 @@
         ```python
         client = OAuth2Client(token_endpoint="https://my.as.local/token", auth=("client_id", "client_secret"))
         code = "my_code" # you must obtain this code yourself
         resp = requests.post("https://my.api.local/resource", auth=OAuth2AuthorizationCodeAuth(client, code))
         ````
     """
 
-    def __init__(self, client: "OAuth2Client", code: str, **token_kwargs: Any) -> None:
+    def __init__(
+        self,
+        client: "OAuth2Client",
+        code: Union[str, AuthorizationResponse],
+        **token_kwargs: Any,
+    ) -> None:
         super().__init__(client, None)
-        self.code: Optional[str] = code
+        self.code: Union[str, AuthorizationResponse, None] = code
         self.token_kwargs = token_kwargs
 
     def __call__(self, request: requests.PreparedRequest) -> requests.PreparedRequest:
         """Implement the Authorization Code grant as an Authentication Handler.
 
         This exchanges an Authorization Code for an access token and adds it in the request.
 
@@ -239,35 +246,35 @@
         """Obtain the initial access token with the authorization_code grant."""
         if self.code:  # pragma: no branch
             self.token = self.client.authorization_code(code=self.code, **self.token_kwargs)
             self.code = None
 
 
 class OAuth2DeviceCodeAuth(OAuth2AccessTokenAuth):
-    """Authentication Handler for Device Code.
+    """Authentication Handler for the [Device Code Flow](https://www.rfc-editor.org/rfc/rfc8628).
 
     This [Requests Auth handler][requests.auth.AuthBase] implementation exchanges a Device Code for
-    an access token, then automatically refreshes it once it is expired.
+    an Access Token, then automatically refreshes it once it is expired.
 
     It needs a Device Code and an [OAuth2Client][requests_oauth2client.client.OAuth2Client] to be able to get
     a token from the AS Token Endpoint just before the first request using this Auth Handler is being sent.
 
     Args:
         client: the [OAuth2Client][requests_oauth2client.client.OAuth2Client] to use to obtain Access Tokens.
         device_code: a Device Code obtained from the AS.
         interval: the interval to use to pool the Token Endpoint, in seconds.
         expires_in: the lifetime of the token, in seconds.
         **token_kwargs: additional kwargs to pass to the token endpoint.
 
     Usage:
         ```python
         client = OAuth2Client(token_endpoint="https://my.as.local/token", auth=("client_id", "client_secret"))
-        device_code = "my_device_code"
-        oauth2ac_auth = OAuth2DeviceCodeAuth(client, device_code)
-        resp = requests.post("https://my.api.local/resource", auth=oauth2ac_auth)
+        device_code = client.device_authorization()
+        auth = OAuth2DeviceCodeAuth(client, device_code)
+        resp = requests.post("https://my.api.local/resource", auth=auth)
         ````
     """
 
     def __init__(
         self,
         client: "OAuth2Client",
         device_code: Union[str, DeviceAuthorizationResponse],
@@ -280,29 +287,36 @@
         self.interval = interval
         self.expires_in = expires_in
         self.token_kwargs = token_kwargs
 
     def __call__(self, request: requests.PreparedRequest) -> requests.PreparedRequest:
         """Implement the Device Code grant as a request Authentication Handler.
 
-        This exchanges a Device Code for an access token and adds it in the request.
+        This exchanges a Device Code for an access token and adds it in HTTP requests.
 
         Args:
-            request: a [PreparedRequest][requests.PreparedRequest]
+            request: a [requests.PreparedRequest][]
 
         Returns:
-            a [PreparedRequest][requests.PreparedRequest] with an Access Token added in Authorization Header
+            a [requests.PreparedRequest][] with an Access Token added in Authorization Header
         """
-        from .device_authorization import DeviceAuthorizationPoolingJob
-
         token = self.token
         if token is None or token.is_expired():
-            if self.device_code:  # pragma: no branch
-                pooling_job = DeviceAuthorizationPoolingJob(
-                    client=self.client,
-                    device_code=self.device_code,
-                    interval=self.interval,
-                )
-                while self.token is None:
-                    self.token = pooling_job()
-                self.device_code = None
+            self.exchange_device_code_for_token()
         return super().__call__(request)
+
+    def exchange_device_code_for_token(self) -> None:
+        """Exchange the Device Code for an access token.
+
+        This will poll the Token Endpoint until the user finishes the authorization process.
+        """
+        from .device_authorization import DeviceAuthorizationPoolingJob
+
+        if self.device_code:  # pragma: no branch
+            pooling_job = DeviceAuthorizationPoolingJob(
+                client=self.client,
+                device_code=self.device_code,
+                interval=self.interval,
+            )
+            while self.token is None:
+                self.token = pooling_job()
+            self.device_code = None
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/authorization_request.py` & `requests_oauth2client-1.2.0/requests_oauth2client/authorization_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Classes and utilities related to Authorization Requests and Responses."""
-
+from __future__ import annotations
 
 import re
 import secrets
 from datetime import datetime
-from typing import Any, Dict, Iterable, Optional, Tuple, Type, Union
+from typing import Any, Callable, Dict, Iterable, Mapping, Optional, Tuple, Type, Union
 
 from binapy import BinaPy
 from furl import furl  # type: ignore[import]
-from jwskate import Jwk, Jwt
+from jwskate import JweCompact, Jwk, Jwt, SignedJwt
+from typing_extensions import Literal
 
 from .exceptions import (
     AuthorizationResponseError,
     ConsentRequired,
     InteractionRequired,
     LoginRequired,
     MismatchingIssuer,
     MismatchingState,
     MissingAuthCode,
+    MissingIssuer,
     SessionSelectionRequired,
 )
 from .utils import accepts_expires_in
 
 
 class PkceUtils:
     """Contains helper methods for PKCE, as described in RFC7636.
@@ -140,24 +142,30 @@
             response
         )  # you can pass this response on a call to `OAuth2Client.authorization_code()`
         ```
     """
 
     def __init__(
         self,
-        code: Optional[str] = None,
+        code: str,
         redirect_uri: Optional[str] = None,
         code_verifier: Optional[str] = None,
         state: Optional[str] = None,
+        nonce: Optional[str] = None,
+        acr_values: Optional[Iterable[str]] = None,
+        max_age: Optional[int] = None,
         **kwargs: str,
     ):
         self.code = code
         self.redirect_uri = redirect_uri
         self.code_verifier = code_verifier
         self.state = state
+        self.nonce = nonce
+        self.acr_values = list(acr_values) if acr_values is not None else None
+        self.max_age = max_age
         self.others = kwargs
 
     def __getattr__(self, item: str) -> Optional[str]:
         """Make additional parameters available as attributes.
 
         Args:
             item: the attribute name
@@ -192,56 +200,80 @@
         client_id: the client_id to include in the request.
         redirect_uri: the redirect_uri to include in the request. This is required in OAuth 2.0 and optional
             in OAuth 2.1. Pass `None` if you don't need any redirect_uri in the Authorization Request.
         scope: the scope to include in the request, as an iterable of `str`, or a single space-separated `str`.
         response_type: the response type to include in the request.
         state: the state to include in the request, or `True` to autogenerate one (default).
         nonce: the nonce to include in the request, or `True` to autogenerate one (default).
-        code_verifier: the state to include in the request, or `True` to autogenerate one (default).
+        code_verifier: the code verifier to include in the request. If left as `None` and `code_challenge_method` is set, a valid code_verifier will be generated.
         code_challenge_method: the method to use to derive the `code_challenge` from the `code_verifier`.
-        issuer: Issuer Identifier value from the OAuth/OIDC Server, if known. Set it to `False` if the AS doesn't support Server Issuer Identification.
+        acr_values: requested Authentication Context Class Reference values.
+        issuer: Issuer Identifier value from the OAuth/OIDC Server, if using Server Issuer Identification.
         **kwargs: extra parameters to include in the request, as-is.
     """
 
     exception_classes: Dict[str, Type[Exception]] = {
         "interaction_required": InteractionRequired,
         "login_required": LoginRequired,
         "session_selection_required": SessionSelectionRequired,
         "consent_required": ConsentRequired,
     }
 
+    @classmethod
+    def generate_state(cls) -> str:
+        """Generate a random `state` parameter."""
+        return secrets.token_urlsafe(32)
+
+    @classmethod
+    def generate_nonce(cls) -> str:
+        """Generate a random `nonce`."""
+        return secrets.token_urlsafe(32)
+
     def __init__(
         self,
         authorization_endpoint: str,
         client_id: str,
-        redirect_uri: Optional[str],
-        scope: Union[None, str, Iterable[str]],
+        redirect_uri: Optional[str] = None,
+        scope: Union[None, str, Iterable[str]] = "openid",
         response_type: str = "code",
-        state: Union[str, bool, None] = True,
-        nonce: Union[str, bool, None] = True,
+        state: Union[str, Literal[True], None] = True,
+        nonce: Union[str, Literal[True], None] = True,
         code_verifier: Optional[str] = None,
         code_challenge_method: Optional[str] = "S256",
-        issuer: Union[str, bool, None] = None,
+        acr_values: Union[str, Iterable[str], None] = None,
+        max_age: Union[int, None] = None,
+        issuer: Optional[str] = None,
+        authorization_response_iss_parameter_supported: bool = False,
         **kwargs: Any,
     ) -> None:
+        if authorization_response_iss_parameter_supported and not issuer:
+            raise ValueError(
+                "When 'authorization_response_iss_parameter_supported' is True, you must provide the expected 'issuer' as parameter."
+            )
+
         if state is True:
-            state = secrets.token_urlsafe(32)
-        elif state is False:
-            state = None
-
-        if scope is not None and isinstance(scope, str):
-            scope = scope.split(" ")
-
-        if nonce is True and scope is not None and "openid" in scope:
-            nonce = secrets.token_urlsafe(32)
-        elif nonce is False:
-            nonce = None
+            state = self.generate_state()
 
-        if scope is not None and not isinstance(scope, str):
-            scope = " ".join(str(s) for s in scope)
+        if scope is not None:
+            if isinstance(scope, str):
+                scope = scope.split(" ")
+            else:
+                scope = tuple(scope)
+
+        if nonce is True:
+            if scope is not None and "openid" in scope:
+                nonce = self.generate_nonce()
+            else:
+                nonce = None
+
+        if acr_values is not None:
+            if isinstance(acr_values, str):
+                acr_values = acr_values.split()
+            elif not isinstance(acr_values, list):
+                acr_values = list(acr_values)
 
         if "code_challenge" in kwargs:
             raise ValueError(
                 "A code_challenge must not be passed as parameter. "
                 "Pass the code_verifier instead, and the appropriate code_challenge "
                 "will automatically be derived from it and included in the request, "
                 "based on code_challenge_method."
@@ -250,190 +282,264 @@
         if not code_challenge_method:
             code_verifier = code_challenge = code_challenge_method = None
         else:
             if not code_verifier:
                 code_verifier = PkceUtils.generate_code_verifier()
             code_challenge = PkceUtils.derive_challenge(code_verifier, code_challenge_method)
 
+        if max_age is not None:
+            if max_age < 0:
+                raise ValueError(
+                    "The `max_age` parameter is a number of seconds and cannot be negative."
+                )
+
         self.authorization_endpoint = authorization_endpoint
         self.client_id = client_id
         self.redirect_uri = redirect_uri
+        self.issuer = issuer
         self.response_type = response_type
         self.scope = scope
         self.state = state
         self.nonce = nonce
         self.code_verifier = code_verifier
         self.code_challenge = code_challenge
         self.code_challenge_method = code_challenge_method
+        self.acr_values = acr_values
+        self.max_age = max_age
+        self.authorization_response_iss_parameter_supported = (
+            authorization_response_iss_parameter_supported
+        )
         self.kwargs = kwargs
 
-        self.issuer = issuer
-
         self.args = dict(
             client_id=client_id,
             redirect_uri=redirect_uri,
             response_type=response_type,
-            scope=scope,
+            scope=" ".join(scope) if scope is not None else None,
             state=state,
             nonce=nonce,
             code_challenge=code_challenge,
             code_challenge_method=code_challenge_method,
+            acr_values=" ".join(acr_values) if acr_values is not None else None,
+            max_age=max_age,
             **kwargs,
         )
 
+    def as_dict(self) -> Mapping[str, Any]:
+        """Return a dict with all the parameters used to init this Authorization Request.
+
+        Used for serialization of this request. A new AuthorizationRequest initialized with the same parameters will be
+        equal to this one.
+
+        Returns:
+            a dict of parameters
+        """
+        return {
+            "authorization_endpoint": self.authorization_endpoint,
+            "client_id": self.client_id,
+            "redirect_uri": self.redirect_uri,
+            "scope": self.scope,
+            "response_type": self.response_type,
+            "state": self.state,
+            "nonce": self.nonce,
+            "code_verifier": self.code_verifier,
+            "code_challenge_method": self.code_challenge_method,
+            "issuer": self.issuer,
+            "authorization_response_iss_parameter_supported": self.authorization_response_iss_parameter_supported,
+            "acr_values": self.acr_values,
+            "max_age": self.max_age,
+            **self.kwargs,
+        }
+
     def sign_request_jwt(
-        self, jwk: Union[Jwk, Dict[str, Any]], alg: Optional[str] = None
-    ) -> Jwt:
+        self,
+        jwk: Union[Jwk, Dict[str, Any]],
+        alg: Optional[str] = None,
+        lifetime: Optional[int] = None,
+    ) -> SignedJwt:
         """Sign the `request` object that matches this Authorization Request parameters.
 
         Args:
             jwk: the JWK to use to sign the request
             alg: the alg to use to sign the request, if the passed `jwk` has no `alg` parameter.
+            lifetime: an optional number of seconds of validity for the signed reqeust. If present, `iat` an `exp` claims will be included in the signed JWT.
 
         Returns:
-            a :class:`Jwt` that contains the signed request object.
+            a `Jwt` that contains the signed request object.
         """
+        claims = {key: val for key, val in self.args.items() if val is not None}
+        if lifetime:
+            claims["iat"] = Jwt.timestamp()
+            claims["exp"] = Jwt.timestamp(lifetime)
         return Jwt.sign(
-            claims={key: val for key, val in self.args.items() if val is not None},
-            jwk=jwk,
+            claims,
+            key=jwk,
             alg=alg,
         )
 
     def sign(
-        self, jwk: Union[Jwk, Dict[str, Any]], alg: Optional[str] = None
-    ) -> "AuthorizationRequest":
-        """Sign the current Authorization Request.
+        self,
+        jwk: Union[Jwk, Dict[str, Any]],
+        alg: Optional[str] = None,
+        lifetime: Optional[int] = None,
+    ) -> RequestParameterAuthorizationRequest:
+        """Sign this Authorization Request and return a new one.
 
         This replaces all parameters with a signed `request` JWT.
 
         Args:
             jwk: the JWK to use to sign the request
             alg: the alg to use to sign the request, if the passed `jwk` has no `alg` parameter.
+            lifetime: lifetime of the resulting Jwt (used to calculate the 'exp' claim). By default, don't use an 'exp' claim.
 
         Returns:
             the signed Authorization Request
         """
-        request_jwt = self.sign_request_jwt(jwk, alg)
-        self.args = {"request": str(request_jwt)}
-        return self
+        request_jwt = self.sign_request_jwt(jwk, alg, lifetime)
+        return RequestParameterAuthorizationRequest(
+            authorization_endpoint=self.authorization_endpoint,
+            client_id=self.client_id,
+            request=str(request_jwt),
+            expires_at=request_jwt.expires_at,
+        )
 
     def sign_and_encrypt_request_jwt(
         self,
         sign_jwk: Union[Jwk, Dict[str, Any]],
         enc_jwk: Union[Jwk, Dict[str, Any]],
         sign_alg: Optional[str] = None,
         enc_alg: Optional[str] = None,
-        enc: Optional[str] = None,
-    ) -> Jwt:
+        enc: str = "A128CBC-HS256",
+        lifetime: Optional[int] = None,
+    ) -> JweCompact:
         """Sign and encrypt a `request` object for this Authorization Request.
 
         The signed `request` will contain the same parameters as this AuthorizationRequest.
 
         Args:
             sign_jwk: the JWK to use to sign the request
             enc_jwk: the JWK to use to encrypt the request
             sign_alg: the alg to use to sign the request, if the passed `jwk` has no `alg` parameter.
             enc_alg: the alg to use to encrypt the request, if the passed `jwk` has no `alg` parameter.
             enc: the encoding to use to encrypt the request, if the passed `jwk` has no `enc` parameter.
+            lifetime: lifetime of the resulting Jwt (used to calculate the 'exp' claim). By default, do not include an 'exp' claim.
 
         Returns:
             the signed and encrypted request object, as a `jwskate.Jwt`
         """
+        claims = {key: val for key, val in self.args.items() if val is not None}
+        if lifetime:
+            claims["iat"] = Jwt.timestamp()
+            claims["exp"] = Jwt.timestamp(lifetime)
         return Jwt.sign_and_encrypt(
-            claims={key: val for key, val in self.args.items() if val is not None},
-            sign_jwk=sign_jwk,
+            claims=claims,
+            sign_key=sign_jwk,
             sign_alg=sign_alg,
-            enc_jwk=enc_jwk,
+            enc_key=enc_jwk,
             enc_alg=enc_alg,
             enc=enc,
         )
 
     def sign_and_encrypt(
         self,
         sign_jwk: Union[Jwk, Dict[str, Any]],
         enc_jwk: Union[Jwk, Dict[str, Any]],
         sign_alg: Optional[str] = None,
         enc_alg: Optional[str] = None,
-        enc: Optional[str] = None,
-    ) -> "AuthorizationRequest":
+        enc: str = "A128CBC-HS256",
+        lifetime: Optional[int] = None,
+    ) -> RequestParameterAuthorizationRequest:
         """Sign and encrypt the current Authorization Request.
 
         This replaces all parameters with a matching `request` object.
 
         Args:
             sign_jwk: the JWK to use to sign the request
             enc_jwk: the JWK to use to encrypt the request
             sign_alg: the alg to use to sign the request, if the passed `jwk` has no `alg` parameter.
             enc_alg: the alg to use to encrypt the request, if the passed `jwk` has no `alg` parameter.
             enc: the encoding to use to encrypt the request, if the passed `jwk` has no `enc` parameter.
+            lifetime: lifetime of the resulting Jwt (used to calculate the 'exp' claim). By default, do not include an 'exp' claim.
 
         Returns:
             the same AuthorizationRequest, with a request object as parameter
         """
         request_jwt = self.sign_and_encrypt_request_jwt(
             sign_jwk=sign_jwk,
             enc_jwk=enc_jwk,
             sign_alg=sign_alg,
             enc_alg=enc_alg,
             enc=enc,
+            lifetime=lifetime,
+        )
+        return RequestParameterAuthorizationRequest(
+            authorization_endpoint=self.authorization_endpoint,
+            client_id=self.client_id,
+            request=str(request_jwt),
         )
-        self.args = {"client_id": self.client_id, "request": str(request_jwt)}
-        return self
 
     def validate_callback(self, response: str) -> AuthorizationResponse:
         """Validate an Authorization Response against this Request.
 
         Validate a given Authorization Response URI against this Authorization
         Request, and return an [AuthorizationResponse][requests_oauth2client.authorization_request.AuthorizationResponse].
 
         This includes matching the `state` parameter, checking for returned errors, and extracting the returned `code`
         and other parameters.
 
         Args:
             response: the Authorization Response URI. This can be the full URL, or just the query parameters.
 
         Returns:
-            the extracted code, if the
+            the extracted code, if all checks are successful
 
         Raises:
+            MismatchingIssuer: if the 'iss' received in the response doesn't match the expected value.
             MismatchingState: if the response `state` does not match the expected value.
             OAuth2Error: if the response includes an error.
             MissingAuthCode: if the response does not contain a `code`.
+            NotImplementedError: if response_type anything else than 'code'
         """
         try:
             response_url = furl(response)
         except ValueError:
             return self.on_response_error(response)
 
-        # validate 'iss' according to https://www.ietf.org/archive/id/draft-ietf-oauth-iss-auth-resp-05.html
-        expected_issuer = self.issuer
-        if expected_issuer is not None:
-            received_issuer = response_url.args.get("iss")
-            if (expected_issuer is False and received_issuer is not None) or (
-                expected_issuer and received_issuer != expected_issuer
-            ):
-                raise MismatchingIssuer(expected_issuer, received_issuer)
+        # validate 'iss' according to RFC9207
+        received_issuer = response_url.args.get("iss")
+        if self.authorization_response_iss_parameter_supported or received_issuer:
+            if received_issuer is None:
+                raise MissingIssuer()
+            if self.issuer and received_issuer != self.issuer:
+                raise MismatchingIssuer(self.issuer, received_issuer)
 
+        # validate state
         requested_state = self.state
         if requested_state:
             received_state = response_url.args.get("state")
             if requested_state != received_state:
                 raise MismatchingState(requested_state, received_state)
 
         error = response_url.args.get("error")
         if error:
             return self.on_response_error(response)
 
-        code: str = response_url.args.get("code")
-        if code is None:
-            raise MissingAuthCode()
+        if "code" in self.response_type:
+            code: str = response_url.args.get("code")
+            if code is None:
+                raise MissingAuthCode()
+        else:
+            raise NotImplementedError()
 
         return AuthorizationResponse(
             code_verifier=self.code_verifier,
             redirect_uri=self.redirect_uri,
+            nonce=self.nonce,
+            acr_values=self.acr_values,
+            max_age=self.max_age,
             **response_url.args,
         )
 
     def on_response_error(self, response: str) -> AuthorizationResponse:
         """Error handler for Authorization Response errors.
 
         Triggered by [validate_callback()][requests_oauth2client.authorization_request.AuthorizationRequest.validate_callback] if the response uri contains
@@ -449,68 +555,96 @@
         error = response_url.args.get("error")
         error_description = response_url.args.get("error_description")
         error_uri = response_url.args.get("error_uri")
         exception_class = self.exception_classes.get(error, AuthorizationResponseError)
         raise exception_class(error, error_description, error_uri)
 
     @property
-    def uri(self) -> str:
-        """Return the Authorization Request URI, as a `str`.
-
-        You may also use `repr()` or `str()` on an AuthorizationRequest to obtain the same uri.
-
-        Authorization requests typically look like:
-        ```
-        https://myas.local/authorize?client_id=<client_id>&response_type=code&scope=openid&redirect_uri=<redirect_uri>
-        ```
-        Unless they have been signed, and optionally encrypted, into a `request` object, then they look like:
-        ```
-        https://myas.local/authorize?client_id=<client_id>&request=<request>
-        ```
-
-        Returns:
-            the Authorization Request URI.
-        """
-        return str(
-            furl(
-                self.authorization_endpoint,
-                args={key: value for key, value in self.args.items() if value is not None},
-            ).url
+    def furl(self) -> furl:
+        """Return the Authorization Request URI, as a `furl`."""
+        return furl(
+            self.authorization_endpoint,
+            args={key: value for key, value in self.args.items() if value is not None},
         )
 
-    def __repr__(self) -> str:
-        """Return the Authorization Request URI, as a `str`.
+    @property
+    def uri(self) -> str:
+        """Return the Authorization Request URI, as a `str`."""
+        return str(self.furl.url)
 
-        Returns:
-            the Authorization Request URI.
-        """
+    def __repr__(self) -> str:
+        """Return the Authorization Request URI, as a `str`."""
         return self.uri
 
     def __eq__(self, other: Any) -> bool:
         """Check if this Authorization Request is the same as another one.
 
         Args:
             other: another AuthorizationRequest, or a url as string
 
         Returns:
             `True` if the other AuthorizationRequest is the same as this one, `False` otherwise
         """
         if isinstance(other, AuthorizationRequest):
             return (
                 self.authorization_endpoint == other.authorization_endpoint
-                and self.args == other.kwargs
-                and self.issuer == other.issuer
+                and self.args == other.args
             )
         elif isinstance(other, str):
             return self.uri == other
         return super().__eq__(other)
 
 
+class RequestParameterAuthorizationRequest:
+    """Represent an Authorization Request that includes a `request` JWT.
+
+    Args:
+        authorization_endpoint: the Authorization Endpoint uri
+        client_id: the client_id
+        request: the request JWT
+        expires_at: the expiration date for this request
+    """
+
+    @accepts_expires_in
+    def __init__(
+        self,
+        authorization_endpoint: str,
+        client_id: str,
+        request: str,
+        expires_at: Optional[datetime] = None,
+    ):
+        self.authorization_endpoint = authorization_endpoint
+        self.client_id = client_id
+        self.request = request
+        self.expires_at = expires_at
+
+    @property
+    def furl(self) -> furl:
+        """Return the Authorization Request URI, as a `furl` instance."""
+        return furl(
+            self.authorization_endpoint,
+            args={"client_id": self.client_id, "request": self.request},
+        )
+
+    @property
+    def uri(self) -> str:
+        """Return the Authorization Request URI, as a `str`."""
+        return str(self.furl.url)
+
+    def __repr__(self) -> str:
+        """Return the Authorization Request URI, as a `str`.
+
+        Returns:
+             the Authorization Request URI
+        """
+        return self.uri
+
+
 class RequestUriParameterAuthorizationRequest:
-    """Represent an Authorization Request that includes a `request` object.
+    """Represent an Authorization Request that includes a `request_uri` parameter.
 
     Args:
         authorization_endpoint: the Authorization Endpoint uri
         client_id: the client_id
         request_uri: the request_uri
         expires_at: the expiration date for this request
     """
@@ -525,27 +659,91 @@
     ):
         self.authorization_endpoint = authorization_endpoint
         self.client_id = client_id
         self.request_uri = request_uri
         self.expires_at = expires_at
 
     @property
+    def furl(self) -> furl:
+        """Return the Authorization Request URI, as a `furl` instance."""
+        return furl(
+            self.authorization_endpoint,
+            args={"client_id": self.client_id, "request_uri": self.request_uri},
+        )
+
+    @property
     def uri(self) -> str:
-        """Return the Authorization Request URI, as a `str`.
+        """Return the Authorization Request URI, as a `str`."""
+        return str(self.furl.url)
+
+    def __repr__(self) -> str:
+        """Return the Authorization Request URI, as a `str`."""
+        return self.uri
+
+
+class AuthorizationRequestSerializer:
+    """(De)Serializer for `AuthorizationRequest` instances.
+
+    You might need to store pending authorization requests in session, either server-side or client-
+    side. This class is here to help you do that.
+    """
+
+    def __init__(
+        self,
+        dumper: Optional[Callable[[AuthorizationRequest], str]] = None,
+        loader: Optional[Callable[[str], AuthorizationRequest]] = None,
+    ):
+        self.dumper = dumper or self.default_dumper
+        self.loader = loader or self.default_loader
+
+    @staticmethod
+    def default_dumper(azr: AuthorizationRequest) -> str:
+        """Provide a default dumper implementation.
+
+        Serialize an AuthorizationRequest as JSON, then compress with deflate, then encodes
+        as base64url.
+
+        Args:
+            azr: the `AuthorizationRequest` to serialize
 
         Returns:
-            the Authorization Request URI
+            the serialized value
         """
-        return str(
-            furl(
-                self.authorization_endpoint,
-                args={"client_id": self.client_id, "request_uri": self.request_uri},
-            ).url
-        )
+        return BinaPy.serialize_to("json", azr.as_dict()).to("deflate").to("b64u").ascii()
 
-    def __repr__(self) -> str:
-        """Return the Authorization Request URI, as a `str`.
+    def default_loader(
+        self, serialized: str, azr_class: Type[AuthorizationRequest] = AuthorizationRequest
+    ) -> AuthorizationRequest:
+        """Provide a default deserializer implementation.
+
+        This does the opposite operations than `default_dumper`.
+
+        Args:
+            serialized: the serialized AuthorizationRequest
 
         Returns:
-             the Authorization Request URI
+            an AuthorizationRequest
         """
-        return self.uri
+        args = BinaPy(serialized).decode_from("b64u").decode_from("deflate").parse_from("json")
+        return azr_class(**args)
+
+    def dumps(self, azr: AuthorizationRequest) -> str:
+        """Serialize and compress a given AuthorizationRequest for easier storage.
+
+        Args:
+            azr: an AuthorizationRequest to serialize
+
+        Returns:
+            the serialized AuthorizationRequest, as a str
+        """
+        return self.dumper(azr)
+
+    def loads(self, serialized: str) -> AuthorizationRequest:
+        """Deserialize a serialized AuthorizationRequest.
+
+        Args:
+            serialized: the serialized AuthorizationRequest
+
+        Returns:
+            the deserialized AuthorizationRequest
+        """
+        return self.loader(serialized)
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/backchannel_authentication.py` & `requests_oauth2client-1.2.0/requests_oauth2client/backchannel_authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Implementation of CIBA.
 
-CIBA stands for Client Initiated BackChannel Authentication and is standardised by the OpenID Fundation.
-https://openid.net/specs/openid-client-initiated-backchannel- authentication-core-1_0.html.
+CIBA stands for Client Initiated BackChannel Authentication and is standardised by the OpenID
+Fundation.
+https://openid.net/specs/openid-client-initiated-backchannel-
+authentication-core-1_0.html.
 """
 
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 from .pooling import TokenEndpointPoolingJob
 from .tokens import BearerToken
@@ -104,14 +106,15 @@
         ```
     """
 
     def __init__(
         self,
         client: "OAuth2Client",
         auth_req_id: Union[str, BackChannelAuthenticationResponse],
+        *,
         interval: Optional[int] = None,
         slow_down_interval: int = 5,
         requests_kwargs: Optional[Dict[str, Any]] = None,
         **token_kwargs: Any,
     ):
         if isinstance(auth_req_id, BackChannelAuthenticationResponse) and interval is None:
             interval = auth_req_id.interval
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/client.py` & `requests_oauth2client-1.2.0/requests_oauth2client/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 """This module contains the `OAuth2Client` class."""
+from __future__ import annotations
 
 from typing import Any, Dict, Iterable, Optional, Tuple, Type, Union
 
 import requests
 from jwskate import Jwk, JwkSet, Jwt
+from typing_extensions import Literal
 
 from .auth import BearerAuth
 from .authorization_request import (
     AuthorizationRequest,
     AuthorizationResponse,
     RequestUriParameterAuthorizationRequest,
 )
 from .backchannel_authentication import BackChannelAuthenticationResponse
-from .client_authentication import ClientSecretPost, client_auth_factory
+from .client_authentication import ClientSecretPost, PrivateKeyJwt, client_auth_factory
 from .device_authorization import DeviceAuthorizationResponse
+from .discovery import oidc_discovery_document_url
 from .exceptions import (
     AccessDenied,
     AuthorizationPending,
     BackChannelAuthenticationError,
     DeviceAuthorizationError,
     ExpiredToken,
     IntrospectionError,
     InvalidBackChannelAuthenticationResponse,
+    InvalidClient,
     InvalidDeviceAuthorizationResponse,
     InvalidGrant,
     InvalidPushedAuthorizationResponse,
+    InvalidRequest,
     InvalidScope,
     InvalidTarget,
     InvalidTokenResponse,
     RevocationError,
     ServerError,
     SlowDown,
     UnauthorizedClient,
@@ -37,130 +42,222 @@
     UnsupportedTokenType,
 )
 from .tokens import BearerToken, IdToken
 from .utils import validate_endpoint_uri
 
 
 class OAuth2Client:
-    """An OAuth 2.0 client, that can send requests to an OAuth 2.0 Authorization Server.
+    """An OAuth 2.x client, that can send requests to an OAuth 2.x Authorization Server.
 
-    `OAuth2Client` is able to obtain tokens from the Token Endpoint using one of the standardised Grant Types,
+    `OAuth2Client` is able to obtain tokens from the Token Endpoint using any of the standardised Grant Types,
     and to communicate with the various backend endpoints like the Revocation, Introspection, and UserInfo Endpoint.
 
-    This class doesn't implement anything related to the end-user authentication or any request that goes in a browser.
+    To init an OAuth2Client, you only need the url to the Token Endpoint and the Credentials that will be used to authenticate
+    to that endpoint. Other endpoint urls, such as the  can be passed as parameter as well if you intend to use them.
+
+
+    This class is not intended to help with the end-user authentication or any request that goes in a browser.
     For authentication requests, see [AuthorizationRequest][requests_oauth2client.authorization_request.AuthorizationRequest].
+    You may use the helper method `authorization_request()` to generate `AuthorizationRequest`s with the preconfigured
+    `authorization_endpoint`, `client_id` and `redirect_uri' from this client.
 
     Args:
         token_endpoint: the Token Endpoint URI where this client will get access tokens
         auth: the authentication handler to use for client authentication on the token endpoint. Can be a [requests.auth.AuthBase][] instance (which will be as-is), or a tuple of `(client_id, client_secret)` which will initialize an instance of [ClientSecretPost][requests_oauth2client.client_authentication.ClientSecretPost], a `(client_id, jwk)` to initialize a [PrivateKeyJwt][requests_oauth2client.client_authentication.PrivateKeyJwt], or a `client_id` which will use [PublicApp][requests_oauth2client.client_authentication.PublicApp] authentication.
+        client_id: client ID
+        client_secret: client secret
+        private_key: private_key to use for client authentication
         revocation_endpoint: the Revocation Endpoint URI to use for revoking tokens
         introspection_endpoint: the Introspection Endpoint URI to use to get info about tokens
         userinfo_endpoint: the Userinfo Endpoint URI to use to get information about the user
+        authorization_endpoint: the Authorization Endpoint URI for initializing Authorization Requests
+        redirect_uri: the redirect_uri for this client
         backchannel_authentication_endpoint: the BackChannel Authentication URI
         device_authorization_endpoint: the Device Authorization Endpoint URI to use to authorize devices
         jwks_uri: the JWKS URI to use to obtain the AS public keys
+        code_challenge_method: challenge method to use for PKCE (should always be 'S256')
         session: a requests Session to use when sending HTTP requests. Useful if some extra parameters such as proxy or client certificate must be used to connect to the AS.
-        extra_metadata: additional metadata for this client, unused by this class, but may be used by subclasses. Those will be accessible with the `extra_metadata` attribute.
+        **extra_metadata: additional metadata for this client, unused by this class, but may be used by subclasses. Those will be accessible with the `extra_metadata` attribute.
 
     Usage:
         ```python
         client = OAuth2Client(
             token_endpoint="https://my.as.local/token",
             revocation_endpoint="https://my.as.local/revoke",
             auth=("client_id", "client_secret"),
         )
 
-        # once intialized, a client can send requests to its configured endpoints
+        # once initialized, a client can send requests to its configured endpoints
         cc_token = client.client_credentials(scope="my_scope")
         ac_token = client.authorization_code(code="my_code")
         client.revoke_access_token(cc_token)
         ```
     """
 
     exception_classes: Dict[str, Type[Exception]] = {
         "server_error": ServerError,
+        "invalid_request": InvalidRequest,
+        "invalid_client": InvalidClient,
         "invalid_scope": InvalidScope,
         "invalid_target": InvalidTarget,
         "invalid_grant": InvalidGrant,
         "access_denied": AccessDenied,
         "unauthorized_client": UnauthorizedClient,
         "authorization_pending": AuthorizationPending,
         "slow_down": SlowDown,
         "expired_token": ExpiredToken,
         "unsupported_token_type": UnsupportedTokenType,
     }
 
+    token_class: Type[BearerToken] = BearerToken
+
     def __init__(
         self,
         token_endpoint: str,
         auth: Union[
             requests.auth.AuthBase,
             Tuple[str, str],
             Tuple[str, Jwk],
             Tuple[str, Dict[str, Any]],
             str,
-        ],
+            None,
+        ] = None,
         *,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
+        private_key: Union[Jwk, Dict[str, Any], None] = None,
         revocation_endpoint: Optional[str] = None,
         introspection_endpoint: Optional[str] = None,
         userinfo_endpoint: Optional[str] = None,
+        authorization_endpoint: Optional[str] = None,
+        redirect_uri: Optional[str] = None,
         backchannel_authentication_endpoint: Optional[str] = None,
         device_authorization_endpoint: Optional[str] = None,
         pushed_authorization_request_endpoint: Optional[str] = None,
         jwks_uri: Optional[str] = None,
+        authorization_server_jwks: Union[JwkSet, Dict[str, Any], None] = None,
+        issuer: Optional[str] = None,
+        id_token_signed_response_alg: Optional[str] = "RS256",
+        id_token_encrypted_response_alg: Optional[str] = None,
+        id_token_decryption_key: Union[Jwk, Dict[str, Any], None] = None,
+        code_challenge_method: str = "S256",
+        authorization_response_iss_parameter_supported: bool = False,
         session: Optional[requests.Session] = None,
         **extra_metadata: Any,
     ):
+        if authorization_response_iss_parameter_supported and not issuer:
+            raise ValueError(
+                "If the Authorization Server supports Issuer Identification, "
+                "as specified by `authorization_response_iss_parameter_supported=True`, "
+                "then you must specify the expected `issuer` value with parameter `issuer`."
+            )
         self.token_endpoint = str(token_endpoint)
         self.revocation_endpoint = str(revocation_endpoint) if revocation_endpoint else None
         self.introspection_endpoint = (
             str(introspection_endpoint) if introspection_endpoint else None
         )
         self.userinfo_endpoint = str(userinfo_endpoint) if userinfo_endpoint else None
+        self.authorization_endpoint = (
+            str(authorization_endpoint) if authorization_endpoint else None
+        )
+        self.redirect_uri = str(redirect_uri) if redirect_uri else None
         self.backchannel_authentication_endpoint = (
             str(backchannel_authentication_endpoint)
             if backchannel_authentication_endpoint
             else None
         )
         self.device_authorization_endpoint = (
             str(device_authorization_endpoint) if device_authorization_endpoint else None
         )
         self.pushed_authorization_request_endpoint = (
             str(pushed_authorization_request_endpoint)
             if pushed_authorization_request_endpoint
             else None
         )
         self.jwks_uri = str(jwks_uri) if jwks_uri else None
+        self.authorization_server_jwks = (
+            JwkSet(authorization_server_jwks) if authorization_server_jwks else None
+        )
+        self.issuer = str(issuer) if issuer else None
         self.session = session or requests.Session()
-        self.auth = client_auth_factory(auth, ClientSecretPost)
+        self.auth = client_auth_factory(
+            auth,
+            client_id=client_id,
+            client_secret=client_secret,
+            private_key=private_key,
+            default_auth_handler=ClientSecretPost,
+        )
+        self.id_token_signed_response_alg = id_token_signed_response_alg
+        self.id_token_encrypted_response_alg = id_token_encrypted_response_alg
+        self.id_token_decryption_key = (
+            Jwk(id_token_decryption_key) if id_token_decryption_key else None
+        )
+        self.code_challenge_method = code_challenge_method
+        self.authorization_response_iss_parameter_supported = (
+            authorization_response_iss_parameter_supported
+        )
         self.extra_metadata = extra_metadata
 
+    @property
+    def client_id(self) -> str:
+        """Client ID."""
+        if hasattr(self.auth, "client_id"):
+            return self.auth.client_id  # type: ignore[no-any-return]
+        raise AttributeError(  # pragma: no cover
+            "This client uses a custom authentication method without client_id."
+        )
+
+    @property
+    def client_secret(self) -> Optional[str]:
+        """Client Secret."""
+        if hasattr(self.auth, "client_secret"):
+            return self.auth.client_secret  # type: ignore[no-any-return]
+        return None
+
+    @property
+    def client_jwks(self) -> JwkSet:
+        """A `JwkSet` containing the public keys for this client.
+
+        Keys are:
+
+        - the public key for client assertion signature verification (if using private_key_jwt)
+        - the ID Token encryption key
+        """
+        jwks = JwkSet()
+        if isinstance(self.auth, PrivateKeyJwt):
+            jwks.add_jwk(self.auth.private_jwk.public_jwk().with_usage_parameters())
+        if self.id_token_decryption_key:
+            jwks.add_jwk(self.id_token_decryption_key.public_jwk().with_usage_parameters())
+        return jwks
+
     def token_request(
         self, data: Dict[str, Any], timeout: int = 10, **requests_kwargs: Any
     ) -> BearerToken:
         """Send a request to the token endpoint.
 
         Authentication will be added automatically based on the defined `auth` for this client.
 
         Args:
              data: parameters to send to the token endpoint. Items with a None or empty value will not be sent in the request.
              timeout: a timeout value for the call
              **requests_kwargs: additional parameters for requests.post()
 
         Returns:
-            the token endpoint response, as [BearerToken][requests_oauth2client.tokens.BearerToken] instance.
+            the token endpoint response, as [`BearerToken`][requests_oauth2client.tokens.BearerToken] instance.
         """
+        token_endpoint = self._require_endpoint("token_endpoint")
+
         requests_kwargs = {
             key: value
             for key, value in requests_kwargs.items()
             if value is not None and value != ""
         }
 
         response = self.session.post(
-            self.token_endpoint,
+            token_endpoint,
             auth=self.auth,
             data=data,
             timeout=timeout,
             **requests_kwargs,
         )
         if response.ok:
             return self.parse_token_response(response)
@@ -173,18 +270,18 @@
         Invoked by [token_request][requests_oauth2client.client.OAuth2Client.token_request] to parse responses returned by the Token Endpoint.
         Those response contain an `access_token` and additional attributes.
 
         Args:
             response: the [Response][requests.Response] returned by the Token Endpoint.
 
         Returns:
-            a [BearerToken][requests_oauth2client.tokens.BearerToken] based on the response contents.
+            a [`BearerToken`][requests_oauth2client.tokens.BearerToken] based on the response contents.
         """
         try:
-            token_response = BearerToken(**response.json())
+            token_response = self.token_class(**response.json())
             return token_response
         except Exception as response_class_exc:
             try:
                 return self.on_token_error(response)
             except Exception as token_error_exc:
                 raise token_error_exc from response_class_exc
 
@@ -193,28 +290,26 @@
 
         Invoked by [token_request][requests_oauth2client.client.OAuth2Client.token_request] when the Token Endpoint returns an error.
 
         Args:
             response: the [Response][requests.Response] returned by the Token Endpoint.
 
         Returns:
-            nothing, and raises an exception instead. But a subclass may return a [BearerToken][requests_oauth2client.tokens.BearerToken] to implement a default behaviour if needed.
+            nothing, and raises an exception instead. But a subclass may return a [`BearerToken`][requests_oauth2client.tokens.BearerToken] to implement a default behaviour if needed.
         """
-        error_json = response.json()
-        error = error_json.get("error")
-        error_description = error_json.get("error_description")
-        error_uri = error_json.get("error_uri")
-        if error:
+        try:
+            data = response.json()
+            error = data["error"]
+            error_description = data.get("error_description")
+            error_uri = data.get("error_uri")
             exception_class = self.exception_classes.get(error, UnknownTokenEndpointError)
-            raise exception_class(error, error_description, error_uri)
-        else:
-            raise InvalidTokenResponse(
-                "token endpoint returned an HTTP error without error message",
-                error_json,
-            )
+            exception = exception_class(response, error, error_description, error_uri)
+        except Exception as exc:
+            raise InvalidTokenResponse(response) from exc
+        raise exception
 
     def client_credentials(
         self,
         scope: Optional[Union[str, Iterable[str]]] = None,
         requests_kwargs: Optional[Dict[str, Any]] = None,
         **token_kwargs: Any,
     ) -> BearerToken:
@@ -239,56 +334,59 @@
 
         data = dict(grant_type="client_credentials", scope=scope, **token_kwargs)
         return self.token_request(data, **requests_kwargs)
 
     def authorization_code(
         self,
         code: Union[str, AuthorizationResponse],
+        validate: bool = True,
         requests_kwargs: Optional[Dict[str, Any]] = None,
         **token_kwargs: Any,
     ) -> BearerToken:
         """Send a request to the token endpoint with the `authorization_code` grant.
 
         Args:
-             code: an authorization code to exchange for tokens
+             code: an authorization code or an `AuthorizationResponse` to exchange for tokens
+             validate: if `True`, validate the received ID Token (this works only if `code` is an AuthorizationResponse)
              requests_kwargs: additional parameters for the call to requests
              **token_kwargs: additional parameters for the token endpoint, alongside `grant_type`, `code`, etc.
 
         Returns:
-            a BearerToken
+            a `BearerToken`
         """
+        azr: Optional[AuthorizationResponse] = None
         if isinstance(code, AuthorizationResponse):
-            if code.code is None or not isinstance(code.code, str):
-                raise ValueError(
-                    "This AuthorizationResponse doesn't contain an authorization code"
-                )
-            token_kwargs.setdefault("code_verifer", code.code_verifier)
+            token_kwargs.setdefault("code_verifier", code.code_verifier)
             token_kwargs.setdefault("redirect_uri", code.redirect_uri)
+            azr = code
             code = code.code
 
         requests_kwargs = requests_kwargs or {}
 
         data = dict(grant_type="authorization_code", code=code, **token_kwargs)
-        return self.token_request(data, **requests_kwargs)
+        token = self.token_request(data, **requests_kwargs)
+        if validate and token.id_token and isinstance(azr, AuthorizationResponse):
+            token.validate_id_token(self, azr)
+        return token
 
     def refresh_token(
         self,
         refresh_token: Union[str, BearerToken],
         requests_kwargs: Optional[Dict[str, Any]] = None,
         **token_kwargs: Any,
     ) -> BearerToken:
         """Send a request to the token endpoint with the `refresh_token` grant.
 
         Args:
-            refresh_token: a refresh_token, as a string, or as a BearerToken. That BearerToken must have a `refresh_token`.
+            refresh_token: a refresh_token, as a string, or as a `BearerToken`. That `BearerToken` must have a `refresh_token`.
             requests_kwargs: additional parameters for the call to `requests`
             **token_kwargs: additional parameters for the token endpoint, alongside `grant_type`, `refresh_token`, etc.
 
         Returns:
-            a BearerToken
+            a `BearerToken`
         """
         if isinstance(refresh_token, BearerToken):
             if refresh_token.refresh_token is None or not isinstance(
                 refresh_token.refresh_token, str
             ):
                 raise ValueError("This BearerToken doesn't have a refresh_token")
             refresh_token = refresh_token.refresh_token
@@ -305,20 +403,20 @@
     ) -> BearerToken:
         """Send a request to the token endpoint using the Device Code grant.
 
         The grant_type is `urn:ietf:params:oauth:grant-type:device_code`.
         This needs a Device Code, or a `DeviceAuthorizationResponse` as parameter.
 
         Args:
-            device_code: a device code, as received during the Device Authorization request
+            device_code: a device code, or a `DeviceAuthorizationResponse`
             requests_kwargs: additional parameters for the call to requests
             **token_kwargs: additional parameters for the token endpoint, alongside `grant_type`, `device_code`, etc.
 
         Returns:
-            a BearerToken
+            a `BearerToken`
         """
         if isinstance(device_code, DeviceAuthorizationResponse):
             if device_code.device_code is None or not isinstance(device_code.device_code, str):
                 raise ValueError("This DeviceAuthorizationResponse doesn't have a device_code")
             device_code = device_code.device_code
 
         requests_kwargs = requests_kwargs or {}
@@ -341,15 +439,15 @@
 
         Args:
             auth_req_id: an authentication request ID, as returned by the AS
             requests_kwargs: additional parameters for the call to requests
             **token_kwargs: additional parameters for the token endpoint, alongside `grant_type`, `auth_req_id`, etc.
 
         Returns:
-            a BearerToken
+            a `BearerToken`
         """
         if isinstance(auth_req_id, BackChannelAuthenticationResponse):
             if auth_req_id.auth_req_id is None or not isinstance(auth_req_id.auth_req_id, str):
                 raise ValueError(
                     "This BackChannelAuthenticationResponse doesn't have an auth_req_id"
                 )
             auth_req_id = auth_req_id.auth_req_id
@@ -384,15 +482,15 @@
             actor_token_type: a token type identifier for the actor_token, mandatory if it cannot be guessed based
                 on `type(actor_token)`.
             requested_token_type: a token type identifier for the requested token.
             requests_kwargs: additional parameters to pass to the underlying `requests.post()` call.
             **token_kwargs: additional parameters to include in the request body.
 
         Returns:
-            a BearerToken as returned by the Authorization Server.
+            a `BearerToken` as returned by the Authorization Server.
         """
         requests_kwargs = requests_kwargs or {}
 
         try:
             subject_token_type = self.get_token_type(subject_token_type, subject_token)
         except ValueError:
             raise TypeError(
@@ -415,35 +513,146 @@
             actor_token=actor_token,
             actor_token_type=actor_token_type,
             requested_token_type=requested_token_type,
             **token_kwargs,
         )
         return self.token_request(data, **requests_kwargs)
 
+    def jwt_bearer(
+        self,
+        assertion: Union[Jwt, str],
+        requests_kwargs: Optional[Dict[str, Any]] = None,
+        **token_kwargs: Any,
+    ) -> BearerToken:
+        """Send a request using a JWT as authorization grant.
+
+        This is a defined in (RFC7523 $2.1)[https://www.rfc-editor.org/rfc/rfc7523.html#section-2.1).
+
+        Args:
+            assertion: a JWT (as an instance of `jwskate.Jwt` or as a `str`) to use as authorization grant.
+            requests_kwargs: additional parameters to pass to the underlying `requests.post()` call.
+            **token_kwargs: additional parameters to include in the request body.
+
+        Returns:
+            a `BearerToken` as returned by the Authorization Server.
+        """
+        requests_kwargs = requests_kwargs or {}
+
+        if not isinstance(assertion, Jwt):
+            assertion = Jwt(assertion)
+
+        data = dict(
+            grant_type="urn:ietf:params:oauth:grant-type:jwt-bearer",
+            assertion=assertion,
+            **token_kwargs,
+        )
+
+        return self.token_request(data, **requests_kwargs)
+
+    def resource_owner_password(
+        self,
+        username: str,
+        password: str,
+        requests_kwargs: Optional[Dict[str, Any]] = None,
+        **token_kwargs: Any,
+    ) -> BearerToken:
+        """Send a request using the Resource Owner Password Grant.
+
+        This Grant Type is deprecated and should only be used when there is no other choice.
+
+        Args:
+            username: the resource owner user name
+            password: the resource owner password
+            requests_kwargs: additional parameters to pass to the underlying `requests.post()` call.
+            **token_kwargs: additional parameters to include in the request body.
+
+        Returns:
+            a `BearerToken` as returned by the Authorization Server
+        """
+        requests_kwargs = requests_kwargs or {}
+        data = dict(
+            grant_type="password",
+            username=username,
+            password=password,
+            **token_kwargs,
+        )
+
+        return self.token_request(data, **requests_kwargs)
+
+    def authorization_request(
+        self,
+        scope: Union[None, str, Iterable[str]] = "openid",
+        response_type: str = "code",
+        redirect_uri: Optional[str] = None,
+        state: Union[str, Literal[True], None] = True,
+        nonce: Union[str, Literal[True], None] = True,
+        code_verifier: Optional[str] = None,
+        **kwargs: Any,
+    ) -> AuthorizationRequest:
+        """Generate an Authorization Request for this client.
+
+        Args:
+            scope: the scope to use
+            response_type: the response_type to use
+            redirect_uri: the redirect_uri to include in the request. By default, the redirect_uri defined at init time is used.
+            state: the state parameter to use. Leave default to generate a random value.
+            nonce: a nonce. Leave default to generate a random value.
+            code_verifier: the PKCE code verifier to use. Leave default to generate a random value.
+            **kwargs: additional parameters to include in the auth request
+
+        Returns:
+            an AuthorizationRequest with the supplied parameters
+        """
+        authorization_endpoint = self._require_endpoint("authorization_endpoint")
+
+        redirect_uri = redirect_uri or self.redirect_uri
+        if not redirect_uri:
+            raise AttributeError(
+                "No 'redirect_uri' defined for this client. "
+                "You must either pass a redirect_uri as parameter to this method, "
+                "or include a redirect_uri when initializing your OAuth2Client."
+            )
+
+        if response_type != "code":
+            raise ValueError("Only response_type=code is supported.")
+
+        return AuthorizationRequest(
+            authorization_endpoint=authorization_endpoint,
+            client_id=self.client_id,
+            redirect_uri=redirect_uri,
+            issuer=self.issuer,
+            response_type=response_type,
+            scope=scope,
+            state=state,
+            nonce=nonce,
+            code_verifier=code_verifier,
+            code_challenge_method=self.code_challenge_method,
+            **kwargs,
+        )
+
     def pushed_authorization_request(
         self, authorization_request: AuthorizationRequest
     ) -> RequestUriParameterAuthorizationRequest:
         """Send a Pushed Authorization Request.
 
         This sends a request to the Pushed Authorization Request Endpoint, and returns a
         `RequestUriParameterAuthorizationRequest` initialized with the AS response.
 
         Args:
             authorization_request: the authorization request to send
 
         Returns:
-            the RequestUriParameterAuthorizationRequest initialized based on the AS response
+            the `RequestUriParameterAuthorizationRequest` initialized based on the AS response
         """
-        if not self.pushed_authorization_request_endpoint:
-            raise AttributeError(
-                "No 'pushed_authorization_request_endpoint' defined for this client."
-            )
+        pushed_authorization_request_endpoint = self._require_endpoint(
+            "pushed_authorization_request_endpoint"
+        )
 
         response = self.session.post(
-            self.pushed_authorization_request_endpoint,
+            pushed_authorization_request_endpoint,
             data=authorization_request.args,
             auth=self.auth,
         )
         if not response.ok:
             return self.on_pushed_authorization_request_error(response)
 
         response_json = response.json()
@@ -469,42 +678,38 @@
             a RequestUriParameterAuthorizationRequest, if the error is recoverable
 
         Raises:
             EndpointError: a subclass of this error depending on the error returned by the AS
             InvalidPushedAuthorizationResponse: if the returned response is not following the specifications
             UnknownTokenEndpointError: for unknown/unhandled errors
         """
-        error_json = response.json()
-        error = error_json.get("error")
-        error_description = error_json.get("error_description")
-        error_uri = error_json.get("error_uri")
-        if error:
+        try:
+            data = response.json()
+            error = data["error"]
+            error_description = data.get("error_description")
+            error_uri = data.get("error_uri")
             exception_class = self.exception_classes.get(error, UnknownTokenEndpointError)
-            raise exception_class(error, error_description, error_uri)
-        else:
-            raise InvalidPushedAuthorizationResponse(
-                "pushed authorization endpoint returned an HTTP error without error message",
-                error_json,
-            )
+            exception = exception_class(response, error, error_description, error_uri)
+        except Exception as exc:
+            raise InvalidPushedAuthorizationResponse(response) from exc
+        raise exception
 
     def userinfo(self, access_token: Union[BearerToken, str]) -> Any:
         """Call the UserInfo endpoint.
 
         This sends a request to the UserInfo endpoint, with the specified access_token, and returns the parsed result.
 
         Args:
             access_token: the access token to use
 
         Returns:
             the [Response][requests.Response] returned by the userinfo endpoint.
         """
-        if not self.userinfo_endpoint:
-            raise AttributeError("No userinfo_endpoint defined for this client")
-
-        response = self.session.post(self.userinfo_endpoint, auth=BearerAuth(access_token))
+        userinfo_endpoint = self._require_endpoint("userinfo_endpoint")
+        response = self.session.post(userinfo_endpoint, auth=BearerAuth(access_token))
         return self.parse_userinfo_response(response)
 
     def parse_userinfo_response(self, resp: requests.Response) -> Any:
         """Parse the response obtained by `userinfo()`.
 
         Invoked by [userinfo()][requests_oauth2client.client.OAuth2Client.userinfo] to parse the response from the UserInfo endpoint, this will extract and return its JSON
         content.
@@ -526,15 +731,15 @@
         """Get standardised token type identifiers.
 
         Return a standardised token type identifier, based on a short `token_type`
         hint and/or a token value.
 
         Args:
             token_type: a token_type hint, as `str`. May be "access_token", "refresh_token" or "id_token" (optional)
-            token: a token value, as an instance of BearerToken or IdToken, or as a `str`.
+            token: a token value, as an instance of `BearerToken` or IdToken, or as a `str`.
 
         Returns:
             the token_type as defined in the Token Exchange RFC8693.
         """
         if not (token_type or token):
             raise ValueError(
                 "Cannot determine type of an empty token without a token_type hint"
@@ -683,23 +888,22 @@
             response: the [Response][requests.Response] as returned by the Revocation Endpoint
 
         Returns:
             `False` to signal that an error occurred. May raise exceptions instead depending on the revocation response.
         """
         try:
             data = response.json()
-        except ValueError:
-            return False
-        error = data.get("error")
-        error_description = data.get("error_description")
-        error_uri = data.get("error_uri")
-        if error is not None:
+            error = data["error"]
+            error_description = data.get("error_description")
+            error_uri = data.get("error_uri")
             exception_class = self.exception_classes.get(error, RevocationError)
-            raise exception_class(error, error_description, error_uri)
-        return False
+            exception = exception_class(error, error_description, error_uri)
+        except Exception:
+            return False
+        raise exception
 
     def introspect_token(
         self,
         token: Union[str, BearerToken],
         token_type_hint: Optional[str] = None,
         requests_kwargs: Optional[Dict[str, Any]] = None,
         **introspect_kwargs: Any,
@@ -710,30 +914,29 @@
             token_type_hint: the token_type_hint to include in the request.
             requests_kwargs: additional parameters to the underling call to requests.post()
             **introspect_kwargs: additional parameters to send to the introspection endpoint.
 
         Returns:
             the response as returned by the Introspection Endpoint.
         """
-        if not self.introspection_endpoint:
-            raise AttributeError("No introspection endpoint defined for this client")
+        introspection_endpoint = self._require_endpoint("introspection_endpoint")
 
         requests_kwargs = requests_kwargs or {}
 
         if token_type_hint == "refresh_token" and isinstance(token, BearerToken):
             if token.refresh_token is None:
                 raise ValueError("The supplied BearerToken doesn't have a refresh token.")
             token = token.refresh_token
 
         data = dict(introspect_kwargs, token=str(token))
         if token_type_hint:
             data["token_type_hint"] = token_type_hint
 
         response = self.session.post(
-            self.introspection_endpoint,
+            introspection_endpoint,
             data=data,
             auth=self.auth,
             **requests_kwargs,
         )
         if response.ok:
             return self.parse_introspection_response(response)
 
@@ -765,26 +968,22 @@
             response: the response as returned by the Introspection Endpoint.
 
         Returns:
             usually raises exeptions. A subclass can return a default response instead.
         """
         try:
             data = response.json()
-        except ValueError:
-            try:
-                response.raise_for_status()
-            except Exception as exc:
-                raise UnknownIntrospectionError(response) from exc
-        error = data.get("error")
-        error_description = data.get("error_description")
-        error_uri = data.get("error_uri")
-        if error is not None:
+            error = data["error"]
+            error_description = data.get("error_description")
+            error_uri = data.get("error_uri")
             exception_class = self.exception_classes.get(error, IntrospectionError)
-            raise exception_class(error, error_description, error_uri)
-        raise UnknownIntrospectionError(response)
+            exception = exception_class(error, error_description, error_uri)
+        except Exception as exc:
+            raise UnknownIntrospectionError(response) from exc
+        raise exception
 
     def backchannel_authentication_request(
         self,
         scope: Union[None, str, Iterable[str]] = "openid",
         client_notification_token: Optional[str] = None,
         acr_values: Union[None, str, Iterable[str]] = None,
         login_hint_token: Optional[str] = None,
@@ -814,18 +1013,17 @@
              alg: the alg to use to sign the request, if the provided JWK does not include an "alg" parameter.
              requests_kwargs: additional parameters for
              **ciba_kwargs: additional parameters to include in the request.
 
         Returns:
             a BackChannelAuthenticationResponse as returned by AS
         """
-        if not self.backchannel_authentication_endpoint:
-            raise AttributeError(
-                "No backchannel authentication endpoint defined for this client"
-            )
+        backchannel_authentication_endpoint = self._require_endpoint(
+            "backchannel_authentication_endpoint"
+        )
 
         if not (login_hint or login_hint_token or id_token_hint):
             raise ValueError(
                 "One of `login_hint`, `login_hint_token` or `ìd_token_hint` must be provided"
             )
 
         if (
@@ -861,18 +1059,18 @@
             login_hint=login_hint,
             binding_message=binding_message,
             user_code=user_code,
             requested_expiry=requested_expiry,
         )
 
         if private_jwk is not None:
-            data = {"request": str(Jwt.sign(data, jwk=private_jwk, alg=alg))}
+            data = {"request": str(Jwt.sign(data, key=private_jwk, alg=alg))}
 
         response = self.session.post(
-            self.backchannel_authentication_endpoint,
+            backchannel_authentication_endpoint,
             data=data,
             auth=self.auth,
             **requests_kwargs,
         )
 
         if response.ok:
             return self.parse_backchannel_authentication_response(response)
@@ -909,42 +1107,36 @@
         Args:
             response: the response returned by the BackChannel Authentication Endpoint.
 
         Returns:
             usually raises an exception. But a subclass can return a default response instead.
         """
         try:
-            error_json = response.json()
-        except ValueError as exc:
-            raise InvalidBackChannelAuthenticationResponse(response) from exc
-
-        error = error_json.get("error")
-        error_description = error_json.get("error_description")
-        error_uri = error_json.get("error_uri")
-        if error:
+            data = response.json()
+            error = data["error"]
+            error_description = data.get("error_description")
+            error_uri = data.get("error_uri")
             exception_class = self.exception_classes.get(error, BackChannelAuthenticationError)
-            raise exception_class(error, error_description, error_uri)
-
-        raise InvalidBackChannelAuthenticationResponse(response)
+            exception = exception_class(error, error_description, error_uri)
+        except Exception as exc:
+            raise InvalidBackChannelAuthenticationResponse(response) from exc
+        raise exception
 
     def authorize_device(self, **data: Any) -> DeviceAuthorizationResponse:
         """Send a Device Authorization Request.
 
         Args:
             **data: additional data to send to the Device Authorization Endpoint
 
         Returns:
             a Device Authorization Response
         """
-        if self.device_authorization_endpoint is None:
-            raise AttributeError("No device authorization endpoint defined for this client")
+        device_authorization_endpoint = self._require_endpoint("device_authorization_endpoint")
 
-        response = self.session.post(
-            self.device_authorization_endpoint, data=data, auth=self.auth
-        )
+        response = self.session.post(device_authorization_endpoint, data=data, auth=self.auth)
 
         if response.ok:
             return self.parse_device_authorization_response(response)
 
         return self.on_device_authorization_error(response)
 
     def parse_device_authorization_response(
@@ -972,110 +1164,198 @@
 
         Args:
             response: the response returned by the Device Authorization Endpoint.
 
         Returns:
             usually raises an Exception. But a subclass may return a default response instead.
         """
-        error_json = response.json()
-        error = error_json.get("error")
-        error_description = error_json.get("error_description")
-        error_uri = error_json.get("error_uri")
-        if error:
+        try:
+            data = response.json()
+            error = data["error"]
+            error_description = data.get("error_description")
+            error_uri = data.get("error_uri")
             exception_class = self.exception_classes.get(error, DeviceAuthorizationError)
-            raise exception_class(error, error_description, error_uri)
+            exception = exception_class(response, error, error_description, error_uri)
+        except Exception as exc:
+            raise InvalidDeviceAuthorizationResponse(response) from exc
+        raise exception
 
-        raise InvalidDeviceAuthorizationResponse(
-            "device authorization endpoint returned an HTTP error without an error message",
-            error_json,
-        )
+    def update_authorization_server_public_keys(self) -> JwkSet:
+        """Update the cached AS public keys by retrieving them from its `jwks_uri`.
 
-    def get_public_jwks(self) -> JwkSet:
-        """Fetch and parse the public keys from the JWKS endpoint.
+        Public keys are returned by this method, as a [JwkSet][jwskate.JwkSet].
+        They are also available in attribute `authorization_server_jwks`.
 
         Returns:
-            a JwkSet based on the retrieved keys.
+            the retrieved public keys
+
+        Raises:
+            ValueError: if no jwks_uri is configured
         """
-        if not self.jwks_uri:
-            raise ValueError("No jwks uri defined for this client")
-        jwks = self.session.get(self.jwks_uri, auth=None).json()
-        return JwkSet(jwks)
+        jwks_uri = self._require_endpoint("jwks_uri")
+
+        jwks = self.session.get(jwks_uri, auth=None).json()
+        self.authorization_server_jwks = JwkSet(jwks)
+        return self.authorization_server_jwks
 
     @classmethod
     def from_discovery_endpoint(
         cls,
-        url: str,
-        issuer: Optional[str],
-        auth: Union[requests.auth.AuthBase, Tuple[str, str], str],
+        url: Optional[str] = None,
+        issuer: Optional[str] = None,
+        auth: Union[requests.auth.AuthBase, Tuple[str, str], str, None] = None,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
+        private_key: Union[Jwk, Dict[str, Any], None] = None,
         session: Optional[requests.Session] = None,
-    ) -> "OAuth2Client":
+        **kwargs: Any,
+    ) -> OAuth2Client:
         """Initialise an OAuth2Client based on Authorization Server Metadata.
 
-        This will retrieve the standardised metadata document available at `url`, and will extract all Endpoint Uris from that document,
-        then will initialize an OAuth2Client based on those endpoint.
+        This will retrieve the standardised metadata document available at `url`, and will extract all Endpoint Uris
+        from that document, will fetch the current public keys from its `jwks_uri`, then will initialize an OAuth2Client
+        based on those endpoints.
 
         Args:
              url: the url where the server metadata will be retrieved
              auth: the authentication handler to use for client authentication
+             client_id: client ID
+             client_secret: client secret to use to authenticate the client
+             private_key: private key to sign client assertions
              session: a requests Session to use to retrieve the document and initialise the client with
              issuer: if an issuer is given, check that it matches the one from the retrieved document
 
         Returns:
             an OAuth2Client with endpoint initialized based on the obtained metadata
+
+        Raises:
+            ValueError: if neither `url` or `issuer` are suitable urls.
+            requests.HTTPError: if an error happens while fetching the documents
         """
+        if url is None and issuer is not None:
+            url = oidc_discovery_document_url(issuer)
+        if url is None:
+            raise ValueError("Please specify at least one of `issuer` or `url`")
+
+        validate_endpoint_uri(url, path=False)
+
         session = session or requests.Session()
         discovery = session.get(url).json()
 
-        return cls.from_discovery_document(discovery, issuer=issuer, auth=auth, session=session)
+        jwks_uri = discovery.get("jwks_uri")
+        if jwks_uri:
+            jwks = JwkSet(session.get(jwks_uri).json())
+
+        return cls.from_discovery_document(
+            discovery,
+            issuer=issuer,
+            auth=auth,
+            session=session,
+            client_id=client_id,
+            client_secret=client_secret,
+            private_key=private_key,
+            authorization_server_jwks=jwks,
+            **kwargs,
+        )
 
     @classmethod
     def from_discovery_document(
         cls,
         discovery: Dict[str, Any],
-        issuer: Optional[str],
-        auth: Union[requests.auth.AuthBase, Tuple[str, str], str],
+        issuer: Optional[str] = None,
+        auth: Union[requests.auth.AuthBase, Tuple[str, str], str, None] = None,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
+        private_key: Union[Jwk, Dict[str, Any], None] = None,
+        authorization_server_jwks: Union[JwkSet, Dict[str, Any], None] = None,
         session: Optional[requests.Session] = None,
         https: bool = True,
-    ) -> "OAuth2Client":
+        **kwargs: Any,
+    ) -> OAuth2Client:
         """Initialise an OAuth2Client, based on the server metadata from `discovery`.
 
         Args:
              discovery: a dict of server metadata, in the same format as retrieved from a discovery endpoint.
              issuer: if an issuer is given, check that it matches the one mentioned in the document
              auth: the authentication handler to use for client authentication
+             client_id: client ID
+             client_secret: client secret to use to authenticate the client
+             private_key: private key to sign client assertions
+             authorization_server_jwks: the current authorization server JWKS keys
              session: a requests Session to use to retrieve the document and initialise the client with
              https: if True, validates that urls in the discovery document use the https scheme
 
         Returns:
             an OAuth2Client
         """
-        if issuer:  # pragma: no branch
-            issuer_from_doc = discovery.get("issuer")
-            if issuer_from_doc != issuer:
-                raise ValueError("issuer mismatch!", issuer_from_doc)
+        if issuer and discovery.get("issuer") != issuer:
+            raise ValueError(
+                "Mismatching issuer value in discovery document: ",
+                issuer,
+                discovery.get("issuer"),
+            )
+        elif issuer is None:
+            issuer = discovery.get("issuer")
 
         token_endpoint = discovery.get("token_endpoint")
         if token_endpoint is None:
             raise ValueError("token_endpoint not found in that discovery document")
         validate_endpoint_uri(token_endpoint, https=https)
+        authorization_endpoint = discovery.get("authorization_endpoint")
+        if authorization_endpoint is not None:
+            validate_endpoint_uri(authorization_endpoint, https=https)
+        validate_endpoint_uri(token_endpoint, https=https)
         revocation_endpoint = discovery.get("revocation_endpoint")
         if revocation_endpoint is not None:
             validate_endpoint_uri(revocation_endpoint, https=https)
         introspection_endpoint = discovery.get("introspection_endpoint")
         if introspection_endpoint is not None:
             validate_endpoint_uri(introspection_endpoint, https=https)
         userinfo_endpoint = discovery.get("userinfo_endpoint")
         if userinfo_endpoint is not None:
             validate_endpoint_uri(userinfo_endpoint, https=https)
         jwks_uri = discovery.get("jwks_uri")
         if jwks_uri is not None:
             validate_endpoint_uri(userinfo_endpoint, https=https)
+        authorization_response_iss_parameter_supported = discovery.get(
+            "authorization_response_iss_parameter_supported", False
+        )
 
         return cls(
             token_endpoint=token_endpoint,
+            authorization_endpoint=authorization_endpoint,
             revocation_endpoint=revocation_endpoint,
             introspection_endpoint=introspection_endpoint,
             userinfo_endpoint=userinfo_endpoint,
             jwks_uri=jwks_uri,
+            authorization_server_jwks=authorization_server_jwks,
             auth=auth,
+            client_id=client_id,
+            client_secret=client_secret,
+            private_key=private_key,
             session=session,
+            issuer=issuer,
+            authorization_response_iss_parameter_supported=authorization_response_iss_parameter_supported,
+            **kwargs,
         )
+
+    def __enter__(self) -> OAuth2Client:
+        """Allow using OAuth2Client as a context-manager.
+
+        The Authorization Server public keys are retrieved on __enter__.
+        """
+        self.update_authorization_server_public_keys()
+        return self
+
+    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> bool:  # noqa: D105
+        return True
+
+    def _require_endpoint(self, endpoint: str) -> str:
+        """Check that a required endpoint url is set."""
+        url = getattr(self, endpoint, None)
+        if not url:
+            raise AttributeError(
+                f"No '{endpoint}' defined for this client. "
+                f"Please provide the URL for that endpoint when initializing your {self.__class__.__name__} instance."
+            )
+
+        return str(url)
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/client_authentication.py` & `requests_oauth2client-1.2.0/requests_oauth2client/client_authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """This modules implements OAuth 2.0 Client Authentication Methods.
 
-An OAuth 2.0 Client must authenticate to the AS whenever it sends a request to the Token
-Endpoint, by including appropriate credentials. This module contains helper classes and methods
-that implement the standardised and commonly used Client Authentication Methods.
+An OAuth 2.0 Client must authenticate to the AS whenever it sends a request to the Token Endpoint,
+by including appropriate credentials. This module contains helper classes and methods that implement
+the standardised and commonly used Client Authentication Methods.
 """
-
 from datetime import datetime
-from typing import Any, Callable, Dict, Tuple, Type, Union
+from typing import Any, Callable, Dict, Optional, Tuple, Type, Union
 from uuid import uuid4
 
 import furl  # type: ignore[import]
 import requests
 from binapy import BinaPy
 from jwskate import Jwk, Jwt, SymmetricJwk
 
 
 class BaseClientAuthenticationMethod(requests.auth.AuthBase):
     """Base class for all Client Authentication methods. This extends [requests.auth.AuthBase].
 
-    This base class only checks that requests are suitable to add Client Authentication
-    parameters to, and doesn't modify the request.
+    This base class only checks that requests are suitable to add Client Authentication parameters
+    to, and doesn't modify the request.
     """
 
+    def __init__(self, client_id: str):
+        self.client_id = str(client_id)
+
     def __call__(self, request: requests.PreparedRequest) -> requests.PreparedRequest:
         """Check that the request is suitable for Client Authentication.
 
         It checks:
         * that the method is `POST`
         * that the Content-Type is "application/x-www-form-urlencoded" or None
 
@@ -47,24 +49,24 @@
             )
         return request
 
 
 class ClientSecretBasic(BaseClientAuthenticationMethod):
     """Implement `client_secret_basic` authentication.
 
-    With this method, the client sends its Client ID and Secret, in the Auhtorization header, with the "Basic" scheme,
+    With this method, the client sends its Client ID and Secret, in the Authorization header, with the "Basic" scheme,
     in each authenticated request to the AS.
 
     Args:
         client_id: `client_id` to use.
         client_secret: `client_secret` to use.
     """
 
     def __init__(self, client_id: str, client_secret: str):
-        self.client_id = str(client_id)
+        super().__init__(client_id)
         self.client_secret = str(client_secret)
 
     def __call__(self, request: requests.PreparedRequest) -> requests.PreparedRequest:
         """Add the appropriate `Authorization` header in each request.
 
         The Authorization header is formatted as such:
         `Authorization: Basic BASE64('<client_id:client_secret>')`
@@ -90,15 +92,15 @@
 
     Args:
         client_id: `client_id` to use.
         client_secret: `client_secret` to use.
     """
 
     def __init__(self, client_id: str, client_secret: str) -> None:
-        self.client_id = str(client_id)
+        super().__init__(client_id)
         self.client_secret = str(client_secret)
 
     def __call__(self, request: requests.PreparedRequest) -> requests.PreparedRequest:
         """Add the `client_id` and `client_secret` parameters in the request body.
 
         Args:
             request: a [requests.PreparedRequest][].
@@ -117,23 +119,30 @@
     """Base class for assertion based client authentication methods.
 
     Args:
         client_id: the client_id to use
         alg: the alg to use to sign generated Client Assertions.
         lifetime: the lifetime to use for generated Client Assertions.
         jti_gen: a function to generate JWT Token Ids (`jti`) for generated Client Assertions.
+        aud: the audience value to use. If `None` (default), the endpoint URL will be used.
     """
 
     def __init__(
-        self, client_id: str, alg: str, lifetime: int, jti_gen: Callable[[], str]
+        self,
+        client_id: str,
+        alg: str,
+        lifetime: int,
+        jti_gen: Callable[[], str],
+        aud: Optional[str] = None,
     ) -> None:
-        self.client_id = str(client_id)
+        super().__init__(client_id)
         self.alg = alg
         self.lifetime = lifetime
         self.jti_gen = jti_gen
+        self.aud = aud
 
     def client_assertion(self, audience: str) -> str:
         """Generate a Client Assertion for a specific audience.
 
         Args:
             audience: the audience to use for the `aud` claim of the generated Client Assertion.
 
@@ -148,18 +157,18 @@
         Args:
             request: a [requests.PreparedRequest][].
 
         Returns:
             a [requests.PreparedRequest][] with the added `client_assertion` field.
         """
         request = super().__call__(request)
-        token_endpoint = request.url
-        assert token_endpoint is not None
+        audience = self.aud or request.url
+        assert audience is not None
         data = furl.Query(request.body)
-        client_assertion = self.client_assertion(token_endpoint)
+        client_assertion = self.client_assertion(audience)
         data.set(
             [
                 ("client_id", self.client_id),
                 ("client_assertion", client_assertion),
                 (
                     "client_assertion_type",
                     "urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
@@ -178,29 +187,31 @@
 
     Args:
         client_id: the `client_id` to use.
         client_secret: the `client_secret` to use to sign generated Client Assertions.
         alg: the alg to use to sign generated Client Assertions.
         lifetime: the lifetime to use for generated Client Assertions.
         jti_gen: a function to generate JWT Token Ids (`jti`) for generated Client Assertions.
+        aud: the audience value to use. If `None` (default), the endpoint URL will be used.
     """
 
     def __init__(
         self,
         client_id: str,
         client_secret: str,
         alg: str = "HS256",
         lifetime: int = 60,
         jti_gen: Callable[[], Any] = lambda: uuid4(),
+        aud: Optional[str] = None,
     ) -> None:
-        super().__init__(client_id, alg, lifetime, jti_gen)
+        super().__init__(client_id, alg, lifetime, jti_gen, aud)
         self.client_secret = str(client_secret)
 
     def client_assertion(self, audience: str) -> str:
-        """Generate a  symmetrically signed Client Assertion.
+        """Generate a symmetrically signed Client Assertion.
 
         Assertion is signed with the `client_secret` as key and the `alg` passed at init time.
 
         Args:
             audience: the audience to use for the generated Client Assertion.
 
         Returns:
@@ -217,15 +228,15 @@
                 "iss": self.client_id,
                 "sub": self.client_id,
                 "aud": audience,
                 "iat": iat,
                 "exp": exp,
                 "jti": jti,
             },
-            jwk=jwk,
+            key=jwk,
             alg=self.alg,
         )
         return str(jwt)
 
 
 class PrivateKeyJwt(ClientAssertionAuthenticationMethod):
     """Implement `private_key_jwt` client authentication method.
@@ -235,46 +246,50 @@
 
     Args:
         client_id: the `client_id` to use.
         private_jwk: the private JWK to use to sign generated Client Assertions.
         alg: the alg to use to sign generated Client Assertions.
         lifetime: the lifetime to use for generated Client Assertions.
         jti_gen: a function to generate JWT Token Ids (`jti`) for generated Client Assertions.
+        aud: the audience value to use. If `None` (default), the endpoint URL will be used.k
     """
 
     def __init__(
         self,
         client_id: str,
         private_jwk: Union[Jwk, Dict[str, Any]],
         alg: str = "RS256",
         lifetime: int = 60,
         jti_gen: Callable[[], Any] = lambda: uuid4(),
+        aud: Optional[str] = None,
     ) -> None:
         if not isinstance(private_jwk, Jwk):
             private_jwk = Jwk(private_jwk)
 
-        if not private_jwk.is_private or isinstance(private_jwk, SymmetricJwk):
-            raise ValueError("Asymmetric signing requires a private key")
+        if not private_jwk.is_private or private_jwk.is_symmetric:
+            raise ValueError(
+                "Private Key JWT client authentication method uses asymmetric signing thus requires a private key."
+            )
 
         alg = private_jwk.alg or alg
         if not alg:
             raise ValueError(
-                "Asymmetric signing requires an alg, either as part of the private JWK, or passed as parameter"
+                "An asymmetric signing alg is required, either as part of the private JWK, or passed as parameter."
             )
         kid = private_jwk.get("kid")
         if not kid:
             raise ValueError(
-                "Asymmetric signing requires a kid, either as part of the private JWK, or passed as parameter"
+                "Asymmetric signing requires the private JWK to have a Key ID (kid)."
             )
 
-        super().__init__(client_id, alg, lifetime, jti_gen)
+        super().__init__(client_id, alg, lifetime, jti_gen, aud)
         self.private_jwk = private_jwk
 
     def client_assertion(self, audience: str) -> str:
-        """Generate a Client Assertion, asymetrically signed with `private_jwk` as key.
+        """Generate a Client Assertion, asymmetrically signed with `private_jwk` as key.
 
         Args:
             audience: the audience to use for the generated Client Assertion.
 
         Returns:
             a Client Assertion.
         """
@@ -287,15 +302,15 @@
                 "iss": self.client_id,
                 "sub": self.client_id,
                 "aud": audience,
                 "iat": iat,
                 "exp": exp,
                 "jti": jti,
             },
-            jwk=self.private_jwk,
+            key=self.private_jwk,
             alg=self.alg,
         )
         return str(jwt)
 
 
 class PublicApp(BaseClientAuthenticationMethod):
     """Implement the `none` authentication method for public apps.
@@ -329,49 +344,68 @@
 def client_auth_factory(
     auth: Union[
         requests.auth.AuthBase,
         Tuple[str, str],
         Tuple[str, Jwk],
         Tuple[str, Dict[str, Any]],
         str,
+        None,
     ],
+    *,
+    client_id: Optional[str] = None,
+    client_secret: Optional[str] = None,
+    private_key: Union[Jwk, Dict[str, Any], None] = None,
     default_auth_handler: Union[
         Type[ClientSecretPost], Type[ClientSecretBasic], Type[ClientSecretJwt]
     ] = ClientSecretPost,
 ) -> requests.auth.AuthBase:
     """Initialize the appropriate Auth Handler based on the provided parameters.
 
     This initializes a `ClientAuthenticationMethod` subclass based on the provided parameters.
 
     Args:
-        auth: Can be a :class:`requests.auth.AuthBase` instance (which will be used directly), or a tuple
-            of (client_id, client_secret) which will initialize, by default, an instance of `default_auth_handler`,
-            a (client_id, jwk) to initialize a :class:`PrivateKeyJWK`, or a `client_id` which will use :class:`PublicApp`
-            authentication.
-        default_auth_handler: if auth is a tuple of two string, consider that they are a client_id and client_secret,
-            and initialize an instance of this class with those 2 parameters.
+        auth: can be:
+            - a `requests.auth.AuthBase` instance (which will be used directly)
+            - a tuple of (client_id, client_secret) which will be used to initialize an instance of `default_auth_handler`,
+            - a tuple of (client_id, jwk), used to initialize a `PrivateKeyJwk` (`jwk` being an instance of `jwskate.Jwk` or a `dict`),
+            - a `client_id`, as `str`,
+            - or `None`, to pass `client_id` and other credentials as dedicated parameters, see below.
+        client_id: the Client ID to use for this client
+        client_secret: the Client Secret to use for this client, if any (for clients using an authentication method based on a secret)
+        private_key: the private key to use for private_key_jwt authentication method
+        default_auth_handler: if a client_id and client_secret are provided, initialize an instance of this class with those 2 parameters.
+            You can choose between `ClientSecretBasic`, `ClientSecretPost`, or `ClientSecretJwt`.
 
     Returns:
         an Auth Handler that will manage client authentication to the AS Token Endpoint or other backend endpoints.
     """
-    if isinstance(auth, requests.auth.AuthBase):
+    if auth is not None and (
+        client_id is not None or client_secret is not None or private_key is not None
+    ):
+        raise ValueError(
+            "Please use either `auth` parameter to provide an authentication method, or use `client_id` and one of `client_secret` or `private_key`."
+        )
+
+    if isinstance(auth, str):
+        client_id = auth
+    elif isinstance(auth, requests.auth.AuthBase):
         return auth
     elif isinstance(auth, tuple) and len(auth) == 2:
         client_id, credential = auth
         if isinstance(credential, (Jwk, dict)):
-            private_jwk = credential
-            return PrivateKeyJwt(str(client_id), private_jwk)
+            private_key = credential
+        elif isinstance(credential, str):
+            client_secret = credential
         else:
-            return default_auth_handler(str(client_id), credential)
-    elif isinstance(auth, str):
-        client_id = auth
-        return PublicApp(client_id)
+            raise TypeError(
+                "This credential type is not supported:", type(credential), credential
+            )
+
+    if client_id is None:
+        raise ValueError("A client_id must be provided.")
+
+    if private_key is not None:
+        return PrivateKeyJwt(str(client_id), private_key)
+    elif client_secret is None:
+        return PublicApp(str(client_id))
     else:
-        raise ValueError(
-            """Parameter 'auth' is required to define the Authentication Method that this Client will use when sending requests to the Token Endpoint.
-'auth' can be:
-- an instance of a requests.auth.AuthBase subclass, including ClientSecretPost, ClientSecretBasic, ClientSecretJwt, PrivateKeyJwt, PublicApp,
-- a (client_id, client_secret) tuple, both as str, for ClientSecretPost,
-- a (client_id, private_key) tuple, with client_id as str and private_key as a dict in JWK format, for PrivateKeyJwt,
-- a client_id, as str, for PublicApp.
-"""
-        )
+        return default_auth_handler(str(client_id), str(client_secret))
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/device_authorization.py` & `requests_oauth2client-1.2.0/requests_oauth2client/device_authorization.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/discovery.py` & `requests_oauth2client-1.2.0/requests_oauth2client/discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/exceptions.py` & `requests_oauth2client-1.2.0/requests_oauth2client/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 """This module contains all exception classes from `requests_oauth2client`."""
+from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from jwskate import InvalidJwt
 
+if TYPE_CHECKING:
+    import requests
+
 
 class OAuth2Error(Exception):
-    """Base class for Exceptions raised by requests_oauth2client."""
+    """Base class for Exceptions raised when a backend endpoint returns an error.
+
+    Args:
+        response: the HTTP response containing the error
+    """
+
+    def __init__(self, response: requests.Response):
+        self.response = response
+
+    @property
+    def request(self) -> requests.PreparedRequest:
+        """The request leading to the error."""
+        return self.response.request
 
 
 class EndpointError(OAuth2Error):
-    """Base class for exceptions raised from the token endpoint errors.
+    """Base class for exceptions raised from backend endpoint errors.
 
-    An `EndpointError` contains the error message, description and uri that are returned by the AS in the OAuth 2.0 standardised way.
+    This contains the error message, description and uri that are returned by the AS in the OAuth 2.0 standardised way.
 
     Args:
-        error: the `error` identifier as returned by the AS
-        description: the `error_description` as returned by the AS
-        uri: the `error_uri` as returned by the AS
+        response: the raw requests.PreparedResponse containing the error.
+        error: the `error` identifier as returned by the AS.
+        description: the `error_description` as returned by the AS.
+        uri: the `error_uri` as returned by the AS.
     """
 
     def __init__(
-        self, error: str, description: Optional[str] = None, uri: Optional[str] = None
+        self,
+        response: requests.Response,
+        error: str,
+        description: Optional[str] = None,
+        uri: Optional[str] = None,
     ):
+        super().__init__(response)
         self.error = error
         self.description = description
         self.uri = uri
 
 
 class InvalidTokenResponse(OAuth2Error):
     """Raised when the Token Endpoint returns a non-standard response."""
 
 
-class ExpiredAccessToken(OAuth2Error):
+class ExpiredAccessToken(RuntimeError):
     """Raised when an expired access token is used."""
 
 
 class UnknownTokenEndpointError(EndpointError):
     """Raised when an otherwise unknown error is returned by the token endpoint."""
 
 
@@ -44,14 +66,22 @@
     """Raised when the token endpoint returns `error = server_error`."""
 
 
 class TokenEndpointError(EndpointError):
     """Base class for errors that are specific to the token endpoint."""
 
 
+class InvalidRequest(TokenEndpointError):
+    """Raised when the Token Endpoint returns `error = invalid_request`."""
+
+
+class InvalidClient(TokenEndpointError):
+    """Raised when the Token Endpoint returns `error = invalid_client`."""
+
+
 class InvalidScope(TokenEndpointError):
     """Raised when the Token Endpoint returns `error = invalid_scope`."""
 
 
 class InvalidTarget(TokenEndpointError):
     """Raised when the Token Endpoint returns `error = invalid_target`."""
 
@@ -77,15 +107,15 @@
 
 
 class IntrospectionError(EndpointError):
     """Base class for Introspection Endpoint errors."""
 
 
 class UnknownIntrospectionError(OAuth2Error):
-    """Raised when the Introspection Endpoint retuns a non-standard error."""
+    """Raised when the Introspection Endpoint returns a non-standard error."""
 
 
 class DeviceAuthorizationError(EndpointError):
     """Base class for Device Authorization Endpoint errors."""
 
 
 class AuthorizationPending(TokenEndpointError):
@@ -143,42 +173,92 @@
     """Raised when the Authorization Endpoint returns `error = session_selection_required`."""
 
 
 class ConsentRequired(InteractionRequired):
     """Raised when the Authorization Endpoint returns `error = consent_required`."""
 
 
-class InvalidAuthResponse(OAuth2Error):
+class InvalidAuthResponse(Exception):
     """Raised when the Authorization Endpoint returns an invalid response."""
 
 
 class MissingAuthCode(InvalidAuthResponse):
-    """Raised when the Authorization Endpoint does not return a `code`.
+    """Raised when the Authorization Endpoint does not return the mandatory `code`.
+
+    This happens when the Authorization Endpoint does not return an error, but does not return an
+    authorization `code` either.
+    """
+
+
+class MissingIssuer(InvalidAuthResponse):
+    """Raised when the Authorization Endpoint does not return an `iss` parameter as expected.
+
+    The Authorization Server advertises its support with a flag
+    `authorization_response_iss_parameter_supported` in its discovery document. If it is set to
+    `true`, it must include an `iss` parameter in its authorization responses, containing its issuer
+    identifier.
+    """
+
+
+class MissingIdToken(InvalidAuthResponse):
+    """Raised when the Authorization Endpoint does not return a mandatory ID Token.
 
-    This happens when the Authorization Endpoint does not return an error, but does not return
-    an authorization `code` either.
+    This happens when the Authorization Endpoint does not return an error, but does not return an ID
+    Token either.
     """
 
 
 class MismatchingState(InvalidAuthResponse):
     """Raised on mismatching `state` value.
 
-    This happens when the Authorization Endpoints returns a 'state' parameter that doesn't match
-    the value passed in the Authorization Request.
+    This happens when the Authorization Endpoints returns a 'state' parameter that doesn't match the
+    value passed in the Authorization Request.
     """
 
 
 class MismatchingIssuer(InvalidAuthResponse):
     """Raised on mismatching `iss` value.
 
-    This happens when the Authorization Endpoints returns an 'iss' that doesn't match the
-    expected value.
+    This happens when the Authorization Endpoints returns an 'iss' that doesn't match the expected
+    value.
+    """
+
+
+class MismatchingNonce(InvalidIdToken):
+    """Raised on mismatching `nonce` value in an ID Token.
+
+    This happens when the authorization request includes a `nonce` but the returned ID Token include
+    a different value.
     """
 
 
+class MismatchingAcr(InvalidIdToken):
+    """Raised when the returned ID Token doesn't contain one of the requested ACR Values.
+
+    This happens when the authorization request includes an `acr_values` parameter but the returned
+    ID Token includes a different value.
+    """
+
+
+class MismatchingAudience(InvalidIdToken):
+    """Raised when the ID Token audience does not include the requesting Client ID."""
+
+
+class MismatchingAzp(InvalidIdToken):
+    """Raised when the ID Token Authorized Presenter (azp) claim is not the Client ID."""
+
+
+class MismatchingIdTokenAlg(InvalidIdToken):
+    """Raised when the returned ID Token is signed with an unexpected alg."""
+
+
+class ExpiredIdToken(InvalidIdToken):
+    """Raised when the returned ID Token is expired."""
+
+
 class BackChannelAuthenticationError(EndpointError):
     """Base class for errors returned by the BackChannel Authentication endpoint."""
 
 
 class InvalidBackChannelAuthenticationResponse(OAuth2Error):
     """Raised when the BackChannel Authentication endpoint returns a non-standard response."""
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/flask/auth.py` & `requests_oauth2client-1.2.0/requests_oauth2client/flask/auth.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/pooling.py` & `requests_oauth2client-1.2.0/requests_oauth2client/pooling.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/utils.py` & `requests_oauth2client-1.2.0/requests_oauth2client/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Various utilities used in multiple places.
 
-This module contains helper methods that are used in multiple places within
-`requests_oauth2client`.
+This module contains helper methods that are used in multiple places within `requests_oauth2client`.
 """
 
 from datetime import datetime, timedelta
 from functools import wraps
 from typing import Any, Callable, Optional
 
 from furl import furl  # type: ignore[import]
```

### Comparing `requests_oauth2client-1.1.0/requests_oauth2client/vendor_specific/auth0.py` & `requests_oauth2client-1.2.0/requests_oauth2client/vendor_specific/auth0.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,35 +19,44 @@
         auth: the client credentials, same definition as for [OAuth2Client][requests_oauth2client.client.OAuth2Client]
         session: the session to use, same definition as for [OAuth2Client][requests_oauth2client.client.OAuth2Client]
     """
 
     def __init__(
         self,
         tenant: str,
-        auth: Union[requests.auth.AuthBase, Tuple[str, str], str],
+        auth: Union[requests.auth.AuthBase, Tuple[str, str], str, None] = None,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
         session: Optional[requests.Session] = None,
     ):
         if (
             "." not in tenant
             or tenant.endswith(".eu")
             or tenant.endswith(".us")
             or tenant.endswith(".au")
+            or tenant.endswith(".jp")
         ):
             tenant = f"{tenant}.auth0.com"
+        if "://" in tenant and not tenant.startswith("https://"):
+            raise ValueError(
+                "Invalid tenant name. It must be a tenant name like 'mytenant.myregion' or a full issuer like 'https://mytenant.myregion.auth0.com'."
+            )
         self.tenant = tenant
         token_endpoint = f"https://{tenant}/oauth/token"
         revocation_endpoint = f"https://{tenant}/oauth/revoke"
         userinfo_endpoint = f"https://{tenant}/userinfo"
         jwks_uri = f"https://{tenant}/.well-known/jwks.json"
         super().__init__(
             token_endpoint=token_endpoint,
             revocation_endpoint=revocation_endpoint,
             userinfo_endpoint=userinfo_endpoint,
             jwks_uri=jwks_uri,
             auth=auth,
+            client_id=client_id,
+            client_secret=client_secret,
             session=session,
         )
 
 
 class Auth0ManagementApiClient(ApiClient):
     """A wrapper around the Auth0 Management API.
 
@@ -66,19 +75,23 @@
         users = a0mgmt.get("users", params={"page": 0, "per_page": 100})
         ```
     """
 
     def __init__(
         self,
         tenant: str,
-        auth: Union[requests.auth.AuthBase, Tuple[str, str], str],
+        auth: Union[requests.auth.AuthBase, Tuple[str, str], str, None] = None,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
         session: Optional[requests.Session] = None,
         **kwargs: Any,
     ):
-        client = Auth0Client(tenant, auth, session=session)
+        client = Auth0Client(
+            tenant, auth=auth, client_id=client_id, client_secret=client_secret, session=session
+        )
         audience = f"https://{client.tenant}/api/v2/"
         api_auth = OAuth2ClientCredentialsAuth(client, audience=audience)
         super().__init__(
             base_url=audience,
             auth=api_auth,
             session=session,
             **kwargs,
```

### Comparing `requests_oauth2client-1.1.0/tests/.coveragerc` & `requests_oauth2client-1.2.0/tests/.coveragerc`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/tests/conftest.py` & `requests_oauth2client-1.2.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,24 @@
 
 
 @pytest.fixture(scope="session", params=["oidc/jwks", ".well-known/jwks.json"])
 def jwks_uri(request: FixtureRequest, issuer: str) -> str:
     return join_url(issuer, request.param)
 
 
+@pytest.fixture(scope="session")
+def as_private_jwks() -> JwkSet:
+    return Jwk.generate_for_alg("RS256").as_jwks()
+
+
+@pytest.fixture(scope="session")
+def as_public_jwks(as_private_jwks: JwkSet) -> JwkSet:
+    return as_private_jwks.public_jwks()
+
+
 @pytest.fixture(scope="session", params=["oauth/par"])
 def pushed_authorization_request_endpoint(request: FixtureRequest, issuer: str) -> str:
     return join_url(issuer, request.param)
 
 
 @pytest.fixture(scope="session")
 def client_id() -> str:
```

### Comparing `requests_oauth2client-1.1.0/tests/test_authorization_code.py` & `requests_oauth2client-1.2.0/tests/test_authorization_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,15 +82,17 @@
 
     access_token = secrets.token_urlsafe()
 
     requests_mock.post(
         token_endpoint,
         json={"access_token": access_token, "token_type": "Bearer", "expires_in": 3600},
     )
-    token = client.authorization_code(code=auth_response, redirect_uri=redirect_uri)
+    token = client.authorization_code(
+        code=auth_response, redirect_uri=redirect_uri, validate=False
+    )
 
     assert isinstance(token, BearerToken)
     assert token.access_token == access_token
     assert not token.is_expired()
     assert token.expires_at is not None
     assert (
         datetime.now() + timedelta(seconds=3598)
```

### Comparing `requests_oauth2client-1.1.0/tests/test_client_credentials.py` & `requests_oauth2client-1.2.0/tests/test_client_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     requests_mock: Mocker,
     access_token: str,
     token_endpoint: str,
     client_id: str,
     client_secret: str,
     target_api: str,
 ) -> None:
-
     client = OAuth2Client(token_endpoint, ClientSecretPost(client_id, client_secret))
     auth = OAuth2ClientCredentialsAuth(client)
 
     requests_mock.post(
         token_endpoint,
         json={"access_token": access_token, "token_type": "Bearer", "expires_in": 3600},
     )
```

### Comparing `requests_oauth2client-1.1.0/tests/test_device_authorization.py` & `requests_oauth2client-1.2.0/tests/test_device_authorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,14 @@
 def test_invalid_response(
     requests_mock: Mocker,
     token_endpoint: str,
     device_authorization_endpoint: str,
     client_id: str,
     client_secret: str,
 ) -> None:
-
     da_client = OAuth2Client(
         token_endpoint=token_endpoint,
         device_authorization_endpoint=device_authorization_endpoint,
         auth=(client_id, client_secret),
     )
 
     requests_mock.post(
```

### Comparing `requests_oauth2client-1.1.0/tests/test_refresh_token.py` & `requests_oauth2client-1.2.0/tests/test_refresh_token.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/tests/test_token_exchange.py` & `requests_oauth2client-1.2.0/tests/test_token_exchange.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/conftest.py` & `requests_oauth2client-1.2.0/tests/unit_tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import hashlib
 from typing import Any, Dict, List, Optional, Type, Union
 
 import pytest
 import requests
 from furl import furl  # type: ignore[import]
 from jwskate import Jwk
+from typing_extensions import Literal
 
 from requests_oauth2client import (
     ApiClient,
     AuthorizationRequest,
+    AuthorizationResponse,
     BearerAuth,
     ClientSecretBasic,
     ClientSecretJwt,
     ClientSecretPost,
     OAuth2Client,
     PrivateKeyJwt,
     PublicApp,
@@ -114,15 +116,15 @@
 @pytest.fixture(
     scope="session",
     params=[PublicApp, ClientSecretPost, ClientSecretBasic, ClientSecretJwt],
 )
 def client_auth_method_handler(
     request: pytest.FixtureRequest,
 ) -> Type[BaseClientAuthenticationMethod]:
-    return request.param  # type: ignore[attr-defined,no-any-return]
+    return request.param  # type: ignore[no-any-return]
 
 
 @pytest.fixture(scope="session")
 def kid() -> str:
     return "JWK-ABCD"
 
 
@@ -272,67 +274,90 @@
         "jwks_uri": jwks_uri,
     }
 
 
 @pytest.fixture(scope="session")
 def oauth2client(
     token_endpoint: str,
+    authorization_endpoint: str,
+    redirect_uri: str,
+    expected_issuer: str,
     revocation_endpoint: str,
     introspection_endpoint: str,
     userinfo_endpoint: str,
     pushed_authorization_request_endpoint: str,
     jwks_uri: str,
     client_auth_method: BaseClientAuthenticationMethod,
+    client_id: str,
+    client_secret: str,
 ) -> OAuth2Client:
-    return OAuth2Client(
-        token_endpoint,
+    client = OAuth2Client(
+        token_endpoint=token_endpoint,
+        authorization_endpoint=authorization_endpoint,
+        redirect_uri=redirect_uri,
+        issuer=expected_issuer,
         revocation_endpoint=revocation_endpoint,
         introspection_endpoint=introspection_endpoint,
         userinfo_endpoint=userinfo_endpoint,
         pushed_authorization_request_endpoint=pushed_authorization_request_endpoint,
         jwks_uri=jwks_uri,
         auth=client_auth_method,
     )
+    assert client.token_endpoint == token_endpoint
+    assert client.authorization_endpoint == authorization_endpoint
+    assert client.revocation_endpoint == revocation_endpoint
+    assert client.introspection_endpoint == introspection_endpoint
+    assert client.userinfo_endpoint == userinfo_endpoint
+    assert client.pushed_authorization_request_endpoint == pushed_authorization_request_endpoint
+    assert client.jwks_uri == jwks_uri
+    assert client.auth == client_auth_method
+    assert client.client_id == client_id
+    if not isinstance(client_auth_method, PublicApp):
+        assert client.client_secret == client_secret
+    else:
+        assert client.client_secret is None
+
+    return client
 
 
 @pytest.fixture(scope="session")
 def sub() -> str:
     return "abcdefghijklmnopqrstuvwxyz"
 
 
 @pytest.fixture(
     scope="session",
     params=[None, "state", True],
 )
-def state(request: FixtureRequest) -> Union[None, bool, str]:
+def state(request: FixtureRequest) -> Union[None, Literal[True], str]:
     return request.param
 
 
-@pytest.fixture(scope="session", params=[None, "https://myas.local", False])
+@pytest.fixture(scope="session", params=[None, "https://myas.local"])
 def expected_issuer(request: FixtureRequest) -> Optional[str]:
     return request.param
 
 
 @pytest.fixture(scope="session", params=[None, {"foo": "bar"}])
 def auth_request_kwargs(request: FixtureRequest) -> Dict[str, Any]:
     return request.param or {}  # type: ignore[return-value]
 
 
 @pytest.fixture(
     scope="session",
-    params=[None, "nonce", False],
+    params=[None, "nonce", True],
 )
 def nonce(request: FixtureRequest) -> Union[None, bool, str]:
     return request.param
 
 
 @pytest.fixture(
     scope="session",
-    params=[None, "openid", "openid profile email", ["openid", "profile", "email"], []],
-    ids=["None", "single", "space-separated", "list", "empty-list"],
+    params=[None, "openid", "openid profile email", ("openid", "profile", "email"), ()],
+    ids=["None", "single", "space-separated", "tuple", "empty"],
 )
 def scope(request: FixtureRequest) -> Union[None, str, List[str]]:
     return request.param
 
 
 @pytest.fixture(
     scope="session",
@@ -351,30 +376,33 @@
 @pytest.fixture(scope="session")
 @pytest.mark.slow
 def authorization_request(
     authorization_endpoint: str,
     client_id: str,
     redirect_uri: str,
     scope: Union[None, str, List[str]],
-    state: Union[None, bool, str],
-    nonce: Union[None, bool, str],
+    state: Union[None, Literal[True], str],
+    nonce: Union[None, Literal[True], str],
     code_verifier: str,
     code_challenge_method: str,
-    expected_issuer: Union[str, bool, None],
+    expected_issuer: Union[str, None],
     auth_request_kwargs: Dict[str, Any],
 ) -> AuthorizationRequest:
+    authorization_response_iss_parameter_supported = True if expected_issuer else False
+
     azr = AuthorizationRequest(
         authorization_endpoint=authorization_endpoint,
         client_id=client_id,
         redirect_uri=redirect_uri,
         scope=scope,
         state=state,
         nonce=nonce,
         code_verifier=code_verifier,
         code_challenge_method=code_challenge_method,
+        authorization_response_iss_parameter_supported=authorization_response_iss_parameter_supported,
         issuer=expected_issuer,
         **auth_request_kwargs,
     )
 
     url = furl(str(azr))
     assert url.origin + str(url.path) == authorization_endpoint
 
@@ -390,50 +418,51 @@
         redirect_uri=redirect_uri,
         response_type="code",
         scope=scope,
         **auth_request_kwargs,
     )
 
     if nonce is True:
-        generated_nonce = args.pop("nonce")
-        assert isinstance(generated_nonce, str)
-        assert len(generated_nonce) > 20
-        assert azr.nonce == generated_nonce
-    elif nonce is False or nonce is None:
+        if scope is not None and "openid" in scope:
+            generated_nonce = args.pop("nonce")
+            assert isinstance(generated_nonce, str)
+            assert len(generated_nonce) > 20
+            assert azr.nonce == generated_nonce
+        else:
+            assert "nonce" not in args
+    elif nonce is None:
         assert azr.nonce is None
         assert "nonce" not in args
     elif isinstance(nonce, str):
         assert azr.nonce == nonce
         assert args.pop("nonce") == nonce
     else:
         assert False
 
     if state is True:
         generated_state = args.pop("state")
         assert isinstance(generated_state, str)
         assert len(generated_state) > 20
         assert azr.state == generated_state
-    elif state is False:
+    elif state is None:
         assert "state" not in args
         assert azr.state is None
     elif isinstance(state, str):
         assert args.pop("state") == state
         assert azr.state == state
 
     if scope is None:
         assert azr.scope is None
         assert "scope" not in args
         del expected_args["scope"]
-    elif isinstance(scope, list):
-        joined_scope = " ".join(scope)
-        expected_args["scope"] = joined_scope
-        assert azr.scope == joined_scope
-    if isinstance(scope, str):
-        expected_args["scope"] = scope
+    elif isinstance(scope, tuple):
+        expected_args["scope"] = " ".join(scope)
         assert azr.scope == scope
+    elif isinstance(scope, str):
+        assert azr.scope == scope.split()
 
     if code_challenge_method is None:
         assert "code_challenge_method" not in args
         assert "code_challenge" not in args
         assert azr.code_challenge_method is None
         assert azr.code_verifier is None
         assert azr.code_challenge is None
@@ -464,7 +493,40 @@
         else:
             assert generated_code_challenge == code_verifier
             assert azr.code_verifier == code_verifier
 
     assert args == expected_args
 
     return azr
+
+
+@pytest.fixture()
+def authorization_response_uri(
+    authorization_request: AuthorizationRequest,
+    redirect_uri: str,
+    authorization_code: str,
+    expected_issuer: Union[str, bool, None],
+) -> furl:
+    auth_url = furl(redirect_uri).add(args={"code": authorization_code})
+    if authorization_request.state is not None:
+        auth_url.add(args={"state": authorization_request.state})
+    if expected_issuer:
+        auth_url.add(args={"iss": expected_issuer})
+
+    return auth_url
+
+
+@pytest.fixture()
+def authorization_response(
+    authorization_request: AuthorizationRequest,
+    authorization_response_uri: furl,
+    redirect_uri: str,
+    authorization_code: str,
+) -> AuthorizationResponse:
+    auth_response = authorization_request.validate_callback(authorization_response_uri)
+    assert isinstance(auth_response, AuthorizationResponse)
+    assert auth_response.code == authorization_code
+    assert auth_response.state == authorization_request.state
+    assert auth_response.redirect_uri == redirect_uri
+    assert auth_response.code_verifier == authorization_request.code_verifier
+
+    return auth_response
```

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_api_client.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_auth.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,14 @@
     token_endpoint: str,
     client_id: str,
     client_secret: str,
     authorization_code: str,
     access_token: str,
     refresh_token: str,
 ) -> None:
-
     client = OAuth2Client(token_endpoint, (client_id, client_secret))
     auth = OAuth2AuthorizationCodeAuth(client, authorization_code)
 
     requests_mock.post(target_api)
     requests_mock.post(
         token_endpoint,
         json={
@@ -159,15 +158,14 @@
     device_code: str,
     user_code: str,
     verification_uri: str,
     verification_uri_complete: str,
     access_token: str,
     refresh_token: str,
 ) -> None:
-
     oauth2client = OAuth2Client(
         token_endpoint=token_endpoint,
         device_authorization_endpoint=device_authorization_endpoint,
         auth=(client_id, client_secret),
     )
     requests_mock.post(
         device_authorization_endpoint,
```

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_auth0.py` & `requests_oauth2client-1.2.0/tests/unit_tests/vendor_specific/test_auth0.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from requests_oauth2client import OAuth2ClientCredentialsAuth
 from requests_oauth2client.vendor_specific import Auth0Client, Auth0ManagementApiClient
 
 
 def test_auth0_management() -> None:
     auth0api = Auth0ManagementApiClient("test.eu.auth0.com", ("client_id", "client_secret"))
     assert auth0api.session.auth is not None
@@ -25,7 +27,12 @@
 
 def test_auth0_client_short_tenant_name() -> None:
     auth0client = Auth0Client("test.eu", ("client_id", "client_secret"))
     assert auth0client.token_endpoint == "https://test.eu.auth0.com/oauth/token"
     assert auth0client.revocation_endpoint == "https://test.eu.auth0.com/oauth/revoke"
     assert auth0client.userinfo_endpoint == "https://test.eu.auth0.com/userinfo"
     assert auth0client.jwks_uri == "https://test.eu.auth0.com/.well-known/jwks.json"
+
+
+def test_auth0_invalid_domain() -> None:
+    with pytest.raises(ValueError):
+        Auth0Client("ftp://mytenant.eu")
```

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_backchannel_authentication.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_backchannel_authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     requests_mock: RequestsMocker,
     backchannel_authentication_endpoint: str,
     bca_client: OAuth2Client,
     auth_req_id: str,
     scope: Union[None, str, List[str]],
     backchannel_auth_request_validator: RequestValidatorType,
 ) -> None:
-
     requests_mock.post(
         backchannel_authentication_endpoint,
         json={"auth_req_id": auth_req_id, "expires_in": 360, "interval": 3},
     )
     bca_resp = bca_client.backchannel_authentication_request(
         scope=scope, login_hint="user@example.com"
     )
@@ -115,15 +114,14 @@
 def test_backchannel_authentication_invalid_response(
     requests_mock: RequestsMocker,
     backchannel_authentication_endpoint: str,
     bca_client: OAuth2Client,
     scope: Union[None, str, List[str]],
     backchannel_auth_request_validator: RequestValidatorType,
 ) -> None:
-
     requests_mock.post(
         backchannel_authentication_endpoint,
         json={"foo": "bar"},
     )
     with pytest.raises(InvalidBackChannelAuthenticationResponse):
         bca_client.backchannel_authentication_request(
             scope=scope, login_hint="user@example.com"
@@ -141,15 +139,14 @@
     bca_client: OAuth2Client,
     private_jwk: Jwk,
     public_jwk: Jwk,
     auth_req_id: str,
     scope: Union[None, str, List[str]],
     backchannel_auth_request_jwt_validator: RequestValidatorType,
 ) -> None:
-
     requests_mock.post(
         backchannel_authentication_endpoint,
         json={"auth_req_id": auth_req_id, "expires_in": 360, "interval": 3},
     )
     bca_resp = bca_client.backchannel_authentication_request(
         private_jwk=private_jwk, scope=scope, login_hint="user@example.com", alg="RS256"
     )
@@ -169,15 +166,14 @@
 def test_backchannel_authentication_error(
     requests_mock: RequestsMocker,
     backchannel_authentication_endpoint: str,
     bca_client: OAuth2Client,
     scope: Union[None, str, List[str]],
     backchannel_auth_request_validator: RequestValidatorType,
 ) -> None:
-
     requests_mock.post(
         backchannel_authentication_endpoint,
         status_code=400,
         json={"error": "unauthorized_client"},
     )
     with pytest.raises(UnauthorizedClient):
         bca_client.backchannel_authentication_request(
@@ -193,15 +189,14 @@
 def test_backchannel_authentication_invalid_error(
     requests_mock: RequestsMocker,
     backchannel_authentication_endpoint: str,
     bca_client: OAuth2Client,
     scope: Union[None, str, List[str]],
     backchannel_auth_request_validator: RequestValidatorType,
 ) -> None:
-
     requests_mock.post(
         backchannel_authentication_endpoint,
         status_code=400,
         json={"foo": "bar"},
     )
     with pytest.raises(InvalidBackChannelAuthenticationResponse):
         bca_client.backchannel_authentication_request(
@@ -217,15 +212,14 @@
 def test_backchannel_authentication_not_json_error(
     requests_mock: RequestsMocker,
     backchannel_authentication_endpoint: str,
     bca_client: OAuth2Client,
     scope: Union[None, str, List[str]],
     backchannel_auth_request_validator: RequestValidatorType,
 ) -> None:
-
     requests_mock.post(
         backchannel_authentication_endpoint,
         status_code=400,
         text="Error!",
     )
     with pytest.raises(InvalidBackChannelAuthenticationResponse):
         bca_client.backchannel_authentication_request(
```

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_client.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import secrets
 from datetime import datetime, timedelta
 from typing import Dict, Type, Union
 
 import pytest
-from jwskate import Jwk, JwkSet
+from jwskate import Jwk, JwkSet, Jwt, KeyManagementAlgs
 
 from requests_oauth2client import (
     AuthorizationRequest,
-    AuthorizationResponse,
     BackChannelAuthenticationResponse,
     BaseClientAuthenticationMethod,
     BearerToken,
     ClientSecretBasic,
     ClientSecretJwt,
     ClientSecretPost,
     DeviceAuthorizationResponse,
     IdToken,
+    InvalidPushedAuthorizationResponse,
     InvalidTokenResponse,
     OAuth2Client,
     PrivateKeyJwt,
     PublicApp,
     RequestUriParameterAuthorizationRequest,
     ServerError,
     UnauthorizedClient,
@@ -62,18 +62,32 @@
     `default_auth_handler` uses ClientSecretBasic authentication."""
     client = OAuth2Client(token_endpoint, auth=ClientSecretBasic(client_id, client_secret))
     assert isinstance(client.auth, ClientSecretBasic)
     assert client.auth.client_id == client_id
     assert client.auth.client_secret == client_secret
 
 
-def test_missing_auth(token_endpoint: str) -> None:
+def test_invalid_auth(token_endpoint: str) -> None:
     """`auth` is required."""
     with pytest.raises(ValueError):
-        OAuth2Client(token_endpoint, auth=None)  # type: ignore[arg-type]
+        OAuth2Client(token_endpoint)
+    with pytest.raises(ValueError):
+        OAuth2Client(token_endpoint, auth=("client_id", "client_secret"), client_id="client_id")
+    with pytest.raises(ValueError):
+        OAuth2Client(
+            token_endpoint, auth=("client_id", "client_secret"), client_secret="client_secret"
+        )
+    with pytest.raises(ValueError):
+        OAuth2Client(token_endpoint, ("client_id", "client_secret"), client_id="client_id")
+    with pytest.raises(ValueError):
+        OAuth2Client(
+            token_endpoint,
+            client_secret="client_secret",
+            private_key=Jwk.generate_for_kty("EC", crv="P-256"),
+        )
 
 
 def test_client_credentials_grant(
     requests_mock: RequestsMocker,
     oauth2client: OAuth2Client,
     token_endpoint: str,
     access_token: str,
@@ -270,18 +284,40 @@
             requests_mock.last_request,
             client_id=client_id,
             endpoint=token_endpoint,
             public_jwk=public_jwk,
         )
 
 
+def test_ressource_owner_password_grant(
+    requests_mock: RequestsMocker,
+    oauth2client: OAuth2Client,
+    token_endpoint: str,
+) -> None:
+    username = "User01"
+    password = "Th1s_I5_a_P4ssw0rd!"
+
+    scope = "foo"
+    new_access_token = secrets.token_urlsafe()
+    requests_mock.post(
+        token_endpoint,
+        json={
+            "access_token": new_access_token,
+            "token_type": "Bearer",
+            "expires_in": 3600,
+            "scope": scope,
+        },
+    )
+
+    oauth2client.resource_owner_password(username, password, scope=scope)
+    assert requests_mock.called_once
+
+
 def test_grants_with_invalid_response_objects_as_parameter(oauth2client: OAuth2Client) -> None:
     with pytest.raises(ValueError):
-        oauth2client.authorization_code(AuthorizationResponse())
-    with pytest.raises(ValueError):
         oauth2client.refresh_token(BearerToken(access_token="foo"))
     with pytest.raises(ValueError):
         oauth2client.ciba(BackChannelAuthenticationResponse(auth_req_id=None))
     with pytest.raises(ValueError):
         oauth2client.device_code(
             DeviceAuthorizationResponse(
                 device_code=None, user_code="foo", verification_uri="bar"
@@ -367,16 +403,15 @@
     token_exchange_grant_validator: RequestValidatorType,
     public_app_auth_validator: RequestValidatorType,
     client_secret_basic_auth_validator: RequestValidatorType,
     client_secret_post_auth_validator: RequestValidatorType,
     client_secret_jwt_auth_validator: RequestValidatorType,
     private_key_jwt_auth_validator: RequestValidatorType,
 ) -> None:
-    """.token_exchange() sends a requests to the Token Endpoint using the Token Exchange
-    grant."""
+    """.token_exchange() sends a requests to the Token Endpoint using the Token Exchange grant."""
     subject_token = secrets.token_urlsafe()
     actor_token = secrets.token_urlsafe()
     new_access_token = secrets.token_urlsafe()
     new_refresh_token = secrets.token_urlsafe()
     requests_mock.post(
         token_endpoint,
         json={
@@ -493,14 +528,28 @@
 
     assert client.token_endpoint == token_endpoint
     assert client.revocation_endpoint == revocation_endpoint
     assert client.introspection_endpoint == introspection_endpoint
     assert client.userinfo_endpoint == userinfo_endpoint
     assert client.jwks_uri == jwks_uri
 
+    with pytest.raises(ValueError):
+        OAuth2Client.from_discovery_document(
+            {
+                "issuer": "https://something.else",
+                "token_endpoint": token_endpoint,
+                "revocation_endpoint": revocation_endpoint,
+                "introspection_endpoint": introspection_endpoint,
+                "userinfo_endpoint": userinfo_endpoint,
+                "jwks_uri": jwks_uri,
+            },
+            issuer=issuer,
+            auth=client_id,
+        )
+
 
 def test_from_discovery_document_missing_token_endpoint(
     revocation_endpoint: str, client_id: str
 ) -> None:
     """Invalid discovery documents raises an exception."""
     with pytest.raises(ValueError):
         OAuth2Client.from_discovery_document(
@@ -537,27 +586,35 @@
         )
 
 
 def test_from_discovery_endpoint(
     requests_mock: RequestsMocker,
     issuer: str,
     discovery_document: Dict[str, str],
+    jwks_uri: str,
+    as_public_jwks: JwkSet,
     client_auth_method: BaseClientAuthenticationMethod,
 ) -> None:
     discovery_url = oidc_discovery_document_url(issuer)
 
     requests_mock.get(discovery_url, json=discovery_document)
+    requests_mock.get(jwks_uri, json=as_public_jwks)
 
     client = OAuth2Client.from_discovery_endpoint(
         discovery_url, issuer, auth=client_auth_method
     )
 
-    assert requests_mock.called_once
+    assert requests_mock.request_history[0].url == discovery_url
+    assert requests_mock.request_history[1].url == jwks_uri
     assert isinstance(client, OAuth2Client)
     assert client.auth == client_auth_method
+    assert client.authorization_server_jwks == as_public_jwks
+
+    with pytest.raises(ValueError, match="at least one of `issuer` or `url`"):
+        OAuth2Client.from_discovery_endpoint()
 
 
 def test_invalid_token_response(
     requests_mock: RequestsMocker, token_endpoint: str, client_id: str
 ) -> None:
     """Token Endpoint error responses outside the standard raises an InvalidTokenResponse."""
     client = OAuth2Client(token_endpoint, auth=client_id)
@@ -575,26 +632,25 @@
         client.authorization_code("mycode")
     assert requests_mock.called_once
 
 
 def test_invalid_token_response_200(
     requests_mock: RequestsMocker, token_endpoint: str, client_id: str
 ) -> None:
-    """Token Endpoint successful responses outside the standard raises an
-    InvalidTokenResponse."""
+    """Token Endpoint successful responses outside the standard raises an InvalidTokenResponse."""
     client = OAuth2Client(token_endpoint, auth=client_id)
     requests_mock.post(token_endpoint, status_code=200, json={"confusing": "data"})
     with pytest.raises(InvalidTokenResponse):
         client.authorization_code("mycode")
 
     requests_mock.reset_mock()
     requests_mock.post(
         token_endpoint,
         status_code=200,
-        json={"error_description": "this shouldn't happen"},
+        json={"foo": "this shouldn't happen"},
     )
     with pytest.raises(InvalidTokenResponse):
         client.authorization_code("mycode")
     assert requests_mock.called_once
 
 
 def test_revoke_access_token(
@@ -811,16 +867,16 @@
     token_endpoint: str,
     revocation_endpoint: str,
     client_auth_method: BaseClientAuthenticationMethod,
     access_token: str,
     refresh_token: str,
     revocation_request_validator: RequestValidatorType,
 ) -> None:
-    """if a BearerToken is supplied and token_token_type_hint=refresh_token, take the refresh
-    token from the BearerToken."""
+    """If a BearerToken is supplied and token_token_type_hint=refresh_token, take the refresh token
+    from the BearerToken."""
     client = OAuth2Client(
         token_endpoint, revocation_endpoint=revocation_endpoint, auth=client_auth_method
     )
     bearer = BearerToken(access_token, refresh_token=refresh_token)
     requests_mock.post(revocation_endpoint, status_code=200)
 
     assert client.revoke_token(bearer, token_type_hint="refresh_token") is True
@@ -927,45 +983,47 @@
 
 def test_server_jwks(
     requests_mock: RequestsMocker,
     oauth2client: OAuth2Client,
     jwks_uri: str,
     server_public_jwks: JwkSet,
 ) -> None:
-    """get_public_jwks() fetches the AS public JWKS from its JWKS URI."""
+    """Use OAuth2Client as a context manager to automatically get the public JWKS from its JWKS
+    URI."""
     requests_mock.get(jwks_uri, json=dict(server_public_jwks))
-    assert oauth2client.get_public_jwks() == server_public_jwks
+    with oauth2client as client:
+        assert client.authorization_server_jwks == server_public_jwks
     assert requests_mock.called_once
 
 
 def test_server_jwks_no_jwks_uri(token_endpoint: str) -> None:
-    """If JWKS URI is not known, get_public_jwks() raises an exception."""
+    """If JWKS URI is not known, update_authorization_server_public_keys() raises an exception."""
     client = OAuth2Client(token_endpoint=token_endpoint, auth=("foo", "bar"))
-    with pytest.raises(ValueError):
-        assert client.get_public_jwks()
+    with pytest.raises(AttributeError):
+        assert client.update_authorization_server_public_keys()
 
 
 def test_server_jwks_not_json(
     requests_mock: RequestsMocker, token_endpoint: str, jwks_uri: str
 ) -> None:
     """If JWKS URI is not known, get_public_jwks() raises an exception."""
     requests_mock.get(jwks_uri, text="Hello World!")
     client = OAuth2Client(token_endpoint=token_endpoint, jwks_uri=jwks_uri, auth=("foo", "bar"))
     with pytest.raises(ValueError):
-        assert client.get_public_jwks()
+        assert client.update_authorization_server_public_keys()
     assert requests_mock.called_once
 
 
 def test_server_jwks_invalid_doc(
     requests_mock: RequestsMocker, token_endpoint: str, jwks_uri: str
 ) -> None:
     """If JWKS URI is an invalid document, get_public_jwks() raises an exception."""
     requests_mock.get(jwks_uri, json={"foo": "bar"})
     client = OAuth2Client(token_endpoint=token_endpoint, jwks_uri=jwks_uri, auth=("foo", "bar"))
-    jwks = client.get_public_jwks()
+    jwks = client.update_authorization_server_public_keys()
     assert requests_mock.called_once
     assert not jwks.jwks
 
 
 def test_get_token_type() -> None:
     assert (
         OAuth2Client.get_token_type(token_type="access_token")
@@ -1219,7 +1277,105 @@
 ) -> None:
     requests_mock.post(
         pushed_authorization_request_endpoint, json={"error": "server_error"}, status_code=500
     )
 
     with pytest.raises(ServerError):
         oauth2client.pushed_authorization_request(authorization_request)
+
+    requests_mock.post(pushed_authorization_request_endpoint, text="foobar", status_code=500)
+
+    with pytest.raises(InvalidPushedAuthorizationResponse):
+        oauth2client.pushed_authorization_request(authorization_request)
+
+
+def test_jwt_bearer_grant(
+    requests_mock: RequestsMocker, oauth2client: OAuth2Client, token_endpoint: str
+) -> None:
+    key = Jwk.generate_for_kty("EC", alg="ES256")
+    assertion = Jwt.sign({"iat": 1661759343, "exp": 1661759403, "sub": "some_user_id"}, key)
+    scope = "my_scope"
+
+    requests_mock.post(
+        token_endpoint,
+        json={"access_token": "access_token", "token_type": "Bearer", "scope": scope},
+    )
+
+    # pass the assertion as a `Jwt`
+    token = oauth2client.jwt_bearer(assertion=assertion, scope=scope)
+    assert isinstance(token, BearerToken)
+    assert requests_mock.called_once
+    assert token.scope == scope
+
+    # pass the assertion as `str`
+    requests_mock.reset_mock()
+    token = oauth2client.jwt_bearer(assertion=str(assertion), scope=scope)
+    assert isinstance(token, BearerToken)
+    assert requests_mock.called_once
+    assert token.scope == scope
+
+
+def test_authorization_request(oauth2client: OAuth2Client, authorization_endpoint: str) -> None:
+    scope = "my_scope"
+    auth_req = oauth2client.authorization_request(scope="my_scope")
+    assert isinstance(auth_req, AuthorizationRequest)
+    assert auth_req.authorization_endpoint == authorization_endpoint
+    assert auth_req.response_type == "code"
+    assert auth_req.scope == scope.split()
+
+    with pytest.raises(ValueError):
+        oauth2client.authorization_request(response_type="token")
+
+    with pytest.raises(AttributeError, match="No 'redirect_uri'"):
+        OAuth2Client(
+            auth=("client_id", "client_secret"),
+            token_endpoint="https://url.to.the/token_endpoint",
+            authorization_endpoint="https://url.to.the/authorization_endpoint",
+        ).authorization_request()
+
+
+def test_custom_token_type(requests_mock: RequestsMocker) -> None:
+    class WeirdBearerToken(BearerToken):
+        TOKEN_TYPE = "BearerToken"
+
+    class WeirdOAuth2Client(OAuth2Client):
+        token_class = WeirdBearerToken
+
+    TOKEN_ENDPOINT = "https://as.local/token"
+    client = WeirdOAuth2Client(TOKEN_ENDPOINT, ("client_id", "client_secret"))
+
+    requests_mock.post(
+        TOKEN_ENDPOINT,
+        json={"access_token": "access_token", "token_type": "BearerToken"},
+    )
+
+    token = client.client_credentials()
+    assert isinstance(token, WeirdBearerToken)
+
+
+def test_client_jwks() -> None:
+    private_key = Jwk.generate_for_alg(KeyManagementAlgs.RSA_OAEP_256).with_kid_thumbprint()
+    id_token_decryption_key = Jwk.generate_for_alg(
+        KeyManagementAlgs.ECDH_ES_A256KW
+    ).with_kid_thumbprint()
+    client = OAuth2Client(
+        authorization_endpoint="https://as.local/authorize",
+        token_endpoint="https://as.local/token",
+        client_id="my_client_id",
+        private_key=private_key,
+        id_token_decryption_key=id_token_decryption_key,
+    )
+
+    jwks = client.client_jwks
+    assert not jwks.is_private
+    assert private_key.public_jwk() in jwks.jwks
+    assert id_token_decryption_key.public_jwk() in jwks.jwks
+
+
+def test_issuer_identification_missing_issuer() -> None:
+    with pytest.raises(ValueError, match="issuer"):
+        OAuth2Client(
+            authorization_endpoint="https://as.local/authorize",
+            token_endpoint="https://as.local/token",
+            client_id="my_client_id",
+            authorization_response_iss_parameter_supported=True,
+        )
```

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_client_authentication.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_client_authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     requests_mock: RequestsMocker,
     access_token: str,
     token_endpoint: str,
     client_id: str,
     client_secret: str,
     client_secret_basic_auth_validator: RequestValidatorType,
 ) -> None:
-
     client = OAuth2Client(token_endpoint, ClientSecretBasic(client_id, client_secret))
 
     requests_mock.post(
         token_endpoint,
         json={"access_token": access_token, "token_type": "Bearer", "expires_in": 3600},
     )
 
@@ -63,15 +62,14 @@
     access_token: str,
     token_endpoint: str,
     client_id: str,
     private_jwk: Jwk,
     private_key_jwt_auth_validator: RequestValidatorType,
     public_jwk: Jwk,
 ) -> None:
-
     client = OAuth2Client(token_endpoint, PrivateKeyJwt(client_id, private_jwk=private_jwk))
 
     requests_mock.post(
         token_endpoint,
         json={"access_token": access_token, "token_type": "Bearer", "expires_in": 3600},
     )
 
@@ -80,14 +78,17 @@
     private_key_jwt_auth_validator(
         requests_mock.last_request,
         client_id=client_id,
         public_jwk=public_jwk,
         endpoint=token_endpoint,
     )
 
+    with pytest.raises(ValueError, match="requires a private key"):
+        PrivateKeyJwt(client_id, private_jwk.public_jwk())
+
 
 def test_private_key_jwt_with_kid(
     requests_mock: RequestsMocker,
     access_token: str,
     token_endpoint: str,
     client_id: str,
     private_jwk: Jwk,
@@ -115,15 +116,14 @@
     requests_mock: RequestsMocker,
     access_token: str,
     token_endpoint: str,
     client_id: str,
     client_secret: str,
     client_secret_jwt_auth_validator: RequestValidatorType,
 ) -> None:
-
     client = OAuth2Client(token_endpoint, ClientSecretJwt(client_id, client_secret))
 
     requests_mock.post(
         token_endpoint,
         json={"access_token": access_token, "token_type": "Bearer", "expires_in": 3600},
     )
 
@@ -141,15 +141,14 @@
     requests_mock: RequestsMocker,
     access_token: str,
     token_endpoint: str,
     client_id: str,
     target_api: str,
     public_app_auth_validator: RequestValidatorType,
 ) -> None:
-
     client = OAuth2Client(token_endpoint, client_id)
 
     requests_mock.post(
         token_endpoint,
         json={"access_token": access_token, "token_type": "Bearer", "expires_in": 3600},
     )
 
@@ -190,7 +189,10 @@
     pkj_client = OAuth2Client(token_endpoint, (client_id, dict(private_jwk)))
     assert isinstance(pkj_client.auth, PrivateKeyJwt)
     assert pkj_client.auth.client_id == client_id
     assert pkj_client.auth.private_jwk == private_jwk
 
     with pytest.raises(ValueError):
         OAuth2Client(token_endpoint, (client_id, {"foo": "bar"}))
+
+    with pytest.raises(TypeError, match="not supported"):
+        OAuth2Client(token_endpoint, (client_id, object()))  # type: ignore[arg-type]
```

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_device_authorization.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_device_authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 def test_device_authorization_response(
     device_code: str,
     user_code: str,
     verification_uri: str,
     verification_uri_complete: str,
 ) -> None:
-
     response = DeviceAuthorizationResponse(
         device_code=device_code,
         user_code=user_code,
         verification_uri=verification_uri,
         verification_uri_complete=verification_uri_complete,
         expires_in=180,
         interval=10,
@@ -68,15 +67,14 @@
 
 def test_device_authorization_response_no_expiration(
     device_code: str,
     user_code: str,
     verification_uri: str,
     verification_uri_complete: str,
 ) -> None:
-
     response = DeviceAuthorizationResponse(
         device_code=device_code,
         user_code=user_code,
         verification_uri=verification_uri,
         verification_uri_complete=verification_uri_complete,
         interval=10,
     )
```

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_discovery.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_flask.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_pkce.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_pkce.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_tokens.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import pytest
 from jwskate import (
     ExpiredJwt,
     InvalidClaim,
     InvalidJwt,
     InvalidSignature,
     Jwk,
-    Jwt,
     SignedJwt,
 )
 
 from requests_oauth2client import BearerToken, BearerTokenSerializer, IdToken
 
 ID_TOKEN = (
     "eyJhbGciOiJSUzI1NiIsImtpZCI6Im15X2tleSJ9.eyJhY3IiOiIyIiwiYW1yIjpbInB3ZCIsIm90cCJdLCJhdWQiOiJjbGllbnRfaWQiL"
@@ -39,41 +38,56 @@
         "access_token": "foo",
         "token_type": "Bearer",
     }
 
     assert str(token) == "foo"
     assert repr(token)
 
+    assert token == "foo"
+    assert token != 1.2
+
 
 def test_bearer_token_complete() -> None:
+    id_token = IdToken.sign(
+        {
+            "iss": "https://issuer.local",
+            "iat": IdToken.timestamp(),
+            "exp": IdToken.timestamp(60),
+            "sub": "myuserid",
+        },
+        Jwk.generate_for_alg("RS256"),
+    )
     token = BearerToken(
         access_token="foo",
         expires_in=180,
         scope="myscope1 myscope2",
         refresh_token="refresh_token",
         custom_attr="custom_value",
+        id_token=str(id_token),
     )
     assert "access_token" in token
     assert "refresh_token" in token
     assert "scope" in token
     assert "token_type" in token
     assert "expires_in" in token
     assert "foo" not in token
     assert "custom_attr" in token
+    assert "id_token" in token
     assert token.expires_in is not None
     assert token.expires_at is not None
     assert token.token_type == "Bearer"
 
     assert token.as_dict() == {
         "access_token": "foo",
         "token_type": "Bearer",
         "refresh_token": "refresh_token",
         "expires_in": token.expires_in,  # TODO: enhance
         "scope": "myscope1 myscope2",
         "custom_attr": "custom_value",
+        "id_token": str(id_token),
     }
 
     assert token.expires_in <= 180
     assert token.custom_attr == "custom_value"
 
     with pytest.raises(AttributeError):
         token.foo
@@ -95,26 +109,26 @@
         "kty": "RSA",
         "alg": "RS256",
         "kid": "my_key",
         "n": "2m4QVSHdUo2DFSbGY24cJbxE10KbgdkSCtm0YZ1q0Zmna8pJg8YhaWCJHV7D5AxQ_L1b1PK0jsdpGYWc5-Pys0FB2hyABGPxXIdg1mjxn6geHLpWzsA3MHD29oqfl0Rt7g6AFc5St3lBgJCyWtci6QYBmBkX9oIMOx9pgv4BaT6y1DdrNh27-oSMXZ0a58KwnC6jbCpdA3V3Eume-Be1Tx9lJN3j6S8ydT7CGY1Xd-sc3oB8pXfkr1_EYf0Sgb9EwOJfqlNK_kVjT3GZ-1JJMKJ6zkU7H0yXe2SKXAzfayvJaIcYrk-sYwmf-u7yioOLLvjlGjysN7SOSM8socACcw",
         "e": "AQAB",
     }
 
-    assert jwt.verify_signature(jwk=public_jwk)
+    assert jwt.verify_signature(public_jwk)
     assert jwt.expires_at is None
     assert jwt.issued_at is None
     assert jwt.not_before is None
     assert jwt.issuer is None
     assert jwt.alg == "RS256"
 
     with pytest.raises(InvalidClaim):
-        jwt.validate(jwk=public_jwk, issuer="foo")
+        jwt.validate(key=public_jwk, issuer="foo")
 
     with pytest.raises(InvalidClaim):
-        jwt.validate(jwk=public_jwk, audience="foo")
+        jwt.validate(key=public_jwk, audience="foo")
 
 
 def test_jwt_iat_exp_nbf() -> None:
     jwt = SignedJwt(
         "eyJhbGciOiJSUzI1NiIsImtpZCI6Im15X2tleSJ9.eyJleHAiOjE2MjkzODQ5ODgsImlhdCI6MTYyOTM4NDkyOCwibmJmIjoxNjI5Mzg0ODY4fQ.k_0abUntpK5yVOvalZGnhEhUuq1lmtoRQfKmEJuQpYiHCb3x9buYWclQCMNGzHikiyGtrRqN0RcyUPeGI9QN7hasvj1ItzrhsdXJDO968y3VXjfPnOz2lDPUKJjsTdWXbCGDZD82d4OX8E9WFaOwwutMb_5ismEBvttNAmwHJG433TzEO2rFhno9X3RPo8IqOJg_HSw8Q0BLsub7Ak9I0eGDsb8x5J8_fp6zqGkZaqL35DkLPZSHdLzYalmH4ksH69SVWu-7rD-W1brGxVpJg8unV9fy_1AmiQu-8tIedo68br2Tg0oNekwT-lXMTjmiJkYv8hpnECbtFXMRQSGcvQ"
     )
     public_jwk = {
@@ -156,15 +170,15 @@
     nonce = "nonce"
     acr = "2"
     id_token = IdToken(
         "eyJhbGciOiJSUzI1NiIsImtpZCI6Im15X2tleSJ9.eyJhY3IiOiIyIiwiYW1yIjpbInB3ZCIsIm90cCJdLCJhdWQiOiJjbGllbnRfaWQiLCJhdXRoX3RpbWUiOjE2MjkyMDQ1NjAsImV4cCI6MTYyOTIwNDYyMCwiaWF0IjoxNjI5MjA0NTYwLCJpc3MiOiJodHRwczovL215YXMubG9jYWwiLCJub25jZSI6Im5vbmNlIiwic3ViIjoiMTIzNDU2In0.wUfjMyjlOSdvbFGFP8O8wGcNBK7akeyOUBMvYcNZclFUtokOyxhLUPxmo1THo1DV1BHUVd6AWfeKUnyTxl_8-G3E_a9u5wJfDyfghPDhCmfkYARvqQnnV_3aIbfTfUBC4f0bHr08d_q0fED88RLu77wESIPCVqQYy2bk4FLucc63yGBvaCskqzthZ85DbBJYWLlR8qBUk_NA8bWATYEtjwTrxoZe-uA-vB6NwUv1h8DKRsDF-9HSVHeWXXAeoG9UW7zgxoY3KbDIVzemvGzs2R9OgDBRRafBBVeAkDV6CdbdMNJDmHzcjase5jX6LE-3YCy7c7AMM1uWRCnK3f-azA"
     )
 
     with pytest.raises(AttributeError):
-        id_token.not_found
+        id_token.attr_not_found
 
     id_token.validate(
         public_jwk,
         issuer=issuer,
         audience=audience,
         nonce=nonce,
         check_exp=False,
```

### Comparing `requests_oauth2client-1.1.0/tests/unit_tests/test_utils.py` & `requests_oauth2client-1.2.0/tests/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.1.0/setup.py` & `requests_oauth2client-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,923 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+`requests_oauth2client` is an OAuth 2.x client for Python, able to obtain, refresh and revoke tokens from any
+OAuth2.x/OIDC compliant Authorization Server. It sits upon and extends the famous [requests] HTTP client module.
 
-packages = \
-['requests_oauth2client',
- 'requests_oauth2client.flask',
- 'requests_oauth2client.vendor_specific',
- 'tests',
- 'tests.unit_tests']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['binapy>=0.6,<0.7', 'furl>=2.1.2', 'jwskate>=0.3.0,<0.4.0', 'requests>=2.19.0']
-
-setup_kwargs = {
-    'name': 'requests-oauth2client',
-    'version': '1.1.0',
-    'description': 'An OAuth2.x Client based on requests.',
-    'long_description': '`requests_oauth2client` is a OAuth 2.x client for Python, able to obtain, refresh and revoke tokens from any OAuth2.x/OIDC\ncompliant Authorization Server. It sits upon and extends the famous [requests] HTTP client module.\n\nIt can act as an [OAuth 2.0](https://tools.ietf.org/html/rfc6749) /\n[2.1](https://datatracker.ietf.org/doc/draft-ietf-oauth-v2-1) client, to automatically get and renew Access Tokens,\nbased on the\n[Client Credentials](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-03.html#name-client-credentials),\n[Authorization Code](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-03.html#name-authorization-code),\n[Refresh token](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-03.html#name-refresh-token),\n[Token Exchange](https://www.rfc-editor.org/rfc/rfc8693.html),\n[Device Authorization](https://www.rfc-editor.org/rfc/rfc8628.html), or\n[CIBA](https://openid.net/specs/openid-client-initiated-backchannel-authentication-core-1_0.html) grants.\n\nIt also supports [OpenID Connect 1.0](https://openid.net/specs/openid-connect-core-1_0.html),\n[PKCE](https://www.rfc-editor.org/rfc/rfc7636.html),\n[Client Assertions](https://www.rfc-editor.org/rfc/rfc7523.html),\n[Token Revocation](https://www.rfc-editor.org/rfc/rfc7009.html),\nand [Introspection](https://www.rfc-editor.org/rfc/rfc7662.html),\n[Resource Indicators](https://www.rfc-editor.org/rfc/rfc8707.html),\n[JWT-secured Authorization Requests](https://datatracker.ietf.org/doc/rfc9101/),\n[Pushed Authorization Requests](https://datatracker.ietf.org/doc/rfc9126/),\n[Authorization Server Issuer Identification](https://www.rfc-editor.org/rfc/rfc9207.html)\nas well as using custom params to any endpoint, and other important features that are often overlooked in other client\nlibraries.\n\nAnd it also includes a [wrapper][apiclient] around [requests.Session] that makes it super easy to use REST-style APIs,\nwith or without OAuth 2.x.\n\nPlease note that despite the name, this library has no relationship with Google\n[oauth2client](https://github.com/googleapis/oauth2client) library.\n\n[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)\n[![Downloads](https://pepy.tech/badge/requests_oauth2client/month)](https://pepy.tech/project/requests_oauth2client)\n[![Supported Versions](https://img.shields.io/pypi/pyversions/requests_oauth2client.svg)](https://pypi.org/project/requests_oauth2client)\n[![PyPi license](https://badgen.net/pypi/license/requests_oauth2client/)](https://pypi.com/project/requests_oauth2client/)\n[![PyPI status](https://img.shields.io/pypi/status/requests_oauth2client.svg)](https://pypi.python.org/pypi/requests_oauth2client/)\n[![GitHub commits](https://badgen.net/github/commits/guillp/requests_oauth2client)](https://github.com/guillp/requests_oauth2client/commit/)\n[![GitHub latest commit](https://badgen.net/github/last-commit/guillp/requests_oauth2client)](https://github.com/guillp/requests_oauth2client/commit/)\n\n# Documentation\n\nFull module documentation is available at https://guillp.github.io/requests_oauth2client/\n\n# Installation\n\n`requests_oauth2client` is [available from PyPi](https://pypi.org/project/requests-oauth2client/), so installing it is as easy as:\n\n```shell\npip install requests_oauth2client\n```\n\n# Usage\n\nEverything from `requests_oauth2client` is available from the root module, so you can import it like this:\n\n```python\nfrom requests_oauth2client import *\n```\n\nNote that this automatically imports `requests`, so no need to import it yourself.\n\n## Calling APIs with Access Tokens\n\nIf you already managed to obtain an access token, you can simply use the [BearerAuth] Auth Handler for [requests]:\n\n```python\nimport requests\nfrom requests_oauth2client import BearerToken\n\ntoken = "an_access_token"\nresp = requests.get("https://my.protected.api/endpoint", auth=BearerAuth(token))\n```\n\nThis authentication handler will add a properly formatted `Authorization` header in the request, with your access token\naccording to [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1).\n\n## Using an OAuth2Client\n\n[OAuth2Client] offers several methods that implement the communication to the various endpoints that are standardised by\nOAuth 2.0 and its extensions. Those endpoints include the Token Endpoint, the Revocation, Introspection, UserInfo,\nBackChannel Authentication and Device Authorization Endpoints. You only have to provide those if you intend to use them.\n\nTo initialize an [OAuth2Client], you only need a Token Endpoint URI, and the credentials for your application, which are\noften a `client_id` and a `client_secret`:\n\n```python\nfrom requests_oauth2client import OAuth2Client\n\noauth2client = OAuth2Client(\n    token_endpoint="https://myas.local/token_endpoint",\n    auth=("client_id", "client_secret"),\n)\n```\n\nThe Token Endpoint is the only endpoint that is mandatory to obtain tokens. Credentials are used to authenticate the\nclient everytime it sends a request to its Authorization Server. Usually, those are a static Client ID and Secret, which\nare the direct equivalent of a username and a password, but meant for an application instead of for a human user. The\ndefault authentication method used by `OAuth2Client` is *Client Secret Post*, but other standardised methods such as\n*Client Secret Basic*, *Client Secret JWT* or *Private Key JWT* are supported as well. See\n[more about client authentication methods below](#supported-client-authentication-methods).\n\n## Obtaining tokens\n\n[OAuth2Client] has methods to send requests to the Token Endpoint using the different standardised (and/or custom)\ngrants. Since the token endpoint and authentication method are already declared for the client at init time, the only\nrequired parameters are those that will be sent in the request to the Token Endpoint.\n\nThose methods directly return a [BearerToken] if the request is successful, or raise an exception if it fails.\n[BearerToken] will manage the token expiration, will contain the eventual refresh token that matches the access token,\nand will keep track of other associated metadata as well. You can create such a [BearerToken] yourself if you need:\n\n```python\nfrom requests_oauth2client import BearerToken\n\nbearer_token = BearerToken(access_token="an_access_token", expires_in=60)\nprint(bearer_token)\n# {\'access_token\': \'an_access_token\',\n#  \'expires_in\': 55,\n#  \'token_type\': \'Bearer\'}\nprint(bearer_token.expires_at)\n# datetime.datetime(2021, 8, 20, 9, 56, 59, 498793)\nassert not bearer_token.is_expired()\n```\n\nNote that the `expires_in` indicator here is not static. It keeps track of the token lifetime and is calculated as the\ntime flies. The actual static expiration date is accessible with the `expires_at` property. You can check if a token is\nexpired with [bearer_token.is_expired()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.tokens.BearerToken.is_expired).\n\nYou can use a [BearerToken] instance anywhere you can supply an access_token as string.\n\n### Using OAuth2Client as a requests Auth Handler\n\nWhile using [OAuth2Client] directly is great for testing or debugging OAuth2.x flows, it is not a viable option for\nactual applications where tokens must be obtained, used during their lifetime then obtained again or refreshed once they\nare expired. `requests_oauth2client` contains several [requests] compatible Auth Handlers (as subclasses of\n[requests.auth.AuthBase](https://requests.readthedocs.io/en/latest/user/advanced/#custom-authentication)), that will\ntake care of obtaining tokens when required, then will cache those tokens until they are expired, and will obtain new\nones (or refresh them, when possible), once the initial token is expired. Those are best used with a [requests.Session],\nor an [ApiClient], which is a wrapper around `Session` with a few enhancements as described below.\n\n### Client Credentials grant\n\nTo send a request using the Client Credentials grant, use the aptly named\n[.client_credentials()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.client_credentials)\nmethod, with the parameters to send in the token request as keyword parameters:\n\n```python\ntoken = oauth2client.client_credentials(scope="myscope", resource="https://myapi.local")\n```\n\nParameters such as `scope`, `resource` or `audience` that may be required by the AS can be passed as keyword\nparameters. Those will be included in the token request that is sent to the AS.\n\n#### As Auth Handler\n\nYou can use the\n[OAuth2ClientCredentialsAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2ClientCredentialsAuth)\nauth handler. It takes an [OAuth2Client] as parameter, and the additional kwargs to pass to the token endpoint:\n\n```python\nimport requests\n\nauth = OAuth2ClientCredentialsAuth(\n    oauth2client, scope="myscope", resource="https://myapi.local"\n)\n\n# use it like this:\nrequests.get("https://myapi.local/resource", auth=auth)\n\n# or\nsession = requests.Session()\nsession.auth = auth\n\nresp = session.get("https://myapi.local/resource")\n```\n\nOnce again, extra parameters such as `scope`, `resource` or `audience` are allowed if required.\n\nWhen you send your first request, [OAuth2ClientCredentialsAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2ClientCredentialsAuth)\nwill automatically retrieve an access token from the AS using the Client Credentials grant, then will include it in the\nrequest. Next requests will use the same token, as long as it is valid. A new token will be automatically retrieved once\nthe previous one is expired.\n\n### Authorization Code Grant\n\nObtaining tokens with the Authorization code grant is made in 3 steps:\n\n1. your application must open specific url called the *Authentication Request* in a browser.\n\n2. your application must obtain and validate the *Authorization Response*, which is a redirection back to your\n   application that contains an *Authorization Code* as parameter.\n\n3. your application must then exchange this Authorization Code for an *Access Token*, with a request to the Token\n   Endpoint.\n\n[OAuth2Client] doesn\'t implement anything that is related to the Authorization Request or Response. It is only able to\nexchange the Authorization Code for a Token in step 3. But `requests_oauth2client` has other classes to help you with\nsteps 1 and 2, as described below:\n\n#### Generating Authorization Requests\n\nYou can generate valid authorization requests with the\n[AuthorizationRequest](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.authorization_request.AuthorizationRequest)\nclass:\n\n```python\nauth_request = AuthorizationRequest(\n    authorization_endpoint,\n    client_id,\n    redirect_uri=redirect_uri,\n    scope=scope,\n    resource=resource,  # extra parameters can be included as well if required by your AS\n)\nprint(auth_request)  # redirect the user to that URL to get a code\n```\n\nThis request will look like this (with line breaks for display purposes only):\n\n```\nhttps://myas.local/authorize\n?client_id=my_client_id\n&redirect_uri=http%3A%2F%2Flocalhost%2Fcallback\n&response_type=code\n&state=kHWL4VwcbUbtPR4mtht6yMAGG_S-ZcBh5RxI_IGDmJc\n&nonce=mSGOS1M3LYU9ncTvvutoqUR4n1EtmaC_sQ3db4dyMAc\n&scope=openid+email+profile\n&code_challenge=Dk11ttaDb_Hyq1dObMqQcTIlfYYRVblFMC9lFM3UWW8\n&code_challenge_method=S256\n&resource=https%3A%2F%2Fmy.resource.local%2Fapi\n```\n\n[AuthorizationRequest] supports PKCE and uses it by default. You can avoid it by passing `code_challenge_method=None` to\n[AuthorizationRequest]. You can obtain the generated code_verifier from `auth_request.code_verifier`.\n\nRedirecting or otherwise sending the user to this url is your application responsibility, as well as obtaining the\nAuthorization Response url.\n\n#### Validating the Authorization Response\n\nOnce the user is successfully authenticated and authorized, the AS will respond with a redirection to your redirect_uri.\nThat is the *Authorization Response*. It contains several parameters that must be retrieved by your client. The\nauthorization code is one of those parameters, but you must also validate that the *state* matches your request. You can\ndo this with:\n\n```python\nresponse_uri = input(\n    "Please enter the full url and/or params obtained on the redirect_uri: "\n)\nauth_response = auth_request.validate_callback(response_uri)\n```\n\n#### Exchanging code for tokens\n\nTo exchange a code for Access and/or ID tokens, use the\n[OAuth2Client.authorization_code()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.authorization_code)\nmethod. If you have obtained an AuthorizationResponse as described above, you can simply do:\n\n```python\ntoken = oauth2client.authorization_code(auth_response)\n```\n\nThis will automatically include the `code`, `redirect_uri` and `code_verifier` parameters in the Token Request,\nas expected by the AS.\n\nIf you managed another way to obtain an Authorization Code, you can manually pass those parameters like this:\n\n```python\ntoken = oauth2client.authorization_code(\n    code=code,\n    code_verifier=code_verifier,\n    redirect_uri=redirect_uri,\n    custom_param=custom_value,\n)\n```\n\n#### As Auth Handler\n\nThe\n[OAuth2AuthorizationCodeAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2AuthorizationCodeAuth)\nhandler takes an [OAuth2Client] and an authorization code as parameter, plus whatever additional keyword parameters are\nrequired by your Authorization Server:\n\n```python\napi_client = ApiClient(\n    "https://your.protected.api/endpoint",\n    auth=OAuth2AuthorizationCodeAuth(\n        client,\n        code,\n        code_verifier=auth_request.code_verifier,\n        redirect_uri=redirect_uri,\n    ),\n)\n\nresp = api_client.post(\n    data={...}\n)  # first call will exchange the code for an initial access/refresh tokens\n```\n\n[OAuth2AuthorizationCodeAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2AuthorizationCodeAuth)\nwill take care of refreshing the token automatically once it is expired, using the refresh token, if available.\n\n### Device Authorization Grant\n\nHelpers for the Device Authorization Grant are also included. To get device and user codes:\n\n```python\nclient = OAuth2Client(\n    token_endpoint="https://myas.local/token",\n    device_authorization_endpoint="https://myas.local/device",\n    auth=(client_id, client_secret),\n)\n\nda_resp = client.authorize_device()\n```\n\n`da_resp` contains the Device Code, User Code, Verification URI and other info returned by the AS:\n\n```python\nda_resp.device_code\nda_resp.user_code\nda_resp.verification_uri\nda_resp.verification_uri_complete\nda_resp.expires_at  # just like for BearerToken, expiration is tracked by requests_oauth2client\nda_resp.interval\n```\n\nSend/show the Verification Uri and User Code to the user. He must use a browser to visit that url, authenticate and\ninput the User Code. You can then request the Token endpoint to check if the user successfully authorized you using an\n[OAuth2Client]:\n\n```python\ntoken = client.device_code(da_resp.device_code)\n```\n\nThis will raise an exception, either\n[AuthorizationPending](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.exceptions.AuthorizationPending),\n[SlowDown](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.exceptions.SlowDown),\n[ExpiredToken](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.exceptions.ExpiredToken), or\n[AccessDenied](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.exceptions.AccessDenied) if the\nuser did not yet finish authorizing your device, if you should increase your pooling period, or if the device code is no\nlonger valid, or the user finally denied your access, respectively. Other exceptions may be raised depending on the\nerror code that the AS responds with. If the user did finish authorizing successfully, `token` will contain your access\ntoken.\n\nTo make pooling easier, you can use a\n[DeviceAuthorizationPoolingJob](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.device_authorization.DeviceAuthorizationPoolingJob)\nlike this:\n\n```python\npool_job = DeviceAuthorizationPoolingJob(\n    client, device_auth_resp.device_code, interval=device_auth_resp.interval\n)\n\nresp = None\nwhile resp is None:\n    resp = pool_job()\n\nassert isinstance(resp, BearerToken)\n```\n\n[DeviceAuthorizationPoolingJob](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.device_authorization.DeviceAuthorizationPoolingJob)\nwill automatically obey the pooling period. Everytime you call pool_job(), it will wait the appropriate number of\nseconds as indicated by the AS, and will apply slow_down requests.\n\n#### As Auth Handler\n\nUse\n[OAuth2DeviceCodeAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2DeviceCodeAuth)\nas auth handler to exchange a device code for an access token:\n\n```python\napi_client = ApiClient(\n    "https://your.protected.api/endpoint",\n    auth=OAuth2DeviceCodeAuth(\n        client,\n        device_auth_resp.device_code,\n        interval=device_auth_resp.interval,\n        expires_in=device_auth_resp.expires_in,\n    ),\n)\n\nresp = api_client.post(\n    data={...}\n)  # first call will hang until the user authorizes your app and the token endpoint returns a token.\n```\n\n### Client-Initiated BackChannel Authentication (CIBA)\n\nTo initiate a BackChannel Authentication against the dedicated endpoint:\n\n```python\nclient = OAuth2Client(\n    token_endpoint="https://myas.local/token",\n    backchannel_authentication_endpoint="https://myas.local/backchannel_authorize",\n    auth=(client_id, client_secret),\n)\n\nba_resp = client.backchannel_authentication_request(\n    scope="openid email profile",\n    login_hint="user@example.net",\n)\n```\n\n`ba_resp` will contain the response attributes as returned by the AS, including an `auth_req_id`:\n\n```python\nba_resp.auth_req_id\nba_resp.expires_in  # decreases as times fly\nba_resp.expires_at  # a datetime to keep track of the expiration date, based on the "expires_in" returned by the AS\nba_resp.interval  # the pooling interval indicated by the AS\nba_resp.custom  # if the AS respond with additional attributes, they are also accessible\n```\n\nTo pool the Token Endpoint until the end-user successfully authenticates:\n\n```python\npool_job = BackChannelAuthenticationPoolingJob(\n    client=client,\n    auth_req_id=ba_resp.auth_req_id,\n    interval=bca_resp.interval,\n)\n\nresp = None\nwhile resp is None:\n    resp = pool_job()\n\nassert isinstance(resp, BearerToken)\n```\n\nHints by the AS to slow down pooling will automatically be obeyed.\n\n### Token Exchange\n\nTo send a token exchange request, use the\n[OAuth2Client.token_exchange()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.token_exchange)\nmethod:\n\n```python\nclient = OAuth2Client(token_endpoint, auth=...)\ntoken = client.token_exchange(\n    subject_token="your_token_value",\n    subject_token_type="urn:ietf:params:oauth:token-type:access_token",\n)\n```\n\nAs with the other grant-type specific methods, you may specify additional keyword parameters, that will be passed to the\ntoken endpoint, including any standardised attribute like `actor_token` or `actor_token_type`, or any custom parameter.\nThere are short names for token types, that will be automatically translated to standardised types:\n\n```python\ntoken = client.token_exchange(\n    subject_token="your_token_value",\n    subject_token_type="access_token",  # will be automatically replaced by "urn:ietf:params:oauth:token-type:access_token"\n    actor_token="your_actor_token",\n    actor_token_type="id_token",  # will be automatically replaced by "urn:ietf:params:oauth:token-type:id_token"\n)\n```\n\nOr to make it even easier, types can be guessed based on the supplied subject or actor token:\n\n```python\ntoken = client.token_exchange(\n    subject_token=BearerToken(\n        "your_token_value"\n    ),  # subject_token_type will be "urn:ietf:params:oauth:token-type:access_token"\n    actor_token=IdToken(\n        "your_actor_token"\n    ),  # actor_token_type will be "urn:ietf:params:oauth:token-type:id_token"\n)\n```\n\n## Supported Client Authentication Methods\n\n`requests_oauth2client` supports several client authentication methods, as defined in multiple OAuth2.x standards. You\nselect the appropriate method to use when initializing your [OAuth2Client], with the `auth` parameter. Once initialized,\na client will automatically use the configured authentication method every time it sends a requested to an endpoint that\nrequires client authentication. You don\'t have anything else to do afterwards.\n\n### Client Secret Basic\n\nWith **client_secret_basic**, `client_id` and `client_secret` are included in clear-text in the `Authorization` header when sending requests to the Token Endpoint. To use\nit, just pass a\n[`ClientSecretBasic(client_id, client_secret)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.ClientSecretBasic)\nas `auth` parameter:\n\n```python\nfrom requests_oauth2client import OAuth2Client, ClientSecretBasic\n\nclient = OAuth2Client(token_endpoint, auth=ClientSecretBasic(client_id, client_secret))\n```\n\n### Client Secret Post\n\nWith **client_secret_post**, `client_id` and `client_secret` are included as part of the body form data. To use it, pass a\n[`ClientSecretPost(client_id, client_secret)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.ClientSecretPost)\nas `auth` parameter. This is the default when you pass a tuple `(client_id, client_secret)` as\n`auth` when initializing an `OAuth2Client`:\n\n```python\nfrom requests_oauth2client import OAuth2Client, ClientSecretPost\n\nclient = OAuth2Client(token_endpoint, auth=ClientSecretPost(client_id, client_secret))\n# or\nclient = OAuth2Client(token_endpoint, auth=(client_id, client_secret))\n```\n\n### Client Secret JWT\n\nWith **client_secret_jwt**, the client generates an ephemeral JWT assertion including information about itself (client_id), the\nAS (url of the endpoint), and an expiration date a few seconds in the future. To use it, pass a\n[`ClientSecretJwt(client_id, client_secret)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.ClientSecretJwt)\nas `auth` parameter. Assertion generation is entirely automatic, you don\'t have anything to do:\n\n```python\nfrom requests_oauth2client import OAuth2Client, ClientSecretJwt\n\nclient = OAuth2Client(token_endpoint, auth=ClientSecretJwt(client_id, client_secret))\n```\n\nThis method is more secure than the 2 previous, because only ephemeral credentials are transmitted, which limits the possibility for interception and replay of the Client Secret.\nBut that Client Secret still needs to be shared between the AS and Client owner(s).\n\n### Private Key JWT\n\nWith **private_key_jwt**, client uses a JWT assertion that is just like _client_secret_jwt_, but it is signed with an _asymmetric_ key.\nTo use it, you need a private signing key, in a `dict` that matches the JWK format, or as an instance of `jwskate.Jwk`. The matching public key must be\nregistered for your client on AS side. Once you have that, using this auth method is simple with the\n[`PrivateKeyJwt(client_id, private_jwk)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.PrivateKeyJwt)\nauth handler:\n\n```python\nfrom requests_oauth2client import OAuth2Client, PrivateKeyJwt\n\nprivate_jwk = {\n    "kid": "mykid",\n    "kty": "RSA",\n    "e": "AQAB",\n    "n": "...",\n    "d": "...",\n    "p": "...",\n    "q": "...",\n    "dp": "...",\n    "dq": "...",\n    "qi": "...",\n}\n\nclient = OAuth2Client(\n    "https://myas.local/token", auth=PrivateKeyJwt(client_id, private_jwk)\n)\n# or\nclient = OAuth2Client(token_endpoint, auth=(client_id, private_jwk))\n```\n\nThis method can be considered more secure than those relying on a client secret, because only ephemeral credentials are sent over the wire, and it uses asymetric cryptography: the signing key is generated by the client, and only the public key is known by the AS.\nTransmitting that public key between owner(s) of the client and of the AS is much easier than transmitting the Client Secret, which is a shared key that must be considered as confidential.\n\n### None\n\nThe latest Client Authentication Method, **none**, is for Public Clients which do not authenticate to the Token Endpoint.\nThose clients only include their `client_id` in body form data, without any authentication credentials. Use\n[`PublicApp(client_id)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.PublicApp):\n\n```python\nfrom requests_oauth2client import OAuth2Client, PublicApp\n\nclient = OAuth2Client(token_endpoint, auth=PublicApp(client_id, client_secret))\n```\n\n## Token Revocation\n\n[OAuth2Client] can send revocation requests to a Revocation Endpoint. You need to provide a Revocation Endpoint URI when\ncreating the [OAuth2Client] :\n\n```python\noauth2client = OAuth2Client(\n    token_endpoint,\n    revocation_endpoint=revocation_endpoint,\n    auth=ClientSecretJwt("client_id", "client_secret"),\n)\n```\n\nThe\n[OAuth2Client.revoke_token()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.revoke_token)\nmethod and its specialized aliases\n[.revoke_access_token()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.revoke_access_token)\nand\n[.revoke_refresh_token()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.revoke_refresh_token)\nare then available:\n\n```python\noauth2client.revoke_token("mytoken", token_type_hint="access_token")\noauth2client.revoke_access_token(\n    "mytoken"\n)  # will automatically add token_type_hint=access_token\noauth2client.revoke_refresh_token(\n    "mytoken"\n)  # will automatically add token_type_hint=refresh_token\n```\n\nBecause Revocation Endpoints usually don\'t return meaningful responses, those methods return a boolean. This boolean\nindicates that a request was successfully sent and no error was returned. If the Authorization Server actually returns a\nstandardised error, an exception will be raised instead.\n\n## Token Introspection\n\n[OAuth2Client] can send requests to a Token Introspection Endpoint. You need to provide an Introspection Endpoint URI\nwhen creating the `OAuth2Client`:\n\n```python\noauth2client = OAuth2Client(\n    token_endpoint,\n    introspection_endpoint=introspection_endpoint,\n    auth=ClientSecretJwt("client_id", "client_secret"),\n)\n```\n\nThe\n[OAuth2Client.introspect_token()](<https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.instrospect_token()>)\nmethod is then available:\n\n```python\nresp = oauth2client.introspect_token("mytoken", token_type_hint="access_token")\n```\n\nIt returns whatever data is returned by the introspection endpoint (if it is a JSON, its content is returned decoded).\n\n## UserInfo Requests\n\n[OAuth2Client] can send requests to an UserInfo Endpoint. You need to provide an UserInfo Endpoint URI when creating the\n`OAuth2Client`:\n\n```python\noauth2client = OAuth2Client(\n    token_endpoint,\n    userinfo_endpoint=userinfo_endpoint,\n    auth=ClientSecretJwt("client_id", "client_secret"),\n)\n```\n\nThe\n[OAuth2Client.userinfo()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.userinfo))\nmethod is then available:\n\n```python\nresp = oauth2client.userinfo("mytoken")\n```\n\nIt returns whatever data is returned by the userinfo endpoint (if it is a JSON, its content is returned decoded).\n\n## Initializing an OAuth2Client from a discovery document\n\nYou can initialize an [OAuth2Client] with the endpoint URIs mentioned in a standardised discovery document with the\n[OAuth2Client.from_discovery_endpoint()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.from_discovery_document)\nclass method:\n\n```python\noauth2client = OAuth2Client.from_discovery_endpoint(\n    "https://myas.local/.well-known/openid-configuration"\n)\n```\n\nThis will fetch the document from the specified URI, then will decode it and initialize an [OAuth2Client] pointing to\nthe appropriate endpoint URIs.\n\n## Specialized API Client\n\nUsing APIs usually involves multiple endpoints under the same root url, with a common authentication method. To make it\neasier, `requests_oauth2client` includes a [requests.Session] wrapper called [ApiClient], which takes the\nroot API url as parameter on initialization. You can then send requests to different endpoints by passing their relative\npath instead of the full url. [ApiClient] also accepts an `auth` parameter with an AuthHandler. You can pass any of the\nOAuth2 Auth Handler from this module, or any [requests]-compatible\n[Authentication Handler](https://requests.readthedocs.io/en/latest/user/advanced/#custom-authentication). Which makes\nit very easy to call APIs that are protected with an OAuth2 Client Credentials Grant:\n\n```python\noauth2client = OAuth2Client("https://myas.local/token", (client_id, client_secret))\napi = ApiClient(\n    "https://myapi.local/root", auth=OAuth2ClientCredentialsAuth(oauth2client)\n)\n\n# will actually send a GET to https://myapi.local/root/resource/foo\nresp = api.get("/resource/foo")\n```\n\nNote that [ApiClient] will never send requests "outside" its configured root url, unless you specifically give it a full\nurl at request time. The leading `/` in `/resource` above is optional. A leading `/` will not "reset" the url path to\nroot, which means that you can also write the relative path without the `/` and it will automatically be included:\n\n```python\napi.get("resource/foo")  # will also send a GET to https://myapi.local/root/resource/foo\n```\n\nYou may also pass the path as an iterable of strings (or string-able objects), in which case they will be joined with a\n`/` and appended to the url path:\n\n```python\n# will send a GET to https://myapi.local/root/resource/foo\napi.get(["resource", "foo"])\n# will send a GET to https://myapi.local/root/users/1234/details\napi.get(["users", 1234, "details"])\n```\n\nYou can also use a syntax based on `__getattr__` or `__getitem__`:\n\n```python\napi.resource.get()  # will send a GET to https://myapi.local/root/resource\napi["my-resource"].get()  # will send a GET to https://myapi.local/root/my-resource\n```\n\nBoth `__getattr__` and `__getitem__` return a new `ApiClient` initialised on the new base_url.\nSo you can easily call multiple sub-resources on the same API this way:\n\n```python\napi = ApiClient("https://myapi.local")\nusers_api = api.users\nuser = users_api.get("userid")  # GET https://myapi.local/users/userid\nother_user = users_api.get("other_userid")  # GET https://myapi.local/users/other_userid\nresources_api = api.resources\nresources = resources_api.get()  # GET https://myapi.local/resources\n```\n\n[ApiClient] will, by default, raise exceptions whenever a request returns an error status. You can disable that by\npassing `raise_for_status=False` when initializing your [ApiClient]:\n\n```python\napi = ApiClient(\n    "http://httpstat.us", raise_for_status=False\n)  # raise_for_status defaults to True\nresp = api.get("500")\nassert resp is not None\n# without raise_for_status=False, a requests.exceptions.HTTPError exception would be raised instead\n```\n\nYou may override this at request time:\n\n```python\n# raise_for_status at request-time overrides the value defined at init-time\nresp = api.get("500", raise_for_status=True)\n```\n\nYou can access the underlying `requests.Session` with the session attribute, and you can provide an already existing and configured `Session` instance at init time:\n\n```python\nimport requests\n\nsession = requests.Session()\nsession.proxies = {"https": "http://localhost:3128"}\napi = ApiClient("https://myapi.local/resource", session=session)\nassert api.session == session\n```\n\n## Vendor-Specific clients\n\n`requests_oauth2client` being flexible enough to handle most use cases, you should be able to use any AS by any vendor\nas long as it supports OAuth 2.0.\n\nYou can however create a subclass of [OAuth2Client] or [ApiClient] to make it easier to use with specific Authorization\nServers or APIs. The sub-module `requests_oauth2client.vendor_specific` includes such classes for [Auth0](https://auth0.com):\n\n```python\nfrom requests_oauth2client.vendor_specific import Auth0Client\n\na0client = Auth0Client("mytenant.eu", (client_id, client_secret))\n# this will automatically initialize the token endpoint to https://mytenant.eu.auth0.com/oauth/token\n# and other endpoints accordingly\ntoken = a0client.client_credentials(audience="audience")\n\n# this is a wrapper around Auth0 Management API\na0mgmt = Auth0ManagementApiClient("mytenant.eu", (client_id, client_secret))\nmyusers = a0mgmt.get("users")\n```\n\n[apiclient]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.api_client.ApiClient\n[authorizationrequest]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.authorization_request.AuthorizationRequest\n[bearerauth]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.BearerAuth\n[bearertoken]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.tokens.BearerToken\n[oauth2client]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client\n[requests]: https://requests.readthedocs.io/en/latest/\n[requests.session]: https://requests.readthedocs.io/en/latest/api/#requests.Session\n',
-    'author': 'Guillaume Pujol',
-    'author_email': 'guill.p.linux@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/guillp/requests_oauth2client',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+It can act as an [OAuth 2.0](https://tools.ietf.org/html/rfc6749) /
+[2.1](https://datatracker.ietf.org/doc/draft-ietf-oauth-v2-1) client, to automatically get and renew Access Tokens,
+based on the
+[Client Credentials](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-07.html#name-client-credentials),
+[Authorization Code](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-07.html#name-authorization-code),
+[Refresh token](https://www.ietf.org/archive/id/draft-ietf-oauth-v2-1-07.html#name-refresh-token),
+[Token Exchange](https://www.rfc-editor.org/rfc/rfc8693.html),
+[JWT Bearer](https://www.rfc-editor.org/rfc/rfc7523.html#section-2.1),
+[Device Authorization](https://www.rfc-editor.org/rfc/rfc8628.html),
+[Resource Owner Password](https://www.rfc-editor.org/rfc/rfc6749#section-4.3) or
+[CIBA](https://openid.net/specs/openid-client-initiated-backchannel-authentication-core-1_0.html) grants. Additional
+grant types are easy to add if needed.
+
+It also supports [OpenID Connect 1.0](https://openid.net/specs/openid-connect-core-1_0.html),
+[PKCE](https://www.rfc-editor.org/rfc/rfc7636.html),
+[Client Assertions](https://www.rfc-editor.org/rfc/rfc7523.html#section-2.2),
+[Token Revocation](https://www.rfc-editor.org/rfc/rfc7009.html), and
+[Introspection](https://www.rfc-editor.org/rfc/rfc7662.html),
+[Resource Indicators](https://www.rfc-editor.org/rfc/rfc8707.html),
+[JWT-secured Authorization Requests](https://datatracker.ietf.org/doc/rfc9101/),
+[Pushed Authorization Requests](https://datatracker.ietf.org/doc/rfc9126/),
+[Authorization Server Issuer Identification](https://www.rfc-editor.org/rfc/rfc9207.html), as well as using custom
+params to any endpoint, and other important features that are often overlooked in other client libraries.
+
+And it also includes a [wrapper][apiclient] around [requests.Session] that makes it super easy to use REST-style APIs,
+with or without OAuth 2.x.
+
+Please note that despite the name, this library has no relationship with Google
+[oauth2client](https://github.com/googleapis/oauth2client) library.
+
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![Downloads](https://pepy.tech/badge/requests_oauth2client/month)](https://pepy.tech/project/requests_oauth2client)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/requests_oauth2client.svg)](https://pypi.org/project/requests_oauth2client)
+[![PyPi license](https://badgen.net/pypi/license/requests_oauth2client/)](https://pypi.com/project/requests_oauth2client/)
+[![PyPI status](https://img.shields.io/pypi/status/requests_oauth2client.svg)](https://pypi.python.org/pypi/requests_oauth2client/)
+[![GitHub commits](https://badgen.net/github/commits/guillp/requests_oauth2client)](https://github.com/guillp/requests_oauth2client/commit/)
+[![GitHub latest commit](https://badgen.net/github/last-commit/guillp/requests_oauth2client)](https://github.com/guillp/requests_oauth2client/commit/)
+
+# Documentation
+
+Full module documentation is available at https://guillp.github.io/requests_oauth2client/
+
+# Installation
+
+`requests_oauth2client` is [available from PyPi](https://pypi.org/project/requests-oauth2client/), so installing it is
+as easy as:
+
+```shell
+pip install requests_oauth2client
+```
+
+# Usage
+
+Everything from `requests_oauth2client` is available from the root module, so you can import it like this:
+
+```python
+from requests_oauth2client import *
+```
+
+Or you can import individual objects from this package as usual. Note that importing `*` automatically imports
+`requests`, so no need to import it yourself.
+
+## Calling APIs with Access Tokens
+
+If you already managed to obtain an access token for the API you want to call, you can simply use the [BearerAuth] Auth
+Handler for [requests]:
+
+```python
+import requests
+from requests_oauth2client import BearerAuth
+
+token = "an_access_token"
+resp = requests.get("https://my.protected.api/endpoint", auth=BearerAuth(token))
+```
+
+This authentication handler will add a properly formatted `Authorization: Bearer <access_token>` header in the request,
+with your access token according to [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1).
+
+## Using an OAuth2Client
+
+[OAuth2Client] offers several methods that implement the communication to the various endpoints that are standardised by
+OAuth 2.0 and its extensions. Those endpoints include the Token Endpoint, the Revocation, Introspection, UserInfo,
+BackChannel Authentication and Device Authorization Endpoints.
+
+You have to provide the URLs for those endpoints if you intend to use them. Otherwise, only the Token Endpoint is
+mandatory to initialize an `OAuth2Client`.
+
+To initialize an [OAuth2Client], you only need a Token Endpoint URI from your AS, and the credentials for your
+application, which are often a `client_id` and a `client_secret`, usually also provided by the AS:
+
+```python
+from requests_oauth2client import OAuth2Client
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    client_id="my_client_id",
+    client_secret="my_client_secret",
+)
+```
+
+The Token Endpoint is the only endpoint that is mandatory to obtain tokens. Credentials are used to authenticate the
+client everytime it sends a request to its Authorization Server. Usually, those are a static Client ID and Secret, which
+are the direct equivalent of a username and a password, but meant for an application instead of for a human user. The
+default authentication method used by `OAuth2Client` is *Client Secret Post*, but other standardised methods such as
+*Client Secret Basic*, *Client Secret JWT* or *Private Key JWT* are supported as well. See
+[more about client authentication methods below](#supported-client-authentication-methods).
+
+## Obtaining tokens
+
+[OAuth2Client] has dedicated methods to send requests to the Token Endpoint using the different standardised (and/or
+custom) grants. Since the Token Endpoint URL and Client Authentication Method to use are already declared for the client
+at init time, the only required parameters for those methods are those that will be sent in the request to the Token
+Endpoint.
+
+Those methods directly return a [BearerToken] if the request is successful, or raise an exception if it fails.
+[BearerToken] contains all the data as returned by the Token Endpoint, including the Access Token. It will:
+
+- keep track of the Access Token expiration date (based on the `expires_in` hint as returned by the AS). This date is
+  accessible with the `expires_at` attribute.
+- contain the Refresh Token, if returned by the AS, accessible with the `refresh_token` attribute.
+- contain the ID Token, if returned by the AS, accessible with the `ìd_token` attribute (when using the Authorization
+  Code flow).
+- keep track of other associated metadata as well, also accessible as attributes with the same name:
+  `token.custom_attr`, or with subscription syntax `token["my.custom.attr"]`.
+
+You can create such a [BearerToken] yourself if you need:
+
+```python
+from requests_oauth2client import BearerToken
+
+bearer_token = BearerToken(access_token="an_access_token", expires_in=60)
+print(bearer_token)
+# {'access_token': 'an_access_token',
+#  'expires_in': 55,
+#  'token_type': 'Bearer'}
+print(bearer_token.expires_at)
+# datetime.datetime(2021, 8, 20, 9, 56, 59, 498793)
+assert not bearer_token.is_expired()
+
+print(bearer_token.expires_in)
+# 40
+```
+
+Note that the `expires_in` indicator here is not static. It keeps track of the token lifetime, in seconds, and is
+calculated as the time flies. The actual static expiration date is accessible with the `expires_at` property. You can
+check if a token is expired with
+[bearer_token.is_expired()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.tokens.BearerToken.is_expired).
+
+You can use a [BearerToken] instance anywhere you can use an access_token as string.
+
+### Using OAuth2Client as a requests Auth Handler
+
+While using [OAuth2Client] directly is great for testing or debugging OAuth2.x flows, it is not a viable option for
+actual applications where tokens must be obtained, used during their lifetime then obtained again or refreshed once they
+are expired. `requests_oauth2client` contains several [requests] compatible Auth Handlers (as subclasses of
+[requests.auth.AuthBase](https://requests.readthedocs.io/en/latest/user/advanced/#custom-authentication)), that will
+take care of obtaining tokens when required, then will cache those tokens until they are expired, and will obtain new
+ones (or refresh them, when possible), once the initial token is expired. Those are best used with a [requests.Session],
+or an [ApiClient], which is a wrapper around `Session` with a few enhancements as described below.
+
+### Client Credentials grant
+
+To send a request using the Client Credentials grant, use the aptly named
+[.client_credentials()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.client_credentials)
+method, with the parameters to send in the token request as keyword parameters:
+
+```python
+from requests_oauth2client import OAuth2Client
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    auth=("client_id", "client_secret"),
+)
+
+token = oauth2client.client_credentials(scope="myscope")
+# or, if your AS uses resource indicator:
+token = oauth2client.client_credentials(scope="myscope", resource="https://myapi.local")
+# or, if your AS uses 'audience' as parameter to identify the requested API (Auth0 style):
+token = oauth2client.client_credentials(audience="https://myapi.local")
+# or, if your AS uses custom parameters:
+token = oauth2client.client_credentials(scope="myscope", custom_param="custom_value")
+```
+
+Parameters such as `scope`, `resource` or `audience` or any other parameter that may be required by the AS can be passed
+as keyword parameters. Those will be included in the token request that is sent to the AS. `scope` is not mandatory at
+client level (but it might be required by your AS to serve your request).
+
+#### As Auth Handler
+
+You can use the
+[OAuth2ClientCredentialsAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2ClientCredentialsAuth)
+auth handler. It takes an [OAuth2Client] as parameter, and the additional kwargs to pass to the token endpoint:
+
+```python
+import requests
+from requests_oauth2client import OAuth2Client, OAuth2ClientCredentialsAuth
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    auth=("client_id", "client_secret"),
+)
+
+auth = OAuth2ClientCredentialsAuth(
+    oauth2client, scope="myscope", resource="https://myapi.local"
+)
+
+# use it like this:
+requests.get("https://myapi.local/resource", auth=auth)
+
+# or like this:
+session = requests.Session()
+session.auth = auth
+
+resp = session.get("https://myapi.local/resource")
+```
+
+Once again, extra parameters such as `scope`, `resource` or `audience` are allowed if required.
+
+When you send your first request,
+[OAuth2ClientCredentialsAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2ClientCredentialsAuth)
+will automatically retrieve an access token from the AS using the Client Credentials grant, then will include it in the
+request. Next requests will use the same token, as long as it is valid. A new token will be automatically retrieved once
+the previous one is expired.
+
+### Authorization Code Grant
+
+Obtaining tokens with the Authorization code grant is made in 3 steps:
+
+1. your application must open a specific url called the *Authentication Request* in a browser.
+
+2. your application must obtain and validate the *Authorization Response*, which is a redirection back to your
+   application that contains an *Authorization Code* as parameter. This redirect back (often called "callback") is
+   initiated by the Authorization Server after any necessary interaction with the user is complete (Registration, Login,
+   Profile completion, Multi-Factor Authentication, Authorization, Consent, etc.)
+
+3. your application must then exchange this Authorization Code for an *Access Token*, with a request to the Token
+   Endpoint.
+
+`requests_oauth2client`, and more specifically [OAuth2Client] will help you with all those steps, as described below.
+
+#### Generating Authorization Requests
+
+To be able to use the Authorization Code grant, you need two urls:
+
+- the URL for Authorization Endpoint, which is the url where you must send your Authorization Requests
+- the Redirect URI, which is the url pointing to your application, where the Authorization Server will reply with
+  Authorization Response
+
+You can declare those urls when initializing your OAuth2Client instance. Then you can generate valid Authorization
+Requests by calling the method `.authorization_request()`:
+
+```python
+from requests_oauth2client import OAuth2Client
+
+client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endoint",
+    authorization_endpoint="https://url.to.the/authorization_endpoint",
+    redirect_uri="https://url.to.my.application/redirect_uri",
+    client_id="client_id",
+    client_secret="client_secret",
+)
+
+az_request = client.authorization_request(scope="openid email profile")
+
+print(az_request)
+# this will look like this, with line feeds for display purposes only:
+# https://url.to.the/authorization_endpoint
+# ?client_id=client_id
+# &redirect_uri=https%3A%2F%2Furl.to.my.application%2Fredirect_uri
+# &response_type=code
+# &scope=openid+email+profile
+# &state=FBx9mWeLwoKGgG76vhi6v61-4mgxmgZhtWIa7aTffdY
+# &nonce=iHZJokhkGOAojff1tdknRyz9mPZyy5vq9JDlVaUHyqk
+# &code_challenge=TG7qgdyKnwUPuoQ6NNJRlLMoHbeVmJlB8g0VOcfQEkc
+# &code_challenge_method=S256
+
+# you can send the user to that url with:
+import webbrowser
+
+webbrowser.open(az_request.uri)
+```
+
+Note that the `state`, `nonce` and `code_challenge` parameters are generated with secure random values by default.
+Should you wish to use your own values, you can pass them as parameters to `OAuth2Client.authorization_request()`. For
+PKCE, you need to pass your generated `code_verifier`, and the `code_challenge` will automatically be derived from it.
+If you don't want to use PKCE, you can pass `code_challenge_method=None` when initializing your `OAuth2Client`.
+
+#### Validating the Authorization Response
+
+Once you have redirected the user browser to the Authorization Request URI, and after the user is successfully
+authenticated and authorized, plus any other extra interactive step is complete, the AS will respond with a redirection
+to your redirect_uri. That is the *Authorization Response*. It contains several parameters that must be retrieved by
+your client. The *Authorization Code* is one of those parameters, but you must also validate that the *state* matches
+your request. You can do this with:
+
+```python
+# using the `az_request` as defined above
+
+response_uri = input(
+    "Please enter the full url and/or params obtained on the redirect_uri: "
+)
+az_response = az_request.validate_callback(response_uri)
+```
+
+This auth_response is an `AuthorizationResponse` instance and contains everything that is needed for your application to
+complete the authentication and get its tokens from the AS.
+
+#### Exchanging code for tokens
+
+Once you have obtained the AS response, containing an authorization code, your application must exchange it for actual
+Token(s).
+
+To exchange a code for Access and/or ID tokens, use the
+[OAuth2Client.authorization_code()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.authorization_code)
+method. If you have obtained an AuthorizationResponse as described above, you can simply do:
+
+```python
+token = oauth2client.authorization_code(az_response)
+```
+
+This will automatically include the `code`, `redirect_uri` and `code_verifier` parameters in the Token Request, as
+expected by the AS. You may include extra parameters if required, or you may pass your own parameters, without using an
+`AuthorizationResponse` instance, like this:
+
+```python
+token = oauth2client.authorization_code(
+    code=code,
+    code_verifier=code_verifier,
+    redirect_uri=redirect_uri,
+    custom_param=custom_value,
+)
+```
+
+#### As Auth Handler
+
+The
+[OAuth2AuthorizationCodeAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2AuthorizationCodeAuth)
+handler takes an [OAuth2Client] and an authorization code as parameter, plus whatever additional keyword parameters are
+required by your Authorization Server:
+
+```python
+from requests_oauth2client import OAuth2Client, ApiClient, OAuth2AuthorizationCodeAuth
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    authorization_endpoint="https://url.to.the/authorization_endpoint",
+    auth=("client_id", "client_secret"),
+)
+
+api_client = ApiClient(
+    "https://your.protected.api/endpoint",
+    auth=OAuth2AuthorizationCodeAuth(
+        oauth2client,
+        "my_authorization_code",
+    ),
+)
+
+# any request using api_client will trigger exchanging the code for an access_token, which is then cached, and refreshed later if needed
+resp = api_client.post(data={...})
+```
+
+[OAuth2AuthorizationCodeAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2AuthorizationCodeAuth)
+will take care of refreshing the token automatically once it is expired, using the refresh token, if available.
+
+### Note on AuthorizationRequest
+
+Authorization Requests generated by `OAuth2Client.authorization_request()` are instance of the class
+[`AuthorizationRequest`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.authorization_request.AuthorizationRequest).
+You can also use that class directly to generate your requests, but in that case you need to supply your Authorization
+Endpoint URI, your `client_id`, `redirect_uri`, etc. You can access every parameter from an `AuthorizationRequest`
+instance, as well as the generated `code_verifier`, as attributes of this instance. Once an Authorization Request URL is
+generated, it your application responsibility to redirect or otherwise send the user to that URL. You may use the
+`webbrowser` module from Python standard library to do so. Here is an example for generating Authorization Requests:
+
+```python
+from requests_oauth2client import AuthorizationRequest
+
+az_request = AuthorizationRequest(
+    "https://url.to.the/authorization_endpoint",
+    client_id="my_client_id",
+    redirect_uri="http://localhost/callback",  # this redirect_uri is specific to your app
+    scope="openid email profile",
+    # extra parameters such as `resource` can be included as well if required by your AS
+    resource="https://my.resource.local/api",
+)
+print(
+    az_request
+)  # this request will look like this, with line breaks for display purposes only
+# https://url.to.the/authorization_endpoint
+# ?client_id=my_client_id
+# &redirect_uri=http%3A%2F%2Flocalhost%callback
+# &response_type=code
+# &state=kHWL4VwcbUbtPR4mtht6yMAGG_S-ZcBh5RxI_IGDmJc
+# &nonce=mSGOS1M3LYU9ncTvvutoqUR4n1EtmaC_sQ3db4dyMAc
+# &scope=openid+email+profile
+# &code_challenge=W3n02f6xUKoDVbmhWEWz3h780b-Ci6ucnBS_d7nogmQ
+# &code_challenge_method=S256
+# &resource=https%3A%2F%2Fmy.resource.local%2Fapi
+
+print(az_request.code_verifier)
+# 'gYK-ZnQfoat2bghwed7oEz--wvn4D70ksJ5GuWO9sXXygZ7PMnUlSpBmMCcNRHxdgTS9m_roYwGxF6HQxIqZVwXmxRJUziFHUFxDrNuUIjCJCx6gBhPlpFbUXulB1fo2'
+```
+
+### Device Authorization Grant
+
+Helpers for the Device Authorization Grant are also included. To get device and user codes, read the response attributes
+(including Device Code, User Code, Verification URI, etc.), then pooling the Token Endpoint:
+
+```python
+from requests_oauth2client import (
+    OAuth2Client,
+    DeviceAuthorizationPoolingJob,
+    BearerToken,
+)
+
+client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    device_authorization_endpoint="https://url.to.the/device_authorization_endpoint",
+    auth=("client_id", "client_secret"),
+)
+
+da_resp = client.authorize_device()
+
+# `da_resp` contains the Device Code, User Code, Verification URI and other info returned by the AS:
+da_resp.device_code
+da_resp.user_code
+da_resp.verification_uri
+da_resp.verification_uri_complete
+da_resp.expires_at  # just like for BearerToken, expiration is tracked by requests_oauth2client
+da_resp.interval
+
+# Send/show the Verification Uri and User Code to the user. He must use a browser to visit that url, authenticate and
+# input the User Code.
+
+# You can then request the Token endpoint to check if the user successfully authorized your device like this:
+pool_job = DeviceAuthorizationPoolingJob(client, da_resp)
+
+resp = None
+while resp is None:
+    resp = pool_job()
+
+assert isinstance(resp, BearerToken)
+```
+
+[DeviceAuthorizationPoolingJob](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.device_authorization.DeviceAuthorizationPoolingJob)
+will automatically obey the pooling period. Everytime you call `pool_job()`, it will wait the appropriate number of
+seconds as indicated by the AS, and will apply slow_down requests.
+
+#### As Auth Handler
+
+Use
+[OAuth2DeviceCodeAuth](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.OAuth2DeviceCodeAuth)
+as auth handler to exchange a device code for an access token:
+
+```python
+from requests_oauth2client import ApiClient, OAuth2DeviceCodeAuth, OAuth2Client
+
+client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    device_authorization_endpoint="https://url.to.the/device_authorization_endpoint",
+    auth=("client_id", "client_secret"),
+)
+
+device_auth_resp = client.authorize_device()
+
+# expose user_code and verification_uri or verification_uri_complete to the user
+device_auth_resp.user_code
+device_auth_resp.verification_uri
+device_auth_resp.verification_uri_complete
+
+# then try to send your request with a OAuth2DeviceCodeAuth handler
+# this will pool the token endpoint until the user authorize the device
+api_client = ApiClient(
+    "https://your.protected.api/endpoint",
+    auth=OAuth2DeviceCodeAuth(client, device_auth_resp),
+)
+
+resp = api_client.post(
+    data={...}
+)  # first call will hang until the user authorizes your app and the token endpoint returns a token.
+```
+
+### Client-Initiated BackChannel Authentication (CIBA)
+
+To initiate a BackChannel Authentication against the dedicated endpoint, read the response attributes, and pool the
+Token Endpoint until the end-user successfully authenticates:
+
+```python
+from requests_oauth2client import (
+    OAuth2Client,
+    BearerToken,
+    BackChannelAuthenticationPoolingJob,
+)
+
+client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    backchannel_authentication_endpoint="https://url.to.the/backchannel_authorization_endpoint",
+    auth=("client_id", "client_secret"),
+)
+
+ba_resp = client.backchannel_authentication_request(
+    scope="openid email profile",
+    login_hint="user@example.net",
+)
+
+# `ba_resp` will contain the response attributes as returned by the AS, including an `auth_req_id`:
+ba_resp.auth_req_id
+ba_resp.expires_in  # decreases as times fly
+ba_resp.expires_at  # a datetime to keep track of the expiration date, based on the "expires_in" returned by the AS
+ba_resp.interval  # the pooling interval indicated by the AS
+ba_resp.custom  # if the AS respond with additional attributes, they are also accessible
+
+pool_job = BackChannelAuthenticationPoolingJob(client, ba_resp)
+
+resp = None
+while resp is None:
+    resp = pool_job()
+
+assert isinstance(resp, BearerToken)
+```
+
+Hints by the AS to slow down pooling will automatically be obeyed.
+
+### Token Exchange
+
+To send a token exchange request, use the
+[OAuth2Client.token_exchange()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.token_exchange)
+method:
+
+```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
+token = client.token_exchange(
+    subject_token="your_token_value",
+    subject_token_type="urn:ietf:params:oauth:token-type:access_token",
+)
+```
+
+As with the other grant-type specific methods, you may specify additional keyword parameters, that will be passed to the
+token endpoint, including any standardised attribute like `actor_token` or `actor_token_type`, or any custom parameter.
+There are short names for token types, that will be automatically translated to standardised types:
+
+```python
+token = client.token_exchange(
+    subject_token="your_token_value",
+    subject_token_type="access_token",  # will be automatically replaced by "urn:ietf:params:oauth:token-type:access_token"
+    actor_token="your_actor_token",
+    actor_token_type="id_token",  # will be automatically replaced by "urn:ietf:params:oauth:token-type:id_token"
+)
+```
+
+Or to make it even easier, types can be guessed based on the supplied subject or actor token:
+
+```python
+from requests_oauth2client import BearerToken, ClientSecretJwt, IdToken, OAuth2Client
+
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
+
+token = client.token_exchange(
+    subject_token=BearerToken(
+        "your_token_value"
+    ),  # subject_token_type will be "urn:ietf:params:oauth:token-type:access_token"
+    actor_token=IdToken(
+        "your_actor_token"
+    ),  # actor_token_type will be "urn:ietf:params:oauth:token-type:id_token"
+)
+```
+
+## Supported Client Authentication Methods
+
+`requests_oauth2client` supports several client authentication methods, as defined in multiple OAuth2.x standards. You
+select the appropriate method to use when initializing your [OAuth2Client], with the `auth` parameter. Once initialized,
+a client will automatically use the configured authentication method every time it sends a requested to an endpoint that
+requires client authentication. You don't have anything else to do afterwards.
+
+### Client Secret Basic
+
+With **client_secret_basic**, `client_id` and `client_secret` are included in clear-text in the `Authorization` header
+when sending requests to the Token Endpoint. To use it, just pass a
+[`ClientSecretBasic(client_id, client_secret)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.ClientSecretBasic)
+as `auth` parameter:
+
+```python
+from requests_oauth2client import OAuth2Client, ClientSecretBasic
+
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretBasic("client_id", "client_secret"),
+)
+```
+
+### Client Secret Post
+
+With **client_secret_post**, `client_id` and `client_secret` are included as part of the body form data. To use it, pass
+a
+[`ClientSecretPost(client_id, client_secret)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.ClientSecretPost)
+as `auth` parameter. This is the default when you pass a tuple `(client_id, client_secret)` as `auth` when initializing
+an `OAuth2Client`:
+
+```python
+from requests_oauth2client import OAuth2Client, ClientSecretPost
+
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretPost("client_id", "client_secret"),
+)
+# or
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint", auth=("client_id", "client_secret")
+)
+# or
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    client_id="my_client_id",
+    client_secret="my_client_secret",
+)
+```
+
+### Client Secret JWT
+
+With **client_secret_jwt**, the client generates an ephemeral JWT assertion including information about itself
+(client_id), the AS (url of the endpoint), and an expiration date a few seconds in the future. To use it, pass a
+[`ClientSecretJwt(client_id, client_secret)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.ClientSecretJwt)
+as `auth` parameter. Assertion generation is entirely automatic, you don't have anything to do:
+
+```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
+```
+
+This method is more secure than the 2 previous, because only ephemeral credentials are transmitted, which limits the
+possibility for interception and replay of the Client Secret. But that Client Secret still needs to be shared between
+the AS and Client owner(s).
+
+### Private Key JWT
+
+With **private_key_jwt**, client uses a JWT assertion that is just like the one for _client_secret_jwt_, but it is
+signed with an _asymmetric_ key. To use it, you need a private signing key, in a `dict` that matches the JWK format, or
+as an instance of `jwskate.Jwk`. The matching public key must be registered for your client on AS side. Once you have
+that, using this auth method is simple with the
+[`PrivateKeyJwt(client_id, private_jwk)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.PrivateKeyJwt)
+auth handler:
+
+```python
+from requests_oauth2client import OAuth2Client, PrivateKeyJwt
+
+private_jwk = {
+    "kid": "mykid",
+    "kty": "RSA",
+    "e": "AQAB",
+    "n": "...",
+    "d": "...",
+    "p": "...",
+    "q": "...",
+    "dp": "...",
+    "dq": "...",
+    "qi": "...",
 }
 
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint", auth=PrivateKeyJwt("client_id", private_jwk)
+)
+# or
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint", auth=("client_id", private_jwk)
+)
+# or
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint", client_id="client_id", private_jwk=private_jwk
+)
+```
+
+This method can be considered more secure than those relying on a client secret, because only ephemeral credentials are
+sent over the wire, and it uses asymmetric cryptography: the signing key is generated by the client, and only the public
+key is known by the AS. Transmitting that public key between owner(s) of the client and of the AS is much easier than
+transmitting the Client Secret, which is a shared key that must be considered as confidential.
+
+### None
+
+The latest Client Authentication Method, **none**, is for Public Clients which do not authenticate to the Token
+Endpoint. Those clients only include their `client_id` in body form data, without any authentication credentials. Use
+[`PublicApp(client_id)`](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client_authentication.PublicApp):
+
+```python
+from requests_oauth2client import OAuth2Client, PublicApp
+
+client = OAuth2Client(
+    "https://url.to.the/token_endpoint", auth=PublicApp("app_client_id")
+)
+```
+
+## Token Revocation
+
+[OAuth2Client] can send revocation requests to a Revocation Endpoint. You need to provide a Revocation Endpoint URI when
+creating the [OAuth2Client]. The
+[OAuth2Client.revoke_token()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.revoke_token)
+method and its specialized aliases
+[.revoke_access_token()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.revoke_access_token)
+and
+[.revoke_refresh_token()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.revoke_refresh_token)
+are then available:
+
+```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    revocation_endpoint="https://url.to.the/revocation_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
+
+oauth2client.revoke_token("mytoken", token_type_hint="access_token")
+oauth2client.revoke_access_token(
+    "mytoken"
+)  # will automatically add token_type_hint=access_token
+oauth2client.revoke_refresh_token(
+    "mytoken"
+)  # will automatically add token_type_hint=refresh_token
+```
+
+Because Revocation Endpoints usually don't return meaningful responses, those methods return a boolean. This boolean
+indicates that a request was successfully sent and no error was returned. If the Authorization Server returns a
+non-successful HTTP code, but no standardised error message, it will return `False`. If the Authorization Server
+actually returns a standardised error, an exception will be raised instead, like the other methods from `OAuth2Client`.
+
+## Token Introspection
+
+[OAuth2Client] can send requests to a Token Introspection Endpoint. You need to provide an Introspection Endpoint URI
+when creating the `OAuth2Client`. The
+[OAuth2Client.introspect_token()](<https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.instrospect_token()>)
+method is then available:
+
+```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    introspection_endpoint="https://url.to.the/introspection_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
+
+resp = oauth2client.introspect_token("mytoken", token_type_hint="access_token")
+```
+
+It returns whatever data is returned by the introspection endpoint (if it is a JSON, its content is returned decoded).
+
+## UserInfo Requests
+
+[OAuth2Client] can send requests to an UserInfo Endpoint. You need to provide an UserInfo Endpoint URI when creating the
+`OAuth2Client`. The
+[OAuth2Client.userinfo()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.userinfo))
+method is then available:
+
+```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
+oauth2client = OAuth2Client(
+    token_endpoint="https://url.to.the/token_endpoint",
+    userinfo_endpoint="https://url.to.the/userinfo_endpoint",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
+resp = oauth2client.userinfo("mytoken")
+```
+
+It returns whatever data is returned by the userinfo endpoint (if it is a JSON, its content is returned decoded).
+
+## Initializing an OAuth2Client from a discovery document
+
+You can initialize an [OAuth2Client] with the endpoint URIs mentioned in a standardised discovery document with the
+[OAuth2Client.from_discovery_endpoint()](https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client.from_discovery_document)
+class method:
+
+```python
+from requests_oauth2client import OAuth2Client, ClientSecretJwt
+
+oauth2client = OAuth2Client.from_discovery_endpoint(
+    "https://url.to.the/.well-known/openid-configuration",
+    auth=ClientSecretJwt("client_id", "client_secret"),
+)
+```
+
+This will fetch the document from the specified URI, then will decode it and initialize an [OAuth2Client] pointing to
+the appropriate endpoint URIs.
+
+## Specialized API Client
+
+Using APIs usually involves multiple endpoints under the same root url, with a common authentication method. To make it
+easier, `requests_oauth2client` includes a [requests.Session] wrapper called [ApiClient], which takes the root API url
+as parameter on initialization. You can then send requests to different endpoints by passing their relative path instead
+of the full url. [ApiClient] also accepts an `auth` parameter with an AuthHandler. You can pass any of the OAuth2 Auth
+Handler from this module, or any [requests]-compatible
+[Authentication Handler](https://requests.readthedocs.io/en/latest/user/advanced/#custom-authentication). Which makes it
+very easy to call APIs that are protected with an OAuth2 Client Credentials Grant:
+
+```python
+from requests_oauth2client import OAuth2Client, ApiClient, OAuth2ClientCredentialsAuth
+
+oauth2client = OAuth2Client(
+    "https://url.to.the/token_endpoint", ("client_id", "client_secret")
+)
+api = ApiClient(
+    "https://myapi.local/root", auth=OAuth2ClientCredentialsAuth(oauth2client)
+)
+
+# will actually send a GET to https://myapi.local/root/resource/foo
+resp = api.get("/resource/foo")
+```
+
+Note that [ApiClient] will never send requests "outside" its configured root url, unless you specifically give it a full
+url at request time. The leading `/` in `/resource` above is optional. A leading `/` will not "reset" the url path to
+root, which means that you can also write the relative path without the `/` and it will automatically be included:
+
+```python
+api.get("resource/foo")  # will also send a GET to https://myapi.local/root/resource/foo
+```
+
+You may also pass the path as an iterable of strings (or string-able objects), in which case they will be joined with a
+`/` and appended to the url path:
+
+```python
+# will send a GET to https://myapi.local/root/resource/foo
+api.get(["resource", "foo"])
+# will send a GET to https://myapi.local/root/users/1234/details
+api.get(["users", 1234, "details"])
+```
+
+You can also use a syntax based on `__getattr__` or `__getitem__`:
+
+```python
+api.resource.get()  # will send a GET to https://myapi.local/root/resource
+api["my-resource"].get()  # will send a GET to https://myapi.local/root/my-resource
+```
+
+Both `__getattr__` and `__getitem__` return a new `ApiClient` initialised on the new base_url. So you can easily call
+multiple sub-resources on the same API this way:
+
+```python
+from requests_oauth2client import ApiClient
+
+api = ApiClient("https://myapi.local")
+users_api = api.users
+user = users_api.get("userid")  # GET https://myapi.local/users/userid
+other_user = users_api.get("other_userid")  # GET https://myapi.local/users/other_userid
+resources_api = api.resources
+resources = resources_api.get()  # GET https://myapi.local/resources
+```
+
+[ApiClient] will, by default, raise exceptions whenever a request returns an error status. You can disable that by
+passing `raise_for_status=False` when initializing your [ApiClient]:
+
+```python
+from requests_oauth2client import ApiClient
+
+api = ApiClient(
+    "http://httpstat.us", raise_for_status=False
+)  # raise_for_status defaults to True
+resp = api.get("500")
+assert resp is not None
+# without raise_for_status=False, a requests.exceptions.HTTPError exception would be raised instead
+```
+
+You may override this at request time:
+
+```python
+# raise_for_status at request-time overrides the value defined at init-time
+resp = api.get("500", raise_for_status=True)
+```
+
+You can access the underlying `requests.Session` with the session attribute, and you can provide an already existing and
+configured `Session` instance at init time:
+
+```python
+import requests
+from requests_oauth2client import ApiClient
+
+session = requests.Session()
+session.proxies = {"https": "http://localhost:3128"}
+api = ApiClient("https://myapi.local/resource", session=session)
+assert api.session == session
+```
+
+## Vendor-Specific clients
+
+`requests_oauth2client` being flexible enough to handle most use cases, you should be able to use any AS by any vendor
+as long as it supports OAuth 2.0.
+
+You can however create a subclass of [OAuth2Client] or [ApiClient] to make it easier to use with specific Authorization
+Servers or APIs. The sub-module `requests_oauth2client.vendor_specific` includes such classes for
+[Auth0](https://auth0.com):
+
+```python
+from requests_oauth2client.vendor_specific import Auth0Client, Auth0ManagementApiClient
+
+a0client = Auth0Client("mytenant.eu", ("client_id", "client_secret"))
+# this will automatically initialize the token endpoint to https://mytenant.eu.auth0.com/oauth/token
+# and other endpoints accordingly
+token = a0client.client_credentials(audience="audience")
+
+# this is a wrapper around Auth0 Management API
+a0mgmt = Auth0ManagementApiClient("mytenant.eu", ("client_id", "client_secret"))
+myusers = a0mgmt.get("users")
+```
 
-setup(**setup_kwargs)
+[apiclient]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.api_client.ApiClient
+[bearerauth]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.auth.BearerAuth
+[bearertoken]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.tokens.BearerToken
+[oauth2client]: https://guillp.github.io/requests_oauth2client/api/#requests_oauth2client.client.OAuth2Client
+[requests]: https://requests.readthedocs.io/en/latest/
+[requests.session]: https://requests.readthedocs.io/en/latest/api/#requests.Session
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

