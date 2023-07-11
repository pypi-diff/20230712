# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev8.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0.dev9.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev8.tar` & `dbt_semantic_interfaces-0.1.0.dev9.tar`

### file list

```diff
@@ -1,85 +1,105 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/CHANGELOG.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/project_configuration.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_version.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    15561 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/generate_json_schema_file.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/project_configuration.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/semantic_version.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/time_spine_configuration.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    28360 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
--rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/README.md
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/.tool-versions
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/project_configuration.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_version.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/generate_json_schema_file.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/project_configuration.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_version.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/time_spine_configuration.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/agg_time_dimension.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28360 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/Activate.ps1
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/activate
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/activate.csh
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/activate.fish
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/hatch
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/hatchling
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/httpx
+-rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/keyring
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/markdown-it
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/pip3.9
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/python3.9 -> python
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/userpath
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/virtualenv
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/README.md
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/Makefile` & `dbt_semantic_interfaces-0.1.0.dev9/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/project_configuration.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/project_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_version.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_version.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/where_filter.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,14 @@
     semantic_models = []
     metrics = []
     project_configurations = []
     valid_object_classes = [semantic_model_class.__name__, metric_class.__name__, project_configuration_class.__name__]
     issues: List[ValidationIssue] = []
 
     for config_file in files:
-        logger.error(f"Parsing: {config_file}")
         parsing_result = parse_config_yaml(  # parse config file
             config_file,
             semantic_model_class=semantic_model_class,
             metric_class=metric_class,
             project_configuration_class=project_configuration_class,
         )
         file_issues = parsing_result.issues
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/generate_json_schema_file.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/generate_json_schema_file.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/__init__.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/measure.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,19 +65,14 @@
     @property
     @abstractmethod
     def description(self) -> Optional[str]:  # noqa: D
         pass
 
     @property
     @abstractmethod
-    def create_metric(self) -> Optional[bool]:  # noqa: D
-        pass
-
-    @property
-    @abstractmethod
     def expr(self) -> Optional[str]:  # noqa: D
         pass
 
     @property
     @abstractmethod
     def agg_params(self) -> Optional[MeasureAggregationParameters]:  # noqa: D
         pass
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/project_configuration.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/project_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/time_spine_configuration.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/time_spine_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/names.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/semantic_manifest_validator.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,19 +193,18 @@
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="checking validity of the semantic model's default agg_time_dimension")
     def _validate_default_agg_time_dimension(semantic_model: SemanticModel) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
-        if semantic_model.defaults is None:
+        if semantic_model.defaults is None or semantic_model.defaults.agg_time_dimension is None:
             return []
 
         default_agg_time_dimension = semantic_model.defaults.agg_time_dimension
-        assert default_agg_time_dimension is not None, "should not be None"
 
         if not SemanticModelValidationHelpers.time_dimension_in_model(
             time_dimension_name=default_agg_time_dimension, semantic_model=semantic_model
         ):
             issues.append(
                 ValidationError(
                     context=SemanticModelContext(
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,13 +403,13 @@
         issues_str = "\n".join([x.as_readable_str(verbose=True) for x in issues])
         super().__init__(f"Error validating model. Issues:\n{issues_str}")
 
 
 class SemanticModelValidationHelpers:
     """Class containing all the helpers related to semantic model validations."""
 
-    @classmethod
-    def time_dimension_in_model(cls, time_dimension_name: str, semantic_model: SemanticModel) -> bool:  # noqa: D
+    @staticmethod
+    def time_dimension_in_model(time_dimension_name: str, semantic_model: SemanticModel) -> bool:  # noqa: D
         for dimension in semantic_model.dimensions:
             if dimension.type == DimensionType.TIME and dimension.name == time_dimension_name:
                 return True
         return False
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/.gitignore` & `dbt_semantic_interfaces-0.1.0.dev9/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/LICENSE` & `dbt_semantic_interfaces-0.1.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/README.md` & `dbt_semantic_interfaces-0.1.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/pyproject.toml` & `dbt_semantic_interfaces-0.1.0.dev9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev8"
+version = "0.1.0.dev9"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev8/PKG-INFO` & `dbt_semantic_interfaces-0.1.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev8
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev9
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

