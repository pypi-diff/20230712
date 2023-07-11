# Comparing `tmp/bci-essentials-0.0.2.tar.gz` & `tmp/bci-essentials-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bci-essentials-0.0.2.tar", last modified: Tue Jul 11 22:05:20 2023, max compression
+gzip compressed data, was "bci-essentials-0.0.3.tar", last modified: Tue Jul 11 23:40:14 2023, max compression
```

## Comparing `bci-essentials-0.0.2.tar` & `bci-essentials-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gregwilding   (501) staff       (20)        0 2023-07-11 22:05:20.453771 bci-essentials-0.0.2/
--rw-r--r--   0 gregwilding   (501) staff       (20)     1065 2023-07-11 22:03:22.000000 bci-essentials-0.0.2/LICENSE
--rw-r--r--   0 gregwilding   (501) staff       (20)     3581 2023-07-11 22:05:20.453644 bci-essentials-0.0.2/PKG-INFO
--rw-r--r--   0 gregwilding   (501) staff       (20)     3394 2023-07-05 14:33:28.000000 bci-essentials-0.0.2/README.md
-drwxr-xr-x   0 gregwilding   (501) staff       (20)        0 2023-07-11 22:05:20.452700 bci-essentials-0.0.2/bci_essentials/
--rw-r--r--   0 gregwilding   (501) staff       (20)      286 2023-05-05 16:48:22.000000 bci-essentials-0.0.2/bci_essentials/__init__.py
--rw-r--r--   0 gregwilding   (501) staff       (20)    71000 2023-05-05 16:48:22.000000 bci-essentials-0.0.2/bci_essentials/bci_data.py
--rw-r--r--   0 gregwilding   (501) staff       (20)    16414 2023-05-05 16:48:22.000000 bci-essentials-0.0.2/bci_essentials/channel_selection.py
--rw-r--r--   0 gregwilding   (501) staff       (20)    54254 2023-07-05 14:33:28.000000 bci-essentials-0.0.2/bci_essentials/classification.py
--rw-r--r--   0 gregwilding   (501) staff       (20)     7257 2023-05-05 16:48:22.000000 bci-essentials-0.0.2/bci_essentials/resting_state.py
--rw-r--r--   0 gregwilding   (501) staff       (20)     5470 2023-05-05 16:48:22.000000 bci-essentials-0.0.2/bci_essentials/signal_processing.py
--rw-r--r--   0 gregwilding   (501) staff       (20)     5393 2022-11-25 23:17:55.000000 bci-essentials-0.0.2/bci_essentials/visuals.py
-drwxr-xr-x   0 gregwilding   (501) staff       (20)        0 2023-07-11 22:05:20.453467 bci-essentials-0.0.2/bci_essentials.egg-info/
--rw-r--r--   0 gregwilding   (501) staff       (20)     3581 2023-07-11 22:05:20.000000 bci-essentials-0.0.2/bci_essentials.egg-info/PKG-INFO
--rw-r--r--   0 gregwilding   (501) staff       (20)      438 2023-07-11 22:05:20.000000 bci-essentials-0.0.2/bci_essentials.egg-info/SOURCES.txt
--rw-r--r--   0 gregwilding   (501) staff       (20)        1 2023-07-11 22:05:20.000000 bci-essentials-0.0.2/bci_essentials.egg-info/dependency_links.txt
--rw-r--r--   0 gregwilding   (501) staff       (20)      195 2023-07-11 22:05:20.000000 bci-essentials-0.0.2/bci_essentials.egg-info/requires.txt
--rw-r--r--   0 gregwilding   (501) staff       (20)       20 2023-07-11 22:05:20.000000 bci-essentials-0.0.2/bci_essentials.egg-info/top_level.txt
--rw-r--r--   0 gregwilding   (501) staff       (20)      597 2023-07-11 22:03:18.000000 bci-essentials-0.0.2/pyproject.toml
--rw-r--r--   0 gregwilding   (501) staff       (20)       38 2023-07-11 22:05:20.453819 bci-essentials-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/bci_essentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71000 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/bci_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/channel_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54254 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/resting_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/bci_essentials/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/bci_essentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 23:40:14.000000 bci-essentials-0.0.3/bci_essentials.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-11 23:36:47.000000 bci-essentials-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 23:40:14.900561 bci-essentials-0.0.3/setup.cfg
```

### Comparing `bci-essentials-0.0.2/LICENSE` & `bci-essentials-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.2/PKG-INFO` & `bci-essentials-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,31 @@
-Metadata-Version: 2.1
-Name: bci-essentials
-Version: 0.0.2
-Summary: Python backend for bci-essentials
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # bci-essentials-python
 This repository contains python modules and scripts for the processing of EEG-based BCI. 
 These modules are specifically designed to be equivalent whether run offline or online.
 
 
 ## Related packages
 ### bci-essentials-unity
 The front end for this package can be found in [bci-essentials-unity](https://www.github.com/kirtonBCIlab/bci-essentials-unity)
 
 ## Getting Started
 
-Using the terminal
-1. Clone from git
+BCI Essentials requires Python 3.9 or later.  To install for Windows, MacOS or Linux:
+
 ```
-git clone https://github.com/kirtonBCIlab/bci-essentials-python.git
-cd bci-essentials-python
+pip install bci-essentials
 ```
 
-2. Create and activate a conda environment (RECOMMENDED)
+On some systems, it may be necessary to install [liblsl](https://github.com/sccn/liblsl).  Alternatively, you can use the Conda to set up dependencies that are not provided by pip:
+
 ```
 conda env create -f ./environment.yml
 conda activate bci
 ```
 
-3. Install dependencies with pip
-```
-pip install .
-```
-
-
 ## Offline processing
 Offline processing can be done by running the corresponding offline test script (ie. mi_offline_test.py, p300_offline_test.py, etc.)
 Change the filename in the script to point to the data you want to process.
 ```
 python examples/mi_offline_test.py
 ```
```

### Comparing `bci-essentials-0.0.2/README.md` & `bci-essentials-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
+Metadata-Version: 2.1
+Name: bci-essentials
+Version: 0.0.3
+Summary: Python backend for bci-essentials
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bci-essentials-python
 This repository contains python modules and scripts for the processing of EEG-based BCI. 
 These modules are specifically designed to be equivalent whether run offline or online.
 
 
 ## Related packages
 ### bci-essentials-unity
 The front end for this package can be found in [bci-essentials-unity](https://www.github.com/kirtonBCIlab/bci-essentials-unity)
 
 ## Getting Started
 
-Using the terminal
-1. Clone from git
+BCI Essentials requires Python 3.9 or later.  To install for Windows, MacOS or Linux:
+
 ```
-git clone https://github.com/kirtonBCIlab/bci-essentials-python.git
-cd bci-essentials-python
+pip install bci-essentials
 ```
 
-2. Create and activate a conda environment (RECOMMENDED)
+On some systems, it may be necessary to install [liblsl](https://github.com/sccn/liblsl).  Alternatively, you can use the Conda to set up dependencies that are not provided by pip:
+
 ```
 conda env create -f ./environment.yml
 conda activate bci
 ```
 
-3. Install dependencies with pip
-```
-pip install .
-```
-
-
 ## Offline processing
 Offline processing can be done by running the corresponding offline test script (ie. mi_offline_test.py, p300_offline_test.py, etc.)
 Change the filename in the script to point to the data you want to process.
 ```
 python examples/mi_offline_test.py
 ```
```

### Comparing `bci-essentials-0.0.2/bci_essentials/bci_data.py` & `bci-essentials-0.0.3/bci_essentials/bci_data.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.2/bci_essentials/channel_selection.py` & `bci-essentials-0.0.3/bci_essentials/channel_selection.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.2/bci_essentials/classification.py` & `bci-essentials-0.0.3/bci_essentials/classification.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.2/bci_essentials/resting_state.py` & `bci-essentials-0.0.3/bci_essentials/resting_state.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.2/bci_essentials/signal_processing.py` & `bci-essentials-0.0.3/bci_essentials/signal_processing.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.2/bci_essentials/visuals.py` & `bci-essentials-0.0.3/bci_essentials/visuals.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.2/bci_essentials.egg-info/PKG-INFO` & `bci-essentials-0.0.3/bci_essentials.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bci-essentials
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python backend for bci-essentials
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bci-essentials-python
 This repository contains python modules and scripts for the processing of EEG-based BCI. 
@@ -13,33 +13,27 @@
 
 ## Related packages
 ### bci-essentials-unity
 The front end for this package can be found in [bci-essentials-unity](https://www.github.com/kirtonBCIlab/bci-essentials-unity)
 
 ## Getting Started
 
-Using the terminal
-1. Clone from git
+BCI Essentials requires Python 3.9 or later.  To install for Windows, MacOS or Linux:
+
 ```
-git clone https://github.com/kirtonBCIlab/bci-essentials-python.git
-cd bci-essentials-python
+pip install bci-essentials
 ```
 
-2. Create and activate a conda environment (RECOMMENDED)
+On some systems, it may be necessary to install [liblsl](https://github.com/sccn/liblsl).  Alternatively, you can use the Conda to set up dependencies that are not provided by pip:
+
 ```
 conda env create -f ./environment.yml
 conda activate bci
 ```
 
-3. Install dependencies with pip
-```
-pip install .
-```
-
-
 ## Offline processing
 Offline processing can be done by running the corresponding offline test script (ie. mi_offline_test.py, p300_offline_test.py, etc.)
 Change the filename in the script to point to the data you want to process.
 ```
 python examples/mi_offline_test.py
 ```
```

### Comparing `bci-essentials-0.0.2/pyproject.toml` & `bci-essentials-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bci-essentials"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python backend for bci-essentials"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
 	"numpy",
 	"scipy",
 	"scikit-learn",
```

