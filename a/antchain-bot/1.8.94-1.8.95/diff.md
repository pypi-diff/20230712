# Comparing `tmp/antchain_bot-1.8.94.tar.gz` & `tmp/antchain_bot-1.8.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_bot-1.8.94.tar", last modified: Tue Jul  4 06:40:46 2023, max compression
+gzip compressed data, was "dist/antchain_bot-1.8.95.tar", last modified: Wed Jul 12 02:45:03 2023, max compression
```

## Comparing `antchain_bot-1.8.94.tar` & `antchain_bot-1.8.95.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_sdk_bot/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/antchain_sdk_bot/__init__.py
--rw-r--r--   0 root         (0) root         (0)   444092 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/antchain_sdk_bot/client.py
--rw-r--r--   0 root         (0) root         (0)  1185996 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/antchain_sdk_bot/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_bot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_bot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_bot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_bot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_sdk_bot/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_sdk_bot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   444092 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_sdk_bot/client.py
+-rw-r--r--   0 root         (0) root         (0)  1185698 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/antchain_sdk_bot/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-07-12 02:45:03.000000 antchain_bot-1.8.95/setup.py
```

### Comparing `antchain_bot-1.8.94/LICENSE` & `antchain_bot-1.8.95/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.94/PKG-INFO` & `antchain_bot-1.8.95/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_bot
-Version: 1.8.94
+Version: 1.8.95
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.94/README-CN.md` & `antchain_bot-1.8.95/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.94/README.md` & `antchain_bot-1.8.95/README.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.94/antchain_bot.egg-info/PKG-INFO` & `antchain_bot-1.8.95/antchain_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-bot
-Version: 1.8.94
+Version: 1.8.95
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.94/antchain_sdk_bot/client.py` & `antchain_bot-1.8.95/antchain_sdk_bot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.94',
+                    'sdk_version': '1.8.95',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.94',
+                    'sdk_version': '1.8.95',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_bot-1.8.94/antchain_sdk_bot/models.py` & `antchain_bot-1.8.95/antchain_sdk_bot/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,81 +780,73 @@
             self.gateway_public_key = m.get('gateway_public_key')
         return self
 
 
 class QueryChainDataTransactionResultData(TeaModel):
     def __init__(
         self,
-        biz_id: str = None,
         biz_scene: str = None,
         data_scene: str = None,
         asset_id: str = None,
         tenant_id: str = None,
-        asset_data: str = None,
+        text_hash: str = None,
         timestamp: int = None,
     ):
-        # 业务ID
-        self.biz_id = biz_id
         # 所属业务
         self.biz_scene = biz_scene
         # 数据资产类型
         self.data_scene = data_scene
         # 资产ID
         self.asset_id = asset_id
         # 租户id
         self.tenant_id = tenant_id
-        # 资产数据
-        self.asset_data = asset_data
+        # 业务数据hash
+        self.text_hash = text_hash
         # 时间
         self.timestamp = timestamp
 
     def validate(self):
-        self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.biz_scene, 'biz_scene')
         self.validate_required(self.data_scene, 'data_scene')
         self.validate_required(self.asset_id, 'asset_id')
         self.validate_required(self.tenant_id, 'tenant_id')
-        self.validate_required(self.asset_data, 'asset_data')
+        self.validate_required(self.text_hash, 'text_hash')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.biz_id is not None:
-            result['biz_id'] = self.biz_id
         if self.biz_scene is not None:
             result['biz_scene'] = self.biz_scene
         if self.data_scene is not None:
             result['data_scene'] = self.data_scene
         if self.asset_id is not None:
             result['asset_id'] = self.asset_id
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
-        if self.asset_data is not None:
-            result['asset_data'] = self.asset_data
+        if self.text_hash is not None:
+            result['text_hash'] = self.text_hash
         if self.timestamp is not None:
             result['timestamp'] = self.timestamp
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('biz_id') is not None:
-            self.biz_id = m.get('biz_id')
         if m.get('biz_scene') is not None:
             self.biz_scene = m.get('biz_scene')
         if m.get('data_scene') is not None:
             self.data_scene = m.get('data_scene')
         if m.get('asset_id') is not None:
             self.asset_id = m.get('asset_id')
         if m.get('tenant_id') is not None:
             self.tenant_id = m.get('tenant_id')
-        if m.get('asset_data') is not None:
-            self.asset_data = m.get('asset_data')
+        if m.get('text_hash') is not None:
+            self.text_hash = m.get('text_hash')
         if m.get('timestamp') is not None:
             self.timestamp = m.get('timestamp')
         return self
 
 
 class BaiGoodsPointIdentificationResult(TeaModel):
     def __init__(
```

### Comparing `antchain_bot-1.8.94/setup.py` & `antchain_bot-1.8.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_bot.
 
-Created on 04/07/2023
+Created on 12/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_bot"
 NAME = "antchain_bot" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BOT SDK Library for Python"
```

