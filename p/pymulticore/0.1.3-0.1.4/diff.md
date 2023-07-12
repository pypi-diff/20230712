# Comparing `tmp/pymulticore-0.1.3.tar.gz` & `tmp/pymulticore-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymulticore-0.1.3.tar", last modified: Wed Jul 12 01:03:37 2023, max compression
+gzip compressed data, was "pymulticore-0.1.4.tar", last modified: Wed Jul 12 03:21:43 2023, max compression
```

## Comparing `pymulticore-0.1.3.tar` & `pymulticore-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 01:03:37.186000 pymulticore-0.1.3/
--rw-rw-rw-   0        0        0     2663 2023-07-12 01:03:37.178000 pymulticore-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2418 2023-07-12 01:01:48.000000 pymulticore-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 01:03:37.110000 pymulticore-0.1.3/pymulticore/
--rw-rw-rw-   0        0        0       26 2023-07-09 15:44:29.000000 pymulticore-0.1.3/pymulticore/__init__.py
--rw-rw-rw-   0        0        0    14335 2023-07-11 16:31:20.000000 pymulticore-0.1.3/pymulticore/pymulticore.py
-drwxrwxrwx   0        0        0        0 2023-07-12 01:03:37.169000 pymulticore-0.1.3/pymulticore.egg-info/
--rw-rw-rw-   0        0        0     2663 2023-07-12 01:03:36.000000 pymulticore-0.1.3/pymulticore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-12 01:03:37.000000 pymulticore-0.1.3/pymulticore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 01:03:36.000000 pymulticore-0.1.3/pymulticore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 01:03:36.000000 pymulticore-0.1.3/pymulticore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 01:03:36.000000 pymulticore-0.1.3/pymulticore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 01:03:37.184000 pymulticore-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-07-12 01:02:31.000000 pymulticore-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 03:21:43.816000 pymulticore-0.1.4/
+-rw-rw-rw-   0        0        0     2663 2023-07-12 03:21:43.806000 pymulticore-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2418 2023-07-12 01:01:48.000000 pymulticore-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 03:21:43.724000 pymulticore-0.1.4/pymulticore/
+-rw-rw-rw-   0        0        0       26 2023-07-09 15:44:29.000000 pymulticore-0.1.4/pymulticore/__init__.py
+-rw-rw-rw-   0        0        0    14565 2023-07-12 03:19:17.000000 pymulticore-0.1.4/pymulticore/pymulticore.py
+drwxrwxrwx   0        0        0        0 2023-07-12 03:21:43.795000 pymulticore-0.1.4/pymulticore.egg-info/
+-rw-rw-rw-   0        0        0     2663 2023-07-12 03:21:43.000000 pymulticore-0.1.4/pymulticore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-12 03:21:43.000000 pymulticore-0.1.4/pymulticore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 03:21:43.000000 pymulticore-0.1.4/pymulticore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 03:21:43.000000 pymulticore-0.1.4/pymulticore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 03:21:43.000000 pymulticore-0.1.4/pymulticore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 03:21:43.814000 pymulticore-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-07-12 03:21:38.000000 pymulticore-0.1.4/setup.py
```

### Comparing `pymulticore-0.1.3/PKG-INFO` & `pymulticore-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymulticore
-Version: 0.1.3
+Version: 0.1.4
 Summary: A secure python library for parallelizing tasks across several CPU cores
 Author: Anish Kanthamneni
 Author-email: akneni@gmail.com
 Description-Content-Type: text/markdown
 
 # Parallel Processing Library
```

### Comparing `pymulticore-0.1.3/README.md` & `pymulticore-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pymulticore-0.1.3/pymulticore/pymulticore.py` & `pymulticore-0.1.4/pymulticore/pymulticore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from joblib import Parallel as _Parallel
 from joblib import delayed as _delayed
 from joblib import cpu_count as _cpu_count
 from time import perf_counter as _perf_counter
 import numpy as _np
 import ctypes as _ctypes
+import os as _os
+from pathlib import Path as _Path
+
+_current_dir = _Path(_os.path.dirname(_os.path.realpath(__file__)))
+_cudalib_path = _current_dir / "cuda-libraries" / "cudalib.dll"
+cudalib = _ctypes.cdll.LoadLibrary(str(_cudalib_path))
+
 
-cudalib = _ctypes.cdll.LoadLibrary("./cuda-libraries/cudalib.dll")
 # clib = _ctypes.cdll.LoadLibrary("./c-libraries/clib.dll")
 
 def map(func, iterable, num_cores:int=None, log_time:bool=False):
     """
     Applies a function to all items in an input iterable using multiple cores.
 
     This function is a parallelized version of the built-in map() function, 
@@ -131,15 +137,15 @@
         res = return_type([x for x, keep in res if keep])
     end_time = _perf_counter()
     if log_time:
         print(f"Time Elapsed for filter(): {end_time-start_time} seconds.")
 
     return res
 
-def get_freq(iterable, log_time=False) -> dict:
+def frequency(iterable, log_time=False) -> dict:
     """
     Computes the frequency of items in an iterable.
 
     This function iterates over the input iterable and computes the frequency of each item. 
     The frequencies are returned as a dictionary where the keys are the items and the values are the frequencies.
 
     Parameters:
@@ -302,15 +308,15 @@
         num_cores (int, optional): The number of cores to use. If None, all available cores are used.
         log_time (bool, optional): If True, the time taken to compute the standard deviation is printed.
 
     Returns:
         float: The standard deviation of the iterable.
     """
     start_time = _perf_counter()
-    res = varience(iterable, num_cores)
+    res = var(iterable, num_cores)
     res = res**0.5
 
     end_time = _perf_counter()
     if log_time:
         print(f"Time Elapsed for sum(): {end_time-start_time} seconds.")
     
     return res
@@ -359,15 +365,17 @@
     trials = []
     while len(trials) < num_trials:
         start = _perf_counter()
         func(*args)
         end = _perf_counter()
         trials.append(end-start)
     return mean(trials)
-    
+
+def num_gpu():
+    return max(cudalib.cuda_enabled(), 0)
 
 def __partition(num, num_cores):
     dif = num // num_cores
     partitions = []
     curr = 0
     for i in range (num_cores):
         if i != num_cores-1:
```

### Comparing `pymulticore-0.1.3/pymulticore.egg-info/PKG-INFO` & `pymulticore-0.1.4/pymulticore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymulticore
-Version: 0.1.3
+Version: 0.1.4
 Summary: A secure python library for parallelizing tasks across several CPU cores
 Author: Anish Kanthamneni
 Author-email: akneni@gmail.com
 Description-Content-Type: text/markdown
 
 # Parallel Processing Library
```

### Comparing `pymulticore-0.1.3/setup.py` & `pymulticore-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pymulticore',
-    version='0.1.3',
+    version='0.1.4',
     description='A secure python library for parallelizing tasks across several CPU cores',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     author='Anish Kanthamneni',
     packages=find_packages(),
     package_data={
         '': ['*.dll'],
```

