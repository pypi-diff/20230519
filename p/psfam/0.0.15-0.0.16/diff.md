# Comparing `tmp/psfam-0.0.15.tar.gz` & `tmp/psfam-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psfam-0.0.15.tar", last modified: Wed May 17 22:44:55 2023, max compression
+gzip compressed data, was "psfam-0.0.16.tar", last modified: Fri May 19 19:07:42 2023, max compression
```

## Comparing `psfam-0.0.15.tar` & `psfam-0.0.16.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 22:44:55.005569 psfam-0.0.15/
--rw-rw-rw-   0        0        0     6349 2023-05-17 22:44:55.004560 psfam-0.0.15/PKG-INFO
--rw-rw-rw-   0        0        0     5758 2023-05-15 20:34:34.000000 psfam-0.0.15/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 22:44:54.969540 psfam-0.0.15/psfam/
--rw-rw-rw-   0        0        0        0 2023-04-24 20:25:09.000000 psfam-0.0.15/psfam/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-29 21:06:06.000000 psfam-0.0.15/psfam/family.py
--rw-rw-rw-   0        0        0     5818 2023-04-25 15:45:54.000000 psfam-0.0.15/psfam/matrix_generator.py
--rw-rw-rw-   0        0        0     9947 2023-04-28 19:02:32.000000 psfam-0.0.15/psfam/pauli_organizer.py
--rw-rw-rw-   0        0        0     7605 2023-04-25 15:41:08.000000 psfam-0.0.15/psfam/pauli_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 22:44:55.002594 psfam-0.0.15/psfam.egg-info/
--rw-rw-rw-   0        0        0     6349 2023-05-17 22:44:54.000000 psfam-0.0.15/psfam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-17 22:44:54.000000 psfam-0.0.15/psfam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 22:44:54.000000 psfam-0.0.15/psfam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-17 22:44:54.000000 psfam-0.0.15/psfam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-17 22:44:54.000000 psfam-0.0.15/psfam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 22:44:55.005569 psfam-0.0.15/setup.cfg
--rw-rw-rw-   0        0        0      968 2023-05-17 22:43:47.000000 psfam-0.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:07:42.562424 psfam-0.0.16/
+-rw-rw-rw-   0        0        0     6456 2023-05-19 19:07:42.560424 psfam-0.0.16/PKG-INFO
+-rw-rw-rw-   0        0        0     5857 2023-05-19 18:59:08.000000 psfam-0.0.16/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 19:07:42.505360 psfam-0.0.16/psfam/
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:25:09.000000 psfam-0.0.16/psfam/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-29 21:06:06.000000 psfam-0.0.16/psfam/family.py
+-rw-rw-rw-   0        0        0     5818 2023-04-25 15:45:54.000000 psfam-0.0.16/psfam/matrix_generator.py
+-rw-rw-rw-   0        0        0     9947 2023-04-28 19:02:32.000000 psfam-0.0.16/psfam/pauli_organizer.py
+-rw-rw-rw-   0        0        0     7605 2023-04-25 15:41:08.000000 psfam-0.0.16/psfam/pauli_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:07:42.554878 psfam-0.0.16/psfam.egg-info/
+-rw-rw-rw-   0        0        0     6456 2023-05-19 19:07:42.000000 psfam-0.0.16/psfam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-19 19:07:42.000000 psfam-0.0.16/psfam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:07:42.000000 psfam-0.0.16/psfam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-19 19:07:42.000000 psfam-0.0.16/psfam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-19 19:07:42.000000 psfam-0.0.16/psfam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:07:42.564431 psfam-0.0.16/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-05-19 19:07:28.000000 psfam-0.0.16/setup.py
```

### Comparing `psfam-0.0.15/PKG-INFO` & `psfam-0.0.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: psfam
-Version: 0.0.15
+Version: 0.0.16
 Summary: Pauli string organizer for dense operators.
 Home-page: UNKNOWN
 Author: Ben Reggio
 Author-email: benjreggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
-# Psfam Documentation
 
-The Psfam package is a python package which organizes the complete set of pauli strings of any size into commuting families for VQE, finding a unitary matrix from clifford operators which diagonalizes all of the strings, and implementing this unitary matrix on a qiskit circuit.
+
+The psfam package is a python package which organizes the complete set of pauli strings of any size into commuting families for VQE, finding a unitary matrix from clifford operators which diagonalizes all of the strings, and implementing this unitary matrix on a qiskit circuit.
+
+psfam can be installed with 
+
+```
+pip install psfam
+```
+
+## Usage
 
 Below are instructions on how to use the Psfam package. It will show the process of using a PauliOrganizer object to partition strings, then calculating an expectation value on a qiskit simulator.
 
 You'll need numpy and qiskit, so lets import those:
 
 ```python
 from psfam.pauli_organizer import *
@@ -151,15 +159,15 @@
 qc.draw('mpl')
 ```
 
 
 
 
     
-![](https://raw.githubusercontent.com/Benjreggio/psfamtest/blob/main/output_15_0.png)
+![Cirucit diagram](https://github.com/Benjreggio/psfam/raw/main/output_15_0.png)
     
 
 
 
 This code is straight from here: https://qiskit.org/documentation/tutorials/circuits/1_getting_started_with_qiskit.html. qiskit has methods to visualize the results.
 
 
@@ -175,15 +183,15 @@
     {'11': 933, '00': 44, '01': 24, '10': 23}
     
 
 
 
 
     
-![png](output_17_1.png)
+![Counts histogram](https://github.com/Benjreggio/psfam/raw/main/output_17_1.png)
     
 
 
 
 Now that we have this result, we can use the counts of each result to get the probability of getting that result:
 
 $$
```

### Comparing `psfam-0.0.15/README.md` & `psfam-0.0.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
-# Psfam Documentation
 
-The Psfam package is a python package which organizes the complete set of pauli strings of any size into commuting families for VQE, finding a unitary matrix from clifford operators which diagonalizes all of the strings, and implementing this unitary matrix on a qiskit circuit.
+
+The psfam package is a python package which organizes the complete set of pauli strings of any size into commuting families for VQE, finding a unitary matrix from clifford operators which diagonalizes all of the strings, and implementing this unitary matrix on a qiskit circuit.
+
+psfam can be installed with 
+
+```
+pip install psfam
+```
+
+## Usage
 
 Below are instructions on how to use the Psfam package. It will show the process of using a PauliOrganizer object to partition strings, then calculating an expectation value on a qiskit simulator.
 
 You'll need numpy and qiskit, so lets import those:
 
 ```python
 from psfam.pauli_organizer import *
@@ -137,15 +145,15 @@
 qc.draw('mpl')
 ```
 
 
 
 
     
-![](https://raw.githubusercontent.com/Benjreggio/psfamtest/blob/main/output_15_0.png)
+![Cirucit diagram](https://github.com/Benjreggio/psfam/raw/main/output_15_0.png)
     
 
 
 
 This code is straight from here: https://qiskit.org/documentation/tutorials/circuits/1_getting_started_with_qiskit.html. qiskit has methods to visualize the results.
 
 
@@ -161,15 +169,15 @@
     {'11': 933, '00': 44, '01': 24, '10': 23}
     
 
 
 
 
     
-![png](output_17_1.png)
+![Counts histogram](https://github.com/Benjreggio/psfam/raw/main/output_17_1.png)
     
 
 
 
 Now that we have this result, we can use the counts of each result to get the probability of getting that result:
 
 $$
```

### Comparing `psfam-0.0.15/psfam/family.py` & `psfam-0.0.16/psfam/family.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.15/psfam/matrix_generator.py` & `psfam-0.0.16/psfam/matrix_generator.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.15/psfam/pauli_organizer.py` & `psfam-0.0.16/psfam/pauli_organizer.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.15/psfam/pauli_utils.py` & `psfam-0.0.16/psfam/pauli_utils.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.15/psfam.egg-info/PKG-INFO` & `psfam-0.0.16/psfam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: psfam
-Version: 0.0.15
+Version: 0.0.16
 Summary: Pauli string organizer for dense operators.
 Home-page: UNKNOWN
 Author: Ben Reggio
 Author-email: benjreggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
-# Psfam Documentation
 
-The Psfam package is a python package which organizes the complete set of pauli strings of any size into commuting families for VQE, finding a unitary matrix from clifford operators which diagonalizes all of the strings, and implementing this unitary matrix on a qiskit circuit.
+
+The psfam package is a python package which organizes the complete set of pauli strings of any size into commuting families for VQE, finding a unitary matrix from clifford operators which diagonalizes all of the strings, and implementing this unitary matrix on a qiskit circuit.
+
+psfam can be installed with 
+
+```
+pip install psfam
+```
+
+## Usage
 
 Below are instructions on how to use the Psfam package. It will show the process of using a PauliOrganizer object to partition strings, then calculating an expectation value on a qiskit simulator.
 
 You'll need numpy and qiskit, so lets import those:
 
 ```python
 from psfam.pauli_organizer import *
@@ -151,15 +159,15 @@
 qc.draw('mpl')
 ```
 
 
 
 
     
-![](https://raw.githubusercontent.com/Benjreggio/psfamtest/blob/main/output_15_0.png)
+![Cirucit diagram](https://github.com/Benjreggio/psfam/raw/main/output_15_0.png)
     
 
 
 
 This code is straight from here: https://qiskit.org/documentation/tutorials/circuits/1_getting_started_with_qiskit.html. qiskit has methods to visualize the results.
 
 
@@ -175,15 +183,15 @@
     {'11': 933, '00': 44, '01': 24, '10': 23}
     
 
 
 
 
     
-![png](output_17_1.png)
+![Counts histogram](https://github.com/Benjreggio/psfam/raw/main/output_17_1.png)
     
 
 
 
 Now that we have this result, we can use the counts of each result to get the probability of getting that result:
 
 $$
```

### Comparing `psfam-0.0.15/setup.py` & `psfam-0.0.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "psfam",
-    version = "0.0.15",
+    version = "0.0.16",
     author = "Ben Reggio",
     author_email = "benjreggio@gmail.com",
     description = ("Pauli string organizer for dense operators."),
     license = "MIT",
     packages=['psfam'],
     long_description=read('README.md'),
     long_description_content_type = "text/markdown",
```

