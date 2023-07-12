# Comparing `tmp/sparseconverter-0.3.1.tar.gz` & `tmp/sparseconverter-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparseconverter-0.3.1.tar", last modified: Tue Apr 18 12:52:48 2023, max compression
+gzip compressed data, was "sparseconverter-0.3.2.tar", last modified: Wed Jul 12 07:45:45 2023, max compression
```

## Comparing `sparseconverter-0.3.1.tar` & `sparseconverter-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/src/sparseconverter/
--rw-r--r--   0 runner    (1001) docker     (123)    46727 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/src/sparseconverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/src/sparseconverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 12:52:48.000000 sparseconverter-0.3.1/src/sparseconverter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:52:48.600355 sparseconverter-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-04-18 12:52:36.000000 sparseconverter-0.3.1/tests/test_sparseconverters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.129136 sparseconverter-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/src/sparseconverter/
+-rw-r--r--   0 runner    (1001) docker     (123)    50194 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/src/sparseconverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/src/sparseconverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/tests/test_sparseconverters.py
```

### Comparing `sparseconverter-0.3.1/LICENSE` & `sparseconverter-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparseconverter-0.3.1/PKG-INFO` & `sparseconverter-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseconverter
-Version: 0.3.1
+Version: 0.3.2
 Summary: Converter matrix and type determination for a range of array formats, focusing on sparse arrays
 Author-email: Dieter Weber <d.weber@fz-juelich.de>
 License: MIT License
         
         Copyright (c) 2022 LiberTEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -113,14 +113,21 @@
 
 * PyTorch arrays
 * SciPy sparse arrays as opposed to SciPy sparse matrices.
 * More detailed cost metric based on more real-world use cases and parameters.
 
 ## Changelog
 
+### 0.3.2
+
+* Detection and workaround for https://github.com/pydata/sparse/issues/602.
+* Detection and workaround for https://github.com/cupy/cupy/issues/7713.
+* Test with duplicates and scrambled indices.
+* Test correctness of basic array operations.
+
 ### 0.3.1
 
 * Include version constraint for `sparse`.
 
 ### 0.3.0
 
 * Introduce `conversion_cost()` to obtain a value roughly proportional to the conversion cost
```

### Comparing `sparseconverter-0.3.1/README.md` & `sparseconverter-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,21 @@
 
 * PyTorch arrays
 * SciPy sparse arrays as opposed to SciPy sparse matrices.
 * More detailed cost metric based on more real-world use cases and parameters.
 
 ## Changelog
 
+### 0.3.2
+
+* Detection and workaround for https://github.com/pydata/sparse/issues/602.
+* Detection and workaround for https://github.com/cupy/cupy/issues/7713.
+* Test with duplicates and scrambled indices.
+* Test correctness of basic array operations.
+
 ### 0.3.1
 
 * Include version constraint for `sparse`.
 
 ### 0.3.0
 
 * Introduce `conversion_cost()` to obtain a value roughly proportional to the conversion cost
```

### Comparing `sparseconverter-0.3.1/pyproject.toml` & `sparseconverter-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparseconverter-0.3.1/src/sparseconverter/__init__.py` & `sparseconverter-0.3.2/src/sparseconverter/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing_extensions import Literal
 
 import numpy as np
 import scipy.sparse as sp
 import sparse
 
 
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 NUMPY = 'numpy'
 NUMPY_MATRIX = 'numpy.matrix'
 CUDA = 'cuda'
 CUPY = 'cupy'
 SPARSE_COO = 'sparse.COO'
 SPARSE_GCXS = 'sparse.GCXS'
@@ -147,14 +147,48 @@
 
 # Exceptions for the above matrix
 _special_mappings = {
     (CUPY_SCIPY_CSR, np.dtype(bool)): bool,
 }
 
 
+def _test_GCXS_supports_non_canonical():
+    # Checks for https://github.com/pydata/sparse/issues/602
+    data = np.array((2., 1., 3., 3., 1.))
+    indices = np.array((1, 0, 0, 1, 1), dtype=int)
+    indptr = np.array((0, 2, 5), dtype=int)
+    ref = np.array(((1., 2.), (3., 4.)))
+
+    csr_check = sp.csr_matrix((data, indices, indptr), shape=(2, 2))
+    csr_works = (
+        np.all(csr_check[:1].todense() == ref[:1])
+        and np.all(csr_check[1:].todense() == ref[1:])
+    )
+    if not csr_works:
+        raise RuntimeError(
+            'scipy.sparse.csr_matrix gave unexpected result. '
+            'This is a bug, please report at https://github.com/LiberTEM/sparseconverter/!'
+        )
+    try:
+        gcxs_check = sparse.GCXS(csr_check)
+        gcxs_works = (
+            np.all(gcxs_check[:1].todense() == ref[:1])
+            and np.all(gcxs_check[1:].todense() == ref[1:])
+        )
+        return gcxs_works
+    # Maybe a first "bandaid" for GCXS is throwing an error? In that case we canonicalize
+    # the same way as if the bug was present.
+    except Exception:
+        raise  # FIXME remove
+        return False
+
+
+_GCXS_supports_non_canonical = _test_GCXS_supports_non_canonical()
+
+
 def result_type(*args) -> np.dtype:
     '''
     Find a dtype that fulfills the following properties:
 
     * Can contain :code:`numpy.result_type(...)` of all items in :code:`args`
       that are not a backend specifier.
     * Supported by all items in :code:`args` that are backend specifiers
@@ -232,14 +266,28 @@
     The return type of :meth:`sparse.GCXS.to_scipy_sparse`
     depends on the compressed axes.
     '''
     reshaped = arr.reshape((arr.shape[0], -1))
     return reshaped.to_scipy_sparse().asformat('csc')
 
 
+_CSR_CSC_T = Union[sp.csr_matrix, sp.csc_matrix]
+
+
+def _ensure_sorted_dedup(arr: _CSR_CSC_T) -> _CSR_CSC_T:
+    # Ensure we operate on a copy since sum_duplicates() is in_place
+    if arr.has_sorted_indices:
+        result = arr.copy()
+    else:
+        # Use the method that returns a copy
+        result = arr.sorted_indices()
+    result.sum_duplicates()
+    return result
+
+
 def chain(*functions: Converter) -> Converter:
     '''
     Create a function G(x) = f3(f2(f1(x)))
     from functions (f1, f2, f3)
     '''
     assert len(functions) >= 1
     return reduce(
@@ -268,15 +316,14 @@
                 for right in (NUMPY, CUDA):
                     self._converters[(left, right)] = _identity
             self._converters[(NUMPY, NUMPY_MATRIX)] = chain(_flatsig, np.asmatrix)
             self._converters[(NUMPY_MATRIX, NUMPY)] = np.asarray
             # Support direct construction from each other
             for left in (
                         NUMPY, CUDA, SPARSE_COO, SPARSE_GCXS, SPARSE_DOK,
-                        SCIPY_COO, SCIPY_CSR, SCIPY_CSC
                     ):
                 for right in SPARSE_COO, SPARSE_GCXS, SPARSE_DOK:
                     if (left, right) not in self._converters:
                         self._converters[(left, right)] = _classes[right]
             # Overwrite from before
             self._converters[(SPARSE_DOK, SPARSE_GCXS)] = partial(
                 sparse.DOK.asformat, format='gcxs'
@@ -293,18 +340,28 @@
                 for right in NUMPY, CUDA:
                     if (left, right) not in self._converters:
                         self._converters[(left, right)] = _classes[left].todense
             for left in SCIPY_COO, SCIPY_CSR, SCIPY_CSC:
                 for right in NUMPY, CUDA:
                     if (left, right) not in self._converters:
                         self._converters[(left, right)] = _classes[left].toarray
-            for left in SCIPY_COO, SCIPY_CSR, SCIPY_CSC:
+            for left in SCIPY_CSR, SCIPY_CSC:
+                for right in SPARSE_COO, SPARSE_GCXS, SPARSE_DOK:
+                    if (left, right) not in self._converters:
+                        if _GCXS_supports_non_canonical:
+                            self._converters[(left, right)] = _classes[right].from_scipy_sparse
+                        else:
+                            self._converters[(left, right)] = chain(
+                                _ensure_sorted_dedup, _classes[right].from_scipy_sparse
+                            )
+            for left in SCIPY_COO, :
                 for right in SPARSE_COO, SPARSE_GCXS, SPARSE_DOK:
                     if (left, right) not in self._converters:
                         self._converters[(left, right)] = _classes[right].from_scipy_sparse
+
             self._converters[(SPARSE_COO, SCIPY_COO)] = chain(_flatsig, sparse.COO.to_scipy_sparse)
             self._converters[(SPARSE_COO, SCIPY_CSR)] = chain(_flatsig, sparse.COO.tocsr)
             self._converters[(SPARSE_COO, SCIPY_CSC)] = chain(_flatsig, sparse.COO.tocsc)
             self._converters[(SPARSE_GCXS, SCIPY_COO)] = _GCXS_to_coo
             self._converters[(SPARSE_GCXS, SCIPY_CSR)] = _GCXS_to_csr
             self._converters[(SPARSE_GCXS, SCIPY_CSC)] = _GCXS_to_csc
 
@@ -365,16 +422,25 @@
                 "Please upgrade CuPy and/or CUDA: "
                 f"Constructing {CUPY_SCIPY_COO} from {CUPY} doesn't work (old CuPy version)"
                 "and installation is affected by this bug: "
                 "https://github.com/cupy/cupy/issues/7035 "
                 "(old cuSPARSE version)."
             )
 
+        def detect_bool_csr_bug():
+            data = cupy.array((True, True, True, False, True))
+            indices = cupy.array((0, 1, 0, 1, 1), dtype=int)
+            indptr = cupy.array((0, 2, 5), dtype=int)
+
+            c_csr = cupyx.scipy.sparse.csr_matrix((data, indices, indptr))
+            return not np.all(c_csr.todense())
+
         has_csr_complex128_bug = detect_csr_complex128_bug()
         has_cupy_coo_construction = detect_coo_works()
+        has_bool_csr_bug = detect_bool_csr_bug()
 
         CUPY_SPARSE_DTYPES = {
             np.float32, np.float64, np.complex64, np.complex128
         }
 
         CUPY_SPARSE_CSR_DTYPES = {
             np.dtype(bool), np.float32, np.float64, np.complex64, np.complex128
@@ -475,15 +541,19 @@
         def _CUPY_to_sparse_gcxs(arr: cupy.ndarray):
             '''
             Use GPU for sparsification if dtype allows, otherwise CPU
             '''
             if arr.dtype in CUPY_SPARSE_CSR_DTYPES:
                 reshaped = arr.reshape((arr.shape[0], -1))
                 intermediate = cupyx.scipy.sparse.csr_matrix(reshaped)
-                return sparse.GCXS(intermediate.get()).reshape(arr.shape)
+                intermediate = intermediate.get()
+                if not _GCXS_supports_non_canonical:
+                    intermediate.sort_indices()
+                    intermediate.sum_duplicates()
+                return sparse.GCXS(intermediate).reshape(arr.shape)
             else:
                 intermediate = cupy.asnumpy(arr)
                 return sparse.GCXS.from_numpy(intermediate)
 
         def _CUPY_to_sparse_dok(arr: cupy.ndarray):
             '''
             Use GPU for sparsification if dtype allows, otherwise CPU
@@ -593,14 +663,18 @@
                 return cupy.array(intermediate)
 
         def _scipy_csr_to_CUPY(arr: sp.csr_matrix):
             '''
             Use GPU for densification if dtype allows, otherwise CPU
             '''
             if arr.dtype in CUPY_SPARSE_CSR_DTYPES:
+                if arr.dtype == bool and has_bool_csr_bug:
+                    # Take copy since duplicates are summed in-place
+                    arr = arr.copy()
+                    arr.sum_duplicates()
                 intermediate = cupyx.scipy.sparse.csr_matrix(arr)
                 return intermediate.toarray()
             else:
                 intermediate = arr.toarray()
                 return cupy.array(intermediate)
 
         def _scipy_coo_to_CUPY(arr: sp.coo_matrix):
@@ -633,20 +707,33 @@
 
         def _cupy_scipy_csr_to_scipy_csc(arr: cupyx.scipy.sparse.csr_matrix):
             if arr.dtype in CUPY_SPARSE_DTYPES:
                 return cupyx.scipy.sparse.csc_matrix(arr).get()
             else:
                 return sp.csc_matrix(arr.get())
 
+        def _cupy_scipy_csr_to_CUPY(arr: cupyx.scipy.sparse.csr_matrix):
+            # Mitigation for https://github.com/cupy/cupy/issues/7713
+            if arr.dtype == bool and has_bool_csr_bug:
+                if not arr.has_canonical_format:
+                    # sum_duplicates() doesn't work for bool, so we deduplicate on the CPU
+                    cpu_arr = arr.get()
+                    cpu_arr.sum_duplicates()
+                    return cupyx.scipy.sparse.csr_matrix(cpu_arr).toarray()
+            # Fallthrough
+            return arr.toarray()
+
         self._converters[(NUMPY, CUPY)] = cupy.array
         self._converters[(CUDA, CUPY)] = cupy.array
         self._converters[(CUPY, NUMPY)] = cupy.asnumpy
         self._converters[(CUPY, CUDA)] = cupy.asnumpy
 
-        for left in CUPY_SCIPY_COO, CUPY_SCIPY_CSR, CUPY_SCIPY_CSC:
+        self._converters[(CUPY_SCIPY_CSR, CUPY)] = _cupy_scipy_csr_to_CUPY
+
+        for left in CUPY_SCIPY_COO, CUPY_SCIPY_CSC:
             if (left, CUPY) not in self._converters:
                 self._converters[(left, CUPY)] = _classes[left].toarray
 
         for (left, right) in [
                     (CUPY_SCIPY_COO, SCIPY_COO),
                     (CUPY_SCIPY_CSR, SCIPY_CSR),
                     (CUPY_SCIPY_CSC, SCIPY_CSC)
@@ -675,15 +762,14 @@
         self._converters[CUPY, CUPY_SCIPY_CSC] = _CUPY_to_cupy_scipy_csc
         for left in NUMPY, CUDA:
             for right in CUPY_SCIPY_COO, CUPY_SCIPY_CSR, CUPY_SCIPY_CSC:
                 if (left, right) not in self._converters:
                     c1 = self._converters[(left, CUPY)]
                     c2 = self._converters[(CUPY, right)]
                     self._converters[(left, right)] = chain(c1, c2)
-
         self._converters[(SPARSE_GCXS, CUPY_SCIPY_COO)] = chain(
             _adjust_dtype_cupy_sparse(CUPY_SCIPY_COO), _GCXS_to_cupy_coo
         )
         self._converters[(SPARSE_GCXS, CUPY_SCIPY_CSR)] = chain(
             _adjust_dtype_cupy_sparse(CUPY_SCIPY_CSR), _GCXS_to_cupy_csr
         )
         self._converters[(SPARSE_GCXS, CUPY_SCIPY_CSC)] = chain(
@@ -791,183 +877,183 @@
 
 _converters = _ConverterDict()
 # Measured with a run of benchmark_conversions on a "representative machine" aka my laptop
 # (32, 512, 512), np.float32, density 0.1
 # See scripts/benchmark.ipynb to generate this list
 # FIXME improve cost basis based on real use cases.
 _cost = {
-    (CUDA, CUDA): 9.52e-06,
-    (CUDA, CUPY): 0.0034923,
-    (CUDA, CUPY_SCIPY_COO): 0.02723361,
-    (CUDA, CUPY_SCIPY_CSC): 0.04614623,
-    (CUDA, CUPY_SCIPY_CSR): 0.03003148,
-    (CUDA, NUMPY): 1.158e-05,
-    (CUDA, NUMPY_MATRIX): 7.85e-05,
-    (CUDA, SCIPY_COO): 0.07095157,
-    (CUDA, SCIPY_CSC): 0.08312156,
-    (CUDA, SCIPY_CSR): 0.08185261,
-    (CUDA, SPARSE_COO): 0.05721102,
-    (CUDA, SPARSE_DOK): 0.47822719,
-    (CUDA, SPARSE_GCXS): 0.0926257,
-    (CUPY, CUDA): 0.04123289,
-    (CUPY, CUPY): 9.94e-06,
-    (CUPY, CUPY_SCIPY_COO): 0.02365191,
-    (CUPY, CUPY_SCIPY_CSC): 0.01339789,
-    (CUPY, CUPY_SCIPY_CSR): 0.02236629,
-    (CUPY, NUMPY): 0.04115815,
-    (CUPY, NUMPY_MATRIX): 0.04145609,
-    (CUPY, SCIPY_COO): 0.12031532,
-    (CUPY, SCIPY_CSC): 0.1171756,
-    (CUPY, SCIPY_CSR): 0.11456013,
-    (CUPY, SPARSE_COO): 0.1018334,
-    (CUPY, SPARSE_DOK): 0.52614732,
-    (CUPY, SPARSE_GCXS): 0.14133173,
-    (CUPY_SCIPY_COO, CUDA): 0.01391734,
-    (CUPY_SCIPY_COO, CUPY): 0.08673978,
-    (CUPY_SCIPY_COO, CUPY_SCIPY_COO): 9.15e-06,
-    (CUPY_SCIPY_COO, CUPY_SCIPY_CSC): 0.03534527,
-    (CUPY_SCIPY_COO, CUPY_SCIPY_CSR): 0.03556132,
-    (CUPY_SCIPY_COO, NUMPY): 0.01307202,
-    (CUPY_SCIPY_COO, NUMPY_MATRIX): 0.02308691,
-    (CUPY_SCIPY_COO, SCIPY_COO): 0.01752424,
-    (CUPY_SCIPY_COO, SCIPY_CSC): 0.04930567,
-    (CUPY_SCIPY_COO, SCIPY_CSR): 0.04840724,
-    (CUPY_SCIPY_COO, SPARSE_COO): 0.02267181,
-    (CUPY_SCIPY_COO, SPARSE_DOK): 0.81842092,
-    (CUPY_SCIPY_COO, SPARSE_GCXS): 0.04826163,
-    (CUPY_SCIPY_CSC, CUDA): 0.0168752,
-    (CUPY_SCIPY_CSC, CUPY): 0.04769173,
-    (CUPY_SCIPY_CSC, CUPY_SCIPY_COO): 0.02170808,
-    (CUPY_SCIPY_CSC, CUPY_SCIPY_CSC): 7.97e-06,
-    (CUPY_SCIPY_CSC, CUPY_SCIPY_CSR): 0.02813724,
-    (CUPY_SCIPY_CSC, NUMPY): 0.01218606,
-    (CUPY_SCIPY_CSC, NUMPY_MATRIX): 0.01833548,
-    (CUPY_SCIPY_CSC, SCIPY_COO): 0.01265958,
-    (CUPY_SCIPY_CSC, SCIPY_CSC): 0.00424232,
-    (CUPY_SCIPY_CSC, SCIPY_CSR): 0.02838422,
-    (CUPY_SCIPY_CSC, SPARSE_COO): 0.12949171,
-    (CUPY_SCIPY_CSC, SPARSE_DOK): 0.91622471,
-    (CUPY_SCIPY_CSC, SPARSE_GCXS): 0.01107186,
-    (CUPY_SCIPY_CSR, CUDA): 0.01544975,
-    (CUPY_SCIPY_CSR, CUPY): 0.04449919,
-    (CUPY_SCIPY_CSR, CUPY_SCIPY_COO): 0.01864054,
-    (CUPY_SCIPY_CSR, CUPY_SCIPY_CSC): 0.03305878,
-    (CUPY_SCIPY_CSR, CUPY_SCIPY_CSR): 9.44e-06,
-    (CUPY_SCIPY_CSR, NUMPY): 0.01093995,
-    (CUPY_SCIPY_CSR, NUMPY_MATRIX): 0.01565349,
-    (CUPY_SCIPY_CSR, SCIPY_COO): 0.0187434,
-    (CUPY_SCIPY_CSR, SCIPY_CSC): 0.01831002,
-    (CUPY_SCIPY_CSR, SCIPY_CSR): 0.00920348,
-    (CUPY_SCIPY_CSR, SPARSE_COO): 0.02926526,
-    (CUPY_SCIPY_CSR, SPARSE_DOK): 0.81829223,
-    (CUPY_SCIPY_CSR, SPARSE_GCXS): 0.00943145,
-    (NUMPY, CUDA): 8.96e-06,
-    (NUMPY, CUPY): 0.00304166,
-    (NUMPY, CUPY_SCIPY_COO): 0.03111887,
-    (NUMPY, CUPY_SCIPY_CSC): 0.03194446,
-    (NUMPY, CUPY_SCIPY_CSR): 0.02707654,
-    (NUMPY, NUMPY): 8.62e-06,
-    (NUMPY, NUMPY_MATRIX): 8.378e-05,
-    (NUMPY, SCIPY_COO): 0.07762542,
-    (NUMPY, SCIPY_CSC): 0.08492988,
-    (NUMPY, SCIPY_CSR): 0.07794126,
-    (NUMPY, SPARSE_COO): 0.05836581,
-    (NUMPY, SPARSE_DOK): 0.48218718,
-    (NUMPY, SPARSE_GCXS): 0.09733027,
-    (NUMPY_MATRIX, CUDA): 1.267e-05,
-    (NUMPY_MATRIX, CUPY): 0.00304186,
-    (NUMPY_MATRIX, CUPY_SCIPY_COO): 0.03103336,
-    (NUMPY_MATRIX, CUPY_SCIPY_CSC): 0.03340842,
-    (NUMPY_MATRIX, CUPY_SCIPY_CSR): 0.02498352,
-    (NUMPY_MATRIX, NUMPY): 1.266e-05,
-    (NUMPY_MATRIX, NUMPY_MATRIX): 9.09e-06,
-    (NUMPY_MATRIX, SCIPY_COO): 0.07374739,
-    (NUMPY_MATRIX, SCIPY_CSC): 0.08479951,
-    (NUMPY_MATRIX, SCIPY_CSR): 0.07748237,
-    (NUMPY_MATRIX, SPARSE_COO): 0.05546078,
-    (NUMPY_MATRIX, SPARSE_DOK): 0.42378837,
-    (NUMPY_MATRIX, SPARSE_GCXS): 0.08626198,
-    (SCIPY_COO, CUDA): 0.00558513,
-    (SCIPY_COO, CUPY): 0.01156896,
-    (SCIPY_COO, CUPY_SCIPY_COO): 0.02330746,
-    (SCIPY_COO, CUPY_SCIPY_CSC): 0.01858102,
-    (SCIPY_COO, CUPY_SCIPY_CSR): 0.01082556,
-    (SCIPY_COO, NUMPY): 0.00653755,
-    (SCIPY_COO, NUMPY_MATRIX): 0.00598033,
-    (SCIPY_COO, SCIPY_COO): 8.16e-06,
-    (SCIPY_COO, SCIPY_CSC): 0.01044739,
-    (SCIPY_COO, SCIPY_CSR): 0.00378696,
-    (SCIPY_COO, SPARSE_COO): 0.00141525,
-    (SCIPY_COO, SPARSE_DOK): 0.80436851,
-    (SCIPY_COO, SPARSE_GCXS): 0.00408728,
-    (SCIPY_CSC, CUDA): 0.00567477,
-    (SCIPY_CSC, CUPY): 0.01150378,
-    (SCIPY_CSC, CUPY_SCIPY_COO): 0.02839993,
-    (SCIPY_CSC, CUPY_SCIPY_CSC): 0.00359595,
-    (SCIPY_CSC, CUPY_SCIPY_CSR): 0.00917898,
-    (SCIPY_CSC, NUMPY): 0.00634705,
-    (SCIPY_CSC, NUMPY_MATRIX): 0.00548948,
-    (SCIPY_CSC, SCIPY_COO): 0.0104994,
-    (SCIPY_CSC, SCIPY_CSC): 8.02e-06,
-    (SCIPY_CSC, SCIPY_CSR): 0.00648227,
-    (SCIPY_CSC, SPARSE_COO): 0.12335432,
-    (SCIPY_CSC, SPARSE_DOK): 0.91889736,
-    (SCIPY_CSC, SPARSE_GCXS): 7.436e-05,
-    (SCIPY_CSR, CUDA): 0.00568018,
-    (SCIPY_CSR, CUPY): 0.0096229,
-    (SCIPY_CSR, CUPY_SCIPY_COO): 0.02727776,
-    (SCIPY_CSR, CUPY_SCIPY_CSC): 0.01258067,
-    (SCIPY_CSR, CUPY_SCIPY_CSR): 0.00259827,
-    (SCIPY_CSR, NUMPY): 0.00597631,
-    (SCIPY_CSR, NUMPY_MATRIX): 0.0056923,
-    (SCIPY_CSR, SCIPY_COO): 0.00909677,
-    (SCIPY_CSR, SCIPY_CSC): 0.01083296,
-    (SCIPY_CSR, SCIPY_CSR): 8.53e-06,
-    (SCIPY_CSR, SPARSE_COO): 0.01889156,
-    (SCIPY_CSR, SPARSE_DOK): 0.81050336,
-    (SCIPY_CSR, SPARSE_GCXS): 6.774e-05,
-    (SPARSE_COO, CUDA): 0.01559104,
-    (SPARSE_COO, CUPY): 0.02050667,
-    (SPARSE_COO, CUPY_SCIPY_COO): 0.04699705,
-    (SPARSE_COO, CUPY_SCIPY_CSC): 0.03912978,
-    (SPARSE_COO, CUPY_SCIPY_CSR): 0.03297643,
-    (SPARSE_COO, NUMPY): 0.01665228,
-    (SPARSE_COO, NUMPY_MATRIX): 0.01669986,
-    (SPARSE_COO, SCIPY_COO): 0.02236511,
-    (SPARSE_COO, SCIPY_CSC): 0.03321482,
-    (SPARSE_COO, SCIPY_CSR): 0.02309729,
-    (SPARSE_COO, SPARSE_COO): 9.63e-06,
-    (SPARSE_COO, SPARSE_DOK): 0.86456496,
-    (SPARSE_COO, SPARSE_GCXS): 0.03934677,
-    (SPARSE_DOK, CUDA): 0.11838129,
-    (SPARSE_DOK, CUPY): 0.12566395,
-    (SPARSE_DOK, CUPY_SCIPY_COO): 0.46361514,
-    (SPARSE_DOK, CUPY_SCIPY_CSC): 0.48294454,
-    (SPARSE_DOK, CUPY_SCIPY_CSR): 0.48472009,
-    (SPARSE_DOK, NUMPY): 0.12760996,
-    (SPARSE_DOK, NUMPY_MATRIX): 0.12691516,
-    (SPARSE_DOK, SCIPY_COO): 0.47121842,
-    (SPARSE_DOK, SCIPY_CSC): 0.45739357,
-    (SPARSE_DOK, SCIPY_CSR): 0.45030841,
-    (SPARSE_DOK, SPARSE_COO): 0.43964837,
-    (SPARSE_DOK, SPARSE_DOK): 8.7e-06,
-    (SPARSE_DOK, SPARSE_GCXS): 0.4815116,
-    (SPARSE_GCXS, CUDA): 0.05721252,
-    (SPARSE_GCXS, CUPY): 0.05968288,
-    (SPARSE_GCXS, CUPY_SCIPY_COO): 0.54629951,
-    (SPARSE_GCXS, CUPY_SCIPY_CSC): 0.51329979,
-    (SPARSE_GCXS, CUPY_SCIPY_CSR): 0.51411286,
-    (SPARSE_GCXS, NUMPY): 0.05773925,
-    (SPARSE_GCXS, NUMPY_MATRIX): 0.05410605,
-    (SPARSE_GCXS, SCIPY_COO): 0.44208745,
-    (SPARSE_GCXS, SCIPY_CSC): 0.43770924,
-    (SPARSE_GCXS, SCIPY_CSR): 0.43229283,
-    (SPARSE_GCXS, SPARSE_COO): 0.03560626,
-    (SPARSE_GCXS, SPARSE_DOK): 0.88085017,
-    (SPARSE_GCXS, SPARSE_GCXS): 2.003e-05,
+    (CUDA, CUDA): 1.397e-05,
+    (CUDA, CUPY): 0.00290094,
+    (CUDA, CUPY_SCIPY_COO): 0.03676262,
+    (CUDA, CUPY_SCIPY_CSC): 0.02478382,
+    (CUDA, CUPY_SCIPY_CSR): 0.03029807,
+    (CUDA, NUMPY): 1.101e-05,
+    (CUDA, NUMPY_MATRIX): 0.00014465,
+    (CUDA, SCIPY_COO): 0.07126909,
+    (CUDA, SCIPY_CSC): 0.07710105,
+    (CUDA, SCIPY_CSR): 0.07387733,
+    (CUDA, SPARSE_COO): 0.06164377,
+    (CUDA, SPARSE_DOK): 0.41626783,
+    (CUDA, SPARSE_GCXS): 0.08713908,
+    (CUPY, CUDA): 0.04128729,
+    (CUPY, CUPY): 1.315e-05,
+    (CUPY, CUPY_SCIPY_COO): 0.03479637,
+    (CUPY, CUPY_SCIPY_CSC): 0.02891527,
+    (CUPY, CUPY_SCIPY_CSR): 0.02077345,
+    (CUPY, NUMPY): 0.04131443,
+    (CUPY, NUMPY_MATRIX): 0.04139519,
+    (CUPY, SCIPY_COO): 0.11484382,
+    (CUPY, SCIPY_CSC): 0.12240084,
+    (CUPY, SCIPY_CSR): 0.11560138,
+    (CUPY, SPARSE_COO): 0.08293617,
+    (CUPY, SPARSE_DOK): 0.45851607,
+    (CUPY, SPARSE_GCXS): 0.13566548,
+    (CUPY_SCIPY_COO, CUDA): 0.01279124,
+    (CUPY_SCIPY_COO, CUPY): 0.08431704,
+    (CUPY_SCIPY_COO, CUPY_SCIPY_COO): 9.8e-06,
+    (CUPY_SCIPY_COO, CUPY_SCIPY_CSC): 0.03095062,
+    (CUPY_SCIPY_COO, CUPY_SCIPY_CSR): 0.03350027,
+    (CUPY_SCIPY_COO, NUMPY): 0.01959753,
+    (CUPY_SCIPY_COO, NUMPY_MATRIX): 0.01955723,
+    (CUPY_SCIPY_COO, SCIPY_COO): 0.0140366,
+    (CUPY_SCIPY_COO, SCIPY_CSC): 0.05566742,
+    (CUPY_SCIPY_COO, SCIPY_CSR): 0.04540595,
+    (CUPY_SCIPY_COO, SPARSE_COO): 0.02240446,
+    (CUPY_SCIPY_COO, SPARSE_DOK): 0.81763242,
+    (CUPY_SCIPY_COO, SPARSE_GCXS): 0.0503551,
+    (CUPY_SCIPY_CSC, CUDA): 0.01170401,
+    (CUPY_SCIPY_CSC, CUPY): 0.04833271,
+    (CUPY_SCIPY_CSC, CUPY_SCIPY_COO): 0.0154935,
+    (CUPY_SCIPY_CSC, CUPY_SCIPY_CSC): 1.079e-05,
+    (CUPY_SCIPY_CSC, CUPY_SCIPY_CSR): 0.01317206,
+    (CUPY_SCIPY_CSC, NUMPY): 0.01652527,
+    (CUPY_SCIPY_CSC, NUMPY_MATRIX): 0.01623056,
+    (CUPY_SCIPY_CSC, SCIPY_COO): 0.03094247,
+    (CUPY_SCIPY_CSC, SCIPY_CSC): 0.00378959,
+    (CUPY_SCIPY_CSC, SCIPY_CSR): 0.04601307,
+    (CUPY_SCIPY_CSC, SPARSE_COO): 0.09272055,
+    (CUPY_SCIPY_CSC, SPARSE_DOK): 0.87353325,
+    (CUPY_SCIPY_CSC, SPARSE_GCXS): 0.01177203,
+    (CUPY_SCIPY_CSR, CUDA): 0.01429861,
+    (CUPY_SCIPY_CSR, CUPY): 0.04460615,
+    (CUPY_SCIPY_CSR, CUPY_SCIPY_COO): 0.01443459,
+    (CUPY_SCIPY_CSR, CUPY_SCIPY_CSC): 0.002124,
+    (CUPY_SCIPY_CSR, CUPY_SCIPY_CSR): 1.167e-05,
+    (CUPY_SCIPY_CSR, NUMPY): 0.01489683,
+    (CUPY_SCIPY_CSR, NUMPY_MATRIX): 0.01469383,
+    (CUPY_SCIPY_CSR, SCIPY_COO): 0.01336538,
+    (CUPY_SCIPY_CSR, SCIPY_CSC): 0.0139769,
+    (CUPY_SCIPY_CSR, SCIPY_CSR): 0.00912916,
+    (CUPY_SCIPY_CSR, SPARSE_COO): 0.02864303,
+    (CUPY_SCIPY_CSR, SPARSE_DOK): 0.80137306,
+    (CUPY_SCIPY_CSR, SPARSE_GCXS): 0.00764849,
+    (NUMPY, CUDA): 1.228e-05,
+    (NUMPY, CUPY): 0.00275125,
+    (NUMPY, CUPY_SCIPY_COO): 0.03072501,
+    (NUMPY, CUPY_SCIPY_CSC): 0.03698203,
+    (NUMPY, CUPY_SCIPY_CSR): 0.02565548,
+    (NUMPY, NUMPY): 2.177e-05,
+    (NUMPY, NUMPY_MATRIX): 0.00011643,
+    (NUMPY, SCIPY_COO): 0.071367,
+    (NUMPY, SCIPY_CSC): 0.08173664,
+    (NUMPY, SCIPY_CSR): 0.07519809,
+    (NUMPY, SPARSE_COO): 0.06172041,
+    (NUMPY, SPARSE_DOK): 0.41673362,
+    (NUMPY, SPARSE_GCXS): 0.08833201,
+    (NUMPY_MATRIX, CUDA): 1.812e-05,
+    (NUMPY_MATRIX, CUPY): 0.00284773,
+    (NUMPY_MATRIX, CUPY_SCIPY_COO): 0.02692905,
+    (NUMPY_MATRIX, CUPY_SCIPY_CSC): 0.0248778,
+    (NUMPY_MATRIX, CUPY_SCIPY_CSR): 0.02930477,
+    (NUMPY_MATRIX, NUMPY): 3.088e-05,
+    (NUMPY_MATRIX, NUMPY_MATRIX): 1.357e-05,
+    (NUMPY_MATRIX, SCIPY_COO): 0.07221178,
+    (NUMPY_MATRIX, SCIPY_CSC): 0.08215391,
+    (NUMPY_MATRIX, SCIPY_CSR): 0.07470251,
+    (NUMPY_MATRIX, SPARSE_COO): 0.05499004,
+    (NUMPY_MATRIX, SPARSE_DOK): 0.36448452,
+    (NUMPY_MATRIX, SPARSE_GCXS): 0.07961737,
+    (SCIPY_COO, CUDA): 0.00554266,
+    (SCIPY_COO, CUPY): 0.01049599,
+    (SCIPY_COO, CUPY_SCIPY_COO): 0.02096826,
+    (SCIPY_COO, CUPY_SCIPY_CSC): 0.01695301,
+    (SCIPY_COO, CUPY_SCIPY_CSR): 0.00833004,
+    (SCIPY_COO, NUMPY): 0.0057289,
+    (SCIPY_COO, NUMPY_MATRIX): 0.00514385,
+    (SCIPY_COO, SCIPY_COO): 1.483e-05,
+    (SCIPY_COO, SCIPY_CSC): 0.00908695,
+    (SCIPY_COO, SCIPY_CSR): 0.00409992,
+    (SCIPY_COO, SPARSE_COO): 0.0015528,
+    (SCIPY_COO, SPARSE_DOK): 0.76291548,
+    (SCIPY_COO, SPARSE_GCXS): 0.00415204,
+    (SCIPY_CSC, CUDA): 0.00534249,
+    (SCIPY_CSC, CUPY): 0.01051322,
+    (SCIPY_CSC, CUPY_SCIPY_COO): 0.02545826,
+    (SCIPY_CSC, CUPY_SCIPY_CSC): 0.00291492,
+    (SCIPY_CSC, CUPY_SCIPY_CSR): 0.00827505,
+    (SCIPY_CSC, NUMPY): 0.00567323,
+    (SCIPY_CSC, NUMPY_MATRIX): 0.00572489,
+    (SCIPY_CSC, SCIPY_COO): 0.00559732,
+    (SCIPY_CSC, SCIPY_CSC): 1.329e-05,
+    (SCIPY_CSC, SCIPY_CSR): 0.00556892,
+    (SCIPY_CSC, SPARSE_COO): 0.07105924,
+    (SCIPY_CSC, SPARSE_DOK): 0.82178102,
+    (SCIPY_CSC, SPARSE_GCXS): 0.00404301,
+    (SCIPY_CSR, CUDA): 0.00493635,
+    (SCIPY_CSR, CUPY): 0.01012645,
+    (SCIPY_CSR, CUPY_SCIPY_COO): 0.02334584,
+    (SCIPY_CSR, CUPY_SCIPY_CSC): 0.01313419,
+    (SCIPY_CSR, CUPY_SCIPY_CSR): 0.00245257,
+    (SCIPY_CSR, NUMPY): 0.00552472,
+    (SCIPY_CSR, NUMPY_MATRIX): 0.00569328,
+    (SCIPY_CSR, SCIPY_COO): 0.00398569,
+    (SCIPY_CSR, SCIPY_CSC): 0.00942009,
+    (SCIPY_CSR, SCIPY_CSR): 1.459e-05,
+    (SCIPY_CSR, SPARSE_COO): 0.01763324,
+    (SCIPY_CSR, SPARSE_DOK): 0.83002728,
+    (SCIPY_CSR, SPARSE_GCXS): 0.00215682,
+    (SPARSE_COO, CUDA): 0.01227037,
+    (SPARSE_COO, CUPY): 0.01397232,
+    (SPARSE_COO, CUPY_SCIPY_COO): 0.03187509,
+    (SPARSE_COO, CUPY_SCIPY_CSC): 0.03986542,
+    (SPARSE_COO, CUPY_SCIPY_CSR): 0.02893439,
+    (SPARSE_COO, NUMPY): 0.0098226,
+    (SPARSE_COO, NUMPY_MATRIX): 0.01040078,
+    (SPARSE_COO, SCIPY_COO): 0.02069974,
+    (SPARSE_COO, SCIPY_CSC): 0.03106024,
+    (SPARSE_COO, SCIPY_CSR): 0.02506089,
+    (SPARSE_COO, SPARSE_COO): 1.328e-05,
+    (SPARSE_COO, SPARSE_DOK): 0.83920339,
+    (SPARSE_COO, SPARSE_GCXS): 0.03594461,
+    (SPARSE_DOK, CUDA): 0.11058626,
+    (SPARSE_DOK, CUPY): 0.10950506,
+    (SPARSE_DOK, CUPY_SCIPY_COO): 0.44371138,
+    (SPARSE_DOK, CUPY_SCIPY_CSC): 0.4265934,
+    (SPARSE_DOK, CUPY_SCIPY_CSR): 0.43226047,
+    (SPARSE_DOK, NUMPY): 0.11354399,
+    (SPARSE_DOK, NUMPY_MATRIX): 0.10729896,
+    (SPARSE_DOK, SCIPY_COO): 0.42308864,
+    (SPARSE_DOK, SCIPY_CSC): 0.45172044,
+    (SPARSE_DOK, SCIPY_CSR): 0.42915226,
+    (SPARSE_DOK, SPARSE_COO): 0.41190378,
+    (SPARSE_DOK, SPARSE_DOK): 1.187e-05,
+    (SPARSE_DOK, SPARSE_GCXS): 0.4325561,
+    (SPARSE_GCXS, CUDA): 0.05120677,
+    (SPARSE_GCXS, CUPY): 0.05303882,
+    (SPARSE_GCXS, CUPY_SCIPY_COO): 0.47022746,
+    (SPARSE_GCXS, CUPY_SCIPY_CSC): 0.45507096,
+    (SPARSE_GCXS, CUPY_SCIPY_CSR): 0.44203396,
+    (SPARSE_GCXS, NUMPY): 0.04957471,
+    (SPARSE_GCXS, NUMPY_MATRIX): 0.04963172,
+    (SPARSE_GCXS, SCIPY_COO): 0.36567051,
+    (SPARSE_GCXS, SCIPY_CSC): 0.34491236,
+    (SPARSE_GCXS, SCIPY_CSR): 0.32723106,
+    (SPARSE_GCXS, SPARSE_COO): 0.03921757,
+    (SPARSE_GCXS, SPARSE_DOK): 0.87211339,
+    (SPARSE_GCXS, SPARSE_GCXS): 1.298e-05,
 }
 
 # In order to support subclasses and not check all formats each time
 # we cache dynamically which type maps to which format code
 _type_cache: Dict[type, Optional[ArrayBackend]] = {}
```

### Comparing `sparseconverter-0.3.1/src/sparseconverter.egg-info/PKG-INFO` & `sparseconverter-0.3.2/src/sparseconverter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseconverter
-Version: 0.3.1
+Version: 0.3.2
 Summary: Converter matrix and type determination for a range of array formats, focusing on sparse arrays
 Author-email: Dieter Weber <d.weber@fz-juelich.de>
 License: MIT License
         
         Copyright (c) 2022 LiberTEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -113,14 +113,21 @@
 
 * PyTorch arrays
 * SciPy sparse arrays as opposed to SciPy sparse matrices.
 * More detailed cost metric based on more real-world use cases and parameters.
 
 ## Changelog
 
+### 0.3.2
+
+* Detection and workaround for https://github.com/pydata/sparse/issues/602.
+* Detection and workaround for https://github.com/cupy/cupy/issues/7713.
+* Test with duplicates and scrambled indices.
+* Test correctness of basic array operations.
+
 ### 0.3.1
 
 * Include version constraint for `sparse`.
 
 ### 0.3.0
 
 * Introduce `conversion_cost()` to obtain a value roughly proportional to the conversion cost
```

