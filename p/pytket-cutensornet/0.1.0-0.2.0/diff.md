# Comparing `tmp/pytket_cutensornet-0.1.0-py3-none-any.whl.zip` & `tmp/pytket_cutensornet-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,18 @@
-Zip file size: 19520 bytes, number of entries: 10
--rw-r--r--  2.0 unx      989 b- defN 23-Jun-05 10:17 pytket/extensions/cutensornet/__init__.py
--rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 10:20 pytket/extensions/cutensornet/_metadata.py
--rw-r--r--  2.0 unx    26897 b- defN 23-Jun-05 10:17 pytket/extensions/cutensornet/tensor_network_convert.py
--rw-r--r--  2.0 unx      705 b- defN 23-Jun-05 10:17 pytket/extensions/cutensornet/backends/__init__.py
--rw-r--r--  2.0 unx    10462 b- defN 23-Jun-05 10:17 pytket/extensions/cutensornet/backends/cutensornet_backend.py
--rw-r--r--  2.0 unx    11356 b- defN 23-Jun-05 10:20 pytket_cutensornet-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5168 b- defN 23-Jun-05 10:20 pytket_cutensornet-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 10:20 pytket_cutensornet-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 10:20 pytket_cutensornet-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      973 b- defN 23-Jun-05 10:20 pytket_cutensornet-0.1.0.dist-info/RECORD
-10 files, 56723 bytes uncompressed, 17812 bytes compressed:  68.6%
+Zip file size: 43853 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/__init__.py
+-rw-r--r--  2.0 unx       74 b- defN 23-Jul-12 14:33 pytket/extensions/cutensornet/_metadata.py
+-rw-r--r--  2.0 unx    29214 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/tensor_network_convert.py
+-rw-r--r--  2.0 unx     2630 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/utils.py
+-rw-r--r--  2.0 unx      705 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/backends/__init__.py
+-rw-r--r--  2.0 unx    11284 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/backends/cutensornet_backend.py
+-rw-r--r--  2.0 unx     1135 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/mps/__init__.py
+-rw-r--r--  2.0 unx    31966 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/mps/mps.py
+-rw-r--r--  2.0 unx    14632 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/mps/mps_gate.py
+-rw-r--r--  2.0 unx    23867 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/mps/mps_mpo.py
+-rw-r--r--  2.0 unx     9464 b- defN 23-Jul-12 14:31 pytket/extensions/cutensornet/mps/simulation.py
+-rw-r--r--  2.0 unx    11356 b- defN 23-Jul-12 14:33 pytket_cutensornet-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5168 b- defN 23-Jul-12 14:33 pytket_cutensornet-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 14:33 pytket_cutensornet-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-12 14:33 pytket_cutensornet-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1578 b- defN 23-Jul-12 14:33 pytket_cutensornet-0.2.0.dist-info/RECORD
+16 files, 144238 bytes uncompressed, 41171 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -3,29 +3,47 @@
 
 Filename: pytket/extensions/cutensornet/_metadata.py
 Comment: 
 
 Filename: pytket/extensions/cutensornet/tensor_network_convert.py
 Comment: 
 
+Filename: pytket/extensions/cutensornet/utils.py
+Comment: 
+
 Filename: pytket/extensions/cutensornet/backends/__init__.py
 Comment: 
 
 Filename: pytket/extensions/cutensornet/backends/cutensornet_backend.py
 Comment: 
 
-Filename: pytket_cutensornet-0.1.0.dist-info/LICENSE
+Filename: pytket/extensions/cutensornet/mps/__init__.py
+Comment: 
+
+Filename: pytket/extensions/cutensornet/mps/mps.py
+Comment: 
+
+Filename: pytket/extensions/cutensornet/mps/mps_gate.py
+Comment: 
+
+Filename: pytket/extensions/cutensornet/mps/mps_mpo.py
+Comment: 
+
+Filename: pytket/extensions/cutensornet/mps/simulation.py
+Comment: 
+
+Filename: pytket_cutensornet-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_cutensornet-0.1.0.dist-info/METADATA
+Filename: pytket_cutensornet-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_cutensornet-0.1.0.dist-info/WHEEL
+Filename: pytket_cutensornet-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_cutensornet-0.1.0.dist-info/top_level.txt
+Filename: pytket_cutensornet-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_cutensornet-0.1.0.dist-info/RECORD
+Filename: pytket_cutensornet-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/extensions/cutensornet/__init__.py

```diff
@@ -19,8 +19,11 @@
 from .backends import CuTensorNetBackend
 
 from .tensor_network_convert import (
     TensorNetwork,
     PauliOperatorTensorNetwork,
     ExpectationValueTensorNetwork,
     tk_to_tensor_network,
+    measure_qubits_state,
 )
+
+from .utils import circuit_statevector_postselect
```

## pytket/extensions/cutensornet/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.1.0"
+__extension_version__ = "0.2.0"
 __extension_name__ = "pytket-cutensornet"
```

## pytket/extensions/cutensornet/tensor_network_convert.py

```diff
@@ -21,15 +21,15 @@
 import networkx as nx  # type: ignore
 from networkx.classes.reportviews import OutMultiEdgeView, OutMultiEdgeDataView  # type: ignore
 import numpy as np
 from numpy.typing import NDArray
 from pytket import Qubit  # type: ignore
 from pytket.utils import Graph
 from pytket.pauli import QubitPauliString  # type: ignore
-from pytket.circuit import Circuit
+from pytket.circuit import Circuit, Qubit  # type: ignore
 from pytket.utils import permute_rows_cols_in_unitary
 
 
 # TODO: decide whether to use logger.
 def set_logger(
     logger_name: str,
     level: int = logging.INFO,
@@ -111,16 +111,16 @@
              created.
 
         Returns:
             A map between the gate type and corresponding tensor representation(s).
 
         Note:
            The returned map values are lists and may contain more than one
-            representation - for >1-qubit gates, different topologies (e.g. upward and
-            downward) are taken into account.
+           representation - for >1-qubit gates, different topologies (e.g. upward and
+           downward) are taken into account.
         """
         name_set = {com.op.get_name() for com in self._circuit.get_commands()}
         gate_tensors = defaultdict(list)
         for i in name_set:
             for com in self._circuit.get_commands():
                 if i == com.op.get_name():
                     if adj:
@@ -181,15 +181,15 @@
 
         Args:
             adj: Whether an adjoint representation of the original circuit is to be
              created.
 
         Returns:
             List of tensors representing circuit gates (tensor network nodes) in the
-             reversed order of circuit graph nodes.
+            reversed order of circuit graph nodes.
         """
         self._gate_tensors = self._get_gate_tensors(adj=adj)
         node_tensors = []
         self._input_nodes = []
         self._output_nodes = []
         for i, node in reversed(list(enumerate(self._network.nodes(data=True)))):
             if node[1]["desc"] not in ("Input", "Output"):
@@ -257,16 +257,16 @@
         Args:
             net: Graph, representing the current circuit.
             adj: Whether an adjoint representation of the original circuit is to be
              created.
 
         Returns:
             A list of lists of tensor network nodes edges (tensors dimensions) indices
-             and a list of outward ("sticky") indices along which there will be no
-             contraction.
+            and a list of outward ("sticky") indices along which there will be no
+            contraction.
         """
         sign = -1 if adj else 1
         self._logger.debug(f"Network nodes: \n{net.nodes(data=True)}")
         self._logger.debug(f"Network edges: \n{net.edges(data=True)}")
         # There can be several identical edges for which we need different indices
         edge_indices = defaultdict(list)
         n_edges = nx.number_of_edges(net)
@@ -420,29 +420,29 @@
         The format is suitable as an input for the cuQuantum-Python `contract` function.
 
         Combines the list of tensor representations of circuit gates and corresponding
         edges indices, that must have been constructed in the same order.
 
         Returns:
             A list of interleaved tensors (ndarrays) and lists of corresponding edges
-             indices.
+            indices.
         """
         tn_interleaved = []
         for tensor, indices in zip(self._node_tensors, self._node_tensor_indices):
             tn_interleaved.append(tensor)
             tn_interleaved.append(indices)
         self._logger.debug(f"cuQuantum input list: \n{input}")
         return tn_interleaved
 
     def dagger(self) -> "TensorNetwork":
         """Constructs an adjoint of a tensor network object.
 
         Returns:
             A new TensorNetwork object, containing an adjoint representation of the
-             input object.
+            input object.
         """
         tn_dagger = TensorNetwork(self._circuit.copy(), adj=True)
         self._logger.debug(
             f"dagger cutensornet input list: \n{tn_dagger._cuquantum_interleaved}"
         )
         return tn_dagger
 
@@ -456,15 +456,15 @@
 
         Args:
             tn_other: a TensorNetwork object representing a circuit, an overlap with
              which is to be calculated.
 
         Returns:
             A tensor network in an interleaved form, representing an overlap of two
-             circuits.
+            circuits.
         """
         if set(self.sticky_indices.keys()) != set(tn_other.sticky_indices.keys()):
             raise RuntimeError("The two tensor networks are incompatible!")
         tn_other_adj = tn_other.dagger()
         i_mat = np.array([[1, 0], [0, 1]], dtype="complex128")
         sticky_index_pairs = []
         for q in self.sticky_indices:
@@ -479,14 +479,75 @@
         tn_concatenated = tn_other_adj.cuquantum_interleaved
         tn_concatenated.extend(connector)
         tn_concatenated.extend(self.cuquantum_interleaved)
         self._logger.debug(f"Overlap input list: \n{tn_concatenated}")
         return tn_concatenated
 
 
+def measure_qubit_state(
+    ket: TensorNetwork, qubit_id: Qubit, bit_value: int, loglevel: int = logging.INFO
+) -> TensorNetwork:
+    """Measures a qubit in a tensor network.
+
+    Does so by appending a measurement gate to the tensor network.
+    The measurment gate is applied via appending a tensor cap of
+    the form:  0: [1, 0] or 1: [0, 1] to the interleaved einsum input.
+    Therefor removing one of the open indices of the tensor network.
+
+    Args:
+        ket: a TensorNetwork object representing a quantum state.
+        qubit_id: a qubit id.
+        bit_value: a bit value to be assigned to the measured qubit.
+        loglevel: logging level.
+
+    Returns:
+        A TensorNetwork object representing a quantum state after the
+        measurement with a modified interleaved notation containing the extra
+        measurement tensor.
+    """
+
+    cap = {
+        0: np.array([1, 0], dtype="complex128"),
+        1: np.array([0, 1], dtype="complex128"),
+    }
+
+    sticky_ind = ket.sticky_indices[qubit_id]
+    ket._cuquantum_interleaved.extend([cap[bit_value], [sticky_ind]])
+    ket.sticky_indices.pop(qubit_id)
+    return ket
+
+
+# TODO: Make this compatible with mid circuit measurements and reset
+def measure_qubits_state(
+    ket: TensorNetwork, measurement_dict: dict[Qubit, int], loglevel: int = logging.INFO
+) -> TensorNetwork:
+    """Measures a list of qubits in a tensor network.
+
+    Does so by appending a measurement gate to the tensor network.
+    The measurment gate is applied via appending a tensor cap
+    of the form:  0: [1, 0] or 1: [0, 1] to the interleaved einsum input.
+    Therefor removing the open indices of the tensor network corresponding
+    to the measured qubits.
+
+    Args:
+        ket: a TensorNetwork object representing a quantum state.
+        measurement_dict: a dictionary of qubit ids and their corresponding bit values
+         to be assigned to the measured qubits.
+        loglevel: logging level.
+
+    Returns:
+        A TensorNetwork object representing a quantum state after
+        the measurement with a modified interleaved notation containing
+        the extra measurement tensors.
+    """
+    for qubit_id, bit_value in measurement_dict.items():
+        ket = measure_qubit_state(ket, qubit_id, bit_value, loglevel)
+    return ket
+
+
 class PauliOperatorTensorNetwork:
     """Handles a tensor network representing a Pauli operator string."""
 
     PAULI = {
         "X": np.array([[0, 1], [1, 0]], dtype="complex128"),
         "Y": np.array([[0, -1j], [1j, 0]], dtype="complex128"),
         "Z": np.array([[1, 0], [0, -1]], dtype="complex128"),
@@ -584,26 +645,26 @@
         return self._cuquantum_interleaved
 
     def _make_interleaved(self) -> list:
         """Concatenates the tensor networks elements of the expectation value.
 
         Returns:
             A tensor network representing expectation value in the interleaved format
-             (list).
+            (list).
         """
-        tn_concatenated = self._bra.cuquantum_interleaved
+        tn_concatenated = self._bra.cuquantum_interleaved.copy()
         tn_concatenated.extend(self._operator.cuquantum_interleaved)
         tn_concatenated.extend(self._ket.cuquantum_interleaved)
         return tn_concatenated
 
 
 def tk_to_tensor_network(tkc: Circuit) -> List[Union[NDArray, List]]:
     """Converts pytket circuit into a tensor network.
 
     Args:
         tkc: Circuit.
 
     Returns:
         A tensor network representing the input circuit in the interleaved format
-         (list).
+        (list).
     """
     return TensorNetwork(tkc).cuquantum_interleaved
```

## pytket/extensions/cutensornet/backends/cutensornet_backend.py

```diff
@@ -21,23 +21,24 @@
 except ImportError:
     warnings.warn("local settings failed to import cutensornet", ImportWarning)
 from logging import warning
 from typing import List, Union, Optional, Sequence
 from uuid import uuid4
 import numpy as np
 from sympy import Expr  # type: ignore
-from pytket.circuit import Circuit, OpType  # type: ignore
+from pytket.circuit import Circuit, OpType, Qubit  # type: ignore
 from pytket.backends import ResultHandle, CircuitStatus, StatusEnum, CircuitNotRunError
 from pytket.backends.backend import KwargTypes, Backend, BackendResult
 from pytket.backends.backendinfo import BackendInfo
 from pytket.backends.resulthandle import _ResultIdTuple
 from pytket.extensions.cutensornet.tensor_network_convert import (
     TensorNetwork,
     ExpectationValueTensorNetwork,
     tk_to_tensor_network,
+    measure_qubits_state,
 )
 from pytket.predicates import Predicate, GateSetPredicate, NoClassicalBitsPredicate  # type: ignore
 from pytket.passes import (  # type: ignore
     BasePass,
     SequencePass,
     DecomposeBoxes,
     SynthesiseTket,
@@ -228,33 +229,51 @@
 
     # TODO: this should be optionally parallelised with MPI
     #  (both wrt Pauli strings and contraction itself).
     def get_operator_expectation_value(
         self,
         state_circuit: Circuit,
         operator: QubitPauliOperator,
+        post_selection: Optional[dict[Qubit, int]] = None,
         valid_check: bool = True,
     ) -> float:
         """Calculates expectation value of an operator using cuTensorNet contraction.
 
+        Has an option to do post selection on an ancilla register.
+
         Args:
             state_circuit: Circuit representing state.
             operator: Operator which expectation value is to be calculated.
             valid_check: Whether to perform circuit validity check.
+            post_selection: Dictionary of qubits to post select where the key is
+                qubit and the value is bit outcome.
 
         Returns:
-            Real part of the expectation value.
+            Expectation value.
         """
         if valid_check:
             self._check_all_circuits([state_circuit])
 
         expectation = 0
+
+        ket_network = TensorNetwork(state_circuit)
+        bra_network = ket_network.dagger()
+
+        if post_selection is not None:
+            post_select_qubits = list(post_selection.keys())
+            if set(post_select_qubits).issubset(operator.all_qubits):
+                raise ValueError(
+                    "Post selection qubit must not be a subset of operator qubits"
+                )
+            ket_network = measure_qubits_state(ket_network, post_selection)
+            bra_network = measure_qubits_state(
+                bra_network, post_selection
+            )  # This needed because dagger does not work with post selection
+
         for qos, coeff in operator._dict.items():
-            ket_network = TensorNetwork(state_circuit)
-            bra_network = ket_network.dagger()
             expectation_value_network = ExpectationValueTensorNetwork(
                 bra_network, qos, ket_network
             )
             if isinstance(coeff, Expr):
                 numeric_coeff = complex(coeff.evalf())  # type: ignore
             else:
                 numeric_coeff = complex(coeff)
```

## Comparing `pytket_cutensornet-0.1.0.dist-info/LICENSE` & `pytket_cutensornet-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_cutensornet-0.1.0.dist-info/METADATA` & `pytket_cutensornet-0.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-cutensornet
-Version: 0.1.0
+Version: 0.2.0
 Summary: Extension for pytket, providing access to the cuTensorNet Python API.
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-cutensornet/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-cutensornet
 Project-URL: Tracker, https://github.com/CQCL/pytket-cutensornet/issues
```

