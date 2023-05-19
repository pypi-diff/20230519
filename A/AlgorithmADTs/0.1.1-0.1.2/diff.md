# Comparing `tmp/algorithmadts-0.1.1.tar.gz` & `tmp/algorithmadts-0.1.2.tar.gz`

## Comparing `algorithmadts-0.1.1.tar` & `algorithmadts-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.DS_Store
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/AlgorithmADTs/.DS_Store
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/AlgorithmADTs/AbstractDataTypes.py
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/AlgorithmADTs/GraphAlgorithms.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/src/AlgorithmADTs/__init__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/tests/experimenting.ipynb
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/tests/test_GraphAlgorithms.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/LICENSE
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/README.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 algorithmadts-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.DS_Store
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/AlgorithmADTs/.DS_Store
+-rw-r--r--   0        0        0    12317 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/AlgorithmADTs/AbstractDataTypes.py
+-rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/AlgorithmADTs/GraphAlgorithms.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/AlgorithmADTs/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/tests/experimenting.ipynb
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/tests/test_GraphAlgorithms.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/README.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/PKG-INFO
```

### Comparing `algorithmadts-0.1.1/.DS_Store` & `algorithmadts-0.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.1/src/.DS_Store` & `algorithmadts-0.1.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.1/src/AlgorithmADTs/.DS_Store` & `algorithmadts-0.1.2/src/AlgorithmADTs/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.1/src/AlgorithmADTs/AbstractDataTypes.py` & `algorithmadts-0.1.2/src/AlgorithmADTs/AbstractDataTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,25 +392,35 @@
     @property
     def edges(self):
         return self._edges
 
     def add_node(self, node: Any):
         self._nodes.append(node)
         return self
-
+    
     def add_edge(self, node1: Any, node2: Any):
         if not (node1 in self._nodes and node2 in self._nodes):
             raise ValueError("Nodes must already be in the graph")
 
         self._edges.append((node1, node2))
         if not self._directed:
             self._edges.append((node2, node1))
 
         return self
 
+    def add_nodes(self, nodes: Any):
+        for node in nodes:
+            self.add_node(node)
+        return self
+
+    def add_edges(self, edges: Any):
+        for edge in edges:
+            self.add_edge(*edge)
+        return self
+    
     def adjacent(self, node1: Any, node2: Any):
         return (node1, node2) in self._edges
 
     def neighbours(self, node: Any):
         node_neighbours = List.create()
 
         for edge in self._edges:
```

### Comparing `algorithmadts-0.1.1/src/AlgorithmADTs/GraphAlgorithms.py` & `algorithmadts-0.1.2/src/AlgorithmADTs/GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.1/tests/experimenting.ipynb` & `algorithmadts-0.1.2/tests/experimenting.ipynb`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.1/tests/test_GraphAlgorithms.py` & `algorithmadts-0.1.2/tests/test_GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.1/LICENSE` & `algorithmadts-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.1/README.md` & `algorithmadts-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -73,34 +73,35 @@
     create: None -> Graph
     add_node: Graph x Element -> Graph
     add_edge: Graph x Element x Element -> Graph
     adjacent: Graph x Element x Element -> Boolean
     neighbours: Graph x Element -> List
     get_weight: Graph x Element x Element -> integer
 ```
+Multiple nodes and edges can now be added at one time with `add_nodes` and `add_edges`, using an iterable
 
 Note that there is no restriction in these classes that elements be hashable, unlike some Python data types
 e.g. a Python `dict` requires keys to be hashable.
 
 It also defines a variable `infinity`, set equal to `float('inf')`
 
 The following magic methods are supported:
 - `__getitem__` and `__setitem__` for classes with a 'get' and 'set' function.
     This allows you to call `instance[key]` and `instance[key] = value`.
 - `__iter__` for Array and List, which operates as expected. Dictionary iter returns an iterable of keys.
     This enables iterating through a class like `for elem in instance`
 - `__str__` and `__repr__` are defined for all classes except graphs and allow for classes to be easily viewed through printing
     Note that only the head element is visible for a stack or queue, so it is the only information that can be returned by these methods
+- Numerical magic methods (e.g. `__add__`) are defined for matrices
 
 ## Graph Algorithms
 Currently, only the following graph algorithms are defined:
 - Prim's algorithm for computing the Minimal Spanning Tree of a weighted, undirected graph
 - Dijkstra's algorithm for finding the single source shortest path in a weighted graph 
 - The Bellman-Ford algorithm which extends the functionality of Dijkstra's algorithm to allow for negative weights
 - The two variants of the Floyd-Warshall algorithm to calculate shortest path between all nodes and transitive closure of an unweighted graph
 - The PageRank algorithm for determining the relative importance of nodes in an unweighted graph
 
-## Version things
-Still trying to figure out readme syntax
+## Version things 
 To implement:
 - Optional hashing for graphs?
 - Search methods like DPS BFS
```

### Comparing `algorithmadts-0.1.1/PKG-INFO` & `algorithmadts-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgorithmADTs
-Version: 0.1.1
+Version: 0.1.2
 Summary: General purpose Abstract Data Types for Algorithmics
 Author-email: Finlay <finlay3.141@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -85,34 +85,35 @@
     create: None -> Graph
     add_node: Graph x Element -> Graph
     add_edge: Graph x Element x Element -> Graph
     adjacent: Graph x Element x Element -> Boolean
     neighbours: Graph x Element -> List
     get_weight: Graph x Element x Element -> integer
 ```
+Multiple nodes and edges can now be added at one time with `add_nodes` and `add_edges`, using an iterable
 
 Note that there is no restriction in these classes that elements be hashable, unlike some Python data types
 e.g. a Python `dict` requires keys to be hashable.
 
 It also defines a variable `infinity`, set equal to `float('inf')`
 
 The following magic methods are supported:
 - `__getitem__` and `__setitem__` for classes with a 'get' and 'set' function.
     This allows you to call `instance[key]` and `instance[key] = value`.
 - `__iter__` for Array and List, which operates as expected. Dictionary iter returns an iterable of keys.
     This enables iterating through a class like `for elem in instance`
 - `__str__` and `__repr__` are defined for all classes except graphs and allow for classes to be easily viewed through printing
     Note that only the head element is visible for a stack or queue, so it is the only information that can be returned by these methods
+- Numerical magic methods (e.g. `__add__`) are defined for matrices
 
 ## Graph Algorithms
 Currently, only the following graph algorithms are defined:
 - Prim's algorithm for computing the Minimal Spanning Tree of a weighted, undirected graph
 - Dijkstra's algorithm for finding the single source shortest path in a weighted graph 
 - The Bellman-Ford algorithm which extends the functionality of Dijkstra's algorithm to allow for negative weights
 - The two variants of the Floyd-Warshall algorithm to calculate shortest path between all nodes and transitive closure of an unweighted graph
 - The PageRank algorithm for determining the relative importance of nodes in an unweighted graph
 
-## Version things
-Still trying to figure out readme syntax
+## Version things 
 To implement:
 - Optional hashing for graphs?
 - Search methods like DPS BFS
```

