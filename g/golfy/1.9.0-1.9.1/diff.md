# Comparing `tmp/golfy-1.9.0.tar.gz` & `tmp/golfy-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.9.0.tar", last modified: Wed Jul 12 20:43:35 2023, max compression
+gzip compressed data, was "golfy-1.9.1.tar", last modified: Wed Jul 12 20:50:05 2023, max compression
```

## Comparing `golfy-1.9.0.tar` & `golfy-1.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:43:35.495134 golfy-1.9.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.9.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-12 20:43:35.495001 golfy-1.9.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.9.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:43:35.493101 golfy-1.9.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      693 2023-07-12 20:33:04.000000 golfy-1.9.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.9.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)    18052 2023-07-12 20:19:24.000000 golfy-1.9.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4254 2023-07-12 20:42:46.000000 golfy-1.9.0/golfy/main.py
--rw-r--r--   0 iskander   (501) staff       (20)     6810 2023-07-12 19:40:02.000000 golfy-1.9.0/golfy/merging.py
--rw-r--r--   0 iskander   (501) staff       (20)    11274 2023-07-12 20:19:16.000000 golfy-1.9.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4177 2023-07-12 19:26:25.000000 golfy-1.9.0/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.9.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.9.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.9.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:43:35.493703 golfy-1.9.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      479 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.9.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.9.0/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-12 20:43:35.495167 golfy-1.9.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:43:35.494703 golfy-1.9.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.9.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)      538 2023-07-12 20:35:22.000000 golfy-1.9.0/tests/test_find_best_solution.py
--rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-1.9.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-1.9.0/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:50:05.679633 golfy-1.9.1/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.9.1/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-12 20:50:05.679486 golfy-1.9.1/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.9.1/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:50:05.677535 golfy-1.9.1/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      693 2023-07-12 20:49:55.000000 golfy-1.9.1/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.9.1/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)    18266 2023-07-12 20:48:49.000000 golfy-1.9.1/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4254 2023-07-12 20:42:46.000000 golfy-1.9.1/golfy/main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6810 2023-07-12 19:40:02.000000 golfy-1.9.1/golfy/merging.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11274 2023-07-12 20:19:16.000000 golfy-1.9.1/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4177 2023-07-12 19:26:25.000000 golfy-1.9.1/golfy/solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.9.1/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.9.1/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.9.1/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:50:05.678127 golfy-1.9.1/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-12 20:50:05.000000 golfy-1.9.1/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      479 2023-07-12 20:50:05.000000 golfy-1.9.1/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-12 20:50:05.000000 golfy-1.9.1/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 20:50:05.000000 golfy-1.9.1/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 20:50:05.000000 golfy-1.9.1/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.9.1/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.9.1/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-12 20:50:05.679669 golfy-1.9.1/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:50:05.679081 golfy-1.9.1/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.9.1/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      538 2023-07-12 20:35:22.000000 golfy-1.9.1/tests/test_find_best_solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-1.9.1/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-1.9.1/tests/test_optimize.py
```

### Comparing `golfy-1.9.0/LICENSE` & `golfy-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/PKG-INFO` & `golfy-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.9.0
+Version: 1.9.1
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.9.0/README.md` & `golfy-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/golfy/__init__.py` & `golfy-1.9.1/golfy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 from .initialization import init
 from .optimization import optimize
 from .solution import Solution
 from .validity import is_valid, count_violations, violations_per_replicate
 from .main import find_best_solution
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 __all__ = [
     "__version__",
     "find_best_solution",
     "Solution",
     "init",
     "optimize",
```

### Comparing `golfy-1.9.0/golfy/deconvolution.py` & `golfy-1.9.1/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/golfy/initialization.py` & `golfy-1.9.1/golfy/initialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,28 +247,32 @@
     peptide_to_preferred = transitive_closure(pairs_to_dict(preferred_neighbors))
     if verbose:
         print("[_greedy_init] Invalid neighbors: %s" % (peptide_to_invalid,))
         print("[_greedy_init] Preferred neighbors: %s" % (peptide_to_preferred,))
 
     replicate_to_pool_to_peptides = {}
 
-    random_peptide_order = np.arange(num_peptides)
-    np.random.shuffle(random_peptide_order)
-    assert len(set(random_peptide_order)) == num_peptides
-    # assign all peptides with preferred neighbors first
-    peptides_with_preferred_neighbors = [
-        p for p in random_peptide_order if p in peptide_to_preferred
-    ]
-    peptides_without_preferred_neighbors = [
-        p for p in random_peptide_order if p not in peptide_to_preferred
-    ]
-    peptide_list = (
-        peptides_with_preferred_neighbors + peptides_without_preferred_neighbors
-    )
     for i in range(num_replicates):
+        # shuffling the peptide order for each replicate, in
+        # case there's some ordering effect in the accumulation
+        # of repeated peptide pairs
+        random_peptide_order = np.arange(num_peptides)
+        np.random.shuffle(random_peptide_order)
+        assert len(set(random_peptide_order)) == num_peptides
+        # assign all peptides with preferred neighbors first
+        peptides_with_preferred_neighbors = [
+            p for p in random_peptide_order if p in peptide_to_preferred
+        ]
+        peptides_without_preferred_neighbors = [
+            p for p in random_peptide_order if p not in peptide_to_preferred
+        ]
+        peptide_list = (
+            peptides_with_preferred_neighbors + peptides_without_preferred_neighbors
+        )
+
         num_pools = num_pools_per_replicate[i]
         peptides_per_pool = int(math.ceil(num_peptides / num_pools))
 
         peptide_to_pool = {}
         pool_to_peptides = defaultdict(set)
 
         def add_to_pool(peptide, pool_idx):
```

### Comparing `golfy-1.9.0/golfy/main.py` & `golfy-1.9.1/golfy/main.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/golfy/merging.py` & `golfy-1.9.1/golfy/merging.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/golfy/optimization.py` & `golfy-1.9.1/golfy/optimization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/golfy/solution.py` & `golfy-1.9.1/golfy/solution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/golfy/util.py` & `golfy-1.9.1/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/golfy/validity.py` & `golfy-1.9.1/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/golfy.egg-info/PKG-INFO` & `golfy-1.9.1/golfy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.9.0
+Version: 1.9.1
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.9.0/pyproject.toml` & `golfy-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/tests/test_deconvolution.py` & `golfy-1.9.1/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/tests/test_find_best_solution.py` & `golfy-1.9.1/tests/test_find_best_solution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.0/tests/test_init.py` & `golfy-1.9.1/tests/test_init.py`

 * *Files identical despite different names*

