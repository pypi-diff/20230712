# Comparing `tmp/langsmith-0.0.3.tar.gz` & `tmp/langsmith-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsmith-0.0.3.tar", max compression
+gzip compressed data, was "langsmith-0.0.4.tar", max compression
```

## Comparing `langsmith-0.0.3.tar` & `langsmith-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     8006 2023-07-05 17:54:45.352295 langsmith-0.0.3/README.md
--rw-r--r--   0        0        0      478 2023-07-10 20:55:19.191988 langsmith-0.0.3/langsmith/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 17:54:45.352774 langsmith-0.0.3/langsmith/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-07-05 17:54:45.353156 langsmith-0.0.3/langsmith/cli/conf/nginx.conf
--rw-r--r--   0        0        0      315 2023-07-05 17:54:45.353418 langsmith-0.0.3/langsmith/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1198 2023-07-05 17:54:45.353810 langsmith-0.0.3/langsmith/cli/docker-compose.yaml
--rw-r--r--   0        0        0    14054 2023-07-05 17:54:45.354144 langsmith-0.0.3/langsmith/cli/main.py
--rw-r--r--   0        0        0    27876 2023-07-11 05:55:53.837648 langsmith-0.0.3/langsmith/client.py
--rw-r--r--   0        0        0      234 2023-07-05 17:54:45.355050 langsmith-0.0.3/langsmith/evaluation/__init__.py
--rw-r--r--   0        0        0     1411 2023-07-05 17:54:45.355316 langsmith-0.0.3/langsmith/evaluation/evaluator.py
--rw-r--r--   0        0        0     1529 2023-07-05 17:54:45.355546 langsmith-0.0.3/langsmith/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     9462 2023-07-05 17:54:45.355760 langsmith-0.0.3/langsmith/run_helpers.py
--rw-r--r--   0        0        0     6120 2023-07-05 17:54:45.356170 langsmith-0.0.3/langsmith/run_trees.py
--rw-r--r--   0        0        0     6503 2023-07-11 05:53:09.644342 langsmith-0.0.3/langsmith/schemas.py
--rw-r--r--   0        0        0     3683 2023-07-11 05:55:51.017340 langsmith-0.0.3/langsmith/utils.py
--rw-r--r--   0        0        0      878 2023-07-11 06:02:01.855164 langsmith-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8609 1970-01-01 00:00:00.000000 langsmith-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     8026 2023-07-12 06:32:31.833667 langsmith-0.0.4/README.md
+-rw-r--r--   0        0        0      478 2023-07-12 06:32:31.833667 langsmith-0.0.4/langsmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 06:32:31.833667 langsmith-0.0.4/langsmith/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-07-12 06:32:31.833667 langsmith-0.0.4/langsmith/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      143 2023-07-12 06:32:31.833667 langsmith-0.0.4/langsmith/cli/docker-compose.dev.yaml
+-rw-r--r--   0        0        0      315 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1186 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    14432 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/cli/main.py
+-rw-r--r--   0        0        0    27851 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/client.py
+-rw-r--r--   0        0        0      234 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/evaluation/__init__.py
+-rw-r--r--   0        0        0     1411 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1529 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     9462 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/run_helpers.py
+-rw-r--r--   0        0        0     6116 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/run_trees.py
+-rw-r--r--   0        0        0     6499 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/schemas.py
+-rw-r--r--   0        0        0     3647 2023-07-12 06:32:31.837667 langsmith-0.0.4/langsmith/utils.py
+-rw-r--r--   0        0        0      878 2023-07-12 06:32:31.837667 langsmith-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8629 1970-01-01 00:00:00.000000 langsmith-0.0.4/PKG-INFO
```

### Comparing `langsmith-0.0.3/README.md` & `langsmith-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # LangSmith Client SDK
 
-This package contains the Python client for interacting with the [LangSmith platform](https://www.langchain.plus/).
+This package contains the Python client for interacting with the [LangSmith platform](https://smith.langchain.com/).
 
 To install:
 
 ```bash
 pip install langsmith
 ```
 
 LangSmith helps you and your team develop and evaluate language models and intelligent agents. It is compatible with any LLM Application and provides seamless integration with [LangChain](https://github.com/hwchase17/langchain), a widely recognized open-source framework that simplifies the process for developers to create powerful language model applications.
 
 > **Note**: You can enjoy the benefits of LangSmith without using the LangChain open-source packages! To get started with your own proprietary framework, set up your account and then skip to [Logging Traces Outside LangChain](#logging-traces-outside-langchain).
 
 A typical workflow looks like:
 
-1. Set up an account with LangSmith or host your [local server](https://docs.langchain.plus/docs/getting-started/local_installation).
+1. Set up an account with LangSmith or host your [local server](https://docs.smith.langchain.com/docs/getting-started/local_installation).
 2. Log traces.
 3. Debug, Create Datasets, and Evaluate Runs.
 
 We'll walk through these steps in more detail below.
 
 ## 1. Connect to LangSmith
 
-Sign up for [LangSmith](https://www.langchain.plus/) using your GitHub, Discord accounts, or an email address and password. If you sign up with an email, make sure to verify your email address before logging in.
+Sign up for [LangSmith](https://smith.langchain.com/) using your GitHub, Discord accounts, or an email address and password. If you sign up with an email, make sure to verify your email address before logging in.
 
-Then, create a unique API key on the [Settings Page](https://www.langchain.plus/settings), which is found in the menu at the top right corner of the page.
+Then, create a unique API key on the [Settings Page](https://smith.langchain.com/settings), which is found in the menu at the top right corner of the page.
 
 Note: Save the API Key in a secure location. It will not be shown again.
 
 ## 2. Log Traces
 
 You can log traces natively in your LangChain application or using a LangSmith RunTree.
 
@@ -39,16 +39,16 @@
 1. **Copy the environment variables from the Settings Page and add them to your application.**
 
 Tracing can be activated by setting the following environment variables or by manually specifying the LangChainTracer.
 
 ```python
 import os
 os.environ["LANGCHAIN_TRACING_V2"] = "true"
-os.environ["LANGCHAIN_ENDPOINT"] = "https://api.langchain.plus" # or your own server
-os.environ["LANGCHAIN_API_KEY"] = "<YOUR-LANGCHAINPLUS-API-KEY>"
+os.environ["LANGCHAIN_ENDPOINT"] = "https://api.smith.langchain.com" # or your own server
+os.environ["LANGCHAIN_API_KEY"] = "<YOUR-LANGSMITH-API-KEY>"
 # os.environ["LANGCHAIN_PROJECT"] = "My Project Name" # Optional: "default" is used if not set
 ```
 
 > **Tip:** Projects are groups of traces. All runs are logged to a project. If not specified, the project is set to `default`.
 
 2. **Run an Agent, Chain, or Language Model in LangChain**
 
@@ -72,16 +72,16 @@
 LangChain code. You can connect either by setting the appropriate environment variables,
 or by directly specifying the connection information in the RunTree.
 
 1. **Copy the environment variables from the Settings Page and add them to your application.**
 
 ```python
 import os
-os.environ["LANGCHAIN_ENDPOINT"] = "https://api.langchain.plus" # or your own server
-os.environ["LANGCHAIN_API_KEY"] = "<YOUR-LANGCHAINPLUS-API-KEY>"
+os.environ["LANGCHAIN_ENDPOINT"] = "https://api.smith.langchain.com" # or your own server
+os.environ["LANGCHAIN_API_KEY"] = "<YOUR-LANGSMITH-API-KEY>"
 # os.environ["LANGCHAIN_PROJECT"] = "My Project Name" # Optional: "default" is used if not set
 ```
 
 2. **Log traces using a RunTree.**
 
 A RunTree tracks your application. Each RunTree object is required to have a `name` and `run_type`. These and other important attributes are as follows:
 
@@ -153,15 +153,15 @@
 res.result()
 ```
 
 ## Create a Dataset from Existing Runs
 
 Once your runs are stored in LangSmith, you can convert them into a dataset.
 For this example, we will do so using the Client, but you can also do this using
-the web interface, as explained in the [LangSmith docs](https://docs.langchain.plus/docs/).
+the web interface, as explained in the [LangSmith docs](https://docs.smith.langchain.com/docs/).
 
 ```python
 from langsmith import Client
 
 client = Client()
 dataset_name = "Example Dataset"
 # We will only use examples from the top level AgentExecutor run here,
@@ -218,8 +218,8 @@
 )
 for run in runs:
     client.evaluate_run(run, evaluator)
 ```
 
 ## Additional Documentation
 
-To learn more about the LangSmith platform, check out the [docs](https://docs.langchain.plus/docs/).
+To learn more about the LangSmith platform, check out the [docs](https://docs.smith.langchain.com/docs/).
```

### Comparing `langsmith-0.0.3/langsmith/cli/main.py` & `langsmith-0.0.4/langsmith/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,68 +160,77 @@
     """Manage the LangSmith Tracing server."""
 
     def __init__(self) -> None:
         self.docker_compose_command = get_docker_compose_command()
         self.docker_compose_file = (
             Path(__file__).absolute().parent / "docker-compose.yaml"
         )
+        self.docker_compose_dev_file = (
+            Path(__file__).absolute().parent / "docker-compose.dev.yaml"
+        )
         self.ngrok_path = Path(__file__).absolute().parent / "docker-compose.ngrok.yaml"
 
     def _open_browser(self, url: str) -> None:
         try:
             subprocess.run(["open", url])
         except FileNotFoundError:
             pass
 
-    def _start_local(self) -> None:
+    def _start_local(self, dev: bool) -> None:
         command = [
             *self.docker_compose_command,
             "-f",
             str(self.docker_compose_file),
         ]
+        if dev:
+            command.append("-f")
+            command.append(str(self.docker_compose_dev_file))
         subprocess.run(
             [
                 *command,
                 "up",
                 "--quiet-pull",
                 "--wait",
             ]
         )
         logger.info(
-            "langchain plus server is running at http://localhost:1984.  To connect"
+            "LangSmith server is running at http://localhost:1984.  To connect"
             " locally, set the following environment variable"
             " when running your LangChain application."
         )
 
         logger.info("\tLANGCHAIN_TRACING_V2=true")
         self._open_browser("http://localhost")
 
-    def _start_and_expose(self, auth_token: Optional[str]) -> None:
+    def _start_and_expose(self, auth_token: Optional[str], dev: bool) -> None:
         with create_ngrok_config(auth_token=auth_token):
             command = [
                 *self.docker_compose_command,
                 "-f",
                 str(self.docker_compose_file),
                 "-f",
                 str(self.ngrok_path),
             ]
+            if dev:
+                command.append("-f")
+                command.append(str(self.docker_compose_dev_file))
             subprocess.run(
                 [
                     *command,
                     "up",
                     "--quiet-pull",
                     "--wait",
                 ]
             )
         logger.info(
             "ngrok is running. You can view the dashboard at http://0.0.0.0:4040"
         )
         ngrok_url = get_ngrok_url(auth_token)
         logger.info(
-            "langchain plus server is running at http://localhost:1984."
+            "LangSmith server is running at http://localhost:1984."
             " To connect remotely, set the following environment"
             " variable when running your LangChain application."
         )
         logger.info("\tLANGCHAIN_TRACING_V2=true")
         logger.info(f"\tLANGCHAIN_ENDPOINT={ngrok_url}")
         self._open_browser("http://0.0.0.0:4040")
         self._open_browser("http://localhost")
@@ -233,15 +242,15 @@
     ) -> None:
         """Pull the latest LangSmith images.
 
         Args:
             dev: If True, pull the development (rc) image of LangSmith.
         """
         if dev:
-            os.environ["_LANGCHAINPLUS_IMAGE_PREFIX"] = "rc-"
+            os.environ["_LANGSMITH_IMAGE_PREFIX"] = "rc-"
         subprocess.run(
             [
                 *self.docker_compose_command,
                 "-f",
                 str(self.docker_compose_file),
                 "pull",
             ]
@@ -264,22 +273,22 @@
             dev: If True, use the development (rc) image of LangSmith.
             openai_api_key: The OpenAI API key to use for LangSmith
                 If not provided, the OpenAI API Key will be read from the
                 OPENAI_API_KEY environment variable. If neither are provided,
                 some features of LangSmith will not be available.
         """
         if dev:
-            os.environ["_LANGCHAINPLUS_IMAGE_PREFIX"] = "rc-"
+            os.environ["_LANGSMITH_IMAGE_PREFIX"] = "rc-"
         if openai_api_key is not None:
             os.environ["OPENAI_API_KEY"] = openai_api_key
         self.pull(dev=dev)
         if expose:
-            self._start_and_expose(auth_token=auth_token)
+            self._start_and_expose(auth_token=auth_token, dev=dev)
         else:
-            self._start_local()
+            self._start_local(dev=dev)
 
     def stop(self) -> None:
         """Stop the LangSmith server."""
         subprocess.run(
             [
                 *self.docker_compose_command,
                 "-f",
```

### Comparing `langsmith-0.0.3/langsmith/client.py` & `langsmith-0.0.4/langsmith/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     Run,
     RunBase,
     RunTypeEnum,
     TracerSession,
     TracerSessionResult,
 )
 from langsmith.utils import (
-    LangChainPlusAPIError,
-    LangChainPlusError,
-    LangChainPlusUserError,
+    LangSmithAPIError,
+    LangSmithError,
+    LangSmithUserError,
     get_runtime_environment,
     raise_for_status_with_text,
     request_with_retries,
     xor_args,
 )
 
 if TYPE_CHECKING:
@@ -83,15 +83,15 @@
 ID_TYPE = Union[UUID, str]
 
 
 def _default_retry_config() -> Dict[str, Any]:
     return dict(
         stop=stop_after_attempt(3),
         wait=wait_exponential(multiplier=1, min=4, max=10),
-        retry=retry_if_exception_type(LangChainPlusAPIError),
+        retry=retry_if_exception_type(LangSmithAPIError),
         before_sleep=before_sleep_log(logger, logging.WARNING),
     )
 
 
 def _serialize_json(obj: Any) -> str:
     if isinstance(obj, datetime):
         return obj.isoformat()
@@ -113,27 +113,27 @@
     @root_validator(pre=True)
     def validate_api_key_if_hosted(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Verify API key is provided if url not localhost."""
         api_url: str = values.get("api_url", "http://localhost:1984")
         api_key: Optional[str] = values.get("api_key")
         if not _is_localhost(api_url):
             if not api_key:
-                raise LangChainPlusUserError(
+                raise LangSmithUserError(
                     "API key must be provided when using hosted LangSmith API"
                 )
         return values
 
     def _repr_html_(self) -> str:
         """Return an HTML representation of the instance with a link to the URL."""
         if _is_localhost(self.api_url):
             link = "http://localhost"
         elif "dev" in self.api_url.split(".", maxsplit=1)[0]:
-            link = "https://dev.langchain.plus"
+            link = "https://dev.smith.langchain.com/"
         else:
-            link = "https://www.langchain.plus"
+            link = "https://smith.langchain.com"
         return f'<a href="{link}", target="_blank" rel="noopener">LangSmith Client</a>'
 
     def __repr__(self) -> str:
         """Return a string representation of the instance with a link to the URL."""
         return f"Client (API URL: {self.api_url})"
 
     @property
@@ -313,15 +313,15 @@
 
     def _load_child_runs(self, run: Run) -> Run:
         child_runs = self.list_runs(id=run.child_run_ids)
         treemap: DefaultDict[UUID, List[Run]] = defaultdict(list)
         runs: Dict[UUID, Run] = {}
         for child_run in sorted(child_runs, key=lambda r: r.execution_order):
             if child_run.parent_run_id is None:
-                raise LangChainPlusError(f"Child run {child_run.id} has no parent")
+                raise LangSmithError(f"Child run {child_run.id} has no parent")
             treemap[child_run.parent_run_id].append(child_run)
             runs[child_run.id] = child_run
         run.child_runs = treemap.pop(run.id, [])
         for run_id, children in treemap.items():
             runs[run_id].child_runs = children
         return run
 
@@ -425,15 +425,15 @@
             params["name"] = project_name
         else:
             raise ValueError("Must provide project_name or project_id")
         response = self._get_with_retries(path, params=params)
         result = response.json()
         if isinstance(result, list):
             if len(result) == 0:
-                raise LangChainPlusError(f"Project {project_name} not found")
+                raise LangSmithError(f"Project {project_name} not found")
             return TracerSessionResult(**result[0])
         return TracerSessionResult(**response.json())
 
     def list_projects(self) -> Iterator[TracerSession]:
         """List projects from the LangSmith API."""
         yield from (
             TracerSession(**project)
@@ -494,15 +494,15 @@
         response = self._get_with_retries(
             path,
             params=params,
         )
         result = response.json()
         if isinstance(result, list):
             if len(result) == 0:
-                raise LangChainPlusError(f"Dataset {dataset_name} not found")
+                raise LangSmithError(f"Dataset {dataset_name} not found")
             return Dataset(**result[0])
         return Dataset(**result)
 
     def list_datasets(self) -> Iterator[Dataset]:
         """List the datasets on the LangSmith API."""
         yield from (
             Dataset(**dataset) for dataset in self._get_paginated_list("/datasets")
```

### Comparing `langsmith-0.0.3/langsmith/evaluation/evaluator.py` & `langsmith-0.0.4/langsmith/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.3/langsmith/evaluation/string_evaluator.py` & `langsmith-0.0.4/langsmith/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.3/langsmith/run_helpers.py` & `langsmith-0.0.4/langsmith/run_helpers.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.3/langsmith/run_trees.py` & `langsmith-0.0.4/langsmith/run_trees.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Schemas for the langchainplus API."""
+"""Schemas for the LangSmith API."""
 from __future__ import annotations
 
 import logging
 import os
 from concurrent.futures import Future, ThreadPoolExecutor, wait
 from datetime import datetime
 from typing import Dict, List, Optional, Union, cast
```

### Comparing `langsmith-0.0.3/langsmith/schemas.py` & `langsmith-0.0.4/langsmith/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Schemas for the langchainplus API."""
+"""Schemas for the LangSmith API."""
 from __future__ import annotations
 
 from datetime import datetime, timedelta
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
```

### Comparing `langsmith-0.0.3/langsmith/utils.py` & `langsmith-0.0.4/langsmith/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,59 +4,59 @@
 from typing import Any, Callable, Mapping, Tuple
 
 import requests
 from requests import ConnectionError, HTTPError, Response
 from tenacity import Retrying
 
 
-class LangChainPlusAPIError(Exception):
+class LangSmithAPIError(Exception):
     """An error occurred while communicating with the LangChain API."""
 
 
-class LangChainPlusUserError(Exception):
+class LangSmithUserError(Exception):
     """An error occurred while communicating with the LangChain API."""
 
 
-class LangChainPlusError(Exception):
+class LangSmithError(Exception):
     """An error occurred while communicating with the LangChain API."""
 
 
-class LangChainPlusConnectionError(Exception):
+class LangSmithConnectionError(Exception):
     """Couldn't connect to the LC+ API."""
 
 
 def request_with_retries(
     request_method: str, url: str, request_kwargs: Mapping, retry_config: Mapping
 ) -> Response:
     for attempt in Retrying(**retry_config):
         with attempt:
             try:
                 response = requests.request(request_method, url, **request_kwargs)
                 raise_for_status_with_text(response)
                 return response
             except HTTPError as e:
                 if response is not None and response.status_code == 500:
-                    raise LangChainPlusAPIError(
+                    raise LangSmithAPIError(
                         f"Server error caused failure to {request_method} {url} in"
                         f" LangSmith API. {e}"
                     )
                 else:
-                    raise LangChainPlusUserError(
+                    raise LangSmithUserError(
                         f"Failed to {request_method} {url} in LangSmith API. {e}"
                     )
             except ConnectionError as e:
-                raise LangChainPlusConnectionError(
+                raise LangSmithConnectionError(
                     f"Connection error caused failure to {request_method} {url}"
                     "  in LangSmith API. Please confirm your LANGCHAIN_ENDPOINT."
                 ) from e
             except Exception as e:
-                raise LangChainPlusError(
+                raise LangSmithError(
                     f"Failed to {request_method} {url} in LangSmith API. {e}"
                 ) from e
-    raise LangChainPlusError(f"Failed to {request_method}  {url} in LangSmith API. ")
+    raise LangSmithError(f"Failed to {request_method}  {url} in LangSmith API. ")
 
 
 def xor_args(*arg_groups: Tuple[str, ...]) -> Callable:
     """Validate specified keyword args are mutually exclusive."""
 
     def decorator(func: Callable) -> Callable:
         def wrapper(*args: Any, **kwargs: Any) -> Callable:
```

### Comparing `langsmith-0.0.3/pyproject.toml` & `langsmith-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langsmith"
-version = "0.0.3"
+version = "0.0.4"
 description = "Client library to connect to the LangSmith LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langsmith"}]
 
 [tool.poetry.scripts]
```

### Comparing `langsmith-0.0.3/PKG-INFO` & `langsmith-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsmith
-Version: 0.0.3
+Version: 0.0.4
 Summary: Client library to connect to the LangSmith LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -13,39 +13,39 @@
 Requires-Dist: pydantic (>=1,<2)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Description-Content-Type: text/markdown
 
 # LangSmith Client SDK
 
-This package contains the Python client for interacting with the [LangSmith platform](https://www.langchain.plus/).
+This package contains the Python client for interacting with the [LangSmith platform](https://smith.langchain.com/).
 
 To install:
 
 ```bash
 pip install langsmith
 ```
 
 LangSmith helps you and your team develop and evaluate language models and intelligent agents. It is compatible with any LLM Application and provides seamless integration with [LangChain](https://github.com/hwchase17/langchain), a widely recognized open-source framework that simplifies the process for developers to create powerful language model applications.
 
 > **Note**: You can enjoy the benefits of LangSmith without using the LangChain open-source packages! To get started with your own proprietary framework, set up your account and then skip to [Logging Traces Outside LangChain](#logging-traces-outside-langchain).
 
 A typical workflow looks like:
 
-1. Set up an account with LangSmith or host your [local server](https://docs.langchain.plus/docs/getting-started/local_installation).
+1. Set up an account with LangSmith or host your [local server](https://docs.smith.langchain.com/docs/getting-started/local_installation).
 2. Log traces.
 3. Debug, Create Datasets, and Evaluate Runs.
 
 We'll walk through these steps in more detail below.
 
 ## 1. Connect to LangSmith
 
-Sign up for [LangSmith](https://www.langchain.plus/) using your GitHub, Discord accounts, or an email address and password. If you sign up with an email, make sure to verify your email address before logging in.
+Sign up for [LangSmith](https://smith.langchain.com/) using your GitHub, Discord accounts, or an email address and password. If you sign up with an email, make sure to verify your email address before logging in.
 
-Then, create a unique API key on the [Settings Page](https://www.langchain.plus/settings), which is found in the menu at the top right corner of the page.
+Then, create a unique API key on the [Settings Page](https://smith.langchain.com/settings), which is found in the menu at the top right corner of the page.
 
 Note: Save the API Key in a secure location. It will not be shown again.
 
 ## 2. Log Traces
 
 You can log traces natively in your LangChain application or using a LangSmith RunTree.
 
@@ -56,16 +56,16 @@
 1. **Copy the environment variables from the Settings Page and add them to your application.**
 
 Tracing can be activated by setting the following environment variables or by manually specifying the LangChainTracer.
 
 ```python
 import os
 os.environ["LANGCHAIN_TRACING_V2"] = "true"
-os.environ["LANGCHAIN_ENDPOINT"] = "https://api.langchain.plus" # or your own server
-os.environ["LANGCHAIN_API_KEY"] = "<YOUR-LANGCHAINPLUS-API-KEY>"
+os.environ["LANGCHAIN_ENDPOINT"] = "https://api.smith.langchain.com" # or your own server
+os.environ["LANGCHAIN_API_KEY"] = "<YOUR-LANGSMITH-API-KEY>"
 # os.environ["LANGCHAIN_PROJECT"] = "My Project Name" # Optional: "default" is used if not set
 ```
 
 > **Tip:** Projects are groups of traces. All runs are logged to a project. If not specified, the project is set to `default`.
 
 2. **Run an Agent, Chain, or Language Model in LangChain**
 
@@ -89,16 +89,16 @@
 LangChain code. You can connect either by setting the appropriate environment variables,
 or by directly specifying the connection information in the RunTree.
 
 1. **Copy the environment variables from the Settings Page and add them to your application.**
 
 ```python
 import os
-os.environ["LANGCHAIN_ENDPOINT"] = "https://api.langchain.plus" # or your own server
-os.environ["LANGCHAIN_API_KEY"] = "<YOUR-LANGCHAINPLUS-API-KEY>"
+os.environ["LANGCHAIN_ENDPOINT"] = "https://api.smith.langchain.com" # or your own server
+os.environ["LANGCHAIN_API_KEY"] = "<YOUR-LANGSMITH-API-KEY>"
 # os.environ["LANGCHAIN_PROJECT"] = "My Project Name" # Optional: "default" is used if not set
 ```
 
 2. **Log traces using a RunTree.**
 
 A RunTree tracks your application. Each RunTree object is required to have a `name` and `run_type`. These and other important attributes are as follows:
 
@@ -170,15 +170,15 @@
 res.result()
 ```
 
 ## Create a Dataset from Existing Runs
 
 Once your runs are stored in LangSmith, you can convert them into a dataset.
 For this example, we will do so using the Client, but you can also do this using
-the web interface, as explained in the [LangSmith docs](https://docs.langchain.plus/docs/).
+the web interface, as explained in the [LangSmith docs](https://docs.smith.langchain.com/docs/).
 
 ```python
 from langsmith import Client
 
 client = Client()
 dataset_name = "Example Dataset"
 # We will only use examples from the top level AgentExecutor run here,
@@ -235,9 +235,9 @@
 )
 for run in runs:
     client.evaluate_run(run, evaluator)
 ```
 
 ## Additional Documentation
 
-To learn more about the LangSmith platform, check out the [docs](https://docs.langchain.plus/docs/).
+To learn more about the LangSmith platform, check out the [docs](https://docs.smith.langchain.com/docs/).
```

