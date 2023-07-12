# Comparing `tmp/equine-0.1.1rc3.tar.gz` & `tmp/equine-0.1.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equine-0.1.1rc3.tar", last modified: Tue Jul 11 23:05:41 2023, max compression
+gzip compressed data, was "equine-0.1.1rc4.tar", last modified: Wed Jul 12 02:08:57 2023, max compression
```

## Comparing `equine-0.1.1rc3.tar` & `equine-0.1.1rc4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:05:41.268428 equine-0.1.1rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-11 23:05:31.000000 equine-0.1.1rc3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-11 23:05:41.268428 equine-0.1.1rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-11 23:05:31.000000 equine-0.1.1rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-11 23:05:31.000000 equine-0.1.1rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 23:05:41.268428 equine-0.1.1rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:05:41.264428 equine-0.1.1rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:05:41.264428 equine-0.1.1rc3/src/equine/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-11 23:05:31.000000 equine-0.1.1rc3/src/equine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-11 23:05:31.000000 equine-0.1.1rc3/src/equine/equine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23483 2023-07-11 23:05:31.000000 equine-0.1.1rc3/src/equine/equine_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-11 23:05:31.000000 equine-0.1.1rc3/src/equine/equine_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    30231 2023-07-11 23:05:31.000000 equine-0.1.1rc3/src/equine/equine_protonet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-07-11 23:05:31.000000 equine-0.1.1rc3/src/equine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:05:41.268428 equine-0.1.1rc3/src/equine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-11 23:05:41.000000 equine-0.1.1rc3/src/equine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-11 23:05:41.000000 equine-0.1.1rc3/src/equine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 23:05:41.000000 equine-0.1.1rc3/src/equine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 23:05:41.000000 equine-0.1.1rc3/src/equine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 23:05:41.000000 equine-0.1.1rc3/src/equine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:05:41.268428 equine-0.1.1rc3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3897 2023-07-11 23:05:31.000000 equine-0.1.1rc3/tests/test_equine_gp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2005 2023-07-11 23:05:31.000000 equine-0.1.1rc3/tests/test_equine_integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7470 2023-07-11 23:05:31.000000 equine-0.1.1rc3/tests/test_equine_protonet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-11 23:05:31.000000 equine-0.1.1rc3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:08:57.244254 equine-0.1.1rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-12 02:08:47.000000 equine-0.1.1rc4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-12 02:08:57.244254 equine-0.1.1rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-12 02:08:47.000000 equine-0.1.1rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-12 02:08:47.000000 equine-0.1.1rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 02:08:57.244254 equine-0.1.1rc4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:08:57.240254 equine-0.1.1rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:08:57.244254 equine-0.1.1rc4/src/equine/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-12 02:08:47.000000 equine-0.1.1rc4/src/equine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-12 02:08:47.000000 equine-0.1.1rc4/src/equine/equine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23483 2023-07-12 02:08:47.000000 equine-0.1.1rc4/src/equine/equine_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-12 02:08:47.000000 equine-0.1.1rc4/src/equine/equine_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30231 2023-07-12 02:08:47.000000 equine-0.1.1rc4/src/equine/equine_protonet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-07-12 02:08:47.000000 equine-0.1.1rc4/src/equine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:08:57.244254 equine-0.1.1rc4/src/equine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-12 02:08:57.000000 equine-0.1.1rc4/src/equine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-12 02:08:57.000000 equine-0.1.1rc4/src/equine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 02:08:57.000000 equine-0.1.1rc4/src/equine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-12 02:08:57.000000 equine-0.1.1rc4/src/equine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 02:08:57.000000 equine-0.1.1rc4/src/equine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:08:57.244254 equine-0.1.1rc4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3897 2023-07-12 02:08:47.000000 equine-0.1.1rc4/tests/test_equine_gp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2005 2023-07-12 02:08:47.000000 equine-0.1.1rc4/tests/test_equine_integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7470 2023-07-12 02:08:47.000000 equine-0.1.1rc4/tests/test_equine_protonet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-12 02:08:47.000000 equine-0.1.1rc4/tests/test_utils.py
```

### Comparing `equine-0.1.1rc3/LICENSE.md` & `equine-0.1.1rc4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `equine-0.1.1rc3/PKG-INFO` & `equine-0.1.1rc4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equine
-Version: 0.1.1rc3
+Version: 0.1.1rc4
 Summary: EQUINE^2: Establishing Quantified Uncertainty for Neural Networks
 Author: Allan Wollaber, Steven Jorgensen, John Holodnak, Jensen Dempsey, Harry Li
 License: MIT
 Project-URL: Homepage, https://mit-ll-responsible-ai.github.io/equine/
 Project-URL: Bug Tracker, https://github.com/mit-ll-responsible-ai/equine/issues
 Project-URL: Source, https://github.com/mit-ll-responsible-ai/equine
 Keywords: machine learning,robustness,pytorch,responsible,AI
@@ -19,15 +19,15 @@
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # Establishing Quantified Uncertainty in Neural Networks 
 <p align="center"><img src="assets/equine_full_logo.svg" width="720"\></p>
 
-
+[![PyPi](https://img.shields.io/pypi/v/equine.svg)](https://pypi.org/project/equine/)
 [![Build Status](https://github.com/mit-ll-responsible-ai/equine/actions/workflows/Tests.yml/badge.svg?branch=main)](https://github.com/mit-ll-responsible-ai/equine/actions/workflows/Tests.yml)
 ![python_passing_tests](https://img.shields.io/badge/Tests%20Passed-100%25-green)
 ![python_coverage](https://img.shields.io/badge/Coverage-97%25-green)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Tested with Hypothesis](https://img.shields.io/badge/hypothesis-tested-brightgreen.svg)](https://hypothesis.readthedocs.io/)
 
 ## Usage
```

### Comparing `equine-0.1.1rc3/README.md` & `equine-0.1.1rc4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Establishing Quantified Uncertainty in Neural Networks 
 <p align="center"><img src="assets/equine_full_logo.svg" width="720"\></p>
 
-
+[![PyPi](https://img.shields.io/pypi/v/equine.svg)](https://pypi.org/project/equine/)
 [![Build Status](https://github.com/mit-ll-responsible-ai/equine/actions/workflows/Tests.yml/badge.svg?branch=main)](https://github.com/mit-ll-responsible-ai/equine/actions/workflows/Tests.yml)
 ![python_passing_tests](https://img.shields.io/badge/Tests%20Passed-100%25-green)
 ![python_coverage](https://img.shields.io/badge/Coverage-97%25-green)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Tested with Hypothesis](https://img.shields.io/badge/hypothesis-tested-brightgreen.svg)](https://hypothesis.readthedocs.io/)
 
 ## Usage
```

### Comparing `equine-0.1.1rc3/pyproject.toml` & `equine-0.1.1rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `equine-0.1.1rc3/setup.cfg` & `equine-0.1.1rc4/setup.cfg`

 * *Files identical despite different names*

### Comparing `equine-0.1.1rc3/src/equine/__init__.py` & `equine-0.1.1rc4/src/equine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     generate_support,
     generate_episode,
     generate_model_metrics,
     generate_train_summary,
     generate_model_summary,
 )
 
-__version__ = "0.1.1rc3"
+__version__ = "0.1.1rc4"
 
 __all__ = [
     "Equine",
     "EquineOutput",
     "EquineGP",
     "EquineProtonet",
     "CovType",
```

### Comparing `equine-0.1.1rc3/src/equine/equine_gp.py` & `equine-0.1.1rc4/src/equine/equine_gp.py`

 * *Files identical despite different names*

### Comparing `equine-0.1.1rc3/src/equine/equine_output.py` & `equine-0.1.1rc4/src/equine/equine_output.py`

 * *Files identical despite different names*

### Comparing `equine-0.1.1rc3/src/equine/equine_protonet.py` & `equine-0.1.1rc4/src/equine/equine_protonet.py`

 * *Files identical despite different names*

### Comparing `equine-0.1.1rc3/src/equine/utils.py` & `equine-0.1.1rc4/src/equine/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -194,14 +194,27 @@
 
     if return_indexes:
         return support, shuffled_idxs
     else:
         return support
 
 
+@icontract.require(lambda train_x: len(train_x.shape) == 2)
+@icontract.require(lambda train_y: len(train_y.shape) == 1)
+@icontract.require(lambda support_size: support_size > 1)
+@icontract.require(lambda way: way > 0)
+@icontract.require(lambda episode_size: episode_size > 0)
+@icontract.ensure(lambda result: len(result) == 3)
+@icontract.ensure(lambda result: result[1].shape[0] == result[2].shape[0])
+@icontract.ensure(lambda way, result: len(result[0]) == way)
+@icontract.ensure(
+    lambda support_size, result: all(
+        len(support) == support_size for support in result[0].values()
+    )
+)
 @typechecked
 def generate_episode(
     train_x: torch.Tensor,
     train_y: torch.Tensor,
     support_size: int,
     way: int,
     episode_size: int,
@@ -232,15 +245,15 @@
         labels[torch.randperm(labels.shape[0])][:way].tolist()
     )  # need to be in same order every time
 
     support, shuffled_idxs = generate_support(
         train_x, train_y, support_size, selected_labels, return_indexes=True
     )
 
-    examples_per_task = int(episode_size / way)
+    examples_per_task = episode_size // way
 
     episode_data_list = []
     episode_label_list = []
     episode_support = OrderedDict()
     for episode_label, label in enumerate(selected_labels):
         shuffled_x = train_x[shuffled_idxs[label]]
         shuffled_y = torch.Tensor(
@@ -302,14 +315,19 @@
         "expectedCalibrationError": expected_calibration_error(
             eq_preds.classes, true_y
         ),
     }
     return metrics
 
 
+@icontract.require(lambda Y: len(Y.shape) == 1)
+@icontract.ensure(
+    lambda result: all("label" in d and "numExamples" in d for d in result)
+)
+@icontract.ensure(lambda result: all(d["numExamples"] >= 0 for d in result))
 @typechecked
 def get_num_examples_per_label(Y: torch.Tensor) -> List[Dict[str, Any]]:
     """
     Get the number of examples per label in the given tensor.
 
     Parameters
     ----------
```

### Comparing `equine-0.1.1rc3/src/equine.egg-info/PKG-INFO` & `equine-0.1.1rc4/src/equine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equine
-Version: 0.1.1rc3
+Version: 0.1.1rc4
 Summary: EQUINE^2: Establishing Quantified Uncertainty for Neural Networks
 Author: Allan Wollaber, Steven Jorgensen, John Holodnak, Jensen Dempsey, Harry Li
 License: MIT
 Project-URL: Homepage, https://mit-ll-responsible-ai.github.io/equine/
 Project-URL: Bug Tracker, https://github.com/mit-ll-responsible-ai/equine/issues
 Project-URL: Source, https://github.com/mit-ll-responsible-ai/equine
 Keywords: machine learning,robustness,pytorch,responsible,AI
@@ -19,15 +19,15 @@
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # Establishing Quantified Uncertainty in Neural Networks 
 <p align="center"><img src="assets/equine_full_logo.svg" width="720"\></p>
 
-
+[![PyPi](https://img.shields.io/pypi/v/equine.svg)](https://pypi.org/project/equine/)
 [![Build Status](https://github.com/mit-ll-responsible-ai/equine/actions/workflows/Tests.yml/badge.svg?branch=main)](https://github.com/mit-ll-responsible-ai/equine/actions/workflows/Tests.yml)
 ![python_passing_tests](https://img.shields.io/badge/Tests%20Passed-100%25-green)
 ![python_coverage](https://img.shields.io/badge/Coverage-97%25-green)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Tested with Hypothesis](https://img.shields.io/badge/hypothesis-tested-brightgreen.svg)](https://hypothesis.readthedocs.io/)
 
 ## Usage
```

### Comparing `equine-0.1.1rc3/tests/test_equine_gp.py` & `equine-0.1.1rc4/tests/test_equine_gp.py`

 * *Files identical despite different names*

### Comparing `equine-0.1.1rc3/tests/test_equine_integration.py` & `equine-0.1.1rc4/tests/test_equine_integration.py`

 * *Files identical despite different names*

### Comparing `equine-0.1.1rc3/tests/test_equine_protonet.py` & `equine-0.1.1rc4/tests/test_equine_protonet.py`

 * *Files identical despite different names*

### Comparing `equine-0.1.1rc3/tests/test_utils.py` & `equine-0.1.1rc4/tests/test_utils.py`

 * *Files identical despite different names*

