# Comparing `tmp/SpecLab-4.2.0.tar.gz` & `tmp/SpecLab-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpecLab-4.2.0.tar", last modified: Tue Jul 11 15:56:28 2023, max compression
+gzip compressed data, was "SpecLab-4.2.1.tar", last modified: Wed Jul 12 15:13:20 2023, max compression
```

## Comparing `SpecLab-4.2.0.tar` & `SpecLab-4.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5081 2023-07-11 15:56:28.575577 SpecLab-4.2.0/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4827 2023-07-11 15:47:12.000000 SpecLab-4.2.0/README.md
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/aux/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/aux/param_files/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/param_files/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param.default.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param_ARCES.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    36728 2023-07-11 15:31:38.000000 SpecLab-4.2.0/SpecLab/aux/pyqtgraph_modifications.tar.gz
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/cfg/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2166 2023-07-11 15:37:55.000000 SpecLab-4.2.0/SpecLab/cfg/SpecLab_config.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/cfg/epar_imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/doc/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      689 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/CHANGELOG.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1073 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/KNOWN_ISSUES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/LICENSE.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4827 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/README.md
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/gen/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/gen/SpecLabFunctions.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/gen/__init__.py
--rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/gen/globals.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/gen/myfunc.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/imXam/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/imXam/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    49771 2023-07-11 15:40:44.000000 SpecLab-4.2.0/SpecLab/imXam/imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab.egg-info/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5081 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      760 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        1 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      138 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/requires.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        8 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/top_level.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)       38 2023-07-11 15:56:28.575577 SpecLab-4.2.0/setup.cfg
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1476 2023-07-11 15:56:25.000000 SpecLab-4.2.0/setup.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5301 2023-07-12 15:13:20.229832 SpecLab-4.2.1/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5047 2023-07-12 15:04:51.000000 SpecLab-4.2.1/README.md
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/aux/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/aux/param_files/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/param_files/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param.default.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param_ARCES.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    36736 2023-07-12 15:12:23.000000 SpecLab-4.2.1/SpecLab/aux/pyqtgraph_modifications.tar.gz
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/cfg/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2183 2023-07-12 15:02:27.000000 SpecLab-4.2.1/SpecLab/cfg/SpecLab_config.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/cfg/epar_imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/doc/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1020 2023-07-12 14:58:03.000000 SpecLab-4.2.1/SpecLab/doc/CHANGELOG.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1385 2023-07-12 14:56:42.000000 SpecLab-4.2.1/SpecLab/doc/KNOWN_ISSUES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/doc/LICENSE.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5047 2023-07-12 14:59:23.000000 SpecLab-4.2.1/SpecLab/doc/README.md
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/doc/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/gen/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/gen/SpecLabFunctions.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/gen/__init__.py
+-rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/gen/globals.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/gen/myfunc.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab/imXam/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.1/SpecLab/imXam/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    49681 2023-07-12 14:30:50.000000 SpecLab-4.2.1/SpecLab/imXam/imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:13:20.229832 SpecLab-4.2.1/SpecLab.egg-info/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5301 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      760 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        1 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      138 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/requires.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        8 2023-07-12 15:13:20.000000 SpecLab-4.2.1/SpecLab.egg-info/top_level.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)       38 2023-07-12 15:13:20.229832 SpecLab-4.2.1/setup.cfg
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1299 2023-07-12 15:04:25.000000 SpecLab-4.2.1/setup.py
```

### Comparing `SpecLab-4.2.0/PKG-INFO` & `SpecLab-4.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: SpecLab
-Version: 4.2.0
-Summary: IRAF imexam+DS9 replacement for Python
+Version: 4.2.1
+Summary: IRAF imexam+DS9 alternative for Python
 Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 Description-Content-Type: text/markdown
 
-# imXam:  v4.1.2 (Latest)
+# imXam:  v4.2.1 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
-This uses [PyQTGraph](https://www.pyqtgraph.org/), but a customized version of v10 will be installed automatically with the commands below
+This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
+A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
+to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (June 28, 2023)
+author: Adam F Kowalski (July 12, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
-From terminal (if you have a conda environment already; if not, go to Step 2):
+From terminal (if you want to install to your current conda environment; if not, go to Step 2):
 
 `pip install SpecLab`
 
 
 ### Step 2
 
-Create a conda environment to install into.  If you already have a conda environment set up, and you have
+Create a conda environment to install into.  If you already have
 run `pip install SpecLab` in that environment, then skip to Step 3 below.
 
 To set up a fresh conda environment:
 
 From a terminal window:
 
-`conda create --name your_env_name python=3.8`
-
-(Note, imXam will work with Python 3.6, 3.7, and 3.8.  Note that Python 3.7 was unfortunately deprecated on 6/27/23!)
-imXam will be fully updated to work with Python 3.9+ and PyQtGraph(v.latest) by the time Python 3.8 is deprecated.
+`conda create --name your_env_name python=3.11`
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
 
 ### Step 3
 
-After pip install, run the command (from anywhere), which will untar v10 (with my modifications) of PyQtGraph to your site-packages:
+After pip install, run the command (from anywhere), which will untar the modifications to PyQtGraph to your site-packages:
 
 `SpecLab_config.py`
 
 You may have to open a fresh tab in your terminal for your system to see the new routines in .../your_env_name/bin/.  You can also:
 
 `cd /location_of_your_anaconda/anaconda3/envs/your_env_name/bin/`
 
@@ -145,8 +144,22 @@
 
 Will have to remove pyqtgraph10_speclab/ from your environment site-packages by hand.
 
 # Acknowledgments
 
 Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.
 Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  
+Thanks to Gordon MacDonald for helpful suggestions.
+
+# Troubleshooting
+On a Linux, one may have to try these commands if one gets an error during `pip install Speclab`:
+
+`sudo apt install libxcb-cursor0`
+
+or
+
+`sudo apt install --reinstall libxcb-cursor0`
+
+or
+
+`sudo apt-get install --reinstall libxcb-xinerama0`
```

### Comparing `SpecLab-4.2.0/README.md` & `SpecLab-4.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-# imXam:  v4.1.2 (Latest)
+# imXam:  v4.2.1 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
-This uses [PyQTGraph](https://www.pyqtgraph.org/), but a customized version of v10 will be installed automatically with the commands below
+This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
+A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
+to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (June 28, 2023)
+author: Adam F Kowalski (July 12, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
-From terminal (if you have a conda environment already; if not, go to Step 2):
+From terminal (if you want to install to your current conda environment; if not, go to Step 2):
 
 `pip install SpecLab`
 
 
 ### Step 2
 
-Create a conda environment to install into.  If you already have a conda environment set up, and you have
+Create a conda environment to install into.  If you already have
 run `pip install SpecLab` in that environment, then skip to Step 3 below.
 
 To set up a fresh conda environment:
 
 From a terminal window:
 
-`conda create --name your_env_name python=3.8`
-
-(Note, imXam will work with Python 3.6, 3.7, and 3.8.  Note that Python 3.7 was unfortunately deprecated on 6/27/23!)
-imXam will be fully updated to work with Python 3.9+ and PyQtGraph(v.latest) by the time Python 3.8 is deprecated.
+`conda create --name your_env_name python=3.11`
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
 
 ### Step 3
 
-After pip install, run the command (from anywhere), which will untar v10 (with my modifications) of PyQtGraph to your site-packages:
+After pip install, run the command (from anywhere), which will untar the modifications to PyQtGraph to your site-packages:
 
 `SpecLab_config.py`
 
 You may have to open a fresh tab in your terminal for your system to see the new routines in .../your_env_name/bin/.  You can also:
 
 `cd /location_of_your_anaconda/anaconda3/envs/your_env_name/bin/`
 
@@ -136,8 +135,22 @@
 
 Will have to remove pyqtgraph10_speclab/ from your environment site-packages by hand.
 
 # Acknowledgments
 
 Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.
 Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  
+Thanks to Gordon MacDonald for helpful suggestions.
+
+# Troubleshooting
+On a Linux, one may have to try these commands if one gets an error during `pip install Speclab`:
+
+`sudo apt install libxcb-cursor0`
+
+or
+
+`sudo apt install --reinstall libxcb-cursor0`
+
+or
+
+`sudo apt-get install --reinstall libxcb-xinerama0`
```

### Comparing `SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param.dat` & `SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param.default.dat` & `SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param.default.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param_ARCES.dat` & `SpecLab-4.2.1/SpecLab/aux/param_files/imXam_param_ARCES.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.0/SpecLab/cfg/SpecLab_config.py` & `SpecLab-4.2.1/SpecLab/cfg/SpecLab_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,34 +18,32 @@
  
     tarfgz = tarfile.open(tar_fname)
     tarfgz.extractall(your_site_packages_location[0]+'/')
     tarfgz.close()
     #else:
     #    print('Could not unpack pyqtgraph modifications.')
 
-
-    print('PyQtGraph is in ', your_site_packages_location[0]+'/pyqtgraph/')
-    print('Several routines were overwritten with imXam modifications:  ')
-    print('pyqtgraph/imageview/ImageView.py')
-    print('pyqtgraph/GraphicsScene/GraphicsScene.py')
-    print('pyqtgraph/graphicsItems/ROI.py')
-    print(' ********* ')
-    print('  ')
+    print('    ')
+    print('    PyQtGraph is in ', your_site_packages_location[0]+'/pyqtgraph/')
+    print('    Several routines were overwritten with imXam modifications:  ')
+    print('      pyqtgraph/imageview/ImageView.py')
+    print('      pyqtgraph/GraphicsScene/GraphicsScene.py')
+    print('      pyqtgraph/graphicsItems/ROI.py')
     print('  ')
-    print('Installation and configuration complete! ')
+    print('    SUCCESS. Installation and configuration complete! ')
     print('  ')
-    print('Basic use (from anywhere on disk) in Unix command line: imXam.py -f <file.fits>')
+    print('    Basic use (from anywhere on disk) in Unix command line: imXam.py -f <file.fits>')
     print('  ')
-    print('Notes:  Can put alias in .bash_profile:  alias imXam=<single quotes>imXam.py -f<single quotes>')
+    print('   ')
+    print('    Notes:  Can put alias in .bash_profile:  alias imXam=<single quotes>imXam.py -f<single quotes>')
     print('If the command python imXam.py is not recognized (it should be in your anaconda3 environment bin/), the source is located here:  ', your_site_packages_location[0]+'/SpecLab/imXam/')
-    print(' in which case, just put an alias to the command <single quotes>python .../site-packages/SpecLab/imXam/imXam.py -f<single quotes> in .bash_profile (or create a softlink through ln -s to a bin/ folder')
+    print('    in which case, just put an alias to the command <single quotes>python .../site-packages/SpecLab/imXam/imXam.py -f<single quotes> in .bash_profile (or create a softlink through ln -s to a bin/ folder')
     print('  ')
     print('  ')
     print('To uninstall:  pip uninstall SpecLab')
     print('  ')
-    print(' *********  ')
     
 
 except:
     print('Unable to complete configuration of PyQtGraph routines for imXam.')
```

### Comparing `SpecLab-4.2.0/SpecLab/doc/KNOWN_ISSUES.txt` & `SpecLab-4.2.1/SpecLab/doc/KNOWN_ISSUES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 Plotly opens a new tab in a browser each time it is used.  I am not sure how to fix this as searching for solutions for a while did not bring up any browser settings that could be modified.
 
-Some PyQTGraph default commands (right click selections) do not work.  I have not removed these from the PyQTGraph source.
-
 Have not tested this in Jupyter Notebooks.  I don't think it will work yet in Jupyter Notebooks but you can try.
 
 The spectral trace success relies on a decent to good Gaussian fit in spatial direction at every ~20-50 columns, so this could fail entirely on spectra that are very out of focus and show double peaks.  I plan to fix this and make it more flexible in a future update.
 
 When running epar_imXam.py, "Greys" is the only option for color map at the moment.  Will be changed in the future.
 
 Note 1: the first time you use imXam, it will take longer than normal to start b/c it's creating
 all those pycache/ folders.
 
 Note 2: imXam requires vim, which is already installed on most systems that use UNIX (make sure that your
 system has vim, not vi).
 
+Note 3: For Linux, one may have to do the following:  
+sudo apt install libxcb-cursor0 
+or 
+sudo apt install --reinstall libxcb-cursor0 
+or
+sudo apt-get install --reinstall libxcb-xinerama0
+
+Note 4: The default version of PyQtGraph encounters a problem with Python 3.11:
+https://github.com/python/cpython/issues/105497
+This fix won't get pushed until August 2023.  In the meantime, I've made the necessary
+fixes to ROI.py in PyQtGraph.
```

### Comparing `SpecLab-4.2.0/SpecLab/doc/LICENSE.txt` & `SpecLab-4.2.1/SpecLab/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.0/SpecLab/doc/README.md` & `SpecLab-4.2.1/SpecLab/doc/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-# imXam:  v4.1.2 (Latest)
+# imXam:  v4.2.1 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
-This uses [PyQTGraph](https://www.pyqtgraph.org/), but a customized version of v10 will be installed automatically with the commands below
+This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
+A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
+to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (June 28, 2023)
+author: Adam F Kowalski (July 12, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
-From terminal (if you have a conda environment already; if not, go to Step 2):
+From terminal (if you want to install to your current conda environment; if not, go to Step 2):
 
 `pip install SpecLab`
 
 
 ### Step 2
 
-Create a conda environment to install into.  If you already have a conda environment set up, and you have
+Create a conda environment to install into.  If you already have
 run `pip install SpecLab` in that environment, then skip to Step 3 below.
 
 To set up a fresh conda environment:
 
 From a terminal window:
 
-`conda create --name your_env_name python=3.8`
-
-(Note, imXam will work with Python 3.6, 3.7, and 3.8.  Note that Python 3.7 was unfortunately deprecated on 6/27/23!)
-imXam will be fully updated to work with Python 3.9+ and PyQtGraph(v.latest) by the time Python 3.8 is deprecated.
+`conda create --name your_env_name python=3.11`
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
 
 ### Step 3
 
-After pip install, run the command (from anywhere), which will untar v10 (with my modifications) of PyQtGraph to your site-packages:
+After pip install, run the command (from anywhere), which will untar the modifications to PyQtGraph to your site-packages:
 
 `SpecLab_config.py`
 
 You may have to open a fresh tab in your terminal for your system to see the new routines in .../your_env_name/bin/.  You can also:
 
 `cd /location_of_your_anaconda/anaconda3/envs/your_env_name/bin/`
 
@@ -136,8 +135,22 @@
 
 Will have to remove pyqtgraph10_speclab/ from your environment site-packages by hand.
 
 # Acknowledgments
 
 Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.
 Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  
+Thanks to Gordon MacDonald for helpful suggestions.
+
+# Troubleshooting
+On a Linux, one may have to try these commands if one gets an error during `pip install Speclab`:
+
+`sudo apt install libxcb-cursor0`
+
+or
+
+`sudo apt install --reinstall libxcb-cursor0`
+
+or
+
+`sudo apt-get install --reinstall libxcb-xinerama0`
```

### Comparing `SpecLab-4.2.0/SpecLab/gen/SpecLabFunctions.py` & `SpecLab-4.2.1/SpecLab/gen/SpecLabFunctions.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.0/SpecLab/gen/globals.py` & `SpecLab-4.2.1/SpecLab/gen/globals.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.0/SpecLab/gen/myfunc.py` & `SpecLab-4.2.1/SpecLab/gen/myfunc.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.0/SpecLab/imXam/imXam.py` & `SpecLab-4.2.1/SpecLab/imXam/imXam.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     z2_zscale = imclean[midpoint] + (coeffsz[0] / 1.0) * (npoints - midpoint)
     return z1_zscale, z2_zscale
 
 
 
 print('======================================================')
 print('======================================================')
-print('imXam: v4.2.0 (July 11, 2023)')
+print('imXam: v4.2.1 (July 12, 2023)')
 print(' To shut down gui, type q into terminal, type h for interactive commands, use middle mouse wheel to zoom in and out')
 print(' You may have to click on gui with left mouse button in order to use interactive commands')
 print(' To get a list of command-line options, type imXam.py -h from a terminal.')
 print('======================================================')
 print('imXam.py located in ',your_site_packages_location[0]+'/SpecLab/imXam/')
 print(' and .../anaconda3/envs/<your_env_name>/bin/')
 print('Default param files located in ',your_site_packages_location[0]+'/SpecLab/aux/param_files/')
@@ -117,16 +117,16 @@
 parser.add_argument("-repl", "--replace", dest="replace", help="Replace NaN, -Inf, and Inf values of array with value specified after -repl.  Must be > -999 or doesn't replace.", default=-9999.)
 parser.add_argument("-irisras", "--iris_lvl2", dest="lvl2", help='IRIS Level 2 spec raster;  the integer after -irasras will be the image to plot starting from 0')
 parser.add_argument("-cube", "--datacube", dest="cube", help='data dube FITS file with time (or another quantity such as wavelength) along one of the dimensions;  time (or wavelength) dimension is the one that is the 0th dimension [nt, ny, nx] if reading in with astropy.io.fits.getdata;  the integer after -cube will be the extension starting from 0 to plot')
 parser.add_argument("-scube", "--sdatacube", dest="scube", help='3rd axis image to subtract of data cube; default is last index',default=-1)
 parser.add_argument("-tlim1", "--tlim1", dest="tlim1", help='starting index of cube to plot ',default=0)
 parser.add_argument("-tlim2", "--tlim2", dest="tlim2", help='ending index of cube to plot',default=-1)
 parser.add_argument("-hsg", "--hsg", dest="hsg",help='if any integer, then reads in cal.xxx.fits FITS file with first extension a [nrast, ny, nx] data cube from Adams HSG reduction pipeline. Does fits.getdata(file,1).  There are many other extensions in cal.xxx.fits so this is why there is a separate -hsg trigger;  NOTE:  -cube should be used for .other fits files with datacubes read in through fits.getdata(file).')
-parser.add_argument("-i", "--param_file", dest="param",help='You can use a custom parameter file by specifying its FULL path; default is the one in anaconda3/envs/main/lib/python3.6/site-packages/SpecLab/aux/param_files/ (default:  imXam_param.dat)',default='imXam_param.dat')
-parser.add_argument("-ec", "--", dest="echelle",help='(0 or 1) if 1, loads in default imXam_param_ARCES.dat with some reasonable parameters for inspecting echelle, is the one in anaconda3/envs/main/lib/python3.6/site-packages/SpecLab/aux/param_files/ (default: 0)',default=0)
+parser.add_argument("-i", "--param_file", dest="param",help='You can use a custom parameter file by specifying its FULL path; default is the one in .../site-packages/SpecLab/aux/param_files/ (default:  imXam_param.dat)',default='imXam_param.dat')
+parser.add_argument("-ec", "--", dest="echelle",help='(0 or 1) if 1, loads in default imXam_param_ARCES.dat with some reasonable parameters for inspecting echelle, is the one in .../site-packages/SpecLab/aux/param_files/ (default: 0)',default=0)
 
         
 
 from matplotlib.colors import LinearSegmentedColormap
 # paul tol color blind safe colors:https://personal.sron.nl/~pault/
 from matplotlib import cm # this can be interpolated!
 clrs = [  '#C3A8D1', '#B58FC2','#A778B4',\
@@ -307,15 +307,15 @@
 
 print('   ')
 print('File [ny , nx] = ',ifile,'[',nyy,',',nxx,']','   Max = ',np.max(data),'   Median = ',np.median(data))
 print('   ')
 
 roi = pg.LineSegmentROI([[int(nxx*0.03), int(nyy*0.5)], [int(nxx*0.97),int(nyy*0.5)]], pen=rcol)#,handlePen=(220,5,12),hoverPen=(0,0,0),handleHoverPen=(0,0,0))  # x = 0, y = 0 is at the top, left
 roi_v = pg.LineSegmentROI([[int(nxx*0.5), int(nyy*0.15)], [int(nxx*0.5),int(nyy*0.85)]], pen=rcol)#,handlePen=(220,5,12),hoverPen=(0,0,0),handleHoverPen=(0,0,0))  # x = 0, y = 0 is at the top, left
-# colors of hovering, endpoints, etc. are controlled in ROI.py in /anaconda3/envs/hst/lib/python3.6/site-packages/pyqtgraph/graphicsItems/ but many arguments were added recently so I don't need to e. 
+# colors of hovering, endpoints, etc. are controlled in ROI.py in .../site-packages/pyqtgraph/graphicsItems/ but many arguments were added recently so I don't need to e. 
 
 imv1.addItem(roi)
 imv1.addItem(roi_v)
 
 penax = pg.mkPen(color=(0,0,0))
```

### Comparing `SpecLab-4.2.0/SpecLab.egg-info/PKG-INFO` & `SpecLab-4.2.1/SpecLab.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: SpecLab
-Version: 4.2.0
-Summary: IRAF imexam+DS9 replacement for Python
+Version: 4.2.1
+Summary: IRAF imexam+DS9 alternative for Python
 Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 Description-Content-Type: text/markdown
 
-# imXam:  v4.1.2 (Latest)
+# imXam:  v4.2.1 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
-This uses [PyQTGraph](https://www.pyqtgraph.org/), but a customized version of v10 will be installed automatically with the commands below
+This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
+A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
+to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (June 28, 2023)
+author: Adam F Kowalski (July 12, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
-From terminal (if you have a conda environment already; if not, go to Step 2):
+From terminal (if you want to install to your current conda environment; if not, go to Step 2):
 
 `pip install SpecLab`
 
 
 ### Step 2
 
-Create a conda environment to install into.  If you already have a conda environment set up, and you have
+Create a conda environment to install into.  If you already have
 run `pip install SpecLab` in that environment, then skip to Step 3 below.
 
 To set up a fresh conda environment:
 
 From a terminal window:
 
-`conda create --name your_env_name python=3.8`
-
-(Note, imXam will work with Python 3.6, 3.7, and 3.8.  Note that Python 3.7 was unfortunately deprecated on 6/27/23!)
-imXam will be fully updated to work with Python 3.9+ and PyQtGraph(v.latest) by the time Python 3.8 is deprecated.
+`conda create --name your_env_name python=3.11`
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
 
 ### Step 3
 
-After pip install, run the command (from anywhere), which will untar v10 (with my modifications) of PyQtGraph to your site-packages:
+After pip install, run the command (from anywhere), which will untar the modifications to PyQtGraph to your site-packages:
 
 `SpecLab_config.py`
 
 You may have to open a fresh tab in your terminal for your system to see the new routines in .../your_env_name/bin/.  You can also:
 
 `cd /location_of_your_anaconda/anaconda3/envs/your_env_name/bin/`
 
@@ -145,8 +144,22 @@
 
 Will have to remove pyqtgraph10_speclab/ from your environment site-packages by hand.
 
 # Acknowledgments
 
 Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.
 Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  
+Thanks to Gordon MacDonald for helpful suggestions.
+
+# Troubleshooting
+On a Linux, one may have to try these commands if one gets an error during `pip install Speclab`:
+
+`sudo apt install libxcb-cursor0`
+
+or
+
+`sudo apt install --reinstall libxcb-cursor0`
+
+or
+
+`sudo apt-get install --reinstall libxcb-xinerama0`
```

### Comparing `SpecLab-4.2.0/SpecLab.egg-info/SOURCES.txt` & `SpecLab-4.2.1/SpecLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.0/setup.py` & `SpecLab-4.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 from distutils.core import setup
 from pathlib import Path
 
-
-try:
-   import pypandoc
-   long_desc = pypandoc.convert_file('SpecLab/doc/README.md', 'rst')
-except(IOError, ImportError):
-   long_desc = open('SpecLab/doc/README.md').read()
-
 setup(
     name='SpecLab',
-    version='4.2.0',
+    version='4.2.1',
     author='A. F. Kowalski',
     author_email='adam.f.kowalski@colorado.edu',
     packages=['SpecLab','SpecLab.aux','SpecLab.aux.param_files','SpecLab.imXam','SpecLab.doc','SpecLab.gen',],
     package_data = {'':['*.tar.gz', '*.txt', '*.dat', '*.md', '*.rst'],},
    # include_package_data=True,
    # package_dir={"": ""},
     scripts=['SpecLab/cfg/SpecLab_config.py','SpecLab/imXam/imXam.py','SpecLab/cfg/epar_imXam.py',],
     url='http://pypi.python.org/pypi/SpecLab/',
-    description='IRAF imexam+DS9 replacement for Python',long_description_content_type='text/markdown',
+    description='IRAF imexam+DS9 alternative for Python',long_description_content_type='text/markdown',
     long_description=open('SpecLab/doc/README.md').read(),
     install_requires=['numpy>=1.25.0', 'plotly>=5.15.0', 'pandas>=2.0.3','astropy>=5.3.1','scipy>=1.11.1','matplotlib>=3.7.2','PyQt6==6.5.1', 'photutils>=1.8.0','pyqtgraph==0.13.3',]
 )
 
 # python setup.py sdist
 # python -m twine upload --repository testpypi dist/*
 # pip install -i https://test.pypi.org/simple/ speclab-imXam==3.1.2
```

