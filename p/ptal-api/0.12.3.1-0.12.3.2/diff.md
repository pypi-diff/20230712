# Comparing `tmp/ptal_api-0.12.3.1.tar.gz` & `tmp/ptal_api-0.12.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.12.3.1.tar", max compression
+gzip compressed data, was "ptal_api-0.12.3.2.tar", max compression
```

## Comparing `ptal_api-0.12.3.1.tar` & `ptal_api-0.12.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      627 2023-06-27 07:04:23.668768 ptal_api-0.12.3.1/README.md
--rw-r--r--   0        0        0        0 2023-07-12 10:45:37.648937 ptal_api-0.12.3.1/ptal_api/__init__.py
--rw-r--r--   0        0        0   119338 2023-07-10 07:23:26.618206 ptal_api-0.12.3.1/ptal_api/adapter.py
--rw-r--r--   0        0        0      184 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      484 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/query_factory.py
--rw-r--r--   0        0        0      435 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      737 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    14955 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      904 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3255 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2194 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1464 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4556 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    23314 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1800 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3571 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0      295 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/common.py
--rw-r--r--   0        0        0     1880 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/object_types.py
--rw-r--r--   0        0        0     2884 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/objects.py
--rw-r--r--   0        0        0     3716 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/pretty_adapter.py
--rw-r--r--   0        0        0      595 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/property_values.py
--rw-r--r--   0        0        0    16486 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/pretty_adapter/transformer.py
--rw-r--r--   0        0        0        0 2023-07-12 10:45:37.652937 ptal_api-0.12.3.1/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-03 14:44:56.725951 ptal_api-0.12.3.1/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1282 2023-06-27 07:04:23.672768 ptal_api-0.12.3.1/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-07-12 10:45:37.652937 ptal_api-0.12.3.1/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   289388 2023-07-11 09:39:21.014656 ptal_api-0.12.3.1/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    99292 2023-07-11 09:39:21.014656 ptal_api-0.12.3.1/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-06-27 07:04:23.676768 ptal_api-0.12.3.1/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   135630 2023-07-11 09:39:21.014656 ptal_api-0.12.3.1/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3662 2023-06-27 07:04:23.676768 ptal_api-0.12.3.1/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-07-12 10:45:37.652937 ptal_api-0.12.3.1/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-27 07:04:23.676768 ptal_api-0.12.3.1/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1914 2023-07-12 10:38:31.980190 ptal_api-0.12.3.1/pyproject.toml
--rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 ptal_api-0.12.3.1/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-07-12 15:50:14.546886 ptal_api-0.12.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 15:50:14.606886 ptal_api-0.12.3.2/ptal_api/__init__.py
+-rw-r--r--   0        0        0   120733 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/adapter.py
+-rw-r--r--   0        0        0      184 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      484 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/query_factory.py
+-rw-r--r--   0        0        0      435 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      737 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    14955 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      904 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3255 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2194 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1464 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4556 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    23314 2023-07-12 15:50:14.550886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1800 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      387 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     5437 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0      295 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/pretty_adapter/common.py
+-rw-r--r--   0        0        0     1880 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/pretty_adapter/object_types.py
+-rw-r--r--   0        0        0     2884 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/pretty_adapter/objects.py
+-rw-r--r--   0        0        0     3716 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/pretty_adapter/pretty_adapter.py
+-rw-r--r--   0        0        0      595 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/pretty_adapter/property_values.py
+-rw-r--r--   0        0        0    16643 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/pretty_adapter/transformer.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:50:14.610886 ptal_api-0.12.3.2/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1282 2023-07-12 15:50:14.554886 ptal_api-0.12.3.2/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 15:50:14.610886 ptal_api-0.12.3.2/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   289388 2023-07-12 15:50:14.558886 ptal_api-0.12.3.2/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    99292 2023-07-12 15:50:14.558886 ptal_api-0.12.3.2/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-07-12 15:50:14.558886 ptal_api-0.12.3.2/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   135630 2023-07-12 15:50:14.558886 ptal_api-0.12.3.2/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3662 2023-07-12 15:50:14.558886 ptal_api-0.12.3.2/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:50:14.610886 ptal_api-0.12.3.2/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-12 15:50:14.558886 ptal_api-0.12.3.2/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1914 2023-07-12 15:50:14.558886 ptal_api-0.12.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 ptal_api-0.12.3.2/PKG-INFO
```

### Comparing `ptal_api-0.12.3.1/README.md` & `ptal_api-0.12.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/adapter.py` & `ptal_api-0.12.3.2/ptal_api/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     ConceptSorting,
     ConceptType,
     ConceptTypeFilterSettings,
     ConceptTypePagination,
     ConceptTypeSorting,
     ConceptUnmergeInput,
     ConceptUpdateInput,
+    DateInput,
     DateTimeValue,
     DateTimeValueInput,
     Document,
     DocumentFilterSettings,
     DocumentGrouping,
     DocumentLinkFilterSetting,
     DocumentSorting,
@@ -95,14 +96,15 @@
     Story,
     StoryPagination,
     StringFilter,
     StringLocaleValue,
     StringLocaleValueInput,
     StringValue,
     StringValueInput,
+    TimeInput,
     TimestampInterval,
     ValueInput,
 )
 from .schema.crawlers_api_schema import Crawler, CrawlerPagination
 from .schema.crawlers_api_schema import Query as CrQuery
 from .tdm_builder.tdm_builder import AbstractTdmBuilder
 
@@ -187,14 +189,17 @@
         self.concept_type_fields = ("id", "name")
 
         self.concept_property_fields = ("id", "is_main", "system_registration_date")
         self.concept_property_type_fields = ("id", "name")
         self.cpvt_fields_truncated = ("id", "name", "value_type")
         self.cpvt_fields = ("id", "name", "value_type", "value_restriction", "pretrained_nercmodels")
 
+        self.composite_property_value_template_fields = ("id", "name")
+        self.component_value_types_fields = ("id", "name")
+
         self.concept_link_fields = ("id", "notes")
         self.concept_link_type_fields = ("id", "name", "is_directed", "is_hierarchical")
         self.concept_link_type_fields_truncated = ("id", "name", "is_directed")
 
         self.concept_fact_fields = ("id",)
 
         self.composite_concept_widget_type = ("id", "name")
@@ -310,15 +315,29 @@
     def _configure_output_properties_fields(
         self,
         property_object,
         with_facts=False,
     ):
         property_object.__fields__(*self.concept_property_fields)
         property_object.access_level()
-        property_object.property_type().__fields__(*self.concept_property_type_fields)
+        pt = property_object.property_type()
+        pt.__fields__(*self.concept_property_type_fields)
+        vt = pt.value_type()
+
+        cpvt_frag = Fragment(ConceptPropertyValueType, "ConceptPropertyValueType")
+        cpvt_frag.__fields__(*self.cpvt_fields_truncated)
+
+        comp_frag = Fragment(CompositePropertyValueTemplate, "CompositePropertyValueTemplate")
+        comp_frag.__fields__(*self.composite_property_value_template_fields)
+        comp_frag.component_value_types().__fields__(*self.component_value_types_fields)
+        comp_frag.component_value_types().value_type().__fields__(*self.cpvt_fields_truncated)
+
+        vt.__fragment__(cpvt_frag)
+        vt.__fragment__(comp_frag)
+
         self._configure_output_value_fields(property_object.value)
         if with_facts:
             property_object.__fields__("list_concept_property_fact")
 
     def _configure_output_concept_fields(
         self,
         concept_object,
@@ -1421,29 +1440,43 @@
 
     def _get_value_input_by_value(self, value: Any, named_value_id: Optional[str] = None) -> ComponentValueInput:
         if isinstance(value, (StringValue, uas.StringValue)):
             value_input = ComponentValueInput(value=ValueInput(string_value_input=StringValueInput(value=value.value)))
         elif isinstance(value, (IntValue, uas.IntValue)):
             value_input = ComponentValueInput(value=ValueInput(int_value_input=IntValueInput(value=value.number)))
         elif isinstance(value, (DateTimeValue, uas.DateTimeValue)):
+            date_input = DateInput(
+                year=getattr(value.date, "year", None),
+                month=getattr(value.date, "month", None),
+                day=getattr(value.date, "day", None),
+            )
+            if all(
+                (
+                    hasattr(value, "time"),
+                    hasattr(value.time, "hour"),
+                    hasattr(value.time, "minute"),
+                    hasattr(value.time, "second"),
+                )
+            ):
+                time_input = TimeInput(hour=value.time.hour, minute=value.time.minute, second=value.time.second)
+            else:
+                time_input = None
             value_input = ComponentValueInput(
-                value=ValueInput(date_time_value_input=DateTimeValueInput(date=value.date, time=value.time))
+                value=ValueInput(date_time_value_input=DateTimeValueInput(date=date_input, time=time_input))
             )
         elif isinstance(value, (StringLocaleValue, uas.StringLocaleValue)):
             value_input = ComponentValueInput(
                 value=ValueInput(
                     string_locale_value_input=StringLocaleValueInput(value=value.value, locale=value.locale)
                 )
             )
         elif isinstance(value, (LinkValue, uas.LinkValue)):
             value_input = ComponentValueInput(value=ValueInput(link_value_input=LinkValueInput(link=value.link)))
         elif isinstance(value, (DoubleValue, uas.DoubleValue)):
-            value_input = ComponentValueInput(
-                value=ValueInput(double_value_input=DoubleValueInput(double=value.double))
-            )
+            value_input = ComponentValueInput(value=ValueInput(double_value_input=DoubleValueInput(value=value.double)))
         else:
             raise NotImplementedError(f"{type(value)} type is not supported")
 
         if named_value_id:
             value_input.id = named_value_id
         return value_input
```

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.12.3.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/pretty_adapter/object_types.py` & `ptal_api-0.12.3.2/ptal_api/pretty_adapter/object_types.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/pretty_adapter/objects.py` & `ptal_api-0.12.3.2/ptal_api/pretty_adapter/objects.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/pretty_adapter/pretty_adapter.py` & `ptal_api-0.12.3.2/ptal_api/pretty_adapter/pretty_adapter.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/pretty_adapter/property_values.py` & `ptal_api-0.12.3.2/ptal_api/pretty_adapter/property_values.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/pretty_adapter/transformer.py` & `ptal_api-0.12.3.2/ptal_api/pretty_adapter/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import wraps
 from types import GeneratorType
 from typing import Any, Callable, List, Optional, Union
 
 from ptal_api.core.values.date_dataclass import PartialDateValue
 from ptal_api.core.values.value_mapping import (
     COMPOSITE_VALUE,
-    DATE_TIME_VALUE,
+    DATE_VALUE,
     DOUBLE_VALUE,
     INT_VALUE,
     LINK_VALUE,
     STRING_VALUE,
     get_map_helper,
 )
 from ptal_api.pretty_adapter.object_types import (
@@ -57,36 +57,35 @@
 
     @staticmethod
     def value_to_schema_value_type(value) -> str:
         if isinstance(value, str):
             return STRING_VALUE
         if isinstance(value, int):
             return INT_VALUE
-        if isinstance(value, DateTime):
-            return DATE_TIME_VALUE
+        if isinstance(value, (Date, DateTime)):
+            return DATE_VALUE
         if isinstance(value, LinkValue):
             return LINK_VALUE
         if isinstance(value, float):
             return DOUBLE_VALUE
         if isinstance(value, dict):
             return COMPOSITE_VALUE
         raise NotImplementedError(f"Type {type(value)} is not supported")
 
     @staticmethod
-    def value_schema_to_value(value_schema) -> Value:
-        value_type: str = value_schema.__typename__
+    def value_schema_to_value(value_schema: Any, value_type: str) -> Value:
         if value_type == STRING_VALUE:
             return str(value_schema.value)
         if value_type == INT_VALUE:
             return int(value_schema.number)
         if value_type == LINK_VALUE:
             return LinkValue(link=value_schema.link)
         if value_type == DOUBLE_VALUE:
             return float(value_schema.value.double)
-        if value_type == DATE_TIME_VALUE:
+        if value_type == DATE_VALUE:
             date_value = value_schema.date
             time_value = getattr(value_schema, "time", None)
             time_input = (
                 Time(hour=time_value.hour, minute=time_value.minute, second=time_value.second) if time_value else None
             )
             return DateTime(
                 date=Date(
@@ -100,15 +99,15 @@
             return {
                 ComponentValueType(
                     id=nv.id,
                     name=nv.property_value_type.name,
                     value_type=Transformer.base_value_type_schema_to_base_value_type(nv.property_value_type.value_type),
                     system_registration_date=getattr(nv, "system_registration_date", None),
                     system_update_date=getattr(nv, "system_update_date", None),
-                ): Transformer.value_schema_to_value(nv.value)
+                ): Transformer.value_schema_to_value(nv.value, nv.property_value_type.value_type.value_type)
                 for nv in value_schema.list_value
             }
         raise NotImplementedError(f"not implemented value type {value_type}")
 
     @staticmethod
     def pretty_value_to_adapter_value(value: Value) -> Any:
         adapter_value = value
@@ -148,35 +147,39 @@
 
     @staticmethod
     def property_schema_to_property(
         property_schema: api_schema.ConceptProperty,
         property_type_code: Optional[str] = None,
         object_from: Union[Concept, Link, None] = None,
     ) -> Property:
+        prop_type = Transformer.property_type_schema_to_property_type(property_schema.property_type, property_type_code)
+        if isinstance(prop_type.value_type, CompositeValueType):
+            value_type = COMPOSITE_VALUE
+        else:
+            value_type = property_schema.property_type.value_type.value_type
         return Property(
             id=property_schema.id,
-            type=Transformer.property_type_schema_to_property_type(property_schema.property_type, property_type_code),
-            value=Transformer.value_schema_to_value(property_schema.value),
+            type=prop_type,
+            value=Transformer.value_schema_to_value(property_schema.value, value_type),
             object_from=object_from,
             is_main=property_schema.is_main,
             system_registration_date=property_schema.system_registration_date,
             system_update_date=getattr(property_schema, "system_update_date", None),
             access_level=Transformer.access_level_schema_to_access_level(property_schema.access_level),
         )
 
     @staticmethod
     def base_value_type_schema_to_base_value_type(
         value_type_schema: api_schema.ConceptPropertyValueType, type_code: Optional[str] = None
     ) -> BaseValueType:
-        value_type = getattr(value_type_schema, "value_type", None)
         return BaseValueType(
             id=value_type_schema.id,
             name=value_type_schema.name,
             code=type_code,
-            value_type=value_type if isinstance(value_type, str) else None,
+            value_type=value_type_schema.value_type,
             system_registration_date=getattr(value_type_schema, "system_registration_date", None),
             system_update_date=getattr(value_type_schema, "system_update_date", None),
         )
 
     @staticmethod
     def composite_value_type_schema_to_composite_value_type(
         value_type_schema: api_schema.CompositePropertyValueTemplate, type_code: Optional[str] = None
```

### Comparing `ptal_api-0.12.3.1/ptal_api/providers/gql_providers.py` & `ptal_api-0.12.3.2/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/schema/README.md` & `ptal_api-0.12.3.2/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/schema/api_schema.py` & `ptal_api-0.12.3.2/ptal_api/schema/api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.12.3.2/ptal_api/schema/crawlers_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.12.3.2/ptal_api/schema/tcontroller_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.12.3.2/ptal_api/schema/utils_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/scripts/type_mapper.py` & `ptal_api-0.12.3.2/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.12.3.2/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.3.1/pyproject.toml` & `ptal_api-0.12.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.12.3.1"
+version = "0.12.3.2"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
```

### Comparing `ptal_api-0.12.3.1/PKG-INFO` & `ptal_api-0.12.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.12.3.1
+Version: 0.12.3.2
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

