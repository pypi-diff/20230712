# Comparing `tmp/TEST_TC-1.0.5.tar.gz` & `tmp/TEST_TC-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-1.0.5.tar", last modified: Wed Jul 12 09:02:47 2023, max compression
+gzip compressed data, was "TEST_TC-1.0.6.tar", last modified: Wed Jul 12 16:06:11 2023, max compression
```

## Comparing `TEST_TC-1.0.5.tar` & `TEST_TC-1.0.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.561674 TEST_TC-1.0.5/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.374551 TEST_TC-1.0.5/LIB_tc/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.412588 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1606 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      213 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/top_level.txt
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.418100 TEST_TC-1.0.5/LIB_tc/test_tc/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-12 09:02:25.000000 TEST_TC-1.0.5/LIB_tc/test_tc/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.437104 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5672 2023-07-10 11:05:00.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5282 2023-07-10 11:04:51.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/experiment_model.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7149 2023-07-12 09:00:07.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/hierarchical_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-07-10 11:07:26.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.442101 TEST_TC-1.0.5/LIB_tc/test_tc/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4306 2023-07-10 11:09:32.000000 TEST_TC-1.0.5/LIB_tc/test_tc/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.450101 TEST_TC-1.0.5/LIB_tc/test_tc/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7301 2023-07-10 11:10:43.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.462125 TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    23316 2023-07-12 08:57:29.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3746 2023-07-12 08:58:31.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.469127 TEST_TC-1.0.5/LIB_tc/test_tc/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.489640 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     8437 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/plotPrediction.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15062 2023-07-10 14:14:17.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14560 2023-07-10 14:14:17.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/visualization.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.511711 TEST_TC-1.0.5/LIB_tc/test_tc/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2125 2023-07-12 08:59:04.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-07-10 11:14:05.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6624 2023-07-10 11:14:29.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/experiment_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2038 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6293 2023-07-10 11:15:17.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/tele_logger.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-12 09:02:47.560675 TEST_TC-1.0.5/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.0.5/README.md
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1148 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-12 09:02:47.561674 TEST_TC-1.0.5/setup.cfg
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.557674 TEST_TC-1.0.5/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3411 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11110 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2688 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4438 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_experiment_job.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4045 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_experiment_models.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2086 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_experiment_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2977 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2116 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3089 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.392203 TEST_TC-1.0.6/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.246560 TEST_TC-1.0.6/LIB_tc/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.273665 TEST_TC-1.0.6/LIB_tc/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-12 16:06:11.000000 TEST_TC-1.0.6/LIB_tc/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1606 2023-07-12 16:06:11.000000 TEST_TC-1.0.6/LIB_tc/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-12 16:06:11.000000 TEST_TC-1.0.6/LIB_tc/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      213 2023-07-12 16:06:11.000000 TEST_TC-1.0.6/LIB_tc/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-12 16:06:11.000000 TEST_TC-1.0.6/LIB_tc/TEST_TC.egg-info/top_level.txt
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.276580 TEST_TC-1.0.6/LIB_tc/test_tc/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-12 15:52:05.000000 TEST_TC-1.0.6/LIB_tc/test_tc/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.296304 TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5672 2023-07-10 11:05:00.000000 TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6569 2023-07-12 15:50:29.000000 TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/experiment_model.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7149 2023-07-12 14:57:21.000000 TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/hierarchical_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15204 2023-07-12 15:50:42.000000 TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.302489 TEST_TC-1.0.6/LIB_tc/test_tc/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.6/LIB_tc/test_tc/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4306 2023-07-10 11:09:32.000000 TEST_TC-1.0.6/LIB_tc/test_tc/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.309395 TEST_TC-1.0.6/LIB_tc/test_tc/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.6/LIB_tc/test_tc/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7301 2023-07-10 11:10:43.000000 TEST_TC-1.0.6/LIB_tc/test_tc/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.319752 TEST_TC-1.0.6/LIB_tc/test_tc/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.6/LIB_tc/test_tc/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    23316 2023-07-12 14:57:21.000000 TEST_TC-1.0.6/LIB_tc/test_tc/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3730 2023-07-12 15:51:06.000000 TEST_TC-1.0.6/LIB_tc/test_tc/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.322939 TEST_TC-1.0.6/LIB_tc/test_tc/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.6/LIB_tc/test_tc/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.338294 TEST_TC-1.0.6/LIB_tc/test_tc/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.6/LIB_tc/test_tc/datavisualization/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     8437 2023-07-12 14:57:21.000000 TEST_TC-1.0.6/LIB_tc/test_tc/datavisualization/plotPrediction.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14626 2023-07-12 16:05:13.000000 TEST_TC-1.0.6/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-12 14:57:21.000000 TEST_TC-1.0.6/LIB_tc/test_tc/datavisualization/visualization.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.359831 TEST_TC-1.0.6/LIB_tc/test_tc/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.6/LIB_tc/test_tc/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2125 2023-07-12 14:57:21.000000 TEST_TC-1.0.6/LIB_tc/test_tc/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-07-10 11:14:05.000000 TEST_TC-1.0.6/LIB_tc/test_tc/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7128 2023-07-12 15:51:56.000000 TEST_TC-1.0.6/LIB_tc/test_tc/utility/experiment_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2038 2023-07-12 14:57:21.000000 TEST_TC-1.0.6/LIB_tc/test_tc/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6293 2023-07-10 11:15:17.000000 TEST_TC-1.0.6/LIB_tc/test_tc/utility/tele_logger.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-12 16:06:11.390203 TEST_TC-1.0.6/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.0.6/README.md
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1148 2023-07-10 10:31:23.000000 TEST_TC-1.0.6/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-12 16:06:11.392286 TEST_TC-1.0.6/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 16:06:11.386202 TEST_TC-1.0.6/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3411 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11110 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2688 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4438 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_experiment_job.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4045 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_experiment_models.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2086 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_experiment_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2977 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2116 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3089 2023-07-12 14:57:22.000000 TEST_TC-1.0.6/tests/test_tele_logger.py
```

### Comparing `TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-1.0.6/LIB_tc/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/algorithm.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/experiment_model.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/experiment_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,97 @@
-from typing import Any
+from typing import Any, Dict
 
 import pandas as pd
 from prophet import Prophet
 from typing_extensions import Self
-from copy import deepcopy
 
 from ..analytics.evaluationMetrics import evaluations
 from ..datapreparation.datapreparation_utils import logger
 from ..datapreparation.prep import PreprocessingClass
 from ..utility.experiment_utils import create_zero_dataframe
 from ..utility.constants import predict_dataframe_columns
 from .algorithm import Prophet_model, prophet_tuning
 from .prophet_utils import preprocess_prophet_input, preprocess_prophet_output
+from copy import deepcopy
 
 class ProphetExperiment:
     def __init__(self):
         pass
     
-    def fit(self, df_train_dict: dict, df_val_dict: dict, 
-            hyperparameters_grid: dict[str, Any], max_na_ratio: float = 0.5,) -> Self:
+    def fit(self, df_train_dict: Dict, df_val_dict: Dict, 
+            hyperparameters_grid: Dict[str, Any], max_na_ratio: float = 0.5,) -> Self:
         
         count = 0
-        self.models_dict: dict[str, Prophet_model] = {}
+        self.models_dict = {}
+        self.models_best_params = {}
+        self.max_na_ratio = max_na_ratio
+
         # Train and tune all models for all the possible levels in the hierarchy
         tmp_df_train_dict = deepcopy(df_train_dict)
         tmp_df_val_dict = deepcopy(df_val_dict)
+
         for id_pred in tmp_df_train_dict.keys():
             self.models_dict[id_pred] = None
+            self.models_best_params[id_pred] = {}
+
             logger.info(f"START training {id_pred}")
             prophet_train_df = preprocess_prophet_input(tmp_df_train_dict[id_pred], date = "Timestamp", target = "Target")
             prophet_val_df = preprocess_prophet_input(tmp_df_val_dict[id_pred], date = "Timestamp", target = "Target")
 
-            if prophet_train_df.isna().sum().sum() / len(prophet_train_df) >= max_na_ratio:
-                logger.info(f"The train set for time series {id_pred} has more than {max_na_ratio*100}% null values, skipping it.")
+            if (prophet_train_df['y'] > 0).sum() / len(prophet_train_df) < self.max_na_ratio:
+                logger.info(f"The train set for time series {id_pred} has more than {self.max_na_ratio*100}% null values, skipping it.")
                 count += 1
                 logger.info(f"Remaining number of iteration - {len(tmp_df_train_dict.keys())-count}")
                 continue
             try:
                 # Tune if we have a non-empty validation set
                 best_params = prophet_tuning(hyperparameters_grid, prophet_train_df, prophet_val_df)
                 Model = Prophet_model(best_params)
                 # Retrain on train and val data with best parameters
                 Model.fit(pd.concat([prophet_train_df, prophet_val_df]))
+
+                self.models_best_params[id_pred] = best_params
+                self.models_dict[id_pred] = Model
             except ValueError as e:
                 logger.info(f"Skipping training {id_pred}, due to: {e}")
                 count += 1
                 logger.info(f"Remaining number of iteration - {len(tmp_df_train_dict.keys())-count}")
                 continue
 
-            self.models_dict[id_pred] = Model
             logger.info(f"DONE training {id_pred}")
 
             count += 1
             logger.info(f"Remaining number of iteration - {len(tmp_df_train_dict.keys())-count}")
 
         return self
+    
+    def refit(self, df_dict : Dict):
+                
+        count = 0
+        # Train and tune all models for all the possible levels in the hierarchy
+        tmp_df_dict = deepcopy(df_dict)
+
+        for id_pred in tmp_df_dict.keys():
+            logger.info(f"START Re-Training {id_pred}")
+            prophet_df = preprocess_prophet_input(tmp_df_dict[id_pred], date = "Timestamp", target = "Target")
+
+            # If the models exists and have been trained, execute the retrain on the whole dataset
+            if isinstance(self.models_dict[id_pred], Prophet_model):
+                Model = Prophet_model(self.models_best_params[id_pred])
+                # Retrain on train and val data with best parameters
+                Model.fit(prophet_df)
+
+                self.models_dict[id_pred] = Model
+
+            logger.info(f"DONE Re-Training {id_pred}")
+
+            count += 1
+            logger.info(f"Remaining number of iteration - {len(tmp_df_dict.keys())-count}")
+
+        return self
 
     def create_hyperparameters_table(
         self, hyperparameters: dict[str, Any]) -> dict[str, Any]:
         def get_params_to_log(
             model: Prophet, hyperparameters: list[str]) -> dict[str, Any]:
             return {hyper: getattr(model, hyper) for hyper in hyperparameters}
 
@@ -94,14 +127,16 @@
 
         return pd.concat(predictions)
 
     def evaluate(self, df_test_dict: dict) -> pd.DataFrame: 
         metrics = []
         tmp_df_test_dict = deepcopy(df_test_dict)
         predictions = self.predict(df_test_dict)
+        
         for id_pred, df_test in tmp_df_test_dict.items():
             logger.info(f"START evaluating {id_pred}")           
             df_pred = predictions[predictions["Id_pred"] == id_pred]
-            metrics.append(evaluations(df_test, df_pred, date='Timestamp' , y_true='Target', y_pred='Pred_mean'))  
-
+            if df_pred.Pred_mean.sum() > 0:
+                metrics.append(evaluations(df_test, df_pred, date='Timestamp' , y_true='Target', y_pred='Pred_mean'))  
+        
         metrics = pd.concat(metrics).dropna()
         return metrics
```

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/hierarchical_utils.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/hierarchical_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/prophet_utils.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/algorithms/prophet_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,19 +182,19 @@
         raise ValueError("Il dataframe non contiene una colonna di tipo datetime")
 
     # Controllo se la colonna temporale è ordinata in modo monotono
     for col in datetime_columns:
         if not df[col].is_monotonic_increasing and not df[col].is_monotonic_decreasing:
             raise ValueError(f"La colonna '{col}' non è ordinata in modo monotono")
 
-    if not (0 <= val_size <= 1):
-        raise ValueError("val_size deve essere compreso tra 0 e 1")
+    if not (val_size > 0):
+        raise ValueError("val_size must be greater or equal than 1")
 
-    if test_size is not None and not (0 <= test_size <= 1):
-        raise ValueError("test_size deve essere compreso tra 0 e 1")
+    if test_size is not None and not (test_size > 0):
+        raise ValueError("test_size must be greater or equal than 1")
 
 def train_val_test_split(df: pd.DataFrame, val_size: float, test_size: float = None) -> tuple:
     """
     Create train, validation, test dataframes
 
     Parameters
     ----------
@@ -209,36 +209,24 @@
 
     Returns
     -------
         Tuple: (train_set, val_set, test_set)
     """
     # Parameters check
     check_split_input(df = df, val_size = val_size, test_size = test_size)
-    if test_size:
-        train_size = 1 - (val_size + test_size)
 
-    else: 
-        train_size = 1 - val_size
-
-    # Calcolo delle dimensioni dei subset
     total_rows = len(df)
-    train_rows = int(train_size * total_rows)
-    val_rows = int(val_size * total_rows)
 
-    if test_size:
-        # Effettua lo split dei dati
-        train_set = df[:train_rows]
-        val_set = df[train_rows:train_rows+val_rows]
-        test_set = df[train_rows+val_rows:]
-        return train_set, val_set, test_set
-    else:
-        train_set = df[:train_rows]
-        val_set = df[train_rows:train_rows+val_rows]
-        return train_set, val_set
+    # Effettua lo split dei dati
+    train_set = df.iloc[:-(val_size+test_size)]
+    val_set = df.iloc[(total_rows-val_size-test_size):(-1)*test_size]
+    test_set = df.iloc[(total_rows-test_size):]
 
+    return train_set, val_set, test_set
+    
 def preprocess_prophet_output(df: pd.DataFrame, id_pred: str) -> pd.DataFrame:
     """
     The function generates the results table from the Prophet table.
     The results table has columns (Timestamp, Id_pred, Pred_mean, Sigma, Pi_lower_95, Pi_upper_95)
 
     Parameters
     ----------
```

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/analytics/evaluationMetrics.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/datahandler/datahandler.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/datapreparation_utils.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/datapreparation/datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/prep.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/datapreparation/prep.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing_extensions import Self, Any
 import pandas as pd
 import pickle
 
 from ..utility.tele_logger import logger
 from ..utility.resources import *
-from .datapreparation.datapreparation_utils import ModelPreprocess
+from .datapreparation_utils import ModelPreprocess
 
 
 class PreprocessingClass(BaseEstimator, TransformerMixin):
 
     def __init__(self,
                  usecase: str,
                  model: str,
```

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/plotPrediction.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/datavisualization/plotPrediction.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import calendar
 import warnings
+
 import matplotlib.pyplot as plt
 import numpy as np
 from prophet import Prophet
 from prophet.plot import plot_components_plotly
 import pandas as pd
 import plotly
 import plotly.express as px
@@ -57,15 +58,15 @@
         # df = df.dropna()
 
         # Plot
         fig = px.line(
             self.df,
             x=self.data,
             y=self.target,
-            labels={self.data: "data", self.target: f"numero {self.use_case}"},
+            labels={self.data: "data", self.target: f"{self.target}"},
             title=f"Andamento {self.use_case} - {self.regione}",
             color_discrete_sequence=["blue"],
             width=800,
             height=500,
             template=dict(
                 layout=go.Layout(
                     title_font=dict(family="Rockwell", size=24, color="red"),
@@ -75,15 +76,15 @@
         )
 
         # Plot (mirror)
         fig_mirror = px.area(
             self.df,
             x=self.data,
             y=self.target,
-            labels={self.data: "data", self.target: f"numero {self.use_case}"},
+            labels={self.data: "data", self.target: f"{self.target}"},
             title=f"Andamento {self.use_case} - {self.regione} (mirror plot)",
             color_discrete_sequence=["green"],
             width=800,
             height=500,
             template=dict(
                 layout=go.Layout(
                     title_font=dict(family="Rockwell", size=24, color="red"),
@@ -258,32 +259,37 @@
             stazionarieta = "differenza stazionaria"
         res += f"Risultato dei test: {stazionarieta}"
         print(res)
 
         return res
 
     # Autocorrelation
-    def autocorrelation(self, n_lags: int = 50) -> tuple:
+    def autocorrelation(self, n_lags: int = 50, detrend: bool = True) -> tuple:
 
         """Plot that show autocorrelation of time series
 
         Parameters
         ----------
         n_lags : int
-            number of lags to compute autocorrelation and partial autocorrelation
+            number of lags to compute autocorrelation
+        detrend : bool
+            whether to detrend the time series before computing the autocorrelation. Default is True
 
         Returns
         -------
         tuple
-            tuple that containing figure for autocorrelation and partial autocorrelation
+            tuple that containing figure for autocorrelation
 
         """
 
-        trend = self.additive_decomposition()[0]
-        time_series = self.df[self.target] - trend
+        if detrend:
+            trend = self.additive_decomposition()[0]
+            time_series = self.df[self.target] - trend
+        else:
+            time_series = self.df[self.target]
 
         autocorr = acf(time_series.dropna(), nlags=n_lags)[1:]
         fig1 = px.bar(
             x=np.arange(autocorr.shape[0]) + 1,
             y=autocorr,
             labels={"x": "Lag", "y": "Autocorrelazione"},
             title="Autocorrelazione (detrendizzata)",
@@ -292,32 +298,14 @@
                     title_font=dict(family="Rockwell", size=24, color="red"),
                     font=dict(color="green"),
                 )
             ),
         )
         fig1.update_layout(showlegend=False)
 
-        # p_autocorr = pacf(time_series.dropna(), nlags=n_lags)[1:]
-        # fig2 = px.bar(
-        #     x=np.arange(p_autocorr.shape[0]) + 1,
-        #     y=p_autocorr,
-        #     labels={"x": "Lag", "y": "Autocorrelazione"},
-        #     title="Autocorrelazione parziale",
-        #     template=dict(
-        #         layout=go.Layout(
-        #             title_font=dict(family="Rockwell", size=24, color="red"),
-        #             font=dict(color="green"),
-        #         )
-        #     ),
-        # )
-        # fig2.update_layout(showlegend=False)
-
-        # fig1.show()
-        # fig2.show()
-
         return [fig1]
 
     # Decomposizione Additiva (Trend + Seasonality + Residual)
     def additive_decomposition(self) -> tuple:
 
         """Compute and plot additive decompostion
 
@@ -330,21 +318,24 @@
             result of additive decomposition (trend and seasonality)
         """
         df = self.df.dropna()
 
         df = pd.DataFrame({'ds': df[self.data], 'y': df[self.target]})
         m = Prophet()
         m.fit(df)
-        future_df = m.make_future_dataframe(periods=0)
         forecast = m.predict(df[["ds"]])
 
         fig = plot_components_plotly(m, forecast)
 
         forecast = forecast.set_index("ds")
-        return (forecast["trend"], forecast["weekly"], fig)
+        try:
+            weekly = forecast["weekly"]
+        except:
+            weekly = None
+        return (forecast["trend"], weekly, fig)
 
     def boxplots_seasons(self) -> plt.figure:
         
         """Creates a boxplot showing weekday-season effects
 
         Parameters
         ----------
```

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/visualization.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/datavisualization/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
             yaxis = dict(
                 tickmode = 'array',
                 tickvals = [i for i in range(len(lista))],
                 ticktext = [i[1] for i in lista],tickangle=-45,tickfont=dict(family='Rockwell', color='green', size=10)
             )           
         )
 
-        return (fig,distance_matrix_normalized)
+        return (fig,distance_matrix_normalized,lista)
 
     def plot_distance_matrix(self, distance_matrix: np.ndarray, lista: list[tuple]):
         
         dists = squareform(distance_matrix)
         linkage_matrix = linkage(dists, "ward",optimal_ordering=0)
         
         dendr = plt.figure(figsize=(10,6))
```

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/utility/constants.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/utility/constants.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/utility/exceptions.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/utility/experiment_utils.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/utility/experiment_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 import os
 import shutil
 
 from .constants import code_to_region_name, code_to_speciality
 from ..datapreparation.datapreparation_utils import logger
 
-from ...prophet_utils import train_val_test_split
+from ..algorithms.prophet_utils import train_val_test_split
 from ..datapreparation.prep import PreprocessingClass
 from ..datahandler.datahandler import DataHandler
 
 
 def add_mapped_columns(
     hierarchy: dict[str, str], df: pd.DataFrame, conversion: dict[str, str]
 ) -> tuple[pd.DataFrame, dict[str, str]]:
@@ -97,47 +97,54 @@
     Parameters
     ----------
     val_size : int
         The size of the validation set.
     test_size : int
         The size of the test set.
     """
-    if val_size < 0.1 or test_size < 0.1:
+    if val_size == 0 or test_size == 0:
         logger.info(
-            f"Be aware that either validation size {val_size} or test size {test_size} is less than 0.1"
+            f"Be aware that either validation size {val_size} or test size {test_size} is equal to 0"
         )
+    
+    if test_size >= val_size:
+         logger.error(f'Validation Set size MUST be greater than Test Size. Inputs given were: Validation Size -> {val_size} / Test Size -> {test_size}')
+         raise ValueError(f'Validation Set size MUST be greater than Test Size. Inputs given were: Validation Size -> {val_size} / Test Size -> {test_size}')
 
 
 def get_prophetexperiment_datasets(df: pd.DataFrame, dict_id_pred_queries: dict[str, str],
-                                   preprocessor: PreprocessingClass, time_granularity: str,
-                                   date_col: str) -> dict:
+                                   preprocessor: PreprocessingClass,
+                                   preprocessing_dict: dict
+                                #    , time_granularity: str,
+                                #    date_col: str
+                                   ) -> dict:
     """
     _summary_
 
     Parameters
     ----------
     df
         _description_
     dict_id_pred_queries
         _description_
     preprocessor
         _description_
-    time_granularity
+    preproc_details
         _description_
 
     Returns
     -------
         _description_
     """
     dict_preprocessed_df = {} 
     for id_pred, query in dict_id_pred_queries.items():
             filtered_df = df.query(query)
             filtered_df = filtered_df.reset_index(drop = True)
-            filtered_df = allign_dates(filtered_df, date_col, df)
-            full_df = preprocessor.fit_transform(filtered_df, time_granularity=time_granularity)
+            filtered_df = allign_dates(filtered_df, preprocessing_dict['date_col'], df)
+            full_df = preprocessor.fit_transform(filtered_df, **preprocessing_dict)
             dict_preprocessed_df[id_pred] = full_df
     return dict_preprocessed_df
 
 
 def split_prophetexperiment_datasets(dict_preprocessed_df: dict, val_size: float, test_size: float = None) -> dict:
     """
     _summary_
```

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/utility/resources.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/LIB_tc/test_tc/utility/tele_logger.py` & `TEST_TC-1.0.6/LIB_tc/test_tc/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/README.md` & `TEST_TC-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/pyproject.toml` & `TEST_TC-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_algorithm.py` & `TEST_TC-1.0.6/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_datahandler.py` & `TEST_TC-1.0.6/tests/test_datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_datapreparation_utils.py` & `TEST_TC-1.0.6/tests/test_datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_evaluations.py` & `TEST_TC-1.0.6/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_exceptions.py` & `TEST_TC-1.0.6/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_experiment_job.py` & `TEST_TC-1.0.6/tests/test_experiment_job.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_experiment_models.py` & `TEST_TC-1.0.6/tests/test_experiment_models.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_experiment_utils.py` & `TEST_TC-1.0.6/tests/test_experiment_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_prep.py` & `TEST_TC-1.0.6/tests/test_prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_prophet_utils.py` & `TEST_TC-1.0.6/tests/test_prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_resources.py` & `TEST_TC-1.0.6/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.5/tests/test_tele_logger.py` & `TEST_TC-1.0.6/tests/test_tele_logger.py`

 * *Files identical despite different names*

