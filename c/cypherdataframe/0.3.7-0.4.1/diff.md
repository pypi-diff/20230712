# Comparing `tmp/cypherdataframe-0.3.7.tar.gz` & `tmp/cypherdataframe-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypherdataframe-0.3.7.tar", last modified: Tue Jul 11 21:49:43 2023, max compression
+gzip compressed data, was "cypherdataframe-0.4.1.tar", last modified: Tue Jul 11 22:53:17 2023, max compression
```

## Comparing `cypherdataframe-0.3.7.tar` & `cypherdataframe-0.4.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.650329 cypherdataframe-0.3.7/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 21:49:43.650000 cypherdataframe-0.3.7/PKG-INFO
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.634496 cypherdataframe-0.3.7/cypherdataframe/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.3.7/cypherdataframe/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.3.7/cypherdataframe/branch_maker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.3.7/cypherdataframe/config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     9473 2023-07-05 21:26:56.000000 cypherdataframe-0.3.7/cypherdataframe/cypher.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.636939 cypherdataframe-0.3.7/cypherdataframe/garner_domain/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1340 2023-06-29 20:43:49.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/BranchMaker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.637506 cypherdataframe-0.3.7/cypherdataframe/garner_domain/logistics/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:02:39.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/logistics/TransferBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/logistics/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.638230 cypherdataframe-0.3.7/cypherdataframe/garner_domain/measure/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-07-11 21:47:41.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/measure/MeasureBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/measure/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/properties_defaults.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.638777 cypherdataframe-0.3.7/cypherdataframe/garner_domain/queries/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      919 2023-06-29 20:44:47.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/queries/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.639355 cypherdataframe-0.3.7/cypherdataframe/garner_domain/reference/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      613 2023-06-29 21:20:43.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/reference/ReferenceBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/reference/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.640830 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:17:38.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-06-29 21:18:56.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/AttainedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      658 2023-06-29 21:17:38.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      615 2023-06-29 21:18:10.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/ForecastedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.643619 cypherdataframe-0.3.7/cypherdataframe/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2213 2023-06-15 17:59:52.000000 cypherdataframe-0.3.7/cypherdataframe/model/Branch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.3.7/cypherdataframe/model/Config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      829 2023-05-05 22:58:23.000000 cypherdataframe-0.3.7/cypherdataframe/model/LabelNode.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.3.7/cypherdataframe/model/Property.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.3.7/cypherdataframe/model/Query.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.3.7/cypherdataframe/model/QueryAccumulation.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.3.7/cypherdataframe/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.3.7/cypherdataframe/testfunctions.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.635954 cypherdataframe-0.3.7/cypherdataframe.egg-info/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/PKG-INFO
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/SOURCES.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/dependency_links.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/requires.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-11 21:49:43.000000 cypherdataframe-0.3.7/cypherdataframe.egg-info/top_level.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-11 21:49:43.650406 cypherdataframe-0.3.7/setup.cfg
--rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-11 21:49:27.000000 cypherdataframe-0.3.7/setup.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.645826 cypherdataframe-0.3.7/tests/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.3.7/tests/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.3.7/tests/branch_maker_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.3.7/tests/conftest.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.3.7/tests/cypher_integration_test.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.646183 cypherdataframe-0.3.7/tests/fixtures/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.7/tests/fixtures/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.648211 cypherdataframe-0.3.7/tests/fixtures/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.3.7/tests/fixtures/model/Branch_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.3.7/tests/fixtures/model/Node_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.3.7/tests/fixtures/model/Property_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.3.7/tests/fixtures/model/Query_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.7/tests/fixtures/model/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 21:49:43.649706 cypherdataframe-0.3.7/tests/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.3.7/tests/model/Branch_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.3.7/tests/model/Node_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.3.7/tests/model/Query_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.7/tests/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.3.7/tests/test_config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.3.7/tests/test_testfunctions.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.3.7/tests/tsest_ignorefunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.864379 cypherdataframe-0.4.1/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 22:53:17.864128 cypherdataframe-0.4.1/PKG-INFO
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.846746 cypherdataframe-0.4.1/cypherdataframe/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.4.1/cypherdataframe/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.4.1/cypherdataframe/branch_maker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.4.1/cypherdataframe/config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     9473 2023-07-05 21:26:56.000000 cypherdataframe-0.4.1/cypherdataframe/cypher.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.850203 cypherdataframe-0.4.1/cypherdataframe/garner_domain/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1412 2023-07-11 22:52:04.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/BranchMaker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.851280 cypherdataframe-0.4.1/cypherdataframe/garner_domain/logistics/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:02:39.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/logistics/TransferBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/logistics/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.851897 cypherdataframe-0.4.1/cypherdataframe/garner_domain/measure/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-07-11 21:47:41.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/measure/MeasureBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/measure/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/properties_defaults.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.852511 cypherdataframe-0.4.1/cypherdataframe/garner_domain/queries/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1001 2023-07-11 22:52:04.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/queries/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.853063 cypherdataframe-0.4.1/cypherdataframe/garner_domain/reference/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      613 2023-06-29 21:20:43.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/reference/ReferenceBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/reference/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.855179 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:17:38.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-06-29 21:18:56.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/AttainedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      658 2023-06-29 21:17:38.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      615 2023-06-29 21:18:10.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/ForecastedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.858354 cypherdataframe-0.4.1/cypherdataframe/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2345 2023-07-11 22:51:01.000000 cypherdataframe-0.4.1/cypherdataframe/model/Branch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.4.1/cypherdataframe/model/Config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      860 2023-07-11 22:49:50.000000 cypherdataframe-0.4.1/cypherdataframe/model/LabelNode.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.4.1/cypherdataframe/model/Property.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.4.1/cypherdataframe/model/Query.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.4.1/cypherdataframe/model/QueryAccumulation.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.4.1/cypherdataframe/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.4.1/cypherdataframe/testfunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.848951 cypherdataframe-0.4.1/cypherdataframe.egg-info/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/PKG-INFO
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/requires.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/top_level.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-11 22:53:17.864470 cypherdataframe-0.4.1/setup.cfg
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-11 22:52:41.000000 cypherdataframe-0.4.1/setup.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.861008 cypherdataframe-0.4.1/tests/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.4.1/tests/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.4.1/tests/branch_maker_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.4.1/tests/conftest.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.4.1/tests/cypher_integration_test.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.861333 cypherdataframe-0.4.1/tests/fixtures/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.1/tests/fixtures/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.862700 cypherdataframe-0.4.1/tests/fixtures/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.4.1/tests/fixtures/model/Branch_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.4.1/tests/fixtures/model/Node_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.4.1/tests/fixtures/model/Property_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.4.1/tests/fixtures/model/Query_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.1/tests/fixtures/model/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.863815 cypherdataframe-0.4.1/tests/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.4.1/tests/model/Branch_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.4.1/tests/model/Node_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.4.1/tests/model/Query_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.1/tests/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.4.1/tests/test_config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.4.1/tests/test_testfunctions.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.4.1/tests/tsest_ignorefunctions.py
```

### Comparing `cypherdataframe-0.3.7/cypherdataframe/branch_maker.py` & `cypherdataframe-0.4.1/cypherdataframe/branch_maker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/cypher.py` & `cypherdataframe-0.4.1/cypherdataframe/cypher.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/BranchMaker.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/BranchMaker.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from abc import ABC, abstractmethod
 
 
 @dataclass
 class BranchMaker(ABC):
     props: list[Property]
     label: str
+    post_label: str | None
     relationship: str
     relationship_postfix: str | None
     required: bool
     archived: bool
     domain_label: str | None
 
 
@@ -40,8 +41,9 @@
         )
 
     def to_label_node(self) -> LabelNode:
         return LabelNode(
             return_id=self.return_id()
             , label=self.node_label()
             , properties=self.props
+            , post_label_str=self.post_label
         )
```

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/logistics/TransferBranch.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/logistics/TransferBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/measure/MeasureBranch.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/measure/MeasureBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/properties_defaults.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/properties_defaults.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 from cypherdataframe.model.Property import Property
 from cypherdataframe.model.Query import Query
 
 @dataclass
 class LogisticsTableQuery:
     branchMakers: list[BranchMaker]
     label: str
+    post_label: str | None = None
     return_id: str = "l"
     props: list[Property] = field(default_factory=lambda: [ID_PROP])
     def to_query(self, skip: int | None = None, limit: int | None = None):
         return Query(
             LabelNode(
                 return_id=self.return_id,
                 label=self.label,
                 properties=self.props,
-                collect=False
+                collect=False,
+                post_label_str=self.post_label
             ),
             branches=[b.to_branch() for b in self.branchMakers],
             skip=skip,
             limit=limit
         )
```

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/reference/ReferenceBranch.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/reference/ReferenceBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/AttainedBranch.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/AttainedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/garner_domain/status/ForecastedBranch.py` & `cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/ForecastedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/model/Branch.py` & `cypherdataframe-0.4.1/cypherdataframe/model/Branch.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,19 @@
     def relationship_cypher_final_assignment(self) -> str | None:
         if self.relationship == None:
             return f"TYPE({self.relationship_cypher_assignment()}) as {self.relationship_cypher_assignment()}"
         else:
             return None
 
     def match_statement(self, corenode: LabelNode, with_assignment: bool):
+        if self.post_label_str:
+            post_label = self.post_label_str
+        else:
+            post_label = ""
+
         if self.away_from_core == True:
             back = ''
             forward = '>'
         elif self.away_from_core == False:
             back = '<'
             forward = ''
         else:
@@ -67,14 +72,14 @@
         else:
             relationship_str = f":{self.relationship}"
 
         fragment = (
             f" {optional} " 
             f"match({corenode.return_id}){back}" 
             f"-[{relationship_str}]-"
-            f"{forward}({node_id}:{self.branch_node.label})"
+            f"{forward}({node_id}:{self.branch_node.label}{post_label})"
         )
 
         return fragment
```

### Comparing `cypherdataframe-0.3.7/cypherdataframe/model/LabelNode.py` & `cypherdataframe-0.4.1/cypherdataframe/model/LabelNode.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from cypherdataframe.model.Property import Property
 
 
 @dataclass(frozen=True)
 class LabelNode:
     return_id: str
     label: str
+    post_label_str: str | None
     properties: list[Property]
     collect: bool = False
 
     def properties_by_final_assigment(self):
         return {prop.final_assigment(self): prop for prop in self.properties}
 
     def property_fragments_by_cypher_assignments(self):
```

### Comparing `cypherdataframe-0.3.7/cypherdataframe/model/Query.py` & `cypherdataframe-0.4.1/cypherdataframe/model/Query.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe/model/QueryAccumulation.py` & `cypherdataframe-0.4.1/cypherdataframe/model/QueryAccumulation.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/cypherdataframe.egg-info/SOURCES.txt` & `cypherdataframe-0.4.1/cypherdataframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/setup.py` & `cypherdataframe-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             'cypherdataframe.garner_domain.logistics',
             'cypherdataframe.garner_domain.measure',
             'cypherdataframe.garner_domain.queries',
             'cypherdataframe.garner_domain.reference',
             'cypherdataframe.garner_domain.status'
         ]
     ),
-    version='0.3.7',
+    version='0.4.1',
     description='Cypher Query to df Toolkit',
     author='Attila Vanderploeg',
     license='MIT',
     install_requires=['py2neo>=2021.2.3', 'dacite>=1.6.0'],
     setup_requires=[],
     tests_require=[],
     test_suite='tests',
```

### Comparing `cypherdataframe-0.3.7/tests/branch_maker_test.py` & `cypherdataframe-0.4.1/tests/branch_maker_test.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/tests/fixtures/model/Property_fixture.py` & `cypherdataframe-0.4.1/tests/fixtures/model/Property_fixture.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.7/tests/tsest_ignorefunctions.py` & `cypherdataframe-0.4.1/tests/tsest_ignorefunctions.py`

 * *Files identical despite different names*

