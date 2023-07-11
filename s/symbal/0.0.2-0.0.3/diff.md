# Comparing `tmp/symbal-0.0.2.tar.gz` & `tmp/symbal-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbal-0.0.2.tar", last modified: Mon Jul 10 15:56:23 2023, max compression
+gzip compressed data, was "symbal-0.0.3.tar", last modified: Tue Jul 11 22:23:02 2023, max compression
```

## Comparing `symbal-0.0.2.tar` & `symbal-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:23.225362 symbal-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      666 2023-07-10 15:56:23.224364 symbal-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.2/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 15:56:23.225362 symbal-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-10 15:56:14.000000 symbal-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:23.217383 symbal-0.0.2/symbal/
--rw-rw-rw-   0        0        0      303 2023-07-10 15:56:14.000000 symbal-0.0.2/symbal/__init__.py
--rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.2/symbal/penalties.py
--rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.2/symbal/test_function.py
--rw-rw-rw-   0        0        0     2135 2023-07-09 21:47:00.000000 symbal-0.0.2/symbal/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:23.223366 symbal-0.0.2/symbal.egg-info/
--rw-rw-rw-   0        0        0      666 2023-07-10 15:56:23.000000 symbal-0.0.2/symbal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-10 15:56:23.000000 symbal-0.0.2/symbal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 15:56:23.000000 symbal-0.0.2/symbal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 15:56:23.000000 symbal-0.0.2/symbal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 22:23:02.450878 symbal-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      666 2023-07-11 22:23:02.450878 symbal-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.3/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 22:23:02.451875 symbal-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-10 19:44:08.000000 symbal-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 22:23:02.442900 symbal-0.0.3/symbal/
+-rw-rw-rw-   0        0        0      353 2023-07-10 19:44:08.000000 symbal-0.0.3/symbal/__init__.py
+-rw-rw-rw-   0        0        0     3104 2023-07-11 22:22:17.000000 symbal-0.0.3/symbal/main.py
+-rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.3/symbal/penalties.py
+-rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.3/symbal/test_function.py
+-rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.3/symbal/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 22:23:02.448883 symbal-0.0.3/symbal.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-07-11 22:23:02.000000 symbal-0.0.3/symbal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-11 22:23:02.000000 symbal-0.0.3/symbal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 22:23:02.000000 symbal-0.0.3/symbal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 22:23:02.000000 symbal-0.0.3/symbal.egg-info/top_level.txt
```

### Comparing `symbal-0.0.2/LICENSE` & `symbal-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `symbal-0.0.2/PKG-INFO` & `symbal-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

### Comparing `symbal-0.0.2/setup.py` & `symbal-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='symbal',
-    version='0.0.2',
+    version='0.0.3',
     author='Alex Summers',
     author_email='ajs0201@auburn.edu',
     description='A Python package for batch adaptive sampling with symbolic regression',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ajsummers/symbal',
     project_urls={
```

### Comparing `symbal-0.0.2/symbal/test_function.py` & `symbal-0.0.3/symbal/test_function.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.2/symbal/utils.py` & `symbal-0.0.3/symbal/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 
 import numpy as np
 from symbal.penalties import invquad_penalty
+import pandas as pd
 
 
 def new_penalty(penalty_array, penalty_function, a, b, by_range, batch_size):
     """
     Selects maximum from given values and penalizes area around selection.
 
     Assumes first column in penalty_array is penalized value, other columns are
     independent variables.
 
     Returns: independent variables for selected point & new penalty_array w/ penalized values
     """
 
-    max_index = np.argmax(penalty_array[:, 0])  # index for largest value
+    max_index = np.nanargmax(penalty_array[:, 0])  # index for largest value
+    penalty_array[max_index, 0] = np.nan
     max_pos = penalty_array[max_index, 1:]  # independent variable values for this index
-    new_array = np.delete(penalty_array, max_index, axis=0)  # Remove selected value from array
 
-    r_x = np.abs(new_array[:, 1:] - max_pos)  # Distance to selected point for each variable
+    r_x = np.abs(penalty_array[:, 1:] - max_pos)  # Distance to selected point for each variable
     if by_range:
-        s_x = np.ptp(new_array[:, 1:], axis=0) / batch_size  # Tune width of penalty by range / batch_size
+        s_x = np.ptp(penalty_array[:, 1:], axis=0) / batch_size  # Tune width of penalty by range / batch_size
     else:
-        s_x = np.std(new_array[:, 1:],
+        s_x = np.std(penalty_array[:, 1:],
                      axis=0)  # Tune width of penalty by standard deviation of each independent variable
-    s_y = np.std(new_array[:, 0], axis=0)  # Standard deviation of penalized value
+    s_y = np.nanstd(penalty_array[:, 0], axis=0)  # Standard deviation of penalized value
 
     penalty = penalty_function(a, b, r_x, s_x, s_y)
+    penalty_array[:, 0] -= penalty  # subtract penalty
 
-    new_array[:, 0] -= penalty  # subtract penalty
+    return max_index, penalty_array
 
-    return max_pos, new_array
 
+def batch_selection(uncertainty_array, penalty_function=invquad_penalty, a=1, b=1, by_range=False, batch_size=10):
 
-def batch_selection(uncertainty_array, penalty_function=invquad_penalty, a=1, b=1, by_range=False, batch_size=10,
-                    capture_penalties=False):
+    captured_penalties = pd.DataFrame()
+    selected_indices = []
+    penalty_array = uncertainty_array
 
-    captured_penalties = dict()
+    for i in range(batch_size):
 
-    if capture_penalties:
-        captured_penalties[0] = uncertainty_array
+        selected_index, penalty_array = new_penalty(penalty_array, penalty_function, a, b, by_range, batch_size)
 
-    selected_points = np.empty((batch_size, uncertainty_array.shape[1] - 1))
-    penalty_array = uncertainty_array
+        captured_penalties[f'{i}'] = penalty_array[:, 0]
+        selected_indices.append(selected_index)
 
-    for i in range(batch_size):
+    return selected_indices, captured_penalties
 
-        selected_point, penalty_array = new_penalty(penalty_array, penalty_function, a, b, by_range, batch_size)
 
-        if capture_penalties:
-            captured_penalties[i+1] = penalty_array
+def get_score(input_df, pysr_model):
 
-        selected_points[i, :] = selected_point
+    predicted = pysr_model.predict(input_df)
+    actual = np.array(input_df['output'])
+    score = np.mean(np.abs(predicted - actual))
 
-    if capture_penalties:
-        return selected_points, captured_penalties
-    else:
-        return selected_points
+    return score
+
+
+def get_metrics(pysr_model):
+
+    best_index = np.argmax(pysr_model.equations_['score'])
+    equation = pysr_model.equations_.loc[best_index, 'equation']
+    loss = pysr_model.equations_.loc[best_index, 'loss']
+    score = pysr_model.equations_.loc[best_index, 'score']
+
+    other_equations = pysr_model.equations_.drop(best_index, axis=0)
+    loss_other = np.mean(other_equations['loss'])
+    score_other = np.mean(other_equations['score'])
+
+    return equation, loss, score, loss_other, score_other
```

### Comparing `symbal-0.0.2/symbal.egg-info/PKG-INFO` & `symbal-0.0.3/symbal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

