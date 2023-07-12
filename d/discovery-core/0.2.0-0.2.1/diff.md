# Comparing `tmp/discovery-core-0.2.0.tar.gz` & `tmp/discovery-core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.2.0.tar", last modified: Tue Jul 11 23:26:56 2023, max compression
+gzip compressed data, was "discovery-core-0.2.1.tar", last modified: Wed Jul 12 13:48:12 2023, max compression
```

## Comparing `discovery-core-0.2.0.tar` & `discovery-core-0.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.693702 discovery-core-0.2.0/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.0/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.0/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-11 23:26:56.693917 discovery-core-0.2.0/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.0/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.670216 discovery-core-0.2.0/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-11 23:26:56.000000 discovery-core-0.2.0/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-11 23:26:56.000000 discovery-core-0.2.0/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-11 23:26:56.000000 discovery-core-0.2.0/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-11 23:26:56.000000 discovery-core-0.2.0/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.670558 discovery-core-0.2.0/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-11 23:26:36.000000 discovery-core-0.2.0/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.673351 discovery-core-0.2.0/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.0/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.0/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20927 2023-07-11 23:16:51.000000 discovery-core-0.2.0/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.676782 discovery-core-0.2.0/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.0/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.0/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.0/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.678041 discovery-core-0.2.0/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.0/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.0/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.682786 discovery-core-0.2.0/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.0/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.0/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.0/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.0/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-11 23:26:56.694619 discovery-core-0.2.0/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.0/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.683978 discovery-core-0.2.0/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.0/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.686197 discovery-core-0.2.0/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.0/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.0/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11890 2023-07-11 23:26:07.000000 discovery-core-0.2.0/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.688535 discovery-core-0.2.0/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.0/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.0/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.0/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.690542 discovery-core-0.2.0/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.0/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3039 2023-06-29 16:24:13.000000 discovery-core-0.2.0/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7688 2023-06-29 23:15:54.000000 discovery-core-0.2.0/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-11 23:26:56.692884 discovery-core-0.2.0/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.0/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.0/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.0/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.902934 discovery-core-0.2.1/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.1/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.1/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 13:48:12.903206 discovery-core-0.2.1/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.1/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.882124 discovery-core-0.2.1/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 13:48:12.000000 discovery-core-0.2.1/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-12 13:48:12.000000 discovery-core-0.2.1/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-12 13:48:12.000000 discovery-core-0.2.1/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-12 13:48:12.000000 discovery-core-0.2.1/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.882717 discovery-core-0.2.1/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-11 23:27:34.000000 discovery-core-0.2.1/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.885968 discovery-core-0.2.1/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.1/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21031 2023-07-12 13:35:41.000000 discovery-core-0.2.1/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.888820 discovery-core-0.2.1/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.1/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.1/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.890429 discovery-core-0.2.1/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.1/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.894151 discovery-core-0.2.1/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.1/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.1/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.1/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-12 13:48:12.904032 discovery-core-0.2.1/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.1/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.895121 discovery-core-0.2.1/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.1/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.896748 discovery-core-0.2.1/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.1/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12105 2023-07-12 13:45:09.000000 discovery-core-0.2.1/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.898217 discovery-core-0.2.1/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.1/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.1/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.899598 discovery-core-0.2.1/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2962 2023-07-12 13:39:52.000000 discovery-core-0.2.1/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7688 2023-06-29 23:15:54.000000 discovery-core-0.2.1/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 13:48:12.902191 discovery-core-0.2.1/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.1/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.1/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.1/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.2.0/LICENSE.txt` & `discovery-core-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/PKG-INFO` & `discovery-core-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.0/README.rst` & `discovery-core-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.2.1/discovery_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.0/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.2.1/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/ds_core/components/abstract_component.py` & `discovery-core-0.2.1/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/ds_core/components/core_commons.py` & `discovery-core-0.2.1/ds_core/components/core_commons.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,14 +301,16 @@
         """ attempt to cast a pyarrow table columns to the given type """
         cat_max = cat_max if isinstance(cat_max, int) else 40
         rtn_tbl = None
         for n in t.column_names:
             c = t.combine_chunks().column(n)
             if pa.types.is_string(c.type):
                 c = CoreCommons.column_cast(c, pa.timestamp('ns'))
+            if pa.types.is_string(c.type):
+                c = CoreCommons.column_cast(c, pa.float64())
             if pa.types.is_floating(c.type):
                 c = CoreCommons.column_cast(c, pa.int64())
             if pa.types.is_integer(c.type) and c.drop_null().unique().sort().equals(pa.array([0, 1])):
                 c = CoreCommons.column_cast(c, pa.bool_())
             if pa.types.is_string(c.type) and pc.count_distinct(c.drop_null()).equals(pa.scalar(2)):
                 c = CoreCommons.column_cast(c, pa.bool_())
             if pa.types.is_string(c.type) and 1 <= pc.count_distinct(c.drop_null()).as_py() <= cat_max:
```

### Comparing `discovery-core-0.2.0/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.2.1/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.2.1/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/ds_core/intent/abstract_intent.py` & `discovery-core-0.2.1/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/ds_core/properties/abstract_properties.py` & `discovery-core-0.2.1/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/ds_core/properties/decorator_patterns.py` & `discovery-core-0.2.1/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/ds_core/properties/property_manager.py` & `discovery-core-0.2.1/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/setup.py` & `discovery-core-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/test/components/abstract_component_test.py` & `discovery-core-0.2.1/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/test/components/commons_test.py` & `discovery-core-0.2.1/test/components/commons_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,31 +83,36 @@
         self.assertEqual(pa.string(), CoreCommons.column_cast(text, pa.string()).type)
         self.assertEqual(pa.bool_(), CoreCommons.column_cast(bool1, pa.bool_()).type)
         self.assertEqual(pa.bool_(), CoreCommons.column_cast(bool2, pa.bool_()).type)
         self.assertEqual(pa.string(), CoreCommons.column_cast(bool3, pa.bool_()).type)
 
     def test_table_cast(self):
         num = pa.array([1.0, 12.0, 5.0, None], pa.float64())
+
         date = pa.array(["2023-01-02 04:49:06", "2023-01-02 04:57:12", None, "2023-01-02 05:23:50"], pa.string())
+        value = pa.array([None, '1.5', '3.2', '2.0'], pa.string())
         text = pa.array(["Blue", "Green", None, 'Red'], pa.string())
         bool1 = pa.array([1, 0, 1, None], pa.int64())
         bool2 = pa.array(['true', 'true', None, 'false'], pa.string())
         bool3 = pa.array([None, 'M', 'F', 'M'], pa.string())
-        tbl = pa.table([num, date, text, bool1, bool2, bool3], names=['num', 'date', 'text', 'bool1', 'bool2', 'bool3'])
+        tbl = pa.table([num, value, date, text, bool1, bool2, bool3],
+                       names=['num', 'value', 'date', 'text', 'bool1', 'bool2', 'bool3'])
         result = CoreCommons.table_cast(tbl).combine_chunks()
         control = pa.schema([('num', pa.int64()),
+                             ('value', pa.float64()),
                              ('date', pa.timestamp('ns')),
                              ('text', pa.dictionary(pa.int32(), pa.string())),
                              ('bool1', pa.bool_()),
                              ('bool2', pa.bool_()),
                              ('bool3', pa.dictionary(pa.int32(), pa.string())),
                              ])
         self.assertEqual(control, result.schema)
         result = CoreCommons.table_cast(tbl, cat_max=2).combine_chunks()
         control = pa.schema([('num', pa.int64()),
+                             ('value', pa.float64()),
                              ('date', pa.timestamp('ns')),
                              ('text', pa.string()),
                              ('bool1', pa.bool_()),
                              ('bool2', pa.bool_()),
                              ('bool3', pa.dictionary(pa.int32(), pa.string())),
                              ])
         self.assertEqual(control, result.schema)
```

### Comparing `discovery-core-0.2.0/test/handlers/connector_contract_test.py` & `discovery-core-0.2.1/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/test/handlers/handler_factory_test.py` & `discovery-core-0.2.1/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/test/intent/abstract_intent_test.py` & `discovery-core-0.2.1/test/intent/abstract_intent_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
 import os
 import shutil
 
 from ds_core.handlers.abstract_handlers import ConnectorContract
-from ds_core.intent.python_cleaners_intent import PyarrowCleanersIntentModel
 from ds_core.properties.abstract_properties import AbstractPropertyManager
 from ds_core.properties.property_manager import PropertyManager
 
 
 class ControlPropertyManager(AbstractPropertyManager):
 
     def __init__(self, task_name: str, creator: str=None):
```

### Comparing `discovery-core-0.2.0/test/intent/pyarrow_intent_model.py` & `discovery-core-0.2.1/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.2.1/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.0/test/properties/property_manager_test.py` & `discovery-core-0.2.1/test/properties/property_manager_test.py`

 * *Files identical despite different names*

