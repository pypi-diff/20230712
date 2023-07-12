# Comparing `tmp/alibabacloud_ha3engine-1.3.4.tar.gz` & `tmp/alibabacloud_ha3engine-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ha3engine-1.3.4.tar", last modified: Tue Jun  6 11:03:40 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ha3engine-1.3.5.tar", last modified: Wed Jul 12 09:33:04 2023, max compression
```

## Comparing `alibabacloud_ha3engine-1.3.4.tar` & `alibabacloud_ha3engine-1.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/
--rw-r--r--   0 root         (0) root         (0)      888 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37206 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/client.py
--rw-r--r--   0 root         (0) root         (0)    23930 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/
--rw-r--r--   0 root         (0) root         (0)      888 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2608 2023-06-06 11:03:40.000000 alibabacloud_ha3engine-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:33:04.000000 alibabacloud_ha3engine-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)      888 2023-07-12 09:33:04.000000 alibabacloud_ha3engine-1.3.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:33:04.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 09:33:03.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38862 2023-07-12 09:33:03.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine/client.py
+-rw-r--r--   0 root         (0) root         (0)    23930 2023-07-12 09:33:03.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:33:04.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      888 2023-07-12 09:33:03.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2023-07-12 09:33:03.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:33:03.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      170 2023-07-12 09:33:03.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-12 09:33:03.000000 alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 09:33:04.000000 alibabacloud_ha3engine-1.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-07-12 09:33:03.000000 alibabacloud_ha3engine-1.3.5/setup.py
```

### Comparing `alibabacloud_ha3engine-1.3.4/PKG-INFO` & `alibabacloud_ha3engine-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ha3engine
-Version: 1.3.4
+Version: 1.3.5
 Summary: Alibaba Cloud Ha3engine SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-ha3-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,ha3engine
```

### Comparing `alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/client.py` & `alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -790,14 +790,56 @@
             'X-Opensearch-Swift-PK-Field': key_field
         }
         return TeaCore.from_map(
             ha_3engine_models.PushDocumentsResponseModel(),
             await self._request_async('POST', f'/update/{data_source_name}/actions/bulk', None, request.headers, request.body, await self.build_runtime_options_async())
         )
 
+    def push_documents_with_swift(
+        self,
+        data_source_name: str,
+        key_field: str,
+        topic: str,
+        swift: str,
+        request: ha_3engine_models.PushDocumentsRequestModel,
+    ) -> ha_3engine_models.PushDocumentsResponseModel:
+        """
+        用于内网环境的新增、更新、删除 等操作，以及对应批量操作
+        """
+        request.headers = {
+            'X-Opensearch-Swift-PK-Field': key_field,
+            'X-Opensearch-Swift-Topic': topic,
+            'X-Opensearch-Swift-Swift': swift
+        }
+        return TeaCore.from_map(
+            ha_3engine_models.PushDocumentsResponseModel(),
+            self._request('POST', f'/update/{data_source_name}/actions/bulk', None, request.headers, request.body, self.build_runtime_options())
+        )
+
+    async def push_documents_with_swift_async(
+        self,
+        data_source_name: str,
+        key_field: str,
+        topic: str,
+        swift: str,
+        request: ha_3engine_models.PushDocumentsRequestModel,
+    ) -> ha_3engine_models.PushDocumentsResponseModel:
+        """
+        用于内网环境的新增、更新、删除 等操作，以及对应批量操作
+        """
+        request.headers = {
+            'X-Opensearch-Swift-PK-Field': key_field,
+            'X-Opensearch-Swift-Topic': topic,
+            'X-Opensearch-Swift-Swift': swift
+        }
+        return TeaCore.from_map(
+            ha_3engine_models.PushDocumentsResponseModel(),
+            await self._request_async('POST', f'/update/{data_source_name}/actions/bulk', None, request.headers, request.body, await self.build_runtime_options_async())
+        )
+
     def build_runtime_options(self) -> util_models.RuntimeOptions:
         """
         构建RuntimeOptions
         """
         return util_models.RuntimeOptions(
             connect_timeout=5000,
             read_timeout=10000,
```

### Comparing `alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine/models.py` & `alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ha3engine-1.3.4/alibabacloud_ha3engine.egg-info/PKG-INFO` & `alibabacloud_ha3engine-1.3.5/alibabacloud_ha3engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ha3engine
-Version: 1.3.4
+Version: 1.3.5
 Summary: Alibaba Cloud Ha3engine SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-ha3-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,ha3engine
```

### Comparing `alibabacloud_ha3engine-1.3.4/setup.py` & `alibabacloud_ha3engine-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ha3engine.
 
-Created on 06/06/2023
+Created on 12/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ha3engine"
 NAME = "alibabacloud_ha3engine" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Ha3engine SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-ha3-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_darabonba_string>=0.0.4, <1.0.0",
     "alibabacloud_darabonba_encode_util>=0.0.2, <1.0.0",
     "alibabacloud_darabonba_map>=0.0.1, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

