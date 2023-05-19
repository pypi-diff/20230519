# Comparing `tmp/pyplink-1.3.5.tar.gz` & `tmp/pyplink-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyplink-1.3.5.tar", last modified: Tue Feb 20 14:47:44 2018, max compression
+gzip compressed data, was "pyplink-1.3.6.tar", last modified: Fri May 19 17:41:03 2023, max compression
```

## Comparing `pyplink-1.3.5.tar` & `pyplink-1.3.6.tar`

### file list

```diff
@@ -1,28 +1,41 @@
-drwx------   0 lemieuxl (12551) pgx      (35376)        0 2018-02-20 14:47:44.000000 pyplink-1.3.5/
--rw-r--r--   0 lemieuxl (12551) pgx      (35376)       39 2015-07-09 19:40:05.000000 pyplink-1.3.5/MANIFEST.in
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)     1107 2015-06-23 17:29:27.000000 pyplink-1.3.5/LICENSE.txt
-drwx------   0 lemieuxl (12551) pgx      (35376)        0 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink.egg-info/
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)      534 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink.egg-info/SOURCES.txt
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)        1 2015-07-07 19:39:27.000000 pyplink-1.3.5/pyplink.egg-info/not-zip-safe
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)        1 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink.egg-info/dependency_links.txt
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)        8 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink.egg-info/top_level.txt
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)       39 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink.egg-info/requires.txt
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)      973 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink.egg-info/PKG-INFO
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)       47 2015-09-01 13:37:48.000000 pyplink-1.3.5/pyplink.egg-info/pbr.json
--rw-------   0 lemieuxl (12551) pgx      (35376)       38 2018-02-20 14:47:44.000000 pyplink-1.3.5/setup.cfg
--rw-------   0 lemieuxl (12551) pgx      (35376)     2290 2018-02-20 14:43:48.000000 pyplink-1.3.5/README.mkd
-drwx------   0 lemieuxl (12551) pgx      (35376)        0 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink/
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)     2095 2017-03-10 17:53:48.000000 pyplink-1.3.5/pyplink/__init__.py
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)       87 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink/version.py
-drwx------   0 lemieuxl (12551) pgx      (35376)        0 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink/tests/
-drwx------   0 lemieuxl (12551) pgx      (35376)        0 2018-02-20 14:47:44.000000 pyplink-1.3.5/pyplink/tests/data/
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)      240 2017-03-10 17:53:48.000000 pyplink-1.3.5/pyplink/tests/data/test_data_with_dup.bim
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)      243 2017-03-10 17:53:48.000000 pyplink-1.3.5/pyplink/tests/data/test_data.bim
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)       13 2015-07-07 14:56:27.000000 pyplink-1.3.5/pyplink/tests/data/test_data.bed
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)       95 2015-07-07 14:56:27.000000 pyplink-1.3.5/pyplink/tests/data/test_data.fam
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)     1386 2015-07-07 19:39:14.000000 pyplink-1.3.5/pyplink/tests/__init__.py
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)    45684 2017-03-24 18:02:59.000000 pyplink-1.3.5/pyplink/tests/test_pyplink.py
--rw-rw-r--   0 lemieuxl (12551) pgx      (35376)     1406 2017-03-10 17:53:48.000000 pyplink-1.3.5/pyplink/tests/__main__.py
--rw-------   0 lemieuxl (12551) pgx      (35376)    18688 2018-02-20 14:43:48.000000 pyplink-1.3.5/pyplink/pyplink.py
--rw-------   0 lemieuxl (12551) pgx      (35376)     2650 2018-02-20 14:43:48.000000 pyplink-1.3.5/setup.py
--rw-------   0 lemieuxl (12551) pgx      (35376)      973 2018-02-20 14:47:44.000000 pyplink-1.3.5/PKG-INFO
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 17:41:03.464606 pyplink-1.3.6/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      153 2018-05-02 17:13:27.000000 pyplink-1.3.6/.coveragerc
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      130 2022-02-28 14:27:42.000000 pyplink-1.3.6/.gitignore
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1107 2018-05-02 17:13:27.000000 pyplink-1.3.6/LICENSE.txt
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       38 2022-02-28 14:27:42.000000 pyplink-1.3.6/MANIFEST.in
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      978 2023-05-19 17:41:03.464606 pyplink-1.3.6/PKG-INFO
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     2162 2023-05-19 17:37:51.000000 pyplink-1.3.6/README.md
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 17:41:03.462606 pyplink-1.3.6/conda_recipe/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       46 2019-11-29 21:01:40.000000 pyplink-1.3.6/conda_recipe/build.sh
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      841 2019-11-29 21:05:22.000000 pyplink-1.3.6/conda_recipe/meta.yaml
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      195 2019-11-29 21:05:22.000000 pyplink-1.3.6/conda_recipe/run_test.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 17:41:03.462606 pyplink-1.3.6/demo/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    48320 2018-05-02 17:13:27.000000 pyplink-1.3.6/demo/PyPlink Demo.ipynb
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 17:41:03.463606 pyplink-1.3.6/docs/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      604 2018-05-02 17:13:27.000000 pyplink-1.3.6/docs/Makefile
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     5505 2018-05-02 17:13:27.000000 pyplink-1.3.6/docs/conf.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1067 2018-05-02 17:13:27.000000 pyplink-1.3.6/docs/index.rst
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      616 2018-05-02 17:13:27.000000 pyplink-1.3.6/docs/installation.rst
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      115 2018-05-02 17:13:27.000000 pyplink-1.3.6/docs/pyplink.rst
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 17:41:03.463606 pyplink-1.3.6/pyplink/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     2095 2018-05-02 17:13:27.000000 pyplink-1.3.6/pyplink/__init__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    18413 2023-05-19 17:37:51.000000 pyplink-1.3.6/pyplink/pyplink.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 17:41:03.463606 pyplink-1.3.6/pyplink/tests/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1405 2023-05-19 17:37:51.000000 pyplink-1.3.6/pyplink/tests/__init__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1435 2023-05-19 17:37:51.000000 pyplink-1.3.6/pyplink/tests/__main__.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 17:41:03.464606 pyplink-1.3.6/pyplink/tests/data/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       13 2018-05-02 17:13:27.000000 pyplink-1.3.6/pyplink/tests/data/test_data.bed
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      243 2018-05-02 17:13:27.000000 pyplink-1.3.6/pyplink/tests/data/test_data.bim
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       95 2018-05-02 17:13:27.000000 pyplink-1.3.6/pyplink/tests/data/test_data.fam
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      240 2018-05-02 17:13:28.000000 pyplink-1.3.6/pyplink/tests/data/test_data_with_dup.bim
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    45710 2023-05-19 17:37:51.000000 pyplink-1.3.6/pyplink/tests/test_pyplink.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       87 2023-05-19 17:41:03.000000 pyplink-1.3.6/pyplink/version.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 17:41:03.463606 pyplink-1.3.6/pyplink.egg-info/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      978 2023-05-19 17:41:03.000000 pyplink-1.3.6/pyplink.egg-info/PKG-INFO
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      705 2023-05-19 17:41:03.000000 pyplink-1.3.6/pyplink.egg-info/SOURCES.txt
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)        1 2023-05-19 17:41:03.000000 pyplink-1.3.6/pyplink.egg-info/dependency_links.txt
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)        1 2019-11-29 19:49:26.000000 pyplink-1.3.6/pyplink.egg-info/not-zip-safe
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       39 2023-05-19 17:41:03.000000 pyplink-1.3.6/pyplink.egg-info/requires.txt
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)        8 2023-05-19 17:41:03.000000 pyplink-1.3.6/pyplink.egg-info/top_level.txt
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       38 2023-05-19 17:41:03.464606 pyplink-1.3.6/setup.cfg
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     2950 2023-05-19 17:37:51.000000 pyplink-1.3.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyplink-1.3.5/LICENSE.txt` & `pyplink-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyplink-1.3.5/pyplink.egg-info/PKG-INFO` & `pyplink-1.3.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyplink
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python module to read binary Plink files.
 Home-page: https://github.com/lemieuxl/pyplink
 Author: Louis-Philippe Lemieux Perreault
 Author-email: louis-philippe.lemieux.perreault@statgen.org
 License: MIT
-Description-Content-Type: UNKNOWN
-Description: UNKNOWN
 Keywords: bioinformatics format Plink binary
-Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+License-File: LICENSE.txt
```

### Comparing `pyplink-1.3.5/README.mkd` & `pyplink-1.3.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-[![Build Status](https://travis-ci.org/lemieuxl/pyplink.svg?branch=master)](https://travis-ci.org/lemieuxl/pyplink)
-[![Coverage Status](https://coveralls.io/repos/lemieuxl/pyplink/badge.svg?branch=master&service=github)](https://coveralls.io/github/lemieuxl/pyplink?branch=master)
+[![Build Status](https://github.com/lemieuxl/pyplink/actions/workflows/python-tests.yml/badge.svg?branch=master)](https://github.com/lemieuxl/pyplink/actions)
 [![PyPI version](https://badge.fury.io/py/pyplink.svg)](http://badge.fury.io/py/pyplink)
 
-
 # pyplink - Module to process Plink's binary files
 
 `PyPlink` is a Python module to read and write Plink's binary files. Short
 documentation available at
 [https://lemieuxl.github.io/pyplink/](https://lemieuxl.github.io/pyplink/).
 
-
 ## Dependencies
 
 The tool requires a standard [Python](http://python.org/) installation (2.7 and
-3.3 or higher are supported) with the following modules:
+3.7 or higher are supported) with the following modules:
 
 1. [numpy](http://www.numpy.org/) version 1.8.2 or latest
 2. [pandas](http://pandas.pydata.org/) version 0.17.1 or latest
 3. [six](https://pythonhosted.org/six/) version 1.9.0 or latest
 
 The tool has been tested on *Linux* only, but should work on *MacOS* and
 *Windows* operating systems as well.
 
-
 ## Installation
 
 Using `pip`:
 
 ```bash
 pip install pyplink
 ```
@@ -41,15 +37,14 @@
 `-c http://statgen.org/...` can be omitted to update or install the package.
 To add the channel, perform the following command:
 
 ```bash
 conda config --add channels http://statgen.org/wp-content/uploads/Softwares/pyplink
 ```
 
-
 ### Updating
 
 To update the module using `pip`:
 
 ```bash
 pip install -U pyplink
 ```
@@ -60,27 +55,25 @@
 # If the channel has been configured (see above)
 conda update pyplink
 
 # Otherwise
 conda update pyplink -c http://statgen.org/wp-content/uploads/Softwares/pyplink
 ```
 
-
 ## Testing
 
 To test the module, just perform the following command:
 
 ```console
 $ python -m pyplink.tests
 .............................................
 ----------------------------------------------------------------------
 Ran 45 tests in 0.334s
 
 OK
 ```
 
-
 ## Example
 
 The following
 [notebook](http://nbviewer.ipython.org/github/lemieuxl/pyplink/blob/master/demo/PyPlink%20Demo.ipynb)
 contains a demonstration (for both Python 2 and 3) of the `PyPlink` module.
```

### Comparing `pyplink-1.3.5/pyplink/__init__.py` & `pyplink-1.3.6/pyplink/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplink-1.3.5/pyplink/tests/__init__.py` & `pyplink-1.3.6/pyplink/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Test module."""
 # This file is part of pyplink.
 #
 # The MIT License (MIT)
 #
 # Copyright (c) 2014 Louis-Philippe Lemieux Perreault
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyplink-1.3.5/pyplink/tests/test_pyplink.py` & `pyplink-1.3.6/pyplink/tests/test_pyplink.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""PyPlink test suite."""
 # This file is part of pyplink.
 #
 # The MIT License (MIT)
 #
 # Copyright (c) 2014 Louis-Philippe Lemieux Perreault
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyplink-1.3.5/pyplink/tests/__main__.py` & `pyplink-1.3.6/pyplink/tests/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Main script for tests."""
 # This file is part of pyplink.
 #
 # The MIT License (MIT)
 #
 # Copyright (c) 2014 Louis-Philippe Lemieux Perreault
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyplink-1.3.5/pyplink/pyplink.py` & `pyplink-1.3.6/pyplink/pyplink.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import os
 import logging
 from itertools import repeat
 from collections import Counter
 from io import UnsupportedOperation
 
 try:
-    from itertools import zip_longest as zip_longest
+    from itertools import zip_longest
 except ImportError:
     from itertools import izip_longest as zip_longest
 
 import numpy as np
 import pandas as pd
 
 from six.moves import range
@@ -239,15 +239,15 @@
         bim["i"] = bim.index
 
         # Checking for duplicated markers
         try:
             bim = bim.set_index("snp", verify_integrity=True)
             self._has_duplicated = False
 
-        except ValueError as e:
+        except ValueError:
             # Setting this flag to true
             self._has_duplicated = True
 
             # Finding the duplicated markers
             duplicated = bim.snp.duplicated(keep=False)
             duplicated_markers = bim.loc[duplicated, "snp"]
             duplicated_marker_counts = duplicated_markers.value_counts()
@@ -256,22 +256,22 @@
             # markers
             self._dup_markers = {
                 m: [] for m in duplicated_marker_counts.index
             }
 
             # Logging a warning
             logger.warning("Duplicated markers found")
-            for marker, count in duplicated_marker_counts.iteritems():
+            for marker, count in duplicated_marker_counts.items():
                 logger.warning("  - {}: {:,d} times".format(marker, count))
             logger.warning("Appending ':dupX' to the duplicated markers "
                            "according to their location in the BIM file")
 
             # Renaming the markers
             counter = Counter()
-            for i, marker in duplicated_markers.iteritems():
+            for i, marker in duplicated_markers.items():
                 counter[marker] += 1
                 new_name = "{}:dup{}".format(marker, counter[marker])
                 bim.loc[i, "snp"] = new_name
 
                 # Updating the dictionary containing the duplicated markers
                 self._dup_markers[marker].append(new_name)
 
@@ -334,35 +334,29 @@
         """Reads the FAM file."""
         # Reading the FAM file and setting the values
         fam = pd.read_csv(self.fam_filename, delim_whitespace=True,
                           names=["fid", "iid", "father", "mother", "gender",
                                  "status"],
                           dtype=dict(fid=str, iid=str, father=str, mother=str))
 
-        # Getting the byte and bit location of each samples
-        fam["byte"] = [
-            int(np.ceil((1 + 1) / 4.0)) - 1 for i in range(len(fam))
-        ]
-        fam["bit"] = [(i % 4) * 2 for i in range(len(fam))]
-
         # Saving the data in the object
         self._fam = fam
         self._nb_samples = self._fam.shape[0]
 
     def get_fam(self):
         """Returns the FAM file.
 
         Returns:
             pandas.DataFrame: The FAM file.
 
         """
         if self._mode != "r":
             raise UnsupportedOperation("not available in 'w' mode")
 
-        return self._fam.drop(["byte", "bit"], axis=1)
+        return self._fam.copy()
 
     def get_nb_samples(self):
         """Returns the number of samples.
 
         Returns:
             int: The number of samples in the dataset.
```

### Comparing `pyplink-1.3.5/setup.py` & `pyplink-1.3.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 #!/usr/bin/env python
+"""Setup."""
 
 # How to build source distribution
 #   - python setup.py sdist --format bztar
 #   - python setup.py sdist --format gztar
 #   - python setup.py sdist --format zip
 #   - python setup.py bdist_wheel --universal
 
 # How to build for conda (do both with 2.7 and 3.4)
-#   - bash conda_build.sh
+#   - cd conda_recipe
+#   - conda clean -ytps; conda build purge; conda build --python $VERSION .
+#   - cp $FILE ../conda_dist/linux-64
+#   - conda convert -p all ../conda_dist/linux-64/$FILE -o ../conda_dist
+#   - cd ../conda_dist && conda index *
 
 
 import os
 import sys
 from setuptools import setup
 
 
 MAJOR = 1
 MINOR = 3
-MICRO = 5
+MICRO = 6
 VERSION = "{}.{}.{}".format(MAJOR, MINOR, MICRO)
 
 
 def write_version_file(fn=None):
     if fn is None:
         fn = os.path.join(
             os.path.dirname(os.path.abspath(__file__)),
@@ -70,18 +75,19 @@
         install_requires=get_requirements(),
         classifiers=["Operating System :: POSIX :: Linux",
                      "Operating System :: MacOS :: MacOS X",
                      "Operating System :: Microsoft",
                      "Programming Language :: Python",
                      "Programming Language :: Python :: 2.7",
                      "Programming Language :: Python :: 3",
-                     "Programming Language :: Python :: 3.3",
-                     "Programming Language :: Python :: 3.4",
-                     "Programming Language :: Python :: 3.5",
-                     "Programming Language :: Python :: 3.6",
+                     "Programming Language :: Python :: 3.7",
+                     "Programming Language :: Python :: 3.8",
+                     "Programming Language :: Python :: 3.9",
+                     "Programming Language :: Python :: 3.10",
+                     "Programming Language :: Python :: 3.11",
                      "License :: OSI Approved :: MIT License",
                      "Topic :: Scientific/Engineering :: Bio-Informatics"],
         keywords="bioinformatics format Plink binary",
     )
 
     return
```

### Comparing `pyplink-1.3.5/PKG-INFO` & `pyplink-1.3.6/pyplink.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyplink
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python module to read binary Plink files.
 Home-page: https://github.com/lemieuxl/pyplink
 Author: Louis-Philippe Lemieux Perreault
 Author-email: louis-philippe.lemieux.perreault@statgen.org
 License: MIT
-Description-Content-Type: UNKNOWN
-Description: UNKNOWN
 Keywords: bioinformatics format Plink binary
-Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+License-File: LICENSE.txt
```

