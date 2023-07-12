# Comparing `tmp/uglyduck-0.0.2.tar.gz` & `tmp/uglyduck-0.0.3.tar.gz`

## Comparing `uglyduck-0.0.2.tar` & `uglyduck-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 uglyduck-0.0.2/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uglyduck-0.0.2/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 uglyduck-0.0.2/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 uglyduck-0.0.2/src/uglyduck/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uglyduck-0.0.2/src/uglyduck/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 uglyduck-0.0.2/src/uglyduck/analyzer.py
--rw-r--r--   0        0        0    18607 2020-02-02 00:00:00.000000 uglyduck-0.0.2/src/uglyduck/inspector.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 uglyduck-0.0.2/src/uglyduck/parse.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 uglyduck-0.0.2/src/uglyduck/tests.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 uglyduck-0.0.2/src/uglyduck/types.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 uglyduck-0.0.2/src/uglyduck/utils.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 uglyduck-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 uglyduck-0.0.2/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 uglyduck-0.0.2/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 uglyduck-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 uglyduck-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 uglyduck-0.0.3/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 uglyduck-0.0.3/.gitattributes
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 uglyduck-0.0.3/build.sh
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 uglyduck-0.0.3/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 uglyduck-0.0.3/src/uglyduck/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uglyduck-0.0.3/src/uglyduck/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 uglyduck-0.0.3/src/uglyduck/analyzer.py
+-rw-r--r--   0        0        0    19551 2020-02-02 00:00:00.000000 uglyduck-0.0.3/src/uglyduck/inspector.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 uglyduck-0.0.3/src/uglyduck/parse.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 uglyduck-0.0.3/src/uglyduck/tests.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 uglyduck-0.0.3/src/uglyduck/types.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 uglyduck-0.0.3/src/uglyduck/utils.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 uglyduck-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 uglyduck-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 uglyduck-0.0.3/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 uglyduck-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 uglyduck-0.0.3/PKG-INFO
```

### Comparing `uglyduck-0.0.2/.DS_Store` & `uglyduck-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `uglyduck-0.0.2/src/.DS_Store` & `uglyduck-0.0.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `uglyduck-0.0.2/src/uglyduck/.DS_Store` & `uglyduck-0.0.3/src/uglyduck/.DS_Store`

 * *Files identical despite different names*

### Comparing `uglyduck-0.0.2/src/uglyduck/inspector.py` & `uglyduck-0.0.3/src/uglyduck/inspector.py`

 * *Files 10% similar despite different names*

```diff
@@ -407,16 +407,44 @@
         ]:
             if len(t) == 0:
                 type_name = 'typing.List[typing.Any]'
             else:
                 list_type = self.get_type_name(t[0])
                 type_name = f'typing.List[{list_type}]'
         elif isinstance(t, dict):
-            items = ', '.join([self.get_type_name(item) for item in t])
-            type_name = f'typing.Dict[{items}]'
+            key_types = []
+            value_types = []
+            for d_key, d_val in t.items():
+                key_type = self.get_type_name(d_key)
+                value_type = self.get_type_name(d_val)
+
+                if key_type not in key_types:
+                    key_types.append(key_type)
+
+                if value_type not in value_types:
+                    value_types.append(value_type)
+
+            if len(key_types) > 1:
+                key_type = f"typing.Union[{', '.join(key_types)}]"
+            elif len(key_types) == 1:
+                key_type = key_types[0]
+            else:
+                key_type = None
+
+            if len(value_types) > 1:
+                value_type = f"typing.Union[{', '.join(value_types)}]"
+            elif len(value_types) == 1:
+                value_type = value_types[0]
+            else:
+                value_type = None
+
+            if key_type is None or value_type is None:
+                type_name = 'typing.Dict'
+            else:
+                type_name = f'typing.Dict[{key_type}, {value_type}]'
         elif isinstance(t, (int, float, bool, str)):
             if isinstance(t, str) and str(t) in self.current_module.__dict__ or str(t) in self.classes:
                 if self.is_interface_method_name(t):
                     type_name = f"'{t}'"
                 else:
                     type_name = f"'I{t}'"
             else:
```

### Comparing `uglyduck-0.0.2/src/uglyduck/parse.py` & `uglyduck-0.0.3/src/uglyduck/parse.py`

 * *Files identical despite different names*

### Comparing `uglyduck-0.0.2/src/uglyduck/tests.py` & `uglyduck-0.0.3/src/uglyduck/tests.py`

 * *Files identical despite different names*

### Comparing `uglyduck-0.0.2/.gitignore` & `uglyduck-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `uglyduck-0.0.2/LICENSE` & `uglyduck-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uglyduck-0.0.2/README.md` & `uglyduck-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `uglyduck-0.0.2/pyproject.toml` & `uglyduck-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uglyduck"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Malero", email="contact@maleero.com" },
 ]
 description = "Generate a types.py file for a package that contains protocols for classes generated from the files specified."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `uglyduck-0.0.2/PKG-INFO` & `uglyduck-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uglyduck
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate a types.py file for a package that contains protocols for classes generated from the files specified.
 Project-URL: Homepage, https://github.com/malero/uglyduck
 Project-URL: Bug Tracker, https://github.com/malero/uglyduck/issues
 Author-email: Malero <contact@maleero.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

