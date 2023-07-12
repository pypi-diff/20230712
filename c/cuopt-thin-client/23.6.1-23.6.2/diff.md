# Comparing `tmp/cuopt-thin-client-23.6.1.tar.gz` & `tmp/cuopt-thin-client-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuopt-thin-client-23.6.1.tar", last modified: Fri Jun 30 16:06:57 2023, max compression
+gzip compressed data, was "cuopt-thin-client-23.6.2.tar", last modified: Wed Jul 12 06:06:49 2023, max compression
```

## Comparing `cuopt-thin-client-23.6.1.tar` & `cuopt-thin-client-23.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-30 16:06:57.633548 cuopt-thin-client-23.6.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      449 2023-06-30 16:06:57.000000 cuopt-thin-client-23.6.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 10:03:35.000000 cuopt-thin-client-23.6.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2023-06-30 16:06:57.000000 cuopt-thin-client-23.6.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-30 16:06:57.633548 cuopt-thin-client-23.6.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      256 2023-06-30 16:06:57.000000 cuopt-thin-client-23.6.1/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-30 16:06:57.633548 cuopt-thin-client-23.6.1/cuopt_thin_client.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-06-30 16:06:57.000000 cuopt-thin-client-23.6.1/cuopt_thin_client.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2023-06-30 16:06:57.000000 cuopt-thin-client-23.6.1/cuopt_thin_client.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-30 16:06:57.000000 cuopt-thin-client-23.6.1/cuopt_thin_client.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-30 16:06:57.000000 cuopt-thin-client-23.6.1/cuopt_thin_client.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-30 16:06:57.634548 cuopt-thin-client-23.6.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 10:03:35.000000 cuopt-thin-client-23.6.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-12 06:06:49.098726 cuopt-thin-client-23.6.2/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      449 2023-07-12 06:06:49.000000 cuopt-thin-client-23.6.2/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 10:03:35.000000 cuopt-thin-client-23.6.2/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2023-07-12 06:06:49.000000 cuopt-thin-client-23.6.2/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-07-12 06:06:49.097726 cuopt-thin-client-23.6.2/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      256 2023-07-12 06:06:49.000000 cuopt-thin-client-23.6.2/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-12 06:06:49.097726 cuopt-thin-client-23.6.2/cuopt_thin_client.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1616 2023-07-12 06:06:49.000000 cuopt-thin-client-23.6.2/cuopt_thin_client.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2023-07-12 06:06:49.000000 cuopt-thin-client-23.6.2/cuopt_thin_client.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-12 06:06:49.000000 cuopt-thin-client-23.6.2/cuopt_thin_client.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-12 06:06:49.000000 cuopt-thin-client-23.6.2/cuopt_thin_client.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-12 06:06:49.098726 cuopt-thin-client-23.6.2/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 10:03:35.000000 cuopt-thin-client-23.6.2/setup.py
```

### Comparing `cuopt-thin-client-23.6.1/LICENSE.md` & `cuopt-thin-client-23.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cuopt-thin-client-23.6.1/PKG-INFO` & `cuopt-thin-client-23.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuopt-thin-client
-Version: 23.6.1
+Version: 23.6.2
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cuopt-thin-client-23.6.1/cuopt_thin_client.egg-info/PKG-INFO` & `cuopt-thin-client-23.6.2/cuopt_thin_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuopt-thin-client
-Version: 23.6.1
+Version: 23.6.2
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cuopt-thin-client-23.6.1/setup.py` & `cuopt-thin-client-23.6.2/setup.py`

 * *Files identical despite different names*

