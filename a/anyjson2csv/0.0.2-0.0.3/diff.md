# Comparing `tmp/anyjson2csv-0.0.2.tar.gz` & `tmp/anyjson2csv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyjson2csv-0.0.2.tar", last modified: Wed Jul 12 11:29:21 2023, max compression
+gzip compressed data, was "anyjson2csv-0.0.3.tar", last modified: Wed Jul 12 12:05:06 2023, max compression
```

## Comparing `anyjson2csv-0.0.2.tar` & `anyjson2csv-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:29:21.447466 anyjson2csv-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-07-12 08:57:26.000000 anyjson2csv-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      526 2023-07-12 11:29:21.445469 anyjson2csv-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-12 08:55:33.000000 anyjson2csv-0.0.2/README.md
--rw-rw-rw-   0        0        0      626 2023-07-12 11:27:35.000000 anyjson2csv-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 11:29:21.448465 anyjson2csv-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 11:29:21.378466 anyjson2csv-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 11:29:21.401467 anyjson2csv-0.0.2/src/anyjson2csv/
--rw-rw-rw-   0        0        0        2 2023-07-12 11:27:26.000000 anyjson2csv-0.0.2/src/anyjson2csv/__init__.py
--rw-rw-rw-   0        0        0     3446 2023-07-12 10:02:58.000000 anyjson2csv-0.0.2/src/anyjson2csv/flatten_json.py
--rw-rw-rw-   0        0        0      686 2023-07-12 11:28:48.000000 anyjson2csv-0.0.2/src/anyjson2csv/json_to_csv.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:29:21.442460 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/
--rw-rw-rw-   0        0        0      526 2023-07-12 11:29:21.000000 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-12 11:29:21.000000 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:29:21.000000 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 11:29:21.000000 anyjson2csv-0.0.2/src/anyjson2csv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 12:05:06.571759 anyjson2csv-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-07-12 08:57:26.000000 anyjson2csv-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      526 2023-07-12 12:05:06.568757 anyjson2csv-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:55:33.000000 anyjson2csv-0.0.3/README.md
+-rw-rw-rw-   0        0        0      626 2023-07-12 12:04:23.000000 anyjson2csv-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 12:05:06.571759 anyjson2csv-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 12:05:06.495755 anyjson2csv-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 12:05:06.520761 anyjson2csv-0.0.3/src/anyjson2csv/
+-rw-rw-rw-   0        0        0        2 2023-07-12 11:27:26.000000 anyjson2csv-0.0.3/src/anyjson2csv/__init__.py
+-rw-rw-rw-   0        0        0     3312 2023-07-12 12:03:37.000000 anyjson2csv-0.0.3/src/anyjson2csv/flatten_json.py
+-rw-rw-rw-   0        0        0      462 2023-07-12 12:03:34.000000 anyjson2csv-0.0.3/src/anyjson2csv/json_to_csv.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:05:06.565757 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-07-12 12:05:06.000000 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-07-12 12:05:06.000000 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:05:06.000000 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 12:05:06.000000 anyjson2csv-0.0.3/src/anyjson2csv.egg-info/top_level.txt
```

### Comparing `anyjson2csv-0.0.2/LICENSE.txt` & `anyjson2csv-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anyjson2csv-0.0.2/PKG-INFO` & `anyjson2csv-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyjson2csv
-Version: 0.0.2
+Version: 0.0.3
 Summary: JSON flatten to CSV for Python
 Author-email: BrainsLogic <info@brainslogic.com>
 Project-URL: Homepage, https://github.com/mehdiabidi/json2csv
 Project-URL: Bug Tracker, https://github.com/mehdiabidi/json2csv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anyjson2csv-0.0.2/pyproject.toml` & `anyjson2csv-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anyjson2csv"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="BrainsLogic", email="info@brainslogic.com" },
 ]
 description = "JSON flatten to CSV for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `anyjson2csv-0.0.2/src/anyjson2csv/flatten_json.py` & `anyjson2csv-0.0.3/src/anyjson2csv/flatten_json.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
             elif type(d_v) == list:
                 to_be_flat_dict.update(list_flatten_json(d_k, d_v))
 
             else:
                 to_be_flat_dict[d_k] = d_v
 
-        # print(to_be_flat_dict)
         updated_json_list.append(to_be_flat_dict)
 
     else:
         pass
 
     return updated_json_list
 
@@ -60,24 +59,22 @@
                 )
             else:
                 dictionary_fun_dict.update(
                     list_flatten_json(d_k, d_v, c_str=str(dict_key))
                 )
 
         else:
-            # print("Testing-------")
             if c_str:
                 dictionary_fun_dict[
                     str(c_str) + "_" + str(dict_key) + "_" + str(d_k)
                 ] = d_v
 
             else:
                 dictionary_fun_dict[str(dict_key) + "_" + str(d_k)] = d_v
 
-    # print("Dict", dict_fun_dict)
     return dictionary_fun_dict
 
 
 def list_flatten_json(d_k, d_v, c_str=None):
     list_fun_dict = {}
 
     for lst_index, lst_obj in enumerate(d_v):
@@ -103,9 +100,8 @@
             if c_str:
                 list_fun_dict[
                     str(c_str) + "_" + str(d_k) + "_" + str(lst_index)
                 ] = lst_obj
             else:
                 list_fun_dict[str(d_k) + "_" + str(lst_index)] = lst_obj
 
-    # print(new_data_r)
     return list_fun_dict
```

### Comparing `anyjson2csv-0.0.2/src/anyjson2csv.egg-info/PKG-INFO` & `anyjson2csv-0.0.3/src/anyjson2csv.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyjson2csv
-Version: 0.0.2
+Version: 0.0.3
 Summary: JSON flatten to CSV for Python
 Author-email: BrainsLogic <info@brainslogic.com>
 Project-URL: Homepage, https://github.com/mehdiabidi/json2csv
 Project-URL: Bug Tracker, https://github.com/mehdiabidi/json2csv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

