# Comparing `tmp/bci-essentials-0.0.3.tar.gz` & `tmp/bci-essentials-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bci-essentials-0.0.3.tar", last modified: Tue Jul 11 23:40:14 2023, max compression
+gzip compressed data, was "bci-essentials-0.0.4.tar", last modified: Wed Jul 12 18:28:58 2023, max compression
```

## Comparing `bci-essentials-0.0.3.tar` & `bci-essentials-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/bci_essentials/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71000 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/bci_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/channel_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    54254 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/resting_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/bci_essentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:28:58.801367 bci-essentials-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-12 18:28:58.801367 bci-essentials-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:28:58.801367 bci-essentials-0.0.4/bci_essentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/bci_essentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71000 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/bci_essentials/bci_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/bci_essentials/channel_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54254 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/bci_essentials/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/bci_essentials/resting_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/bci_essentials/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/bci_essentials/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:28:58.801367 bci-essentials-0.0.4/bci_essentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-12 18:28:58.000000 bci-essentials-0.0.4/bci_essentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-12 18:28:58.000000 bci-essentials-0.0.4/bci_essentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:28:58.000000 bci-essentials-0.0.4/bci_essentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-12 18:28:58.000000 bci-essentials-0.0.4/bci_essentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 18:28:58.000000 bci-essentials-0.0.4/bci_essentials.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 18:26:19.000000 bci-essentials-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:28:58.801367 bci-essentials-0.0.4/setup.cfg
```

### Comparing `bci-essentials-0.0.3/LICENSE` & `bci-essentials-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.3/PKG-INFO` & `bci-essentials-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: bci-essentials
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python backend for bci-essentials
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bci-essentials-python
 This repository contains python modules and scripts for the processing of EEG-based BCI. 
 These modules are specifically designed to be equivalent whether run offline or online.
 
 
 ## Related packages
-### bci-essentials-unity
 The front end for this package can be found in [bci-essentials-unity](https://www.github.com/kirtonBCIlab/bci-essentials-unity)
 
 ## Getting Started
 
 BCI Essentials requires Python 3.9 or later.  To install for Windows, MacOS or Linux:
 
 ```
 pip install bci-essentials
 ```
 
-On some systems, it may be necessary to install [liblsl](https://github.com/sccn/liblsl).  Alternatively, you can use the Conda to set up dependencies that are not provided by pip:
+On some systems, it may be necessary to install [liblsl](https://github.com/sccn/liblsl).  Alternatively, use the Conda [environment](/environment.yml) to set up dependencies that are not provided by pip:
 
 ```
 conda env create -f ./environment.yml
 conda activate bci
 ```
 
 ## Offline processing
```

### Comparing `bci-essentials-0.0.3/README.md` & `bci-essentials-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # bci-essentials-python
 This repository contains python modules and scripts for the processing of EEG-based BCI. 
 These modules are specifically designed to be equivalent whether run offline or online.
 
 
 ## Related packages
-### bci-essentials-unity
 The front end for this package can be found in [bci-essentials-unity](https://www.github.com/kirtonBCIlab/bci-essentials-unity)
 
 ## Getting Started
 
 BCI Essentials requires Python 3.9 or later.  To install for Windows, MacOS or Linux:
 
 ```
 pip install bci-essentials
 ```
 
-On some systems, it may be necessary to install [liblsl](https://github.com/sccn/liblsl).  Alternatively, you can use the Conda to set up dependencies that are not provided by pip:
+On some systems, it may be necessary to install [liblsl](https://github.com/sccn/liblsl).  Alternatively, use the Conda [environment](/environment.yml) to set up dependencies that are not provided by pip:
 
 ```
 conda env create -f ./environment.yml
 conda activate bci
 ```
 
 ## Offline processing
```

### Comparing `bci-essentials-0.0.3/bci_essentials/bci_data.py` & `bci-essentials-0.0.4/bci_essentials/bci_data.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.3/bci_essentials/channel_selection.py` & `bci-essentials-0.0.4/bci_essentials/channel_selection.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.3/bci_essentials/classification.py` & `bci-essentials-0.0.4/bci_essentials/classification.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.3/bci_essentials/resting_state.py` & `bci-essentials-0.0.4/bci_essentials/resting_state.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.3/bci_essentials/signal_processing.py` & `bci-essentials-0.0.4/bci_essentials/signal_processing.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.3/bci_essentials/visuals.py` & `bci-essentials-0.0.4/bci_essentials/visuals.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.3/bci_essentials.egg-info/PKG-INFO` & `bci-essentials-0.0.4/bci_essentials.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: bci-essentials
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python backend for bci-essentials
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bci-essentials-python
 This repository contains python modules and scripts for the processing of EEG-based BCI. 
 These modules are specifically designed to be equivalent whether run offline or online.
 
 
 ## Related packages
-### bci-essentials-unity
 The front end for this package can be found in [bci-essentials-unity](https://www.github.com/kirtonBCIlab/bci-essentials-unity)
 
 ## Getting Started
 
 BCI Essentials requires Python 3.9 or later.  To install for Windows, MacOS or Linux:
 
 ```
 pip install bci-essentials
 ```
 
-On some systems, it may be necessary to install [liblsl](https://github.com/sccn/liblsl).  Alternatively, you can use the Conda to set up dependencies that are not provided by pip:
+On some systems, it may be necessary to install [liblsl](https://github.com/sccn/liblsl).  Alternatively, use the Conda [environment](/environment.yml) to set up dependencies that are not provided by pip:
 
 ```
 conda env create -f ./environment.yml
 conda activate bci
 ```
 
 ## Offline processing
```

### Comparing `bci-essentials-0.0.3/pyproject.toml` & `bci-essentials-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bci-essentials"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python backend for bci-essentials"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
 	"numpy",
 	"scipy",
 	"scikit-learn",
```

