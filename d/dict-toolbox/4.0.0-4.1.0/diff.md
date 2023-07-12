# Comparing `tmp/dict-toolbox-4.0.0.tar.gz` & `tmp/dict-toolbox-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dict-toolbox-4.0.0.tar", last modified: Fri Jun 23 16:46:59 2023, max compression
+gzip compressed data, was "dict-toolbox-4.1.0.tar", last modified: Wed Jul 12 15:33:49 2023, max compression
```

## Comparing `dict-toolbox-4.0.0.tar` & `dict-toolbox-4.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/
--rw-r--r--   0 root         (0) root         (0)    19053 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6368 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5499 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/dict_toolbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6368 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/dict_tools/
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/aggregation.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/args.py
--rw-r--r--   0 root         (0) root         (0)    28294 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/data.py
--rw-r--r--   0 root         (0) root         (0)    15032 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/differ.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/mysql.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/trim.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/typing.py
--rw-r--r--   0 root         (0) root         (0)     9583 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/update.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/utils.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/xml.py
--rw-r--r--   0 root         (0) root         (0)    12071 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/yamlex.py
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2638 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:33:49.185046 dict-toolbox-4.1.0/
+-rw-r--r--   0 root         (0) root         (0)    19053 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-07-12 15:33:49.185046 dict-toolbox-4.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5499 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:33:49.185046 dict-toolbox-4.1.0/dict_toolbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-07-12 15:33:49.000000 dict-toolbox-4.1.0/dict_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-07-12 15:33:49.000000 dict-toolbox-4.1.0/dict_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 15:33:49.000000 dict-toolbox-4.1.0/dict_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-12 15:33:49.000000 dict-toolbox-4.1.0/dict_toolbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-12 15:33:49.000000 dict-toolbox-4.1.0/dict_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:33:49.185046 dict-toolbox-4.1.0/dict_tools/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/aggregation.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/args.py
+-rw-r--r--   0 root         (0) root         (0)    29589 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/data.py
+-rw-r--r--   0 root         (0) root         (0)    15032 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/differ.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/trim.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/typing.py
+-rw-r--r--   0 root         (0) root         (0)     9583 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/update.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/xml.py
+-rw-r--r--   0 root         (0) root         (0)    12071 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/dict_tools/yamlex.py
+-rw-r--r--   0 root         (0) root         (0)      265 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 15:33:49.189046 dict-toolbox-4.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-07-12 15:33:33.000000 dict-toolbox-4.1.0/setup.py
```

### Comparing `dict-toolbox-4.0.0/LICENSE` & `dict-toolbox-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/PKG-INFO` & `dict-toolbox-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dict-toolbox
-Version: 4.0.0
+Version: 4.1.0
 Summary: Dict tools for Python projects
 Home-page: https://gitlab.com/saltstack/open/dict-toolbox
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `dict-toolbox-4.0.0/README.rst` & `dict-toolbox-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/dict_toolbox.egg-info/PKG-INFO` & `dict-toolbox-4.1.0/dict_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dict-toolbox
-Version: 4.0.0
+Version: 4.1.0
 Summary: Dict tools for Python projects
 Home-page: https://gitlab.com/saltstack/open/dict-toolbox
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `dict-toolbox-4.0.0/dict_tools/aggregation.py` & `dict-toolbox-4.1.0/dict_tools/aggregation.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/dict_tools/args.py` & `dict-toolbox-4.1.0/dict_tools/args.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/dict_tools/data.py` & `dict-toolbox-4.1.0/dict_tools/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -416,86 +416,106 @@
     return False
 
 
 def recursive_diff(
     old: Iterable,
     new: Iterable,
     ignore_keys: List = None,
+    ignore_keys_dict: Dict = None,
     ignore_order: bool = False,
     ignore_missing_keys: bool = False,
 ) -> Dict[str, Iterable]:
     """
     Performs a recursive diff on mappings and/or iterables and returns the result
     in a {'old': values, 'new': values}-style.
     Compares dicts and sets unordered (obviously), OrderedDicts and Lists ordered
     (but only if both ``old`` and ``new`` are of the same type),
     all other Mapping types unordered, and all other iterables ordered.
 
     :param old: Mapping or Iterable to compare from.
     :param new: Mapping or Iterable to compare to.
-    :param ignore_keys: List of keys to ignore when comparing Mappings.
-    :param ignore_order: Compare ordered mapping/iterables as if they were unordered.
+    :param ignore_keys: List of keys to ignore when comparing Mappings
+        .. deprecated:: 4.1.0 Use ignore_keys_dict instead
+    :param ignore_keys_dict: Map of keys to ignore when comparing Mappings with support for nested Mappings.
+        For example, in this collection foo is ignored as a top level key and as part of the nested "bar" -> "foo" key:
+              "foo": None
+              "bar":
+                "baz": None
+                "foo": None
+        Either ignore_keys or ignore_keys_dict must be used, but not both.
+    :param ignore_order: Compare ordered mapping/iterables as if they were unordered. Defaults to False
     :param ignore_missing_keys: Do not return keys only present in ``old``
-        but missing in ``new``. Only works for regular dicts.
+        but missing in ``new``. Only works for regular dicts. Defaults to False.
     :return dict: Returns dict with keys 'old' and 'new' containing the differences.
     """
-    ignore_keys = ignore_keys or []
+    if ignore_keys and ignore_keys_dict and ignore_keys_dict != {}:
+        raise TypeError(
+            "Either ignore_keys or ignore_keys_dict must be used, but not both."
+        )
+
+    if not ignore_keys_dict:
+        if ignore_keys:
+            ignore_keys_dict = {item: None for item in ignore_keys}
+        else:
+            ignore_keys_dict = {}
     ret_old = copy.deepcopy(old)
     ret_new = copy.deepcopy(new)
     if isinstance(old, Mapping) and isinstance(new, Mapping) and not ignore_order:
         append_old, append_new = [], []
         if len(old) != len(new):
             min_length = min(len(old), len(new))
             # The list coercion is required for Py3
             append_old = list(old.keys())[min_length:]
             append_new = list(new.keys())[min_length:]
         # Compare ordered
         for key_old, key_new in zip(old, new):
             if key_old == key_new:
-                if key_old in ignore_keys:
+                if key_old in ignore_keys_dict.keys() and not ignore_keys_dict[key_old]:
                     del ret_old[key_old]
                     del ret_new[key_new]
                 else:
                     res = recursive_diff(
                         old[key_old],
                         new[key_new],
                         ignore_keys=ignore_keys,
+                        ignore_keys_dict=ignore_keys_dict.get(key_old, {}),
                         ignore_order=ignore_order,
                         ignore_missing_keys=ignore_missing_keys,
                     )
                     if not res:  # Equal
                         del ret_old[key_old]
                         del ret_new[key_new]
                     else:
                         ret_old[key_old] = res["old"]
                         ret_new[key_new] = res["new"]
             else:
-                if key_old in ignore_keys:
+                if key_old in ignore_keys_dict.keys() and not ignore_keys_dict[key_old]:
                     del ret_old[key_old]
-                if key_new in ignore_keys:
+                if key_new in ignore_keys_dict.keys() and not ignore_keys_dict[key_old]:
                     del ret_new[key_new]
-        # If the OrderedDicts were of inequal length, add the remaining key/values.
+        # If the OrderedDicts were of not equal length, add the remaining key/values.
         for item in append_old:
             ret_old[item] = old[item]
         for item in append_new:
             ret_new[item] = new[item]
         ret = {"old": ret_old, "new": ret_new} if ret_old or ret_new else {}
     elif isinstance(old, Mapping) and isinstance(new, Mapping):
         # Compare unordered
         for key in set(list(old) + list(new)):
-            if key in ignore_keys:
+            if key in ignore_keys_dict.keys() and not ignore_keys_dict[key]:
                 if key in ret_old:
                     del ret_old[key]
                 if key in ret_new:
                     del ret_new[key]
             elif key in old and key in new:
                 res = recursive_diff(
                     old[key],
                     new[key],
                     ignore_keys=ignore_keys,
+                    ignore_keys_dict=ignore_keys_dict.get(key, {}),
                     ignore_order=ignore_order,
                     ignore_missing_keys=ignore_missing_keys,
                 )
                 if not res:  # Equal
                     del ret_old[key]
                     del ret_new[key]
                 else:
@@ -521,28 +541,30 @@
         if ignore_order:
             for item_old in old:
                 for item_new in new:
                     res = recursive_diff(
                         item_old,
                         item_new,
                         ignore_keys=ignore_keys,
+                        ignore_keys_dict=ignore_keys_dict,
                         ignore_order=ignore_order,
                         ignore_missing_keys=ignore_missing_keys,
                     )
                     if not res:
                         list_old.remove(item_old)
                         list_new.remove(item_new)
                         continue
         else:
             remove_indices = []
             for index, (iter_old, iter_new) in enumerate(zip(old, new)):
                 res = recursive_diff(
                     iter_old,
                     iter_new,
                     ignore_keys=ignore_keys,
+                    ignore_keys_dict=ignore_keys_dict,
                     ignore_order=ignore_order,
                     ignore_missing_keys=ignore_missing_keys,
                 )
                 if not res:  # Equal
                     remove_indices.append(index)
                 else:
                     list_old[index] = res["old"]
```

### Comparing `dict-toolbox-4.0.0/dict_tools/differ.py` & `dict-toolbox-4.1.0/dict_tools/differ.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/dict_tools/mysql.py` & `dict-toolbox-4.1.0/dict_tools/mysql.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/dict_tools/trim.py` & `dict-toolbox-4.1.0/dict_tools/trim.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/dict_tools/typing.py` & `dict-toolbox-4.1.0/dict_tools/typing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import get_args
 from typing import Type
 from typing import Union
 
 
 class _SpecialForm:
     __slots__ = ("_name", "__doc__", "_getitem")
 
@@ -35,14 +36,23 @@
 
       def function(arg1: typing.Computed[str]):
           ...
     """
     return Union[type_, ComputedValue]
 
 
+def is_computed(type_):
+    """Returns True if type_ is Computed type."""
+    return (
+        hasattr(type_, "__origin__")
+        and type_.__origin__ is Union
+        and ComputedValue in get_args(type_)
+    )
+
+
 class SensitiveValue:
     ...
 
 
 @_SpecialForm
 def Sensitive(self, type_: Type):
     """
```

### Comparing `dict-toolbox-4.0.0/dict_tools/update.py` & `dict-toolbox-4.1.0/dict_tools/update.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/dict_tools/utils.py` & `dict-toolbox-4.1.0/dict_tools/utils.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/dict_tools/xml.py` & `dict-toolbox-4.1.0/dict_tools/xml.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/dict_tools/yamlex.py` & `dict-toolbox-4.1.0/dict_tools/yamlex.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-4.0.0/setup.py` & `dict-toolbox-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import Command
 from setuptools import setup
 
 NAME = "dict_tools"
 DESC = "Dict tools for Python projects"
 
 # Version info -- read without importing
-VERSION = "4.0.0"
+VERSION = "4.1.0"
 
 SETUP_DIRNAME = os.path.dirname(__file__)
 if not SETUP_DIRNAME:
     SETUP_DIRNAME = os.getcwd()
 
 with open("README.rst", encoding="utf-8") as f:
     LONG_DESC = f.read()
```

