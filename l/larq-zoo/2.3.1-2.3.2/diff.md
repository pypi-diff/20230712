# Comparing `tmp/larq-zoo-2.3.1.tar.gz` & `tmp/larq-zoo-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "larq-zoo-2.3.1.tar", last modified: Mon Aug 22 14:19:05 2022, max compression
+gzip compressed data, was "larq-zoo-2.3.2.tar", last modified: Wed Jul 12 15:25:59 2023, max compression
```

## Comparing `larq-zoo-2.3.1.tar` & `larq-zoo-2.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:05.979469 larq-zoo-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-08-22 14:19:05.979469 larq-zoo-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:05.975469 larq-zoo-2.3.1/larq_zoo/
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:05.975469 larq-zoo-2.3.1/larq_zoo/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/core/model_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     6845 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:05.975469 larq-zoo-2.3.1/larq_zoo/literature/
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/literature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6109 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/literature/binary_alex_net.py
--rw-r--r--   0 runner    (1001) docker     (121)     6136 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/literature/birealnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    16277 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/literature/densenet.py
--rw-r--r--   0 runner    (1001) docker     (121)     6512 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/literature/dorefanet.py
--rw-r--r--   0 runner    (1001) docker     (121)     9575 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/literature/meliusnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    16809 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/literature/real_to_bin_nets.py
--rw-r--r--   0 runner    (1001) docker     (121)     7274 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/literature/resnet_e.py
--rw-r--r--   0 runner    (1001) docker     (121)     6784 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/literature/xnornet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:05.975469 larq-zoo-2.3.1/larq_zoo/sota/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/sota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13040 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/sota/quicknet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:05.979469 larq-zoo-2.3.1/larq_zoo/training/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5612 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/basic_experiments.py
--rw-r--r--   0 runner    (1001) docker     (121)     8325 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/data.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:05.979469 larq-zoo-2.3.1/larq_zoo/training/knowledge_distillation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/knowledge_distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21532 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/knowledge_distillation/knowledge_distillation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7779 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/knowledge_distillation/multi_stage_training.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/learning_schedules.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5461 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/multi_stage_experiments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/sota_experiments.py
--rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/larq_zoo/training/train.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:05.975469 larq-zoo-2.3.1/larq_zoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-08-22 14:19:05.000000 larq-zoo-2.3.1/larq_zoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-08-22 14:19:05.000000 larq-zoo-2.3.1/larq_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 14:19:05.000000 larq-zoo-2.3.1/larq_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-22 14:19:05.000000 larq-zoo-2.3.1/larq_zoo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-08-22 14:19:05.000000 larq-zoo-2.3.1/larq_zoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-22 14:19:05.000000 larq-zoo-2.3.1/larq_zoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-08-22 14:19:05.979469 larq-zoo-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:05.979469 larq-zoo-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/tests/data_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/tests/models_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/tests/train_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-08-22 14:19:03.000000 larq-zoo-2.3.1/tests/version_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:59.565790 larq-zoo-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-12 15:25:59.565790 larq-zoo-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:59.561790 larq-zoo-2.3.2/larq_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:59.561790 larq-zoo-2.3.2/larq_zoo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/core/model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:59.565790 larq-zoo-2.3.2/larq_zoo/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/literature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/literature/binary_alex_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/literature/birealnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/literature/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/literature/dorefanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/literature/meliusnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/literature/real_to_bin_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/literature/resnet_e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/literature/xnornet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:59.565790 larq-zoo-2.3.2/larq_zoo/sota/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/sota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/sota/quicknet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:59.565790 larq-zoo-2.3.2/larq_zoo/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/basic_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:59.565790 larq-zoo-2.3.2/larq_zoo/training/knowledge_distillation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/knowledge_distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/knowledge_distillation/knowledge_distillation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/knowledge_distillation/multi_stage_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/learning_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/multi_stage_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/sota_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/larq_zoo/training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:59.561790 larq-zoo-2.3.2/larq_zoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-12 15:25:59.000000 larq-zoo-2.3.2/larq_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-12 15:25:59.000000 larq-zoo-2.3.2/larq_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:25:59.000000 larq-zoo-2.3.2/larq_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 15:25:59.000000 larq-zoo-2.3.2/larq_zoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-12 15:25:59.000000 larq-zoo-2.3.2/larq_zoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 15:25:59.000000 larq-zoo-2.3.2/larq_zoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-12 15:25:59.569790 larq-zoo-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:59.565790 larq-zoo-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/tests/data_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/tests/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/tests/train_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-12 15:25:56.000000 larq-zoo-2.3.2/tests/version_test.py
```

### Comparing `larq-zoo-2.3.1/LICENSE` & `larq-zoo-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/PKG-INFO` & `larq-zoo-2.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: larq-zoo
-Version: 2.3.1
+Version: 2.3.2
 Summary: Reference implementations of popular Binarized Neural Networks
 Home-page: https://github.com/plumerai/larq-zoo
 Author: Plumerai
 Author-email: opensource@plumerai.com
 License: Apache 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: tensorflow_gpu
@@ -35,16 +34,16 @@
 
 *Larq Zoo is part of a family of libraries for BNN development; you can also check out [Larq](https://github.com/larq/larq) for building and training BNNs and [Larq Compute Engine](https://github.com/larq/compute-engine) for deployment on mobile and edge devices.*
 
 ## Requirements
 
 Before installing Larq Zoo, please install:
 
-- [Python](https://python.org) version `3.6`, `3.7`, `3.8`, or `3.9`
-- [Tensorflow](https://www.tensorflow.org/install) version `1.15`, `2.0`, `2.1`, `2.2`, `2.3`, `2.4`, `2.5`, `2.6`, 2.7`, or `2.8`
+- [Python](https://python.org) version `3.8`, `3.9`, or `3.10`
+- [Tensorflow](https://www.tensorflow.org/install) version `2.4` up to `2.12` (latest at time of writing).
 
 ## Installation
 
 You can install Larq Zoo with Python's [pip](https://pip.pypa.io/en/stable/) package manager:
 
 ```shell
 pip install larq-zoo
```

### Comparing `larq-zoo-2.3.1/README.md` & `larq-zoo-2.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 *Larq Zoo is part of a family of libraries for BNN development; you can also check out [Larq](https://github.com/larq/larq) for building and training BNNs and [Larq Compute Engine](https://github.com/larq/compute-engine) for deployment on mobile and edge devices.*
 
 ## Requirements
 
 Before installing Larq Zoo, please install:
 
-- [Python](https://python.org) version `3.6`, `3.7`, `3.8`, or `3.9`
-- [Tensorflow](https://www.tensorflow.org/install) version `1.15`, `2.0`, `2.1`, `2.2`, `2.3`, `2.4`, `2.5`, `2.6`, 2.7`, or `2.8`
+- [Python](https://python.org) version `3.8`, `3.9`, or `3.10`
+- [Tensorflow](https://www.tensorflow.org/install) version `2.4` up to `2.12` (latest at time of writing).
 
 ## Installation
 
 You can install Larq Zoo with Python's [pip](https://pip.pypa.io/en/stable/) package manager:
 
 ```shell
 pip install larq-zoo
```

### Comparing `larq-zoo-2.3.1/larq_zoo/core/model_factory.py` & `larq-zoo-2.3.2/larq_zoo/core/model_factory.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/core/utils.py` & `larq-zoo-2.3.2/larq_zoo/core/utils.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/literature/__init__.py` & `larq-zoo-2.3.2/larq_zoo/literature/__init__.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/literature/binary_alex_net.py` & `larq-zoo-2.3.2/larq_zoo/literature/binary_alex_net.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/literature/birealnet.py` & `larq-zoo-2.3.2/larq_zoo/literature/birealnet.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/literature/densenet.py` & `larq-zoo-2.3.2/larq_zoo/literature/densenet.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/literature/dorefanet.py` & `larq-zoo-2.3.2/larq_zoo/literature/dorefanet.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/literature/meliusnet.py` & `larq-zoo-2.3.2/larq_zoo/literature/meliusnet.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/literature/real_to_bin_nets.py` & `larq-zoo-2.3.2/larq_zoo/literature/real_to_bin_nets.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/literature/resnet_e.py` & `larq-zoo-2.3.2/larq_zoo/literature/resnet_e.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/literature/xnornet.py` & `larq-zoo-2.3.2/larq_zoo/literature/xnornet.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/sota/quicknet.py` & `larq-zoo-2.3.2/larq_zoo/sota/quicknet.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/training/basic_experiments.py` & `larq-zoo-2.3.2/larq_zoo/training/basic_experiments.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/training/data.py` & `larq-zoo-2.3.2/larq_zoo/training/data.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/training/datasets.py` & `larq-zoo-2.3.2/larq_zoo/training/datasets.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/training/knowledge_distillation/knowledge_distillation.py` & `larq-zoo-2.3.2/larq_zoo/training/knowledge_distillation/knowledge_distillation.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/training/knowledge_distillation/multi_stage_training.py` & `larq-zoo-2.3.2/larq_zoo/training/knowledge_distillation/multi_stage_training.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/training/learning_schedules.py` & `larq-zoo-2.3.2/larq_zoo/training/learning_schedules.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/training/multi_stage_experiments.py` & `larq-zoo-2.3.2/larq_zoo/training/multi_stage_experiments.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/training/sota_experiments.py` & `larq-zoo-2.3.2/larq_zoo/training/sota_experiments.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo/training/train.py` & `larq-zoo-2.3.2/larq_zoo/training/train.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/larq_zoo.egg-info/PKG-INFO` & `larq-zoo-2.3.2/larq_zoo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: larq-zoo
-Version: 2.3.1
+Version: 2.3.2
 Summary: Reference implementations of popular Binarized Neural Networks
 Home-page: https://github.com/plumerai/larq-zoo
 Author: Plumerai
 Author-email: opensource@plumerai.com
 License: Apache 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: tensorflow_gpu
@@ -35,16 +34,16 @@
 
 *Larq Zoo is part of a family of libraries for BNN development; you can also check out [Larq](https://github.com/larq/larq) for building and training BNNs and [Larq Compute Engine](https://github.com/larq/compute-engine) for deployment on mobile and edge devices.*
 
 ## Requirements
 
 Before installing Larq Zoo, please install:
 
-- [Python](https://python.org) version `3.6`, `3.7`, `3.8`, or `3.9`
-- [Tensorflow](https://www.tensorflow.org/install) version `1.15`, `2.0`, `2.1`, `2.2`, `2.3`, `2.4`, `2.5`, `2.6`, 2.7`, or `2.8`
+- [Python](https://python.org) version `3.8`, `3.9`, or `3.10`
+- [Tensorflow](https://www.tensorflow.org/install) version `2.4` up to `2.12` (latest at time of writing).
 
 ## Installation
 
 You can install Larq Zoo with Python's [pip](https://pip.pypa.io/en/stable/) package manager:
 
 ```shell
 pip install larq-zoo
```

### Comparing `larq-zoo-2.3.1/larq_zoo.egg-info/SOURCES.txt` & `larq-zoo-2.3.2/larq_zoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/setup.py` & `larq-zoo-2.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 from setuptools import find_packages, setup
 
 
 def readme():
-    with open("README.md", "r") as f:
+    with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="larq-zoo",
-    version="2.3.1",
+    version="2.3.2",
     author="Plumerai",
     author_email="opensource@plumerai.com",
     description="Reference implementations of popular Binarized Neural Networks",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/plumerai/larq-zoo",
     packages=find_packages(),
     license="Apache 2.0",
     install_requires=[
         "numpy>=1.15.0",
         "packaging>=19",
-        "larq>=0.9.2,<0.13.0",
-        "zookeeper>=1.0.0,<1.4.0",
+        "larq>=0.9.2,<0.13.2",
+        "zookeeper>=1.0.0",
+        "typeguard<3.0.0",
+        "protobuf<3.20",
         "importlib-metadata ~= 2.0 ; python_version<'3.8'",
     ],
     extras_require={
-        "tensorflow": ["tensorflow>=1.15.0"],
-        "tensorflow_gpu": ["tensorflow-gpu>=1.15.0"],
+        "tensorflow": ["tensorflow>=2.4.0"],
+        "tensorflow_gpu": ["tensorflow-gpu>=2.4.0"],
         "test": [
-            "black==22.6.0",
-            "flake8==4.0.1",
-            "isort==5.10.1",
-            "pytype>=2022.01.05",
-            "pytest==7.0.1",
-            "pytest-cov==3.0.0",
-            "pytest-mock>=3.6.1,<3.9.0",
-            "pytest-xdist==2.5.0",
-            "Pillow>=8.4.0,<10.0.0",
-            "tensorflow_datasets>=3.1.0,!=4.3.0",
+            "black==23.7.0",
+            "dill==0.3.6",
+            "flake8==6.0.0",
+            "isort==5.12.0",
+            "pytype==2023.6.16",
+            "pytest==7.4.0",
+            "pytest-cov==4.1.0",
+            "pytest-mock==3.11.1",
+            "pytest-xdist==3.3.1",
+            "Pillow==10.0.0",
+            "tensorflow_datasets>=3.1.0,<4.9.0",
         ],
     },
     entry_points="""
         [console_scripts]
         lqz=larq_zoo.training.main:cli
     """,
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
     ],
 )
```

### Comparing `larq-zoo-2.3.1/tests/data_test.py` & `larq-zoo-2.3.2/tests/data_test.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/tests/models_test.py` & `larq-zoo-2.3.2/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/tests/train_test.py` & `larq-zoo-2.3.2/tests/train_test.py`

 * *Files identical despite different names*

### Comparing `larq-zoo-2.3.1/tests/utils_test.py` & `larq-zoo-2.3.2/tests/utils_test.py`

 * *Files identical despite different names*

