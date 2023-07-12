# Comparing `tmp/ginormal-0.0.2.tar.gz` & `tmp/ginormal-0.0.3.tar.gz`

## Comparing `ginormal-0.0.2.tar` & `ginormal-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 ginormal-0.0.2/src/ginormal/__init__.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 ginormal-0.0.2/src/ginormal/example.py
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 ginormal-0.0.2/src/ginormal/main.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ginormal-0.0.2/src/intermediate/_F0g.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ginormal-0.0.2/src/intermediate/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 ginormal-0.0.2/src/intermediate/_dg1.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ginormal-0.0.2/src/intermediate/_msh.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ginormal-0.0.2/src/intermediate/_pbd.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 ginormal-0.0.2/src/intermediate/_rtg1.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ginormal-0.0.2/LICENSE.md
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 ginormal-0.0.2/README.md
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 ginormal-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 ginormal-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 ginormal-0.0.3/src/ginormal/__init__.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 ginormal-0.0.3/src/ginormal/example.py
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 ginormal-0.0.3/src/ginormal/main.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ginormal-0.0.3/src/intermediate/_F0g.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ginormal-0.0.3/src/intermediate/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 ginormal-0.0.3/src/intermediate/_dg1.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ginormal-0.0.3/src/intermediate/_msh.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ginormal-0.0.3/src/intermediate/_pbd.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 ginormal-0.0.3/src/intermediate/_rtg1.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ginormal-0.0.3/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ginormal-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 ginormal-0.0.3/README.md
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 ginormal-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 ginormal-0.0.3/PKG-INFO
```

### Comparing `ginormal-0.0.2/src/ginormal/__init__.py` & `ginormal-0.0.3/src/ginormal/__init__.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.2/src/ginormal/example.py` & `ginormal-0.0.3/src/ginormal/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Try it! Let's plot the true pdf and the sampled histogram for many draws
-import gin
+import ginormal as gin
 import numpy as np
 from matplotlib import pyplot as plt
 
 # Set-up with suitable parameter values
 n_draws = 1000
 a1 = 2.5
 a2 = 5
```

### Comparing `ginormal-0.0.2/src/ginormal/main.py` & `ginormal-0.0.3/src/ginormal/main.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.2/src/intermediate/_F0g.py` & `ginormal-0.0.3/src/intermediate/_F0g.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.2/src/intermediate/_dg1.py` & `ginormal-0.0.3/src/intermediate/_dg1.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.2/src/intermediate/_rtg1.py` & `ginormal-0.0.3/src/intermediate/_rtg1.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.2/README.md` & `ginormal-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.2/pyproject.toml` & `ginormal-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Package metadata
 [project]
 name = "ginormal"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.8"
 description = "Generalized Inverse Normal (GIN) distribution density and generation"
 readme = "README.md"
 authors = [
   { name = "Santiago Montoya-Blandón", email = "Santiago.Montoya-Blandon@glasgow.ac.uk" },
   { name = "Cheng Ding", email = "cheng.ding.emory@gmail.com"},
   { name = "Juan Estrada", email = "jjestra@emory.edu"},
@@ -24,12 +24,12 @@
     "Programming Language :: Python :: 3.8", # "Programming Language" represents the top-level category, "Python" represents the second-level category, and "3.8" represents the third-level category.
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent",    # The software package is not dependent on any specific operating system
 ]
 keywords = ["statistics", "distribution", "generalized inverse normal", "random variable generation"]
 
 [project.urls]
-"Bug tracking" = "https://github.com/smonto2/GIN/issues"
 "Homepage" = "https://github.com/smonto2/GIN"
+"Bug tracking" = "https://github.com/smonto2/GIN/issues"
 
 [tool.hatch.build.targets]
 packages = ["src/ginormal"]
```

### Comparing `ginormal-0.0.2/PKG-INFO` & `ginormal-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ginormal
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generalized Inverse Normal (GIN) distribution density and generation
-Project-URL: Bug tracking, https://github.com/smonto2/GIN/issues
 Project-URL: Homepage, https://github.com/smonto2/GIN
+Project-URL: Bug tracking, https://github.com/smonto2/GIN/issues
 Author-email: Santiago Montoya-Blandón <Santiago.Montoya-Blandon@glasgow.ac.uk>, Cheng Ding <cheng.ding.emory@gmail.com>, Juan Estrada <jjestra@emory.edu>, Zhilang Xia <zhilang.xia@glasgow.ac.uk>
 Maintainer-email: Santiago Montoya-Blandón <Santiago.Montoya-Blandon@glasgow.ac.uk>
 License-File: LICENSE.md
 Keywords: distribution,generalized inverse normal,random variable generation,statistics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

