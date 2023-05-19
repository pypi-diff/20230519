# Comparing `tmp/symmer-0.0.2.tar.gz` & `tmp/symmer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symmer-0.0.2.tar", max compression
+gzip compressed data, was "symmer-0.0.3.tar", max compression
```

## Comparing `symmer-0.0.2.tar` & `symmer-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0     1085 2023-04-04 11:10:51.637319 symmer-0.0.2/LICENSE
--rw-r--r--   0        0        0      646 2023-04-04 11:36:53.322481 symmer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-04 11:10:51.668194 symmer-0.0.2/symmer/.DS_Store
--rw-r--r--   0        0        0      176 2022-10-17 18:51:18.580060 symmer-0.0.2/symmer/.idea/.gitignore
--rw-r--r--   0        0        0      697 2022-10-17 18:51:18.580669 symmer-0.0.2/symmer/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2022-10-17 18:51:18.581057 symmer-0.0.2/symmer/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      194 2022-10-17 18:51:18.581395 symmer-0.0.2/symmer/.idea/misc.xml
--rw-r--r--   0        0        0      264 2022-10-17 18:51:18.581714 symmer-0.0.2/symmer/.idea/modules.xml
--rw-r--r--   0        0        0      483 2022-10-17 18:51:18.582579 symmer-0.0.2/symmer/.idea/symmer.iml
--rw-r--r--   0        0        0      183 2022-10-17 18:51:18.582914 symmer-0.0.2/symmer/.idea/vcs.xml
--rw-r--r--   0        0        0      148 2023-04-04 11:10:51.670029 symmer-0.0.2/symmer/__init__.py
--rw-r--r--   0        0        0      108 2023-02-17 13:01:54.920728 symmer-0.0.2/symmer/approximate/__init__.py
--rw-r--r--   0        0        0     6356 2023-04-04 11:10:51.671447 symmer-0.0.2/symmer/approximate/tensor_network.py
--rw-r--r--   0        0        0     6224 2023-04-04 11:10:51.672518 symmer-0.0.2/symmer/command_line.py
--rw-r--r--   0        0        0      167 2023-04-04 11:10:51.673955 symmer-0.0.2/symmer/evolution/__init__.py
--rw-r--r--   0        0        0     6245 2023-04-04 11:10:51.674756 symmer-0.0.2/symmer/evolution/decomposition.py
--rw-r--r--   0        0        0     1042 2023-04-04 11:10:51.676236 symmer-0.0.2/symmer/evolution/exponentiation.py
--rw-r--r--   0        0        0     2210 2023-04-04 11:10:51.677436 symmer-0.0.2/symmer/evolution/gate_library.py
--rw-r--r--   0        0        0      202 2023-04-04 11:10:51.678331 symmer-0.0.2/symmer/operators/__init__.py
--rw-r--r--   0        0        0    13453 2023-04-04 11:10:51.679143 symmer-0.0.2/symmer/operators/anticommuting_op.py
--rw-r--r--   0        0        0    74691 2023-04-04 11:10:55.046987 symmer-0.0.2/symmer/operators/base.py
--rw-r--r--   0        0        0    13945 2023-04-04 11:10:55.048272 symmer-0.0.2/symmer/operators/independent_op.py
--rw-r--r--   0        0        0    31207 2023-04-04 11:10:55.049518 symmer-0.0.2/symmer/operators/noncontextual_op.py
--rw-r--r--   0        0        0    13164 2023-04-04 11:10:55.051306 symmer-0.0.2/symmer/operators/utils.py
--rw-r--r--   0        0        0      173 2022-10-31 10:37:23.235873 symmer-0.0.2/symmer/projection/__init__.py
--rw-r--r--   0        0        0     7018 2023-04-04 11:10:51.684446 symmer-0.0.2/symmer/projection/base.py
--rw-r--r--   0        0        0    17681 2023-04-04 11:10:55.052682 symmer-0.0.2/symmer/projection/contextual_subspace.py
--rw-r--r--   0        0        0     3785 2023-04-04 11:10:51.686021 symmer-0.0.2/symmer/projection/qubit_tapering.py
--rw-r--r--   0        0        0     8647 2023-04-04 11:10:55.055075 symmer-0.0.2/symmer/projection/utils.py
--rw-r--r--   0        0        0     7651 2023-04-04 11:10:51.689155 symmer-0.0.2/symmer/utils.py
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 symmer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-08 14:33:42.105206 symmer-0.0.3/LICENSE
+-rw-r--r--   0        0        0      650 2023-05-15 13:32:06.458847 symmer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-08 14:33:42.138846 symmer-0.0.3/symmer/.DS_Store
+-rw-r--r--   0        0        0      176 2023-05-08 14:33:42.139272 symmer-0.0.3/symmer/.idea/.gitignore
+-rw-r--r--   0        0        0      697 2023-05-08 14:33:42.139787 symmer-0.0.3/symmer/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-05-08 14:33:42.140112 symmer-0.0.3/symmer/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      194 2023-05-08 14:33:42.140413 symmer-0.0.3/symmer/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2023-05-08 14:33:42.140811 symmer-0.0.3/symmer/.idea/modules.xml
+-rw-r--r--   0        0        0      483 2023-05-08 14:33:42.141118 symmer-0.0.3/symmer/.idea/symmer.iml
+-rw-r--r--   0        0        0      183 2023-05-08 14:33:42.141394 symmer-0.0.3/symmer/.idea/vcs.xml
+-rw-r--r--   0        0        0      170 2023-05-19 14:18:19.485009 symmer-0.0.3/symmer/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-08 14:38:27.294495 symmer-0.0.3/symmer/approximate/__init__.py
+-rw-r--r--   0        0        0     6711 2023-05-08 14:38:27.294854 symmer-0.0.3/symmer/approximate/tensor_network.py
+-rw-r--r--   0        0        0     6224 2023-05-08 14:33:42.143074 symmer-0.0.3/symmer/command_line.py
+-rw-r--r--   0        0        0      256 2023-05-15 13:32:06.459186 symmer-0.0.3/symmer/evolution/__init__.py
+-rw-r--r--   0        0        0     7633 2023-05-15 13:32:06.459607 symmer-0.0.3/symmer/evolution/decomposition.py
+-rw-r--r--   0        0        0     1042 2023-05-08 14:33:42.144166 symmer-0.0.3/symmer/evolution/exponentiation.py
+-rw-r--r--   0        0        0     2210 2023-05-08 14:33:42.144427 symmer-0.0.3/symmer/evolution/gate_library.py
+-rw-r--r--   0        0        0    17903 2023-05-15 13:32:06.459996 symmer-0.0.3/symmer/evolution/variational_optimization.py
+-rw-r--r--   0        0        0      202 2023-05-08 14:38:27.296321 symmer-0.0.3/symmer/operators/__init__.py
+-rw-r--r--   0        0        0    15429 2023-05-19 14:18:19.486093 symmer-0.0.3/symmer/operators/anticommuting_op.py
+-rw-r--r--   0        0        0    76272 2023-05-15 13:32:06.461060 symmer-0.0.3/symmer/operators/base.py
+-rw-r--r--   0        0        0    13998 2023-05-15 13:32:06.461441 symmer-0.0.3/symmer/operators/independent_op.py
+-rw-r--r--   0        0        0    25586 2023-05-19 14:18:19.486624 symmer-0.0.3/symmer/operators/noncontextual_op.py
+-rw-r--r--   0        0        0    15094 2023-05-19 14:18:19.487540 symmer-0.0.3/symmer/operators/utils.py
+-rw-r--r--   0        0        0      230 2023-05-19 14:18:19.488089 symmer-0.0.3/symmer/projection/__init__.py
+-rw-r--r--   0        0        0     7018 2023-05-08 14:33:42.149064 symmer-0.0.3/symmer/projection/base.py
+-rw-r--r--   0        0        0    15114 2023-05-19 14:18:19.488622 symmer-0.0.3/symmer/projection/contextual_subspace.py
+-rw-r--r--   0        0        0     7732 2023-05-19 14:18:19.489043 symmer-0.0.3/symmer/projection/qubit_subspace_manager.py
+-rw-r--r--   0        0        0     3785 2023-05-08 14:33:42.150052 symmer-0.0.3/symmer/projection/qubit_tapering.py
+-rw-r--r--   0        0        0     8799 2023-05-19 14:18:19.489567 symmer-0.0.3/symmer/projection/utils.py
+-rw-r--r--   0        0        0    10502 2023-05-19 14:18:19.489901 symmer-0.0.3/symmer/utils.py
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 symmer-0.0.3/PKG-INFO
```

### Comparing `symmer-0.0.2/LICENSE` & `symmer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `symmer-0.0.2/pyproject.toml` & `symmer-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "symmer"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["AlexisRalli <rallilex@hotmail.co.uk>", "TimWeaving <weaving.timothy@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8 <3.11"
 openfermion = "^1.3.0"
@@ -13,15 +13,15 @@
 pydocstyle = "^6.1.1"
 isort = "^5.10.1"
 black = "^22.1.0"
 flake8 = "^4.0.1"
 py3Dmol = "^1.8.0"
 ipywidgets = "7.7.2"
 ncon = "^1.0.0"
-quimb = "^1.4.2"
+quimb = ">=1.4 <1.5"
 opt-einsum = "^3.3.0"
 autoray = "^0.5.3"
 qubovert = "^1.2.5"
 pytest = "^7.2.2"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `symmer-0.0.2/symmer/.DS_Store` & `symmer-0.0.3/symmer/.DS_Store`

 * *Files identical despite different names*

### Comparing `symmer-0.0.2/symmer/.idea/inspectionProfiles/Project_Default.xml` & `symmer-0.0.3/symmer/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `symmer-0.0.2/symmer/approximate/tensor_network.py` & `symmer-0.0.3/symmer/approximate/tensor_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,22 @@
             σ1, l1, i1, j1 = contr.shape
             σ2, l2, i2, j2 = tensor.shape
             contr = ncon([contr, tensor], ((-1, -3, -5, 1), (-2, -4, 1, -6)))
             contr = np.reshape(contr, (σ1 * σ2, l1 * l2, i1, j2))
 
         contr = np.squeeze(contr)
         return contr
-
+    
+def get_MPO(operator: PauliwordOp, max_bond_dimension: int) -> MPOOp:
+    """ Return the Matrix Product Operator (MPO) of a PauliwordOp 
+    (linear combination of Paulis) given a maximum bond dimension
+    """
+    pstrings, coefflist = zip(*operator.to_dictionary.items())
+    mpo = MPOOp(pstrings, coefflist, Dmax=max_bond_dimension)
+    return mpo
 
 def find_groundstate_quimb(MPOOp: MPOOp, dmrg=None, gs_guess=None) -> QuantumState:
     """
     Use quimb's DMRG2 optimiser to approximate groundstate of MPOOp
 
     Args:
         MPOOp: MPOOp representing operator
```

### Comparing `symmer-0.0.2/symmer/command_line.py` & `symmer-0.0.3/symmer/command_line.py`

 * *Files identical despite different names*

### Comparing `symmer-0.0.2/symmer/evolution/decomposition.py` & `symmer-0.0.3/symmer/evolution/decomposition.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from functools import reduce
-from typing import Dict, List
-from symmer.operators import PauliwordOp
+from typing import Dict, List, Union
+from symmer.operators import PauliwordOp, QuantumState
 from symmer.evolution.gate_library import *
 from qiskit.circuit import QuantumCircuit, ParameterVector
+import networkx as nx
+import warnings
+warnings.filterwarnings("ignore", category=DeprecationWarning) 
 
 ##############################################
 # Decompose any QASM file into a PauliwordOp #
 ##############################################
 
 def qasm_to_PauliwordOp(qasm: str, reverse=False, combine=True) -> PauliwordOp:
     """ Decompose an QASM circuit into a linear combination of Pauli 
@@ -85,76 +88,104 @@
                                         'S_indices':S_indices, 
                                         'CNOT_indices':CNOT_indices,
                                         'RZ_index':CNOT_indices[-1]}
         return circuit_instructions
 
 def PauliwordOp_to_QuantumCircuit(
     PwordOp: PauliwordOp, 
-    ref_state: np.array = None,
+    ref_state: np.array  = None,
     basis_change_indices: Dict[str, List[int]] = {'X_indices':[],'Y_indices':[]},
     trotter_number: int = 1, 
     bind_params: bool = True,
     include_barriers:bool = True,
+    parameter_label: str = 'P'
     ) -> QuantumCircuit:
     """
     Convert the operator to a QASM circuit string for input 
     into quantum computing packages such as Qiskit and Cirq
 
     basis_change_indices in form [X_indices, Y_indices]
     """
+    if isinstance(ref_state, QuantumState):
+        assert ref_state.n_terms == 1
+        ref_state = ref_state.state_matrix[0]
+
     def qiskit_ordering(indices):
         """ we index from left to right - in Qiskit this ordering is reversed
         """
         return PwordOp.n_qubits - 1 - indices
 
     qc = QuantumCircuit(PwordOp.n_qubits)
     for i in qiskit_ordering(np.where(ref_state==1)[0]):
         qc.x(i)
 
-    def CNOT_cascade(cascade_indices, reverse=False):
-        index_pairs = list(zip(cascade_indices[:-1], cascade_indices[1:]))
-        if reverse:
-            index_pairs = index_pairs[::-1]
-        for source, target in index_pairs:
-            qc.cx(source, target)
-
-    def circuit_from_step(angle, H_indices, S_indices, CNOT_indices, RZ_index):
-        # to Pauli X basis
-        for i in S_indices:
-            qc.sdg(i)
-        # to Pauli Z basis
-        for i in H_indices:
-            qc.h(i)
-        # compute parity
-        CNOT_cascade(CNOT_indices)
-        qc.rz(-2*angle, RZ_index)
-        CNOT_cascade(CNOT_indices, reverse=True)
-        for i in H_indices:
-            qc.h(i)
-        for i in S_indices:
-            qc.s(i)
+    non_identity = PwordOp[np.any(PwordOp.symp_matrix, axis=1)]
 
-    if bind_params:
-        angles = PwordOp.coeff_vec.real/trotter_number
-    else:
-        angles = np.array(ParameterVector('P', PwordOp.n_terms))/trotter_number
+    if non_identity.n_terms > 0:
 
-    instructions = PauliwordOp_to_instructions(PwordOp)
-    assert(len(angles)==len(instructions)), 'Number of parameters does not match the circuit instructions'
-    for trot_step in range(trotter_number):
-        for step, gate_indices in instructions.items():
-            qiskit_gate_indices = [qiskit_ordering(indices) for indices in gate_indices.values()]
+        def CNOT_cascade(cascade_indices, reverse=False):
+            index_pairs = list(zip(cascade_indices[:-1], cascade_indices[1:]))
+            if reverse:
+                index_pairs = index_pairs[::-1]
+            for source, target in index_pairs:
+                qc.cx(source, target)
+
+        def circuit_from_step(angle, H_indices, S_indices, CNOT_indices, RZ_index):
+            # to Pauli X basis
+            for i in S_indices:
+                qc.sdg(i)
+            # to Pauli Z basis
+            for i in H_indices:
+                qc.h(i)
+            # compute parity
+            CNOT_cascade(CNOT_indices)
+            qc.rz(-2*angle, RZ_index)
+            CNOT_cascade(CNOT_indices, reverse=True)
+            for i in H_indices:
+                qc.h(i)
+            for i in S_indices:
+                qc.s(i)
+
+        if bind_params:
+            angles = non_identity.coeff_vec.real/trotter_number
+        else:
+            angles = np.array(ParameterVector(parameter_label, non_identity.n_terms))/trotter_number
 
-            if include_barriers:
-                qc.barrier()
+        instructions = PauliwordOp_to_instructions(non_identity)
+        assert(len(angles)==len(instructions)), 'Number of parameters does not match the circuit instructions'
+        for trot_step in range(trotter_number):
+            for step, gate_indices in instructions.items():
+                qiskit_gate_indices = [qiskit_ordering(indices) for indices in gate_indices.values()]
 
-            circuit_from_step(angles[step], *qiskit_gate_indices)
+                if include_barriers:
+                    qc.barrier()
+
+                circuit_from_step(angles[step], *qiskit_gate_indices)
 
     if include_barriers:
         qc.barrier()
 
     for i in basis_change_indices['Y_indices']:
         qc.s(qiskit_ordering(i))
     for i in basis_change_indices['X_indices']:
         qc.h(qiskit_ordering(i))
         
-    return qc
+    return qc
+
+def get_CNOT_connectivity_graph(evolution_obj: Union[PauliwordOp, QuantumCircuit], print_graph=False):
+    """ Get the graph whoss edges denote nonlocal interaction between two qubits.
+    This is useful for device-aware ansatz construction to ensure the circuit connectiviy
+    may be accomodated by the topology of the target quantum processor. 
+    """
+    if isinstance(evolution_obj, PauliwordOp):
+        qc = PauliwordOp_to_QuantumCircuit(evolution_obj)
+    else:
+        assert isinstance(evolution_obj, QuantumCircuit)
+        qc = evolution_obj
+    nodes = [q.index for q in qc.qregs[0]]
+    edges = [[q.index for q in step[1]] for step in qc.data if step[0].name!='barrier' and len(step[1])>1]
+    G = nx.Graph()
+    G.add_nodes_from(nodes)
+    G.add_edges_from(edges)
+    if print_graph:
+        nx.draw_kamada_kawai(G)
+    return G
```

### Comparing `symmer-0.0.2/symmer/evolution/exponentiation.py` & `symmer-0.0.3/symmer/evolution/exponentiation.py`

 * *Files identical despite different names*

### Comparing `symmer-0.0.2/symmer/evolution/gate_library.py` & `symmer-0.0.3/symmer/evolution/gate_library.py`

 * *Files identical despite different names*

### Comparing `symmer-0.0.2/symmer/operators/anticommuting_op.py` & `symmer-0.0.3/symmer/operators/anticommuting_op.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                                         np.delete(op_for_rotation.coeff_vec, k_index, axis=0))
 
             ## know how operator acts therefore don't need to actually do rotations
 
             return self._recursive_seq_rotations(AC_op_rotated)
 
 
-    def unitary_partitioning(self, s_index: int=None, up_method: Optional[str]='LCU') \
+    def unitary_partitioning(self, s_index: int=None, up_method: Optional[str]='seq_rot') \
             -> Tuple[PauliwordOp, Union[PauliwordOp, List[Tuple[PauliwordOp, float]]], float, "AntiCommutingOp"]:
         """
         Apply unitary partitioning on anticommuting operator (self)
 
         Args:
             s_index (int): index of row in symplectic matrix that defines Pauli operator to reduce too (Ps).
                            if set to None then code will find least dense Pauli operator and use that.
@@ -123,38 +123,48 @@
 
         Returns:
             Ps (PauliwordOp): Pauli operator of term reduced too
             rotations (PauliwordOp): rotations to perform unitary partitioning
             gamma_l (float): normalization constant of clique (anticommuting operator)
             AC_op (AntiCommutingOp): normalized clique - i.e. self == gamma_l * AC_op
         """
+        assert up_method in ['LCU', 'seq_rot'], f'unknown unitary partitioning method: {up_method}'
         AC_op = self.copy()
+
         if AC_op.n_terms == 1:
             rotations = None
             gamma_l = np.linalg.norm(AC_op.coeff_vec)
             AC_op.coeff_vec = AC_op.coeff_vec / gamma_l
-            Ps = AC_op
+            Ps = PauliwordOp(AC_op.symp_matrix, [1])
             return Ps, rotations, gamma_l, AC_op
+
         else:
 
-            assert (np.sum(AC_op.coeff_vec.imag)==0), 'cannot apply unitary partitioning to operator with complex coeffs'
+            assert np.isclose(np.sum(AC_op.coeff_vec.imag), 0), 'cannot apply unitary partitioning to operator with complex coeffs'
 
             gamma_l = np.linalg.norm(AC_op.coeff_vec)
             AC_op.coeff_vec = AC_op.coeff_vec / gamma_l
 
             if s_index is None:
                 s_index = self.get_least_dense_term_index()
 
             if s_index!=0:
                 # re-order so s term is ALWAYS at top of symplectic matrix and thus is index as 0!
                 ### assert s_index <= AC_op.n_terms-1, 's_index out of range'
                 AC_op.coeff_vec[[0, s_index]] = AC_op.coeff_vec[[s_index, 0]]
                 AC_op.symp_matrix[[0, s_index]] = AC_op.symp_matrix[[s_index, 0]]
                 AC_op = AntiCommutingOp(AC_op.symp_matrix, AC_op.coeff_vec) # need to reinit otherwise Z and X blocks wrong
 
+            # assert not np.isclose(AC_op.coeff_vec[0], 0), f's_index cannot have zero coefficent: {AC_op.coeff_vec[0]}'
+            if np.isclose(AC_op[0].coeff_vec, 0):
+                # need to correct for s_index having zero coeff... then need to swap to nonzero index
+                non_zero_index = np.argmax(abs(AC_op.coeff_vec))
+                AC_op.coeff_vec[[0, non_zero_index]] = AC_op.coeff_vec[[non_zero_index, 0]]
+                AC_op.symp_matrix[[0, non_zero_index]] = AC_op.symp_matrix[[non_zero_index, 0]]
+
             if up_method=='seq_rot':
                 if len(self.X_sk_rotations)!=0:
                     self.X_sk_rotations = []
                 Ps = self._recursive_seq_rotations(AC_op)
                 rotations = self.X_sk_rotations
             elif up_method=='LCU':
                 if self.R_LCU is not None:
@@ -182,18 +192,42 @@
                            least dense Pauli operator in AC operator.
             check_reduction (bool): flag to check reduction by applying LCU on original operator.
 
         Returns:
             R_LCU (PauliwordOp): PauliwordOp that is a linear combination of unitaries
             P_s (PauliwordOp): single PauliwordOp that has been reduced too.
         """
+        # need to remove zero coeff terms
+        AC_op_cpy = AC_op.copy()
+        before_cleanup = AC_op_cpy.n_terms
+        AC_op = AC_op_cpy[np.where(abs(AC_op.coeff_vec)>1e-15)[0]]
+        post_cleanup = AC_op.n_terms
+        # AC_op = AC_op.cleanup(zero_threshold=1e-15)  ## cleanup re-orders which is BAD for s_index
+
+
+        if (before_cleanup>1 and post_cleanup==1):
+            if AC_op.coeff_vec[0]<0:
+                # need to fix neg sign (use Pauli multiplication)
 
-        if AC_op.n_terms==1:
-            self.R_LCU = None
-            Ps_LCU = None
+                # as s index defaults to 0, take the next term (in CS-VQE this will commute with symmetries)!
+                if np.isclose(AC_op_cpy[0].coeff_vec, 0):
+                    # need to correct for s_index having zero coeff... then need to swap to nonzero index
+                    non_zero_index = np.argmax(abs(AC_op_cpy.coeff_vec))
+
+                    AC_op_cpy.coeff_vec[[0, non_zero_index]] = AC_op_cpy.coeff_vec[[non_zero_index, 0]]
+                    AC_op_cpy.symp_matrix[[0, non_zero_index]] = AC_op_cpy.symp_matrix[[non_zero_index, 0]]
+
+
+                sign_correction = PauliwordOp(AC_op_cpy.symp_matrix[1],[1])
+
+                self.R_LCU = sign_correction
+                Ps_LCU = PauliwordOp(AC_op.symp_matrix, [1])
+            else:
+                self.R_LCU = PauliwordOp.from_list(['I'*AC_op.n_qubits])
+                Ps_LCU = PauliwordOp(AC_op.symp_matrix, AC_op.coeff_vec)
         else:
             s_index=0
 
             # note gamma_l norm applied on init!
             Ps_LCU = PauliwordOp(AC_op.symp_matrix[s_index], [1])
             βs = AC_op.coeff_vec[s_index]
```

### Comparing `symmer-0.0.2/symmer/operators/base.py` & `symmer-0.0.3/symmer/operators/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import pandas as pd
 import networkx as nx
 from tqdm.auto import tqdm
 from copy import deepcopy
-from itertools import product
 from functools import reduce
 from typing import List, Union
 from numbers import Number
 import multiprocessing as mp
 from cached_property import cached_property
 from scipy.sparse import csr_matrix, csc_matrix, coo_matrix, dok_matrix
 from symmer.operators.utils import *
@@ -195,15 +194,22 @@
         operator_out = decomposition.cleanup()
 
         # fix ZX Y phases generated!
         Y_sign = (operator_out.Y_count % 2 * -2) + 1
         operator_out.coeff_vec = operator_out.coeff_vec * Y_sign
 
         if operator_basis is not None:
-            if not np.all(operator_out.to_sparse_matrix.toarray() == matrix):
+            if isinstance(matrix, csr_matrix):
+                tol=1e-15
+                max_diff = np.abs(matrix - operator_out.to_sparse_matrix).max()
+                flag = not (max_diff <= tol)
+            else:
+                flag = not np.allclose(operator_out.to_sparse_matrix.toarray(), matrix)
+
+            if flag:
                 warnings.warn('Basis not sufficiently expressive, output operator projected onto basis supplied.')
 
         return operator_out
 
     @classmethod
     def _from_matrix_projector(cls, 
             matrix: Union[np.array, csr_matrix],
@@ -226,26 +232,27 @@
         coeff_operator = dok_matrix((4 ** n_qubits, 1),
                                     dtype=complex)
 
         binary_vec = (
                 (
                         np.arange(2 ** n_qubits).reshape([-1, 1]) &
                         (1 << np.arange(n_qubits))[::-1]
-                ) > 0).astype(bool)
+                ) > 0)#.astype(bool)
 
         binary_convert = 1 << np.arange(2 * n_qubits)[::-1]
         # P_out = cls.empty(n_qubits)
         for i, j in tqdm(zip(row, col), desc='Building operator via projectors', total=len(row)):
             ij_symp_matrix, proj_coeffs = get_ij_operator(i, j,
                                                           n_qubits,
                                                           binary_vec=binary_vec,
                                                           return_operator=False)
 
             ### find location in symp matrix
-            int_list = ij_symp_matrix @ binary_convert  # (1 << np.arange(ij_symp_matrix.shape[1])[::-1])
+            # int_list = ij_symp_matrix @ binary_convert  # (1 << np.arange(ij_symp_matrix.shape[1])[::-1])
+            int_list = np.einsum('j, ij->i', binary_convert, ij_symp_matrix)
 
             # populate sparse mats
             sym_operator[int_list, :] = ij_symp_matrix
             coeff_operator[int_list] += proj_coeffs.reshape(-1, 1) * matrix[i, j]
 
         ### only keep nonzero coeffs! (skips expensive cleanup)
         nonzero = coeff_operator.nonzero()[0]
@@ -417,45 +424,42 @@
         op_reconstruction = reduced[dim:,:dim]
         return op_reconstruction.astype(int), mask_successfully_reconstructed
 
     def jordan_generator_reconstruction(self, generators: "PauliwordOp"):
         """ Reconstruct this PauliwordOp under the Jordan product PQ = {P,Q}/2
         with respect to the supplied generators
         """
-        assert (
-            check_jordan_independent(generators),
-            'The non-symmetry elements do not pairwise anticommute.'
-        )
+        assert check_jordan_independent(generators), 'The non-symmetry elements do not pairwise anticommute.'
+
         # empty reconstruction matrix to be updated in loop over anticommuting elements
         op_reconstruction = np.zeros([self.n_terms, generators.n_terms])
         successfully_reconstructed = np.zeros(self.n_terms, dtype=bool)
 
         # first, separate symmetry elements  from anticommuting ones
         mask_symmetries = np.all(generators.adjacency_matrix, axis=1)
-        Symmetries = generators[mask_symmetries]
-        Anticommuting = generators[~mask_symmetries]
-        where_anti = np.where(~mask_symmetries)[0]
-        
-        if Anticommuting.n_terms == 0:
+
+        if np.all(mask_symmetries):
             # If not anticommuting component, return standard generator recon over symmetries
-            return self.generator_reconstruction(Symmetries)
+            return self.generator_reconstruction(generators)
         else:
             # loop over anticommuting elements to enforce Jordan condition (no two anticommuting elements multiplied)
-            for index, P in zip(where_anti, Anticommuting):
+            for _, clq in generators[~mask_symmetries].clique_cover(edge_relation='C').items():
+                clq_indices = [np.where(np.all(generators.symp_matrix == t, axis=1))[0][0] for t in clq.symp_matrix]   
                 mask_symmetries_with_P = mask_symmetries.copy()
-                mask_symmetries_with_P[index] = True
+                mask_symmetries_with_P[np.array(clq_indices)] = True   
                 # reconstruct this PauliwordOp in the augemented symmetry + single anticommuting term generating set
-                recon_mat_P, successful_P = self.generator_reconstruction(P+Symmetries)
+                augmented_symmetries = generators[mask_symmetries_with_P]
+                recon_mat_P, successful_P = self.generator_reconstruction(augmented_symmetries)
                 # np.ix_ needed to correctly slice op_reconstruction as mask method does not work
                 row, col = np.ix_(successful_P,mask_symmetries_with_P)
                 op_reconstruction[row, col] = recon_mat_P[successful_P]
                 # will have duplicate succesful reconstruction of symmetries, so only sets True once in logical OR
                 successfully_reconstructed = np.logical_or(successfully_reconstructed, successful_P)
-
-            return op_reconstruction, successfully_reconstructed
+            
+            return op_reconstruction.astype(int), successfully_reconstructed
 
     @cached_property
     def Y_count(self) -> np.array:
         """ 
         Count the qubit positions of each term set to Pauli Y
 
         cached_property means this only runs once and then is stored
@@ -478,45 +482,62 @@
         else:
             return PauliwordOp(
                 *symplectic_cleanup(
                     self.symp_matrix, self.coeff_vec, zero_threshold=zero_threshold
                 )
             )
 
-    def __eq__(self, 
+    def __eq__(self,
             Pword: "PauliwordOp"
         ) -> bool:
         """ In theory should use logical XNOR to check symplectic matrix match, however
         can use standard logical XOR and look for False indices instead (implementation
-        skips an additional NOT operation) 
+        skips an additional NOT operation)
         """
         check_1 = self.cleanup()
         check_2 = Pword.cleanup()
         if check_1.n_qubits != check_2.n_qubits:
             raise ValueError('Operators defined over differing numbers of qubits.')
         elif check_1.n_terms != check_2.n_terms:
             return False
         else:
-            return (
-                not np.sum(np.logical_xor(check_1.symp_matrix, check_2.symp_matrix)) and 
-                np.allclose(check_1.coeff_vec, check_2.coeff_vec)
-            )
+            return (not np.sum(np.logical_xor(check_1.symp_matrix, check_2.symp_matrix)) and
+                         np.allclose(check_1.coeff_vec, check_2.coeff_vec))
+            # if eq_flag is True:
+            #     assert hash(check_1) == hash(check_2), 'equal objects have different hash values'
+            # return eq_flag
+
+    def __hash__(self) -> int:
+        """ build unique hash from dictionary of PauliwordOp"""
+
+        self.cleanup()  # self.cleanup(zero_threshold=1e-15)
+
+        # tuples are immutable
+        tuple_of_tuples = tuple(self.to_dictionary.items())
+        hash_val = hash(tuple_of_tuples)
+        return hash_val
 
-    def __add__(self, 
+    def append(self, 
             PwordOp: "PauliwordOp"
         ) -> "PauliwordOp":
-        """ Add to this PauliwordOp another PauliwordOp by stacking the
-        respective symplectic matrices and cleaning any resulting duplicates
+        """ Append another PauliwordOp onto this one - duplicates allowed
         """
         assert (self.n_qubits == PwordOp.n_qubits), 'Pauliwords defined for different number of qubits'
         P_symp_mat_new = np.vstack((self.symp_matrix, PwordOp.symp_matrix))
-        P_new_coeffs = np.hstack((self.coeff_vec, PwordOp.coeff_vec)) 
+        P_new_coeffs = np.hstack((self.coeff_vec, PwordOp.coeff_vec))
+        return PauliwordOp(P_symp_mat_new, P_new_coeffs) 
 
+    def __add__(self, 
+            PwordOp: "PauliwordOp"
+        ) -> "PauliwordOp":
+        """ Add to this PauliwordOp another PauliwordOp by stacking the
+        respective symplectic matrices and cleaning any resulting duplicates
+        """
         # cleanup run to remove duplicate rows (Pauliwords)
-        return PauliwordOp(P_symp_mat_new, P_new_coeffs).cleanup()
+        return self.append(PwordOp).cleanup()
 
     def __radd__(self, 
             add_obj: Union[int, "PauliwordOp"]
         ) -> "PauliwordOp":
         """ Allows use of sum() over a list of PauliwordOps
         """
         if add_obj == 0:
@@ -877,15 +898,15 @@
         # build graph
         graph = self.get_graph(edge_relation=edge_relation)
         pauli_indices = sorted(nx.find_cliques(graph), key=lambda x:-len(x))[0]
         return sum([self[i] for i in pauli_indices])
 
     def clique_cover(self, 
             edge_relation = 'C', 
-            strategy='independent_set',
+            strategy='largest_first',
             colouring_interchange=False
         ) -> Dict[int, "PauliwordOp"]:
         """ Perform a graph colouring to identify a clique partition
 
         ------------------------
         | colouring strategies |
         ------------------------
@@ -1014,22 +1035,24 @@
 
         Returns:
             sparse_matrix (csr_matrix): sparse matrix of PauliOp
         """
         if self.n_qubits == 0:
             return csr_matrix(self.coeff_vec)
 
-        if self.n_qubits > 64:
-            # numpy cannot handle ints over int64s (2**64) therefore use python objects
-            binary_int_array = 1 << np.arange(self.n_qubits - 1, -1, -1).astype(object)
-        else:
-            binary_int_array = 1 << np.arange(self.n_qubits - 1, -1, -1)
+        # if self.n_qubits > 64:
+        #     # numpy cannot handle ints over int64s (2**64) therefore use python objects
+        #     binary_int_array = 1 << np.arange(self.n_qubits - 1, -1, -1).astype(object)
+        # else:
+        #     binary_int_array = 1 << np.arange(self.n_qubits - 1, -1, -1)
+        # x_int = (self.X_block @ binary_int_array).reshape(-1, 1)
+        # z_int = (self.Z_block @ binary_int_array).reshape(-1, 1)
 
-        x_int = (self.X_block @ binary_int_array).reshape(-1, 1)
-        z_int = (self.Z_block @ binary_int_array).reshape(-1, 1)
+        x_int = binary_array_to_int(self.X_block).reshape(-1, 1)
+        z_int = binary_array_to_int(self.Z_block).reshape(-1, 1)
 
         Y_number = np.sum(np.bitwise_and(self.X_block, self.Z_block).astype(int), axis=1)
         global_phase = (-1j) ** Y_number
 
         dimension = 2 ** self.n_qubits
         row_ind = np.repeat(np.arange(dimension).reshape(1, -1), self.X_block.shape[0], axis=0)
         col_ind = np.bitwise_xor(row_ind, x_int)
@@ -1280,20 +1303,28 @@
         
         assert(self.n_qubits == mul_obj.n_qubits), 'Multiplication object defined for different number of qubits'
         assert(self.vec_type=='bra'), 'Cannot multiply a ket from the right'
         
         if isinstance(mul_obj, QuantumState):
             assert(mul_obj.vec_type=='ket'), 'Cannot multiply a bra with another bra'
             inner_product=0
-            for (bra_string, bra_coeff),(ket_string, ket_coeff) in product(
-                    zip(self.state_matrix, self.state_op.coeff_vec), 
-                    zip(mul_obj.state_matrix, mul_obj.state_op.coeff_vec)
-                ):
-                if np.all(bra_string == ket_string):
-                    inner_product += (bra_coeff*ket_coeff)
+
+            # set left state to be smallest in number of bitstrings making loop short!
+            if self.state_op.n_terms < mul_obj.n_terms:
+                left_state = self
+                right_state = mul_obj
+            else:
+                left_state = mul_obj
+                right_state = self
+
+            # O(length_smallest_statevector) runtime. (Note linear rather than quadratic!)
+            for bstring, left_coeff in left_state.to_dictionary.items():
+                right_coeff = right_state.to_dictionary.get(bstring, 0)
+                inner_product += left_coeff * right_coeff
+
             return inner_product
 
         elif isinstance(mul_obj, PauliwordOp):
             new_state_op = self.state_op * mul_obj
             new_state_op.coeff_vec*=((-1j)**new_state_op.Y_count)
             new_bra_state = QuantumState(
                 new_state_op.X_block, 
@@ -1428,18 +1459,19 @@
     @cached_property
     def to_sparse_matrix(self):
         """
         Returns:
             sparse_Qstate (csr_matrix): sparse matrix representation of the statevector
         """
         # nonzero_indices = [int(''.join([str(i) for i in row]),2) for row in self.state_matrix]
-        if self.n_qubits<64:
-            nonzero_indices = self.state_matrix @ (1 << np.arange(self.state_matrix.shape[1])[::-1])
-        else:
-            nonzero_indices = self.state_matrix @ (1 << np.arange(self.state_matrix.shape[1], dtype=object)[::-1])
+        # if self.n_qubits<64:
+        #     nonzero_indices = self.state_matrix @ (1 << np.arange(self.state_matrix.shape[1])[::-1])
+        # else:
+        #     nonzero_indices = self.state_matrix @ (1 << np.arange(self.state_matrix.shape[1], dtype=object)[::-1])
+        nonzero_indices = binary_array_to_int(self.state_matrix)
 
         sparse_Qstate = csr_matrix(
             (self.state_op.coeff_vec, (nonzero_indices, np.zeros_like(nonzero_indices))),
             shape = (2**self.n_qubits, 1), 
             dtype=np.complex128
         )
         if self.vec_type == 'bra':
@@ -1583,18 +1615,19 @@
         else:
             zero_threshold = None
         q_state = self.cleanup(zero_threshold=zero_threshold)
         prob = np.abs(q_state.state_op.coeff_vec) ** 2
 
         fig, ax = plt.subplots(1, 1, dpi=dpi)
 
-        if q_state.state_op.n_qubits<64:
-            x_binary_ints = q_state.state_matrix @ (1 << np.arange(q_state.state_matrix.shape[1])[::-1])
-        else:
-            x_binary_ints = q_state.state_matrix @ (1 << np.arange(q_state.state_matrix.shape[1], dtype=object)[::-1])
+        # if q_state.state_op.n_qubits<64:
+        #     x_binary_ints = q_state.state_matrix @ (1 << np.arange(q_state.state_matrix.shape[1])[::-1])
+        # else:
+        #     x_binary_ints = q_state.state_matrix @ (1 << np.arange(q_state.state_matrix.shape[1], dtype=object)[::-1])
+        x_binary_ints = binary_array_to_int(q_state.state_matrix)
 
         if prob.shape[0]<2**8:
             # bar chart
             ax.bar(x_binary_ints, prob, width=1, edgecolor="white", linewidth=0.8)
             if binary_xlabels:
                 ax.set_xticks(x_binary_ints, labels=[np.binary_repr(x, self.n_qubits) for x in x_binary_ints])
                 plt.xticks(rotation = 90)
```

### Comparing `symmer-0.0.2/symmer/operators/independent_op.py` & `symmer-0.0.3/symmer/operators/independent_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         PwordOp = super().from_dictionary(operator_dict)
         return cls.from_PauliwordOp(PwordOp)
 
     @classmethod
     def symmetry_generators(cls, 
             PwordOp: PauliwordOp, 
             commuting_override:bool=False,
+            largest_clique = False
         ) -> "IndependentOp":
         """ Identify a symmetry basis for the supplied Pauli operator with
         symplectic representation  M = [ X | Z ]. We perform columnwise 
         Gaussian elimination to yield the matrix
 
                 [ Z | X ]     [ R ]
                 |-------| ->  |---|
@@ -91,15 +92,15 @@
             warnings.warn('The input PauliwordOp has no Z2 symmetries.')
             return S
             # raise RuntimeError('The input PauliwordOp has no Z2 symmetries.')
         if np.all(S.adjacency_matrix) or commuting_override:
             return S
         else:
             # if any of the stabilizers are not mutually commuting, take the largest commuting subset
-            if S.n_terms < 10:
+            if S.n_terms < 10 or largest_clique:
                 # expensive clique cover finding optimal commuting subset
                 S_commuting = S.largest_clique(edge_relation='C')    
             else:
                 # greedy graph-colouring approach when symmetry basis is large
                 S_commuting = S.clique_cover(edge_relation='C')[0]
                 warnings.warn('Greedy method may identify non-optimal commuting symmetry terms; might be able to taper again.')
```

### Comparing `symmer-0.0.2/symmer/operators/noncontextual_op.py` & `symmer-0.0.3/symmer/operators/noncontextual_op.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,101 @@
 import warnings
-
+import itertools
 import numpy as np
+import networkx as nx
+import multiprocessing as mp
+import qubovert as qv
+from cached_property import cached_property
 from time import time
 from functools import reduce
-from typing import Optional, Union, Tuple
-import multiprocessing as mp
+from typing import Optional, Union, Tuple, List
+from matplotlib import pyplot as plt
 from scipy.optimize import differential_evolution, shgo
 from symmer.operators import PauliwordOp, IndependentOp, AntiCommutingOp, QuantumState
-from symmer.operators.utils import unit_n_sphere_cartesian_coords, check_adjmat_noncontextual
-import itertools
-import qubovert as qv
+from symmer.operators.utils import binomial_coefficient, perform_noncontextual_sweep
 
 class NoncontextualOp(PauliwordOp):
     """ Class for representing noncontextual Hamiltonians
 
     Noncontextual Hamiltonians are precisely those whose terms may be reconstructed 
     under the Jordan product (AB = {A, B}/2) from a generating set of the form 
     G ∪ {C_1, ..., C_M} where {C_i, C_j}=0 for i != j and G commutes universally.
     Refer to https://arxiv.org/abs/1904.02260 for further details. 
     
     """
+    up_method = 'seq_rot'
+
     def __init__(self,
             symp_matrix,
             coeff_vec
         ):
         """
         """
         super().__init__(symp_matrix, coeff_vec)
         assert(self.is_noncontextual), 'Specified operator is contextual.'
-        self.symmetry_generators, self.clique_operator = self.noncontextual_basis()
+        # extract the symmetry generating set G and clique operator C(r)
+        self.noncontextual_generators()
         # Reconstruct the noncontextual Hamiltonian into its G and C(r) components
         self.noncontextual_reconstruction()
-        # determine the noncontextual ground state - this updates the coefficients of the clique 
-        # representative operator C(r) and symmetry generators G with the optimal configuration
         
     @classmethod
-    def from_PauliwordOp(cls, H):
+    def from_PauliwordOp(cls, H) -> "NoncontextualOp":
         """ for convenience, initialize from an existing PauliwordOp
         """
         noncontextual_operator = cls(
             H.symp_matrix,
             H.coeff_vec
         )
         return noncontextual_operator
 
     @classmethod
     def from_hamiltonian(cls, 
             H: PauliwordOp, 
             strategy: str = 'diag', 
-            basis: PauliwordOp = None, 
+            generators:  PauliwordOp = None,
+            stabilizers: IndependentOp = None, 
             DFS_runtime: int = 10,
+            use_jordan_product = False,
             override_noncontextuality_check: bool = True
         ) -> "NoncontextualOp":
         """ Given a PauliwordOp, extract from it a noncontextual sub-Hamiltonian by the specified strategy
         """
         if not override_noncontextuality_check:
             if H.is_noncontextual:
                 warnings.warn('input H is already noncontextual ignoring strategy')
                 return cls.from_PauliwordOp(H)
         
         if strategy == 'diag':
             return cls._diag_noncontextual_op(H)
-        elif strategy == 'basis':
-            return cls._from_basis_noncontextual_op(H, basis)
+        elif strategy == 'generators':
+            return cls._from_generators_noncontextual_op(H, generators, use_jordan_product=use_jordan_product)
+        elif strategy == 'stabilizers':
+            return cls._from_stabilizers_noncontextual_op(H, stabilizers, use_jordan_product=use_jordan_product)
         elif strategy.find('DFS') != -1:
             _, strategy = strategy.split('_')
             return cls._dfs_noncontextual_op(H, strategy=strategy, runtime=DFS_runtime)
         elif strategy.find('SingleSweep') != -1:
             _, strategy = strategy.split('_')
             return cls._single_sweep_noncontextual_operator(H, strategy=strategy)
         else:
             raise ValueError(f'Unrecognised noncontextual operator strategy {strategy}')
 
     @classmethod
-    def _diag_noncontextual_op(cls, H: PauliwordOp):
+    def _diag_noncontextual_op(cls, H: PauliwordOp) -> "NoncontextualOp":
         """ Return the diagonal terms of the PauliwordOp - this is the simplest noncontextual operator
         """
         mask_diag = np.where(~np.any(H.X_block, axis=1))
         noncontextual_operator = cls(
             H.symp_matrix[mask_diag],
             H.coeff_vec[mask_diag]
         )
         return noncontextual_operator
 
     @classmethod
-    def _dfs_noncontextual_op(cls, H: PauliwordOp, runtime=10, strategy='magnitude'):
+    def _dfs_noncontextual_op(cls, H: PauliwordOp, runtime=10, strategy='magnitude') -> "NoncontextualOp":
         """ function orders operator by coeff mag
         then going from first term adds ops to a pauliword op ensuring it is noncontextual
         adds to a tracking list and then changes the original ordering so first term is now at the end
         repeats from the start (aka generating a list of possible noncon Hamiltonians)
         from this list one can then choose the noncon op with the most terms OR largest sum of abs coeff weights
         cutoff time ensures if the number of possibilities is large the function will STOP and not take too long
 
@@ -100,48 +107,44 @@
         start_time = time()
         while n < H.n_terms and time()-start_time < runtime:
             order = np.roll(np.arange(H.n_terms), -n)
             ordered_operator = PauliwordOp(
                 symp_matrix=operator.symp_matrix[order],
                 coeff_vec=operator.coeff_vec[order]
             )
-            noncontextual_operator = PauliwordOp.empty(H.n_qubits)
-            for op in ordered_operator:
-                noncon_check = noncontextual_operator + op
-                if noncon_check.is_noncontextual:
-                    noncontextual_operator += op
+            noncontextual_operator = perform_noncontextual_sweep(ordered_operator)
             noncontextual_ops.append(noncontextual_operator)
             n+=1
 
         if strategy == 'magnitude':
             noncontextual_operator = sorted(noncontextual_ops, key=lambda x:-np.sum(abs(x.coeff_vec)))[0]
         elif strategy == 'largest':
             noncontextual_operator = sorted(noncontextual_ops, key=lambda x:-x.n_terms)[0]
         else:
             raise ValueError('Unrecognised noncontextual operator strategy.')
 
         return cls.from_PauliwordOp(noncontextual_operator)
 
     @classmethod
-    def _diag_first_noncontextual_op(cls, H: PauliwordOp):
+    def _diag_first_noncontextual_op(cls, H: PauliwordOp) -> "NoncontextualOp":
         """ Start from the diagonal noncontextual form and append additional off-diagonal
         contributions with respect to their coefficient magnitude.
         """
         noncontextual_operator = cls._diag_noncontextual_op(H)
         # order the remaining terms by coefficient magnitude
         off_diag_terms = (H - noncontextual_operator).sort(by='magnitude')
         # append terms that do not make the noncontextual_operator contextual!
         for term in off_diag_terms:
             if (noncontextual_operator+term).is_noncontextual:
                 noncontextual_operator+=term
         
         return cls.from_PauliwordOp(noncontextual_operator)
 
     @classmethod
-    def _single_sweep_noncontextual_operator(cls, H, strategy='magnitude'):
+    def _single_sweep_noncontextual_operator(cls, H, strategy='magnitude') -> "NoncontextualOp":
         """ Order the operator by some sorting key (magnitude, random or CurrentOrder)
         and then sweep accross the terms, appending to a growing noncontextual operator
         whenever possible.
         """
         if strategy=='magnitude':
             operator = H.sort(by='magnitude')
         elif strategy=='random':
@@ -152,191 +155,212 @@
                 H.coeff_vec[order]
             )
         elif strategy =='CurrentOrder':
             operator = H
         else:
             raise ValueError('Unrecognised strategy, must be one of magnitude, random or CurrentOrder')            
 
-        # initialize noncontextual operator with first element of input operator
-        noncon_indices = np.array([0])
-        adjmat = np.array([[True]], dtype=bool)
-        for index, term in enumerate(operator[1:]):
-            # pad the adjacency matrix term-by-term - avoids full construction each time
-            adjmat_vector = np.append(term.commutes_termwise(operator[noncon_indices]), True)
-            adjmat_padded = np.pad(adjmat, pad_width=((0, 1), (0, 1)), mode='constant')
-            adjmat_padded[-1,:] = adjmat_vector; adjmat_padded[:,-1] = adjmat_vector
-            # check whether the adjacency matrix has a noncontextual structure
-            if check_adjmat_noncontextual(adjmat_padded):
-                noncon_indices = np.append(noncon_indices, index+1)
-                adjmat = adjmat_padded
-
-        return cls.from_PauliwordOp(operator[noncon_indices])
+        nc_operator = perform_noncontextual_sweep(operator)
+        return cls.from_PauliwordOp(nc_operator)
 
     @classmethod
-    def _from_basis_noncontextual_op(cls, H: PauliwordOp, generators: PauliwordOp):
-        """ Construct a noncontextual operator given a noncontextual basis, via the Jordan product ( regular matrix product if the operators commute, and equal to zero if the operators anticommute.)
+    def _from_generators_noncontextual_op(cls, 
+            H: PauliwordOp, generators: PauliwordOp, use_jordan_product:bool=False
+        ) -> "NoncontextualOp":
+        """ Construct a noncontextual operator given a noncontextual generating set, via the Jordan product ( regular matrix product if the operators commute, and equal to zero if the operators anticommute.)
         """
-        assert generators is not None, 'Must specify a noncontextual basis.'
-        assert generators.is_noncontextual, 'Basis is contextual.'
-
-        _, noncontextual_terms_mask = H.jordan_generator_reconstruction(generators)
-        return cls.from_PauliwordOp(H[noncontextual_terms_mask])
-
-    def noncontextual_basis(self) -> IndependentOp:
-        """ Find an independent *generating set* for the noncontextual symmetry
-        * technically not a basis!
-        """
-        self.decomposed = {}
-        # identify a basis of universally commuting operators
-        symmetry_generators = IndependentOp.symmetry_generators(self)
-        # try to reconstruct the noncontextual operator in this basis
-        # not all terms can be decomposed in this basis, so check which can
-        reconstructed_indices, succesfully_reconstructed = self.generator_reconstruction(symmetry_generators)
-        # extract the universally commuting noncontextual terms (i.e. those which may be constructed from symmetry generators)
-        universal_operator = PauliwordOp(self.symp_matrix[succesfully_reconstructed],
-                                         self.coeff_vec[succesfully_reconstructed])
-        self.decomposed['symmetry'] = universal_operator
-        # identify the anticommuting cliques
-        clique_union = self - universal_operator
-        if clique_union.n_terms != 0:
-            # identify unique rows in the adjacency matrix with inverse mapping 
-            # so that terms of the same clique have matching indices
-            clique_characters, clique_inverse_map = np.unique(clique_union.adjacency_matrix, axis=0, return_inverse=True)
-            clique_reps = []
-            for i in np.unique(clique_inverse_map):
-                # mask each clique and select a class represetative for its contribution in the noncontextual basis
-                Ci_indices = np.where(clique_inverse_map==i)[0]
-                Ci_symp,Ci_coeff = clique_union.symp_matrix[Ci_indices],clique_union.coeff_vec[Ci_indices]
-                Ci_operator = PauliwordOp(Ci_symp, Ci_coeff)
-                self.decomposed[f'clique_{i}'] = Ci_operator
-                # choose cliques representative that maximises basis_score (summed coefficients of commuting terms)
-                clique_reps.append(Ci_operator.symp_matrix[0])
-            clique_reps = np.vstack(clique_reps)
-            self.n_cliques = clique_reps.shape[0]
-            clique_operator = AntiCommutingOp(clique_reps, np.ones(self.n_cliques))
+        assert generators is not None, 'Must specify a noncontextual generating set.'
+        if use_jordan_product:
+            _, noncontextual_terms_mask = H.jordan_generator_reconstruction(generators)
         else:
-            clique_operator = None
-            self.n_cliques  = 0
-
-        return symmetry_generators, clique_operator
-
-    def noncontextual_reconstruction(self):
-        """ Reconstruct the noncontextual operator in each independent basis GuCi - one for every clique.
-        This mitigates against dependency between the symmetry generators G and the clique representatives Ci
+            assert generators.is_noncontextual, 'Generating set is contextual.'
+            _, noncontextual_terms_mask = H.generator_reconstruction(generators, override_independence_check=True)
+        
+        return cls.from_PauliwordOp(H[noncontextual_terms_mask])
+    
+    @classmethod
+    def _from_stabilizers_noncontextual_op(cls, 
+            H:PauliwordOp, stabilizers: IndependentOp, use_jordan_product=False
+        ) -> "NoncontextualOp":
+        """
+        """
+        symmetries = IndependentOp.symmetry_generators(stabilizers, commuting_override=True)
+        generators = NoncontextualOp.from_hamiltonian(symmetries, strategy='DFS_magnitude')
+        return cls._from_generators_noncontextual_op(H=H, generators=generators, use_jordan_product=use_jordan_product)
+        
+    def draw_graph_structure(self, 
+            clique_lw=1,
+            symmetry_lw=.25,
+            node_colour='black',
+            node_size=20,
+            seed=None,
+            axis=None,
+            include_symmetries=True
+        ):
+        """ Draw the noncontextual graph structure
         """
+        adjmat = self.adjacency_matrix.copy()
+        adjmat = self.adjacency_matrix.copy()
+        index_symmetries = np.where(np.all(adjmat, axis=1))[0]
+        np.fill_diagonal(adjmat, False)
+        
+        G = nx.Graph()
+        for i,j in list(zip(*np.where(adjmat))):
+            if i in index_symmetries or j in index_symmetries:
+                if include_symmetries:
+                    G.add_edge(i,j,color='grey',weight=symmetry_lw)
+            else:
+                G.add_edge(i,j,color='black',weight=clique_lw)
+
+        pos = nx.spring_layout(G, seed=seed)
+        edges = G.edges()
+        colors = [G[u][v]['color'] for u,v in edges]
+        weights = [G[u][v]['weight'] for u,v in edges]
+        nx.draw(G, pos, edge_color=colors, width=weights, 
+                node_color=node_colour, node_size=node_size, ax=axis)
+
+    def noncontextual_generators(self) -> None:
+        """ Find an independent generating set for the noncontextual operator
+        """
+        # identify the symmetry generating set
+        self.symmetry_generators = IndependentOp.symmetry_generators(self, commuting_override=True)
+        # mask the symmetry terms within the noncontextual operator
+        _, symmetry_mask = self.generator_reconstruction(self.symmetry_generators)
+        # identify the reamining commuting cliques
+        self.decomposed = self[~symmetry_mask].clique_cover(edge_relation='C')
+        self.n_cliques = len(self.decomposed)
         if self.n_cliques > 0:
-            reconstruction_ind_matrix = np.zeros(
-                [self.n_terms, self.symmetry_generators.n_terms + self.n_cliques], dtype=int
+            # choose clique representatives with the greatest coefficient
+            self.clique_operator = AntiCommutingOp.from_PauliwordOp(
+                sum([C.sort()[0] for C in self.decomposed.values()])
             )
-            # Cannot simultaneously know eigenvalues of cliques so zero rows with more than one clique
-            # therefore, we decompose the noncontextual terms in the respective independent bases
-            for index, Ci in enumerate(self.clique_operator):
-                clique_column_index = self.symmetry_generators.n_terms+index
-                col_mask_inds = np.append(
-                    np.arange(self.symmetry_generators.n_terms), clique_column_index
-                )
-                GuCi_symp = np.vstack([self.symmetry_generators.symp_matrix, Ci.symp_matrix])
-                GuCi = IndependentOp(GuCi_symp)
-                reconstructed, row_mask_inds = self.generator_reconstruction(GuCi)
-                row_col_mask = np.ix_(row_mask_inds, col_mask_inds)
-                reconstruction_ind_matrix[row_col_mask] = reconstructed[row_mask_inds]
         else:
-            (
-                reconstruction_ind_matrix, 
-                succesfully_reconstructed
-            ) = self.generator_reconstruction(self.symmetry_generators)
+            self.clique_operator = PauliwordOp.empty(self.n_qubits).cleanup()
+        # extract the universally commuting noncontextual terms (i.e. those which may be constructed from symmetry generators)
+        self.decomposed['symmetry'] = self[symmetry_mask]
         
-        G_part = reconstruction_ind_matrix[:,:self.symmetry_generators.n_terms]
-        r_part = reconstruction_ind_matrix[:,self.symmetry_generators.n_terms:]
+    def noncontextual_reconstruction(self) -> None:
+        """ Reconstruct the noncontextual operator in each independent basis GuCi - one for every clique.
+        This mitigates against dependency between the symmetry generators G and the clique representatives Ci
+        """
+        noncon_generators = PauliwordOp(
+            np.vstack([self.symmetry_generators.symp_matrix, self.clique_operator.symp_matrix]),
+            np.ones(self.symmetry_generators.n_terms + self.n_cliques)
+        )
+        # Cannot simultaneously know eigenvalues of cliques so we peform a generator reconstruction
+        # that respects the jordan product A*B = {A, B}/2, i.e. anticommuting elements are zeroed out
+        jordan_recon_matrix, successful = self.jordan_generator_reconstruction(noncon_generators)#, override_independence_check=True)
+        assert(np.all(successful)), 'The generating set is not sufficient to reconstruct the noncontextual Hamiltonian'
+        self.G_indices = jordan_recon_matrix[:, :self.symmetry_generators.n_terms]
+        self.C_indices = jordan_recon_matrix[:, self.symmetry_generators.n_terms:]
+        self.mask_S0 = ~np.any(self.C_indices, axis=1)
+        self.mask_Ci = self.C_indices.astype(bool).T
         # individual elements of r_part commute with all of G_part - taking products over G_part with
         # a single element of r_part will therefore never produce a complex phase, but might result in
-        # a sign slip that must be accounted for in the basis reconstruction TODO: add to generator_reconstruction!
-        pauli_mult_signs = np.ones(self.n_terms)
-        for index, (G, r) in enumerate(zip(G_part, r_part)):
-            G_inds = np.where(G!=0)[0]
-            r_inds = np.where(r!=0)[0]
-            G_component = self.symmetry_generators.symp_matrix[G_inds]
-            if self.n_cliques > 0:
-                r_component = self.clique_operator.symp_matrix[r_inds]
-                all_factors_symp_matrix = np.vstack([G_component, r_component])
-            else:
-                all_factors_symp_matrix = G_component
-            all_factors = PauliwordOp(
-                all_factors_symp_matrix,
-                np.ones(all_factors_symp_matrix.shape[0])
-            )
-            if all_factors.n_terms > 0:
-                gen_mult = reduce(lambda x,y:x*y, list(all_factors))
-                pauli_mult_signs[index] = int(gen_mult.coeff_vec.real[0])
-        self.G_indices, self.r_indices, self.pauli_mult_signs = G_part, r_part, pauli_mult_signs
-
-    def noncontextual_objective_function(self, 
-            nu: np.array, 
-            r: np.array
-        ) -> float:
+        # a sign flip that must be accounted for in the generator reconstruction:
+        multiply_indices = lambda inds:reduce(
+            lambda x,y:x*y, # pairwise multiplication of Pauli factors
+            noncon_generators[inds], # index the relevant noncontextual generating elements
+            PauliwordOp.from_list(['I'*self.n_qubits]) # initialise product with identity
+        ).coeff_vec[0].real
+
+        self.pauli_mult_signs = np.array(
+            list(map(multiply_indices,jordan_recon_matrix.astype(bool)))
+        ).astype(int)
+        
+    def symmetrized_operator(self, expansion_order=1):
+        """ Get the symmetrized noncontextual operator S_0 - sqrt(S_1^2 + .. S_M^2).
+        In the infinite limit of expansion_order the ground state of this operator
+        will coincide exactly with the true noncontextual operator. This is used
+        for xUSO solver since this reformulation of the Hamiltonian is polynomial.
+        """
+        Si_list = [self.decomposed['symmetry']]
+        for i in range(self.n_cliques):
+            Ci = self.decomposed[i][0]; Ci.coeff_vec[0]=1
+            Si = Ci*self.decomposed[i]
+            Si_list.append(Si)
+
+        S = sum([Si**2 for Si in Si_list[1:]])
+        norm = np.linalg.norm(S.coeff_vec, ord=2)
+        S *= (1/norm)
+        I = PauliwordOp.from_list(['I'*self.n_qubits])
+        terms = [
+            (I-S)**n * (-1)**n * binomial_coefficient(.5, n) 
+            for n in range(expansion_order+1)
+        ] # power series expansion of the oeprator root
+        S_root = sum(terms) * np.sqrt(norm)
+        
+        return Si_list[0] - S_root
+
+    def get_symmetry_contributions(self, nu: np.array) -> float:
+        """
+        """
+        nu = np.asarray(nu)
+        coeff_mod =  (
+            # coefficient vector whose signs we are modifying:
+            self.coeff_vec *
+            # sign flips from generator reconstruction:
+            self.pauli_mult_signs *
+            # sign flips from nu assignment:
+            (-1)**np.count_nonzero(np.logical_and(self.G_indices==1, nu == -1), axis=1)
+        )
+        s0 = np.sum(coeff_mod[self.mask_S0]).real
+        si = np.array([np.sum(coeff_mod[mask]).real for mask in self.mask_Ci])
+        return s0, si
+
+    def get_energy(self, nu: np.array) -> float:
         """ The classical objective function that encodes the noncontextual energies
         """
-        nu = np.asarray(nu, dtype=int) # must be an array!
-        G_prod = (-1)**np.count_nonzero(np.logical_and(self.G_indices==1, nu == -1), axis=1)
-        r_part = np.sum(self.r_indices*r, axis=1)
-        r_part[~np.any(self.r_indices, axis=1)]=1
-        return np.sum(self.coeff_vec*G_prod*r_part*self.pauli_mult_signs).real
-
-    def _convex_problem(self, nu):
-        """ given +/-1 value assignments nu, solve for the clique operator coefficients.
-        Note that, with nu fixed, the optimization problem is now convex.
-        """
-        if self.n_cliques==0:
-            optimized_energy = self.noncontextual_objective_function(nu=nu, r=None)
-            r_optimal = None
-        else:
-            # given M cliques, optimize over the unit (M-1)-sphere and convert to cartesians for the r vector
-            r_bounds = [(0, np.pi)]*(self.n_cliques-2)+[(0, 2*np.pi)]
-            optimizer_output = differential_evolution(
-                func=lambda angles:self.noncontextual_objective_function(
-                    nu, unit_n_sphere_cartesian_coords(angles)
-                    ), 
-                bounds=r_bounds
-            )
-            optimized_energy = optimizer_output['fun']
-            optimized_angles = optimizer_output['x']
-            r_optimal = unit_n_sphere_cartesian_coords(optimized_angles)
-
-        return optimized_energy, r_optimal
-
+        s0, si = self.get_symmetry_contributions(nu)
+        return s0 - np.linalg.norm(si)
+    
+    def update_clique_representative_operator(self, clique_index:int = None) -> List[Tuple[PauliwordOp, float]]:
+        _, si = self.get_symmetry_contributions(self.symmetry_generators.coeff_vec)
+        self.clique_operator.coeff_vec = si
+        if clique_index is None:
+            clique_index = 0
+        (
+            self.mapped_clique_rep, 
+            self.unitary_partitioning_rotations, 
+            self.clique_normalization,
+            self.clique_operator
+        ) = self.clique_operator.unitary_partitioning(up_method=self.up_method, s_index=clique_index)
+        
     def solve(self, 
             strategy: str = 'brute_force', 
             ref_state: np.array = None, 
             num_anneals:int = 1_000,
-            discrete_optimization_order = 'first'
+            expansion_order:int = 1
         ) -> None:
-        """ Minimize the classical objective function, yielding the noncontextual ground state
+        """ Minimize the classical objective function, yielding the noncontextual 
+        ground state. This updates the coefficients of the clique representative 
+        operator C(r) and symmetry generators G with the optimal configuration.
 
         Note most QUSO functions/methods work faster than their PUSO counterparts.
+
         """
-        
         if ref_state is not None:
             # update the symmetry generator G coefficients w.r.t. the reference state
             self.symmetry_generators.update_sector(ref_state)
             ev_assignment = self.symmetry_generators.coeff_vec
             fixed_ev_mask = ev_assignment!=0
             fixed_eigvals = (ev_assignment[fixed_ev_mask]).astype(int)
             NC_solver = NoncontextualSolver(self, fixed_ev_mask, fixed_eigvals)
             # any remaining unfixed symmetry generators are solved via other means:
         else:
             NC_solver = NoncontextualSolver(self)
 
         NC_solver.num_anneals = num_anneals
-        NC_solver.discrete_optimization_order = discrete_optimization_order
+        NC_solver.expansion_order = expansion_order
 
         if strategy=='brute_force':
-            self.energy, nu, r = NC_solver.energy_via_brute_force()
+            self.energy, nu = NC_solver.energy_via_brute_force()
 
         elif strategy=='binary_relaxation':
-            self.energy, nu, r = NC_solver.energy_via_relaxation()
+            self.energy, nu = NC_solver.energy_via_relaxation()
         
         else:
             #### qubovert strategies below this point ####
             # PUSO = Polynomial unconstrained spin Optimization
             # QUSO: Quadratic Unconstrained Spin Optimization
             if strategy == 'brute_force_PUSO':
                 NC_solver.method = 'brute_force'
@@ -349,141 +373,33 @@
                 NC_solver.x = 'P'
             elif strategy == 'annealing_QUSO':
                 NC_solver.method = 'annealing'
                 NC_solver.x = 'Q'
             else:
                 raise ValueError(f'Unknown optimization strategy: {strategy}')
         
-            self.energy, nu, r = NC_solver.energy_xUSO()
+            self.energy, nu = NC_solver.energy_xUSO()
 
         # optimize the clique operator coefficients
         self.symmetry_generators.coeff_vec = nu.astype(int)
-        if r is not None:
-            self.clique_operator.coeff_vec = r
-
-    def get_qaoa(self, ref_state:QuantumState=None, type='qubo') -> dict:
-        """
-        For a given PUBO / QUBO problem make the following replacement:
-
-         𝑥_𝑖 <--> (𝐼−𝑍_𝑖) / 2
-
-         This defined the QAOA Hamiltonian
-        Args:
-            ref_state (optional): optional QuantumState to fix symmetry generators with
-        Returns:
-            QAOA_dict (dict): Dictionary of different QAOA Hamiltonians from discrete r_vectors
-
-        """
-        assert type in ['qubo', 'pubo']
-
-        # fix symm generators if reference state given
-        if ref_state is not None:
-            # update the symmetry generator G coefficients w.r.t. the reference state
-            self.symmetry_generators.update_sector(ref_state)
-            ev_assignment = self.symmetry_generators.coeff_vec
-            fixed_ev_mask = ev_assignment!=0
-            fixed_eigvals = (ev_assignment[fixed_ev_mask]).astype(int)
-        else:
-            fixed_ev_mask = np.zeros(self.symmetry_generators.n_terms, dtype=bool)
-            fixed_eigvals = np.array([], dtype=int)
-
-
-        fixed_indices = np.where(fixed_ev_mask)[0]  # bool to indices
-        fixed_assignments = dict(zip(fixed_indices, fixed_eigvals))
-
-        r_vec_size = self.clique_operator.n_terms
-        QAOA_dict = {}
-        for j in range(r_vec_size):
-
-            ## set extreme values of r_vec
-            r_vec = np.zeros(r_vec_size)
-            r_vec[j]=1
-
-            r_part = np.sum(self.r_indices * r_vec, axis=1)
-            r_part[~np.any(self.r_indices, axis=1)] = 1  # set all zero terms to 1 (aka multiply be value of 1)
-
-            # setup spin
-            q_vec_SPIN = {}
-            for ind in range(self.symmetry_generators.n_terms):
-                if ind in fixed_assignments.keys():
-                    q_vec_SPIN[ind] = fixed_assignments[ind]
-                else:
-                    q_vec_SPIN[ind] = qv.spin_var('x%d' % ind)
-
-
-            ## setup cost function
-            COST = 0
-            for P_index, term in enumerate(self.G_indices):
-                non_zero_inds = term.nonzero()[0]
-                # collect all the spin terms
-                G_term = 1
-                for i in non_zero_inds:
-                    G_term *= q_vec_SPIN[i]
-
-                COST += G_term * self.coeff_vec[P_index].real * self.pauli_mult_signs[P_index] * r_part[P_index].real
-
-            if not isinstance(COST, qv._pcso.PCSO):
-                # no degrees of freedom... Cost function is just Identity term
-                QAOA_dict[j] = {
-                    'r_vec': r_vec,
-                    'H':PauliwordOp.from_dictionary({'I'*self.n_qubits: COST}),
-                    'qubo': None
-                }
-            else:
-
-                # make a spin/binary problem
-                if type == 'qubo':
-                    QUBO_problem = COST.to_qubo()
-                elif type == 'pubo':
-                    QUBO_problem = COST.to_pubo()
-                else:
-                    raise ValueError(f'unknown tspin problem: {type}')
-
-                # note mapping often requires more qubits!
-                QAOA_n_qubits = QUBO_problem.max_index+1
-
-                I_string = 'I' * QAOA_n_qubits
-                QAOA_H = PauliwordOp.empty(QAOA_n_qubits)
-                for spin_inds, coeff in QUBO_problem.items():
-
-                    if len(spin_inds) == 0:
-                        QAOA_H += PauliwordOp.from_dictionary({I_string: coeff})
-                    else:
-                        temp = PauliwordOp.from_dictionary({I_string: coeff})
-                        for q_ind in spin_inds:
-                            op = list(I_string)
-                            op[q_ind] = 'Z'
-                            op_str = ''.join(op)
-                            Qop = PauliwordOp.from_dictionary({I_string: 0.5,
-                                                               op_str: -0.5})
-                            temp *= Qop
-
-                        QAOA_H += temp
-
-                QAOA_dict[j] = {
-                    'r_vec': r_vec,
-                    'H': QAOA_H.copy(),
-                    'qubo': dict(QUBO_problem.items())
-                }
-
-        return QAOA_dict
-
+        if self.n_cliques > 0:
+            self.update_clique_representative_operator()
+        
 ###############################################################################
 ################### NONCONTEXTUAL SOLVERS BELOW ###############################
 ###############################################################################
 
 class NoncontextualSolver:
 
     # xUSO settings
     method:str = 'brute_force'
     x:str = 'P'
     num_anneals:int = 1_000,
-    discrete_optimization_order:str = 'first'
-    reoptimize_r_vec:bool = False
-    _nu = None
+    _nu = None,
+    expansion_order=1
 
     def __init__(
         self,
         NC_op: NoncontextualOp,
         fixed_ev_mask: np.array = None,
         fixed_eigvals: np.array = None
         ) -> None:
@@ -501,33 +417,33 @@
     #################################################################
     ########################## BRUTE FORCE ##########################
     #################################################################
 
     def energy_via_brute_force(self) -> Tuple[float, np.array, np.array]:
         """ Does what is says on the tin! Try every single eigenvalue assignment in parallel
         and return the minimizing noncontextual configuration. This scales exponentially in 
-        the number of qubits.
+        the number of unassigned symmetry elements.
         """
         if np.all(self.fixed_ev_mask):
             nu_list = self.fixed_eigvals.reshape([1,-1])
         else:
             search_size = 2**np.sum(~self.fixed_ev_mask)
             nu_list = np.ones([search_size, self.NC_op.symmetry_generators.n_terms], dtype=int)
             nu_list[:,self.fixed_ev_mask] = np.tile(self.fixed_eigvals, [search_size,1])
             nu_list[:,~self.fixed_ev_mask] = np.array(list(itertools.product([-1,1],repeat=np.sum(~self.fixed_ev_mask))))
         
-        # optimize over all discrete value assignments of nu in parallel
+        # # optimize over all discrete value assignments of nu in parallel
         with mp.Pool(mp.cpu_count()) as pool:    
-            tracker = pool.map(self.NC_op._convex_problem, nu_list)
+            tracker = pool.map(self.NC_op.get_energy, nu_list)
         
         # find the lowest energy eigenvalue assignment from the full list
         full_search_results = zip(tracker, nu_list)
-        (energy, r_optimal), fixed_nu = min(full_search_results, key=lambda x:x[0][0])
+        energy, fixed_nu = min(full_search_results, key=lambda x:x[0])
 
-        return energy, fixed_nu, r_optimal
+        return energy, fixed_nu
 
     #################################################################
     ###################### BINARY RELAXATION ########################
     #################################################################
 
     def energy_via_relaxation(self) -> Tuple[float, np.array, np.array]:
         """ Relax the binary value assignment of symmetry generators to continuous variables
@@ -539,144 +455,103 @@
             """ Build nu vector given fixed values
             """
             nu = np.ones(self.NC_op.symmetry_generators.n_terms)
             nu[self.fixed_ev_mask] = self.fixed_eigvals
             nu[~self.fixed_ev_mask] = np.cos(angles)
             return nu
 
-        optimizer_output = shgo(func=lambda angles:self.NC_op._convex_problem(get_nu(angles))[0], bounds=nu_bounds)
+        optimizer_output = shgo(func=lambda angles:self.NC_op.get_energy(get_nu(angles)), bounds=nu_bounds)
         # if optimization was successful the optimal angles should consist of 0 and pi
         fix_nu = np.sign(np.array(get_nu(np.cos(optimizer_output['x'])))).astype(int)
         self.NC_op.symmetry_generators.coeff_vec = fix_nu 
-        energy, r_optimal = self.NC_op._convex_problem(fix_nu)
-        return energy, fix_nu, r_optimal
+        return optimizer_output['fun'], fix_nu
     
     #################################################################
     ################ UNCONSTRAINED SPIN OPTIMIZATION ################
     #################################################################    
-    
-    def _energy_xUSO(self, r_vec: np.array) -> Tuple[float, np.array, np.array]:
+
+    def get_cost_func(self):
+        """ Define the unconstrained spin cost function
+        """
+        symmetrized_operator = self.NC_op.symmetrized_operator(expansion_order=self.expansion_order)
+        G_indices, _ = symmetrized_operator.generator_reconstruction(self.NC_op.symmetry_generators)
+        # setup spin variables
+        fixed_indices = np.where(self.fixed_ev_mask)[0] # bool to indices
+        fixed_assignments = dict(zip(fixed_indices, self.fixed_eigvals))
+        q_vec_SPIN={}
+        for ind in range(self.NC_op.symmetry_generators.n_terms):
+            if ind in fixed_assignments.keys():
+                q_vec_SPIN[ind] = fixed_assignments[ind]
+            else:
+                q_vec_SPIN[ind] = qv.spin_var('x%d' % ind)
+
+        COST = 0
+        for P_index, term in enumerate(G_indices):
+            non_zero_inds = term.nonzero()[0]
+            # collect all the spin terms
+            G_term = 1
+            for i in non_zero_inds:
+                G_term *= q_vec_SPIN[i]
+
+            # cost function
+            COST += (
+                G_term * 
+                symmetrized_operator.coeff_vec[P_index].real
+                #self.NC_op.pauli_mult_signs[P_index]# * 
+                #r_part[P_index].real
+            )
+
+        return COST
+
+    def energy_xUSO(self) -> Tuple[float, np.array, np.array]:
         """
         Get energy via either: Polynomial unconstrained spin Optimization (x=P)
                                     or
                                 Quadratic Unconstrained Spin Optimization  (x=Q)
 
         via a brute force search over q_vector or via simulated annealing
 
         Note in this method the r_vector is fixed upon input! (aka just does binary optimization)
 
         Args:
             NC_op (NoncontextualOp): noncontextual operator
-            r_vec (np.array): array of clique expectation values <r_i>
             fixed_ev_mask (np.array): bool list of where eigenvalues in nu vector are fixed
             fixed_eigvals (np.array): list of nu eigenvalues that are fixed
             method (str): brute force or annealing optimization
             x (str): Whether method is Polynomial or Quadratic optimization
             num_anneals (optional): number of simulated anneals to do
 
         Returns:
             energy (float): noncontextual energy
 
         """
         assert self.x in ['P', 'Q']
         assert self.method in ['brute_force', 'annealing']
         
-        r_part = np.sum(self.NC_op.r_indices * r_vec, axis=1)
-        r_part[~np.any(self.NC_op.r_indices, axis=1)] = 1  # set all zero terms to 1 (aka multiply be value of 1)
+        COST = self.get_cost_func()
         
-        # setup spin variables
-        fixed_indices = np.where(self.fixed_ev_mask)[0] # bool to indices
-        fixed_assignments = dict(zip(fixed_indices, self.fixed_eigvals))
-        q_vec_SPIN={}
-        for ind in range(self.NC_op.symmetry_generators.n_terms):
-            if ind in fixed_assignments.keys():
-                q_vec_SPIN[ind] = fixed_assignments[ind]
-            else:
-                q_vec_SPIN[ind] = qv.spin_var('x%d' % ind)
-
-        COST = 0
-        for P_index, term in enumerate(self.NC_op.G_indices):
-            non_zero_inds = term.nonzero()[0]
-            # collect all the spin terms
-            G_term = 1
-            for i in non_zero_inds:
-                G_term *= q_vec_SPIN[i]
-
-            # cost function
-            COST += G_term * self.NC_op.coeff_vec[P_index].real * self.NC_op.pauli_mult_signs[P_index] * r_part[P_index].real
-
         if np.all(self.fixed_ev_mask):
             # if no degrees of freedom over nu vector, COST is a number
-            self._nu = self.fixed_eigvals
-            return COST, self.fixed_eigvals, r_vec
-
-        if self.x =='P':
-            spin_problem = COST.to_puso()
+            nu_vec = self.fixed_eigvals
         else:
-            spin_problem = COST.to_quso()
-
-        if self.method=='brute_force':
-            sol = spin_problem.solve_bruteforce()
-        elif self.method == 'annealing':
-            if self.x == 'P':
-                puso_res = qv.sim.anneal_puso(spin_problem, num_anneals=self.num_anneals)
-            elif self.x == 'Q':
-                puso_res= qv.sim.anneal_quso(spin_problem, num_anneals=self.num_anneals)
-                assert COST.is_solution_valid(puso_res.best.state) is True
-            sol = puso_res.best.state
-
-        solution = COST.convert_solution(sol)
-        energy = COST.value(solution)
-        nu_vec = np.ones(self.NC_op.symmetry_generators.n_terms, dtype=int)
-        nu_vec[self.fixed_ev_mask] = self.fixed_eigvals
-        nu_vec[~self.fixed_ev_mask] = np.array(list(solution.values()))
-        self._nu = nu_vec # so nu accessible during the _convex_then_xUSO optimization 
-
-        if self.reoptimize_r_vec:
-            opt_energy, opt_r_vec = self.NC_op._convex_problem(nu_vec)
-            return opt_energy, nu_vec, opt_r_vec
-        else:
-            return energy, nu_vec, r_vec
-    
-    def _xUSO_then_convex(self) -> Tuple[float, np.array, np.array]:
-        """
-        """
-        self.reoptimize_r_vec = True
-        
-        extreme_r_vecs = np.eye(self.NC_op.n_cliques, dtype=int)
-        extreme_r_vecs = np.vstack([extreme_r_vecs, -extreme_r_vecs])
-        
-        with mp.Pool(mp.cpu_count()) as pool:    
-            tracker = pool.map(self._energy_xUSO, extreme_r_vecs)
-
-        return sorted(tracker, key=lambda x:x[0])[0]
-    
-    def _convex_then_xUSO(self) -> Tuple[float, np.array, np.array]:
-        """
-        """
-        self.reoptimize_r_vec = False
+            if self.x =='P':
+                spin_problem = COST.to_puso()
+            else:
+                spin_problem = COST.to_quso()
 
-        r_bounds = [(0, np.pi)]*(self.NC_op.n_cliques-2)+[(0, 2*np.pi)]
-    
-        optimizer_output = differential_evolution(
-            func=lambda angles:self._energy_xUSO(
-                unit_n_sphere_cartesian_coords(angles)
-            )[0],
-            bounds=r_bounds
-        )
-        optimized_energy = optimizer_output['fun']
-        optimized_angles = optimizer_output['x']
-        r_optimal = unit_n_sphere_cartesian_coords(optimized_angles)
+            if self.method=='brute_force':
+                sol = spin_problem.solve_bruteforce()
+            elif self.method == 'annealing':
+                if self.x == 'P':
+                    puso_res = qv.sim.anneal_puso(spin_problem, num_anneals=self.num_anneals)
+                elif self.x == 'Q':
+                    puso_res= qv.sim.anneal_quso(spin_problem, num_anneals=self.num_anneals)
+                    assert COST.is_solution_valid(puso_res.best.state) is True
+                sol = puso_res.best.state
+
+            solution = COST.convert_solution(sol)
+            nu_vec = np.ones(self.NC_op.symmetry_generators.n_terms, dtype=int)
+            nu_vec[self.fixed_ev_mask] = self.fixed_eigvals
+            # must ensure the binary variables are correctly ordered in the solution:
+            nu_vec[~self.fixed_ev_mask] = np.array([solution[f'x{i}'] for i in range(COST.num_binary_variables)])
         
-        return optimized_energy, self._nu, r_optimal
-    
-    def energy_xUSO(self) -> Tuple[float, np.array, np.array]:
-        """
-        """
-        if self.NC_op.n_cliques == 0:
-            return self._energy_xUSO(None)
-        elif self.discrete_optimization_order == 'first':
-            return self._xUSO_then_convex()
-        elif self.discrete_optimization_order == 'last':
-            return self._convex_then_xUSO()
-        else:
-            raise ValueError('Unrecognised discrete optimization order, must be first or last')
+        return self.NC_op.get_energy(nu_vec), nu_vec
```

### Comparing `symmer-0.0.2/symmer/operators/utils.py` & `symmer-0.0.3/symmer/operators/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
     """
     n_qubits = len(symp_vec) // 2
 
     X_block = symp_vec[:n_qubits]
     Z_block = symp_vec[n_qubits:]
 
-    Y_loc = np.bitwise_and(X_block, Z_block).astype(bool)
-    X_loc = np.bitwise_xor(Y_loc, X_block).astype(bool)
-    Z_loc = np.bitwise_xor(Y_loc, Z_block).astype(bool)
+    Y_loc = np.logical_and(X_block, Z_block)
+    X_loc = np.logical_xor(Y_loc, X_block)
+    Z_loc = np.logical_xor(Y_loc, Z_block)
 
     char_aray = np.array(list('I' * n_qubits), dtype=str)
 
     char_aray[Y_loc] = 'Y'
     char_aray[X_loc] = 'X'
     char_aray[Z_loc] = 'Z'
 
@@ -190,15 +190,15 @@
     """ Column-reduced echelon form with static columns (used in symmetry identification)
     """
     return _rref_binary(matrix.T).T  
 
 def cref_binary(matrix: np.array) -> np.array:
     """ Column-reduced echelon form with ordered columns (used in basis reconstruction)
     """
-    return rref_binary(matrix.T).T         
+    return rref_binary(matrix.T).T        
 
 def QubitOperator_to_dict(op, num_qubits):
     """ OpenFermion
     """
     assert(type(op) == of.QubitOperator)
     op_dict = {}
     term_dict = op.terms
@@ -297,14 +297,40 @@
     """ Input an array of angles of length n, returns the n+1 cartesian coordinates 
     of the corresponding unit n-sphere in (n+1)-dimensional Euclidean space.
     """
     cartesians = [np.prod(np.sin(angles[:i]))*np.cos(angles[i]) for i in range(len(angles))]
     cartesians.append(np.prod(np.sin(angles)))
     return np.array(cartesians)
 
+def binomial_coefficient(n,k):
+    """ Calculate the binomial coefficient n choose k
+    Differs from np.math.comb as this allows non-integer n
+    """
+    prod = 1
+    for r in range(k):
+        prod *= (n-r)/(k-r) 
+    return prod
+
+def check_independent(operators):
+    """ Check if the input PauliwordOp contains algebraically dependent terms
+    """
+    check_independent = _rref_binary(operators.symp_matrix)
+    return ~np.any(np.all(~check_independent, axis=1))
+
+def check_jordan_independent(operators):
+    """ Check if the input PauliwordOp contains algebraically dependent terms
+    """
+    mask_symmetries = np.all(operators.adjacency_matrix, axis=1)
+    Symmetries = operators[mask_symmetries]
+    Anticommuting = operators[~mask_symmetries]
+    return (
+        check_independent(Symmetries) & 
+        np.all(Anticommuting.adjacency_matrix == np.eye(Anticommuting.n_terms))
+    )
+
 def check_adjmat_noncontextual(adjmat) -> bool:
     """ Check whether the input boolean square matrix has a noncontextual structure...
     ... see https://doi.org/10.1103/PhysRevLett.123.200501 for details.
     """
     # mask the terms that do not commute universally amongst the operator
     mask_non_universal = np.where(~np.all(adjmat, axis=1))[0]
     # look only at the unique rows in the masked adjacency matrix -
@@ -314,23 +340,50 @@
         axis=0
     )
     # if the unique commutation characteristics are disjoint, i.e. no overlapping ones 
     # between rows, the operator is noncontextual - hence we sum over rows and check
     # the resulting vector consists of all ones.
     return np.all(np.count_nonzero(unique_commutation_character, axis=0)==1)
 
-def check_independent(operators):
-    """ Check if the input PauliwordOp contains algebraically dependent terms
+def perform_noncontextual_sweep(operator):
+    """ Given an ordered operator, sweep over its terms and append 
+    to a list if the newly appended term maintains noncontextuality.
+    """
+    # initialize noncontextual operator with first element of input operator
+    noncon_indices = np.array([0])
+    adjmat = np.array([[True]], dtype=bool)
+    for index, term in enumerate(operator[1:]):
+        # pad the adjacency matrix term-by-term - avoids full construction each time
+        adjmat_vector = np.append(term.commutes_termwise(operator[noncon_indices]), True)
+        adjmat_padded = np.pad(adjmat, pad_width=((0, 1), (0, 1)), mode='constant')
+        adjmat_padded[-1,:] = adjmat_vector; adjmat_padded[:,-1] = adjmat_vector
+        # check whether the adjacency matrix has a noncontextual structure
+        if check_adjmat_noncontextual(adjmat_padded):
+            noncon_indices = np.append(noncon_indices, index+1)
+            adjmat = adjmat_padded
+
+    return operator[noncon_indices] 
+
+def binary_array_to_int(bin_arr):
     """
-    check_independent = _rref_binary(operators.symp_matrix)
-    return ~np.any(np.all(~check_independent, axis=1))
+    function to convert an array composed of rows of binary into integars
+
+    Args:
+        bin_arr(np.array): 2D numpy array of binary
+    Returns:
+        int_arr (np.array): 1D numpy array of ints
 
-def check_jordan_independent(operators):
-    """ Check if the input PauliwordOp contains algebraically dependent terms
     """
-    mask_symmetries = np.all(operators.adjacency_matrix, axis=1)
-    Symmetries = operators[mask_symmetries]
-    Anticommuting = operators[~mask_symmetries]
-    return (
-        check_independent(Symmetries) & 
-        np.all(Anticommuting.adjacency_matrix == np.eye(Anticommuting.n_terms))
-    )
+
+    if bin_arr.shape[1] < 64:
+        b2i = 2 ** np.arange(bin_arr.shape[1] - 1, -1, -1)
+    else:
+        b2i = 2 ** np.arange(bin_arr.shape[1] - 1, -1, -1, dtype=float)
+        # b2i = 2 ** np.arange(bin_arr.shape[1] - 1, -1, -1, dtype=object)
+
+    int_arr = np.einsum('j, ij->i', b2i, bin_arr)
+    # int_arr = (b2i*bin_arr).sum(axis=1)
+
+    ## slower as does matrix product rather than multiplication along rows followed by a sum!
+    # int_arr = bin_arr @ b2i
+
+    return int_arr
```

### Comparing `symmer-0.0.2/symmer/projection/base.py` & `symmer-0.0.3/symmer/projection/base.py`

 * *Files identical despite different names*

### Comparing `symmer-0.0.2/symmer/projection/contextual_subspace.py` & `symmer-0.0.3/symmer/projection/contextual_subspace.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
-from symmer.operators import PauliwordOp, IndependentOp, NoncontextualOp
+from symmer.operators import PauliwordOp, IndependentOp, NoncontextualOp, QuantumState
 from symmer.projection.utils import (
     update_eigenvalues, StabilizerIdentification, ObservableBiasing, stabilizer_walk
 )
 from symmer.projection import S3_projection
+from symmer.evolution import trotter
 from typing import List, Union, Optional
 
 class ContextualSubspace(S3_projection):
     """ Class for performing contextual subspace methods as per https://quantum-journal.org/papers/q-2021-05-14-456/.
     Reduces the number of qubits in the problem while aiming to control the systematic error incurred along the way.
 
     This class handles the following:
@@ -24,149 +25,114 @@
     6. fixing the +/-1 eigenvalues
     """
     def __init__(self,
             operator: PauliwordOp,
             noncontextual_strategy: str = 'diag',
             noncontextual_solver: str = 'brute_force',
             num_anneals:Optional[int] = 1000,
-            discrete_optimization_order = 'first',
-            unitary_partitioning_method: str = 'LCU',
-            reference_state: np.array = None,
+            unitary_partitioning_method: str = 'seq_rot',
+            reference_state: Union[np.array, QuantumState] = None,
             noncontextual_operator: NoncontextualOp = None,
+            noncontextual_expansion_order: int = 1
         ):
         """
         """
         # noncontextual startegy will have the form x_y, where x is the actual strategy
         # and y is some supplementary method indicating a sorting key such as magnitude
-        self.ref_state = reference_state
+        if reference_state is None or isinstance(reference_state, QuantumState):
+            self.ref_state = reference_state
+        else:
+            self.ref_state = QuantumState(reference_state)            
         extract_noncon_strat = noncontextual_strategy.split('_')
         self.nc_strategy = extract_noncon_strat[0]
         self.noncontextual_solver = noncontextual_solver
         self.num_anneals = num_anneals
-        self.discrete_optimization_order = discrete_optimization_order
-        if self.nc_strategy=='StabilizeFirst':
-            self.stabilize_first_method = extract_noncon_strat[1]
+        self.noncontextual_expansion_order = noncontextual_expansion_order
         # With the exception of the StabilizeFirst noncontextual strategy, here we build
         # the noncontextual Hamiltonian in line with the specified strategy
         self.operator = operator
         if noncontextual_operator is None and self.nc_strategy != 'StabilizeFirst':
             self.noncontextual_operator = NoncontextualOp.from_hamiltonian(
                 operator, strategy=noncontextual_strategy
             )
         else:
             self.noncontextual_operator = noncontextual_operator
-        self._noncontextual_update()
         self.unitary_partitioning_method = unitary_partitioning_method
-    
-    def _noncontextual_update(self):
-        """ To be executed each time the noncontextual operator is updated.
-        """
-        if self.noncontextual_operator is not None:
-            self.contextual_operator = self.operator - self.noncontextual_operator
-            if self.contextual_operator.n_terms == 0:
-                raise ValueError('The Hamiltonian is noncontextual, the contextual subspace is empty.')
-            self.noncontextual_operator.solve(
-                strategy=self.noncontextual_solver, 
-                ref_state=self.ref_state, 
-                num_anneals=self.num_anneals,
-                discrete_optimization_order=self.discrete_optimization_order
-            )
-            self.n_cliques = self.noncontextual_operator.n_cliques
+        self._noncontextual_update()
 
     def manual_stabilizers(self, S: Union[List[str], IndependentOp]) -> None:
         """ Specify a set of operators to enforce manually
         """
         if isinstance(S, list):
             S = IndependentOp.from_list(S)
         self.n_qubits_in_subspace = self.operator.n_qubits - S.n_terms
+        if self.n_qubits_in_subspace == 0:
+            self.return_NC = True
+        else:
+            self.return_NC = False
         self.stabilizers = S
+        self._prepare_stabilizers()
 
     def update_stabilizers(self, 
             n_qubits: int, 
             strategy: str = 'aux_preserving',
             aux_operator: PauliwordOp = None,
-            depth: int = 2,
-            n_cliques: int = 2,
-            n_stabilizers_in_clique: int = 1,
             HF_array: np.array = None,
             use_X_only: bool = True
         ) -> None:
         """ Update the stabilizers that will be used for the subspace projection
         """
         assert(n_qubits<=self.operator.n_qubits), (
             'Cannot define a contextual subspace larger than the base Hamiltonian'
         )
-        # will ensure one too few stabilizers will be selected, with the 
-        # additional one identified via the following clique expansion step
-        if self.nc_strategy=='StabilizeFirst':
-            if self.stabilize_first_method=='magnitude':
-                n_qubits += 1
-
-        if strategy == 'aux_preserving':
-            S = self._aux_operator_preserving_stabilizer_search(
-                n_qubits=n_qubits, aux_operator=aux_operator, use_X_only=use_X_only
-            )
-        elif strategy == 'greedy_search':
-            S = self._greedy_stabilizer_search(
-                n_qubits=n_qubits, depth=depth
-            )
-        elif strategy == 'random':
-            S = self._random_stabilizers(
-                n_qubits=n_qubits
-            )
-        elif strategy == 'HOMO_LUMO_biasing':
-            S = self._HOMO_LUMO_biasing(
-                n_qubits=n_qubits, HF_array=HF_array, 
-                weighting_operator=aux_operator, use_X_only=use_X_only
-            )
+        if n_qubits == 0:
+            n_qubits = 1
+            self.return_NC = True
         else:
-            raise ValueError('Unrecognised stabilizer search strategy.')
-
-        self.n_qubits_in_subspace = self.operator.n_qubits - S.n_terms
-        self.stabilizers = S
+            self.return_NC = False
 
-        # the StabilizeFirst strategy differs from the others in that the noncontextual
-        # Hamiltonian is constructed AFTER selecting stabilizers, which is what we do next:
-        if self.nc_strategy == 'StabilizeFirst':
-            if self.stabilize_first_method == 'commuting':
-                assert n_stabilizers_in_clique < self.stabilizers.n_terms, 'At least one stabilizer must be assigned to the symmetry generating set.'
-                # move stabilizers into a clique by increasing commutativity with full Hamiltonian
-                stabilizer_commutativity_count = np.count_nonzero(
-                    self.stabilizers.commutes_termwise(self.operator), axis=1
+        if n_qubits == self.operator.n_qubits:
+            self.stabilizers = None
+        else:
+            if strategy == 'aux_preserving':
+                S = self._aux_operator_preserving_stabilizer_search(
+                    n_qubits=n_qubits, aux_operator=aux_operator, use_X_only=use_X_only
                 )
-                order_by_commutativity = np.argsort(stabilizer_commutativity_count)
-                force_clique_rep = self.stabilizers[order_by_commutativity][:n_stabilizers_in_clique]
-                force_symmetries = self.stabilizers[order_by_commutativity][1+n_stabilizers_in_clique:]
-                sum_clique_reps = self._get_clique_representatives(
-                    symmetry_terms=force_symmetries, n_cliques=n_cliques, clique_reps=[force_clique_rep]
+            elif strategy == 'random':
+                S = self._random_stabilizers(
+                    n_qubits=n_qubits
                 )
-            elif self.stabilize_first_method == 'magnitude':
-                # find list of anticommuting operators that commute with the stabilizers, selected by coefficient magnitude
-                sum_clique_reps = self._get_clique_representatives(n_cliques=n_cliques, clique_reps=[])
-                # choose the dominant term to be enforced in noncontextual solution
-                extra_stabilizer = sum_clique_reps.sort(by='magnitude')[0]
-                extra_stabilizer.coeff_vec[0]=1
-                self.stabilizers += extra_stabilizer
-
-            # find symmetry generators given a sum of anticommuting operators
-            symgen = IndependentOp.symmetry_generators(sum_clique_reps+self.stabilizers)
-            # this forms a noncontextual generating set under the Jordan product
-            noncon_basis = symgen*1 + sum_clique_reps
-            self.noncontextual_operator = NoncontextualOp.from_hamiltonian(strategy='basis', H=self.operator, basis=noncon_basis)
-            # finally, solve the noncontextual optimization problem
-            self._noncontextual_update()
+            elif strategy == 'HOMO_LUMO_biasing':
+                S = self._HOMO_LUMO_biasing(
+                    n_qubits=n_qubits, HF_array=HF_array, 
+                    weighting_operator=aux_operator, use_X_only=use_X_only
+                )
+            else:
+                raise ValueError('Unrecognised stabilizer search strategy.')
 
-    def _greedy_stabilizer_search(self,
-            n_qubits: int, 
-            depth: int=2
-        ) -> IndependentOp:
-        """
-        """
-        raise NotImplementedError
+            self.n_qubits_in_subspace = self.operator.n_qubits - S.n_terms
+            self.stabilizers = S
+            self._prepare_stabilizers()
 
+    def _noncontextual_update(self):
+        """ To be executed each time the noncontextual operator is updated.
+        """
+        if self.noncontextual_operator is not None:
+            self.noncontextual_operator.up_method = self.unitary_partitioning_method
+            self.contextual_operator = self.operator - self.noncontextual_operator
+            if self.contextual_operator.n_terms == 0:
+                raise ValueError('The Hamiltonian is noncontextual, the contextual subspace is empty.')
+            self.noncontextual_operator.solve(
+                strategy=self.noncontextual_solver, 
+                ref_state=self.ref_state, 
+                num_anneals=self.num_anneals,
+                expansion_order=self.noncontextual_expansion_order
+            )
+            self.n_cliques = self.noncontextual_operator.n_cliques
+        
     def _aux_operator_preserving_stabilizer_search(self,
             n_qubits: int,
             aux_operator: PauliwordOp,
             use_X_only: bool = True
         ) -> IndependentOp:
         """ Choose stabilizers that preserve some auxiliary operator.
         This could be an Ansatz operator such as UCCSD, for example.
@@ -223,50 +189,28 @@
                 S = IndependentOp.from_PauliwordOp(S)
                 found_stabilizers = True
             except:
                 pass
         
         return S
 
-    def _get_clique_representatives(self, 
-            symmetry_terms: IndependentOp = None, 
-            n_cliques: int = 2, 
-            clique_reps: List[PauliwordOp] = []
-        ) -> PauliwordOp:
-        """" For use with the StabilizeFirst noncontextual strategy. Given a set of terms we wish
-        to ensure are symmetries and potentially some initial clique representatives, grow the clique_reps
-        until we achieve the desired number n_cliques.
-        """
-        assert n_cliques > 1, 'Must specify more than one clique.'
-        if symmetry_terms is None:
-            symmetry_terms = self.stabilizers
-        non_identity = self.operator[np.any(self.operator.symp_matrix, axis=1)]
-        commutes_with_stabilizers_mask = np.all(symmetry_terms.commutes_termwise(non_identity), axis=0)
-        non_symmetry_mask = ~non_identity.generator_reconstruction(symmetry_terms)[1]
-        valid_terms = non_identity[non_symmetry_mask & commutes_with_stabilizers_mask]
-        if clique_reps != []:
-            clique_elements = sum(clique_reps, PauliwordOp.empty(self.operator.n_qubits))
-            anticom_with_existing_clique_reps_mask = (
-                ~np.any(clique_elements.commutes_termwise(valid_terms), axis=0)
-            )
-            valid_terms = valid_terms[anticom_with_existing_clique_reps_mask]
-        
-        if len(clique_reps)==n_cliques:
-            return sum(clique_reps)
-        elif valid_terms.n_terms == 0:
-            raise RuntimeError(f'Cannot identify {n_cliques} cliques, try lowering n_cliques.')
-        else:
-            clique_reps.append(valid_terms.sort()[0])
-            return self._get_clique_representatives(symmetry_terms, n_cliques, clique_reps)
-
     def _prepare_stabilizers(self) -> None:
         """ Prepare the chosen stabilizers for projection into the contextual subspace.
         This includes eigenvalue assignment (obtained from the solution of the noncontextual Hamiltonian),
         and application of unitary partitioning if enforcing a clique element.
         """
+        self.S3_initialized = False
+        #the StabilizeFirst strategy differs from the others in that the noncontextual
+        #Hamiltonian is constructed AFTER selecting stabilizers, which is what we do here:
+        if self.nc_strategy == 'StabilizeFirst':
+            self.noncontextual_operator = NoncontextualOp._from_stabilizers_noncontextual_op(
+                H=self.operator, stabilizers=self.stabilizers, use_jordan_product=False
+            )
+            self._noncontextual_update()
+
         if self.noncontextual_operator.n_cliques > 0:
             # mask stabilizers that lie within one of the noncontextual cliques
             clique_commutation = self.stabilizers.commutes_termwise(self.noncontextual_operator.clique_operator)
             mask_which_clique = np.all(clique_commutation, axis=0)
         else:
             mask_which_clique = []
 
@@ -274,84 +218,92 @@
             # we may only enforce stabilizers that live within the same clique, not accross them:
             assert(sum(mask_which_clique)==1), (
                 'Cannot enforce stabilizers from different cliques since '+
                 'unitary partitioning collapses onto just one of them.'
             )
             # generate the unitary partitioning rotations that map onto the 
             # clique representative correpsonding with the given stabilizers
-            (
-                self.mapped_clique_rep, 
-                self.unitary_partitioning_rotations,        
-                clique_normalizaion, # always normalized in contextual subspace...
-                normalized_clique # therefore will be the same as the clique_operator
-
-            ) = self.noncontextual_operator.clique_operator.unitary_partitioning(
-                up_method=self.unitary_partitioning_method, s_index=int(np.where(mask_which_clique)[0][0])
+            self.noncontextual_operator.update_clique_representative_operator(
+                clique_index=int(np.where(mask_which_clique)[0][0])
             )
-            # add the clique representative to the noncontextual basis in order to 
+            # add the clique representative to the noncontextual generators in order to 
             # update the eigenvalue assignments of the chosen stablizers so they are 
             # consistent with the noncontextual ground state configuration - this is 
             # G U {RARdag} in the original CS-VQE notation. 
-            augmented_basis = (
-                IndependentOp.from_PauliwordOp(self.mapped_clique_rep) + 
+            augmented_generators = (
+                IndependentOp(self.noncontextual_operator.mapped_clique_rep.symp_matrix, [-1]) + 
                 self.noncontextual_operator.symmetry_generators
             )
-            # given this new basis, we reconstruct the given stabilizers to identify
+            # given these new generators, we reconstruct the given stabilizers to identify
             # the correct subspace corresponding with the noncontextual ground state (nu, r)
-            update_eigenvalues(basis=augmented_basis, stabilizers=self.stabilizers)
+            update_eigenvalues(generators=augmented_generators, stabilizers=self.stabilizers)
             self.perform_unitary_partitioning = True
         else:
             update_eigenvalues(
-                basis=self.noncontextual_operator.symmetry_generators, 
+                generators=self.noncontextual_operator.symmetry_generators, 
                 stabilizers=self.stabilizers
             )
             self.perform_unitary_partitioning = False
 
     def project_onto_subspace(self, operator_to_project:PauliwordOp=None) -> PauliwordOp:
         """ Projects with respect to the current stabilizers; these are 
         updated using the ContextualSubspace.update_stabilizers method.
         """
         # if not supplied with an alternative operator for projection, use the internal operator 
         if operator_to_project is None:
-            operator_to_project = self.operator.copy()    
-        # first prepare the stabilizers, which is particularly relevant when 
-        # one wishes to enforce stabilizer(s) lying within a noncontextual clique
-        self._prepare_stabilizers()
+            operator_to_project = self.operator.copy() 
+        # if there are no stabilizers, return the input operator
+        if self.stabilizers is None:
+            return operator_to_project   
         # instantiate the parent S3_projection class that handles the subspace projection
         super().__init__(self.stabilizers)
+        self.S3_initialized = True
         # perform unitary partitioning
         if self.perform_unitary_partitioning:
             # the rotation is implemented differently depending on the choice of LCU or seq_rot
-            if self.unitary_partitioning_method=='LCU':
+            if self.noncontextual_operator.up_method=='LCU':
                 # linear-combination-of-unitaries approach
-                rotated_op = (self.unitary_partitioning_rotations * operator_to_project
-                        * self.unitary_partitioning_rotations.dagger).cleanup()
-            elif self.unitary_partitioning_method=='seq_rot':
+                rotated_op = (self.noncontextual_operator.unitary_partitioning_rotations * operator_to_project
+                        * self.noncontextual_operator.unitary_partitioning_rotations.dagger).cleanup()
+            elif self.noncontextual_operator.up_method=='seq_rot':
                 # sequence-of-rotations approach
-                rotated_op = operator_to_project.perform_rotations(self.unitary_partitioning_rotations)
+                rotated_op = operator_to_project.perform_rotations(self.noncontextual_operator.unitary_partitioning_rotations)
             else:
                 raise ValueError('Unrecognised unitary partitioning rotation method, must be one of LCU or seq_rot.')
         else:
             rotated_op = operator_to_project
         # finally, project the operator before returning
         cs_operator = self.perform_projection(rotated_op)
 
-        return cs_operator
+        if self.return_NC:
+            assert cs_operator.n_qubits == 1, 'Projected operator consists of more than one qubit.'
+            cs_operator = NoncontextualOp.from_PauliwordOp(cs_operator)
+            cs_operator.solve()
+            return cs_operator.energy
+        else:
+            return cs_operator
 
-    def hamiltonian(self, 
-            n_qubits: int, 
-            strategy: str = 'aux_preserving',
-            aux_operator: PauliwordOp = None,
-            depth: int = 2,
-            HF_array: np.array = None
-        ) -> PauliwordOp:
-        """ Wraps all the above methods for ease of use
-        """
-        self.update_stabilizers(
-            n_qubits=n_qubits, 
-            strategy=strategy, 
-            aux_operator=aux_operator, 
-            depth=depth,
-            HF_array = HF_array
-        )
-        cs_operator = self.project_onto_subspace()
-        return cs_operator
+    def project_state_onto_subspace(self, 
+            state_to_project: QuantumState = None
+        ) -> QuantumState:
+        """ Project a QuantumState into the contextual subspace
+        """
+        # if there are no stabilizers, return the input QuantumState
+        if self.stabilizers is None:
+            return state_to_project
+        
+        assert self.S3_initialized, 'Must first project an operator into the contextual subspace via the project_onto_subspace method'
+        # can provide an auxiliary state to project, although not in general scalable
+        if state_to_project is None:
+            assert self.ref_state is not None, 'Must provide a state to project into the contextual subspace'
+            state_to_project = self.ref_state
+
+        if self.perform_unitary_partitioning:
+            # behaviour is different whether using the LCU or seq_rot UP methods
+            if self.noncontextual_operator.up_method == 'LCU':
+                rotation = self.noncontextual_operator.unitary_partitioning_rotations
+            elif self.noncontextual_operator.up_method == 'seq_rot':
+                rotation_generator = sum([R*angle*.5*1j for R,angle in self.noncontextual_operator.unitary_partitioning_rotations])
+                rotation = trotter(rotation_generator)
+            return self.project_state(rotation * state_to_project)
+        else:
+            return self.project_state(state_to_project)
```

### Comparing `symmer-0.0.2/symmer/projection/qubit_tapering.py` & `symmer-0.0.3/symmer/projection/qubit_tapering.py`

 * *Files identical despite different names*

### Comparing `symmer-0.0.2/symmer/projection/utils.py` & `symmer-0.0.3/symmer/projection/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 def lp_norm(vector: np.array, p:int=2) -> float:
     """
     Returns:
         lp-norm of vector
     """
     return np.power(np.sum(np.power(np.abs(vector), p)), 1/p)
 
+def one_qubit_noncontextual_gs(op: PauliwordOp):
+    assert op.n_qubits == 1, 'Operator consists of more than one qubit'
+    op.to
+
 def basis_score(
         weighting_operator: PauliwordOp,
         basis: IndependentOp,
         p:int=1
     ) -> float:
     """ Evaluate the score of an input basis according 
     to the basis weighting operator, for example:
@@ -35,27 +39,27 @@
     mask_preserved = np.where(np.all(weighting_operator.commutes_termwise(basis),axis=1))[0]
     return (
         lp_norm(weighting_operator.coeff_vec[mask_preserved], p=p) /
         lp_norm(weighting_operator.coeff_vec, p=p)
     )
 
 def update_eigenvalues(
-        basis: IndependentOp, 
+        generators: IndependentOp, 
         stabilizers: IndependentOp
     ) -> None:
     """ Update the +/-1 eigenvalue assigned to the input stabilizer
     according to the noncontextual ground state configuration
     """
-    reconstruction, successfully_reconstructed = stabilizers.generator_reconstruction(basis)
+    reconstruction, successfully_reconstructed = stabilizers.generator_reconstruction(generators)
     if ~np.all(successfully_reconstructed):
-        raise ValueError('Basis not sufficient to reconstruct symmetry operators')
+        raise ValueError('Generators not sufficient to reconstruct symmetry operators')
     stabilizers.coeff_vec = (-1) ** np.count_nonzero(
         np.bitwise_and(
             reconstruction, 
-            np.asarray(basis.coeff_vec)==-1
+            np.asarray(generators.coeff_vec)==-1
         ),
         axis=1
     )
 
 class StabilizerIdentification:
     def __init__(self,
         weighting_operator: PauliwordOp,
```

### Comparing `symmer-0.0.2/symmer/utils.py` & `symmer-0.0.3/symmer/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from symmer.operators import PauliwordOp, QuantumState
 import numpy as np
 import scipy as sp
 from typing import List, Tuple, Union
 from functools import reduce
 import py3Dmol
+from scipy.sparse import csr_matrix
+from scipy.sparse import kron as sparse_kron
+import multiprocessing as mp
 
 def exact_gs_energy(
         sparse_matrix, 
         initial_guess=None, 
         n_particles=None, 
         number_operator=None, 
         n_eigs=6
     ) -> Tuple[float, np.array]:
     """ Return the ground state energy and corresponding ground statevector for the input operator
     
     Specifying a particle number will restrict to eigenvectors |ψ> such that <ψ|N_op|ψ> = n_particles
     where N_op is the given number operator.
     """
+    if number_operator is None:
+        # if no number operator then need not compute any further eigenvalues
+        n_eigs = 1
+
     # Note the eigenvectors are stored column-wise so need to transpose
     if sparse_matrix.shape[0] > 2**5:
         eigvals, eigvecs = sp.sparse.linalg.eigsh(
             sparse_matrix,k=n_eigs,v0=initial_guess,which='SA',maxiter=1e7
         )
     else:
         # for small matrices the dense representation can be more efficient than sparse!
@@ -188,8 +195,87 @@
         view.setStyle({'sphere': {"radius": 0.2}})
     elif style == "stick":
         view.setStyle({'stick': {}})
     else:
         raise ValueError(f"unknown py3dmol style: {style}")
 
     view.zoomTo()
-    return view
+    return view
+
+
+def get_sparse_matrix_large_pauliwordop(P_op: PauliwordOp) -> csr_matrix:
+    """
+    In order to build the sparse matrix (e.g. above 18 qubits), this function goes through each pauli term
+    divides into two equally sized tensor products finds the sparse matrix of those and then does a sparse
+    kron product to get the large matrix.
+
+    TODO:  Could also add how many junks to split problem into (e.g. three/four/... tensor products).
+
+    Args:
+        P_op (PauliwordOp): Pauli operator to convert into sparse matrix
+    Returns:
+        mat (csr_matrix): sparse matrix of P_op
+    """
+    nq = P_op.n_qubits
+    if nq<16:
+        mat = P_op.to_sparse_matrix
+    else:
+        n_cpus = mp.cpu_count()
+        P_op_chunks_inds = np.rint(np.linspace(0, P_op.n_terms, min(n_cpus, P_op.n_terms))).astype(set).astype(int)
+
+        # miss zero index out (as emtpy list)
+        P_op_chunks = [P_op[P_op_chunks_inds[ind_i]: P_op_chunks_inds[ind_i+1]] for ind_i, _ in enumerate(P_op_chunks_inds[1:])]
+        with mp.Pool(n_cpus) as pool:
+            tracker = pool.map(_get_sparse_matrix_large_pauliwordop, P_op_chunks)
+
+        mat = reduce(lambda x, y: x + y, tracker)
+
+    return mat
+
+
+def _get_sparse_matrix_large_pauliwordop(P_op: PauliwordOp) -> csr_matrix:
+    """
+    """
+    nq = P_op.n_qubits
+    mat = PauliwordOp.empty(nq).to_sparse_matrix
+    for op in P_op:
+        left_tensor = np.hstack((op.X_block[:, :nq // 2],
+                                 op.Z_block[:, :nq // 2]))
+        left_coeff = op.coeff_vec
+
+        right_tensor = np.hstack((op.X_block[:, nq // 2:],
+                                  op.Z_block[:, nq // 2:]))
+        right_coeff = np.array([1])
+
+        temp = sparse_kron(PauliwordOp(left_tensor, left_coeff).to_sparse_matrix,
+                           PauliwordOp(right_tensor, right_coeff).to_sparse_matrix,
+                           format='csr')  # setting format makes this faster!
+
+        mat += temp
+        del temp
+
+    return mat
+
+
+def matrix_allclose(A: Union[csr_matrix, np.array], B:Union[csr_matrix, np.array], tol:int = 1e-15) -> bool:
+    """
+    check matrix A and B have the same entries up to a given tolerance
+    Args:
+        A : matrix A
+        B:  matrix B
+        tol: allowed difference
+
+    Returns:
+        bool
+
+    """
+    if isinstance(A, csr_matrix) and isinstance(B, csr_matrix):
+        max_diff = np.abs(A-B).max()
+        return max_diff <= tol
+    else:
+        if isinstance(A, csr_matrix):
+            A = A.toarray()
+
+        if isinstance(B, csr_matrix):
+            B = B.toarray()
+
+        return np.allclose(A, B, atol=tol)
```

### Comparing `symmer-0.0.2/PKG-INFO` & `symmer-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symmer
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: MIT
 Author: AlexisRalli
 Author-email: rallilex@hotmail.co.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,8 +21,8 @@
 Requires-Dist: openfermion (>=1.3.0,<2.0.0)
 Requires-Dist: opt-einsum (>=3.3.0,<4.0.0)
 Requires-Dist: py3Dmol (>=1.8.0,<2.0.0)
 Requires-Dist: pydocstyle (>=6.1.1,<7.0.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: qiskit (>=0.38.0,<0.39.0)
 Requires-Dist: qubovert (>=1.2.5,<2.0.0)
-Requires-Dist: quimb (>=1.4.2,<2.0.0)
+Requires-Dist: quimb (>=1.4,<1.5)
```

