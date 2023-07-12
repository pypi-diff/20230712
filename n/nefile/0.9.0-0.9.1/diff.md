# Comparing `tmp/nefile-0.9.0.tar.gz` & `tmp/nefile-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nefile-0.9.0.tar", last modified: Mon Jun 26 21:42:43 2023, max compression
+gzip compressed data, was "nefile-0.9.1.tar", last modified: Wed Jul 12 14:12:31 2023, max compression
```

## Comparing `nefile-0.9.0.tar` & `nefile-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:42:43.765614 nefile-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 21:42:32.000000 nefile-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-26 21:42:43.765614 nefile-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-26 21:42:32.000000 nefile-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:42:43.761614 nefile-0.9.0/nefile/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:42:32.000000 nefile-0.9.0/nefile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-06-26 21:42:32.000000 nefile-0.9.0/nefile/nefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-06-26 21:42:32.000000 nefile-0.9.0/nefile/resource_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:42:43.765614 nefile-0.9.0/nefile/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:42:32.000000 nefile-0.9.0/nefile/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-26 21:42:32.000000 nefile-0.9.0/nefile/resources/application_defined_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-26 21:42:32.000000 nefile-0.9.0/nefile/resources/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-26 21:42:32.000000 nefile-0.9.0/nefile/resources/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-06-26 21:42:32.000000 nefile-0.9.0/nefile/resources/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-26 21:42:32.000000 nefile-0.9.0/nefile/resources/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:42:43.765614 nefile-0.9.0/nefile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-26 21:42:43.000000 nefile-0.9.0/nefile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 21:42:43.000000 nefile-0.9.0/nefile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:42:43.000000 nefile-0.9.0/nefile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:42:43.000000 nefile-0.9.0/nefile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 21:42:43.000000 nefile-0.9.0/nefile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-26 21:42:32.000000 nefile-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:42:43.765614 nefile-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:42:32.000000 nefile-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:12:31.268587 nefile-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 14:12:21.000000 nefile-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-12 14:12:31.268587 nefile-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-12 14:12:21.000000 nefile-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:12:31.268587 nefile-0.9.1/nefile/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 14:12:21.000000 nefile-0.9.1/nefile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-12 14:12:21.000000 nefile-0.9.1/nefile/nefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-12 14:12:21.000000 nefile-0.9.1/nefile/resource_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:12:31.268587 nefile-0.9.1/nefile/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:12:21.000000 nefile-0.9.1/nefile/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-12 14:12:21.000000 nefile-0.9.1/nefile/resources/application_defined_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-12 14:12:21.000000 nefile-0.9.1/nefile/resources/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-12 14:12:21.000000 nefile-0.9.1/nefile/resources/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-12 14:12:21.000000 nefile-0.9.1/nefile/resources/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-12 14:12:21.000000 nefile-0.9.1/nefile/resources/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:12:31.268587 nefile-0.9.1/nefile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-12 14:12:31.000000 nefile-0.9.1/nefile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-12 14:12:31.000000 nefile-0.9.1/nefile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:12:31.000000 nefile-0.9.1/nefile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 14:12:31.000000 nefile-0.9.1/nefile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 14:12:31.000000 nefile-0.9.1/nefile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-12 14:12:21.000000 nefile-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:12:31.268587 nefile-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:12:21.000000 nefile-0.9.1/setup.py
```

### Comparing `nefile-0.9.0/LICENSE` & `nefile-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nefile-0.9.0/PKG-INFO` & `nefile-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nefile
-Version: 0.9.0
+Version: 0.9.1
 Summary: Parse 16-bit New Executable (NE) programs.
 Author: npjg
 License: MIT License
         
         Copyright (c) 2022 Nathanael Gentry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,20 +30,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Like its namesake [`pefile`](https://github.com/erocarrera/pefile) does for the modern Portable Executable format, this `nefile` library parses the ancient 16-bit New Executable (NE) format.I
+Like its namesake [`pefile`](https://github.com/erocarrera/pefile) does for the modern Portable Executable format, this `nefile` library parses the ancient 16-bit New Executable (NE) format. 
 I drafted this library because here are not many good cross-platform tools for analyzing and extracting data (more than just code) from NE files. For instance, Ghidra is great at decompilation but not really at resources. This library fills that gap. Also, I just love Windows 3.1.
 
-Currently there is read-only support for the NE header and resources, as that's all I need at the moment. Feel free to contribute if you need other functionality!
+Currently there is read-only support for the NE header and resources, as that's all I need at the moment. Feel free to contribute if you need other functionality from Python!
 
-## Example Usage
+## Installation
+Get it [on PyPI](https://pypi.org/project/nefile/): ```pip3 install nefile```
+
+## Usage
 
 ```python
 import nefile
 from nefile.resource_table import ResourceType
 
 # OPEN THE WINDOWS 3.1 PROGRAM MANAGER.
 progman = nefile.NE('/media/windows-3.1/WINDOWS/PROGMAN.EXE')
```

### Comparing `nefile-0.9.0/README.md` & `nefile-0.9.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-Like its namesake [`pefile`](https://github.com/erocarrera/pefile) does for the modern Portable Executable format, this `nefile` library parses the ancient 16-bit New Executable (NE) format.I
+Like its namesake [`pefile`](https://github.com/erocarrera/pefile) does for the modern Portable Executable format, this `nefile` library parses the ancient 16-bit New Executable (NE) format. 
 I drafted this library because here are not many good cross-platform tools for analyzing and extracting data (more than just code) from NE files. For instance, Ghidra is great at decompilation but not really at resources. This library fills that gap. Also, I just love Windows 3.1.
 
-Currently there is read-only support for the NE header and resources, as that's all I need at the moment. Feel free to contribute if you need other functionality!
+Currently there is read-only support for the NE header and resources, as that's all I need at the moment. Feel free to contribute if you need other functionality from Python!
 
-## Example Usage
+## Installation
+Get it [on PyPI](https://pypi.org/project/nefile/): ```pip3 install nefile```
+
+## Usage
 
 ```python
 import nefile
 from nefile.resource_table import ResourceType
 
 # OPEN THE WINDOWS 3.1 PROGRAM MANAGER.
 progman = nefile.NE('/media/windows-3.1/WINDOWS/PROGMAN.EXE')
```

### Comparing `nefile-0.9.0/nefile/nefile.py` & `nefile-0.9.1/nefile/nefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(self, stream):
         # READ THE NE HEADER START OFFSET.
         stream.seek(0x3c)
         self.ne_header_offset = struct.unpack.uint16_le(stream)
 
 ## Models a New Executable file.
 class NE:
-    def __init__(self, filepath: str = None, stream = None):
+    def __init__(self, filepath: str = None, stream = None, user_defined_resource_parsers = {}):
         # MAP THE FILE DATA.
         # A filepath can be provided to open a file from disk, or an in-memory binary stream can be provided.
         # However, providing both of these is an error.
         # First, we see if the data sources are ambiguous.
         more_than_one_data_source_provided: bool = filepath is not None and stream is not None
         if more_than_one_data_source_provided:
             raise ValueError('A filepath and a stream cannot both be provided to define a stream.' 
@@ -45,24 +45,24 @@
         # READ THE NE HEADER.
         # This is sometimes calld a Windows header, 
         # but it could be for another platform too.
         self.header = NEHeader(self.stream)
 
         # READ THE RESOURCE TABLE.
         self.stream.seek(self.header.resource_table_offset)
-        self.resource_table = resource_table.ResourceTable(self.stream)
+        self.resource_table = resource_table.ResourceTable(self.stream, user_defined_resource_parsers)
 
     @property
     def executable_name(self):
         return os.path.split(self.filepath)[1]
 
     ## Exports all the resources in this executable.
     def export_resources(self, directory_path):
         for resource_type_code, resource_type in self.resource_table.resources.items():
-            resource_type_string: str = resource_type_code.name if isinstance(resource_type_code, resource_table.ResourceType) else resource_type_code
+            resource_type_string: str = resource_type_code.name if isinstance(resource_type_code, Enum) else resource_type_code
             for resource_id, resource in resource_type.items():
                 export_filename = f'{self.executable_name}-{resource_type_string}-{resource_id}'
                 export_filepath = os.path.join(directory_path, export_filename)
                 resource.export(export_filepath)
 
 ## Models an NE header. This is sometimes called a "Windows header",
 ## but that is not quite correct as other platforms like OS/2 can use this header too.
```

### Comparing `nefile-0.9.0/nefile/resource_table.py` & `nefile-0.9.1/nefile/resource_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import dataclass
 import resource
 import self_documenting_struct as struct
 from enum import Enum, IntFlag
 
 from .resources.bitmap import Bitmap
 from .resources.icon import GroupIcon, Icon
+from .resources.cursor import Cursor
 from .resources.application_defined_data import ApplicationDefinedData
 from .resources.string import StringTable
 
 ## I did not know exactly what the NE resource types are,
 ## so I copied the relevant ones from the Win32 documentation:
 ## https://learn.microsoft.com/en-us/windows/win32/menurc/resource-types.
 class ResourceType(Enum):
@@ -30,19 +31,40 @@
     RT_VERSION = 16
 
     ## Returns true if the provided value is in this enum; False otherwise. 
     @classmethod
     def has_value(cls, value):
         return value in (val.value for val in cls.__members__.values())
 
-## The resource table follows the segment table and contains entries 
-## for each resource type and resource in this NE stream.
-## Resource data itself is lazily loaded; the resources are only loaded when requested.
+
+## Declares each of the resource types and resources in this NE stream.
+## The resource declarations are read immediately, but the resource data 
+## is only parsed when requested.
 class ResourceTable:
-    def __init__(self, stream):
+    BUILT_IN_RESOURCE_PARSERS = {
+        ResourceType.RT_CURSOR: Cursor,
+        ResourceType.RT_GROUP_ICON: GroupIcon,
+        ResourceType.RT_STRING: StringTable
+    }
+
+    ## Reads a resource table from a binary stream.
+    ## \param[in] stream - The binary stream positioned at the resource table start.
+    ## \param[in] user_defined_resource_parsers - A dict that maps resource type IDs
+    ##            to resource parser classes.
+    def __init__(self, stream, user_defined_resource_parsers):
+        # DEFINE THE RESOURCE PARSERS.
+        # TODO: Support more built-in resources.
+        self.resource_parsers = {
+            ResourceType.RT_CURSOR: Cursor,
+            ResourceType.RT_GROUP_ICON: GroupIcon,
+            ResourceType.RT_STRING: StringTable
+        }
+        self.resource_parsers.update(user_defined_resource_parsers)
+    
+        # READ THE RESORUCE METADATA.
         self.stream = stream
         self._resources = None
         self.resource_table_start_offset = stream.tell()
         # The shift count is the an exponent of 2 (left shift),
         # for calculating start offsets and lengths of resource data.
         self.alignment_shift_count = struct.unpack.uint16_le(stream)
 
@@ -50,88 +72,78 @@
         self.resource_type_tables = {}
         resource_type = ResourceTypeTable(stream, self.alignment_shift_count, self.resource_table_start_offset)
         while not resource_type.is_end_flag:
             resource_dictionary_key = ResourceType(resource_type.type_code) if ResourceType.has_value(resource_type.type_code) else resource_type.type_code
             self.resource_type_tables.update({resource_dictionary_key: resource_type})
             resource_type = ResourceTypeTable(stream, self.alignment_shift_count, self.resource_table_start_offset)
 
+    ## Parses the resources in this resource table.
+    ## The resources are always parsed in this order:
+    ##  - Built-in types (ResourceType) in numerical order.
+    ##  - All other types in the order they appear in the file.
+    ##
+    ## This ordering helps resolve dependencies within and among
+    ## these groups. Built-in types with higher numerical order (like
+    ## RT_GROUPICON) can depend on built-in types with lower numerical
+    ## order (like RT_ICON). And user-defined types can depend on built-
+    ## in types, and so forth.
+    ##
+    ## Built-in and user-defined types are parsed with the provided classes,
+    ## any any other types have raw resource data read for processing later.
     @property
     def resources(self):
+        # CHECK IF THE RESOURCES HAVE PREVIOUSLY BEEN PARSED.
+        # Parsing resources can be expensive, so we cache the
+        # parsing results after parsing the first time.
         if self._resources is not None:
             # RETURN THE CACHED RESOURCE DICTIONARY.
             return self._resources
+        self._resources = {}
 
-        # PROCESS RESOURCE TYPES THAT REQUIRE PRE-PROCESSING.
-        # These resource types must be in the resource dictionary
-        # since they might be referenced at any time by group resources,
-        # and it is not guaranteed that group resources are read before 
-        # the individual resources.
-        self._resources = {
-            ResourceType.RT_ICON: self._parse_icons(),
-            ResourceType.RT_CURSOR: self._parse_cursors()
-        }
+        # PARSE RESOURCES FROM THE BUILT-IN RESOURCE TYPES.
+        # This loop guarantees the resource types are processed in definition order.
+        for resource_type in ResourceType:
+            resource_type_table = self.resource_type_tables.get(resource_type)
+            if resource_type_table is not None:
+                resources = self._parse_resources(resource_type_table)
+                self._resources.update({resource_type_table.type_code: resources})
 
+        # PARSE RESOURCES FROM ALL OTHER RESOURCE TYPES.
+        # THese resource types are processed as they appear in the file.
         for resource_type_table in self.resource_type_tables.values():
-            resource_pre_parsed = resource_type_table.type_code == ResourceType.RT_ICON or \
-                resource_type_table.type_code == ResourceType.RT_CURSOR
-            if resource_pre_parsed:
-                continue
-
-            # PARSE THE RESOURCES OF THIS TYPE.
-            current_type_resources = {}
-            for resource_declaration in resource_type_table.resource_declarations:
-                # PARSE THIS INDIVIDUAL RESOURCE.
-                resource = self._parse_other_resource(resource_declaration, resource_type_table.type_code)
-                current_type_resources.update({resource_declaration.id: resource})
+            resource_already_parsed = ResourceType.has_value(resource_type_table.type_code)
+            if not resource_already_parsed:
+                resources = self._parse_resources(resource_type_table)
+                self._resources.update({resource_type_table.type_code: resources})
 
-            self._resources.update({resource_type_table.type_code: current_type_resources})
+        # RETURN THE PARSED RESOURCES.
         return self._resources
 
-    ## Finds a resource by 
+    ## Passes the actual data referenced by each resource declaration
+    ## to the appropriate parsing class and returns the result.
+    def _parse_resources(self, resource_type_table):
+        # GET THE PARSER CLASS FOR THIS RESOURCE TYPE.
+        defined_resource_parser = self.resource_parsers.get(resource_type_table.type_code, ApplicationDefinedData)
+
+        # PARSE THE RESOURCES OF THIS TYPE.
+        resources = {}
+        for resource_declaration in resource_type_table.resource_declarations:
+            self.stream.seek(resource_declaration.data_start_offset)
+            resource = defined_resource_parser(self.stream, resource_declaration, self)
+            resources.update({resource_declaration.id: resource})
+        return resources
+
+    ## Finds a resource by its type and resource ID.
+    ## The type is required because two resources with different types
+    ## can have the same resource ID.
     def find_resource_by_id(self, resource_id, type_id):
         return self.resources.get(type_id, {}).get(resource_id, None)
 
-    ## Constructs the icons in this resource table.
-    ## These must be constructed first because the group resources refer to them.
-    def _parse_icons(self):
-        icon_resource_type_table = self.resource_type_tables.get(ResourceType.RT_ICON, None)
-        icon_resources = {}
-        if icon_resource_type_table is None:
-            return icon_resources
-
-        for resource_declaration in icon_resource_type_table.resource_declarations:
-            self.stream.seek(resource_declaration.data_start_offset)
-            icon = Icon(self.stream, resource_declaration, self)
-            icon_resources.update({resource_declaration.id: icon})
-        return icon_resources
-
-    def _parse_cursors(self):
-        cursor_resource_type_table = self.resource_type_tables.get(ResourceType.RT_CURSOR, None)
-        cursor_resources = {}
-        if cursor_resource_type_table is None:
-            return cursor_resources
-
-        for resource_declaration in cursor_resource_type_table.resource_declarations:
-            self.stream.seek(resource_declaration.data_start_offset)
-            cursor = Cursor(self.stream, resource_declaration, self)
-            cursor_resources.update({resource_declaration.id: cursor})
-        return cursor_resources
-
-    def _parse_other_resource(self, resource_declaration, resource_type_code):
-        self.stream.seek(resource_declaration.data_start_offset)
-        if resource_type_code == ResourceType.RT_BITMAP:
-            return Bitmap(self.stream, resource_declaration, self)
-        elif resource_type_code == ResourceType.RT_GROUP_ICON:
-            return GroupIcon(self.stream, resource_declaration, self)
-        elif resource_type_code == ResourceType.RT_STRING:
-            return StringTable(self.stream, resource_declaration, self)
-        else:
-            return ApplicationDefinedData(self.stream, resource_declaration, self)
-
-## Declares each of the resource types stored in this stream,
+## Declares each of the resource types stored in this stream.
+## Resource data is not actually accessible until the resources are parsed.
 class ResourceTypeTable:
     def __init__(self, stream, alignment_shift_count, resource_table_start_offset):
         # READ THE RESOURCE TYPE INFORMATION.
         # There must be one resource type info entry for each type
         # of resource in the executable stream.
         #
         # This is an integer type if the high-order bit is 
@@ -158,15 +170,16 @@
         resource_count = struct.unpack.uint16_le(stream)
         # TODO: Document this, if it can be documented.
         self.reserved = stream.read(4)
         for index in range(resource_count):
             resource_declaration = ResourceDeclaration(stream, alignment_shift_count, resource_table_start_offset)
             self.resource_declarations.append(resource_declaration)
 
-## Reads a resource stored in the stream.
+## Declares a resource stored in the stream.
+## Resource data is not actually accessible until the resources are parsed.
 class ResourceDeclaration:
     class ResourceFlags(IntFlag):
         MOVEABLE = 0x0010,
         PURE = 0x0020,
         # If the resource is not preloaded, it is loaded on demand.
         PRELOAD = 0x0040
 
@@ -191,14 +204,18 @@
             # This specifies the offset in bytes, relative to the start of the resource table,
             # where the string name for this type can be found.
             id_string_offset_from_file_start = resource_table_start_offset + raw_id_data
             self.id = ResourceString(stream, id_string_offset_from_file_start).string
         # TODO: Document this, if it can be documented.
         self.reserved = stream.read(4)
 
+    @property
+    def data_end_offset(self):
+        return self.data_start_offset + self.resource_length_in_bytes
+
 ## Reads a resource name or type string by seeking to the correct offset.
 ## These strings are Pascal strings - case-sensitive and not null-terminated.
 class ResourceString:
     def __init__(self, stream, offset_from_stream_start):
         saved_stream_position = stream.tell()
         stream.seek(offset_from_stream_start)
         string_length = struct.unpack.uint8(stream)
```

### Comparing `nefile-0.9.0/nefile/resources/application_defined_data.py` & `nefile-0.9.1/nefile/resources/application_defined_data.py`

 * *Files identical despite different names*

### Comparing `nefile-0.9.0/nefile/resources/bitmap.py` & `nefile-0.9.1/nefile/resources/bitmap.py`

 * *Files identical despite different names*

### Comparing `nefile-0.9.0/nefile/resources/cursor.py` & `nefile-0.9.1/nefile/resources/cursor.py`

 * *Files identical despite different names*

### Comparing `nefile-0.9.0/nefile/resources/icon.py` & `nefile-0.9.1/nefile/resources/icon.py`

 * *Files identical despite different names*

### Comparing `nefile-0.9.0/nefile/resources/string.py` & `nefile-0.9.1/nefile/resources/string.py`

 * *Files identical despite different names*

### Comparing `nefile-0.9.0/nefile.egg-info/PKG-INFO` & `nefile-0.9.1/nefile.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nefile
-Version: 0.9.0
+Version: 0.9.1
 Summary: Parse 16-bit New Executable (NE) programs.
 Author: npjg
 License: MIT License
         
         Copyright (c) 2022 Nathanael Gentry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,20 +30,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Like its namesake [`pefile`](https://github.com/erocarrera/pefile) does for the modern Portable Executable format, this `nefile` library parses the ancient 16-bit New Executable (NE) format.I
+Like its namesake [`pefile`](https://github.com/erocarrera/pefile) does for the modern Portable Executable format, this `nefile` library parses the ancient 16-bit New Executable (NE) format. 
 I drafted this library because here are not many good cross-platform tools for analyzing and extracting data (more than just code) from NE files. For instance, Ghidra is great at decompilation but not really at resources. This library fills that gap. Also, I just love Windows 3.1.
 
-Currently there is read-only support for the NE header and resources, as that's all I need at the moment. Feel free to contribute if you need other functionality!
+Currently there is read-only support for the NE header and resources, as that's all I need at the moment. Feel free to contribute if you need other functionality from Python!
 
-## Example Usage
+## Installation
+Get it [on PyPI](https://pypi.org/project/nefile/): ```pip3 install nefile```
+
+## Usage
 
 ```python
 import nefile
 from nefile.resource_table import ResourceType
 
 # OPEN THE WINDOWS 3.1 PROGRAM MANAGER.
 progman = nefile.NE('/media/windows-3.1/WINDOWS/PROGMAN.EXE')
```

### Comparing `nefile-0.9.0/pyproject.toml` & `nefile-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nefile"
-version = "0.9.0"
+version = "0.9.1"
 description = "Parse 16-bit New Executable (NE) programs."
 readme = "README.md"
 authors = [{ name = "npjg" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

