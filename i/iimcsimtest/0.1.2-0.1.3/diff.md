# Comparing `tmp/iimcsimtest-0.1.2.tar.gz` & `tmp/iimcsimtest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iimcsimtest-0.1.2.tar", last modified: Fri May 19 13:28:30 2023, max compression
+gzip compressed data, was "iimcsimtest-0.1.3.tar", last modified: Fri May 19 13:31:14 2023, max compression
```

## Comparing `iimcsimtest-0.1.2.tar` & `iimcsimtest-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 13:28:30.973663 iimcsimtest-0.1.2/
--rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsimtest-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4264 2023-05-19 13:28:30.973663 iimcsimtest-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsimtest-0.1.2/README.md
--rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsimtest-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      751 2023-05-19 13:28:30.975654 iimcsimtest-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 13:28:30.919804 iimcsimtest-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 13:28:30.956705 iimcsimtest-0.1.2/src/iimcsimtest/
--rw-rw-rw-   0        0        0     2435 2023-05-19 13:22:19.000000 iimcsimtest-0.1.2/src/iimcsimtest/MC.py
--rw-rw-rw-   0        0        0    11861 2023-05-19 11:37:00.000000 iimcsimtest-0.1.2/src/iimcsimtest/MonteCarlo.py
--rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsimtest-0.1.2/src/iimcsimtest/__init__.py
--rw-rw-rw-   0        0        0     4636 2023-05-19 13:28:11.000000 iimcsimtest-0.1.2/src/iimcsimtest/data_gen.py
--rw-rw-rw-   0        0        0      695 2023-05-19 13:17:15.000000 iimcsimtest-0.1.2/src/iimcsimtest/data_gen_run.py
--rw-rw-rw-   0        0        0     2486 2023-05-19 11:37:01.000000 iimcsimtest-0.1.2/src/iimcsimtest/shape_ext.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:28:30.971665 iimcsimtest-0.1.2/src/iimcsimtest.egg-info/
--rw-rw-rw-   0        0        0     4264 2023-05-19 13:28:30.000000 iimcsimtest-0.1.2/src/iimcsimtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-05-19 13:28:30.000000 iimcsimtest-0.1.2/src/iimcsimtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 13:28:30.000000 iimcsimtest-0.1.2/src/iimcsimtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-19 13:28:30.000000 iimcsimtest-0.1.2/src/iimcsimtest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 13:31:14.807293 iimcsimtest-0.1.3/
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsimtest-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4264 2023-05-19 13:31:14.807293 iimcsimtest-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsimtest-0.1.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsimtest-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      751 2023-05-19 13:31:14.809292 iimcsimtest-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 13:31:14.762417 iimcsimtest-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 13:31:14.790340 iimcsimtest-0.1.3/src/iimcsimtest/
+-rw-rw-rw-   0        0        0     2435 2023-05-19 13:22:19.000000 iimcsimtest-0.1.3/src/iimcsimtest/MC.py
+-rw-rw-rw-   0        0        0    11861 2023-05-19 11:37:00.000000 iimcsimtest-0.1.3/src/iimcsimtest/MonteCarlo.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsimtest-0.1.3/src/iimcsimtest/__init__.py
+-rw-rw-rw-   0        0        0     4636 2023-05-19 13:28:11.000000 iimcsimtest-0.1.3/src/iimcsimtest/data_gen.py
+-rw-rw-rw-   0        0        0      696 2023-05-19 13:30:25.000000 iimcsimtest-0.1.3/src/iimcsimtest/data_gen_run.py
+-rw-rw-rw-   0        0        0     2486 2023-05-19 11:37:01.000000 iimcsimtest-0.1.3/src/iimcsimtest/shape_ext.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:31:14.805299 iimcsimtest-0.1.3/src/iimcsimtest.egg-info/
+-rw-rw-rw-   0        0        0     4264 2023-05-19 13:31:14.000000 iimcsimtest-0.1.3/src/iimcsimtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-05-19 13:31:14.000000 iimcsimtest-0.1.3/src/iimcsimtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 13:31:14.000000 iimcsimtest-0.1.3/src/iimcsimtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-19 13:31:14.000000 iimcsimtest-0.1.3/src/iimcsimtest.egg-info/top_level.txt
```

### Comparing `iimcsimtest-0.1.2/PKG-INFO` & `iimcsimtest-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsimtest
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsimtest Version: 0.1.2 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsimtest Version: 0.1.3 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

### Comparing `iimcsimtest-0.1.2/README.md` & `iimcsimtest-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `iimcsimtest-0.1.2/setup.cfg` & `iimcsimtest-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 696d 6373 696d 7465 7374 0d0a   = iimcsimtest..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 320d  version = 0.1.2.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 330d  version = 0.1.3.
 00000030: 0a61 7574 686f 7220 3d20 4a69 6761 7220  .author = Jigar 
 00000040: 4268 616e 6465 7269 0d0a 6175 7468 6f72  Bhanderi..author
 00000050: 5f65 6d61 696c 203d 206a 6967 6172 6268  _email = jigarbh
 00000060: 616e 6465 7269 4067 6d61 696c 2e63 6f6d  anderi@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4120 7061 636b 6167 6520 666f 7220 4d6f  A package for Mo
 00000090: 6e74 652d 4361 726c 6f20 7369 6d75 6c61  nte-Carlo simula
```

### Comparing `iimcsimtest-0.1.2/src/iimcsimtest/MC.py` & `iimcsimtest-0.1.3/src/iimcsimtest/MC.py`

 * *Files identical despite different names*

### Comparing `iimcsimtest-0.1.2/src/iimcsimtest/MonteCarlo.py` & `iimcsimtest-0.1.3/src/iimcsimtest/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `iimcsimtest-0.1.2/src/iimcsimtest/data_gen.py` & `iimcsimtest-0.1.3/src/iimcsimtest/data_gen.py`

 * *Files identical despite different names*

### Comparing `iimcsimtest-0.1.2/src/iimcsimtest/data_gen_run.py` & `iimcsimtest-0.1.3/src/iimcsimtest/data_gen_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 
 def generate_data(train_exe = 50,
                 name = './src/data/plateauless_uniq_pulses_345.npy',
                 samp_size = 256,
                 max_num_photon = 60,
                 folder_name = 'sh06x2'):
     data_gen.generator(samp_size, max_num_photon, name, train_exe, folder_name)
-generate_data()
+#generate_data()
```

### Comparing `iimcsimtest-0.1.2/src/iimcsimtest/shape_ext.py` & `iimcsimtest-0.1.3/src/iimcsimtest/shape_ext.py`

 * *Files identical despite different names*

### Comparing `iimcsimtest-0.1.2/src/iimcsimtest.egg-info/PKG-INFO` & `iimcsimtest-0.1.3/src/iimcsimtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsimtest
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsimtest Version: 0.1.2 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsimtest Version: 0.1.3 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

