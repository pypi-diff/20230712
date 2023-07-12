# Comparing `tmp/landmarkclassifier-2.0.7.tar.gz` & `tmp/landmarkclassifier-2.1.0.tar.gz`

## Comparing `landmarkclassifier-2.0.7.tar` & `landmarkclassifier-2.1.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/environment.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/LANDMark.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/__init__.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/lm_dtree_clfs.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/lm_linear_clfs.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/lm_nnet_clfs.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/lm_oracle_clfs.py
--rw-r--r--   0        0        0    21548 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/tree.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LANDMark/utils.py
--rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/docs/API.md
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/tests/__init__.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/tests/test_landmark.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/.gitignore
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/LICENSE
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/README.md
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/environment.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/LANDMark.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/__init__.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/lm_dtree_clfs.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/lm_linear_clfs.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/lm_nnet_clfs.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/lm_oracle_clfs.py
+-rw-r--r--   0        0        0    29098 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/tree.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/utils.py
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/docs/API.md
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0    38524 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/notebooks/ExampleUsage.ipynb
+-rw-r--r--   0        0        0   388411 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/notebooks/ParameterChoices.ipynb
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/tests/test_landmark.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/README.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/PKG-INFO
```

### Comparing `landmarkclassifier-2.0.7/.github/ISSUE_TEMPLATE/bug_report.md` & `landmarkclassifier-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.7/.github/ISSUE_TEMPLATE/feature_request.md` & `landmarkclassifier-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.7/.github/workflows/ci.yml` & `landmarkclassifier-2.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.7/.github/workflows/python-publish.yml` & `landmarkclassifier-2.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.7/LANDMark/LANDMark.py` & `landmarkclassifier-2.1.0/LANDMark/LANDMark.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,51 +8,56 @@
 from sklearn.base import ClassifierMixin, BaseEstimator
 from sklearn.metrics import balanced_accuracy_score
 from sklearn.utils import check_X_y
 from sklearn.utils.validation import check_is_fitted
 
 from typing import Optional, List
 
+from scipy.sparse import csr_array, issparse
 
-class LANDMarkClassifier(BaseEstimator, ClassifierMixin):
 
+class LANDMarkClassifier(BaseEstimator, ClassifierMixin):
     def __init__(
         self,
         n_estimators: int = 64,
         min_samples_in_leaf: int = 5,
         max_depth: Optional[int] = None,
         max_features: float = 0.80,
         min_gain: float = 0.0,
         impurity: str = "gain",
         q: float = 1.5,
         use_oracle: bool = True,
         use_lm_l2: bool = True,
         use_lm_l1: bool = True,
+        minority_sz_lm: int = 6,
         use_nnet: bool = True,
         nnet_min_samples: int = 32,
+        minority_sz_nnet: int = 6,
         use_etc: bool = True,
         etc_max_depth: int = 5,
         etc_max_trees: int = 128,
-        resampler = None,
+        resampler=None,
         use_cascade: bool = False,
-        n_jobs: int = 4
+        n_jobs: int = 4,
     ):
         # Tree construction parameters
         self.n_estimators = n_estimators
         self.min_samples_in_leaf = min_samples_in_leaf
         self.max_depth = max_depth
         self.max_features = max_features
         self.min_gain = min_gain
         self.impurity = impurity
         self.q = q
         self.use_oracle = use_oracle
         self.use_lm_l2 = use_lm_l2
         self.use_lm_l1 = use_lm_l1
+        self.minority_sz_lm = minority_sz_lm
         self.use_nnet = use_nnet
         self.nnet_min_samples = nnet_min_samples
+        self.minority_sz_nnet = minority_sz_nnet
         self.use_etc = use_etc
         self.etc_max_depth = etc_max_depth
         self.etc_max_trees = etc_max_trees
         self.resampler = resampler
         self.use_cascade = use_cascade
 
         self.n_jobs = n_jobs
@@ -81,20 +86,23 @@
                 max_features=self.max_features,
                 min_gain=self.min_gain,
                 impurity=self.impurity,
                 q=self.q,
                 use_oracle=self.use_oracle,
                 use_lm_l2=self.use_lm_l2,
                 use_lm_l1=self.use_lm_l1,
+                minority_sz_lm=self.minority_sz_lm,
                 use_nnet=self.use_nnet,
                 nnet_min_samples=self.nnet_min_samples,
+                minority_sz_nnet=self.minority_sz_nnet,
                 use_etc=self.use_etc,
                 etc_max_depth=self.etc_max_depth,
                 etc_max_trees=self.etc_max_trees,
-                resampler=self.resampler
+                resampler=self.resampler,
+                use_cascade=self.use_cascade,
             ),
             n_estimators=self.n_estimators,
             class_names=self.classes_,
             n_jobs=self.n_jobs,
         )
 
         self.estimators_.fit(X_checked, y_checked)
@@ -136,31 +144,86 @@
     def score(self, X: np.ndarray, y: np.ndarray) -> float:
         check_is_fitted(self, attributes=["classes_", "estimators_"])
 
         score = balanced_accuracy_score(y, self.predict(X))
 
         return score
 
-    def proximity(self, X: np.ndarray) -> np.ndarray:
+    def proximity(self, X: np.ndarray, prox_type: str = "path") -> np.ndarray:
         check_is_fitted(self, attributes=["classes_", "estimators_"])
 
-        tree_mats = []
-
-        for estimator in self.estimators_.estimators_:
-            tree_mats.append(estimator.proximity(X))
+        if prox_type == "terminal":
+            tree_mats = []
 
-        emb = np.hstack(tree_mats)
+            for estimator in self.estimators_.estimators_:
+                tree_mats.append(estimator.proximity(X, prox_type))
 
-        return emb
+            emb = np.hstack(tree_mats)
 
-    def _check_params(self, X: np.ndarray, y: np.ndarray) -> List[np.ndarray, np.ndarray]:
+            return csr_array(emb.astype(np.uint8))
+
+        elif prox_type == "path":
+            if hasattr(self, "node_set"):
+                embs = [
+                    est.proximity(X, prox_type) for est in self.estimators_.estimators_
+                ]
+
+                if X.ndim == 1:
+                    emb = np.zeros(shape=(1, len(self.node_set)), dtype=np.uint8)
+                else:
+                    emb = np.zeros(
+                        shape=(X.shape[0], len(self.node_set)), dtype=np.uint8
+                    )
+
+                for tree_emb in embs:
+                    for sample, nodes in tree_emb.items():
+                        for node in nodes:
+                            emb[sample, self.node_set[node]] = 1
+
+                return csr_array(emb)
+
+            else:
+                # Get the list of nodes associated with each sample in X
+                embs = [
+                    est.proximity(X, prox_type) for est in self.estimators_.estimators_
+                ]
+
+                # Create a list of all nodes across all trees in the forest
+                node_set = set()
+                [node_set.update(est.all_nodes) for est in self.estimators_.estimators_]
+
+                node_set = list(node_set)
+
+                # Create the embedding matrix
+                emb = np.zeros(shape=(X.shape[0], len(node_set)), dtype=np.uint8)
+
+                # Create a mapping between node id and index in the embedding matrix
+                self.node_set = {node: i for i, node in enumerate(node_set)}
+                
+                # Update the embedding matrix
+                for tree_emb in embs:
+                    for sample, nodes in tree_emb.items():
+                        for node in nodes:
+                            emb[sample, self.node_set[node]] = 1
+
+                return csr_array(emb)
+
+    def _check_params(
+        self, X: np.ndarray, y: np.ndarray
+    ) -> List[np.ndarray, np.ndarray]:
         SUPPORTED_IMPURITY = {"gain", "gain-ratio", "tsallis", "tsallis-gain-ratio"}
 
         # Check that X and y meet the minimum requirements
-        X_conv, y_conv = check_X_y(X, y, accept_sparse=False)
+        X_conv, y_conv = check_X_y(X, y, accept_sparse=True)
+
+        if not issparse(X_conv):
+            sparsity = 1.0 - (np.count_nonzero(X_conv) / X_conv.size)
+
+            if sparsity >= 0.9:
+                X_conv = csr_array(X_conv)
 
         if not isinstance(self.n_estimators, int):
             raise TypeError("'n_estimators' must be an integer.")
 
         if isinstance(self.n_estimators, int):
             if self.n_estimators <= 0:
                 raise ValueError("'n_estimators' must be greater than zero.")
@@ -170,17 +233,19 @@
 
         if isinstance(self.min_samples_in_leaf, int):
             if self.min_samples_in_leaf <= 0:
                 raise ValueError("'min_samples_in_leaf' must be greater than zero.")
 
         if isinstance(self.max_depth, type(None)):
             pass
+
         elif isinstance(self.max_depth, int):
             if self.max_depth <= 0:
                 raise ValueError("'max_depth' must be an greater than zero.")
+
         else:
             raise TypeError("'max_depth' must be an integer greater than zero or None.")
 
         if not isinstance(self.max_features, float):
             raise TypeError("'max_features' must be float.")
 
         if isinstance(self.max_features, float):
@@ -188,14 +253,15 @@
                 raise ValueError(
                     "'max_features' must be greater than zero but less than or equal to one."
                 )
 
         if isinstance(self.min_gain, float):
             if self.min_gain < 0:
                 raise ValueError("'min_gain' must be greater than or equal to zero.")
+
         else:
             raise TypeError("'min_gain' must be float.")
 
         if isinstance(self.impurity, str):
             if self.impurity not in SUPPORTED_IMPURITY:
                 raise ValueError(
                     "Supplied 'impurity' is not supported. 'impurity' must be 'gain', 'gain-ratio', 'tsallis', or 'tsallis-gain-ratio'."
@@ -229,15 +295,15 @@
 
         if isinstance(self.nnet_min_samples, int):
             if self.nnet_min_samples <= 0:
                 raise ValueError("'nnet_min_samples' must be greater than zero.")
 
         if not isinstance(self.use_etc, bool):
             raise TypeError("'use_etc' must be True or False.")
-            
+
         if isinstance(self.etc_max_depth, int):
             if self.etc_max_depth <= 0:
                 raise ValueError("'etc_max_depth' must be greater than zero.")
 
         else:
             if not isinstance(self.etc_max_depth, type(None)):
                 raise TypeError("'etc_max_depth' must be an integer.")
@@ -255,11 +321,11 @@
         if isinstance(self.n_jobs, int):
             if self.n_jobs <= 0:
                 raise ValueError("'n_jobs' must be greater than zero.")
 
         if isinstance(self.resampler, type(None)):
             pass
 
-        elif hasattr(self.resampler, "fit_transform") == False:
+        elif hasattr(self.resampler, "fit_transform") is False:
             raise ValueError("'resampler' must have a 'fit_transform(X, y)' function.")
 
         return X_conv, y_conv
```

### Comparing `landmarkclassifier-2.0.7/LANDMark/lm_dtree_clfs.py` & `landmarkclassifier-2.1.0/LANDMark/lm_dtree_clfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from sklearn.ensemble import ExtraTreesClassifier
 from sklearn.utils import resample
 
 from math import ceil
 
 import numpy as np
 
+
 class ETClassifier(ClassifierMixin, BaseEstimator):
     def __init__(self, n_feat=0.8, max_depth=5, max_trees=128):
         self.n_feat = n_feat
         self.max_depth = max_depth
         self.max_trees = max_trees
 
     def fit(self, X, y):
@@ -25,30 +26,27 @@
 
         X_re, y_re = resample(X, y, n_samples=X.shape[0], stratify=y)
 
         X_re = X_re[:, self.features]
 
         self.classes_, y_counts = np.unique(y_re, return_counts=True)
 
-        clf_1 = ExtraTreesClassifier(
+        clf = ExtraTreesClassifier(
             n_estimators=self.max_trees, max_depth=self.max_depth
         )
 
         self.model_type = "nonlinear_etc"
 
-        self.clf_model = clf_1.fit(X_re, y_re)
+        self.clf_model = clf.fit(X_re, y_re)
 
         return self, self.decision_function(X)
 
     def predict(self, X):
         return self.clf_model.predict(X[:, self.features])
 
     def predict_proba(self, X):
-
         return self.clf_model.predict_proba(X[:, self.features])
 
     def decision_function(self, X):
         D = self.clf_model.predict_proba(X[:, self.features])
 
         return np.where(D > 0.5, 1, -1)
-
-
```

### Comparing `landmarkclassifier-2.0.7/LANDMark/lm_linear_clfs.py` & `landmarkclassifier-2.1.0/LANDMark/lm_linear_clfs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-import logging
-import os
-
 import warnings
 from sklearn.exceptions import ConvergenceWarning
 
 warnings.filterwarnings("ignore", category=ConvergenceWarning, module="sklearn")
 
 import numpy as np
 
 from sklearn.base import ClassifierMixin, BaseEstimator
 from sklearn.linear_model import (
     RidgeClassifierCV,
     LogisticRegressionCV,
-    LogisticRegression,
     SGDClassifier,
-    RidgeClassifier,
 )
 from sklearn.svm import LinearSVC
-from sklearn.ensemble import ExtraTreesClassifier
 from sklearn.model_selection import GridSearchCV
 from sklearn.utils import resample
-
-from random import choice
+from sklearn.model_selection import StratifiedKFold
 
 from math import ceil
 
 
 class LMClassifier(ClassifierMixin, BaseEstimator):
-    def __init__(self, model_type, n_feat=0.8):
+    def __init__(self, model_type, n_feat=0.8, minority=6, use_etc_split=True):
         self.model_type = model_type
         self.n_feat = n_feat
+        self.minority = minority
 
     def fit(self, X, y):
         if X.shape[1] >= 4:
             self.features = np.random.choice(
                 [i for i in range(X.shape[1])],
                 size=ceil(X.shape[1] * self.n_feat),
                 replace=False,
@@ -44,79 +38,74 @@
 
         X_re, y_re = resample(X, y, n_samples=X.shape[0], stratify=y)
 
         X_re = X_re[:, self.features]
 
         self.classes_, y_counts = np.unique(y_re, return_counts=True)
 
-        self.y_min = min(y_counts)
-        
-        if self.y_min > 6:
+        self.y_min = min(y_counts) * 0.8
+
+        if self.y_min > self.minority:
             if self.model_type == "lr_l2":
-                self.clf = LogisticRegressionCV(max_iter=2000, cv=5).fit(X_re, y_re)
+                self.clf = LogisticRegressionCV(
+                    max_iter=2000, cv=StratifiedKFold(5)
+                ).fit(X_re, y_re)
 
             elif self.model_type == "lr_l1":
                 solver = "liblinear"
                 if X.shape[0] >= 500:
                     solver = "saga"
 
                 self.clf = LogisticRegressionCV(
-                    max_iter=2000, cv=5, solver=solver, penalty="l1"
+                    max_iter=2000, cv=StratifiedKFold(5), solver=solver, penalty="l1"
                 ).fit(X_re, y_re)
 
             elif self.model_type == "sgd_l2":
                 self.cv = GridSearchCV(
                     SGDClassifier(max_iter=2000),
                     param_grid={
                         "alpha": [0.001, 0.01, 0.1, 1.0, 10, 100],
                         "loss": ["hinge", "modified_huber"],
                     },
-                    cv=5,
+                    cv=StratifiedKFold(5),
                 ).fit(X_re, y_re)
 
                 self.clf = self.cv.best_estimator_
 
             elif self.model_type == "sgd_l1":
                 self.cv = GridSearchCV(
                     SGDClassifier(max_iter=2000, penalty="elasticnet"),
                     param_grid={
                         "alpha": [0.001, 0.01, 0.1, 1.0, 10, 100],
                         "loss": ["hinge", "modified_huber"],
                     },
-                    cv=5,
+                    cv=StratifiedKFold(5),
                 ).fit(X_re, y_re)
 
                 self.clf = self.cv.best_estimator_
 
             elif self.model_type == "ridge":
                 self.clf = RidgeClassifierCV(
-                    alphas=(0.001, 0.01, 0.1, 1.0, 10, 100, 1000), cv=5
+                    alphas=(0.001, 0.01, 0.1, 1.0, 10, 100, 1000), cv=StratifiedKFold(5)
                 ).fit(X_re, y_re)
 
             elif self.model_type == "lsvc":
                 self.cv = GridSearchCV(
                     LinearSVC(max_iter=2000),
                     param_grid={"C": [0.001, 0.01, 0.1, 1.0, 10, 100]},
-                    cv=5,
+                    cv=StratifiedKFold(5),
                 ).fit(X_re, y_re)
 
                 self.clf = self.cv.best_estimator_
 
-        else:
-            self.clf = ExtraTreesClassifier(n_estimators = 128, max_depth = 1)
-            
-            self.clf.fit(X_re, y_re)
+            return self, self.decision_function(X)
 
-        return self, self.decision_function(X)
+        # Otherwise use an Extra Trees Classifier or Nothing
+        else:
+            return self, None
 
     def predict(self, X):
         return self.clf.predict(X[:, self.features])
 
     def decision_function(self, X):
-        
-        if self.y_min > 6:
-            return self.clf.decision_function(X[:, self.features])
-
-        else:
-            D = self.clf.predict_proba(X[:, self.features])
+        return self.clf.decision_function(X[:, self.features])
 
-            return np.where(D > 0.5, 1, -1)
```

### Comparing `landmarkclassifier-2.0.7/LANDMark/lm_nnet_clfs.py` & `landmarkclassifier-2.1.0/LANDMark/lm_nnet_clfs.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,37 +6,46 @@
 
 import numpy as np
 
 import torch as pyt
 
 from skorch import NeuralNetClassifier
 
+from scipy.sparse import issparse
+
+
 class LMNNet(pyt.nn.Module):
     def __init__(self, n_in, n_out):
         super(LMNNet, self).__init__()
 
         self.n_in = n_in
         self.n_out = n_out
 
-        self.IN = pyt.nn.Linear(in_features = self.n_in, out_features = self.n_out * 32)
-        self.IN_Dr = pyt.nn.Dropout(0.5)
-        
-        self.D_1 = pyt.nn.Linear(in_features = self.n_out * 32, out_features = self.n_out * 16)
+        self.IN = pyt.nn.Linear(in_features=self.n_in, out_features=self.n_out * 32)
+        self.A_1 = pyt.nn.Mish()
+        self.IN_Dr = pyt.nn.Dropout(0.375)
+
+        self.D_1 = pyt.nn.Linear(
+            in_features=self.n_out * 32, out_features=self.n_out * 16
+        )
         self.A_1 = pyt.nn.Mish()
         self.Dr_1 = pyt.nn.Dropout(0.375)
 
-        self.D_2 = pyt.nn.Linear(in_features = self.n_out * 16, out_features = self.n_out * 8)
+        self.D_2 = pyt.nn.Linear(
+            in_features=self.n_out * 16, out_features=self.n_out * 16
+        )  # n_out * 8
         self.A_2 = pyt.nn.Mish()
         self.Dr_2 = pyt.nn.Dropout(0.375)
 
-        self.D_3 = pyt.nn.Linear(in_features = self.n_out * 8, out_features = self.n_out)
-        self.O = pyt.nn.Softmax(dim = -1)
+        self.D_3 = pyt.nn.Linear(
+            in_features=self.n_out * 16, out_features=self.n_out
+        )  # in_features = *8
+        self.O = pyt.nn.Softmax(dim=-1)
 
     def forward(self, x):
-
         o = self.IN(x)
         o = self.IN_Dr(o)
         o = self.D_1(o)
         o = self.A_1(o)
         o = self.Dr_1(o)
         o = self.D_2(o)
         o = self.A_2(o)
@@ -44,98 +53,119 @@
         o = self.D_3(o)
         o = self.O(o)
 
         return o
 
 
 class ANNClassifier(ClassifierMixin, BaseEstimator):
-    def __init__(self, n_feat=0.8):
+    def __init__(self, n_feat=0.8, minority=6, use_etc_split=True):
         self.n_feat = n_feat
+        self.minority = minority
 
     def fit(self, X, y):
         self.model_type = "nonlinear_nnet"
 
-        self.classes_, _ = np.unique(y, return_counts=True)
+        if issparse(X):
+            X_not_sparse = X.toarray()
 
+        else:
+            X_not_sparse = X
+
+        # Encode y
         self.y_transformer = LabelEncoder().fit(y)
 
-        if X.shape[1] >= 4:
+        # Select features
+        if X_not_sparse.shape[1] >= 4:
             self.features = np.random.choice(
-                [i for i in range(X.shape[1])],
-                size=ceil(X.shape[1] * self.n_feat),
+                [i for i in range(X_not_sparse.shape[1])],
+                size=ceil(X_not_sparse.shape[1] * self.n_feat),
                 replace=False,
             )
 
         else:
-            self.features = np.asarray([i for i in range(X.shape[1])])
+            self.features = np.asarray([i for i in range(X_not_sparse.shape[1])])
 
-        X_trf, y_trf = resample(X[:, self.features], y, n_samples=X.shape[0], stratify=y)
+        # Bootstrap resample
+        X_trf, y_trf = resample(
+            X_not_sparse[:, self.features],
+            y,
+            n_samples=X_not_sparse.shape[0],
+            stratify=y,
+        )
         X_trf = X_trf.astype(np.float32)
         y_trf = self.y_transformer.transform(y_trf).astype(np.int64)
 
-        self.n_in = X_trf.shape[1]
-        self.n_out = self.classes_.shape[0]
+        # Determine if minimum class count exists
+        self.classes_, y_counts = np.unique(y_trf, return_counts=True)
 
-        if pyt.cuda.is_available():
-            device = "cuda"
-        else:
-            device = "cpu"
+        self.y_min = min(y_counts) * 0.8
+
+        # Use neural network if more than 6 samples are present in the minority class
+        if self.y_min > self.minority:
+            self.n_in = X_trf.shape[1]
+            self.n_out = self.classes_.shape[0]
+
+            if pyt.cuda.is_available():
+                device = "cuda"
+            else:
+                device = "cpu"
+
+            clf = NeuralNetClassifier(
+                LMNNet(n_in=X_trf.shape[1], n_out=self.classes_.shape[0]),
+                optimizer=pyt.optim.AdamW,
+                lr=0.001,
+                max_epochs=100,
+                batch_size=16,
+                device=device,
+                iterator_train__shuffle=True,
+                verbose=0,
+            )
+
+            clf.fit(X_trf, y_trf)
 
-        clf = NeuralNetClassifier(LMNNet(n_in = X_trf.shape[1], n_out = self.classes_.shape[0]),
-                             optimizer = pyt.optim.AdamW,
-                             lr = 0.001,
-                             max_epochs = 100,
-                             batch_size = 16,
-                             device = device,
-                             iterator_train__shuffle=True,
-                             verbose = 0
-                             )
-
-        clf.fit(X_trf, y_trf)
-        
-        self.params = clf.module.state_dict()
+            self.params = clf.module.state_dict()
 
-        with pyt.inference_mode():
-            D = clf.predict_proba(X[:, self.features].astype(np.float32))
+            del clf
 
-            D = np.where(D > 0.5, 1, -1)
+            return self, self.decision_function(X)
 
-        return self, D
+        # Otherwise use an Extra Trees Classifier or Nothing
+        else:
+            return self, None
 
     def predict_proba(self, X):
+        if issparse(X):
+            X_not_sparse = X.toarray()
 
-        if pyt.cuda.is_available():
-            device = "cuda"
         else:
-            device = "cpu"
+            X_not_sparse = X
+
+        clf = LMNNet(n_in=self.n_in, n_out=self.n_out)
+
+        clf.load_state_dict(self.params)
 
-        clf = NeuralNetClassifier(LMNNet(n_in = self.n_in, n_out = self.n_out),
-                                  optimizer = pyt.optim.AdamW,
-                                  optimizer__lr = 0.001,
-                                  max_epochs = 100,
-                                  batch_size = 16,
-                                  device = device
-                                  )
+        n_batch = pyt.arange(0, len(X_not_sparse), 16)
 
-        clf.module.load_state_dict(self.params)
+        X_tensor = pyt.tensor(X_not_sparse[:, self.features].astype(np.float32))
 
-        clf.initialize()
+        predictions = []
+        for start in n_batch:
+            p = clf(X_tensor[start : start + 16]).detach().cpu().numpy()
+            predictions.extend(p)
 
-        with pyt.inference_mode():
-            predictions = clf.predict_proba(X[:, self.features].astype(np.float32))
+        predictions = np.asarray(predictions)
+
+        del clf
 
         return predictions
 
     def decision_function(self, X):
-
         D = self.predict_proba(X)
 
         return np.where(D > 0.5, 1, -1)
 
     def predict(self, X):
-
         predictions = self.predict_proba(X)
 
-        predictions = np.argmax(predictions, axis = 1)
+        predictions = np.argmax(predictions, axis=1)
 
         return self.y_transformer.inverse_transform(predictions)
-
```

### Comparing `landmarkclassifier-2.0.7/LANDMark/lm_oracle_clfs.py` & `landmarkclassifier-2.1.0/LANDMark/lm_oracle_clfs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,72 @@
 import numpy as np
 
 from math import ceil
 
 from sklearn.base import ClassifierMixin, BaseEstimator
 
+from scipy.sparse import issparse
+
 
 class RandomOracle(ClassifierMixin, BaseEstimator):
     def __init__(self, oracle="Linear", n_feat=0.8):
         self.oracle = "Linear"
         self.n_feat = n_feat
 
     def fit(self, X, y):
-        if X.shape[1] >= 4:
+        if issparse(X):
+            X_not_sparse = X.toarray()
+
+        else:
+            X_not_sparse = X
+
+        if X_not_sparse.shape[1] >= 4:
             self.features = np.random.choice(
-                [i for i in range(X.shape[1])],
-                size=ceil(X.shape[1] * self.n_feat),
+                [i for i in range(X_not_sparse.shape[1])],
+                size=ceil(X_not_sparse.shape[1] * self.n_feat),
                 replace=False,
             )
 
         else:
-            self.features = np.asarray([i for i in range(X.shape[1])])
+            self.features = np.asarray([i for i in range(X_not_sparse.shape[1])])
 
         if self.oracle == "Linear":
             # Select two points at random
             index = np.random.choice(
-                [i for i in range(X.shape[0])], size=2, replace=False
+                [i for i in range(X_not_sparse.shape[0])], size=2, replace=False
             )
-            x = X[index]
+            x = X_not_sparse[index]
 
             # Make sure two unique instances are chosen
             while np.array_equal(x[0, self.features], x[1, self.features]):
                 index = np.random.choice(
-                    [i for i in range(X.shape[0])], size=2, replace=False
+                    [i for i in range(X_not_sparse.shape[0])], size=2, replace=False
                 )
-                x = X[index]
+                x = X_not_sparse[index]
 
             # Find the midpoint
             midpoint = np.sum(x[:, self.features], axis=0) * 0.5
 
             # Find the normal vector and intercept
             self.weights = x[1, self.features] - x[0, self.features]
             self.intercept = 0 - np.dot(self.weights.T, midpoint)
 
         return self
 
     def decision_function(self, X):
+        if issparse(X):
+            X_not_sparse = X.toarray()
+
+        else:
+            X_not_sparse = X
+
         if self.oracle == "Linear":
-            predictions = np.dot(X[:, self.features], self.weights.T) + self.intercept
+            predictions = (
+                np.dot(X_not_sparse[:, self.features], self.weights.T) + self.intercept
+            )
 
         return predictions
 
     def predict(self, X):
         predictions = np.where(self.decision_function(X) > 0, 1, -1)
 
         return predictions
```

### Comparing `landmarkclassifier-2.0.7/LANDMark/tree.py` & `landmarkclassifier-2.1.0/LANDMark/tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -116,22 +116,25 @@
         max_depth,
         max_features,
         min_gain,
         impurity,
         q,
         use_lm_l2,
         use_lm_l1,
+        minority_sz_lm,
         use_nnet,
         nnet_min_samples,
+        minority_sz_nnet,
         use_etc,
         etc_max_depth,
         etc_max_trees,
         N,
         current_depth,
-        use_oracle
+        use_oracle,
+        use_cascade,
     ):
         # Get the ID of the node
         self.node_id = id(self)
 
         # Prepare the list of hyperplanes, gains, and model types
         hyperplane_list = []
         gains = []
@@ -164,31 +167,34 @@
             leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
 
             self.label = leaf_predictions.predict
             self.terminal = True
 
             return self
 
-        if isinstance(max_depth, int):
-            if current_depth >= max_depth:
-                leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
+        if not isinstance(max_depth, type(None)) and current_depth >= max_depth:
+            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
 
-                self.label = leaf_predictions.predict
-                self.terminal = True
+            self.label = leaf_predictions.predict
+            self.terminal = True
 
-                return self
+            return self
 
         # Otherwise split
         else:
             # Create a Random Oracle Splitter
             if use_oracle:
                 self.splitter = RandomOracle(n_feat=max_features).fit(X, y)
 
                 D = self.splitter.decision_function(X)
 
+                # Extend X using the output of the decision function, D, if the cascade parameter is True
+                if use_cascade:
+                    X = np.hstack((X, D.reshape(-1, 1)))
+
                 L = np.where(D > 0, True, False)
                 R = np.where(D <= 0, True, False)
 
                 IG = purity_function(counts_sum, counts_prob, L, R, y, impurity, q)
 
                 self.gain = IG
 
@@ -200,113 +206,120 @@
                     max_depth=max_depth,
                     max_features=max_features,
                     min_gain=min_gain,
                     impurity=impurity,
                     q=q,
                     use_lm_l2=use_lm_l2,
                     use_lm_l1=use_lm_l1,
+                    minority_sz_lm=minority_sz_lm,
                     use_nnet=use_nnet,
                     nnet_min_samples=nnet_min_samples,
+                    minority_sz_nnet=minority_sz_nnet,
                     use_etc=use_etc,
                     etc_max_depth=etc_max_depth,
                     etc_max_trees=etc_max_trees,
                     N=X.shape[0],
                     current_depth=current_depth + 1,
                     use_oracle=False,
+                    use_cascade=use_cascade,
                 )
 
                 self.right = Node().get_split(
                     X[R],
                     y[R],
                     min_samples_in_leaf=min_samples_in_leaf,
                     max_depth=max_depth,
                     max_features=max_features,
                     min_gain=min_gain,
                     impurity=impurity,
                     q=q,
                     use_lm_l2=use_lm_l2,
                     use_lm_l1=use_lm_l1,
+                    minority_sz_lm=minority_sz_lm,
                     use_nnet=use_nnet,
                     nnet_min_samples=nnet_min_samples,
+                    minority_sz_nnet=minority_sz_nnet,
                     use_etc=use_etc,
                     etc_max_depth=etc_max_depth,
                     etc_max_trees=etc_max_trees,
                     N=X.shape[0],
                     current_depth=current_depth + 1,
                     use_oracle=False,
+                    use_cascade=use_cascade,
                 )
 
                 return self
 
-            # Split using a Linear or Neural Network Models
+            # Split using a Linear, Tree, or Neural Network Models
             else:
                 self.c_choice = choice([i for i in range(outcomes.shape[0])])
 
                 # Train Linear Models - L2
                 if use_lm_l2:
                     for clf in [
-                        LMClassifier(model_type="lr_l2", n_feat=max_features),
-                        LMClassifier(model_type="sgd_l2", n_feat=max_features),
-                        LMClassifier(model_type="ridge", n_feat=max_features),
-                        LMClassifier(model_type="lsvc", n_feat=max_features),
+                        LMClassifier(
+                            model_type="lr_l2",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                        LMClassifier(
+                            model_type="sgd_l2",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                        LMClassifier(
+                            model_type="ridge",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                        LMClassifier(
+                            model_type="lsvc",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
                     ]:
                         model, D = clf.fit(X, y)
 
-                        if D.ndim > 1:
-                            D = D[:, self.c_choice]
+                        if not isinstance(D, type(None)):
+                            if D.ndim > 1:
+                                D = D[:, self.c_choice]
 
-                        L = np.where(D > 0, True, False)
-                        R = np.where(D <= 0, True, False)
+                            L = np.where(D > 0, True, False)
+                            R = np.where(D <= 0, True, False)
 
-                        X_L_n = X[L].shape[0]
-                        X_R_n = X[R].shape[0]
+                            X_L_n = X[L].shape[0]
+                            X_R_n = X[R].shape[0]
 
-                        # Calculate Information Gain
-                        if X_L_n > 0 and X_R_n > 0:
-                            IG = purity_function(
-                                counts_sum, counts_prob, L, R, y, impurity, q
-                            )
+                            # Calculate Information Gain
+                            if X_L_n > 0 and X_R_n > 0:
+                                IG = purity_function(
+                                    counts_sum, counts_prob, L, R, y, impurity, q
+                                )
 
-                            gains.append(IG)
-                            hyperplane_list.append((model, L, R))
-                            model_type.append(model.model_type)
+                                gains.append(IG)
+                                hyperplane_list.append((model, L, R))
+                                model_type.append(model.model_type)
 
                 # Train Linear Models - L1 / ElasticNet
                 if use_lm_l1:
                     for clf in [
-                        LMClassifier(model_type="lr_l1", n_feat=max_features),
-                        LMClassifier(model_type="sgd_l1", n_feat=max_features),
+                        LMClassifier(
+                            model_type="lr_l1",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                        LMClassifier(
+                            model_type="sgd_l1",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
                     ]:
                         model, D = clf.fit(X, y)
 
-                        if D.ndim > 1:
-                            D = D[:, self.c_choice]
-
-                        L = np.where(D > 0, True, False)
-                        R = np.where(D <= 0, True, False)
-
-                        X_L_n = X[L].shape[0]
-                        X_R_n = X[R].shape[0]
-
-                        # Calculate Information Gain
-                        if X_L_n > 0 and X_R_n > 0:
-                            IG = purity_function(
-                                counts_sum, counts_prob, L, R, y, impurity, q
-                            )
-
-                            gains.append(IG)
-                            hyperplane_list.append((model, L, R))
-                            model_type.append(model.model_type)
-
-                # Train a Neural Network
-                if use_nnet:
-                    if X.shape[0] >= nnet_min_samples:
-                        for clf in [ANNClassifier(n_feat=max_features)]:
-                            model, D = clf.fit(X, y)
-
+                        if not isinstance(D, type(None)):
                             if D.ndim > 1:
                                 D = D[:, self.c_choice]
 
                             L = np.where(D > 0, True, False)
                             R = np.where(D <= 0, True, False)
 
                             X_L_n = X[L].shape[0]
@@ -318,43 +331,75 @@
                                     counts_sum, counts_prob, L, R, y, impurity, q
                                 )
 
                                 gains.append(IG)
                                 hyperplane_list.append((model, L, R))
                                 model_type.append(model.model_type)
 
+                # Train a Neural Network
+                if use_nnet:
+                    if X.shape[0] >= nnet_min_samples:
+                        for clf in [
+                            ANNClassifier(
+                                n_feat=max_features,
+                                minority=minority_sz_nnet,
+                            )
+                        ]:
+                            model, D = clf.fit(X, y)
+
+                            if not isinstance(D, type(None)):
+                                if D.ndim > 1:
+                                    D = D[:, self.c_choice]
+
+                                L = np.where(D > 0, True, False)
+                                R = np.where(D <= 0, True, False)
+
+                                X_L_n = X[L].shape[0]
+                                X_R_n = X[R].shape[0]
+
+                                # Calculate Information Gain
+                                if X_L_n > 0 and X_R_n > 0:
+                                    IG = purity_function(
+                                        counts_sum, counts_prob, L, R, y, impurity, q
+                                    )
+
+                                    gains.append(IG)
+                                    hyperplane_list.append((model, L, R))
+                                    model_type.append(model.model_type)
+
                 # Train Decision Tree Models
                 if use_etc:
                     for clf in [
                         ETClassifier(
                             n_feat=max_features,
                             max_depth=etc_max_depth,
                             max_trees=etc_max_trees,
                         )
                     ]:
                         model, D = clf.fit(X, y)
 
-                        if D.ndim > 1:
-                            D = D[:, self.c_choice]
+                        if not isinstance(D, type(None)):
+                            if D.ndim > 1:
+                                D = D[:, self.c_choice]
 
-                        L = np.where(D > 0, True, False)
-                        R = np.where(D <= 0, True, False)
+                            L = np.where(D > 0, True, False)
+                            R = np.where(D <= 0, True, False)
 
-                        X_L_n = X[L].shape[0]
-                        X_R_n = X[R].shape[0]
+                            X_L_n = X[L].shape[0]
+                            X_R_n = X[R].shape[0]
 
-                        # Calculate Information Gain
-                        if X_L_n > 0 and X_R_n > 0:
-                            IG = purity_function(
-                                counts_sum, counts_prob, L, R, y, impurity, q
-                            )
+                            # Calculate Information Gain
+                            if X_L_n > 0 and X_R_n > 0:
+                                IG = purity_function(
+                                    counts_sum, counts_prob, L, R, y, impurity, q
+                                )
 
-                            gains.append(IG)
-                            hyperplane_list.append((model, L, R))
-                            model_type.append(model.model_type)
+                                gains.append(IG)
+                                hyperplane_list.append((model, L, R))
+                                model_type.append(model.model_type)
 
                 gains = np.asarray(gains)
                 hyperplane_list = np.asarray(hyperplane_list, dtype="object")
                 model_type = np.asarray(model_type, dtype=np.str)
 
                 # Ensure that there is at least one set of splits that meets the minimum gain criteria
                 gain_mask = np.where(gains >= min_gain, True, False)
@@ -371,55 +416,77 @@
                     best_hyperplane = choice(hyperplane_list)
                     L = best_hyperplane[1]
                     R = best_hyperplane[2]
 
                     self.gain = best_gain
                     self.splitter = best_hyperplane[0]
 
+                    # Append the output of the decision function to each dataframe
+                    if use_cascade:
+                        if isinstance(self.splitter, LMClassifier):
+                            X_cascade = self.splitter.decision_function(X)
+
+                            if X_cascade.ndim == 1:
+                                X_cascade = X_cascade.reshape(-1, 1)
+
+                        else:
+                            X_cascade = self.splitter.predict_proba(X)
+
+                        X_new = np.hstack((X, X_cascade))
+
+                    else:
+                        X_new = X
+
                     # Recursivly split
                     self.left = Node().get_split(
-                        X[L],
+                        X_new[L],
                         y[L],
                         min_samples_in_leaf=min_samples_in_leaf,
                         max_depth=max_depth,
                         max_features=max_features,
                         min_gain=min_gain,
                         impurity=impurity,
                         q=q,
                         use_lm_l2=use_lm_l2,
                         use_lm_l1=use_lm_l1,
+                        minority_sz_lm=minority_sz_lm,
                         use_nnet=use_nnet,
                         nnet_min_samples=nnet_min_samples,
+                        minority_sz_nnet=minority_sz_nnet,
                         use_etc=use_etc,
                         etc_max_depth=etc_max_depth,
                         etc_max_trees=etc_max_trees,
                         N=X.shape[0],
                         current_depth=current_depth + 1,
                         use_oracle=use_oracle,
+                        use_cascade=use_cascade,
                     )
 
                     self.right = Node().get_split(
-                        X[R],
+                        X_new[R],
                         y[R],
                         min_samples_in_leaf=min_samples_in_leaf,
                         max_depth=max_depth,
                         max_features=max_features,
                         min_gain=min_gain,
                         impurity=impurity,
                         q=q,
                         use_lm_l2=use_lm_l2,
                         use_lm_l1=use_lm_l1,
+                        minority_sz_lm=minority_sz_lm,
                         use_nnet=use_nnet,
                         nnet_min_samples=nnet_min_samples,
+                        minority_sz_nnet=minority_sz_nnet,
                         use_etc=use_etc,
                         etc_max_depth=etc_max_depth,
                         etc_max_trees=etc_max_trees,
                         N=X.shape[0],
                         current_depth=current_depth + 1,
                         use_oracle=use_oracle,
+                        use_cascade=use_cascade,
                     )
 
                     return self
 
                 # Create a Leaf
                 else:
                     leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
@@ -438,36 +505,42 @@
         max_features,
         min_gain,
         impurity,
         q,
         use_oracle,
         use_lm_l2,
         use_lm_l1,
+        minority_sz_lm,
         use_nnet,
         nnet_min_samples,
+        minority_sz_nnet,
         use_etc,
         etc_max_depth,
         etc_max_trees,
         resampler,
+        use_cascade,
     ):
         self.min_samples_in_leaf = min_samples_in_leaf
         self.max_depth = max_depth
         self.max_features = max_features
         self.min_gain = min_gain
         self.impurity = impurity
         self.q = q
         self.use_oracle = use_oracle
         self.use_lm_l2 = use_lm_l2
         self.use_lm_l1 = use_lm_l1
+        self.minority_sz_lm = minority_sz_lm
         self.use_nnet = use_nnet
         self.nnet_min_samples = nnet_min_samples
+        self.minority_sz_nnet = minority_sz_nnet
         self.use_etc = use_etc
         self.etc_max_depth = etc_max_depth
         self.etc_max_trees = etc_max_trees
         self.resampler = resampler
+        self.use_cascade = use_cascade
 
     def fit(self, X, y):
         self.classes_ = np.unique(y)
 
         # Increase diversity by resampling
         if isinstance(self.resampler, type(None)):
             X_re = X
@@ -489,83 +562,91 @@
             max_depth=self.max_depth,
             max_features=self.max_features,
             min_gain=self.min_gain,
             impurity=self.impurity,
             q=self.q,
             use_lm_l2=self.use_lm_l2,
             use_lm_l1=self.use_lm_l1,
+            minority_sz_lm=self.minority_sz_lm,
             use_nnet=self.use_nnet,
             nnet_min_samples=self.nnet_min_samples,
+            minority_sz_nnet=self.minority_sz_nnet,
             use_etc=self.use_etc,
             etc_max_depth=self.etc_max_depth,
             etc_max_trees=self.etc_max_trees,
             N=X.shape[0],
             current_depth=1,
             use_oracle=self.use_oracle,
+            use_cascade=self.use_cascade,
         )
 
         self.LMTree = tree
 
-        # Find all Node Ids
-        self.all_ids = list(set(self._get_node_ids(self.LMTree)))
-
-        return self
+        self.all_nodes = self._get_all_nodes(self.LMTree)
 
-    def _get_node_ids(self, node):
-        ids = []
-
-        if node.terminal is False:
-            ids.extend(self._get_node_ids(node.left))
-            ids.extend(self._get_node_ids(node.right))
-
-        else:
-            ids.append(node.node_id)
+        self.terminal_nodes = [x[0] for x in self.all_nodes if x[1] == 1]
+        self.all_nodes = [x[0] for x in self.all_nodes]
 
-        return ids
+        return self
 
     def _predict(self, X, current_node=None, samp_idx=None):
         final_predictions = []
 
         # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
         if isinstance(samp_idx, type(None)):
             samp_idx = np.asarray([i for i in range(X.shape[0])])
 
             current_node = self.LMTree
 
         if current_node.terminal is False:
-
+            # Determine where each sample goes
             D = current_node.splitter.decision_function(X)
 
             if D.ndim > 1:
                 D = D[:, current_node.c_choice]
 
             L = np.where(D > 0, True, False)
             R = np.where(D <= 0, True, False)
 
-            X_L = X[L]
+            # Append decision function data
+            if self.use_cascade:
+                if isinstance(current_node.splitter, LMClassifier) or isinstance(
+                    current_node.splitter, RandomOracle
+                ):
+                    C = current_node.splitter.decision_function(X)
+
+                    if C.ndim == 1:
+                        C = C.reshape(-1, 1)
+
+                else:
+                    C = current_node.splitter.predict_proba(X)
+
+                X_new = np.hstack((X, C))
+
+            else:
+                X_new = X
+
+            X_L = X_new[L]
             left = samp_idx[L]
 
-            X_R = X[R]
+            X_R = X_new[R]
             right = samp_idx[R]
 
             if left.shape[0] > 0:
                 predictions_left = self._predict(X_L, current_node.left, left)
                 final_predictions.extend(predictions_left)
 
             if right.shape[0] > 0:
                 predictions_right = self._predict(X_R, current_node.right, right)
                 final_predictions.extend(predictions_right)
 
         elif current_node.terminal:
             predictions = current_node.label(X)
             predictions = np.asarray(
-                [
-                    (samp_idx[i], prediction)
-                    for i, prediction in enumerate(predictions)
-                ]
+                [(samp_idx[i], prediction) for i, prediction in enumerate(predictions)]
             )
 
             return predictions
 
         return final_predictions
 
     def predict(self, X):
@@ -583,39 +664,72 @@
         return np.asarray(tree_predictions)[:, 1]
 
     def score(self, X, y):
         score = balanced_accuracy_score(y, self.predict(X))
 
         return score
 
+    def _get_all_nodes(self, node):
+        node_list = set()
+
+        if node.terminal is False:
+            node_list.update([(node.node_id, 0)])
+
+            node_list = node_list.union(self._get_all_nodes(node.left))
+            node_list = node_list.union(self._get_all_nodes(node.right))
+
+        elif node.terminal:
+            node_list.update([(node.node_id, 1)])
+
+            return node_list
+
+        return node_list
+
     def _proximity(self, X, current_node=None, samp_idx=None):
         final_predictions = []
 
         # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
         if isinstance(samp_idx, type(None)):
             samp_idx = np.asarray([i for i in range(X.shape[0])])
 
             current_node = self.LMTree
 
         # Check if the node is a terminal node
         if current_node.terminal is False:
-
-            # Determine splits
+            # Determine where each sample goes
             D = current_node.splitter.decision_function(X)
 
             if D.ndim > 1:
                 D = D[:, current_node.c_choice]
 
             L = np.where(D > 0, True, False)
             R = np.where(D <= 0, True, False)
 
-            X_L = X[L]
+            # Append decision function data
+            if self.use_cascade:
+                if isinstance(current_node.splitter, LMClassifier) or isinstance(
+                    current_node.splitter, RandomOracle
+                ):
+                    C = current_node.splitter.decision_function(X)
+
+                    if C.ndim == 1:
+                        C = C.reshape(-1, 1)
+
+                else:
+                    C = current_node.splitter.predict_proba(X)
+
+                X_new = np.hstack((X, C))
+
+            else:
+                X_new = X
+
+            X_L = X_new[L]
             left = samp_idx[L]
 
-            X_R = X[R]
+            X_R = X_new[R]
             right = samp_idx[R]
 
             if left.shape[0] > 0:
                 predictions_left = self._proximity(X_L, current_node.left, left)
                 final_predictions.extend(predictions_left)
 
             if right.shape[0] > 0:
@@ -623,29 +737,107 @@
                 final_predictions.extend(predictions_right)
 
         elif current_node.terminal:
             return [(entry, current_node.node_id) for entry in samp_idx]
 
         return final_predictions
 
-    def proximity(self, X):
+    def _proximity_path(self, X, current_node=None, samp_idx=None):
+        final_predictions = []
+
+        # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
+        if isinstance(samp_idx, type(None)):
+            samp_idx = np.asarray([i for i in range(X.shape[0])])
+
+            current_node = self.LMTree
+
+        # Check if the node is a terminal node
+        if current_node.terminal is False:
+            # Determine where each sample goes
+            D = current_node.splitter.decision_function(X)
+
+            if D.ndim > 1:
+                D = D[:, current_node.c_choice]
+
+            L = np.where(D > 0, True, False)
+            R = np.where(D <= 0, True, False)
+
+            # Append decision function data
+            if self.use_cascade:
+                if isinstance(current_node.splitter, LMClassifier) or isinstance(
+                    current_node.splitter, RandomOracle
+                ):
+                    C = current_node.splitter.decision_function(X)
+
+                    if C.ndim == 1:
+                        C = C.reshape(-1, 1)
+
+                else:
+                    C = current_node.splitter.predict_proba(X)
+
+                X_new = np.hstack((X, C))
+
+            else:
+                X_new = X
+
+            X_L = X_new[L]
+            left = samp_idx[L]
+
+            X_R = X_new[R]
+            right = samp_idx[R]
+
+            if left.shape[0] > 0:
+                final_predictions.extend(
+                    [(entry, current_node.node_id) for entry in samp_idx[L]]
+                )
+                predictions_left = self._proximity_path(X_L, current_node.left, left)
+                final_predictions.extend(predictions_left)
+
+            if right.shape[0] > 0:
+                final_predictions.extend(
+                    [(entry, current_node.node_id) for entry in samp_idx[R]]
+                )
+                predictions_right = self._proximity_path(X_R, current_node.right, right)
+                final_predictions.extend(predictions_right)
+
+        elif current_node.terminal:
+            return [(entry, current_node.node_id) for entry in samp_idx]
+
+        return final_predictions
+
+    def proximity(self, X, prox_type="path"):
         if hasattr(self.resampler, "transform"):
             X_trf = self.resampler.transform(X)
 
         else:
             X_trf = X
 
-        tree_predictions = self._proximity(X_trf)
+        if prox_type == "terminal":
+            tree_predictions = self._proximity(X_trf)
 
-        tree_predictions.sort()
+            tree_predictions.sort()
+
+            col_dict = {col: i for i, col in enumerate(self.terminal_nodes)}
+
+            emb_matrix = np.zeros(
+                shape=(X.shape[0], len(self.terminal_nodes)), dtype=np.ushort
+            )
+
+            for entry in tree_predictions:
+                row = entry[0]
+                col = col_dict[entry[1]]
+
+                emb_matrix[row, col] = 1
 
-        col_dict = {col: i for i, col in enumerate(self.all_ids)}
+            return emb_matrix
 
-        emb_matrix = np.zeros(shape=(X.shape[0], len(self.all_ids)), dtype=np.ushort)
+        elif prox_type == "path":
+            tree_predictions = self._proximity_path(X_trf)
 
-        for entry in tree_predictions:
-            row = entry[0]
-            col = col_dict[entry[1]]
+            emb_matrix = {}
+            for sample in tree_predictions:
+                if sample[0] not in emb_matrix:
+                    emb_matrix[sample[0]] = set()
 
-            emb_matrix[row, col] = 1
+                emb_matrix[sample[0]].add(sample[1])
 
-        return emb_matrix
+            return emb_matrix
```

### Comparing `landmarkclassifier-2.0.7/LANDMark/utils.py` & `landmarkclassifier-2.1.0/LANDMark/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 
         return predictions
 
     def predict_proba(self, X):
         class_map = {class_name: i for i, class_name in enumerate(self.classes_)}
 
         # Returns an array that of shape (n_estimators, n_samples)
-        prediction_results = Parallel(self.n_jobs)(
-            delayed(self.estimators_[i].predict)(X) for i in range(self.n_estimators)
-        )
+        prediction_results = [
+            self.estimators_[i].predict(X) for i in range(self.n_estimators)
+        ]
 
         prediction_results = np.asarray(prediction_results)
 
         # Create an array that will hold all probabilities
         prediction_probs = np.zeros(
             shape=(X.shape[0], self.classes_.shape[0]), dtype=float
         )
@@ -70,8 +70,8 @@
                 for idx, prob in enumerate(probs):
                     index = class_map[class_names[idx]]
                     prediction_probs[sample_num, index] = prob
 
         # Ensure all probabilities sum to one
         prediction_probs = softmax(prediction_probs, axis=1)
 
-        return prediction_probs
+        return prediction_probs
```

### Comparing `landmarkclassifier-2.0.7/docs/API.md` & `landmarkclassifier-2.1.0/docs/API.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 ## Overview of Section
 
 This section provides an overview of the `LANDMark` and the different parameters
 of the `LANDMark` class and its methods.
 
 ## Class
 
-    class LANDMark.LANDMark(n_estimators, min_samples_in_leaf, max_depth, max_features, min_gain, impurity, use_oracle, use_lm_l2, use_lm_l1, 
-        use_nnet, nnet_min_samples, use_etc, etc_max_depth = 5, etc_max_trees = 128, max_samples_tree, bootstrap, n_jobs = 4)
+    class LANDMark.LANDMark(n_estimators, min_samples_in_leaf, max_depth, max_features, min_gain, impurity, q, use_oracle, 
+        use_lm_l2, use_lm_l1, use_nnet, nnet_min_samples, use_etc, etc_max_depth = 5, etc_max_trees = 128, resampler = None,
+        use_cascade = False, n_jobs = 4)
 
 ### Parameters
 
 ### Class Parameters
     n_estimators: int, default = 64
         The number of trees used to construct the ensemble.
 
     min_samples_in_leaf: int, default = 5
         The minimum number of samples in each leaf to proceed to cutting.
         
-    max_depth: int, default = -1
-        The maximum depth of the tree. '-1' implies that trees will fully
+    max_depth: Optional[int], default = None
+        The maximum depth of the tree. 'None' implies that trees will fully
         grow until a stopping criterion is met.
         
     max_features: float, default = 0.80
         The maximum features used to train each model at each node. These
         features are randomly selected at each node.
         
     min_gain: float, default = 0.0
@@ -64,24 +65,25 @@
     etc_max_depth: int, default = 5
         Specifies the maximum depth of each ExtraTreesClassifier. Only used
         if 'use_etc' is set to True.
 
     etc_max_trees: int, default = 128
         Specifies the maximum depth of trees used to train each ExtraTreesClassifier. 
         Only used if 'use_etc' is set to True.
-        
-    max_samples_tree: int, default = -1
-        Specifies the maximum number of samples used to construct each tree.
-        A stratified random sample is chosen to construct each tree. If '-1'
-        is selected, all samples are chosen.
-        
+                
     resampler: The resampling object. Cloning of the object must be possible and,
         at a minimum, the object must have a 'fit_resample(X, y)' method. The
         resampling object can also have a 'transform(X)' method if a user-defined
         transformation occurs during fitting.
+
+    use_cascade: bool, default = False
+        This parameter extends 'X' using the information returned by the best decision
+        function within each node. By doing this, information about the split is
+        retained and has the potential to be used within deeper nodes of the tree.
+        The inspiration for this idea comes from: https://www.ijcai.org/proceedings/2017/0497.pdf
         
     n_jobs: int, default = 4
         The number of processes used to create the LANDMark model.
             
 
 ### Attributes
```

### Comparing `landmarkclassifier-2.0.7/docs/CONTRIBUTING.md` & `landmarkclassifier-2.1.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.7/tests/test_landmark.py` & `landmarkclassifier-2.1.0/tests/test_landmark.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,70 @@
 from LANDMark import LANDMarkClassifier
 from LANDMark.lm_nnet_clfs import ANNClassifier
 from LANDMark.lm_linear_clfs import LMClassifier
 from LANDMark.lm_oracle_clfs import RandomOracle
 from LANDMark.lm_dtree_clfs import ETClassifier
 
-from sklearn.datasets import load_wine
+from sklearn.datasets import load_wine, load_breast_cancer
 from sklearn.preprocessing import StandardScaler
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import balanced_accuracy_score
 
 from pathlib import Path
 
 dirpath = Path(__file__).parent
 
 # Tests the transformer modules
 def test_landmark():
 
     # Create the dataset
-    X, y = load_wine(return_X_y = True)
+    X, y = load_breast_cancer(return_X_y = True)
 
     # Split into train and test sets
     X_train, X_test, y_train, y_test = train_test_split(
         X, y, test_size=0.2, random_state=0, stratify=y
     )
 
     # Standardize
     X_trf = StandardScaler()
     X_trf.fit(X_train)
 
     X_train = X_trf.transform(X_train)
     X_test = X_trf.transform(X_test)
 
-    # Setup a LANDMark model and fit
-    clf = LANDMarkClassifier(n_estimators = 16, n_jobs = 2, min_samples_in_leaf = 2)
+    # Setup a LANDMark model and fit (With Cascade)
+    clf = LANDMarkClassifier(n_estimators = 16, n_jobs = 4, min_samples_in_leaf = 2, use_cascade = True)
     clf.fit(X_train, y_train)
 
     # Make a prediction
     predictions = clf.predict(X_test)
 
     # Score
+    BAccC = clf.score(X_test, y_test)
+    assert BAccC >= 0.85
+
+    # Get proximity - Test Logic
+    clf.proximity(X_train, "terminal")
+    clf.proximity(X_train, "path")
+
+    # Setup a LANDMark model and fit (Without Cascade)
+    clf = LANDMarkClassifier(n_estimators = 16, n_jobs = 4, min_samples_in_leaf = 2, use_cascade = False)
+    clf.fit(X_train, y_train)
+
+    # Make a prediction
+    clf.predict(X_test)
+
+    # Score
     BAcc = clf.score(X_test, y_test)
     assert BAcc >= 0.85
 
     # Get proximity
-    prox = clf.proximity(X_train)
+    clf.proximity(X_train, "terminal")
+    clf.proximity(X_train, "path")
+
 
 def test_models():
 
     # Create the dataset
     X, y = load_wine(return_X_y = True)
 
     # Split into train and test sets
```

### Comparing `landmarkclassifier-2.0.7/.gitignore` & `landmarkclassifier-2.1.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -104,8 +104,9 @@
 # IDE settings
 .vscode/
 .idea/
 
 .ruff_cache
 /.vs/LANDMark/v16
 /.vs/LANDMark/config
-/.vs
+/.vs
+/notebooks/Untitled.ipynb
```

### Comparing `landmarkclassifier-2.0.7/LICENSE` & `landmarkclassifier-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.7/pyproject.toml` & `landmarkclassifier-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "LANDMarkClassifier"
-version = "2.0.7"
+version = "2.1.0"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "Teresita M. Porter"},
     {name = "Michael Wright"},
     {name = "G. Brian Golding"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
```

### Comparing `landmarkclassifier-2.0.7/PKG-INFO` & `landmarkclassifier-2.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LANDMarkClassifier
-Version: 2.0.7
+Version: 2.1.0
 Summary: LANDMark: An ensemble approach to the supervised selection of biomarkers in high-throughput sequencing data
 Project-URL: Homepage, https://github.com/jrudar/LANDMark
 Project-URL: Repository, https://github.com/jrudar/LANDMark.git
 Project-URL: Bug Tracker, https://github.com/jrudar/LANDMark/issues
 Author: Teresita M. Porter, Michael Wright, G. Brian Golding
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
@@ -86,54 +86,20 @@
 
 ## Interface
 
 An overview of the API can be found [here](docs/API.md).
 
 ## Usage and Examples
 
-Comming Soon
+Examples of how to use `LANDMark` can be found [here](notebooks/README.md).
 
 ## Contributing
 
 To contribute to the development of `LANDMark` please read our [contributing guide](docs/CONTRIBUTING.md)
 
-## Basic Usage
-
-    from LANDMark import LANDMarkClassifier
-
-    from sklearn.datasets import load_wine
-    from sklearn.preprocessing import StandardScaler
-    from sklearn.model_selection import train_test_split
-
-    # Create the dataset
-    X, y = load_wine(return_X_y = True)
-
-    # Split into train and test sets
-    X_train, X_test, y_train, y_test = train_test_split(
-        X, y, test_size=0.2, random_state=0, stratify=y
-    )
-
-    # Standardize
-    X_trf = StandardScaler()
-    X_trf.fit(X_train)
-
-    X_train = X_trf.transform(X_train)
-    X_test = X_trf.transform(X_test)
-
-    # Setup a LANDMark model and fit
-    clf = LANDMarkClassifier()
-    clf.fit(X_train, y_train)
-
-    # Make a prediction
-    predictions = clf.predict(X_test)
-
-### Specal Notes
-
-Starting with TensorFlow 2.11, GPU support on Windows 10 and higher requires Windows WSL2.
-See: https://www.tensorflow.org/install/pip
 
 ### References
 
     Rudar, J., Porter, T.M., Wright, M., Golding G.B., Hajibabaei, M. LANDMark: an ensemble 
     approach to the supervised selection of biomarkers in high-throughput sequencing data. 
     BMC Bioinformatics 23, 110 (2022). https://doi.org/10.1186/s12859-022-04631-z
```

