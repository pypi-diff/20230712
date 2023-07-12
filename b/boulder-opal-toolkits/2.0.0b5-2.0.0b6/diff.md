# Comparing `tmp/boulder_opal_toolkits-2.0.0b5.tar.gz` & `tmp/boulder_opal_toolkits-2.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boulder_opal_toolkits-2.0.0b5.tar", max compression
+gzip compressed data, was "boulder_opal_toolkits-2.0.0b6.tar", max compression
```

## Comparing `boulder_opal_toolkits-2.0.0b5.tar` & `boulder_opal_toolkits-2.0.0b6.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0    36653 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/LICENSE
--rw-r--r--   0        0        0       95 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/README.md
--rwxr-xr-x   0        0        0     1107 2023-03-30 01:37:03.098121 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/__init__.py
--rw-r--r--   0        0        0      550 2023-03-30 01:37:03.098121 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/closed_loop/__init__.py
--rw-r--r--   0        0        0    26928 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/closed_loop/functions.py
--rw-r--r--   0        0        0      550 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/closed_loop/nodes.py
--rw-r--r--   0        0        0      550 2023-03-30 01:37:03.102120 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/deprecated/__init__.py
--rw-r--r--   0        0        0     1316 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/deprecated/deprecate_utils.py
--rw-r--r--   0        0        0      643 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/deprecated/functions.py
--rw-r--r--   0        0        0      639 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/deprecated/nodes.py
--rw-r--r--   0        0        0      550 2023-03-30 01:37:03.098121 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/ions/__init__.py
--rw-r--r--   0        0        0    39744 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/ions/functions.py
--rw-r--r--   0        0        0     5035 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/namespace.py
--rw-r--r--   0        0        0     4788 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/registry.py
--rw-r--r--   0        0        0      550 2023-03-30 01:37:03.106120 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/__init__.py
--rw-r--r--   0        0        0    33447 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/functions.py
--rw-r--r--   0        0        0    60465 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/pwc_nodes.py
--rw-r--r--   0        0        0     1656 2023-03-30 01:36:47.562166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/signal_utils.py
--rw-r--r--   0        0        0    23975 2023-03-30 01:36:47.566166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/stf_nodes.py
--rw-r--r--   0        0        0      550 2023-03-30 01:37:03.094120 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/superconducting/__init__.py
--rw-r--r--   0        0        0    56080 2023-03-30 01:36:47.566166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/superconducting/functions.py
--rw-r--r--   0        0        0      550 2023-03-30 01:36:47.566166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/superconducting/nodes.py
--rw-r--r--   0        0        0     9307 2023-03-30 01:36:47.566166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/toolkit_utils.py
--rwxr-xr-x   0        0        0      550 2023-03-30 01:37:03.102120 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/utils/__init__.py
--rw-r--r--   0        0        0    16789 2023-03-30 01:36:47.566166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/utils/functions.py
--rw-r--r--   0        0        0     8580 2023-03-30 01:36:47.566166 boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/utils/nodes.py
--rw-r--r--   0        0        0     2658 2023-03-30 01:37:03.082121 boulder_opal_toolkits-2.0.0b5/pyproject.toml
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 boulder_opal_toolkits-2.0.0b5/setup.py
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 boulder_opal_toolkits-2.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/LICENSE
+-rw-r--r--   0        0        0      570 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/README.md
+-rwxr-xr-x   0        0        0     1107 2023-07-12 05:34:46.139327 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/__init__.py
+-rw-r--r--   0        0        0      550 2023-07-12 05:34:46.143328 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/closed_loop/__init__.py
+-rw-r--r--   0        0        0    26928 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/closed_loop/functions.py
+-rw-r--r--   0        0        0      550 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/closed_loop/nodes.py
+-rw-r--r--   0        0        0      550 2023-07-12 05:34:46.135327 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/deprecated/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/deprecated/deprecate_utils.py
+-rw-r--r--   0        0        0      643 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/deprecated/functions.py
+-rw-r--r--   0        0        0      639 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/deprecated/nodes.py
+-rw-r--r--   0        0        0      550 2023-07-12 05:34:46.139327 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/ions/__init__.py
+-rw-r--r--   0        0        0    39744 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/ions/functions.py
+-rw-r--r--   0        0        0     5035 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/namespace.py
+-rw-r--r--   0        0        0     4788 2023-07-12 05:34:23.258657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/registry.py
+-rw-r--r--   0        0        0      550 2023-07-12 05:34:46.135327 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/__init__.py
+-rw-r--r--   0        0        0    33447 2023-07-12 05:34:23.262657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/functions.py
+-rw-r--r--   0        0        0    60465 2023-07-12 05:34:23.262657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/pwc_nodes.py
+-rw-r--r--   0        0        0     1656 2023-07-12 05:34:23.262657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/signal_utils.py
+-rw-r--r--   0        0        0    23975 2023-07-12 05:34:23.262657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/stf_nodes.py
+-rw-r--r--   0        0        0      550 2023-07-12 05:34:46.131327 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/superconducting/__init__.py
+-rw-r--r--   0        0        0    56080 2023-07-12 05:34:23.262657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/superconducting/functions.py
+-rw-r--r--   0        0        0      550 2023-07-12 05:34:23.262657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/superconducting/nodes.py
+-rw-r--r--   0        0        0     9307 2023-07-12 05:34:23.262657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/toolkit_utils.py
+-rwxr-xr-x   0        0        0      550 2023-07-12 05:34:46.135327 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/utils/__init__.py
+-rw-r--r--   0        0        0    16789 2023-07-12 05:34:23.262657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/utils/functions.py
+-rw-r--r--   0        0        0     8580 2023-07-12 05:34:23.262657 boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/utils/nodes.py
+-rw-r--r--   0        0        0     2651 2023-07-12 05:34:46.123326 boulder_opal_toolkits-2.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 boulder_opal_toolkits-2.0.0b6/PKG-INFO
```

### Comparing `boulder_opal_toolkits-2.0.0b5/LICENSE` & `boulder_opal_toolkits-2.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/__init__.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """boulderopaltoolkits - a toolkit library for Boulder Opal."""
 
-__version__ = "2.0.0-beta.5"
+__version__ = "2.0.0-beta.6"
 __author__ = "Q-CTRL <support@q-ctrl.com>"
 
 from boulderopaltoolkits.namespace import (
     TOOLKIT_MAIN_DOC,
     Namespace,
 )
 from boulderopaltoolkits.registry import (
```

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/closed_loop/__init__.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/closed_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/closed_loop/functions.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/closed_loop/functions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/closed_loop/nodes.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/closed_loop/nodes.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/deprecated/__init__.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/deprecated/deprecate_utils.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/deprecated/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/deprecated/functions.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/deprecated/functions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/deprecated/nodes.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/deprecated/nodes.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/ions/__init__.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/ions/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/ions/functions.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/ions/functions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/namespace.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/namespace.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/registry.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/registry.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/__init__.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/functions.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/functions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/pwc_nodes.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/pwc_nodes.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/signal_utils.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/signal_utils.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/signals/stf_nodes.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/signals/stf_nodes.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/superconducting/__init__.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/superconducting/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/superconducting/functions.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/superconducting/functions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/superconducting/nodes.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/superconducting/nodes.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/toolkit_utils.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/toolkit_utils.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/utils/__init__.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/utils/functions.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/utils/functions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/boulderopaltoolkits/utils/nodes.py` & `boulder_opal_toolkits-2.0.0b6/boulderopaltoolkits/utils/nodes.py`

 * *Files identical despite different names*

### Comparing `boulder_opal_toolkits-2.0.0b5/pyproject.toml` & `boulder_opal_toolkits-2.0.0b6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "boulder-opal-toolkits"
-version = "2.0.0-beta.5"
-description = "Q-CTRL Boulder Opal Toolkits"
+version = "2.0.0-beta.6"
+description = "Boulder Opal Toolkits"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
 documentation = ""
@@ -61,25 +61,25 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 numpy = "^1.23.5"
 scipy = ">=1.9.3"
 python-forge = "^18.6.0"
-qctrl-commons = "^18.0.0"
+qctrl-commons = "^19.1.0"
 numpydoc = "^1.5.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 lemminflect = "^0.2.2"
-mypy = "^1.1.1"
-pre-commit = "^2.9.3"
+mypy = "^1.2.0"
+pre-commit = "^3.2.2"
 pylint = "^2.17.1"
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 
 [[tool.poetry.source]]
 name = "Q-CTRL PyPI"
 url = "https://pypi.q-ctrl.com/simple"
 secondary = true
```

### Comparing `boulder_opal_toolkits-2.0.0b5/PKG-INFO` & `boulder_opal_toolkits-2.0.0b6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boulder-opal-toolkits
-Version: 2.0.0b5
-Summary: Q-CTRL Boulder Opal Toolkits
+Version: 2.0.0b6
+Summary: Boulder Opal Toolkits
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
 Maintainer-email: support@q-ctrl.com
@@ -31,20 +31,22 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: numpydoc (>=1.5.0,<2.0.0)
 Requires-Dist: python-forge (>=18.6.0,<19.0.0)
-Requires-Dist: qctrl-commons (>=18.0.0,<19.0.0)
+Requires-Dist: qctrl-commons (>=19.1.0,<20.0.0)
 Requires-Dist: scipy (>=1.9.3)
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
 Description-Content-Type: text/markdown
 
-# Q-CTRL Boulder Opal Toolkits
+# Boulder Opal Toolkits
 
-Toolkit of convenience functions and classes for Boulder Opal.
+The Boulder Opal Toolkits provide convenience nodes, classes, and functions that simplify the development in Boulder Opal. These toolkits enable you to develop and implement workflows faster and with less code, for a particular physical system or system-agnostic tasks.
+
+See the [Boulder Opal Toolkits topic](https://docs.q-ctrl.com/boulder-opal/topics/boulder-opal-toolkits) in the Boulder Opal documentation for further information. See also how you can [get started with Boulder Opal](https://docs.q-ctrl.com/boulder-opal/get-started) today.
```

