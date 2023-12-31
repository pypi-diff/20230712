# Comparing `tmp/xdmod_data-1.0.0b3-py3-none-any.whl.zip` & `tmp/xdmod_data-1.0.0b4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 16295 bytes, number of entries: 13
+Zip file size: 16265 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       37 b- defN 23-Jul-11 14:04 xdmod_data/__init__.py
--rw-r--r--  2.0 unx       54 b- defN 23-Jul-12 14:34 xdmod_data/__version__.py
+-rw-r--r--  2.0 unx       54 b- defN 23-Jul-12 18:50 xdmod_data/__version__.py
 -rw-r--r--  2.0 unx     2262 b- defN 23-Jul-11 14:04 xdmod_data/_descriptors.py
 -rw-r--r--  2.0 unx     5230 b- defN 23-Jul-11 14:04 xdmod_data/_http_requester.py
 -rw-r--r--  2.0 unx     4435 b- defN 23-Jul-11 14:04 xdmod_data/_response_processor.py
 -rw-r--r--  2.0 unx    10394 b- defN 23-Jul-11 14:04 xdmod_data/_validator.py
 -rw-r--r--  2.0 unx     3018 b- defN 23-Jul-11 14:04 xdmod_data/themes.py
 -rw-r--r--  2.0 unx    16931 b- defN 23-Jul-11 14:04 xdmod_data/warehouse.py
--rw-r--r--  2.0 unx     7652 b- defN 23-Jul-12 14:35 xdmod_data-1.0.0b3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3901 b- defN 23-Jul-12 14:35 xdmod_data-1.0.0b3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 14:35 xdmod_data-1.0.0b3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-12 14:35 xdmod_data-1.0.0b3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1067 b- defN 23-Jul-12 14:35 xdmod_data-1.0.0b3.dist-info/RECORD
-13 files, 55084 bytes uncompressed, 14513 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx     7652 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3801 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1067 b- defN 23-Jul-12 18:50 xdmod_data-1.0.0b4.dist-info/RECORD
+13 files, 54984 bytes uncompressed, 14483 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: xdmod_data/themes.py
 Comment: 
 
 Filename: xdmod_data/warehouse.py
 Comment: 
 
-Filename: xdmod_data-1.0.0b3.dist-info/LICENSE
+Filename: xdmod_data-1.0.0b4.dist-info/LICENSE
 Comment: 
 
-Filename: xdmod_data-1.0.0b3.dist-info/METADATA
+Filename: xdmod_data-1.0.0b4.dist-info/METADATA
 Comment: 
 
-Filename: xdmod_data-1.0.0b3.dist-info/WHEEL
+Filename: xdmod_data-1.0.0b4.dist-info/WHEEL
 Comment: 
 
-Filename: xdmod_data-1.0.0b3.dist-info/top_level.txt
+Filename: xdmod_data-1.0.0b4.dist-info/top_level.txt
 Comment: 
 
-Filename: xdmod_data-1.0.0b3.dist-info/RECORD
+Filename: xdmod_data-1.0.0b4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xdmod_data/__version__.py

```diff
@@ -1,2 +1,2 @@
 __title__ = 'xdmod-data'
-__version__ = '1.0.0-beta.3'
+__version__ = '1.0.0-beta.4'
```

## Comparing `xdmod_data-1.0.0b3.dist-info/LICENSE` & `xdmod_data-1.0.0b4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xdmod_data-1.0.0b3.dist-info/METADATA` & `xdmod_data-1.0.0b4.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdmod-data
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Python package for XDMoD data access
 Author: Aaron Weeden, Joseph P. White
 Maintainer: Aaron Weeden, Joseph P. White
 Project-URL: Source Code, https://github.com/ubccr/xdmod-data
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,16 +18,14 @@
 
 The package can be installed from PyPI via `pip install xdmod-data`.
 
 It has dependencies on [NumPy](https://pypi.org/project/numpy/), [Pandas](https://pypi.org/project/pandas/), [Plotly](https://pypi.org/project/plotly/), and [Requests](https://pypi.org/project/requests/).
 
 Example usage is documented through Jupyter notebooks in the [xdmod-notebooks](https://github.com/ubccr/xdmod-notebooks) repository.
 
-The details of the API are documented [here](https://open.xdmod.org/data-analytics-framework/api).
-
 ## API Token Access
 Use of the Data Analytics Framework requires an API token. To obtain an API token, follow the steps below to obtain an API token from the XDMoD portal.
 
 1. First, if you are not already signed in to the portal, sign in in the top-left corner:
 
     ![Screenshot of "Sign In" button](https://raw.githubusercontent.com/ubccr/xdmod-data/main/docs/images/api-token/sign-in.jpg)
```

## Comparing `xdmod_data-1.0.0b3.dist-info/RECORD` & `xdmod_data-1.0.0b4.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 xdmod_data/__init__.py,sha256=e3S0EcDGJlWIp2hddSFjvt633jfeZ4W7VyAeLpfTWVM,37
-xdmod_data/__version__.py,sha256=8_0sFmNx20X_8Xxcx-wS_hCysu7unYzV17jD0erP1sU,54
+xdmod_data/__version__.py,sha256=mtscD2fli52hysFpfP78r-oPIMOIc7UJF4-dBuA062Y,54
 xdmod_data/_descriptors.py,sha256=uUbC65oW5Vur-DhFEs__NrYTpCt5FrngTYVgu08FgwE,2262
 xdmod_data/_http_requester.py,sha256=7936UGqjrKrW4vY0bEsONRx0CYfPQojr-YEVieEkosg,5230
 xdmod_data/_response_processor.py,sha256=Vslz3-DtlhhoukJ11yJWcLi0wIcZSCIHMLlETzA9WEU,4435
 xdmod_data/_validator.py,sha256=GWHH_U5r_QVcZG9C_yo1xMGoxIFXmC__5l94-hqLcPE,10394
 xdmod_data/themes.py,sha256=eSD7_dJsFhiB3qrMW7FP54IFPXh9tr1XjHXIB6nvx-c,3018
 xdmod_data/warehouse.py,sha256=W7vMIAp_BiKEa15oipiRfZRmVBTfShqie4hFuj6TMdQ,16931
-xdmod_data-1.0.0b3.dist-info/LICENSE,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
-xdmod_data-1.0.0b3.dist-info/METADATA,sha256=kS-EHhoBn5b-Vse3T6ENHT_NzKvqtwK7xL_DdItSCvU,3901
-xdmod_data-1.0.0b3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-xdmod_data-1.0.0b3.dist-info/top_level.txt,sha256=ph-NOi5tK19CfM5XnNOGuId1orUYaKQPxOPiS-geLPk,11
-xdmod_data-1.0.0b3.dist-info/RECORD,,
+xdmod_data-1.0.0b4.dist-info/LICENSE,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
+xdmod_data-1.0.0b4.dist-info/METADATA,sha256=wdrB_MtdxlWLtoaBDnJrcOcotH1L5qvy3TDPrVOESEo,3801
+xdmod_data-1.0.0b4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+xdmod_data-1.0.0b4.dist-info/top_level.txt,sha256=ph-NOi5tK19CfM5XnNOGuId1orUYaKQPxOPiS-geLPk,11
+xdmod_data-1.0.0b4.dist-info/RECORD,,
```

