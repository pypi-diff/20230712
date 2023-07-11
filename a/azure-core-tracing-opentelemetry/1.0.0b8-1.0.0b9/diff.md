# Comparing `tmp/azure-core-tracing-opentelemetry-1.0.0b8.zip` & `tmp/azure-core-tracing-opentelemetry-1.0.0b9.zip`

## zipinfo {}

```diff
@@ -1,35 +1,36 @@
-Zip file size: 22295 bytes, number of entries: 33
-drwxr-xr-x  2.0 unx        0 b- stor 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/samples/
--rw-r--r--  2.0 unx       67 b- defN 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/setup.cfg
--rw-r--r--  2.0 unx     6706 b- defN 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/PKG-INFO
--rw-r--r--  2.0 unx     2462 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/setup.py
--rw-r--r--  2.0 unx      213 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/MANIFEST.in
--rw-r--r--  2.0 unx      712 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/CHANGELOG.md
--rw-r--r--  2.0 unx     3910 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/README.md
--rw-r--r--  2.0 unx      384 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/tests/conftest.py
--rw-r--r--  2.0 unx      731 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/tests/test_threading.py
--rw-r--r--  2.0 unx     8915 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/tests/test_tracing_implementations.py
--rw-r--r--  2.0 unx     6706 b- defN 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       83 b- defN 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/requires.txt
--rw-r--r--  2.0 unx      765 b- defN 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        6 b- defN 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/not-zip-safe
-drwxr-xr-x  2.0 unx        0 b- stor 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure/core/
--rw-r--r--  2.0 unx       81 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/azure/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/
--rw-r--r--  2.0 unx       81 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/azure/core/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/
--rw-r--r--  2.0 unx       81 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Feb-08 18:49 azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/opentelemetry_span/
--rw-r--r--  2.0 unx       81 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/__init__.py
--rw-r--r--  2.0 unx     9489 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/opentelemetry_span/__init__.py
--rw-r--r--  2.0 unx      172 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/opentelemetry_span/_version.py
--rw-r--r--  2.0 unx     2286 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/samples/sample_servicebus.py
--rw-r--r--  2.0 unx     2122 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/samples/sample_eventgrid.py
--rw-r--r--  2.0 unx     2010 b- defN 21-Feb-08 18:47 azure-core-tracing-opentelemetry-1.0.0b8/samples/sample_storage.py
-33 files, 48065 bytes uncompressed, 15243 bytes compressed:  68.3%
+Zip file size: 23811 bytes, number of entries: 34
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/samples/
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure/
+-rw-r--r--  2.0 unx     2324 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/setup.py
+-rw-r--r--  2.0 unx     6736 b- defN 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/PKG-INFO
+-rw-r--r--  2.0 unx      213 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/MANIFEST.in
+-rw-r--r--  2.0 unx       67 b- defN 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/setup.cfg
+-rw-r--r--  2.0 unx      858 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/CHANGELOG.md
+-rw-r--r--  2.0 unx     3910 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/README.md
+-rw-r--r--  2.0 unx     1998 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_storage.py
+-rw-r--r--  2.0 unx     2274 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_servicebus.py
+-rw-r--r--  2.0 unx     2110 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_eventgrid.py
+-rw-r--r--  2.0 unx     2122 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_receive_sb.py
+-rw-r--r--  2.0 unx      731 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/tests/test_threading.py
+-rw-r--r--  2.0 unx     8915 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/tests/test_tracing_implementations.py
+-rw-r--r--  2.0 unx      384 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/tests/conftest.py
+-rw-r--r--  2.0 unx       90 b- defN 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/requires.txt
+-rw-r--r--  2.0 unx      794 b- defN 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        6 b- defN 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     6736 b- defN 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx        1 b- defN 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure/core/
+-rw-r--r--  2.0 unx       81 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/azure/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/
+-rw-r--r--  2.0 unx       81 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/azure/core/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/
+-rw-r--r--  2.0 unx       81 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-07 04:19 azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/opentelemetry_span/
+-rw-r--r--  2.0 unx       81 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/__init__.py
+-rw-r--r--  2.0 unx      172 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/opentelemetry_span/_version.py
+-rw-r--r--  2.0 unx    11365 b- defN 21-Apr-07 04:17 azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/opentelemetry_span/__init__.py
+34 files, 52131 bytes uncompressed, 16545 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -1,100 +1,103 @@
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/tests/
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/samples/
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/tests/
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/samples/
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/setup.cfg
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/setup.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/PKG-INFO
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/PKG-INFO
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/setup.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/MANIFEST.in
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/MANIFEST.in
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/setup.cfg
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/CHANGELOG.md
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/CHANGELOG.md
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/README.md
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/README.md
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/tests/conftest.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_storage.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/tests/test_threading.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_servicebus.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/tests/test_tracing_implementations.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_eventgrid.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/PKG-INFO
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_receive_sb.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/requires.txt
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/tests/test_threading.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/SOURCES.txt
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/tests/test_tracing_implementations.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/top_level.txt
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/tests/conftest.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/dependency_links.txt
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/requires.txt
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/not-zip-safe
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/core/
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/__init__.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/core/__init__.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/core/
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/__init__.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/__init__.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/opentelemetry_span/
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/__init__.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/core/__init__.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/opentelemetry_span/__init__.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/opentelemetry_span/_version.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/__init__.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/samples/sample_servicebus.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/opentelemetry_span/
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/samples/sample_eventgrid.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/__init__.py
 Comment: 
 
-Filename: azure-core-tracing-opentelemetry-1.0.0b8/samples/sample_storage.py
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/opentelemetry_span/_version.py
+Comment: 
+
+Filename: azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/opentelemetry_span/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/PKG-INFO` & `azure-core-tracing-opentelemetry-1.0.0b9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-core-tracing-opentelemetry
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: Microsoft Azure Azure Core OpenTelemetry plugin Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/core/azure-core-tracing-opentelemetry
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: 
         
@@ -98,17 +98,21 @@
         This project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.microsoft.com.
         
         When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
         
         This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
         
         
-        
         # Release History
         
+        ## 1.0.0b9 (2021-04-06)
+        
+        - Updated opentelemetry-api to version 1.0.0
+        - `Link` and `SpanKind` can now be added while creating the span instance.
+        
         ## 1.0.0b8 (2021-02-08)
         
         - Pinned opentelemetry-api to version 0.17b0
         
         ## 1.0.0b7 (2020-10-05)
         
         - Pinned opentelemetry-api to version 0.13b0
@@ -134,27 +138,24 @@
         
         ## 1.0.0b2 (2020-03-09)
         
         ### Features
         
         - Pinned opentelemetry-api to version 0.4a0
         
-        ## 1.0.0b1
+        ## 1.0.0b1 
         
         ### Features
         
         - Opentelemetry implementation of azure-core tracing protocol
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.5.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/setup.py` & `azure-core-tracing-opentelemetry-1.0.0b9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,30 +39,27 @@
     license='MIT License',
     author='Microsoft Corporation',
     author_email='azpysdkhelp@microsoft.com',
     url='https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/core/azure-core-tracing-opentelemetry',
     classifiers=[
         "Development Status :: 4 - Beta",
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: MIT License',
     ],
     zip_safe=False,
     packages=[
         'azure.core.tracing.ext.opentelemetry_span',
     ],
-    python_requires=">=3.5.0",
+    python_requires=">=3.6.0",
     install_requires=[
-        'opentelemetry-api==0.17b0',
-        'azure-core<2.0.0,>=1.0.0',
+        'opentelemetry-api<2.0.0,>=1.0.0',
+        'azure-core<2.0.0,>=1.13.0',
     ],
     extras_require={
         ":python_version<'3.5'": ['typing'],
     }
 )
```

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/CHANGELOG.md` & `azure-core-tracing-opentelemetry-1.0.0b9/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-
 # Release History
 
+## 1.0.0b9 (2021-04-06)
+
+- Updated opentelemetry-api to version 1.0.0
+- `Link` and `SpanKind` can now be added while creating the span instance.
+
 ## 1.0.0b8 (2021-02-08)
 
 - Pinned opentelemetry-api to version 0.17b0
 
 ## 1.0.0b7 (2020-10-05)
 
 - Pinned opentelemetry-api to version 0.13b0
@@ -30,12 +34,12 @@
 
 ## 1.0.0b2 (2020-03-09)
 
 ### Features
 
 - Pinned opentelemetry-api to version 0.4a0
 
-## 1.0.0b1
+## 1.0.0b1 
 
 ### Features
 
 - Opentelemetry implementation of azure-core tracing protocol
```

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/README.md` & `azure-core-tracing-opentelemetry-1.0.0b9/README.md`

 * *Files identical despite different names*

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/tests/test_threading.py` & `azure-core-tracing-opentelemetry-1.0.0b9/tests/test_threading.py`

 * *Files identical despite different names*

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/tests/test_tracing_implementations.py` & `azure-core-tracing-opentelemetry-1.0.0b9/tests/test_tracing_implementations.py`

 * *Files identical despite different names*

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/PKG-INFO` & `azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-core-tracing-opentelemetry
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: Microsoft Azure Azure Core OpenTelemetry plugin Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/core/azure-core-tracing-opentelemetry
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: 
         
@@ -98,17 +98,21 @@
         This project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.microsoft.com.
         
         When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
         
         This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
         
         
-        
         # Release History
         
+        ## 1.0.0b9 (2021-04-06)
+        
+        - Updated opentelemetry-api to version 1.0.0
+        - `Link` and `SpanKind` can now be added while creating the span instance.
+        
         ## 1.0.0b8 (2021-02-08)
         
         - Pinned opentelemetry-api to version 0.17b0
         
         ## 1.0.0b7 (2020-10-05)
         
         - Pinned opentelemetry-api to version 0.13b0
@@ -134,27 +138,24 @@
         
         ## 1.0.0b2 (2020-03-09)
         
         ### Features
         
         - Pinned opentelemetry-api to version 0.4a0
         
-        ## 1.0.0b1
+        ## 1.0.0b1 
         
         ### Features
         
         - Opentelemetry implementation of azure-core tracing protocol
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.5.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/azure_core_tracing_opentelemetry.egg-info/SOURCES.txt` & `azure-core-tracing-opentelemetry-1.0.0b9/azure_core_tracing_opentelemetry.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 azure_core_tracing_opentelemetry.egg-info/PKG-INFO
 azure_core_tracing_opentelemetry.egg-info/SOURCES.txt
 azure_core_tracing_opentelemetry.egg-info/dependency_links.txt
 azure_core_tracing_opentelemetry.egg-info/not-zip-safe
 azure_core_tracing_opentelemetry.egg-info/requires.txt
 azure_core_tracing_opentelemetry.egg-info/top_level.txt
 samples/sample_eventgrid.py
+samples/sample_receive_sb.py
 samples/sample_servicebus.py
 samples/sample_storage.py
 tests/conftest.py
 tests/test_threading.py
 tests/test_tracing_implementations.py
```

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/azure/core/tracing/ext/opentelemetry_span/__init__.py` & `azure-core-tracing-opentelemetry-1.0.0b9/azure/core/tracing/ext/opentelemetry_span/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 """Implements azure.core.tracing.AbstractSpan to wrap OpenTelemetry spans."""
 
+import warnings
 from opentelemetry import trace
-from opentelemetry.trace import Span, Link, Tracer, SpanKind as OpenTelemetrySpanKind
+from opentelemetry.trace import Span, Tracer, SpanKind as OpenTelemetrySpanKind, Link as OpenTelemetryLink
 from opentelemetry.context import attach, detach, get_current
-from opentelemetry.propagators import extract, inject
+from opentelemetry.propagate import extract, inject
 from opentelemetry.trace.propagation import get_current_span as get_span_from_context
-from opentelemetry.trace.propagation.textmap import DictGetter
 
 from azure.core.tracing import SpanKind, HttpSpanMixin  # pylint: disable=no-name-in-module
 
 from ._version import VERSION
 
 try:
     from typing import TYPE_CHECKING, ContextManager
 except ImportError:
     TYPE_CHECKING = False
 
 if TYPE_CHECKING:
-    from typing import Any, Mapping, MutableMapping, Dict, Optional, Union, Callable, Sequence
+    from typing import Any, Mapping, Dict, Optional, Union, Callable, Sequence
 
     from azure.core.pipeline.transport import HttpRequest, HttpResponse
     AttributeValue = Union[
         str,
         bool,
         int,
         float,
@@ -35,64 +35,80 @@
         Sequence[float],
     ]
     Attributes = Optional[Dict[str, AttributeValue]]
 
 __version__ = VERSION
 
 
-def _get_headers_from_http_request_headers(headers: "Mapping[str, Any]", key: str):
-    """Return headers that matches this key.
-
-    Must comply to opentelemetry.context.propagation.httptextformat.Getter:
-    Getter = typing.Callable[[_T, str], typing.List[str]]
-    """
-    return [headers.get(key, "")]
-
-
-def _set_headers_from_http_request_headers(headers: "MutableMapping[str, Any]", key: str, value: str):
-    """Set headers in the given headers dict.
-
-    Must comply to opentelemetry.context.propagation.httptextformat.Setter:
-    Setter = typing.Callable[[_T, str, str], None]
-    """
-    headers[key] = value
-
-
 class OpenTelemetrySpan(HttpSpanMixin, object):
     """OpenTelemetry plugin for Azure client libraries.
 
     :param span: The OpenTelemetry span to wrap, or nothing to create a new one.
     :type span: ~OpenTelemetry.trace.Span
     :param name: The name of the OpenTelemetry span to create if a new span is needed
     :type name: str
+    :keyword SpanKind kind: The span kind of this span.
+    :keyword links: The list of links to be added to the span.
+    :paramtype links: list[~azure.core.tracing.Link]
     """
 
-    def __init__(self, span=None, name="span"):
-        # type: (Optional[Span], Optional[str]) -> None
+    def __init__(self, span=None, name="span", **kwargs):
+        # type: (Optional[Span], Optional[str], Any) -> None
         current_tracer = self.get_current_tracer()
-        self._span_instance = span or current_tracer.start_span(name=name)
+
+        ## kind
+        value = kwargs.pop('kind', None)
+        kind = (
+            OpenTelemetrySpanKind.CLIENT if value == SpanKind.CLIENT else
+            OpenTelemetrySpanKind.PRODUCER if value == SpanKind.PRODUCER else
+            OpenTelemetrySpanKind.SERVER if value == SpanKind.SERVER else
+            OpenTelemetrySpanKind.CONSUMER if value == SpanKind.CONSUMER else
+            OpenTelemetrySpanKind.INTERNAL if value == SpanKind.INTERNAL else
+            OpenTelemetrySpanKind.INTERNAL if value == SpanKind.UNSPECIFIED else
+            None
+        ) # type: SpanKind
+        if value and kind is None:
+            raise ValueError("Kind {} is not supported in OpenTelemetry".format(value))
+
+        links = kwargs.pop('links', None)
+        if links:
+            try:
+                ot_links = []
+                for link in links:
+                    ctx = extract(link.headers)
+                    span_ctx = get_span_from_context(ctx).get_span_context()
+                    ot_links.append(OpenTelemetryLink(span_ctx, link.attributes))
+                kwargs.setdefault('links', ot_links)
+            except AttributeError:
+                # we will just send the links as is if it's not ~azure.core.tracing.Link without any validation
+                # assuming user knows what they are doing.
+                kwargs.setdefault('links', links)
+        self._span_instance = span or current_tracer.start_span(name=name, kind=kind, **kwargs)
         self._current_ctxt_manager = None
 
     @property
     def span_instance(self):
         # type: () -> Span
         """
         :return: The OpenTelemetry span that is being wrapped.
         """
         return self._span_instance
 
-    def span(self, name="span"):
-        # type: (Optional[str]) -> OpenTelemetrySpan
+    def span(self, name="span", **kwargs):
+        # type: (Optional[str], Any) -> OpenTelemetrySpan
         """
         Create a child span for the current span and append it to the child spans list in the span instance.
         :param name: Name of the child span
         :type name: str
+        :keyword SpanKind kind: The span kind of this span.
+        :keyword links: The list of links to be added to the span.
+        :paramtype links: list[Link]
         :return: The OpenTelemetrySpan that is wrapping the child span instance
         """
-        return self.__class__(name=name)
+        return self.__class__(name=name, **kwargs)
 
     @property
     def kind(self):
         # type: () -> Optional[SpanKind]
         """Get the span kind of this span."""
         value = self.span_instance.kind
         return (
@@ -116,26 +132,33 @@
             OpenTelemetrySpanKind.CONSUMER if value == SpanKind.CONSUMER else
             OpenTelemetrySpanKind.INTERNAL if value == SpanKind.INTERNAL else
             OpenTelemetrySpanKind.INTERNAL if value == SpanKind.UNSPECIFIED else
             None
         )
         if kind is None:
             raise ValueError("Kind {} is not supported in OpenTelemetry".format(value))
-        self.span_instance.kind = kind
+        try:
+            self._span_instance._kind = kind # pylint: disable=protected-access
+        except AttributeError:
+            warnings.warn(
+                """Kind must be set while creating the span for Opentelemetry. It might be possible
+                that one of the packages you are using doesn't follow the latest Opentelemtry Spec.
+                Try updating the azure packages to the latest versions."""
+            )
 
     def __enter__(self):
         """Start a span."""
-        self._current_ctxt_manager = self.get_current_tracer().use_span(self._span_instance, end_on_exit=True)
-        self._current_ctxt_manager.__enter__()
+        self._current_ctxt_manager = trace.use_span(self._span_instance, end_on_exit=True)
+        self._current_ctxt_manager.__enter__() # pylint: disable=no-member
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
         """Finish a span."""
         if self._current_ctxt_manager:
-            self._current_ctxt_manager.__exit__(exception_type, exception_value, traceback)
+            self._current_ctxt_manager.__exit__(exception_type, exception_value, traceback) # pylint: disable=no-member
             self._current_ctxt_manager = None
 
     def start(self):
         # Spans are automatically started at their creation with OpenTelemetry
         pass
 
     def finish(self):
@@ -146,15 +169,15 @@
     def to_header(self): # pylint: disable=no-self-use
         # type: () -> Dict[str, str]
         """
         Returns a dictionary with the header labels and values.
         :return: A key value pair dictionary
         """
         temp_headers = {} # type: Dict[str, str]
-        inject(_set_headers_from_http_request_headers, temp_headers)
+        inject(temp_headers)
         return temp_headers
 
     def add_attribute(self, key, value):
         # type: (str, Union[str, int]) -> None
         """
         Add attribute (key value pair) to the current span.
 
@@ -199,18 +222,25 @@
         # type: (Dict[str, str], Attributes) -> None
         """
         Given a dictionary, extracts the context and links the context to the current tracer.
 
         :param headers: A key value pair dictionary
         :type headers: dict
         """
-        ctx = extract(DictGetter(), headers)
+        ctx = extract(headers)
         span_ctx = get_span_from_context(ctx).get_span_context()
         current_span = cls.get_current_span()
-        current_span.links.append(Link(span_ctx, attributes))
+        try:
+            current_span._links.append(OpenTelemetryLink(span_ctx, attributes)) # pylint: disable=protected-access
+        except AttributeError:
+            warnings.warn(
+                """Link must be added while creating the span for Opentelemetry. It might be possible
+                that one of the packages you are using doesn't follow the latest Opentelemtry Spec.
+                Try updating the azure packages to the latest versions."""
+            )
 
     @classmethod
     def get_current_span(cls):
         # type: () -> Span
         """
         Get the current span from the execution context. Return None otherwise.
         """
@@ -225,15 +255,15 @@
         return trace.get_tracer(__name__, __version__)
 
     @classmethod
     def change_context(cls, span):
         # type: (Span) -> ContextManager
         """Change the context for the life of this context manager.
         """
-        return cls.get_current_tracer().use_span(span, end_on_exit=False)
+        return trace.use_span(span, end_on_exit=False)
 
     @classmethod
     def set_current_span(cls, span):
         # type: (Span) -> None
         """Not supported by OpenTelemetry.
         """
         raise NotImplementedError(
```

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/samples/sample_servicebus.py` & `azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_servicebus.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 # )
 
 # Regular open telemetry usage from here, see https://github.com/open-telemetry/opentelemetry-python
 # for details
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter
-from opentelemetry.sdk.trace.export import SimpleExportSpanProcessor
+from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 
 # Simple console exporter
 exporter = ConsoleSpanExporter()
 
 trace.set_tracer_provider(TracerProvider())
 tracer = trace.get_tracer(__name__)
 trace.get_tracer_provider().add_span_processor(
-    SimpleExportSpanProcessor(exporter)
+    SimpleSpanProcessor(exporter)
 )
 
 # Example with Servicebus SDKs
 
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 import os
```

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/samples/sample_eventgrid.py` & `azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_eventgrid.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 # )
 
 # Regular open telemetry usage from here, see https://github.com/open-telemetry/opentelemetry-python
 # for details
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter
-from opentelemetry.sdk.trace.export import SimpleExportSpanProcessor
+from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 
 # Simple console exporter
 exporter = ConsoleSpanExporter()
 
 trace.set_tracer_provider(TracerProvider())
 tracer = trace.get_tracer(__name__)
 trace.get_tracer_provider().add_span_processor(
-    SimpleExportSpanProcessor(exporter)
+    SimpleSpanProcessor(exporter)
 )
 
 # Example with Eventgrid SDKs
 import os
 from azure.eventgrid import EventGridPublisherClient, CloudEvent
 from azure.core.credentials import AzureKeyCredential
```

## Comparing `azure-core-tracing-opentelemetry-1.0.0b8/samples/sample_storage.py` & `azure-core-tracing-opentelemetry-1.0.0b9/samples/sample_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 # )
 
 # Regular open telemetry usage from here, see https://github.com/open-telemetry/opentelemetry-python
 # for details
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter
-from opentelemetry.sdk.trace.export import SimpleExportSpanProcessor
+from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 
 # Simple console exporter
 exporter = ConsoleSpanExporter()
 
 trace.set_tracer_provider(TracerProvider())
 tracer = trace.get_tracer(__name__)
 trace.get_tracer_provider().add_span_processor(
-    SimpleExportSpanProcessor(exporter)
+    SimpleSpanProcessor(exporter)
 )
 
 # Example with Storage SDKs
 import os
 from azure.storage.blob import BlobServiceClient
 
 connection_string = os.environ['AZURE_STORAGE_CONNECTION_STRING']
```

