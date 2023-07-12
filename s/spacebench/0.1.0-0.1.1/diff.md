# Comparing `tmp/spacebench-0.1.0.tar.gz` & `tmp/spacebench-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacebench-0.1.0.tar", last modified: Wed Jul 12 21:01:05 2023, max compression
+gzip compressed data, was "spacebench-0.1.1.tar", last modified: Wed Jul 12 21:09:14 2023, max compression
```

## Comparing `spacebench-0.1.0.tar` & `spacebench-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:01:05.452978 spacebench-0.1.0/
--rw-r--r--   0 nak443     (502) staff       (20)     1071 2023-04-05 23:54:49.000000 spacebench-0.1.0/LICENSE
--rw-r--r--   0 nak443     (502) staff       (20)       25 2023-07-12 20:52:35.000000 spacebench-0.1.0/MANIFEST.in
--rw-r--r--   0 nak443     (502) staff       (20)     7124 2023-07-12 21:01:05.452448 spacebench-0.1.0/PKG-INFO
--rw-r--r--   0 nak443     (502) staff       (20)     5496 2023-06-21 02:44:38.000000 spacebench-0.1.0/README.md
--rw-r--r--   0 nak443     (502) staff       (20)      167 2023-06-20 21:37:54.000000 spacebench-0.1.0/requirements.txt
--rw-r--r--   0 nak443     (502) staff       (20)       38 2023-07-12 21:01:05.453206 spacebench-0.1.0/setup.cfg
--rw-r--r--   0 nak443     (502) staff       (20)     2457 2023-07-12 21:00:56.000000 spacebench-0.1.0/setup.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:01:05.440300 spacebench-0.1.0/spacebench/
--rw-r--r--   0 nak443     (502) staff       (20)      717 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/__init__.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:01:05.448615 spacebench-0.1.0/spacebench/algorithms/
--rw-r--r--   0 nak443     (502) staff       (20)        0 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/algorithms/__init__.py
--rw-r--r--   0 nak443     (502) staff       (20)      459 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/algorithms/classes.py
--rw-r--r--   0 nak443     (502) staff       (20)    11918 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/algorithms/dapsm.py
--rw-r--r--   0 nak443     (502) staff       (20)     7789 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/algorithms/gcn.py
--rw-r--r--   0 nak443     (502) staff       (20)     3705 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/algorithms/ols.py
--rw-r--r--   0 nak443     (502) staff       (20)     1547 2023-06-21 02:44:38.000000 spacebench-0.1.0/spacebench/algorithms/spatial.py
--rw-r--r--   0 nak443     (502) staff       (20)     3941 2023-06-21 02:44:38.000000 spacebench-0.1.0/spacebench/algorithms/spatialplus.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:01:05.451385 spacebench-0.1.0/spacebench/api/
--rw-r--r--   0 nak443     (502) staff       (20)        0 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/api/__init__.py
--rw-r--r--   0 nak443     (502) staff       (20)     5798 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/api/cli.py
--rw-r--r--   0 nak443     (502) staff       (20)     5535 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/api/dataverse.py
--rw-r--r--   0 nak443     (502) staff       (20)     3824 2023-06-21 02:44:38.000000 spacebench-0.1.0/spacebench/datamaster.py
--rw-r--r--   0 nak443     (502) staff       (20)    14565 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/env.py
--rw-r--r--   0 nak443     (502) staff       (20)     3659 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/eval.py
--rw-r--r--   0 nak443     (502) staff       (20)      620 2023-06-20 21:37:54.000000 spacebench-0.1.0/spacebench/log.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:01:05.443489 spacebench-0.1.0/spacebench.egg-info/
--rw-r--r--   0 nak443     (502) staff       (20)     7124 2023-07-12 21:01:04.000000 spacebench-0.1.0/spacebench.egg-info/PKG-INFO
--rw-r--r--   0 nak443     (502) staff       (20)      630 2023-07-12 21:01:05.000000 spacebench-0.1.0/spacebench.egg-info/SOURCES.txt
--rw-r--r--   0 nak443     (502) staff       (20)        1 2023-07-12 21:01:04.000000 spacebench-0.1.0/spacebench.egg-info/dependency_links.txt
--rw-r--r--   0 nak443     (502) staff       (20)      378 2023-07-12 21:01:05.000000 spacebench-0.1.0/spacebench.egg-info/requires.txt
--rw-r--r--   0 nak443     (502) staff       (20)       11 2023-07-12 21:01:05.000000 spacebench-0.1.0/spacebench.egg-info/top_level.txt
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:09:14.628807 spacebench-0.1.1/
+-rw-r--r--   0 nak443     (502) staff       (20)     1071 2023-04-05 23:54:49.000000 spacebench-0.1.1/LICENSE
+-rw-r--r--   0 nak443     (502) staff       (20)       59 2023-07-12 21:08:15.000000 spacebench-0.1.1/MANIFEST.in
+-rw-r--r--   0 nak443     (502) staff       (20)     7095 2023-07-12 21:09:14.628337 spacebench-0.1.1/PKG-INFO
+-rw-r--r--   0 nak443     (502) staff       (20)     5496 2023-06-21 02:44:38.000000 spacebench-0.1.1/README.md
+-rw-r--r--   0 nak443     (502) staff       (20)      204 2023-06-20 21:37:54.000000 spacebench-0.1.1/optional-requirements.txt
+-rw-r--r--   0 nak443     (502) staff       (20)      167 2023-06-20 21:37:54.000000 spacebench-0.1.1/requirements.txt
+-rw-r--r--   0 nak443     (502) staff       (20)       38 2023-07-12 21:09:14.629021 spacebench-0.1.1/setup.cfg
+-rw-r--r--   0 nak443     (502) staff       (20)     2373 2023-07-12 21:07:03.000000 spacebench-0.1.1/setup.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:09:14.618721 spacebench-0.1.1/spacebench/
+-rw-r--r--   0 nak443     (502) staff       (20)      717 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/__init__.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:09:14.625555 spacebench-0.1.1/spacebench/algorithms/
+-rw-r--r--   0 nak443     (502) staff       (20)        0 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/algorithms/__init__.py
+-rw-r--r--   0 nak443     (502) staff       (20)      459 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/algorithms/classes.py
+-rw-r--r--   0 nak443     (502) staff       (20)    11918 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/algorithms/dapsm.py
+-rw-r--r--   0 nak443     (502) staff       (20)     7789 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/algorithms/gcn.py
+-rw-r--r--   0 nak443     (502) staff       (20)     3705 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/algorithms/ols.py
+-rw-r--r--   0 nak443     (502) staff       (20)     1547 2023-06-21 02:44:38.000000 spacebench-0.1.1/spacebench/algorithms/spatial.py
+-rw-r--r--   0 nak443     (502) staff       (20)     3941 2023-06-21 02:44:38.000000 spacebench-0.1.1/spacebench/algorithms/spatialplus.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:09:14.627371 spacebench-0.1.1/spacebench/api/
+-rw-r--r--   0 nak443     (502) staff       (20)        0 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/api/__init__.py
+-rw-r--r--   0 nak443     (502) staff       (20)     5798 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/api/cli.py
+-rw-r--r--   0 nak443     (502) staff       (20)     5535 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/api/dataverse.py
+-rw-r--r--   0 nak443     (502) staff       (20)     3824 2023-06-21 02:44:38.000000 spacebench-0.1.1/spacebench/datamaster.py
+-rw-r--r--   0 nak443     (502) staff       (20)    14565 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/env.py
+-rw-r--r--   0 nak443     (502) staff       (20)     3659 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/eval.py
+-rw-r--r--   0 nak443     (502) staff       (20)      620 2023-06-20 21:37:54.000000 spacebench-0.1.1/spacebench/log.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-07-12 21:09:14.621806 spacebench-0.1.1/spacebench.egg-info/
+-rw-r--r--   0 nak443     (502) staff       (20)     7095 2023-07-12 21:09:14.000000 spacebench-0.1.1/spacebench.egg-info/PKG-INFO
+-rw-r--r--   0 nak443     (502) staff       (20)      656 2023-07-12 21:09:14.000000 spacebench-0.1.1/spacebench.egg-info/SOURCES.txt
+-rw-r--r--   0 nak443     (502) staff       (20)        1 2023-07-12 21:09:14.000000 spacebench-0.1.1/spacebench.egg-info/dependency_links.txt
+-rw-r--r--   0 nak443     (502) staff       (20)      378 2023-07-12 21:09:14.000000 spacebench-0.1.1/spacebench.egg-info/requires.txt
+-rw-r--r--   0 nak443     (502) staff       (20)       11 2023-07-12 21:09:14.000000 spacebench-0.1.1/spacebench.egg-info/top_level.txt
```

### Comparing `spacebench-0.1.0/LICENSE` & `spacebench-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/PKG-INFO` & `spacebench-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: spacebench
-Version: 0.1.0
-Summary: ('Spatial confounding poses a significant challenge in scientific studies ', 'where unobserved spatial variables influence both treatment and ', 'outcome, leading to spurious associations. ', 'SpaCE provides realistic benchmark datasets and tools for systematically ', 'evaluating causal inference methods for spatial confounding. Each dataset includes training data with spatial confounding, true ', 'counterfactuals, a spatial graph with coordinates, and realistic semi-', 'synthetic outcomes.')
+Version: 0.1.1
+Summary: Spatial confounding poses a significant challenge in scientific studies where unobserved spatial variables influence both treatment and outcome, leading to spurious associations. SpaCE provides realistic benchmark datasets and tools for systematically valuating causal inference methods for spatial confounding. Each dataset includes training data with spatial confounding, true counterfactuals, a spatial graph with coordinates, and realistic semi-synthetic outcomes.
 Home-page: https://github.com/NSAPH-Projects/space
 Author: Mauricio Tec, Ana Trisovic, Audirac, Michelle, Jie Hu,Sophie Mirabai Woodward, Naeem Khoshnevis, Francesca Dominici
 Author-email: mauriciogtec@hsph.harvard.edu,anatrisovic@g.harvard.edu,maudirac@hsph.harvard.edu,khu@hsph.harvard.edu,swoodward@fas.harvard.edu,nkhoshnevis@g.harvard.edu,fdominic@hsph.harvard.edu
 Maintainer: Naeem Khoshnevis
 Maintainer-email: nkhoshnevis@g.harvard.edu
 License: MIT
 Platform: UNKNOWN
```

### Comparing `spacebench-0.1.0/README.md` & `spacebench-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/setup.py` & `spacebench-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def read_requirements(file):
     with open(file) as f:
         return f.read().splitlines()
 
 
 setup(
     name="spacebench",
-    version="0.1.0",
+    version="0.1.1",
     author=(
         "Mauricio Tec, Ana Trisovic, Audirac, Michelle, Jie Hu,"
         "Sophie Mirabai Woodward, Naeem Khoshnevis, Francesca Dominici"
     ),
     author_email=(
         "mauriciogtec@hsph.harvard.edu,"
         "anatrisovic@g.harvard.edu,"
@@ -25,22 +25,15 @@
         "swoodward@fas.harvard.edu,"
         "nkhoshnevis@g.harvard.edu,"
         "fdominic@hsph.harvard.edu"
     ),
     maintainer="Naeem Khoshnevis",
     maintainer_email="nkhoshnevis@g.harvard.edu",
     description=(
-        "Spatial confounding poses a significant challenge in scientific studies ",
-        "where unobserved spatial variables influence both treatment and ",
-        "outcome, leading to spurious associations. ",
-        "SpaCE provides realistic benchmark datasets and tools for systematically ",
-        "evaluating causal inference methods for spatial confounding. Each "
-        "dataset includes training data with spatial confounding, true ",
-        "counterfactuals, a spatial graph with coordinates, and realistic semi-",
-        "synthetic outcomes."
+        "Spatial confounding poses a significant challenge in scientific studies where unobserved spatial variables influence both treatment and outcome, leading to spurious associations. SpaCE provides realistic benchmark datasets and tools for systematically valuating causal inference methods for spatial confounding. Each dataset includes training data with spatial confounding, true counterfactuals, a spatial graph with coordinates, and realistic semi-synthetic outcomes."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NSAPH-Projects/space", # cli api needs update
     license="MIT",
     packages=find_packages(exclude=["tests*", "scripts*", "notebooks*", "examples*"]),
     classifiers=[
```

### Comparing `spacebench-0.1.0/spacebench/__init__.py` & `spacebench-0.1.1/spacebench/__init__.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/algorithms/dapsm.py` & `spacebench-0.1.1/spacebench/algorithms/dapsm.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/algorithms/gcn.py` & `spacebench-0.1.1/spacebench/algorithms/gcn.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/algorithms/ols.py` & `spacebench-0.1.1/spacebench/algorithms/ols.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/algorithms/spatial.py` & `spacebench-0.1.1/spacebench/algorithms/spatial.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/algorithms/spatialplus.py` & `spacebench-0.1.1/spacebench/algorithms/spatialplus.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/api/cli.py` & `spacebench-0.1.1/spacebench/api/cli.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/api/dataverse.py` & `spacebench-0.1.1/spacebench/api/dataverse.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/datamaster.py` & `spacebench-0.1.1/spacebench/datamaster.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/env.py` & `spacebench-0.1.1/spacebench/env.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/eval.py` & `spacebench-0.1.1/spacebench/eval.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench/log.py` & `spacebench-0.1.1/spacebench/log.py`

 * *Files identical despite different names*

### Comparing `spacebench-0.1.0/spacebench.egg-info/PKG-INFO` & `spacebench-0.1.1/spacebench.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: spacebench
-Version: 0.1.0
-Summary: ('Spatial confounding poses a significant challenge in scientific studies ', 'where unobserved spatial variables influence both treatment and ', 'outcome, leading to spurious associations. ', 'SpaCE provides realistic benchmark datasets and tools for systematically ', 'evaluating causal inference methods for spatial confounding. Each dataset includes training data with spatial confounding, true ', 'counterfactuals, a spatial graph with coordinates, and realistic semi-', 'synthetic outcomes.')
+Version: 0.1.1
+Summary: Spatial confounding poses a significant challenge in scientific studies where unobserved spatial variables influence both treatment and outcome, leading to spurious associations. SpaCE provides realistic benchmark datasets and tools for systematically valuating causal inference methods for spatial confounding. Each dataset includes training data with spatial confounding, true counterfactuals, a spatial graph with coordinates, and realistic semi-synthetic outcomes.
 Home-page: https://github.com/NSAPH-Projects/space
 Author: Mauricio Tec, Ana Trisovic, Audirac, Michelle, Jie Hu,Sophie Mirabai Woodward, Naeem Khoshnevis, Francesca Dominici
 Author-email: mauriciogtec@hsph.harvard.edu,anatrisovic@g.harvard.edu,maudirac@hsph.harvard.edu,khu@hsph.harvard.edu,swoodward@fas.harvard.edu,nkhoshnevis@g.harvard.edu,fdominic@hsph.harvard.edu
 Maintainer: Naeem Khoshnevis
 Maintainer-email: nkhoshnevis@g.harvard.edu
 License: MIT
 Platform: UNKNOWN
```

### Comparing `spacebench-0.1.0/spacebench.egg-info/SOURCES.txt` & `spacebench-0.1.1/spacebench.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+optional-requirements.txt
 requirements.txt
 setup.py
 spacebench/__init__.py
 spacebench/datamaster.py
 spacebench/env.py
 spacebench/eval.py
 spacebench/log.py
```

