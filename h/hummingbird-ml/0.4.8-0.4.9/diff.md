# Comparing `tmp/hummingbird-ml-0.4.8.tar.gz` & `tmp/hummingbird-ml-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hummingbird-ml-0.4.8.tar", last modified: Tue Feb 28 17:30:17 2023, max compression
+gzip compressed data, was "hummingbird-ml-0.4.9.tar", last modified: Wed Jul 12 16:54:01 2023, max compression
```

## Comparing `hummingbird-ml-0.4.8.tar` & `hummingbird-ml-0.4.9.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.300576 hummingbird-ml-0.4.8/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)       69 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/.coveragerc
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.252575 hummingbird-ml-0.4.8/.devcontainer/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      911 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/.devcontainer/Dockerfile
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      196 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/.devcontainer/devcontainer.json
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      126 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/.flake8
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.244575 hummingbird-ml-0.4.8/.github/
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.256575 hummingbird-ml-0.4.8/.github/workflows/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6488 2023-02-28 04:33:36.000000 hummingbird-ml-0.4.8/.github/workflows/pythonapp.yml
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1029 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/.gitignore
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      430 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/.pre-commit-config.yaml
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      453 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/CODE_OF_CONDUCT.md
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4242 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/CONTRIBUTING.md
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      708 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/Dockerfile
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1162 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/LICENSE
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3351 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/NOTICE
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10964 2023-02-28 17:30:17.300576 hummingbird-ml-0.4.8/PKG-INFO
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9982 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/README.md
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2865 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/SECURITY.md
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1244 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/TROUBLESHOOTING.md
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.256575 hummingbird-ml-0.4.8/benchmarks/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      683 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/README.md
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      310 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    12895 2023-02-03 01:13:36.000000 hummingbird-ml-0.4.8/benchmarks/datasets.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.256575 hummingbird-ml-0.4.8/benchmarks/operators/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      487 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/operators/README.md
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      310 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/operators/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    12241 2022-06-22 23:08:33.000000 hummingbird-ml-0.4.8/benchmarks/operators/run.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9239 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/operators/score.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10986 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/benchmarks/operators/train.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.260576 hummingbird-ml-0.4.8/benchmarks/pipelines/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1728 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/pipelines/README.md
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    14551 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/benchmarks/pipelines/openml_pipelines.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6825 2022-06-22 23:08:33.000000 hummingbird-ml-0.4.8/benchmarks/pipelines/run.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2016 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/pipelines/score.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      682 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/timer.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.260576 hummingbird-ml-0.4.8/benchmarks/trees/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3284 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/trees/README.md
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      310 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/trees/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3635 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/trees/metrics.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    13558 2022-06-22 23:08:33.000000 hummingbird-ml-0.4.8/benchmarks/trees/run.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9763 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/trees/score.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9705 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/benchmarks/trees/train.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.260576 hummingbird-ml-0.4.8/hummingbird/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      518 2023-02-28 17:29:53.000000 hummingbird-ml-0.4.8/hummingbird/__init__.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.260576 hummingbird-ml-0.4.8/hummingbird/ml/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1346 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5988 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/_executor.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    36239 2023-02-28 04:33:34.000000 hummingbird-ml-0.4.8/hummingbird/ml/_parse.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    18450 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/_topology.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9131 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/_utils.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.264576 hummingbird-ml-0.4.8/hummingbird/ml/containers/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1769 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/containers/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1048 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/containers/_input_containers.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6583 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/containers/_sklearn_api_containers.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5413 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/containers/batch_container.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.264576 hummingbird-ml-0.4.8/hummingbird/ml/containers/sklearn/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      398 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/containers/sklearn/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9308 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/containers/sklearn/onnx_containers.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    12931 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/containers/sklearn/pytorch_containers.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10448 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/containers/sklearn/tvm_containers.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    22310 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/convert.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1451 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/exceptions.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.272576 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2795 2023-02-03 01:13:36.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1488 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_array_feature_extractor_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4223 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_decomposition_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1984 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_discretizer_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     8211 2023-02-03 01:13:36.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_gbdt_commons.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3587 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_imputer_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6522 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_kneighbors_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2590 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_label_encoder_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3221 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_linear_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5797 2023-02-03 01:13:36.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_mixture_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2811 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_mlp_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3394 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_nb_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1184 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_normalizer_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4478 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_one_hot_encoder_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1379 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_physical_operator.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1464 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_pipeline_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1529 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_scaler_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3794 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_sv_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    16826 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_tree_commons.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    27221 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_tree_implementations.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3352 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/constants.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4901 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/lightgbm.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.276576 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      380 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1942 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/array_feature_extractor.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1342 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/binarizer.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1120 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/feature_vectorizer.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1627 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/imputer.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1671 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/label_encoder.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4293 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/linear.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1323 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/normalizer.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1600 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/one_hot_encoder.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    14093 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/onnx_operator.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1426 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/scaler.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3626 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/sv.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    11201 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/tree_ensemble.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2969 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/prophet.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.280576 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      388 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3018 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/array_feature_extractor.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2224 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/bagging.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1497 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/cluster.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5493 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/decision_tree.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5835 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/decomposition.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2511 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/discretizer.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9087 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/gbdt.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    11535 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/iforest.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1941 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/imputer.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4938 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/kneighbors.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1407 2023-01-09 23:54:57.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/label_encoder.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5402 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/linear.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1744 2023-02-03 01:13:36.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/mixture.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2434 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/mlp.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3924 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/nb.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1124 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/normalizer.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1615 2023-02-03 01:13:34.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/one_hot_encoder.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3092 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/pipeline.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3326 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/poly_features.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2128 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/scaler.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2088 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/sv.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.280576 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sparkml/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      384 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sparkml/__init__.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1688 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sparkml/discretizer.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1712 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sparkml/linear.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1219 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sparkml/vector_assembler.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5824 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/xgb.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    16006 2023-02-28 04:33:34.000000 hummingbird-ml-0.4.8/hummingbird/ml/supported.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.284576 hummingbird-ml-0.4.8/hummingbird_ml.egg-info/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10964 2023-02-28 17:30:17.000000 hummingbird-ml-0.4.8/hummingbird_ml.egg-info/PKG-INFO
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     8008 2023-02-28 17:30:17.000000 hummingbird-ml-0.4.8/hummingbird_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)        1 2023-02-28 17:30:17.000000 hummingbird-ml-0.4.8/hummingbird_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      467 2023-02-28 17:30:17.000000 hummingbird-ml-0.4.8/hummingbird_ml.egg-info/requires.txt
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)       23 2023-02-28 17:30:17.000000 hummingbird-ml-0.4.8/hummingbird_ml.egg-info/top_level.txt
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.284576 hummingbird-ml-0.4.8/notebooks/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2586 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/notebooks/LGBM-ONNX-example.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     8610 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/notebooks/LGBM-ONNXML-example.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3192 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/notebooks/LGBM-example.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    31400 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/notebooks/LGBM_year_with_train.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3608 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/notebooks/XGB-example.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4006 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/notebooks/blog_example.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5669 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/notebooks/prophet-example.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4093 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/notebooks/sklearn-random-forest-example.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    31419 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/notebooks/sklearn_year_with_train.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    21629 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/notebooks/tvm_and_pyt_graph.ipynb
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      257 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/pyproject.toml
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      209 2023-02-28 17:30:17.300576 hummingbird-ml-0.4.8/setup.cfg
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2192 2023-02-03 01:13:36.000000 hummingbird-ml-0.4.8/setup.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.296576 hummingbird-ml-0.4.8/tests/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    32497 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_backends.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    34792 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_extra_conf.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    21988 2023-02-03 01:13:36.000000 hummingbird-ml-0.4.8/tests/test_lightgbm_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2226 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_no_extra_install.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4455 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_onnxml_binarizer_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    11954 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_onnxml_decision_tree_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4095 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_onnxml_imputer_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5073 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_onnxml_label_encoder_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    14904 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_onnxml_lightgbm_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7080 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_onnxml_linear_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3539 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_onnxml_normalizer_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6480 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_onnxml_one_hot_encoder_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7271 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_onnxml_scaler_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3878 2022-12-09 20:02:55.000000 hummingbird-ml-0.4.8/tests/test_onnxml_sv_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2507 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_prophet.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3215 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_array_feature_extractor_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3384 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_bagging.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3193 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_clustering.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    32950 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_decision_tree_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7000 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_decomposition.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2121 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_discretizer_converters.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1826 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_feature_union.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9521 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_gbdt_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6302 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_histgbdt_converters.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5777 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_imputer_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6272 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_isolation_forest_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     8958 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_kneighbors.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1630 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_label_encoder_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    19429 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_linear_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1911 2023-02-03 01:13:36.000000 hummingbird-ml-0.4.8/tests/test_sklearn_mixture.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4815 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_mlp_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2664 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_model_selection.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3472 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_multioutput_regression.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10300 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_nb_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3228 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_normalizer_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      671 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_notfitted.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3960 2023-02-03 01:13:34.000000 hummingbird-ml-0.4.8/tests/test_sklearn_one_hot_encoder_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    29908 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_pipeline.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2619 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_poly_features_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5596 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sklearn_scaler_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7534 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sklearn_sv_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1721 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sparkml_discretizer_converters.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2222 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sparkml_linear_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5257 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/test_sparkml_pipeline.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1837 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/tests/test_sparkml_vector_assembler.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    15198 2023-02-28 04:33:34.000000 hummingbird-ml-0.4.8/tests/test_xgboost_converter.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1164 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/tests/tree_utils.py
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.296576 hummingbird-ml-0.4.8/website/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      864 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/website/Makefile
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      476 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/website/README.md
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.296576 hummingbird-ml-0.4.8/website/images/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)   119242 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/images/1-simple-reg-tree.png
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    13078 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/images/2-calc-output.png
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    89665 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/images/3-matrix.png
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    74406 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.8/website/images/4-matrixnext.png
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    41753 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/images/5-singletensor.png
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    11746 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/images/hb-logo-notext.png
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.300576 hummingbird-ml-0.4.8/website/sphinx/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7370 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/Makefile
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.248575 hummingbird-ml-0.4.8/website/sphinx/_static/
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.300576 hummingbird-ml-0.4.8/website/sphinx/_static/css/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      367 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/_static/css/hummingbird.css
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.300576 hummingbird-ml-0.4.8/website/sphinx/_static/js/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2803 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/_static/js/copybutton.js
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.300576 hummingbird-ml-0.4.8/website/sphinx/_templates/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      290 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/_templates/class.rst
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      229 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/_templates/function.rst
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      172 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/_templates/module.rst_t
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      818 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/_templates/package.rst_t
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5433 2023-02-28 17:29:53.000000 hummingbird-ml-0.4.8/website/sphinx/conf.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      401 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/index.rst
-drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-02-28 17:30:17.300576 hummingbird-ml-0.4.8/website/sphinx/sphinxext/
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)       43 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/sphinxext/MANIFEST.in
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2602 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/sphinxext/github_link.py
--rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7956 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.8/website/sphinx/sphinxext/sphinx_issues.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.653142 hummingbird-ml-0.4.9/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)       69 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/.coveragerc
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.601141 hummingbird-ml-0.4.9/.devcontainer/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      911 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/.devcontainer/Dockerfile
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      196 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/.devcontainer/devcontainer.json
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      126 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/.flake8
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.593141 hummingbird-ml-0.4.9/.github/
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.601141 hummingbird-ml-0.4.9/.github/workflows/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6581 2023-07-12 16:53:56.000000 hummingbird-ml-0.4.9/.github/workflows/pythonapp.yml
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1029 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/.gitignore
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      430 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/.pre-commit-config.yaml
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      453 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4242 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/CONTRIBUTING.md
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      708 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/Dockerfile
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1162 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/LICENSE
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3351 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/NOTICE
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10964 2023-07-12 16:54:01.653142 hummingbird-ml-0.4.9/PKG-INFO
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9982 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/README.md
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2865 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/SECURITY.md
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1244 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/TROUBLESHOOTING.md
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.601141 hummingbird-ml-0.4.9/benchmarks/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      683 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/README.md
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      310 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    12895 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/benchmarks/datasets.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.605141 hummingbird-ml-0.4.9/benchmarks/operators/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      487 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/operators/README.md
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      310 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/operators/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    12241 2022-06-22 23:08:33.000000 hummingbird-ml-0.4.9/benchmarks/operators/run.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9239 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/operators/score.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10972 2023-06-21 21:23:44.000000 hummingbird-ml-0.4.9/benchmarks/operators/train.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.605141 hummingbird-ml-0.4.9/benchmarks/pipelines/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1728 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/pipelines/README.md
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    14551 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/benchmarks/pipelines/openml_pipelines.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6825 2022-06-22 23:08:33.000000 hummingbird-ml-0.4.9/benchmarks/pipelines/run.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2016 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/pipelines/score.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      682 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/timer.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.605141 hummingbird-ml-0.4.9/benchmarks/trees/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3284 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/trees/README.md
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      310 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/trees/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3635 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/trees/metrics.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    13558 2022-06-22 23:08:33.000000 hummingbird-ml-0.4.9/benchmarks/trees/run.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9763 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/trees/score.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9705 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/benchmarks/trees/train.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.605141 hummingbird-ml-0.4.9/hummingbird/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      518 2023-07-12 16:53:56.000000 hummingbird-ml-0.4.9/hummingbird/__init__.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.609141 hummingbird-ml-0.4.9/hummingbird/ml/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1346 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5988 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/_executor.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    36239 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/_parse.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    18450 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/_topology.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9757 2023-06-21 21:23:44.000000 hummingbird-ml-0.4.9/hummingbird/ml/_utils.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.609141 hummingbird-ml-0.4.9/hummingbird/ml/containers/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1769 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/containers/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1048 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/containers/_input_containers.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6693 2023-06-21 21:23:44.000000 hummingbird-ml-0.4.9/hummingbird/ml/containers/_sklearn_api_containers.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5413 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/containers/batch_container.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.609141 hummingbird-ml-0.4.9/hummingbird/ml/containers/sklearn/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      398 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/containers/sklearn/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10075 2023-06-21 21:23:44.000000 hummingbird-ml-0.4.9/hummingbird/ml/containers/sklearn/onnx_containers.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    13708 2023-06-21 21:23:44.000000 hummingbird-ml-0.4.9/hummingbird/ml/containers/sklearn/pytorch_containers.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    11215 2023-06-21 21:23:44.000000 hummingbird-ml-0.4.9/hummingbird/ml/containers/sklearn/tvm_containers.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    22310 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/convert.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1451 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/exceptions.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.613141 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2795 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1488 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_array_feature_extractor_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4223 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_decomposition_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1984 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_discretizer_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     8211 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_gbdt_commons.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3587 2023-04-04 00:00:38.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_imputer_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6522 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_kneighbors_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2590 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_label_encoder_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3125 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_linear_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5797 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_mixture_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2811 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_mlp_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3394 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_nb_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1184 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_normalizer_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4478 2023-06-12 20:59:03.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_one_hot_encoder_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1379 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_physical_operator.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1464 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_pipeline_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1529 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_scaler_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3794 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_sv_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    16826 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_tree_commons.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    27221 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_tree_implementations.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3352 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/constants.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4901 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/lightgbm.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.617141 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      380 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1942 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/array_feature_extractor.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1342 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/binarizer.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1120 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/feature_vectorizer.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1627 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/imputer.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1671 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/label_encoder.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4293 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/linear.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1323 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/normalizer.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1600 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/one_hot_encoder.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    14093 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/onnx_operator.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1426 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/scaler.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3626 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/sv.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    11201 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/tree_ensemble.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2969 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/prophet.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.621141 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      388 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3018 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/array_feature_extractor.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2224 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/bagging.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1497 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/cluster.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5493 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/decision_tree.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6081 2023-07-12 16:53:56.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/decomposition.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2511 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/discretizer.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9087 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/gbdt.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    11535 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/iforest.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1941 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/imputer.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4938 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/kneighbors.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1407 2023-01-09 23:54:57.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/label_encoder.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5402 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/linear.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1744 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/mixture.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2434 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/mlp.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3924 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/nb.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1124 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/normalizer.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1615 2023-05-09 16:05:26.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/one_hot_encoder.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3092 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/pipeline.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3326 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/poly_features.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2128 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/scaler.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2088 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/sv.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.621141 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sparkml/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      384 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sparkml/__init__.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1688 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sparkml/discretizer.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1712 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sparkml/linear.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1219 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sparkml/vector_assembler.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5824 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/xgb.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    16006 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/hummingbird/ml/supported.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.621141 hummingbird-ml-0.4.9/hummingbird_ml.egg-info/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10964 2023-07-12 16:54:01.000000 hummingbird-ml-0.4.9/hummingbird_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     8008 2023-07-12 16:54:01.000000 hummingbird-ml-0.4.9/hummingbird_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)        1 2023-07-12 16:54:01.000000 hummingbird-ml-0.4.9/hummingbird_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      472 2023-07-12 16:54:01.000000 hummingbird-ml-0.4.9/hummingbird_ml.egg-info/requires.txt
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)       23 2023-07-12 16:54:01.000000 hummingbird-ml-0.4.9/hummingbird_ml.egg-info/top_level.txt
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.629141 hummingbird-ml-0.4.9/notebooks/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2586 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/notebooks/LGBM-ONNX-example.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     8610 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/notebooks/LGBM-ONNXML-example.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3192 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/notebooks/LGBM-example.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    31400 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/notebooks/LGBM_year_with_train.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3608 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/notebooks/XGB-example.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4006 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/notebooks/blog_example.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5669 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/notebooks/prophet-example.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4093 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/notebooks/sklearn-random-forest-example.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    31419 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/notebooks/sklearn_year_with_train.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    21629 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/notebooks/tvm_and_pyt_graph.ipynb
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      257 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/pyproject.toml
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      209 2023-07-12 16:54:01.657142 hummingbird-ml-0.4.9/setup.cfg
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2198 2023-06-17 00:02:38.000000 hummingbird-ml-0.4.9/setup.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.641142 hummingbird-ml-0.4.9/tests/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    37572 2023-06-21 21:23:44.000000 hummingbird-ml-0.4.9/tests/test_backends.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    34792 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_extra_conf.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    21988 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_lightgbm_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2226 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/tests/test_no_extra_install.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4455 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_onnxml_binarizer_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    11954 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_onnxml_decision_tree_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4095 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_onnxml_imputer_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5073 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_onnxml_label_encoder_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    14869 2023-06-21 21:23:44.000000 hummingbird-ml-0.4.9/tests/test_onnxml_lightgbm_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7080 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_onnxml_linear_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3539 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_onnxml_normalizer_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6480 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_onnxml_one_hot_encoder_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7271 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/tests/test_onnxml_scaler_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3878 2022-12-09 20:02:55.000000 hummingbird-ml-0.4.9/tests/test_onnxml_sv_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2507 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_prophet.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3215 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_array_feature_extractor_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3384 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_bagging.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3193 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/tests/test_sklearn_clustering.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    32950 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/tests/test_sklearn_decision_tree_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7000 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_sklearn_decomposition.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2121 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_discretizer_converters.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1826 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_sklearn_feature_union.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     9521 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_sklearn_gbdt_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6302 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_histgbdt_converters.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5777 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_imputer_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     6272 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_isolation_forest_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     8958 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_sklearn_kneighbors.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1630 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_label_encoder_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    19429 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_sklearn_linear_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1911 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_sklearn_mixture.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     4815 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_mlp_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2664 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_model_selection.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3472 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_multioutput_regression.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    10300 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_nb_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3228 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_sklearn_normalizer_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      671 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/tests/test_sklearn_notfitted.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     3960 2023-06-12 20:59:03.000000 hummingbird-ml-0.4.9/tests/test_sklearn_one_hot_encoder_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    29908 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_pipeline.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2619 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_poly_features_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5596 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sklearn_scaler_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7534 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/tests/test_sklearn_sv_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1721 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sparkml_discretizer_converters.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2222 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_sparkml_linear_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5257 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/test_sparkml_pipeline.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1837 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_sparkml_vector_assembler.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    15198 2023-06-12 20:59:50.000000 hummingbird-ml-0.4.9/tests/test_xgboost_converter.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     1164 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/tests/tree_utils.py
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.641142 hummingbird-ml-0.4.9/website/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      864 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/website/Makefile
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      476 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/website/README.md
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.649142 hummingbird-ml-0.4.9/website/images/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)   119242 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/images/1-simple-reg-tree.png
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    13078 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/images/2-calc-output.png
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    89665 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/images/3-matrix.png
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    74406 2023-01-09 23:17:31.000000 hummingbird-ml-0.4.9/website/images/4-matrixnext.png
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    41753 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/images/5-singletensor.png
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)    11746 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/images/hb-logo-notext.png
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.649142 hummingbird-ml-0.4.9/website/sphinx/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7370 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/Makefile
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.593141 hummingbird-ml-0.4.9/website/sphinx/_static/
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.649142 hummingbird-ml-0.4.9/website/sphinx/_static/css/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      367 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/_static/css/hummingbird.css
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.649142 hummingbird-ml-0.4.9/website/sphinx/_static/js/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2803 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/_static/js/copybutton.js
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.653142 hummingbird-ml-0.4.9/website/sphinx/_templates/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      290 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/_templates/class.rst
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      229 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/_templates/function.rst
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      172 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/_templates/module.rst_t
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      818 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/_templates/package.rst_t
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     5433 2023-07-12 16:53:56.000000 hummingbird-ml-0.4.9/website/sphinx/conf.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)      401 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/index.rst
+drwxrwxr-x   0 kasaur    (1000) kasaur    (1000)        0 2023-07-12 16:54:01.653142 hummingbird-ml-0.4.9/website/sphinx/sphinxext/
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)       43 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/sphinxext/MANIFEST.in
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     2602 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/sphinxext/github_link.py
+-rw-rw-r--   0 kasaur    (1000) kasaur    (1000)     7956 2022-06-22 23:05:13.000000 hummingbird-ml-0.4.9/website/sphinx/sphinxext/sphinx_issues.py
```

### Comparing `hummingbird-ml-0.4.8/.devcontainer/Dockerfile` & `hummingbird-ml-0.4.9/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/.github/workflows/pythonapp.yml` & `hummingbird-ml-0.4.9/.github/workflows/pythonapp.yml`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   push:
     branches:
       - main
 
   pull_request:
     branches:
       - main
-      
+
   schedule:
     - cron: "15 21 * * FRI"
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
@@ -35,24 +35,26 @@
         python -m pip install --upgrade pip
         python -m pip install flake8
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # The GitHub editor is 127 chars wide
         flake8 . --count  --max-complexity=10 --max-line-length=127 --statistics
     # PyTorch CPU for Linux has different pip syntax wrt Win and Mac.
-    - name: Install torch-1.13.0+cpu if linux
+    - name: Install torch-2.0.0+cpu if linux
       if: ${{ startsWith(matrix.os, 'ubuntu') }}
-      run: python -m pip install torch==1.13.0 --extra-index-url https://download.pytorch.org/whl/cpu
-    - name: Install torch-1.13.0+cpu if not linux
+      run: python -m pip install torch==2.0.0 --extra-index-url https://download.pytorch.org/whl/cpu
+    - name: Install torch-2.0.0+cpu if not linux
       if:  ${{ !startsWith(matrix.os, 'ubuntu') }}
-      run: python -m pip install torch==1.13.0
+      run: python -m pip install torch==2.0.0
     - name: Install basic dependencies
       run: |
-        pip install git+https://github.com/onnx/sklearn-onnx.git
         python -m pip install -e .[tests] -f https://download.pytorch.org/whl/torch_stable.html
+    - name: Test with older SKLearn on Linux with py3.9 to check backward compatibility
+      if: ${{ matrix.python-version == '3.9' && startsWith(matrix.os, 'ubuntu') == true }}
+      run: python -m pip install scikit-learn==1.2.1
     # Compile (but not push) documentation only for one of the runs (Linux py3.8).
     - name: Generate Documentation
       if: ${{ matrix.python-version == '3.8' && startsWith(matrix.os, 'ubuntu') }}
       run: |
         # We're mocking out the torch. So now we also need to sub this on out
         find ../. -type f -exec sed -i 's/{torch.__version__}/1.12.0/g' {} +
         find ../. -type f -exec sed -i 's/torch.__version__/"1.12.0"/g' {} +
@@ -74,15 +76,14 @@
         export CPPFLAGS="$CPPFLAGS -Xpreprocessor -fopenmp"
         export CFLAGS="$CFLAGS -I/usr/local/opt/libomp/include"
         export CXXFLAGS="$CXXFLAGS -I/usr/local/opt/libomp/include"
         export LDFLAGS="$LDFLAGS -Wl,-rpath,/usr/local/opt/libomp/lib -L/usr/local/opt/libomp/lib -lomp"
     - name: Install extra dependencies
       run: |
         python -m pip install .[extra,onnx,sparkml]
-        pip install git+https://github.com/onnx/sklearn-onnx.git
         python -m pip install pandas
     - name: Install TVM from pypi if Ubuntu
       if: ${{ startsWith(matrix.os, 'ubuntu') }}
       run: python -m pip install apache-tvm==0.10.0
     - uses: actions/cache@v3
       # TVM takes forever, we try to cache it.
       if: ${{ startsWith(matrix.os, 'macos')}}
@@ -144,12 +145,12 @@
       if: ${{ matrix.python-version == '3.8' && startsWith(matrix.os, 'ubuntu') }}
       uses: codecov/codecov-action@v3
       with:
         file: ./coverage.xml
         flags: unittests
     - name: Deploy to GitHub pages 🚀
       if: ${{ github.ref == 'refs/heads/main' && matrix.python-version == '3.8' && startsWith(matrix.os, 'ubuntu') }}
-      uses: JamesIves/github-pages-deploy-action@4.0.0
+      uses: JamesIves/github-pages-deploy-action@v4.4.1
       with:
         branch: gh-pages
         folder: website/public
```

### Comparing `hummingbird-ml-0.4.8/.gitignore` & `hummingbird-ml-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/CONTRIBUTING.md` & `hummingbird-ml-0.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/Dockerfile` & `hummingbird-ml-0.4.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/LICENSE` & `hummingbird-ml-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/NOTICE` & `hummingbird-ml-0.4.9/NOTICE`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/PKG-INFO` & `hummingbird-ml-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hummingbird-ml
-Version: 0.4.8
+Version: 0.4.9
 Summary: Convert trained traditional machine learning models into tensor computations
 Home-page: https://github.com/microsoft/hummingbird
 Author: Microsoft Corporation
 Author-email: hummingbird-dev@microsoft.com
 License: MIT License
 Description: ## Introduction
         *Hummingbird* is a library for compiling trained traditional ML models into tensor computations. *Hummingbird* allows users to seamlessly leverage neural network frameworks (such as [PyTorch](https://pytorch.org/)) to accelerate traditional ML models. Thanks to *Hummingbird*, users can benefit from: (1) all the current and future optimizations implemented in neural network frameworks; (2) native hardware acceleration; (3) having a unique platform to support for both traditional and neural network models; and have all of this (4) without having to re-engineer their models.
```

### Comparing `hummingbird-ml-0.4.8/README.md` & `hummingbird-ml-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/SECURITY.md` & `hummingbird-ml-0.4.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/TROUBLESHOOTING.md` & `hummingbird-ml-0.4.9/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/README.md` & `hummingbird-ml-0.4.9/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/datasets.py` & `hummingbird-ml-0.4.9/benchmarks/datasets.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/operators/run.py` & `hummingbird-ml-0.4.9/benchmarks/operators/run.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/operators/score.py` & `hummingbird-ml-0.4.9/benchmarks/operators/score.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/operators/train.py` & `hummingbird-ml-0.4.9/benchmarks/operators/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 # Copyright (c) Microsoft Corporation. All rights reserved.
 
 from abc import ABC, abstractmethod
 import time
 import numpy as np
 import pandas as pd
-import pickle
 import os.path
 
 from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
 from sklearn.linear_model.stochastic_gradient import SGDClassifier
 from sklearn.naive_bayes import BernoulliNB
 from sklearn.neural_network import MLPClassifier
 from sklearn.tree import DecisionTreeClassifier
```

### Comparing `hummingbird-ml-0.4.8/benchmarks/pipelines/README.md` & `hummingbird-ml-0.4.9/benchmarks/pipelines/README.md`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/pipelines/openml_pipelines.py` & `hummingbird-ml-0.4.9/benchmarks/pipelines/openml_pipelines.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/pipelines/run.py` & `hummingbird-ml-0.4.9/benchmarks/pipelines/run.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/pipelines/score.py` & `hummingbird-ml-0.4.9/benchmarks/pipelines/score.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/timer.py` & `hummingbird-ml-0.4.9/benchmarks/timer.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/trees/README.md` & `hummingbird-ml-0.4.9/benchmarks/trees/README.md`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/trees/metrics.py` & `hummingbird-ml-0.4.9/benchmarks/trees/metrics.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/trees/run.py` & `hummingbird-ml-0.4.9/benchmarks/trees/run.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/trees/score.py` & `hummingbird-ml-0.4.9/benchmarks/trees/score.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/benchmarks/trees/train.py` & `hummingbird-ml-0.4.9/benchmarks/trees/train.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/__init__.py` & `hummingbird-ml-0.4.9/hummingbird/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 # license information.
 # --------------------------------------------------------------------------
 
 """
 Entrypoint for Hummingbird modules.
 """
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 __author__ = "Microsoft"
 __producer__ = "hummingbird"
 __producer_version__ = __version__
 __domain__ = "microsoft.gsl"
 __model_version__ = 0
```

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/__init__.py` & `hummingbird-ml-0.4.9/hummingbird/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/_executor.py` & `hummingbird-ml-0.4.9/hummingbird/ml/_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/_parse.py` & `hummingbird-ml-0.4.9/hummingbird/ml/_parse.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/_topology.py` & `hummingbird-ml-0.4.9/hummingbird/ml/_topology.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/_utils.py` & `hummingbird-ml-0.4.9/hummingbird/ml/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -233,48 +233,64 @@
     Utility function used to transform string inputs into a numerical representation.
     """
     shape = list(input.shape)
     shape.append(max_string_length // 4)
     return np.array(input, dtype="|S" + str(max_string_length)).view(np.int32).reshape(shape)
 
 
-def load(location):
+def load(location, digest=None):
     """
     Utility function used to load arbitrary Hummingbird models.
+
+    Args:
+        location: The location of the model.
+        digest (optional): A digest string to verify the model integrity (created during save).
     """
     # Add load capabilities.
     from hummingbird.ml.containers import PyTorchSklearnContainer
     from hummingbird.ml.containers import TVMSklearnContainer
     from hummingbird.ml.containers import ONNXSklearnContainer
     from hummingbird.ml.operator_converters import constants
+    import hmac
+    import hashlib
 
     model = None
     model_type = None
 
     # Unzip the dir.
     zip_location = location
     if not location.endswith("zip"):
         zip_location = location + ".zip"
     else:
         location = zip_location[:-4]
     assert os.path.exists(zip_location), "Zip file {} does not exist.".format(zip_location)
+
+    # Verify the digest if provided.
+    if digest is None:
+        print("Warning: No digest provided. Model integrity not verified.")
+    else:
+        with open(zip_location, 'rb') as file:
+            new_digest = hmac.new(b'shared-key', file.read(), hashlib.sha1).hexdigest()
+            if digest != new_digest:
+                raise RuntimeError('Integrity check failed')
+
     shutil.unpack_archive(zip_location, location, format="zip")
 
     assert os.path.exists(location), "Model location {} does not exist.".format(location)
 
     # Load the model type.
     with open(os.path.join(location, constants.SAVE_LOAD_MODEL_TYPE_PATH), "r") as file:
         model_type = file.readline()
 
     if "torch" in model_type:
-        model = PyTorchSklearnContainer.load(location, do_unzip_and_model_type_check=False)
+        model = PyTorchSklearnContainer.load(location, do_unzip_and_model_type_check=False, digest=digest)
     elif "onnx" in model_type:
-        model = ONNXSklearnContainer.load(location, do_unzip_and_model_type_check=False)
+        model = ONNXSklearnContainer.load(location, do_unzip_and_model_type_check=False, digest=digest)
     elif "tvm" in model_type:
-        model = TVMSklearnContainer.load(location, do_unzip_and_model_type_check=False)
+        model = TVMSklearnContainer.load(location, do_unzip_and_model_type_check=False, digest=digest)
     else:
         shutil.rmtree(location)
         raise RuntimeError("Model type {} not recognized.".format(model_type))
 
     assert model.model is not None
     return model
```

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/containers/__init__.py` & `hummingbird-ml-0.4.9/hummingbird/ml/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/containers/_input_containers.py` & `hummingbird-ml-0.4.9/hummingbird/ml/containers/_input_containers.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/containers/_sklearn_api_containers.py` & `hummingbird-ml-0.4.9/hummingbird/ml/containers/_sklearn_api_containers.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,17 @@
     @abstractmethod
     def save(self, location):
         """
         Method used to save the container for future use.
 
         Args:
             location: The location on the file system where to save the model.
+
+        Returns:
+            A string digest of the saved model to be used for integrity checks during load.
         """
         return
 
     def _run(self, function, *inputs):
         """
         This function scores the full dataset at once. See BatchContainer below for batched scoring.
         """
```

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/containers/batch_container.py` & `hummingbird-ml-0.4.9/hummingbird/ml/containers/batch_container.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/containers/sklearn/onnx_containers.py` & `hummingbird-ml-0.4.9/hummingbird/ml/containers/sklearn/onnx_containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         """
         Method used to save the container for future use.
 
         Args:
             location: The location on the file system where to save the model.
         """
         assert self.model is not None, "Saving a None model is undefined."
+        import hmac
+        import hashlib
 
         if constants.TEST_INPUT in self._extra_config:
             self._extra_config[constants.TEST_INPUT] = None
 
         if location.endswith("zip"):
             location = location[:-4]
         assert not os.path.exists(location), "Directory {} already exists.".format(location)
@@ -89,47 +91,64 @@
         # Save the container.
         with open(os.path.join(location, constants.SAVE_LOAD_CONTAINER_PATH), "wb") as file:
             pickle.dump(self, file)
 
         # Zip the dir.
         shutil.make_archive(location, "zip", location)
 
+        with open(location + '.zip', "rb") as file:
+            digest = hmac.new(b'shared-key', file.read(), hashlib.sha1).hexdigest()
+            print("Model saved with digest: {}".format(digest))
+
         # Remove the directory.
         shutil.rmtree(location)
 
         self._model = model
         self._session = session
+        return digest
 
     @staticmethod
-    def load(location, do_unzip_and_model_type_check=True):
+    def load(location, do_unzip_and_model_type_check=True, digest=None):
         """
         Method used to load a container from the file system.
 
         Args:
             location: The location on the file system where to load the model.
             do_unzip_and_model_type_check: Whether to unzip the model and check the type.
 
         Returns:
             The loaded model.
         """
 
         assert onnx_runtime_installed
         import onnx
         import onnxruntime as ort
+        import hmac
+        import hashlib
 
         container = None
 
         if do_unzip_and_model_type_check:
             # Unzip the dir.
             zip_location = location
             if not location.endswith("zip"):
                 zip_location = location + ".zip"
             else:
                 location = zip_location[:-4]
             assert os.path.exists(zip_location), "Zip file {} does not exist.".format(zip_location)
+
+            # Verify the digest if provided.
+            if digest is None:
+                print("Warning: No digest provided. Model integrity not verified.")
+            else:
+                with open(zip_location, 'rb') as file:
+                    new_digest = hmac.new(b'shared-key', file.read(), hashlib.sha1).hexdigest()
+                    if digest != new_digest:
+                        raise RuntimeError('Integrity check failed')
+
             shutil.unpack_archive(zip_location, location, format="zip")
 
             assert os.path.exists(location), "Model location {} does not exist.".format(location)
 
             # Load the model type.
             with open(os.path.join(location, constants.SAVE_LOAD_MODEL_TYPE_PATH), "r") as file:
                 model_type = file.readline()
```

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/containers/sklearn/pytorch_containers.py` & `hummingbird-ml-0.4.9/hummingbird/ml/containers/sklearn/pytorch_containers.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         """
         Method used to save the container for future use.
 
         Args:
             location: The location on the file system where to save the model.
         """
         assert self.model is not None, "Saving a None model is undefined."
+        import hmac
+        import hashlib
 
         if constants.TEST_INPUT in self._extra_config:
             self._extra_config[constants.TEST_INPUT] = None
 
         if location.endswith("zip"):
             location = location[:-4]
         assert not os.path.exists(location), "Directory {} already exists.".format(location)
@@ -58,15 +60,15 @@
         if "torch.jit" in str(type(self.model)):
             # This is a torchscript model.
             # Save the model type.
             with open(os.path.join(location, constants.SAVE_LOAD_MODEL_TYPE_PATH), "w") as file:
                 file.write("torch.jit")
 
             # Save the actual model.
-            self.model.save(os.path.join(location, constants.SAVE_LOAD_TORCH_JIT_PATH))
+            digest = self.model.save(os.path.join(location, constants.SAVE_LOAD_TORCH_JIT_PATH))
 
             model = self.model
             self._model = None
 
             # Save the container.
             with open(os.path.join(location, "container.pkl"), "wb") as file:
                 pickle.dump(self, file)
@@ -89,41 +91,59 @@
         versions = dump_versions(hummingbird, torch)
         with open(os.path.join(location, constants.SAVE_LOAD_MODEL_CONFIGURATION_PATH), "w") as file:
             file.writelines(versions)
 
         # Zip the dir.
         shutil.make_archive(location, "zip", location)
 
+        with open(location + '.zip', "rb") as file:
+            digest = hmac.new(b'shared-key', file.read(), hashlib.sha1).hexdigest()
+            print("Model saved with digest: {}".format(digest))
+
         # Remove the directory.
         shutil.rmtree(location)
 
+        return digest
+
     @staticmethod
-    def load(location, do_unzip_and_model_type_check=True, delete_unzip_location_folder: bool = True):
+    def load(location, do_unzip_and_model_type_check=True, delete_unzip_location_folder: bool = True, digest=None):
         """
         Method used to load a container from the file system.
 
         Args:
             location: The location on the file system where to load the model.
             do_unzip_and_model_type_check: Whether to unzip the model and check the type.
             delete_unzip_location_folder: Whether to delete the folder provided by caller or created by this method
                                             where the model is unzipped
 
         Returns:
             The loaded model.
         """
+        import hmac
+        import hashlib
         container = None
 
         # Unzip the dir.
         if do_unzip_and_model_type_check:
             zip_location = location
             if not location.endswith("zip"):
                 zip_location = location + ".zip"
             else:
                 location = zip_location[:-4]
             assert os.path.exists(zip_location), "Zip file {} does not exist.".format(zip_location)
+
+            # Verify the digest if provided.
+            if digest is None:
+                print("Warning: No digest provided. Model integrity not verified.")
+            else:
+                with open(zip_location, 'rb') as file:
+                    new_digest = hmac.new(b'shared-key', file.read(), hashlib.sha1).hexdigest()
+                    if digest != new_digest:
+                        raise RuntimeError('Integrity check failed')
+
             shutil.unpack_archive(zip_location, location, format="zip")
 
             assert os.path.exists(location), "Model location {} does not exist.".format(location)
 
         # Load the model type.
         with open(os.path.join(location, constants.SAVE_LOAD_MODEL_TYPE_PATH), "r") as file:
             model_type = file.readline()
```

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/containers/sklearn/tvm_containers.py` & `hummingbird-ml-0.4.9/hummingbird/ml/containers/sklearn/tvm_containers.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         """
         Method used to save the container for future use.
 
         Args:
             location: The location on the file system where to save the model.
         """
         assert self.model is not None, "Saving a None model is undefined."
+        import hmac
+        import hashlib
 
         if location.endswith("zip"):
             location = location[:-4]
         assert not os.path.exists(location), "Directory {} already exists.".format(location)
         os.makedirs(location)
 
         # Save the model type.
@@ -105,52 +107,69 @@
         # Save the container.
         with open(os.path.join(location, constants.SAVE_LOAD_CONTAINER_PATH), "wb") as file:
             dill.dump(self, file)
 
         # Zip the dir.
         shutil.make_archive(location, "zip", location)
 
+        with open(location + '.zip', "rb") as file:
+            digest = hmac.new(b'shared-key', file.read(), hashlib.sha1).hexdigest()
+            print("Model saved with digest: {}".format(digest))
+
         # Remove the directory.
         shutil.rmtree(location)
 
         # Restore the information
         self._tvm_tensors = input_tensors
         self._extra_config[constants.TVM_LIB] = lib
         self._extra_config[constants.TVM_GRAPH] = graph
         self._extra_config[constants.TVM_PARAMS] = params
         self._extra_config[constants.TVM_CONTEXT] = ctx
         self._ctx = ctx
         self._model = model
+        return digest
 
     @staticmethod
-    def load(location, do_unzip_and_model_type_check=True):
+    def load(location, do_unzip_and_model_type_check=True, digest=None):
         """
         Method used to load a container from the file system.
 
         Args:
             location: The location on the file system where to load the model.
             do_unzip_and_model_type_check: Whether to unzip the model and check the type.
 
         Returns:
             The loaded model.
         """
         assert tvm_installed(), "TVM Container requires TVM installed."
 
         from tvm.runtime.params import load_param_dict
+        import hmac
+        import hashlib
 
         container = None
 
         if do_unzip_and_model_type_check:
             # Unzip the dir.
             zip_location = location
             if not location.endswith("zip"):
                 zip_location = location + ".zip"
             else:
                 location = zip_location[:-4]
             assert os.path.exists(zip_location), "Zip file {} does not exist.".format(zip_location)
+
+            # Verify the digest if provided.
+            if digest is None:
+                print("Warning: No digest provided. Model integrity not verified.")
+            else:
+                with open(zip_location, 'rb') as file:
+                    new_digest = hmac.new(b'shared-key', file.read(), hashlib.sha1).hexdigest()
+                    if digest != new_digest:
+                        raise RuntimeError('Integrity check failed')
+
             shutil.unpack_archive(zip_location, location, format="zip")
 
             assert os.path.exists(location), "Model location {} does not exist.".format(location)
 
             # Load the model type.
             with open(os.path.join(location, constants.SAVE_LOAD_MODEL_TYPE_PATH), "r") as file:
                 model_type = file.readline()
```

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/convert.py` & `hummingbird-ml-0.4.9/hummingbird/ml/convert.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/exceptions.py` & `hummingbird-ml-0.4.9/hummingbird/ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/__init__.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_array_feature_extractor_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_array_feature_extractor_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_decomposition_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_decomposition_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_discretizer_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_discretizer_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_gbdt_commons.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_gbdt_commons.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_imputer_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_imputer_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_kneighbors_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_kneighbors_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_label_encoder_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_label_encoder_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_linear_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_linear_implementations.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,31 +32,35 @@
         self.multi_class = multi_class
         self.regression = is_linear_regression
         self.classification = not is_linear_regression
         self.loss = loss
         if self.loss is None and self.classification:
             self.loss = "log"
 
-        self.perform_class_select = False
-        if min(classes) != 0 or max(classes) != len(classes) - 1:
-            self.perform_class_select = True
-
         self.binary_classification = False
         if len(classes) == 2:
             self.binary_classification = True
 
     def forward(self, x):
         x = x.float()
         output = torch.addmm(self.intercepts, x, self.coefficients)
-        if self.multi_class == "multinomial":
-            output = torch.softmax(output, dim=1)
-        elif self.regression:
+
+        if self.regression:
             if self.loss == "log":
                 return torch.exp(output)
             return output
+
+        if self.binary_classification:
+            indices = (output > 0).squeeze().int()
+        else:
+            indices = torch.argmax(output, dim=1)
+        predict_res = torch.index_select(self.classes, 0, indices)
+
+        if self.multi_class == "multinomial":
+            output = torch.softmax(output, dim=1)
         else:
             if self.loss == "modified_huber":
                 output = torch.clip(output, -1, 1)
                 output += 1
                 output /= 2
             else:
                 output = torch.sigmoid(output)
@@ -73,11 +77,8 @@
                     output /= prob_sum.view((output.shape[0], -1))
                 else:
                     output /= torch.sum(output, dim=1, keepdim=True)
 
         if self.binary_classification:
             output = torch.cat([1 - output, output], dim=1)
 
-        if self.perform_class_select:
-            return torch.index_select(self.classes, 0, torch.argmax(output, dim=1)), output
-        else:
-            return torch.argmax(output, dim=1), output
+        return predict_res, output
```

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_mixture_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_mixture_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_mlp_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_mlp_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_nb_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_nb_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_normalizer_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_normalizer_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_one_hot_encoder_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_one_hot_encoder_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_physical_operator.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_physical_operator.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_pipeline_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_pipeline_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_scaler_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_scaler_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_sv_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_sv_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_tree_commons.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_tree_commons.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/_tree_implementations.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/_tree_implementations.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/constants.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/lightgbm.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/lightgbm.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/array_feature_extractor.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/array_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/binarizer.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/binarizer.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/feature_vectorizer.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/feature_vectorizer.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/imputer.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/imputer.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/label_encoder.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/label_encoder.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/linear.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/linear.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/normalizer.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/normalizer.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/one_hot_encoder.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/onnx_operator.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/onnx_operator.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/scaler.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/scaler.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/sv.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/sv.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/onnx/tree_ensemble.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/onnx/tree_ensemble.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/prophet.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/prophet.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/array_feature_extractor.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/array_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/bagging.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/bagging.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/cluster.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/decision_tree.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/decision_tree.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/decomposition.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,19 @@
         extra_config: Extra configuration used to select the best conversion strategy
 
     Returns:
         A PyTorch model
     """
     assert operator is not None, "Cannot convert None operator"
 
-    coefficients = operator.raw_operator.coef_
+    # Check if operator.raw_operator._coef_ does not exist, which means to transpose coefficients (#26016)
+    if hasattr(operator.raw_operator, "_coef_"):  # SKL<1.3
+        coefficients = operator.raw_operator.coef_
+    else:  # SKL>=1.3
+        coefficients = operator.raw_operator.coef_.T
     x_mean = operator.raw_operator._x_mean
     x_std = operator.raw_operator._x_std
     y_mean = operator.raw_operator._y_mean
     return CrossDecomposition(operator, x_mean, x_std, y_mean, coefficients.astype("float32"), device)
 
 
 register_converter("SklearnPCA", convert_sklearn_pca)
```

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/discretizer.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/discretizer.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/gbdt.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/gbdt.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/iforest.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/iforest.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/imputer.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/imputer.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/kneighbors.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/kneighbors.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/label_encoder.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/label_encoder.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/linear.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/linear.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/mixture.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/mixture.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/mlp.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/mlp.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/nb.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/nb.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/normalizer.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/normalizer.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/one_hot_encoder.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/pipeline.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/poly_features.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/poly_features.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/scaler.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/scaler.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sklearn/sv.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sklearn/sv.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sparkml/discretizer.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sparkml/discretizer.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sparkml/linear.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sparkml/linear.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/sparkml/vector_assembler.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/sparkml/vector_assembler.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/operator_converters/xgb.py` & `hummingbird-ml-0.4.9/hummingbird/ml/operator_converters/xgb.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird/ml/supported.py` & `hummingbird-ml-0.4.9/hummingbird/ml/supported.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/hummingbird_ml.egg-info/PKG-INFO` & `hummingbird-ml-0.4.9/hummingbird_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hummingbird-ml
-Version: 0.4.8
+Version: 0.4.9
 Summary: Convert trained traditional machine learning models into tensor computations
 Home-page: https://github.com/microsoft/hummingbird
 Author: Microsoft Corporation
 Author-email: hummingbird-dev@microsoft.com
 License: MIT License
 Description: ## Introduction
         *Hummingbird* is a library for compiling trained traditional ML models into tensor computations. *Hummingbird* allows users to seamlessly leverage neural network frameworks (such as [PyTorch](https://pytorch.org/)) to accelerate traditional ML models. Thanks to *Hummingbird*, users can benefit from: (1) all the current and future optimizations implemented in neural network frameworks; (2) native hardware acceleration; (3) having a unique platform to support for both traditional and neural network models; and have all of this (4) without having to re-engineer their models.
```

### Comparing `hummingbird-ml-0.4.8/hummingbird_ml.egg-info/SOURCES.txt` & `hummingbird-ml-0.4.9/hummingbird_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/LGBM-ONNX-example.ipynb` & `hummingbird-ml-0.4.9/notebooks/LGBM-ONNX-example.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/LGBM-ONNXML-example.ipynb` & `hummingbird-ml-0.4.9/notebooks/LGBM-ONNXML-example.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/LGBM-example.ipynb` & `hummingbird-ml-0.4.9/notebooks/LGBM-example.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/LGBM_year_with_train.ipynb` & `hummingbird-ml-0.4.9/notebooks/LGBM_year_with_train.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/XGB-example.ipynb` & `hummingbird-ml-0.4.9/notebooks/XGB-example.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/blog_example.ipynb` & `hummingbird-ml-0.4.9/notebooks/blog_example.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/prophet-example.ipynb` & `hummingbird-ml-0.4.9/notebooks/prophet-example.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/sklearn-random-forest-example.ipynb` & `hummingbird-ml-0.4.9/notebooks/sklearn-random-forest-example.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/sklearn_year_with_train.ipynb` & `hummingbird-ml-0.4.9/notebooks/sklearn_year_with_train.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/notebooks/tvm_and_pyt_graph.ipynb` & `hummingbird-ml-0.4.9/notebooks/tvm_and_pyt_graph.ipynb`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/setup.py` & `hummingbird-ml-0.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,20 +28,21 @@
     "psutil",
     "dill",
     "protobuf>=3.20.2",
 ]
 onnx_requires = [
     "onnxruntime>=1.0.0",
     "onnxmltools>=1.6.0,<=1.11.0",
-    "skl2onnx>=1.7.0,<=1.12.0",
+    "skl2onnx>=1.7.0",
 ]
 extra_requires = [
     # The need each for these depends on which libraries you plan to convert from
     "xgboost>=0.90",
     "lightgbm>=2.2",
+    "holidays==0.24",
     "prophet==1.1",
 ]
 setup(
     name="hummingbird-ml",
     version=version_str,
     description="Convert trained traditional machine learning models into tensor computations",
     long_description=long_description,
@@ -51,15 +52,15 @@
     author_email="hummingbird-dev@microsoft.com",
     url="https://github.com/microsoft/hummingbird",
     packages=packages,
     include_package_data=True,
     install_requires=install_requires,
     extras_require={
         "tests": ["flake8", "pytest", "coverage", "pre-commit"],
-        "sparkml": ["pyspark>=2.4.4,<3.1.2", "pyarrow>1.0"],
+        "sparkml": ["pyspark>=2.4.4", "pyarrow>1.0"],
         "onnx": onnx_requires,
         "extra": extra_requires,
         "benchmark": onnx_requires + extra_requires + ["memory-profiler", "psutil"],
     },
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `hummingbird-ml-0.4.8/tests/test_backends.py` & `hummingbird-ml-0.4.9/tests/test_backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,14 +114,39 @@
         hb_model.save("pt-tmp")
 
         hb_model_loaded = hummingbird.ml.TorchContainer.load("pt-tmp")
         np.testing.assert_allclose(hb_model_loaded.predict_proba(X), hb_model.predict_proba(X), rtol=1e-06, atol=1e-06)
 
         os.remove("pt-tmp.zip")
 
+    # Test pytorch save and load with digest
+    def test_pytorch_save_load_with_digest(self):
+        warnings.filterwarnings("ignore")
+        max_depth = 10
+        num_classes = 2
+        model = GradientBoostingClassifier(n_estimators=10, max_depth=max_depth)
+        np.random.seed(0)
+        X = np.random.rand(100, 200)
+        X = np.array(X, dtype=np.float32)
+        y = np.random.randint(num_classes, size=100)
+
+        model.fit(X, y)
+
+        hb_model = hummingbird.ml.convert(model, "torch")
+        self.assertIsNotNone(hb_model)
+        my_digest = hb_model.save("pt-tmp")
+
+        hb_model_loaded = hummingbird.ml.TorchContainer.load("pt-tmp", digest=my_digest)
+        np.testing.assert_allclose(hb_model_loaded.predict_proba(X), hb_model.predict_proba(X), rtol=1e-06, atol=1e-06)
+
+        # Now try to load with a different digest
+        self.assertRaises(RuntimeError, hummingbird.ml.TorchContainer.load, "pt-tmp", digest="BAD_DIGEST")
+
+        os.remove("pt-tmp.zip")
+
     # Test pytorch save and load
     def test_pytorch_save_load_delete_folder(self):
         warnings.filterwarnings("ignore")
         max_depth = 10
         num_classes = 2
         model = GradientBoostingClassifier(n_estimators=10, max_depth=max_depth)
         np.random.seed(0)
@@ -303,14 +328,39 @@
         hb_model.save("ts-tmp")
 
         hb_model_loaded = hummingbird.ml.TorchContainer.load("ts-tmp")
         np.testing.assert_allclose(hb_model_loaded.predict_proba(X), hb_model.predict_proba(X), rtol=1e-06, atol=1e-06)
 
         os.remove("ts-tmp.zip")
 
+    # Test torchscript save and load with digest
+    def test_torchscript_save_load_digest(self):
+        warnings.filterwarnings("ignore")
+        max_depth = 10
+        num_classes = 2
+        model = GradientBoostingClassifier(n_estimators=10, max_depth=max_depth)
+        np.random.seed(0)
+        X = np.random.rand(100, 200)
+        X = np.array(X, dtype=np.float32)
+        y = np.random.randint(num_classes, size=100)
+
+        model.fit(X, y)
+
+        hb_model = hummingbird.ml.convert(model, "torch.jit", X)
+        self.assertIsNotNone(hb_model)
+        my_digest = hb_model.save("ts-tmp")
+
+        hb_model_loaded = hummingbird.ml.TorchContainer.load("ts-tmp", digest=my_digest)
+        np.testing.assert_allclose(hb_model_loaded.predict_proba(X), hb_model.predict_proba(X), rtol=1e-06, atol=1e-06)
+
+        # Now try to load with a different digest
+        self.assertRaises(RuntimeError, hummingbird.ml.TorchContainer.load, "ts-tmp", digest="BAD_DIGEST")
+
+        os.remove("ts-tmp.zip")
+
     # Test torchscript save and generic load
     def test_torchscript_save_generic_load(self):
         warnings.filterwarnings("ignore")
         max_depth = 10
         num_classes = 2
         model = GradientBoostingClassifier(n_estimators=10, max_depth=max_depth)
         np.random.seed(0)
@@ -418,14 +468,40 @@
         hb_model.save("tvm-tmp")
 
         hb_model_loaded = hummingbird.ml.TVMContainer.load("tvm-tmp")
         np.testing.assert_allclose(hb_model_loaded.predict_proba(X), hb_model.predict_proba(X), rtol=1e-06, atol=1e-06)
 
         os.remove("tvm-tmp.zip")
 
+    # Test tvm save and load
+    @unittest.skipIf(not tvm_installed(), reason="TVM test requires TVM installed")
+    def test_tvm_save_load_digest(self):
+        warnings.filterwarnings("ignore")
+        max_depth = 10
+        num_classes = 2
+        model = GradientBoostingClassifier(n_estimators=10, max_depth=max_depth)
+        np.random.seed(0)
+        X = np.random.rand(100, 200)
+        X = np.array(X, dtype=np.float32)
+        y = np.random.randint(num_classes, size=100)
+
+        model.fit(X, y)
+
+        hb_model = hummingbird.ml.convert(model, "tvm", X)
+        self.assertIsNotNone(hb_model)
+        my_digest = hb_model.save("tvm-tmp")
+
+        hb_model_loaded = hummingbird.ml.TVMContainer.load("tvm-tmp", digest=my_digest)
+        np.testing.assert_allclose(hb_model_loaded.predict_proba(X), hb_model.predict_proba(X), rtol=1e-06, atol=1e-06)
+
+        # Now try to load with a different digest
+        self.assertRaises(RuntimeError, hummingbird.ml.TVMContainer.load, "tvm-tmp", digest="BAD_DIGEST")
+
+        os.remove("tvm-tmp.zip")
+
     # Test tvm save and generic load
     @unittest.skipIf(not tvm_installed(), reason="TVM test requires TVM installed")
     def test_tvm_save_generic_load(self):
         warnings.filterwarnings("ignore")
         max_depth = 10
         num_classes = 2
         model = GradientBoostingClassifier(n_estimators=10, max_depth=max_depth)
@@ -513,14 +589,39 @@
 
         # Removing the configuration file with the versions does not create problems.
         os.remove(os.path.join("tvm-tmp", constants.SAVE_LOAD_MODEL_CONFIGURATION_PATH))
 
         hummingbird.ml.load("tvm-tmp")
         os.remove("tvm-tmp.zip")
 
+    # Test *generic* save and load with digest
+    def test_generic_save_load_with_digest(self):
+        warnings.filterwarnings("ignore")
+        max_depth = 10
+        num_classes = 2
+        model = GradientBoostingClassifier(n_estimators=10, max_depth=max_depth)
+        np.random.seed(0)
+        X = np.random.rand(100, 200)
+        X = np.array(X, dtype=np.float32)
+        y = np.random.randint(num_classes, size=100)
+
+        model.fit(X, y)
+
+        hb_model = hummingbird.ml.convert(model, "torch")
+        self.assertIsNotNone(hb_model)
+        my_digest = hb_model.save("gen-tmp")
+
+        hb_model_loaded = hummingbird.ml.load("gen-tmp", digest=my_digest)
+        np.testing.assert_allclose(hb_model_loaded.predict_proba(X), hb_model.predict_proba(X), rtol=1e-06, atol=1e-06)
+
+        # Now try to load with a different digest
+        self.assertRaises(RuntimeError, hummingbird.ml.load, "gen-tmp", digest="BAD_DIGEST")
+
+        os.remove("gen-tmp.zip")
+
     # Test onnx requires test_data or initial_types
     @unittest.skipIf(
         not (onnx_ml_tools_installed() and onnx_runtime_installed()), reason="ONNXML test require ONNX, ORT and ONNXMLTOOLS"
     )
     def test_onnx_no_test_data_float(self):
         warnings.filterwarnings("ignore")
         max_depth = 10
@@ -650,14 +751,40 @@
         hb_model.save("onnx-tmp")
 
         hb_model_loaded = hummingbird.ml.ONNXContainer.load("onnx-tmp")
         np.testing.assert_allclose(hb_model_loaded.predict_proba(X), hb_model.predict_proba(X), rtol=1e-06, atol=1e-06)
 
         os.remove("onnx-tmp.zip")
 
+    # Test ONNX save and load
+    @unittest.skipIf(not onnx_runtime_installed(), reason="ONNX test requires ORT")
+    def test_onnx_save_load_digest(self):
+        warnings.filterwarnings("ignore")
+        max_depth = 10
+        num_classes = 2
+        model = GradientBoostingClassifier(n_estimators=10, max_depth=max_depth)
+        np.random.seed(0)
+        X = np.random.rand(100, 200)
+        X = np.array(X, dtype=np.float32)
+        y = np.random.randint(num_classes, size=100)
+
+        model.fit(X, y)
+
+        hb_model = hummingbird.ml.convert(model, "onnx", X)
+        self.assertIsNotNone(hb_model)
+        my_digest = hb_model.save("onnx-tmp")
+
+        hb_model_loaded = hummingbird.ml.ONNXContainer.load("onnx-tmp", digest=my_digest)
+        np.testing.assert_allclose(hb_model_loaded.predict_proba(X), hb_model.predict_proba(X), rtol=1e-06, atol=1e-06)
+
+        # Now try to load with a different digest
+        self.assertRaises(RuntimeError, hummingbird.ml.ONNXContainer.load, "onnx-tmp", digest="BAD_DIGEST")
+
+        os.remove("onnx-tmp.zip")
+
     # Test ONNX save and generic load
     @unittest.skipIf(not onnx_runtime_installed(), reason="ONNX test requires ORT")
     def test_onnx_save_generic_load(self):
         warnings.filterwarnings("ignore")
         max_depth = 10
         num_classes = 2
         model = GradientBoostingClassifier(n_estimators=10, max_depth=max_depth)
```

### Comparing `hummingbird-ml-0.4.8/tests/test_extra_conf.py` & `hummingbird-ml-0.4.9/tests/test_extra_conf.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_lightgbm_converter.py` & `hummingbird-ml-0.4.9/tests/test_lightgbm_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_no_extra_install.py` & `hummingbird-ml-0.4.9/tests/test_no_extra_install.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_binarizer_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_binarizer_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_decision_tree_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_decision_tree_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_imputer_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_imputer_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_label_encoder_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_label_encoder_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_lightgbm_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_lightgbm_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """
 Tests lightgbm->onnxmltools->hb conversion for lightgbm models.
 """
 import unittest
 import warnings
 
-import sys
-import os
-import pickle
 import numpy as np
 from onnxconverter_common.data_types import FloatTensorType
 
 from hummingbird.ml import convert
 from hummingbird.ml import constants
 from hummingbird.ml._utils import onnx_ml_tools_installed, onnx_runtime_installed, lightgbm_installed
```

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_linear_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_linear_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_normalizer_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_normalizer_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_one_hot_encoder_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_one_hot_encoder_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_scaler_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_scaler_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_onnxml_sv_converter.py` & `hummingbird-ml-0.4.9/tests/test_onnxml_sv_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_prophet.py` & `hummingbird-ml-0.4.9/tests/test_prophet.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_array_feature_extractor_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_array_feature_extractor_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_bagging.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_bagging.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_clustering.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_clustering.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_decision_tree_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_decision_tree_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_decomposition.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_decomposition.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_discretizer_converters.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_discretizer_converters.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_feature_union.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_feature_union.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_gbdt_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_gbdt_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_histgbdt_converters.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_histgbdt_converters.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_imputer_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_imputer_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_isolation_forest_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_isolation_forest_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_kneighbors.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_kneighbors.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_label_encoder_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_label_encoder_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_linear_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_linear_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_mixture.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_mixture.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_mlp_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_mlp_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_model_selection.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_model_selection.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_multioutput_regression.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_multioutput_regression.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_nb_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_nb_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_normalizer_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_normalizer_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_notfitted.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_notfitted.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_one_hot_encoder_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_one_hot_encoder_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_pipeline.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_pipeline.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_poly_features_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_poly_features_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_scaler_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_scaler_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sklearn_sv_converter.py` & `hummingbird-ml-0.4.9/tests/test_sklearn_sv_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sparkml_discretizer_converters.py` & `hummingbird-ml-0.4.9/tests/test_sparkml_discretizer_converters.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sparkml_linear_converter.py` & `hummingbird-ml-0.4.9/tests/test_sparkml_linear_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sparkml_pipeline.py` & `hummingbird-ml-0.4.9/tests/test_sparkml_pipeline.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_sparkml_vector_assembler.py` & `hummingbird-ml-0.4.9/tests/test_sparkml_vector_assembler.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/test_xgboost_converter.py` & `hummingbird-ml-0.4.9/tests/test_xgboost_converter.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/tests/tree_utils.py` & `hummingbird-ml-0.4.9/tests/tree_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/Makefile` & `hummingbird-ml-0.4.9/website/Makefile`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/images/1-simple-reg-tree.png` & `hummingbird-ml-0.4.9/website/images/1-simple-reg-tree.png`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/images/2-calc-output.png` & `hummingbird-ml-0.4.9/website/images/2-calc-output.png`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/images/3-matrix.png` & `hummingbird-ml-0.4.9/website/images/3-matrix.png`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/images/4-matrixnext.png` & `hummingbird-ml-0.4.9/website/images/4-matrixnext.png`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/images/5-singletensor.png` & `hummingbird-ml-0.4.9/website/images/5-singletensor.png`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/images/hb-logo-notext.png` & `hummingbird-ml-0.4.9/website/images/hb-logo-notext.png`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/sphinx/Makefile` & `hummingbird-ml-0.4.9/website/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/sphinx/_static/js/copybutton.js` & `hummingbird-ml-0.4.9/website/sphinx/_static/js/copybutton.js`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/sphinx/_templates/package.rst_t` & `hummingbird-ml-0.4.9/website/sphinx/_templates/package.rst_t`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/sphinx/conf.py` & `hummingbird-ml-0.4.9/website/sphinx/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 copyright = u"2020, Microsoft"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "0.4.8"
+version = "0.4.9"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `hummingbird-ml-0.4.8/website/sphinx/sphinxext/github_link.py` & `hummingbird-ml-0.4.9/website/sphinx/sphinxext/github_link.py`

 * *Files identical despite different names*

### Comparing `hummingbird-ml-0.4.8/website/sphinx/sphinxext/sphinx_issues.py` & `hummingbird-ml-0.4.9/website/sphinx/sphinxext/sphinx_issues.py`

 * *Files identical despite different names*

