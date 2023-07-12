# Comparing `tmp/rubicon-ml-0.4.4.tar.gz` & `tmp/rubicon-ml-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubicon-ml-0.4.4.tar", last modified: Wed Apr 19 18:45:21 2023, max compression
+gzip compressed data, was "rubicon-ml-0.4.5.tar", last modified: Wed Jul 12 19:53:07 2023, max compression
```

## Comparing `rubicon-ml-0.4.4.tar` & `rubicon-ml-0.4.5.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/rubicon_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/rubicon_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.209481 rubicon-ml-0.4.4/rubicon_ml/client/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    16101 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/rubicon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.209481 rubicon-ml-0.4.4/rubicon_ml/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/utils/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/utils/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/domain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/utils/training_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/utils/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/publish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/repository/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/utils/slugify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/estimator_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/filter_estimator_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.209481 rubicon-ml-0.4.4/rubicon_ml/viz/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/common.css
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/dropdown-header.css
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/experiments-table.css
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/frame.css
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/metric-correlation-plot.css
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/metric-lists-comparison.css
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/plots-comparison.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/viz/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/images/rubicon-logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/viz/common/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/common/dropdown_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/dataframe_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/experiments_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/metric_correlation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/metric_lists_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/rubicon_ml/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.209481 rubicon-ml-0.4.4/rubicon_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.677426 rubicon-ml-0.4.5/rubicon_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-12 19:53:07.677426 rubicon-ml-0.4.5/rubicon_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.665425 rubicon-ml-0.4.5/rubicon_ml/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/rubicon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.665425 rubicon-ml-0.4.5/rubicon_ml/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/utils/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/client/utils/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/domain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/utils/training_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/domain/utils/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/publish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44598 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/repository/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/repository/utils/slugify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.669426 rubicon-ml-0.4.5/rubicon_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/estimator_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/filter_estimator_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/sklearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.661425 rubicon-ml-0.4.5/rubicon_ml/viz/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/common.css
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/dropdown-header.css
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/experiments-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/frame.css
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/metric-correlation-plot.css
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/metric-lists-comparison.css
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/css/plots-comparison.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/viz/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/assets/images/rubicon-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/viz/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/common/dropdown_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/dataframe_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/experiments_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/metric_correlation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/viz/metric_lists_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.665425 rubicon-ml-0.4.5/rubicon_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 19:53:07.000000 rubicon-ml-0.4.5/rubicon_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-12 19:53:07.677426 rubicon-ml-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:53:07.673426 rubicon-ml-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-07-12 19:52:54.000000 rubicon-ml-0.4.5/versioneer.py
```

### Comparing `rubicon-ml-0.4.4/LICENSE` & `rubicon-ml-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/PKG-INFO` & `rubicon-ml-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-ml
-Version: 0.4.4
+Version: 0.4.5
 Summary: "an ML library for model development and governance"
 Home-page: https://github.com/capitalone/rubicon-ml
 Author: "Joe Wolfe, Ryan Soley, Diane Lee, Mike McCarty, CapitalOne"
 License: "Apache License, Version 2.0"
 Project-URL: Documentation, https://capitalone.github.io/rubicon-ml/
 Project-URL: Bug Tracker, https://github.com/capitalone/rubicon-ml/issues
 Project-URL: Source Code, https://github.com/capitalone/rubicon-ml
```

### Comparing `rubicon-ml-0.4.4/README.md` & `rubicon-ml-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/__init__.py` & `rubicon-ml-0.4.5/rubicon_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/cli.py` & `rubicon-ml-0.4.5/rubicon_ml/cli.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/__init__.py` & `rubicon-ml-0.4.5/rubicon_ml/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/artifact.py` & `rubicon-ml-0.4.5/rubicon_ml/client/artifact.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import warnings
 
 import fsspec
 
 from rubicon_ml.client.base import Base
 from rubicon_ml.client.mixin import TagMixin
 from rubicon_ml.client.utils.exception_handling import failsafe
+from rubicon_ml.exceptions import RubiconException
 
 
 class Artifact(Base, TagMixin):
     """A client artifact.
 
     An `artifact` is a catch-all for any other type of
     data that can be logged to a file.
@@ -36,37 +37,51 @@
 
         self._data = None
         self._parent = parent
 
     def _get_data(self):
         """Loads the data associated with this artifact."""
         project_name, experiment_id = self.parent._get_identifiers()
-
-        self._data = self.repository.get_artifact_data(
-            project_name, self.id, experiment_id=experiment_id
-        )
+        return_err = None
+        for repo in self.repositories:
+            self._data = None
+            try:
+                self._data = repo.get_artifact_data(
+                    project_name, self.id, experiment_id=experiment_id
+                )
+            except Exception as err:
+                return_err = err
+            else:
+                return
+        if self._data is None:
+            raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def get_data(self, unpickle=False):
         """Loads the data associated with this artifact and
         unpickles if needed.
 
         Parameters
         ----------
         unpickle : bool, optional
             Flag indicating whether artifact data must be
             unpickled. Will be returned as bytes by default.
         """
         project_name, experiment_id = self.parent._get_identifiers()
-
-        data = self.repository.get_artifact_data(project_name, self.id, experiment_id=experiment_id)
-        if unpickle:
-            data = pickle.loads(data)
-
-        return data
+        return_err = None
+        for repo in self.repositories:
+            try:
+                data = repo.get_artifact_data(project_name, self.id, experiment_id=experiment_id)
+            except Exception as err:
+                return_err = err
+            else:
+                if unpickle:
+                    data = pickle.loads(data)
+                return data
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def download(self, location=None, name=None):
         """Download this artifact's data.
 
         Parameters
         ----------
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/base.py` & `rubicon-ml-0.4.5/rubicon_ml/client/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,7 +15,14 @@
 
     def __str__(self):
         return self._domain.__str__()
 
     @property
     def repository(self):
         return self._config.repository
+
+    @property
+    def repositories(self):
+        if hasattr(self._config, "repositories"):
+            return self._config.repositories
+        else:
+            return [self._config.repository]
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/config.py` & `rubicon-ml-0.4.5/rubicon_ml/client/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,20 +34,30 @@
         "filesystem-local": LocalRepository,
         "filesystem-s3": S3Repository,
     }
 
     def __init__(
         self, persistence=None, root_dir=None, is_auto_git_enabled=False, **storage_options
     ):
-        self.persistence, self.root_dir, self.is_auto_git_enabled = self._load_config(
-            persistence, root_dir, is_auto_git_enabled
-        )
         self.storage_options = storage_options
-
-        self.repository = self._get_repository()
+        if storage_options is not None and "composite_config" in storage_options:
+            composite_config = storage_options.get("composite_config")
+            repositories = []
+            for config in composite_config:
+                self.persistence, self.root_dir, self.is_auto_git_enabled = self._load_config(
+                    config["persistence"], config["root_dir"], is_auto_git_enabled
+                )
+                repositories.append(self._get_repository())
+
+            self.repositories = repositories
+        else:
+            self.persistence, self.root_dir, self.is_auto_git_enabled = self._load_config(
+                persistence, root_dir, is_auto_git_enabled
+            )
+            self.repository = self._get_repository()
 
     def _check_is_in_git_repo(self):
         """Raise a `RubiconException` if not called from within a `git` repository."""
         if subprocess.run(["git", "rev-parse", "--git-dir"], capture_output=True).returncode != 0:
             raise RubiconException(
                 "Not a `git` repo: Falied to locate the '.git' directory in this or any parent directories."
             )
@@ -89,8 +99,8 @@
         if repository is None:
             raise RubiconException(
                 f"{self.__class__.__module__}.{self.__class__.__name__} has no persistence "
                 + f"layer for the provided configuration: `persistence`: {self.persistence}, "
                 + f"`protocol` (from `root_dir`): {protocol}"
             )
 
-        return repository(self.root_dir, **self.storage_options)
+        return repository(root_dir=self.root_dir, **self.storage_options)
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/dataframe.py` & `rubicon-ml-0.4.5/rubicon_ml/client/dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,23 +38,29 @@
         Parameters
         ----------
         df_type : str, optional
             The type of dataframe to return. Valid options include
             ["dask", "pandas"]. Defaults to "pandas".
         """
         project_name, experiment_id = self.parent._get_identifiers()
+        return_err = None
+        for repo in self.repositories:
+            try:
+                self._data = repo.get_dataframe_data(
+                    project_name,
+                    self.id,
+                    experiment_id=experiment_id,
+                    df_type=df_type,
+                )
+            except Exception as err:
+                return_err = err
+            else:
+                return self._data
 
-        self._data = self.repository.get_dataframe_data(
-            project_name,
-            self.id,
-            experiment_id=experiment_id,
-            df_type=df_type,
-        )
-
-        return self._data
+        raise RubiconException(return_err)
 
     @failsafe
     def plot(self, df_type="pandas", plotting_func=None, **kwargs):
         """Render the dataframe using `plotly.express`.
 
         Parameters
         ----------
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/experiment.py` & `rubicon-ml-0.4.5/rubicon_ml/client/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Feature,
     Metric,
     Parameter,
     TagMixin,
 )
 from rubicon_ml.client.utils.exception_handling import failsafe
 from rubicon_ml.client.utils.tags import filter_children
+from rubicon_ml.exceptions import RubiconException
 
 
 class Experiment(Base, ArtifactMixin, DataframeMixin, TagMixin):
     """A client experiment.
 
     An `experiment` represents a model run and is identified by
     its 'created_at' time. It can have `metrics`, `parameters`,
@@ -72,15 +73,16 @@
         """
         if not isinstance(tags, list) or not all([isinstance(tag, str) for tag in tags]):
             raise ValueError("`tags` must be `list` of type `str`")
 
         metric = domain.Metric(
             name, value, directionality=directionality, description=description, tags=tags
         )
-        self.repository.create_metric(metric, self.project.name, self.id)
+        for repo in self.repositories:
+            repo.create_metric(metric, self.project.name, self.id)
 
         return Metric(metric, self)
 
     @failsafe
     def metrics(self, name=None, tags=[], qtype="or"):
         """Get the metrics logged to this experiment.
 
@@ -95,18 +97,25 @@
             'and'. Defaults to 'or'.
 
         Returns
         -------
         list of rubicon.client.Metric
             The metrics previously logged to this experiment.
         """
-        metrics = [Metric(m, self) for m in self.repository.get_metrics(self.project.name, self.id)]
-        self._metrics = filter_children(metrics, tags, qtype, name)
+        return_err = None
+        for repo in self.repositories:
+            try:
+                metrics = [Metric(m, self) for m in repo.get_metrics(self.project.name, self.id)]
+            except Exception as err:
+                return_err = err
+            else:
+                self._metrics = filter_children(metrics, tags, qtype, name)
+                return self._metrics
 
-        return self._metrics
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def metric(self, name=None, id=None):
         """Get a metric.
 
         Parameters
         ----------
@@ -120,20 +129,27 @@
         rubicon.client.Metric
             The metric with name `name` or id `id`.
         """
         if (name is None and id is None) or (name is not None and id is not None):
             raise ValueError("`name` OR `id` required.")
 
         if name is not None:
-            metric = self.repository.get_metric(self.project.name, self.id, name)
-            metric = Metric(metric, self)
+            return_err = None
+            for repo in self.repositories:
+                try:
+                    metric = repo.get_metric(self.project.name, self.id, name)
+                except Exception as err:
+                    return_err = err
+                else:
+                    metric = Metric(metric, self)
+                    return metric
+            raise RubiconException("all configured storage backends failed") from return_err
         else:
             metric = [m for m in self.metrics() if m.id == id][0]
-
-        return metric
+            return metric
 
     @failsafe
     def log_feature(self, name, description=None, importance=None, tags=[]):
         """Create a feature under the experiment.
 
         Parameters
         ----------
@@ -153,15 +169,16 @@
         rubicon.client.Feature
             The created feature.
         """
         if not isinstance(tags, list) or not all([isinstance(tag, str) for tag in tags]):
             raise ValueError("`tags` must be `list` of type `str`")
 
         feature = domain.Feature(name, description=description, importance=importance, tags=tags)
-        self.repository.create_feature(feature, self.project.name, self.id)
+        for repo in self.repositories:
+            repo.create_feature(feature, self.project.name, self.id)
 
         return Feature(feature, self)
 
     @failsafe
     def features(self, name=None, tags=[], qtype="or"):
         """Get the features logged to this experiment.
 
@@ -176,21 +193,25 @@
             'and'. Defaults to 'or'.
 
         Returns
         -------
         list of rubicon.client.Feature
             The features previously logged to this experiment.
         """
+        return_err = None
+        for repo in self.repositories:
+            try:
+                features = [Feature(f, self) for f in repo.get_features(self.project.name, self.id)]
+            except Exception as err:
+                return_err = err
+            else:
+                self._features = filter_children(features, tags, qtype, name)
+                return self._features
 
-        features = [
-            Feature(f, self) for f in self.repository.get_features(self.project.name, self.id)
-        ]
-
-        self._features = filter_children(features, tags, qtype, name)
-        return self._features
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def feature(self, name=None, id=None):
         """Get a feature.
 
         Parameters
         ----------
@@ -202,22 +223,28 @@
         Returns
         -------
         rubicon.client.Feature
             The feature with name `name` or id `id`.
         """
         if (name is None and id is None) or (name is not None and id is not None):
             raise ValueError("`name` OR `id` required.")
-
         if name is not None:
-            feature = self.repository.get_feature(self.project.name, self.id, name)
-            feature = Feature(feature, self)
+            return_err = None
+            for repo in self.repositories:
+                try:
+                    feature = repo.get_feature(self.project.name, self.id, name)
+                except Exception as err:
+                    return_err = err
+                else:
+                    feature = Feature(feature, self)
+                    return feature
+            raise RubiconException("all configured storage backends failed") from return_err
         else:
             feature = [f for f in self.features() if f.id == id][0]
-
-        return feature
+            return feature
 
     @failsafe
     def log_parameter(self, name, value=None, description=None, tags=[]):
         """Create a parameter under the experiment.
 
         Parameters
         ----------
@@ -239,15 +266,16 @@
         rubicon.client.Parameter
             The created parameter.
         """
         if not isinstance(tags, list) or not all([isinstance(tag, str) for tag in tags]):
             raise ValueError("`tags` must be `list` of type `str`")
 
         parameter = domain.Parameter(name, value=value, description=description, tags=tags)
-        self.repository.create_parameter(parameter, self.project.name, self.id)
+        for repo in self.repositories:
+            repo.create_parameter(parameter, self.project.name, self.id)
 
         return Parameter(parameter, self)
 
     @failsafe
     def parameters(self, name=None, tags=[], qtype="or"):
         """Get the parameters logged to this experiment.
 
@@ -262,22 +290,27 @@
             'and'. Defaults to 'or'.
 
         Returns
         -------
         list of rubicon.client.Parameter
             The parameters previously logged to this experiment.
         """
+        return_err = None
+        for repo in self.repositories:
+            try:
+                parameters = [
+                    Parameter(p, self) for p in repo.get_parameters(self.project.name, self.id)
+                ]
+            except Exception as err:
+                return_err = err
+            else:
+                self._parameters = filter_children(parameters, tags, qtype, name)
+                return self._parameters
 
-        parameters = [
-            Parameter(p, self) for p in self.repository.get_parameters(self.project.name, self.id)
-        ]
-
-        self._parameters = filter_children(parameters, tags, qtype, name)
-
-        return self._parameters
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def parameter(self, name=None, id=None):
         """Get a parameter.
 
         Parameters
         ----------
@@ -291,20 +324,27 @@
         rubicon.client.Parameter
             The parameter with name `name` or id `id`.
         """
         if (name is None and id is None) or (name is not None and id is not None):
             raise ValueError("`name` OR `id` required.")
 
         if name is not None:
-            parameter = self.repository.get_parameter(self.project.name, self.id, name)
-            parameter = Parameter(parameter, self)
+            return_err = None
+            for repo in self.repositories:
+                try:
+                    parameter = repo.get_parameter(self.project.name, self.id, name)
+                except Exception as err:
+                    return_err = err
+                else:
+                    parameter = Parameter(parameter, self)
+                    return parameter
+            raise RubiconException("all configured storage backends failed") from return_err
         else:
             parameter = [p for p in self.parameters() if p.id == id][0]
-
-        return parameter
+            return parameter
 
     @property
     def id(self):
         """Get the experiment's id."""
         return self._domain.id
 
     @property
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/feature.py` & `rubicon-ml-0.4.5/rubicon_ml/client/feature.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/metric.py` & `rubicon-ml-0.4.5/rubicon_ml/client/metric.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/mixin.py` & `rubicon-ml-0.4.5/rubicon_ml/client/mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,17 +118,16 @@
             name=name,
             description=description,
             parent_id=self._domain.id,
             tags=tags,
         )
 
         project_name, experiment_id = self._get_identifiers()
-        self.repository.create_artifact(
-            artifact, data_bytes, project_name, experiment_id=experiment_id
-        )
+        for repo in self.repositories:
+            repo.create_artifact(artifact, data_bytes, project_name, experiment_id=experiment_id)
 
         return client.Artifact(artifact, self)
 
     def _get_environment_bytes(self, export_cmd):
         """Get the working environment as a sequence of bytes.
 
         Parameters
@@ -214,24 +213,28 @@
 
         Returns
         -------
         list of rubicon.client.Artifact
             The artifacts previously logged to this client object.
         """
         project_name, experiment_id = self._get_identifiers()
-        artifacts = [
-            client.Artifact(a, self)
-            for a in self.repository.get_artifacts_metadata(
-                project_name, experiment_id=experiment_id
-            )
-        ]
+        return_err = None
+        for repo in self.repositories:
+            try:
+                artifacts = [
+                    client.Artifact(a, self)
+                    for a in repo.get_artifacts_metadata(project_name, experiment_id=experiment_id)
+                ]
+            except Exception as err:
+                return_err = err
+            else:
+                self._artifacts = filter_children(artifacts, tags, qtype, name)
+                return self._artifacts
 
-        self._artifacts = filter_children(artifacts, tags, qtype, name)
-
-        return self._artifacts
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def artifact(self, name=None, id=None):
         """Get an artifact logged to this project by id or name.
 
         Parameters
         ----------
@@ -255,36 +258,45 @@
                 raise RubiconException(f"No artifact found with name '{name}'.")
             if len(artifacts) > 1:
                 warnings.warn(
                     f"Multiple artifacts found with name '{name}'. Returning most recently logged."
                 )
 
             artifact = artifacts[-1]
+            return artifact
         else:
             project_name, experiment_id = self._get_identifiers()
-            artifact = client.Artifact(
-                self.repository.get_artifact_metadata(project_name, id, experiment_id), self
-            )
+            return_err = None
+            for repo in self.repositories:
+                try:
+                    artifact = client.Artifact(
+                        repo.get_artifact_metadata(project_name, id, experiment_id), self
+                    )
+                except Exception as err:
+                    return_err = err
+                else:
+                    return artifact
 
-        return artifact
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def delete_artifacts(self, ids):
         """Delete the artifacts logged to with client object
         with ids `ids`.
 
         Parameters
         ----------
         ids : list of str
             The ids of the artifacts to delete.
         """
         project_name, experiment_id = self._get_identifiers()
 
         for artifact_id in ids:
-            self.repository.delete_artifact(project_name, artifact_id, experiment_id=experiment_id)
+            for repo in self.repositories:
+                repo.delete_artifact(project_name, artifact_id, experiment_id=experiment_id)
 
 
 class DataframeMixin:
     """Adds dataframe support to a client object."""
 
     @failsafe
     def log_dataframe(self, df, description=None, name=None, tags=[]):
@@ -312,15 +324,16 @@
             parent_id=self._domain.id,
             description=description,
             name=name,
             tags=tags,
         )
 
         project_name, experiment_id = self._get_identifiers()
-        self.repository.create_dataframe(dataframe, df, project_name, experiment_id=experiment_id)
+        for repo in self.repositories:
+            repo.create_dataframe(dataframe, df, project_name, experiment_id=experiment_id)
 
         return client.Dataframe(dataframe, self)
 
     @failsafe
     def dataframes(self, name=None, tags=[], qtype="or"):
         """Get the dataframes logged to this client object.
 
@@ -336,24 +349,28 @@
 
         Returns
         -------
         list of rubicon.client.Dataframe
             The dataframes previously logged to this client object.
         """
         project_name, experiment_id = self._get_identifiers()
-        dataframes = [
-            client.Dataframe(d, self)
-            for d in self.repository.get_dataframes_metadata(
-                project_name, experiment_id=experiment_id
-            )
-        ]
+        return_err = None
+        for repo in self.repositories:
+            try:
+                dataframes = [
+                    client.Dataframe(d, self)
+                    for d in repo.get_dataframes_metadata(project_name, experiment_id=experiment_id)
+                ]
+            except Exception as err:
+                return_err = err
+            else:
+                self._dataframes = filter_children(dataframes, tags, qtype, name)
+                return self._dataframes
 
-        self._dataframes = filter_children(dataframes, tags, qtype, name)
-
-        return self._dataframes
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def dataframe(self, name=None, id=None):
         """
         Get the dataframe logged to this client object.
 
         Parameters
@@ -378,41 +395,48 @@
             elif len(dataframes) > 1:
                 warnings.warn(
                     f"Multiple dataframes found with name '{name}'."
                     " Returning most recently logged."
                 )
 
             dataframe = dataframes[-1]
+            return dataframe
         else:
             project_name, experiment_id = self._get_identifiers()
-            dataframe = client.Dataframe(
-                self.repository.get_dataframe_metadata(
-                    project_name, experiment_id=experiment_id, dataframe_id=id
-                ),
-                self,
-            )
+            return_err = None
+            for repo in self.repositories:
+                try:
+                    dataframe = client.Dataframe(
+                        repo.get_dataframe_metadata(
+                            project_name, experiment_id=experiment_id, dataframe_id=id
+                        ),
+                        self,
+                    )
+                except Exception as err:
+                    return_err = err
+                else:
+                    return dataframe
 
-        return dataframe
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def delete_dataframes(self, ids):
         """Delete the dataframes with ids `ids` logged to
         this client object.
 
         Parameters
         ----------
         ids : list of str
             The ids of the dataframes to delete.
         """
         project_name, experiment_id = self._get_identifiers()
 
         for dataframe_id in ids:
-            self.repository.delete_dataframe(
-                project_name, dataframe_id, experiment_id=experiment_id
-            )
+            for repo in self.repositories:
+                repo.delete_dataframe(project_name, dataframe_id, experiment_id=experiment_id)
 
 
 class TagMixin:
     """Adds tag support to a client object."""
 
     def _get_taggable_identifiers(self):
         project_name, experiment_id = self._parent._get_identifiers()
@@ -441,57 +465,66 @@
         """
         if not isinstance(tags, list) or not all([isinstance(tag, str) for tag in tags]):
             raise ValueError("`tags` must be `list` of type `str`")
 
         project_name, experiment_id, entity_identifier = self._get_taggable_identifiers()
 
         self._domain.add_tags(tags)
-        self.repository.add_tags(
-            project_name,
-            tags,
-            experiment_id=experiment_id,
-            entity_identifier=entity_identifier,
-            entity_type=self.__class__.__name__,
-        )
+        for repo in self.repositories:
+            repo.add_tags(
+                project_name,
+                tags,
+                experiment_id=experiment_id,
+                entity_identifier=entity_identifier,
+                entity_type=self.__class__.__name__,
+            )
 
     @failsafe
     def remove_tags(self, tags):
         """Remove tags from this client object.
 
         Parameters
         ----------
         tags : list of str
              The tag values to remove.
         """
         project_name, experiment_id, entity_identifier = self._get_taggable_identifiers()
 
         self._domain.remove_tags(tags)
-        self.repository.remove_tags(
-            project_name,
-            tags,
-            experiment_id=experiment_id,
-            entity_identifier=entity_identifier,
-            entity_type=self.__class__.__name__,
-        )
+        for repo in self.repositories:
+            repo.remove_tags(
+                project_name,
+                tags,
+                experiment_id=experiment_id,
+                entity_identifier=entity_identifier,
+                entity_type=self.__class__.__name__,
+            )
 
     def _update_tags(self, tag_data):
         """Add or remove the tags in `tag_data` based on
         their key.
         """
         for tag in tag_data:
             self._domain.add_tags(tag.get("added_tags", []))
             self._domain.remove_tags(tag.get("removed_tags", []))
 
     @property
     def tags(self):
         """Get this client object's tags."""
         project_name, experiment_id, entity_identifier = self._get_taggable_identifiers()
-        tag_data = self.repository.get_tags(
-            project_name,
-            experiment_id=experiment_id,
-            entity_identifier=entity_identifier,
-            entity_type=self.__class__.__name__,
-        )
+        return_err = None
+        for repo in self.repositories:
+            try:
+                tag_data = repo.get_tags(
+                    project_name,
+                    experiment_id=experiment_id,
+                    entity_identifier=entity_identifier,
+                    entity_type=self.__class__.__name__,
+                )
+            except Exception as err:
+                return_err = err
+            else:
+                self._update_tags(tag_data)
 
-        self._update_tags(tag_data)
+                return self._domain.tags
 
-        return self._domain.tags
+        raise RubiconException("all configured storage backends failed") from return_err
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/parameter.py` & `rubicon-ml-0.4.5/rubicon_ml/client/parameter.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/project.py` & `rubicon-ml-0.4.5/rubicon_ml/client/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import subprocess
 import warnings
+from typing import List, Optional
 
 import dask.dataframe as dd
 import pandas as pd
 
 from rubicon_ml import domain
 from rubicon_ml.client import ArtifactMixin, Base, DataframeMixin, Experiment
 from rubicon_ml.client.utils.exception_handling import failsafe
@@ -249,15 +250,16 @@
             description,
             model_name,
             branch_name,
             commit_hash,
             training_metadata,
             tags,
         )
-        self.repository.create_experiment(experiment)
+        for repo in self.repositories:
+            repo.create_experiment(experiment)
 
         return Experiment(experiment, self)
 
     @failsafe
     def experiment(self, id=None, name=None):
         """Get an experiment logged to this project by id or name.
 
@@ -284,18 +286,25 @@
             elif len(experiments) > 1:
                 warnings.warn(
                     f"Multiple experiments found with name '{name}'."
                     " Returning most recently logged."
                 )
 
             experiment = experiments[-1]
+            return experiment
         else:
-            experiment = Experiment(self.repository.get_experiment(self.name, id), self)
-
-        return experiment
+            return_err = None
+            for repo in self.repositories:
+                try:
+                    experiment = Experiment(repo.get_experiment(self.name, id), self)
+                except Exception as err:
+                    return_err = err
+                else:
+                    return experiment
+            raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def experiments(self, tags=[], qtype="or", name=None):
         """Get the experiments logged to this project.
 
         Parameters
         ----------
@@ -308,18 +317,25 @@
             The name of the experiment(s) to filter results on.
 
         Returns
         -------
         list of rubicon.client.Experiment
             The experiments previously logged to this project.
         """
-        experiments = [Experiment(e, self) for e in self.repository.get_experiments(self.name)]
-        self._experiments = filter_children(experiments, tags, qtype, name)
+        return_err = None
+        for repo in self.repositories:
+            try:
+                experiments = [Experiment(e, self) for e in repo.get_experiments(self.name)]
+            except Exception as err:
+                return_err = err
+            else:
+                self._experiments = filter_children(experiments, tags, qtype, name)
+                return self._experiments
 
-        return self._experiments
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def dataframes(self, tags=[], qtype="or", recursive=False, name=None):
         """Get the dataframes logged to this project.
 
         Parameters
         ----------
@@ -343,14 +359,70 @@
 
         if recursive is True:
             for experiment in self.experiments():
                 self._dataframes.extend(experiment.dataframes(tags=tags, qtype=qtype, name=name))
 
         return self._dataframes
 
+    @failsafe
+    def archive(self, experiments: Optional[List[Experiment]] = None, remote_rubicon=None):
+        """Archive the experiments logged to this project.
+
+        Parameters
+        ----------
+        experiments : list of Experiments, optional
+            The rubicon.client.Experiment objects to archive. If None all logged experiments are archived.
+        remote_rubicon : rubicon_ml.Rubicon object, optional
+            The remote Rubicon object with the repository to archive to
+
+        Returns
+        -------
+        filepath of newly created archive
+        """
+        if len(self.experiments()) == 0:
+            raise ValueError("`project` has no logged `experiments` to archive")
+        if experiments is not None:
+            if not isinstance(experiments, list) or not all(
+                [isinstance(experiment, Experiment) for experiment in experiments]
+            ):
+                raise ValueError(
+                    "`experiments` must be `list` of type `rubicon_ml.client.Experiment`"
+                )
+
+        if remote_rubicon is not None:
+            from rubicon_ml import Rubicon
+
+            if not isinstance(remote_rubicon, Rubicon):
+                raise ValueError("`remote_rubicon` must be of type `rubicon_ml.client.Rubicon`")
+            else:
+                return self.repository._archive(
+                    self.name, experiments, remote_rubicon.repository.root_dir
+                )
+        else:
+            return self.repository._archive(self.name, experiments, None)
+
+    @failsafe
+    def experiments_from_archive(self, remote_rubicon, latest_only: Optional[bool] = False):
+        """Retrieve archived experiments into this project's experiments folder.
+
+        Parameters
+        ----------
+        remote_rubicon : rubicon_ml.Rubicon object
+            The remote Rubicon object with the repository containing archived experiments to read in
+        latest_only : bool, optional
+            Indicates whether or not experiments should only be read from the latest archive
+        """
+        from rubicon_ml import Rubicon
+
+        if not isinstance(remote_rubicon, Rubicon):
+            raise ValueError("`remote_rubicon` must be of type `rubicon_ml.client.Rubicon`")
+        self.repository._experiments_from_archive(
+            self.name, remote_rubicon.repository.root_dir, latest_only
+        )
+
     @property
     def name(self):
         """Get the project's name."""
         return self._domain.name
 
     @property
     def id(self):
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/rubicon.py` & `rubicon-ml-0.4.5/rubicon_ml/client/rubicon.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,14 +36,21 @@
     ):
         self.config = Config(persistence, root_dir, auto_git_enabled, **storage_options)
 
     @property
     def repository(self):
         return self.config.repository
 
+    @property
+    def repositories(self):
+        if hasattr(self.config, "repositories"):
+            return self.config.repositories
+        else:
+            return [self.config.repository]
+
     @repository.setter
     def repository(self, value):
         self.config.repository = value
 
     def _get_github_url(self):
         """Returns the repository URL of the `git` repo it is called from."""
         completed_process = subprocess.run(["git", "remote", "-v"], capture_output=True)
@@ -92,15 +99,16 @@
 
         Returns
         -------
         rubicon.client.Project
             The created project.
         """
         project = self._create_project_domain(name, description, github_url, training_metadata)
-        self.repository.create_project(project)
+        for repo in self.repositories:
+            repo.create_project(project)
 
         return Project(project, self.config)
 
     @failsafe
     def get_project(self, name=None, id=None):
         """Get a project.
 
@@ -116,20 +124,27 @@
         rubicon.client.Project
             The project with name `name` or id `id`.
         """
         if (name is None and id is None) or (name is not None and id is not None):
             raise ValueError("`name` OR `id` required.")
 
         if name is not None:
-            project = self.repository.get_project(name)
-            project = Project(project, self.config)
+            return_err = None
+            for repo in self.repositories:
+                try:
+                    project = repo.get_project(name)
+                except Exception as err:
+                    return_err = err
+                else:
+                    project = Project(project, self.config)
+                    return project
+            raise RubiconException("all configured storage backends failed") from return_err
         else:
             project = [p for p in self.projects() if p.id == id][0]
-
-        return project
+            return project
 
     def get_project_as_dask_df(self, name, group_by=None):
         """DEPRECATED: Available for backwards compatibility."""
         warnings.warn(
             "`get_project_as_dask_df` is deprecated and will be removed in a future "
             "release. use `get_project_as_df('name', df_type='dask') instead.",
             DeprecationWarning,
@@ -195,15 +210,23 @@
         """Get a list of available projects.
 
         Returns
         -------
         list of rubicon.client.Project
             The list of available projects.
         """
-        return [Project(project, self.config) for project in self.repository.get_projects()]
+        return_err = None
+        for repo in self.repositories:
+            try:
+                projects = [Project(project, self.config) for project in repo.get_projects()]
+            except Exception as err:
+                return_err = err
+            else:
+                return projects
+        raise RubiconException("all configured storage backends failed") from return_err
 
     @failsafe
     def sync(self, project_name, s3_root_dir):
         """Sync a local project to S3.
 
         Parameters
         ----------
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/utils/exception_handling.py` & `rubicon-ml-0.4.5/rubicon_ml/client/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/client/utils/tags.py` & `rubicon-ml-0.4.5/rubicon_ml/client/utils/tags.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/domain/experiment.py` & `rubicon-ml-0.4.5/rubicon_ml/domain/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/domain/metric.py` & `rubicon-ml-0.4.5/rubicon_ml/domain/metric.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/domain/utils/training_metadata.py` & `rubicon-ml-0.4.5/rubicon_ml/domain/utils/training_metadata.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/base.py` & `rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/experiment.py` & `rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/publish.py` & `rubicon-ml-0.4.5/rubicon_ml/intake_rubicon/publish.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         with fsspec.open(output_filepath, "w", auto_mkdir=False) as f:
             f.write(catalog_yaml)
 
     return catalog_yaml
 
 
 def _update_catalog(base_catalog_filepath, new_experiments, output_filepath=None):
-
     """Helper function to update exisiting intake catalog.
 
     Parameters
     ----------
     base_catalog_filepath : str
         the absolute or relative catalog filepath or S3 bucket
         and key to log the generated YAML file to. S3 buckets
@@ -88,15 +87,14 @@
         yaml.safe_dump(curr_catalog, yamlfile)
         updated_catalog = yaml.dump(curr_catalog)
 
     return updated_catalog
 
 
 def _build_catalog(experiments):
-
     """Helper function to build catalog dictionary from given experiments.
 
     Parameters
     ----------
     experiments : list of rubicon_ml.client.experiment.Experiment
         The expriments that are used to build the catalog to eventually publish
     Returns
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/repository/base.py` & `rubicon-ml-0.4.5/rubicon_ml/repository/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import os
+import shutil
+import tempfile
 import warnings
+from datetime import datetime
+from typing import List, Optional
+from zipfile import ZipFile
 
 import fsspec
 import pandas as pd
 
 from rubicon_ml import domain
 from rubicon_ml.exceptions import RubiconException
 from rubicon_ml.repository.utils import json, slugify
@@ -70,17 +75,23 @@
             os.path.join(p.get("name"), "metadata.json")
             for p in self.filesystem.ls(path, detail=True)
             if p.get("type", p.get("StorageClass")).lower() == "directory"
         ]
 
         return directories
 
+    def _ls(self, path):
+        return self.filesystem.ls(path)
+
     def _mkdir(self, dirpath):
         """Creates a directory `dirpath` with parents."""
-        return self.filesystem.mkdir(dirpath, parents=True, exist_ok=True)
+        return self.filesystem.mkdirs(dirpath, exist_ok=True)
+
+    def _modified(self, path):
+        return self.filesystem.modified(path)
 
     def _persist_bytes(self, bytes_data, path):
         """Write bytes to the filesystem.
 
         To be implemented by extensions of the base filesystem.
         """
         raise NotImplementedError()
@@ -259,14 +270,123 @@
             ]
             experiments.sort(key=lambda e: e.created_at)
         except FileNotFoundError:
             return []
 
         return experiments
 
+    # ------- Archiving --------
+
+    def _archive(
+        self,
+        project_name,
+        experiments: Optional[List] = None,
+        remote_rubicon_root: Optional[str] = None,
+    ):
+        """Archive the experiments logged to this project.
+
+        Parameters
+        ----------
+        project_name : str
+            Name of the calling project (project to create archive for)
+        experiments : list of Experiments, optional
+            The rubicon.client.Experiment objects to archive. If None all logged experiments are archived.
+        remote_rubicon_root : str or pathlike object, optional
+            The remote root of the repository to archive to
+
+        Returns
+        -------
+        filepath of newly created archive
+        """
+        remote_s3 = True if remote_rubicon_root and remote_rubicon_root.startswith("s3") else False
+        root_dir = remote_rubicon_root if remote_rubicon_root is not None else self.root_dir
+        archive_dir = os.path.join(root_dir, slugify(project_name), "archives")
+        ts = datetime.timestamp(datetime.now())
+        archive_path = os.path.join(archive_dir, "archive-" + str(ts))
+        zip_archive_filename = str(archive_path + ".zip")
+        experiments_path = self._get_experiment_metadata_root(project_name)
+
+        if not remote_s3:
+            if not self._exists(archive_dir):
+                self._mkdir(archive_dir)
+
+        file_name = None
+        with tempfile.NamedTemporaryFile() as tf:
+            if experiments is not None:
+                with ZipFile(tf, "x") as archive:
+                    experiment_paths = []
+                    for experiment in experiments:
+                        experiment_paths.append(os.path.join(experiments_path, experiment.id))
+                    for file_path in experiment_paths:
+                        archive.write(file_path, os.path.basename(file_path))
+                file_name = archive.filename
+
+            else:
+                file_name = shutil.make_archive(tf.name, "zip", experiments_path)
+
+            with fsspec.open(zip_archive_filename, "wb") as fp:
+                with open(file_name, "rb") as tf:
+                    fp.write(tf.read())
+
+        return zip_archive_filename
+
+    def _experiments_from_archive(
+        self, project_name, remote_rubicon_root: str, latest_only: Optional[bool] = False
+    ):
+        """Retrieve archived experiments into this project's experiments folder.
+
+        Parameters
+        ----------
+        project_name : str
+            Name of the calling project (project to read experiments into)
+        remote_rubicon_root : str or pathlike object
+            The remote Rubicon object with the repository containing archived experiments to read in
+        latest_only : bool, optional
+            Indicates whether or not experiments should only be read from the latest archive
+        """
+        root_dir = self.root_dir
+        shutil.copy(
+            os.path.join(remote_rubicon_root, slugify(project_name), "metadata.json"),
+            os.path.join(root_dir, slugify(project_name)),
+        )
+        archive_dir = os.path.join(remote_rubicon_root, slugify(project_name), "archives")
+        if not self._exists(archive_dir):
+            raise ValueError("`remote_rubicon_root` has no archives")
+
+        dest_experiments_dir = self._get_experiment_metadata_root(project_name)
+        if not self._exists(dest_experiments_dir):
+            self._mkdir(dest_experiments_dir)
+
+        og_num_experiments = len(self._ls(dest_experiments_dir))
+
+        if not latest_only:
+            for zip_archive_name in self._ls(archive_dir):
+                zip_archive_filepath = os.path.join(archive_dir, zip_archive_name)
+                with ZipFile(zip_archive_filepath, "r") as curr_archive:
+                    curr_archive.extractall(dest_experiments_dir)
+        else:
+            latest_zip_archive_filepath = None
+            latest_time = None
+            for zip_archive in self._ls(archive_dir):
+                zip_archive_filepath = os.path.join(archive_dir, zip_archive)
+                mod_time = self._modified(zip_archive_filepath)
+                if latest_time is None:
+                    latest_time = mod_time
+                    latest_zip_archive_filepath = zip_archive_filepath
+                elif mod_time > latest_time:
+                    latest_zip_archive_filepath = zip_archive_filepath
+                    latest_time = mod_time
+            with ZipFile(latest_zip_archive_filepath, "r") as zip_archive:
+                zip_archive.extractall(dest_experiments_dir)
+
+        if len(self._ls(dest_experiments_dir)) > og_num_experiments:
+            print("experiments read from archive")
+        else:
+            print("experiments not read from archive")
+
     # ------- Artifacts --------
 
     def _get_artifact_metadata_root(self, project_name, experiment_id=None):
         """Returns the artifacts directory of the project with name
         `project_name` or experiment with ID `experiment_id`.
         """
         if experiment_id is not None:
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml/repository/local.py` & `rubicon-ml-0.4.5/rubicon_ml/repository/local.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/repository/memory.py` & `rubicon-ml-0.4.5/rubicon_ml/repository/memory.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/repository/s3.py` & `rubicon-ml-0.4.5/rubicon_ml/repository/s3.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/repository/utils/json.py` & `rubicon-ml-0.4.5/rubicon_ml/repository/utils/json.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/sklearn/estimator_logger.py` & `rubicon-ml-0.4.5/rubicon_ml/sklearn/estimator_logger.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/sklearn/filter_estimator_logger.py` & `rubicon-ml-0.4.5/rubicon_ml/sklearn/filter_estimator_logger.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/sklearn/pipeline.py` & `rubicon-ml-0.4.5/rubicon_ml/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/viz/assets/images/rubicon-logo-dark.png` & `rubicon-ml-0.4.5/rubicon_ml/viz/assets/images/rubicon-logo-dark.png`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/viz/base.py` & `rubicon-ml-0.4.5/rubicon_ml/viz/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/viz/common/dropdown_header.py` & `rubicon-ml-0.4.5/rubicon_ml/viz/common/dropdown_header.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/viz/dashboard.py` & `rubicon-ml-0.4.5/rubicon_ml/viz/dashboard.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/viz/dataframe_plot.py` & `rubicon-ml-0.4.5/rubicon_ml/viz/dataframe_plot.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/viz/experiments_table.py` & `rubicon-ml-0.4.5/rubicon_ml/viz/experiments_table.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/viz/metric_correlation_plot.py` & `rubicon-ml-0.4.5/rubicon_ml/viz/metric_correlation_plot.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/viz/metric_lists_comparison.py` & `rubicon-ml-0.4.5/rubicon_ml/viz/metric_lists_comparison.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/__init__.py` & `rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/tasks.py` & `rubicon-ml-0.4.5/rubicon_ml/workflow/prefect/tasks.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/rubicon_ml.egg-info/PKG-INFO` & `rubicon-ml-0.4.5/rubicon_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-ml
-Version: 0.4.4
+Version: 0.4.5
 Summary: "an ML library for model development and governance"
 Home-page: https://github.com/capitalone/rubicon-ml
 Author: "Joe Wolfe, Ryan Soley, Diane Lee, Mike McCarty, CapitalOne"
 License: "Apache License, Version 2.0"
 Project-URL: Documentation, https://capitalone.github.io/rubicon-ml/
 Project-URL: Bug Tracker, https://github.com/capitalone/rubicon-ml/issues
 Project-URL: Source Code, https://github.com/capitalone/rubicon-ml
```

### Comparing `rubicon-ml-0.4.4/rubicon_ml.egg-info/SOURCES.txt` & `rubicon-ml-0.4.5/rubicon_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/setup.cfg` & `rubicon-ml-0.4.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -25,38 +25,38 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	click<=8.1.3,>=7.1
-	fsspec<=2023.4.0,>=2021.4.0
-	intake[dataframe]<=0.6.8,>=0.5.2
-	numpy<=1.24.2,>=1.22.0
-	pandas<=2.0.0,>=1.0.0
-	pyarrow<=11.0.0,>=0.18.0
+	fsspec<=2023.5.0,>=2021.4.0
+	intake[dataframe]<=0.7.0,>=0.5.2
+	numpy<=1.24.3,>=1.22.0
+	pandas<=2.0.2,>=1.0.0
+	pyarrow<=12.0.0,>=0.18.0
 	PyYAML<=6.0,>=5.4.0
 	scikit-learn<=1.2.2,>=0.22.0
 
 [options.extras_require]
 prefect = 
 	prefect<=1.2.4,>=0.12.0
 s3 = 
-	s3fs<=2023.4.0,>=0.4
+	s3fs<=2023.5.0,>=0.4
 ui = 
-	dash<=2.9.3,>=2.0.0
+	dash<=2.10.2,>=2.0.0
 	dash-bootstrap-components<=1.4.1,>=1.0.0
 viz = 
-	dash<=2.9.3,>=2.0.0
+	dash<=2.10.2,>=2.0.0
 	dash-bootstrap-components<=1.4.1,>=1.0.0
 all = 
-	dash<=2.9.3,>=2.0.0
+	dash<=2.10.2,>=2.0.0
 	dash-bootstrap-components<=1.4.1,>=1.0.0
 	prefect<=1.2.4,>=0.12.0
-	s3fs<=2023.4.0,>=0.4
+	s3fs<=2023.5.0,>=0.4
 
 [options.entry_points]
 console_scripts = 
 	rubicon_ml = rubicon_ml.cli:cli
 intake.drivers = 
 	rubicon_ml_experiment = rubicon_ml.intake_rubicon.experiment:ExperimentSource
 
@@ -94,23 +94,22 @@
 addopts = --cov=./rubicon_ml --cov-report=term-missing --cov-fail-under=90 -m="not write_files"
 minversion = 3.2
 xfail_strict = True
 
 [edgetest.envs.core]
 python_version = 3.9
 deps = 
-	kaleido
-	palmerpenguins
-	Pillow
-conda_install = 
 	dask
 	jupyterlab
+	kaleido
 	nodejs
 	nbconvert
 	nbformat
+	palmerpenguins
+	Pillow
 	pytest
 	pytest-cov
 	prefect
 extras = 
 	all
 upgrade = 
 	click
```

### Comparing `rubicon-ml-0.4.4/tests/fixtures.py` & `rubicon-ml-0.4.5/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.4/versioneer.py` & `rubicon-ml-0.4.5/versioneer.py`

 * *Files identical despite different names*

