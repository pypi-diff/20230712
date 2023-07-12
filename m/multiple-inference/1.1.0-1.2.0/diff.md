# Comparing `tmp/multiple-inference-1.1.0.tar.gz` & `tmp/multiple-inference-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\DBSpe\repos\conditional-inference\dist\tmpgcsl92fj\multiple-inference-1.1.0.tar", last modified: Wed Jul 13 20:17:42 2022, max compression
+gzip compressed data, was "multiple-inference-1.2.0.tar", last modified: Wed Jul 12 00:01:12 2023, max compression
```

## Comparing `multiple-inference-1.1.0.tar` & `multiple-inference-1.2.0.tar`

### file list

```diff
@@ -1,108 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:41.929943 multiple-inference-1.1.0/
--rw-rw-rw-   0        0        0     1631 2021-10-21 13:21:43.000000 multiple-inference-1.1.0/.gitignore
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.204965 multiple-inference-1.1.0/.gitlab/
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.270852 multiple-inference-1.1.0/.gitlab/issue_templates/
--rw-rw-rw-   0        0        0      655 2022-05-14 12:14:18.000000 multiple-inference-1.1.0/.gitlab/issue_templates/bug_template.md
--rw-rw-rw-   0        0        0      595 2022-05-14 12:15:51.000000 multiple-inference-1.1.0/.gitlab/issue_templates/feature_request.md
--rw-rw-rw-   0        0        0     2366 2022-07-09 04:34:11.000000 multiple-inference-1.1.0/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      473 2022-01-23 02:36:04.000000 multiple-inference-1.1.0/.gitpod.yml
--rw-rw-rw-   0        0        0      209 2022-07-09 04:29:34.000000 multiple-inference-1.1.0/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1074 2021-08-21 12:10:24.000000 multiple-inference-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1416 2022-07-09 03:04:12.000000 multiple-inference-1.1.0/Makefile
--rw-rw-rw-   0        0        0     1869 2022-07-13 20:17:41.930967 multiple-inference-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2022-07-08 20:28:49.000000 multiple-inference-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.299532 multiple-inference-1.1.0/docs/
--rw-rw-rw-   0        0        0      598 2021-08-21 12:10:25.000000 multiple-inference-1.1.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.299532 multiple-inference-1.1.0/docs/_static/
--rw-rw-rw-   0        0        0     9862 2021-10-22 13:16:42.000000 multiple-inference-1.1.0/docs/_static/icon.png
--rw-rw-rw-   0        0        0     1891 2022-07-13 18:41:19.000000 multiple-inference-1.1.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     6268 2022-07-08 20:11:42.000000 multiple-inference-1.1.0/docs/conf.py
--rw-rw-rw-   0        0        0     2581 2022-07-13 18:43:15.000000 multiple-inference-1.1.0/docs/contribute.rst
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.332843 multiple-inference-1.1.0/docs/examples/
--rw-rw-rw-   0        0        0    26207 2022-07-13 19:37:35.000000 multiple-inference-1.1.0/docs/examples/bayes_primer.ipynb
--rw-rw-rw-   0        0        0      533 2022-05-11 18:30:15.000000 multiple-inference-1.1.0/docs/examples/data.csv
--rw-rw-rw-   0        0        0      156 2022-07-09 01:47:06.000000 multiple-inference-1.1.0/docs/examples/index.rst
--rw-rw-rw-   0        0        0    25887 2022-07-13 19:20:34.000000 multiple-inference-1.1.0/docs/examples/multiple_inference.ipynb
--rw-rw-rw-   0        0        0     7172 2022-07-13 19:16:33.000000 multiple-inference-1.1.0/docs/examples/rank_conditions.ipynb
--rw-rw-rw-   0        0        0     4194 2022-07-13 19:11:15.000000 multiple-inference-1.1.0/docs/examples/stats.ipynb
--rw-rw-rw-   0        0        0     4608 2022-07-13 19:44:53.000000 multiple-inference-1.1.0/docs/index.rst
--rwxrwxrwx   0        0        0      787 2021-08-21 12:10:25.000000 multiple-inference-1.1.0/docs/make.bat
--rw-rw-rw-   0        0        0      112 2021-08-21 13:27:55.000000 multiple-inference-1.1.0/environment.yml
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.332843 multiple-inference-1.1.0/paper/
--rw-rw-rw-   0        0        0    14525 2022-07-13 18:57:08.000000 multiple-inference-1.1.0/paper/paper.bib
--rw-rw-rw-   0        0        0    11932 2022-07-13 19:05:11.000000 multiple-inference-1.1.0/paper/paper.md
--rw-rw-rw-   0        0        0       49 2021-08-21 12:10:24.000000 multiple-inference-1.1.0/postBuild
--rw-rw-rw-   0        0        0      108 2021-08-21 12:10:24.000000 multiple-inference-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      178 2022-07-08 20:11:11.000000 multiple-inference-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       12 2021-08-21 12:10:24.000000 multiple-inference-1.1.0/runtime.txt
--rw-rw-rw-   0        0        0     1349 2022-07-13 20:17:42.089941 multiple-inference-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2021-08-21 12:10:25.000000 multiple-inference-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.366196 multiple-inference-1.1.0/simulations/
--rw-rw-rw-   0        0        0     2554 2021-08-22 02:56:43.000000 multiple-inference-1.1.0/simulations/README.md
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.382866 multiple-inference-1.1.0/simulations/bayes-stylized/
--rw-rw-rw-   0        0        0  2776084 2021-08-22 19:23:10.000000 multiple-inference-1.1.0/simulations/bayes-stylized/analyze.ipynb
--rw-rw-rw-   0        0        0     3366 2021-08-22 16:38:24.000000 multiple-inference-1.1.0/simulations/bayes-stylized/simulation.py
--rw-rw-rw-   0        0        0       58 2021-08-22 15:08:32.000000 multiple-inference-1.1.0/simulations/bayes-stylized/variables.py
--rw-rw-rw-   0        0        0     1074 2021-08-22 14:08:44.000000 multiple-inference-1.1.0/simulations/cluster_setup.py
--rw-rw-rw-   0        0        0      166 2021-08-21 22:05:48.000000 multiple-inference-1.1.0/simulations/cluster_setup.sh
--rw-rw-rw-   0        0        0     1180 2022-01-10 20:13:12.000000 multiple-inference-1.1.0/simulations/cluster_teardown.py
--rw-rw-rw-   0        0        0      164 2021-08-21 22:05:52.000000 multiple-inference-1.1.0/simulations/cluster_teardown.sh
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.416186 multiple-inference-1.1.0/simulations/losers-empirical/
--rw-rw-rw-   0        0        0   943822 2021-11-27 12:19:30.000000 multiple-inference-1.1.0/simulations/losers-empirical/analyze.ipynb
--rw-rw-rw-   0        0        0     6203 2021-10-21 13:48:13.000000 multiple-inference-1.1.0/simulations/losers-empirical/movers.csv
--rw-rw-rw-   0        0        0     6593 2021-10-21 13:49:05.000000 multiple-inference-1.1.0/simulations/losers-empirical/oa.csv
--rw-rw-rw-   0        0        0     1882 2021-12-10 13:57:21.000000 multiple-inference-1.1.0/simulations/losers-empirical/simulation.py
--rw-rw-rw-   0        0        0      273 2021-12-10 13:30:02.000000 multiple-inference-1.1.0/simulations/losers-empirical/variables.py
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.449536 multiple-inference-1.1.0/simulations/losers-presentation/
--rw-rw-rw-   0        0        0   869558 2022-02-16 23:08:20.000000 multiple-inference-1.1.0/simulations/losers-presentation/analysis.ipynb
--rw-rw-rw-   0        0        0     2526 2021-12-10 17:13:01.000000 multiple-inference-1.1.0/simulations/losers-presentation/simulation.py
--rw-rw-rw-   0        0        0      284 2021-12-10 17:12:39.000000 multiple-inference-1.1.0/simulations/losers-presentation/variables.py
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.532852 multiple-inference-1.1.0/simulations/losers-stylized/
--rw-rw-rw-   0        0        0  5026506 2021-08-22 16:29:24.000000 multiple-inference-1.1.0/simulations/losers-stylized/analyze.ipynb
--rw-rw-rw-   0        0        0     3221 2021-08-22 14:13:18.000000 multiple-inference-1.1.0/simulations/losers-stylized/simulation.py
--rw-rw-rw-   0        0        0       58 2021-08-22 13:57:33.000000 multiple-inference-1.1.0/simulations/losers-stylized/variables.py
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.582817 multiple-inference-1.1.0/simulations/ranking-stylized/
--rw-rw-rw-   0        0        0   107668 2022-01-10 23:10:47.000000 multiple-inference-1.1.0/simulations/ranking-stylized/analyze.ipynb
--rw-rw-rw-   0        0        0     1776 2022-01-10 20:47:46.000000 multiple-inference-1.1.0/simulations/ranking-stylized/simulation.py
--rw-rw-rw-   0        0        0       58 2022-01-10 20:14:32.000000 multiple-inference-1.1.0/simulations/ranking-stylized/variables.py
--rw-rw-rw-   0        0        0      336 2021-08-21 22:05:55.000000 multiple-inference-1.1.0/simulations/simulation.sh
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.599464 multiple-inference-1.1.0/simulations/winners-stylized/
--rw-rw-rw-   0        0        0   664696 2021-08-22 01:11:30.000000 multiple-inference-1.1.0/simulations/winners-stylized/analyze.ipynb
--rw-rw-rw-   0        0        0     2931 2021-08-22 14:14:34.000000 multiple-inference-1.1.0/simulations/winners-stylized/simulation.py
--rw-rw-rw-   0        0        0       58 2021-08-22 14:12:30.000000 multiple-inference-1.1.0/simulations/winners-stylized/variables.py
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.221096 multiple-inference-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.823917 multiple-inference-1.1.0/src/multiple_inference/
--rw-rw-rw-   0        0        0       22 2022-07-09 03:03:41.000000 multiple-inference-1.1.0/src/multiple_inference/__init__.py
--rw-rw-rw-   0        0        0    16762 2022-07-13 19:13:20.000000 multiple-inference-1.1.0/src/multiple_inference/base.py
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:41.073021 multiple-inference-1.1.0/src/multiple_inference/bayes/
--rw-rw-rw-   0        0        0      102 2022-05-10 21:56:38.000000 multiple-inference-1.1.0/src/multiple_inference/bayes/__init__.py
--rw-rw-rw-   0        0        0    13307 2022-07-13 19:14:44.000000 multiple-inference-1.1.0/src/multiple_inference/bayes/base.py
--rw-rw-rw-   0        0        0     2288 2022-07-13 19:14:56.000000 multiple-inference-1.1.0/src/multiple_inference/bayes/improper.py
--rw-rw-rw-   0        0        0     8222 2022-07-13 19:14:52.000000 multiple-inference-1.1.0/src/multiple_inference/bayes/nonparametric.py
--rw-rw-rw-   0        0        0    27679 2022-07-13 19:14:49.000000 multiple-inference-1.1.0/src/multiple_inference/bayes/normal.py
--rw-rw-rw-   0        0        0    31869 2022-07-13 19:13:11.000000 multiple-inference-1.1.0/src/multiple_inference/confidence_set.py
--rw-rw-rw-   0        0        0    11454 2022-07-13 19:13:05.000000 multiple-inference-1.1.0/src/multiple_inference/rank_condition.py
--rw-rw-rw-   0        0        0     4436 2022-07-13 19:12:58.000000 multiple-inference-1.1.0/src/multiple_inference/significance_condition.py
--rw-rw-rw-   0        0        0    24437 2022-07-13 20:12:05.000000 multiple-inference-1.1.0/src/multiple_inference/stats.py
--rw-rw-rw-   0        0        0     4936 2022-05-14 01:42:50.000000 multiple-inference-1.1.0/src/multiple_inference/utils.py
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:40.944029 multiple-inference-1.1.0/src/multiple_inference.egg-info/
--rw-rw-rw-   0        0        0     1869 2022-07-13 20:17:40.000000 multiple-inference-1.1.0/src/multiple_inference.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2630 2022-07-13 20:17:40.000000 multiple-inference-1.1.0/src/multiple_inference.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-13 20:17:40.000000 multiple-inference-1.1.0/src/multiple_inference.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2022-07-13 20:17:40.000000 multiple-inference-1.1.0/src/multiple_inference.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-07-13 20:17:40.000000 multiple-inference-1.1.0/src/multiple_inference.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:41.547334 multiple-inference-1.1.0/tests/
--rw-rw-rw-   0        0        0      344 2021-08-22 23:56:45.000000 multiple-inference-1.1.0/tests/README.md
--rw-rw-rw-   0        0        0     5375 2022-05-02 16:23:53.000000 multiple-inference-1.1.0/tests/test_base.py
-drwxrwxrwx   0        0        0        0 2022-07-13 20:17:41.927951 multiple-inference-1.1.0/tests/test_bayes/
--rw-rw-rw-   0        0        0        0 2022-05-12 19:33:20.000000 multiple-inference-1.1.0/tests/test_bayes/__init__.py
--rw-rw-rw-   0        0        0      993 2022-05-13 11:57:35.000000 multiple-inference-1.1.0/tests/test_bayes/test_improper.py
--rw-rw-rw-   0        0        0     2470 2022-05-13 14:51:45.000000 multiple-inference-1.1.0/tests/test_bayes/test_nonparametric.py
--rw-rw-rw-   0        0        0     5415 2022-06-16 14:51:16.000000 multiple-inference-1.1.0/tests/test_bayes/test_normal.py
--rw-rw-rw-   0        0        0      450 2022-05-13 11:57:35.000000 multiple-inference-1.1.0/tests/test_bayes/utils.py
--rw-rw-rw-   0        0        0     7097 2022-07-09 03:04:18.000000 multiple-inference-1.1.0/tests/test_confidence_set.py
--rw-rw-rw-   0        0        0     1883 2022-05-12 18:26:25.000000 multiple-inference-1.1.0/tests/test_rank_condition.py
--rw-rw-rw-   0        0        0      787 2022-05-12 18:26:25.000000 multiple-inference-1.1.0/tests/test_significance_condition.py
--rw-rw-rw-   0        0        0     5874 2022-05-12 18:28:48.000000 multiple-inference-1.1.0/tests/test_stats.py
--rw-rw-rw-   0        0        0     1444 2022-05-12 18:57:48.000000 multiple-inference-1.1.0/tests/test_utils.py
--rw-rw-rw-   0        0        0      486 2022-07-13 19:25:03.000000 multiple-inference-1.1.0/tox.ini
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-12 00:01:12.977305 multiple-inference-1.2.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1056 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1843 2023-07-12 00:01:12.978280 multiple-inference-1.2.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1363 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      103 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1286 2023-07-12 00:01:12.981898 multiple-inference-1.2.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       68 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-12 00:01:12.768479 multiple-inference-1.2.0/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-12 00:01:12.864694 multiple-inference-1.2.0/src/multiple_inference/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       22 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/src/multiple_inference/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16067 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/src/multiple_inference/base.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-12 00:01:12.933584 multiple-inference-1.2.0/src/multiple_inference/bayes/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       99 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/src/multiple_inference/bayes/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24475 2023-07-11 22:53:28.000000 multiple-inference-1.2.0/src/multiple_inference/bayes/base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2224 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/src/multiple_inference/bayes/improper.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8040 2023-07-11 23:46:51.000000 multiple-inference-1.2.0/src/multiple_inference/bayes/nonparametric.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26941 2023-07-11 22:25:54.000000 multiple-inference-1.2.0/src/multiple_inference/bayes/normal.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    38934 2023-07-11 23:45:32.000000 multiple-inference-1.2.0/src/multiple_inference/confidence_set.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11454 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/src/multiple_inference/rank_condition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4311 2023-07-11 22:25:54.000000 multiple-inference-1.2.0/src/multiple_inference/significance_condition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25896 2023-07-11 22:25:54.000000 multiple-inference-1.2.0/src/multiple_inference/stats.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4804 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/src/multiple_inference/utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-12 00:01:12.905511 multiple-inference-1.2.0/src/multiple_inference.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1843 2023-07-12 00:01:12.000000 multiple-inference-1.2.0/src/multiple_inference.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      899 2023-07-12 00:01:12.000000 multiple-inference-1.2.0/src/multiple_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-12 00:01:12.000000 multiple-inference-1.2.0/src/multiple_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      121 2023-07-12 00:01:12.000000 multiple-inference-1.2.0/src/multiple_inference.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       19 2023-07-12 00:01:12.000000 multiple-inference-1.2.0/src/multiple_inference.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-12 00:01:12.964696 multiple-inference-1.2.0/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5229 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/tests/test_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8917 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/tests/test_confidence_set.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1823 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/tests/test_rank_condition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      761 2023-06-01 02:12:46.000000 multiple-inference-1.2.0/tests/test_significance_condition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6143 2023-07-11 22:25:54.000000 multiple-inference-1.2.0/tests/test_stats.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1399 2023-07-11 22:25:54.000000 multiple-inference-1.2.0/tests/test_utils.py
```

### Comparing `multiple-inference-1.1.0/PKG-INFO` & `multiple-inference-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1
-Name: multiple-inference
-Version: 1.1.0
-Summary: A statistics package for comparing multiple parameters.
-Home-page: https://dsbowen.gitlab.io/conditional-inference
-Author: Dillon Bowen
-Author-email: dsbowen@wharton.upenn.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Multiple Inference
-
-[![Documentation Status](https://readthedocs.org/projects/dsbowen-conditional-inference/badge/?version=latest)](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest)
-[![status](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888/status.svg)](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888)
-[![pipeline status](https://gitlab.com/dsbowen/conditional-inference/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
-[![coverage report](https://gitlab.com/dsbowen/conditional-inference/badges/master/coverage.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
-[![PyPI version](https://badge.fury.io/py/conditional-inference.svg)](https://badge.fury.io/py/conditional-inference)
-[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/conditional-inference/-/blob/master/LICENSE)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fconditional-inference/HEAD?urlpath=lab/tree/examples)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-A statistics package for comparing multiple parameters. Read the docs [here](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest).
+Metadata-Version: 2.1
+Name: multiple-inference
+Version: 1.2.0
+Summary: A statistics package for comparing multiple parameters.
+Home-page: https://dsbowen.gitlab.io/conditional-inference
+Author: Dillon Bowen
+Author-email: dsbowen@wharton.upenn.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Multiple Inference
+
+[![Documentation Status](https://readthedocs.org/projects/dsbowen-conditional-inference/badge/?version=latest)](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest)
+[![status](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888/status.svg)](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888)
+[![pipeline status](https://gitlab.com/dsbowen/conditional-inference/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
+[![coverage report](https://gitlab.com/dsbowen/conditional-inference/badges/master/coverage.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
+[![PyPI version](https://badge.fury.io/py/conditional-inference.svg)](https://badge.fury.io/py/conditional-inference)
+[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/conditional-inference/-/blob/master/LICENSE)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fconditional-inference/HEAD?urlpath=lab/tree/examples)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A statistics package for comparing multiple parameters. Read the docs [here](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest).
```

### Comparing `multiple-inference-1.1.0/README.md` & `multiple-inference-1.2.0/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Multiple Inference
-
-[![Documentation Status](https://readthedocs.org/projects/dsbowen-conditional-inference/badge/?version=latest)](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest)
-[![status](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888/status.svg)](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888)
-[![pipeline status](https://gitlab.com/dsbowen/conditional-inference/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
-[![coverage report](https://gitlab.com/dsbowen/conditional-inference/badges/master/coverage.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
-[![PyPI version](https://badge.fury.io/py/conditional-inference.svg)](https://badge.fury.io/py/conditional-inference)
-[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/conditional-inference/-/blob/master/LICENSE)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fconditional-inference/HEAD?urlpath=lab/tree/examples)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
+# Multiple Inference
+
+[![Documentation Status](https://readthedocs.org/projects/dsbowen-conditional-inference/badge/?version=latest)](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest)
+[![status](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888/status.svg)](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888)
+[![pipeline status](https://gitlab.com/dsbowen/conditional-inference/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
+[![coverage report](https://gitlab.com/dsbowen/conditional-inference/badges/master/coverage.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
+[![PyPI version](https://badge.fury.io/py/conditional-inference.svg)](https://badge.fury.io/py/conditional-inference)
+[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/conditional-inference/-/blob/master/LICENSE)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fconditional-inference/HEAD?urlpath=lab/tree/examples)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 A statistics package for comparing multiple parameters. Read the docs [here](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest).
```

### Comparing `multiple-inference-1.1.0/setup.cfg` & `multiple-inference-1.2.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,81 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206d 756c 7469 706c 652d 696e 6665   = multiple-infe
-00000020: 7265 6e63 650d 0a76 6572 7369 6f6e 203d  rence..version =
-00000030: 2061 7474 723a 206d 756c 7469 706c 655f   attr: multiple_
-00000040: 696e 6665 7265 6e63 652e 5f5f 7665 7273  inference.__vers
-00000050: 696f 6e5f 5f0d 0a61 7574 686f 7220 3d20  ion__..author = 
-00000060: 4469 6c6c 6f6e 2042 6f77 656e 0d0a 6175  Dillon Bowen..au
-00000070: 7468 6f72 5f65 6d61 696c 203d 2064 7362  thor_email = dsb
-00000080: 6f77 656e 4077 6861 7274 6f6e 2e75 7065  owen@wharton.upe
-00000090: 6e6e 2e65 6475 0d0a 6465 7363 7269 7074  nn.edu..descript
-000000a0: 696f 6e20 3d20 4120 7374 6174 6973 7469  ion = A statisti
-000000b0: 6373 2070 6163 6b61 6765 2066 6f72 2063  cs package for c
-000000c0: 6f6d 7061 7269 6e67 206d 756c 7469 706c  omparing multipl
-000000d0: 6520 7061 7261 6d65 7465 7273 2e0d 0a6c  e parameters...l
-000000e0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000f0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-00000100: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-00000110: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000120: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000130: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000140: 6473 626f 7765 6e2e 6769 746c 6162 2e69  dsbowen.gitlab.i
-00000150: 6f2f 636f 6e64 6974 696f 6e61 6c2d 696e  o/conditional-in
-00000160: 6665 7265 6e63 650d 0a63 6c61 7373 6966  ference..classif
-00000170: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-00000180: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000190: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-000001a0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000001b0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-000001c0: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
-000001d0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-000001e0: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
-000001f0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000200: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
-00000210: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000220: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-00000230: 7265 7320 3d20 3e3d 332e 380d 0a69 6e73  res = >=3.8..ins
-00000240: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000250: 0d0a 096d 6174 706c 6f74 6c69 6220 3e3d  ...matplotlib >=
-00000260: 2033 2e34 0d0a 096e 756d 7079 203e 3d20   3.4...numpy >= 
-00000270: 312e 3230 0d0a 0973 6369 6b69 742d 6c65  1.20...scikit-le
-00000280: 6172 6e20 3e3d 2031 2e30 2e32 0d0a 0973  arn >= 1.0.2...s
-00000290: 6369 7079 203e 3d20 312e 360d 0a09 7365  cipy >= 1.6...se
-000002a0: 6162 6f72 6e20 3e3d 2030 2e31 312e 310d  aborn >= 0.11.1.
-000002b0: 0a09 7374 6174 736d 6f64 656c 7320 3e3d  ..statsmodels >=
-000002c0: 2030 2e31 320d 0a09 7479 7069 6e67 2d65   0.12...typing-e
-000002d0: 7874 656e 7369 6f6e 7320 3e3d 2033 2e31  xtensions >= 3.1
-000002e0: 302e 302e 300d 0a0d 0a5b 6f70 7469 6f6e  0.0.0....[option
-000002f0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000300: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000310: 0a5b 6275 696c 645f 7370 6869 6e78 5d0d  .[build_sphinx].
-00000320: 0a70 726f 6a65 6374 203d 204d 756c 7469  .project = Multi
-00000330: 706c 6520 496e 6665 7265 6e63 650d 0a63  ple Inference..c
-00000340: 6f70 7972 6967 6874 203d 2032 3032 312c  opyright = 2021,
-00000350: 2044 696c 6c6f 6e20 426f 7765 6e0d 0a72   Dillon Bowen..r
-00000360: 656c 6561 7365 203d 2061 7474 723a 206d  elease = attr: m
-00000370: 756c 7469 706c 655f 696e 6665 7265 6e63  ultiple_inferenc
-00000380: 652e 5f5f 7665 7273 696f 6e5f 5f0d 0a73  e.__version__..s
-00000390: 6f75 7263 652d 6469 7220 3d20 646f 6373  ource-dir = docs
-000003a0: 0d0a 0d0a 5b63 6f76 6572 6167 653a 7265  ....[coverage:re
-000003b0: 706f 7274 5d0d 0a65 7863 6c75 6465 5f6c  port]..exclude_l
-000003c0: 696e 6573 203d 200d 0a09 7072 6167 6d61  ines = ...pragma
-000003d0: 3a20 6e6f 2063 6f76 6572 0d0a 090d 0a09  : no cover......
-000003e0: 7261 6973 6520 4173 7365 7274 696f 6e45  raise AssertionE
-000003f0: 7272 6f72 0d0a 0972 6169 7365 2041 7474  rror...raise Att
-00000400: 7269 6275 7465 4572 726f 720d 0a09 7261  ributeError...ra
-00000410: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-00000420: 6564 4572 726f 720d 0a09 7261 6973 6520  edError...raise 
-00000430: 5661 6c75 6545 7272 6f72 0d0a 0977 6172  ValueError...war
-00000440: 6e69 6e67 732e 7761 726e 0d0a 090d 0a09  nings.warn......
-00000450: 6966 2030 3a0d 0a09 6966 205f 5f6e 616d  if 0:...if __nam
-00000460: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
-00000470: 223a 0d0a 6f6d 6974 203d 200d 0a09 7465  ":..omit = ...te
-00000480: 7374 732f 2a0d 0a09 7665 6e76 2f2a 0d0a  sts/*...venv/*..
-00000490: 0d0a 5b6d 7970 795d 0d0a 6967 6e6f 7265  ..[mypy]..ignore
-000004a0: 5f6d 6973 7369 6e67 5f69 6d70 6f72 7473  _missing_imports
-000004b0: 203d 2054 7275 650d 0a0d 0a5b 7079 6c69   = True....[pyli
-000004c0: 6e74 2e62 6173 6963 5d0d 0a67 6f6f 642d  nt.basic]..good-
-000004d0: 6e61 6d65 7320 3d20 582c 585f 542c 5854  names = X,X_T,XT
-000004e0: 5f74 6175 696e 765f 582c 5854 5f74 6175  _tauinv_X,XT_tau
-000004f0: 696e 765f 585f 696e 762c 612c 6178 2c62  inv_X_inv,a,ax,b
-00000500: 2c64 662c 6478 2c69 2c6a 2c6d 752c 782c  ,df,dx,i,j,mu,x,
-00000510: 7830 2c78 692c 5f0d 0a0d 0a5b 6567 675f  x0,xi,_....[egg_
-00000520: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000530: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000540: 300d 0a0d 0a                             0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6d75 6c74 6970 6c65 2d69 6e66 6572  = multiple-infer
+00000020: 656e 6365 0a76 6572 7369 6f6e 203d 2061  ence.version = a
+00000030: 7474 723a 206d 756c 7469 706c 655f 696e  ttr: multiple_in
+00000040: 6665 7265 6e63 652e 5f5f 7665 7273 696f  ference.__versio
+00000050: 6e5f 5f0a 6175 7468 6f72 203d 2044 696c  n__.author = Dil
+00000060: 6c6f 6e20 426f 7765 6e0a 6175 7468 6f72  lon Bowen.author
+00000070: 5f65 6d61 696c 203d 2064 7362 6f77 656e  _email = dsbowen
+00000080: 4077 6861 7274 6f6e 2e75 7065 6e6e 2e65  @wharton.upenn.e
+00000090: 6475 0a64 6573 6372 6970 7469 6f6e 203d  du.description =
+000000a0: 2041 2073 7461 7469 7374 6963 7320 7061   A statistics pa
+000000b0: 636b 6167 6520 666f 7220 636f 6d70 6172  ckage for compar
+000000c0: 696e 6720 6d75 6c74 6970 6c65 2070 6172  ing multiple par
+000000d0: 616d 6574 6572 732e 0a6c 6f6e 675f 6465  ameters..long_de
+000000e0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+000000f0: 3a20 5245 4144 4d45 2e6d 640a 6c6f 6e67  : README.md.long
+00000100: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+00000110: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+00000120: 2f6d 6172 6b64 6f77 6e0a 7572 6c20 3d20  /markdown.url = 
+00000130: 6874 7470 733a 2f2f 6473 626f 7765 6e2e  https://dsbowen.
+00000140: 6769 746c 6162 2e69 6f2f 636f 6e64 6974  gitlab.io/condit
+00000150: 696f 6e61 6c2d 696e 6665 7265 6e63 650a  ional-inference.
+00000160: 636c 6173 7369 6669 6572 7320 3d20 0a09  classifiers = ..
+00000170: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000180: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000190: 3a20 330a 094c 6963 656e 7365 203a 3a20  : 3..License :: 
+000001a0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+000001b0: 4d49 5420 4c69 6365 6e73 650a 094f 7065  MIT License..Ope
+000001c0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000001d0: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+000001e0: 0a5b 6f70 7469 6f6e 735d 0a70 6163 6b61  .[options].packa
+000001f0: 6765 5f64 6972 203d 200a 093d 2073 7263  ge_dir = ..= src
+00000200: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000210: 3a0a 7079 7468 6f6e 5f72 6571 7569 7265  :.python_require
+00000220: 7320 3d20 3e3d 332e 380a 696e 7374 616c  s = >=3.8.instal
+00000230: 6c5f 7265 7175 6972 6573 203d 200a 096d  l_requires = ..m
+00000240: 6174 706c 6f74 6c69 6220 3e3d 2033 2e34  atplotlib >= 3.4
+00000250: 0a09 6e75 6d70 7920 3e3d 2031 2e32 300a  ..numpy >= 1.20.
+00000260: 0973 6369 6b69 742d 6c65 6172 6e20 3e3d  .scikit-learn >=
+00000270: 2031 2e30 2e32 0a09 7363 6970 7920 3e3d   1.0.2..scipy >=
+00000280: 2031 2e36 0a09 7365 6162 6f72 6e20 3e3d   1.6..seaborn >=
+00000290: 2030 2e31 312e 310a 0973 7461 7473 6d6f   0.11.1..statsmo
+000002a0: 6465 6c73 203e 3d20 302e 3132 0a09 7479  dels >= 0.12..ty
+000002b0: 7069 6e67 2d65 7874 656e 7369 6f6e 7320  ping-extensions 
+000002c0: 3e3d 2033 2e31 302e 302e 300a 0a5b 6f70  >= 3.10.0.0..[op
+000002d0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+000002e0: 696e 645d 0a77 6865 7265 203d 2073 7263  ind].where = src
+000002f0: 0a0a 5b62 7569 6c64 5f73 7068 696e 785d  ..[build_sphinx]
+00000300: 0a70 726f 6a65 6374 203d 204d 756c 7469  .project = Multi
+00000310: 706c 6520 496e 6665 7265 6e63 650a 636f  ple Inference.co
+00000320: 7079 7269 6768 7420 3d20 3230 3231 2c20  pyright = 2021, 
+00000330: 4469 6c6c 6f6e 2042 6f77 656e 0a72 656c  Dillon Bowen.rel
+00000340: 6561 7365 203d 2061 7474 723a 206d 756c  ease = attr: mul
+00000350: 7469 706c 655f 696e 6665 7265 6e63 652e  tiple_inference.
+00000360: 5f5f 7665 7273 696f 6e5f 5f0a 736f 7572  __version__.sour
+00000370: 6365 2d64 6972 203d 2064 6f63 730a 0a5b  ce-dir = docs..[
+00000380: 636f 7665 7261 6765 3a72 6570 6f72 745d  coverage:report]
+00000390: 0a65 7863 6c75 6465 5f6c 696e 6573 203d  .exclude_lines =
+000003a0: 200a 0970 7261 676d 613a 206e 6f20 636f   ..pragma: no co
+000003b0: 7665 720a 090a 0972 6169 7365 2041 7373  ver....raise Ass
+000003c0: 6572 7469 6f6e 4572 726f 720a 0972 6169  ertionError..rai
+000003d0: 7365 2041 7474 7269 6275 7465 4572 726f  se AttributeErro
+000003e0: 720a 0972 6169 7365 204e 6f74 496d 706c  r..raise NotImpl
+000003f0: 656d 656e 7465 6445 7272 6f72 0a09 7261  ementedError..ra
+00000400: 6973 6520 5661 6c75 6545 7272 6f72 0a09  ise ValueError..
+00000410: 7761 726e 696e 6773 2e77 6172 6e0a 090a  warnings.warn...
+00000420: 0969 6620 303a 0a09 6966 205f 5f6e 616d  .if 0:..if __nam
+00000430: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
+00000440: 223a 0a6f 6d69 7420 3d20 0a09 7465 7374  ":.omit = ..test
+00000450: 732f 2a0a 0976 656e 762f 2a0a 0a5b 6d79  s/*..venv/*..[my
+00000460: 7079 5d0a 6967 6e6f 7265 5f6d 6973 7369  py].ignore_missi
+00000470: 6e67 5f69 6d70 6f72 7473 203d 2054 7275  ng_imports = Tru
+00000480: 650a 0a5b 7079 6c69 6e74 2e62 6173 6963  e..[pylint.basic
+00000490: 5d0a 676f 6f64 2d6e 616d 6573 203d 2058  ].good-names = X
+000004a0: 2c58 5f54 2c58 545f 7461 7569 6e76 5f58  ,X_T,XT_tauinv_X
+000004b0: 2c58 545f 7461 7569 6e76 5f58 5f69 6e76  ,XT_tauinv_X_inv
+000004c0: 2c61 2c61 782c 622c 6466 2c64 782c 692c  ,a,ax,b,df,dx,i,
+000004d0: 6a2c 6d75 2c78 2c78 302c 7869 2c5f 0a0a  j,mu,x,x0,xi,_..
+000004e0: 5b65 6767 5f69 6e66 6f5d 0a74 6167 5f62  [egg_info].tag_b
+000004f0: 7569 6c64 203d 200a 7461 675f 6461 7465  uild = .tag_date
+00000500: 203d 2030 0a0a                            = 0..
```

### Comparing `multiple-inference-1.1.0/src/multiple_inference/base.py` & `multiple-inference-1.2.0/src/multiple_inference/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,477 +1,473 @@
-"""Base classes.
-"""
-from __future__ import annotations
-
-import pickle
-from typing import Any, Optional, Sequence, Type, TypeVar, Union
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-from statsmodels.base.model import LikelihoodModelResults
-from statsmodels.iolib.summary import Summary
-from statsmodels.iolib.table import SimpleTable
-
-# TODO: remove type ignore statements for starred arguments when this issue is fixed
-# https://github.com/python/mypy/issues/6799
-
-ColumnType = Union[str, int]
-ColumnsType = Union[Sequence[int], Sequence[str], Sequence[bool]]
-ModelType = TypeVar("ModelType", bound="ModelBase")
-Numeric1DArray = Sequence[float]
-ResultsType = TypeVar("ResultsType", bound="ResultsBase")
-
-
-class ResultsBase:
-    """Base for results classes.
-
-    Args:
-        model (ModelBase): Model on which the results are based.
-        title (str, optional): Results title. Defaults to "Estimation results".
-    """
-
-    _default_title = "Estimation results"
-
-    def __init__(
-        self,
-        model: ModelType,
-        title: str = None,
-    ):
-        self.model = model
-        self.exog_names = model.exog_names.copy()
-        if not hasattr(self, "pvalues"):
-            self.pvalues = np.full(len(model.mean), np.nan)
-        self.title = title
-        self._conf_int_cached = {}
-
-    @property
-    def title(self) -> str:
-        return self._title or self._default_title
-
-    @title.setter
-    def title(self, title: str) -> None:
-        self._title = title
-
-    def conf_int(
-        self, alpha: float = 0.05, columns: ColumnsType = None, **kwargs: Any
-    ) -> np.ndarray:
-        """Compute the 1-alpha confidence interval.
-
-        Args:
-            alpha (float, optional): The CI will cover the truth with probability
-                1-alpha. Defaults to 0.05.
-            columns (ColumnsType, optional): Selected columns. Defaults to None.
-
-        Returns:
-            np.ndarray: (# params, 2) array of confidence intervals.
-        """
-        return self._conf_int(
-            alpha, self.model.get_indices(columns, self.exog_names), **kwargs
-        )
-
-    def _conf_int(self, alpha: float, indices: np.array) -> np.ndarray:
-        if not hasattr(self, "marginal_distributions"):
-            raise AttributeError(
-                "Results object does not have `marginal_distributions` attribute."
-            )
-
-        return np.array(
-            [
-                self.marginal_distributions[i].ppf([alpha / 2, 1 - alpha / 2])
-                for i in indices
-            ]
-        )
-
-    def point_plot(
-        self,
-        yname: str = None,
-        xname: Sequence[str] = None,
-        title: str = None,
-        alpha: float = 0.05,
-        columns: ColumnsType = None,
-        spacing: float = 1,
-        ax=None,
-        **kwargs: Any,
-    ):
-        """Create a point plot.
-
-        Args:
-            yname (str, optional): Name of the endogenous variable. Defaults to None.
-            xname (Sequence[str], optional): (# params,) sequence of parameter names.
-                Defaults to None.
-            title (str, optional): Plot title. Defaults to None.
-            alpha (float, optional): Plot the 1-alpha CI. Defaults to 0.05.
-            columns (ColumnsType, optional): Selected columns. Defaults to None.
-            spacing (float): Spacing on the horizontal axis. Defaults to 1.
-            ax (AxesSubplot, optional): Axis to write on.
-            **kwargs (Any): Passed to :meth:`ResultsBase.conf_int`.
-
-        Returns:
-            AxesSubplot: Plot.
-        """
-
-        if not hasattr(self, "params"):
-            raise AttributeError("Results object does not have `params` attribute.")
-
-        indices = self.model.get_indices(columns, self.exog_names)
-        params = self.params[indices]
-        conf_int = self.conf_int(alpha, columns, **kwargs)
-        yticks = spacing * np.arange(len(indices), 0, -1)
-
-        if ax is None:
-            _, ax = plt.subplots()
-        ax.errorbar(
-            x=params,  # type: ignore, pylint: disable=no-member
-            y=yticks,
-            xerr=[params - conf_int[:, 0], conf_int[:, 1] - params],  # type: ignore, pylint: disable=no-member
-            fmt="o",
-        )
-        ax.set_title(title or self.title)
-        ax.set_xlabel(yname or self.model.endog_names)
-        ax.set_yticks(yticks)
-        ax.set_yticklabels(self.exog_names[indices] if xname is None else xname)
-
-        return ax
-
-    def save(self: ResultsType, filename: str) -> None:
-        """Pickle results.
-
-        Args:
-            filename (str): File name.
-        """
-        with open(filename, "wb") as results_file:
-            pickle.dump(self, results_file)
-
-    def summary(
-        self,
-        yname: str = None,
-        xname: Sequence[str] = None,
-        title: str = None,
-        alpha: float = 0.05,
-        columns: ColumnsType = None,
-        **kwargs: Any,
-    ) -> Summary:
-        """Create a summary table.
-
-        Args:
-            yname (str, optional): Name of the endogenous variable. Defaults to None.
-            xname (Sequence[str], optional): Names of the exogenous variables. Defaults
-                to None.
-            title (str, optional): Table title. Defaults to None.
-            alpha (float, optional): Display 1-alpha confidence interval. Defaults to
-                0.05.
-            columns (ColumnsType, optional): Selected columns. Defaults to None.
-            **kwargs (Any): Passed to :meth:`ResultsBase.conf_int`.
-
-        Returns:
-            Summary: Summary table.
-        """
-        indices = self.model.get_indices(columns, self.exog_names)
-        params_header = self._make_summary_header(alpha)
-        params_data = self._make_summary_data(alpha, indices, **kwargs)
-        params_data_str = [[f"{val:.3f}" for val in row] for row in params_data]
-        if xname is None:
-            xname = self.exog_names[indices]
-
-        smry = Summary()
-        smry.tables = [
-            SimpleTable(
-                params_data_str,
-                params_header,
-                list(xname),
-                title=title or self.title,
-            ),
-            SimpleTable(
-                [[yname or self.model.endog_names]],
-                stubs=["Dep. Variable"],
-            ),
-        ]
-
-        return smry
-
-    def _make_summary_header(self, alpha: float) -> list[str]:
-        # make the header for the summary table
-        # when subclassing ResultsBase, you may wish to overwrite this method
-        return ["coef", "pvalue", f"[{alpha/2}", f"{1-alpha/2}]"]
-
-    def _make_summary_data(
-        self, alpha: float, indices: np.ndarray, **kwargs: Any
-    ) -> np.ndarray:
-        # make the data for the summary table
-        # returns (# params, # columns) array
-        # columns should correspond to the output of _make_summary_header
-        if not hasattr(self, "params"):
-            raise AttributeError("Results object does not have `params` attribute.")
-
-        return np.hstack(
-            (np.array([self.params, self.pvalues]).T[indices], self.conf_int(alpha, indices, **kwargs))  # type: ignore, pylint: disable=no-member
-        )
-
-
-class ModelBase:
-    """Base for model classes.
-
-    Args:
-        mean (Numeric1DArray): (# params,) array of conventionally estimated means.
-        cov (np.ndarray): (# params, # params) covariance matrix.
-        X (np.ndarray, optional): (# params, # features) feature matrix. Defaults to
-            None.
-        endog_names (str, optional): Name of endogenous variable. Defaults to None.
-        exog_names (Sequence[str], optional): Names of the exogenous variables. Defaults
-            to None.
-        columns (ColumnsType, optional): Columns to use. This can be a sequence of
-            indices (int), parameter names (str), or a Boolean mask. Defaults to None.
-        sort (bool, optional): Sort the parameters by the conventionally estimated
-            mean. Defaults to False.
-        seed (int, optional): Random seed. Defaults to 0.
-
-    Attributes:
-        n_params (int): Number of estimated parameters.
-        mean (np.ndarray): (# params,) array of conventionally estimated means.
-        cov (np.ndarray): (# params, # params) covariance matrix.
-        X (np.ndarray): (# params, # features) feature matrix.
-        endog_names (str): Name of the endogenous variable.
-        exog_names (np.ndarray): Name of exogenous variables.
-        seed (int): Random seed.
-    """
-
-    _results_cls = ResultsBase
-
-    def __init__(
-        self,
-        mean: Numeric1DArray,
-        cov: np.ndarray,
-        X: np.ndarray = None,
-        endog_names: str = None,
-        exog_names: Sequence[str] = None,
-        columns: ColumnsType = None,
-        sort: bool = False,
-        random_state: int = 0,
-    ):
-        self.mean = mean
-        self.n_params = len(self.mean) if columns is None else len(columns)
-        self.cov = cov * np.identity(self.n_params) if np.isscalar(cov) else cov
-        self.X = np.ones((len(self.mean), 1)) if X is None else X
-        self.endog_names = endog_names
-        if exog_names is None and isinstance(mean, pd.Series):
-            self.exog_names = np.array(mean.index)
-        else:
-            self.exog_names = exog_names
-        self.random_state = random_state
-
-        # select columns
-        indices = self.get_indices(columns)
-        self.mean = self.mean[indices]
-        self.cov = self.cov[indices][:, indices]
-        self.X = self.X[indices]
-        if exog_names is not None or isinstance(mean, pd.Series):
-            self.exog_names = self.exog_names[indices]
-
-        # sort columns
-        if sort:
-            argsort = (-self.mean).argsort()
-            self.mean = self.mean[argsort]
-            self.cov = self.cov[argsort][:, argsort]
-            self.X = self.X[argsort]
-            if exog_names is not None or isinstance(mean, pd.Series):
-                self.exog_names = self.exog_names[argsort]
-
-    @property
-    def mean(self) -> np.ndarray:  # pylint: disable=missing-function-docstring
-        return self._mean
-
-    @mean.setter
-    def mean(
-        self, mean: Numeric1DArray
-    ) -> None:  # pylint: disable=missing-function-docstring
-        self._mean = np.atleast_1d(mean)
-
-    @property
-    def cov(self) -> np.ndarray:
-        return self._cov
-
-    @cov.setter
-    def cov(self, cov: np.ndarray) -> None:
-        self._cov = np.atleast_2d(cov)
-
-    @property
-    def endog_names(self) -> str:  # pylint: disable=missing-function-docstring
-        return "y" if self._endog_names is None else self._endog_names
-
-    @endog_names.setter
-    def endog_names(
-        self, endog_names: str
-    ) -> None:  # pylint: disable=missing-function-docstring
-        self._endog_names = endog_names
-
-    @property
-    def exog_names(self) -> np.ndarray:  # pylint: disable=missing-function-docstring
-        if self._exog_names is not None:
-            return self._exog_names
-        zfill = int(np.log10(max(1, len(self.mean) - 1))) + 1
-        return np.array([f"x{str(i).zfill(zfill)}" for i in range(len(self.mean))])
-
-    @exog_names.setter
-    def exog_names(
-        self, exog_names: Optional[Sequence[str]]
-    ) -> None:  # pylint: disable=missing-function-docstring
-        self._exog_names = None if exog_names is None else np.atleast_1d(exog_names)
-
-    @classmethod
-    def from_results(
-        cls: Type[ModelType],
-        results: LikelihoodModelResults,
-        **kwargs: Any,
-    ) -> ModelType:
-        """Initialize an estimator from conventional regression results.
-
-        Args:
-            results (LikelihoodModelResults): Conventional estimation results.
-            **kwargs (Any): Passed to the model class constructor.
-
-        Returns:
-            Model: Estimator.
-
-        Examples:
-
-            .. testcode::
-
-                import numpy as np
-                import pandas as pd
-                import statsmodels.api as sm
-                from multiple_inference.base import ModelBase
-
-                X = np.repeat(np.identity(3), 100, axis=0)
-                beta = np.arange(3)
-                y = X @ beta + np.random.normal(size=300)
-                ols_results = sm.OLS(y, X).fit()
-                model = ModelBase.from_results(ols_results)
-                print(model.mean)
-                print(model.cov)
-
-            .. testoutput::
-
-                [0.05980802 1.08201297 1.94076774]
-                [[0.01007633 0.         0.        ]
-                 [0.         0.01007633 0.        ]
-                 [0.         0.         0.01007633]]
-        """
-        cov = results.cov_params()
-        if isinstance(cov, pd.DataFrame):
-            cov = cov.values
-
-        return cls(
-            results.params,
-            cov,
-            endog_names=kwargs.pop("endog_names", results.model.endog_names),
-            exog_names=kwargs.pop("exog_names", results.model.exog_names),
-            **kwargs,
-        )
-
-    @classmethod
-    def from_csv(
-        cls: Type[ModelType],
-        filename: str,
-        **kwargs: Any,
-    ) -> ModelType:
-        """Instantiate an estimator from csv file.
-
-        Args:
-            filename (str): Name of the csv file.
-            **kwargs (Any): Passed to the model class constructor.
-
-        Returns:
-            Model: Estimator.
-        """
-        df = pd.read_csv(filename)
-        mean, cov = df.values[:, 0], df.values[:, 1:]  # pylint: disable=no-member
-        endog_names, exog_names = (
-            df.columns[0],  # pylint: disable=no-member
-            df.columns[1:],  # pylint: disable=no-member
-        )
-
-        return cls(
-            mean,
-            cov,
-            endog_names=kwargs.pop("endog_names", endog_names),
-            exog_names=kwargs.pop("exog_names", exog_names),
-            **kwargs,
-        )
-
-    def to_csv(self, filename: str) -> None:
-        """Write data to a csv.
-
-        Args:
-            filename (str): Name of the file to write to.
-        """
-        pd.DataFrame(
-            np.hstack((self.mean.reshape(-1, 1), self.cov)),
-            columns=[self.endog_names] + list(self.exog_names),
-        ).to_csv(filename, index=False)
-
-    def fit(self, *args: Any, **kwargs: Any) -> ResultsType:
-        """Fit the model.
-
-        Args:
-            *args (Any): Passed to the results class constructor.
-            **kwargs (Any): Passed to the results class constructor.
-
-        Returns:
-            ResultsType: Results.
-        """
-        return self._results_cls(self, *args, **kwargs)
-
-    def get_index(self, column: ColumnType, names: Sequence[str] = None) -> int:
-        """Get the index of a selected column.
-
-        Args:
-            column (ColumnType): Index or name of selected column.
-            names (Sequence[str], optional): (# params,) sequence of names to select
-                from.
-
-        Returns:
-            int: Index.
-        """
-        try:
-            return int(column)
-        except:
-            pass
-
-        return list(self.exog_names if names is None else names).index(column)
-
-    def get_indices(
-        self, columns: ColumnsType = None, names: Sequence[str] = None
-    ) -> np.ndarray:
-        """Get indices of the selected columns.
-
-        Args:
-            columns (ColumnsType, optional): Sequence of columns to select. The
-            sequence can be a (# selected params,) sequence of column names (str) or
-            indices (int), or a (# params,) boolean mask. Defaults to None.
-            names (Sequence[str], optional): (# params,) sequence of names to select
-                from.
-
-        Returns:
-            np.ndarray: (# selected params,) array of indices.
-        """
-        if names is None:
-            names = self.exog_names
-
-        if columns is None:
-            return np.arange(len(names)).astype(int)
-
-        cols = np.atleast_1d(columns)
-        if cols.dtype == np.dtype("float"):
-            cols = cols.astype(int)
-
-        if cols.dtype in (np.dtype(int), np.dtype("int64")):
-            # cols is a sequence of indices
-            return cols
-
-        if cols.dtype == np.dtype(bool):
-            # cols is a boolean mask
-            return np.where(cols)[0]
-
-        # cols are the parameter names (exogenous variables)
-        sorter = np.argsort(names)
-        return sorter[np.searchsorted(names, cols, sorter=sorter)]
+"""Base classes.
+"""
+from __future__ import annotations
+
+import pickle
+from typing import Any, Optional, Sequence, Type, TypeVar, Union
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+from statsmodels.base.model import LikelihoodModelResults
+from statsmodels.iolib.summary import Summary
+from statsmodels.iolib.table import SimpleTable
+
+# TODO: remove type ignore statements for starred arguments when this issue is fixed
+# https://github.com/python/mypy/issues/6799
+
+ColumnType = Union[str, int]
+ColumnsType = Union[Sequence[int], Sequence[str], Sequence[bool]]
+ModelType = TypeVar("ModelType", bound="ModelBase")
+Numeric1DArray = Sequence[float]
+ResultsType = TypeVar("ResultsType", bound="ResultsBase")
+
+
+class ResultsBase:
+    """Base for results classes.
+
+    Args:
+        model (ModelBase): Model on which the results are based.
+        title (str, optional): Results title. Defaults to "Estimation results".
+    """
+
+    _default_title = "Estimation results"
+
+    def __init__(
+        self,
+        model: ModelType,
+        title: str = None,
+    ):
+        self.model = model
+        self.exog_names = model.exog_names.copy()
+        if not hasattr(self, "pvalues"):
+            self.pvalues = np.full(len(model.mean), np.nan)
+        self.title = title
+        self._conf_int_cached = {}
+
+    @property
+    def title(self) -> str:
+        return self._title or self._default_title
+
+    @title.setter
+    def title(self, title: str) -> None:
+        self._title = title
+
+    def conf_int(
+        self, alpha: float = 0.05, columns: ColumnsType = None, **kwargs: Any
+    ) -> np.ndarray:
+        """Compute the 1-alpha confidence interval.
+
+        Args:
+            alpha (float, optional): The CI will cover the truth with probability
+                1-alpha. Defaults to 0.05.
+            columns (ColumnsType, optional): Selected columns. Defaults to None.
+
+        Returns:
+            np.ndarray: (# params, 2) array of confidence intervals.
+        """
+        return self._conf_int(
+            alpha, self.model.get_indices(columns, self.exog_names), **kwargs
+        )
+
+    def _conf_int(self, alpha: float, indices: np.array) -> np.ndarray:
+        if not hasattr(self, "marginal_distributions"):
+            raise AttributeError(
+                "Results object does not have `marginal_distributions` attribute."
+            )
+
+        return np.array(
+            [
+                self.marginal_distributions[i].ppf([alpha / 2, 1 - alpha / 2])
+                for i in indices
+            ]
+        )
+
+    def point_plot(
+        self,
+        yname: str = None,
+        xname: Sequence[str] = None,
+        title: str = None,
+        columns: ColumnsType = None,
+        ax=None,
+        **kwargs: Any,
+    ):
+        """Create a point plot.
+
+        Args:
+            yname (str, optional): Name of the endogenous variable. Defaults to None.
+            xname (Sequence[str], optional): (# params,) sequence of parameter names.
+                Defaults to None.
+            title (str, optional): Plot title. Defaults to None.
+            columns (ColumnsType, optional): Selected columns. Defaults to None.
+            ax (AxesSubplot, optional): Axis to write on.
+            **kwargs (Any): Passed to :meth:`ResultsBase.conf_int`.
+
+        Returns:
+            AxesSubplot: Plot.
+        """
+
+        if not hasattr(self, "params"):
+            raise AttributeError("Results object does not have `params` attribute.")
+
+        indices = self.model.get_indices(columns, self.exog_names)
+        params = self.params[indices]
+        conf_int = self.conf_int(columns=columns, **kwargs)
+        yticks = np.arange(len(indices), 0, -1)
+
+        if ax is None:
+            _, ax = plt.subplots()
+        ax.errorbar(
+            x=params,  # type: ignore, pylint: disable=no-member
+            y=yticks,
+            xerr=[params - conf_int[:, 0], conf_int[:, 1] - params],  # type: ignore, pylint: disable=no-member
+            fmt="o",
+        )
+        ax.set_title(title or self.title)
+        ax.set_xlabel(yname or self.model.endog_names)
+        ax.set_yticks(yticks)
+        ax.set_yticklabels(self.exog_names[indices] if xname is None else xname)
+
+        return ax
+
+    def save(self: ResultsType, filename: str) -> None:
+        """Pickle results.
+
+        Args:
+            filename (str): File name.
+        """
+        with open(filename, "wb") as results_file:
+            pickle.dump(self, results_file)
+
+    def summary(
+        self,
+        yname: str = None,
+        xname: Sequence[str] = None,
+        title: str = None,
+        alpha: float = 0.05,
+        columns: ColumnsType = None,
+        **kwargs: Any,
+    ) -> Summary:
+        """Create a summary table.
+
+        Args:
+            yname (str, optional): Name of the endogenous variable. Defaults to None.
+            xname (Sequence[str], optional): Names of the exogenous variables. Defaults
+                to None.
+            title (str, optional): Table title. Defaults to None.
+            alpha (float, optional): Display 1-alpha confidence interval. Defaults to
+                0.05.
+            columns (ColumnsType, optional): Selected columns. Defaults to None.
+            **kwargs (Any): Passed to :meth:`ResultsBase.conf_int`.
+
+        Returns:
+            Summary: Summary table.
+        """
+        indices = self.model.get_indices(columns, self.exog_names)
+        params_header = self._make_summary_header(alpha)
+        params_data = self._make_summary_data(alpha, indices, **kwargs)
+        params_data_str = [[f"{val:.3f}" for val in row] for row in params_data]
+        if xname is None:
+            xname = self.exog_names[indices]
+
+        smry = Summary()
+        smry.tables = [
+            SimpleTable(
+                params_data_str,
+                params_header,
+                list(xname),
+                title=title or self.title,
+            ),
+            SimpleTable(
+                [[yname or self.model.endog_names]],
+                stubs=["Dep. Variable"],
+            ),
+        ]
+
+        return smry
+
+    def _make_summary_header(self, alpha: float) -> list[str]:
+        # make the header for the summary table
+        # when subclassing ResultsBase, you may wish to overwrite this method
+        return ["coef", "pvalue", f"[{alpha/2}", f"{1-alpha/2}]"]
+
+    def _make_summary_data(
+        self, alpha: float, indices: np.ndarray, **kwargs: Any
+    ) -> np.ndarray:
+        # make the data for the summary table
+        # returns (# params, # columns) array
+        # columns should correspond to the output of _make_summary_header
+        if not hasattr(self, "params"):
+            raise AttributeError("Results object does not have `params` attribute.")
+
+        return np.hstack(
+            (np.array([self.params, self.pvalues]).T[indices], self.conf_int(alpha, indices, **kwargs))  # type: ignore, pylint: disable=no-member
+        )
+
+
+class ModelBase:
+    """Base for model classes.
+
+    Args:
+        mean (Numeric1DArray): (# params,) array of conventionally estimated means.
+        cov (np.ndarray): (# params, # params) covariance matrix.
+        X (np.ndarray, optional): (# params, # features) feature matrix. Defaults to
+            None.
+        endog_names (str, optional): Name of endogenous variable. Defaults to None.
+        exog_names (Sequence[str], optional): Names of the exogenous variables. Defaults
+            to None.
+        columns (ColumnsType, optional): Columns to use. This can be a sequence of
+            indices (int), parameter names (str), or a Boolean mask. Defaults to None.
+        sort (bool, optional): Sort the parameters by the conventionally estimated
+            mean. Defaults to False.
+        seed (int, optional): Random seed. Defaults to 0.
+
+    Attributes:
+        n_params (int): Number of estimated parameters.
+        mean (np.ndarray): (# params,) array of conventionally estimated means.
+        cov (np.ndarray): (# params, # params) covariance matrix.
+        X (np.ndarray): (# params, # features) feature matrix.
+        endog_names (str): Name of the endogenous variable.
+        exog_names (np.ndarray): Name of exogenous variables.
+        seed (int): Random seed.
+    """
+
+    _results_cls = ResultsBase
+
+    def __init__(
+        self,
+        mean: Numeric1DArray,
+        cov: np.ndarray,
+        X: np.ndarray = None,
+        endog_names: str = None,
+        exog_names: Sequence[str] = None,
+        columns: ColumnsType = None,
+        sort: bool = False,
+        random_state: int = 0,
+    ):
+        self.mean = mean
+        self.n_params = len(self.mean) if columns is None else len(columns)
+        self.cov = cov * np.identity(self.n_params) if np.isscalar(cov) else cov
+        self.X = np.ones((len(self.mean), 1)) if X is None else X
+        self.endog_names = endog_names
+        if exog_names is None and isinstance(mean, pd.Series):
+            self.exog_names = np.array(mean.index)
+        else:
+            self.exog_names = exog_names
+        self.random_state = random_state
+
+        # select columns
+        indices = self.get_indices(columns)
+        self.mean = self.mean[indices]
+        self.cov = self.cov[indices][:, indices]
+        self.X = self.X[indices]
+        if exog_names is not None or isinstance(mean, pd.Series):
+            self.exog_names = self.exog_names[indices]
+
+        # sort columns
+        if sort:
+            argsort = (-self.mean).argsort()
+            self.mean = self.mean[argsort]
+            self.cov = self.cov[argsort][:, argsort]
+            self.X = self.X[argsort]
+            if exog_names is not None or isinstance(mean, pd.Series):
+                self.exog_names = self.exog_names[argsort]
+
+    @property
+    def mean(self) -> np.ndarray:  # pylint: disable=missing-function-docstring
+        return self._mean
+
+    @mean.setter
+    def mean(
+        self, mean: Numeric1DArray
+    ) -> None:  # pylint: disable=missing-function-docstring
+        self._mean = np.atleast_1d(mean)
+
+    @property
+    def cov(self) -> np.ndarray:
+        return self._cov
+
+    @cov.setter
+    def cov(self, cov: np.ndarray) -> None:
+        self._cov = np.atleast_2d(cov)
+
+    @property
+    def endog_names(self) -> str:  # pylint: disable=missing-function-docstring
+        return "y" if self._endog_names is None else self._endog_names
+
+    @endog_names.setter
+    def endog_names(
+        self, endog_names: str
+    ) -> None:  # pylint: disable=missing-function-docstring
+        self._endog_names = endog_names
+
+    @property
+    def exog_names(self) -> np.ndarray:  # pylint: disable=missing-function-docstring
+        if self._exog_names is not None:
+            return self._exog_names
+        zfill = int(np.log10(max(1, len(self.mean) - 1))) + 1
+        return np.array([f"x{str(i).zfill(zfill)}" for i in range(len(self.mean))])
+
+    @exog_names.setter
+    def exog_names(
+        self, exog_names: Optional[Sequence[str]]
+    ) -> None:  # pylint: disable=missing-function-docstring
+        self._exog_names = None if exog_names is None else np.atleast_1d(exog_names)
+
+    @classmethod
+    def from_results(
+        cls: Type[ModelType],
+        results: LikelihoodModelResults,
+        **kwargs: Any,
+    ) -> ModelType:
+        """Initialize an estimator from conventional regression results.
+
+        Args:
+            results (LikelihoodModelResults): Conventional estimation results.
+            **kwargs (Any): Passed to the model class constructor.
+
+        Returns:
+            Model: Estimator.
+
+        Examples:
+
+            .. testcode::
+
+                import numpy as np
+                import pandas as pd
+                import statsmodels.api as sm
+                from multiple_inference.base import ModelBase
+
+                X = np.repeat(np.identity(3), 100, axis=0)
+                beta = np.arange(3)
+                y = X @ beta + np.random.normal(size=300)
+                ols_results = sm.OLS(y, X).fit()
+                model = ModelBase.from_results(ols_results)
+                print(model.mean)
+                print(model.cov)
+
+            .. testoutput::
+
+                [0.05980802 1.08201297 1.94076774]
+                [[0.01007633 0.         0.        ]
+                 [0.         0.01007633 0.        ]
+                 [0.         0.         0.01007633]]
+        """
+        cov = results.cov_params()
+        if isinstance(cov, pd.DataFrame):
+            cov = cov.values
+
+        return cls(
+            results.params,
+            cov,
+            endog_names=kwargs.pop("endog_names", results.model.endog_names),
+            exog_names=kwargs.pop("exog_names", results.model.exog_names),
+            **kwargs,
+        )
+
+    @classmethod
+    def from_csv(
+        cls: Type[ModelType],
+        filename: str,
+        **kwargs: Any,
+    ) -> ModelType:
+        """Instantiate an estimator from csv file.
+
+        Args:
+            filename (str): Name of the csv file.
+            **kwargs (Any): Passed to the model class constructor.
+
+        Returns:
+            Model: Estimator.
+        """
+        df = pd.read_csv(filename)
+        mean, cov = df.values[:, 0], df.values[:, 1:]  # pylint: disable=no-member
+        endog_names, exog_names = (
+            df.columns[0],  # pylint: disable=no-member
+            df.columns[1:],  # pylint: disable=no-member
+        )
+
+        return cls(
+            mean,
+            cov,
+            endog_names=kwargs.pop("endog_names", endog_names),
+            exog_names=kwargs.pop("exog_names", exog_names),
+            **kwargs,
+        )
+
+    def to_csv(self, filename: str) -> None:
+        """Write data to a csv.
+
+        Args:
+            filename (str): Name of the file to write to.
+        """
+        pd.DataFrame(
+            np.hstack((self.mean.reshape(-1, 1), self.cov)),
+            columns=[self.endog_names] + list(self.exog_names),
+        ).to_csv(filename, index=False)
+
+    def fit(self, *args: Any, **kwargs: Any) -> ResultsType:
+        """Fit the model.
+
+        Args:
+            *args (Any): Passed to the results class constructor.
+            **kwargs (Any): Passed to the results class constructor.
+
+        Returns:
+            ResultsType: Results.
+        """
+        return self._results_cls(self, *args, **kwargs)
+
+    def get_index(self, column: ColumnType, names: Sequence[str] = None) -> int:
+        """Get the index of a selected column.
+
+        Args:
+            column (ColumnType): Index or name of selected column.
+            names (Sequence[str], optional): (# params,) sequence of names to select
+                from.
+
+        Returns:
+            int: Index.
+        """
+        try:
+            return int(column)
+        except:
+            pass
+
+        return list(self.exog_names if names is None else names).index(column)
+
+    def get_indices(
+        self, columns: ColumnsType = None, names: Sequence[str] = None
+    ) -> np.ndarray:
+        """Get indices of the selected columns.
+
+        Args:
+            columns (ColumnsType, optional): Sequence of columns to select. The
+            sequence can be a (# selected params,) sequence of column names (str) or
+            indices (int), or a (# params,) boolean mask. Defaults to None.
+            names (Sequence[str], optional): (# params,) sequence of names to select
+                from.
+
+        Returns:
+            np.ndarray: (# selected params,) array of indices.
+        """
+        if names is None:
+            names = self.exog_names
+
+        if columns is None:
+            return np.arange(len(names)).astype(int)
+
+        cols = np.atleast_1d(columns)
+        if cols.dtype == np.dtype("float"):
+            cols = cols.astype(int)
+
+        if cols.dtype in (np.dtype(int), np.dtype("int64")):
+            # cols is a sequence of indices
+            return cols
+
+        if cols.dtype == np.dtype(bool):
+            # cols is a boolean mask
+            return np.where(cols)[0]
+
+        # cols are the parameter names (exogenous variables)
+        sorter = np.argsort(names)
+        return sorter[np.searchsorted(names, cols, sorter=sorter)]
```

### Comparing `multiple-inference-1.1.0/src/multiple_inference/bayes/improper.py` & `multiple-inference-1.2.0/src/multiple_inference/bayes/improper.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-"""Bayesian model with an improper prior.
-"""
-from __future__ import annotations
-
-import numpy as np
-from scipy.stats import multivariate_normal, norm, rv_continuous
-
-from .base import BayesBase
-
-
-class Improper(BayesBase):
-    """Bayesian model with an improper prior.
-
-    The improper prior is a uniform distribution on $(-\infty, \infty)$. The posterior
-    is equivalent to the conventionally estimated joint normal distribution.
-
-    Examples:
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.bayes import Improper
-
-            model = Improper(np.arange(10), np.identity(10))
-            results = model.fit()
-            print(results.summary())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-                       Bayesian estimates
-            =======================================
-                coef pvalue (1-sided) [0.025 0.975]
-            ---------------------------------------
-            x0 0.000            0.500 -1.960  1.960
-            x1 1.000            0.159 -0.960  2.960
-            x2 2.000            0.023  0.040  3.960
-            x3 3.000            0.001  1.040  4.960
-            x4 4.000            0.000  2.040  5.960
-            x5 5.000            0.000  3.040  6.960
-            x6 6.000            0.000  4.040  7.960
-            x7 7.000            0.000  5.040  8.960
-            x8 8.000            0.000  6.040  9.960
-            x9 9.000            0.000  7.040 10.960
-            ===============
-            Dep. Variable y
-            ---------------
-    """
-
-    def _get_marginal_prior(self, index: int) -> rv_continuous:
-        raise RuntimeError(
-            "The improper prior is a uniform distribution from -inf to inf"
-        )
-
-    def _get_marginal_distribution(self, index: int) -> rv_continuous:
-        return norm(self.mean[index], np.sqrt(self.cov[index, index]))
-
-    def _get_joint_prior(self, indices: np.ndarray):
-        raise RuntimeError(
-            "The improper prior is a uniform distribution from -inf to inf"
-        )
-
-    def _get_joint_distribution(self, indices: np.ndarray):
-        return multivariate_normal(self.mean[indices], self.cov[indices][:, indices])
+"""Bayesian model with an improper prior.
+"""
+from __future__ import annotations
+
+import numpy as np
+from scipy.stats import multivariate_normal, norm, rv_continuous
+
+from .base import BayesBase
+
+
+class Improper(BayesBase):
+    """Bayesian model with an improper prior.
+
+    The improper prior is a uniform distribution on $(-\infty, \infty)$. The posterior
+    is equivalent to the conventionally estimated joint normal distribution.
+
+    Examples:
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.bayes import Improper
+
+            model = Improper(np.arange(10), np.identity(10))
+            results = model.fit()
+            print(results.summary())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+                       Bayesian estimates
+            =======================================
+                coef pvalue (1-sided) [0.025 0.975]
+            ---------------------------------------
+            x0 0.000            0.500 -1.960  1.960
+            x1 1.000            0.159 -0.960  2.960
+            x2 2.000            0.023  0.040  3.960
+            x3 3.000            0.001  1.040  4.960
+            x4 4.000            0.000  2.040  5.960
+            x5 5.000            0.000  3.040  6.960
+            x6 6.000            0.000  4.040  7.960
+            x7 7.000            0.000  5.040  8.960
+            x8 8.000            0.000  6.040  9.960
+            x9 9.000            0.000  7.040 10.960
+            ===============
+            Dep. Variable y
+            ---------------
+    """
+
+    def _get_marginal_prior(self, index: int) -> rv_continuous:
+        raise RuntimeError(
+            "The improper prior is a uniform distribution from -inf to inf"
+        )
+
+    def _get_marginal_distribution(self, index: int) -> rv_continuous:
+        return norm(self.mean[index], np.sqrt(self.cov[index, index]))
+
+    def _get_joint_prior(self, indices: np.ndarray):
+        raise RuntimeError(
+            "The improper prior is a uniform distribution from -inf to inf"
+        )
+
+    def _get_joint_distribution(self, indices: np.ndarray):
+        return multivariate_normal(self.mean[indices], self.cov[indices][:, indices])
```

### Comparing `multiple-inference-1.1.0/src/multiple_inference/bayes/nonparametric.py` & `multiple-inference-1.2.0/src/multiple_inference/bayes/nonparametric.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-"""Nonparametric empirical Bayes.
-
-References:
-
-    .. code-block::
-
-        @article{cai2021nonparametric,
-            title={Nonparametric empirical bayes estimation and testing for sparse and heteroscedastic signals},
-            author={Cai, Junhui and Han, Xu and Ritov, Ya'acov and Zhao, Linda},
-            journal={arXiv preprint arXiv:2106.08881},
-            year={2021}
-        }
-
-Notes:
-
-    This implementation is based on Cai et al.'s nonparametric Dirac delta prior. Future
-    work should also implement their mixture model with a Laplace prior.
-"""
-from __future__ import annotations
-
-from itertools import product
-from typing import Any
-
-import numpy as np
-from scipy.optimize import minimize_scalar
-from scipy.stats import loguniform, norm, rv_continuous
-from sklearn.cluster import KMeans
-from sklearn.model_selection import check_cv
-from sklearn.neighbors import KernelDensity
-
-from ..stats import mixture, nonparametric
-from .base import BayesBase
-
-
-class Nonparametric(BayesBase):
-    """Bayesian model with a nonparametric Dirac delta prior.
-
-    Args:
-        num (int, optional): Number of parameters to fit for the prior. Defaults to 100.
-        n_clusters (int, optional): Number of clusters to use for featurized
-            estimation. Defaults to 1.
-        cv (int, optional): Determines the cross validation splitting strategy (input to
-            ``sklearn.model_selection.check_cv``). Defaults to 5.
-        rtol (float, optional): Relative tolerance stopping criteria for expectation
-            maximization. The EM algorithm terminates when the relative improvement
-            between iterations falls below this threshold. Defaults to .99.
-        max_iter (int, optional): Maximum number of EM iterations. Defaults to 100.
-        bandwidth_rvs_size (int, optional): Number of bandwidth values to try when
-            tuning the kernel density estimator in between EM iterations to smooth the
-            prior. Defaults to 32.
-
-    Examples:
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.bayes import Nonparametric
-
-            np.random.seed(0)
-
-            model = Nonparametric(np.arange(10), np.identity(10))
-            results = model.fit()
-            print(results.summary())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-                       Bayesian estimates
-            =======================================
-                coef pvalue (1-sided) [0.025 0.975]
-            ---------------------------------------
-            x0 0.686            0.197 -0.594  2.148
-            x1 1.226            0.062 -0.189  2.965
-            x2 1.977            0.011  0.304  3.982
-            x3 2.982            0.001  0.991  4.941
-            x4 3.990            0.000  1.960  5.892
-            x5 4.943            0.000  3.050  7.061
-            x6 6.036            0.000  3.989  8.037
-            x7 7.063            0.000  5.024  8.673
-            x8 7.768            0.000  6.089  9.123
-            x9 8.264            0.000  6.862  9.506
-            ===============
-            Dep. Variable y
-            ---------------
-    """
-
-    def __init__(
-        self,
-        *args: Any,
-        num: int = 100,
-        n_clusters: int = 1,
-        cv=5,
-        rtol: float = 0.99,
-        max_iter: int = 100,
-        bandwidth_rvs_size: int = 32,
-        **kwargs: Any,
-    ):
-        super().__init__(*args, **kwargs)
-        std = self.mean.std()
-        lower, upper = self.mean.min() - 2 * std, self.mean.max() + 2 * std
-        # (num,) array of values over which the prior is defined
-        self._values = np.linspace(lower, upper, num)
-        # (num, n_clusters) probability mass function
-        self._pmf_values = np.full((num, n_clusters), 1 / num)
-        # (# params, n_clusters) mixture weights for each parameter
-        self._mixture_weights = KMeans(n_clusters).fit_transform(self.X)
-        if (self._mixture_weights == 0).all():
-            self._mixture_weights = np.ones(self._mixture_weights.shape)
-        self._mixture_weights = (
-            self._mixture_weights.T / self._mixture_weights.sum(axis=1)
-        ).T
-
-        def loss(value, index, cluster):
-            factor = (1 - value) / (1 - self._pmf_values[index, cluster])
-            self._pmf_values[:, cluster] *= factor
-            self._pmf_values[index, cluster] = value
-            arr = self._mixture_weights * (conditional_pdf @ self._pmf_values)
-            return -np.log(arr.sum(axis=1)).sum()
-
-        # density function of the conventional estimates evaluated at self._values
-        conditional_pdf = [
-            norm.pdf(self._values, mean_i, np.sqrt(variance_i))
-            for mean_i, variance_i in zip(self.mean, self.cov.diagonal())
-        ]
-        conditional_pdf = np.array(conditional_pdf)
-        # fit the prior using an EM algorithm
-        prev_loss, current_loss, i = np.inf, None, 0
-        values = self._values.reshape(-1, 1)
-        index_cluster = list(product(np.arange(num), np.arange(n_clusters)))
-        index_cluster = np.array(index_cluster).astype(int)
-        cv = check_cv(cv)
-        cv.shuffle = True
-        for i in range(max_iter):
-            # optimize each value of ``self._pmf_values``
-            np.random.shuffle(index_cluster)
-            for index, cluster in index_cluster:
-                current_loss = minimize_scalar(
-                    loss, bounds=(0, 1), method="bounded", args=(index, cluster)
-                ).fun
-
-            # smooth the PMF using a kernel density estimator
-            cv.random_state = i
-            for cluster in range(n_clusters):
-                pmf_values = self._pmf_values[:, cluster]
-                mean = np.average(self._values, weights=pmf_values)
-                std = np.sqrt(
-                    np.average((self._values - mean) ** 2, weights=pmf_values)
-                )
-                bandwidth_rvs = loguniform(0.1 * std, 2 * std).rvs(bandwidth_rvs_size)
-                best_score = -np.inf
-                for bandwidth in bandwidth_rvs:
-                    for train_index, test_index in cv.split(values):
-                        X_train, X_test = values[train_index], values[test_index]
-                        weight_train = pmf_values[train_index]
-                        weight_test = pmf_values[test_index]
-                        weight_train /= weight_train.sum()
-                        weight_test /= weight_test.sum()
-                        kde = KernelDensity(bandwidth=bandwidth).fit(
-                            X_train, sample_weight=weight_train
-                        )
-                        score = (weight_test * kde.score_samples(X_test)).mean()
-                        if score > best_score:
-                            best_score, best_bandwidth = score, bandwidth
-
-                kde = KernelDensity(bandwidth=best_bandwidth).fit(
-                    values, sample_weight=pmf_values
-                )
-                self._pmf_values[:, cluster] = np.exp(kde.score_samples(values))
-
-            self._pmf_values /= self._pmf_values.sum(axis=0)
-            if current_loss / prev_loss > rtol:
-                break
-            prev_loss = current_loss
-
-        # fit a nonparametric distribution for each cluster
-        self._cluster_distributions = [
-            nonparametric((self._values, self._pmf_values[:, i]))
-            for i in range(n_clusters)
-        ]
-
-    def _get_marginal_prior(self, index: int) -> rv_continuous:
-        if len(self._cluster_distributions) == 1:
-            return self._cluster_distributions[0]
-
-        return mixture(self._cluster_distributions, self._mixture_weights[index])
-
-    def _get_marginal_distribution(self, index: int) -> rv_continuous:
-        pmf = (self._pmf_values * self._mixture_weights[index]).sum(axis=1)
-        logpmf = np.log(pmf) + norm.logpdf(
-            self._values, self.mean[index], np.sqrt(self.cov[index, index])
-        )
-        return nonparametric((self._values, np.exp(logpmf - logpmf.max())))
+"""Nonparametric empirical Bayes.
+
+References:
+
+    .. code-block::
+
+        @article{cai2021nonparametric,
+            title={Nonparametric empirical bayes estimation and testing for sparse and heteroscedastic signals},
+            author={Cai, Junhui and Han, Xu and Ritov, Ya'acov and Zhao, Linda},
+            journal={arXiv preprint arXiv:2106.08881},
+            year={2021}
+        }
+
+Notes:
+
+    This implementation is based on Cai et al.'s nonparametric Dirac delta prior. Future
+    work should also implement their mixture model with a Laplace prior.
+"""
+from __future__ import annotations
+
+from itertools import product
+from typing import Any
+
+import numpy as np
+from scipy.optimize import minimize_scalar
+from scipy.stats import loguniform, norm, rv_continuous
+from sklearn.cluster import KMeans
+from sklearn.model_selection import check_cv
+from sklearn.neighbors import KernelDensity
+
+from ..stats import mixture, nonparametric
+from .base import BayesBase
+
+
+class Nonparametric(BayesBase):
+    """Bayesian model with a nonparametric Dirac delta prior.
+
+    Args:
+        num (int, optional): Number of parameters to fit for the prior. Defaults to 100.
+        n_clusters (int, optional): Number of clusters to use for featurized
+            estimation. Defaults to 1.
+        cv (int, optional): Determines the cross validation splitting strategy (input to
+            ``sklearn.model_selection.check_cv``). Defaults to 5.
+        rtol (float, optional): Relative tolerance stopping criteria for expectation
+            maximization. The EM algorithm terminates when the relative improvement
+            between iterations falls below this threshold. Defaults to .99.
+        max_iter (int, optional): Maximum number of EM iterations. Defaults to 100.
+        bandwidth_rvs_size (int, optional): Number of bandwidth values to try when
+            tuning the kernel density estimator in between EM iterations to smooth the
+            prior. Defaults to 32.
+
+    Examples:
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.bayes import Nonparametric
+
+            np.random.seed(0)
+
+            model = Nonparametric(np.arange(10), np.identity(10))
+            results = model.fit()
+            print(results.summary())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+                       Bayesian estimates          
+            =======================================
+                coef pvalue (1-sided) [0.025 0.975]
+            ---------------------------------------
+            x0 0.837            0.058 -0.197  1.962
+            x1 1.200            0.017  0.080  2.968
+            x2 1.873            0.003  0.410  3.978
+            x3 3.021            0.000  0.927  4.969
+            x4 4.037            0.000  1.947  5.858
+            x5 4.938            0.000  3.148  7.077
+            x6 6.026            0.000  3.981  8.056
+            x7 7.092            0.000  5.030  8.573
+            x8 7.765            0.000  6.097  8.912
+            x9 8.171            0.000  6.942  9.193
+            ===============
+            Dep. Variable y
+            ---------------
+    """
+
+    def __init__(
+        self,
+        *args: Any,
+        num: int = 100,
+        n_clusters: int = 1,
+        cv=5,
+        rtol: float = 0.99,
+        max_iter: int = 100,
+        bandwidth_rvs_size: int = 32,
+        **kwargs: Any,
+    ):
+        super().__init__(*args, **kwargs)
+        std = self.mean.std()
+        lower, upper = self.mean.min() - 2 * std, self.mean.max() + 2 * std
+        # (num,) array of values over which the prior is defined
+        self._values = np.linspace(lower, upper, num)
+        # (num, n_clusters) probability mass function
+        self._pmf_values = np.full((num, n_clusters), 1 / num)
+        # (# params, n_clusters) mixture weights for each parameter
+        self._mixture_weights = KMeans(n_clusters).fit_transform(self.X)
+        if (self._mixture_weights == 0).all():
+            self._mixture_weights = np.ones(self._mixture_weights.shape)
+        self._mixture_weights = (
+            self._mixture_weights.T / self._mixture_weights.sum(axis=1)
+        ).T
+
+        def loss(value, index, cluster):
+            factor = (1 - value) / (1 - self._pmf_values[index, cluster])
+            self._pmf_values[:, cluster] *= factor
+            self._pmf_values[index, cluster] = value
+            arr = self._mixture_weights * (conditional_pdf @ self._pmf_values)
+            return -np.log(arr.sum(axis=1)).sum()
+
+        # density function of the conventional estimates evaluated at self._values
+        conditional_pdf = [
+            norm.pdf(self._values, mean_i, np.sqrt(variance_i))
+            for mean_i, variance_i in zip(self.mean, self.cov.diagonal())
+        ]
+        conditional_pdf = np.array(conditional_pdf)
+        # fit the prior using an EM algorithm
+        prev_loss, current_loss, i = np.inf, None, 0
+        values = self._values.reshape(-1, 1)
+        index_cluster = list(product(np.arange(num), np.arange(n_clusters)))
+        index_cluster = np.array(index_cluster).astype(int)
+        cv = check_cv(cv)
+        cv.shuffle = True
+        for i in range(max_iter):
+            # optimize each value of ``self._pmf_values``
+            np.random.shuffle(index_cluster)
+            for index, cluster in index_cluster:
+                current_loss = minimize_scalar(
+                    loss, bounds=(0, 1), method="bounded", args=(index, cluster)
+                ).fun
+
+            # smooth the PMF using a kernel density estimator
+            cv.random_state = i
+            for cluster in range(n_clusters):
+                pmf_values = self._pmf_values[:, cluster]
+                mean = np.average(self._values, weights=pmf_values)
+                std = np.sqrt(
+                    np.average((self._values - mean) ** 2, weights=pmf_values)
+                )
+                bandwidth_rvs = loguniform(0.1 * std, 2 * std).rvs(bandwidth_rvs_size)
+                best_score = -np.inf
+                for bandwidth in bandwidth_rvs:
+                    for train_index, test_index in cv.split(values):
+                        X_train, X_test = values[train_index], values[test_index]
+                        weight_train = pmf_values[train_index]
+                        weight_test = pmf_values[test_index]
+                        weight_train /= weight_train.sum()
+                        weight_test /= weight_test.sum()
+                        kde = KernelDensity(bandwidth=bandwidth).fit(
+                            X_train, sample_weight=weight_train
+                        )
+                        score = (weight_test * kde.score_samples(X_test)).mean()
+                        if score > best_score:
+                            best_score, best_bandwidth = score, bandwidth
+
+                kde = KernelDensity(bandwidth=best_bandwidth).fit(
+                    values, sample_weight=pmf_values
+                )
+                self._pmf_values[:, cluster] = np.exp(kde.score_samples(values))
+
+            self._pmf_values /= self._pmf_values.sum(axis=0)
+            if current_loss / prev_loss > rtol:
+                break
+            prev_loss = current_loss
+
+        # fit a nonparametric distribution for each cluster
+        self._cluster_distributions = [
+            nonparametric((self._values, self._pmf_values[:, i]))
+            for i in range(n_clusters)
+        ]
+
+    def _get_marginal_prior(self, index: int) -> rv_continuous:
+        if len(self._cluster_distributions) == 1:
+            return self._cluster_distributions[0]
+
+        return mixture(self._cluster_distributions, self._mixture_weights[index])
+
+    def _get_marginal_distribution(self, index: int) -> rv_continuous:
+        pmf = (self._pmf_values * self._mixture_weights[index]).sum(axis=1)
+        logpmf = np.log(pmf) + norm.logpdf(
+            self._values, self.mean[index], np.sqrt(self.cov[index, index])
+        )
+        return nonparametric((self._values, np.exp(logpmf - logpmf.max())))
```

### Comparing `multiple-inference-1.1.0/src/multiple_inference/bayes/normal.py` & `multiple-inference-1.2.0/src/multiple_inference/bayes/normal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,695 +1,694 @@
-"""Empirical Bayes with a normal prior.
-
-References:
-
-    .. code-block::
-
-        @inproceedings{stein1956inadmissibility,
-            title={Inadmissibility of the usual estimator for the mean of a multivariate normal distribution},
-            author={Stein, Charles and others},
-            booktitle={Proceedings of the Third Berkeley symposium on mathematical statistics and probability},
-            volume={1},
-            number={1},
-            pages={197--206},
-            year={1956}
-        }
-
-        @incollection{james1992estimation,
-            title={Estimation with quadratic loss},
-            author={James, William and Stein, Charles},
-            booktitle={Breakthroughs in statistics},
-            pages={443--460},
-            year={1992},
-            publisher={Springer}
-        }
-
-        @article{bock1975minimax,
-            title={Minimax estimators of the mean of a multivariate normal distribution},
-            author={Bock, Mary Ellen},
-            journal={The Annals of Statistics},
-            pages={209--218},
-            year={1975},
-            publisher={JSTOR}
-        }
-
-        @inproceedings{dimmery2019shrinkage,
-            title={Shrinkage estimators in online experiments},
-            author={Dimmery, Drew and Bakshy, Eytan and Sekhon, Jasjeet},
-            booktitle={Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery \& Data Mining},
-            pages={2914--2922},
-            year={2019}
-        }
-
-        @article{armstrong2020robust,
-            title={Robust empirical bayes confidence intervals},
-            author={Armstrong, Timothy B and Koles{\'a}r, Michal and Plagborg-M{\o}ller, Mikkel},
-            journal={arXiv preprint arXiv:2004.03448},
-            year={2020}
-        }
-
-Notes:
-
-    The James-Stein method of fitting the normal prior relies on my own fully Bayesian
-    derivation that extends Dimmery et al. (2019)'s derivation by 1) accounting for correlated
-    errors and 2) allowing the prior mean vector to depend on a feature matrix ``X``.
-"""
-from __future__ import annotations
-
-import math
-import warnings
-from typing import Any, Callable, Union
-
-import numpy as np
-from scipy.optimize import minimize_scalar, root_scalar
-from scipy.stats import multivariate_normal, ncx2, norm, rv_continuous
-
-from multiple_inference.base import ColumnsType
-from multiple_inference.bayes.base import BayesBase, BayesResults
-
-
-def compute_robust_critical_value(
-    m2: float, kurtosis: float = np.inf, alpha: float = 0.05
-) -> tuple[float, np.ndarray, np.ndarray]:
-    """Compute the critical value for robust confidence intervals.
-
-    Args:
-        m2 (float): Equality constraint on :math:`E[b^2]`.
-        kurtosis (float, optional): Estimated kurtosis of the prior distribution.
-            Defaults to np.inf.
-        alpha (float, optional): Significance level. Defaults to .05.
-
-    Returns:
-        tuple[float, np.ndarray, np.ndarray]: Critical value, array of :math:`x` values
-        for the least favorable mass function, array of probabilities for the least
-        favorable mass function.
-
-    Notes:
-
-        See Armstrong et al., 2020 for mathematical details. This function is equivalent
-        to the ``cva`` function in the
-        `ebci R package <https://cran.r-project.org/web/packages/ebci/index.html>`_ and
-        uses the same variable names and tolerance thresholds.
-    """
-
-    def rho0(chi):
-        t0 = rt0(chi)[0]
-        return r(m2, chi) if m2 >= t0 else r(t0, chi) + (m2 - t0) * r1(t0, chi)
-
-    def rt0(chi):
-        # returns t0, inflection point
-        # the inflection point is denoted t1 in the paper
-        if (chi_sq := chi ** 2) < 3:
-            return 0, 0
-
-        if abs(r2(inflection := chi_sq - 1.5, chi=chi)) > tol:
-            inflection = root_scalar(
-                lambda x: r2(x, chi=chi), bracket=(chi_sq - 3, chi_sq), method="brentq"
-            ).root
-
-        func = lambda t: r(t, chi) - t * r1(t, chi) - r(0, chi)
-        lower, upper = inflection, 2 * chi_sq
-        t0 = (
-            root_scalar(lambda x: func(x), bracket=(lower, upper), method="brentq").root
-            if func(lower) < 0
-            else lower
-        )
-        return t0, inflection
-
-    def r(t, chi):
-        # called r0 in the paper
-        sqrt_t = np.sqrt(t)
-        return (
-            (norm.cdf(-sqrt_t - chi) + norm.cdf(sqrt_t - chi))
-            if sqrt_t - chi < 5
-            else 1
-        )
-
-    def r1(t, chi):
-        # first derivative of r
-        sqrt_t = np.sqrt(t)
-        if t < 1e-8:
-            # apply L'Hopital's rule
-            return chi * norm.pdf(chi)
-        return (norm.pdf(sqrt_t - chi) - norm.pdf(sqrt_t + chi)) / (2 * sqrt_t)
-
-    def r2(t, chi):
-        # second derivative of r
-        sqrt_t = np.sqrt(t)
-        if t < 2e-6:
-            # apply L'Hopital's rule
-            return chi * (chi ** 2 - 3) * norm.pdf(chi) / 6
-        coef0 = chi * sqrt_t
-        coef1 = t + 1
-        return (
-            (coef0 + coef1) * norm.pdf(sqrt_t + chi)
-            + (coef0 - coef1) * norm.pdf(sqrt_t - chi)
-        ) / (4 * t ** 1.5)
-
-    def r3(t, chi):
-        # third derivative of r
-        sqrt_t = np.sqrt(t)
-        if t < 2e-4:
-            # apply L'Hopital's rule
-            return (chi ** 5 - 10 * chi ** 3 + 15 * chi) * norm.pdf(chi) / 60
-        coef0 = t ** 2 + (2 + chi ** 2) * t + 3
-        coef1 = 2 * chi * t ** 1.5 + 3 * chi * sqrt_t
-        return (
-            (coef0 - coef1) * norm.pdf(chi - sqrt_t)
-            - (coef0 + coef1) * norm.pdf(chi + sqrt_t)
-        ) / (8 * t ** 2.5)
-
-    def rho(chi):
-        # return (optimum loss, x values for pmf, probabilities for pmf)
-        if kurtosis == 1:
-            return r(m2, chi), np.array([0, m2]), np.array([0, 1])
-
-        r0, t0 = rho0(chi), rt0(chi)[0]
-        if m2 >= t0:
-            return r0, np.array([0, m2]), np.array([0, 1])
-
-        if kurtosis == np.inf or m2 * kurtosis >= t0:
-            return r0, np.array([0, t0]), np.array([1 - m2 / t0, m2 / t0])
-
-        tbar = lam(0, chi)[1]
-        lammax = lambda x0: delta(0, x0, chi) if x0 >= tbar else max(lam(x0, chi)[0], 0)
-        loss = (
-            lambda x0: r(x0, chi)
-            + (m2 - x0) * r1(x0, chi)
-            + (kurtosis * m2 ** 2 - 2 * x0 * m2 + x0 ** 2) * lammax(x0)
-        )
-        result_above = minimize_scalar(loss, bounds=(tbar, t0), method="bounded")
-        if tbar > 0:
-            result_below = minimize_scalar(loss, bounds=(0, tbar), method="bounded")
-            minimum_below, fun_below = result_below.x, result_below.fun
-        else:
-            minimum_below, fun_below = 0, loss(0)
-        minimum, fun = (
-            (result_above.x, result_above.fun)
-            if result_above.fun < fun_below
-            else (minimum_below, fun_below)
-        )
-
-        values = np.sort([minimum, lam(minimum, chi)[1]])
-        probability = (m2 - values[1]) / (values[0] - values[1])
-        return fun, values, np.array([probability, 1 - probability])
-
-    def lam(x0, chi):
-        # returns delta(x*, x0, chi), x*
-        # where x* = argmax_x(delta(x, x0, chi))
-        # check 0, inflection point, t0, and x0
-        x = np.sort(rt0(chi))
-        x = np.array([0, x[0]]) if x0 >= x[0] else np.unique([0, x0, *x])
-        derivatives = delta1(x, x0, chi)
-        values = delta(x, x0, chi)
-        optimum = values[0], 0
-        if (derivatives <= 0).all() and values.argmax() == 0:
-            return optimum
-
-        if (np.diff(derivatives >= 0) >= 0).all() and derivatives[-1] <= 0:
-            index = max((derivatives >= 0).argmin(), 1)
-            bounds = x[index - 1], x[index]
-        elif abs(derivatives).min() < 1e-6:
-            argmax = values.argmax()
-            bounds = x[max(argmax - 1, 0)], x[min(argmax + 1, len(values) - 1)]
-        else:
-            raise RuntimeError(
-                f"There are multiple optima in the function delta(x, x0={x0}, chi={chi})."
-            )
-
-        result = minimize_scalar(
-            lambda x: -delta(x, x0, chi), bounds=bounds, method="bounded"
-        )
-        return (-result.fun, result.x) if -result.fun > optimum[0] else optimum
-
-    def delta(x, x0, chi):
-        def func(x):
-            return (
-                0.5 * r2(x0, chi)  # apply L'Hopital's rule
-                if abs(x - x0) < 1e-4
-                else (r(x, chi) - r(x0, chi) - (x - x0) * r1(x0, chi)) / (x - x0) ** 2
-            )
-
-        return func(x) if np.isscalar(x) else np.array([func(x_i) for x_i in x])
-
-    def delta1(x, x0, chi):
-        # first derivative of delta
-        def func(x):
-            if abs(x - x0) < 1e-3:
-                # apply L'Hoptial's rule
-                return r3(x0, chi)
-            return (
-                r1(x, chi) + r1(x0, chi) - 2 * (r(x, chi) - r(x0, chi)) / (x - x0)
-            ) / (x - x0) ** 2
-
-        return func(x) if np.isscalar(x) else np.array([func(x_i) for x_i in x])
-
-    tol = 1e-12
-    critical_value_b = (
-        np.sqrt(ncx2.ppf(1 - alpha, nc=m2, df=1))
-        if m2 < 100
-        else norm.ppf(1 - alpha, np.sqrt(m2))
-    )
-    if m2 == 0 or kurtosis == 1:
-        return critical_value_b, np.array([0, m2]), np.array([0, 1])
-
-    if m2 > 1 / tol and kurtosis != np.inf:
-        kurtosis = np.inf
-
-    # get bounds for when kappa == 1 and kappa == infinity
-    lower, upper = critical_value_b - 0.01, np.sqrt((m2 + 1) / alpha)
-    if abs(rho0(upper) - alpha) > 9e-6:
-        upper = root_scalar(
-            lambda chi: rho0(chi) - alpha, bracket=(lower, upper), method="brentq"
-        ).root
-
-    if rho(upper)[0] - alpha < -1e-5:
-        critical_value = root_scalar(
-            lambda chi: rho(chi)[0] - alpha, bracket=(lower, upper), method="brentq"
-        ).root
-    else:
-        critical_value = upper
-    return critical_value, *rho(critical_value)[1:]
-
-
-class NormalResults(BayesResults):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        # estimate constraints and kurtosis for computing robust confidence intervals
-        # constraints are denoted "m2" in Armstrong et al., 2020
-        self._robust_conf_int_constraints = (
-            self.model.cov.diagonal() / self.model.prior_cov.diagonal()
-        )
-        cov_inv = np.linalg.inv(self.model.cov)
-        weights = (
-            np.linalg.inv(self.model.X.T @ cov_inv @ self.model.X)
-            @ self.model.X.T
-            @ cov_inv
-        )
-        error = self.model.mean - self.model.prior_mean
-        cov_diag = self.model.cov.diagonal()
-        prior_cov_diag = self.model.prior_cov.diagonal()
-        kurtosis0 = (
-            weights * (error ** 4 - 6 * cov_diag * error ** 2 + 3 * cov_diag ** 2)
-        ).sum() / (weights * prior_cov_diag ** 2).sum()
-        kurtosis1 = (
-            1
-            + 32
-            * (weights ** 2 * cov_diag ** 4).sum()
-            / (weights * (prior_cov_diag ** 2 + cov_diag ** 2)).sum()
-        )
-        self._kurtosis = max(kurtosis0, kurtosis1)
-
-    def conf_int(
-        self,
-        alpha: float = 0.05,
-        columns: ColumnsType = None,
-        robust: bool = False,
-        fast: bool = False,
-        **kwargs: Any,
-    ) -> np.ndarray:
-        """Compute the 1-alpha confidence interval.
-
-        Args:
-            alpha (float, optional): Significance level. Defaults to .05.
-            columns (ColumnsType, optional): Selected columns. Defaults to None.
-            robust (bool, optional): Use robust confidence intervals. These will have
-                correct average coverage even if the normal prior assumption is
-                violated. Defaults to False.
-            fast (bool, optional): Use a "fast" computation method for the robust
-                confidence intervals. This assumes the critical value is the same for
-                all parameters. Defaults to False.
-
-        Returns:
-            np.ndarray: (# params, 2) array of confidence intervals.
-        """
-        if not robust:
-            return super().conf_int(alpha, columns, **kwargs)
-
-        indices = self.model.get_indices(columns)
-        constraints = self._robust_conf_int_constraints[indices]
-        if fast or np.isclose(constraints, constraints[0]).all():
-            constraint = constraints.mean()
-            critical_values = np.full(
-                len(constraints),
-                [compute_robust_critical_value(constraint, self._kurtosis, alpha)[0]],
-            )
-        else:
-            critical_values = np.array(
-                [
-                    compute_robust_critical_value(x, self._kurtosis, alpha)[0]
-                    for x in constraints
-                ]
-            )
-        len_conf_int = critical_values * np.sqrt(
-            self.model.posterior_cov.diagonal()[indices]
-        )
-        params = self.params[indices]
-        return np.array([params - len_conf_int, params + len_conf_int]).T
-
-
-class Normal(BayesBase):
-    """Bayesian model with a normal prior.
-
-    Args:
-        fit_method (Union[str, Callable[[], None]], optional): Specifies how to fit the
-            prior ("mle", "bock", or "james_stein"). You can also use a custom function
-            that sets the ``prior_mean``, ``prior_cov``, ``posterior_mean`` and
-            ``posterior_cov`` attributes. Defaults to "mle".
-        prior_mean (Union[float, np.ndarray], optional): (# params,) prior mean vector.
-            Defaults to None.
-        prior_cov (Union[float, np.ndarray], optional): (# params, # params) prior
-            covariance matrix. Defaults to None.
-
-    Examples:
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.bayes import Normal
-
-            model = Normal(np.arange(10), np.identity(10))
-            results = model.fit()
-            print(results.summary())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-                       Bayesian estimates
-            =======================================
-                coef pvalue (1-sided) [0.025 0.975]
-            ---------------------------------------
-            x0 0.545            0.282 -1.305  2.395
-            x1 1.424            0.066 -0.426  3.274
-            x2 2.303            0.007  0.453  4.153
-            x3 3.182            0.000  1.332  5.032
-            x4 4.061            0.000  2.211  5.911
-            x5 4.939            0.000  3.089  6.789
-            x6 5.818            0.000  3.968  7.668
-            x7 6.697            0.000  4.847  8.547
-            x8 7.576            0.000  5.726  9.426
-            x9 8.455            0.000  6.605 10.305
-            ===============
-            Dep. Variable y
-            ---------------
-    """
-
-    _results_cls = NormalResults
-
-    def __init__(
-        self,
-        *args: Any,
-        fit_method: Union[str, Callable[[], None]] = "mle",
-        prior_mean: Union[float, np.ndarray] = None,
-        prior_cov: Union[float, np.ndarray] = None,
-        **kwargs: Any,
-    ):
-
-        super().__init__(*args, **kwargs)
-        self.prior_mean, self.prior_cov = prior_mean, prior_cov
-        if np.isscalar(prior_mean):
-            self.prior_mean = np.full(self.n_params, prior_mean)
-        if np.isscalar(prior_cov):
-            self.prior_cov = prior_cov * np.identity(self.n_params)
-
-        self.posterior_mean, self.posterior_cov = None, None
-        if callable(fit_method):
-            fit_method()
-            self._set_posterior_estimates()
-        else:
-            fit_methods = {
-                "mle": self._fit_mle,
-                "james_stein": self._fit_james_stein,
-                "bock": self._fit_bock,
-            }
-            if fit_method not in fit_methods:
-                raise ValueError(
-                    f"`fit_method` must be one of {fit_methods.keys()}, got {fit_method}."
-                )
-            fit_methods[fit_method]()
-
-    def _fit_mle(self, max_iter: int = 100, rtol: float = 0.99) -> None:
-        """Fit the model using maximum likelihood estimation.
-
-        Args:
-            max_iter (int, optional): Maximum number of EM iterations. Defaults to 100.
-            rtol (float, optional): Stopping criterion for EM. Defaults to .99.
-        """
-
-        def neg_log_likelihood(prior_std):
-            # negative log likelihood as a function of the prior standard deviation
-            marginal_cov = prior_std ** 2 * np.identity(self.n_params) + self.cov
-            # note: the prior mean is also the marginal mean
-            return -multivariate_normal.logpdf(self.mean, prior_mean, marginal_cov)
-
-        # use EM to iteratively update the prior mean and covariance
-        prior_cov = (
-            np.zeros(self.cov.shape) if self.prior_cov is None else self.prior_cov
-        )
-        current_log_likelihood, prev_log_likelihood = None, -np.inf
-        for _ in range(max_iter):
-            # update prior mean
-            if self.prior_mean is not None:
-                prior_mean = self.prior_mean
-            else:
-                marginal_cov_inv = np.linalg.inv(self.cov + prior_cov)
-                prior_mean = (
-                    self.X
-                    @ np.linalg.inv(self.X.T @ marginal_cov_inv @ self.X)
-                    @ self.X.T
-                    @ marginal_cov_inv
-                    @ self.mean
-                )
-
-            # update prior cov
-            if self.prior_cov is not None:
-                prior_cov = self.prior_cov
-                break  # prior_mean is computed analytically, so no need to iterate futher
-            else:
-                result = minimize_scalar(
-                    neg_log_likelihood, bounds=(0, self.mean.std()), method="bounded"
-                )
-                prior_cov = result.x ** 2 * np.identity(self.n_params)
-                current_log_likelihood = -result.fun
-
-            if current_log_likelihood / prev_log_likelihood > rtol:
-                break
-            prev_log_likelihood = current_log_likelihood
-
-        # set the posterior mean and covariance estimates
-        # and adjust the prior and posterior covariances to account for uncertainty in the MLE estimate of the prior mean
-        prior_uncertainty = post_uncertainty = 0
-        if self.prior_mean is None:
-            marginal_cov_inv = np.linalg.inv(prior_cov + self.cov)
-            prior_uncertainty = (
-                self.X @ np.linalg.inv(self.X.T @ marginal_cov_inv @ self.X) @ self.X.T
-            )
-            xi = self.cov @ marginal_cov_inv
-            post_uncertainty = xi @ prior_uncertainty @ xi
-
-        self.prior_mean, self.prior_cov = prior_mean, prior_cov
-        self._set_posterior_estimates()  # note: set the posterior estimates *before* adjusting the prior covariance
-        self.prior_cov += prior_uncertainty
-        self.posterior_cov += post_uncertainty
-
-    def _fit_bock(self, max_iter: int = 100, rtol: float = 0.99) -> None:
-        """Fit the model using Bock (1975)'s multivariate Stein-type estimator.
-
-        Args:
-            max_iter (int, optional): Maximum number of iterations. Defaults to 100.
-            rtol (float, optional): Stopping criteria. Defaults to .99.
-
-        Raises:
-            RuntimeError: The shrinkage factor must be positve.
-        """
-        cov_inv = np.linalg.inv(self.cov)
-        prior_mean_df = self.X.shape[1] if self.prior_mean is None else 0
-        effective_dimension = np.trace(self.cov) / np.linalg.eig(self.cov)[0].max()
-        if effective_dimension - prior_mean_df - 2 < 0:
-            raise RuntimeError(
-                "Failed to fit the Bock (1975) estimator because the effective dimension"
-                " of the covariance matrix is too small. Try another fit method like"
-                " 'mle'."
-            )
-
-        xi = (
-            np.identity(self.n_params)
-            if self.prior_cov is None
-            else self.cov @ np.linalg.inv(self.cov + self.prior_cov)
-        )
-        current_log_likelihood, prev_log_likelihood = None, -np.inf
-        for _ in range(max_iter):
-            if self.prior_mean is None:
-                # update prior mean
-                marginal_cov_inv = cov_inv @ xi
-                prior_mean = (
-                    self.X
-                    @ np.linalg.inv(self.X.T @ marginal_cov_inv @ self.X)
-                    @ self.X.T
-                    @ marginal_cov_inv
-                    @ self.mean
-                )
-            else:
-                prior_mean = self.prior_mean
-
-            if self.prior_cov is None:
-                # update prior covariance
-                error = self.mean - prior_mean
-                param = min(
-                    (effective_dimension - prior_mean_df - 2)
-                    / (error.T @ cov_inv @ error),
-                    1,
-                )
-                xi = param * np.identity(self.n_params)
-            else:
-                prior_cov = self.prior_cov
-                # prior mean is computed analytically, so no need to iterate
-                break
-
-            # check for convergence
-            marginal_cov = np.linalg.inv(xi) @ self.cov
-            prior_cov = marginal_cov - self.cov
-            current_log_likelihood = multivariate_normal.logpdf(
-                self.mean, prior_mean, marginal_cov
-            )
-            if current_log_likelihood / prev_log_likelihood > rtol:
-                break
-            prev_log_likelihood = current_log_likelihood
-
-        # set the posterior mean and covariance estimates
-        # and adjust the prior and posterior covariances to account for uncertainty in the MLE estimate of the prior mean
-        prior_uncertainty = post_uncertainty = 0
-        if self.prior_mean is None:
-            marginal_cov_inv = np.linalg.inv(prior_cov + self.cov)
-            prior_uncertainty = (
-                self.X @ np.linalg.inv(self.X.T @ marginal_cov_inv @ self.X) @ self.X.T
-            )
-            xi = self.cov @ marginal_cov_inv
-            post_uncertainty = xi @ prior_uncertainty @ xi
-
-        self.prior_mean, self.prior_cov = prior_mean, prior_cov
-        self._set_posterior_estimates()  # note: set the posterior estimates *before* adjusting the prior covariance
-        self.prior_cov += prior_uncertainty
-        self.posterior_cov += post_uncertainty
-
-    def _set_posterior_estimates(self):
-        """Sets the posterior mean and covariance using plugin estimates from the prior
-        mean and covariance if the posterior parameters haven't already been set.
-        """
-        xi = self.cov @ np.linalg.inv(self.prior_cov + self.cov)
-        if self.posterior_mean is None:
-            self.posterior_mean = self.prior_mean + (
-                np.identity(self.n_params) - xi
-            ) @ (self.mean - self.prior_mean)
-
-        if self.posterior_cov is None:
-            self.posterior_cov = (np.identity(self.n_params) - xi) @ self.cov
-
-    def _fit_james_stein(self, max_iter: int = 100, tol: float = 1e-6) -> None:
-        """Fit the model using James-Stein estimates.
-
-        Args:
-            max_iter (int, optional): Maximum number of iterations to find the
-                positive-part prior covariance.. Defaults to 100.
-            tol (float, optional): Stopping criteria for finding the positive-part prior
-                covariance. Defaults to 1e-6.
-        """
-        if self.prior_mean is None:
-            prior_mean = (
-                self.X @ np.linalg.inv(self.X.T @ self.X) @ self.X.T @ self.mean
-            )
-            prior_mean_df = self.X.shape[1]
-        else:
-            prior_mean = self.prior_mean
-            prior_mean_df = 0
-
-        s_squared = ((self.mean - prior_mean) ** 2).sum()
-        try:
-            np.linalg.cholesky(
-                s_squared
-                / (self.n_params - prior_mean_df - 2)
-                * np.identity(self.n_params)
-                - self.cov
-            )
-        except np.linalg.LinAlgError:
-            # find minimum s_squared such that the (unadjusted) prior covariance is positive semidefinite
-            warnings.warn(
-                "The James-Stein prior covariance estimate is not positive semidefinite."
-                " Using the positive-part James-Stein covariance estimate instead."
-                " This may result in too little shrinkage."
-            )
-            bounds = [np.sqrt(s_squared), np.inf]
-            for _ in range(max_iter):
-                s_squared = (
-                    2 * bounds[0] if bounds[1] == np.inf else sum(bounds) / 2
-                ) ** 2
-                try:
-                    np.linalg.cholesky(
-                        s_squared
-                        / (self.n_params - prior_mean_df - 2)
-                        * np.identity(self.n_params)
-                        - self.cov
-                    )
-                    bounds[1] = np.sqrt(s_squared)
-                except:
-                    bounds[0] = np.sqrt(s_squared)
-                if bounds[1] - bounds[0] < tol:
-                    break
-            s_squared = bounds[1] ** 2
-
-        # compute the prior covariance
-        param = s_squared / (self.n_params - prior_mean_df - 4)
-        self.prior_cov = (
-            param * np.identity(self.n_params)
-            - self.cov
-            + param * self.X @ np.linalg.inv(self.X.T @ self.X) @ self.X.T
-        )
-
-        # compute the posterior mean
-        xi = self.cov * (self.n_params - prior_mean_df - 2) / s_squared
-        self.posterior_mean = prior_mean + (np.identity(self.n_params) - xi) @ (
-            self.mean - prior_mean
-        )
-
-        # compute the posterior covariance
-        plugin_posterior_cov = (np.identity(self.n_params) - xi) @ self.cov
-        if self.prior_mean is None:
-            prior_mean_uncertainty = (
-                self.cov @ self.X @ np.linalg.inv(self.X.T @ self.X) @ self.X.T @ xi
-            )
-        else:
-            prior_mean_uncertainty = 0
-        prior_cov_uncertainty = (
-            2
-            / (self.n_params - self.X.shape[1] - 2)
-            * xi
-            @ (self.mean - prior_mean).reshape(-1, 1)
-            @ (self.mean - prior_mean).reshape(1, -1)
-            @ xi
-        )
-        self.posterior_cov = (
-            plugin_posterior_cov + prior_mean_uncertainty + prior_cov_uncertainty
-        )
-
-        self.prior_mean = prior_mean
-
-    def _get_marginal_prior(self, index: int) -> rv_continuous:
-        return norm(self.prior_mean[index], np.sqrt(self.prior_cov[index, index]))
-
-    def _get_marginal_distribution(self, index: int) -> rv_continuous:
-        return norm(
-            self.posterior_mean[index], np.sqrt(self.posterior_cov[index, index])
-        )
-
-    def _get_joint_prior(self, indices: np.ndarray):
-        return multivariate_normal(
-            self.prior_mean[indices],
-            self.prior_cov[indices][:, indices],
-            allow_singular=True,
-        )
-
-    def _get_joint_distribution(self, indices: np.ndarray):
-        return multivariate_normal(
-            self.posterior_mean[indices],
-            self.posterior_cov[indices][:, indices],
-            allow_singular=True,
-        )
+"""Empirical Bayes with a normal prior.
+
+References:
+
+    .. code-block::
+
+        @inproceedings{stein1956inadmissibility,
+            title={Inadmissibility of the usual estimator for the mean of a multivariate normal distribution},
+            author={Stein, Charles and others},
+            booktitle={Proceedings of the Third Berkeley symposium on mathematical statistics and probability},
+            volume={1},
+            number={1},
+            pages={197--206},
+            year={1956}
+        }
+
+        @incollection{james1992estimation,
+            title={Estimation with quadratic loss},
+            author={James, William and Stein, Charles},
+            booktitle={Breakthroughs in statistics},
+            pages={443--460},
+            year={1992},
+            publisher={Springer}
+        }
+
+        @article{bock1975minimax,
+            title={Minimax estimators of the mean of a multivariate normal distribution},
+            author={Bock, Mary Ellen},
+            journal={The Annals of Statistics},
+            pages={209--218},
+            year={1975},
+            publisher={JSTOR}
+        }
+
+        @inproceedings{dimmery2019shrinkage,
+            title={Shrinkage estimators in online experiments},
+            author={Dimmery, Drew and Bakshy, Eytan and Sekhon, Jasjeet},
+            booktitle={Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery \& Data Mining},
+            pages={2914--2922},
+            year={2019}
+        }
+
+        @article{armstrong2020robust,
+            title={Robust empirical bayes confidence intervals},
+            author={Armstrong, Timothy B and Koles{\'a}r, Michal and Plagborg-M{\o}ller, Mikkel},
+            journal={arXiv preprint arXiv:2004.03448},
+            year={2020}
+        }
+
+Notes:
+
+    The James-Stein method of fitting the normal prior relies on my own fully Bayesian
+    derivation that extends Dimmery et al. (2019)'s derivation by 1) accounting for correlated
+    errors and 2) allowing the prior mean vector to depend on a feature matrix ``X``.
+"""
+from __future__ import annotations
+
+import math
+import warnings
+from typing import Any, Callable, Union
+
+import numpy as np
+from scipy.optimize import minimize_scalar, root_scalar
+from scipy.stats import multivariate_normal, ncx2, norm, rv_continuous
+
+from multiple_inference.base import ColumnsType
+from multiple_inference.bayes.base import BayesBase, BayesResults
+
+
+def compute_robust_critical_value(
+    m2: float, kurtosis: float = np.inf, alpha: float = 0.05
+) -> tuple[float, np.ndarray, np.ndarray]:
+    """Compute the critical value for robust confidence intervals.
+
+    Args:
+        m2 (float): Equality constraint on :math:`E[b^2]`.
+        kurtosis (float, optional): Estimated kurtosis of the prior distribution.
+            Defaults to np.inf.
+        alpha (float, optional): Significance level. Defaults to .05.
+
+    Returns:
+        tuple[float, np.ndarray, np.ndarray]: Critical value, array of :math:`x` values
+        for the least favorable mass function, array of probabilities for the least
+        favorable mass function.
+
+    Notes:
+
+        See Armstrong et al., 2020 for mathematical details. This function is equivalent
+        to the ``cva`` function in the
+        `ebci R package <https://cran.r-project.org/web/packages/ebci/index.html>`_ and
+        uses the same variable names and tolerance thresholds.
+    """
+
+    def rho0(chi):
+        t0 = rt0(chi)[0]
+        return r(m2, chi) if m2 >= t0 else r(t0, chi) + (m2 - t0) * r1(t0, chi)
+
+    def rt0(chi):
+        # returns t0, inflection point
+        # the inflection point is denoted t1 in the paper
+        if (chi_sq := chi**2) < 3:
+            return 0, 0
+
+        if abs(r2(inflection := chi_sq - 1.5, chi=chi)) > tol:
+            inflection = root_scalar(
+                lambda x: r2(x, chi=chi), bracket=(chi_sq - 3, chi_sq), method="brentq"
+            ).root
+
+        func = lambda t: r(t, chi) - t * r1(t, chi) - r(0, chi)
+        lower, upper = inflection, 2 * chi_sq
+        t0 = (
+            root_scalar(lambda x: func(x), bracket=(lower, upper), method="brentq").root
+            if func(lower) < 0
+            else lower
+        )
+        return t0, inflection
+
+    def r(t, chi):
+        # called r0 in the paper
+        sqrt_t = np.sqrt(t)
+        return (
+            (norm.cdf(-sqrt_t - chi) + norm.cdf(sqrt_t - chi))
+            if sqrt_t - chi < 5
+            else 1
+        )
+
+    def r1(t, chi):
+        # first derivative of r
+        sqrt_t = np.sqrt(t)
+        if t < 1e-8:
+            # apply L'Hopital's rule
+            return chi * norm.pdf(chi)
+        return (norm.pdf(sqrt_t - chi) - norm.pdf(sqrt_t + chi)) / (2 * sqrt_t)
+
+    def r2(t, chi):
+        # second derivative of r
+        sqrt_t = np.sqrt(t)
+        if t < 2e-6:
+            # apply L'Hopital's rule
+            return chi * (chi**2 - 3) * norm.pdf(chi) / 6
+        coef0 = chi * sqrt_t
+        coef1 = t + 1
+        return (
+            (coef0 + coef1) * norm.pdf(sqrt_t + chi)
+            + (coef0 - coef1) * norm.pdf(sqrt_t - chi)
+        ) / (4 * t**1.5)
+
+    def r3(t, chi):
+        # third derivative of r
+        sqrt_t = np.sqrt(t)
+        if t < 2e-4:
+            # apply L'Hopital's rule
+            return (chi**5 - 10 * chi**3 + 15 * chi) * norm.pdf(chi) / 60
+        coef0 = t**2 + (2 + chi**2) * t + 3
+        coef1 = 2 * chi * t**1.5 + 3 * chi * sqrt_t
+        return (
+            (coef0 - coef1) * norm.pdf(chi - sqrt_t)
+            - (coef0 + coef1) * norm.pdf(chi + sqrt_t)
+        ) / (8 * t**2.5)
+
+    def rho(chi):
+        # return (optimum loss, x values for pmf, probabilities for pmf)
+        if kurtosis == 1:
+            return r(m2, chi), np.array([0, m2]), np.array([0, 1])
+
+        r0, t0 = rho0(chi), rt0(chi)[0]
+        if m2 >= t0:
+            return r0, np.array([0, m2]), np.array([0, 1])
+
+        if kurtosis == np.inf or m2 * kurtosis >= t0:
+            return r0, np.array([0, t0]), np.array([1 - m2 / t0, m2 / t0])
+
+        tbar = lam(0, chi)[1]
+        lammax = lambda x0: delta(0, x0, chi) if x0 >= tbar else max(lam(x0, chi)[0], 0)
+        loss = (
+            lambda x0: r(x0, chi)
+            + (m2 - x0) * r1(x0, chi)
+            + (kurtosis * m2**2 - 2 * x0 * m2 + x0**2) * lammax(x0)
+        )
+        result_above = minimize_scalar(loss, bounds=(tbar, t0), method="bounded")
+        if tbar > 0:
+            result_below = minimize_scalar(loss, bounds=(0, tbar), method="bounded")
+            minimum_below, fun_below = result_below.x, result_below.fun
+        else:
+            minimum_below, fun_below = 0, loss(0)
+        minimum, fun = (
+            (result_above.x, result_above.fun)
+            if result_above.fun < fun_below
+            else (minimum_below, fun_below)
+        )
+
+        values = np.sort([minimum, lam(minimum, chi)[1]])
+        probability = (m2 - values[1]) / (values[0] - values[1])
+        return fun, values, np.array([probability, 1 - probability])
+
+    def lam(x0, chi):
+        # returns delta(x*, x0, chi), x*
+        # where x* = argmax_x(delta(x, x0, chi))
+        # check 0, inflection point, t0, and x0
+        x = np.sort(rt0(chi))
+        x = np.array([0, x[0]]) if x0 >= x[0] else np.unique([0, x0, *x])
+        derivatives = delta1(x, x0, chi)
+        values = delta(x, x0, chi)
+        optimum = values[0], 0
+        if (derivatives <= 0).all() and values.argmax() == 0:
+            return optimum
+
+        if (np.diff(derivatives >= 0) >= 0).all() and derivatives[-1] <= 0:
+            index = max((derivatives >= 0).argmin(), 1)
+            bounds = x[index - 1], x[index]
+        elif abs(derivatives).min() < 1e-6:
+            argmax = values.argmax()
+            bounds = x[max(argmax - 1, 0)], x[min(argmax + 1, len(values) - 1)]
+        else:
+            raise RuntimeError(
+                f"There are multiple optima in the function delta(x, x0={x0}, chi={chi})."
+            )
+
+        result = minimize_scalar(
+            lambda x: -delta(x, x0, chi), bounds=bounds, method="bounded"
+        )
+        return (-result.fun, result.x) if -result.fun > optimum[0] else optimum
+
+    def delta(x, x0, chi):
+        def func(x):
+            return (
+                0.5 * r2(x0, chi)  # apply L'Hopital's rule
+                if abs(x - x0) < 1e-4
+                else (r(x, chi) - r(x0, chi) - (x - x0) * r1(x0, chi)) / (x - x0) ** 2
+            )
+
+        return func(x) if np.isscalar(x) else np.array([func(x_i) for x_i in x])
+
+    def delta1(x, x0, chi):
+        # first derivative of delta
+        def func(x):
+            if abs(x - x0) < 1e-3:
+                # apply L'Hoptial's rule
+                return r3(x0, chi)
+            return (
+                r1(x, chi) + r1(x0, chi) - 2 * (r(x, chi) - r(x0, chi)) / (x - x0)
+            ) / (x - x0) ** 2
+
+        return func(x) if np.isscalar(x) else np.array([func(x_i) for x_i in x])
+
+    tol = 1e-12
+    critical_value_b = (
+        np.sqrt(ncx2.ppf(1 - alpha, nc=m2, df=1))
+        if m2 < 100
+        else norm.ppf(1 - alpha, np.sqrt(m2))
+    )
+    if m2 == 0 or kurtosis == 1:
+        return critical_value_b, np.array([0, m2]), np.array([0, 1])
+
+    if m2 > 1 / tol and kurtosis != np.inf:
+        kurtosis = np.inf
+
+    # get bounds for when kappa == 1 and kappa == infinity
+    lower, upper = critical_value_b - 0.01, np.sqrt((m2 + 1) / alpha)
+    if abs(rho0(upper) - alpha) > 9e-6:
+        upper = root_scalar(
+            lambda chi: rho0(chi) - alpha, bracket=(lower, upper), method="brentq"
+        ).root
+
+    if rho(upper)[0] - alpha < -1e-5:
+        critical_value = root_scalar(
+            lambda chi: rho(chi)[0] - alpha, bracket=(lower, upper), method="brentq"
+        ).root
+    else:
+        critical_value = upper
+    return critical_value, *rho(critical_value)[1:]
+
+
+class NormalResults(BayesResults):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # estimate constraints and kurtosis for computing robust confidence intervals
+        # constraints are denoted "m2" in Armstrong et al., 2020
+        self._robust_conf_int_constraints = (
+            self.model.cov.diagonal() / self.model.prior_cov.diagonal()
+        )
+        cov_inv = np.linalg.inv(self.model.cov)
+        weights = (
+            np.linalg.inv(self.model.X.T @ cov_inv @ self.model.X)
+            @ self.model.X.T
+            @ cov_inv
+        )
+        error = self.model.mean - self.model.prior_mean
+        cov_diag = self.model.cov.diagonal()
+        prior_cov_diag = self.model.prior_cov.diagonal()
+        kurtosis0 = (
+            weights * (error**4 - 6 * cov_diag * error**2 + 3 * cov_diag**2)
+        ).sum() / (weights * prior_cov_diag**2).sum()
+        kurtosis1 = (
+            1
+            + 32
+            * (weights**2 * cov_diag**4).sum()
+            / (weights * (prior_cov_diag**2 + cov_diag**2)).sum()
+        )
+        self._kurtosis = max(kurtosis0, kurtosis1)
+
+    def conf_int(
+        self,
+        alpha: float = 0.05,
+        columns: ColumnsType = None,
+        robust: bool = False,
+        fast: bool = False,
+        **kwargs: Any,
+    ) -> np.ndarray:
+        """Compute the 1-alpha confidence interval.
+
+        Args:
+            alpha (float, optional): Significance level. Defaults to .05.
+            columns (ColumnsType, optional): Selected columns. Defaults to None.
+            robust (bool, optional): Use robust confidence intervals. These will have
+                correct average coverage even if the normal prior assumption is
+                violated. Defaults to False.
+            fast (bool, optional): Use a "fast" computation method for the robust
+                confidence intervals. This assumes the critical value is the same for
+                all parameters. Defaults to False.
+
+        Returns:
+            np.ndarray: (# params, 2) array of confidence intervals.
+        """
+        if not robust:
+            return super().conf_int(alpha, columns, **kwargs)
+
+        indices = self.model.get_indices(columns)
+        constraints = self._robust_conf_int_constraints[indices]
+        if fast or np.isclose(constraints, constraints[0]).all():
+            constraint = constraints.mean()
+            critical_values = np.full(
+                len(constraints),
+                [compute_robust_critical_value(constraint, self._kurtosis, alpha)[0]],
+            )
+        else:
+            critical_values = np.array(
+                [
+                    compute_robust_critical_value(x, self._kurtosis, alpha)[0]
+                    for x in constraints
+                ]
+            )
+        len_conf_int = critical_values * np.sqrt(
+            self.model.posterior_cov.diagonal()[indices]
+        )
+        params = self.params[indices]
+        return np.array([params - len_conf_int, params + len_conf_int]).T
+
+
+class Normal(BayesBase):
+    """Bayesian model with a normal prior.
+
+    Args:
+        fit_method (Union[str, Callable[[], None]], optional): Specifies how to fit the
+            prior ("mle", "bock", or "james_stein"). You can also use a custom function
+            that sets the ``prior_mean``, ``prior_cov``, ``posterior_mean`` and
+            ``posterior_cov`` attributes. Defaults to "mle".
+        prior_mean (Union[float, np.ndarray], optional): (# params,) prior mean vector.
+            Defaults to None.
+        prior_cov (Union[float, np.ndarray], optional): (# params, # params) prior
+            covariance matrix. Defaults to None.
+
+    Examples:
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.bayes import Normal
+
+            model = Normal(np.arange(10), np.identity(10))
+            results = model.fit()
+            print(results.summary())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+                       Bayesian estimates
+            =======================================
+                coef pvalue (1-sided) [0.025 0.975]
+            ---------------------------------------
+            x0 0.545            0.282 -1.305  2.395
+            x1 1.424            0.066 -0.426  3.274
+            x2 2.303            0.007  0.453  4.153
+            x3 3.182            0.000  1.332  5.032
+            x4 4.061            0.000  2.211  5.911
+            x5 4.939            0.000  3.089  6.789
+            x6 5.818            0.000  3.968  7.668
+            x7 6.697            0.000  4.847  8.547
+            x8 7.576            0.000  5.726  9.426
+            x9 8.455            0.000  6.605 10.305
+            ===============
+            Dep. Variable y
+            ---------------
+    """
+
+    _results_cls = NormalResults
+
+    def __init__(
+        self,
+        *args: Any,
+        fit_method: Union[str, Callable[[], None]] = "mle",
+        prior_mean: Union[float, np.ndarray] = None,
+        prior_cov: Union[float, np.ndarray] = None,
+        **kwargs: Any,
+    ):
+        super().__init__(*args, **kwargs)
+        self.prior_mean, self.prior_cov = prior_mean, prior_cov
+        if np.isscalar(prior_mean):
+            self.prior_mean = np.full(self.n_params, prior_mean)
+        if np.isscalar(prior_cov):
+            self.prior_cov = prior_cov * np.identity(self.n_params)
+
+        self.posterior_mean, self.posterior_cov = None, None
+        if callable(fit_method):
+            fit_method()
+            self._set_posterior_estimates()
+        else:
+            fit_methods = {
+                "mle": self._fit_mle,
+                "james_stein": self._fit_james_stein,
+                "bock": self._fit_bock,
+            }
+            if fit_method not in fit_methods:
+                raise ValueError(
+                    f"`fit_method` must be one of {fit_methods.keys()}, got {fit_method}."
+                )
+            fit_methods[fit_method]()
+
+    def _fit_mle(self, max_iter: int = 100, rtol: float = 0.99) -> None:
+        """Fit the model using maximum likelihood estimation.
+
+        Args:
+            max_iter (int, optional): Maximum number of EM iterations. Defaults to 100.
+            rtol (float, optional): Stopping criterion for EM. Defaults to .99.
+        """
+
+        def neg_log_likelihood(prior_std):
+            # negative log likelihood as a function of the prior standard deviation
+            marginal_cov = prior_std**2 * np.identity(self.n_params) + self.cov
+            # note: the prior mean is also the marginal mean
+            return -multivariate_normal.logpdf(self.mean, prior_mean, marginal_cov)
+
+        # use EM to iteratively update the prior mean and covariance
+        prior_cov = (
+            np.zeros(self.cov.shape) if self.prior_cov is None else self.prior_cov
+        )
+        current_log_likelihood, prev_log_likelihood = None, -np.inf
+        for _ in range(max_iter):
+            # update prior mean
+            if self.prior_mean is not None:
+                prior_mean = self.prior_mean
+            else:
+                marginal_cov_inv = np.linalg.inv(self.cov + prior_cov)
+                prior_mean = (
+                    self.X
+                    @ np.linalg.inv(self.X.T @ marginal_cov_inv @ self.X)
+                    @ self.X.T
+                    @ marginal_cov_inv
+                    @ self.mean
+                )
+
+            # update prior cov
+            if self.prior_cov is not None:
+                prior_cov = self.prior_cov
+                break  # prior_mean is computed analytically, so no need to iterate futher
+            else:
+                result = minimize_scalar(
+                    neg_log_likelihood, bounds=(0, self.mean.std()), method="bounded"
+                )
+                prior_cov = result.x**2 * np.identity(self.n_params)
+                current_log_likelihood = -result.fun
+
+            if current_log_likelihood / prev_log_likelihood > rtol:
+                break
+            prev_log_likelihood = current_log_likelihood
+
+        # set the posterior mean and covariance estimates
+        # and adjust the prior and posterior covariances to account for uncertainty in the MLE estimate of the prior mean
+        prior_uncertainty = post_uncertainty = 0
+        if self.prior_mean is None:
+            marginal_cov_inv = np.linalg.inv(prior_cov + self.cov)
+            prior_uncertainty = (
+                self.X @ np.linalg.inv(self.X.T @ marginal_cov_inv @ self.X) @ self.X.T
+            )
+            xi = self.cov @ marginal_cov_inv
+            post_uncertainty = xi @ prior_uncertainty @ xi
+
+        self.prior_mean, self.prior_cov = prior_mean, prior_cov
+        self._set_posterior_estimates()  # note: set the posterior estimates *before* adjusting the prior covariance
+        self.prior_cov += prior_uncertainty
+        self.posterior_cov += post_uncertainty
+
+    def _fit_bock(self, max_iter: int = 100, rtol: float = 0.99) -> None:
+        """Fit the model using Bock (1975)'s multivariate Stein-type estimator.
+
+        Args:
+            max_iter (int, optional): Maximum number of iterations. Defaults to 100.
+            rtol (float, optional): Stopping criteria. Defaults to .99.
+
+        Raises:
+            RuntimeError: The shrinkage factor must be positve.
+        """
+        cov_inv = np.linalg.inv(self.cov)
+        prior_mean_df = self.X.shape[1] if self.prior_mean is None else 0
+        effective_dimension = np.trace(self.cov) / np.linalg.eig(self.cov)[0].max()
+        if effective_dimension - prior_mean_df - 2 < 0:
+            raise RuntimeError(
+                "Failed to fit the Bock (1975) estimator because the effective dimension"
+                " of the covariance matrix is too small. Try another fit method like"
+                " 'mle'."
+            )
+
+        xi = (
+            np.identity(self.n_params)
+            if self.prior_cov is None
+            else self.cov @ np.linalg.inv(self.cov + self.prior_cov)
+        )
+        current_log_likelihood, prev_log_likelihood = None, -np.inf
+        for _ in range(max_iter):
+            if self.prior_mean is None:
+                # update prior mean
+                marginal_cov_inv = cov_inv @ xi
+                prior_mean = (
+                    self.X
+                    @ np.linalg.inv(self.X.T @ marginal_cov_inv @ self.X)
+                    @ self.X.T
+                    @ marginal_cov_inv
+                    @ self.mean
+                )
+            else:
+                prior_mean = self.prior_mean
+
+            if self.prior_cov is None:
+                # update prior covariance
+                error = self.mean - prior_mean
+                param = min(
+                    (effective_dimension - prior_mean_df - 2)
+                    / (error.T @ cov_inv @ error),
+                    1,
+                )
+                xi = param * np.identity(self.n_params)
+            else:
+                prior_cov = self.prior_cov
+                # prior mean is computed analytically, so no need to iterate
+                break
+
+            # check for convergence
+            marginal_cov = np.linalg.inv(xi) @ self.cov
+            prior_cov = marginal_cov - self.cov
+            current_log_likelihood = multivariate_normal.logpdf(
+                self.mean, prior_mean, marginal_cov
+            )
+            if current_log_likelihood / prev_log_likelihood > rtol:
+                break
+            prev_log_likelihood = current_log_likelihood
+
+        # set the posterior mean and covariance estimates
+        # and adjust the prior and posterior covariances to account for uncertainty in the MLE estimate of the prior mean
+        prior_uncertainty = post_uncertainty = 0
+        if self.prior_mean is None:
+            marginal_cov_inv = np.linalg.inv(prior_cov + self.cov)
+            prior_uncertainty = (
+                self.X @ np.linalg.inv(self.X.T @ marginal_cov_inv @ self.X) @ self.X.T
+            )
+            xi = self.cov @ marginal_cov_inv
+            post_uncertainty = xi @ prior_uncertainty @ xi
+
+        self.prior_mean, self.prior_cov = prior_mean, prior_cov
+        self._set_posterior_estimates()  # note: set the posterior estimates *before* adjusting the prior covariance
+        self.prior_cov += prior_uncertainty
+        self.posterior_cov += post_uncertainty
+
+    def _set_posterior_estimates(self):
+        """Sets the posterior mean and covariance using plugin estimates from the prior
+        mean and covariance if the posterior parameters haven't already been set.
+        """
+        xi = self.cov @ np.linalg.inv(self.prior_cov + self.cov)
+        if self.posterior_mean is None:
+            self.posterior_mean = self.prior_mean + (
+                np.identity(self.n_params) - xi
+            ) @ (self.mean - self.prior_mean)
+
+        if self.posterior_cov is None:
+            self.posterior_cov = (np.identity(self.n_params) - xi) @ self.cov
+
+    def _fit_james_stein(self, max_iter: int = 100, tol: float = 1e-6) -> None:
+        """Fit the model using James-Stein estimates.
+
+        Args:
+            max_iter (int, optional): Maximum number of iterations to find the
+                positive-part prior covariance.. Defaults to 100.
+            tol (float, optional): Stopping criteria for finding the positive-part prior
+                covariance. Defaults to 1e-6.
+        """
+        if self.prior_mean is None:
+            prior_mean = (
+                self.X @ np.linalg.inv(self.X.T @ self.X) @ self.X.T @ self.mean
+            )
+            prior_mean_df = self.X.shape[1]
+        else:
+            prior_mean = self.prior_mean
+            prior_mean_df = 0
+
+        s_squared = ((self.mean - prior_mean) ** 2).sum()
+        try:
+            np.linalg.cholesky(
+                s_squared
+                / (self.n_params - prior_mean_df - 2)
+                * np.identity(self.n_params)
+                - self.cov
+            )
+        except np.linalg.LinAlgError:
+            # find minimum s_squared such that the (unadjusted) prior covariance is positive semidefinite
+            warnings.warn(
+                "The James-Stein prior covariance estimate is not positive semidefinite."
+                " Using the positive-part James-Stein covariance estimate instead."
+                " This may result in too little shrinkage."
+            )
+            bounds = [np.sqrt(s_squared), np.inf]
+            for _ in range(max_iter):
+                s_squared = (
+                    2 * bounds[0] if bounds[1] == np.inf else sum(bounds) / 2
+                ) ** 2
+                try:
+                    np.linalg.cholesky(
+                        s_squared
+                        / (self.n_params - prior_mean_df - 2)
+                        * np.identity(self.n_params)
+                        - self.cov
+                    )
+                    bounds[1] = np.sqrt(s_squared)
+                except:
+                    bounds[0] = np.sqrt(s_squared)
+                if bounds[1] - bounds[0] < tol:
+                    break
+            s_squared = bounds[1] ** 2
+
+        # compute the prior covariance
+        param = s_squared / (self.n_params - prior_mean_df - 4)
+        self.prior_cov = (
+            param * np.identity(self.n_params)
+            - self.cov
+            + param * self.X @ np.linalg.inv(self.X.T @ self.X) @ self.X.T
+        )
+
+        # compute the posterior mean
+        xi = self.cov * (self.n_params - prior_mean_df - 2) / s_squared
+        self.posterior_mean = prior_mean + (np.identity(self.n_params) - xi) @ (
+            self.mean - prior_mean
+        )
+
+        # compute the posterior covariance
+        plugin_posterior_cov = (np.identity(self.n_params) - xi) @ self.cov
+        if self.prior_mean is None:
+            prior_mean_uncertainty = (
+                self.cov @ self.X @ np.linalg.inv(self.X.T @ self.X) @ self.X.T @ xi
+            )
+        else:
+            prior_mean_uncertainty = 0
+        prior_cov_uncertainty = (
+            2
+            / (self.n_params - self.X.shape[1] - 2)
+            * xi
+            @ (self.mean - prior_mean).reshape(-1, 1)
+            @ (self.mean - prior_mean).reshape(1, -1)
+            @ xi
+        )
+        self.posterior_cov = (
+            plugin_posterior_cov + prior_mean_uncertainty + prior_cov_uncertainty
+        )
+
+        self.prior_mean = prior_mean
+
+    def _get_marginal_prior(self, index: int) -> rv_continuous:
+        return norm(self.prior_mean[index], np.sqrt(self.prior_cov[index, index]))
+
+    def _get_marginal_distribution(self, index: int) -> rv_continuous:
+        return norm(
+            self.posterior_mean[index], np.sqrt(self.posterior_cov[index, index])
+        )
+
+    def _get_joint_prior(self, indices: np.ndarray):
+        return multivariate_normal(
+            self.prior_mean[indices],
+            self.prior_cov[indices][:, indices],
+            allow_singular=True,
+        )
+
+    def _get_joint_distribution(self, indices: np.ndarray):
+        return multivariate_normal(
+            self.posterior_mean[indices],
+            self.posterior_cov[indices][:, indices],
+            allow_singular=True,
+        )
```

### Comparing `multiple-inference-1.1.0/src/multiple_inference/confidence_set.py` & `multiple-inference-1.2.0/src/multiple_inference/confidence_set.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,855 +1,1037 @@
-"""Simultaneous confidence sets and multiple hypothesis testing.
-
-References:
-
-    .. code-block::
-
-        @article{storey2003statistical,
-            title={Statistical significance for genomewide studies},
-            author={Storey, John D and Tibshirani, Robert},
-            journal={Proceedings of the National Academy of Sciences},
-            volume={100},
-            number={16},
-            pages={9440--9445},
-            year={2003},
-            publisher={National Acad Sciences}
-        }
-
-        @article{romano2005stepwise,
-            title={Stepwise multiple testing as formalized data snooping},
-            author={Romano, Joseph P and Wolf, Michael},
-            journal={Econometrica},
-            volume={73},
-            number={4},
-            pages={1237--1282},
-            year={2005},
-            publisher={Wiley Online Library}
-        }
-
-        @techreport{mogstad2020inference,
-            title={Inference for ranks with applications to mobility across neighborhoods and academic achievement across countries},
-            author={Mogstad, Magne and Romano, Joseph P and Shaikh, Azeem and Wilhelm, Daniel},
-            year={2020},
-            institution={National Bureau of Economic Research}
-        }
-"""
-from __future__ import annotations
-
-import warnings
-from itertools import combinations
-from typing import Any, Sequence, Union
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import seaborn as sns
-from scipy.optimize import minimize
-from scipy.stats import multivariate_normal, norm
-
-from multiple_inference.base import ColumnsType, ModelBase, ResultsBase
-
-
-class ConfidenceSetResults(ResultsBase):
-    """Results for simultaneous confidence sets.
-
-    Subclasses :class:`multiple_inference.base.ResultsBase`.
-
-    Args:
-        n_samples (int, optional): Number of samples to draw when approximating the
-            confidence set. Defaults to 10000.
-    """
-
-    _default_title = "Confidence set results"
-
-    def __init__(self, *args: Any, n_samples: int = 10000, **kwargs: Any):
-        super().__init__(*args, **kwargs)
-        self.params = self.model.mean.copy()
-
-        # draw random values for confidence set approximation
-        self._std_diagonal = np.sqrt(self.model.cov.diagonal())
-        rvs = multivariate_normal.rvs(
-            np.zeros(self.model.n_params),
-            self.model.cov,
-            size=n_samples,
-            random_state=self.model.random_state,
-        )
-        rvs /= self._std_diagonal
-        self._rvs = np.hstack([rvs, -rvs])
-        self._set_pvalues()
-        self._set_qvalues()
-
-    def _set_pvalues(self):
-        if self.model.n_params == 1:
-            self.pvalues = 2 * np.atleast_1d(
-                norm.cdf(-abs(self.model.mean[0]), 0, np.sqrt(self.model.cov[0, 0]))
-            )
-        else:
-            params = np.expand_dims(self.params, -1)
-            arr = self._rvs.max(axis=1) * np.expand_dims(self._std_diagonal, -1)
-            self.pvalues = np.array(
-                [(params - arr < 0).mean(axis=1), (params + arr > 0).mean(axis=1)]
-            ).min(axis=0)
-
-    def _set_qvalues(self):
-        if self.model.n_params == 1:
-            self.qvalues = self.pvalues.copy()
-        else:
-            # get conventional pvalues
-            pvalues = norm.cdf(self.params / self._std_diagonal)
-            # convert to 2-sided pvalues
-            pvalues = 2 * np.min([pvalues, 1 - pvalues], axis=0)
-            argsort = (-pvalues).argsort()
-            pvalues = pvalues[argsort]
-            # define x over (0, .9 * max pvalue)
-            # extending x too close to the max pvalue introduces noise
-            x = np.linspace(0, 0.9 * pvalues[0])
-            pi0 = (pvalues > np.expand_dims(x, 1)).mean(axis=1) / (1 - x)
-            # fit an exponential smoothing spline to estimate the true null rate
-            spline = lambda x, params: params[0] + params[1] * np.exp(
-                -params[1] * x / params[2]
-            )
-            params = minimize(
-                lambda params: ((spline(x, params) - pi0) ** 2).sum(), [0, 1, 1]
-            ).x
-            true_null_rate = np.clip(spline(pvalues[0], params), 0, 1)
-            # compute qvalues
-            qvalues = [1]
-            for i, pvalue in enumerate(pvalues):
-                qvalues.append(
-                    min(
-                        true_null_rate * pvalue * len(pvalues) / (len(pvalues) - i),
-                        qvalues[-1],
-                    )
-                )
-            self.qvalues = np.array(qvalues[1:])[argsort.argsort()]
-
-    def _conf_int(self, alpha: float, indices: np.ndarray) -> np.ndarray:
-        if self.model.n_params == 1:
-            return np.atleast_2d(
-                norm.ppf(
-                    [alpha / 2, 1 - alpha / 2],
-                    self.model.mean[0],
-                    np.sqrt(self.model.cov[0, 0]),
-                )
-            )
-
-        params = self.params[indices]
-        arr = (
-            np.quantile(self._rvs.max(axis=1), 1 - alpha) * self._std_diagonal[indices]
-        )
-        return np.array([params - arr, params + arr]).T
-
-    def test_hypotheses(
-        self, alpha: float = 0.05, columns: ColumnsType = None, two_tailed: bool = True
-    ) -> Union[pd.DataFrame, pd.Series]:
-        """Test the null hypothesis that the parameter is equal to 0.
-
-        Args:
-            alpha (float, optional): Significance level. Defaults to 0.05.
-            columns (ColumnsType, optional): Selected columns. Defaults to None.
-            two_tailed (bool, optional): Run two-tailed hypothesis tests. Set to False
-                to run one-tailed hypothesis tests. Defaults to True.
-
-        Returns:
-            Union[pd.DataFrame, pd.Series]: Results dataframe (if two-tailed) or series
-                (if one-tailed).
-        """
-        # use pvalues to reject hypotheses to control the familywise error rate
-        if two_tailed:
-            params = np.concatenate([self.params, -self.params])
-            rvs = self._rvs
-            std_diagonal = np.concatenate([self._std_diagonal, self._std_diagonal])
-        else:
-            params = self.params
-            rvs = self._rvs[:, : self.model.n_params]
-            std_diagonal = self._std_diagonal
-
-        rejected, newly_rejected = np.full(rvs.shape[1], False), None
-        while newly_rejected is None or (newly_rejected.any() and not rejected.all()):
-            quantile = np.quantile(rvs[:, ~rejected].max(axis=1), 1 - alpha)
-            newly_rejected = (params - quantile * std_diagonal > 0) & ~rejected
-            rejected = rejected | newly_rejected
-
-        indices = self.model.get_indices(columns, self.exog_names)
-        if two_tailed:
-            return pd.DataFrame(
-                rejected.reshape(2, -1).T[indices],
-                columns=["param>0", "param<0"],
-                index=self.exog_names[indices],
-            )
-        return pd.Series(
-            rejected[indices], name="param>0", index=self.exog_names[indices]
-        )
-
-    def _make_summary_header(self, alpha: float) -> list[str]:
-        return [
-            "coef (conventional)",
-            "pvalue",
-            "qvalue",
-            f"{1-alpha} CI lower",
-            f"{1-alpha} CI upper",
-        ]
-
-    def _make_summary_data(
-        self, alpha: float, indices: np.ndarray, **kwargs: Any
-    ) -> np.ndarray:
-        if not hasattr(self, "params"):
-            raise AttributeError("Results object does not have `params` attribute.")
-
-        return np.hstack(
-            (
-                np.array([self.params, self.pvalues, self.qvalues]).T[indices],
-                self.conf_int(alpha, indices, **kwargs),
-            )
-        )
-
-
-class ConfidenceSet(ModelBase):
-    """Model for simultaneous confidence sets.
-
-    Examples:
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.confidence_set import ConfidenceSet
-
-            x = np.arange(-1, 2)
-            cov = np.identity(3) / 10
-            model = ConfidenceSet(x, cov)
-            results = model.fit()
-            print(results.summary())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-            Confidence set results
-            ================================================================
-               coef (conventional) pvalue qvalue 0.95 CI lower 0.95 CI upper
-            ----------------------------------------------------------------
-            x0              -1.000  0.004  0.002        -1.755        -0.245
-            x1               0.000  1.000  1.000        -0.755         0.755
-            x2               1.000  0.004  0.002         0.245         1.755
-            ===============
-            Dep. Variable y
-            ---------------
-
-        .. testcode::
-
-            print(results.test_hypotheses())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-                param>0  param<0
-            x0    False     True
-            x1    False    False
-            x2     True    False
-    """
-
-    _results_cls = ConfidenceSetResults
-
-
-class AverageComparison(ConfidenceSet):
-    """Compare each parameter to the average value across all parameters.
-
-    Subclasses :class:`ConfidenceSet`.
-
-    Args:
-        *args (Any): Passed to :class:`ConfidenceSet`.
-        **kwargs (Any): Passed to :class:`ConfidenceSet`.
-
-    Examples:
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.confidence_set import AverageComparison
-
-            x = np.arange(-1, 2)
-            cov = np.identity(3) / 10
-            model = AverageComparison(x, cov)
-            results = model.fit()
-            print(results.summary())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-            Confidence set results
-            ================================================================
-               coef (conventional) pvalue qvalue 0.95 CI lower 0.95 CI upper
-            ----------------------------------------------------------------
-            x0              -1.000  0.000  0.000        -1.603        -0.397
-            x1               0.000  1.000  1.000        -0.603         0.603
-            x2               1.000  0.000  0.000         0.397         1.603
-            ===============
-            Dep. Variable y
-            ---------------
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        identity = np.identity(self.n_params)
-        cov_inv = np.linalg.inv(self.cov)
-        projection = (
-            self.X @ np.linalg.inv(self.X.T @ cov_inv @ self.X) @ self.X.T @ cov_inv
-        )
-        self.mean = (identity - projection) @ self.mean
-        cov = (identity - projection) @ self.cov @ (identity - projection).T
-        if np.isnan(cov).all():
-            warnings.warn(
-                f"Error encountered in recomputing covariance matrix. "
-                "Using original covariance matrix instead.",
-                RuntimeWarning,
-            )
-        else:
-            self.cov = cov
-
-
-class BaselineComparison(ConfidenceSet):
-    """Compare parameters to a baseline parameter.
-
-    Subclasses :class:`ConfidenceSet`.
-
-    Args:
-        baseline (Union[int, str]): Index or name of the baseline parameter.
-
-    Examples:
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.confidence_set import BaselineComparison
-
-            x = np.arange(-1, 2)
-            cov = np.identity(3) / 10
-            model = BaselineComparison(x, cov, exog_names=["x0", "x1", "x2"], baseline="x0")
-            results = model.fit()
-            print(results.summary())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-            Confidence set results
-            ================================================================
-               coef (conventional) pvalue qvalue 0.95 CI lower 0.95 CI upper
-            ----------------------------------------------------------------
-            x1               1.000  0.045  0.012         0.022         1.978
-            x2               2.000  0.000  0.000         1.022         2.978
-            ===============
-            Dep. Variable y
-            ---------------
-    """
-
-    def __init__(self, *args, baseline: Union[int, str], **kwargs):
-        super().__init__(*args, **kwargs)
-        index = int(
-            baseline
-            if isinstance(baseline, (float, int))
-            else list(self.exog_names).index(baseline)
-        )
-        self.n_params -= 1
-        self.mean = np.delete(self.mean, index) - self.mean[index]
-        self.cov = (
-            np.delete(np.delete(self.cov, index, axis=0), index, axis=1)
-            + self.cov[index, index]
-        )
-        if self._exog_names is not None:
-            self.exog_names = np.delete(self.exog_names, index)
-
-
-class PairwiseComparisonResults(ConfidenceSetResults):
-    """Results of pairwise comparisons.
-
-    Subclasses :class:`ConfidenceSetResults`.
-
-    Args:
-        n_samples (int, optional): Number of samples to draw to obtain critical
-            values. Defaults to 10000.
-        groups (np.ndarray, optional): (# params,) array of parameter groups.
-            Defaults to None.
-
-    Raises:
-        ValueError: Length of ``groups`` must match the number of parameters.
-    """
-
-    _default_title = "Pairwise comparisons"
-
-    def __init__(
-        self,
-        *args: Any,
-        n_samples: int = 10000,
-        groups: np.ndarray = None,
-        **kwargs: Any,
-    ):
-
-        super().__init__(*args, **kwargs)
-        self._groups = (
-            np.zeros(self.model.n_params) if groups is None else np.array(groups)
-        )
-        if len(self._groups) != self.model.n_params:
-            raise ValueError(
-                "Length of groups must equal the number of parameters. Got "
-                f"{self.model.n_params} parameters and groups of length "
-                f" {len(self._groups)}."
-            )
-
-        variance = self.model.cov.diagonal()
-        rvs = multivariate_normal.rvs(
-            self.model.mean,
-            self.model.cov,
-            size=n_samples,
-            random_state=self.model.random_state,
-        )
-        exog_names, params, delta_variance, delta_rvs = [], [], [], []
-        pairwise_groups = []
-        for group in np.unique(self._groups):
-            mask = self._groups == group
-            pairwise_groups += int(0.5 * mask.sum() * (mask.sum() - 1)) * [group]
-            group_exog_names, group_params, group_variance, group_rvs = (
-                self.exog_names[mask],
-                self.params[mask],
-                variance[mask],
-                rvs[:, mask],
-            )
-            for i in range(mask.sum()):
-                exog_names.append(
-                    [
-                        f"{name} - {group_exog_names[i]}"
-                        for name in group_exog_names[i + 1 :]
-                    ]
-                )
-                params.append(group_params[i + 1 :] - group_params[i])
-                # variance of the differences between x_i and x_j
-                delta_variance.append(group_variance[i + 1 :] + group_variance[i])
-                # random sample of the differences between x_i and x_j
-                delta_rvs.append(
-                    group_rvs[:, i + 1 :] - np.expand_dims(group_rvs[:, i], -1)
-                )
-
-        self.exog_names = np.concatenate(exog_names)
-        self.params = np.concatenate(params)
-        self._std_diagonal = np.sqrt(np.concatenate(delta_variance))
-        rvs = (np.hstack(delta_rvs) - self.params) / self._std_diagonal
-        self._rvs = np.hstack([rvs, -rvs])
-        self._pairwise_groups = np.array(pairwise_groups)
-        self._set_pvalues()
-        self._set_qvalues()
-
-    def test_hypotheses(
-        self,
-        alpha: float = 0.05,
-        columns: ColumnsType = None,
-        criterion: str = "fwer",
-        groups: Sequence = None,
-        wide: bool = True,
-    ) -> Union[pd.DataFrame, dict[Any, pd.DataFrame]]:
-        """Test pairwise hypotheses.
-
-        Args:
-            alpha (float, optional): Significance level. Defaults to .05.
-            columns (ColumnsType, optional): Selected columns. In wide format, these are
-                the original column names (e.g., "x0"). In long format, these are the
-                names of the differences (e.g., "x1 - x0"). Defaults to None.
-            criterion (str, optional): "fwer" to control for the family-wise error rate
-                (using pvalues), "fdr" to control for the false discovery rate (using
-                qvalues). Defaults to "fwer".
-            groups (Sequence, optional). Selected groups of parameters. Defaults to None.
-            wide (bool, optional): Return the results is wide (square) format. Ignored
-                when controlling for the false discovery rate. Defaults to True.
-
-        Raises:
-            ValueError: ``criterion`` must be one of "fwer" or "fdr".
-
-        Returns:
-            Union[pd.DataFrame, dict[Any, pd.DataFrame]]: Results dataframe if only one
-                group is used, mapping of group name to results dataframe if multiple
-                groups are used.
-
-        Notes:
-            When controlling for the familywise error rate, the null hypotheses are
-            $$mu_k \leq \mu_j$$. When controlling for the false discovery rate, the null
-            hypotheses are $$\mu_k = \mu_j$$.
-        """
-        if criterion not in ("fwer", "fdr"):
-            raise ValueError(f"criterion should be in 'fwer', 'fdr', got {criterion}.")
-
-        if criterion == "fwer":
-            if not wide:
-                return super().test_hypotheses(alpha, columns)
-            rejected = super().test_hypotheses(alpha).values
-        else:
-            rejected = self.qvalues < alpha
-            rejected = np.vstack([rejected, rejected]).T
-
-        # reshape rejected array into a square matrix
-        return_value = {}
-        for group in groups or np.unique(self._groups):
-            mask = self._groups == group
-            pairwise_mask = self._pairwise_groups == group
-            n_params = mask.sum()
-            tri = np.full((n_params, n_params), False)
-            indices = np.triu_indices(n_params, 1)
-            tri[indices] = rejected[pairwise_mask, 0]
-            tri[(indices[1], indices[0])] = rejected[pairwise_mask, 1]
-
-            exog_names = self.model.exog_names[mask]
-            indices = self.model.get_indices(columns, exog_names)
-            column_names = exog_names[indices]
-            return_value[group] = pd.DataFrame(
-                tri[indices][:, indices], index=column_names, columns=column_names
-            )
-
-        return (
-            list(return_value.values())[0] if len(return_value) == 1 else return_value
-        )
-
-    def hypothesis_heatmap(
-        self,
-        *args: Any,
-        title: str = None,
-        axes=None,
-        triangular: bool = False,
-        **kwargs: Any,
-    ):
-        """Create a heatmap of pairwise hypothesis tests.
-
-        Args:
-            title (str, optional): Title.
-            axes (Union[AxesSubplot, Sequence[AxesSubplot]], optional): Axes to write
-                on. Defaults to None.
-            triangular (bool, optional): Display the results in a triangular (as opposed
-                to square) output. Usually, you should set this to True if and only if
-                your columns are sorted. Defaults to False.
-
-        Returns:
-            np.ndarray: Array of axes.
-        """
-
-        def write_heatmap(group, matrix, ax):
-            if triangular:
-                mask = np.zeros_like(matrix)
-                mask[np.triu_indices_from(mask)] = True
-            else:
-                mask = None
-
-            sns.heatmap(
-                matrix,
-                cbar=False,
-                ax=ax,
-                yticklabels=matrix.index,
-                xticklabels=matrix.columns,
-                mask=mask,
-                square=True,
-                cmap=sns.color_palette()[3:1:-1],
-                center=0.5,
-            )
-            ax.set_title(
-                (title or self.title) + ("" if group is None else f" group = {group}")
-            )
-            ax.set_yticklabels(ax.get_yticklabels(), rotation=0)
-
-        results = self.test_hypotheses(*args, **kwargs)
-        if isinstance(results, dict):
-            if axes is None:
-                fig, axes = plt.subplots(len(results))
-                fig.tight_layout()
-            for (group, matrix), ax in zip(results.items(), axes):
-                write_heatmap(group, matrix, ax)
-        else:
-            if axes is None:
-                _, axes = plt.subplots()
-            write_heatmap(None, results, axes)
-
-        return axes
-
-    def _make_summary_header(self, alpha: float) -> list[str]:
-        return [
-            "delta (conventional)",
-            "pvalue",
-            "qvalue",
-            f"{1-alpha} CI lower",
-            f"{1-alpha} CI upper",
-        ]
-
-
-class PairwiseComparison(ConfidenceSet):
-    """Compute pairwise comparisons.
-
-    Examples:
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.confidence_set import PairwiseComparison
-
-            x = np.arange(-1, 2)
-            cov = np.identity(3) / 10
-            model = PairwiseComparison(x, cov)
-            results = model.fit()
-            print(results.summary())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-            Pairwise comparisons
-            ======================================================================
-                    delta (conventional) pvalue qvalue 0.95 CI lower 0.95 CI upper
-            ----------------------------------------------------------------------
-            x1 - x0                1.000  0.061  0.017        -0.031         2.031
-            x2 - x0                2.000  0.000  0.000         0.969         3.031
-            x2 - x1                1.000  0.061  0.017        -0.031         2.031
-            ===============
-            Dep. Variable y
-            ---------------
-
-        .. testcode::
-
-            print(results.test_hypotheses())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-                   x0     x1     x2
-            x0  False  False   True
-            x1  False  False  False
-            x2  False  False  False
-
-        This means that parameter x2 is significantly greater than x0.
-    """
-
-    _results_cls = PairwiseComparisonResults
-
-
-class MarginalRankingResults(ResultsBase):
-    """Marginal ranking results."""
-
-    _default_title = "Marginal ranking"
-
-    def __init__(
-        self, model: MarginalRanking, *args: Any, n_samples: int = 10000, **kwargs: Any
-    ):
-        super().__init__(model, *args, **kwargs)
-        self.params = (-self.model.mean).argsort().argsort() + 1
-        self._baseline_comparisons = [
-            BaselineComparison(model.mean, model.cov, baseline=i).fit(
-                n_samples=n_samples
-            )
-            for i in range(model.n_params)
-        ]
-
-    def _conf_int(self, alpha: float, indices: np.ndarray) -> np.array:
-        def get_rank_ci(results):
-            hypotheses_count = results.test_hypotheses(alpha).sum(axis=0)
-            return [hypotheses_count[0], self.model.n_params - hypotheses_count[1] - 1]
-
-        return (
-            np.array([get_rank_ci(self._baseline_comparisons[i]) for i in indices]) + 1
-        )
-
-    def _make_summary_header(self, alpha: float) -> list[str]:
-        return [
-            "rank (conventional)",
-            "pvalue",
-            f"{1-alpha} CI lower",
-            f"{1-alpha} CI upper",
-        ]
-
-
-class MarginalRanking(ConfidenceSet):
-    """Estimate rankings with marginal confidence intervals.
-
-    Subclasses :class:`ConfidenceSet`.
-
-    Examples:
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.confidence_set import MarginalRanking
-
-            x = np.arange(-1, 2)
-            cov = np.diag([1, 2, 3]) / 10
-            model = MarginalRanking(x, cov)
-            results = model.fit()
-            print(results.summary())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-                              Marginal ranking
-            =========================================================
-               rank (conventional) pvalue 0.95 CI lower 0.95 CI upper
-            ---------------------------------------------------------
-            x0               3.000    nan         2.000         3.000
-            x1               2.000    nan         1.000         3.000
-            x2               1.000    nan         1.000         2.000
-            ===============
-            Dep. Variable y
-            ---------------
-
-    """
-
-    _results_cls = MarginalRankingResults
-
-
-class SimultaneousRankingResults(ResultsBase):
-    """Simultaneous ranking results."""
-
-    _default_title = "Simultaneous ranking"
-
-    def __init__(
-        self,
-        model: SimultaneousRanking,
-        *args: Any,
-        n_samples: int = 10000,
-        **kwargs: Any,
-    ):
-        super().__init__(model, *args, **kwargs)
-        self.params = (-model.mean).argsort().argsort() + 1
-        pairwise_model = PairwiseComparison(model.mean, model.cov)
-        self._pairwise_comparison = pairwise_model.fit(n_samples=n_samples)
-
-        # compute test statistics for finding the top tau parameters
-        # self._test_stats is a (# params, # params) matrix where
-        # `self._test_stats[tau, k]`` is the test statistic for the null hypothesis that
-        # the parameter k is not in the top tau parameters
-        indices = np.triu_indices(model.n_params, 1)
-        self._test_stats = np.full((model.n_params, model.n_params), 0.0)
-        test_stats = (
-            self._pairwise_comparison.params / self._pairwise_comparison._std_diagonal
-        )
-        self._test_stats[indices] = -test_stats
-        self._test_stats[(indices[1], indices[0])] = test_stats
-        self._test_stats = np.sort(self._test_stats, 0)[::-1]
-
-        # compute random values to find the critical values for finding the top tau
-        # parameters
-        # self._rvs is a (# samples, # params, # params) matrix where
-        # `self._rvs[n, k, l]`` is the nth sample of the studentized param_k - param_l
-        def reshape(arr):
-            arr = arr[: int(len(arr) / 2)]
-            matrix = np.zeros((model.n_params, model.n_params))
-            matrix[indices] = arr
-            matrix[(indices[1], indices[0])] = -arr
-            return matrix
-
-        self._rvs = np.apply_along_axis(reshape, -1, self._pairwise_comparison._rvs)
-
-    def _conf_int(self, alpha: float, indices: np.ndarray) -> np.ndarray:
-        hypothesis_matrix = self._pairwise_comparison.test_hypotheses(alpha).values
-        return (
-            np.array(
-                [
-                    hypothesis_matrix.sum(axis=1),
-                    self.model.n_params - hypothesis_matrix.sum(axis=0) - 1,
-                ]
-            ).T[indices]
-            + 1
-        )
-
-    def compute_best_params(
-        self, n_best_params: int = 1, alpha: float = 0.05, superset: bool = True
-    ) -> pd.Series:
-        """Compute the set of best (largest) parameters.
-
-        Find the set of parameters such that the truly best ``n_best_params`` parameters
-        are in this set with probability ``1-alpha``. Or, find the set of parameters
-        such that these parameters are in the truly best ``n_best_params`` parameters
-        with probability ``1-alpha``.
-
-        Args:
-            n_best_params (int, optional): Number of best parameters. Defaults to 1.
-            alpha (float, optional): Significance level. Defaults to 0.05.
-            superset (bool, optional): Indicates that the returned set is a superset of
-                the truly best n parameters. If False, the returned set is a subset of
-                the truly best n parameters. Defaults to True.
-
-        Returns:
-            pd.Series: Indicates which parameters are in the selected set.
-        """
-        if superset:
-            test_stats = self._test_stats[n_best_params - 1]
-        else:
-            test_stats = -self._test_stats[n_best_params]
-            n_best_params = self.model.n_params - n_best_params
-
-        subsets = []
-        for indices in combinations(np.arange(self.model.n_params), n_best_params - 1):
-            arr = np.full(self.model.n_params, True)
-            if len(indices) > 0:
-                arr[list(indices)] = False
-
-            subsets.append(arr)
-
-        compute_critical_value = lambda subset: np.quantile(
-            rvs[:, :, subset].max(axis=(1, 2)), 1 - alpha
-        )
-        rejected, newly_rejected = np.full(self.model.n_params, False), None
-        while newly_rejected is None or (newly_rejected.any() and not rejected.all()):
-            rvs = self._rvs[:, ~rejected]
-            critical_value = max([compute_critical_value(subset) for subset in subsets])
-            newly_rejected = (test_stats > critical_value) & ~rejected
-            rejected = newly_rejected | rejected
-
-        return pd.Series(
-            ~rejected if superset else rejected, index=self.model.exog_names
-        )
-
-    def _make_summary_header(self, alpha: float) -> list[str]:
-        return [
-            "rank (conventional)",
-            "pvalue",
-            f"{1-alpha} CI lower",
-            f"{1-alpha} CI upper",
-        ]
-
-
-class SimultaneousRanking(ConfidenceSet):
-    """Estimate rankings with simultaneous confidence intervals.
-
-    Subclasses :class:`ConfidenceSet`.
-
-    Examples:
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.confidence_set import SimultaneousRanking
-
-            x = np.arange(3)
-            cov = np.identity(3) / 10
-            model = SimultaneousRanking(x, cov)
-            results = model.fit()
-            print(results.summary())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-                               Simultaneous ranking
-            =========================================================
-               rank (conventional) pvalue 0.95 CI lower 0.95 CI upper
-            ---------------------------------------------------------
-            x0               3.000    nan         2.000         3.000
-            x1               2.000    nan         1.000         3.000
-            x2               1.000    nan         1.000         2.000
-            ===============
-            Dep. Variable y
-            ---------------
-
-        .. testcode::
-
-            print(results.compute_best_params())
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-            x0    False
-            x1    False
-            x2     True
-            dtype: bool
-
-        This we can be 95% confident that the best (largest) parameter is x2.
-    """
-
-    _results_cls = SimultaneousRankingResults
+"""Simultaneous confidence sets and multiple hypothesis testing.
+
+References:
+
+    .. code-block::
+
+        @article{storey2003statistical,
+            title={Statistical significance for genomewide studies},
+            author={Storey, John D and Tibshirani, Robert},
+            journal={Proceedings of the National Academy of Sciences},
+            volume={100},
+            number={16},
+            pages={9440--9445},
+            year={2003},
+            publisher={National Acad Sciences}
+        }
+
+        @article{romano2005stepwise,
+            title={Stepwise multiple testing as formalized data snooping},
+            author={Romano, Joseph P and Wolf, Michael},
+            journal={Econometrica},
+            volume={73},
+            number={4},
+            pages={1237--1282},
+            year={2005},
+            publisher={Wiley Online Library}
+        }
+
+        @techreport{mogstad2020inference,
+            title={Inference for ranks with applications to mobility across neighborhoods and academic achievement across countries},
+            author={Mogstad, Magne and Romano, Joseph P and Shaikh, Azeem and Wilhelm, Daniel},
+            year={2020},
+            institution={National Bureau of Economic Research}
+        }
+"""
+from __future__ import annotations
+
+import warnings
+from itertools import combinations
+from typing import Any, Sequence, Union
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import seaborn as sns
+from scipy.optimize import minimize
+from scipy.stats import multivariate_normal, norm
+
+from multiple_inference.base import ColumnsType, ModelBase, ResultsBase
+
+
+def _test_hypotheses(
+    z_stat_rvs: np.ndarray,
+    z_stats: np.ndarray,
+    max_rvs: np.ndarray,
+    alpha: float,
+    fast: Union[bool, str],
+) -> np.ndarray:
+    """Perform stepwise hypothesis testing.
+
+    Args:
+        rvs (np.ndarray): (# params, # samples) array of standardized samples from the
+            conventional distribution.
+        z_stats (np.ndarray): ($ params,) array of z statistics.
+        max_rvs (np.ndarray): (# samples,) array of maximum random values.
+        alpha (float): Significance level.
+        fast (Union[bool, str]): If True, do not use the stepwise procedure.
+
+    Raises:
+        ValueError: ``fast`` must be True, False, or "auto".
+
+    Returns:
+        np.ndarray: (# params,) boolean array indicating that hypothesis k was rejected.
+    """
+    if fast not in ("auto", True, False):
+        raise ValueError(f"`fast` must be True, False, or 'auto', got {fast}.")
+
+    if not fast or (fast == "auto" and z_stat_rvs.shape[1] < 10000):
+        # stepwise rejection will take a long time with more than 10000 parameters
+        rejected, newly_rejected = np.full(z_stat_rvs.shape[1], False), None
+        while newly_rejected is None or (newly_rejected.any() and not rejected.all()):
+            critical_value = np.quantile(
+                z_stat_rvs[:, ~rejected].max(axis=1), 1 - alpha
+            )
+            newly_rejected = (z_stats > critical_value) & ~rejected
+            rejected = rejected | newly_rejected
+    else:
+        rejected = z_stats > np.quantile(max_rvs, 1 - alpha)
+
+    return rejected
+
+
+class ConfidenceSetResults(ResultsBase):
+    """Results for simultaneous confidence sets.
+
+    Subclasses :class:`multiple_inference.base.ResultsBase`.
+
+    Args:
+        n_samples (int, optional): Number of samples to draw when approximating the
+            confidence set. Defaults to 10000.
+    """
+
+    _default_title = "Confidence set results"
+
+    def __init__(self, *args: Any, n_samples: int = 10000, **kwargs: Any):
+        super().__init__(*args, **kwargs)
+        self.params = self.model.mean.copy()
+
+        # draw random values for confidence set approximation
+        self._std_diagonal = np.sqrt(self.model.cov.diagonal())
+        self._z_stats = self.params / self._std_diagonal
+        self._z_stat_rvs = (
+            multivariate_normal.rvs(
+                np.zeros(self.model.n_params),
+                self.model.cov,
+                size=n_samples,
+                random_state=self.model.random_state,
+            )
+            / self._std_diagonal
+        )
+        self._max_z_stats = (
+            self._z_stat_rvs.copy()
+            if self.model.n_params == 1
+            else abs(self._z_stat_rvs).max(axis=1)
+        )
+        self._set_pvalues()
+        self._set_qvalues()
+
+    def _set_pvalues(self):
+        if self.model.n_params == 1:
+            self.pvalues = 2 * np.atleast_1d(
+                norm.cdf(-abs(self.model.mean[0]), 0, np.sqrt(self.model.cov[0, 0]))
+            )
+        else:
+            self.pvalues = (
+                np.expand_dims(abs(self._z_stats), -1) < self._max_z_stats
+            ).mean(axis=1)
+
+    def _set_qvalues(self):
+        if self.model.n_params == 1:
+            self.qvalues = self.pvalues.copy()
+        else:
+            # get conventional pvalues
+            pvalues = norm.cdf(self.params / self._std_diagonal)
+            # convert to 2-sided pvalues
+            pvalues = 2 * np.min([pvalues, 1 - pvalues], axis=0)
+            argsort = (-pvalues).argsort()
+            pvalues = pvalues[argsort]
+            # define x over (0, .9 * max pvalue)
+            # extending x too close to the max pvalue introduces noise
+            x = np.linspace(0, 0.9 * pvalues[0])
+            pi0 = (pvalues > np.expand_dims(x, 1)).mean(axis=1) / (1 - x)
+            # fit an exponential smoothing spline to estimate the true null rate
+            spline = lambda x, params: params[0] + params[1] * np.exp(
+                -params[1] * x / params[2]
+            )
+            params = minimize(
+                lambda params: ((spline(x, params) - pi0) ** 2).sum(), [0, 1, 1]
+            ).x
+            true_null_rate = np.clip(spline(pvalues[0], params), 0, 1)
+            # compute qvalues
+            qvalues = [1]
+            for i, pvalue in enumerate(pvalues):
+                qvalues.append(
+                    min(
+                        true_null_rate * pvalue * len(pvalues) / (len(pvalues) - i),
+                        qvalues[-1],
+                    )
+                )
+            self.qvalues = np.array(qvalues[1:])[argsort.argsort()]
+
+    def _conf_int(self, alpha: float, indices: np.ndarray) -> np.ndarray:
+        if self.model.n_params == 1:
+            return np.atleast_2d(
+                norm.ppf(
+                    [alpha / 2, 1 - alpha / 2],
+                    self.model.mean[0],
+                    np.sqrt(self.model.cov[0, 0]),
+                )
+            )
+
+        params = self.params[indices]
+        arr = np.quantile(self._max_z_stats, 1 - alpha) * self._std_diagonal[indices]
+        return np.array([params - arr, params + arr]).T
+
+    def test_hypotheses(
+        self,
+        alpha: float = 0.05,
+        columns: ColumnsType = None,
+        two_tailed: bool = True,
+        fast: Union[bool, str] = "auto",
+    ) -> Union[pd.DataFrame, pd.Series]:
+        """Test the null hypothesis that the parameter is equal to 0.
+
+        Args:
+            alpha (float, optional): Significance level. Defaults to 0.05.
+            columns (ColumnsType, optional): Selected columns. Defaults to None.
+            two_tailed (bool, optional): Run two-tailed hypothesis tests. Set to False
+                to run one-tailed hypothesis tests. Defaults to True.
+            fast (Union[bool, str], optional): Avoid the stepdown procedure. Defaults to
+                "auto".
+
+        Returns:
+            Union[pd.DataFrame, pd.Series]: Results dataframe (if two-tailed) or series
+                (if one-tailed).
+        """
+        # use pvalues to reject hypotheses to control the familywise error rate
+        if two_tailed:
+            rejected = _test_hypotheses(
+                np.hstack([self._z_stat_rvs, -self._z_stat_rvs]),
+                np.concatenate([self._z_stats, -self._z_stats]),
+                self._max_z_stats,
+                alpha,
+                fast,
+            )
+        else:
+            rejected = _test_hypotheses(
+                self._z_stat_rvs,
+                self._z_stats,
+                self._max_z_stats,
+                alpha,
+                fast,
+            )
+
+        indices = self.model.get_indices(columns, self.exog_names)
+        if two_tailed:
+            return pd.DataFrame(
+                rejected.reshape(2, -1).T[indices],
+                columns=["param>0", "param<0"],
+                index=self.exog_names[indices],
+            )
+        return pd.Series(
+            rejected[indices], name="param>0", index=self.exog_names[indices]
+        )
+
+    def _make_summary_header(self, alpha: float) -> list[str]:
+        return [
+            "coef (conventional)",
+            "pvalue",
+            "qvalue",
+            f"{1-alpha} CI lower",
+            f"{1-alpha} CI upper",
+        ]
+
+    def _make_summary_data(
+        self, alpha: float, indices: np.ndarray, **kwargs: Any
+    ) -> np.ndarray:
+        if not hasattr(self, "params"):
+            raise AttributeError("Results object does not have `params` attribute.")
+
+        return np.hstack(
+            (
+                np.array([self.params, self.pvalues, self.qvalues]).T[indices],
+                self.conf_int(alpha, indices, **kwargs),
+            )
+        )
+
+
+class ConfidenceSet(ModelBase):
+    """Model for simultaneous confidence sets.
+
+    Examples:
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.confidence_set import ConfidenceSet
+
+            x = np.arange(-1, 2)
+            cov = np.identity(3) / 10
+            model = ConfidenceSet(x, cov)
+            results = model.fit()
+            print(results.summary())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+            Confidence set results
+            ================================================================
+               coef (conventional) pvalue qvalue 0.95 CI lower 0.95 CI upper
+            ----------------------------------------------------------------
+            x0              -1.000  0.004  0.002        -1.755        -0.245
+            x1               0.000  1.000  1.000        -0.755         0.755
+            x2               1.000  0.004  0.002         0.245         1.755
+            ===============
+            Dep. Variable y
+            ---------------
+
+        .. testcode::
+
+            print(results.test_hypotheses())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+                param>0  param<0
+            x0    False     True
+            x1    False    False
+            x2     True    False
+    """
+
+    _results_cls = ConfidenceSetResults
+
+
+class AverageComparison(ConfidenceSet):
+    """Compare each parameter to the average value across all parameters.
+
+    Subclasses :class:`ConfidenceSet`.
+
+    Args:
+        *args (Any): Passed to :class:`ConfidenceSet`.
+        **kwargs (Any): Passed to :class:`ConfidenceSet`.
+
+    Examples:
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.confidence_set import AverageComparison
+
+            x = np.arange(-1, 2)
+            cov = np.identity(3) / 10
+            model = AverageComparison(x, cov)
+            results = model.fit()
+            print(results.summary())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+                                 Confidence set results                     
+            ================================================================
+               coef (conventional) pvalue qvalue 0.95 CI lower 0.95 CI upper
+            ----------------------------------------------------------------
+            x0              -1.000  0.000  0.000        -1.604        -0.396
+            x1               0.000  1.000  1.000        -0.604         0.604
+            x2               1.000  0.000  0.000         0.396         1.604
+            ===============
+            Dep. Variable y
+            ---------------
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        identity = np.identity(self.n_params)
+        cov_inv = np.linalg.inv(self.cov)
+        projection = (
+            self.X @ np.linalg.inv(self.X.T @ cov_inv @ self.X) @ self.X.T @ cov_inv
+        )
+        self.mean = (identity - projection) @ self.mean
+        cov = (identity - projection) @ self.cov @ (identity - projection).T
+        if np.isnan(cov).all():
+            warnings.warn(
+                f"Error encountered in recomputing covariance matrix. "
+                "Using original covariance matrix instead.",
+                RuntimeWarning,
+            )
+        else:
+            self.cov = cov
+
+
+class BaselineComparison(ConfidenceSet):
+    """Compare parameters to a baseline parameter.
+
+    Subclasses :class:`ConfidenceSet`.
+
+    Args:
+        baseline (Union[int, str]): Index or name of the baseline parameter.
+
+    Examples:
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.confidence_set import BaselineComparison
+
+            x = np.arange(-1, 2)
+            cov = np.identity(3) / 10
+            model = BaselineComparison(x, cov, exog_names=["x0", "x1", "x2"], baseline="x0")
+            results = model.fit()
+            print(results.summary())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+            Confidence set results
+            ================================================================
+               coef (conventional) pvalue qvalue 0.95 CI lower 0.95 CI upper
+            ----------------------------------------------------------------
+            x1               1.000  0.045  0.012         0.022         1.978
+            x2               2.000  0.000  0.000         1.022         2.978
+            ===============
+            Dep. Variable y
+            ---------------
+    """
+
+    def __init__(self, *args, baseline: Union[int, str], **kwargs):
+        super().__init__(*args, **kwargs)
+        index = int(
+            baseline
+            if isinstance(baseline, (float, int))
+            else list(self.exog_names).index(baseline)
+        )
+        self.n_params -= 1
+        self.mean = np.delete(self.mean, index) - self.mean[index]
+        cov = (
+            self.cov[index, index]
+            + self.cov
+            - np.expand_dims(self.cov[index], 1)
+            - np.expand_dims(self.cov[index], 0)
+        )
+        self.cov = np.delete(np.delete(cov, index, axis=0), index, axis=1)
+        if self._exog_names is not None:
+            self.exog_names = np.delete(self.exog_names, index)
+
+
+class PairwiseComparisonResults(ConfidenceSetResults):
+    """Results of pairwise comparisons.
+
+    Subclasses :class:`ConfidenceSetResults`.
+
+    Args:
+        n_samples (int, optional): Number of samples to draw to obtain critical
+            values. Defaults to 10000.
+        groups (np.ndarray, optional): (# params,) array of parameter groups.
+            Defaults to None.
+
+    Raises:
+        ValueError: Length of ``groups`` must match the number of parameters.
+    """
+
+    _default_title = "Pairwise comparisons"
+
+    def __init__(
+        self,
+        *args: Any,
+        n_samples: int = 10000,
+        groups: np.ndarray = None,
+        **kwargs: Any,
+    ):
+        super().__init__(*args, **kwargs)
+        self._groups = (
+            np.zeros(self.model.n_params) if groups is None else np.array(groups)
+        )
+        if len(self._groups) != self.model.n_params:
+            raise ValueError(
+                "Length of groups must equal the number of parameters. Got "
+                f"{self.model.n_params} parameters and groups of length "
+                f" {len(self._groups)}."
+            )
+
+        self._rvs = multivariate_normal.rvs(
+            self.model.mean,
+            self.model.cov,
+            size=n_samples,
+            random_state=self.model.random_state,
+        )
+        self._exog_names, self._params, self._std_diagonal = [], [], []
+        self._max_z_stats = np.full(n_samples, -np.inf)
+        pairwise_groups = []
+        for group in np.unique(self._groups):
+            mask = self._groups == group
+            pairwise_groups += int(0.5 * mask.sum() * (mask.sum() - 1)) * [group]
+            group_exog_names, group_params, group_variance, group_rvs = (
+                self.exog_names[mask],
+                self.params[mask],
+                self.model.cov[mask][:, mask],
+                self._rvs[:, mask],
+            )
+            group_variance_diag = group_variance.diagonal()
+            for i in range(mask.sum()):
+                self._exog_names.append(
+                    [
+                        f"{name} - {group_exog_names[i]}"
+                        for name in group_exog_names[i + 1 :]
+                    ]
+                )
+                self._params.append(group_params[i + 1 :] - group_params[i])
+                # variance of the differences between x_i and x_j
+                self._std_diagonal.append(
+                    np.sqrt(
+                        group_variance_diag[i]
+                        + group_variance_diag[i + 1 :]
+                        - 2 * group_variance[i, i + 1 :]
+                    )
+                )
+                # random sample of the differences between x_i and x_j
+                delta_rvs = group_rvs[:, i + 1 :] - np.expand_dims(group_rvs[:, i], -1)
+                self._max_z_stats = np.hstack(
+                    [
+                        np.expand_dims(self._max_z_stats, -1),
+                        abs(delta_rvs - self._params[-1]) / self._std_diagonal[-1],
+                    ]
+                ).max(axis=1)
+
+        self.exog_names = np.concatenate(self._exog_names)
+        self.params = np.concatenate(self._params)
+        self._std_diagonal = np.concatenate(self._std_diagonal)
+        self._z_stats = self.params / self._std_diagonal
+        self._pairwise_groups = np.array(pairwise_groups)
+        self._set_pvalues()
+        self._set_qvalues()
+
+    def test_hypotheses(
+        self,
+        alpha: float = 0.05,
+        columns: ColumnsType = None,
+        criterion: str = "fwer",
+        groups: Sequence = None,
+        fast: Union[bool, str] = "auto",
+    ) -> Union[pd.DataFrame, dict[Any, pd.DataFrame]]:
+        """Test pairwise hypotheses.
+
+        Args:
+            alpha (float, optional): Significance level. Defaults to .05.
+            columns (ColumnsType, optional): Selected columns. In wide format, these are
+                the original column names (e.g., "x0"). In long format, these are the
+                names of the differences (e.g., "x1 - x0"). Defaults to None.
+            criterion (str, optional): "fwer" to control for the family-wise error rate
+                (using pvalues), "fdr" to control for the false discovery rate (using
+                qvalues). Defaults to "fwer".
+            groups (Sequence, optional). Selected groups of parameters. Defaults to None.
+            fast (Union[bool, str], optional): Indicates to use a fast version of the
+                algorithm. Defaults to "auto".
+
+        Raises:
+            ValueError: ``criterion`` must be one of "fwer" or "fdr".
+
+        Returns:
+            Union[pd.DataFrame, dict[Any, pd.DataFrame]]: Results dataframe if only one
+                group is used, mapping of group name to results dataframe if multiple
+                groups are used.
+
+        Notes:
+            When controlling for the familywise error rate, the null hypotheses are
+            $$mu_k \leq \mu_j$$. When controlling for the false discovery rate, the null
+            hypotheses are $$\mu_k = \mu_j$$.
+        """
+        if criterion not in ("fwer", "fdr"):
+            raise ValueError(f"criterion should be in 'fwer', 'fdr', got {criterion}.")
+
+        if criterion == "fdr":
+            rejected = self.qvalues < alpha
+            rejected = np.vstack([rejected, rejected]).T
+        else:
+            if fast not in ("auto", True, False):
+                raise ValueError(f"`fast` must be True, False, or 'auto', got {fast}.")
+
+            if not fast or (fast == "auto" and self.model.n_params < 100):
+                # stepwise rejection will take a long time with more than 100 pairwise
+                # comparisons
+                rejected = self._stepwise_rejection(alpha)
+            else:
+                critical_value = np.quantile(self._max_z_stats, 1 - alpha)
+                rejected = np.vstack(
+                    [self._z_stats > critical_value, self._z_stats < -critical_value]
+                ).T
+
+        # reshape rejected array into a square matrix
+        return_value = {}
+        for group in groups or np.unique(self._groups):
+            mask = self._groups == group
+            pairwise_mask = self._pairwise_groups == group
+            n_params = mask.sum()
+            tri = np.full((n_params, n_params), False)
+            indices = np.triu_indices(n_params, 1)
+            tri[indices] = rejected[pairwise_mask, 0]
+            tri[(indices[1], indices[0])] = rejected[pairwise_mask, 1]
+
+            exog_names = self.model.exog_names[mask]
+            indices = self.model.get_indices(columns, exog_names)
+            column_names = exog_names[indices]
+            return_value[group] = pd.DataFrame(
+                tri[indices][:, indices], index=column_names, columns=column_names
+            )
+
+        return (
+            list(return_value.values())[0] if len(return_value) == 1 else return_value
+        )
+
+    def _stepwise_rejection(self, alpha: float) -> np.ndarray:
+        # indicates directional hypothesis rejection
+        rejected_pos = np.full(len(self.params), False)
+        rejected_neg = np.full(len(self.params), False)
+        newly_rejected = None
+        while newly_rejected is None or newly_rejected.any():
+            max_z_stats = np.full(len(self._rvs), -np.inf)
+            for group in np.unique(self._groups):
+                # get the parameters, standard errors, and random samples for this group
+                mask = self._groups == group
+                pairwise_mask = self._pairwise_groups == group
+                rvs = self._rvs[:, mask]
+                params = self.params[pairwise_mask]
+                std_diag = self._std_diagonal[pairwise_mask]
+                group_rejected_pos = rejected_pos[pairwise_mask]
+                group_rejected_neg = rejected_neg[pairwise_mask]
+
+                start, stop = 0, mask.sum() - 1
+                for i in range(mask.sum()):
+                    # update max z stats in linearly sized chunks
+                    # this reduces memory complexity from quadratic to linear
+                    # which is important when testing many parameters
+                    delta_rvs = rvs[:, i + 1 :] - np.expand_dims(rvs[:, i], -1)
+                    max_z_stats = np.hstack(
+                        [
+                            np.expand_dims(max_z_stats, 1),
+                            ((delta_rvs - params[start:stop]) / std_diag[start:stop])[
+                                :, ~group_rejected_pos[start:stop]
+                            ],
+                        ]
+                    ).max(axis=1)
+                    max_z_stats = np.hstack(
+                        [
+                            np.expand_dims(max_z_stats, -1),
+                            -((delta_rvs - params[start:stop]) / std_diag[start:stop])[
+                                :, ~group_rejected_neg[start:stop]
+                            ],
+                        ]
+                    ).max(axis=1)
+                    start, stop = stop, stop + (stop - start - 1)
+
+            # compute the critical value and reject hypotheses
+            critical_value = np.quantile(max_z_stats, 1 - alpha)
+            rejected = np.concatenate([rejected_pos, rejected_neg])
+            rejected_pos = self._z_stats > critical_value
+            rejected_neg = self._z_stats < -critical_value
+            newly_rejected = np.concatenate([rejected_pos, rejected_neg]) & ~rejected
+
+        return np.vstack([rejected_pos, rejected_neg]).T
+
+    def hypothesis_heatmap(
+        self,
+        *args: Any,
+        title: str = None,
+        axes=None,
+        triangular: bool = False,
+        **kwargs: Any,
+    ):
+        """Create a heatmap of pairwise hypothesis tests.
+
+        Args:
+            title (str, optional): Title.
+            axes (Union[AxesSubplot, Sequence[AxesSubplot]], optional): Axes to write
+                on. Defaults to None.
+            triangular (bool, optional): Display the results in a triangular (as opposed
+                to square) output. Usually, you should set this to True if and only if
+                your columns are sorted. Defaults to False.
+
+        Returns:
+            np.ndarray: Array of axes.
+        """
+
+        def write_heatmap(group, matrix, ax):
+            if triangular:
+                mask = np.zeros_like(matrix)
+                mask[np.triu_indices_from(mask)] = True
+            else:
+                mask = None
+
+            sns.heatmap(
+                matrix,
+                cbar=False,
+                ax=ax,
+                yticklabels=matrix.index,
+                xticklabels=matrix.columns,
+                mask=mask,
+                square=True,
+                cmap=sns.color_palette()[3:1:-1],
+                center=0.5,
+            )
+            ax.set_title(
+                (title or self.title) + ("" if group is None else f" group = {group}")
+            )
+            ax.set_yticklabels(ax.get_yticklabels(), rotation=0)
+
+        results = self.test_hypotheses(*args, **kwargs)
+        if isinstance(results, dict):
+            if axes is None:
+                fig, axes = plt.subplots(len(results))
+                fig.tight_layout()
+            for (group, matrix), ax in zip(results.items(), axes):
+                write_heatmap(group, matrix, ax)
+        else:
+            if axes is None:
+                _, axes = plt.subplots()
+            write_heatmap(None, results, axes)
+
+        return axes
+
+    def _make_summary_header(self, alpha: float) -> list[str]:
+        return [
+            "delta (conventional)",
+            "pvalue",
+            "qvalue",
+            f"{1-alpha} CI lower",
+            f"{1-alpha} CI upper",
+        ]
+
+
+class PairwiseComparison(ConfidenceSet):
+    """Compute pairwise comparisons.
+
+    Examples:
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.confidence_set import PairwiseComparison
+
+            x = np.arange(-1, 2)
+            cov = np.identity(3) / 10
+            model = PairwiseComparison(x, cov)
+            results = model.fit()
+            print(results.summary())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+            Pairwise comparisons
+            ======================================================================
+                    delta (conventional) pvalue qvalue 0.95 CI lower 0.95 CI upper
+            ----------------------------------------------------------------------
+            x1 - x0                1.000  0.061  0.017        -0.031         2.031
+            x2 - x0                2.000  0.000  0.000         0.969         3.031
+            x2 - x1                1.000  0.061  0.017        -0.031         2.031
+            ===============
+            Dep. Variable y
+            ---------------
+
+        .. testcode::
+
+            print(results.test_hypotheses())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+                   x0     x1     x2
+            x0  False  False   True
+            x1  False  False  False
+            x2  False  False  False
+
+        This means that parameter x2 is significantly greater than x0.
+    """
+
+    _results_cls = PairwiseComparisonResults
+
+
+class MarginalRankingResults(ResultsBase):
+    """Marginal ranking results."""
+
+    _default_title = "Marginal ranking"
+
+    def __init__(
+        self, model: MarginalRanking, *args: Any, n_samples: int = 10000, **kwargs: Any
+    ):
+        super().__init__(model, *args, **kwargs)
+        self.params = (-self.model.mean).argsort().argsort() + 1
+        self._rvs = multivariate_normal.rvs(
+            self.model.mean,
+            self.model.cov,
+            size=n_samples,
+            random_state=self.model.random_state,
+        )
+
+    def _conf_int(
+        self, alpha: float, indices: np.ndarray, fast: Union[bool, str] = "auto"
+    ) -> np.array:
+        def get_rank_ci(index):
+            # get the marginal rank confidence interval for `index`
+            # get random samples for the difference between this index and other parameters
+            rvs = np.delete(
+                self._rvs - np.expand_dims(self._rvs[:, index], 1), index, axis=1
+            )
+            params = np.delete(self.model.mean - self.model.mean[index], index)
+            variance = variance_diag[index] + variance_diag - 2 * self.model.cov[index]
+            std_diagonal = np.sqrt(np.delete(variance, index))
+            z_stats = params / std_diagonal
+
+            # standardize the differences
+            rvs = (rvs - params) / std_diagonal
+            rejected = _test_hypotheses(
+                np.hstack([rvs, -rvs]),
+                np.concatenate([z_stats, -z_stats]),
+                abs(rvs).max(axis=1),
+                alpha,
+                fast,
+            )
+
+            n_params = int(len(rejected) / 2)
+            return [rejected[:n_params].sum(), n_params - rejected[n_params:].sum()]
+
+        variance_diag = self.model.cov.diagonal()
+        return np.array([get_rank_ci(i) for i in indices]) + 1
+
+    def _make_summary_header(self, alpha: float) -> list[str]:
+        return [
+            "rank (conventional)",
+            "pvalue",
+            f"{1-alpha} CI lower",
+            f"{1-alpha} CI upper",
+        ]
+
+
+class MarginalRanking(ConfidenceSet):
+    """Estimate rankings with marginal confidence intervals.
+
+    Subclasses :class:`ConfidenceSet`.
+
+    Examples:
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.confidence_set import MarginalRanking
+
+            x = np.arange(-1, 2)
+            cov = np.diag([1, 2, 3]) / 10
+            model = MarginalRanking(x, cov)
+            results = model.fit()
+            print(results.summary())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+                              Marginal ranking
+            =========================================================
+               rank (conventional) pvalue 0.95 CI lower 0.95 CI upper
+            ---------------------------------------------------------
+            x0               3.000    nan         2.000         3.000
+            x1               2.000    nan         1.000         3.000
+            x2               1.000    nan         1.000         2.000
+            ===============
+            Dep. Variable y
+            ---------------
+
+    """
+
+    _results_cls = MarginalRankingResults
+
+
+class SimultaneousRankingResults(ResultsBase):
+    """Simultaneous ranking results."""
+
+    _default_title = "Simultaneous ranking"
+
+    def __init__(
+        self,
+        model: SimultaneousRanking,
+        *args: Any,
+        n_samples: int = 10000,
+        **kwargs: Any,
+    ):
+        super().__init__(model, *args, **kwargs)
+        self.params = (-model.mean).argsort().argsort() + 1
+        pairwise_model = PairwiseComparison(model.mean, model.cov)
+        self._pairwise_comparison = pairwise_model.fit(n_samples=n_samples)
+
+        # compute test statistics for finding the top tau parameters
+        # self._test_stats is a (# params, # params) matrix where
+        # `self._test_stats[tau, k]`` is the test statistic for the null hypothesis that
+        # the parameter k is not in the top tau parameters
+        indices = np.triu_indices(model.n_params, 1)
+        self._test_stats = np.full((model.n_params, model.n_params), 0.0)
+        self._test_stats[indices] = -self._pairwise_comparison._z_stats
+        self._test_stats[(indices[1], indices[0])] = self._pairwise_comparison._z_stats
+        self._test_stats = np.sort(self._test_stats, 0)[::-1]
+
+    def _conf_int(self, alpha: float, indices: np.ndarray, **kwargs: Any) -> np.ndarray:
+        hypothesis_matrix = self._pairwise_comparison.test_hypotheses(
+            alpha, **kwargs
+        ).values
+        return (
+            np.array(
+                [
+                    hypothesis_matrix.sum(axis=1),
+                    self.model.n_params - hypothesis_matrix.sum(axis=0) - 1,
+                ]
+            ).T[indices]
+            + 1
+        )
+
+    def compute_best_params(
+        self,
+        n_best_params: int = 1,
+        alpha: float = 0.05,
+        superset: bool = True,
+        fast: Union[bool, str] = "auto",
+    ) -> pd.Series:
+        """Compute the set of best (largest) parameters.
+
+        Find the set of parameters such that the truly best ``n_best_params`` parameters
+        are in this set with probability ``1-alpha``. Or, find the set of parameters
+        such that these parameters are in the truly best ``n_best_params`` parameters
+        with probability ``1-alpha``.
+
+        Args:
+            n_best_params (int, optional): Number of best parameters. Defaults to 1.
+            alpha (float, optional): Significance level. Defaults to 0.05.
+            superset (bool, optional): Indicates that the returned set is a superset of
+                the truly best n parameters. If False, the returned set is a subset of
+                the truly best n parameters. Defaults to True.
+            fast (Union[bool, str], optional). Indicates to use a fast version of the
+                selection algorithm. Defaults to "auto".
+
+        Returns:
+            pd.Series: Indicates which parameters are in the selected set.
+        """
+        if not isinstance(fast, bool) and fast != "auto":
+            raise ValueError(f"`fast` must be bool or 'auto', got {fast}.")
+
+        if not fast or (fast == "auto" and self.model.n_params < 100):
+            # perform stepwise rejection algorithm
+            # this will take a long time when testing more than 100 parameters
+            if superset:
+                test_stats = self._test_stats[n_best_params - 1]
+            else:
+                test_stats = -self._test_stats[n_best_params]
+                n_best_params = self.model.n_params - n_best_params
+
+            rejected = self._stepwise_rejection(test_stats, n_best_params, alpha)
+        else:
+            # perform rejections based on confidence intervals
+            conf_int = self.conf_int(alpha)
+            rejected = (
+                conf_int[:, 0] > n_best_params
+                if superset
+                else conf_int[:, 1] <= n_best_params
+            )
+
+        return pd.Series(
+            ~rejected if superset else rejected, index=self.model.exog_names
+        )
+
+    def _stepwise_rejection(
+        self, test_stats: np.ndarray, n_best_params: int, alpha: float
+    ) -> np.ndarray:
+        cov_diag = self.model.cov.diagonal()
+        rejected, newly_rejected = np.full(self.model.n_params, False), None
+        while newly_rejected is None or (newly_rejected.any() and not rejected.all()):
+            # perform stepwise rejection of parameters that cannot be the best
+            max_critical_value = -np.inf
+            for indices_k in combinations(
+                np.arange(self.model.n_params), n_best_params - 1
+            ):
+                # compute maximum critical value over all possible subsets of rejected
+                # hypotheses (indices_k)
+                max_z_stats = np.full(len(self._pairwise_comparison._rvs), -np.inf)
+                subset = np.full(self.model.n_params, True)
+                if len(indices_k) > 0:
+                    subset[list(indices_k)] = False
+
+                for index_j in np.where(~rejected)[0]:
+                    # update max z statistics using the difference between one parameter
+                    # (index_j) # and the rest each iteration
+                    # this reduces memory complexity
+                    subset_j = subset.copy()
+                    subset_j[index_j] = False
+                    delta_rvs = (
+                        np.expand_dims(self._pairwise_comparison._rvs[:, index_j], 1)
+                        - self._pairwise_comparison._rvs[:, subset_j]
+                    )
+                    params = self.model.mean[index_j] - self.model.mean[subset_j]
+                    std = np.sqrt(
+                        cov_diag[index_j]
+                        + cov_diag[subset_j]
+                        - 2 * self.model.cov[index_j, subset_j]
+                    )
+                    max_z_stats = np.hstack(
+                        [np.expand_dims(max_z_stats, 1), (delta_rvs - params) / std]
+                    ).max(axis=1)
+
+                if max_critical_value < (
+                    critical_value := np.quantile(max_z_stats, 1 - alpha)
+                ):
+                    max_critical_value = critical_value
+
+            newly_rejected = (test_stats > max_critical_value) & ~rejected
+            rejected = newly_rejected | rejected
+
+        return rejected
+
+    def _make_summary_header(self, alpha: float) -> list[str]:
+        return [
+            "rank (conventional)",
+            "pvalue",
+            f"{1-alpha} CI lower",
+            f"{1-alpha} CI upper",
+        ]
+
+
+class SimultaneousRanking(ConfidenceSet):
+    """Estimate rankings with simultaneous confidence intervals.
+
+    Subclasses :class:`ConfidenceSet`.
+
+    Examples:
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.confidence_set import SimultaneousRanking
+
+            x = np.arange(3)
+            cov = np.identity(3) / 10
+            model = SimultaneousRanking(x, cov)
+            results = model.fit()
+            print(results.summary())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+                               Simultaneous ranking
+            =========================================================
+               rank (conventional) pvalue 0.95 CI lower 0.95 CI upper
+            ---------------------------------------------------------
+            x0               3.000    nan         2.000         3.000
+            x1               2.000    nan         1.000         3.000
+            x2               1.000    nan         1.000         2.000
+            ===============
+            Dep. Variable y
+            ---------------
+
+        .. testcode::
+
+            print(results.compute_best_params())
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+            x0    False
+            x1    False
+            x2     True
+            dtype: bool
+
+        This we can be 95% confident that the best (largest) parameter is x2.
+    """
+
+    _results_cls = SimultaneousRankingResults
```

### Comparing `multiple-inference-1.1.0/src/multiple_inference/rank_condition.py` & `multiple-inference-1.2.0/src/multiple_inference/rank_condition.py`

 * *Files identical despite different names*

### Comparing `multiple-inference-1.1.0/src/multiple_inference/significance_condition.py` & `multiple-inference-1.2.0/src/multiple_inference/significance_condition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,124 +1,123 @@
-"""Inference for parameters that achieve statistical significance.
-"""
-from __future__ import annotations
-
-from typing import Any, Mapping
-
-import numpy as np
-from multiple_inference.base import ColumnType, ModelBase, ResultsBase
-from multiple_inference.confidence_set import ConfidenceSet
-from multiple_inference.stats import quantile_unbiased
-
-
-class SignificanceConditionResults(ResultsBase):
-    """Quantile-unbiased results.
-
-    Sublcasses :class:`multiple_inference.base.ResultsBase`.
-
-    Args:
-        *args (Any): Passed to :class:`multiple_inference.base.ResultsBase`.
-        marginal_distribution_kwargs (Mapping[str, Any], optional): Passed to
-            :meth:`SignificanceCondition.get_marginal_distribution`. Defaults to None.
-        **kwargs (Any): Passed to :class:`multiple_inference.base.ResultsBase`.
-    """
-
-    _default_title = "Significance condition quantile-unbiased estimates"
-
-    def __init__(
-        self,
-        *args: Any,
-        marginal_distribution_kwargs: Mapping[str, Any] = None,
-        **kwargs: Any,
-    ):
-
-        super().__init__(*args, **kwargs)
-        if marginal_distribution_kwargs is None:
-            marginal_distribution_kwargs = {}
-        self.marginal_distributions, self.params, self.pvalues = [], [], []
-        for i in range(self.model.n_params):
-            dist = self.model.get_marginal_distribution(
-                i, **marginal_distribution_kwargs
-            )
-            self.marginal_distributions.append(dist)
-            self.params.append(dist.ppf(0.5))
-            self.pvalues.append(dist.cdf(0))
-        self.params, self.pvalues = np.array(self.params), np.array(self.pvalues)
-
-    def _make_summary_header(self, alpha: float) -> list[str]:
-        return ["coef (median)", "pvalue (1-sided)", f"[{alpha/2}", f"{1-alpha/2}]"]
-
-
-class SignificanceCondition(ModelBase):
-    """Significance condition quantile-unbiased estimator.
-
-    Subclasses :class:`multiple_inference.base.ModelBase`.
-
-    Examples:
-        Get a quantile-unbiased distribution for x3.
-
-        .. testcode::
-
-            import numpy as np
-            from multiple_inference.significance_condition import SignificanceCondition
-
-            model = SignificanceCondition(np.arange(4), np.identity(4))
-            dist = model.get_marginal_distribution("x3")
-            print(dist.ppf([.025, .5, .975]))
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-            [-0.33936473  1.86862792  4.79906012]
-
-        Display the results.
-
-        .. testcode::
-
-            results = model.fit()
-            print(results.summary(columns=["x3"]))
-
-        .. testoutput::
-            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-            Significance condition quantile-unbiased estimates
-            ===============================================
-                coef (median) pvalue (1-sided) [0.025 0.975]
-            -----------------------------------------------
-            x3         1.869            0.115 -0.339  4.799
-            ===============
-            Dep. Variable y
-            ---------------
-    """
-
-    _results_cls = SignificanceConditionResults
-
-    def __init__(self, *args: Any, **kwargs: Any):
-        super().__init__(*args, **kwargs)
-        self._confidence_set = ConfidenceSet(self.mean, self.cov).fit()
-
-    def get_marginal_distribution(
-        self, column: ColumnType, alpha: float = 0.05, **kwargs: Any
-    ) -> quantile_unbiased:
-        """Get the marginal quantile-unbiased distribution.
-
-        The distribution is quantile-unbiased conditional on the parameter being
-        statistically significant at level ``alpha``.
-
-        Args:
-            column (ColumnType): Selected column.
-            alpha (float, optional): Significance level. Defaults to .05.
-
-        Returns:
-            quantile_unbiased: Quantile-unbiased distribution.
-        """
-        index = self.get_index(column)
-        critical_value = (
-            self._confidence_set.conf_int(alpha, [index]) - self.mean[index]
-        )[0, 1]
-        truncation_set = [[-np.inf, -critical_value], [critical_value, np.inf]]
-        return quantile_unbiased(
-            y=self.mean[index],
-            scale=np.sqrt(self.cov[index, index]),
-            truncation_set=truncation_set,
-            **kwargs,
-        )
+"""Inference for parameters that achieve statistical significance.
+"""
+from __future__ import annotations
+
+from typing import Any, Mapping
+
+import numpy as np
+from multiple_inference.base import ColumnType, ModelBase, ResultsBase
+from multiple_inference.confidence_set import ConfidenceSet
+from multiple_inference.stats import quantile_unbiased
+
+
+class SignificanceConditionResults(ResultsBase):
+    """Quantile-unbiased results.
+
+    Sublcasses :class:`multiple_inference.base.ResultsBase`.
+
+    Args:
+        *args (Any): Passed to :class:`multiple_inference.base.ResultsBase`.
+        marginal_distribution_kwargs (Mapping[str, Any], optional): Passed to
+            :meth:`SignificanceCondition.get_marginal_distribution`. Defaults to None.
+        **kwargs (Any): Passed to :class:`multiple_inference.base.ResultsBase`.
+    """
+
+    _default_title = "Significance condition quantile-unbiased estimates"
+
+    def __init__(
+        self,
+        *args: Any,
+        marginal_distribution_kwargs: Mapping[str, Any] = None,
+        **kwargs: Any,
+    ):
+        super().__init__(*args, **kwargs)
+        if marginal_distribution_kwargs is None:
+            marginal_distribution_kwargs = {}
+        self.marginal_distributions, self.params, self.pvalues = [], [], []
+        for i in range(self.model.n_params):
+            dist = self.model.get_marginal_distribution(
+                i, **marginal_distribution_kwargs
+            )
+            self.marginal_distributions.append(dist)
+            self.params.append(dist.ppf(0.5))
+            self.pvalues.append(dist.cdf(0))
+        self.params, self.pvalues = np.array(self.params), np.array(self.pvalues)
+
+    def _make_summary_header(self, alpha: float) -> list[str]:
+        return ["coef (median)", "pvalue (1-sided)", f"[{alpha/2}", f"{1-alpha/2}]"]
+
+
+class SignificanceCondition(ModelBase):
+    """Significance condition quantile-unbiased estimator.
+
+    Subclasses :class:`multiple_inference.base.ModelBase`.
+
+    Examples:
+        Get a quantile-unbiased distribution for x3.
+
+        .. testcode::
+
+            import numpy as np
+            from multiple_inference.significance_condition import SignificanceCondition
+
+            model = SignificanceCondition(np.arange(4), np.identity(4))
+            dist = model.get_marginal_distribution("x3")
+            print(dist.ppf([.025, .5, .975]))
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+            [-0.33936473  1.86862792  4.79906012]
+
+        Display the results.
+
+        .. testcode::
+
+            results = model.fit()
+            print(results.summary(columns=["x3"]))
+
+        .. testoutput::
+            :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+            Significance condition quantile-unbiased estimates
+            ===============================================
+                coef (median) pvalue (1-sided) [0.025 0.975]
+            -----------------------------------------------
+            x3         1.869            0.115 -0.339  4.799
+            ===============
+            Dep. Variable y
+            ---------------
+    """
+
+    _results_cls = SignificanceConditionResults
+
+    def __init__(self, *args: Any, **kwargs: Any):
+        super().__init__(*args, **kwargs)
+        self._confidence_set = ConfidenceSet(self.mean, self.cov).fit()
+
+    def get_marginal_distribution(
+        self, column: ColumnType, alpha: float = 0.05, **kwargs: Any
+    ) -> quantile_unbiased:
+        """Get the marginal quantile-unbiased distribution.
+
+        The distribution is quantile-unbiased conditional on the parameter being
+        statistically significant at level ``alpha``.
+
+        Args:
+            column (ColumnType): Selected column.
+            alpha (float, optional): Significance level. Defaults to .05.
+
+        Returns:
+            quantile_unbiased: Quantile-unbiased distribution.
+        """
+        index = self.get_index(column)
+        critical_value = (
+            self._confidence_set.conf_int(alpha, [index]) - self.mean[index]
+        )[0, 1]
+        truncation_set = [[-np.inf, -critical_value], [critical_value, np.inf]]
+        return quantile_unbiased(
+            y=self.mean[index],
+            scale=np.sqrt(self.cov[index, index]),
+            truncation_set=truncation_set,
+            **kwargs,
+        )
```

### Comparing `multiple-inference-1.1.0/src/multiple_inference/stats.py` & `multiple-inference-1.2.0/src/multiple_inference/stats.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,669 +1,717 @@
-"""Statistical distributions.
-"""
-from __future__ import annotations
-
-import warnings
-from typing import Any, Callable, List, Sequence, Tuple, Union
-
-import numpy as np
-from scipy.integrate import quad
-from scipy.interpolate import interp1d
-from scipy.misc import derivative
-from scipy.optimize import NonlinearConstraint, fsolve, minimize
-from scipy.stats import norm, rv_continuous, truncnorm as truncnorm_base
-
-
-from .base import Numeric1DArray
-from .utils import weighted_quantile
-
-
-class joint_distribution:
-    """Join distribution based on independent marginal distributions.
-
-    Args:
-        marginal_distributions (Sequence[rv_continuous]): Marginal distributions.
-    """
-
-    def __init__(self, marginal_distributions: Sequence[rv_continuous]):
-        self._marginal_distributions = list(marginal_distributions)
-
-    def logpdf(self, x: np.ndarray) -> np.ndarray:
-        """Log of the probability density function evaluated at ``x``.
-
-        Args:
-            x (np.ndarray): (n, # marginals) matrix of values at which to evaluate the
-                density function.
-
-        Returns:
-            np.ndarray: (n,) array of log density.
-        """
-        x = np.array(x).reshape(-1, len(self._marginal_distributions))
-        return np.sum(
-            [dist.logpdf(x_i) for dist, x_i in zip(self._marginal_distributions, x.T)],
-            axis=0,
-        )
-
-    def pdf(self, x: np.ndarray) -> np.ndarray:
-        """Probability density function evaluated at ``x``.
-
-        Args:
-            x (np.ndarray): (n, # marginals) matrix of values at which to evaluate the
-                density function.
-
-        Returns:
-            np.ndarray: (n,) array of densities.
-        """
-        return np.exp(self.logpdf(x))
-
-    def rvs(self, size: int = 1) -> np.ndarray:
-        """Sample random values.
-
-        Args:
-            size (int, optional): Number of samples to draw. Defaults to 1.
-
-        Returns:
-            np.ndarray: (size, # marginals) matrix of samples.
-        """
-        return np.vstack(
-            [dist.rvs(size=size) for dist in self._marginal_distributions]
-        ).T
-
-
-class mixture(rv_continuous):
-    """Mixture distribution.
-
-    Args:
-        distributions (list[rv_continuous]): List of n distributions to mix over.
-        weights (Numeric1DArray, optional): (n,) array of mixture weights. Defaults to None.
-
-    Attributes:
-        distributions (list[rv_continuous]): Distributions to mix over.
-        weights (np.ndarray): Mixture weights.
-    """
-
-    def __init__(
-        self,
-        distributions: list[rv_continuous],
-        weights: Numeric1DArray = None,
-        **kwargs: Any,
-    ):
-
-        super().__init__(**kwargs)
-        self.distributions = distributions
-        self.weights = (
-            np.ones(len(distributions)) if weights is None else np.atleast_1d(weights)
-        )
-        self.weights /= self.weights.sum()
-
-    def _pdf(self, x):
-        return (
-            self.weights * np.array([dist.pdf(x) for dist in self.distributions]).T
-        ).sum(axis=1)
-
-    def _cdf(self, x):
-        return (
-            self.weights * np.array([dist.cdf(x) for dist in self.distributions]).T
-        ).sum(axis=1)
-
-    def mean(self):
-        return (
-            self.weights * np.array([dist.mean() for dist in self.distributions])
-        ).sum()
-
-    def var(self):
-        return (
-            self.weights * np.array([dist.var() for dist in self.distributions])
-        ).sum()
-
-    def std(self):
-        return np.sqrt(self.var())
-
-
-class nonparametric(rv_continuous):
-    """Nonparametric distribution.
-
-    Args:
-        values (tuple[np.array, np.array]): (n,) array of x values, (n,) array of the
-            probability mass function evaluated at x.
-        kind (str, optional): Type of interpolation to use. Passed to
-            ``scipy.interpolate.interp1d``. Defaults to None.
-
-    Attributes:
-        xk (np.ndarray): (n,) array of x values.
-        pk (np.ndarray): (n,) array of the probability mass function evaluated at x.
-
-    Notes:
-        This distribution interpolates between the probability mass function to
-        "continuize" the discrete function.
-    """
-
-    def __init__(self, values, kind=None, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.xk, self.pk = np.array(values[0], float), np.array(values[1], float)
-        self.pk /= self.pk.sum()
-        self._cdf_values = np.cumsum(self.pk)
-        if kind is not None:
-            self._kind = kind
-        else:
-            self._kind = "cubic" if len(self.xk) > 3 else "linear"
-        self._scale = 1
-        self._scale = 1 / quad(self._pdf, self.xk[0], self.xk[-1])[0]
-
-    def _pdf(self, x: np.ndarray) -> np.ndarray:
-        x = np.atleast_1d(x)
-        pdf = np.zeros(len(x))
-        in_range = (self.xk[0] < x) & (x < self.xk[-1])
-        pdf[in_range] = interp1d(self.xk, self.pk, kind=self._kind)(x[in_range])
-        return self._scale * pdf
-
-    def _cdf(self, x: np.ndarray) -> np.ndarray:
-        x = np.atleast_1d(x)
-        cdf = np.zeros(len(x))
-        cdf[x >= self.xk[-1]] = 1
-        in_range = (self.xk[0] < x) & (x < self.xk[-1])
-        cdf[in_range] = interp1d(self.xk, self._cdf_values, kind=self._kind)(
-            x[in_range]
-        )
-        return cdf
-
-    def _ppf(self, q: np.ndarray) -> np.ndarray:
-        return weighted_quantile(self.xk, q, self.pk)
-
-    def moment(self, func: Callable[[np.ndarray], np.ndarray]) -> float:
-        """Compute a moment.
-
-        Args:
-            func (Callable[[np.ndarray], np.ndarray]): Moment function that takes
-                ``self.xk`` and returns an array of the same shape.
-
-        Returns:
-            float: Moment.
-        """
-        return sum(self.pk * func(self.xk))
-
-    def mean(self) -> float:
-        """Compute the mean.
-
-        Returns:
-            float: Mean.
-        """
-        return self.moment(lambda x: x)
-
-    def var(self) -> float:
-        """Compute the variance.
-
-        Returns:
-            float: Variance.
-        """
-        mean = self.mean()
-        return self.moment(lambda x: (x - mean) ** 2)
-
-    def std(self) -> float:
-        """Compute the standard deviation.
-
-        Returns:
-            float: Standard deviation.
-        """
-        return np.sqrt(self.var())
-
-
-class quantile_unbiased(rv_continuous):  # pylint: disable=invalid-name
-    """Conditional quantile-unbiased distribution.
-
-    Inherits from `scipy.stats.rv_continuous <https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_continuous.html>`_
-    and handles standard public methods (``pdf``, ``cdf``, etc.).
-
-    Args:
-        y (float): Value at which the truncated CDF is evaluated
-        projection_interval (Union[float, Tuple[float, float]], optional): Lower and
-            upper bounds of the projection confidence interval. Defaults to
-            (-np.inf, np.inf).
-        bounds (Tuple[float, float], optional): Lower and upper bounds of the support
-            of the distribution. Defaults to (-np.inf, np.inf).
-        dx (float): Used to numerically approximate the PDF.
-        **truncnorm_kwargs (Any): Keyword arguments for :class:`truncnorm`.
-
-    Attributes:
-        y (float): Value at which the truncated CDF is evaluated.
-        bounds (Tuple[float, float]): Lower and upper bound of the support of the
-            distribution.
-        dx (float): Used to numerically approximate the PDF.
-        truncnorm_kwargs (dict): Keyword arguments for :class:`truncnorm`.
-
-    Examples:
-        Compute a median-unbiased estimate of a normally distributed variable given
-            that its observed value is 1 and falls between 0 and 3.
-
-        .. doctest::
-
-            >>> from multiple_inference.stats import quantile_unbiased
-            >>> dist = quantile_unbiased(1, truncation_set=[(0, 3)])
-            >>> dist.ppf(.5)
-            0.7108033900602351
-    """
-
-    def __init__(
-        self,
-        y: float,
-        projection_interval: Union[float, Tuple[float, float]] = (-np.inf, np.inf),
-        bounds: Tuple[float, float] = (-np.inf, np.inf),
-        dx: float = None,
-        **truncnorm_kwargs: Any,
-    ):
-        super().__init__()
-        self.y = y  # pylint: disable=invalid-name
-        if np.isscalar(projection_interval):
-            projection_interval = abs(projection_interval)  # type: ignore
-            projection_interval = (-projection_interval, projection_interval)
-        self.projection_interval = tuple(projection_interval)
-        self.bounds = bounds
-        self.truncnorm_kwargs = truncnorm_kwargs
-        self.dx = dx
-
-        self._cdf_min: float = (
-            0  # type: ignore
-            if bounds[0] == -np.inf
-            else 1 - self._truncated_cdf(np.array([bounds[0]]))
-        )
-        if self._cdf_min >= 1:
-            warnings.warn(
-                "Untruncated CDF of lower bound == 1: try decreasing the lower bound",
-                RuntimeWarning,
-            )
-        self._cdf_max: float = (
-            1  # type: ignore
-            if bounds[1] == np.inf
-            else 1 - self._truncated_cdf(np.array([bounds[1]]))
-        )
-        if self._cdf_max <= 0:
-            warnings.warn(
-                "Untruncated CDF of upper bound == 0: try increasing the upper bound",
-                RuntimeWarning,
-            )
-
-    @property
-    def dx(self):  # pylint: disable=missing-docstring
-        # create a default dx value if this property has not yet been set
-        if self._dx is None:
-            self.dx = np.diff(self.ppf([0.95, 0.05])) / 50
-        return self._dx
-
-    @dx.setter
-    def dx(self, value):
-        self._dx = value
-
-    @property
-    def bounds(self):  # pylint: disable=missing-docstring
-        # Potentially restrict the bounds of this distribution to ensure the truncation
-        # set and # projection interval overlap
-        truncation_set = self.truncnorm_kwargs.get("truncation_set")
-        if truncation_set is None or self.projection_interval == (-np.inf, np.inf):
-            return self._bounds
-
-        a, b = zip(*truncation_set)  # pylint: disable=invalid-name
-        return (
-            max(self._bounds[0], np.min(a) - self.projection_interval[1]),
-            min(self._bounds[1], np.max(b) - self.projection_interval[0]),
-        )
-
-    @bounds.setter
-    def bounds(self, bounds):
-        self._bounds = bounds
-
-    def _truncated_cdf(  # pylint: disable=invalid-name
-        self, x: np.ndarray
-    ) -> np.ndarray:
-        """Compute the truncated CDF evaluated at ``self.y`` with shift ``x``."""
-
-        def truncated_cdf(x_i):
-            # get the intersection of the truncation set and the projection confidence
-            # interval centered on x_i
-            intersection = []
-            for interval in truncation_set:
-                clipped_interval = (
-                    float(max(interval[0], x_i + self.projection_interval[0])),
-                    float(min(interval[1], x_i + self.projection_interval[1])),
-                )
-                if clipped_interval[0] < clipped_interval[1]:
-                    interval = (
-                        normalize(clipped_interval[0], x_i),
-                        normalize(clipped_interval[1], x_i),
-                    )
-                    intersection.append(interval)
-
-            return truncnorm(intersection, loc=x_i, **truncnorm_kwargs).cdf(self.y)
-
-        def normalize(value, loc):
-            return (value - loc) / scale
-
-        truncation_set = self.truncnorm_kwargs.get("truncation_set")
-        scale = self.truncnorm_kwargs.get("scale", 1)
-        truncnorm_kwargs = {
-            key: value
-            for key, value in self.truncnorm_kwargs.items()
-            if key != "truncation_set"
-        }
-        rval = np.array([truncated_cdf(x_i) for x_i in x])
-        return rval[0] if len(rval) == 1 else rval
-
-    def _cdf(self, x: np.ndarray) -> np.ndarray:  # pylint: disable=arguments-differ
-        """Cumulative distribution function.
-
-        Args:
-            x (np.ndarray): (n,) array of values at which to evaluate the CDF.
-
-        Returns:
-            np.ndarray: (n,) array of evaluations.
-        """
-        if self._cdf_min >= 1 or self._cdf_max <= 0:
-
-            def handle_cdf_out_of_bounds(x_i):
-                return self.bounds[0] <= x_i if self.y < x_i else self.bounds[1] < x_i
-
-            warnings.warn(
-                "Untruncated CDF of lower bound >= 1 or CDF of upper bound <= 0"
-            )
-            return np.array([handle_cdf_out_of_bounds(x_i) for x_i in x]).astype(float)
-
-        cdf = (1 - self._truncated_cdf(x) - self._cdf_min) / (
-            self._cdf_max - self._cdf_min
-        )
-        return ((self.bounds[0] < x) & (x < self.bounds[1])) * cdf + (
-            self.bounds[1] <= x
-        ).astype(float)
-
-    def _pdf(self, x: np.ndarray) -> np.ndarray:  # pylint: disable=arguments-differ
-        """Probability density function.
-
-        Args:
-            x (np.ndarray): (n,) array of values at which to evaluate the PDF.
-
-        Returns:
-            np.ndarray: (n,) array of evaluations.
-        """
-        pdf = derivative(self._cdf, x, dx=self.dx, order=5)
-        return ((self.bounds[0] < x) & (x < self.bounds[1])) * pdf
-
-    def _ppf(self, q: np.ndarray) -> np.ndarray:  # pylint: disable=arguments-differ
-        """See self.ppf."""
-
-        def func(mu, q_i):
-            return self._truncated_cdf(mu) - (1 - q_i)
-
-        if self._cdf_min >= 1 or self._cdf_max <= 0:
-            warnings.warn(
-                "Untruncated CDF of lower bound >= 1 or CDF of upper bound <= 0"
-            )
-
-            value = self.bounds[0] if self.bounds[0] > self.y else self.bounds[1]
-            return np.full(q.shape, value)
-
-        q_t = np.atleast_1d(q) * (self._cdf_max - self._cdf_min) + self._cdf_min
-        return np.array([fsolve(func, [self.y], args=(q_i,))[0] for q_i in q_t])
-
-    def ppf(  # pylint: disable=arguments-differ
-        self, q: Union[float, Numeric1DArray]
-    ) -> np.ndarray:
-        """Percent point function.
-
-        Args:
-            q (np.ndarray): (n,) array of quantiles at which to evaluate the PPF.
-
-        Returns:
-            np.ndarray: (n,) array of evaluations.
-        """
-        return np.clip(super().ppf(q), *self.bounds)
-
-
-class truncnorm(rv_continuous):  # pylint: disable=invalid-name
-    """Truncated normal distribution.
-
-    Inherits from `scipy.stats.rv_continuous <https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_continuous.html>`_
-    and handles standard public methods (``pdf``, ``cdf``, etc.).
-
-    This uses the `exponential tilting <https://ieeexplore.ieee.org/document/7408180>`_
-    approximation method.
-
-    Args:
-        truncation_set (List[Tuple[float, float]], optional): List of truncation
-            intervals, e.g., ``[(-1, 0), (1, 2)]`` truncates the distribution to
-            [-1, 0] union [1, 2]. Defaults to None.
-        loc (float, optional): Location. Defaults to 0.
-        scale (float, optional): Scale parameter. Defaults to 1.
-        n_samples (int, optional): Number of samples to draw for approximation.
-            Defaults to 10000.
-        seed (int, optional): Random seed. Defaults to 0.
-
-    Attributes:
-        loc (float): Location parameter.
-        scale (float): Scale parameter.
-        lower_bound (np.array): (# intervals,) array of lower bounds of the truncation
-            intervals.
-        upper_bound (np.array): (# intervals,) array of upper bounds of the truncation
-            intervals.
-        interval_masses (np.array): (# intervals,) array of the amount of mass in each
-            truncation interval.
-        n_samples (int): Number of samples to draw for approximation. Defaults to
-            10000.
-
-    Examples:
-        Let's evaluate the CDF of a standard normal truncated to the interval $(-1, 0)$ at -0.5.
-
-        .. testcode::
-
-            from multiple_inference.stats import truncnorm
-            print(truncnorm([(-1, 0)]).cdf(-.5))
-
-        .. testoutput::
-
-            0.4390935748119969
-
-        Let's evaluate the CDF of a standard normal truncated to the interval $(-1, 0) \cup (1, 2)$ at -0.5.
-
-        .. testcode::
-
-            from multiple_inference.stats import truncnorm
-            print(truncnorm([(-1, 0), (1, 2)]).cdf(-.5))
-
-        .. testoutput::
-
-            0.3140541146849627
-
-    Note:
-        The truncation set is defined over the domain of the standard normal. To
-        convert the truncation set for a specific mean and standard deviation, use:
-
-        .. code-block:: python
-
-            >>> truncation_set = [(myclip_a - my_mean) / my_std, (myclip_b - my_mean) / my_std)]
-    """
-
-    def __init__(
-        self,
-        truncation_set: List[Tuple[float, float]] = None,
-        loc: float = 0,
-        scale: float = 1,
-        n_samples: int = 10000,
-        seed: int = 0,
-    ):
-
-        self.seed = seed
-        self.loc = loc
-        self.scale = scale
-        self.n_samples = n_samples
-        if truncation_set is None:
-            truncation_set = [(-np.inf, np.inf)]
-        self.lower_bound, self.upper_bound = self._get_truncation_bounds(truncation_set)
-        self.interval_masses = np.array(
-            [
-                self._compute_mass_in_interval_avg(a, b)
-                for a, b in zip(self.lower_bound, self.upper_bound)
-            ]
-        )
-        super().__init__()
-
-    def _pdf(self, x):  # pylint: disable=arguments-differ
-        x = self._normalize(x)
-        # n x 1 indicator that x is in an interval
-        in_interval = np.array(
-            [np.any((self.lower_bound <= x_i) & (x_i <= self.upper_bound)) for x_i in x]
-        )
-        return in_interval * norm.pdf(x) / (self.scale * self.interval_masses.sum())
-
-    def _logpdf(self, x):  # pylint: disable=arguments-differ
-        x = self._normalize(x)
-        # n x 1 indicator that x is in an interval
-        in_interval = np.array(
-            [np.any((self.lower_bound <= x_i) & (x_i <= self.upper_bound)) for x_i in x]
-        )
-        logpdf = (
-            norm.logpdf(x) - np.log(self.scale) - np.log(self.interval_masses.sum())
-        )
-        logpdf[~in_interval] = -np.inf
-        return logpdf
-
-    def _cdf(self, x):  # pylint: disable=arguments-differ
-        x = self._normalize(x)
-
-        if self.lower_bound.size == self.upper_bound.size == 0:
-            # i.e., truncation set is empty
-            return (x > 0).astype(float)
-
-        denominator = self.interval_masses.sum()
-        if denominator == 0:
-            # converts cdf to 0 or 1 depending on bounds and x
-            a = self.lower_bound.min()
-            b = self.upper_bound.max()
-            convert_0_1 = lambda x_i: a < x_i if x_i > 0 else b < x_i
-            return np.array([convert_0_1(x_i) for x_i in x]).astype(float)
-
-        return np.clip(self._compute_cdf_numerator(x) / denominator, 0, 1)
-
-    def _logcdf(self, x):  # pylint: disable=arguments-differ
-        x = self._normalize(x)
-        denominator = self.interval_masses.sum()
-        return np.log(self._compute_cdf_numerator(x)) - np.log(denominator)
-
-    def _compute_mass_in_interval_avg(self, a, b):
-        # compute the amount of mass in the interval [a, b] by averaging approximate
-        # mass in [a, b] and [-b, -a]
-        # the amount of mass in these intervals is the same because the normal is symmetric
-        # this can improve performance
-        arr = [
-            self._compute_mass_in_interval(a, b, int(self.n_samples / 2)),
-            self._compute_mass_in_interval(-b, -a, int(self.n_samples / 2)),
-        ]
-        return np.mean(arr, where=~np.isnan(arr))
-
-    def _compute_mass_in_interval(self, a, b, n_samples=None):
-        # compute the amount of mass in the interval [a, b] using minimax exponential tilt
-        def compute_psi(params):
-            x, mu = params
-            return -x * mu + (0.5 * mu ** 2 + np.log(norm.cdf(b, mu) - norm.cdf(a, mu)))
-
-        def d_psi_d_mu(params):
-            # derivative of psi with respect to mu
-            x, mu = params
-            return (
-                -x
-                + mu
-                + (norm.pdf(b, mu) - norm.pdf(a, mu))
-                / ((norm.cdf(b, mu) - norm.cdf(a, mu)))
-            )
-
-        def optimize_params(x0):
-            # maximize psi subject to x being contained in the interval and the
-            # derivative of psi wrt mu =0 0
-            derivative_constraint = NonlinearConstraint(d_psi_d_mu, 0, 0)
-            return minimize(
-                lambda x: -compute_psi(x),
-                x0=x0,
-                bounds=[(a, b), (-np.inf, np.inf)],
-                constraints=[derivative_constraint],
-            )
-
-        def compute_tilting_param():
-            # compute the optimal tilting parameter
-            try:
-                # initial guess for x, denoted as Psi in the paper
-                # in the univariate case, the initial guess for mu is 0
-                x_init = (norm.pdf(a) - norm.pdf(b)) / ((norm.cdf(b) - norm.cdf(a)))
-            except ZeroDivisionError:
-                x_init = a if a < 0 else b
-
-            if a < x_init < b:
-                # optimal x is in the truncation set, so optimal mu is 0
-                return 0
-
-            # optimal mu must be found by non-linear optimization
-            res = optimize_params([x_init, 0])
-            if res.success:
-                return res.x[1]
-            next_guess, final_guess = ([a, a], [b, b]) if a > 0 else ([b, b], [a, a])
-            res = optimize_params(next_guess)
-            if res.success:
-                return res.x[1]
-            res = optimize_params(final_guess)
-            if res.success:
-                return res.x[1]
-            warnings.warn(
-                "Optimizer failed to find truncated normal tilt parameter",
-                RuntimeWarning,
-            )
-            return x_init
-
-        if b < a:
-            return 0
-        mu = compute_tilting_param()
-        x = truncnorm_base.rvs(
-            a - mu, b - mu, mu, size=n_samples or self.n_samples, random_state=self.seed
-        )
-        return np.exp(compute_psi((x, mu))).mean()
-
-    def _compute_cdf_numerator(self, x):
-        # n x p indicates x is above the upper bound of the interval
-        index = np.array([self.upper_bound <= x_i for x_i in x])
-        # n x 1 CDF for the intervals where x is above the upper bound
-        cdf = index @ self.interval_masses
-
-        # tuple of (x index, interval index) such that x[x index] is in interval[interval_index]
-        indices = np.where(
-            [(self.lower_bound < x_i) & (x_i < self.upper_bound) for x_i in x]
-        )
-        # add mass from intervals containing x
-        cdf[indices[0]] += np.array(
-            [
-                self._compute_mass_in_interval_avg(
-                    self.lower_bound[interval_index], x[x_index]
-                )
-                for x_index, interval_index in zip(*indices)
-            ]
-        )
-
-        return cdf
-
-    def _get_truncation_bounds(self, truncation_set):
-        if not truncation_set:
-            return np.array([]), np.array([])
-
-        for interval in truncation_set:
-            if interval[1] < interval[0]:
-                raise ValueError(f"Invalid interval {interval}")
-
-        truncation_set.sort(key=lambda x: x[0])
-        a, b = list(zip(*truncation_set))
-
-        # ensure b is strictly increasing
-        b = [b[0]] + [max(b_i, b_j) for b_i, b_j in zip(b[1:], b[:-1])]
-
-        new_a, new_b = [a[0]], []
-        for a_i, b_i in zip(a[1:], b[:-1]):
-            if a_i > b_i:
-                new_b.append(b_i)
-                new_a.append(a_i)
-        new_b.append(b[-1])
-
-        return np.array(new_a), np.array(new_b)
-
-    def _normalize(self, arr):
-        return (arr - self.loc) / self.scale
+"""Statistical distributions.
+"""
+from __future__ import annotations
+
+import warnings
+from typing import Any, Callable, List, Sequence, Tuple, Union
+
+import numpy as np
+from scipy.integrate import quad
+from scipy.interpolate import CubicSpline, PchipInterpolator
+from scipy.misc import derivative
+from scipy.optimize import NonlinearConstraint, fsolve, minimize, minimize_scalar
+from scipy.stats import norm, rv_continuous, truncnorm as truncnorm_base
+
+
+from .base import Numeric1DArray
+from .utils import weighted_quantile
+
+
+class joint_distribution:
+    """Join distribution based on independent marginal distributions.
+
+    Args:
+        marginal_distributions (Sequence[rv_continuous]): Marginal distributions.
+    """
+
+    def __init__(self, marginal_distributions: Sequence[rv_continuous]):
+        self._marginal_distributions = list(marginal_distributions)
+
+    def logpdf(self, x: np.ndarray) -> np.ndarray:
+        """Log of the probability density function evaluated at ``x``.
+
+        Args:
+            x (np.ndarray): (n, # marginals) matrix of values at which to evaluate the
+                density function.
+
+        Returns:
+            np.ndarray: (n,) array of log density.
+        """
+        x = np.array(x).reshape(-1, len(self._marginal_distributions))
+        return np.sum(
+            [dist.logpdf(x_i) for dist, x_i in zip(self._marginal_distributions, x.T)],
+            axis=0,
+        )
+
+    def pdf(self, x: np.ndarray) -> np.ndarray:
+        """Probability density function evaluated at ``x``.
+
+        Args:
+            x (np.ndarray): (n, # marginals) matrix of values at which to evaluate the
+                density function.
+
+        Returns:
+            np.ndarray: (n,) array of densities.
+        """
+        return np.exp(self.logpdf(x))
+
+    def rvs(self, size: int = 1) -> np.ndarray:
+        """Sample random values.
+
+        Args:
+            size (int, optional): Number of samples to draw. Defaults to 1.
+
+        Returns:
+            np.ndarray: (size, # marginals) matrix of samples.
+        """
+        return np.vstack(
+            [dist.rvs(size=size) for dist in self._marginal_distributions]
+        ).T
+
+
+class mixture(rv_continuous):
+    """Mixture distribution.
+
+    Args:
+        distributions (list[rv_continuous]): List of n distributions to mix over.
+        weights (Numeric1DArray, optional): (n,) array of mixture weights. Defaults to None.
+
+    Attributes:
+        distributions (list[rv_continuous]): Distributions to mix over.
+        weights (np.ndarray): Mixture weights.
+    """
+
+    def __init__(
+        self,
+        distributions: list[rv_continuous],
+        weights: Numeric1DArray = None,
+        **kwargs: Any,
+    ):
+        super().__init__(**kwargs)
+        self.distributions = distributions
+        self.weights = (
+            np.ones(len(distributions)) if weights is None else np.atleast_1d(weights)
+        )
+        self.weights /= self.weights.sum()
+
+    def _pdf(self, x):
+        return (
+            self.weights * np.array([dist.pdf(x) for dist in self.distributions]).T
+        ).sum(axis=1)
+
+    def _cdf(self, x):
+        return (
+            self.weights * np.array([dist.cdf(x) for dist in self.distributions]).T
+        ).sum(axis=1)
+
+    def mean(self):
+        return (
+            self.weights * np.array([dist.mean() for dist in self.distributions])
+        ).sum()
+
+    def var(self):
+        return (
+            self.weights * np.array([dist.var() for dist in self.distributions])
+        ).sum()
+
+    def std(self):
+        return np.sqrt(self.var())
+
+
+class nonparametric(rv_continuous):
+    """Nonparametric distribution.
+
+    Args:
+        values (tuple[np.array, np.array]): (n,) array of x values, (n,) array of the
+            probability mass function evaluated at x.
+        moment_approximation_samples (int): Number of samples to use when numerically
+            approximating moments.
+
+    Attributes:
+        xk (np.ndarray): (n,) array of x values.
+        pk (np.ndarray): (n,) array of the probability mass function evaluated at x.
+
+    Notes:
+        This distribution interpolates between the probability mass function to
+        "continuize" the discrete function.
+    """
+
+    def __init__(self, values, moment_approximation_samples: int = 50, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.xk, self.pk = np.array(values[0], float), np.array(values[1], float)
+        self.moment_approximation_samples = moment_approximation_samples
+        if len(self.xk) > 3:
+            self._cubic_spline = CubicSpline(self.xk, self.pk)
+            self._pchip_interpolater = PchipInterpolator(self.xk, self.pk)
+
+            # put as little weight as possible on the PCHIP interpolater such that the pdf
+            # is always above 0
+            self._pchip_weight = 0
+            min_pdf_result = minimize_scalar(
+                self._interpolate, bounds=(self.xk[0], self.xk[-1])
+            )
+            while min_pdf_result.fun < 0:
+                # pdf goes below 0, need to increase weight on the PCHIP interpolater
+                pchip_min_fun = self._pchip_interpolater(min_pdf_result.x)
+                pchip_weight = min_pdf_result.x / (min_pdf_result.x - pchip_min_fun)
+                self._pchip_weight += pchip_weight * (1 - self._pchip_weight)
+                min_pdf_result = minimize_scalar(
+                    self._interpolate, bounds=(self.xk[0], self.xk[-1])
+                )
+        else:
+            self._cubic_spline = None
+            self._pchip_interpolater = None
+            self._pchip_weight = None
+
+        # determine the scale so the PDF integrates to 1
+        self._scale = 1
+        self._scale = 1 / quad(self._pdf, self.xk[0], self.xk[-1])[0]
+
+        # cache evaluations of the CDF
+        # this vastly speeds up the ppf and rvs methods
+        self._cdf_x = np.linspace(self.xk[0], self.xk[-1], num=10000)
+        pdf = self._pdf(self._cdf_x)
+        self._cdf_cache = pdf.cumsum()
+        self._cdf_cache /= self._cdf_cache[-1]
+
+        super().__init__(*args, **kwargs)
+
+    def _interpolate(self, x: np.ndarray) -> np.ndarray:
+        """Apply interpolation to get the PDF evaluated at x.
+
+        Args:
+            x (np.ndarray): Points at which to evaluate the PDF.
+
+        Returns:
+            np.ndarray: PDF evaluated at x.
+        """
+        if len(self.xk) < 4:
+            return np.interp(x, self.xk, self.pk)
+
+        if self._pchip_weight == 0:
+            return self._cubic_spline(x)
+
+        return self._pchip_weight * self._pchip_interpolater(x) + (
+            1 - self._pchip_weight
+        ) * self._cubic_spline(x)
+
+    def _pdf(self, x: np.ndarray) -> np.ndarray:
+        x = np.atleast_1d(x)
+        pdf = np.zeros(len(x))
+        in_range = (self.xk[0] < x) & (x < self.xk[-1])
+        pdf[in_range] = self._interpolate(x[in_range])
+        return self._scale * pdf
+
+    def _cdf(self, x: np.ndarray) -> np.ndarray:
+        x = np.atleast_1d(x)
+        cdf = np.zeros(len(x))
+        cdf[x >= self.xk[-1]] = 1
+        in_range = (self.xk[0] < x) & (x < self.xk[-1])
+        cdf[in_range] = np.interp(x[in_range], self._cdf_x, self._cdf_cache)
+        return cdf
+
+    def ppf(self, x: np.ndarray) -> np.ndarray:
+        x = np.atleast_1d(x)
+        ppf = super()._ppf(x)
+        ppf[ppf == np.inf] = self.xk[-1]
+        ppf[ppf == -np.inf] = self.xk[0]
+        return ppf[0] if len(x) == 1 else ppf
+
+    def moment(self, func: Callable[[np.ndarray], np.ndarray]) -> float:
+        """Compute a moment.
+
+        Args:
+            func (Callable[[np.ndarray], np.ndarray]): Moment function that takes
+                ``self.xk`` and returns an array of the same shape.
+
+        Returns:
+            float: Moment.
+        """
+        x = np.linspace(self.xk[0], self.xk[-1], num=self.moment_approximation_samples)
+        return sum(self.pdf(x) * func(x) * (x[1] - x[0]))
+
+    def mean(self) -> float:
+        """Compute the mean.
+
+        Returns:
+            float: Mean.
+        """
+        return self.moment(lambda x: x)
+
+    def var(self) -> float:
+        """Compute the variance.
+
+        Returns:
+            float: Variance.
+        """
+        mean = self.mean()
+        return self.moment(lambda x: (x - mean) ** 2)
+
+    def std(self) -> float:
+        """Compute the standard deviation.
+
+        Returns:
+            float: Standard deviation.
+        """
+        return np.sqrt(self.var())
+
+
+class quantile_unbiased(rv_continuous):  # pylint: disable=invalid-name
+    """Conditional quantile-unbiased distribution.
+
+    Inherits from `scipy.stats.rv_continuous <https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_continuous.html>`_
+    and handles standard public methods (``pdf``, ``cdf``, etc.).
+
+    Args:
+        y (float): Value at which the truncated CDF is evaluated
+        projection_interval (Union[float, Tuple[float, float]], optional): Lower and
+            upper bounds of the projection confidence interval. Defaults to
+            (-np.inf, np.inf).
+        bounds (Tuple[float, float], optional): Lower and upper bounds of the support
+            of the distribution. Defaults to (-np.inf, np.inf).
+        dx (float): Used to numerically approximate the PDF.
+        **truncnorm_kwargs (Any): Keyword arguments for :class:`truncnorm`.
+
+    Attributes:
+        y (float): Value at which the truncated CDF is evaluated.
+        bounds (Tuple[float, float]): Lower and upper bound of the support of the
+            distribution.
+        dx (float): Used to numerically approximate the PDF.
+        truncnorm_kwargs (dict): Keyword arguments for :class:`truncnorm`.
+
+    Examples:
+        Compute a median-unbiased estimate of a normally distributed variable given
+            that its observed value is 1 and falls between 0 and 3.
+
+        .. doctest::
+
+            >>> from multiple_inference.stats import quantile_unbiased
+            >>> dist = quantile_unbiased(1, truncation_set=[(0, 3)])
+            >>> dist.ppf(.5)
+            0.7108033900602351
+    """
+
+    def __init__(
+        self,
+        y: float,
+        projection_interval: Union[float, Tuple[float, float]] = (-np.inf, np.inf),
+        bounds: Tuple[float, float] = (-np.inf, np.inf),
+        dx: float = None,
+        **truncnorm_kwargs: Any,
+    ):
+        super().__init__()
+        self.y = y  # pylint: disable=invalid-name
+        if np.isscalar(projection_interval):
+            projection_interval = abs(projection_interval)  # type: ignore
+            projection_interval = (-projection_interval, projection_interval)
+        self.projection_interval = tuple(projection_interval)
+        self.bounds = bounds
+        self.truncnorm_kwargs = truncnorm_kwargs
+        self.dx = dx
+
+        self._cdf_min: float = (
+            0  # type: ignore
+            if bounds[0] == -np.inf
+            else 1 - self._truncated_cdf(np.array([bounds[0]]))
+        )
+        if self._cdf_min >= 1:
+            warnings.warn(
+                "Untruncated CDF of lower bound == 1: try decreasing the lower bound",
+                RuntimeWarning,
+            )
+        self._cdf_max: float = (
+            1  # type: ignore
+            if bounds[1] == np.inf
+            else 1 - self._truncated_cdf(np.array([bounds[1]]))
+        )
+        if self._cdf_max <= 0:
+            warnings.warn(
+                "Untruncated CDF of upper bound == 0: try increasing the upper bound",
+                RuntimeWarning,
+            )
+
+    @property
+    def dx(self):  # pylint: disable=missing-docstring
+        # create a default dx value if this property has not yet been set
+        if self._dx is None:
+            self.dx = np.diff(self.ppf([0.95, 0.05])) / 50
+        return self._dx
+
+    @dx.setter
+    def dx(self, value):
+        self._dx = value
+
+    @property
+    def bounds(self):  # pylint: disable=missing-docstring
+        # Potentially restrict the bounds of this distribution to ensure the truncation
+        # set and # projection interval overlap
+        truncation_set = self.truncnorm_kwargs.get("truncation_set")
+        if truncation_set is None or self.projection_interval == (-np.inf, np.inf):
+            return self._bounds
+
+        a, b = zip(*truncation_set)  # pylint: disable=invalid-name
+        return (
+            max(self._bounds[0], np.min(a) - self.projection_interval[1]),
+            min(self._bounds[1], np.max(b) - self.projection_interval[0]),
+        )
+
+    @bounds.setter
+    def bounds(self, bounds):
+        self._bounds = bounds
+
+    def _truncated_cdf(  # pylint: disable=invalid-name
+        self, x: np.ndarray
+    ) -> np.ndarray:
+        """Compute the truncated CDF evaluated at ``self.y`` with shift ``x``."""
+
+        def truncated_cdf(x_i):
+            # get the intersection of the truncation set and the projection confidence
+            # interval centered on x_i
+            intersection = []
+            for interval in truncation_set:
+                clipped_interval = (
+                    float(max(interval[0], x_i + self.projection_interval[0])),
+                    float(min(interval[1], x_i + self.projection_interval[1])),
+                )
+                if clipped_interval[0] < clipped_interval[1]:
+                    interval = (
+                        normalize(clipped_interval[0], x_i),
+                        normalize(clipped_interval[1], x_i),
+                    )
+                    intersection.append(interval)
+
+            return truncnorm(intersection, loc=x_i, **truncnorm_kwargs).cdf(self.y)
+
+        def normalize(value, loc):
+            return (value - loc) / scale
+
+        truncation_set = self.truncnorm_kwargs.get("truncation_set")
+        scale = self.truncnorm_kwargs.get("scale", 1)
+        truncnorm_kwargs = {
+            key: value
+            for key, value in self.truncnorm_kwargs.items()
+            if key != "truncation_set"
+        }
+        rval = np.array([truncated_cdf(x_i) for x_i in x])
+        return rval[0] if len(rval) == 1 else rval
+
+    def _cdf(self, x: np.ndarray) -> np.ndarray:  # pylint: disable=arguments-differ
+        """Cumulative distribution function.
+
+        Args:
+            x (np.ndarray): (n,) array of values at which to evaluate the CDF.
+
+        Returns:
+            np.ndarray: (n,) array of evaluations.
+        """
+        if self._cdf_min >= 1 or self._cdf_max <= 0:
+
+            def handle_cdf_out_of_bounds(x_i):
+                return self.bounds[0] <= x_i if self.y < x_i else self.bounds[1] < x_i
+
+            warnings.warn(
+                "Untruncated CDF of lower bound >= 1 or CDF of upper bound <= 0"
+            )
+            return np.array([handle_cdf_out_of_bounds(x_i) for x_i in x]).astype(float)
+
+        cdf = (1 - self._truncated_cdf(x) - self._cdf_min) / (
+            self._cdf_max - self._cdf_min
+        )
+        return ((self.bounds[0] < x) & (x < self.bounds[1])) * cdf + (
+            self.bounds[1] <= x
+        ).astype(float)
+
+    def _pdf(self, x: np.ndarray) -> np.ndarray:  # pylint: disable=arguments-differ
+        """Probability density function.
+
+        Args:
+            x (np.ndarray): (n,) array of values at which to evaluate the PDF.
+
+        Returns:
+            np.ndarray: (n,) array of evaluations.
+        """
+        pdf = derivative(self._cdf, x, dx=self.dx, order=5)
+        return ((self.bounds[0] < x) & (x < self.bounds[1])) * pdf
+
+    def _ppf(self, q: np.ndarray) -> np.ndarray:  # pylint: disable=arguments-differ
+        """See self.ppf."""
+
+        def func(mu, q_i):
+            return self._truncated_cdf(mu) - (1 - q_i)
+
+        if self._cdf_min >= 1 or self._cdf_max <= 0:
+            warnings.warn(
+                "Untruncated CDF of lower bound >= 1 or CDF of upper bound <= 0"
+            )
+
+            value = self.bounds[0] if self.bounds[0] > self.y else self.bounds[1]
+            return np.full(q.shape, value)
+
+        q_t = np.atleast_1d(q) * (self._cdf_max - self._cdf_min) + self._cdf_min
+        return np.array([fsolve(func, [self.y], args=(q_i,))[0] for q_i in q_t])
+
+    def ppf(  # pylint: disable=arguments-differ
+        self, q: Union[float, Numeric1DArray]
+    ) -> np.ndarray:
+        """Percent point function.
+
+        Args:
+            q (np.ndarray): (n,) array of quantiles at which to evaluate the PPF.
+
+        Returns:
+            np.ndarray: (n,) array of evaluations.
+        """
+        return np.clip(super().ppf(q), *self.bounds)
+
+
+class truncnorm(rv_continuous):  # pylint: disable=invalid-name
+    """Truncated normal distribution.
+
+    Inherits from `scipy.stats.rv_continuous <https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_continuous.html>`_
+    and handles standard public methods (``pdf``, ``cdf``, etc.).
+
+    This uses the `exponential tilting <https://ieeexplore.ieee.org/document/7408180>`_
+    approximation method.
+
+    Args:
+        truncation_set (List[Tuple[float, float]], optional): List of truncation
+            intervals, e.g., ``[(-1, 0), (1, 2)]`` truncates the distribution to
+            [-1, 0] union [1, 2]. Defaults to None.
+        loc (float, optional): Location. Defaults to 0.
+        scale (float, optional): Scale parameter. Defaults to 1.
+        n_samples (int, optional): Number of samples to draw for approximation.
+            Defaults to 10000.
+        seed (int, optional): Random seed. Defaults to 0.
+
+    Attributes:
+        loc (float): Location parameter.
+        scale (float): Scale parameter.
+        lower_bound (np.array): (# intervals,) array of lower bounds of the truncation
+            intervals.
+        upper_bound (np.array): (# intervals,) array of upper bounds of the truncation
+            intervals.
+        interval_masses (np.array): (# intervals,) array of the amount of mass in each
+            truncation interval.
+        n_samples (int): Number of samples to draw for approximation. Defaults to
+            10000.
+
+    Examples:
+        Let's evaluate the CDF of a standard normal truncated to the interval (-1, 0) at -0.5.
+
+        .. testcode::
+
+            from multiple_inference.stats import truncnorm
+            print(truncnorm([(-1, 0)]).cdf(-.5))
+
+        .. testoutput::
+
+            0.4390935748119969
+
+        Let's evaluate the CDF of a standard normal truncated to the union of (-1, 0) and (1, 2) at -0.5.
+
+        .. testcode::
+
+            from multiple_inference.stats import truncnorm
+            print(truncnorm([(-1, 0), (1, 2)]).cdf(-.5))
+
+        .. testoutput::
+
+            0.3140541146849627
+
+    Note:
+        The truncation set is defined over the domain of the standard normal. To
+        convert the truncation set for a specific mean and standard deviation, use:
+
+        .. code-block:: python
+
+            >>> truncation_set = [(myclip_a - my_mean) / my_std, (myclip_b - my_mean) / my_std)]
+    """
+
+    def __init__(
+        self,
+        truncation_set: List[Tuple[float, float]] = None,
+        loc: float = 0,
+        scale: float = 1,
+        n_samples: int = 10000,
+        seed: int = 0,
+    ):
+        self.seed = seed
+        self.loc = loc
+        self.scale = scale
+        self.n_samples = n_samples
+        if truncation_set is None:
+            truncation_set = [(-np.inf, np.inf)]
+        self.lower_bound, self.upper_bound = self._get_truncation_bounds(truncation_set)
+        self.interval_masses = np.array(
+            [
+                self._compute_mass_in_interval_avg(a, b)
+                for a, b in zip(self.lower_bound, self.upper_bound)
+            ]
+        )
+        super().__init__()
+
+    def _pdf(self, x):  # pylint: disable=arguments-differ
+        x = self._normalize(x)
+        # n x 1 indicator that x is in an interval
+        in_interval = np.array(
+            [np.any((self.lower_bound <= x_i) & (x_i <= self.upper_bound)) for x_i in x]
+        )
+        return in_interval * norm.pdf(x) / (self.scale * self.interval_masses.sum())
+
+    def _logpdf(self, x):  # pylint: disable=arguments-differ
+        x = self._normalize(x)
+        # n x 1 indicator that x is in an interval
+        in_interval = np.array(
+            [np.any((self.lower_bound <= x_i) & (x_i <= self.upper_bound)) for x_i in x]
+        )
+        logpdf = (
+            norm.logpdf(x) - np.log(self.scale) - np.log(self.interval_masses.sum())
+        )
+        logpdf[~in_interval] = -np.inf
+        return logpdf
+
+    def _cdf(self, x):  # pylint: disable=arguments-differ
+        x = self._normalize(x)
+
+        if self.lower_bound.size == self.upper_bound.size == 0:
+            # i.e., truncation set is empty
+            return (x > 0).astype(float)
+
+        denominator = self.interval_masses.sum()
+        if denominator == 0:
+            # converts cdf to 0 or 1 depending on bounds and x
+            a = self.lower_bound.min()
+            b = self.upper_bound.max()
+            convert_0_1 = lambda x_i: a < x_i if x_i > 0 else b < x_i
+            return np.array([convert_0_1(x_i) for x_i in x]).astype(float)
+
+        return np.clip(self._compute_cdf_numerator(x) / denominator, 0, 1)
+
+    def _logcdf(self, x):  # pylint: disable=arguments-differ
+        x = self._normalize(x)
+        denominator = self.interval_masses.sum()
+        return np.log(self._compute_cdf_numerator(x)) - np.log(denominator)
+
+    def _compute_mass_in_interval_avg(self, a, b):
+        # compute the amount of mass in the interval [a, b] by averaging approximate
+        # mass in [a, b] and [-b, -a]
+        # the amount of mass in these intervals is the same because the normal is symmetric
+        # this can improve performance
+        arr = [
+            self._compute_mass_in_interval(a, b, int(self.n_samples / 2)),
+            self._compute_mass_in_interval(-b, -a, int(self.n_samples / 2)),
+        ]
+        return np.mean(arr, where=~np.isnan(arr))
+
+    def _compute_mass_in_interval(self, a, b, n_samples=None):
+        # compute the amount of mass in the interval [a, b] using minimax exponential tilt
+        def compute_psi(params):
+            x, mu = params
+            return -x * mu + (0.5 * mu**2 + np.log(norm.cdf(b, mu) - norm.cdf(a, mu)))
+
+        def d_psi_d_mu(params):
+            # derivative of psi with respect to mu
+            x, mu = params
+            return (
+                -x
+                + mu
+                + (norm.pdf(b, mu) - norm.pdf(a, mu))
+                / ((norm.cdf(b, mu) - norm.cdf(a, mu)))
+            )
+
+        def optimize_params(x0):
+            # maximize psi subject to x being contained in the interval and the
+            # derivative of psi wrt mu =0 0
+            derivative_constraint = NonlinearConstraint(d_psi_d_mu, 0, 0)
+            return minimize(
+                lambda x: -compute_psi(x),
+                x0=x0,
+                bounds=[(a, b), (-np.inf, np.inf)],
+                constraints=[derivative_constraint],
+            )
+
+        def compute_tilting_param():
+            # compute the optimal tilting parameter
+            try:
+                # initial guess for x, denoted as Psi in the paper
+                # in the univariate case, the initial guess for mu is 0
+                x_init = (norm.pdf(a) - norm.pdf(b)) / ((norm.cdf(b) - norm.cdf(a)))
+            except ZeroDivisionError:
+                x_init = a if a < 0 else b
+
+            if a < x_init < b:
+                # optimal x is in the truncation set, so optimal mu is 0
+                return 0
+
+            # optimal mu must be found by non-linear optimization
+            res = optimize_params([x_init, 0])
+            if res.success:
+                return res.x[1]
+            next_guess, final_guess = ([a, a], [b, b]) if a > 0 else ([b, b], [a, a])
+            res = optimize_params(next_guess)
+            if res.success:
+                return res.x[1]
+            res = optimize_params(final_guess)
+            if res.success:
+                return res.x[1]
+            warnings.warn(
+                "Optimizer failed to find truncated normal tilt parameter",
+                RuntimeWarning,
+            )
+            return x_init
+
+        if b < a:
+            return 0
+        mu = compute_tilting_param()
+        x = truncnorm_base.rvs(
+            a - mu, b - mu, mu, size=n_samples or self.n_samples, random_state=self.seed
+        )
+        return np.exp(compute_psi((x, mu))).mean()
+
+    def _compute_cdf_numerator(self, x):
+        # n x p indicates x is above the upper bound of the interval
+        index = np.array([self.upper_bound <= x_i for x_i in x])
+        # n x 1 CDF for the intervals where x is above the upper bound
+        cdf = index @ self.interval_masses
+
+        # tuple of (x index, interval index) such that x[x index] is in interval[interval_index]
+        indices = np.where(
+            [(self.lower_bound < x_i) & (x_i < self.upper_bound) for x_i in x]
+        )
+        # add mass from intervals containing x
+        cdf[indices[0]] += np.array(
+            [
+                self._compute_mass_in_interval_avg(
+                    self.lower_bound[interval_index], x[x_index]
+                )
+                for x_index, interval_index in zip(*indices)
+            ]
+        )
+
+        return cdf
+
+    def _get_truncation_bounds(self, truncation_set):
+        if not truncation_set:
+            return np.array([]), np.array([])
+
+        for interval in truncation_set:
+            if interval[1] < interval[0]:
+                raise ValueError(f"Invalid interval {interval}")
+
+        truncation_set.sort(key=lambda x: x[0])
+        a, b = list(zip(*truncation_set))
+
+        # ensure b is strictly increasing
+        b = [b[0]] + [max(b_i, b_j) for b_i, b_j in zip(b[1:], b[:-1])]
+
+        new_a, new_b = [a[0]], []
+        for a_i, b_i in zip(a[1:], b[:-1]):
+            if a_i > b_i:
+                new_b.append(b_i)
+                new_a.append(a_i)
+        new_b.append(b[-1])
+
+        return np.array(new_a), np.array(new_b)
+
+    def _normalize(self, arr):
+        return (arr - self.loc) / self.scale
```

### Comparing `multiple-inference-1.1.0/src/multiple_inference/utils.py` & `multiple-inference-1.2.0/src/multiple_inference/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-"""Conditional inference utilities.
-"""
-from typing import Any, Optional, Sequence, Union
-
-import numpy as np
-import pandas as pd
-from scipy.stats import multivariate_normal, wasserstein_distance
-from statsmodels.base.model import LikelihoodModelResults
-
-Numeric1DArray = Sequence[float]
-
-
-def _get_sample_weight(sample_weight: Optional[np.ndarray], shape: int) -> np.ndarray:
-    if sample_weight is None:
-        sample_weight = np.ones(shape)
-    sample_weight = np.array(sample_weight)
-    return sample_weight / sample_weight.sum()
-
-
-def expected_wasserstein_distance(
-    mean: Numeric1DArray,
-    cov: np.ndarray,
-    estimated_means: np.ndarray,
-    sample_weight: np.ndarray = None,
-    **kwargs: Any
-) -> float:
-    """Compute the expected Wasserstein distance.
-
-    This loss function computes the Wasserstein distance between the observed means
-    ``mean`` and the distribution of means you would expect to observe given the
-    estimated population means ``estimated_means``.
-
-    Args:
-        mean (Numeric1DArray): (n,) array of conventional point estimates.
-        cov (np.ndarray): (n, n) covariance matrix of conventional estimates.
-        estimated_means (np.ndarray): (# samples, n) matrix of draws from
-            a distribution of population means.
-        sample_weight (np.ndarray, optional): (# samples,) array of sample weights for
-            ``estimated_means``. Defaults to None.
-        **kwargs (Any): Keyword arguments for ``scipy.stats.wasserstein_distance``.
-
-    Returns:
-        float: Loss.
-    """
-    sample_weight = _get_sample_weight(sample_weight, estimated_means.shape[0])
-    compute_distance = lambda mu: wasserstein_distance(
-        multivariate_normal.rvs(mu, cov), mean, **kwargs
-    )
-    distances = np.apply_along_axis(compute_distance, 1, estimated_means)
-    return (sample_weight * distances).sum()
-
-
-def holm_bonferroni_correction(
-    filename: str = None, results: LikelihoodModelResults = None, alpha: float = 0.05
-) -> pd.Series:
-    """Get significant coefficients by performing a Holm-Bonferroni correction.
-
-    Args:
-        filename (str, optional): Name of the csv file with conventional estimates.
-            Defaults to None.
-        results (LikelihoodModelResults, optional): Results. Defaults to None.
-        alpha (float, optional): Significance level. Defaults to .05.
-
-    Raises:
-        ValueError: You must specify either ``filename`` or ``results`` but not both.
-
-    Returns:
-        pd.DataFrame: Dataframe indicating which coefficients are significant.
-    """
-    if filename is None and results is None:
-        raise ValueError("filename or results must be specified.")
-
-    if filename is not None and results is not None:
-        raise ValueError("Please specify either filename or results; not both.")
-
-    if results is None:
-        from .bayes import Improper
-
-        results = Improper.from_csv(filename).fit()
-        # Improper gives pvalues for 1-tailed tests
-        pvalues = np.min(
-            np.array([2 * results.pvalues, 2 * (1 - results.pvalues)]), axis=0
-        )
-    else:
-        pvalues = results.pvalues
-
-    argsort = pvalues.argsort()
-    df = pd.DataFrame(
-        {"pvalues": pvalues[argsort]},
-        index=np.array(results.model.exog_names)[argsort],
-    )
-    index = np.where(df.pvalues > alpha / (len(df) - np.arange(len(df))))[0][0]
-    df["significant"] = np.arange(len(df)) < index
-    return df
-
-
-def weighted_quantile(
-    values: np.ndarray,
-    quantiles: Union[float, Numeric1DArray],
-    sample_weight: np.ndarray = None,
-    values_sorted: bool = False,
-) -> np.ndarray:
-    """Compute weighted quantiles.
-
-    Args:
-        values (np.ndarray): (n,) array over which to compute quantiles.
-        quantiles (Union[float, Numeric1DArray]): (k,) array of quantiles of interest.
-        sample_weight (np.ndarray, optional): (n,) array of sample weights. Defaults to
-            None.
-        values_sorted (bool, optional): Indicates that ``values`` have been pre-sorted.
-            Defaults to False.
-
-    Returns:
-        np.array: (k,) array of weighted quantiles.
-
-    Acknowledgements:
-        Credit to `Stackoverflow <https://stackoverflow.com/a/29677616/10676300>`_.
-    """
-    values = np.array(values)
-    quantiles = np.atleast_1d(quantiles)  # type: ignore
-    sample_weight = _get_sample_weight(sample_weight, len(values))
-    assert np.all(quantiles >= 0) and np.all(  # type: ignore
-        quantiles <= 1  # type: ignore
-    ), "quantiles should be in [0, 1]"
-
-    if not values_sorted:
-        sorter = np.argsort(values)
-        values = values[sorter]
-        sample_weight = sample_weight[sorter]
-
-    weighted_quantiles = np.cumsum(sample_weight) - 0.5 * sample_weight  # type: ignore
-    return np.interp(quantiles, weighted_quantiles, values)
+"""Conditional inference utilities.
+"""
+from typing import Any, Optional, Sequence, Union
+
+import numpy as np
+import pandas as pd
+from scipy.stats import multivariate_normal, wasserstein_distance
+from statsmodels.base.model import LikelihoodModelResults
+
+Numeric1DArray = Sequence[float]
+
+
+def _get_sample_weight(sample_weight: Optional[np.ndarray], shape: int) -> np.ndarray:
+    if sample_weight is None:
+        sample_weight = np.ones(shape)
+    sample_weight = np.array(sample_weight)
+    return sample_weight / sample_weight.sum()
+
+
+def expected_wasserstein_distance(
+    mean: Numeric1DArray,
+    cov: np.ndarray,
+    estimated_means: np.ndarray,
+    sample_weight: np.ndarray = None,
+    **kwargs: Any
+) -> float:
+    """Compute the expected Wasserstein distance.
+
+    This loss function computes the Wasserstein distance between the observed means
+    ``mean`` and the distribution of means you would expect to observe given the
+    estimated population means ``estimated_means``.
+
+    Args:
+        mean (Numeric1DArray): (n,) array of conventional point estimates.
+        cov (np.ndarray): (n, n) covariance matrix of conventional estimates.
+        estimated_means (np.ndarray): (# samples, n) matrix of draws from
+            a distribution of population means.
+        sample_weight (np.ndarray, optional): (# samples,) array of sample weights for
+            ``estimated_means``. Defaults to None.
+        **kwargs (Any): Keyword arguments for ``scipy.stats.wasserstein_distance``.
+
+    Returns:
+        float: Loss.
+    """
+    sample_weight = _get_sample_weight(sample_weight, estimated_means.shape[0])
+    compute_distance = lambda mu: wasserstein_distance(
+        multivariate_normal.rvs(mu, cov), mean, **kwargs
+    )
+    distances = np.apply_along_axis(compute_distance, 1, estimated_means)
+    return (sample_weight * distances).sum()
+
+
+def holm_bonferroni_correction(
+    filename: str = None, results: LikelihoodModelResults = None, alpha: float = 0.05
+) -> pd.Series:
+    """Get significant coefficients by performing a Holm-Bonferroni correction.
+
+    Args:
+        filename (str, optional): Name of the csv file with conventional estimates.
+            Defaults to None.
+        results (LikelihoodModelResults, optional): Results. Defaults to None.
+        alpha (float, optional): Significance level. Defaults to .05.
+
+    Raises:
+        ValueError: You must specify either ``filename`` or ``results`` but not both.
+
+    Returns:
+        pd.DataFrame: Dataframe indicating which coefficients are significant.
+    """
+    if filename is None and results is None:
+        raise ValueError("filename or results must be specified.")
+
+    if filename is not None and results is not None:
+        raise ValueError("Please specify either filename or results; not both.")
+
+    if results is None:
+        from .bayes import Improper
+
+        results = Improper.from_csv(filename).fit()
+        # Improper gives pvalues for 1-tailed tests
+        pvalues = np.min(
+            np.array([2 * results.pvalues, 2 * (1 - results.pvalues)]), axis=0
+        )
+    else:
+        pvalues = results.pvalues
+
+    argsort = pvalues.argsort()
+    df = pd.DataFrame(
+        {"pvalues": pvalues[argsort]},
+        index=np.array(results.model.exog_names)[argsort],
+    )
+    index = np.where(df.pvalues > alpha / (len(df) - np.arange(len(df))))[0][0]
+    df["significant"] = np.arange(len(df)) < index
+    return df
+
+
+def weighted_quantile(
+    values: np.ndarray,
+    quantiles: Union[float, Numeric1DArray],
+    sample_weight: np.ndarray = None,
+    values_sorted: bool = False,
+) -> np.ndarray:
+    """Compute weighted quantiles.
+
+    Args:
+        values (np.ndarray): (n,) array over which to compute quantiles.
+        quantiles (Union[float, Numeric1DArray]): (k,) array of quantiles of interest.
+        sample_weight (np.ndarray, optional): (n,) array of sample weights. Defaults to
+            None.
+        values_sorted (bool, optional): Indicates that ``values`` have been pre-sorted.
+            Defaults to False.
+
+    Returns:
+        np.array: (k,) array of weighted quantiles.
+
+    Acknowledgements:
+        Credit to `Stackoverflow <https://stackoverflow.com/a/29677616/10676300>`_.
+    """
+    values = np.array(values)
+    quantiles = np.atleast_1d(quantiles)  # type: ignore
+    sample_weight = _get_sample_weight(sample_weight, len(values))
+    assert np.all(quantiles >= 0) and np.all(  # type: ignore
+        quantiles <= 1  # type: ignore
+    ), "quantiles should be in [0, 1]"
+
+    if not values_sorted:
+        sorter = np.argsort(values)
+        values = values[sorter]
+        sample_weight = sample_weight[sorter]
+
+    weighted_quantiles = np.cumsum(sample_weight) - 0.5 * sample_weight  # type: ignore
+    return np.interp(quantiles, weighted_quantiles, values)
```

### Comparing `multiple-inference-1.1.0/src/multiple_inference.egg-info/PKG-INFO` & `multiple-inference-1.2.0/src/multiple_inference.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1
-Name: multiple-inference
-Version: 1.1.0
-Summary: A statistics package for comparing multiple parameters.
-Home-page: https://dsbowen.gitlab.io/conditional-inference
-Author: Dillon Bowen
-Author-email: dsbowen@wharton.upenn.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Multiple Inference
-
-[![Documentation Status](https://readthedocs.org/projects/dsbowen-conditional-inference/badge/?version=latest)](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest)
-[![status](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888/status.svg)](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888)
-[![pipeline status](https://gitlab.com/dsbowen/conditional-inference/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
-[![coverage report](https://gitlab.com/dsbowen/conditional-inference/badges/master/coverage.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
-[![PyPI version](https://badge.fury.io/py/conditional-inference.svg)](https://badge.fury.io/py/conditional-inference)
-[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/conditional-inference/-/blob/master/LICENSE)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fconditional-inference/HEAD?urlpath=lab/tree/examples)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-A statistics package for comparing multiple parameters. Read the docs [here](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest).
+Metadata-Version: 2.1
+Name: multiple-inference
+Version: 1.2.0
+Summary: A statistics package for comparing multiple parameters.
+Home-page: https://dsbowen.gitlab.io/conditional-inference
+Author: Dillon Bowen
+Author-email: dsbowen@wharton.upenn.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Multiple Inference
+
+[![Documentation Status](https://readthedocs.org/projects/dsbowen-conditional-inference/badge/?version=latest)](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest)
+[![status](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888/status.svg)](https://joss.theoj.org/papers/7a2a4af277c0ad6ad6f41897f4489888)
+[![pipeline status](https://gitlab.com/dsbowen/conditional-inference/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
+[![coverage report](https://gitlab.com/dsbowen/conditional-inference/badges/master/coverage.svg)](https://gitlab.com/dsbowen/conditional-inference/-/commits/master)
+[![PyPI version](https://badge.fury.io/py/conditional-inference.svg)](https://badge.fury.io/py/conditional-inference)
+[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/conditional-inference/-/blob/master/LICENSE)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fconditional-inference/HEAD?urlpath=lab/tree/examples)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A statistics package for comparing multiple parameters. Read the docs [here](https://dsbowen-conditional-inference.readthedocs.io/en/latest/?badge=latest).
```

### Comparing `multiple-inference-1.1.0/tests/test_base.py` & `multiple-inference-1.2.0/tests/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-import io
-import os
-import pickle
-
-import numpy as np
-import pandas as pd
-import pytest
-import statsmodels.api as sm
-from scipy.stats import norm
-
-from conditional_inference.base import ModelBase
-
-N_POLICIES = 3
-
-
-@pytest.fixture(scope="module", params=[True, False])
-def ols_results(
-    request,
-    n_obs_per_policy=100,
-    exog_names=[f"var{i}" for i in range(N_POLICIES)],
-    endog_name="target",
-):
-    # create statsmodels OLS results
-    X = pd.DataFrame(
-        np.repeat(np.identity(N_POLICIES), n_obs_per_policy, axis=0), columns=exog_names
-    )
-    y = X @ np.arange(N_POLICIES) + norm.rvs(size=N_POLICIES * n_obs_per_policy)
-    y = pd.Series(y, name=endog_name)
-    ols_results = sm.OLS(y, X).fit()
-    return ols_results if request.param else ols_results.get_robustcov_results()
-
-
-class TestModelBase:
-    @pytest.mark.parametrize(
-        "mean", ([0, 1, 2], pd.Series([0, 1, 2], index=["world", "moon", "star"]))
-    )
-    @pytest.mark.parametrize("exog_names", (None, ["mars", "europa", "sun"]))
-    @pytest.mark.parametrize("sort", (True, False))
-    def test__init__(self, mean, exog_names, sort):
-        model = ModelBase(mean, np.diag([1, 2, 3]), exog_names=exog_names, sort=sort)
-
-        expected_exog_names = ["x0", "x1", "x2"]
-
-        if sort:
-            expected_mean = [2, 1, 0]
-            expected_cov = np.diag([3, 2, 1])
-            if isinstance(mean, pd.Series):
-                expected_exog_names = ["star", "moon", "world"]
-            if exog_names is not None:
-                expected_exog_names = ["sun", "europa", "mars"]
-        else:
-            expected_mean = [0, 1, 2]
-            expected_cov = np.diag([1, 2, 3])
-            if isinstance(mean, pd.Series):
-                expected_exog_names = ["world", "moon", "star"]
-            if exog_names is not None:
-                expected_exog_names = ["mars", "europa", "sun"]
-
-        np.testing.assert_array_equal(model.mean, expected_mean)
-        np.testing.assert_array_equal(model.cov, expected_cov)
-        np.testing.assert_array_equal(model.exog_names, expected_exog_names)
-
-    @pytest.mark.parametrize(
-        "columns", ([0.0, 2.0], [0, 2], ["world", "star"], [True, False, True])
-    )
-    @pytest.mark.parametrize("sort", (True, False))
-    def test_column_selection(self, columns, sort):
-        model = ModelBase(
-            pd.Series([0, 1, 2], index=["world", "moon", "star"]),
-            np.diag([1, 2, 3]),
-            columns=columns,
-            sort=sort,
-        )
-
-        if sort:
-            expected_mean = [2, 0]
-            expected_cov = np.diag([3, 1])
-            expected_exog_names = ["star", "world"]
-        else:
-            expected_mean = [0, 2]
-            expected_cov = np.diag([1, 3])
-            expected_exog_names = ["world", "star"]
-        np.testing.assert_array_equal(model.mean, expected_mean)
-        np.testing.assert_array_equal(model.cov, expected_cov)
-        np.testing.assert_array_equal(model.exog_names, expected_exog_names)
-
-    @pytest.mark.parametrize("endog_names", [None, "target"])
-    def test_endog_names(self, endog_names):
-        # test that the data has the correct endogenous variable name
-        model = ModelBase(
-            np.arange(N_POLICIES), np.identity(N_POLICIES), endog_names=endog_names
-        )
-        if endog_names is None:
-            assert model.endog_names == "y"
-        else:
-            assert model.endog_names == endog_names
-
-    def get_params_cov(self, ols_results):
-        params = ols_results.params
-        if isinstance(params, pd.Series):
-            params = params.values
-
-        cov = ols_results.cov_params()
-        if isinstance(cov, pd.DataFrame):
-            cov = cov.values
-
-        return params, cov
-
-    def compare_model_to_ols_results(self, model, ols_results):
-        # make sure the model's attributes match those of the OLS results
-        params, cov = self.get_params_cov(ols_results)
-        np.testing.assert_almost_equal(model.mean, params)
-        np.testing.assert_almost_equal(model.cov, cov)
-        np.testing.assert_array_equal(model.exog_names, ols_results.model.exog_names)
-        assert model.endog_names == ols_results.model.endog_names
-
-    def test_from_results(self, ols_results):
-        # test that you can initialize a model from statsmodels results object
-        model = ModelBase.from_results(ols_results)
-        self.compare_model_to_ols_results(model, ols_results)
-
-    def test_to_and_from_csv(self, ols_results):
-        # test that you can initialize a model from a csv file
-        ModelBase.from_results(ols_results).to_csv(bytes := io.BytesIO())
-        bytes.seek(0)
-        model = ModelBase.from_csv(bytes)
-        self.compare_model_to_ols_results(model, ols_results)
-
-
-results = ModelBase(np.arange(N_POLICIES), np.identity(N_POLICIES)).fit()
-
-
-class TestResults:
-    def test_conf_int(self):
-        with pytest.raises(AttributeError):
-            results.conf_int()
-
-    def test_save(self):
-        results.save(filename := "temp.p")
-        with open(filename, "rb") as results_file:
-            loaded_results = pickle.load(results_file)
-        os.remove(filename)
-        np.testing.assert_almost_equal(loaded_results.model.mean, results.model.mean)
+import io
+import os
+import pickle
+
+import numpy as np
+import pandas as pd
+import pytest
+import statsmodels.api as sm
+from scipy.stats import norm
+
+from multiple_inference.base import ModelBase
+
+N_POLICIES = 3
+
+
+@pytest.fixture(scope="module", params=[True, False])
+def ols_results(
+    request,
+    n_obs_per_policy=100,
+    exog_names=[f"var{i}" for i in range(N_POLICIES)],
+    endog_name="target",
+):
+    # create statsmodels OLS results
+    X = pd.DataFrame(
+        np.repeat(np.identity(N_POLICIES), n_obs_per_policy, axis=0), columns=exog_names
+    )
+    y = X @ np.arange(N_POLICIES) + norm.rvs(size=N_POLICIES * n_obs_per_policy)
+    y = pd.Series(y, name=endog_name)
+    ols_results = sm.OLS(y, X).fit()
+    return ols_results if request.param else ols_results.get_robustcov_results()
+
+
+class TestModelBase:
+    @pytest.mark.parametrize(
+        "mean", ([0, 1, 2], pd.Series([0, 1, 2], index=["world", "moon", "star"]))
+    )
+    @pytest.mark.parametrize("exog_names", (None, ["mars", "europa", "sun"]))
+    @pytest.mark.parametrize("sort", (True, False))
+    def test__init__(self, mean, exog_names, sort):
+        model = ModelBase(mean, np.diag([1, 2, 3]), exog_names=exog_names, sort=sort)
+
+        expected_exog_names = ["x0", "x1", "x2"]
+
+        if sort:
+            expected_mean = [2, 1, 0]
+            expected_cov = np.diag([3, 2, 1])
+            if isinstance(mean, pd.Series):
+                expected_exog_names = ["star", "moon", "world"]
+            if exog_names is not None:
+                expected_exog_names = ["sun", "europa", "mars"]
+        else:
+            expected_mean = [0, 1, 2]
+            expected_cov = np.diag([1, 2, 3])
+            if isinstance(mean, pd.Series):
+                expected_exog_names = ["world", "moon", "star"]
+            if exog_names is not None:
+                expected_exog_names = ["mars", "europa", "sun"]
+
+        np.testing.assert_array_equal(model.mean, expected_mean)
+        np.testing.assert_array_equal(model.cov, expected_cov)
+        np.testing.assert_array_equal(model.exog_names, expected_exog_names)
+
+    @pytest.mark.parametrize(
+        "columns", ([0.0, 2.0], [0, 2], ["world", "star"], [True, False, True])
+    )
+    @pytest.mark.parametrize("sort", (True, False))
+    def test_column_selection(self, columns, sort):
+        model = ModelBase(
+            pd.Series([0, 1, 2], index=["world", "moon", "star"]),
+            np.diag([1, 2, 3]),
+            columns=columns,
+            sort=sort,
+        )
+
+        if sort:
+            expected_mean = [2, 0]
+            expected_cov = np.diag([3, 1])
+            expected_exog_names = ["star", "world"]
+        else:
+            expected_mean = [0, 2]
+            expected_cov = np.diag([1, 3])
+            expected_exog_names = ["world", "star"]
+        np.testing.assert_array_equal(model.mean, expected_mean)
+        np.testing.assert_array_equal(model.cov, expected_cov)
+        np.testing.assert_array_equal(model.exog_names, expected_exog_names)
+
+    @pytest.mark.parametrize("endog_names", [None, "target"])
+    def test_endog_names(self, endog_names):
+        # test that the data has the correct endogenous variable name
+        model = ModelBase(
+            np.arange(N_POLICIES), np.identity(N_POLICIES), endog_names=endog_names
+        )
+        if endog_names is None:
+            assert model.endog_names == "y"
+        else:
+            assert model.endog_names == endog_names
+
+    def get_params_cov(self, ols_results):
+        params = ols_results.params
+        if isinstance(params, pd.Series):
+            params = params.values
+
+        cov = ols_results.cov_params()
+        if isinstance(cov, pd.DataFrame):
+            cov = cov.values
+
+        return params, cov
+
+    def compare_model_to_ols_results(self, model, ols_results):
+        # make sure the model's attributes match those of the OLS results
+        params, cov = self.get_params_cov(ols_results)
+        np.testing.assert_almost_equal(model.mean, params)
+        np.testing.assert_almost_equal(model.cov, cov)
+        np.testing.assert_array_equal(model.exog_names, ols_results.model.exog_names)
+        assert model.endog_names == ols_results.model.endog_names
+
+    def test_from_results(self, ols_results):
+        # test that you can initialize a model from statsmodels results object
+        model = ModelBase.from_results(ols_results)
+        self.compare_model_to_ols_results(model, ols_results)
+
+    def test_to_and_from_csv(self, ols_results):
+        # test that you can initialize a model from a csv file
+        ModelBase.from_results(ols_results).to_csv(bytes := io.BytesIO())
+        bytes.seek(0)
+        model = ModelBase.from_csv(bytes)
+        self.compare_model_to_ols_results(model, ols_results)
+
+
+results = ModelBase(np.arange(N_POLICIES), np.identity(N_POLICIES)).fit()
+
+
+class TestResults:
+    def test_conf_int(self):
+        with pytest.raises(AttributeError):
+            results.conf_int()
+
+    def test_save(self):
+        results.save(filename := "temp.p")
+        with open(filename, "rb") as results_file:
+            loaded_results = pickle.load(results_file)
+        os.remove(filename)
+        np.testing.assert_almost_equal(loaded_results.model.mean, results.model.mean)
```

### Comparing `multiple-inference-1.1.0/tests/test_confidence_set.py` & `multiple-inference-1.2.0/tests/test_confidence_set.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,198 +1,255 @@
-import numpy as np
-import pytest
-from scipy.stats import norm
-
-from conditional_inference.confidence_set import (
-    ConfidenceSet,
-    AverageComparison,
-    BaselineComparison,
-    PairwiseComparison,
-    MarginalRanking,
-    SimultaneousRanking,
-)
-
-N_PARAMS = 3
-MEAN = np.arange(N_PARAMS) - (N_PARAMS - 1) / 2
-COV = np.identity(N_PARAMS)
-
-
-@pytest.mark.parametrize(
-    "cls",
-    (
-        ConfidenceSet,
-        AverageComparison,
-        BaselineComparison,
-        PairwiseComparison,
-        MarginalRanking,
-        SimultaneousRanking,
-    ),
-)
-def test_common_methods(cls):
-    # test that the common methods (conf_int, summary, point_plot) can run on all
-    # classes without error
-    kwargs = {"baseline": 0} if cls is BaselineComparison else {}
-    results = cls(MEAN, COV, **kwargs).fit()
-    results.conf_int()
-    results.summary()
-    results.point_plot()
-
-
-class TestConfidenceSet:
-    results = ConfidenceSet(MEAN, COV).fit()
-
-    def test_conf_int_shape(self):
-        assert self.results.conf_int().shape == (N_PARAMS, 2)
-
-    def test_1_param(self):
-        np.testing.assert_equal(
-            ConfidenceSet(0, 1).fit().conf_int(), [norm.ppf([0.025, 0.975])]
-        )
-
-    def test_conf_int(self):
-        # test the the marginal CI is in the simultaneous CI
-        alpha = 0.05
-        simultaneous_ci = self.results.conf_int(alpha)
-        marginal_ci = np.array(
-            [
-                norm.ppf([alpha / 2, 1 - alpha / 2], mean, np.sqrt(var))
-                for mean, var in zip(MEAN, COV.diagonal())
-            ]
-        )
-        np.testing.assert_array_less(simultaneous_ci[:, 0], marginal_ci[:, 0])
-        np.testing.assert_array_less(marginal_ci[:, 1], simultaneous_ci[:, 1])
-
-    @pytest.mark.parametrize("two_tailed", (True, False))
-    def test_test_hypotheses(self, two_tailed):
-        results = ConfidenceSet([-3, -2, 0, 2, 3], np.identity(5)).fit()
-        values = results.test_hypotheses(two_tailed=two_tailed)
-        if two_tailed:
-            np.testing.assert_array_equal(
-                values,
-                [
-                    [False, True],  # significantly less than 0
-                    [False, False],
-                    [False, False],
-                    [False, False],
-                    [True, False],  # significantly greater than 0
-                ],
-            )
-        else:
-            np.testing.assert_array_equal(values, [False, False, False, False, True])
-
-
-class TestAverageComparison:
-    def test___init__(self):
-        model = AverageComparison(MEAN, COV)
-        np.testing.assert_almost_equal(model.mean, [-1, 0, 1])
-        np.testing.assert_almost_equal(
-            model.cov,
-            [[2 / 3, -1 / 3, -1 / 3], [-1 / 3, 2 / 3, -1 / 3], [-1 / 3, -1 / 3, 2 / 3]],
-        )
-
-
-class TestBaselineComparison:
-    def test___init__(self):
-        model = BaselineComparison(MEAN, COV, baseline=0)
-        np.testing.assert_almost_equal(model.mean, [1, 2])
-        np.testing.assert_almost_equal(model.cov, [[2, 1], [1, 2]])
-
-
-class TestPairwiseComparison:
-    def test___init__(self):
-        results = PairwiseComparison(MEAN, COV).fit()
-        np.testing.assert_array_equal(
-            results.exog_names, ["x1 - x0", "x2 - x0", "x2 - x1"]
-        )
-        np.testing.assert_almost_equal(results.params, [1, 2, 1])  # [1-0, 2-0, 2-1]
-        np.testing.assert_almost_equal(results._std_diagonal, np.sqrt([2, 2, 2]))
-
-    def test_conf_int_shape(self):
-        results = PairwiseComparison(np.arange(4), np.identity(4)).fit()
-        assert results.conf_int().shape[0] == 4 * (4 - 1) / 2
-
-    @pytest.mark.parametrize("columns", (None, ["x2", "x1"]))
-    def test_test_hypotheses(self, columns):
-        results = PairwiseComparison([0, 4, 1, 2], np.identity(4) / 3).fit()
-        if columns is None:
-            expected_values = [
-                [False, True, False, False],  # x1 > 0
-                [False, False, False, False],
-                [False, True, False, False],  # x1 > x2
-                [False, False, False, False],
-            ]
-        else:
-            expected_values = [[False, True], [False, False]]
-
-        np.testing.assert_array_equal(
-            results.test_hypotheses(columns=columns).values, expected_values
-        )
-
-    @pytest.mark.parametrize("triangular", (True, False))
-    def test_hypothesis_heatmap(self, triangular):
-        PairwiseComparison(MEAN, COV).fit().hypothesis_heatmap(triangular=triangular)
-
-
-class TestMarginalRanking:
-    @pytest.mark.parametrize("columns", (None, ["x2", "x1"]))
-    def test_conf_int(self, columns):
-        # x0 is ranked 1 or 2
-        # s1 is ranked 0, 1, or 2
-        # x2 is ranked 0 or 1
-        results = MarginalRanking(MEAN, COV / 3).fit()
-        if columns is None:
-            expected_values = [[2, 3], [1, 3], [1, 2]]
-        else:
-            expected_values = [[1, 2], [1, 3]]
-        np.testing.assert_array_equal(
-            results.conf_int(columns=columns), expected_values
-        )
-
-
-class TestSimultaneousRanking:
-    @pytest.mark.parametrize("columns", (None, ["x2", "x1"]))
-    def test_conf_int(self, columns):
-        # x0 is ranked 1 or 2
-        # s1 is ranked 0, 1, or 2
-        # x2 is ranked 0 or 1
-        results = SimultaneousRanking(MEAN, COV / 3).fit()
-        if columns is None:
-            expected_values = [[2, 3], [1, 3], [1, 2]]
-        else:
-            expected_values = [[1, 2], [1, 3]]
-        np.testing.assert_array_equal(
-            results.conf_int(columns=columns), expected_values
-        )
-
-    @pytest.mark.parametrize("n_best_params", (1, 2))
-    @pytest.mark.parametrize("superset", (True, False))
-    def test_compute_best_params(self, n_best_params, superset):
-        # these parameters are from the stylized example in Mogstad's Inference for
-        # Rankings paper
-        x = np.array([3.3, 4.1, 4.2, 4.3, 6.2])
-        cov = np.array(
-            [
-                [0.01, 0, 0, 0, 0],
-                [0, 0.25, 0, 0, 0],
-                [0, 0, 0.05, 0, 0],
-                [0, 0, 0, 0.05, 0],
-                [0, 0, 0, 0, 0.05],
-            ]
-        )
-        results = SimultaneousRanking(x, cov).fit()
-        if n_best_params == 1:
-            # 95% chance x4 is the best parameter
-            if superset:
-                expected_values = [False, False, False, False, True]
-            else:
-                expected_values = [False, False, False, False, True]
-        else:
-            if superset:
-                # 95% chance the two best parameters are x1-x4
-                expected_values = [False, True, True, True, True]
-            else:
-                # 95% chance that x4 is in the two best parameters
-                expected_values = [False, False, False, False, True]
-        np.testing.assert_array_equal(
-            results.compute_best_params(n_best_params, superset=superset).values,
-            expected_values,
-        )
+import numpy as np
+import pytest
+from scipy.stats import norm
+
+# test for large numbers of params
+# test with groups
+
+from multiple_inference.confidence_set import (
+    ConfidenceSet,
+    AverageComparison,
+    BaselineComparison,
+    PairwiseComparison,
+    MarginalRanking,
+    SimultaneousRanking,
+)
+
+N_PARAMS = 3
+MEAN = np.arange(N_PARAMS) - (N_PARAMS - 1) / 2
+COV = np.identity(N_PARAMS)
+
+
+@pytest.mark.parametrize(
+    "cls",
+    (
+        ConfidenceSet,
+        AverageComparison,
+        BaselineComparison,
+        PairwiseComparison,
+        MarginalRanking,
+        SimultaneousRanking,
+    ),
+)
+def test_common_methods(cls):
+    # test that the common methods (conf_int, summary, point_plot) can run on all
+    # classes without error
+    kwargs = {"baseline": 0} if cls is BaselineComparison else {}
+    results = cls(MEAN, COV, **kwargs).fit()
+    results.conf_int()
+    results.summary()
+    if cls not in (MarginalRanking, SimultaneousRanking):
+        results.test_hypotheses()
+    results.point_plot()
+
+
+class TestConfidenceSet:
+    results = ConfidenceSet(MEAN, COV).fit()
+
+    def test_conf_int_shape(self):
+        assert self.results.conf_int().shape == (N_PARAMS, 2)
+
+    def test_1_param(self):
+        np.testing.assert_equal(
+            ConfidenceSet(0, 1).fit().conf_int(), [norm.ppf([0.025, 0.975])]
+        )
+
+    def test_conf_int(self):
+        # test the the marginal CI is in the simultaneous CI
+        alpha = 0.05
+        simultaneous_ci = self.results.conf_int(alpha)
+        marginal_ci = np.array(
+            [
+                norm.ppf([alpha / 2, 1 - alpha / 2], mean, np.sqrt(var))
+                for mean, var in zip(MEAN, COV.diagonal())
+            ]
+        )
+        np.testing.assert_array_less(simultaneous_ci[:, 0], marginal_ci[:, 0])
+        np.testing.assert_array_less(marginal_ci[:, 1], simultaneous_ci[:, 1])
+
+    @pytest.mark.parametrize("two_tailed", (True, False))
+    def test_test_hypotheses(self, two_tailed):
+        results = ConfidenceSet([-3, -2, 0, 2, 3], np.identity(5)).fit()
+        values = results.test_hypotheses(two_tailed=two_tailed)
+        if two_tailed:
+            np.testing.assert_array_equal(
+                values,
+                [
+                    [False, True],  # significantly less than 0
+                    [False, False],
+                    [False, False],
+                    [False, False],
+                    [True, False],  # significantly greater than 0
+                ],
+            )
+        else:
+            np.testing.assert_array_equal(values, [False, False, False, False, True])
+
+
+class TestAverageComparison:
+    def test___init__(self):
+        model = AverageComparison(MEAN, COV)
+        np.testing.assert_almost_equal(model.mean, [-1, 0, 1])
+        np.testing.assert_almost_equal(
+            model.cov,
+            [[2 / 3, -1 / 3, -1 / 3], [-1 / 3, 2 / 3, -1 / 3], [-1 / 3, -1 / 3, 2 / 3]],
+        )
+
+
+class TestBaselineComparison:
+    def test___init__(self):
+        model = BaselineComparison(MEAN, COV, baseline=0)
+        np.testing.assert_almost_equal(model.mean, [1, 2])
+        np.testing.assert_almost_equal(model.cov, [[2, 1], [1, 2]])
+
+
+class TestPairwiseComparison:
+    def test___init__(self):
+        results = PairwiseComparison(MEAN, COV).fit()
+        np.testing.assert_array_equal(
+            results.exog_names, ["x1 - x0", "x2 - x0", "x2 - x1"]
+        )
+        np.testing.assert_almost_equal(results.params, [1, 2, 1])  # [1-0, 2-0, 2-1]
+        np.testing.assert_almost_equal(results._std_diagonal, np.sqrt([2, 2, 2]))
+
+    def test_conf_int_shape(self):
+        results = PairwiseComparison(np.arange(4), np.identity(4)).fit()
+        assert results.conf_int().shape[0] == 4 * (4 - 1) / 2
+
+    @pytest.mark.parametrize("columns", (None, ["x2", "x1"]))
+    @pytest.mark.parametrize("criterion", ("fdr", "fwer"))
+    def test_test_hypotheses(self, columns, criterion):
+        results = PairwiseComparison([0, 4, 1, 2], np.identity(4) / 3).fit()
+        if columns is None:
+            if criterion == "fwer":
+                expected_values = [
+                    [False, True, False, False],  # x1 > 0
+                    [False, False, False, False],
+                    [False, True, False, False],  # x1 > x2
+                    [False, False, False, False],
+                ]
+            else:
+                expected_values = [
+                    [False, True, False, True],
+                    [True, False, True, True],
+                    [False, True, False, False],
+                    [True, True, False, False],
+                ]
+        else:
+            if criterion == "fwer":
+                expected_values = [[False, True], [False, False]]
+            else:
+                expected_values = [[False, True], [True, False]]
+
+        np.testing.assert_array_equal(
+            results.test_hypotheses(criterion=criterion, columns=columns).values,
+            expected_values,
+        )
+
+    def test_large_n_params(self, n_params=500):
+        results = PairwiseComparison(np.arange(n_params), np.identity(n_params)).fit(
+            n_samples=1000
+        )
+        results.summary()
+        results.test_hypotheses()
+
+    @pytest.mark.parametrize("triangular", (True, False))
+    def test_hypothesis_heatmap(self, triangular):
+        PairwiseComparison(MEAN, COV).fit().hypothesis_heatmap(triangular=triangular)
+
+
+@pytest.fixture(scope="module")
+def pairwise_groups(n_params=5):
+    # make groups of (x0, x2, x4) and (x1, x3)
+    groups = np.full(n_params, 0)
+    groups[[i for i in range(n_params) if i % 2 == 1]] = 1
+    return PairwiseComparison(np.arange(n_params), np.identity(n_params)).fit(
+        groups=groups
+    )
+
+
+class TestPairwiseGroups:
+    def test_exog_names(self, pairwise_groups):
+        np.testing.assert_equal(
+            pairwise_groups.exog_names, ["x2 - x0", "x4 - x0", "x4 - x2", "x3 - x1"]
+        )
+
+    def test_test_hypotheses(self, pairwise_groups):
+        results = pairwise_groups.test_hypotheses()
+        assert results[0].shape == (3, 3)  # group of x0, x2, x4
+        assert results[1].shape == (2, 2)  # group of x1, x3
+
+    def test_hypothesis_heatmap(self, pairwise_groups):
+        pairwise_groups.hypothesis_heatmap()
+
+
+class TestMarginalRanking:
+    @pytest.mark.parametrize("columns", (None, ["x2", "x1"]))
+    def test_conf_int(self, columns):
+        # x0 is ranked 1 or 2
+        # s1 is ranked 0, 1, or 2
+        # x2 is ranked 0 or 1
+        results = MarginalRanking(MEAN, COV / 3).fit()
+        if columns is None:
+            expected_values = [[2, 3], [1, 3], [1, 2]]
+        else:
+            expected_values = [[1, 2], [1, 3]]
+        np.testing.assert_array_equal(
+            results.conf_int(columns=columns), expected_values
+        )
+
+
+class TestSimultaneousRanking:
+    @pytest.mark.parametrize("columns", (None, ["x2", "x1"]))
+    def test_conf_int(self, columns):
+        # x0 is ranked 1 or 2
+        # s1 is ranked 0, 1, or 2
+        # x2 is ranked 0 or 1
+        results = SimultaneousRanking(MEAN, COV / 3).fit()
+        if columns is None:
+            expected_values = [[2, 3], [1, 3], [1, 2]]
+        else:
+            expected_values = [[1, 2], [1, 3]]
+        np.testing.assert_array_equal(
+            results.conf_int(columns=columns), expected_values
+        )
+
+    @pytest.mark.parametrize("n_best_params", (1, 2))
+    @pytest.mark.parametrize("superset", (True, False))
+    def test_compute_best_params(self, n_best_params, superset):
+        # these parameters are from the stylized example in Mogstad's Inference for
+        # Rankings paper
+        x = np.array([3.3, 4.1, 4.2, 4.3, 6.2])
+        cov = np.array(
+            [
+                [0.01, 0, 0, 0, 0],
+                [0, 0.25, 0, 0, 0],
+                [0, 0, 0.05, 0, 0],
+                [0, 0, 0, 0.05, 0],
+                [0, 0, 0, 0, 0.05],
+            ]
+        )
+        results = SimultaneousRanking(x, cov).fit()
+        if n_best_params == 1:
+            # 95% chance x4 is the best parameter
+            if superset:
+                expected_values = [False, False, False, False, True]
+            else:
+                expected_values = [False, False, False, False, True]
+        else:
+            if superset:
+                # 95% chance the two best parameters are x1-x4
+                expected_values = [False, True, True, True, True]
+            else:
+                # 95% chance that x4 is in the two best parameters
+                expected_values = [False, False, False, False, True]
+        np.testing.assert_array_equal(
+            results.compute_best_params(n_best_params, superset=superset).values,
+            expected_values,
+        )
+
+    def test_large_n_params(self, n_params=500):
+        results = SimultaneousRanking(np.arange(n_params), np.identity(n_params)).fit(
+            n_samples=1000
+        )
+        results.summary()
+        results.compute_best_params()
```

### Comparing `multiple-inference-1.1.0/tests/test_rank_condition.py` & `multiple-inference-1.2.0/tests/test_rank_condition.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import numpy as np
-import pytest
-
-from conditional_inference.rank_condition import RankCondition
-
-
-def test_common_methods():
-    model = RankCondition(np.arange(3), np.identity(3))
-    results = model.fit()
-    results.conf_int()
-    results.summary()
-    results.point_plot()
-
-
-class TestRankCondition:
-    model = RankCondition(np.arange(3), np.diag([1, 2, 3]) ** 2)
-
-    @pytest.mark.parametrize("column", ("x0", "x1", "x2"))
-    @pytest.mark.parametrize("beta", (0, 0.005))
-    def test_get_marginal_distribution(self, column, beta):
-        dist = self.model.get_marginal_distribution(column, beta=beta)
-
-        if column == "x0":
-            expected_truncation_set = [-np.inf, 1]
-            expected_scale = 1
-            expected_y = 0
-        elif column == "x1":
-            expected_truncation_set = [0, 2]
-            expected_scale = 2
-            expected_y = 1
-        else:
-            expected_truncation_set = [1, np.inf]
-            expected_scale = 3
-            expected_y = 2
-
-        np.testing.assert_almost_equal(
-            dist.truncnorm_kwargs["truncation_set"][0], expected_truncation_set
-        )
-        assert dist.truncnorm_kwargs["scale"] == expected_scale
-        assert dist.y == expected_y
-
-        assert (dist.projection_interval == (-np.inf, np.inf)) == (beta == 0)
-
-    @pytest.mark.parametrize("rank", ([0], [0, 1], [0, 1, 2]))
-    def test_truncation_set(self, rank):
-        dist = self.model.get_marginal_distribution("x2", rank)
-
-        if rank == [0]:
-            expected_value = [[1, np.inf]]
-        elif rank == [0, 1]:
-            expected_value = [[0, 1], [1, np.inf]]
-        else:
-            expected_value = [[-np.inf, 0], [0, 1], [1, np.inf]]
-
-        np.testing.assert_almost_equal(
-            dist.truncnorm_kwargs["truncation_set"], expected_value
-        )
+import numpy as np
+import pytest
+
+from multiple_inference.rank_condition import RankCondition
+
+
+def test_common_methods():
+    model = RankCondition(np.arange(3), np.identity(3))
+    results = model.fit()
+    results.conf_int()
+    results.summary()
+    results.point_plot()
+
+
+class TestRankCondition:
+    model = RankCondition(np.arange(3), np.diag([1, 2, 3]) ** 2)
+
+    @pytest.mark.parametrize("column", ("x0", "x1", "x2"))
+    @pytest.mark.parametrize("beta", (0, 0.005))
+    def test_get_marginal_distribution(self, column, beta):
+        dist = self.model.get_marginal_distribution(column, beta=beta)
+
+        if column == "x0":
+            expected_truncation_set = [-np.inf, 1]
+            expected_scale = 1
+            expected_y = 0
+        elif column == "x1":
+            expected_truncation_set = [0, 2]
+            expected_scale = 2
+            expected_y = 1
+        else:
+            expected_truncation_set = [1, np.inf]
+            expected_scale = 3
+            expected_y = 2
+
+        np.testing.assert_almost_equal(
+            dist.truncnorm_kwargs["truncation_set"][0], expected_truncation_set
+        )
+        assert dist.truncnorm_kwargs["scale"] == expected_scale
+        assert dist.y == expected_y
+
+        assert (dist.projection_interval == (-np.inf, np.inf)) == (beta == 0)
+
+    @pytest.mark.parametrize("rank", ([0], [0, 1], [0, 1, 2]))
+    def test_truncation_set(self, rank):
+        dist = self.model.get_marginal_distribution("x2", rank)
+
+        if rank == [0]:
+            expected_value = [[1, np.inf]]
+        elif rank == [0, 1]:
+            expected_value = [[0, 1], [1, np.inf]]
+        else:
+            expected_value = [[-np.inf, 0], [0, 1], [1, np.inf]]
+
+        np.testing.assert_almost_equal(
+            dist.truncnorm_kwargs["truncation_set"], expected_value
+        )
```

### Comparing `multiple-inference-1.1.0/tests/test_stats.py` & `multiple-inference-1.2.0/tests/test_stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,170 +1,182 @@
-from itertools import product
-
-import numpy as np
-import pytest
-from numpy.testing import assert_allclose
-from scipy.stats import norm, truncnorm as scipy_truncnorm
-
-from conditional_inference.stats import (
-    joint_distribution,
-    mixture,
-    nonparametric,
-    quantile_unbiased,
-    truncnorm,
-)
-
-
-VALUES = np.linspace(-2, 2, num=5)
-LOC = [-1, 0, 1]
-SCALE = [1, 2]
-TRUNCATION_SET = [(-np.inf, -1), (-1, 1), (1, np.inf)]
-
-
-class TestJointDistribution:
-    marginals = [norm(), norm(4)]
-    dist = joint_distribution(marginals)
-    values = np.vstack([marginals[0].rvs(10), marginals[1].rvs(10)]).T
-
-    def test_logpdf(self):
-        np.testing.assert_array_almost_equal(
-            self.dist.logpdf(self.values),
-            self.marginals[0].logpdf(self.values[:, 0])
-            + self.marginals[1].logpdf(self.values[:, 1]),
-        )
-
-    def test_pdf(self):
-        np.testing.assert_array_almost_equal(
-            self.dist.pdf(self.values),
-            self.marginals[0].pdf(self.values[:, 0])
-            * self.marginals[1].pdf(self.values[:, 1]),
-        )
-
-    @pytest.mark.parametrize("size", (1, 10))
-    def test_rvs(self, size):
-        assert self.dist.rvs(size).shape == (size, 2)
-
-
-class TestMixture:
-    mixed = [norm(), norm(4)]
-    dist = mixture(mixed)
-
-    def test_pdf(self):
-        np.testing.assert_array_almost_equal(
-            self.dist.pdf(VALUES),
-            0.5 * (self.mixed[0].pdf(VALUES) + self.mixed[1].pdf(VALUES)),
-        )
-
-    def test_cdf(self):
-        np.testing.assert_array_almost_equal(
-            self.dist.cdf(VALUES),
-            0.5 * (self.mixed[0].cdf(VALUES) + self.mixed[1].cdf(VALUES)),
-        )
-
-    def test_mean(self):
-        assert self.dist.mean() == 0.5 * (self.mixed[0].mean() + self.mixed[1].mean())
-
-    def test_variance(self):
-        assert self.dist.var() == 0.5 * (self.mixed[0].var() + self.mixed[1].var())
-
-
-class TestNonparametric:
-    x = np.linspace(-3, 3)
-    dist = nonparametric((x, norm.pdf(x)))
-
-    def test_pdf(self):
-        np.testing.assert_array_almost_equal(
-            self.dist.pdf(self.x), norm.pdf(self.x), decimal=2
-        )
-
-    def test_cdf(self):
-        np.testing.assert_array_almost_equal(
-            self.dist.cdf(self.x), norm.cdf(self.x), decimal=1
-        )
-
-    def test_ppf(self):
-        q = np.linspace(0.025, 0.975, num=10)
-        np.testing.assert_array_almost_equal(self.dist.ppf(q), norm.ppf(q), decimal=2)
-
-    def test_mean(self):
-        assert abs(self.dist.mean() - norm.mean()) < 0.01
-
-    def test_std(self):
-        assert abs(self.dist.std() - norm.std()) < 0.02
-
-
-@pytest.fixture(scope="module", params=list(product(LOC, SCALE, TRUNCATION_SET)))
-def quantile_unbiased_distribution(request):
-    loc, scale, truncation_set = request.param
-    return quantile_unbiased(loc, scale=scale, truncation_set=[truncation_set])
-
-
-class TestQuantileUnbiased:
-    # the quantile unbiased distribution behaves like a normal when the truncation set
-    # is all real values
-    untruncated_dist = quantile_unbiased(0, scale=1, truncation_set=[(-np.inf, np.inf)])
-
-    def test_pdf(self, quantile_unbiased_distribution):
-        quantile_unbiased_distribution.pdf(VALUES)
-
-    def test_untruncated_pdf(self):
-        x = np.linspace(-2, 2)
-        np.testing.assert_array_almost_equal(self.untruncated_dist.pdf(x), norm.pdf(x))
-
-    def test_cdf(self, quantile_unbiased_distribution):
-        quantile_unbiased_distribution.cdf(VALUES)
-
-    def test_untruncated_cdf(self):
-        x = np.linspace(-2, 2)
-        np.testing.assert_array_almost_equal(self.untruncated_dist.cdf(x), norm.cdf(x))
-
-    def test_ppf(self, quantile_unbiased_distribution):
-        quantile_unbiased_distribution.ppf(np.linspace(0, 1, 5))
-
-    def test_untruncated_ppf(self):
-        x = np.linspace(0.025, 0.975, 5)
-        np.testing.assert_almost_equal(self.untruncated_dist.ppf(x), norm.ppf(x))
-
-
-@pytest.fixture(scope="module", params=list(product(LOC, SCALE, TRUNCATION_SET)))
-def truncnorm_distributions(request):
-    loc, scale, truncation_set = request.param
-    return (
-        truncnorm([truncation_set], loc=loc, scale=scale),
-        scipy_truncnorm(*truncation_set, loc=loc, scale=scale),
-    )
-
-
-class TestTruncnorm:
-    # test that conditional inference truncnorm behaves like scipy truncnorm
-    # for reasonable ranges of values
-    # conditional inference truncnorm should perform better in tails
-    def test_pdf(self, truncnorm_distributions):
-        dist0, dist1 = truncnorm_distributions
-        assert_allclose(dist0.pdf(VALUES), dist1.pdf(VALUES), atol=1e-3)
-
-    def test_logpdf(self, truncnorm_distributions):
-        dist0, dist1 = truncnorm_distributions
-        assert_allclose(dist0.logpdf(VALUES), dist1.logpdf(VALUES), atol=1e-3)
-
-    def test_cdf(self, truncnorm_distributions):
-        dist0, dist1 = truncnorm_distributions
-        assert_allclose(dist0.cdf(VALUES), dist1.cdf(VALUES), atol=1e-3)
-
-    def test_logcdf(self, truncnorm_distributions):
-        dist0, dist1 = truncnorm_distributions
-        assert_allclose(dist0.logcdf(VALUES), dist1.logcdf(VALUES), atol=1e-3)
-
-    def test_tails(self):
-        # test that truncnorm can handle extreme truncation sets
-        assert truncnorm([(8, np.inf)]).cdf(8.5) < 1
-        assert truncnorm([(-np.inf, -8)]).cdf(-8.5) > 0
-        assert truncnorm([(100, np.inf)]).cdf(101) <= 1
-        assert truncnorm([(-np.inf, -100)]).cdf(-101) >= 0
-
-    def test_default_truncation_set(self):
-        assert_allclose(
-            truncnorm().ppf([0.25, 0.5, 0.75]), norm().ppf([0.25, 0.5, 0.75])
-        )
-
-    def test_concave_truncation_set(self):
-        truncnorm([(-2, -1), (1, 2)]).ppf([0.05, 0.25, 0.5, 0.75, 0.95])
+from itertools import product
+
+import numpy as np
+import pytest
+from numpy.testing import assert_allclose
+from scipy.optimize import minimize_scalar
+from scipy.stats import norm, truncnorm as scipy_truncnorm
+
+from multiple_inference.stats import (
+    joint_distribution,
+    mixture,
+    nonparametric,
+    quantile_unbiased,
+    truncnorm,
+)
+
+
+VALUES = np.linspace(-2, 2, num=5)
+LOC = [-1, 0, 1]
+SCALE = [1, 2]
+TRUNCATION_SET = [(-np.inf, -1), (-1, 1), (1, np.inf)]
+
+
+class TestJointDistribution:
+    marginals = [norm(), norm(4)]
+    dist = joint_distribution(marginals)
+    values = np.vstack([marginals[0].rvs(10), marginals[1].rvs(10)]).T
+
+    def test_logpdf(self):
+        np.testing.assert_array_almost_equal(
+            self.dist.logpdf(self.values),
+            self.marginals[0].logpdf(self.values[:, 0])
+            + self.marginals[1].logpdf(self.values[:, 1]),
+        )
+
+    def test_pdf(self):
+        np.testing.assert_array_almost_equal(
+            self.dist.pdf(self.values),
+            self.marginals[0].pdf(self.values[:, 0])
+            * self.marginals[1].pdf(self.values[:, 1]),
+        )
+
+    @pytest.mark.parametrize("size", (1, 10))
+    def test_rvs(self, size):
+        assert self.dist.rvs(size).shape == (size, 2)
+
+
+class TestMixture:
+    mixed = [norm(), norm(4)]
+    dist = mixture(mixed)
+
+    def test_pdf(self):
+        np.testing.assert_array_almost_equal(
+            self.dist.pdf(VALUES),
+            0.5 * (self.mixed[0].pdf(VALUES) + self.mixed[1].pdf(VALUES)),
+        )
+
+    def test_cdf(self):
+        np.testing.assert_array_almost_equal(
+            self.dist.cdf(VALUES),
+            0.5 * (self.mixed[0].cdf(VALUES) + self.mixed[1].cdf(VALUES)),
+        )
+
+    def test_mean(self):
+        assert self.dist.mean() == 0.5 * (self.mixed[0].mean() + self.mixed[1].mean())
+
+    def test_variance(self):
+        assert self.dist.var() == 0.5 * (self.mixed[0].var() + self.mixed[1].var())
+
+    def test_std(self):
+        assert self.dist.std() == np.sqrt(
+            0.5 * (self.mixed[0].var() + self.mixed[1].var())
+        )
+
+
+class TestNonparametric:
+    x = np.linspace(-3, 3)
+    dist = nonparametric((x, norm.pdf(x)))
+
+    def test_pdf(self):
+        np.testing.assert_array_almost_equal(
+            self.dist.pdf(self.x), norm.pdf(self.x), decimal=2
+        )
+
+    def test_cdf(self):
+        np.testing.assert_array_almost_equal(
+            self.dist.cdf(self.x), norm.cdf(self.x), decimal=1
+        )
+
+    def test_ppf(self):
+        q = np.linspace(0.05, 0.95, num=10)
+        np.testing.assert_array_almost_equal(self.dist.ppf(q), norm.ppf(q), decimal=2)
+
+    def test_mean(self):
+        assert abs(self.dist.mean() - norm.mean()) < 0.01
+
+    def test_std(self):
+        assert abs(self.dist.std() - norm.std()) < 0.02
+
+    def test_pdf_gt_0(self):
+        # earlier versions used a cubic spline which could go below zero
+        dist = nonparametric(([0, 1, 2, 3], [0.05, 0.1, 0.4, 0.25]))
+        result = minimize_scalar(dist.pdf, bounds=(0, 3))
+        assert result.fun >= 0
+
+
+@pytest.fixture(scope="module", params=list(product(LOC, SCALE, TRUNCATION_SET)))
+def quantile_unbiased_distribution(request):
+    loc, scale, truncation_set = request.param
+    return quantile_unbiased(loc, scale=scale, truncation_set=[truncation_set])
+
+
+class TestQuantileUnbiased:
+    # the quantile unbiased distribution behaves like a normal when the truncation set
+    # is all real values
+    untruncated_dist = quantile_unbiased(0, scale=1, truncation_set=[(-np.inf, np.inf)])
+
+    def test_pdf(self, quantile_unbiased_distribution):
+        quantile_unbiased_distribution.pdf(VALUES)
+
+    def test_untruncated_pdf(self):
+        x = np.linspace(-2, 2)
+        np.testing.assert_array_almost_equal(self.untruncated_dist.pdf(x), norm.pdf(x))
+
+    def test_cdf(self, quantile_unbiased_distribution):
+        quantile_unbiased_distribution.cdf(VALUES)
+
+    def test_untruncated_cdf(self):
+        x = np.linspace(-2, 2)
+        np.testing.assert_array_almost_equal(self.untruncated_dist.cdf(x), norm.cdf(x))
+
+    def test_ppf(self, quantile_unbiased_distribution):
+        quantile_unbiased_distribution.ppf(np.linspace(0, 1, 5))
+
+    def test_untruncated_ppf(self):
+        x = np.linspace(0.025, 0.975, 5)
+        np.testing.assert_almost_equal(self.untruncated_dist.ppf(x), norm.ppf(x))
+
+
+@pytest.fixture(scope="module", params=list(product(LOC, SCALE, TRUNCATION_SET)))
+def truncnorm_distributions(request):
+    loc, scale, truncation_set = request.param
+    return (
+        truncnorm([truncation_set], loc=loc, scale=scale),
+        scipy_truncnorm(*truncation_set, loc=loc, scale=scale),
+    )
+
+
+class TestTruncnorm:
+    # test that conditional inference truncnorm behaves like scipy truncnorm
+    # for reasonable ranges of values
+    # conditional inference truncnorm should perform better in tails
+    def test_pdf(self, truncnorm_distributions):
+        dist0, dist1 = truncnorm_distributions
+        assert_allclose(dist0.pdf(VALUES), dist1.pdf(VALUES), atol=1e-3)
+
+    def test_logpdf(self, truncnorm_distributions):
+        dist0, dist1 = truncnorm_distributions
+        assert_allclose(dist0.logpdf(VALUES), dist1.logpdf(VALUES), atol=1e-3)
+
+    def test_cdf(self, truncnorm_distributions):
+        dist0, dist1 = truncnorm_distributions
+        assert_allclose(dist0.cdf(VALUES), dist1.cdf(VALUES), atol=1e-3)
+
+    def test_logcdf(self, truncnorm_distributions):
+        dist0, dist1 = truncnorm_distributions
+        assert_allclose(dist0.logcdf(VALUES), dist1.logcdf(VALUES), atol=1e-3)
+
+    def test_tails(self):
+        # test that truncnorm can handle extreme truncation sets
+        assert truncnorm([(8, np.inf)]).cdf(8.5) < 1
+        assert truncnorm([(-np.inf, -8)]).cdf(-8.5) > 0
+        assert truncnorm([(100, np.inf)]).cdf(101) <= 1
+        assert truncnorm([(-np.inf, -100)]).cdf(-101) >= 0
+
+    def test_default_truncation_set(self):
+        assert_allclose(
+            truncnorm().ppf([0.25, 0.5, 0.75]), norm().ppf([0.25, 0.5, 0.75])
+        )
+
+    def test_concave_truncation_set(self):
+        truncnorm([(-2, -1), (1, 2)]).ppf([0.05, 0.25, 0.5, 0.75, 0.95])
```

### Comparing `multiple-inference-1.1.0/tests/test_utils.py` & `multiple-inference-1.2.0/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from turtle import home
-from unittest.mock import Mock
-
-import numpy as np
-from scipy.stats import multivariate_normal
-
-from conditional_inference.utils import (
-    expected_wasserstein_distance,
-    holm_bonferroni_correction,
-    weighted_quantile,
-)
-
-
-def test_expected_wasserstein_distance():
-    # expected Wasserstein distance should be smaller when the parameters are estimated with greater precision
-    n_params = 3
-    mean, cov = np.arange(n_params), np.identity(n_params)
-    rvs0 = multivariate_normal.rvs(mean, 1, size=100)
-    rvs1 = multivariate_normal.rvs(mean, 0.1 ** 2, size=100)
-    assert expected_wasserstein_distance(
-        mean, cov, rvs0
-    ) > expected_wasserstein_distance(mean, cov, rvs1)
-
-
-def test_holm_bonferroni_correction():
-    results = Mock()
-    results.pvalues = np.array([0.1, 0.05, 0.01])
-    results.model = Mock()
-    results.model.exog_names = np.array(["x0", "x1", "x2"])
-    correction = holm_bonferroni_correction(results=results)
-    np.testing.assert_array_equal(correction.pvalues, [0.01, 0.05, 0.1])
-    np.testing.assert_array_equal(correction.significant, [True, False, False])
-    np.testing.assert_array_equal(correction.index, ["x2", "x1", "x0"])
-
-
-def test_weighted_quantile():
-    quantiles = [0, 0.25, 0.5, 0.75, 1]
-    np.testing.assert_array_almost_equal(
-        weighted_quantile(np.linspace(0, 1), quantiles), quantiles, decimal=2
-    )
+from turtle import home
+from unittest.mock import Mock
+
+import numpy as np
+from scipy.stats import multivariate_normal
+
+from multiple_inference.utils import (
+    expected_wasserstein_distance,
+    holm_bonferroni_correction,
+    weighted_quantile,
+)
+
+
+def test_expected_wasserstein_distance():
+    # expected Wasserstein distance should be smaller when the parameters are estimated with greater precision
+    n_params = 3
+    mean, cov = np.arange(n_params), np.identity(n_params)
+    rvs0 = multivariate_normal.rvs(mean, 1, size=100)
+    rvs1 = multivariate_normal.rvs(mean, 0.1**2, size=100)
+    assert expected_wasserstein_distance(
+        mean, cov, rvs0
+    ) > expected_wasserstein_distance(mean, cov, rvs1)
+
+
+def test_holm_bonferroni_correction():
+    results = Mock()
+    results.pvalues = np.array([0.1, 0.05, 0.01])
+    results.model = Mock()
+    results.model.exog_names = np.array(["x0", "x1", "x2"])
+    correction = holm_bonferroni_correction(results=results)
+    np.testing.assert_array_equal(correction.pvalues, [0.01, 0.05, 0.1])
+    np.testing.assert_array_equal(correction.significant, [True, False, False])
+    np.testing.assert_array_equal(correction.index, ["x2", "x1", "x0"])
+
+
+def test_weighted_quantile():
+    quantiles = [0, 0.25, 0.5, 0.75, 1]
+    np.testing.assert_array_almost_equal(
+        weighted_quantile(np.linspace(0, 1), quantiles), quantiles, decimal=2
+    )
```

