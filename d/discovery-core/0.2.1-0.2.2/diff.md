# Comparing `tmp/discovery-core-0.2.1.tar.gz` & `tmp/discovery-core-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.2.1.tar", last modified: Wed Jul 12 13:48:12 2023, max compression
+gzip compressed data, was "discovery-core-0.2.2.tar", last modified: Wed Jul 12 21:02:38 2023, max compression
```

## Comparing `discovery-core-0.2.1.tar` & `discovery-core-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.902934 discovery-core-0.2.1/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.1/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.1/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 13:48:12.903206 discovery-core-0.2.1/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.1/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.882124 discovery-core-0.2.1/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 13:48:12.000000 discovery-core-0.2.1/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-12 13:48:12.000000 discovery-core-0.2.1/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-12 13:48:12.000000 discovery-core-0.2.1/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-12 13:48:12.000000 discovery-core-0.2.1/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.882717 discovery-core-0.2.1/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-11 23:27:34.000000 discovery-core-0.2.1/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.885968 discovery-core-0.2.1/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.1/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21031 2023-07-12 13:35:41.000000 discovery-core-0.2.1/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.888820 discovery-core-0.2.1/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.1/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.1/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.890429 discovery-core-0.2.1/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.1/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.894151 discovery-core-0.2.1/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.1/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.1/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.1/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-12 13:48:12.904032 discovery-core-0.2.1/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.1/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.895121 discovery-core-0.2.1/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.1/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.896748 discovery-core-0.2.1/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.1/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12105 2023-07-12 13:45:09.000000 discovery-core-0.2.1/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.898217 discovery-core-0.2.1/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.1/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.1/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.899598 discovery-core-0.2.1/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2962 2023-07-12 13:39:52.000000 discovery-core-0.2.1/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7688 2023-06-29 23:15:54.000000 discovery-core-0.2.1/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.902191 discovery-core-0.2.1/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.1/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.1/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.734677 discovery-core-0.2.2/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.2/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.2/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 21:02:38.734875 discovery-core-0.2.2/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.2/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.721680 discovery-core-0.2.2/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 21:02:38.000000 discovery-core-0.2.2/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-12 21:02:38.000000 discovery-core-0.2.2/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-12 21:02:38.000000 discovery-core-0.2.2/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-12 21:02:38.000000 discovery-core-0.2.2/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.722265 discovery-core-0.2.2/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-12 13:48:57.000000 discovery-core-0.2.2/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.723856 discovery-core-0.2.2/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.2/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21096 2023-07-12 20:57:17.000000 discovery-core-0.2.2/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.725152 discovery-core-0.2.2/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.2/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.2/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.726245 discovery-core-0.2.2/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.2/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.728496 discovery-core-0.2.2/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.2/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.2/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.2/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-12 21:02:38.736203 discovery-core-0.2.2/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.2/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.728894 discovery-core-0.2.2/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.2/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.730302 discovery-core-0.2.2/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.2/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14057 2023-07-12 21:00:25.000000 discovery-core-0.2.2/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.731675 discovery-core-0.2.2/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.2/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.2/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.732972 discovery-core-0.2.2/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.2/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.2/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.734338 discovery-core-0.2.2/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.2/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.2/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.2.1/LICENSE.txt` & `discovery-core-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/PKG-INFO` & `discovery-core-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.1/README.rst` & `discovery-core-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.2.2/discovery_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.1/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.2.2/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/ds_core/components/abstract_component.py` & `discovery-core-0.2.2/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/ds_core/components/core_commons.py` & `discovery-core-0.2.2/ds_core/components/core_commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,53 +210,55 @@
         precision = precision if isinstance(precision, int) else 5
         seq_min = min(seq)
         seq_range = max(seq) - seq_min
         n_range = (b - a)
         return [round((n_range * ((x - seq_min) / seq_range)) + a, precision) for x in seq]
 
     @staticmethod
-    def filter_headers(data: pa.Table, headers: [str, list]=None, drop: bool=None, regex: [str, list]=None) -> list:
+    def filter_headers(data: pa.Table, headers: [str, list]=None, d_type: pa.DataType=None, drop: bool=None,
+                       regex: [str, list]=None) -> list:
         """ returns a list of headers based on the filter criteria
 
         :param data: the Canonical data to get the column headers from
         :param headers: a list of headers to drop or filter on type
-        :param drop: to drop or not drop the headers
+        :param d_type: a li
+        :param drop: to drop or not drop the selection
         :param regex: a regular expression to search the headers
         :return: a filtered list of headers
 
         :raise: TypeError if any of the types are not as expected
         """
-        if drop is None or not isinstance(drop, bool):
-            drop = False
-
         if not isinstance(data, pa.Table):
             raise TypeError("The first function attribute must be a pa.Table")
-        _headers = CoreCommons.list_formatter(headers)
+        drop = drop if isinstance(drop, bool) else False
+        headers = CoreCommons.list_formatter(headers)
         regex = '|'.join(CoreCommons.list_formatter(regex))
-        _obj_cols = data.column_names
 
-        if _headers is not None and _headers:
-            result = pc.is_in(data.column_names, pa.array(_headers))
-            return pa.array(data.column_names).filter(result)
+        rtn_list = data.column_names
+        if headers is not None and headers:
+            _ = pc.is_in(rtn_list, pa.array(headers))
+            rtn_list = pa.array(rtn_list).filter(_).to_pylist()
         if regex is not None and regex:
-            result = pc.extract_regex(data.column_names, regex).is_valid()
-            return pa.array(data.column_names).filter(result)
+            _ = pc.extract_regex(rtn_list, regex).is_valid()
+            rtn_list = pa.array(rtn_list).filter(_).to_pylist()
+        if drop:
+            return CoreCommons.list_diff(data.column_names, rtn_list)
+        return rtn_list
 
     @staticmethod
     def filter_columns(data: pa.Table, headers=None, drop: bool=None, regex: [str, list]=None) -> pa.Table:
         """ Returns a subset of columns based on the filter criteria
 
         :param data: the Canonical data to get the column headers from
         :param headers: a list of headers to drop or filter on type
         :param drop: to drop or not drop the headers
         :param regex: a regular expression to search the headers
         :return:
         """
-        result = CoreCommons.filter_headers(data=data, headers=headers, drop=drop, regex=regex)
-        return data.drop_columns(CoreCommons.list_diff(data.column_names, result))
+        return data.select(CoreCommons.filter_headers(data=data, headers=headers, drop=drop, regex=regex))
 
     @staticmethod
     def table_append(t1: pa.Table, t2: pa.Table):
         """ appends all the columns in t2 to t1 """
         if not isinstance(t2, pa.Table):
             raise ValueError("As a minimum, the second value passed must be a PyArrow Table")
         if not isinstance(t1, pa.Table):
```

### Comparing `discovery-core-0.2.1/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.2.2/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.2.2/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/ds_core/intent/abstract_intent.py` & `discovery-core-0.2.2/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/ds_core/properties/abstract_properties.py` & `discovery-core-0.2.2/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/ds_core/properties/decorator_patterns.py` & `discovery-core-0.2.2/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/ds_core/properties/property_manager.py` & `discovery-core-0.2.2/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/setup.py` & `discovery-core-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/test/components/abstract_component_test.py` & `discovery-core-0.2.2/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/test/components/commons_test.py` & `discovery-core-0.2.2/test/components/commons_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         self.assertEqual(pa.string(), CoreCommons.column_cast(text, pa.string()).type)
         self.assertEqual(pa.bool_(), CoreCommons.column_cast(bool1, pa.bool_()).type)
         self.assertEqual(pa.bool_(), CoreCommons.column_cast(bool2, pa.bool_()).type)
         self.assertEqual(pa.string(), CoreCommons.column_cast(bool3, pa.bool_()).type)
 
     def test_table_cast(self):
         num = pa.array([1.0, 12.0, 5.0, None], pa.float64())
-
         date = pa.array(["2023-01-02 04:49:06", "2023-01-02 04:57:12", None, "2023-01-02 05:23:50"], pa.string())
         value = pa.array([None, '1.5', '3.2', '2.0'], pa.string())
         text = pa.array(["Blue", "Green", None, 'Red'], pa.string())
         bool1 = pa.array([1, 0, 1, None], pa.int64())
         bool2 = pa.array(['true', 'true', None, 'false'], pa.string())
         bool3 = pa.array([None, 'M', 'F', 'M'], pa.string())
         tbl = pa.table([num, value, date, text, bool1, bool2, bool3],
@@ -113,15 +112,43 @@
                              ('text', pa.string()),
                              ('bool1', pa.bool_()),
                              ('bool2', pa.bool_()),
                              ('bool3', pa.dictionary(pa.int32(), pa.string())),
                              ])
         self.assertEqual(control, result.schema)
 
+    def test_filter_headers(self):
+        num = pa.array([1.0, 12.0, 5.0, None], pa.float64())
+        date = pa.array(["2023-01-02 04:49:06", "2023-01-02 04:57:12", None, "2023-01-02 05:23:50"], pa.string())
+        value = pa.array([None, '1.5', '3.2', '2.0'], pa.string())
+        text = pa.array(["Blue", "Green", None, 'Red'], pa.string())
+        bool1 = pa.array([1, 0, 1, None], pa.int64())
+        bool2 = pa.array(['true', 'true', None, 'false'], pa.string())
+        cat = pa.array([None, 'M', 'F', 'M'], pa.string())
+        tbl = pa.table([num, value, date, text, bool1, bool2, cat],
+                       names=['num', 'value', 'date', 'text', 'bool1', 'bool2', 'cat'])
+        result = CoreCommons.filter_headers(tbl)
+        self.assertEqual(tbl.column_names, result)
+        result = CoreCommons.filter_headers(tbl, headers=['num', 'value', 'text'])
+        self.assertCountEqual(['num', 'value', 'text'], result)
+        result = CoreCommons.filter_headers(tbl, regex=['t', 'value'])
+        self.assertCountEqual(['value', 'date', 'text', 'cat'], result)
+        result = CoreCommons.filter_headers(tbl, regex=['t', 'value'], drop=True)
+        self.assertCountEqual(['bool1', 'bool2', 'num'], result)
+        result = CoreCommons.filter_headers(tbl, headers=['value', 'text', 'bool1'], regex='e')
+        self.assertCountEqual(['value', 'text'], result)
 
+    def test_filter_columns(self):
+        num = pa.array([1.0, 12.0, 5.0, None], pa.float64())
+        date = pa.array(["2023-01-02 04:49:06", "2023-01-02 04:57:12", None, "2023-01-02 05:23:50"], pa.string())
+        value = pa.array([None, '1.5', '3.2', '2.0'], pa.string())
+        text = pa.array(["Blue", "Green", None, 'Red'], pa.string())
+        tbl = pa.table([num, value, date, text], names=['num', 'value', 'date', 'text'])
+        result = CoreCommons.filter_columns(tbl, headers=['num', 'date'])
+        self.assertCountEqual(['num', 'date'], result.column_names)
 
     def test_list_formatter(self):
         sample = {'A': [1,2], 'B': [1,2], 'C': [1,2]}
         result = CoreCommons.list_formatter(sample)
         self.assertEqual(list("ABC"), result)
         result = CoreCommons.list_formatter(sample.keys())
         self.assertEqual(list("ABC"), result)
```

### Comparing `discovery-core-0.2.1/test/handlers/connector_contract_test.py` & `discovery-core-0.2.2/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/test/handlers/handler_factory_test.py` & `discovery-core-0.2.2/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/test/intent/abstract_intent_test.py` & `discovery-core-0.2.2/test/intent/abstract_intent_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import os
 import shutil
 
 from ds_core.handlers.abstract_handlers import ConnectorContract
 from ds_core.properties.abstract_properties import AbstractPropertyManager
 from ds_core.properties.property_manager import PropertyManager
 
+from test.intent.pyarrow_intent_model import PyarrowIntentModel
+
 
 class ControlPropertyManager(AbstractPropertyManager):
 
     def __init__(self, task_name: str, creator: str=None):
         # set additional keys
         root_keys = []
         knowledge_keys = []
@@ -20,15 +22,15 @@
     def manager_name(cls) -> str:
         return str(cls.__name__).lower().replace('propertymanager', '')
 
 
 class IntentModelTest(unittest.TestCase):
 
     def setUp(self):
-        self.connector = ConnectorContract(uri='contracts/config_contract.pkl?sep=.&encoding=Latin1',
+        self.connector = ConnectorContract(uri='contracts/config_contract.pq?sep=.&encoding=Latin1',
                                            module_name='ds_core.handlers.pyarrow_handlers',
                                            handler='PyarrowPersistHandler')
         try:
             os.makedirs('contracts')
         except:
             pass
         PropertyManager._remove_all()
@@ -39,28 +41,27 @@
         try:
             shutil.rmtree('contracts')
         except:
             pass
 
     def test_runs(self):
         """Basic smoke test"""
-        PyarrowCleanersIntentModel(property_manager=self.pm)
+        PyarrowIntentModel(property_manager=self.pm)
 
     def test_run_intent_pipeline(self):
-        model = PyarrowCleanersIntentModel(property_manager=self.pm)
+        model = PyarrowIntentModel(property_manager=self.pm)
         canonical = {'A': [1,4,7], 'B': [4,5,9]}
         result = model.run_intent_pipeline(canonical=canonical, inplace=False)
         self.assertDictEqual(canonical, result)
-        model.to_remove(data=canonical, headers=['B'], inplace=True)
-        model.auto_clean_header(data=canonical, case='lower', inplace=True)
-        result = model.run_intent_pipeline(canonical=canonical, inplace=False)
+        model.to_str_type(data=canonical, headers=['B'])
+        result = model.run_intent_pipeline(canonical=canonical)
         self.assertDictEqual({'a': [1, 4, 7]}, result)
 
     def test_run_intent_pipeline_levels(self):
-        model = PyarrowCleanersIntentModel(property_manager=self.pm)
+        model = PyarrowIntentModel(property_manager=self.pm)
         data = {'A': [1,4,7], 'B': [4,5,9]}
         model.to_remove(data=data, headers=['B'], inplace=False, intent_level=0)
         model.auto_clean_header(data=data, case='lower', inplace=False, intent_level=1)
         result = model.run_intent_pipeline(canonical=data, inplace=False, intent_levels=0)
         self.assertDictEqual({'A': [1, 4, 7]}, result)
         result = model.run_intent_pipeline(canonical=data, inplace=False, intent_levels=1)
         self.assertDictEqual({'a': [1,4,7], 'b': [4,5,9]}, result)
```

### Comparing `discovery-core-0.2.1/test/intent/pyarrow_intent_model.py` & `discovery-core-0.2.2/test/intent/pyarrow_intent_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,31 +70,27 @@
                         _ = params.pop('intent_creator', 'default')
                         # add excluded parameters to the params
                         params.update({'inplace': False, 'save_intent': False})
                         canonical = eval(f"self.{method}(canonical, **{params})", globals(), locals())
         if not inplace:
             return canonical
 
-    def to_str_type(self, data: pa.Table, headers: [str, list]=None, drop: bool=False, dtype: [str, list]=None,
-                    exclude: bool=False, regex: [str, list]=None, re_ignore_case: bool=True,
-                    nulls_list: [bool, list]=None, save_intent: bool=None, intent_level: [int, str]=None,
-                    intent_order: int=None, replace_intent: bool=None, remove_duplicates: bool=None) -> pa.Table:
+    def to_remove(self, data: pa.Table, headers: [str, list]=None, drop: bool=False, d_type: [str, list]=None,
+                  exclude: bool=False, regex: [str, list]=None, re_ignore_case: bool=True, save_intent: bool=None,
+                  intent_level: [int, str]=None, intent_order: int=None, replace_intent: bool=None,
+                  remove_duplicates: bool=None) -> pa.Table:
         """ converts columns to object type
 
         :param data: the Canonical data to get the column headers from
         :param headers: a list of headers to drop or filter on type
         :param drop: to drop or not drop the headers
-        :param dtype: the column types to include or excluse. Default None else int, float, bool, object, 'number'
+        :param d_type: the column types to include or exclude. Default None else int, float, bool, object, 'number'
         :param exclude: to exclude or include the dtypes
-        :param regex: a regiar expression to seach the headers
+        :param regex: a regular expression to search the headers
         :param re_ignore_case: true if the regex should ignore case. Default is False
-        :param nulls_list: can be boolean or a list:
-                    if boolean and True then null_list equals ['NaN', 'nan', 'null', '', 'None']
-                    if list then this is considered potential null values.
-        :param inplace: if the passed Canonical, should be used or a deep copy
         :param save_intent (optional) if the intent contract should be saved to the property manager
         :param intent_level: (optional) the level name that groups intent by a reference name
         :param intent_order: (optional) the order in which each intent should run.
                         If None: default's to -1
                         if -1: added to a level above any current instance of the intent section, level 0 if not found
                         if int: added to the level specified, overwriting any that already exist
         :param replace_intent: (optional) if the intent method exists at the level, or default level
@@ -103,14 +99,10 @@
         :param remove_duplicates: (optional) removes any duplicate intent in any level that is identical
         :return: if inplace, returns a formatted cleaner contract for this method, else a deep copy Canonical,.
        """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
+        selection = CoreCommons.filter_headers(data, headers=headers, drop=drop, regex=regex)
 
-        selection = CoreCommons.filter_headers(data=data, headers=headers, drop=drop, d_type=dtype, exclude=exclude,
-                                               regex=regex, re_ignore_case=re_ignore_case)
-        for c in selection:
-            values = data.pop(c)
-            data[c] = [str(x) if x is not None else None for x in values]
         return data
```

### Comparing `discovery-core-0.2.1/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.2.2/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.1/test/properties/property_manager_test.py` & `discovery-core-0.2.2/test/properties/property_manager_test.py`

 * *Files identical despite different names*

