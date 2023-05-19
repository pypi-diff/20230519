# Comparing `tmp/komm-0.7.2.tar.gz` & `tmp/komm-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komm-0.7.2.tar", last modified: Sat May 13 23:26:15 2023, max compression
+gzip compressed data, was "komm-0.7.3.tar", last modified: Fri May 19 20:27:46 2023, max compression
```

## Comparing `komm-0.7.2.tar` & `komm-0.7.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-13 23:26:15.274428 komm-0.7.2/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    35147 2023-05-13 23:05:18.000000 komm-0.7.2/LICENSE
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-13 23:26:15.271095 komm-0.7.2/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1757 2023-05-13 23:19:40.000000 komm-0.7.2/README.rst
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-13 23:26:15.267762 komm-0.7.2/komm/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      620 2023-05-13 23:18:38.000000 komm-0.7.2/komm/__init__.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    32335 2023-05-13 23:09:56.000000 komm-0.7.2/komm/_algebra.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      189 2023-05-13 23:05:18.000000 komm-0.7.2/komm/_aux.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14967 2023-05-13 23:11:52.000000 komm-0.7.2/komm/_channels.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    67646 2023-05-13 23:12:00.000000 komm-0.7.2/komm/_error_control_block.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      123 2023-05-13 23:05:18.000000 komm-0.7.2/komm/_error_control_checksum.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    20369 2023-05-13 23:09:56.000000 komm-0.7.2/komm/_error_control_convolutional.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    18086 2023-05-13 23:08:37.000000 komm-0.7.2/komm/_finite_state_machine.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    30566 2023-05-13 23:11:52.000000 komm-0.7.2/komm/_modulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14874 2023-05-13 23:08:37.000000 komm-0.7.2/komm/_pulses.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8251 2023-05-13 23:08:37.000000 komm-0.7.2/komm/_quantization.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19729 2023-05-13 23:08:28.000000 komm-0.7.2/komm/_sequences.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19050 2023-05-13 23:05:18.000000 komm-0.7.2/komm/_source_coding.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2190 2023-05-13 23:08:37.000000 komm-0.7.2/komm/_sources.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5404 2023-05-13 23:13:14.000000 komm-0.7.2/komm/_util.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-13 23:26:15.271095 komm-0.7.2/komm.egg-info/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      791 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/SOURCES.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/dependency_links.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       12 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/requires.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        5 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/top_level.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2023-05-13 23:26:15.274428 komm-0.7.2/setup.cfg
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1623 2023-05-13 23:25:06.000000 komm-0.7.2/setup.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-13 23:26:15.271095 komm-0.7.2/tests/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7141 2023-05-13 23:05:18.000000 komm-0.7.2/tests/test_algebra.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2023-05-13 23:05:18.000000 komm-0.7.2/tests/test_channels.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14875 2023-05-13 23:08:28.000000 komm-0.7.2/tests/test_error_control_block.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8605 2023-05-13 23:08:28.000000 komm-0.7.2/tests/test_error_control_convolutional.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2661 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_finite_state_machine.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1860 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_modulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1802 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_quantization.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      976 2023-05-13 23:08:28.000000 komm-0.7.2/tests/test_sequences.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3028 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_source_coding.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      289 2023-05-13 23:08:28.000000 komm-0.7.2/tests/test_sources.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-19 20:27:46.246847 komm-0.7.3/
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    35147 2022-07-22 15:17:50.000000 komm-0.7.3/LICENSE
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-19 20:27:46.243513 komm-0.7.3/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1757 2023-05-13 23:19:40.000000 komm-0.7.3/README.rst
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-19 20:27:46.230180 komm-0.7.3/komm/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      620 2023-05-13 23:18:38.000000 komm-0.7.3/komm/__init__.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    32335 2023-05-13 23:09:56.000000 komm-0.7.3/komm/_algebra.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      189 2022-07-22 15:17:50.000000 komm-0.7.3/komm/_aux.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14964 2023-05-19 20:25:27.000000 komm-0.7.3/komm/_channels.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    67646 2023-05-13 23:12:00.000000 komm-0.7.3/komm/_error_control_block.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      123 2022-07-22 15:17:50.000000 komm-0.7.3/komm/_error_control_checksum.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    20369 2023-05-13 23:09:56.000000 komm-0.7.3/komm/_error_control_convolutional.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    18086 2023-05-13 23:08:37.000000 komm-0.7.3/komm/_finite_state_machine.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    30566 2023-05-13 23:11:52.000000 komm-0.7.3/komm/_modulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14874 2023-05-13 23:08:37.000000 komm-0.7.3/komm/_pulses.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8251 2023-05-13 23:08:37.000000 komm-0.7.3/komm/_quantization.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19729 2023-05-13 23:08:28.000000 komm-0.7.3/komm/_sequences.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19050 2022-07-22 15:17:50.000000 komm-0.7.3/komm/_source_coding.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2190 2023-05-13 23:08:37.000000 komm-0.7.3/komm/_sources.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5404 2023-05-13 23:36:24.000000 komm-0.7.3/komm/_util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-19 20:27:46.230180 komm-0.7.3/komm.egg-info/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      791 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/SOURCES.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/dependency_links.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       12 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/requires.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        5 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/top_level.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2023-05-19 20:27:46.246847 komm-0.7.3/setup.cfg
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1623 2023-05-19 20:26:34.000000 komm-0.7.3/setup.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-19 20:27:46.240180 komm-0.7.3/tests/
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7141 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_algebra.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_channels.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14875 2023-05-13 23:08:28.000000 komm-0.7.3/tests/test_error_control_block.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8605 2023-05-13 23:08:28.000000 komm-0.7.3/tests/test_error_control_convolutional.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2661 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_finite_state_machine.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1860 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_modulation.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1802 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_quantization.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      976 2023-05-13 23:08:28.000000 komm-0.7.3/tests/test_sequences.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3028 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_source_coding.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      289 2023-05-13 23:08:28.000000 komm-0.7.3/tests/test_sources.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_util.py
```

### Comparing `komm-0.7.2/LICENSE` & `komm-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/PKG-INFO` & `komm-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komm
-Version: 0.7.2
+Version: 0.7.3
 Summary: An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.
 Home-page: https://github.com/rwnobrega/komm/
 Author: Roberto W. Nobrega
 Author-email: rwnobrega@gmail.com
 License: GPL
 Project-URL: Documentation, http://komm.readthedocs.io/
 Project-URL: Source, https://github.com/rwnobrega/komm/
```

### Comparing `komm-0.7.2/README.rst` & `komm-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/__init__.py` & `komm-0.7.3/komm/__init__.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_algebra.py` & `komm-0.7.3/komm/_algebra.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_channels.py` & `komm-0.7.3/komm/_channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         if self._signal_power == 'measured':
             signal_power = np.linalg.norm(input_signal)**2 / size
         else:
             signal_power = self._signal_power
 
         noise_power = signal_power / self._snr
 
-        if input_signal.dtype == np.complex:
+        if input_signal.dtype == complex:
             noise = np.sqrt(noise_power / 2) * (np.random.normal(size=size) + 1j * np.random.normal(size=size))
         else:
             noise = np.sqrt(noise_power) * np.random.normal(size=size)
 
         return input_signal + noise
 
     def __repr__(self):
```

### Comparing `komm-0.7.2/komm/_error_control_block.py` & `komm-0.7.3/komm/_error_control_block.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_error_control_convolutional.py` & `komm-0.7.3/komm/_error_control_convolutional.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_finite_state_machine.py` & `komm-0.7.3/komm/_finite_state_machine.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_modulation.py` & `komm-0.7.3/komm/_modulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_pulses.py` & `komm-0.7.3/komm/_pulses.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_quantization.py` & `komm-0.7.3/komm/_quantization.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_sequences.py` & `komm-0.7.3/komm/_sequences.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_source_coding.py` & `komm-0.7.3/komm/_source_coding.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_sources.py` & `komm-0.7.3/komm/_sources.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm/_util.py` & `komm-0.7.3/komm/_util.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/komm.egg-info/PKG-INFO` & `komm-0.7.3/komm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komm
-Version: 0.7.2
+Version: 0.7.3
 Summary: An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.
 Home-page: https://github.com/rwnobrega/komm/
 Author: Roberto W. Nobrega
 Author-email: rwnobrega@gmail.com
 License: GPL
 Project-URL: Documentation, http://komm.readthedocs.io/
 Project-URL: Source, https://github.com/rwnobrega/komm/
```

### Comparing `komm-0.7.2/komm.egg-info/SOURCES.txt` & `komm-0.7.3/komm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/setup.py` & `komm-0.7.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 For library reference, please check the project's `documentation page at Read the Docs <http://komm.readthedocs.io/>`_.
 
 This software is still under development. Contributions are very welcome!
 '''
 
 setup(
     name='komm',
-    version='0.7.2',
+    version='0.7.3',
     description='An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.',
     long_description=_long_description,
     url='https://github.com/rwnobrega/komm/',
     author='Roberto W. Nobrega',
     author_email='rwnobrega@gmail.com',
     license='GPL',
     project_urls={
```

### Comparing `komm-0.7.2/tests/test_algebra.py` & `komm-0.7.3/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/tests/test_error_control_block.py` & `komm-0.7.3/tests/test_error_control_block.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/tests/test_error_control_convolutional.py` & `komm-0.7.3/tests/test_error_control_convolutional.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/tests/test_finite_state_machine.py` & `komm-0.7.3/tests/test_finite_state_machine.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/tests/test_modulation.py` & `komm-0.7.3/tests/test_modulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/tests/test_quantization.py` & `komm-0.7.3/tests/test_quantization.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/tests/test_sequences.py` & `komm-0.7.3/tests/test_sequences.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.2/tests/test_source_coding.py` & `komm-0.7.3/tests/test_source_coding.py`

 * *Files identical despite different names*

