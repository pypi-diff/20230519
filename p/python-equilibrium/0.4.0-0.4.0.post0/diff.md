# Comparing `tmp/python_equilibrium-0.4.0.tar.gz` & `tmp/python_equilibrium-0.4.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.4.0.tar", max compression
+gzip compressed data, was "python_equilibrium-0.4.0.post0.tar", max compression
```

## Comparing `python_equilibrium-0.4.0.tar` & `python_equilibrium-0.4.0.post0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.4.0/LICENSE
--rw-r--r--   0        0        0     2026 2023-05-19 08:36:02.306401 python_equilibrium-0.4.0/README.md
--rw-r--r--   0        0        0     1609 2023-05-19 09:08:22.027151 python_equilibrium-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      714 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/AdmissionController.py
--rw-r--r--   0        0        0     8461 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/CrudResourceController.py
--rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/JsonResourceStore.py
--rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/JsonResourceStore_test.py
--rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/Namespace.py
--rw-r--r--   0        0        0    13234 2023-05-16 21:15:49.967795 python_equilibrium-0.4.0/src/equilibrium/Resource.py
--rw-r--r--   0        0        0    15427 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/ResourceContext.py
--rw-r--r--   0        0        0      482 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/ResourceController.py
--rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/ResourceStore.py
--rw-r--r--   0        0        0     2189 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/Resource_test.py
--rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0/src/equilibrium/Service.py
--rw-r--r--   0        0        0     1045 2023-05-19 09:08:22.027151 python_equilibrium-0.4.0/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.4.0/src/equilibrium/py.typed
--rw-r--r--   0        0        0     2749 1970-01-01 00:00:00.000000 python_equilibrium-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.4.0.post0/LICENSE
+-rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.4.0.post0/README.md
+-rw-r--r--   0        0        0     1615 2023-05-19 09:28:12.252441 python_equilibrium-0.4.0.post0/pyproject.toml
+-rw-r--r--   0        0        0      714 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/AdmissionController.py
+-rw-r--r--   0        0        0     8461 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/CrudResourceController.py
+-rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/JsonResourceStore.py
+-rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/Namespace.py
+-rw-r--r--   0        0        0    13234 2023-05-16 21:15:49.967795 python_equilibrium-0.4.0.post0/src/equilibrium/Resource.py
+-rw-r--r--   0        0        0    15427 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/ResourceContext.py
+-rw-r--r--   0        0        0      482 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/ResourceController.py
+-rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/ResourceStore.py
+-rw-r--r--   0        0        0     2189 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/Resource_test.py
+-rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/Service.py
+-rw-r--r--   0        0        0     1051 2023-05-19 09:28:12.252441 python_equilibrium-0.4.0.post0/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.4.0.post0/src/equilibrium/py.typed
+-rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 python_equilibrium-0.4.0.post0/PKG-INFO
```

### Comparing `python_equilibrium-0.4.0/LICENSE` & `python_equilibrium-0.4.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/README.md` & `python_equilibrium-0.4.0.post0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # equilibrium
 
 > __Equilibrium__ _(noun)_: A state in which opposing forces or influences are balanced, resulting in a stable system
 > that does not undergo significant changes. In a broader sense, equilibrium can refer to a state of mental or emotional
 > balance, as well as the balance of forces in physical or chemical systems.
 
-Equilibrium is a Python framework inspired by various other open-source tools for implementing control loops
-(Kubernetes) and rules-engines (Pants build system).
+Equilibrium is a framework for implementing control loops and is heavily Kubernets-inspired. A control loop is a
+system that continuously monitors the state of a system and takes action to bring the system into a desired state.
+It is designed to be extensible and flexible, allowing you to implement control loops that are tailored to your
+specific use case.
 
-## Overview: Resource management & control loops
+__Installation__
 
-Equilibrium is a framework for implementing control loops. A control loop is a system that continuously monitors
-the state of a system and takes action to bring the system into a desired state. Equilibrium is designed to be
-extensible and flexible, allowing you to implement control loops that are tailored to your specific use case.
+Equilibrium is available on PyPI. You need at least Python 3.10.
+
+```bash
+pip install python-equilibrium
+```
+
+__Example__
 
 Check out the [examples/local_file/](examples/local_file/) directory for a simple example of a control loop that
 monitors a local file and takes action when the file is modified.
 
+```mermaid
+graph LR
+  subgraph Equilibrium
+    LocalFile["Resource[LocalFile]"] --> LocalFileController
+  end
+  subgraph "Local filesystem"
+    LocalFileController --> LocalFileModification["Local filesystem changes"]
+  end
+  subgraph "State Backend"
+    LocalFileController --> State["Last known state"]
+  end
+```
+
 __Difference to Kubernetes resources__
 
 * Equilibrium does not currently support any key other than `spec` next to `apiVersion`, `kind`, and `metadata` in
   a resource definition. This means Equilibrium cannot be used to deserialize actual Kubernetes `Secret` of `Config`
   resources.
-
-## Overview: Rules engine
-
-Equilibrium is also a framework for implementing rules engines. A rules engine is a system derives a sequence of rules
-to execute to reach a desired and goal based on a given set of inputs, ensuring that rules are never exexcuted multiple
-times with the same inputs.
-
-Check out the [examples/codegen/](examples/codegen/) directory for a simple example of a rules engine that generates
-Terraform code based on a set of Kubernetes-like resources. This example combines the resource management API with
-the rules engine API.
-
-## Installation
-
-Equilibrium is available on PyPI:
-
-```bash
-pip install python-equilibrium
-```
-
-It requires at least Python 3.10.
```

### Comparing `python_equilibrium-0.4.0/pyproject.toml` & `python_equilibrium-0.4.0.post0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.4.0"
+version = "0.4.0.post0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_equilibrium-0.4.0/src/equilibrium/AdmissionController.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/AdmissionController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/CrudResourceController.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/CrudResourceController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/JsonResourceStore.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/JsonResourceStore_test.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/Namespace.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/Resource.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/Resource.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/ResourceContext.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/ResourceContext.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/ResourceStore.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/Resource_test.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/Resource_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/Service.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/Service.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0/src/equilibrium/__init__.py` & `python_equilibrium-0.4.0.post0/src/equilibrium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     "ResourceRegistry",
     "ResourceStore",
     "ResourceTypeRegistry",
     "Service",
     "ServiceRegistry",
 ]
 
-__version__ = "0.4.0"
+__version__ = "0.4.0.post0"
```

### Comparing `python_equilibrium-0.4.0/PKG-INFO` & `python_equilibrium-0.4.0.post0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.4.0
+Version: 0.4.0.post0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,45 +19,44 @@
 
 # equilibrium
 
 > __Equilibrium__ _(noun)_: A state in which opposing forces or influences are balanced, resulting in a stable system
 > that does not undergo significant changes. In a broader sense, equilibrium can refer to a state of mental or emotional
 > balance, as well as the balance of forces in physical or chemical systems.
 
-Equilibrium is a Python framework inspired by various other open-source tools for implementing control loops
-(Kubernetes) and rules-engines (Pants build system).
+Equilibrium is a framework for implementing control loops and is heavily Kubernets-inspired. A control loop is a
+system that continuously monitors the state of a system and takes action to bring the system into a desired state.
+It is designed to be extensible and flexible, allowing you to implement control loops that are tailored to your
+specific use case.
 
-## Overview: Resource management & control loops
+__Installation__
 
-Equilibrium is a framework for implementing control loops. A control loop is a system that continuously monitors
-the state of a system and takes action to bring the system into a desired state. Equilibrium is designed to be
-extensible and flexible, allowing you to implement control loops that are tailored to your specific use case.
+Equilibrium is available on PyPI. You need at least Python 3.10.
+
+```bash
+pip install python-equilibrium
+```
+
+__Example__
 
 Check out the [examples/local_file/](examples/local_file/) directory for a simple example of a control loop that
 monitors a local file and takes action when the file is modified.
 
+```mermaid
+graph LR
+  subgraph Equilibrium
+    LocalFile["Resource[LocalFile]"] --> LocalFileController
+  end
+  subgraph "Local filesystem"
+    LocalFileController --> LocalFileModification["Local filesystem changes"]
+  end
+  subgraph "State Backend"
+    LocalFileController --> State["Last known state"]
+  end
+```
+
 __Difference to Kubernetes resources__
 
 * Equilibrium does not currently support any key other than `spec` next to `apiVersion`, `kind`, and `metadata` in
   a resource definition. This means Equilibrium cannot be used to deserialize actual Kubernetes `Secret` of `Config`
   resources.
 
-## Overview: Rules engine
-
-Equilibrium is also a framework for implementing rules engines. A rules engine is a system derives a sequence of rules
-to execute to reach a desired and goal based on a given set of inputs, ensuring that rules are never exexcuted multiple
-times with the same inputs.
-
-Check out the [examples/codegen/](examples/codegen/) directory for a simple example of a rules engine that generates
-Terraform code based on a set of Kubernetes-like resources. This example combines the resource management API with
-the rules engine API.
-
-## Installation
-
-Equilibrium is available on PyPI:
-
-```bash
-pip install python-equilibrium
-```
-
-It requires at least Python 3.10.
-
```

