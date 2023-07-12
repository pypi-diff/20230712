# Comparing `tmp/strinpy-0.0.3.tar.gz` & `tmp/strinpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strinpy-0.0.3.tar", last modified: Tue Jul 11 12:51:13 2023, max compression
+gzip compressed data, was "strinpy-0.0.4.tar", last modified: Wed Jul 12 04:24:20 2023, max compression
```

## Comparing `strinpy-0.0.3.tar` & `strinpy-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:51:13.594259 strinpy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-11 12:51:05.000000 strinpy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-11 12:51:13.594259 strinpy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-11 12:51:05.000000 strinpy-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:51:13.594259 strinpy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 12:51:05.000000 strinpy-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:51:13.594259 strinpy-0.0.3/strinpy/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 12:51:05.000000 strinpy-0.0.3/strinpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-11 12:51:05.000000 strinpy-0.0.3/strinpy/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:51:13.594259 strinpy-0.0.3/strinpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-11 12:51:13.000000 strinpy-0.0.3/strinpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-11 12:51:13.000000 strinpy-0.0.3/strinpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:51:13.000000 strinpy-0.0.3/strinpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 12:51:13.000000 strinpy-0.0.3/strinpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:24:20.585061 strinpy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-12 04:24:09.000000 strinpy-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 04:24:20.585061 strinpy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-12 04:24:09.000000 strinpy-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 04:24:20.585061 strinpy-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 04:24:09.000000 strinpy-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:24:20.585061 strinpy-0.0.4/strinpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 04:24:09.000000 strinpy-0.0.4/strinpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-12 04:24:09.000000 strinpy-0.0.4/strinpy/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:24:20.585061 strinpy-0.0.4/strinpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-12 04:24:20.000000 strinpy-0.0.4/strinpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-12 04:24:20.000000 strinpy-0.0.4/strinpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:24:20.000000 strinpy-0.0.4/strinpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 04:24:20.000000 strinpy-0.0.4/strinpy.egg-info/top_level.txt
```

### Comparing `strinpy-0.0.3/LICENSE` & `strinpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strinpy-0.0.3/PKG-INFO` & `strinpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strinpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: React like string builder
 Home-page: https://github.com/am230/strinpy
 Author: am230
 License: MIT Licence
 Keywords: string
 Platform: any
 Description-Content-Type: text/x-rst
```

### Comparing `strinpy-0.0.3/README.rst` & `strinpy-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `strinpy-0.0.3/setup.py` & `strinpy-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 author = 'am230'
 name = 'strinpy'
 py_modules = [name]
 
 setup(
     name=name,
-    version="0.0.3",
+    version="0.0.4",
     keywords=["string"],
     description="React like string builder",
     long_description=long_description,
     license="MIT Licence",
     long_description_content_type='text/x-rst',
     packages=find_packages(),
     url=f"https://github.com/{author}/{name}",
```

### Comparing `strinpy-0.0.3/strinpy/builder.py` & `strinpy-0.0.4/strinpy/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 class Builder(_t.Generic[V]):
     def __init__(self, formatter: Formatter = Formatter()) -> None:
         self.formatter = formatter
 
     def format_value(self, value: V | Value) -> _t.Tuple[str]:
         if value in (False, None):
             return EMPTY_TUPLE
-        if isinstance(value, list):
+        type_ = type(value)
+        if type_ in (list, tuple, set, map, filter, frozenset):
             return tuple(itertools.chain.from_iterable(map(self.format_value, value)))
         elif callable(value):
             return value()
         return self.formatter.format_value(value)
 
     def build(self, value: V) -> str:
         parts = self.format_value(value)
```

### Comparing `strinpy-0.0.3/strinpy.egg-info/PKG-INFO` & `strinpy-0.0.4/strinpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strinpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: React like string builder
 Home-page: https://github.com/am230/strinpy
 Author: am230
 License: MIT Licence
 Keywords: string
 Platform: any
 Description-Content-Type: text/x-rst
```

