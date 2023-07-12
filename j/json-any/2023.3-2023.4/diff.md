# Comparing `tmp/json-any-2023.3.tar.gz` & `tmp/json-any-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-any-2023.3.tar", last modified: Wed Jul 12 11:37:56 2023, max compression
+gzip compressed data, was "json-any-2023.4.tar", last modified: Wed Jul 12 16:20:20 2023, max compression
```

## Comparing `json-any-2023.3.tar` & `json-any-2023.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 11:37:56.153664 json-any-2023.3/
--rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.3/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-12 11:37:56.150330 json-any-2023.3/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.3/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.3/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 11:37:56.146997 json-any-2023.3/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 11:37:56.150330 json-any-2023.3/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.3/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 11:37:56.150330 json-any-2023.3/json_any/
--rw-r--r--   0 eric      (1000) users      (984)     1754 2023-07-11 10:57:55.000000 json-any-2023.3/json_any/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 11:37:56.150330 json-any-2023.3/json_any/catalog/
--rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.3/json_any/catalog/module.py
--rw-r--r--   0 eric      (1000) users      (984)     2848 2023-07-11 10:24:57.000000 json-any-2023.3/json_any/catalog/type.py
--rw-r--r--   0 eric      (1000) users      (984)     2895 2023-07-11 10:56:35.000000 json-any-2023.3/json_any/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 11:37:56.150330 json-any-2023.3/json_any/extension/
--rw-r--r--   0 eric      (1000) users      (984)     6528 2023-07-11 09:47:11.000000 json-any-2023.3/json_any/extension/numpy.py
--rw-r--r--   0 eric      (1000) users      (984)     4259 2023-07-11 15:42:31.000000 json-any-2023.3/json_any/extension/type.py
--rw-r--r--   0 eric      (1000) users      (984)    11811 2023-07-12 11:12:25.000000 json-any-2023.3/json_any/json_to_object.py
--rw-r--r--   0 eric      (1000) users      (984)    13632 2023-07-12 11:25:58.000000 json-any-2023.3/json_any/object_to_json.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-12 11:36:11.000000 json-any-2023.3/json_any/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 11:37:56.150330 json-any-2023.3/json_any.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-12 11:37:56.000000 json-any-2023.3/json_any.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      461 2023-07-12 11:37:56.000000 json-any-2023.3/json_any.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-12 11:37:56.000000 json-any-2023.3/json_any.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-12 11:37:56.000000 json-any-2023.3/json_any.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.3/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-12 11:37:56.153664 json-any-2023.3/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5293 2023-07-11 12:01:48.000000 json-any-2023.3/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/
+-rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.4/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-12 16:20:20.027000 json-any-2023.4/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.4/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.4/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.023667 json-any-2023.4/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.4/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/json_any/
+-rw-r--r--   0 eric      (1000) users      (984)     1754 2023-07-11 10:57:55.000000 json-any-2023.4/json_any/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/json_any/catalog/
+-rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.4/json_any/catalog/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     2848 2023-07-11 10:24:57.000000 json-any-2023.4/json_any/catalog/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     2895 2023-07-11 10:56:35.000000 json-any-2023.4/json_any/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/json_any/extension/
+-rw-r--r--   0 eric      (1000) users      (984)     6528 2023-07-11 09:47:11.000000 json-any-2023.4/json_any/extension/numpy.py
+-rw-r--r--   0 eric      (1000) users      (984)     4259 2023-07-11 15:42:31.000000 json-any-2023.4/json_any/extension/type.py
+-rw-r--r--   0 eric      (1000) users      (984)    11674 2023-07-12 16:06:38.000000 json-any-2023.4/json_any/json_to_object.py
+-rw-r--r--   0 eric      (1000) users      (984)    13809 2023-07-12 16:07:02.000000 json-any-2023.4/json_any/object_to_json.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-12 16:17:18.000000 json-any-2023.4/json_any/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/json_any.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-12 16:20:20.000000 json-any-2023.4/json_any.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      461 2023-07-12 16:20:20.000000 json-any-2023.4/json_any.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-12 16:20:20.000000 json-any-2023.4/json_any.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-12 16:20:20.000000 json-any-2023.4/json_any.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.4/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-12 16:20:20.027000 json-any-2023.4/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5293 2023-07-11 12:01:48.000000 json-any-2023.4/setup.py
```

### Comparing `json-any-2023.3/PKG-INFO` & `json-any-2023.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.3
+Version: 2023.4
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.3/README-LICENCE-utf8.txt` & `json-any-2023.4/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.3/README.rst` & `json-any-2023.4/README.rst`

 * *Files identical despite different names*

### Comparing `json-any-2023.3/documentation/wiki/description.asciidoc` & `json-any-2023.4/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `json-any-2023.3/json_any/__init__.py` & `json-any-2023.4/json_any/__init__.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.3/json_any/catalog/module.py` & `json-any-2023.4/json_any/catalog/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.3/json_any/catalog/type.py` & `json-any-2023.4/json_any/catalog/type.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.3/json_any/constant.py` & `json-any-2023.4/json_any/constant.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.3/json_any/extension/numpy.py` & `json-any-2023.4/json_any/extension/numpy.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.3/json_any/extension/type.py` & `json-any-2023.4/json_any/extension/type.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.3/json_any/json_to_object.py` & `json-any-2023.4/json_any/json_to_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,16 +179,21 @@
     elif json_type.startswith(JSON_TYPE_PREFIX_PATHLIB):
         path_type = json_type[JSON_TYPE_PREFIX_PATHLIB.__len__() :]
         output_t = getattr(pthl, path_type)
         output = output_t(instance)
     elif json_type == JSON_TYPE[array_t]:
         output = AsNumpyArray(*instance)
     elif json_type.startswith(JSON_TYPE_PREFIX_PANDAS):
-        output_t = json_type[JSON_TYPE_PREFIX_PANDAS.__len__() :]
-        output = pnds.read_json(path_or_buf=instance, typ=output_t)
+        type_name, as_dict = _ObjectFromUnJSONed(
+            instance,
+            builders=builders,
+            should_continue_on_error=should_continue_on_error,
+        )
+        output_t = getattr(pnds, type_name)
+        output = output_t(as_dict)
     elif json_type.startswith(JSON_TYPE_PREFIX_SCIPY):
         sparse_type = json_type[JSON_TYPE_PREFIX_SCIPY.__len__() :]
         output_t = getattr(sprs, sparse_type)
         output = output_t(AsNumpyArray(*instance))
     elif json_type == JSON_TYPE_NUMPY_SCALAR:
         dtype, value = instance
         if isinstance(value, list):
@@ -199,46 +204,37 @@
         fake_file = io_bytes_t(instance.encode(encoding="iso-8859-1"))
         image = pypl.imread(fake_file)
         fake_file.close()
         output, axes = pypl.subplots()
         axes.set_axis_off()
         axes.matshow(image)
     elif json_type == JSON_TYPE[date_time_t]:
-        date, time = _ObjectFromUnJSONed(
-            instance,
-            should_continue_on_error=should_continue_on_error,
-        )
+        date, time = _ObjectFromUnJSONed(instance)
         output = date_time_t(
             date.year,
             date.month,
             date.day,
             time.hour,
             time.minute,
             time.second,
             time.microsecond,
             time.tzinfo,
             fold=time.fold,
         )
     elif json_type == JSON_TYPE[time_t]:
-        time_zone = _ObjectFromUnJSONed(
-            instance[4],
-            should_continue_on_error=should_continue_on_error,
-        )
+        time_zone = _ObjectFromUnJSONed(instance[4])
         as_dict = dict(
             zip(
                 ("hour", "minute", "second", "microsecond", "tzinfo", "fold"),
                 (*instance[:4], time_zone, *instance[5:]),
             )
         )
         output = time_t(**as_dict)
     elif json_type == JSON_TYPE[time_zone_t]:
-        time_delta, name = _ObjectFromUnJSONed(
-            instance,
-            should_continue_on_error=should_continue_on_error,
-        )
+        time_delta, name = _ObjectFromUnJSONed(instance)
         output = time_zone_t(time_delta, name=name)
     elif json_type.startswith(JSON_TYPE[enum_t]):
         output_t = TypeFromJsonType(
             json_type,
             prefix=JSON_TYPE[enum_t],
             should_continue_on_error=should_continue_on_error,
         )
```

### Comparing `json-any-2023.3/json_any/object_to_json.py` & `json-any-2023.4/json_any/object_to_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,20 @@
         json_type = f"{JSON_TYPE_PREFIX_PATHLIB}{instance_type.__name__}"
         jsonable = str(instance)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is array_t:
         json_type, jsonable = JSON_TYPE[array_t], AsMostConciseRepresentation(instance)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type in (data_frame_t, series_t):
-        json_type, jsonable = JSON_TYPE[instance_type], instance.to_json()
+        json_type, jsonable = JSON_TYPE[instance_type], _JsonableVersionOf(
+            (instance_type.__name__, instance.to_dict()),
+            history,
+            history_level + _HISTORY_INDENTATION,
+            descriptors=descriptors,
+        )
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type in SPARSE_ARRAY_CLASSES:
         json_type = f"{JSON_TYPE_PREFIX_SCIPY}{instance_type.__name__}"
         jsonable = AsMostConciseRepresentation(instance.toarray())
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif nmpy.issubclass_(instance_type, (nmpy.bool_, nmpy.number, nmpy.character)):
         json_type = JSON_TYPE_NUMPY_SCALAR
```

### Comparing `json-any-2023.3/json_any/version.py` & `json-any-2023.4/json_any/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.3"
+__version__ = "2023.4"
```

### Comparing `json-any-2023.3/json_any.egg-info/PKG-INFO` & `json-any-2023.4/json_any.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.3
+Version: 2023.4
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.3/setup.py` & `json-any-2023.4/setup.py`

 * *Files identical despite different names*

