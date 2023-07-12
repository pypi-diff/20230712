# Comparing `tmp/mscales-1.3.4.tar.gz` & `tmp/mscales-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscales-1.3.4.tar", last modified: Wed Jul  5 11:05:53 2023, max compression
+gzip compressed data, was "mscales-1.3.5.tar", last modified: Wed Jul 12 08:42:23 2023, max compression
```

## Comparing `mscales-1.3.4.tar` & `mscales-1.3.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.4/AUTHORS.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.4/CONTRIBUTING.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.4/LICENSE
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.4/MANIFEST.in
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-05 11:05:53.992607 mscales-1.3.4/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      953 2023-07-05 10:34:36.000000 mscales-1.3.4/README.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/docs/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/Makefile
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/make.bat
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/docs/source/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-07-05 10:34:36.000000 mscales-1.3.4/docs/source/conf.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/source/index.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/source/pcsets.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/source/quickstart.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1234 2023-07-05 11:03:13.000000 mscales-1.3.4/docs/source/release-history.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/source/scales.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/mscales/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-05 11:05:53.992607 mscales-1.3.4/mscales/_version.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/concepts.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     8762 2023-07-05 10:57:19.000000 mscales-1.3.4/mscales/pcsets.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/plots.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/scales.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/sound.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/mscales/tests/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/tests/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/tests/conftest.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/tests/test_examples.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/utils.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/mscales.egg-info/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/SOURCES.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/dependency_links.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/requires.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/top_level.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.4/pyproject.toml
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.4/requirements.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-05 11:05:53.992607 mscales-1.3.4/setup.cfg
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.3.4/setup.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.4/versioneer.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.5/AUTHORS.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.5/CONTRIBUTING.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.5/LICENSE
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.5/MANIFEST.in
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-12 08:42:23.156825 mscales-1.3.5/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      953 2023-07-05 10:34:36.000000 mscales-1.3.5/README.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/docs/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/Makefile
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/make.bat
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/docs/source/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-07-05 10:34:36.000000 mscales-1.3.5/docs/source/conf.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/source/index.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/source/pcsets.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/source/quickstart.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1309 2023-07-12 08:40:35.000000 mscales-1.3.5/docs/source/release-history.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.5/docs/source/scales.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/mscales/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-12 08:42:23.156825 mscales-1.3.5/mscales/_version.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/concepts.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     9308 2023-07-10 17:10:13.000000 mscales-1.3.5/mscales/pcsets.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/plots.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/scales.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/sound.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/mscales/tests/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/tests/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/tests/conftest.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/tests/test_examples.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.5/mscales/utils.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 08:42:23.156825 mscales-1.3.5/mscales.egg-info/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/SOURCES.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/dependency_links.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/requires.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-12 08:42:23.000000 mscales-1.3.5/mscales.egg-info/top_level.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.5/pyproject.toml
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.5/requirements.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-12 08:42:23.156825 mscales-1.3.5/setup.cfg
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.3.5/setup.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.5/versioneer.py
```

### Comparing `mscales-1.3.4/CONTRIBUTING.rst` & `mscales-1.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/LICENSE` & `mscales-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/PKG-INFO` & `mscales-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mscales-1.3.4/README.rst` & `mscales-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/docs/Makefile` & `mscales-1.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/docs/make.bat` & `mscales-1.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/docs/source/conf.py` & `mscales-1.3.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/docs/source/pcsets.rst` & `mscales-1.3.5/docs/source/pcsets.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/docs/source/quickstart.rst` & `mscales-1.3.5/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/docs/source/release-history.rst` & `mscales-1.3.5/docs/source/release-history.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Release History
 ===============
 
+v1.3.5 (2023-07-12)
+-------------------
+
+- deal with singletons and pairs
+
 v1.3.4 (2023-07-05)
 -------------------
 
 - minor fix
 
 v1.3.3 (2023-07-05)
 -------------------
```

### Comparing `mscales-1.3.4/mscales/concepts.py` & `mscales-1.3.5/mscales/concepts.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/mscales/pcsets.py` & `mscales-1.3.5/mscales/pcsets.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 class PitchClassSet:
     """Set of pitch classes."""
 
     def __init__(self, pcset, c: int = 12):
         self.c = c
         self.d = len(pcset)
 
+        if isinstance(pcset, Iterable):
+            pcset = set(pcset)
+
         if isinstance(pcset, str):
             assert all(
                 x in [str(i) for i in range(10)] + ["T"] + ["E"] for x in list(pcset)
             ), "Some pitch classes are not valid."
             self.pcs = np.array([10 if p == "T" else 11 if p == "E" else int(p) for p in list(pcset)])
         elif isinstance(pcset, (Iterable, PitchClassSet)):
             self.pcs = np.array(list(pcset))
@@ -117,14 +120,19 @@
         """
         Bring pitch-class set in normal form according to description at:
         https://musictheory.pugetsound.edu/mt21c/NormalForm.html
         """
 
         self = self.sort()
 
+        if len(self.pcs) == 0:
+            raise "PitchClassSet is empty!"
+        elif len(self.pcs) == 1:
+            return self
+
         rotations = np.array([np.roll(self.pcs, i) for i in range(self.pcs.shape[0])])
         for length in range(self.d - 1, 0, -1):
             spans = [(r[-1] - r[0]) % self.c for r in rotations[:, : length + 1]]
             mask = spans == min(spans)
             min_span_rotations = rotations[mask]
 
             # if there is a tie in the first step and we want to obtain all candidates
@@ -142,14 +150,23 @@
             min_idx = np.argmin(min_span_rotations, axis=0)[0]
             return PitchClassSet(min_span_rotations[min_idx])
 
     def prime_form(self):
         """Prime form of the pitch-class set, after Rahn.
         See also: https://ianring.com/musictheory/scales/#primeform
         """
+
+        if len(self.pcs) == 0:
+            return "PitchClassSet is empty!"
+        elif len(self.pcs) == 1:
+            # TODO: transoposition should know whether it operates
+            # on Pitches, PitchSets, or PitchClass sets, and take the modulo
+            # from the Class
+            return self.transpose(-self.pcs[0] % self.c)
+
         normal = self.normal_form()
         transposed = normal.transpose(-normal.pcs[0])
         candidate1 = transposed
 
         inverted = transposed.invert()
         sorted = inverted.sort()
```

### Comparing `mscales-1.3.4/mscales/plots.py` & `mscales-1.3.5/mscales/plots.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/mscales/scales.py` & `mscales-1.3.5/mscales/scales.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/mscales/sound.py` & `mscales-1.3.5/mscales/sound.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/mscales/utils.py` & `mscales-1.3.5/mscales/utils.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/mscales.egg-info/PKG-INFO` & `mscales-1.3.5/mscales.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mscales-1.3.4/mscales.egg-info/SOURCES.txt` & `mscales-1.3.5/mscales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/setup.py` & `mscales-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.4/versioneer.py` & `mscales-1.3.5/versioneer.py`

 * *Files identical despite different names*

