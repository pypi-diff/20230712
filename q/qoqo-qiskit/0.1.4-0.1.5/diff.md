# Comparing `tmp/qoqo_qiskit-0.1.4.tar.gz` & `tmp/qoqo_qiskit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoqo_qiskit-0.1.4.tar", last modified: Thu Jun  1 09:22:37 2023, max compression
+gzip compressed data, was "qoqo_qiskit-0.1.5.tar", last modified: Wed Jul 12 15:13:53 2023, max compression
```

## Comparing `qoqo_qiskit-0.1.4.tar` & `qoqo_qiskit-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.945057 qoqo_qiskit-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.945057 qoqo_qiskit-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.945057 qoqo_qiskit-0.1.4/src/qoqo_qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.945057 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 09:22:37.000000 qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/backend/test_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:22:37.949056 qoqo_qiskit-0.1.4/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-01 09:22:18.000000 qoqo_qiskit-0.1.4/tests/interface/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.698480 qoqo_qiskit-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.698480 qoqo_qiskit-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/src/qoqo_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/src/qoqo_qiskit/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit/backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/src/qoqo_qiskit/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit/interface/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/src/qoqo_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-07-12 15:13:53.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-12 15:13:53.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:13:53.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-12 15:13:53.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 15:13:53.000000 qoqo_qiskit-0.1.5/src/qoqo_qiskit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/tests/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/tests/backend/test_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:13:53.702480 qoqo_qiskit-0.1.5/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/tests/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-12 15:13:38.000000 qoqo_qiskit-0.1.5/tests/interface/test_interface.py
```

### Comparing `qoqo_qiskit-0.1.4/LICENSE` & `qoqo_qiskit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/PKG-INFO` & `qoqo_qiskit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_qiskit
-Version: 0.1.4
+Version: 0.1.5
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,15 +201,15 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src="../qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
```

### Comparing `qoqo_qiskit-0.1.4/README.md` & `qoqo_qiskit-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/docs/Makefile` & `qoqo_qiskit-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/docs/conf.py` & `qoqo_qiskit-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/pyproject.toml` & `qoqo_qiskit-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "qoqo_qiskit"
-version = "0.1.4"
+version = "0.1.5"
 license = {file="LICENSE"}
 authors = [
     {name="HQS Quantum Simulation GmbH", email="info@quantumsimulations.de"}
 ]
 maintainers = [
     {name="Matteo Lodi", email="matteo.lodi@quantumsimulations.de"}
 ]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
-    "qoqo>=1.4",
-    "qoqo_qasm>=0.7",
+    "qoqo>=1.5",
+    "qoqo_qasm>=0.8",
     "qiskit",
     "numpy"
 ]
 
 [project.optional-dependencies]
 tests = [
   'pytest',
@@ -27,15 +27,16 @@
     'flake8',
     'flake8-bugbear',
     'flake8-pyproject',
     'flake8-pydocstyle',
     'darglint',
     'bandit',
     'mypy',
-    'black'
+    'black',
+    'ruff',
 ]
 docs = [
     'sphinx>=2.1',
     'nbsphinx',
     'pygments',
     'recommonmark',
     'myst_parser',
```

### Comparing `qoqo_qiskit-0.1.4/src/qoqo_qiskit/__init__.py` & `qoqo_qiskit-0.1.5/src/qoqo_qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/__init__.py` & `qoqo_qiskit-0.1.5/src/qoqo_qiskit/backend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 """Qoqo-qiskit backend package for compatibility and simulation purposes."""
 
 
 from qoqo_qiskit.backend.backend import QoqoQiskitBackend
 
-__all__ = "QoqoQiskitBackend"
+__all__ = ["QoqoQiskitBackend"]
```

### Comparing `qoqo_qiskit-0.1.4/src/qoqo_qiskit/backend/backend.py` & `qoqo_qiskit-0.1.5/src/qoqo_qiskit/backend/backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,46 +66,20 @@
             Tuple[Dict[str, List[List[bool]]],\
                   Dict[str, List[List[float]]],\
                   Dict[str, List[List[complex]]]]: bit, float and complex registers dictionaries.
 
         Raises:
             ValueError: the Circuit does not contain Measurement operations
         """
-        clas_regs_sizes: Dict[str, int] = dict()
-
-        # Initializing the classical registers for calculation and output
-        internal_bit_register_dict: Dict[str, List[bool]] = dict()
-        internal_float_register_dict: Dict[str, List[float]] = dict()
-        internal_complex_register_dict: Dict[str, List[complex]] = dict()
-
-        output_bit_register_dict: Dict[str, List[List[bool]]] = dict()
-        output_float_register_dict: Dict[str, List[List[float]]] = dict()
-        output_complex_register_dict: Dict[str, List[List[complex]]] = dict()
-
-        for bit_def in circuit.filter_by_tag("DefinitionBit"):
-            internal_bit_register_dict[bit_def.name()] = [False for _ in range(bit_def.length())]
-            clas_regs_sizes[bit_def.name()] = bit_def.length()
-            if bit_def.is_output():
-                output_bit_register_dict[bit_def.name()] = list()
-
-        for float_def in circuit.filter_by_tag("DefinitionFloat"):
-            internal_float_register_dict[float_def.name()] = [
-                0.0 for _ in range(float_def.length())
-            ]
-            if float_def.is_output():
-                output_float_register_dict[float_def.name()] = cast(List[List[float]], list())
-
-        for complex_def in circuit.filter_by_tag("DefinitionComplex"):
-            internal_complex_register_dict[complex_def.name()] = [
-                complex(0.0) for _ in range(complex_def.length())
-            ]
-            if complex_def.is_output():
-                output_complex_register_dict[complex_def.name()] = cast(
-                    List[List[complex]], list()
-                )
+        (
+            clas_regs_sizes,
+            output_bit_register_dict,
+            output_float_register_dict,
+            output_complex_register_dict,
+        ) = self._setup_registers(circuit)
 
         # Qiskit conversion
         res = to_qiskit_circuit(circuit)
         compiled_circuit: QuantumCircuit = res[0]
         run_options: Dict[str, Any] = res[1]
 
         # Raise ValueError:
@@ -155,36 +129,26 @@
 
         # Simulation
         result = execute(
             compiled_circuit, self.qiskit_backend, shots=shots, memory=self.memory
         ).result()
 
         # Result transformation
-        if sim_type == "automatic":
-            if self.memory:
-                transformed_counts = self._counts_to_registers(
-                    result.get_memory(), True, clas_regs_sizes
-                )
-            else:
-                transformed_counts = self._counts_to_registers(
-                    result.get_counts(), False, clas_regs_sizes
-                )
-            for id, reg in enumerate(output_bit_register_dict):
-                reversed_list = []
-                for shot in transformed_counts[id]:
-                    reversed_list.append(shot[::-1])
-                output_bit_register_dict[reg] = reversed_list
-        elif sim_type == "statevector":
-            vector = list(np.asarray(result.data(0)["statevector"]).flatten())
-            for reg in output_complex_register_dict:
-                output_complex_register_dict[reg].append(vector)
-        elif sim_type == "density_matrix":
-            vector = list(np.asarray(result.data(0)["density_matrix"]).flatten())
-            for reg in output_complex_register_dict:
-                output_complex_register_dict[reg].append(vector)
+        (
+            output_bit_register_dict,
+            output_float_register_dict,
+            output_complex_register_dict,
+        ) = self._transform_result(
+            sim_type,
+            result,
+            clas_regs_sizes,
+            output_bit_register_dict,
+            output_float_register_dict,
+            output_complex_register_dict,
+        )
 
         return (
             output_bit_register_dict,
             output_float_register_dict,
             output_complex_register_dict,
         )
 
@@ -202,17 +166,17 @@
 
         Returns:
             Tuple[Dict[str, List[List[bool]]],\
                   Dict[str, List[List[float]]],\
                   Dict[str, List[List[complex]]]]
         """
         constant_circuit = measurement.constant_circuit()
-        output_bit_register_dict: Dict[str, List[List[bool]]] = dict()
-        output_float_register_dict: Dict[str, List[List[float]]] = dict()
-        output_complex_register_dict: Dict[str, List[List[complex]]] = dict()
+        output_bit_register_dict: Dict[str, List[List[bool]]] = {}
+        output_float_register_dict: Dict[str, List[List[float]]] = {}
+        output_complex_register_dict: Dict[str, List[List[complex]]] = {}
 
         for circuit in measurement.circuits():
             if constant_circuit is None:
                 run_circuit = circuit
             else:
                 run_circuit = constant_circuit + circuit
 
@@ -260,25 +224,25 @@
         reg_num = 0
         for key in clas_regs_sizes:
             reg_num += clas_regs_sizes[key]
         for _ in range(reg_num):
             bit_map.append([])
         for key in counts:
             splitted = self._split(key, clas_regs_sizes)
-            for id, measurement in enumerate(splitted):
+            for i, measurement in enumerate(splitted):
                 transf_measurement = self._bit_to_bool(measurement)
                 if mem:
-                    bit_map[id].append(transf_measurement)
+                    bit_map[i].append(transf_measurement)
                 else:
                     for _ in range(counts[key]):
-                        bit_map[id].append(transf_measurement)
+                        bit_map[i].append(transf_measurement)
         return bit_map
 
-    def _are_measurement_operations_in(self, input: Circuit) -> bool:
-        for op in input:
+    def _are_measurement_operations_in(self, circuit: Circuit) -> bool:
+        for op in circuit:
             if "Measurement" in op.tags():
                 return True
         return False
 
     def _bit_to_bool(self, element: str) -> List[bool]:
         ret = []
         for char in element:
@@ -293,7 +257,92 @@
         else:
             element = element[::-1]
             for key in clas_regs_sizes:
                 splitted.append(element[: clas_regs_sizes[key] :])
                 splitted[-1] = splitted[-1][::-1]
                 element = element[clas_regs_sizes[key] :]
         return splitted
+
+    def _setup_registers(
+        self, circuit: Circuit
+    ) -> Tuple[
+        Dict[str, int],
+        Dict[str, List[List[bool]]],
+        Dict[str, List[List[float]]],
+        Dict[str, List[List[complex]]],
+    ]:
+        clas_regs_sizes: Dict[str, int] = {}
+
+        # Initializing the classical registers for calculation and output
+        internal_bit_register_dict: Dict[str, List[bool]] = {}
+        internal_float_register_dict: Dict[str, List[float]] = {}
+        internal_complex_register_dict: Dict[str, List[complex]] = {}
+
+        output_bit_register_dict: Dict[str, List[List[bool]]] = {}
+        output_float_register_dict: Dict[str, List[List[float]]] = {}
+        output_complex_register_dict: Dict[str, List[List[complex]]] = {}
+
+        for bit_def in circuit.filter_by_tag("DefinitionBit"):
+            internal_bit_register_dict[bit_def.name()] = [False for _ in range(bit_def.length())]
+            clas_regs_sizes[bit_def.name()] = bit_def.length()
+            if bit_def.is_output():
+                output_bit_register_dict[bit_def.name()] = []
+        for float_def in circuit.filter_by_tag("DefinitionFloat"):
+            internal_float_register_dict[float_def.name()] = [
+                0.0 for _ in range(float_def.length())
+            ]
+            if float_def.is_output():
+                output_float_register_dict[float_def.name()] = cast(List[List[float]], [])
+        for complex_def in circuit.filter_by_tag("DefinitionComplex"):
+            internal_complex_register_dict[complex_def.name()] = [
+                complex(0.0) for _ in range(complex_def.length())
+            ]
+            if complex_def.is_output():
+                output_complex_register_dict[complex_def.name()] = cast(List[List[complex]], [])
+        return (
+            clas_regs_sizes,
+            output_bit_register_dict,
+            output_float_register_dict,
+            output_complex_register_dict,
+        )
+
+    def _transform_result(
+        self,
+        sim_type: str,
+        result: Any,
+        clas_regs_sizes: Dict[str, int],
+        output_bit_register_dict: Dict[str, List[List[bool]]],
+        _output_float_register_dict: Dict[str, List[List[float]]],
+        output_complex_register_dict: Dict[str, List[List[complex]]],
+    ) -> Tuple[
+        Dict[str, List[List[bool]]],
+        Dict[str, List[List[float]]],
+        Dict[str, List[List[complex]]],
+    ]:
+        if sim_type == "automatic":
+            if self.memory:
+                transformed_counts = self._counts_to_registers(
+                    result.get_memory(), True, clas_regs_sizes
+                )
+            else:
+                transformed_counts = self._counts_to_registers(
+                    result.get_counts(), False, clas_regs_sizes
+                )
+            for i, reg in enumerate(output_bit_register_dict):
+                reversed_list = []
+                for shot in transformed_counts[i]:
+                    reversed_list.append(shot[::-1])
+                output_bit_register_dict[reg] = reversed_list
+        elif sim_type == "statevector":
+            vector = list(np.asarray(result.data(0)["statevector"]).flatten())
+            for reg in output_complex_register_dict:
+                output_complex_register_dict[reg].append(vector)
+        elif sim_type == "density_matrix":
+            vector = list(np.asarray(result.data(0)["density_matrix"]).flatten())
+            for reg in output_complex_register_dict:
+                output_complex_register_dict[reg].append(vector)
+
+        return (
+            output_bit_register_dict,
+            _output_float_register_dict,
+            output_complex_register_dict,
+        )
```

### Comparing `qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/__init__.py` & `qoqo_qiskit-0.1.5/src/qoqo_qiskit/interface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 """Qiskit interface for qoqo circuits."""
 
 
 from qoqo_qiskit.interface.interface import to_qiskit_circuit
 
-__all__ = "to_qiskit_circuit"
+__all__ = ["to_qiskit_circuit"]
```

### Comparing `qoqo_qiskit-0.1.4/src/qoqo_qiskit/interface/interface.py` & `qoqo_qiskit-0.1.5/src/qoqo_qiskit/interface/interface.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/PKG-INFO` & `qoqo_qiskit-0.1.5/src/qoqo_qiskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo-qiskit
-Version: 0.1.4
+Version: 0.1.5
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,15 +201,15 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src="../qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
```

### Comparing `qoqo_qiskit-0.1.4/src/qoqo_qiskit.egg-info/SOURCES.txt` & `qoqo_qiskit-0.1.5/src/qoqo_qiskit.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 docs/Makefile
 docs/conf.py
 docs/index.rst
-docs/modules.rst
 src/qoqo_qiskit/__init__.py
 src/qoqo_qiskit.egg-info/PKG-INFO
 src/qoqo_qiskit.egg-info/SOURCES.txt
 src/qoqo_qiskit.egg-info/dependency_links.txt
 src/qoqo_qiskit.egg-info/requires.txt
 src/qoqo_qiskit.egg-info/top_level.txt
 src/qoqo_qiskit/backend/__init__.py
```

### Comparing `qoqo_qiskit-0.1.4/tests/__init__.py` & `qoqo_qiskit-0.1.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/tests/backend/__init__.py` & `qoqo_qiskit-0.1.5/tests/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/tests/backend/test_backend.py` & `qoqo_qiskit-0.1.5/tests/backend/test_backend.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/tests/interface/__init__.py` & `qoqo_qiskit-0.1.5/tests/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.4/tests/interface/test_interface.py` & `qoqo_qiskit-0.1.5/tests/interface/test_interface.py`

 * *Files identical despite different names*

