# Comparing `tmp/gdash-1.1.6.tar.gz` & `tmp/gdash-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdash-1.1.6.tar", last modified: Thu Jun 29 14:12:41 2023, max compression
+gzip compressed data, was "gdash-1.1.7.tar", last modified: Wed Jul 12 06:53:24 2023, max compression
```

## Comparing `gdash-1.1.6.tar` & `gdash-1.1.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:12:41.187402 gdash-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-29 14:11:34.000000 gdash-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-29 14:11:34.000000 gdash-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-29 14:12:41.187402 gdash-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-29 14:11:34.000000 gdash-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:12:41.183402 gdash-1.1.6/gdash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:11:34.000000 gdash-1.1.6/gdash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-29 14:11:34.000000 gdash-1.1.6/gdash/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:12:41.187402 gdash-1.1.6/gdash/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-29 14:12:39.000000 gdash-1.1.6/gdash/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-29 14:12:39.000000 gdash-1.1.6/gdash/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-29 14:12:22.000000 gdash-1.1.6/gdash/ui/logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-29 14:12:22.000000 gdash-1.1.6/gdash/ui/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-29 14:12:22.000000 gdash-1.1.6/gdash/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 14:12:22.000000 gdash-1.1.6/gdash/ui/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:12:41.183402 gdash-1.1.6/gdash/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:12:41.187402 gdash-1.1.6/gdash/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-06-29 14:12:39.000000 gdash-1.1.6/gdash/ui/static/css/main.bb354ed4.css
--rw-r--r--   0 runner    (1001) docker     (123)    22664 2023-06-29 14:12:39.000000 gdash-1.1.6/gdash/ui/static/css/main.bb354ed4.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:12:41.187402 gdash-1.1.6/gdash/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-06-29 14:12:39.000000 gdash-1.1.6/gdash/ui/static/js/main.c4611ae3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-29 14:12:39.000000 gdash-1.1.6/gdash/ui/static/js/main.c4611ae3.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   912003 2023-06-29 14:12:39.000000 gdash-1.1.6/gdash/ui/static/js/main.c4611ae3.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:12:41.187402 gdash-1.1.6/gdash/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    20692 2023-06-29 14:12:39.000000 gdash-1.1.6/gdash/ui/static/media/bg1.434ec9b5178c983b027e73e271858301.svg
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 14:11:46.000000 gdash-1.1.6/gdash/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:12:41.183402 gdash-1.1.6/gdash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-29 14:12:41.000000 gdash-1.1.6/gdash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-29 14:12:41.000000 gdash-1.1.6/gdash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:12:41.000000 gdash-1.1.6/gdash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 14:12:41.000000 gdash-1.1.6/gdash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:12:41.000000 gdash-1.1.6/gdash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 14:12:41.000000 gdash-1.1.6/gdash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 14:12:41.000000 gdash-1.1.6/gdash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 14:12:41.187402 gdash-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-29 14:11:34.000000 gdash-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:53:24.462367 gdash-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-12 06:52:33.000000 gdash-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 06:52:33.000000 gdash-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 06:53:24.462367 gdash-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-12 06:52:33.000000 gdash-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:53:24.458366 gdash-1.1.7/gdash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 06:52:33.000000 gdash-1.1.7/gdash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-12 06:52:33.000000 gdash-1.1.7/gdash/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:53:24.462367 gdash-1.1.7/gdash/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-12 06:53:23.000000 gdash-1.1.7/gdash/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-12 06:53:23.000000 gdash-1.1.7/gdash/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-12 06:53:09.000000 gdash-1.1.7/gdash/ui/logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-12 06:53:09.000000 gdash-1.1.7/gdash/ui/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-12 06:53:09.000000 gdash-1.1.7/gdash/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 06:53:09.000000 gdash-1.1.7/gdash/ui/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:53:24.458366 gdash-1.1.7/gdash/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:53:24.462367 gdash-1.1.7/gdash/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-07-12 06:53:23.000000 gdash-1.1.7/gdash/ui/static/css/main.bb354ed4.css
+-rw-r--r--   0 runner    (1001) docker     (123)    22664 2023-07-12 06:53:23.000000 gdash-1.1.7/gdash/ui/static/css/main.bb354ed4.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:53:24.462367 gdash-1.1.7/gdash/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-07-12 06:53:23.000000 gdash-1.1.7/gdash/ui/static/js/main.c4611ae3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-12 06:53:23.000000 gdash-1.1.7/gdash/ui/static/js/main.c4611ae3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   912003 2023-07-12 06:53:23.000000 gdash-1.1.7/gdash/ui/static/js/main.c4611ae3.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:53:24.462367 gdash-1.1.7/gdash/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    20692 2023-07-12 06:53:23.000000 gdash-1.1.7/gdash/ui/static/media/bg1.434ec9b5178c983b027e73e271858301.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 06:52:42.000000 gdash-1.1.7/gdash/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:53:24.458366 gdash-1.1.7/gdash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 06:53:24.000000 gdash-1.1.7/gdash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 06:53:24.000000 gdash-1.1.7/gdash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 06:53:24.000000 gdash-1.1.7/gdash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 06:53:24.000000 gdash-1.1.7/gdash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 06:53:24.000000 gdash-1.1.7/gdash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 06:53:24.000000 gdash-1.1.7/gdash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 06:53:24.000000 gdash-1.1.7/gdash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 06:53:24.462367 gdash-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-12 06:52:33.000000 gdash-1.1.7/setup.py
```

### Comparing `gdash-1.1.6/LICENSE` & `gdash-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/PKG-INFO` & `gdash-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdash
-Version: 1.1.6
+Version: 1.1.7
 Summary: GlusterFS Dashboard
 Home-page: https://github.com/kadalu/gdash
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: Apache-2.0
 Keywords: glusterfs,gui,dashboard
 Platform: linux
```

### Comparing `gdash-1.1.6/README.md` & `gdash-1.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 **Note**: Port can be customized by providing `--port` option(For example, `--port 3000`)
 
 Other available options are
 
 ```
 $ gdash --help
 usage: gdash [-h] [--version] [--port PORT] [--gluster-binary GLUSTER_BINARY]
-             [--auth-file AUTH_FILE] [--ssl-cert CERT_FILE] [--ssl-key KEY_FILE] [--ssl-ca CA_CERT_FILE]
+             [--auth-file AUTH_FILE] [--ssl-cert CERT_FILE] [--ssl-key KEY_FILE] [--ssl-ca CA_CERT_FILE] [--ssl-ciphers LIST_OF_CIPHERS]
              host
 
 gdash - GlusterFS Dashboard
 
 positional arguments:
   host                  Hostname of Current node as used in Gluster peer
                         commands. Gdash replaces the "localhost" references
@@ -64,14 +64,15 @@
   --gluster-binary GLUSTER_BINARY  Gluster binary path.
   --auth-file AUTH_FILE            Users Credentials file. One user
                                    entry per row in the
                                    format <username>=<password_hash>
   --ssl-cert CERT_FILE             Path to SSL Certificate file
   --ssl-key KEY_FILE               Path to SSL Key file
   --ssl-ca CA_FILE                 Path to SSL CA Certificate file
+  --ssl-ciphers                    List of SSL Ciphers to allow
 ```
 
 ## Blog
 
 * [Dec 04, 2014] http://aravindavk.in/blog/introducing-gdash (Previous version, UI is different now)
 * [Oct 19, 2020] https://kadalu.io/blog/gdash-v1.0
```

### Comparing `gdash-1.1.6/gdash/__main__.py` & `gdash-1.1.7/gdash/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,24 +19,29 @@
         "tools.response_headers.headers": [("Content-Type", "application/json")],
         "tools.caching.on": True,
         "tools.caching.delay": 5,
     },
     "/": {
         "tools.staticdir.on": True,
         "tools.sessions.on": True,
-        "tools.sessions.secure" = True,
-        "tools.sessions.httponly" = True,
-        "tools.secureheaders.on" = True,
-        "tools.staticdir.dir": os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "ui"
-        ),
+        "tools.sessions.secure": True,
+        "tools.sessions.httponly": True,
+        "tools.secureheaders.on": True,
+        "tools.staticdir.dir": os.path.join(os.path.dirname(os.path.abspath(__file__)), "ui"),
     },
 }
 
 
+def secureheaders():
+    headers = cherrypy.response.headers
+    headers["X-Frame-Options"] = "DENY"
+    headers["X-XSS-Protection"] = "1; mode=block"
+    headers["Content-Security-Policy"] = "default-src='self'"
+
+
 def is_valid_admin_login(username, password):
     if USERS is None:
         return True
 
     pwd_hash = USERS.get(username, None)
     if pwd_hash is None:
         return False
@@ -158,32 +163,20 @@
             'peer commands. Gdash replaces the "localhost" '
             "references with this name"
         ),
     )
     parser.add_argument("--gluster-binary", default="gluster")
     parser.add_argument(
         "--auth-file",
-        help=(
-            "Users Credentials file. One user entry per row "
-            "in the format <username>=<password_hash>"
-        ),
-    )
-    parser.add_argument(
-        "--ssl-cert", default=None, help=("Path to SSL Certificate used by Gdash")
+        help=("Users Credentials file. One user entry per row " "in the format <username>=<password_hash>"),
     )
-    parser.add_argument(
-        "--ssl-key", default=None, help=("Path to SSL Key used by Gdash")
-    )
-    parser.add_argument(
-        "--ssl-ca", default=None, help=("Path to SSL CA Certificate used by Gdash")
-    )
-    parser.add_argument(
-        "--ssl-ciphers", default=None, help=("List of SSL Ciphers to allow")
-    )
-
+    parser.add_argument("--ssl-cert", default=None, help=("Path to SSL Certificate used by Gdash"))
+    parser.add_argument("--ssl-key", default=None, help=("Path to SSL Key used by Gdash"))
+    parser.add_argument("--ssl-ca", default=None, help=("Path to SSL CA Certificate used by Gdash"))
+    parser.add_argument("--ssl-ciphers", default=None, help=("List of SSL Ciphers to allow"))
     return parser.parse_args()
 
 
 def main():
     global ARGS, USERS
 
     ARGS = get_args()
@@ -213,14 +206,15 @@
     if ARGS.ssl_ciphers:
         cherrypy_cfg["server.ssl_ciphers"] = ARGS.ssl_ciphers
 
     if ARGS.ssl_cert and ARGS.ssl_key:
         cherrypy_cfg["server.ssl_module"] = "builtin"
 
     cherrypy.config.update(cherrypy_cfg)
+    cherrypy.tools.secureheaders = cherrypy.Tool("before_finalize", secureheaders, priority=60)
     webapp = GdashWeb()
     webapp.api = GdashApis()
     cherrypy.quickstart(webapp, "/", conf)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gdash-1.1.6/gdash/ui/index.html` & `gdash-1.1.7/gdash/ui/index.html`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/gdash/ui/logo-small.png` & `gdash-1.1.7/gdash/ui/logo-small.png`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/gdash/ui/logo.png` & `gdash-1.1.7/gdash/ui/logo.png`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/gdash/ui/static/css/main.bb354ed4.css` & `gdash-1.1.7/gdash/ui/static/css/main.bb354ed4.css`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/gdash/ui/static/css/main.bb354ed4.css.map` & `gdash-1.1.7/gdash/ui/static/css/main.bb354ed4.css.map`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/gdash/ui/static/js/main.c4611ae3.js` & `gdash-1.1.7/gdash/ui/static/js/main.c4611ae3.js`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/gdash/ui/static/js/main.c4611ae3.js.LICENSE.txt` & `gdash-1.1.7/gdash/ui/static/js/main.c4611ae3.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/gdash/ui/static/js/main.c4611ae3.js.map` & `gdash-1.1.7/gdash/ui/static/js/main.c4611ae3.js.map`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/gdash/ui/static/media/bg1.434ec9b5178c983b027e73e271858301.svg` & `gdash-1.1.7/gdash/ui/static/media/bg1.434ec9b5178c983b027e73e271858301.svg`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/gdash.egg-info/PKG-INFO` & `gdash-1.1.7/gdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdash
-Version: 1.1.6
+Version: 1.1.7
 Summary: GlusterFS Dashboard
 Home-page: https://github.com/kadalu/gdash
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: Apache-2.0
 Keywords: glusterfs,gui,dashboard
 Platform: linux
```

### Comparing `gdash-1.1.6/gdash.egg-info/SOURCES.txt` & `gdash-1.1.7/gdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdash-1.1.6/setup.py` & `gdash-1.1.7/setup.py`

 * *Files identical despite different names*

