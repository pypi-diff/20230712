# Comparing `tmp/cycleops-0.2.2.tar.gz` & `tmp/cycleops-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycleops-0.2.2.tar", max compression
+gzip compressed data, was "cycleops-0.3.0.tar", max compression
```

## Comparing `cycleops-0.2.2.tar` & `cycleops-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-05-26 14:08:21.326726 cycleops-0.2.2/LICENSE
--rw-r--r--   0        0        0     3994 2023-05-26 14:08:21.326726 cycleops-0.2.2/README.md
--rw-r--r--   0        0        0     1125 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/__main__.py
--rw-r--r--   0        0        0      414 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/auth.py
--rw-r--r--   0        0        0     5468 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/client.py
--rw-r--r--   0        0        0     1113 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/exceptions.py
--rw-r--r--   0        0        0    12653 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/services.py
--rw-r--r--   0        0        0     4249 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/setups.py
--rw-r--r--   0        0        0     3047 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/stacks.py
--rw-r--r--   0        0        0      869 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/units.py
--rw-r--r--   0        0        0      972 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/utils.py
--rw-r--r--   0        0        0      556 2023-05-26 14:08:21.326726 cycleops-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4519 1970-01-01 00:00:00.000000 cycleops-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 14:21:04.818804 cycleops-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3994 2023-07-12 14:21:04.818804 cycleops-0.3.0/README.md
+-rw-r--r--   0        0        0     1125 2023-07-12 14:21:04.818804 cycleops-0.3.0/cycleops/__main__.py
+-rw-r--r--   0        0        0      414 2023-07-12 14:21:04.818804 cycleops-0.3.0/cycleops/auth.py
+-rw-r--r--   0        0        0     5601 2023-07-12 14:21:04.818804 cycleops-0.3.0/cycleops/client.py
+-rw-r--r--   0        0        0     1113 2023-07-12 14:21:04.818804 cycleops-0.3.0/cycleops/exceptions.py
+-rw-r--r--   0        0        0    12653 2023-07-12 14:21:04.818804 cycleops-0.3.0/cycleops/services.py
+-rw-r--r--   0        0        0     5304 2023-07-12 14:21:04.818804 cycleops-0.3.0/cycleops/setups.py
+-rw-r--r--   0        0        0     3047 2023-07-12 14:21:04.818804 cycleops-0.3.0/cycleops/stacks.py
+-rw-r--r--   0        0        0      869 2023-07-12 14:21:04.818804 cycleops-0.3.0/cycleops/units.py
+-rw-r--r--   0        0        0      972 2023-07-12 14:21:04.818804 cycleops-0.3.0/cycleops/utils.py
+-rw-r--r--   0        0        0      556 2023-07-12 14:21:04.818804 cycleops-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4519 1970-01-01 00:00:00.000000 cycleops-0.3.0/PKG-INFO
```

### Comparing `cycleops-0.2.2/LICENSE` & `cycleops-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.2/README.md` & `cycleops-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.2/cycleops/__main__.py` & `cycleops-0.3.0/cycleops/__main__.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.2/cycleops/client.py` & `cycleops-0.3.0/cycleops/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class Client:
     """
     A client for the Cycleops API.
     """
 
     def __init__(
         self,
-        base_url: Optional[str] = "https://cloud.cycleops.io/manager",
+        base_url: Optional[str] = "https://cloud.cycleops.io/stack-manager",
         api_key: Optional[str] = None,
     ):
         self.base_url: str = sec.load("CYCLEOPS_BASE_URL", base_url)
         self.api_key: str = sec.load("CYCLEOPS_API_KEY", api_key)
 
     def _request(
         self, method: str, endpoint: str, payload: Optional[Dict[str, Any]] = None
@@ -98,14 +98,17 @@
     """
 
     def create(self, **kwargs: Any) -> Optional[Dict[str, Any]]:
         payload: Dict[str, Any] = {k: v for (k, v) in kwargs.items() if v}
 
         return self.client._request("POST", "jobs", payload)
 
+    def retrieve(self, job_id: int) -> Optional[Dict[str, Any]]:
+        return self.client._request("GET", f"jobs/{job_id}")
+
 
 class SetupClient(SubClient):
     """
     Client for managing Cycleops setups.
     """
 
     def list(self) -> Optional[Dict[str, Any]]:
```

### Comparing `cycleops-0.2.2/cycleops/exceptions.py` & `cycleops-0.3.0/cycleops/exceptions.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.2/cycleops/services.py` & `cycleops-0.3.0/cycleops/services.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -304,16 +304,16 @@
         service["variables"]["containers"].append(
             {
                 "name": container_name,
                 "image": image_name,
                 "tag": image_tag,
                 "ports": ports_list,
                 "volumes": volumes_list,
-                "command": command,
                 "env_vars": env_vars,
+                "command": command,
             }
         )
 
         service_client.update(
             service_id,
             variables=service["variables"],
         )
@@ -408,16 +408,16 @@
 
         variables = {
             "name": container_name,
             "image": image_name,
             "tag": image_tag,
             "ports": ports_list,
             "volumes": volumes_list,
-            "command": command,
             "env_vars": env_vars,
+            "command": command,
         }
 
         for key, value in variables.items():
             if value:
                 service["variables"]["containers"][container_index][key] = value
 
         service_client.update(
```

### Comparing `cycleops-0.2.2/cycleops/setups.py` & `cycleops-0.3.0/cycleops/setups.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import time
 from typing import List, Optional
 
 import typer
 from rich import print
 
-from .client import SetupClient, cycleops_client
+from .client import JobClient, SetupClient, cycleops_client
 from .exceptions import NotFound
 from .utils import display_error_message, display_success_message
 
 app = typer.Typer()
 
 setup_client: SetupClient = SetupClient(cycleops_client)
+job_client: JobClient = JobClient(cycleops_client)
 
 
 @app.command()
 def list() -> None:
     """
     List all of the available setups.
     """
@@ -153,18 +155,43 @@
         display_success_message(f"Setup {setup_id} has been deleted")
     except Exception as error:
         display_error_message(error)
         raise typer.Abort()
 
 
 @app.command()
-def deploy(setup_id: int = typer.Argument(..., help="The ID of the setup.")) -> None:
+def deploy(
+    setup_id: int = typer.Argument(..., help="The ID of the setup."),
+    wait: Optional[bool] = typer.Option(
+        default=False, help="Wait for the deployment job to complete"
+    ),
+) -> None:
     """
     Deploy the setup with the specified setup_id.
     """
 
     try:
-        setup_client.deploy(setup_id)
-        display_success_message(f"Setup {setup_id} has been queued for deployment")
+        job = setup_client.deploy(setup_id)
+        report_queued = print if wait else display_success_message
+        report_queued(f"Setup {setup_id} has been queued for deployment")
+
+        while wait:
+            match status := job["status"]:
+                case "Initialized":
+                    print(f"Setup {setup_id} has been initialized")
+                case "Deploying":
+                    print(f"Setup {setup_id} is being deployed")
+                case "Deployed":
+                    display_success_message(
+                        f"Setup {setup_id} has been deployed successfully"
+                    )
+                    break
+                case "Failed":
+                    display_error_message(job)
+                    raise Exception(f"Setup {setup_id} could not be deployed")
+                case _:
+                    print(f"Setup {setup_id} is in status {status}")
+            time.sleep(3)
+            job = job_client.retrieve(job["id"])
     except Exception as error:
         display_error_message(error)
         raise typer.Abort()
```

### Comparing `cycleops-0.2.2/cycleops/stacks.py` & `cycleops-0.3.0/cycleops/stacks.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.2/cycleops/units.py` & `cycleops-0.3.0/cycleops/units.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.2/cycleops/utils.py` & `cycleops-0.3.0/cycleops/utils.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.2/pyproject.toml` & `cycleops-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycleops"
-version = "0.2.2"
+version = "0.3.0"
 description = "The official command line interface for Cycleops"
 authors = ["George Margaritis <george@withlogic.co>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `cycleops-0.2.2/PKG-INFO` & `cycleops-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycleops
-Version: 0.2.2
+Version: 0.3.0
 Summary: The official command line interface for Cycleops
 License: MIT
 Author: George Margaritis
 Author-email: george@withlogic.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

