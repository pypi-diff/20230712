# Comparing `tmp/mi-pyral-0.2.1.tar.gz` & `tmp/mi-pyral-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mi-pyral-0.2.1.tar", last modified: Wed Jul 12 13:39:13 2023, max compression
+gzip compressed data, was "mi-pyral-0.2.2.tar", last modified: Wed Jul 12 15:33:35 2023, max compression
```

## Comparing `mi-pyral-0.2.1.tar` & `mi-pyral-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 13:39:13.843759 mi-pyral-0.2.1/
--rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/LICENSE
--rw-r--r--   0 starr      (501) staff       (20)       66 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/MANIFEST.in
--rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 13:39:13.843654 mi-pyral-0.2.1/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)      210 2022-10-08 18:13:55.000000 mi-pyral-0.2.1/README.md
--rw-r--r--   0 starr      (501) staff       (20)      922 2023-07-12 13:38:58.000000 mi-pyral-0.2.1/pyproject.toml
--rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-12 13:39:13.843795 mi-pyral-0.2.1/setup.cfg
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 13:39:13.841295 mi-pyral-0.2.1/src/
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 13:39:13.842283 mi-pyral-0.2.1/src/mi_pyral.egg-info/
--rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)      479 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/SOURCES.txt
--rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/dependency_links.txt
--rw-r--r--   0 starr      (501) staff       (20)       47 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/entry_points.txt
--rw-r--r--   0 starr      (501) staff       (20)       91 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/requires.txt
--rw-r--r--   0 starr      (501) staff       (20)        6 2023-07-12 13:39:13.000000 mi-pyral-0.2.1/src/mi_pyral.egg-info/top_level.txt
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 13:39:13.843507 mi-pyral-0.2.1/src/pyral/
--rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-12 13:38:58.000000 mi-pyral-0.2.1/src/pyral/__init__.py
--rw-r--r--   0 starr      (501) staff       (20)     1453 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/__main__.py
--rw-r--r--   0 starr      (501) staff       (20)     1131 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/command.py
--rw-r--r--   0 starr      (501) staff       (20)     2041 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/database.py
--rw-r--r--   0 starr      (501) staff       (20)      726 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/exceptions.py
--rw-r--r--   0 starr      (501) staff       (20)      807 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/log.conf
--rw-r--r--   0 starr      (501) staff       (20)    25036 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/relation.py
--rw-r--r--   0 starr      (501) staff       (20)    18344 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/relvar.py
--rw-r--r--   0 starr      (501) staff       (20)      435 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/rtypes.py
--rw-r--r--   0 starr      (501) staff       (20)     2104 2023-07-12 13:36:46.000000 mi-pyral-0.2.1/src/pyral/transaction.py
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 15:33:35.881379 mi-pyral-0.2.2/
+-rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-12 13:36:46.000000 mi-pyral-0.2.2/LICENSE
+-rw-r--r--   0 starr      (501) staff       (20)       66 2023-07-12 13:36:46.000000 mi-pyral-0.2.2/MANIFEST.in
+-rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 15:33:35.881276 mi-pyral-0.2.2/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)      210 2022-10-08 18:13:55.000000 mi-pyral-0.2.2/README.md
+-rw-r--r--   0 starr      (501) staff       (20)      922 2023-07-12 15:32:52.000000 mi-pyral-0.2.2/pyproject.toml
+-rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-12 15:33:35.881414 mi-pyral-0.2.2/setup.cfg
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 15:33:35.879001 mi-pyral-0.2.2/src/
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 15:33:35.880036 mi-pyral-0.2.2/src/mi_pyral.egg-info/
+-rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 15:33:35.000000 mi-pyral-0.2.2/src/mi_pyral.egg-info/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)      479 2023-07-12 15:33:35.000000 mi-pyral-0.2.2/src/mi_pyral.egg-info/SOURCES.txt
+-rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-12 15:33:35.000000 mi-pyral-0.2.2/src/mi_pyral.egg-info/dependency_links.txt
+-rw-r--r--   0 starr      (501) staff       (20)       47 2023-07-12 15:33:35.000000 mi-pyral-0.2.2/src/mi_pyral.egg-info/entry_points.txt
+-rw-r--r--   0 starr      (501) staff       (20)       91 2023-07-12 15:33:35.000000 mi-pyral-0.2.2/src/mi_pyral.egg-info/requires.txt
+-rw-r--r--   0 starr      (501) staff       (20)        6 2023-07-12 15:33:35.000000 mi-pyral-0.2.2/src/mi_pyral.egg-info/top_level.txt
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 15:33:35.881117 mi-pyral-0.2.2/src/pyral/
+-rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-12 15:32:52.000000 mi-pyral-0.2.2/src/pyral/__init__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1453 2023-07-12 13:36:46.000000 mi-pyral-0.2.2/src/pyral/__main__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1131 2023-07-12 13:36:46.000000 mi-pyral-0.2.2/src/pyral/command.py
+-rw-r--r--   0 starr      (501) staff       (20)     2047 2023-07-12 15:32:41.000000 mi-pyral-0.2.2/src/pyral/database.py
+-rw-r--r--   0 starr      (501) staff       (20)      726 2023-07-12 13:36:46.000000 mi-pyral-0.2.2/src/pyral/exceptions.py
+-rw-r--r--   0 starr      (501) staff       (20)      807 2023-07-12 13:36:46.000000 mi-pyral-0.2.2/src/pyral/log.conf
+-rw-r--r--   0 starr      (501) staff       (20)    25048 2023-07-12 15:32:41.000000 mi-pyral-0.2.2/src/pyral/relation.py
+-rw-r--r--   0 starr      (501) staff       (20)    18368 2023-07-12 15:32:41.000000 mi-pyral-0.2.2/src/pyral/relvar.py
+-rw-r--r--   0 starr      (501) staff       (20)      435 2023-07-12 13:36:46.000000 mi-pyral-0.2.2/src/pyral/rtypes.py
+-rw-r--r--   0 starr      (501) staff       (20)     2110 2023-07-12 15:32:41.000000 mi-pyral-0.2.2/src/pyral/transaction.py
```

### Comparing `mi-pyral-0.2.1/LICENSE` & `mi-pyral-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.1/PKG-INFO` & `mi-pyral-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mi-pyral
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyRAL Pythonic interface to TclRAL
 Author-email: Leon Starr <leon_starr@modelint.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Leon Starr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mi-pyral-0.2.1/pyproject.toml` & `mi-pyral-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mi-pyral"
-version = "0.2.1"
+version = "0.2.2"
 description = "PyRAL Pythonic interface to TclRAL"
 readme = "README.md"
 authors = [{ name = "Leon Starr", email = "leon_starr@modelint.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mi-pyral-0.2.1/src/mi_pyral.egg-info/PKG-INFO` & `mi-pyral-0.2.2/src/mi_pyral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mi-pyral
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyRAL Pythonic interface to TclRAL
 Author-email: Leon Starr <leon_starr@modelint.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Leon Starr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mi-pyral-0.2.1/src/pyral/__main__.py` & `mi-pyral-0.2.2/src/pyral/__main__.py`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.1/src/pyral/command.py` & `mi-pyral-0.2.2/src/pyral/command.py`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.1/src/pyral/database.py` & `mi-pyral-0.2.2/src/pyral/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 database.py - Create and manage a tclRAL database
 """
 
 import logging
 import tkinter
-from transaction import Transaction
+from pyral.transaction import Transaction
 
 class Database:
     """
     Proxy for a tclRAL database.
 
     First we must initiate the connection with an optionally specified database.
     If none is specified, a new in memory database may be created
```

### Comparing `mi-pyral-0.2.1/src/pyral/exceptions.py` & `mi-pyral-0.2.2/src/pyral/exceptions.py`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.1/src/pyral/log.conf` & `mi-pyral-0.2.2/src/pyral/log.conf`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.1/src/pyral/relation.py` & `mi-pyral-0.2.2/src/pyral/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 relation.py – Operations on relations
 """
 
 import logging
 import re
 from tabulate import tabulate
 from typing import List, Optional, Dict, Tuple
-from rtypes import RelationValue
-from command import Command
+from pyral.rtypes import RelationValue
+from pyral.command import Command
 
 from tkinter import Tk
 
 # If we want to apply successive (nested) operations in TclRAL we need to have the result
 # of each TclRAL command saved in tcl variable. So each time we execute a command that produces
 # a relation result we save it. The variable name is chosen so that it shouldn't conflict with
 # any user relvars. Do not ever use the name below as one of your user relvars!
```

### Comparing `mi-pyral-0.2.1/src/pyral/relvar.py` & `mi-pyral-0.2.2/src/pyral/relvar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 relvar.py – TclRAL operations on relvars
 """
 
 import logging
 from typing import List, Dict, Any
-from rtypes import Attribute, Mult, delim
-from transaction import Transaction
-from command import Command
-from relation import Relation
+from pyral.rtypes import Attribute, Mult, delim
+from pyral.transaction import Transaction
+from pyral.command import Command
+from pyral.relation import Relation
 from collections import namedtuple
 from tkinter import Tk
 
 class Relvar:
     """
     A relational variable (table)
```

### Comparing `mi-pyral-0.2.1/src/pyral/transaction.py` & `mi-pyral-0.2.2/src/pyral/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 transaction.py -- Database transaction
 """
 import logging
-from exceptions import IncompleteTransactionPending, NoOpenTransaction
+from pyral.exceptions import IncompleteTransactionPending, NoOpenTransaction
 from tkinter import Tk
 
 class Transaction:
     """
     A TclRAL transaction
 
     """
```

