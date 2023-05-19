# Comparing `tmp/dkist-inventory-0.9.3.tar.gz` & `tmp/dkist-inventory-0.9.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-inventory-0.9.3.tar", last modified: Thu Mar 10 22:21:24 2022, max compression
+gzip compressed data, was "dkist-inventory-0.9.4rc1.tar", last modified: Thu Sep  8 15:33:23 2022, max compression
```

## Comparing `dkist-inventory-0.9.3.tar` & `dkist-inventory-0.9.4rc1.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-10 22:21:24.110252 dkist-inventory-0.9.3/
--rw-rw-rw-   0 root         (0) root         (0)     3019 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      333 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      791 2022-03-10 22:21:24.110252 dkist-inventory-0.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      448 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      634 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-10 22:21:24.110252 dkist-inventory-0.9.3/dkist_inventory/
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/dkist_inventory/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8798 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/dkist_inventory/asdf_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    14709 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/dkist_inventory/inventory.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-10 22:21:24.110252 dkist-inventory-0.9.3/dkist_inventory/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/dkist_inventory/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2509 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/dkist_inventory/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3077 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/dkist_inventory/tests/test_asdf_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    11011 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/dkist_inventory/tests/test_inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/dkist_inventory/tests/test_transforms.py
--rw-rw-rw-   0 root         (0) root         (0)    19580 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/dkist_inventory/transforms.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2022-03-10 22:21:23.000000 dkist-inventory-0.9.3/dkist_inventory/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-10 22:21:24.110252 dkist-inventory-0.9.3/dkist_inventory.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      791 2022-03-10 22:21:23.000000 dkist-inventory-0.9.3/dkist_inventory.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      800 2022-03-10 22:21:24.000000 dkist-inventory-0.9.3/dkist_inventory.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-03-10 22:21:23.000000 dkist-inventory-0.9.3/dkist_inventory.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-03-10 22:21:23.000000 dkist-inventory-0.9.3/dkist_inventory.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      252 2022-03-10 22:21:23.000000 dkist-inventory-0.9.3/dkist_inventory.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       16 2022-03-10 22:21:23.000000 dkist-inventory-0.9.3/dkist_inventory.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-10 22:21:24.110252 dkist-inventory-0.9.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2309 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-10 22:21:24.110252 dkist-inventory-0.9.3/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2557 2022-03-10 22:21:24.110252 dkist-inventory-0.9.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      603 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2022-03-10 22:21:00.000000 dkist-inventory-0.9.3/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-09-08 15:33:23.618825 dkist-inventory-0.9.4rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     3019 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      333 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2022-09-08 15:33:23.618825 dkist-inventory-0.9.4rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      634 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      884 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-09-08 15:33:23.614825 dkist-inventory-0.9.4rc1/dkist_inventory/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8902 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/asdf_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/header_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)    15487 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/inventory.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-09-08 15:33:23.618825 dkist-inventory-0.9.4rc1/dkist_inventory/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3992 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3419 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/tests/test_asdf_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3192 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/tests/test_header_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)    11966 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/tests/test_inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6729 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/tests/test_transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    20891 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/dkist_inventory/transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2022-09-08 15:33:23.000000 dkist-inventory-0.9.4rc1/dkist_inventory/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-09-08 15:33:23.618825 dkist-inventory-0.9.4rc1/dkist_inventory.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2022-09-08 15:33:23.000000 dkist-inventory-0.9.4rc1/dkist_inventory.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      891 2022-09-08 15:33:23.000000 dkist-inventory-0.9.4rc1/dkist_inventory.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2022-09-08 15:33:23.000000 dkist-inventory-0.9.4rc1/dkist_inventory.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2022-09-08 15:33:23.000000 dkist-inventory-0.9.4rc1/dkist_inventory.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      317 2022-09-08 15:33:23.000000 dkist-inventory-0.9.4rc1/dkist_inventory.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2022-09-08 15:33:23.000000 dkist-inventory-0.9.4rc1/dkist_inventory.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-09-08 15:33:23.618825 dkist-inventory-0.9.4rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-09-08 15:33:23.618825 dkist-inventory-0.9.4rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2022-09-08 15:33:23.618825 dkist-inventory-0.9.4rc1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      603 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2022-09-08 15:32:59.000000 dkist-inventory-0.9.4rc1/tox.ini
```

### Comparing `dkist-inventory-0.9.3/.gitignore` & `dkist-inventory-0.9.4rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-inventory-0.9.3/bitbucket-pipelines.yml` & `dkist-inventory-0.9.4rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-inventory-0.9.3/dkist_inventory/asdf_generator.py` & `dkist-inventory-0.9.4rc1/dkist_inventory/asdf_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 from astropy.io.fits.hdu.base import BITPIX2DTYPE
 from dkist.dataset import Dataset, TiledDataset
 from dkist.io import FileManager
 from dkist.io.loaders import AstropyFITSLoader
 
 from dkist_inventory.inventory import (extract_inventory, group_mosaic_tiles,
                                        headers_from_filenames,
-                                       make_sorted_table, validate_headers)
+                                       make_sorted_table, validate_headers, table_from_headers)
 from dkist_inventory.transforms import TransformBuilder
 
 __all__ = ["references_from_filenames", "dataset_from_fits", "asdf_tree_from_filenames"]
 
 
 def references_from_filenames(filenames: npt.NDArray[Any],
-                              headers: npt.NDArray[Any],
+                              header_table: astropy.table.Table,
                               array_shape: Tuple[int, ...],
                               hdu_index: int = 0,
                               relative_to: os.PathLike = None) -> FileManager:
     """
     Given an array of paths to FITS files create a `dkist.io.FileManager`.
 
     Parameters
@@ -49,47 +49,40 @@
     Returns
     -------
     `dkist.io.FileManager`
         A container that represents a set of FITS files, and can generate a
         `dask.array.Array` from them.
     """
     filenames = np.asanyarray(filenames)
-    filepaths = np.empty(array_shape, dtype=object)
-    if filenames.size != filepaths.size:
-        raise ValueError(
-            f"An incorrect number of filenames ({filenames.size})"
-            f" supplied for array_shape ({array_shape})"
-        )
-
-    dtypes = []
-    shapes = []
-    for i, (filepath, head) in enumerate(zip(filenames.flat, headers.flat)):
-        dtypes.append(BITPIX2DTYPE[head["BITPIX"]])
-        shapes.append(tuple([int(head[f"NAXIS{a}"]) for a in range(head["NAXIS"], 0, -1)]))
-
-        # Convert paths to relative paths
-        relative_path = filepath
-        if relative_to:
-            relative_path = os.path.relpath(filepath, str(relative_to))
+    header_table = astropy.table.Table(header_table)
+    shaped_filepaths = filenames.reshape(array_shape, order='F')
+    shaped_headers = np.array(header_table).reshape(array_shape, order='F')
+
+    dtypes = np.vectorize(lambda x: BITPIX2DTYPE[x])(shaped_headers["BITPIX"])
+    shapes = shaped_headers[[f"NAXIS{a}" for a in range(header_table[0]["NAXIS"], 0, -1)]]
+
+    filepath_fixer = np.vectorize(lambda p: str(p))
+    if relative_to:
+        filepath_fixer = np.vectorize(lambda p: os.path.relpath(p, str(relative_to)))
 
-        filepaths.flat[i] = str(relative_path)  # type: ignore
+    shaped_filepaths = filepath_fixer(shaped_filepaths)
 
     # Validate all shapes and dtypes are consistent.
-    dtype = set(dtypes)
+    dtype = np.unique(dtypes)
     if len(dtype) != 1:
         raise ValueError("Not all the dtypes of these files are the same.")
     dtype = list(dtype)[0]
 
-    shape = set(shapes)
+    shape = np.unique(shapes)
     if len(shape) != 1:
         raise ValueError("Not all the shapes of these files are the same")
     shape = list(shape)[0]  #
 
-    return FileManager(
-        filepaths.tolist(), hdu_index, dtype, shape, loader=AstropyFITSLoader
+    return FileManager.from_parts(
+        shaped_filepaths.tolist(), hdu_index, dtype, shape, loader=AstropyFITSLoader
     )
 
 
 def dataset_object_from_filenames(sorted_table: astropy.table.Table,
                                   inventory: Mapping[str, Any],
                                   hdu: int,
                                   relative_to: os.PathLike = None) -> Dataset:
@@ -108,29 +101,28 @@
     hdu
         The HDU to read the headers from and reference the data to.
 
     relative_to
         The path to reference the FITS files to inside the asdf. If not
         specified will be local to the asdf (i.e. ``./``).
     """
-
     sorted_filenames = np.array(sorted_table["filenames"])
     sorted_headers = np.array(sorted_table["headers"])
     sorted_table.remove_columns(["headers", "filenames"])
 
     ds_wcs = TransformBuilder(sorted_table)
 
     # Get the array shape
     shape = tuple(
         (int(sorted_headers[0][f"DNAXIS{n}"]) for n in range(sorted_headers[0]["DNAXIS"],
                                                              sorted_headers[0]["DAAXES"], -1))
     )
     # References from filenames
     array_container = references_from_filenames(
-        sorted_filenames, sorted_headers, array_shape=shape, hdu_index=hdu, relative_to=relative_to
+        sorted_filenames, sorted_table, array_shape=shape, hdu_index=hdu, relative_to=relative_to
     )
 
     ds = Dataset(array_container._generate_array(),
                  ds_wcs.gwcs,
                  meta={'inventory': inventory, 'headers': sorted_table})
 
     ds._file_manager = array_container
@@ -175,14 +167,16 @@
 
     # In case filenames is a generator we cast to list.
     filenames = list(filenames)
 
     # headers is an iterator
     if not headers:
         headers = headers_from_filenames(filenames, hdu=hdu)
+    else:
+        headers = table_from_headers(headers)
 
     table_headers = make_sorted_table(headers, filenames)
 
     table_headers = group_mosaic_tiles(table_headers)
 
     if not inventory:
         inventory = extract_inventory(table_headers, **extra_inventory)
@@ -215,15 +209,15 @@
 
 
 def dataset_from_fits(path: Union[str, os.PathLike],
                       asdf_filename: str,
                       inventory: Mapping[str, str] = None,
                       hdu: int = 0,
                       relative_to: os.PathLike = None,
-                      **kwargs):
+                      **kwargs) -> pathlib.Path:
     """
     Given a path containing FITS files write an asdf file in the same path.
 
     Parameters
     ----------
     path
         The path to read the FITS files (with a `.fits` file extension) from
@@ -242,20 +236,27 @@
         The base path to use in the asdf references. By default this is the
         parent of ``path=``, it's unlikely you should need to change this from
         the default.
 
     kwargs
         Additional kwargs are passed to `asdf.AsdfFile.write_to`.
 
+    Returns
+    -------
+    asdf_filename
+        The path of the ASDF file written.
+
     """
     path = pathlib.Path(path).expanduser()
-    relative_to = relative_to or path.parent
+    relative_to = pathlib.Path(relative_to or path).expanduser()
 
     files = path.glob("*fits")
 
     tree = asdf_tree_from_filenames(
         list(files), inventory=inventory, hdu=hdu, relative_to=relative_to
     )
 
     with resources.path("dkist.io", "level_1_dataset_schema.yaml") as schema_path:
         with asdf.AsdfFile(tree, custom_schema=schema_path) as afile:
             afile.write_to(path / asdf_filename, **kwargs)
+
+    return path / asdf_filename
```

### Comparing `dkist-inventory-0.9.3/dkist_inventory/inventory.py` & `dkist-inventory-0.9.4rc1/dkist_inventory/inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 Helper functions for parsing files and processing headers.
 """
 import datetime
 import re
 from functools import partial
 from pathlib import Path
-from typing import Mapping, Any, Dict, List
+from typing import Any, Dict, List, Mapping
 
+import astropy.units as u
 import numpy as np
 import scipy.stats
 from astropy.io import fits
 from astropy.table import Table
-import astropy.units as u
+from dkist_fits_specifications.utils.formatter import reformat_spec214_header
 from ndcube import NDCube
 
 from dkist_inventory.transforms import TransformBuilder
 
 __all__ = ['generate_inventory_from_frame_inventory', 'headers_from_filenames']
 
 
@@ -44,15 +45,17 @@
         "_id",
         "bucket",
         "frameStatus",
         "objectKey",
         "createDate",
         "updateDate",
         "lostDate",
-        "headerHDU"
+        "headerHDU",
+        "COMMENT",
+        "",
     }
     fits_keys = set(json_headers[0].keys()).difference(known_non_fits_keys)
 
     def key_filter(keys, headers):
         return {x: headers[x] for x in keys if x in headers}
 
     non_fits_headers = list(map(partial(key_filter, known_non_fits_keys), json_headers))
@@ -69,19 +72,30 @@
     return filenames, fits_headers, extra_inventory
 
 
 def headers_from_filenames(filenames, hdu=0):
     """
     Generator to get the headers from filenames.
     """
-    return Table([dict(fits.getheader(fname, ext=hdu)) for fname in filenames])
+    # Here we filter out empty cards and COMMENT cards
+    filter_keys = ("", "COMMENT")
+    headers = [dict(fits.getheader(fname, ext=hdu)) for fname in filenames]
+    headers = [dict(filter(lambda x: x[0] not in filter_keys, h.items())) for h in headers]
+    return Table(headers)
 
 
 def table_from_headers(headers):
-    return Table(rows=headers, names=list(headers[0].keys()))
+    """
+    Convert a list of dicts into a table.
+
+    This also orders the columns of the table as if it were a 214 FITS file.
+    """
+    formatted_header = reformat_spec214_header(fits.Header(headers[0]))
+    ordered_keys = [key for key in formatted_header.keys() if key in headers[0].keys()]
+    return Table(rows=headers, names=ordered_keys)
 
 
 def validate_headers(table_headers):
     """
     Given a bunch of headers, validate that they form a coherent set.
 
     This function also adds the headers to a list as they are read from the
@@ -93,15 +107,15 @@
         An iterator of headers.
 
     Returns
     -------
     out_headers : `list`
         A list of headers.
     """
-    t = table_headers
+    t = table_headers.copy()
 
     # Let's do roughly the minimal amount of verification here for construction
     # of the WCS. Validation for inventory records is done independently.
 
     # For some keys all the values must be the same
     same_keys = ["NAXIS", "DNAXIS"]
     naxis_same_keys = ["NAXISn", "CTYPEn", "CUNITn"]
@@ -124,15 +138,18 @@
     return table_headers
 
 
 def make_sorted_table(headers, filenames):
     """
     Return an `astropy.table.Table` instance where the rows are correctly sorted.
     """
-    theaders = table_from_headers(headers)
+    if not isinstance(headers, Table):
+        raise TypeError("This function expects an Astropy Table.")
+
+    theaders = headers.copy()
     theaders["filenames"] = filenames
     theaders["headers"] = headers
     dataset_axes = headers[0]["DNAXIS"]
     array_axes = headers[0]["DAAXES"]
     keys = [f"DINDEX{k}" for k in range(dataset_axes, array_axes, -1)]
     t = np.array(theaders[keys])
     return theaders[np.argsort(t, order=keys)]
@@ -262,43 +279,43 @@
             results.append(_get_unique(headers[key], singular=True))
     return list(set(results))
 
 
 def _inventory_from_headers(headers: Table):
     inventory = {}
 
-    mode = partial(scipy.stats.mode, axis=None, nan_policy="raise")
+    mode = partial(scipy.stats.mode, keepdims=False, nan_policy="raise")
 
     # These keys might get updated by parsing the gwcs object.
     inventory["wavelengthMin"] = inventory["wavelengthMax"] = _get_unique(headers['LINEWAV'])[0]
 
     inventory["datasetId"] = _get_unique(headers["DSETID"], singular=True)
-    inventory["exposureTime"] = _get_number_apply(headers['TEXPOSUR'], mode).mode[0]
+    inventory["exposureTime"] = _get_number_apply(headers['XPOSURE'], mode).mode
     inventory["instrumentName"] = _get_unique(headers['INSTRUME'], singular=True)
     inventory["recipeId"] = int(_get_unique(headers['RECIPEID'], singular=True))
     inventory["recipeInstanceId"] = int(_get_unique(headers['RINSTID'], singular=True))
     inventory["recipeRunId"] = int(_get_unique(headers['RRUNID'], singular=True))
     inventory["targetTypes"] = list(map(str, _get_unique(headers['OBJECT'])))
     inventory["primaryProposalId"] = _get_unique(headers['PROP_ID'], singular=True)
     inventory["primaryExperimentId"] = _get_unique(headers['EXPER_ID'], singular=True)
-    inventory["dataset_size"] = _get_number_apply(headers['FRAMEVOL'], np.sum)
+    inventory["dataset_size"] = (_get_number_apply(headers['FRAMEVOL'], np.sum) * u.Mibyte).to_value(u.Gibyte)
     inventory["contributingExperimentIds"] = list(map(str, (_get_keys_matching(headers, r"EXPERID\d\d$") +
                                                             [_get_unique(headers["EXPER_ID"], singular=True)])))
     inventory["contributingProposalIds"] = list(map(str, (_get_keys_matching(headers, r"PROPID\d\d$") +
                                                           [_get_unique(headers["PROP_ID"], singular=True)])))
     friedval = np.nan
-    if 'FRIEDVAL' in headers.colnames:
-        friedval = _get_number_apply(headers['FRIEDVAL'], np.mean)
+    if 'ATMOS_R0' in headers.colnames:
+        friedval = _get_number_apply(headers['ATMOS_R0'], np.mean)
 
     inventory["qualityAverageFriedParameter"] = friedval
 
-    polacc = np.nan
-    if 'POL_ACC' in headers.colnames:
-        polacc = _get_number_apply(headers['POL_ACC'], np.mean)
-    inventory["qualityAveragePolarimetricAccuracy"] = polacc
+    polsens = np.nan
+    if 'POL_SENS' in headers.colnames:
+        polsens = _get_number_apply(headers['POL_SENS'], np.mean)
+    inventory["qualityAveragePolarimetricAccuracy"] = polsens
 
     return inventory
 
 
 def extract_inventory(headers: Table,
                       transform_builder: TransformBuilder = None,
                       **extra_inventory: Mapping[str, Any]) -> Mapping[str, Any]:
@@ -381,10 +398,11 @@
 
     Returns
     -------
     dataset_inventory
         The complete dataset inventory
     """
     filenames, fits_headers, extra_inventory = process_json_headers(bucket, json_headers)
-    table_headers = make_sorted_table(fits_headers, filenames)
+    table_headers = Table(fits_headers)
+    table_headers = make_sorted_table(table_headers, filenames)
 
     return extract_inventory(table_headers, **extra_inventory)
```

### Comparing `dkist-inventory-0.9.3/dkist_inventory/tests/test_asdf_generator.py` & `dkist-inventory-0.9.4rc1/dkist_inventory/tests/test_asdf_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,58 +12,71 @@
 from dkist_inventory.asdf_generator import (
     asdf_tree_from_filenames,
     dataset_from_fits,
     references_from_filenames,
 )
 from dkist_inventory.inventory import (
     headers_from_filenames,
-    table_from_headers,
     validate_headers,
     make_sorted_table,
     group_mosaic_tiles,
 )
 
 
 def test_array_container_shape(header_filenames):
-    vbi = "vbi-" in str(header_filenames[0])
-
     headers = headers_from_filenames(header_filenames, hdu=0)
     table_headers = make_sorted_table(headers, header_filenames)
     table_headers = group_mosaic_tiles(table_headers)
     if len(table_headers.groups) > 1:
         table_headers = table_headers.groups[0]
     sorted_headers = np.array(table_headers["headers"])
     sorted_filenames = np.array(table_headers["filenames"])
 
     # Get the array shape
     shape = tuple(
         (headers[0][f"DNAXIS{n}"] for n in range(headers[0]["DNAXIS"], headers[0]["DAAXES"], -1))
     )
     # References from filenames
     array_container = references_from_filenames(
-        sorted_filenames, sorted_headers, array_shape=shape, hdu_index=0, relative_to="."
+        sorted_filenames, table_headers, array_shape=shape, hdu_index=0, relative_to="."
     )
 
-    if vbi:
-        assert len(array_container.output_shape) == 3
-    else:
-        assert len(array_container.output_shape) == 5
     assert array_container.output_shape == array_container._generate_array().shape
 
 
 def test_asdf_tree(header_filenames):
     tree = asdf_tree_from_filenames(header_filenames)
     assert isinstance(tree, dict)
 
 
+def test_asdf_tree_with_headers_and_inventory_args():
+    # given
+    file_count = 5
+    from dkist_data_simulator.spec214.vbi import SimpleVBIDataset
+    import astropy.units as u
+    headers = []
+    file_names = []
+    for i, ds in enumerate(SimpleVBIDataset(
+            n_time=file_count,
+            time_delta=1,
+            linewave=550 * u.nm,
+            detector_shape=(10, 10),)):
+        h = ds.header()
+        h['BITPIX'] = 8
+        headers.append(h)
+        file_names.append(f"wibble_{i}.fits")
+    tree = asdf_tree_from_filenames(file_names, headers)
+    assert isinstance(tree, dict)
+
+
 def test_validator(header_filenames):
     headers = headers_from_filenames(header_filenames)
     headers[3]["NAXIS"] = 5
     with pytest.raises(ValueError) as excinfo:
-        validate_headers(table_from_headers(headers))
+        validate_headers(headers)
         assert "NAXIS" in str(excinfo)
 
 
 def test_references_from_filenames_shape_error(header_filenames):
     headers = headers_from_filenames(header_filenames, hdu=0)
     with pytest.raises(ValueError) as exc:
         references_from_filenames(header_filenames, headers, [2, 3])
@@ -74,15 +87,15 @@
 
 
 def test_references_from_filenames(header_filenames):
     headers = headers_from_filenames(header_filenames, hdu=0)
     base = os.path.split(header_filenames[0])[0]
     refs: FileManager = references_from_filenames(
         header_filenames,
-        np.array([dict(h) for h in headers], dtype=object),
+        headers,
         (len(header_filenames),),
         relative_to=base,
     )
 
     for ref in refs.filenames:
         assert base not in ref
```

### Comparing `dkist-inventory-0.9.3/dkist_inventory/tests/test_inventory.py` & `dkist-inventory-0.9.4rc1/dkist_inventory/tests/test_inventory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-from itertools import combinations
 import copy
 import datetime
-
-import numpy as np
-import pytest
+from itertools import combinations
 
 import astropy.units as u
 import gwcs.coordinate_frames as cf
+import numpy as np
+import pytest
 from astropy.table import Table
-
 from dkist_data_simulator.spec214.vbi import MosaicedVBIBlueDataset
-from dkist_inventory.inventory import (
-    _get_unique,
-    _inventory_from_headers,
-    _inventory_from_wcs,
-    extract_inventory,
-    process_json_headers,
-    generate_inventory_from_frame_inventory
-)
+from dkist_data_simulator.spec214.vtf import SimpleVTFDataset
+from dkist_inventory.inventory import (_get_unique, _inventory_from_headers,
+                                       _inventory_from_wcs, extract_inventory,
+                                       generate_inventory_from_frame_inventory,
+                                       headers_from_filenames,
+                                       process_json_headers)
+from dkist_inventory.transforms import TransformBuilder
 
 
 @pytest.fixture
 def headers_inventory_214():
     """A minimal collection of headers to test inventory creation."""  # noqa
     return Table(
         {
             "LINEWAV": [550, 550, 550],
-            "TEXPOSUR": [10, 20, 30],
+            "XPOSURE": [10, 20, 30],
             "INSTRUME": ["VBI", "VBI", "VBI"],
-            "FRIEDVAL": [1, 2, 3],
-            "POL_ACC": [500, 500, 500],
+            "ATMOS_R0": [1, 2, 3],
+            "POL_SENS": [500, 500, 500],
             "RECIPEID": [10, 10, 10],
             "RINSTID": [20, 20, 20],
             "RRUNID": [30, 30, 30],
             "OBJECT": ["A", "B", "C"],
             "FRAMEVOL": [100, 120, 130],
             "EXPER_ID": ["00", "00", "00"],
             "EXPERID01": ["10", "10", "10"],
@@ -253,21 +250,38 @@
     assert inv['hasTemporalAxis'] == True
     assert inv['averageDatasetSpectralSampling'] is None
     assert inv['averageDatasetSpatialSampling'] == 1
     assert inv['averageDatasetTemporalSampling'] == 0.4
 
 
 @pytest.fixture(scope="session")
-def vbi_mosaic_headers():
-    ds_gen = MosaicedVBIBlueDataset(n_time=2, time_delta=10, linewave=400 * u.nm)
+def vbi_mosaic_headers(dataset):
+    ds_gen = dataset("vbi-mosaic")
     return ds_gen.generate_headers()
 
 
 def test_vbi_mosaic(vbi_mosaic_headers):
     json_headers = add_mongo_fields_to_header(vbi_mosaic_headers)
     inventory = generate_inventory_from_frame_inventory("data", json_headers)
     # TODO: This test asserts the bounding box code gives the same answer it
     # did when it was first written With a known dataset we should check this
     # matches reality by plotting these coordinates
     np.testing.assert_allclose(inventory["boundingBox"],
-                               ((0.0019644450431604552, -83.12297632393219),
-                                (1295999.9949319072, 36.722166192701394)))
+                               [[1.295916e+06, -8.312298e+01],
+                                [1.295991e+06, -7.981833e+00]], rtol=1e-5)
+
+
+def test_stokes_shape(simulated_dataset):
+    dataset_path = simulated_dataset("vtf")
+    headers = headers_from_filenames(dataset_path.glob("*"))
+    wcs = TransformBuilder(headers).gwcs
+
+    acm = np.array([[ True,  True, False, False, False],  # noqa
+                    [ True,  True, False, False, False],  # noqa
+                    [False, False,  True, False, False],  # noqa
+                    [False, False,  True,  True, False],  # noqa
+                    [False, False, False, False,  True]])  # noqa
+
+    assert acm.shape == wcs.axis_correlation_matrix.shape
+    assert np.allclose(wcs.axis_correlation_matrix, acm)
+    inventory = _inventory_from_wcs(wcs)
+    assert inventory["stokesParameters"] == ["I", "Q", "U", "V"]
```

### Comparing `dkist-inventory-0.9.3/dkist_inventory/tests/test_transforms.py` & `dkist-inventory-0.9.4rc1/dkist_inventory/tests/test_transforms.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,77 +2,113 @@
 import pytest
 
 import astropy.units as u
 import gwcs.coordinate_frames as cf
 from astropy.io import fits
 from astropy.modeling import Model, models
 from astropy.time import Time
+from astropy.table import Table
 
 from dkist_inventory.transforms import (
     linear_spectral_model,
     linear_time_model,
     spatial_model_from_header,
     spectral_model_from_framewave,
     time_model_from_date_obs,
+    TransformBuilder
 )
 
 
 @pytest.fixture
 def wcs(transform_builder):
     return transform_builder.gwcs
 
 
-def test_reset(transform_builder):
-    transform_builder._i = 2
-    transform_builder.reset()
-    assert transform_builder._i == 0
+@pytest.fixture
+def non_varying_wcs(non_varying_transform_builder):
+    return non_varying_transform_builder.gwcs
 
 
 def test_transform(transform_builder):
     assert isinstance(transform_builder.transform, Model)
 
 
 def test_frames(transform_builder):
     frames = transform_builder.frames
     assert all([isinstance(frame, cf.CoordinateFrame) for frame in frames])
 
 
-def test_input_name_ordering(wcs):
+def test_input_name_ordering(transform_builder):
     # Check the ordering of the input and output frames
-    allowed_pixel_names = (
-        ("spatial x", "spatial y", "scan position", "scan repeat number", "stokes"),
-        ("wavelength", "slit position", "raster position", "scan number", "stokes"),
-        ("spatial x", "spatial y", "frame number"),
-    )
-    assert wcs.input_frame.axes_names in allowed_pixel_names
-
-
-def test_output_name_ordering(wcs):
-    allowed_world_names = (
-        ("helioprojective longitude", "helioprojective latitude", "wavelength", "time", "stokes"),
-        ("wavelength", "helioprojective latitude", "helioprojective longitude", "time", "stokes"),
-        ("helioprojective longitude", "helioprojective latitude", "time"),
-    )
-    assert wcs.output_frame.axes_names in allowed_world_names
-
-
-def test_output_frames(wcs):
-    allowed_frame_orders = (
-        (cf.CelestialFrame, cf.SpectralFrame, cf.TemporalFrame, cf.StokesFrame),
-        (cf.SpectralFrame, cf.CelestialFrame, cf.TemporalFrame, cf.StokesFrame),
-        (cf.CelestialFrame, cf.TemporalFrame),
-    )
+    wcs = transform_builder.gwcs
+    allowed_pixel_names = {
+        "VISP": (
+            ("slit position", "wavelength", "raster position", "scan number"),
+            ("slit position", "wavelength", "raster position", "scan number", "stokes"),
+            ("slit position", "wavelength", "raster position"),
+            ("slit position", "wavelength", "raster position", "stokes"),
+        ),
+        "VTF": (
+            ("spatial x", "spatial y", "scan position", "scan repeat number", "stokes"),
+            ("spatial x", "spatial y", "scan position", "scan repeat number"),
+            ("spatial x", "spatial y", "scan position"),
+        ),
+        "VBI": (
+            ("spatial x", "spatial y", "frame number"),
+        ),
+
+    }
+    assert wcs.input_frame.axes_names in allowed_pixel_names[transform_builder.header["INSTRUME"]]
+
+
+def test_output_name_ordering(transform_builder):
+    wcs = transform_builder.gwcs
+
+    allowed_world_names = {
+        "VISP": (
+            # These are split to correspond to the order of the `_values`
+            # numbers not the high level objects.
+            ("helioprojective latitude", "wavelength", "helioprojective longitude", "time"),
+            ("helioprojective latitude", "wavelength", "helioprojective longitude", "time", "stokes"),
+        ),
+        "VTF": (
+            ("helioprojective longitude", "helioprojective latitude", "wavelength", "time", "stokes"),
+            ("helioprojective longitude", "helioprojective latitude", "wavelength", "time"),
+        ),
+        "VBI": (
+            ("helioprojective longitude", "helioprojective latitude", "time"),
+        ),
+    }
+
+    assert wcs.output_frame.axes_names in allowed_world_names[transform_builder.header["INSTRUME"]]
+
+
+def test_output_frames(transform_builder):
+    wcs = transform_builder.gwcs
+    allowed_frame_orders = {
+        "VISP": (
+            (cf.CelestialFrame, cf.SpectralFrame, cf.TemporalFrame, cf.StokesFrame),
+            (cf.CelestialFrame, cf.SpectralFrame, cf.TemporalFrame),
+        ),
+        "VTF": (
+            (cf.CelestialFrame, cf.SpectralFrame, cf.TemporalFrame, cf.StokesFrame),
+            (cf.CelestialFrame, cf.SpectralFrame, cf.TemporalFrame),
+        ),
+        "VBI": (
+            (cf.CelestialFrame, cf.TemporalFrame),
+        ),
+    }
     types = tuple((type(frame) for frame in wcs.output_frame.frames))
-    assert types in allowed_frame_orders
+    assert types in allowed_frame_orders[transform_builder.header["INSTRUME"]]
 
 
-def test_transform_models(wcs):
+def test_transform_models(non_varying_wcs):
     # Test that there is one lookup table and two linear models for both the
     # wcses
-    sms = wcs.forward_transform._leaflist
+    sms = non_varying_wcs.forward_transform._leaflist
     smtypes = [type(m) for m in sms]
     if len(smtypes) == 4:  # VTF and VISP
         assert sum(mt is models.Linear1D for mt in smtypes) == 2
         assert sum(mt is models.Tabular1D for mt in smtypes) == 1
     if len(smtypes) == 2:  # VBI
         assert sum(mt is models.Linear1D for mt in smtypes) == 1
 
@@ -82,49 +118,45 @@
 
 
 def test_spatial_model(header_filenames):
     sampling, spatial = spatial_model_from_header(first_header(header_filenames))
     assert isinstance(spatial, Model)
 
 
-def test_spatial_model_fail(header_filenames):
-    header = first_header(header_filenames)
-    header["CTYPE2"] = "WAVE"
-    with pytest.raises(ValueError):
-        spatial_model_from_header(header)
-
-
 def test_linear_spectral():
     lin = linear_spectral_model(10 * u.nm, 0 * u.nm)
     assert isinstance(lin, models.Linear1D)
     assert u.allclose(lin.slope, 10 * u.nm / u.pix)
     assert u.allclose(lin.intercept, 0 * u.nm)
 
 
 def test_linear_time():
-    lin = linear_time_model(10*u.s)
+    lin = linear_time_model(10 * u.s)
     assert isinstance(lin, models.Linear1D)
     assert u.allclose(lin.slope, 10 * u.s / u.pix)
     assert u.allclose(lin.intercept, 0 * u.s)
 
 
-def test_time_from_dateobs(header_filenames):
+@pytest.mark.parametrize("dataset_name", ["vbi"])
+def test_time_from_dateobs(dataset_name, simulated_dataset):
+    directory = simulated_dataset(dataset_name)
+    header_filenames = directory.glob("*")
     date_obs = [fits.getheader(f)["DATE-BEG"] for f in header_filenames]
     date_obs.sort()
     delta = Time(date_obs[1]) - Time(date_obs[0])
-    sampling, time = time_model_from_date_obs(date_obs)
+    sampling, time = time_model_from_date_obs(np.array(date_obs))
     assert isinstance(time, models.Linear1D)
     np.testing.assert_allclose(time.slope, delta.to(u.s) / (1 * u.pix))
 
 
 def test_time_from_dateobs_lookup(header_filenames):
     date_obs = [fits.getheader(f)["DATE-BEG"] for f in header_filenames]
     date_obs[3] = (Time(date_obs[3]) + 10 * u.s).isot
     deltas = Time(date_obs) - Time(date_obs[0])
-    sampling, time = time_model_from_date_obs(date_obs)
+    sampling, time = time_model_from_date_obs(np.array(date_obs))
     assert isinstance(time, models.Tabular1D)
     assert (time.lookup_table == deltas.to(u.s)).all()
     np.testing.assert_allclose(time.lookup_table, deltas.to(u.s))
 
 
 def test_spectral_framewave(header_filenames):
     head = first_header(header_filenames)
@@ -144,10 +176,18 @@
 
 
 def test_time_varying_vbi_wcs(vbi_time_varying_transform_builder):
     if not hasattr(Model, "_calculate_separability_matrix"):
         pytest.skip()
     wcs = vbi_time_varying_transform_builder.gwcs
     assert np.allclose(wcs.axis_correlation_matrix,
-                       np.array([[True,  True,  True],
-                                 [True,  True,  True],
+                       np.array([[True,  True,  True],  # noqa
+                                 [True,  True,  True],  # noqa
                                  [False, False, True]]))
+
+
+def test_non_time_varying_vtf(dataset):
+    ds = dataset("vtf")
+    headers = Table(ds.generate_headers())
+
+    wcs = TransformBuilder(headers).gwcs
+    assert wcs.forward_transform.n_inputs == 5
```

### Comparing `dkist-inventory-0.9.3/dkist_inventory/transforms.py` & `dkist-inventory-0.9.4rc1/dkist_inventory/transforms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """
 Functionality relating to creating gWCS frames and Astropy models from SPEC 214 headers.
 """
 import re
-from collections import defaultdict
 from functools import partial
 from itertools import product
 
 import astropy.modeling.models as m
 import astropy.table
 import astropy.units as u
 import gwcs
 import gwcs.coordinate_frames as cf
 import numpy as np
 from astropy.modeling import CompoundModel
 from astropy.time import Time
-from dkist.wcs.models import (VaryingCelestialTransform,
-                              generate_celestial_transform, CoupledCompoundModel)
+from dkist.wcs.models import (CoupledCompoundModel,
+                              VaryingCelestialTransformSlit,
+                              VaryingCelestialTransformSlit2D,
+                              generate_celestial_transform,
+                              varying_celestial_transform_from_tables)
 from sunpy.coordinates import Helioprojective
 
+from dkist_inventory.header_parsing import HeaderParser
+
 __all__ = [
     "TransformBuilder",
     "spectral_model_from_framewave",
     "time_model_from_date_obs",
     "generate_lookup_table",
     "linear_time_model",
     "linear_spectral_model",
@@ -90,75 +94,75 @@
 
     if not lonpole:
         raise ValueError(f"LONPOLE not specified and not known for projection {latproj}")
 
     projections = {"TAN": m.Pix2Sky_TAN()}
 
     return (
-        np.mean(cdelt).to_value(u.arcsec/u.pix),
+        np.mean(cdelt).to_value(u.arcsec / u.pix),
         generate_celestial_transform(crpix, cdelt, pc, crval,
                                      lon_pole=lonpole, projection=projections[latproj])
     )
 
 
-def varying_spatial_model_from_headers(headers: astropy.table.Table, varying_axes: dict[str, list[int]]):
+def varying_spatial_model_from_headers(axes: list[int], parser: HeaderParser):
     """
     Generate a varying celestial model from a set of headers.
     """
-    if "pc" in varying_axes and "crval" in varying_axes:
-        if varying_axes["pc"] != varying_axes["crval"]:
-            raise ValueError(
-                "Both the pointing and the rotation vary over different"
-                " dimensions of the dataset. I don't know what to do here."
-            )
-        vaxes = varying_axes["crval"]
-    elif "crval" in varying_axes:
-        vaxes = varying_axes["crval"]
-    elif "pc" in varying_axes:
-        vaxes = varying_axes["pc"]
-    else:
-        raise ValueError("What is this varying_axes dict you have given me?!")
+    header = dict(parser.header)
+    varying_axes = parser.varying_spatial_daxes
+    vaxes = parser.compute_varying_axes_numbers(varying_axes)
 
-    header = dict(headers[0])
     latind, lonind = identify_spatial_axes(header)
     cunit1, cunit2 = u.Unit(header[f"CUNIT{lonind}"]), u.Unit(header[f"CUNIT{latind}"])
     crpix = (header[f"CRPIX{lonind}"], header[f"CRPIX{latind}"]) * u.pix
     cdelt = u.Quantity([
         header[f"CDELT{lonind}"] * (cunit1 / u.pix),
         header[f"CDELT{latind}"] * (cunit2 / u.pix),
     ])
 
     # Extract tables
+    varying_header_array = parser.header_array[parser.slice_for_dataset_array_axes(*vaxes, indexing="fits")]
     varying_shape = [header[f"DNAXIS{d}"] for d in vaxes]
 
     if "crval" in varying_axes:
-        crval_table = headers[[f"CRVAL{i}" for i in (lonind, latind)]]
+        crval_table = varying_header_array[[f"CRVAL{i}" for i in (lonind, latind)]]
         # Coerce the astropy table to a regular float numpy array
-        crval_table = crval_table.as_array().view((float, len(crval_table.columns)))
+        crval_table = np.array(crval_table.tolist())
         crval_table = crval_table.reshape(varying_shape + [2])
         crval_table = crval_table << cunit1
     else:
-        crval_table = u.Quantity(header[f"CRVAL{lonind}"] * cunit1, header[f"CRVAL{latind}"] * cunit2)
+        crval_table = u.Quantity([header[f"CRVAL{lonind}"] * cunit1, header[f"CRVAL{latind}"] * cunit2])
 
     if "pc" in varying_axes:
-        pc_table = headers[[f"PC{i}_{j}" for i, j in product(*[(lonind, latind)]*2)]]
+        pc_table = varying_header_array[[f"PC{i}_{j}" for i, j in product(*[(lonind, latind)] * 2)]]
         # Coerce the astropy table to a regular float numpy array
-        pc_table = pc_table.as_array().view((float, len(pc_table.columns)))
+        pc_table = np.array(pc_table.tolist())
         pc_table = pc_table.reshape(varying_shape + [2, 2])
         pc_table = pc_table << cunit1
     else:
         pc_table = np.array([
             [header[f"PC{lonind}_{lonind}"], header[f"PC{lonind}_{latind}"]],
             [header[f"PC{latind}_{lonind}"], header[f"PC{latind}_{latind}"]],
         ]) * cunit1
 
-    vct = VaryingCelestialTransform(cdelt=cdelt, crpix=crpix, crval_table=crval_table, pc_table=pc_table)
+    # Which daxes have DTYPE == "SPATIAL" (+1 to shift to FITS)
+    primary_spatial_axes = (np.array(parser.axes_types) == "SPATIAL").nonzero()[0] + 1
+    # If any axes the pointing is varying across have a primary type of SPATIAL
+    # then we are a slit spectrograph where the pointing is changing with the
+    # raster dimension (hopefully).
+    slit = False
+    if (np.array(vaxes)[:, None] == primary_spatial_axes).any():
+        slit = True
+    vct = varying_celestial_transform_from_tables(cdelt=cdelt, crpix=crpix,
+                                                  crval_table=crval_table,
+                                                  pc_table=pc_table,
+                                                  slit=slit)
 
-    # TODO: estimate the spatial sampling somehow?
-    return 0, vct
+    return np.mean(cdelt).to_value(u.arcsec / u.pix), vct
 
 
 @u.quantity_input
 def linear_spectral_model(spectral_width: u.nm, reference_val: u.nm):
     """
     Linear model in a spectral dimension. The reference pixel is always 0.
     """
@@ -175,40 +179,46 @@
     return m.Linear1D(slope=cadence / (1 * u.pix), intercept=reference_val)
 
 
 def generate_lookup_table(lookup_table, interpolation="linear", points_unit=u.pix, **kwargs):
     if not isinstance(lookup_table, u.Quantity):
         raise TypeError("lookup_table must be a Quantity.")
 
-    # The integer location is at the centre of the pixel.
-    points = (np.arange(lookup_table.size) - 0) * points_unit
-
     kwargs = {"bounds_error": False, "fill_value": np.nan, "method": interpolation, **kwargs}
 
-    return m.Tabular1D(points, lookup_table, **kwargs)
+    points = tuple(np.arange(na) * u.pix for na in lookup_table.shape)
+    if lookup_table.ndim == 1:
+        # The integer location is at the centre of the pixel.
+        return m.Tabular1D(points, lookup_table, **kwargs)
+    elif lookup_table.ndim == 2:
+        # TODO: This doesn't support inverse
+        return m.Tabular2D(points, lookup_table, **kwargs)
+    else:
+        raise ValueError("Lookup tables with >2 dimensions are not supported.")
 
 
 def time_model_from_date_obs(date_obs, date_beg=None):
     """
     Return a time model that best fits a list of dateobs's.
     """
     if not date_beg:
-        date_beg = date_obs[0]
-    date_obs = Time(date_obs)
-    date_beg = Time(date_beg)
+        date_beg = date_obs.flat[0]
 
-    deltas = date_obs - date_beg
+    # I assume we need the .T here to change from fortran to C order which time expects
+    deltas = Time(date_obs.T.flat) - Time(date_beg.T.flat)
 
     # Work out if we have a uniform delta (i.e. a linear model)
     ddelta = deltas.to(u.s)[1:] - deltas.to(u.s)[:-1]
 
+    deltas = deltas.reshape(date_obs.shape, order="F")
+
     # If the length of the axis is one, then return a very simple model
     if ddelta.size == 0:
         raise ValueError("Why do you have a temporal axis in the DTYPEn keys if you only have a len 1 time axis?")
-    elif u.allclose(ddelta[0], ddelta):
+    elif u.allclose(ddelta[0], ddelta, atol=10*u.us) and deltas.ndim == 1:
         slope = ddelta[0]
         intercept = 0 * u.s
         return slope.to_value(u.s), linear_time_model(cadence=slope, reference_val=intercept)
     else:
         print(f"Creating tabular temporal axis. ddeltas: {ddelta}")
         return np.mean(deltas).to_value(u.s), generate_lookup_table(deltas.to(u.s))
 
@@ -237,64 +247,54 @@
 class TransformBuilder:
     """
     This class builds compound models and frames in order when given axes types.
     """
     def __init__(self, headers: astropy.table.Table):
         if not isinstance(headers, astropy.table.Table):
             raise TypeError("headers should be an astropy table")
-        self.header = dict(headers[0])
 
-        # Reshape the headers to match the Dataset shape, so we can extract headers along various axes.
-        shape = tuple(
-            self.header[f"DNAXIS{n}"]
-            for n in range(self.header["DNAXIS"], self.header["DAAXES"], -1)
-        )
-        arr_headers = np.empty(shape, dtype=object)
-        for i in range(arr_headers.size):
-            arr_headers.flat[i] = dict(headers[i])
-
-        self.pixel_shape = tuple(
-            self.header[f"DNAXIS{n}"] for n in range(1, self.header["DNAXIS"] + 1)
-        )
-
-        self.headers = arr_headers
-        self.header_table = headers
-        self.reset()
-        self._build()
+        self.header = dict(headers[0])
+        self.headers = headers
+        self.parser = HeaderParser(self.headers)
 
         self.spectral_sampling = None
         self.spatial_sampling = None
         self.temporal_sampling = None
 
+        # This must be last
+        # Build the components of the transform
+        self._build()
+
     @property
     def pixel_frame(self):
         """
         A `gwcs.coordinate_frames.CoordinateFrame` object describing the pixel frame.
         """
+        DNAXIS = self.header["DNAXIS"]
         return cf.CoordinateFrame(
-            naxes=self.header["DNAXIS"],
-            axes_type=self.axes_types,
-            axes_order=range(self.header["DNAXIS"]),
-            unit=[u.pixel] * self.header["DNAXIS"],
-            axes_names=[self.header[f"DPNAME{n}"] for n in range(1, self.header["DNAXIS"] + 1)],
+            naxes=DNAXIS,
+            axes_type=["PIXEL"] * DNAXIS,
+            axes_order=range(DNAXIS),
+            unit=[u.pixel] * DNAXIS,
+            axes_names=[self.header[f"DPNAME{n}"] for n in range(1, DNAXIS + 1)],
             name="pixel",
         )
 
     @property
     def gwcs(self):
         """
         `gwcs.WCS` object representing these headers.
         """
         world_frame = cf.CompositeFrame(self.frames)
 
         out_wcs = gwcs.WCS(
             forward_transform=self.transform, input_frame=self.pixel_frame, output_frame=world_frame
         )
-        out_wcs.pixel_shape = self.pixel_shape
-        out_wcs.array_shape = self.pixel_shape[::-1]
+        out_wcs.pixel_shape = self.parser.dataset_shape
+        out_wcs.array_shape = self.parser.dataset_shape[::-1]
 
         return out_wcs
 
     @property
     def frames(self):
         """
         The coordinate frames, in Python order.
@@ -302,251 +302,236 @@
         return self._frames
 
     @property
     def transform(self):
         """
         Return the compound model.
         """
-        # self._transforms is a tuple of (model, callable(left)).
+        # self._transforms is a tuple of (pixel_axes, model, callable(right)).
         # The callable returns a CompoundModel instance when the right hand
         # side of the operator is passed.
         # We iterate backwards through the models generating the model for the
         # right hand side of the next step up the tree (i.e. from the inner
         # most operator to the outermost). So we start with the last model
         # instance (ignoring the callable), then pass that model to the next
         # callable as the right hand side, and continue to work our way back up
         # the tree.
-        right, _ = self._transforms[-1]
-        for _, func in self._transforms[:-1][::-1]:
+        axes, right, _ = self._transforms[-1]
+        pixel_inputs = [*axes]
+        for axes, _, func in self._transforms[:-1][::-1]:
+            pixel_inputs = [*axes, *pixel_inputs]
             right = func(right=right)
+
+        # If the number of inputs to the generated transform doesn't match the
+        # number of pixel dimensions in the dataset then we construct a mapping
+        # to share some pixel inputs between multiple models
+        expected_inputs = len(self.parser.dataset_shape)
+        if right.n_inputs != expected_inputs:
+            mapping = m.Mapping(pixel_inputs)
+            right = mapping | right
+
+        # If the number of inputs *still* doesn't match something has gone very wrong.
+        if right.n_inputs != expected_inputs:
+            raise ValueError(
+                f"The transform that has been constructed has {right.n_inputs} inputs "
+                f"which does not match the expected number ({expected_inputs}) of pixel inputs."
+            )  # pragma: no cover
+
+        # If any of the world axes are in the wrong order (i.e. spatial axes are split)
+        # then we need to reorder the outputs to match.
+        all_known_world_indicies = np.concatenate(list(self.world_type_index_map.values()),
+                                                  axis=None)
+        if (all_known_world_indicies != np.arange(len(all_known_world_indicies))).any():
+            right = right | m.Mapping(all_known_world_indicies.tolist())
+
         return right
 
     """
     Internal Stuff
     """
 
     @staticmethod
     def _compound_model_partial(left, op="&"):
         return partial(CompoundModel, left=left, op=op)
 
     def _build(self):
         """
         Build the state of the thing.
         """
-        type_map = {
+        make_map = {
             "STOKES": self.make_stokes,
             "TEMPORAL": self.make_temporal,
             "SPECTRAL": self.make_spectral,
             "SPATIAL": self.make_spatial,
         }
 
-        xx = 0
-        while self._i < self.header["DNAXIS"]:  # < because FITS is i+1
-            atype = self.axes_types[self._i]
-            type_map[atype]()
-            xx += 1
-            if xx > 100:
-                raise ValueError("Infinite loop in header parsing")  # pragma: no cover
-
-    @property
-    def axes_types(self):
-        """
-        The list of DTYPEn for the first header.
-        """
-        return [self.header[f"DTYPE{n}"] for n in range(1, self.header["DNAXIS"] + 1)]
+        # This is the number of world coordinates allowed for each physical type
+        type_world_lengths = {
+            "STOKES": 1,
+            "TEMPORAL": 1,
+            "SPECTRAL": 1,
+            "SPATIAL": 2,
+        }
 
-    def reset(self):
-        """
-        Reset the builder.
-        """
-        self._i = 0
         self._frames = []
         self._transforms = []
 
-    @property
-    def n(self):
-        """
-        The FITS index of the current dimension.
-        """
-        return self._n(self._i)
-
-    def _n(self, i):
-        """
-        Convert a Python index ``i`` to a FITS order index for keywords ``n``.
-        """
-        # return range(self.header['DNAXIS'], 0, -1)[i]
-        return i + 1
-
-    @property
-    def slice_for_n(self):
-        i = self._i - self.header["DAAXES"]
-        naxes = self.header["DEAXES"]
-        ss = [0] * naxes
-        ss[i] = slice(None)
-        return ss[::-1]
-
-    @property
-    def slice_headers(self):
-        return self.headers[tuple(self.slice_for_n)]
+        # type_map is the mapping of world type to pixel axes.
+        # i.e. the pixel axes along which a given world coordinate varies.
+        type_map = self.parser.pixel_axis_type_map
+
+        # Figure out what world indices map to what type
+        world_type_index_map = {}
+        for pixel_type, pixel_indicies in type_map.items():
+            pixel_indicies = np.array(pixel_indicies)
+            all_known_world_indicies = np.array([])
+            if world_type_index_map:
+                all_known_world_indicies = np.concatenate(list(world_type_index_map.values()),
+                                                          axis=None)
+
+            # Make sure that we truncate any many pixel to fewer world transforms
+            # For example this applies to 3 pixel spatial and 2 pixel temporal
+            if len(pixel_indicies) > type_world_lengths[pixel_type]:
+                pixel_indicies = pixel_indicies[0:type_world_lengths[pixel_type]]
+
+            # Compute any overlap with the known list of world dimensions and
+            # shift the output so there is no overlap
+            world_offset = 0
+            duplicate_indicies = np.intersect1d(all_known_world_indicies, pixel_indicies)
+            if duplicate_indicies.any():
+                world_offset = duplicate_indicies.size
+
+            world_type_index_map[pixel_type] = (np.array(pixel_indicies) + world_offset).tolist()
+
+        self.world_type_index_map = world_type_index_map
+
+        for dtype, axes in type_map.items():
+            frame, transform_pair = make_map[dtype](axes)
+            self._frames.append(frame)
+            self._transforms.append((axes, *transform_pair))
 
     def get_units(self, *iargs):
         """
         Get zee units
         """
-        u = [self.header.get(f"DUNIT{self._n(i)}", None) for i in iargs]
-
+        u = [self.header.get(f"DUNIT{i + 1}", None) for i in iargs]
         return u
 
-    def make_stokes(self):
+    def make_stokes(self, axes):
         """
         Add a stokes axes to the builder.
         """
-        name = self.header[f"DWNAME{self.n}"]
-        self._frames.append(cf.StokesFrame(axes_order=(self._i,), name=name))
+        if not len(axes) == 1:
+            raise ValueError("There can only be one STOKES axis.")
+        i = axes[0]
+
+        name = self.header[f"DWNAME{i + 1}"]
+        frame = cf.StokesFrame(axes_order=self.world_type_index_map["STOKES"], name=name)
         transform = generate_lookup_table([0, 1, 2, 3] * u.one, interpolation="nearest")
-        self._transforms.append((
-            transform,
-            self._compound_model_partial(left=transform))
-        )
-        self._i += 1
 
-    def make_temporal(self):
+        return frame, (transform, self._compound_model_partial(left=transform))
+
+    def make_spectral(self, axes):
         """
-        Add a temporal axes to the builder.
+        Decide how to make a spectral axes.
         """
-
-        name = self.header[f"DWNAME{self.n}"]
-        self._frames.append(
-            cf.TemporalFrame(
-                axes_order=(self._i,),
-                name=name,
-                axes_names=(name,),
-                unit=self.get_units(self._i),
-                reference_frame=Time(self.header["DATE-BEG"]),
-            )
+        if not len(axes) == 1:
+            raise ValueError("There can only be one SPECTRAL axis.")
+        i = axes[0]
+        n = i + 1
+        name = self.header[f"DWNAME{n}"]
+        frame = cf.SpectralFrame(
+            axes_order=self.world_type_index_map["SPECTRAL"], axes_names=(name,), unit=self.get_units(i), name=name
         )
-        self.temporal_sampling, transform = time_model_from_date_obs([e["DATE-BEG"] for e in self.slice_headers])
-        self._transforms.append((transform, self._compound_model_partial(left=transform)))
 
-        self._i += 1
+        if "WAV" in self.header.get(f"CTYPE{n}", ""):  # Matches AWAV and WAVE
+            self.spectral_sampling, transform = self.make_spectral_from_wcs(n)
+        elif "FRAMEWAV" in self.header.keys():
+            self.spectral_sampling, transform = self.make_spectral_from_dataset(n)
+        else:
+            raise ValueError(
+                "Could not parse spectral WCS information from this header."
+            )  # pragma: no cover
 
-    @staticmethod
-    def constant_columns(table: astropy.table.Table, keys: list[str]):
-        """
-        Returns true if all columns given by keys have a constant value in table.
-        """
-        return all([np.allclose(table[0][k], table[k]) for k in keys])
+        return frame, (transform, self._compound_model_partial(left=transform))
 
-    def get_varying_spatial_axes(self) -> dict[str, list[int]]:
+    def make_temporal(self, axes):
         """
-        Compute the axes over which CRVAL or PC vary.
-        """
-        NAXIS, DAAXES, DNAXIS = self.header["NAXIS"], self.header["DAAXES"], self.header["DNAXIS"]
-        # Find which dataset axes the pointing varies along
-        # If any of these keys vary along any of the dataset axes we want to know
-        naxis_v = list(range(1, NAXIS + 1))
-        crval_keys = [f"CRVAL{n}" for n in naxis_v]
-        pc_keys = [f"PC{i}_{j}" for i, j in product(naxis_v, naxis_v)]
-        varying_axes = defaultdict(list)
-        for daxis in range(DAAXES + 1, DNAXIS + 1):
-            key = f"DINDEX{daxis}"
-            group = self.header_table.group_by(key)
-            groups = group.groups if len(group.groups) < len(self.header_table) else [self.header_table]
-            if all([not self.constant_columns(g, pc_keys) for g in groups]):
-                varying_axes["pc"].append(daxis)
-            if all([not self.constant_columns(g, crval_keys) for g in groups]):
-                varying_axes["crval"].append(daxis)
-
-        return dict(varying_axes)
+        Add a temporal axes to the builder.
+        """
+        frame = cf.TemporalFrame(
+            axes_order=self.world_type_index_map["TEMPORAL"],
+            name="temporal",
+            axes_names=("time",),
+            unit=(u.s,),
+            reference_frame=Time(self.header["DATE-AVG"]),
+        )
+        dslice = self.parser.slice_for_dataset_array_axes(*axes, indexing="python")
+        dates = self.parser.header_array[dslice]["DATE-AVG"]
+        self.temporal_sampling, transform = time_model_from_date_obs(dates)
+        return frame, (transform, self._compound_model_partial(left=transform))
 
-    def make_spatial(self):
+    def make_spatial(self, axes):
         """
         Add a helioprojective spatial pair to the builder.
-
-        .. note::
-            This increments the counter by two.
-
         """
-        i = self._i
-        name = self.header[f"DWNAME{self.n}"]
+        daxes = (np.array(axes) + 1).tolist()
+        name = self.header[f"DWNAME{daxes[0]}"]
         name = name.split(" ")[0]
-        axes_names = [
-            self.header[f"DWNAME{nn}"] for nn in (self.n, self._n(i + 1))
-        ]
 
+        # TODO: don't just use the first obstime
         obstime = Time(self.header["DATE-AVG"])
-        axes_types = [
-            "lat" if "LT" in self.axes_types[i] else "lon",
-            "lon" if "LN" in self.axes_types[i] else "lat",
-        ]
-        self._frames.append(
-            cf.CelestialFrame(
-                axes_order=(i, i + 1),
-                name=name,
-                # TODO: the celestial frame is wrong, we need to account for varying position and obstime
-                reference_frame=Helioprojective(obstime=obstime),
-                axes_names=axes_names,
-                unit=self.get_units(self._i, self._i + 1),
-                axis_physical_types=(
-                    f"custom:pos.helioprojective.{axes_types[0]}",
-                    f"custom:pos.helioprojective.{axes_types[1]}",
-                ),
-            )
+
+        # The dataset axes with a type of SPATIAL
+        spatial_dind = [d for d in range(1, self.header["DNAXIS"] + 1)
+                        if self.header[f"DTYPE{d}"] == "SPATIAL"]
+        axes_names = [self.header[f"DWNAME{da}"] for da in spatial_dind]
+
+        # Identify the indices of lat, lon based on CTYPE
+        spatial_ind = identify_spatial_axes(self.header)
+        # Generate a sorted list of [lat, lon] based on the indices.
+        axes_types = [t for _, t in sorted(zip(spatial_ind, ["lat", "lon"]))]
+        frame = cf.CelestialFrame(
+            axes_order=self.world_type_index_map["SPATIAL"],
+            name=name,
+            # TODO: Add (varying) observer location
+            reference_frame=Helioprojective(obstime=obstime),
+            axes_names=axes_names,
+            unit=self.get_units(*np.array(spatial_dind) - 1),
+            axis_physical_types=(
+                f"custom:pos.helioprojective.{axes_types[0]}",
+                f"custom:pos.helioprojective.{axes_types[1]}",
+            ),
         )
 
-        varying_spatial_axes = self.get_varying_spatial_axes()
+        varying_spatial_axes = self.parser.varying_spatial_daxes
         if varying_spatial_axes:
-            self.spatial_sampling, transform = varying_spatial_model_from_headers(self.header_table,
-                                                                                  varying_spatial_axes)
-
+            self.spatial_sampling, transform = varying_spatial_model_from_headers(axes, self.parser)
             # At this point we have already verified that if there are both pc and
             # crval keys in this dict they are the same length, so just use the
             # first one.
             shared_inputs = len(list(varying_spatial_axes.values())[0])
-            self._transforms.append((transform, partial(CoupledCompoundModel, op="&",
-                                                        left=transform, shared_inputs=shared_inputs)))
-
+            transform_pair = (transform, partial(CoupledCompoundModel, op="&",
+                                                 left=transform, shared_inputs=shared_inputs))
         else:
             self.spatial_sampling, transform = spatial_model_from_header(self.header)
-            self._transforms.append((transform, self._compound_model_partial(left=transform)))
-
-        self._i += 2
-
-    def make_spectral(self):
-        """
-        Decide how to make a spectral axes.
-        """
-        name = self.header[f"DWNAME{self.n}"]
-        self._frames.append(
-            cf.SpectralFrame(
-                axes_order=(self._i,), axes_names=(name,), unit=self.get_units(self._i), name=name
-            )
-        )
-
-        if "WAV" in self.header.get(f"CTYPE{self.n}", ""):  # Matches AWAV and WAVE
-            self.spectral_sampling, transform = self.make_spectral_from_wcs()
-        elif "FRAMEWAV" in self.header.keys():
-            self.spectral_sampling, transform = self.make_spectral_from_dataset()
-        else:
-            raise ValueError(
-                "Could not parse spectral WCS information from this header."
-            )  # pragma: no cover
-
-        self._transforms.append((transform, self._compound_model_partial(left=transform)))
+            transform_pair = (transform, self._compound_model_partial(left=transform))
 
-        self._i += 1
+        return frame, transform_pair
 
-    def make_spectral_from_dataset(self):
+    def make_spectral_from_dataset(self, n):
         """
         Make a spectral axes from (VTF) dataset info.
         """
-        framewave = [h["FRAMEWAV"] for h in self.slice_headers[: self.header[f"DNAXIS{self.n}"]]]
+        s = self.parser.slice_for_dataset_array_axes(n - 1, indexing="python")
+        framewave = np.array(self.parser.header_array[s]["FRAMEWAV"])
         return spectral_model_from_framewave(framewave)
 
-    def make_spectral_from_wcs(self):
+    def make_spectral_from_wcs(self, n):
         """
         Add a spectral axes from the FITS-WCS keywords.
         """
-        spectral_cdelt = self.header[f"CDELT{self.n}"] * u.nm
-        return spectral_cdelt, linear_spectral_model(
-            spectral_cdelt, self.header[f"CRVAL{self.n}"] * u.nm
+        unit = u.Unit(self.header[f"CUNIT{n}"])
+        spectral_cdelt = self.header[f"CDELT{n}"] * unit
+        return spectral_cdelt.to_value(u.nm), linear_spectral_model(
+            spectral_cdelt, self.header[f"CRVAL{n}"] * unit
         )
```

### Comparing `dkist-inventory-0.9.3/dkist_inventory.egg-info/SOURCES.txt` & `dkist-inventory-0.9.4rc1/dkist_inventory.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 .gitignore
 MANIFEST.in
 README.rst
 bitbucket-pipelines.yml
+conftest.py
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 dkist_inventory/__init__.py
 dkist_inventory/asdf_generator.py
+dkist_inventory/header_parsing.py
 dkist_inventory/inventory.py
 dkist_inventory/transforms.py
 dkist_inventory/version.py
 dkist_inventory.egg-info/PKG-INFO
 dkist_inventory.egg-info/SOURCES.txt
 dkist_inventory.egg-info/dependency_links.txt
 dkist_inventory.egg-info/not-zip-safe
 dkist_inventory.egg-info/requires.txt
 dkist_inventory.egg-info/top_level.txt
 dkist_inventory/tests/__init__.py
 dkist_inventory/tests/conftest.py
 dkist_inventory/tests/test_asdf_generator.py
+dkist_inventory/tests/test_header_parsing.py
 dkist_inventory/tests/test_inventory.py
 dkist_inventory/tests/test_transforms.py
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 licenses/LICENSE.rst
```

### Comparing `dkist-inventory-0.9.3/docs/Makefile` & `dkist-inventory-0.9.4rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-inventory-0.9.3/docs/conf.py` & `dkist-inventory-0.9.4rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-0.9.3/docs/make.bat` & `dkist-inventory-0.9.4rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-inventory-0.9.3/licenses/LICENSE.rst` & `dkist-inventory-0.9.4rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-inventory-0.9.3/licenses/TEMPLATE_LICENSE.rst` & `dkist-inventory-0.9.4rc1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-inventory-0.9.3/setup.cfg` & `dkist-inventory-0.9.4rc1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -10,30 +10,33 @@
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
 python_requires = >=3.9
 setup_requires = setuptools_scm
 install_requires = 
-	astropy>=5.0.2
+	astropy>=5.0.4
 	gwcs>=0.17.1
 	sunpy[net,asdf]>=2.1
 	numpy>=1.20  # For numpy typing support
 	ndcube>=2.0.1
 	packaging
-	dkist>=1.0.0b5
+	dkist>=1.0.0b8
+	dkist-fits-specifications>=2.0.0
+	scipy>=1.9.0
+	jsonschema!=4.10.0
 
 [options.extras_require]
 asdf = 
 	asdf
 test = 
 	pytest
 	pytest-doctestplus
 	pytest-cov
-	dkist-data-simulator>=1.3
+	dkist-data-simulator>=1.6
 	dkist-header-validator
 	pytest-mock
 docs = 
 	sphinx
 	sphinx-automodapi
 
 [tool:pytest]
```

### Comparing `dkist-inventory-0.9.3/setup.py` & `dkist-inventory-0.9.4rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-0.9.3/tox.ini` & `dkist-inventory-0.9.4rc1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 #     tox -l -v
 #
 description =
     run tests
 extras =
     asdf
     test
+deps =
+    pytest-xdist
 
 commands =
     pip freeze
     pytest --pyargs dkist_inventory {toxinidir}/docs --cov dkist_inventory --cov-config={toxinidir}/setup.cfg {posargs}
 
 [testenv:build_docs]
 changedir = docs
```

