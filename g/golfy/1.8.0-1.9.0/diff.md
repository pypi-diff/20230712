# Comparing `tmp/golfy-1.8.0.tar.gz` & `tmp/golfy-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.8.0.tar", last modified: Tue Jul 11 21:58:46 2023, max compression
+gzip compressed data, was "golfy-1.9.0.tar", last modified: Wed Jul 12 20:43:35 2023, max compression
```

## Comparing `golfy-1.8.0.tar` & `golfy-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 21:58:46.372710 golfy-1.8.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.8.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-11 21:58:46.372598 golfy-1.8.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.8.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 21:58:46.370950 golfy-1.8.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      630 2023-07-11 21:49:17.000000 golfy-1.8.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.8.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     9217 2023-07-11 20:03:28.000000 golfy-1.8.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)    14407 2023-07-11 21:49:36.000000 golfy-1.8.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4089 2023-07-11 19:30:21.000000 golfy-1.8.0/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.8.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.8.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.8.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 21:58:46.371546 golfy-1.8.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      415 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-11 21:58:46.000000 golfy-1.8.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.8.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.8.0/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-11 21:58:46.372749 golfy-1.8.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-11 21:58:46.372321 golfy-1.8.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.8.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     1660 2023-07-07 14:04:35.000000 golfy-1.8.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.8.0/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:43:35.495134 golfy-1.9.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.9.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-12 20:43:35.495001 golfy-1.9.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.9.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:43:35.493101 golfy-1.9.0/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      693 2023-07-12 20:33:04.000000 golfy-1.9.0/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.9.0/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)    18052 2023-07-12 20:19:24.000000 golfy-1.9.0/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4254 2023-07-12 20:42:46.000000 golfy-1.9.0/golfy/main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6810 2023-07-12 19:40:02.000000 golfy-1.9.0/golfy/merging.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11274 2023-07-12 20:19:16.000000 golfy-1.9.0/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4177 2023-07-12 19:26:25.000000 golfy-1.9.0/golfy/solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.9.0/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.9.0/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.9.0/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:43:35.493703 golfy-1.9.0/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      479 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 20:43:35.000000 golfy-1.9.0/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.9.0/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.9.0/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-12 20:43:35.495167 golfy-1.9.0/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:43:35.494703 golfy-1.9.0/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.9.0/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      538 2023-07-12 20:35:22.000000 golfy-1.9.0/tests/test_find_best_solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-1.9.0/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-1.9.0/tests/test_optimize.py
```

### Comparing `golfy-1.8.0/LICENSE` & `golfy-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.8.0/PKG-INFO` & `golfy-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.8.0
+Version: 1.9.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.8.0/README.md` & `golfy-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `golfy-1.8.0/golfy/__init__.py` & `golfy-1.9.0/golfy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,19 +5,21 @@
     SpotCounts,
     DeconvolutionResult,
 )
 from .initialization import init
 from .optimization import optimize
 from .solution import Solution
 from .validity import is_valid, count_violations, violations_per_replicate
+from .main import find_best_solution
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 __all__ = [
     "__version__",
+    "find_best_solution",
     "Solution",
     "init",
     "optimize",
     "count_violations",
     "is_valid",
     "violations_per_replicate",
     "simulate_elispot_counts",
```

### Comparing `golfy-1.8.0/golfy/deconvolution.py` & `golfy-1.9.0/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.8.0/golfy/initialization.py` & `golfy-1.9.0/golfy/initialization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,252 @@
 from collections import defaultdict
 import math
 from typing import Optional, Literal
 
 import numpy as np
 
 from .solution import Solution
-from .types import PeptidePairList
+from .types import PeptidePairList, Replicate
 from .util import pairs_to_dict, transitive_closure
 from .validity import count_violations
 
 
+def _pools_per_replicate(
+    num_peptides: int,
+    max_peptides_per_pool: int,
+    num_replicates: int,
+    allow_extra_pools: bool,
+    verbose: bool,
+) -> dict[Replicate, int]:
+    too_few_pools = num_peptides < max_peptides_per_pool**2
+    if too_few_pools and not allow_extra_pools and verbose:
+        print(
+            "Warning: cannot satisfy constraints with %d peptides and %d peptides per pool (max allowed %d)"
+            % (num_peptides, max_peptides_per_pool, int(np.sqrt(num_peptides)))
+        )
+    num_pools_first_replicate = int(np.ceil(num_peptides / max_peptides_per_pool))
+    result = {0: num_pools_first_replicate}
+    for replicate_idx in range(1, num_replicates):
+        if too_few_pools and allow_extra_pools:
+            max_peptides_per_pool = num_pools_first_replicate
+            result[replicate_idx] = int(np.ceil(num_peptides / max_peptides_per_pool))
+        else:
+            result[replicate_idx] = num_pools_first_replicate
+    return result
+
+
 def _random_init(
-    num_peptides: int = 100,
-    peptides_per_pool: int = 5,
-    num_replicates: int = 3,
-    num_pools: Optional[int] = None,
+    num_peptides: int,
+    max_peptides_per_pool: int,
+    num_replicates: int,
+    num_pools_per_replicate: dict[Replicate, int],
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
+    allow_extra_pools: bool = False,
     verbose: bool = False,
 ) -> Solution:
-    if num_pools is None:
-        num_pools = int(np.ceil(num_peptides / peptides_per_pool))
-
     replicate_to_pool_to_peptides = {}
     for i in range(num_replicates):
         peptide_array = np.arange(num_peptides)
         np.random.shuffle(peptide_array)
         pool_assignments = {}
         replicate_to_pool_to_peptides[i] = pool_assignments
-
+        num_pools = num_pools_per_replicate[i]
+        peptides_per_pool = int(np.ceil(num_peptides / num_pools))
         for j in range(num_pools):
             start_idx = peptides_per_pool * j
             end_idx = peptides_per_pool * (j + 1)
             pool_assignments[j] = peptide_array[start_idx:end_idx]
 
     return Solution(
         num_peptides=num_peptides,
-        max_peptides_per_pool=peptides_per_pool,
+        max_peptides_per_pool=max_peptides_per_pool,
         num_replicates=num_replicates,
         invalid_neighbors=invalid_neighbors,
         preferred_neighbors=preferred_neighbors,
         assignments=replicate_to_pool_to_peptides,
     )
 
 
-def _greedy_init(
-    num_peptides: int = 100,
-    peptides_per_pool: int = 5,
-    num_replicates: int = 3,
-    num_pools: Optional[int] = None,
+def _singleton_init(
+    num_peptides: int,
+    max_peptides_per_pool: int,
+    num_replicates: int,
+    num_pools_per_replicate: dict[Replicate, int],
+    invalid_neighbors: PeptidePairList = [],
+    preferred_neighbors: PeptidePairList = [],
+    allow_extra_pools: bool = False,
+    verbose: bool = False,
+) -> Solution:
+    """
+    Initialize every peptide to be in its own pool
+    """
+
+    replicate_to_pool_to_peptides = {}
+    for i in range(num_replicates):
+        pool_to_peptides = {}
+        for p in range(num_peptides):
+            pool_to_peptides[p] = np.array([p])
+        replicate_to_pool_to_peptides[i] = pool_to_peptides
+    return Solution(
+        num_peptides=num_peptides,
+        max_peptides_per_pool=max_peptides_per_pool,
+        num_replicates=num_replicates,
+        invalid_neighbors=invalid_neighbors,
+        preferred_neighbors=preferred_neighbors,
+        assignments=replicate_to_pool_to_peptides,
+    )
+
+
+def _valid_init(
+    num_peptides: int,
+    max_peptides_per_pool: int,
+    num_replicates: int,
+    num_pools_per_replicate: dict[Replicate, int],
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
+    allow_extra_pools: bool = False,
     verbose: bool = False,
 ) -> Solution:
-    if num_pools is None:
-        num_pools = int(np.ceil(num_peptides / peptides_per_pool))
+    peptide_to_invalid = pairs_to_dict(invalid_neighbors)
+    peptide_to_preferred = transitive_closure(pairs_to_dict(preferred_neighbors))
+    if verbose:
+        print("[_valid_init] Invalid neighbors: %s" % (peptide_to_invalid,))
+        print("[_valid_init] Preferred neighbors: %s" % (peptide_to_preferred,))
+
+    replicate_to_pool_to_peptides = {}
+
+    random_peptide_order = np.arange(num_peptides)
+    np.random.shuffle(random_peptide_order)
+    assert len(set(random_peptide_order)) == num_peptides
+    # assign all peptides with preferred neighbors first
+    peptides_with_preferred_neighbors = [
+        p for p in random_peptide_order if p in peptide_to_preferred
+    ]
+    peptides_without_preferred_neighbors = [
+        p for p in random_peptide_order if p not in peptide_to_preferred
+    ]
+    peptide_list = (
+        peptides_with_preferred_neighbors + peptides_without_preferred_neighbors
+    )
+    for i in range(num_replicates):
+        num_pools = num_pools_per_replicate[i]
+        peptides_per_pool = int(math.ceil(num_peptides / num_pools))
+
+        peptide_to_pool = {}
+        pool_to_peptides = defaultdict(set)
+
+        def add_to_pool(peptide, pool_idx):
+            pool = pool_to_peptides[pool_idx]
+            pool.add(peptide)
+            peptide_to_pool[peptide] = pool_idx
+            for other_peptide in pool:
+                peptide_to_invalid[peptide].add(other_peptide)
+                peptide_to_invalid[other_peptide].add(peptide)
+
+        def curr_num_pools():
+            return len(pool_to_peptides)
+
+        def make_new_pool(peptide):
+            new_pool_idx = curr_num_pools()
+            add_to_pool(peptide, new_pool_idx)
+            return new_pool_idx
+
+        for peptide in peptide_list:
+            for preferred_neighbor in peptide_to_preferred.get(peptide, []):
+                if preferred_neighbor in peptide_to_invalid[peptide]:
+                    if verbose:
+                        print(
+                            "[_greedy_init] replicate %d, peptide %d already invalid with preferred neighbor %d"
+                            % (i, peptide, preferred_neighbor)
+                        )
+                    continue
+                preferred_pool_idx = peptide_to_pool.get(preferred_neighbor)
+                if preferred_pool_idx is None:
+                    if verbose:
+                        print(
+                            "[_greedy_init] replicate %d, peptide %d, preferred neighbor %d not in a pool yet"
+                            % (i, peptide, preferred_neighbor)
+                        )
+                    continue
+                preferred_pool = pool_to_peptides[preferred_pool_idx]
+                if len(preferred_pool) >= peptides_per_pool:
+                    if verbose:
+                        print(
+                            "[_greedy_init] replicate %d, preferred neighbor %d in pool %d which is already full"
+                            % (i, preferred_neighbor, preferred_pool_idx)
+                        )
+                    continue
+
+                add_to_pool(peptide, preferred_pool_idx)
+                if verbose:
+                    print(
+                        "[_greedy_init] replicate %d, adding peptide %d to preferred pool %d to pair with peptide %d"
+                        % (i, peptide, preferred_pool_idx, preferred_neighbor)
+                    )
+                break
+            # if we didn't get a preferred peptide pool that's valid
+            # and there's room for more pools, just make a singleton
+            if peptide not in peptide_to_pool:
+                if curr_num_pools() < num_pools:
+                    assigned_pool_idx = make_new_pool(peptide)
+                    if verbose:
+                        print(
+                            "[_greedy_init] replicate %d, making new pool %d for peptide %d"
+                            % (i, assigned_pool_idx, peptide)
+                        )
 
+            # otherwise, try to find a valid pool
+            if peptide not in peptide_to_pool:
+                for pool_idx, pool in pool_to_peptides.items():
+                    if len(pool) < peptides_per_pool:
+                        disallowed_peptides = peptide_to_invalid[peptide]
+                        valid = all(
+                            [
+                                other_peptide not in disallowed_peptides
+                                for other_peptide in pool
+                            ]
+                        )
+                        if valid:
+                            add_to_pool(peptide, pool_idx)
+                            break
+
+            # otherwise, make a new pool
+            if peptide not in peptide_to_pool:
+                if not allow_extra_pools and verbose:
+                    print(
+                        "Warning: unable to create valid configuration without exceeding max pools for replicate %d (max %d, adding %d)"
+                        % (i + 1, num_pools, curr_num_pools() + 1)
+                    )
+                make_new_pool(peptide)
+
+        replicate_to_pool_to_peptides[i] = {
+            pool_idx: np.array(sorted(peptides))
+            for (pool_idx, peptides) in pool_to_peptides.items()
+        }
+    return Solution(
+        num_peptides=num_peptides,
+        max_peptides_per_pool=max_peptides_per_pool,
+        num_replicates=num_replicates,
+        invalid_neighbors=invalid_neighbors,
+        preferred_neighbors=preferred_neighbors,
+        assignments=replicate_to_pool_to_peptides,
+    )
+
+
+def _greedy_init(
+    num_peptides: int,
+    max_peptides_per_pool: int,
+    num_replicates: int,
+    num_pools_per_replicate: dict[Replicate, int],
+    invalid_neighbors: PeptidePairList = [],
+    preferred_neighbors: PeptidePairList = [],
+    allow_extra_pools: bool = False,
+    verbose: bool = False,
+) -> Solution:
     peptide_to_invalid = pairs_to_dict(invalid_neighbors)
     peptide_to_preferred = transitive_closure(pairs_to_dict(preferred_neighbors))
     if verbose:
         print("[_greedy_init] Invalid neighbors: %s" % (peptide_to_invalid,))
         print("[_greedy_init] Preferred neighbors: %s" % (peptide_to_preferred,))
 
     replicate_to_pool_to_peptides = {}
@@ -74,14 +261,17 @@
     peptides_without_preferred_neighbors = [
         p for p in random_peptide_order if p not in peptide_to_preferred
     ]
     peptide_list = (
         peptides_with_preferred_neighbors + peptides_without_preferred_neighbors
     )
     for i in range(num_replicates):
+        num_pools = num_pools_per_replicate[i]
+        peptides_per_pool = int(math.ceil(num_peptides / num_pools))
+
         peptide_to_pool = {}
         pool_to_peptides = defaultdict(set)
 
         def add_to_pool(peptide, pool_idx):
             pool = pool_to_peptides[pool_idx]
             pool.add(peptide)
             peptide_to_pool[peptide] = pool_idx
@@ -162,40 +352,44 @@
                     if len(pool) < peptides_per_pool:
                         add_to_pool(peptide, pool_idx)
                         break
 
             # lastly, violate the num_pools constraint to make a
             # new singleton anyways
             if peptide not in peptide_to_pool:
-                make_new_pool(peptide)
+                if allow_extra_pools:
+                    make_new_pool(peptide)
+                else:
+                    raise ValueError("Unable to create valid configuration")
 
         replicate_to_pool_to_peptides[i] = {
             pool_idx: np.array(sorted(peptides))
             for (pool_idx, peptides) in pool_to_peptides.items()
         }
 
     return Solution(
         num_peptides=num_peptides,
-        max_peptides_per_pool=peptides_per_pool,
+        max_peptides_per_pool=max_peptides_per_pool,
         num_replicates=num_replicates,
         invalid_neighbors=invalid_neighbors,
         preferred_neighbors=preferred_neighbors,
         assignments=replicate_to_pool_to_peptides,
     )
 
 
 def init(
     num_peptides: int = 100,
-    peptides_per_pool: int = 5,
+    max_peptides_per_pool: int = 5,
     num_replicates: int = 3,
-    num_pools_per_replicate: Optional[int] = None,
+    num_pools_per_replicate: Optional[int | dict[Replicate, int]] = None,
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
-    strategy: Literal["greedy", "random"] = "greedy",
-    verbose=False,
+    strategy: Literal["greedy", "random", "valid", "singleton"] = "greedy",
+    allow_extra_pools: bool = False,
+    verbose: bool = False,
 ) -> Solution:
     """
     Initialize a Solution for a given configuration
 
     Args
     ----
     num_peptides
@@ -213,36 +407,56 @@
     invalid_neighbors
         list of peptide pairs that cannot be in the same pool
 
     preferred_neighbors
         list of peptide pairs that should be in the same pool
 
     strategy
-        initialization strategy, either "greedy" or "random" (default: "greedy")
+        initialization strategy, one of {"greedy", "random", "singleton", "valid"} (default: "greedy")
+
+    allow_extra_pools
+        whether to allow extra pools to be created to satisfy constraints (default: False)
+
+    verbose
+        print diagnostic information during initialization (default: False)
     """
-    if strategy == "greedy":
-        s = _greedy_init(
-            num_peptides=num_peptides,
-            peptides_per_pool=peptides_per_pool,
-            num_replicates=num_replicates,
-            num_pools=num_pools_per_replicate,
-            invalid_neighbors=invalid_neighbors,
-            preferred_neighbors=preferred_neighbors,
-            verbose=verbose,
-        )
-    elif strategy == "random":
-        s = _random_init(
+    fn = {
+        "greedy": _greedy_init,
+        "random": _random_init,
+        "singleton": _singleton_init,
+        "valid": _valid_init,
+    }.get(strategy)
+    if num_pools_per_replicate is None:
+        num_pools_per_replicate = _pools_per_replicate(
             num_peptides=num_peptides,
-            peptides_per_pool=peptides_per_pool,
+            max_peptides_per_pool=max_peptides_per_pool,
             num_replicates=num_replicates,
-            num_pools=num_pools_per_replicate,
-            invalid_neighbors=invalid_neighbors,
-            preferred_neighbors=preferred_neighbors,
+            allow_extra_pools=allow_extra_pools,
             verbose=verbose,
         )
-    else:
-        raise ValueError("Unknown initialization strategy: '%s'" % strategy)
+    elif isinstance(num_pools_per_replicate, int):
+        num_pools_per_replicate = {
+            i: num_pools_per_replicate for i in range(num_replicates)
+        }
+    if fn is None:
+        raise ValueError("Unknown initialization strategy: '%s'" % (strategy,))
 
+    if verbose:
+        print(
+            "Using '%s' initialization strategy, pools per replicate: %s"
+            % (strategy, num_pools_per_replicate)
+        )
+    kwargs = dict(
+        num_peptides=num_peptides,
+        max_peptides_per_pool=max_peptides_per_pool,
+        num_replicates=num_replicates,
+        num_pools_per_replicate=num_pools_per_replicate,
+        invalid_neighbors=invalid_neighbors,
+        preferred_neighbors=preferred_neighbors,
+        allow_extra_pools=allow_extra_pools,
+        verbose=verbose,
+    )
+    s = fn(**kwargs)
     violations = count_violations(s)
     if verbose:
         print("Generated solution with %d initial violations" % (violations))
     return s
```

### Comparing `golfy-1.8.0/golfy/optimization.py` & `golfy-1.9.0/golfy/optimization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from collections import defaultdict
 import random
 import time
 
 import numpy as np
 
+from .merging import cleanup
 from .solution import Solution
-from .types import SwapCandidateList, ReplicateToNeighborDict
-from .validity import violations_per_replicate, is_valid
+from .types import SwapCandidateList, ReplicateToNeighborDict, Replicate, Pool, Peptide
+from .validity import violations_per_replicate, is_valid, count_violations
 from .util import pairs_to_dict
 
 
 def find_violating_peptides(
     s: Solution,
 ) -> tuple[SwapCandidateList, ReplicateToNeighborDict]:
     replicate_to_pool_to_peptides = s.assignments
@@ -31,252 +32,163 @@
         replicate_to_neighbor_dict[replicate_idx] = {
             peptide: neighbors.copy()
             for (peptide, neighbors) in peptide_to_neighbors.items()
         }
     return needs_swap, replicate_to_neighbor_dict
 
 
+def _groupby_replicate(
+    swap_candidates: SwapCandidateList,
+) -> dict[Replicate, tuple[Pool, Peptide]]:
+    result = defaultdict(list)
+    for replicate_idx, pool_idx, peptide in swap_candidates:
+        result[replicate_idx].append((pool_idx, peptide))
+    return result
+
+
 def improve_solution(s: Solution, verbose: bool = False):
     replicate_to_pool_to_peptides = s.assignments
+    replicate_to_peptide_to_pool = s.replicate_to_peptide_to_pool_dict()
 
     needs_swap, replicate_to_neighbor_dict = find_violating_peptides(s)
 
     random.shuffle(needs_swap)
 
-    swapped_pools = set()
-    swapped_peptides = set()
-    empty_pools_per_replicate = {
-        replicate_idx: {
+    replicate_to_swap_candidates = _groupby_replicate(needs_swap)
+
+    for replicate_idx in sorted(replicate_to_swap_candidates.keys()):
+        pool_to_peptides = replicate_to_pool_to_peptides[replicate_idx]
+        peptide_to_pool_idx = replicate_to_peptide_to_pool[replicate_idx]
+        neighbors = replicate_to_neighbor_dict[replicate_idx]
+        swapped_pools = set()
+        swapped_peptides = set()
+        empty_pools = {
             pool_idx
-            for (pool_idx, pool_peptides) in pool_to_peptides.items()
+            for (pool_idx, pool_peptides) in replicate_to_pool_to_peptides[
+                replicate_idx
+            ].items()
             if len(pool_peptides) == 0
         }
-        for (replicate_idx, pool_to_peptides) in replicate_to_pool_to_peptides.items()
-    }
-    for replicate_idx, pool_idx_a, peptide_a in needs_swap:
-        if pool_idx_a in swapped_pools or peptide_a in swapped_peptides:
-            continue
-
-        pool_to_peptides = replicate_to_pool_to_peptides[replicate_idx]
-        pool_a = pool_to_peptides[pool_idx_a]
-        empty_pools = empty_pools_per_replicate[replicate_idx]
-        # if a pool is empty, just move the offending peptide there
-        if empty_pools:
-            pool_idx_b = random.choice(list(empty_pools))
-            s.move_peptide(replicate_idx, pool_idx_a, peptide_a, pool_idx_b)
-            swapped_pools.add(pool_idx_a)
-            swapped_pools.add(pool_idx_b)
-            swapped_peptides.add(peptide_a)
-            empty_pools.remove(pool_idx_b)
-        else:
-            other_peptides = []
-            peptide_to_pool_idx = {}
-            for pool_idx_i, pool_peptides_i in pool_to_peptides.items():
-                if pool_idx_i != pool_idx_a and pool_idx_i not in swapped_pools:
-                    all_peptides_ok = True
-                    for p in pool_peptides_i:
-                        peptide_to_pool_idx[p] = pool_idx_i
-                        all_peptides_ok = all_peptides_ok and (
-                            peptide_a
-                            not in replicate_to_neighbor_dict[replicate_idx][p]
-                        )
-                    if all_peptides_ok:
-                        other_peptides.extend(
-                            [p for p in pool_peptides_i if p not in swapped_peptides]
-                        )
 
-            if len(other_peptides) == 0:
-                if verbose:
-                    print(
-                        "Not able to find a valid peptide to swap with for (%s, %s, %s)"
-                        % (replicate_idx, pool_idx_a, peptide_a)
-                    )
+        all_pool_idx_peptide_pairs = list(pool_to_peptides.items())
+        random.shuffle(all_pool_idx_peptide_pairs)
+        for pool_idx_a, peptide_a in replicate_to_swap_candidates[replicate_idx]:
+            if pool_idx_a in swapped_pools or peptide_a in swapped_peptides:
                 continue
-            peptide_b = random.choice(other_peptides)
-            pool_idx_b = peptide_to_pool_idx[peptide_b]
-            assert peptide_a != peptide_b
-            assert pool_idx_a != pool_idx_b
-            pool_b = pool_to_peptides[pool_idx_b]
-            if (
-                len(pool_a) > 1
-                and len(pool_b) < s.max_peptides_per_pool
-                and random.choice([False, True])
-            ):
-                # just move peptide a to the pool with fewer than max peptides
-                if verbose:
-                    print(
-                        "Moving peptide %d from pool %d to pool %d"
-                        % (peptide_a, pool_idx_a, pool_idx_b)
-                    )
-                s.move_peptide(replicate_idx, pool_idx_a, peptide_a, pool_idx_b)
-                swapped_pools.add(pool_idx_a)
-                swapped_pools.add(pool_idx_b)
-                swapped_peptides.add(peptide_a)
-            else:
-                if verbose:
-                    print("Before swap")
-                    print(
-                        "pool",
-                        pool_idx_a,
-                        "peptide",
-                        peptide_a,
-                        pool_to_peptides[pool_idx_a],
-                    )
-                    print(
-                        "pool",
-                        pool_idx_b,
-                        "peptide",
-                        peptide_b,
-                        pool_to_peptides[pool_idx_b],
-                    )
-
-                # actually swap them
-                s.swap_peptides(
-                    replicate_idx, pool_idx_a, peptide_a, pool_idx_b, peptide_b
-                )
-
-                if verbose:
-                    print("After")
-                    print(
-                        "pool",
-                        pool_idx_a,
-                        "peptide",
-                        peptide_a,
-                        pool_to_peptides[pool_idx_a],
-                    )
-                    print(
-                        "pool",
-                        pool_idx_b,
-                        "peptide",
-                        peptide_b,
-                        pool_to_peptides[pool_idx_b],
-                    )
+            previous_neighbors = neighbors[peptide_a]
 
+            # if a pool is empty, just move the offending peptide there
+            if empty_pools:
+                pool_idx_b = random.choice(list(empty_pools))
+                s.move_peptide(replicate_idx, pool_idx_a, peptide_a, pool_idx_b)
                 swapped_pools.add(pool_idx_a)
                 swapped_pools.add(pool_idx_b)
                 swapped_peptides.add(peptide_a)
-                swapped_peptides.add(peptide_b)
+                empty_pools.remove(pool_idx_b)
 
+            else:
+                other_peptides = []
+                for pool_idx_i, pool_peptides_i in all_pool_idx_peptide_pairs:
+                    if pool_idx_i == pool_idx_a:
+                        continue
 
-def merge_small_pools(s: Solution) -> int:
-    num_merged = 0
-    peptide_to_invalid = pairs_to_dict(s.invalid_neighbors)
-    peptide_to_invalid_excluding_replicate = {
-        replicate_idx: peptide_to_invalid.copy()
-        for replicate_idx in range(s.num_replicates)
-    }
-    replicate_to_peptide_to_pool_idx = {}
-
-    for replicate_idx, pool_to_peptides in s.assignments.items():
-        peptide_to_pool_idx = {}
-        replicate_to_peptide_to_pool_idx[replicate_idx] = peptide_to_pool_idx
-        for pool_idx, peptides in pool_to_peptides.items():
-            for peptide in peptides:
-                peptide_to_pool_idx[peptide] = pool_idx
-    # print("replicate_to_peptide_to_pool_idx", replicate_to_peptide_to_pool_idx)
-
-    for replicate_idx, pool_to_peptides_1 in s.assignments.items():
-        for other_replicate_idx, pool_to_peptides_2 in s.assignments.items():
-            if replicate_idx == other_replicate_idx:
-                continue
-            for peptides in pool_to_peptides.values():
-                for peptide in peptides:
-                    other_pool_idx = replicate_to_peptide_to_pool_idx[
-                        other_replicate_idx
-                    ][peptide]
-
-                    for other_peptide in pool_to_peptides_2[other_pool_idx]:
-                        if other_peptide != peptide:
-                            peptide_to_invalid_excluding_replicate[replicate_idx][
-                                peptide
-                            ].add(other_peptide)
-                            peptide_to_invalid_excluding_replicate[replicate_idx][
-                                other_peptide
-                            ].add(peptide)
-
-    # print("peptide_to_invalid_excluding_replicate", peptide_to_invalid_excluding_replicate)
-    for i in range(s.num_replicates):
-        pool_to_peptides = s.assignments[i]
-
-        merged = set()
-        # next, try to merge any pools that are smaller than the max size
-        for pool_idx_1, peptides_1 in list(pool_to_peptides.items()):
-            if pool_idx_1 in merged:
-                continue
-
-            if len(peptides_1) >= s.max_peptides_per_pool:
-                continue
+                    if pool_idx_i in swapped_pools:
+                        continue  # already swapped this pool
 
-            if len(peptides_1) == 0:
-                # skip empty pools, they'll be removed at the end
-                continue
+                    all_peptides_ok = True
+                    for p in pool_peptides_i:
+                        if p in swapped_peptides or p in previous_neighbors:
+                            all_peptides_ok = False
+                            break
 
-            for pool_idx_2, peptides_2 in list(pool_to_peptides.items()):
-                if pool_idx_1 == pool_idx_2:
-                    # can't merge a pool with itself
-                    continue
-                if len(peptides_2) == 0:
-                    # skip empty pools, they'll be removed at the end
-                    continue
+                    if all_peptides_ok:
+                        other_peptides.extend(
+                            [p for p in pool_peptides_i if p not in swapped_peptides]
+                        )
 
-                if len(peptides_1) + len(peptides_2) >= s.max_peptides_per_pool:
-                    # can't exceed the max pool size
+                if len(other_peptides) == 0:
+                    if verbose:
+                        print(
+                            "Not able to find a valid peptide to swap with for (%s, %s, %s)"
+                            % (replicate_idx, pool_idx_a, peptide_a)
+                        )
                     continue
 
-                all_valid = True
-                # check if any peptides in pool 1 are invalid with any peptides in pool 2
-                combined_peptides = list(peptides_1) + list(peptides_2)
-                for peptide in list(combined_peptides):
-                    other_peptides = {p for p in combined_peptides if p != peptide}
-                    all_valid = (
-                        len(
-                            peptide_to_invalid_excluding_replicate[i][
-                                peptide
-                            ].intersection(other_peptides)
+                peptide_b = random.choice(other_peptides)
+                pool_idx_b = peptide_to_pool_idx[peptide_b]
+                assert peptide_a != peptide_b
+                assert pool_idx_a != pool_idx_b
+                pool_a = pool_to_peptides[pool_idx_a]
+                pool_b = pool_to_peptides[pool_idx_b]
+                if (
+                    len(pool_a) > 1
+                    and len(pool_b) < s.max_peptides_per_pool
+                    and random.choice([False, True])
+                ):
+                    # just move peptide a to the pool with fewer than max peptides
+                    if verbose:
+                        print(
+                            "Moving peptide %d from pool %d to pool %d"
+                            % (peptide_a, pool_idx_a, pool_idx_b)
+                        )
+                    s.move_peptide(replicate_idx, pool_idx_a, peptide_a, pool_idx_b)
+                    swapped_pools.add(pool_idx_a)
+                    swapped_pools.add(pool_idx_b)
+                    swapped_peptides.add(peptide_a)
+                else:
+                    if verbose:
+                        print("Before swap")
+                        print(
+                            "pool",
+                            pool_idx_a,
+                            "peptide",
+                            peptide_a,
+                            pool_to_peptides[pool_idx_a],
+                        )
+                        print(
+                            "pool",
+                            pool_idx_b,
+                            "peptide",
+                            peptide_b,
+                            pool_to_peptides[pool_idx_b],
                         )
-                        == 0
-                    )
-                    if not all_valid:
-                        break
 
-                if all_valid:
-                    num_merged += 1
-                    print(
-                        "-- merging pools %d and %d in replicate %d"
-                        % (pool_idx_1, pool_idx_2, i + 1)
+                    # actually swap them
+                    s.swap_peptides(
+                        replicate_idx, pool_idx_a, peptide_a, pool_idx_b, peptide_b
                     )
-                    pool_to_peptides[pool_idx_1] = np.array(combined_peptides)
-                    pool_to_peptides[pool_idx_2] = np.array([])
-                    merged.update([pool_idx_1, pool_idx_2])
-                    break
-
-    # just in case we ended up with any empty pools, remove them from the solution
-    s.remove_empty_pools()
-    return num_merged
 
+                    if verbose:
+                        print("After")
+                        print(
+                            "pool",
+                            pool_idx_a,
+                            "peptide",
+                            peptide_a,
+                            pool_to_peptides[pool_idx_a],
+                        )
+                        print(
+                            "pool",
+                            pool_idx_b,
+                            "peptide",
+                            peptide_b,
+                            pool_to_peptides[pool_idx_b],
+                        )
 
-def cleanup(s: Solution, verbose: bool = True) -> int:
-    total_num_merged = 0
-    num_merged = merge_small_pools(s)
-    while num_merged > 0:
-        if verbose:
-            print(
-                "-- merged %d small pools, final number of pools: %d"
-                % (num_merged, s.num_pools())
-            )
-        total_num_merged += num_merged
-        num_merged = merge_small_pools(s)
-    return total_num_merged
+                    swapped_pools.add(pool_idx_a)
+                    swapped_pools.add(pool_idx_b)
+                    swapped_peptides.add(peptide_a)
+                    swapped_peptides.add(peptide_b)
 
 
 def optimize(
     s: Solution,
     max_iters: int = 2000,
     verbose: bool = False,
-    add_pool_if_stuck: bool = True,
+    allow_extra_pools: bool = True,
     return_history: bool = False,
 ) -> bool:
     """
     Iteratively update solution by randomly swapping a violating peptide with a random other peptide
 
     Args
     ----
@@ -285,16 +197,16 @@
 
     max_iters
         Maximum number of swaps to consider performing
 
     verbose
         print number of violations and pools for each iteration
 
-    add_pool_if_stuck
-        If no improvements have been made for 10 iters, add a pool
+    allow_extra_pools
+        If no improvements have been made for 3 iters, add a pool
         to the last replicate
 
     return_history
         Return array of constraint validation counts per iteration
 
 
     Returns True if non-violating solution found, False if solution still has violations after
@@ -303,15 +215,15 @@
     replicate_to_violation_count = violations_per_replicate(s)
     old_num_violations = sum(replicate_to_violation_count.values())
 
     history = [old_num_violations]
     if verbose:
         print("Initial solution has %s violations" % (old_num_violations,))
 
-    if old_num_violations / s.num_replicates > 1000:
+    if allow_extra_pools and (old_num_violations / s.num_replicates > 1000):
         # before first iteration, add a lot of empty pools to any replicates with
         # more than 1000 violations
         for replicate_idx, violation_count in replicate_to_violation_count.items():
             if violation_count > 1000:
                 num_new_pools = int(np.ceil(violation_count / 1000))
                 if verbose:
                     print(
@@ -352,34 +264,41 @@
         old_num_violations = new_num_violations
 
         if new_num_violations == 0:
             if verbose:
                 print("Found valid solution after %d swaps" % (i + 1,))
             break
 
-        if num_iters_without_improvement >= 3 and add_pool_if_stuck:
-            replicates_in_need = [
-                r for (r, v) in replicate_to_violation_count.items() if v > 0
-            ]
-            assert len(replicates_in_need) > 0
-            for replicate_idx in replicates_in_need:
-                if verbose:
-                    print(
-                        "-- adding pool %d to replicate %d"
-                        % (len(s.assignments[replicate_idx]), replicate_idx + 1)
-                    )
-                s.add_empty_pool(replicate_idx)
-            num_iters_without_improvement = 0
+        if num_iters_without_improvement >= 3:
+            if allow_extra_pools:
+                replicates_in_need = [
+                    r for (r, v) in replicate_to_violation_count.items() if v > 0
+                ]
+                assert len(replicates_in_need) > 0
+                for replicate_idx in replicates_in_need:
+                    if verbose:
+                        print(
+                            "-- adding pool %d to replicate %d"
+                            % (len(s.assignments[replicate_idx]), replicate_idx + 1)
+                        )
+                    s.add_empty_pool(replicate_idx)
+                num_iters_without_improvement = 0
+            else:
+                # give up if we can't solve this problem
+                break
 
     result = old_num_violations == 0
 
     # clean up the solution by merging small pools
     # and removing any empty pools
-    cleanup(s, verbose=verbose)
+    cleanup(s, verbose=verbose, max_iters=max_iters)
 
-    if result == 0:
-        assert is_valid(s)
+    if result and not is_valid(s):
+        raise ValueError(
+            "Solution is not valid after cleanup step! Violations: %d"
+            % (count_violations(s),)
+        )
 
     if return_history:
         return result, np.array(history)
     else:
         return result
```

### Comparing `golfy-1.8.0/golfy/solution.py` & `golfy-1.9.0/golfy/solution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from dataclasses import dataclass
 import numpy as np
 from typing import Iterable, Mapping
 
 from .types import PeptidePairList, Replicate, Pool, Peptide
 
 
@@ -109,18 +110,18 @@
         self,
     ) -> Mapping[Replicate, Mapping[Peptide, Pool]]:
         return {
             replicate_idx: self.peptide_to_pool_dict_for_replicate(replicate_idx)
             for replicate_idx in range(self.num_replicates)
         }
 
-    def peptide_to_replicate_pool_pair_dict(
+    def peptide_to_replicate_pool_pairs_dict(
         self,
-    ) -> Mapping[Peptide, tuple[Replicate, Pool]]:
-        return {
-            p: (replicate_idx, pool)
-            for (
-                replicate_idx,
-                peptide_to_pool,
-            ) in self.replicate_to_peptide_to_pool_dict().items()
-            for (p, pool) in peptide_to_pool.items()
-        }
+    ) -> Mapping[Peptide, list[tuple[Replicate, Pool]]]:
+        result = defaultdict(list)
+        for (
+            replicate_idx,
+            peptide_to_pool,
+        ) in self.replicate_to_peptide_to_pool_dict().items():
+            for peptide, pool in peptide_to_pool.items():
+                result[peptide].append((replicate_idx, pool))
+        return result
```

### Comparing `golfy-1.8.0/golfy/util.py` & `golfy-1.9.0/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-1.8.0/golfy/validity.py` & `golfy-1.9.0/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-1.8.0/golfy.egg-info/PKG-INFO` & `golfy-1.9.0/golfy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.8.0
+Version: 1.9.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.8.0/pyproject.toml` & `golfy-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-1.8.0/tests/test_deconvolution.py` & `golfy-1.9.0/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.8.0/tests/test_init.py` & `golfy-1.9.0/tests/test_init.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,44 @@
 from golfy import init
 
 
+def test_valid_init():
+    s = init(
+        num_peptides=100, max_peptides_per_pool=5, num_replicates=3, strategy="valid"
+    )
+    assert len(s.assignments) == 3
+    assert len(s.assignments[0]) == 20
+    assert len(s.assignments[0][0]) == 5
+
+
+def test_singleton_init():
+    s = init(
+        num_peptides=100,
+        max_peptides_per_pool=5,
+        num_replicates=3,
+        strategy="singleton",
+    )
+    assert len(s.assignments) == 3
+    assert len(s.assignments[0]) == 100
+    assert len(s.assignments[0][0]) == 1
+
+
 def test_random_init():
-    s = init(num_peptides=100, peptides_per_pool=5, num_replicates=3, strategy="random")
+    s = init(
+        num_peptides=100, max_peptides_per_pool=5, num_replicates=3, strategy="random"
+    )
     assert len(s.assignments) == 3
     assert len(s.assignments[0]) == 20
     assert len(s.assignments[0][0]) == 5
 
 
 def test_greedy_init():
-    s = init(num_peptides=100, peptides_per_pool=5, num_replicates=3, strategy="greedy")
+    s = init(
+        num_peptides=100, max_peptides_per_pool=5, num_replicates=3, strategy="greedy"
+    )
     assert len(s.assignments) == 3
     assert len(s.assignments[0]) == 20
     assert len(s.assignments[0][0]) == 5
 
 
 def test_greedy_init_with_preferred_neighbors():
     """
@@ -22,15 +47,15 @@
         2023-07-06 17:57:30 INFO     peptide_7 and peptide_10
         2023-07-06 17:57:30 INFO     peptide_12 and peptide_17
         2023-07-06 17:57:30 INFO     peptide_14 and peptide_15
         2023-07-06 17:57:30 INFO     peptide_15 and peptide_17
     """
     s = init(
         num_peptides=25,
-        peptides_per_pool=5,
+        max_peptides_per_pool=5,
         num_replicates=3,
         strategy="greedy",
         preferred_neighbors=[(7, 10), (12, 17), (14, 15), (15, 17)],
         verbose=True,
     )
     assert len(s.assignments) == 3
     assert len(s.assignments[0]) == 5
```

