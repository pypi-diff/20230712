# Comparing `tmp/OpenFisca-Survey-Manager-1.0.1.tar.gz` & `tmp/OpenFisca-Survey-Manager-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Survey-Manager-1.0.1.tar", last modified: Tue Jul 11 09:54:03 2023, max compression
+gzip compressed data, was "OpenFisca-Survey-Manager-1.0.2.tar", last modified: Wed Jul 12 12:01:37 2023, max compression
```

## Comparing `OpenFisca-Survey-Manager-1.0.1.tar` & `OpenFisca-Survey-Manager-1.0.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.933717 OpenFisca-Survey-Manager-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)    17044 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.925717 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      734 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-11 09:54:03.000000 OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-11 09:54:03.933717 OpenFisca-Survey-Manager-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13360 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/
--rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/coicop.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/google_colab.py
--rw-r--r--   0 runner    (1001) docker     (122)    12877 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/input_dataframe_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_dbf.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_spss.py
--rw-r--r--   0 runner    (1001) docker     (122)    79386 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10047 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scripts/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/statshelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5323 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/survey_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 09:54:03.929717 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/data_files/
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/data_files/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_add_survey_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_legislation_inflator.py
--rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_summarize_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_top_bottom_share.py
--rw-r--r--   0 runner    (1001) docker     (122)     8319 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-11 09:54:03.933717 OpenFisca-Survey-Manager-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3155 2023-07-11 09:53:39.000000 OpenFisca-Survey-Manager-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    17279 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.525532 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13360 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/coicop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/google_colab.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13357 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/input_dataframe_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_dbf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_spss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10047 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scripts/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/statshelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/survey_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/data_files/
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8319 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/setup.py
```

### Comparing `OpenFisca-Survey-Manager-1.0.1/CHANGELOG.md` & `OpenFisca-Survey-Manager-1.0.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 ﻿# Changelog
 
+### 1.0.2 [#259](https://github.com/openfisca/openfisca-survey-manager/pull/259)
+
+* Technical changes
+- A parameter `config_files_directory` exist but it is not used evrywhere, this PR generalize it.
+- Add tests using this parameter.
+
 ### 1.0.1 [#257](https://github.com/openfisca/openfisca-survey-manager/pull/257)
 
 * Technical changes
 - In GitHub Actions workflow, fixes the `check-for-functional-changes` → **`deploy`** → `publish-to-conda` jobs sequence
   - Fix the activation of the `deploy` job by fixing how it gets `check-for-functional-changes` output status
   - Allow the activation of `publish-to-conda` job that needs the `deploy` job
 - Add conda configuration files to non functional files for CI
```

### Comparing `OpenFisca-Survey-Manager-1.0.1/LICENSE.AGPL.txt` & `OpenFisca-Survey-Manager-1.0.2/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/PKG-INFO` & `OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/SOURCES.txt` & `OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/OpenFisca_Survey_Manager.egg-info/requires.txt` & `OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 flake8-print<6.0,>=5.0.0
 flake8-rst-docstrings<0.4.0,>=0.3.0
 openfisca-country-template<7,>=6
 pytest<8.0,>=7.2.2
 pytest-cov<5.0,>=4.0.0
 scipy<2.0,>=1.10.1
 tables<4.0,>=3.8.0
+pytest-order<2.0,>=1.1.0
 
 [matching]
 feather
 rpy2<4.0,>=3.5.10
 
 [sas]
 pyreadstat<2.0,>=1.2.1
```

### Comparing `OpenFisca-Survey-Manager-1.0.1/PKG-INFO` & `OpenFisca-Survey-Manager-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.0.1/README.md` & `OpenFisca-Survey-Manager-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/__init__.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/aggregates.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/calibration.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/calmar.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/coicop.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/coicop.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/config.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/google_colab.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/google_colab.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/input_dataframe_generator.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/input_dataframe_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import pandas as pd
 import pkg_resources
 
 
 from openfisca_core import periods
 from openfisca_survey_manager.survey_collections import SurveyCollection
 from openfisca_survey_manager.surveys import Survey
+from openfisca_survey_manager import default_config_files_directory
 
 
 log = logging.getLogger(__name__)
 
 
 def make_input_dataframe_by_entity(tax_benefit_system, nb_persons, nb_groups):
     """Generate a dictionnary of dataframes containing nb_persons persons spread in nb_groups groups.
@@ -176,56 +177,60 @@
     np.random.seed(seed)
     count = len(input_dataframe_by_entity[entity.key])
     value = (np.random.rand(count) * max_value * condition).astype(variable.dtype)
     input_dataframe_by_entity[entity.key][variable_name] = value
 
 
 def set_table_in_survey(input_dataframe, entity, period, collection, survey_name, survey_label = None,
-        table_label = None, table_name = None):
+        table_label = None, table_name = None, config_files_directory = default_config_files_directory):
     period = periods.period(period)
     if table_name is None:
         table_name = entity + '_' + str(period)
     if table_label is None:
         table_label = "Input data for entity {} at period {}".format(entity, period)
     try:
-        survey_collection = SurveyCollection.load(collection = collection)
-    except configparser.NoOptionError:
+        survey_collection = SurveyCollection.load(collection = collection, config_files_directory=config_files_directory)
+    except configparser.NoOptionError as e:
+        log.warning(f"set_table_in_survey configparser.NoOptionError : {e}")
         survey_collection = SurveyCollection(name = collection)
-    except configparser.NoSectionError:  # For tests
+    except configparser.NoSectionError as e:  # For tests
+        log.warning(f"set_table_in_survey configparser.NoSectionError : {e}")
         data_dir = os.path.join(
             pkg_resources.get_distribution('openfisca-survey-manager').location,
             'openfisca_survey_manager',
             'tests',
             'data_files',
             )
         survey_collection = SurveyCollection(
             name = collection,
             config_files_directory = data_dir,
             )
 
     try:
         survey = survey_collection.get_survey(survey_name)
     except AssertionError:
+        log.info(f"Survey {survey_name} does not exist, it will be created.")
         survey = Survey(
             name = survey_name,
             label = survey_label or None,
             survey_collection = survey_collection,
             )
 
     if survey.hdf5_file_path is None:
         config = survey.survey_collection.config
         directory_path = config.get("data", "output_directory")
         if not os.path.isdir(directory_path):
-            log.warn("{} who should be the HDF5 data directory does not exist: we create the directory".format(
+            log.warning("{} who should be the HDF5 data directory does not exist: we create the directory".format(
                 directory_path))
             os.makedirs(directory_path)
         survey.hdf5_file_path = os.path.join(directory_path, survey.name + '.h5')
 
     assert survey.hdf5_file_path is not None
     survey.insert_table(label = table_label, name = table_name, dataframe = input_dataframe)
+    # If a survey with save name exist it will be overwritten
     survey_collection.surveys = [
         kept_survey for kept_survey in survey_collection.surveys if kept_survey.name != survey_name
         ]
     survey_collection.surveys.append(survey)
     collections_directory = survey_collection.config.get('collections', 'collections_directory')
     assert os.path.isdir(collections_directory), """{} who should be the collections' directory does not exist.
 Fix the option collections_directory in the collections section of your config file.""".format(collections_directory)
```

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/matching.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_dbf.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_dbf.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/read_sas.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scenarios.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scenarios.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from openfisca_core import periods
 from openfisca_core.simulation_builder import SimulationBuilder
 from openfisca_core.indexed_enums import Enum
 from openfisca_core.periods import MONTH, YEAR, ETERNITY
 from openfisca_core.tools.simulation_dumper import dump_simulation, restore_simulation
 
 from openfisca_survey_manager.calibration import Calibration
-
+from openfisca_survey_manager import default_config_files_directory
 from openfisca_survey_manager.survey_collections import SurveyCollection
 from openfisca_survey_manager.surveys import Survey
 
 log = logging.getLogger(__name__)
 
 
 class AbstractSurveyScenario(object):
@@ -51,14 +51,15 @@
     trace = False
     used_as_input_variables = None
     used_as_input_variables_by_entity = None
     variation_factor = .03  # factor used to compute variation when estimating marginal tax rate
     varying_variable = None
     weight_variable_by_entity = None
     year = None
+    config_files_directory = default_config_files_directory
 
     def build_input_data(self, **kwargs):
         """Build input data."""
         NotImplementedError
 
     def calculate_series(self, variable, period = None, use_baseline = False):
         """Compute variable values for period and baseline or reform tax benefit and system.
@@ -903,26 +904,27 @@
 
                 array = simulation.calculate_add(variable_name, period = period)
                 assert array is not None
                 simulation.delete_arrays(variable_name, period = period)  # delete existing arrays
                 simulation.set_input(variable_name, period, inflator * array)  # insert inflated array
 
     def init_from_data(self, calibration_kwargs = None, inflation_kwargs = None,
-            rebuild_input_data = False, rebuild_kwargs = None, data = None, memory_config = None, use_marginal_tax_rate = False):
+            rebuild_input_data = False, rebuild_kwargs = None, data = None, memory_config = None, use_marginal_tax_rate = False,
+            config_files_directory = default_config_files_directory):
         """Initialise a survey scenario from data.
 
         Args:
           rebuild_input_data(bool):  Whether or not to clean, format and save data. Take a look at :func:`build_input_data`
           data(dict): Contains the data, or metadata needed to know where to find it.
           use_marginal_tax_rate(bool): True to go into marginal effective tax rate computation mode.
           calibration_kwargs(dict):  Calibration options (Default value = None)
           inflation_kwargs(dict): Inflations options (Default value = None)
           rebuild_input_data(bool): Whether to rebuild the data (Default value = False)
           rebuild_kwargs:  Rebuild options (Default value = None)
-
+          config_files_directory:  Directory where to find the configuration files (Default value = default_config_files_directory)
         """
         # When not ``None``, it'll try to get the data for *year*.
         if data is not None:
             data_year = data.get("data_year", self.year)
 
         self._set_id_variable_by_entity_key()
         self._set_role_variable_by_entity_key()
@@ -1229,15 +1231,15 @@
             simulation.period = periods.period(self.year)
 
         return simulation
 
     def load_table(self, variables = None, collection = None, survey = None,
             table = None):
         collection = collection or self.collection
-        survey_collection = SurveyCollection.load(collection = self.collection)
+        survey_collection = SurveyCollection.load(collection = self.collection, config_files_directory=self.config_files_directory)
         if survey is not None:
             survey = survey
         else:
             survey = "{}_{}".format(self.input_data_survey_prefix, self.year)
         survey_ = survey_collection.get_survey(survey)
         log.debug("Loading table {} in survey {} from collection {}".format(table, survey, collection))
         return survey_.get_values(table = table, variables = variables)
```

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/scripts/build_collection.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scripts/build_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/statshelpers.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/statshelpers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/survey_collections.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/survey_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,31 +99,31 @@
         assert os.path.exists(config_files_directory)
         config = Config(config_files_directory = config_files_directory)
         if json_file_path is None:
             assert collection is not None, "A collection is needed"
             try:
                 json_file_path = config.get("collections", collection)
             except Exception as error:
-                log.debug("Looking for congi file in {}".format(config_files_directory))
+                log.debug("Looking for config file in {}".format(config_files_directory))
                 log.error(error)
                 raise
 
         with open(json_file_path, 'r') as _file:
             self_json = json.load(_file)
-            name = self_json.get('name')
+            name = self_json['name']
 
-        self = cls(name = name)
+        self = cls(config_files_directory = config_files_directory, name = name)
         self.config = config
         with open(json_file_path, 'r') as _file:
             self_json = json.load(_file)
             self.json_file_path = json_file_path
             self.label = self_json.get('label')
             self.name = self_json.get('name')
 
-        surveys = self_json.get('surveys')
+        surveys = self_json['surveys']
         for survey_name, survey_json in surveys.items():
             survey = Survey(name = survey_name)
             self.surveys.append(survey.create_from_json(survey_json))
         return self
 
     def to_json(self):
         self_json = collections.OrderedDict((
```

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/surveys.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tables.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/temporary.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/temporary.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_add_survey_to_collection.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_surveys.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,55 @@
 
-
 import os
 import pkg_resources
 
 
 from openfisca_survey_manager.survey_collections import SurveyCollection
-from openfisca_survey_manager.scripts.build_collection import add_survey_to_collection
-
-# Travis, Gitlab runner, Gihub Action and circle has env variable "CI" set by default
-if 'CI' in os.environ:
-    is_in_ci = True
-else:
-    is_in_ci = False
+from openfisca_survey_manager.surveys import Survey
 
 
-def test_add_survey_to_collection():
-    if is_in_ci:
-        return
+def test_survey():
     name = 'fake'
-    survey_name = 'fake_survey'
     data_dir = os.path.join(
         pkg_resources.get_distribution('openfisca-survey-manager').location,
         'openfisca_survey_manager',
         'tests',
         'data_files',
         )
-    survey_collection = SurveyCollection(name = name)
+
+    survey_collection = SurveyCollection(
+        name = name,
+        config_files_directory = data_dir,
+        json_file_path = os.path.join(data_dir, 'fake.json')
+        )
+
+    saved_fake_survey_hdf5_file_path = os.path.join(data_dir, 'fake.hdf5')
     saved_fake_survey_file_path = os.path.join(data_dir, 'help.sas7bdat')
-    add_survey_to_collection(
-        survey_name = survey_name,
-        survey_collection = survey_collection,
+    survey = Survey(
+        hdf5_file_path = saved_fake_survey_hdf5_file_path,
+        name = 'fake_survey',
         sas_files = [saved_fake_survey_file_path],
-        stata_files = []
+        survey_collection = survey_collection,
+        )
+    survey.insert_table(name = 'help')
+    survey.fill_hdf(source_format = 'sas')
+
+
+def test_survey_load():
+    survey_name = 'test_set_table_in_survey_2021'
+    collection = 'fake'
+    data_dir = os.path.join(
+        pkg_resources.get_distribution('openfisca-survey-manager').location,
+        'openfisca_survey_manager',
+        'tests',
+        'data_files',
+        )
+    survey_collection = SurveyCollection.load(
+        collection=collection, config_files_directory=data_dir
         )
-    ordered_dict = survey_collection.to_json()
-    assert survey_name in list(ordered_dict['surveys'].keys())
+    survey = survey_collection.get_survey(survey_name)
+    for table_name, _ in survey.tables.items():
+        assert table_name == "foyer_2021"
+
+
+if __name__ == '__main__':
+    test_survey()
```

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_calmar.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_legislation_inflator.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_legislation_inflator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_marginal_tax_rate.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_matching.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_quantile.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_read_sas.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_scenario.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_summarize_variables.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_summarize_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/utils.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/openfisca_survey_manager/variables.py` & `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/setup.cfg` & `OpenFisca-Survey-Manager-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.1/setup.py` & `OpenFisca-Survey-Manager-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 doc_lines = __doc__.split('\n')
 
 
 setup(
     name = 'OpenFisca-Survey-Manager',
-    version = '1.0.1',
+    version = '1.0.2',
     author = 'OpenFisca Team',
     author_email = 'contact@openfisca.fr',
     classifiers = [classifier for classifier in classifiers.split('\n') if classifier],
     description = doc_lines[0],
     keywords = 'survey data',
     license = 'http://www.fsf.org/licensing/licenses/agpl-3.0.html',
     license_files = ("LICENSE.AGPL.txt",),
@@ -62,14 +62,15 @@
             'flake8-print >= 5.0.0, < 6.0',
             'flake8-rst-docstrings >= 0.3.0, < 0.4.0',
             'openfisca-country-template >=6 , <7 ',
             'pytest >= 7.2.2, < 8.0',
             'pytest-cov >= 4.0.0, < 5.0',
             'scipy >= 1.10.1, < 2.0',
             'tables >= 3.8.0, < 4.0',
+            'pytest-order >=1.1.0, <2.0',
             ],
         'casd': [
             'autopep8 >= 2.0.2, < 3',
             'flake8 >= 6.0.0, < 7.0',
             'pycodestyle >= 2.10.0, < 3.0',
             'pytest >= 7.2.2, < 8.0',
             'scipy >= 1.10.1, < 2.0',
```

