# Comparing `tmp/punktdict-0.10.tar.gz` & `tmp/punktdict-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punktdict-0.10.tar", last modified: Mon Jul 10 17:15:42 2023, max compression
+gzip compressed data, was "punktdict-0.11.tar", last modified: Wed Jul 12 12:04:31 2023, max compression
```

## Comparing `punktdict-0.10.tar` & `punktdict-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 17:15:42.035198 punktdict-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-10 17:15:37.000000 punktdict-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0       98 2023-07-10 17:15:36.000000 punktdict-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3679 2023-07-10 17:15:42.036194 punktdict-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     3081 2023-07-10 17:15:16.000000 punktdict-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 17:15:42.032205 punktdict-0.10/punktdict/
--rw-rw-rw-   0        0        0     3081 2023-07-10 17:15:16.000000 punktdict-0.10/punktdict/README.MD
--rw-rw-rw-   0        0        0     7860 2023-07-10 17:13:09.000000 punktdict-0.10/punktdict/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-10 17:15:41.000000 punktdict-0.10/punktdict/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-07-10 17:15:41.000000 punktdict-0.10/punktdict/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-10 17:15:42.035198 punktdict-0.10/punktdict.egg-info/
--rw-rw-rw-   0        0        0     3679 2023-07-10 17:15:41.000000 punktdict-0.10/punktdict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-10 17:15:41.000000 punktdict-0.10/punktdict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 17:15:41.000000 punktdict-0.10/punktdict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 17:15:41.000000 punktdict-0.10/punktdict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-10 17:15:42.036194 punktdict-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1234 2023-07-10 17:15:41.000000 punktdict-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:04:31.903320 punktdict-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-12 12:04:25.000000 punktdict-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0       98 2023-07-12 12:04:21.000000 punktdict-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2918 2023-07-12 12:04:31.904317 punktdict-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2320 2023-07-12 12:02:52.000000 punktdict-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 12:04:31.901325 punktdict-0.11/punktdict/
+-rw-rw-rw-   0        0        0     2320 2023-07-12 12:02:52.000000 punktdict-0.11/punktdict/README.MD
+-rw-rw-rw-   0        0        0     6996 2023-07-12 11:58:15.000000 punktdict-0.11/punktdict/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 12:04:30.000000 punktdict-0.11/punktdict/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-07-12 12:04:30.000000 punktdict-0.11/punktdict/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-12 12:04:31.903320 punktdict-0.11/punktdict.egg-info/
+-rw-rw-rw-   0        0        0     2918 2023-07-12 12:04:31.000000 punktdict-0.11/punktdict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-12 12:04:31.000000 punktdict-0.11/punktdict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:04:31.000000 punktdict-0.11/punktdict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 12:04:31.000000 punktdict-0.11/punktdict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-12 12:04:31.904317 punktdict-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2023-07-12 12:04:30.000000 punktdict-0.11/setup.py
```

### Comparing `punktdict-0.10/LICENSE.rst` & `punktdict-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `punktdict-0.10/punktdict/__init__.py` & `punktdict-0.11/punktdict/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,188 +1,201 @@
-def convert_back(di):
+import sys
+
+dictconfig = sys.modules[__name__]
+# Create a reference to the current module's `sys.modules` dictionary,
+# which allows accessing and modifying the configuration options.
+
+dictconfig.allow_nested_attribute_creation = True
+# Set the configuration option `allow_nested_attribute_creation` to True,
+# allowing the creation of nested attributes in PunktDict objects.
+
+dictconfig.allow_nested_key_creation = True
+# Set the configuration option `allow_nested_key_creation` to True,
+# allowing the creation of nested keys in PunktDict objects.
+
+dictconfig.convert_all_dicts_recursively = True
+# Set the configuration option `convert_all_dicts_recursively` to True,
+# enabling recursive conversion of all nested dictionaries in PunktDict objects.
+
+
+def check_if_compatible_dict(di, class_):
+    """
+    Check if the provided object is a compatible dictionary based on its type and attributes.
+
+    Args:
+    - di: The object to check for compatibility.
+    - class_: The class representing the compatible dictionary type.
+
+    Returns:
+    - True if the object is a compatible dictionary, False otherwise.
+
+
+    """
+    return (isinstance(di, dict) and not isinstance(di, class_)) or (
+        (hasattr(di, "items") and hasattr(di, "keys") and hasattr(di, "values"))
+    )
+
+
+def convert_to_dict(di):
+    """
+    Recursively converts a PunktDict object or a compatible dictionary to a regular dictionary.
+
+    Args:
+    - di: The PunktDict object or compatible dictionary to convert.
+
+    Returns:
+    - The converted regular dictionary.
+    """
     if isinstance(di, dict) or (
-        hasattr(di, "items") and hasattr(di, "keys") and hasattr(di, "keys")
+        hasattr(di, "items") and hasattr(di, "keys") and hasattr(di, "values")
     ):
-        di = {k: convert_back(v) for k, v in di.items()}
+        di = {k: convert_to_dict(v) for k, v in di.items()}
     return di
 
 
-_extra_methods_and_attributes = (
-    "_check_forbidden_key",
-    "convert_to_regular_dict",
-    "_allow_nested_creation",
-)
-
-
 class PunktDict(dict):
     """
-    A dictionary-like object with extended functionality.
+    A subclass of dict with additional functionality for handling nested dictionaries.
 
-    This class is a subclass of the built-in `dict` class. It adds several features and overrides
-    certain methods to provide additional behavior.
+    Overrides some methods and provides additional methods to handle nested dictionaries.
 
     Attributes:
-        _allow_nested_creation: whether to allow nested key creation:
-            if True, this will work:
-            dd["school"]["room2"]["student1"] = "Bruno"
-            dd.school.room3.student1 = "Bruno"
+    - allow_nested_attribute_creation: A boolean flag indicating whether PunktDict allows creation of nested attributes.
+    - allow_nested_key_creation: A boolean flag indicating whether PunktDict allows creation of nested keys.
+    - convert_all_dicts_recursively: A boolean flag indicating whether PunktDict recursively converts all nested dictionaries to PunktDict objects.
 
     Methods:
-        __new__(cls, o=None, *args, **kwargs): Overrides the creation of a new instance of `PunktDict`.
-        __init__(self, seq=None, **kwargs): Initializes a `PunktDict` instance.
-        _check_forbidden_key(self, *args, **kwargs): Checks if a key is forbidden.
-        __setattr__(self, key, value): Overrides the setting of an attribute.
-        __delitem__(self, key): Overrides the deletion of an item.
-        __getitem__(self, item): Overrides the retrieval of an item.
-        __setitem__(self, key, value): Overrides the assignment of an item.
-        __delattr__(self, item): Overrides the deletion of an attribute.
-        __missing__(self, key): Overrides the handling of missing keys.
-        __getattribute__(self, name): Overrides the retrieval of an attribute.
-        __getattr__(self, item): Overrides the retrieval of a missing attribute.
-        convert_to_regular_dict: Converts the PunktDict to a regular dict
-
-    Usage:
-        # Create a new instance of PunktDict
-        dd = PunktDict({'school': {'room1': {'student1': 'Mario', 'student2': 'Mario'}}})
-
-        # Access and modify values using dictionary-like syntax
-        dd['school']['room1']['student6'] = 'Antonio'
-        dd['school']['room2']['student1'] = 'Bruno'
-        dd.school.room3.student1 = 'Bruno'
-
-        # Delete an item
-        del dd['school']['room2']['student1']
-
-        # Access and modify attributes using dot notation
-        dd.university.all_rooms = []
-        dd.university.all_rooms.append(1)
-        dd['university']['all_rooms'].append(2)
-        dd.university['all_rooms'].append(3)
-
-        # Print the PunktDict object
-        print(dd)
-    """
-
-    def __new__(cls, seq=None, allow_nested_creation=True, *args, **kwargs):
-        # Create a new instance of the class
-        new_dict = super().__new__(cls, seq)
-        new_dict._allow_nested_creation = allow_nested_creation
-        if seq:
-            # Check if the keys are strings and set them as attributes of the object
-            for key, item in new_dict.items():
-                if isinstance(key, str):
-                    if not hasattr(new_dict, key):
-                        try:
-                            new_dict.__setattr__(key, item)
-                        except (TypeError, ValueError):
-                            continue
-
-        return new_dict
-
-    def __init__(self, seq=None, allow_nested_creation=True, **kwargs):
-        if seq:
-            # Initialize the dictionary with the given sequence
-            super().__init__(seq, **kwargs)
+    - __init__(self, *args, **kwargs): Initializes a new PunktDict object.
+    - __setitem__(self, key, value): Sets an item in the PunktDict.
+    - __missing__(self, key): Handles missing key access in the PunktDict.
+    - update(self, *args, **kwargs): Updates the PunktDict with new data.
+    - _check_forbidden_key(self, *args, **kwargs): Checks if a key is forbidden.
+    - __getattr__(self, item): Handles attribute access in the PunktDict.
+
+
+    """
+
+    def __init__(self, *args, **kwargs):
+        """
+        Initializes a new PunktDict object.
+
+        Args:
+        - *args: Variable length argument list.
+        - **kwargs: Arbitrary keyword arguments.
+
+        Notes:
+        - Converts all nested dictionaries in the PunktDict object to PunktDict objects
+          if the `convert_all_dicts_recursively` option is enabled.
+        - Maps the PunktDict object itself to its `__dict__` attribute.
+        """
 
         def convert_dict(di):
-            if (isinstance(di, dict) and not isinstance(di, self.__class__)) or (
-                (hasattr(di, "items") and hasattr(di, "keys") and hasattr(di, "keys"))
-            ):
-                # Convert nested dictionaries to PunktDict instances recursively
-                ndi = self.__class__({}, allow_nested_creation=allow_nested_creation)
+            """
+            Recursively converts a compatible dictionary to a PunktDict object.
+
+            Args:
+            - di: The compatible dictionary to convert.
+
+            Returns:
+            - The converted PunktDict object.
+            """
+            if check_if_compatible_dict(di, self.__class__):
+                ndi = self.__class__({})
                 for k, v in di.items():
                     ndi[k] = convert_dict(v)
                 return ndi
             return di
 
-        for key in self:
-            if key not in dir(dict) and key not in _extra_methods_and_attributes:
-                # Convert non-dictionary values to PunktDict instances
-                self[key] = convert_dict(self[key])
+        super().__init__(*args, **kwargs)
+        if dictconfig.convert_all_dicts_recursively:
+            for key in self:
+                if key not in dir(dict):
+                    self[key] = convert_dict(self[key])
+        self.__dict__ = self
 
-    def _check_forbidden_key(self, *args, **kwargs):
-        # can be overwritten like:
-        # PunktDict._check_forbidden_key = lambda self, x: x.startswith('_ipytho') or x == '_repr_mimebundle_'
-        # to prevent accidental dict creation when _allow_nested_creation is True, if the function returns True, the key will not be created
-        return False
+    def __setitem__(self, key, value):
+        """
+        Sets an item in the PunktDict.
 
-    def __setattr__(self, key, value):
-        if key in dir(dict):
-            raise KeyError
-        # Set an attribute and an item with the same key
+        Args:
+        - key: The key to set.
+        - value: The value to assign to the key.
+
+        Notes:
+        - Converts the value to a PunktDict object if it is a compatible dictionary
+          and the `convert_all_dicts_recursively` option is enabled.
+        - Raises a ValueError if the key is not allowed.
+        """
+        if dictconfig.convert_all_dicts_recursively:
+            if check_if_compatible_dict(value, self.__class__):
+                value = self.__class__(value)
         if key not in dir(dict):
-            super().__setattr__(key, value)
-
-        if key not in _extra_methods_and_attributes:
             super().__setitem__(key, value)
+        else:
+            raise ValueError(f'Key "{key}" not allowed!')
 
-    def update(self, *args, **kwargs) -> None:
-        allargs = [self.__class__(x) for x in args]
-        super().update(*allargs, **kwargs)
+    def __missing__(self, key):
+        """
+        Handles missing key access in the PunktDict.
 
-    def __delitem__(self, key):
-        # Delete an item and its corresponding attribute (if it exists)
-        super().__delitem__(key)
-        if isinstance(key, str):
-            if hasattr(self, key):
-                if key not in dir(dict) and key not in _extra_methods_and_attributes:
-                    super().__delattr__(key)
-
-    def __getitem__(self, item):
-        try:
-            # Get an item using dictionary-like syntax
-            return super().__getitem__(item)
-        except KeyError:
-            if item not in dir(dict) and item not in _extra_methods_and_attributes:
-                # If the key doesn't exist, create an empty PunktDict instance for that key
-                self.__setitem__(item, self.__class__())
-                return self.__getitem__(item)
+        Args:
+        - key: The missing key.
 
-    def __setitem__(self, key, value):
-        # Set an item using dictionary-like syntax
-        if isinstance(value, dict) and not isinstance(value, self.__class__):
-            print(value)
-            value = self.__class__(value)
-        super().__setitem__(key, value)
-        if isinstance(key, str):
-            if key not in dir(dict) and key not in _extra_methods_and_attributes:
-                try:
-                    # Set an attribute with the same key
-                    self.__setattr__(key, self[key])
-                except (TypeError, ValueError):
-                    pass
-
-    def __delattr__(self, item):
-        # Delete an attribute and its corresponding item (if it exists)
-        if item not in dir(dict) and item not in _extra_methods_and_attributes:
-            super().__delattr__(item)
-        if item in self:
-            del self[item]
+        Returns:
+        - The created nested PunktDict if `allow_nested_key_creation` is enabled.
 
-    def __missing__(self, key):
-        # Handle missing keys by creating an empty PunktDict instance for that key
-        if not self._allow_nested_creation:
-            raise KeyError
-        if key not in dir(dict) and key not in _extra_methods_and_attributes:
+        Raises:
+        - KeyError: If `allow_nested_key_creation` is disabled and the key is not found.
+        """
+        if dictconfig.allow_nested_key_creation:
             self[key] = self.__class__({})
             return self[key]
+        raise KeyError(f'"{key}" not found')
+
+    def update(self, *args, **kwargs) -> None:
+        """
+        Updates the PunktDict with new data.
 
-    def __getattribute__(self, name):
-        if name in dir(dict) or name in _extra_methods_and_attributes:
-            return super().__getattribute__(name)
-        if name in self:
-            # Get an attribute using dot notation
-            return self[name]
-        return super().__getattribute__(name)
+        Args:
+        - *args: Variable length argument list.
+        - **kwargs: Arbitrary keyword arguments.
+
+        Notes:
+        - Converts all nested dictionaries in the new data to PunktDict objects
+          if the `convert_all_dicts_recursively` option is enabled.
+        """
+        if dictconfig.convert_all_dicts_recursively:
+            args = [self.__class__(x) for x in args]
+        super().update(*args, **kwargs)
+
+    def _check_forbidden_key(self, *args, **kwargs):
+        """
+        Checks if a key is forbidden.
+        Method can be overwritten
+
+        Args:
+        - *args: Variable length argument list.
+        - **kwargs: Arbitrary keyword arguments.
+
+        Returns:
+        - False always.
+        """
+        return False
 
     def __getattr__(self, item):
-        if not self._allow_nested_creation:
-            raise KeyError
-        if not self._check_forbidden_key(item):
-            # If the attribute doesn't exist, create an empty PunktDict instance for that attribute
-            self.__setitem__(item, self.__class__())
-        return self.__getattribute__(item)
+        """
+        Handles attribute access in the PunktDict.
 
-    def convert_to_regular_dict(self):
-        return convert_back(self)
+        Args:
+        - item: The attribute name.
 
+        Returns:
+        - The created nested PunktDict if `allow_nested_attribute_creation` is enabled.
 
+        Raises:
+        - AttributeError: If `allow_nested_attribute_creation` is disabled or the attribute is forbidden.
+        """
+        if not self._check_forbidden_key(item):
+            if dictconfig.allow_nested_attribute_creation:
+                self[item] = self.__class__({})
+                return self[item]
+        raise AttributeError
```

### Comparing `punktdict-0.10/setup.py` & `punktdict-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''a dict with key attributes'''
 
 # Setting up
 setup(
     name="punktdict",
     version=VERSION,
     license='MIT',
```

