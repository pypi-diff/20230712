# Comparing `tmp/oxasl-ve-0.2.0.post5.tar.gz` & `tmp/oxasl-ve-0.2.0.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oxasl-ve-0.2.0.post5.tar", last modified: Tue Jul 11 12:08:57 2023, max compression
+gzip compressed data, was "oxasl-ve-0.2.0.post6.tar", last modified: Wed Jul 12 12:35:27 2023, max compression
```

## Comparing `oxasl-ve-0.2.0.post5.tar` & `oxasl-ve-0.2.0.post6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/
--rw-r--r--   0 martin    (1000) martin    (1000)    10174 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post5/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1000)       33 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     1001 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      356 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/README.md
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/oxasl_ve/
--rw-r--r--   0 martin    (1000) martin    (1000)      632 2023-07-11 12:08:12.000000 oxasl-ve-0.2.0.post5/oxasl_ve/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)       77 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve/_version.py
--rw-r--r--   0 martin    (1000) martin    (1000)    22544 2023-07-11 12:08:29.000000 oxasl-ve-0.2.0.post5/oxasl_ve/api.py
--rwxr-xr-x   0 martin    (1000) martin    (1000)    36072 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/oxasl_ve/modmat_default.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1845 2023-07-11 12:08:12.000000 oxasl-ve-0.2.0.post5/oxasl_ve/veaslc_cli_wrapper.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/oxasl_ve/wrappers/
--rw-r--r--   0 martin    (1000) martin    (1000)       49 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/oxasl_ve/wrappers/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1006 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post5/oxasl_ve/wrappers/veaslc.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     1001 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      388 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       24 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        9 2023-07-11 12:08:56.000000 oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/top_level.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       25 2023-07-11 12:03:38.000000 oxasl-ve-0.2.0.post5/requirements.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-07-11 12:08:57.000000 oxasl-ve-0.2.0.post5/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)     3768 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post5/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-12 12:35:27.758793 oxasl-ve-0.2.0.post6/
+-rw-r--r--   0 martin    (1000) martin    (1000)    10174 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post6/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1000)       33 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)      981 2023-07-12 12:35:27.748793 oxasl-ve-0.2.0.post6/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      356 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/README.md
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-12 12:35:27.748793 oxasl-ve-0.2.0.post6/oxasl_ve/
+-rw-r--r--   0 martin    (1000) martin    (1000)      642 2023-07-12 12:33:06.000000 oxasl-ve-0.2.0.post6/oxasl_ve/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)       77 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve/_version.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    22544 2023-07-12 12:32:40.000000 oxasl-ve-0.2.0.post6/oxasl_ve/api.py
+-rwxr-xr-x   0 martin    (1000) martin    (1000)    36072 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/oxasl_ve/modmat_default.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1845 2023-07-11 12:08:12.000000 oxasl-ve-0.2.0.post6/oxasl_ve/veaslc_cli_wrapper.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-12 12:35:27.748793 oxasl-ve-0.2.0.post6/oxasl_ve/wrappers/
+-rw-r--r--   0 martin    (1000) martin    (1000)       49 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/oxasl_ve/wrappers/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1006 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/oxasl_ve/wrappers/veaslc.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-12 12:35:27.748793 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)      981 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      388 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       24 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        9 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/top_level.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       25 2023-07-11 12:03:38.000000 oxasl-ve-0.2.0.post6/requirements.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-07-12 12:35:27.758793 oxasl-ve-0.2.0.post6/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)     3768 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `oxasl-ve-0.2.0.post5/LICENSE` & `oxasl-ve-0.2.0.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post5/PKG-INFO` & `oxasl-ve-0.2.0.post6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: oxasl-ve
-Version: 0.2.0.post5
+Version: 0.2.0.post6
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -22,9 +21,7 @@
 processing pipeline
 
 ## Citation
 
 *A General Framework for the Analysis of Vessel Encoded Arterial Spin Labelling for Vascular Territory Mapping*
 M Chappell, T Okell, P Jezzard and M Woolrich
 Magnetic Resonance in Medicine 64:1529-1539 (2010)
-
-
```

### Comparing `oxasl-ve-0.2.0.post5/oxasl_ve/__init__.py` & `oxasl-ve-0.2.0.post6/oxasl_ve/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 If installed, then it will be called by ``oxasl.oxford_asl.oxasl``
 whenever vessel-encoded data is supplied.
 
 The relevant processing function can also be called independently
 on a ``Workspace`` object, however this will not include the
 standard oxasl preprocessing or registration.
 """
-from .api import run, VeaslOptions, two_to_mac, mac_to_two, veslocs_to_enc, generate_mask
+from .api import model_ve, VeaslOptions, two_to_mac, mac_to_two, veslocs_to_enc, generate_mask
 from ._version import __version__
 
-__all__ = ["__version__", "run", "VeaslOptions", "two_to_mac", "mac_to_two", "veslocs_to_enc", "generate_mask"]
+__all__ = ["__version__", "model_ve", "VeaslOptions", "two_to_mac", "mac_to_two", "veslocs_to_enc", "generate_mask"]
```

### Comparing `oxasl-ve-0.2.0.post5/oxasl_ve/api.py` & `oxasl-ve-0.2.0.post6/oxasl_ve/api.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post5/oxasl_ve/modmat_default.py` & `oxasl-ve-0.2.0.post6/oxasl_ve/modmat_default.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post5/oxasl_ve/veaslc_cli_wrapper.py` & `oxasl-ve-0.2.0.post6/oxasl_ve/veaslc_cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post5/oxasl_ve/wrappers/veaslc.py` & `oxasl-ve-0.2.0.post6/oxasl_ve/wrappers/veaslc.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post5/oxasl_ve.egg-info/PKG-INFO` & `oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: oxasl-ve
-Version: 0.2.0.post5
+Version: 0.2.0.post6
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -22,9 +21,7 @@
 processing pipeline
 
 ## Citation
 
 *A General Framework for the Analysis of Vessel Encoded Arterial Spin Labelling for Vascular Territory Mapping*
 M Chappell, T Okell, P Jezzard and M Woolrich
 Magnetic Resonance in Medicine 64:1529-1539 (2010)
-
-
```

### Comparing `oxasl-ve-0.2.0.post5/setup.py` & `oxasl-ve-0.2.0.post6/setup.py`

 * *Files identical despite different names*

