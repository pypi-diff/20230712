# Comparing `tmp/alibabacloud_alimt20181012_py2-1.1.0.tar.gz` & `tmp/alibabacloud_alimt20181012_py2-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alimt20181012_py2-1.1.0.tar", last modified: Tue Apr 11 09:30:26 2023, max compression
+gzip compressed data, was "dist/alibabacloud_alimt20181012_py2-1.1.1.tar", last modified: Wed Jul 12 08:59:39 2023, max compression
```

## Comparing `alibabacloud_alimt20181012_py2-1.1.0.tar` & `alibabacloud_alimt20181012_py2-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:30:26.000000 alibabacloud_alimt20181012_py2-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2498 2023-04-11 09:30:26.000000 alibabacloud_alimt20181012_py2-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:30:26.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38808 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012/client.py
--rw-r--r--   0 root         (0) root         (0)   105838 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:30:26.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2498 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 09:30:26.000000 alibabacloud_alimt20181012_py2-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3134 2023-04-11 09:30:25.000000 alibabacloud_alimt20181012_py2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39387 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012/client.py
+-rw-r--r--   0 root         (0) root         (0)   106462 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-07-12 08:59:39.000000 alibabacloud_alimt20181012_py2-1.1.1/setup.py
```

### Comparing `alibabacloud_alimt20181012_py2-1.1.0/LICENSE` & `alibabacloud_alimt20181012_py2-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012_py2-1.1.0/PKG-INFO` & `alibabacloud_alimt20181012_py2-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alimt20181012_py2
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012_py2-1.1.0/README-CN.md` & `alibabacloud_alimt20181012_py2-1.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012_py2-1.1.0/README.md` & `alibabacloud_alimt20181012_py2-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012/client.py` & `alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -763,14 +763,25 @@
             )
             oss_client.post_object(upload_request, oss_runtime)
             translate_certificate_req.image_url = 'http://%s.%s/%s' % (TeaConverter.to_unicode(auth_response.body.bucket), TeaConverter.to_unicode(auth_response.body.endpoint), TeaConverter.to_unicode(auth_response.body.object_key))
         translate_certificate_resp = self.translate_certificate_with_options(translate_certificate_req, runtime)
         return translate_certificate_resp
 
     def translate_ecommerce_with_options(self, request, runtime):
+        """
+        @deprecated : TranslateECommerce is deprecated, please use alimt::2018-10-12::Translate instead.
+        
+
+        @param request: TranslateECommerceRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
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
@@ -799,14 +810,23 @@
         )
         return TeaCore.from_map(
             alimt_20181012_models.TranslateECommerceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def translate_ecommerce(self, request):
+        """
+        @deprecated : TranslateECommerce is deprecated, please use alimt::2018-10-12::Translate instead.
+        
+
+        @param request: TranslateECommerceRequest
+
+        @return: TranslateECommerceResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return self.translate_ecommerce_with_options(request, runtime)
 
     def translate_general_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.context):
```

### Comparing `alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012/models.py` & `alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2035,35 +2035,40 @@
             self.source_text = m.get('SourceText')
         if m.get('TargetLanguage') is not None:
             self.target_language = m.get('TargetLanguage')
         return self
 
 
 class TranslateResponseBodyData(TeaModel):
-    def __init__(self, translated=None, word_count=None):
+    def __init__(self, detected_language=None, translated=None, word_count=None):
+        self.detected_language = detected_language  # type: str
         self.translated = translated  # type: str
         self.word_count = word_count  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(TranslateResponseBodyData, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('DetectedLanguage') is not None:
+            self.detected_language = m.get('DetectedLanguage')
         if m.get('Translated') is not None:
             self.translated = m.get('Translated')
         if m.get('WordCount') is not None:
             self.word_count = m.get('WordCount')
         return self
 
 
@@ -2584,35 +2589,40 @@
             self.source_text = m.get('SourceText')
         if m.get('TargetLanguage') is not None:
             self.target_language = m.get('TargetLanguage')
         return self
 
 
 class TranslateGeneralResponseBodyData(TeaModel):
-    def __init__(self, translated=None, word_count=None):
+    def __init__(self, detected_language=None, translated=None, word_count=None):
+        self.detected_language = detected_language  # type: str
         self.translated = translated  # type: str
         self.word_count = word_count  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(TranslateGeneralResponseBodyData, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('DetectedLanguage') is not None:
+            self.detected_language = m.get('DetectedLanguage')
         if m.get('Translated') is not None:
             self.translated = m.get('Translated')
         if m.get('WordCount') is not None:
             self.word_count = m.get('WordCount')
         return self
```

### Comparing `alibabacloud_alimt20181012_py2-1.1.0/alibabacloud_alimt20181012_py2.egg-info/PKG-INFO` & `alibabacloud_alimt20181012_py2-1.1.1/alibabacloud_alimt20181012_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alimt20181012-py2
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012_py2-1.1.0/setup.py` & `alibabacloud_alimt20181012_py2-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alimt20181012_py2.
 
-Created on 11/04/2023
+Created on 12/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alimt20181012"
 NAME = "alibabacloud_alimt20181012_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Machine Translation (20181012) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_oss_sdk_py2>=0.0.1, <1.0.0",
     "alibabacloud_openplatform20191219_py2>=1.0.0, <2.0.0",
     "alibabacloud_oss_util_py2>=0.0.1, <1.0.0",
     "alibabacloud_tea_fileform_py2>=0.0.1, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
```

