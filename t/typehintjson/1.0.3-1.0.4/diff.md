# Comparing `tmp/typehintjson-1.0.3.tar.gz` & `tmp/typehintjson-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typehintjson-1.0.3.tar", last modified: Wed Jul 12 19:29:59 2023, max compression
+gzip compressed data, was "typehintjson-1.0.4.tar", last modified: Wed Jul 12 19:58:04 2023, max compression
```

## Comparing `typehintjson-1.0.3.tar` & `typehintjson-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 19:29:59.801664 typehintjson-1.0.3/
--rw-rw-rw-   0        0        0     1563 2023-07-12 19:29:59.800697 typehintjson-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 19:29:59.801664 typehintjson-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-07-12 19:26:27.000000 typehintjson-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 19:29:59.781316 typehintjson-1.0.3/typehintjson/
--rw-rw-rw-   0        0        0      223 2023-03-24 07:05:32.000000 typehintjson-1.0.3/typehintjson/__init__.py
--rw-rw-rw-   0        0        0     4053 2023-07-12 19:27:06.000000 typehintjson-1.0.3/typehintjson/_impl.py
--rw-rw-rw-   0        0        0      390 2022-12-26 18:49:51.000000 typehintjson-1.0.3/typehintjson/example.py
-drwxrwxrwx   0        0        0        0 2023-07-12 19:29:59.797662 typehintjson-1.0.3/typehintjson.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-07-12 19:29:58.000000 typehintjson-1.0.3/typehintjson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-12 19:29:59.000000 typehintjson-1.0.3/typehintjson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 19:29:58.000000 typehintjson-1.0.3/typehintjson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 19:29:59.000000 typehintjson-1.0.3/typehintjson.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 19:58:04.532863 typehintjson-1.0.4/
+-rw-rw-rw-   0        0        0     1563 2023-07-12 19:58:04.531863 typehintjson-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:58:04.532863 typehintjson-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-07-12 19:57:51.000000 typehintjson-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:58:04.500852 typehintjson-1.0.4/typehintjson/
+-rw-rw-rw-   0        0        0      223 2023-03-24 07:05:32.000000 typehintjson-1.0.4/typehintjson/__init__.py
+-rw-rw-rw-   0        0        0     4140 2023-07-12 19:57:43.000000 typehintjson-1.0.4/typehintjson/_impl.py
+-rw-rw-rw-   0        0        0      390 2022-12-26 18:49:51.000000 typehintjson-1.0.4/typehintjson/example.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:58:04.527896 typehintjson-1.0.4/typehintjson.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-07-12 19:58:03.000000 typehintjson-1.0.4/typehintjson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-12 19:58:04.000000 typehintjson-1.0.4/typehintjson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:58:03.000000 typehintjson-1.0.4/typehintjson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 19:58:04.000000 typehintjson-1.0.4/typehintjson.egg-info/top_level.txt
```

### Comparing `typehintjson-1.0.3/PKG-INFO` & `typehintjson-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typehintjson
-Version: 1.0.3
+Version: 1.0.4
 Summary: Converts dataclasses / enums to JSON and back using type hints
 Home-page: https://github.com/Sanjay-Ganeshan/typehintjson
 Author: Julie Ganeshan
 Author-email: HeavenlyQueen@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `typehintjson-1.0.3/setup.py` & `typehintjson-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("typehintjson/README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="typehintjson",
-    version="1.0.3",
+    version="1.0.4",
     author="Julie Ganeshan",
     author_email="HeavenlyQueen@outlook.com",
     description="Converts dataclasses / enums to JSON and back using type hints",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sanjay-Ganeshan/typehintjson",
     packages=setuptools.find_packages(),
```

### Comparing `typehintjson-1.0.3/typehintjson/_impl.py` & `typehintjson-1.0.4/typehintjson/_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,23 +23,23 @@
             return obj.value
         else:
             return {"name": obj.name, "value": obj.value}
     
     if dataclasses.is_dataclass(obj):
         fields = dataclasses.fields(obj)
         return {
-            f.name: dataclass_to_dictionary(getattr(obj, f.name))
+            f.name: dataclass_to_dictionary(getattr(obj, f.name), flatten_enums=flatten_enums)
             for f in fields
         }
 
     if isinstance(obj, list):
-        return [dataclass_to_dictionary(item) for item in obj]
+        return [dataclass_to_dictionary(item, flatten_enums=flatten_enums) for item in obj]
 
     if isinstance(obj, dict):
-        return {k: dataclass_to_dictionary(obj[k]) for k in obj}
+        return {k: dataclass_to_dictionary(obj[k], flatten_enums=flatten_enums) for k in obj}
     
     return obj
 
 def parse_as_type(js_obj: T.Any, expected_type: T.Type[T.Any]) -> T.Any:
     """
     Parses the json object js_obj as an instance of the given type.
     Raises an exception if the object does not match the type.
```

### Comparing `typehintjson-1.0.3/typehintjson.egg-info/PKG-INFO` & `typehintjson-1.0.4/typehintjson.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typehintjson
-Version: 1.0.3
+Version: 1.0.4
 Summary: Converts dataclasses / enums to JSON and back using type hints
 Home-page: https://github.com/Sanjay-Ganeshan/typehintjson
 Author: Julie Ganeshan
 Author-email: HeavenlyQueen@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

