# Comparing `tmp/quiltcore-0.2.0.tar.gz` & `tmp/quiltcore-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltcore-0.2.0.tar", max compression
+gzip compressed data, was "quiltcore-0.2.1.tar", max compression
```

## Comparing `quiltcore-0.2.0.tar` & `quiltcore-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.2.0/LICENSE
--rw-r--r--   0        0        0     1579 2023-07-06 04:28:48.600645 quiltcore-0.2.0/README.md
--rw-r--r--   0        0        0      852 2023-07-06 05:21:55.381836 quiltcore-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1061 2023-07-05 18:42:27.110229 quiltcore-0.2.0/quiltcore/__init__.py
--rw-r--r--   0        0        0     2937 2023-07-05 20:12:19.916372 quiltcore-0.2.0/quiltcore/changes.py
--rw-r--r--   0        0        0      972 2023-07-05 20:12:59.420575 quiltcore-0.2.0/quiltcore/delta.py
--rw-r--r--   0        0        0     3195 2023-07-06 01:48:32.771447 quiltcore-0.2.0/quiltcore/entry.py
--rw-r--r--   0        0        0     2149 2023-07-06 03:48:54.467767 quiltcore-0.2.0/quiltcore/manifest.py
--rw-r--r--   0        0        0      631 2023-07-06 04:20:34.805585 quiltcore-0.2.0/quiltcore/namespace.py
--rw-r--r--   0        0        0     1621 2023-07-06 04:19:58.111513 quiltcore-0.2.0/quiltcore/registry.py
--rw-r--r--   0        0        0     3402 2023-07-06 04:20:56.858303 quiltcore-0.2.0/quiltcore/resource.py
--rw-r--r--   0        0        0     1937 2023-07-05 23:05:35.899259 quiltcore-0.2.0/quiltcore/resource_key.py
--rw-r--r--   0        0        0     1520 2023-07-05 23:13:46.646052 quiltcore-0.2.0/quiltcore/resource_path.py
--rw-r--r--   0        0        0     4708 2023-07-06 05:18:41.827854 quiltcore-0.2.0/quiltcore/volume.py
--rw-r--r--   0        0        0      693 2023-07-03 20:20:23.166091 quiltcore-0.2.0/quiltcore/yaml/config.py
--rw-r--r--   0        0        0      743 2023-07-06 01:15:21.327702 quiltcore-0.2.0/quiltcore/yaml/quiltcore.yaml
--rw-r--r--   0        0        0      160 2023-06-30 01:13:50.059736 quiltcore-0.2.0/quiltcore/yaml/schema.yaml
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 quiltcore-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1579 2023-07-06 04:28:48.600645 quiltcore-0.2.1/README.md
+-rw-r--r--   0        0        0      852 2023-07-12 20:05:58.181559 quiltcore-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1061 2023-07-05 18:42:27.110229 quiltcore-0.2.1/quiltcore/__init__.py
+-rw-r--r--   0        0        0     2939 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/changes.py
+-rw-r--r--   0        0        0      972 2023-07-05 20:12:59.420575 quiltcore-0.2.1/quiltcore/delta.py
+-rw-r--r--   0        0        0     3172 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/entry.py
+-rw-r--r--   0        0        0     2138 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/manifest.py
+-rw-r--r--   0        0        0      632 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/namespace.py
+-rw-r--r--   0        0        0     1615 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/registry.py
+-rw-r--r--   0        0        0     4050 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/resource.py
+-rw-r--r--   0        0        0     1968 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/resource_key.py
+-rw-r--r--   0        0        0     1525 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/resource_path.py
+-rw-r--r--   0        0        0     4748 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/volume.py
+-rw-r--r--   0        0        0      774 2023-07-12 03:19:19.355733 quiltcore-0.2.1/quiltcore/yaml/config.py
+-rw-r--r--   0        0        0      761 2023-07-12 03:16:11.259596 quiltcore-0.2.1/quiltcore/yaml/quiltcore.yaml
+-rw-r--r--   0        0        0      160 2023-06-30 01:13:50.059736 quiltcore-0.2.1/quiltcore/yaml/schema.yaml
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 quiltcore-0.2.1/PKG-INFO
```

### Comparing `quiltcore-0.2.0/LICENSE` & `quiltcore-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quiltcore-0.2.0/README.md` & `quiltcore-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `quiltcore-0.2.0/pyproject.toml` & `quiltcore-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quiltcore"
-version = "0.2.0"
+version = "0.2.1"
 description = "low-level plubming to read/write Quilt packages"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typing-extensions = "^4.6.3"
```

### Comparing `quiltcore-0.2.0/quiltcore/__init__.py` & `quiltcore-0.2.1/quiltcore/__init__.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.2.0/quiltcore/changes.py` & `quiltcore-0.2.1/quiltcore/changes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
-from upath import UPath
 
+from upath import UPath
 from yaml import dump
 
 from .delta import Delta
 from .manifest import Manifest
 from .resource import Resource
 from .resource_key import ResourceKey
 
@@ -76,15 +76,15 @@
             return
         raise KeyError(f"Key {key} not found in {self.keystore}")
 
     #
     # ResourceKey helper methods
     #
 
-    def child_dict(self, key: str) -> dict:
+    def _child_dict(self, key: str) -> dict:
         """Return the dict for a child resource."""
         delta = self.get_delta(key)
         return {self.kName: [delta.name], self.kPlaces: str(delta.path)}
 
     def get_delta(self, key: str, **kwargs) -> Delta:
         """Return a Delta by key. Raise KeyError if not found."""
         if key in self.keystore:
@@ -92,10 +92,10 @@
         raise KeyError(f"Key {key} not found in {self.keystore}")
 
     def key_path(self, key: str, args: dict = {}) -> Path:
         """Return the Path for a child resource."""
         delta = self.get_delta(key)
         return delta.path
 
-    def child_names(self, **kwargs) -> list[str]:
+    def _child_names(self, **kwargs) -> list[str]:
         """Return keys for each change."""
         return list(self.keystore.keys())
```

### Comparing `quiltcore-0.2.0/quiltcore/delta.py` & `quiltcore-0.2.1/quiltcore/delta.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.2.0/quiltcore/entry.py` & `quiltcore-0.2.1/quiltcore/entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from copy import copy
 from pathlib import Path
-from upath import UPath
 
 from multiformats import multihash
+from upath import UPath
 
 from .resource import Resource
 from .resource_key import ResourceKey
 
 
 class Entry(ResourceKey):
     """
@@ -48,22 +48,20 @@
         self.size = self.get_value(row, self.kSize)
         if not self.size:
             self.size = self.path.stat().st_size
 
     def to_row(self) -> dict:
         return {
             self.kName: self.name,
-            self.kPlaces: [str(self.path)],
+            self.kPlaces: [self.encode(self.path)],
             self.kSize: self.size,
-            self.kHash: {
-                "value": self.hash,
-                "type": self.DEFAULT_HASH_TYPE
-            },
-            self.kMeta: self.meta,                
+            self.kHash: {"value": self.hash, "type": self.DEFAULT_HASH_TYPE},
+            self.kMeta: self.meta,
         }
+
     #
     # Calculate and verify hash
     #
 
     def setup_hash(self, opt: dict = {}):
         """Set or create hash attributes."""
         type = opt.get("type", self.defaultHash)
@@ -93,15 +91,15 @@
         return digest == self.multihash
 
     def get(self, key: str, **kwargs) -> Resource:
         """Copy contents of resource's path into _key_ directory."""
         dir = UPath(key)
         dir.mkdir(parents=True, exist_ok=True)
         path = dir / self.name
-        print(path)
+        logging.debug(f"path: {path}")
         path.write_bytes(self.path.read_bytes())  # for binary files
         clone = copy(self)
         clone.path = path.resolve()
         clone.args = kwargs
-        print("clone", clone)
+        logging.debug(f"clone: {clone}")
 
         return clone
```

### Comparing `quiltcore-0.2.0/quiltcore/manifest.py` & `quiltcore-0.2.1/quiltcore/manifest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from pathlib import Path
 
 import pyarrow as pa  # type: ignore
 import pyarrow.compute as pc  # type: ignore
 import pyarrow.json as pj  # type: ignore
 
-from .entry import Entry
 from .resource_key import ResourceKey
 
 
 class Manifest(ResourceKey):
     """
     In-memory representation of a serialized package manifest.
     list/get returns Entry with Path to the Place data actually lives
@@ -21,17 +20,17 @@
             self.body = self.setup_table()
         except FileNotFoundError:
             logging.warning(f"Manifest not found: {path}")
 
     def hash(self) -> str:
         return self.name
 
-#
-# Parse Table
-#
+    #
+    # Parse Table
+    #
 
     def header_keys(self) -> list[str]:
         headers = self.cf.get_dict("quilt3/headers")
         return list(headers.keys())
 
     def header_dict(self) -> dict:
         return {k: getattr(self, k) for k in self.header_keys()}
@@ -50,20 +49,20 @@
             setattr(self, header, first[header][0])
         return self.table.drop_columns(keys).slice(1)
 
     #
     # Private Methods for child resources
     #
 
-    def child_names(self, **kwargs) -> list[str]:
+    def _child_names(self, **kwargs) -> list[str]:
         """List all child resources."""
         names = self.body.column(self.kName).to_pylist()
         return names
 
-    def child_dict(self, key: str) -> dict:
+    def _child_dict(self, key: str) -> dict:
         """Return the dict for a child resource."""
         # TODO: cache to avoid continually re-calcluating
         rows = self.body.filter(pc.field(self.kName) == key)
         if rows.num_rows == 0:
             raise KeyError(f"Key [{key}] not found in {self.kName} of {self.path}")
         row = rows.to_pydict()
         place = row[self.kPlaces][0][0]
```

### Comparing `quiltcore-0.2.0/quiltcore/namespace.py` & `quiltcore-0.2.1/quiltcore/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
         super().__init__(path, **kwargs)
         self.manifests = kwargs["manifests"]
 
     def hash(self, tag: str = ResourcePath.TAG_DEFAULT) -> str:
         hash_file = self.path / tag
         return hash_file.read_text()
 
-    def child_path(self, key: str) -> Path:
+    def _child_path(self, key: str) -> Path:
         """Return the path for a child resource."""
         hash = self.hash(key)
         return self.manifests / hash
```

### Comparing `quiltcore-0.2.0/quiltcore/registry.py` & `quiltcore-0.2.1/quiltcore/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,23 @@
         super().__init__(path, **kwargs)
         self.root = path
         self.base = self.setup_dir(path, "quilt3/dirs/config")
         self.path = self.setup_dir(self.base, "quilt3/dirs/names")
         self.manifests = self.setup_dir(self.base, "quilt3/dirs/manifests")
 
     def setup_dir(self, path: Path, key: str) -> Path:
-        """ Form dir and create if it does not exist."""
+        """Form dir and create if it does not exist."""
         dir = path / self.cf.get_path(key)
         if not dir.exists():
             dir.mkdir(parents=True, exist_ok=True)
         return dir
 
-    def child_args(self, key: str) -> dict:
+    def _child_args(self, key: str) -> dict:
         return {"manifests": self.manifests}
-    
+
     def put(self, res: Resource, **kwargs) -> "Resource":
         """Link manifest into namespace"""
         if not isinstance(res, Manifest):
             raise TypeError(f"Expected Manifest, got {type(res)}")
         hash = res.hash()
         name = kwargs[self.KEY_NAME]
         name_dir = self.path / name
@@ -43,9 +43,7 @@
         tag_file.write_text(hash)
 
         latest_file = name_dir / self.TAG_DEFAULT
         latest_file.unlink(missing_ok=True)
         latest_file.write_text(hash)
 
         return res
-
-
```

### Comparing `quiltcore-0.2.0/quiltcore/resource.py` & `quiltcore-0.2.1/quiltcore/resource.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from time import time
 from typing import Generator
+from urllib.parse import quote, unquote
 
 import quiltcore
+from upath import UPath
 
 from .yaml.config import Config
 
 
 class Resource:
     """
     Base class for all Quilt resources.
@@ -20,15 +22,15 @@
     DEFAULT_HASH_TYPE = "SHA256"
     KEY_GLOB = "glob"
     KEY_KEY = "_key"
     KEY_NAME = f"namespace.{KEY_KEY}"
     KEY_PATH = "_path"
     MANIFEST = "_manifest"
     TAG_DEFAULT = "latest"
-    
+    UNQUOTED = "/:"
 
     @staticmethod
     def TempGen(filename: str = "") -> Generator[Path, None, None]:
         """Return generator to a temporary directory."""
         with TemporaryDirectory() as tmpdirname:
             temp_path = (
                 Path(tmpdirname) / filename if len(filename) > 0 else Path(tmpdirname)
@@ -41,15 +43,15 @@
             return path
         return Path(".")  # should never happen
 
     @staticmethod
     def ClassFromName(name: str) -> type:
         """Return a class from a string."""
         return getattr(quiltcore, name)
-    
+
     @staticmethod
     def Timestamp() -> str:
         "Return integer timestamp."
         return str(int(time()))
 
     def __init__(self, path: Path, **kwargs):
         self.path = path
@@ -65,15 +67,15 @@
         self.setup_params()
 
     def __repr__(self):
         return f"<{self.class_name}({self.path}, {self.args})>"
 
     def __str__(self):
         return f"<{self.class_name}({self.path})>"
-    
+
     def __eq__(self, other):
         return str(self) == str(other)
 
     def param(self, key: str, default: str) -> str:
         """Return a param."""
         return self.params[key] if key in self.params else default  # type: ignore
 
@@ -81,14 +83,34 @@
         """Load Resource-specific params from config file."""
         self.params = self.cf.get_dict(f"resources/{self.class_name}")
         self.glob = self.param("glob", "*")
         _child = self.param("child", "Resource")
         self.klass = Resource.ClassFromName(_child)
 
     #
+    # URL Encoding of Physical Keys
+    #
+
+    def encoded(self) -> bool:
+        """Return True if Resource keys should be encoded."""
+        return self.cf.get_bool("quilt3/urlencode")
+
+    def encode(self, path: Path) -> str:
+        """Encode path as a string."""
+        key = str(path)
+        return quote(key, safe=self.UNQUOTED) if self.encoded() else key
+
+    def decode(self, key: str) -> Path:
+        """Decode string into a Path."""
+        if not self.encoded():
+            return UPath(key)
+        decoded = unquote(key)
+        return UPath(decoded)
+
+    #
     # Abstract HTTP Methods
     #
 
     def list(self, **kwargs) -> list["Resource"]:
         """List all child resources."""
         return []
```

### Comparing `quiltcore-0.2.0/quiltcore/resource_key.py` & `quiltcore-0.2.1/quiltcore/resource_key.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,44 +21,45 @@
         self.kPlaces = self.cf.get_str("quilt3/places", "physical_keys")
         self.kSize = self.cf.get_str("quilt3/size", "size")
 
     #
     # Abstract Methods for child resources
     #
 
-    def child_names(self, **kwargs) -> list[str]:
+    def _child_names(self, **kwargs) -> list[str]:
         """Return names of each child resource."""
         return []
 
-    def child_dict(self, key: str) -> dict:
+    def _child_dict(self, key: str) -> dict:
         """Return the dict for a child resource."""
         return {}
 
     #
     # Concrete Methods for child resources
     #
 
     def key_path(self, key: str, args: dict = {}) -> Path:
         """Return the Path for a child resource."""
         if self.KEY_PATH not in args:
             raise KeyError(f"Missing {self.KEY_PATH} in {args.keys()}")
         place = args[self.KEY_PATH]
+        self.decode(place)
         return UPath(place)
 
     def child(self, key: str, **kwargs):
         """Return a child resource."""
-        args = self.child_dict(key)
+        args = self._child_dict(key)
         path = self.key_path(key, args)
         merged = {**self.args, **args}
         return self.klass(path, **merged)
 
     #
     # Concrete HTTP Methods
     #
 
     def get(self, key: str, **kwargs) -> "Resource":
         """Get a child resource by name."""
         return self.child(key, **kwargs)
 
     def list(self, **kwargs) -> list[Resource]:
         """List all child resources by name."""
-        return [self.child(key, **kwargs) for key in self.child_names(**kwargs)]
+        return [self.child(key, **kwargs) for key in self._child_names(**kwargs)]
```

### Comparing `quiltcore-0.2.0/quiltcore/resource_path.py` & `quiltcore-0.2.1/quiltcore/resource_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Generator
 
-
 from .resource import Resource
 
 
 class ResourcePath(Resource):
     """
     Path-based list and get.
     """
@@ -16,40 +15,40 @@
         super().__init__(path, **kwargs)
         self.glob = self.param(self.KEY_GLOB, "*")
 
     #
     # Private Methods for Path-based child resources
     #
 
-    def child_args(self, key: str) -> dict:
+    def _child_args(self, key: str) -> dict:
         """Return the kwargs for a child resource."""
         return {}
 
     def child(self, path: Path, key: str = ""):
         """Return a child resource."""
-        args = self.child_args(key)
+        args = self._child_args(key)
         args[self.KEY_KEY] = key
         merged = {**self.args, **args}
         return self.klass(path, **merged)
 
-    def child_path(self, key: str) -> Path:
+    def _child_path(self, key: str) -> Path:
         """Return the path for a child resource."""
         return self.path / key
 
-    def child_list(self) -> Generator[Path, None, None]:
+    def _child_list(self) -> Generator[Path, None, None]:
         """List/generator of valid child paths; defaults to self.glob"""
         return self.path.glob(self.glob)
 
     #
     # Public HTTP-like Methods
     #
 
     def list(self, **kwargs) -> list["Resource"]:
         """List all child resources."""
-        return [self.child(x) for x in self.child_list()]
+        return [self.child(x) for x in self._child_list()]
 
     def get(self, key: str, **kwargs) -> "Resource":
         """Get a child resource by name."""
-        path = self.child_path(key)
+        path = self._child_path(key)
         if not path.exists():
             raise KeyError(f"Key {key} not found in {self.path}")
         return self.child(path, key)
```

### Comparing `quiltcore-0.2.0/quiltcore/volume.py` & `quiltcore-0.2.1/quiltcore/volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import pyarrow as pa  # type: ignore
+from pathlib import Path
 
+import pyarrow as pa  # type: ignore
 from jsonlines import Writer
-from pathlib import Path
 from upath import UPath
 
 from .entry import Entry
 from .manifest import Manifest
-from .namespace import Namespace
 from .registry import Registry
 from .resource import Resource
 from .resource_key import ResourceKey
 
 
 class Volume(ResourceKey):
     """
     Top-level Resource reperesenting a logical unit of storage
     with a single type of filesystem or blob storage
     and its own Registry
     """
+
     ERR_REQUIRE_REGISTRY = "Volume.get requires registry keyword argument"
     KEY_MH = "multihash"
     KEY_HSH = "hash"
     KEY_TAG = "tag"
     KEY_SELF = "."
     MH_PREFIX = Entry.MH_PREFIX["SHA256"]
 
@@ -31,45 +31,45 @@
         path = UPath(uri)
         return Volume(path, **kwargs)
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
         self.registry = Registry(path, **self.args)
         self.uri = self.path.as_uri()
-        self.keystore: dict[str,dict] = {
+        self.keystore: dict[str, dict] = {
             self.KEY_SELF: self.args,
         }
 
     def is_local(self) -> bool:
         return self.uri.startswith("file://")
-    
-    def child_names(self, **kwargs) -> list[str]:
+
+    def _child_names(self, **kwargs) -> list[str]:
         """Return names of each child resource."""
         names = list(self.keystore.keys())
         names.remove(self.KEY_SELF)
         return names
-    
-#
-# List/Delete vs keystore
-#
+
+    #
+    # List/Delete vs keystore
+    #
 
     def delete(self, key: str, **kwargs) -> None:
         """Delete the key from this keystore"""
         if key in self.keystore:
             del self.keystore[key]
             return
         raise KeyError(f"Key {key} not found in {self.keystore.keys()}")
 
     def list(self, **kwargs) -> list["Resource"]:
         """List all child resources."""
-        return [self.get(x) for x in self.child_names()]
-    
-#
-# GET and helpers - return a Manfiest
-#
+        return [self.get(x) for x in self._child_names()]
+
+    #
+    # GET and helpers - return a Manfiest
+    #
 
     def get(self, key: str, **kwargs) -> "Resource":
         """
         Return and keystore manifest for Namespace `key`
 
         * hash
         * multihash
@@ -81,66 +81,69 @@
             return opts["manifest"]
 
         manifest = self.get_manifest(key, **kwargs)
         args = manifest.args.copy()
         args[self.KEY_PATH] = manifest.path
         self.keystore[key] = args
         return manifest
-    
+
     def get_manifest(self, key: str, **kwargs) -> "Resource":
         """
         Create manifest for Namespace `key` and `kwargs`
         """
-        opts: dict[str,str] = kwargs
+        opts: dict[str, str] = kwargs
         hash = self.get_hash(opts)
         if len(hash) > 0:
             return Manifest(self.registry.manifests / hash, **self.args)
 
         tag = opts.get(self.KEY_TAG, self.TAG_DEFAULT)
         name = self.registry.get(key)
-        return name.get(tag)        
+        return name.get(tag)
 
-    def get_hash(self, opts: dict[str,str]) -> str:
+    def get_hash(self, opts: dict[str, str]) -> str:
         if self.KEY_HSH in opts:
             return opts[self.KEY_HSH]
         if self.KEY_MH in opts:
             mh = opts[self.KEY_MH]
             return mh.strip(self.MH_PREFIX)
         return ""
-        
-#
-# PUT and helpers - upload a Manfiest or other resource
-#
-# - PUT Entry: copies individual file onto Volume
-# - PUT Manifest:
-#   - copies necessary Entries onto Volume (unless --nocopy and non-local)
-#   - calculates hash and creates Namespaced folders
-#   - copies Manifest onto Volume
+
+    #
+    # PUT and helpers - upload a Manfiest or other resource
+    #
+    # - PUT Entry: copies individual file onto Volume
+    # - PUT Manifest:
+    #   - copies necessary Entries onto Volume (unless --nocopy and non-local)
+    #   - calculates hash and creates Namespaced folders
+    #   - copies Manifest onto Volume
 
     def put(self, res: Resource, **kwargs) -> "Resource":
         """Insert/Replace and return a child resource."""
         if not isinstance(res, Manifest):
             raise TypeError(f"Volume.put requires a Manifest, not {type(res)}")
         man: Manifest = res
         hash_path = self.registry.manifests / man.hash()
         if hash_path.exists():
             raise FileExistsError(f"Manifest {hash_path} already exists")
 
-        ns_name = kwargs.get(self.KEY_NAME) or man.args.get(self.KEY_NAME) or f"unknown/{self.Timestamp()}"
+        ns_name = (
+            kwargs.get(self.KEY_NAME)
+            or man.args.get(self.KEY_NAME)
+            or f"unknown/{self.Timestamp()}"
+        )
         kwargs[self.KEY_NAME] = ns_name
 
         ns_name = self.write_entries(man, hash_path, ns_name)
         man2 = Manifest(hash_path, **self.args)
         self.registry.put(man2, **kwargs)
         return man2
-    
+
     def write_entries(self, man: Manifest, path: Path, name: str) -> str:
         dest = str(self.path / name)
         entries = [entry.get(dest) for entry in man.list()]
         rows = [entry.to_row() for entry in entries]  # type: ignore
         table = pa.Table.from_pylist(rows)
         with path.open(mode="wb") as fo:
             with Writer(fo) as writer:
                 writer.write(man.header_dict())
                 writer.write(table.to_pydict())
         return name
-
```

### Comparing `quiltcore-0.2.0/quiltcore/yaml/config.py` & `quiltcore-0.2.1/quiltcore/yaml/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,9 +17,12 @@
     def get_str(self, key: str, default="") -> str:
         return super().get(key) or default
 
     def get_path(self, key: str) -> Path:
         str_path = self.get_str(key, ".")
         return Path(str_path)
 
+    def get_bool(self, key: str) -> bool:
+        return self.get(key) or False
+
     def get_dict(self, key: str) -> dict:
         return self.get(key) or {}
```

### Comparing `quiltcore-0.2.0/quiltcore/yaml/quiltcore.yaml` & `quiltcore-0.2.1/quiltcore/yaml/quiltcore.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -39,7 +39,8 @@
   hash: hash
   headers:
     version: string
     message: string
   mime_type: application/ld+json
   name: logical_key
   places: physical_keys
+  urlencode: True
```

### Comparing `quiltcore-0.2.0/PKG-INFO` & `quiltcore-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiltcore
-Version: 0.2.0
+Version: 0.2.1
 Summary: low-level plubming to read/write Quilt packages
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

