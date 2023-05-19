# Comparing `tmp/raster2dggs-0.2.0.tar.gz` & `tmp/raster2dggs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster2dggs-0.2.0.tar", max compression
+gzip compressed data, was "raster2dggs-0.2.1.tar", max compression
```

## Comparing `raster2dggs-0.2.0.tar` & `raster2dggs-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8362 2023-05-03 02:57:00.605422 raster2dggs-0.2.0/README.md
--rw-r--r--   0        0        0     1091 2023-05-03 02:57:00.605422 raster2dggs-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-03 02:59:48.530270 raster2dggs-0.2.0/raster2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-03 02:59:13.750096 raster2dggs-0.2.0/raster2dggs/cli.py
--rw-r--r--   0        0        0    15356 2023-05-03 03:00:03.146344 raster2dggs-0.2.0/raster2dggs/h3.py
--rw-r--r--   0        0        0     9781 1970-01-01 00:00:00.000000 raster2dggs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     8424 2023-05-19 04:54:29.612237 raster2dggs-0.2.1/README.md
+-rw-r--r--   0        0        0     1091 2023-05-19 04:54:52.024349 raster2dggs-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-03 02:59:48.530270 raster2dggs-0.2.1/raster2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-03 02:59:13.750096 raster2dggs-0.2.1/raster2dggs/cli.py
+-rw-r--r--   0        0        0    15766 2023-05-19 04:52:32.967656 raster2dggs-0.2.1/raster2dggs/h3.py
+-rw-r--r--   0        0        0     9843 1970-01-01 00:00:00.000000 raster2dggs-0.2.1/PKG-INFO
```

### Comparing `raster2dggs-0.2.0/README.md` & `raster2dggs-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   s3://).
 
 Options:
   -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
                                   DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
-  -pr,--parent_res [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
+  -pr, --parent_res [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 Parent resolution to index and aggregate
                                   to. Defaults to resolution - 6
   -u, --upscale INTEGER           Upscaling factor, used to upsample input
                                   data on the fly; useful when the raster
                                   resolution is lower than the target DGGS
                                   resolution. Default (1) applies no
                                   upscaling. The resampling method controls
@@ -65,14 +65,15 @@
   --resampling [nearest|bilinear|cubic|cubic_spline|lanczos|average|mode|gauss|max|min|med|q1|q3|sum|rms]
                                   Input raster may be warped to EPSG:4326 if
                                   it is not already in this CRS. Or, if the
                                   upscale parameter is greater than 1, there
                                   is a need to resample. This setting
                                   specifies this resampling algorithm.
                                   [default: average]
+  --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
 
 ## Visualising output
 
 Output is in the Apache Parquet format, a directory with one file per partition. Partitions are based on parent cell IDs, with the parent resolution determined as an offset from the target DGGS resolution.
 
@@ -147,17 +148,17 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.2.0},
+  version={0.2.1},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.2.0) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.2.1) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `raster2dggs-0.2.0/pyproject.toml` & `raster2dggs-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raster2dggs"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/raster2dggs"
 keywords = ["dggs", "raster", "h3", "cli"]
```

### Comparing `raster2dggs-0.2.0/raster2dggs/cli.py` & `raster2dggs-0.2.1/raster2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `raster2dggs-0.2.0/raster2dggs/h3.py` & `raster2dggs-0.2.1/raster2dggs/h3.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,33 +41,34 @@
     "upscale": 1,
     "compression": "snappy",
     "threads": (multiprocessing.cpu_count() - 1),
     "aggfunc": "mean",
     "decimals": 1,
     "warp_mem_limit": 12000,
     "resampling": "average",
+    "tempdir": tempfile.tempdir
 }
 
 DEFAULT_PARENT_OFFSET = 6
 
 
 class ParentResolutionException(Exception):
     pass
 
 
-def _get_parent_res(parent_res: int, resolution: int) -> int:
+def _get_parent_res(parent_res: Union[None, int], resolution: int) -> int:
     """
     Uses a parent resolution,
     OR,
     Given a target resolution, returns our recommended parent resolution.
 
     Used for intermediate re-partioning.
     """
     return (
-        parent_res
+        int(parent_res)
         if parent_res is not None
         else max(MIN_H3, (resolution - DEFAULT_PARENT_OFFSET))
     )
 
 
 def _h3func(
     sdf: xr.DataArray,
@@ -106,15 +107,15 @@
     return pa.Table.from_pandas(h3index)
 
 
 def _initial_index(
     raster_input: Union[Path, str],
     output: Path,
     resolution: int,
-    parent_res: int,
+    parent_res: Union[None, int],
     warp_args: dict,
     **kwargs,
 ) -> Path:
     """
     Responsible for opening the raster_input, and performing H3 indexing per window of a WarpedVRT.
 
     A WarpedVRT is used to enforce reprojection to https://epsg.io/4326, which is required for H3 indexing.
@@ -361,36 +362,45 @@
 )
 @click.option(
     "--resampling",
     default=DEFAULTS["resampling"],
     type=click.Choice(Resampling._member_names_),
     help="Input raster may be warped to EPSG:4326 if it is not already in this CRS. Or, if the upscale parameter is greater than 1, there is a need to resample. This setting specifies this resampling algorithm.",
 )
+@click.option(
+    "--tempdir",
+    default=DEFAULTS["tempdir"],
+    type=click.Path(),
+    help="Temporary data is created during the execution of this program. This parameter allows you to control where this data will be written."
+)
 @click.version_option(version=__version__)
 def h3(
     raster_input: Union[str, Path],
     output_directory: Union[str, Path],
     resolution: str,
     parent_res: str,
     upscale: int,
     compression: str,
     threads: int,
     aggfunc: str,
     decimals: int,
     overwrite: bool,
     warp_mem_limit: int,
     resampling: str,
+    tempdir: Union[str, Path],
 ):
     """
     Ingest a raster image and index it to the H3 DGGS.
 
     RASTER_INPUT is the path to input raster data; prepend with protocol like s3:// or hdfs:// for remote data.
     OUTPUT_DIRECTORY should be a directory, not a file, as it will be the write location for an Apache Parquet data store, with partitions equivalent to parent cells of target cells at a fixed offset. However, this can also be remote (use the appropriate prefix, e.g. s3://).
     """
-    if not int(parent_res) < int(resolution):
+    tempfile.tempdir = tempdir
+    print(tempfile.tempdir)
+    if parent_res is not None and not int(parent_res) < int(resolution):
         raise ParentResolutionException(
             "Parent resolution ({pr}) must be less than target resolution ({r})".format(
                 pr=parent_res, r=resolution
             )
         )
     if not Path(raster_input).exists():
         if not urlparse(raster_input).scheme:
@@ -421,11 +431,11 @@
         "resampling": resampling,
         "overwrite": overwrite,
     }
     _initial_index(
         raster_input,
         output_directory,
         int(resolution),
-        int(parent_res),
+        parent_res,
         warp_args,
         **kwargs,
     )
```

### Comparing `raster2dggs-0.2.0/PKG-INFO` & `raster2dggs-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster2dggs
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/manaakiwhenua/raster2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,raster,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -64,15 +64,15 @@
   s3://).
 
 Options:
   -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
                                   DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
-  -pr,--parent_res [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
+  -pr, --parent_res [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 Parent resolution to index and aggregate
                                   to. Defaults to resolution - 6
   -u, --upscale INTEGER           Upscaling factor, used to upsample input
                                   data on the fly; useful when the raster
                                   resolution is lower than the target DGGS
                                   resolution. Default (1) applies no
                                   upscaling. The resampling method controls
@@ -100,14 +100,15 @@
   --resampling [nearest|bilinear|cubic|cubic_spline|lanczos|average|mode|gauss|max|min|med|q1|q3|sum|rms]
                                   Input raster may be warped to EPSG:4326 if
                                   it is not already in this CRS. Or, if the
                                   upscale parameter is greater than 1, there
                                   is a need to resample. This setting
                                   specifies this resampling algorithm.
                                   [default: average]
+  --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
 
 ## Visualising output
 
 Output is in the Apache Parquet format, a directory with one file per partition. Partitions are based on parent cell IDs, with the parent resolution determined as an offset from the target DGGS resolution.
 
@@ -182,18 +183,18 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.2.0},
+  version={0.2.1},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.2.0) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.2.1) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

