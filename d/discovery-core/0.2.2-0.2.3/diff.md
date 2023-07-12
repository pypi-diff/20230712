# Comparing `tmp/discovery-core-0.2.2.tar.gz` & `tmp/discovery-core-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.2.2.tar", last modified: Wed Jul 12 21:02:38 2023, max compression
+gzip compressed data, was "discovery-core-0.2.3.tar", last modified: Wed Jul 12 21:09:50 2023, max compression
```

## Comparing `discovery-core-0.2.2.tar` & `discovery-core-0.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.734677 discovery-core-0.2.2/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.2/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.2/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 21:02:38.734875 discovery-core-0.2.2/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.2/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.721680 discovery-core-0.2.2/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 21:02:38.000000 discovery-core-0.2.2/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-12 21:02:38.000000 discovery-core-0.2.2/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-12 21:02:38.000000 discovery-core-0.2.2/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-12 21:02:38.000000 discovery-core-0.2.2/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.722265 discovery-core-0.2.2/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-12 13:48:57.000000 discovery-core-0.2.2/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.723856 discovery-core-0.2.2/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.2/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21096 2023-07-12 20:57:17.000000 discovery-core-0.2.2/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.725152 discovery-core-0.2.2/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.2/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.2/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.726245 discovery-core-0.2.2/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.2/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.728496 discovery-core-0.2.2/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.2/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.2/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.2/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-12 21:02:38.736203 discovery-core-0.2.2/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.2/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.728894 discovery-core-0.2.2/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.2/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.730302 discovery-core-0.2.2/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.2/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14057 2023-07-12 21:00:25.000000 discovery-core-0.2.2/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.731675 discovery-core-0.2.2/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.2/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.2/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.732972 discovery-core-0.2.2/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.2/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.2/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:02:38.734338 discovery-core-0.2.2/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.2/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.2/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.2/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.396818 discovery-core-0.2.3/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.3/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.3/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 21:09:50.397028 discovery-core-0.2.3/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.3/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.378588 discovery-core-0.2.3/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 21:09:50.000000 discovery-core-0.2.3/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-12 21:09:50.000000 discovery-core-0.2.3/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-12 21:09:50.000000 discovery-core-0.2.3/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-12 21:09:50.000000 discovery-core-0.2.3/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.378943 discovery-core-0.2.3/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-12 21:03:05.000000 discovery-core-0.2.3/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.381288 discovery-core-0.2.3/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.3/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21096 2023-07-12 21:06:16.000000 discovery-core-0.2.3/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.383422 discovery-core-0.2.3/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.3/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.3/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.384462 discovery-core-0.2.3/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.3/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.387719 discovery-core-0.2.3/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.3/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.3/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.3/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-12 21:09:50.397651 discovery-core-0.2.3/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.3/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.388725 discovery-core-0.2.3/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.3/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.390466 discovery-core-0.2.3/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.3/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14057 2023-07-12 21:07:34.000000 discovery-core-0.2.3/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.391867 discovery-core-0.2.3/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.3/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.3/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.393811 discovery-core-0.2.3/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.3/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.3/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.395956 discovery-core-0.2.3/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.3/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.3/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.2.2/LICENSE.txt` & `discovery-core-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/PKG-INFO` & `discovery-core-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.2/README.rst` & `discovery-core-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.2.3/discovery_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.2/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.2.3/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/ds_core/components/abstract_component.py` & `discovery-core-0.2.3/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/ds_core/components/core_commons.py` & `discovery-core-0.2.3/ds_core/components/core_commons.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         while working:
             working = False
             for idx in range(len(t.column_names)):
                 c = t.column_names[idx]
                 record = t.column(c).combine_chunks()
                 if pa.types.is_list(record.type):
                     for i in range(pc.min(pc.list_value_length(record)).as_py()):
-                        t = t.append_column(f'{c}_{i}', pc.list_element(t.column(c), i).combine_chunks())
+                        t = t.append_column(f'{c}.{i}', pc.list_element(t.column(c), i).combine_chunks())
                     t = t.drop_columns(c)
                     working = True
                 if pa.types.is_struct(record.type):
                     t = t.flatten()
                     working = True
         return t
```

### Comparing `discovery-core-0.2.2/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.2.3/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.2.3/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/ds_core/intent/abstract_intent.py` & `discovery-core-0.2.3/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/ds_core/properties/abstract_properties.py` & `discovery-core-0.2.3/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/ds_core/properties/decorator_patterns.py` & `discovery-core-0.2.3/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/ds_core/properties/property_manager.py` & `discovery-core-0.2.3/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/setup.py` & `discovery-core-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/test/components/abstract_component_test.py` & `discovery-core-0.2.3/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/test/components/commons_test.py` & `discovery-core-0.2.3/test/components/commons_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,17 @@
              "productId": ["PR716796"],
              }
         ]
         tbl = pa.Table.from_pylist(document)
         result = CoreCommons.table_flatten(tbl)
         control = ['_id',
                    'interactionDate.endDateTime', 'interactionDate.startDateTime',
-                   'relatedParty_0._id', 'relatedParty_0.engagedParty.referredType', 'relatedParty_0.role',
-                   'relatedParty_1._id', 'relatedParty_1.engagedParty.referredType', 'relatedParty_1.role',
-                   'productId_0']
+                   'relatedParty.0._id', 'relatedParty.0.engagedParty.referredType', 'relatedParty.0.role',
+                   'relatedParty.1._id', 'relatedParty.1.engagedParty.referredType', 'relatedParty.1.role',
+                   'productId.0']
         self.assertEqual(control, result.column_names)
 
     def test_array_cast(self):
         num = pa.array([1.0, 12.0, 5.0, None], pa.float64())
         date = pa.array(["2023-01-02 04:49:06", "2023-01-02 04:57:12", None, "2023-01-02 05:23:50"], pa.string())
         text = pa.array(["Blue", "Green", None, 'Blue'], pa.string())
         bool1 = pa.array([1, 0, 1, None], pa.int64())
```

### Comparing `discovery-core-0.2.2/test/handlers/connector_contract_test.py` & `discovery-core-0.2.3/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/test/handlers/handler_factory_test.py` & `discovery-core-0.2.3/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/test/intent/abstract_intent_test.py` & `discovery-core-0.2.3/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/test/intent/pyarrow_intent_model.py` & `discovery-core-0.2.3/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.2.3/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.2/test/properties/property_manager_test.py` & `discovery-core-0.2.3/test/properties/property_manager_test.py`

 * *Files identical despite different names*

