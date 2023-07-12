# Comparing `tmp/osemosys2iamc-0.2.1.tar.gz` & `tmp/osemosys2iamc-0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osemosys2iamc-0.2.1.tar", last modified: Wed Jul 12 08:32:33 2023, max compression
+gzip compressed data, was "osemosys2iamc-0.2a2.tar", last modified: Tue Jul 11 10:54:24 2023, max compression
```

## Comparing `osemosys2iamc-0.2.1.tar` & `osemosys2iamc-0.2a2.tar`

### file list

```diff
@@ -1,50 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:32:33.477813 osemosys2iamc-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:32:33.473813 osemosys2iamc-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:32:33.473813 osemosys2iamc-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-12 08:32:33.477813 osemosys2iamc-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-12 08:32:33.477813 osemosys2iamc-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:32:33.473813 osemosys2iamc-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:32:33.473813 osemosys2iamc-0.2.1/src/osemosys2iamc/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/src/osemosys2iamc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/src/osemosys2iamc/resultify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:32:33.477813 osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-12 08:32:33.000000 osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-12 08:32:33.000000 osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:32:33.000000 osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 08:32:33.000000 osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:32:33.000000 osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-12 08:32:33.000000 osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 08:32:33.000000 osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:32:33.477813 osemosys2iamc-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:32:33.477813 osemosys2iamc-0.2.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/AnnualTechnologyEmissions.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/Demand.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/ProductionByTechnologyAnnual.csv
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/TotalCapacityAnnual.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/UseByTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/VariableCost.csv
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/config_input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/config_result.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/config_result_capture.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:32:33.477813 osemosys2iamc-0.2.1/tests/fixtures/trade/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/trade/ProductionByTechnologyAnnual.csv
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/trade/UseByTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/fixtures/trade/config_trade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tests/test_resultify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-12 08:32:19.000000 osemosys2iamc-0.2.1/tox.ini
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.506636 osemosys2iamc-0.2a2/
+-rw-r--r--   0 wusher     (501) staff       (20)      596 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/.coveragerc
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.466470 osemosys2iamc-0.2a2/.github/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.476819 osemosys2iamc-0.2a2/.github/workflows/
+-rw-r--r--   0 wusher     (501) staff       (20)      911 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/.github/workflows/pytest.yml
+-rw-r--r--   0 wusher     (501) staff       (20)     1111 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/.github/workflows/python-publish.yml
+-rw-r--r--   0 wusher     (501) staff       (20)      653 2022-12-14 13:36:48.000000 osemosys2iamc-0.2a2/.gitignore
+-rw-r--r--   0 wusher     (501) staff       (20)      261 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/.pre-commit-config.yaml
+-rw-r--r--   0 wusher     (501) staff       (20)       99 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/AUTHORS.rst
+-rw-r--r--   0 wusher     (501) staff       (20)      111 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/CHANGELOG.rst
+-rw-r--r--   0 wusher     (501) staff       (20)    12790 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/CONTRIBUTING.rst
+-rwxr-xr-x   0 wusher     (501) staff       (20)     1090 2022-12-14 13:36:48.000000 osemosys2iamc-0.2a2/LICENSE.txt
+-rw-r--r--   0 wusher     (501) staff       (20)     8782 2023-07-11 10:54:24.507135 osemosys2iamc-0.2a2/PKG-INFO
+-rw-r--r--   0 wusher     (501) staff       (20)     8175 2023-07-11 10:53:16.000000 osemosys2iamc-0.2a2/README.md
+-rw-r--r--   0 wusher     (501) staff       (20)      355 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/pyproject.toml
+-rw-r--r--   0 wusher     (501) staff       (20)       99 2023-07-11 10:22:07.000000 osemosys2iamc-0.2a2/requirements.txt
+-rw-r--r--   0 wusher     (501) staff       (20)     1543 2023-07-11 10:54:24.508928 osemosys2iamc-0.2a2/setup.cfg
+-rw-r--r--   0 wusher     (501) staff       (20)      710 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/setup.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.468272 osemosys2iamc-0.2a2/src/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.478378 osemosys2iamc-0.2a2/src/openentrance/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.467251 osemosys2iamc-0.2a2/src/openentrance/definitions/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.467458 osemosys2iamc-0.2a2/src/openentrance/definitions/region/
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.480535 osemosys2iamc-0.2a2/src/openentrance/definitions/region/data/
+-rw-r--r--   0 wusher     (501) staff       (20)     1113 2022-07-13 12:47:35.000000 osemosys2iamc-0.2a2/src/openentrance/definitions/region/data/write-countries.py
+-rw-r--r--   0 wusher     (501) staff       (20)     2250 2022-07-13 12:47:35.000000 osemosys2iamc-0.2a2/src/openentrance/definitions/region/data/write-nuts.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.481503 osemosys2iamc-0.2a2/src/openentrance/openentrance/
+-rw-r--r--   0 wusher     (501) staff       (20)     1559 2023-05-05 09:56:45.000000 osemosys2iamc-0.2a2/src/openentrance/openentrance/__init__.py
+-rw-r--r--   0 wusher     (501) staff       (20)       58 2022-07-13 12:47:35.000000 osemosys2iamc-0.2a2/src/openentrance/setup.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.484136 osemosys2iamc-0.2a2/src/openentrance/tests/
+-rw-r--r--   0 wusher     (501) staff       (20)      414 2022-07-13 12:47:35.000000 osemosys2iamc-0.2a2/src/openentrance/tests/test_core.py
+-rw-r--r--   0 wusher     (501) staff       (20)     1801 2023-05-05 09:56:45.000000 osemosys2iamc-0.2a2/src/openentrance/tests/test_definitions.py
+-rw-r--r--   0 wusher     (501) staff       (20)     2690 2023-05-05 09:56:45.000000 osemosys2iamc-0.2a2/src/openentrance/tests/test_validate.py
+-rwxr-xr-x   0 wusher     (501) staff       (20)     3103 2023-05-05 09:56:45.000000 osemosys2iamc-0.2a2/src/openentrance/workflow.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.485928 osemosys2iamc-0.2a2/src/osemosys2iamc/
+-rw-r--r--   0 wusher     (501) staff       (20)      577 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/src/osemosys2iamc/__init__.py
+-rw-r--r--   0 wusher     (501) staff       (20)    18663 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/src/osemosys2iamc/resultify.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.491325 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/
+-rw-r--r--   0 wusher     (501) staff       (20)     8782 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/PKG-INFO
+-rw-r--r--   0 wusher     (501) staff       (20)     1329 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/SOURCES.txt
+-rw-r--r--   0 wusher     (501) staff       (20)        1 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/dependency_links.txt
+-rw-r--r--   0 wusher     (501) staff       (20)       70 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/entry_points.txt
+-rw-r--r--   0 wusher     (501) staff       (20)        1 2023-07-11 10:54:23.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/not-zip-safe
+-rw-r--r--   0 wusher     (501) staff       (20)      127 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/requires.txt
+-rw-r--r--   0 wusher     (501) staff       (20)       27 2023-07-11 10:54:24.000000 osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/top_level.txt
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.495243 osemosys2iamc-0.2a2/tests/
+-rw-r--r--   0 wusher     (501) staff       (20)      281 2022-07-08 07:04:39.000000 osemosys2iamc-0.2a2/tests/conftest.py
+drwxr-xr-x   0 wusher     (501) staff       (20)        0 2023-07-11 10:54:24.505906 osemosys2iamc-0.2a2/tests/fixtures/
+-rw-r--r--   0 wusher     (501) staff       (20)      733 2022-04-06 09:10:17.000000 osemosys2iamc-0.2a2/tests/fixtures/AnnualTechnologyEmissions.csv
+-rw-r--r--   0 wusher     (501) staff       (20)     1295 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/Demand.csv
+-rw-r--r--   0 wusher     (501) staff       (20)     1320 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/ProductionByTechnologyAnnual.csv
+-rw-r--r--   0 wusher     (501) staff       (20)      481 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/TotalCapacityAnnual.csv
+-rw-r--r--   0 wusher     (501) staff       (20)     1480 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/UseByTechnology.csv
+-rw-r--r--   0 wusher     (501) staff       (20)      453 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/fixtures/VariableCost.csv
+-rw-r--r--   0 wusher     (501) staff       (20)      345 2023-07-11 10:22:07.000000 osemosys2iamc-0.2a2/tests/fixtures/config_input.yaml
+-rw-r--r--   0 wusher     (501) staff       (20)      325 2023-07-11 10:22:07.000000 osemosys2iamc-0.2a2/tests/fixtures/config_result.yaml
+-rw-r--r--   0 wusher     (501) staff       (20)      380 2023-07-11 10:22:07.000000 osemosys2iamc-0.2a2/tests/fixtures/config_result_capture.yaml
+-rw-r--r--   0 wusher     (501) staff       (20)      741 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/test_cli.py
+-rw-r--r--   0 wusher     (501) staff       (20)     3682 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/test_main.py
+-rw-r--r--   0 wusher     (501) staff       (20)    20554 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tests/test_resultify.py
+-rw-r--r--   0 wusher     (501) staff       (20)     2553 2023-07-11 10:53:11.000000 osemosys2iamc-0.2a2/tox.ini
```

### Comparing `osemosys2iamc-0.2.1/.coveragerc` & `osemosys2iamc-0.2a2/.coveragerc`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/.github/workflows/pytest.yml` & `osemosys2iamc-0.2a2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/.github/workflows/python-publish.yml` & `osemosys2iamc-0.2a2/.github/workflows/python-publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 permissions:
   contents: read
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
-    environment: release
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
```

### Comparing `osemosys2iamc-0.2.1/.gitignore` & `osemosys2iamc-0.2a2/.gitignore`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/CONTRIBUTING.rst` & `osemosys2iamc-0.2a2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/LICENSE.txt` & `osemosys2iamc-0.2a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/PKG-INFO` & `osemosys2iamc-0.2a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osemosys2iamc
-Version: 0.2.1
+Version: 0.2a2
 Summary: A utility package to convert OSeMOSYS results into IAMC format
 Home-page: https://github.com/osemosys/osemosys2iamc/
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Source, https://github.com/osemosys/osemosys2iamc/
 Project-URL: Tracker, https://github.com/osemosys/osemosys2iamc/issues
@@ -14,24 +14,19 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # osemosys2iamc
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7473185.svg)](https://doi.org/10.5281/zenodo.7473185)
-
 Convert OSeMOSYS results to IAMC format
 
 ## Acknowledgements
 
-This work was financially supported by:
-
-- The European Union’s Horizon 2020 research and innovation programme under the grant agreement No 101022622 ([European Climate and Energy Modelling Forum ECEMF](https://doi.org/10.3030/101022622))
-- The [IAM COMPACT](https://doi.org/10.3030/101056306) project has received funding from the European Union’s HORIZON EUROPE Research and Innovation Programme under grant agreement No 101056306
+This work was financially supported by the European Union’s Horizon 2020 research and innovation programme under the grant agreement No 101022622 ([European Climate and Energy Modelling Forum ECEMF](https://doi.org/10.3030/101022622)).
 
 ## Install from Github repository
 
     pip install git+https://github.com/osemosys/osemosys2iamc@main#egg=osemosys2iamc
 
 ## Run the package
```

### Comparing `osemosys2iamc-0.2.1/README.md` & `osemosys2iamc-0.2a2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 # osemosys2iamc
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7473185.svg)](https://doi.org/10.5281/zenodo.7473185)
-
 Convert OSeMOSYS results to IAMC format
 
 ## Acknowledgements
 
-This work was financially supported by:
-
-- The European Union’s Horizon 2020 research and innovation programme under the grant agreement No 101022622 ([European Climate and Energy Modelling Forum ECEMF](https://doi.org/10.3030/101022622))
-- The [IAM COMPACT](https://doi.org/10.3030/101056306) project has received funding from the European Union’s HORIZON EUROPE Research and Innovation Programme under grant agreement No 101056306
+This work was financially supported by the European Union’s Horizon 2020 research and innovation programme under the grant agreement No 101022622 ([European Climate and Energy Modelling Forum ECEMF](https://doi.org/10.3030/101022622)).
 
 ## Install from Github repository
 
     pip install git+https://github.com/osemosys/osemosys2iamc@main#egg=osemosys2iamc
 
 ## Run the package
```

### Comparing `osemosys2iamc-0.2.1/setup.cfg` & `osemosys2iamc-0.2a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/setup.py` & `osemosys2iamc-0.2a2/setup.py`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/src/osemosys2iamc/__init__.py` & `osemosys2iamc-0.2a2/src/osemosys2iamc/__init__.py`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/src/osemosys2iamc/resultify.py` & `osemosys2iamc-0.2a2/src/osemosys2iamc/resultify.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,14 @@
 import os
 from typing import List, Dict, Optional
 from yaml import load, SafeLoader
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 import re
 
-# Creates an alias for United Kingdom and Greece using alternate 2-letter code
-# (see issue https://github.com/OSeMOSYS/osemosys2iamc/issues/33)
-countries_by_alpha2["UK"] = countries_by_alpha2["GB"]
-countries_by_alpha2["EL"] = countries_by_alpha2["GR"]
-
 
 def iso_to_country(
     iso_format: str, index: List[str], osemosys_param: str
 ) -> pd.DataFrame:
     """Reads in selected CSV file and applies chosen region naming convention
 
     Uses naming convention as given in the config file into a Pandas DataFrame
@@ -53,15 +48,15 @@
     List[str]
     """
     countries_list = []
     no_country_extracted = []
     format_regex = r"^iso[23]_([1-9]\d*|start|end)$"
 
     # Verifies that given format is the expected format; Raises an error if expectation not met
-    if re.search(format_regex, iso_format) is not None:
+    if re.search(format_regex, iso_format) != None:
 
         iso_type, abbr_loc = iso_format[3:].split("_")
 
         # Assigns the correct dictionary to search based on iso type
         if iso_type == "2":
             country_dict = countries_by_alpha2
         elif iso_type == "3":
@@ -76,22 +71,22 @@
             region_regex = (
                 r"^.{" + str(int(abbr_loc) - 1) + r"}(.{" + iso_type + r"}).*$"
             )
 
         """
         Checks every technology/fuel name for a valid code. If found,
         adds that country to the list for that tech/fuel name, otherwise
-        adds an empty string for that tech/fuel. A position exceeding the
+        adds an empty string for that tech/fuel. A position exceeeding the
         length of the name, adds an empty string instead
         """
         for i in index:
             if re.search(region_regex, i.upper()) != None:
                 code = re.search(region_regex, i.upper()).groups()[0]
                 if code in country_dict:
-                    countries_list.append(country_dict[code].name)
+                    countries_list.append(country_dict[code].name.upper())
                 else:
                     countries_list.append("")
                     no_country_extracted.append(i)
             else:
                 countries_list.append("")
                 no_country_extracted.append(i)
 
@@ -432,15 +427,15 @@
                 blob.append(iamc)
     except KeyError:
         pass
 
     try:
         for result in config["results"]:
 
-            if isinstance(result["osemosys_param"], str):
+            if type(result["osemosys_param"]) == str:
                 results = read_file(
                     results_path, result["osemosys_param"], config["region"]
                 )
 
                 try:
                     technologies = result["technology"]
                 except KeyError:
@@ -471,33 +466,23 @@
                     data = filter_capacity(results, technologies)
                 elif "demand" in result.keys():
                     demands = result["demand"]
                     data = filter_final_energy(results, demands)
                 else:
                     data = extract_results(results, technologies)
 
-            elif isinstance(result["osemosys_param"], list):
+            else:
                 results = {}
-                unit = result["unit"]
                 for p in result["osemosys_param"]:
-                    results[p] = read_file(results_path, p, config["region"])
-
+                    path_name = os.path.join(results_path, p + ".csv")
+                    results[p] = read_file(path_name)
                 if "trade_tech" in result.keys():
                     technologies = result["trade_tech"]
                     data = calculate_trade(results, technologies)
 
-                else:
-                    name = result["iamc_variable"]
-                    raise ValueError(f"No data found for {name}")
-
-            else:
-                name = result["iamc_variable"]
-                msg = f"Error in configuration file for entry {name}. The `osemosys_param` key must be a string or a list"
-                raise ValueError(msg)
-
             if "transform" in result.keys():
                 if result["transform"] == "abs":
                     data["VALUE"] = data["VALUE"].abs()
                 else:
                     pass
 
             if not data.empty:
@@ -512,26 +497,23 @@
                     variable=result["iamc_variable"],
                     unit=unit,
                 )
                 blob.append(iamc)
     except KeyError:
         pass
 
-    if len(blob) > 0:
-        all_data = pyam.concat(blob)
+    all_data = pyam.concat(blob)
 
-        all_data = all_data.convert_unit("PJ/yr", to="EJ/yr")
-        all_data = all_data.convert_unit("ktCO2/yr", to="Mt CO2/yr", factor=0.001)
-        all_data = all_data.convert_unit("MEUR_2015/PJ", to="EUR_2020/GJ", factor=1.05)
-        all_data = all_data.convert_unit("kt CO2/yr", to="Mt CO2/yr")
+    all_data = all_data.convert_unit("PJ/yr", to="EJ/yr")
+    all_data = all_data.convert_unit("ktCO2/yr", to="Mt CO2/yr", factor=0.001)
+    all_data = all_data.convert_unit("MEUR_2015/PJ", to="EUR_2020/GJ", factor=1.05)
+    all_data = all_data.convert_unit("kt CO2/yr", to="Mt CO2/yr")
 
-        all_data = pyam.IamDataFrame(all_data)
-        return all_data
-    else:
-        raise ValueError("No data found")
+    all_data = pyam.IamDataFrame(all_data)
+    return all_data
 
 
 def aggregate(func):
     """Decorator for filters which returns the aggregated data"""
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
```

### Comparing `osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/PKG-INFO` & `osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osemosys2iamc
-Version: 0.2.1
+Version: 0.2a2
 Summary: A utility package to convert OSeMOSYS results into IAMC format
 Home-page: https://github.com/osemosys/osemosys2iamc/
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Source, https://github.com/osemosys/osemosys2iamc/
 Project-URL: Tracker, https://github.com/osemosys/osemosys2iamc/issues
@@ -14,24 +14,19 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # osemosys2iamc
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7473185.svg)](https://doi.org/10.5281/zenodo.7473185)
-
 Convert OSeMOSYS results to IAMC format
 
 ## Acknowledgements
 
-This work was financially supported by:
-
-- The European Union’s Horizon 2020 research and innovation programme under the grant agreement No 101022622 ([European Climate and Energy Modelling Forum ECEMF](https://doi.org/10.3030/101022622))
-- The [IAM COMPACT](https://doi.org/10.3030/101056306) project has received funding from the European Union’s HORIZON EUROPE Research and Innovation Programme under grant agreement No 101056306
+This work was financially supported by the European Union’s Horizon 2020 research and innovation programme under the grant agreement No 101022622 ([European Climate and Energy Modelling Forum ECEMF](https://doi.org/10.3030/101022622)).
 
 ## Install from Github repository
 
     pip install git+https://github.com/osemosys/osemosys2iamc@main#egg=osemosys2iamc
 
 ## Run the package
```

### Comparing `osemosys2iamc-0.2.1/src/osemosys2iamc.egg-info/SOURCES.txt` & `osemosys2iamc-0.2a2/src/osemosys2iamc.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/pytest.yml
 .github/workflows/python-publish.yml
+src/openentrance/setup.py
+src/openentrance/workflow.py
+src/openentrance/definitions/region/data/write-countries.py
+src/openentrance/definitions/region/data/write-nuts.py
+src/openentrance/openentrance/__init__.py
+src/openentrance/tests/test_core.py
+src/openentrance/tests/test_definitions.py
+src/openentrance/tests/test_validate.py
 src/osemosys2iamc/__init__.py
 src/osemosys2iamc/resultify.py
 src/osemosys2iamc.egg-info/PKG-INFO
 src/osemosys2iamc.egg-info/SOURCES.txt
 src/osemosys2iamc.egg-info/dependency_links.txt
 src/osemosys2iamc.egg-info/entry_points.txt
 src/osemosys2iamc.egg-info/not-zip-safe
@@ -30,11 +38,8 @@
 tests/fixtures/Demand.csv
 tests/fixtures/ProductionByTechnologyAnnual.csv
 tests/fixtures/TotalCapacityAnnual.csv
 tests/fixtures/UseByTechnology.csv
 tests/fixtures/VariableCost.csv
 tests/fixtures/config_input.yaml
 tests/fixtures/config_result.yaml
-tests/fixtures/config_result_capture.yaml
-tests/fixtures/trade/ProductionByTechnologyAnnual.csv
-tests/fixtures/trade/UseByTechnology.csv
-tests/fixtures/trade/config_trade.yaml
+tests/fixtures/config_result_capture.yaml
```

### Comparing `osemosys2iamc-0.2.1/tests/fixtures/AnnualTechnologyEmissions.csv` & `osemosys2iamc-0.2a2/tests/fixtures/AnnualTechnologyEmissions.csv`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/tests/fixtures/Demand.csv` & `osemosys2iamc-0.2a2/tests/fixtures/Demand.csv`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/tests/fixtures/ProductionByTechnologyAnnual.csv` & `osemosys2iamc-0.2a2/tests/fixtures/ProductionByTechnologyAnnual.csv`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/tests/fixtures/UseByTechnology.csv` & `osemosys2iamc-0.2a2/tests/fixtures/UseByTechnology.csv`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/tests/test_cli.py` & `osemosys2iamc-0.2a2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osemosys2iamc-0.2.1/tests/test_main.py` & `osemosys2iamc-0.2a2/tests/test_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     with open(config, "r") as config_file:
         config = load(config_file, Loader=SafeLoader)
 
     actual = main(config, inputs, results)
 
     data = pd.DataFrame(
         [
-            ["Austria", "Price|Primary Energy|Biomass", 2015, 3.15],
-            ["Austria", "Price|Primary Energy|Biomass", 2016, 4.2],
-            ["Belgium", "Price|Primary Energy|Biomass", 2015, 1.785],
-            ["Belgium", "Price|Primary Energy|Biomass", 2016, 1.890],
+            ["AUSTRIA", "Price|Primary Energy|Biomass", 2015, 3.15],
+            ["AUSTRIA", "Price|Primary Energy|Biomass", 2016, 4.2],
+            ["BELGIUM", "Price|Primary Energy|Biomass", 2015, 1.785],
+            ["BELGIUM", "Price|Primary Energy|Biomass", 2016, 1.890],
         ],
         columns=["region", "variable", "year", "value"],
     )
 
     expected = IamDataFrame(
         data,
         model="OSeMBE v1.0.0",
@@ -46,26 +46,26 @@
     with open(config, "r") as config_file:
         config = load(config_file, Loader=SafeLoader)
 
     actual = main(config, inputs, results)
 
     data = pd.DataFrame(
         [
-            ["Austria", "Capacity|Electricity", 2015, 0.446776],
-            ["Belgium", "Capacity|Electricity", 2016, 0.184866],
-            ["Bulgaria", "Capacity|Electricity", 2015, 4.141],
-            ["Cyprus", "Capacity|Electricity", 2015, 0.3904880555817921],
-            ["Czechia", "Capacity|Electricity", 2015, 0.299709],
-            ["Denmark", "Capacity|Electricity", 2015, 0.0005],
-            ["Estonia", "Capacity|Electricity", 2015, 0.006],
-            ["Finland", "Capacity|Electricity", 2015, 0.0263],
-            ["France", "Capacity|Electricity", 2015, 0.47835],
-            ["Germany", "Capacity|Electricity", 2015, 9.62143],
-            ["Spain", "Capacity|Electricity", 2015, 7.7308],
-            ["Switzerland", "Capacity|Electricity", 2026, 0.004563975391582646],
+            ["AUSTRIA", "Capacity|Electricity", 2015, 0.446776],
+            ["BELGIUM", "Capacity|Electricity", 2016, 0.184866],
+            ["BULGARIA", "Capacity|Electricity", 2015, 4.141],
+            ["CYPRUS", "Capacity|Electricity", 2015, 0.3904880555817921],
+            ["CZECHIA", "Capacity|Electricity", 2015, 0.299709],
+            ["DENMARK", "Capacity|Electricity", 2015, 0.0005],
+            ["ESTONIA", "Capacity|Electricity", 2015, 0.006],
+            ["FINLAND", "Capacity|Electricity", 2015, 0.0263],
+            ["FRANCE", "Capacity|Electricity", 2015, 0.47835],
+            ["GERMANY", "Capacity|Electricity", 2015, 9.62143],
+            ["SPAIN", "Capacity|Electricity", 2015, 7.7308],
+            ["SWITZERLAND", "Capacity|Electricity", 2026, 0.004563975391582646],
         ],
         columns=["region", "variable", "year", "value"],
     )
 
     expected = IamDataFrame(
         data, model="OSeMBE v1.0.0", scenario="DIAG-C400-lin-ResidualFossil", unit="GW"
     )
@@ -88,66 +88,23 @@
     with open(config, "r") as config_file:
         config = load(config_file, Loader=SafeLoader)
 
     actual = main(config, inputs, results)
 
     data = pd.DataFrame(
         [
-            ["Austria", "Carbon Capture|Biomass", 2026, 7.573069442598169],
-            ["Austria", "Carbon Capture|Biomass", 2027, 7.766777427515737],
-            ["Belgium", "Carbon Capture|Biomass", 2026, 2.24498280006968],
-            ["Belgium", "Carbon Capture|Biomass", 2027, 6.746886436926597],
+            ["AUSTRIA", "Carbon Capture|Biomass", 2026, 7.573069442598169],
+            ["AUSTRIA", "Carbon Capture|Biomass", 2027, 7.766777427515737],
+            ["BELGIUM", "Carbon Capture|Biomass", 2026, 2.24498280006968],
+            ["BELGIUM", "Carbon Capture|Biomass", 2027, 6.746886436926597],
         ],
         columns=["region", "variable", "year", "value"],
     )
 
     expected = IamDataFrame(
         data,
         model="OSeMBE v1.0.0",
         scenario="DIAG-C400-lin-ResidualFossil",
         unit="Mt CO2/yr",
     )
 
     assert_iamframe_equal(actual, expected)
-
-
-def test_main_trade():
-    """Test operation of trade filter
-
-    Config
-    ------
-        - iamc_variable: Trade|Secondary Energy|Electricity|Volume
-          osemosys_param:
-          - UseByTechnology
-          - ProductionByTechnologyAnnual
-          trade_tech:
-          - (?=^.{2}(EL))^((?!00).)*$
-          unit: PJ/yr
-
-    """
-
-    config_path = os.path.join("tests", "fixtures", "trade", "config_trade.yaml")
-    inputs_path = os.path.join("tests", "fixtures", "trade")
-    results_path = os.path.join("tests", "fixtures", "trade")
-
-    with open(config_path, "r") as config_file:
-        config = load(config_file, Loader=SafeLoader)
-
-    actual = main(config, inputs_path, results_path)
-
-    data = pd.DataFrame(
-        [
-            ["Austria", "Trade|Secondary Energy|Electricity|Volume", 2010, -0.024824],
-            ["Austria", "Trade|Secondary Energy|Electricity|Volume", 2011, -0.024924],
-            ["Austria", "Trade|Secondary Energy|Electricity|Volume", 2012, -0.025024],
-        ],
-        columns=["region", "variable", "year", "value"],
-    )
-
-    expected = IamDataFrame(
-        data,
-        model="OSeMBE v1.0.0",
-        scenario="DIAG-C400-lin-ResidualFossil",
-        unit="EJ/yr",
-    )
-
-    assert_iamframe_equal(actual, expected)
```

### Comparing `osemosys2iamc-0.2.1/tests/test_resultify.py` & `osemosys2iamc-0.2a2/tests/test_resultify.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,24 +57,24 @@
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "AnnualTechnologyEmissions", "iso2_start")
 
         emission = ["CO2"]
         actual = filter_emission_tech(input_data, emission)
 
         data = [
-            ["Austria", 2026, -6244.862561],
-            ["Austria", 2027, -6529.532083],
-            ["Austria", 2030, 3043.148835],
-            ["Austria", 2031, 2189.064681],
-            ["Austria", 2032, 2315.821267],
-            ["Belgium", 2026, -2244.982800],
-            ["Belgium", 2027, -6746.886437],
-            ["Bulgaria", 2030, 11096.556931],
-            ["Bulgaria", 2031, 11069.257141],
-            ["Bulgaria", 2032, 11041.957354],
+            ["AUSTRIA", 2026, -6244.862561],
+            ["AUSTRIA", 2027, -6529.532083],
+            ["AUSTRIA", 2030, 3043.148835],
+            ["AUSTRIA", 2031, 2189.064681],
+            ["AUSTRIA", 2032, 2315.821267],
+            ["BELGIUM", 2026, -2244.982800],
+            ["BELGIUM", 2027, -6746.886437],
+            ["BULGARIA", 2030, 11096.556931],
+            ["BULGARIA", 2031, 11069.257141],
+            ["BULGARIA", 2032, 11041.957354],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_tech_emission(self):
@@ -83,18 +83,18 @@
         input_data = read_file(folderpath, "AnnualTechnologyEmissions", "iso2_start")
 
         tech = ["(?=^.{2}(BM))^.{4}(CS)"]
         emission = ["CO2"]
         actual = filter_emission_tech(input_data, emission, tech)
 
         data = [
-            ["Austria", 2026, -7573.069442598169],
-            ["Austria", 2027, -7766.777427515737],
-            ["Belgium", 2026, -2244.98280006968],
-            ["Belgium", 2027, -6746.886436926597],
+            ["AUSTRIA", 2026, -7573.069442598169],
+            ["AUSTRIA", 2027, -7766.777427515737],
+            ["BELGIUM", 2026, -2244.98280006968],
+            ["BELGIUM", 2027, -6746.886436926597],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
         print(actual)
         print(expected)
         pd.testing.assert_frame_equal(actual, expected)
 
@@ -133,188 +133,188 @@
             "^.{2}(OC)",
             "^.{2}(SO)",
             "^.{2}(WI)",
         ]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Austria", 2015, 26.324108350683794],
-            ["Austria", 2016, 26.324108350683794],
-            ["Austria", 2017, 26.324108350683794],
-            ["Austria", 2018, 26.324108350683787],
-            ["Austria", 2019, 26.324108350683794],
-            ["Belgium", 2016, 141.0],
-            ["Bulgaria", 2015, 1.423512],
-            ["Czechia", 2015, 329.5950809],
-            ["Denmark", 2015, 0.0031536],
-            ["Estonia", 2015, 28.512108],
-            ["Finland", 2015, 0.296581102],
-            ["France", 2015, 72.25974846],
-            ["Spain", 2015, 26.75595496],
-            ["Switzerland", 2047, 69.9750212433476],
-            ["Switzerland", 2048, 91.45662886581975],
-            ["Switzerland", 2049, 76.86770297185006],
-            ["Switzerland", 2050, 70.86078033897608],
-            ["Switzerland", 2051, 53.88447040760964],
+            ["AUSTRIA", 2015, 26.324108350683794],
+            ["AUSTRIA", 2016, 26.324108350683794],
+            ["AUSTRIA", 2017, 26.324108350683794],
+            ["AUSTRIA", 2018, 26.324108350683787],
+            ["AUSTRIA", 2019, 26.324108350683794],
+            ["BELGIUM", 2016, 141.0],
+            ["BULGARIA", 2015, 1.423512],
+            ["CZECHIA", 2015, 329.5950809],
+            ["DENMARK", 2015, 0.0031536],
+            ["ESTONIA", 2015, 28.512108],
+            ["FINLAND", 2015, 0.296581102],
+            ["FRANCE", 2015, 72.25974846],
+            ["SPAIN", 2015, 26.75595496],
+            ["SWITZERLAND", 2047, 69.9750212433476],
+            ["SWITZERLAND", 2048, 91.45662886581975],
+            ["SWITZERLAND", 2049, 76.86770297185006],
+            ["SWITZERLAND", 2050, 70.86078033897608],
+            ["SWITZERLAND", 2051, 53.88447040760964],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_bm(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["(?=^.{2}(BM))^.{4}(00)", "(?=^.{2}(WS))^.{4}(00)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Austria", 2015, 26.324108350683794],
-            ["Austria", 2016, 26.324108350683794],
-            ["Austria", 2017, 26.324108350683794],
-            ["Austria", 2018, 26.324108350683787],
-            ["Austria", 2019, 26.324108350683794],
+            ["AUSTRIA", 2015, 26.324108350683794],
+            ["AUSTRIA", 2016, 26.324108350683794],
+            ["AUSTRIA", 2017, 26.324108350683794],
+            ["AUSTRIA", 2018, 26.324108350683787],
+            ["AUSTRIA", 2019, 26.324108350683794],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_co(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["(?=^.{2}(CO))^.{4}(00)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Switzerland", 2047, 69.9750212433476],
-            ["Switzerland", 2048, 91.45662886581975],
-            ["Switzerland", 2049, 76.86770297185006],
-            ["Switzerland", 2050, 70.86078033897608],
-            ["Switzerland", 2051, 53.88447040760964],
+            ["SWITZERLAND", 2047, 69.9750212433476],
+            ["SWITZERLAND", 2048, 91.45662886581975],
+            ["SWITZERLAND", 2049, 76.86770297185006],
+            ["SWITZERLAND", 2050, 70.86078033897608],
+            ["SWITZERLAND", 2051, 53.88447040760964],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_ng(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["(?=^.{2}(NG))^.{4}(00)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Belgium", 2016, 141.0],
+            ["BELGIUM", 2016, 141.0],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_go(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["(?=^.{2}(GO))^.{4}(00)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Bulgaria", 2015, 1.423512],
+            ["BULGARIA", 2015, 1.423512],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_hy(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["^.{2}(HY)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Czechia", 2015, 3.3637616987287244],
+            ["CZECHIA", 2015, 3.3637616987287244],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_nu(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["^.{2}(UR)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Czechia", 2015, 326.2313192401038],
+            ["CZECHIA", 2015, 326.2313192401038],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_oc(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["^.{2}(OC)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Denmark", 2015, 0.0031536000000000003],
+            ["DENMARK", 2015, 0.0031536000000000003],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_oi(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["(?=^.{2}(OI))^.{4}(00)", "(?=^.{2}(HF))^.{4}(00)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Estonia", 2015, 28.512107999999998],
+            ["ESTONIA", 2015, 28.512107999999998],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_so(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["^.{2}(SO)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Spain", 2015, 26.75595496070811],
+            ["SPAIN", 2015, 26.75595496070811],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_primary_wi(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "ProductionByTechnologyAnnual", "iso2_start")
 
         technologies = ["^.{2}(WI)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Finland", 2015, 0.29658110158442175],
-            ["France", 2015, 72.25974845531343],
+            ["FINLAND", 2015, 0.29658110158442175],
+            ["FRANCE", 2015, 72.25974845531343],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_secondary_bm(self):
@@ -325,35 +325,35 @@
             "(?=^.{2}(BF))^((?!00).)*$",
             "(?=^.{2}(BM))^((?!00).)*$",
             "(?=^.{2}(WS))^((?!00).)*$",
         ]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Austria", 2042, 0.6636346353894057],
-            ["Austria", 2043, 1.3300518531620575],
-            ["Austria", 2044, 1.9992691432067637],
-            ["Austria", 2045, 2.6713041901899794],
-            ["Austria", 2046, 3.4778527409137996],
+            ["AUSTRIA", 2042, 0.6636346353894057],
+            ["AUSTRIA", 2043, 1.3300518531620575],
+            ["AUSTRIA", 2044, 1.9992691432067637],
+            ["AUSTRIA", 2045, 2.6713041901899794],
+            ["AUSTRIA", 2046, 3.4778527409137996],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_final_energy(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "Demand", "iso2_start")
 
         fuels = ["^.*E2$"]
         actual = filter_final_energy(input_data, fuels)
 
         data = [
-            ["Austria", 2015, 227.5944502],
-            ["Belgium", 2016, 296.0570016],
+            ["AUSTRIA", 2015, 227.5944502],
+            ["BELGIUM", 2016, 296.0570016],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         print(actual)
         print(expected)
 
@@ -364,26 +364,26 @@
     def test_filter_inst_capacity(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["^((?!(EL)|(00)).)*$"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Austria", 2015, 0.446776],
-            ["Belgium", 2016, 0.184866],
-            ["Bulgaria", 2015, 4.141],
-            ["Cyprus", 2015, 0.3904880555817921],
-            ["Czechia", 2015, 0.299709],
-            ["Denmark", 2015, 0.0005],
-            ["Estonia", 2015, 0.006],
-            ["Finland", 2015, 0.0263],
-            ["France", 2015, 0.47835],
-            ["Germany", 2015, 9.62143],
-            ["Spain", 2015, 7.7308],
-            ["Switzerland", 2026, 0.004563975391582646],
+            ["AUSTRIA", 2015, 0.446776],
+            ["BELGIUM", 2016, 0.184866],
+            ["BULGARIA", 2015, 4.141],
+            ["CYPRUS", 2015, 0.3904880555817921],
+            ["CZECHIA", 2015, 0.299709],
+            ["DENMARK", 2015, 0.0005],
+            ["ESTONIA", 2015, 0.006],
+            ["FINLAND", 2015, 0.0263],
+            ["FRANCE", 2015, 0.47835],
+            ["GERMANY", 2015, 9.62143],
+            ["SPAIN", 2015, 7.7308],
+            ["SWITZERLAND", 2026, 0.004563975391582646],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         print(actual)
 
         print(expected)
@@ -397,143 +397,143 @@
             "(?=^.{2}(BF))^((?!00).)*$",
             "(?=^.{2}(BM))^((?!00).)*$",
             "(?=^.{2}(WS))^((?!00).)*$",
         ]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Austria", 2015, 0.446776],
-            ["Belgium", 2016, 0.184866],
-            ["France", 2015, 0.47835],
+            ["AUSTRIA", 2015, 0.446776],
+            ["BELGIUM", 2016, 0.184866],
+            ["FRANCE", 2015, 0.47835],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_inst_capacity_coal(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["(?=^.{2}(CO))^((?!00).)*$"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Bulgaria", 2015, 4.141],
+            ["BULGARIA", 2015, 4.141],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_inst_capacity_gas(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["(?=^.{2}(NG))^((?!00).)*$"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Germany", 2015, 9.62143],
+            ["GERMANY", 2015, 9.62143],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_inst_capacity_geo(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["(?=^.{2}(GO))^((?!00).)*$"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Switzerland", 2026, 0.004563975391582646],
+            ["SWITZERLAND", 2026, 0.004563975391582646],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_inst_capacity_hydro(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["^.{2}(HY)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Czechia", 2015, 0.299709],
+            ["CZECHIA", 2015, 0.299709],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_inst_capacity_nuclear(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["^.{2}(NU)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Spain", 2015, 7.7308],
+            ["SPAIN", 2015, 7.7308],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_inst_capacity_ocean(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["^.{2}(OC)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Denmark", 2015, 0.0005],
+            ["DENMARK", 2015, 0.0005],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_inst_capacity_oil(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["(?=^.{2}(HF))^((?!00).)*$"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Cyprus", 2015, 0.3904880555817921],
+            ["CYPRUS", 2015, 0.3904880555817921],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_inst_capacity_solar(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["^.{2}(SO)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Estonia", 2015, 0.006],
+            ["ESTONIA", 2015, 0.006],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
     def test_filter_inst_capacity_wi_offshore(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "TotalCapacityAnnual", "iso2_start")
         technologies = ["(?=^.{2}(WI))^.{4}(OF)"]
         actual = filter_capacity(input_data, technologies)
 
         data = [
-            ["Finland", 2015, 0.0263],
+            ["FINLAND", 2015, 0.0263],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         pd.testing.assert_frame_equal(actual, expected)
 
 
@@ -541,18 +541,18 @@
     def test_price_bm(self):
         folderpath = os.path.join("tests", "fixtures")
         input_data = read_file(folderpath, "VariableCost", "iso2_start")
         commodity = ["(?=^.{2}(BM))^.{6}(X0)"]
         actual = filter_capacity(input_data, commodity)
 
         data = [
-            ["Austria", 2015, 3.0],
-            ["Austria", 2016, 4.0],
-            ["Belgium", 2015, 1.7],
-            ["Belgium", 2016, 1.8],
+            ["AUSTRIA", 2015, 3.0],
+            ["AUSTRIA", 2016, 4.0],
+            ["BELGIUM", 2015, 1.7],
+            ["BELGIUM", 2016, 1.8],
         ]
 
         expected = pd.DataFrame(data=data, columns=["REGION", "YEAR", "VALUE"])
 
         print(actual)
         print(expected)
 
@@ -561,61 +561,55 @@
 
 class TestCountryConversion:
     def test_iso_to_country_iso2start(self):
         techs = ["NGNGA2", "DENGA2", "NGKENGX", "ZXNGA"]
 
         actual = iso_to_country("iso2_start", techs, "TotalCapacityAnnual")
 
-        expected = ["Nigeria", "Germany", "Nigeria", ""]
+        expected = ["NIGERIA", "GERMANY", "NIGERIA", ""]
 
         assert actual == expected
 
     def test_iso_to_country_iso3start(self):
         techs = ["NGANGA", "BHSHYA", "TCASOA", "ZXNGA"]
 
         actual = iso_to_country("iso3_start", techs, "TotalCapacityAnnual")
 
-        expected = ["Nigeria", "Bahamas", "Turks and Caicos Islands", ""]
+        expected = ["NIGERIA", "BAHAMAS", "TURKS AND CAICOS ISLANDS", ""]
 
         assert actual == expected
 
     def test_iso_to_country_iso2end(self):
         techs = ["NGA2NG", "NGA2DE", "KENGXNG", "NGAZX"]
 
         actual = iso_to_country("iso2_end", techs, "TotalCapacityAnnual")
 
-        expected = ["Nigeria", "Germany", "Nigeria", ""]
+        expected = ["NIGERIA", "GERMANY", "NIGERIA", ""]
 
         assert actual == expected
 
     def test_iso_to_country_iso3end(self):
         techs = ["NGANGA", "HYABHS", "SOATCA", "NGAZX"]
 
         actual = iso_to_country("iso3_end", techs, "TotalCapacityAnnual")
 
-        expected = ["Nigeria", "Bahamas", "Turks and Caicos Islands", ""]
+        expected = ["NIGERIA", "BAHAMAS", "TURKS AND CAICOS ISLANDS", ""]
 
         assert actual == expected
 
     def test_iso_to_country_iso2middle(self):
         techs = ["NGA2NGZZ", "NGA2DEVV", "NGAZXVV", "CZF"]
 
         actual = iso_to_country("iso2_5", techs, "TotalCapacityAnnual")
 
-        expected = ["Nigeria", "Germany", "", ""]
+        expected = ["NIGERIA", "GERMANY", "", ""]
 
         assert actual == expected
 
     def test_iso_to_country_iso3middle(self):
         techs = ["NGANGAGHAPP", "HYABHSLCA", "ABWBMUABC", "NGAZX"]
 
         actual = iso_to_country("iso3_7", techs, "TotalCapacityAnnual")
 
-        expected = ["Ghana", "Saint Lucia", "", ""]
+        expected = ["GHANA", "SAINT LUCIA", "", ""]
 
         assert actual == expected
-
-    def test_iso_to_country_uk(self):
-        techs = ["UKNGA"]
-        actual = iso_to_country("iso2_start", techs, "TotalCapacityAnnual")
-        expected = ["United Kingdom of Great Britain and Northern Ireland"]
-        assert actual == expected
```

### Comparing `osemosys2iamc-0.2.1/tox.ini` & `osemosys2iamc-0.2a2/tox.ini`

 * *Files identical despite different names*

