# Comparing `tmp/flask_cognito_lib-1.4.1.tar.gz` & `tmp/flask_cognito_lib-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_cognito_lib-1.4.1.tar", max compression
+gzip compressed data, was "flask_cognito_lib-1.5.0.tar", max compression
```

## Comparing `flask_cognito_lib-1.4.1.tar` & `flask_cognito_lib-1.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/LICENSE
--rw-r--r--   0        0        0     7676 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/README.md
--rw-r--r--   0        0        0     2278 2023-07-08 10:57:01.203231 flask_cognito_lib-1.4.1/pyproject.toml
--rw-r--r--   0        0        0       82 2023-07-08 10:57:01.183231 flask_cognito_lib-1.4.1/src/flask_cognito_lib/__init__.py
--rw-r--r--   0        0        0     4687 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/config.py
--rw-r--r--   0        0        0     6129 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/decorators.py
--rw-r--r--   0        0        0      384 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/exceptions.py
--rw-r--r--   0        0        0     5995 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/plugin.py
--rw-r--r--   0        0        0      326 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/__init__.py
--rw-r--r--   0        0        0     3820 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/cognito_svc.py
--rw-r--r--   0        0        0     5802 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/token_svc.py
--rw-r--r--   0        0        0     1124 2023-07-08 10:56:40.099217 flask_cognito_lib-1.4.1/src/flask_cognito_lib/utils.py
--rw-r--r--   0        0        0     9063 1970-01-01 00:00:00.000000 flask_cognito_lib-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/LICENSE
+-rw-r--r--   0        0        0     8071 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/README.md
+-rw-r--r--   0        0        0     2278 2023-07-12 09:38:49.400958 flask_cognito_lib-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-07-12 09:38:49.376958 flask_cognito_lib-1.5.0/src/flask_cognito_lib/__init__.py
+-rw-r--r--   0        0        0     4687 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/src/flask_cognito_lib/config.py
+-rw-r--r--   0        0        0     6314 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/src/flask_cognito_lib/decorators.py
+-rw-r--r--   0        0        0      384 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/src/flask_cognito_lib/exceptions.py
+-rw-r--r--   0        0        0     5995 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/src/flask_cognito_lib/plugin.py
+-rw-r--r--   0        0        0      326 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/src/flask_cognito_lib/services/__init__.py
+-rw-r--r--   0        0        0     3820 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/src/flask_cognito_lib/services/cognito_svc.py
+-rw-r--r--   0        0        0     5802 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/src/flask_cognito_lib/services/token_svc.py
+-rw-r--r--   0        0        0     1124 2023-07-12 09:38:24.352508 flask_cognito_lib-1.5.0/src/flask_cognito_lib/utils.py
+-rw-r--r--   0        0        0     9458 1970-01-01 00:00:00.000000 flask_cognito_lib-1.5.0/PKG-INFO
```

### Comparing `flask_cognito_lib-1.4.1/LICENSE` & `flask_cognito_lib-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.1/README.md` & `flask_cognito_lib-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,24 @@
     # If their auth is valid, the set of groups the user is a member of will be
     # shown.
 
     # Could also use: jsonify(session["user_info"]["cognito:groups"])
     return jsonify(session["claims"]["cognito:groups"])
 
 
+@app.route("/edit")
+@auth_required(groups=["admin", "editor"], any_group=True)
+def edit():
+    # This route will only be accessible to a user who is a member of any of
+    # groups specified in the "groups" argument on the auth_required decorator
+    # If they are not, a CognitoGroupRequiredError is raised which is handled
+    # below
+    return jsonify(session["claims"]["cognito:groups"])
+
+
 @app.route("/logout")
 @cognito_logout
 def logout():
     # Logout of the Cognito User pool and delete the cookies that were set
     # on login.
     # No logic is required here as it simply redirects to Cognito.
     pass
```

### Comparing `flask_cognito_lib-1.4.1/pyproject.toml` & `flask_cognito_lib-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask_cognito_lib"
-version = "1.4.1"
+version = "1.5.0"
 description = "A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices"
 license = "MIT"
 authors = ["mblackgeo <18327836+mblackgeo@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/mblackgeo/flask-cognito-lib"
 repository = "https://github.com/mblackgeo/flask-cognito-lib"
 keywords = ["Flask", "Extension", "OAuth", "Cognito"]
```

### Comparing `flask_cognito_lib-1.4.1/src/flask_cognito_lib/config.py` & `flask_cognito_lib-1.5.0/src/flask_cognito_lib/config.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.1/src/flask_cognito_lib/decorators.py` & `flask_cognito_lib-1.5.0/src/flask_cognito_lib/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         # Cognito will redirect to the sign-out URL (if set) or else use
         # the callback URL
         return resp
 
     return wrapper
 
 
-def auth_required(groups: Optional[Iterable[str]] = None):
+def auth_required(groups: Optional[Iterable[str]] = None, any_group: bool = False):
     """A decorator to protect a route with AWS Cognito"""
 
     def wrapper(fn):
         @wraps(fn)
         def decorator(*args, **kwargs):
             with app.app_context():
                 # return early if the extension is disabled
@@ -167,15 +167,19 @@
                         token=access_token,
                         leeway=cfg.cognito_expiration_leeway,
                     )
                     valid = True
 
                     # Check for required group membership
                     if groups:
-                        valid = all(g in claims["cognito:groups"] for g in groups)
+                        if any_group:
+                            valid = any(g in claims["cognito:groups"] for g in groups)
+                        else:
+                            valid = all(g in claims["cognito:groups"] for g in groups)
+
                         if not valid:
                             raise CognitoGroupRequiredError
 
                 except (TokenVerifyError, KeyError):
                     valid = False
 
                 if valid:
```

### Comparing `flask_cognito_lib-1.4.1/src/flask_cognito_lib/plugin.py` & `flask_cognito_lib-1.5.0/src/flask_cognito_lib/plugin.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/cognito_svc.py` & `flask_cognito_lib-1.5.0/src/flask_cognito_lib/services/cognito_svc.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.1/src/flask_cognito_lib/services/token_svc.py` & `flask_cognito_lib-1.5.0/src/flask_cognito_lib/services/token_svc.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.1/src/flask_cognito_lib/utils.py` & `flask_cognito_lib-1.5.0/src/flask_cognito_lib/utils.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.4.1/PKG-INFO` & `flask_cognito_lib-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-cognito-lib
-Version: 1.4.1
+Version: 1.5.0
 Summary: A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices
 Home-page: https://github.com/mblackgeo/flask-cognito-lib
 License: MIT
 Keywords: Flask,Extension,OAuth,Cognito
 Author: mblackgeo
 Author-email: 18327836+mblackgeo@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -133,14 +133,24 @@
     # If their auth is valid, the set of groups the user is a member of will be
     # shown.
 
     # Could also use: jsonify(session["user_info"]["cognito:groups"])
     return jsonify(session["claims"]["cognito:groups"])
 
 
+@app.route("/edit")
+@auth_required(groups=["admin", "editor"], any_group=True)
+def edit():
+    # This route will only be accessible to a user who is a member of any of
+    # groups specified in the "groups" argument on the auth_required decorator
+    # If they are not, a CognitoGroupRequiredError is raised which is handled
+    # below
+    return jsonify(session["claims"]["cognito:groups"])
+
+
 @app.route("/logout")
 @cognito_logout
 def logout():
     # Logout of the Cognito User pool and delete the cookies that were set
     # on login.
     # No logic is required here as it simply redirects to Cognito.
     pass
```

