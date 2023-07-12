# Comparing `tmp/SpecLab-4.2.1.tar.gz` & `tmp/SpecLab-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpecLab-4.2.1.tar", last modified: Wed Jul 12 15:13:20 2023, max compression
+gzip compressed data, was "SpecLab-4.2.2.tar", last modified: Wed Jul 12 15:23:27 2023, max compression
```

## Comparing `SpecLab-4.2.1.tar` & `SpecLab-4.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5301 2023-07-12 15:13:20.229832 SpecLab-4.2.1/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5047 2023-07-12 15:04:51.000000 SpecLab-4.2.1/README.md
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/aux/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/aux/param_files/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/param_files/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param.default.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param_ARCES.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    36736 2023-07-12 15:12:23.000000 SpecLab-4.2.1/SpecLab/aux/pyqtgraph_modifications.tar.gz
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/cfg/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2183 2023-07-12 15:02:27.000000 SpecLab-4.2.1/SpecLab/cfg/SpecLab_config.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/cfg/epar_imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/doc/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1020 2023-07-12 14:58:03.000000 SpecLab-4.2.1/SpecLab/doc/CHANGELOG.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1385 2023-07-12 14:56:42.000000 SpecLab-4.2.1/SpecLab/doc/KNOWN_ISSUES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/doc/LICENSE.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5047 2023-07-12 14:59:23.000000 SpecLab-4.2.1/SpecLab/doc/README.md
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/doc/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/gen/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/gen/SpecLabFunctions.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/gen/__init__.py
--rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/gen/globals.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/gen/myfunc.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/imXam/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/imXam/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    49681 2023-07-12 14:30:50.000000 SpecLab-4.2.1/SpecLab/imXam/imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab.egg-info/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5301 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      760 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        1 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      138 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/requires.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        8 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/top_level.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)       38 2023-07-12 15:13:20.229832 SpecLab-4.2.1/setup.cfg
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1299 2023-07-12 15:04:25.000000 SpecLab-4.2.1/setup.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5301 2023-07-12 15:23:27.964980 SpecLab-4.2.2/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5047 2023-07-12 15:23:09.000000 SpecLab-4.2.2/README.md
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.960980 SpecLab-4.2.2/SpecLab/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/aux/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/aux/param_files/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/param_files/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param.default.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param_ARCES.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    36736 2023-07-12 15:12:23.000000 SpecLab-4.2.2/SpecLab/aux/pyqtgraph_modifications.tar.gz
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/cfg/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2183 2023-07-12 15:02:27.000000 SpecLab-4.2.2/SpecLab/cfg/SpecLab_config.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/cfg/epar_imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/doc/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1020 2023-07-12 15:22:43.000000 SpecLab-4.2.2/SpecLab/doc/CHANGELOG.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1385 2023-07-12 14:56:42.000000 SpecLab-4.2.2/SpecLab/doc/KNOWN_ISSUES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/doc/LICENSE.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5047 2023-07-12 15:22:57.000000 SpecLab-4.2.2/SpecLab/doc/README.md
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/doc/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/gen/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/gen/SpecLabFunctions.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/gen/__init__.py
+-rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/gen/globals.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/gen/myfunc.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/imXam/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/imXam/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    49849 2023-07-12 15:22:22.000000 SpecLab-4.2.2/SpecLab/imXam/imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab.egg-info/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5301 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      760 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        1 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      138 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/requires.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        8 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/top_level.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)       38 2023-07-12 15:23:27.964980 SpecLab-4.2.2/setup.cfg
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1299 2023-07-12 15:20:08.000000 SpecLab-4.2.2/setup.py
```

### Comparing `SpecLab-4.2.1/PKG-INFO` & `SpecLab-4.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SpecLab
-Version: 4.2.1
+Version: 4.2.2
 Summary: IRAF imexam+DS9 alternative for Python
 Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 Description-Content-Type: text/markdown
 
-# imXam:  v4.2.1 (Latest)
+# imXam:  v4.2.2 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
```

### Comparing `SpecLab-4.2.1/README.md` & `SpecLab-4.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# imXam:  v4.2.1 (Latest)
+# imXam:  v4.2.2 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
```

### Comparing `SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param.dat` & `SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param.default.dat` & `SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param.default.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param_ARCES.dat` & `SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param_ARCES.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/aux/pyqtgraph_modifications.tar.gz` & `SpecLab-4.2.2/SpecLab/aux/pyqtgraph_modifications.tar.gz`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/cfg/SpecLab_config.py` & `SpecLab-4.2.2/SpecLab/cfg/SpecLab_config.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/doc/CHANGELOG.txt` & `SpecLab-4.2.2/SpecLab/doc/CHANGELOG.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 
 - updates for python 3.6 and 3.7
 
 4.1.1 
 
 - updates to PyQtGraph, photutils module call for Python 3.8, Numpy 1.
 
-4.2.1
+4.2.2
 
 Updated everything to PyQtGraph 0.13, PyQt6, and Python 3.11.4.  All other packages were updated to latest version.
 No longer packages up the PyQtGraph into a tar, now only packages up the modified routines (ROI, GraphicsScene, ImageView).
 
 install_requires=['numpy>=1.25.0', 'plotly>=5.15.0', 'pandas>=2.0.3','astropy>=5.3.1','scipy>=1.11.1','matplotlib>=3.7.2','PyQt6==6.5.1', 'photutils>=1.8.0','pyqtgraph==0.13.3',]
```

### Comparing `SpecLab-4.2.1/SpecLab/doc/KNOWN_ISSUES.txt` & `SpecLab-4.2.2/SpecLab/doc/KNOWN_ISSUES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/doc/LICENSE.txt` & `SpecLab-4.2.2/SpecLab/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/doc/README.md` & `SpecLab-4.2.2/SpecLab/doc/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# imXam:  v4.2.1 (Latest)
+# imXam:  v4.2.2 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
```

### Comparing `SpecLab-4.2.1/SpecLab/gen/SpecLabFunctions.py` & `SpecLab-4.2.2/SpecLab/gen/SpecLabFunctions.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/gen/globals.py` & `SpecLab-4.2.2/SpecLab/gen/globals.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/gen/myfunc.py` & `SpecLab-4.2.2/SpecLab/gen/myfunc.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/SpecLab/imXam/imXam.py` & `SpecLab-4.2.2/SpecLab/imXam/imXam.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     z2_zscale = imclean[midpoint] + (coeffsz[0] / 1.0) * (npoints - midpoint)
     return z1_zscale, z2_zscale
 
 
 
 print('======================================================')
 print('======================================================')
-print('imXam: v4.2.1 (July 12, 2023)')
+print('imXam: v4.2.2 (July 12, 2023)')
 print(' To shut down gui, type q into terminal, type h for interactive commands, use middle mouse wheel to zoom in and out')
 print(' You may have to click on gui with left mouse button in order to use interactive commands')
 print(' To get a list of command-line options, type imXam.py -h from a terminal.')
 print('======================================================')
 print('imXam.py located in ',your_site_packages_location[0]+'/SpecLab/imXam/')
 print(' and .../anaconda3/envs/<your_env_name>/bin/')
 print('Default param files located in ',your_site_packages_location[0]+'/SpecLab/aux/param_files/')
@@ -912,15 +912,16 @@
                     scaleratio = 1,
                 )
 
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='y pixel')
         fig.update_xaxes(title='x pixel')
         fig.show()
-    
+        print('Trace parameters:  xstart = ', user_x, '  tsum = ',TSum, '   ntrace = ',NTrace, '   t_func =', trace_func, ' otrace = ', OTrace, '  N_iter = ', trace_iter)
+ 
 
         QtCore.QCoreApplication.processEvents()
 
     if val == 'T':  # Find and show pixels above a threshold.
         thressh =  input('Enter threshold value: ')
         thresh = float(thressh)
         t_data = np.transpose(data)
```

### Comparing `SpecLab-4.2.1/SpecLab.egg-info/PKG-INFO` & `SpecLab-4.2.2/SpecLab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SpecLab
-Version: 4.2.1
+Version: 4.2.2
 Summary: IRAF imexam+DS9 alternative for Python
 Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 Description-Content-Type: text/markdown
 
-# imXam:  v4.2.1 (Latest)
+# imXam:  v4.2.2 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
```

### Comparing `SpecLab-4.2.1/SpecLab.egg-info/SOURCES.txt` & `SpecLab-4.2.2/SpecLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.1/setup.py` & `SpecLab-4.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from pathlib import Path
 
 setup(
     name='SpecLab',
-    version='4.2.1',
+    version='4.2.2',
     author='A. F. Kowalski',
     author_email='adam.f.kowalski@colorado.edu',
     packages=['SpecLab','SpecLab.aux','SpecLab.aux.param_files','SpecLab.imXam','SpecLab.doc','SpecLab.gen',],
     package_data = {'':['*.tar.gz', '*.txt', '*.dat', '*.md', '*.rst'],},
    # include_package_data=True,
    # package_dir={"": ""},
     scripts=['SpecLab/cfg/SpecLab_config.py','SpecLab/imXam/imXam.py','SpecLab/cfg/epar_imXam.py',],
```

