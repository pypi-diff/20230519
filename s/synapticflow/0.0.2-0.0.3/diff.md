# Comparing `tmp/synapticflow-0.0.2.tar.gz` & `tmp/synapticflow-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapticflow-0.0.2.tar", max compression
+gzip compressed data, was "synapticflow-0.0.3.tar", max compression
```

## Comparing `synapticflow-0.0.2.tar` & `synapticflow-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,22 @@
--rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.2/LICENSE
--rw-r--r--   0        0        0     3224 2023-04-10 04:18:10.075412 synapticflow-0.0.2/README.md
--rw-r--r--   0        0        0     1202 2023-05-11 01:31:07.115029 synapticflow-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-11 01:13:36.467467 synapticflow-0.0.2/synapticflow/.DS_Store
--rw-r--r--   0        0        0      967 2023-05-11 01:31:13.044893 synapticflow-0.0.2/synapticflow/__init__.py
--rw-r--r--   0        0        0      969 2023-05-11 01:16:12.645161 synapticflow-0.0.2/synapticflow/network/__init__.py
--rw-r--r--   0        0        0      651 2023-04-09 16:31:19.669191 synapticflow-0.0.2/synapticflow/network/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    60989 2023-04-10 04:13:39.844147 synapticflow-0.0.2/synapticflow/network/__pycache__/neural_populations.cpython-39.pyc
--rw-r--r--   0        0        0     8041 2023-05-11 01:16:31.982145 synapticflow-0.0.2/synapticflow/network/connections.py
--rw-r--r--   0        0        0    87884 2023-04-10 03:54:27.580176 synapticflow-0.0.2/synapticflow/network/neural_populations.py
--rw-r--r--   0        0        0      776 2023-04-07 14:45:50.487754 synapticflow-0.0.2/synapticflow/plotting/__init__.py
--rw-r--r--   0        0        0      649 2023-04-09 16:34:08.316076 synapticflow-0.0.2/synapticflow/plotting/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    16708 2023-04-10 04:13:42.214184 synapticflow-0.0.2/synapticflow/plotting/__pycache__/visualization.cpython-39.pyc
--rw-r--r--   0        0        0    16715 2023-04-10 03:52:43.853966 synapticflow-0.0.2/synapticflow/plotting/visualization.py
--rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 synapticflow-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3224 2023-05-19 18:52:23.078528 synapticflow-0.0.3/README.md
+-rw-r--r--   0        0        0     1202 2023-05-19 20:06:03.249236 synapticflow-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-05-19 20:05:58.347482 synapticflow-0.0.3/synapticflow/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.512954 synapticflow-0.0.3/synapticflow/decision/__init__.py
+-rw-r--r--   0        0        0     1464 2023-05-18 16:57:01.513061 synapticflow-0.0.3/synapticflow/decision/decision.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.513202 synapticflow-0.0.3/synapticflow/encoding/__init__.py
+-rw-r--r--   0        0        0    10258 2023-05-18 21:55:51.403569 synapticflow-0.0.3/synapticflow/encoding/encoders.py
+-rw-r--r--   0        0        0       51 2023-05-18 16:57:01.513461 synapticflow-0.0.3/synapticflow/learning/__init__.py
+-rw-r--r--   0        0        0    22956 2023-05-18 21:48:21.478245 synapticflow-0.0.3/synapticflow/learning/learning_rules.py
+-rw-r--r--   0        0        0     1252 2023-05-18 16:57:01.513703 synapticflow-0.0.3/synapticflow/learning/rewards.py
+-rw-r--r--   0        0        0      102 2023-05-18 16:57:01.513880 synapticflow-0.0.3/synapticflow/network/__init__.py
+-rw-r--r--   0        0        0    11840 2023-05-18 21:51:10.445427 synapticflow-0.0.3/synapticflow/network/connections.py
+-rw-r--r--   0        0        0     4766 2023-05-18 16:57:01.514217 synapticflow-0.0.3/synapticflow/network/monitors.py
+-rw-r--r--   0        0        0     7874 2023-05-18 16:57:01.514367 synapticflow-0.0.3/synapticflow/network/network.py
+-rw-r--r--   0        0        0    87912 2023-05-19 19:41:44.825988 synapticflow-0.0.3/synapticflow/network/neural_populations.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.515139 synapticflow-0.0.3/synapticflow/plotting/__init__.py
+-rw-r--r--   0        0        0      463 2023-05-18 16:57:01.515777 synapticflow-0.0.3/synapticflow/plotting/plotting.py
+-rw-r--r--   0        0        0    16715 2023-05-19 18:46:34.831952 synapticflow-0.0.3/synapticflow/plotting/visualization.py
+-rw-r--r--   0        0        0       19 2023-05-19 18:53:07.864217 synapticflow-0.0.3/synapticflow/synapticflow.py
+-rw-r--r--   0        0        0      303 2023-05-18 16:57:01.515915 synapticflow-0.0.3/synapticflow/utils.py
+-rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 synapticflow-0.0.3/PKG-INFO
```

### Comparing `synapticflow-0.0.2/LICENSE` & `synapticflow-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.2/README.md` & `synapticflow-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.2/pyproject.toml` & `synapticflow-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "synapticflow"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     "Arsham Gholamzadeh Khoee <arsham.gh97@gmail.com>",
     "Mobin Nesari <mobinnesari81@gmail.com>",
     "Mohammad Mehdi Begmaz <mohammadmehdi.begmaz@gmail.com>",
     "Negar Sourati <negarsourati@gmail.com>"
 ]
 maintainers =[
```

### Comparing `synapticflow-0.0.2/synapticflow/network/neural_populations.py` & `synapticflow-0.0.3/synapticflow/network/neural_populations.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,14 +139,15 @@
             self.shape = shape # Shape is passed in as an argument
         
         assert self.n == reduce(mul, self.shape), "Number of neurons and shape do not match"
         
         self.spike_trace = spike_trace
         self.additive_spike_trace = additive_spike_trace
         self.sum_input = sum_input # Whether to sum all inputs
+        self.batch_size = 1
 
         if self.spike_trace:
             self.register_buffer("traces", torch.zeros(*self.shape))
             self.register_buffer("tau_s", torch.tensor(tau_s))
 
             if self.additive_spike_trace:
                 self.register_buffer("trace_scale", torch.tensor(trace_scale))
```

### Comparing `synapticflow-0.0.2/synapticflow/plotting/visualization.py` & `synapticflow-0.0.3/synapticflow/plotting/visualization.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.2/PKG-INFO` & `synapticflow-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapticflow
-Version: 0.0.2
+Version: 0.0.3
 Summary: A powerful Python package for simulating spiking neural networks (SNNs) using PyTorch with GPU acceleration.
 Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network (SNN)
 Author: Arsham Gholamzadeh Khoee
 Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee
 Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: torch (<=1.13.1)
 Description-Content-Type: text/markdown
 
 # SynapticFlow
 
 <img align='center' src="https://raw.githubusercontent.com/arsham-khoee/synapticflow/Document/docs/_static/logo-light-mode.png" alt="Light Logo" style="width: 600px; padding: 25px;"/>
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: synapticflow Version: 0.0.2 Summary: A powerful
+Metadata-Version: 2.1 Name: synapticflow Version: 0.0.3 Summary: A powerful
 Python package for simulating spiking neural networks (SNNs) using PyTorch with
 GPU acceleration. Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network
 (SNN) Author: Arsham Gholamzadeh Khoee Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 2 Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.4 Classifier:
 Programming Language :: Python :: 3.5 Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Requires-Dist: torch (<=1.13.1) Description-Content-Type: text/
-markdown # SynapticFlow [Light Logo] Spiking Neural Networks (SNNs) are a type
-of artificial neural network that attempts to mimic the behavior of neurons in
-the brain. Unlike traditional neural networks that use continuous-valued
-signals, SNNs operate using discrete spikes of activity that are similar to the
-action potentials in biological neurons. SynapticFlow is a powerful Python
-package for prototyping and simulating SNNs. It is based on PyTorch and
-supports both CPU and GPU computation. SynapticFlow extends the capabilities of
-PyTorch and enables us to take advantage of using spiking neurons.
-Additionally, it offers different variations of synaptic plasticity as well as
-delay learning for SNNs. Please consider supporting the SynapticFlow project by
-giving it a star â­ï¸ on Github, as it is a simple and effective way to show
-your appreciation and help the project gain more visibility. If you encounter
-any problems, want to share your thoughts or have any questions related to
-training spiking neural networks, we welcome you to open an issue, start a
-discussion, or join our Discord channel where we can chat and offer advice. ##
-Installation To install synapticflow, run the following command in your
-terminal: ```python $ pip install synapticflow ``` We recommend using this
-method to install synapticflow since it will ensure that you have the latest
-stable version installed. If you prefer to install synapticflow from source
-instead, follow these instructions: ```python $ git clone https://github.com/
-arsham-khoee/synapticflow $ cd synapticflow $ python setup.py install ```
+Programming Language :: Python :: 3.11 Requires-Dist: torch (<=1.13.1)
+Description-Content-Type: text/markdown # SynapticFlow [Light Logo] Spiking
+Neural Networks (SNNs) are a type of artificial neural network that attempts to
+mimic the behavior of neurons in the brain. Unlike traditional neural networks
+that use continuous-valued signals, SNNs operate using discrete spikes of
+activity that are similar to the action potentials in biological neurons.
+SynapticFlow is a powerful Python package for prototyping and simulating SNNs.
+It is based on PyTorch and supports both CPU and GPU computation. SynapticFlow
+extends the capabilities of PyTorch and enables us to take advantage of using
+spiking neurons. Additionally, it offers different variations of synaptic
+plasticity as well as delay learning for SNNs. Please consider supporting the
+SynapticFlow project by giving it a star â­ï¸ on Github, as it is a simple
+and effective way to show your appreciation and help the project gain more
+visibility. If you encounter any problems, want to share your thoughts or have
+any questions related to training spiking neural networks, we welcome you to
+open an issue, start a discussion, or join our Discord channel where we can
+chat and offer advice. ## Installation To install synapticflow, run the
+following command in your terminal: ```python $ pip install synapticflow ``` We
+recommend using this method to install synapticflow since it will ensure that
+you have the latest stable version installed. If you prefer to install
+synapticflow from source instead, follow these instructions: ```python $ git
+clone https://github.com/arsham-khoee/synapticflow $ cd synapticflow $ python
+setup.py install ```
 **** Requirements ****
 The requirements for SynapticFlow are as follows:
     * torch
     * matplotlib
 ## Usage After package installation has been finished, you can use it by
 following command: ```python import synapticflow as sf ``` In following code, a
 simple LIF neuron has been instantiated: ```python model = sf.LIFPopulation
```

