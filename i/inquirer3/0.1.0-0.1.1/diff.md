# Comparing `tmp/inquirer3-0.1.0.tar.gz` & `tmp/inquirer3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inquirer3-0.1.0.tar", max compression
+gzip compressed data, was "inquirer3-0.1.1.tar", max compression
```

## Comparing `inquirer3-0.1.0.tar` & `inquirer3-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1088 2023-07-08 18:57:19.916773 inquirer3-0.1.0/LICENSE
--rw-r--r--   0        0        0     5331 2023-07-08 18:57:19.916773 inquirer3-0.1.0/README.md
--rw-r--r--   0        0        0     1829 2023-07-08 18:57:31.660991 inquirer3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      974 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/__init__.py
--rw-r--r--   0        0        0      412 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/errors.py
--rw-r--r--   0        0        0      351 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/events.py
--rw-r--r--   0        0        0      565 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/prompt.py
--rw-r--r--   0        0        0     9746 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/questions.py
--rw-r--r--   0        0        0      315 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/__init__.py
--rw-r--r--   0        0        0     6156 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/__init__.py
--rw-r--r--   0        0        0     5368 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_checkbox.py
--rw-r--r--   0        0        0      726 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_confirm.py
--rw-r--r--   0        0        0     1091 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_editor.py
--rw-r--r--   0        0        0     3550 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_list.py
--rw-r--r--   0        0        0      103 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_other.py
--rw-r--r--   0        0        0      382 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_password.py
--rw-r--r--   0        0        0       77 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_path.py
--rw-r--r--   0        0        0     2483 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/_text.py
--rw-r--r--   0        0        0     1314 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/render/console/base.py
--rw-r--r--   0        0        0     1457 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/shortcuts.py
--rw-r--r--   0        0        0     4484 2023-07-08 18:57:19.920774 inquirer3-0.1.0/src/inquirer3/themes.py
--rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 inquirer3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-07-11 23:35:58.051726 inquirer3-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5331 2023-07-11 23:35:58.051726 inquirer3-0.1.1/README.md
+-rw-r--r--   0        0        0     1829 2023-07-11 23:36:13.444804 inquirer3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      974 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/errors.py
+-rw-r--r--   0        0        0      351 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/events.py
+-rw-r--r--   0        0        0      565 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/prompt.py
+-rw-r--r--   0        0        0     9746 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/questions.py
+-rw-r--r--   0        0        0      315 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/__init__.py
+-rw-r--r--   0        0        0     6156 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/__init__.py
+-rw-r--r--   0        0        0     5368 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/_checkbox.py
+-rw-r--r--   0        0        0      726 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/_confirm.py
+-rw-r--r--   0        0        0     1091 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/_editor.py
+-rw-r--r--   0        0        0     3550 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/_list.py
+-rw-r--r--   0        0        0      103 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/_other.py
+-rw-r--r--   0        0        0      382 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/_password.py
+-rw-r--r--   0        0        0       77 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/_path.py
+-rw-r--r--   0        0        0     2483 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/_text.py
+-rw-r--r--   0        0        0     1314 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/render/console/base.py
+-rw-r--r--   0        0        0     1457 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/shortcuts.py
+-rw-r--r--   0        0        0     4484 2023-07-11 23:35:58.059727 inquirer3-0.1.1/src/inquirer3/themes.py
+-rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 inquirer3-0.1.1/PKG-INFO
```

### Comparing `inquirer3-0.1.0/LICENSE` & `inquirer3-0.1.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-The MIT License (MIT)
+# The MIT License (MIT)
 
 Copyright (c) 2014 Miguel Ángel García
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `inquirer3-0.1.0/README.md` & `inquirer3-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/pyproject.toml` & `inquirer3-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inquirer3"
-version = "0.1.0"
+version = "0.1.1"
 description = "Collection of common interactive command line user interfaces, based on Inquirer.js"
 authors = ["Guy Salton <guy123121@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/guysalt/python-inquirer3"
 repository = "https://github.com/guysalt/python-inquirer3"
 documentation = "https://python-inquirer3.readthedocs.io/en/latest/"
@@ -38,15 +38,15 @@
 pre-commit = "^3.3.3"
 pre-commit-hooks = "^4.4.0"
 pyupgrade = "^3.8.0"
 safety = "^2.3.5"
 sphinx = "^7.0.1"
 sphinx-autobuild = "^2021.3.14"
 nox = "^2023.4.22"
-nox-poetry = "^1.0.2"
+nox-poetry = "^1.0.3"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `inquirer3-0.1.0/src/inquirer3/__init__.py` & `inquirer3-0.1.1/src/inquirer3/__init__.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/prompt.py` & `inquirer3-0.1.1/src/inquirer3/prompt.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/questions.py` & `inquirer3-0.1.1/src/inquirer3/questions.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/render/console/__init__.py` & `inquirer3-0.1.1/src/inquirer3/render/console/__init__.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/render/console/_checkbox.py` & `inquirer3-0.1.1/src/inquirer3/render/console/_checkbox.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/render/console/_confirm.py` & `inquirer3-0.1.1/src/inquirer3/render/console/_confirm.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/render/console/_editor.py` & `inquirer3-0.1.1/src/inquirer3/render/console/_editor.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/render/console/_list.py` & `inquirer3-0.1.1/src/inquirer3/render/console/_list.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/render/console/_text.py` & `inquirer3-0.1.1/src/inquirer3/render/console/_text.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/render/console/base.py` & `inquirer3-0.1.1/src/inquirer3/render/console/base.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/shortcuts.py` & `inquirer3-0.1.1/src/inquirer3/shortcuts.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/src/inquirer3/themes.py` & `inquirer3-0.1.1/src/inquirer3/themes.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.1.0/PKG-INFO` & `inquirer3-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inquirer3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collection of common interactive command line user interfaces, based on Inquirer.js
 Home-page: https://github.com/guysalt/python-inquirer3
 License: MIT
 Author: Guy Salton
 Author-email: guy123121@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

