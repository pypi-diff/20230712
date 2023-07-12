# Comparing `tmp/stactask-0.1.0b5.tar.gz` & `tmp/stactask-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactask-0.1.0b5.tar", last modified: Sun Oct 23 21:32:23 2022, max compression
+gzip compressed data, was "stactask-0.1.1.tar", last modified: Wed Jul 12 14:38:15 2023, max compression
```

## Comparing `stactask-0.1.0b5.tar` & `stactask-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 21:32:23.857278 stactask-0.1.0b5/
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-10-23 21:32:13.000000 stactask-0.1.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-10-23 21:32:23.857278 stactask-0.1.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5548 2022-10-23 21:32:13.000000 stactask-0.1.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-23 21:32:23.857278 stactask-0.1.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-10-23 21:32:13.000000 stactask-0.1.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 21:32:23.853278 stactask-0.1.0b5/stactask/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-10-23 21:32:13.000000 stactask-0.1.0b5/stactask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4384 2022-10-23 21:32:13.000000 stactask-0.1.0b5/stactask/asset_io.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-10-23 21:32:13.000000 stactask-0.1.0b5/stactask/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12316 2022-10-23 21:32:13.000000 stactask-0.1.0b5/stactask/task.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-10-23 21:32:13.000000 stactask-0.1.0b5/stactask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 21:32:23.857278 stactask-0.1.0b5/stactask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-10-23 21:32:23.000000 stactask-0.1.0b5/stactask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-10-23 21:32:23.000000 stactask-0.1.0b5/stactask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 21:32:23.000000 stactask-0.1.0b5/stactask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-23 21:32:23.000000 stactask-0.1.0b5/stactask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 21:32:23.000000 stactask-0.1.0b5/stactask.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-23 21:32:23.000000 stactask-0.1.0b5/stactask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-23 21:32:23.000000 stactask-0.1.0b5/stactask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:38:15.005290 stactask-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-12 14:38:01.000000 stactask-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 14:38:01.000000 stactask-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-12 14:38:15.005290 stactask-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-12 14:38:01.000000 stactask-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 14:38:01.000000 stactask-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:38:15.005290 stactask-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-12 14:38:01.000000 stactask-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:38:15.005290 stactask-0.1.1/stactask/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 14:38:01.000000 stactask-0.1.1/stactask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-12 14:38:01.000000 stactask-0.1.1/stactask/asset_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-12 14:38:01.000000 stactask-0.1.1/stactask/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:38:01.000000 stactask-0.1.1/stactask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-12 14:38:01.000000 stactask-0.1.1/stactask/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-12 14:38:01.000000 stactask-0.1.1/stactask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:38:15.005290 stactask-0.1.1/stactask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-12 14:38:14.000000 stactask-0.1.1/stactask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-12 14:38:14.000000 stactask-0.1.1/stactask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:38:14.000000 stactask-0.1.1/stactask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:38:14.000000 stactask-0.1.1/stactask.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 14:38:14.000000 stactask-0.1.1/stactask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 14:38:14.000000 stactask-0.1.1/stactask.egg-info/top_level.txt
```

### Comparing `stactask-0.1.0b5/LICENSE` & `stactask-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stactask-0.1.0b5/PKG-INFO` & `stactask-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactask
-Version: 0.1.0b5
+Version: 0.1.1
 Summary: STAC Task class provides a class interface for running custom algorithms on STAC Items
 Home-page: https://github.com/stac-utils/stac-task
 Author: Matthew Hanson
 Author-email: matt.a.hanson@gmail.com
 License: Apache Software License 2.0
 Project-URL: Tracker, https://github.com/stac-utils/stactask/issues
 Keywords: pystac,imagery,raster,catalog,STAC
@@ -165,23 +165,26 @@
     "description": "My process configuration",
     "collections": {
         "landsat-c2l2": "$[?(@.id =~ 'LC08.*')]"
     },
     "upload_options": {
         "path_template": "s3://my-bucket/${collection}/${year}/${month}/${day}/${id}"
     },
-    "tasks": {
-        "task-name": {
-            "param": "value"
+    "tasks": [
+        {
+            "name": "task-name"
+            "parameters": {
+                "param": "value"
+            }
         }
-    }
+    ]
 }
 ```
 
 
 ## Development
 
 ### run tests
 
 ```
-$ pytest -v -s tests
+$ ./scripts/test
 ```
```

### Comparing `stactask-0.1.0b5/README.md` & `stactask-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -140,23 +140,26 @@
     "description": "My process configuration",
     "collections": {
         "landsat-c2l2": "$[?(@.id =~ 'LC08.*')]"
     },
     "upload_options": {
         "path_template": "s3://my-bucket/${collection}/${year}/${month}/${day}/${id}"
     },
-    "tasks": {
-        "task-name": {
-            "param": "value"
+    "tasks": [
+        {
+            "name": "task-name"
+            "parameters": {
+                "param": "value"
+            }
         }
-    }
+    ]
 }
 ```
 
 
 ## Development
 
 ### run tests
 
 ```
-$ pytest -v -s tests
+$ ./scripts/test
 ```
```

### Comparing `stactask-0.1.0b5/setup.py` & `stactask-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open(os.path.join(here, "README.md")) as readme_file:
     readme = readme_file.read()
 
 
 setup(
     name="stactask",
-    version="0.1.0b5",
+    version="0.1.1",
     description=(
         "STAC Task class provides a class interface for running custom algorithms on STAC Items"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Matthew Hanson",
     author_email="matt.a.hanson@gmail.com",
@@ -50,9 +50,8 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     project_urls={
         "Tracker": "https://github.com/stac-utils/stactask/issues",
     },
     test_suite="tests",
-    entry_points={"console_scripts": ["stac-task = stactask.cli:cli"]},
 )
```

### Comparing `stactask-0.1.0b5/stactask/asset_io.py` & `stactask-0.1.1/stactask/asset_io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import asyncio
 import logging
 import os
 from os import path as op
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import fsspec
 from boto3utils import s3
+from fsspec import AbstractFileSystem
 from pystac import Item
 from pystac.layout import LayoutTemplate
 
 logger = logging.getLogger(__name__)
 
 # global dictionary of sessions per bucket
 s3_client = s3()
 
-SIMULTANEOUS_DOWNLOADS = os.getenv("STAC_SIMULTANEOUS_DOWNLOADS", 3)
+SIMULTANEOUS_DOWNLOADS = int(os.getenv("STAC_SIMULTANEOUS_DOWNLOADS", 3))
 sem = asyncio.Semaphore(SIMULTANEOUS_DOWNLOADS)
 
 
-async def download_file(fs, src, dest):
+async def download_file(fs: AbstractFileSystem, src: str, dest: str) -> None:
     async with sem:
         logger.debug(f"{src} start")
         await fs._get_file(src, dest)
         logger.debug(f"{src} completed")
 
 
 async def download_item_assets(
     item: Item,
     assets: Optional[List[str]] = None,
-    save_item: Optional[bool] = True,
-    overwrite: Optional[bool] = False,
-    path_template: Optional[str] = "${collection}/${id}",
-    absolute_path: Optional[bool] = False,
-    **kwargs,
-):
-
+    save_item: bool = True,
+    overwrite: bool = False,
+    path_template: str = "${collection}/${id}",
+    absolute_path: bool = False,
+    **kwargs: Any,
+) -> Item:
     _assets = item.assets.keys() if assets is None else assets
 
     # determine path from template and item
     layout = LayoutTemplate(path_template)
     path = layout.substitute(item)
 
     # make necessary directories
@@ -73,52 +73,64 @@
     if save_item:
         new_item.remove_links("root")
         new_item.save_object(dest_href=os.path.join(path, "item.json"))
 
     return new_item
 
 
-async def download_items_assets(items, **kwargs):
+async def download_items_assets(items: List[Item], **kwargs: Any) -> List[Item]:
     tasks = []
     for item in items:
         tasks.append(asyncio.create_task(download_item_assets(item, **kwargs)))
-    new_items = await asyncio.gather(*tasks)
+    new_items: List[Item] = await asyncio.gather(*tasks)
     return new_items
 
 
 def upload_item_assets_to_s3(
     item: Item,
-    assets: List[str] = None,
-    public_assets: List[str] = [],
+    assets: Optional[List[str]] = None,
+    public_assets: Union[None, List[str], str] = None,
     path_template: str = "${collection}/${id}",
     s3_urls: bool = False,
-    headers: Dict = {},
-    **kwargs,
-) -> Dict:
+    headers: Optional[Dict[str, Any]] = None,
+    **kwargs: Any,
+) -> Item:
     """Upload Item assets to s3 bucket
     Args:
         item (Dict): STAC Item
         assets (List[str], optional): List of asset keys to upload. Defaults to None.
-        public_assets (List[str], optional): List of assets keys that should be public. Defaults to [].
-        path_template (str, optional): Path string template. Defaults to '${collection}/${id}'.
-        s3_urls (bool, optional): Return s3 URLs instead of http URLs. Defaults to False.
-        headers (Dict, optional): Dictionary of headers to set on uploaded assets. Defaults to {},
+        public_assets (List[str], optional): List of assets keys that should be
+            public. Defaults to [].
+        path_template (str, optional): Path string template. Defaults to
+            '${collection}/${id}'.
+        s3_urls (bool, optional): Return s3 URLs instead of http URLs. Defaults
+            to False.
+        headers (Dict, optional): Dictionary of headers to set on uploaded
+            assets. Defaults to {},
     Returns:
         Dict: A new STAC Item with uploaded assets pointing to newly uploaded file URLs
     """
+    if headers is None:
+        headers = {}
+
     # deepcopy of item
     _item = item.to_dict()
 
+    if public_assets is None:
+        public_assets = []
+    # determine which assets should be public
+    elif type(public_assets) is str:
+        if public_assets == "ALL":
+            public_assets = list(_item["assets"].keys())
+        else:
+            raise ValueError(f"unexpected value for `public_assets`: {public_assets}")
+
     # if assets not provided, upload all assets
     _assets = assets if assets is not None else _item["assets"].keys()
 
-    # determine which assets should be public
-    if type(public_assets) is str and public_assets == "ALL":
-        public_assets = _item["assets"].keys()
-
     for key in [a for a in _assets if a in _item["assets"].keys()]:
         asset = _item["assets"][key]
         filename = asset["href"]
         if not op.exists(filename):
             logger.warning(f"Cannot upload {filename}: does not exist")
             continue
         public = True if key in public_assets else False
```

### Comparing `stactask-0.1.0b5/stactask/task.py` & `stactask-0.1.1/stactask/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,32 +7,33 @@
 import warnings
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from os import makedirs
 from pathlib import Path
 from shutil import rmtree
 from tempfile import mkdtemp
-from typing import Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 import fsspec
-from pystac import ItemCollection
+from pystac import Item, ItemCollection
 
 from .asset_io import (
     download_item_assets,
     download_items_assets,
     upload_item_assets_to_s3,
 )
 from .exceptions import FailedValidation
 from .utils import stac_jsonpath_match
 
 # types
 PathLike = Union[str, Path]
 """
-Tasks can use parameters provided in a `process` Dictionary that is supplied in the ItemCollection
-JSON under the "process" field. An example process definition:
+Tasks can use parameters provided in a `process` Dictionary that is supplied in
+the ItemCollection JSON under the "process" field. An example process
+definition:
 
 ```
 {
     "description": "My process configuration"
     "upload_options": {
         "path_template": "s3://my-bucket/${collection}/${year}/${month}/${day}/${id}",
         "collections": {
@@ -49,26 +50,25 @@
     ]
 }
 ```
 """
 
 
 class Task(ABC):
-
     name = "task"
     description = "A task for doing things"
     version = "0.1.0"
 
     def __init__(
         self: "Task",
-        payload: Dict,
+        payload: Dict[str, Any],
         workdir: Optional[PathLike] = None,
-        save_workdir: Optional[bool] = False,
-        skip_upload: Optional[bool] = False,
-        skip_validation: Optional[bool] = False,
+        save_workdir: bool = False,
+        skip_upload: bool = False,
+        skip_validation: bool = False,
     ):
         # set up logger
         self.logger = logging.getLogger(self.name)
 
         # set this to avoid confusion in destructor if called during validation
         self._save_workdir = True
 
@@ -85,155 +85,166 @@
         # create temporary work directory if workdir is None
         if workdir is None:
             self._workdir = Path(mkdtemp())
         else:
             self._workdir = Path(workdir)
             makedirs(self._workdir, exist_ok=True)
 
-    def __del__(self):
+    def __del__(self) -> None:
         # remove work directory if not running locally
         if not self._save_workdir:
             self.logger.debug("Removing work directory %s", self._workdir)
             rmtree(self._workdir)
 
     @property
-    def process_definition(self) -> Dict:
+    def process_definition(self) -> Dict[str, Any]:
         return self._payload.get("process", {})
 
     @property
-    def parameters(self) -> Dict:
+    def parameters(self) -> Dict[str, Any]:
         task_configs = self.process_definition.get("tasks", [])
         if isinstance(task_configs, List):
             # tasks is a list
-            task_config = [cfg for cfg in task_configs if cfg["name"] == self.name]
-            if len(task_config) == 0:
-                task_config = {}
+            task_config_list = [cfg for cfg in task_configs if cfg["name"] == self.name]
+            if len(task_config_list) == 0:
+                return {}
             else:
-                task_config = task_config[0]
-            return task_config.get("parameters", {})
+                task_config: Dict[str, Any] = task_config_list[0]
+                return task_config.get("parameters", {})
         elif isinstance(task_configs, Dict):
             # tasks is a dictionary of parameters (deprecated)
             warnings.warn(
                 "task configs is Dictionary (deprecated), convert to List ",
                 DeprecationWarning,
                 stacklevel=2,
             )
             return task_configs.get(self.name, {})
+        else:
+            raise ValueError(f"unexpected value for 'tasks': {task_configs}")
 
     @property
-    def upload_options(self) -> Dict:
+    def upload_options(self) -> Dict[str, Any]:
         return self.process_definition.get("upload_options", {})
 
     @property
-    def items_as_dicts(self) -> List[Dict]:
+    def items_as_dicts(self) -> List[Dict[str, Any]]:
         return self._payload.get("features", [])
 
     @property
     def items(self) -> ItemCollection:
         items_dict = {"type": "FeatureCollection", "features": self.items_as_dicts}
         return ItemCollection.from_dict(items_dict, preserve_dict=True)
 
     @classmethod
-    def validate(cls, payload: Dict) -> bool:
+    def validate(cls, payload: Dict[str, Any]) -> bool:
         # put validation logic on input Items and process definition here
         return True
 
     @classmethod
-    def add_software_version(cls, items: List[Dict]):
+    def add_software_version(cls, items: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         processing_ext = (
             "https://stac-extensions.github.io/processing/v1.1.0/schema.json"
         )
         for i in items:
             if "stac_extensions" not in i:
                 i["stac_extensions"] = []
             i["stac_extensions"].append(processing_ext)
             i["stac_extensions"] = list(set(i["stac_extensions"]))
             if "properties" not in i:
                 i["properties"] = {}
             i["properties"]["processing:software"] = {cls.name: cls.version}
         return items
 
-    def assign_collections(self):
+    def assign_collections(self) -> None:
         """Assigns new collection names based on"""
         for i, (coll, expr) in itertools.product(
             self._payload["features"],
             self.upload_options.get("collections", dict()).items(),
         ):
             if stac_jsonpath_match(i, expr):
                 i["collection"] = coll
 
     def download_item_assets(
-        self, item: Dict, path_template: Optional[str] = "${collection}/${id}", **kwargs
-    ):
-        """Download provided asset keys for all items in payload. Assets are saved in workdir in a
-           directory named by the Item ID, and the items are updated with the new asset hrefs.
+        self,
+        item: Item,
+        path_template: str = "${collection}/${id}",
+        **kwargs: Any,
+    ) -> Item:
+        """Download provided asset keys for all items in payload. Assets are
+        saved in workdir in a directory named by the Item ID, and the items are
+        updated with the new asset hrefs.
 
         Args:
-            assets (Optional[List[str]], optional): List of asset keys to download. Defaults to all assets.
+            assets (Optional[List[str]], optional): List of asset keys to
+                download. Defaults to all assets.
         """
         outdir = str(self._workdir / path_template)
         loop = asyncio.get_event_loop()
         item = loop.run_until_complete(
             download_item_assets(item, path_template=outdir, **kwargs)
         )
         return item
 
     def download_items_assets(
         self,
-        items: List[Dict],
-        path_template: Optional[str] = "${collection}/${id}",
-        **kwargs
-    ):
+        items: List[Item],
+        path_template: str = "${collection}/${id}",
+        **kwargs: Any,
+    ) -> List[Item]:
         outdir = str(self._workdir / path_template)
         loop = asyncio.get_event_loop()
         items = loop.run_until_complete(
-            download_items_assets(self.items, path_template=outdir, **kwargs)
+            download_items_assets(items, path_template=outdir, **kwargs)
         )
         return items
 
-    def upload_item_assets_to_s3(self, item: Dict, assets: Optional[List[str]] = None):
+    def upload_item_assets_to_s3(
+        self, item: Item, assets: Optional[List[str]] = None
+    ) -> Item:
         if self._skip_upload:
             self.logger.warning("Skipping upload of new and modified assets")
             return item
         item = upload_item_assets_to_s3(item, assets=assets, **self.upload_options)
         return item
 
     # this should be in PySTAC
     @staticmethod
-    def create_item_from_item(item):
+    def create_item_from_item(item: Dict[str, Any]) -> Dict[str, Any]:
         new_item = deepcopy(item)
         # create a derived output item
-        links = [link["href"] for link in item["links"] if link["rel"] == "self"]
+        links = [
+            link["href"] for link in item.get("links", []) if link["rel"] == "self"
+        ]
         if len(links) == 1:
             # add derived from link
             new_item["links"].append(
                 {
                     "title": "Source STAC Item",
                     "rel": "derived_from",
                     "href": links[0],
                     "type": "application/json",
                 }
             )
         return new_item
 
     @abstractmethod
-    def process(self, **kwargs) -> List[Dict]:
+    def process(self, **kwargs: Any) -> List[Dict[str, Any]]:
         """Main task logic - virtual
 
         Returns:
             [type]: [description]
         """
         # download assets of interest, this will update self.items
         # self.download_assets(['key1', 'key2'])
         # do some stuff
         # self.upload_assets(['key1', 'key2'])
         pass
 
     @classmethod
-    def handler(cls, payload: Dict, **kwargs) -> "Task":
+    def handler(cls, payload: Dict[str, Any], **kwargs: Any) -> Dict[str, Any]:
         if "href" in payload or "url" in payload:
             # read input
             with fsspec.open(payload.get("href", payload.get("url"))) as f:
                 payload = json.loads(f.read())
 
         task = cls(payload, **kwargs)
         try:
@@ -245,15 +256,15 @@
 
             return task._payload
         except Exception as err:
             task.logger.error(err, exc_info=True)
             raise err
 
     @classmethod
-    def parse_args(cls, args):
+    def parse_args(cls, args: List[str]) -> Dict[str, Any]:
         dhf = argparse.ArgumentDefaultsHelpFormatter
         parser0 = argparse.ArgumentParser(description=cls.description)
         parser0.add_argument(
             "--version",
             help="Print version and exit",
             action="version",
             version=cls.version,
@@ -293,16 +304,16 @@
         parser.add_argument(
             "--skip-validation",
             dest="skip_validation",
             action="store_true",
             default=False,
         )
         h = """ Run local mode
-                (save-workdir = True, skip-upload = True, skip-validation = True,
-                workdir = 'local-output', output = 'local-output/output-payload.json') """
+(save-workdir = True, skip-upload = True, skip-validation = True,
+workdir = 'local-output', output = 'local-output/output-payload.json') """
         parser.add_argument("--local", help=h, action="store_true", default=False)
 
         # turn Namespace into dictionary
         pargs = vars(parser0.parse_args(args))
         # only keep keys that are not None
         pargs = {k: v for k, v in pargs.items() if v is not None}
 
@@ -318,15 +329,15 @@
         if pargs.get("command", None) is None:
             parser.print_help()
             sys.exit(0)
 
         return pargs
 
     @classmethod
-    def cli(cls):
+    def cli(cls) -> None:
         args = cls.parse_args(sys.argv[1:])
         cmd = args.pop("command")
 
         # logging
         loglevel = args.pop("logging")
         logging.basicConfig(level=loglevel)
 
@@ -360,23 +371,25 @@
 
 # from https://pythonalgos.com/runtimeerror-event-loop-is-closed-asyncio-fix/
 """fix yelling at me error"""
 from asyncio.proactor_events import _ProactorBasePipeTransport  # noqa
 from functools import wraps  # noqa
 
 
-def silence_event_loop_closed(func):
+def silence_event_loop_closed(func: Callable[[Any], Any]) -> Callable[[Any], Any]:
     @wraps(func)
-    def wrapper(self, *args, **kwargs):
+    def wrapper(self, *args: Any, **kwargs: Any) -> Any:  # type: ignore
         try:
             return func(self, *args, **kwargs)
         except RuntimeError as e:
             if str(e) != "Event loop is closed":
                 raise
 
     return wrapper
 
 
-_ProactorBasePipeTransport.__del__ = silence_event_loop_closed(
-    _ProactorBasePipeTransport.__del__
+setattr(
+    _ProactorBasePipeTransport,
+    "__del__",
+    silence_event_loop_closed(_ProactorBasePipeTransport.__del__),
 )
 """fix yelling at me error end"""
```

### Comparing `stactask-0.1.0b5/stactask/utils.py` & `stactask-0.1.1/stactask/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Dict
+from typing import Any, Dict
 
 from jsonpath_ng.ext import parser
 
 
-def stac_jsonpath_match(item: Dict, expr: str) -> bool:
+def stac_jsonpath_match(item: Dict[str, Any], expr: str) -> bool:
     """Match jsonpath expression against STAC JSON.
        Use https://jsonpath.herokuapp.com/ to experiment with JSONpath
         and https://regex101.com/ to experiment with regex
 
     Args:
         item (Dict): A STAC Item
         expr (str): A valid JSONPath expression
```

### Comparing `stactask-0.1.0b5/stactask.egg-info/PKG-INFO` & `stactask-0.1.1/stactask.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactask
-Version: 0.1.0b5
+Version: 0.1.1
 Summary: STAC Task class provides a class interface for running custom algorithms on STAC Items
 Home-page: https://github.com/stac-utils/stac-task
 Author: Matthew Hanson
 Author-email: matt.a.hanson@gmail.com
 License: Apache Software License 2.0
 Project-URL: Tracker, https://github.com/stac-utils/stactask/issues
 Keywords: pystac,imagery,raster,catalog,STAC
@@ -165,23 +165,26 @@
     "description": "My process configuration",
     "collections": {
         "landsat-c2l2": "$[?(@.id =~ 'LC08.*')]"
     },
     "upload_options": {
         "path_template": "s3://my-bucket/${collection}/${year}/${month}/${day}/${id}"
     },
-    "tasks": {
-        "task-name": {
-            "param": "value"
+    "tasks": [
+        {
+            "name": "task-name"
+            "parameters": {
+                "param": "value"
+            }
         }
-    }
+    ]
 }
 ```
 
 
 ## Development
 
 ### run tests
 
 ```
-$ pytest -v -s tests
+$ ./scripts/test
 ```
```

