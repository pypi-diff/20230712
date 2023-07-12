# Comparing `tmp/fire_opal-5.3.0.tar.gz` & `tmp/fire_opal-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fire_opal-5.3.0.tar", max compression
+gzip compressed data, was "fire_opal-5.3.1.tar", max compression
```

## Comparing `fire_opal-5.3.0.tar` & `fire_opal-5.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    36653 2023-07-12 14:14:00.202212 fire_opal-5.3.0/LICENSE
--rw-r--r--   0        0        0      532 2023-07-12 14:14:00.202212 fire_opal-5.3.0/README.md
--rw-r--r--   0        0        0      884 2023-07-12 14:14:24.474140 fire_opal-5.3.0/fireopal/__init__.py
--rw-r--r--   0        0        0     2900 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/_utils.py
--rw-r--r--   0        0        0      697 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/admin.py
--rw-r--r--   0        0        0     3298 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/config.py
--rw-r--r--   0        0        0      869 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/constants.py
--rw-r--r--   0        0        0      835 2023-07-12 14:14:24.470140 fire_opal-5.3.0/fireopal/credentials/__init__.py
--rw-r--r--   0        0        0     3345 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/credentials/_credentials.py
--rw-r--r--   0        0        0      891 2023-07-12 14:14:24.474140 fire_opal-5.3.0/fireopal/functions/__init__.py
--rw-r--r--   0        0        0      818 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/base.py
--rw-r--r--   0        0        0     1478 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/benchmark.py
--rw-r--r--   0        0        0     2711 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/create_calibration_data.py
--rw-r--r--   0        0        0     1435 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/create_mitigation_data.py
--rw-r--r--   0        0        0     2029 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/execute.py
--rw-r--r--   0        0        0     1140 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/read_data.py
--rw-r--r--   0        0        0     1276 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/show_supported_devices.py
--rw-r--r--   0        0        0     2315 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/solve_qaoa.py
--rw-r--r--   0        0        0     1702 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/validate.py
--rw-r--r--   0        0        0     2771 2023-07-12 14:14:24.458140 fire_opal-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 fire_opal-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-07-12 16:47:11.839560 fire_opal-5.3.1/LICENSE
+-rw-r--r--   0        0        0      532 2023-07-12 16:47:11.839560 fire_opal-5.3.1/README.md
+-rw-r--r--   0        0        0      884 2023-07-12 16:47:31.987769 fire_opal-5.3.1/fireopal/__init__.py
+-rw-r--r--   0        0        0     2995 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/_utils.py
+-rw-r--r--   0        0        0      697 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/admin.py
+-rw-r--r--   0        0        0     3298 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/config.py
+-rw-r--r--   0        0        0      869 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/constants.py
+-rw-r--r--   0        0        0      835 2023-07-12 16:47:31.987769 fire_opal-5.3.1/fireopal/credentials/__init__.py
+-rw-r--r--   0        0        0     3345 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/credentials/_credentials.py
+-rw-r--r--   0        0        0      891 2023-07-12 16:47:31.991769 fire_opal-5.3.1/fireopal/functions/__init__.py
+-rw-r--r--   0        0        0      818 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/base.py
+-rw-r--r--   0        0        0     1478 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/benchmark.py
+-rw-r--r--   0        0        0     2711 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/create_calibration_data.py
+-rw-r--r--   0        0        0     1435 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/create_mitigation_data.py
+-rw-r--r--   0        0        0     2029 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/execute.py
+-rw-r--r--   0        0        0     1140 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/read_data.py
+-rw-r--r--   0        0        0     1276 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/show_supported_devices.py
+-rw-r--r--   0        0        0     2315 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/solve_qaoa.py
+-rw-r--r--   0        0        0     1702 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/validate.py
+-rw-r--r--   0        0        0     2771 2023-07-12 16:47:31.975769 fire_opal-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 fire_opal-5.3.1/PKG-INFO
```

### Comparing `fire_opal-5.3.0/LICENSE` & `fire_opal-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/README.md` & `fire_opal-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/__init__.py` & `fire_opal-5.3.1/fireopal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-__version__ = "5.3.0"
+__version__ = "5.3.1"
 
 from . import credentials
 from ._utils import print_package_versions
 from .functions import (
     execute,
     show_supported_devices,
     solve_qaoa,
```

### Comparing `fire_opal-5.3.0/fireopal/_utils.py` & `fire_opal-5.3.1/fireopal/_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -46,18 +46,22 @@
         ) as file:
             config = tomli.load(file)
             return config["tool"]["poetry"]["name"]
 
     top_level_module_names = [
         # External packages.
         "matplotlib",
+        "networkx",
         "numpy",
         "qiskit",
+        "qiskit-ibm-provider",
+        "sympy",
         # Q-CTRL packages.
         "fireopal",
+        "qctrlvisualizer",
     ]
 
     python_version = (
         f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
     )
 
     # List containing the items in the different rows.
```

### Comparing `fire_opal-5.3.0/fireopal/admin.py` & `fire_opal-5.3.1/fireopal/admin.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/config.py` & `fire_opal-5.3.1/fireopal/config.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/constants.py` & `fire_opal-5.3.1/fireopal/constants.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/credentials/__init__.py` & `fire_opal-5.3.1/fireopal/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/credentials/_credentials.py` & `fire_opal-5.3.1/fireopal/credentials/_credentials.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/__init__.py` & `fire_opal-5.3.1/fireopal/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/base.py` & `fire_opal-5.3.1/fireopal/functions/base.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/benchmark.py` & `fire_opal-5.3.1/fireopal/functions/benchmark.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/create_calibration_data.py` & `fire_opal-5.3.1/fireopal/functions/create_calibration_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/create_mitigation_data.py` & `fire_opal-5.3.1/fireopal/functions/create_mitigation_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/execute.py` & `fire_opal-5.3.1/fireopal/functions/execute.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/read_data.py` & `fire_opal-5.3.1/fireopal/functions/read_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/show_supported_devices.py` & `fire_opal-5.3.1/fireopal/functions/show_supported_devices.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/solve_qaoa.py` & `fire_opal-5.3.1/fireopal/functions/solve_qaoa.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/fireopal/functions/validate.py` & `fire_opal-5.3.1/fireopal/functions/validate.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.0/pyproject.toml` & `fire_opal-5.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fire-opal"
-version = "5.3.0"
+version = "5.3.1"
 description = "Fire Opal Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `fire_opal-5.3.0/PKG-INFO` & `fire_opal-5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fire-opal
-Version: 5.3.0
+Version: 5.3.1
 Summary: Fire Opal Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

