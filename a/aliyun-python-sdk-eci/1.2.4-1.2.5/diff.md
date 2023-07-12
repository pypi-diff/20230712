# Comparing `tmp/aliyun-python-sdk-eci-1.2.4.tar.gz` & `tmp/aliyun-python-sdk-eci-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-eci-1.2.4.tar", last modified: Mon May 15 06:51:48 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-eci-1.2.5.tar", last modified: Wed Jul 12 03:35:05 2023, max compression
```

## Comparing `aliyun-python-sdk-eci-1.2.4.tar` & `aliyun-python-sdk-eci-1.2.5.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1321 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      351 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyun_python_sdk_eci.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1321 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyun_python_sdk_eci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1607 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyun_python_sdk_eci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyun_python_sdk_eci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyun_python_sdk_eci.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyun_python_sdk_eci.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/
--rwxr-xr-x   0 root         (0) root         (0)       22 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/
--rw-r--r--   0 root         (0) root         (0)     2360 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/CommitContainerRequest.py
--rwxr-xr-x   0 root         (0) root         (0)    36659 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/CreateContainerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     6260 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/CreateImageCacheRequest.py
--rwxr-xr-x   0 root         (0) root         (0)     2167 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DeleteContainerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2087 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DeleteContainerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2111 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DeleteImageCacheRequest.py
--rw-r--r--   0 root         (0) root         (0)     2478 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeAvailableResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeCommitContainerTaskRequest.py
--rwxr-xr-x   0 root         (0) root         (0)     2448 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeContainerGroupMetricRequest.py
--rwxr-xr-x   0 root         (0) root         (0)     2791 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeContainerGroupPriceRequest.py
--rwxr-xr-x   0 root         (0) root         (0)     3562 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeContainerGroupsRequest.py
--rwxr-xr-x   0 root         (0) root         (0)     2456 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeContainerLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeImageCachesRequest.py
--rwxr-xr-x   0 root         (0) root         (0)     2198 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeMultiContainerGroupMetricRequest.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeRegionsRequest.py
--rwxr-xr-x   0 root         (0) root         (0)     2749 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/ExecContainerCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/ListUsageRequest.py
--rwxr-xr-x   0 root         (0) root         (0)     2144 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/RestartContainerGroupRequest.py
--rwxr-xr-x   0 root         (0) root         (0)    21339 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/UpdateContainerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     7186 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/UpdateImageCacheRequest.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2452 2023-05-15 06:51:48.000000 aliyun-python-sdk-eci-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      351 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyun_python_sdk_eci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyun_python_sdk_eci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyun_python_sdk_eci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyun_python_sdk_eci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyun_python_sdk_eci.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyun_python_sdk_eci.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/
+-rwxr-xr-x   0 root         (0) root         (0)       22 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/CommitContainerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/CopyDataCacheRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)    36659 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/CreateContainerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/CreateDataCacheRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6260 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/CreateImageCacheRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)     2167 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DeleteContainerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DeleteContainerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DeleteDataCacheRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DeleteImageCacheRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeAvailableResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeCommitContainerTaskRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)     2448 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeContainerGroupMetricRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)     2791 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeContainerGroupPriceRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)     3562 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeContainerGroupsRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)     2456 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeContainerLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeDataCachesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeImageCachesRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)     2198 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeMultiContainerGroupMetricRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeRegionsRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)     2749 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/ExecContainerCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/ListUsageRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)     2144 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/RestartContainerGroupRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)    21339 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/UpdateContainerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/UpdateDataCacheRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7186 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/UpdateImageCacheRequest.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2452 2023-07-12 03:35:05.000000 aliyun-python-sdk-eci-1.2.5/setup.py
```

### Comparing `aliyun-python-sdk-eci-1.2.4/PKG-INFO` & `aliyun-python-sdk-eci-1.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eci
-Version: 1.2.4
+Version: 1.2.5
 Summary: The eci module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: aliyun-python-sdk-eci
         This is the eci module of Aliyun Python SDK.
```

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyun_python_sdk_eci.egg-info/PKG-INFO` & `aliyun-python-sdk-eci-1.2.5/aliyun_python_sdk_eci.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eci
-Version: 1.2.4
+Version: 1.2.5
 Summary: The eci module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: aliyun-python-sdk-eci
         This is the eci module of Aliyun Python SDK.
```

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyun_python_sdk_eci.egg-info/SOURCES.txt` & `aliyun-python-sdk-eci-1.2.5/aliyun_python_sdk_eci.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,32 @@
 aliyun_python_sdk_eci.egg-info/SOURCES.txt
 aliyun_python_sdk_eci.egg-info/dependency_links.txt
 aliyun_python_sdk_eci.egg-info/requires.txt
 aliyun_python_sdk_eci.egg-info/top_level.txt
 aliyunsdkeci/__init__.py
 aliyunsdkeci/request/__init__.py
 aliyunsdkeci/request/v20180808/CommitContainerRequest.py
+aliyunsdkeci/request/v20180808/CopyDataCacheRequest.py
 aliyunsdkeci/request/v20180808/CreateContainerGroupRequest.py
+aliyunsdkeci/request/v20180808/CreateDataCacheRequest.py
 aliyunsdkeci/request/v20180808/CreateImageCacheRequest.py
 aliyunsdkeci/request/v20180808/DeleteContainerGroupRequest.py
 aliyunsdkeci/request/v20180808/DeleteContainerGroupsRequest.py
+aliyunsdkeci/request/v20180808/DeleteDataCacheRequest.py
 aliyunsdkeci/request/v20180808/DeleteImageCacheRequest.py
 aliyunsdkeci/request/v20180808/DescribeAvailableResourceRequest.py
 aliyunsdkeci/request/v20180808/DescribeCommitContainerTaskRequest.py
 aliyunsdkeci/request/v20180808/DescribeContainerGroupMetricRequest.py
 aliyunsdkeci/request/v20180808/DescribeContainerGroupPriceRequest.py
 aliyunsdkeci/request/v20180808/DescribeContainerGroupsRequest.py
 aliyunsdkeci/request/v20180808/DescribeContainerLogRequest.py
+aliyunsdkeci/request/v20180808/DescribeDataCachesRequest.py
 aliyunsdkeci/request/v20180808/DescribeImageCachesRequest.py
 aliyunsdkeci/request/v20180808/DescribeMultiContainerGroupMetricRequest.py
 aliyunsdkeci/request/v20180808/DescribeRegionsRequest.py
 aliyunsdkeci/request/v20180808/ExecContainerCommandRequest.py
 aliyunsdkeci/request/v20180808/ListUsageRequest.py
 aliyunsdkeci/request/v20180808/RestartContainerGroupRequest.py
 aliyunsdkeci/request/v20180808/UpdateContainerGroupRequest.py
+aliyunsdkeci/request/v20180808/UpdateDataCacheRequest.py
 aliyunsdkeci/request/v20180808/UpdateImageCacheRequest.py
 aliyunsdkeci/request/v20180808/__init__.py
```

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/CommitContainerRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/CommitContainerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/CreateContainerGroupRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/CreateContainerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/CreateImageCacheRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/CreateImageCacheRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DeleteContainerGroupRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DeleteContainerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DeleteContainerGroupsRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DeleteContainerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DeleteImageCacheRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DeleteImageCacheRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeAvailableResourceRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeAvailableResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeCommitContainerTaskRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeCommitContainerTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeContainerGroupMetricRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeContainerGroupMetricRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeContainerGroupPriceRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeContainerGroupPriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeContainerGroupsRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeContainerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeContainerLogRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeContainerLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeImageCachesRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeImageCachesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeMultiContainerGroupMetricRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeMultiContainerGroupMetricRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/DescribeRegionsRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/ExecContainerCommandRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/ExecContainerCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/ListUsageRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/ListUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/RestartContainerGroupRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/RestartContainerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/UpdateContainerGroupRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/UpdateContainerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/aliyunsdkeci/request/v20180808/UpdateImageCacheRequest.py` & `aliyun-python-sdk-eci-1.2.5/aliyunsdkeci/request/v20180808/UpdateImageCacheRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eci-1.2.4/setup.py` & `aliyun-python-sdk-eci-1.2.5/setup.py`

 * *Files identical despite different names*

