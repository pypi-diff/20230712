# Comparing `tmp/pybond-0.1.9.tar.gz` & `tmp/pybond-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybond-0.1.9.tar", max compression
+gzip compressed data, was "pybond-0.2.0.tar", max compression
```

## Comparing `pybond-0.1.9.tar` & `pybond-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3030 2023-07-11 20:10:22.266214 pybond-0.1.9/README.md
--rw-r--r--   0        0        0      385 2023-01-23 06:22:02.588103 pybond-0.1.9/pybond/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-14 22:59:40.370502 pybond-0.1.9/pybond/assertions.py
--rw-r--r--   0        0        0     5696 2023-07-11 20:10:22.266567 pybond-0.1.9/pybond/james.py
--rw-r--r--   0        0        0      633 2023-05-15 00:58:17.181063 pybond-0.1.9/pybond/memory.py
--rw-r--r--   0        0        0      400 2023-05-15 16:32:17.555194 pybond-0.1.9/pybond/types.py
--rw-r--r--   0        0        0     2017 2023-05-15 16:32:17.555907 pybond-0.1.9/pybond/util.py
--rw-r--r--   0        0        0      984 2023-07-11 20:10:22.266815 pybond-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 pybond-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     3014 2023-07-12 14:17:19.545774 pybond-0.2.0/README.md
+-rw-r--r--   0        0        0      385 2023-01-23 06:22:02.588103 pybond-0.2.0/pybond/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-14 22:59:40.370502 pybond-0.2.0/pybond/assertions.py
+-rw-r--r--   0        0        0     5701 2023-07-12 14:17:19.546088 pybond-0.2.0/pybond/james.py
+-rw-r--r--   0        0        0      633 2023-05-15 00:58:17.181063 pybond-0.2.0/pybond/memory.py
+-rw-r--r--   0        0        0      345 2023-07-12 14:17:19.546481 pybond-0.2.0/pybond/types.py
+-rw-r--r--   0        0        0     2017 2023-05-15 16:32:17.555907 pybond-0.2.0/pybond/util.py
+-rw-r--r--   0        0        0      984 2023-07-12 14:17:19.546810 pybond-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 pybond-0.2.0/PKG-INFO
```

### Comparing `pybond-0.1.9/README.md` & `pybond-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 [clojure `bond` library](https://github.com/circleci/bond/).
 
 ## Installation
 
 pip
 
 ```bash
-pip install pybond==0.1.9
+pip install pybond==0.2.0
 ```
 
 requirements.txt
 
 ```python
-pybond==0.1.9
+pybond==0.2.0
 ```
 
 pyproject.toml
 
 ```toml
-pybond = "0.1.9"
+pybond = "0.2.0"
 ```
 
 ## Example usage
 
 Let's say you wanted to test the functions in this module:
 
 ```python
@@ -56,29 +56,29 @@
 
 import sample_code.other_package as other_package
 import sample_code.my_module as my_module
 from sample_code.my_module import bar
 
 
 def test_foo_is_called():
-    with spy([my_module, "foo"]):
+    with spy(my_module.foo):
         assert times_called(my_module.foo, 0)
         bar(42)
         assert times_called(my_module.foo, 1)
         bar(42)
         bar(42)
         assert times_called(my_module.foo, 3)
 
 
 def test_bar_handles_response():
     with stub(
-        [other_package, "make_a_network_request", lambda x: {"result": x * 2}],
-        [other_package, "write_to_disk", lambda _: None],
+        (other_package.make_a_network_request, lambda x: {"result": x * 2}),
+        (other_package.write_to_disk, lambda _: None),
     ), spy(
-        [my_module, "foo"],
+        my_module.foo,
     ):
         assert times_called(my_module.foo, 0)
         assert times_called(other_package.make_a_network_request, 0)
         assert bar(21) == {"result": 42}
         assert times_called(my_module.foo, 1)
         assert times_called(other_package.make_a_network_request, 1)
         assert called_with_args(my_module.foo, args=[21])
```

### Comparing `pybond-0.1.9/pybond/assertions.py` & `pybond-0.2.0/pybond/assertions.py`

 * *Files identical despite different names*

### Comparing `pybond-0.1.9/pybond/james.py` & `pybond-0.2.0/pybond/james.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,32 +142,35 @@
     Context manager which takes a list of targets to stub and spy on.
 
     Example usage:
 
     ```
     import my_module
 
-    with stub([my_module, "test_function", lambda x: 42]):
+    with stub((my_module.test_function, lambda x: 42)):
         assert my_module.test_function("abc") == 42  # True
         function_calls = calls(my_module.test_function)
     ```
     """
     with MonkeyPatch.context() as m:
         try:
-            for module, obj_name, stub_obj in targets:
-                original_obj = getattr(module, obj_name)
-                new_obj = _instrumented_obj(original_obj, stub_obj, strict)
+            for target, stub_obj in targets:
+                new_obj = _instrumented_obj(target, stub_obj, strict)
 
                 # The following only covers imports in the form:
                 #     `import some_module`
-                m.setattr(target=module, name=obj_name, value=new_obj)
+                m.setattr(
+                    target=sys.modules[target.__module__],
+                    name=target.__name__,
+                    value=new_obj,
+                )
 
                 # The following covers bound imports in the form:
                 #     `from some_module import some_object`
-                replace_bound_references_in_memory(m, original_obj, new_obj)
+                replace_bound_references_in_memory(m, target, new_obj)
 
             yield
         except Exception:
             raise
 
 
 @contextmanager
@@ -175,14 +178,14 @@
     """
     Context manager which takes a list of targets to spy on.
 
     Example usage:
 
     ```
     import my_module
-    with spy([my_module, "test_function"]):
+    with spy(my_module.test_function):
         my_module.test_function("abc")
         function_calls = calls(my_module.test_function)
     ```
     """
-    with stub(*[(m, n, getattr(m, n)) for m, n in targets]):
+    with stub(*[(t, t) for t in targets]):
         yield
```

### Comparing `pybond-0.1.9/pybond/memory.py` & `pybond-0.2.0/pybond/memory.py`

 * *Files identical despite different names*

### Comparing `pybond-0.1.9/pybond/util.py` & `pybond-0.2.0/pybond/util.py`

 * *Files identical despite different names*

### Comparing `pybond-0.1.9/pyproject.toml` & `pybond-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybond"
-version = "0.1.9"
+version = "0.2.0"
 description = "pybond is a spying and stubbing library inspired by the clojure bond library."
 authors = ["Guillaume Pelletier <guigui.p@gmail.com>"]
 license = "Eclipse Public License - v 1.0"
 readme = "README.md"
 homepage = "https://github.com/epgui/pybond"
 repository = "https://github.com/epgui/pybond"
 keywords = [
```

### Comparing `pybond-0.1.9/PKG-INFO` & `pybond-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybond
-Version: 0.1.9
+Version: 0.2.0
 Summary: pybond is a spying and stubbing library inspired by the clojure bond library.
 Home-page: https://github.com/epgui/pybond
 License: Eclipse Public License - v 1.0
 Keywords: bond,monkeypatch,spy,stub,clojure,functional programming
 Author: Guillaume Pelletier
 Author-email: guigui.p@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -30,27 +30,27 @@
 [clojure `bond` library](https://github.com/circleci/bond/).
 
 ## Installation
 
 pip
 
 ```bash
-pip install pybond==0.1.9
+pip install pybond==0.2.0
 ```
 
 requirements.txt
 
 ```python
-pybond==0.1.9
+pybond==0.2.0
 ```
 
 pyproject.toml
 
 ```toml
-pybond = "0.1.9"
+pybond = "0.2.0"
 ```
 
 ## Example usage
 
 Let's say you wanted to test the functions in this module:
 
 ```python
@@ -79,29 +79,29 @@
 
 import sample_code.other_package as other_package
 import sample_code.my_module as my_module
 from sample_code.my_module import bar
 
 
 def test_foo_is_called():
-    with spy([my_module, "foo"]):
+    with spy(my_module.foo):
         assert times_called(my_module.foo, 0)
         bar(42)
         assert times_called(my_module.foo, 1)
         bar(42)
         bar(42)
         assert times_called(my_module.foo, 3)
 
 
 def test_bar_handles_response():
     with stub(
-        [other_package, "make_a_network_request", lambda x: {"result": x * 2}],
-        [other_package, "write_to_disk", lambda _: None],
+        (other_package.make_a_network_request, lambda x: {"result": x * 2}),
+        (other_package.write_to_disk, lambda _: None),
     ), spy(
-        [my_module, "foo"],
+        my_module.foo,
     ):
         assert times_called(my_module.foo, 0)
         assert times_called(other_package.make_a_network_request, 0)
         assert bar(21) == {"result": 42}
         assert times_called(my_module.foo, 1)
         assert times_called(other_package.make_a_network_request, 1)
         assert called_with_args(my_module.foo, args=[21])
```

