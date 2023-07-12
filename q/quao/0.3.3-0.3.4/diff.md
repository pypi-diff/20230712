# Comparing `tmp/quao-0.3.3.tar.gz` & `tmp/quao-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.3.3.tar", last modified: Wed Jul 12 04:05:12 2023, max compression
+gzip compressed data, was "quao-0.3.4.tar", last modified: Wed Jul 12 04:37:47 2023, max compression
```

## Comparing `quao-0.3.3.tar` & `quao-0.3.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.131163 quao-0.3.3/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-07-12 04:05:12.130162 quao-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.3.3/README.md
--rw-rw-rw-   0        0        0      967 2023-07-12 04:04:56.000000 quao-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 04:05:12.132169 quao-0.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.039159 quao-0.3.3/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.043162 quao-0.3.3/src/quao/
--rw-rw-rw-   0        0        0      203 2023-07-12 04:04:56.000000 quao-0.3.3/src/quao/__init__.py
--rw-rw-rw-   0        0        0     7544 2023-07-12 04:04:48.000000 quao-0.3.3/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.076161 quao-0.3.3/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.3/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      237 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.077159 quao-0.3.3/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.080162 quao-0.3.3/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      971 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.085162 quao-0.3.3/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      680 2023-06-22 02:52:41.000000 quao-0.3.3/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.097160 quao-0.3.3/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      185 2023-06-22 02:52:41.000000 quao-0.3.3/src/quao/enum/http_header.py
--rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.3.3/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/enum/sdk.py
--rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.3.3/src/quao/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.103162 quao-0.3.3/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.104161 quao-0.3.3/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.114160 quao-0.3.3/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     2313 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3422 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1008 2023-07-07 07:51:32.000000 quao-0.3.3/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      874 2023-07-12 03:59:19.000000 quao-0.3.3/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0     1192 2023-07-12 04:04:48.000000 quao-0.3.3/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     3268 2023-07-12 03:05:28.000000 quao-0.3.3/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.117169 quao-0.3.3/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     3262 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.125160 quao-0.3.3/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.3.3/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.128160 quao-0.3.3/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.3/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.3.3/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1631 2023-07-12 01:46:07.000000 quao-0.3.3/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 04:05:12.070161 quao-0.3.3/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-07-12 04:05:11.000000 quao-0.3.3/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1537 2023-07-12 04:05:12.000000 quao-0.3.3/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 04:05:11.000000 quao-0.3.3/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      201 2023-07-12 04:05:11.000000 quao-0.3.3/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-12 04:05:11.000000 quao-0.3.3/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.560077 quao-0.3.4/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-07-12 04:37:47.559074 quao-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.3.4/README.md
+-rw-rw-rw-   0        0        0      967 2023-07-12 04:36:49.000000 quao-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 04:37:47.560077 quao-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.504078 quao-0.3.4/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.506075 quao-0.3.4/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-07-12 04:36:49.000000 quao-0.3.4/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     7544 2023-07-12 04:04:48.000000 quao-0.3.4/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.527073 quao-0.3.4/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.4/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-06-29 09:59:18.000000 quao-0.3.4/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.528072 quao-0.3.4/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.530073 quao-0.3.4/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-07-12 01:46:07.000000 quao-0.3.4/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.532073 quao-0.3.4/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-06-22 02:52:41.000000 quao-0.3.4/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.541074 quao-0.3.4/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-06-22 02:52:41.000000 quao-0.3.4/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.3.4/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.3.4/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/enum/sdk.py
+-rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.3.4/src/quao/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.543073 quao-0.3.4/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.3.4/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.3.4/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.544073 quao-0.3.4/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.549074 quao-0.3.4/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     2541 2023-07-12 04:36:49.000000 quao-0.3.4/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3612 2023-07-12 04:28:24.000000 quao-0.3.4/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1008 2023-07-07 07:51:32.000000 quao-0.3.4/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      788 2023-07-12 04:24:43.000000 quao-0.3.4/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0     1170 2023-07-12 04:33:18.000000 quao-0.3.4/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     3337 2023-07-12 04:36:49.000000 quao-0.3.4/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.550073 quao-0.3.4/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     3938 2023-07-12 04:36:49.000000 quao-0.3.4/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.556073 quao-0.3.4/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.3.4/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.3.4/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.3.4/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.3.4/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.3.4/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.558075 quao-0.3.4/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.4/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.3.4/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1631 2023-07-12 01:46:07.000000 quao-0.3.4/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:37:47.526073 quao-0.3.4/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-07-12 04:37:47.000000 quao-0.3.4/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1537 2023-07-12 04:37:47.000000 quao-0.3.4/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 04:37:47.000000 quao-0.3.4/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      201 2023-07-12 04:37:47.000000 quao-0.3.4/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 04:37:47.000000 quao-0.3.4/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.3.3/LICENSE` & `quao-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/PKG-INFO` & `quao-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.3.3
+Version: 0.3.4
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.3.3/README.md` & `quao-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/pyproject.toml` & `quao-0.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.3.3"
+version = "0.3.4"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.3.3/src/quao/backend.py` & `quao-0.3.4/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/data/job/job_response.py` & `quao-0.3.4/src/quao/data/job/job_response.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/data/request/request_data.py` & `quao-0.3.4/src/quao/data/request/request_data.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/factory/device_factory.py` & `quao-0.3.4/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/factory/provider_factory.py` & `quao-0.3.4/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/model/device/aws_braket_device.py` & `quao-0.3.4/src/quao/model/device/aws_braket_device.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,18 +42,24 @@
         if JobStatus.COMPLETED.value.__eq__(job_state):
             job_state = JobStatus.DONE.value
         return job_state
 
     def _parse_job_result(self, job_result) -> dict:
         return JsonParserUtils.parse(job_result.__dict__)
 
-    def _get_execution_time(self, job_result):
+    def _calculate_execution_time(self, job_result):
+        if 'task_metadata' not in job_result:
+            return
+
         task_metadata = job_result['task_metadata']
 
-        if task_metadata is None:
+        if task_metadata is None \
+                or not bool(task_metadata)\
+                or 'createdAt' not in task_metadata \
+                or 'endedAt' not in task_metadata:
             return self.execution_time
 
         created_at = task_metadata['createdAt']
         ended_at = task_metadata['endedAt']
 
         if created_at is None or ended_at is None:
             return self.execution_time
```

### Comparing `quao-0.3.3/src/quao/model/device/device.py` & `quao-0.3.4/src/quao/model/device/device.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,32 +43,36 @@
 
                 content_type = MediaType.APPLICATION_JSON.value
 
                 logger.debug('Producing histogram ....')
                 job_histogram = self._produce_histogram_data(job_result)
                 logger.debug('Producing histogram completed!')
 
+                logger.debug('Calculating execution time ....')
+                self._calculate_execution_time(job_result_dictionary)
+                logger.debug('Execution time calculation was completed!')
+
         except Exception as exception:
             logger.debug('Exception when invoke job on device {0}: {1}'
-                          .format(self._get_name(), str(exception)))
+                         .format(self._get_name(), str(exception)))
 
             job_result_dictionary = {
                 "error": "Exception when invoke job on device: " + self._get_name(),
                 "exception": str(exception)
             }
 
             job_status = JobStatus.ERROR.value
 
         return JobResponse(
             provider_job_id=provider_job_id,
             job_status=job_status,
             job_result=job_result_dictionary,
             content_type=content_type,
             job_histogram=job_histogram,
-            execution_time=self._get_execution_time(job_result_dictionary)
+            execution_time=self.execution_time
         )
 
     @abstractmethod
     def _create_job(self, circuit, shots):
         """
 
         @param circuit:
@@ -116,12 +120,12 @@
     def _get_name(self) -> str:
         """
 
         """
         pass
 
     @abstractmethod
-    def _get_execution_time(self, job_result) -> float:
+    def _calculate_execution_time(self, job_result) -> float:
         """
 
         """
         pass
```

### Comparing `quao-0.3.3/src/quao/model/device/ibm_cloud_device.py` & `quao-0.3.4/src/quao/model/device/ibm_cloud_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/model/device/ibm_quantum_device.py` & `quao-0.3.4/src/quao/model/device/ibm_quantum_device.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,12 +16,9 @@
 
     def _parse_job_result(self, job_result) -> dict:
         return JsonParserUtils.parse(job_result.to_dict())
 
     def _create_job(self, circuit, shots):
         logger.debug('Create Ibm Quantum job with {0} shots'.format(shots))
         transpile_circuit = transpile(circuit, self.device)
-        try:
-            return self.device.run(transpile_circuit, shots=shots)
-        except Exception as exception:
-            str(exception)
 
+        return self.device.run(transpile_circuit, shots=shots)
```

### Comparing `quao-0.3.3/src/quao/model/device/qiskit_device.py` & `quao-0.3.4/src/quao/model/device/qiskit_device.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
     def _get_job_status(self, job) -> str:
         return job.status().name
 
     def _get_name(self) -> str:
         return str(self.device.configuration().backend_name)
 
-    def _get_execution_time(self, job_result):
-        logger.debug(job_result)
+    def _calculate_execution_time(self, job_result):
+        if 'metadata' not in job_result:
+            return
+
         metadata = job_result['metadata']
 
         if metadata is None or not bool(metadata):
-            return self.execution_time
+            return
 
         self.execution_time = metadata['time_taken_execute']
-
-        return self.execution_time
```

### Comparing `quao-0.3.3/src/quao/model/device/quao_device.py` & `quao-0.3.4/src/quao/model/device/quao_device.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,18 +78,20 @@
 
         if Sdk.BRAKET.value.__eq__(self.sdk):
             job_state = job.state()
             if JobStatus.COMPLETED.value.__eq__(job_state):
                 job_state = JobStatus.DONE.value
             return job_state
 
-    def _get_execution_time(self, job_result):
+    def _calculate_execution_time(self, job_result):
         if Sdk.QISKIT.value.__eq__(self.sdk):
-            metadata = job_result['metadata']
+            if 'metadata' not in job_result:
+                return
 
-            if metadata is None or not bool(metadata):
-                return self.execution_time
+            metadata = job_result['metadata']
 
-            return metadata['time_taken_execute']
+            if metadata is None \
+                    or not bool(metadata)\
+                    or 'time_taken_execute' not in metadata:
+                return
 
-        if Sdk.BRAKET.value.__eq__(self.sdk):
-            return self.execution_time
+            self.execution_time = metadata['time_taken_execute']
```

### Comparing `quao-0.3.3/src/quao/model/provider/aws_braket_provider.py` & `quao-0.3.4/src/quao/model/provider/aws_braket_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.3.4/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.3.4/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/model/provider/provider.py` & `quao-0.3.4/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/model/provider/quao_provider.py` & `quao-0.3.4/src/quao/model/provider/quao_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/util/json_parser_util.py` & `quao-0.3.4/src/quao/util/json_parser_util.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao/util/response_utils.py` & `quao-0.3.4/src/quao/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.3/src/quao.egg-info/PKG-INFO` & `quao-0.3.4/src/quao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.3.3
+Version: 0.3.4
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.3.3/src/quao.egg-info/SOURCES.txt` & `quao-0.3.4/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

