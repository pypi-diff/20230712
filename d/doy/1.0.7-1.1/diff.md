# Comparing `tmp/doy-1.0.7.tar.gz` & `tmp/doy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doy-1.0.7.tar", max compression
+gzip compressed data, was "doy-1.1.tar", max compression
```

## Comparing `doy-1.0.7.tar` & `doy-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.0.7/README.md
--rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.0.7/doy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.0.7/doy/__init__.py
--rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.0.7/doy/data.py
--rw-r--r--   0        0        0     1227 2023-06-13 16:12:21.379462 doy-1.0.7/doy/logger.py
--rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.0.7/doy/plotting.py
--rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.0.7/doy/progress.py
--rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.0.7/doy/rich_utils.py
--rw-r--r--   0        0        0     1276 2023-06-06 16:01:09.609216 doy-1.0.7/doy/utils.py
--rw-r--r--   0        0        0      344 2023-06-13 16:15:55.465364 doy-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 doy-1.0.7/setup.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 doy-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.1/README.md
+-rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.1/doy/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.1/doy/__init__.py
+-rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.1/doy/data.py
+-rw-r--r--   0        0        0     1517 2023-07-12 11:50:17.468975 doy-1.1/doy/logger.py
+-rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.1/doy/plotting.py
+-rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.1/doy/progress.py
+-rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.1/doy/rich_utils.py
+-rw-r--r--   0        0        0     2685 2023-07-12 13:40:24.055859 doy-1.1/doy/utils.py
+-rw-r--r--   0        0        0      360 2023-07-12 13:42:04.040694 doy-1.1/pyproject.toml
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 doy-1.1/setup.py
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 doy-1.1/PKG-INFO
```

### Comparing `doy-1.0.7/doy/.ipynb_checkpoints/__init__-checkpoint.py` & `doy-1.1/doy/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.7/doy/data.py` & `doy-1.1/doy/data.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.7/doy/logger.py` & `doy-1.1/doy/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 from collections import defaultdict
 from doy.utils import smooth_ema, smooth_conv
-
-# TODO: support logging keys at different timescales (e.g. train_loss, eval_loss)
-#       and then match them up again for plotting
+from typing import Optional, Union
+import os
+import wandb
+import doy
+import numpy as np
 
 
 class Logger:
-    def __init__(self, use_wandb=True):
+    def __init__(self, use_wandb: bool = True):
         self.data = defaultdict(list)
+        self.data_x = defaultdict(list)
         self.use_wandb = use_wandb
 
-    def __call__(self, step, **kwargs):
+    def __call__(self, step: int, **kwargs):
         assert kwargs
         for k, v in list(kwargs.items()):
             if v is None:
                 del kwargs[k]
                 continue
+
             try:
-                self.data[k].append(v.item())
+                v = v.item()
             except AttributeError:
-                self.data[k].append(v)
+                pass
+
+            self.data[k].append(v)
+            self.data_x[k].append(step)
+
         if self.use_wandb:
-            import wandb
             wandb.log(data=kwargs, step=step)
 
     def __getitem__(self, key):
-        return self.data[key]
+        return np.array(self.data[key])
 
-    def get(self, key, smooth_method="ema", smoothing_p=0.9):
-        if smooth_method is None:
+    def get(self, key, smooth_args: Optional[tuple] = ("ema", 0.9)):
+        if smooth_args is None:
             return self[key]
-        elif smooth_method == "ema":
-            return smooth_ema(self[key], smoothing_p)
-        elif smooth_method == "conv":
-            return smooth_conv(self[key], smoothing_p)
+
+        smoothing_method, smoothing_param = smooth_args
+        if smoothing_method == "ema":
+            return smooth_ema(self[key], smoothing_param)
+        elif smoothing_method == "conv":
+            return smooth_conv(self[key], smoothing_param)
         else:
-            raise ValueError(f"Unknown smoothing method: {smooth_method}")
+            raise ValueError(
+                f"Unknown smoothing method: {smoothing_method}, should be 'ema' or 'conv'."
+            )
+
+    def save(self, path: Union[str, os.PathLike]):
+        doy.dump({"data": self.data, "data_x": self.data_x}, path)
```

### Comparing `doy-1.0.7/doy/plotting.py` & `doy-1.1/doy/plotting.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.7/doy/progress.py` & `doy-1.1/doy/progress.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.7/doy/rich_utils.py` & `doy-1.1/doy/rich_utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.7/setup.py` & `doy-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['doy', 'doy..ipynb_checkpoints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.6.2', 'numpy', 'rich>=13.4.1', 'tqdm>=4.65.0']
+['matplotlib>=3.6.2', 'numpy', 'rich>=13.4.1', 'tqdm>=4.65.0', 'wandb>=0.15.5']
 
 setup_kwargs = {
     'name': 'doy',
-    'version': '1.0.7',
+    'version': '1.1',
     'description': '',
     'long_description': '# Doy\n\nSimple utility package\n',
     'author': 'Dominik Schmidt',
     'author_email': 'schmidtdominik30@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `doy-1.0.7/PKG-INFO` & `doy-1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: doy
-Version: 1.0.7
+Version: 1.1
 Summary: 
 Author: Dominik Schmidt
 Author-email: schmidtdominik30@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: matplotlib (>=3.6.2)
 Requires-Dist: numpy
 Requires-Dist: rich (>=13.4.1)
 Requires-Dist: tqdm (>=4.65.0)
+Requires-Dist: wandb (>=0.15.5)
 Description-Content-Type: text/markdown
 
 # Doy
 
 Simple utility package
```

