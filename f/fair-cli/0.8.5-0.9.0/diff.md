# Comparing `tmp/fair_cli-0.8.5.tar.gz` & `tmp/fair_cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.8.5.tar", max compression
+gzip compressed data, was "fair_cli-0.9.0.tar", max compression
```

## Comparing `fair_cli-0.8.5.tar` & `fair_cli-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.8.5/CHANGELOG.md
--rw-r--r--   0        0        0     1358 2023-07-11 20:40:08.968781 fair_cli-0.8.5/CITATION.cff
--rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.8.5/LICENSE
--rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.8.5/README.md
--rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.8.5/fair/__init__.py
--rw-r--r--   0        0        0    21730 2023-07-11 16:34:34.113408 fair_cli-0.8.5/fair/cli.py
--rw-r--r--   0        0        0     9447 2023-07-11 16:34:34.113605 fair_cli-0.8.5/fair/common.py
--rw-r--r--   0        0        0    30704 2023-07-11 16:34:34.113863 fair_cli-0.8.5/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.8.5/fair/configuration/validation.py
--rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.8.5/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.8.5/fair/files.txt
--rw-r--r--   0        0        0     4773 2023-07-11 16:34:34.114027 fair_cli-0.8.5/fair/history.py
--rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.8.5/fair/identifiers.py
--rw-r--r--   0        0        0     3035 2023-07-11 16:34:34.114175 fair_cli-0.8.5/fair/logging.py
--rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.8.5/fair/register.py
--rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.8.5/fair/registry/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.8.5/fair/registry/file_formats.json
--rw-r--r--   0        0        0      138 2023-07-11 16:34:34.114333 fair_cli-0.8.5/fair/registry/file_types.py
--rw-r--r--   0        0        0    18004 2023-07-11 16:34:34.114556 fair_cli-0.8.5/fair/registry/requests.py
--rw-r--r--   0        0        0    15020 2023-07-11 16:34:34.114766 fair_cli-0.8.5/fair/registry/server.py
--rw-r--r--   0        0        0    24284 2023-07-11 16:34:34.115007 fair_cli-0.8.5/fair/registry/storage.py
--rw-r--r--   0        0        0    42144 2023-07-11 20:37:03.466251 fair_cli-0.8.5/fair/registry/sync.py
--rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.8.5/fair/registry/versioning.py
--rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.8.5/fair/run.py
--rw-r--r--   0        0        0    51996 2023-07-11 16:34:34.115371 fair_cli-0.8.5/fair/session.py
--rw-r--r--   0        0        0    16498 2023-07-11 16:34:34.115607 fair_cli-0.8.5/fair/staging.py
--rw-r--r--   0        0        0      526 2023-07-11 16:34:34.115767 fair_cli-0.8.5/fair/templates/__init__.py
--rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.8.5/fair/templates/config.jinja
--rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.8.5/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3244 2023-07-11 16:34:34.115922 fair_cli-0.8.5/fair/testing.py
--rw-r--r--   0        0        0    54227 2023-07-11 16:34:34.116289 fair_cli-0.8.5/fair/user_config/__init__.py
--rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.8.5/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9205 2023-07-11 16:34:34.116474 fair_cli-0.8.5/fair/user_config/validation.py
--rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.8.5/fair/utilities.py
--rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.8.5/fair/virtualenv.py
--rw-r--r--   0        0        0     2496 2023-07-11 20:39:56.996799 fair_cli-0.8.5/pyproject.toml
--rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-07-12 09:43:39.260411 fair_cli-0.9.0/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.9.0/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.9.0/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.9.0/fair/__init__.py
+-rw-r--r--   0        0        0    23763 2023-07-12 09:43:39.260687 fair_cli-0.9.0/fair/cli.py
+-rw-r--r--   0        0        0     9447 2023-07-11 16:34:34.113605 fair_cli-0.9.0/fair/common.py
+-rw-r--r--   0        0        0    30704 2023-07-11 16:34:34.113863 fair_cli-0.9.0/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.9.0/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.9.0/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.9.0/fair/files.txt
+-rw-r--r--   0        0        0     4773 2023-07-11 16:34:34.114027 fair_cli-0.9.0/fair/history.py
+-rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.9.0/fair/identifiers.py
+-rw-r--r--   0        0        0     3035 2023-07-11 16:34:34.114175 fair_cli-0.9.0/fair/logging.py
+-rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.9.0/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.9.0/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.9.0/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      138 2023-07-11 16:34:34.114333 fair_cli-0.9.0/fair/registry/file_types.py
+-rw-r--r--   0        0        0    18004 2023-07-11 16:34:34.114556 fair_cli-0.9.0/fair/registry/requests.py
+-rw-r--r--   0        0        0    15020 2023-07-11 16:34:34.114766 fair_cli-0.9.0/fair/registry/server.py
+-rw-r--r--   0        0        0    24284 2023-07-11 16:34:34.115007 fair_cli-0.9.0/fair/registry/storage.py
+-rw-r--r--   0        0        0    42144 2023-07-11 20:37:03.466251 fair_cli-0.9.0/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.9.0/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.9.0/fair/run.py
+-rw-r--r--   0        0        0    58739 2023-07-12 09:43:39.261073 fair_cli-0.9.0/fair/session.py
+-rw-r--r--   0        0        0    16498 2023-07-11 16:34:34.115607 fair_cli-0.9.0/fair/staging.py
+-rw-r--r--   0        0        0      526 2023-07-11 16:34:34.115767 fair_cli-0.9.0/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.9.0/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.9.0/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3244 2023-07-11 16:34:34.115922 fair_cli-0.9.0/fair/testing.py
+-rw-r--r--   0        0        0    54227 2023-07-12 09:40:05.032694 fair_cli-0.9.0/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.9.0/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9205 2023-07-11 16:34:34.116474 fair_cli-0.9.0/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.9.0/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.9.0/fair/virtualenv.py
+-rw-r--r--   0        0        0     2496 2023-07-12 09:43:39.261253 fair_cli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.9.0/PKG-INFO
```

### Comparing `fair_cli-0.8.5/CHANGELOG.md` & `fair_cli-0.9.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/CITATION.cff` & `fair_cli-0.9.0/CITATION.cff`

 * *Files 7% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 - FAIR
 - Data Management
 - Provenance
 license: BSD-2-Clause
 message: If you use this software, please cite it using these metadata.
 repository-code: https://github.com/FAIRDataPipeline/FAIR-CLI/
 title: "The FAIR Data Pipeline command line tool"
-version: 0.8.5
+version: 0.9.0
```

### Comparing `fair_cli-0.8.5/LICENSE` & `fair_cli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/README.md` & `fair_cli-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/__init__.py` & `fair_cli-0.9.0/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/cli.py` & `fair_cli-0.9.0/fair/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,72 @@
 @click.group()
 @click.version_option(package_name="fair-cli")
 @click.pass_context
 def cli(ctx):
     """Welcome to FAIR-CLI, the FAIR data pipeline command-line interface."""
     pass
 
+@cli.command()
+@click.argument("file_path")
+@click.option("--remote", help="Show Remote Code Runs", default= "origin")
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option(
+    "--local/--no-local",
+    help="init without a remote registry - useful for closed systems",
+    default=False,
+)
+def identify(file_path: str, remote:str, debug, local:bool) -> None:
+    """
+    list details of a file
+    
+    Usage: fair identify /path/to/file [remote]
+    """
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI, local=local
+        ) as fair_session:
+            fair_session.get_details(file_path, remote = "")
+            if not local:
+                fair_session.get_details(file_path, remote = remote)
+    except fdp_exc.FAIRCLIException as e:
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+@cli.command()
+@click.argument("data_product")
+@click.option("--remote", help="Show Remote Code Runs", default= "origin")
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option(
+    "--local/--no-local",
+    help="init without a remote registry - useful for closed systems",
+    default=False,
+)
+def find(data_product: str, remote: str, debug:bool, local:bool) -> None:
+    """
+    Shows where a data product is located
+    
+    Data Products should be formatted: 
+    <namespace>:<data product name>@v<version>
+    eg:
+    PSU:SEIRS_model/parameters@v1.0.0
+
+    Usage: fair find data_product [remote]
+    """
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI, local=local
+        ) as fair_session:
+            fair_session.find_data_product(data_product, "")
+            if not local:
+                fair_session.find_data_product(data_product, remote)
+    except fdp_exc.FAIRCLIException as e:
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 @cli.command()
 @click.option("--verbose/--not-verbose", help="Display URLs", default=False)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def status(verbose, debug) -> None:
     """Get the status of files under staging"""
     try:
```

### Comparing `fair_cli-0.8.5/fair/common.py` & `fair_cli-0.9.0/fair/common.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/configuration/__init__.py` & `fair_cli-0.9.0/fair/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/configuration/validation.py` & `fair_cli-0.9.0/fair/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/exceptions.py` & `fair_cli-0.9.0/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/files.txt` & `fair_cli-0.9.0/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/history.py` & `fair_cli-0.9.0/fair/history.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/identifiers.py` & `fair_cli-0.9.0/fair/identifiers.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/logging.py` & `fair_cli-0.9.0/fair/logging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/register.py` & `fair_cli-0.9.0/fair/register.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/registry/file_formats.json` & `fair_cli-0.9.0/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/registry/requests.py` & `fair_cli-0.9.0/fair/registry/requests.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/registry/server.py` & `fair_cli-0.9.0/fair/registry/server.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/registry/storage.py` & `fair_cli-0.9.0/fair/registry/storage.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/registry/sync.py` & `fair_cli-0.9.0/fair/registry/sync.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/registry/versioning.py` & `fair_cli-0.9.0/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/run.py` & `fair_cli-0.9.0/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/session.py` & `fair_cli-0.9.0/fair/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 import fair.registry.server as fdp_serv
 import fair.registry.sync as fdp_sync
 import fair.staging as fdp_stage
 import fair.templates as fdp_tpl
 import fair.testing as fdp_test
 import fair.user_config as fdp_user
 import fair.logging as fdp_logging
+import fair.registry.storage as fdp_store
 
 
 class FAIR:
     """
     A class which provides the main interface for managing runs and data
     transfer between FAIR Data Pipeline registries.
 
@@ -920,29 +921,48 @@
                     params={"uuid": uuid})
                 if _remote_code_run:
                     return _remote_code_run[0]["description"]
         except Exception:
             pass
         return "Unknown"
 
+    def get_code_run_date(self, uuid: str)-> str:
+        _local_uri = fdp_conf.get_local_uri()
+        _local_code_run = fdp_req.get(_local_uri, "code_run", fdp_req.local_token(), params={"uuid": uuid})
+        if _local_code_run:
+            return _local_code_run[0]["run_date"]
+        try:
+            for label in self._local_config["registries"]:
+                _remote_code_run = fdp_req.get(
+                    fdp_conf.get_remote_uri(self._session_loc, label),
+                    "code_run",
+                    fdp_conf.get_remote_token(self._session_loc, label, local=self._local),
+                    params={"uuid": uuid})
+                if _remote_code_run:
+                    return _remote_code_run[0]["run_date"]
+        except Exception:
+            pass
+        return "Unknown"
+
     def show_code_runs(
         self, code_runs: typing.List[str], title: str, style="green"
     ) -> None:
         console = Console()
         table = Table(
             title=title,
             title_style="bold",
             title_justify="left",
             box=rich.box.SIMPLE,
         )
-        table.add_column("Code Run UUID", style=style, no_wrap=True)
+        table.add_column("Code Run UUID", style=style, no_wrap=False)
         table.add_column("Code Run Description", style=style, no_wrap=True)
+        table.add_column("Code Run Date", style=style, no_wrap=True)
         for i, code_run in enumerate(code_runs):
 
-            table.add_row(code_run, self.get_code_run_description(code_run))
+            table.add_row(code_run, self.get_code_run_description(code_run), self.get_code_run_date(code_run))
             if i == 9 and i != len(code_runs) - 1:
                 table.add_row(
                     f"+ {len(code_runs) - i - 1} more...",
                     "",
                     "",
                 )
                 break
@@ -1340,14 +1360,112 @@
 
         with open(fdp_com.global_fdpconfig(), encoding='utf-8', mode= "w") as f:
             yaml.dump(_glob_cfg, f)
 
         with open(fdp_com.local_fdpconfig(self._session_loc), encoding='utf-8', mode= "w") as f:
             yaml.dump(_loc_cfg, f)
 
+    def get_details(self, file_path: str, remote = "origin"):
+        if self._local:
+            remote = None
+        _api_url = fdp_conf.get_local_uri() if not remote else fdp_conf.get_remote_uri(self._session_loc, remote)
+        _token = fdp_req.local_token() if not remote else fdp_conf.get_remote_token(self._session_loc, remote)
+        _registry = f"Local Registry {_api_url}" if not remote else f"Remote Registry {remote} {_api_url}"
+        if not os.path.exists(file_path):
+            raise fdp_exc.FileNotFoundError(f"File: {file_path} does not exist")
+        click.echo(f"Information about file: {file_path}")
+        _hash = fdp_store.calculate_file_hash(file_path)
+        _storage_location = fdp_req.get(_api_url,
+                                         "storage_location",
+                                         _token,
+                                         params= {'hash': _hash})
+        if _storage_location:
+            _storage_location = _storage_location[0]
+        else:
+            click.echo(f"File: {file_path} could not be found on the {_registry}")
+            return
+        _objects = fdp_req.get(_api_url,
+                               "object",
+                               _token,
+                               params= {"storage_location": fdp_req.get_obj_id_from_url(_storage_location["url"])}
+                               )
+        for _object in _objects:
+            if _object["data_products"]:
+                for _data_product_url in _object["data_products"]:
+                    _data_product = fdp_req.url_get(_data_product_url, _token)
+                    if _data_product:
+                        click.echo(f"Is linked to 'data_product': {_data_product['name']} with url: {_data_product_url}")
+            if _object["components"]:
+                for _component_url in _object["components"]:
+                    _component = fdp_req.url_get(_component_url, _token)
+                    if _component:
+                        if _component["inputs_of"]:
+                            for _input_url in _component["inputs_of"]:
+                                _input = fdp_req.url_get(_input_url, _token)
+                                if _input:
+                                    _input_description = _input["description"]
+                                    _input_uuid = _input["uuid"]
+                                    click.echo(f"is an input of coderun: {_input_uuid} {_input_description} {_input_url}")
+                        if _component["outputs_of"]:
+                            for _output_url in _component["outputs_of"]:
+                                _output = fdp_req.url_get(_output_url, _token)
+                                if _output:
+                                    _output_description = _output["description"]
+                                    _output_uuid = _output["uuid"]
+                                    click.echo(f"Is an output of coderun: {_output_uuid} {_output_description} {_output_url}")
+
+
+    def find_data_product(self, data_product: str, remote = "origin"):
+        if self._local:
+            remote = None
+        _api_url = fdp_conf.get_local_uri() if not remote else fdp_conf.get_remote_uri(self._session_loc, remote)
+        _token = fdp_req.local_token() if not remote else fdp_conf.get_remote_token(self._session_loc, remote)
+        _registry = f"Local Registry {_api_url}" if not remote else f"Remote Registry {remote} {_api_url}"
+        if "@" not in data_product:
+            namespace, name = re.split("[:]", data_product)
+            version = None
+        else:
+            namespace, name, version = re.split("[:@]", data_product)
+            version = version.replace("v", "")
+        _namespace = fdp_req.get(_api_url,
+                                    "namespace",
+                                    _token,
+                                    params= {'name': namespace})
+        if _namespace:
+            _namespace_url = _namespace[0]["url"]
+            _data_product = fdp_req.get(_api_url,
+                                        "data_product",
+                                        _token,
+                                        params= {
+                                            'name': name,
+                                            'namespace': fdp_req.get_obj_id_from_url(_namespace_url),
+                                            'version': version
+                                        })
+            if _data_product:
+                _object_url = _data_product[0]["object"]
+                _object = fdp_req.url_get(_object_url, _token)
+                if _object:
+                    _storage_location_url = _object["storage_location"]
+                    if _storage_location_url:
+                        _storage_location = fdp_req.url_get(_storage_location_url, _token)
+                        if _storage_location:
+                            _storage_root_url = _storage_location["storage_root"]
+                            _storage_location_path = _storage_location["path"]
+                            _storage_root = fdp_req.url_get(_storage_root_url, _token)
+                            if _storage_root:
+                                _root = _storage_root["root"]
+                                if "file://" in _root:
+                                    click.echo(f"Data Product: {data_product} is located {_root}{os.pathsep}{_storage_location_path}")
+                                else:
+                                    click.echo(f"Data Product: {data_product} is located {_root}/{_storage_location_path}")
+            else:
+                click.echo(f"Data Product {data_product} could not be found on {_registry}")
+        else:
+            click.echo(f"Namespace {namespace} not found on {_registry}")
+
     def _set_logger_info(self):
         handler = logging.StreamHandler()
         handler.setFormatter(
             fdp_logging.LevelFormatter(
                 {
                     logging.INFO: '%(message)s'
                 }
```

### Comparing `fair_cli-0.8.5/fair/staging.py` & `fair_cli-0.9.0/fair/staging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/templates/__init__.py` & `fair_cli-0.9.0/fair/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/testing.py` & `fair_cli-0.9.0/fair/testing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/user_config/__init__.py` & `fair_cli-0.9.0/fair/user_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/user_config/globbing.py` & `fair_cli-0.9.0/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/user_config/validation.py` & `fair_cli-0.9.0/fair/user_config/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/utilities.py` & `fair_cli-0.9.0/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/fair/virtualenv.py` & `fair_cli-0.9.0/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.8.5/pyproject.toml` & `fair_cli-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Environment :: Console",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Operating System :: OS Independent",
 ]
 description = "Synchronization interface for the SCRC FAIR Data Pipeline registry"
 name = "fair-cli"
-version = "0.8.5"
+version = "0.9.0"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
```

### Comparing `fair_cli-0.8.5/PKG-INFO` & `fair_cli-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.8.5
+Version: 0.9.0
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
```

