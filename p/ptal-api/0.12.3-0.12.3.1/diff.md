# Comparing `tmp/ptal_api-0.12.3.tar.gz` & `tmp/ptal_api-0.12.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.12.3.tar", max compression
+gzip compressed data, was "ptal_api-0.12.3.1.tar", max compression
```

## Comparing `ptal_api-0.12.3.tar` & `ptal_api-0.12.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      627 2023-07-11 09:36:41.189674 ptal_api-0.12.3/README.md
--rw-r--r--   0        0        0        0 2023-07-11 09:36:41.269676 ptal_api-0.12.3/ptal_api/__init__.py
--rw-r--r--   0        0        0   119338 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/adapter.py
--rw-r--r--   0        0        0      184 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      484 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/query_factory.py
--rw-r--r--   0        0        0      435 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      737 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    14955 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      904 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3255 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2194 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1464 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4556 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    23314 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1800 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3571 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0      295 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/common.py
--rw-r--r--   0        0        0     1880 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/object_types.py
--rw-r--r--   0        0        0     2884 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/objects.py
--rw-r--r--   0        0        0     3716 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/pretty_adapter.py
--rw-r--r--   0        0        0      595 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/property_values.py
--rw-r--r--   0        0        0    16486 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/transformer.py
--rw-r--r--   0        0        0        0 2023-07-11 09:36:41.273676 ptal_api-0.12.3/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1282 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-07-11 09:36:41.273676 ptal_api-0.12.3/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   289388 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    99292 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   135630 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3662 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-07-11 09:36:41.273676 ptal_api-0.12.3/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1211 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1889 2023-07-11 09:36:41.197674 ptal_api-0.12.3/pyproject.toml
--rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 ptal_api-0.12.3/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-06-27 07:04:23.668768 ptal_api-0.12.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 10:45:37.648937 ptal_api-0.12.3.1/ptal_api/__init__.py
+-rw-r--r--   0        0        0   119338 2023-07-10 07:23:26.618206 ptal_api-0.12.3.1/ptal_api/adapter.py
+-rw-r--r--   0        0        0      184 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      484 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/query_factory.py
+-rw-r--r--   0        0        0      435 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      737 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    14955 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      904 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3255 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2194 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1464 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4556 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    23314 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1800 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3571 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0      295 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/common.py
+-rw-r--r--   0        0        0     1880 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/object_types.py
+-rw-r--r--   0        0        0     2884 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/objects.py
+-rw-r--r--   0        0        0     3716 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/pretty_adapter.py
+-rw-r--r--   0        0        0      595 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/property_values.py
+-rw-r--r--   0        0        0    16486 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/transformer.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:45:37.652937 ptal_api-0.12.3.1/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-03 14:44:56.725951 ptal_api-0.12.3.1/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1282 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 10:45:37.652937 ptal_api-0.12.3.1/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   289388 2023-07-11 09:39:21.014656 ptal_api-0.12.3.1/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    99292 2023-07-11 09:39:21.014656 ptal_api-0.12.3.1/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-06-27 07:04:23.676768 ptal_api-0.12.3.1/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   135630 2023-07-11 09:39:21.014656 ptal_api-0.12.3.1/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3662 2023-06-27 07:04:23.676768 ptal_api-0.12.3.1/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-07-12 10:45:37.652937 ptal_api-0.12.3.1/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-27 07:04:23.676768 ptal_api-0.12.3.1/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1914 2023-07-12 10:38:31.980190 ptal_api-0.12.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 ptal_api-0.12.3.1/PKG-INFO
```

### Comparing `ptal_api-0.12.3/README.md` & `ptal_api-0.12.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/adapter.py` & `ptal_api-0.12.3.1/ptal_api/adapter.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/core/values/value_mapping.py` & `ptal_api-0.12.3.1/ptal_api/core/values/value_mapping.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/pretty_adapter/object_types.py` & `ptal_api-0.12.3.1/ptal_api/pretty_adapter/object_types.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/pretty_adapter/objects.py` & `ptal_api-0.12.3.1/ptal_api/pretty_adapter/objects.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/pretty_adapter/pretty_adapter.py` & `ptal_api-0.12.3.1/ptal_api/pretty_adapter/pretty_adapter.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/pretty_adapter/property_values.py` & `ptal_api-0.12.3.1/ptal_api/pretty_adapter/property_values.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/pretty_adapter/transformer.py` & `ptal_api-0.12.3.1/ptal_api/pretty_adapter/transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/providers/gql_providers.py` & `ptal_api-0.12.3.1/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/schema/README.md` & `ptal_api-0.12.3.1/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/schema/api_schema.py` & `ptal_api-0.12.3.1/ptal_api/schema/api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.12.3.1/ptal_api/schema/crawlers_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.12.3.1/ptal_api/schema/tcontroller_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.12.3.1/ptal_api/schema/utils_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/scripts/type_mapper.py` & `ptal_api-0.12.3.1/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.12.3.1/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3/pyproject.toml` & `ptal_api-0.12.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.12.3"
+version = "0.12.3.1"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
@@ -25,14 +25,15 @@
 python-keycloak = ">=2.6.0"
 graphql-core = ">=3.2.3"
 transliterate = ">=1.10.2"
 marshmallow-dataclass = ">=8.5.11"
 "ruamel.yaml" = ">=0.17.21"
 click = ">=8.1.3"
 pyjwt = ">=2.7.0"
+deprecation = "^2.1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
 ruff = "^0.0.261"
 black = "^23.3.0"
 
 [tool.black]
```

### Comparing `ptal_api-0.12.3/PKG-INFO` & `ptal_api-0.12.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.12.3
+Version: 0.12.3.1
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3)
+Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: graphql-core (>=3.2.3)
 Requires-Dist: marshmallow-dataclass (>=8.5.11)
 Requires-Dist: pyjwt (>=2.7.0)
 Requires-Dist: python-keycloak (>=2.6.0)
 Requires-Dist: ruamel.yaml (>=0.17.21)
 Requires-Dist: sgqlc (>=16.0)
 Requires-Dist: transliterate (>=1.10.2)
```

