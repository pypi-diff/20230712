# Comparing `tmp/fedjax-0.0.8.tar.gz` & `tmp/fedjax-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedjax-0.0.8.tar", last modified: Tue Nov  9 03:31:15 2021, max compression
+gzip compressed data, was "fedjax-0.0.9.tar", last modified: Mon Nov 29 17:09:27 2021, max compression
```

## Comparing `fedjax-0.0.8.tar` & `fedjax-0.0.9.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.550492 fedjax-0.0.8/
--rw-r-----   0 wuke     (203014) primarygroup (89939)    11357 2021-11-09 03:22:33.000000 fedjax-0.0.8/LICENSE
--rw-r-----   0 wuke     (203014) primarygroup (89939)     6854 2021-11-09 03:31:15.550492 fedjax-0.0.8/PKG-INFO
--rw-r-----   0 wuke     (203014) primarygroup (89939)     6065 2021-11-09 03:22:33.000000 fedjax-0.0.8/README.md
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.534490 fedjax-0.0.8/docs/
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3210 2021-11-09 03:22:33.000000 fedjax-0.0.8/docs/conf.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.534490 fedjax-0.0.8/examples/
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4403 2021-11-09 03:22:33.000000 fedjax-0.0.8/examples/emnist_fed_avg.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4131 2021-11-09 03:22:33.000000 fedjax-0.0.8/examples/fed_avg.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2281 2021-11-09 03:22:33.000000 fedjax-0.0.8/examples/fed_avg_test.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.534490 fedjax-0.0.8/experiments/
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.538491 fedjax-0.0.8/experiments/fed_avg/
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4053 2021-11-09 03:22:33.000000 fedjax-0.0.8/experiments/fed_avg/run_fed_avg.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.538491 fedjax-0.0.8/fedjax/
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3536 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/__init__.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.538491 fedjax-0.0.8/fedjax/aggregators/
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1054 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/aggregators/__init__.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2676 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/aggregators/aggregator.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1370 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/aggregators/aggregator_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4827 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/aggregators/compression.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3985 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/aggregators/compression_test.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.538491 fedjax-0.0.8/fedjax/algorithms/
--rw-r-----   0 wuke     (203014) primarygroup (89939)      830 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/__init__.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    13310 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/agnostic_fed_avg.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     8794 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/agnostic_fed_avg_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     6264 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/fed_avg.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3119 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/fed_avg_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    19762 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/hyp_cluster.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    16838 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/hyp_cluster_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     8579 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/mime.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     6562 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/mime_lite.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3300 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/mime_lite_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4009 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/algorithms/mime_test.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.542491 fedjax-0.0.8/fedjax/core/
--rw-r-----   0 wuke     (203014) primarygroup (89939)      671 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/__init__.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    29970 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/client_datasets.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3301 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/client_datasets_benchmark.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    24174 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/client_datasets_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4788 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/client_samplers.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3765 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/client_samplers_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1864 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/dataclasses.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4012 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/federated_algorithm.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    18855 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/federated_data.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     9697 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/federated_data_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    20149 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/for_each_client.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    18021 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/for_each_client_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     6833 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/in_memory_federated_data.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3744 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/in_memory_federated_data_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    36464 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/metrics.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    15176 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/metrics_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    21434 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/models.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    15420 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/models_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     9377 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/optimizers.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3335 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/optimizers_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1974 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/regularizers.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1840 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/regularizers_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     6173 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/serialization.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2504 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/serialization_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    12119 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/sqlite_federated_data.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)    12713 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/sqlite_federated_data_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2923 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/tree_util.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1896 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/tree_util_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1343 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/typing.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2438 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/util.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1265 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/core/util_test.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.546491 fedjax-0.0.8/fedjax/datasets/
--rw-r-----   0 wuke     (203014) primarygroup (89939)      791 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/__init__.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     7700 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/cifar100.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3752 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/cifar100_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4570 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/downloads.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3407 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/downloads_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     5062 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/emnist.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2227 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/emnist_test.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.534490 fedjax-0.0.8/fedjax/datasets/scripts/
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.546491 fedjax-0.0.8/fedjax/datasets/scripts/cornell_movie_dialogs/
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4703 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/scripts/cornell_movie_dialogs/data_to_sqlite.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2480 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/scripts/cornell_movie_dialogs/data_to_sqlite_test.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.546491 fedjax-0.0.8/fedjax/datasets/scripts/sent140/
--rw-r-----   0 wuke     (203014) primarygroup (89939)     5551 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/scripts/sent140/data_to_sqlite.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1823 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/scripts/sent140/data_to_sqlite_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     6976 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/shakespeare.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1445 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/shakespeare_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     8378 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/stackoverflow.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3644 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/datasets/stackoverflow_test.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.546491 fedjax-0.0.8/fedjax/experimental/
--rw-r-----   0 wuke     (203014) primarygroup (89939)      753 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/experimental/__init__.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1219 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/fedjax_test.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.546491 fedjax-0.0.8/fedjax/models/
--rw-r-----   0 wuke     (203014) primarygroup (89939)      785 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/models/__init__.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     5674 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/models/emnist.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2447 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/models/emnist_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4243 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/models/shakespeare.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1756 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/models/shakespeare_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     5453 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/models/stackoverflow.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2693 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/models/stackoverflow_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1508 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/models/toy_regression.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1581 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/models/toy_regression_test.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.550492 fedjax-0.0.8/fedjax/training/
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1485 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/__init__.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2201 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/checkpoint.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2696 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/checkpoint_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     9830 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/federated_experiment.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     8690 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/federated_experiment_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2342 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/logging.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1360 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/logging_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     7981 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/structured_flags.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     4379 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/structured_flags_test.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)     2839 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/training/tasks.py
--rw-r-----   0 wuke     (203014) primarygroup (89939)      620 2021-11-09 03:22:33.000000 fedjax-0.0.8/fedjax/version.py
-drwxr-x---   0 wuke     (203014) primarygroup (89939)        0 2021-11-09 03:31:15.538491 fedjax-0.0.8/fedjax.egg-info/
--rw-r-----   0 wuke     (203014) primarygroup (89939)     6854 2021-11-09 03:31:14.000000 fedjax-0.0.8/fedjax.egg-info/PKG-INFO
--rw-r-----   0 wuke     (203014) primarygroup (89939)     3092 2021-11-09 03:31:14.000000 fedjax-0.0.8/fedjax.egg-info/SOURCES.txt
--rw-r-----   0 wuke     (203014) primarygroup (89939)        1 2021-11-09 03:31:14.000000 fedjax-0.0.8/fedjax.egg-info/dependency_links.txt
--rw-r-----   0 wuke     (203014) primarygroup (89939)       51 2021-11-09 03:31:14.000000 fedjax-0.0.8/fedjax.egg-info/requires.txt
--rw-r-----   0 wuke     (203014) primarygroup (89939)       33 2021-11-09 03:31:14.000000 fedjax-0.0.8/fedjax.egg-info/top_level.txt
--rw-r-----   0 wuke     (203014) primarygroup (89939)       38 2021-11-09 03:31:15.550492 fedjax-0.0.8/setup.cfg
--rw-r-----   0 wuke     (203014) primarygroup (89939)     1864 2021-11-09 03:22:33.000000 fedjax-0.0.8/setup.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.411511 fedjax-0.0.9/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    11357 2021-11-29 17:09:03.000000 fedjax-0.0.9/LICENSE
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     6965 2021-11-29 17:09:27.411511 fedjax-0.0.9/PKG-INFO
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     6176 2021-11-29 17:09:03.000000 fedjax-0.0.9/README.md
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.399510 fedjax-0.0.9/docs/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3210 2021-11-29 17:09:03.000000 fedjax-0.0.9/docs/conf.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.399510 fedjax-0.0.9/examples/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4403 2021-11-29 17:09:03.000000 fedjax-0.0.9/examples/emnist_fed_avg.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4131 2021-11-29 17:09:03.000000 fedjax-0.0.9/examples/fed_avg.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2281 2021-11-29 17:09:03.000000 fedjax-0.0.9/examples/fed_avg_test.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.395510 fedjax-0.0.9/experiments/
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.399510 fedjax-0.0.9/experiments/fed_avg/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4053 2021-11-29 17:09:03.000000 fedjax-0.0.9/experiments/fed_avg/run_fed_avg.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.399510 fedjax-0.0.9/fedjax/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3596 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/__init__.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.399510 fedjax-0.0.9/fedjax/aggregators/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1054 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/aggregators/__init__.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2665 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/aggregators/aggregator.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1370 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/aggregators/aggregator_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4827 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/aggregators/compression.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3985 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/aggregators/compression_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3766 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/aggregators/walsh_hadamard.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1672 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/aggregators/walsh_hadamard_test.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.403510 fedjax-0.0.9/fedjax/algorithms/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)      830 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/__init__.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    13310 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/agnostic_fed_avg.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     8794 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/agnostic_fed_avg_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     6264 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/fed_avg.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3119 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/fed_avg_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    19869 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/hyp_cluster.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    17515 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/hyp_cluster_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     8579 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/mime.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     7186 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/mime_lite.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4470 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/mime_lite_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4009 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/algorithms/mime_test.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.407511 fedjax-0.0.9/fedjax/core/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)      671 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/__init__.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    29970 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/client_datasets.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3301 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/client_datasets_benchmark.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    24174 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/client_datasets_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4788 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/client_samplers.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3765 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/client_samplers_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1864 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/dataclasses.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4012 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/federated_algorithm.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    18855 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/federated_data.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     9697 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/federated_data_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    20149 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/for_each_client.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    18021 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/for_each_client_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     6833 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/in_memory_federated_data.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3744 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/in_memory_federated_data_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    36466 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/metrics.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    15176 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/metrics_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    21434 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/models.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    15420 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/models_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     9377 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/optimizers.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3335 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/optimizers_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1974 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/regularizers.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1840 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/regularizers_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     6173 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/serialization.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2504 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/serialization_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    12122 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/sqlite_federated_data.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)    12713 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/sqlite_federated_data_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3444 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/tree_util.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2359 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/tree_util_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1343 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/typing.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2438 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/util.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1265 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/core/util_test.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.407511 fedjax-0.0.9/fedjax/datasets/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)      791 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/__init__.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     7700 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/cifar100.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3752 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/cifar100_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4570 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/downloads.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3407 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/downloads_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     5062 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/emnist.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2227 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/emnist_test.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.399510 fedjax-0.0.9/fedjax/datasets/scripts/
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.407511 fedjax-0.0.9/fedjax/datasets/scripts/cornell_movie_dialogs/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4703 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/scripts/cornell_movie_dialogs/data_to_sqlite.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2480 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/scripts/cornell_movie_dialogs/data_to_sqlite_test.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.407511 fedjax-0.0.9/fedjax/datasets/scripts/sent140/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     5551 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/scripts/sent140/data_to_sqlite.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1823 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/scripts/sent140/data_to_sqlite_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     6976 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/shakespeare.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1445 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/shakespeare_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     8376 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/stackoverflow.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3644 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/datasets/stackoverflow_test.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.407511 fedjax-0.0.9/fedjax/experimental/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)      753 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/experimental/__init__.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1219 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/fedjax_test.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.411511 fedjax-0.0.9/fedjax/models/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)      785 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/models/__init__.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     5674 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/models/emnist.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2447 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/models/emnist_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4243 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/models/shakespeare.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1756 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/models/shakespeare_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     5453 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/models/stackoverflow.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2693 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/models/stackoverflow_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1508 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/models/toy_regression.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1581 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/models/toy_regression_test.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.411511 fedjax-0.0.9/fedjax/training/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1485 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/__init__.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2201 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/checkpoint.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2696 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/checkpoint_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     9830 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/federated_experiment.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     8690 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/federated_experiment_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2342 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/logging.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1360 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/logging_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     7981 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/structured_flags.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     4379 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/structured_flags_test.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     2839 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/training/tasks.py
+-rw-r-----   0 jaero    (603126) primarygroup (89939)      620 2021-11-29 17:09:03.000000 fedjax-0.0.9/fedjax/version.py
+drwxr-x---   0 jaero    (603126) primarygroup (89939)        0 2021-11-29 17:09:27.399510 fedjax-0.0.9/fedjax.egg-info/
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     6965 2021-11-29 17:09:27.000000 fedjax-0.0.9/fedjax.egg-info/PKG-INFO
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     3171 2021-11-29 17:09:27.000000 fedjax-0.0.9/fedjax.egg-info/SOURCES.txt
+-rw-r-----   0 jaero    (603126) primarygroup (89939)        1 2021-11-29 17:09:27.000000 fedjax-0.0.9/fedjax.egg-info/dependency_links.txt
+-rw-r-----   0 jaero    (603126) primarygroup (89939)       57 2021-11-29 17:09:27.000000 fedjax-0.0.9/fedjax.egg-info/requires.txt
+-rw-r-----   0 jaero    (603126) primarygroup (89939)       33 2021-11-29 17:09:27.000000 fedjax-0.0.9/fedjax.egg-info/top_level.txt
+-rw-r-----   0 jaero    (603126) primarygroup (89939)       38 2021-11-29 17:09:27.411511 fedjax-0.0.9/setup.cfg
+-rw-r-----   0 jaero    (603126) primarygroup (89939)     1881 2021-11-29 17:09:03.000000 fedjax-0.0.9/setup.py
```

### Comparing `fedjax-0.0.8/LICENSE` & `fedjax-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/PKG-INFO` & `fedjax-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedjax
-Version: 0.0.8
+Version: 0.0.9
 Summary: Federated learning simulation with JAX.
 Home-page: https://github.com/google/fedjax
 Author: FedJAX Team
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: federated python machine learning
 Platform: UNKNOWN
@@ -120,32 +120,35 @@
     jnp.sum(client_weights))
   # Server learning rate of 0.01.
   server_params = server_params - server_update * 0.01
 ```
 
 ## Installation
 
-You will need Python 3.6 or later and a working JAX installation. For a CPU-only
-version:
+You will need a moderately recent version of Python. Please check
+[the PyPI page](https://pypi.org/project/fedjax/) for the up to date version
+requirement.
+
+First, install JAX. For a CPU-only version:
 
 ```
 pip install --upgrade pip
 pip install --upgrade jax jaxlib  # CPU-only version
 ```
 
 For other devices (e.g. GPU), follow
 [these instructions](https://github.com/google/jax#installation).
 
-Then, install fedjax from PyPi:
+Then, install FedJAX from PyPI:
 
 ```
 pip install fedjax
 ```
 
-Or, to upgrade to the latest version of fedjax:
+Or, to upgrade to the latest version of FedJAX:
 
 ```
 pip install --upgrade git+https://github.com/google/fedjax.git
 ```
 
 ## Citing FedJAX
```

### Comparing `fedjax-0.0.8/README.md` & `fedjax-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,32 +98,35 @@
     jnp.sum(client_weights))
   # Server learning rate of 0.01.
   server_params = server_params - server_update * 0.01
 ```
 
 ## Installation
 
-You will need Python 3.6 or later and a working JAX installation. For a CPU-only
-version:
+You will need a moderately recent version of Python. Please check
+[the PyPI page](https://pypi.org/project/fedjax/) for the up to date version
+requirement.
+
+First, install JAX. For a CPU-only version:
 
 ```
 pip install --upgrade pip
 pip install --upgrade jax jaxlib  # CPU-only version
 ```
 
 For other devices (e.g. GPU), follow
 [these instructions](https://github.com/google/jax#installation).
 
-Then, install fedjax from PyPi:
+Then, install FedJAX from PyPI:
 
 ```
 pip install fedjax
 ```
 
-Or, to upgrade to the latest version of fedjax:
+Or, to upgrade to the latest version of FedJAX:
 
 ```
 pip install --upgrade git+https://github.com/google/fedjax.git
 ```
 
 ## Citing FedJAX
```

### Comparing `fedjax-0.0.8/docs/conf.py` & `fedjax-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/examples/emnist_fed_avg.py` & `fedjax-0.0.9/examples/emnist_fed_avg.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/examples/fed_avg.py` & `fedjax-0.0.9/examples/fed_avg.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/examples/fed_avg_test.py` & `fedjax-0.0.9/examples/fed_avg_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/experiments/fed_avg/run_fed_avg.py` & `fedjax-0.0.9/experiments/fed_avg/run_fed_avg.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/__init__.py` & `fedjax-0.0.9/fedjax/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 from fedjax.core.federated_data import ClientPreprocessor
 from fedjax.core.federated_data import FederatedData
 from fedjax.core.federated_data import padded_batch_federated_data
 from fedjax.core.federated_data import RepeatableIterator
 from fedjax.core.federated_data import shuffle_repeat_batch_federated_data
 from fedjax.core.federated_data import SubsetFederatedData
+from fedjax.core.federated_data import FederatedDataBuilder
 
 from fedjax.core.for_each_client import for_each_client
 from fedjax.core.for_each_client import for_each_client_backend
 from fedjax.core.for_each_client import get_for_each_client_backend
 from fedjax.core.for_each_client import set_for_each_client_backend
 from fedjax.core.for_each_client import ForEachClientBackend
```

### Comparing `fedjax-0.0.8/fedjax/aggregators/__init__.py` & `fedjax-0.0.9/fedjax/aggregators/__init__.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/aggregators/aggregator.py` & `fedjax-0.0.9/fedjax/aggregators/aggregator.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,23 @@
   This interface defines aggregator algorithms that are used at each round.
   Aggregator state contains any round specific parameters (e.g. number of bits)
   that will be passed from round to round. This state is initialized by
   `init` and passed as input into and returned as output from `aggregate`.
   We strongly recommend using fedjax.dataclass to define state as this provides
   immutability, type hinting, and works by default with JAX transformations.
 
-  The expected usage of Aggregator is as follows:
-  ```
+  The expected usage of Aggregator is as follows::
+
    aggregator = mean_aggregator()
    state = aggregator.init()
    for i in range(num_rounds):
      clients_params_and_weights = compute_client_outputs(i)
      aggregated_params, state = aggregator.apply(clients_params_and_weights,
                                                  state)
 
-  ```
-
   Attributes:
     init: Returns initial state of aggregator.
     apply: Returns the new aggregator state and aggregated params.
   """
   init: Callable[[], AggregatorState]
   apply: Callable[
       [Iterable[Tuple[ClientId, Params, float]], AggregatorState],
```

### Comparing `fedjax-0.0.8/fedjax/aggregators/aggregator_test.py` & `fedjax-0.0.9/fedjax/aggregators/aggregator_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/aggregators/compression.py` & `fedjax-0.0.9/fedjax/aggregators/compression.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/aggregators/compression_test.py` & `fedjax-0.0.9/fedjax/aggregators/compression_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/algorithms/__init__.py` & `fedjax-0.0.9/fedjax/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/algorithms/agnostic_fed_avg.py` & `fedjax-0.0.9/fedjax/algorithms/agnostic_fed_avg.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/algorithms/agnostic_fed_avg_test.py` & `fedjax-0.0.9/fedjax/algorithms/agnostic_fed_avg_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/algorithms/fed_avg.py` & `fedjax-0.0.9/fedjax/algorithms/fed_avg.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/algorithms/fed_avg_test.py` & `fedjax-0.0.9/fedjax/algorithms/fed_avg_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/algorithms/hyp_cluster.py` & `fedjax-0.0.9/fedjax/algorithms/hyp_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,38 +431,39 @@
   """Evaluates cluster params on a Model."""
 
   def __init__(self,
                model: models.Model,
                regularizer: Optional[Callable[[Params], jnp.ndarray]] = None):
     """Initializes some reusable components.
 
-    Because we need to make 2 passes over each client during evaluation, the
-    number of clients that can be evaluated at once is limited. Therefore
+    Because we need to make multiple passes over each client during evaluation,
+    the number of clients that can be evaluated at once is limited. Therefore
     multiple calls to :meth:`~HypClusterEvaluator.evaluate_clients` are needed
     to evaluate a large federated dataset. We factor out some reusable
     components so that the same computation can be jit compiled.
 
     Args:
       model: Model being evaluated.
       regularizer: Optional regularizer.
     """
     self._maximization_step_evaluator = models.AverageLossEvaluator(
         models.model_per_example_loss(model), regularizer)
     self._model_evaluator = models.ModelEvaluator(model)
 
   def evaluate_clients(
       self, cluster_params: List[Params],
-      clients: Sequence[Tuple[federated_data.ClientId,
-                              client_datasets.ClientDataset, PRNGKey]],
+      train_clients: Sequence[Tuple[federated_data.ClientId,
+                                    client_datasets.ClientDataset, PRNGKey]],
+      test_clients: Sequence[Tuple[federated_data.ClientId,
+                                   client_datasets.ClientDataset]],
       batch_hparams: client_datasets.PaddedBatchHParams
   ) -> Iterator[Tuple[federated_data.ClientId, Dict[str, jnp.ndarray]]]:
     """Evaluates each client on the cluster with best average loss."""
-    maximization_clients = clients
     cluster_client_ids = maximization_step(
         evaluator=self._maximization_step_evaluator,
         cluster_params=cluster_params,
-        clients=maximization_clients,
+        clients=train_clients,
         batch_hparams=batch_hparams)
     eval_clients = [(client_id, dataset.padded_batch(batch_hparams),
                      cluster_params[cluster_client_ids[client_id]])
-                    for client_id, dataset, _ in clients]
+                    for client_id, dataset in test_clients]
     yield from self._model_evaluator.evaluate_per_client_params(eval_clients)
```

### Comparing `fedjax-0.0.8/fedjax/algorithms/hyp_cluster_test.py` & `fedjax-0.0.9/fedjax/algorithms/hyp_cluster_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,34 +308,54 @@
             init=None,
             apply_for_eval=apply_for_eval,
             apply_for_train=apply_for_train,
             train_loss=train_loss,
             eval_metrics={'accuracy': metrics.Accuracy()}), regularizer)
 
     cluster_params = [jnp.array(1.), jnp.array(-1.)]
-    clients = [
+    train_clients = [
+        # Evaluated using cluster 0.
+        (b'0',
+         client_datasets.ClientDataset({
+             'x': np.array([3., 2., 1.]),
+             'y': np.array([1, 1, 0])
+         }), jax.random.PRNGKey(0)),
+        # Evaluated using cluster 1.
+        (b'1',
+         client_datasets.ClientDataset({
+             'x': np.array([0.9, -0.9, 0.8, -0.8, -0.3]),
+             'y': np.array([0, 1, 0, 1, 0])
+         }), jax.random.PRNGKey(1)),
+    ]
+    # Test clients are generated from train_clients by swapping client ids and
+    # then flipping labels.
+    test_clients = [
         # Evaluated using cluster 0.
         (b'0',
          client_datasets.ClientDataset({
              'x': np.array([0.9, -0.9, 0.8, -0.8, -0.3]),
              'y': np.array([1, 0, 1, 0, 1])
-         }), jax.random.PRNGKey(0)),
+         })),
         # Evaluated using cluster 1.
         (b'1',
          client_datasets.ClientDataset({
              'x': np.array([3., 2., 1.]),
              'y': np.array([0, 0, 1])
-         }), jax.random.PRNGKey(1)),
+         })),
     ]
     for batch_size in [1, 2, 4]:
       with self.subTest(f'batch_size = {batch_size}'):
         batch_hparams = client_datasets.PaddedBatchHParams(
             batch_size=batch_size)
         metric_values = dict(
-            evaluator.evaluate_clients(cluster_params, clients, batch_hparams))
+            evaluator.evaluate_clients(
+                cluster_params=cluster_params,
+                train_clients=train_clients,
+                test_clients=test_clients,
+                batch_hparams=batch_hparams))
         self.assertCountEqual(metric_values, [b'0', b'1'])
         self.assertCountEqual(metric_values[b'0'], ['accuracy'])
         npt.assert_allclose(metric_values[b'0']['accuracy'], 4 / 5)
         self.assertCountEqual(metric_values[b'1'], ['accuracy'])
         npt.assert_allclose(metric_values[b'1']['accuracy'], 2 / 3)
     self.assertCountEqual(
         functions_called,
```

### Comparing `fedjax-0.0.8/fedjax/algorithms/mime.py` & `fedjax-0.0.9/fedjax/algorithms/mime.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/algorithms/mime_lite.py` & `fedjax-0.0.9/fedjax/algorithms/mime_lite.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,28 +78,31 @@
 
 def mime_lite(
     per_example_loss: Callable[[Params, BatchExample, PRNGKey], jnp.ndarray],
     base_optimizer: optimizers.Optimizer,
     client_batch_hparams: client_datasets.ShuffleRepeatBatchHParams,
     grads_batch_hparams: client_datasets.PaddedBatchHParams,
     server_learning_rate: float,
-    regularizer: Optional[Callable[[Params], jnp.ndarray]] = None
+    regularizer: Optional[Callable[[Params], jnp.ndarray]] = None,
+    client_delta_clip_norm: Optional[float] = None,
 ) -> federated_algorithm.FederatedAlgorithm:
   """Builds mime lite.
 
   Args:
     per_example_loss: A function from (params, batch_example, rng) to a vector
       of loss values for each example in the batch. This is used in both the
       server gradient computation and gradient descent training.
     base_optimizer: Base optimizer to mimic.
     client_batch_hparams: Hyperparameters for batching client dataset for train.
     grads_batch_hparams: Hyperparameters for batching client dataset for server
       gradient computation.
     server_learning_rate: Server learning rate.
     regularizer: Optional regularizer that only depends on params.
+    client_delta_clip_norm: Maximum allowed global norm per client update.
+      Defaults to no clipping.
 
   Returns:
     FederatedAlgorithm
   """
   grad_fn = models.grad(per_example_loss, regularizer)
   grads_for_each_client = mime.create_grads_for_each_client(grad_fn)
   train_for_each_client = create_train_for_each_client(grad_fn, base_optimizer)
@@ -124,20 +127,28 @@
     }
     # Running weighted mean of client updates.
     delta_params_sum = tree_util.tree_zeros_like(server_state.params)
     num_examples_sum = 0.
     for client_id, delta_params in train_for_each_client(
         shared_input, batch_clients):
       num_examples = client_num_examples[client_id]
-      delta_params_sum = tree_util.tree_add(
-          delta_params_sum, tree_util.tree_weight(delta_params, num_examples))
-      num_examples_sum += num_examples
       client_diagnostics[client_id] = {
           'delta_l2_norm': tree_util.tree_l2_norm(delta_params)
       }
+      if client_delta_clip_norm is not None:
+        delta_params = tree_util.tree_clip_by_global_norm(
+            delta_params, client_delta_clip_norm)
+        client_diagnostics[client_id]['clipped_delta_l2_norm'] = (
+            tree_util.tree_l2_norm(delta_params))
+        client_diagnostics[client_id]['clipped'] = jnp.not_equal(
+            client_diagnostics[client_id]['delta_l2_norm'],
+            client_diagnostics[client_id]['clipped_delta_l2_norm'])
+      delta_params_sum = tree_util.tree_add(
+          delta_params_sum, tree_util.tree_weight(delta_params, num_examples))
+      num_examples_sum += num_examples
     mean_delta_params = tree_util.tree_inverse_weight(delta_params_sum,
                                                       num_examples_sum)
 
     # Compute full-batch gradient at server params on train data.
     grads_batch_clients = [(cid, cds.padded_batch(grads_batch_hparams), crng)
                            for cid, cds, crng in clients]
     grads_sum_total, num_sum_total = tree_util.tree_sum(
```

### Comparing `fedjax-0.0.8/fedjax/algorithms/mime_lite_test.py` & `fedjax-0.0.9/fedjax/algorithms/mime_lite_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -85,10 +85,39 @@
         'params': server_params,
         'opt_state': server_opt_state,
     }
     client_outputs = dict(train_for_each_client(shared_input, batch_clients))
     npt.assert_allclose(client_outputs[b'cid0']['w'], 0.7)
     npt.assert_allclose(client_outputs[b'cid1']['w'], 0.45000002)
 
+  def test_client_delta_clip_norm(self):
+    base_optimizer = optimizers.sgd(learning_rate=1.0)
+    train_batch_hparams = client_datasets.ShuffleRepeatBatchHParams(
+        batch_size=2, num_epochs=1, seed=0)
+    grad_batch_hparams = client_datasets.PaddedBatchHParams(batch_size=2)
+    server_learning_rate = 0.2
+    algorithm = mime_lite.mime_lite(
+        per_example_loss,
+        base_optimizer,
+        train_batch_hparams,
+        grad_batch_hparams,
+        server_learning_rate,
+        client_delta_clip_norm=0.5)
+
+    clients = [
+        (b'cid0',
+         client_datasets.ClientDataset({'x': jnp.array([0.2, 0.4, 0.6])}),
+         jax.random.PRNGKey(0)),
+        (b'cid1', client_datasets.ClientDataset({'x': jnp.array([0.8, 0.1])}),
+         jax.random.PRNGKey(1)),
+    ]
+    state = algorithm.init({'w': jnp.array(4.)})
+    state, client_diagnostics = algorithm.apply(state, clients)
+    npt.assert_allclose(state.params['w'], 3.904)
+    npt.assert_allclose(client_diagnostics[b'cid0']['clipped_delta_l2_norm'],
+                        0.5)
+    npt.assert_allclose(client_diagnostics[b'cid1']['clipped_delta_l2_norm'],
+                        0.45000005)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fedjax-0.0.8/fedjax/algorithms/mime_test.py` & `fedjax-0.0.9/fedjax/algorithms/mime_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/__init__.py` & `fedjax-0.0.9/fedjax/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/client_datasets.py` & `fedjax-0.0.9/fedjax/core/client_datasets.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/client_datasets_benchmark.py` & `fedjax-0.0.9/fedjax/core/client_datasets_benchmark.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/client_datasets_test.py` & `fedjax-0.0.9/fedjax/core/client_datasets_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/client_samplers.py` & `fedjax-0.0.9/fedjax/core/client_samplers.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/client_samplers_test.py` & `fedjax-0.0.9/fedjax/core/client_samplers_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/dataclasses.py` & `fedjax-0.0.9/fedjax/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/federated_algorithm.py` & `fedjax-0.0.9/fedjax/core/federated_algorithm.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/federated_data.py` & `fedjax-0.0.9/fedjax/core/federated_data.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/federated_data_test.py` & `fedjax-0.0.9/fedjax/core/federated_data_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/for_each_client.py` & `fedjax-0.0.9/fedjax/core/for_each_client.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/for_each_client_test.py` & `fedjax-0.0.9/fedjax/core/for_each_client_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/in_memory_federated_data.py` & `fedjax-0.0.9/fedjax/core/in_memory_federated_data.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/in_memory_federated_data_test.py` & `fedjax-0.0.9/fedjax/core/in_memory_federated_data_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/metrics.py` & `fedjax-0.0.9/fedjax/core/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -956,15 +956,16 @@
   known. The model's predictions are represented through the columns, and the
   known data values through the rows. This allows one to view in which areas the
   model is doing well, as well as where there is room for improvement. For each
   row in the confusion matrix, if there are a lot of numbers outside of the main
   diagonal, the model is not doing so well in respect to when it is supposed to
   output that row's relative output class.
 
-  Theoretical Example:
+  Theoretical Example::
+
                 Predicted P     Predicted N
 
     Actual P       TP               FN
 
     Actual N       FP               TN
 
     **This is for a binary classification model but the same concept applies
@@ -974,18 +975,18 @@
   Example::
 
     example = {'y': jnp.array(2)}
     prediction = jnp.array([0., 1., 0.])
     metric = ConfusionMatrix(num_classes=3)
     print(metric.evaluate_example(example, prediction))
     # SumStat(accum=DeviceArray([[0., 0., 0.],
-                                 [0., 0., 0.],
-                                 [0., 1., 0.]], dtype=float32)) => [[0. 0. 0.]
-                                                                    [0. 0. 0.]
-                                                                    [0. 1. 0.]]
+    #                            [0., 0., 0.],
+    #                            [0., 1., 0.]], dtype=float32)) => [[0. 0. 0.]
+    #                                                               [0. 0. 0.]
+    #                                                               [0. 1. 0.]]
 
   Attributes:
     target_key: Key name in ``example`` for target.
     pred_key: Key name in ``prediction`` for unnormalized model output pred.
     num_classes: Number of output classes of the model. Used to generate a
       matrix of shape [num_classes, num_classes].
   """
```

### Comparing `fedjax-0.0.8/fedjax/core/metrics_test.py` & `fedjax-0.0.9/fedjax/core/metrics_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/models.py` & `fedjax-0.0.9/fedjax/core/models.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/models_test.py` & `fedjax-0.0.9/fedjax/core/models_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/optimizers.py` & `fedjax-0.0.9/fedjax/core/optimizers.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/optimizers_test.py` & `fedjax-0.0.9/fedjax/core/optimizers_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/regularizers.py` & `fedjax-0.0.9/fedjax/core/regularizers.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/regularizers_test.py` & `fedjax-0.0.9/fedjax/core/regularizers_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/serialization.py` & `fedjax-0.0.9/fedjax/core/serialization.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/serialization_test.py` & `fedjax-0.0.9/fedjax/core/serialization_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/sqlite_federated_data.py` & `fedjax-0.0.9/fedjax/core/sqlite_federated_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,23 +28,24 @@
   return serialization.msgpack_deserialize(data)
 
 
 class SQLiteFederatedData(federated_data.FederatedData):
   """Federated dataset backed by SQLite.
 
   The SQLite database should contain a table named "federated_data" created with
-  the following command:
-  ```
-  CREATE TABLE federated_data (
-    client_id BLOB NOT NULL PRIMARY KEY,
-    data BLOB NOT NULL,
-    num_examples INTEGER NOT NULL
-  );
-  ```
+  the following command::
+
+    CREATE TABLE federated_data (
+      client_id BLOB NOT NULL PRIMARY KEY,
+      data BLOB NOT NULL,
+      num_examples INTEGER NOT NULL
+    );
+
   where,
+
   - `client_id` is the bytes client id.
   - `data` is the serialized client dataset examples.
   - `num_examples` is the number of examples in the client dataset.
 
   By default we use zlib compressed msgpack blobs for `data` (see
   decompress_and_deserialize()).
   """
@@ -286,14 +287,15 @@
       split_name TEXT NOT NULL,
       num_examples INTEGER NOT NULL);
 
     CREATE INDEX idx_metadata_client_id
       ON client_metadata (client_id);
 
   where,
+
   - `split_name` is the split name (e.g. "train" or "test").
   - `client_id` is the client id.
   - `serialized_example_proto` is a single serialized `tf.train.Example`
   protocol buffer message.
   - `num_examples` is the number of examples in the client dataset.
   """
```

### Comparing `fedjax-0.0.8/fedjax/core/sqlite_federated_data_test.py` & `fedjax-0.0.9/fedjax/core/sqlite_federated_data_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/tree_util.py` & `fedjax-0.0.9/fedjax/core/tree_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,7 +89,26 @@
 
 
 @jax.jit
 def tree_l2_norm(pytree: PyTree) -> float:
   """Returns l2 norm of tree."""
   return jnp.sqrt(
       sum(jnp.vdot(x, x) for x in jax.tree_util.tree_leaves(pytree)))
+
+
+@jax.jit
+def tree_clip_by_global_norm(pytree: PyTree, max_norm: float) -> PyTree:
+  """Clips a pytree of arrays using their global norm.
+
+  References:
+    [Pascanu et al, 2012](https://arxiv.org/abs/1211.5063)
+
+  Args:
+    pytree: A pytree to be potentially clipped.
+    max_norm: The maximum global norm for a pytree.
+
+  Returns:
+    A potentially clipped pytree.
+  """
+  global_norm = tree_l2_norm(pytree)
+  scale = jnp.minimum(1, max_norm / global_norm)
+  return jax.tree_util.tree_map(lambda t: scale * t, pytree)
```

### Comparing `fedjax-0.0.8/fedjax/core/tree_util_test.py` & `fedjax-0.0.9/fedjax/core/tree_util_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,10 +50,21 @@
     pytrees = [(0, 1), (2, 3), (4, 5)]
     weights = [6., 7., 8.]
     pytrees_and_weights = zip(pytrees, weights)
     pytree = tree_util.tree_mean(pytrees_and_weights)
     npt.assert_array_almost_equal(pytree,
                                   (2.1904761904761907, 3.1904761904761907))
 
+  def test_tree_clip_by_global_norm(self):
+    pytree = {
+        'x': jnp.array([[[4, 5]], [[1, 1]]]),
+        'y': jnp.array([[3], [1]]),
+    }
+    max_norm = 3.640055  # 0.5 * tree_l2_norm(pytree)
+    clipped_pytree = tree_util.tree_clip_by_global_norm(pytree, max_norm)
+    npt.assert_array_almost_equal(clipped_pytree['x'],
+                                  [[[2, 2.5]], [[0.5, 0.5]]])
+    npt.assert_array_almost_equal(clipped_pytree['y'], [[1.5], [0.5]])
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fedjax-0.0.8/fedjax/core/typing.py` & `fedjax-0.0.9/fedjax/core/typing.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/util.py` & `fedjax-0.0.9/fedjax/core/util.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/core/util_test.py` & `fedjax-0.0.9/fedjax/core/util_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/__init__.py` & `fedjax-0.0.9/fedjax/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/cifar100.py` & `fedjax-0.0.9/fedjax/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/cifar100_test.py` & `fedjax-0.0.9/fedjax/datasets/cifar100_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/downloads.py` & `fedjax-0.0.9/fedjax/datasets/downloads.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/downloads_test.py` & `fedjax-0.0.9/fedjax/datasets/downloads_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/emnist.py` & `fedjax-0.0.9/fedjax/datasets/emnist.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/emnist_test.py` & `fedjax-0.0.9/fedjax/datasets/emnist_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/scripts/cornell_movie_dialogs/data_to_sqlite.py` & `fedjax-0.0.9/fedjax/datasets/scripts/cornell_movie_dialogs/data_to_sqlite.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/scripts/cornell_movie_dialogs/data_to_sqlite_test.py` & `fedjax-0.0.9/fedjax/datasets/scripts/cornell_movie_dialogs/data_to_sqlite_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/scripts/sent140/data_to_sqlite.py` & `fedjax-0.0.9/fedjax/datasets/scripts/sent140/data_to_sqlite.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/scripts/sent140/data_to_sqlite_test.py` & `fedjax-0.0.9/fedjax/datasets/scripts/sent140/data_to_sqlite_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/shakespeare.py` & `fedjax-0.0.9/fedjax/datasets/shakespeare.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/shakespeare_test.py` & `fedjax-0.0.9/fedjax/datasets/shakespeare_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/datasets/stackoverflow.py` & `fedjax-0.0.9/fedjax/datasets/stackoverflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         The special tokens are added and handled automatically by the tokenizer.
         The preprocessed examples will have vocabulary size `len(vocab) + 3 +
         num_oov_buckets`.
       default_vocab_size: Number of words in the default vocabulary. This is
         only used when `vocab` is not specified. The preprocessed examples will
         have vocabulary size `default_vocab_size + 3 + num_oov_buckets`
         with 3 special labels: 0 (PAD), 1 (BOS), 2 (EOS), and `num_oov_buckets`
-          OOV labels starting at `default_vocab_size + 3`.
+        OOV labels starting at `default_vocab_size + 3`.
       num_oov_buckets: Number of out of vocabulary buckets.
     """
     if vocab is None:
       # Load default vocabulary.
       vocab = default_vocab(default_vocab_size)
     with tf.device('cpu'):
       self._table = tf.lookup.StaticVocabularyTable(
```

### Comparing `fedjax-0.0.8/fedjax/datasets/stackoverflow_test.py` & `fedjax-0.0.9/fedjax/datasets/stackoverflow_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/experimental/__init__.py` & `fedjax-0.0.9/fedjax/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/fedjax_test.py` & `fedjax-0.0.9/fedjax/fedjax_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/models/__init__.py` & `fedjax-0.0.9/fedjax/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/models/emnist.py` & `fedjax-0.0.9/fedjax/models/emnist.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/models/emnist_test.py` & `fedjax-0.0.9/fedjax/models/emnist_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/models/shakespeare.py` & `fedjax-0.0.9/fedjax/models/shakespeare.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/models/shakespeare_test.py` & `fedjax-0.0.9/fedjax/models/shakespeare_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/models/stackoverflow.py` & `fedjax-0.0.9/fedjax/models/stackoverflow.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/models/stackoverflow_test.py` & `fedjax-0.0.9/fedjax/models/stackoverflow_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/models/toy_regression.py` & `fedjax-0.0.9/fedjax/models/toy_regression.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/models/toy_regression_test.py` & `fedjax-0.0.9/fedjax/models/toy_regression_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/__init__.py` & `fedjax-0.0.9/fedjax/training/__init__.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/checkpoint.py` & `fedjax-0.0.9/fedjax/training/checkpoint.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/checkpoint_test.py` & `fedjax-0.0.9/fedjax/training/checkpoint_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/federated_experiment.py` & `fedjax-0.0.9/fedjax/training/federated_experiment.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/federated_experiment_test.py` & `fedjax-0.0.9/fedjax/training/federated_experiment_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/logging.py` & `fedjax-0.0.9/fedjax/training/logging.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/logging_test.py` & `fedjax-0.0.9/fedjax/training/logging_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/structured_flags.py` & `fedjax-0.0.9/fedjax/training/structured_flags.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/structured_flags_test.py` & `fedjax-0.0.9/fedjax/training/structured_flags_test.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/training/tasks.py` & `fedjax-0.0.9/fedjax/training/tasks.py`

 * *Files identical despite different names*

### Comparing `fedjax-0.0.8/fedjax/version.py` & `fedjax-0.0.9/fedjax/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """FedJAX version."""
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
```

### Comparing `fedjax-0.0.8/fedjax.egg-info/PKG-INFO` & `fedjax-0.0.9/fedjax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedjax
-Version: 0.0.8
+Version: 0.0.9
 Summary: Federated learning simulation with JAX.
 Home-page: https://github.com/google/fedjax
 Author: FedJAX Team
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: federated python machine learning
 Platform: UNKNOWN
@@ -120,32 +120,35 @@
     jnp.sum(client_weights))
   # Server learning rate of 0.01.
   server_params = server_params - server_update * 0.01
 ```
 
 ## Installation
 
-You will need Python 3.6 or later and a working JAX installation. For a CPU-only
-version:
+You will need a moderately recent version of Python. Please check
+[the PyPI page](https://pypi.org/project/fedjax/) for the up to date version
+requirement.
+
+First, install JAX. For a CPU-only version:
 
 ```
 pip install --upgrade pip
 pip install --upgrade jax jaxlib  # CPU-only version
 ```
 
 For other devices (e.g. GPU), follow
 [these instructions](https://github.com/google/jax#installation).
 
-Then, install fedjax from PyPi:
+Then, install FedJAX from PyPI:
 
 ```
 pip install fedjax
 ```
 
-Or, to upgrade to the latest version of fedjax:
+Or, to upgrade to the latest version of FedJAX:
 
 ```
 pip install --upgrade git+https://github.com/google/fedjax.git
 ```
 
 ## Citing FedJAX
```

### Comparing `fedjax-0.0.8/fedjax.egg-info/SOURCES.txt` & `fedjax-0.0.9/fedjax.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 fedjax.egg-info/requires.txt
 fedjax.egg-info/top_level.txt
 fedjax/aggregators/__init__.py
 fedjax/aggregators/aggregator.py
 fedjax/aggregators/aggregator_test.py
 fedjax/aggregators/compression.py
 fedjax/aggregators/compression_test.py
+fedjax/aggregators/walsh_hadamard.py
+fedjax/aggregators/walsh_hadamard_test.py
 fedjax/algorithms/__init__.py
 fedjax/algorithms/agnostic_fed_avg.py
 fedjax/algorithms/agnostic_fed_avg_test.py
 fedjax/algorithms/fed_avg.py
 fedjax/algorithms/fed_avg_test.py
 fedjax/algorithms/hyp_cluster.py
 fedjax/algorithms/hyp_cluster_test.py
```

### Comparing `fedjax-0.0.8/setup.py` & `fedjax-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         'absl-py',
         'dm-haiku',
         'jax',
         'jaxlib',
         'msgpack',
         'optax',
         'requests',
+        'scipy',
     ],
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
```

