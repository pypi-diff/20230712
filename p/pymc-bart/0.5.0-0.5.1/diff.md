# Comparing `tmp/pymc_bart-0.5.0.tar.gz` & `tmp/pymc_bart-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc_bart-0.5.0.tar", last modified: Mon Jul 10 17:47:16 2023, max compression
+gzip compressed data, was "pymc_bart-0.5.1.tar", last modified: Wed Jul 12 11:34:29 2023, max compression
```

## Comparing `pymc_bart-0.5.0.tar` & `pymc_bart-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:47:16.811866 pymc_bart-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-10 17:47:16.811866 pymc_bart-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:47:16.807866 pymc_bart-0.5.0/pymc_bart/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/bart.py
--rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/pgbart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/split_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    27945 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:47:16.807866 pymc_bart-0.5.0/pymc_bart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:47:16.811866 pymc_bart-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:47:16.811866 pymc_bart-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/test_bart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/test_pgbart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/test_split_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:34:29.538965 pymc_bart-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-12 11:34:29.538965 pymc_bart-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:34:29.534965 pymc_bart-0.5.1/pymc_bart/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/pymc_bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/pymc_bart/bart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/pymc_bart/pgbart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/pymc_bart/split_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/pymc_bart/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28037 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/pymc_bart/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:34:29.538965 pymc_bart-0.5.1/pymc_bart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-12 11:34:29.000000 pymc_bart-0.5.1/pymc_bart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-12 11:34:29.000000 pymc_bart-0.5.1/pymc_bart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:34:29.000000 pymc_bart-0.5.1/pymc_bart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 11:34:29.000000 pymc_bart-0.5.1/pymc_bart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 11:34:29.000000 pymc_bart-0.5.1/pymc_bart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 11:34:29.538965 pymc_bart-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:34:29.538965 pymc_bart-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/tests/test_bart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/tests/test_pgbart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/tests/test_split_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-12 11:34:20.000000 pymc_bart-0.5.1/tests/test_tree.py
```

### Comparing `pymc_bart-0.5.0/CODE_OF_CONDUCT.md` & `pymc_bart-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/CONTRIBUTING.md` & `pymc_bart-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/LICENSE` & `pymc_bart-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/PKG-INFO` & `pymc_bart-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pymc_bart
-Version: 0.5.0
+Version: 0.5.1
 Summary: Bayesian Additive Regression Trees for Probabilistic programming with PyMC
 Home-page: http://github.com/pymc-devs/pymc-bart
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pymc_bart-0.5.0/README.md` & `pymc_bart-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/pymc_bart/__init__.py` & `pymc_bart-0.5.1/pymc_bart/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     plot_pdp,
     plot_ice,
     plot_dependence,
     plot_variable_importance,
 )
 
 __all__ = ["BART", "PGBART"]
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 pm.STEP_METHODS = list(pm.STEP_METHODS) + [PGBART]
```

### Comparing `pymc_bart-0.5.0/pymc_bart/bart.py` & `pymc_bart-0.5.1/pymc_bart/bart.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+import warnings
 from multiprocessing import Manager
 from typing import List, Optional, Tuple
-import warnings
 
 import numpy as np
 import numpy.typing as npt
 import pytensor.tensor as pt
 from pandas import DataFrame, Series
 from pymc.distributions.distribution import Distribution, _moment
 from pymc.logprob.abstract import _logprob
 from pytensor.tensor.random.op import RandomVariable
 
+from .split_rules import SplitRule
 from .tree import Tree
 from .utils import TensorLike, _sample_posterior
-from .split_rules import SplitRule
 
 __all__ = ["BART"]
 
 
 class BARTRV(RandomVariable):
     """Base class for BART."""
 
@@ -43,15 +43,15 @@
     _print_name: Tuple[str, str] = ("BART", "\\operatorname{BART}")
     all_trees = List[List[List[Tree]]]
 
     def _supp_shape_from_params(self, dist_params, rep_param_idx=1, param_shapes=None):
         return dist_params[0].shape[:1]
 
     @classmethod
-    def rng_fn(
+    def rng_fn(  # pylint: disable=W0237
         cls, rng=None, X=None, Y=None, m=None, alpha=None, beta=None, split_prior=None, size=None
     ):
         if not cls.all_trees:
             if size is not None:
                 return np.full((size[0], cls.Y.shape[0]), cls.Y.mean())
             else:
                 return np.full(cls.Y.shape[0], cls.Y.mean())
@@ -89,15 +89,15 @@
     beta : float
         Controls the prior probability over the number of leaves of the trees.
         Should be positive.
     split_prior : Optional[List[float]], default None.
         Each element of split_prior should be in the [0, 1] interval and the elements should sum to
         1. Otherwise they will be normalized.
         Defaults to 0, i.e. all covariates have the same prior probability to be selected.
-    split_rules : Optional[SplitRule], default None
+    split_rules : Optional[List[SplitRule]], default None
         List of SplitRule objects, one per column in input data.
         Allows using different split rules for different columns. Default is ContinuousSplitRule.
         Other options are OneHotSplitRule and SubsetSplitRule, both meant for categorical variables.
     shape: : Optional[Tuple], default None
         Specify the output shape. If shape is different from (len(X)) (the default), train a
         separate tree for each value in other dimensions.
     separate_trees : Optional[bool], default False
@@ -123,15 +123,15 @@
         X: TensorLike,
         Y: TensorLike,
         m: int = 50,
         alpha: float = 0.95,
         beta: float = 2.0,
         response: str = "constant",
         split_prior: Optional[List[float]] = None,
-        split_rules: Optional[SplitRule] = None,
+        split_rules: Optional[List[SplitRule]] = None,
         separate_trees: Optional[bool] = False,
         **kwargs,
     ):
         if response in ["linear", "mix"]:
             warnings.warn(
                 "Options linear and mix are experimental and still not well tested\n"
                 + "Use with caution."
@@ -143,29 +143,29 @@
 
         if split_prior is None:
             split_prior = []
 
         bart_op = type(
             f"BART_{name}",
             (BARTRV,),
-            dict(
-                name="BART",
-                all_trees=cls.all_trees,
-                inplace=False,
-                initval=Y.mean(),
-                X=X,
-                Y=Y,
-                m=m,
-                response=response,
-                alpha=alpha,
-                beta=beta,
-                split_prior=split_prior,
-                split_rules=split_rules,
-                separate_trees=separate_trees,
-            ),
+            {
+                "name": "BART",
+                "all_trees": cls.all_trees,
+                "inplace": False,
+                "initval": Y.mean(),
+                "X": X,
+                "Y": Y,
+                "m": m,
+                "response": response,
+                "alpha": alpha,
+                "beta": beta,
+                "split_prior": split_prior,
+                "split_rules": split_rules,
+                "separate_trees": separate_trees,
+            },
         )()
 
         Distribution.register(BARTRV)
 
         @_moment.register(BARTRV)
         def get_moment(rv, size, *rv_inputs):
             return cls.get_moment(rv, size, *rv_inputs)
```

### Comparing `pymc_bart-0.5.0/pymc_bart/pgbart.py` & `pymc_bart-0.5.1/pymc_bart/pgbart.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/pymc_bart/split_rules.py` & `pymc_bart-0.5.1/pymc_bart/split_rules.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/pymc_bart/tree.py` & `pymc_bart-0.5.1/pymc_bart/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from functools import lru_cache
 from typing import Dict, Generator, List, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 from pytensor import config
+
 from .split_rules import SplitRule
 
 
 class Node:
     """Node of a binary tree.
 
     Attributes
@@ -97,14 +98,18 @@
         A dictionary that represents the nodes stored in breadth-first order, based in the array
         method for storing binary trees (https://en.wikipedia.org/wiki/Binary_tree#Arrays).
         The dictionary's keys are integers that represent the nodes position.
         The dictionary's values are objects of type Node that represent the split and leaf nodes
         of the tree itself.
     output: Optional[npt.NDArray[np.float_]]
         Array of shape number of observations, shape
+    split_rules : List[SplitRule]
+        List of SplitRule objects, one per column in input data.
+        Allows using different split rules for different columns. Default is ContinuousSplitRule.
+        Other options are OneHotSplitRule and SubsetSplitRule, both meant for categorical variables.
     idx_leaf_nodes : Optional[List[int]], by default None.
         Array with the index of the leaf nodes of the tree.
 
     Parameters
     ----------
     tree_structure : Dictionary of nodes
     output : Array of shape number of observations, shape
```

### Comparing `pymc_bart-0.5.0/pymc_bart/utils.py` & `pymc_bart-0.5.1/pymc_bart/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,19 @@
     -------
     axes: matplotlib axes
     """
     all_trees = bartrv.owner.op.all_trees
     rng = np.random.default_rng(random_seed)
 
     if func is None:
-        func = lambda x: x
+
+        def identity(x):
+            return x
+
+        func = identity
 
     (
         X,
         x_labels,
         y_label,
         indices,
         var_idx,
@@ -285,15 +289,15 @@
         for s_i in range(shape):
             if centered:
                 p_di = func(p_d[:, :, s_i]) - func(p_d[:, :, s_i][:, 0][:, None])
             else:
                 p_di = func(p_d[:, :, s_i])
             if var in var_discrete:
                 axes[count].plot(new_x, p_di.mean(0), "o", color=color_mean)
-                axes[count].plot(new_x, p_di, ".", color=color, alpha=alpha)
+                axes[count].plot(new_x, p_di.T, ".", color=color, alpha=alpha)
             else:
                 if smooth:
                     x_data, y_data = _smooth_mean(new_x, p_di, "ice", smooth_kwargs)
                     axes[count].plot(x_data, y_data.mean(1), color=color_mean)
                     axes[count].plot(x_data, y_data, color=color, alpha=alpha)
                 else:
                     idx = np.argsort(new_x)
@@ -353,15 +357,15 @@
     var_idx : Optional[List[int]], by default None.
         List of the indices of the covariate for which to compute the pdp or ice.
     var_discrete : Optional[List[int]], by default None.
         List of the indices of the covariate treated as discrete.
     func : Optional[Callable], by default None.
         Arbitrary function to apply to the predictions. Defaults to the identity function.
     samples : int
-        Number of posterior samples used in the predictions. Defaults to 400
+        Number of posterior samples used in the predictions. Defaults to 200
     random_seed : Optional[int], by default None.
         Seed used to sample from the posterior. Defaults to None.
     sharey : bool
         Controls sharing of properties among y-axes. Defaults to True.
     smooth : bool
         If True the result will be smoothed by first computing a linear interpolation of the data
         over a regular grid and then applying the Savitzky-Golay filter to the interpolated data.
@@ -388,15 +392,19 @@
     -------
     axes: matplotlib axes
     """
     all_trees: list = bartrv.owner.op.all_trees
     rng = np.random.default_rng(random_seed)
 
     if func is None:
-        func = lambda x: x
+
+        def identity(x):
+            return x
+
+        func = identity
 
     (
         X,
         x_labels,
         y_label,
         indices,
         var_idx,
```

### Comparing `pymc_bart-0.5.0/pymc_bart.egg-info/PKG-INFO` & `pymc_bart-0.5.1/pymc_bart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pymc-bart
-Version: 0.5.0
+Version: 0.5.1
 Summary: Bayesian Additive Regression Trees for Probabilistic programming with PyMC
 Home-page: http://github.com/pymc-devs/pymc-bart
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pymc_bart-0.5.0/pymc_bart.egg-info/SOURCES.txt` & `pymc_bart-0.5.1/pymc_bart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/setup.py` & `pymc_bart-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 URL = "http://github.com/pymc-devs/pymc-bart"
 LICENSE = "Apache License, Version 2.0"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pymc_bart-0.5.0/tests/__init__.py` & `pymc_bart-0.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/tests/test_bart.py` & `pymc_bart-0.5.1/tests/test_bart.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
                 "xs_interval": "quantiles",
                 "xs_values": [0.25, 0.5, 0.75],
                 "var_discrete": [3],
             },
             {"instances": 2},
             {"var_idx": [0], "smooth": False, "color": "k"},
             {"grid": (1, 2), "sharey": "none", "alpha": 1},
+            {"var_discrete": [0]}
         ],
     )
     def test_ice(self, kwargs):
         pmb.plot_ice(self.mu, X=self.X, Y=self.Y, **kwargs)
 
     @pytest.mark.parametrize(
         "kwargs",
@@ -173,14 +174,15 @@
                 "samples": 2,
                 "xs_interval": "quantiles",
                 "xs_values": [0.25, 0.5, 0.75],
                 "var_discrete": [3],
             },
             {"var_idx": [0], "smooth": False, "color": "k"},
             {"grid": (1, 2), "sharey": "none", "alpha": 1},
+            {"var_discrete": [0]}
         ],
     )
     def test_pdp(self, kwargs):
         pmb.plot_pdp(self.mu, X=self.X, Y=self.Y, **kwargs)
 
     @pytest.mark.parametrize(
         "kwargs",
```

### Comparing `pymc_bart-0.5.0/tests/test_pgbart.py` & `pymc_bart-0.5.1/tests/test_pgbart.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/tests/test_split_rules.py` & `pymc_bart-0.5.1/tests/test_split_rules.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.0/tests/test_tree.py` & `pymc_bart-0.5.1/tests/test_tree.py`

 * *Files identical despite different names*

