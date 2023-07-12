# Comparing `tmp/qfieldcloud-sdk-0.6.1.tar.gz` & `tmp/qfieldcloud-sdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfieldcloud-sdk-0.6.1.tar", last modified: Tue Jun 21 13:54:22 2022, max compression
+gzip compressed data, was "qfieldcloud-sdk-0.7.0.tar", last modified: Wed Jul 12 11:31:01 2023, max compression
```

## Comparing `qfieldcloud-sdk-0.6.1.tar` & `qfieldcloud-sdk-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 13:54:22.946076 qfieldcloud-sdk-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-06-21 13:54:09.000000 qfieldcloud-sdk-0.6.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-06-21 13:54:22.946076 qfieldcloud-sdk-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2022-06-21 13:54:09.000000 qfieldcloud-sdk-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-21 13:54:09.000000 qfieldcloud-sdk-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-21 13:54:22.946076 qfieldcloud-sdk-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-21 13:54:09.000000 qfieldcloud-sdk-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 13:54:22.946076 qfieldcloud-sdk-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 13:54:22.946076 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-21 13:54:09.000000 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14396 2022-06-21 13:54:09.000000 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    23304 2022-06-21 13:54:09.000000 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 13:54:22.946076 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-06-21 13:54:22.000000 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-06-21 13:54:22.000000 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-21 13:54:22.000000 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-21 13:54:22.000000 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-21 13:54:22.000000 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-21 13:54:22.000000 qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:31:01.526840 qfieldcloud-sdk-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-07-12 11:30:53.000000 qfieldcloud-sdk-0.7.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-07-12 11:31:01.526840 qfieldcloud-sdk-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-07-12 11:30:53.000000 qfieldcloud-sdk-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-12 11:30:53.000000 qfieldcloud-sdk-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 11:31:01.526840 qfieldcloud-sdk-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-07-12 11:30:53.000000 qfieldcloud-sdk-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:31:01.526840 qfieldcloud-sdk-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:31:01.526840 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 11:30:53.000000 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    15006 2023-07-12 11:30:53.000000 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23659 2023-07-12 11:30:53.000000 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:31:01.526840 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-07-12 11:31:01.000000 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-12 11:31:01.000000 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 11:31:01.000000 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-12 11:31:01.000000 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-12 11:31:01.000000 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-12 11:31:01.000000 qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk.egg-info/top_level.txt
```

### Comparing `qfieldcloud-sdk-0.6.1/LICENCE` & `qfieldcloud-sdk-0.7.0/LICENCE`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.6.1/PKG-INFO` & `qfieldcloud-sdk-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfieldcloud-sdk
-Version: 0.6.1
+Version: 0.7.0
 Summary: The official QFieldCloud SDK and CLI.
 Home-page: https://github.com/opengisch/qfieldcloud-sdk-python
 Author: Ivan Ivanov
 Author-email: ivan@opengis.ch
 Project-URL: Bug Tracker, https://github.com/opengisch/qfieldcloud-sdk-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,16 +23,16 @@
 
 ## Module usage
 
 ```
 import requests
 from qfieldcloud_sdk import sdk
 
-client = sdk.Client(
-    url="https://app.qfield.cloud/api/v1/",
+client = sdk.Client(url="https://app.qfield.cloud/api/v1/")
+client.login(
     username="user1",
     password="pass1",
 )
 
 try:
     projects = client.list_projects()
 except requests.exceptions.RequestException:
```

### Comparing `qfieldcloud-sdk-0.6.1/README.md` & `qfieldcloud-sdk-0.7.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 ## Module usage
 
 ```
 import requests
 from qfieldcloud_sdk import sdk
 
-client = sdk.Client(
-    url="https://app.qfield.cloud/api/v1/",
+client = sdk.Client(url="https://app.qfield.cloud/api/v1/")
+client.login(
     username="user1",
     password="pass1",
 )
 
 try:
     projects = client.list_projects()
 except requests.exceptions.RequestException:
```

### Comparing `qfieldcloud-sdk-0.6.1/setup.py` & `qfieldcloud-sdk-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk/cli.py` & `qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/bin/env python3
 
 import collections
 import json
 import platform
 import sys
 from enum import Enum
+from typing import Any, Dict, List
 
 import click
 
 from qfieldcloud_sdk import sdk
 
 QFIELDCLOUD_DEFAULT_URL = "https://app.qfield.cloud/api/v1/"
 
@@ -156,48 +157,67 @@
         print_json(payload)
     else:
         log(payload["detail"])
 
 
 @cli.command()
 @click.option(
+    "-off",
+    "--offset",
+    default=None,
+    is_flag=False,
+    help="Offsets the given number of projects in the paginated JSON response",
+)
+@click.option(
+    "-l",
+    "--limit",
+    default=None,
+    is_flag=False,
+    help="Limits the number of projects to return in the paginated JSON response",
+)
+@click.option(
     "--include-public/--no-public",
     default=False,
+    is_flag=True,
     help="Includes the public project in the list. Default: False",
 )
 @click.pass_context
-def list_projects(ctx, include_public):
+def list_projects(ctx, **opts):
     """List QFieldCloud projects."""
 
     log("Listing projects…")
 
-    projects = ctx.obj["client"].list_projects(
-        include_public=include_public,
-    )
+    projects: List[Dict[str, Any]] = ctx.obj["client"].list_projects(**opts)
 
     if ctx.obj["format_json"]:
         print_json(projects)
     else:
         if projects:
             log("Projects:")
             for project in projects:
                 log(f'{project["id"]}\t{project["owner"]}/{project["name"]}')
         else:
             log("User does not have any projects yet.")
 
 
 @cli.command()
 @click.argument("project_id")
+@click.option(
+    "--skip-metadata/--no-skip-metadata",
+    "skip_metadata",
+    default=True,
+    help="Skip requesting for additional metadata (currently the `sha256` checksum) for each version. Default: --skip-metadata",
+)
 @click.pass_context
-def list_files(ctx, project_id):
+def list_files(ctx, project_id, skip_metadata):
     """List QFieldCloud project files."""
 
     log(f'Getting file list for "{project_id}"…')
 
-    files = ctx.obj["client"].list_remote_files(project_id)
+    files = ctx.obj["client"].list_remote_files(project_id, skip_metadata)
 
     if ctx.obj["format_json"]:
         print_json(files)
     else:
         if files:
             log(f'Files for project "{project_id}":')
             for file in files:
```

### Comparing `qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk/sdk.py` & `qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 class Client:
     def __init__(
         self, url: str = None, verify_ssl: bool = None, token: str = None
     ) -> None:
         """Prepares a new client.
 
         If the `url` is not provided, uses `QFIELDCLOUD_URL` from the environment.
-        If the `token` is not provided, uses `QFIELDCLOUD_TOKEN` from the environment."""
+        If the `token` is not provided, uses `QFIELDCLOUD_TOKEN` from the environment.
+        """
         self.url = url or os.environ.get("QFIELDCLOUD_URL", None)
         self.token = token or os.environ.get("QFIELDCLOUD_TOKEN", None)
         self.verify_ssl = verify_ssl
 
         if not self.verify_ssl:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
@@ -113,29 +114,43 @@
     def logout(self) -> None:
         """Logout from the current session."""
         resp = self._request("POST", "auth/logout")
 
         return resp.json()
 
     def list_projects(
-        self, username: Optional[str] = None, include_public: Optional[bool] = False
-    ) -> Dict:
-        """Lists the project of a given user. If the user is omitted, it fallbacks to the currently logged in user"""
-        resp = self._request(
-            "GET",
-            "projects",
-            params={
-                "include-public": "1" if include_public else "0",
-            },
-        )
+        self,
+        username: Optional[str] = None,
+        include_public: Optional[bool] = False,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+    ) -> List[Dict[str, Any]]:
+        """Returns a paginated lists the project of a given user. If the user is omitted, it fallbacks to the currently logged in user"""
+        params = {
+            "include-public": int(include_public),
+        }
+
+        if limit:
+            params["limit"] = limit
+        if offset:
+            params["offset"] = offset
+
+        resp = self._request("GET", "projects", params=params)
 
         return resp.json()
 
-    def list_remote_files(self, project_id: str) -> List[Dict[str, Any]]:
-        resp = self._request("GET", f"files/{project_id}")
+    def list_remote_files(
+        self, project_id: str, skip_metadata: bool = True
+    ) -> List[Dict[str, Any]]:
+        params = {}
+
+        if skip_metadata:
+            params["skip_metadata"] = "1"
+
+        resp = self._request("GET", f"files/{project_id}", params=params)
         return resp.json()
 
     def create_project(
         self,
         name: str,
         owner: str = None,
         description: str = "",
```

### Comparing `qfieldcloud-sdk-0.6.1/src/qfieldcloud_sdk.egg-info/PKG-INFO` & `qfieldcloud-sdk-0.7.0/src/qfieldcloud_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfieldcloud-sdk
-Version: 0.6.1
+Version: 0.7.0
 Summary: The official QFieldCloud SDK and CLI.
 Home-page: https://github.com/opengisch/qfieldcloud-sdk-python
 Author: Ivan Ivanov
 Author-email: ivan@opengis.ch
 Project-URL: Bug Tracker, https://github.com/opengisch/qfieldcloud-sdk-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,16 +23,16 @@
 
 ## Module usage
 
 ```
 import requests
 from qfieldcloud_sdk import sdk
 
-client = sdk.Client(
-    url="https://app.qfield.cloud/api/v1/",
+client = sdk.Client(url="https://app.qfield.cloud/api/v1/")
+client.login(
     username="user1",
     password="pass1",
 )
 
 try:
     projects = client.list_projects()
 except requests.exceptions.RequestException:
```

