# Comparing `tmp/TEST_TC-1.0.4.tar.gz` & `tmp/TEST_TC-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-1.0.4.tar", last modified: Mon Jul 10 11:15:43 2023, max compression
+gzip compressed data, was "TEST_TC-1.0.5.tar", last modified: Wed Jul 12 09:02:47 2023, max compression
```

## Comparing `TEST_TC-1.0.4.tar` & `TEST_TC-1.0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.905882 TEST_TC-1.0.4/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.803238 TEST_TC-1.0.4/LIB_tc/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.822995 TEST_TC-1.0.4/LIB_tc/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-10 11:15:43.000000 TEST_TC-1.0.4/LIB_tc/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1606 2023-07-10 11:15:43.000000 TEST_TC-1.0.4/LIB_tc/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-10 11:15:43.000000 TEST_TC-1.0.4/LIB_tc/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      213 2023-07-10 11:15:43.000000 TEST_TC-1.0.4/LIB_tc/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-10 11:15:43.000000 TEST_TC-1.0.4/LIB_tc/TEST_TC.egg-info/top_level.txt
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.824997 TEST_TC-1.0.4/LIB_tc/test_tc/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-10 11:10:59.000000 TEST_TC-1.0.4/LIB_tc/test_tc/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.834021 TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5672 2023-07-10 11:05:00.000000 TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5282 2023-07-10 11:04:51.000000 TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/experiment_model.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7149 2023-07-10 11:04:45.000000 TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/hierarchical_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-07-10 11:07:26.000000 TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.840082 TEST_TC-1.0.4/LIB_tc/test_tc/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.4/LIB_tc/test_tc/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4306 2023-07-10 11:09:32.000000 TEST_TC-1.0.4/LIB_tc/test_tc/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.843088 TEST_TC-1.0.4/LIB_tc/test_tc/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.4/LIB_tc/test_tc/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7301 2023-07-10 11:10:43.000000 TEST_TC-1.0.4/LIB_tc/test_tc/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.848083 TEST_TC-1.0.4/LIB_tc/test_tc/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.4/LIB_tc/test_tc/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11358 2023-07-10 11:10:40.000000 TEST_TC-1.0.4/LIB_tc/test_tc/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3679 2023-07-10 11:11:57.000000 TEST_TC-1.0.4/LIB_tc/test_tc/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.850082 TEST_TC-1.0.4/LIB_tc/test_tc/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.4/LIB_tc/test_tc/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.862231 TEST_TC-1.0.4/LIB_tc/test_tc/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.4/LIB_tc/test_tc/datavisualization/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     8228 2023-07-10 10:31:23.000000 TEST_TC-1.0.4/LIB_tc/test_tc/datavisualization/plotPrediction.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15046 2023-07-10 11:12:30.000000 TEST_TC-1.0.4/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14591 2023-07-10 10:36:42.000000 TEST_TC-1.0.4/LIB_tc/test_tc/datavisualization/visualization.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.876745 TEST_TC-1.0.4/LIB_tc/test_tc/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.4/LIB_tc/test_tc/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1616 2023-07-10 11:13:37.000000 TEST_TC-1.0.4/LIB_tc/test_tc/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-07-10 11:14:05.000000 TEST_TC-1.0.4/LIB_tc/test_tc/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6624 2023-07-10 11:14:29.000000 TEST_TC-1.0.4/LIB_tc/test_tc/utility/experiment_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2038 2023-07-10 11:15:04.000000 TEST_TC-1.0.4/LIB_tc/test_tc/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6293 2023-07-10 11:15:17.000000 TEST_TC-1.0.4/LIB_tc/test_tc/utility/tele_logger.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-10 11:15:43.903885 TEST_TC-1.0.4/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.0.4/README.md
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1148 2023-07-10 10:31:23.000000 TEST_TC-1.0.4/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-10 11:15:43.906616 TEST_TC-1.0.4/setup.cfg
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-10 11:15:43.900874 TEST_TC-1.0.4/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 17:28:54.000000 TEST_TC-1.0.4/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3411 2023-06-27 17:28:54.000000 TEST_TC-1.0.4/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11110 2023-07-04 08:52:34.000000 TEST_TC-1.0.4/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2688 2023-07-04 08:52:34.000000 TEST_TC-1.0.4/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 17:28:54.000000 TEST_TC-1.0.4/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4438 2023-07-04 08:52:34.000000 TEST_TC-1.0.4/tests/test_experiment_job.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4045 2023-07-04 08:52:34.000000 TEST_TC-1.0.4/tests/test_experiment_models.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2086 2023-07-04 08:52:34.000000 TEST_TC-1.0.4/tests/test_experiment_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2977 2023-07-04 08:52:34.000000 TEST_TC-1.0.4/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 17:28:54.000000 TEST_TC-1.0.4/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2116 2023-06-28 16:32:49.000000 TEST_TC-1.0.4/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3089 2023-06-27 17:28:54.000000 TEST_TC-1.0.4/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.561674 TEST_TC-1.0.5/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.374551 TEST_TC-1.0.5/LIB_tc/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.412588 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1606 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      213 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-12 09:02:47.000000 TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/top_level.txt
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.418100 TEST_TC-1.0.5/LIB_tc/test_tc/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-12 09:02:25.000000 TEST_TC-1.0.5/LIB_tc/test_tc/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.437104 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5672 2023-07-10 11:05:00.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5282 2023-07-10 11:04:51.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/experiment_model.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7149 2023-07-12 09:00:07.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/hierarchical_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-07-10 11:07:26.000000 TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.442101 TEST_TC-1.0.5/LIB_tc/test_tc/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4306 2023-07-10 11:09:32.000000 TEST_TC-1.0.5/LIB_tc/test_tc/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.450101 TEST_TC-1.0.5/LIB_tc/test_tc/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7301 2023-07-10 11:10:43.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.462125 TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    23316 2023-07-12 08:57:29.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3746 2023-07-12 08:58:31.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.469127 TEST_TC-1.0.5/LIB_tc/test_tc/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.489640 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     8437 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/plotPrediction.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15062 2023-07-10 14:14:17.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14560 2023-07-10 14:14:17.000000 TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/visualization.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.511711 TEST_TC-1.0.5/LIB_tc/test_tc/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2125 2023-07-12 08:59:04.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-07-10 11:14:05.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6624 2023-07-10 11:14:29.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/experiment_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2038 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6293 2023-07-10 11:15:17.000000 TEST_TC-1.0.5/LIB_tc/test_tc/utility/tele_logger.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-12 09:02:47.560675 TEST_TC-1.0.5/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.0.5/README.md
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1148 2023-07-10 10:31:23.000000 TEST_TC-1.0.5/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-12 09:02:47.561674 TEST_TC-1.0.5/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-12 09:02:47.557674 TEST_TC-1.0.5/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3411 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    11110 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2688 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4438 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_experiment_job.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4045 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_experiment_models.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2086 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_experiment_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2977 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2116 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3089 2023-07-12 08:55:54.000000 TEST_TC-1.0.5/tests/test_tele_logger.py
```

### Comparing `TEST_TC-1.0.4/LIB_tc/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-1.0.5/LIB_tc/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/algorithm.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/experiment_model.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/experiment_model.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/hierarchical_utils.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/hierarchical_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                             intervals_method = method)
     
     numeric_columns = Y_rec_df.select_dtypes(include=[np.number]).columns
     Y_rec_df[numeric_columns] = Y_rec_df[numeric_columns].round().astype(int) # update a round before astype (as astype is like "floor")
     return Y_rec_df, hrec.reconcilers
 
 def best_reconcile(concat_df_test, reconciled_df, y_true,
-                     model_name, weight_rmse = 0.5, weights_mape = 0.5):
+                     model_name, weight_rmse = 0.5, weights_mape = 0.0):
     
     # TODO -> funzione che riallinea le colonne di output di predizione (Id_pred)
     concat_df_test = concat_df_test.dropna()
     reconciled_df = reconciled_df.dropna()
     joined_df = reconciled_df.join(concat_df_test, how='inner')
 
     if len(joined_df) > 0:
```

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/algorithms/prophet_utils.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/algorithms/prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/analytics/evaluationMetrics.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/datahandler/datahandler.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/datapreparation/prep.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/datapreparation/prep.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,71 @@
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing_extensions import Self, Any
 import pandas as pd
 import pickle
 
 from ..utility.tele_logger import logger
 from ..utility.resources import *
-from .datapreparation_utils import ModelPreprocess
+from .datapreparation.datapreparation_utils import ModelPreprocess
+
 
 class PreprocessingClass(BaseEstimator, TransformerMixin):
 
     def __init__(self,
-                 target_col : str,
-                 date_col : str,
-                 usecase: str = "teleconsulto",
-                 model: str = "prophet"
+                 usecase: str,
+                 model: str,
                  ):
         """Pass all the parameters that can be set as explicit keyword
         arguments.
         
         Parameters
         ----------
-        target_col: str
-            Column name identifying column from which to generate target aggregate
-        date_col: str
-            Column name identifying the datetime column to index on
         usecase: str
             Parameter identifying usecase into account
         model: str
             Parameter identifying model to use
             
         """
 
-        self.usecase = usecase
-        self.model = model
+        self.usecase = usecase.lower()
+        self.model  = model.lower()
 
         if self.usecase == "teleconsulto":
-            self.preprocessing = ModelPreprocess(target_col=target_col, date_col=date_col)
+            self.preprocessing = ModelPreprocess()
         elif self.usecase == "televisita":
             pass
         elif self.usecase == "teleassistenza":
             pass
         elif self.usecase == "telemonitoraggio":
             pass
         return
     
     @log_exception(logger)
     def fit(self,
             X: pd.DataFrame,
-            time_granularity: str,
-            y: Any = None) -> Self:
+            y: Any = None,
+            **params: dict) -> Self:
         """Learn parameters useful for transforming data.
 
         Parameters
         ----------
         X : pd.DataFrame
             The input DataFrame.
-        time_granularity: str 
-            specifies temporal granularity
+        parmas: dict 
+            specifies prameters to initialize preprocessing
         y : None
             Ignored (only for compatibility).
         """
 
         if self.usecase == "teleconsulto":
             if self.model == "prophet":
-                self.time_granularity = time_granularity
-                pass
+                 for key, value in params.items():
+                     setattr(self, key, value)    
+            pass
+      
         return self
 
 
     def transform(self,
                 X: pd.DataFrame) -> pd.DataFrame:
         """Preparing Data to feed models"
 
@@ -84,15 +81,19 @@
         -------
         pd.DataFrame 
             DataFrame identifying the timeseries 
         """
 
         if self.usecase == "teleconsulto":
             if self.model == "prophet":
-                X = self.preprocessing.prophet(X, self.time_granularity)
+                X = self.preprocessing.generate_time_series(X, 
+                                                            self.date_col, 
+                                                            self.target_col, 
+                                                            self.time_granularity,
+                                                            self.missing_data_strategy)
             else:
                 pass
         elif self.usecase == "televisita":
             pass
         elif self.usecase == "teleassistenza":
             pass
         elif self.usecase == "telemonitoraggio":
```

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/datavisualization/plotPrediction.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/plotPrediction.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.data = data
         self.pred_mean = pred_mean
         self.pi_lower = pi_lower
         self.pi_upper = pi_upper
         self.use_case = use_case
 
     def plot_pred(self, df_pred: pd.DataFrame, id_pred: str = None,
-                  df_real: pd.DataFrame = None, target: str = None) -> plotly.graph_objs._figure.Figure:
+                  df_real: pd.DataFrame = None, data_real: str = None, target: str = None, confidence_interval: bool = False) -> plotly.graph_objs._figure.Figure:
             
         """Plot prediction
 
         Parameters
         ----------
         df_pred : pd:DataFrame
             dataframe of prediction
@@ -81,15 +81,15 @@
             regione = id_pre
 
             df_pred_parz = df_pred[df_pred[self.id_pred] == id_pre]
 
             if not isinstance(df_real,type(None)):
                 df_real_parz = df_real[df_real[self.id_pred] == id_pre]
                 real = [go.Scatter(
-                        x=df_real_parz[self.data],
+                        x=df_real_parz[data_real],
                         y=df_real_parz[target],
                         marker=dict(color="blue"),
                         mode="lines",
                         name="past value (true)",showlegend=True
                     )]
             else:
                 real = []
@@ -111,35 +111,38 @@
                     )
                 ),
             )
 
             fig.data[0].name = "predict value"
             fig.update_traces(showlegend=True)
 
-            fig.add_traces(
-                [
-                    go.Scatter(
-                        x=df_pred_parz[self.data],
-                        y=(df_pred_parz[self.pi_lower]),
-                        mode="lines",
-                        line_color="rgba(0,0,0,0)",
-                        showlegend=False,
-                    ),
-                    go.Scatter(
-                        x=df_pred_parz[self.data],
-                        y=(df_pred_parz[self.pi_upper]),
-                        mode="lines",
-                        line_color="rgba(0,0,0,0)",
-                        name="95% confidence interval",
-                        fill="tonexty",
-                        fillcolor="rgba(124, 252, 0, 0.2)",
-                        showlegend=True,
-                    )
-                ] + real
-            )
+            if confidence_interval:
+                fig.add_traces(
+                    [
+                        go.Scatter(
+                            x=df_pred_parz[self.data],
+                            y=(df_pred_parz[self.pi_lower]),
+                            mode="lines",
+                            line_color="rgba(0,0,0,0)",
+                            showlegend=False,
+                        ),
+                        go.Scatter(
+                            x=df_pred_parz[self.data],
+                            y=(df_pred_parz[self.pi_upper]),
+                            mode="lines",
+                            line_color="rgba(0,0,0,0)",
+                            name="95% confidence interval",
+                            fill="tonexty",
+                            fillcolor="rgba(124, 252, 0, 0.2)",
+                            showlegend=True,
+                        )
+                    ] 
+                )
+
+            fig.add_traces(real)
 
             fig.update_layout(legend=dict(yanchor="top", y=0.99, xanchor="left", x=0.01))
 
             lista_fig += [fig]
 
         return lista_fig
```

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         time_series = self.df[self.target] - trend
 
         autocorr = acf(time_series.dropna(), nlags=n_lags)[1:]
         fig1 = px.bar(
             x=np.arange(autocorr.shape[0]) + 1,
             y=autocorr,
             labels={"x": "Lag", "y": "Autocorrelazione"},
-            title="Autocorrelazione",
+            title="Autocorrelazione (detrendizzata)",
             template=dict(
                 layout=go.Layout(
                     title_font=dict(family="Rockwell", size=24, color="red"),
                     font=dict(color="green"),
                 )
             ),
         )
```

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/datavisualization/visualization.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/datavisualization/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,17 +308,16 @@
 
         df_sort = df.sort_values(data)
 
         lista = [(df_sort[df_sort[column] == i][self.target].values.astype(np.double),i)
          for i in df_sort[column].unique()]
 
         lista_time_series = [i[0]/i[0].max() for i in lista]
-        len_time_series = [len(i[0]) for i in lista]
-        len_matrix_time_series = np.array([i[0]*i[1] for i in itertools.product([len(i[0]) for i in len_time_series],repeat=2)])
-        len_matrix_time_series.shape = (21,21)
+        len_time_series = np.array([len(i[0]) for i in lista])
+        len_matrix_time_series = np.sqrt(np.einsum("i, j -> ij", len_time_series, len_time_series))
         distance_matrix = dtw.distance_matrix_fast(lista_time_series)
         
         distance_matrix_normalized = distance_matrix / len_matrix_time_series
 
         fig = px.imshow(distance_matrix_normalized, text_auto=True, template=dict(
                 layout=go.Layout(
                     title_font=dict(family="Rockwell", size=24, color="grey"),
@@ -327,27 +326,27 @@
                 height=700,
                 title=f"Distance matrix ({column})",
                 )))
 
         fig.update_layout(
             xaxis = dict(
                 tickmode = 'array',
-                tickvals = [i for i in range(21)],
+                tickvals = [i for i in range(len(lista))],
                 ticktext = [i[1] for i in lista],tickfont=dict(family='Rockwell', color='green', size=10)
             ),
             yaxis = dict(
                 tickmode = 'array',
-                tickvals = [i for i in range(21)],
+                tickvals = [i for i in range(len(lista))],
                 ticktext = [i[1] for i in lista],tickangle=-45,tickfont=dict(family='Rockwell', color='green', size=10)
             )           
         )
 
         return (fig,distance_matrix_normalized)
 
-    def plot_distance_matrix(self, distance_matrix: np.ndarray):
+    def plot_distance_matrix(self, distance_matrix: np.ndarray, lista: list[tuple]):
         
         dists = squareform(distance_matrix)
         linkage_matrix = linkage(dists, "ward",optimal_ordering=0)
         
         dendr = plt.figure(figsize=(10,6))
         dendrogram(linkage_matrix, labels=[i[1] for i in lista],leaf_rotation=0,orientation="right")
         plt.title("DTW distance - dendrogramm")
```

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/utility/exceptions.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/utility/experiment_utils.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/utility/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/utility/resources.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/LIB_tc/test_tc/utility/tele_logger.py` & `TEST_TC-1.0.5/LIB_tc/test_tc/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/README.md` & `TEST_TC-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/pyproject.toml` & `TEST_TC-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_algorithm.py` & `TEST_TC-1.0.5/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_datahandler.py` & `TEST_TC-1.0.5/tests/test_datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_datapreparation_utils.py` & `TEST_TC-1.0.5/tests/test_datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_evaluations.py` & `TEST_TC-1.0.5/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_exceptions.py` & `TEST_TC-1.0.5/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_experiment_job.py` & `TEST_TC-1.0.5/tests/test_experiment_job.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_experiment_models.py` & `TEST_TC-1.0.5/tests/test_experiment_models.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_experiment_utils.py` & `TEST_TC-1.0.5/tests/test_experiment_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_prep.py` & `TEST_TC-1.0.5/tests/test_prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_prophet_utils.py` & `TEST_TC-1.0.5/tests/test_prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_resources.py` & `TEST_TC-1.0.5/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.0.4/tests/test_tele_logger.py` & `TEST_TC-1.0.5/tests/test_tele_logger.py`

 * *Files identical despite different names*

