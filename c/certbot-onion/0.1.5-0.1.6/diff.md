# Comparing `tmp/certbot-onion-0.1.5.tar.gz` & `tmp/certbot-onion-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-onion-0.1.5.tar", last modified: Thu Jun 29 12:39:28 2023, max compression
+gzip compressed data, was "certbot-onion-0.1.6.tar", last modified: Wed Jul 12 13:04:49 2023, max compression
```

## Comparing `certbot-onion-0.1.5.tar` & `certbot-onion-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.588712 certbot-onion-0.1.5/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/rust/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.588712 certbot-onion-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/src/certbot_onion/
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/src/certbot_onion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/src/certbot_onion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:49.416775 certbot-onion-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 13:04:39.000000 certbot-onion-0.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-12 13:04:39.000000 certbot-onion-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-12 13:04:49.416775 certbot-onion-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-12 13:04:39.000000 certbot-onion-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-12 13:04:39.000000 certbot-onion-0.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:49.416775 certbot-onion-0.1.6/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-12 13:04:39.000000 certbot-onion-0.1.6/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:49.416775 certbot-onion-0.1.6/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-12 13:04:39.000000 certbot-onion-0.1.6/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:04:49.416775 certbot-onion-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-12 13:04:39.000000 certbot-onion-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:49.412775 certbot-onion-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:49.416775 certbot-onion-0.1.6/src/certbot_onion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-12 13:04:39.000000 certbot-onion-0.1.6/src/certbot_onion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:49.416775 certbot-onion-0.1.6/src/certbot_onion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-12 13:04:49.000000 certbot-onion-0.1.6/src/certbot_onion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-12 13:04:49.000000 certbot-onion-0.1.6/src/certbot_onion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:04:49.000000 certbot-onion-0.1.6/src/certbot_onion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 13:04:49.000000 certbot-onion-0.1.6/src/certbot_onion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:04:49.000000 certbot-onion-0.1.6/src/certbot_onion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 13:04:49.000000 certbot-onion-0.1.6/src/certbot_onion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 13:04:49.000000 certbot-onion-0.1.6/src/certbot_onion.egg-info/top_level.txt
```

### Comparing `certbot-onion-0.1.5/LICENSE.md` & `certbot-onion-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.5/PKG-INFO` & `certbot-onion-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.5
+Version: 0.1.6
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `certbot-onion-0.1.5/README.md` & `certbot-onion-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.5/pyproject.toml` & `certbot-onion-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "certbot-onion"
-version = "0.1.5"
+version = "0.1.6"
 description = "Certbot authenticator plugin for the onion-csr-01 challenge"
 authors = [
     {name = "Q Misell", email = "q@as207960.net"}
 ]
 license = {text = "MIT"}
 dependencies = [
     "certbot>=2.6.0"
```

### Comparing `certbot-onion-0.1.5/rust/src/lib.rs` & `certbot-onion-0.1.6/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.5/src/certbot_onion/__init__.py` & `certbot-onion-0.1.6/src/certbot_onion/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,18 +44,20 @@
     def __init__(self, *args, **kwargs):
         self.hs = []
 
         super().__init__(*args, **kwargs)
 
     @classmethod
     def add_parser_arguments(cls, add: typing.Callable[..., None]) -> None:
-        add("hs-dir", help="Path to a Tor hidden service directory", nargs="+", required=True)
+        add("hs-dir", help="Path to a Tor hidden service directory", nargs="+", required=False)
 
     def prepare(self) -> None:
-        for hs_dir in self.conf("hs-dir"):
+        hs_dirs = self.conf("hs-dir")
+        hs_dirs = hs_dirs if hs_dirs is not None else []
+        for hs_dir in hs_dirs:
             if not os.path.isdir(hs_dir):
                 raise certbot.errors.PluginError(f"Hidden service directory path {hs_dir} is not a directory")
 
             hostname_path = os.path.join(hs_dir, "hostname")
             private_key_path = os.path.join(hs_dir, "hs_ed25519_secret_key")
 
             if not os.path.isfile(hostname_path):
```

### Comparing `certbot-onion-0.1.5/src/certbot_onion.egg-info/PKG-INFO` & `certbot-onion-0.1.6/src/certbot_onion.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.5
+Version: 0.1.6
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

