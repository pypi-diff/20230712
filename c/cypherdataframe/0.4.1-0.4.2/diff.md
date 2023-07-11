# Comparing `tmp/cypherdataframe-0.4.1.tar.gz` & `tmp/cypherdataframe-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypherdataframe-0.4.1.tar", last modified: Tue Jul 11 22:53:17 2023, max compression
+gzip compressed data, was "cypherdataframe-0.4.2.tar", last modified: Tue Jul 11 23:02:40 2023, max compression
```

## Comparing `cypherdataframe-0.4.1.tar` & `cypherdataframe-0.4.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.864379 cypherdataframe-0.4.1/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 22:53:17.864128 cypherdataframe-0.4.1/PKG-INFO
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.846746 cypherdataframe-0.4.1/cypherdataframe/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.4.1/cypherdataframe/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.4.1/cypherdataframe/branch_maker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.4.1/cypherdataframe/config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     9473 2023-07-05 21:26:56.000000 cypherdataframe-0.4.1/cypherdataframe/cypher.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.850203 cypherdataframe-0.4.1/cypherdataframe/garner_domain/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1412 2023-07-11 22:52:04.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/BranchMaker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.851280 cypherdataframe-0.4.1/cypherdataframe/garner_domain/logistics/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:02:39.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/logistics/TransferBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/logistics/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.851897 cypherdataframe-0.4.1/cypherdataframe/garner_domain/measure/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-07-11 21:47:41.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/measure/MeasureBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/measure/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/properties_defaults.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.852511 cypherdataframe-0.4.1/cypherdataframe/garner_domain/queries/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1001 2023-07-11 22:52:04.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/queries/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.853063 cypherdataframe-0.4.1/cypherdataframe/garner_domain/reference/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      613 2023-06-29 21:20:43.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/reference/ReferenceBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/reference/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.855179 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:17:38.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-06-29 21:18:56.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/AttainedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      658 2023-06-29 21:17:38.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      615 2023-06-29 21:18:10.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/ForecastedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.858354 cypherdataframe-0.4.1/cypherdataframe/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2345 2023-07-11 22:51:01.000000 cypherdataframe-0.4.1/cypherdataframe/model/Branch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.4.1/cypherdataframe/model/Config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      860 2023-07-11 22:49:50.000000 cypherdataframe-0.4.1/cypherdataframe/model/LabelNode.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.4.1/cypherdataframe/model/Property.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.4.1/cypherdataframe/model/Query.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.4.1/cypherdataframe/model/QueryAccumulation.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.4.1/cypherdataframe/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.4.1/cypherdataframe/testfunctions.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.848951 cypherdataframe-0.4.1/cypherdataframe.egg-info/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/PKG-INFO
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/SOURCES.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/dependency_links.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/requires.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-11 22:53:17.000000 cypherdataframe-0.4.1/cypherdataframe.egg-info/top_level.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-11 22:53:17.864470 cypherdataframe-0.4.1/setup.cfg
--rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-11 22:52:41.000000 cypherdataframe-0.4.1/setup.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.861008 cypherdataframe-0.4.1/tests/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.4.1/tests/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.4.1/tests/branch_maker_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.4.1/tests/conftest.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.4.1/tests/cypher_integration_test.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.861333 cypherdataframe-0.4.1/tests/fixtures/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.1/tests/fixtures/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.862700 cypherdataframe-0.4.1/tests/fixtures/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.4.1/tests/fixtures/model/Branch_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.4.1/tests/fixtures/model/Node_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.4.1/tests/fixtures/model/Property_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.4.1/tests/fixtures/model/Query_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.1/tests/fixtures/model/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 22:53:17.863815 cypherdataframe-0.4.1/tests/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.4.1/tests/model/Branch_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.4.1/tests/model/Node_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.4.1/tests/model/Query_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.1/tests/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.4.1/tests/test_config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.4.1/tests/test_testfunctions.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.4.1/tests/tsest_ignorefunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.215281 cypherdataframe-0.4.2/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 23:02:40.214911 cypherdataframe-0.4.2/PKG-INFO
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.201043 cypherdataframe-0.4.2/cypherdataframe/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.4.2/cypherdataframe/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.4.2/cypherdataframe/branch_maker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.4.2/cypherdataframe/config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     9473 2023-07-05 21:26:56.000000 cypherdataframe-0.4.2/cypherdataframe/cypher.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.203391 cypherdataframe-0.4.2/cypherdataframe/garner_domain/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1412 2023-07-11 22:52:04.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/BranchMaker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.204368 cypherdataframe-0.4.2/cypherdataframe/garner_domain/logistics/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-07-11 23:01:55.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/logistics/TransferBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/logistics/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.205158 cypherdataframe-0.4.2/cypherdataframe/garner_domain/measure/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-07-11 23:01:55.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/measure/MeasureBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/measure/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/properties_defaults.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.205685 cypherdataframe-0.4.2/cypherdataframe/garner_domain/queries/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1001 2023-07-11 22:52:04.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/queries/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.206245 cypherdataframe-0.4.2/cypherdataframe/garner_domain/reference/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      647 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/reference/ReferenceBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/reference/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.207655 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/AttainedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      692 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      649 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/ForecastedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.209744 cypherdataframe-0.4.2/cypherdataframe/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2345 2023-07-11 22:51:01.000000 cypherdataframe-0.4.2/cypherdataframe/model/Branch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.4.2/cypherdataframe/model/Config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      860 2023-07-11 22:49:50.000000 cypherdataframe-0.4.2/cypherdataframe/model/LabelNode.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.4.2/cypherdataframe/model/Property.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.4.2/cypherdataframe/model/Query.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.4.2/cypherdataframe/model/QueryAccumulation.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.4.2/cypherdataframe/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.4.2/cypherdataframe/testfunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.202567 cypherdataframe-0.4.2/cypherdataframe.egg-info/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/PKG-INFO
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/requires.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/top_level.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-11 23:02:40.215398 cypherdataframe-0.4.2/setup.cfg
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-11 23:02:32.000000 cypherdataframe-0.4.2/setup.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.211634 cypherdataframe-0.4.2/tests/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.4.2/tests/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.4.2/tests/branch_maker_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.4.2/tests/conftest.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.4.2/tests/cypher_integration_test.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.211916 cypherdataframe-0.4.2/tests/fixtures/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.2/tests/fixtures/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.213233 cypherdataframe-0.4.2/tests/fixtures/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.4.2/tests/fixtures/model/Branch_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.4.2/tests/fixtures/model/Node_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.4.2/tests/fixtures/model/Property_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.4.2/tests/fixtures/model/Query_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.2/tests/fixtures/model/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.214474 cypherdataframe-0.4.2/tests/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.4.2/tests/model/Branch_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.4.2/tests/model/Node_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.4.2/tests/model/Query_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.2/tests/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.4.2/tests/test_config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.4.2/tests/test_testfunctions.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.4.2/tests/tsest_ignorefunctions.py
```

### Comparing `cypherdataframe-0.4.1/cypherdataframe/branch_maker.py` & `cypherdataframe-0.4.2/cypherdataframe/branch_maker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/cypherdataframe/cypher.py` & `cypherdataframe-0.4.2/cypherdataframe/cypher.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/BranchMaker.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/BranchMaker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/logistics/TransferBranch.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/AttainedBranch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import dataclass, field
 
 from cypherdataframe.garner_domain.BranchMaker import BranchMaker
-from cypherdataframe.garner_domain.properties_defaults import \
-    TRANSFER_RELATIONSHIP, \
-    TRANSFER_RETURN_ID, TRANSFER_LABEL
+from cypherdataframe.garner_domain.properties_defaults import ATTAINED_RELATIONSHIP, ATTAINED_RETURN_POSTFIX
 from cypherdataframe.model.Property import Property
 
 
+
 @dataclass
-class TransferBranch(BranchMaker):
+class AttainedBranch(BranchMaker):
     props: list[Property]
-    label: str = TRANSFER_LABEL
-    relationship: str = field(default_factory=lambda: TRANSFER_RELATIONSHIP)
-    relationship_postfix: str | None = field(default_factory=lambda: TRANSFER_RETURN_ID)
+    post_label: str | None = None
+    relationship: str = field(default_factory=lambda: ATTAINED_RELATIONSHIP)
+    relationship_postfix: str | None = field(default_factory=lambda: ATTAINED_RETURN_POSTFIX)
     required: bool = False
-    archived: bool = True
+    archived: bool = False
     domain_label: str | None = None
+
```

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/measure/MeasureBranch.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/measure/MeasureBranch.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,13 +5,14 @@
     MEASURE_RELATIONSHIP, MEASURE_RETURN_POSTFIX
 from cypherdataframe.model.Property import Property
 
 
 @dataclass
 class MeasureBranch(BranchMaker):
     props: list[Property]
+    post_label: str | None = None
     relationship: str = field(default_factory=lambda: MEASURE_RELATIONSHIP)
     relationship_postfix: str | None = field(default_factory=lambda: MEASURE_RETURN_POSTFIX)
     required: bool = False
     archived: bool = False
     domain_label: str | None = None
```

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/properties_defaults.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/properties_defaults.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/reference/ReferenceBranch.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/reference/ReferenceBranch.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,12 +4,13 @@
 from cypherdataframe.garner_domain.properties_defaults import REFERENCED_RELATIONSHIP, REFERENCED_RETURN_POSTFIX
 from cypherdataframe.model.Property import Property
 
 
 @dataclass
 class ReferenceBranch(BranchMaker):
     props: list[Property]
+    post_label: str | None = None
     relationship: str = field(default_factory=lambda: REFERENCED_RELATIONSHIP)
     relationship_postfix: str | None = field(default_factory=lambda: REFERENCED_RETURN_POSTFIX)
     required: bool = False
     archived: bool = False
     domain_label: str | None = None
```

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,12 +5,13 @@
     ARCHIVED_ATTAINED_RETURN_POSTFIX
 from cypherdataframe.model.Property import Property
 
 
 @dataclass
 class AttainedArchivedBranch(BranchMaker):
     props: list[Property]
+    post_label: str | None = None
     relationship: str = field(default_factory=lambda: ARCHIVED_ATTAINED_RELATIONSHIP)
     relationship_postfix: str | None = field(default_factory=lambda: ARCHIVED_ATTAINED_RETURN_POSTFIX)
     required: bool = False
     archived: bool = True
     domain_label: str | None = None
```

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/AttainedBranch.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from dataclasses import dataclass, field
 
 from cypherdataframe.garner_domain.BranchMaker import BranchMaker
-from cypherdataframe.garner_domain.properties_defaults import ATTAINED_RELATIONSHIP, ATTAINED_RETURN_POSTFIX
+from cypherdataframe.garner_domain.properties_defaults import ARCHIVED_FORECASTED_RELATIONSHIP, ARCHIVED_FORECASTED_RETURN_POSTFIX
 from cypherdataframe.model.Property import Property
 
 
-
 @dataclass
-class AttainedBranch(BranchMaker):
+class ForecastedArchivedBranch(BranchMaker):
     props: list[Property]
-    relationship: str = field(default_factory=lambda: ATTAINED_RELATIONSHIP)
-    relationship_postfix: str | None = field(default_factory=lambda: ATTAINED_RETURN_POSTFIX)
+    post_label: str | None = None
+    relationship: str = field(default_factory=lambda: ARCHIVED_FORECASTED_RELATIONSHIP)
+    relationship_postfix: str | None = field(default_factory=lambda: ARCHIVED_FORECASTED_RETURN_POSTFIX)
     required: bool = False
-    archived: bool = False
+    archived: bool = True
     domain_label: str | None = None
```

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/logistics/TransferBranch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from dataclasses import dataclass, field
 
 from cypherdataframe.garner_domain.BranchMaker import BranchMaker
-from cypherdataframe.garner_domain.properties_defaults import ARCHIVED_FORECASTED_RELATIONSHIP, ARCHIVED_FORECASTED_RETURN_POSTFIX
+from cypherdataframe.garner_domain.properties_defaults import \
+    TRANSFER_RELATIONSHIP, \
+    TRANSFER_RETURN_ID, TRANSFER_LABEL
 from cypherdataframe.model.Property import Property
 
 
 @dataclass
-class ForecastedArchivedBranch(BranchMaker):
+class TransferBranch(BranchMaker):
     props: list[Property]
-    relationship: str = field(default_factory=lambda: ARCHIVED_FORECASTED_RELATIONSHIP)
-    relationship_postfix: str | None = field(default_factory=lambda: ARCHIVED_FORECASTED_RETURN_POSTFIX)
+    label: str = TRANSFER_LABEL
+    post_label: str | None = None
+    relationship: str = field(default_factory=lambda: TRANSFER_RELATIONSHIP)
+    relationship_postfix: str | None = field(default_factory=lambda: TRANSFER_RETURN_ID)
     required: bool = False
     archived: bool = True
     domain_label: str | None = None
-
```

### Comparing `cypherdataframe-0.4.1/cypherdataframe/garner_domain/status/ForecastedBranch.py` & `cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/ForecastedBranch.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 from cypherdataframe.garner_domain.properties_defaults import FORECASTED_RETURN_POSTFIX, FORECASTED_RELATIONSHIP
 from cypherdataframe.model.Property import Property
 
 
 @dataclass
 class ForecastedBranch(BranchMaker):
     props: list[Property]
+    post_label: str | None = None
     relationship: str = field(default_factory=lambda: FORECASTED_RELATIONSHIP)
     relationship_postfix: str | None = field(default_factory=lambda: FORECASTED_RETURN_POSTFIX)
     required: bool = False
     archived: bool = False
     domain_label: str | None = None
```

### Comparing `cypherdataframe-0.4.1/cypherdataframe/model/Branch.py` & `cypherdataframe-0.4.2/cypherdataframe/model/Branch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/cypherdataframe/model/LabelNode.py` & `cypherdataframe-0.4.2/cypherdataframe/model/LabelNode.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/cypherdataframe/model/Query.py` & `cypherdataframe-0.4.2/cypherdataframe/model/Query.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/cypherdataframe/model/QueryAccumulation.py` & `cypherdataframe-0.4.2/cypherdataframe/model/QueryAccumulation.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/cypherdataframe.egg-info/SOURCES.txt` & `cypherdataframe-0.4.2/cypherdataframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/setup.py` & `cypherdataframe-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             'cypherdataframe.garner_domain.logistics',
             'cypherdataframe.garner_domain.measure',
             'cypherdataframe.garner_domain.queries',
             'cypherdataframe.garner_domain.reference',
             'cypherdataframe.garner_domain.status'
         ]
     ),
-    version='0.4.1',
+    version='0.4.2',
     description='Cypher Query to df Toolkit',
     author='Attila Vanderploeg',
     license='MIT',
     install_requires=['py2neo>=2021.2.3', 'dacite>=1.6.0'],
     setup_requires=[],
     tests_require=[],
     test_suite='tests',
```

### Comparing `cypherdataframe-0.4.1/tests/branch_maker_test.py` & `cypherdataframe-0.4.2/tests/branch_maker_test.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/tests/fixtures/model/Property_fixture.py` & `cypherdataframe-0.4.2/tests/fixtures/model/Property_fixture.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.1/tests/tsest_ignorefunctions.py` & `cypherdataframe-0.4.2/tests/tsest_ignorefunctions.py`

 * *Files identical despite different names*

