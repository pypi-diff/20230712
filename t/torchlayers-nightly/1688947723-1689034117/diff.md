# Comparing `tmp/torchlayers-nightly-1688947723.tar.gz` & `tmp/torchlayers-nightly-1689034117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchlayers-nightly-1688947723.tar", last modified: Mon Jul 10 00:08:52 2023, max compression
+gzip compressed data, was "dist/torchlayers-nightly-1689034117.tar", last modified: Tue Jul 11 00:08:46 2023, max compression
```

## Comparing `torchlayers-nightly-1688947723.tar` & `torchlayers-nightly-1689034117.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/attributes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/convolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/general_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/jit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/padding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/pickle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/recurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/tests/torchlayers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/torchlayers/
--rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/torchlayers/_dev_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/_dev_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/_dev_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/_dev_utils/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    36698 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-10 00:08:43.000000 torchlayers-nightly-1688947723/torchlayers/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/torchlayers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/torchlayers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/torchlayers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/torchlayers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/torchlayers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 00:08:52.000000 torchlayers-nightly-1688947723/torchlayers_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/
+-rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/attributes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/convolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/general_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/jit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/padding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/pickle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/recurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/tests/torchlayers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/torchlayers/
+-rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/torchlayers/_dev_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/_dev_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/_dev_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/_dev_utils/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36698 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-11 00:08:37.000000 torchlayers-nightly-1689034117/torchlayers/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/torchlayers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/torchlayers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/torchlayers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/torchlayers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/torchlayers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 00:08:46.000000 torchlayers-nightly-1689034117/torchlayers_nightly.egg-info/top_level.txt
```

### Comparing `torchlayers-nightly-1688947723/PKG-INFO` & `torchlayers-nightly-1689034117/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlayers-nightly
-Version: 1688947723
+Version: 1689034117
 Summary: Input shape inference and SOTA custom layers for PyTorch.
 Home-page: https://github.com/pypa/torchlayers
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchlayers
 Project-URL: Documentation, https://szymonmaszke.github.io/torchlayers/#torchlayers
```

### Comparing `torchlayers-nightly-1688947723/README.md` & `torchlayers-nightly-1689034117/README.md`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/setup.py` & `torchlayers-nightly-1689034117/setup.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/tests/convolution_test.py` & `torchlayers-nightly-1689034117/tests/convolution_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/tests/general_test.py` & `torchlayers-nightly-1689034117/tests/general_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/tests/jit_test.py` & `torchlayers-nightly-1689034117/tests/jit_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/tests/pickle_test.py` & `torchlayers-nightly-1689034117/tests/pickle_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/tests/preprocessing_test.py` & `torchlayers-nightly-1689034117/tests/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/tests/regularization_test.py` & `torchlayers-nightly-1689034117/tests/regularization_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/tests/torchlayers_test.py` & `torchlayers-nightly-1689034117/tests/torchlayers_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/__init__.py` & `torchlayers-nightly-1689034117/torchlayers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/_dev_utils/helpers.py` & `torchlayers-nightly-1689034117/torchlayers/_dev_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/_dev_utils/infer.py` & `torchlayers-nightly-1689034117/torchlayers/_dev_utils/infer.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/activations.py` & `torchlayers-nightly-1689034117/torchlayers/activations.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/convolution.py` & `torchlayers-nightly-1689034117/torchlayers/convolution.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/module.py` & `torchlayers-nightly-1689034117/torchlayers/module.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/normalization.py` & `torchlayers-nightly-1689034117/torchlayers/normalization.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/pooling.py` & `torchlayers-nightly-1689034117/torchlayers/pooling.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/preprocessing.py` & `torchlayers-nightly-1689034117/torchlayers/preprocessing.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/regularization.py` & `torchlayers-nightly-1689034117/torchlayers/regularization.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers/upsample.py` & `torchlayers-nightly-1689034117/torchlayers/upsample.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1688947723/torchlayers_nightly.egg-info/PKG-INFO` & `torchlayers-nightly-1689034117/torchlayers_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlayers-nightly
-Version: 1688947723
+Version: 1689034117
 Summary: Input shape inference and SOTA custom layers for PyTorch.
 Home-page: https://github.com/pypa/torchlayers
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchlayers
 Project-URL: Documentation, https://szymonmaszke.github.io/torchlayers/#torchlayers
```

### Comparing `torchlayers-nightly-1688947723/torchlayers_nightly.egg-info/SOURCES.txt` & `torchlayers-nightly-1689034117/torchlayers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

