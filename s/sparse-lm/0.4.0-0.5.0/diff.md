# Comparing `tmp/sparse-lm-0.4.0.tar.gz` & `tmp/sparse-lm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse-lm-0.4.0.tar", last modified: Wed Mar  8 19:00:55 2023, max compression
+gzip compressed data, was "sparse-lm-0.5.0.tar", last modified: Wed Jul 12 00:23:31 2023, max compression
```

## Comparing `sparse-lm-0.4.0.tar` & `sparse-lm-0.5.0.tar`

### file list

```diff
@@ -1,71 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.305808 sparse-lm-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.297808 sparse-lm-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.297808 sparse-lm-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.297808 sparse-lm-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.github/workflows/update-precommit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-08 19:00:55.305808 sparse-lm-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.301808 sparse-lm-0.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.301808 sparse-lm-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   230291 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/sparselm.model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/sparselm.model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/sparselm.stepwise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/docs/sparselm.tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 19:00:55.305808 sparse-lm-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.297808 sparse-lm-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.301808 sparse-lm-0.4.0/src/sparse_lm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-08 19:00:55.000000 sparse-lm-0.4.0/src/sparse_lm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-08 19:00:55.000000 sparse-lm-0.4.0/src/sparse_lm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 19:00:55.000000 sparse-lm-0.4.0/src/sparse_lm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-08 19:00:55.000000 sparse-lm-0.4.0/src/sparse_lm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-08 19:00:55.000000 sparse-lm-0.4.0/src/sparse_lm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.301808 sparse-lm-0.4.0/src/sparselm/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.301808 sparse-lm-0.4.0/src/sparselm/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/_utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.301808 sparse-lm-0.4.0/src/sparselm/model/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33463 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model/_adaptive_lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30168 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model/_lasso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.301808 sparse-lm-0.4.0/src/sparselm/model/_miqp/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model/_miqp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model/_miqp/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model/_miqp/_best_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21211 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model/_miqp/_regularized_l0.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model/_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)    33752 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/stepwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/src/sparselm/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:55.305808 sparse-lm-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/tests/test_lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/tests/test_miqp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/tests/test_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/tests/test_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/tests/test_stepwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-03-08 19:00:46.000000 sparse-lm-0.4.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/update-precommit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   235080 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/_static/logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   230291 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/sparselm.model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/sparselm.model_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/sparselm.stepwise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/sparselm.tools.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.444223 sparse-lm-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   153248 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/corr.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/plot_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/plot_chull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/plot_gl_sgl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/plot_sparse_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)   399600 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/structures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.444223 sparse-lm-0.5.0/src/sparse_lm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.444223 sparse-lm-0.5.0/src/sparselm/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.444223 sparse-lm-0.5.0/src/sparselm/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/_utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/src/sparselm/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33463 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_adaptive_lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31119 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_lasso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/src/sparselm/model/_miqp/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_miqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_miqp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_miqp/_best_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_miqp/_regularized_l0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33496 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_miqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_tools.py
```

### Comparing `sparse-lm-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/.github/pull_request_template.md` & `sparse-lm-0.5.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/.github/workflows/build.yml` & `sparse-lm-0.5.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/.github/workflows/docs.yml` & `sparse-lm-0.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/.github/workflows/lint.yml` & `sparse-lm-0.5.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/.github/workflows/test.yml` & `sparse-lm-0.5.0/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -39,13 +39,13 @@
           pip install cython
           pip install .[tests,dev]
 
       - name: Test with pytest
         run: |
           pytest tests --cov=sparselm --cov-report=xml
 
-      - if: ${{ matrix.python_version == 3.9 && github.event_name == 'push' }}
+      - if: ${{ matrix.python_version == 3.10 && github.event_name == 'push' }}
         name: codacy-coverage-reporter
         uses: codacy/codacy-coverage-reporter-action@v1
         with:
             project-token: ${{ secrets.CODACY_PROJECT_TOKEN }}
             coverage-reports: coverage.xml
```

### Comparing `sparse-lm-0.4.0/.github/workflows/update-precommit.yaml` & `sparse-lm-0.5.0/.github/workflows/update-precommit.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - name: Install pre-commit
         run: pip install pre-commit
 
       - name: Run pre-commit autoupdate
         run: pre-commit autoupdate
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@v4.2.3
+        uses: peter-evans/create-pull-request@v5.0.2
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           branch: update/pre-commit-autoupdate
           title: auto-update pre-commit hooks
           commit-message: auto-update pre-commit hooks
           body: Update versions of tools in pre-commit hooks to latest versions.
           labels: dependencies
```

### Comparing `sparse-lm-0.4.0/.gitignore` & `sparse-lm-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/.pre-commit-config.yaml` & `sparse-lm-0.5.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -14,41 +14,41 @@
     - --remove
   - id: end-of-file-fixer
   - id: trailing-whitespace
   - id: check-added-large-files
     args: ['--maxkb=500']
 
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
 
 - repo: https://github.com/asottile/blacken-docs
-  rev: 1.13.0
+  rev: 1.14.0
   hooks:
   - id: blacken-docs
     additional_dependencies: [black==23.1.0]
     exclude: README.md
 
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
   - id: isort
     name: isort (python)
     args:
     - --profile=black
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.8.0
   hooks:
     - id: pyupgrade
       args: [--py38-plus]
 
 - repo: https://github.com/PyCQA/autoflake
-  rev: v2.0.1
+  rev: v2.2.0
   hooks:
     - id: autoflake
       args:
         - --in-place
         - --remove-unused-variables
         - --remove-all-unused-imports
         - --expand-star-imports
```

### Comparing `sparse-lm-0.4.0/LICENSE` & `sparse-lm-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/PKG-INFO` & `sparse-lm-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse-lm
-Version: 0.4.0
+Version: 0.5.0
 Summary: Sparse linear regression models
 Author-email: Luis Barroso-Luque <lbluque@berkeley.edu>
 License: BSD 3-Clause License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,15 +29,15 @@
 [![test](https://github.com/CederGroupHub/sparse-lm/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/CederGroupHub/sparse-lm/actions/workflows/test.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/9b72db506d9c49b2a6c849348de8945e)](https://www.codacy.com/gh/CederGroupHub/sparse-lm/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CederGroupHub/sparse-lm&utm_campaign=Badge_Coverage)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/CederGroupHub/sparse-lm/main.svg)](https://results.pre-commit.ci/latest/github/CederGroupHub/sparse-lm/main)
 [![pypi version](https://img.shields.io/pypi/v/sparse-lm?color=blue)](https://pypi.org/project/sparse-lm)
 
 **sparse-lm**  includes several (structured) sparse linear regression estimators that are absent in the
 `sklearn.linear_model` module. The estimators in **sparse-lm** are designed to fit right into
-[scikit-lean](https://scikit-learn.org/stable/index.html), but the underlying optimization problem is expressed and
+[scikit-learn](https://scikit-learn.org/stable/index.html), but the underlying optimization problem is expressed and
 solved by leveraging [cvxpy](https://www.cvxpy.org/).
 
 ---------------------------------------------------------------------------------------
 
 Available regression models
 ---------------------------
 - Lasso, Group Lasso, Overlap Group Lasso, Sparse Group Lasso & Ridged Group Lasso.
@@ -59,7 +59,9 @@
 alasso = AdaptiveLasso(fit_intercept=False)
 param_grid = {'alpha': np.logsppace(-7, -2)}
 
 cvsearch = GridSearchCV(alasso, param_grid)
 cvsearch.fit(X, y)
 print(cvsearch.best_params_)
 ```
+
+For more details on use and functionality see the [documentation](https://cedergrouphub.github.io/sparse-lm/).
```

### Comparing `sparse-lm-0.4.0/README.md` & `sparse-lm-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![test](https://github.com/CederGroupHub/sparse-lm/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/CederGroupHub/sparse-lm/actions/workflows/test.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/9b72db506d9c49b2a6c849348de8945e)](https://www.codacy.com/gh/CederGroupHub/sparse-lm/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CederGroupHub/sparse-lm&utm_campaign=Badge_Coverage)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/CederGroupHub/sparse-lm/main.svg)](https://results.pre-commit.ci/latest/github/CederGroupHub/sparse-lm/main)
 [![pypi version](https://img.shields.io/pypi/v/sparse-lm?color=blue)](https://pypi.org/project/sparse-lm)
 
 **sparse-lm**  includes several (structured) sparse linear regression estimators that are absent in the
 `sklearn.linear_model` module. The estimators in **sparse-lm** are designed to fit right into
-[scikit-lean](https://scikit-learn.org/stable/index.html), but the underlying optimization problem is expressed and
+[scikit-learn](https://scikit-learn.org/stable/index.html), but the underlying optimization problem is expressed and
 solved by leveraging [cvxpy](https://www.cvxpy.org/).
 
 ---------------------------------------------------------------------------------------
 
 Available regression models
 ---------------------------
 - Lasso, Group Lasso, Overlap Group Lasso, Sparse Group Lasso & Ridged Group Lasso.
@@ -35,7 +35,9 @@
 alasso = AdaptiveLasso(fit_intercept=False)
 param_grid = {'alpha': np.logsppace(-7, -2)}
 
 cvsearch = GridSearchCV(alasso, param_grid)
 cvsearch.fit(X, y)
 print(cvsearch.best_params_)
 ```
+
+For more details on use and functionality see the [documentation](https://cedergrouphub.github.io/sparse-lm/).
```

### Comparing `sparse-lm-0.4.0/docs/_static/logo.png` & `sparse-lm-0.5.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/docs/conf.py` & `sparse-lm-0.5.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,17 +33,15 @@
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinx.ext.autosummary",
     "sphinx.ext.mathjax",
     "m2r2",
-    # "nbsphinx",
-    # "nbsphinx_link",
-    # "sphinxcontrib.autodoc_pydantic",
+    "sphinx_gallery.gen_gallery",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -122,7 +120,14 @@
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3.9", None),
     "scikit-learn": ("https://scikit-learn.org/stable", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "cvxpy": ("https://www.cvxpy.org/en/latest/", None),
 }
+
+# -- Options for sphinx gallery extension  ---------------------------------------
+
+sphinx_gallery_conf = {
+    "examples_dirs": "../examples",  # path to your example scripts
+    "gallery_dirs": "auto_examples",  # path to where to save gallery generated output
+}
```

### Comparing `sparse-lm-0.4.0/docs/contributing.rst` & `sparse-lm-0.5.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/docs/index.rst` & `sparse-lm-0.5.0/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 
 .. toctree::
    :caption: Getting Started
    :hidden:
 
    install
-   examples
+   auto_examples/index
 
 .. toctree::
    :caption: Information
    :hidden:
 
    contributing
    license
-   changelog
    GitHub <https://github.com/CederGroupHub/sparse-lm>
 
 
 .. toctree::
    :caption: Reference
    :maxdepth: -1
    :hidden:
@@ -25,13 +24,17 @@
    genindex
 
 
 .. image:: _static/logo.png
     :width: 700
     :class: only-dark
 
+.. image:: _static/logo-light.png
+   :width: 700
+   :class: only-light
+
 ===============================
 Sparse Linear Regression Models
 ===============================
 
 .. mdinclude:: ../README.md
    :start-line: 4
```

### Comparing `sparse-lm-0.4.0/pyproject.toml` & `sparse-lm-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [project.optional-dependencies]
 dev = ["pre-commit", "black", "isort", "flake8", "pylint", "pydocstyle", "flake8-pyproject"]
 # Gurobipy needed by mixedL0 tests, pandas needed by sklearn convention checks.
 tests = ["pytest >=7.2.0", "pytest-cov >=4.0.0", "coverage", "pandas", "gurobipy", "pyscipopt"]
-docs = ["sphinx>=5.3", "furo", "m2r2"]
+docs = ["sphinx>=5.3", "furo", "m2r2", "sphinx-gallery"]
 optional = ["gurobipy"]
 
 # pyproject.toml
 [tool.setuptools_scm]
 
 # linting tools, etc
 [tool.pytest.ini_options]
```

### Comparing `sparse-lm-0.4.0/src/sparse_lm.egg-info/PKG-INFO` & `sparse-lm-0.5.0/src/sparse_lm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse-lm
-Version: 0.4.0
+Version: 0.5.0
 Summary: Sparse linear regression models
 Author-email: Luis Barroso-Luque <lbluque@berkeley.edu>
 License: BSD 3-Clause License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,15 +29,15 @@
 [![test](https://github.com/CederGroupHub/sparse-lm/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/CederGroupHub/sparse-lm/actions/workflows/test.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/9b72db506d9c49b2a6c849348de8945e)](https://www.codacy.com/gh/CederGroupHub/sparse-lm/dashboard?utm_source=github.com&utm_medium=referral&utm_content=CederGroupHub/sparse-lm&utm_campaign=Badge_Coverage)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/CederGroupHub/sparse-lm/main.svg)](https://results.pre-commit.ci/latest/github/CederGroupHub/sparse-lm/main)
 [![pypi version](https://img.shields.io/pypi/v/sparse-lm?color=blue)](https://pypi.org/project/sparse-lm)
 
 **sparse-lm**  includes several (structured) sparse linear regression estimators that are absent in the
 `sklearn.linear_model` module. The estimators in **sparse-lm** are designed to fit right into
-[scikit-lean](https://scikit-learn.org/stable/index.html), but the underlying optimization problem is expressed and
+[scikit-learn](https://scikit-learn.org/stable/index.html), but the underlying optimization problem is expressed and
 solved by leveraging [cvxpy](https://www.cvxpy.org/).
 
 ---------------------------------------------------------------------------------------
 
 Available regression models
 ---------------------------
 - Lasso, Group Lasso, Overlap Group Lasso, Sparse Group Lasso & Ridged Group Lasso.
@@ -59,7 +59,9 @@
 alasso = AdaptiveLasso(fit_intercept=False)
 param_grid = {'alpha': np.logsppace(-7, -2)}
 
 cvsearch = GridSearchCV(alasso, param_grid)
 cvsearch.fit(X, y)
 print(cvsearch.best_params_)
 ```
+
+For more details on use and functionality see the [documentation](https://cedergrouphub.github.io/sparse-lm/).
```

### Comparing `sparse-lm-0.4.0/src/sparse_lm.egg-info/SOURCES.txt` & `sparse-lm-0.5.0/src/sparse_lm.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,32 +9,40 @@
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/build.yml
 .github/workflows/docs.yml
 .github/workflows/lint.yml
 .github/workflows/test.yml
 .github/workflows/update-precommit.yaml
 docs/api.rst
-docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
-docs/examples.rst
 docs/index.rst
 docs/install.rst
 docs/license.rst
 docs/sparselm.model.rst
 docs/sparselm.model_selection.rst
 docs/sparselm.stepwise.rst
 docs/sparselm.tools.rst
+docs/_static/logo-light.png
 docs/_static/logo.png
+examples/README.rst
+examples/corr.npy
+examples/energy.npy
+examples/plot_adaptive.py
+examples/plot_chull.py
+examples/plot_gl_sgl.py
+examples/plot_sparse_signal.py
+examples/structures.json
 src/sparse_lm.egg-info/PKG-INFO
 src/sparse_lm.egg-info/SOURCES.txt
 src/sparse_lm.egg-info/dependency_links.txt
 src/sparse_lm.egg-info/requires.txt
 src/sparse_lm.egg-info/top_level.txt
 src/sparselm/__init__.py
+src/sparselm/dataset.py
 src/sparselm/model_selection.py
 src/sparselm/stepwise.py
 src/sparselm/tools.py
 src/sparselm/_utils/__init__.py
 src/sparselm/_utils/validation.py
 src/sparselm/model/__init__.py
 src/sparselm/model/_adaptive_lasso.py
@@ -44,13 +52,14 @@
 src/sparselm/model/_miqp/__init__.py
 src/sparselm/model/_miqp/_base.py
 src/sparselm/model/_miqp/_best_subset.py
 src/sparselm/model/_miqp/_regularized_l0.py
 tests/conftest.py
 tests/pytest.ini
 tests/test_common.py
+tests/test_dataset.py
 tests/test_lasso.py
 tests/test_miqp.py
 tests/test_model_selection.py
 tests/test_ols.py
 tests/test_stepwise.py
 tests/test_tools.py
```

### Comparing `sparse-lm-0.4.0/src/sparselm/_utils/validation.py` & `sparse-lm-0.5.0/src/sparselm/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/src/sparselm/model/__init__.py` & `sparse-lm-0.5.0/src/sparselm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/src/sparselm/model/_adaptive_lasso.py` & `sparse-lm-0.5.0/src/sparselm/model/_adaptive_lasso.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/src/sparselm/model/_base.py` & `sparse-lm-0.5.0/src/sparselm/model/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 The classes make use of and follow the scikit-learn API.
 """
 
 from __future__ import annotations
 
 __author__ = "Luis Barroso-Luque, Fengyu Xie"
 
+import warnings
 from abc import ABCMeta, abstractmethod
 from collections.abc import Sequence
 from numbers import Integral
 from types import SimpleNamespace
 from typing import Any, NamedTuple
 
 import cvxpy as cp
@@ -47,31 +48,34 @@
         parameters (SimpleNamespace of cp.Parameter or ArrayLike):
             SimpleNamespace with named cp.Parameter objects or ArrayLike of parameters.
             The namespace should be defined by the Regressor generating it.
         auxiliaries (SimpleNamespace of cp.Variable or cp.Expression):
             SimpleNamespace with auxiliary cp.Variable or cp.Expression objects.
             The namespace should be defined by the Regressor generating it.
         constraints (list of cp.Constaint):
-            List of constraints.
+            List of constraints intrinsic to regression problem.
+        user_constraints (list of cp.Constaint):
+            List of user-defined constraints.
     """
 
     problem: cp.Problem
     objective: cp.Expression
     beta: cp.Variable
     parameters: SimpleNamespace | None
     auxiliaries: SimpleNamespace | None
-    constraints: list[cp.Expression] | None
+    constraints: list[cp.Expression | cp.Constraint] | None
+    user_constraints: list[cp.Expression | cp.Constraint] | None
 
 
 class CVXRegressor(RegressorMixin, LinearModel, metaclass=ABCMeta):
     r"""Abstract base class for Regressors using cvxpy with a sklearn interface.
 
     Note cvxpy can use one of many 3rd party solvers, default is most often
-    CVXOPT or ECOS. For integer and mixed integer problems options include SCIP (open source)
-    and Gurobi, among other commercial solvers.
+    CVXOPT or ECOS. For integer and mixed integer problems options include
+    SCIP (open source) and Gurobi, among other commercial solvers.
 
     The solver can be specified by setting the solver keyword argument.
     And can solver specific settings can be set by passing a dictionary of
     solver_options.
 
     See "Setting solver options" in documentation for details of available options:
     https://www.cvxpy.org/tutorial/advanced/index.html#advanced
@@ -91,22 +95,24 @@
             https://www.cvxpy.org/tutorial/advanced/index.html#solve-method-options
         solver_options (dict):
             dictionary of keyword arguments passed to cvxpy solve.
             See docs linked above for more information.
 
     Attributes:
         coef_ (NDArray):
-            Parameter vector (:math:`\beta` in the cost function formula) of shape (n_features,).
+            Parameter vector (:math:`\beta` in the cost function formula) of shape
+            (n_features,).
         intercept_ (float):
             Independent term in decision function.
         canonicals_ (SimpleNamespace):
             Namespace that contains underlying cvxpy objects used to define
             the optimization problem. The objects included are the following:
                 - objective - the objective function.
-                - beta - variable to be optimized (corresponds to the estimated coef_ attribute).
+                - beta - variable to be optimized (corresponds to the estimated
+                         coef_ attribute).
                 - parameters - hyper-parameters
                 - auxiliaries - auxiliary variables and expressions
                 - constraints - solution constraints
     """
 
     # parameter constraints that do not need any cvxpy Parameter object
     _parameter_constraints: dict[str, list[Any]] = {
@@ -139,16 +145,17 @@
         y: ArrayLike,
         sample_weight: ArrayLike | None = None,
         *args,
         **kwargs,
     ):
         """Fit the linear model coefficients.
 
-        Prepares the  fit data input, generates cvxpy objects to represent the minimization
-        objective, and solves the regression problem using the given solver.
+        Prepares the  fit data input, generates cvxpy objects to represent the
+        minimization objective, and solves the regression problem using the given
+        solver.
 
         Args:
             X (ArrayLike):
                 Training data of shape (n_samples, n_features).
             y (ArrayLike):
                 Target values. Will be cast to X's dtype if necessary
                 of shape (n_samples,) or (n_samples, n_targets)
@@ -163,14 +170,48 @@
         Returns:
             instance of self
         """
         X, y = self._validate_data(
             X, y, accept_sparse=False, y_numeric=True, multi_output=False
         )
 
+        X, y, X_offset, y_offset, X_scale = self._preprocess_data(X, y, sample_weight)
+
+        self._validate_params(X, y)
+
+        # TODO test theses cases
+        if not hasattr(self, "canonicals_"):
+            self.generate_problem(X, y, preprocess_data=False)
+        elif not np.array_equal(self.cached_X_, X) or not np.array_equal(
+            self.cached_y_, y
+        ):
+            if self.canonicals_.user_constraints:
+                warnings.warn(
+                    "User constraints are set on a problem with different data (X, y). "
+                    "These constraints will be ignored.",
+                    UserWarning,
+                )
+            self.generate_problem(X, y, preprocess_data=False)
+        else:
+            self._set_param_values()  # set parameter values
+
+        solver_options = self.solver_options if self.solver_options is not None else {}
+        if not isinstance(solver_options, dict):
+            raise TypeError("solver_options must be a dictionary")
+
+        self.coef_ = self._solve(X, y, solver_options, *args, **kwargs)
+        self._set_intercept(X_offset, y_offset, X_scale)
+
+        # return self for chaining fit and predict calls
+        return self
+
+    def _preprocess_data(
+        self, X: ArrayLike, y: ArrayLike, sample_weight: ArrayLike | None = None
+    ) -> tuple[ArrayLike, ArrayLike, ArrayLike, ArrayLike, ArrayLike]:
+        """Preprocess data for fitting."""
         if sample_weight is not None:
             sample_weight = _check_sample_weight(sample_weight, X, dtype=X.dtype)
             # rescale sample_weight to sum to number of samples
             sample_weight = sample_weight * (X.shape[0] / np.sum(sample_weight))
 
         X, y, X_offset, y_offset, X_scale = _preprocess_data(
             X,
@@ -179,43 +220,15 @@
             fit_intercept=self.fit_intercept,
             sample_weight=sample_weight,
         )
 
         if sample_weight is not None:
             X, y, _ = _rescale_data(X, y, sample_weight)
 
-        self._validate_params(X, y)
-
-        if not hasattr(self, "canonicals_") or self.warm_start is False:
-            self.generate_problem(X, y)
-
-        if self.warm_start is True:
-            # cache training data
-            if not hasattr(self, "cached_X_"):
-                self.cached_X_ = X
-            if not hasattr(self, "cached_y_"):
-                self.cached_y_ = y
-
-            # check if input data has changed and force reset accordingly
-            if not np.array_equal(self.cached_X_, X) or not np.array_equal(
-                self.cached_y_, y
-            ):
-                self.generate_problem(X, y)
-            else:
-                self._set_param_values()  # set parameter values
-
-        solver_options = self.solver_options if self.solver_options is not None else {}
-        if not isinstance(solver_options, dict):
-            raise TypeError("solver_options must be a dictionary")
-
-        self.coef_ = self._solve(X, y, solver_options, *args, **kwargs)
-        self._set_intercept(X_offset, y_offset, X_scale)
-
-        # return self for chaining fit and predict calls
-        return self
+        return X, y, X_offset, y_offset, X_scale
 
     def _validate_params(self, X: ArrayLike, y: ArrayLike) -> None:
         """Validate hyperparameter values.
 
         Implement this in an Regressor for additional parameter value validation.
         """
         if self._cvx_parameter_constraints is None:
@@ -229,14 +242,17 @@
             parameter_constraints,
             self.get_params(deep=False),
             caller_name=self.__class__.__name__,
         )
 
     def _set_param_values(self) -> None:
         """Set the values of cvxpy parameters from param attributes for warm starts."""
+        if self._cvx_parameter_constraints is None:
+            return
+
         for parameter, value in self.get_params(deep=False).items():
             if parameter in self._cvx_parameter_constraints:
                 cvx_parameter = getattr(self.canonicals_.parameters, parameter)
                 # check for parameters that take a scalar or an array
                 if isinstance(value, np.ndarray) or isinstance(value, Sequence):
                     if len(value) == 1:
                         value = value * np.ones_like(cvx_parameter.value)
@@ -270,16 +286,16 @@
 
             # make constraints sklearn constraint objects
             constraints = [
                 make_constraint(constraint)
                 for constraint in cvx_constraints[param_name]
             ]
 
-            # For now we will only set nonneg, nonpos, neg, pos, integer, boolean and/or shape
-            # of the cvxpy Parameter objects.
+            # For now we will only set nonneg, nonpos, neg, pos, integer, boolean and/or
+            # shape of the cvxpy Parameter objects.
             # TODO cxvpy only allows a single one of these to be set (except bool and integer)
             param_kwargs = {}
             for constraint in constraints:
                 if isinstance(constraint, _ArrayLikes):
                     if not hasattr(param_val, "shape"):
                         param_val = np.asarray(param_val)
 
@@ -318,15 +334,15 @@
                 )
 
         return SimpleNamespace(**cvx_parameters)
 
     def _generate_auxiliaries(
         self, X: ArrayLike, y: ArrayLike, beta: cp.Variable, parameters: SimpleNamespace
     ) -> SimpleNamespace | None:
-        """Generate any auxiliary variables or expressions necessary in defining the objective.
+        """Generate any auxiliary variables/expressions necessary to define objective.
 
         Args:
             X (ArrayLike):
                 Covariate/Feature matrix
             y (ArrayLike):
                 Target vector
             beta (cp.Variable):
@@ -372,15 +388,15 @@
     def _generate_constraints(
         self,
         X: ArrayLike,
         y: ArrayLike,
         beta: cp.Variable,
         parameters: SimpleNamespace | None = None,
         auxiliaries: SimpleNamespace | None = None,
-    ) -> list[cp.constraints] | None:
+    ) -> list[cp.constraints]:
         """Generate constraints for optimization problem.
 
         Args:
             X (ArrayLike):
                 Covariate/Feature matrix
             y (ArrayLike):
                 Target vector
@@ -390,45 +406,114 @@
                 SimpleNamespace with cp.Parameter objects
             auxiliaries (SimpleNamespace): optional
                 SimpleNamespace with auxiliary cvxpy objects
 
         Returns:
             list of cvxpy constraints
         """
-        return None
+        return []
 
-    def generate_problem(self, X: ArrayLike, y: ArrayLike) -> None:
+    def generate_problem(
+        self,
+        X: ArrayLike,
+        y: ArrayLike,
+        preprocess_data: bool = True,
+        sample_weight: ArrayLike | None = None,
+    ) -> None:
         """Generate regression problem and auxiliary cvxpy objects.
 
-        This initializes the minimization problem, the objective, coefficient variable (beta), problem parameters,
-        solution constraints, and auxiliary variables/terms.
+        This initializes the minimization problem, the objective, coefficient variable
+        (beta), problem parameters, solution constraints, and auxiliary variables/terms.
 
-        This is (almost always) called in the fit method, and not directly. However, it can be called directly if
-        further control over the problem is needed by accessing the canonicals_ objects. For example to add additional
-        constraints on problem variables.
+        This is (almost always) called in the fit method, and not directly. However, it
+        can be called directly if further control over the problem is needed by
+        accessing the canonicals_ objects. For example to add additional constraints on
+        problem variables.
 
         Args:
             X (ArrayLike):
                 Covariate/Feature matrix
             y (ArrayLike):
                 Target vector
+            preprocess_data (bool):
+                Whether to preprocess the data before generating the problem. If calling
+                generate_problem directly, this should be kept as True to ensure the
+                problem is generated correctly for a subsequent call to fit.
+            sample_weight (ArrayLike):
+                Individual weights for each sample of shape (n_samples,)
+                default=None. Only used if preprocess_data=True to rescale the data
+                accordingly.
         """
+        if preprocess_data is True:
+            X, y, _, _, _ = self._preprocess_data(X, y, sample_weight)
+
+        # X, y are cached to avoid re-generating problem if fit is called again with
+        # same data
+        self.cached_X_ = X
+        self.cached_y_ = y
+
         beta = cp.Variable(X.shape[1])
         parameters = self._generate_params(X, y)
         auxiliaries = self._generate_auxiliaries(X, y, beta, parameters)
         objective = self._generate_objective(X, y, beta, parameters, auxiliaries)
         constraints = self._generate_constraints(X, y, beta, parameters, auxiliaries)
         problem = cp.Problem(cp.Minimize(objective), constraints)
         self.canonicals_ = CVXCanonicals(
             problem=problem,
             objective=objective,
             beta=beta,
             parameters=parameters,
             auxiliaries=auxiliaries,
             constraints=constraints,
+            user_constraints=[],
+        )
+
+    def add_constraints(
+        self, constraints: list[cp.constraint | cp.expressions]
+    ) -> None:
+        """Add a constraint to the problem.
+
+        .. warning::
+            Adding constraints will not work with any sklearn class that relies on
+            cloning the estimator (ie GridSearchCV, etc) . This is because a new cvxpy
+            problem is generated for any cloned estimator.
+
+        Args:
+            constraints (list of cp.constraint or cp.expressions):
+                cvxpy constraint to add to the problem
+        """
+        if not hasattr(self, "canonicals_"):
+            raise RuntimeError(
+                "Problem has not been generated. Please call generate_problem before"
+                " adding constraints."
+            )
+        self.canonicals_.user_constraints.extend(list(constraints))
+        # need to reset problem to update constraints
+        self._reset_problem()
+
+    def _reset_problem(self) -> None:
+        """Reset the cvxpy problem."""
+        if not hasattr(self, "canonicals_"):
+            raise RuntimeError(
+                "Problem has not been generated. Please call generate_problem before"
+                " resetting."
+            )
+
+        problem = cp.Problem(
+            cp.Minimize(self.canonicals_.objective),
+            self.canonicals_.constraints + self.canonicals_.user_constraints,
+        )
+        self.canonicals_ = CVXCanonicals(
+            problem=problem,
+            objective=self.canonicals_.objective,
+            beta=self.canonicals_.beta,
+            parameters=self.canonicals_.parameters,
+            auxiliaries=self.canonicals_.auxiliaries,
+            constraints=self.canonicals_.constraints,
+            user_constraints=self.canonicals_.user_constraints,
         )
 
     def _solve(
         self, X: ArrayLike, y: ArrayLike, solver_options: dict, *args, **kwargs
     ) -> NDArray[float]:
         """Solve the cvxpy problem."""
         self.canonicals_.problem.solve(
@@ -436,17 +521,17 @@
         )
         return self.canonicals_.beta.value
 
 
 class TikhonovMixin:
     """Mixin class to add a Tihhonov/ridge regularization term.
 
-    When using this Mixin, a cvxpy parameter named "eta" should be saved in the parameters
-    SimpleNamespace an attribute tikhonov_w can be added to allow a matrix otherwise simple l2/Ridge
-    is used.
+    When using this Mixin, a cvxpy parameter named "eta" should be saved in the
+    parameters SimpleNamespace an attribute tikhonov_w can be added to allow a matrix
+    otherwise simple l2/Ridge is used.
     """
 
     def _generate_objective(
         self,
         X: ArrayLike,
         y: ArrayLike,
         beta: cp.Variable,
```

### Comparing `sparse-lm-0.4.0/src/sparselm/model/_lasso.py` & `sparse-lm-0.5.0/src/sparselm/model/_lasso.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         beta: cp.Variable,
         parameters: SimpleNamespace,
         auxiliaries: SimpleNamespace | None = None,
     ) -> cp.Expression:
         return parameters.alpha * (parameters.group_weights @ auxiliaries.group_norms)
 
 
-# TODO this implementation is not efficient, reimplement.
+# TODO this implementation is not efficient, reimplement, or simply deprecate.
 class OverlapGroupLasso(GroupLasso):
     r"""Overlap Group Lasso implementation.
 
     Regularized regression objective:
 
     .. math::
 
@@ -396,23 +396,45 @@
 
         group_weights = (
             np.ones(n_groups) if self.group_weights is None else self.group_weights
         )
         parameters.group_weights = group_weights
         return parameters
 
-    def generate_problem(self, X: ArrayLike, y: ArrayLike) -> None:
+    def generate_problem(
+        self,
+        X: ArrayLike,
+        y: ArrayLike,
+        preprocess_data: bool = True,
+        sample_weight: ArrayLike | None = None,
+    ) -> None:
         """Initialize cvxpy problem from the generated objective function.
 
         Args:
             X (ArrayLike):
                 Covariate/Feature matrix
             y (ArrayLike):
                 Target vector
+            preprocess_data (bool):
+                Whether to preprocess the data before generating the problem. If calling
+                generate_problem directly, this should be kept as True to ensure the
+                problem is generated correctly for a subsequent call to fit.
+            sample_weight (ArrayLike):
+                Individual weights for each sample of shape (n_samples,)
+                default=None. Only used if preprocess_data=True to rescale the data
+                accordingly.
         """
+        if preprocess_data is True:
+            X, y, _, _, _ = self._preprocess_data(X, y, sample_weight)
+
+        # X, y are cached to avoid re-generating problem if fit is called again with
+        # same data
+        self.cached_X_ = X
+        self.cached_y_ = y
+
         # need to generate the auxiliaries here since the problem data is "augmented"
         # based on them
         if self.group_list is None:
             group_list = [[i] for i in range(X.shape[1])]
         else:
             group_list = self.group_list
 
@@ -448,14 +470,15 @@
         self.canonicals_ = CVXCanonicals(
             problem=problem,
             objective=objective,
             beta=beta,
             parameters=parameters,
             auxiliaries=auxiliaries,
             constraints=constraints,
+            user_constraints=[],
         )
 
     def _solve(self, X, y, solver_options, *args, **kwargs) -> NDArray[float]:
         """Solve the cvxpy problem."""
         self.canonicals_.problem.solve(
             solver=self.solver, warm_start=self.warm_start, **solver_options
         )
```

### Comparing `sparse-lm-0.4.0/src/sparselm/model/_miqp/_base.py` & `sparse-lm-0.5.0/src/sparselm/model/_miqp/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 from sklearn.utils._param_validation import Interval
 
 from ..._utils.validation import _check_groups
 from .._base import CVXRegressor
 
 
 class MIQPl0(CVXRegressor, metaclass=ABCMeta):
-    """Base class for mixed-integer quadratic programming (MIQP) Regressors.
+    r"""Base class for mixed-integer quadratic programming (MIQP) Regressors.
 
     Generalized l0 formulation that allows grouping coefficients, based on:
 
     https://doi.org/10.1287/opre.2015.1436
 
     Args:
         groups (list or ndarray):
             array-like of integers specifying groups. Length should be the
             same as model, where each integer entry specifies the group
             each parameter corresponds to. If no grouping is required, simply
             pass a list of all different numbers, i.e. using range.
         big_M (float):
             Upper bound on the norm of coefficients associated with each
-            cluster (groups of coefficients) ||Beta_c||_2
+            groups of coefficients :math:`||\beta_c||_2`.
         hierarchy (list):
             A list of lists of integers storing hierarchy relations between
             coefficients.
             Each sublist contains indices of other coefficients
             on which the coefficient associated with each element of
             the list depends. i.e. hierarchy = [[1, 2], [0], []] mean that
             coefficient 0 depends on 1, and 2; 1 depends on 0, and 2 has no
```

### Comparing `sparse-lm-0.4.0/src/sparselm/model/_miqp/_best_subset.py` & `sparse-lm-0.5.0/src/sparselm/model/_miqp/_best_subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             each parameter corresponds to. If no grouping is required,
             simply pass a list of all different numbers, i.e. using range.
         sparse_bound (int):
             Upper bound on sparsity. The upper bound on total number of
             nonzero coefficients.
         big_M (float):
             Upper bound on the norm of coefficients associated with each
-            cluster (groups of coefficients) ||Beta_c||_2
+            groups of coefficients :math:`||\beta_c||_2`.
         hierarchy (list):
             A list of lists of integers storing hierarchy relations between
             coefficients.
             Each sublist contains indices of other coefficients
             on which the coefficient associated with each element of
             the list depends. i.e. hierarchy = [[1, 2], [0], []] mean that
             coefficient 0 depends on 1, and 2; 1 depends on 0, and 2 has no
@@ -148,15 +148,15 @@
         sparse_bound (int):
             Upper bound on sparsity. The upper bound on total number of
             nonzero coefficients.
         eta (float):
             L2 regularization hyper-parameter.
         big_M (float):
             Upper bound on the norm of coefficients associated with each
-            cluster (groups of coefficients) ||Beta_c||_2
+            groups of coefficients :math:`||\beta_c||_2`.
         hierarchy (list):
             A list of lists of integers storing hierarchy relations between
             coefficients.
             Each sublist contains indices of other coefficients
             on which the coefficient associated with each element of
             the list depends. i.e. hierarchy = [[1, 2], [0], []] mean that
             coefficient 0 depends on 1, and 2; 1 depends on 0, and 2 has no
```

### Comparing `sparse-lm-0.4.0/src/sparselm/model/_miqp/_regularized_l0.py` & `sparse-lm-0.5.0/src/sparselm/model/_miqp/_regularized_l0.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             each parameter corresponds to. If no grouping is needed pass a list
             of all distinct numbers (ie range(len(coefs)) to create singleton groups
             for each parameter.
         alpha (float):
             L0 pseudo-norm regularization hyper-parameter.
         big_M (float):
             Upper bound on the norm of coefficients associated with each
-            cluster (groups of coefficients) ||Beta_c||_2
+            groups of coefficients :math:`||\beta_c||_2`.
         hierarchy (list):
             A list of lists of integers storing hierarchy relations between
             groups.
             Each sublist contains indices of other groups
             on which the group associated with each element of
             the list depends. i.e. hierarchy = [[1, 2], [0], []] mean that
             group 0 depends on 1, and 2; 1 depends on 0, and 2 has no
@@ -192,15 +192,15 @@
                 for each parameter.
             alpha (float):
                 L0 pseudo-norm regularization hyper-parameter.
             eta (float):
                 standard norm regularization hyper-parameter (usually l1 or l2).
             big_M (float):
                 Upper bound on the norm of coefficients associated with each
-                cluster (groups of coefficients) ||Beta_c||_2
+
             hierarchy (list):
                 A list of lists of integers storing hierarchy relations between
                 coefficients.
                 Each sublist contains indices of other coefficients
                 on which the coefficient associated with each element of
                 the list depends. i.e. hierarchy = [[1, 2], [0], []] mean that
                 coefficient 0 depends on 1, and 2; 1 depends on 0, and 2 has no
@@ -284,15 +284,15 @@
             for each parameter.
         alpha (float):
             L0 pseudo-norm regularization hyper-parameter.
         eta (float):
             L1 regularization hyper-parameter.
         big_M (float):
             Upper bound on the norm of coefficients associated with each
-            cluster (groups of coefficients) ||Beta_c||_2
+            groups of coefficients :math:`||\beta_c||_2`.
         hierarchy (list):
             A list of lists of integers storing hierarchy relations between
             coefficients.
             Each sublist contains indices of other coefficients
             on which the coefficient associated with each element of
             the list depends. i.e. hierarchy = [[1, 2], [0], []] mean that
             coefficient 0 depends on 1, and 2; 1 depends on 0, and 2 has no
@@ -437,15 +437,15 @@
             for each parameter.
         alpha (float):
             L0 pseudo-norm regularization hyper-parameter.
         eta (float):
             L2 regularization hyper-parameter.
         big_M (float):
             Upper bound on the norm of coefficients associated with each
-            cluster (groups of coefficients) ||Beta_c||_2
+            groups of coefficients :math:`||\beta_c||_2`.
         hierarchy (list):
             A list of lists of integers storing hierarchy relations between
             coefficients.
             Each sublist contains indices of other coefficients
             on which the coefficient associated with each element of
             the list depends. i.e. hierarchy = [[1, 2], [0], []] mean that
             coefficient 0 depends on 1, and 2; 1 depends on 0, and 2 has no
```

### Comparing `sparse-lm-0.4.0/src/sparselm/model/_ols.py` & `sparse-lm-0.5.0/src/sparselm/model/_ols.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/src/sparselm/model_selection.py` & `sparse-lm-0.5.0/src/sparselm/model_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class GridSearchCV(_GridSearchCV):
     """Exhaustive search over specified parameter values for an estimator.
 
     Same as GridSearchCV but allows to use one standard error rule on all
     non-negative numerical hyper-parameters, in order to get a
-    robust sparce estimation. Same documentation as scikit-learn's
+    robust sparse estimation. Same documentation as scikit-learn's
     GridSearchCV.
 
     An additional class variable opt_selection named opt_selection
     is added to allow switching hyper params selection mode. Currently,
     supports "max_score" (default), which is to maximize the score;
     also supports "one_std_score", which is to apply one-standard-error
     rule to the score.
@@ -64,17 +64,15 @@
             - a list or tuple of unique strings;
             - a callable returning a dictionary where the keys are the
             metric names and the values are the metric scores;
             - a dictionary with metric names as keys and callables a
             values.
             See :ref:`multimetric_grid_search` for an example.
             In sparse-lm, using "neg_root_mean_squared_error" is default
-            because in cluster expansion it is more conventional to
-            analyze and present errors in the root-mean-square error format
-            compared to the r2_score.
+            in contrast to r2_score used in scikit-learn.
         n_jobs (int, default=None):
             Number of jobs to run in parallel.
             ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
             context.
             ``-1`` means using all processors. See
             :term:`Glossary <n_jobs>` for more details.
         refit (bool, str, or callable, default=True)
@@ -491,17 +489,15 @@
                 - a list or tuple of unique strings;
                 - a callable returning a dictionary where the keys are the
                 metric names and the values are the metric scores;
                 - a dictionary with metric names as keys and callables a
                 values.
                 See :ref:`multimetric_grid_search` for an example.
                 In sparse-lm, using "neg_root_mean_squared_error" is default
-                because in cluster expansion it is more conventional to
-                analyze and present errors in the root-mean-square error format
-                compared to the r2_score.
+                in contrast to r2_score used in scikit-learn.
             n_jobs (int, default=None):
                 Number of jobs to run in parallel.
                 ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
                 context.
                 ``-1`` means using all processors. See
                 :term:`Glossary <n_jobs>` for more details.
             refit (bool, str, or callable, default=True):
```

### Comparing `sparse-lm-0.4.0/src/sparselm/stepwise.py` & `sparse-lm-0.5.0/src/sparselm/stepwise.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/src/sparselm/tools.py` & `sparse-lm-0.5.0/src/sparselm/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,20 @@
 def constrain_coefficients(
     indices: ArrayLike,
     high: float | ArrayLike = None,
     low: float | ArrayLike = None,
 ):
     """Constrain a fit method to keep coefficients within a specified range.
 
-    Decorator to enforce that a fit method fitting a cluster expansion that
-    contains an EwaldTerm to constrain the dielectric constant to be positive
-    and below the supplied value.
-
     Use this as a standard decorator with parameters:
     - At runtime:
-    coefs = constrain_coefficients(indices, high, low)(fit_method)(X, y)
+        coefs = constrain_coefficients(indices, high, low)(fit_method)(X, y)
     - In fit_method definitions:
-      @constrain_coefficients(indices, high, low)
-      def your_fit_method(X, y):
+        @constrain_coefficients(indices, high, low)
+        def your_fit_method(X, y):
 
     Args:
         indices (array or list):
             indices of coefficients to constrain
         high (float or array):
             upper bound for indices,
         low (float or array):
@@ -56,15 +52,15 @@
         low = -np.inf * np.ones(len(indices))
 
     def decorate_fit_method(fit_method):
         """Decorate a fit method to constrain "dielectric constant".
 
         Args:
             fit_method (callable):
-                the fit_method you will use to fit your cluster expansion.
+                the fit_method you will use to fit your regression model.
                 Must take the feature matrix X and target vector y as first
                 arguments. (i.e. fit_method(X, y, *args, **kwargs)
         """
 
         @wraps(fit_method)
         def wrapped(X, y, *args, **kwargs):
             coefs = fit_method(X, y, *args, **kwargs)
```

### Comparing `sparse-lm-0.4.0/tests/conftest.py` & `sparse-lm-0.5.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,27 +68,23 @@
         beta[idx] = eci
     y = X @ beta + rng.normal(size=N_SAMPLES) * 2e-3  # fake energies
     return X, y, beta
 
 
 @pytest.fixture(scope="package")
 def sparse_coded_signal(rng):
-    n_samples, n_features, n_nonzero = 10, 30, 5
+    n_components, n_features, n_nonzero = 24, 12, 6
     y, X, beta = make_sparse_coded_signal(
-        n_samples=n_samples,
-        n_components=n_features,
-        n_features=n_samples,
+        n_samples=1,
+        n_components=n_components,
+        n_features=n_features,
         n_nonzero_coefs=n_nonzero,
         random_state=rng.integers(0, 2**32 - 1),
-        data_transposed=True,
     )
-    # Make X not of norm 1 for testing
-    X *= 10
-    y *= 10
-    return X, y[:, 0], beta[:, 0]
+    return X, y, beta
 
 
 @pytest.fixture(params=[4, 6], scope="package")
 def random_model_with_groups(random_model, rng, request):
     """Add a correct set of groups to model."""
     X, y, beta = random_model
     n_groups = request.param
```

### Comparing `sparse-lm-0.4.0/tests/test_lasso.py` & `sparse-lm-0.5.0/tests/test_lasso.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/tests/test_miqp.py` & `sparse-lm-0.5.0/tests/test_miqp.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,40 +28,42 @@
             assert all(
                 (abs(coef[groups == parent]) >= THRESHOLD).all() for parent in parents
             )
 
 
 def test_perfect_signal_recovery(sparse_coded_signal):
     X, y, beta = sparse_coded_signal
+    X = X.T
+
     (idx,) = beta.nonzero()
 
     estimator = BestSubsetSelection(sparse_bound=np.count_nonzero(beta))
     estimator.fit(X, y)
 
     npt.assert_array_equal(idx, np.flatnonzero(estimator.coef_))
     npt.assert_array_almost_equal(beta, estimator.coef_)
 
     r_estimator = RidgedBestSubsetSelection(sparse_bound=np.count_nonzero(beta))
 
     # very low regularization should be the same
-    r_estimator.eta = 1e-10
+    r_estimator.eta = 1e-16
     r_estimator.fit(X, y)
     npt.assert_array_almost_equal(beta, r_estimator.coef_)
+    npt.assert_array_equal(idx, np.flatnonzero(r_estimator.coef_))
     assert all(i in np.flatnonzero(r_estimator.coef_) for i in idx)
 
     # a bit higher regularization, check shrinkage
-    coef = estimator.coef_.copy()
+    coef = r_estimator.coef_.copy()
     r_estimator.eta = 1e-4
     r_estimator.fit(X, y)
-    npt.assert_array_almost_equal(beta, r_estimator.coef_, decimal=2)
-    assert all(i in np.flatnonzero(r_estimator.coef_) for i in idx)
+    npt.assert_array_almost_equal(beta, r_estimator.coef_, decimal=1)
     assert np.linalg.norm(coef) > np.linalg.norm(r_estimator.coef_)
 
     # very sensitive to the value of alpha for exact results
-    estimator = RegularizedL0(alpha=0.01)
+    estimator = RegularizedL0(alpha=0.0008)
     estimator.fit(X, y)
 
     npt.assert_array_equal(idx, np.flatnonzero(estimator.coef_))
     npt.assert_array_almost_equal(beta, estimator.coef_, decimal=2)
 
 
 @pytest.mark.parametrize("estimator_cls", MIQP_estimators)
```

### Comparing `sparse-lm-0.4.0/tests/test_model_selection.py` & `sparse-lm-0.5.0/tests/test_model_selection.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/tests/test_ols.py` & `sparse-lm-0.5.0/tests/test_ols.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/tests/test_stepwise.py` & `sparse-lm-0.5.0/tests/test_stepwise.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.4.0/tests/test_tools.py` & `sparse-lm-0.5.0/tests/test_tools.py`

 * *Files identical despite different names*

