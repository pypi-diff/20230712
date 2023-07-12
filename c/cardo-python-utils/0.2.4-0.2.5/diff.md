# Comparing `tmp/cardo-python-utils-0.2.4.tar.gz` & `tmp/cardo-python-utils-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardo-python-utils-0.2.4.tar", last modified: Tue Jul 11 13:47:31 2023, max compression
+gzip compressed data, was "cardo-python-utils-0.2.5.tar", last modified: Wed Jul 12 13:14:03 2023, max compression
```

## Comparing `cardo-python-utils-0.2.4.tar` & `cardo-python-utils-0.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-11 13:47:31.368748 cardo-python-utils-0.2.4/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/MANIFEST.in
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-11 13:47:31.368748 cardo-python-utils-0.2.4/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.4/README.rst
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-11 13:47:31.364748 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/top_level.txt
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-11 13:47:31.368748 cardo-python-utils-0.2.4/python_utils/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2501 2023-07-11 13:35:59.000000 cardo-python-utils-0.2.4/python_utils/choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/data_structures.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/db.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/django_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16152 2023-07-11 13:44:06.000000 cardo-python-utils-0.2.4/python_utils/esma_choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/imports.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/math.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/pandas_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/rest.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/text.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/time.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/types_hinting.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-07-11 13:47:31.368748 cardo-python-utils-0.2.4/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-12 13:14:03.000482 cardo-python-utils-0.2.5/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/MANIFEST.in
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-12 13:14:03.000482 cardo-python-utils-0.2.5/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.5/README.rst
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-12 13:14:03.000482 cardo-python-utils-0.2.5/cardo_python_utils.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-12 13:14:02.000000 cardo-python-utils-0.2.5/cardo_python_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-07-12 13:14:02.000000 cardo-python-utils-0.2.5/cardo_python_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-07-12 13:14:02.000000 cardo-python-utils-0.2.5/cardo_python_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-07-12 13:14:02.000000 cardo-python-utils-0.2.5/cardo_python_utils.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-07-12 13:14:02.000000 cardo-python-utils-0.2.5/cardo_python_utils.egg-info/top_level.txt
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-12 13:14:03.000482 cardo-python-utils-0.2.5/python_utils/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2501 2023-07-11 13:35:59.000000 cardo-python-utils-0.2.5/python_utils/choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/data_structures.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/db.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/django_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16141 2023-07-12 13:13:16.000000 cardo-python-utils-0.2.5/python_utils/esma_choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/imports.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/math.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/pandas_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/rest.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/text.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/time.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/python_utils/types_hinting.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-07-12 13:14:03.004482 cardo-python-utils-0.2.5/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.5/setup.py
```

### Comparing `cardo-python-utils-0.2.4/LICENSE` & `cardo-python-utils-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/PKG-INFO` & `cardo-python-utils-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.4/README.rst` & `cardo-python-utils-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/cardo_python_utils.egg-info/PKG-INFO` & `cardo-python-utils-0.2.5/cardo_python_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.4/cardo_python_utils.egg-info/SOURCES.txt` & `cardo-python-utils-0.2.5/cardo_python_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/choices.py` & `cardo-python-utils-0.2.5/python_utils/choices.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/data_structures.py` & `cardo-python-utils-0.2.5/python_utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/django_utils.py` & `cardo-python-utils-0.2.5/python_utils/django_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/esma_choices.py` & `cardo-python-utils-0.2.5/python_utils/esma_choices.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,14 @@
     OTHR_R3 = 34, "Ancillary units"
     CBLD_R1 = 35, "Retail"
     CBLD_R2 = 36, "Office"
     IBLD = 37, "Industrial"
     RBLD = 38, "Residential"
 
 
-
 class GuaranteeAssetClassChoices(ChoiceEnum):
     GUAR_G1 = 40, "Personal Guarantee"
     GUAR_G2 = 41, "Government Guarantee"
     GUAR_G3 = 42, "Bank Guarantee"
     GUAR_G4 = 43, "Corporate Guarantee"
     OTHR_G1 = 44, "Pledge on titles"
     OTHR_G2 = 45, "Pledge on goods or inventory"
@@ -332,16 +331,16 @@
 
 class SPVCashAccountTypeChoices(ChoiceEnum):
     CARE = 1, "Cash Reserve Account"
     CORE = 2, "Commingling Reserve Account"
     SORE = 3, "Set-off Reserve Account"
     LQDF = 4, "Liquidity Facility"
     MGAC = 5, "Margin Account"
-    COLLECTION_ACCOUNT = 6, "Collection Account"
-    OTHR = 10, "Other Account"
+    OTHR_1 = 6, "Collection Account"
+    OTHR_2 = 10, "Other Account"
 
 
 class SPVTriggerConsequenceChoices(ChoiceEnum):
     CHPP = 1, "Change in the priority of payments"
     CHCP = 2, "Replacement of a counterparty"
     BOTH = 3, "Both change in the priority of payments and replacement of a counterparty"
     OTHR = 10, "Other consequence"
```

### Comparing `cardo-python-utils-0.2.4/python_utils/exceptions.py` & `cardo-python-utils-0.2.5/python_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/imports.py` & `cardo-python-utils-0.2.5/python_utils/imports.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/math.py` & `cardo-python-utils-0.2.5/python_utils/math.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/pandas_utils.py` & `cardo-python-utils-0.2.5/python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/rest.py` & `cardo-python-utils-0.2.5/python_utils/rest.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/text.py` & `cardo-python-utils-0.2.5/python_utils/text.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/python_utils/time.py` & `cardo-python-utils-0.2.5/python_utils/time.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.4/setup.cfg` & `cardo-python-utils-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardo-python-utils
-version = 0.2.4
+version = 0.2.5
 description = Python library enhanced with a wide range of functions for different scenarios.
 long_description = file: README.rst
 url = https://github.com/CardoAI/cardo-python-utils
 author = Kristi Kotini
 author_email = hello@cardoai.com
 license = MIT (X11)
 classifiers =
```

