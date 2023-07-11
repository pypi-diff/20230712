# Comparing `tmp/discovery-core-0.1.5.tar.gz` & `tmp/discovery-core-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.1.5.tar", last modified: Mon Jul 10 15:36:17 2023, max compression
+gzip compressed data, was "discovery-core-0.1.6.tar", last modified: Tue Jul 11 23:19:20 2023, max compression
```

## Comparing `discovery-core-0.1.5.tar` & `discovery-core-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.796233 discovery-core-0.1.5/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.1.5/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.1.5/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-10 15:36:17.796667 discovery-core-0.1.5/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.1.5/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.772629 discovery-core-0.1.5/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-10 15:36:17.000000 discovery-core-0.1.5/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-10 15:36:17.000000 discovery-core-0.1.5/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-10 15:36:17.000000 discovery-core-0.1.5/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-10 15:36:17.000000 discovery-core-0.1.5/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.773048 discovery-core-0.1.5/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-09 15:09:33.000000 discovery-core-0.1.5/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.775601 discovery-core-0.1.5/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.5/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.1.5/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    19500 2023-07-09 14:21:43.000000 discovery-core-0.1.5/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.778550 discovery-core-0.1.5/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.5/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.1.5/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.1.5/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.779673 discovery-core-0.1.5/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.5/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.1.5/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.783532 discovery-core-0.1.5/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.5/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.1.5/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.1.5/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.1.5/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-10 15:36:17.798122 discovery-core-0.1.5/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.1.5/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.784751 discovery-core-0.1.5/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.1.5/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.787049 discovery-core-0.1.5/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.5/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.1.5/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9044 2023-07-09 23:08:44.000000 discovery-core-0.1.5/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.789406 discovery-core-0.1.5/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.5/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.1.5/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.1.5/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.791875 discovery-core-0.1.5/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.5/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3039 2023-06-29 16:24:13.000000 discovery-core-0.1.5/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7688 2023-06-29 23:15:54.000000 discovery-core-0.1.5/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:36:17.795156 discovery-core-0.1.5/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.5/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.1.5/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.1.5/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.089847 discovery-core-0.1.6/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.1.6/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.1.6/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-11 23:19:20.090074 discovery-core-0.1.6/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.1.6/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.069640 discovery-core-0.1.6/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-11 23:19:19.000000 discovery-core-0.1.6/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-11 23:19:19.000000 discovery-core-0.1.6/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-11 23:19:19.000000 discovery-core-0.1.6/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-11 23:19:19.000000 discovery-core-0.1.6/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.070007 discovery-core-0.1.6/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-10 23:30:59.000000 discovery-core-0.1.6/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.072589 discovery-core-0.1.6/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.6/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.1.6/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20927 2023-07-11 23:16:51.000000 discovery-core-0.1.6/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.074782 discovery-core-0.1.6/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.6/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.1.6/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.1.6/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.076291 discovery-core-0.1.6/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.6/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.1.6/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.080050 discovery-core-0.1.6/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.6/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.1.6/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.1.6/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.1.6/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-11 23:19:20.090963 discovery-core-0.1.6/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.1.6/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.081127 discovery-core-0.1.6/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.1.6/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.083312 discovery-core-0.1.6/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.6/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.1.6/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11391 2023-07-11 23:09:45.000000 discovery-core-0.1.6/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.084941 discovery-core-0.1.6/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.6/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.1.6/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.1.6/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.086565 discovery-core-0.1.6/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.6/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3039 2023-06-29 16:24:13.000000 discovery-core-0.1.6/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7688 2023-06-29 23:15:54.000000 discovery-core-0.1.6/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:19:20.089123 discovery-core-0.1.6/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.1.6/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.1.6/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.1.6/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.1.5/LICENSE.txt` & `discovery-core-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/PKG-INFO` & `discovery-core-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.1.5/README.rst` & `discovery-core-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.1.6/discovery_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.1.5/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.1.6/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/ds_core/components/abstract_component.py` & `discovery-core-0.1.6/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/ds_core/components/core_commons.py` & `discovery-core-0.1.6/ds_core/components/core_commons.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from collections import abc, Counter
 import math
 import re
 from datetime import datetime
 from typing import Any
 import pyarrow as pa
 import pyarrow.compute as pc
-__author__ = 'Darryl Oatridge'
-
+from pyarrow.lib import ArrowInvalid, ArrowTypeError, ArrowNotImplementedError
 
 class CoreCommons(object):
     """ common methods """
 
     @staticmethod
     def list_formatter(value: Any) -> list:
         """ Useful utility method to convert any type of str, list, tuple or pd.Series into a list"""
@@ -285,14 +284,42 @@
                     t = t.drop_columns(c)
                     working = True
                 if pa.types.is_struct(record.type):
                     t = t.flatten()
                     working = True
         return t
 
+    @staticmethod
+    def column_cast(a: pa.Array, ty: pa.DataType) -> pa.Array:
+        """ attempt to cast a pyarrow array to the given type """
+        try:
+            return a.cast(ty)
+        except (ArrowInvalid, ArrowTypeError, ArrowNotImplementedError):
+            return a
+
+    @staticmethod
+    def table_cast(t: pa.Table, cat_max: int=None):
+        """ attempt to cast a pyarrow table columns to the given type """
+        cat_max = cat_max if isinstance(cat_max, int) else 40
+        rtn_tbl = None
+        for n in t.column_names:
+            c = t.combine_chunks().column(n)
+            if pa.types.is_string(c.type):
+                c = CoreCommons.column_cast(c, pa.timestamp('ns'))
+            if pa.types.is_floating(c.type):
+                c = CoreCommons.column_cast(c, pa.int64())
+            if pa.types.is_integer(c.type) and c.drop_null().unique().sort().equals(pa.array([0, 1])):
+                c = CoreCommons.column_cast(c, pa.bool_())
+            if pa.types.is_string(c.type) and pc.count_distinct(c.drop_null()).equals(pa.scalar(2)):
+                c = CoreCommons.column_cast(c, pa.bool_())
+            if pa.types.is_string(c.type) and 1 <= pc.count_distinct(c.drop_null()).as_py() <= cat_max:
+                c = c.dictionary_encode()
+            rtn_tbl = CoreCommons.table_append(rtn_tbl, pa.table([c], names=[n]))
+        return rtn_tbl
+
 
 class AnalyticsSection(object):
     """A section  subset of the analytics"""
 
     _section = {}
 
     def __init__(self, section: dict):
```

### Comparing `discovery-core-0.1.5/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.1.6/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.1.6/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/ds_core/intent/abstract_intent.py` & `discovery-core-0.1.6/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/ds_core/properties/abstract_properties.py` & `discovery-core-0.1.6/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/ds_core/properties/decorator_patterns.py` & `discovery-core-0.1.6/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/ds_core/properties/property_manager.py` & `discovery-core-0.1.6/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/setup.py` & `discovery-core-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/test/components/abstract_component_test.py` & `discovery-core-0.1.6/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/test/handlers/connector_contract_test.py` & `discovery-core-0.1.6/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/test/handlers/handler_factory_test.py` & `discovery-core-0.1.6/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/test/intent/abstract_intent_test.py` & `discovery-core-0.1.6/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/test/intent/pyarrow_intent_model.py` & `discovery-core-0.1.6/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.1.6/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.1.5/test/properties/property_manager_test.py` & `discovery-core-0.1.6/test/properties/property_manager_test.py`

 * *Files identical despite different names*

