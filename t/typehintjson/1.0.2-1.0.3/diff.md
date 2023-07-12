# Comparing `tmp/typehintjson-1.0.2.tar.gz` & `tmp/typehintjson-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typehintjson-1.0.2.tar", last modified: Fri Mar 24 07:06:08 2023, max compression
+gzip compressed data, was "typehintjson-1.0.3.tar", last modified: Wed Jul 12 19:29:59 2023, max compression
```

## Comparing `typehintjson-1.0.2.tar` & `typehintjson-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 07:06:08.731173 typehintjson-1.0.2/
--rw-rw-rw-   0        0        0     1563 2023-03-24 07:06:08.730182 typehintjson-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-03-24 07:06:08.732175 typehintjson-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-03-24 07:05:46.000000 typehintjson-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:06:08.699159 typehintjson-1.0.2/typehintjson/
--rw-rw-rw-   0        0        0      223 2023-03-24 07:05:32.000000 typehintjson-1.0.2/typehintjson/__init__.py
--rw-rw-rw-   0        0        0     3948 2023-03-23 20:37:23.000000 typehintjson-1.0.2/typehintjson/_impl.py
--rw-rw-rw-   0        0        0      390 2022-12-26 18:49:51.000000 typehintjson-1.0.2/typehintjson/example.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:06:08.727146 typehintjson-1.0.2/typehintjson.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-03-24 07:06:07.000000 typehintjson-1.0.2/typehintjson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-03-24 07:06:08.000000 typehintjson-1.0.2/typehintjson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 07:06:07.000000 typehintjson-1.0.2/typehintjson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-24 07:06:07.000000 typehintjson-1.0.2/typehintjson.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 19:29:59.801664 typehintjson-1.0.3/
+-rw-rw-rw-   0        0        0     1563 2023-07-12 19:29:59.800697 typehintjson-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:29:59.801664 typehintjson-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-07-12 19:26:27.000000 typehintjson-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:29:59.781316 typehintjson-1.0.3/typehintjson/
+-rw-rw-rw-   0        0        0      223 2023-03-24 07:05:32.000000 typehintjson-1.0.3/typehintjson/__init__.py
+-rw-rw-rw-   0        0        0     4053 2023-07-12 19:27:06.000000 typehintjson-1.0.3/typehintjson/_impl.py
+-rw-rw-rw-   0        0        0      390 2022-12-26 18:49:51.000000 typehintjson-1.0.3/typehintjson/example.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:29:59.797662 typehintjson-1.0.3/typehintjson.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-07-12 19:29:58.000000 typehintjson-1.0.3/typehintjson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-12 19:29:59.000000 typehintjson-1.0.3/typehintjson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:29:58.000000 typehintjson-1.0.3/typehintjson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 19:29:59.000000 typehintjson-1.0.3/typehintjson.egg-info/top_level.txt
```

### Comparing `typehintjson-1.0.2/PKG-INFO` & `typehintjson-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typehintjson
-Version: 1.0.2
+Version: 1.0.3
 Summary: Converts dataclasses / enums to JSON and back using type hints
 Home-page: https://github.com/Sanjay-Ganeshan/typehintjson
 Author: Julie Ganeshan
 Author-email: HeavenlyQueen@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `typehintjson-1.0.2/setup.py` & `typehintjson-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("typehintjson/README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="typehintjson",
-    version="1.0.2",
+    version="1.0.3",
     author="Julie Ganeshan",
     author_email="HeavenlyQueen@outlook.com",
     description="Converts dataclasses / enums to JSON and back using type hints",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sanjay-Ganeshan/typehintjson",
     packages=setuptools.find_packages(),
```

### Comparing `typehintjson-1.0.2/typehintjson/_impl.py` & `typehintjson-1.0.3/typehintjson/_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,23 @@
     in the dataclass's generated __init__ function
     """
     fields = {f.name for f in dataclasses.fields(as_dataclass) if f.init}
     return {
         k: args_dict[k] for k in args_dict if k in fields
     }
 
-def dataclass_to_dictionary(obj: T.Any) -> T.Any:
+def dataclass_to_dictionary(obj: T.Any, flatten_enums: bool = False) -> T.Any:
     """
     Converts a dataclass to a dictionary
     """
     if isinstance(obj, enum.Enum):
-        return {"name": obj.name, "value": obj.value}
+        if flatten_enums:
+            return obj.value
+        else:
+            return {"name": obj.name, "value": obj.value}
     
     if dataclasses.is_dataclass(obj):
         fields = dataclasses.fields(obj)
         return {
             f.name: dataclass_to_dictionary(getattr(obj, f.name))
             for f in fields
         }
```

### Comparing `typehintjson-1.0.2/typehintjson.egg-info/PKG-INFO` & `typehintjson-1.0.3/typehintjson.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typehintjson
-Version: 1.0.2
+Version: 1.0.3
 Summary: Converts dataclasses / enums to JSON and back using type hints
 Home-page: https://github.com/Sanjay-Ganeshan/typehintjson
 Author: Julie Ganeshan
 Author-email: HeavenlyQueen@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

