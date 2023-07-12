# Comparing `tmp/flatdata-py-0.4.5.tar.gz` & `tmp/flatdata-py-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatdata-py-0.4.5.tar", last modified: Thu Dec 16 15:56:36 2021, max compression
+gzip compressed data, was "flatdata-py-0.4.6.tar", last modified: Wed Jul 12 08:02:44 2023, max compression
```

## Comparing `flatdata-py-0.4.5.tar` & `flatdata-py-0.4.6.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxrwxr-x   0 cvetter   (1000) cvetter   (1000)        0 2021-12-16 15:56:36.730279 flatdata-py-0.4.5/
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2461 2021-12-16 15:56:36.730279 flatdata-py-0.4.5/PKG-INFO
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2023 2021-10-12 06:27:15.000000 flatdata-py-0.4.5/README.md
-drwxrwxr-x   0 cvetter   (1000) cvetter   (1000)        0 2021-12-16 15:56:36.730279 flatdata-py-0.4.5/flatdata/
-drwxrwxr-x   0 cvetter   (1000) cvetter   (1000)        0 2021-12-16 15:56:36.730279 flatdata-py-0.4.5/flatdata/lib/
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)      217 2021-08-13 15:24:40.000000 flatdata-py-0.4.5/flatdata/lib/__init__.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     4665 2020-02-23 17:08:36.000000 flatdata-py-0.4.5/flatdata/lib/archive.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)    10023 2021-08-13 15:24:40.000000 flatdata-py-0.4.5/flatdata/lib/archive_builder.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2297 2021-08-13 15:24:40.000000 flatdata-py-0.4.5/flatdata/lib/data_access.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     3624 2021-08-13 15:24:40.000000 flatdata-py-0.4.5/flatdata/lib/errors.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     1134 2021-10-12 06:27:15.000000 flatdata-py-0.4.5/flatdata/lib/file_resource_storage.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     1513 2021-08-13 15:24:40.000000 flatdata-py-0.4.5/flatdata/lib/file_resource_writer.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2621 2021-08-13 15:24:40.000000 flatdata-py-0.4.5/flatdata/lib/flatdata_writer.py
--rwxrwxr-x   0 cvetter   (1000) cvetter   (1000)     3831 2021-10-12 06:27:15.000000 flatdata-py-0.4.5/flatdata/lib/inspector.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     3808 2021-08-13 15:24:40.000000 flatdata-py-0.4.5/flatdata/lib/resource_storage.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     6122 2021-11-29 12:45:23.000000 flatdata-py-0.4.5/flatdata/lib/resources.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2256 2020-02-23 17:08:36.000000 flatdata-py-0.4.5/flatdata/lib/structure.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     3652 2021-10-12 06:27:15.000000 flatdata-py-0.4.5/flatdata/lib/tar_archive_resource_storage.py
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     1670 2021-08-13 15:24:40.000000 flatdata-py-0.4.5/flatdata/lib/writer.py
-drwxrwxr-x   0 cvetter   (1000) cvetter   (1000)        0 2021-12-16 15:56:36.730279 flatdata-py-0.4.5/flatdata_py.egg-info/
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2461 2021-12-16 15:56:36.000000 flatdata-py-0.4.5/flatdata_py.egg-info/PKG-INFO
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)      663 2021-12-16 15:56:36.000000 flatdata-py-0.4.5/flatdata_py.egg-info/SOURCES.txt
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)        1 2021-12-16 15:56:36.000000 flatdata-py-0.4.5/flatdata_py.egg-info/dependency_links.txt
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)      132 2021-12-16 15:56:36.000000 flatdata-py-0.4.5/flatdata_py.egg-info/entry_points.txt
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)       60 2021-12-16 15:56:36.000000 flatdata-py-0.4.5/flatdata_py.egg-info/requires.txt
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)        9 2021-12-16 15:56:36.000000 flatdata-py-0.4.5/flatdata_py.egg-info/top_level.txt
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)      103 2021-12-16 15:54:42.000000 flatdata-py-0.4.5/pyproject.toml
--rw-rw-r--   0 cvetter   (1000) cvetter   (1000)       38 2021-12-16 15:56:36.730279 flatdata-py-0.4.5/setup.cfg
--rwxrwxr-x   0 cvetter   (1000) cvetter   (1000)     1201 2021-12-16 12:31:13.000000 flatdata-py-0.4.5/setup.py
+drwxrwxr-x   0 cvetter   (1000) cvetter   (1000)        0 2023-07-12 08:02:44.182093 flatdata-py-0.4.6/
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2424 2023-07-12 08:02:44.182093 flatdata-py-0.4.6/PKG-INFO
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2023 2021-10-12 06:27:15.000000 flatdata-py-0.4.6/README.md
+drwxrwxr-x   0 cvetter   (1000) cvetter   (1000)        0 2023-07-12 08:02:44.178093 flatdata-py-0.4.6/flatdata/
+drwxrwxr-x   0 cvetter   (1000) cvetter   (1000)        0 2023-07-12 08:02:44.178093 flatdata-py-0.4.6/flatdata/lib/
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)      217 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/flatdata/lib/__init__.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     4665 2023-05-31 09:14:23.000000 flatdata-py-0.4.6/flatdata/lib/archive.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)    10023 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/flatdata/lib/archive_builder.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2297 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/flatdata/lib/data_access.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     3624 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/flatdata/lib/errors.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     1134 2021-10-12 06:27:15.000000 flatdata-py-0.4.6/flatdata/lib/file_resource_storage.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     1513 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/flatdata/lib/file_resource_writer.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2621 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/flatdata/lib/flatdata_writer.py
+-rwxrwxr-x   0 cvetter   (1000) cvetter   (1000)     3831 2021-10-12 06:27:15.000000 flatdata-py-0.4.6/flatdata/lib/inspector.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     3808 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/flatdata/lib/resource_storage.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     7669 2023-05-31 09:14:23.000000 flatdata-py-0.4.6/flatdata/lib/resources.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2256 2020-02-23 17:08:36.000000 flatdata-py-0.4.6/flatdata/lib/structure.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2386 2023-05-31 09:14:23.000000 flatdata-py-0.4.6/flatdata/lib/tar_archive_resource_storage.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     1670 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/flatdata/lib/writer.py
+drwxrwxr-x   0 cvetter   (1000) cvetter   (1000)        0 2023-07-12 08:02:44.178093 flatdata-py-0.4.6/flatdata_py.egg-info/
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2424 2023-07-12 08:02:44.000000 flatdata-py-0.4.6/flatdata_py.egg-info/PKG-INFO
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)      825 2023-07-12 08:02:44.000000 flatdata-py-0.4.6/flatdata_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)        1 2023-07-12 08:02:44.000000 flatdata-py-0.4.6/flatdata_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)      131 2023-07-12 08:02:44.000000 flatdata-py-0.4.6/flatdata_py.egg-info/entry_points.txt
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)       60 2023-07-12 08:02:44.000000 flatdata-py-0.4.6/flatdata_py.egg-info/requires.txt
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)        9 2023-07-12 08:02:44.000000 flatdata-py-0.4.6/flatdata_py.egg-info/top_level.txt
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)      103 2022-01-12 07:45:12.000000 flatdata-py-0.4.6/pyproject.toml
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)       38 2023-07-12 08:02:44.182093 flatdata-py-0.4.6/setup.cfg
+-rwxrwxr-x   0 cvetter   (1000) cvetter   (1000)     1201 2023-07-12 08:02:16.000000 flatdata-py-0.4.6/setup.py
+drwxrwxr-x   0 cvetter   (1000) cvetter   (1000)        0 2023-07-12 08:02:44.182093 flatdata-py-0.4.6/tests/
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     5359 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/tests/test_archive_creation.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     2198 2020-02-23 17:08:36.000000 flatdata-py-0.4.6/tests/test_archive_validation.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     3717 2023-05-31 09:14:23.000000 flatdata-py-0.4.6/tests/test_backward_compatibility.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)   215926 2021-08-13 15:24:40.000000 flatdata-py-0.4.6/tests/test_data_access.py
+-rw-rw-r--   0 cvetter   (1000) cvetter   (1000)     1304 2021-10-12 06:27:15.000000 flatdata-py-0.4.6/tests/test_tar_resource_storage.py
```

### Comparing `flatdata-py-0.4.5/PKG-INFO` & `flatdata-py-0.4.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: flatdata-py
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python 3 implementation of Flatdata
 Home-page: https://github.com/heremaps/flatdata
 Author: Flatdata Developers
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: inspector
 
 # flatdata-py
@@ -71,9 +69,7 @@
 
 * if you want to install flatdata-py:
 
 ```sh
 pip3 install flatdata-py[writer]
 flatdata-writer --schema archive.flatdata --output-dir testdir --json-file data.json --resource-name resourcename
 ```
-
-
```

### Comparing `flatdata-py-0.4.5/README.md` & `flatdata-py-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/archive.py` & `flatdata-py-0.4.6/flatdata/lib/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,11 +113,11 @@
             if resource:
                 resource.__doc__ = resource_signature.doc
                 return resource
         return None
 
     @staticmethod
     def _check_non_subarchive_schema(name, resource_signature, storage):
-        actual_schema = storage.read().decode()
+        actual_schema = bytes(storage).decode()
         if actual_schema != resource_signature.schema:
             raise SchemaMismatchError(
                 name, resource_signature.schema.splitlines(), actual_schema.splitlines())
```

### Comparing `flatdata-py-0.4.5/flatdata/lib/archive_builder.py` & `flatdata-py-0.4.6/flatdata/lib/archive_builder.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/data_access.py` & `flatdata-py-0.4.6/flatdata/lib/data_access.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/errors.py` & `flatdata-py-0.4.6/flatdata/lib/errors.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/file_resource_storage.py` & `flatdata-py-0.4.6/flatdata/lib/file_resource_storage.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/file_resource_writer.py` & `flatdata-py-0.4.6/flatdata/lib/file_resource_writer.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/flatdata_writer.py` & `flatdata-py-0.4.6/flatdata/lib/flatdata_writer.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/inspector.py` & `flatdata-py-0.4.6/flatdata/lib/inspector.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/resource_storage.py` & `flatdata-py-0.4.6/flatdata/lib/resource_storage.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/resources.py` & `flatdata-py-0.4.6/flatdata/lib/resources.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
- Copyright (c) 2017 HERE Europe B.V.
+ Copyright (c) 2023 HERE Europe B.V.
  See the LICENSE file in the root of this project for license details.
 '''
 
 import json
 
 import pandas as pd
 import numpy as np
@@ -16,15 +16,15 @@
 SIZE_PADDING_IN_BYTES = 8
 
 
 class ResourceBase:
     def __init__(self, mem, element_type):
         if len(mem) < (SIZE_OFFSET_IN_BYTES + SIZE_PADDING_IN_BYTES):
             raise CorruptResourceError()
-        self._mem = mem
+        self._mem = memoryview(mem)
         self._element_type = element_type
         self._element_types = [element_type]
         self._type_size_in_bytes = self._element_type._SIZE_IN_BYTES if self._element_type else 1
 
     def size_in_bytes(self):
         return len(self._mem)
 
@@ -62,15 +62,15 @@
     def to_numpy(self, limit=None):
         indices = self._slice.indices(len(self._sequence))
         num_items = len(range(*indices)) if not limit else limit
         result = np.empty(
             shape=num_items,
             dtype=self._sequence._element_type.dtype()
         )
-        for index, item in self:
+        for index, item in enumerate(self):
             result[index] = item.as_tuple()
         return result
 
     def to_data_frame(self, limit=None):
         return pd.DataFrame(data=self.to_numpy(limit))
 
     def __iter__(self):
@@ -98,48 +98,65 @@
     def __getitem__(self, index):
         if isinstance(index, slice):
             return _VectorSlice(index, self)
 
         if index < 0:
             index += len(self)
         if index >= self._size or index < 0:
-            raise IndexError("Vector access out of bounds")
+            raise IndexError("Vector access out of bounds: " + str(index))
         return self._get_item(index)
 
     def __iter__(self):
         for i in range(len(self)):
             yield self._get_item(i)
 
     def __getattr__(self, name):
         return pd.DataFrame(data=[[getattr(item, name)] for item in self], columns=[name])
 
     def __len__(self):
         return self._size
 
 
+class _MultivectorSlice:
+    def __init__(self, s, sequence):
+        self._slice = s
+        self._sequence = sequence
+
+    def __iter__(self):
+        for i in range(*self._slice.indices(len(self._sequence))):
+            yield self._sequence[i]
+
+    def __repr__(self):
+        return [x for x in self].__repr__()
+
+
 class Multivector(ResourceBase):
     def __init__(self, index_mem, mem, index_type, *element_types):
         self._index = Vector(index_mem, index_type)
         self._mem = mem
         self._element_types = element_types
         self._index_type = index_type
 
     @classmethod
     def open(cls, storage, name, initializer, is_optional=False):
         return cls(storage.get(name + "_index", is_optional),
                    storage.get(name, is_optional),
                    *initializer)
 
     def __len__(self):
-        return len(self._index)
+        # The last entry is just a sentinel
+        return max(0, len(self._index) - 1)
 
     def _bucket_offset(self, index):
         return self._index[index].value + SIZE_OFFSET_IN_BYTES
 
     def __getitem__(self, index):
+        if isinstance(index, slice):
+            return _MultivectorSlice(index, self)
+
         offset = self._bucket_offset(index)
         next_offset = self._bucket_offset(index + 1)
         elements = []
         while offset < next_offset:
             type_index = read_value(self._mem, offset * 8, 8, False)
             offset += 1
             element_type = self._element_types[type_index]
@@ -167,14 +184,40 @@
             return self._mem[
                 slice(item.start + SIZE_OFFSET_IN_BYTES,
                       (item.stop + SIZE_OFFSET_IN_BYTES) if item.stop is not None else None,
                       item.step)
             ]
         return self._mem[item + SIZE_OFFSET_IN_BYTES:item + SIZE_OFFSET_IN_BYTES + 1]
 
+    def sub_str(self, index, separator = b'\0'):
+        for i in range(index, len(self)):
+            if self[i:i + len(separator)] == separator:
+                return bytes(self[index:i]).decode("utf-8")
+        return bytes(self[index]).decode("utf-8")
+
+    def sub_str_list(self, index, separator = b'\0', list_separator = b'\0\0'):
+        result = []
+        for i in range(index, len(self)):
+            if index == i and self[i:i + len(list_separator)] == list_separator:
+                break
+            if self[i:i + len(separator)] == separator:
+                result.append(bytes(self[index:i]).decode("utf-8"))
+                index = i + 1
+        return result
+
+    def sub_str_array(self, index, size, separator = b'\0'):
+        result = []
+        for i in range(index, len(self)):
+            if self[i:i + len(separator)] == separator:
+                result.append(bytes(self[index:i]).decode("utf-8"))
+                index = i + 1
+                if len(result) == size:
+                    break
+        return result
+
 
 class Instance(ResourceBase):
     def __getitem__(self, index):
         if isinstance(index, slice):
             raise IndexError("Instance has only one item")
 
         if index < 0:
```

### Comparing `flatdata-py-0.4.5/flatdata/lib/structure.py` & `flatdata-py-0.4.6/flatdata/lib/structure.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata/lib/tar_archive_resource_storage.py` & `flatdata-py-0.4.6/flatdata/lib/tar_archive_resource_storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.tar_map = tar_map
         self.file_entries = file_entries
         self.dir_entries = dir_entries
         self.sub_path = sub_path
 
     @classmethod
     def create(cls, tar_path, sub_path=""):
-        tar_map = FileResourceStorage.memory_map(tar_path)
+        tar_map = memoryview(FileResourceStorage.memory_map(tar_path))
         file_entries = dict()
         dir_entries = set()
         with tarfile.open(tar_path, "r:") as tar:
             for file in tar:
                 name = file.name
                 if name.startswith("./"):
                     name = name[2:]
@@ -40,15 +40,15 @@
 
         return cls(tar_map, file_entries, dir_entries, sub_path)
 
     def get(self, key, is_optional=False):
         path = self._path(key)
         if path in self.file_entries:
             (offset, length) = self.file_entries[path]
-            return MemoryMapSection(self.tar_map, offset, length)
+            return self.tar_map[offset:offset + length]
 
         if path in self.dir_entries:
             return TarArchiveResourceStorage(self.tar_map, self.file_entries, self.dir_entries, path)
 
         if not is_optional:
             raise MissingResourceError(key)
         else:
@@ -66,47 +66,7 @@
         return entries
 
     def _path(self, key):
         if not self.sub_path:
             return key
         else:
             return self.sub_path + '/' + key
-
-
-class MemoryMapSection:
-    """
-    Represent a slice of a memory mapped file.
-    Keeps track of its position, as to emulate pointing to a dedicated file.
-    """
-
-    def __init__(self, inner, offset, length):
-        self.inner = inner
-        self.offset = offset
-        self.length = length;
-        self.pos = 0
-
-    def __len__(self):
-        return self.size()
-
-    def __getitem__(self, key):
-        if isinstance(key, slice):
-            start = key.start if key.start is not None else 0
-            start = self.offset + min(start, self.length)
-            stop = key.stop if key.stop is not None else self.length
-            stop = self.offset + min(stop, self.length)
-            return self.inner[slice(start, stop, key.step)]
-        else:
-            if key < self.length:
-                return self.inner.__getitem__(self.offset + key)
-            else:
-                raise IndexError('index out of range')
-
-    def read(self, n=None):
-        if n is None:
-            n = self.length - self.pos
-        self.inner.seek(self.offset + self.pos)
-        data = self.inner.read(min(n, self.length - self.pos))
-        self.pos += len(data)
-        return data
-
-    def size(self):
-        return min(self.length, self.inner.size() - self.offset)
```

### Comparing `flatdata-py-0.4.5/flatdata/lib/writer.py` & `flatdata-py-0.4.6/flatdata/lib/writer.py`

 * *Files identical despite different names*

### Comparing `flatdata-py-0.4.5/flatdata_py.egg-info/PKG-INFO` & `flatdata-py-0.4.6/flatdata_py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: flatdata-py
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python 3 implementation of Flatdata
 Home-page: https://github.com/heremaps/flatdata
 Author: Flatdata Developers
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: inspector
 
 # flatdata-py
@@ -71,9 +69,7 @@
 
 * if you want to install flatdata-py:
 
 ```sh
 pip3 install flatdata-py[writer]
 flatdata-writer --schema archive.flatdata --output-dir testdir --json-file data.json --resource-name resourcename
 ```
-
-
```

### Comparing `flatdata-py-0.4.5/setup.py` & `flatdata-py-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from setuptools import find_packages, setup
 
 SOURCE_FILEPATH = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name="flatdata-py",
-    version="0.4.5",
+    version="0.4.6",
     author="Flatdata Developers",
     description="Python 3 implementation of Flatdata",
     long_description=open(os.path.join(SOURCE_FILEPATH, "README.md")).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/heremaps/flatdata",
     # we can't use find_namespace_packages as it is only a very recent addition to setuptools
     packages=["flatdata." + p for p in find_packages("flatdata")],
```

