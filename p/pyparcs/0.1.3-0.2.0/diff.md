# Comparing `tmp/pyparcs-0.1.3.tar.gz` & `tmp/pyparcs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyparcs-0.1.3.tar", last modified: Fri Feb 24 17:53:02 2023, max compression
+gzip compressed data, was "pyparcs-0.2.0.tar", last modified: Wed Jul 12 20:06:59 2023, max compression
```

## Comparing `pyparcs-0.1.3.tar` & `pyparcs-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-02-24 17:53:02.604551 pyparcs-0.1.3/
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    18092 2023-01-23 12:45:22.000000 pyparcs-0.1.3/LICENSE.txt
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    25890 2023-02-24 17:53:02.600551 pyparcs-0.1.3/PKG-INFO
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     4178 2023-02-24 17:35:21.000000 pyparcs-0.1.3/README.md
-drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-02-24 17:53:02.584550 pyparcs-0.1.3/pyparcs/
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      933 2023-01-23 12:45:22.000000 pyparcs-0.1.3/pyparcs/__init__.py
-drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-02-24 17:53:02.588551 pyparcs-0.1.3/pyparcs/cdag/
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      933 2023-01-23 12:45:22.000000 pyparcs-0.1.3/pyparcs/cdag/__init__.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    29711 2023-02-24 13:10:38.000000 pyparcs-0.1.3/pyparcs/cdag/graph_objects.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     6347 2023-02-24 13:10:38.000000 pyparcs-0.1.3/pyparcs/cdag/mapping_functions.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    10294 2023-02-24 13:10:38.000000 pyparcs-0.1.3/pyparcs/cdag/output_distributions.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    12074 2023-02-24 13:10:38.000000 pyparcs-0.1.3/pyparcs/cdag/utils.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     3122 2023-01-23 12:45:22.000000 pyparcs-0.1.3/pyparcs/exceptions.py
-drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-02-24 17:53:02.588551 pyparcs-0.1.3/pyparcs/graph_builder/
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      933 2023-01-23 12:45:22.000000 pyparcs-0.1.3/pyparcs/graph_builder/__init__.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    14830 2023-02-24 13:10:38.000000 pyparcs-0.1.3/pyparcs/graph_builder/parsers.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    17591 2023-02-24 13:10:38.000000 pyparcs-0.1.3/pyparcs/graph_builder/randomizer.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     2991 2023-01-23 15:00:26.000000 pyparcs-0.1.3/pyparcs/graph_builder/utils.py
-drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-02-24 17:53:02.600551 pyparcs-0.1.3/pyparcs/helpers/
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      933 2023-01-23 12:45:22.000000 pyparcs-0.1.3/pyparcs/helpers/__init__.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     6378 2023-01-23 15:00:27.000000 pyparcs-0.1.3/pyparcs/helpers/missing_data.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     1138 2023-01-23 12:45:22.000000 pyparcs-0.1.3/pyparcs/utils.py
-drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-02-24 17:53:02.584550 pyparcs-0.1.3/pyparcs.egg-info/
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    25890 2023-02-24 17:53:02.000000 pyparcs-0.1.3/pyparcs.egg-info/PKG-INFO
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      761 2023-02-24 17:53:02.000000 pyparcs-0.1.3/pyparcs.egg-info/SOURCES.txt
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)        1 2023-02-24 17:53:02.000000 pyparcs-0.1.3/pyparcs.egg-info/dependency_links.txt
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)       35 2023-02-24 17:53:02.000000 pyparcs-0.1.3/pyparcs.egg-info/entry_points.txt
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      138 2023-02-24 17:53:02.000000 pyparcs-0.1.3/pyparcs.egg-info/requires.txt
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)        8 2023-02-24 17:53:02.000000 pyparcs-0.1.3/pyparcs.egg-info/top_level.txt
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     1221 2023-02-24 16:58:47.000000 pyparcs-0.1.3/pyproject.toml
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)       38 2023-02-24 17:53:02.604551 pyparcs-0.1.3/setup.cfg
-drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-02-24 17:53:02.600551 pyparcs-0.1.3/tests/
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     3919 2023-01-23 15:00:26.000000 pyparcs-0.1.3/tests/test_graph_objects.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     8642 2023-02-24 10:36:12.000000 pyparcs-0.1.3/tests/test_node_distributions.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    18294 2023-02-24 13:10:38.000000 pyparcs-0.1.3/tests/test_parsers.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     5499 2023-01-23 15:00:26.000000 pyparcs-0.1.3/tests/test_randomizers.py
--rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     8176 2023-02-24 13:10:38.000000 pyparcs-0.1.3/tests/test_simple_graph.py
+drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-07-12 20:06:59.372202 pyparcs-0.2.0/
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    18092 2023-01-23 12:45:22.000000 pyparcs-0.2.0/LICENSE.txt
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    25890 2023-07-12 20:06:59.372202 pyparcs-0.2.0/PKG-INFO
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     4178 2023-02-24 17:35:21.000000 pyparcs-0.2.0/README.md
+drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-07-12 20:06:59.356202 pyparcs-0.2.0/pyparcs/
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      933 2023-07-12 20:03:17.000000 pyparcs-0.2.0/pyparcs/__init__.py
+drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-07-12 20:06:59.360202 pyparcs-0.2.0/pyparcs/cdag/
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      933 2023-01-23 12:45:22.000000 pyparcs-0.2.0/pyparcs/cdag/__init__.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    29711 2023-07-12 20:03:17.000000 pyparcs-0.2.0/pyparcs/cdag/graph_objects.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     6347 2023-02-24 13:10:38.000000 pyparcs-0.2.0/pyparcs/cdag/mapping_functions.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    10294 2023-07-12 20:03:17.000000 pyparcs-0.2.0/pyparcs/cdag/output_distributions.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    12074 2023-07-12 20:03:17.000000 pyparcs-0.2.0/pyparcs/cdag/utils.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     3122 2023-07-12 20:03:17.000000 pyparcs-0.2.0/pyparcs/exceptions.py
+drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-07-12 20:06:59.360202 pyparcs-0.2.0/pyparcs/graph_builder/
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      933 2023-01-23 12:45:22.000000 pyparcs-0.2.0/pyparcs/graph_builder/__init__.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    17507 2023-07-12 20:03:25.000000 pyparcs-0.2.0/pyparcs/graph_builder/parsers.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    19892 2023-07-12 20:03:25.000000 pyparcs-0.2.0/pyparcs/graph_builder/randomizer.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     8372 2023-07-12 20:03:25.000000 pyparcs-0.2.0/pyparcs/graph_builder/temporal_parsers.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     2991 2023-01-23 15:00:26.000000 pyparcs-0.2.0/pyparcs/graph_builder/utils.py
+drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-07-12 20:06:59.360202 pyparcs-0.2.0/pyparcs/helpers/
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      933 2023-01-23 12:45:22.000000 pyparcs-0.2.0/pyparcs/helpers/__init__.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     6378 2023-01-23 15:00:27.000000 pyparcs-0.2.0/pyparcs/helpers/missing_data.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     1138 2023-01-23 12:45:22.000000 pyparcs-0.2.0/pyparcs/utils.py
+drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-07-12 20:06:59.360202 pyparcs-0.2.0/pyparcs.egg-info/
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    25890 2023-07-12 20:06:59.000000 pyparcs-0.2.0/pyparcs.egg-info/PKG-INFO
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      834 2023-07-12 20:06:59.000000 pyparcs-0.2.0/pyparcs.egg-info/SOURCES.txt
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)        1 2023-07-12 20:06:59.000000 pyparcs-0.2.0/pyparcs.egg-info/dependency_links.txt
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)       35 2023-07-12 20:06:59.000000 pyparcs-0.2.0/pyparcs.egg-info/entry_points.txt
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)      138 2023-07-12 20:06:59.000000 pyparcs-0.2.0/pyparcs.egg-info/requires.txt
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)        8 2023-07-12 20:06:59.000000 pyparcs-0.2.0/pyparcs.egg-info/top_level.txt
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     1221 2023-07-12 20:03:25.000000 pyparcs-0.2.0/pyproject.toml
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)       38 2023-07-12 20:06:59.372202 pyparcs-0.2.0/setup.cfg
+drwxr-xr-x   0 alireza   (1001) raid-warrior  (1001)        0 2023-07-12 20:06:59.372202 pyparcs-0.2.0/tests/
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     3919 2023-01-23 15:00:26.000000 pyparcs-0.2.0/tests/test_graph_objects.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     8642 2023-02-24 10:36:12.000000 pyparcs-0.2.0/tests/test_node_distributions.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)    21392 2023-07-12 20:03:25.000000 pyparcs-0.2.0/tests/test_parsers.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     6129 2023-07-12 20:03:25.000000 pyparcs-0.2.0/tests/test_randomizers.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     8176 2023-07-12 20:03:17.000000 pyparcs-0.2.0/tests/test_simple_graph.py
+-rw-r--r--   0 alireza   (1001) raid-warrior  (1001)     4365 2023-07-12 20:03:25.000000 pyparcs-0.2.0/tests/test_temporal_parsers.py
```

### Comparing `pyparcs-0.1.3/LICENSE.txt` & `pyparcs-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/PKG-INFO` & `pyparcs-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparcs
-Version: 0.1.3
+Version: 0.2.0
 Summary: A simulation package for causal methods
 Author-email: Alireza Zamanian <alireza.zamanian@iks.fraunhofer.de>, Leopold Mareis <leopold.mareis@iks.fraunhofer.de>
 Maintainer-email: Alireza Zamanian <alireza.zamanian@iks.fraunhofer.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
```

### Comparing `pyparcs-0.1.3/README.md` & `pyparcs-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/__init__.py` & `pyparcs-0.2.0/pyparcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/cdag/__init__.py` & `pyparcs-0.2.0/pyparcs/cdag/__init__.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/cdag/graph_objects.py` & `pyparcs-0.2.0/pyparcs/cdag/graph_objects.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/cdag/mapping_functions.py` & `pyparcs-0.2.0/pyparcs/cdag/mapping_functions.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/cdag/output_distributions.py` & `pyparcs-0.2.0/pyparcs/cdag/output_distributions.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/cdag/utils.py` & `pyparcs-0.2.0/pyparcs/cdag/utils.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/exceptions.py` & `pyparcs-0.2.0/pyparcs/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/graph_builder/__init__.py` & `pyparcs-0.2.0/pyparcs/graph_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/graph_builder/parsers.py` & `pyparcs-0.2.0/pyparcs/graph_builder/parsers.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 #
 #  https://www.gnu.de/documents/gpl-2.0.de.html
 #
 #  Contact: alireza.zamanian@iks.fraunhofer.de
 
 import re
+import sys
 from typing import List, Tuple
 from typeguard import typechecked
 import numpy as np
 from pyparcs.graph_builder.utils import config_parser
 from pyparcs.cdag.output_distributions import DISTRIBUTION_PARAMS
 from pyparcs.cdag.mapping_functions import EDGE_FUNCTIONS, FUNCTION_PARAMS
 from pyparcs.cdag.utils import get_interactions_length, get_interactions_dict
@@ -202,15 +203,26 @@
         # it's not constant
         pass
 
     # 4. deterministic node
     try:
         res = det_pattern.search(line)
         directory = res.group(1)
-        assert directory[-3:] == '.py'
+        parcs_assert(
+            directory[-3:] == '.py',
+            ExternalResourceError,
+            'module directory must end with the module name, i.e. with .py '
+        )
+        if '/' in directory:
+            # strip the module name which is the last element after the last '/'
+            path_to_module = '/'.join(directory.split('/')[:-1])
+            sys.path.append(path_to_module)
+            # update directory for the next step, remaining only the module name
+            directory = directory.split('/')[-1]
+        # strip .py extension
         directory = directory[:-3]
         function_name = res.group(2)
         try:
             function_file = __import__(directory)
         except ModuleNotFoundError as exc:
             raise ExternalResourceError(f'Python script {directory} containing the function does '
                                         f'not exist.') from exc
@@ -240,15 +252,22 @@
             ''') from exc
     # split into param - value
     try:
         keys_ = [p.split('=')[0] for p in params.split(',')]
         values_ = [p.split('=')[1] for p in params.split(',')]
     except IndexError:
         # all ?
-        assert params == '?'
+        parcs_assert(
+            params == '?',
+            DescriptionFileError,
+            (f'Error in parameter "({params})" for the distribution "{dist}". '
+             'The convention to parameterize a distribution is: '
+             'dist(p1=..., p2=..., ...) even for distributions with 1 parameter, '
+             'unless the parameters are all randomized via question mark: "dist(?)"')
+        )
         keys_ = DISTRIBUTION_PARAMS[dist]
         values_ = ['?'] * len(keys_)
 
     parcs_assert(
         set(keys_) == set(DISTRIBUTION_PARAMS[dist]),
         DescriptionFileError,
         f"params {set(keys_)} not valid for distribution '{dist}'"
@@ -373,77 +392,128 @@
     return {
         'function_name': func,
         'function_params': func_params,
         'do_correction': do_correction
     }
 
 
-def graph_file_parser(file_dir):
+def graph_file_parser(file_dir, infer_edges=False):
     """**Parser for graph description YAML files**
     This function reads the graph description `.yml` files and returns the list of nodes and edges.
+    It uses the :func:`~pyparcs.graph_builder.parsers.description_parser` function
     These lists are used to instantiate a :func:`~pyparcs.cdag.graph_objects.Graph` object.
 
     See Also
     --------
 
     Parameters
     ----------
     file_dir : str
         directory of the description file.
+    infer_edges: bool, default=False
+        If true, then the missing edges are inferred and added to the list
 
     Returns
     -------
 
     """
     # if file is empty
     if file_dir is None:
         return [], []
     try:
         file = config_parser(file_dir)
     except Exception as exc:
         raise DescriptionFileError("Error in parsing YAML file.") from exc
+    return graph_description_parser(file, infer_edges=infer_edges)
+
+
+def graph_description_parser(desc_dict, infer_edges=False):
+    """**Parser for graph description dictionaries**
+    This function reads a description object and returns the list of nodes and edges.
+    These lists are used to instantiate a :func:`~pyparcs.cdag.graph_objects.Graph` object.
+
+    See Also
+    --------
+
+    Parameters
+    ----------
+    desc_dict: dict
+        a dictionary of nodes and edges description
+    infer_edges: bool, default=False
+        If true, then the missing edges are inferred and added to the list
+
+    Returns
+    -------
+
+    """
+    nodes_sublist, edges_sublist = graph_dict_splitter(desc_dict)
+    if infer_edges:
+        edges_sublist = infer_missing_edges(nodes_sublist, edges_sublist)
+
     # edges
     edges = [{
         'name': e,
-        **edge_parser(file[e])
-    } for e in file if '->' in e]
+        **edge_parser(edges_sublist[e])
+    } for e in edges_sublist]
     # node list
-    node_list = [n for n in file if '->' not in n]
+    node_list = list(nodes_sublist)
 
     # PARCS asserts:
     # 0. names are standard
     name_standard = r'^[a-zA-Z](?:[a-zA-Z0-9_]*[a-zA-Z0-9])?$'
     parcs_assert(
         all(re.match(name_standard, node_name) for node_name in node_list),
         DescriptionFileError,
         "One or more node names does not follow the PARCS naming conventions. Please see the docs."
     )
     # 1. node in edges are also in node list
-    edge_names = [e['name'] for e in edges]
-    node_in_edge = {i for element in edge_names for i in element.split('->')}
+    node_in_edge = {i for element in edges_sublist.keys() for i in element.split('->')}
     parcs_assert(
         node_in_edge.issubset(set(node_list)),
         DescriptionFileError,
         "A parent/child node in the edge list does not exist in node lines."
     )
 
     parent_dict = {
         node: sorted([
-            e['name'].split('->')[0] for e in edges
-            if e['name'].split('->')[1] == node
+            e.split('->')[0] for e in edges_sublist.keys()
+            if e.split('->')[1] == node
         ])
         for node in node_list
     }
     # nodes
     nodes = [{
         'name': n,
-        **node_parser(file[n], parent_dict[n])
-    } for n in file if '->' not in n]
+        **node_parser(desc_dict[n], parent_dict[n])
+    } for n in nodes_sublist]
 
     return nodes, edges
 
 
+def infer_missing_edges(nodes_sublist, edges_sublist):
+    # extracts list of nodes that appear in the params of the nodes
+    existing_nodes = {
+        node: [parent for parent in nodes_sublist.keys()
+               if parent in nodes_sublist[node] and parent != node]
+        for node in nodes_sublist
+    }
+    # add missing edges
+    for node in nodes_sublist:
+        for parent in existing_nodes[node]:
+            if f'{parent}->{node}' not in edges_sublist.keys():
+                edges_sublist[f'{parent}->{node}'] = 'identity()'
+
+    return edges_sublist
+
+
+def graph_dict_splitter(graph_dict):
+    edges_sublist = {k: v for k, v in graph_dict.items() if '->' in k}
+    nodes_sublist = {k: v for k, v in graph_dict.items() if k not in edges_sublist}
+
+    return nodes_sublist, edges_sublist
+
+
 def guideline_parser(file_dir):
     try:
         return config_parser(file_dir)
     except Exception as exc:
         raise GuidelineError("Error in parsing YAML file.") from exc
```

### Comparing `pyparcs-0.1.3/pyparcs/graph_builder/randomizer.py` & `pyparcs-0.2.0/pyparcs/graph_builder/randomizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,40 +17,58 @@
 #  https://www.gnu.de/documents/gpl-2.0.de.html
 #
 #  Contact: alireza.zamanian@iks.fraunhofer.de
 
 import os
 import re
 import warnings
-from pathlib import Path
 from copy import deepcopy
 from itertools import product, combinations
 from typing import Union, Optional, Iterable
 from typeguard import typechecked
 import numpy as np
 import pandas as pd
 from pyparcs.cdag.mapping_functions import FUNCTION_PARAMS
 from pyparcs.graph_builder import parsers
 from pyparcs.cdag.utils import get_interactions_length, topological_sort
 from pyparcs.graph_builder.utils import config_parser, config_dumper
 from pyparcs.cdag.output_distributions import OUTPUT_DISTRIBUTIONS, DISTRIBUTION_PARAMS
-from pyparcs.exceptions import parcs_assert, DescriptionFileError
+from pyparcs.exceptions import parcs_assert, DescriptionFileError, RandomizerError
 
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 
 @typechecked
 class ParamRandomizer:
     def __init__(self,
-                 graph_dir: Optional[Union[str, Path]] = None,
-                 guideline_dir: Optional[Union[str, Path]] = None):
+                 graph_dir: Optional[Union[str, None]] = None,
+                 guideline_dir: Optional[Union[str, None]] = None,
+                 graph_dict: Optional[Union[dict, None]] = None,
+                 guideline_dict: Optional[Union[dict, None]] = None):
+        # assert only file or dir is given
+        parcs_assert(
+            graph_dir is None or graph_dict is None,
+            RandomizerError,
+            "only a description file OR dict must be given. Both have values"
+        )
+        parcs_assert(
+            guideline_dir is None or guideline_dict is None,
+            RandomizerError,
+            "only a guideline file OR dict must be given. Both have values"
+        )
         # read randomization guideline
-        self.guideline = parsers.guideline_parser(guideline_dir)
+        if guideline_dict is None:
+            self.guideline = parsers.guideline_parser(guideline_dir)
+        else:
+            self.guideline = guideline_dict
         # read fixed nodes and edges
-        self.nodes, self.edges = parsers.graph_file_parser(graph_dir)
+        if graph_dict is None:
+            self.nodes, self.edges = parsers.graph_file_parser(graph_dir)
+        else:
+            self.nodes, self.edges = parsers.graph_description_parser(graph_dict)
 
     @staticmethod
     def directive_picker(directive: Union[list, int, float]):
         if isinstance(directive, list):
             if directive[0] == 'choice':
                 options = directive[1:]
                 return np.random.choice(options)
@@ -156,17 +174,20 @@
         self._setup()
         return self.nodes, self.edges
 
 
 @typechecked
 class ExtendRandomizer(ParamRandomizer):
     def __init__(self,
-                 graph_dir: Optional[Union[str, Path]] = None,
-                 guideline_dir: Optional[Union[str, Path]] = None):
-        super().__init__(graph_dir=graph_dir, guideline_dir=guideline_dir)
+                 graph_dir: Optional[Union[str, None]] = None,
+                 guideline_dir: Optional[Union[str, None]] = None,
+                 graph_dict: Optional[Union[dict, None]] = None,
+                 guideline_dict: Optional[Union[dict, None]] = None):
+        super().__init__(graph_dir=graph_dir, guideline_dir=guideline_dir,
+                         graph_dict=graph_dict, guideline_dict=guideline_dict)
 
         # pick number of nodes:
         self.num_nodes = self._set_num_nodes()
         # pick names
         if 'node_name_prefix' not in self.guideline['graph']:
             self.guideline['graph']['node_name_prefix'] = 'H'
         self.node_names = self._set_node_names()
@@ -254,35 +275,69 @@
 
     def _update_param_coefs(self):
         return self
 
 
 @typechecked
 class FreeRandomizer(ExtendRandomizer):
-    def __init__(self, guideline_dir: Optional[Union[str, Path]] = None):
-        super().__init__(graph_dir=None, guideline_dir=guideline_dir)
+    def __init__(self, guideline_dir: Optional[Union[str, None]] = None,
+                 guideline_dict: Optional[Union[dict, None]] = None):
+        super().__init__(guideline_dir=guideline_dir, guideline_dict=guideline_dict)
 
 
 @typechecked
 class ConnectRandomizer(ParamRandomizer):
     def __init__(self,
-                 parent_graph_dir: Optional[Union[str, Path]] = None,
-                 child_graph_dir: Optional[Union[str, Path]] = None,
-                 guideline_dir: Optional[Union[str, Path]] = None,
+                 parent_graph_dir: Optional[Union[str, None]] = None,
+                 parent_graph_dict: Optional[Union[str, None]] = None,
+                 child_graph_dir: Optional[Union[str, None]] = None,
+                 child_graph_dict: Optional[Union[str, None]] = None,
+                 guideline_dir: Optional[Union[str, None]] = None,
+                 guideline_dict: Optional[Union[str, None]] = None,
                  adj_matrix_mask: pd.DataFrame = None,
                  delete_temp_graph_description: bool = True):
-        pgd = config_parser(parent_graph_dir)
-        cgd = config_parser(child_graph_dir)
+
+
+        # assert only file or dir is given
+        parcs_assert(
+            parent_graph_dir is None or parent_graph_dict is None,
+            RandomizerError,
+            "only a description file OR dict must be given. Parent graph has both arguments"
+        )
+        parcs_assert(
+            child_graph_dir is None or child_graph_dict is None,
+            RandomizerError,
+            "only a description file OR dict must be given. child graph has both arguments"
+        )
+        parcs_assert(
+            guideline_dir is None or guideline_dict is None,
+            RandomizerError,
+            "only a guideline file OR dict must be given. Both have values"
+        )
+
+        if parent_graph_dict is None:
+            pgd = config_parser(parent_graph_dir)
+        else:
+            pgd = parent_graph_dict
+        if child_graph_dict is None:
+            cgd = config_parser(child_graph_dir)
+        else:
+            cgd = child_graph_dict
+
         n_p = [n for n in pgd if '->' not in n]
         l_p = len(n_p)
         n_c = [n for n in cgd if '->' not in n]
         e_c = [n for n in cgd if '->' in n]
         l_c = len(n_c)
 
-        guideline = config_parser(guideline_dir)
+        # read randomization guideline
+        if guideline_dict is None:
+            guideline = parsers.guideline_parser(guideline_dir)
+        else:
+            guideline = guideline_dict
 
         # sample connection adj_matrix
         density = self.directive_picker(guideline['graph']['graph_density'])
         adj_matrix = np.random.choice([0, 1], p=[1 - density, density], size=(l_p, l_c))
         adj_matrix = np.multiply(adj_matrix, adj_matrix_mask.values)
         adj_matrix = pd.DataFrame(adj_matrix,
                                   index=adj_matrix_mask.index, columns=adj_matrix_mask.columns)
@@ -351,15 +406,15 @@
         config_dumper(gd, 'combined_gdf.yml')
         super().__init__(graph_dir='combined_gdf.yml', guideline_dir=guideline_dir)
         if delete_temp_graph_description:
             os.remove('combined_gdf.yml')
 
 
 @typechecked
-def guideline_iterator(guideline_dir: Optional[Union[str, Path]] = None,
+def guideline_iterator(guideline_dir: Optional[Union[str, None]] = None,
                        to_iterate: str = None, steps: int = None,
                        repeat: int = 1):
     @typechecked
     def _get_iterable(directive: list, steps: Optional[int]):
         # assert isinstance(directive, list),
         # 'GuidelineIterator received fixed value as the directive'
         if directive[0] == 'f-range':
```

### Comparing `pyparcs-0.1.3/pyparcs/graph_builder/utils.py` & `pyparcs-0.2.0/pyparcs/graph_builder/utils.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/helpers/__init__.py` & `pyparcs-0.2.0/pyparcs/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/helpers/missing_data.py` & `pyparcs-0.2.0/pyparcs/helpers/missing_data.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs/utils.py` & `pyparcs-0.2.0/pyparcs/utils.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/pyparcs.egg-info/PKG-INFO` & `pyparcs-0.2.0/pyparcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparcs
-Version: 0.1.3
+Version: 0.2.0
 Summary: A simulation package for causal methods
 Author-email: Alireza Zamanian <alireza.zamanian@iks.fraunhofer.de>, Leopold Mareis <leopold.mareis@iks.fraunhofer.de>
 Maintainer-email: Alireza Zamanian <alireza.zamanian@iks.fraunhofer.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
```

### Comparing `pyparcs-0.1.3/pyparcs.egg-info/SOURCES.txt` & `pyparcs-0.2.0/pyparcs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 pyparcs/cdag/graph_objects.py
 pyparcs/cdag/mapping_functions.py
 pyparcs/cdag/output_distributions.py
 pyparcs/cdag/utils.py
 pyparcs/graph_builder/__init__.py
 pyparcs/graph_builder/parsers.py
 pyparcs/graph_builder/randomizer.py
+pyparcs/graph_builder/temporal_parsers.py
 pyparcs/graph_builder/utils.py
 pyparcs/helpers/__init__.py
 pyparcs/helpers/missing_data.py
 tests/test_graph_objects.py
 tests/test_node_distributions.py
 tests/test_parsers.py
 tests/test_randomizers.py
-tests/test_simple_graph.py
+tests/test_simple_graph.py
+tests/test_temporal_parsers.py
```

### Comparing `pyparcs-0.1.3/pyproject.toml` & `pyparcs-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyparcs"
-version = "0.1.3"
+version = "0.2.0"
 description = "A simulation package for causal methods"
 authors = [
     {name = "Alireza Zamanian", email = "alireza.zamanian@iks.fraunhofer.de"},
     {name = "Leopold Mareis", email = "leopold.mareis@iks.fraunhofer.de"}
 ]
 maintainers = [
     {name = "Alireza Zamanian", email = "alireza.zamanian@iks.fraunhofer.de"}
```

### Comparing `pyparcs-0.1.3/tests/test_graph_objects.py` & `pyparcs-0.2.0/tests/test_graph_objects.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/tests/test_node_distributions.py` & `pyparcs-0.2.0/tests/test_node_distributions.py`

 * *Files identical despite different names*

### Comparing `pyparcs-0.1.3/tests/test_parsers.py` & `pyparcs-0.2.0/tests/test_parsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 #
 #  https://www.gnu.de/documents/gpl-2.0.de.html
 #
 #  Contact: alireza.zamanian@iks.fraunhofer.de
 import numpy as np
 import os
 import pytest
-from pyparcs.graph_builder.parsers import *
+from pyparcs.graph_builder.parsers import (term_parser, equation_parser, node_parser,
+                                           edge_parser, graph_file_parser, graph_description_parser)
 from pyparcs.exceptions import *
 
 
 class TestTermParser:
     """
     Term parser parses the individual terms in an equation such as 2XY, -0.5Z, etc.
     """
@@ -429,7 +430,94 @@
         # teardown
         os.remove(file_name)
 
     @staticmethod
     def test_parses_gdf_raises_error(setup_wrong_gdf):
         with pytest.raises(DescriptionFileError):
             graph_file_parser(setup_wrong_gdf)
+
+
+class TestGraphDescriptionParser:
+    """
+    Testing the parser function from a dictionary object rather than a yml file.
+    """
+    @staticmethod
+    @pytest.mark.parametrize('description,nodes,edges', [
+        ({"A": "bernoulli(p_=0.2)",
+          "B": "gaussian(mu_=2A, sigma_=1)",
+          "A->B": "identity()"},
+         # nodes
+         {'A': 'bernoulli', 'B': 'gaussian'},
+         # edges
+         {'A->B': 'identity'}),
+
+        ({"A": "bernoulli(p_=0.2)",
+          "B": "gaussian(mu_=1, sigma_=1)"},
+         # nodes
+         {'A': 'bernoulli', 'B': 'gaussian'},
+         # edges
+         {}),
+
+        ({"A": "bernoulli(p_=0.2)"},
+         # nodes
+         {'A': 'bernoulli'},
+         # edges
+         {})
+    ])
+    def test_graph_desc_file(description, nodes, edges):
+        out_nodes, out_edges = graph_description_parser(description)
+        # Nodes
+        # 1. names
+        assert len(nodes) == len(out_nodes)
+        extracted_node_names = [i['name'] for i in out_nodes]
+        assert set(extracted_node_names) == set(nodes.keys())
+        # 2. distributions
+        for node in out_nodes:
+            assert nodes[node['name']] == node['output_distribution']
+
+        # edges
+        # 1. names
+        assert len(edges) == len(out_edges)
+        extracted_edges_names = [i['name'] for i in out_edges]
+        assert set(extracted_edges_names) == set(edges.keys())
+        # 2. distributions
+        for edge in out_edges:
+            assert edges[edge['name']] == edge['function_name']
+
+    @staticmethod
+    @pytest.mark.parametrize('description,nodes,edges', [
+        ({"A": "bernoulli(p_=0.2)",
+          "B": "gaussian(mu_=2A, sigma_=1)"},
+         # nodes
+         {'A': 'bernoulli', 'B': 'gaussian'},
+         # edges
+         {'A->B': 'identity'}),
+
+        ({"A": "bernoulli(p_=0.2)",
+          "B": "bernoulli(p_=A+C)",
+          "C": "bernoulli(p_=0.9)",
+          "A->B": "identity()"},
+         # nodes
+         {'A': 'bernoulli', 'B': 'bernoulli', 'C': 'bernoulli'},
+         # edges
+         {'A->B': 'identity', 'C->B': 'identity'})
+    ])
+    def test_infer_edges_functionality(description, nodes, edges):
+        out_nodes, out_edges = graph_description_parser(description,
+                                                        infer_edges=True)
+        # Nodes
+        # 1. names
+        assert len(nodes) == len(out_nodes)
+        extracted_node_names = [i['name'] for i in out_nodes]
+        assert set(extracted_node_names) == set(nodes.keys())
+        # 2. distributions
+        for node in out_nodes:
+            assert nodes[node['name']] == node['output_distribution']
+
+        # edges
+        # 1. names
+        assert len(edges) == len(out_edges)
+        extracted_edges_names = [i['name'] for i in out_edges]
+        assert set(extracted_edges_names) == set(edges.keys())
+        # 2. distributions
+        for edge in out_edges:
+            assert edges[edge['name']] == edge['function_name']
```

### Comparing `pyparcs-0.1.3/tests/test_randomizers.py` & `pyparcs-0.2.0/tests/test_randomizers.py`

 * *Files 11% similar despite different names*

```diff
@@ -118,7 +118,23 @@
         assert edge['function_params']['gamma'] in {0, 1}
         if edge['function_name'] == 'gaussian_rbf':
             assert edge['function_params']['tau'] == 2
         elif edge['function_name'] == 'arctan':
             pass
         else:
             raise AssertionError
+
+    @staticmethod
+    def test_dict_inputs():
+        description = {'A': 'random'}
+        guideline = {'nodes': {'bernoulli': {'p_': [['f-range', 0.8, 0.9], 0, 0]}}}
+        # preliminaries
+        rndz = ParamRandomizer(graph_dict=description, guideline_dict=guideline)
+        nodes, edges = rndz.get_graph_params()
+        # assert correct number of nodes have been established
+        assert len(nodes) == 1
+        assert len(edges) == 0
+        # assert edge is parsed
+        node = nodes[0]
+
+        assert node['output_distribution'] == 'bernoulli'
+        assert 0.8 <= node['dist_params_coefs']['p_']['bias'] <= 0.9
```

### Comparing `pyparcs-0.1.3/tests/test_simple_graph.py` & `pyparcs-0.2.0/tests/test_simple_graph.py`

 * *Files identical despite different names*

