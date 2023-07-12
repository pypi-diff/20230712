# Comparing `tmp/loadingpy-0.0.2.tar.gz` & `tmp/loadingpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadingpy-0.0.2.tar", last modified: Fri Jul  7 09:10:37 2023, max compression
+gzip compressed data, was "loadingpy-0.0.3.tar", last modified: Wed Jul 12 14:17:11 2023, max compression
```

## Comparing `loadingpy-0.0.2.tar` & `loadingpy-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-07 09:10:37.584319 loadingpy-0.0.2/
--rw-r--r--   0 edouard    (501) staff       (20)     1070 2023-07-06 11:00:49.000000 loadingpy-0.0.2/LICENCE
--rw-r--r--   0 edouard    (501) staff       (20)     1938 2023-07-07 09:10:37.584155 loadingpy-0.0.2/PKG-INFO
--rw-r--r--   0 edouard    (501) staff       (20)     1666 2023-07-06 15:50:10.000000 loadingpy-0.0.2/README.md
--rw-r--r--   0 edouard    (501) staff       (20)      384 2023-07-07 09:10:03.000000 loadingpy-0.0.2/pyproject.toml
--rw-r--r--   0 edouard    (501) staff       (20)       38 2023-07-07 09:10:37.584374 loadingpy-0.0.2/setup.cfg
-drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-07 09:10:37.580751 loadingpy-0.0.2/src/
-drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-07 09:10:37.582899 loadingpy-0.0.2/src/loadingpy/
--rw-r--r--   0 edouard    (501) staff       (20)       31 2023-07-06 12:46:20.000000 loadingpy-0.0.2/src/loadingpy/__init__.py
--rw-r--r--   0 edouard    (501) staff       (20)     3329 2023-07-06 16:02:08.000000 loadingpy-0.0.2/src/loadingpy/basic_bar.py
--rw-r--r--   0 edouard    (501) staff       (20)     1500 2023-07-06 11:25:44.000000 loadingpy-0.0.2/src/loadingpy/colored_bar.py
--rw-r--r--   0 edouard    (501) staff       (20)     4306 2023-07-07 09:08:44.000000 loadingpy-0.0.2/src/loadingpy/loading_bar.py
-drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-07 09:10:37.583923 loadingpy-0.0.2/src/loadingpy.egg-info/
--rw-r--r--   0 edouard    (501) staff       (20)     1938 2023-07-07 09:10:37.000000 loadingpy-0.0.2/src/loadingpy.egg-info/PKG-INFO
--rw-r--r--   0 edouard    (501) staff       (20)      291 2023-07-07 09:10:37.000000 loadingpy-0.0.2/src/loadingpy.egg-info/SOURCES.txt
--rw-r--r--   0 edouard    (501) staff       (20)        1 2023-07-07 09:10:37.000000 loadingpy-0.0.2/src/loadingpy.egg-info/dependency_links.txt
--rw-r--r--   0 edouard    (501) staff       (20)       10 2023-07-07 09:10:37.000000 loadingpy-0.0.2/src/loadingpy.egg-info/top_level.txt
+drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-12 14:17:11.753572 loadingpy-0.0.3/
+-rw-r--r--   0 edouard    (501) staff       (20)     1070 2023-07-06 11:00:49.000000 loadingpy-0.0.3/LICENCE
+-rw-r--r--   0 edouard    (501) staff       (20)     2123 2023-07-12 14:17:11.753435 loadingpy-0.0.3/PKG-INFO
+-rw-r--r--   0 edouard    (501) staff       (20)     1851 2023-07-12 12:36:52.000000 loadingpy-0.0.3/README.md
+-rw-r--r--   0 edouard    (501) staff       (20)      384 2023-07-12 12:37:11.000000 loadingpy-0.0.3/pyproject.toml
+-rw-r--r--   0 edouard    (501) staff       (20)       38 2023-07-12 14:17:11.753616 loadingpy-0.0.3/setup.cfg
+drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-12 14:17:11.750714 loadingpy-0.0.3/src/
+drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-12 14:17:11.752446 loadingpy-0.0.3/src/loadingpy/
+-rw-r--r--   0 edouard    (501) staff       (20)       64 2023-07-12 12:36:43.000000 loadingpy-0.0.3/src/loadingpy/__init__.py
+-rw-r--r--   0 edouard    (501) staff       (20)     5770 2023-07-12 14:14:41.000000 loadingpy-0.0.3/src/loadingpy/basic_bar.py
+-rw-r--r--   0 edouard    (501) staff       (20)     1547 2023-07-12 13:44:29.000000 loadingpy-0.0.3/src/loadingpy/colored_bar.py
+-rw-r--r--   0 edouard    (501) staff       (20)     4862 2023-07-12 14:15:47.000000 loadingpy-0.0.3/src/loadingpy/loading_bar.py
+drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-12 14:17:11.753202 loadingpy-0.0.3/src/loadingpy.egg-info/
+-rw-r--r--   0 edouard    (501) staff       (20)     2123 2023-07-12 14:17:11.000000 loadingpy-0.0.3/src/loadingpy.egg-info/PKG-INFO
+-rw-r--r--   0 edouard    (501) staff       (20)      291 2023-07-12 14:17:11.000000 loadingpy-0.0.3/src/loadingpy.egg-info/SOURCES.txt
+-rw-r--r--   0 edouard    (501) staff       (20)        1 2023-07-12 14:17:11.000000 loadingpy-0.0.3/src/loadingpy.egg-info/dependency_links.txt
+-rw-r--r--   0 edouard    (501) staff       (20)       10 2023-07-12 14:17:11.000000 loadingpy-0.0.3/src/loadingpy.egg-info/top_level.txt
```

### Comparing `loadingpy-0.0.2/LICENCE` & `loadingpy-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `loadingpy-0.0.2/PKG-INFO` & `loadingpy-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadingpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: fancy progress bar
 Author-email: Edouard Yvinec <edouardyvinec@hotmail.fr>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
@@ -22,15 +22,21 @@
 accuracy = 0.0
 for inputs, labels in pybar(dataset, monitoring=[loss, accuracy], naming=["loss", "accuracy"], base_str="training"):
     # do whatever you please
     loss += 0.0 # update monitoring variables in place
     accuracy += 0.0 # update monitoring variables in place
 ```
 
-For a more detailed exampel (in torch) check this [tutorial](https://gitlab.com/ey_datakalab/loadingpy/-/blob/main/notebooks/unit_test.ipynb).
+For a more detailed exampel (in torch) check this [tutorial](https://gitlab.com/ey_datakalab/loadingpy/-/blob/main/notebooks/unit_test.ipynb). You can use a global argument in order to disable the verbatim from the loading bars as follows:
+
+```python
+from loadingpy import BarConfig
+
+BarConfig["disable loading bar"] = True
+```
 
 ## Arguments
 
 Here is a list of the arguments and their description
 | argument | description | type |
 | :---: | :---: | :---: |
 | iterable | python object that can be iterated over | can be a list, tuple, range, np.ndarray, torch.Tensor, dataset,... |
```

### Comparing `loadingpy-0.0.2/README.md` & `loadingpy-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 accuracy = 0.0
 for inputs, labels in pybar(dataset, monitoring=[loss, accuracy], naming=["loss", "accuracy"], base_str="training"):
     # do whatever you please
     loss += 0.0 # update monitoring variables in place
     accuracy += 0.0 # update monitoring variables in place
 ```
 
-For a more detailed exampel (in torch) check this [tutorial](https://gitlab.com/ey_datakalab/loadingpy/-/blob/main/notebooks/unit_test.ipynb).
+For a more detailed exampel (in torch) check this [tutorial](https://gitlab.com/ey_datakalab/loadingpy/-/blob/main/notebooks/unit_test.ipynb). You can use a global argument in order to disable the verbatim from the loading bars as follows:
+
+```python
+from loadingpy import BarConfig
+
+BarConfig["disable loading bar"] = True
+```
 
 ## Arguments
 
 Here is a list of the arguments and their description
 | argument | description | type |
 | :---: | :---: | :---: |
 | iterable | python object that can be iterated over | can be a list, tuple, range, np.ndarray, torch.Tensor, dataset,... |
```

### Comparing `loadingpy-0.0.2/src/loadingpy/colored_bar.py` & `loadingpy-0.0.3/src/loadingpy/colored_bar.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 class ColoredBar(ProgressBar):
     def __init__(
         self,
         iterable: Iterable,
         total_steps: int = -1,
         base_str: str = "loop",
+        interpolation: int = 1,
         color: str = "green",
     ) -> None:
-        super().__init__(iterable, total_steps, base_str)
+        super().__init__(iterable, total_steps, base_str, interpolation)
         self.color = color
 
     def build_prefix(self) -> str:
         base_string = f"\r[{color_map[self.color]}{self.base_str}\033[0m]"
         return base_string
 
     def build_bar(self, progression_complete: bool) -> str:
```

### Comparing `loadingpy-0.0.2/src/loadingpy/loading_bar.py` & `loadingpy-0.0.3/src/loadingpy/loading_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     def __init__(
         self,
         iterable: Iterable,
         monitoring: Optional[Any] = None,
         naming: Optional[Any] = None,
         total_steps: int = -1,
         base_str: str = "loop",
+        interpolation: int = 1,
         color: str = "green",
     ) -> None:
         """
         creates a progress bar for a python iterable.
 
         Args:
             iterable: python object that can be iterated over
@@ -23,15 +24,15 @@
                 update inplace, in order to see the changes
             naming [OPTIONAL]: if you want to add a descritpion prefix to the monitoring variables
             total_steps [OPTIONAL]: number of iterations to perform (if you set it to a lower value than the length of the iterable,
                 then the process will stop after the given total_steps)
             base_str [OPTIONAL]: prefix description of the loop we are iterating over
             color [OPTIONAL]: which color to use for the loading bar
         """
-        super().__init__(iterable, total_steps, base_str, color)
+        super().__init__(iterable, total_steps, base_str, interpolation, color)
         self.monitoring = monitoring
         self.naming = naming
         self.description = None
         if isinstance(self.monitoring, (list, tuple)) and isinstance(
             self.naming, (list, tuple)
         ):
             assert len(self.naming) == len(self.monitoring)
@@ -92,34 +93,49 @@
 
 
 if __name__ == "__main__":
     import time
 
     import torch
 
+    from .basic_bar import BarConfig
+
     a = torch.tensor(list(range(1, 15)))
     b = torch.tensor(0.0)
     for i in pybar(a, monitoring=b):
         b += i
-        time.sleep(1)
+        time.sleep(0.1)
     print("---")
+    BarConfig["disable loading bar"] = True
     b = torch.tensor(0.0)
     c = torch.tensor(1.0)
     bar = pybar(a)
     for i in bar:
         b += i
         c *= i
-        time.sleep(1)
+        time.sleep(0.1)
         bar.set_description(f"b={b}")
     print("---")
+    BarConfig["disable loading bar"] = False
     b = torch.tensor(0.0)
     c = torch.tensor(1.0)
     for i in pybar(a, monitoring=[b, c], naming=["sum", "prod"]):
         b += i
         c *= i
-        time.sleep(1)
+        time.sleep(0.1)
     print("---")
     for i in pybar(a, total_steps=5):
-        time.sleep(1)
+        time.sleep(0.1)
+    print("last value", i)
+    mybar = pybar(a, interpolation=3)
+    for i in mybar:
+        time.sleep(0.5)
+        mybar.set_description(f"eta (gt):{(14-i)*0.5 }")
+    print("last value", i)
+    a = list(range(1, 15))
+    mybar = pybar(a, interpolation=6)
+    for i in mybar:
+        time.sleep(i * 0.5)
+        mybar.set_description(f"eta (gt):{sum(range(i,14)) * 0.5}")
     print("last value", i)
 
 # python -m src.loadingpy.loading_bar
```

### Comparing `loadingpy-0.0.2/src/loadingpy.egg-info/PKG-INFO` & `loadingpy-0.0.3/src/loadingpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadingpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: fancy progress bar
 Author-email: Edouard Yvinec <edouardyvinec@hotmail.fr>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
@@ -22,15 +22,21 @@
 accuracy = 0.0
 for inputs, labels in pybar(dataset, monitoring=[loss, accuracy], naming=["loss", "accuracy"], base_str="training"):
     # do whatever you please
     loss += 0.0 # update monitoring variables in place
     accuracy += 0.0 # update monitoring variables in place
 ```
 
-For a more detailed exampel (in torch) check this [tutorial](https://gitlab.com/ey_datakalab/loadingpy/-/blob/main/notebooks/unit_test.ipynb).
+For a more detailed exampel (in torch) check this [tutorial](https://gitlab.com/ey_datakalab/loadingpy/-/blob/main/notebooks/unit_test.ipynb). You can use a global argument in order to disable the verbatim from the loading bars as follows:
+
+```python
+from loadingpy import BarConfig
+
+BarConfig["disable loading bar"] = True
+```
 
 ## Arguments
 
 Here is a list of the arguments and their description
 | argument | description | type |
 | :---: | :---: | :---: |
 | iterable | python object that can be iterated over | can be a list, tuple, range, np.ndarray, torch.Tensor, dataset,... |
```

