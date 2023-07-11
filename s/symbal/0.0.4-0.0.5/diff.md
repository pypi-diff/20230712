# Comparing `tmp/symbal-0.0.4.tar.gz` & `tmp/symbal-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbal-0.0.4.tar", last modified: Tue Jul 11 22:27:51 2023, max compression
+gzip compressed data, was "symbal-0.0.5.tar", last modified: Tue Jul 11 22:37:04 2023, max compression
```

## Comparing `symbal-0.0.4.tar` & `symbal-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 22:27:51.471892 symbal-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      666 2023-07-11 22:27:51.471892 symbal-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.4/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 22:27:51.472890 symbal-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-11 22:27:05.000000 symbal-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 22:27:51.464911 symbal-0.0.4/symbal/
--rw-rw-rw-   0        0        0      353 2023-07-11 22:27:05.000000 symbal-0.0.4/symbal/__init__.py
--rw-rw-rw-   0        0        0     3252 2023-07-11 22:27:05.000000 symbal-0.0.4/symbal/main.py
--rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.4/symbal/penalties.py
--rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.4/symbal/test_function.py
--rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.4/symbal/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 22:27:51.469898 symbal-0.0.4/symbal.egg-info/
--rw-rw-rw-   0        0        0      666 2023-07-11 22:27:51.000000 symbal-0.0.4/symbal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-11 22:27:51.000000 symbal-0.0.4/symbal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 22:27:51.000000 symbal-0.0.4/symbal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 22:27:51.000000 symbal-0.0.4/symbal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 22:37:04.838013 symbal-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      666 2023-07-11 22:37:04.837016 symbal-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.5/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 22:37:04.838013 symbal-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-11 22:36:55.000000 symbal-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 22:37:04.830035 symbal-0.0.5/symbal/
+-rw-rw-rw-   0        0        0      353 2023-07-11 22:36:55.000000 symbal-0.0.5/symbal/__init__.py
+-rw-rw-rw-   0        0        0     3259 2023-07-11 22:36:55.000000 symbal-0.0.5/symbal/main.py
+-rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.5/symbal/penalties.py
+-rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.5/symbal/test_function.py
+-rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.5/symbal/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 22:37:04.836018 symbal-0.0.5/symbal.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-07-11 22:37:04.000000 symbal-0.0.5/symbal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-11 22:37:04.000000 symbal-0.0.5/symbal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 22:37:04.000000 symbal-0.0.5/symbal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 22:37:04.000000 symbal-0.0.5/symbal.egg-info/top_level.txt
```

### Comparing `symbal-0.0.4/LICENSE` & `symbal-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `symbal-0.0.4/PKG-INFO` & `symbal-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

### Comparing `symbal-0.0.4/setup.py` & `symbal-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='symbal',
-    version='0.0.4',
+    version='0.0.5',
     author='Alex Summers',
     author_email='ajs0201@auburn.edu',
     description='A Python package for batch adaptive sampling with symbolic regression',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ajsummers/symbal',
     project_urls={
```

### Comparing `symbal-0.0.4/symbal/main.py` & `symbal-0.0.5/symbal/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             scores_other.append(score_other)
 
             x_cand = tf.candidates.drop('output', axis=1)
             predictions = np.empty((len(x_cand), len(pysr_model.equations_['equation'])))
 
             equation_best = pysr_model.predict(x_cand)
 
-            for j in range(pysr_model.equations_['equation']):
+            for j, _ in enumerate(pysr_model.equations_['equation']):
                 predictions[:, j] = pysr_model.predict(x_cand, j) - equation_best
 
             scores = np.array(pysr_model.equations_['score'])
 
             predictions_weight = predictions * scores
             uncertainty = np.sum(np.abs(predictions_weight), axis=1)
```

### Comparing `symbal-0.0.4/symbal/test_function.py` & `symbal-0.0.5/symbal/test_function.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.4/symbal/utils.py` & `symbal-0.0.5/symbal/utils.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.4/symbal.egg-info/PKG-INFO` & `symbal-0.0.5/symbal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

