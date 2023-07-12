# Comparing `tmp/symbal-0.0.5.tar.gz` & `tmp/symbal-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbal-0.0.5.tar", last modified: Tue Jul 11 22:37:04 2023, max compression
+gzip compressed data, was "symbal-0.0.6.tar", last modified: Wed Jul 12 16:50:22 2023, max compression
```

## Comparing `symbal-0.0.5.tar` & `symbal-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 22:37:04.838013 symbal-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      666 2023-07-11 22:37:04.837016 symbal-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.5/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 22:37:04.838013 symbal-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-11 22:36:55.000000 symbal-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 22:37:04.830035 symbal-0.0.5/symbal/
--rw-rw-rw-   0        0        0      353 2023-07-11 22:36:55.000000 symbal-0.0.5/symbal/__init__.py
--rw-rw-rw-   0        0        0     3259 2023-07-11 22:36:55.000000 symbal-0.0.5/symbal/main.py
--rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.5/symbal/penalties.py
--rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.5/symbal/test_function.py
--rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.5/symbal/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 22:37:04.836018 symbal-0.0.5/symbal.egg-info/
--rw-rw-rw-   0        0        0      666 2023-07-11 22:37:04.000000 symbal-0.0.5/symbal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-11 22:37:04.000000 symbal-0.0.5/symbal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 22:37:04.000000 symbal-0.0.5/symbal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 22:37:04.000000 symbal-0.0.5/symbal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 16:50:22.612990 symbal-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      666 2023-07-12 16:50:22.611992 symbal-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.6/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:50:22.612990 symbal-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-12 16:50:14.000000 symbal-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:50:22.605011 symbal-0.0.6/symbal/
+-rw-rw-rw-   0        0        0      353 2023-07-12 16:50:14.000000 symbal-0.0.6/symbal/__init__.py
+-rw-rw-rw-   0        0        0     3261 2023-07-12 16:50:14.000000 symbal-0.0.6/symbal/main.py
+-rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.6/symbal/penalties.py
+-rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.6/symbal/test_function.py
+-rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.6/symbal/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:50:22.610995 symbal-0.0.6/symbal.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-07-12 16:50:22.000000 symbal-0.0.6/symbal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-12 16:50:22.000000 symbal-0.0.6/symbal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:50:22.000000 symbal-0.0.6/symbal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 16:50:22.000000 symbal-0.0.6/symbal.egg-info/top_level.txt
```

### Comparing `symbal-0.0.5/LICENSE` & `symbal-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `symbal-0.0.5/PKG-INFO` & `symbal-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

### Comparing `symbal-0.0.5/setup.py` & `symbal-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='symbal',
-    version='0.0.5',
+    version='0.0.6',
     author='Alex Summers',
     author_email='ajs0201@auburn.edu',
     description='A Python package for batch adaptive sampling with symbolic regression',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ajsummers/symbal',
     project_urls={
```

### Comparing `symbal-0.0.5/symbal/main.py` & `symbal-0.0.6/symbal/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             selected_indices, captured_penalties = bs(np.array(x_cand), batch_size=batch_size, **batch_config)
             captured_penalties = captured_penalties.rename(columns={
                 column: f'{i+1}-{column}' for column in list(captured_penalties.columns)
             })
             self.captured_penalties = pd.concat([self.captured_penalties, captured_penalties], axis=1)
             self.selected_indices.append(selected_indices)
 
-            tf.inital_set = pd.concat([tf.inital_set, tf.candidates.loc[selected_indices, :]], axis=0)
+            tf.initial_set = pd.concat([tf.initial_set, tf.candidates.loc[selected_indices, :]], axis=0)
             tf.candidates = tf.candidates.drop(selected_indices, axis=0)
 
         scores_dict = {
             'equation': equations,
             'extrap': extrap_scores,
             'interp': interp_scores,
             'existing': existing_scores,
```

### Comparing `symbal-0.0.5/symbal/test_function.py` & `symbal-0.0.6/symbal/test_function.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.5/symbal/utils.py` & `symbal-0.0.6/symbal/utils.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.5/symbal.egg-info/PKG-INFO` & `symbal-0.0.6/symbal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

