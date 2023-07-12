# Comparing `tmp/namespace_mahdimir-2.0.0.tar.gz` & `tmp/namespace_mahdimir-2.1.0.tar.gz`

## Comparing `namespace_mahdimir-2.0.0.tar` & `namespace_mahdimir-2.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-2.0.0/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.0.0/src/namespace_mahdimir/__init__.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 namespace_mahdimir-2.0.0/src/namespace_mahdimir/tse.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 namespace_mahdimir-2.0.0/src/namespace_mahdimir/tse_github_data_url.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-2.0.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-2.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.0.0/README.md
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 namespace_mahdimir-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 namespace_mahdimir-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-2.1.0/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.1.0/src/namespace_mahdimir/__init__.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 namespace_mahdimir-2.1.0/src/namespace_mahdimir/tse.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 namespace_mahdimir-2.1.0/src/namespace_mahdimir/tse_github_data_url.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-2.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.1.0/README.md
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 namespace_mahdimir-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 namespace_mahdimir-2.1.0/PKG-INFO
```

### Comparing `namespace_mahdimir-2.0.0/src/namespace_mahdimir/tse.py` & `namespace_mahdimir-2.1.0/src/namespace_mahdimir/tse.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     b = "Bank"
     i = "Insurance"
     l = "Leasing"
     r = "RealEstate"
     a = "Agriculture"
     f = "Financing"
 
-class DInsIndCols :
+class DIndInsCols :
     bdc = 'Buy-Ind-Count'
     bsc = 'Buy-Ins-Count'
     sdc = 'Sell-Ind-Count'
     ssc = 'Sell-Ins-Count'
 
     bdv = 'Buy-Ind-Vol'
     bsv = 'Buy-Ins-Vol'
```

### Comparing `namespace_mahdimir-2.0.0/src/namespace_mahdimir/tse_github_data_url.py` & `namespace_mahdimir-2.1.0/src/namespace_mahdimir/tse_github_data_url.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,12 +11,13 @@
     rf = 'd-Iran-RiskFree-Rate-Monthly'
     mkt_indx = 'd-TSE-Overall-Index-TEDPIX'
     codal_ltrs = 'd-all-Codal-letters'
     codal_tics_2_ftics = 'd-CodalTicker-2-FirmTicker'
     adj_price = 'd-Adj-Price'
     tse_work_days = 'd-TSE-Work-Days'
     adj_ret = 'd-Adj-Ret'
+    tedpix = 'd-TEDPIX'
 
     def __init__(self) :
         for ky , vl in vars(GitHubDataUrl).items() :
             if not ky.startswith('_') :
                 setattr(self , ky , m + vl)
```

### Comparing `namespace_mahdimir-2.0.0/.gitignore` & `namespace_mahdimir-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-2.0.0/LICENSE` & `namespace_mahdimir-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-2.0.0/pyproject.toml` & `namespace_mahdimir-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "namespace_mahdimir"
-version = "2.0.0"
+version = "2.1.0"
 authors = [{ name = "Mahdi Mir", email = "imahdimir@gmail.com" }]
 description = "Some Namespaces for Python"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
 
 ]
```

### Comparing `namespace_mahdimir-2.0.0/PKG-INFO` & `namespace_mahdimir-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namespace_mahdimir
-Version: 2.0.0
+Version: 2.1.0
 Summary: Some Namespaces for Python
 Project-URL: Homepage, https://github.com/imahdimir/namespace_mahdimir
 Project-URL: Bug Tracker, https://github.com/imahdimir/namespace_mahdimir/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
```

