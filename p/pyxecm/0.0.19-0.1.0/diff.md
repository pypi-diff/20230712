# Comparing `tmp/pyxecm-0.0.19.tar.gz` & `tmp/pyxecm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.0.19.tar", last modified: Fri Jun 23 05:26:26 2023, max compression
+gzip compressed data, was "pyxecm-0.1.0.tar", last modified: Wed Jul 12 13:06:50 2023, max compression
```

## Comparing `pyxecm-0.0.19.tar` & `pyxecm-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:26:26.130016 pyxecm-0.0.19/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-06-23 05:25:58.000000 pyxecm-0.0.19/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1639 2023-06-23 05:26:26.130016 pyxecm-0.0.19/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-06-23 05:25:58.000000 pyxecm-0.0.19/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-06-23 05:26:16.000000 pyxecm-0.0.19/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:26:26.127016 pyxecm-0.0.19/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/assoc.py
--rw-rw-rw-   0 root         (0) root         (0)    33694 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)    77794 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/m365.py
--rw-rw-rw-   0 root         (0) root         (0)    51479 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/main.py
--rw-rw-rw-   0 root         (0) root         (0)     9554 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   256466 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   129349 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1627 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10240 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)   297179 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/payload.py
--rw-rw-rw-   0 root         (0) root         (0)     5986 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/sap.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/translate.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/web.py
--rw-rw-rw-   0 root         (0) root         (0)    21850 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:26:26.129016 pyxecm-0.0.19/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1639 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      424 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 05:26:26.130016 pyxecm-0.0.19/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-23 05:25:58.000000 pyxecm-0.0.19/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:06:50.292936 pyxecm-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-07-12 13:06:32.000000 pyxecm-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-07-12 13:06:50.292936 pyxecm-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-12 13:06:32.000000 pyxecm-0.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-12 13:06:40.000000 pyxecm-0.1.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:06:50.290936 pyxecm-0.1.0/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/assoc.py
+-rw-rw-rw-   0 root         (0) root         (0)    33694 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)     9554 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   256462 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   129349 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10240 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    21848 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:06:50.291936 pyxecm-0.1.0/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 13:06:50.292936 pyxecm-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-12 13:06:32.000000 pyxecm-0.1.0/setup.py
```

### Comparing `pyxecm-0.0.19/LICENSE` & `pyxecm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.19/PKG-INFO` & `pyxecm-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.19
+Version: 0.1.0
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
-Project-URL: Homepage, https://gitlab.otxlab.net/ecm/pyxecm
+Project-URL: Homepage, https://ecm.glpages.otxlab.net/pyxecm/
 Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
```

### Comparing `pyxecm-0.0.19/README.md` & `pyxecm-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.19/pyproject.toml` & `pyxecm-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 
 [build-system]
   build-backend = "setuptools.build_meta"
   requires = ["setuptools >= 61.0"]
 
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
-  dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36", "suds"]
+  dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "zipfile36", "suds"]
   description = "A Python library to interact with Opentext Extended ECM REST API"
   keywords = ["opentext", "extendedecm", "contentserver", "otds", "appworks", "archivecenter"]
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.0.19"
+  version = "0.1.0"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
     name = "Dr. Marc Diefenbruch"
 
   [project.urls]
-    Homepage = "https://gitlab.otxlab.net/ecm/pyxecm"
+    Homepage = "https://ecm.glpages.otxlab.net/pyxecm/"
 
 [tool]
 
   [tool.setuptools]
     packages = ["pyxecm"]
```

### Comparing `pyxecm-0.0.19/pyxecm/assoc.py` & `pyxecm-0.1.0/pyxecm/assoc.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.19/pyxecm/k8s.py` & `pyxecm-0.1.0/pyxecm/k8s.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.19/pyxecm/otac.py` & `pyxecm-0.1.0/pyxecm/otac.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.19/pyxecm/otcs.py` & `pyxecm-0.1.0/pyxecm/otcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 import os
 import logging
 import requests
 import json
 import urllib.parse
 from datetime import datetime
 import zipfile
-from pyxecm.xml import *
+from .xml import XML
 
 logger = logging.getLogger(os.path.basename(__file__))
 
 requestJsonHeaders = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
```

### Comparing `pyxecm-0.0.19/pyxecm/otds.py` & `pyxecm-0.1.0/pyxecm/otds.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.19/pyxecm/otiv.py` & `pyxecm-0.1.0/pyxecm/otiv.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.19/pyxecm/otpd.py` & `pyxecm-0.1.0/pyxecm/otpd.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.19/pyxecm/web.py` & `pyxecm-0.1.0/pyxecm/web.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.19/pyxecm/xml.py` & `pyxecm-0.1.0/pyxecm/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import re
 # import regex as re
 
 # we need lxml instead of stadard xml.etree to have xpath capabilities!
 from lxml import etree
 
 # import xml.etree.ElementTree as etree
-from pyxecm.assoc import *
+from .assoc import Assoc
 
 logger = logging.getLogger(os.path.basename(__file__))
 
 
 class XML:
     @classmethod
     def getXmlElement(cls, xml_content: str, xpath: str):
```

### Comparing `pyxecm-0.0.19/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.1.0/pyxecm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.19
+Version: 0.1.0
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
-Project-URL: Homepage, https://gitlab.otxlab.net/ecm/pyxecm
+Project-URL: Homepage, https://ecm.glpages.otxlab.net/pyxecm/
 Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
```

