# Comparing `tmp/conveyant-0.0.1.tar.gz` & `tmp/conveyant-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conveyant-0.0.1.tar", last modified: Sun Jul  9 07:00:43 2023, max compression
+gzip compressed data, was "conveyant-0.0.2.tar", last modified: Wed Jul 12 21:26:02 2023, max compression
```

## Comparing `conveyant-0.0.1.tar` & `conveyant-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 rastkociric   (501) staff       (20)        0 2023-07-09 07:00:43.012598 conveyant-0.0.1/
--rw-r--r--   0 rastkociric   (501) staff       (20)    11357 2023-07-09 06:21:21.000000 conveyant-0.0.1/LICENSE
--rw-r--r--   0 rastkociric   (501) staff       (20)    13581 2023-07-09 07:00:43.012073 conveyant-0.0.1/PKG-INFO
--rw-r--r--   0 rastkociric   (501) staff       (20)       49 2023-07-09 06:21:21.000000 conveyant-0.0.1/README.md
-drwxr-xr-x   0 rastkociric   (501) staff       (20)        0 2023-07-09 07:00:43.009739 conveyant-0.0.1/conveyant/
--rw-r--r--   0 rastkociric   (501) staff       (20)      290 2023-07-09 06:54:41.000000 conveyant-0.0.1/conveyant/__init__.py
--rw-r--r--   0 rastkociric   (501) staff       (20)     1216 2023-07-09 06:45:32.000000 conveyant-0.0.1/conveyant/axisutil.py
--rw-r--r--   0 rastkociric   (501) staff       (20)    12031 2023-07-09 06:47:20.000000 conveyant-0.0.1/conveyant/flows.py
-drwxr-xr-x   0 rastkociric   (501) staff       (20)        0 2023-07-09 07:00:43.011455 conveyant-0.0.1/conveyant.egg-info/
--rw-r--r--   0 rastkociric   (501) staff       (20)    13581 2023-07-09 07:00:42.000000 conveyant-0.0.1/conveyant.egg-info/PKG-INFO
--rw-r--r--   0 rastkociric   (501) staff       (20)      227 2023-07-09 07:00:43.000000 conveyant-0.0.1/conveyant.egg-info/SOURCES.txt
--rw-r--r--   0 rastkociric   (501) staff       (20)        1 2023-07-09 07:00:42.000000 conveyant-0.0.1/conveyant.egg-info/dependency_links.txt
--rw-r--r--   0 rastkociric   (501) staff       (20)       10 2023-07-09 07:00:42.000000 conveyant-0.0.1/conveyant.egg-info/top_level.txt
--rw-r--r--   0 rastkociric   (501) staff       (20)      712 2023-07-09 07:00:32.000000 conveyant-0.0.1/pyproject.toml
--rw-r--r--   0 rastkociric   (501) staff       (20)       38 2023-07-09 07:00:43.012723 conveyant-0.0.1/setup.cfg
+drwxr-xr-x   0 rastkociric   (501) staff       (20)        0 2023-07-12 21:26:02.478738 conveyant-0.0.2/
+-rw-r--r--   0 rastkociric   (501) staff       (20)    11357 2023-07-12 04:35:47.000000 conveyant-0.0.2/LICENSE
+-rw-r--r--   0 rastkociric   (501) staff       (20)    15398 2023-07-12 21:26:02.478185 conveyant-0.0.2/PKG-INFO
+-rw-r--r--   0 rastkociric   (501) staff       (20)     1866 2023-07-12 16:55:24.000000 conveyant-0.0.2/README.md
+-rw-r--r--   0 rastkociric   (501) staff       (20)     1017 2023-07-12 21:25:47.000000 conveyant-0.0.2/pyproject.toml
+-rw-r--r--   0 rastkociric   (501) staff       (20)       38 2023-07-12 21:26:02.478839 conveyant-0.0.2/setup.cfg
+drwxr-xr-x   0 rastkociric   (501) staff       (20)        0 2023-07-12 21:26:02.470816 conveyant-0.0.2/src/
+drwxr-xr-x   0 rastkociric   (501) staff       (20)        0 2023-07-12 21:26:02.475581 conveyant-0.0.2/src/conveyant/
+-rw-r--r--   0 rastkociric   (501) staff       (20)      667 2023-07-12 06:21:03.000000 conveyant-0.0.2/src/conveyant/__init__.py
+-rw-r--r--   0 rastkociric   (501) staff       (20)     8689 2023-07-12 04:35:47.000000 conveyant-0.0.2/src/conveyant/compositors.py
+-rw-r--r--   0 rastkociric   (501) staff       (20)      215 2023-07-12 04:35:47.000000 conveyant-0.0.2/src/conveyant/config.py
+-rw-r--r--   0 rastkociric   (501) staff       (20)     7399 2023-07-12 04:35:47.000000 conveyant-0.0.2/src/conveyant/flows.py
+-rw-r--r--   0 rastkociric   (501) staff       (20)     7340 2023-07-12 04:35:47.000000 conveyant-0.0.2/src/conveyant/replicate.py
+-rw-r--r--   0 rastkociric   (501) staff       (20)     1839 2023-07-12 07:06:36.000000 conveyant-0.0.2/src/conveyant/sanitised.py
+drwxr-xr-x   0 rastkociric   (501) staff       (20)        0 2023-07-12 21:26:02.477181 conveyant-0.0.2/src/conveyant.egg-info/
+-rw-r--r--   0 rastkociric   (501) staff       (20)    15398 2023-07-12 21:26:02.000000 conveyant-0.0.2/src/conveyant.egg-info/PKG-INFO
+-rw-r--r--   0 rastkociric   (501) staff       (20)      351 2023-07-12 21:26:02.000000 conveyant-0.0.2/src/conveyant.egg-info/SOURCES.txt
+-rw-r--r--   0 rastkociric   (501) staff       (20)        1 2023-07-12 21:26:02.000000 conveyant-0.0.2/src/conveyant.egg-info/dependency_links.txt
+-rw-r--r--   0 rastkociric   (501) staff       (20)       10 2023-07-12 21:26:02.000000 conveyant-0.0.2/src/conveyant.egg-info/top_level.txt
+drwxr-xr-x   0 rastkociric   (501) staff       (20)        0 2023-07-12 21:26:02.477487 conveyant-0.0.2/tests/
+-rw-r--r--   0 rastkociric   (501) staff       (20)    15931 2023-07-12 06:46:27.000000 conveyant-0.0.2/tests/tests.py
```

### Comparing `conveyant-0.0.1/LICENSE` & `conveyant-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conveyant-0.0.1/PKG-INFO` & `conveyant-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conveyant
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple, lightweight functional flows
 Author-email: Rastko Ciric <rastko@stanford.edu>
 Maintainer-email: Rastko Ciric <rastko@stanford.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -212,8 +212,12 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # conveyant
-Simple, lightweight functional flows
+A minimal system for compositional functional programming abstractions
+
+We use this system to separate abstract or complicated core routines from specific, concrete implementations that operate with particular dataset or input / output types. For example, instead of separately handling different imaging data types and output types (e.g., screenshots and interactive HTML) in our plotting function, the preprocessors for each data type and postprocessors for each artefact type are lifted out from a plotting function that operates directly on tensor types. Different compositional chains can then transform the general and minimal core plotting routine into a pipeline that reads a desired file type and outputs each desired artefact.
+
+This system is supercharged with the addition of different "compositors", or composition operators. The default compositor is the familiar functional composition, which substitutes outputs of the first ("inner") functional primitive as the inputs of the next ("outer") primitive in the chain. Other compositors change the interpretation of functional composition. For example, an input mapper compositor replicates the inner and outer function calls across each combination of a specified set of parameter assignments. Apparently, an output mapper compositor evaluates the inner primitive and then copies the outer primitive for each output, potentially also mapping different parameter values to each instance of the outer primitive call. Finally, a delayed execution compositor underpins a join transformation that reduces a sequence of parameters to the outer function into a scalar argument. These compositors together can operationalise a DAG-like pipeline, and future compositors might be added that automatically wrap primitives into nodes of distributed HPC-compatible graphical workflow engines like pydra.
```

### Comparing `conveyant-0.0.1/conveyant.egg-info/PKG-INFO` & `conveyant-0.0.2/src/conveyant.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conveyant
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple, lightweight functional flows
 Author-email: Rastko Ciric <rastko@stanford.edu>
 Maintainer-email: Rastko Ciric <rastko@stanford.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -212,8 +212,12 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # conveyant
-Simple, lightweight functional flows
+A minimal system for compositional functional programming abstractions
+
+We use this system to separate abstract or complicated core routines from specific, concrete implementations that operate with particular dataset or input / output types. For example, instead of separately handling different imaging data types and output types (e.g., screenshots and interactive HTML) in our plotting function, the preprocessors for each data type and postprocessors for each artefact type are lifted out from a plotting function that operates directly on tensor types. Different compositional chains can then transform the general and minimal core plotting routine into a pipeline that reads a desired file type and outputs each desired artefact.
+
+This system is supercharged with the addition of different "compositors", or composition operators. The default compositor is the familiar functional composition, which substitutes outputs of the first ("inner") functional primitive as the inputs of the next ("outer") primitive in the chain. Other compositors change the interpretation of functional composition. For example, an input mapper compositor replicates the inner and outer function calls across each combination of a specified set of parameter assignments. Apparently, an output mapper compositor evaluates the inner primitive and then copies the outer primitive for each output, potentially also mapping different parameter values to each instance of the outer primitive call. Finally, a delayed execution compositor underpins a join transformation that reduces a sequence of parameters to the outer function into a scalar argument. These compositors together can operationalise a DAG-like pipeline, and future compositors might be added that automatically wrap primitives into nodes of distributed HPC-compatible graphical workflow engines like pydra.
```

