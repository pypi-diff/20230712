# Comparing `tmp/bigeye_sdk-0.4.55.tar.gz` & `tmp/bigeye_sdk-0.4.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.55.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.56.tar", max compression
```

## Comparing `bigeye_sdk-0.4.55.tar` & `bigeye_sdk-0.4.56.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     2092 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/LICENSE
--rw-r--r--   0        0        0      873 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/README.md
--rw-r--r--   0        0        0     3727 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       82 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    17489 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0     1182 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0    10264 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      701 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9206 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3042 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    39917 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    38282 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0      390 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    33079 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     1018 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     3343 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0     4517 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2544 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      117 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0    20235 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     2540 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1227 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1676 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5088 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4031 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1701 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/com/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/com/bigeye/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/com/bigeye/models/__init__.py
--rw-r--r--   0        0        0   220193 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/com/bigeye/models/generated.py
--rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/google/__init__.py
--rw-r--r--   0        0        0    14816 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/google/api.py
--rw-r--r--   0        0        0      507 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      489 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    22303 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0     3948 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     3504 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0     9456 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0     8396 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      220 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    50205 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0      865 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7114 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3685 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/pyproject.toml
--rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.55/PKG-INFO
+-rw-r--r--   0        0        0     2092 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/LICENSE
+-rw-r--r--   0        0        0      873 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/README.md
+-rw-r--r--   0        0        0     3727 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    17489 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0     1182 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    10276 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      701 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9206 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3042 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    38926 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    38282 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    33079 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     1018 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     3343 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0     4517 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2544 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      117 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0    20235 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     2540 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1227 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1676 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5088 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4031 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   227101 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      507 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    27454 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0     3948 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     3504 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0     9456 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0     8396 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      220 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    50437 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0      865 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7346 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3685 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/pyproject.toml
+-rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.56/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.55/LICENSE` & `bigeye_sdk-0.4.56/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/README.md` & `bigeye_sdk-0.4.56/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.56/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.56/bigeye_sdk/authentication/api_authentication.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/authentication/credentials.py` & `bigeye_sdk-0.4.56/bigeye_sdk/authentication/credentials.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.56/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     report_files = []
     errors_reported = False
 
     source_reports = []
 
     for report in REPORTS:
         file_name = f'{output_path}/{report.source_name.replace(" ", "_")}_{report.process_stage}.yml'
-        report.save(file_name)
+        report.save(output_path=file_name)
         report_files.append(file_name)
         errors_reported = errors_reported or report.has_errors()
         source_reports.append(report.get_console_report())
 
     if errors_reported and strict_mode:
         raise BigConfigValidationException(
             FAILED_API_EXECUTION_MSG.format(
```

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.56/bigeye_sdk/client/datawatch_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -551,59 +551,39 @@
         else:
             url = f"{mc_url}/dry-run"
 
         return MetricSuiteResponse().from_dict(
             self._call_datawatch(Method.POST, url=url, body=metric_suite.to_json())
         )
 
-    def __get_metric_suite_response_for_queue(self, metric_suite: MetricSuite, mc_url: str) -> MetricSuiteResponse:
-
-        suite_response: MetricSuiteResponse = MetricSuiteResponse()
-        # TODO: Update once backend returns expected response from queue
-        """Silently plan to obtain the MetricSuiteResponse, in order to generate reports for users."""
-        if isinstance(self, BasicAuthDatawatchClient):
-            suite_response.from_dict(requests.post(
-                f"{self.get_base_url()}{mc_url}/dry-run",
-                headers={"Content-Type": "application/json", "Accept": "application/json"},
-                data=metric_suite.to_json(),
-                auth=self._auth
-            ).json())
-        elif isinstance(self, BrowserAuthDatawatchClient):
-            suite_response.from_dict(requests.post(
-                f"{self.get_base_url()}{mc_url}/dry-run",
-                headers={"Content-Type": "application/json", "Accept": "application/json"},
-                data=metric_suite.to_json(),
-                cookies=self._cookies
-            ).json())
-
-        return suite_response
-
-    def post_metric_suite_queue(self, metric_suite: MetricSuite) -> MetricSuiteResponse:
-        mc_url = "/api/v1/metric-suites"
-
-        suite_response = self.__get_metric_suite_response_for_queue(metric_suite=metric_suite, mc_url=mc_url)
+    def post_metric_suite_queue(self, metric_suite: MetricSuite, apply: bool = False) -> MetricSuiteResponse:
+        if apply:
+            url = "/api/v1/metric-suites/queue"
+        else:
+            url = f"/api/v1/metric-suites/dry-run/queue"
 
         response: WorkflowStatusResponse = WorkflowStatusResponse().from_dict(
-            self._call_datawatch(Method.POST, url=f"{mc_url}/queue", body=metric_suite.to_json())
+            self._call_datawatch(Method.POST, url=url, body=metric_suite.to_json())
         )
 
-        status_url = f"/api/v1/workflows/{response.workflow_id}/status"
+        status_url = f"/api/v1/metric-suites/status/{response.workflow_id}"
         while response.status == WorkflowProcessingStatus.WORKFLOW_PROCESSING_STATUS_QUEUED or \
                 response.status == WorkflowProcessingStatus.WORKFLOW_PROCESSING_STATUS_IN_PROGRESS:
             log.info(f"Bigconfig in queue...")
             time.sleep(10)
+            status = self._call_datawatch(Method.GET, url=status_url)
             wsr = WorkflowStatusResponse()
-            r: WorkflowStatusResponse = wsr.from_dict(self._call_datawatch(Method.GET, url=status_url))
-            response.status = r.status
+            r: WorkflowStatusResponse = wsr.from_dict(status['workflowStatusResponse'])
+            response.status = WorkflowProcessingStatus(r.status)
         log.info(f"Queuing complete. Workflow finished with status {response.status.name}")
         if response.status != WorkflowProcessingStatus.WORKFLOW_PROCESSING_STATUS_COMPLETED:
             err = f"Bigconfig workflow was not completed. Final status: {response.status.name}"
             raise BigconfigIncompleteException(err)
 
-        return suite_response
+        return MetricSuiteResponse().from_dict(status["metricSuiteResponse"])
 
     def upsert_metric(
             self,
             *,
             id: int = 0,
             schedule_frequency: Optional[TimeInterval] = None,
             filters: List[str] = [],
```

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.56/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.56/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,18 +582,18 @@
         # Applies changes and overwrites once local validations have passed.
         # if apply:
         #     self._upsert_collections(bigconfig=bigconfig, overwrite=True,
         #                              apply=apply)  # Will always overwrite for Bigconfig.
 
         for metric_suite in metric_suites:
             j = metric_suite.to_json()
-            if not apply or no_queue:
+            if no_queue:
                 response = self.client.post_metric_suite(metric_suite=metric_suite, apply=apply)
             else:
-                response = self.client.post_metric_suite_queue(metric_suite=metric_suite)
+                response = self.client.post_metric_suite_queue(metric_suite=metric_suite, apply=apply)
             process_stage = ProcessStage.APPLY if apply else ProcessStage.PLAN
             MetricSuiteReport.from_datawatch_object(response,
                                                     source_name=self.sources_by_id_ix[metric_suite.source_id].name,
                                                     process_stage=process_stage)
 
         process_reports(output_path=output_path, strict_mode=strict_mode)
```

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.56/bigeye_sdk/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/metric_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/metric_run_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/table_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.56/bigeye_sdk/functions/urlfuncts.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/generated/com/bigeye/models/generated.py` & `bigeye_sdk-0.4.56/bigeye_sdk/generated/com/bigeye/models/generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,17 @@
     TAGGABLE_ENTITY_TYPE_DELTA = 5
     TAGGABLE_ENTITY_TYPE_COLUMN = 6
     TAGGABLE_ENTITY_TYPE_SLA = 7
     TAGGABLE_ENTITY_TYPE_BI_TOOL = 8
     TAGGABLE_ENTITY_TYPE_TABLEAU_WORKBOOK = 9
     TAGGABLE_ENTITY_TYPE_N_WAY_DELTA = 10
     TAGGABLE_ENTITY_TYPE_VIRTUAL_TABLE = 11
-    TAGGABLE_ENTITY_TYPE_DBT_PROJECT = 12
+    TAGGABLE_ENTITY_TYPE_INTEGRATION = 12
+    TAGGABLE_ENTITY_TYPE_DBT_PROJECT = 13
+    TAGGABLE_ENTITY_TYPE_DBT_JOB = 14
 
 
 class TableType(betterproto.Enum):
     TABLE_TYPE_UNSPECIFIED = 0
     TABLE_TYPE_TABLE = 1
     TABLE_TYPE_VIEW = 2
     TABLE_TYPE_VIRTUAL = 3
@@ -409,14 +411,16 @@
     AGGREGATE_FIELD_METRICS_MUTED = 8
     AGGREGATE_FIELD_METRICS_HEALTHY = 9
     AGGREGATE_FIELD_AUTOMETRICS = 10
     AGGREGATE_FIELD_GROUP_METRIC_STATUS = 11
     AGGREGATE_FIELD_ALERTS = 12
     AGGREGATE_FIELD_ISSUES = 13
     AGGREGATE_FIELD_INTEGRATIONS = 14
+    AGGREGATE_FIELD_BI_TOOLS = 15
+    AGGREGATE_FIELD_ETL_TOOLS = 16
 
 
 class GroupByEntityType(betterproto.Enum):
     GROUP_BY_ENTITY_TYPE_UNSPECIFIED = 0
     GROUP_BY_ENTITY_TYPE_WAREHOUSE = 1
     GROUP_BY_ENTITY_TYPE_SCHEMA = 2
     GROUP_BY_ENTITY_TYPE_TABLE = 3
@@ -584,14 +588,15 @@
     WORKFLOW_PROCESSING_TYPE_GENERATE_AUTOMETRICS = 6
     WORKFLOW_PROCESSING_TYPE_GENERATE_POP_SCORES = 7
     WORKFLOW_PROCESSING_TYPE_CATALOG_INDEX_INTEGRATION = 8
     WORKFLOW_PROCESSING_TYPE_APPLY_BIGCONFIG = 9
     WORKFLOW_PROCESSING_TYPE_RUN_DELTA = 10
     WORKFLOW_PROCESSING_TYPE_RUN_COMPARISON_TABLE = 11
     WORKFLOW_PROCESSING_TYPE_RUN_METRIC_BATCH = 12
+    WORKFLOW_PROCESSING_TYPE_PLAN_BIGCONFIG = 13
 
 
 class CatalogIndexOperationType(betterproto.Enum):
     CATALOG_INDEX_OPERATION_TYPE_UNSPECIFIED = 0
     CATALOG_INDEX_OPERATION_TYPE_ADD = 1
     CATALOG_INDEX_OPERATION_TYPE_UPDATE = 2
     CATALOG_INDEX_OPERATION_TYPE_DELETE = 3
@@ -642,14 +647,21 @@
     DASHBOARD_DATA_POINT_TYPE_TOTAL_TABLES_WITH_METRICS_BY_CATEGORY = 16
     DASHBOARD_DATA_POINT_TYPE_PCT_TABLES_WITH_METRICS_BY_CATEGORY = 17
     DASHBOARD_DATA_POINT_TYPE_TOTAL_TABLES_WITH_ISSUE_BY_CATEGORY = 18
     DASHBOARD_DATA_POINT_TYPE_NUMBER_ISSUES_INTERACTED = 19
     DASHBOARD_DATA_POINT_TYPE_NUMBER_ISSUES_OPENED = 20
     DASHBOARD_DATA_POINT_TYPE_PCT_ISSUES_INTERACTED = 21
     DASHBOARD_DATA_POINT_TYPE_PCT_TABLES_WITHOUT_ISSUE_BY_CATEGORY = 22
+    DASHBOARD_DATA_POINT_TYPE_TOTAL_TABLES_WITHOUT_ISSUE_BY_CATEGORY = 23
+
+
+class DashboardDateAggregationType(betterproto.Enum):
+    DASHBOARD_DATE_AGGREGATION_TYPE_DAY = 0
+    DASHBOARD_DATE_AGGREGATION_TYPE_WEEK = 1
+    DASHBOARD_DATE_AGGREGATION_TYPE_MONTH = 2
 
 
 class GroupUserOperation(betterproto.Enum):
     GROUP_USER_OPERATION_UNSPECIFIED = 0
     GROUP_USER_OPERATION_ADD = 1
     GROUP_USER_OPERATION_REMOVE = 2
 
@@ -729,26 +741,14 @@
 class UserInviteRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
     email: str = betterproto.string_field(2)
     group_ids: List[int] = betterproto.int32_field(3)
 
 
 @dataclass
-class CompanyInfo(betterproto.Message):
-    needs_admin: bool = betterproto.bool_field(1)
-
-
-@dataclass
-class SaasCustomer(betterproto.Message):
-    owner_email: str = betterproto.string_field(1)
-    company_name: str = betterproto.string_field(2)
-    company_uuid: str = betterproto.string_field(3)
-
-
-@dataclass
 class SimpleBound(betterproto.Message):
     bound_type: "SimpleBoundType" = betterproto.enum_field(1)
     # Value of the threshold. For AutoThreshold types this is ignored.
     value: float = betterproto.double_field(2)
 
 
 @dataclass
@@ -1032,14 +1032,17 @@
 class SinglePathParamColumnIdRequest(betterproto.Message):
     column_id: int = betterproto.int32_field(1)
 
 
 @dataclass
 class SchemaSearchRequest(betterproto.Message):
     warehouse_id: List[int] = betterproto.int32_field(1)
+    schema_name: List[str] = betterproto.string_field(2)
+    schema_id: List[int] = betterproto.int32_field(3)
+    workspace_id: int = betterproto.int32_field(4)
 
 
 @dataclass
 class TableAndColumnIdRequest(betterproto.Message):
     table_id: int = betterproto.int32_field(1)
     column_id: int = betterproto.int32_field(2)
 
@@ -1049,14 +1052,15 @@
     warehouse_id: List[int] = betterproto.int32_field(1)
     schema: List[str] = betterproto.string_field(2)
     table_name: List[str] = betterproto.string_field(3)
     ids: List[int] = betterproto.int32_field(4)
     schema_id: List[int] = betterproto.int32_field(5)
     include_favorites: bool = betterproto.bool_field(6)
     ignore_fields: bool = betterproto.bool_field(7)
+    workspace_id: int = betterproto.int32_field(8)
 
 
 @dataclass
 class MetricHistoryDataPoint(betterproto.Message):
     epoch_seconds: int = betterproto.int32_field(1)
     value: float = betterproto.double_field(2)
     lower_threshold: float = betterproto.double_field(3)
@@ -1350,14 +1354,15 @@
     metrics: List["MetricWithRuns"] = betterproto.message_field(1)
 
 
 @dataclass
 class MetricSuiteRequest(betterproto.Message):
     metric_suite: "MetricSuite" = betterproto.message_field(1)
     workflow_info: "WorkflowInfo" = betterproto.message_field(2)
+    is_apply: bool = betterproto.bool_field(3)
 
 
 @dataclass
 class MetricSuite(betterproto.Message):
     source_id: int = betterproto.int32_field(1)
     definitions: List["CohortAndMetricDefinition"] = betterproto.message_field(2)
     row_creation_cohorts: List["CohortDefinition"] = betterproto.message_field(3)
@@ -1548,14 +1553,15 @@
 
 @dataclass
 class CreateDataNodeRequest(betterproto.Message):
     node_type: "DataNodeType" = betterproto.enum_field(1)
     node_entity_id: int = betterproto.int32_field(2)
     node_name: str = betterproto.string_field(3)
     node_container_name: str = betterproto.string_field(4)
+    workspace_id: int = betterproto.int32_field(5)
 
 
 @dataclass
 class SinglePathParamDataNodeIdRequest(betterproto.Message):
     data_node_id: int = betterproto.int32_field(1)
 
 
@@ -1625,14 +1631,15 @@
     api_port: int = betterproto.int32_field(4)
     web_base_uri: str = betterproto.string_field(5)
     web_port: int = betterproto.int32_field(6)
     namespace: str = betterproto.string_field(7)
     credentials_public: str = betterproto.string_field(8)
     credentials_private: str = betterproto.string_field(9)
     timeout: int = betterproto.int32_field(10)
+    workspace_id: int = betterproto.int32_field(11)
 
 
 @dataclass
 class IntegrationsResponse(betterproto.Message):
     integrations: List["Integration"] = betterproto.message_field(1)
 
 
@@ -1640,14 +1647,25 @@
 class GetIntegrationEntitiesResponse(betterproto.Message):
     integration_partner: "IntegrationPartner" = betterproto.enum_field(1)
     tableau_workbooks: List["TableauWorkbook"] = betterproto.message_field(2)
     dbt_projects: List["DbtProject"] = betterproto.message_field(3)
 
 
 @dataclass
+class UpsertDbtProject(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    account_id: int = betterproto.int32_field(2)
+    name: str = betterproto.string_field(3)
+    integration_entity_id: str = betterproto.string_field(4)
+    integration_id: int = betterproto.int32_field(5)
+    company_id: int = betterproto.int32_field(6)
+    workspace_id: int = betterproto.int32_field(7)
+
+
+@dataclass
 class DbtProject(betterproto.Message):
     id: int = betterproto.int32_field(1)
     account_id: int = betterproto.int32_field(2)
     name: str = betterproto.string_field(3)
     job_count: int = betterproto.int32_field(4)
     is_favorite: bool = betterproto.bool_field(5)
     company_id: int = betterproto.int32_field(6)
@@ -1661,14 +1679,15 @@
 @dataclass
 class GetDbtProjectsRequest(betterproto.Message):
     integration_id: int = betterproto.int32_field(1)
     page_size: int = betterproto.int32_field(2)
     page_cursor: str = betterproto.string_field(3)
     sort_options: List["DbtProjectSortOption"] = betterproto.message_field(4)
     search: str = betterproto.string_field(5)
+    workspace_id: int = betterproto.int32_field(6)
 
 
 @dataclass
 class DbtProjectSortOption(betterproto.Message):
     sort_direction: "SortDirection" = betterproto.enum_field(1)
     sort_field: "DbtProjectSortField" = betterproto.enum_field(2)
 
@@ -1981,14 +2000,15 @@
     schema_name: str = betterproto.string_field(11)
     column_ids: List[int] = betterproto.int32_field(12)
     search: str = betterproto.string_field(13)
     sort_direction: "SortDirection" = betterproto.enum_field(14)
     schema_id: int = betterproto.int32_field(15)
     metric_types: List["PredefinedMetricName"] = betterproto.enum_field(16)
     include_latest_metric_runs: bool = betterproto.bool_field(17)
+    workspace_id: int = betterproto.int32_field(18)
 
 
 @dataclass
 class SearchMetricConfigurationRequest(betterproto.Message):
     ids: List[int] = betterproto.int32_field(1)
     # If searching by table name, at least one warehouse ID must be present
     warehouse_ids: List[int] = betterproto.int32_field(2)
@@ -2294,14 +2314,15 @@
     comparison_table_ids: List[int] = betterproto.int32_field(1)
     exclude_comparison_metrics: bool = betterproto.bool_field(2)
     page_size: int = betterproto.int32_field(3)
     page_cursor: str = betterproto.string_field(4)
     sort_field: "ComparisonTableSortField" = betterproto.enum_field(5)
     sort_direction: "SortDirection" = betterproto.enum_field(6)
     search: str = betterproto.string_field(7)
+    workspace_id: int = betterproto.int32_field(8)
 
 
 @dataclass
 class GetComparisonTableInfosResponse(betterproto.Message):
     comparison_table_infos: List["ComparisonTableInfo"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -2368,14 +2389,15 @@
     start_issue_closed_epoch_seconds: int = betterproto.int64_field(10, group="filter")
     end_issue_closed_epoch_seconds: int = betterproto.int64_field(11, group="filter")
     issue_priority: "IssuePriority" = betterproto.enum_field(12, group="filter")
     metric_status: "MetricStatus" = betterproto.enum_field(13, group="filter")
     collection_id: int = betterproto.int32_field(14, group="filter")
     metric_type: "MetricType" = betterproto.message_field(15, group="filter")
     metric_category: "MetricCategory" = betterproto.enum_field(16, group="filter")
+    workspace_id: int = betterproto.int32_field(17, group="filter")
 
 
 @dataclass
 class CountsQuery(betterproto.Message):
     fields: List["AggregateField"] = betterproto.enum_field(1)
     filters: List["SearchFilter"] = betterproto.message_field(2)
     group_by_entity_type: "GroupByEntityType" = betterproto.enum_field(3)
@@ -2422,14 +2444,15 @@
     search_all: bool = betterproto.bool_field(3)
     source_ids: List[int] = betterproto.int32_field(4)
     schema_ids: List[int] = betterproto.int32_field(5)
     table_ids: List[int] = betterproto.int32_field(6)
     column_ids: List[int] = betterproto.int32_field(7)
     statuses: List[str] = betterproto.string_field(8)
     metric_types: List["PredefinedMetricName"] = betterproto.enum_field(9)
+    workspace_id: int = betterproto.int32_field(10)
 
 
 @dataclass
 class BulkIssueUpdateWhereClause(betterproto.Message):
     ids: List[int] = betterproto.int32_field(1)
     search: str = betterproto.string_field(2)
     search_all: bool = betterproto.bool_field(3)
@@ -2442,14 +2465,15 @@
     metric_ids: List[int] = betterproto.int32_field(10)
     collection_ids: List[int] = betterproto.int32_field(11)
     priority: List["IssuePriority"] = betterproto.enum_field(12)
     metric_status: List["MetricStatus"] = betterproto.enum_field(13)
     metric_type: List["MetricType"] = betterproto.message_field(14)
     min_opened_time: int = betterproto.int64_field(15)
     max_opened_time: int = betterproto.int64_field(16)
+    workspace_id: int = betterproto.int32_field(17)
 
 
 @dataclass
 class BulkMetricOperation(betterproto.Message):
     where: "WhereClause" = betterproto.message_field(1)
     edit_request: "MetricConfiguration" = betterproto.message_field(2)
     mute_request: "MuteRequest" = betterproto.message_field(3)
@@ -2657,14 +2681,15 @@
     related_issue_ids: List[int] = betterproto.int32_field(22)
     priority: List["IssuePriority"] = betterproto.enum_field(23)
     metric_status: List["MetricStatus"] = betterproto.enum_field(24)
     metric_type: List["MetricType"] = betterproto.message_field(25)
     min_opened_time: int = betterproto.int64_field(26)
     max_opened_time: int = betterproto.int64_field(27)
     sort_options: List["IssueSortOption"] = betterproto.message_field(28)
+    workspace_id: int = betterproto.int32_field(29)
 
 
 @dataclass
 class IssueSortOption(betterproto.Message):
     sort_direction: "SortDirection" = betterproto.enum_field(1)
     sort_field: "IssueSortField" = betterproto.enum_field(2)
 
@@ -2890,14 +2915,15 @@
 
 
 @dataclass
 class CreateNamedScheduleRequest(betterproto.Message):
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     cron: str = betterproto.string_field(3)
+    workspace_id: int = betterproto.int32_field(4)
 
 
 @dataclass
 class GetNamedScheduleEntitiesResponse(betterproto.Message):
     table_comparisons: List["IdAndDisplayName"] = betterproto.message_field(1)
     metrics: List["IdAndDisplayName"] = betterproto.message_field(2)
 
@@ -2957,14 +2983,15 @@
 @dataclass
 class GetMetricTemplateListRequest(betterproto.Message):
     page_size: int = betterproto.int32_field(1)
     page_cursor: str = betterproto.string_field(2)
     sort_field: "MetricTemplateSortField" = betterproto.enum_field(3)
     sort_direction: "SortDirection" = betterproto.enum_field(4)
     search: str = betterproto.string_field(5)
+    workspace_id: int = betterproto.int32_field(6)
 
 
 @dataclass
 class GetMetricTemplateListResponse(betterproto.Message):
     metric_templates: List["MetricTemplate"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -3059,14 +3086,15 @@
     query_timeout_seconds: int = betterproto.int32_field(11)
     skip_indexing: bool = betterproto.bool_field(12)
     alation_source_id: int = betterproto.int32_field(13)
     atlan_connection_id: str = betterproto.string_field(14)
     temporal_agent_secret: str = betterproto.string_field(15)
     target_bigquery_project_id: str = betterproto.string_field(16)
     bigquery_query_project_ids: str = betterproto.string_field(17)
+    workspace_id: int = betterproto.int32_field(18)
 
 
 @dataclass
 class MetadataSchemaRequest(betterproto.Message):
     source_id: int = betterproto.int32_field(1)
     schema_name: List[str] = betterproto.string_field(2)
 
@@ -3096,14 +3124,15 @@
 @dataclass
 class GetSourceListRequest(betterproto.Message):
     page_size: int = betterproto.int32_field(1)
     page_cursor: str = betterproto.string_field(2)
     sort_field: "SourceSortField" = betterproto.enum_field(3)
     sort_direction: "SortDirection" = betterproto.enum_field(4)
     search: str = betterproto.string_field(5)
+    workspace_id: int = betterproto.int32_field(6)
 
 
 @dataclass
 class GetSourceListResponse(betterproto.Message):
     sources: List["Source"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -3127,14 +3156,15 @@
 class GetSchemaListRequest(betterproto.Message):
     source_ids: List[int] = betterproto.int32_field(1)
     page_size: int = betterproto.int32_field(2)
     page_cursor: str = betterproto.string_field(3)
     sort_field: "SchemaSortField" = betterproto.enum_field(4)
     sort_direction: "SortDirection" = betterproto.enum_field(5)
     search: str = betterproto.string_field(6)
+    workspace_id: int = betterproto.int32_field(7)
 
 
 @dataclass
 class GetSchemaListResponse(betterproto.Message):
     schemas: List["Schema"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -3146,14 +3176,15 @@
     table_ids: List[int] = betterproto.int32_field(3)
     page_size: int = betterproto.int32_field(4)
     page_cursor: str = betterproto.string_field(5)
     sort_field: "TableSortField" = betterproto.enum_field(6)
     sort_direction: "SortDirection" = betterproto.enum_field(7)
     search: str = betterproto.string_field(8)
     ignore_fields: bool = betterproto.bool_field(9)
+    workspace_id: int = betterproto.int32_field(10)
 
 
 @dataclass
 class GetTableListResponse(betterproto.Message):
     tables: List["Table"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -3165,14 +3196,15 @@
     table_ids: List[int] = betterproto.int32_field(3)
     column_ids: List[int] = betterproto.int32_field(4)
     page_size: int = betterproto.int32_field(5)
     page_cursor: str = betterproto.string_field(6)
     sort_field: "ColumnSortField" = betterproto.enum_field(7)
     sort_direction: "SortDirection" = betterproto.enum_field(8)
     search: str = betterproto.string_field(9)
+    workspace_id: int = betterproto.int32_field(10)
 
 
 @dataclass
 class ColumnWithTable(betterproto.Message):
     column: "TableColumn" = betterproto.message_field(1)
     table: "Table" = betterproto.message_field(2)
 
@@ -3180,24 +3212,30 @@
 @dataclass
 class GetColumnListResponse(betterproto.Message):
     columns: List["ColumnWithTable"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
 
 @dataclass
+class GetAllVirtualTablesRequest(betterproto.Message):
+    workspace_id: int = betterproto.int32_field(1)
+
+
+@dataclass
 class GetVirtualTableListRequest(betterproto.Message):
     source_ids: List[int] = betterproto.int32_field(1)
     schema_ids: List[int] = betterproto.int32_field(2)
     table_ids: List[int] = betterproto.int32_field(3)
     page_size: int = betterproto.int32_field(4)
     page_cursor: str = betterproto.string_field(5)
     sort_field: "VirtualTableSortField" = betterproto.enum_field(6)
     sort_direction: "SortDirection" = betterproto.enum_field(7)
     search: str = betterproto.string_field(8)
     ignore_fields: bool = betterproto.bool_field(9)
+    workspace_id: int = betterproto.int32_field(10)
 
 
 @dataclass
 class GetVirtualTableListResponse(betterproto.Message):
     virtual_tables: List["VirtualTable"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -3262,20 +3300,27 @@
     total_ops: int = betterproto.int32_field(2)
     completed_ops: int = betterproto.int32_field(3)
     status: "WorkflowProcessingStatus" = betterproto.enum_field(4)
     workflow_type: "WorkflowProcessingType" = betterproto.enum_field(5)
 
 
 @dataclass
+class BigconfigWorkflowStatusResponse(betterproto.Message):
+    workflow_status_response: "WorkflowStatusResponse" = betterproto.message_field(1)
+    metric_suite_response: "MetricSuiteResponse" = betterproto.message_field(2)
+
+
+@dataclass
 class CatalogIndexRequest(betterproto.Message):
     id: int = betterproto.int32_field(1)
     workflow_info: "WorkflowInfo" = betterproto.message_field(2)
     priority: int = betterproto.int32_field(3)
     is_first_indexing: bool = betterproto.bool_field(4)
     indexed_at: int = betterproto.int64_field(5)
+    warehouse_id: int = betterproto.int32_field(6)
 
 
 @dataclass
 class DeltaRunRequest(betterproto.Message):
     id: int = betterproto.int32_field(1)
     workflow_info: "WorkflowInfo" = betterproto.message_field(2)
 
@@ -3293,25 +3338,50 @@
     table: "Table" = betterproto.message_field(2)
     catalog_index_operation_type: "CatalogIndexOperationType" = betterproto.enum_field(
         3
     )
     workflow_process_id: int = betterproto.int64_field(4)
     is_first_indexing: bool = betterproto.bool_field(5)
     indexed_at: int = betterproto.int64_field(6)
+    warehouse_id: int = betterproto.int32_field(7)
 
 
 @dataclass
 class TableauWorkbookIndexRequest(betterproto.Message):
     tableau_workbook_id: int = betterproto.int32_field(1)
     tableau_workbook: "TableauWorkbook" = betterproto.message_field(2)
     integration_partner: "IntegrationPartner" = betterproto.enum_field(3)
     catalog_index_operation_type: "CatalogIndexOperationType" = betterproto.enum_field(
         4
     )
     workflow_process_id: int = betterproto.int64_field(5)
+    integration_id: int = betterproto.int32_field(7)
+
+
+@dataclass
+class DbtProjectIndexRequest(betterproto.Message):
+    dbt_project_id: int = betterproto.int32_field(1)
+    dbt_project: "UpsertDbtProject" = betterproto.message_field(2)
+    integration_partner: "IntegrationPartner" = betterproto.enum_field(3)
+    catalog_index_operation_type: "CatalogIndexOperationType" = betterproto.enum_field(
+        4
+    )
+    workflow_process_id: int = betterproto.int64_field(5)
+    integration_id: int = betterproto.int32_field(6)
+
+
+@dataclass
+class DbtJobIndexRequest(betterproto.Message):
+    dbt_job_id: int = betterproto.int32_field(1)
+    dbt_job: "UpsertDbtJob" = betterproto.message_field(2)
+    catalog_index_operation_type: "CatalogIndexOperationType" = betterproto.enum_field(
+        3
+    )
+    workflow_process_id: int = betterproto.int64_field(4)
+    integration_id: int = betterproto.int32_field(5)
 
 
 @dataclass
 class LineageCriticalEntitiesExportRequest(betterproto.Message):
     filters: List[str] = betterproto.string_field(1)
 
 
@@ -3362,14 +3432,15 @@
     sort_field: "SchemaChangeSortField" = betterproto.enum_field(3)
     sort_direction: "SortDirection" = betterproto.enum_field(4)
     search: str = betterproto.string_field(5)
     source_id: int = betterproto.int32_field(6)
     schema_id: int = betterproto.int32_field(7)
     table_id: int = betterproto.int32_field(8)
     column_id: int = betterproto.int32_field(9)
+    workspace_id: int = betterproto.int32_field(10)
 
 
 @dataclass
 class GetSchemaChangesResponse(betterproto.Message):
     schema_changes: List["SchemaChange"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -3383,14 +3454,19 @@
 class FavoriteItem(betterproto.Message):
     entity_id: int = betterproto.int32_field(1)
     entity_type: "TaggableEntityType" = betterproto.enum_field(2)
     entity_name: str = betterproto.string_field(3)
 
 
 @dataclass
+class GetFavoritesRequest(betterproto.Message):
+    workspace_id: int = betterproto.int32_field(1)
+
+
+@dataclass
 class FavoriteListResponse(betterproto.Message):
     favorites: List["FavoriteItem"] = betterproto.message_field(1)
 
 
 @dataclass
 class FavoriteRequest(betterproto.Message):
     favorite: "FavoriteItem" = betterproto.message_field(1)
@@ -3417,14 +3493,15 @@
 class PublicKeyMessage(betterproto.Message):
     public_key: str = betterproto.string_field(1)
 
 
 @dataclass
 class UpsertDeltaRequest(betterproto.Message):
     delta: "Delta" = betterproto.message_field(1)
+    workspace_id: int = betterproto.int32_field(2)
 
 
 @dataclass
 class UpsertDeltaResponse(betterproto.Message):
     delta: "Delta" = betterproto.message_field(1)
 
 
@@ -3571,28 +3648,44 @@
 class DashboardDataPointsRequest(betterproto.Message):
     company_id: int = betterproto.int32_field(1)
     workspace_ids: List[int] = betterproto.int32_field(2)
     source_ids: List[int] = betterproto.int32_field(3)
     starting_timestamp: int = betterproto.int64_field(4)
     ending_timestamp: int = betterproto.int64_field(5)
     data_point_types: List["DashboardDataPointType"] = betterproto.enum_field(6)
+    aggregation_type: "DashboardDateAggregationType" = betterproto.enum_field(7)
 
 
 @dataclass
 class DashboardDataPointsResponse(betterproto.Message):
     company_id: int = betterproto.int32_field(1)
     workspace_ids: List[int] = betterproto.int32_field(2)
     source_ids: List[int] = betterproto.int32_field(3)
     starting_timestamp: int = betterproto.int64_field(4)
     ending_timestamp: int = betterproto.int64_field(5)
     data_point_types: List["DashboardDataPointType"] = betterproto.enum_field(6)
     data_point_series: List["DashboardDataPointSeries"] = betterproto.message_field(7)
 
 
 @dataclass
+class DashboardRefreshInfoRequest(betterproto.Message):
+    company_id: int = betterproto.int32_field(1)
+    workspace_ids: List[int] = betterproto.int32_field(2)
+    source_ids: List[int] = betterproto.int32_field(3)
+    starting_timestamp: int = betterproto.int64_field(4)
+    ending_timestamp: int = betterproto.int64_field(5)
+
+
+@dataclass
+class DashboardRefreshInfoResponse(betterproto.Message):
+    last_updated_at: int = betterproto.int64_field(1)
+    next_updated_at: int = betterproto.int64_field(2)
+
+
+@dataclass
 class DashboardDataPointSeries(betterproto.Message):
     company_id: int = betterproto.int32_field(1)
     workspace_ids: List[int] = betterproto.int32_field(2)
     source_ids: List[int] = betterproto.int32_field(3)
     key: str = betterproto.string_field(4)
     starting_timestamp: int = betterproto.int64_field(5)
     ending_timestamp: int = betterproto.int64_field(6)
@@ -3694,14 +3787,51 @@
 @dataclass
 class GetBigQueryRegionResponse(betterproto.Message):
     region: str = betterproto.string_field(1)
     manually_set: bool = betterproto.bool_field(2)
 
 
 @dataclass
+class DbtJob(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    project_id: int = betterproto.int32_field(2)
+    name: str = betterproto.string_field(3)
+    dbt_job_ext_id: int = betterproto.int32_field(4)
+    is_favorite: bool = betterproto.bool_field(5)
+
+
+@dataclass
+class UpsertDbtJob(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    project_id: int = betterproto.int32_field(2)
+    name: str = betterproto.string_field(3)
+    dbt_job_id: int = betterproto.int32_field(4)
+
+
+@dataclass
+class GetDbtJobResponse(betterproto.Message):
+    dbt_job: "DbtJob" = betterproto.message_field(1)
+
+
+@dataclass
+class GetDbtJobsRequest(betterproto.Message):
+    project_id: int = betterproto.int32_field(1)
+
+
+@dataclass
+class GetDbtJobsResponse(betterproto.Message):
+    dbt_jobs: List["DbtJob"] = betterproto.message_field(1)
+
+
+@dataclass
+class UpdateUserRoleRequest(betterproto.Message):
+    role: "Role" = betterproto.enum_field(1)
+
+
+@dataclass
 class Empty(betterproto.Message):
     pass
 
 
 @dataclass
 class DimensionRun(betterproto.Message):
     dim_name: str = betterproto.string_field(1)
@@ -3910,14 +4040,15 @@
 
 @dataclass
 class CreateUserAndCompanyRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
     email: str = betterproto.string_field(2)
     password: str = betterproto.string_field(3)
     company_name: str = betterproto.string_field(4)
+    role: str = betterproto.string_field(5)
 
 
 @dataclass
 class AddUserRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
     email: str = betterproto.string_field(2)
     password: str = betterproto.string_field(3)
@@ -4001,14 +4132,15 @@
         schema_name: str = "",
         column_ids: List[int] = [],
         search: str = "",
         sort_direction: "SortDirection" = 0,
         schema_id: int = 0,
         metric_types: List["PredefinedMetricName"] = [],
         include_latest_metric_runs: bool = False,
+        workspace_id: int = 0,
     ) -> MetricInfoList:
         """Get metric information"""
 
         request = GetMetricInfoListRequest()
         request.metric_ids = metric_ids
         request.warehouse_ids = warehouse_ids
         request.table_ids = table_ids
@@ -4022,14 +4154,15 @@
         request.schema_name = schema_name
         request.column_ids = column_ids
         request.search = search
         request.sort_direction = sort_direction
         request.schema_id = schema_id
         request.metric_types = metric_types
         request.include_latest_metric_runs = include_latest_metric_runs
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.MetricService/GetMetricInfoBatch",
             request,
             MetricInfoList,
         )
 
@@ -4049,14 +4182,15 @@
         schema_name: str = "",
         column_ids: List[int] = [],
         search: str = "",
         sort_direction: "SortDirection" = 0,
         schema_id: int = 0,
         metric_types: List["PredefinedMetricName"] = [],
         include_latest_metric_runs: bool = False,
+        workspace_id: int = 0,
     ) -> MetricInfoList:
         """Get batch metric information"""
 
         request = GetMetricInfoListRequest()
         request.metric_ids = metric_ids
         request.warehouse_ids = warehouse_ids
         request.table_ids = table_ids
@@ -4070,14 +4204,15 @@
         request.schema_name = schema_name
         request.column_ids = column_ids
         request.search = search
         request.sort_direction = sort_direction
         request.schema_id = schema_id
         request.metric_types = metric_types
         request.include_latest_metric_runs = include_latest_metric_runs
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.MetricService/GetMetricInfoBatchPost",
             request,
             MetricInfoList,
         )
 
@@ -4097,14 +4232,15 @@
         schema_name: str = "",
         column_ids: List[int] = [],
         search: str = "",
         sort_direction: "SortDirection" = 0,
         schema_id: int = 0,
         metric_types: List["PredefinedMetricName"] = [],
         include_latest_metric_runs: bool = False,
+        workspace_id: int = 0,
     ) -> GetMetricsCountResponse:
         """Get count of metrics"""
 
         request = GetMetricInfoListRequest()
         request.metric_ids = metric_ids
         request.warehouse_ids = warehouse_ids
         request.table_ids = table_ids
@@ -4118,14 +4254,15 @@
         request.schema_name = schema_name
         request.column_ids = column_ids
         request.search = search
         request.sort_direction = sort_direction
         request.schema_id = schema_id
         request.metric_types = metric_types
         request.include_latest_metric_runs = include_latest_metric_runs
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.MetricService/GetMetricsCount",
             request,
             GetMetricsCountResponse,
         )
 
@@ -4697,25 +4834,27 @@
         warehouse_id: List[int] = [],
         schema: List[str] = [],
         table_name: List[str] = [],
         ids: List[int] = [],
         schema_id: List[int] = [],
         include_favorites: bool = False,
         ignore_fields: bool = False,
+        workspace_id: int = 0,
     ) -> TableList:
         """Search tables"""
 
         request = TableSearchRequest()
         request.warehouse_id = warehouse_id
         request.schema = schema
         request.table_name = table_name
         request.ids = ids
         request.schema_id = schema_id
         request.include_favorites = include_favorites
         request.ignore_fields = ignore_fields
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.TableService/SearchTables",
             request,
             TableList,
         )
 
@@ -4851,27 +4990,29 @@
         table_ids: List[int] = [],
         page_size: int = 0,
         page_cursor: str = "",
         sort_field: "TableSortField" = 0,
         sort_direction: "SortDirection" = 0,
         search: str = "",
         ignore_fields: bool = False,
+        workspace_id: int = 0,
     ) -> GetTableListResponse:
         """Get tables"""
 
         request = GetTableListRequest()
         request.source_ids = source_ids
         request.schema_ids = schema_ids
         request.table_ids = table_ids
         request.page_size = page_size
         request.page_cursor = page_cursor
         request.sort_field = sort_field
         request.sort_direction = sort_direction
         request.search = search
         request.ignore_fields = ignore_fields
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.TableService/GetTables",
             request,
             GetTableListResponse,
         )
 
@@ -4919,19 +5060,29 @@
             GetCountsResponse,
         )
 
 
 class SchemaServiceStub(betterproto.ServiceStub):
     """Get list of schemas"""
 
-    async def search_schemas(self, *, warehouse_id: List[int] = []) -> SchemaList:
+    async def search_schemas(
+        self,
+        *,
+        warehouse_id: List[int] = [],
+        schema_name: List[str] = [],
+        schema_id: List[int] = [],
+        workspace_id: int = 0,
+    ) -> SchemaList:
         """Search schemas"""
 
         request = SchemaSearchRequest()
         request.warehouse_id = warehouse_id
+        request.schema_name = schema_name
+        request.schema_id = schema_id
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.SchemaService/SearchSchemas",
             request,
             SchemaList,
         )
 
@@ -4966,24 +5117,26 @@
         *,
         source_ids: List[int] = [],
         page_size: int = 0,
         page_cursor: str = "",
         sort_field: "SchemaSortField" = 0,
         sort_direction: "SortDirection" = 0,
         search: str = "",
+        workspace_id: int = 0,
     ) -> GetSchemaListResponse:
         """Get schemas"""
 
         request = GetSchemaListRequest()
         request.source_ids = source_ids
         request.page_size = page_size
         request.page_cursor = page_cursor
         request.sort_field = sort_field
         request.sort_direction = sort_direction
         request.search = search
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.SchemaService/GetSchemas",
             request,
             GetSchemaListResponse,
         )
 
@@ -5091,27 +5244,29 @@
         table_ids: List[int] = [],
         column_ids: List[int] = [],
         page_size: int = 0,
         page_cursor: str = "",
         sort_field: "ColumnSortField" = 0,
         sort_direction: "SortDirection" = 0,
         search: str = "",
+        workspace_id: int = 0,
     ) -> GetColumnListResponse:
         """Get columns"""
 
         request = GetColumnListRequest()
         request.source_ids = source_ids
         request.schema_ids = schema_ids
         request.table_ids = table_ids
         request.column_ids = column_ids
         request.page_size = page_size
         request.page_cursor = page_cursor
         request.sort_field = sort_field
         request.sort_direction = sort_direction
         request.search = search
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.ColumnService/GetColumns",
             request,
             GetColumnListResponse,
         )
 
@@ -5123,23 +5278,25 @@
         self,
         *,
         page_size: int = 0,
         page_cursor: str = "",
         sort_field: "MetricTemplateSortField" = 0,
         sort_direction: "SortDirection" = 0,
         search: str = "",
+        workspace_id: int = 0,
     ) -> GetMetricTemplateListResponse:
         """Get all metric templates"""
 
         request = GetMetricTemplateListRequest()
         request.page_size = page_size
         request.page_cursor = page_cursor
         request.sort_field = sort_field
         request.sort_direction = sort_direction
         request.search = search
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.MetricTemplateService/GetMetricTemplates",
             request,
             GetMetricTemplateListResponse,
         )
 
@@ -5185,22 +5342,23 @@
         )
 
 
 class NamedScheduleServiceStub(betterproto.ServiceStub):
     """Named Schedules"""
 
     async def create_named_schedule(
-        self, *, id: int = 0, name: str = "", cron: str = ""
+        self, *, id: int = 0, name: str = "", cron: str = "", workspace_id: int = 0
     ) -> NamedSchedule:
         """Create a named schedule"""
 
         request = CreateNamedScheduleRequest()
         request.id = id
         request.name = name
         request.cron = cron
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.NamedScheduleService/CreateNamedSchedule",
             request,
             NamedSchedule,
         )
 
@@ -5323,25 +5481,27 @@
         comparison_table_ids: List[int] = [],
         exclude_comparison_metrics: bool = False,
         page_size: int = 0,
         page_cursor: str = "",
         sort_field: "ComparisonTableSortField" = 0,
         sort_direction: "SortDirection" = 0,
         search: str = "",
+        workspace_id: int = 0,
     ) -> GetComparisonTableInfosResponse:
         """Get information about deltas"""
 
         request = GetComparisonTableInfosRequest()
         request.comparison_table_ids = comparison_table_ids
         request.exclude_comparison_metrics = exclude_comparison_metrics
         request.page_size = page_size
         request.page_cursor = page_cursor
         request.sort_field = sort_field
         request.sort_direction = sort_direction
         request.search = search
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.DeltasService/GetComparisonTableInfos",
             request,
             GetComparisonTableInfosResponse,
         )
 
@@ -5398,14 +5558,15 @@
         related_issue_ids: List[int] = [],
         priority: List["IssuePriority"] = [],
         metric_status: List["MetricStatus"] = [],
         metric_type: List["MetricType"] = [],
         min_opened_time: int = 0,
         max_opened_time: int = 0,
         sort_options: List["IssueSortOption"] = [],
+        workspace_id: int = 0,
     ) -> GetIssuesResponse:
         """Get issues"""
 
         request = GetIssuesRequest()
         request.issue_ids = issue_ids
         request.current_status = current_status
         request.metric_ids = metric_ids
@@ -5426,14 +5587,15 @@
         request.metric_status = metric_status
         if metric_type is not None:
             request.metric_type = metric_type
         request.min_opened_time = min_opened_time
         request.max_opened_time = max_opened_time
         if sort_options is not None:
             request.sort_options = sort_options
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.IssueService/GetIssues",
             request,
             GetIssuesResponse,
         )
 
@@ -5563,23 +5725,25 @@
         self,
         *,
         page_size: int = 0,
         page_cursor: str = "",
         sort_field: "SourceSortField" = 0,
         sort_direction: "SortDirection" = 0,
         search: str = "",
+        workspace_id: int = 0,
     ) -> GetSourceListResponse:
         """Get sources"""
 
         request = GetSourceListRequest()
         request.page_size = page_size
         request.page_cursor = page_cursor
         request.sort_field = sort_field
         request.sort_direction = sort_direction
         request.search = search
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.SourceService/GetSources",
             request,
             GetSourceListResponse,
         )
 
@@ -5611,14 +5775,15 @@
         query_timeout_seconds: int = 0,
         skip_indexing: bool = False,
         alation_source_id: int = 0,
         atlan_connection_id: str = "",
         temporal_agent_secret: str = "",
         target_bigquery_project_id: str = "",
         bigquery_query_project_ids: str = "",
+        workspace_id: int = 0,
     ) -> SourceValidationResponse:
         """Validate source"""
 
         request = CreateSourceRequest()
         request.id = id
         request.name = name
         request.hostname = hostname
@@ -5632,14 +5797,15 @@
         request.query_timeout_seconds = query_timeout_seconds
         request.skip_indexing = skip_indexing
         request.alation_source_id = alation_source_id
         request.atlan_connection_id = atlan_connection_id
         request.temporal_agent_secret = temporal_agent_secret
         request.target_bigquery_project_id = target_bigquery_project_id
         request.bigquery_query_project_ids = bigquery_query_project_ids
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.SourceService/ValidateSource",
             request,
             SourceValidationResponse,
         )
 
@@ -5659,14 +5825,15 @@
         query_timeout_seconds: int = 0,
         skip_indexing: bool = False,
         alation_source_id: int = 0,
         atlan_connection_id: str = "",
         temporal_agent_secret: str = "",
         target_bigquery_project_id: str = "",
         bigquery_query_project_ids: str = "",
+        workspace_id: int = 0,
     ) -> CreateSourceResponse:
         """Create or update source"""
 
         request = CreateSourceRequest()
         request.id = id
         request.name = name
         request.hostname = hostname
@@ -5680,14 +5847,15 @@
         request.query_timeout_seconds = query_timeout_seconds
         request.skip_indexing = skip_indexing
         request.alation_source_id = alation_source_id
         request.atlan_connection_id = atlan_connection_id
         request.temporal_agent_secret = temporal_agent_secret
         request.target_bigquery_project_id = target_bigquery_project_id
         request.bigquery_query_project_ids = bigquery_query_project_ids
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.SourceService/CreateOrUpdateSource",
             request,
             CreateSourceResponse,
         )
 
@@ -5886,18 +6054,21 @@
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.VirtualTableService/UpdateVirtualTable",
             request,
             VirtualTable,
         )
 
-    async def get_all_virtual_tables(self) -> VirtualTableList:
+    async def get_all_virtual_tables(
+        self, *, workspace_id: int = 0
+    ) -> VirtualTableList:
         """Get all Virtual Tables"""
 
-        request = Empty()
+        request = GetAllVirtualTablesRequest()
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.VirtualTableService/GetAllVirtualTables",
             request,
             VirtualTableList,
         )
 
@@ -5909,27 +6080,29 @@
         table_ids: List[int] = [],
         page_size: int = 0,
         page_cursor: str = "",
         sort_field: "VirtualTableSortField" = 0,
         sort_direction: "SortDirection" = 0,
         search: str = "",
         ignore_fields: bool = False,
+        workspace_id: int = 0,
     ) -> GetVirtualTableListResponse:
         """Get Virtual Tables"""
 
         request = GetVirtualTableListRequest()
         request.source_ids = source_ids
         request.schema_ids = schema_ids
         request.table_ids = table_ids
         request.page_size = page_size
         request.page_cursor = page_cursor
         request.sort_field = sort_field
         request.sort_direction = sort_direction
         request.search = search
         request.ignore_fields = ignore_fields
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.VirtualTableService/GetVirtualTables",
             request,
             GetVirtualTableListResponse,
         )
 
@@ -5962,20 +6135,22 @@
     async def create_data_node(
         self,
         *,
         node_type: "DataNodeType" = 0,
         node_entity_id: int = 0,
         node_name: str = "",
         node_container_name: str = "",
+        workspace_id: int = 0,
     ) -> DataNode:
         request = CreateDataNodeRequest()
         request.node_type = node_type
         request.node_entity_id = node_entity_id
         request.node_name = node_name
         request.node_container_name = node_container_name
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.LineageService/CreateDataNode",
             request,
             DataNode,
         )
 
@@ -6142,26 +6317,28 @@
         api_port: int = 0,
         web_base_uri: str = "",
         web_port: int = 0,
         namespace: str = "",
         credentials_public: str = "",
         credentials_private: str = "",
         timeout: int = 0,
+        workspace_id: int = 0,
     ) -> Integration:
         request = CreateOrUpdateIntegrationRequest()
         request.name = name
         request.integration_partner = integration_partner
         request.api_base_uri = api_base_uri
         request.api_port = api_port
         request.web_base_uri = web_base_uri
         request.web_port = web_port
         request.namespace = namespace
         request.credentials_public = credentials_public
         request.credentials_private = credentials_private
         request.timeout = timeout
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.IntegrationService/CreateIntegration",
             request,
             Integration,
         )
 
@@ -6224,16 +6401,17 @@
             "/com.bigeye.models.generated.IntegrationService/getTableauWorkbook",
             request,
             TableauWorkbook,
         )
 
 
 class FavoriteServiceStub(betterproto.ServiceStub):
-    async def get_favorites(self) -> FavoriteListResponse:
-        request = Empty()
+    async def get_favorites(self, *, workspace_id: int = 0) -> FavoriteListResponse:
+        request = GetFavoritesRequest()
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.FavoriteService/GetFavorites",
             request,
             FavoriteListResponse,
         )
 
@@ -6295,25 +6473,27 @@
         sort_field: "SchemaChangeSortField" = 0,
         sort_direction: "SortDirection" = 0,
         search: str = "",
         source_id: int = 0,
         schema_id: int = 0,
         table_id: int = 0,
         column_id: int = 0,
+        workspace_id: int = 0,
     ) -> GetSchemaChangesResponse:
         request = GetSchemaChangesRequest()
         request.page_size = page_size
         request.page_cursor = page_cursor
         request.sort_field = sort_field
         request.sort_direction = sort_direction
         request.search = search
         request.source_id = source_id
         request.schema_id = schema_id
         request.table_id = table_id
         request.column_id = column_id
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.SchemaChangeService/GetSchemaChanges",
             request,
             GetSchemaChangesResponse,
         )
 
@@ -6336,19 +6516,20 @@
         return await self._unary_unary(
             "/com.bigeye.models.generated.DeltaService/RunDelta",
             request,
             RunDeltaResponse,
         )
 
     async def create_delta(
-        self, *, delta: Optional["Delta"] = None
+        self, *, delta: Optional["Delta"] = None, workspace_id: int = 0
     ) -> UpsertDeltaResponse:
         request = UpsertDeltaRequest()
         if delta is not None:
             request.delta = delta
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.DeltaService/CreateDelta",
             request,
             UpsertDeltaResponse,
         )
 
@@ -6371,19 +6552,20 @@
         return await self._unary_unary(
             "/com.bigeye.models.generated.DeltaService/BulkOperationDeltas",
             request,
             BulkResponse,
         )
 
     async def edit_delta(
-        self, *, delta: Optional["Delta"] = None
+        self, *, delta: Optional["Delta"] = None, workspace_id: int = 0
     ) -> UpsertDeltaResponse:
         request = UpsertDeltaRequest()
         if delta is not None:
             request.delta = delta
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.DeltaService/EditDelta",
             request,
             UpsertDeltaResponse,
         )
 
@@ -6403,23 +6585,25 @@
         comparison_table_ids: List[int] = [],
         exclude_comparison_metrics: bool = False,
         page_size: int = 0,
         page_cursor: str = "",
         sort_field: "ComparisonTableSortField" = 0,
         sort_direction: "SortDirection" = 0,
         search: str = "",
+        workspace_id: int = 0,
     ) -> GetDeltaInfosResponse:
         request = GetComparisonTableInfosRequest()
         request.comparison_table_ids = comparison_table_ids
         request.exclude_comparison_metrics = exclude_comparison_metrics
         request.page_size = page_size
         request.page_cursor = page_cursor
         request.sort_field = sort_field
         request.sort_direction = sort_direction
         request.search = search
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.DeltaService/FetchDeltas",
             request,
             GetDeltaInfosResponse,
         )
```

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/generated/google/api.py` & `bigeye_sdk-0.4.56/bigeye_sdk/generated/google/api.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.56/bigeye_sdk/model/big_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import List, Optional, Dict, Tuple, Any, Union
 
+import os
 import yaml
 from pydantic import Field, PrivateAttr, validator, root_validator
 
 from bigeye_sdk.bigconfig_validation.validation_functions import safe_split_dict_entry_lines, must_be_list_validator
 from bigeye_sdk.bigconfig_validation.yaml_model_base import YamlModelWithValidatorContext
 from bigeye_sdk.bigconfig_validation.yaml_validation_error_messages import DUPLICATE_SAVED_METRIC_ID_EXISTS_ERRMSG, \
     DUPLICATE_TAG_EXISTS_ERRMSG, TAG_ID_NOT_EXISTS_IN_TAG_DEFINITION_ERRMSG, \
@@ -119,17 +120,17 @@
         must_be_list_validator(clazz=RowCreationTimes, attribute_name='tag_ids', values=values)
         must_be_list_validator(clazz=RowCreationTimes, attribute_name='column_selectors', values=values)
 
         return values
 
 
 class TagDeployment(YamlModelWithValidatorContext):
+    column_selectors: Optional[List[ColumnSelector]] = Field(default_factory=lambda: [])
     metrics: List[SimpleMetricDefinition]
     tag_id: Optional[str] = None
-    column_selectors: Optional[List[ColumnSelector]] = Field(default_factory=lambda: [])
 
     @root_validator(pre=True)
     def must_be_list(cls, values):
         must_be_list_validator(clazz=TagDeployment, attribute_name='metrics', values=values)
         must_be_list_validator(clazz=TagDeployment, attribute_name='column_selectors', values=values)
 
         return values
@@ -144,17 +145,17 @@
 
         Returns: list of names from each fully qualified column selector in the Tag Deployment
         """
         return [explode_fq_column_selectors(i.name) for i in self.column_selectors]
 
 
 class TagDeploymentSuite(YamlModelWithValidatorContext):
+    collection: Optional[SimpleCollection] = None
     deployments: List[TagDeployment]
     sla: Optional[SimpleSLA] = None
-    collection: Optional[SimpleCollection] = None
 
     @root_validator(pre=True)
     def must_be_list(cls, values):
         must_be_list_validator(clazz=TagDeploymentSuite, attribute_name='deployments', values=values)
 
         return values
 
@@ -239,17 +240,17 @@
         Returns: list of names from the fully qualified table name
         """
 
         return explode_fq_table_name(self.fq_table_name)
 
 
 class TableDeploymentSuite(YamlModelWithValidatorContext):
+    collection: Optional[SimpleCollection] = None
     deployments: List[TableDeployment]
     sla: Optional[SimpleSLA] = None
-    collection: Optional[SimpleCollection] = None
 
     @root_validator(pre=True)
     def must_be_list(cls, values):
         must_be_list_validator(clazz=TableDeploymentSuite, attribute_name='deployments', values=values)
 
         return values
 
@@ -512,7 +513,127 @@
                 collections.append(d.collection)
 
         for d in self.table_deployments:
             if d.collection:
                 collections.append(d.collection)
 
         return collections
+    
+    def create_bigconfig_from_metrics(self, tag_deployments: List[TagDeployment], 
+                                      collection_name: str = 'SDK Generated', 
+                                      collection_description: str = None) -> BigConfig:
+        """
+        This function accepts a list of tag deployments and converts it into a valid and
+        readable Bigconfig file for export. 
+
+        This will take an input that looks like this...
+
+        {
+            tag_deployments: [
+                {
+                    tag_deployment: {
+                        column_selectors: ['some_path_to_column'], 
+                        metrics: [metric_1, metric_2, metric_3]}
+                },
+                {
+                    tag_deployment: {
+                        column_selectors: ['some_path_to_other_column'], 
+                        metrics: [metric_1, metric_2, metric_3]}
+                },
+            ]
+        }
+
+        And convert it into something that looks like this...
+
+        {
+            saved_metric_definitions: [
+                metric_1,
+                metric_2,
+                metric_3
+            ]
+            tag_deployments: [
+                {
+                    collection: some_name,
+                    description: some description,
+                    deployments: {
+                        column_selectors: [
+                            'some_path_to_column',
+                            'some_path_to_other_column
+                        ]', 
+                        metrics: [
+                            metric_1_id, 
+                            metric_2_id, 
+                            metric_3_id
+                        ]
+                    }
+                }
+            ]
+        }
+        """
+        def _simple_metrics_to_saved_metric_defs(simple_metric_defs: List[SimpleMetricDefinition]) -> SavedMetricDefinitions:
+            output: List[SimpleMetricDefinition] = []
+            for m in simple_metric_defs:
+                m.saved_metric_id = m.metric_name.replace(" ","_") # this will only work for dbt tests
+                # params should only be given for template metrics with parameters provided
+                if m.parameters:
+                    for i, param in enumerate(m.parameters):
+                        if param.key == 'arg1':
+                            m.parameters.pop(i)
+                    if len(m.parameters) == 0:
+                        m.parameters = None
+                # need this b/c lookback gets added as empty object rather than default None
+                if m.lookback and m.lookback.is_default_value:
+                    m.lookback = None
+                if m not in output:
+                    output.append(m)
+
+            return SavedMetricDefinitions(metrics=output)
+
+        def _group_column_selectors_for_saved_config(smd:SimpleMetricDefinition):
+            column_selectors: List[ColumnSelector] = []
+            for td in tag_deployments:
+                for metric in td.metrics:
+                    if metric == smd:
+                        column_selectors.extend(td.column_selectors)
+            return column_selectors
+        
+        def _dedupe_column_selectors(deployments: List[TagDeployment]) -> List[TagDeployment]:
+            final_deployments: List[TagDeployment] = []
+            last_deployment: TagDeployment = None
+            for deployment in deployments:
+                if last_deployment is None or deployment.column_selectors != last_deployment.column_selectors:
+                    final_deployments.append(deployment)
+                    last_deployment = deployment
+                else:
+                    last_deployment.metrics.extend(deployment.metrics)
+                last_deployment = deployment
+            
+            return final_deployments
+        
+        simple_metrics: List[SimpleMetricDefinition] = []
+        for tag_deployment in tag_deployments:
+            for m in tag_deployment.metrics:
+                simple_metrics.append(m)
+        
+        saved_metric_defs: SavedMetricDefinitions = _simple_metrics_to_saved_metric_defs(simple_metric_defs=simple_metrics)
+        deployments: List[TagDeployment] = []
+        for smd in saved_metric_defs.metrics:
+            tag_deployment = TagDeployment(
+                column_selectors=_group_column_selectors_for_saved_config(smd=smd),
+                metrics=[SimpleMetricDefinition(saved_metric_id=smd.saved_metric_id)]
+            )
+            deployments.append(tag_deployment)       
+        
+        final_deployments = _dedupe_column_selectors(deployments)
+        
+        tag_deployment_suite = TagDeploymentSuite(
+                                collection=SimpleCollection(
+                                    name=collection_name,
+                                    description=collection_description
+                                ),
+                                deployments=final_deployments
+                            )
+
+        return BigConfig(
+            type='BIGCONFIG_FILE',
+            saved_metric_definitions=saved_metric_defs,
+            tag_deployments=[tag_deployment_suite])
```

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.56/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/model/dbt_schema.py` & `bigeye_sdk-0.4.56/bigeye_sdk/model/dbt_schema.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.56/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.56/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -1084,15 +1084,17 @@
         builder.lookback = SimpleLookback(lookback_window=SimpleTimeInterval.from_datawatch_object(obj.lookback),
                                           lookback_type=SimpleLookbackType.from_datawatch_object(obj.lookback_type),
                                           bucket_size=BucketSize.from_seconds(obj.grain_seconds))
 
         builder.muted_until_epoch_seconds = obj.muted_until_epoch_seconds
         builder.grain_seconds = obj.grain_seconds
 
-        builder.collection_ids = obj.collection_ids
+        if isinstance(obj,MetricDefinition):
+            builder.collection_ids = obj.collection_ids
+
         builder.metric_schedule = SimpleMetricSchedule.from_datawatch_object(obj.metric_schedule)
         return builder
 
     def to_datawatch_object(self, to_config: bool = False, **kwargs) -> Union[MetricDefinition, MetricConfiguration]:
         if to_config:
             builder = MetricConfiguration()
         else:
@@ -1126,15 +1128,18 @@
         if self.lookback:
             if self.lookback.lookback_window:
                 builder.lookback = self.lookback.lookback_window.to_datawatch_object()
 
             if self.lookback.lookback_type:
                 builder.lookback_type = self.lookback.lookback_type.to_datawatch_object()
 
-            """Freshness metrics require data time lookback"""
+            """
+            Freshness metrics require data time lookback. This is handled by the backend.
+            See https://linear.app/torodata/issue/WIZ-2583/[061223]-metric-deployed-via-bigconfig-not-showing-as-clock-time
+            """
             if SimpleMetricType.is_freshness_metric(self.metric_type):
                 builder.lookback_type = SimpleLookbackType.DATA_TIME.to_datawatch_object()
 
             builder.grain_seconds = self.lookback.bucket_size.to_seconds()
 
         if SimpleMetricType.is_freshness_volume(self.metric_type):
             builder.grain_seconds = BucketSize.HOUR.to_seconds()
@@ -1142,8 +1147,8 @@
         builder.muted_until_epoch_seconds = self.muted_until_epoch_seconds
 
         if self.collection_ids:
             builder.collection_ids = self.collection_ids
         if self.metric_schedule:
             builder.metric_schedule = self.metric_schedule.to_datawatch_object()
 
-        return builder
+        return builder
```

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.56/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.55/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.56/bigeye_sdk/serializable.py`

 * *Files 9% similar despite different names*

```diff
@@ -147,16 +147,21 @@
                 log.info('Generating FixMe files.')
                 errmsg = f'File is invalid.  File: {file_name};' \
                          f"\nErrors: \n{errmsg};" \
                          f'\nFIXME Files: {yaml.safe_dump(fixme_file_list)}'
 
             raise FileLoadException(errmsg)
 
-    def save(self, file: str):
-        with open(file, 'w') as fout:
+    def save(self, output_path: str, default_file_name: str = None):
+        if os.path.isfile(output_path):
+            output_path = output_path
+        elif os.path.isdir(output_path):
+            output_path = f'{output_path}/{default_file_name}.yml'
+
+        with open(output_path, 'w') as fout:
             lines = self.yaml(exclude_unset=True, exclude_none=True, exclude_defaults=self._exclude_defaults,
                               indent=True)
             fout.writelines(lines)
 
 
 BIGCONFIG_FILE = TypeVar('BIGCONFIG_FILE', bound='BigConfigFile')
```

### Comparing `bigeye_sdk-0.4.55/pyproject.toml` & `bigeye_sdk-0.4.56/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.55"
+version = "0.4.56"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
```

### Comparing `bigeye_sdk-0.4.55/PKG-INFO` & `bigeye_sdk-0.4.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.55
+Version: 0.4.56
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```

