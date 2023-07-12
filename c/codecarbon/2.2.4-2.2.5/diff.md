# Comparing `tmp/codecarbon-2.2.4.tar.gz` & `tmp/codecarbon-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecarbon-2.2.4.tar", last modified: Wed Jun 21 08:40:51 2023, max compression
+gzip compressed data, was "codecarbon-2.2.5.tar", last modified: Wed Jul 12 17:40:00 2023, max compression
```

## Comparing `codecarbon-2.2.4.tar` & `codecarbon-2.2.5.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.903775 codecarbon-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 08:40:35.000000 codecarbon-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-21 08:40:51.903775 codecarbon-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-21 08:40:35.000000 codecarbon-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.879774 codecarbon-2.2.4/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.883774 codecarbon-2.2.4/carbonserver/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.883774 codecarbon-2.2.4/carbonserver/carbonserver/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.883774 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/domain/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.887774 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.887774 codecarbon-2.2.4/carbonserver/carbonserver/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/carbonserver/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-21 08:40:35.000000 codecarbon-2.2.4/carbonserver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.887774 codecarbon-2.2.4/codecarbon/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/rapl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.879774 codecarbon-2.2.4/codecarbon/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/data/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/cloud/impact.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/data/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)    49423 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/hardware/cpu_power.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/data/private_infra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.891775 codecarbon-2.2.4/codecarbon/data/private_infra/2016/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0 runner    (1001) docker     (123)   124501 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)    39720 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/emissions_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.895774 codecarbon-2.2.4/codecarbon/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/geography.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/external/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.895774 codecarbon-2.2.4/codecarbon/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/prometheus/metric_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.895774 codecarbon-2.2.4/codecarbon/viz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.899775 codecarbon-2.2.4/codecarbon/viz/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/carbonboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-06-21 08:40:35.000000 codecarbon-2.2.4/codecarbon/viz/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.887774 codecarbon-2.2.4/codecarbon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 08:40:51.000000 codecarbon-2.2.4/codecarbon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:40:51.903775 codecarbon-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-21 08:40:36.000000 codecarbon-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:40:51.903775 codecarbon-2.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_api_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_core_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_emissions_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_emissions_tracker_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_emissions_tracker_flush.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_geography.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_logging_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/test_ram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-21 08:40:36.000000 codecarbon-2.2.4/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.708821 codecarbon-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 17:39:42.000000 codecarbon-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-12 17:40:00.708821 codecarbon-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-12 17:39:42.000000 codecarbon-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.688821 codecarbon-2.2.5/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.688821 codecarbon-2.2.5/carbonserver/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.688821 codecarbon-2.2.5/carbonserver/carbonserver/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.692821 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.692821 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.692821 codecarbon-2.2.5/carbonserver/carbonserver/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.696821 codecarbon-2.2.5/codecarbon/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.696821 codecarbon-2.2.5/codecarbon/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/rapl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.684821 codecarbon-2.2.5/codecarbon/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/data/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/cloud/impact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/data/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    49563 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/hardware/cpu_power.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/data/private_infra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/data/private_infra/2016/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)   124501 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39720 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/emissions_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/prometheus/metric_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.704821 codecarbon-2.2.5/codecarbon/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.704821 codecarbon-2.2.5/codecarbon/viz/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/carbonboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.696821 codecarbon-2.2.5/codecarbon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:40:00.708821 codecarbon-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-12 17:39:43.000000 codecarbon-2.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.708821 codecarbon-2.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_core_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_emissions_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_emissions_tracker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_emissions_tracker_flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_logging_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/testutils.py
```

### Comparing `codecarbon-2.2.4/LICENSE` & `codecarbon-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/PKG-INFO` & `codecarbon-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.4
+Version: 2.2.5
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.4/README.md` & `codecarbon-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/dependencies.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/domain/experiments.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/domain/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/errors.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/errors.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/authenticate.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/authenticate.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/emissions.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/experiments.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/organizations.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/organizations.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/projects.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/projects.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/runs.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/runs.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/teams.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/teams.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/routers/users.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/api/schemas.py` & `codecarbon-2.2.5/carbonserver/carbonserver/api/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/carbonserver/database/database.py` & `codecarbon-2.2.5/carbonserver/carbonserver/database/database.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/container.py` & `codecarbon-2.2.5/carbonserver/container.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/main.py` & `codecarbon-2.2.5/carbonserver/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/carbonserver/setup.py` & `codecarbon-2.2.5/carbonserver/setup.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/cli/cli_utils.py` & `codecarbon-2.2.5/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/cli/main.py` & `codecarbon-2.2.5/codecarbon/cli/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/api_client.py` & `codecarbon-2.2.5/codecarbon/core/api_client.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/cloud.py` & `codecarbon-2.2.5/codecarbon/core/cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/co2_signal.py` & `codecarbon-2.2.5/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/config.py` & `codecarbon-2.2.5/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/cpu.py` & `codecarbon-2.2.5/codecarbon/core/cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/emissions.py` & `codecarbon-2.2.5/codecarbon/core/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/gpu.py` & `codecarbon-2.2.5/codecarbon/core/gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/rapl.py` & `codecarbon-2.2.5/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/schemas.py` & `codecarbon-2.2.5/codecarbon/core/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/units.py` & `codecarbon-2.2.5/codecarbon/core/units.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/core/util.py` & `codecarbon-2.2.5/codecarbon/core/util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/data/cloud/impact.csv` & `codecarbon-2.2.5/codecarbon/data/cloud/impact.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/data/hardware/cpu_power.csv` & `codecarbon-2.2.5/codecarbon/data/hardware/cpu_power.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1496,14 +1496,15 @@
 Intel Core i7-1165G7,28
 Intel Core i7-11700,65
 Intel Core i7-11700F,65
 Intel Core i7-11700K,125
 Intel Core i7-11700KF,125
 Intel Core i7-11700T,35
 Intel Core i7-1185G7,28
+Intel Core i7-1270P,64
 Intel Core i7-2670QM,45
 Intel Core i7-2675QM,45
 Intel Core i7-2700K,95
 Intel Core i7-2760QM,45
 Intel Core i7-2760QM,45
 Intel Core i7-2860QM,45
 Intel Core i7-2860QM,45
@@ -1573,14 +1574,15 @@
 Intel Core i7-6700K,95
 Intel Core i7-6700T,35
 Intel Core i7-6700TE,35
 Intel Core i7-6800K,140
 Intel Core i7-6850K,140
 Intel Core i7-6900K,140
 Intel Core i7-6950X,140
+Intel Core i7-7600U,15
 Intel Core i7-7700,65
 Intel Core i7-7700K,91
 Intel Core i7-7700T,35
 Intel Core i7-7740X,112
 Intel Core i7-7800X,140
 Intel Core i7-7820X,140
 Intel Core i7-8086K,95
@@ -2009,22 +2011,25 @@
 Intel Xeon E5-2643 v2,130
 Intel Xeon E5-2650 v2,95
 Intel Xeon E5-2650L v2,70
 Intel Xeon E5-2660 v2,95
 Intel Xeon E5-2667 v2,130
 Intel Xeon E5-2670 v2,115
 Intel Xeon E5-2673 v3,110
+Intel Xeon E5-2660 v4,105
 Intel Xeon E5-2680 v2,115
+Intel Xeon E5-2680 v4,120
 Intel Xeon E5-2687W v2,130
 Intel Xeon E5-2690 v2,130
 Intel Xeon E5-2692 v2,100
 Intel Xeon E5-2695 v2,115
 Intel Xeon E5-2697 v2,130
 Intel Xeon E5-4607,95
 Intel Xeon E5-4610,130
+Intel Xeon 5320,185
 Intel Xeon E5502,80
 Intel Xeon E5503,80
 Intel Xeon E5504,80
 Intel Xeon E5506,80
 Intel Xeon E5507,80
 Intel Xeon E5520,80
 Intel Xeon E5530,80
@@ -2121,14 +2126,15 @@
 Intel Xeon Platinum 8280M,205
 Intel Xeon Platinum 9221,250
 Intel Xeon Platinum 9222,250
 Intel Xeon Platinum 9242,350
 Intel Xeon Platinum 9282,400
 Intel Xeon Silver 4116,85
 Intel Xeon W-2195,140
+Intel Xeon W-2275,165
 Intel Xeon W-3175X,255
 Intel Xeon W3503,130
 Intel Xeon W3505,130
 Intel Xeon W3520,130
 Intel Xeon W3530,130
 Intel Xeon W3540,130
 Intel Xeon W3550,130
```

### Comparing `codecarbon-2.2.4/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.2.5/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.2.5/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.2.5/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/data/private_infra/global_energy_mix.json` & `codecarbon-2.2.5/codecarbon/data/private_infra/global_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/emissions_tracker.py` & `codecarbon-2.2.5/codecarbon/emissions_tracker.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/external/geography.py` & `codecarbon-2.2.5/codecarbon/external/geography.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     @classmethod
     def from_geo_js(cls, url: str) -> "GeoMetadata":
         try:
             response: Dict = requests.get(url, timeout=0.5).json()
         except Exception as e:
             # If there is a timeout, we default to Canada
             logger.warning(
-                f"Unable to access geographical location. Using 'Canada' as the default value - Exception : {e}"
+                f"Unable to access geographical location. Using 'Canada' as the default value - Exception : {e} - url={url}"
             )
             return cls(
                 country_iso_code="CAN",
                 country_name="Canada",
                 region="Quebec",
                 latitude=46.8,
                 longitude=-71.2,
```

### Comparing `codecarbon-2.2.4/codecarbon/external/hardware.py` & `codecarbon-2.2.5/codecarbon/external/hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/external/logger.py` & `codecarbon-2.2.5/codecarbon/external/logger.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/external/scheduler.py` & `codecarbon-2.2.5/codecarbon/external/scheduler.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/input.py` & `codecarbon-2.2.5/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/output.py` & `codecarbon-2.2.5/codecarbon/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,17 @@
         self.energy_consumed -= previous_emission.energy_consumed
         if delta_duration > 0:
             # emissions_rate in g/s : delta_emissions in kg.CO2 / delta_duration in s
             self.emissions_rate = delta_emissions / delta_duration
         else:
             self.emissions_rate = 0
 
+    def toJSON(self):
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
+
 
 class BaseOutput(ABC):
     """
     An abstract class that requires children to inherit a single method,
     `out` which is used for persisting data. This could be by saving it to a file,
     posting to Json Box, saving to a database, sending a slack message etc.
     """
```

### Comparing `codecarbon-2.2.4/codecarbon/prometheus/metric_definitions.py` & `codecarbon-2.2.5/codecarbon/prometheus/metric_definitions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/prometheus/prometheus.py` & `codecarbon-2.2.5/codecarbon/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.2.5/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.2.5/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.2.5/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/viz/carbonboard.py` & `codecarbon-2.2.5/codecarbon/viz/carbonboard.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.2.5/codecarbon/viz/carbonboard_on_api.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/viz/components.py` & `codecarbon-2.2.5/codecarbon/viz/components.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon/viz/data.py` & `codecarbon-2.2.5/codecarbon/viz/data.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/codecarbon.egg-info/PKG-INFO` & `codecarbon-2.2.5/codecarbon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.4
+Version: 2.2.5
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.4/codecarbon.egg-info/SOURCES.txt` & `codecarbon-2.2.5/codecarbon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/setup.py` & `codecarbon-2.2.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,23 @@
     "pandas",
     "pynvml",
     "requests",
     "psutil",
     "py-cpuinfo",
     "fuzzywuzzy",
     "click",
+    "prometheus_client",
 ]
 
 TEST_DEPENDENCIES = ["mock", "pytest", "responses", "tox", "numpy", "requests-mock"]
 
 
 setuptools.setup(
     name="codecarbon",
-    version="2.2.4",
+    version="2.2.5",
     author="Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files=("LICENSE",),
     packages=setuptools.find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]
     ),
```

### Comparing `codecarbon-2.2.4/tests/test_api_call.py` & `codecarbon-2.2.5/tests/test_api_call.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_cloud.py` & `codecarbon-2.2.5/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_co2_signal.py` & `codecarbon-2.2.5/tests/test_co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_config.py` & `codecarbon-2.2.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_core_util.py` & `codecarbon-2.2.5/tests/test_core_util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_cpu.py` & `codecarbon-2.2.5/tests/test_cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_emissions.py` & `codecarbon-2.2.5/tests/test_emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_emissions_tracker.py` & `codecarbon-2.2.5/tests/test_emissions_tracker.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_emissions_tracker_constant.py` & `codecarbon-2.2.5/tests/test_emissions_tracker_constant.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_emissions_tracker_flush.py` & `codecarbon-2.2.5/tests/test_emissions_tracker_flush.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_energy.py` & `codecarbon-2.2.5/tests/test_energy.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_geography.py` & `codecarbon-2.2.5/tests/test_geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_gpu.py` & `codecarbon-2.2.5/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_hardware.py` & `codecarbon-2.2.5/tests/test_hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_logging_output.py` & `codecarbon-2.2.5/tests/test_logging_output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/test_ram.py` & `codecarbon-2.2.5/tests/test_ram.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/testdata.py` & `codecarbon-2.2.5/tests/testdata.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.4/tests/testutils.py` & `codecarbon-2.2.5/tests/testutils.py`

 * *Files identical despite different names*

