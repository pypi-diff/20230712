# Comparing `tmp/nomic-2.0.3.tar.gz` & `tmp/nomic-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomic-2.0.3.tar", last modified: Mon Jul  3 15:01:21 2023, max compression
+gzip compressed data, was "nomic-2.0.5.tar", last modified: Wed Jul 12 18:36:39 2023, max compression
```

## Comparing `nomic-2.0.3.tar` & `nomic-2.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2023-07-03 15:01:21.990885 nomic-2.0.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2023-07-03 15:01:15.000000 nomic-2.0.3/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/nomic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10917 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/atlas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4531 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2040 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/data_inference.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28176 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/data_operations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2028 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/embedders.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/nomic/pl_callbacks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/pl_callbacks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6975 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/pl_callbacks/pl_callback.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    57993 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/project.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      521 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/nomic/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10483 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/tests/test_atlas_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1502 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/nomic.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      223 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-03 15:01:21.990885 nomic-2.0.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1259 2023-07-03 15:01:15.000000 nomic-2.0.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-12 18:36:39.867521 nomic-2.0.5/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2023-07-12 18:36:39.867521 nomic-2.0.5/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2023-07-12 18:36:30.000000 nomic-2.0.5/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-12 18:36:39.863521 nomic-2.0.5/nomic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10917 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/atlas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4531 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2040 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/data_inference.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    31597 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/data_operations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2028 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/embedders.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-12 18:36:39.863521 nomic-2.0.5/nomic/pl_callbacks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/pl_callbacks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6975 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/pl_callbacks/pl_callback.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    59018 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/project.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      521 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-12 18:36:39.863521 nomic-2.0.5/nomic/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10477 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/tests/test_atlas_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1502 2023-07-12 18:36:30.000000 nomic-2.0.5/nomic/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-12 18:36:39.863521 nomic-2.0.5/nomic.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2023-07-12 18:36:39.000000 nomic-2.0.5/nomic.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2023-07-12 18:36:39.000000 nomic-2.0.5/nomic.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-12 18:36:39.000000 nomic-2.0.5/nomic.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-07-12 18:36:39.000000 nomic-2.0.5/nomic.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      223 2023-07-12 18:36:39.000000 nomic-2.0.5/nomic.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-07-12 18:36:39.000000 nomic-2.0.5/nomic.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-12 18:36:39.867521 nomic-2.0.5/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1259 2023-07-12 18:36:30.000000 nomic-2.0.5/setup.py
```

### Comparing `nomic-2.0.3/README.md` & `nomic-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nomic-2.0.3/nomic/atlas.py` & `nomic-2.0.5/nomic/atlas.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.3/nomic/cli.py` & `nomic-2.0.5/nomic/cli.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.3/nomic/data_inference.py` & `nomic-2.0.5/nomic/data_inference.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.3/nomic/data_operations.py` & `nomic-2.0.5/nomic/data_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import concurrent.futures
 import io
 import json
 import os
 from collections import defaultdict
 from datetime import datetime
 from typing import Dict, Iterable, List, Tuple
-
+from io import BytesIO
 import numpy as np
 import pandas
 import pandas as pd
 import pyarrow as pa
+from pyarrow import feather
 import requests
 from loguru import logger
 from pyarrow import compute as pc
 from pyarrow import ipc
 from tqdm import tqdm
 
 from .settings import EMBEDDING_PAGINATION_LIMIT
@@ -215,17 +216,17 @@
             topics = [topic for topic in row if pd.notna(topic)]
 
             # Iterate over the topics in each row, adding each topic to the
             # list of subtopics for the topic at the previous depth
             for i in range(1, len(topics) - 1):
                 if topics[i + 1] not in topic_hierarchy[topics[i]]:
                     topic_hierarchy[topics[i]].append(topics[i + 1])
-        self._heirarchy = dict(topic_hierarchy)
+        self._hierarchy = dict(topic_hierarchy)
 
-        return self._heirarchy
+        return self._hierarchy
 
     def group_by_topic(self, topic_depth: int = 1) -> List[Dict]:
         """
         Associates topics at a given depth in the topic hierarchy to the identifiers of their contained datapoints.
 
         Args:
             topic_depth: Topic depth to group datums by. Acceptable values
@@ -255,16 +256,17 @@
         for topic, datum_ids in topic_datum_dict.items():
             # Encountered topic with zero datums
             if len(datum_ids) == 0:
                 continue
 
             result_dict = {}
             topic_metadata = topic_df[topic_df["topic_short_description"] == topic]
-
-            subtopics = hierarchy[topic]
+            subtopics = []
+            if topic in hierarchy:
+                subtopics = hierarchy[topic]
             result_dict["subtopics"] = subtopics
             result_dict["subtopic_ids"] = topic_df[topic_df["topic_short_description"].isin(subtopics)][
                 "topic_id"
             ].tolist()
             result_dict["topic_id"] = topic_metadata["topic_id"].item()
             result_dict["topic_short_description"] = topic_metadata["topic_short_description"].item()
             result_dict["topic_long_description"] = topic_metadata["topic_description"].item()
@@ -343,18 +345,19 @@
     def __repr__(self) -> str:
         return str(self.df)
 
 class AtlasMapEmbeddings:
     """
     Atlas Embeddings State
 
-    Access latent (high-dimensional) and projected (two-dimensional) embeddings of your datapoints. High dimensional embeddings
-    are not immediately downloaded when you access the embeddings attribute.
+    Access latent (high-dimensional) and projected (two-dimensional) embeddings of your datapoints.
 
-    === "Accessing Embeddings Example"
+    ## Two-dimensional projected embeddings
+
+    === "Accessing 2D Embeddings Example"
         ``` py
         from nomic import AtlasProject
 
         project = AtlasProject(name='My Project')
         map = project.maps[0]
         print(map.embeddings)
         ```
@@ -364,21 +367,44 @@
         0      0A  -6.164423  21.517719
         1      0g  -6.606402  -5.601104
         2      0Q  -9.206946   7.448542
         ...   ...        ...        ...
         9998  JZQ   2.110881 -12.937058
         9999  JZU   7.865006  -6.876243
         ```
+
+    ## High dimensional latent embeddings
+
+
+    === "Accessing Latent Embeddings Example"
+        ``` py
+        from nomic import AtlasProject
+
+        project = AtlasProject(name='My Project')
+        map = project.maps[0]
+        embeddings = map.embeddings.latent
+        print(embeddings.shape)
+        ```
+    === "Output"
+        ```
+        [10000, 384]
+        ```
+
+
+    !!! warning "High dimensional embeddings"
+        High dimensional embeddings are not immediately downloaded when you access the embeddings attribute - you must explicitly call `map.embeddings.latent`. Once downloaded, subsequent calls will reference your downloaded local copy.
+
     """
 
     def __init__(self, projection: "AtlasProjection"):
         self.projection = projection
         self.id_field = self.projection.project.id_field
         self._tb: pa.Table = projection._fetch_tiles().select([self.id_field, 'x', 'y'])
         self.project = projection.project
+        self._latent = None
 
     @property
     def df(self):
         """
         Pandas dataframe containing information about embeddings of your datapoints.
 
         Includes only the two-dimensional embeddings
@@ -405,28 +431,80 @@
 
         Returns:
             Pandas dataframe mapping your datapoints to their two-dimensional embeddings.
         """
         return self.df
 
     @property
-    def latent(self):
-        # """
-        # #TODO
-        # 1. download embeddings and store it in a fixed location on disk (e.g. .nomic directory)
-        # 2. make sure the embeddings align with the arrow table download order.
-        # """
-        raise NotImplementedError(
-            "Accessing latent embeddings is not yet implemented. You must use map.download_embeddings() method for now."
-        )
+    def latent(self) -> np.array:
+        """
+        High dimensional embeddings.
+
+        Returns:
+            A memmapped numpy array where each row contains the latent embedding of the corresponding datapoint in the same order as `map.embeddings.projected`.
+        """
+        if self._latent is not None:
+            return self._latent
+
+        root_embedding = self.projection.tile_destination / "0/0/0-0.embeddings.feather"
+        # Not the most complete check, hence the warning below.
+        if not root_embedding.exists():
+            self._download_latent()
+        all_embeddings = []
+
+
+        for path in self.projection._tiles_in_order():
+            # double with-suffix to remove '.embeddings.feather'
+            files = path.parent.glob(path.with_suffix("").stem + "-*.embeddings.feather")
+            # Should there be more than 10, we need to sort by int values, not string values
+            sortable = sorted(files, key=lambda x: int(x.with_suffix("").stem.split("-")[-1]))
+            if len(sortable) == 0:
+                raise FileNotFoundError("Could not find any embeddings for tile {}".format(path) + 
+                " If you possibly downloaded only some of the embeddings, run '[map_name].download_latent()'.")
+            for file in sortable:
+                tb = feather.read_table(file)
+                dims = tb['_embeddings'].type.list_size
+                all_embeddings.append(pc.list_flatten(tb['_embeddings']).to_numpy().reshape(-1, dims))
+        return np.vstack(all_embeddings)
+
+    def _download_latent(self):
+        """
+        Downloads the latent embeddings one file at a time.
+        """
+        logger.warning("Downloading latent embeddings of all datapoints.")
+        limit = 10_000
+        route = self.projection.project.atlas_api_path + '/v1/project/data/get/embedding/paged'
+        last = None
+
+        with tqdm(total=self.project.total_datums//limit) as pbar:
+            while True:
+                params = {
+                    'projection_id': self.projection.id,
+                    "last_file": last,
+                    "page_size": limit
+                }
+                r = requests.post(route, headers=self.projection.project.header, json=params)
+                if r.status_code == 204:
+                    # Download complete!
+                    break
+                fin = BytesIO(r.content)
+                tb = feather.read_table(fin)
+
+                tilename = tb.schema.metadata[b'tile'].decode("utf-8")
+                dest = (self.projection.tile_destination / tilename).with_suffix(".embeddings.feather")
+                dest.parent.mkdir(parents=True, exist_ok=True)
+                feather.write_feather(tb, dest)
+                last = tilename
+                pbar.update(1)
+
 
     def vector_search(self, queries: np.array = None, ids: List[str] = None, k: int = 5) -> Dict[str, List]:
         '''
         Performs semantic vector search over data points on your map.
-        If ids is specified, receive back the most similar data ids in vector space to your input ids.
+        If ids is specified, receive back the most similar data ids in latent vector space to your input ids.
         If queries is specified, receive back the data ids with representations most similar to the query vectors.
 
         You should not specify both queries and ids.
 
         Args:
             queries: a 2d numpy array where each row corresponds to a query vector
             ids: a list of ids
@@ -486,23 +564,27 @@
         if response.status_code != 200:
             raise Exception(response.text)
 
         response = response.json()
 
         return response['neighbors'], response['distances']
 
-    def get_embedding_iterator(self) -> Iterable[Tuple[str, str]]:
+    def _get_embedding_iterator(self) -> Iterable[Tuple[str, str]]:
         '''
+        Deprecated in favor of `map.embeddings.latent`.
+
         Iterate through embeddings of your datums.
 
         Returns:
-            A iterable mapping datum ids to their embeddings.
+            An iterable mapping datum ids to their embeddings.
 
         '''
 
+        raise DeprecationWarning("Deprecated as of June 2023. Iterate `map.embeddings.latent`.")
+
         if self.project.is_locked:
             raise Exception('Project is locked! Please wait until the project is unlocked to download embeddings')
 
         offset = 0
         limit = EMBEDDING_PAGINATION_LIMIT
         while True:
             response = requests.get(
@@ -516,25 +598,28 @@
             content = response.json()
             if len(content['datum_ids']) == 0:
                 break
             offset += len(content['datum_ids'])
 
             yield content['datum_ids'], content['embeddings']
 
-    def download_embeddings(self, save_directory: str, num_workers: int = 10) -> bool:
+    def _download_embeddings(self, save_directory: str, num_workers: int = 10) -> bool:
         '''
+        Deprecated in favor of `map.embeddings.latent`.
+
         Downloads embeddings to the specified save_directory.
 
         Args:
             save_directory: The directory to save your embeddings.
         Returns:
             True on success
 
 
         '''
+        raise DeprecationWarning("Deprecated as of June 2023. Use `map.embeddings.latent`.")
         self.project._latest_project_state()
 
         total_datums = self.project.total_datums
         if self.project.is_locked:
             raise Exception('Project is locked! Please wait until the project is unlocked to download embeddings')
 
         offset = 0
```

### Comparing `nomic-2.0.3/nomic/embedders.py` & `nomic-2.0.5/nomic/embedders.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.3/nomic/pl_callbacks/pl_callback.py` & `nomic-2.0.5/nomic/pl_callbacks/pl_callback.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.3/nomic/project.py` & `nomic-2.0.5/nomic/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,21 @@
             if "_embeddings" not in data.column_names:
                 msg = "Must include embeddings in embedding project upload."
                 raise ValueError(msg)
 
         if project.id_field not in data.column_names:
             raise ValueError(f'Data must contain the ID column `{project.id_field}`')
 
+        seen = set()
+        for col in data.column_names:
+            if col.lower() in seen:
+                raise ValueError(f'Two different fields have the same lowercased name, `{col}`'
+                ': you must use unique column names.')
+            seen.add(col.lower())
+            
         if project.schema is None:
             project._schema = convert_pyarrow_schema_for_atlas(data.schema)
         # Reformat to match the schema of the project.
         # This includes shuffling the order around if necessary,
         # filling in nulls, etc.
         reformatted = {}
 
@@ -515,28 +522,47 @@
         self._download_feather(overwrite=overwrite)
         tbs = []
         root = feather.read_table(self.tile_destination / "0/0/0.feather")
         try:
             sidecars = set([v for k, v in json.loads(root.schema.metadata[b'sidecars']).items()])
         except KeyError:
             sidecars = []
-        for path in self.tile_destination.glob('**/*.feather'):
-            if len(path.stem.split(".")) > 1:
-                # Sidecars are loaded alongside
-                continue
+        for path in self._tiles_in_order():
             tb = pa.feather.read_table(path)
             for sidecar_file in sidecars:
                 carfile = pa.feather.read_table(path.parent / f"{path.stem}.{sidecar_file}.feather")
                 for col in carfile.column_names:
                     tb = tb.append_column(col, carfile[col])
             tbs.append(tb)
         self._tile_data = pa.concat_tables(tbs)
 
         return self._tile_data
 
+    def _tiles_in_order(self):
+        """
+        Returns:
+            A list of all tiles in the projection in a fixed order so that all 
+            datasets are guaranteed to be aligned.
+        """
+        def children(z, x, y):
+            # This is the definition of a quadtree.
+            return [(z + 1, x * 2, y * 2),
+                    (z + 1, x * 2 + 1, y * 2),
+                    (z + 1, x * 2, y * 2 + 1),
+                    (z + 1, x * 2 + 1, y * 2 + 1)]
+        # start with the root
+        paths = [(0, 0, 0)]
+        # Pop off the front, extend the back (breadth first traversal)
+        while len(paths) > 0:
+            z, x, y = paths.pop(0)
+            path = Path(self.tile_destination, str(z), str(x), str(y)).with_suffix(".feather")
+            if path.exists():
+                yield path
+                paths.extend(children(z,x,y))
+    
     @property
     def tile_destination(self):
         return Path("~/.nomic/cache", self.id).expanduser()
 
     def _download_feather(self, dest: Optional[Union[str, Path]] = None, overwrite: bool = True):
         '''
         Downloads the feather tree.
```

### Comparing `nomic-2.0.3/nomic/settings.py` & `nomic-2.0.5/nomic/settings.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.3/nomic/tests/test_atlas_client.py` & `nomic-2.0.5/nomic/tests/test_atlas_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,18 +322,20 @@
         is_public=True,
         reset_project_if_exists=True,
     )
 
     map = project.get_map(name='UNITTEST1')
 
     time.sleep(10)
-    with tempfile.TemporaryDirectory() as td:
-        retrieved_embeddings = map.embeddings.download_embeddings(td)
+
+    retrieved_embeddings = map.embeddings.latent
+
 
     assert project.total_datums == num_embeddings
+    assert retrieved_embeddings.shape[0] == num_embeddings
 
     project = AtlasProject(name='UNITTEST1')
     map = project.get_map(name='UNITTEST1')
 
     assert len(map.topics.df) == 20
 
     assert isinstance(map.topics.hierarchy, dict)
```

### Comparing `nomic-2.0.3/nomic/utils.py` & `nomic-2.0.5/nomic/utils.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.3/setup.py` & `nomic-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 description = 'The official Nomic python client.'
     
 setup(
     name='nomic',
-    version='2.0.3',
+    version='2.0.5',
     url='https://github.com/nomic-ai/nomic',
     description=description,
     long_description=description,
     packages=find_packages(),
     author_email="support@nomic.ai",
     author="nomic.ai",
     classifiers=[
```

