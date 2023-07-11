# Comparing `tmp/nirtorch-0.0.1.tar.gz` & `tmp/nirtorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nirtorch-0.0.1.tar", last modified: Wed Jul  5 00:36:46 2023, max compression
+gzip compressed data, was "nirtorch-0.0.2.tar", last modified: Tue Jul 11 22:23:36 2023, max compression
```

## Comparing `nirtorch-0.0.1.tar` & `nirtorch-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-05 00:36:46.136951 nirtorch-0.0.1/
--rw-rw-r--   0 jens      (1003) jens      (1003)     1349 2023-07-05 00:36:46.136951 nirtorch-0.0.1/PKG-INFO
--rw-rw-r--   0 jens      (1003) jens      (1003)      289 2023-07-04 19:24:41.000000 nirtorch-0.0.1/README.md
-drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-05 00:36:46.136951 nirtorch-0.0.1/nirtorch/
--rw-rw-r--   0 jens      (1003) jens      (1003)      102 2023-07-05 00:28:12.000000 nirtorch-0.0.1/nirtorch/__init__.py
--rw-rw-r--   0 jens      (1003) jens      (1003)     1753 2023-07-05 00:28:24.000000 nirtorch-0.0.1/nirtorch/from_nir.py
--rw-rw-r--   0 jens      (1003) jens      (1003)    12538 2023-07-05 00:29:17.000000 nirtorch-0.0.1/nirtorch/graph.py
--rw-rw-r--   0 jens      (1003) jens      (1003)     2060 2023-07-05 00:29:37.000000 nirtorch-0.0.1/nirtorch/to_nir.py
-drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-05 00:36:46.136951 nirtorch-0.0.1/nirtorch.egg-info/
--rw-rw-r--   0 jens      (1003) jens      (1003)     1349 2023-07-05 00:36:46.000000 nirtorch-0.0.1/nirtorch.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1003) jens      (1003)      300 2023-07-05 00:36:46.000000 nirtorch-0.0.1/nirtorch.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1003) jens      (1003)        1 2023-07-05 00:36:46.000000 nirtorch-0.0.1/nirtorch.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1003) jens      (1003)       10 2023-07-05 00:36:46.000000 nirtorch-0.0.1/nirtorch.egg-info/requires.txt
--rw-rw-r--   0 jens      (1003) jens      (1003)        9 2023-07-05 00:36:46.000000 nirtorch-0.0.1/nirtorch.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1003) jens      (1003)     1264 2023-07-05 00:36:40.000000 nirtorch-0.0.1/pyproject.toml
--rw-rw-r--   0 jens      (1003) jens      (1003)       38 2023-07-05 00:36:46.136951 nirtorch-0.0.1/setup.cfg
-drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-05 00:36:46.136951 nirtorch-0.0.1/tests/
--rw-rw-r--   0 jens      (1003) jens      (1003)     7366 2023-07-05 00:31:20.000000 nirtorch-0.0.1/tests/test_graph.py
--rw-rw-r--   0 jens      (1003) jens      (1003)     2079 2023-07-05 00:28:12.000000 nirtorch-0.0.1/tests/test_nir.py
+drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-11 22:23:36.702988 nirtorch-0.0.2/
+-rw-rw-r--   0 jens      (1003) jens      (1003)     3070 2023-07-11 22:23:36.702988 nirtorch-0.0.2/PKG-INFO
+-rw-rw-r--   0 jens      (1003) jens      (1003)     2010 2023-07-11 22:20:12.000000 nirtorch-0.0.2/README.md
+drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-11 22:23:36.698988 nirtorch-0.0.2/nirtorch/
+-rw-rw-r--   0 jens      (1003) jens      (1003)       91 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/__init__.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     4182 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/from_nir.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)    12733 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/graph.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     2206 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/graph_utils.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     2885 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/to_nir.py
+drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-11 22:23:36.702988 nirtorch-0.0.2/nirtorch.egg-info/
+-rw-rw-r--   0 jens      (1003) jens      (1003)     3070 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1003) jens      (1003)      350 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1003) jens      (1003)        1 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1003) jens      (1003)       10 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1003) jens      (1003)        9 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1003) jens      (1003)     1265 2023-07-11 22:20:12.000000 nirtorch-0.0.2/pyproject.toml
+-rw-rw-r--   0 jens      (1003) jens      (1003)       38 2023-07-11 22:23:36.702988 nirtorch-0.0.2/setup.cfg
+drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-11 22:23:36.702988 nirtorch-0.0.2/tests/
+-rw-rw-r--   0 jens      (1003) jens      (1003)     1427 2023-07-11 22:20:12.000000 nirtorch-0.0.2/tests/test_from_nir.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     7367 2023-07-11 22:20:12.000000 nirtorch-0.0.2/tests/test_graph.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     3170 2023-07-11 22:20:12.000000 nirtorch-0.0.2/tests/test_to_nir.py
```

### Comparing `nirtorch-0.0.1/nirtorch/graph.py` & `nirtorch-0.0.2/nirtorch/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+from numbers import Number
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import torch
 import torch.nn as nn
 
 
 def named_modules_map(
@@ -105,15 +106,18 @@
         if elem in self:
             return self.find_node(elem)
         else:
             # Generate a name
             if elem in self.module_names:
                 name = self.module_names[elem]
             else:
-                assert isinstance(elem, torch.Tensor)
+                if isinstance(elem, Number):
+                    elem = torch.as_tensor(elem)
+                if not isinstance(elem, torch.Tensor):
+                    raise ValueError(f"Unknown element type {type(elem)}")
                 name = f"Tensor_{self.get_unique_tensor_id()}{tuple(elem.shape)}"
             # add and return the node
             new_node = self.add_elem(elem, name)
             return new_node
 
     def find_node(self, elem: Union[torch.Tensor, nn.Module]):
         for node in self.node_list:
@@ -268,15 +272,15 @@
                 # Get all of its destinations
                 if node.outgoing_nodes:
                     # If no destinations, it is a leaf node, just drop it.
                     for outgoing_node in node.outgoing_nodes:
                         # Directly add an edge from source to destination
                         for source_node in source_node_list:
                             graph.add_edge(source_node.elem, outgoing_node.elem)
-                            # NOTE: Assuming that the destination is not of the same 
+                            # NOTE: Assuming that the destination is not of the same
                             # type here
             else:
                 # This is to preserve the graph if executed on a graph that is
                 # already filtered
                 for outnode in node.outgoing_nodes:
                     if not isinstance(outnode.elem, class_type):
                         graph.add_edge(node.elem, outnode.elem)
@@ -349,15 +353,15 @@
         nn.Module.__call__ = self.original_torch_call
 
 
 def extract_torch_graph(
     model: nn.Module, sample_data: Any, model_name: Optional[str] = "model"
 ) -> Graph:
     """Extract computational graph between various modules in the model
-    NOTE: This method is not capable of any compute happening outside of module 
+    NOTE: This method is not capable of any compute happening outside of module
     definitions.
 
     Args:
         model (nn.Module): The module to be analysed
         sample_data (Any): Sample data to be used to run by the model
         model_name (Optional[str], optional): Name of the top level module.
           If specified, it will be included in the graph.
```

### Comparing `nirtorch-0.0.1/nirtorch/to_nir.py` & `nirtorch-0.0.2/nirtorch/to_nir.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from typing import Any, Optional, Callable
+
 import torch.nn as nn
-from typing import Any, Optional, Callable, List, Union
 import nir
+import numpy as np
+
 from .graph import extract_torch_graph
 
 
 def extract_nir_graph(
     model: nn.Module,
-    model_map: Callable[[nn.Module], Union[nir.NIRNode, List[nir.NIRNode]]],
+    model_map: Callable[[nn.Module], nir.NIRNode],
     sample_data: Any,
     model_name: Optional[str] = "model",
-) -> nir.NIR:
+) -> nir.NIRNode:
     """Given a `model`, generate an NIR representation using the specified `model_map`.
 
     Args:
         model (nn.Module): The model of interest
         model_map (Callable[[nn.Module], nir.NIRNode]): A method that converts a given
             module type to an NIRNode type
         sample_data (Any): Sample input data to be used for model extraction
@@ -29,32 +32,54 @@
         model_name = None
 
     # Extract a torch graph given the model
     torch_graph = extract_torch_graph(
         model, sample_data=sample_data, model_name=model_name
     ).ignore_tensors()
 
+    # Get the root node
+    root_nodes = torch_graph.get_root()
+    if len(root_nodes) != 1:
+        raise ValueError(
+            f"Currently, only one input is supported, but {len(root_nodes)} was given"
+        )
+
     # Convert the nodes and get indices
-    edges = []
-    nir_nodes = []
+    nir_edges = []
+    nir_nodes = [nir.Input(np.array(sample_data.shape))]
     indices = {}
 
     # Get all the NIR nodes
     for indx, node in enumerate(torch_graph.node_list):
-        # Convert the node type
+        # Convert the node type to NIR subgraph
         mapped_node = model_map(node.elem)
-        if isinstance(mapped_node, list):  # Node maps to multiple nodes
-            nir_nodes.extend(mapped_node)
-            # Add edges sequentially between the nodes
-            for n_idx in range(len(mapped_node[:-1])):
-                edges.append((indx + n_idx, indx + n_idx + 1))
-        elif isinstance(mapped_node, nir.NIRNode):
+
+        if isinstance(mapped_node, nir.NIRGraph):
+            current_node_index = len(nir_nodes)
+            nir_nodes.extend(mapped_node.nodes)
+            indices[node] = indx + len(mapped_node.nodes)
+            # Add edges from graph
+            for x, y in mapped_node.edges:
+                nir_edges.append((x + current_node_index, y + current_node_index))
+        else:
             nir_nodes.append(mapped_node)
+            indices[node] = indx + 1
+
+        # Add edges from input, if first element
+        # TODO: Replace with mapping to input(s)/output(s) of subgraph
+        if indx == 0:  # TODO:
+            for sub_index in range(1, len(nir_nodes)):
+                nir_edges.append((0, sub_index))
 
-        indices[node] = indx
+    outputs = []
 
     # Get all the edges
     for node in torch_graph.node_list:
         for destination in node.outgoing_nodes:
-            edges.append((indices[node], indices[destination]))
+            nir_edges.append((indices[node], indices[destination]))
+        if len(node.outgoing_nodes) == 0:
+            output_node = nir.Output()
+            outputs.append(output_node)
+            nir_nodes.append(output_node)
+            nir_edges.append((indices[node], len(nir_nodes) - 1))
 
-    return nir.NIR(nir_nodes, edges)
+    return nir.NIRGraph(nir_nodes, nir_edges)
```

### Comparing `nirtorch-0.0.1/pyproject.toml` & `nirtorch-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "nirtorch"
-version = "0.0.1"
+version = "0.0.2"
 description = "Neuromorphic Intermediate Representation"
 authors = [
   { name = "Steven Abreu", email = "s.abreu@rug.nl" },
   { name = "Felix Bauer", email = "felix.bauer@synsen.ai" },
   { name = "Jason Eshraghian", email = "jeshragh@ucsc.edu" },
   { name = "Matthias Jobst", email = "matthias.jobst2@tu-dresden.de" },
   { name = "Gregor Lenz", email = "mail@lenzgregor.com" },
@@ -24,8 +24,8 @@
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-dependencies = [ "torch", "nir" ]
+dependencies = [ "torch", "nir" ]
```

### Comparing `nirtorch-0.0.1/tests/test_graph.py` & `nirtorch-0.0.2/tests/test_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch.nn as nn
 import torch
+
 from sinabs.layers import Merge
 from norse.torch import LIFCell, SequentialState
 import pytest
 
 
 class TupleModule(torch.nn.Module):
     def forward(self, data):
```

