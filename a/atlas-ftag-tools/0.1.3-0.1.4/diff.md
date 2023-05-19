# Comparing `tmp/atlas-ftag-tools-0.1.3.tar.gz` & `tmp/atlas-ftag-tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-ftag-tools-0.1.3.tar", last modified: Wed May 10 10:04:11 2023, max compression
+gzip compressed data, was "atlas-ftag-tools-0.1.4.tar", last modified: Fri May 19 12:34:10 2023, max compression
```

## Comparing `atlas-ftag-tools-0.1.3.tar` & `atlas-ftag-tools-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.922552 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/ftag/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/flavour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/flavours.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/ftag/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/hdf5/h5reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/hdf5/h5utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/hdf5/h5writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/vds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/ftag/wps/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/wps/discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/wps/working_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.232859 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/ftag/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/flavour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/flavours.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/ftag/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/hdf5/h5reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/hdf5/h5utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/hdf5/h5writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/vds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/ftag/wps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/wps/discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/wps/working_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/setup.cfg
```

### Comparing `atlas-ftag-tools-0.1.3/PKG-INFO` & `atlas-ftag-tools-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-ftag-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: ATLAS Flavour Tagging Tools
 Author: Sam Van Stroud, Philipp Gadow
 License: MIT
 Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -25,15 +25,15 @@
 
 If you want to use this package without modification, you can install from [pypi](https://pypi.org/project/atlas-ftag-tools/) using `pip`.
 
 ```bash
 pip install atlas-ftag-tools
 ```
 
-To additionally install the development dependencies (for formatting and linting) rn
+To additionally install the development dependencies (for formatting and linting) use
 ```bash
 pip install atlas-ftag-tools[dev]
 ```
 
 ## Development
 
 If you plan on making changes to teh code, instead clone the repository and install the package from source in editable mode with
@@ -44,31 +44,35 @@
 
 Include development dependencies with
 
 ```bash
 python -m pip install -e ".[dev]"
 ```
 
-You can set up pre-commit hooks with
+You can set up and run pre-commit hooks with
 
 ```bash
 pre-commit install
+pre-commmit run --all-files
 ```
 
 To run the tests you can use the `pytest` or `coverage` command, for example
 
 ```bash
 coverage run --source ftag -m pytest --show-capture=stdout
 ```
 
 Running `coverage report` will display the test coverage.
 
 
 # Usage
 
+Please see the [example notebook](ftag/example.ipynb) for full usage.
+Additional functionality is also documented below.
+
 ## Create virtual file
 
 This package contains a script to easily merge a set of H5 files.
 A virtual file is a fast and lightweight way to wrap a set of files.
 See the [h5py documentation](https://docs.h5py.org/en/stable/vds.html) for more information on virtual datasets.
 
 The script is `vds.py` and can be run after installing this package with
```

### Comparing `atlas-ftag-tools-0.1.3/README.md` & `atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: atlas-ftag-tools
+Version: 0.1.4
+Summary: ATLAS Flavour Tagging Tools
+Author: Sam Van Stroud, Philipp Gadow
+License: MIT
+Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/atlas-ftag-tools.svg)](https://badge.fury.io/py/atlas-ftag-tools)
 [![codecov](https://codecov.io/gh/umami-hep/atlas-ftag-tools/branch/main/graph/badge.svg?token=MBHLIYYQ7I)](https://codecov.io/gh/umami-hep/atlas-ftag-tools)
 
 # ATLAS FTAG Python Tools
 
 This is a collection of Python tools for working with files produced with the FTAG [ntuple dumper](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-dataset-dumper/).
@@ -14,15 +25,15 @@
 
 If you want to use this package without modification, you can install from [pypi](https://pypi.org/project/atlas-ftag-tools/) using `pip`.
 
 ```bash
 pip install atlas-ftag-tools
 ```
 
-To additionally install the development dependencies (for formatting and linting) rn
+To additionally install the development dependencies (for formatting and linting) use
 ```bash
 pip install atlas-ftag-tools[dev]
 ```
 
 ## Development
 
 If you plan on making changes to teh code, instead clone the repository and install the package from source in editable mode with
@@ -33,31 +44,35 @@
 
 Include development dependencies with
 
 ```bash
 python -m pip install -e ".[dev]"
 ```
 
-You can set up pre-commit hooks with
+You can set up and run pre-commit hooks with
 
 ```bash
 pre-commit install
+pre-commmit run --all-files
 ```
 
 To run the tests you can use the `pytest` or `coverage` command, for example
 
 ```bash
 coverage run --source ftag -m pytest --show-capture=stdout
 ```
 
 Running `coverage report` will display the test coverage.
 
 
 # Usage
 
+Please see the [example notebook](ftag/example.ipynb) for full usage.
+Additional functionality is also documented below.
+
 ## Create virtual file
 
 This package contains a script to easily merge a set of H5 files.
 A virtual file is a fast and lightweight way to wrap a set of files.
 See the [h5py documentation](https://docs.h5py.org/en/stable/vds.html) for more information on virtual datasets.
 
 The script is `vds.py` and can be run after installing this package with
```

### Comparing `atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/PKG-INFO` & `atlas-ftag-tools-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: atlas-ftag-tools
-Version: 0.1.3
-Summary: ATLAS Flavour Tagging Tools
-Author: Sam Van Stroud, Philipp Gadow
-License: MIT
-Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/atlas-ftag-tools.svg)](https://badge.fury.io/py/atlas-ftag-tools)
 [![codecov](https://codecov.io/gh/umami-hep/atlas-ftag-tools/branch/main/graph/badge.svg?token=MBHLIYYQ7I)](https://codecov.io/gh/umami-hep/atlas-ftag-tools)
 
 # ATLAS FTAG Python Tools
 
 This is a collection of Python tools for working with files produced with the FTAG [ntuple dumper](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-dataset-dumper/).
@@ -25,15 +14,15 @@
 
 If you want to use this package without modification, you can install from [pypi](https://pypi.org/project/atlas-ftag-tools/) using `pip`.
 
 ```bash
 pip install atlas-ftag-tools
 ```
 
-To additionally install the development dependencies (for formatting and linting) rn
+To additionally install the development dependencies (for formatting and linting) use
 ```bash
 pip install atlas-ftag-tools[dev]
 ```
 
 ## Development
 
 If you plan on making changes to teh code, instead clone the repository and install the package from source in editable mode with
@@ -44,31 +33,35 @@
 
 Include development dependencies with
 
 ```bash
 python -m pip install -e ".[dev]"
 ```
 
-You can set up pre-commit hooks with
+You can set up and run pre-commit hooks with
 
 ```bash
 pre-commit install
+pre-commmit run --all-files
 ```
 
 To run the tests you can use the `pytest` or `coverage` command, for example
 
 ```bash
 coverage run --source ftag -m pytest --show-capture=stdout
 ```
 
 Running `coverage report` will display the test coverage.
 
 
 # Usage
 
+Please see the [example notebook](ftag/example.ipynb) for full usage.
+Additional functionality is also documented below.
+
 ## Create virtual file
 
 This package contains a script to easily merge a set of H5 files.
 A virtual file is a fast and lightweight way to wrap a set of files.
 See the [h5py documentation](https://docs.h5py.org/en/stable/vds.html) for more information on virtual datasets.
 
 The script is `vds.py` and can be run after installing this package with
```

### Comparing `atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/SOURCES.txt` & `atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.3/ftag/__init__.py` & `atlas-ftag-tools-0.1.4/ftag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """atlas-ftag-tools - Common tools for ATLAS flavour tagging software."""
 
 
-__version__ = "v0.1.3"
+__version__ = "v0.1.4"
 
 
 import ftag.hdf5 as hdf5
 from ftag.cuts import Cuts
 from ftag.flavour import Flavour, Flavours
 from ftag.mock import get_mock_file
 from ftag.sample import Sample
```

### Comparing `atlas-ftag-tools-0.1.3/ftag/cuts.py` & `atlas-ftag-tools-0.1.4/ftag/cuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "<=": operator.le,
     ">": operator.gt,
     "<": operator.lt,
     "in": lambda x, y: np.isin(x, y),
     "notin": lambda x, y: ~np.isin(x, y),
 }
 
-for i in range(2, 20):
+for i in range(2, 101):
     OPERATORS[f"%{i}=="] = functools.partial(lambda x, y, i: (x % i) == y, i=i)
     OPERATORS[f"%{i}<="] = functools.partial(lambda x, y, i: (x % i) <= y, i=i)
     OPERATORS[f"%{i}>="] = functools.partial(lambda x, y, i: (x % i) >= y, i=i)
 
 CutsResult = namedtuple("CutsResult", "idx values")
```

### Comparing `atlas-ftag-tools-0.1.3/ftag/flavour.py` & `atlas-ftag-tools-0.1.4/ftag/flavour.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.3/ftag/flavours.yaml` & `atlas-ftag-tools-0.1.4/ftag/flavours.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,19 @@
   colour: "#B45F06"
   category: xbb
 - name: top
   label: Top
   cuts: ["R10TruthLabel_R22v1 == 1"]
   colour: "#A300A3"
   category: xbb
+- name: inclusive_top
+  label: Inclusive Top
+  cuts: ["R10TruthLabel_R22v1 in (1,6,7)"]
+  colour: "#A300A3"
+  category: xbb
 - name: qcd
   label: QCD
   cuts: ["R10TruthLabel_R22v1 == 10"]
   colour: "#38761D"
   category: xbb
 
 # partonic labelling
```

### Comparing `atlas-ftag-tools-0.1.3/ftag/hdf5/h5reader.py` & `atlas-ftag-tools-0.1.4/ftag/hdf5/h5reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,16 @@
 
             # select
             yield data
 
     def load(
         self, variables: dict | None = None, num_jets: int | None = None, cuts: Cuts | None = None
     ) -> dict:
+        if num_jets == -1:
+            num_jets = self.num_jets
         if variables is None:
             variables = {self.jets_name: None}
         data: dict[str, list] = {name: [] for name in variables}
         for sample in self.stream(variables, num_jets, cuts):
             for name, array in sample.items():
                 if name in data:
                     data[name].append(array)
```

### Comparing `atlas-ftag-tools-0.1.3/ftag/hdf5/h5utils.py` & `atlas-ftag-tools-0.1.4/ftag/hdf5/h5utils.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.3/ftag/hdf5/h5writer.py` & `atlas-ftag-tools-0.1.4/ftag/hdf5/h5writer.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.3/ftag/mock.py` & `atlas-ftag-tools-0.1.4/ftag/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     scores = get_mock_scores(jets["HadronConeExclTruthLabelID"])
     jets = join_structured_arrays([jets, scores])
 
     # create a tempfile in a new folder
     fname = NamedTemporaryFile(suffix=".h5", dir=mkdtemp()).name
     f = h5py.File(fname, "w")
     f.create_dataset("jets", data=jets)
+    f.attrs["test"] = "test"
 
     # setup tracks
     if tracks_name:
         tracks_dtype = np.dtype(TRACK_VARS)
         tracks = u2s(rng.random((num_jets, num_tracks, len(TRACK_VARS))), tracks_dtype)
         valid = rng.choice([True, False], size=(num_jets, num_tracks))
         valid = valid.astype(bool).view(dtype=np.dtype([("valid", bool)]))
```

### Comparing `atlas-ftag-tools-0.1.3/ftag/sample.py` & `atlas-ftag-tools-0.1.4/ftag/sample.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.3/ftag/vds.py` & `atlas-ftag-tools-0.1.4/ftag/vds.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 from __future__ import annotations
 
+import argparse
 import glob
 from pathlib import Path
 
 import h5py
 
 
+def parse_args(args):
+    parser = argparse.ArgumentParser(
+        description="Create a lightweight wrapper around a set of h5 files"
+    )
+    parser.add_argument("pattern", type=Path, help="quotes-enclosed glob pattern of files to merge")
+    parser.add_argument("output", type=Path, help="path to output virtual file")
+    args = parser.parse_args(args)
+    return args
+
+
 def get_virtual_layout(fnames: list[str], group: str):
     # get sources
     sources = []
     total = 0
     for fname in fnames:
         with h5py.File(fname) as f:
             vsource = h5py.VirtualSource(f[group])
@@ -54,28 +65,30 @@
 
     # create virtual file
     out_fname.parent.mkdir(exist_ok=True)
     with h5py.File(out_fname, "w") as f:
         for group in h5py.File(fnames[0]):
             layout = get_virtual_layout(fnames, group)
             f.create_virtual_dataset(group, layout)
+            attrs_dict: dict = {}
+            for fname in fnames:
+                with h5py.File(fname) as g:
+                    for name, value in g[group].attrs.items():
+                        if name not in attrs_dict:
+                            attrs_dict[name] = []
+                        attrs_dict[name].append(value)
+            for name, value in attrs_dict.items():
+                if len(value) > 0:
+                    f[group].attrs[name] = value[0]
 
     return out_fname
 
 
-def main():
-    import argparse
-
-    parser = argparse.ArgumentParser(
-        description="Create a lightweight wrapper around a set of h5 files"
-    )
-    parser.add_argument("pattern", type=Path, help="quotes-enclosed glob pattern of files to merge")
-    parser.add_argument("output", type=Path, help="path to output virtual file")
-    args = parser.parse_args()
-
+def main(args=None):
+    args = parse_args(args)
     print(f"Globbing {args.pattern}...")
     create_virtual_file(args.pattern, args.output, overwrite=True)
     with h5py.File(args.output) as f:
         key = list(f.keys())[0]
         num = len(f[key])
     print(f"Virtual dataset '{key}' has {num:,} entries")
     print(f"Saved virtual file to {args.output.resolve()}")
```

### Comparing `atlas-ftag-tools-0.1.3/ftag/wps/discriminant.py` & `atlas-ftag-tools-0.1.4/ftag/wps/discriminant.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.3/ftag/wps/working_points.py` & `atlas-ftag-tools-0.1.4/ftag/wps/working_points.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.3/pyproject.toml` & `atlas-ftag-tools-0.1.4/pyproject.toml`

 * *Files identical despite different names*

