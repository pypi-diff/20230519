# Comparing `tmp/pdbufr-0.8.2.tar.gz` & `tmp/pdbufr-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdbufr-0.8.2.tar", last modified: Wed Dec  2 11:21:59 2020, max compression
+gzip compressed data, was "dist/pdbufr-0.9.0.tar", last modified: Tue Jun  8 09:46:53 2021, max compression
```

## Comparing `pdbufr-0.8.2.tar` & `pdbufr-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,64 @@
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2020-12-02 11:21:59.908775 pdbufr-0.8.2/
--rw-r--r--   0 amici      (501) staff       (20)    11357 2020-12-02 11:21:59.000000 pdbufr-0.8.2/LICENSE
--rw-r--r--   0 amici      (501) staff       (20)      152 2020-12-02 11:21:59.000000 pdbufr-0.8.2/MANIFEST.in
--rw-r--r--   0 amici      (501) staff       (20)     2642 2020-12-02 11:21:59.000000 pdbufr-0.8.2/Makefile
--rw-r--r--   0 amici      (501) staff       (20)     7315 2020-12-02 11:21:59.908920 pdbufr-0.8.2/PKG-INFO
--rw-r--r--   0 amici      (501) staff       (20)     5234 2020-12-02 11:21:59.000000 pdbufr-0.8.2/README.rst
--rw-r--r--   0 amici      (501) staff       (20)      113 2020-12-02 11:21:59.000000 pdbufr-0.8.2/environment.in.yml
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2020-12-02 11:21:59.893649 pdbufr-0.8.2/pdbufr/
--rw-r--r--   0 amici      (501) staff       (20)       81 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr/__init__.py
--rw-r--r--   0 amici      (501) staff       (20)     1243 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr/__main__.py
--rw-r--r--   0 amici      (501) staff       (20)     1822 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr/bufr_filters.py
--rw-r--r--   0 amici      (501) staff       (20)    11562 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr/bufr_read.py
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2020-12-02 11:21:59.895265 pdbufr-0.8.2/pdbufr.egg-info/
--rw-r--r--   0 amici      (501) staff       (20)     7315 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr.egg-info/PKG-INFO
--rw-r--r--   0 amici      (501) staff       (20)     1354 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr.egg-info/SOURCES.txt
--rw-r--r--   0 amici      (501) staff       (20)        1 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr.egg-info/dependency_links.txt
--rw-r--r--   0 amici      (501) staff       (20)       49 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr.egg-info/requires.txt
--rw-r--r--   0 amici      (501) staff       (20)        7 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr.egg-info/top_level.txt
--rw-r--r--   0 amici      (501) staff       (20)        1 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pdbufr.egg-info/zip-safe
--rw-r--r--   0 amici      (501) staff       (20)      170 2020-12-02 11:21:59.000000 pdbufr-0.8.2/pyproject.toml
--rw-r--r--   0 amici      (501) staff       (20)      101 2020-12-02 11:21:59.909342 pdbufr-0.8.2/setup.cfg
--rw-r--r--   0 amici      (501) staff       (20)     2511 2020-12-02 11:21:59.000000 pdbufr-0.8.2/setup.py
--rw-r--r--   0 amici      (501) staff       (20)   497568 2020-12-02 11:21:59.000000 pdbufr-0.8.2/temp.bufr
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2020-12-02 11:21:59.900681 pdbufr-0.8.2/tests/
--rw-r--r--   0 amici      (501) staff       (20)     1024 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/environment-macos-3.8.yml
--rw-r--r--   0 amici      (501) staff       (20)     1082 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/environment-ubuntu-3.6.yml
--rw-r--r--   0 amici      (501) staff       (20)     1081 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/environment-ubuntu-3.7.yml
--rw-r--r--   0 amici      (501) staff       (20)     1081 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/environment-ubuntu-3.8.yml
--rw-r--r--   0 amici      (501) staff       (20)      943 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/environment-windows-3.8.yml
--rw-r--r--   0 amici      (501) staff       (20)     1012 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/perf_aircraft.py
--rw-r--r--   0 amici      (501) staff       (20)      444 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/perf_mv_aircraft.py
--rw-r--r--   0 amici      (501) staff       (20)      568 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/perf_mv_sat_compressed.py
--rw-r--r--   0 amici      (501) staff       (20)      426 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/perf_mv_synop.py
--rw-r--r--   0 amici      (501) staff       (20)     1066 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/perf_sat_compressed.py
--rw-r--r--   0 amici      (501) staff       (20)     1001 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/perf_synop.py
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2020-12-02 11:21:59.908525 pdbufr-0.8.2/tests/sample-data/
--rwxr-xr-x   0 amici      (501) staff       (20)  2861237 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/M02-HIRS-HIRxxx1B-NA-1.0-20181122114854.000000000Z-20181122132602-1304602.bufr
--rw-r--r--   0 amici      (501) staff       (20)     2380 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/aircraft_small.bufr
--rw-r--r--   0 amici      (501) staff       (20)    56123 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/compress_3.bufr
--rw-r--r--   0 amici      (501) staff       (20)     4076 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/ens_multi_subset_compressed.bufr
--rw-r--r--   0 amici      (501) staff       (20)     9987 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/ens_multi_subset_uncompressed.bufr
--rw-r--r--   0 amici      (501) staff       (20)    11000 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/obs_3day.bufr
--rwxr-xr-x   0 amici      (501) staff       (20)  1083986 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/perf_aircraft.bufr
--rw-r--r--   0 amici      (501) staff       (20)      994 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/syn_new.bufr
--rw-r--r--   0 amici      (501) staff       (20)     1652 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/synop_multi_subset_uncompressed.bufr
--rw-r--r--   0 amici      (501) staff       (20)   497568 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/temp.bufr
--rw-r--r--   0 amici      (501) staff       (20)     7664 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/temp_small.bufr
--rw-r--r--   0 amici      (501) staff       (20)    41357 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/tropical_cyclone.bufr
--rwxr-xr-x   0 amici      (501) staff       (20)    27341 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/sample-data/wave_uncompressed.bufr
--rw-r--r--   0 amici      (501) staff       (20)      807 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/test_10_main.py
--rw-r--r--   0 amici      (501) staff       (20)     3317 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/test_20_bufr_filters.py
--rw-r--r--   0 amici      (501) staff       (20)     3138 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/test_30_bufr_read.py
--rw-r--r--   0 amici      (501) staff       (20)    30354 2020-12-02 11:21:59.000000 pdbufr-0.8.2/tests/test_40_sample_data.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-06-08 09:46:53.000000 pdbufr-0.9.0/
+-rw-r--r--   0 iain       (501) staff       (20)    11357 2021-06-08 09:46:52.000000 pdbufr-0.9.0/LICENSE
+-rw-r--r--   0 iain       (501) staff       (20)      169 2021-06-08 09:46:52.000000 pdbufr-0.9.0/MANIFEST.in
+-rw-r--r--   0 iain       (501) staff       (20)      846 2021-06-08 09:46:52.000000 pdbufr-0.9.0/Makefile
+-rw-r--r--   0 iain       (501) staff       (20)     7627 2021-06-08 09:46:53.000000 pdbufr-0.9.0/PKG-INFO
+-rw-r--r--   0 iain       (501) staff       (20)     5482 2021-06-08 09:46:52.000000 pdbufr-0.9.0/README.rst
+-rw-r--r--   0 iain       (501) staff       (20)      112 2021-06-08 09:46:52.000000 pdbufr-0.9.0/environment-minimal.in.yml
+-rw-r--r--   0 iain       (501) staff       (20)      123 2021-06-08 09:46:52.000000 pdbufr-0.9.0/environment.in.yml
+-rw-r--r--   0 iain       (501) staff       (20)       59 2021-06-08 09:46:52.000000 pdbufr-0.9.0/mypy.ini
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-06-08 09:46:53.000000 pdbufr-0.9.0/pdbufr/
+-rw-r--r--   0 iain       (501) staff       (20)      599 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pdbufr/__init__.py
+-rw-r--r--   0 iain       (501) staff       (20)      951 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pdbufr/__main__.py
+-rw-r--r--   0 iain       (501) staff       (20)     2384 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pdbufr/bufr_filters.py
+-rw-r--r--   0 iain       (501) staff       (20)     1453 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pdbufr/bufr_read.py
+-rw-r--r--   0 iain       (501) staff       (20)    10944 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pdbufr/bufr_structure.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-06-08 09:46:53.000000 pdbufr-0.9.0/pdbufr/high_level_bufr/
+-rw-r--r--   0 iain       (501) staff       (20)        0 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pdbufr/high_level_bufr/__init__.py
+-rw-r--r--   0 iain       (501) staff       (20)     3376 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pdbufr/high_level_bufr/bufr.py
+-rw-r--r--   0 iain       (501) staff       (20)     2527 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pdbufr/high_level_bufr/codesfile.py
+-rw-r--r--   0 iain       (501) staff       (20)     7155 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pdbufr/high_level_bufr/codesmessage.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-06-08 09:46:53.000000 pdbufr-0.9.0/pdbufr.egg-info/
+-rw-r--r--   0 iain       (501) staff       (20)     7627 2021-06-08 09:46:53.000000 pdbufr-0.9.0/pdbufr.egg-info/PKG-INFO
+-rw-r--r--   0 iain       (501) staff       (20)     1679 2021-06-08 09:46:53.000000 pdbufr-0.9.0/pdbufr.egg-info/SOURCES.txt
+-rw-r--r--   0 iain       (501) staff       (20)        1 2021-06-08 09:46:53.000000 pdbufr-0.9.0/pdbufr.egg-info/dependency_links.txt
+-rw-r--r--   0 iain       (501) staff       (20)       55 2021-06-08 09:46:53.000000 pdbufr-0.9.0/pdbufr.egg-info/requires.txt
+-rw-r--r--   0 iain       (501) staff       (20)        7 2021-06-08 09:46:53.000000 pdbufr-0.9.0/pdbufr.egg-info/top_level.txt
+-rw-r--r--   0 iain       (501) staff       (20)        1 2021-06-08 09:46:53.000000 pdbufr-0.9.0/pdbufr.egg-info/zip-safe
+-rw-r--r--   0 iain       (501) staff       (20)      170 2021-06-08 09:46:52.000000 pdbufr-0.9.0/pyproject.toml
+-rw-r--r--   0 iain       (501) staff       (20)      132 2021-06-08 09:46:53.000000 pdbufr-0.9.0/setup.cfg
+-rw-r--r--   0 iain       (501) staff       (20)     2213 2021-06-08 09:46:52.000000 pdbufr-0.9.0/setup.py
+-rw-r--r--   0 iain       (501) staff       (20)   497568 2021-06-08 09:46:53.000000 pdbufr-0.9.0/temp.bufr
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/
+-rw-r--r--   0 iain       (501) staff       (20)     1024 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/environment-macos-3.8.yml
+-rw-r--r--   0 iain       (501) staff       (20)     1082 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/environment-ubuntu-3.6.yml
+-rw-r--r--   0 iain       (501) staff       (20)     1081 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/environment-ubuntu-3.7.yml
+-rw-r--r--   0 iain       (501) staff       (20)     1037 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/environment-ubuntu-3.8-minimal.yml
+-rw-r--r--   0 iain       (501) staff       (20)     1081 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/environment-ubuntu-3.8.yml
+-rw-r--r--   0 iain       (501) staff       (20)      943 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/environment-windows-3.8.yml
+-rw-r--r--   0 iain       (501) staff       (20)      767 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/perf_aircraft.py
+-rw-r--r--   0 iain       (501) staff       (20)      839 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/perf_mv_aircraft.py
+-rw-r--r--   0 iain       (501) staff       (20)      963 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/perf_mv_sat_compressed.py
+-rw-r--r--   0 iain       (501) staff       (20)      821 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/perf_mv_synop.py
+-rw-r--r--   0 iain       (501) staff       (20)      821 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/perf_sat_compressed.py
+-rw-r--r--   0 iain       (501) staff       (20)      756 2021-06-08 09:46:52.000000 pdbufr-0.9.0/tests/perf_synop.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/
+-rwxr-xr-x   0 iain       (501) staff       (20)  2861237 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/M02-HIRS-HIRxxx1B-NA-1.0-20181122114854.000000000Z-20181122132602-1304602.bufr
+-rw-r--r--   0 iain       (501) staff       (20)     2380 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/aircraft_small.bufr
+-rw-r--r--   0 iain       (501) staff       (20)    56123 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/compress_3.bufr
+-rw-r--r--   0 iain       (501) staff       (20)     4076 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/ens_multi_subset_compressed.bufr
+-rw-r--r--   0 iain       (501) staff       (20)     9987 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/ens_multi_subset_uncompressed.bufr
+-rw-r--r--   0 iain       (501) staff       (20)    11000 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/obs_3day.bufr
+-rwxr-xr-x   0 iain       (501) staff       (20)  1083986 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/perf_aircraft.bufr
+-rw-r--r--   0 iain       (501) staff       (20)  5668423 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/perf_sat_compressed.bufr
+-rw-r--r--   0 iain       (501) staff       (20)  3464576 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/perf_synop.bufr
+-rw-r--r--   0 iain       (501) staff       (20)      994 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/syn_new.bufr
+-rw-r--r--   0 iain       (501) staff       (20)     1652 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/synop_multi_subset_uncompressed.bufr
+-rw-r--r--   0 iain       (501) staff       (20)   497568 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/temp.bufr
+-rw-r--r--   0 iain       (501) staff       (20)     7664 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/temp_small.bufr
+-rw-r--r--   0 iain       (501) staff       (20)    41357 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/tropical_cyclone.bufr
+-rwxr-xr-x   0 iain       (501) staff       (20)    27341 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/sample-data/wave_uncompressed.bufr
+-rw-r--r--   0 iain       (501) staff       (20)     3937 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/test_10_bufr_filters.py
+-rw-r--r--   0 iain       (501) staff       (20)      570 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/test_10_main.py
+-rw-r--r--   0 iain       (501) staff       (20)    10562 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/test_20_bufr_structure.py
+-rw-r--r--   0 iain       (501) staff       (20)    31182 2021-06-08 09:46:53.000000 pdbufr-0.9.0/tests/test_40_sample_data.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pdbufr-0.8.2/LICENSE` & `pdbufr-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/PKG-INFO` & `pdbufr-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: pdbufr
-Version: 0.8.2
+Version: 0.9.0
 Summary: Pandas reader for the BUFR format using ecCodes.
 Home-page: https://github.com/ecmwf/pdbufr
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
-Description: 
+Description: pdbufr
+        ======
+        
+        .. image:: https://img.shields.io/pypi/v/pdbufr.svg
+           :target: https://pypi.python.org/pypi/pdbufr/
+        
         Pandas reader for the BUFR format using ecCodes.
         
-        Features with development status **Alpha**:
+        Features with development status **Beta**:
         
         - extracts observations from a BUFR file as a Pandas DataFrame,
         - reads BUFR 3 and 4 files with uncompressed and compressed subsets,
         - supports all modern versions of Python 3.9, 3.8, 3.7, 3.6 and PyPy3,
-        - works on Linux, MacOS and Windows, the ecCodes C-library is the only binary dependency.
+        - works on Linux, MacOS and Windows, the ecCodes C-library is the only binary dependency,
+        - sports a rich filtering engine.
         
         Limitations:
         
-        - no special handling of nodata values (yet),
-        - no conda-forge package (yet),
-        - filters only match exact values.
+        - no conda-forge package (yet).
         
         Installation
         ============
         
         The easiest way to install *pdbufr* dependencies is via Conda::
         
             $ conda install -c conda-forge python-eccodes pandas
@@ -133,22 +137,26 @@
         Lead developer:
         
         - `Alessandro Amici <https://github.com/alexamici>`_ - `B-Open <https://bopen.eu>`_
         
         Main contributors:
         
         - `Sandor Kertesz <https://github.com/sandorkertesz>`_ - `ECMWF <https://ecmwf.int>`_
+        - `Iain Russell <https://github.com/iainrussell>`_ - ECMWF
+        
+        Also:
+        - Daniel Lee - DWD, who contributed the code in the high_level_bufr directory, originally part of eccodes-python
         
         See also the list of `contributors <https://github.com/ecmwf/pdbufr/contributors>`_ who participated in this project.
         
         
         License
         =======
         
-        Copyright 2019 European Centre for Medium-Range Weather Forecasts (ECMWF).
+        Copyright 2019- European Centre for Medium-Range Weather Forecasts (ECMWF).
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at: http://www.apache.org/licenses/LICENSE-2.0.
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `pdbufr-0.8.2/README.rst` & `pdbufr-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+pdbufr
+======
+
+.. image:: https://img.shields.io/pypi/v/pdbufr.svg
+   :target: https://pypi.python.org/pypi/pdbufr/
 
 Pandas reader for the BUFR format using ecCodes.
 
-Features with development status **Alpha**:
+Features with development status **Beta**:
 
 - extracts observations from a BUFR file as a Pandas DataFrame,
 - reads BUFR 3 and 4 files with uncompressed and compressed subsets,
 - supports all modern versions of Python 3.9, 3.8, 3.7, 3.6 and PyPy3,
-- works on Linux, MacOS and Windows, the ecCodes C-library is the only binary dependency.
+- works on Linux, MacOS and Windows, the ecCodes C-library is the only binary dependency,
+- sports a rich filtering engine.
 
 Limitations:
 
-- no special handling of nodata values (yet),
-- no conda-forge package (yet),
-- filters only match exact values.
+- no conda-forge package (yet).
 
 Installation
 ============
 
 The easiest way to install *pdbufr* dependencies is via Conda::
 
     $ conda install -c conda-forge python-eccodes pandas
@@ -125,22 +129,26 @@
 Lead developer:
 
 - `Alessandro Amici <https://github.com/alexamici>`_ - `B-Open <https://bopen.eu>`_
 
 Main contributors:
 
 - `Sandor Kertesz <https://github.com/sandorkertesz>`_ - `ECMWF <https://ecmwf.int>`_
+- `Iain Russell <https://github.com/iainrussell>`_ - ECMWF
+
+Also:
+- Daniel Lee - DWD, who contributed the code in the high_level_bufr directory, originally part of eccodes-python
 
 See also the list of `contributors <https://github.com/ecmwf/pdbufr/contributors>`_ who participated in this project.
 
 
 License
 =======
 
-Copyright 2019 European Centre for Medium-Range Weather Forecasts (ECMWF).
+Copyright 2019- European Centre for Medium-Range Weather Forecasts (ECMWF).
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at: http://www.apache.org/licenses/LICENSE-2.0.
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `pdbufr-0.8.2/pdbufr.egg-info/PKG-INFO` & `pdbufr-0.9.0/pdbufr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: pdbufr
-Version: 0.8.2
+Version: 0.9.0
 Summary: Pandas reader for the BUFR format using ecCodes.
 Home-page: https://github.com/ecmwf/pdbufr
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
-Description: 
+Description: pdbufr
+        ======
+        
+        .. image:: https://img.shields.io/pypi/v/pdbufr.svg
+           :target: https://pypi.python.org/pypi/pdbufr/
+        
         Pandas reader for the BUFR format using ecCodes.
         
-        Features with development status **Alpha**:
+        Features with development status **Beta**:
         
         - extracts observations from a BUFR file as a Pandas DataFrame,
         - reads BUFR 3 and 4 files with uncompressed and compressed subsets,
         - supports all modern versions of Python 3.9, 3.8, 3.7, 3.6 and PyPy3,
-        - works on Linux, MacOS and Windows, the ecCodes C-library is the only binary dependency.
+        - works on Linux, MacOS and Windows, the ecCodes C-library is the only binary dependency,
+        - sports a rich filtering engine.
         
         Limitations:
         
-        - no special handling of nodata values (yet),
-        - no conda-forge package (yet),
-        - filters only match exact values.
+        - no conda-forge package (yet).
         
         Installation
         ============
         
         The easiest way to install *pdbufr* dependencies is via Conda::
         
             $ conda install -c conda-forge python-eccodes pandas
@@ -133,22 +137,26 @@
         Lead developer:
         
         - `Alessandro Amici <https://github.com/alexamici>`_ - `B-Open <https://bopen.eu>`_
         
         Main contributors:
         
         - `Sandor Kertesz <https://github.com/sandorkertesz>`_ - `ECMWF <https://ecmwf.int>`_
+        - `Iain Russell <https://github.com/iainrussell>`_ - ECMWF
+        
+        Also:
+        - Daniel Lee - DWD, who contributed the code in the high_level_bufr directory, originally part of eccodes-python
         
         See also the list of `contributors <https://github.com/ecmwf/pdbufr/contributors>`_ who participated in this project.
         
         
         License
         =======
         
-        Copyright 2019 European Centre for Medium-Range Weather Forecasts (ECMWF).
+        Copyright 2019- European Centre for Medium-Range Weather Forecasts (ECMWF).
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at: http://www.apache.org/licenses/LICENSE-2.0.
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `pdbufr-0.8.2/pdbufr.egg-info/SOURCES.txt` & `pdbufr-0.9.0/pdbufr.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
+environment-minimal.in.yml
 environment.in.yml
+mypy.ini
 pyproject.toml
 setup.cfg
 setup.py
 temp.bufr
 pdbufr/__init__.py
 pdbufr/__main__.py
 pdbufr/bufr_filters.py
 pdbufr/bufr_read.py
+pdbufr/bufr_structure.py
 pdbufr.egg-info/PKG-INFO
 pdbufr.egg-info/SOURCES.txt
 pdbufr.egg-info/dependency_links.txt
 pdbufr.egg-info/requires.txt
 pdbufr.egg-info/top_level.txt
 pdbufr.egg-info/zip-safe
+pdbufr/high_level_bufr/__init__.py
+pdbufr/high_level_bufr/bufr.py
+pdbufr/high_level_bufr/codesfile.py
+pdbufr/high_level_bufr/codesmessage.py
 tests/environment-macos-3.8.yml
 tests/environment-ubuntu-3.6.yml
 tests/environment-ubuntu-3.7.yml
+tests/environment-ubuntu-3.8-minimal.yml
 tests/environment-ubuntu-3.8.yml
 tests/environment-windows-3.8.yml
 tests/perf_aircraft.py
 tests/perf_mv_aircraft.py
 tests/perf_mv_sat_compressed.py
 tests/perf_mv_synop.py
 tests/perf_sat_compressed.py
 tests/perf_synop.py
+tests/test_10_bufr_filters.py
 tests/test_10_main.py
-tests/test_20_bufr_filters.py
-tests/test_30_bufr_read.py
+tests/test_20_bufr_structure.py
 tests/test_40_sample_data.py
 tests/sample-data/M02-HIRS-HIRxxx1B-NA-1.0-20181122114854.000000000Z-20181122132602-1304602.bufr
 tests/sample-data/aircraft_small.bufr
 tests/sample-data/compress_3.bufr
 tests/sample-data/ens_multi_subset_compressed.bufr
 tests/sample-data/ens_multi_subset_uncompressed.bufr
 tests/sample-data/obs_3day.bufr
 tests/sample-data/perf_aircraft.bufr
+tests/sample-data/perf_sat_compressed.bufr
+tests/sample-data/perf_synop.bufr
 tests/sample-data/syn_new.bufr
 tests/sample-data/synop_multi_subset_uncompressed.bufr
 tests/sample-data/temp.bufr
 tests/sample-data/temp_small.bufr
 tests/sample-data/tropical_cyclone.bufr
 tests/sample-data/wave_uncompressed.bufr
```

### Comparing `pdbufr-0.8.2/setup.py` & `pdbufr-0.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 #!/usr/bin/env python
 #
-# Copyright 2019 European Centre for Medium-Range Weather Forecasts (ECMWF).
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Authors:
-#   Alessandro Amici - B-Open - https://bopen.eu
+# (C) Copyright 2019- ECMWF.
 #
+# This software is licensed under the terms of the Apache Licence Version 2.0
+# which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
+# In applying this licence, ECMWF does not waive the privileges and immunities
+# granted to it by virtue of its status as an intergovernmental organisation
+# nor does it submit to any jurisdiction.
 
 import os
 import re
 
 import setuptools  # type: ignore
 
 
@@ -46,15 +36,15 @@
     long_description=read("README.rst"),
     author="European Centre for Medium-Range Weather Forecasts (ECMWF)",
     author_email="software.support@ecmwf.int",
     license="Apache License Version 2.0",
     url="https://github.com/ecmwf/pdbufr",
     packages=setuptools.find_packages(),
     include_package_data=True,
-    install_requires=["eccodes", "pandas"],
+    install_requires=["attrs", "eccodes", "pandas"],
     extras_require={"tests": ["flake8", "pytest", "pytest-cov"]},
     zip_safe=True,
     keywords="eccodes bufr pandas",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `pdbufr-0.8.2/temp.bufr` & `pdbufr-0.9.0/temp.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/environment-macos-3.8.yml` & `pdbufr-0.9.0/tests/environment-macos-3.8.yml`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/environment-ubuntu-3.6.yml` & `pdbufr-0.9.0/tests/environment-ubuntu-3.6.yml`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/environment-ubuntu-3.7.yml` & `pdbufr-0.9.0/tests/environment-ubuntu-3.7.yml`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/environment-ubuntu-3.8.yml` & `pdbufr-0.9.0/tests/environment-ubuntu-3.8.yml`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/environment-windows-3.8.yml` & `pdbufr-0.9.0/tests/environment-windows-3.8.yml`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/perf_synop.py` & `pdbufr-0.9.0/tests/perf_synop.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,14 @@
+# (C) Copyright 2019- ECMWF.
 #
-# Copyright 2019 European Centre for Medium-Range Weather Forecasts (ECMWF).
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This software is licensed under the terms of the Apache Licence Version 2.0
+# which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
+# In applying this licence, ECMWF does not waive the privileges and immunities
+# granted to it by virtue of its status as an intergovernmental organisation
+# nor does it submit to any jurisdiction.
 
 import os
 
 import pdbufr
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA = os.path.join(SAMPLE_DATA_FOLDER, "perf_synop.bufr")
```

### Comparing `pdbufr-0.8.2/tests/sample-data/M02-HIRS-HIRxxx1B-NA-1.0-20181122114854.000000000Z-20181122132602-1304602.bufr` & `pdbufr-0.9.0/tests/sample-data/M02-HIRS-HIRxxx1B-NA-1.0-20181122114854.000000000Z-20181122132602-1304602.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/aircraft_small.bufr` & `pdbufr-0.9.0/tests/sample-data/aircraft_small.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/compress_3.bufr` & `pdbufr-0.9.0/tests/sample-data/compress_3.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/ens_multi_subset_compressed.bufr` & `pdbufr-0.9.0/tests/sample-data/ens_multi_subset_compressed.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/ens_multi_subset_uncompressed.bufr` & `pdbufr-0.9.0/tests/sample-data/ens_multi_subset_uncompressed.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/obs_3day.bufr` & `pdbufr-0.9.0/tests/sample-data/obs_3day.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/perf_aircraft.bufr` & `pdbufr-0.9.0/tests/sample-data/perf_aircraft.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/syn_new.bufr` & `pdbufr-0.9.0/tests/sample-data/syn_new.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/synop_multi_subset_uncompressed.bufr` & `pdbufr-0.9.0/tests/sample-data/synop_multi_subset_uncompressed.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/temp.bufr` & `pdbufr-0.9.0/tests/sample-data/temp.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/temp_small.bufr` & `pdbufr-0.9.0/tests/sample-data/temp_small.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/tropical_cyclone.bufr` & `pdbufr-0.9.0/tests/sample-data/tropical_cyclone.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/sample-data/wave_uncompressed.bufr` & `pdbufr-0.9.0/tests/sample-data/wave_uncompressed.bufr`

 * *Files identical despite different names*

### Comparing `pdbufr-0.8.2/tests/test_20_bufr_filters.py` & `pdbufr-0.9.0/tests/test_10_bufr_filters.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,91 @@
+# (C) Copyright 2019- ECMWF.
+#
+# This software is licensed under the terms of the Apache Licence Version 2.0
+# which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
+# In applying this licence, ECMWF does not waive the privileges and immunities
+# granted to it by virtue of its status as an intergovernmental organisation
+# nor does it submit to any jurisdiction.
+
 import typing as T
 
 import numpy as np  # type: ignore
 
 from pdbufr import bufr_filters
 
 
-def test_BufrFilter_value():
-    assert bufr_filters.BufrFilter(1).match(1) is True
-    assert bufr_filters.BufrFilter(1).match(True) is True
-    assert bufr_filters.BufrFilter(1).match(1.0) is True
+def test_BufrFilter_value() -> None:
+    assert bufr_filters.BufrFilter.from_user(1).match(1) is True
+    assert bufr_filters.BufrFilter.from_user(1).match(True) is True
+    assert bufr_filters.BufrFilter.from_user(1).match(1.0) is True
 
-    assert bufr_filters.BufrFilter(1).match(False) is False
-    assert bufr_filters.BufrFilter(1).match(float("inf")) is False
+    assert bufr_filters.BufrFilter.from_user(1).match(False) is False
+    assert bufr_filters.BufrFilter.from_user(1).match(float("inf")) is False
+    assert bufr_filters.BufrFilter.from_user(1).match(None) is False
 
+    assert bufr_filters.BufrFilter.from_user(1).max() == 1
 
-def test_BufrFilter_iterator():
-    assert bufr_filters.BufrFilter([1, 2]).match(1) is True
-    assert bufr_filters.BufrFilter((1, 2)).match(True) is True
-    assert bufr_filters.BufrFilter({1, 2}).match(1.0) is True
 
-    assert bufr_filters.BufrFilter([1, 2]).match(False) is False
-    assert bufr_filters.BufrFilter({1, 2}).match(float("inf")) is False
+def test_BufrFilter_iterator() -> None:
+    assert bufr_filters.BufrFilter.from_user([1, 2]).match(1) is True
+    assert bufr_filters.BufrFilter.from_user((1, 2)).match(True) is True
+    assert bufr_filters.BufrFilter.from_user({1, 2}).match(1.0) is True
 
+    assert bufr_filters.BufrFilter.from_user([1, 2]).match(False) is False
+    assert bufr_filters.BufrFilter.from_user({1, 2}).match(float("inf")) is False
 
-def test_BufrFilter_slice():
-    assert bufr_filters.BufrFilter(slice(1, None)).match(float("inf")) is True
-    assert bufr_filters.BufrFilter(slice(None, 1)).match(True) is True
-    assert bufr_filters.BufrFilter(slice(1.0, 2.1)).match(1.0) is True
+    assert bufr_filters.BufrFilter.from_user({1, 2}).max() == 2
 
-    assert bufr_filters.BufrFilter(slice(0.1, 1.1, 0.1)).match(1.0) is True
 
-    assert bufr_filters.BufrFilter(slice(1, None)).match(False) is False
-    assert bufr_filters.BufrFilter(slice(1000.0)).match(float("inf")) is False
+def test_BufrFilter_slice() -> None:
+    assert bufr_filters.BufrFilter.from_user(slice(1, None)).match(float("inf")) is True
+    assert bufr_filters.BufrFilter.from_user(slice(None, 1)).match(True) is True
+    assert bufr_filters.BufrFilter.from_user(slice(1.0, 2.1)).match(1.0) is True
 
+    assert bufr_filters.BufrFilter.from_user(slice(0.1, 1.1, 0.1)).match(1.0) is True
 
-def test_BufrFilter_range():
-    assert bufr_filters.BufrFilter(range(1, 3)).match(1) is True
-    assert bufr_filters.BufrFilter(range(1, 3)).match(True) is True
-    assert bufr_filters.BufrFilter(range(1, 3)).match(1.0) is True
-    assert bufr_filters.BufrFilter(range(1, 3)).match(2) is True
+    assert bufr_filters.BufrFilter.from_user(slice(1, None)).match(False) is False
+    assert bufr_filters.BufrFilter.from_user(slice(1000.0)).match(float("inf")) is False
 
-    assert bufr_filters.BufrFilter(range(1, 3)).match(0) is False
-    assert bufr_filters.BufrFilter(range(1, 3)).match(1.5) is False
-    assert bufr_filters.BufrFilter(range(1, 3)).match(3) is False
+    assert bufr_filters.BufrFilter.from_user(slice(1, None)).max() is None
+    assert bufr_filters.BufrFilter.from_user(slice(None, 1)).max() == 1
 
-    assert bufr_filters.BufrFilter(np.arange(1, 3, 0.5)).match(1.5) is True
 
+def test_BufrFilter_range() -> None:
+    assert bufr_filters.BufrFilter.from_user(range(1, 3)).match(1) is True
+    assert bufr_filters.BufrFilter.from_user(range(1, 3)).match(True) is True
+    assert bufr_filters.BufrFilter.from_user(range(1, 3)).match(1.0) is True
+    assert bufr_filters.BufrFilter.from_user(range(1, 3)).match(2) is True
 
-def test_BufrFilter_callable():
-    assert bufr_filters.BufrFilter(lambda x: x > 0).match(1) is True
-    assert bufr_filters.BufrFilter(lambda x: x > 0).match(True) is True
-    assert bufr_filters.BufrFilter(lambda x: x > 0).match(1.0) is True
+    assert bufr_filters.BufrFilter.from_user(range(1, 3)).match(0) is False
+    assert bufr_filters.BufrFilter.from_user(range(1, 3)).match(1.5) is False
+    assert bufr_filters.BufrFilter.from_user(range(1, 3)).match(3) is False
 
-    assert bufr_filters.BufrFilter(lambda x: x > 0).match(0) is False
-    assert bufr_filters.BufrFilter(lambda x: x > 0).match(-1) is False
+    assert bufr_filters.BufrFilter.from_user(np.arange(1, 3, 0.5)).match(1.5) is True
 
 
-def test_compile_filters():
-    user_filters = {
-        "station": 234,
-        "level": range(1, 12),
-        "height": slice(1.5, 2.1),
-    }
+def test_BufrFilter_callable() -> None:
+    assert bufr_filters.BufrFilter.from_user(lambda x: x > 0).match(1) is True
+    assert bufr_filters.BufrFilter.from_user(lambda x: x > 0).match(True) is True
+    assert bufr_filters.BufrFilter.from_user(lambda x: x > 0).match(1.0) is True
 
-    res = bufr_filters.compile_filters(user_filters)
+    assert bufr_filters.BufrFilter.from_user(lambda x: x > 0).match(0) is False
+    assert bufr_filters.BufrFilter.from_user(lambda x: x > 0).match(-1) is False
 
-    assert isinstance(res, dict)
-    assert set(res) == set(user_filters)
-    assert all(isinstance(r, bufr_filters.BufrFilter) for r in res.values())
+    assert bufr_filters.BufrFilter.from_user(lambda x: x > 0).max() is None
 
 
-def test_match_compiled_filters():
+def test_is_match() -> None:
     compile_filters = {
-        "station": bufr_filters.BufrFilter(234),
-        "level": bufr_filters.BufrFilter(range(1, 12)),
+        "station": bufr_filters.BufrFilter({234}),
+        "level": bufr_filters.BufrFilter(set(range(1, 12))),
         "height": bufr_filters.BufrFilter(slice(1.5, 2.1)),
     }
 
-    message_items: T.List[T.Tuple[str, str, T.Any]] = [("station", "station", 233)]
-    assert bufr_filters.match_compiled_filters(message_items, compile_filters) is False
+    message: T.Dict[str, T.Any] = {"station": 233}
+    assert bufr_filters.is_match(message, compile_filters) is False
 
-    message_items = [("station", "station", 234), ("temperature", "temperature", 300.0)]
-    assert bufr_filters.match_compiled_filters(message_items, compile_filters) is False
+    message = {"station": 234, "temperature": 300.0}
+    assert bufr_filters.is_match(message, compile_filters) is False
 
-    message_items += [("#1#level", "level", 1), ("height", "height", 1.5)]
-    assert bufr_filters.match_compiled_filters(message_items, compile_filters) is True
+    message.update({"level": 1, "height": 1.5})
+    assert bufr_filters.is_match(message, compile_filters) is True
```

### Comparing `pdbufr-0.8.2/tests/test_40_sample_data.py` & `pdbufr-0.9.0/tests/test_40_sample_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,24 @@
+# (C) Copyright 2019- ECMWF.
 #
-# Copyright 2019 European Centre for Medium-Range Weather Forecasts (ECMWF).
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# This software is licensed under the terms of the Apache Licence Version 2.0
+# which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
+# In applying this licence, ECMWF does not waive the privileges and immunities
+# granted to it by virtue of its status as an intergovernmental organisation
+# nor does it submit to any jurisdiction.
 
-import math
 import os
 import typing as T
 
 import numpy as np  # type: ignore
-import pandas as pd  # type: ignore
 import pytest
 
+pd = pytest.importorskip("pandas")
+assert_frame_equal = pd.testing.assert_frame_equal
+
 import pdbufr
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA_1 = os.path.join(SAMPLE_DATA_FOLDER, "obs_3day.bufr")
 TEST_DATA_2 = os.path.join(SAMPLE_DATA_FOLDER, "synop_multi_subset_uncompressed.bufr")
 TEST_DATA_3 = os.path.join(SAMPLE_DATA_FOLDER, "temp.bufr")
 TEST_DATA_4 = os.path.join(
@@ -52,27 +46,33 @@
 # contains aircraft messages
 TEST_DATA_11 = os.path.join(SAMPLE_DATA_FOLDER, "aircraft_small.bufr")
 
 # contains new types of synop messages
 TEST_DATA_12 = os.path.join(SAMPLE_DATA_FOLDER, "syn_new.bufr")
 
 
-def test_read_bufr_one_subset_one_filters():
+def test_read_bufr_one_subset_one_filters() -> None:
     res = pdbufr.read_bufr(TEST_DATA_1, columns=("latitude",))
 
     assert isinstance(res, pd.DataFrame)
     assert "latitude" in res
     assert len(res) == 50
 
     res = pdbufr.read_bufr(
         TEST_DATA_1, columns=("latitude",), filters={"rdbtimeTime": "115557"}
     )
 
     assert len(res) == 6
 
+    res = pdbufr.read_bufr(
+        TEST_DATA_1, columns=("latitude"), filters={"rdbtimeTime": "115557"}
+    )
+
+    assert len(res) == 6
+
     res = pdbufr.read_bufr(TEST_DATA_1, columns=("latitude",), filters={"count": 1})
 
     assert len(res) == 1
 
     res = pdbufr.read_bufr(
         TEST_DATA_1, columns=("latitude",), filters={"stationNumber": 894}
     )
@@ -82,29 +82,29 @@
     res = pdbufr.read_bufr(
         TEST_DATA_1, columns=("latitude",), filters={"stationNumber": [894, 103]}
     )
 
     assert len(res) == 2
 
 
-def test_read_bufr_one_subset_one_observation_data():
+def test_read_bufr_one_subset_one_observation_data() -> None:
     columns = (
         "count",
         "stationNumber",
         "data_datetime",
         "latitude",
         "longitude",
         "heightOfStation",
         "airTemperatureAt2M",
         "dewpointTemperatureAt2M",
         "horizontalVisibility",
     )
     expected_first_row = {
         "count": 1,
-        "stationNumber": 894.0,
+        "stationNumber": 894,
         "data_datetime": pd.Timestamp("2017-04-25 12:00:00"),
         "latitude": 49.43000000000001,
         "longitude": -2.6,
         "heightOfStation": 101.0,
         "airTemperatureAt2M": 282.40000000000003,
         "dewpointTemperatureAt2M": 274.0,
         "horizontalVisibility": 55000.0,
@@ -112,15 +112,15 @@
 
     res = pdbufr.read_bufr(TEST_DATA_1, columns=columns)
 
     assert len(res) == 50
     assert res.iloc[0].to_dict() == expected_first_row
 
 
-def test_read_bufr_multiple_uncompressed_subsets_one_observation():
+def test_read_bufr_multiple_uncompressed_subsets_one_observation() -> None:
     res = pdbufr.read_bufr(TEST_DATA_2, columns=("latitude",))
 
     assert isinstance(res, pd.DataFrame)
     assert "latitude" in dict(res)
     assert len(res) == 12
 
     res = pdbufr.read_bufr(
@@ -156,29 +156,29 @@
 
     res = pdbufr.read_bufr(TEST_DATA_2, columns=columns, filters={"stationNumber": 27})
 
     assert len(res) == 1
     assert res.iloc[0].to_dict() == expected_first_row
 
 
-def test_read_bufr_one_subsets_multiple_observations_filters():
+def test_read_bufr_one_subsets_multiple_observations_filters() -> None:
     res = pdbufr.read_bufr(
         TEST_DATA_3, columns=("latitude",), filters={"stationNumber": 907}
     )
 
     assert len(res) == 1
 
     res = pdbufr.read_bufr(
         TEST_DATA_3, columns=("latitude",), filters={"pressure": [100000, 26300]}
     )
 
     assert len(res) == 425
 
 
-def test_read_bufr_one_subsets_multiple_observations_data():
+def test_read_bufr_one_subsets_multiple_observations_data() -> None:
     columns = [
         "stationNumber",
         "data_datetime",
         "longitude",
         "latitude",
         "heightOfStation",
         "pressure",
@@ -187,61 +187,61 @@
     expected_first_rows = pd.DataFrame.from_records(
         [
             {
                 "stationNumber": 907,
                 "data_datetime": pd.Timestamp("2008-12-08 12:00:00"),
                 "longitude": -78.08000000000001,
                 "latitude": 58.470000000000006,
-                "heightOfStation": 26,
+                "heightOfStation": 26.0,
                 "pressure": 100000.0,
                 "airTemperature": 259.7,
             },
             {
                 "stationNumber": 823,
                 "data_datetime": pd.Timestamp("2008-12-08 12:00:00"),
                 "longitude": -73.67,
                 "latitude": 53.75000000000001,
-                "heightOfStation": 302,
+                "heightOfStation": 302.0,
                 "pressure": 100000.0,
-                "airTemperature": math.nan,
+                "airTemperature": None,
             },
         ]
     )
 
     res = pdbufr.read_bufr(TEST_DATA_3, columns=columns, filters={"pressure": 100000})
 
     assert len(res) == 408
     assert res.iloc[:2].equals(expected_first_rows[res.columns])
 
 
-def test_read_bufr_multiple_compressed_subsets_multiple_observations_filters():
+def test_read_bufr_multiple_compressed_subsets_multiple_observations_filters() -> None:
     res = pdbufr.read_bufr(
         TEST_DATA_4, columns=("latitude",), filters={"hour": 11, "minute": 48}
     )
 
     assert len(res) == 56
 
     res = pdbufr.read_bufr(
         TEST_DATA_4, columns=("latitude",), filters={"hour": 11, "minute": [48, 49]}
     )
 
     assert len(res) == 616
 
 
-def test_read_bufr_multiple_compressed_subsets_multiple_observations_data():
+def test_read_bufr_multiple_compressed_subsets_multiple_observations_data() -> None:
     columns = [
         "data_datetime",
         "longitude",
         "latitude",
         "heightOfStation",
         "tovsOrAtovsOrAvhrrInstrumentationChannelNumber",
         "brightnessTemperature",
     ]
     expected_first_row = {
-        "data_datetime": pd.Timestamp("2018-11-22 11:48:54"),
+        "data_datetime": pd.Timestamp("2018-11-22 11:48:54.396"),
         "longitude": -9.201400000000001,
         "latitude": 53.354200000000006,
         "heightOfStation": 828400.0,
         "tovsOrAtovsOrAvhrrInstrumentationChannelNumber": 2.0,
         "brightnessTemperature": 218.76,
     }
 
@@ -255,15 +255,15 @@
         },
     )
 
     assert len(res) == 56
     assert res.iloc[0].to_dict() == expected_first_row
 
 
-def test_temp_single_station_1():
+def test_temp_single_station_1() -> None:
     columns = [
         "WMO_station_id",
         "stationNumber",
         "longitude",
         "latitude",
         "pressure",
         "verticalSoundingSignificance",
@@ -329,15 +329,15 @@
                 32,
                 4,
                 32,
                 4,
                 4,
             ],
             "airTemperature": [
-                math.nan,
+                None,
                 256.7,
                 255.10000000000002,
                 255.3,
                 256.7,
                 253.3,
                 253.10000000000002,
                 248.9,
@@ -360,18 +360,18 @@
                 221.5,
             ],
         }
     )
 
     res = pdbufr.read_bufr(TEST_DATA_3, columns=columns, filters={"stationNumber": 823})
 
-    assert res.equals(expected[res.columns])
+    assert_frame_equal(res, expected[res.columns])
 
 
-def test_temp_single_station_2():
+def test_temp_single_station_2() -> None:
     columns = [
         "stationNumber",
         "longitude",
         "latitude",
         "pressure",
         "airTemperature",
     ]
@@ -390,15 +390,15 @@
                 70000.0,
                 50000.0,
                 40000.0,
                 30000.0,
                 25000.0,
             ],
             "airTemperature": [
-                math.nan,
+                None,
                 255.3,
                 253.3,
                 241.9,
                 229.3,
                 222.9,
                 218.9,
                 221.10000000000002,
@@ -408,18 +408,18 @@
 
     res = pdbufr.read_bufr(
         TEST_DATA_3,
         columns=columns,
         filters={"stationNumber": 823, "verticalSoundingSignificance": 32},
     )
 
-    assert res.equals(expected[res.columns])
+    assert_frame_equal(res, expected[res.columns])
 
 
-def test_temp_single_station_3():
+def test_temp_single_station_3() -> None:
     columns = [
         "stationNumber",
         "data_datetime",
         "longitude",
         "latitude",
         "airTemperature",
         "pressure",
@@ -429,133 +429,152 @@
 
     ref = {
         "stationNumber": np.full(ref_num, 823),
         "latitude": np.full(ref_num, 53.75),
         "longitude": np.full(ref_num, -73.67),
         "pressure": [92500.0, 40000.0],
         "airTemperature": [255.3, 222.9],
+        "data_datetime": [
+            pd.Timestamp("2008-12-08 12:00:00"),
+            pd.Timestamp("2008-12-08 12:00:00"),
+        ],
     }
+    ref = pd.DataFrame.from_dict(ref)
 
     res = pdbufr.read_bufr(
         TEST_DATA_3,
         columns=columns,
         filters={
             "stationNumber": 823,
             "verticalSoundingSignificance": 32,
             "pressure": [40000.0, 92500.0],
         },
     )
 
-    for k in ref.keys():
-        assert np.allclose(res[k].values, ref[k])
+    assert_frame_equal(res, ref)
 
 
-def test_tropicalcyclone_1():
+def test_tropicalcyclone_1() -> None:
     columns = ["data_datetime", "longitude", "latitude", "windSpeedAt10M"]
 
+    expected = pd.DataFrame.from_dict(
+        {
+            "latitude": [None, 11.3, 12.7, 10.2],
+            "longitude": [None, -126.0, -124.9, -126],
+            "data_datetime": [
+                pd.Timestamp("2015-11-18 00:00:00"),
+                pd.Timestamp("2015-11-18 00:00:00"),
+                pd.Timestamp("2015-11-18 00:00:00"),
+                pd.Timestamp("2015-11-18 00:00:00"),
+            ],
+            "windSpeedAt10M": [None, None, 30.4, None],
+        }
+    )
+
     res = pdbufr.read_bufr(
         TEST_DATA_5,
         columns=columns,
         filters={"stormIdentifier": "70E", "ensembleMemberNumber": 4},
     )
 
-    assert len(res) == 67
+    assert len(res) == 34
 
     res = pdbufr.read_bufr(
         TEST_DATA_5,
         columns=columns,
         filters={"stormIdentifier": "70E", "ensembleMemberNumber": 4},
         required_columns=False,
     )
 
     assert len(res) == 69
+    assert_frame_equal(res[0:4], expected[0:4])
 
 
-def test_tropicalcyclone_2():
+def test_tropicalcyclone_2() -> None:
     columns = ["longitude", "latitude", "windSpeedAt10M"]
 
     expected = pd.DataFrame.from_dict(
         {
             "latitude": [
-                12.700000000000001,
+                12.7,
                 13.0,
-                12.700000000000001,
-                math.nan,
+                12.7,
+                None,
                 12.5,
-                12.200000000000001,
+                12.2,
                 12.5,
-                12.700000000000001,
-                12.700000000000001,
+                12.7,
+                12.7,
                 14.1,
                 13.6,
                 14.1,
                 14.1,
                 13.9,
                 15.3,
                 15.0,
-                14.700000000000001,
+                14.7,
                 15.0,
                 14.4,
                 14.4,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
             ],
             "longitude": [
                 -124.9,
                 -125.5,
                 -125.2,
-                math.nan,
+                None,
                 -127.5,
                 -128.0,
                 -128.0,
-                -126.60000000000001,
+                -126.6,
                 -128.3,
                 -126.0,
                 -128.9,
                 -129.4,
                 -130.5,
                 -131.4,
                 -128.9,
                 -128.9,
                 -130.3,
                 -128.9,
                 -129.4,
                 -127.5,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
             ],
             "windSpeedAt10M": [
-                30.400000000000002,
+                30.4,
                 17.0,
                 16.5,
-                math.nan,
+                None,
                 16.5,
                 15.4,
                 14.9,
                 12.4,
                 10.8,
                 11.8,
                 11.8,
@@ -564,207 +583,205 @@
                 11.3,
                 10.3,
                 11.8,
                 11.8,
                 11.8,
                 11.3,
                 11.3,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
-                math.nan,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
+                None,
             ],
         }
     )
 
     res = pdbufr.read_bufr(
         TEST_DATA_5,
         columns=columns,
         filters={
             "stormIdentifier": "70E",
             "ensembleMemberNumber": 4,
             "meteorologicalAttributeSignificance": 3,
         },
     )
 
-    assert res.equals(expected[res.columns])
+    assert_frame_equal(res, expected)
 
 
-def test_wave_1():
+def test_wave_1() -> None:
     columns = ["data_datetime", "longitude", "latitude", "significantWaveHeight"]
     expected_0 = pd.DataFrame.from_records(
         [
             {
-                "latitude": -28.866670000000003,
-                "longitude": 153.38333,
+                "latitude": -28.86667,
+                "longitude": 153.3833,
                 "significantWaveHeight": 2.34,
                 "data_datetime": pd.Timestamp("2017-11-02 10:00:00"),
             },
             {
-                "latitude": -28.866670000000003,
-                "longitude": 153.38333,
-                "significantWaveHeight": math.nan,
+                "latitude": -28.86667,
+                "longitude": 153.3833,
+                "significantWaveHeight": None,
                 "data_datetime": pd.Timestamp("2017-11-02 10:00:00"),
             },
             {
-                "latitude": -30.366670000000003,
+                "latitude": -30.36667,
                 "longitude": 153.36667,
                 "significantWaveHeight": 1.72,
                 "data_datetime": pd.Timestamp("2017-11-02 10:00:00"),
             },
         ]
     )
     expected_1 = pd.DataFrame.from_records(
         [
             {
                 "latitude": -35.7,
-                "longitude": 150.33333000000002,
+                "longitude": 150.33333,
                 "significantWaveHeight": 1.7,
                 "data_datetime": pd.Timestamp("2017-11-02 10:00:00"),
             },
             {
                 "latitude": -35.7,
-                "longitude": 150.33333000000002,
-                "significantWaveHeight": math.nan,
+                "longitude": 150.3333,
+                "significantWaveHeight": None,
                 "data_datetime": pd.Timestamp("2017-11-02 10:00:00"),
             },
         ]
     )
 
     res = pdbufr.read_bufr(TEST_DATA_6, columns=columns)
-    assert len(res) == 72
+    res_end = res[70:].reset_index(drop=True)
 
-    assert res.iloc[:3].equals(expected_0[res.columns])
-    assert res.iloc[70:].reset_index(drop=True).equals(expected_1[res.columns])
+    assert len(res) == 72
+    assert_frame_equal(res[:3], expected_0)
+    assert_frame_equal(res_end, expected_1)
 
 
-def test_ens_uncompressed():
+def test_ens_uncompressed() -> None:
     columns = [
         "longitude",
         "latitude",
         "ensembleMemberNumber",
         "timePeriod",
         "airTemperatureAt2M",
     ]
 
     res = pdbufr.read_bufr(TEST_DATA_7, columns=columns)
 
     ref = {
         "latitude": [51.52, 51.52],
-        "longitude": [0.9700000000000001, 0.9700000000000001],
+        "longitude": [0.97, 0.97],
         "ensembleMemberNumber": [0, 0],
         "timePeriod": [0, 6],
         "airTemperatureAt2M": [292.7, 291.6],
     }
+    ref = pd.DataFrame.from_dict(ref)
 
     assert len(res) == 3111
+    assert_frame_equal(res[:2], ref[res.columns])
 
-    for k in ref.keys():
-        assert np.allclose(res[k].values[0:2], ref[k])
 
-
-def test_ens_compressed():
+def test_ens_compressed() -> None:
     columns = ["longitude", "latitude", "ensembleMemberNumber", "timePeriod", "cape"]
 
     res = pdbufr.read_bufr(
         TEST_DATA_9,
         columns=columns,
         filters={"timePeriod": [0, 24], "ensembleMemberNumber": [2, 5]},
     )
 
     ref = {
         "latitude": [51.52, 51.52, 51.52, 51.52],
-        "longitude": [
-            0.9700000000000001,
-            0.9700000000000001,
-            0.9700000000000001,
-            0.9700000000000001,
-        ],
+        "longitude": [0.97, 0.97, 0.97, 0.97],
         "ensembleMemberNumber": [2, 2, 5, 5],
         "timePeriod": [0, 24, 0, 24],
         "cape": [41.9, 0, 14.4, 0],
     }
+    ref = pd.DataFrame.from_dict(ref)
 
     assert len(res) == 4
+    assert_frame_equal(res, ref[res.columns])
 
-    for k in ref.keys():
-        assert np.allclose(res[k].values[0:4], ref[k])
 
-
-def test_sat_compressed_1():
+def test_sat_compressed_1() -> None:
     columns = [
         "data_datetime",
         "latitude",
         "longitude",
         "nonCoordinateLatitude",
         "nonCoordinateLongitude",
         "significandOfVolumetricMixingRatio",
         "nonCoordinatePressure",
     ]
 
     expected_first_row = {
         "data_datetime": pd.Timestamp("2015-08-21 01:59:05"),
-        "latitude": -44.833890000000004,
-        "longitude": 171.16350000000003,
+        "latitude": -44.83389,
+        "longitude": 171.1635,
         "nonCoordinateLatitude": -44.82399,
-        "nonCoordinateLongitude": 171.05569000000003,
+        "nonCoordinateLongitude": 171.05569,
         "nonCoordinatePressure": 8555.0,
         "significandOfVolumetricMixingRatio": 8531573,
     }
 
     expected_second_row = {
         "data_datetime": pd.Timestamp("2015-08-21 01:59:05"),
-        "latitude": -44.833890000000004,
-        "longitude": 171.16350000000003,
+        "latitude": -44.83389,
+        "longitude": 171.1635,
         "nonCoordinateLatitude": -44.82399,
-        "nonCoordinateLongitude": 171.05569000000003,
-        "nonCoordinatePressure": 17100.100000000002,
+        "nonCoordinateLongitude": 171.05569,
+        "nonCoordinatePressure": 17100.1,
         "significandOfVolumetricMixingRatio": 8486850,
     }
 
     expected_12_row = {
         "data_datetime": pd.Timestamp("2015-08-21 01:59:05"),
-        "latitude": -44.833890000000004,
-        "longitude": 171.16350000000003,
+        "latitude": -44.83389,
+        "longitude": 171.1635,
         "nonCoordinateLatitude": -44.82399,
-        "nonCoordinateLongitude": 171.05569000000003,
+        "nonCoordinateLongitude": 171.05569,
         "nonCoordinatePressure": 102550.5,
         "significandOfVolumetricMixingRatio": 6018766,
     }
 
     expected_13_row = {
         "data_datetime": pd.Timestamp("2015-08-21 01:59:06"),
         "latitude": -44.77121,
-        "longitude": 171.15150000000003,
-        "nonCoordinateLatitude": -44.761320000000005,
+        "longitude": 171.1515,
+        "nonCoordinateLatitude": -44.76132,
         "nonCoordinateLongitude": 171.04379,
         "nonCoordinatePressure": 8556.9,
         "significandOfVolumetricMixingRatio": 8533734,
     }
 
+    ref_1 = pd.DataFrame(expected_first_row, index=[0])
+    ref_2 = pd.DataFrame(expected_second_row, index=[1])
+    ref_12 = pd.DataFrame(expected_12_row, index=[11])
+    ref_13 = pd.DataFrame(expected_13_row, index=[12])
+
     res = pdbufr.read_bufr(
         TEST_DATA_8, columns=columns, filters={"firstOrderStatistics": 15}
     )
 
     assert len(res) == 128 * 12 * 3
-
-    assert res.iloc[0].to_dict() == expected_first_row
-    assert res.iloc[1].to_dict() == expected_second_row
-    assert res.iloc[11].to_dict() == expected_12_row
-    assert res.iloc[12].to_dict() == expected_13_row
+    assert_frame_equal(res[0:1], ref_1[res.columns])
+    assert_frame_equal(res[1:2], ref_2[res.columns])
+    assert_frame_equal(res[11:12], ref_12[res.columns])
+    assert_frame_equal(res[12:13], ref_13[res.columns])
 
 
 def assert_simple_key_core(path, param, key, key_value, ref, part=False):
     # type: (str, str, str, T.Any, T.Any, bool) -> None
     columns = [param, key]
     filters = {key: key_value}
 
@@ -778,15 +795,15 @@
         else:
             assert len(res) == ref_cnt
             np.allclose(res[param], ref)
     else:
         assert len(res) == ref_cnt
 
 
-def test_bufr_header():
+def test_bufr_header() -> None:
     ref = np.array([26, 302, 2835, 38, 30, 11, 567])
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "edition", 3, ref)
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "edition", 4, None)
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "edition", [3, 4], ref)
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "bufrHeaderCentre", 98, ref)
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "bufrHeaderCentre", 1, None)
     # assert_simple_key_core(TEST_DATA_10, "heightOfStation", "bufrHeaderCentre", "ecmf", ref)
@@ -812,15 +829,15 @@
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "dataCategory", 1, None)
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "dataSubCategory", 101, ref)
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "dataSubCategory", 1, None)
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "rdbType", 5, ref)
     assert_simple_key_core(TEST_DATA_10, "heightOfStation", "rdbType", 1, None)
 
 
-def test_ident():
+def test_ident() -> None:
     assert_simple_key_core(
         TEST_DATA_10, "airTemperature", "ident", "91348", np.array([298.4]), part=True
     )
 
     assert_simple_key_core(
         TEST_DATA_10,
         "airTemperature",
@@ -868,15 +885,15 @@
     ref_cnt = len(ref_param) if ref_param is not None else 0
     assert len(res) == ref_cnt
     if ref_cnt > 0:
         np.allclose(res[param], ref_param)
         np.allclose(res["pressure"], ref_pressure)
 
 
-def test_temp_profile():
+def test_temp_profile() -> None:
     assert_temp_profile_core(
         TEST_DATA_10,
         "airTemperature",
         32,
         np.array([259.7, 258.1, 253.1, 241.7, 228.1, 219.1, 216.3]),
         np.array([100000, 92500, 85000, 70000, 50000, 40000, 30000]),
     )
@@ -968,15 +985,15 @@
             assert len(res) == ref_cnt
             np.allclose(res[param], ref_param)
             np.allclose(res[coord_key_1], ref_level)
     else:
         assert len(res) == ref_cnt
 
 
-def test_nested_coords():
+def test_nested_coords() -> None:
     # uncompressed
     assert_nested_coords_core(
         TEST_DATA_7,
         "airTemperatureAt2M",
         "ensembleMemberNumber",
         4,
         "timePeriod",
@@ -1042,47 +1059,64 @@
             ]
         ),
         np.array([15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15]),
         part=True,
     )
 
 
-@pytest.mark.xfail
-def test_new_synop_data():
-    columns = (
+def test_new_synop_data() -> None:
+    columns_1 = (
         "stationNumber",
         "heightOfStationGroundAboveMeanSeaLevel",
         "heightOfSensorAboveLocalGroundOrDeckOfMarinePlatform",
         "airTemperature",
         "dewpointTemperature",
     )
 
     expected_first_row = {
-        "stationNumber": 948.0,
+        "stationNumber": 948,
         "heightOfStationGroundAboveMeanSeaLevel": 91.0,
         "heightOfSensorAboveLocalGroundOrDeckOfMarinePlatform": 1.5,
         "airTemperature": 300.45,
-        "dewpointTemperature": 295.15000000000003,
+        "dewpointTemperature": 295.15,
     }
 
     expected_second_row = {
-        "stationNumber": 766.0,
+        "stationNumber": 766,
         "heightOfStationGroundAboveMeanSeaLevel": 748.1,
         "heightOfSensorAboveLocalGroundOrDeckOfMarinePlatform": 2,
         "airTemperature": 269.25,
         "dewpointTemperature": 263.55,
     }
 
     expected_third_row = {
-        "stationNumber": 3950.0,
-        "heightOfStationGroundAboveMeanSeaLevel": 748.1,
+        "stationNumber": 257,
+        "heightOfStationGroundAboveMeanSeaLevel": 3950.0,
         "heightOfSensorAboveLocalGroundOrDeckOfMarinePlatform": 1.5,
         "airTemperature": 276.35,
         "dewpointTemperature": 263.05,
     }
 
-    res = pdbufr.read_bufr(TEST_DATA_12, columns=columns)
+    ref = pd.DataFrame([expected_first_row, expected_second_row, expected_third_row])
+
+    res = pdbufr.read_bufr(TEST_DATA_12, columns=columns_1)
 
     assert len(res) == 3
-    assert res.iloc[0].to_dict() == expected_first_row
-    assert res.iloc[1].to_dict() == expected_second_row
-    assert res.iloc[2].to_dict() == expected_third_row
+    assert_frame_equal(res, ref[res.columns])
+
+    columns_2 = (
+        "stationNumber",
+        "heightOfStationGroundAboveMeanSeaLevel",
+        "heightOfSensorAboveLocalGroundOrDeckOfMarinePlatform",
+        "airTemperature",
+        "dewpointTemperature",
+        "windDirection",
+        "windSpeed",
+    )
+    filters = {
+        "heightOfSensorAboveLocalGroundOrDeckOfMarinePlatform": slice(1, 20),
+    }
+    res = pdbufr.read_bufr(
+        TEST_DATA_12, columns=columns_2, filters=filters, required_columns=False
+    )
+
+    assert len(res) == 14
```

