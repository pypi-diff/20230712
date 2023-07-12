# Comparing `tmp/useckit-0.3.3.tar.gz` & `tmp/useckit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "useckit-0.3.3.tar", last modified: Fri Jan 20 00:00:46 2023, max compression
+gzip compressed data, was "useckit-0.4.0.tar", last modified: Wed Jul 12 08:41:44 2023, max compression
```

## Comparing `useckit-0.3.3.tar` & `useckit-0.4.0.tar`

### file list

```diff
@@ -1,94 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.411307 useckit-0.3.3/
--rw-rw-rw-   0        0        0    35821 2021-01-21 13:00:25.000000 useckit-0.3.3/LICENSE
--rw-rw-rw-   0        0        0      523 2023-01-20 00:00:46.410313 useckit-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-01-19 23:13:48.000000 useckit-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-01-20 00:00:46.412423 useckit-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1009 2023-01-20 00:00:36.000000 useckit-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.130781 useckit-0.3.3/useckit/
--rw-rw-rw-   0        0        0     7931 2023-01-18 11:26:29.000000 useckit-0.3.3/useckit/Evaluators.py
--rw-rw-rw-   0        0        0      531 2023-01-16 21:07:19.000000 useckit-0.3.3/useckit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.196781 useckit-0.3.3/useckit/evaluation/
--rw-rw-rw-   0        0        0        0 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/evaluation/__init__.py
--rw-rw-rw-   0        0        0     1286 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/evaluation/identification.py
--rw-rw-rw-   0        0        0      937 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/evaluation/identification_with_reject.py
--rw-rw-rw-   0        0        0     2895 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/evaluation/verification.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.200791 useckit-0.3.3/useckit/paradigms/
--rw-rw-rw-   0        0        0        0 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/__init__.py
--rw-rw-rw-   0        0        0     8287 2023-01-18 12:14:50.000000 useckit-0.3.3/useckit/paradigms/_paradigm_base.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.206780 useckit-0.3.3/useckit/paradigms/anomaly_detection/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/__init__.py
--rw-rw-rw-   0        0        0     2517 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/anomaly_paradigm.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.228787 useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/__init__.py
--rw-rw-rw-   0        0        0     1907 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/_fixed_false_negative_thresholding_method.py
--rw-rw-rw-   0        0        0      690 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/anomaly_evaluation_method_base.py
--rw-rw-rw-   0        0        0     1496 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/identification.py
--rw-rw-rw-   0        0        0     2606 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/identification_with_reject.py
--rw-rw-rw-   0        0        0     3690 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/legacy_identification_with_reject.py
--rw-rw-rw-   0        0        0     2388 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/verification.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.238778 useckit-0.3.3/useckit/paradigms/anomaly_detection/prediction_models/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/prediction_models/__init__.py
--rw-rw-rw-   0        0        0     1484 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/prediction_models/anomaly_prediction_model_base.py
--rw-rw-rw-   0        0        0     8179 2023-01-19 23:13:48.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/prediction_models/auto_encoder_keras_prediction_model.py
--rw-rw-rw-   0        0        0     1282 2023-01-19 23:13:48.000000 useckit-0.3.3/useckit/paradigms/anomaly_detection/prediction_models/keras_model_descriptions.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.244783 useckit-0.3.3/useckit/paradigms/distance_learning/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.3.3/useckit/paradigms/distance_learning/__init__.py
--rw-rw-rw-   0        0        0     2467 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/distance_learning/distance_paradigm.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.262780 useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/__init__.py
--rw-rw-rw-   0        0        0     2730 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/_equal_error_thresholding_method.py
--rw-rw-rw-   0        0        0      623 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/distance_evaluation_method_base.py
--rw-rw-rw-   0        0        0     2160 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/identification.py
--rw-rw-rw-   0        0        0     3144 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/identification_with_reject.py
--rw-rw-rw-   0        0        0     1078 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/pairwise_accuracy_eval.py
--rw-rw-rw-   0        0        0     3254 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/verification.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.266783 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.275783 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/
--rw-rw-rw-   0        0        0        0 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/__init__.py
--rw-rw-rw-   0        0        0     5201 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_keras_prediction_model.py
--rw-rw-rw-   0        0        0     1674 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_model_description.py
--rw-rw-rw-   0        0        0      489 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/distance_prediction_model_base.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.287789 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/
--rw-rw-rw-   0        0        0        0 2023-01-12 19:59:01.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/__init__.py
--rw-rw-rw-   0        0        0     5171 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/offline_triplet_keras_prediction_model.py
--rw-rw-rw-   0        0        0     4031 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triple_tower_model.py
--rw-rw-rw-   0        0        0      682 2023-01-12 19:59:01.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triplet_distance_layer.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.299779 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/
--rw-rw-rw-   0        0        0        0 2023-01-12 19:59:01.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/__init__.py
--rw-rw-rw-   0        0        0     5214 2023-01-12 19:59:01.000000 useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/online_triplet_keras_prediction_model.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.305308 useckit-0.3.3/useckit/paradigms/time_series_classification/
--rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.318306 useckit-0.3.3/useckit/paradigms/time_series_classification/evaluation_methods/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/evaluation_methods/__init__.py
--rw-rw-rw-   0        0        0     1373 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/evaluation_methods/identification.py
--rw-rw-rw-   0        0        0     1733 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/evaluation_methods/legacy_identification.py
--rw-rw-rw-   0        0        0      396 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/evaluation_methods/tsc_evaluation_method_base.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.353305 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/
--rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/__init__.py
--rw-rw-rw-   0        0        0     4675 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/classification_keras_prediction_model.py
--rw-rw-rw-   0        0        0     5213 2023-01-19 23:13:48.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/inception.py
--rw-rw-rw-   0        0        0     9420 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/keras_model_descriptions.py
--rw-rw-rw-   0        0        0     3589 2023-01-19 23:13:48.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/mcdcnn.py
--rw-rw-rw-   0        0        0    23050 2023-01-19 23:13:48.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/mcnn.py
--rw-rw-rw-   0        0        0    11617 2023-01-19 23:13:48.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/tlenet.py
--rw-rw-rw-   0        0        0     1616 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/tsc_prediction_model_base.py
--rw-rw-rw-   0        0        0    12921 2023-01-19 23:13:48.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/twiesn.py
--rw-rw-rw-   0        0        0     2826 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/paradigms/time_series_classification/tsc_paradigm.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.384306 useckit-0.3.3/useckit/tests/
--rw-rw-rw-   0        0        0        0 2021-02-10 15:30:41.000000 useckit-0.3.3/useckit/tests/__init__.py
--rw-rw-rw-   0        0        0     3148 2023-01-18 13:11:17.000000 useckit-0.3.3/useckit/tests/test_dataset.py
--rw-rw-rw-   0        0        0     4123 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/tests/test_evaluations.py
--rw-rw-rw-   0        0        0     7686 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/tests/test_models.py
--rw-rw-rw-   0        0        0      536 2023-01-12 19:58:05.000000 useckit-0.3.3/useckit/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.401305 useckit-0.3.3/useckit/util/
--rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.3.3/useckit/util/__init__.py
--rw-rw-rw-   0        0        0    13798 2023-01-16 21:07:19.000000 useckit-0.3.3/useckit/util/dataset.py
--rw-rw-rw-   0        0        0    10235 2023-01-12 20:29:18.000000 useckit-0.3.3/useckit/util/plotting.py
--rw-rw-rw-   0        0        0    18872 2023-01-19 23:58:06.000000 useckit-0.3.3/useckit/util/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-20 00:00:46.185778 useckit-0.3.3/useckit.egg-info/
--rw-rw-rw-   0        0        0      523 2023-01-20 00:00:45.000000 useckit-0.3.3/useckit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4595 2023-01-20 00:00:45.000000 useckit-0.3.3/useckit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-20 00:00:45.000000 useckit-0.3.3/useckit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-01-20 00:00:45.000000 useckit-0.3.3/useckit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-20 00:00:45.000000 useckit-0.3.3/useckit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.927735 useckit-0.4.0/
+-rw-rw-rw-   0        0        0    35821 2021-01-21 13:00:25.000000 useckit-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      523 2023-07-12 08:41:44.927735 useckit-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2023-01-19 23:13:48.000000 useckit-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 08:41:44.927735 useckit-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2023-07-12 08:41:36.000000 useckit-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.810750 useckit-0.4.0/useckit/
+-rw-rw-rw-   0        0        0     7931 2023-01-18 11:26:29.000000 useckit-0.4.0/useckit/Evaluators.py
+-rw-rw-rw-   0        0        0      531 2023-01-16 21:07:19.000000 useckit-0.4.0/useckit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.823859 useckit-0.4.0/useckit/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-01-12 19:58:05.000000 useckit-0.4.0/useckit/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     3040 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/evaluation/identification.py
+-rw-rw-rw-   0        0        0      937 2023-01-12 20:29:18.000000 useckit-0.4.0/useckit/evaluation/identification_with_reject.py
+-rw-rw-rw-   0        0        0     4831 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/evaluation/verification.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.825859 useckit-0.4.0/useckit/paradigms/
+-rw-rw-rw-   0        0        0        0 2023-01-12 20:29:18.000000 useckit-0.4.0/useckit/paradigms/__init__.py
+-rw-rw-rw-   0        0        0     9750 2023-05-06 11:41:04.000000 useckit-0.4.0/useckit/paradigms/_paradigm_base.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.827971 useckit-0.4.0/useckit/paradigms/anomaly_detection/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/anomaly_paradigm.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.839120 useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/__init__.py
+-rw-rw-rw-   0        0        0     2012 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/_fixed_false_negative_thresholding_method.py
+-rw-rw-rw-   0        0        0      690 2023-01-12 19:58:05.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/anomaly_evaluation_method_base.py
+-rw-rw-rw-   0        0        0     1687 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/identification.py
+-rw-rw-rw-   0        0        0     2848 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/identification_with_reject.py
+-rw-rw-rw-   0        0        0     3693 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/legacy_identification_with_reject.py
+-rw-rw-rw-   0        0        0     2418 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/verification.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.847300 useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/anomaly_prediction_model_base.py
+-rw-rw-rw-   0        0        0     8667 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/auto_encoder_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     1342 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/keras_model_descriptions.py
+-rw-rw-rw-   0        0        0     2497 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/scikit_anomaly_prediction_model.py
+-rw-rw-rw-   0        0        0      587 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/scikit_model_descriptions.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.850300 useckit-0.4.0/useckit/paradigms/distance_learning/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.0/useckit/paradigms/distance_learning/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/distance_paradigm.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.864467 useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/__init__.py
+-rw-rw-rw-   0        0        0     3076 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/_equal_error_thresholding_method.py
+-rw-rw-rw-   0        0        0     4081 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/_sample_broadcasting.py
+-rw-rw-rw-   0        0        0      623 2023-01-12 19:58:05.000000 useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/distance_evaluation_method_base.py
+-rw-rw-rw-   0        0        0     4388 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/identification.py
+-rw-rw-rw-   0        0        0     5181 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/identification_with_reject.py
+-rw-rw-rw-   0        0        0     1078 2023-01-12 19:58:05.000000 useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/pairwise_accuracy_eval.py
+-rw-rw-rw-   0        0        0     7752 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/verification.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.869665 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.874654 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/
+-rw-rw-rw-   0        0        0        0 2023-01-12 19:58:05.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/__init__.py
+-rw-rw-rw-   0        0        0     5872 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     1674 2023-01-12 20:29:18.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_model_description.py
+-rw-rw-rw-   0        0        0      489 2023-01-12 19:58:05.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/distance_prediction_model_base.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.878800 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/
+-rw-rw-rw-   0        0        0        0 2023-01-12 19:59:01.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/__init__.py
+-rw-rw-rw-   0        0        0     5171 2023-01-12 20:29:18.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/offline_triplet_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     4035 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triple_tower_model.py
+-rw-rw-rw-   0        0        0      682 2023-01-12 19:59:01.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triplet_distance_layer.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.885802 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/
+-rw-rw-rw-   0        0        0        0 2023-01-12 19:59:01.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/__init__.py
+-rw-rw-rw-   0        0        0     5218 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/online_triplet_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     1959 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/scikit_distance_model.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.887968 useckit-0.4.0/useckit/paradigms/time_series_classification/
+-rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.893970 useckit-0.4.0/useckit/paradigms/time_series_classification/evaluation_methods/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:36:26.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/evaluation_methods/__init__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/evaluation_methods/identification.py
+-rw-rw-rw-   0        0        0     1733 2023-01-12 20:29:18.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/evaluation_methods/legacy_identification.py
+-rw-rw-rw-   0        0        0      396 2023-01-12 20:29:18.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/evaluation_methods/tsc_evaluation_method_base.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.911229 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/
+-rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/__init__.py
+-rw-rw-rw-   0        0        0     4675 2023-01-12 20:29:18.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/classification_keras_prediction_model.py
+-rw-rw-rw-   0        0        0     1597 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/classification_scikit_prediction_model.py
+-rw-rw-rw-   0        0        0     1512 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/classification_xgboost_prediction_model.py
+-rw-rw-rw-   0        0        0     5217 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/inception.py
+-rw-rw-rw-   0        0        0     9420 2023-01-12 19:58:05.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/keras_model_descriptions.py
+-rw-rw-rw-   0        0        0     3589 2023-01-19 23:13:48.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/mcdcnn.py
+-rw-rw-rw-   0        0        0    23759 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/mcnn.py
+-rw-rw-rw-   0        0        0    11621 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/tlenet.py
+-rw-rw-rw-   0        0        0     1616 2023-01-12 20:29:18.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/tsc_prediction_model_base.py
+-rw-rw-rw-   0        0        0    12771 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/twiesn.py
+-rw-rw-rw-   0        0        0     2692 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/paradigms/time_series_classification/tsc_paradigm.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.920593 useckit-0.4.0/useckit/tests/
+-rw-rw-rw-   0        0        0        0 2021-02-10 15:30:41.000000 useckit-0.4.0/useckit/tests/__init__.py
+-rw-rw-rw-   0        0        0     4312 2023-06-02 09:26:04.000000 useckit-0.4.0/useckit/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     5328 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/tests/test_evaluations.py
+-rw-rw-rw-   0        0        0     3773 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/tests/test_model_save_load.py
+-rw-rw-rw-   0        0        0    11092 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/tests/test_models.py
+-rw-rw-rw-   0        0        0     3061 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.925594 useckit-0.4.0/useckit/util/
+-rw-rw-rw-   0        0        0        0 2022-09-27 11:27:44.000000 useckit-0.4.0/useckit/util/__init__.py
+-rw-rw-rw-   0        0        0    13985 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/util/dataset.py
+-rw-rw-rw-   0        0        0     9142 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/util/dataset_windowsliced.py
+-rw-rw-rw-   0        0        0    10255 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/util/plotting.py
+-rw-rw-rw-   0        0        0    25370 2023-04-12 08:55:25.000000 useckit-0.4.0/useckit/util/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:41:44.817861 useckit-0.4.0/useckit.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-07-12 08:41:44.000000 useckit-0.4.0/useckit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5211 2023-07-12 08:41:44.000000 useckit-0.4.0/useckit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 08:41:44.000000 useckit-0.4.0/useckit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-07-12 08:41:44.000000 useckit-0.4.0/useckit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 08:41:44.000000 useckit-0.4.0/useckit.egg-info/top_level.txt
```

### Comparing `useckit-0.3.3/LICENSE` & `useckit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/PKG-INFO` & `useckit-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useckit
-Version: 0.3.3
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://blindforreview.com
 Author: BlindForReview.com
 Author-email: mail@blindforreview.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `useckit-0.3.3/setup.py` & `useckit-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="useckit",
-    version="0.3.3",
+    version="0.4.0",
     author="BlindForReview.com",
     author_email="mail@blindforreview.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://blindforreview.com",
     packages=setuptools.find_packages(include=['useckit', 'useckit.*']),
```

### Comparing `useckit-0.3.3/useckit/Evaluators.py` & `useckit-0.4.0/useckit/Evaluators.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/__init__.py` & `useckit-0.4.0/useckit/__init__.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/evaluation/identification_with_reject.py` & `useckit-0.4.0/useckit/evaluation/identification_with_reject.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/_paradigm_base.py` & `useckit-0.4.0/useckit/paradigms/_paradigm_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
+import pickle
 import random
+import sys
 import time
 from abc import ABC, abstractmethod
 from datetime import datetime
 
-import dill
 import numpy as np
 
 from useckit.util.dataset import Dataset
 from useckit.util.plotting import plot_history_df
 
 
 class PredictionModelBase(ABC):
@@ -82,51 +83,54 @@
         self.verbose = verbose
         if seed is not None:
             self.set_seed(seed)
         self._manage_output_dir(name, output_dir, subname, prediction_model)
         self._propagate_output_dir_to_model_evaluation(prediction_model, evaluation_methods)
 
     def persist(self):
-        with open(os.path.join(self.output_dir, f"paradigm_{self.name}.pickle"), "wb") as file:
-            dill.dump(self, file)
+        try:
+            with open(os.path.join(self.output_dir, f"paradigm_{self.name}.pickle"), "wb") as file:
+                pickle.dump(self, file)
+        except Exception as e:
+            print(f'useckit warning: persisting paradigm {self.name} ran into an exception {e}. Paradigm not persisted!',
+                  file=sys.stderr)
 
     @staticmethod
-    def restore(persisted_path_like: str, new_name: str, new_output_dir: str):
+    def restore(persisted_path_like: str, new_name: str, new_output_dir: str, new_subname: str = None):
         with open(persisted_path_like, "rb") as file:
-            paradigm = dill.load(file)
-            paradigm._manage_output_dir(new_name, new_output_dir)
+            paradigm = pickle.load(file)
+            paradigm._manage_output_dir(new_name, new_output_dir, new_subname, paradigm.prediction_model)
             paradigm._propagate_output_dir_to_model_evaluation(paradigm.prediction_model, paradigm.evalution_methods)
         return paradigm
 
     def _manage_output_dir(self, name: str, output_dir: str, subname: str, prediction_model):
         # root folder
         if output_dir is None or output_dir.strip() == "":
             self.output_dir = f"_useckit-out_" \
                               f"{ParadigmBase._init_timestamp}"
         else:
             self.output_dir = output_dir
         # subfolder
         if name is None or name.strip() == "":
             self.name = f"experiment_{ParadigmBase._experiment_number}_{type(self).__name__}"
-            if subname is not None:  # append to name if appendix is given
-                if subname.strip() != "":
-                    self.name += f'_{subname}'
-            else:
-                try:
-                    self.name += '_' + prediction_model.model_description.__name__
-                except AttributeError:
-                    # some models do not provide these descriptions, then we try to get the string via class name
-                    # in case this does not work out, we append nothing
-                    try:
-                        self.name += '_' + type(prediction_model).__name__
-                    except Exception:
-                        pass  # append nothing
-
         else:
             self.name = name
+        if subname is not None:  # append to name if appendix is given
+            if subname.strip() != "":
+                self.name += f'_{subname}'
+        else:
+            try:
+                self.name += '_' + prediction_model.model_description.__name__
+            except AttributeError:
+                # some models do not provide these descriptions, then we try to get the string via class name
+                # in case this does not work out, we append nothing
+                try:
+                    self.name += '_' + type(prediction_model).__name__
+                except Exception:
+                    pass  # append nothing
         self.output_dir = os.path.join(self.output_dir, self.name)
         os.makedirs(self.output_dir, exist_ok=True)
         ParadigmBase._experiment_number += 1
         if len(os.listdir(self.output_dir)) != 0:
             raise AttributeError(
                 "Please choose a unique name for your experiment or delete/move previous results, " +
                 "if you want to refrain from naming them by hand")
@@ -143,31 +147,49 @@
     def _set_evaluation_methods(self, evaluation_methods: [EvaluationMethodBase]):
         for eval_method in evaluation_methods:
             eval_method.merge_paradigm_output_folder(self.output_dir)
         self.evalution_methods = evaluation_methods
 
     def evaluate(self, dataset: Dataset):
         start_time = time.time()
+        with open(os.path.join(self.output_dir, 'timing.txt'), 'w') as f:
+            f.writelines(
+                ['# Start time timestamp:\n', f'{start_time}\n\n', '# Start time:\n',
+                 f'{datetime.fromtimestamp(start_time)}\n\n'])
 
         if self.verbose > 0:
             print(f'useckit info: persisting paradigm {self.name} of type {type(self).__name__}')
         self.persist()
 
         if self.verbose > 0:
             print(f'useckit info: fitting model of type {type(self.prediction_model).__name__}')
         self.fit_prediction_model(dataset)
 
+        with open(os.path.join(self.output_dir, 'timing.txt'), 'a') as f:
+            now = time.time()
+            f.writelines(
+                ['# Prediction finished time timestamp:\n', f'{now}\n\n', '# Prediction finished time:\n',
+                 f'{datetime.fromtimestamp(now)}\n\n', '# Prediction duration seconds:\n', f'{now - start_time}\n\n',
+                 '# Prediction duration:\n', f'{datetime.fromtimestamp(now) - datetime.fromtimestamp(start_time)}\n\n'])
+
         if self.verbose > 0:
             print(
                 f'useckit info: finished fitting model of type {type(self.prediction_model).__name__} ' +
                 f'after {round((time.time() - start_time), 2)} seconds.')
             print(f'useckit info: running evaluation methods')
 
         self.run_evaluation_methods(dataset)
 
+        with open(os.path.join(self.output_dir, 'timing.txt'), 'a') as f:
+            now = time.time()
+            f.writelines(
+                ['# Evaluation finished time timestamp:\n', f'{now}\n\n', '# Evaluation finished time:\n',
+                 f'{datetime.fromtimestamp(now)}\n\n', '# Evaluation duration seconds:\n', f'{now - start_time}\n\n',
+                 '# Evaluation duration:\n', f'{datetime.fromtimestamp(now) - datetime.fromtimestamp(start_time)}\n\n'])
+
         if self.verbose > 0:
             print(
                 f'useckit info: Finished evaluation the paradigm {self.name} of type {type(self)} ' +
                 f'after {round((time.time() - start_time), 2)} seconds.')
 
     def fit_prediction_model(self, dataset: Dataset) -> PredictionModelBase:
         self.prediction_model.fit(dataset)
```

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/anomaly_paradigm.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/anomaly_paradigm.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,31 @@
 from .prediction_models.auto_encoder_keras_prediction_model import AutoEncoderKerasPredictionModel
 from .._paradigm_base import ParadigmBase, PredictionModelBase
 from ...util.dataset import Dataset
 
 
 class AnomalyParadigm(ParadigmBase):
 
-    def __init__(self, name: str = None,
-                 output_dir: str = None,
+    def __init__(self,
                  prediction_model: AnomalyBasePredictionModel = None,
                  evaluation_methods: [AnomalyBaseEvaluationMethod] = None,
-                 verbose: bool = True,
                  seed=42,
+                 **base_kwargs
                  ):
         # This looks really stupid, but if the default value is initiated in the method head, not in the call to the
         # super constructor as blow, python will only instantiate one object for all calls to this method, hence
         # causing different paradigms to share the same instances of prediction model or evaluation method.
         # For more information see:
         # https://florimond.dev/en/posts/2018/08/python-mutable-defaults-are-the-source-of-all-evil/
-        super().__init__(prediction_model=AutoEncoderKerasPredictionModel() if prediction_model is None else prediction_model,
-                         name=name,
-                         output_dir=output_dir,
-                         evaluation_methods=
-                         [IdentificationOnly()] if evaluation_methods is None else evaluation_methods,
-                         verbose=verbose,
-                         seed=seed)
+        super().__init__(
+            prediction_model=AutoEncoderKerasPredictionModel() if prediction_model is None else prediction_model,
+            evaluation_methods=
+            [IdentificationOnly()] if evaluation_methods is None else evaluation_methods,
+            seed=seed,
+            **base_kwargs)
 
     def restore_prediction_model_trainables(self,
                                             anomaly_paradigm_prediction_model_directory_path_like: str,
                                             dataset: Dataset,
                                             individual_models_file_name_path_like: str = 'best_model.hdf5') \
             -> PredictionModelBase:
         self.prediction_model.restore_model_trainables(anomaly_paradigm_prediction_model_directory_path_like,
```

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/_fixed_false_negative_thresholding_method.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/_fixed_false_negative_thresholding_method.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import math
 import os
 
 import numpy as np
 import pandas as pd
 
 from useckit.paradigms.anomaly_detection.evaluation_methods.anomaly_evaluation_method_base import \
     BaseThresholdingMethod
@@ -15,26 +16,27 @@
     def __init__(self, anomaly_detection_model: AnomalyBasePredictionModel, output_dir: str,
                  target_false_negative_rate=0.05):
         self.target_false_negative_rate = target_false_negative_rate
         self.anomaly_detection_model = anomaly_detection_model
         self.output_dir = output_dir
 
     def compute_thresholds(self, enrollment_data: np.ndarray, enrollment_labels: np.ndarray) -> [float]:
-        result = []
-        prediction = self.anomaly_detection_model.predict(enrollment_data)
+        result = dict()
+        prediction, labels = self.anomaly_detection_model.predict(enrollment_data)
 
         columns = [f'{i}\'th model prediction' for i in list(range(len(prediction)))]
         pred_df = pd.DataFrame(prediction.transpose(), columns=columns)
         pred_df.to_csv(os.path.join(self.output_dir, 'enrollment_data_raw_predictions.csv'))
 
-        for user_index, anomaly_predictions in enumerate(prediction):
+        for user_index, anomaly_predictions in zip(labels, prediction):
             same_user_predictions = anomaly_predictions[enrollment_labels == user_index]
             same_user_predictions = np.sort(same_user_predictions)
             threshold_cutoff_index = len(same_user_predictions) * (1 - self.target_false_negative_rate)
             threshold_cutoff_index = math.floor(threshold_cutoff_index)
-            result.append(same_user_predictions[threshold_cutoff_index])
+            result[user_index] = same_user_predictions[threshold_cutoff_index]
 
-        result = np.array(result)
-        columns = [f'model thresholds']
-        result_df = pd.DataFrame(result, columns=columns)
+        result_copy = dict()
+        for key, value in result.items():
+            result_copy[str(key)] = [value]  # need to cast keys to str for pandas...
+        result_df = pd.DataFrame(result_copy)
         result_df.to_csv(os.path.join(self.output_dir, 'model_thresholds.csv'))
         return result
```

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/anomaly_evaluation_method_base.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/anomaly_evaluation_method_base.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/identification.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/identification.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,21 @@
     def __init__(self,
                  anomaly_prediction_model: AnomalyBasePredictionModel,
                  dataset: Dataset):
         self.anomaly_prediction_model = anomaly_prediction_model
         self.dataset = dataset
 
     def identify(self, samples: np.ndarray) -> np.ndarray:
-        preds = self.anomaly_prediction_model.predict(samples)
+        preds, labels = self.anomaly_prediction_model.predict(samples)
         preds = preds.transpose()  # 0-axis = samples, 1-axis = the predictions of the different models for the sample
-        preds = np.argmin(preds, axis=1)  # reduce to the indices of the model with the minimum prediction
-        return self.dataset.reverse_label_transform(preds)
+        result = np.argmin(preds, axis=1)  # reduce to the indices of the model with the minimum prediction
+        for i in range(len(result)):
+            result[i] = labels[result[i]]  # pick for each sample the label corresponding to the model with the
+            # min prediction
+        return self.dataset.reverse_label_transform(result)
 
 
 class IdentificationOnly(AnomalyBaseEvaluationMethod):
 
     def __init__(self,
                  output_dir: str = "evaluation_identification"):
         super().__init__(output_dir)
```

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/identification_with_reject.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/identification_with_reject.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,29 +8,35 @@
 from ....util.dataset import Dataset
 
 
 class AnomalyIdentificationOrRejectModel(IdentificationOrRejectModel):
 
     def __init__(self,
                  anomaly_prediction_model: AnomalyBasePredictionModel,
-                 rejection_thresholds_per_trained_user: [float],
+                 rejection_thresholds_per_trained_user: dict,
                  dataset: Dataset):
         self.anomaly_prediction_model = anomaly_prediction_model
         self.rejection_thresholds_per_trained_user = rejection_thresholds_per_trained_user
         self.dataset = dataset
 
     def identify_or_reject(self, samples: np.ndarray):
-        preds = self.anomaly_prediction_model.predict(samples)
+        preds, labels = self.anomaly_prediction_model.predict(samples)
         preds = preds.transpose()  # 0-axis = samples, 1-axis = the predictions of the different models for the sample
-        preds_identities = np.argmin(preds, axis=1)  # reduce to the indices of the model with the minimum prediction
-        for i in range(len(preds_identities)):
-            reject = preds[i][preds_identities[i]] >= self.rejection_thresholds_per_trained_user[preds_identities[i]]
+
+        result = np.argmin(preds, axis=1)  # reduce to the indices of the model with the minimum prediction
+        result_index = np.argmin(preds, axis=1)  # and a copy, please
+        for i in range(len(result)):
+            result[i] = labels[result[i]]  # pick for each sample the label corresponding to the model with the
+            # min prediction
+
+        for i in range(len(preds)):  # iterate all samples
+            reject = preds[i][result_index[i]] > self.rejection_thresholds_per_trained_user[labels[result_index[i]]]
             if reject:
-                preds_identities[i] = -1
-        return self.dataset.reverse_label_transform(preds_identities)
+                result[i] = -1
+        return self.dataset.reverse_label_transform(result)
 
 
 class IdentificationWithReject(AnomalyBaseEvaluationMethod):
 
     def __init__(self,
                  output_dir: str = "evaluation_identification_with_reject",
                  threshold_method: BaseThresholdingMethod = None):
```

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/legacy_identification_with_reject.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/legacy_identification_with_reject.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,8 +74,8 @@
 
         label_set = np.unique(np.concatenate((test_labels, test_predict_labels)))
         label_set = label_set[label_set != -1]
         label_names = dataset.reverse_label_transform(label_set)
         label_names = list(label_names)
         label_names.append("reject")
         plot_confusion_matrix(contingency_table, target_names=label_names, path=self.output_dir,
-                              title='Contingency Table', fname='contingency_table.pdf', normalize=False)
+                              title='Contingency Table', filename='contingency_table.pdf', normalize=False)
```

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/evaluation_methods/verification.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/evaluation_methods/verification.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,20 @@
     def __init__(self,
                  anomaly_prediction_model: AnomalyBasePredictionModel,
                  rejection_thresholds_per_trained_user: [float]):
         self.anomaly_prediction_model = anomaly_prediction_model
         self.rejection_thresholds_per_trained_user = rejection_thresholds_per_trained_user
 
     def verify(self, samples: np.ndarray, identity_claims: np.ndarray) -> np.ndarray:
-        preds = self.anomaly_prediction_model.predict(samples)
-        preds = preds.transpose()  # 0-axis = samples, 1-axis = the predictions of the different models for the sample
+        preds, labels = self.anomaly_prediction_model.predict(samples)
+
         result = np.zeros(shape=identity_claims.shape)
-        for i in range(len(identity_claims)):
-            reject = preds[i][identity_claims[i]] >= self.rejection_thresholds_per_trained_user[identity_claims[i]]
+        for i in range(len(identity_claims)):  # iterate over all samples
+            label_index = np.argwhere(labels == identity_claims[i])[0][0]  # this should never give more than 1 value!
+            reject = preds[label_index][i] > self.rejection_thresholds_per_trained_user[identity_claims[i]]
             if reject:
                 result[i] = 0
             else:
                 result[i] = 1
         return result == 1  # dirty transform to bool array
```

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/prediction_models/anomaly_prediction_model_base.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/anomaly_prediction_model_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import abstractmethod
+from typing import Tuple
 
 import numpy as np
 
 from useckit.util.dataset import Dataset
 from ..._paradigm_base import PredictionModelBase
 
 
@@ -15,26 +16,22 @@
     def fit(self, dataset: Dataset):
         pass
 
     # outputs a np array of shape (number_individual_models, x_test.shape[0]) containing the normalised mse values
     # the individual models produce when recreating the samples contained in x_test.
     # Therefore output[i][j] returns the i'th model's output (corresponding to the i'th user) of sample j.
     @abstractmethod
-    def predict(self, x_test) -> np.ndarray:
+    def predict(self, x_test) -> Tuple[np.ndarray, np.ndarray]:
         pass
 
     @abstractmethod
     def persist_model_trainables(self, path_like: str = 'saved_trainable_values',
                                  overridden_individual_file_name: str = None, **kwargs):
         pass
 
     @abstractmethod
     def restore_model_trainables(self,
                                  path_like: str,
                                  dataset: Dataset = None,
                                  path_like_individual_models_file_name: str = 'best_model.hdf5',
                                  **kwargs):
         pass
-
-    @abstractmethod
-    def modify_output_dir_for_individual_model(self, index: int, base_output_dir: str = None) -> str:
-        pass
```

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/prediction_models/auto_encoder_keras_prediction_model.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/auto_encoder_keras_prediction_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from dataclasses import dataclass
 from pathlib import Path
 
 import numpy as np
 import tensorflow.keras as keras
 
 from .anomaly_prediction_model_base import AnomalyBasePredictionModel
-from .keras_model_descriptions import BaseDescription, SequentialAutoEncoder
+from .keras_model_descriptions import KerasBaseDescription, SequentialAutoEncoder
 from ....util.dataset import Dataset
 from ....util.plotting import plot_history_df
 
 
 @dataclass
 class _IndividualModel:
     keras_model: keras.Model
     training_max_mse_threshold: float
     path_like_individual_model_file_name: str
+    label: int
 
 
 class AutoEncoderKerasPredictionModel(AnomalyBasePredictionModel):
     def persist_model_trainables(self, path_like: str = 'saved_trainable_values',
                                  overridden_individual_file_name: str = None, **kwargs):
         for i, model in enumerate(self.models):
             self._persist_individual_model(i, model, path_like, overridden_individual_file_name)
@@ -33,38 +34,43 @@
         else:
             file_name = path_like_individual_model_file_name_override
         output_dir = self.modify_output_dir_for_individual_model(index,
                                                                  base_output_dir=path_like_individual_model_parent_dir)
         model.keras_model.save_weights(os.path.join(output_dir, file_name))
         with open(os.path.join(output_dir, file_name + ".max_mse.pickle"), 'wb') as f:
             pickle.dump(model.training_max_mse_threshold, f)
+        with open(os.path.join(output_dir, file_name + ".label.pickle"), 'wb') as f:
+            pickle.dump(model.label, f)
 
     def restore_model_trainables(self,
                                  path_like: str,
                                  dataset: Dataset = None,
                                  path_like_individual_models_file_name: str = 'best_model.hdf5',
                                  **kwargs):
         x_train = dataset.trainset_data
         input_shape = x_train.shape[1:]
         nb_classes = dataset.train_classes()
         keras_models_built = self.build_model(input_shape, nb_classes)
         for i, keras_model in enumerate(keras_models_built):
             model = _IndividualModel(keras_model=keras_model, training_max_mse_threshold=0.,
-                                     path_like_individual_model_file_name=path_like_individual_models_file_name)
+                                     path_like_individual_model_file_name=path_like_individual_models_file_name, label=0)
             self._restore_individual_model(i, model, path_like)
 
     def _restore_individual_model(self, index: int, model: _IndividualModel,
                                   path_like_individual_model_parent_dir: str):
         output_dir = os.path.join(path_like_individual_model_parent_dir, f'auto_encoder_{index}')
         model.keras_model.load_weights(os.path.join(output_dir, model.path_like_individual_model_file_name))
         with open(os.path.join(output_dir, model.path_like_individual_model_file_name + ".max_mse.pickle"), 'rb') as f:
             model.training_max_mse_threshold = pickle.load(f)
+        with open(os.path.join(output_dir, model.path_like_individual_model_file_name + ".label.pickle"), 'rb') as f:
+            model.label = pickle.load(f)
+        self.models.append(model)
 
     def __init__(self,
-                 model_description: BaseDescription = SequentialAutoEncoder(),
+                 model_description: KerasBaseDescription = SequentialAutoEncoder(),
                  verbose: bool = True,
                  output_dir: str = "keras_prediction_model_out",
                  nb_epochs=100):
         super().__init__(output_dir=output_dir, verbose=verbose)
         self.validation_test_data_confusion_warning_printed_once = False
         self.model_description = model_description
         self.nb_epochs = nb_epochs
@@ -100,35 +106,35 @@
         x_train, y_train = dataset.trainset_data, dataset.trainset_labels
         x_val, y_val = dataset.validationset_data, dataset.validationset_labels
         input_shape = x_train.shape[1:]
         nb_classes = dataset.train_classes()
 
         assert nb_classes > 0
         keras_models_built = self.build_model(input_shape, nb_classes)
-        for i, keras_model in enumerate(keras_models_built):
+        for i, keras_model in zip(np.unique(y_train), keras_models_built):
             # find the elements in the training data that belong to class `i`
             training_indexes = y_train == i
             x_train_model_i = x_train[training_indexes]
 
             validation_indexes = y_val == i
             x_val_model_i = x_val[validation_indexes]
 
             model = _IndividualModel(keras_model=keras_model, training_max_mse_threshold=0.,
-                                     path_like_individual_model_file_name='best_model.hdf5')
+                                     path_like_individual_model_file_name='best_model.hdf5', label=i)
             self._persist_individual_model(i, model, self.output_dir, 'model_init.hdf5')
 
             if self.verbose:
                 print(f'useckit info: fitting AE {i + 1} of {nb_classes}')
                 model.keras_model.summary()
 
             callbacks = []
             model_checkpoint = keras.callbacks.ModelCheckpoint(
                 filepath=os.path.join(self.modify_output_dir_for_individual_model(i),
                                       model.path_like_individual_model_file_name),
-                monitor='loss',
+                monitor='val_loss',
                 save_best_only=True,
                 save_weights_only=True)
             callbacks.append(model_checkpoint)
             callbacks += self.model_description.callbacks()
 
             history = model.keras_model.fit(
                 x_train_model_i,
@@ -151,15 +157,17 @@
             # but whatever
             self._persist_individual_model(i, model, self.output_dir, 'best_model.hdf5')
 
             # store model in internal array
             self.models.append(model)
 
     def predict(self, x_test):
-        result = []
+        result_pred = []
+        result_id = []
         for i, model in enumerate(self.models):
             mse_list = []
             preds = model.keras_model.predict(x_test)
             for pred, x in zip(preds, x_test):
                 mse_list.append(self._get_mse(pred, x))
-            result.append(np.array(mse_list) / model.training_max_mse_threshold)
-        return np.array(result)
+            result_pred.append(np.array(mse_list) / model.training_max_mse_threshold)
+            result_id.append(model.label)
+        return np.array(result_pred), np.array(result_id)
```

### Comparing `useckit-0.3.3/useckit/paradigms/anomaly_detection/prediction_models/keras_model_descriptions.py` & `useckit-0.4.0/useckit/paradigms/anomaly_detection/prediction_models/keras_model_descriptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from abc import ABC, abstractmethod
 
 import numpy as np
+from sklearn.ensemble import RandomForestRegressor
 from tensorflow import keras
 from tensorflow.keras import Sequential
 from tensorflow.keras import layers
 
 
-class BaseDescription(ABC):
+class KerasBaseDescription(ABC):
 
     @abstractmethod
     def build_model(self, input_shape) -> keras.models.Model:
         pass
 
     @abstractmethod
     def callbacks(self) -> [keras.callbacks.Callback]:
         pass
 
 
-class SequentialAutoEncoder(BaseDescription):
+class SequentialAutoEncoder(KerasBaseDescription):
 
     def build_model(self, input_shape):
         hidden_size = np.prod(np.array(input_shape))
 
         model = Sequential()
-        model.add(layers.Dense(50, activation='relu', input_shape=input_shape))
-        model.add(layers.Flatten())
+        model.add(layers.Flatten(input_shape=input_shape))
+        model.add(layers.Dense(50, activation='relu'))
         model.add(layers.Dense(hidden_size, activation='sigmoid'))
         model.add(layers.Reshape(input_shape))
         model.build(input_shape=input_shape)
         model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['acc', 'mse'])
         return model
 
     def callbacks(self) -> [keras.callbacks.Callback]:
```

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/distance_paradigm.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/distance_paradigm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,32 @@
+from useckit.paradigms.distance_learning.prediction_models.contrastive_loss.contrastive_keras_prediction_model import ContrastiveKerasPredictionModel
 from useckit.util.dataset import Dataset
 from .evaluation_methods.distance_evaluation_method_base import DistanceBaseEvaluationMethod
 from .evaluation_methods.identification import IdentificationOnly
 from .prediction_models.distance_prediction_model_base import DistanceBasePredictionModel
-from useckit.paradigms.distance_learning.prediction_models.contrastive_loss.contrastive_keras_prediction_model import ContrastiveKerasPredictionModel
 from .._paradigm_base import ParadigmBase, PredictionModelBase
 
 
 class DistanceMetricParadigm(ParadigmBase):
 
-    def __init__(self, name: str = None,
-                 output_dir: str = None,
+    def __init__(self,
                  prediction_model: DistanceBasePredictionModel = None,
                  evaluation_methods: [DistanceBaseEvaluationMethod] = None,
-                 verbose: bool = True,
-                 seed=42):
+                 seed=42,
+                 **base_kwargs):
         # This looks really stupid, but if the default value is initiated in the method head, not in the call to the
         # super constructor as blow, python will only instantiate one object for all calls to this method, hence
         # causing different paradigms to share the same instances of prediction model or evaluation method.
         # For more information see:
         # https://florimond.dev/en/posts/2018/08/python-mutable-defaults-are-the-source-of-all-evil/
         super().__init__(
             prediction_model=ContrastiveKerasPredictionModel() if prediction_model is None else prediction_model,
-            name=name,
-            output_dir=output_dir,
             evaluation_methods=
             [IdentificationOnly()] if evaluation_methods is None else evaluation_methods,
-            verbose=verbose, seed=seed)
+            seed=seed, **base_kwargs)
 
     def restore_prediction_model_trainables(self,
                                             saved_weights_path_like: str,
                                             dataset: Dataset) -> PredictionModelBase:
         if dataset is None:
             raise ValueError(
                 "The dataset argument may not be None, as the method uses it to infer the size of the " +
```

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/_equal_error_thresholding_method.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/_equal_error_thresholding_method.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,39 +18,46 @@
                  pair_function: Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]],
                  output_dir: str):
         self.distance_metric = distance_metric
         self.pair_function = pair_function
         self.output_dir = output_dir
 
     def compute_threshold(self, enrollment_data: np.ndarray, enrollment_labels: np.ndarray) -> float:
-        pairs_test, same_user_in_pair = self.pair_function(enrollment_data,
-                                                           enrollment_labels)
+        pairs_test, distances_in_pairs = self.pair_function(enrollment_data,
+                                                            enrollment_labels)
 
         # split test pairs
-        x_test_1 = pairs_test[:, 0]  # x_test_1.shape = (20000, 28, 28)
+        x_test_1 = pairs_test[:, 0]
         x_test_2 = pairs_test[:, 1]
 
         raw_distance_predictions = self.distance_metric.predict(x_test_1, x_test_2)
         raw_distance_predictions = np.squeeze(raw_distance_predictions)
 
+        accept_reject_in_pairs = (distances_in_pairs * -1) + 1
+        accept_reject_predictions = (raw_distance_predictions * -1) + 1
+
         fpr, tpr, threshold_roc, precision, recall, threshold_prc = \
-            plot_roc_curve(same_user_in_pair, raw_distance_predictions, self.output_dir)
+            plot_roc_curve(accept_reject_in_pairs, accept_reject_predictions, self.output_dir)
 
         fnr = 1 - tpr
         eer_threshold = threshold_roc[np.nanargmin(np.absolute((fnr - fpr)))]
 
         # rates closest to the equal error rate among all possible thresholds
         eer_1 = fpr[np.nanargmin(np.absolute((fnr - fpr)))]
         eer_2 = fnr[np.nanargmin(np.absolute((fnr - fpr)))]
 
         roc_curve_dict = {'distance threshold': threshold_roc, 'false positive rate': fpr, 'true positive rate': tpr}
         prc_curve_dict = {'distance threshold': threshold_prc, 'precision': precision, 'recall': recall}
-        raw_dict = {'raw distance predicted': raw_distance_predictions, 'same user in input pair': same_user_in_pair}
+        raw_dict = {'raw distance predicted': raw_distance_predictions,
+                    'same user in input pair': accept_reject_in_pairs}
 
         pd.DataFrame(roc_curve_dict).to_csv(os.path.join(self.output_dir, 'roc_curve_table.csv'))
         pd.DataFrame(prc_curve_dict).to_csv(os.path.join(self.output_dir, 'prc_curve_table.csv'))
         pd.DataFrame(raw_dict).to_csv(os.path.join(self.output_dir, 'raw_predictions.csv'))
 
+        result = (eer_threshold * -1) + 1  # the result eer_threshold needs to be re-transformed into a distance, just
+        # like the raw_distance_predictions were transformed into accept_reject_predictions earlier
+
         with open(os.path.join(self.output_dir, 'equal_error_rate.txt'), 'w') as f:
-            f.write(f'Equal Error Rate candidates: \n{eer_1}\n{eer_2}\n\nEqual Error Rate distance: \n{eer_threshold}')
+            f.write(f'Equal Error Rate candidates: \n{eer_1}\n{eer_2}\n\nEqual Error Rate distance: \n{result}')
 
-        return eer_threshold
+        return result
```

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/distance_evaluation_method_base.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/distance_evaluation_method_base.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/evaluation_methods/pairwise_accuracy_eval.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/evaluation_methods/pairwise_accuracy_eval.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_keras_prediction_model.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_keras_prediction_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 import time
 from typing import Callable, Tuple
 
 import numpy as np
 import tensorflow.keras as keras
 
-from ..distance_prediction_model_base import DistanceBasePredictionModel
 from .contrastive_model_description import tower_mlp, merge_constractive
+from ..distance_prediction_model_base import DistanceBasePredictionModel
 from .....util.dataset import Dataset
 from .....util.plotting import plot_history_df
 from .....util.utils import contrastive_make_pairs
 
 
 class ContrastiveKerasPredictionModel(DistanceBasePredictionModel):
 
     def __init__(self,
                  tower_model_description: Callable[[keras.layers.Input], keras.models.Model]
                  = tower_mlp,
                  merge_model_description: Callable[[keras.models.Model, keras.layers.Input,
                                                     keras.models.Model, keras.layers.Input],
-                                                    keras.models.Model]
+                                                   keras.models.Model]
                  = merge_constractive,
                  output_dir: str = "keras_pred_model_out",
                  verbose=False,
                  nb_epochs=10,
                  batch_size: Callable[[int], int] = 16,
                  pair_function: Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]] =
                  contrastive_make_pairs):
@@ -60,25 +60,29 @@
         tower_1 = self.tower_model_description(input_layer)
         tower_2 = self.tower_model_description(input_layer)
         input_1 = keras.layers.Input(input_shape)
         input_2 = keras.layers.Input(input_shape)
         merge = self.merge_model_description(tower_1, input_1, tower_2, input_2)
         model_checkpoint = keras.callbacks.ModelCheckpoint(
             filepath=os.path.join(self.output_dir, 'best_model.hdf5'),
-            monitor='loss',
+            monitor='val_loss',
             save_best_only=True,
             save_weights_only=True)
         self.callbacks = [model_checkpoint]
         return merge
 
     def fit(self, dataset: Dataset):
         pairs_train, labels_train = self.pair_function(dataset.trainset_data, dataset.trainset_labels)
+        # labels_train = (labels_train * -1) + 1  # the pair function gives the correct distances, however, for the
+        # contractive loss to work, pairs of the same class need to be labelled 1 and pairs of different classes need to
+        # be labelled 0. Hence, we need to switch this array around.
 
         # make validation pairs
         pairs_val, labels_val = self.pair_function(dataset.validationset_data, dataset.validationset_labels)
+        # labels_val = (labels_val * -1) + 1  # same as above
 
         # split trainig pairs
         x_train_1 = pairs_train[:, 0]
         x_train_2 = pairs_train[:, 1]
 
         # split validation pairs
         x_val_1 = pairs_val[:, 0]
@@ -115,8 +119,12 @@
         # Not using restore here to not build a new model
         self.model.load_weights(os.path.join(self.output_dir, 'best_model.hdf5'))
 
         keras.backend.clear_session()
 
     def predict(self, x_test_1, x_test_2):
         y_pred = self.model.predict([x_test_1, x_test_2])
+        y_pred = np.squeeze(y_pred)
+        y_pred = (y_pred * -1) + 1  # due to a quirk in the tfa implementation of the constractive loss, it actually
+        # trains the model to output one minus what it receives as true labels. This needs to be corrected for during
+        # prediction
         return y_pred
```

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_model_description.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_model_description.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/offline_triplet_keras_prediction_model.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/offline_triplet_keras_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triple_tower_model.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triple_tower_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.tower_2 = self.tower_model_description(self.input_layer)  # positive
         self.tower_3 = self.tower_model_description(self.input_layer)  # negative
 
         self.merge = TrippleTowerDistanceLayer()
 
         model_checkpoint = tf.keras.callbacks.ModelCheckpoint(
             filepath=os.path.join(self.output_dir, 'best_model.hdf5'),
-            monitor='loss',
+            monitor='val_loss',
             save_best_only=True,
             save_weights_only=True)
         self.callbacks = [model_checkpoint]
 
         self.compile(optimizer=tf.keras.optimizers.Adam(0.0001))
 
         self.margin = margin
```

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triplet_distance_layer.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triplet_distance_layer.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/online_triplet_keras_prediction_model.py` & `useckit-0.4.0/useckit/paradigms/distance_learning/prediction_models/online_triplet_loss/online_triplet_keras_prediction_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         self.persist_model_trainables('model_init.hdf5')
 
         batch_size = self.batch_size
 
         model_checkpoint = keras.callbacks.ModelCheckpoint(
             filepath=os.path.join(self.output_dir, 'best_model.hdf5'),
-            monitor='loss',
+            monitor='val_loss',
             save_best_only=True,
             save_weights_only=True)
         self.callbacks = [model_checkpoint]
 
         start_time = time.time()
         hist = self.model.fit(x=pairs_train, y=y_train, batch_size=batch_size, epochs=self.nb_epochs,
                               verbose=self.verbose, validation_data=tuple([pairs_val, y_val]),
```

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/evaluation_methods/identification.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/evaluation_methods/identification.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         self.dataset = dataset
         self.prediction_model = prediction_model
 
     def identify(self, samples: np.ndarray) -> int:
         x_train, x_val, y_train, y_val, y_true, input_shape, nb_classes = \
             self.prediction_model.convert_dataset_to_legacy_values(self.dataset)
         x_test = samples
-        y_pred = self.prediction_model.predict(x_test, y_true, x_train, y_train, y_val, return_df_metrics=False)
+        _, _, _, y_test = self.dataset.view_one_hot_encoded_labels()
+        y_pred = self.prediction_model.predict(x_test, y_true, x_train, y_train, y_test, return_df_metrics=False)
         return self.dataset.reverse_label_transform(y_pred)
 
 
 class IdentificationOnly(TSCBaseEvaluationMethod):
 
     def __init__(self, output_dir: str = "evaluation_identification"):
         super().__init__(output_dir)
```

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/evaluation_methods/legacy_identification.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/evaluation_methods/legacy_identification.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/classification_keras_prediction_model.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/classification_keras_prediction_model.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/inception.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/inception.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,13 +111,13 @@
                       metrics=['accuracy'])
 
         reduce_lr = keras.callbacks.ReduceLROnPlateau(monitor='loss', factor=0.5, patience=50,
                                                       min_lr=0.0001)
 
         file_path = os.path.join(self.output_dir, 'best_model.hdf5')
 
-        model_checkpoint = keras.callbacks.ModelCheckpoint(filepath=file_path, monitor='loss',
+        model_checkpoint = keras.callbacks.ModelCheckpoint(filepath=file_path, monitor='val_loss',
                                                            save_best_only=True)
 
         self.callbacks = [reduce_lr, model_checkpoint]
 
         return model
```

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/keras_model_descriptions.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/keras_model_descriptions.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/mcdcnn.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/mcdcnn.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/mcnn.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/mcnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     def __init__(self, nb_classes, verbose=False, nb_epochs=None, output_dir: str = "MCNN_model_out"):
         super().__init__(verbose=verbose, output_dir=output_dir)
         self.nb_classes = nb_classes
         self.nb_epochs = nb_epochs
         self.pool_factors = [2, 3, 5]  # used for hyperparameters grid search
         self.filter_sizes = [0.05, 0.1, 0.2]  # used for hyperparameters grid search
         self.y_pred = None
+        self.input_shapes = None
+        self.ma_base, self.ma_step, self.ma_num = 5, 6, 1
+        self.ds_base, self.ds_step, self.ds_num = 2, 1, 4
 
     def slice_data(self, data_x, data_y, slice_ratio):
         n = data_x.shape[0]
         length = data_x.shape[1]
         n_dim = data_x.shape[2]  # for MTS
         nb_classes = self.nb_classes
 
@@ -157,26 +160,21 @@
             temp_pool_size = int(int(conv_shape) / pool_factor)
             print(temp_pool_size)
             if temp_pool_size == pool_size:
                 return pool_factor
 
         raise Exception('Error on pool factor')
 
-    def train(self, x_train, y_train, x_test, y_test, y_true, pool_factor=None, filter_size=None, do_train=True):
+    def train(self, x_train, y_train, x_val, y_val, x_test, y_test, y_true, pool_factor=None, filter_size=None,
+              do_train=True):
         window_size = 0.2
         n_train_batch = 10
         n_epochs = 200 if self.nb_epochs is None else self.nb_epochs
         max_train_batch_size = 256
 
-        # print('Original train shape: ', x_train.shape)
-        # print('Original test shape: ', x_test.shape)
-
-        # split train into validation set with validation_size = 0.2 train_size 
-        x_train, y_train, x_val, y_val = self.split_train(x_train, y_train)
-
         ori_len = x_train.shape[1]  # original_length of time series
         slice_ratio = 0.9
 
         if do_train == True:
             kernel_size = int(ori_len * filter_size)
 
         if do_train == False:
@@ -221,19 +219,20 @@
         test_num_batch = int(test_num / increase_num)
 
         length_train = train_set_x.shape[1]  # length after slicing.
 
         window_size = int(length_train * window_size) if window_size < 1 else int(window_size)
 
         # *******set up the ma and ds********#
-        ma_base, ma_step, ma_num = 5, 6, 1
-        ds_base, ds_step, ds_num = 2, 1, 4
+        ma_base, ma_step, ma_num = self.ma_base, self.ma_step, self.ma_num
+        ds_base, ds_step, ds_num = self.ds_base, self.ds_step, self.ds_num
 
         ds_num_max = length_train / (pool_factor * window_size)
         ds_num = int(min(ds_num, ds_num_max))
+        self.ds_num = ds_num
 
         # *******set up the ma and ds********#
 
         (ma_train, ma_valid, ma_test, ma_lengths) = self.batch_movingavrg(train_set_x,
                                                                           valid_set_x, test_set_x,
                                                                           ma_base, ma_step, ma_num)
         (ds_train, ds_valid, ds_test, ds_lengths) = self.batch_downsample(train_set_x,
@@ -274,14 +273,15 @@
 
         ######################
         # BUILD ACTUAL MODEL #
         ######################
         # print('building the model...')
 
         input_shapes, max_length = self.get_list_of_input_shapes(data_lengths, num_dim)
+        self.input_shapes = input_shapes
 
         start_time = time.time()
 
         best_validation_loss = np.inf
 
         if do_train == True:
 
@@ -490,42 +490,54 @@
         max_length = 0
         for i in data_lengths:
             input_shapes.append((i, num_dim))
             max_length = max(max_length, i)
         return input_shapes, max_length
 
     def fit(self, dataset: Dataset, *args, **kwargs):
-        x_train, x_val, y_train, y_val, y_true, input_shape, nb_classes = self.convert_dataset_to_legacy_values(dataset)
+        x_train, x_val, y_train, y_val, _, input_shape, nb_classes = self.convert_dataset_to_legacy_values(dataset)
+        x_test = dataset.testset_matching_data
+        _, _, _, y_test = dataset.view_one_hot_encoded_labels()
+        y_true = dataset.testset_matching_labels
 
         best_df_metrics = None
         best_valid_loss = np.inf
 
         output_directory_root = self.output_dir
         # grid search 
         for pool_factor in self.pool_factors:
             for filter_size in self.filter_sizes:
                 self.output_directory = os.path.join(output_directory_root,
                                                      'hyper_param_search',
                                                      'pool_factor_' + str(pool_factor),
                                                      'filter_size_' + str(filter_size))
                 create_directory(self.output_directory)
                 df_metrics, model, valid_loss = self.train(x_train, y_train, x_val,
-                                                           y_val, y_true, pool_factor, filter_size)
+                                                           y_val, x_test, y_test, y_true, pool_factor, filter_size)
 
                 if (valid_loss < best_valid_loss):
                     best_valid_loss = valid_loss
                     best_df_metrics = df_metrics
                     best_df_metrics.to_csv(os.path.join(output_directory_root, 'df_metrics.csv'), index=False)
                     model.save(os.path.join(output_directory_root, 'best_model.hdf5'))
 
                 model = None
                 # clear memeory 
                 keras.backend.clear_session()
 
-    def predict(self, x_test, y_true, x_train, y_train, y_test, return_df_metrics=True):
+    def predict(self, x_test, y_true, x_train, y_train, y_test, return_df_metrics=False):
         if return_df_metrics:
-            df_metrics, _, _ = self.train(x_train, y_train, x_test, y_test, y_true, do_train=False)
-            return df_metrics
+            raise NotImplementedError('returning df_metrics is not supported for MCNN prediction models!')
         else:
-            assert self.y_pred is not None, 'dl4tsc_mcnn was called for prediction before training. ' \
-                                            'self.y_pred is None!'
-            return self.y_pred
+            model = keras.models.load_model(os.path.join(self.output_directory, 'best_model.hdf5'))
+            (ma_test, ma_lengths) = self.movingavrg(x_test, self.ma_base, self.ma_step, self.ma_num)
+            (ds_test, ds_lengths) = self.downsample(x_test, self.ds_base, self.ds_step, self.ds_num)
+            if ds_lengths != []:
+                x_test = np.concatenate([x_test, ds_test], axis=1)
+
+            # moving average part
+            if ma_lengths != []:
+                x_test = np.concatenate([x_test, ma_test], axis=1)
+
+            y_pred = model.predict_on_batch(self.split_input_for_model(x_test, self.input_shapes))
+            y_pred = np.argmax(y_pred, axis=1)
+            return y_pred
```

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/tlenet.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/tlenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         model = keras.models.Model(inputs=input_layer, outputs=output_layer)
 
         model.compile(optimizer=keras.optimizers.legacy.Adam(learning_rate=0.01, decay=0.005),
                       loss='categorical_crossentropy', metrics=['accuracy'])
 
         file_path = os.path.join(self.output_dir, 'best_model.hdf5')
 
-        model_checkpoint = keras.callbacks.ModelCheckpoint(filepath=file_path, monitor='loss',
+        model_checkpoint = keras.callbacks.ModelCheckpoint(filepath=file_path, monitor='val_loss',
                                                            save_best_only=True)
 
         self.callbacks = [model_checkpoint]
 
         return model
 
     def pre_processing(self, x_train, y_train, x_test, y_test):
```

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/tsc_prediction_model_base.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/tsc_prediction_model_base.py`

 * *Files identical despite different names*

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/prediction_models/twiesn.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/prediction_models/twiesn.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,26 +187,24 @@
         # save the metrics
         df_metrics.to_csv(os.path.join(self.output_dir, 'df_metrics.csv'), index=False)
 
         # return the training accuracy and the prediction metrics on the test set
         return df_metrics, train_acc, ridge_classifier
 
     def fit(self, dataset: Dataset, *args, **kwargs):
-        x_train, x_val, y_train, y_val, y_true, input_shape, nb_classes = self.convert_dataset_to_legacy_values(dataset)
+        self.x_train, self.x_val, self.y_train, self.y_val, y_true, input_shape, nb_classes = self.convert_dataset_to_legacy_values(dataset)
 
         best_train_acc = -1
 
-        self.num_dim = x_train.shape[2]
-        self.T = x_train.shape[1]
-        self.x_test = x_val
+        self.num_dim = self.x_train.shape[2]
+        self.T = self.x_train.shape[1]
+        self.x_test = self.x_val
         self.y_true = y_true
-        self.y_test = y_val
+        self.y_test = self.y_val
 
-        # split train to validation set to choose best hyper parameters
-        self.x_train, self.x_val, self.y_train, self.y_val = train_test_split(x_train, y_train, test_size=0.2)
         self.N = self.x_train.shape[0]
 
         # limit the hyperparameter search if dataset is too big
         if self.x_train.shape[0] > 1000 or self.x_test.shape[0] > 1000:
             for config in self.configs:
                 config['N_x'] = 100
             self.configs = [self.configs[0], self.configs[1], self.configs[2]]
@@ -269,10 +267,10 @@
                                                                             self.num_dim + self.N_x)
         # memory free
         state_matrix = None
         gc.collect()
         # get the prediction on the test set
         y_pred = ridge_classifier.predict(new_x_test)
         # reconstruct the test predictions
-        y_pred_reshaped = self.reshape_prediction(y_pred, self.x_test.shape[0], self.T)
+        y_pred_reshaped = self.reshape_prediction(y_pred, x_test.shape[0], self.T)
 
         return y_pred_reshaped
```

### Comparing `useckit-0.3.3/useckit/paradigms/time_series_classification/tsc_paradigm.py` & `useckit-0.4.0/useckit/paradigms/time_series_classification/tsc_paradigm.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,37 +4,34 @@
 from .prediction_models.tsc_prediction_model_base import TSCBasePredictionModel
 from .._paradigm_base import ParadigmBase, PredictionModelBase
 from ...util.dataset import Dataset
 
 
 class TSCParadigm(ParadigmBase):
 
-    def __init__(self, name: str = None,
-                 output_dir: str = None,
+    def __init__(self,
                  prediction_model: TSCBasePredictionModel = None,
                  evaluation_methods: [TSCBaseEvaluationMethod] = None,
                  seed=42,
-                 verbose=True,
                  disable_normalization_check=False,
-                 class_weights=None
+                 class_weights=None,
+                 **base_kwargs
                  ):
         # This looks really stupid, but if the default value is initiated in the method head, not in the call to the
         # super constructor as blow, python will only instantiate one object for all calls to this method, hence
         # causing different paradigms to share the same instances of prediction model or evaluation method.
         # For more information see:
         # https://florimond.dev/en/posts/2018/08/python-mutable-defaults-are-the-source-of-all-evil/
         super().__init__(
             prediction_model=ClassificationKerasPredictionModel() if prediction_model is None else prediction_model,
-            name=name, output_dir=output_dir,
             evaluation_methods=
             [IdentificationOnly()] if evaluation_methods is None else evaluation_methods,
             seed=seed,
-            verbose=verbose)
+            **base_kwargs)
         self.disable_normalization_check = disable_normalization_check
-        self.seed = seed
         self.prediction_model = prediction_model
 
         if class_weights is not None:
             assert isinstance(class_weights, dict), 'class_weights must be a dict. See: https://bit.ly/3ljOI9c'
         self.class_weights = class_weights
 
     def restore_prediction_model_trainables(self,
```

### Comparing `useckit-0.3.3/useckit/tests/test_models.py` & `useckit-0.4.0/useckit/tests/test_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 import os
 import sys
 import unittest
 
 from useckit.paradigms.anomaly_detection.anomaly_paradigm import AnomalyParadigm
+from useckit.paradigms.anomaly_detection.prediction_models.scikit_anomaly_prediction_model import \
+    ScikitAnomalyPredictionModel
 from useckit.paradigms.distance_learning.distance_paradigm import DistanceMetricParadigm
+from useckit.paradigms.distance_learning.prediction_models.offline_triplet_loss.offline_triplet_keras_prediction_model import \
+    TripletKerasPredictionModel
 from useckit.paradigms.distance_learning.prediction_models.online_triplet_loss.online_triplet_keras_prediction_model import \
     OnlineTripletKerasPredictionModel
+from useckit.paradigms.distance_learning.prediction_models.scikit_distance_model import ScikitDistancePredictionModel
 from useckit.paradigms.time_series_classification.prediction_models.classification_keras_prediction_model import \
     ClassificationKerasPredictionModel
+from useckit.paradigms.time_series_classification.prediction_models.classification_scikit_prediction_model import \
+    ClassificationScikitPredictionModel
+from useckit.paradigms.time_series_classification.prediction_models.classification_xgboost_prediction_model import \
+    ClassificationXGBoostPredictionModel
 from useckit.paradigms.time_series_classification.prediction_models.inception import dl4tsc_inception
 from useckit.paradigms.time_series_classification.prediction_models.keras_model_descriptions import *
 from useckit.paradigms.time_series_classification.prediction_models.mcdcnn import dl4tsc_mcdcnn
 from useckit.paradigms.time_series_classification.prediction_models.mcnn import dl4tsc_mcnn
 from useckit.paradigms.time_series_classification.prediction_models.tlenet import dl4tsc_tlenet
 from useckit.paradigms.time_series_classification.prediction_models.twiesn import dl4tsc_twiesn
 from useckit.paradigms.time_series_classification.tsc_paradigm import TSCParadigm
 from useckit.tests.test_utils import make_some_intelligent_noise
 from useckit.util.dataset import Dataset
 from useckit.util.utils import triplet_make_pairs_random
-from useckit.paradigms.distance_learning.prediction_models.offline_triplet_loss.offline_triplet_keras_prediction_model import \
-    TripletKerasPredictionModel
 
 # resolves issues with gitlab runner
 sys.setrecursionlimit(10000)
 # disable gpu training for unittests
 os.environ['CUDA_VISIBLE_DEVICES'] = '-1'
 
 
 class TestUseckit(unittest.TestCase):
     @classmethod
     def setUpClass(self):
-        x_train, y_train = make_some_intelligent_noise()
-        x_val, y_val = make_some_intelligent_noise()
-        x_enroll, y_enroll = make_some_intelligent_noise()
-        x_test, y_test = make_some_intelligent_noise()
+        x_train, y_train = make_some_intelligent_noise(shape=(100, 100, 100))
+        x_val, y_val = make_some_intelligent_noise(shape=(110, 100, 100))
+        x_enroll, y_enroll = make_some_intelligent_noise(shape=(120, 100, 100))
+        x_test, y_test = make_some_intelligent_noise(shape=(130, 100, 100))
         self.data = Dataset(x_train, y_train, x_val, y_val, x_enroll, y_enroll, x_test, y_test)
 
     def test_tsc_mlp(self):
         keras_mlp = TSCParadigm(
             prediction_model=ClassificationKerasPredictionModel(verbose=True, nb_epochs=2,
                                                                 model_description=dl4tsc_mlp),
             verbose=True)
@@ -104,25 +111,60 @@
 
     def test_tsc_mcdcnn(self):
         mcdcnn = TSCParadigm(
             prediction_model=dl4tsc_mcdcnn(verbose=True, nb_epochs=2),
             verbose=True)
         mcdcnn.evaluate(self.data)
 
+    def test_tsc_scikit_classifier(self):
+        scikit_classifier = TSCParadigm(
+            prediction_model=ClassificationScikitPredictionModel(),
+            verbose=True)
+        scikit_classifier.evaluate(self.data)
+
+    def test_tsc_xgboost_classifier(self):
+        xgb_classifier = TSCParadigm(
+            prediction_model=ClassificationXGBoostPredictionModel(),
+            verbose=True)
+        xgb_classifier.evaluate(self.data)
+
     def test_siamese_contrastive_loss(self):
         from useckit.paradigms.distance_learning.prediction_models.contrastive_loss.contrastive_keras_prediction_model \
             import ContrastiveKerasPredictionModel
+        from useckit.paradigms.distance_learning.evaluation_methods.identification import \
+            IdentificationOnly as DistanceIdentification
+        from useckit.paradigms.distance_learning.evaluation_methods.identification_with_reject import \
+            IdentificationWithReject as DistanceIdentificationWithReject
+        from useckit.paradigms.distance_learning.evaluation_methods.verification import \
+            Verification as DistanceVerification
+
         x_train, y_train = make_some_intelligent_noise(shape=(20, 64, 64, 4))
         x_val, y_val = make_some_intelligent_noise(shape=(20, 64, 64, 4))
         x_enroll, y_enroll = make_some_intelligent_noise(shape=(20, 64, 64, 4))
         x_test, y_test = make_some_intelligent_noise(shape=(20, 64, 64, 4))
-        self.data = Dataset(x_train, y_train, x_val, y_val, x_enroll, y_enroll, x_test, y_test)
+        data = Dataset(x_train, y_train, x_val, y_val, x_enroll, y_enroll, x_test, y_test)
 
-        dmp = DistanceMetricParadigm(prediction_model=ContrastiveKerasPredictionModel(nb_epochs=2), verbose=True)
-        dmp.evaluate(self.data)
+        dmp = DistanceMetricParadigm(prediction_model=ContrastiveKerasPredictionModel(nb_epochs=2), verbose=True,
+                                     evaluation_methods=[
+                                         DistanceVerification(tradeoff_computation_speed_for_memory=False),
+                                         DistanceIdentification(tradeoff_computation_speed_for_memory=False),
+                                         DistanceIdentificationWithReject(
+                                             tradeoff_computation_speed_for_memory=False),
+                                         DistanceVerification(tradeoff_computation_speed_for_memory=True),
+                                         DistanceIdentification(tradeoff_computation_speed_for_memory=True),
+                                         DistanceIdentificationWithReject(
+                                             tradeoff_computation_speed_for_memory=True)
+                                     ])
+        dmp.evaluate(data)
+
+    def test_distance_scikit_regressor(self):
+        scikit_regressor = DistanceMetricParadigm(
+            prediction_model=ScikitDistancePredictionModel(),
+            verbose=True)
+        scikit_regressor.evaluate(self.data)
 
     def test_siamese_triplet_loss_offline(self):
         shape = (100, 200, 12)
         x_train, y_train = make_some_intelligent_noise(shape=shape)
         x_val, y_val = make_some_intelligent_noise(shape=shape)
         x_enroll, y_enroll = make_some_intelligent_noise(shape=shape)
         x_test, y_test = make_some_intelligent_noise(shape=shape)
@@ -135,23 +177,35 @@
 
         dmp.evaluate(data)
 
     def test_siamese_triplet_loss_online(self):
         shape = (100, 200, 12)
         x_train, y_train = make_some_intelligent_noise(shape=shape)
         x_val, y_val = make_some_intelligent_noise(shape=shape)
+        x_enroll, y_enroll = make_some_intelligent_noise(shape=shape)
         x_test, y_test = make_some_intelligent_noise(shape=shape)
-        data = Dataset(x_train, y_train, x_val, y_val, x_test, y_test)
+        data = Dataset(x_train, y_train, x_val, y_val, x_enroll, y_enroll, x_test, y_test)
 
         dmp = DistanceMetricParadigm(verbose=True,
                                      prediction_model=OnlineTripletKerasPredictionModel(verbose=True))
         dmp.evaluate(data)
 
     def test_encoders(self):
         from useckit.paradigms.anomaly_detection.prediction_models.auto_encoder_keras_prediction_model import \
             AutoEncoderKerasPredictionModel
+        x_train, y_train = make_some_intelligent_noise(shape=(20, 10, 10, 10))
+        x_val, y_val = make_some_intelligent_noise(shape=(20, 10, 10, 10))
+        x_enroll, y_enroll = make_some_intelligent_noise(shape=(20, 10, 10, 10))
+        x_test, y_test = make_some_intelligent_noise(shape=(20, 10, 10, 10))
+        data = Dataset(x_train, y_train, x_val, y_val, x_enroll, y_enroll, x_test, y_test)
         encoder = AnomalyParadigm(prediction_model=AutoEncoderKerasPredictionModel(nb_epochs=2), verbose=True)
-        encoder.evaluate(self.data)
+        encoder.evaluate(data)
+
+    def test_anomaly_scikit_regressor(self):
+        scikit_regressor = AnomalyParadigm(
+            prediction_model=ScikitAnomalyPredictionModel(),
+            verbose=True)
+        scikit_regressor.evaluate(self.data)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `useckit-0.3.3/useckit/util/dataset.py` & `useckit-0.4.0/useckit/util/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,28 +54,28 @@
     def _setup_missing_sets(self):
         if self.validationset_data is None:
             if self.testset_enrollment_data is None:
                 raise ValueError(f"Critical: a validation set needs to be present.")
             else:
                 self.validationset_data = self.testset_enrollment_data
                 self.validationset_labels = self.testset_enrollment_labels
-                print(f"useckit warning: because the validation set is None, the supplied testset enrollment data will "
+                print(f"Warning: because the validation set is None, the supplied testset enrollment data will "
                       f"be used instead.", file=sys.stderr)
         if self.testset_enrollment_data is None:
             if self.testset_matching_data is None:
-                print(f"useckit warning: testset enrollment and matching data are None. This will cause all evaluation "
+                print(f"Warning: testset enrollment and matching data are None. This will cause all evaluation "
                       f"methods to fail.", file=sys.stderr)
             else:
                 self.testset_enrollment_data = self.testset_matching_data
                 self.testset_enrollment_labels = self.testset_matching_labels
-                print(f"useckit warning: because the enrollment testset is None, the matching testset will be used "
+                print(f"Warning: because the enrollment testset is None, the matching testset will be used "
                       f"instead.", file=sys.stderr)
         else:
             if self.testset_matching_data is None:
-                print(f"useckit warning: testset matching data is None. This will cause all evaluation "
+                print(f"Warning: testset matching data is None. This will cause all evaluation "
                       f"methods to fail.", file=sys.stderr)
 
     def _setup_reject_label(self):
         self.reject_label = 'reject'  # In some cases this will be changed further down in the method
         if self.testset_matching_labels is not None:
             try:
                 match_label_set = set(self.testset_matching_labels)
@@ -96,33 +96,40 @@
 
         return convert_to_onehot(self.trainset_labels), convert_to_onehot(self.validationset_labels), \
                convert_to_onehot(self.testset_enrollment_labels), convert_to_onehot(self.testset_matching_labels)
 
     @staticmethod
     def _check_and_convert_type_data(obj, name) -> np.array:
         """Check the types of objects, print warnings and perform conversions."""
-        return Dataset._check_and_convert_type(obj, name, float)
+        return Dataset._check_and_convert_type(obj, name, 'float16')
 
     @staticmethod
     def _check_and_convert_type_label(obj, name) -> np.array:
         """Check the types of objects, print warnings and perform conversions."""
-        return Dataset._check_and_convert_type(obj, name, str)
+        result = Dataset._check_and_convert_type(obj, name, str)
+        if result is not None and len(result.shape) != 1:
+            raise ValueError("Critical: label arrays must be one-dimensional.")
+        return result
 
     @staticmethod
     def _check_and_convert_type(obj, name, dtype):
         if obj is None:
             return None
 
         if not isinstance(obj, np.ndarray):
             print(f"Warning: provided object {name} is of type {str(type(obj))} (expected: np.ndarray). "
                   f"Attempting a cast to np.ndarray.", file=sys.stderr)
-            arr = np.array(obj, dtype=dtype)
-            return arr
+            result = np.array(obj, dtype=dtype)  # this fails if dtype is float and the resulting array would be ragged
+        elif obj.dtype != dtype:
+            print(f"Warning: provided object {name} contains values of type {obj.dtype} (expected: {dtype}). "
+                  f"Attempting a cast to expected datatype!", file=sys.stderr)
+            result = obj.astype(dtype=dtype, copy=False)
         else:
-            return obj
+            result = obj
+        return result
 
     def _check_data_pairs_provided(self):
         """Checks that if training data is provided also labels are provided. Raises exception if not."""
 
         # check for None
         if self.trainset_data is None or len(self.trainset_data) == 0:
             raise ValueError("Critical: trainset_data must not be None or empty.")
@@ -153,21 +160,17 @@
                     raise ValueError(f'Critical: provided array {name} contains NaN values!')
             except TypeError:
                 print(f'Warning: could not check if NaNs exist in array {name}, as its dtype is "{array.dtype}". '
                       f'A numerical dtype (e.g., int or float) is expected. This might lead to subsequent '
                       f'critical errors and wrong calculations.', file=sys.stderr)
 
         _check_nan(self.trainset_data, name="trainset_data")
-        _check_nan(self.trainset_labels, name="trainset_labels")
         _check_nan(self.testset_matching_data, name="testset_matching_data")
-        _check_nan(self.testset_matching_labels, name="testset_matching_labels")
         _check_nan(self.testset_enrollment_data, name="testset_enrollment_data")
-        _check_nan(self.testset_enrollment_labels, name="testset_enrollment_labels")
         _check_nan(self.validationset_data, name="validationset_data")
-        _check_nan(self.validationset_labels, name="validationset_labels")
 
     def _check_dataset_is_balanced(self):
         return True  # TODO implement
 
     def _normalisation_check(self):
         def _normalisation_check(array: ndarray):
             if array is not None:
```

### Comparing `useckit-0.3.3/useckit/util/plotting.py` & `useckit-0.4.0/useckit/util/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import Counter
 
 import keras.callbacks
 import matplotlib.pyplot as plt
 import numpy as np
 import sklearn.metrics as metrics
 
-from useckit.util.utils import serialize_classification_report
+from useckit.util.utils import legacy_serialize_classification_report
 
 
 def plot_roc_curve(labels_test, predictions, output_directory):
     fpr, tpr, threshold_roc = metrics.roc_curve(labels_test, predictions)
     roc_auc = metrics.auc(fpr, tpr)
 
     plt.title('Receiver Operating Characteristic')
@@ -24,30 +24,30 @@
     plt.tight_layout()
     plt.savefig(os.path.join(output_directory, "roc_curve.pdf"))
     plt.clf()
 
     precision, recall, threshold_prc = metrics.precision_recall_curve(labels_test, predictions)
     precision = np.array(precision[:-1])
     recall = np.array(recall[:-1])
-    f1 = precision * recall / (precision + recall)
+    f1 = 2 * precision * recall / (precision + recall)
     plt.title('Precision, Recall and F1-Score over Threshold')
     plt.plot(threshold_prc, precision)
     plt.plot(threshold_prc, recall)
     plt.plot(threshold_prc, f1)
     plt.xlabel("Threshold")
     plt.ylabel("Rate")
     plt.legend(['precision', 'recall', 'f1'], loc='lower left')
     plt.tight_layout()
     plt.savefig(os.path.join(output_directory, "precision_recall_curve.pdf"))
     plt.clf()
 
     return fpr, tpr, threshold_roc, precision, recall, threshold_prc
 
 
-def plot_history_df(history: keras.callbacks.History, path, name=''):
+def plot_history_df(history: keras.callbacks.History, output_dir, name=''):
     """Plots keras history."""
     import matplotlib.pyplot as plt
     import os
 
     # adapt type if keras-object is passed
     if isinstance(history, keras.callbacks.History):
         history = history.history
@@ -73,37 +73,37 @@
     epochs = range(len(training_acc))
 
     plt.ylim(0, 1)
     plt.plot(epochs, training_acc, 'tab:blue', label='Training acc')
     plt.plot(epochs, validation_acc, 'tab:orange', label='Validation acc')
     plt.title('Training and validation accuracy ' + name)
     plt.legend()
-    plt.savefig(os.path.join(os.path.dirname(path), 'history_acc.pdf'))
+    plt.savefig(os.path.join(output_dir, 'history_acc.pdf'))
     # plt.show()
     plt.close()
 
     plt.figure()
 
     plt.plot(epochs, loss, 'tab:green', label='Training loss')
     plt.plot(epochs, val_loss, 'tab:red', label='Validation loss')
     plt.title('Training and validation loss ' + name)
     plt.legend()
-    plt.savefig(os.path.join(os.path.dirname(path), 'history_loss.pdf'))
+    plt.savefig(os.path.join(output_dir, 'history_loss.pdf'))
     # plt.show()
     plt.close()
     return training_acc, validation_acc
 
 
 def plot_confusion_matrix(cm,
                           target_names,
                           path='',
                           title='Confusion Matrix',
                           cmap=None,
                           normalize=True,
-                          fname='confusion-matrix.pdf'):
+                          filename='confusion-matrix.pdf'):
     """
     given a sklearn confusion matrix (cm), make a nice plot
 
     Arguments
     ---------
     cm:           confusion matrix from sklearn.metrics.confusion_matrix
 
@@ -115,15 +115,15 @@
     cmap:         the gradient of the values displayed from matplotlib.pyplot.cm
                   see http://matplotlib.org/examples/color/colormaps_reference.html
                   plt.get_cmap('jet') or plt.cm.Blues
 
     normalize:    If False, plot the raw numbers
                   If True, plot the proportions
 
-    fname:        filename.
+    filename:        filename.
 
     Usage
     -----
     plot_confusion_matrix(cm           = cm,                  # confusion matrix created by
                                                               # sklearn.metrics.confusion_matrix
                           normalize    = True,                # show proportions
                           target_names = y_labels_vals,       # list of names of the classes
@@ -166,15 +166,15 @@
             plt.text(j, i, "{:,}".format(cm[i, j]),
                      horizontalalignment="center",
                      color="white" if cm[i, j] > thresh else "black")
 
     plt.tight_layout()
     plt.ylabel('True class')
     plt.xlabel('Predicted class\naccuracy={:0.4f}; misclass={:0.4f}'.format(accuracy, misclass))
-    plt.savefig(os.path.join(path, fname), bbox_inches='tight')
+    plt.savefig(os.path.join(path, filename), bbox_inches='tight')
     # plt.show()
     plt.close()
 
 
 def do_cm(x_val: np.ndarray,
           y_val: np.ndarray,
           model,  # : TSCBasePredictionModel should be the type hint, but that can lead to circular imports. However,
@@ -191,15 +191,15 @@
     assert x_val.shape[0] == y_val.shape[0]
 
     # Confusion Matrix and Classification Report
     y_pred = model.predict(x_val, y_val, x_val, y_val, y_val, return_df_metrics=False)
     y_val = np.argmax(y_val, axis=1)
     cm = confusion_matrix(y_val, y_pred)
 
-    serialize_classification_report(y_val, y_pred, output_dir)
+    legacy_serialize_classification_report(y_val, y_pred, output_dir)
     plot_confusion_matrix(cm, set(y_val), output_dir, normalize=False)
 
     assert perform_per_sample_majority_vote is False or \
            perform_majority_vote is False, 'perform_per_sample_majority_vote and _perform_majority_vote cannot both be active in do_cm()!'
 
     if perform_per_sample_majority_vote:
         cm_lst = np.zeros(np.array(cm).shape).tolist()
@@ -213,19 +213,19 @@
             assert len(ground_truth) == 1  # check that ground truth really exists only once for all slices
             ground_truth = ground_truth[0][0]  # determine ground truth label
 
             cm_lst[ground_truth][majority_vote_pred] += 1  # increment confusion matrix at correct cell
 
         plot_confusion_matrix(np.array(cm_lst), set(y_val),
                               path=output_dir,
-                              fname=f'confusion-matrix-per-sample-vote-normalized.pdf')
+                              filename=f'confusion-matrix-per-sample-vote-normalized.pdf')
         plot_confusion_matrix(np.array(cm_lst).astype(int), set(y_val),
                               normalize=False,
                               path=output_dir,
-                              fname=f'confusion-matrix-per-sample-vote-nonnormalized.pdf')
+                              filename=f'confusion-matrix-per-sample-vote-nonnormalized.pdf')
         with open(os.path.join(output_dir, "confusion-matrix-per-sample-vote-nonnormalized.txt"),
                   'w') as f:
             f.write(np.array2string(np.array(cm_lst).astype(int)))
 
     if perform_majority_vote:
         assert False, 'perform_majority_vote has been disabled.'
         reduced_cm = []
@@ -239,8 +239,8 @@
                 reduced_cm.append([0] * line_len)  # add zeros to fit the line length
                 reduced_cm[-1][np.argmax(line)] = 1  # find argmax of line and set it to '1'
         reduced_cm_arr = np.array(reduced_cm)  # create np array
         plot_confusion_matrix(reduced_cm_arr,
                               set(y_val),
                               path=output_dir,
                               normalize=False,
-                              fname='confusion-matrix-vote.pdf')
+                              filename='confusion-matrix-vote.pdf')
```

### Comparing `useckit-0.3.3/useckit.egg-info/PKG-INFO` & `useckit-0.4.0/useckit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useckit
-Version: 0.3.3
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://blindforreview.com
 Author: BlindForReview.com
 Author-email: mail@blindforreview.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `useckit-0.3.3/useckit.egg-info/SOURCES.txt` & `useckit-0.4.0/useckit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -23,25 +23,29 @@
 useckit/paradigms/anomaly_detection/evaluation_methods/identification_with_reject.py
 useckit/paradigms/anomaly_detection/evaluation_methods/legacy_identification_with_reject.py
 useckit/paradigms/anomaly_detection/evaluation_methods/verification.py
 useckit/paradigms/anomaly_detection/prediction_models/__init__.py
 useckit/paradigms/anomaly_detection/prediction_models/anomaly_prediction_model_base.py
 useckit/paradigms/anomaly_detection/prediction_models/auto_encoder_keras_prediction_model.py
 useckit/paradigms/anomaly_detection/prediction_models/keras_model_descriptions.py
+useckit/paradigms/anomaly_detection/prediction_models/scikit_anomaly_prediction_model.py
+useckit/paradigms/anomaly_detection/prediction_models/scikit_model_descriptions.py
 useckit/paradigms/distance_learning/__init__.py
 useckit/paradigms/distance_learning/distance_paradigm.py
 useckit/paradigms/distance_learning/evaluation_methods/__init__.py
 useckit/paradigms/distance_learning/evaluation_methods/_equal_error_thresholding_method.py
+useckit/paradigms/distance_learning/evaluation_methods/_sample_broadcasting.py
 useckit/paradigms/distance_learning/evaluation_methods/distance_evaluation_method_base.py
 useckit/paradigms/distance_learning/evaluation_methods/identification.py
 useckit/paradigms/distance_learning/evaluation_methods/identification_with_reject.py
 useckit/paradigms/distance_learning/evaluation_methods/pairwise_accuracy_eval.py
 useckit/paradigms/distance_learning/evaluation_methods/verification.py
 useckit/paradigms/distance_learning/prediction_models/__init__.py
 useckit/paradigms/distance_learning/prediction_models/distance_prediction_model_base.py
+useckit/paradigms/distance_learning/prediction_models/scikit_distance_model.py
 useckit/paradigms/distance_learning/prediction_models/contrastive_loss/__init__.py
 useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_keras_prediction_model.py
 useckit/paradigms/distance_learning/prediction_models/contrastive_loss/contrastive_model_description.py
 useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/__init__.py
 useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/offline_triplet_keras_prediction_model.py
 useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triple_tower_model.py
 useckit/paradigms/distance_learning/prediction_models/offline_triplet_loss/triplet_distance_layer.py
@@ -51,23 +55,27 @@
 useckit/paradigms/time_series_classification/tsc_paradigm.py
 useckit/paradigms/time_series_classification/evaluation_methods/__init__.py
 useckit/paradigms/time_series_classification/evaluation_methods/identification.py
 useckit/paradigms/time_series_classification/evaluation_methods/legacy_identification.py
 useckit/paradigms/time_series_classification/evaluation_methods/tsc_evaluation_method_base.py
 useckit/paradigms/time_series_classification/prediction_models/__init__.py
 useckit/paradigms/time_series_classification/prediction_models/classification_keras_prediction_model.py
+useckit/paradigms/time_series_classification/prediction_models/classification_scikit_prediction_model.py
+useckit/paradigms/time_series_classification/prediction_models/classification_xgboost_prediction_model.py
 useckit/paradigms/time_series_classification/prediction_models/inception.py
 useckit/paradigms/time_series_classification/prediction_models/keras_model_descriptions.py
 useckit/paradigms/time_series_classification/prediction_models/mcdcnn.py
 useckit/paradigms/time_series_classification/prediction_models/mcnn.py
 useckit/paradigms/time_series_classification/prediction_models/tlenet.py
 useckit/paradigms/time_series_classification/prediction_models/tsc_prediction_model_base.py
 useckit/paradigms/time_series_classification/prediction_models/twiesn.py
 useckit/tests/__init__.py
 useckit/tests/test_dataset.py
 useckit/tests/test_evaluations.py
+useckit/tests/test_model_save_load.py
 useckit/tests/test_models.py
 useckit/tests/test_utils.py
 useckit/util/__init__.py
 useckit/util/dataset.py
+useckit/util/dataset_windowsliced.py
 useckit/util/plotting.py
 useckit/util/utils.py
```

