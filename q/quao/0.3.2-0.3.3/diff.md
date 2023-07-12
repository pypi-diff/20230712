# Comparing `tmp/quao-0.3.2.tar.gz` & `tmp/quao-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.3.2.tar", last modified: Wed Jul 12 04:00:34 2023, max compression
+gzip compressed data, was "quao-0.3.3.tar", last modified: Wed Jul 12 04:05:12 2023, max compression
```

## Comparing `quao-0.3.2.tar` & `quao-0.3.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:34.021014 quao-0.3.2/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-07-12 04:00:34.020019 quao-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.3.2/README.md
--rw-rw-rw-   0        0        0      967 2023-07-12 04:00:18.000000 quao-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 04:00:34.021014 quao-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:33.961823 quao-0.3.2/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:33.965825 quao-0.3.2/src/quao/
--rw-rw-rw-   0        0        0      203 2023-07-12 04:00:18.000000 quao-0.3.2/src/quao/__init__.py
--rw-rw-rw-   0        0        0     7514 2023-07-12 03:59:49.000000 quao-0.3.2/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:33.989017 quao-0.3.2/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.2/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      237 2023-06-29 09:59:18.000000 quao-0.3.2/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:33.990015 quao-0.3.2/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:33.991016 quao-0.3.2/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      971 2023-07-12 01:46:07.000000 quao-0.3.2/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:33.993014 quao-0.3.2/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      680 2023-06-22 02:52:41.000000 quao-0.3.2/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:34.002017 quao-0.3.2/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      185 2023-06-22 02:52:41.000000 quao-0.3.2/src/quao/enum/http_header.py
--rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.3.2/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.3.2/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/enum/sdk.py
--rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.3.2/src/quao/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:34.004017 quao-0.3.2/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.3.2/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.3.2/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:34.004017 quao-0.3.2/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:34.010033 quao-0.3.2/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     2313 2023-07-12 01:46:07.000000 quao-0.3.2/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3422 2023-07-12 01:46:07.000000 quao-0.3.2/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1008 2023-07-07 07:51:32.000000 quao-0.3.2/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      874 2023-07-12 03:59:19.000000 quao-0.3.2/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0     1158 2023-07-12 03:03:44.000000 quao-0.3.2/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     3268 2023-07-12 03:05:28.000000 quao-0.3.2/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:34.012015 quao-0.3.2/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     3262 2023-07-12 01:46:07.000000 quao-0.3.2/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:34.017018 quao-0.3.2/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.3.2/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.3.2/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.3.2/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.3.2/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.3.2/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:34.019018 quao-0.3.2/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.2/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.3.2/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1631 2023-07-12 01:46:07.000000 quao-0.3.2/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:00:33.987014 quao-0.3.2/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-07-12 04:00:33.000000 quao-0.3.2/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1537 2023-07-12 04:00:33.000000 quao-0.3.2/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 04:00:33.000000 quao-0.3.2/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      201 2023-07-12 04:00:33.000000 quao-0.3.2/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-12 04:00:33.000000 quao-0.3.2/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.131163 quao-0.3.3/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-07-12 04:05:12.130162 quao-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.3.3/README.md
+-rw-rw-rw-   0        0        0      967 2023-07-12 04:04:56.000000 quao-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 04:05:12.132169 quao-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.039159 quao-0.3.3/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.043162 quao-0.3.3/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-07-12 04:04:56.000000 quao-0.3.3/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     7544 2023-07-12 04:04:48.000000 quao-0.3.3/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.076161 quao-0.3.3/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.3/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.077159 quao-0.3.3/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.080162 quao-0.3.3/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.085162 quao-0.3.3/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-06-22 02:52:41.000000 quao-0.3.3/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.097160 quao-0.3.3/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-06-22 02:52:41.000000 quao-0.3.3/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.3.3/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/sdk.py
+-rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.3.3/src/quao/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.103162 quao-0.3.3/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.104161 quao-0.3.3/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.114160 quao-0.3.3/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     2313 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3422 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1008 2023-07-07 07:51:32.000000 quao-0.3.3/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      874 2023-07-12 03:59:19.000000 quao-0.3.3/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0     1192 2023-07-12 04:04:48.000000 quao-0.3.3/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     3268 2023-07-12 03:05:28.000000 quao-0.3.3/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.117169 quao-0.3.3/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     3262 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.125160 quao-0.3.3/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.128160 quao-0.3.3/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1631 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.070161 quao-0.3.3/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-07-12 04:05:11.000000 quao-0.3.3/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1537 2023-07-12 04:05:12.000000 quao-0.3.3/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 04:05:11.000000 quao-0.3.3/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      201 2023-07-12 04:05:11.000000 quao-0.3.3/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 04:05:11.000000 quao-0.3.3/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.3.2/LICENSE` & `quao-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/PKG-INFO` & `quao-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.3.2
+Version: 0.3.3
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.3.2/README.md` & `quao-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/pyproject.toml` & `quao-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.3.2"
+version = "0.3.3"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.3.2/src/quao/backend.py` & `quao-0.3.3/src/quao/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,30 +145,30 @@
         shots = self.shots
 
         if circuit and self.backend_data:
             device_name = self.backend_data.get("deviceName")
             provider_tag = self.backend_data.get("providerTag")
             authentication = self.backend_data.get("authentication")
 
-            # try:
-            logger.debug('Execute job with provider tag: {0}'.format(provider_tag))
-            provider = ProviderFactory().create_provider(provider_tag, authentication)
-
-            logger.debug('Execute job with device name: {0}'.format(device_name))
-            device = DeviceFactory().create_device(provider, device_name, authentication,
-                                                   self.sdk)
-
-            job_response = device.run_circuit(circuit=circuit, shots=shots)
-            job_response.user_identity = self.user_identity
-            job_response.user_token = self.user_token
+            try:
+                logger.debug('Execute job with provider tag: {0}'.format(provider_tag))
+                provider = ProviderFactory().create_provider(provider_tag, authentication)
+
+                logger.debug('Execute job with device name: {0}'.format(device_name))
+                device = DeviceFactory().create_device(provider, device_name, authentication,
+                                                       self.sdk)
+
+                job_response = device.run_circuit(circuit=circuit, shots=shots)
+                job_response.user_identity = self.user_identity
+                job_response.user_token = self.user_token
 
-            return job_response
+                return job_response
 
-            # except Exception as exception:
-            #     error_job_response.job_result = {"error": str(exception)}
+            except Exception as exception:
+                error_job_response.job_result = {"error": str(exception)}
 
         elif self.backend_data is None:
             error_job_response.job_result = {"error": "Backend not found"}
 
         return error_job_response
 
     def __post_execute_job(self, circuit):
```

### Comparing `quao-0.3.2/src/quao/data/job/job_response.py` & `quao-0.3.3/src/quao/data/job/job_response.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/data/request/request_data.py` & `quao-0.3.3/src/quao/data/request/request_data.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/factory/device_factory.py` & `quao-0.3.3/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/factory/provider_factory.py` & `quao-0.3.3/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/device/aws_braket_device.py` & `quao-0.3.3/src/quao/model/device/aws_braket_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/device/device.py` & `quao-0.3.3/src/quao/model/device/device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/device/ibm_cloud_device.py` & `quao-0.3.3/src/quao/model/device/ibm_cloud_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/device/ibm_quantum_device.py` & `quao-0.3.3/src/quao/model/device/ibm_quantum_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/device/qiskit_device.py` & `quao-0.3.3/src/quao/model/device/qiskit_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     def _get_job_status(self, job) -> str:
         return job.status().name
 
     def _get_name(self) -> str:
         return str(self.device.configuration().backend_name)
 
     def _get_execution_time(self, job_result):
+        logger.debug(job_result)
         metadata = job_result['metadata']
 
         if metadata is None or not bool(metadata):
             return self.execution_time
 
         self.execution_time = metadata['time_taken_execute']
```

### Comparing `quao-0.3.2/src/quao/model/device/quao_device.py` & `quao-0.3.3/src/quao/model/device/quao_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/job/qiskit_status.py` & `quao-0.3.3/src/quao/model/job/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/provider/aws_braket_provider.py` & `quao-0.3.3/src/quao/model/provider/aws_braket_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.3.3/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.3.3/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/provider/provider.py` & `quao-0.3.3/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/model/provider/quao_provider.py` & `quao-0.3.3/src/quao/model/provider/quao_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/util/json_parser_util.py` & `quao-0.3.3/src/quao/util/json_parser_util.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao/util/response_utils.py` & `quao-0.3.3/src/quao/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.2/src/quao.egg-info/PKG-INFO` & `quao-0.3.3/src/quao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.3.2
+Version: 0.3.3
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.3.2/src/quao.egg-info/SOURCES.txt` & `quao-0.3.3/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

