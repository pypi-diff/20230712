# Comparing `tmp/pyqtorch-0.3.1.tar.gz` & `tmp/pyqtorch-0.3.2.tar.gz`

## Comparing `pyqtorch-0.3.1.tar` & `pyqtorch-0.3.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/README.md
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/mkdocs.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/.github/workflows/run-tests-and-mypy.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/QAOA.ipynb
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/circuit.md
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/essentials.ipynb
--rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/fit_function.ipynb
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/gate_composition.ipynb
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/hamevo.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/index.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/matrices.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/parametric.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/primitive.md
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/getting_started.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/embedding.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    22858 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/abstract.py
--rw-r--r--   0        0        0     9728 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0    12266 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_converters.py
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_module_hamevo.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_modules.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/LICENSE
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/README.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/mkdocs.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/.github/workflows/run-tests-and-mypy.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/QAOA.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/circuit.md
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/essentials.ipynb
+-rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/fit_function.ipynb
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/gate_composition.ipynb
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/hamevo.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/matrices.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/parametric.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/primitive.md
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/getting_started.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    23548 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/abstract.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_converters.py
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_modules.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/PKG-INFO
```

### Comparing `pyqtorch-0.3.1/.pre-commit-config.yaml` & `pyqtorch-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/CODE_OF_CONDUCT.md` & `pyqtorch-0.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/CONTRIBUTING.md` & `pyqtorch-0.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/mkdocs.yml` & `pyqtorch-0.3.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.3.2/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/QAOA.ipynb` & `pyqtorch-0.3.2/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/essentials.ipynb` & `pyqtorch-0.3.2/docs/essentials.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/fit_function.ipynb` & `pyqtorch-0.3.2/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/gate_composition.ipynb` & `pyqtorch-0.3.2/docs/gate_composition.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/hamevo.md` & `pyqtorch-0.3.2/docs/hamevo.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.3.2/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/deprecated/bench.py` & `pyqtorch-0.3.2/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.3.2/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/deprecated/getting_started.ipynb` & `pyqtorch-0.3.2/docs/deprecated/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.3.2/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.3.2/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/__init__.py` & `pyqtorch-0.3.2/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/ansatz.py` & `pyqtorch-0.3.2/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/embedding.py` & `pyqtorch-0.3.2/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/matrices.py` & `pyqtorch-0.3.2/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/matrices_sparse.py` & `pyqtorch-0.3.2/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/converters/store_ops.py` & `pyqtorch-0.3.2/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.3.2/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/core/__init__.py` & `pyqtorch-0.3.2/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/core/batched_operation.py` & `pyqtorch-0.3.2/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/core/circuit.py` & `pyqtorch-0.3.2/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/core/measurement.py` & `pyqtorch-0.3.2/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/core/operation.py` & `pyqtorch-0.3.2/pyqtorch/core/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,17 @@
 
         operation_matrix (torch.Tensor): the type of operation which should be performed (RX,RY,RZ)
 
     Returns:
 
         torch.Tensor: the resulting controlled gate populated by operation_matrix
     """
-    controlled_mat: torch.Tensor = torch.eye(4, dtype=torch.cdouble)
-    controlled_mat[2:, 2:] = operation_matrix
+    mat_size = len(operation_matrix)
+    controlled_mat: torch.Tensor = torch.eye(2 * mat_size, dtype=torch.cdouble)
+    controlled_mat[-mat_size:, -mat_size:] = operation_matrix
     return controlled_mat
 
 
 def RX(theta: torch.Tensor, state: torch.Tensor, qubits: ArrayLike, N_qubits: int) -> torch.Tensor:
     """Parametrized single-qubit RX rotation
 
     Args:
@@ -495,14 +496,33 @@
             [0, 0, 0, torch.exp(torch.tensor(1j * theta))],
         ],
         dtype=torch.cdouble,
     ).to(dev)
     return _apply_gate(state, mat, qubits, N_qubits)
 
 
+def CSWAP(state: torch.Tensor, qubits: ArrayLike, N_qubits: int) -> torch.Tensor:
+    """Controlled SWAP gate with three-qubit support
+
+    Args:
+        state (torch.Tensor): the input quantum state, of shape `(N_0, N_1,..., N_N, batch_size)`
+        qubits (ArrayLike): list of qubit indices where the gate will operate
+        N_qubits (int): the number of qubits in the system
+
+    Returns:
+
+        torch.Tensor: the resulting state after applying the gate
+    """
+
+    if ops_cache.enabled:
+        store_operation("CSWAP", qubits)
+
+    return ControlledOperationGate(state, qubits, N_qubits, OPERATIONS_DICT["SWAP"])
+
+
 def hamiltonian_evolution(
     H: torch.Tensor,
     state: torch.Tensor,
     t: torch.Tensor,
     qubits: Any,
     N_qubits: int,
     n_steps: int = 100,
```

### Comparing `pyqtorch-0.3.1/pyqtorch/core/utils.py` & `pyqtorch-0.3.2/pyqtorch/core/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,27 +31,41 @@
 ZMAT = torch.tensor([[1, 0], [0, -1]], dtype=torch.cdouble)
 SMAT = torch.tensor([[1, 0], [0, 1j]], dtype=torch.cdouble)
 SDAGGERMAT = torch.tensor([[1, 0], [0, -1j]], dtype=torch.cdouble)
 TMAT = torch.tensor([[1, 0], [0, torch.exp(torch.tensor(1.0j * torch.pi / 4))]])
 SWAPMAT = torch.tensor(
     [[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]], dtype=torch.cdouble
 )
+CSWAPMAT = torch.tensor(
+    [
+        [1, 0, 0, 0, 0, 0, 0, 0],
+        [0, 1, 0, 0, 0, 0, 0, 0],
+        [0, 0, 1, 0, 0, 0, 0, 0],
+        [0, 0, 0, 1, 0, 0, 0, 0],
+        [0, 0, 0, 0, 1, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 1, 0],
+        [0, 0, 0, 0, 0, 1, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 1],
+    ],
+    dtype=torch.cdouble,
+)
 HMAT = 1 / torch.sqrt(torch.tensor(2)) * torch.tensor([[1, 1], [1, -1]], dtype=torch.cdouble)
 
 
 OPERATIONS_DICT = {
     "I": IMAT,
     "X": XMAT,
     "Y": YMAT,
     "Z": ZMAT,
     "S": SMAT,
     "SDAGGER": SDAGGERMAT,
     "T": TMAT,
     "H": HMAT,
     "SWAP": SWAPMAT,
+    "CSWAP": CSWAPMAT,
 }
 
 
 def _apply_gate(
     state: torch.Tensor,
     mat: torch.Tensor,
     qubits: Any,
```

### Comparing `pyqtorch-0.3.1/pyqtorch/modules/abstract.py` & `pyqtorch-0.3.2/pyqtorch/modules/abstract.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/modules/circuit.py` & `pyqtorch-0.3.2/pyqtorch/modules/circuit.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,95 +3,19 @@
 from typing import Any
 
 import torch
 from torch.nn import Module, ModuleList, Parameter, init
 
 from pyqtorch.modules.abstract import AbstractGate
 from pyqtorch.modules.primitive import CNOT
+from pyqtorch.modules.utils import zero_state
 
 PI = 2.0 * torch.asin(torch.Tensor([1.0]).double()).item()
 
 
-def zero_state(
-    n_qubits: int,
-    batch_size: int = 1,
-    device: str | torch.device = "cpu",
-    dtype: torch.dtype = torch.cdouble,
-) -> torch.Tensor:
-    """
-    Generates the zero state for a specified number of qubits.
-
-    Arguments:
-        n_qubits (int): The number of qubits for which the zero state is to be generated.
-        batch_size (int): The batch size for the zero state.
-        device (str): The device on which the zero state tensor is to be allocated eg cpu or gpu.
-        dtype (torch.cdouble): The data type of the zero state tensor.
-
-    Returns:
-        torch.Tensor: A tensor representing the zero state.
-        The shape of the tensor is (batch_size, 2^n_qubits),
-        where 2^n_qubits is the total number of possible states for the given number of qubits.
-        The data type of the tensor is specified by the dtype parameter.
-
-    Examples:
-    ```python exec="on" source="above" result="json"
-    import torch
-    import pyqtorch.modules as pyq
-
-    state = pyq.zero_state(n_qubits=2)
-    print(state)  #tensor([[[1.+0.j],[0.+0.j]],[[0.+0.j],[0.+0.j]]], dtype=torch.complex128)
-    ```
-    """
-    state = torch.zeros((2**n_qubits, batch_size), dtype=dtype, device=device)
-    state[0] = 1
-    state = state.reshape([2] * n_qubits + [batch_size])
-    return state
-
-
-def uniform_state(
-    n_qubits: int,
-    batch_size: int = 1,
-    device: str | torch.device = "cpu",
-    dtype: torch.dtype = torch.cdouble,
-) -> torch.Tensor:
-    """
-    Generates the uniform state for a specified number of qubits.
-    Returns a tensor representing the uniform state.
-    The shape of the tensor is (2^n_qubits, batch_size),
-    where 2^n_qubits is the total number of possible states for the given number of qubits.
-    The data type of the tensor is specified by the dtype parameter.
-    Each element of the tensor is initialized to 1/sqrt(2^n_qubits),
-    ensuring that the total probability of the state is equal to 1.
-
-    Arguments:
-        n_qubits (int): The number of qubits for which the uniform state is to be generated.
-        batch_size (int): The batch size for the uniform state.
-        device (str): The device on which the uniform state tensor is to be allocated.
-        dtype (torch.cdouble): The data type of the uniform state tensor.
-
-    Returns:
-        torch.Tensor: A tensor representing the uniform state.
-
-
-    Examples:
-    ```python exec="on" source="above" result="json"
-    import torch
-    import pyqtorch.modules as pyq
-
-    state = pyq.uniform_state(n_qubits=2)
-    print(state)
-    #tensor([[[0.5000+0.j],[0.5000+0.j]],[[0.5000+0.j],[0.5000+0.j]]], dtype=torch.complex128)
-    ```
-    """
-    state = torch.ones((2**n_qubits, batch_size), dtype=dtype, device=device)
-    state = state / torch.sqrt(torch.tensor(2**n_qubits))
-    state = state.reshape([2] * n_qubits + [batch_size])
-    return state
-
-
 class QuantumCircuit(Module):
     def __init__(self, n_qubits: int, operations: list):
         """
         Creates a QuantumCircuit that can be used to compose multiple gates
         from a list of operations.
 
         Arguments:
```

### Comparing `pyqtorch-0.3.1/pyqtorch/modules/hamevo.py` & `pyqtorch-0.3.2/pyqtorch/modules/hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/modules/parametric.py` & `pyqtorch-0.3.2/pyqtorch/modules/parametric.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyqtorch/modules/primitive.py` & `pyqtorch-0.3.2/pyqtorch/modules/primitive.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,7 +393,37 @@
 
         # Apply the CZ gate to the zero state
         result = cz_gate(z_state)
         print(result)
         ```
         """
         super().__init__("Z", qubits, n_qubits)
+
+
+class CSWAP(ControlledOperationGate):
+    def __init__(self, qubits: ArrayLike, n_qubits: int):
+        """
+        Represents a controlled-SWAP (CSWAP) gate in a quantum circuit.
+        The CSWAP gate class creates a controlled SWAP gate, applying
+        the SWAP gate according to the control qubit state.
+
+
+        Arguments:
+            qubits (ArrayLike): The control and targets qubits for the CSWAP gate.
+            n_qubits (int): The total number of qubits in the circuit.
+
+        Examples:
+        ```python exec="on" source="above" result="json"
+        import torch
+        import pyqtorch.modules as pyq
+
+        # Create a CSWAP gate
+        cswap_gate = pyq.CSWAP(qubits=[0, 1, 2], n_qubits=3)
+
+        # Create a zero state
+        swap_state = pyq.zero_state(n_qubits=3)
+
+        # Apply the CSWAP gate to the zero state
+        result = cswap_gate(swap_state)
+        print(result)
+        """
+        super().__init__("SWAP", qubits, n_qubits)
```

### Comparing `pyqtorch-0.3.1/tests/conftest.py` & `pyqtorch-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/tests/test_batched_operations.py` & `pyqtorch-0.3.2/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/tests/test_converters.py` & `pyqtorch-0.3.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/tests/test_module_hamevo.py` & `pyqtorch-0.3.2/tests/test_module_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/tests/test_modules.py` & `pyqtorch-0.3.2/tests/test_modules.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 from __future__ import annotations
 
+from typing import Callable
+
 import pytest
 import torch
 
 import pyqtorch.core as func_pyq
 import pyqtorch.modules as pyq
 from pyqtorch.modules.abstract import AbstractGate
 
+state_000 = pyq.zero_state(3, device="cpu", dtype=torch.cdouble)
+state_001 = pyq.X(qubits=[2], n_qubits=3)(state_000)
+state_100 = pyq.X(qubits=[0], n_qubits=3)(state_000)
+state_101 = pyq.X(qubits=[2], n_qubits=3)(pyq.X(qubits=[0], n_qubits=3)(state_000))
+state_110 = pyq.X(qubits=[1], n_qubits=3)(pyq.X(qubits=[0], n_qubits=3)(state_000))
+
 
 @pytest.mark.parametrize("gate", ["X", "Y", "Z", "H", "I", "S", "T", "Sdagger"])
 def test_constant_gates(gate: str) -> None:
     dtype = torch.cdouble
     device = "cpu"
     batch_size = 100
     qubits = [0]
@@ -185,7 +193,65 @@
     assert circ == truth
 
     circ = pyq.QuantumCircuit(1, [pyq.X([0], 1), pyq.Y([0], 1)]) * pyq.QuantumCircuit(
         n_qubits, [rx, pyq.RY([0], 1)]
     )
     truth = pyq.QuantumCircuit(n_qubits, [pyq.X([0], 1), pyq.Y([0], 1), rx, pyq.RY([0], 1)])
     assert circ == truth
+
+
+def test_CSWAP_state000_controlqubit_0() -> None:
+    n_qubits = 3
+    cswap = pyq.CSWAP([0, 1, 2], n_qubits)
+    assert torch.allclose(cswap(state_000), state_000)
+
+
+def test_CSWAP_state001_controlqubit_0() -> None:
+    n_qubits = 3
+    cswap = pyq.CSWAP([0, 1, 2], n_qubits)
+    assert torch.allclose(cswap(state_001), state_001)
+
+
+def test_CSWAP_state100_controlqubit_0() -> None:
+    n_qubits = 3
+    cswap = pyq.CSWAP([0, 1, 2], n_qubits)
+    assert torch.allclose(cswap(state_100), state_100)
+
+
+def test_CSWAP_state101_controlqubit_0() -> None:
+    n_qubits = 3
+    cswap = pyq.CSWAP([0, 1, 2], n_qubits)
+    assert torch.allclose(cswap(state_101), state_110)
+
+
+def test_CSWAP_state110_controlqubit_0() -> None:
+    n_qubits = 3
+    cswap = pyq.CSWAP([0, 1, 2], n_qubits)
+    assert torch.allclose(cswap(state_110), state_101)
+
+
+@pytest.mark.parametrize("state_fn", [pyq.random_state, pyq.zero_state, pyq.uniform_state])
+@pytest.mark.parametrize("n_qubits", [i for i in range(1, 8)])
+@pytest.mark.parametrize("batch_size", [i for i in range(1, 8)])
+def test_isnormalized_states(state_fn: Callable, n_qubits: int, batch_size: int) -> None:
+    state = state_fn(n_qubits, batch_size)
+    assert pyq.is_normalized(state)
+
+
+@pytest.mark.parametrize("n_qubits", [i for i in range(1, 8)])
+@pytest.mark.parametrize("batch_size", [i for i in range(1, 8)])
+def test_state_shapes(n_qubits: int, batch_size: int) -> None:
+    zero = pyq.zero_state(n_qubits, batch_size)
+    uni = pyq.uniform_state(n_qubits, batch_size)
+    rand = pyq.random_state(n_qubits, batch_size)
+    assert zero.shape == rand.shape and uni.shape == rand.shape
+
+
+@pytest.mark.parametrize("state_fn", [pyq.random_state, pyq.zero_state, pyq.uniform_state])
+@pytest.mark.parametrize("n_qubits", [i for i in range(1, 8)])
+@pytest.mark.parametrize("batch_size", [i for i in range(1, 8)])
+def test_overlap_states_batch_nqubits(state_fn: Callable, n_qubits: int, batch_size: int) -> None:
+    state = state_fn(n_qubits, batch_size)
+    assert torch.allclose(
+        pyq.overlap(state, state),
+        torch.ones(batch_size),
+    )
```

### Comparing `pyqtorch-0.3.1/tests/test_notebooks.py` & `pyqtorch-0.3.2/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/tests/test_operations.py` & `pyqtorch-0.3.2/tests/test_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import random
 
 import numpy as np
 import torch
 from torch.autograd import grad
 
+from pyqtorch.modules import X, zero_state
+
 random.seed(0)
 np.random.seed(0)
 torch.manual_seed(0)
 torch.use_deterministic_algorithms(not torch.cuda.is_available())
 
 from conftest import TestBatchedFM, TestFM, TestNetwork  # noqa: E402
 
@@ -20,14 +22,20 @@
 state_1 = torch.tensor([[0, 1]], dtype=torch.cdouble)
 
 state_00 = torch.tensor([[1, 0], [0, 0]], dtype=torch.cdouble).unsqueeze(2)
 state_10 = torch.tensor([[0, 1], [0, 0]], dtype=torch.cdouble).unsqueeze(2)
 state_01 = torch.tensor([[0, 0], [1, 0]], dtype=torch.cdouble).unsqueeze(2)
 state_11 = torch.tensor([[0, 0], [0, 1]], dtype=torch.cdouble).unsqueeze(2)
 
+state_000 = zero_state(3)
+state_001 = X(qubits=[2], n_qubits=3)(zero_state(3))
+state_100 = X(qubits=[0], n_qubits=3)(zero_state(3))
+state_101 = X(qubits=[2], n_qubits=3)(X(qubits=[0], n_qubits=3)(zero_state(3)))
+state_110 = X(qubits=[1], n_qubits=3)(X(qubits=[0], n_qubits=3)(zero_state(3)))
+
 pi = torch.tensor(torch.pi, dtype=torch.cdouble)
 
 CNOT_mat: torch.Tensor = torch.tensor(
     [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]], dtype=torch.cdouble
 )
 
 
@@ -133,7 +141,32 @@
     result: torch.Tensor = operation.CRY(pi, state_10, (0, 1), 2)
     assert torch.allclose(state_11, result)
 
 
 def test_CRY_state01_controlqubit_0() -> None:
     result: torch.Tensor = operation.CRY(pi, state_01, (1, 0), 2)
     assert torch.allclose(state_11, result)
+
+
+def test_CSWAP_state000_controlqubit_0() -> None:
+    result: torch.Tensor = operation.CSWAP(state_000, (0, 1, 2), 3)
+    assert torch.allclose(state_000, result)
+
+
+def test_CSWAP_state001_controlqubit_0() -> None:
+    result: torch.Tensor = operation.CSWAP(state_001, (0, 1, 2), 3)
+    assert torch.allclose(state_001, result)
+
+
+def test_CSWAP_state100_controlqubit_0() -> None:
+    result: torch.Tensor = operation.CSWAP(state_100, (0, 1, 2), 3)
+    assert torch.allclose(state_100, result)
+
+
+def test_CSWAP_state101_controlqubit_0() -> None:
+    result: torch.Tensor = operation.CSWAP(state_101, (0, 1, 2), 3)
+    assert torch.allclose(state_110, result)
+
+
+def test_CSWAP_state110_controlqubit_0() -> None:
+    result: torch.Tensor = operation.CSWAP(state_110, (0, 1, 2), 3)
+    assert torch.allclose(state_101, result)
```

### Comparing `pyqtorch-0.3.1/tests/test_operations_hamevo.py` & `pyqtorch-0.3.2/tests/test_operations_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/.gitignore` & `pyqtorch-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/LICENSE` & `pyqtorch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.1/pyproject.toml` & `pyqtorch-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8,<3.12"
 license = {text = "Proprietary"}
-version = "0.3.1"
+version = "0.3.2"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyqtorch-0.3.1/PKG-INFO` & `pyqtorch-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

