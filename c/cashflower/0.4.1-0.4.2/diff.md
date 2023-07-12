# Comparing `tmp/cashflower-0.4.1.tar.gz` & `tmp/cashflower-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.4.1.tar", last modified: Fri Jul  7 18:02:55 2023, max compression
+gzip compressed data, was "cashflower-0.4.2.tar", last modified: Wed Jul 12 19:30:35 2023, max compression
```

## Comparing `cashflower-0.4.1.tar` & `cashflower-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-07 18:02:44.000000 cashflower-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 18:02:44.000000 cashflower-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-07 18:02:55.895984 cashflower-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-07 18:02:44.000000 cashflower-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/cashflower/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/model_tpl/model.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/model_tpl/run.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:02:55.895984 cashflower-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 18:02:44.000000 cashflower-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-07 18:02:44.000000 cashflower-0.4.1/tests/test_cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-07 18:02:44.000000 cashflower-0.4.1/tests/test_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-07 18:02:44.000000 cashflower-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-12 19:30:21.000000 cashflower-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 19:30:21.000000 cashflower-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-12 19:30:35.348088 cashflower-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-12 19:30:21.000000 cashflower-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/model_tpl/model.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/model_tpl/run.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 19:30:35.348088 cashflower-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-12 19:30:21.000000 cashflower-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-12 19:30:21.000000 cashflower-0.4.2/tests/test_cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-12 19:30:21.000000 cashflower-0.4.2/tests/test_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-12 19:30:21.000000 cashflower-0.4.2/tests/test_utils.py
```

### Comparing `cashflower-0.4.1/LICENSE` & `cashflower-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.1/PKG-INFO` & `cashflower-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.1
+Version: 0.4.2
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
@@ -41,46 +41,31 @@
 create_model("my_model")
 ```
 
 ## Input
 
 my_model/input.py
 ```python
-main = ModelPointSet(data=pd.read_csv("C:/my_data/main.csv"))
+runplan = Runplan(data=pd.DataFrame({"version": [1]}))
 
-assumption = dict()
-assumption["interest_rates"] = pd.read_csv("C:/my_data/interest_rates.csv")
-assumption["mortality"] = pd.read_csv("C:/my_data/mortality.csv", index_col="age")
+main = ModelPointSet(data=pd.DataFrame({"id": [1]}))
 ```
 
 ## Model
 
 my_model/model.py
 ```python
 @variable()
-def age(t):
+def projection_year(t):
     if t == 0:
-        return int(main.get("AGE"))
-    elif t % 12 == 0:
-        return age(t-1) + 1
+        return 0
+    elif t % 12 == 1:
+        return projection_year(t - 1) + 1
     else:
-        return age(t-1)
-
-
-@variable()
-def death_prob(t):
-    if age(t) == age(t-1):
-        return death_prob(t-1) 
-    elif age(t) <= 100:
-        sex = main.get("SEX")
-        yearly_rate = assumption["mortality"].loc[age(t)][sex]
-        monthly_rate = (1 - (1 - yearly_rate)**(1/12))
-        return monthly_rate
-    else:
-        return 1
+        return projection_year(t - 1)
 ```
 
 ## Calculate
 
 Run `run.py`
 
 # Contribution
```

### Comparing `cashflower-0.4.1/README.md` & `cashflower-0.4.2/cashflower.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: cashflower
+Version: 0.4.2
+Summary: Framework for actuarial cash flow models
+Home-page: https://github.com/acturtle/cashflower
+Author: Zuzanna Chmielewska
+Project-URL: Source, https://github.com/acturtle/cashflower
+Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
+Project-URL: Documentation, https://cashflower.acturtle.com
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cashflower.svg)](https://pypi.org/project/cashflower/)
 [![pytest](https://github.com/acturtle/cashflower/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/acturtle/cashflower/actions/workflows/pytest.yml)
 [![Documentation Status](https://readthedocs.org/projects/cashflower/badge/)](https://cashflower.acturtle.com)
 
 # Info
 
 Cashflower is an open-source Python framework for actuarial cash flow models.
@@ -28,46 +41,31 @@
 create_model("my_model")
 ```
 
 ## Input
 
 my_model/input.py
 ```python
-main = ModelPointSet(data=pd.read_csv("C:/my_data/main.csv"))
+runplan = Runplan(data=pd.DataFrame({"version": [1]}))
 
-assumption = dict()
-assumption["interest_rates"] = pd.read_csv("C:/my_data/interest_rates.csv")
-assumption["mortality"] = pd.read_csv("C:/my_data/mortality.csv", index_col="age")
+main = ModelPointSet(data=pd.DataFrame({"id": [1]}))
 ```
 
 ## Model
 
 my_model/model.py
 ```python
 @variable()
-def age(t):
+def projection_year(t):
     if t == 0:
-        return int(main.get("AGE"))
-    elif t % 12 == 0:
-        return age(t-1) + 1
-    else:
-        return age(t-1)
-
-
-@variable()
-def death_prob(t):
-    if age(t) == age(t-1):
-        return death_prob(t-1) 
-    elif age(t) <= 100:
-        sex = main.get("SEX")
-        yearly_rate = assumption["mortality"].loc[age(t)][sex]
-        monthly_rate = (1 - (1 - yearly_rate)**(1/12))
-        return monthly_rate
+        return 0
+    elif t % 12 == 1:
+        return projection_year(t - 1) + 1
     else:
-        return 1
+        return projection_year(t - 1)
 ```
 
 ## Calculate
 
 Run `run.py`
 
 # Contribution
```

### Comparing `cashflower-0.4.1/cashflower/cashflow.py` & `cashflower-0.4.2/cashflower/cashflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,17 @@
         self.variables = sorted(self.variables, key=lambda x: (x.calc_order, x.name))
 
         # Get calc_direction of calculation
         max_calc_order = self.variables[-1].calc_order
         for calc_order in range(1, max_calc_order+1):
             # Either a single variable or a cycle
             variables = [variable for variable in self.variables if variable.calc_order == calc_order]
-            get_calc_direction(variables)
+            calc_direction = get_calc_direction(variables)
+            for variable in variables:
+                variable.calc_direction = calc_direction
 
         # Iterate over model points
         main = get_object_by_name(self.model_point_sets, "main")
         print_log(f"Total number of model points: {main.data.shape[0]}", one_core)
         if one_core and self.settings["MULTIPROCESSING"]:
             if len(main) > self.cpu_count:
                 print_log(f"Multiprocessing on {self.cpu_count} cores")
```

### Comparing `cashflower-0.4.1/cashflower/graph.py` & `cashflower-0.4.2/cashflower/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,21 +26,34 @@
 
 
 def get_calc_direction(variables):
     """Set calculation direction to irrelevant/forward/backward"""
     # For non-cycle => single variable, for cycle => variables from the cycle
     variable_names = [variable.name for variable in variables]
 
-    visitor = CalcDirectionVisitor(variable_names)
     for variable in variables:
         node = ast.parse(inspect.getsource(variable.func))
-        visitor.visit(node)
-        variable.calc_direction = visitor.calc_direction
+        for subnode in ast.walk(node):
+            if isinstance(subnode, ast.Call):
+                if isinstance(subnode.func, ast.Name):  # not a method
+                    if subnode.func.id in variable_names:  # single variable or another variable in the cycle
+                        arg = subnode.args[0]
+                        if isinstance(arg, ast.BinOp):
+                            # Does it call t+... or t-...?
+                            check1 = isinstance(arg.left, ast.Name) and arg.left.id == "t"
+                            check2 = isinstance(arg.op, ast.Add)
+                            check3 = isinstance(arg.op, ast.Sub)
 
-    return None
+                            if check1 and check2:
+                                return "backward"
+
+                            if check1 and check3:
+                                return "forward"
+
+    return "irrelevant"
 
 
 def get_predecessors(node, DG):
     """Get predecessors and their predecessors and their..."""
     queue = Queue()
     visited = []
 
@@ -86,30 +99,7 @@
         check3 = isinstance(arg.right, ast.Constant) and isinstance(arg.right.value, int)
         if not (check1 and check2 and check3):
             raise CashflowModelError(msg)
 
     # The model variable calls something else
     if not (isinstance(arg, ast.Name) or isinstance(arg, ast.Constant) or isinstance(arg, ast.BinOp)):
         raise CashflowModelError(msg)
-
-
-class CalcDirectionVisitor(ast.NodeVisitor):
-    def __init__(self, variable_names):
-        self.variable_names = variable_names
-        self.calc_direction = "irrelevant"
-
-    def visit_Call(self, node):
-        if isinstance(node.func, ast.Name):
-            if node.func.id in self.variable_names:
-                arg = node.args[0]
-                if isinstance(arg, ast.BinOp):
-                    # Does it call t+... or t-...?
-                    check1 = isinstance(arg.left, ast.Name) and arg.left.id == "t"
-                    check2 = isinstance(arg.op, ast.Add)
-                    check3 = isinstance(arg.op, ast.Sub)
-
-                    if check1 and check2:
-                        self.calc_direction = "backward"
-
-                    if check1 and check3:
-                        self.calc_direction = "forward"
-        return None
```

### Comparing `cashflower-0.4.1/cashflower/start.py` & `cashflower-0.4.2/cashflower/start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.1/cashflower/utils.py` & `cashflower-0.4.2/cashflower/utils.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.1/cashflower.egg-info/SOURCES.txt` & `cashflower-0.4.2/cashflower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.1/setup.py` & `cashflower-0.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     project_urls={
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.4.1",
+    version="0.4.2",
 )
```

### Comparing `cashflower-0.4.1/tests/test_cashflow.py` & `cashflower-0.4.2/tests/test_cashflow.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.1/tests/test_start.py` & `cashflower-0.4.2/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.1/tests/test_utils.py` & `cashflower-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

