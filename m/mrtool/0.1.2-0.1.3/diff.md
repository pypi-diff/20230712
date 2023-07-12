# Comparing `tmp/mrtool-0.1.2.tar.gz` & `tmp/mrtool-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrtool-0.1.2.tar", last modified: Wed Apr 26 18:55:07 2023, max compression
+gzip compressed data, was "mrtool-0.1.3.tar", last modified: Wed Jul 12 17:07:29 2023, max compression
```

## Comparing `mrtool-0.1.2.tar` & `mrtool-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-26 18:54:05.000000 mrtool-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 18:55:07.990967 mrtool-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-26 18:54:05.000000 mrtool-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 18:54:05.000000 mrtool-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 18:55:07.994967 mrtool-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 18:54:05.000000 mrtool-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.986967 mrtool-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.986967 mrtool-0.1.2/src/mrtool/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/src/mrtool/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35415 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/cov_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/src/mrtool/cov_selection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/cov_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/cov_selection/covfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/src/mrtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:54:13.000000 mrtool-0.1.2/src/mrtool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-04-26 18:54:05.000000 mrtool-0.1.2/tests/test_covmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-26 18:54:05.000000 mrtool-0.1.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-26 18:54:05.000000 mrtool-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:07:29.244793 mrtool-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-12 17:06:30.000000 mrtool-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-12 17:07:29.244793 mrtool-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-12 17:06:30.000000 mrtool-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-12 17:06:30.000000 mrtool-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:07:29.244793 mrtool-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:07:29.240793 mrtool-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:07:29.244793 mrtool-0.1.3/src/mrtool/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-12 17:06:30.000000 mrtool-0.1.3/src/mrtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:07:29.244793 mrtool-0.1.3/src/mrtool/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:30.000000 mrtool-0.1.3/src/mrtool/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35415 2023-07-12 17:06:30.000000 mrtool-0.1.3/src/mrtool/core/cov_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-07-12 17:06:30.000000 mrtool-0.1.3/src/mrtool/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-12 17:06:30.000000 mrtool-0.1.3/src/mrtool/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-12 17:06:30.000000 mrtool-0.1.3/src/mrtool/core/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17850 2023-07-12 17:06:30.000000 mrtool-0.1.3/src/mrtool/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:07:29.244793 mrtool-0.1.3/src/mrtool/cov_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:30.000000 mrtool-0.1.3/src/mrtool/cov_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-07-12 17:06:30.000000 mrtool-0.1.3/src/mrtool/cov_selection/covfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:07:29.244793 mrtool-0.1.3/src/mrtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-12 17:07:29.000000 mrtool-0.1.3/src/mrtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-12 17:07:29.000000 mrtool-0.1.3/src/mrtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:07:29.000000 mrtool-0.1.3/src/mrtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-12 17:07:29.000000 mrtool-0.1.3/src/mrtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 17:07:29.000000 mrtool-0.1.3/src/mrtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:07:29.244793 mrtool-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-07-12 17:06:30.000000 mrtool-0.1.3/tests/test_covmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-12 17:06:30.000000 mrtool-0.1.3/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-12 17:06:30.000000 mrtool-0.1.3/tests/test_utils.py
```

### Comparing `mrtool-0.1.2/LICENSE` & `mrtool-0.1.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2020, IHME Math Sciences
+Copyright (c) 2023, IHME Math Sciences
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `mrtool-0.1.2/README.rst` & `mrtool-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.2/src/mrtool/core/cov_model.py` & `mrtool-0.1.3/src/mrtool/core/cov_model.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.2/src/mrtool/core/data.py` & `mrtool-0.1.3/src/mrtool/core/data.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.2/src/mrtool/core/model.py` & `mrtool-0.1.3/src/mrtool/core/model.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.2/src/mrtool/core/plots.py` & `mrtool-0.1.3/src/mrtool/core/plots.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.2/src/mrtool/core/utils.py` & `mrtool-0.1.3/src/mrtool/core/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,22 +459,24 @@
 
     if alt_mat.size == 0:
         fun = None
         jac_fun = None
     else:
         if ref_mat is None or ref_mat.size == 0:
             def fun(beta):
-                return np.log(shift + alt_mat.dot(beta))
+                alt_val = np.abs(shift + alt_mat.dot(beta))
+                return np.log(alt_val)
 
             def jac_fun(beta):
                 return alt_mat/(shift + alt_mat.dot(beta)[:, None])
         else:
             def fun(beta):
-                return np.log(shift + alt_mat.dot(beta)) - \
-                       np.log(shift + ref_mat.dot(beta))
+                alt_val = np.abs(shift + alt_mat.dot(beta))
+                ref_val = np.abs(shift + ref_mat.dot(beta))
+                return np.log(alt_val) - np.log(ref_val)
 
             def jac_fun(beta):
                 return alt_mat/(shift + alt_mat.dot(beta)[:, None]) - \
                        ref_mat/(shift + ref_mat.dot(beta)[:, None])
 
     return fun, jac_fun
```

### Comparing `mrtool-0.1.2/src/mrtool/cov_selection/covfinder.py` & `mrtool-0.1.3/src/mrtool/cov_selection/covfinder.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.2/src/mrtool.egg-info/SOURCES.txt` & `mrtool-0.1.3/src/mrtool.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
 src/mrtool/__init__.py
 src/mrtool.egg-info/PKG-INFO
 src/mrtool.egg-info/SOURCES.txt
 src/mrtool.egg-info/dependency_links.txt
-src/mrtool.egg-info/not-zip-safe
 src/mrtool.egg-info/requires.txt
 src/mrtool.egg-info/top_level.txt
 src/mrtool/core/__init__.py
 src/mrtool/core/cov_model.py
 src/mrtool/core/data.py
 src/mrtool/core/model.py
 src/mrtool/core/plots.py
```

### Comparing `mrtool-0.1.2/tests/test_covmodel.py` & `mrtool-0.1.3/tests/test_covmodel.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.2/tests/test_data.py` & `mrtool-0.1.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.2/tests/test_utils.py` & `mrtool-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

