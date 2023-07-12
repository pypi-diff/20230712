# Comparing `tmp/alibabacloud_alimt20181012-1.1.0.tar.gz` & `tmp/alibabacloud_alimt20181012-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alimt20181012-1.1.0.tar", last modified: Tue Apr 11 09:30:16 2023, max compression
+gzip compressed data, was "dist/alibabacloud_alimt20181012-1.1.1.tar", last modified: Wed Jul 12 08:59:57 2023, max compression
```

## Comparing `alibabacloud_alimt20181012-1.1.0.tar` & `alibabacloud_alimt20181012-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      301 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85868 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/client.py
--rw-r--r--   0 root         (0) root         (0)   105220 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2825 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87016 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012/client.py
+-rw-r--r--   0 root         (0) root         (0)   105848 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-12 08:59:57.000000 alibabacloud_alimt20181012-1.1.1/setup.py
```

### Comparing `alibabacloud_alimt20181012-1.1.0/LICENSE` & `alibabacloud_alimt20181012-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.1.0/PKG-INFO` & `alibabacloud_alimt20181012-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alimt20181012
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012-1.1.0/README-CN.md` & `alibabacloud_alimt20181012-1.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.1.0/README.md` & `alibabacloud_alimt20181012-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/client.py` & `alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1689,14 +1689,22 @@
         return translate_certificate_resp
 
     def translate_ecommerce_with_options(
         self,
         request: alimt_20181012_models.TranslateECommerceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alimt_20181012_models.TranslateECommerceResponse:
+        """
+        @deprecated : TranslateECommerce is deprecated, please use alimt::2018-10-12::Translate instead.
+        
+        @param request: TranslateECommerceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TranslateECommerceResponse
+        Deprecated
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.context):
             query['Context'] = request.context
         body = {}
         if not UtilClient.is_unset(request.format_type):
             body['FormatType'] = request.format_type
@@ -1729,14 +1737,22 @@
         )
 
     async def translate_ecommerce_with_options_async(
         self,
         request: alimt_20181012_models.TranslateECommerceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alimt_20181012_models.TranslateECommerceResponse:
+        """
+        @deprecated : TranslateECommerce is deprecated, please use alimt::2018-10-12::Translate instead.
+        
+        @param request: TranslateECommerceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TranslateECommerceResponse
+        Deprecated
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.context):
             query['Context'] = request.context
         body = {}
         if not UtilClient.is_unset(request.format_type):
             body['FormatType'] = request.format_type
@@ -1768,21 +1784,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def translate_ecommerce(
         self,
         request: alimt_20181012_models.TranslateECommerceRequest,
     ) -> alimt_20181012_models.TranslateECommerceResponse:
+        """
+        @deprecated : TranslateECommerce is deprecated, please use alimt::2018-10-12::Translate instead.
+        
+        @param request: TranslateECommerceRequest
+        @return: TranslateECommerceResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return self.translate_ecommerce_with_options(request, runtime)
 
     async def translate_ecommerce_async(
         self,
         request: alimt_20181012_models.TranslateECommerceRequest,
     ) -> alimt_20181012_models.TranslateECommerceResponse:
+        """
+        @deprecated : TranslateECommerce is deprecated, please use alimt::2018-10-12::Translate instead.
+        
+        @param request: TranslateECommerceRequest
+        @return: TranslateECommerceResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return await self.translate_ecommerce_with_options_async(request, runtime)
 
     def translate_general_with_options(
         self,
         request: alimt_20181012_models.TranslateGeneralRequest,
         runtime: util_models.RuntimeOptions,
```

### Comparing `alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/models.py` & `alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2320,37 +2320,43 @@
             self.target_language = m.get('TargetLanguage')
         return self
 
 
 class TranslateResponseBodyData(TeaModel):
     def __init__(
         self,
+        detected_language: str = None,
         translated: str = None,
         word_count: str = None,
     ):
+        self.detected_language = detected_language
         self.translated = translated
         self.word_count = word_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.detected_language is not None:
+            result['DetectedLanguage'] = self.detected_language
         if self.translated is not None:
             result['Translated'] = self.translated
         if self.word_count is not None:
             result['WordCount'] = self.word_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('DetectedLanguage') is not None:
+            self.detected_language = m.get('DetectedLanguage')
         if m.get('Translated') is not None:
             self.translated = m.get('Translated')
         if m.get('WordCount') is not None:
             self.word_count = m.get('WordCount')
         return self
 
 
@@ -2943,37 +2949,43 @@
             self.target_language = m.get('TargetLanguage')
         return self
 
 
 class TranslateGeneralResponseBodyData(TeaModel):
     def __init__(
         self,
+        detected_language: str = None,
         translated: str = None,
         word_count: str = None,
     ):
+        self.detected_language = detected_language
         self.translated = translated
         self.word_count = word_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.detected_language is not None:
+            result['DetectedLanguage'] = self.detected_language
         if self.translated is not None:
             result['Translated'] = self.translated
         if self.word_count is not None:
             result['WordCount'] = self.word_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('DetectedLanguage') is not None:
+            self.detected_language = m.get('DetectedLanguage')
         if m.get('Translated') is not None:
             self.translated = m.get('Translated')
         if m.get('WordCount') is not None:
             self.word_count = m.get('WordCount')
         return self
```

### Comparing `alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/PKG-INFO` & `alibabacloud_alimt20181012-1.1.1/alibabacloud_alimt20181012.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alimt20181012
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012-1.1.0/setup.py` & `alibabacloud_alimt20181012-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alimt20181012.
 
-Created on 11/04/2023
+Created on 12/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alimt20181012"
 NAME = "alibabacloud_alimt20181012" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Machine Translation (20181012) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
```

