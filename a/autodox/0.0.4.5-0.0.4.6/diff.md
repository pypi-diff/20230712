# Comparing `tmp/autodox-0.0.4.5.tar.gz` & `tmp/autodox-0.0.4.6.tar.gz`

## Comparing `autodox-0.0.4.5.tar` & `autodox-0.0.4.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autodox-0.0.4.5/autodox/__init__.py
--rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 autodox-0.0.4.5/autodox/functions.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 autodox-0.0.4.5/tests/context.py
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 autodox-0.0.4.5/tests/test_hooks.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.4.5/.gitignore
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 autodox-0.0.4.5/license
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 autodox-0.0.4.5/pyproject.toml
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 autodox-0.0.4.5/readme.md
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 autodox-0.0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autodox-0.0.4.6/autodox/__init__.py
+-rw-r--r--   0        0        0    18544 2020-02-02 00:00:00.000000 autodox-0.0.4.6/autodox/functions.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 autodox-0.0.4.6/tests/context.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 autodox-0.0.4.6/tests/test_hooks.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.4.6/.gitignore
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 autodox-0.0.4.6/license
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 autodox-0.0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 autodox-0.0.4.6/readme.md
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 autodox-0.0.4.6/PKG-INFO
```

### Comparing `autodox-0.0.4.5/autodox/functions.py` & `autodox-0.0.4.6/autodox/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,17 @@
                 annotations[i+offset] += f' = {defaults[i]}'
 
     annotations = ', '.join(annotations) or ''
     docstring = function.__doc__ if hasattr(function, '__doc__') else None
 
     signature = f'`{prepend}{name}({annotations})'
     if return_annotation:
-        if hasattr(return_annotation, '__name__'):
+        if '[' in str(return_annotation):
+            return_annotation = str(return_annotation)
+        elif hasattr(return_annotation, '__name__'):
             return_annotation = return_annotation.__name__
         signature += f' -> {return_annotation}'
     signature += ':` '
 
     doc = ''
 
     match format:
```

### Comparing `autodox-0.0.4.5/tests/test_hooks.py` & `autodox-0.0.4.6/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `autodox-0.0.4.5/license` & `autodox-0.0.4.6/license`

 * *Files identical despite different names*

### Comparing `autodox-0.0.4.5/pyproject.toml` & `autodox-0.0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autodox"
-version = "0.0.4.5"
+version = "0.0.4.6"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Tool for generating documentation automatically from code annotations, types, and docstrings."
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `autodox-0.0.4.5/readme.md` & `autodox-0.0.4.6/readme.md`

 * *Files identical despite different names*

### Comparing `autodox-0.0.4.5/PKG-INFO` & `autodox-0.0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodox
-Version: 0.0.4.5
+Version: 0.0.4.6
 Summary: Tool for generating documentation automatically from code annotations, types, and docstrings.
 Project-URL: Homepage, https://github.com/k98kurz/autodox
 Project-URL: Bug Tracker, https://github.com/k98kurz/autodox/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

