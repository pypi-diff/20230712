# Comparing `tmp/pyclpu-1.1.1.tar.gz` & `tmp/pyclpu-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclpu-1.1.1.tar", last modified: Fri Jul  7 18:05:07 2023, max compression
+gzip compressed data, was "pyclpu-1.1.2.tar", last modified: Wed Jul 12 07:27:30 2023, max compression
```

## Comparing `pyclpu-1.1.1.tar` & `pyclpu-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 18:05:07.201583 pyclpu-1.1.1/
--rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.1.1/LICENSE
--rw-rw-rw-   0        0        0    10583 2023-07-07 18:05:07.201583 pyclpu-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10175 2023-07-07 18:00:36.000000 pyclpu-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 18:05:07.178987 pyclpu-1.1.1/pyclpu/
--rw-rw-rw-   0        0        0      629 2023-07-07 18:04:22.000000 pyclpu-1.1.1/pyclpu/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.1.1/pyclpu/constants.py
--rw-rw-rw-   0        0        0      981 2023-07-05 07:06:32.000000 pyclpu-1.1.1/pyclpu/formats.py
--rw-rw-rw-   0        0        0    21605 2023-07-05 10:21:29.000000 pyclpu-1.1.1/pyclpu/image.py
--rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.1.1/pyclpu/main.py
--rw-rw-rw-   0        0        0    25307 2023-07-07 17:59:55.000000 pyclpu-1.1.1/pyclpu/manager.py
--rw-rw-rw-   0        0        0    28837 2023-07-07 14:47:26.000000 pyclpu-1.1.1/pyclpu/metrology.py
--rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.1.1/pyclpu/s33293804.py
--rw-rw-rw-   0        0        0    14839 2023-07-07 12:39:09.000000 pyclpu-1.1.1/pyclpu/waveform.py
-drwxrwxrwx   0        0        0        0 2023-07-07 18:05:07.201583 pyclpu-1.1.1/pyclpu.egg-info/
--rw-rw-rw-   0        0        0    10583 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 18:05:06.000000 pyclpu-1.1.1/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-07-07 18:05:07.201583 pyclpu-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2437 2023-07-05 11:27:02.000000 pyclpu-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:27:30.782912 pyclpu-1.1.2/
+-rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     8019 2023-07-12 07:27:30.782912 pyclpu-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7611 2023-07-11 13:30:45.000000 pyclpu-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 07:27:30.773250 pyclpu-1.1.2/pyclpu/
+-rw-rw-rw-   0        0        0      629 2023-07-12 07:27:09.000000 pyclpu-1.1.2/pyclpu/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.1.2/pyclpu/constants.py
+-rw-rw-rw-   0        0        0      987 2023-07-11 12:56:55.000000 pyclpu-1.1.2/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    21605 2023-07-07 18:08:41.000000 pyclpu-1.1.2/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.1.2/pyclpu/main.py
+-rw-rw-rw-   0        0        0    25587 2023-07-07 18:16:16.000000 pyclpu-1.1.2/pyclpu/manager.py
+-rw-rw-rw-   0        0        0    28889 2023-07-12 07:19:58.000000 pyclpu-1.1.2/pyclpu/metrology.py
+-rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.1.2/pyclpu/s33293804.py
+-rw-rw-rw-   0        0        0    15876 2023-07-11 13:40:42.000000 pyclpu-1.1.2/pyclpu/waveform.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:27:30.781476 pyclpu-1.1.2/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0     8019 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-07-12 07:27:30.783969 pyclpu-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2437 2023-07-07 18:08:41.000000 pyclpu-1.1.2/setup.py
```

### Comparing `pyclpu-1.1.1/LICENSE` & `pyclpu-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.1/README.md` & `pyclpu-1.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,28 @@
+Metadata-Version: 2.1
+Name: pyclpu
+Version: 1.1.2
+Summary: CLPU Utilities
+Home-page: https://git.clpu.es/mehret/pyclpu
+Author: Michael Ehret
+Author-email: mehret@clpu.es
+License: MIT
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 **This file describes the module of CLPU utilities and related aspects to users and maintainers.**
 
 # CLPU Utilities
 
 **Abstract:** This module bundels functions which are frequently used for applications at the Centro de Laseres Pulsados, Villamayor, Spain. Although we intend to deliver reliable software solutions, we can not guarantee that every implementation is flawless. We encourage the user to re-read the code and alert us if bugs are found.
 
-:paperclip: The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format.
+:paperclip: The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format. :warning: **But relative links work only on [GitLab](https://git.clpu.es/mehret/pyclpu) / GitHub, not on [PYPI](https://pypi.org/project/pyclpu/).**
 
 ## Installation
 
 Run `pip install pyclpu` when connected to the internet; or if not connected to the internet `pip install .` within the main folder of the project (where you find also files like `README.md`, `setup.py`, `LICENCE`).
 
 ## Use-cases
 
@@ -122,20 +136,19 @@
 
 tof_detector.waveform = "path/to/data.csv"
 
 tof_detector.analyse()
 tof_detector.show()
 ```
 
-The following code sniffes in a directory `bin` for new files by means of `manager.CatchAndRename` and performs a Warp Transform by means of `image.PerspectiveTransform`. Results are stored in `bin/output_warp` if such directory exists (else in the current working directory).
+The following code sniffes in a directory `bin` for new files by means of `manager.Catch` and performs a Warp Transform by means of `image.PerspectiveTransform`. Results are stored in `bin/output_warp` if such directory exists (else in the current working directory).
 
 ```
 import os
 import numpy as np
-import time
 
 from pyclpu import manager
 from pyclpu import metrology
 
 chase = manager.Catch()
 chase.directory = "C:\\bin"
 
@@ -160,121 +173,32 @@
                     manager.strip_extension(new_file)+".spec.dat"
                 ),
                 np.array([tof_detector.Gminus1,tof_detector.dN_dGminus1]).T,
                 header='gamma-1 dN/d(gamma-1)'
             )
 ```
 
-## Scripts in Modules
-
-### Management Module
-
-#### Rename Incoming Files `CatchAndRename`
-
-This class waits for new files in a directory and renames them to `str(prefix+"_"+number+"."+extension)` according to 
-- an optional input variable `prefix` with default `""`, 
-- counting up from an optional input variable `number` that defaults to `number = 0`, 
-- and without changing the original extension.
-
-The chase for new files is activated by setting the input parameter `loop = True`. The class can be used in a functional way
-
-```
-from pyclpu import manager
-
-chase = manager.CatchAndRename(directory = "path/to/directory/", prefix = "any_string", number = 42, loop=True)
-```
-
-with 
-
-A more object oriented use case is described below. The chase for new files is activated by setting the input parameter `loop = True` and paused by setting `loop = False`.
-
-```
-from pyclpu import manager
-import time
-
-chase = manager.CatchAndRename()
-
-chase.directory = "path/to/test"
-chase.prefix = "any_string"
-chase.number = 42
-
-chase.loop = True
-
-time.sleep(100)
-
-chase.loop = False`
-
-time.sleep(100)
-
-chase.loop = True
-
-```
-
-Files that arrive in the directory during a pause will be ignored when switching on the loop again with `loop = True`.
-
-### Image Module
-
-### Interactive Point Picker `PerspectiveTransform`
-
-The class allows interactive picking of a veriable number of points in a picture. The class can be used in a functional way
-```
-from pyclpu import image
-pick = image.PointPicker(image = image.imread("path/to/test.jpg")) 
-```
-
-A more object oriented use case demonstrates how a run can be started after initialization
-```
-from pyclpu import image
-pick = image.PointPicker()
-img = image.imread("path/to/test.jpg")
-pick.image = img
-pick.n = 3
-pick.run()
-pick.status
-True
-```
-
-The output is
-- the picked points in `pick.point_list` of shape `(n,2)`,
-- the status of the execution in `pick.status`, which is True only after a successful run.
-    
-Note that the source image is not part of the object after processing.
-    
-
-#### Warp Transform `PerspectiveTransform`
-
-The class allows to transform a linearly distorted input image into a trapez-corrected view on it. The class can be used in a functional way
+The following sniplet allows to see time-of-flight results from one single waveform file and saves them to a destination.
 
 ```
-from pyclpu import image
+from pyclpu import waveform
 
-warp = image.PerspectiveTransform(source = image.imread("path/to/test.jpg")) 
-```
+wfm = waveform.wfmread("C:\\bin\\emp_2023-07-10_44_122214.Wfm.bin")
+waveform.wfmshow(wfm)
 
-with output
-- the warped image in `warp.warped` and 
-- the coordinates of cornes from the source image stored in `warp.sourcecorners`.
-
-Note that the source image is not part of the object in its final form. The coordinates of the corner points of the target rectangle can also be parsed to the function as `np.array()` of shape `(4,2)` with the keyword `sourcecorners`. A more object oriented use case can deal with loops where all warps have the same source corner coordinates
+channel = 1
+trace = waveform.Waveform(wfm = wfm, channel = channel)
 
+trace.show()
+trace.save("C:\\bin\\output.csv")
 ```
-from pyclpu import image
 
-warp_it = image.PerspectiveTransform()
-
-image_stack = image.imread("path/to/directory/with/many/images/")
-
-warp = []
-
-for image in image_stack:
-    warp_it.source = image
-    warp.append[{"warped" : warp_it.warped, "sourcecorners" : warp_it.sourcecorners}]
-```
+## Scripts in Modules
 
-with results beeing stored in a list `warp`. The dynamic modification of `warp.sourcecorners` is possible.
+:paperclip: The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format. :warning: **But relative links work only on GitLab / GitHub, not on PYPI.**
 
 ## Developper's Guide
 
 To get started, clone the project into your working directory `git clone https://srvgitlab.clpu.int/mehret/pyclpu.git` and hop inside `cd pyclpu`. Create the anaconda environment in Anaconda based on the `clpu.yml` file delivered in the main folder of the project, e.g. in the Anaconda prompt with `conda env create -f clpu.yml` and activate it with `conda activate clpu`.
 
 ### Integration and Testing
```

### Comparing `pyclpu-1.1.1/pyclpu/__init__.py` & `pyclpu-1.1.2/pyclpu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-1.1.1/pyclpu/constants.py` & `pyclpu-1.1.2/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.1/pyclpu/formats.py` & `pyclpu-1.1.2/pyclpu/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,9 @@
                 'pbm','pgm','ppm','pxm','pnm',\
                 'pfm',\
                 'sr',\
                 'tiff','tif',\
                 'exr',\
                 'hdr','pic'],
     'tifffile' : ['tiff','tif'],
-    'waveform' : ['dat','csv',"wfm"]
+    'waveform' : ['dat','csv',"wfm","bin"]
 }
```

### Comparing `pyclpu-1.1.1/pyclpu/image.py` & `pyclpu-1.1.2/pyclpu/image.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.1/pyclpu/main.py` & `pyclpu-1.1.2/pyclpu/main.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.1/pyclpu/manager.py` & `pyclpu-1.1.2/pyclpu/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,15 +409,18 @@
             del self.chase
         except:
             pass
         return None
         
 class CatchAndRename():
     """ Responsive file catcher
-    This class waits for new files in a directory and renames them upon arrival.
+    This class waits for new files in a directory and renames them upon arrival. Renaming results in `str(prefix+"_"+number+"."+extension)` according to 
+    - an optional input variable `prefix` with default `""`, 
+    - counting up from an optional input variable `number` that defaults to `number = 0`, 
+    - and without changing the original extension.
     
     Args:
         directory (str) : Path to directory where new files are expected.
         prefix (str, optional) : Prefix of renamed filename. Defaults to `""`.
         number (int, optional) : Suffix of renamed filename. Defaults to `0`.
         extension (str, optional) : Extension of renamed files. Defaults to the old extension.
         loop (bool, optional) : Activity status of the catcher. Inactive if `False`, active if `True`.
```

### Comparing `pyclpu-1.1.1/pyclpu/metrology.py` & `pyclpu-1.1.2/pyclpu/metrology.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,14 +552,15 @@
         # transform the signal amplitude in spectral counts (so far without multiplying a calibration factor)
         dT_dt = (T_m[1:]-T_m[:-1])/(tof[1:]-tof[:-1])
         dT_dt = np.append(dT_dt, [dT_dt[-1]])
         dN_dT = trace.vertical[N_Prise:N_Pfall] / ( - dT_dt)
         dN_dT_lowpass = moving_average[N_Prise:N_Pfall] / ( - dT_dt)
         # publication
         self.tof = tof
+        self.amp = trace.vertical[N_Prise:N_Pfall]
         self.Gminus1 = T_m
         self.dN_dGminus1 = dN_dT
         self.dN_dGminus1_lowpass = dN_dT_lowpass
         # integrity of results
         if isinstance(dN_dT,np.ndarray):
             self.status = True
         else:
```

### Comparing `pyclpu-1.1.1/pyclpu/s33293804.py` & `pyclpu-1.1.2/pyclpu/s33293804.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.1/pyclpu/waveform.py` & `pyclpu-1.1.2/pyclpu/waveform.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,18 +139,28 @@
     The function tries to read a waveform file to a numpy array as `[channel,amplitude,timebase]`.
  
     Args:
         path (str) : The path to a waveform file.
     
     Returns:
         wfm (:obj: `numpy.array`) : Matrix of values as ``[channel,amplitude,timebase]``
+        
+    Examples:
+        ```python
+        from pyclpu import waveform
+        wfm = waveform.wfmread("")
+        ```
+        returns
+        ```
+        None
+        ```
     """
     # METHODS
     def loader(from_file):
-        if give_extension(from_file) == ".bin":
+        if give_extension(from_file) == "bin":
             try:
                 from RSRTxReadBin import RTxReadBin
             except:
                 path_to_module = os.path.join(*give_dirlst(root)[:-1],"lib","RTxReadBin-1.0-py3-none-any.whl")
                 error(wfmread.__name__,"RTxReadBin not installed. Run pip install "+path_to_module,1169)
                 return None
             # load all
@@ -237,19 +247,27 @@
         ```
         returns
         ```
         False
         ```
     """
     name = kwargs.get('name', "ANONYMOUS")
+    nolabel = kwargs.get('nolabel', False)
     # Routine
     #try:
+    if np.ndim(wfm["vertical"]) == 1:
+        wfm["vertical"] = [wfm["vertical"]]
     for ai,active_channel in enumerate(wfm["vertical"]):
-        plt.plot(wfm["horizontal"],active_channel,label=str(ai))
-    plt.legend()
+        if nolabel:
+            label = ""
+        else:
+            label = str(ai+1)
+        plt.plot(wfm["horizontal"],active_channel,label=label)
+    if not nolabel:
+        plt.legend()
     plt.show()
     plt.close('all')
     return True
     #except:
     #    error(wfmshow.__name__,"",13)
     #    return False
  
@@ -264,21 +282,30 @@
     
     Returns:
         exit_stat (bool) : True in case of a completed run and False else.
     """
     try:
         # data
         output = [wfm["horizontal"]]
-        for active_channel in enumerate(wfm["vertical"]):
+        if np.ndim(wfm["vertical"]) == 1:
+            wfm["vertical"] = [wfm["vertical"]]
+        header = "Time/[s],"
+        i = 1
+        for active_channel in wfm["vertical"]:
             output.append(active_channel)
-        np.savetxt(full_name, np.array(output).T, delimiter=",")
+            header = header + "CH" + str(i) + "/[V],"
+            i = i + 1
+        header = header[:-1]
+        np.savetxt(full_name, np.array(output).T, delimiter=",",header=header)
         # visual feedback
-        for active_channel in enumerate(wfm["vertical"]):
+        for active_channel in wfm["vertical"]:
             plt.plot(wfm["horizontal"],active_channel)
-        plt.savefig(full_name+".png")
+        plt.xlabel("time / [s]")
+        plt.ylabel("signal / [V]")
+        plt.savefig(full_name+".png", dpi = 600)
         plt.close('all')
         return True
     except:
         error(wfmwrite.__name__,"",13)
         return False
         
 # WAVEFORM MANIPULATION
@@ -383,14 +410,20 @@
         # fourier transform etc.
         
         # integrity of results
         self.status = True
         # housekeeping
         del self.wfm
         return None
+    def show(self):
+        wfmshow({"horizontal" : self.horizontal, "vertical" : self.vertical, "nolabel" : True })
+        return None
+    def save(self,path):
+        wfmwrite(path,{"horizontal" : self.horizontal, "vertical" : self.vertical, "nolabel" : True })
+        return None
 
 
 # =============================================================================
 # PYTHON MAIN
 # =============================================================================
 # SELF AND TEST
 if globals()["__name__"] == '__main__':
```

### Comparing `pyclpu-1.1.1/setup.py` & `pyclpu-1.1.2/setup.py`

 * *Files identical despite different names*

