# Comparing `tmp/mscales-1.3.5.tar.gz` & `tmp/mscales-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscales-1.3.5.tar", last modified: Wed Jul 12 08:42:23 2023, max compression
+gzip compressed data, was "mscales-1.3.6.tar", last modified: Wed Jul 12 11:03:35 2023, max compression
```

## Comparing `mscales-1.3.5.tar` & `mscales-1.3.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.5/AUTHORS.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.5/CONTRIBUTING.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.5/LICENSE
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.5/MANIFEST.in
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-12 08:42:23.156825 mscales-1.3.5/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      953 2023-07-05 10:34:36.000000 mscales-1.3.5/README.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/docs/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/Makefile
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/make.bat
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/docs/source/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-07-05 10:34:36.000000 mscales-1.3.5/docs/source/conf.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/source/index.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/source/pcsets.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/source/quickstart.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1309 2023-07-12 08:40:35.000000 mscales-1.3.5/docs/source/release-history.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/source/scales.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/mscales/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-12 08:42:23.156825 mscales-1.3.5/mscales/_version.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/concepts.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     9308 2023-07-10 17:10:13.000000 mscales-1.3.5/mscales/pcsets.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/plots.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/scales.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/sound.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/mscales/tests/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/tests/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/tests/conftest.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/tests/test_examples.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/utils.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/mscales.egg-info/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/SOURCES.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/dependency_links.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/requires.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/top_level.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.5/pyproject.toml
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.5/requirements.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-12 08:42:23.156825 mscales-1.3.5/setup.cfg
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.3.5/setup.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.5/versioneer.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.6/AUTHORS.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.6/CONTRIBUTING.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.6/LICENSE
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.6/MANIFEST.in
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-12 11:03:35.284790 mscales-1.3.6/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      953 2023-07-05 10:34:36.000000 mscales-1.3.6/README.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/docs/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/Makefile
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/make.bat
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/docs/source/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-07-05 10:34:36.000000 mscales-1.3.6/docs/source/conf.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/source/index.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/source/pcsets.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/source/quickstart.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1422 2023-07-12 11:01:23.000000 mscales-1.3.6/docs/source/release-history.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/source/scales.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/mscales/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-12 11:03:35.284790 mscales-1.3.6/mscales/_version.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/concepts.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    10724 2023-07-12 11:00:53.000000 mscales-1.3.6/mscales/pcsets.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/plots.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/scales.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/sound.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/mscales/tests/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/tests/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/tests/conftest.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/tests/test_examples.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/utils.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/mscales.egg-info/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/SOURCES.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/dependency_links.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/requires.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/top_level.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.6/pyproject.toml
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.6/requirements.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-12 11:03:35.284790 mscales-1.3.6/setup.cfg
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.3.6/setup.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.6/versioneer.py
```

### Comparing `mscales-1.3.5/CONTRIBUTING.rst` & `mscales-1.3.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/LICENSE` & `mscales-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/PKG-INFO` & `mscales-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mscales-1.3.5/README.rst` & `mscales-1.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/docs/Makefile` & `mscales-1.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/docs/make.bat` & `mscales-1.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/docs/source/conf.py` & `mscales-1.3.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/docs/source/pcsets.rst` & `mscales-1.3.6/docs/source/pcsets.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/docs/source/quickstart.rst` & `mscales-1.3.6/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/docs/source/release-history.rst` & `mscales-1.3.6/docs/source/release-history.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Release History
 ===============
 
+v1.3.6 (2023-07-12)
+-------------------
+
+- fix normal form bugs
+- add plotting functionality for PitchClassSets
+
 v1.3.5 (2023-07-12)
 -------------------
 
 - deal with singletons and pairs
 
 v1.3.4 (2023-07-05)
 -------------------
```

### Comparing `mscales-1.3.5/mscales/concepts.py` & `mscales-1.3.6/mscales/concepts.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/mscales/pcsets.py` & `mscales-1.3.6/mscales/pcsets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from itertools import combinations
 from collections.abc import Iterable
+import matplotlib.pyplot as plt
 
 
 class PitchClass:
     """Basic pitch-class representation as integers."""
 
     def __init__(self, p, c: int = 12):
         self.c = c
@@ -69,24 +70,21 @@
 class PitchClassSet:
     """Set of pitch classes."""
 
     def __init__(self, pcset, c: int = 12):
         self.c = c
         self.d = len(pcset)
 
-        if isinstance(pcset, Iterable):
-            pcset = set(pcset)
-
         if isinstance(pcset, str):
             assert all(
                 x in [str(i) for i in range(10)] + ["T"] + ["E"] for x in list(pcset)
             ), "Some pitch classes are not valid."
             self.pcs = np.array([10 if p == "T" else 11 if p == "E" else int(p) for p in list(pcset)])
         elif isinstance(pcset, (Iterable, PitchClassSet)):
-            self.pcs = np.array(list(pcset))
+            self.pcs = np.array([int(p) for p in pcset])
         else:
             raise TypeError(f"I don't recognize the pitch-class input {type(pcset)}.")
 
     def __repr__(self):
         return f"PitchClassSet({self.pcs})"
 
     # def __str__(self):
@@ -112,47 +110,47 @@
 
     def invert(self, n: int = 0):
         return PitchClassSet((n - self.pcs) % self.c)
 
     def complement(self):
         return PitchClassSet(np.setdiff1d(np.arange(self.c), self.pcs))
 
-    def normal_form(self, all=False):
+    def normal_form(self):
         """
         Bring pitch-class set in normal form according to description at:
         https://musictheory.pugetsound.edu/mt21c/NormalForm.html
         """
 
         self = self.sort()
 
         if len(self.pcs) == 0:
             raise "PitchClassSet is empty!"
         elif len(self.pcs) == 1:
             return self
-
-        rotations = np.array([np.roll(self.pcs, i) for i in range(self.pcs.shape[0])])
-        for length in range(self.d - 1, 0, -1):
-            spans = [(r[-1] - r[0]) % self.c for r in rotations[:, : length + 1]]
-            mask = spans == min(spans)
-            min_span_rotations = rotations[mask]
-
-            # if there is a tie in the first step and we want to obtain all candidates
-            # (if there are more than one)
-            if (length == self.d - 1) and all and (min_span_rotations.shape[0] > 1):
-                return min_span_rotations
-            # if there is only one candidate left
-            elif min_span_rotations.shape[0] == 1:
-                return PitchClassSet(min_span_rotations.flatten())
-            else:
-                continue
-
-            # if there is an absolute tie, chose the one with smaller first element
-        if min_span_rotations.shape[0] > 1:
-            min_idx = np.argmin(min_span_rotations, axis=0)[0]
-            return PitchClassSet(min_span_rotations[min_idx])
+        else:
+            rotations = np.array([np.roll(self.pcs, i) for i in range(self.pcs.shape[0])])
+            for length in range(self.d - 1, 0, -1):
+                spans = [(r[-1] - r[0]) % self.c for r in rotations[:, : length + 1]]
+                mask = spans == min(spans)
+                min_span_rotations = rotations[mask]
+
+                # if there is a tie in the first step and we want to obtain all candidates
+                # if there is only one candidate left
+                if min_span_rotations.shape[0] == 1:
+                    return PitchClassSet(min_span_rotations.flatten())
+                # (if there are more than one)
+                elif min_span_rotations.shape[0] > 1:  # (length == self.d - 1) and
+                    rotations = min_span_rotations
+                else:
+                    raise "Something went wrong!"
+
+                # if there is an absolute tie, chose the one with smaller first element
+            if min_span_rotations.shape[0] > 1:
+                min_idx = np.argmin(min_span_rotations, axis=0)[0]
+                return PitchClassSet(min_span_rotations[min_idx])
 
     def prime_form(self):
         """Prime form of the pitch-class set, after Rahn.
         See also: https://ianring.com/musictheory/scales/#primeform
         """
 
         if len(self.pcs) == 0:
@@ -168,33 +166,21 @@
         candidate1 = transposed
 
         inverted = transposed.invert()
         sorted = inverted.sort()
 
         candidate2 = sorted.normal_form().transpose(-sorted.normal_form().pcs[0])
 
-        if np.less_equal(candidate1.pcs, candidate2.pcs).all():
-            return candidate1
-        elif np.less_equal(candidate2.pcs, candidate1.pcs).all():
-            return candidate2
-        else:
-            return candidate1, candidate2
-
-        # # if there had been more than one candidate for normal form
-
-        # return sorted.normal_form().transpose(-sorted.normal_form().pcs[0]), transposed
-        #     transposed_inverted = transposed_inverted.sort().normal_form()
-        # # if np.array_equal(inverted.pcs, transposed_inverted.pcs):
-        # #     return transposed
-        # if np.less_equal(transposed.pcs, transposed_inverted.pcs).all():
-        #     return transposed
-        # elif np.less_equal(transposed_inverted.pcs, transposed.pcs).all():
-        #     return transposed_inverted
-        # else:
-        #     return "Something went wrong.", (transposed_inverted.pcs, transposed.pcs)
+        try:
+            if np.less_equal(candidate1.pcs, candidate2.pcs).all():
+                return candidate1
+            elif np.less_equal(candidate2.pcs, candidate1.pcs).all():
+                return candidate2
+        except Exception as e:
+            return e
 
         # The following special cases were taken from https://ianring.com/
         # TODO: Implement special cases!
         # // Special set classes:
         # // Forte  Prime form packed    Prime form packed
         # // name   from the right       to the left
         # // ----------------------------------------------
@@ -224,14 +210,69 @@
     def inversion(self):
         """This is different from `self.invert` !!"""
         return self.invert(self.pcs[0]).transpose(self.pcs[0])
 
     def matrix(self):
         return np.asarray([self.transpose(-i).pcs for i in self.pcs])
 
+    def plot(self, kind="lollipop", save=False):
+
+        if kind == "lollipop":
+            # c = s.shape[0]
+
+            # figure and axis settings
+            _, ax = plt.subplots(subplot_kw={"projection": "polar", "clip_on": False})
+            ax.set_theta_direction(-1)
+            ax.set_theta_zero_location("N")
+            ax.set_yticklabels([])
+            ax.set_ylim(0, 1)
+            plt.thetagrids(np.linspace(0, 360, self.c, endpoint=False), np.arange(self.c))
+
+            # data
+            thetas = [k / self.c * 2 * np.pi for k in np.flatnonzero(self.to_vector())]
+            radii = np.ones(len(thetas))
+
+            stems = ax.stem(thetas, radii, linefmt="k", markerfmt="ok")
+            for st in stems:
+                st.set_clip_on(False)
+            plt.setp(stems, "linewidth", 3)
+            plt.setp(stems[0], "markersize", 10)
+        if kind == "area":
+            # c = s.shape[0]
+
+            # figure and axis settings
+            _, ax = plt.subplots(subplot_kw={"projection": "polar", "clip_on": False})
+            ax.set_theta_direction(-1)
+            ax.set_theta_zero_location("N")
+            ax.set_yticklabels([])
+            ax.set_ylim(0, 1)
+            plt.thetagrids(np.linspace(0, 360, self.c, endpoint=False), np.arange(self.c))
+
+            # data
+            thetas = [k / self.c * 2 * np.pi for k in np.flatnonzero(self.to_vector())]
+            radii = [1 for _ in range(len(thetas))]
+
+            thetas += thetas[:1]
+            radii += radii[:1]
+
+            ax.plot(thetas, radii, c="k", zorder=5)
+            ax.fill(thetas, radii, alpha=0.75, zorder=4)
+
+        elif kind == "bar":
+            _, ax = plt.subplots()
+            ax.bar(np.arange(self.c), self.to_vector(), color="k")
+            ax.set(xlabel="Pitch class", yticks=[], ylim=(0, 1))
+
+        else:
+            print("I don't recognize the plot kind." "Valid values are 'polar' and 'bar'.")
+
+        if save:
+            plt.savefig(save)
+        plt.show()
+
     def info(self):
         print("=" * len(repr(self)))
         print(repr(self))
         print("=" * len(repr(self)))
         print()
         print("Set Theory")
         print("==========")
@@ -253,24 +294,25 @@
         print("retro.-inv.\t:", self.inversion().retrograde())
         print("matrix\t\t:", str(self.matrix()).replace("\n", "\n\t\t"))
 
 
 if __name__ == "__main__":
 
     # test cases from https://musictheory.pugetsound.edu/mt21c/PrimeForm.html
-    # s = {3, 11, 2}
-    # s = {8,0,9}
+    s = {3, 11, 2}
+    s = {8, 0, 9}
     s = "123E"
     s = "17TE"
+    s = "941"
     # s = {11,2,3,7,2}
     # s = {2,3,8,9}
     # s = {0, 2, 4}
     # s = {0, 1, 4, 6}  # all-interval tetrachord
     # s = {1,5,6,7} # from Straus, p. 58
     # s = {0, 2, 4, 5, 7, 9, 11}
     # s = {0,1,2}
     # s = {6,9,2}
     # s = {7, 10, 1, 5}
     # s = [0, 1, 6, 7, 5, 2, 4, 3, 10, 9, 11, 8]  # 12-tone row
-    pcset = PitchClassSet(s)
 
+    pcset = PitchClassSet(s)
     pcset.info()
```

### Comparing `mscales-1.3.5/mscales/plots.py` & `mscales-1.3.6/mscales/plots.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/mscales/scales.py` & `mscales-1.3.6/mscales/scales.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/mscales/sound.py` & `mscales-1.3.6/mscales/sound.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/mscales/utils.py` & `mscales-1.3.6/mscales/utils.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/mscales.egg-info/PKG-INFO` & `mscales-1.3.6/mscales.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mscales-1.3.5/mscales.egg-info/SOURCES.txt` & `mscales-1.3.6/mscales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/setup.py` & `mscales-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.5/versioneer.py` & `mscales-1.3.6/versioneer.py`

 * *Files identical despite different names*

