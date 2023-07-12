# Comparing `tmp/pyem_st_artifacts-1.0.1.post2.tar.gz` & `tmp/pyem_st_artifacts-1.0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyem_st_artifacts-1.0.1.post2.tar", last modified: Wed Jun  7 13:59:52 2023, max compression
+gzip compressed data, was "dist\pyem_st_artifacts-1.0.1.post3.tar", last modified: Wed Jul 12 15:47:14 2023, max compression
```

## Comparing `pyem_st_artifacts-1.0.1.post2.tar` & `pyem_st_artifacts-1.0.1.post3.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/
--rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyem_st_artifacts-1.0.1.post2/LICENSE
--rw-rw-rw-   0        0        0     9709 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/PKG-INFO
--rw-rw-rw-   0        0        0     9155 2023-06-07 12:28:29.000000 pyem_st_artifacts-1.0.1.post2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/__init__.py
--rw-rw-rw-   0        0        0    23950 2023-06-07 09:59:08.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/emotional_math.py
--rw-rw-rw-   0        0        0     3448 2023-06-07 13:09:40.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/sample.py
-drwxrwxrwx   0        0        0        0 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/__init__.py
--rw-rw-rw-   0        0        0      944 2023-06-06 14:04:47.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/lib_settings.py
--rw-rw-rw-   0        0        0      655 2023-06-06 13:59:02.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/support_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/
--rw-rw-rw-   0        0        0     9709 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/setup.cfg
--rw-rw-rw-   0        0        0     1357 2023-06-07 13:59:45.000000 pyem_st_artifacts-1.0.1.post2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/
+-rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyem_st_artifacts-1.0.1.post3/LICENSE
+-rw-rw-rw-   0        0        0     9699 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     9145 2023-07-12 15:47:03.000000 pyem_st_artifacts-1.0.1.post3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/__init__.py
+-rw-rw-rw-   0        0        0    23999 2023-07-12 15:29:15.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/emotional_math.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/
+drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/
+-rw-rw-rw-   0        0        0    73216 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/artifacts-x64.dll
+-rw-rw-rw-   0        0        0   174080 2023-06-07 09:52:32.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll
+-rw-rw-rw-   0        0        0   320512 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/filters.dll
+drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/
+-rw-rw-rw-   0        0        0    56320 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/artifacts-x86.dll
+-rw-rw-rw-   0        0        0   133632 2023-06-07 09:53:04.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll
+-rw-rw-rw-   0        0        0   268288 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/filters.dll
+-rw-rw-rw-   0        0        0     3448 2023-06-07 13:09:40.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/
+-rw-rw-rw-   0        0        0      193 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/EmotionalMathException.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-06-06 14:04:47.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/lib_settings.py
+-rw-rw-rw-   0        0        0      655 2023-06-06 13:59:02.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/support_classes.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/
+-rw-rw-rw-   0        0        0     9699 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/setup.cfg
+-rw-rw-rw-   0        0        0     1414 2023-07-12 15:43:13.000000 pyem_st_artifacts-1.0.1.post3/setup.py
```

### Comparing `pyem_st_artifacts-1.0.1.post2/LICENSE` & `pyem_st_artifacts-1.0.1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post2/PKG-INFO` & `pyem_st_artifacts-1.0.1.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyem_st_artifacts
-Version: 1.0.1.post2
+Version: 1.0.1.post3
 Summary: Python wrapper for Emotions library
 Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -182,17 +182,17 @@
 math.push_data_arr(samples)
 math.process_data_arr()
 ``` 
 2. Then check calibration status if you need to calibrate values:
 
 ##### Python
 ```python
-calibration_finished = math.emotions.calibration_finished()
+calibration_finished = math.calibration_finished()
 # and calibration progress
-calibration_progress = math.get_callibration_percents()
+calibration_progress = math.get_calibration_percents()
 ``` 
 3. If calibration finished (or you don't need to calibrate) read output values:
 
 ##### Python
 ```python
 # Reading mental levels in percent
 mental_data = math.read_mental_data_arr()
```

### Comparing `pyem_st_artifacts-1.0.1.post2/README.md` & `pyem_st_artifacts-1.0.1.post3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -166,17 +166,17 @@
 math.push_data_arr(samples)
 math.process_data_arr()
 ``` 
 2. Then check calibration status if you need to calibrate values:
 
 ##### Python
 ```python
-calibration_finished = math.emotions.calibration_finished()
+calibration_finished = math.calibration_finished()
 # and calibration progress
-calibration_progress = math.get_callibration_percents()
+calibration_progress = math.get_calibration_percents()
 ``` 
 3. If calibration finished (or you don't need to calibrate) read output values:
 
 ##### Python
 ```python
 # Reading mental levels in percent
 mental_data = math.read_mental_data_arr()
```

### Comparing `pyem_st_artifacts-1.0.1.post2/em_st_artifacts/emotional_math.py` & `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/emotional_math.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import ctypes
 import pathlib
 import platform
 import sys
 
 from typing import List
 
-from utils.EmotionalMathException import EmotionalMathException
-from utils.libsettings import (ArtifactDetectSetting, MathLibSetting, MentalAndSpectralSetting,
+from em_st_artifacts.utils.EmotionalMathException import EmotionalMathException
+from em_st_artifacts.utils.lib_settings import (ArtifactDetectSetting, MathLibSetting, MentalAndSpectralSetting,
                                ShortArtifactDetectSetting, )
-from utils.support_classes import MindData, RawChannels, RawChannelsArray, RawSpectVals, SpectralDataPercents
+from em_st_artifacts.utils.support_classes import MindData, RawChannels, RawChannelsArray, RawSpectVals, SpectralDataPercents
 
 _main_lib_name = None
 _support_lib_name = None
 _filters_lib_name = None
 if sys.platform == "win32":
     arc = platform.architecture()
     if arc[0].__contains__("64"):
@@ -26,17 +26,17 @@
 elif sys.platform.startswith("linux"):
     print('Add linux lib')
 elif sys.platform == "darwin":
     print('Add macos lib')
 else:
     raise FileNotFoundError("This platform (%s) is currently not supported by pyem-st-artifactslib." % sys.platform)
 
-_em_st_artifacts_lib = ctypes.WinDLL(str(_main_lib_name))
 ctypes.windll.LoadLibrary(str(_filters_lib_name))
 ctypes.windll.LoadLibrary(str(_support_lib_name))
+_em_st_artifacts_lib = ctypes.WinDLL(str(_main_lib_name))
 
 
 class EmotionalMath:
     class _NativeMathLibSetting(ctypes.Structure):
         _fields_ = [('sampling_rate', ctypes.c_int32), ('process_win_freq', ctypes.c_int32),
                     ('fft_window', ctypes.c_int32), ('n_first_sec_skipped', ctypes.c_int32),
                     ('bipolar_mode', ctypes.c_int32), ('channels_number', ctypes.c_int32),
```

### Comparing `pyem_st_artifacts-1.0.1.post2/em_st_artifacts/sample.py` & `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/sample.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/lib_settings.py` & `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/lib_settings.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/support_classes.py` & `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/support_classes.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/PKG-INFO` & `pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyem-st-artifacts
-Version: 1.0.1.post2
+Version: 1.0.1.post3
 Summary: Python wrapper for Emotions library
 Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -182,17 +182,17 @@
 math.push_data_arr(samples)
 math.process_data_arr()
 ``` 
 2. Then check calibration status if you need to calibrate values:
 
 ##### Python
 ```python
-calibration_finished = math.emotions.calibration_finished()
+calibration_finished = math.calibration_finished()
 # and calibration progress
-calibration_progress = math.get_callibration_percents()
+calibration_progress = math.get_calibration_percents()
 ``` 
 3. If calibration finished (or you don't need to calibrate) read output values:
 
 ##### Python
 ```python
 # Reading mental levels in percent
 mental_data = math.read_mental_data_arr()
```

### Comparing `pyem_st_artifacts-1.0.1.post2/setup.py` & `pyem_st_artifacts-1.0.1.post3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyem_st_artifacts',
-    version='1.0.1.post2',
+    version='1.0.1.post3',
     py_modules=[
         'em_st_artifacts.emotional_math',
         'em_st_artifacts.utils.lib_settings',
-        'em_st_artifacts.utils.support_classes'],
+        'em_st_artifacts.utils.support_classes',
+        'em_st_artifacts.utils.EmotionalMathException'],
     packages=['em_st_artifacts'],
     url='https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python',
     license='MIT',
     author='Brainbit Inc.',
     author_email='support@brainbit.com',
     description='Python wrapper for Emotions library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
-    package_data={"em-st-artifacts": ['libs\\x64\\artifacts-x64.dll',
+    package_data={"em_st_artifacts": ['libs\\x64\\artifacts-x64.dll',
                                'libs\\x64\\em_st_artifacts-x64.dll',
                                'libs\\x64\\filters.dll', 
                                'libs\\x86\\artifacts-x86.dll',
                                'libs\\x86\\em_st_artifacts-x86.dll',
                                'libs\\x86\\filters.dll']},
     classifiers=[
         "Programming Language :: Python :: 3",
```

