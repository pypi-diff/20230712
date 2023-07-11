# Comparing `tmp/symbal-0.0.3.tar.gz` & `tmp/symbal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbal-0.0.3.tar", last modified: Tue Jul 11 22:23:02 2023, max compression
+gzip compressed data, was "symbal-0.0.4.tar", last modified: Tue Jul 11 22:27:51 2023, max compression
```

## Comparing `symbal-0.0.3.tar` & `symbal-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 22:23:02.450878 symbal-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      666 2023-07-11 22:23:02.450878 symbal-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.3/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 22:23:02.451875 symbal-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-10 19:44:08.000000 symbal-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 22:23:02.442900 symbal-0.0.3/symbal/
--rw-rw-rw-   0        0        0      353 2023-07-10 19:44:08.000000 symbal-0.0.3/symbal/__init__.py
--rw-rw-rw-   0        0        0     3104 2023-07-11 22:22:17.000000 symbal-0.0.3/symbal/main.py
--rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.3/symbal/penalties.py
--rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.3/symbal/test_function.py
--rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.3/symbal/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 22:23:02.448883 symbal-0.0.3/symbal.egg-info/
--rw-rw-rw-   0        0        0      666 2023-07-11 22:23:02.000000 symbal-0.0.3/symbal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-11 22:23:02.000000 symbal-0.0.3/symbal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 22:23:02.000000 symbal-0.0.3/symbal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 22:23:02.000000 symbal-0.0.3/symbal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 22:27:51.471892 symbal-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      666 2023-07-11 22:27:51.471892 symbal-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.4/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 22:27:51.472890 symbal-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-11 22:27:05.000000 symbal-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 22:27:51.464911 symbal-0.0.4/symbal/
+-rw-rw-rw-   0        0        0      353 2023-07-11 22:27:05.000000 symbal-0.0.4/symbal/__init__.py
+-rw-rw-rw-   0        0        0     3252 2023-07-11 22:27:05.000000 symbal-0.0.4/symbal/main.py
+-rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.4/symbal/penalties.py
+-rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.4/symbal/test_function.py
+-rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.4/symbal/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 22:27:51.469898 symbal-0.0.4/symbal.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-07-11 22:27:51.000000 symbal-0.0.4/symbal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-11 22:27:51.000000 symbal-0.0.4/symbal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 22:27:51.000000 symbal-0.0.4/symbal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 22:27:51.000000 symbal-0.0.4/symbal.egg-info/top_level.txt
```

### Comparing `symbal-0.0.3/LICENSE` & `symbal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `symbal-0.0.3/PKG-INFO` & `symbal-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

### Comparing `symbal-0.0.3/setup.py` & `symbal-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='symbal',
-    version='0.0.3',
+    version='0.0.4',
     author='Alex Summers',
     author_email='ajs0201@auburn.edu',
     description='A Python package for batch adaptive sampling with symbolic regression',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ajsummers/symbal',
     project_urls={
```

### Comparing `symbal-0.0.3/symbal/main.py` & `symbal-0.0.4/symbal/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 
 class SymbalTest:
 
     def __init__(self, function, min_vals, max_vals, iterations, batch_size, pysr_model, testfunction=None,
                  batch_config=None):
 
+        testfunction = dict() if testfunction is None else testfunction
+        batch_config = dict() if batch_config is None else batch_config
+
         self.captured_penalties = pd.DataFrame()
         self.selected_indices = []
 
         tf = TestFunction(function, min_vals, max_vals, **testfunction)
         self.initial_set = tf.initial_set
         self.candidates = tf.candidates
```

### Comparing `symbal-0.0.3/symbal/test_function.py` & `symbal-0.0.4/symbal/test_function.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.3/symbal/utils.py` & `symbal-0.0.4/symbal/utils.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.3/symbal.egg-info/PKG-INFO` & `symbal-0.0.4/symbal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

