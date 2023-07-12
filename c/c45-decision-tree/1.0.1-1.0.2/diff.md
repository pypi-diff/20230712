# Comparing `tmp/c45-decision-tree-1.0.1.tar.gz` & `tmp/c45-decision-tree-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c45-decision-tree-1.0.1.tar", last modified: Wed Jul 12 15:46:35 2023, max compression
+gzip compressed data, was "c45-decision-tree-1.0.2.tar", last modified: Wed Jul 12 16:15:40 2023, max compression
```

## Comparing `c45-decision-tree-1.0.1.tar` & `c45-decision-tree-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/C45/
--rw-rw-rw-   0        0        0    13676 2023-07-12 15:30:23.000000 c45-decision-tree-1.0.1/C45/__init__.py
--rw-rw-rw-   0        0        0     3836 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3404 2023-07-12 15:41:03.000000 c45-decision-tree-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/
--rw-rw-rw-   0        0        0     3836 2023-07-12 15:46:35.000000 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-07-12 15:46:35.000000 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:46:35.000000 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-12 15:46:35.000000 c45-decision-tree-1.0.1/c45_decision_tree.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:46:35.356445 c45-decision-tree-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-07-12 15:39:27.000000 c45-decision-tree-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:15:40.066520 c45-decision-tree-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-12 16:15:40.066520 c45-decision-tree-1.0.2/C45/
+-rw-rw-rw-   0        0        0    13681 2023-07-12 16:11:54.000000 c45-decision-tree-1.0.2/C45/__init__.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 16:15:40.066520 c45-decision-tree-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3455 2023-07-12 16:13:39.000000 c45-decision-tree-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 16:15:40.066520 c45-decision-tree-1.0.2/c45_decision_tree.egg-info/
+-rw-rw-rw-   0        0        0     3887 2023-07-12 16:15:40.000000 c45-decision-tree-1.0.2/c45_decision_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-07-12 16:15:40.000000 c45-decision-tree-1.0.2/c45_decision_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:15:40.000000 c45-decision-tree-1.0.2/c45_decision_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-12 16:15:40.000000 c45-decision-tree-1.0.2/c45_decision_tree.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:15:40.066520 c45-decision-tree-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-07-12 16:15:39.000000 c45-decision-tree-1.0.2/setup.py
```

### Comparing `c45-decision-tree-1.0.1/C45/__init__.py` & `c45-decision-tree-1.0.2/C45/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
     def generate_tree_diagram(self, graphviz,filename):
         # Menghasilkan diagram pohon keputusan menggunakan modul graphviz
         dot = graphviz.Digraph()
 
         def build_tree(node, parent_node=None, edge_label=None):
             if isinstance(node, _DecisionNode):
-                current_node_label = node.attribute
+                current_node_label = str(node.attribute)
                 dot.node(str(id(node)), label=current_node_label)
 
                 if parent_node:
                     dot.edge(str(id(parent_node)), str(id(node)), label=edge_label)
 
                 for value, child_node in node.children.items():
                     build_tree(child_node, node, value)
```

### Comparing `c45-decision-tree-1.0.1/PKG-INFO` & `c45-decision-tree-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c45-decision-tree
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for C4.5 Decision Tree Algorithm
 Home-page: https://github.com/novandikp/DecisionTreeC45
 Author: Novandi Kevin Pratama
 Author-email: kevinpret27@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,14 +87,16 @@
 
 ### Draw Tree
 For draw tree use library graphviz and must be installed in your computer. For example:
 ```python
 import graphviz
 model.generate_tree_diagram(graphviz,"File Name")
 ```
+Example output:
+![Example Tree](images/tree.png)
 
 ### Write Rules
 For write rules, you can call `write_rules` method. For example:
 ```python
 model.write_rules()
 ```
```

### Comparing `c45-decision-tree-1.0.1/README.md` & `c45-decision-tree-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 
 ### Draw Tree
 For draw tree use library graphviz and must be installed in your computer. For example:
 ```python
 import graphviz
 model.generate_tree_diagram(graphviz,"File Name")
 ```
+Example output:
+![Example Tree](images/tree.png)
 
 ### Write Rules
 For write rules, you can call `write_rules` method. For example:
 ```python
 model.write_rules()
 ```
```

### Comparing `c45-decision-tree-1.0.1/c45_decision_tree.egg-info/PKG-INFO` & `c45-decision-tree-1.0.2/c45_decision_tree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c45-decision-tree
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for C4.5 Decision Tree Algorithm
 Home-page: https://github.com/novandikp/DecisionTreeC45
 Author: Novandi Kevin Pratama
 Author-email: kevinpret27@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,14 +87,16 @@
 
 ### Draw Tree
 For draw tree use library graphviz and must be installed in your computer. For example:
 ```python
 import graphviz
 model.generate_tree_diagram(graphviz,"File Name")
 ```
+Example output:
+![Example Tree](images/tree.png)
 
 ### Write Rules
 For write rules, you can call `write_rules` method. For example:
 ```python
 model.write_rules()
 ```
```

### Comparing `c45-decision-tree-1.0.1/setup.py` & `c45-decision-tree-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="c45-decision-tree",
-    version="1.0.1",
+    version="1.0.2",
     author="Novandi Kevin Pratama",
     author_email="kevinpret27@gmail.com",
     description="Library for C4.5 Decision Tree Algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novandikp/DecisionTreeC45",
     packages=setuptools.find_packages(),
```

