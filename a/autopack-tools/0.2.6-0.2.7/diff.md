# Comparing `tmp/autopack_tools-0.2.6.tar.gz` & `tmp/autopack_tools-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.2.6.tar", max compression
+gzip compressed data, was "autopack_tools-0.2.7.tar", max compression
```

## Comparing `autopack_tools-0.2.6.tar` & `autopack_tools-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.6/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.6/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.6/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.6/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.6/autopack/__main__.py
--rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.6/autopack/api.py
--rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.6/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.6/autopack/errors.py
--rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.6/autopack/get_pack.py
--rw-r--r--   0        0        0     3877 2023-07-05 01:53:52.116169 autopack_tools-0.2.6/autopack/installation.py
--rw-r--r--   0        0        0     2921 2023-07-03 23:58:49.932953 autopack_tools-0.2.6/autopack/pack.py
--rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.6/autopack/pack_response.py
--rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.6/autopack/search.py
--rw-r--r--   0        0        0     4016 2023-07-05 01:53:01.972972 autopack_tools-0.2.6/autopack/selection.py
--rw-r--r--   0        0        0     4405 2023-07-05 01:53:52.129111 autopack_tools-0.2.6/autopack/utils.py
--rw-r--r--   0        0        0      911 2023-07-05 02:01:03.148675 autopack_tools-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 autopack_tools-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.7/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.7/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.7/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.7/autopack/__main__.py
+-rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.7/autopack/api.py
+-rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.7/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.7/autopack/errors.py
+-rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.7/autopack/get_pack.py
+-rw-r--r--   0        0        0     3804 2023-07-10 00:05:37.324848 autopack_tools-0.2.7/autopack/installation.py
+-rw-r--r--   0        0        0     2976 2023-07-10 03:48:17.484061 autopack_tools-0.2.7/autopack/pack.py
+-rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.7/autopack/pack_response.py
+-rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.7/autopack/search.py
+-rw-r--r--   0        0        0     2947 2023-07-10 00:06:33.061394 autopack_tools-0.2.7/autopack/selection.py
+-rw-r--r--   0        0        0     3874 2023-07-10 18:46:01.025051 autopack_tools-0.2.7/autopack/utils.py
+-rw-r--r--   0        0        0      911 2023-07-11 22:39:45.294645 autopack_tools-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 autopack_tools-0.2.7/PKG-INFO
```

### Comparing `autopack_tools-0.2.6/LICENSE` & `autopack_tools-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.6/README.md` & `autopack_tools-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.6/autopack/api.py` & `autopack_tools-0.2.7/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.6/autopack/cli.py` & `autopack_tools-0.2.7/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.6/autopack/get_pack.py` & `autopack_tools-0.2.7/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.6/autopack/installation.py` & `autopack_tools-0.2.7/autopack/installation.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 from git import Repo
 
 from autopack.api import PackResponse, get_pack_details
 from autopack.errors import AutoPackError, AutoPackInstallationError
 from autopack.get_pack import try_get_pack
 from autopack.pack import Pack
-from autopack.utils import (find_or_create_autopack_dir, load_metadata_file,
-                            write_metadata_file)
+from autopack.utils import find_or_create_autopack_dir, load_metadata_file, write_metadata_file
 
 
 def is_dependency_installed(dependency: str) -> bool:
     try:
         importlib.import_module(dependency)
         return True
     except ImportError:
@@ -38,17 +37,15 @@
     for dependency in dependencies:
         if is_dependency_installed(dependency):
             continue
 
         if force:
             install_dependency(dependency)
         else:
-            print(
-                f"This pack requires the dependency {dependency} to be installed. Continue?"
-            )
+            print(f"This pack requires the dependency {dependency} to be installed. Continue?")
             agree = input("[Yn]")
             if agree.lower() == "y" or agree == "":
                 install_dependency(dependency)
             else:
                 print(f"Skipping install of {dependency}")
 
 
@@ -86,45 +83,43 @@
     write_metadata_file(metadata)
 
 
 def install_pack(pack_id: str, force_dependencies=False) -> Pack:
     print(f"Installing pack: {pack_id}")
     find_or_create_autopack_dir()
 
-    pack = try_get_pack(pack_id, quiet=True)
+    pack = try_get_pack(pack_id, quiet=False)
     if pack:
         print(f"Pack {pack_id} already installed.")
         return pack
 
     try:
         pack_data = get_pack_details(pack_id, remote=True)
 
         if not pack_data:
-            raise AutoPackInstallationError(f"Could not find pack details")
+            raise AutoPackInstallationError("Could not find pack details")
 
         ask_to_install_dependencies(pack_data.dependencies, force_dependencies)
     except AutoPackError as e:
         # Maybe do something else
         raise AutoPackInstallationError(f"Could not install pack {e}")
     except BaseException as e:
         raise AutoPackInstallationError(f"Could not install pack {e}")
 
     git_dir = ""
     try:
         if pack_data.source == "git":
             git_dir = install_from_git(pack_data)
 
         update_metadata_file(pack_data)
-        pack = try_get_pack(pack_id, quiet=True)
+        pack = try_get_pack(pack_id, quiet=False)
 
         if pack:
             return pack
 
     except Exception as e:
         raise AutoPackInstallationError(f"Couldn't install pack due to error {e}")
 
     if git_dir and os.path.isdir(git_dir):
         shutil.rmtree(git_dir)
 
-    raise AutoPackInstallationError(
-        "Error: Installation completed but pack could still not be found."
-    )
+    raise AutoPackInstallationError("Error: Installation completed but pack could still not be found.")
```

### Comparing `autopack_tools-0.2.6/autopack/pack.py` & `autopack_tools-0.2.7/autopack/pack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Any, Optional
+from typing import Any, Optional, TYPE_CHECKING, TYPE_CHECKING
 
 from langchain.tools import BaseTool
 
-from autopack.api import PackResponse
+if TYPE_CHECKING:
+    from autopack.api import PackResponse
 
 
 class Pack(BaseTool):
     """
     Class to describe the Pack that is returned from get_pack calls. Wraps the Tool and provides metadata about the
     pack.
     """
@@ -69,15 +70,15 @@
     @property
     def is_single_input(self) -> bool:
         """Hack on top of BaseTool to allow 0-arg tools"""
         keys = {k for k in self.args if k != "kwargs"}
         return len(keys) <= 1
 
     @classmethod
-    def from_pack_data(cls, tool_class: BaseTool, pack_data: PackResponse):
+    def from_pack_data(cls, tool_class: BaseTool, pack_data: "PackResponse"):
         return cls(
             pack_id=pack_data.pack_id,
             author=pack_data.author,
             repo=pack_data.repo,
             module_path=pack_data.module_path,
             description=pack_data.description,
             name=pack_data.name,
@@ -88,7 +89,8 @@
             tool_class=tool_class,
         )
 
 
 def validate_tool_args(spec: dict[str, Any], actual: dict[str, Any]):
     # TODO: This. Plus maybe some helpful errors?
     return True
+
```

### Comparing `autopack_tools-0.2.6/autopack/pack_response.py` & `autopack_tools-0.2.7/autopack/pack_response.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.6/autopack/selection.py` & `autopack_tools-0.2.7/autopack/selection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,32 @@
 import json
 
 from langchain.chat_models.base import BaseChatModel
-from langchain.schema import HumanMessage, SystemMessage
+from langchain.schema import SystemMessage
 
 from autopack.api import pack_search
 
-TOOL_SELECTION_PROMPT_TEMPLATE = """You are an autonomous AI Assistant named AutoPack.
-
-AutoPack is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, AutoPack is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
-
-AutoPack is constantly learning and improving, and its capabilities are constantly evolving. It is able to process and understand large amounts of text, and can use this knowledge to provide accurate and informative responses to a wide range of questions. Additionally, AutoPack is able to generate its own text based on the input it receives, allowing it to engage in discussions and provide explanations and descriptions on a wide range of topics.
-
-Overall, AutoPack is a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether you need help with a specific question or just want to have a conversation about a particular topic, AutoPack is here to assist.
-
-AutoPack has access to the following tools:
+TOOL_SELECTION_PROMPT_TEMPLATE = """You are an autonomous AI Assistant named AutoPack. AutoPack works on behalf of another AI Assistant who will be completing tasks. AutoPack is excellent at choosing the right tools for the task. Keeping a small tool set is important, so AutoPack aims to include only the tools that are required. AutoPack has access to the following tools:
 --- TOOLS ---
 {tools_string}
 --- END TOOLS ---
-
 Respond with the following JSON structure:
 --- FORMAT INSTRUCTIONS ---
 ```json
 {{"tools": [{{ "tool_id": tool_id, "reason": reason_for_recommending }}] }}
 ```
-
 For example, if you think tool #1234 might be necessary:
-
 ```json
 {{'tools': [{{ "tool_id": 1234, "reason": "The breathe tool might be necessary because the user needs oxygen"}}]}}
 ```
 --- END FORMAT INSTRUCTIONS ---
-
-I am a human user who needs you to accomplish a task.
-First, I need you to narrow down the available tools to the ones that may be necessary to complete the following task.
-
 ---- TASK ----
 {user_input}
 --- END TASK ---
-
+Given the TASK, return all of the tools that are necessary to complete the task.
 Begin!"""
 
 
 def select_packs(task_description: str, llm: BaseChatModel) -> list[str]:
     """Given a user input describing the task they wish to accomplish, return a list of Pack IDs that the given LLM
     thinks will be suitable for this task.
 
@@ -59,25 +44,22 @@
     """
 
     packs = pack_search("")
     pack_summaries = ""
     for i, pack in enumerate(packs):
         # Use a number instead of a tool ID because the AI can mismatch tool names and repos
         pseudo_id = i + 1
-        pack_summaries += f"""--- START TOOL #{pseudo_id} ---
+        pack_summaries += f"""--- TOOL #{pseudo_id} ---
 tool_id: {pseudo_id}
 name: "{pack.name}"
 description: "{pack.description}"
 arguments: "{pack.run_args}"
---- END TOOL #{pseudo_id} ---
 """
 
-    prompt = TOOL_SELECTION_PROMPT_TEMPLATE.format(
-        user_input=task_description, tools_string=pack_summaries
-    )
+    prompt = TOOL_SELECTION_PROMPT_TEMPLATE.format(user_input=task_description, tools_string=pack_summaries)
 
     response = ask_llm(prompt, llm)
 
     tools = json.loads(response.content)
     # TODO Handle json errors, perhaps a retry
 
     selected_packs = []
```

### Comparing `autopack_tools-0.2.6/autopack/utils.py` & `autopack_tools-0.2.7/autopack/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import json
 import os
 import sys
 from json import JSONDecodeError
 from types import ModuleType
 from typing import Any, Type
 
-from autopack.errors import (AutoPackLoadError, AutoPackNotFoundError,
-                             AutoPackNotInstalledError)
+from autopack.errors import AutoPackLoadError, AutoPackNotFoundError, AutoPackNotInstalledError
 from autopack.pack import Pack
 from autopack.pack_response import PackResponse
 
 
 def find_or_create_autopack_dir(depth=0) -> str:
     """Try to find a suitable .autopack directory. Tries in this order:
     1. Directory specified in environment variable AUTOPACK_DIR
@@ -20,17 +19,15 @@
     3. Existing .autopack directory up to 3 directories up
     4. Creates an .autopack directory in current directory
     """
     env_dir = os.environ.get("AUTOPACK_DIR")
     if env_dir:
         return env_dir
 
-    autopack_dir = os.path.abspath(
-        os.path.join(os.getcwd(), *[os.pardir] * depth, ".autopack")
-    )
+    autopack_dir = os.path.abspath(os.path.join(os.getcwd(), *[os.pardir] * depth, ".autopack"))
 
     if not os.path.exists(autopack_dir) or not os.path.isdir(autopack_dir):
         if depth > 3:
             os.makedirs(".autopack", exist_ok=True)
             return ".autopack"
         return find_or_create_autopack_dir(depth=depth + 1)
 
@@ -88,47 +85,31 @@
         for _, obj in inspect.getmembers(module):
             if is_valid_pack(obj, pack_data.name):
                 return Pack(**{"tool_class": obj, **pack_data.__dict__})
 
         message = f"Pack {pack_data.pack_id} found, but {pack_data.name} is not found in its module"
         raise AutoPackNotFoundError(message)
     except ModuleNotFoundError:
-        message = f"Pack {pack_data.pack_id} is available but not installed. To install: autopack install {pack_data.pack_id}"
+        message = (
+            f"Pack {pack_data.pack_id} is available but not installed. To install: autopack install {pack_data.pack_id}"
+        )
         if not quiet:
             print(message)
         raise AutoPackNotInstalledError(message)
     except (ImportError, AttributeError) as e:
         message = f"Error loading {pack_data.pack_id}: {e}"
         if not quiet:
             print(message)
         raise AutoPackLoadError(message)
 
 
 def is_valid_pack(klass: Type, name: str):
     if not inspect.isclass(klass):
         return False
 
-    base_class_names = [k.__name__ for k in klass.__bases__]
-    roughly_adheres_to_interface = (
-        hasattr(klass, "run") or "BaseTool" in base_class_names
-    )
-    if not roughly_adheres_to_interface:
-        return False
-
-    # Pack name is the class name
-    if name == klass.__name__:
-        return True
-
-    # Pack class has a name class variable
-    if hasattr(klass, "name"):
-        if callable(klass.name):
-            klass_name = klass.name()
-        else:
-            klass_name = klass.name
-        return klass_name == name
-
-    # Pack class has a __fields__ class variable (e.g. LangChain's BaseTool)
     if hasattr(klass, "__fields__"):
         name_field = klass.__fields__.get("name")
-        return name_field and name_field.default == name
+        if name_field and name_field.default:
+            snaked_name = name_field.default.lower().replace(" ", "_")
+            return name_field and snaked_name == name
 
     return False
```

### Comparing `autopack_tools-0.2.6/pyproject.toml` & `autopack_tools-0.2.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.2.6"
+version = "0.2.7"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.2.6/PKG-INFO` & `autopack_tools-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.2.6
+Version: 0.2.7
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

