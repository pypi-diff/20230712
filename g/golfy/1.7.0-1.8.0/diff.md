# Comparing `tmp/golfy-1.7.0.tar.gz` & `tmp/golfy-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.7.0.tar", last modified: Tue Jul 11 20:48:42 2023, max compression
+gzip compressed data, was "golfy-1.8.0.tar", last modified: Tue Jul 11 21:58:46 2023, max compression
```

## Comparing `golfy-1.7.0.tar` & `golfy-1.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 20:48:42.623417 golfy-1.7.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.7.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-11 20:48:42.623285 golfy-1.7.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.7.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 20:48:42.621655 golfy-1.7.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      630 2023-07-11 20:48:33.000000 golfy-1.7.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.7.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     9217 2023-07-11 20:03:28.000000 golfy-1.7.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     9777 2023-07-11 20:47:09.000000 golfy-1.7.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4089 2023-07-11 19:30:21.000000 golfy-1.7.0/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.7.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.7.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.7.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 20:48:42.622202 golfy-1.7.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      415 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-11 20:48:42.000000 golfy-1.7.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.7.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.7.0/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-11 20:48:42.623454 golfy-1.7.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 20:48:42.622995 golfy-1.7.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.7.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     1660 2023-07-07 14:04:35.000000 golfy-1.7.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.7.0/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 21:58:46.372710 golfy-1.8.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.8.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-11 21:58:46.372598 golfy-1.8.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.8.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 21:58:46.370950 golfy-1.8.0/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      630 2023-07-11 21:49:17.000000 golfy-1.8.0/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.8.0/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     9217 2023-07-11 20:03:28.000000 golfy-1.8.0/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)    14407 2023-07-11 21:49:36.000000 golfy-1.8.0/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4089 2023-07-11 19:30:21.000000 golfy-1.8.0/golfy/solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.8.0/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.8.0/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.8.0/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 21:58:46.371546 golfy-1.8.0/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      415 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.8.0/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.8.0/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-11 21:58:46.372749 golfy-1.8.0/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 21:58:46.372321 golfy-1.8.0/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.8.0/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1660 2023-07-07 14:04:35.000000 golfy-1.8.0/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.8.0/tests/test_optimize.py
```

### Comparing `golfy-1.7.0/LICENSE` & `golfy-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.7.0/PKG-INFO` & `golfy-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.7.0
+Version: 1.8.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.7.0/README.md` & `golfy-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `golfy-1.7.0/golfy/__init__.py` & `golfy-1.8.0/golfy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     DeconvolutionResult,
 )
 from .initialization import init
 from .optimization import optimize
 from .solution import Solution
 from .validity import is_valid, count_violations, violations_per_replicate
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 __all__ = [
     "__version__",
     "Solution",
     "init",
     "optimize",
     "count_violations",
```

### Comparing `golfy-1.7.0/golfy/deconvolution.py` & `golfy-1.8.0/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.7.0/golfy/initialization.py` & `golfy-1.8.0/golfy/initialization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.7.0/golfy/optimization.py` & `golfy-1.8.0/golfy/optimization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from collections import defaultdict
 import random
 import time
 
 import numpy as np
 
 from .solution import Solution
 from .types import SwapCandidateList, ReplicateToNeighborDict
-from .validity import count_violations, violations_per_replicate
+from .validity import violations_per_replicate, is_valid
 from .util import pairs_to_dict
 
 
 def find_violating_peptides(
     s: Solution,
 ) -> tuple[SwapCandidateList, ReplicateToNeighborDict]:
     replicate_to_pool_to_peptides = s.assignments
@@ -152,14 +153,125 @@
 
                 swapped_pools.add(pool_idx_a)
                 swapped_pools.add(pool_idx_b)
                 swapped_peptides.add(peptide_a)
                 swapped_peptides.add(peptide_b)
 
 
+def merge_small_pools(s: Solution) -> int:
+    num_merged = 0
+    peptide_to_invalid = pairs_to_dict(s.invalid_neighbors)
+    peptide_to_invalid_excluding_replicate = {
+        replicate_idx: peptide_to_invalid.copy()
+        for replicate_idx in range(s.num_replicates)
+    }
+    replicate_to_peptide_to_pool_idx = {}
+
+    for replicate_idx, pool_to_peptides in s.assignments.items():
+        peptide_to_pool_idx = {}
+        replicate_to_peptide_to_pool_idx[replicate_idx] = peptide_to_pool_idx
+        for pool_idx, peptides in pool_to_peptides.items():
+            for peptide in peptides:
+                peptide_to_pool_idx[peptide] = pool_idx
+    # print("replicate_to_peptide_to_pool_idx", replicate_to_peptide_to_pool_idx)
+
+    for replicate_idx, pool_to_peptides_1 in s.assignments.items():
+        for other_replicate_idx, pool_to_peptides_2 in s.assignments.items():
+            if replicate_idx == other_replicate_idx:
+                continue
+            for peptides in pool_to_peptides.values():
+                for peptide in peptides:
+                    other_pool_idx = replicate_to_peptide_to_pool_idx[
+                        other_replicate_idx
+                    ][peptide]
+
+                    for other_peptide in pool_to_peptides_2[other_pool_idx]:
+                        if other_peptide != peptide:
+                            peptide_to_invalid_excluding_replicate[replicate_idx][
+                                peptide
+                            ].add(other_peptide)
+                            peptide_to_invalid_excluding_replicate[replicate_idx][
+                                other_peptide
+                            ].add(peptide)
+
+    # print("peptide_to_invalid_excluding_replicate", peptide_to_invalid_excluding_replicate)
+    for i in range(s.num_replicates):
+        pool_to_peptides = s.assignments[i]
+
+        merged = set()
+        # next, try to merge any pools that are smaller than the max size
+        for pool_idx_1, peptides_1 in list(pool_to_peptides.items()):
+            if pool_idx_1 in merged:
+                continue
+
+            if len(peptides_1) >= s.max_peptides_per_pool:
+                continue
+
+            if len(peptides_1) == 0:
+                # skip empty pools, they'll be removed at the end
+                continue
+
+            for pool_idx_2, peptides_2 in list(pool_to_peptides.items()):
+                if pool_idx_1 == pool_idx_2:
+                    # can't merge a pool with itself
+                    continue
+                if len(peptides_2) == 0:
+                    # skip empty pools, they'll be removed at the end
+                    continue
+
+                if len(peptides_1) + len(peptides_2) >= s.max_peptides_per_pool:
+                    # can't exceed the max pool size
+                    continue
+
+                all_valid = True
+                # check if any peptides in pool 1 are invalid with any peptides in pool 2
+                combined_peptides = list(peptides_1) + list(peptides_2)
+                for peptide in list(combined_peptides):
+                    other_peptides = {p for p in combined_peptides if p != peptide}
+                    all_valid = (
+                        len(
+                            peptide_to_invalid_excluding_replicate[i][
+                                peptide
+                            ].intersection(other_peptides)
+                        )
+                        == 0
+                    )
+                    if not all_valid:
+                        break
+
+                if all_valid:
+                    num_merged += 1
+                    print(
+                        "-- merging pools %d and %d in replicate %d"
+                        % (pool_idx_1, pool_idx_2, i + 1)
+                    )
+                    pool_to_peptides[pool_idx_1] = np.array(combined_peptides)
+                    pool_to_peptides[pool_idx_2] = np.array([])
+                    merged.update([pool_idx_1, pool_idx_2])
+                    break
+
+    # just in case we ended up with any empty pools, remove them from the solution
+    s.remove_empty_pools()
+    return num_merged
+
+
+def cleanup(s: Solution, verbose: bool = True) -> int:
+    total_num_merged = 0
+    num_merged = merge_small_pools(s)
+    while num_merged > 0:
+        if verbose:
+            print(
+                "-- merged %d small pools, final number of pools: %d"
+                % (num_merged, s.num_pools())
+            )
+        total_num_merged += num_merged
+        num_merged = merge_small_pools(s)
+    return total_num_merged
+
+
 def optimize(
     s: Solution,
     max_iters: int = 2000,
     verbose: bool = False,
     add_pool_if_stuck: bool = True,
     return_history: bool = False,
 ) -> bool:
@@ -256,14 +368,18 @@
                         % (len(s.assignments[replicate_idx]), replicate_idx + 1)
                     )
                 s.add_empty_pool(replicate_idx)
             num_iters_without_improvement = 0
 
     result = old_num_violations == 0
 
-    # just in case we ended up with any empty pools, remove them from the solution
-    s.remove_empty_pools()
+    # clean up the solution by merging small pools
+    # and removing any empty pools
+    cleanup(s, verbose=verbose)
+
+    if result == 0:
+        assert is_valid(s)
 
     if return_history:
         return result, np.array(history)
     else:
         return result
```

### Comparing `golfy-1.7.0/golfy/solution.py` & `golfy-1.8.0/golfy/solution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.7.0/golfy/util.py` & `golfy-1.8.0/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-1.7.0/golfy/validity.py` & `golfy-1.8.0/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-1.7.0/golfy.egg-info/PKG-INFO` & `golfy-1.8.0/golfy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.7.0
+Version: 1.8.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.7.0/pyproject.toml` & `golfy-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-1.7.0/tests/test_deconvolution.py` & `golfy-1.8.0/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.7.0/tests/test_init.py` & `golfy-1.8.0/tests/test_init.py`

 * *Files identical despite different names*

