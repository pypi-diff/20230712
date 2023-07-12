# Comparing `tmp/biotrade-0.2.4.tar.gz` & `tmp/biotrade-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotrade-0.2.4.tar", last modified: Wed Jul 12 09:11:28 2023, max compression
+gzip compressed data, was "biotrade-0.2.5.tar", last modified: Wed Jul 12 09:45:33 2023, max compression
```

## Comparing `biotrade-0.2.4.tar` & `biotrade-0.2.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.939033 biotrade-0.2.4/
--rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.2.4/LICENCE.md
--rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.2.4/MANIFEST.in
--rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.2.4/NOTICE.txt
--rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-07-12 09:11:28.939033 biotrade-0.2.4/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     7600 2023-06-26 14:05:44.000000 biotrade-0.2.4/README.md
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.903033 biotrade-0.2.4/biotrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     3634 2023-07-12 09:10:21.000000 biotrade-0.2.4/biotrade/__init__.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.911033 biotrade-0.2.4/biotrade/common/
--rw-r--r--   0 paul      (1000) paul      (1000)    13743 2023-06-26 13:47:11.000000 biotrade-0.2.4/biotrade/common/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)    20436 2023-05-10 16:55:49.000000 biotrade-0.2.4/biotrade/common/compare.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/common/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5731 2023-07-12 09:09:38.000000 biotrade-0.2.4/biotrade/common/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/common/logger.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/common/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)     8972 2023-07-12 09:09:38.000000 biotrade-0.2.4/biotrade/common/reallocate.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/common/sanitize.py
--rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/common/time_series.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.2.4/biotrade/common/update.py
--rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.2.4/biotrade/common/url_request_header.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.911033 biotrade-0.2.4/biotrade/comtrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:50:21.000000 biotrade-0.2.4/biotrade/comtrade/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.2.4/biotrade/comtrade/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.2.4/biotrade/comtrade/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    20233 2023-07-04 08:14:43.000000 biotrade-0.2.4/biotrade/comtrade/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6819 2023-06-26 13:47:11.000000 biotrade-0.2.4/biotrade/comtrade/dump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/comtrade/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    46862 2023-06-26 13:50:21.000000 biotrade-0.2.4/biotrade/comtrade/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/comtrade/quality.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.919033 biotrade-0.2.4/biotrade/config_data/
--rw-r--r--   0 paul      (1000) paul      (1000)     3860 2023-06-26 13:50:21.000000 biotrade-0.2.4/biotrade/config_data/column_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6719 2023-06-26 13:50:21.000000 biotrade-0.2.4/biotrade/config_data/comtrade_faostat_product_mapping.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.2.4/biotrade/config_data/comtrade_hs_2d.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.2.4/biotrade/config_data/comtrade_hs_product_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.2.4/biotrade/config_data/comtrade_reporters.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     5480 2023-07-04 13:18:13.000000 biotrade-0.2.4/biotrade/config_data/faostat_commodity_tree.csv
--rw-r--r--   0 paul      (1000) paul      (1000)    43339 2023-06-26 13:50:21.000000 biotrade-0.2.4/biotrade/config_data/faostat_country_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.2.4/biotrade/config_data/faostat_forestry_production_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.2.4/biotrade/config_data/faostat_forestry_production_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.2.4/biotrade/config_data/faostat_forestry_trade_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.2.4/biotrade/config_data/faostat_products_name_code_shortname.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.2.4/biotrade/config_data/regulation_front_end_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)   233668 2023-06-26 13:50:21.000000 biotrade-0.2.4/biotrade/config_data/regulation_products.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.2.4/biotrade/config_data/wood_product_aggregates.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.923033 biotrade-0.2.4/biotrade/eurostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.2.4/biotrade/eurostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4632 2023-06-26 14:05:44.000000 biotrade-0.2.4/biotrade/eurostat/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.927033 biotrade-0.2.4/biotrade/faostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/faostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.2.4/biotrade/faostat/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.2.4/biotrade/faostat/coefficients.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/faostat/convert.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/faostat/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:47:11.000000 biotrade-0.2.4/biotrade/faostat/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    23993 2023-07-04 08:14:43.000000 biotrade-0.2.4/biotrade/faostat/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4179 2023-06-08 08:14:15.000000 biotrade-0.2.4/biotrade/faostat/mirror.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/faostat/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    18105 2023-05-10 13:26:24.000000 biotrade-0.2.4/biotrade/faostat/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/faostat/quality.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/faostat/share_coefficients.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.927033 biotrade-0.2.4/biotrade/hwp/
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.2.4/biotrade/hwp/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/hwp/country.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.931033 biotrade-0.2.4/biotrade/tests/
--rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/tests/test_aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3469 2023-06-26 13:50:21.000000 biotrade-0.2.4/biotrade/tests/test_front_end.py
--rw-r--r--   0 paul      (1000) paul      (1000)      837 2023-05-15 17:30:05.000000 biotrade-0.2.4/biotrade/tests/test_mirror.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3336 2023-07-07 08:40:14.000000 biotrade-0.2.4/biotrade/tests/test_reallocate.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.931033 biotrade-0.2.4/biotrade/world_bank/
--rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/world_bank/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.2.4/biotrade/world_bank/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     9162 2023-05-15 15:21:01.000000 biotrade-0.2.4/biotrade/world_bank/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.907033 biotrade-0.2.4/biotrade.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-07-12 09:11:28.000000 biotrade-0.2.4/biotrade.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     2723 2023-07-12 09:11:28.000000 biotrade-0.2.4/biotrade.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-07-12 09:11:28.000000 biotrade-0.2.4/biotrade.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      130 2023-07-12 09:11:28.000000 biotrade-0.2.4/biotrade.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       43 2023-07-12 09:11:28.000000 biotrade-0.2.4/biotrade.egg-info/top_level.txt
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.903033 biotrade-0.2.4/scripts/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.935033 biotrade-0.2.4/scripts/front_end/
--rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-04-18 16:19:04.000000 biotrade-0.2.4/scripts/front_end/DEPRECATED_reporter_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2583 2023-06-26 13:50:21.000000 biotrade-0.2.4/scripts/front_end/annual_variation_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6622 2023-07-04 08:14:43.000000 biotrade-0.2.4/scripts/front_end/annual_variation_trade_quantity_value.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3571 2023-06-26 13:50:21.000000 biotrade-0.2.4/scripts/front_end/average_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)    10192 2023-07-04 08:14:43.000000 biotrade-0.2.4/scripts/front_end/average_trade_quantity.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.2.4/scripts/front_end/db_scheduler.py
--rw-r--r--   0 paul      (1000) paul      (1000)    27527 2023-07-04 08:14:43.000000 biotrade-0.2.4/scripts/front_end/functions.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-04-18 16:19:04.000000 biotrade-0.2.4/scripts/front_end/product_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3819 2023-07-04 08:14:43.000000 biotrade-0.2.4/scripts/front_end/trends_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.2.4/scripts/front_end/trends_trade_quantity.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:11:28.939033 biotrade-0.2.4/scripts/quality/
--rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.2.4/scripts/quality/faostat_compare_aggregates_to_constituents.py
--rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-07-12 09:11:28.939033 biotrade-0.2.4/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1651 2023-07-12 09:10:21.000000 biotrade-0.2.4/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.573076 biotrade-0.2.5/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.2.5/LICENCE.md
+-rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.2.5/MANIFEST.in
+-rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.2.5/NOTICE.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-07-12 09:45:33.573076 biotrade-0.2.5/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     7600 2023-06-26 14:05:44.000000 biotrade-0.2.5/README.md
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.545076 biotrade-0.2.5/biotrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3634 2023-07-12 09:43:16.000000 biotrade-0.2.5/biotrade/__init__.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.549076 biotrade-0.2.5/biotrade/common/
+-rw-r--r--   0 paul      (1000) paul      (1000)    13743 2023-06-26 13:47:11.000000 biotrade-0.2.5/biotrade/common/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    20436 2023-05-10 16:55:49.000000 biotrade-0.2.5/biotrade/common/compare.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/common/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5731 2023-07-12 09:09:38.000000 biotrade-0.2.5/biotrade/common/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/common/logger.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/common/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     8972 2023-07-12 09:09:38.000000 biotrade-0.2.5/biotrade/common/reallocate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/common/sanitize.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/common/time_series.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.2.5/biotrade/common/update.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.2.5/biotrade/common/url_request_header.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.553076 biotrade-0.2.5/biotrade/comtrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:50:21.000000 biotrade-0.2.5/biotrade/comtrade/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.2.5/biotrade/comtrade/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.2.5/biotrade/comtrade/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    20233 2023-07-04 08:14:43.000000 biotrade-0.2.5/biotrade/comtrade/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6819 2023-06-26 13:47:11.000000 biotrade-0.2.5/biotrade/comtrade/dump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/comtrade/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    46862 2023-06-26 13:50:21.000000 biotrade-0.2.5/biotrade/comtrade/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/comtrade/quality.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.557076 biotrade-0.2.5/biotrade/config_data/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3860 2023-06-26 13:50:21.000000 biotrade-0.2.5/biotrade/config_data/column_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6719 2023-06-26 13:50:21.000000 biotrade-0.2.5/biotrade/config_data/comtrade_faostat_product_mapping.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.2.5/biotrade/config_data/comtrade_hs_2d.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.2.5/biotrade/config_data/comtrade_hs_product_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.2.5/biotrade/config_data/comtrade_reporters.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     5480 2023-07-04 13:18:13.000000 biotrade-0.2.5/biotrade/config_data/faostat_commodity_tree.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)    43339 2023-06-26 13:50:21.000000 biotrade-0.2.5/biotrade/config_data/faostat_country_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.2.5/biotrade/config_data/faostat_forestry_production_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.2.5/biotrade/config_data/faostat_forestry_production_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.2.5/biotrade/config_data/faostat_forestry_trade_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.2.5/biotrade/config_data/faostat_products_name_code_shortname.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.2.5/biotrade/config_data/regulation_front_end_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)   233668 2023-06-26 13:50:21.000000 biotrade-0.2.5/biotrade/config_data/regulation_products.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.2.5/biotrade/config_data/wood_product_aggregates.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.557076 biotrade-0.2.5/biotrade/eurostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.2.5/biotrade/eurostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4632 2023-06-26 14:05:44.000000 biotrade-0.2.5/biotrade/eurostat/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.565076 biotrade-0.2.5/biotrade/faostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/faostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.2.5/biotrade/faostat/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.2.5/biotrade/faostat/coefficients.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/faostat/convert.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/faostat/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:47:11.000000 biotrade-0.2.5/biotrade/faostat/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    23993 2023-07-04 08:14:43.000000 biotrade-0.2.5/biotrade/faostat/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4179 2023-06-08 08:14:15.000000 biotrade-0.2.5/biotrade/faostat/mirror.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/faostat/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    18119 2023-07-12 09:30:56.000000 biotrade-0.2.5/biotrade/faostat/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/faostat/quality.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/faostat/share_coefficients.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.565076 biotrade-0.2.5/biotrade/hwp/
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.2.5/biotrade/hwp/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/hwp/country.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.565076 biotrade-0.2.5/biotrade/tests/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/tests/test_aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3469 2023-06-26 13:50:21.000000 biotrade-0.2.5/biotrade/tests/test_front_end.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      837 2023-05-15 17:30:05.000000 biotrade-0.2.5/biotrade/tests/test_mirror.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3580 2023-07-12 09:43:16.000000 biotrade-0.2.5/biotrade/tests/test_reallocate.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.565076 biotrade-0.2.5/biotrade/world_bank/
+-rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/world_bank/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.2.5/biotrade/world_bank/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     9058 2023-07-12 09:30:56.000000 biotrade-0.2.5/biotrade/world_bank/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.545076 biotrade-0.2.5/biotrade.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-07-12 09:45:33.000000 biotrade-0.2.5/biotrade.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     2723 2023-07-12 09:45:33.000000 biotrade-0.2.5/biotrade.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-07-12 09:45:33.000000 biotrade-0.2.5/biotrade.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      130 2023-07-12 09:45:33.000000 biotrade-0.2.5/biotrade.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       43 2023-07-12 09:45:33.000000 biotrade-0.2.5/biotrade.egg-info/top_level.txt
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.541076 biotrade-0.2.5/scripts/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.569076 biotrade-0.2.5/scripts/front_end/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-04-18 16:19:04.000000 biotrade-0.2.5/scripts/front_end/DEPRECATED_reporter_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2583 2023-06-26 13:50:21.000000 biotrade-0.2.5/scripts/front_end/annual_variation_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6622 2023-07-04 08:14:43.000000 biotrade-0.2.5/scripts/front_end/annual_variation_trade_quantity_value.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3571 2023-06-26 13:50:21.000000 biotrade-0.2.5/scripts/front_end/average_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    10192 2023-07-04 08:14:43.000000 biotrade-0.2.5/scripts/front_end/average_trade_quantity.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.2.5/scripts/front_end/db_scheduler.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    27527 2023-07-04 08:14:43.000000 biotrade-0.2.5/scripts/front_end/functions.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-04-18 16:19:04.000000 biotrade-0.2.5/scripts/front_end/product_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3819 2023-07-04 08:14:43.000000 biotrade-0.2.5/scripts/front_end/trends_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.2.5/scripts/front_end/trends_trade_quantity.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-12 09:45:33.573076 biotrade-0.2.5/scripts/quality/
+-rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.2.5/scripts/quality/faostat_compare_aggregates_to_constituents.py
+-rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-07-12 09:45:33.573076 biotrade-0.2.5/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)     1651 2023-07-12 09:43:16.000000 biotrade-0.2.5/setup.py
```

### Comparing `biotrade-0.2.4/LICENCE.md` & `biotrade-0.2.5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/NOTICE.txt` & `biotrade-0.2.5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/PKG-INFO` & `biotrade-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotrade
-Version: 0.2.4
+Version: 0.2.5
 Summary: Agriculture and forestry statistics.
 Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
 Author: Paul Rougieux, Selene Patani
 Author-email: paul.rougieux@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `biotrade-0.2.4/README.md` & `biotrade-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/__init__.py` & `biotrade-0.2.5/biotrade/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     >>> print("database_url:", biotrade.database_url)
 
 """
 
 from pathlib import Path
 import os
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 module_dir = Path(__file__).resolve().parent
 
 # Where is the data, default case
 data_dir = Path.home() / "repos/forobs/biotrade_data/"
 
 # But you can override that with an environment variable
```

### Comparing `biotrade-0.2.4/biotrade/common/aggregate.py` & `biotrade-0.2.5/biotrade/common/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/compare.py` & `biotrade-0.2.5/biotrade/common/compare.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/country.py` & `biotrade-0.2.5/biotrade/common/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/database.py` & `biotrade-0.2.5/biotrade/common/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/logger.py` & `biotrade-0.2.5/biotrade/common/logger.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/products.py` & `biotrade-0.2.5/biotrade/common/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/reallocate.py` & `biotrade-0.2.5/biotrade/common/reallocate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/sanitize.py` & `biotrade-0.2.5/biotrade/common/sanitize.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/time_series.py` & `biotrade-0.2.5/biotrade/common/time_series.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/update.py` & `biotrade-0.2.5/biotrade/common/update.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/common/url_request_header.py` & `biotrade-0.2.5/biotrade/common/url_request_header.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/comtrade/__init__.py` & `biotrade-0.2.5/biotrade/comtrade/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/comtrade/aggregate.py` & `biotrade-0.2.5/biotrade/comtrade/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/comtrade/country_groups.py` & `biotrade-0.2.5/biotrade/comtrade/country_groups.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/comtrade/database.py` & `biotrade-0.2.5/biotrade/comtrade/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/comtrade/dump.py` & `biotrade-0.2.5/biotrade/comtrade/dump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/comtrade/products.py` & `biotrade-0.2.5/biotrade/comtrade/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/comtrade/pump.py` & `biotrade-0.2.5/biotrade/comtrade/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/comtrade/quality.py` & `biotrade-0.2.5/biotrade/comtrade/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/column_names.csv` & `biotrade-0.2.5/biotrade/config_data/column_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/comtrade_faostat_product_mapping.csv` & `biotrade-0.2.5/biotrade/config_data/comtrade_faostat_product_mapping.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/comtrade_hs_2d.csv` & `biotrade-0.2.5/biotrade/config_data/comtrade_hs_2d.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/comtrade_hs_product_short_names.csv` & `biotrade-0.2.5/biotrade/config_data/comtrade_hs_product_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/comtrade_reporters.csv` & `biotrade-0.2.5/biotrade/config_data/comtrade_reporters.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/faostat_commodity_tree.csv` & `biotrade-0.2.5/biotrade/config_data/faostat_commodity_tree.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/faostat_country_groups.csv` & `biotrade-0.2.5/biotrade/config_data/faostat_country_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/faostat_forestry_production_groups.csv` & `biotrade-0.2.5/biotrade/config_data/faostat_forestry_production_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/faostat_forestry_production_short_names.csv` & `biotrade-0.2.5/biotrade/config_data/faostat_forestry_production_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/faostat_forestry_trade_groups.csv` & `biotrade-0.2.5/biotrade/config_data/faostat_forestry_trade_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/faostat_products_name_code_shortname.csv` & `biotrade-0.2.5/biotrade/config_data/faostat_products_name_code_shortname.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/regulation_front_end_groups.csv` & `biotrade-0.2.5/biotrade/config_data/regulation_front_end_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/regulation_products.csv` & `biotrade-0.2.5/biotrade/config_data/regulation_products.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/config_data/wood_product_aggregates.csv` & `biotrade-0.2.5/biotrade/config_data/wood_product_aggregates.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/eurostat/__init__.py` & `biotrade-0.2.5/biotrade/eurostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/eurostat/pump.py` & `biotrade-0.2.5/biotrade/eurostat/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/__init__.py` & `biotrade-0.2.5/biotrade/faostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/aggregate.py` & `biotrade-0.2.5/biotrade/faostat/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/convert.py` & `biotrade-0.2.5/biotrade/faostat/convert.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/country.py` & `biotrade-0.2.5/biotrade/faostat/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/country_groups.py` & `biotrade-0.2.5/biotrade/faostat/country_groups.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/database.py` & `biotrade-0.2.5/biotrade/faostat/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/mirror.py` & `biotrade-0.2.5/biotrade/faostat/mirror.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/products.py` & `biotrade-0.2.5/biotrade/faostat/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/pump.py` & `biotrade-0.2.5/biotrade/faostat/pump.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
                 )
                 if temp_dir.exists():
                     # Remove temporary directory
                     shutil.rmtree(temp_dir)
                 return
         # Drop and recreate the table
         table = self.db.tables[short_name]
-        table.drop()
+        table.drop(self.db.engine)
         self.db.create_if_not_existing(table)
         # Read in chunk and pass each chunk to the database
         for df_chunk in pandas.read_csv(
             csv_file_name, chunksize=chunk_size, encoding=encoding_var
         ):
             df_chunk = self.sanitize_variable_names(
                 df_chunk, choose_column_renaming(short_name), short_name
```

### Comparing `biotrade-0.2.4/biotrade/faostat/quality.py` & `biotrade-0.2.5/biotrade/faostat/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/faostat/share_coefficients.py` & `biotrade-0.2.5/biotrade/faostat/share_coefficients.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/hwp/country.py` & `biotrade-0.2.5/biotrade/hwp/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/tests/test_aggregate.py` & `biotrade-0.2.5/biotrade/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/tests/test_front_end.py` & `biotrade-0.2.5/biotrade/tests/test_front_end.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/tests/test_mirror.py` & `biotrade-0.2.5/biotrade/tests/test_mirror.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/tests/test_reallocate.py` & `biotrade-0.2.5/biotrade/tests/test_reallocate.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,19 +43,28 @@
 
 def test_split_prod_imp():
     df = pandas.DataFrame(
         {
             "reporter": ["a", "b", "c"],
             "reporter_code": [1, 2, 3],
             "primary_product": ["p", "p", "q"],
+            "year": 1,
             "primary_eq_0": [1, 2, 4],
+        }
+    )
+    df_share = pandas.DataFrame(
+        {
+            "reporter": ["a", "b", "c"],
+            "reporter_code": [1, 2, 3],
+            "primary_product": ["p", "p", "q"],
+            "year": 1,
             "share_prod_imp": [0, 1, 0.5],
         }
     )
-    output_prod, output_imp = split_prod_imp(df, 1)
+    output_prod, output_imp = split_prod_imp(df, df_share, 1)
     # Use float in the expected series to avoid AssertionError: Attributes of
     # Series are different Attribute "dtype" are different [left]:  float64
     # [right]: int64
     expected_prod = pandas.Series([0, 2, 2.0])
     expected_imp = pandas.Series([1, 0, 2.0])
     assert_series_equal(output_prod, expected_prod)
     assert_series_equal(output_imp, expected_imp)
```

### Comparing `biotrade-0.2.4/biotrade/world_bank/__init__.py` & `biotrade-0.2.5/biotrade/world_bank/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/world_bank/database.py` & `biotrade-0.2.5/biotrade/world_bank/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/biotrade/world_bank/pump.py` & `biotrade-0.2.5/biotrade/world_bank/pump.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 from zipfile import ZipFile
 import tempfile
 import logging
 
 try:
     import requests
 except Exception as e:
-    msg = "Failed to import requests, you will not be able to load data from World Bank,"
+    msg = (
+        "Failed to import requests, you will not be able to load data from World Bank,"
+    )
     msg += "but you can still use other methods.\n"
     print(msg, str(e))
 import shutil
 import pandas as pd
 import csv
 
 # Internal modules
@@ -79,24 +81,20 @@
         self.chunk_size = 10**4
 
     def download_zip_csv(self):
         """download a compressed csv file containing all World Bank indicators"""
         # Load the zip file to the data directory
         output_file = self.data_dir / self.zip_file_name
         self.logger.info("Downloading data from:\n %s", self.url_bulk)
-        response = requests.get(
-            url=self.url_bulk, headers=self.header, stream=True
-        )
+        response = requests.get(url=self.url_bulk, headers=self.header, stream=True)
         with open(output_file, "wb") as out_file:
             print(f"HTTP response code: {response.status_code}")
             shutil.copyfileobj(response.raw, out_file)
 
-    def transfer_csv_to_db_in_chunks(
-        self, short_name, chunk_size, reformatting
-    ):
+    def transfer_csv_to_db_in_chunks(self, short_name, chunk_size, reformatting):
         """Read the World Bank zip csv file and transfer large long format CSV
         file to the database in chunks so that a data frame with millions of
         rows doesn't overload the memory."""
         temp_dir = Path(tempfile.TemporaryDirectory().name)
         try:
             # Unzip the CSV and write it to a temporary file on disk
             zip_file = ZipFile(self.data_dir / self.zip_file_name)
@@ -111,17 +109,15 @@
                 "Indicator Code",
             ]
             if reformatting:
                 # Retrieve series file to append unit column for indicator table
                 unit_file = temp_dir / "WDISeries.csv"
                 df_unit = pd.read_csv(unit_file)
                 # Rename column same as csv file
-                df_unit.rename(
-                    columns={"Series Code": "Indicator Code"}, inplace=True
-                )
+                df_unit.rename(columns={"Series Code": "Indicator Code"}, inplace=True)
                 # Keep only columns needed for the merge
                 df_unit = df_unit[["Indicator Code", "Unit of measure"]]
             else:
                 # Do not split the dataframe into chunks (len(df) = 383572)
                 chunk_size = 10**6
             # Test if the file is corrupted
             with open(csv_file, "r") as csvfile:
@@ -141,22 +137,20 @@
             )
             if temp_dir.exists():
                 # Remove temporary directory
                 shutil.rmtree(temp_dir)
             return
         # Drop and recreate the table
         table = self.db.tables[short_name]
-        table.drop()
+        table.drop(self.db.engine)
         self.db.create_if_not_existing(table)
         # Read the csv file, transform the dataframe and upload data to the database
         for df_chunk in pd.read_csv(csv_file, chunksize=chunk_size):
             # Remove unnamed columns
-            df_chunk.drop(
-                df_chunk.filter(regex="Unnamed"), axis=1, inplace=True
-            )
+            df_chunk.drop(df_chunk.filter(regex="Unnamed"), axis=1, inplace=True)
             if reformatting:
                 # Reformatting year columns into long format
                 df_chunk = df_chunk.melt(
                     id_vars=id_columns, var_name="year", value_name="value"
                 )
                 # Merge with unit column
                 df_chunk = df_chunk.merge(
@@ -210,17 +204,15 @@
         for table_name in datasets:
             # Keep as default reformatting csv to long years format
             reformatting = True
             if table_name == "indicator_name":
                 # Do not reformat the csv file
                 reformatting = False
             # Transfer the compressed CSV file to the database
-            self.transfer_csv_to_db_in_chunks(
-                table_name, self.chunk_size, reformatting
-            )
+            self.transfer_csv_to_db_in_chunks(table_name, self.chunk_size, reformatting)
 
     def update(self, datasets, skip_confirmation=False):
         """Update the given datasets by downloading them from World Bank Data and
         transferring them to the database
 
         :param list or str datasets: list of dataset names, whose keys should
             be in the world_bank.pump.datasets and world_bank.db.tables dictionaries
```

### Comparing `biotrade-0.2.4/biotrade.egg-info/PKG-INFO` & `biotrade-0.2.5/biotrade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotrade
-Version: 0.2.4
+Version: 0.2.5
 Summary: Agriculture and forestry statistics.
 Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
 Author: Paul Rougieux, Selene Patani
 Author-email: paul.rougieux@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `biotrade-0.2.4/biotrade.egg-info/SOURCES.txt` & `biotrade-0.2.5/biotrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/DEPRECATED_reporter_list.py` & `biotrade-0.2.5/scripts/front_end/DEPRECATED_reporter_list.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/annual_variation_harvested_area_production.py` & `biotrade-0.2.5/scripts/front_end/annual_variation_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/annual_variation_trade_quantity_value.py` & `biotrade-0.2.5/scripts/front_end/annual_variation_trade_quantity_value.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/average_harvested_area_production.py` & `biotrade-0.2.5/scripts/front_end/average_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/average_trade_quantity.py` & `biotrade-0.2.5/scripts/front_end/average_trade_quantity.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/db_scheduler.py` & `biotrade-0.2.5/scripts/front_end/db_scheduler.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/functions.py` & `biotrade-0.2.5/scripts/front_end/functions.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/product_list.py` & `biotrade-0.2.5/scripts/front_end/product_list.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/trends_harvested_area_production.py` & `biotrade-0.2.5/scripts/front_end/trends_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/front_end/trends_trade_quantity.py` & `biotrade-0.2.5/scripts/front_end/trends_trade_quantity.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/scripts/quality/faostat_compare_aggregates_to_constituents.py` & `biotrade-0.2.5/scripts/quality/faostat_compare_aggregates_to_constituents.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.4/setup.py` & `biotrade-0.2.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 readme_path = path.join(this_dir, "README.md")
 with open(readme_path, encoding="utf-8") as handle:
     readme = handle.read()
 
 # Call setup #
 setup(
     name="biotrade",
-    version="0.2.4",
+    version="0.2.5",
     description="Agriculture and forestry statistics.",
     license="MIT",
     url="https://gitlab.com/bioeconomy/forobs/biotrade/",
     author="Paul Rougieux, Selene Patani",
     author_email="paul.rougieux@gmail.com",
     packages=find_namespace_packages(exclude=["notebooks", "scripts"]),
     install_requires=[
```

