# Comparing `tmp/pyMOTO-1.0.1.tar.gz` & `tmp/pyMOTO-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/Arnoud/projects/pyMOTO/dist/.tmp-d9k44b7r/pyMOTO-1.0.1.tar", last modified: Wed Mar  8 14:51:30 2023, max compression
+gzip compressed data, was "pyMOTO-1.0.2rc1.tar", last modified: Wed Jul 12 11:27:16 2023, max compression
```

## Comparing `pyMOTO-1.0.1.tar` & `pyMOTO-1.0.2rc1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 Arnoud     (501) staff       (20)        0 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/
--rw-r--r--   0 Arnoud     (501) staff       (20)     1072 2023-01-20 16:53:12.000000 pyMOTO-1.0.1/LICENSE
--rw-r--r--   0 Arnoud     (501) staff       (20)     4858 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/PKG-INFO
--rw-r--r--   0 Arnoud     (501) staff       (20)     4236 2023-02-27 20:33:55.000000 pyMOTO-1.0.1/README.md
-drwxr-xr-x   0 Arnoud     (501) staff       (20)        0 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/pyMOTO.egg-info/
--rw-r--r--   0 Arnoud     (501) staff       (20)     4858 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/pyMOTO.egg-info/PKG-INFO
--rw-r--r--   0 Arnoud     (501) staff       (20)      999 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/pyMOTO.egg-info/SOURCES.txt
--rw-r--r--   0 Arnoud     (501) staff       (20)        1 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/pyMOTO.egg-info/dependency_links.txt
--rw-r--r--   0 Arnoud     (501) staff       (20)       95 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/pyMOTO.egg-info/requires.txt
--rw-r--r--   0 Arnoud     (501) staff       (20)        7 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/pyMOTO.egg-info/top_level.txt
--rw-r--r--   0 Arnoud     (501) staff       (20)        1 2023-03-07 16:54:35.000000 pyMOTO-1.0.1/pyMOTO.egg-info/zip-safe
-drwxr-xr-x   0 Arnoud     (501) staff       (20)        0 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/pymoto/
--rw-r--r--   0 Arnoud     (501) staff       (20)     1958 2023-03-08 14:51:10.000000 pyMOTO-1.0.1/pymoto/__init__.py
-drwxr-xr-x   0 Arnoud     (501) staff       (20)        0 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/pymoto/common/
--rw-r--r--   0 Arnoud     (501) staff       (20)    15136 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/common/domain.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    17206 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/common/dyadcarrier.py
--rw-r--r--   0 Arnoud     (501) staff       (20)     8143 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/common/solvers.py
--rw-r--r--   0 Arnoud     (501) staff       (20)     9901 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/common/solvers_dense.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    15776 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/common/solvers_sparse.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    23212 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/core_objects.py
-drwxr-xr-x   0 Arnoud     (501) staff       (20)        0 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/pymoto/modules/
--rw-r--r--   0 Arnoud     (501) staff       (20)    10650 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/modules/assembly.py
--rw-r--r--   0 Arnoud     (501) staff       (20)     1684 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/modules/autodiff.py
--rw-r--r--   0 Arnoud     (501) staff       (20)     4421 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/modules/complex.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    18840 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/modules/filter.py
--rw-r--r--   0 Arnoud     (501) staff       (20)     8632 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/modules/generic.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    10532 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/modules/io.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    13201 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/modules/linalg.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    14490 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pymoto/routines.py
--rw-r--r--   0 Arnoud     (501) staff       (20)      795 2023-01-20 16:53:12.000000 pyMOTO-1.0.1/pymoto/utils.py
--rw-r--r--   0 Arnoud     (501) staff       (20)       86 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/pyproject.toml
--rw-r--r--   0 Arnoud     (501) staff       (20)      942 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/setup.cfg
-drwxr-xr-x   0 Arnoud     (501) staff       (20)        0 2023-03-08 14:51:30.000000 pyMOTO-1.0.1/tests/
--rw-r--r--   0 Arnoud     (501) staff       (20)     1269 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/tests/test_automod.py
--rw-r--r--   0 Arnoud     (501) staff       (20)     2990 2023-01-20 16:53:12.000000 pyMOTO-1.0.1/tests/test_complex.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    21372 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/tests/test_core.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    26839 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/tests/test_dyadcarrier.py
--rw-r--r--   0 Arnoud     (501) staff       (20)     6518 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/tests/test_module_eigensolve.py
--rw-r--r--   0 Arnoud     (501) staff       (20)     4910 2023-01-20 16:53:12.000000 pyMOTO-1.0.1/tests/test_module_einsum.py
--rw-r--r--   0 Arnoud     (501) staff       (20)     6660 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/tests/test_module_mathgeneral.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    14212 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/tests/test_solvers_dense.py
--rw-r--r--   0 Arnoud     (501) staff       (20)    19764 2023-03-08 14:27:36.000000 pyMOTO-1.0.1/tests/test_solvers_sparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:27:16.210141 pyMOTO-1.0.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-12 11:27:16.210141 pyMOTO-1.0.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:27:16.202140 pyMOTO-1.0.2rc1/pyMOTO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-12 11:27:16.000000 pyMOTO-1.0.2rc1/pyMOTO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-12 11:27:16.000000 pyMOTO-1.0.2rc1/pyMOTO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:27:16.000000 pyMOTO-1.0.2rc1/pyMOTO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 11:27:16.000000 pyMOTO-1.0.2rc1/pyMOTO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 11:27:16.000000 pyMOTO-1.0.2rc1/pyMOTO.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:27:15.000000 pyMOTO-1.0.2rc1/pyMOTO.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:27:16.202140 pyMOTO-1.0.2rc1/pymoto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:27:16.202140 pyMOTO-1.0.2rc1/pymoto/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/common/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17206 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/common/dyadcarrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23304 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/common/mma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/common/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/common/solvers_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15776 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/common/solvers_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23491 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/core_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:27:16.210141 pyMOTO-1.0.2rc1/pymoto/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/modules/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/modules/autodiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/modules/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/modules/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/modules/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/modules/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/modules/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pymoto/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-12 11:27:16.210141 pyMOTO-1.0.2rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:27:16.210141 pyMOTO-1.0.2rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_automod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26839 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_dyadcarrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_module_concatsignal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_module_eigensolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_module_einsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_module_mathgeneral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14212 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_solvers_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19764 2023-07-12 11:27:00.000000 pyMOTO-1.0.2rc1/tests/test_solvers_sparse.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyMOTO-1.0.1/LICENSE` & `pyMOTO-1.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/PKG-INFO` & `pyMOTO-1.0.2rc1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,8 @@
-Metadata-Version: 2.1
-Name: pyMOTO
-Version: 1.0.1
-Summary: Example package description
-Home-page: https://github.com/aatmdelissen/pyMOTO
-Author: Arnoud Delissen
-Author-email: arnouddelissen+pymoto@gmail.com
-License: MIT License
-Keywords: topology optimization,generative design,structural,sensitivities,derivatives,framework,modular,blocks,pipeline
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
+[![10.5281/zenodo.7708738](https://zenodo.org/badge/DOI/10.5281/zenodo.7708738.svg)](https://doi.org/10.5281/zenodo.7708738)
 
 # pyMOTO
 
 * [Link to Documentation](https://pymoto.readthedocs.io)
 * [Link to GitHub](https://github.com/aatmdelissen/pyMOTO)
 
 Modular topology optimization framework with semi-automatic derivatives. The two main types `Module` and `Signal`
@@ -50,39 +35,23 @@
 
 ## Dependencies
 * **NumPy** - Dense linear algebra and solvers
 * **SciPy** - Sparse linear algebra and solvers
 * **SymPy** - Symbolic differentiation for `MathGeneral` module
 * **Matplotlib** - Plotting and visualisation
 * (optional) **SAO** - Sequential approximated optimizers
-* (optional) **opt_einsum** - Optimized function for `EinSum` module
+* (optional) [**opt_einsum**](https://optimized-einsum.readthedocs.io/en/stable/install.html) - Optimized function for `EinSum` module
 
 For fast linear solvers for sparse matrices:
-* (optional) **scikit-umfpack** - Fast LU linear solver based on UMFPACK
-* (optional) **sksparse** - Fast Cholesky solver based on CHOLMOD
-* (optional) **CVXopt** - Another fast Cholesky solver based on CHOLMOD
-* (optional) **Intel OneAPI** - Non-python library with a fast PARDISO solver
+* (optional) [**pypardiso**](https://github.com/haasad/PyPardisoProject) - Uses the Intel OneAPI PARDISO solver (recommended)
+* (optional) [**scikit-umfpack**](https://scikit-umfpack.github.io/scikit-umfpack/install.html) - Fast LU linear solver based on UMFPACK
+* (optional) [**scikit-sparse**](https://github.com/scikit-sparse/scikit-sparse) - Fast Cholesky solver based on CHOLMOD
+* (optional) [**cvxopt**](https://cvxopt.org/install/index.html) - Another fast Cholesky solver based on CHOLMOD
 
 __Note on linear solvers for sparse matrices:__ Scipy implements a version of LU which is quite slow. To increase the 
-speed of the optimization, `Intel OneAPI` is recommended as it contains a very robust and flexible solver for symmetric 
+speed of the optimization, `pypardiso` is recommended as it contains a very robust and flexible solver for symmetric 
 and asymmetric matrices. An alternative is `scikit-umfpack` which provides a fast LU factorization. For symmetric 
 matrices a Cholesky factorization is recommended (not provided with Scipy), which can be used by either installing 
-`sksparse` or `cvxopt`.
-
-
-## How to make Python fast with Intel OneAPI
-Intel provides a toolkit with many fast math operations and solvers called OneAPI (basekit). 
-It can easily be installed on Linux by for instance following the steps described in https://www.intel.com/content/www/us/en/develop/documentation/installation-guide-for-intel-oneapi-toolkits-linux/top/installation/install-using-package-managers/apt.html
-For other OSes installation can be found in https://www.intel.com/content/www/us/en/developer/articles/guide/installation-guide-for-oneapi-toolkits.html
-
-The nice thing about OneAPI is that it also includes an optimized version of Python. To use it follow the next steps (Linux)
-
-1. `source <intel install location>/intel/oneapi/setvars.sh` (usually installed in `/opt/intel` or `/opt/ud/intel`). This loads the Intel OneAPI package.
-2. `conda create --name <venv_name> --clone base` to create a new conda virtual environment to work in.
-3. `conda activate <venv_name>` to activate the virtual environment.
-
-### Usage of multi-thread linear solvers
-Intel has a Pardiso type linear solver for fast solution of large systems.
-To use it.....
+`scikit-sparse` or `cvxopt`.
 
 # License
 pyMOTO is available under te [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `pyMOTO-1.0.1/pyMOTO.egg-info/SOURCES.txt` & `pyMOTO-1.0.2rc1/pyMOTO.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,33 +8,30 @@
 pyMOTO.egg-info/requires.txt
 pyMOTO.egg-info/top_level.txt
 pyMOTO.egg-info/zip-safe
 pymoto/__init__.py
 pymoto/core_objects.py
 pymoto/routines.py
 pymoto/utils.py
-pymoto.egg-info/PKG-INFO
-pymoto.egg-info/SOURCES.txt
-pymoto.egg-info/dependency_links.txt
-pymoto.egg-info/requires.txt
-pymoto.egg-info/top_level.txt
 pymoto/common/domain.py
 pymoto/common/dyadcarrier.py
+pymoto/common/mma.py
 pymoto/common/solvers.py
 pymoto/common/solvers_dense.py
 pymoto/common/solvers_sparse.py
 pymoto/modules/assembly.py
 pymoto/modules/autodiff.py
 pymoto/modules/complex.py
 pymoto/modules/filter.py
 pymoto/modules/generic.py
 pymoto/modules/io.py
 pymoto/modules/linalg.py
 tests/test_automod.py
 tests/test_complex.py
 tests/test_core.py
 tests/test_dyadcarrier.py
+tests/test_module_concatsignal.py
 tests/test_module_eigensolve.py
 tests/test_module_einsum.py
 tests/test_module_mathgeneral.py
 tests/test_solvers_dense.py
 tests/test_solvers_sparse.py
```

### Comparing `pyMOTO-1.0.1/pymoto/__init__.py` & `pyMOTO-1.0.2rc1/pymoto/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-__version__ = '1.0.1'
+__version__ = '1.0.2-rc1'
 
 from .core_objects import Signal, Module, Network, make_signals
 from .routines import finite_difference, minimize_oc, minimize_mma
 
 # Imports from common
 from .common.dyadcarrier import DyadCarrier
 from .common.domain import DomainDefinition
+from .common.mma import MMA
 from .common.solvers import matrix_is_complex, matrix_is_diagonal, matrix_is_symmetric, matrix_is_hermitian, \
     LinearSolver, LDAWrapper
 from .common.solvers_dense import SolverDiagonal, SolverDenseQR, SolverDenseLU, SolverDenseCholesky, SolverDenseLDL
 from .common.solvers_sparse import SolverSparsePardiso, SolverSparseLU, SolverSparseCholeskyScikit, SolverSparseCholeskyCVXOPT
 
 # Import from modules
-from .modules.generic import MathGeneral, EinSum
+from .modules.generic import MathGeneral, EinSum, ConcatSignal
 from .modules.linalg import Inverse, LinSolve, EigenSolve
 from .modules.assembly import AssembleGeneral, AssembleStiffness, AssembleMass
 from .modules.filter import FilterConv, Filter, DensityFilter, OverhangFilter
 from .modules.io import PlotDomain, PlotGraph, PlotIter, WriteToVTI
 from .modules.complex import MakeComplex, RealPart, ImagPart, ComplexNorm
 from .modules.autodiff import AutoMod
 
 __all__ = [
     'Signal', 'Module', 'Network', 'make_signals',
     'finite_difference', 'minimize_oc', 'minimize_mma',
     # Common
+    'MMA',
     'DyadCarrier',
     'DomainDefinition',
     'matrix_is_complex', 'matrix_is_diagonal', 'matrix_is_symmetric', 'matrix_is_hermitian',
     'LinearSolver', 'LDAWrapper',
     'SolverDiagonal', 'SolverDenseQR', 'SolverDenseLU', 'SolverDenseCholesky', 'SolverDenseLDL',
     'SolverSparsePardiso', 'SolverSparseLU', 'SolverSparseCholeskyScikit', 'SolverSparseCholeskyCVXOPT',
     # Modules
-    "MathGeneral", "EinSum",
+    "MathGeneral", "EinSum", "ConcatSignal",
     "Inverse", "LinSolve", "EigenSolve",
     "AssembleGeneral", "AssembleStiffness", "AssembleMass",
     "FilterConv", "Filter", "DensityFilter", "OverhangFilter",
     "PlotDomain", "PlotGraph", "PlotIter", "WriteToVTI",
     "MakeComplex", "RealPart", "ImagPart", "ComplexNorm",
     "AutoMod"
 ]
```

### Comparing `pyMOTO-1.0.1/pymoto/common/domain.py` & `pyMOTO-1.0.2rc1/pymoto/common/domain.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/pymoto/common/dyadcarrier.py` & `pyMOTO-1.0.2rc1/pymoto/common/dyadcarrier.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/pymoto/common/solvers.py` & `pyMOTO-1.0.2rc1/pymoto/common/solvers.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/pymoto/common/solvers_dense.py` & `pyMOTO-1.0.2rc1/pymoto/common/solvers_dense.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/pymoto/common/solvers_sparse.py` & `pyMOTO-1.0.2rc1/pymoto/common/solvers_sparse.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/pymoto/core_objects.py` & `pyMOTO-1.0.2rc1/pymoto/core_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union, List, Any
 import warnings
 import inspect
 import time
-from .utils import _parse_to_list
+from .utils import _parse_to_list, _concatenate_to_array, _split_from_array
 from abc import ABC, abstractmethod
 
 
 # Local helper functions
 def err_fmt(*args):
     """ Format error strings for locating Modules and Signals"""
     err_str = ""
@@ -31,15 +31,15 @@
     stk = inspect.stack()
     frame = None
     for fr in stk:
         if fr[1] != __file__:
             frame = fr
             break
     if frame is None:
-        return ""
+        return "N/A", "N/A", "N/A"
     _, filename, line, func, _, _ = frame
     return filename, line, func
 
 
 def get_init_str():
     filename, line, func = get_init_loc()
     return f"File \"{filename}\", line {line}, in {func}"
@@ -141,14 +141,18 @@
         :param item: Slice indices
         :return: Sliced signal (SignalSlice)
         """
         return SignalSlice(self, item)
 
 
 class SignalSlice(Signal):
+    """ Slice operator for a Signal
+    The sliced values are referenced to their original source Signal, such that they can be used and updated in modules.
+    This means that updating the values in this SignalSlice changes the data in its source Signal.
+    """
     def __init__(self, orig_signal, sl, tag=None):
         self.orig_signal = orig_signal
         self.slice = sl
         self.keep_alloc = True  # This parameter probably doesn't matter
 
         # for s in slice:
         if tag is None:
@@ -161,53 +165,53 @@
 
     @property
     def state(self):
         try:
             return None if self.orig_signal.state is None else self.orig_signal.state[self.slice]
         except Exception as e:
             # Possibilities: Unslicable object (TypeError) or Wrong dimensions or out of range (IndexError)
-            raise type(e)("Get state - " + e.args[0] + self._err_str(), *e.args[1:]) from None
+            raise type(e)("SignalSlice.state (getter)" + self._err_str()) from e
 
     @state.setter
     def state(self, new_state):
         try:
             self.orig_signal.state[self.slice] = new_state
         except Exception as e:
             # Possibilities: Unslicable object (TypeError) or Wrong dimensions or out of range (IndexError)
-            raise type(e)("Set state - " + e.args[0] + self._err_str(), *e.args[1:]) from None
+            raise type(e)("SignalSlice.state (setter)" + self._err_str()) from e
 
     @property
     def sensitivity(self):
         try:
             return None if self.orig_signal.sensitivity is None else self.orig_signal.sensitivity[self.slice]
         except Exception as e:
             # Possibilities: Unslicable object (TypeError) or Wrong dimensions or out of range (IndexError)
-            raise type(e)("Get sensitivity - " + e.args[0] + self._err_str(), *e.args[1:]) from None
+            raise type(e)("SignalSlice.sensitivity (getter)" + self._err_str()) from e
 
     @sensitivity.setter
     def sensitivity(self, new_sens):
-        if self.orig_signal.sensitivity is None:
-            if new_sens is None:
-                return  # Sensitivity doesn't need to be initialized when it is set to None
-            try:
-                self.orig_signal.sensitivity = self.orig_signal.state*0  # Make a new copy with 0 values
-            except TypeError:
-                if self.orig_signal.state is None:
-                    raise TypeError("Could not initialize sensitivity because state is not set" + self._err_str()) from None
-                else:
-                    raise TypeError(f"Could not initialize sensitivity for type \'{type(self.orig_signal.state).__name__}\'" + self._err_str()) from None
+        try:
+            if self.orig_signal.sensitivity is None:
+                if new_sens is None:
+                    return  # Sensitivity doesn't need to be initialized when it is set to None
+                try:
+                    self.orig_signal.sensitivity = self.orig_signal.state * 0  # Make a new copy with 0 values
+                except TypeError:
+                    if self.orig_signal.state is None:
+                        raise TypeError("Could not initialize sensitivity because state is not set" + self._err_str())
+                    else:
+                        raise TypeError(f"Could not initialize sensitivity for type \'{type(self.orig_signal.state).__name__}\'")
 
-        if new_sens is None:
-            new_sens = 0  # reset() uses this
+            if new_sens is None:
+                new_sens = 0  # reset() uses this
 
-        try:
             self.orig_signal.sensitivity[self.slice] = new_sens
         except Exception as e:
             # Possibilities: Unslicable object (TypeError) or Wrong dimensions or out of range (IndexError)
-            raise type(e)("Set sensitivity - " + e.args[0] + self._err_str(), *e.args[1:]) from None
+            raise type(e)("SignalSlice.sensitivity (setter)" + self._err_str()) from e
 
 
 def make_signals(*args):
     """ Batch-initialize a number of Signals
     :param args: Tags for a number of Signals
     :return: Dictionary of Signals, with key index equal to the signal tag
     """
```

### Comparing `pyMOTO-1.0.1/pymoto/modules/assembly.py` & `pyMOTO-1.0.2rc1/pymoto/modules/assembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,18 +233,30 @@
         **kwargs : Other keyword-arguments are passed to AssembleGeneral
     """
     def _prepare(self, domain: DomainDefinition, *args, rho: float = 1.0, bcdiagval=0.0, **kwargs):
         # Element mass matrix
         # 1/36 Mass of one element
         mel = rho * np.prod(domain.element_size)
 
-        # Consistent mass matrix
-        ME = mel / 36 * np.array([[4.0, 0.0, 2.0, 0.0, 2.0, 0.0, 1.0, 0.0],
-                                  [0.0, 4.0, 0.0, 2.0, 0.0, 2.0, 0.0, 1.0],
-                                  [2.0, 0.0, 4.0, 0.0, 1.0, 0.0, 2.0, 0.0],
-                                  [0.0, 2.0, 0.0, 4.0, 0.0, 1.0, 0.0, 2.0],
-                                  [2.0, 0.0, 1.0, 0.0, 4.0, 0.0, 2.0, 0.0],
-                                  [0.0, 2.0, 0.0, 1.0, 0.0, 4.0, 0.0, 2.0],
-                                  [1.0, 0.0, 2.0, 0.0, 2.0, 0.0, 4.0, 0.0],
-                                  [0.0, 1.0, 0.0, 2.0, 0.0, 2.0, 0.0, 4.0]])
+        if domain.dim == 2:
+            # Consistent mass matrix
+            ME = mel / 36 * np.array([[4.0, 0.0, 2.0, 0.0, 2.0, 0.0, 1.0, 0.0],
+                                      [0.0, 4.0, 0.0, 2.0, 0.0, 2.0, 0.0, 1.0],
+                                      [2.0, 0.0, 4.0, 0.0, 1.0, 0.0, 2.0, 0.0],
+                                      [0.0, 2.0, 0.0, 4.0, 0.0, 1.0, 0.0, 2.0],
+                                      [2.0, 0.0, 1.0, 0.0, 4.0, 0.0, 2.0, 0.0],
+                                      [0.0, 2.0, 0.0, 1.0, 0.0, 4.0, 0.0, 2.0],
+                                      [1.0, 0.0, 2.0, 0.0, 2.0, 0.0, 4.0, 0.0],
+                                      [0.0, 1.0, 0.0, 2.0, 0.0, 2.0, 0.0, 4.0]])
+        elif domain.dim == 3:
+            ME = np.zeros((domain.elemnodes*domain.dim, domain.elemnodes*domain.dim))
+            weights = np.array([8.0, 4.0, 2.0, 1.0])
+            for n1 in range(domain.elemnodes):
+                for n2 in range(domain.elemnodes):
+                    dist = round(np.sum(abs(np.array(domain.node_numbering[n1]) - np.array(domain.node_numbering[n2])))/2)
+                    ME[n1*domain.dim+np.arange(domain.dim), n2*domain.dim+np.arange(domain.dim)] = weights[dist]
 
+            ME *= mel / 216
+        else:
+            raise RuntimeError("Only for 2D and 3D")
         super()._prepare(domain, ME, *args, bcdiagval=bcdiagval, **kwargs)
+
```

### Comparing `pyMOTO-1.0.1/pymoto/modules/autodiff.py` & `pyMOTO-1.0.2rc1/pymoto/modules/autodiff.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/pymoto/modules/complex.py` & `pyMOTO-1.0.2rc1/pymoto/modules/complex.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/pymoto/modules/filter.py` & `pyMOTO-1.0.2rc1/pymoto/modules/filter.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/pymoto/modules/generic.py` & `pyMOTO-1.0.2rc1/pymoto/modules/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Generic modules, valid for general mathematical operations """
 import numpy as np
 from pymoto.core_objects import Module
+from pymoto.utils import _concatenate_to_array, _split_from_array
 try:
     from opt_einsum import contract as einsum  # Faster einsum
 except ModuleNotFoundError:
     from numpy import einsum
 
 
 class MathGeneral(Module):
@@ -196,7 +197,27 @@
             ind_out = self.indices_in[ar]
 
             da_i = np.zeros_like(self.sig_in[ar].state)
             op = ",".join(ind_in)+"->"+ind_out
             einsum(op, df_in, *arg_in, out=da_i)
             df_out.append(da_i)
         return df_out
+
+
+class ConcatSignal(Module):
+    """ Concatenates data of multiple signals into one big vector """
+    def _response(self, *args):
+        state, self.cumlens = _concatenate_to_array(list(args))
+        return state
+
+    def _sensitivity(self, dy):
+        dsens = [np.zeros_like(s.state) for s in self.sig_in]
+        dx = _split_from_array(dy, self.cumlens)
+        for i, s in enumerate(self.sig_in):
+            if not isinstance(dsens[i], type(s.state)):
+                dsens[i] = type(s.state)(dx[i])
+                continue
+            try:
+                dsens[i][...] = dx[i]
+            except TypeError:
+                dsens[i] = type(s.state)(dx[i])
+        return dsens
```

### Comparing `pyMOTO-1.0.1/pymoto/modules/io.py` & `pyMOTO-1.0.2rc1/pymoto/modules/io.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/pymoto/modules/linalg.py` & `pyMOTO-1.0.2rc1/pymoto/modules/linalg.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import warnings
 import hashlib
 from inspect import currentframe, getframeinfo
 
 from pymoto import Module, DyadCarrier, LDAWrapper
 import numpy as np
 import scipy.sparse as sps
+import scipy.sparse.linalg as spsla
 import scipy.linalg as spla  # Dense matrix solvers
 
 from pymoto import SolverDenseLU, SolverDenseLDL, SolverDenseCholesky, SolverDiagonal, SolverDenseQR
 from pymoto import matrix_is_symmetric, matrix_is_hermitian, matrix_is_diagonal
 from pymoto import SolverSparseLU, SolverSparseCholeskyCVXOPT, SolverSparsePardiso, SolverSparseCholeskyScikit
 
 
@@ -238,60 +239,137 @@
       - ``λ`` (`vector`): Vector with eigenvalues of size ``(n)``
       - ``Q`` (`matrix`): Matrix with eigenvectors ``Q[:, i]`` corresponding to ``λ[i]``, of size ``(n, n)``
 
     Keyword Args:
         sorting_func: Sorting function to sort the eigenvalues, which must have signature ``func(λ,Q)``
           (default = ``numpy.argsort``)
         hermitian: Flag to omit the automatic detection for Hermitian matrix, saves some work for large matrices
+        nmodes: Number of modes to calculate (only for sparse matrices, default = ``0``)
+        sigma: Shift value for the eigenvalue problem (only for sparse matrices). Eigenvalues around the shift are
+          calculated first (default = ``0.0``)
     """
-    def _prepare(self, sorting_func=lambda W, Q: np.argsort(W), hermitian=None):
+    def _prepare(self, sorting_func=lambda W, Q: np.argsort(W), hermitian=None, nmodes=None, sigma=None):
         self.sorting_fn = sorting_func
         self.is_hermitian = hermitian
+        self.nmodes = nmodes
+        self.sigma = sigma
+        self.Ainv = None
+
 
     def _response(self, A, *args):
         B = args[0] if len(args) > 0 else None
         if self.is_hermitian is None:
             self.is_hermitian = (matrix_is_hermitian(A) and (B is None or matrix_is_hermitian(B)))
-        W, Q = spla.eigh(A, b=B) if self.is_hermitian else spla.eig(A, b=B)
+        self.is_sparse = sps.issparse(A) and (B is None or sps.issparse(B))
+        if self.is_sparse:
+            W, Q = self._sparse_eigs(A, B=B)
+        else:
+            W, Q = spla.eigh(A, b=B) if self.is_hermitian else spla.eig(A, b=B)
+
         isort = self.sorting_fn(W, Q)
         W = W[isort]
         Q = Q[:, isort]
         for i in range(W.size):
             qi, wi = Q[:, i], W[i]
-            qi *= np.sign(np.real(qi[0]))
+            qi *= np.sign(np.real(qi[np.argmax(abs(qi)>0)]))
             Bqi = qi if B is None else B@qi
             qi /= np.sqrt(qi@Bqi)
             assert (abs(qi@(qi if B is None else B@qi) - 1.0) < 1e-5)
             assert (np.linalg.norm(A@qi - wi*(qi if B is None else B@qi)) < 1e-5)
         return W, Q
 
     def _sensitivity(self, dW, dQ):
         A = self.sig_in[0].state
         B = self.sig_in[1].state if len(self.sig_in) > 1 else np.eye(*A.shape)
+        dA, dB = None, None
+        if not self.is_sparse:
+            dA, dB = self._dense_sens(A, B, dW, dQ)
+        else:
+            if dQ is not None:
+                raise NotImplementedError('Sparse eigenvector sensitivities not implemented')
+            elif dW is not None:
+                dA, dB = self._sparse_eigval_sens(A, B, dW)
+
+        if len(self.sig_in) == 1:
+            return dA
+        elif len(self.sig_in) == 2:
+            return dA, dB
+
+
+    def _sparse_eigs(self, A, B=None):
+        if self.nmodes is None:
+            self.nmodes = 6
+        if self.sigma is None:
+            self.sigma = 0.0
+
+        if self.sigma == 0.0:  # No shift
+            mat_shifted = A
+        else:
+            if B is None:  # If no B is given, use identity to shift
+                B = sps.eye(*A.shape)
+            mat_shifted = A - self.sigma * B
+
+        # Use shift-and-invert, so make inverse operator
+        if self.Ainv is None:
+            self.Ainv = auto_determine_solver(mat_shifted, ishermitian=self.is_hermitian)
+        self.Ainv.update(mat_shifted)
+
+        AinvOp = spsla.LinearOperator(mat_shifted.shape, matvec=self.Ainv.solve, rmatvec=self.Ainv.adjoint)
+
+        if self.is_hermitian:
+            return spsla.eigsh(A, M=B, k=self.nmodes, OPinv=AinvOp, sigma=self.sigma)
+        else:
+            # TODO
+            raise NotImplementedError('Non-Hermitian sparse matrix not supported')
+
+    def _dense_sens(self, A, B, dW, dQ):
+        """ Calculates all (eigenvector and eigenvalue) sensitivities for dense matrix """
         dA = np.zeros_like(A)
         dB = np.zeros_like(B) if len(self.sig_in) > 1 else None
         W, Q = [s.state for s in self.sig_out]
         if dW is None:
             dW = np.zeros_like(W)
         if dQ is None:
             dQ = np.zeros_like(Q)
 
         for i in range(W.size):
             dqi, dwi = dQ[:, i], dW[i]
             if np.linalg.norm(dqi) == 0 and dwi == 0:
                 continue
             qi, wi = Q[:, i], W[i]
 
-            P = np.block([[(A - wi*B).T, -((B + B.T)/2)@qi[..., np.newaxis]], [-B@qi.T, 0]])
+            P = np.block([[(A - wi * B).T, -((B + B.T) / 2) @ qi[..., np.newaxis]], [-B @ qi.T, 0]])
             adj = np.linalg.solve(P, np.block([dqi, dwi]))  # Adjoint solve Lee(1999)
             nu = adj[:-1]
             alpha = adj[-1]
             dAi = np.outer(-nu, qi)
             dA += dAi if np.iscomplexobj(A) else np.real(dAi)
             if dB is not None:
-                dBi = np.outer(wi*nu + alpha/2*qi, qi)
+                dBi = np.outer(wi * nu + alpha / 2 * qi, qi)
                 dB += dBi if np.iscomplexobj(B) else np.real(dBi)
+        return dA, dB
+
+    def _sparse_eigval_sens(self, A, B, dW):
+        if dW is None:
+            return None, None
+        W, Q = [s.state for s in self.sig_out]
+        dA, dB = DyadCarrier(), None if B is None else DyadCarrier()
+        for i in range(W.size):
+            wi, dwi = W[i], dW[i]
+            if dwi == 0:
+                continue
+            qi = Q[:, i]
+            qmq = qi@qi if B is None else qi @ (B @ qi)
+            dA_u = (dwi/qmq) * qi
+            if np.isrealobj(A):
+                dA += DyadCarrier([np.real(dA_u), -np.imag(dA_u)], [np.real(qi), np.imag(qi)])
+            else:
+                dA += DyadCarrier(dA_u, qi)
+
+            if dB is not None:
+                dB_u = (wi*dwi/qmq) * qi
+                if np.isrealobj(B):
+                    dB -= DyadCarrier([np.real(dB_u), -np.imag(dB_u)], [np.real(qi), np.imag(qi)])
+                else:
+                    dB -= DyadCarrier(dB_u, qi)
+        return dA, dB
 
-        if len(self.sig_in) == 1:
-            return dA
-        elif len(self.sig_in) == 2:
-            return dA, dB
```

### Comparing `pyMOTO-1.0.1/pymoto/routines.py` & `pyMOTO-1.0.2rc1/pymoto/routines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from .utils import _parse_to_list, _concatenate_to_array
 from .core_objects import Signal, Module, Network
+from .common.mma import MMA
 from typing import List, Iterable, Union, Callable
 
 
 # flake8: noqa: C901
 def finite_difference(blk: Module, fromsig: Union[Signal, Iterable[Signal]] = None,
                       tosig: Union[Signal, Iterable[Signal]] = None,
                       dx: float = 1e-8, tol: float = 1e-5, random: bool = True, use_df: list = None,
@@ -267,15 +268,15 @@
 
         sens.append(the_sens)
     return sens
 
 
 def minimize_oc(function, variables, objective: Signal,
                 tolx=1e-4, tolf=1e-4, maxit=100, xmin=0.0, xmax=1.0, move=0.2,
-                l1init=0, l2init=100000, l1l2tol=1e-4, maxvol=None):
+                l1init=0, l2init=100000, l1l2tol=1e-4, maxvol=None, verbosity=2):
     """ Execute minimization using the OC-method
 
     Args:
         function: The Network defining the optimization problem
         variables: The Signals defining the design variables
         objective: The objective function Signal to be minimized
 
@@ -285,123 +286,81 @@
         maxit: Maximum number of iteration
         xmin: Minimum design variable (can be a vector)
         xmax: Maximum design variable (can be a vector)
         move: Move limit
         l1init: OC internal parameter
         l2init: OC internal parameter
         l1l2tol: OC internal parameter
+        verbosity: 0 - No prints, 1 - Only convergence message, 2 - Convergence and iteration info
+
     """
+    variables = _parse_to_list(variables)
     xval, cumlens = _concatenate_to_array([s.state for s in variables])
 
     if maxvol is None:
         maxvol = np.sum(xval)
 
     f = 0.0
     for it in range(maxit):
         # Calculate response
         function.response()
         fprev, f = f, objective.state
         rel_fchange = abs(f-fprev)/abs(f)
         if rel_fchange < tolf:
-            print(f"OC converged: Relative function change |Δf|/|f| ({rel_fchange}) below tolerance ({tolf})")
+            if verbosity >= 1:
+                print(f"OC converged: Relative function change |Δf|/|f| ({rel_fchange}) below tolerance ({tolf})")
             break
 
-        print("It. {0: 4d}, f0 = {1: .2e}, Δf = {2: .2e}".format(it, f, f-fprev))
+        if verbosity >= 2:
+            print("It. {0: 4d}, f0 = {1: .2e}, Δf = {2: .2e}".format(it, f, f-fprev))
 
         # Calculate sensitivity of the objective
         function.reset()
         objective.sensitivity = 1.0
         function.sensitivity()
         dfdx, _ = _concatenate_to_array(obtain_sensitivities(variables))
+        maxdfdx = max(dfdx)
+        if maxdfdx > 0:
+            raise RuntimeError(f"OC only works for negative sensitivities: max(dfdx) = {maxdfdx}")
 
         # Do OC update
         l1, l2 = l1init, l2init
         while l2 - l1 > l1l2tol:
             lmid = 0.5 * (l1 + l2)
             xnew = np.clip(xval * np.sqrt(-dfdx / lmid), np.maximum(xmin, xval-move), np.minimum(xmax, xval+move))
             l1, l2 = (lmid, l2) if np.sum(xnew) - maxvol > 0 else (l1, lmid)
 
         # Stopping criteria on step size
         rel_stepsize = np.linalg.norm(xval - xnew)/np.linalg.norm(xval)
         if rel_stepsize < tolx:
-            print(f"OC converged: Relative stepsize |Δx|/|x| ({rel_stepsize}) below tolerance ({tolx})")
+            if verbosity >= 1:
+                print(f"OC converged: Relative stepsize |Δx|/|x| ({rel_stepsize}) below tolerance ({tolx})")
             break
 
         xval = xnew
         # Set the new states
         for i, s in enumerate(variables):
             s.state = xnew[cumlens[i]:cumlens[i + 1]]
 
 
-def minimize_mma(function, variables, responses, tolx=1e-4, tolf=1e-4, maxit=1000, xmin=0.0, xmax=1.0):
+def minimize_mma(function, variables, responses, tolx=1e-4, tolf=1e-4, maxit=1000, move=0.1, xmin=0.0, xmax=1.0, verbosity=2):
     """ Execute minimization using the MMA-method
-
-    Uses the ``nlopt`` version of MMA.
-
-    Todo:
-        Improve the MMA implementation as the ``nlopt`` version is not very good
+    Svanberg (1987), The method of moving asymptotes - a new method for structural optimization
 
     Args:
         function: The Network defining the optimization problem
         variables: The Signals defining the design variables
         responses: A list of Signals, where the first is to be minimized and the others are constraints.
 
     Keyword Args:
         tolx: Stopping criterium for relative design change
         tolf: Stopping criterium for relative objective change
         maxit: Maximum number of iteration
+        move: Move limit on relative variable change per iteration
         xmin: Minimum design variable (can be a vector)
         xmax: Maximum design variable (can be a vector)
+        verbosity: 0 - No prints, 1 - Only convergence message, 2 - Convergence and iteration info, 3 - Extended info
+
     """
     # Save initial state
-    xval, cumlens = _concatenate_to_array([s.state for s in variables])
-    n = len(xval)
-
-    def fi(_, grad, i):
-
-        if grad.size > 0:
-            # Calculate sensitivities
-            function.reset()
-
-            responses[i].sensitivity = 1.0
-
-            function.sensitivity()
-
-            grad[:], _ = _concatenate_to_array(obtain_sensitivities(variables))
-
-        return responses[i].state
-
-    global it
-    it = 0
-
-    # Objective function
-    def f0(x, grad):
-        global it
-        # Set the new states
-        for i, s in enumerate(variables):
-            s.state = x[cumlens[i]:cumlens[i + 1]]
-
-        # Calculate response
-        function.response()
-
-        print("It. {0: 4d}, f0 = {1: .2e}, f1 = {2: .2e}".format(it, responses[0].state, responses[1].state))
-        it += 1
-
-        return fi(x, grad, 0)
-
-    # Create optimization
-    import nlopt
-
-    opt = nlopt.opt(nlopt.LD_MMA, n)
-
-    opt.set_min_objective(f0)
-    for ri in range(1, len(responses)):
-        opt.add_inequality_constraint(lambda x, grad: fi(x, grad, ri))
-
-    opt.set_lower_bounds(np.ones_like(xval) * xmin)
-    opt.set_upper_bounds(np.ones_like(xval) * xmax)
-
-    opt.set_maxeval(maxit)
-    opt.set_xtol_rel(tolx)
-    opt.set_ftol_rel(tolf)
-
-    opt.optimize(xval)
+    mma = MMA(function, variables, responses, tolx=tolx, move=move, maxit=maxit, xmin=xmin, xmax=xmax, verbosity=verbosity)
+    mma.response()
```

### Comparing `pyMOTO-1.0.1/setup.cfg` & `pyMOTO-1.0.2rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/tests/test_complex.py` & `pyMOTO-1.0.2rc1/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/tests/test_core.py` & `pyMOTO-1.0.2rc1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/tests/test_dyadcarrier.py` & `pyMOTO-1.0.2rc1/tests/test_dyadcarrier.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/tests/test_module_eigensolve.py` & `pyMOTO-1.0.2rc1/tests/test_module_eigensolve.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/tests/test_module_einsum.py` & `pyMOTO-1.0.2rc1/tests/test_module_einsum.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/tests/test_module_mathgeneral.py` & `pyMOTO-1.0.2rc1/tests/test_module_mathgeneral.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/tests/test_solvers_dense.py` & `pyMOTO-1.0.2rc1/tests/test_solvers_dense.py`

 * *Files identical despite different names*

### Comparing `pyMOTO-1.0.1/tests/test_solvers_sparse.py` & `pyMOTO-1.0.2rc1/tests/test_solvers_sparse.py`

 * *Files identical despite different names*

