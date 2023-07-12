# Comparing `tmp/pymc-experimental-0.0.7.tar.gz` & `tmp/pymc-experimental-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-experimental-0.0.7.tar", last modified: Sat Jun 10 09:24:10 2023, max compression
+gzip compressed data, was "pymc-experimental-0.0.8.tar", last modified: Wed Jul 12 08:10:32 2023, max compression
```

## Comparing `pymc-experimental-0.0.7.tar` & `pymc-experimental-0.0.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.905581 pymc-experimental-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-10 09:24:10.905581 pymc-experimental-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.893581 pymc-experimental-0.0.7/pymc_experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/histogram_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/distributions/multivariate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/multivariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/multivariate/r2d2m2cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/distributions/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/gp/latent_approx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/inference/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/inference/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/model_transform/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/model_transform/conditioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/preprocessing/standard_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.901581 pymc-experimental-0.0.7/pymc_experimental/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.901581 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_multivariate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.901581 pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/test_conditioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_histogram_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_prior_from_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/test_splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.901581 pymc-experimental-0.0.7/pymc_experimental/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/tests/utils/test_model_fgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.905581 pymc-experimental-0.0.7/pymc_experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/model_fgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/pytensorf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/utils/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pymc_experimental/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:24:10.897581 pymc-experimental-0.0.7/pymc_experimental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-10 09:24:10.000000 pymc-experimental-0.0.7/pymc_experimental.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-10 09:24:10.905581 pymc-experimental-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-10 09:24:00.000000 pymc-experimental-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/histogram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/distributions/multivariate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/multivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/multivariate/r2d2m2cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/distributions/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/gp/latent_approx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/inference/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/inference/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/model_transform/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/model_transform/conditioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/preprocessing/standard_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_multivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/test_conditioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_histogram_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_prior_from_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/tests/utils/test_model_fgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/pymc_experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/model_fgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/pytensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/utils/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pymc_experimental/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:10:32.128877 pymc-experimental-0.0.8/pymc_experimental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 08:10:32.000000 pymc-experimental-0.0.8/pymc_experimental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 08:10:32.132877 pymc-experimental-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-12 08:10:20.000000 pymc-experimental-0.0.8/setup.py
```

### Comparing `pymc-experimental-0.0.7/CODE_OF_CONDUCT.md` & `pymc-experimental-0.0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/LICENSE` & `pymc-experimental-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/PKG-INFO` & `pymc-experimental-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.7
+Version: 0.0.8
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.7 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.8 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `pymc-experimental-0.0.7/README.md` & `pymc-experimental-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/__init__.py` & `pymc-experimental-0.0.8/pymc_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/distributions/__init__.py` & `pymc-experimental-0.0.8/pymc_experimental/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/distributions/continuous.py` & `pymc-experimental-0.0.8/pymc_experimental/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/distributions/discrete.py` & `pymc-experimental-0.0.8/pymc_experimental/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/distributions/histogram_utils.py` & `pymc-experimental-0.0.8/pymc_experimental/distributions/histogram_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/distributions/timeseries.py` & `pymc-experimental-0.0.8/pymc_experimental/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/gp/__init__.py` & `pymc-experimental-0.0.8/pymc_experimental/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/gp/latent_approx.py` & `pymc-experimental-0.0.8/pymc_experimental/gp/latent_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/inference/__init__.py` & `pymc-experimental-0.0.8/pymc_experimental/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/inference/fit.py` & `pymc-experimental-0.0.8/pymc_experimental/inference/fit.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/inference/pathfinder.py` & `pymc-experimental-0.0.8/pymc_experimental/inference/pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/linearmodel.py` & `pymc-experimental-0.0.8/pymc_experimental/linearmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,18 @@
             "draws": 1_000,
             "tune": 1_000,
             "chains": 3,
             "target_accept": 0.95,
         }
 
     @property
+    def _serializable_model_config(self) -> Dict:
+        return self.model_config
+
+    @property
     def output_var(self):
         return "y_hat"
 
     def build_model(self, X: pd.DataFrame, y: pd.Series):
         """
         Build the PyMC model.
```

### Comparing `pymc-experimental-0.0.7/pymc_experimental/marginal_model.py` & `pymc-experimental-0.0.8/pymc_experimental/marginal_model.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/model_builder.py` & `pymc-experimental-0.0.8/pymc_experimental/model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
 import hashlib
 import json
+import warnings
 from abc import abstractmethod
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import arviz as az
 import numpy as np
 import pandas as pd
@@ -293,15 +294,15 @@
 
         with self.model:
             sampler_args = {**self.sampler_config, **kwargs}
             idata = pm.sample(**sampler_args)
             idata.extend(pm.sample_prior_predictive())
             idata.extend(pm.sample_posterior_predictive(idata))
 
-        self.set_idata_attrs(idata)
+        idata = self.set_idata_attrs(idata)
         return idata
 
     def set_idata_attrs(self, idata=None):
         """
         Set attributes on an InferenceData object.
 
         Parameters
@@ -334,14 +335,18 @@
         if idata is None:
             raise RuntimeError("No idata provided to set attrs on.")
         idata.attrs["id"] = self.id
         idata.attrs["model_type"] = self._model_type
         idata.attrs["version"] = self.version
         idata.attrs["sampler_config"] = json.dumps(self.sampler_config)
         idata.attrs["model_config"] = json.dumps(self._serializable_model_config)
+        # Only classes with non-dataset parameters will implement save_input_params
+        if hasattr(self, "_save_input_params"):
+            self._save_input_params(idata)
+        return idata
 
     def save(self, fname: str) -> None:
         """
         Save the model's inference data to a file.
 
         Parameters
         ----------
@@ -372,14 +377,25 @@
         if self.idata is not None and "posterior" in self.idata:
             file = Path(str(fname))
             self.idata.to_netcdf(str(file))
         else:
             raise RuntimeError("The model hasn't been fit yet, call .fit() first")
 
     @classmethod
+    def _convert_dims_to_tuple(cls, model_config: Dict) -> Dict:
+        for key in model_config:
+            if (
+                isinstance(model_config[key], dict)
+                and "dims" in model_config[key]
+                and isinstance(model_config[key]["dims"], list)
+            ):
+                model_config[key]["dims"] = tuple(model_config[key]["dims"])
+        return model_config
+
+    @classmethod
     def load(cls, fname: str):
         """
         Creates a ModelBuilder instance from a file,
         Loads inference data for the model.
 
         Parameters
         ----------
@@ -399,16 +415,18 @@
         >>> class MyModel(ModelBuilder):
         >>>     ...
         >>> name = './mymodel.nc'
         >>> imported_model = MyModel.load(name)
         """
         filepath = Path(str(fname))
         idata = az.from_netcdf(filepath)
+        # needs to be converted, because json.loads was changing tuple to list
+        model_config = cls._convert_dims_to_tuple(json.loads(idata.attrs["model_config"]))
         model = cls(
-            model_config=json.loads(idata.attrs["model_config"]),
+            model_config=model_config,
             sampler_config=json.loads(idata.attrs["sampler_config"]),
         )
         model.idata = idata
         dataset = idata.fit_data.to_dataframe()
         X = dataset.drop(columns=[model.output_var])
         y = dataset[model.output_var]
         model.build_model(X, y)
@@ -475,15 +493,22 @@
         sampler_config["random_seed"] = random_seed
         sampler_config.update(**kwargs)
         self.idata = self.sample_model(**sampler_config)
 
         X_df = pd.DataFrame(X, columns=X.columns)
         combined_data = pd.concat([X_df, y], axis=1)
         assert all(combined_data.columns), "All columns must have non-empty names"
-        self.idata.add_groups(fit_data=combined_data.to_xarray())  # type: ignore
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                category=UserWarning,
+                message="The group fit_data is not defined in the InferenceData scheme",
+            )
+            self.idata.add_groups(fit_data=combined_data.to_xarray())  # type: ignore
+
         return self.idata  # type: ignore
 
     def predict(
         self,
         X_pred: Union[np.ndarray, pd.DataFrame, pd.Series],
         extend_idata: bool = True,
         **kwargs,
```

### Comparing `pymc-experimental-0.0.7/pymc_experimental/model_transform/basic.py` & `pymc-experimental-0.0.8/pymc_experimental/model_transform/basic.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/model_transform/conditioning.py` & `pymc-experimental-0.0.8/pymc_experimental/model_transform/conditioning.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/preprocessing/standard_scaler.py` & `pymc-experimental-0.0.8/pymc_experimental/preprocessing/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/__init__.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/distributions/__init__.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_continuous.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_discrete.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/distributions/test_discrete_markov_chain.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/distributions/test_discrete_markov_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     P = np.full((n_states,) * (n_lags + 1), 1 / n_states)
     x0 = pm.Categorical.dist(p=np.ones(n_states) / n_states)
 
     chain = DiscreteMarkovChain.dist(
         P=pt.as_tensor_variable(P), init_dist=x0, steps=steps, n_lags=n_lags
     )
 
-    draws = pm.draw(chain, n_draws)
+    draws = pm.draw(chain, n_draws, random_seed=172)
 
     # Test x0 is uniform over n_states
     for i in range(n_lags):
         assert np.allclose(
             np.histogram(draws[:, ..., i], bins=n_states)[0] / n_draws, 1 / n_states, atol=atol
         )
```

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/test_basic.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/test_basic.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/model_transform/test_conditioning.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/model_transform/test_conditioning.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,44 +88,45 @@
         x = pm.Normal("x", dims="test_dim")
 
     m_new = observe(m_old, {x: np.arange(5, dtype=config.floatX)})
     assert m_new.named_vars_to_dims["x"] == ["test_dim"]
 
 
 def test_do():
+    rng = np.random.default_rng(seed=435)
     with pm.Model() as m_old:
         x = pm.Normal("x", 0, 1e-3)
         y = pm.Normal("y", x, 1e-3)
         z = pm.Normal("z", y + x, 1e-3)
 
-    assert -5 < pm.draw(z) < 5
+    assert -5 < pm.draw(z, random_seed=rng) < 5
 
     m_new = do(m_old, {y: x + 100})
 
     assert len(m_new.free_RVs) == 2
     assert m_new["x"] in m_new.free_RVs
     assert m_new["y"] in m_new.deterministics
     assert m_new["z"] in m_new.free_RVs
 
-    assert 95 < pm.draw(m_new["z"]) < 105
+    assert 95 < pm.draw(m_new["z"], random_seed=rng) < 105
 
     # Test two substitutions
     with m_old:
         switch = pm.MutableData("switch", 1)
     m_new = do(m_old, {y: 100 * switch, x: 100 * switch})
 
     assert len(m_new.free_RVs) == 1
     assert m_new["y"] not in m_new.deterministics
     assert m_new["x"] not in m_new.deterministics
     assert m_new["z"] in m_new.free_RVs
 
-    assert 195 < pm.draw(m_new["z"]) < 205
+    assert 195 < pm.draw(m_new["z"], random_seed=rng) < 205
     with m_new:
         pm.set_data({"switch": 0})
-    assert -5 < pm.draw(m_new["z"]) < 5
+    assert -5 < pm.draw(m_new["z"], random_seed=rng) < 5
 
 
 def test_do_posterior_predictive():
     with pm.Model() as m:
         x = pm.Normal("x", 0, 1)
         y = pm.Normal("y", x, 1)
         z = pm.Normal("z", y + x, 1e-3)
@@ -145,30 +146,32 @@
         idata_do = pm.sample_posterior_predictive(idata_m, var_names="z")
 
     assert 120 < idata_do.posterior_predictive["z"].mean() < 130
 
 
 @pytest.mark.parametrize("mutable", (False, True))
 def test_do_constant(mutable):
+    rng = np.random.default_rng(seed=122)
     with pm.Model() as m:
         x = pm.Data("x", 0, mutable=mutable)
         y = pm.Normal("y", x, 1e-3)
 
     do_m = do(m, {x: 105})
-    assert pm.draw(do_m["y"]) > 100
+    assert pm.draw(do_m["y"], random_seed=rng) > 100
 
 
 def test_do_deterministic():
+    rng = np.random.default_rng(seed=435)
     with pm.Model() as m:
         x = pm.Normal("x", 0, 1e-3)
         y = pm.Deterministic("y", x + 105)
         z = pm.Normal("z", y, 1e-3)
 
     do_m = do(m, {"z": x - 105})
-    assert pm.draw(do_m["z"]) < 100
+    assert pm.draw(do_m["z"], random_seed=rng) < 100
 
 
 def test_do_dims():
     coords = {"test_dim": range(10)}
     with pm.Model(coords=coords) as m:
         x = pm.Normal("x", dims="test_dim")
         y = pm.Deterministic("y", x + 5, dims="test_dim")
```

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/test_histogram_approximation.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/test_histogram_approximation.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/test_linearmodel.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/test_linearmodel.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,32 @@
         "target_accept": 0.95,
     }
     model = LinearModel(sampler_config=sampler_config)
     model.fit(toy_X, toy_y)
     return model
 
 
+@pytest.mark.skipif(
+    sys.platform == "win32", reason="Permissions for temp files not granted on windows CI."
+)
+def test_save_load(fitted_linear_model_instance):
+    model = fitted_linear_model_instance
+    temp = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False)
+    model.save(temp.name)
+    model2 = LinearModel.load(temp.name)
+    assert model.idata.groups() == model2.idata.groups()
+
+    X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=100)})
+    pred1 = model.predict(X_pred, random_seed=423)
+    pred2 = model2.predict(X_pred, random_seed=423)
+    # Predictions should be identical
+    np.testing.assert_array_equal(pred1, pred2)
+    temp.close()
+
+
 def test_save_without_fit_raises_runtime_error(toy_X, toy_y):
     test_model = LinearModel()
     with pytest.raises(RuntimeError):
         test_model.save("saved_model")
 
 
 def test_fit(fitted_linear_model_instance):
@@ -79,32 +97,14 @@
     assert len(new_X_pred) == len(pred)
     assert isinstance(pred, np.ndarray)
     post_pred = model.predict_posterior(new_X_pred)
     assert len(new_X_pred) == len(post_pred)
     assert isinstance(post_pred, xr.DataArray)
 
 
-@pytest.mark.skipif(
-    sys.platform == "win32", reason="Permissions for temp files not granted on windows CI."
-)
-def test_save_load(fitted_linear_model_instance):
-    model = fitted_linear_model_instance
-    temp = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False)
-    model.save(temp.name)
-    model2 = LinearModel.load(temp.name)
-    assert model.idata.groups() == model2.idata.groups()
-
-    X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=100)})
-    pred1 = model.predict(X_pred, random_seed=423)
-    pred2 = model2.predict(X_pred, random_seed=423)
-    # Predictions should be identical
-    np.testing.assert_array_equal(pred1, pred2)
-    temp.close()
-
-
 def test_predict(fitted_linear_model_instance):
     model = fitted_linear_model_instance
     X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=100)})
     pred = model.predict(X_pred)
     assert len(X_pred) == len(pred)
     assert np.issubdtype(pred.dtype, np.floating)
```

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/test_marginal_model.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/test_marginal_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,22 +203,22 @@
 @pytest.mark.filterwarnings("error")
 def test_marginalized_change_point_model(disaster_model):
     m, years = disaster_model
 
     ip = m.initial_point()
     ip.pop("switchpoint")
     ref_logp_fn = m.compile_logp(
-        [m["switchpoint"], m["disasters_observed"], m["disasters_missing"]]
+        [m["switchpoint"], m["disasters_observed"], m["disasters_unobserved"]]
     )
     ref_logp = logsumexp([ref_logp_fn({**ip, **{"switchpoint": year}}) for year in years])
 
     with pytest.warns(UserWarning, match="There are multiple dependent variables"):
         m.marginalize(m["switchpoint"])
 
-    logp = m.compile_logp([m["disasters_observed"], m["disasters_missing"]])(ip)
+    logp = m.compile_logp([m["disasters_observed"], m["disasters_unobserved"]])(ip)
     np.testing.assert_almost_equal(logp, ref_logp)
 
 
 @pytest.mark.slow
 @pytest.mark.filterwarnings("error")
 def test_marginalized_change_point_model_sampling(disaster_model):
     m, _ = disaster_model
@@ -237,15 +237,17 @@
     np.testing.assert_allclose(
         before_marg["early_rate"].mean(), after_marg["early_rate"].mean(), rtol=1e-2
     )
     np.testing.assert_allclose(
         before_marg["late_rate"].mean(), after_marg["late_rate"].mean(), rtol=1e-2
     )
     np.testing.assert_allclose(
-        before_marg["disasters_missing"].mean(), after_marg["disasters_missing"].mean(), rtol=1e-2
+        before_marg["disasters_unobserved"].mean(),
+        after_marg["disasters_unobserved"].mean(),
+        rtol=1e-2,
     )
 
 
 @pytest.mark.filterwarnings("error")
 def test_not_supported_marginalized():
     """Marginalized graphs with non-Elemwise Operations are not supported as they
     would violate the batching logp assumption"""
```

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/test_model_builder.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/test_model_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import hashlib
+import json
 import sys
 import tempfile
 from typing import Dict
 
 import numpy as np
 import pandas as pd
 import pymc as pm
@@ -39,57 +40,66 @@
     y = pd.Series(y, name="output")
     return y
 
 
 @pytest.fixture(scope="module")
 def fitted_model_instance(toy_X, toy_y):
     sampler_config = {
-        "draws": 500,
-        "tune": 300,
+        "draws": 100,
+        "tune": 100,
         "chains": 2,
         "target_accept": 0.95,
     }
     model_config = {
-        "a": {"loc": 0, "scale": 10},
+        "a": {"loc": 0, "scale": 10, "dims": ("numbers",)},
         "b": {"loc": 0, "scale": 10},
         "obs_error": 2,
     }
-    model = test_ModelBuilder(model_config=model_config, sampler_config=sampler_config)
+    model = test_ModelBuilder(
+        model_config=model_config, sampler_config=sampler_config, test_parameter="test_paramter"
+    )
     model.fit(toy_X)
     return model
 
 
 class test_ModelBuilder(ModelBuilder):
+    def __init__(self, model_config=None, sampler_config=None, test_parameter=None):
+        self.test_parameter = test_parameter
+        super().__init__(model_config=model_config, sampler_config=sampler_config)
 
-    _model_type = "LinearModel"
+    _model_type = "test_model"
     version = "0.1"
 
     def build_model(self, X: pd.DataFrame, y: pd.Series, model_config=None):
+        coords = {"numbers": np.arange(len(X))}
         self.generate_and_preprocess_model_data(X, y)
-        with pm.Model() as self.model:
+        with pm.Model(coords=coords) as self.model:
             if model_config is None:
                 model_config = self.default_model_config
             x = pm.MutableData("x", self.X["input"].values)
             y_data = pm.MutableData("y_data", self.y)
 
             # prior parameters
             a_loc = model_config["a"]["loc"]
             a_scale = model_config["a"]["scale"]
             b_loc = model_config["b"]["loc"]
             b_scale = model_config["b"]["scale"]
             obs_error = model_config["obs_error"]
 
             # priors
-            a = pm.Normal("a", a_loc, sigma=a_scale)
+            a = pm.Normal("a", a_loc, sigma=a_scale, dims=model_config["a"]["dims"])
             b = pm.Normal("b", b_loc, sigma=b_scale)
             obs_error = pm.HalfNormal("σ_model_fmc", obs_error)
 
             # observed data
             output = pm.Normal("output", a + b * x, obs_error, shape=x.shape, observed=y_data)
 
+    def _save_input_params(self, idata):
+        idata.attrs["test_paramter"] = json.dumps(self.test_parameter)
+
     @property
     def output_var(self):
         return "output"
 
     def _data_setter(self, x: pd.Series, y: pd.Series = None):
         with self.model:
             pm.set_data({"x": x.values})
@@ -103,29 +113,61 @@
     def generate_and_preprocess_model_data(self, X: pd.DataFrame, y: pd.Series):
         self.X = X
         self.y = y
 
     @property
     def default_model_config(self) -> Dict:
         return {
-            "a": {"loc": 0, "scale": 10},
+            "a": {"loc": 0, "scale": 10, "dims": ("numbers",)},
             "b": {"loc": 0, "scale": 10},
             "obs_error": 2,
         }
 
     @property
     def default_sampler_config(self) -> Dict:
         return {
             "draws": 1_000,
             "tune": 1_000,
             "chains": 3,
             "target_accept": 0.95,
         }
 
 
+def test_save_input_params(fitted_model_instance):
+    assert fitted_model_instance.idata.attrs["test_paramter"] == '"test_paramter"'
+
+
+def test_save_load(fitted_model_instance):
+    temp = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False)
+    fitted_model_instance.save(temp.name)
+    test_builder2 = test_ModelBuilder.load(temp.name)
+    assert fitted_model_instance.idata.groups() == test_builder2.idata.groups()
+    assert fitted_model_instance.id == test_builder2.id
+    x_pred = np.random.uniform(low=0, high=1, size=100)
+    prediction_data = pd.DataFrame({"input": x_pred})
+    pred1 = fitted_model_instance.predict(prediction_data["input"])
+    pred2 = test_builder2.predict(prediction_data["input"])
+    assert pred1.shape == pred2.shape
+    temp.close()
+
+
+def test_convert_dims_to_tuple(fitted_model_instance):
+    model_config = {
+        "a": {
+            "loc": 0,
+            "scale": 10,
+            "dims": [
+                "x",
+            ],
+        },
+    }
+    converted_model_config = fitted_model_instance._convert_dims_to_tuple(model_config)
+    assert converted_model_config["a"]["dims"] == ("x",)
+
+
 def test_initial_build_and_fit(fitted_model_instance, check_idata=True) -> ModelBuilder:
     if check_idata:
         assert fitted_model_instance.idata is not None
         assert "posterior" in fitted_model_instance.idata.groups()
 
 
 def test_save_without_fit_raises_runtime_error():
@@ -158,28 +200,14 @@
     assert model_builder.idata is not None
     assert "posterior" in model_builder.idata.groups()
 
 
 @pytest.mark.skipif(
     sys.platform == "win32", reason="Permissions for temp files not granted on windows CI."
 )
-def test_save_load(fitted_model_instance):
-    temp = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False)
-    fitted_model_instance.save(temp.name)
-    test_builder2 = test_ModelBuilder.load(temp.name)
-    assert fitted_model_instance.idata.groups() == test_builder2.idata.groups()
-
-    x_pred = np.random.uniform(low=0, high=1, size=100)
-    prediction_data = pd.DataFrame({"input": x_pred})
-    pred1 = fitted_model_instance.predict(prediction_data["input"])
-    pred2 = test_builder2.predict(prediction_data["input"])
-    assert pred1.shape == pred2.shape
-    temp.close()
-
-
 def test_predict(fitted_model_instance):
     x_pred = np.random.uniform(low=0, high=1, size=100)
     prediction_data = pd.DataFrame({"input": x_pred})
     pred = fitted_model_instance.predict(prediction_data["input"])
     # Perform elementwise comparison using numpy
     assert type(pred) == np.ndarray
     assert len(pred) > 0
```

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/test_pathfinder.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/test_pivoted_cholesky.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/test_prior_from_trace.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/test_prior_from_trace.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/test_splines.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/tests/utils/test_model_fgraph.py` & `pymc-experimental-0.0.8/pymc_experimental/tests/utils/test_model_fgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     # Shared rng shared variables are not preserved
     m_new["b1"].owner.inputs[0].container is not m_old["b1"].owner.inputs[0].container
 
     with m_old:
         pm.set_data({"x": [100.0, 200.0]}, coords={"test_dim": range(2)})
 
     assert m_new.dim_lengths["test_dim"].eval() == 2
-    np.testing.assert_array_almost_equal(pm.draw(m_new["x"]), [100.0, 200.0])
+    np.testing.assert_array_almost_equal(pm.draw(m_new["x"], random_seed=63), [100.0, 200.0])
 
 
 @pytest.mark.parametrize("inline_views", (False, True))
 def test_deterministics(inline_views):
     """Test handling of deterministics.
 
     We don't want Deterministics in the middle of the FunctionGraph, as they would make rewrites cumbersome
```

### Comparing `pymc-experimental-0.0.7/pymc_experimental/utils/__init__.py` & `pymc-experimental-0.0.8/pymc_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/utils/linear_cg.py` & `pymc-experimental-0.0.8/pymc_experimental/utils/linear_cg.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/utils/model_fgraph.py` & `pymc-experimental-0.0.8/pymc_experimental/utils/model_fgraph.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/utils/pivoted_cholesky.py` & `pymc-experimental-0.0.8/pymc_experimental/utils/pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/utils/prior.py` & `pymc-experimental-0.0.8/pymc_experimental/utils/prior.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/utils/pytensorf.py` & `pymc-experimental-0.0.8/pymc_experimental/utils/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental/utils/spline.py` & `pymc-experimental-0.0.8/pymc_experimental/utils/spline.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/pymc_experimental.egg-info/PKG-INFO` & `pymc-experimental-0.0.8/pymc_experimental.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.7
+Version: 0.0.8
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.7 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.8 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `pymc-experimental-0.0.7/pymc_experimental.egg-info/SOURCES.txt` & `pymc-experimental-0.0.8/pymc_experimental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.7/setup.py` & `pymc-experimental-0.0.8/setup.py`

 * *Files identical despite different names*

