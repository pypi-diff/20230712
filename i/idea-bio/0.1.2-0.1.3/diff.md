# Comparing `tmp/idea_bio-0.1.2.tar.gz` & `tmp/idea_bio-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idea_bio-0.1.2.tar", max compression
+gzip compressed data, was "idea_bio-0.1.3.tar", max compression
```

## Comparing `idea_bio-0.1.2.tar` & `idea_bio-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-11 18:04:15.818870 idea_bio-0.1.2/LICENSE
--rw-r--r--   0        0        0     2051 2023-07-11 22:19:28.950987 idea_bio-0.1.2/README.md
--rw-r--r--   0        0        0      201 2023-07-11 21:11:40.870144 idea_bio-0.1.2/idea/__init__.py
--rw-r--r--   0        0        0     1561 2023-07-11 21:11:40.876811 idea_bio-0.1.2/idea/_go.py
--rw-r--r--   0        0        0    10142 2023-07-11 21:31:09.596173 idea_bio-0.1.2/idea/_idea.py
--rw-r--r--   0        0        0      438 2023-07-11 21:11:40.873478 idea_bio-0.1.2/idea/_utils.py
--rw-r--r--   0        0        0      670 2023-07-11 22:20:58.266995 idea_bio-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 idea_bio-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-11 18:04:15.818870 idea_bio-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2069 2023-07-11 22:22:32.166276 idea_bio-0.1.3/README.md
+-rw-r--r--   0        0        0      201 2023-07-11 21:11:40.870144 idea_bio-0.1.3/idea/__init__.py
+-rw-r--r--   0        0        0     1561 2023-07-11 21:11:40.876811 idea_bio-0.1.3/idea/_go.py
+-rw-r--r--   0        0        0    10142 2023-07-11 21:31:09.596173 idea_bio-0.1.3/idea/_idea.py
+-rw-r--r--   0        0        0      438 2023-07-11 21:11:40.873478 idea_bio-0.1.3/idea/_utils.py
+-rw-r--r--   0        0        0      670 2023-07-11 22:21:58.579869 idea_bio-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2808 1970-01-01 00:00:00.000000 idea_bio-0.1.3/PKG-INFO
```

### Comparing `idea_bio-0.1.2/LICENSE` & `idea_bio-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.2/README.md` & `idea_bio-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # IDEA
 
-![logo](https://github.com/noamteyssier/idea/blob/main/assets/logo.png)
+![logo](https://github.com/noamteyssier/idea/blob/main/assets/logo.png?raw=true)
 
 **I**ntegrated **D**ifferential **E**xpression and **A**nnotation
 
 ## Introduction
 
 This is a python module to perform GO analysis using [Enrichr](https://maayanlab.cloud/Enrichr/)
 and visualize the [bipartite graph](https://en.wikipedia.org/wiki/Bipartite_graph)
@@ -79,8 +79,8 @@
 ### Visualization
 
 We can then visualize and interact with our network by opening
 the created `*.html` in our favorite browser.
 
 Here is a static image of an example network:
 
-![network.png](https://github.com/noamteyssier/idea/blob/main/assets/example_network.png)
+![network.png](https://github.com/noamteyssier/idea/blob/main/assets/example_network.png?raw=true)
```

### Comparing `idea_bio-0.1.2/idea/_go.py` & `idea_bio-0.1.3/idea/_go.py`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.2/idea/_idea.py` & `idea_bio-0.1.3/idea/_idea.py`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.2/pyproject.toml` & `idea_bio-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idea-bio"
-version = "0.1.2"
+version = "0.1.3"
 description = "Integrated Differential Expression and Annotation"
 authors = ["Noam Teyssier"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "idea" }
 ]
```

### Comparing `idea_bio-0.1.2/PKG-INFO` & `idea_bio-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idea-bio
-Version: 0.1.2
+Version: 0.1.3
 Summary: Integrated Differential Expression and Annotation
 Home-page: https://github.com/noamteyssier/idea
 License: MIT
 Keywords: bioinformatics,differential expression,annotation,networks
 Author: Noam Teyssier
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pyvis (>=0.3.2,<0.4.0)
 Project-URL: Repository, https://github.com/noamteyssier/idea
 Description-Content-Type: text/markdown
 
 # IDEA
 
-![logo](https://github.com/noamteyssier/idea/blob/main/assets/logo.png)
+![logo](https://github.com/noamteyssier/idea/blob/main/assets/logo.png?raw=true)
 
 **I**ntegrated **D**ifferential **E**xpression and **A**nnotation
 
 ## Introduction
 
 This is a python module to perform GO analysis using [Enrichr](https://maayanlab.cloud/Enrichr/)
 and visualize the [bipartite graph](https://en.wikipedia.org/wiki/Bipartite_graph)
@@ -99,9 +99,9 @@
 ### Visualization
 
 We can then visualize and interact with our network by opening
 the created `*.html` in our favorite browser.
 
 Here is a static image of an example network:
 
-![network.png](https://github.com/noamteyssier/idea/blob/main/assets/example_network.png)
+![network.png](https://github.com/noamteyssier/idea/blob/main/assets/example_network.png?raw=true)
```

