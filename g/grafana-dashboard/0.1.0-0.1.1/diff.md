# Comparing `tmp/grafana_dashboard-0.1.0.tar.gz` & `tmp/grafana_dashboard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana_dashboard-0.1.0.tar", last modified: Wed Jul 12 01:05:07 2023, max compression
+gzip compressed data, was "grafana_dashboard-0.1.1.tar", last modified: Wed Jul 12 01:20:23 2023, max compression
```

## Comparing `grafana_dashboard-0.1.0.tar` & `grafana_dashboard-0.1.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:05:07.444702 grafana_dashboard-0.1.0/
--rw-r--r--   0 tom        (501) staff       (20)     1064 2023-07-11 02:35:52.000000 grafana_dashboard-0.1.0/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     5339 2023-07-12 01:05:07.444460 grafana_dashboard-0.1.0/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     4583 2023-07-12 00:37:39.000000 grafana_dashboard-0.1.0/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:05:07.417666 grafana_dashboard-0.1.0/grafana_dashboard/
--rw-r--r--   0 tom        (501) staff       (20)       22 2023-07-12 01:01:39.000000 grafana_dashboard-0.1.0/grafana_dashboard/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:05:07.420791 grafana_dashboard-0.1.0/grafana_dashboard/converter/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-11 12:28:16.000000 grafana_dashboard-0.1.0/grafana_dashboard/converter/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      746 2023-07-12 00:35:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/converter/json_to_python.py
--rw-r--r--   0 tom        (501) staff       (20)     1718 2023-07-12 00:35:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/converter/python_to_json.py
--rw-r--r--   0 tom        (501) staff       (20)     1138 2023-07-11 08:22:59.000000 grafana_dashboard-0.1.0/grafana_dashboard/extracted_generated_common_models.py
--rw-r--r--   0 tom        (501) staff       (20)      836 2023-07-11 12:48:05.000000 grafana_dashboard-0.1.0/grafana_dashboard/grafana_dashboard.py
--rw-r--r--   0 tom        (501) staff       (20)     2163 2023-07-11 10:39:35.000000 grafana_dashboard-0.1.0/grafana_dashboard/manual_models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:05:07.443913 grafana_dashboard-0.1.0/grafana_dashboard/model/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-11 06:04:15.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      585 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/alertgroupspanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)      709 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/annotationslistpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)    11586 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/azuremonitordataquery_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     5208 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/barchartpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     1750 2023-07-11 14:06:15.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/bargaugepanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     9586 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/cloudwatchdataquery_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)    24281 2023-07-12 00:47:10.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/dashboard_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)      659 2023-07-11 10:42:23.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/dashboardlistpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)      356 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/datagridpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)      644 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/debugpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)    12450 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/elasticsearchdataquery_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     1391 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/gaugepanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     3111 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/geomappanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     1872 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/grafanapyroscopedataquery_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     8245 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/heatmappanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     2696 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/histogrampanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     4461 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/librarypanel_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)      932 2023-07-11 10:43:39.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/logspanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     2382 2023-07-11 10:57:14.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/lokidataquery_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)      439 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/newspanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     1632 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/nodegraphpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     1651 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/parcadataquery_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     2959 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/piechartpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     4823 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/playlist_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     3901 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/preferences_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     2769 2023-07-11 14:18:07.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/prometheusdataquery_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     3823 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/publicdashboard_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     4462 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/serviceaccount_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     1876 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/statetimelinepanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     2210 2023-07-11 13:09:40.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/statpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     1669 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/statushistorypanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     2224 2023-07-11 08:51:12.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/tablepanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     3882 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/team_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     3724 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/tempodataquery_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     4954 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/testdatadataquery_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     1063 2023-07-11 10:42:43.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/textpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     5335 2023-07-11 08:22:59.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/timeseriespanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     4549 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.0/grafana_dashboard/model/trendpanelcfg_types_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     1416 2023-07-12 00:35:02.000000 grafana_dashboard-0.1.0/grafana_dashboard/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:05:07.419795 grafana_dashboard-0.1.0/grafana_dashboard.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     5339 2023-07-12 01:05:07.000000 grafana_dashboard-0.1.0/grafana_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     2615 2023-07-12 01:05:07.000000 grafana_dashboard-0.1.0/grafana_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-07-12 01:05:07.000000 grafana_dashboard-0.1.0/grafana_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       60 2023-07-12 01:05:07.000000 grafana_dashboard-0.1.0/grafana_dashboard.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       18 2023-07-12 01:05:07.000000 grafana_dashboard-0.1.0/grafana_dashboard.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-07-12 01:05:07.444780 grafana_dashboard-0.1.0/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     2003 2023-07-12 01:04:27.000000 grafana_dashboard-0.1.0/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:20:23.339669 grafana_dashboard-0.1.1/
+-rw-r--r--   0 tom        (501) staff       (20)     1064 2023-07-11 02:35:52.000000 grafana_dashboard-0.1.1/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     5339 2023-07-12 01:20:23.339431 grafana_dashboard-0.1.1/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     4583 2023-07-12 00:37:39.000000 grafana_dashboard-0.1.1/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:20:23.314978 grafana_dashboard-0.1.1/grafana_dashboard/
+-rw-r--r--   0 tom        (501) staff       (20)       22 2023-07-12 01:17:13.000000 grafana_dashboard-0.1.1/grafana_dashboard/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:20:23.318113 grafana_dashboard-0.1.1/grafana_dashboard/converter/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-11 12:28:16.000000 grafana_dashboard-0.1.1/grafana_dashboard/converter/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      746 2023-07-12 00:35:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/converter/json_to_python.py
+-rw-r--r--   0 tom        (501) staff       (20)     1718 2023-07-12 00:35:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/converter/python_to_json.py
+-rw-r--r--   0 tom        (501) staff       (20)     1138 2023-07-11 08:22:59.000000 grafana_dashboard-0.1.1/grafana_dashboard/extracted_generated_common_models.py
+-rw-r--r--   0 tom        (501) staff       (20)      905 2023-07-12 01:15:39.000000 grafana_dashboard-0.1.1/grafana_dashboard/grafana_dashboard.py
+-rw-r--r--   0 tom        (501) staff       (20)     2163 2023-07-11 10:39:35.000000 grafana_dashboard-0.1.1/grafana_dashboard/manual_models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:20:23.339125 grafana_dashboard-0.1.1/grafana_dashboard/model/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-11 06:04:15.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      585 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/alertgroupspanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)      709 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/annotationslistpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)    11586 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/azuremonitordataquery_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     5208 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/barchartpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     1750 2023-07-11 14:06:15.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/bargaugepanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     9586 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/cloudwatchdataquery_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)    24281 2023-07-12 00:47:10.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/dashboard_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)      659 2023-07-11 10:42:23.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/dashboardlistpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)      356 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/datagridpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)      644 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/debugpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)    12450 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/elasticsearchdataquery_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     1391 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/gaugepanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     3111 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/geomappanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     1872 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/grafanapyroscopedataquery_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     8245 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/heatmappanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     2696 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/histogrampanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     4461 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/librarypanel_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)      932 2023-07-11 10:43:39.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/logspanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     2382 2023-07-11 10:57:14.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/lokidataquery_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)      439 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/newspanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     1632 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/nodegraphpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     1651 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/parcadataquery_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     2959 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/piechartpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     4823 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/playlist_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     3901 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/preferences_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     2769 2023-07-11 14:18:07.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/prometheusdataquery_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     3823 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/publicdashboard_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     4462 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/serviceaccount_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     1876 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/statetimelinepanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     2210 2023-07-11 13:09:40.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/statpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     1669 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/statushistorypanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     2224 2023-07-11 08:51:12.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/tablepanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     3882 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/team_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     3724 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/tempodataquery_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     4954 2023-07-11 08:21:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/testdatadataquery_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     1063 2023-07-11 10:42:43.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/textpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     5335 2023-07-11 08:22:59.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/timeseriespanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     4549 2023-07-11 08:24:00.000000 grafana_dashboard-0.1.1/grafana_dashboard/model/trendpanelcfg_types_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     1416 2023-07-12 00:35:02.000000 grafana_dashboard-0.1.1/grafana_dashboard/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-12 01:20:23.317201 grafana_dashboard-0.1.1/grafana_dashboard.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     5339 2023-07-12 01:20:23.000000 grafana_dashboard-0.1.1/grafana_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     2659 2023-07-12 01:20:23.000000 grafana_dashboard-0.1.1/grafana_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-07-12 01:20:23.000000 grafana_dashboard-0.1.1/grafana_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       78 2023-07-12 01:20:23.000000 grafana_dashboard-0.1.1/grafana_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 tom        (501) staff       (20)       43 2023-07-12 01:20:23.000000 grafana_dashboard-0.1.1/grafana_dashboard.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       18 2023-07-12 01:20:23.000000 grafana_dashboard-0.1.1/grafana_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-07-12 01:20:23.339744 grafana_dashboard-0.1.1/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2116 2023-07-12 01:15:55.000000 grafana_dashboard-0.1.1/setup.py
```

### Comparing `grafana_dashboard-0.1.0/LICENSE` & `grafana_dashboard-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/PKG-INFO` & `grafana_dashboard-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana_dashboard
-Version: 0.1.0
+Version: 0.1.1
 Summary: Write Grafana dashboards in Python, without losing thousands of dashboards in the zoo
 Home-page: https://github.com/fzyzcjy/grafana-dashboard-python
 Author: fzyzcjy
 License: MIT
 Keywords: grafana dashboard json
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `grafana_dashboard-0.1.0/README.md` & `grafana_dashboard-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/converter/json_to_python.py` & `grafana_dashboard-0.1.1/grafana_dashboard/converter/json_to_python.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/converter/python_to_json.py` & `grafana_dashboard-0.1.1/grafana_dashboard/converter/python_to_json.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/extracted_generated_common_models.py` & `grafana_dashboard-0.1.1/grafana_dashboard/extracted_generated_common_models.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/grafana_dashboard.py` & `grafana_dashboard-0.1.1/grafana_dashboard/grafana_dashboard.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,9 +29,14 @@
     converter.python_to_json.convert_package(
         python_base_dir=python_base_dir,
         python_base_package=python_base_package,
         json_dir=json_dir,
     )
 
 
-if __name__ == '__main__':
+# https://github.com/tiangolo/typer/issues/34
+def run():
     app()
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/manual_models.py` & `grafana_dashboard-0.1.1/grafana_dashboard/manual_models.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/alertgroupspanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/alertgroupspanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/annotationslistpanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/annotationslistpanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/azuremonitordataquery_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/azuremonitordataquery_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/barchartpanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/barchartpanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/bargaugepanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/bargaugepanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/cloudwatchdataquery_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/cloudwatchdataquery_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/dashboard_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/dashboard_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/dashboardlistpanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/dashboardlistpanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/debugpanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/debugpanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/elasticsearchdataquery_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/elasticsearchdataquery_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/gaugepanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/gaugepanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/geomappanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/geomappanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/grafanapyroscopedataquery_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/grafanapyroscopedataquery_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/heatmappanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/heatmappanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/histogrampanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/histogrampanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/librarypanel_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/librarypanel_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/logspanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/logspanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/lokidataquery_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/lokidataquery_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/nodegraphpanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/nodegraphpanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/parcadataquery_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/parcadataquery_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/piechartpanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/piechartpanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/playlist_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/playlist_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/preferences_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/preferences_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/prometheusdataquery_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/prometheusdataquery_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/publicdashboard_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/publicdashboard_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/serviceaccount_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/serviceaccount_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/statetimelinepanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/statetimelinepanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/statpanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/statpanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/statushistorypanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/statushistorypanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/tablepanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/tablepanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/team_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/team_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/tempodataquery_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/tempodataquery_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/testdatadataquery_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/testdatadataquery_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/textpanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/textpanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/timeseriespanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/timeseriespanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/model/trendpanelcfg_types_gen.py` & `grafana_dashboard-0.1.1/grafana_dashboard/model/trendpanelcfg_types_gen.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard/utils.py` & `grafana_dashboard-0.1.1/grafana_dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard.egg-info/PKG-INFO` & `grafana_dashboard-0.1.1/grafana_dashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-dashboard
-Version: 0.1.0
+Version: 0.1.1
 Summary: Write Grafana dashboards in Python, without losing thousands of dashboards in the zoo
 Home-page: https://github.com/fzyzcjy/grafana-dashboard-python
 Author: fzyzcjy
 License: MIT
 Keywords: grafana dashboard json
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `grafana_dashboard-0.1.0/grafana_dashboard.egg-info/SOURCES.txt` & `grafana_dashboard-0.1.1/grafana_dashboard.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 grafana_dashboard/extracted_generated_common_models.py
 grafana_dashboard/grafana_dashboard.py
 grafana_dashboard/manual_models.py
 grafana_dashboard/utils.py
 grafana_dashboard.egg-info/PKG-INFO
 grafana_dashboard.egg-info/SOURCES.txt
 grafana_dashboard.egg-info/dependency_links.txt
+grafana_dashboard.egg-info/entry_points.txt
 grafana_dashboard.egg-info/requires.txt
 grafana_dashboard.egg-info/top_level.txt
 grafana_dashboard/converter/__init__.py
 grafana_dashboard/converter/json_to_python.py
 grafana_dashboard/converter/python_to_json.py
 grafana_dashboard/model/__init__.py
 grafana_dashboard/model/alertgroupspanelcfg_types_gen.py
```

### Comparing `grafana_dashboard-0.1.0/setup.py` & `grafana_dashboard-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     init = open(os.path.join("grafana_dashboard", "__init__.py"), "r").read().split()
     return init[init.index("__version__") + 2][1:-1]
 
 
 def get_install_requires():
     return [
         "pydantic>=1.10.2",
-        "dataclasses>=0.8",
         "rich>=13.4.2",
         "typer>=0.6.1",
     ]
 
 
 setup(
     name="grafana_dashboard",
@@ -52,8 +51,13 @@
         "Programming Language :: Python :: 3.10",
     ],
     keywords="grafana dashboard json",
     packages=find_packages(
         exclude=["test", "test.*", "examples", "examples.*", "docs", "docs.*"]
     ),
     install_requires=get_install_requires(),
+    entry_points={
+        'console_scripts': [
+            'grafana_dashboard = grafana_dashboard.grafana_dashboard:run',
+        ],
+    },
 )
```

