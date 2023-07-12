# Comparing `tmp/fire_opal-5.2.2.tar.gz` & `tmp/fire_opal-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fire_opal-5.2.2.tar", max compression
+gzip compressed data, was "fire_opal-5.3.0.tar", max compression
```

## Comparing `fire_opal-5.2.2.tar` & `fire_opal-5.3.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0    36653 2023-06-05 06:17:36.114984 fire_opal-5.2.2/LICENSE
--rw-r--r--   0        0        0      524 2023-06-05 06:17:36.114984 fire_opal-5.2.2/README.md
--rw-r--r--   0        0        0      743 2023-06-05 06:17:54.407271 fire_opal-5.2.2/fireopal/__init__.py
--rw-r--r--   0        0        0      697 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/admin.py
--rw-r--r--   0        0        0     3298 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/config.py
--rw-r--r--   0        0        0      869 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/constants.py
--rw-r--r--   0        0        0      891 2023-06-05 06:17:54.407271 fire_opal-5.2.2/fireopal/functions/__init__.py
--rw-r--r--   0        0        0      818 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/base.py
--rw-r--r--   0        0        0     1478 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/benchmark.py
--rw-r--r--   0        0        0     2711 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/create_calibration_data.py
--rw-r--r--   0        0        0     1435 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/create_mitigation_data.py
--rw-r--r--   0        0        0     1826 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/execute.py
--rw-r--r--   0        0        0     1140 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/read_data.py
--rw-r--r--   0        0        0     1063 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/show_supported_devices.py
--rw-r--r--   0        0        0     2247 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/solve_qaoa.py
--rw-r--r--   0        0        0     1643 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/validate.py
--rw-r--r--   0        0        0     2740 2023-06-05 06:17:54.399271 fire_opal-5.2.2/pyproject.toml
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 fire_opal-5.2.2/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-07-12 14:14:00.202212 fire_opal-5.3.0/LICENSE
+-rw-r--r--   0        0        0      532 2023-07-12 14:14:00.202212 fire_opal-5.3.0/README.md
+-rw-r--r--   0        0        0      884 2023-07-12 14:14:24.474140 fire_opal-5.3.0/fireopal/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/_utils.py
+-rw-r--r--   0        0        0      697 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/admin.py
+-rw-r--r--   0        0        0     3298 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/config.py
+-rw-r--r--   0        0        0      869 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/constants.py
+-rw-r--r--   0        0        0      835 2023-07-12 14:14:24.470140 fire_opal-5.3.0/fireopal/credentials/__init__.py
+-rw-r--r--   0        0        0     3345 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/credentials/_credentials.py
+-rw-r--r--   0        0        0      891 2023-07-12 14:14:24.474140 fire_opal-5.3.0/fireopal/functions/__init__.py
+-rw-r--r--   0        0        0      818 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/base.py
+-rw-r--r--   0        0        0     1478 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/benchmark.py
+-rw-r--r--   0        0        0     2711 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/create_calibration_data.py
+-rw-r--r--   0        0        0     1435 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/create_mitigation_data.py
+-rw-r--r--   0        0        0     2029 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/execute.py
+-rw-r--r--   0        0        0     1140 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/read_data.py
+-rw-r--r--   0        0        0     1276 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/show_supported_devices.py
+-rw-r--r--   0        0        0     2315 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/solve_qaoa.py
+-rw-r--r--   0        0        0     1702 2023-07-12 14:14:00.206212 fire_opal-5.3.0/fireopal/functions/validate.py
+-rw-r--r--   0        0        0     2771 2023-07-12 14:14:24.458140 fire_opal-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 fire_opal-5.3.0/PKG-INFO
```

### Comparing `fire_opal-5.2.2/LICENSE` & `fire_opal-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/__init__.py` & `fire_opal-5.3.0/fireopal/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,26 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
+__version__ = "5.3.0"
+
+from . import credentials
+from ._utils import print_package_versions
 from .functions import (
     execute,
     show_supported_devices,
     solve_qaoa,
     validate,
 )
 
 __all__ = [
+    "credentials",
     "execute",
     "show_supported_devices",
     "solve_qaoa",
     "validate",
+    "print_package_versions",
 ]
```

### Comparing `fire_opal-5.2.2/fireopal/admin.py` & `fire_opal-5.3.0/fireopal/admin.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/config.py` & `fire_opal-5.3.0/fireopal/config.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/constants.py` & `fire_opal-5.3.0/fireopal/constants.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/functions/__init__.py` & `fire_opal-5.3.0/fireopal/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/functions/base.py` & `fire_opal-5.3.0/fireopal/functions/base.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/functions/benchmark.py` & `fire_opal-5.3.0/fireopal/functions/benchmark.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/functions/create_calibration_data.py` & `fire_opal-5.3.0/fireopal/functions/create_calibration_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/functions/create_mitigation_data.py` & `fire_opal-5.3.0/fireopal/functions/create_mitigation_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/functions/execute.py` & `fire_opal-5.3.0/fireopal/functions/validate.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,51 +8,49 @@
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 from typing import (
-    Any,
     Dict,
     List,
 )
 
 from qctrlclient.core import print_warnings
 
+from fireopal.credentials import Credentials
+
 from .base import fire_opal_workflow
 
 
-@fire_opal_workflow("compile_and_run_workflow", formatter=print_warnings)
-def execute(
+@fire_opal_workflow("validate_input_circuits_workflow", formatter=print_warnings)
+def validate(
     circuits: List[str],
-    shot_count: int,
-    credentials: Dict[str, Any],
+    credentials: Credentials,
     backend_name: str,
 ) -> Dict:
     """
-    Execute a batch of `circuits` where `shot_count` measurements are taken per circuit.
+    Validate the compatibility of a batch of circuits for Fire Opal.
 
     Parameters
     ----------
     circuits : List[str]
-        A list of quantum circuits in the form of a QASM strings. You may use Qiskit to
+        A list of quantum circuit in the form QASM string. You can use Qiskit to
         generate these strings.
-    shot_count : int
-        Number of bitstrings that are sampled from the final quantum state.
-    credentials : Dict[str, Any]
-        The credentials for running circuits on an IBM backend. This dictionary should
-        contain key-value entries with keys `token`, `project`, `hub`, and `group`.
+    credentials : Credentials
+        The credentials for running circuits on an IBM backend.
+        Use the `make_credentials_for_ibmq` function from the `credentials` module
+        to generate properly formatted credentials.
     backend_name : str
-        The backend device name that should be used to run circuits.
+        The backend device name that will be used to run circuits after validation.
 
     Returns
     -------
     Dict
-        A dictionary containing probability mass functions and warnings.
+        The output of the validate workflow.
     """
     return {
         "circuits": circuits,
-        "shot_count": shot_count,
         "credentials": credentials,
         "backend_name": backend_name,
     }
```

### Comparing `fire_opal-5.2.2/fireopal/functions/read_data.py` & `fire_opal-5.3.0/fireopal/functions/read_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.2/fireopal/functions/solve_qaoa.py` & `fire_opal-5.3.0/fireopal/functions/solve_qaoa.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,37 +17,40 @@
     Optional,
 )
 
 import networkx as nx
 from qctrlclient.core import print_warnings
 from sympy import Expr
 
+from fireopal.credentials import Credentials
+
 from .base import fire_opal_workflow
 
 
 @fire_opal_workflow("solve_qaoa_workflow", formatter=print_warnings)
 def solve_qaoa(
     problem: Expr | nx.Graph,
     problem_type: str,
-    credentials: Dict[str, str],
+    credentials: Credentials,
     backend_name: Optional[str] = None,
 ) -> Dict:
     """
     Solve a QAOA problem.
 
     Parameters
     ----------
     problem : Expr or nx.Graph
         The QAOA problem definition, represented as either an
         `nx.Graph` or `sympy.Expr`.
     problem_type : str
         The class of QAOA problem to solve.
-    credentials : Dict[str, str]
-        The credentials for running circuits on an IBM backend. This dictionary should
-        contain key-value entries with keys `token`, `project`, `hub`, and `group`.
+    credentials : Credentials
+        The credentials for running circuits on an IBM backend.
+        Use the `make_credentials_for_ibmq` function from the `credentials` module
+        to generate properly formatted credentials.
     backend_name : str, optional
         The backend device that should be used to run circuits. Defaults to None.
 
     Returns
     -------
     Dict
         The output of the solve qaoa workflow.
```

### Comparing `fire_opal-5.2.2/fireopal/functions/validate.py` & `fire_opal-5.3.0/fireopal/functions/show_supported_devices.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,48 +7,37 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-from typing import (
-    Any,
-    Dict,
-    List,
-)
+
+from typing import Dict
 
 from qctrlclient.core import print_warnings
 
+from fireopal.credentials import Credentials
+
 from .base import fire_opal_workflow
 
 
-@fire_opal_workflow("validate_input_circuits_workflow", formatter=print_warnings)
-def validate(
-    circuits: List[str],
-    credentials: Dict[str, Any],
-    backend_name: str,
-) -> Dict:
+@fire_opal_workflow("show_supported_devices_workflow", formatter=print_warnings)
+def show_supported_devices(credentials: Credentials) -> Dict:
     """
-    Validate the compatibility of a batch of circuits for Fire Opal.
+    Shows the current supported devices for Fire Opal.
 
     Parameters
     ----------
-    circuits : List[str]
-        A list of quantum circuit in the form QASM string. You can use Qiskit to
-        generate these strings.
-    credentials : Dict[str, Any]
-        The credentials for running circuits on an IBM backend. This dictionary should
-        contain key-value entries with keys `token`, `project`, `hub`, and `group`.
-    backend_name : str
-        The backend device name that will be used to run circuits after validation.
+    credentials : Credentials
+        The hardware provider credentials. See the `credentials` module
+        for functions to generate credentials for your desired provider.
 
     Returns
     -------
     Dict
-        The output of the validate workflow.
+        The output of the show supported devices workflow.
     """
+
     return {
-        "circuits": circuits,
         "credentials": credentials,
-        "backend_name": backend_name,
     }
```

### Comparing `fire_opal-5.2.2/pyproject.toml` & `fire_opal-5.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fire-opal"
-version = "5.2.2"
+version = "5.3.0"
 description = "Fire Opal Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -69,14 +69,16 @@
 [[tool.poetry.source]]
 name = "Q-CTRL PyPI"
 url = "https://pypi.q-ctrl.com/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
+tomli = "^2.0.1"
+importlib-metadata = "^4.13.0"
 qctrl-client = "^7.0.0"
 click = "^8.1.0"
 qctrl-commons = "^18.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
@@ -86,15 +88,14 @@
 pylint_runner = "^0.6.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pre-commit = "^3.3.1"
 qctrl-core-workflow-manager = "^2.0.0"
 sphinx = "^5.3.0"
-tomli = "^2.0.1"
 qctrl-sphinx-theme = "~0.1.3"
 
 [tool.black]
 exclude = '''
 (
     /(
         docs
```

### Comparing `fire_opal-5.2.2/PKG-INFO` & `fire_opal-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fire-opal
-Version: 5.2.2
+Version: 5.3.0
 Summary: Fire Opal Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -28,25 +28,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: click (>=8.1.0,<9.0.0)
+Requires-Dist: importlib-metadata (>=4.13.0,<5.0.0)
 Requires-Dist: qctrl-client (>=7.0.0,<8.0.0)
 Requires-Dist: qctrl-commons (>=18.0.0,<19.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
 Description-Content-Type: text/markdown
 
 # Fire Opal Client
 
-The Fire Opal Client package is a Python client for Q-CTRL's Fire Opal product.
-Fire Opal is a simple and powerful package for algorithm developers and quantum computer end users.
-By applying a complete suite of error suppression techniques, Fire Opal automatically reduces error and vastly improves the quality of quantum algorithm results. This often transforms quantum computer outputs from random to useful.
+The Fire Opal Client package is a Python client for Q-CTRL's Fire Opal product. Fire Opal is a simple and powerful package for algorithm developers and quantum computer end users. By applying a complete suite of error suppression techniques, Fire Opal automatically reduces error and vastly improves the quality of quantum algorithm results. This often transforms quantum computer outputs from random to useful.
 
-Please see how you can [get started](https://docs.q-ctrl.com/fire-opal/get-started) today.
+See how you can [get started with Fire Opal](https://docs.q-ctrl.com/fire-opal/get-started) today.
```

