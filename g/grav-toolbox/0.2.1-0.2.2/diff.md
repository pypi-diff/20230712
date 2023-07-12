# Comparing `tmp/grav-toolbox-0.2.1.tar.gz` & `tmp/grav-toolbox-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grav-toolbox-0.2.1.tar", last modified: Tue Jun 27 11:49:27 2023, max compression
+gzip compressed data, was "grav-toolbox-0.2.2.tar", last modified: Wed Jul 12 11:09:05 2023, max compression
```

## Comparing `grav-toolbox-0.2.1.tar` & `grav-toolbox-0.2.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.786410 grav-toolbox-0.2.1/
--rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/LICENSE
--rw-rw-r--   0 heller    (1000) heller    (1000)     7522 2023-06-27 11:49:27.786410 grav-toolbox-0.2.1/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.2.1/README.md
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.766410 grav-toolbox-0.2.1/bev_legacy/
--rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/__init__.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/adjust.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/adjust_reilly1970.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/command_line.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/const.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/drift_mlr.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/init.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/output.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/plots.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/schwaus.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.2.1/bev_legacy/settings.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/bev_legacy/utils.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.770410 grav-toolbox-0.2.1/grav_toolbox.egg-info/
--rw-rw-r--   0 heller    (1000) heller    (1000)     7522 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     2418 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       59 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/requires.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-06-27 11:49:27.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/top_level.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.2.1/grav_toolbox.egg-info/zip-safe
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.770410 grav-toolbox-0.2.1/gravtools/
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.770410 grav-toolbox-0.2.1/gravtools/CG5_utils/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/CG5_utils/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32664 2023-06-27 11:18:52.000000 grav-toolbox-0.2.1/gravtools/CG5_utils/cg5_survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-06-27 11:49:15.000000 grav-toolbox-0.2.1/gravtools/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/const.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.778410 grav-toolbox-0.2.1/gravtools/gui/
--rw-rw-r--   0 heller    (1000) heller    (1000)    65835 2023-06-20 14:23:44.000000 grav-toolbox-0.2.1/gravtools/gui/MainWindow.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/gui/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_about.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_autoselection_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18526 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    11546 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_estimation_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_export_results.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_gis_export_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_load_stations.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12699 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_load_tsf_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_new_campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_options.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9036 2023-06-15 09:16:03.000000 grav-toolbox-0.2.1/gravtools/gui/dialog_setup_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15540 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/gui/dlg_correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1784 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/gui/dlg_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2371 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/gui/dlg_load_tsf_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)   199780 2023-06-27 11:34:07.000000 grav-toolbox-0.2.1/gravtools/gui/gui_main.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_observation_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_correlation_matrix_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_drift_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_obs_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     7427 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_stat_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_results_vg_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_setup_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_station_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.2.1/gravtools/gui/gui_model_survey_table.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.782410 grav-toolbox-0.2.1/gravtools/models/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/models/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    49963 2023-06-27 11:30:46.000000 grav-toolbox-0.2.1/gravtools/models/campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/models/exceptions.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    38608 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/lsm.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    38803 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/lsm_diff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    35256 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/lsm_nondiff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.2.1/gravtools/models/misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18698 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/mlr_bev_legacy.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    22918 2023-04-21 17:57:27.000000 grav-toolbox-0.2.1/gravtools/models/station.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    99692 2023-06-13 16:10:17.000000 grav-toolbox-0.2.1/gravtools/models/survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32396 2023-05-14 14:10:01.000000 grav-toolbox-0.2.1/gravtools/models/vg_lsm.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.782410 grav-toolbox-0.2.1/gravtools/scripts/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/scripts/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1893 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/scripts/create_correction_time_seriens_from_tsf.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1481 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/scripts/load_tfs_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/scripts/run_gui.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    12252 2023-06-27 11:24:11.000000 grav-toolbox-0.2.1/gravtools/settings.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-27 11:49:27.786410 grav-toolbox-0.2.1/gravtools/tides/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/tides/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16244 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/tides/correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/gravtools/tides/longman1959.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3413 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/tides/tide_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18016 2023-06-07 17:28:21.000000 grav-toolbox-0.2.1/gravtools/tides/tide_data_tfs.py
--rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.2.1/pyproject.toml
--rw-rw-r--   0 heller    (1000) heller    (1000)      917 2023-06-27 11:49:27.786410 grav-toolbox-0.2.1/setup.cfg
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.139649 grav-toolbox-0.2.2/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/LICENSE
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7522 2023-07-12 11:09:05.139649 grav-toolbox-0.2.2/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.2.2/README.md
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.119650 grav-toolbox-0.2.2/bev_legacy/
+-rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/__init__.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/adjust.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/adjust_reilly1970.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/command_line.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/const.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/drift_mlr.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/init.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/output.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/plots.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/schwaus.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.2.2/bev_legacy/settings.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/utils.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.123649 grav-toolbox-0.2.2/grav_toolbox.egg-info/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7522 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2418 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       59 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/top_level.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/zip-safe
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.123649 grav-toolbox-0.2.2/gravtools/
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.123649 grav-toolbox-0.2.2/gravtools/CG5_utils/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/CG5_utils/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32664 2023-06-27 12:10:33.000000 grav-toolbox-0.2.2/gravtools/CG5_utils/cg5_survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/const.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.131649 grav-toolbox-0.2.2/gravtools/gui/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    65336 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/MainWindow.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/gui/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_about.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_autoselection_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18526 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    11546 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_estimation_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_export_results.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_gis_export_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_load_stations.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12699 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_new_campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_options.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9036 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_setup_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15540 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/gui/dlg_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1784 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/gui/dlg_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2371 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/gui/dlg_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)   199887 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/gui_main.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_observation_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_correlation_matrix_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_drift_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_obs_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7493 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_stat_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_vg_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_setup_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_station_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_survey_table.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.135650 grav-toolbox-0.2.2/gravtools/models/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/models/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    49871 2023-06-27 12:10:33.000000 grav-toolbox-0.2.2/gravtools/models/campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/models/exceptions.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    38608 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/lsm.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    38803 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/lsm_diff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35256 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/lsm_nondiff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/models/misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18698 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/mlr_bev_legacy.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    22918 2023-04-21 17:57:27.000000 grav-toolbox-0.2.2/gravtools/models/station.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    99702 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/models/survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32396 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/vg_lsm.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.135650 grav-toolbox-0.2.2/gravtools/scripts/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/scripts/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1893 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/scripts/create_correction_time_seriens_from_tsf.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1481 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/scripts/load_tfs_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/scripts/run_gui.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    12252 2023-06-27 12:10:33.000000 grav-toolbox-0.2.2/gravtools/settings.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.139649 grav-toolbox-0.2.2/gravtools/tides/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/tides/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16244 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/tides/correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/tides/longman1959.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3413 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/tides/tide_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18016 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/tides/tide_data_tfs.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/pyproject.toml
+-rw-rw-r--   0 heller    (1000) heller    (1000)      917 2023-07-12 11:09:05.139649 grav-toolbox-0.2.2/setup.cfg
```

### Comparing `grav-toolbox-0.2.1/LICENSE` & `grav-toolbox-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/PKG-INFO` & `grav-toolbox-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.2.1
+Version: 0.2.2
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grav-toolbox-0.2.1/README.md` & `grav-toolbox-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/adjust.py` & `grav-toolbox-0.2.2/bev_legacy/adjust.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/adjust_reilly1970.py` & `grav-toolbox-0.2.2/bev_legacy/adjust_reilly1970.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/command_line.py` & `grav-toolbox-0.2.2/bev_legacy/command_line.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/drift_mlr.py` & `grav-toolbox-0.2.2/bev_legacy/drift_mlr.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/init.py` & `grav-toolbox-0.2.2/bev_legacy/init.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/output.py` & `grav-toolbox-0.2.2/bev_legacy/output.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/plots.py` & `grav-toolbox-0.2.2/bev_legacy/plots.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/schwaus.py` & `grav-toolbox-0.2.2/bev_legacy/schwaus.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/settings.py` & `grav-toolbox-0.2.2/bev_legacy/settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/bev_legacy/utils.py` & `grav-toolbox-0.2.2/bev_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/grav_toolbox.egg-info/PKG-INFO` & `grav-toolbox-0.2.2/grav_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.2.1
+Version: 0.2.2
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grav-toolbox-0.2.1/grav_toolbox.egg-info/SOURCES.txt` & `grav-toolbox-0.2.2/grav_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/CG5_utils/__init__.py` & `grav-toolbox-0.2.2/gravtools/CG5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/CG5_utils/cg5_survey.py` & `grav-toolbox-0.2.2/gravtools/CG5_utils/cg5_survey.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/__init__.py` & `grav-toolbox-0.2.2/gravtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 :Authors:
     Andreas Hellerschmied (andreas.hellerschmied@bev.gv.at)
 """
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 __author__ = 'Andreas Hellerschmied'
 __git_repo__ = 'https://github.com/ahellers/GravTools'
 __pypi_repo__ = 'https://pypi.org/project/grav-toolbox/'
 __email__ = 'andreas.hellerschmied@bev.gv.at'
 __copyright__ = '(c) 2022 Andreas Hellerschmied'
```

### Comparing `grav-toolbox-0.2.1/gravtools/const.py` & `grav-toolbox-0.2.2/gravtools/const.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/MainWindow.py` & `grav-toolbox-0.2.2/gravtools/gui/MainWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/MainWindow.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
@@ -57,18 +57,14 @@
         self.verticalLayout_31 = QtWidgets.QVBoxLayout(self.groupBox_stations_map_view_options)
         self.verticalLayout_31.setObjectName("verticalLayout_31")
         self.checkBox_stations_map_show_stat_name_labels = QtWidgets.QCheckBox(self.groupBox_stations_map_view_options)
         self.checkBox_stations_map_show_stat_name_labels.setChecked(True)
         self.checkBox_stations_map_show_stat_name_labels.setObjectName("checkBox_stations_map_show_stat_name_labels")
         self.verticalLayout_31.addWidget(self.checkBox_stations_map_show_stat_name_labels)
         self.verticalLayout_3.addWidget(self.groupBox_stations_map_view_options)
-        self.groupBox_edit_options = QtWidgets.QGroupBox(self.tab_main_stations)
-        self.groupBox_edit_options.setEnabled(False)
-        self.groupBox_edit_options.setObjectName("groupBox_edit_options")
-        self.verticalLayout_3.addWidget(self.groupBox_edit_options)
         spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_3.addItem(spacerItem)
         self.horizontalLayout_2.addLayout(self.verticalLayout_3)
         self.tab_Widget_Stations = QtWidgets.QTabWidget(self.tab_main_stations)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
@@ -632,24 +628,22 @@
         self.menu_File.addAction(self.action_Change_output_directory)
         self.menu_File.addAction(self.action_Change_Campaign_name)
         self.menu_File.addAction(self.action_Save_Campaign)
         self.menu_File.addAction(self.action_Load_Campaign)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.menuAdd_Survey.menuAction())
         self.menu_File.addAction(self.menu_Add_Stations.menuAction())
-        self.menu_File.addAction(self.action_Add_Stations)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.action_Export_Results)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.action_Options)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.action_Exit)
         self.menu_Observations.addSeparator()
         self.menu_Observations.addAction(self.action_Autoselection_settings)
-        self.menu_Observations.addAction(self.actionEstimate_long_term_drift)
         self.menu_Observations.addAction(self.action_Setup_data_options)
         self.menu_Observations.addAction(self.action_Flag_observations)
         self.menuEstimation_settings.addAction(self.action_Estimation_settings)
         self.menuEstimation_settings.addAction(self.action_Gis_Export_settings)
         self.menuHelp.addAction(self.action_About)
         self.menuCorrections.addAction(self.action_Corrections)
         self.menuCorrections.addAction(self.action_Correction_time_series)
@@ -673,15 +667,14 @@
         self.groupBox_filter_options.setToolTip(_translate("MainWindow", "Display options for stations"))
         self.groupBox_filter_options.setTitle(_translate("MainWindow", "Filter Options"))
         self.checkBox_filter_observed_stat_only.setToolTip(_translate("MainWindow", "Display only stations that were observed in this campaign. "))
         self.checkBox_filter_observed_stat_only.setText(_translate("MainWindow", "Observed only"))
         self.label.setText(_translate("MainWindow", "Station name filter (regex)"))
         self.groupBox_stations_map_view_options.setTitle(_translate("MainWindow", "Map view options"))
         self.checkBox_stations_map_show_stat_name_labels.setText(_translate("MainWindow", "Show station name labels"))
-        self.groupBox_edit_options.setTitle(_translate("MainWindow", "Edit Options"))
         self.tab_Widget_Stations.setTabText(self.tab_Widget_Stations.indexOf(self.tab_Stations_Table), _translate("MainWindow", "Table"))
         self.tab_Widget_Stations.setTabText(self.tab_Widget_Stations.indexOf(self.tab_stations_map), _translate("MainWindow", "Map"))
         self.tabWidget_Main.setTabText(self.tabWidget_Main.indexOf(self.tab_main_stations), _translate("MainWindow", "Stations"))
         self.treeWidget_observations.setSortingEnabled(False)
         self.treeWidget_observations.headerItem().setText(0, _translate("MainWindow", "Survey"))
         self.treeWidget_observations.headerItem().setText(1, _translate("MainWindow", "Station"))
         self.treeWidget_observations.headerItem().setText(2, _translate("MainWindow", "#Obs"))
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/__init__.py` & `grav-toolbox-0.2.2/gravtools/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_about.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_about.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_about.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_autoselection_settings.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_autoselection_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_autoselection_settings.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_correction_time_series.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_correction_time_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_correction_time_series.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_corrections.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_corrections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_corrections.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_estimation_settings.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_estimation_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_estimation_settings.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_export_results.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_export_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_export_results.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_gis_export_settings.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_gis_export_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_gis_export_settings.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_load_stations.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_load_stations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_load_stations.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_load_tsf_file.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_load_tsf_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_load_tsf_file.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_new_campaign.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_new_campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_new_campaign.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_options.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_options.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dialog_setup_data.py` & `grav-toolbox-0.2.2/gravtools/gui/dialog_setup_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file 'gravtools/gui/dialog_setup_data.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dlg_correction_time_series.py` & `grav-toolbox-0.2.2/gravtools/gui/dlg_correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dlg_corrections.py` & `grav-toolbox-0.2.2/gravtools/gui/dlg_corrections.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/dlg_load_tsf_file.py` & `grav-toolbox-0.2.2/gravtools/gui/dlg_load_tsf_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_main.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
         """Invoked whenever the menu item change output directory is pressed."""
         self.change_campaign_output_directory()
 
     def change_campaign_output_directory(self):
         """Change the output directory of the current campaign."""
         initial_folder_path = self.campaign.output_directory
         output_dir_name = QFileDialog.getExistingDirectory(self, 'Select a directory', initial_folder_path,
-                                                           QtGui.QFileDialog.ShowDirsOnly)
+                                                           QFileDialog.ShowDirsOnly)
         if output_dir_name:
             # Returns pathName with the '/' separators converted to separators that are appropriate for the underlying
             # operating system.
             # On Windows, toNativeSeparators("c:/winnt/system32") returns "c:\winnt\system32".
             output_dir_name = QDir.toNativeSeparators(output_dir_name)
             # Check, if path exists:
             if os.path.isdir(output_dir_name):
@@ -1070,15 +1070,19 @@
             drift_pol_df_short = drift_pol_df.loc[drift_pol_df['survey_name'] == survey_name]
             setup_df = setup_df_orig.copy(deep=True)  # Make hard copy to protect original data!
             # stat_obs_df_short = stat_obs_df.loc[:, ['station_name', 'g_est_mugal', 'sd_g_est_mugal']]
             # setup_df = pd.merge(setup_df, stat_obs_df_short, on='station_name')
             # setup_df['g_plot_mugal'] = setup_df['g_mugal'] - setup_df['g_est_mugal']
             setup_df.sort_values(by='delta_t_campaign_h', inplace=True)
             # Merge df => Colum with post-fit residuals ("v_obs_est_mugal") added to "setup_df":
-            if setup_data['setup_calc_method'] != 'individual_obs':
+            if not hasattr(setup_data, 'setup_calc_method'):  # to grand downward compatibility < v0.2.0
+                setup_calc_method = 'variance_weighted_mean'
+            else:
+                setup_calc_method = setup_data['setup_calc_method']
+            if setup_calc_method != 'individual_obs':
                 setup_obs_df_short = lsm_run.setup_obs_df.loc[
                     lsm_run.setup_obs_df['survey_name'] == survey_name, ['setup_id', 'v_obs_est_mugal']].copy(deep=True)
                 setup_df = pd.merge(setup_df, setup_obs_df_short, how='left', on='setup_id')  # WEG!
             else:
                 setup_obs_df_short = lsm_run.setup_obs_df.loc[
                     lsm_run.setup_obs_df['survey_name'] == survey_name, ['ref_epoch_dt', 'v_obs_est_mugal']].copy(
                     deep=True)
@@ -3079,19 +3083,17 @@
 
                 self.statusBar().showMessage(f"{number_of_stations_added} stations added.")
 
     def enable_station_view_options_based_on_model(self):
         """Enable or disable the station view options based on the number of stations in the model."""
         if len(self.station_model._data) > 0:
             self.groupBox_filter_options.setEnabled(True)
-            self.groupBox_edit_options.setEnabled(True)
             self.groupBox_stations_map_view_options.setEnabled(True)
         else:
             self.groupBox_filter_options.setEnabled(False)
-            self.groupBox_edit_options.setEnabled(False)
             self.groupBox_stations_map_view_options.setEnabled(False)
 
     def refresh_stations_table_model_and_view(self):
         """Refresh the station table model and the respective table view."""
         self.station_model.load_stat_df(self.campaign.stations.stat_df)
         self.station_model.layoutChanged.emit()  # Refresh the table view, after changing the model's size.
         self.tableView_Stations.resizeColumnsToContents()
@@ -3319,15 +3321,15 @@
             self.lineEdit_campaign_name.setText('')
 
     def get_output_directory_dialog(self):
         """Open dialog to get the output directory."""
 
         initial_folder_path = self.lineEdit_output_directory.text()
         output_dir_name = QFileDialog.getExistingDirectory(self, 'Select a directory', initial_folder_path,
-                                                           QtGui.QFileDialog.ShowDirsOnly)
+                                                           QFileDialog.ShowDirsOnly)
 
         if output_dir_name:
             # Returns pathName with the '/' separators converted to separators that are appropriate for the underlying
             # operating system.
             # On Windows, toNativeSeparators("c:/winnt/system32") returns "c:\winnt\system32".
             output_dir_name = QDir.toNativeSeparators(output_dir_name)
             if IS_VERBOSE:
@@ -3426,15 +3428,15 @@
             initial_folder_path = os.path.dirname(os.path.abspath(self.lineEdit_gis_output_dir.text()))
         else:
             try:
                 initial_folder_path = self.campaign_output_dir
             except:
                 initial_folder_path = os.getcwd()
         output_dir_name = QFileDialog.getExistingDirectory(self, 'Select a directory', initial_folder_path,
-                                                           QtGui.QFileDialog.ShowDirsOnly)
+                                                           QFileDialog.ShowDirsOnly)
 
         if output_dir_name:
             # Returns pathName with the '/' separators converted to separators that are appropriate for the underlying
             # operating system.
             # On Windows, toNativeSeparators("c:/winnt/system32") returns "c:\winnt\system32".
             output_dir_name = QDir.toNativeSeparators(output_dir_name)
             if IS_VERBOSE:
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_misc.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_model_observation_table.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_model_observation_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_correlation_matrix_table.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_correlation_matrix_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_drift_table.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_drift_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_obs_table.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_obs_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_stat_table.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_stat_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,17 @@
 
             if role == Qt.TextAlignmentRole:
                 if isinstance(value, int) or isinstance(value, float):
                     # Align right, vertical middle.
                     return Qt.AlignVCenter + Qt.AlignRight
 
             if role == Qt.BackgroundRole:
-                if self._data.iloc[index.row(), self._data_column_names.index('is_datum')]:
-                    return QtGui.QColor(settings.DATUM_STATION_COLOR[0], settings.DATUM_STATION_COLOR[1], settings.DATUM_STATION_COLOR[2])
+                if 'is_datum' in self._data_column_names:
+                    if self._data.iloc[index.row(), self._data_column_names.index('is_datum')]:
+                        return QtGui.QColor(settings.DATUM_STATION_COLOR[0], settings.DATUM_STATION_COLOR[1], settings.DATUM_STATION_COLOR[2])
 
         return None
 
     def headerData(self, section, orientation, role):
         # section is the index of the column/row.
         if role == Qt.DisplayRole and self._data is not None:
             if orientation == Qt.Horizontal:
```

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_model_results_vg_table.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_vg_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_model_setup_table.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_model_setup_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_model_station_table.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_model_station_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/gui/gui_model_survey_table.py` & `grav-toolbox-0.2.2/gravtools/gui/gui_model_survey_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/models/__init__.py` & `grav-toolbox-0.2.2/gravtools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/models/campaign.py` & `grav-toolbox-0.2.2/gravtools/models/campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -822,16 +822,14 @@
             If `True`, status messages are printed to the command line.
 
         Returns
         -------
         `Campaign` object
         """
         campaign = pd.read_pickle(filename)
-        # with open(filename, 'rb') as handle:
-        #     campaign = pickle.load(handle)
         if verbose:
             print(
                 f'Loaded campaign "{campaign.campaign_name}" with {campaign.number_of_stations} station(s) and {campaign.number_of_surveys} survey(s).')
         return campaign
 
     def set_output_directory(self, output_directory):
         """Change the campaign's output directory.
```

### Comparing `grav-toolbox-0.2.1/gravtools/models/exceptions.py` & `grav-toolbox-0.2.2/gravtools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/models/lsm.py` & `grav-toolbox-0.2.2/gravtools/models/lsm.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/models/lsm_diff.py` & `grav-toolbox-0.2.2/gravtools/models/lsm_diff.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/models/lsm_nondiff.py` & `grav-toolbox-0.2.2/gravtools/models/lsm_nondiff.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/models/misc.py` & `grav-toolbox-0.2.2/gravtools/models/misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/models/mlr_bev_legacy.py` & `grav-toolbox-0.2.2/gravtools/models/mlr_bev_legacy.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/models/station.py` & `grav-toolbox-0.2.2/gravtools/models/station.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/models/survey.py` & `grav-toolbox-0.2.2/gravtools/models/survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,15 +629,15 @@
             obs_df['tide'] = obs_df['tide'] * 1e3
             obs_df['keep_obs'] = True
 
             # Check timezone of observation epoch and convert it to UTC, if necessary:
             if obs_df['obs_epoch'].dt.tz is None:  # TZ unaware => set TZ to <UTC>
                 obs_df.loc[:, 'obs_epoch'] = obs_df['obs_epoch'].dt.tz_localize('UTC')
             else:
-                if obs_df['obs_epoch'].dt.tz.zone != 'UTC':  # Change TZ to <UTC>
+                if obs_df['obs_epoch'].dt.tz != dt.timezone.utc:  # Change TZ to <UTC>
                     obs_df.loc[:, 'obs_epoch'] = obs_df['obs_epoch'].dt.tz_convert('UTC')
 
             # Rename columns:
             obs_df.rename(columns={'terrain': 'corr_terrain',
                                    'tide': 'corr_tide_mugal', },
                           inplace=True)
 
@@ -774,15 +774,15 @@
         df['obs_epoch'] = pd.to_datetime(date_str + ' ' + df['time_hh.mm'] + ' ' + timezone_str,
                                          format='%Y %m %d %H.%M %Z')
 
         # Check timezone of observation epoch and convert it to UTC, if necessary:
         if df['obs_epoch'].dt.tz is None:  # TZ unaware => set TZ to <UTC>
             df.loc[:, 'obs_epoch'] = df['obs_epoch'].dt.tz_localize('UTC')
         else:
-            if df['obs_epoch'].dt.tz.zone != 'UTC':  # Change TZ to <UTC>
+            if df['obs_epoch'].dt.tz != dt.timezone.utc:  # Change TZ to <UTC>
                 df.loc[:, 'obs_epoch'] = df['obs_epoch'].dt.tz_convert('UTC')
 
         # Timestamp: https://stackoverflow.com/questions/40881876/python-pandas-convert-datetime-to-timestamp-effectively-through-dt-accessor
         df['setup_id'] = df['obs_epoch'].values.astype(np.int64) // 10 ** 9
 
         df['g_obs_mugal'] = df['g_mgal'] * 1e3
         df['dhb_m'] = df['dhb_cm'] * 1e-2
```

### Comparing `grav-toolbox-0.2.1/gravtools/models/vg_lsm.py` & `grav-toolbox-0.2.2/gravtools/models/vg_lsm.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/scripts/__init__.py` & `grav-toolbox-0.2.2/gravtools/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/scripts/create_correction_time_seriens_from_tsf.py` & `grav-toolbox-0.2.2/gravtools/scripts/create_correction_time_seriens_from_tsf.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/scripts/load_tfs_file.py` & `grav-toolbox-0.2.2/gravtools/scripts/load_tfs_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/scripts/run_gui.py` & `grav-toolbox-0.2.2/gravtools/scripts/run_gui.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/settings.py` & `grav-toolbox-0.2.2/gravtools/settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/tides/__init__.py` & `grav-toolbox-0.2.2/gravtools/tides/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/tides/correction_time_series.py` & `grav-toolbox-0.2.2/gravtools/tides/correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/tides/longman1959.py` & `grav-toolbox-0.2.2/gravtools/tides/longman1959.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/tides/tide_data.py` & `grav-toolbox-0.2.2/gravtools/tides/tide_data.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/gravtools/tides/tide_data_tfs.py` & `grav-toolbox-0.2.2/gravtools/tides/tide_data_tfs.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.1/setup.cfg` & `grav-toolbox-0.2.2/setup.cfg`

 * *Files identical despite different names*

