# Comparing `tmp/cypherdataframe-0.4.2.tar.gz` & `tmp/cypherdataframe-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypherdataframe-0.4.2.tar", last modified: Tue Jul 11 23:02:40 2023, max compression
+gzip compressed data, was "cypherdataframe-0.5.1.tar", last modified: Tue Jul 11 23:06:32 2023, max compression
```

## Comparing `cypherdataframe-0.4.2.tar` & `cypherdataframe-0.5.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.215281 cypherdataframe-0.4.2/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 23:02:40.214911 cypherdataframe-0.4.2/PKG-INFO
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.201043 cypherdataframe-0.4.2/cypherdataframe/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.4.2/cypherdataframe/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.4.2/cypherdataframe/branch_maker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.4.2/cypherdataframe/config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     9473 2023-07-05 21:26:56.000000 cypherdataframe-0.4.2/cypherdataframe/cypher.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.203391 cypherdataframe-0.4.2/cypherdataframe/garner_domain/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1412 2023-07-11 22:52:04.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/BranchMaker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.204368 cypherdataframe-0.4.2/cypherdataframe/garner_domain/logistics/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-07-11 23:01:55.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/logistics/TransferBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/logistics/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.205158 cypherdataframe-0.4.2/cypherdataframe/garner_domain/measure/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-07-11 23:01:55.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/measure/MeasureBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/measure/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/properties_defaults.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.205685 cypherdataframe-0.4.2/cypherdataframe/garner_domain/queries/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1001 2023-07-11 22:52:04.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/queries/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.206245 cypherdataframe-0.4.2/cypherdataframe/garner_domain/reference/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      647 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/reference/ReferenceBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/reference/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.207655 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/AttainedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      692 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      649 2023-07-11 23:02:18.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/ForecastedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.209744 cypherdataframe-0.4.2/cypherdataframe/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2345 2023-07-11 22:51:01.000000 cypherdataframe-0.4.2/cypherdataframe/model/Branch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.4.2/cypherdataframe/model/Config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      860 2023-07-11 22:49:50.000000 cypherdataframe-0.4.2/cypherdataframe/model/LabelNode.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.4.2/cypherdataframe/model/Property.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.4.2/cypherdataframe/model/Query.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.4.2/cypherdataframe/model/QueryAccumulation.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.4.2/cypherdataframe/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.4.2/cypherdataframe/testfunctions.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.202567 cypherdataframe-0.4.2/cypherdataframe.egg-info/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/PKG-INFO
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/SOURCES.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/dependency_links.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/requires.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-11 23:02:40.000000 cypherdataframe-0.4.2/cypherdataframe.egg-info/top_level.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-11 23:02:40.215398 cypherdataframe-0.4.2/setup.cfg
--rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-11 23:02:32.000000 cypherdataframe-0.4.2/setup.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.211634 cypherdataframe-0.4.2/tests/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.4.2/tests/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.4.2/tests/branch_maker_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.4.2/tests/conftest.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.4.2/tests/cypher_integration_test.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.211916 cypherdataframe-0.4.2/tests/fixtures/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.2/tests/fixtures/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.213233 cypherdataframe-0.4.2/tests/fixtures/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.4.2/tests/fixtures/model/Branch_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.4.2/tests/fixtures/model/Node_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.4.2/tests/fixtures/model/Property_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.4.2/tests/fixtures/model/Query_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.2/tests/fixtures/model/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:02:40.214474 cypherdataframe-0.4.2/tests/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.4.2/tests/model/Branch_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.4.2/tests/model/Node_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.4.2/tests/model/Query_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.4.2/tests/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.4.2/tests/test_config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.4.2/tests/test_testfunctions.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.4.2/tests/tsest_ignorefunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.885131 cypherdataframe-0.5.1/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 23:06:32.884872 cypherdataframe-0.5.1/PKG-INFO
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.872190 cypherdataframe-0.5.1/cypherdataframe/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.5.1/cypherdataframe/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.5.1/cypherdataframe/branch_maker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.5.1/cypherdataframe/config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     9473 2023-07-05 21:26:56.000000 cypherdataframe-0.5.1/cypherdataframe/cypher.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.874549 cypherdataframe-0.5.1/cypherdataframe/garner_domain/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1412 2023-07-11 22:52:04.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/BranchMaker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.875152 cypherdataframe-0.5.1/cypherdataframe/garner_domain/logistics/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-07-11 23:01:55.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/logistics/TransferBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/logistics/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.875674 cypherdataframe-0.5.1/cypherdataframe/garner_domain/measure/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-07-11 23:01:55.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/measure/MeasureBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/measure/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/properties_defaults.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.876188 cypherdataframe-0.5.1/cypherdataframe/garner_domain/queries/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1001 2023-07-11 22:52:04.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/queries/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.876721 cypherdataframe-0.5.1/cypherdataframe/garner_domain/reference/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      647 2023-07-11 23:02:18.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/reference/ReferenceBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/reference/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.878101 cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-07-11 23:02:18.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-07-11 23:02:18.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/AttainedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      692 2023-07-11 23:02:18.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      649 2023-07-11 23:02:18.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/ForecastedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.879991 cypherdataframe-0.5.1/cypherdataframe/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2369 2023-07-11 23:05:52.000000 cypherdataframe-0.5.1/cypherdataframe/model/Branch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.5.1/cypherdataframe/model/Config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      860 2023-07-11 22:49:50.000000 cypherdataframe-0.5.1/cypherdataframe/model/LabelNode.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.5.1/cypherdataframe/model/Property.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.5.1/cypherdataframe/model/Query.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.5.1/cypherdataframe/model/QueryAccumulation.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.5.1/cypherdataframe/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.5.1/cypherdataframe/testfunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.873680 cypherdataframe-0.5.1/cypherdataframe.egg-info/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-11 23:06:32.000000 cypherdataframe-0.5.1/cypherdataframe.egg-info/PKG-INFO
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-11 23:06:32.000000 cypherdataframe-0.5.1/cypherdataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-11 23:06:32.000000 cypherdataframe-0.5.1/cypherdataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-11 23:06:32.000000 cypherdataframe-0.5.1/cypherdataframe.egg-info/requires.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-11 23:06:32.000000 cypherdataframe-0.5.1/cypherdataframe.egg-info/top_level.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-11 23:06:32.885217 cypherdataframe-0.5.1/setup.cfg
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-11 23:06:30.000000 cypherdataframe-0.5.1/setup.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.881867 cypherdataframe-0.5.1/tests/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.5.1/tests/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.5.1/tests/branch_maker_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.5.1/tests/conftest.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.5.1/tests/cypher_integration_test.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.882150 cypherdataframe-0.5.1/tests/fixtures/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.5.1/tests/fixtures/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.883500 cypherdataframe-0.5.1/tests/fixtures/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.5.1/tests/fixtures/model/Branch_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.5.1/tests/fixtures/model/Node_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.5.1/tests/fixtures/model/Property_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.5.1/tests/fixtures/model/Query_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.5.1/tests/fixtures/model/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-11 23:06:32.884564 cypherdataframe-0.5.1/tests/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.5.1/tests/model/Branch_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.5.1/tests/model/Node_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.5.1/tests/model/Query_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.5.1/tests/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.5.1/tests/test_config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.5.1/tests/test_testfunctions.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.5.1/tests/tsest_ignorefunctions.py
```

### Comparing `cypherdataframe-0.4.2/cypherdataframe/branch_maker.py` & `cypherdataframe-0.5.1/cypherdataframe/branch_maker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/cypher.py` & `cypherdataframe-0.5.1/cypherdataframe/cypher.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/BranchMaker.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/BranchMaker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/logistics/TransferBranch.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/logistics/TransferBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/measure/MeasureBranch.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/measure/MeasureBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/properties_defaults.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/properties_defaults.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/reference/ReferenceBranch.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/reference/ReferenceBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/AttainedBranch.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/AttainedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/garner_domain/status/ForecastedBranch.py` & `cypherdataframe-0.5.1/cypherdataframe/garner_domain/status/ForecastedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/model/Branch.py` & `cypherdataframe-0.5.1/cypherdataframe/model/Branch.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     def relationship_cypher_final_assignment(self) -> str | None:
         if self.relationship == None:
             return f"TYPE({self.relationship_cypher_assignment()}) as {self.relationship_cypher_assignment()}"
         else:
             return None
 
     def match_statement(self, corenode: LabelNode, with_assignment: bool):
-        if self.post_label_str:
-            post_label = self.post_label_str
+        if self.branch_node.post_label_str:
+            post_label = self.branch_node.post_label_str
         else:
             post_label = ""
 
         if self.away_from_core == True:
             back = ''
             forward = '>'
         elif self.away_from_core == False:
```

### Comparing `cypherdataframe-0.4.2/cypherdataframe/model/LabelNode.py` & `cypherdataframe-0.5.1/cypherdataframe/model/LabelNode.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/model/Query.py` & `cypherdataframe-0.5.1/cypherdataframe/model/Query.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe/model/QueryAccumulation.py` & `cypherdataframe-0.5.1/cypherdataframe/model/QueryAccumulation.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/cypherdataframe.egg-info/SOURCES.txt` & `cypherdataframe-0.5.1/cypherdataframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/setup.py` & `cypherdataframe-0.5.1/setup.py`

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
-    version='0.4.2',
+    version='0.5.1',
     description='Cypher Query to df Toolkit',
     author='Attila Vanderploeg',
     license='MIT',
     install_requires=['py2neo>=2021.2.3', 'dacite>=1.6.0'],
     setup_requires=[],
     tests_require=[],
     test_suite='tests',
```

### Comparing `cypherdataframe-0.4.2/tests/branch_maker_test.py` & `cypherdataframe-0.5.1/tests/branch_maker_test.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/tests/fixtures/model/Property_fixture.py` & `cypherdataframe-0.5.1/tests/fixtures/model/Property_fixture.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.4.2/tests/tsest_ignorefunctions.py` & `cypherdataframe-0.5.1/tests/tsest_ignorefunctions.py`

 * *Files identical despite different names*

