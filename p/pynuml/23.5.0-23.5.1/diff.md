# Comparing `tmp/pynuml-23.5.0.tar.gz` & `tmp/pynuml-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynuml-23.5.0.tar", last modified: Thu May 11 22:09:01 2023, max compression
+gzip compressed data, was "pynuml-23.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynuml-23.5.0.tar` & `pynuml-23.5.1.tar`

### file list

```diff
@@ -1,14 +1,31 @@
-drwxr-xr-x   0 vhewes     (501) staff       (20)        0 2023-05-11 22:09:01.658201 pynuml-23.5.0/
--rw-r--r--   0 vhewes     (501) staff       (20)     1064 2022-08-22 18:47:46.000000 pynuml-23.5.0/LICENCE
--rw-r--r--   0 vhewes     (501) staff       (20)     6376 2023-05-11 22:09:01.658074 pynuml-23.5.0/PKG-INFO
--rw-r--r--   0 vhewes     (501) staff       (20)     5647 2023-05-11 17:09:33.000000 pynuml-23.5.0/README.md
-drwxr-xr-x   0 vhewes     (501) staff       (20)        0 2023-05-11 22:09:01.657366 pynuml-23.5.0/pynuml/
--rw-r--r--   0 vhewes     (501) staff       (20)       79 2023-05-11 17:09:32.000000 pynuml-23.5.0/pynuml/__init__.py
-drwxr-xr-x   0 vhewes     (501) staff       (20)        0 2023-05-11 22:09:01.657925 pynuml-23.5.0/pynuml.egg-info/
--rw-r--r--   0 vhewes     (501) staff       (20)     6376 2023-05-11 22:09:01.000000 pynuml-23.5.0/pynuml.egg-info/PKG-INFO
--rw-r--r--   0 vhewes     (501) staff       (20)      200 2023-05-11 22:09:01.000000 pynuml-23.5.0/pynuml.egg-info/SOURCES.txt
--rw-r--r--   0 vhewes     (501) staff       (20)        1 2023-05-11 22:09:01.000000 pynuml-23.5.0/pynuml.egg-info/dependency_links.txt
--rw-r--r--   0 vhewes     (501) staff       (20)       72 2023-05-11 22:09:01.000000 pynuml-23.5.0/pynuml.egg-info/requires.txt
--rw-r--r--   0 vhewes     (501) staff       (20)        7 2023-05-11 22:09:01.000000 pynuml-23.5.0/pynuml.egg-info/top_level.txt
--rw-r--r--   0 vhewes     (501) staff       (20)      982 2023-05-11 22:01:06.000000 pynuml-23.5.0/pyproject.toml
--rw-r--r--   0 vhewes     (501) staff       (20)       38 2023-05-11 22:09:01.658235 pynuml-23.5.0/setup.cfg
+-rw-r--r--   0        0        0       17 2022-08-22 18:40:35.802435 pynuml-23.5.1/.gitignore
+-rw-r--r--   0        0        0     1074 2023-05-19 17:54:50.911108 pynuml-23.5.1/LICENSE
+-rw-r--r--   0        0        0     5647 2023-05-17 21:45:54.952303 pynuml-23.5.1/README.md
+-rw-r--r--   0        0        0      170 2022-08-22 18:40:35.802435 pynuml-23.5.1/doc/README.md
+-rw-r--r--   0        0        0     9267 2022-08-22 18:40:35.802435 pynuml-23.5.1/doc/graph_create.md
+-rw-r--r--   0        0        0     2903 2022-08-22 18:40:35.802435 pynuml-23.5.1/doc/python_env.md
+-rw-r--r--   0        0        0      638 2023-04-03 15:38:40.928784 pynuml-23.5.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-03 15:38:40.932784 pynuml-23.5.1/docs/make.bat
+-rw-r--r--   0        0        0      916 2023-04-03 15:38:40.932784 pynuml-23.5.1/docs/source/conf.py
+-rw-r--r--   0        0        0      671 2023-04-03 15:38:40.932784 pynuml-23.5.1/docs/source/index.rst
+-rw-r--r--   0        0        0      581 2022-08-22 15:18:00.634737 pynuml-23.5.1/example/plot.py
+-rwxr-xr-x   0        0        0     2089 2022-11-15 22:26:27.438225 pynuml-23.5.1/example/process.py
+-rw-r--r--   0        0        0     1169 2022-08-22 18:40:35.802435 pynuml-23.5.1/h5merge.py
+-rw-r--r--   0        0        0       38 2022-11-15 18:40:24.677584 pynuml-23.5.1/pynuml/.gitignore
+-rw-r--r--   0        0        0      164 2023-05-19 19:12:57.703058 pynuml-23.5.1/pynuml/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-19 18:59:36.039498 pynuml-23.5.1/pynuml/io/__init__.py
+-rw-r--r--   0        0        0    33686 2023-05-17 21:45:54.952303 pynuml-23.5.1/pynuml/io/file.py
+-rw-r--r--   0        0        0     3290 2023-05-17 21:45:54.952303 pynuml-23.5.1/pynuml/io/h5interface.py
+-rw-r--r--   0        0        0     4083 2023-05-17 21:45:54.952303 pynuml-23.5.1/pynuml/io/out.py
+-rw-r--r--   0        0        0       69 2023-03-07 20:27:07.502862 pynuml-23.5.1/pynuml/labels/__init__.py
+-rw-r--r--   0        0        0     1476 2022-11-15 18:40:24.677584 pynuml-23.5.1/pynuml/labels/ccqe.py
+-rw-r--r--   0        0        0      779 2023-03-07 20:27:07.502862 pynuml-23.5.1/pynuml/labels/simple.py
+-rw-r--r--   0        0        0    10532 2023-05-19 19:00:00.405738 pynuml-23.5.1/pynuml/labels/standard.py
+-rw-r--r--   0        0        0       28 2023-03-15 20:32:17.479263 pynuml-23.5.1/pynuml/plot/__init__.py
+-rw-r--r--   0        0        0     5246 2023-05-17 21:45:54.952303 pynuml-23.5.1/pynuml/plot/graph.py
+-rw-r--r--   0        0        0       39 2023-02-28 00:57:35.995625 pynuml-23.5.1/pynuml/process/__init__.py
+-rw-r--r--   0        0        0      463 2023-02-28 00:57:35.995625 pynuml-23.5.1/pynuml/process/base.py
+-rw-r--r--   0        0        0     6095 2023-05-17 21:54:36.098985 pynuml-23.5.1/pynuml/process/hitgraph.py
+-rw-r--r--   0        0        0     3780 2022-11-15 18:40:24.677584 pynuml-23.5.1/pynuml/process/spmap.py
+-rw-r--r--   0        0        0      585 2023-05-19 19:08:37.474232 pynuml-23.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6181 1970-01-01 00:00:00.000000 pynuml-23.5.1/PKG-INFO
```

### Comparing `pynuml-23.5.0/LICENCE` & `pynuml-23.5.1/LICENSE`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
+The MIT License (MIT)
 
-Copyright (c) 2022 v hewes
+Copyright (c) 2023 v hewes
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `pynuml-23.5.0/PKG-INFO` & `pynuml-23.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: pynuml
-Version: 23.5.0
+Version: 23.5.1
 Summary: Standardised ML input processing for particle physics
-License: MIT License
-Project-URL: Homepage, https://github.com/vhewes/pynuml
-Project-URL: Bug Tracker, https://github.com/vhewes/pynuml/issues
-Keywords: physics,neutrino,gnn,hdf5
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Author-email: v hewes <vhewes@fnal.gov>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENCE
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: h5py>=3.7.0
+Requires-Dist: mpi4py
+Requires-Dist: pandas
+Requires-Dist: particle
+Requires-Dist: torch>=1.12.1
+Requires-Dist: torch-geometric>=2.1.0
+Project-URL: Home, https://github.com/vhewes/pynuml
 
 # PyNuML: HDF5 IO and ML processing for neutrino physics
 
 PyNuML is a Python toolkit for processing machine learning (ML) inputs from neutrino physics simulation datasets. It offers efficient MPI parallel processing of datasets, including standardised solutions for generating semantic and instance labels from low-level particle simulation, and constructing PyTorch ML inputs such as pixel maps and graphs. The package uses a modular design to maximise flexibility and extensibility, allowing the user to write custom labelling and/or object formation code in place of the algorithms provided.
 
 ## Parallel Event IO
 
@@ -63,7 +61,8 @@
 
 ```
 git clone https://github.com/vhewes/pynuml
 pip install -e ./pynuml
 ```
 
 If installed using this method, any modifications made to your local PyNuML release will be reflected in the `pynuml` module when imported at runtime.
+
```

### Comparing `pynuml-23.5.0/README.md` & `pynuml-23.5.1/README.md`

 * *Files identical despite different names*

