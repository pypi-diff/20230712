# Comparing `tmp/mbapy-0.1.3.tar.gz` & `tmp/mbapy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.1.3.tar", last modified: Fri Jun 30 13:37:37 2023, max compression
+gzip compressed data, was "mbapy-0.1.4.tar", last modified: Wed Jul 12 13:32:37 2023, max compression
```

## Comparing `mbapy-0.1.3.tar` & `mbapy-0.1.4.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.346296 mbapy-0.1.3/
--rw-rw-rw-   0        0        0     1085 2022-10-19 14:16:22.000000 mbapy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2695 2023-06-30 13:37:37.346296 mbapy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1921 2023-06-29 14:51:48.000000 mbapy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.238641 mbapy-0.1.3/mbapy/
--rw-rw-rw-   0        0        0      731 2023-06-30 04:21:54.000000 mbapy-0.1.3/mbapy/__init__.py
--rw-rw-rw-   0        0        0      402 2023-06-30 13:36:51.000000 mbapy-0.1.3/mbapy/__version__.py
--rw-rw-rw-   0        0        0     6204 2023-06-29 14:12:46.000000 mbapy-0.1.3/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.283713 mbapy-0.1.3/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      363 2023-05-25 14:57:15.000000 mbapy-0.1.3/mbapy/dl_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.286714 mbapy-0.1.3/mbapy/dl_torch/arch/
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.301011 mbapy-0.1.3/mbapy/dl_torch/arch/CL/
--rw-rw-rw-   0        0        0       34 2023-06-06 15:50:53.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CL/__init__.py
--rw-rw-rw-   0        0        0    16561 2023-06-07 03:36:12.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CL/builder.py
--rw-rw-rw-   0        0        0     2419 2023-06-07 03:14:56.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CL/trainer.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.308011 mbapy-0.1.3/mbapy/dl_torch/arch/CLIP/
--rw-rw-rw-   0        0        0       32 2023-06-06 15:37:25.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CLIP/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-06 15:35:10.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CLIP/builder.py
--rw-rw-rw-   0        0        0        0 2023-06-06 15:35:17.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CLIP/trainer.py
--rw-rw-rw-   0        0        0      203 2023-06-06 15:38:23.000000 mbapy-0.1.3/mbapy/dl_torch/arch/__init__.py
--rw-rw-rw-   0        0        0    22606 2023-06-02 01:55:22.000000 mbapy-0.1.3/mbapy/dl_torch/bb.py
--rw-rw-rw-   0        0        0     6379 2023-06-30 02:27:21.000000 mbapy-0.1.3/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     1052 2023-05-01 12:18:06.000000 mbapy-0.1.3/mbapy/dl_torch/hyper_search.py
--rw-rw-rw-   0        0        0     4113 2023-03-20 16:36:17.000000 mbapy-0.1.3/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0    13193 2023-06-02 01:55:22.000000 mbapy-0.1.3/mbapy/dl_torch/m.py
--rw-rw-rw-   0        0        0     3877 2023-06-02 01:55:22.000000 mbapy-0.1.3/mbapy/dl_torch/optim.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.312012 mbapy-0.1.3/mbapy/dl_torch/paper/
--rw-rw-rw-   0        0        0       18 2023-05-04 14:59:39.000000 mbapy-0.1.3/mbapy/dl_torch/paper/__init__.py
--rw-rw-rw-   0        0        0     2947 2023-05-25 14:57:15.000000 mbapy-0.1.3/mbapy/dl_torch/paper/bb.py
--rw-rw-rw-   0        0        0    11474 2023-06-15 14:59:22.000000 mbapy-0.1.3/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0     7865 2023-06-29 14:14:34.000000 mbapy-0.1.3/mbapy/file.py
--rw-rw-rw-   0        0        0    14949 2023-06-30 13:01:18.000000 mbapy-0.1.3/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.332018 mbapy-0.1.3/mbapy/stats/
--rw-rw-rw-   0        0        0      539 2023-04-19 11:56:16.000000 mbapy-0.1.3/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0    10820 2023-06-30 10:49:15.000000 mbapy-0.1.3/mbapy/stats/df.py
--rw-rw-rw-   0        0        0    19333 2022-12-05 10:10:18.000000 mbapy-0.1.3/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0     1281 2023-06-15 15:01:10.000000 mbapy-0.1.3/mbapy/stats/reg.py
--rw-rw-rw-   0        0        0    12704 2023-06-30 13:33:59.000000 mbapy-0.1.3/mbapy/stats/test.py
--rw-rw-rw-   0        0        0    16079 2023-06-15 15:05:25.000000 mbapy-0.1.3/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.246643 mbapy-0.1.3/mbapy.egg-info/
--rw-rw-rw-   0        0        0     2695 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1488 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      393 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      122 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 13:37:37.346296 mbapy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3190 2023-06-30 13:37:03.000000 mbapy-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.344292 mbapy-0.1.3/test/
--rw-rw-rw-   0        0        0     1087 2023-06-30 04:25:46.000000 mbapy-0.1.3/test/test_base.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.088689 mbapy-0.1.4/
+-rw-rw-rw-   0        0        0     1085 2022-10-19 14:16:22.000000 mbapy-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2747 2023-07-12 13:32:37.086689 mbapy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1921 2023-06-29 14:51:48.000000 mbapy-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.013340 mbapy-0.1.4/mbapy/
+-rw-rw-rw-   0        0        0      862 2023-07-11 16:18:10.000000 mbapy-0.1.4/mbapy/__init__.py
+-rw-rw-rw-   0        0        0      402 2023-07-12 13:12:09.000000 mbapy-0.1.4/mbapy/__version__.py
+-rw-rw-rw-   0        0        0    12020 2023-07-11 14:33:25.000000 mbapy-0.1.4/mbapy/base.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.031676 mbapy-0.1.4/mbapy/dl_torch/
+-rw-rw-rw-   0        0        0      363 2023-05-25 14:57:15.000000 mbapy-0.1.4/mbapy/dl_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.033676 mbapy-0.1.4/mbapy/dl_torch/arch/
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.048679 mbapy-0.1.4/mbapy/dl_torch/arch/CL/
+-rw-rw-rw-   0        0        0       34 2023-06-06 15:50:53.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CL/__init__.py
+-rw-rw-rw-   0        0        0    16561 2023-06-07 03:36:12.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CL/builder.py
+-rw-rw-rw-   0        0        0     2419 2023-06-07 03:14:56.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CL/trainer.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.053682 mbapy-0.1.4/mbapy/dl_torch/arch/CLIP/
+-rw-rw-rw-   0        0        0       32 2023-06-06 15:37:25.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CLIP/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:35:10.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CLIP/builder.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:35:17.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CLIP/trainer.py
+-rw-rw-rw-   0        0        0      203 2023-06-06 15:38:23.000000 mbapy-0.1.4/mbapy/dl_torch/arch/__init__.py
+-rw-rw-rw-   0        0        0    22606 2023-06-02 01:55:22.000000 mbapy-0.1.4/mbapy/dl_torch/bb.py
+-rw-rw-rw-   0        0        0     6379 2023-06-30 02:27:21.000000 mbapy-0.1.4/mbapy/dl_torch/data.py
+-rw-rw-rw-   0        0        0     1052 2023-05-01 12:18:06.000000 mbapy-0.1.4/mbapy/dl_torch/hyper_search.py
+-rw-rw-rw-   0        0        0     4113 2023-03-20 16:36:17.000000 mbapy-0.1.4/mbapy/dl_torch/loss.py
+-rw-rw-rw-   0        0        0    13193 2023-06-02 01:55:22.000000 mbapy-0.1.4/mbapy/dl_torch/m.py
+-rw-rw-rw-   0        0        0     3877 2023-06-02 01:55:22.000000 mbapy-0.1.4/mbapy/dl_torch/optim.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.055680 mbapy-0.1.4/mbapy/dl_torch/paper/
+-rw-rw-rw-   0        0        0       18 2023-05-04 14:59:39.000000 mbapy-0.1.4/mbapy/dl_torch/paper/__init__.py
+-rw-rw-rw-   0        0        0     2947 2023-05-25 14:57:15.000000 mbapy-0.1.4/mbapy/dl_torch/paper/bb.py
+-rw-rw-rw-   0        0        0    11474 2023-06-15 14:59:22.000000 mbapy-0.1.4/mbapy/dl_torch/utils.py
+-rw-rw-rw-   0        0        0    10373 2023-07-10 14:50:19.000000 mbapy-0.1.4/mbapy/file.py
+-rw-rw-rw-   0        0        0    16575 2023-07-12 13:05:45.000000 mbapy-0.1.4/mbapy/paper.py
+-rw-rw-rw-   0        0        0    14968 2023-07-10 12:49:19.000000 mbapy-0.1.4/mbapy/plot.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.060683 mbapy-0.1.4/mbapy/stats/
+-rw-rw-rw-   0        0        0      539 2023-04-19 11:56:16.000000 mbapy-0.1.4/mbapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    12351 2023-07-10 12:49:19.000000 mbapy-0.1.4/mbapy/stats/df.py
+-rw-rw-rw-   0        0        0    19333 2022-12-05 10:10:18.000000 mbapy-0.1.4/mbapy/stats/geography.py
+-rw-rw-rw-   0        0        0     1281 2023-06-15 15:01:10.000000 mbapy-0.1.4/mbapy/stats/reg.py
+-rw-rw-rw-   0        0        0    12735 2023-07-10 12:49:19.000000 mbapy-0.1.4/mbapy/stats/test.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.081686 mbapy-0.1.4/mbapy/storage/
+-rw-rw-rw-   0        0        0    86016 2023-07-06 15:23:54.000000 mbapy-0.1.4/mbapy/storage/stats.dll
+-rw-rw-rw-   0        0        0    16243 2023-07-12 13:29:22.000000 mbapy-0.1.4/mbapy/web.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.023343 mbapy-0.1.4/mbapy.egg-info/
+-rw-rw-rw-   0        0        0     2747 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      941 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      432 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 13:32:37.088689 mbapy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2485 2023-07-11 16:18:10.000000 mbapy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.084687 mbapy-0.1.4/test/
+-rw-rw-rw-   0        0        0     1998 2023-07-12 13:19:31.000000 mbapy-0.1.4/test/test_base.py
+-rw-rw-rw-   0        0        0     1740 2023-07-12 13:29:09.000000 mbapy-0.1.4/test/test_web.py
```

### Comparing `mbapy-0.1.3/LICENSE` & `mbapy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/PKG-INFO` & `mbapy-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.1.3
+Version: 0.1.4
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Keywords: mbapy,Utilities,plot
 Platform: any
@@ -13,15 +13,16 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
  * @Author: BHM-Bob 2262029386@qq.com
  * @Date: 2022-10-19 22:16:22
  * @LastEditors: BHM-Bob G 2262029386@qq.com
```

### Comparing `mbapy-0.1.3/README.md` & `mbapy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/arch/CL/builder.py` & `mbapy-0.1.4/mbapy/dl_torch/arch/CL/builder.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/arch/CL/trainer.py` & `mbapy-0.1.4/mbapy/dl_torch/arch/CL/trainer.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/bb.py` & `mbapy-0.1.4/mbapy/dl_torch/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/data.py` & `mbapy-0.1.4/mbapy/dl_torch/data.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/hyper_search.py` & `mbapy-0.1.4/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/loss.py` & `mbapy-0.1.4/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/m.py` & `mbapy-0.1.4/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/optim.py` & `mbapy-0.1.4/mbapy/dl_torch/optim.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/paper/bb.py` & `mbapy-0.1.4/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/dl_torch/utils.py` & `mbapy-0.1.4/mbapy/dl_torch/utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/plot.py` & `mbapy-0.1.4/mbapy/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 from itertools import combinations
 import sys
 from functools import wraps
-from typing import Union
+from typing import Union, List, Dict, Tuple
 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import numpy as np
 import pandas as pd
 import statsmodels.api as sm
@@ -24,24 +24,24 @@
 plt.rcParams['axes.unicode_minus'] = False #用来正常显示负号
 colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
 
 def rgb2hex(r, g, b):
   return '#'+('{:02X}' * 3).format(r, g, b)
 def hex2rgb(hex:str):
   return [int(hex[i:i+2], 16) for i in (1, 3, 5)]
-def rgbs2hexs(rgbs:list[tuple[float]]):
+def rgbs2hexs(rgbs:List[Tuple[float]]):
     """
     Takes a list of RGB tuples and converts them to a list of hexadecimal color codes. 
     Each RGB tuple must contain three floats between 0 and 1 representing the red, green, and blue 
     components of the color. Returns a list of hexadecimal color codes as strings.
     """
     return list(map(lambda x : rgb2hex(*[int(x[i]*255) for i in range(3)]),
                     rgbs))
     
-def get_palette(n:int = 10, mode:Union[None, str] = None, return_n = True) -> list[str]:
+def get_palette(n:int = 10, mode:Union[None, str] = None, return_n = True) -> List[str]:
     """get a seq of hex colors    
     Parameters
     ----------
     n: how many colors required
     mode: kind of colors
         - hls : [default] sns.color_palette('hls', n)
         - green : sum 5 grenns
@@ -67,15 +67,15 @@
 class AxisLable():
     def __init__(self, name:str, hold_space:int = 1) -> None:
         self.name = name
         self.hold_space = hold_space
     def add_space(self, space:int = 1):
         self.hold_space += space
 
-def pro_hue_pos(factors:list[str], df:pd.DataFrame, width:float, bar_space:float):
+def pro_hue_pos(factors:List[str], df:pd.DataFrame, width:float, bar_space:float):
     """
     Returns the x-axis labels and positions of the bars for a plot with multiple categorical variables.
     
     :param factors: A list of column names in the DataFrame to group by.
     :type factors: list[str]
     :param df: The input DataFrame.
     :type df: pd.DataFrame
@@ -107,15 +107,15 @@
             st_pos = 0
             for fc_idx in range(len(xlabels[axis_idx])):
                 this_hue_per = xlabels[axis_idx][fc_idx].hold_space / df.shape[0]
                 pos[axis_idx].append(st_pos+this_hue_per/2)
                 st_pos += this_hue_per
     return xlabels, pos
 
-def plot_bar(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
+def plot_bar(factors:List[str], tags:List[str], df:pd.DataFrame, **kwargs):
     """
     stack bar plot with hue style\n
     factors:[low_lever_factor, medium_lever_factor, ...] or just one
     tags:[stack_low_y, stack_medium_y, ...] or just one
     df:df from pro_bar_data or sort_df_factors
         kwargs:
     width = 0.4
@@ -168,15 +168,15 @@
             plt.setp(axs[-1].axis["bottom"].major_ticklabels, fontsize=args.font_size[idx+1])
         axs[-1].axis["top"].major_ticks.set_ticksize(0)
         # TODO : do not work
         axs[-1].axis["right"].major_ticks.set_ticksize(0)
     
     return np.array(pos[0]), ax1
 
-def plot_positional_hue(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
+def plot_positional_hue(factors:List[str], tags:List[str], df:pd.DataFrame, **kwargs):
     """
     wrapper\n
     support args: width, bar_space, xrotations, colors, offset, bottom\n
     xlabels is in margs
     @plot_positional_hue(['solution', 'type'], ['root', 'leaf'], ndf)\n
     def plot_func(ax, x, y, label, label_idx, margs, **kwargs):
         do something
@@ -212,15 +212,15 @@
                 axs[-1].axis["top"].major_ticks.set_ticksize(0)
                 # TODO : do not work
                 axs[-1].axis["right"].major_ticks.set_ticksize(0)            
             return np.array(pos[0]), ax1
         return core_wrapper
     return ret_wrapper
 
-def qqplot(tags:list[str], df:pd.DataFrame, figsize = (12, 6), nrows = 1, ncols = 1, **kwargs):
+def qqplot(tags:List[str], df:pd.DataFrame, figsize = (12, 6), nrows = 1, ncols = 1, **kwargs):
     """
     Generates a QQPlot for each specified tag in the given DataFrame using statsmodels' qqplot function.
     
     :param tags: A list of strings containing the tags to be plotted.
     :type tags: list[str]
     :param df: A pandas DataFrame containing the data to be plotted.
     :type df: pd.DataFrame
```

### Comparing `mbapy-0.1.3/mbapy/stats/__init__.py` & `mbapy-0.1.4/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/stats/df.py` & `mbapy-0.1.4/mbapy/stats/df.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-04-10 20:59:26
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-06-30 18:48:50
+LastEditTime: 2023-07-10 16:42:29
 Description: pd.dataFrame utils
 '''
 import itertools
 from functools import wraps
+from typing import List, Dict
 
 import pandas as pd
 import numpy as np
 
-from mbapy.file import update_excel
+if __name__ == '__main__':
+    # dev mode
+    from mbapy.file import update_excel
+    from mbapy.base import get_dll_path_for_sys, MyDLL
+else:
+    # release mode
+    from ..file import update_excel
+    from ..base import get_dll_path_for_sys, MyDLL
 
 def get_value(df:pd.DataFrame, column:str, mask:np.array)->list:
     return df.loc[mask, column].tolist()
 
 
 # TODO : not use itertools.product
-def pro_bar_data(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
+def pro_bar_data(factors:List[str], tags:List[str], df:pd.DataFrame, **kwargs):
     """
     cacu mean and SE for each combinations of facotors\n
     data should be like this:\n
     | factor1 | factor2 | y1 | y2 |...\n
     |  f1_1   |   f2_1  |2.1 |-2  |...\n
     after process\n
     | factor1 | factor2 | y1(mean) | y1_SE(SE) | y1_N(sum_data) |...\n
@@ -53,27 +61,27 @@
                     line.append(values.std(ddof = 1)/np.sqrt(values.shape[0]))
                 else:
                     line.append(np.NaN)
                 line.append(values.shape[0])
             ndf.append(list(factorCombi) + line)
     return pd.DataFrame(ndf[1:], columns=ndf[0])
 
-def pro_bar_data_R(factors:list[str], tags:list[str], df:pd.DataFrame, suffixs:list[str], **kwargs):
+def pro_bar_data_R(factors:List[str], tags:List[str], df:pd.DataFrame, suffixs:List[str], **kwargs):
     """
     wrapper\n
     @pro_bar_data_R(['solution', 'type'], ['root', 'leaf'], ndf)\n
     def plot_func(values, **kwargs):
         return produced vars in list format whose length equal to len(suffix)
     """
     def ret_wrapper(core_func):
         def core_wrapper(**kwargs):
             nonlocal tags
             if len(tags) == 0:
                 tags = list(df.columns)[len(factors):]
-            factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
+            factor_contents:List[List[str]] = [ df[f].unique().tolist() for f in factors ]
             ndf = [factors.copy()]
             for tag in tags:
                 for suffix in suffixs:
                     ndf[0] += [tag+suffix]
             for factorCombi in itertools.product(*factor_contents):
                 factorMask = np.array(df[factors[0]] == factorCombi[0])
                 for i in range(1, len(factors)):
@@ -86,15 +94,15 @@
                         assert len(ret_line) == len(suffixs), 'length of return value of core_func != len(suffixs)'
                         line += ret_line
                     ndf.append(list(factorCombi) + line)
             return pd.DataFrame(ndf[1:], columns=ndf[0])
         return core_wrapper
     return ret_wrapper
 
-def get_df_data(factors:dict[str, list[str]], tags:list[str], df:pd.DataFrame,
+def get_df_data(factors:Dict[str, List[str]], tags:List[str], df:pd.DataFrame,
                 include_factors:bool = True):
     """
     Return a subset of the input DataFrame, filtered by the given factors and tags.
 
     Args:
         factors (dict[str, list[str]]): A dictionary containing the factors to filter by.
             The keys are column names in the DataFrame and the values are lists of values
@@ -124,15 +132,15 @@
             # factors[factor_name] asigned with [], get all sub factors
             factors[factor_name] = df[factor_name].unique().tolist()
         for sub_factor in factors[factor_name]:
             sub_mask = update_mask(sub_mask, np.array(df[factor_name] == sub_factor), '|')
         mask = update_mask(mask, sub_mask, '&')
     return df.loc[mask, tags]
 
-def sort_df_factors(factors:list[str], tags:list[str], df:pd.DataFrame):
+def sort_df_factors(factors:List[str], tags:List[str], df:pd.DataFrame):
     """UnTested
     sort each combinations of facotors\n
     data should be like this:\n
     | factor1 | factor2 | y1 | y2 |...\n
     |  f1_1   |   f2_1  |2.1 |-2  |...\n
     |  f1_1   |   f2_2  |2.1 |-2  |...\n
     ...\n
@@ -140,15 +148,15 @@
     | factor2 | factor1 | y1 | y2 |...\n
     |  f2_1   |   f1_1  |2.1 |-2  |...\n
     |  f2_1   |   f1_2  |2.1 |-2  |...\n
     ...\n
     """
     if len(tags) == 0:
         tags = list(df.columns)[len(factors):]
-    factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
+    factor_contents:List[List[str]] = [ df[f].unique().tolist() for f in factors ]
     ndf = [factors.copy()]
     ndf[0] += tags
     for factorCombi in itertools.product(*factor_contents):
         factorMask = df[factors[0]] == factorCombi[0]
         for i in range(1, len(factors)):
             factorMask &= df[factors[i]] == factorCombi[i]
         ndf.append(list(factorCombi) + np.array(df.loc[factorMask, tags].values))
@@ -194,17 +202,18 @@
             elif mat[i][j] >= sh:
                 i += 1
     elif backend == 'torch-array':
         try:
             import torch
         except:
             raise ImportError('no torch available')
-        arr = tensor if tensor is not None else torch.tensor(ndf[tag], device = device, dtype = torch.float32).view(-1)
+        arr = tensor if tensor is not None else torch.tensor(ndf[tag], device = device,
+                                                             dtype = torch.float32).view(-1)
         @torch.jit.script
-        def step_scan(x:torch.Tensor, to_remove:list[int], sh:float):
+        def step_scan(x:torch.Tensor, to_remove:List[int], sh:float):
             i = 0
             while i < x.shape[0]-1:
                 if x[i+1] - x[i] < sh:
                     x[i+1] = x[i]
                     to_remove.append(i+1)
                 i += 1
             return to_remove
@@ -213,29 +222,42 @@
         arr = np.array(ndf[tag]).reshape([len(ndf[tag])])
         i = 0
         while i < arr.shape[0]-1:
             if arr[i+1] - arr[i] < sh:
                 arr[i+1] = arr[i]
                 to_remove_idx.append(i+1)
             i += 1
+    elif backend == 'ba-cpp':
+        raise(NotImplementedError)
+        arr = np.array(ndf[tag]).reshape([len(ndf[tag])]).tolist()
+        dll = MyDLL(get_dll_path_for_sys('stats'))
+        c_result = dll.PTR(dll.FLOAT)
+        c_size = dll.INT
+        c_remove_simi = dll.get_func('remove_simi',
+                                     [dll.PTR(dll.FLOAT), dll.PTR(dll.FLOAT), dll.PTR(dll.INT)])
+        c_remove_simi(dll.convert_c_lst(arr, dll.FLOAT), dll.REF(c_result), dll.REF(c_size))
+        to_remove_idx = dll.convert_py_lst(c_result, c_size)
+    else:
+        raise(NotImplementedError)
     ndf.drop(labels = to_remove_idx, inplace=True)
     return ndf, to_remove_idx
 
 def interp(long_one:pd.Series, short_one:pd.Series):
     """
     给定两个pd.Series,一长一短,用线性插值给短的插值,使其长度与长的pd.Series一样\n
     Given two pd.Series, one long and one short, use linear interpolation to give the short one the same length as the long pd.Series\n
     """
     assert len(long_one) > len(short_one), 'len(long_one) <= len(short_one)'
-    short_one_idx = np.array(np.arange(short_one.shape[0])*(long_one.shape[0]/short_one.shape[0]), dtype=np.int32)
+    short_one_idx = np.array(np.arange(short_one.shape[0])*(long_one.shape[0]/short_one.shape[0]),
+                             dtype=np.int32)
     if short_one_idx[-1] < long_one.shape[0]-1:
         short_one_idx[-1] = long_one.shape[0]-1
     return np.interp(np.arange(long_one.shape[0]), short_one_idx, short_one)
 
-def merge_col2row(df:pd.DataFrame, cols:list[str],
+def merge_col2row(df:pd.DataFrame, cols:List[str],
                   new_cols_name:str, value_name:str):
     """
     Given a pandas.dataFrame, it has some colums, this func will replicate these colums to row\n
     Parameters
     ----------
     df: a pd.dataFrame
     cols: colums which need be merged to rows
@@ -246,8 +268,24 @@
     new_df: a new dataFrame
     """
     # 将需要转换的列转换为行，并将结果存储在一个新的数据框中
     new_df = pd.melt(df, id_vars=df.columns.difference(cols), value_vars=cols,
                      var_name=new_cols_name, value_name=value_name)
     # 重新设置索引
     new_df = new_df.reset_index(drop=True)
-    return new_df
+    return new_df
+
+
+if __name__ == '__main__':
+    # dev code
+    import ctypes
+    dll = MyDLL(get_dll_path_for_sys('stats'))
+    c_size = dll.INT(100)
+    arr = np.random.randn(c_size.value)
+    arr.sort()
+    arr = arr.tolist()
+    c_remove_simi = dll.get_func('remove_simi',
+                                 [dll.PTR(dll.FLOAT), dll.PTR(dll.INT)],
+                                 dll.PTR(dll.FLOAT))
+    to_remove_idx = c_remove_simi(dll.convert_c_lst(arr, dll.FLOAT), dll.REF(c_size))
+    to_remove_idx = dll.convert_py_lst(to_remove_idx, c_size.value)
+    print(to_remove_idx)
```

### Comparing `mbapy-0.1.3/mbapy/stats/geography.py` & `mbapy-0.1.4/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/stats/reg.py` & `mbapy-0.1.4/mbapy/stats/reg.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.3/mbapy/stats/test.py` & `mbapy-0.1.4/mbapy/stats/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-04-04 16:45:23
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-06-30 21:28:57
+LastEditTime: 2023-07-10 16:44:48
 Description: 
 '''
 from typing import Optional, Union
 from itertools import combinations
+from typing import List, Dict
 
 import scipy
 import numpy as np
 import pandas as pd
 import statsmodels.api as sm
 from statsmodels.stats.multicomp import MultiComparison
 from statsmodels.stats.libqsturng import qsturng
 import scikit_posthocs as sp
 
 import mbapy.stats.df as msd
 
-def get_interval(mean = None, se = None, data:Optional[Union[np.ndarray, list[int], pd.Series]] = None, confidence:float = 0.95):
+def get_interval(mean = None, se = None, data:Optional[Union[np.ndarray, List[int], pd.Series]] = None, confidence:float = 0.95):
     """
     置信区间\n
     ± 1.96 * SE or other depends on confidence
     """
     assert se is not None or data is not None, 'se is None and data is None'
     kwargs = {
         'scale':se if se is not None else scipy.stats.sem(data)       
@@ -30,97 +31,97 @@
     if mean is not None:
         kwargs.update({'loc':mean})
     if data is not None:
         kwargs.update({'df':len(data) - 1, 'loc':np.mean(data).item()})
     return scipy.stats.norm.interval(confidence = confidence, loc = kwargs['loc'], scale = kwargs['scale']), kwargs
 
 def _get_x1_x2(x1 = None, x2 = None,
-               factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None):
+               factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None):
     """以同一列factors提取同一列tag的x1和x2，其余factors仅作筛选作用"""
     if factors is not None and tag is not None and df is not None:
         sub_df = msd.get_df_data(factors, [tag], df)
         fac_name = list(factors.keys())[0]
         x1 = sub_df.loc[sub_df[fac_name] == factors[fac_name][0], [tag]].values
         if len(factors[fac_name]) == 2:
             x2 = sub_df.loc[sub_df[fac_name] == factors[fac_name][1], [tag]].values
         elif len(factors[fac_name]) > 2:
             raise ValueError('Only support 1 or 2 value of factors')
     return x1, x2
 
 def _get_x1_x2_R(x1 = None, x2 = None,
-               factors:dict[str, list[str]] = None, tags:list[str] = None, df:pd.DataFrame = None):
+               factors:Dict[str, List[str]] = None, tags:List[str] = None, df:pd.DataFrame = None):
     """
     提取多列tag的x1和x2，factors仅作筛选作用
     tags为x1和x2...的tag
     """
     ret = [x1, x2]
     if factors is not None and tags is not None and df is not None:
         ret = []
         sub_df = msd.get_df_data(factors, tags, df)
         ret = [sub_df.loc[:, [tag]].values.reshape(-1) for tag in tags]
     return ret
 
 def ttest_1samp(x1 = None, x2:float = None,
-                 factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
+                 factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """单样本T检验"""
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     return scipy.stats.ttest_1samp(x1, x2, **kwargs)
 
 def ttest_ind(x1 = None, x2 = None,
-                 factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
+                 factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """
     独立样本t检验(双样本T检验):检验两组独立样本均值是否相等\n
     要求正太分布，正太检验结果由scipy.stats.levene计算并返回\n
     levene 检验P值 > 0.05，接受原假设，认为两组方差相等\n
     如不相等， scipy.stats.ttest_ind() 函数中的参数 equal_var 会设置成 False
     """
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     levene = scipy.stats.levene(x1, x2)
     return levene.pvalue, scipy.stats.ttest_ind(x1, x2, equal_var=levene.pvalue > 0.05)
 
 def ttest_rel(x1 = None, x2 = None,
-                 factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
+                 factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """配对样本T检验:比较从同一总体下分出的两组样本在不同场景下，均值是否存在差异(两个样本的样本量要相同)"""
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     return scipy.stats.ttest_rel(x1, x2, **kwargs)
 
 def mannwhitneyu(x1 = None, x2 = None,
-                 factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
+                 factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """
     Mann-Whitney U检验:数据不具有正态分布时使用。\n
     评估了两个抽样群体是否可能来自同一群体，这两个群体在数据方面是否具有相同的形状？\n
     证明这两个群体是否来自于具有不同水平的相关变量的人群。\n
     此包装函数同时支持直接输入和mbapy-style数据输入
     """
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     return scipy.stats.mannwhitneyu(x1, x2, **kwargs)
 
 def shapiro(x1 = None,
-            factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
+            factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """
     shapiro正态检验:\n
     p > 0.05 为正态分布
     """
     x1, _ = _get_x1_x2(x1, None, factors, tag, df)
     return scipy.stats.shapiro(x1, **kwargs)
 
 def pearsonr(x1 = None, x2 = None,
-             factors:dict[str, list[str]] = None, tags:list[str] = None, df:pd.DataFrame = None, **kwargs):
+             factors:Dict[str, List[str]] = None, tags:List[str] = None, df:pd.DataFrame = None, **kwargs):
     """
     pearsonr相关系数:检验两个样本是否有线性关系\n
     p > 0.05 为独立(不相关)\n
     mbapy-style数据输入:\n
     提取多列tag的x1和x2，factors仅作筛选作用
     tags为x1和x2...的tag
     """
     x1, x2 = _get_x1_x2_R(x1, x2, factors, tags, df)
     return scipy.stats.pearsonr(x1, x2, **kwargs)
 
 def _get_observe(observed = None,
-                 factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None):
+                 factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None):
     if observed is None and factors is not None and tag is not None and df is not None:
         @msd.pro_bar_data_R(list(factors.keys()), [tag], df, [''])
         def get_sum(values):
             return [values.sum()]
         ndf = get_sum()
         col = list(factors.keys())[0]
         rol = list(factors.keys())[1]
@@ -129,41 +130,41 @@
         for c in factors[col]:
             for r in factors[rol]:
                 mat[c][r] = sum(ndf.loc[(ndf[col] == c) & (ndf[rol] == r), [tag]].values)
         observed = mat
     return observed
 
 def chi2_contingency(observed = None,
-                      factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
+                      factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """
     卡方检验 Chi-Squared Test:\n
     p > 0.05 为独立(不相关)。\n
     若存在某一个格子的理论频数T<5或p值与规定的显著性水平(如0.05)相近时，改用Fisher's exact test\n
     1. 样本来自简单随机抽样
     2. 各个格子是相互独立的;
     3. 样本量应尽可能大。总观察数应不小于40，且每个格子的频数应大于等于5\n
     支持直接输入和mbapy-style数据输入\n
     mbapy-style: factors={'a':['a1', 'a2', ...], 'b':['b1', 'b2', ...]}, tag is value of 0/1 or number
     """
     observed = _get_observe(observed, factors, tag, df)
     return scipy.stats.chi2_contingency(observed, **kwargs), observed
 
 def fisher_exact(observed = None,
-                      factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
+                      factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """
     Fisher确切概率法 Fisher's exact test:\n
     2x2 contingency table, p > 0.05 为独立(不相关)\n
     支持直接输入和mbapy-style数据输入\n
     mbapy-style: factors={'a':['a1', 'a2'], 'b':['b1', 'b2']}, tag is value of 0/1 or number
     """
     observed = _get_observe(observed, factors, tag, df)
     return scipy.stats.fisher_exact(observed, **kwargs), observed
 
 def f_oneway(Xs:list = None,
-             factors:dict[str, list[str]] = None, tag:str = None, df:pd.DataFrame = None):
+             factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None):
     """
     方差分析检验(ANOVA) Analysis of Variance Test (ANOVA):p < 0.05 为显著差异\n
     检验两个或多个独立样本的均值是否有显著差异\n
     1. 每个样本中的观测值都是独立和相同分布的(iid)。
     2. 每个样本中的观测值都是正态分布。
     3. 每个样本中的观测值具有相同的方差。\n
     支持直接输入(Xs)和mbapy-style数据输入
@@ -190,15 +191,15 @@
     elif p_value < 0.01:
         return '**'
     elif p_value < 0.05:
         return '*'
     else:
         return ''
 
-def multicomp_turkeyHSD(factors:dict[str, list[str]], tag:str, df:pd.DataFrame, alpha:float = 0.05):
+def multicomp_turkeyHSD(factors:Dict[str, List[str]], tag:str, df:pd.DataFrame, alpha:float = 0.05):
     """
     using statsmodels.stats.multicomp.pairwise_tukeyhsd, Tukey's HSD 检验是一种多重比较方法，用于比较多个处理组之间的差异。\n
     Tukey的HSD法要求各样本的样本相等或者接近, 在样本量相差很大的情况下还是建议使用其他方法\n
     Tukey的HSD检验比Bonferroni法更加的保守\n
     Parameters:
     -----------
     factors: dict[str, list[str]], the first key-values is the data-choosed factor, the other are the factors to help to choose
@@ -244,28 +245,28 @@
         stars = p_value_to_stars(p_value)
         
         table_data.append([group1, group2, mean_diff, p_value, stars, is_rejected])
     
     table = pd.DataFrame(table_data, columns=['Group 1', 'Group 2', 'Mean Difference', 'p-value', 'Stars', 'Reject'])
     return table
 
-def multicomp_dunnett(factor:str, exp:list[str], control:str, df:pd.DataFrame, **kwargs):
+def multicomp_dunnett(factor:str, exp:List[str], control:str, df:pd.DataFrame, **kwargs):
     """
     using SciPy 1.11 scipy.stats.dunnett, 用于比较一个处理组与其他多个处理组之间的差异\n
     Parameters:
     -----------
     factors: str, means colum name for expiremental factor and control factor
     exp: list[str], sub factors stands for experiment group
     control: str, sub factors stands for control group
     df: pd.DataFrame
     """
     exps = [np.array(df[factor][df[factor]==e]) for e in exp]
     return scipy.stats.dunnett(*exps, np.array(df[factor][df[factor]==control]), **kwargs)
 
-def multicomp_bonferroni(factors:dict[str, list[str]], tag:str, df:pd.DataFrame, alpha:float = 0.05):
+def multicomp_bonferroni(factors:Dict[str, List[str]], tag:str, df:pd.DataFrame, alpha:float = 0.05):
     """
     using scikit_posthocs.posthoc_dunn, Dunn 检验是一种非参数的多重比较方法，用于比较多个处理组之间的差异。\n
     Bonferroni method\n
     Parameters:
     -----------
     factors: dict[str, list[str]], the first key-values is the data-choosed factor, the other are the factors to help to choose
     tag: str, data column name
```

### Comparing `mbapy-0.1.3/mbapy/web.py` & `mbapy-0.1.4/mbapy/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,16 @@
     html = browser.page_source
     if return_html_text:
         return BeautifulSoup(html, 'html.parser'), html
     return BeautifulSoup(html, 'html.parser')
 
 def get_between(string:str, head:str, tail:str,
                headRFind:bool = False, tailRFind:bool = True,
-               retHead:bool = False, retTail:bool = False):
+               ret_head:bool = False, ret_tail:bool = False,
+               find_tail_from_head = False):
     """
     Returns a substring of `string` that is between the last occurrence of `head` and the first 
     occurrence of `tail`. If `headRFind` is True, the last occurrence of `head` is used to find 
     the index of the start of the substring; otherwise, the first occurrence of `head` is used. 
     If `tailRFind` is True, the last occurrence of `tail` is used to find the index of the 
     end of the substring; otherwise, the first occurrence of `tail` is used. If `retHead` is 
     True, the returned substring includes the `head`; otherwise it starts after the `head`. 
@@ -117,21 +118,24 @@
     :type retHead: bool
     :param retTail: Whether to include the `tail` in the returned substring
     :type retTail: bool
     :return: The substring between `head` and `tail` in `string`
     :rtype: str
     """
     headIdx = string.rfind(head) if headRFind else string.find(head)
-    tailIdx = string.rfind(tail) if tailRFind else string.find(tail)
+    if find_tail_from_head:
+        tailIdx = string[headIdx+len(head):].find(tail) + headIdx + len(head)
+    else:
+        tailIdx = string.rfind(tail) if tailRFind else string.find(tail)
     if headIdx == -1 or tailIdx == -1:
         return put_err(f"{head if headIdx == -1 else tail:s} not found, return string", string)
     if headIdx == tailIdx:
-        return put_err(f"headIdx == tailIdx with head:{head:s} and string:{string:s}, return string", string)
-    idx1 = headIdx if retHead else headIdx+len(head)
-    idx2 = tailIdx+len(tail) if retTail else tailIdx
+        return put_err(f"headIdx == tailIdx with head:{head:s} and string:{string:s}, return ''", '')
+    idx1 = headIdx if ret_head else headIdx+len(head)
+    idx2 = tailIdx+len(tail) if ret_tail else tailIdx
     return string[idx1:idx2]
 def get_between_re(string:str, head:str, tail:str,
                head_r:bool = False, tail_r:bool = True,
                 ret_head:bool = False, ret_tail:bool = False):
     """
     Returns the substring between the first occurrence of `head` and the first occurrence of `tail` in `string`.
     If `head_r` is True, returns the substring between the last occurrence of `head` and the first occurrence of `tail`.
```

### Comparing `mbapy-0.1.3/mbapy.egg-info/PKG-INFO` & `mbapy-0.1.4/mbapy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.1.3
+Version: 0.1.4
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Keywords: mbapy,Utilities,plot
 Platform: any
@@ -13,15 +13,16 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
  * @Author: BHM-Bob 2262029386@qq.com
  * @Date: 2022-10-19 22:16:22
  * @LastEditors: BHM-Bob G 2262029386@qq.com
```

### Comparing `mbapy-0.1.3/setup.py` & `mbapy-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-06-30 21:37:03
+LastEditTime: 2023-07-10 16:55:48
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 """
 
@@ -32,41 +32,15 @@
     if '__author_email__' in line:
         __author_email__ = line[line.find('"')+1:-1]
     if '__author__' in line:
         __author__ = line[line.find('"')+1:-1]
     if '__url__' in line:
         __url__ = line[line.find('"')+1:-1]
 
-requires = [
-    "beautifulsoup4>=4.10.1",
-    "bokeh>=2.3.3",
-    "chardet>=5.0.0",
-    "cn2an>=0.5.17",
-    "holoviews>=1.13.1",
-    "imageio>=2.20.2",
-    "jieba>=0.42.1",
-    "Markdown>=3.4.1",
-    "matplotlib>=3.5.3",
-    "multiprocess>=0.70.13",
-    "numpy>=1.22.1",
-    "pandas>=1.4.3",
-    "pathtools>=0.1.2",
-    "pdfkit>=1.0.0",
-    "Pillow>=9.2.0",
-    "plotly>=5.10.0",
-    "requests>=2.25.1",
-    "scikit-learn>=1.1.2",
-    "scipy>=1.5.1",
-    "seaborn>=0.11.2",
-    "selenium>=4.2.0",
-    "urllib3>=1.22.12",
-    "openpyxl",
-    "statsmodels",
-    "scikit_posthocs",
-]
+requires = (here / "requirements.txt").read_text(encoding="utf-8")
 
 setup(
     name = "mbapy",
     version = __version__,
 
     classifiers=[
         "Development Status :: 4 - Beta",
@@ -74,40 +48,35 @@
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        # "Programming Language :: Python :: 3.11",# wait to numpy
+        "Programming Language :: Python :: 3.11",
         # "Programming Language :: Python :: 3 :: Only",
     ],
         
     keywords = ["mbapy", "Utilities", "plot"],
     description = "MyBA in Python",
     long_description = long_description,
     long_description_content_type='text/markdown',
-    python_requires=">=3.7, <3.11",
+    python_requires=">=3.7, <3.12",
     license = "MIT Licence",
 
     url = __url__,
     author = __author__,
     author_email = __author_email__,
     
-    # packages=["mbapy"],
-    packages=["mbapy",
-              "mbapy/stats",
-              "mbapy/dl_torch",
-              "mbapy/dl_torch/paper",
-              "mbapy/dl_torch/arch", "mbapy/dl_torch/arch/CL", "mbapy/dl_torch/arch/CLIP"],
+    packages = find_packages(exclude=["test"]),
     
     include_package_data = True,
+    package_data= {'mbapy': ['storage/stats.dll']},
     platforms = "any",
     
     install_requires=requires,
 )
 
 # pip install .
 
-
 # python setup.py sdist
-# twine upload dist/mbapy-0.1.3.tar.gz
+# twine upload dist/mbapy-0.1.4.tar.gz
```

