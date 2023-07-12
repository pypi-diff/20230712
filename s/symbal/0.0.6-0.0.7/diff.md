# Comparing `tmp/symbal-0.0.6.tar.gz` & `tmp/symbal-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbal-0.0.6.tar", last modified: Wed Jul 12 16:50:22 2023, max compression
+gzip compressed data, was "symbal-0.0.7.tar", last modified: Wed Jul 12 17:14:15 2023, max compression
```

## Comparing `symbal-0.0.6.tar` & `symbal-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 16:50:22.612990 symbal-0.0.6/
--rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      666 2023-07-12 16:50:22.611992 symbal-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.6/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 16:50:22.612990 symbal-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-12 16:50:14.000000 symbal-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:50:22.605011 symbal-0.0.6/symbal/
--rw-rw-rw-   0        0        0      353 2023-07-12 16:50:14.000000 symbal-0.0.6/symbal/__init__.py
--rw-rw-rw-   0        0        0     3261 2023-07-12 16:50:14.000000 symbal-0.0.6/symbal/main.py
--rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.6/symbal/penalties.py
--rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.6/symbal/test_function.py
--rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.6/symbal/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:50:22.610995 symbal-0.0.6/symbal.egg-info/
--rw-rw-rw-   0        0        0      666 2023-07-12 16:50:22.000000 symbal-0.0.6/symbal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-12 16:50:22.000000 symbal-0.0.6/symbal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 16:50:22.000000 symbal-0.0.6/symbal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 16:50:22.000000 symbal-0.0.6/symbal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 17:14:15.709661 symbal-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      666 2023-07-12 17:14:15.709661 symbal-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.7/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 17:14:15.709661 symbal-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-12 17:14:11.000000 symbal-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:14:15.702467 symbal-0.0.7/symbal/
+-rw-rw-rw-   0        0        0      353 2023-07-12 17:14:11.000000 symbal-0.0.7/symbal/__init__.py
+-rw-rw-rw-   0        0        0     3276 2023-07-12 17:14:11.000000 symbal-0.0.7/symbal/main.py
+-rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.7/symbal/penalties.py
+-rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.7/symbal/test_function.py
+-rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.7/symbal/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:14:15.707667 symbal-0.0.7/symbal.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-07-12 17:14:15.000000 symbal-0.0.7/symbal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-12 17:14:15.000000 symbal-0.0.7/symbal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 17:14:15.000000 symbal-0.0.7/symbal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 17:14:15.000000 symbal-0.0.7/symbal.egg-info/top_level.txt
```

### Comparing `symbal-0.0.6/LICENSE` & `symbal-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `symbal-0.0.6/PKG-INFO` & `symbal-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

### Comparing `symbal-0.0.6/setup.py` & `symbal-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='symbal',
-    version='0.0.6',
+    version='0.0.7',
     author='Alex Summers',
     author_email='ajs0201@auburn.edu',
     description='A Python package for batch adaptive sampling with symbolic regression',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ajsummers/symbal',
     project_urls={
```

### Comparing `symbal-0.0.6/symbal/main.py` & `symbal-0.0.7/symbal/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.selected_indices = []
 
         tf = TestFunction(function, min_vals, max_vals, **testfunction)
         self.initial_set = tf.initial_set
         self.candidates = tf.candidates
 
         equations, extrap_scores, interp_scores, existing_scores = [[], [], [], []]
-        losses, scores, losses_other, scores_other = [[], [], [], []]
+        losses, best_scores, losses_other, scores_other = [[], [], [], []]
 
         for i in range(iterations):
 
             x_train = tf.initial_set.drop('output', axis=1)
             y_train = tf.initial_set['output']
 
             pysr_model.fit(x_train, y_train)
@@ -34,15 +34,15 @@
             extrap_scores.append(get_score(tf.extrapolation_testset, pysr_model))
             interp_scores.append(get_score(tf.interpolation_testset, pysr_model))
             existing_scores.append(get_score(tf.initial_set, pysr_model))
 
             equation, loss, score, loss_other, score_other = get_metrics(pysr_model)
             equations.append(equation)
             losses.append(loss)
-            scores.append(score)
+            best_scores.append(score)
             losses_other.append(loss_other)
             scores_other.append(score_other)
 
             x_cand = tf.candidates.drop('output', axis=1)
             predictions = np.empty((len(x_cand), len(pysr_model.equations_['equation'])))
 
             equation_best = pysr_model.predict(x_cand)
@@ -69,12 +69,12 @@
 
         scores_dict = {
             'equation': equations,
             'extrap': extrap_scores,
             'interp': interp_scores,
             'existing': existing_scores,
             'loss': losses,
-            'score': scores,
+            'score': best_scores,
             'loss_other': losses_other,
             'score_other': scores_other
         }
         self.scores = pd.DataFrame(scores_dict)
```

### Comparing `symbal-0.0.6/symbal/test_function.py` & `symbal-0.0.7/symbal/test_function.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.6/symbal/utils.py` & `symbal-0.0.7/symbal/utils.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.6/symbal.egg-info/PKG-INFO` & `symbal-0.0.7/symbal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

