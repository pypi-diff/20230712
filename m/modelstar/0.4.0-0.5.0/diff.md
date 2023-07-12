# Comparing `tmp/modelstar-0.4.0.tar.gz` & `tmp/modelstar-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelstar-0.4.0.tar", max compression
+gzip compressed data, was "modelstar-0.5.0.tar", max compression
```

## Comparing `modelstar-0.4.0.tar` & `modelstar-0.5.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0    11361 2022-11-11 16:44:25.395547 modelstar-0.4.0/LICENSE
--rw-r--r--   0        0        0     1235 2022-11-11 16:40:58.498029 modelstar-0.4.0/README.md
--rw-r--r--   0        0        0      864 2022-11-30 10:05:35.261819 modelstar-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      337 2022-11-29 17:54:37.014873 modelstar-0.4.0/src/modelstar/__init__.py
--rw-r--r--   0        0        0       53 2022-11-06 12:12:08.220726 modelstar-0.4.0/src/modelstar/builtins/__init__.py
--rw-r--r--   0        0        0        0 2022-11-06 12:12:08.220811 modelstar-0.4.0/src/modelstar/builtins/functions/__init__.py
--rw-r--r--   0        0        0       74 2022-11-18 13:47:18.095670 modelstar-0.4.0/src/modelstar/builtins/packages/__init__.py
--rw-r--r--   0        0        0  1887204 2022-11-28 18:58:05.078915 modelstar-0.4.0/src/modelstar/builtins/packages/pycaret.zip
--rw-r--r--   0        0        0        0 2022-11-06 12:12:08.220908 modelstar-0.4.0/src/modelstar/builtins/procedures/__init__.py
--rw-r--r--   0        0        0     3975 2022-11-29 18:26:20.103154 modelstar-0.4.0/src/modelstar/builtins/procedures/binary_classifier.py
--rw-r--r--   0        0        0     2753 2022-11-11 17:34:52.560322 modelstar-0.4.0/src/modelstar/builtins/procedures/univariate_time_series_forecast.py
--rw-r--r--   0        0        0     9080 2022-11-29 11:18:48.064068 modelstar-0.4.0/src/modelstar/cli.py
--rw-r--r--   0        0        0        0 2022-11-06 12:12:08.221701 modelstar-0.4.0/src/modelstar/commands/__init__.py
--rw-r--r--   0        0        0     1930 2022-11-06 15:28:10.157787 modelstar-0.4.0/src/modelstar/commands/create.py
--rw-r--r--   0        0        0      344 2022-11-06 15:49:10.355796 modelstar-0.4.0/src/modelstar/commands/database.py
--rw-r--r--   0        0        0     2112 2022-11-28 20:50:33.242374 modelstar-0.4.0/src/modelstar/commands/download.py
--rw-r--r--   0        0        0     2176 2022-11-10 14:18:53.501887 modelstar-0.4.0/src/modelstar/commands/project.py
--rw-r--r--   0        0        0     5162 2022-11-29 11:58:18.221328 modelstar-0.4.0/src/modelstar/commands/register.py
--rw-r--r--   0        0        0      487 2022-11-06 12:12:08.222307 modelstar-0.4.0/src/modelstar/commands/run.py
--rw-r--r--   0        0        0      443 2022-11-06 12:12:08.222386 modelstar-0.4.0/src/modelstar/commands/upload.py
--rw-r--r--   0        0        0        0 2022-11-06 12:12:08.222462 modelstar-0.4.0/src/modelstar/connectors/__init__.py
--rw-r--r--   0        0        0        0 2022-11-06 12:12:08.222562 modelstar-0.4.0/src/modelstar/connectors/snowflake/__init__.py
--rw-r--r--   0        0        0     9645 2022-11-06 12:12:08.222723 modelstar-0.4.0/src/modelstar/connectors/snowflake/context.py
--rw-r--r--   0        0        0     1556 2022-11-06 12:12:08.222808 modelstar-0.4.0/src/modelstar/connectors/snowflake/context_types.py
--rw-r--r--   0        0        0     6283 2022-11-29 18:33:11.476541 modelstar-0.4.0/src/modelstar/connectors/snowflake/modelstar/__init__.py
--rw-r--r--   0        0        0     3307 2022-11-29 11:22:16.349920 modelstar-0.4.0/src/modelstar/connectors/snowflake/sql_dialect/__init__.py
--rw-r--r--   0        0        0     4299 2022-11-29 18:00:36.546434 modelstar-0.4.0/src/modelstar/connectors/snowflake/sql_dialect/register_sproc.py
--rw-r--r--   0        0        0     1204 2022-11-29 11:20:21.353935 modelstar-0.4.0/src/modelstar/connectors/snowflake/sql_dialect/register_udf.py
--rw-r--r--   0        0        0      394 2022-11-06 12:12:08.223210 modelstar-0.4.0/src/modelstar/connectors/snowflake/utils.py
--rw-r--r--   0        0        0        0 2022-11-06 12:12:08.223299 modelstar-0.4.0/src/modelstar/executors/__init__.py
--rw-r--r--   0        0        0     3744 2022-11-06 19:23:38.632787 modelstar-0.4.0/src/modelstar/executors/config.py
--rw-r--r--   0        0        0     2170 2022-11-06 12:12:08.223499 modelstar-0.4.0/src/modelstar/executors/project.py
--rw-r--r--   0        0        0      606 2022-11-06 12:12:08.223621 modelstar-0.4.0/src/modelstar/executors/py_parser/__init__.py
--rw-r--r--   0        0        0    56893 2022-11-18 15:37:51.137787 modelstar-0.4.0/src/modelstar/executors/py_parser/implib_snowflake.py
--rw-r--r--   0        0        0     3230 2022-11-06 12:12:08.224035 modelstar-0.4.0/src/modelstar/executors/py_parser/implib_stdlib.py
--rw-r--r--   0        0        0     1647 2022-11-06 12:12:08.224162 modelstar-0.4.0/src/modelstar/executors/py_parser/module_call.py
--rw-r--r--   0        0        0     3573 2022-11-29 11:55:45.358176 modelstar-0.4.0/src/modelstar/executors/py_parser/module_function.py
--rw-r--r--   0        0        0     3098 2022-11-18 15:11:42.432808 modelstar-0.4.0/src/modelstar/executors/py_parser/module_import.py
--rw-r--r--   0        0        0     2424 2022-11-06 12:12:08.224433 modelstar-0.4.0/src/modelstar/executors/py_parser/node_visitor.py
--rw-r--r--   0        0        0     1258 2022-11-06 12:12:08.224518 modelstar-0.4.0/src/modelstar/executors/py_parser/parse_exceptions.py
--rw-r--r--   0        0        0     1734 2022-11-28 20:54:43.969519 modelstar-0.4.0/src/modelstar/executors/report.py
--rw-r--r--   0        0        0        0 2022-11-06 12:12:08.224634 modelstar-0.4.0/src/modelstar/executors/session.py
--rw-r--r--   0        0        0     1473 2022-11-06 12:12:08.224735 modelstar-0.4.0/src/modelstar/executors/table.py
--rw-r--r--   0        0        0       54 2022-11-06 12:12:08.224845 modelstar-0.4.0/src/modelstar/templates/__init__.py
--rw-r--r--   0        0        0        0 2022-11-06 12:12:08.224924 modelstar-0.4.0/src/modelstar/templates/report/__init__.py
--rw-r--r--   0        0        0      614 2022-11-28 21:16:01.196411 modelstar-0.4.0/src/modelstar/templates/report/base.html
--rw-r--r--   0        0        0     2345 2022-11-28 21:18:38.900605 modelstar-0.4.0/src/modelstar/templates/report/includes/custom.styles.css
--rw-r--r--   0        0        0     4356 2022-11-28 21:45:51.559372 modelstar-0.4.0/src/modelstar/templates/report/includes/main.styles.css
--rw-r--r--   0        0        0     6428 2022-11-06 12:12:08.225346 modelstar-0.4.0/src/modelstar/templates/report/includes/normalize.styles.css
--rw-r--r--   0        0        0     2510 2022-11-06 12:12:08.225450 modelstar-0.4.0/src/modelstar/templates/report/includes/simple-grid.css
--rw-r--r--   0        0        0     1658 2022-11-06 12:12:08.225538 modelstar-0.4.0/src/modelstar/templates/report/includes/simple-grid.min.css
--rw-r--r--   0        0        0    11452 2022-11-06 12:12:08.225648 modelstar-0.4.0/src/modelstar/templates/report/includes/skeleton.css
--rw-r--r--   0        0        0     1438 2022-11-28 21:46:12.459230 modelstar-0.4.0/src/modelstar/templates/report/report.html
--rw-r--r--   0        0        0     4135 2022-11-06 12:12:08.225846 modelstar-0.4.0/src/modelstar/templates/snowflake_project/.gitignore
--rw-r--r--   0        0        0      902 2022-11-10 14:17:42.856979 modelstar-0.4.0/src/modelstar/templates/snowflake_project/README.md
--rw-r--r--   0        0        0      327 2022-11-10 14:17:03.139599 modelstar-0.4.0/src/modelstar/templates/snowflake_project/modelstar.config.yaml
--rw-r--r--   0        0        0   971878 2022-11-30 09:58:45.277307 modelstar-0.4.0/src/modelstar/templates/snowflake_project/sample_data/customer_data.csv
--rw-r--r--   0        0        0    81031 2022-11-06 16:12:05.272293 modelstar-0.4.0/src/modelstar/templates/snowflake_project/sample_data/sales.csv
--rw-r--r--   0        0        0     4135 2022-11-07 11:44:52.937019 modelstar-0.4.0/src/modelstar/templates/starter_kit/.gitignore
--rw-r--r--   0        0        0      974 2022-11-07 11:44:52.938291 modelstar-0.4.0/src/modelstar/templates/starter_kit/README.md
--rw-r--r--   0        0        0      104 2022-11-07 11:44:52.940089 modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/functions/clients.csv
--rw-r--r--   0        0        0    13641 2022-11-07 11:44:52.940727 modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/functions/country-capitals.csv
--rw-r--r--   0        0        0     1032 2022-11-07 11:44:52.941323 modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/functions/find_capital.py
--rw-r--r--   0        0        0    81031 2022-11-07 11:44:52.942589 modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/machine_learning/sales.csv
--rw-r--r--   0        0        0     2969 2022-11-07 11:44:52.943042 modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/machine_learning/univariate_time_series_forecast.py
--rw-r--r--   0        0        0     4012 2022-11-07 11:44:52.943836 modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/stored_procedure/ad_sales.csv
--rw-r--r--   0        0        0      555 2022-11-07 11:44:52.944396 modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/stored_procedure/inference.py
--rw-r--r--   0        0        0     1026 2022-11-07 11:44:52.944826 modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/stored_procedure/training.py
--rw-r--r--   0        0        0        0 2022-11-06 12:12:08.227425 modelstar-0.4.0/src/modelstar/utils/__init__.py
--rw-r--r--   0        0        0     4495 2022-11-28 20:20:44.008906 modelstar-0.4.0/src/modelstar/utils/logging.py
--rw-r--r--   0        0        0     3224 2022-11-29 18:15:41.387757 modelstar-0.4.0/src/modelstar/utils/path.py
--rw-r--r--   0        0        0      236 2022-11-06 12:12:08.227672 modelstar-0.4.0/src/modelstar/utils/report.py
--rw-r--r--   0        0        0     1815 2022-11-06 12:12:08.227749 modelstar-0.4.0/src/modelstar/utils/response.py
--rw-r--r--   0        0        0     3041 2022-11-18 14:00:56.864332 modelstar-0.4.0/src/modelstar/utils/zip.py
--rw-r--r--   0        0        0       22 2022-11-30 10:06:02.298119 modelstar-0.4.0/src/modelstar/version.py
--rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 modelstar-0.4.0/setup.py
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 modelstar-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11361 2022-11-11 16:44:25.395547 modelstar-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1237 2023-01-20 10:37:03.189605 modelstar-0.5.0/README.md
+-rw-r--r--   0        0        0      864 2023-07-12 11:22:15.181972 modelstar-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      337 2022-11-29 17:54:37.014873 modelstar-0.5.0/src/modelstar/__init__.py
+-rw-r--r--   0        0        0       53 2022-11-06 12:12:08.220726 modelstar-0.5.0/src/modelstar/builtins/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-06 12:12:08.220811 modelstar-0.5.0/src/modelstar/builtins/functions/__init__.py
+-rw-r--r--   0        0        0       74 2022-11-18 13:47:18.095670 modelstar-0.5.0/src/modelstar/builtins/packages/__init__.py
+-rw-r--r--   0        0        0  1887204 2022-11-28 18:58:05.078915 modelstar-0.5.0/src/modelstar/builtins/packages/pycaret.zip
+-rw-r--r--   0        0        0        0 2022-11-06 12:12:08.220908 modelstar-0.5.0/src/modelstar/builtins/procedures/__init__.py
+-rw-r--r--   0        0        0     3975 2022-11-29 18:26:20.103154 modelstar-0.5.0/src/modelstar/builtins/procedures/binary_classifier.py
+-rw-r--r--   0        0        0     4042 2022-12-16 19:22:57.933984 modelstar-0.5.0/src/modelstar/builtins/procedures/classifier.py
+-rw-r--r--   0        0        0     3389 2022-12-16 19:31:05.551716 modelstar-0.5.0/src/modelstar/builtins/procedures/regressor.py
+-rw-r--r--   0        0        0     2753 2022-11-11 17:34:52.560322 modelstar-0.5.0/src/modelstar/builtins/procedures/univariate_time_series_forecast.py
+-rw-r--r--   0        0        0     9860 2023-07-12 11:13:14.399964 modelstar-0.5.0/src/modelstar/cli.py
+-rw-r--r--   0        0        0        0 2022-11-06 12:12:08.221701 modelstar-0.5.0/src/modelstar/commands/__init__.py
+-rw-r--r--   0        0        0     1930 2022-11-06 15:28:10.157787 modelstar-0.5.0/src/modelstar/commands/create.py
+-rw-r--r--   0        0        0      344 2022-11-06 15:49:10.355796 modelstar-0.5.0/src/modelstar/commands/database.py
+-rw-r--r--   0        0        0     2112 2022-11-28 20:50:33.242374 modelstar-0.5.0/src/modelstar/commands/download.py
+-rw-r--r--   0        0        0     2176 2022-11-10 14:18:53.501887 modelstar-0.5.0/src/modelstar/commands/project.py
+-rw-r--r--   0        0        0     5162 2022-11-29 11:58:18.221328 modelstar-0.5.0/src/modelstar/commands/register.py
+-rw-r--r--   0        0        0      487 2022-11-06 12:12:08.222307 modelstar-0.5.0/src/modelstar/commands/run.py
+-rw-r--r--   0        0        0      775 2023-07-05 13:32:56.519569 modelstar-0.5.0/src/modelstar/commands/upload.py
+-rw-r--r--   0        0        0        0 2022-11-06 12:12:08.222462 modelstar-0.5.0/src/modelstar/connectors/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-06 12:12:08.222562 modelstar-0.5.0/src/modelstar/connectors/snowflake/__init__.py
+-rw-r--r--   0        0        0    10150 2023-07-12 11:17:16.013812 modelstar-0.5.0/src/modelstar/connectors/snowflake/context.py
+-rw-r--r--   0        0        0     1556 2022-11-06 12:12:08.222808 modelstar-0.5.0/src/modelstar/connectors/snowflake/context_types.py
+-rw-r--r--   0        0        0     6290 2022-12-16 20:03:12.107788 modelstar-0.5.0/src/modelstar/connectors/snowflake/modelstar/__init__.py
+-rw-r--r--   0        0        0     4199 2023-07-12 11:17:47.577487 modelstar-0.5.0/src/modelstar/connectors/snowflake/sql_dialect/__init__.py
+-rw-r--r--   0        0        0     4299 2022-11-29 18:00:36.546434 modelstar-0.5.0/src/modelstar/connectors/snowflake/sql_dialect/register_sproc.py
+-rw-r--r--   0        0        0     1204 2022-11-29 11:20:21.353935 modelstar-0.5.0/src/modelstar/connectors/snowflake/sql_dialect/register_udf.py
+-rw-r--r--   0        0        0      394 2022-11-06 12:12:08.223210 modelstar-0.5.0/src/modelstar/connectors/snowflake/utils.py
+-rw-r--r--   0        0        0        0 2022-11-06 12:12:08.223299 modelstar-0.5.0/src/modelstar/executors/__init__.py
+-rw-r--r--   0        0        0     3744 2022-11-06 19:23:38.632787 modelstar-0.5.0/src/modelstar/executors/config.py
+-rw-r--r--   0        0        0     2170 2022-11-06 12:12:08.223499 modelstar-0.5.0/src/modelstar/executors/project.py
+-rw-r--r--   0        0        0      606 2022-11-06 12:12:08.223621 modelstar-0.5.0/src/modelstar/executors/py_parser/__init__.py
+-rw-r--r--   0        0        0    56893 2022-11-18 15:37:51.137787 modelstar-0.5.0/src/modelstar/executors/py_parser/implib_snowflake.py
+-rw-r--r--   0        0        0     3230 2022-11-06 12:12:08.224035 modelstar-0.5.0/src/modelstar/executors/py_parser/implib_stdlib.py
+-rw-r--r--   0        0        0     1647 2022-11-06 12:12:08.224162 modelstar-0.5.0/src/modelstar/executors/py_parser/module_call.py
+-rw-r--r--   0        0        0     3573 2022-11-29 11:55:45.358176 modelstar-0.5.0/src/modelstar/executors/py_parser/module_function.py
+-rw-r--r--   0        0        0     3098 2022-11-18 15:11:42.432808 modelstar-0.5.0/src/modelstar/executors/py_parser/module_import.py
+-rw-r--r--   0        0        0     2424 2022-11-06 12:12:08.224433 modelstar-0.5.0/src/modelstar/executors/py_parser/node_visitor.py
+-rw-r--r--   0        0        0     1258 2022-11-06 12:12:08.224518 modelstar-0.5.0/src/modelstar/executors/py_parser/parse_exceptions.py
+-rw-r--r--   0        0        0     1734 2022-11-28 20:54:43.969519 modelstar-0.5.0/src/modelstar/executors/report.py
+-rw-r--r--   0        0        0        0 2022-11-06 12:12:08.224634 modelstar-0.5.0/src/modelstar/executors/session.py
+-rw-r--r--   0        0        0     1473 2022-11-06 12:12:08.224735 modelstar-0.5.0/src/modelstar/executors/table.py
+-rw-r--r--   0        0        0       54 2022-11-06 12:12:08.224845 modelstar-0.5.0/src/modelstar/templates/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-06 12:12:08.224924 modelstar-0.5.0/src/modelstar/templates/report/__init__.py
+-rw-r--r--   0        0        0      614 2022-11-28 21:16:01.196411 modelstar-0.5.0/src/modelstar/templates/report/base.html
+-rw-r--r--   0        0        0     2345 2022-11-28 21:18:38.900605 modelstar-0.5.0/src/modelstar/templates/report/includes/custom.styles.css
+-rw-r--r--   0        0        0     4356 2022-11-28 21:45:51.559372 modelstar-0.5.0/src/modelstar/templates/report/includes/main.styles.css
+-rw-r--r--   0        0        0     6428 2022-11-06 12:12:08.225346 modelstar-0.5.0/src/modelstar/templates/report/includes/normalize.styles.css
+-rw-r--r--   0        0        0     2510 2022-11-06 12:12:08.225450 modelstar-0.5.0/src/modelstar/templates/report/includes/simple-grid.css
+-rw-r--r--   0        0        0     1658 2022-11-06 12:12:08.225538 modelstar-0.5.0/src/modelstar/templates/report/includes/simple-grid.min.css
+-rw-r--r--   0        0        0    11452 2022-11-06 12:12:08.225648 modelstar-0.5.0/src/modelstar/templates/report/includes/skeleton.css
+-rw-r--r--   0        0        0     1438 2022-11-28 21:46:12.459230 modelstar-0.5.0/src/modelstar/templates/report/report.html
+-rw-r--r--   0        0        0     4135 2022-11-06 12:12:08.225846 modelstar-0.5.0/src/modelstar/templates/snowflake_project/.gitignore
+-rw-r--r--   0        0        0      902 2022-11-10 14:17:42.856979 modelstar-0.5.0/src/modelstar/templates/snowflake_project/README.md
+-rw-r--r--   0        0        0      327 2022-11-10 14:17:03.139599 modelstar-0.5.0/src/modelstar/templates/snowflake_project/modelstar.config.yaml
+-rw-r--r--   0        0        0   971878 2022-11-30 09:58:45.277307 modelstar-0.5.0/src/modelstar/templates/snowflake_project/sample_data/customer_data.csv
+-rw-r--r--   0        0        0    81031 2022-11-06 16:12:05.272293 modelstar-0.5.0/src/modelstar/templates/snowflake_project/sample_data/sales.csv
+-rw-r--r--   0        0        0     4135 2022-11-07 11:44:52.937019 modelstar-0.5.0/src/modelstar/templates/starter_kit/.gitignore
+-rw-r--r--   0        0        0      974 2022-11-07 11:44:52.938291 modelstar-0.5.0/src/modelstar/templates/starter_kit/README.md
+-rw-r--r--   0        0        0      104 2022-11-07 11:44:52.940089 modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/functions/clients.csv
+-rw-r--r--   0        0        0    13641 2022-11-07 11:44:52.940727 modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/functions/country-capitals.csv
+-rw-r--r--   0        0        0     1032 2022-11-07 11:44:52.941323 modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/functions/find_capital.py
+-rw-r--r--   0        0        0    81031 2022-11-07 11:44:52.942589 modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/machine_learning/sales.csv
+-rw-r--r--   0        0        0     2969 2022-11-07 11:44:52.943042 modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/machine_learning/univariate_time_series_forecast.py
+-rw-r--r--   0        0        0     4012 2022-11-07 11:44:52.943836 modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/stored_procedure/ad_sales.csv
+-rw-r--r--   0        0        0      555 2022-11-07 11:44:52.944396 modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/stored_procedure/inference.py
+-rw-r--r--   0        0        0     1026 2022-11-07 11:44:52.944826 modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/stored_procedure/training.py
+-rw-r--r--   0        0        0        0 2022-11-06 12:12:08.227425 modelstar-0.5.0/src/modelstar/utils/__init__.py
+-rw-r--r--   0        0        0     4495 2022-11-28 20:20:44.008906 modelstar-0.5.0/src/modelstar/utils/logging.py
+-rw-r--r--   0        0        0     4085 2023-07-05 13:11:54.887852 modelstar-0.5.0/src/modelstar/utils/path.py
+-rw-r--r--   0        0        0      236 2022-11-06 12:12:08.227672 modelstar-0.5.0/src/modelstar/utils/report.py
+-rw-r--r--   0        0        0     1815 2022-11-06 12:12:08.227749 modelstar-0.5.0/src/modelstar/utils/response.py
+-rw-r--r--   0        0        0     3041 2022-11-18 14:00:56.864332 modelstar-0.5.0/src/modelstar/utils/zip.py
+-rw-r--r--   0        0        0       22 2022-11-30 10:06:02.298119 modelstar-0.5.0/src/modelstar/version.py
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 modelstar-0.5.0/PKG-INFO
```

### Comparing `modelstar-0.4.0/LICENSE` & `modelstar-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/README.md` & `modelstar-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 
 ```shell
 $ pip install modelstar
 ```
 
 It's recommended to install `modelstar` within a Python virtual environment using `pyenv`, `virtualenv`, or `poetry`.
 
-For a complete quickstart guide visit [**Modelstar-Quickstart**](https://modelstar.io/docs/quickstar)
+For a complete quickstart guide visit [**Modelstar-Quickstart**](https://modelstar.io/docs/quickstart)
 
 ## Tutorials
 
--   [**Forecast Sales inside Snowflake with 1 Line of SQL**](https://modelstar.io/docs/tutorials/sales-forecasting-inside-snowflake)
+-   [**Forecast Sales inside Snowflake with 1 Line of SQL**](https://modelstar.io/docs/tutorials/sales-forecasting-inside-snowflake)
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 engineers. ## Why we build Modelstar? Modelstar is our attempt to simplify ML
 for analysts. Our design philosophy is: **Data is the most critical component
 in ML, so shipping ML solutions should be as easy as creating data objects.**
 ## Installation To get started with Modelstar, install the Modelstar Python
 package into your local Python environment. ```shell $ pip install modelstar
 ``` It's recommended to install `modelstar` within a Python virtual environment
 using `pyenv`, `virtualenv`, or `poetry`. For a complete quickstart guide visit
-[**Modelstar-Quickstart**](https://modelstar.io/docs/quickstar) ## Tutorials -
+[**Modelstar-Quickstart**](https://modelstar.io/docs/quickstart) ## Tutorials -
 [**Forecast Sales inside Snowflake with 1 Line of SQL**](https://modelstar.io/
 docs/tutorials/sales-forecasting-inside-snowflake)
```

### Comparing `modelstar-0.4.0/pyproject.toml` & `modelstar-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelstar"
-version = "0.4.0"
+version = "0.5.0"
 description = "DevOps for User Defined Functions and Stored Procedures in Data Warehouses"
 authors = ["Adithya Krishnan <krishsandeep@gmail.com>"]
 keywords = ["snowflake", "forecast", "UDF", "Stored Procedure"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://modelstar.io"
 repository = "https://github.com/modelstar-labs"
```

### Comparing `modelstar-0.4.0/src/modelstar/builtins/packages/pycaret.zip` & `modelstar-0.5.0/src/modelstar/builtins/packages/pycaret.zip`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/builtins/procedures/binary_classifier.py` & `modelstar-0.5.0/src/modelstar/builtins/procedures/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/builtins/procedures/univariate_time_series_forecast.py` & `modelstar-0.5.0/src/modelstar/builtins/procedures/univariate_time_series_forecast.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/cli.py` & `modelstar-0.5.0/src/modelstar/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import os
 import click
 from modelstar.version import __version__
 from modelstar import logger, session_registry
 from modelstar.commands.project import initialize_project
 from modelstar.commands.database import list_databases
 from modelstar.commands.register import register_function_from_file, register_procedure_from_file
-from modelstar.commands.upload import upload_file
+from modelstar.commands.upload import upload_file, upload_folder
 from modelstar.commands.create import create_table
 from modelstar.commands.run import run_sql
 from modelstar.commands.download import view_download_records, build_new_report
 from modelstar.executors.config import set_session, load_config
 from modelstar.executors.project import check_project_folder_structure
-from modelstar.utils.path import strip_file_namespace_pointer, check_file_path, map_ml_builtins
+from modelstar.utils.path import strip_file_namespace_pointer, check_file_path, map_ml_builtins, check_folder_path
 from modelstar.utils.logging import cli_blue, cli_magenta, cli_green
 
 
 @click.group()
 @click.version_option(__version__, message=f'\n  {click.style("Modelstar", fg="magenta")}, installed version: {click.style("%(version)s", fg="magenta")}\n')
 @click.option('--database', default=None, help='Target database. Optional: if None, modelstar uses the one set in the project config or prompts one to be created.')
 @click.option('--schema', default=None, help='Target schema. Optional: if None, modelstar uses the one set in the project config or prompts one to be created.')
@@ -72,62 +73,37 @@
 
     response = list_databases(config)
 
     logger.echo('Showing available databases for config', detail=config.name)
     logger.echo(response)
     logger.echo(' ')
 
+
 @main.command("show")
 @click.pass_context
 def show(ctx):
     '''
     modelstar use <target_config>
         Checks if the config.modelstar parameters are right
         Connects to the server of snowflake and gets all the database info 
     '''
 
     session_registry.load_registry()
     check_project_folder_structure()
     config = load_config()
-    
+
     logger.echo('Loaded session', detail=config.name)
 
     response = list_databases(config)
 
     logger.echo('Showing available databases for config', detail=config.name)
     logger.echo(response)
     logger.echo(' ')
 
 
-@main.command("upload")
-@click.argument("file_path", required=True)
-@click.pass_context
-def upload(ctx, file_path):
-    '''
-    modelstar upload <file_path>
-        Uploads the file from <file_path> into the cloud location.
-    '''
-
-    logger.echo('Checking file', detail=file_path)
-
-    abs_file_path = check_file_path(file_path)
-
-    logger.echo('Uploading file', detail=abs_file_path)
-
-    check_project_folder_structure()
-    config = load_config()
-
-    response = upload_file(config, file_path)
-
-    logger.echo(response)
-
-    logger.echo('File available at',
-                detail=f'{config.database}.{config.schema}.@{config.stage}')
-
-
 @main.command("register")
 # TODO: Only accept register_type: function, procedure
 @click.argument("register_pointer", required=True)
 @click.argument("file_function_pointer", required=False)
 @click.pass_context
 def register(ctx, register_pointer, file_function_pointer):
     '''
@@ -255,7 +231,48 @@
     logger.echo('Loaded session', detail=config.name)
 
     # build_new_report(run_id)
 
     view_download_records(config=config, run_id=run_id)
     session_registry.dump_registry()
     logger.echo(' ')
+
+
+@main.command("upload")
+@click.argument("local_path", required=True)
+@click.argument("stage_path", required=False)
+@click.pass_context
+def upload(ctx, local_path: str, stage_path: str = None):
+    '''
+    modelstar upload <local_path> <remote_path>        
+    '''
+    if os.path.isfile(local_path):
+        logger.echo('Checking file', detail=local_path)
+        abs_file_path = check_file_path(local_path)
+        logger.echo('Uploading file', detail=abs_file_path)
+
+        check_project_folder_structure()
+        config = load_config()
+
+        response = upload_file(config, local_path)
+
+        logger.echo(response)
+        logger.echo('File available at',
+                    detail=f'{config.database}.{config.schema}.@{config.stage}/{stage_path}')
+    elif os.path.isdir(local_path):
+        logger.echo('Checking folder: ', detail=local_path)
+
+        abs_folder_path = check_folder_path(local_path)
+
+        logger.echo('Uploading folder: ', detail=abs_folder_path)
+
+        check_project_folder_structure()
+        config = load_config()
+
+        response = upload_folder(config, abs_folder_path, stage_path)
+
+        logger.echo(response)
+
+        logger.echo('Folder available at',
+                    detail=f'{config.database}.{config.schema}.@{config.stage}/{stage_path}')
+    else:
+        raise ValueError(f'`{local_path}` is not a valid file or folder path.')
```

### Comparing `modelstar-0.4.0/src/modelstar/commands/create.py` & `modelstar-0.5.0/src/modelstar/commands/create.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/commands/download.py` & `modelstar-0.5.0/src/modelstar/commands/download.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/commands/project.py` & `modelstar-0.5.0/src/modelstar/commands/project.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/commands/register.py` & `modelstar-0.5.0/src/modelstar/commands/register.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/connectors/snowflake/context.py` & `modelstar-0.5.0/src/modelstar/connectors/snowflake/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,24 @@
         if stage_path is not None:
             file_stage_path = f'@{self.config.stage}/{stage_path}/{file_name}'
         else:
             file_stage_path = f'@{self.config.stage}/{file_name}'
 
         return SnowflakeResponse(table=response_table, info={'file_stage_path': file_stage_path})
 
+    def put_folder(self, folder_path: str, stage_path: str = None) -> SnowflakeResponse:
+        sql_statements_0 = SnowSQL.session_use(self.config)
+        sql_statements_1 = SnowSQL.put_folder_from_local(
+            self.config, folder_path, stage_path)
+        sql_statements = sql_statements_0 + sql_statements_1
+
+        response_table = self.execute_with_context(sql_statements, fetch=5)
+
+        return SnowflakeResponse(table=response_table, info={'folder_stage_path': f'@{self.config.stage}'})
+
     def create_table_from_csv(self, file_path: str, table_info: TableInfo, file_format: FileFormat) -> SnowflakeResponse:
         '''
         Operations performed:
         1. Uploads the file from local to stage using: PUT
         2. Creates the table with the column types using: CREATE TABLE
         3. Creates the file format for copying the data from file to table using: CREATE FILE_FORMAT
         4. Copys the data from stage file into table using: COPY INTO
```

### Comparing `modelstar-0.4.0/src/modelstar/connectors/snowflake/context_types.py` & `modelstar-0.5.0/src/modelstar/connectors/snowflake/context_types.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/connectors/snowflake/modelstar/__init__.py` & `modelstar-0.5.0/src/modelstar/connectors/snowflake/modelstar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     
     prediction_table = pcc.predict_model(_model[0], data=data)
     prediction_value = prediction_table[['prediction_label']].iat[0, 0]
 
     if type(prediction_value) == str:
         return_value = str(prediction_value)
     else:
-        return_value = prediction_value
+        return_value = prediction_value.item()
 
     return return_value
 $$;
 """
     
     sql_ =  SNOWFLAKE_SESSION_STATE.session.sql(sql_statement)
     sql_.collect()
```

### Comparing `modelstar-0.4.0/src/modelstar/connectors/snowflake/sql_dialect/__init__.py` & `modelstar-0.5.0/src/modelstar/connectors/snowflake/sql_dialect/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from modelstar.executors.table import TableInfo
 from modelstar.connectors.snowflake.context_types import SnowflakeConfig, FileFormat
 from modelstar.connectors.snowflake.sql_dialect.register_sproc import register_procedure_from_file
 from modelstar.connectors.snowflake.sql_dialect.register_udf import register_udf_from_file
 
 
 def session_use(config: SnowflakeConfig):
@@ -17,18 +18,38 @@
 
 def put_file_from_local(config: SnowflakeConfig, file_path: str, stage_path: str = None):
 
     # TODO add threads to this to make this faster.
     sql_statements = []
     if stage_path is not None:
         sql_statements.append(
-            f'PUT file://{file_path} @{config.stage}/{stage_path} OVERWRITE = TRUE')
+            f'PUT file://{file_path} @{config.stage}/{stage_path} OVERWRITE = TRUE auto_compress=false;')
     else:
         sql_statements.append(
-            f'PUT file://{file_path} @{config.stage} OVERWRITE = TRUE')
+            f'PUT file://{file_path} @{config.stage} OVERWRITE = TRUE auto_compress=false;')
+
+    return sql_statements
+
+
+def put_folder_from_local(config: SnowflakeConfig, folder_path: str, stage_path: str = None):
+
+    # TODO add threads to this to make this faster.
+    sql_statements = []
+    for root, directories, contents in os.walk(folder_path, topdown=False):
+        for name in contents:
+            local_file_path = os.path.join(root, name)
+            file_dir_path = os.path.dirname(
+                os.path.relpath(local_file_path, start=folder_path))
+
+            if stage_path is not None:
+                _stmt = f'PUT file://{local_file_path} @{config.stage}/{stage_path}/{file_dir_path} OVERWRITE = TRUE auto_compress=false;'
+            else:
+                _stmt = f'PUT file://{local_file_path} @{config.stage}/{file_dir_path} OVERWRITE = TRUE auto_compress=false;'
+
+            sql_statements.append(_stmt)
 
     return sql_statements
 
 
 def get_file_from_stage(config: SnowflakeConfig, local_path: str, stage_path: str = None, name_pattern: str = None):
 
     # TODO add threads to this to make this faster.
```

### Comparing `modelstar-0.4.0/src/modelstar/connectors/snowflake/sql_dialect/register_sproc.py` & `modelstar-0.5.0/src/modelstar/connectors/snowflake/sql_dialect/register_sproc.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/connectors/snowflake/sql_dialect/register_udf.py` & `modelstar-0.5.0/src/modelstar/connectors/snowflake/sql_dialect/register_udf.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/config.py` & `modelstar-0.5.0/src/modelstar/executors/config.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/project.py` & `modelstar-0.5.0/src/modelstar/executors/project.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/py_parser/__init__.py` & `modelstar-0.5.0/src/modelstar/executors/py_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/py_parser/implib_snowflake.py` & `modelstar-0.5.0/src/modelstar/executors/py_parser/implib_snowflake.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/py_parser/implib_stdlib.py` & `modelstar-0.5.0/src/modelstar/executors/py_parser/implib_stdlib.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/py_parser/module_call.py` & `modelstar-0.5.0/src/modelstar/executors/py_parser/module_call.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/py_parser/module_function.py` & `modelstar-0.5.0/src/modelstar/executors/py_parser/module_function.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/py_parser/module_import.py` & `modelstar-0.5.0/src/modelstar/executors/py_parser/module_import.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/py_parser/node_visitor.py` & `modelstar-0.5.0/src/modelstar/executors/py_parser/node_visitor.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/py_parser/parse_exceptions.py` & `modelstar-0.5.0/src/modelstar/executors/py_parser/parse_exceptions.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/report.py` & `modelstar-0.5.0/src/modelstar/executors/report.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/executors/table.py` & `modelstar-0.5.0/src/modelstar/executors/table.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/report/base.html` & `modelstar-0.5.0/src/modelstar/templates/report/base.html`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/report/includes/custom.styles.css` & `modelstar-0.5.0/src/modelstar/templates/report/includes/custom.styles.css`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/report/includes/main.styles.css` & `modelstar-0.5.0/src/modelstar/templates/report/includes/main.styles.css`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/report/includes/normalize.styles.css` & `modelstar-0.5.0/src/modelstar/templates/report/includes/normalize.styles.css`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/report/includes/simple-grid.css` & `modelstar-0.5.0/src/modelstar/templates/report/includes/simple-grid.css`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/report/includes/simple-grid.min.css` & `modelstar-0.5.0/src/modelstar/templates/report/includes/simple-grid.min.css`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/report/includes/skeleton.css` & `modelstar-0.5.0/src/modelstar/templates/report/includes/skeleton.css`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/report/report.html` & `modelstar-0.5.0/src/modelstar/templates/report/report.html`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/snowflake_project/.gitignore` & `modelstar-0.5.0/src/modelstar/templates/snowflake_project/.gitignore`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/snowflake_project/README.md` & `modelstar-0.5.0/src/modelstar/templates/snowflake_project/README.md`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/snowflake_project/sample_data/customer_data.csv` & `modelstar-0.5.0/src/modelstar/templates/snowflake_project/sample_data/customer_data.csv`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/snowflake_project/sample_data/sales.csv` & `modelstar-0.5.0/src/modelstar/templates/snowflake_project/sample_data/sales.csv`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/starter_kit/.gitignore` & `modelstar-0.5.0/src/modelstar/templates/starter_kit/.gitignore`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/starter_kit/README.md` & `modelstar-0.5.0/src/modelstar/templates/starter_kit/README.md`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/functions/country-capitals.csv` & `modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/functions/country-capitals.csv`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/functions/find_capital.py` & `modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/functions/find_capital.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/machine_learning/sales.csv` & `modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/machine_learning/sales.csv`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/machine_learning/univariate_time_series_forecast.py` & `modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/machine_learning/univariate_time_series_forecast.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/stored_procedure/ad_sales.csv` & `modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/stored_procedure/ad_sales.csv`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/stored_procedure/inference.py` & `modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/stored_procedure/inference.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/templates/starter_kit/samples/stored_procedure/training.py` & `modelstar-0.5.0/src/modelstar/templates/starter_kit/samples/stored_procedure/training.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/utils/logging.py` & `modelstar-0.5.0/src/modelstar/utils/logging.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/utils/path.py` & `modelstar-0.5.0/src/modelstar/utils/path.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,14 +32,28 @@
     file_name = os.path.basename(abs_file_path)
 
     file_folder_path = os.path.dirname(abs_file_path)
 
     return abs_file_path, file_folder_path, file_name, namespace_pointer
 
 
+def check_folder_path(folder_path: str) -> str:
+    folder_path = folder_path.strip()
+    abs_folder_path = os.path.abspath(folder_path)
+
+    if not os.path.exists(abs_folder_path):
+        raise ValueError(
+            f"Unable to locate {folder_path} or it does not exist. Tip: provide an absolute path.")
+
+    if not os.path.isdir(abs_folder_path):
+        raise ValueError(f'`{folder_path}` is not a valid folder.')
+
+    return abs_folder_path
+
+
 def check_file_path(file_path: str) -> str:
     file_path = file_path.strip()
     abs_file_path = os.path.abspath(file_path)
 
     if not os.path.exists(abs_file_path):
         raise FileNotFoundError(
             f"Unable to locate {file_path} or it does not exist. Tip: provide an absolute path.")
@@ -67,20 +81,28 @@
                 raise ValueError(f'Existing File/Folder Conflict: {ff_path}')
 
 
 def map_ml_builtins(builtin_pointer: str):
     procedures_path = os.path.join(BUILTINS_PATH, 'procedures')
     builtin_pointer_map = {
         'forecast:univariate_time_series_forecast': {
-            'file_path': os.path.join(BUILTINS_PATH, 'procedures/univariate_time_series_forecast.py'),
+            'file_path': os.path.join(BUILTINS_PATH, 'procedures', 'univariate_time_series_forecast.py'),
             'function_name': 'univariate_time_series_forecast',
             'register_type': 'procedure'},
         'classifier:binary_classifier': {
-            'file_path': os.path.join(BUILTINS_PATH, 'procedures/binary_classifier.py'),
+            'file_path': os.path.join(BUILTINS_PATH, 'procedures', 'binary_classifier.py'),
             'function_name': 'train_binary_classifier',
+            'register_type': 'procedure'},
+        'ml:classifier': {
+            'file_path': os.path.join(BUILTINS_PATH, 'procedures', 'classifier.py'),
+            'function_name': 'train_classifier',
+            'register_type': 'procedure'},
+        'ml:regressor': {
+            'file_path': os.path.join(BUILTINS_PATH, 'procedures', 'regressor.py'),
+            'function_name': 'train_regressor',
             'register_type': 'procedure'}
     }
 
     if builtin_pointer in builtin_pointer_map:
         builtin_info = builtin_pointer_map[builtin_pointer]
         file_path = builtin_info['file_path']
         function_name = builtin_info['function_name']
```

### Comparing `modelstar-0.4.0/src/modelstar/utils/response.py` & `modelstar-0.5.0/src/modelstar/utils/response.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/src/modelstar/utils/zip.py` & `modelstar-0.5.0/src/modelstar/utils/zip.py`

 * *Files identical despite different names*

### Comparing `modelstar-0.4.0/PKG-INFO` & `modelstar-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelstar
-Version: 0.4.0
+Version: 0.5.0
 Summary: DevOps for User Defined Functions and Stored Procedures in Data Warehouses
 Home-page: https://modelstar.io
 License: Apache-2.0
 Keywords: snowflake,forecast,UDF,Stored Procedure
 Author: Adithya Krishnan
 Author-email: krishsandeep@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -50,12 +50,13 @@
 
 ```shell
 $ pip install modelstar
 ```
 
 It's recommended to install `modelstar` within a Python virtual environment using `pyenv`, `virtualenv`, or `poetry`.
 
-For a complete quickstart guide visit [**Modelstar-Quickstart**](https://modelstar.io/docs/quickstar)
+For a complete quickstart guide visit [**Modelstar-Quickstart**](https://modelstar.io/docs/quickstart)
 
 ## Tutorials
 
 -   [**Forecast Sales inside Snowflake with 1 Line of SQL**](https://modelstar.io/docs/tutorials/sales-forecasting-inside-snowflake)
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelstar Version: 0.4.0 Summary: DevOps for User
+Metadata-Version: 2.1 Name: modelstar Version: 0.5.0 Summary: DevOps for User
 Defined Functions and Stored Procedures in Data Warehouses Home-page: https://
 modelstar.io License: Apache-2.0 Keywords: snowflake,forecast,UDF,Stored
 Procedure Author: Adithya Krishnan Author-email: krishsandeep@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -21,10 +21,10 @@
 engineers. ## Why we build Modelstar? Modelstar is our attempt to simplify ML
 for analysts. Our design philosophy is: **Data is the most critical component
 in ML, so shipping ML solutions should be as easy as creating data objects.**
 ## Installation To get started with Modelstar, install the Modelstar Python
 package into your local Python environment. ```shell $ pip install modelstar
 ``` It's recommended to install `modelstar` within a Python virtual environment
 using `pyenv`, `virtualenv`, or `poetry`. For a complete quickstart guide visit
-[**Modelstar-Quickstart**](https://modelstar.io/docs/quickstar) ## Tutorials -
+[**Modelstar-Quickstart**](https://modelstar.io/docs/quickstart) ## Tutorials -
 [**Forecast Sales inside Snowflake with 1 Line of SQL**](https://modelstar.io/
 docs/tutorials/sales-forecasting-inside-snowflake)
```

