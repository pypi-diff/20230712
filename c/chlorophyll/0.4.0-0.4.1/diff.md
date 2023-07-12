# Comparing `tmp/chlorophyll-0.4.0.tar.gz` & `tmp/chlorophyll-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chlorophyll-0.4.0.tar", last modified: Wed Jul 12 14:24:22 2023, max compression
+gzip compressed data, was "chlorophyll-0.4.1.tar", last modified: Wed Jul 12 15:40:09 2023, max compression
```

## Comparing `chlorophyll-0.4.0.tar` & `chlorophyll-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:22.995867 chlorophyll-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-12 14:24:22.991866 chlorophyll-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:22.991866 chlorophyll-0.4.0/chlorophyll/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/codeview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:22.991866 chlorophyll-0.4.0/chlorophyll/colorschemes/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/ayu-dark.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/ayu-light.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/dracula.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/mariana.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/colorschemes/monokai.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/chlorophyll/schemeparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:22.991866 chlorophyll-0.4.0/chlorophyll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 14:24:22.000000 chlorophyll-0.4.0/chlorophyll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:24:22.995867 chlorophyll-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-12 14:24:11.000000 chlorophyll-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/chlorophyll/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/codeview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/chlorophyll/colorschemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/ayu-dark.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/ayu-light.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/dracula.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/mariana.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/monokai.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/schemeparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/chlorophyll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/setup.py
```

### Comparing `chlorophyll-0.4.0/LICENSE` & `chlorophyll-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.0/PKG-INFO` & `chlorophyll-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.4.0
+Version: 0.4.1
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
 Home-page: https://gitlab.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `chlorophyll-0.4.0/README.md` & `chlorophyll-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.0/chlorophyll/codeview.py` & `chlorophyll-0.4.1/chlorophyll/codeview.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from contextlib import suppress
 from pathlib import Path
 from tkinter import BaseWidget, Event, Misc, TclError, Text, ttk
 from tkinter.font import Font
 from typing import Any, Callable, Type, Union
 
 import pygments
+import pygments.lexer
 import pygments.lexers
 import toml
 from pyperclip import copy
 from tklinenums import TkLineNumbers
 
 from .schemeparser import _parse_scheme
```

### Comparing `chlorophyll-0.4.0/chlorophyll/colorschemes/ayu-dark.toml` & `chlorophyll-0.4.1/chlorophyll/colorschemes/ayu-dark.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.0/chlorophyll/colorschemes/ayu-light.toml` & `chlorophyll-0.4.1/chlorophyll/colorschemes/ayu-light.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.0/chlorophyll/colorschemes/dracula.toml` & `chlorophyll-0.4.1/chlorophyll/colorschemes/dracula.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.0/chlorophyll/colorschemes/mariana.toml` & `chlorophyll-0.4.1/chlorophyll/colorschemes/mariana.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.0/chlorophyll/colorschemes/monokai.toml` & `chlorophyll-0.4.1/chlorophyll/colorschemes/monokai.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.0/chlorophyll/schemeparser.py` & `chlorophyll-0.4.1/chlorophyll/schemeparser.py`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.0/chlorophyll.egg-info/PKG-INFO` & `chlorophyll-0.4.1/chlorophyll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.4.0
+Version: 0.4.1
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
 Home-page: https://gitlab.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `chlorophyll-0.4.0/setup.py` & `chlorophyll-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 
 setup(
     name="chlorophyll",
-    version="0.4.0",
+    version="0.4.1",
     description="A module that fills your code with color - syntax highlighted text box widget for Tkinter.",
     author="rdbende",
     author_email="rdbende@gmail.com",
     url="https://gitlab.com/rdbende/chlorophyll",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["pygments", "toml", "tklinenums", "pyperclip"],
```

