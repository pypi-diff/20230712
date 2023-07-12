# Comparing `tmp/libyang-2.7.1.tar.gz` & `tmp/libyang-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libyang-2.7.1.tar", last modified: Wed May 24 13:03:57 2023, max compression
+gzip compressed data, was "libyang-2.8.0.tar", last modified: Wed Jul 12 11:48:40 2023, max compression
```

## Comparing `libyang-2.7.1.tar` & `libyang-2.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.407830 libyang-2.7.1/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-24 13:03:32.000000 libyang-2.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2023-05-24 13:03:32.000000 libyang-2.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9337 2023-05-24 13:03:57.407830 libyang-2.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8756 2023-05-24 13:03:32.000000 libyang-2.7.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.407830 libyang-2.7.1/cffi/
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-24 13:03:32.000000 libyang-2.7.1/cffi/build.py
--rw-r--r--   0 root         (0) root         (0)    26553 2023-05-24 13:03:32.000000 libyang-2.7.1/cffi/cdefs.h
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-24 13:03:32.000000 libyang-2.7.1/cffi/source.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.411830 libyang-2.7.1/libyang/
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-24 13:03:57.411830 libyang-2.7.1/libyang/VERSION
--rw-r--r--   0 root         (0) root         (0)     3183 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14358 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/context.py
--rw-r--r--   0 root         (0) root         (0)    42242 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/data.py
--rw-r--r--   0 root         (0) root         (0)    13409 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/diff.py
--rw-r--r--   0 root         (0) root         (0)     5722 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/keyed_list.py
--rw-r--r--   0 root         (0) root         (0)     1941 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/log.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/py.typed
--rw-r--r--   0 root         (0) root         (0)    44040 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/schema.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/util.py
--rw-r--r--   0 root         (0) root         (0)    18831 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/xpath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.407830 libyang-2.7.1/libyang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9337 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      590 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      289 2023-05-24 13:03:32.000000 libyang-2.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      713 2023-05-24 13:03:57.411830 libyang-2.7.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     5815 2023-05-24 13:03:32.000000 libyang-2.7.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.407830 libyang-2.7.1/tests/
--rw-r--r--   0 root         (0) root         (0)     3722 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_context.py
--rw-r--r--   0 root         (0) root         (0)    24778 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_data.py
--rw-r--r--   0 root         (0) root         (0)     3935 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_diff.py
--rw-r--r--   0 root         (0) root         (0)     3547 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_keyedlist.py
--rw-r--r--   0 root         (0) root         (0)    16192 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_schema.py
--rw-r--r--   0 root         (0) root         (0)    15307 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_xpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:48:40.676548 libyang-2.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-12 11:48:24.000000 libyang-2.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      205 2023-07-12 11:48:24.000000 libyang-2.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9337 2023-07-12 11:48:40.676548 libyang-2.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8756 2023-07-12 11:48:24.000000 libyang-2.8.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:48:40.672548 libyang-2.8.0/cffi/
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-12 11:48:24.000000 libyang-2.8.0/cffi/build.py
+-rw-r--r--   0 root         (0) root         (0)    26774 2023-07-12 11:48:24.000000 libyang-2.8.0/cffi/cdefs.h
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-12 11:48:24.000000 libyang-2.8.0/cffi/source.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:48:40.676548 libyang-2.8.0/libyang/
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-12 11:48:40.676548 libyang-2.8.0/libyang/VERSION
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14369 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/context.py
+-rw-r--r--   0 root         (0) root         (0)    42254 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/data.py
+-rw-r--r--   0 root         (0) root         (0)    13430 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/diff.py
+-rw-r--r--   0 root         (0) root         (0)     5722 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/keyed_list.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/log.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/py.typed
+-rw-r--r--   0 root         (0) root         (0)    49432 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/schema.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/util.py
+-rw-r--r--   0 root         (0) root         (0)    18831 2023-07-12 11:48:24.000000 libyang-2.8.0/libyang/xpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:48:40.672548 libyang-2.8.0/libyang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9337 2023-07-12 11:48:40.000000 libyang-2.8.0/libyang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-12 11:48:40.000000 libyang-2.8.0/libyang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 11:48:40.000000 libyang-2.8.0/libyang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 11:48:40.000000 libyang-2.8.0/libyang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-12 11:48:40.000000 libyang-2.8.0/libyang.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-12 11:48:40.000000 libyang-2.8.0/libyang.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      289 2023-07-12 11:48:24.000000 libyang-2.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      713 2023-07-12 11:48:40.676548 libyang-2.8.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     5815 2023-07-12 11:48:24.000000 libyang-2.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:48:40.676548 libyang-2.8.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3722 2023-07-12 11:48:24.000000 libyang-2.8.0/tests/test_context.py
+-rw-r--r--   0 root         (0) root         (0)    24778 2023-07-12 11:48:24.000000 libyang-2.8.0/tests/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     4314 2023-07-12 11:48:24.000000 libyang-2.8.0/tests/test_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-07-12 11:48:24.000000 libyang-2.8.0/tests/test_keyedlist.py
+-rw-r--r--   0 root         (0) root         (0)    17123 2023-07-12 11:48:24.000000 libyang-2.8.0/tests/test_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15307 2023-07-12 11:48:24.000000 libyang-2.8.0/tests/test_xpath.py
```

### Comparing `libyang-2.7.1/LICENSE` & `libyang-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/PKG-INFO` & `libyang-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libyang
-Version: 2.7.1
+Version: 2.8.0
 Summary: CFFI bindings to libyang
 Home-page: https://github.com/CESNET/libyang-python
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: MIT
 Keywords: libyang,cffi
 Classifier: Development Status :: 4 - Beta
```

### Comparing `libyang-2.7.1/README.rst` & `libyang-2.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/cffi/build.py` & `libyang-2.8.0/cffi/build.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/cffi/cdefs.h` & `libyang-2.8.0/cffi/cdefs.h`

 * *Files 0% similar despite different names*

```diff
@@ -974,14 +974,25 @@
 #define LYD_DUP_WITH_FLAGS  ...
 #define LYD_DUP_WITH_PARENTS  ...
 
 LY_ERR lyd_dup_siblings(const struct lyd_node *, struct lyd_node_inner *, uint32_t, struct lyd_node **);
 LY_ERR lyd_dup_single(const struct lyd_node *, struct lyd_node_inner *, uint32_t, struct lyd_node **);
 void lyd_free_meta_single(struct lyd_meta *);
 
+struct lysp_tpdf {
+    const char *name;
+    const char *units;
+    struct lysp_qname dflt;
+    const char *dsc;
+    const char *ref;
+    struct lysp_ext_instance *exts;
+    struct lysp_type type;
+    uint16_t flags;
+};
+
 struct lysc_when {
     struct lyxp_expr *cond;
     struct lysc_node *context;
     struct lysc_prefix *prefixes;
     const char *dsc;
     const char *ref;
     struct lysc_ext_instance *exts;
```

### Comparing `libyang-2.7.1/libyang/__init__.py` & `libyang-2.8.0/libyang/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     SLeaf,
     SLeafList,
     SList,
     SNode,
     SRpc,
     SRpcInOut,
     Type,
+    Typedef,
 )
 from .util import DataType, IOType, LibyangError
 from .xpath import (
     xpath_del,
     xpath_get,
     xpath_getall,
     xpath_move,
```

### Comparing `libyang-2.7.1/libyang/context.py` & `libyang-2.8.0/libyang/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 from .schema import Module, SNode, schema_in_format
 from .util import DataType, IOType, LibyangError, c2str, data_load, str2c
 
 
 # -------------------------------------------------------------------------------------
 class Context:
-    __slots__ = ("cdata",)
+    __slots__ = ("cdata", "__dict__")
 
     def __init__(
         self,
         search_path: Optional[str] = None,
         disable_searchdir_cwd: bool = True,
         explicit_compile: Optional[bool] = False,
         yanglib_path: Optional[str] = None,
```

### Comparing `libyang-2.7.1/libyang/data.py` & `libyang-2.8.0/libyang/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
 # -------------------------------------------------------------------------------------
 class DNode:
     """
     Data tree node.
     """
 
-    __slots__ = ("context", "cdata", "free_func")
+    __slots__ = ("context", "cdata", "free_func", "__dict__")
 
     def __init__(self, context: "libyang.Context", cdata):
         """
         :arg context:
             The libyang.Context python object.
         :arg cdata:
             The pointer to the C structure allocated by libyang.so.
```

### Comparing `libyang-2.7.1/libyang/diff.py` & `libyang-2.8.0/libyang/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     for path in sorted(diffs.keys()):
         yield from diffs[path]
 
 
 # -------------------------------------------------------------------------------------
 class SNodeDiff:
-    pass
+    __slots__ = ("__dict__",)
 
 
 # -------------------------------------------------------------------------------------
 class SNodeRemoved(SNodeDiff):
     __slots__ = ("node",)
 
     def __init__(self, node: SNode):
```

### Comparing `libyang-2.7.1/libyang/keyed_list.py` & `libyang-2.8.0/libyang/keyed_list.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/libyang/log.py` & `libyang-2.8.0/libyang/log.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/libyang/schema.py` & `libyang-2.8.0/libyang/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     if shrink:
         flags |= lib.LYS_PRINT_SHRINK
     return flags
 
 
 # -------------------------------------------------------------------------------------
 class Module:
-    __slots__ = ("context", "cdata")
+    __slots__ = ("context", "cdata", "__dict__")
 
     def __init__(self, context: "libyang.Context", cdata):
         self.context = context
         self.cdata = cdata  # C type: "struct lys_module *"
 
     def name(self) -> str:
         return c2str(self.cdata.name)
@@ -108,14 +108,36 @@
                 return f
         raise self.context.error("no such feature: %r" % name)
 
     def revisions(self) -> Iterator["Revision"]:
         for revision in ly_array_iter(self.cdata.parsed.revs):
             yield Revision(self.context, revision, self)
 
+    def typedefs(self) -> Iterator["Typedef"]:
+        for typedef in ly_array_iter(self.cdata.parsed.typedefs):
+            yield Typedef(self.context, typedef)
+
+    def get_typedef(self, name: str) -> Optional["Typedef"]:
+        for typedef in self.typedefs():
+            if typedef.name() != name:
+                continue
+            return typedef
+        return None
+
+    def imports(self) -> Iterator["Import"]:
+        for i in ly_array_iter(self.cdata.parsed.imports):
+            yield Import(self.context, i, self)
+
+    def get_module_from_prefix(self, prefix: str) -> Optional["Module"]:
+        for i in self.imports():
+            if i.prefix() != prefix:
+                continue
+            return self.context.get_module(i.name())
+        return None
+
     def __iter__(self) -> Iterator["SNode"]:
         return self.children()
 
     def children(self, types: Optional[Tuple[int, ...]] = None) -> Iterator["SNode"]:
         return iter_children(self.context, self.cdata, types=types)
 
     def __str__(self) -> str:
@@ -223,15 +245,15 @@
             rpcreply=rpcreply,
             notification=notification,
         )
 
 
 # -------------------------------------------------------------------------------------
 class Revision:
-    __slots__ = ("context", "cdata", "module")
+    __slots__ = ("context", "cdata", "module", "__dict__")
 
     def __init__(self, context: "libyang.Context", cdata, module):
         self.context = context
         self.cdata = cdata  # C type: "struct lysp_revision *"
         self.module = module
 
     def date(self) -> str:
@@ -265,16 +287,62 @@
         return "<%s.%s: %s>" % (cls.__module__, cls.__name__, str(self))
 
     def __str__(self):
         return self.date()
 
 
 # -------------------------------------------------------------------------------------
+class Import:
+    __slots__ = ("context", "cdata", "module", "__dict__")
+
+    def __init__(self, context: "libyang.Context", cdata, module):
+        self.context = context
+        self.cdata = cdata  # C type: "struct lysp_revision *"
+        self.module = module
+
+    def name(self) -> str:
+        return c2str(self.cdata.name)
+
+    def prefix(self) -> Optional[str]:
+        return c2str(self.cdata.prefix)
+
+    def description(self) -> Optional[str]:
+        return c2str(self.cdata.dsc)
+
+    def reference(self) -> Optional[str]:
+        return c2str(self.cdata.ref)
+
+    def extensions(self) -> Iterator["ExtensionParsed"]:
+        for ext in ly_array_iter(self.cdata.exts):
+            yield ExtensionParsed(self.context, ext, self.module)
+
+    def get_extension(
+        self, name: str, prefix: Optional[str] = None, arg_value: Optional[str] = None
+    ) -> Optional["ExtensionParsed"]:
+        for ext in self.extensions():
+            if ext.name() != name:
+                continue
+            if prefix is not None and ext.module().name() != prefix:
+                continue
+            if arg_value is not None and ext.argument() != arg_value:
+                continue
+            return ext
+        return None
+
+    def __repr__(self):
+        cls = self.__class__
+        return "<%s.%s: %s>" % (cls.__module__, cls.__name__, str(self))
+
+    def __str__(self):
+        return self.name()
+
+
+# -------------------------------------------------------------------------------------
 class Extension:
-    __slots__ = ("context", "cdata")
+    __slots__ = ("context", "cdata", "__dict__")
 
     def __init__(self, context: "libyang.Context", cdata, module_parent: Module = None):
         self.context = context
         self.cdata = cdata
 
     def argument(self) -> Optional[str]:
         return c2str(self.cdata.argument)
@@ -327,15 +395,15 @@
         if not self.cdata_def.module:
             raise self.context.error("cannot get module")
         return Module(self.context, self.cdata_def.module)
 
 
 # -------------------------------------------------------------------------------------
 class _EnumBit:
-    __slots__ = ("context", "cdata")
+    __slots__ = ("context", "cdata", "__dict__")
 
     def __init__(self, context: "libyang.Context", cdata):
         self.context = context
         self.cdata = cdata  # C type "struct lys_type_bit" or "struct lys_type_enum"
 
     def position(self) -> int:
         return self.cdata.position
@@ -378,15 +446,15 @@
 # -------------------------------------------------------------------------------------
 class Bit(_EnumBit):
     pass
 
 
 # -------------------------------------------------------------------------------------
 class Type:
-    __slots__ = ("context", "cdata", "cdata_parsed")
+    __slots__ = ("context", "cdata", "cdata_parsed", "__dict__")
 
     UNKNOWN = lib.LY_TYPE_UNKNOWN
     BINARY = lib.LY_TYPE_BINARY
     UINT8 = lib.LY_TYPE_UINT8
     UINT16 = lib.LY_TYPE_UINT16
     UINT32 = lib.LY_TYPE_UINT32
     UINT64 = lib.LY_TYPE_UINT64
@@ -444,14 +512,17 @@
 
     def name(self) -> str:
         if self.cdata_parsed is not None and self.cdata_parsed.name:
             return c2str(self.cdata_parsed.name)
         return self.basename()
 
     def description(self) -> Optional[str]:
+        typedef = self.typedef()
+        if typedef:
+            return typedef.description()
         return None
 
     def base(self) -> int:
         return self.cdata.basetype
 
     def bases(self) -> Iterator[int]:
         for b in self.get_bases():
@@ -472,20 +543,35 @@
 
     def leafref_path(self) -> Optional["str"]:
         if self.cdata.basetype != self.LEAFREF:
             return None
         lr = ffi.cast("struct lysc_type_leafref *", self.cdata)
         return c2str(lib.lyxp_get_expr(lr.path))
 
+    def typedef(self) -> "Typedef":
+        if ":" in self.name():
+            module_prefix, type_name = self.name().split(":")
+            import_module = self.module().get_module_from_prefix(module_prefix)
+            if import_module:
+                return import_module.get_typedef(type_name)
+        return None
+
     def union_types(self) -> Iterator["Type"]:
         if self.cdata.basetype != self.UNION:
             return
+
         t = ffi.cast("struct lysc_type_union *", self.cdata)
-        for union_type in ly_array_iter(t.types):
-            yield Type(self.context, union_type, None)
+        if self.cdata_parsed and self.cdata_parsed.types != ffi.NULL:
+            for union_type, union_type_parsed in zip(
+                ly_array_iter(t.types), ly_array_iter(self.cdata_parsed.types)
+            ):
+                yield Type(self.context, union_type, union_type_parsed)
+        else:
+            for union_type in ly_array_iter(t.types):
+                yield Type(self.context, union_type, None)
 
     def enums(self) -> Iterator[Enum]:
         if self.cdata.basetype != self.ENUM:
             return
         t = ffi.cast("struct lysc_type_enum *", self.cdata)
         for enum in ly_array_iter(t.enums):
             yield Enum(self.context, enum)
@@ -565,19 +651,17 @@
         if self.cdata.basetype == lib.LY_TYPE_UNION:
             for t in self.union_types():
                 yield from t.all_patterns()
         else:
             yield from self.patterns()
 
     def module(self) -> Module:
-        # TODO: pointer to the parsed module wehere is the type defined is in self.cdata_parsed.pmod
-        # however there is no way how to get name of the module from lysp_module
-        if not self.cdata.der.module:
+        if not self.cdata_parsed:
             return None
-        return Module(self.context, self.cdata.der.module)
+        return Module(self.context, self.cdata_parsed.pmod.mod)
 
     def extensions(self) -> Iterator[ExtensionCompiled]:
         for extension in ly_array_iter(self.cdata.exts):
             yield ExtensionCompiled(self.context, extension)
 
     def get_extension(
         self, name: str, prefix: Optional[str] = None, arg_value: Optional[str] = None
@@ -597,16 +681,69 @@
         return "<%s.%s: %s>" % (cls.__module__, cls.__name__, str(self))
 
     def __str__(self):
         return self.name()
 
 
 # -------------------------------------------------------------------------------------
+class Typedef:
+    __slots__ = ("context", "cdata", "__dict__")
+
+    def __init__(self, context: "libyang.Context", cdata):
+        self.context = context
+        self.cdata = cdata  # C type: "struct lysp_tpdf *"
+
+    def name(self) -> str:
+        return c2str(self.cdata.name)
+
+    def description(self) -> Optional[str]:
+        return c2str(self.cdata.dsc)
+
+    def units(self) -> Optional[str]:
+        return c2str(self.cdata.units)
+
+    def reference(self) -> Optional[str]:
+        return c2str(self.cdata.ref)
+
+    def extensions(self) -> Iterator[ExtensionCompiled]:
+        ext = ffi.cast("struct lysc_ext_instance *", self.cdata.exts)
+        if ext == ffi.NULL:
+            return
+        for extension in ly_array_iter(ext):
+            yield ExtensionCompiled(self.context, extension)
+
+    def get_extension(
+        self, name: str, prefix: Optional[str] = None, arg_value: Optional[str] = None
+    ) -> Optional[ExtensionCompiled]:
+        for ext in self.extensions():
+            if ext.name() != name:
+                continue
+            if prefix is not None and ext.module().name() != prefix:
+                continue
+            if arg_value is not None and ext.argument() != arg_value:
+                continue
+            return ext
+        return None
+
+    def deprecated(self) -> bool:
+        return bool(self.cdata.flags & lib.LYS_STATUS_DEPRC)
+
+    def obsolete(self) -> bool:
+        return bool(self.cdata.flags & lib.LYS_STATUS_OBSLT)
+
+    def module(self) -> Module:
+        return Module(self.context, self.cdata.module)
+
+    def __str__(self):
+        return self.name()
+
+
+# -------------------------------------------------------------------------------------
 class Feature:
-    __slots__ = ("context", "cdata")
+    __slots__ = ("context", "cdata", "__dict__")
 
     def __init__(self, context: "libyang.Context", cdata):
         self.context = context
         self.cdata = cdata  # C type: "struct lysp_feature *"
 
     def name(self) -> str:
         return c2str(self.cdata.name)
@@ -641,15 +778,15 @@
 
     def __str__(self):
         return self.name()
 
 
 # -------------------------------------------------------------------------------------
 class IfFeatureExpr:
-    __slots__ = ("context", "cdata", "module_features", "compiled")
+    __slots__ = ("context", "cdata", "module_features", "compiled", "__dict__")
 
     def __init__(self, context: "libyang.Context", cdata, module_features=None):
         """
         if module_features is not None, it means we are using a parsed IfFeatureExpr
         """
         self.context = context
         # Can be "struct lysc_iffeature *" if comes from module feature
@@ -864,17 +1001,19 @@
 
     def __str__(self):
         return "(%s OR %s)" % (self.a, self.b)
 
 
 # -------------------------------------------------------------------------------------
 class SNode:
-    __slots__ = ("context", "cdata", "cdata_parsed")
+    __slots__ = ("context", "cdata", "cdata_parsed", "__dict__")
 
     CONTAINER = lib.LYS_CONTAINER
+    CHOICE = lib.LYS_CHOICE
+    CASE = lib.LYS_CASE
     LEAF = lib.LYS_LEAF
     LEAFLIST = lib.LYS_LEAFLIST
     LIST = lib.LYS_LIST
     RPC = lib.LYS_RPC
     ACTION = lib.LYS_ACTION
     INPUT = lib.LYS_INPUT
     OUTPUT = lib.LYS_OUTPUT
@@ -1185,14 +1324,34 @@
     def __iter__(self) -> Iterator[SNode]:
         return self.children()
 
     def children(self, types: Optional[Tuple[int, ...]] = None) -> Iterator[SNode]:
         return iter_children(self.context, self.cdata, types=types)
 
 
+# -------------------------------------------------------------------------------------
+@SNode.register(SNode.CHOICE)
+class SChoice(SNode):
+    def __iter__(self) -> Iterator[SNode]:
+        return self.children()
+
+    def children(self, types: Optional[Tuple[int, ...]] = None) -> Iterator[SNode]:
+        return iter_children(self.context, self.cdata, types=types)
+
+
+# -------------------------------------------------------------------------------------
+@SNode.register(SNode.CASE)
+class SCase(SNode):
+    def __iter__(self) -> Iterator[SNode]:
+        return self.children()
+
+    def children(self, types: Optional[Tuple[int, ...]] = None) -> Iterator[SNode]:
+        return iter_children(self.context, self.cdata, types=types)
+
+
 # -------------------------------------------------------------------------------------
 @SNode.register(SNode.LIST)
 class SList(SNode):
     __slots__ = ("cdata_list", "cdata_list_parsed")
 
     def __init__(self, context: "libyang.Context", cdata):
         super().__init__(context, cdata)
```

### Comparing `libyang-2.7.1/libyang/util.py` & `libyang-2.8.0/libyang/util.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/libyang/xpath.py` & `libyang-2.8.0/libyang/xpath.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/libyang.egg-info/PKG-INFO` & `libyang-2.8.0/libyang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libyang
-Version: 2.7.1
+Version: 2.8.0
 Summary: CFFI bindings to libyang
 Home-page: https://github.com/CESNET/libyang-python
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: MIT
 Keywords: libyang,cffi
 Classifier: Development Status :: 4 - Beta
```

### Comparing `libyang-2.7.1/libyang.egg-info/SOURCES.txt` & `libyang-2.8.0/libyang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/setup.cfg` & `libyang-2.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/setup.py` & `libyang-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/tests/test_context.py` & `libyang-2.8.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/tests/test_data.py` & `libyang-2.8.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/tests/test_diff.py` & `libyang-2.8.0/tests/test_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,20 @@
             (SNodeAdded, "/yolo-system:alarm-triggered/description"),
             (EnumRemoved, "/yolo-system:conf/url/proto"),
             (EnumRemoved, "/yolo-system:state/url/proto"),
             (EnumStatusAdded, "/yolo-system:conf/url/proto"),
             (EnumStatusAdded, "/yolo-system:state/url/proto"),
             (EnumStatusRemoved, "/yolo-system:conf/url/proto"),
             (EnumStatusRemoved, "/yolo-system:state/url/proto"),
+            (SNodeAdded, "/yolo-system:conf/pill/red/out"),
+            (SNodeAdded, "/yolo-system:state/pill/red/out"),
+            (SNodeAdded, "/yolo-system:conf/pill/blue/in"),
+            (SNodeAdded, "/yolo-system:state/pill/blue/in"),
+            (SNodeAdded, "/yolo-system:alarm-triggered/severity"),
+            (SNodeAdded, "/yolo-system:alarm-triggered/description"),
         )
     )
 
     def test_diff(self):
         with Context(OLD_YANG_DIR) as ctx_old, Context(NEW_YANG_DIR) as ctx_new:
             mod = ctx_old.load_module("yolo-system")
             mod.feature_enable_all()
```

### Comparing `libyang-2.7.1/tests/test_keyedlist.py` & `libyang-2.8.0/tests/test_keyedlist.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.1/tests/test_schema.py` & `libyang-2.8.0/tests/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,20 @@
         self.assertTrue(self.module.feature_state("turbo-boost"))
         self.module.feature_disable_all()
         self.assertFalse(self.module.feature_state("turbo-boost"))
         self.module.feature_enable_all()
         self.assertTrue(self.module.feature_state("turbo-boost"))
         self.module.feature_disable_all()
 
+    def test_mod_imports(self):
+        imports = list(self.module.imports())
+        self.assertEqual(imports[0].name(), "omg-extensions")
+        self.assertEqual(imports[1].name(), "wtf-types")
+        self.assertEqual(len(imports), 2)
+
     def test_mod_features(self):
         features = list(self.module.features())
         self.assertEqual(len(features), 2)
 
     def test_mod_get_feature(self):
         self.module.feature_enable("turbo-boost")
         feature = self.module.get_feature("turbo-boost")
@@ -254,28 +260,28 @@
         self.assertIsInstance(self.container.module(), Module)
         self.assertEqual(self.container.schema_path(), "/yolo-system:conf")
         self.assertEqual(self.container.data_path(), "/yolo-system:conf")
         self.assertIs(self.container.presence(), None)
 
     def test_cont_iter(self):
         children = list(iter(self.container))
-        self.assertEqual(len(children), 9)
+        self.assertEqual(len(children), 11)
 
     def test_cont_children_leafs(self):
         leafs = list(self.container.children(types=(SNode.LEAF,)))
-        self.assertEqual(len(leafs), 7)
+        self.assertEqual(len(leafs), 9)
 
     def test_cont_parent(self):
         self.assertIsNone(self.container.parent())
 
     def test_iter_tree(self):
         tree = list(self.container.iter_tree())
-        self.assertEqual(len(tree), 15)
-        tree = list(self.container.iter_tree(full=True))
         self.assertEqual(len(tree), 20)
+        tree = list(self.container.iter_tree(full=True))
+        self.assertEqual(len(tree), 25)
 
 
 # -------------------------------------------------------------------------------------
 class ListTest(unittest.TestCase):
     SCHEMA_PATH = "/yolo-system:conf/url"
     DATA_PATH = "/yolo-system:conf/url[host='%s'][proto='%s']"
 
@@ -366,17 +372,21 @@
     def test_leaf_type_derived(self):
         leaf = next(self.ctx.find_path("/yolo-system:conf/yolo-system:hostname"))
         self.assertIsInstance(leaf, SLeaf)
         t = leaf.type()
         self.assertIsInstance(t, Type)
         self.assertEqual(t.name(), "types:host")
         self.assertEqual(t.base(), Type.STRING)
-        # mod = t.module()
-        # self.assertIsNot(mod, None)
-        # self.assertEqual(mod.name(), "wtf-types")
+        mod = t.module()
+        self.assertIsNot(mod, None)
+        self.assertEqual(mod.name(), "yolo-system")
+        self.assertEqual(mod.get_module_from_prefix("types").name(), "wtf-types")
+        self.assertEqual(t.typedef().name(), "host")
+        self.assertEqual(t.typedef().description(), "my host type.")
+        self.assertEqual(t.description(), "my host type.")
 
     def test_leaf_type_status(self):
         leaf = next(self.ctx.find_path("/yolo-system:conf/yolo-system:hostname"))
         self.assertIsInstance(leaf, SLeaf)
         self.assertEqual(leaf.deprecated(), False)
         self.assertEqual(leaf.obsolete(), False)
         leaf = next(self.ctx.find_path("/yolo-system:conf/yolo-system:deprecated-leaf"))
@@ -402,14 +412,20 @@
         self.assertIsInstance(leaf, SLeafList)
         t = leaf.type()
         self.assertIsInstance(t, Type)
         self.assertEqual(t.name(), "types:number")
         self.assertEqual(t.base(), Type.UNION)
         types = set(u.name() for u in t.union_types())
         self.assertEqual(types, set(["int16", "int32", "uint16", "uint32"]))
+        for u in t.union_types():
+            ext = u.get_extension(
+                "type-desc", prefix="omg-extensions", arg_value=f"<{u.name()}>"
+            )
+            self.assertIsInstance(ext, Extension)
+            self.assertEqual(len(list(u.extensions())), 2)
         bases = set(t.basenames())
         self.assertEqual(bases, set(["int16", "int32", "uint16", "uint32"]))
 
     def test_leaf_type_extensions(self):
         leaf = next(
             self.ctx.find_path("/yolo-system:conf/yolo-system:url/yolo-system:proto")
         )
@@ -445,7 +461,11 @@
         leaf = next(
             self.ctx.find_path("/yolo-system:conf/yolo-system:url/yolo-system:proto")
         )
         parent = leaf.parent()
         self.assertIsNotNone(parent)
         self.assertIsInstance(parent, SList)
         self.assertEqual(parent.name(), "url")
+
+    def test_iter_tree(self):
+        leaf = next(self.ctx.find_path("/yolo-system:conf"))
+        self.assertEqual(len(list(leaf.iter_tree(full=True))), 23)
```

### Comparing `libyang-2.7.1/tests/test_xpath.py` & `libyang-2.8.0/tests/test_xpath.py`

 * *Files identical despite different names*

