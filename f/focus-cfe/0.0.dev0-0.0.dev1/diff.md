# Comparing `tmp/focus-cfe-0.0.dev0.tar.gz` & `tmp/focus-cfe-0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/focus-cfe-0.0.dev0.tar", last modified: Mon Jul 10 20:27:02 2023, max compression
+gzip compressed data, was "dist/focus-cfe-0.0.dev1.tar", last modified: Wed Jul 12 15:22:35 2023, max compression
```

## Comparing `focus-cfe-0.0.dev0.tar` & `focus-cfe-0.0.dev1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-10 20:27:02.787590 focus-cfe-0.0.dev0/
--rw-r--r--   0 kyosuke    (501) staff       (20)     2809 2023-07-10 20:27:02.787872 focus-cfe-0.0.dev0/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)     1624 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev0/README.rst
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-10 20:27:02.782817 focus-cfe-0.0.dev0/focus/
--rw-r--r--   0 kyosuke    (501) staff       (20)      597 2023-07-09 21:15:11.000000 focus-cfe-0.0.dev0/focus/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)    18301 2023-07-10 20:24:44.000000 focus-cfe-0.0.dev0/focus/core.py
--rw-r--r--   0 kyosuke    (501) staff       (20)    18308 2023-07-10 20:24:44.000000 focus-cfe-0.0.dev0/focus/focus.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-10 20:27:02.784628 focus-cfe-0.0.dev0/focus/tests/
--rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev0/focus/tests/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     3883 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev0/focus/tests/test_focus.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev0/focus/tests/test_utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4643 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev0/focus/utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)      567 2023-07-10 20:24:44.000000 focus-cfe-0.0.dev0/focus/version.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-10 20:27:02.787092 focus-cfe-0.0.dev0/focus_cfe.egg-info/
--rw-r--r--   0 kyosuke    (501) staff       (20)     2809 2023-07-10 20:27:02.000000 focus-cfe-0.0.dev0/focus_cfe.egg-info/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)      316 2023-07-10 20:27:02.000000 focus-cfe-0.0.dev0/focus_cfe.egg-info/SOURCES.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-10 20:27:02.000000 focus-cfe-0.0.dev0/focus_cfe.egg-info/dependency_links.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        6 2023-07-10 20:27:02.000000 focus-cfe-0.0.dev0/focus_cfe.egg-info/top_level.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-10 20:27:02.788833 focus-cfe-0.0.dev0/setup.cfg
--rw-r--r--   0 kyosuke    (501) staff       (20)     1547 2023-07-10 20:26:59.000000 focus-cfe-0.0.dev0/setup.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-12 15:22:35.843560 focus-cfe-0.0.dev1/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     2838 2023-07-12 15:22:35.843812 focus-cfe-0.0.dev1/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1657 2023-07-12 14:42:42.000000 focus-cfe-0.0.dev1/README.rst
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-12 15:22:35.840494 focus-cfe-0.0.dev1/focus/
+-rw-r--r--   0 kyosuke    (501) staff       (20)      597 2023-07-12 15:12:04.000000 focus-cfe-0.0.dev1/focus/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)    18285 2023-07-12 15:12:04.000000 focus-cfe-0.0.dev1/focus/core.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)    18308 2023-07-10 22:03:45.000000 focus-cfe-0.0.dev1/focus/focus.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-12 15:22:35.841923 focus-cfe-0.0.dev1/focus/tests/
+-rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev1/focus/tests/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3883 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev1/focus/tests/test_focus.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev1/focus/tests/test_utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4643 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev1/focus/utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)      568 2023-07-12 15:22:29.000000 focus-cfe-0.0.dev1/focus/version.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-12 15:22:35.843317 focus-cfe-0.0.dev1/focus_cfe.egg-info/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     2838 2023-07-12 15:22:35.000000 focus-cfe-0.0.dev1/focus_cfe.egg-info/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)      316 2023-07-12 15:22:35.000000 focus-cfe-0.0.dev1/focus_cfe.egg-info/SOURCES.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-12 15:22:35.000000 focus-cfe-0.0.dev1/focus_cfe.egg-info/dependency_links.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        6 2023-07-12 15:22:35.000000 focus-cfe-0.0.dev1/focus_cfe.egg-info/top_level.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-12 15:22:35.844478 focus-cfe-0.0.dev1/setup.cfg
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1543 2023-07-10 22:03:45.000000 focus-cfe-0.0.dev1/setup.py
```

### Comparing `focus-cfe-0.0.dev0/PKG-INFO` & `focus-cfe-0.0.dev1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 1.1
 Name: focus-cfe
-Version: 0.0.dev0
-Summary: ``FOCUS`` is a python package for generating counterfactual explanations for a tree-based model
+Version: 0.0.dev1
+Summary: FOCUS is a python package for generating counterfactual explanations for a tree-based model
 Home-page: UNKNOWN
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 License: UNKNOWN
 Description: FOCUS: Flexible Optimizable Counterfactual Explanations for Tree Ensembles
         ==========================================================================
         
         **Deployment & Documentation & Stats & License**
         
-        .. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
-           :target: https://pypi.org/project/focus/
+        .. image:: https://img.shields.io/pypi/v/focus-cfe.svg?color=brightgreen
+           :target: https://pypi.org/project/focus-cfe/
            :alt: PyPI version
         
-        .. image:: https://coveralls.io/repos/github/kyosek/focus/badge.svg
-           :target: https://coveralls.io/github/kyosek/focus
+        .. image:: https://coveralls.io/repos/github/kyosek/focus-cfe/badge.svg
+           :target: https://coveralls.io/github/kyosek/focus-cfe
            :alt: Coverage Status
         
         .. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
-           :target: https://codeclimate.com/github/kyosek/focus/maintainability
+           :target: https://codeclimate.com/github/kyosek/focus-cfe/maintainability
            :alt: Maintainability
         
         -----
         
         This library is an implementation of `FOCUS: Flexible Optimizable Counterfactual Explanations for Tree Ensembles <https://arxiv.org/abs/1911.12199>`_.
         
         FOCUS generates optimal distance counterfactual explanations to the original data for all the instances in tree‐based machine learning models.
@@ -43,20 +43,20 @@
         ^^^^^^^^^^^^
         
         It is recommended to use **pip** or **conda** for installation. Please make sure
         **the latest version** is installed:
         
         .. code-block:: bash
         
-           pip install focus            # normal install
-           pip install --upgrade focus  # or update if needed
+           pip install focus-cfe            # normal install
+           pip install --upgrade focus-cfe  # or update if needed
         
         .. code-block:: bash
         
-           conda install -c conda-forge focus
+           conda install -c conda-forge focus-cfe
         
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `focus-cfe-0.0.dev0/README.rst` & `focus-cfe-0.0.dev1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 FOCUS: Flexible Optimizable Counterfactual Explanations for Tree Ensembles
 ==========================================================================
 
 **Deployment & Documentation & Stats & License**
 
-.. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
-   :target: https://pypi.org/project/focus/
+.. image:: https://img.shields.io/pypi/v/focus-cfe.svg?color=brightgreen
+   :target: https://pypi.org/project/focus-cfe/
    :alt: PyPI version
 
-.. image:: https://coveralls.io/repos/github/kyosek/focus/badge.svg
-   :target: https://coveralls.io/github/kyosek/focus
+.. image:: https://coveralls.io/repos/github/kyosek/focus-cfe/badge.svg
+   :target: https://coveralls.io/github/kyosek/focus-cfe
    :alt: Coverage Status
 
 .. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
-   :target: https://codeclimate.com/github/kyosek/focus/maintainability
+   :target: https://codeclimate.com/github/kyosek/focus-cfe/maintainability
    :alt: Maintainability
 
 -----
 
 This library is an implementation of `FOCUS: Flexible Optimizable Counterfactual Explanations for Tree Ensembles <https://arxiv.org/abs/1911.12199>`_.
 
 FOCUS generates optimal distance counterfactual explanations to the original data for all the instances in tree‐based machine learning models.
@@ -35,13 +35,13 @@
 ^^^^^^^^^^^^
 
 It is recommended to use **pip** or **conda** for installation. Please make sure
 **the latest version** is installed:
 
 .. code-block:: bash
 
-   pip install focus            # normal install
-   pip install --upgrade focus  # or update if needed
+   pip install focus-cfe            # normal install
+   pip install --upgrade focus-cfe  # or update if needed
 
 .. code-block:: bash
 
-   conda install -c conda-forge focus
+   conda install -c conda-forge focus-cfe
```

### Comparing `focus-cfe-0.0.dev0/focus/__init__.py` & `focus-cfe-0.0.dev1/focus/__init__.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev0/focus/core.py` & `focus-cfe-0.0.dev1/focus/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         )
         n_examples = len(X)
         distance_weight: np.ndarray = np.full(n_examples, self.distance_weight)
         to_optimize = [perturbed]
         mask_vector = np.ones(n_examples)
         best_perturb = np.zeros(perturbed.shape)
         best_distance = np.full(n_examples, np.inf)
-        predictions = tf.constant(model.predict(X), dtype=tf.int64)
+        predictions = tf.constant(model.predict(X))
         example_index = tf.constant(np.arange(n_examples, dtype=int))
         example_pred_class_index = tf.stack((example_index, predictions), axis=1)
 
         for i in range(1, self.num_iter + 1):
             if self.verbose != 0:
                 print(f"iteration {i}")
```

### Comparing `focus-cfe-0.0.dev0/focus/focus.py` & `focus-cfe-0.0.dev1/focus/focus.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev0/focus/tests/test_focus.py` & `focus-cfe-0.0.dev1/focus/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev0/focus/tests/test_utils.py` & `focus-cfe-0.0.dev1/focus/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev0/focus/utils.py` & `focus-cfe-0.0.dev1/focus/utils.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev0/focus/version.py` & `focus-cfe-0.0.dev1/focus/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.0.dev"  # pragma: no cover
+__version__ = "0.0.dev1"  # pragma: no cover
```

### Comparing `focus-cfe-0.0.dev0/focus_cfe.egg-info/PKG-INFO` & `focus-cfe-0.0.dev1/focus_cfe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 1.1
 Name: focus-cfe
-Version: 0.0.dev0
-Summary: ``FOCUS`` is a python package for generating counterfactual explanations for a tree-based model
+Version: 0.0.dev1
+Summary: FOCUS is a python package for generating counterfactual explanations for a tree-based model
 Home-page: UNKNOWN
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 License: UNKNOWN
 Description: FOCUS: Flexible Optimizable Counterfactual Explanations for Tree Ensembles
         ==========================================================================
         
         **Deployment & Documentation & Stats & License**
         
-        .. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
-           :target: https://pypi.org/project/focus/
+        .. image:: https://img.shields.io/pypi/v/focus-cfe.svg?color=brightgreen
+           :target: https://pypi.org/project/focus-cfe/
            :alt: PyPI version
         
-        .. image:: https://coveralls.io/repos/github/kyosek/focus/badge.svg
-           :target: https://coveralls.io/github/kyosek/focus
+        .. image:: https://coveralls.io/repos/github/kyosek/focus-cfe/badge.svg
+           :target: https://coveralls.io/github/kyosek/focus-cfe
            :alt: Coverage Status
         
         .. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
-           :target: https://codeclimate.com/github/kyosek/focus/maintainability
+           :target: https://codeclimate.com/github/kyosek/focus-cfe/maintainability
            :alt: Maintainability
         
         -----
         
         This library is an implementation of `FOCUS: Flexible Optimizable Counterfactual Explanations for Tree Ensembles <https://arxiv.org/abs/1911.12199>`_.
         
         FOCUS generates optimal distance counterfactual explanations to the original data for all the instances in tree‐based machine learning models.
@@ -43,20 +43,20 @@
         ^^^^^^^^^^^^
         
         It is recommended to use **pip** or **conda** for installation. Please make sure
         **the latest version** is installed:
         
         .. code-block:: bash
         
-           pip install focus            # normal install
-           pip install --upgrade focus  # or update if needed
+           pip install focus-cfe            # normal install
+           pip install --upgrade focus-cfe  # or update if needed
         
         .. code-block:: bash
         
-           conda install -c conda-forge focus
+           conda install -c conda-forge focus-cfe
         
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `focus-cfe-0.0.dev0/setup.py` & `focus-cfe-0.0.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from io import open
 from os import path
 
 from setuptools import find_packages, setup
 
 DESCRIPTION = (
-    "``FOCUS`` is a python package for "
+    "FOCUS is a python package for "
     "generating counterfactual explanations for a tree-based model"
 )
 
 
 # get __version__ from _version.py
 ver_file = path.join("focus", "version.py")
 with open(ver_file) as f:
```

