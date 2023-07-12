# Comparing `tmp/sortedness-0.230710.0.tar.gz` & `tmp/sortedness-1.230711.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortedness-0.230710.0.tar", max compression
+gzip compressed data, was "sortedness-1.230711.1.tar", max compression
```

## Comparing `sortedness-0.230710.0.tar` & `sortedness-1.230711.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-0.230710.0/LICENSE
--rw-r--r--   0        0        0     5535 2023-07-11 02:49:51.038638 sortedness-0.230710.0/README.md
--rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-0.230710.0/build.py
--rw-r--r--   0        0        0     1328 2023-07-11 02:50:49.082635 sortedness-0.230710.0/pyproject.toml
--rw-r--r--   0        0        0      118 2023-05-02 18:43:33.326749 sortedness-0.230710.0/src/sortedness/__init__.py
--rw-r--r--   0        0        0     7224 2023-07-07 00:44:07.161305 sortedness-0.230710.0/src/sortedness/agnostic.py
--rw-r--r--   0        0        0     1281 2023-05-02 18:58:14.909747 sortedness-0.230710.0/src/sortedness/config.py
--rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-0.230710.0/src/sortedness/evaluation/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-02 18:58:14.873747 sortedness-0.230710.0/src/sortedness/evaluation/plot.py
--rw-r--r--   0        0        0     5145 2023-05-02 18:58:14.889747 sortedness-0.230710.0/src/sortedness/global_.py
--rw-r--r--   0        0        0     3043 2023-07-07 00:44:07.169305 sortedness-0.230710.0/src/sortedness/gtau.py
--rw-r--r--   0        0        0    26230 2023-07-11 02:49:29.806640 sortedness-0.230710.0/src/sortedness/local.py
--rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-0.230710.0/src/sortedness/matrices.py
--rw-r--r--   0        0        0     2983 2023-07-07 00:49:33.533727 sortedness-0.230710.0/src/sortedness/parallel.py
--rw-r--r--   0        0        0     8399 2023-07-07 00:56:13.866263 sortedness-0.230710.0/src/sortedness/rank.py
--rw-r--r--   0        0        0     4707 2023-05-02 18:58:14.909747 sortedness-0.230710.0/src/sortedness/trustworthiness.py
--rw-r--r--   0        0        0     3518 2023-07-07 00:28:29.856946 sortedness-0.230710.0/src/sortedness/wtau/__init__.py
--rw-r--r--   0        0        0  1267818 2023-07-07 01:08:20.579195 sortedness-0.230710.0/src/sortedness/wtau/wtau.c
--rwxr-xr-x   0        0        0  1348408 2023-05-30 20:09:00.000000 sortedness-0.230710.0/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so
--rw-r--r--   0        0        0   334715 2023-07-07 01:08:20.643195 sortedness-0.230710.0/src/sortedness/wtau/wtau.html
--rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-0.230710.0/src/sortedness/wtau/wtau.pyx
--rw-r--r--   0        0        0     6708 1970-01-01 00:00:00.000000 sortedness-0.230710.0/setup.py
--rw-r--r--   0        0        0     6140 1970-01-01 00:00:00.000000 sortedness-0.230710.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-1.230711.1/LICENSE
+-rw-r--r--   0        0        0     7251 2023-07-12 00:44:07.274375 sortedness-1.230711.1/README.md
+-rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-1.230711.1/build.py
+-rw-r--r--   0        0        0     1368 2023-07-12 00:44:09.198374 sortedness-1.230711.1/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-05-02 18:43:33.326749 sortedness-1.230711.1/src/sortedness/__init__.py
+-rw-r--r--   0        0        0     7224 2023-07-07 00:44:07.161305 sortedness-1.230711.1/src/sortedness/agnostic.py
+-rw-r--r--   0        0        0     1281 2023-05-02 18:58:14.909747 sortedness-1.230711.1/src/sortedness/config.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-1.230711.1/src/sortedness/evaluation/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-02 18:58:14.873747 sortedness-1.230711.1/src/sortedness/evaluation/plot.py
+-rw-r--r--   0        0        0     5145 2023-05-02 18:58:14.889747 sortedness-1.230711.1/src/sortedness/global_.py
+-rw-r--r--   0        0        0     3043 2023-07-07 00:44:07.169305 sortedness-1.230711.1/src/sortedness/gtau.py
+-rw-r--r--   0        0        0    30009 2023-07-12 00:02:27.491503 sortedness-1.230711.1/src/sortedness/local.py
+-rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-1.230711.1/src/sortedness/matrices.py
+-rw-r--r--   0        0        0     2983 2023-07-11 23:12:22.741346 sortedness-1.230711.1/src/sortedness/parallel.py
+-rw-r--r--   0        0        0     8399 2023-07-07 00:56:13.866263 sortedness-1.230711.1/src/sortedness/rank.py
+-rw-r--r--   0        0        0     4707 2023-05-02 18:58:14.909747 sortedness-1.230711.1/src/sortedness/trustworthiness.py
+-rw-r--r--   0        0        0     3518 2023-07-07 00:28:29.856946 sortedness-1.230711.1/src/sortedness/wtau/__init__.py
+-rw-r--r--   0        0        0  1267818 2023-07-12 00:38:02.494498 sortedness-1.230711.1/src/sortedness/wtau/wtau.c
+-rwxr-xr-x   0        0        0  1348408 2023-05-30 20:09:00.000000 sortedness-1.230711.1/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0   334715 2023-07-12 00:38:02.518498 sortedness-1.230711.1/src/sortedness/wtau/wtau.html
+-rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-1.230711.1/src/sortedness/wtau/wtau.pyx
+-rw-r--r--   0        0        0     8470 1970-01-01 00:00:00.000000 sortedness-1.230711.1/setup.py
+-rw-r--r--   0        0        0     7856 1970-01-01 00:00:00.000000 sortedness-1.230711.1/PKG-INFO
```

### Comparing `sortedness-0.230710.0/LICENSE` & `sortedness-1.230711.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/README.md` & `sortedness-1.230711.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 [![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)
 [![DOI](https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)
 [![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)
 
 
 # sortedness
 
-`sortedness` is a measure of quality of data transformation, often dimensionality reduction.
-It is less sensitive to irrelevant distortions and return values in a more meaningful interval than Kruskal stress formula I.
+`sortedness` is the level of agreement between two points regarding to how they rank all remaining points in a dataset.
+This ia valid even for points from different spaces, enabling the measurement of the quality of data transformation processes, often dimensionality reduction.
+It is less sensitive to irrelevant distortions, and return values in a more meaningful interval, than Kruskal stress formula I.
 <br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 
 ## Overview
 Local variants return a value for each provided point. The global variant returns a single value for all points.
 Any local variant can be used as a global measure by taking the mean value.
 
 Local variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.
@@ -87,24 +88,34 @@
 ```
 
 ```python3
 
 s = sortedness(original, projected1)
 print(min(s), sum(s) / len(s), max(s))
 """
-0.432937128932 0.7813889452999166 0.944810120534
+0.393463224666 0.7565797804351666 0.944810120534
 """
 ```
 
 ```python3
 
 s = sortedness(original, projectedrnd)
 print(min(s), sum(s) / len(s), max(s))
 """
--0.578096068617 -0.06328160775358334 0.396112816715
+-0.648305479567 -0.09539895194975 0.397019507592
+"""
+```
+
+```python3
+
+# Single point fast calculation.
+s = sortedness(original, projectedrnd, 2)
+print(s)
+"""
+0.231079547491
 """
 ```
 
 
 </p>
 </details>
 
@@ -148,32 +159,42 @@
 ```
 
 ```python3
 
 s = pwsortedness(original, projected1)
 print(min(s), sum(s) / len(s), max(s))
 """
-0.730078995423 0.7744573488776667 0.837310352695
+0.649315577592 0.7534291438323333 0.834601601062
 """
 ```
 
 ```python3
 
 s = pwsortedness(original, projectedrnd)
 print(min(s), sum(s) / len(s), max(s))
 """
--0.198780473657 -0.0645984203715 0.147224384381
+-0.168611098044 -0.07988253899799999 0.14442446342
+"""
+```
+
+```python3
+
+# Single point fast calculation.
+s = pwsortedness(original, projectedrnd, 2)
+print(s)
+"""
+0.036119718802
 """
 ```
 
 
 </p>
 </details>
 
-**Sortedness**
+**Global pairwise sortedness**
 <details>
 <p>
 
 ```python3
 
 import numpy as np
 from numpy.random import permutation
@@ -230,11 +251,36 @@
 </p>
 </details>
 
 
 ** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves**
 
 
+### TODO
+Future work address handling large datasets: approximate sortedness value, and size-insensitive weighting scheme.
 
-
+## Reference
+Please use the following reference to cite this work:
+```
+@inproceedings {10.2312:eurova.20231093,
+booktitle = {EuroVis Workshop on Visual Analytics (EuroVA)},
+editor = {Angelini, Marco and El-Assady, Mennatallah},
+title = {{Nonparametric Dimensionality Reduction Quality Assessment based on Sortedness of Unrestricted Neighborhood}},
+author = {Pereira-Santos, Davi and Neves, Tácito Trindade Araújo Tiburtino and Carvalho, André C. P. L. F. de and Paulovich, Fernando V.},
+year = {2023},
+publisher = {The Eurographics Association},
+ISSN = {2664-4487},
+ISBN = {978-3-03868-222-6},
+DOI = {10.2312/eurova.20231093}
+}
+```
 
 ## Grants
+This work was supported by Wellcome Leap 1kD Program; São
+Paulo Research Foundation (FAPESP) - grant 2020/09835-1; Cana-
+dian Institute for Health Research (CIHR) Canadian Research
+Chairs (CRC) stipend [award number 1024586]; Canadian Foun-
+dation for Innovation (CFI) John R. Evans Leaders Fund (JELF)
+[grant number 38835]; Dalhousie Medical Research Fund (DMRF)
+COVID-19 Research Grant [grant number 603082]; and the Cana-
+dian Institute for Health Research (CIHR) Project Grant [award
+number 177968].
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -3,18 +3,20 @@
 badge.svg)](https://codecov.io/gh/sortedness/sortedness) [github] ![Python
 version](https://img.shields.io/badge/python-3.8+-blue.svg) [![license: GPL v3]
 (https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
 licenses/gpl-3.0)  [![API documentation](https://img.shields.io/badge/doc-
 API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness) [![DOI]
 (https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/
 513273889) [![Downloads](https://static.pepy.tech/badge/sortedness)](https://
-pepy.tech/project/sortedness) # sortedness `sortedness` is a measure of quality
-of data transformation, often dimensionality reduction. It is less sensitive to
-irrelevant distortions and return values in a more meaningful interval than
-Kruskal stress formula I.
+pepy.tech/project/sortedness) # sortedness `sortedness` is the level of
+agreement between two points regarding to how they rank all remaining points in
+a dataset. This ia valid even for points from different spaces, enabling the
+measurement of the quality of data transformation processes, often
+dimensionality reduction. It is less sensitive to irrelevant distortions, and
+return values in a more meaningful interval, than Kruskal stress formula I.
 This [Python library](https://pypi.org/project/sortedness) / [code](https://
 github.com/sortedness/sortedness) provides a reference implementation for the
 functions presented [here (paper unavailable until publication)](https://
 scholar.google.com/
 scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 ## Overview Local variants return a value for each provided point. The global
 variant returns a single value for all points. Any local variant can be used as
@@ -31,42 +33,63 @@
 (seed=0) original = rng.multivariate_normal(mean, cov, size=12) projected2 =
 PCA(n_components=2).fit_transform(original) projected1 = PCA
 (n_components=1).fit_transform(original) np.random.seed(0) projectedrnd =
 permutation(original) # Print `min`, `mean`, and `max` values. s = sortedness
 (original, original) print(min(s), sum(s) / len(s), max(s)) """ 1.0 1.0 1.0 """
 ``` ```python3 s = sortedness(original, projected2) print(min(s), sum(s) / len
 (s), max(s)) """ 1.0 1.0 1.0 """ ``` ```python3 s = sortedness(original,
-projected1) print(min(s), sum(s) / len(s), max(s)) """ 0.432937128932
-0.7813889452999166 0.944810120534 """ ``` ```python3 s = sortedness(original,
-projectedrnd) print(min(s), sum(s) / len(s), max(s)) """ -0.578096068617 -
-0.06328160775358334 0.396112816715 """ ```
+projected1) print(min(s), sum(s) / len(s), max(s)) """ 0.393463224666
+0.7565797804351666 0.944810120534 """ ``` ```python3 s = sortedness(original,
+projectedrnd) print(min(s), sum(s) / len(s), max(s)) """ -0.648305479567 -
+0.09539895194975 0.397019507592 """ ``` ```python3 # Single point fast
+calculation. s = sortedness(original, projectedrnd, 2) print(s) """
+0.231079547491 """ ```
  **Pairwise sortedness**
 ```python3 import numpy as np from numpy.random import permutation from
 sklearn.decomposition import PCA from sortedness import pwsortedness # Some
 synthetic data. mean = (1, 2) cov = np.eye(2) rng = np.random.default_rng
 (seed=0) original = rng.multivariate_normal(mean, cov, size=12) projected2 =
 PCA(n_components=2).fit_transform(original) projected1 = PCA
 (n_components=1).fit_transform(original) np.random.seed(0) projectedrnd =
 permutation(original) # Print `min`, `mean`, and `max` values. s = pwsortedness
 (original, original) print(min(s), sum(s) / len(s), max(s)) """ 1.0 1.0 1.0 """
 ``` ```python3 s = pwsortedness(original, projected2) print(min(s), sum(s) /
 len(s), max(s)) """ 1.0 1.0 1.0 """ ``` ```python3 s = pwsortedness(original,
-projected1) print(min(s), sum(s) / len(s), max(s)) """ 0.730078995423
-0.7744573488776667 0.837310352695 """ ``` ```python3 s = pwsortedness(original,
-projectedrnd) print(min(s), sum(s) / len(s), max(s)) """ -0.198780473657 -
-0.0645984203715 0.147224384381 """ ```
- **Sortedness**
+projected1) print(min(s), sum(s) / len(s), max(s)) """ 0.649315577592
+0.7534291438323333 0.834601601062 """ ``` ```python3 s = pwsortedness(original,
+projectedrnd) print(min(s), sum(s) / len(s), max(s)) """ -0.168611098044 -
+0.07988253899799999 0.14442446342 """ ``` ```python3 # Single point fast
+calculation. s = pwsortedness(original, projectedrnd, 2) print(s) """
+0.036119718802 """ ```
+ **Global pairwise sortedness**
 ```python3 import numpy as np from numpy.random import permutation from
 sklearn.decomposition import PCA from sortedness import global_pwsortedness #
 Some synthetic data. mean = (1, 2) cov = np.eye(2) rng = np.random.default_rng
 (seed=0) original = rng.multivariate_normal(mean, cov, size=12) projected2 =
 PCA(n_components=2).fit_transform(original) projected1 = PCA
 (n_components=1).fit_transform(original) np.random.seed(0) projectedrnd =
 permutation(original) # Print measurement result and p-value. s =
 global_pwsortedness(original, original) print(list(s)) """ [1.0,
 3.6741408919675163e-93] """ ``` ```python3 s = global_pwsortedness(original,
 projected2) print(list(s)) """ [1.0, 3.6741408919675163e-93] """ ``` ```python3
 s = global_pwsortedness(original, projected1) print(list(s)) """
 [0.7715617715617715, 5.240847664048334e-20] """ ``` ```python3 s =
 global_pwsortedness(original, projectedrnd) print(list(s)) """ [-
 0.06107226107226107, 0.46847188611226276] """ ```
- ** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves** ## Grants
+ ** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves** ### TODO
+Future work address handling large datasets: approximate sortedness value, and
+size-insensitive weighting scheme. ## Reference Please use the following
+reference to cite this work: ``` @inproceedings {10.2312:eurova.20231093,
+booktitle = {EuroVis Workshop on Visual Analytics (EuroVA)}, editor =
+{Angelini, Marco and El-Assady, Mennatallah}, title = {{Nonparametric
+Dimensionality Reduction Quality Assessment based on Sortedness of Unrestricted
+Neighborhood}}, author = {Pereira-Santos, Davi and Neves, TÃ¡cito Trindade
+AraÃºjo Tiburtino and Carvalho, AndrÃ© C. P. L. F. de and Paulovich, Fernando
+V.}, year = {2023}, publisher = {The Eurographics Association}, ISSN = {2664-
+4487}, ISBN = {978-3-03868-222-6}, DOI = {10.2312/eurova.20231093} } ``` ##
+Grants This work was supported by Wellcome Leap 1kD Program; SÃ£o Paulo
+Research Foundation (FAPESP) - grant 2020/09835-1; Cana- dian Institute for
+Health Research (CIHR) Canadian Research Chairs (CRC) stipend [award number
+1024586]; Canadian Foun- dation for Innovation (CFI) John R. Evans Leaders Fund
+(JELF) [grant number 38835]; Dalhousie Medical Research Fund (DMRF) COVID-19
+Research Grant [grant number 603082]; and the Cana- dian Institute for Health
+Research (CIHR) Project Grant [award number 177968].
```

### Comparing `sortedness-0.230710.0/build.py` & `sortedness-1.230711.1/build.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/pyproject.toml` & `sortedness-1.230711.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortedness"
-version = "0.230710.0"
+version = "1.230711.1"
 description = "Measures of projection quality"
 authors = ["davips <dpsabc@gmail.com>", "tacito <tacito.neves@gmail.com>"]
 license = "GPLv3"
 build = "build.py"  # For Cython. apt-get package needed: python3-numpy
 readme = 'README.md'
 packages = [
     { include = "sortedness", from = "src" }
@@ -40,11 +40,13 @@
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 black = "^23.3.0"
 pdoc3 = "^0.10.0"
 autoreadme = "^0.2302.3"
 scikit-learn = "^1.2.2"
 numpy = "^1.24.2"  #=1.24.2
+matplotlib = "^3.7.2"
+pandas = "^2.0.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "Cython>=0.29.27", "setuptools>=60.8.1", "numpy>=1.23.3", "scipy>=1.10.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sortedness-0.230710.0/src/sortedness/agnostic.py` & `sortedness-1.230711.1/src/sortedness/agnostic.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/config.py` & `sortedness-1.230711.1/src/sortedness/config.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/evaluation/plot.py` & `sortedness-1.230711.1/src/sortedness/evaluation/plot.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/global_.py` & `sortedness-1.230711.1/src/sortedness/global_.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/gtau.py` & `sortedness-1.230711.1/src/sortedness/gtau.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/local.py` & `sortedness-1.230711.1/src/sortedness/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     nI = ~eye(n_points, dtype=bool)  # Mask to remove diagonal.
     return X[nI].reshape(n_points, -1)
 
 
 weightedtau.isweightedtau = True
 
 
-def sortedness(X, X_, i=None, f=weightedtau, distance_dependent=True, return_pvalues=False, parallel=True, parallel_n_trigger=500, parallel_kwargs=None, **kwargs):
+def sortedness(X, X_, i=None, symmetric=True, f=weightedtau, distance_dependent=True, return_pvalues=False, parallel=True, parallel_n_trigger=500, parallel_kwargs=None, **kwargs):
     """
      Calculate the sortedness (stress-like correlation-based measure that ignores distance proportions) value for each point
      Functions available as scipy correlation coefficients:
          ρ-sortedness (Spearman),
          𝜏-sortedness (Kendall's 𝜏),
          w𝜏-sortedness (Sebastiano Vigna weighted Kendall's 𝜏)  ← default
 
@@ -61,14 +61,19 @@
     X
         matrix with an instance by row in a given space (often the original one)
     X_
         matrix with an instance by row in another given space (often the projected one)
     i
         None:   calculate sortedness for all instances
         `int`:  index of the instance of interest
+    symmetric
+        True: Take the mean between extrusion and intrusion emphasis
+            Equivalent to `(sortedness(a, b) + sortedness(b, a)) / 2` at a slightly lower cost.
+            Might increase memory usage.
+        False: Weight by original distances (extrusion emphasis), not the projected distances.
     f
         Distance criteria:
         callable    =   scipy correlation function:
             weightedtau (weighted Kendall’s τ is the default), kendalltau, spearmanr
             Meaning of resulting values for correlation-based functions:
                 1.0:    perfect projection          (regarding order of examples)
                 0.0:    random projection           (enough distortion to have no information left when considering the overall ordering)
@@ -104,22 +109,22 @@
     >>> rnd = np.random.default_rng(0)
     >>> rnd.shuffle(ll)
     >>> b = np.array(ll)
     >>> b.ravel()
     array([ 2, 10,  3, 11,  0,  4,  7,  5, 16, 12, 13,  6,  9, 14,  8,  1, 15])
     >>> r = sortedness(a, b)
     >>> r
-    array([ 0.19597951, -0.37003858,  0.06014087, -0.42174564,  0.2448619 ,
-            0.24635858,  0.16814336,  0.06919001,  0.1627886 ,  0.33136454,
-            0.41592274, -0.10615388,  0.17549727,  0.17371479, -0.21360864,
-           -0.3677769 , -0.08292823])
+    array([ 0.24691868, -0.17456491,  0.19184376, -0.18193532,  0.07175694,
+            0.27992254,  0.04121859,  0.16249574, -0.03506842,  0.27856259,
+            0.40866965, -0.07617887,  0.12184064,  0.24762942, -0.05049511,
+           -0.46277399,  0.12193493])
     >>> min(r), max(r)
-    (-0.421745643027, 0.415922739891)
+    (-0.462773990559, 0.408669653064)
     >>> round(mean(r), 12)
-    0.040100605153
+    0.070104521222
 
     >>> import numpy as np
     >>> from functools import partial
     >>> from scipy.stats import spearmanr, weightedtau
     >>> me = (1, 2)
     >>> cov = eye(2)
     >>> rng = np.random.default_rng(seed=0)
@@ -134,22 +139,22 @@
     >>> min(s), max(s), s
     (1.0, 1.0, array([1., 1., 1., 1., 1., 1., 1., 1., 1., 1., 1., 1.]))
     >>> s = sortedness(original, projected2)
     >>> min(s), max(s), s
     (1.0, 1.0, array([1., 1., 1., 1., 1., 1., 1., 1., 1., 1., 1., 1.]))
     >>> s = sortedness(original, projected1)
     >>> min(s), max(s), s
-    (0.432937128932, 0.944810120534, array([0.43293713, 0.53333015, 0.88412753, 0.94481012, 0.81485109,
-           0.81330052, 0.76691474, 0.91169619, 0.88998817, 0.90102615,
-           0.61372341, 0.86996213]))
+    (0.393463224666, 0.944810120534, array([0.43735232, 0.39346322, 0.88256382, 0.94481012, 0.794352  ,
+           0.78933235, 0.7409755 , 0.90341771, 0.89081602, 0.90102615,
+           0.53953244, 0.86131572]))
     >>> s = sortedness(original, projectedrnd)
     >>> min(s), max(s), s
-    (-0.578096068617, 0.396112816715, array([ 0.21296126, -0.57809607,  0.33083346, -0.00638865, -0.16007932,
-            0.39611282, -0.27357934,  0.04360717, -0.54534052,  0.19042181,
-           -0.32805008, -0.04178184]))
+    (-0.648305479567, 0.397019507592, array([ 0.12977864, -0.49887948,  0.23107955, -0.09591571, -0.12509467,
+            0.39701951, -0.21772049,  0.11895569, -0.64830548,  0.00279294,
+           -0.34542772, -0.09307021]))
 
     >>> sortedness(original, original, f=kendalltau, return_pvalues=True)
     array([[1.0000e+00, 5.0104e-08],
            [1.0000e+00, 5.0104e-08],
            [1.0000e+00, 5.0104e-08],
            [1.0000e+00, 5.0104e-08],
            [1.0000e+00, 5.0104e-08],
@@ -194,64 +199,70 @@
     >>> sortedness(original, projectedrnd, f=wf)
     array([ 0.23771513, -0.2790059 ,  0.3718005 , -0.16623167,  0.06179047,
             0.40434396, -0.00130294,  0.46569739, -0.67581876, -0.23852189,
            -0.39125007,  0.12131153])
     >>> np.random.seed(14980)
     >>> projectedrnd = permutation(original)
     >>> sortedness(original, projectedrnd)
-    array([ 0.21666209, -0.23798067,  0.16830046, -0.5559795 , -0.23470751,
-            0.35716692, -0.0054951 , -0.35890385,  0.13101743, -0.48460059,
-           -0.46430457,  0.27400939])
+    array([ 0.24432153, -0.19634576, -0.00238081, -0.4999116 , -0.01625951,
+            0.22478766,  0.07176118, -0.48092843,  0.19345964, -0.44895295,
+           -0.42044773,  0.06942218])
     >>> sortedness(original, np.flipud(original))
-    array([-0.26471073,  0.39699442,  0.05022757,  0.21215372,  0.23467884,
-           -0.33277347, -0.31616633,  0.19381204, -0.16114967,  0.08829425,
-            0.3383928 , -0.31012412])
+    array([-0.28741742,  0.36769361,  0.06926091,  0.02550202,  0.21424544,
+           -0.3244699 , -0.3244699 ,  0.21424544,  0.02550202,  0.06926091,
+            0.36769361, -0.28741742])
     >>> original = np.array([[0],[1],[2],[3],[4],[5],[6]])
     >>> projected = np.array([[6],[5],[4],[3],[2],[1],[0]])
     >>> sortedness(original, projected)
     array([1., 1., 1., 1., 1., 1., 1.])
     >>> projected = np.array([[0],[6],[5],[4],[3],[2],[1]])
     >>> sortedness(original, projected)
-    array([-1.        ,  0.42263889,  0.80668827,  0.98180162,  0.98180162,
-            0.82721863,  0.61648537])
+    array([-1.        ,  0.51956213,  0.81695345,  0.98180162,  0.98180162,
+            0.81695345,  0.51956213])
     >>> sortedness(original, projected, 1)
-    0.4226388949217901
+    0.519562134793
+    >>> sortedness(original, projected, 1, symmetric=False)
+    0.422638894922
     >>> sortedness([[1,2,3,3],[1,2,7,3],[3,4,8,5],[1,8,3,5]], [[2,1,2,3],[3,1,2,3],[5,4,5,6],[9,7,6,3]], 1)
-    0.18181818181818177
+    0.181818181818
     """
     isweightedtau = False
     if hasattr(f, "isweightedtau") and f.isweightedtau:
         isweightedtau = True
-        if "rank" not in kwargs:
+        if not symmetric:
+            if "rank" in kwargs:  # pragma: no cover
+                raise Exception(f"Cannot set `symmetric=False` and provide `rank` at the same time.")
             kwargs["rank"] = None
+    elif not symmetric:  # pragma: no cover
+        raise Exception(f"`symmetric=False` not implemented for custom `f`")
     if parallel_kwargs is None:
         parallel_kwargs = {}
     result, pvalues = [], []
     npoints = len(X)
 
     if i is not None:
-        x = X[i] if isinstance(X, (ndarray, list)) else X.iloc[i]
-        x_ = X_[i] if isinstance(X_, (ndarray, list)) else X_.iloc[i]
+        x = X[i] if isinstance(X, (ndarray, list)) else X.iloc[i].to_numpy()
+        x_ = X_[i] if isinstance(X_, (ndarray, list)) else X_.iloc[i].to_numpy()
         X = np.delete(X, i, axis=0)
         X_ = np.delete(X_, i, axis=0)
         d_ = np.sum((X_ - x_) ** 2, axis=1)
         if distance_dependent:
             d = np.sum((X - x) ** 2, axis=1)
             scores_X, scores_X_ = (-d, -d_) if isweightedtau else (d, d_)
             corr, pvalue = f(scores_X, scores_X_, **kwargs)
-            return (corr, pvalue) if return_pvalues else corr
+            return (np.round(corr, 12), pvalue) if return_pvalues else np.round(corr, 12)
         else:  # pragma: no cover
             raise Exception(f"Not implemented yet; it is an open problem")
-            D = abs(X - x).T
-            scores_X, scores_x_ = (-D, -d_) if isweightedtau else (D, d_)
-            for j in range(len(scores_X)):
-                corr, pvalue = f(scores_X[j], scores_x_, **kwargs)
-                result.append(round(corr, 12))
-                pvalues.append(round(pvalue, 12))
-            return (mean(result), mean(pvalues)) if return_pvalues else mean(result)
+            # D = abs(X - x).T
+            # scores_X, scores_x_ = (-D, -d_) if isweightedtau else (D, d_)
+            # for j in range(len(scores_X)):
+            #     corr, pvalue = f(scores_X[j], scores_x_, **kwargs)
+            #     result.append(round(corr, 12))
+            #     pvalues.append(round(pvalue, 12))
+            # return (mean(result), mean(pvalues)) if return_pvalues else mean(result)
 
     if distance_dependent:
         tmap = mp.ThreadingPool(**parallel_kwargs).imap if parallel and npoints > parallel_n_trigger else map
         sqdist_X, sqdist_X_ = tmap(lambda M: cdist(M, M, metric='sqeuclidean'), [X, X_])
         D = remove_diagonal(sqdist_X)
         D_ = remove_diagonal(sqdist_X_)
         scores_X, scores_X_ = (-D, -D_) if isweightedtau else (D, D_)
@@ -269,34 +280,39 @@
 
     result = np.array(result, dtype=float)
     if return_pvalues:
         return np.array(list(zip(result, pvalues)))
     return result
 
 
-def pwsortedness(X, X_, i=None, parallel=True, parallel_n_trigger=200, batches=10, debug=False, dist=None, cython=False, **parallel_kwargs):
+def pwsortedness(X, X_, i=None, symmetric=True, parallel=True, parallel_n_trigger=200, batches=10, debug=False, dist=None, cython=False, **parallel_kwargs):
     """
     Local pairwise sortedness (Λ𝜏w) based on Sebastiano Vigna weighted Kendall's 𝜏
 
     Importance rankings are calculated internally based on proximity of each pair to the point of interest.
 
     # TODO?: add flag to break extremely rare cases of ties that persist after projection (implies a much slower algorithm)
-        This probably doesn't make any difference on the result, except on categorical, pathological or toy datasets
+        This probably doesn't make any difference on the res, except on categorical, pathological or toy datasets
         Values can be lower due to the presence of ties, but only when the projection isn't prefect for all points.
         In the end, it might be even desired to penalize ties, as they don't exactly contribute to a stronger ordering and are (probabilistically) easier to be kept than a specific order.
 
     Parameters
     ----------
     X
         Original dataset
     X_
         Projected points
     i
         None:   calculate pwsortedness for all instances
         `int`:  index of the instance of interest
+    symmetric
+        True: Take the mean between extrusion and intrusion emphasis
+            Equivalent to `(pwsortedness(a, b) + pwsortedness(b, a)) / 2` at a slightly lower cost.
+            Might increase memory usage.
+        False: Weight by original distances (extrusion emphasis), not the projected distances.
     parallel
         None: Avoid high-memory parallelization
         True: Full parallelism
         False: No parallelism
     parallel_kwargs
         Any extra argument to be provided to pathos parallelization
     parallel_n_trigger
@@ -335,119 +351,146 @@
     >>> min(r), max(r), round(mean(r), 12)
     (1.0, 1.0, 1.0)
     >>> r = pwsortedness(original, projected2)
     >>> min(r), round(mean(r), 12), max(r)
     (1.0, 1.0, 1.0)
     >>> r = pwsortedness(original, projected1)
     >>> min(r), round(mean(r), 12), max(r)
-    (0.730078995423, 0.774457348878, 0.837310352695)
+    (0.649315577592, 0.753429143832, 0.834601601062)
     >>> r = pwsortedness(original, projected2[:, 1:])
     >>> min(r), round(mean(r), 12), max(r)
-    (0.18672441995, 0.281712132364, 0.420214364305)
+    (0.035312055682, 0.2002329034, 0.352491282966)
     >>> r = pwsortedness(original, projectedrnd)
     >>> min(r), round(mean(r), 12), max(r)
-    (-0.198780473657, -0.064598420372, 0.147224384381)
+    (-0.168611098044, -0.079882538998, 0.14442446342)
     >>> pwsortedness(original, projected1)[1]
-    0.730078995423
+    0.649315577592
     >>> pwsortedness(original, projected1, cython=True)[1]
-    0.730078995423
+    0.649315577592
     >>> pwsortedness(original, projected1, i=1)
+    0.649315577592
+    >>> pwsortedness(original, projected1, symmetric=False, cython=True)[1]
+    0.730078995423
+    >>> pwsortedness(original, projected1, symmetric=False, i=1)
     0.730078995423
+    >>> pwsortedness(original, projected1, symmetric=False)
+    array([0.75892647, 0.730079  , 0.83496865, 0.73161226, 0.75376525,
+           0.83301104, 0.76695755, 0.74759156, 0.81434161, 0.74067221,
+           0.74425225, 0.83731035])
     """
     npoints = len(X) if X is not None else len(dist[0])  # pragma: no cover
     tmap = mp.ThreadingPool(**parallel_kwargs).imap if parallel and npoints > parallel_n_trigger else map
     pmap = mp.ProcessingPool(**parallel_kwargs).imap if parallel and npoints > parallel_n_trigger else map
     if debug:  # pragma: no cover
         print(1)
     thread = lambda M: -pdist(M, metric="sqeuclidean")
-
-    # if i is not None:
-    #     tmp, tmp_ = X[0], X_[0]
-    #     X[0], X_[0] = X[i], X_[i]
-    #     X[i], X_[i] = tmp, tmp_
-
     scores_X, scores_X_ = tmap(thread, [X, X_]) if X is not None else (-squareform(dist[0]), -squareform(dist[1]))
     if debug:  # pragma: no cover
         print(2)
 
-    def makeM(E, single=False):
+    def makeM(E):
         n = len(E)
         m = (n ** 2 - n) // 2
-        M = np.zeros((m, 1 if single else n))
-        if debug:  # pragma: no cover
-            print(4)
+        M = np.zeros((m, E.shape[1]))
         c = 0
         for i in range(n - 1):  # a bit slow, but only a fraction of wtau (~5%)
             h = n - i - 1
             d = c + h
             M[c:d] = E[i] + E[i + 1:]
             c = d
-        if debug:  # pragma: no cover
-            print(5)
         del E
         gc.collect()
         return M.T
 
-    D = squareform(-scores_X) if dist is None else dist[0]
+    if symmetric:
+        D, D_ = tmap(squareform, [-scores_X, -scores_X_]) if dist is None else (dist[0], dist[1])
+    else:
+        D = squareform(-scores_X) if dist is None else dist[0]
+
     if i is None:
-        if debug:  # pragma: no cover
-            print(3)
         n = len(D)
-        M = makeM(D)
-        if debug:  # pragma: no cover
-            print(6)
+        if symmetric:
+            M, M_ = pmap(makeM, [D, D_])
+            R_ = rank_alongrow(M_, step=n // batches, parallel=parallel, **parallel_kwargs).T
+            del M_
+        else:
+            M = makeM(D)
         R = rank_alongrow(M, step=n // batches, parallel=parallel, **parallel_kwargs).T
         del M
         gc.collect()
-        if debug:  # pragma: no cover
-            print(7)
         if cython:
             from sortedness.wtau import parwtau
-            res = np.round(parwtau(scores_X, scores_X_, npoints, R, parallel=parallel, **parallel_kwargs), 12)
+            res = parwtau(scores_X, scores_X_, npoints, R, parallel=parallel, **parallel_kwargs)
             del R
+            if not symmetric:
+                gc.collect()
+                return np.round(res, 12)
+
+            res_ = parwtau(scores_X, scores_X_, npoints, R_, parallel=parallel, **parallel_kwargs)
+            del R_
             gc.collect()
-            return res
+            return np.round((res + res_) / 2, 12)
         else:
             def thread(r):
-                corr, pvalue = weightedtau(scores_X, scores_X_, rank=r)
-                return round(corr, 12), round(pvalue, 12)
+                corr = weightedtau(scores_X, scores_X_, rank=r)[0]
+                return round(corr, 12)
+
+            gen = (R[:, i] for i in range(len(X)))
+            res = np.array(list(pmap(thread, gen)), dtype=float)
+            del R
+            if not symmetric:
+                gc.collect()
+                return res
+
+            gen = (R_[:, i] for i in range(len(X_)))
+            res_ = np.array(list(pmap(thread, gen)), dtype=float)
+            del R_
+            gc.collect()
+            return np.round((res + res_) / 2, 12)
 
-            result, pvalues = [], []
-            lst = (R[:, i] for i in range(len(X)))
-            for corrs, pvalue in pmap(thread, lst):
-                result.append(corrs)
-                pvalues.append(pvalue)
-            result = np.array(result, dtype=float)
-            return result
+    if symmetric:
+        M, M_ = pmap(makeM, [D[:, i:i + 1], D_[:, i:i + 1]])
+        thread = lambda M: rankdata(M, axis=1, method="average")
+        r, r_ = [r[0].astype(int) - 1 for r in tmap(thread, [M, M_])]
+        s1 = weightedtau(scores_X, scores_X_, r)[0]
+        s2 = weightedtau(scores_X, scores_X_, r_)[0]
+        return round((s1 + s2) / 2, 12)
 
-    M = makeM(D[:, i:i + 1], single=True)
+    M = makeM(D[:, i:i + 1])
     r = rankdata(M, axis=1, method="average")[0].astype(int) - 1
     return round(weightedtau(scores_X, scores_X_, r)[0], 12)
 
-    # D = cdist(X, X[:1])
-    # M = makeM(D, single=True)
-    # r = rankdata(M[0], method="average").astype(int) - 1
-    # return round(weightedtau(scores_X, scores_X_, r)[0], 12)
-
 
-def rsortedness(X, X_, f=weightedtau, return_pvalues=False, parallel=True, parallel_n_trigger=500, parallel_kwargs=None, **kwargs):  # pragma: no cover
+def rsortedness(X, X_, i=None, symmetric=True, f=weightedtau, return_pvalues=False, parallel=True, parallel_n_trigger=500, parallel_kwargs=None, **kwargs):  # pragma: no cover
     """
     Reciprocal sortedness: consider the neighborhood relation the other way around
 
     Might be good to assess the effect of a projection on hubness, and also to serve as a loss function for a custom projection algorithm.
 
     WARNING: this function is experimental, i.e., not as well tested as the others; it might need a better algorithm/fomula as well.
 
     # TODO?: add flag to break (not so rare) cases of ties that persist after projection (implies a much slower algorithm)
         This probably doesn't make any difference on the result, except on categorical, pathological or toy datasets
         Values can be lower due to the presence of ties, but only when the projection isn't prefect for all points.
         In the end, it might be even desired to penalize ties, as they don't exactly contribute to a stronger ordering and are (probabilistically) easier to be kept than a specific order.
 
     Parameters
     ----------
+    X
+        Original dataset
+    X_
+        Projected points
+    i
+        None:   calculate rsortedness for all instances
+        `int`:  index of the instance of interest
+    symmetric
+        True: Take the mean between extrusion and intrusion emphasis
+            Equivalent to `(rsortedness(a, b) + rsortedness(b, a)) / 2` at a slightly lower cost.
+            Might increase memory usage.
+        False: Weight by original distances (extrusion emphasis), not the projected distances.
     f
         Distance criteria:
         callable    =   scipy correlation function:
             weightedtau (weighted Kendall’s τ is the default), kendalltau, spearmanr
             Meaning of resulting values for correlation-based functions:
                 1.0:    perfect projection          (regarding order of examples)
                 0.0:    random projection           (enough distortion to have no information left when considering the overall ordering)
@@ -495,16 +538,23 @@
     # (-0.582915181328, 0.480765206133, 0.087284118913)
     # >>> rsortedness(b, a, f=kendalltau, return_pvalues=True)
     # array([[ 0.2316945 ,  0.04863508],
     #        [-0.37005403,  0.21347624],
     #        [ 0.17618709,  0.04863508],
     #        [-0.35418588,  0.21347624]])
     """
-    if hasattr(f, "isweightedtau") and f.isweightedtau and "rank" not in kwargs:
-        kwargs["rank"] = None
+    isweightedtau = False
+    if hasattr(f, "isweightedtau") and f.isweightedtau:
+        isweightedtau = True
+        if not symmetric:
+            if "rank" in kwargs:
+                raise Exception(f"Cannot set `symmetric=False` and provide `rank` at the same time.")
+            kwargs["rank"] = None
+    elif not symmetric:
+        raise Exception(f"`symmetric=False` not implemented for custom `f`")
     if parallel_kwargs is None:
         parallel_kwargs = {}
     npoints = len(X)
     tmap = mp.ThreadingPool(**parallel_kwargs).imap if parallel and npoints > parallel_n_trigger else map
     pmap = mp.ProcessingPool(**parallel_kwargs).imap if parallel and npoints > parallel_n_trigger else map
     D, D_ = tmap(lambda M: cdist(M, M, metric="sqeuclidean"), [X, X_])
     R, R_ = (rank_alongcol(M, parallel=parallel) for M in [D, D_])
@@ -525,61 +575,82 @@
 
     result, pvalues = [], []
     try:
         from shelchemy.lazy import ichunks
     except Exception as e:
         print("please install shelchemy library.")
         exit()
-    jobs = pmap(thread, ichunks(range(npoints), 15, asgenerators=False))
-    for corrs, pvalues in jobs:
-        result.extend(corrs)
-        pvalues.extend(pvalues)
+    if i is None:
+        jobs = pmap(thread, ichunks(range(npoints), 15, asgenerators=False))
+        for corrs, pvalues in jobs:
+            result.extend(corrs)
+            pvalues.extend(pvalues)
+
+        result = np.array(result, dtype=float)
+        if return_pvalues:
+            return np.array(list(zip(result, pvalues)))
+        return result
 
-    result = np.array(result, dtype=float)
+    corr, pvalue = f(scores_X[i], scores_X_[i], **kwargs)
     if return_pvalues:
-        return np.array(list(zip(result, pvalues)))
-    return result
+        return round(corr, 12), pvalue
+    return round(corr, 12)
 
 
-def stress(X, X_, metric=True, parallel=True, parallel_size_trigger=10000, **parallel_kwargs):
+def stress(X, X_, i=None, metric=True, parallel=True, parallel_size_trigger=10000, **parallel_kwargs):
     """
     Kruskal's "Stress Formula 1" normalized before comparing distances.
     default: Euclidean
 
     >>> import numpy as np
     >>> from functools import partial
     >>> from scipy.stats import spearmanr, weightedtau
     >>> mean = (1, 12)
     >>> cov = eye(2)
     >>> rng = np.random.default_rng(seed=0)
     >>> original = rng.multivariate_normal(mean, cov, size=12)
+    >>> original
+    array([[ 1.12573022, 11.86789514],
+           [ 1.64042265, 12.10490012],
+           [ 0.46433063, 12.36159505],
+           [ 2.30400005, 12.94708096],
+           [ 0.29626476, 10.73457853],
+           [ 0.37672554, 12.04132598],
+           [-1.32503077, 11.78120834],
+           [-0.24591095, 11.26773265],
+           [ 0.45574102, 11.68369984],
+           [ 1.41163054, 13.04251337],
+           [ 0.87146534, 13.36646347],
+           [ 0.33480533, 12.35151007]])
     >>> s = stress(original, original*5)
     >>> min(s), max(s), s
     (0.0, 0.0, array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]))
     >>> from sklearn.decomposition import PCA
     >>> projected = PCA(n_components=2).fit_transform(original)
     >>> s = stress(original, projected)
     >>> min(s), max(s), s
     (0.0, 0.0, array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]))
     >>> projected = PCA(n_components=1).fit_transform(original)
     >>> s = stress(original, projected)
     >>> min(s), max(s), s
-    (0.073462710191, 0.333885390367, array([0.2812499 , 0.31103416, 0.21994448, 0.07346271, 0.2810867 ,
-           0.16411944, 0.17002148, 0.14748528, 0.18341208, 0.14659984,
-           0.33388539, 0.24110857]))
+    (0.073383317103, 0.440609121637, array([0.26748441, 0.31603101, 0.24636389, 0.07338332, 0.34571508,
+           0.19548442, 0.1800883 , 0.16544039, 0.2282494 , 0.16405274,
+           0.44060912, 0.27058614]))
     >>> stress(original, projected)
-    array([0.2812499 , 0.31103416, 0.21994448, 0.07346271, 0.2810867 ,
-           0.16411944, 0.17002148, 0.14748528, 0.18341208, 0.14659984,
-           0.33388539, 0.24110857])
+    array([0.26748441, 0.31603101, 0.24636389, 0.07338332, 0.34571508,
+           0.19548442, 0.1800883 , 0.16544039, 0.2282494 , 0.16405274,
+           0.44060912, 0.27058614])
     >>> stress(original, projected, metric=False)
-    array([0.33947258, 0.29692937, 0.30478874, 0.10509128, 0.2516135 ,
-           0.2901905 , 0.1662822 , 0.13153341, 0.34299717, 0.164696  ,
-           0.35266095, 0.35276684])
-
-
+    array([0.36599664, 0.39465927, 0.27349092, 0.25096851, 0.31476019,
+           0.27612935, 0.3064739 , 0.26141414, 0.2635681 , 0.25811772,
+           0.36113025, 0.29740821])
+    >>> stress(original, projected, 1)
+    0.316031007598
+    >>> stress(original, projected, 1, metric=False)
+    0.39465927169
 
     Parameters
     ----------
     X
         matrix with an instance by row in a given space (often the original one)
     X_
         matrix with an instance by row in another given space (often the projected one)
@@ -591,22 +662,21 @@
     Returns
     -------
 
     """
     tmap = mp.ThreadingPool(**parallel_kwargs).imap if parallel and X.size > parallel_size_trigger else map
     # TODO: parallelize cdist in slices?
     if metric:
-        thread = lambda M, m: cdist(M, M, metric=m)
-        Dsq, D_ = tmap(thread, [X, X_], ["sqeuclidean", "Euclidean"])  # Slowest part (~98%).
-        Dsq /= np.max(Dsq)
-        D = sqrt(Dsq)
-        D_ /= np.max(D_)
+        thread = (lambda M, m: cdist(M, M, metric=m)) if i is None else (lambda M, m: cdist(M[i:i + 1], M, metric=m))
+        D, Dsq_ = tmap(thread, [X, X_], ["Euclidean", "sqeuclidean"])
+        Dsq_ /= Dsq_.max(axis=1, keepdims=True)
+        D_ = sqrt(Dsq_)
     else:
-        thread = lambda M: rankdata(cdist(M, M, metric="sqeuclidean"), method="average", axis=1) - 1
-        D, D_ = tmap(thread, [X, X_])
-        Dsq = D ** 2
-
-    sqdiff = (D - D_) ** 2
-    nume = sum(sqdiff)
-    deno = sum(Dsq)
-    result = np.round(sqrt(nume / deno), 12)
-    return result
+        thread = (lambda M, m: rankdata(cdist(M, M, metric=m), method="average", axis=1) - 1) if i is None else (lambda M, m: rankdata(cdist(M[i:i + 1], M, metric=m), method="average", axis=1) - 1)
+        D, Dsq_ = tmap(thread, [X, X_], ["Euclidean", "sqeuclidean"])
+        Dsq_ /= Dsq_.max(axis=1, keepdims=True)
+        D_ = sqrt(Dsq_)
+
+    D /= D.max(axis=1, keepdims=True)
+    s = ((D - D_) ** 2).sum(axis=1) / 2
+    result = np.round(np.sqrt(s / (Dsq_.sum(axis=1) / 2)), 12)
+    return result if i is None else result[0]
```

### Comparing `sortedness-0.230710.0/src/sortedness/matrices.py` & `sortedness-1.230711.1/src/sortedness/matrices.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/parallel.py` & `sortedness-1.230711.1/src/sortedness/parallel.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/rank.py` & `sortedness-1.230711.1/src/sortedness/rank.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/trustworthiness.py` & `sortedness-1.230711.1/src/sortedness/trustworthiness.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/wtau/__init__.py` & `sortedness-1.230711.1/src/sortedness/wtau/__init__.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/wtau/wtau.c` & `sortedness-1.230711.1/src/sortedness/wtau/wtau.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 /* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/npy_math.h",
-            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/npy_math.h",
+            "/tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3",
             "-ffast-math",
             "-march=native",
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "include_dirs": [
-            "/tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "sortedness.wtau.wtau",
         "sources": [
             "src/sortedness/wtau/wtau.pyx"
@@ -1136,177 +1136,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1337,42 +1337,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -10659,15 +10659,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_perm, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10676,29 +10676,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10709,15 +10709,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10726,29 +10726,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10759,15 +10759,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10776,29 +10776,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10809,15 +10809,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10826,29 +10826,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10859,15 +10859,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10876,29 +10876,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10909,89 +10909,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":925
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -10999,33 +10999,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":925
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -11033,96 +11033,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":931
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":937
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11138,15 +11138,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -11154,53 +11154,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
+      /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
@@ -11208,30 +11208,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11246,15 +11246,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11270,15 +11270,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11286,53 +11286,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
@@ -11340,30 +11340,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11378,15 +11378,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11402,15 +11402,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11418,53 +11418,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
@@ -11472,30 +11472,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11510,176 +11510,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":963
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":975
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":963
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":990
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1000
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+/* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25665,26 +25665,26 @@
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/tmpzja0q3nd/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/tmp72gpi3dz/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 947, __pyx_L1_error)
```

### Comparing `sortedness-0.230710.0/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so` & `sortedness-1.230711.1/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/wtau/wtau.html` & `sortedness-1.230711.1/src/sortedness/wtau/wtau.html`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/src/sortedness/wtau/wtau.pyx` & `sortedness-1.230711.1/src/sortedness/wtau/wtau.pyx`

 * *Files identical despite different names*

### Comparing `sortedness-0.230710.0/setup.py` & `sortedness-1.230711.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['lange>=1.230203.1,<2.0.0', 'pathos>=0.3.0,<0.4.0']
 
 extras_require = \
 {':python_version >= "3.8" and python_version < "3.11"': ['scipy>=1.10.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'sortedness',
-    'version': '0.230710.0',
+    'version': '1.230711.1',
     'description': 'Measures of projection quality',
-    'long_description': '![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/sortedness)\n<a href="https://pypi.org/project/sortedness">\n<img src="https://img.shields.io/github/v/release/sortedness/sortedness?display_name=tag&sort=semver&color=blue" alt="github">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!-- [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->\n[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)\n[![DOI](https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)\n[![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)\n\n\n# sortedness\n\n`sortedness` is a measure of quality of data transformation, often dimensionality reduction.\nIt is less sensitive to irrelevant distortions and return values in a more meaningful interval than Kruskal stress formula I.\n<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).\n\n## Overview\nLocal variants return a value for each provided point. The global variant returns a single value for all points.\nAny local variant can be used as a global measure by taking the mean value.\n\nLocal variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.\n\nGlobal variant: `global_sortedness(X, X_)`.\n\n## Python installation\n### from package through pip\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install -U sortedness\n```\n\n### from source\n```bash\ngit clone https://github.com/sortedness/sortedness\ncd sortedness\npoetry install\n```\n\n\n### Examples\n\n**Sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import sortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = sortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.432937128932 0.7813889452999166 0.944810120534\n"""\n```\n\n```python3\n\ns = sortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.578096068617 -0.06328160775358334 0.396112816715\n"""\n```\n\n\n</p>\n</details>\n\n**Pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = pwsortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.730078995423 0.7744573488776667 0.837310352695\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.198780473657 -0.0645984203715 0.147224384381\n"""\n```\n\n\n</p>\n</details>\n\n**Sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import global_pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print measurement result and p-value.\ns = global_pwsortedness(original, original)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected2)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected1)\nprint(list(s))\n"""\n[0.7715617715617715, 5.240847664048334e-20]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projectedrnd)\nprint(list(s))\n"""\n[-0.06107226107226107, 0.46847188611226276]\n"""\n```\n\n\n</p>\n</details>\n\n\n** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves**\n\n\n\n\n\n## Grants\n',
+    'long_description': '![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/sortedness)\n<a href="https://pypi.org/project/sortedness">\n<img src="https://img.shields.io/github/v/release/sortedness/sortedness?display_name=tag&sort=semver&color=blue" alt="github">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!-- [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->\n[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)\n[![DOI](https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)\n[![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)\n\n\n# sortedness\n\n`sortedness` is the level of agreement between two points regarding to how they rank all remaining points in a dataset.\nThis ia valid even for points from different spaces, enabling the measurement of the quality of data transformation processes, often dimensionality reduction.\nIt is less sensitive to irrelevant distortions, and return values in a more meaningful interval, than Kruskal stress formula I.\n<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).\n\n## Overview\nLocal variants return a value for each provided point. The global variant returns a single value for all points.\nAny local variant can be used as a global measure by taking the mean value.\n\nLocal variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.\n\nGlobal variant: `global_sortedness(X, X_)`.\n\n## Python installation\n### from package through pip\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install -U sortedness\n```\n\n### from source\n```bash\ngit clone https://github.com/sortedness/sortedness\ncd sortedness\npoetry install\n```\n\n\n### Examples\n\n**Sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import sortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = sortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.393463224666 0.7565797804351666 0.944810120534\n"""\n```\n\n```python3\n\ns = sortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.648305479567 -0.09539895194975 0.397019507592\n"""\n```\n\n```python3\n\n# Single point fast calculation.\ns = sortedness(original, projectedrnd, 2)\nprint(s)\n"""\n0.231079547491\n"""\n```\n\n\n</p>\n</details>\n\n**Pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = pwsortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.649315577592 0.7534291438323333 0.834601601062\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.168611098044 -0.07988253899799999 0.14442446342\n"""\n```\n\n```python3\n\n# Single point fast calculation.\ns = pwsortedness(original, projectedrnd, 2)\nprint(s)\n"""\n0.036119718802\n"""\n```\n\n\n</p>\n</details>\n\n**Global pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import global_pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print measurement result and p-value.\ns = global_pwsortedness(original, original)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected2)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected1)\nprint(list(s))\n"""\n[0.7715617715617715, 5.240847664048334e-20]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projectedrnd)\nprint(list(s))\n"""\n[-0.06107226107226107, 0.46847188611226276]\n"""\n```\n\n\n</p>\n</details>\n\n\n** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves**\n\n\n### TODO\nFuture work address handling large datasets: approximate sortedness value, and size-insensitive weighting scheme.\n\n## Reference\nPlease use the following reference to cite this work:\n```\n@inproceedings {10.2312:eurova.20231093,\nbooktitle = {EuroVis Workshop on Visual Analytics (EuroVA)},\neditor = {Angelini, Marco and El-Assady, Mennatallah},\ntitle = {{Nonparametric Dimensionality Reduction Quality Assessment based on Sortedness of Unrestricted Neighborhood}},\nauthor = {Pereira-Santos, Davi and Neves, Tácito Trindade Araújo Tiburtino and Carvalho, André C. P. L. F. de and Paulovich, Fernando V.},\nyear = {2023},\npublisher = {The Eurographics Association},\nISSN = {2664-4487},\nISBN = {978-3-03868-222-6},\nDOI = {10.2312/eurova.20231093}\n}\n```\n\n## Grants\nThis work was supported by Wellcome Leap 1kD Program; São\nPaulo Research Foundation (FAPESP) - grant 2020/09835-1; Cana-\ndian Institute for Health Research (CIHR) Canadian Research\nChairs (CRC) stipend [award number 1024586]; Canadian Foun-\ndation for Innovation (CFI) John R. Evans Leaders Fund (JELF)\n[grant number 38835]; Dalhousie Medical Research Fund (DMRF)\nCOVID-19 Research Grant [grant number 603082]; and the Cana-\ndian Institute for Health Research (CIHR) Project Grant [award\nnumber 177968].\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['sortedness', 'sortedness.evaluation', 'sortedness.wtau']
 package_data = \ {'': ['*']} install_requires = \ ['lange>=1.230203.1,<2.0.0',
 'pathos>=0.3.0,<0.4.0'] extras_require = \ {':python_version >= "3.8" and
 python_version < "3.11"': ['scipy>=1.10.1,<2.0.0']} setup_kwargs = { 'name':
-'sortedness', 'version': '0.230710.0', 'description': 'Measures of projection
+'sortedness', 'version': '1.230711.1', 'description': 'Measures of projection
 quality', 'long_description': '![test](https://github.com/sortedness/
 sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/
 sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/
 sortedness/sortedness)\n\n[github]\n\n![Python version](https://img.shields.io/
 badge/python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/
 License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[![API
 documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)]
 (https://sortedness.github.io/sortedness)\n[![DOI](https://zenodo.org/badge/
 513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)\n[![Downloads]
 (https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/
-sortedness)\n\n\n# sortedness\n\n`sortedness` is a measure of quality of data
-transformation, often dimensionality reduction.\nIt is less sensitive to
-irrelevant distortions and return values in a more meaningful interval than
-Kruskal stress formula I.\n
+sortedness)\n\n\n# sortedness\n\n`sortedness` is the level of agreement between
+two points regarding to how they rank all remaining points in a dataset.\nThis
+ia valid even for points from different spaces, enabling the measurement of the
+quality of data transformation processes, often dimensionality reduction.\nIt
+is less sensitive to irrelevant distortions, and return values in a more
+meaningful interval, than Kruskal stress formula I.\n
 This [Python library](https://pypi.org/project/sortedness) / [code](https://
 github.com/sortedness/sortedness) provides a reference implementation for the
 functions presented [here (paper unavailable until publication)](https://
 scholar.google.com/
 scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).\n\n##
 Overview\nLocal variants return a value for each provided point. The global
 variant returns a single value for all points.\nAny local variant can be used
@@ -39,35 +41,39 @@
 size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1
 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd
 = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns =
 sortedness(original, original)\nprint(min(s), sum(s) / len(s), max
 (s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original,
 projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0
 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected1)\nprint(min
-(s), sum(s) / len(s), max(s))\n"""\n0.432937128932 0.7813889452999166
+(s), sum(s) / len(s), max(s))\n"""\n0.393463224666 0.7565797804351666
 0.944810120534\n"""\n```\n\n```python3\n\ns = sortedness(original,
-projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.578096068617 -
-0.06328160775358334 0.396112816715\n"""\n```\n\n\n
+projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.648305479567 -
+0.09539895194975 0.397019507592\n"""\n```\n\n```python3\n\n# Single point fast
+calculation.\ns = sortedness(original, projectedrnd, 2)\nprint
+(s)\n"""\n0.231079547491\n"""\n```\n\n\n
 \n\n\n**Pairwise sortedness**\n\n
 \n\n```python3\n\nimport numpy as np\nfrom numpy.random import
 permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import
 pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng =
 np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov,
 size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1
 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd
 = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns =
 pwsortedness(original, original)\nprint(min(s), sum(s) / len(s), max
 (s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original,
 projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0
 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected1)\nprint
-(min(s), sum(s) / len(s), max(s))\n"""\n0.730078995423 0.7744573488776667
-0.837310352695\n"""\n```\n\n```python3\n\ns = pwsortedness(original,
-projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.198780473657 -
-0.0645984203715 0.147224384381\n"""\n```\n\n\n
-\n\n\n**Sortedness**\n\n
+(min(s), sum(s) / len(s), max(s))\n"""\n0.649315577592 0.7534291438323333
+0.834601601062\n"""\n```\n\n```python3\n\ns = pwsortedness(original,
+projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.168611098044 -
+0.07988253899799999 0.14442446342\n"""\n```\n\n```python3\n\n# Single point
+fast calculation.\ns = pwsortedness(original, projectedrnd, 2)\nprint
+(s)\n"""\n0.036119718802\n"""\n```\n\n\n
+\n\n\n**Global pairwise sortedness**\n\n
 \n\n```python3\n\nimport numpy as np\nfrom numpy.random import
 permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import
 global_pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye
 (2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal
 (mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform
 (original)\nprojected1 = PCA(n_components=1).fit_transform
 (original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print
@@ -77,13 +83,30 @@
 projected2)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-
 93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original,
 projected1)\nprint(list(s))\n"""\n[0.7715617715617715, 5.240847664048334e-
 20]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original,
 projectedrnd)\nprint(list(s))\n"""\n[-0.06107226107226107,
 0.46847188611226276]\n"""\n```\n\n\n
 \n\n\n\n** Copyright (c) 2023. Davi Pereira dos Santos and Tacito
-Neves**\n\n\n\n\n\n## Grants\n', 'author': 'davips', 'author_email':
-'dpsabc@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'None', 'package_dir': package_dir, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'extras_require':
-extras_require, 'python_requires': '>=3.10,<4.0', } from build import * build
-(setup_kwargs) setup(**setup_kwargs)
+Neves**\n\n\n### TODO\nFuture work address handling large datasets: approximate
+sortedness value, and size-insensitive weighting scheme.\n\n##
+Reference\nPlease use the following reference to cite this work:
+\n```\n@inproceedings {10.2312:eurova.20231093,\nbooktitle = {EuroVis Workshop
+on Visual Analytics (EuroVA)},\neditor = {Angelini, Marco and El-Assady,
+Mennatallah},\ntitle = {{Nonparametric Dimensionality Reduction Quality
+Assessment based on Sortedness of Unrestricted Neighborhood}},\nauthor =
+{Pereira-Santos, Davi and Neves, TÃ¡cito Trindade AraÃºjo Tiburtino and
+Carvalho, AndrÃ© C. P. L. F. de and Paulovich, Fernando V.},\nyear =
+{2023},\npublisher = {The Eurographics Association},\nISSN = {2664-4487},\nISBN
+= {978-3-03868-222-6},\nDOI = {10.2312/eurova.20231093}\n}\n```\n\n##
+Grants\nThis work was supported by Wellcome Leap 1kD Program; SÃ£o\nPaulo
+Research Foundation (FAPESP) - grant 2020/09835-1; Cana-\ndian Institute for
+Health Research (CIHR) Canadian Research\nChairs (CRC) stipend [award number
+1024586]; Canadian Foun-\ndation for Innovation (CFI) John R. Evans Leaders
+Fund (JELF)\n[grant number 38835]; Dalhousie Medical Research Fund
+(DMRF)\nCOVID-19 Research Grant [grant number 603082]; and the Cana-\ndian
+Institute for Health Research (CIHR) Project Grant [award\nnumber 177968].\n',
+'author': 'davips', 'author_email': 'dpsabc@gmail.com', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'None', 'package_dir': package_dir,
+'packages': packages, 'package_data': package_data, 'install_requires':
+install_requires, 'extras_require': extras_require, 'python_requires':
+'>=3.10,<4.0', } from build import * build(setup_kwargs) setup(**setup_kwargs)
```

### Comparing `sortedness-0.230710.0/PKG-INFO` & `sortedness-1.230711.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortedness
-Version: 0.230710.0
+Version: 1.230711.1
 Summary: Measures of projection quality
 License: GPLv3
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -27,16 +27,17 @@
 [![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)
 [![DOI](https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)
 [![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)
 
 
 # sortedness
 
-`sortedness` is a measure of quality of data transformation, often dimensionality reduction.
-It is less sensitive to irrelevant distortions and return values in a more meaningful interval than Kruskal stress formula I.
+`sortedness` is the level of agreement between two points regarding to how they rank all remaining points in a dataset.
+This ia valid even for points from different spaces, enabling the measurement of the quality of data transformation processes, often dimensionality reduction.
+It is less sensitive to irrelevant distortions, and return values in a more meaningful interval, than Kruskal stress formula I.
 <br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 
 ## Overview
 Local variants return a value for each provided point. The global variant returns a single value for all points.
 Any local variant can be used as a global measure by taking the mean value.
 
 Local variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.
@@ -104,24 +105,34 @@
 ```
 
 ```python3
 
 s = sortedness(original, projected1)
 print(min(s), sum(s) / len(s), max(s))
 """
-0.432937128932 0.7813889452999166 0.944810120534
+0.393463224666 0.7565797804351666 0.944810120534
 """
 ```
 
 ```python3
 
 s = sortedness(original, projectedrnd)
 print(min(s), sum(s) / len(s), max(s))
 """
--0.578096068617 -0.06328160775358334 0.396112816715
+-0.648305479567 -0.09539895194975 0.397019507592
+"""
+```
+
+```python3
+
+# Single point fast calculation.
+s = sortedness(original, projectedrnd, 2)
+print(s)
+"""
+0.231079547491
 """
 ```
 
 
 </p>
 </details>
 
@@ -165,32 +176,42 @@
 ```
 
 ```python3
 
 s = pwsortedness(original, projected1)
 print(min(s), sum(s) / len(s), max(s))
 """
-0.730078995423 0.7744573488776667 0.837310352695
+0.649315577592 0.7534291438323333 0.834601601062
 """
 ```
 
 ```python3
 
 s = pwsortedness(original, projectedrnd)
 print(min(s), sum(s) / len(s), max(s))
 """
--0.198780473657 -0.0645984203715 0.147224384381
+-0.168611098044 -0.07988253899799999 0.14442446342
+"""
+```
+
+```python3
+
+# Single point fast calculation.
+s = pwsortedness(original, projectedrnd, 2)
+print(s)
+"""
+0.036119718802
 """
 ```
 
 
 </p>
 </details>
 
-**Sortedness**
+**Global pairwise sortedness**
 <details>
 <p>
 
 ```python3
 
 import numpy as np
 from numpy.random import permutation
@@ -247,12 +268,37 @@
 </p>
 </details>
 
 
 ** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves**
 
 
+### TODO
+Future work address handling large datasets: approximate sortedness value, and size-insensitive weighting scheme.
 
-
+## Reference
+Please use the following reference to cite this work:
+```
+@inproceedings {10.2312:eurova.20231093,
+booktitle = {EuroVis Workshop on Visual Analytics (EuroVA)},
+editor = {Angelini, Marco and El-Assady, Mennatallah},
+title = {{Nonparametric Dimensionality Reduction Quality Assessment based on Sortedness of Unrestricted Neighborhood}},
+author = {Pereira-Santos, Davi and Neves, Tácito Trindade Araújo Tiburtino and Carvalho, André C. P. L. F. de and Paulovich, Fernando V.},
+year = {2023},
+publisher = {The Eurographics Association},
+ISSN = {2664-4487},
+ISBN = {978-3-03868-222-6},
+DOI = {10.2312/eurova.20231093}
+}
+```
 
 ## Grants
+This work was supported by Wellcome Leap 1kD Program; São
+Paulo Research Foundation (FAPESP) - grant 2020/09835-1; Cana-
+dian Institute for Health Research (CIHR) Canadian Research
+Chairs (CRC) stipend [award number 1024586]; Canadian Foun-
+dation for Innovation (CFI) John R. Evans Leaders Fund (JELF)
+[grant number 38835]; Dalhousie Medical Research Fund (DMRF)
+COVID-19 Research Grant [grant number 603082]; and the Cana-
+dian Institute for Health Research (CIHR) Project Grant [award
+number 177968].
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sortedness Version: 0.230710.0 Summary: Measures of
+Metadata-Version: 2.1 Name: sortedness Version: 1.230711.1 Summary: Measures of
 projection quality License: GPLv3 Author: davips Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lange (>=1.230203.1,<2.0.0) Requires-Dist: pathos
 (>=0.3.0,<0.4.0) Requires-Dist: scipy (>=1.10.1,<2.0.0) ; python_version >=
 "3.8" and python_version < "3.11" Description-Content-Type: text/markdown !
@@ -11,18 +11,20 @@
 badge.svg)](https://codecov.io/gh/sortedness/sortedness) [github] ![Python
 version](https://img.shields.io/badge/python-3.8+-blue.svg) [![license: GPL v3]
 (https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
 licenses/gpl-3.0)  [![API documentation](https://img.shields.io/badge/doc-
 API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness) [![DOI]
 (https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/
 513273889) [![Downloads](https://static.pepy.tech/badge/sortedness)](https://
-pepy.tech/project/sortedness) # sortedness `sortedness` is a measure of quality
-of data transformation, often dimensionality reduction. It is less sensitive to
-irrelevant distortions and return values in a more meaningful interval than
-Kruskal stress formula I.
+pepy.tech/project/sortedness) # sortedness `sortedness` is the level of
+agreement between two points regarding to how they rank all remaining points in
+a dataset. This ia valid even for points from different spaces, enabling the
+measurement of the quality of data transformation processes, often
+dimensionality reduction. It is less sensitive to irrelevant distortions, and
+return values in a more meaningful interval, than Kruskal stress formula I.
 This [Python library](https://pypi.org/project/sortedness) / [code](https://
 github.com/sortedness/sortedness) provides a reference implementation for the
 functions presented [here (paper unavailable until publication)](https://
 scholar.google.com/
 scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 ## Overview Local variants return a value for each provided point. The global
 variant returns a single value for all points. Any local variant can be used as
@@ -39,42 +41,63 @@
 (seed=0) original = rng.multivariate_normal(mean, cov, size=12) projected2 =
 PCA(n_components=2).fit_transform(original) projected1 = PCA
 (n_components=1).fit_transform(original) np.random.seed(0) projectedrnd =
 permutation(original) # Print `min`, `mean`, and `max` values. s = sortedness
 (original, original) print(min(s), sum(s) / len(s), max(s)) """ 1.0 1.0 1.0 """
 ``` ```python3 s = sortedness(original, projected2) print(min(s), sum(s) / len
 (s), max(s)) """ 1.0 1.0 1.0 """ ``` ```python3 s = sortedness(original,
-projected1) print(min(s), sum(s) / len(s), max(s)) """ 0.432937128932
-0.7813889452999166 0.944810120534 """ ``` ```python3 s = sortedness(original,
-projectedrnd) print(min(s), sum(s) / len(s), max(s)) """ -0.578096068617 -
-0.06328160775358334 0.396112816715 """ ```
+projected1) print(min(s), sum(s) / len(s), max(s)) """ 0.393463224666
+0.7565797804351666 0.944810120534 """ ``` ```python3 s = sortedness(original,
+projectedrnd) print(min(s), sum(s) / len(s), max(s)) """ -0.648305479567 -
+0.09539895194975 0.397019507592 """ ``` ```python3 # Single point fast
+calculation. s = sortedness(original, projectedrnd, 2) print(s) """
+0.231079547491 """ ```
  **Pairwise sortedness**
 ```python3 import numpy as np from numpy.random import permutation from
 sklearn.decomposition import PCA from sortedness import pwsortedness # Some
 synthetic data. mean = (1, 2) cov = np.eye(2) rng = np.random.default_rng
 (seed=0) original = rng.multivariate_normal(mean, cov, size=12) projected2 =
 PCA(n_components=2).fit_transform(original) projected1 = PCA
 (n_components=1).fit_transform(original) np.random.seed(0) projectedrnd =
 permutation(original) # Print `min`, `mean`, and `max` values. s = pwsortedness
 (original, original) print(min(s), sum(s) / len(s), max(s)) """ 1.0 1.0 1.0 """
 ``` ```python3 s = pwsortedness(original, projected2) print(min(s), sum(s) /
 len(s), max(s)) """ 1.0 1.0 1.0 """ ``` ```python3 s = pwsortedness(original,
-projected1) print(min(s), sum(s) / len(s), max(s)) """ 0.730078995423
-0.7744573488776667 0.837310352695 """ ``` ```python3 s = pwsortedness(original,
-projectedrnd) print(min(s), sum(s) / len(s), max(s)) """ -0.198780473657 -
-0.0645984203715 0.147224384381 """ ```
- **Sortedness**
+projected1) print(min(s), sum(s) / len(s), max(s)) """ 0.649315577592
+0.7534291438323333 0.834601601062 """ ``` ```python3 s = pwsortedness(original,
+projectedrnd) print(min(s), sum(s) / len(s), max(s)) """ -0.168611098044 -
+0.07988253899799999 0.14442446342 """ ``` ```python3 # Single point fast
+calculation. s = pwsortedness(original, projectedrnd, 2) print(s) """
+0.036119718802 """ ```
+ **Global pairwise sortedness**
 ```python3 import numpy as np from numpy.random import permutation from
 sklearn.decomposition import PCA from sortedness import global_pwsortedness #
 Some synthetic data. mean = (1, 2) cov = np.eye(2) rng = np.random.default_rng
 (seed=0) original = rng.multivariate_normal(mean, cov, size=12) projected2 =
 PCA(n_components=2).fit_transform(original) projected1 = PCA
 (n_components=1).fit_transform(original) np.random.seed(0) projectedrnd =
 permutation(original) # Print measurement result and p-value. s =
 global_pwsortedness(original, original) print(list(s)) """ [1.0,
 3.6741408919675163e-93] """ ``` ```python3 s = global_pwsortedness(original,
 projected2) print(list(s)) """ [1.0, 3.6741408919675163e-93] """ ``` ```python3
 s = global_pwsortedness(original, projected1) print(list(s)) """
 [0.7715617715617715, 5.240847664048334e-20] """ ``` ```python3 s =
 global_pwsortedness(original, projectedrnd) print(list(s)) """ [-
 0.06107226107226107, 0.46847188611226276] """ ```
- ** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves** ## Grants
+ ** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves** ### TODO
+Future work address handling large datasets: approximate sortedness value, and
+size-insensitive weighting scheme. ## Reference Please use the following
+reference to cite this work: ``` @inproceedings {10.2312:eurova.20231093,
+booktitle = {EuroVis Workshop on Visual Analytics (EuroVA)}, editor =
+{Angelini, Marco and El-Assady, Mennatallah}, title = {{Nonparametric
+Dimensionality Reduction Quality Assessment based on Sortedness of Unrestricted
+Neighborhood}}, author = {Pereira-Santos, Davi and Neves, TÃ¡cito Trindade
+AraÃºjo Tiburtino and Carvalho, AndrÃ© C. P. L. F. de and Paulovich, Fernando
+V.}, year = {2023}, publisher = {The Eurographics Association}, ISSN = {2664-
+4487}, ISBN = {978-3-03868-222-6}, DOI = {10.2312/eurova.20231093} } ``` ##
+Grants This work was supported by Wellcome Leap 1kD Program; SÃ£o Paulo
+Research Foundation (FAPESP) - grant 2020/09835-1; Cana- dian Institute for
+Health Research (CIHR) Canadian Research Chairs (CRC) stipend [award number
+1024586]; Canadian Foun- dation for Innovation (CFI) John R. Evans Leaders Fund
+(JELF) [grant number 38835]; Dalhousie Medical Research Fund (DMRF) COVID-19
+Research Grant [grant number 603082]; and the Cana- dian Institute for Health
+Research (CIHR) Project Grant [award number 177968].
```

