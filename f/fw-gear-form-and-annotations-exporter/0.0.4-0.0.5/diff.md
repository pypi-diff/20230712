# Comparing `tmp/fw_gear_form_and_annotations_exporter-0.0.4-py3-none-any.whl.zip` & `tmp/fw_gear_form_and_annotations_exporter-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15320 bytes, number of entries: 10
+Zip file size: 16412 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      162 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter/__init__.py
--rw-r--r--  2.0 unx    14519 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter/collect_form_annot_data.py
+-rw-r--r--  2.0 unx    14474 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter/collect_form_annot_data.py
 -rw-r--r--  2.0 unx     6448 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter/constants.py
--rw-r--r--  2.0 unx     5758 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter/flywheel_api_helpers.py
--rw-r--r--  2.0 unx     4009 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter/main.py
+-rw-r--r--  2.0 unx    14267 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter/flywheel_api_helpers.py
+-rw-r--r--  2.0 unx     3799 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter/main.py
 -rw-r--r--  2.0 unx     3096 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter/parser.py
--rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    12571 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter-0.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1073 b- defN 16-Jan-01 00:00 fw_gear_form_and_annotations_exporter-0.0.4.dist-info/RECORD
-10 files, 48816 bytes uncompressed, 13422 bytes compressed:  72.5%
+-rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12418 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_form_and_annotations_exporter-0.0.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1074 b- defN 16-Jan-01 00:00 fw_gear_form_and_annotations_exporter-0.0.5.dist-info/RECORD
+10 files, 56918 bytes uncompressed, 14514 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: fw_gear_form_and_annotations_exporter/main.py
 Comment: 
 
 Filename: fw_gear_form_and_annotations_exporter/parser.py
 Comment: 
 
-Filename: fw_gear_form_and_annotations_exporter-0.0.4.dist-info/LICENSE
+Filename: fw_gear_form_and_annotations_exporter-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: fw_gear_form_and_annotations_exporter-0.0.4.dist-info/METADATA
+Filename: fw_gear_form_and_annotations_exporter-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: fw_gear_form_and_annotations_exporter-0.0.4.dist-info/WHEEL
+Filename: fw_gear_form_and_annotations_exporter-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: fw_gear_form_and_annotations_exporter-0.0.4.dist-info/RECORD
+Filename: fw_gear_form_and_annotations_exporter-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_gear_form_and_annotations_exporter/collect_form_annot_data.py

```diff
@@ -13,14 +13,15 @@
     TASK_TYPE_MAPPING,
 )
 from .flywheel_api_helpers import (
     get_acquisition,
     get_file,
     get_file_annotations,
     get_files,
+    get_form_responses,
     get_project,
     get_session,
     get_subject,
     get_task_annotations,
 )
 
 log = logging.getLogger(__name__)
@@ -197,19 +198,15 @@
         parent_id (str): The id of the parent container.
 
     Returns:
         list: List of form responses.
     """
 
     export_list = []
-
-    results_list = client.get(
-        "/api/formresponses",
-        params={"filter": f"parents.{parent_type}={parent_id},form_id={form_id}"},
-    )
+    results_list = get_form_responses(client, parent_type, parent_id, form_id)
 
     if form_responses_scope in ["task", "both"]:
         export_list.extend(
             [resp for resp in results_list["results"] if resp.get("task_id")]
         )
 
     if form_responses_scope in ["non-task", "both"]:
@@ -229,15 +226,15 @@
 
     Returns:
         DataFrame: Processed dataframe to save as output.
     """
 
     # If we have no form responses, return an empty DataFrame with the correct columns
     if not form_responses:
-        log.warn("No form responses found")
+        log.warning("No form responses found")
         return pd.DataFrame(columns=RESPONSE_COLS_MAPPING.values())
 
     raw_df = pd.json_normalize(form_responses)
 
     # Select columns representing the form responses
     prefix = "response_data"
     selected_columns = [col for col in raw_df.columns if col.startswith(prefix)]
```

## fw_gear_form_and_annotations_exporter/flywheel_api_helpers.py

```diff
@@ -1,25 +1,89 @@
+"""This module contains helper functions for interacting with the Flywheel API.
+
+TODO: Move this to a separate package.
+"""
 import logging
 from functools import lru_cache
 
+from fw_client import ClientError
+
 log = logging.getLogger(__name__)
 
 
 @lru_cache(maxsize=512)
 def get_task(client, task_id):
     """Get task from api by task_id.
 
     Args:
         client (FW_Client): The Flywheel api client.
         task_id (str): The ID of the task.
 
     Returns:
         dict: Result of the api call.
     """
-    return client.get(f"/api/readertasks/{task_id}")
+    try:
+        result = client.get(f"/api/readertasks/{task_id}")
+    except ClientError:
+        # If the task does not exist, return None
+        result = None
+    except Exception:  # pylint: disable=broad-except
+        # If another error occurs, handle it by returning None
+        result = None
+
+    return result
+
+
+def put_reader_task(client, task_id, task_data):
+    """Put task to api by task_id.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        task_id (str): The ID of the task.
+        task_data (dict): The task data to put.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    return client.put(f"/api/readertasks/{task_id}", json=task_data)
+
+
+@lru_cache(maxsize=512)
+def get_project_tasks(
+    client, project_id, protocol_id=None, parent_type=None, parent_id=None
+):
+    """Get tasks from api by project_id.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        project_id (str): The ID of the project.
+        protocol_id (str, optional): The ID of the protocol. Defaults to None.
+        parent_type (str, optional): The type of the parent container. Defaults to None.
+        parent_id (str, optional): The ID of the parent container. Defaults to None.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    filter_str = ""
+    # NOTE: This API endpoint requires that the protocol_id in the filter string
+    #       has double quotes around it.
+    #       This is not the case for other container ids.
+    if protocol_id:
+        filter_str = f'protocol_id="{protocol_id}"'
+    # If the destination container is a subject, session, or acquisition
+    if parent_type in ["subject", "session", "acquisition"] and parent_id:
+        filter_str += "," if filter_str else ""
+        filter_str += f"parents.{parent_type}={parent_id}"
+    if filter_str:
+        return client.get(
+            f"/api/readertasks/project/{project_id}",
+            params={"filter": filter_str},
+        )
+    else:
+        return client.get(f"/api/readertasks/project/{project_id}")
 
 
 @lru_cache(maxsize=512)
 def get_task_annotations(client, task_id):
     """Get task annotations from api by task_id.
 
     TODO: Can this be filtered by the container in which the gear is run?
@@ -30,40 +94,196 @@
 
     Returns:
         dict: Result of the api call.
     """
     return client.get(f"/api/readertasks/{task_id}/annotations")
 
 
+def batch_create_tasks(client, tasks_definition):
+    """Batch create tasks.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        tasks_definition (dict): Dictionary of tasks to create.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    return client.post("/api/readertasks/batch", json=tasks_definition)
+
+
+def post_viewer_config(client, config):
+    """Post viewer config to api client.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        config (dict): The viewer config object.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    return client.post("/api/viewerconfigs", json=config)
+
+
 @lru_cache(maxsize=512)
-def get_protocol(client, protocol_id):
+def get_viewer_config(client, config_id=None, config_name=None):
+    """Get viewer config by id from api client.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        config_id (str): The ID of the viewer config.
+        config_name (str): The name of the viewer config.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    if config_name:
+        params = {"filter": f"name={config_name}"}
+        return client.get("/api/viewerconfigs", params=params)
+    if config_id:
+        return client.get(f"/api/viewerconfigs/{config_id}")
+    return {}
+
+
+def post_protocol(client, protocol: dict):
+    """Post protocol to api client.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        protocol (dict): The protocol object.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    return client.post("/api/read_task_protocols", json=protocol)
+
+
+@lru_cache(maxsize=512)
+def get_protocol(client, protocol_id=None, protocol_name=None, project_id=None):
     """Get protocol by id from api client.
 
     Args:
         client (FW_Client): The Flywheel api client.
+        protocol_id (str): The ID of the protocol. Defaults to None.
+        protocol_name (str): The name of the protocol. Defaults to None.
+        project_id (str): The ID of the project. Defaults to None.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    if protocol_name and project_id:
+        params = {"filter": f"name={protocol_name},parents.project={project_id}"}
+        return client.get("/api/read_task_protocols", params=params)
+    if protocol_id:
+        return client.get(f"/api/read_task_protocols/{protocol_id}")
+    return client.get("/api/read_task_protocols")
+
+
+def put_protocol(client, protocol_id, protocol):
+    """Put protocol to api client.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
         protocol_id (str): The ID of the protocol.
+        protocol (dict): The protocol object.
 
     Returns:
         dict: Result of the api call.
     """
-    return client.get(f"/api/read_task_protocols/{protocol_id}")
+    return client.put(f"/api/read_task_protocols/{protocol_id}", json=protocol)
+
+
+def post_form(client, form_data: dict):
+    """Post form to api client.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        form (dict): The form object.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    return client.post("/api/forms", json=form_data)
 
 
 @lru_cache(maxsize=512)
-def get_form(client, form_id):
+def get_form(client, form_id=None, project_id=None):
     """Get form by id from api client.
 
     Args:
         client (FW_Client): The Flywheel api client.
+        form_id (str): The ID of the form. Defaults to None.
+        project_id (str): The ID of the project. Defaults to None.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    if project_id:
+        params = {"filter": f"parents.project={project_id}"}
+        return client.get("/api/forms", params=params)
+    if form_id:
+        return client.get(f"/api/forms/{form_id}")
+    return client.get("/api/forms")
+
+
+@lru_cache(maxsize=512)
+def get_form_responses(
+    client, parent_type=None, parent_id=None, form_id=None, task_id=None
+):
+    """Get form responses from api client.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        parent_type (str): The type of parent container. Defaults to None.
+        parent_id (str): The ID of the parent container. Defaults to None.
+        form_id (str): The ID of the form. Defaults to None.
+        task_id (str): The ID of the task. Defaults to None.
+
+    Returns:
+        dict: Result of the api call.
+    """
+    filter_string = ""
+    if parent_type and parent_id:
+        filter_string = f"parents.{parent_type}={parent_id}"
+
+    if form_id:
+        filter_string += "," if filter_string else ""
+        filter_string += f"form_id={form_id}"
+
+    if task_id:
+        filter_string += "," if filter_string else ""
+        filter_string += f"task_id={task_id}"
+
+    params = {"filter": filter_string}
+    return client.get("/api/formresponses", params=params)
+
+
+def post_form_responses(
+    client, parent_type, parent_id, form_id, task_id, response_data
+):
+    """Post form responses to api client.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        parent_type (str): The type of parent container.
+        parent_id (str): The ID of the parent container.
         form_id (str): The ID of the form.
+        task_id (str): The ID of the task.
+        response_data (dict): The response_data of the form data object.
 
     Returns:
         dict: Result of the api call.
     """
-    return client.get(f"/api/forms/{form_id}")
+    post_data = {
+        "form_id": form_id,
+        "parent": {"id": parent_id, "type": parent_type},
+        "task_id": task_id,
+        "response_data": response_data,
+    }
+    return client.post("/api/formresponses", json=post_data)
 
 
 @lru_cache(maxsize=512)
 def get_project(client, project_id):
     """Get project by id from api client.
 
     Args:
@@ -140,15 +360,15 @@
         parent_type (str): Container type of the parent the gear is run within.
         parent_id (str): Container ID of the parent the gear is run within.
 
     Returns:
         dict: Result of the api call.
     """
 
-    filter_string = f"{parent_type}={parent_id}"
+    filter_string = f"parents.{parent_type}={parent_id}"
     params = {"filter": filter_string}
     return client.get("/api/files", params=params)
 
 
 @lru_cache(maxsize=512)
 def get_file_annotations(client, file_id, version=None):
     """Get all annotations for a file version.
@@ -165,14 +385,65 @@
         filter_string = f"file_ref.file_id={file_id},file_ref.version={version}"
     else:
         filter_string = f"file_ref.file_id={file_id}"
 
     return client.get("/api/annotations", params={"filter": filter_string})
 
 
+def post_file_annotation(client, data, viewer_format, file_id=None, task_id=None):
+    """Post annotations for a file.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        data (dict): The annotation data to post.
+        viewer_format (str): The viewer format of the annotation.
+        file_id (str): The id of the file. Defaults to None.
+        task_id (str): The id of the task. Defaults to None.
+
+    Returns:
+        dict: Result of the api call.
+    """
+
+    post_data = {
+        "_id": "",
+        "file_id": file_id,
+        "task_id": task_id,
+        "data": data,
+        "viewer_format": viewer_format,
+    }
+
+    return client.post("/api/annotations", json=post_data)
+
+
+def post_file_annotations(client, annotations, file_id=None, task_id=None):
+    """Iterate through annotations and post them into the api.
+
+    Args:
+        client (FW_Client): The Flywheel api client.
+        annotations (dict): The annotation data to post.
+        file_id (str): The id of the file. Defaults to None.
+        task_id (str): The id of the task. Defaults to None.
+
+    Returns:
+        dict: A dictionary of results.
+    """
+    results = {"count": 0, "total": 0, "results": []}
+    for annotation in annotations:
+        result = post_file_annotation(
+            client, annotation["data"], annotation["viewer_format"], file_id, task_id
+        )
+        if result:
+            results["count"] += 1
+            results["total"] += 1
+            results["results"].append(result)
+
+    return results
+
+
+@lru_cache(maxsize=512)
 def get_protocol_from_name(client, protocol_name, project_id=None):
     """Get Protocol object from api by name.
 
     Args:
         client (FW_Client): The Flywheel api client.
         protocol_name (str): The name of the protocol. Protocol Names are unique within
                              a project.
```

## fw_gear_form_and_annotations_exporter/main.py

```diff
@@ -9,15 +9,15 @@
 from .collect_form_annot_data import (
     build_annotations_dataframe,
     build_annotations_list,
     build_form_responses_dataframe,
     build_form_responses_list,
     process_task_list,
 )
-from .flywheel_api_helpers import get_protocol_from_name
+from .flywheel_api_helpers import get_project_tasks, get_protocol_from_name
 
 log = logging.getLogger(__name__)
 
 
 def run(context, api_key, protocol_name, annotations_scope, form_responses_scope):
     """Run the algorithm defined in this gear.
 
@@ -32,35 +32,31 @@
     dest_parent_type = destination_container.parent["type"]
     dest_parent_id = destination_container.parent["id"]
     dest_proj_id = destination_container.parents["project"]
     if protocol_name:
         # Ensure the protocol exists for that project
         # Protocol Names are unique within a project
         if not (
-            protocol := get_protocol_from_name(client, protocol_name, dest_proj_id)
+            protocol := get_protocol_from_name(
+                client, protocol_name=protocol_name, project_id=dest_proj_id
+            )
         ):
             log.error(
                 "Protocol %s not found for project (%s).", protocol_name, dest_proj_id
             )
             log.info(
                 "Check protocol definitions and project permissions for your API key."
             )
             return 1
 
         project_id = dest_proj_id
         form_id = protocol["form_id"]
 
-        filter_str = f"protocol_id={protocol['_id']}"
-        # If the destination container is a subject, session, or acquisition
-        if dest_parent_type in ["subject", "session", "acquisition"]:
-            filter_str += f",parents.{dest_parent_type}={dest_parent_id}"
-
-        tasks = client.get(
-            f"/api/readertasks/project/{project_id}",
-            params={"filter": filter_str},
+        tasks = get_project_tasks(
+            client, project_id, protocol["_id"], dest_parent_type, dest_parent_id
         )
 
     else:
         project_id = None
         form_id = None
         tasks = {"results": []}
```

## Comparing `fw_gear_form_and_annotations_exporter-0.0.4.dist-info/LICENSE` & `fw_gear_form_and_annotations_exporter-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_gear_form_and_annotations_exporter-0.0.4.dist-info/METADATA` & `fw_gear_form_and_annotations_exporter-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: fw-gear-form-and-annotations-exporter
-Version: 0.0.4
-Summary: This was created from [poetry-cow-says](https://gitlab.com/flywheel-io/flywheel-apps/templates/poetry-cow-says). Some things (packages in .toml, GUIDELINES.md, `tests/test_main.py` methods) were removed to remove conflicts for new gears. This gear does not do anything, just used as a "bare bones" template.
+Version: 0.0.5
+Summary: Export Form Responses and/or Annotations to CSV file(s).
 Home-page: https://gitlab.com/flywheel-io/scientific-solutions/gears/fw-gear-form-and-annotations-exporter
 License: MIT
 Keywords: Flywheel,Gears
 Author: Flywheel
 Author-email: support@flywheel.io
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: flywheel-gear-toolkit (>=0.6.10,<0.7.0)
-Requires-Dist: flywheel-sdk (>=16.19.0,<17.0.0)
-Requires-Dist: fw-client (>=0.5.0,<0.6.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: flywheel-gear-toolkit (>=0.6.11,<0.7.0)
+Requires-Dist: flywheel-sdk (>=17.0.0,<18.0.0)
+Requires-Dist: fw-client (>=0.5.1,<0.6.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://gitlab.com/flywheel-io/scientific-solutions/gears/fw-gear-form-and-annotations-exporter
 Description-Content-Type: text/markdown
 
 # Form and Annotation Exporter
 
 ## Overview
```

