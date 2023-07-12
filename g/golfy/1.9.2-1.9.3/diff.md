# Comparing `tmp/golfy-1.9.2.tar.gz` & `tmp/golfy-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.9.2.tar", last modified: Wed Jul 12 20:55:25 2023, max compression
+gzip compressed data, was "golfy-1.9.3.tar", last modified: Wed Jul 12 21:33:56 2023, max compression
```

## Comparing `golfy-1.9.2.tar` & `golfy-1.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:55:25.073547 golfy-1.9.2/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.9.2/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-12 20:55:25.073435 golfy-1.9.2/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.9.2/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:55:25.071669 golfy-1.9.2/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      693 2023-07-12 20:54:05.000000 golfy-1.9.2/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.9.2/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)    17960 2023-07-12 20:55:06.000000 golfy-1.9.2/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4254 2023-07-12 20:42:46.000000 golfy-1.9.2/golfy/main.py
--rw-r--r--   0 iskander   (501) staff       (20)     6810 2023-07-12 19:40:02.000000 golfy-1.9.2/golfy/merging.py
--rw-r--r--   0 iskander   (501) staff       (20)    11274 2023-07-12 20:19:16.000000 golfy-1.9.2/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4177 2023-07-12 19:26:25.000000 golfy-1.9.2/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.9.2/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.9.2/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.9.2/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:55:25.072314 golfy-1.9.2/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-12 20:55:25.000000 golfy-1.9.2/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      479 2023-07-12 20:55:25.000000 golfy-1.9.2/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-12 20:55:25.000000 golfy-1.9.2/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 20:55:25.000000 golfy-1.9.2/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 20:55:25.000000 golfy-1.9.2/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.9.2/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.9.2/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-12 20:55:25.073578 golfy-1.9.2/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 20:55:25.073161 golfy-1.9.2/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.9.2/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)      538 2023-07-12 20:35:22.000000 golfy-1.9.2/tests/test_find_best_solution.py
--rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-1.9.2/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-1.9.2/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 21:33:56.525096 golfy-1.9.3/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.9.3/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     3658 2023-07-12 21:33:56.524983 golfy-1.9.3/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     2932 2023-07-12 21:27:59.000000 golfy-1.9.3/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 21:33:56.523220 golfy-1.9.3/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      693 2023-07-12 21:28:41.000000 golfy-1.9.3/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-11 19:26:17.000000 golfy-1.9.3/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)    17960 2023-07-12 20:55:06.000000 golfy-1.9.3/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4264 2023-07-12 21:30:39.000000 golfy-1.9.3/golfy/main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6810 2023-07-12 19:40:02.000000 golfy-1.9.3/golfy/merging.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11274 2023-07-12 20:19:16.000000 golfy-1.9.3/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4177 2023-07-12 19:26:25.000000 golfy-1.9.3/golfy/solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.9.3/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.9.3/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.9.3/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 21:33:56.523787 golfy-1.9.3/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     3658 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      479 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-12 21:33:56.000000 golfy-1.9.3/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.9.3/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.9.3/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-12 21:33:56.525127 golfy-1.9.3/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-12 21:33:56.524730 golfy-1.9.3/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.9.3/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      538 2023-07-12 20:35:22.000000 golfy-1.9.3/tests/test_find_best_solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-1.9.3/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-1.9.3/tests/test_optimize.py
```

### Comparing `golfy-1.9.2/LICENSE` & `golfy-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/golfy/__init__.py` & `golfy-1.9.3/golfy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 from .initialization import init
 from .optimization import optimize
 from .solution import Solution
 from .validity import is_valid, count_violations, violations_per_replicate
 from .main import find_best_solution
 
-__version__ = "1.9.2"
+__version__ = "1.9.3"
 
 __all__ = [
     "__version__",
     "find_best_solution",
     "Solution",
     "init",
     "optimize",
```

### Comparing `golfy-1.9.2/golfy/deconvolution.py` & `golfy-1.9.3/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/golfy/initialization.py` & `golfy-1.9.3/golfy/initialization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/golfy/main.py` & `golfy-1.9.3/golfy/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from typing import Optional, Literal
 
 from .initialization import init
 from .optimization import optimize
 from .solution import Solution
 from .types import Replicate, Pool, Peptide, PeptidePairList
 from .validity import count_violations
@@ -86,27 +87,27 @@
     }
     best_solution = None
     best_violations = None
     best_num_pools = None
 
     for strategy, s in solutions.items():
         print(
-            "Initial solution for init strategy '%s', violations=%d, num_pools=%d"
+            "Initialized with strategy '%s': violations=%d, num_pools=%d"
             % (strategy, count_violations(s), s.num_pools())
         )
         optimize(s, allow_extra_pools=allow_extra_pools, verbose=verbose)
         violations = count_violations(s)
         num_pools = s.num_pools()
         print(
-            "After optimization strategy '%s', violations=%d, num_pools=%d"
+            "-- after optimization of '%s' solution: violations=%d, num_pools=%d"
             % (strategy, violations, num_pools)
         )
         if (
             best_solution is None
             or (violations < best_violations)
             or (violations == best_violations and num_pools < best_num_pools)
         ):
             best_solution = s
             best_violations = violations
             best_num_pools = num_pools
-            print("^ new best solution")
+            print("^^ new best solution")
     return best_solution
```

### Comparing `golfy-1.9.2/golfy/merging.py` & `golfy-1.9.3/golfy/merging.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/golfy/optimization.py` & `golfy-1.9.3/golfy/optimization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/golfy/solution.py` & `golfy-1.9.3/golfy/solution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/golfy/util.py` & `golfy-1.9.3/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/golfy/validity.py` & `golfy-1.9.3/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/pyproject.toml` & `golfy-1.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/tests/test_deconvolution.py` & `golfy-1.9.3/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/tests/test_find_best_solution.py` & `golfy-1.9.3/tests/test_find_best_solution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.9.2/tests/test_init.py` & `golfy-1.9.3/tests/test_init.py`

 * *Files identical despite different names*

