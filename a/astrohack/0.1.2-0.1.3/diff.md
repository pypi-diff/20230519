# Comparing `tmp/astrohack-0.1.2.tar.gz` & `tmp/astrohack-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.1.2.tar", last modified: Fri May 12 20:00:47 2023, max compression
+gzip compressed data, was "astrohack-0.1.3.tar", last modified: Fri May 19 20:04:48 2023, max compression
```

## Comparing `astrohack-0.1.2.tar` & `astrohack-0.1.3.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 20:00:28.000000 astrohack-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:00:28.000000 astrohack-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-12 20:00:47.466786 astrohack-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-12 20:00:28.000000 astrohack-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:28.000000 astrohack-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 20:00:28.000000 astrohack-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:00:47.470786 astrohack-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.454786 astrohack-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.458786 astrohack-0.1.2/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.458786 astrohack-0.1.2/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    30692 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    21553 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31185 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.454786 astrohack-0.1.2/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    20249 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.458786 astrohack-0.1.2/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_class_antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_class_ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_class_telescope.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_stakeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.749603 astrohack-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 20:04:27.000000 astrohack-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:04:27.000000 astrohack-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-19 20:04:48.749603 astrohack-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-19 20:04:27.000000 astrohack-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:27.000000 astrohack-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-19 20:04:27.000000 astrohack-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:04:48.749603 astrohack-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.729604 astrohack-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.733604 astrohack-0.1.3/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.737604 astrohack-0.1.3/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    32566 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.741603 astrohack-0.1.3/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_dask_graph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.741603 astrohack-0.1.3/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22921 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.741603 astrohack-0.1.3/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32810 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.741603 astrohack-0.1.3/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/_utils/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.729604 astrohack-0.1.3/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.741603 astrohack-0.1.3/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.741603 astrohack-0.1.3/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.741603 astrohack-0.1.3/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.745603 astrohack-0.1.3/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.745603 astrohack-0.1.3/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.745603 astrohack-0.1.3/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.745603 astrohack-0.1.3/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.745603 astrohack-0.1.3/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)    19946 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.745603 astrohack-0.1.3/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-19 20:04:27.000000 astrohack-0.1.3/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.737604 astrohack-0.1.3/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-19 20:04:48.000000 astrohack-0.1.3/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-19 20:04:48.000000 astrohack-0.1.3/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:04:48.000000 astrohack-0.1.3/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-19 20:04:48.000000 astrohack-0.1.3/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 20:04:48.000000 astrohack-0.1.3/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:04:48.749603 astrohack-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-19 20:04:27.000000 astrohack-0.1.3/tests/test_class_antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-05-19 20:04:27.000000 astrohack-0.1.3/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-19 20:04:27.000000 astrohack-0.1.3/tests/test_class_ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-19 20:04:27.000000 astrohack-0.1.3/tests/test_class_telescope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-05-19 20:04:27.000000 astrohack-0.1.3/tests/test_stakeholder.py
```

### Comparing `astrohack-0.1.2/LICENSE` & `astrohack-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/PKG-INFO` & `astrohack-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.2
+Version: 0.1.3
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.2/README.md` & `astrohack-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/pyproject.toml` & `astrohack-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.1.2"
+version = "0.1.3"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.1.2/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.1.3/src/astrohack/_classes/antenna_surface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import numpy as np
 import xarray as xr
 from matplotlib import pyplot as plt
 from matplotlib import colormaps as cmaps
 
 from astrohack._classes.base_panel import panel_models, irigid
 from astrohack._classes.ring_panel import RingPanel
 from astrohack._utils._constants import *
 from astrohack._utils._conversion import _convert_to_db
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._tools import _add_prefix, _well_positioned_colorbar
+from astrohack._utils._tools import _add_prefix, _well_positioned_colorbar, _axis_to_fits_header
+from astrohack._utils._io import _write_fits
 
 lnbr = "\n"
 figsize = [5, 4]
 
 
 class AntennaSurface:
     def __init__(self, inputxds, telescope, cutoff=None, pmodel=None, crop=False, panel_margins=None, reread=False):
@@ -529,15 +529,16 @@
         nplots = len(maps)
         vmax = np.nanmax(np.abs(conversion*maps[0]))
         vmin = -vmax
         for iplot in range(nplots):
             title = f'{prefix.capitalize()} {labels[iplot]}'
             plotname = _add_prefix(basename, labels[iplot])
             plotname = _add_prefix(plotname, prefix)
-            self._plot_map(plotname, conversion*maps[iplot], title, vmin, vmax, unit, screws=screws, dpi=dpi)
+            self._plot_map(plotname, conversion*maps[iplot], title, vmin, vmax, unit, screws=screws, dpi=dpi,
+                           colormap=colormap, figuresize=figuresize)
 
     def _plot_map(self, filename, data, title, vmin, vmax, unit, screws=False, colormap=None, figuresize=None, dpi=300,
                   colorbar=True):
         if colormap is None:
             colormap = 'viridis'
         if figuresize is None:
             figuresize = figsize
@@ -705,7 +706,41 @@
             xds.attrs['input_rms'] = rms
             xds.attrs['input_gain'] = gains[0]
             xds.attrs['theoretical_gain'] = gains[1]
             coords = {"u": self.u_axis, "v": self.v_axis}
 
         xds = xds.assign_coords(coords)
         return xds
+
+    def export_to_fits(self, basename):
+        """
+        Data to export: Amplitude, mask, phase, phase_corrections, phase_residuals, deviations, deviation_corrections, deviation_residuals
+        conveniently all data are on the same grid!
+        Returns:
+        """
+
+        head = {
+            'PMODEL'  : self.panelmodel,
+            'PMARGIN' : self.panel_margins,
+            'CUTOFF'  : self.cut,
+            'TELESCOP': self.antenna_name,
+            'INSTRUME': self.telescope.name,
+            'WAVELENG': self.wavelength,
+            'FREQUENC': clight/self.wavelength
+        }
+        head = _axis_to_fits_header(head, self.u_axis, 1, 'X', 'm')
+        head = _axis_to_fits_header(head, self.v_axis, 2, 'Y', 'm')
+
+        _write_fits(head, 'Amplitude', self.amplitude, basename + '_amplitude.fits', self.amp_unit, 'panel')
+        _write_fits(head, 'Mask', np.where(self.mask, 1.0, np.nan), basename + '_mask.fits', '', 'panel')
+        _write_fits(head, 'Original Phase', self.phase, basename + '_phase_original.fits', 'rad', 'panel')
+        _write_fits(head, 'Phase Corrections', self.phase_corrections, basename + '_phase_correction.fits', 'rad',
+                    'panel')
+        _write_fits(head, 'Phase residuals', self.phase_residuals, basename + '_phase_residual.fits', 'rad',
+                    'panel')
+        _write_fits(head, 'Original Deviation', self.deviation, basename + '_deviation_original.fits', 'm',
+                    'panel')
+        _write_fits(head, 'Deviation Corrections', self.corrections, basename + '_deviation_correction.fits', 'm',
+                    'panel')
+        _write_fits(head, 'Deviation residuals', self.residuals, basename + '_deviation_residual.fits', 'm',
+                    'panel')
+
```

### Comparing `astrohack-0.1.2/src/astrohack/_classes/base_panel.py` & `astrohack-0.1.3/src/astrohack/_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.1.3/src/astrohack/_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_classes/ring_panel.py` & `astrohack-0.1.3/src/astrohack/_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_classes/telescope.py` & `astrohack-0.1.3/src/astrohack/_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_algorithms.py` & `astrohack-0.1.3/src/astrohack/_utils/_algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     if system.shape[0] < system.shape[1]:
         raise Exception('System must have at least the same number of rows as it has of columns')
     
     fit = np.linalg.lstsq(system, vector, rcond=None)
     
     result = fit[0]
     residuals = fit[1]
-    covar = np.matrix(np.dot(system.T, system)).I
+    covar = np.linalg.inv(np.dot(system.T, system))
     variances = np.diagonal(covar)
     
     return result, variances, residuals
 
 def _least_squares_fit_block(system, vector):
     """
     Least squares fitting of a system of linear equations
@@ -220,16 +220,27 @@
         n_pix = np.sum([r_diff > max_dis]) + 1
         cell_size = np.mean(r_diff[r_diff > max_dis])
         
         grid_parms['ant_'+ant_names[ant_index]] = {'n_pix':n_pix,'cell_size':cell_size}
 
 
     return grid_parms
-    
-    
+
+def _significant_digits(x, digits):
+    if np.isscalar(x):
+        return _significant_digits_scalar(x,digits)
+    else:
+        return list(map(_significant_digits,x,[digits]*len(x)))
+
+
+def _significant_digits_scalar(x, digits):
+    if x == 0 or not np.isfinite(x):
+        return x
+    digits = int(digits - np.ceil(np.log10(abs(x))))
+    return round(x, digits)
     
     
 #Does not work
 #def _average_repeated_pointings(vis_map_dict, weight_map_dict, flagged_mapping_antennas,time_vis,pnt_map_dict, ant_names):
 #
 #    for ant_index in vis_map_dict.keys():
 #        diff_ideal = np.diff(pnt_map_dict['ant_'+ant_names[ant_index]]['POINTING_OFFSET'],axis=0)
```

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_combine.py` & `astrohack-0.1.3/src/astrohack/_utils/_combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_constants.py` & `astrohack-0.1.3/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_conversion.py` & `astrohack-0.1.3/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.1.3/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.1.3/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_dio.py` & `astrohack-0.1.3/src/astrohack/_utils/_dio.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,25 +94,25 @@
         Returns:
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
         if file is None:
             file = self.file
 
-        self._meta_data = _read_meta_data(file, 'image')
-
         try:
             _load_image_file(file, image_dict=self)
 
             self._open = True
 
         except Exception as e:
             logger.error("[AstroHackImageFile.open()]: {}".format(e))
             self._open = False
 
+        self._meta_data = _read_meta_data(file, 'image', ['combine', 'holog'])
+
         return self._open
 
     def summary(self):
         """
            Prints summary table of holog image file. 
         """
 
@@ -179,24 +179,24 @@
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
 
-        self._meta_data = _read_meta_data(file, 'holog')
-
         try:
             _load_holog_file(holog_file=file, dask_load=dask_load, load_pnt_dict=False, holog_dict=self)
             self._open = True
 
         except Exception as e:
             logger.error("[AstrohackHologFile]: {}".format(e))
             self._open = False
-        
+
+        self._meta_data = _read_meta_data(file, 'holog', 'extract_holog')
+
         return self._open
 
     def summary(self):
         """
             Prints summary table of holog file.
         """
         print("Atributes:")
@@ -271,23 +271,23 @@
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
 
-        self._meta_data = _read_meta_data(file, 'panel')
-
         try:
             _load_panel_file(file, panel_dict=self)
             self._open = True
         except Exception as e:
             logger.error("[AstroHackPanelFile.open()]: {}".format(e))
             self._open = False
 
+        self._meta_data = _read_meta_data(file, 'panel', 'panel')
+
         return self._open
 
     def summary(self):
         """
            Prints summary table of panel image file.
         """
 
@@ -301,24 +301,25 @@
         
         for ant in self.keys():
             table.add_row([ant, list(self[ant].keys())])
 
         print('\nContents:')
         print(table)
 
-    def get_antenna(self, antenna, ddi):
+    def get_antenna(self, antenna, ddi, dask_load=True):
         """
         Return an AntennaSurface object for interaction
         Args:
             antenna: Which antenna in to be used
             ddi: Which ddi is to be used
+            dask_load: Load xds using dask?
         Returns:
             AntennaSurface object contaning relevant information for panel adjustments
         """
-        xds = _load_image_xds(self.file, antenna, ddi)
+        xds = _load_image_xds(self.file, antenna, ddi, dask_load)
         telescope = Telescope(xds.attrs['telescope_name'])
         
         return AntennaSurface(xds, telescope, reread=True)
 
 
 class AstrohackPointFile(dict):
     """
@@ -349,23 +350,24 @@
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
 
-        self._meta_data = _read_meta_data(file, 'point')
         try:
             _load_point_file(file=file, dask_load=dask_load, pnt_dict=self)
             self._open = True
 
         except Exception as e:
             logger.error("[AstrohackPointFile]: {}".format(e))
             self._open = False
-        
+
+        self._meta_data = _read_meta_data(file, 'point', 'extract_holog')
+
         return self._open
 
     def summary(self):
         """
             Prints summary table of pointing file.
         """
         print("Atributes:")
```

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.1.3/src/astrohack/_utils/_extract_holog.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 from numba import njit
 from numba.core import types
 
 from casacore import tables as ctables
 from astrohack._utils._imaging import _calculate_parallactic_angle_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._io import _write_meta_data
-from astrohack._utils._algorithms import _get_grid_parms
+from astrohack._utils._algorithms import _get_grid_parms, _significant_digits
 
 from astrohack._utils._io import _load_point_file
 
 
 def _extract_holog_chunk(extract_holog_params):
     """Perform data query on holography data chunk and get unique time and state_ids/
 
     Args:
         ms_name (str): Measurementset name
-        data_col (str): Data column to extract.
+        data_column (str): Data column to extract.
         ddi (int): Data description id
         scan (int): Scan number
         map_ant_ids (numpy.narray): Array of antenna_id values corresponding to mapping data.
         ref_ant_ids (numpy.narray): Arry of antenna_id values corresponding to reference data.
         sel_state_ids (list): List pf state_ids corresponding to holography data/
     """
     logger = _get_astrohack_logger()
 
     ms_name = extract_holog_params["ms_name"]
     pnt_name = extract_holog_params["point_name"]
-    data_col = extract_holog_params["data_col"]
+    data_column = extract_holog_params["data_column"]
     ddi = extract_holog_params["ddi"]
     scans = extract_holog_params["scans"]
     ant_names = extract_holog_params["ant_names"]
     ref_ant_per_map_ant_tuple = extract_holog_params["ref_ant_per_map_ant_tuple"]
     map_ant_tuple = extract_holog_params["map_ant_tuple"]
     ref_ant_per_map_ant_name_tuple = extract_holog_params["ref_ant_per_map_ant_name_tuple"]
     map_ant_name_tuple = extract_holog_params["map_ant_name_tuple"]
@@ -53,23 +53,23 @@
     pol = extract_holog_params["pol_setup"]["pol"]
     
     table_obj = ctables.table(ms_name, readonly=True, lockoptions={'option': 'usernoread'}, ack=False)
 
     if sel_state_ids:
         ctb = ctables.taql(
             "select %s, ANTENNA1, ANTENNA2, TIME, TIME_CENTROID, WEIGHT, FLAG_ROW, FLAG from $table_obj WHERE DATA_DESC_ID == %s AND SCAN_NUMBER in %s AND STATE_ID in %s"
-            % (data_col, ddi, list(scans), list(sel_state_ids))
+            % (data_column, ddi, list(scans), list(sel_state_ids))
         )
     else:
         ctb = ctables.taql(
             "select %s, ANTENNA1, ANTENNA2, TIME, TIME_CENTROID, WEIGHT, FLAG_ROW, FLAG from $table_obj WHERE DATA_DESC_ID == %s AND SCAN_NUMBER in %s"
-            % (data_col, ddi, list(scans))
+            % (data_column, ddi, list(scans))
         )
         
-    vis_data = ctb.getcol(data_col)
+    vis_data = ctb.getcol(data_column)
     weight = ctb.getcol("WEIGHT")
     ant1 = ctb.getcol("ANTENNA1")
     ant2 = ctb.getcol("ANTENNA2")
     time_vis_row = ctb.getcol("TIME")
     time_vis_row_centroid = ctb.getcol("TIME_CENTROID")
     flag = ctb.getcol("FLAG")
     flag_row = ctb.getcol("FLAG_ROW")
@@ -340,14 +340,18 @@
                 weight_map_dict[map_ant_index], dims=["time", "chan", "pol"]
             )
 
             xds["DIRECTIONAL_COSINES"] = xr.DataArray(
                 pnt_map_dict[map_ant_tag]["DIRECTIONAL_COSINES"].values, dims=["time", "lm"]
             )
             
+            xds["IDEAL_DIRECTIONAL_COSINES"] = xr.DataArray(
+                pnt_map_dict[map_ant_tag]["POINTING_OFFSET"].values, dims=["time", "lm"]
+            )
+            
             xds.attrs["holog_map_key"] = holog_map_key
             #xds.attrs["ant_id"] = map_ant_tag
             xds.attrs["ddi"] = ddi
             xds.attrs["parallactic_samples"] = parallactic_samples
             xds.attrs["telescope_name"] = telescope_name
             xds.attrs["antenna_name"] = ant_names[map_ant_index]
             
@@ -381,15 +385,15 @@
         else:
             logger.warning(
                 "[FLAGGED DATA] mapping antenna index {index}".format(index=ant_names[map_ant_index]
                 )
             )
 
 
-def _create_holog_obs_dict(pnt_dict,baseline_average_distance,ant_names,ant_pos,ant_names_main):
+def _create_holog_obs_dict(pnt_dict,baseline_average_distance,baseline_average_nearest,ant_names,ant_pos,ant_names_main):
     '''
     Generate holog_obs_dict.
     '''
 
     logger = _get_astrohack_logger()
     mapping_scans_dict = {}
     holog_obs_dict = {}
@@ -402,60 +406,79 @@
             ant_name = ant_name.replace('ant_','')
             if ant_name in ant_names_main: #Check if antenna in main table.
                 ant_names_set.add(ant_name)
                 for ddi, map_dict in ant_ds.attrs['mapping_scans_obs_dict'][0].items():
                     if ddi not in holog_obs_dict:
                             holog_obs_dict[ddi] = {}
                     for ant_map_id, scan_list in map_dict.items():
+                        #logger.debug('ant name ' + ant_name + ' scan list' + str(scan_list))
                         if scan_list:
                             map_key = _check_if_array_in_dict(mapping_scans_dict,scan_list)
                             if not map_key:
                                 map_key = 'map_' + str(map_id)
                                 mapping_scans_dict [map_key] = scan_list
                                 map_id = map_id+1
                                 
                             if map_key not in holog_obs_dict[ddi]:
                                 holog_obs_dict[ddi][map_key] = {'scans':np.array(scan_list),'ant':{}}
-                                                        
+                                
                             holog_obs_dict[ddi][map_key]['ant'][ant_name] = []
-       
+
     # If users specifies a baseline_average_distance we need to create an antenna distance matrix.
-    if baseline_average_distance != 'ALL':
+    if (baseline_average_distance != 'all') or (baseline_average_nearest != 'all'):
         import pandas as pd
         from scipy.spatial import distance_matrix
         df = pd.DataFrame(ant_pos, columns=['x', 'y', 'z'], index=ant_names)
         df_mat = pd.DataFrame(distance_matrix(df.values, df.values), index=df.index, columns=df.index)
         logger.debug('Antenna distance matrix in meters: \n' + str(df_mat))
-                        
+        
+                
+    if (baseline_average_distance != 'all') and (baseline_average_nearest != 'all'):
+        logger.error('baseline_average_distance and baseline_average_nearest can not both be specified.')
+        raise
+
+    
     #The reference antennas are then given by ref_ant_set = ant_names_set - map_ant_set.
     for ddi, ddi_dict in holog_obs_dict.items():
         for map_id, map_dict in ddi_dict.items():
             map_ant_set = set(map_dict['ant'].keys())
-            ref_ant_set = ant_names_set - map_ant_set
-
             map_ant_keys = list(map_dict['ant'].keys()) #Need a copy because of del holog_obs_dict[ddi][map_id]['ant'][map_ant_key] below.
+            
             for map_ant_key in map_ant_keys:
-                #add code for distance from antenna
+                ref_ant_set = ant_names_set - map_ant_set
+
+                #Select reference antennas by distance from mapping antenna
                 if baseline_average_distance != 'all':
                     sub_ref_ant_set = []
                     for ref_ant in ref_ant_set:
                         if df_mat.loc[map_ant_key,ref_ant] < baseline_average_distance:
                             sub_ref_ant_set.append(ref_ant)
                         
                     if (not sub_ref_ant_set) and (ref_ant_set):
                         logger.warning('DDI ' + str(ddi) + ' and mapping antenna ' + str(map_ant_key) + ' has no reference antennas. If baseline_average_distance was specified increase this distance. See antenna distance matrix in log by setting debug level to DEBUG in astrohack_client function.')
                      
                     ref_ant_set = sub_ref_ant_set
+                    
+                #Select reference antennas by n closest antennas
+                if baseline_average_nearest != 'all':
+                    sub_ref_ant_set = []
+                    nearest_ant_list = df_mat.loc[map_ant_key,:].loc[list(ref_ant_set)].sort_values().index.tolist()[1:baseline_average_nearest+1] #Skip first value since that is the antenna itself (distance=0)
+                    for ref_ant in ref_ant_set:
+                        if ref_ant in nearest_ant_list:
+                            sub_ref_ant_set.append(ref_ant)
+                            
+                    ref_ant_set = sub_ref_ant_set
+                ##################################################
                 
                 if ref_ant_set:
                     holog_obs_dict[ddi][map_id]['ant'][map_ant_key] = np.array(list(ref_ant_set))
                 else:
                     del holog_obs_dict[ddi][map_id]['ant'][map_ant_key] #Don't want mapping antennas with no reference antennas.
                     logger.warning('DDI ' + str(ddi) + ' and mapping antenna ' + str(map_ant_key) + ' has no reference antennas.')
-                     
+    
     return holog_obs_dict
 
 
 def _check_if_array_in_dict(array_dict,array):
     
     for key,val in array_dict.items():
         if np.array_equiv(val,array):
@@ -516,16 +539,17 @@
                             elif ddi not in ant_holog_dict[ant]:
                                 ant_holog_dict[ant][ddi] = {map:{}}
                     
                             ant_holog_dict[ant][ddi][map] = xds.to_dict(data=False)
                             cell_sizes.append(xds.attrs["grid_parms"]["cell_size"])
                             n_pixs.append(xds.attrs["grid_parms"]["n_pix"])
                             telescope_names.append(xds.attrs['telescope_name'])
-
-    if not (len(set(cell_sizes)) == 1):
+    
+    cell_sizes_sigfigs =  _significant_digits(cell_sizes,digits=3)
+    if not (len(set(cell_sizes_sigfigs)) == 1):
         logger.error('Cell size not consistant: ' + str(cell_sizes))
         raise
         
     if not (len(set(n_pixs)) == 1):
         logger.error('Number of pixels not consistant: ' + str(n_pixs))
         raise
         
@@ -536,15 +560,15 @@
     try:
         with open(output_meta_file, "w") as json_file:
             json.dump(ant_holog_dict, json_file)
 
     except Exception as error:
         logger.error("[_create_holog_meta_data] {error}".format(error=error))
 
-    meta_data = {'cell_size': cell_sizes[0],
+    meta_data = {'cell_size': np.mean(cell_sizes),
                  'n_pix': n_pixs[0],
                  'telescope_name': telescope_names[0]}
     meta_data.update(input_params)
     holog_attr_file = "{name}/{ext}".format(name=holog_file, ext=".holog_attr")
     _write_meta_data('extract_holog', holog_attr_file, meta_data)
     point_attr_file = "{name}/{ext}".format(name=input_params['point_name'], ext=".point_attr")
     _write_meta_data('extract_holog', point_attr_file, input_params)
```

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_extract_point.py` & `astrohack-0.1.3/src/astrohack/_utils/_extract_point.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_gaussfitter.py` & `astrohack-0.1.3/src/astrohack/_utils/_gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_holog.py` & `astrohack-0.1.3/src/astrohack/_utils/_holog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import scipy
-import json
 import numpy as np
 import xarray as xr
 
 from scipy.interpolate import griddata
 
 from astrohack._classes.telescope import Telescope
 
-from astrohack._utils._io import _load_holog_file
-from astrohack._utils._io import _read_meta_data, _write_meta_data
+from astrohack._utils._io import _load_holog_file, _load_image_xds
+from astrohack._utils._io import _read_meta_data, _write_meta_data, _write_fits
 
 from astrohack._utils._panel import _phase_fitting_block
 
 from astrohack._utils._algorithms import _chunked_average
 from astrohack._utils._algorithms import _find_peak_beam_value
 from astrohack._utils._algorithms import _find_nearest
 from astrohack._utils._algorithms import _calc_coords
 
 from astrohack._utils._conversion import _to_stokes
+from astrohack._utils._constants import clight
+from astrohack._utils._tools import _bool_to_string, _axis_to_fits_header, _stokes_axis_to_fits_header
 
 from astrohack._utils._imaging import _parallactic_derotation
 from astrohack._utils._imaging import _mask_circular_disk
 from astrohack._utils._imaging import _calculate_aperture_pattern
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
@@ -42,15 +43,15 @@
         holog_chunk_params["holog_file"],
         dask_load=False,
         load_pnt_dict=False,
         ant_id=holog_chunk_params["ant_id"],
         ddi_id=holog_chunk_params["ddi_id"]
     )
 
-    meta_data = _read_meta_data(holog_chunk_params["holog_file"], 'holog')
+    meta_data = _read_meta_data(holog_chunk_params["holog_file"], 'holog', 'extract_holog')
 
     # Calculate lm coordinates
     l, m = _calc_coords(holog_chunk_params["grid_size"], holog_chunk_params["cell_size"])
     grid_l, grid_m = list(map(np.transpose, np.meshgrid(l, m)))
     
     to_stokes = holog_chunk_params["to_stokes"]
 
@@ -105,25 +106,25 @@
             
             freq_chan = [np.mean(avg_freq)]
         else:
             beam_grid[holog_map_index, ...] = np.moveaxis(griddata(lm, vis, (grid_l, grid_m), method=holog_chunk_params["grid_interpolation_mode"],fill_value=0.0), (0,1), (2,3))
 
 
         time_centroid_index = ant_data_dict[ddi][holog_map].dims["time"] // 2
-
         time_centroid.append(ant_data_dict[ddi][holog_map].coords["time"][time_centroid_index].values)
 
         for chan in range(n_chan): ### Todo: Vectorize holog_map and channel axis
             try:
                 xx_peak = _find_peak_beam_value(beam_grid[holog_map_index, chan, 0, ...], scaling=0.25)
                 yy_peak = _find_peak_beam_value(beam_grid[holog_map_index, chan, 3, ...], scaling=0.25)
             except:
-                center_pixel = np.array(beam_grid.shape[0:2])//2
+                center_pixel = np.array(beam_grid.shape[-2:])//2
                 xx_peak = beam_grid[holog_map_index, chan, 0, center_pixel[0], center_pixel[1]]
                 yy_peak = beam_grid[holog_map_index, chan, 3, center_pixel[0], center_pixel[1]]
+
             normalization = np.abs(0.5 * (xx_peak + yy_peak))
             beam_grid[holog_map_index, chan, ...] /= normalization
 
     beam_grid = _parallactic_derotation(data=beam_grid, parallactic_angle_dict=ant_data_dict[ddi])
     
 
     ###############
@@ -188,15 +189,14 @@
     end_cut = center_pixel + radius
 
     amplitude = np.absolute(aperture_grid[..., start_cut[0]:end_cut[0], start_cut[1]:end_cut[1]])
     phase = np.angle(aperture_grid[..., start_cut[0]:end_cut[0], start_cut[1]:end_cut[1]])
     phase_corrected_angle = np.zeros_like(phase)
     u_prime = u[start_cut[0]:end_cut[0]]
     v_prime = v[start_cut[1]:end_cut[1]]
-    
 
     phase_fit_par = holog_chunk_params["phase_fit"]
     if isinstance(phase_fit_par, bool):
         do_phase_fit = phase_fit_par
         do_pnt_off = True
         do_xy_foc_off = True
         do_z_foc_off = True
@@ -315,7 +315,99 @@
     Save image meta data to a json file
     Args:
         image_file: image file
         input_params: holog input parameter dictionaire
     """
     output_attr_file = "{name}/{ext}".format(name=image_file, ext=".image_attr")
     _write_meta_data('holog', output_attr_file, input_params)
+
+
+def _export_to_fits_holog_chunk(parm_dict):
+    """
+    Holog side chunk function for the user facing function export_to_fits
+    Args:
+        parm_dict: parameter dictionary
+    """
+    logger = _get_astrohack_logger()
+
+    inputxds = _load_image_xds(parm_dict['filename'], parm_dict['this_antenna'], parm_dict['this_ddi'], dask_load=False)
+    metadata = parm_dict['holog_mds']._meta_data
+
+    antenna = parm_dict['this_antenna']
+    ddi = parm_dict['this_ddi']
+    destination = parm_dict['destination']
+    basename = f'{destination}/image_{antenna}_{ddi}'
+
+    logger.info(f'Exporting image contents of {antenna} {ddi} to FITS files in {destination}')
+
+    nchan = len(inputxds.chan)
+    if nchan == 1:
+        reffreq = inputxds.chan.values[0]
+    else:
+        reffreq = inputxds.chan.values[nchan//2]
+    telname = inputxds.attrs['telescope_name']
+    if telname in ['EVLA', 'VLA', 'JVLA']:
+        telname = 'VLA'
+    polist = []
+    for pol in inputxds.pol:
+        polist.append(str(pol.values))
+    baseheader = {
+        'STOKES'  : ", ".join(polist),
+        'WAVELENG': clight/reffreq,
+        'FREQUENC': reffreq,
+        'TELESCOP': inputxds.attrs['ant_name'],
+        'INSTRUME': telname,
+        'TIME_CEN': inputxds.attrs['time_centroid'],
+        'PADDING' : metadata['padding_factor'],
+        'GRD_INTR': metadata['grid_interpolation_mode'],
+        'CHAN_AVE': _bool_to_string(metadata['chan_average']),
+        'CHAN_TOL': metadata['chan_tolerance_factor'],
+        'SCAN_AVE': _bool_to_string(metadata['scan_average']),
+        'TO_STOKE': _bool_to_string(metadata['to_stokes']),
+    }
+    ntime = len(inputxds.time)
+    if ntime != 1:
+        logger.error("Data with multiple times not supported for FITS export")
+        raise Exception("Data with multiple times not supported for FITS export")
+
+    carta_dim_order = (1, 0, 2, 3, )
+
+    baseheader = _axis_to_fits_header(baseheader, inputxds.chan.values, 3, 'Frequency', 'Hz')
+    baseheader = _stokes_axis_to_fits_header(baseheader, 4)
+
+    beamheader = _axis_to_fits_header(baseheader, inputxds.l.values, 1, 'L', 'rad')
+    beamheader = _axis_to_fits_header(beamheader, inputxds.m.values, 2, 'M', 'rad')
+    transpobeam = np.transpose(inputxds['BEAM'][0, ...].values, carta_dim_order)
+    if parm_dict['complex_split'] == 'cartesian':
+        _write_fits(beamheader, 'Complex beam real part', transpobeam.real, basename + '_beam_real.fits', 'Normalized',
+                    'image')
+        _write_fits(beamheader, 'Complex beam imag part', transpobeam.imag, basename + '_beam_imag.fits', 'Normalized',
+                    'image')
+    else:
+        _write_fits(beamheader, 'Complex beam amplitude', np.absolute(transpobeam),
+                    basename + '_beam_amplitude.fits', 'Normalized', 'image')
+        _write_fits(beamheader, 'Complex beam phase', np.angle(transpobeam), basename + '_beam_phase.fits',
+                    'Radians', 'image')
+
+    apertureheader = _axis_to_fits_header(baseheader, inputxds.u.values, 1, 'X', 'm')
+    apertureheader = _axis_to_fits_header(apertureheader, inputxds.v.values, 2, 'Y', 'm')
+    transpoaper = np.transpose(inputxds['APERTURE'][0, ...].values, carta_dim_order)
+    if parm_dict['complex_split'] == 'cartesian':
+        _write_fits(apertureheader, 'Complex aperture real part', transpoaper.real,
+                    basename + '_aperture_real.fits', 'Normalized', 'image')
+        _write_fits(apertureheader, 'Complex aperture imag part', transpoaper.imag,
+                    basename + '_aperture_imag.fits', 'Normalized', 'image')
+    else:
+        _write_fits(apertureheader, 'Complex aperture amplitude', np.absolute(transpoaper),
+                    basename + '_aperture_amplitude.fits', 'Normalized', 'image')
+        _write_fits(apertureheader, 'Complex aperture phase', np.angle(transpoaper),
+                    basename + '_aperture_phase.fits', 'rad', 'image')
+
+    phase_amp_header = _axis_to_fits_header(baseheader, inputxds.u_prime.values, 1, 'X', 'm')
+    phase_amp_header = _axis_to_fits_header(phase_amp_header, inputxds.v_prime.values, 2, 'Y', 'm')
+    transpoamp = np.transpose(inputxds['AMPLITUDE'][0, ...].values, carta_dim_order)
+    _write_fits(phase_amp_header, 'Cropped aperture amplitude', transpoamp, basename + '_amplitude.fits',
+                'Normalized', 'image')
+    transpopha = np.transpose(inputxds['CORRECTED_PHASE'][0, ...].values, carta_dim_order)
+    _write_fits(phase_amp_header, 'Cropped aperture corrected phase', transpopha, basename + '_corrected_phase.fits',
+                'rad', 'image')
+    return
```

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_imaging.py` & `astrohack-0.1.3/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_io.py` & `astrohack-0.1.3/src/astrohack/_utils/_io.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import json
 import zarr
 import copy
 import numpy as np
 import xarray as xr
+import datetime
 
 from astropy.io import fits
 from astrohack import __version__ as code_version
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._tools import _numpy_to_json
 
 DIMENSION_KEY = "_ARRAY_DIMENSIONS"
@@ -49,15 +50,15 @@
     """
     logger = _get_astrohack_logger()
     panel_data_dict = {}
 
     if panel_dict is not None:
             panel_data_dict = panel_dict
     
-    ant_list =  [dir_name for dir_name in os.listdir(file) if os.path.isdir(file)]
+    ant_list = [dir_name for dir_name in os.listdir(file) if os.path.isdir(file)]
     
     try:
         for ant in ant_list:
             if 'ant' in ant:
                 ddi_list =  [dir_name for dir_name in os.listdir(file + "/" + str(ant)) if os.path.isdir(file + "/" + str(ant))]
                 panel_data_dict[ant] = {}
                 
@@ -150,15 +151,14 @@
                         holog_dict[ddi][holog_map] = {}
                     for ant in os.listdir(os.path.join(holog_file, ddi + "/" + holog_map)):
                         if "ant_" in ant:
                             if (ant_id is None) or (ant_id in ant):
                                 mapping_ant_vis_holog_data_name = os.path.join(
                                     holog_file, ddi + "/" + holog_map + "/" + ant
                                 )
-                                
 
                                 if dask_load:
                                     holog_dict[ddi][holog_map][ant] = xr.open_zarr(
                                         mapping_ant_vis_holog_data_name
                                     )
                                 else:
                                     holog_dict[ddi][holog_map][ant] = _open_no_dask_zarr(mapping_ant_vis_holog_data_name)
@@ -191,25 +191,32 @@
                 if head["NAXIS" + str(iax + 1)] != 1:
                     raise Exception(filename + " is not bi-dimensional")
     if head["NAXIS1"] != head["NAXIS2"]:
         raise Exception(filename + " does not have the same amount of pixels in the x and y axes")
     return head, data
 
 
-def _write_fits(head, data, filename):
+def _write_fits(header, imagetype, data, filename, unit, origin):
     """
     Write a dictionary and a dataset to a FITS file
     Args:
-        head: The dictionary containing the header
+        header: The dictionary containing the header
+        imagetype: Type to be added to FITS header
         data: The dataset
         filename: The name of the output file
+        unit: to be set to bunit
     """
+
+    header['BUNIT'] = unit
+    header['TYPE'] = imagetype
+    header['ORIGIN'] = f'Astrohack v{code_version}: {origin}'
+    header['DATE'] = datetime.datetime.now().strftime('%b %d %Y, %H:%M:%S')
     hdu = fits.PrimaryHDU(data)
-    hdu.header = head
-    hdu.header["ORIGIN"] = "Astrohack"
+    for key in header.keys():
+        hdu.header.set(key, header[key])
     hdu.writeto(filename, overwrite=True)
     return
 
 
 def _aips_holog_to_xds(ampname, devname):
     """
     Read amplitude and deviation FITS files onto a common Xarray dataset
@@ -294,36 +301,89 @@
             return xr.open_zarr(image_path)
         else:
             return _open_no_dask_zarr(image_path)
     else:
         raise FileNotFoundError("Image file: {} not found".format(image_path))
 
 
-def _read_meta_data(file_name, file_type):
+def _read_meta_data(file_name, file_type, origin):
     """Reads dimensional data from holog meta file.
 
     Args:
         file_name (str): astorhack file name.
         file_type (str): astrohack file type
+        origin (str, list): Astrohack expected origin(s)
 
     Returns:
         dict: dictionary containing dimension data.
     """
     logger = _get_astrohack_logger()
     try:
         with open(f'{file_name}/.{file_type}_attr') as json_file:
             json_dict = json.load(json_file)
 
     except Exception as error:
         logger.error(str(error))
         raise
 
+    try:
+        metadataorigin = json_dict['origin']
+    except KeyError:
+        logger.error("[_read_meta_data]: Badly formatted metadata in input file")
+        raise Exception('Bad metadata')
+    if isinstance(origin, str):
+        if metadataorigin != origin:
+            logger.error(f"[_read_meta_data]: Input file is not an Astrohack {file_type} file")
+            logger.error(f"Expected origin was {origin} but got {metadataorigin}")
+            raise TypeError('Incorrect file type')
+    elif isinstance(origin, (list, tuple)):
+        if metadataorigin not in origin:
+            logger.error(f"[_read_meta_data]: Input file is not an Astrohack {file_type} file")
+            logger.error(f"Expected origin was {origin} but got {metadataorigin}")
+            raise TypeError('Incorrect file type')
+
     return json_dict
 
 
+def _check_mds_origin(file_name, file_type):
+    """
+
+    Args:
+        file_name(str): astrohack file name.
+        file_type(str, list): accepted astrohack file type
+
+    Returns: origin(str) the origin of the mds file
+
+    """
+    logger = _get_astrohack_logger()
+    if isinstance(file_type, str):
+        file_type = [file_type]
+
+    for ftype in file_type:
+        try:
+            with open(f'{file_name}/.{ftype}_attr') as json_file:
+                json_dict = json.load(json_file)
+                found = True
+        except FileNotFoundError:
+            found = False
+        if found:
+            break
+    if not found:
+        logger.error("[_check_mds_origin]: metadata not found")
+        raise Exception('Metadata not found')
+
+    try:
+        metadataorigin = json_dict['origin']
+    except KeyError:
+        logger.error("[_check_mds_origin]: Badly formatted metadata in input file")
+        raise Exception('Bad metadata')
+
+    return metadataorigin
+
+
 def _write_meta_data(origin, file_name, input_dict):
     """
     Creates a metadata dictionary that is compatible with JSON and writes it to a file
     Args:
         origin: Which function created the mds
         file_name: Output json file name
         input_dict: Dictionary to be included in the metadata
```

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.1.3/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_panel.py` & `astrohack-0.1.3/src/astrohack/_utils/_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,38 @@
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._algorithms import _least_squares_fit_block
 from astrohack._utils._constants import plot_types
 from astrohack._utils._io import _load_image_xds
 
 from astrohack._classes.telescope import Telescope
 from astrohack._classes.antenna_surface import AntennaSurface
+from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
 # global constants
 NPAR = 10
 
+
 def _panel_chunk(panel_chunk_params):
     """
     Process a chunk of the holographies, usually a chunk consists of an antenna over a ddi
     Args:
         panel_chunk_params: dictionary of inputs
     """
+    logger = _get_astrohack_logger()
     if panel_chunk_params['origin'] == 'AIPS':
         inputxds = xr.open_zarr(panel_chunk_params['image_name'])
         telescope = Telescope(inputxds.attrs['telescope_name'])
         panel_chunk_params['antenna'] = inputxds.attrs['ant_name']
 
     else:
-        inputxds = _load_image_xds(panel_chunk_params['image_name'],
-                                   panel_chunk_params['antenna'],
-                                   panel_chunk_params['ddi'],
-                                   dask_load=False)
+        ddi = panel_chunk_params['this_ddi']
+        antenna = panel_chunk_params['this_antenna']
+        inputxds = _load_image_xds(panel_chunk_params['image_name'], antenna, ddi, dask_load=False)
 
+        logger.info(f'[panel]: processing antenna {antenna} DDI {ddi}')
         inputxds.attrs['AIPS'] = False
 
         if inputxds.attrs['telescope_name'] == "ALMA":
             tname = inputxds.attrs['telescope_name']+'_'+inputxds.attrs['ant_name'][0:2]
             telescope = Telescope(tname)
         elif inputxds.attrs['telescope_name'] == "EVLA":
             tname = "VLA"
@@ -44,15 +47,15 @@
     surface = AntennaSurface(inputxds, telescope, panel_chunk_params['cutoff'], panel_chunk_params['panel_kind'],
                              panel_margins=panel_chunk_params['panel_margins'])
 
     surface.compile_panel_points()
     surface.fit_surface()
     surface.correct_surface()
     
-    xds_name = panel_chunk_params['panel_name'] + '/' + panel_chunk_params['antenna'] + '/' + panel_chunk_params['ddi']
+    xds_name = panel_chunk_params['panel_name'] + f'/{antenna}/{ddi}'
     xds = surface.export_xds()
     xds.to_zarr(xds_name, mode='w')
 
 
 def _create_phase_model(npix, parameters, wavelength, telescope, cellxy):
     """
     Create a phase model with npix by npix size according to the given parameters
@@ -69,14 +72,15 @@
     iNPARameters = _external_to_internal_parameters(parameters, wavelength, telescope, cellxy)
     dummyphase = np.zeros((npix, npix))
 
     _, model = _correct_phase(dummyphase, cellxy, iNPARameters, telescope.magnification, telescope.focus,
                               telescope.surp_slope)
     return model
 
+
 def _phase_fitting_block(pols, wavelength, telescope, cellxy, amplitude_image, phase_image, pointing_offset,
                          focus_xy_offsets, focus_z_offset, subreflector_tilt, cassegrain_offset):
     """
     Corrects the grading phase for pointing, focus, and feed offset errors using the least squares method, and a model
     incorporating subreflector position errors.  Includes reference pointing
 
     This is a revised version of the task, offering a two-reflector solution.  M. Kesteven, 6/12/1994
@@ -627,25 +631,64 @@
         for chan in range(nchan):
             for pol in range(npol):
                 rms[time, chan, pol] = np.sqrt(np.nanmean(phase_image[time, chan, pol] ** 2))
     return rms
 
 
 def _plot_antenna_chunk(parm_dict):
+    """
+    Chunk function for the user facing function plot_antenna
+    Args:
+        parm_dict: parameter dictionary
+    """
     antenna = parm_dict['this_antenna']
     ddi = parm_dict['this_ddi']
     destination = parm_dict['destination']
     plot_type = parm_dict['plot_type']
     basename = f'{destination}/{antenna}_{ddi}'
-    surface = parm_dict['panel_mds'].get_antenna(antenna, ddi)
+    surface = parm_dict['panel_mds'].get_antenna(antenna, ddi, dask_load=False)
     if plot_type == plot_types[0]:  # deviation plot
         surface.plot_deviation(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
     elif plot_type == plot_types[1]:  # phase plot
         surface.plot_phase(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
     elif plot_type == plot_types[2]:  # Ancillary plot
         surface.plot_mask(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
         surface.plot_amplitude(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
     else: # all plots
         surface.plot_deviation(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
         surface.plot_phase(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
         surface.plot_mask(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
         surface.plot_amplitude(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
+
+
+def _export_to_fits_panel_chunk(parm_dict):
+    """
+    Panel side chunk function for the user facing function export_to_fits
+    Args:
+        parm_dict: parameter dictionary
+    """
+    logger = _get_astrohack_logger()
+    antenna = parm_dict['this_antenna']
+    ddi = parm_dict['this_ddi']
+    destination = parm_dict['destination']
+    logger.info(f'Exporting panel contents of {antenna} {ddi} to FITS files in {destination}')
+    surface = parm_dict['panel_mds'].get_antenna(antenna, ddi, dask_load=False)
+    basename = f'{destination}/panel_{antenna}_{ddi}'
+    surface.export_to_fits(basename)
+    return
+
+
+def _export_screws_chunk(parm_dict):
+    """
+    Chunk function for the user facing function export_screws
+    Args:
+        parm_dict: parameter dictionary
+    """
+    antenna = parm_dict['this_antenna']
+    ddi = parm_dict['this_ddi']
+    export_name = parm_dict['destination'] + f'/screws_{antenna}_{ddi}.'
+    surface = parm_dict['panel_mds'].get_antenna(antenna, ddi, dask_load=False)
+    surface.export_screws(export_name + 'csv', unit=parm_dict['unit'])
+    if parm_dict['plot_map']:
+        surface.plot_screw_adjustments(export_name + 'png', unit=parm_dict['unit'], threshold=parm_dict['threshold'],
+                                       colormap=parm_dict['colormap'], figuresize=parm_dict['figuresize'],
+                                       dpi=parm_dict['dpi'])
```

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.1.3/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.1.3/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/astrohack_client.py` & `astrohack-0.1.3/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/combine.py` & `astrohack-0.1.3/src/astrohack/combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json` & `astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json` & `astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json` & `astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json` & `astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json` & `astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json` & `astrohack-0.1.3/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.1.3/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.1.3/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.1.3/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.1.3/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.1.3/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.1.3/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.1.3/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.1.3/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.1.3/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.1.3/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.1.3/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.1.3/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/dio.py` & `astrohack-0.1.3/src/astrohack/dio.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,219 @@
 import os
-import dask
 import numbers
 import numpy as np
 from matplotlib import colormaps as cmaps
 
 from casacore import tables
 
+from astrohack._utils._io import _check_mds_origin, check_if_file_exists
 from astrohack._utils._constants import length_units, trigo_units, plot_types
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._tools import _parm_to_list
+from astrohack._utils._dask_graph_tools import _generate_antenna_ddi_graph_and_compute
 
 from astrohack._utils._dio import AstrohackImageFile
 from astrohack._utils._dio import AstrohackHologFile
 from astrohack._utils._dio import AstrohackPanelFile
 from astrohack._utils._dio import AstrohackPointFile
 
-from astrohack._utils._panel import _plot_antenna_chunk
+from astrohack._utils._panel import _plot_antenna_chunk, _export_to_fits_panel_chunk, _export_screws_chunk
+from astrohack._utils._holog import _export_to_fits_holog_chunk
 
 
-def export_screws(panel_mds_name, destination, ant_name=None, ddi=None,  unit='mm', threshold=None, plot_map=False,
+def open_holog(file):
+    """ Open holog file and return instance of the holog data object. Object includes summary function to list available dictionary keys.
+
+    :param file: Path to holog file.
+    :type file: str
+  
+    :return: Holography holog object.
+    :rtype: AstrohackHologFile
+
+    .. _Description:
+    **AstrohackHologFile**
+    Holog object allows the user to access holog data via compound dictionary keys with values, in order of depth, `ddi` -> `map` -> `ant`. The holog object also provides a `summary()` helper function to list available keys for each file. An outline of the holog object structure is show below:
+
+    .. parsed-literal::
+        holog_mds =
+            {
+                ddi_0:{
+                    map_0:{
+                         ant_0: holog_ds,
+                             ⋮
+                         ant_n: holog_ds
+                    },
+                    ⋮
+                    map_p: …
+                },
+            ⋮
+            ddi_m: …
+            }
+    """
+
+    logger = _get_astrohack_logger()
+
+    _data_file = AstrohackHologFile(file=file)
+
+    if _data_file.open():
+        return _data_file
+
+    else:
+        logger.error(f"Error opening holgraphy file: {file}")
+
+
+def open_image(file):
+    """ Open image file and return instance of the image data object. Object includes summary function to list available dictionary keys.
+
+    :param file: Path to image file.
+    :type file: str
+  
+    :return: Holography image object.
+    :rtype: AstrohackImageFile
+
+    .. _Description:
+    **AstrohackImageFile**
+    Image object allows the user to access image data via compound dictionary keys with values, in order of depth, `ant` -> `ddi`. The image object also provides a `summary()` helper function to list available keys for each file. An outline of the image object structure is show below:
+
+    .. parsed-literal::
+       image_mds =
+           {
+               ant_0:{
+                   ddi_0: image_ds,
+                   ⋮
+                   ddi_m: image_ds
+               },
+               ⋮
+               ant_n: …
+           }
+
+    """
+
+    logger = _get_astrohack_logger()
+
+    _data_file = AstrohackImageFile(file=file)
+
+    if _data_file.open():
+        return _data_file
+
+    else:
+        logger.error(f"Error opening holgraphy image file: {file}")
+
+
+def open_panel(file):
+    """ Open panel file and return instance of the panel data object. Object includes summary function to list available dictionary keys.
+
+    :param file: Path ot panel file.
+    :type file: str
+  
+    :return: Holography panel object.
+    :rtype: AstrohackPanelFile
+
+    .. _Description:
+    **AstrohackPanelFile**
+    Panel object allows the user to access panel data via compound dictionary keys with values, in order of depth, `ant` -> `ddi`. The panel object also provides a `summary()` helper function to list available keys for each file. An outline of the panel object structure is show below:
+
+    .. parsed-literal::
+        panel_mds =
+            {
+                ant_0:{
+                    ddi_0: panel_ds,
+                    ⋮
+                    ddi_m: panel_ds
+                },
+                ⋮
+                ant_n: …
+            }
+
+    """
+
+    logger = _get_astrohack_logger()
+
+    _data_file = AstrohackPanelFile(file=file)
+
+    if _data_file.open():
+        return _data_file
+
+    else:
+        logger.error(f"Error opening holgraphy panel file: {file}")
+
+
+def open_pointing(file):
+    """ Open pointing file and return instance of the pointing data object. Object includes summary function to list available dictionary keys.
+
+    :param file: Path to pointing file.
+    :type file: str
+  
+    :return: Holography pointing object.
+    :rtype: AstrohackPointFile
+
+    .. _Description:
+
+    **AstrohackPointFile**
+    Pointing object allows the user to access pointing data via dictionary key with value based on `ant`. The pointing object also provides a `summary()` helper function to list available keys for each file. An outline of the pointing object structure is show below:
+
+    .. parsed-literal::
+        point_mds =
+            {
+                ant_0: point_ds,
+                ⋮
+                ant_n: point_ds
+            }
+
+    """
+
+    logger = _get_astrohack_logger()
+
+    _data_file = AstrohackPointFile(file=file)
+
+    if _data_file.open():
+        return _data_file
+
+    else:
+        logger.error(f"Error opening holgraphy pointing file: {file}")
+
+
+def fix_pointing_table(ms_name, reference_antenna):
+    """ Fix pointing table for a user defined subset of reference antennas.
+
+  Args:
+      ms_name (str): Measurement set.
+      reference_antenna (list): List of reference antennas.
+  """
+
+    ms_table = "/".join((ms_name, 'ANTENNA'))
+
+    query = 'select NAME from {table}'.format(table=ms_table)
+
+    ant_names = np.array(tables.taql(query).getcol('NAME'))
+    ant_id = np.arange(len(ant_names))
+
+    query_ant = np.searchsorted(ant_names, reference_antenna)
+
+    ms_table = "/".join((ms_name, 'POINTING'))
+
+    ant_list = " or ".join(["ANTENNA_ID=={ant}".format(ant=ant) for ant in query_ant])
+
+    update = "update {table} set POINTING_OFFSET=0, TARGET=DIRECTION where {antennas}".format(table=ms_table,
+                                                                                              antennas=ant_list)
+
+    tables.taql(update)
+
+    ms_table = "/".join((ms_name, "HISTORY"))
+    tb = tables.table(ms_table, readonly=False)
+
+    message = tb.getcol("MESSAGE")
+
+    if "pnt_tbl:fixed" not in message:
+        tb.addrows(nrows=1)
+        length = len(message)
+        tb.putcol(columnname="MESSAGE", value='pnt_tbl:fixed', startrow=length)
+
+
+def export_screws(panel_mds_name, destination, ant_name=None, ddi=None, unit='mm', threshold=None, plot_map=False,
                   colormap='seismic', figuresize=None, dpi=300):
     """ Export screw adjustment from panel to text file and save to disk.
 
     :param panel_mds_name: Input panel_mds file
     :type panel_mds_name: str
     :param destination: Name of the destination folder to contain exported screw adjustments
     :type destination: str
@@ -76,35 +266,24 @@
                                                  default='None', log_default_setting=False)
     parms_passed = parms_passed and _check_parms(parm_dict, 'dpi', [int], default=300)
 
     if not parms_passed:
         logger.error("export_screws parameter checking failed.")
         raise Exception("export_screws parameter checking failed.")
 
+    check_if_file_exists(panel_mds_name)
     panel_mds = AstrohackPanelFile(panel_mds_name)
     panel_mds.open()
 
     try:
         os.mkdir(parm_dict['destination'])
     except FileExistsError:
         logger.warning('Destination folder already exists, results may be overwritten')
 
-    antennae = _parm_to_list(parm_dict['ant_name'], parm_dict['filename'])
-    for antenna in antennae:
-        if 'ant' in antenna:
-            ddis = _parm_to_list(parm_dict['ddi'], parm_dict['filename']+'/'+antenna)
-            for ddi in ddis:
-                if 'ddi' in ddi:
-                    export_name = parm_dict['destination']+f'/screws_{antenna}_{ddi}.'
-                    surface = panel_mds.get_antenna(antenna, ddi)
-                    surface.export_screws(export_name+'csv', unit=unit)
-                    if parm_dict['plot_map']:
-                        surface.plot_screw_adjustments(export_name+'png', unit=unit, threshold=parm_dict['threshold'],
-                                                       colormap=parm_dict['colormap'], figuresize=parm_dict['figuresize'],
-                                                       dpi=parm_dict['dpi'])
+    _generate_antenna_ddi_graph_and_compute('export_screws', _export_screws_chunk, parm_dict, False)
 
 
 def plot_antenna(panel_mds_name, destination, ant_name=None, ddi=None, plot_type='deviation', plot_screws=False,
                  unit=None, colormap='viridis', figuresize=None, dpi=300, parallel=True):
     """ Create diagnostic plots of antenna surface deviations from panel data file. Available plots listed in additional information.
 
     :param panel_mds_name: Input panel_mds file
@@ -138,17 +317,17 @@
         .. rubric:: Available plot types:
         - *deviation*: Surface deviation estimated from phase and wavelength, three plots are produced for each antenna
                        and ddi combination, surface before correction, the corrections applied and the corrected
                        surface, most length units available
         - *phase*: Phase deviations over the surface, three plots are produced for each antenna and ddi combination,
                    phase before correction, the corrections applied and the corrected phase, deg and rad available as
                    units
-        - *ancillary*: Three ancillary plots with useful information: The mask used to select data to be fitted, the
-                       amplitude data used to derive the mask and the panel assignments of each pixel, units are
-                       irrelevant for these plots
+        - *ancillary*: Two ancillary plots with useful information: The mask used to select data to be fitted, the
+                       amplitude data used to derive the mask, units are irrelevant for these plots
+        - *all*: All the plots listed above
     """
     logger = _get_astrohack_logger()
     parm_dict = {'filename': panel_mds_name,
                  'ant_name': ant_name,
                  'ddi': ddi,
                  'destination': destination,
                  'unit': unit,
@@ -183,217 +362,97 @@
                                                  default='None', log_default_setting=False)
     parms_passed = parms_passed and _check_parms(parm_dict, 'dpi', [int], default=300)
 
     if not parms_passed:
         logger.error("plot_antenna parameter checking failed.")
         raise Exception("plot_antenna parameter checking failed.")
 
+    check_if_file_exists(panel_mds_name)
     panel_mds = AstrohackPanelFile(panel_mds_name)
     panel_mds.open()
     parm_dict['panel_mds'] = panel_mds
 
     try:
         os.mkdir(parm_dict['destination'])
     except FileExistsError:
         logger.warning('Destination folder already exists, results may be overwritten')
 
-    delayed_list = []
-    antennae = _parm_to_list(parm_dict['ant_name'], parm_dict['filename'])
-    for antenna in antennae:
-        if 'ant' in antenna:
-            parm_dict['this_antenna'] = antenna
-            ddis = _parm_to_list(parm_dict['ddi'], parm_dict['filename']+'/'+antenna)
-            for ddi in ddis:
-                if 'ddi' in ddi:
-                    parm_dict['this_ddi'] = ddi
-                    if parallel:
-                        delayed_list.append(dask.delayed(_plot_antenna_chunk)(dask.delayed(parm_dict)))
-                    else:
-                        _plot_antenna_chunk(parm_dict)
-
-    if parallel:
-        dask.compute(delayed_list)
-
-def open_holog(file):
-  """ Open holog file and return instance of the holog data object. Object includes summary function to list available dictionary keys.
+    _generate_antenna_ddi_graph_and_compute('plot_antenna', _plot_antenna_chunk, parm_dict, parallel)
 
-  :param file: Path to holog file.
-  :type file: str
-  
-  :return: Holography holog object.
-  :rtype: AstrohackHologFile
 
-  .. _Description:
-  **AstrohackHologFile**
-  Holog object allows the user to access holog data via compound dictionary keys with values, in order of depth, `ddi` -> `map` -> `ant`. The holog object also provides a `summary()` helper function to list available keys for each file. An outline of the holog object structure is show below:
-
-  .. parsed-literal::
-    holog_mds = 
-      {
-      ddi_0:{
-          map_0:{
-                 ant_0: holog_ds,
-                          ⋮
-                 ant_n: holog_ds
-                },
-              ⋮
-          map_p: …
-         },
-       ⋮
-      ddi_m: …
-    }
-
-  """
-
-  logger = _get_astrohack_logger()
-
-  _data_file = AstrohackHologFile(file=file)
-  
-  if _data_file.open():
-    return _data_file
+def export_to_fits(mds_name, destination, complex_split='cartesian', ant_name=None, ddi=None, parallel=True):
+    """ Export contents of an Astrohack MDS file to several FITS files in the destination folder
 
-  else:
-    logger.error("Error opening holgraphy file: {file}".format(file))
-
-def open_image(file):
-  """ Open image file and return instance of the image data object. Object includes summary function to list available dictionary keys.
-
-  :param file: Path to image file.
-  :type file: str
-  
-  :return: Holography image object.
-  :rtype: AstrohackImageFile
-
-  .. _Description:
-  **AstrohackImageFile**
-  Image object allows the user to access image data via compound dictionary keys with values, in order of depth, `ant` -> `ddi`. The image object also provides a `summary()` helper function to list available keys for each file. An outline of the image object structure is show below:
-
-  .. parsed-literal::
-    image_mds = 
-      {
-        ant_0:{
-          ddi_0: image_ds,
-                 ⋮               
-          ddi_m: image_ds
-         },
-        ⋮
-        ant_n: …
-      }
-
-  """
-
-  logger = _get_astrohack_logger()
-
-  _data_file = AstrohackImageFile(file=file)
-  
-  if _data_file.open():
-    return _data_file
-
-  else:
-    logger.error("Error opening holgraphy image file: {file}".format(file))
-
-def open_panel(file):
-  """ Open panel file and return instance of the panel data object. Object includes summary function to list available dictionary keys.
-
-  :param file: Path ot panel file.
-  :type file: str
-  
-  :return: Holography panel object.
-  :rtype: AstrohackPanelFile
-
-  .. _Description:
-  **AstrohackPanelFile**
-  Panel object allows the user to access panel data via compound dictionary keys with values, in order of depth, `ant` -> `ddi`. The panel object also provides a `summary()` helper function to list available keys for each file. An outline of the panel object structure is show below:
-
-  .. parsed-literal::
-    panel_mds = 
-      {
-        ant_0:{
-          ddi_0: panel_ds,
-                 ⋮               
-          ddi_m: panel_ds
-         },
-        ⋮
-        ant_n: …
-      }
-
-  """
-
-  logger = _get_astrohack_logger()
-
-  _data_file = AstrohackPanelFile(file=file)
-  
-  if _data_file.open():
-    return _data_file
-
-  else:
-    logger.error("Error opening holgraphy panel file: {file}".format(file))
-
-def open_pointing(file):
-  """ Open pointing file and return instance of the pointing data object. Object includes summary function to list available dictionary keys.
-
-  :param file: Path to pointing file.
-  :type file: str
-  
-  :return: Holography pointing object.
-  :rtype: AstrohackPointFile
-
-  .. _Description:
-
-  **AstrohackPointFile**
-  Pointing object allows the user to access pointing data via dictionary key with value based on `ant`. The pointing object also provides a `summary()` helper function to list available keys for each file. An outline of the pointing object structure is show below:
-
-  .. parsed-literal::
-    point_mds = 
-      {
-        ant_0: point_ds,
-            ⋮
-        ant_n: point_ds
-      }
-
-
-  """
-
-  logger = _get_astrohack_logger()
+    :param mds_name: Input panel_mds file
+    :type mds_name: str
+    :param destination: Name of the destination folder to contain plots
+    :type destination: str
+    :param complex_split: How to split complex data, cartesian (real + imaginary) or polar (amplitude + phase)
+    :type complex_split: str
+    :param ant_name: List of antennae/antenna to be plotted, defaults to "all" when None
+    :type ant_name: list or str, optional, ex. ant_ea25
+    :param ddi: List of ddis/ddi to be plotted, defaults to "all" when None
+    :type ddi: list or str, optional, ex. ddi_0
+    :param parallel: If True will use an existing astrohack client to produce plots in parallel
+    :type parallel: bool
 
-  _data_file = AstrohackPointFile(file=file)
-  
-  if _data_file.open():
-    return _data_file
+    .. _Description:
+    Export the products from either holog or panel onto FITS files to be read by other software packages
 
-  else:
-    logger.error("Error opening holgraphy pointing file: {file}".format(file))
+    **Additional Information**
+    The image products of holog are complex images due to the nature of interferometric measurements and Fourier
+    transforms, currently complex128 FITS files are not supported by astropy, hence the need to split complex images
+    onto two real image products, we present the user with two options to carry out this split.
 
-def fix_pointing_table(ms_name, reference_antenna):
-  """ Fix pointing table for a user defined subset of reference antennas.
+        .. rubric:: Available complex splitting possibilities:
+        - *cartesian*: Split is done to a real part and an imaginary part FITS files
+        - *polar*:     Split is done to an amplitude and a phase FITS files
 
-  Args:
-      ms_name (str): Measurement set.
-      reference_antenna (list): List of reference antennas.
-  """
-    
-  ms_table = "/".join((ms_name, 'ANTENNA'))
 
-  query = 'select NAME from {table}'.format(table=ms_table)
+    The FITS produced by this function have been tested are known to work with CARTA and DS9
+    """
 
-  ant_names = np.array(tables.taql(query).getcol('NAME'))
-  ant_id = np.arange(len(ant_names))
+    logger = _get_astrohack_logger()
+    parm_dict = {'filename': mds_name,
+                 'ant_name': ant_name,
+                 'ddi': ddi,
+                 'destination': destination,
+                 'complex_split': complex_split,
+                 'parallel': parallel}
 
-  query_ant = np.searchsorted(ant_names, reference_antenna)
+    parms_passed = _check_parms(parm_dict, 'filename', [str], default=None)
+    parms_passed = parms_passed and _check_parms(parm_dict, 'complex_split', [str],
+                                                 acceptable_data=['cartesian', 'polar'], default="cartesian")
+    parms_passed = parms_passed and _check_parms(parm_dict, 'ant_name', [list], list_acceptable_data_types=[str],
+                                                 default='all')
+    parms_passed = parms_passed and _check_parms(parm_dict, 'ddi', [list], list_acceptable_data_types=[str],
+                                                 default='all')
+    parms_passed = parms_passed and _check_parms(parm_dict, 'destination', [str], default=None)
+    parms_passed = parms_passed and _check_parms(parm_dict, 'parallel', [bool], default=True)
 
-  ms_table = "/".join((ms_name, 'POINTING'))
+    if not parms_passed:
+        logger.error("export_screws parameter checking failed.")
+        raise Exception("export_screws parameter checking failed.")
 
-  ant_list = " or ".join(["ANTENNA_ID=={ant}".format(ant=ant) for ant in query_ant])
+    check_if_file_exists(mds_name)
+    mds_origin = _check_mds_origin(mds_name, ['image', 'panel', 'point', 'holog'])
 
-  update = "update {table} set POINTING_OFFSET=0, TARGET=DIRECTION where {antennas}".format(table=ms_table, antennas=ant_list)
+    if mds_origin in ['combine', 'holog']:
+        chunk_function = _export_to_fits_holog_chunk
+        holog_mds = AstrohackImageFile(mds_name)
+        holog_mds.open()
+        parm_dict['holog_mds'] = holog_mds
+    elif mds_origin == 'panel':
+        chunk_function = _export_to_fits_panel_chunk
+        panel_mds = AstrohackPanelFile(mds_name)
+        panel_mds.open()
+        parm_dict['panel_mds'] = panel_mds
+    else:
+        logger.error(f"Cannot export mds_files created by {mds_origin} to FITS")
+        return
 
-  tables.taql(update)
+    try:
+        os.mkdir(parm_dict['destination'])
+    except FileExistsError:
+        logger.warning('Destination folder already exists, results may be overwritten')
 
-  ms_table = "/".join((ms_name, "HISTORY"))
-  tb = tables.table(ms_table, readonly=False)
-    
-  message = tb.getcol("MESSAGE")
-    
-  if "pnt_tbl:fixed" not in message:
-    tb.addrows(nrows=1)
-    length = len(message)
-    tb.putcol(columnname="MESSAGE", value='pnt_tbl:fixed', startrow=length)
+    _generate_antenna_ddi_graph_and_compute('export_to_fits', chunk_function, parm_dict, parallel)
```

### Comparing `astrohack-0.1.2/src/astrohack/extract_holog.py` & `astrohack-0.1.3/src/astrohack/extract_holog.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,26 +30,26 @@
 from astrohack._utils._extract_holog import _extract_holog_chunk
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
 
 from astrohack._utils._tools import _remove_suffix
 from astrohack._utils._tools import _jsonify
-from astrohack._utils._tools import _print_holog_obs_dict
 
 from astrohack._utils._dio import AstrohackHologFile
 
 def extract_holog(
     ms_name,
     holog_obs_dict=None,
     ddi_sel=None,
     baseline_average_distance=None,
+    baseline_average_nearest=None,
     holog_name=None,
     point_name=None,
-    data_col="DATA",
+    data_column="DATA",
     parallel=False,
     reuse_point_zarr=False,
     overwrite=False,
 ):
     """
     Extract holography and optionally pointing data, from measurement set. Creates holography output file.
 
@@ -58,25 +58,28 @@
 
     :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set. If not specified holog_obs_dict will be generated. For auto generation of the holog_obs_dict the assumtion is made that the same antanna beam is not mapped twice in a row (alternating sets of antennas is fine).
     :type holog_obs_dict: dict, optional
     
     :param ddi_sel:  Value(s) of DDI that should be extracted from the measurement set. Defaults to all DDI's in the ms.
     :type ddi_sel: int numpy.ndarray | int list, optional
        
-    :param baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used.
+    :param baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used. baseline_average_distance and baseline_average_nearest can not be used together.
     :type holog_obs_dict: float, optional
+    
+    :param baseline_average_nearest: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_nearest is the number of nearest reference antennas to use. The baseline_average_nearest is only used if the holog_obs_dict is not specified.  baseline_average_distance and baseline_average_nearest can not be used together.
+    :type holog_obs_dict: int, optional
 
     :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
     :type holog_name: str, optional
 
     :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
     :type point_name: str, optional
 
-    :param data_col: Determines the data column to pull from the measurement set. Defaults to "DATA"
-    :type data_col: str, optional, ex. DATA, CORRECTED_DATA
+    :param data_column: Determines the data column to pull from the measurement set. Defaults to "CORRECTED_DATA"
+    :type data_column: str, optional, ex. DATA, CORRECTED_DATA
 
     :param parallel: Boolean for whether to process in parallel. Defaults to False
     :type parallel: bool, optional
     
     :param reuse_point_zarr: If true the point.zarr specified in point_name is reused.
     :type reuse_point_zarr: bool, optional
 
@@ -153,29 +156,34 @@
     
     
     ######### Parameter Checking #########
     extract_holog_parms = _check_extract_holog_parms(ms_name,
                                 holog_obs_dict,
                                 ddi_sel,
                                 baseline_average_distance,
+                                baseline_average_nearest,
                                 holog_name,
                                 point_name,
-                                data_col,
+                                data_column,
                                 parallel,
                                 reuse_point_zarr,
                                 overwrite)
     input_params = extract_holog_parms.copy()
     
     check_if_file_exists(extract_holog_parms['ms_name'])
     check_if_file_will_be_overwritten(extract_holog_parms['holog_name'],extract_holog_parms['overwrite'])
     check_if_file_will_be_overwritten(extract_holog_parms['point_name'],extract_holog_parms['overwrite'])
         
     ############# Exstract pointing infromation and save to point.zarr #############
     if extract_holog_parms["reuse_point_zarr"]:
-        pnt_dict = _load_point_file(extract_holog_parms['point_name'])
+        try:
+            pnt_dict = _load_point_file(extract_holog_parms['point_name'])
+        except:
+            logger.warning('Could not find ' + extract_holog_parms['point_name'] + ', creating point new point.zarr .')
+            pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
     else:
         pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
 
     ######## Get Spectral Windows ########
     ctb = ctables.table(
         os.path.join(extract_holog_parms['ms_name'], "DATA_DESCRIPTION"),
         readonly=True,
@@ -217,15 +225,15 @@
     ant_names_main = ant_names[ant_id_main]
     ctb.close()
     
     # Create holog_obs_dict or modify user supplied holog_obs_dict.
     ddi_sel = extract_holog_parms['ddi_sel']
     if holog_obs_dict is None: #Automatically create holog_obs_dict
         from astrohack._utils._extract_holog import _create_holog_obs_dict
-        holog_obs_dict = _create_holog_obs_dict(pnt_dict, extract_holog_parms['baseline_average_distance'],ant_names,ant_pos,ant_names_main)
+        holog_obs_dict = _create_holog_obs_dict(pnt_dict, extract_holog_parms['baseline_average_distance'], extract_holog_parms['baseline_average_nearest'], ant_names,ant_pos,ant_names_main)
         
         #From the generated holog_obs_dict subselect user supplied ddis.
         if ddi_sel != 'all':
             holog_obs_dict_keys = list(holog_obs_dict.keys())
             for ddi_key in holog_obs_dict_keys:
                 if 'ddi' in ddi_key:
                     ddi_id = int(ddi_key.replace('ddi_',''))
@@ -239,15 +247,16 @@
                 holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
         else:
             for ddi_id in ddi_sel:
                 holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
         
         holog_obs_dict = holog_obs_dict_with_ddi
             
-    _print_holog_obs_dict(holog_obs_dict)
+    from pprint import pformat
+    logger.info("holog_obs_dict: \n%s", pformat(list(holog_obs_dict.values())[0],indent=2,width=2))
 
 
     outfile_obj = copy.deepcopy(holog_obs_dict)
 
     _jsonify(outfile_obj)
 
     with open(".holog_obs_dict.json", "w") as outfile:
@@ -414,31 +423,33 @@
 
 
 def _check_extract_holog_parms(
     ms_name,
     holog_obs_dict,
     ddi_sel,
     baseline_average_distance,
+    baseline_average_nearest,
     holog_name,
     point_name,
-    data_col,
+    data_column,
     parallel,
     reuse_point_zarr,
     overwrite):
     
     extract_holog_parms = {}
     extract_holog_parms["ms_name"] = ms_name
     extract_holog_parms["holog_name"] = holog_name
     extract_holog_parms["ddi_sel"] = ddi_sel
     extract_holog_parms["point_name"] = point_name
-    extract_holog_parms["data_col"] = data_col
+    extract_holog_parms["data_column"] = data_column
     extract_holog_parms["parallel"] = parallel
     extract_holog_parms["overwrite"] = overwrite
     extract_holog_parms["reuse_point_zarr"] = reuse_point_zarr
     extract_holog_parms["baseline_average_distance"] = baseline_average_distance
+    extract_holog_parms["baseline_average_nearest"] = baseline_average_nearest
 
     
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
     parms_passed = parms_passed and _check_parms(extract_holog_parms, 'ms_name', [str],default=None)
@@ -454,17 +465,23 @@
   
     #To Do: special function needed to check holog_obs_dict.
     parm_check = isinstance(holog_obs_dict,dict) or (holog_obs_dict is None)
     parms_passed = parms_passed and parm_check
     if not parm_check:
         logger.error('Parameter holog_obs_dict must be of type '+ str(dict))
         
-    parms_passed = parms_passed and _check_parms(extract_holog_parms,'baseline_average_distance', [numbers.Number],default='all')
-        
-    parms_passed = parms_passed and _check_parms(extract_holog_parms,'data_col', [str],default='DATA')
+    parms_passed = parms_passed and _check_parms(extract_holog_parms,'baseline_average_distance',[numbers.Number],default='all')
+    
+    parms_passed = parms_passed and _check_parms(extract_holog_parms,'baseline_average_nearest',[int], default='all')
+    
+    if (extract_holog_parms['baseline_average_distance'] != 'all') and (extract_holog_parms['baseline_average_nearest'] != 'all'):
+        logger.error('baseline_average_distance: ' + str(baseline_average_distance ) + ' and baseline_average_nearest: ' + str(baseline_average_distance ) + ' can not both be specified.')
+        parms_passed = False
+ 
+    parms_passed = parms_passed and _check_parms(extract_holog_parms,'data_column', [str],default='CORRECTED_DATA')
 
     parms_passed = parms_passed and _check_parms(extract_holog_parms, 'parallel', [bool],default=False)
     
     parms_passed = parms_passed and _check_parms(extract_holog_parms, 'reuse_point_zarr', [bool],default=False)
 
     parms_passed = parms_passed and _check_parms(extract_holog_parms, 'overwrite', [bool],default=False)
```

### Comparing `astrohack-0.1.2/src/astrohack/gdown_utils.py` & `astrohack-0.1.3/src/astrohack/gdown_utils.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/holog.py` & `astrohack-0.1.3/src/astrohack/holog.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 def holog(
     holog_name,
     grid_size=None,
     cell_size=None,
     image_name=None,
     padding_factor=50,
-    grid_interpolation_mode="nearest",
+    grid_interpolation_mode="linear",
     chan_average=True,
     chan_tolerance_factor=0.005,
     scan_average=True,
     ant_list=None,
     to_stokes=True,
     apply_mask=True,
     phase_fit=True,
@@ -48,15 +48,15 @@
 
     :param padding_factor: Padding factor applied to beam grid before computing the fast-fourier transform. The default has been set for operation on most systems. The user should be aware of memory constraints before increasing this parameter significatly., defaults to 50
     :type padding_factor: int, optional
 
     :param parallel: Run in parallel with Dask or in serial., defaults to True
     :type parallel: bool, optional
 
-    :param grid_interpolation_mode: Method of interpolation used when gridding data. This is done using the `scipy.interpolate.griddata` method. For more information on the interpolation see `scipy.interploate <https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.griddata.html#scipy.interpolate.griddata>`_, defaults to "nearest"
+    :param grid_interpolation_mode: Method of interpolation used when gridding data. This is done using the `scipy.interpolate.griddata` method. For more information on the interpolation see `scipy.interploate <https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.griddata.html#scipy.interpolate.griddata>`_, defaults to "linear"
     :type grid_interpolation_mode: str, optional. Available options: {"linear", "nearest", "cubic"} 
 
     :param chan_average: Boolean dictating whether the channel average is computed and written to the output holog file., defaults to True
     :type chan_average: bool, optional
 
     :param chan_tolerance_factor: Tolerance used in channel averaging to determine the number of primary beam channels., defaults to 0.005
     :type chan_tolerance_factor: float, optional
@@ -133,41 +133,39 @@
     
     check_if_file_exists(holog_params['holog_file'])
     check_if_file_will_be_overwritten(holog_params['image_file'],holog_params['overwrite'])
 
     json_data = "/".join((holog_params['holog_file'], ".holog_json"))
     with open(json_data, "r") as json_file:
         holog_json = json.load(json_file)
-    meta_data = _read_meta_data(holog_params['holog_file'], 'holog')
+    meta_data = _read_meta_data(holog_params['holog_file'], 'holog', 'extract_holog')
 
     if  holog_params['ant_list'] == 'all':
         holog_params['ant_list'] = list(holog_json.keys())
         
     logger.info('Mapping antennas ' + str(holog_params['ant_list']))
 
+    if (holog_params["cell_size"] is None):
+        cell_size = np.array([-meta_data["cell_size"], meta_data["cell_size"]])
+        holog_params["cell_size"] = cell_size
     
-    if (cell_size is None) and (grid_size is None):
+    if  (holog_params["grid_size"] is None):
         n_pix = int(np.sqrt(meta_data["n_pix"]))
         grid_size = np.array([n_pix, n_pix])
-        cell_size = np.array([-meta_data["cell_size"], meta_data["cell_size"]])
-
-        holog_params["cell_size"] = cell_size
-        holog_params["grid_size"] = grid_size
-        
-        logger.info("Cell size: " + str(cell_size) + " Grid size " + str(grid_size))
-    else:
-        holog_params["cell_size"] = cell_size
         holog_params["grid_size"] = grid_size
     
     
+    logger.info("Cell size: " + str(cell_size) + " Grid size " + str(grid_size))
     json_data = {
-            "cell_size": list(map(float, cell_size)),
-            "grid_size": list(map(float, grid_size))
+            "cell_size": holog_params["cell_size"].tolist(),
+            "grid_size": holog_params["grid_size"].tolist()
     }
-
+    
+    print(holog_params["grid_size"])
+    
     with open(".holog_diagnostic.json", "w") as out_file:
         json.dump(json_data, out_file)
 
     
     holog_chunk_params =  holog_params
     delayed_list = []
     
@@ -222,21 +220,25 @@
     
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
     parms_passed = parms_passed and _check_parms(holog_params, 'holog_file', [str],default=None)
 
-    parms_passed = parms_passed and _check_parms(holog_params, 'grid_size', [list, np.ndarray], list_acceptable_data_types=[np.int64, np.int64], list_len=2, default='None',log_default_setting=False)
-    if (isinstance(holog_params['grid_size'],str)) and (holog_params['grid_size'] == 'None'): holog_params['grid_size'] =  None
-    holog_params['grid_size'] = np.array(holog_params['grid_size'])
+    parms_passed = parms_passed and _check_parms(holog_params, 'grid_size', [list, np.ndarray], list_acceptable_data_types=[np.int64, int], list_len=2, default='None',log_default_setting=False)
+    if (isinstance(holog_params['grid_size'],str)) and (holog_params['grid_size'] == 'None'):
+        holog_params['grid_size'] =  None
+    else:
+        holog_params['grid_size'] = np.array(holog_params['grid_size'])
 
     parms_passed = parms_passed and _check_parms(holog_params, 'cell_size', [list,np.ndarray], list_acceptable_data_types=[numbers.Number], list_len=2, default='None',log_default_setting=False)
-    if (isinstance(holog_params['cell_size'],str)) and (holog_params['cell_size'] == 'None'): holog_params['cell_size'] =  None
-    holog_params['cell_size'] = np.array(holog_params['cell_size'])
+    if (isinstance(holog_params['cell_size'],str)) and (holog_params['cell_size'] == 'None'):
+        holog_params['cell_size'] =  None
+    else:
+        holog_params['cell_size'] = np.array(holog_params['cell_size'])
 
     
     base_name = _remove_suffix(holog_params['holog_file'],'.holog.zarr')
     parms_passed = parms_passed and _check_parms(holog_params,'image_file', [str],default=base_name+'.image.zarr')
     parms_passed = parms_passed and _check_parms(holog_params, 'padding_factor', [int], default=50)
     parms_passed = parms_passed and _check_parms(holog_params, 'parallel', [bool],default=False)
     parms_passed = parms_passed and _check_parms(holog_params,'grid_interpolation_mode', [str],acceptable_data=["nearest","linear","cubic"],default="nearest")
```

### Comparing `astrohack-0.1.2/src/astrohack/panel.py` & `astrohack-0.1.3/src/astrohack/panel.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,35 +6,39 @@
 
 from astrohack._classes.base_panel import panel_models
 from astrohack._utils._io import _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
 from astrohack._utils._panel import _panel_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._tools import _remove_suffix
+from astrohack._utils._dask_graph_tools import _generate_antenna_ddi_graph_and_compute
 
 from astrohack._utils._dio import AstrohackPanelFile
 
 
-def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, parallel=False, sel_ddi=None, overwrite=False):
+def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, ant_name=None, ddi=None,
+          parallel=False, overwrite=False):
     """Analyze holography images to derive panel adjustments
 
     :param image_name: Input holography data file name. Accepted data formats are the output from ``astrohack.holog.holog`` and AIPS holography data prepackaged using ``astrohack.panel.aips_holog_to_astrohack``.
     :type image_name: str
     :param panel_name: Name of output file; File name will be appended with suffix *.panel.zarr*. Defaults to *basename* of input file plus holography panel file suffix.
     :type panel_name: str, optional
     :param cutoff: Relative amplitude cut-off which defines fitting mask. Defaults to 0.2.
     :type cutoff: float, optional
     :param panel_model: Model of surface fitting function used to fit panel surfaces, None will default to "rigid". Possible models are listed below.
     :type panel_model: str, optional
     :param panel_margins: Relative margin from the edge of the panel used to decide which points are margin points or internal points of each panel. Defaults to 0.2.
     :type panel_margins: float, optional
     :param parallel: Run in parallel. Defaults to False.
     :type parallel: bool, optional
-    :param sel_ddi: List of DDIs to be processed. None will use all DDIs. Defaults to None.
-    :type sel_ddi: list, optional, ex. [ddi_0 ... ddi_N]
+    :param ant_name: List of antennae to be processed. None will use all antennae. Defaults to None.
+    :type ant_name: list, optional, ex. [ant_ea25 ... ant_ea06]
+    :param ddi: List of DDIs to be processed. None will use all DDIs. Defaults to None.
+    :type ddi: list, optional, ex. [ddi_0 ... ddi_N]
     :param overwrite: Overwrite files on disk. Defaults to False.
     :type overwrite: bool, optional
 
     :return: Holography panel object.
     :rtype: AstrohackPanelFile
 
     .. _Description:
@@ -86,60 +90,38 @@
             ant_n: …
         }
 
     """
     
     logger = _get_astrohack_logger()
     
-    panel_params = _check_panel_parms(image_name, panel_name, cutoff, panel_model, panel_margins, parallel, sel_ddi,
-                                      overwrite)
+    panel_params = _check_panel_parms(image_name, panel_name, cutoff, panel_model, panel_margins, ant_name, ddi,
+                                      parallel, overwrite)
     input_params = panel_params.copy()
-          
+    # Doubled this entry for compatibility with the factorized antenna ddi loop
+    panel_params['filename'] = panel_params['image_name']
     check_if_file_exists(panel_params['image_name'])
     check_if_file_will_be_overwritten(panel_params['panel_name'], panel_params['overwrite'])
 
     if os.path.exists(panel_params['image_name']+'/.aips'):
         panel_params['origin'] = 'AIPS'
         _panel_chunk(panel_params)
 
     else:
-        panel_chunk_params = panel_params
-        panel_chunk_params['origin'] = 'astrohack'
-        delayed_list = []
-
-        antennae = os.listdir(panel_chunk_params['image_name'])
-        count = 0
-        for antenna in antennae:
-            if 'ant_' in antenna:
-                panel_chunk_params['antenna'] = antenna
-                
-                if panel_chunk_params['sel_ddi'] == "all":
-                    panel_chunk_params['sel_ddi'] = os.listdir(panel_chunk_params['image_name']+'/'+antenna)
-
-                for ddi in panel_chunk_params['sel_ddi']:
-                    if 'ddi_' in ddi:
-                        logger.info(f"Processing {ddi} for {antenna}")
-                        panel_chunk_params['ddi'] = ddi
-                        if parallel:
-                            delayed_list.append(dask.delayed(_panel_chunk)(dask.delayed(panel_chunk_params)))
-                        else:
-                            _panel_chunk(panel_chunk_params)
-                        count += 1
-        if parallel:
-            dask.compute(delayed_list)
-
+        panel_params['origin'] = 'astrohack'
+        count = _generate_antenna_ddi_graph_and_compute('panel', _panel_chunk, panel_params, parallel)
         if count == 0:
             logger.warning("No data to process")
             return None
         else:
-            logger.info("Panel finished processing")
+            logger.info("[panel] Finished processing")
 
-            output_attr_file = "{name}/{ext}".format(name=panel_chunk_params['panel_name'], ext=".panel_attr")
+            output_attr_file = "{name}/{ext}".format(name=panel_params['panel_name'], ext=".panel_attr")
             _write_meta_data('panel', output_attr_file, input_params)
-            panel_mds = AstrohackPanelFile(panel_chunk_params['panel_name'])
+            panel_mds = AstrohackPanelFile(panel_params['panel_name'])
             panel_mds.open()
             return panel_mds
 
 
 def aips_holog_to_astrohack(amp_image, dev_image, telescope_name, holog_name, overwrite=False):
     """
     Package AIPS HOLOG products in a .image.zarr file compatible with astrohack.panel.panel
@@ -165,53 +147,60 @@
     if os.path.exists(holog_name):
         shutil.rmtree(holog_name, ignore_errors=False, onerror=None)
     xds.to_zarr(holog_name, mode='w', compute=True, consolidated=True)
     aips_mark = open(holog_name+'/.aips', 'w')
     aips_mark.close()
 
 
-def _check_panel_parms(image_name, panel_name, cutoff, panel_kind, panel_margins, parallel, sel_ddi, overwrite):
+def _check_panel_parms(image_name, panel_name, cutoff, panel_kind, panel_margins, ant_name, ddi, parallel, overwrite):
     """
     Tests inputs to panel function
     Args:
         image_name: Input holography data, can be from astrohack.holog, but also preprocessed AIPS data
         panel_name: Name for the output directory structure containing the products
 
         cutoff: Cut off in amplitude for the physical deviation fitting, None means 20%
         panel_kind: Type of fitting function used to fit panel surfaces, defaults to corotated_paraboloid for ringed
                     telescopes
+        ant_name: Which Antennae are to be processed by panel, None means all of them
+        ddi: Which DDIs are to be processed by panel, None means all of them
         parallel: Run chunks of processing in parallel
         panel_margins: Margin to be ignored at edges of panels when fitting
-        sel_ddi: Which DDIs are to be processed by panel, None means all of them
+
         overwrite: Overwrite previous hack_file of same name?
     """
 
     panel_params = {'image_name': image_name,
                     'panel_name': panel_name,
                     'cutoff': cutoff,
                     'panel_kind': panel_kind,
                     'panel_margins': panel_margins,
                     'parallel': parallel,
-                    'sel_ddi': sel_ddi,
+                    'ddi': ddi,
+                    'ant_name': ant_name,
                     'overwrite': overwrite
                     }
                           
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
     parms_passed = parms_passed and _check_parms(panel_params, 'image_name', [str], default=None)
     base_name = _remove_suffix(panel_params['image_name'], '.image.zarr')
     base_name = _remove_suffix(base_name, '.combine.zarr')
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_name', [str], default=base_name+'.panel.zarr')
+    parms_passed = parms_passed and _check_parms(panel_params, 'ant_name', [list], list_acceptable_data_types=[str],
+                                                 default='all')
+    parms_passed = parms_passed and _check_parms(panel_params, 'ddi', [list], list_acceptable_data_types=[str],
+                                                 default='all')
     parms_passed = parms_passed and _check_parms(panel_params, 'cutoff', [float], acceptable_range=[0, 1], default=0.2)
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_kind', [str], acceptable_data=panel_models, default="rigid")
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_margins', [float], acceptable_range=[0, 0.5], default=0.2)
     parms_passed = parms_passed and _check_parms(panel_params, 'parallel', [bool], default=False)
-    parms_passed = parms_passed and _check_parms(panel_params, 'sel_ddi', [list, np.array], list_acceptable_data_types=[int, np.int64], default='all')
     parms_passed = parms_passed and _check_parms(panel_params, 'overwrite', [bool], default=False)
 
+
     if not parms_passed:
         logger.error("panel parameter checking failed.")
         raise Exception("panel parameter checking failed.")
     
-    return panel_params
+    return panel_params
```

### Comparing `astrohack-0.1.2/src/astrohack/profiling.py` & `astrohack-0.1.3/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack/visualization/viewer.py` & `astrohack-0.1.3/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.1.3/src/astrohack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.2
+Version: 0.1.3
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.2/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.1.3/src/astrohack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/astrohack/_classes/ring_panel.py
 src/astrohack/_classes/telescope.py
 src/astrohack/_utils/__init__.py
 src/astrohack/_utils/_algorithms.py
 src/astrohack/_utils/_combine.py
 src/astrohack/_utils/_constants.py
 src/astrohack/_utils/_conversion.py
+src/astrohack/_utils/_dask_graph_tools.py
 src/astrohack/_utils/_dio.py
 src/astrohack/_utils/_extract_holog.py
 src/astrohack/_utils/_extract_point.py
 src/astrohack/_utils/_gaussfitter.py
 src/astrohack/_utils/_holog.py
 src/astrohack/_utils/_imaging.py
 src/astrohack/_utils/_io.py
```

### Comparing `astrohack-0.1.2/src/astrohack.egg-info/requires.txt` & `astrohack-0.1.3/src/astrohack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/tests/test_class_antenna_surface.py` & `astrohack-0.1.3/tests/test_class_antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/tests/test_class_base_panel.py` & `astrohack-0.1.3/tests/test_class_base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/tests/test_class_ring_panel.py` & `astrohack-0.1.3/tests/test_class_ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/tests/test_class_telescope.py` & `astrohack-0.1.3/tests/test_class_telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.2/tests/test_stakeholder.py` & `astrohack-0.1.3/tests/test_stakeholder.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     }
 
 
     extract_holog(
       ms_name=before_ms, 
       holog_name=before_holog, 
       ddi_sel=[0],
-      data_col='CORRECTED_DATA',
+      data_column='CORRECTED_DATA',
       parallel=False,
       overwrite=True,
       reuse_point_zarr=False
     )
 
     assert verify_holog_obs_dictionary(holog_obs_dict)
 
@@ -168,15 +168,15 @@
         }
     }
 
 
     holog_mds_after, _ = extract_holog(
         ms_name=after_ms, 
         holog_name=after_holog,
-        data_col='CORRECTED_DATA',
+        data_column='CORRECTED_DATA',
         parallel=False,
         overwrite=True,
         reuse_point_zarr=False
     )
 
     assert verify_holog_obs_dictionary(holog_obs_dict)
```

