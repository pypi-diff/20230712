# Comparing `tmp/wizlib-0.3.0.tar.gz` & `tmp/wizlib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.3.0.tar", last modified: Sat Jul  8 17:25:39 2023, max compression
+gzip compressed data, was "wizlib-0.5.1.tar", last modified: Wed Jul 12 03:03:58 2023, max compression
```

## Comparing `wizlib-0.3.0.tar` & `wizlib-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:25:39.706326 wizlib-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-08 17:24:50.000000 wizlib-0.3.0/.version
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-08 17:25:39.706326 wizlib-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1506 2023-07-08 17:25:31.000000 wizlib-0.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-08 17:25:31.000000 wizlib-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 17:25:39.706326 wizlib-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:25:39.704326 wizlib-0.3.0/test/
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-08 17:25:31.000000 wizlib-0.3.0/test/test_super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:25:39.704326 wizlib-0.3.0/wizlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:25:31.000000 wizlib-0.3.0/wizlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2023-07-08 17:25:31.000000 wizlib-0.3.0/wizlib/rlinput.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-08 17:25:31.000000 wizlib-0.3.0/wizlib/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:25:39.705326 wizlib-0.3.0/wizlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      270 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:03:58.147327 wizlib-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-12 03:03:04.000000 wizlib-0.5.1/.version
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-12 03:03:58.147327 wizlib-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2023-07-12 03:03:48.000000 wizlib-0.5.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-12 03:03:48.000000 wizlib-0.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 03:03:58.147327 wizlib-0.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:03:58.145327 wizlib-0.5.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-12 03:03:48.000000 wizlib-0.5.1/test/test_class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-12 03:03:48.000000 wizlib-0.5.1/test/test_super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:03:58.145327 wizlib-0.5.1/wizlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 03:03:48.000000 wizlib-0.5.1/wizlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-07-12 03:03:48.000000 wizlib-0.5.1/wizlib/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-07-12 03:03:48.000000 wizlib-0.5.1/wizlib/rlinput.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-12 03:03:48.000000 wizlib-0.5.1/wizlib/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:03:58.146327 wizlib-0.5.1/wizlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 03:03:58.000000 wizlib-0.5.1/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.3.0/PKG-INFO` & `wizlib-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.3.0
+Version: 0.5.1
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

### Comparing `wizlib-0.3.0/README.md` & `wizlib-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-0.3.0/pyproject.toml` & `wizlib-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.3.0/test/test_super_wrapper.py` & `wizlib-0.5.1/wizlib/super_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from unittest import TestCase
-from unittest.mock import patch
-from io import StringIO
-
-from wizlib.super_wrapper import SuperWrapper
-
-
-class TestSuperWrapper(TestCase):
-
-    def test_super_wrapper(self):
-
-        class Parent(SuperWrapper):
-            def execute(self, method, *args, **kwargs):
-                print(f"Parent execute before")
-                method(self, *args, **kwargs)
-                print(f"Parent execute after")
-
-        class InBetween(Parent):
-            @Parent.wrap
-            def execute(self, method, *args, **kwargs):
-                print(f"IB execute before")
-                method(self, *args, **kwargs)
-                print(f"IB execute after")
-
-        class NewChild(InBetween):
-            @InBetween.wrap
-            def execute(self, name):
-                print(f"Hello {name}")
-
-        with patch('sys.stdout', o:=StringIO()):
-            c = NewChild()
-            c.execute("Jane")
-        o.seek(0)
-        r = o.read()
-        self.assertEqual(r, "Parent execute before\nIB execute before\nHello Jane\nIB execute after\nParent execute after\n")
-
+# Provide a decorator to wrap a method so that it's called within the inherited
+# version of that method.
+#
+# Example of use:
+#
+# class Parent(SuperWrapper):
+#     def execute(self, method, *args, **kwargs):
+#         print(f"Parent execute before")
+#         method(self, *args, **kwargs)
+#         print(f"Parent execute after")
+#
+# class InBetween(Parent):
+#     @Parent.wrap
+#     def execute(self, method, *args, **kwargs):
+#         print(f"IB execute before")
+#         method(self, *args, **kwargs)
+#         print(f"IB execute after")
+#
+# class NewChild(InBetween):
+#     @InBetween.wrap
+#     def execute(self, name):
+#         print(f"Hello {name}")
+#
+# c = NewChild()
+# c.execute("Jane")
+
+
+class SuperWrapper:
+    @classmethod
+    def wrap(parent_class, method):
+        def wrapper(self, *args, **kwargs):
+            parent_method = getattr(parent_class, method.__name__)
+            return parent_method(self, method, *args, **kwargs)
+        return wrapper
```

### Comparing `wizlib-0.3.0/wizlib/rlinput.py` & `wizlib-0.5.1/wizlib/rlinput.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 
 
 # Readline defaults to complete with local filenames. Definitely not what we
 # want.
 
 def null_complete(text, start):
     return None
+
+
 readline.set_completer(null_complete)
 
 
-def rlinput(prompt:str="", default:str="", options:list=None):
+def rlinput(prompt: str = "", default: str = "", options: list = None):
     """
     Get input with preset default and/or tab completion of options
 
     Parameters:
 
     prompt:str - string to output before requesting input, same as in the
     input() function
@@ -53,14 +55,16 @@
     try:
         value = input(prompt)
     finally:
         readline.set_startup_hook()
         readline.set_completer(null_complete)
     return value.strip()
 
+
 def tryit():
     """Quick and dirty tester function"""
-    return rlinput(prompt='>', \
-            options=['a-b','a-c','b-a'])
+    return rlinput(prompt='>',
+                   options=['a-b', 'a-c', 'b-a'])
+
 
 if __name__ == '__main__':
-    tryit()
+    tryit()
```

### Comparing `wizlib-0.3.0/wizlib/super_wrapper.py` & `wizlib-0.5.1/test/test_super_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,51 @@
-# Provide a decorator to wrap a method so that it's called within the inherited
-# version of that method.
-#
-# Example of use:
-#
-# class Parent(SuperWrapper):
-#     def execute(self, method, *args, **kwargs):
-#         print(f"Parent execute before")
-#         method(self, *args, **kwargs)
-#         print(f"Parent execute after")
-#
-# class InBetween(Parent):
-#     @Parent.wrap
-#     def execute(self, method, *args, **kwargs):
-#         print(f"IB execute before")
-#         method(self, *args, **kwargs)
-#         print(f"IB execute after")
-#
-# class NewChild(InBetween):
-#     @InBetween.wrap
-#     def execute(self, name):
-#         print(f"Hello {name}")
-#
-# c = NewChild()
-# c.execute("Jane")
-
-
-class SuperWrapper:
-    @classmethod
-    def wrap(parent_class, method):
-        def wrapper(self, *args, **kwargs):
-            parent_method = getattr(parent_class, method.__name__)
-            return parent_method(self, method, *args, **kwargs)
-        return wrapper
+from unittest import TestCase
+from unittest.mock import patch
+from io import StringIO
+
+from wizlib.super_wrapper import SuperWrapper
+
+correct = """
+Parent execute before
+IB execute before
+    Hello Jane
+    IB execute after
+    Parent execute after
+"""
+
+
+class TestSuperWrapper(TestCase):
+
+    def test_super_wrapper(self):
+
+        class Parent(SuperWrapper):
+            def execute(self, method, *args, **kwargs):
+                print(f"Parent execute before")
+                method(self, *args, **kwargs)
+                print(f"Parent execute after")
+
+        class InBetween(Parent):
+            @Parent.wrap
+            def execute(self, method, *args, **kwargs):
+                print(f"IB execute before")
+                method(self, *args, **kwargs)
+                print(f"IB execute after")
+
+        class NewChild(InBetween):
+            @InBetween.wrap
+            def execute(self, name):
+                print(f"Hello {name}")
+
+        with patch('sys.stdout', o := StringIO()):
+            c = NewChild()
+            c.execute("Jane")
+        o.seek(0)
+        r = o.read()
+        correct = """
+            Parent execute before
+            IB execute before
+            Hello Jane
+            IB execute after
+            Parent execute after
+        """.lstrip().split('\n')
+        correct_clean = '\n'.join([i.lstrip() for i in correct])
+        self.assertEqual(r, correct_clean)
```

### Comparing `wizlib-0.3.0/wizlib.egg-info/PKG-INFO` & `wizlib-0.5.1/wizlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.3.0
+Version: 0.5.1
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

