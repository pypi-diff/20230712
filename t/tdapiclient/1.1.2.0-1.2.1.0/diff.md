# Comparing `tmp/tdapiclient-1.1.2.0.tar.gz` & `tmp/tdapiclient-1.2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdapiclient-1.1.2.0.tar", last modified: Tue Jul 11 18:12:07 2023, max compression
+gzip compressed data, was "tdapiclient-1.2.1.0.tar", last modified: Wed Jul 12 16:03:59 2023, max compression
```

## Comparing `tdapiclient-1.1.2.0.tar` & `tdapiclient-1.2.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 18:12:07.606804 tdapiclient-1.1.2.0/
--rw-rw-rw-   0        0        0    19485 2023-07-11 18:12:07.606804 tdapiclient-1.1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-11 18:12:07.606804 tdapiclient-1.1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2138 2023-06-08 15:23:28.000000 tdapiclient-1.1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:12:07.556805 tdapiclient-1.1.2.0/tdapiclient/
--rw-rw-rw-   0        0        0    17380 2022-11-07 17:49:50.000000 tdapiclient-1.1.2.0/tdapiclient/LICENSE-3RD-PARTY.pdf
--rw-rw-rw-   0        0        0    13208 2022-07-01 15:19:13.000000 tdapiclient-1.1.2.0/tdapiclient/LICENSE.txt
--rw-rw-rw-   0        0        0    15759 2023-07-11 18:09:55.000000 tdapiclient-1.1.2.0/tdapiclient/README.md
--rw-rw-rw-   0        0        0      222 2023-05-24 16:52:43.000000 tdapiclient-1.1.2.0/tdapiclient/__init__.py
--rw-rw-rw-   0        0        0      378 2023-06-08 15:23:28.000000 tdapiclient-1.1.2.0/tdapiclient/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:12:07.602576 tdapiclient-1.1.2.0/tdapiclient/common/
--rw-rw-rw-   0        0        0        0 2023-02-16 18:49:47.000000 tdapiclient-1.1.2.0/tdapiclient/common/__init__.py
--rw-rw-rw-   0        0        0      872 2023-07-11 16:22:37.000000 tdapiclient-1.1.2.0/tdapiclient/common/constants.py
--rw-rw-rw-   0        0        0     2172 2023-02-16 18:49:56.000000 tdapiclient-1.1.2.0/tdapiclient/common/exceptions.py
--rw-rw-rw-   0        0        0     1076 2023-02-16 18:49:56.000000 tdapiclient-1.1.2.0/tdapiclient/common/logger.py
--rw-rw-rw-   0        0        0     3513 2023-07-11 16:22:37.000000 tdapiclient-1.1.2.0/tdapiclient/common/messagecodes.py
--rw-rw-rw-   0        0        0     4151 2023-07-11 16:22:37.000000 tdapiclient-1.1.2.0/tdapiclient/common/messages.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:12:07.604578 tdapiclient-1.1.2.0/tdapiclient/core/
--rw-rw-rw-   0        0        0        0 2022-07-01 15:19:13.000000 tdapiclient-1.1.2.0/tdapiclient/core/__init__.py
--rw-rw-rw-   0        0        0   104897 2023-07-11 16:22:37.000000 tdapiclient-1.1.2.0/tdapiclient/core/tdapiclient.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:12:07.606577 tdapiclient-1.1.2.0/tdapiclient/utils/
--rw-rw-rw-   0        0        0        0 2022-07-01 15:19:13.000000 tdapiclient-1.1.2.0/tdapiclient/utils/__init__.py
--rw-rw-rw-   0        0        0     4054 2022-11-07 17:49:50.000000 tdapiclient-1.1.2.0/tdapiclient/utils/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:12:07.596576 tdapiclient-1.1.2.0/tdapiclient.egg-info/
--rw-rw-rw-   0        0        0    19485 2023-07-11 18:12:07.000000 tdapiclient-1.1.2.0/tdapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-07-11 18:12:07.000000 tdapiclient-1.1.2.0/tdapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 18:12:07.000000 tdapiclient-1.1.2.0/tdapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-07-11 18:12:07.000000 tdapiclient-1.1.2.0/tdapiclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 18:12:07.000000 tdapiclient-1.1.2.0/tdapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-10 00:02:43.000000 tdapiclient-1.1.2.0/tdapiclient.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-12 16:03:59.958724 tdapiclient-1.2.1.0/
+-rw-rw-rw-   0        0        0    19485 2023-07-12 16:03:59.958724 tdapiclient-1.2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:03:59.958724 tdapiclient-1.2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2138 2023-06-08 15:23:28.000000 tdapiclient-1.2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:03:59.902035 tdapiclient-1.2.1.0/tdapiclient/
+-rw-rw-rw-   0        0        0    17380 2022-11-07 17:49:50.000000 tdapiclient-1.2.1.0/tdapiclient/LICENSE-3RD-PARTY.pdf
+-rw-rw-rw-   0        0        0    13208 2022-07-01 15:19:13.000000 tdapiclient-1.2.1.0/tdapiclient/LICENSE.txt
+-rw-rw-rw-   0        0        0    15759 2023-07-12 14:15:26.000000 tdapiclient-1.2.1.0/tdapiclient/README.md
+-rw-rw-rw-   0        0        0      222 2023-05-24 16:52:43.000000 tdapiclient-1.2.1.0/tdapiclient/__init__.py
+-rw-rw-rw-   0        0        0      378 2023-07-12 16:02:01.000000 tdapiclient-1.2.1.0/tdapiclient/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:03:59.958724 tdapiclient-1.2.1.0/tdapiclient/common/
+-rw-rw-rw-   0        0        0        0 2023-02-16 18:49:47.000000 tdapiclient-1.2.1.0/tdapiclient/common/__init__.py
+-rw-rw-rw-   0        0        0      872 2023-07-12 15:59:15.000000 tdapiclient-1.2.1.0/tdapiclient/common/constants.py
+-rw-rw-rw-   0        0        0     2172 2023-02-16 18:49:56.000000 tdapiclient-1.2.1.0/tdapiclient/common/exceptions.py
+-rw-rw-rw-   0        0        0     1076 2023-02-16 18:49:56.000000 tdapiclient-1.2.1.0/tdapiclient/common/logger.py
+-rw-rw-rw-   0        0        0     3513 2023-07-12 15:59:15.000000 tdapiclient-1.2.1.0/tdapiclient/common/messagecodes.py
+-rw-rw-rw-   0        0        0     4151 2023-07-12 15:59:15.000000 tdapiclient-1.2.1.0/tdapiclient/common/messages.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:03:59.958724 tdapiclient-1.2.1.0/tdapiclient/core/
+-rw-rw-rw-   0        0        0        0 2022-07-01 15:19:13.000000 tdapiclient-1.2.1.0/tdapiclient/core/__init__.py
+-rw-rw-rw-   0        0        0   104897 2023-07-12 15:59:15.000000 tdapiclient-1.2.1.0/tdapiclient/core/tdapiclient.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:03:59.958724 tdapiclient-1.2.1.0/tdapiclient/utils/
+-rw-rw-rw-   0        0        0        0 2022-07-01 15:19:13.000000 tdapiclient-1.2.1.0/tdapiclient/utils/__init__.py
+-rw-rw-rw-   0        0        0     4054 2022-11-07 17:49:50.000000 tdapiclient-1.2.1.0/tdapiclient/utils/validators.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:03:59.924113 tdapiclient-1.2.1.0/tdapiclient.egg-info/
+-rw-rw-rw-   0        0        0    19485 2023-07-12 16:03:59.000000 tdapiclient-1.2.1.0/tdapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-07-12 16:03:59.000000 tdapiclient-1.2.1.0/tdapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:03:59.000000 tdapiclient-1.2.1.0/tdapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-07-12 16:03:59.000000 tdapiclient-1.2.1.0/tdapiclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 16:03:59.000000 tdapiclient-1.2.1.0/tdapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-10 00:02:43.000000 tdapiclient-1.2.1.0/tdapiclient.egg-info/zip-safe
```

### Comparing `tdapiclient-1.1.2.0/PKG-INFO` & `tdapiclient-1.2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdapiclient
-Version: 1.1.2.0
+Version: 1.2.1.0
 Summary: Teradata API Client Python package
 Home-page: http://www.teradata.com/
 Author: Teradata Corporation
 License: Teradata License Agreement
 Description: ## tdapiclient - Teradata Third Party Analytics Integration Python Library
         
          tdapiclient Python library allows AWS SageMaker and Teradata users to use AWS SageMaker Python library's interface to train/predict using teradataml DataFrame. tdapiclient will transparantly convert teradataml DataFrame in S3 address to be used for training and it will also allow user to use teradataml DataFrame as input for inference.
@@ -23,16 +23,16 @@
         - [Installation and Requirements](#installation-and-requirements)
         - [Using the tdapiclient Python Package with Sagemaker](#using-the-tdapiclient-python-package-with-sagemaker)
         - [Using the tdapiclient Python Package with Azure-ML](#using-the-tdapiclient-python-package-with-azure-ml)
         - [Documentation](#documentation)
         - [License](#license)
         
         ## Release Notes
-        #### tdapiclient 1.1.2.0
-        * `tdapiclient 1.1.2.00` is the third release version. This release adds BYOM deployment support for SageMaker and optimizes fit method for CSV data format. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
+        #### tdapiclient 1.2.1.0
+        * `tdapiclient 1.2.1.00` is the third release version. This release adds BYOM deployment support for SageMaker and optimizes fit method for CSV data format. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
         
         #### tdapiclient 1.1.1.0
         * `tdapiclient 1.1.1.00` is the second release version. This release adds a support for AzureML integration with Teradata vantage. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
         
         #### tdapiclient 1.0.0.0
         * `tdapiclient 1.00.00.00` is the first release version. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
```

### Comparing `tdapiclient-1.1.2.0/setup.py` & `tdapiclient-1.2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient/LICENSE-3RD-PARTY.pdf` & `tdapiclient-1.2.1.0/tdapiclient/LICENSE-3RD-PARTY.pdf`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient/LICENSE.txt` & `tdapiclient-1.2.1.0/tdapiclient/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient/README.md` & `tdapiclient-1.2.1.0/tdapiclient/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 - [Installation and Requirements](#installation-and-requirements)
 - [Using the tdapiclient Python Package with Sagemaker](#using-the-tdapiclient-python-package-with-sagemaker)
 - [Using the tdapiclient Python Package with Azure-ML](#using-the-tdapiclient-python-package-with-azure-ml)
 - [Documentation](#documentation)
 - [License](#license)
 
 ## Release Notes
-#### tdapiclient 1.1.2.0
-* `tdapiclient 1.1.2.00` is the third release version. This release adds BYOM deployment support for SageMaker and optimizes fit method for CSV data format. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
+#### tdapiclient 1.2.1.0
+* `tdapiclient 1.2.1.00` is the third release version. This release adds BYOM deployment support for SageMaker and optimizes fit method for CSV data format. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
 
 #### tdapiclient 1.1.1.0
 * `tdapiclient 1.1.1.00` is the second release version. This release adds a support for AzureML integration with Teradata vantage. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
 
 #### tdapiclient 1.0.0.0
 * `tdapiclient 1.00.00.00` is the first release version. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
```

### Comparing `tdapiclient-1.1.2.0/tdapiclient/common/constants.py` & `tdapiclient-1.2.1.0/tdapiclient/common/constants.py`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient/common/exceptions.py` & `tdapiclient-1.2.1.0/tdapiclient/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient/common/logger.py` & `tdapiclient-1.2.1.0/tdapiclient/common/logger.py`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient/common/messagecodes.py` & `tdapiclient-1.2.1.0/tdapiclient/common/messagecodes.py`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient/common/messages.py` & `tdapiclient-1.2.1.0/tdapiclient/common/messages.py`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient/core/tdapiclient.py` & `tdapiclient-1.2.1.0/tdapiclient/core/tdapiclient.py`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient/utils/validators.py` & `tdapiclient-1.2.1.0/tdapiclient/utils/validators.py`

 * *Files identical despite different names*

### Comparing `tdapiclient-1.1.2.0/tdapiclient.egg-info/PKG-INFO` & `tdapiclient-1.2.1.0/tdapiclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdapiclient
-Version: 1.1.2.0
+Version: 1.2.1.0
 Summary: Teradata API Client Python package
 Home-page: http://www.teradata.com/
 Author: Teradata Corporation
 License: Teradata License Agreement
 Description: ## tdapiclient - Teradata Third Party Analytics Integration Python Library
         
          tdapiclient Python library allows AWS SageMaker and Teradata users to use AWS SageMaker Python library's interface to train/predict using teradataml DataFrame. tdapiclient will transparantly convert teradataml DataFrame in S3 address to be used for training and it will also allow user to use teradataml DataFrame as input for inference.
@@ -23,16 +23,16 @@
         - [Installation and Requirements](#installation-and-requirements)
         - [Using the tdapiclient Python Package with Sagemaker](#using-the-tdapiclient-python-package-with-sagemaker)
         - [Using the tdapiclient Python Package with Azure-ML](#using-the-tdapiclient-python-package-with-azure-ml)
         - [Documentation](#documentation)
         - [License](#license)
         
         ## Release Notes
-        #### tdapiclient 1.1.2.0
-        * `tdapiclient 1.1.2.00` is the third release version. This release adds BYOM deployment support for SageMaker and optimizes fit method for CSV data format. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
+        #### tdapiclient 1.2.1.0
+        * `tdapiclient 1.2.1.00` is the third release version. This release adds BYOM deployment support for SageMaker and optimizes fit method for CSV data format. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
         
         #### tdapiclient 1.1.1.0
         * `tdapiclient 1.1.1.00` is the second release version. This release adds a support for AzureML integration with Teradata vantage. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
         
         #### tdapiclient 1.0.0.0
         * `tdapiclient 1.00.00.00` is the first release version. Please refer to the _API Integration Guide for Cloud Machine Learning_ for a list of Limitations and Usage Considerations.
```

### Comparing `tdapiclient-1.1.2.0/tdapiclient.egg-info/SOURCES.txt` & `tdapiclient-1.2.1.0/tdapiclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

