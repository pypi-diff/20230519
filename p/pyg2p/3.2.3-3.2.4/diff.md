# Comparing `tmp/pyg2p-3.2.3.tar.gz` & `tmp/pyg2p-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyg2p-3.2.3.tar", last modified: Wed Apr 26 09:40:42 2023, max compression
+gzip compressed data, was "dist/pyg2p-3.2.4.tar", last modified: Fri May 19 09:37:07 2023, max compression
```

## Comparing `pyg2p-3.2.3.tar` & `pyg2p-3.2.4.tar`

### file list

```diff
@@ -1,157 +1,167 @@
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    13760 2023-04-26 09:09:26.000000 pyg2p-3.2.3/LICENSE
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       84 2023-04-26 09:09:26.000000 pyg2p-3.2.3/MANIFEST.in
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    47878 2023-04-26 09:40:42.000000 pyg2p-3.2.3/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    46863 2023-04-26 09:09:26.000000 pyg2p-3.2.3/README.md
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/bin/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      191 2023-04-26 09:09:26.000000 pyg2p-3.2.3/bin/pyg2p
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/configuration/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/ftp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/geopotentials.json
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/configuration/global/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      100 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/ftp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2946 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/geopotentials.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      149 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/global_conf.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    36594 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/intertables.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7000 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/parameters.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      155 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/test.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/intertables.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        3 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/parameters.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      214 2023-04-26 09:09:26.000000 pyg2p-3.2.3/requirements.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-04-26 09:40:42.000000 pyg2p-3.2.3/setup.cfg
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6305 2023-04-26 09:09:26.000000 pyg2p-3.2.3/setup.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/VERSION
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7644 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4261 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/exceptions.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2334 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    15678 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/api.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    14257 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/config.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    22879 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/context.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8033 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/controller.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    19605 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    11019 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/grib_interpolation_lib.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2020 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/latlong.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    50993 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/scipy_interpolation_lib.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    14068 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/aggregator.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1752 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/conversion.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4907 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/correction.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/readers/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       61 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/readers/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    11805 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/readers/grib.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3116 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/readers/netcdf.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1386 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/readers/pcr.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/writers/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6837 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/writers/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8513 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/writers/netcdf.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1952 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/writers/pcr.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/util/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2978 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/files.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      593 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/generics.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      940 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/numeric.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/util/profiling/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/profiling/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    24815 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/profiling/profilehooks.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      970 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/strings.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    47878 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4206 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/SOURCES.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/dependency_links.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      132 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/requires.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        6 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/top_level.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-04-26 09:25:41.000000 pyg2p-3.2.3/src/pyg2p.egg-info/zip-safe
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      112 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/templates/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      655 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_cp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      658 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_lsp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_rg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_rn.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_ta.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_td.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_wu.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_wv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_15d.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_15d_glob.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      520 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy_inv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy_nn.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      650 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_agg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      592 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_december.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      565 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/UKMO_t24_LA.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/UKMO_t24_LA_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      854 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/UKMO_t24_LA_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      536 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cin.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      665 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      739 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_e06_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      617 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      677 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      751 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_r06_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      629 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      809 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      885 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_t24_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      743 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      694 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06_2.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06_3.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      646 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      737 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      642 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      715 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06_efas.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      683 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06_gmi.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      614 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      881 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_t24_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      740 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwdl_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/efas_sro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      710 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      705 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_r24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_r24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      821 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      654 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_e24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      649 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_e24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      656 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_15days.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_15days_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_15days_noagg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      742 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_15days_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      773 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/glofas_sro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      699 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/glofas_sro_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/glofas_ssro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      702 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/glofas_ssro_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      807 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      817 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_global.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      675 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_global_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      684 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      812 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_scipy_global.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      670 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_scipy_global_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_scipy_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      631 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/rn_false_mv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      647 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_r06_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      714 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_r06_scipy_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      789 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      855 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_t24_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      790 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_t24_scipy_rotated.json
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    13760 2023-02-15 12:18:09.000000 pyg2p-3.2.4/LICENSE
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       84 2023-02-20 17:30:36.000000 pyg2p-3.2.4/MANIFEST.in
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    47858 2023-05-19 09:37:07.000000 pyg2p-3.2.4/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    46863 2023-04-26 09:56:42.000000 pyg2p-3.2.4/README.md
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/bin/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      191 2023-02-15 12:18:09.000000 pyg2p-3.2.4/bin/pyg2p
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/configuration/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/ftp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/geopotentials.json
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/configuration/global/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      100 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/global/ftp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3225 2023-05-19 09:35:08.000000 pyg2p-3.2.4/configuration/global/geopotentials.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      149 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/global/global_conf.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    41874 2023-05-19 09:35:08.000000 pyg2p-3.2.4/configuration/global/intertables.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8250 2023-05-19 09:35:08.000000 pyg2p-3.2.4/configuration/global/parameters.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      155 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/global/test.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/intertables.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        3 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/parameters.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      214 2023-02-15 12:18:09.000000 pyg2p-3.2.4/requirements.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-05-19 09:37:07.000000 pyg2p-3.2.4/setup.cfg
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7115 2023-05-19 09:35:08.000000 pyg2p-3.2.4/setup.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2023-05-19 09:35:08.000000 pyg2p-3.2.4/src/pyg2p/VERSION
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7644 2023-05-17 14:15:45.000000 pyg2p-3.2.4/src/pyg2p/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4261 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/exceptions.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2334 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    15678 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/api.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    14257 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/config.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    22879 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/context.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8033 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/controller.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    19605 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    11019 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/grib_interpolation_lib.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2020 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/latlong.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    50993 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/scipy_interpolation_lib.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    14068 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/aggregator.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1752 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/conversion.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4907 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/correction.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/readers/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       61 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/readers/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    11805 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/readers/grib.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3116 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/readers/netcdf.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1386 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/readers/pcr.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/writers/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     6837 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/writers/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8513 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/writers/netcdf.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2012 2023-05-19 09:35:08.000000 pyg2p-3.2.4/src/pyg2p/main/writers/pcr.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/util/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2978 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/files.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      593 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/generics.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      940 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/numeric.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/util/profiling/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/profiling/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    24815 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/profiling/profilehooks.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      970 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/strings.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    47858 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4419 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      132 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/requires.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        6 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/top_level.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-02-20 16:19:14.000000 pyg2p-3.2.4/src/pyg2p.egg-info/zip-safe
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      112 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/templates/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      655 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_cp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      658 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_lsp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_rg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_rn.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_ta.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_td.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_wu.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_wv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_15d.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_15d_glob.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      520 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy_inv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy_nn.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      650 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_agg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      592 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_december.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      565 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/UKMO_t24_LA.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/UKMO_t24_LA_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      854 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/UKMO_t24_LA_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      536 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cin.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      665 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      739 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_e06_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      617 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      677 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      751 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_r06_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      629 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      809 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      885 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_t24_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      743 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      694 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06_2.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06_3.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      646 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      737 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      642 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      715 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06_efas.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      683 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06_gmi.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      614 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      881 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_t24_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      740 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwdl_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/efas_sro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      710 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      705 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_r24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_r24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      821 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      654 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_e24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      649 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_e24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      656 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_15days.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_15days_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_15days_noagg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      742 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_15days_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      773 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/glofas_sro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      699 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/glofas_sro_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/glofas_ssro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      702 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/glofas_ssro_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      807 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      817 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_global.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      675 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_global_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      684 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      812 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_scipy_global.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      670 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_scipy_global_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_scipy_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      631 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/rn_false_mv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      647 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_r06_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      714 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_r06_scipy_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      789 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      855 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_t24_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      790 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_t24_scipy_rotated.json
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/tests/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4666 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_aggregator.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8785 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_api.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      938 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_conversion.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2786 2023-04-26 09:56:42.000000 pyg2p-3.2.4/tests/test_correction.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     6597 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_interpolation.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2246 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_oracle_data.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1997 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_readers.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      669 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_strings.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       76 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_writers.py
```

### Comparing `pyg2p-3.2.3/LICENSE` & `pyg2p-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/PKG-INFO` & `pyg2p-3.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyg2p
-Version: 3.2.3
+Version: 3.2.4
 Summary: Convert GRIB files to netCDF or PCRaster
 Author: Domenico Nappo
 Author-email: domenico.nappo@gmail.com
 License: EUPL 1.2
 Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -1274,9 +1273,7 @@
         time: Unlimited dimension for time steps
 Variables:
         lon: 2D array with shape (yc, xc)
         lat: 2D array with shape (yc, xc)
         time_nc: 1D array of values representing hours/days since dataDate of first grib message (endStep)
         values_nc: a 3D array of dimensions (time, yc, xc), with coordinates set to 'lon, lat'.
 ```
-
-
```

### Comparing `pyg2p-3.2.3/README.md` & `pyg2p-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/configuration/global/geopotentials.json` & `pyg2p-3.2.4/configuration/global/geopotentials.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.92%*

 * *Differences: {"'-25$15$1001$601$601601$rotated_ll'": "'cosmo_z_seemhews.grib'",*

 * * "'7$49$1556$1066$1644290$regular_ll'": "'nmmb_z_seemhews.grib'",*

 * * "'9.4$44.98$1187$1049$1244967$regular_ll'": "'alsmws_verif_geop_seemhews.grb2'",*

 * * "'9.4$45$1425$961$1369425$regular_ll'": "'icon_gp_seemhews.grib'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "-10$40$140$112$15680$regular_ll": "dwd_grib1_ispra_gmi_20110417.geo.grib",
     "-12$14$306$258$78948$rotated_ll": "cosmos_geopotential.grib",
     "-15.75$16.125$511$415$212065$rotated_ll": "cosmo7km.grb",
     "-16$7$393$338$132834$rotated_ll": "imprints_ex_const_c7.grib1",
     "-18$23.5$665$657$436905$rotated_ll": "dwd_grib1_ispra_LME_2012111900.grib",
+    "-25$15$1001$601$601601$rotated_ll": "cosmo_z_seemhews.grib",
     "-32$53$341$161$54901$regular_ll": "025x025_54901.grb",
     "-35$45$161$91$14651$regular_ll": "europe_0.5_degree_T799.grb",
     "-35$45$81$46$3726$regular_ll": "europe_1_degree_T399.grb",
     "-40$80$M$106$14996$reduced_gg": "efhs_14996.grb",
     "-40$80$M$214$41826$reduced_gg": "O320_p80_m40_p20_p80.grb",
     "-40$80$M$214$58717$reduced_gg": "efhs_58717.grb",
     "-40$80$M$427$164585$reduced_gg": "O640_p80_m40_p20_p80.grb",
@@ -40,9 +41,12 @@
     "344.25$16.125$511$415$212065$rotated_ll": "arpa_orography.grib",
     "345$17$129$105$13545$regular_ll": "meteo_france_orography.grib",
     "346.325$11.075$496$372$184512$rotated_ll": "dmi_orography.grib",
     "350$40$201$161$32361$regular_ll": "dwd_gme_2004_72_i256_geo.grib2",
     "350$40.04$201$161$32361$regular_ll": "icon_32361.grb",
     "354.9108$363.3107$421$548$230708$rotated_ll": "ukmo_orography.grib",
     "355$5.5$421$461$194081$rotated_ll": "dwd_orography.grib",
-    "37$47$101$111$11211$regular_ll": "africa_01_degrees.grb"
+    "37$47$101$111$11211$regular_ll": "africa_01_degrees.grb",
+    "7$49$1556$1066$1644290$regular_ll": "nmmb_z_seemhews.grib",
+    "9.4$44.98$1187$1049$1244967$regular_ll": "alsmws_verif_geop_seemhews.grb2",
+    "9.4$45$1425$961$1369425$regular_ll": "icon_gp_seemhews.grib"
 }
```

### Comparing `pyg2p-3.2.3/configuration/global/intertables.json` & `pyg2p-3.2.4/configuration/global/intertables.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8706896551724138%*

 * *Differences: {"'I-15.75_16.125_511_415_212065_rotated_ll_-1700000_1360000_1000_-1000_0.00_60.22_-1700000_1360000_1000_-1000_-10.32_37.93scipy_nearest'": "OrderedDict([('filename', "*

 * *                                                                                                                                            "'cos_212065_to_2878x3479_nearest.npy'), "*

 * *                                                                                                                                            "('method', "*

 * *       […]*

```diff
@@ -50,14 +50,25 @@
             32361
         ],
         "target_shape": [
             950,
             1000
         ]
     },
+    "I-15.75_16.125_511_415_212065_rotated_ll_-1700000_1360000_1000_-1000_0.00_60.22_-1700000_1360000_1000_-1000_-10.32_37.93scipy_nearest": {
+        "filename": "cos_212065_to_2878x3479_nearest.npy",
+        "method": "nearest",
+        "source_shape": [
+            212065
+        ],
+        "target_shape": [
+            2980,
+            3570
+        ]
+    },
     "I-15.75_16.125_511_415_212065_rotated_ll_-1700000_2700000_5000_-5000_34.12_72.41_-1700000_2700000_5000_-5000_-33.50_51.50scipy_nearest": {
         "filename": "cos_212065_to_810x680_nearest.npy",
         "method": "nearest",
         "source_shape": [
             212065
         ],
         "target_shape": [
@@ -105,14 +116,25 @@
             212065
         ],
         "target_shape": [
             2981,
             3571
         ]
     },
+    "I-15.75_16.125_511_415_212065_rotated_ll_2614000_4078000_1000_-1000_32.03_59.80_2614000_4078000_1000_-1000_-10.48_36.57scipy_nearest": {
+        "filename": "cos_212065_to_2878x3479_nearest.npy",
+        "method": "nearest",
+        "source_shape": [
+            212065
+        ],
+        "target_shape": [
+            2878,
+            3479
+        ]
+    },
     "I-18_23.5_665_657_436905_rotated_ll_-1700000_2700000_5000_-5000_-14.19_21.00_-1700000_2700000_5000_-5000_-16.50_15.75grib_nearest": {
         "filename": "tbl_dwdgrib1is_550800_grib_nearest.npy",
         "method": "grib_nearest",
         "source_shape": [
             436905
         ],
         "target_shape": [
@@ -160,14 +182,25 @@
             436905
         ],
         "target_shape": [
             950,
             1000
         ]
     },
+    "I-25_15_1001_601_601601_rotated_ll_4790000_2550000_5000_-5000_43.34_45.87_4790000_2550000_5000_-5000_15.83_19.90scipy_nearest": {
+        "filename": "tbl_csm_3111_scipy_nearest.npy",
+        "method": "nearest",
+        "source_shape": [
+            601601
+        ],
+        "target_shape": [
+            51,
+            61
+        ]
+    },
     "I-32_53_341_161_54901_regular_ll_-1700000_2700000_5000_-5000_34.12_72.41_-1700000_2700000_5000_-5000_-33.50_51.50scipy_nearest": {
         "filename": "025x025_54901_to_810x680_nearest.npy",
         "method": "nearest",
         "source_shape": [
             54901
         ],
         "target_shape": [
@@ -369,14 +402,25 @@
             542080
         ],
         "target_shape": [
             810,
             680
         ]
     },
+    "I0_359.718_M_640_542080_reduced_gg_-179_-59_0_0_-59.97_89.97_-179_-59_0_0_-179.97_179.97scipy_bilinear": {
+        "filename": "tbl_1_det0to1_21600000_scipy_bilinear.npy.gz",
+        "method": "bilinear",
+        "source_shape": [
+            542080
+        ],
+        "target_shape": [
+            3000,
+            7200
+        ]
+    },
     "I0_359.718_M_640_542080_reduced_gg_-180_90_0_0_-59.95_89.95_-180_90_0_0_0.05_359.95grib_nearest": {
         "filename": "tbl_en0to10_5400000_grib_nearest.npy",
         "method": "grib_nearest",
         "source_shape": [
             542080
         ],
         "target_shape": [
@@ -468,14 +512,36 @@
             421120
         ],
         "target_shape": [
             810,
             680
         ]
     },
+    "I0_359.722_M_640_421120_reduced_gg_-179_-59_0_0_-59.97_89.97_-179_-59_0_0_-179.97_179.97scipy_bilinear": {
+        "filename": "tbl_1_fcroo6400_21600000_scipy_bilinear.npy.gz",
+        "method": "bilinear",
+        "source_shape": [
+            421120
+        ],
+        "target_shape": [
+            3000,
+            7200
+        ]
+    },
+    "I0_359.722_M_640_421120_reduced_gg_-179_-89_0_0_-89.97_89.97_-179_-89_0_0_-179.97_179.97scipy_bilinear": {
+        "filename": "tbl_fcroo6400_25920000_scipy_bilinear.npy.gz",
+        "method": "bilinear",
+        "source_shape": [
+            421120
+        ],
+        "target_shape": [
+            3600,
+            7200
+        ]
+    },
     "I0_359.722_M_640_421120_reduced_gg_-180_90_0_0_-59.95_89.95_-180_90_0_0_0.05_359.95grib_invdist": {
         "filename": "tbl_1_8_grb_5400000_grib_invdist.npy",
         "method": "grib_invdist",
         "source_shape": [
             421120
         ],
         "target_shape": [
@@ -524,14 +590,36 @@
             421120
         ],
         "target_shape": [
             950,
             1000
         ]
     },
+    "I0_359.723_M_640_421120_reduced_gg_-179_-59_0_0_-59.97_89.97_-179_-59_0_0_-179.97_179.97scipy_bilinear": {
+        "filename": "tbl_1_fcinsto640_21600000_scipy_bilinear.npy.gz",
+        "method": "bilinear",
+        "source_shape": [
+            421120
+        ],
+        "target_shape": [
+            3000,
+            7200
+        ]
+    },
+    "I0_359.723_M_640_421120_reduced_gg_-179_-89_0_0_-89.97_89.97_-179_-89_0_0_-179.97_179.97scipy_bilinear": {
+        "filename": "tbl_1_fcinsto640_25920000_scipy_bilinear.npy.gz",
+        "method": "bilinear",
+        "source_shape": [
+            421120
+        ],
+        "target_shape": [
+            3600,
+            7200
+        ]
+    },
     "I0_359.723_M_640_421120_reduced_gg_-180_90_0_0_-59.95_89.95_-180_90_0_0_0.05_359.95scipy_nearest": {
         "filename": "O320_421120B_to_1500x3600_nearest.npy",
         "method": "nearest",
         "source_shape": [
             421120
         ],
         "target_shape": [
@@ -624,14 +712,36 @@
             1661440
         ],
         "target_shape": [
             810,
             680
         ]
     },
+    "I0_359.86_M_1280_1661440_reduced_gg_-179_-59_0_0_-59.97_89.97_-179_-59_0_0_-179.97_179.97scipy_bilinear": {
+        "filename": "tbl_fcroo6400_21600000_scipy_bilinear.npy.gz",
+        "method": "bilinear",
+        "source_shape": [
+            1661440
+        ],
+        "target_shape": [
+            3000,
+            7200
+        ]
+    },
+    "I0_359.86_M_1280_1661440_reduced_gg_-179_-89_0_0_-89.97_89.97_-179_-89_0_0_-179.97_179.97scipy_bilinear": {
+        "filename": "tbl_fcacco6400_25920000_scipy_bilinear.npy.gz",
+        "method": "bilinear",
+        "source_shape": [
+            1661440
+        ],
+        "target_shape": [
+            3600,
+            7200
+        ]
+    },
     "I0_359.86_M_1280_1661440_reduced_gg_-180_90_0_0_-59.95_89.95_-180_90_0_0_0.05_359.95grib_invdist": {
         "filename": "tbl_8_grb_5400000_grib_invdist.npy",
         "method": "grib_invdist",
         "source_shape": [
             1661440
         ],
         "target_shape": [
@@ -734,14 +844,25 @@
             6599680
         ],
         "target_shape": [
             950,
             1000
         ]
     },
+    "I0_359.929_M_2560_6599680_reduced_gg_4790000_2550000_5000_-5000_43.34_45.87_4790000_2550000_5000_-5000_15.83_19.90scipy_nearest": {
+        "filename": "tbl_1_2021061700_3111_scipy_nearest.npy",
+        "method": "nearest",
+        "source_shape": [
+            6599680
+        ],
+        "target_shape": [
+            51,
+            61
+        ]
+    },
     "I0_359.93_M_2560_6599680_reduced_gg_-180_90_0_0_-59.95_89.95_-180_90_0_0_0.05_359.95scipy_nearest": {
         "filename": "N640@O1280_6599680_to_1500x3600_nearest.npy",
         "method": "nearest",
         "source_shape": [
             6599680
         ],
         "target_shape": [
@@ -1107,9 +1228,53 @@
         "source_shape": [
             194081
         ],
         "target_shape": [
             810,
             680
         ]
+    },
+    "I7_49_1556_1066_1644290_regular_ll_4790000_2550000_5000_-5000_43.34_45.87_4790000_2550000_5000_-5000_15.83_19.90scipy_nearest": {
+        "filename": "tbl_nmmb_3111_scipy_nearest.npy",
+        "method": "nearest",
+        "source_shape": [
+            1658696
+        ],
+        "target_shape": [
+            51,
+            61
+        ]
+    },
+    "I7_49_1556_1066_1658696_regular_ll_4790000_2550000_5000_-5000_43.34_45.87_4790000_2550000_5000_-5000_15.83_19.90scipy_nearest": {
+        "filename": "tbl_1_nmmb_3111_scipy_nearest.npy",
+        "method": "nearest",
+        "source_shape": [
+            1658696
+        ],
+        "target_shape": [
+            51,
+            61
+        ]
+    },
+    "I9.4_44.98_1187_1049_1244967_regular_ll_4790000_2550000_5000_-5000_43.34_45.87_4790000_2550000_5000_-5000_15.83_19.90scipy_nearest": {
+        "filename": "tbl_2_2021061700_3111_scipy_nearest.npy",
+        "method": "nearest",
+        "source_shape": [
+            1245163
+        ],
+        "target_shape": [
+            51,
+            61
+        ]
+    },
+    "I9.4_45_1425_961_1369425_regular_ll_4790000_2550000_5000_-5000_43.34_45.87_4790000_2550000_5000_-5000_15.83_19.90scipy_nearest": {
+        "filename": "tbl_3_2021061700_3111_scipy_nearest.npy",
+        "method": "nearest",
+        "source_shape": [
+            1369425
+        ],
+        "target_shape": [
+            51,
+            61
+        ]
     }
 }
```

### Comparing `pyg2p-3.2.3/configuration/global/parameters.json` & `pyg2p-3.2.4/configuration/global/parameters.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8125%*

 * *Differences: {"'pev'": "OrderedDict([('@description', 'Potential Evaporation'), ('@shortName', 'pev'), "*

 * *          "('@unit', 'm'), ('Conversion', OrderedDict([('@cutOffNegative', True), ('@function', "*

 * *          "'x=-x*1000'), ('@id', 'tomm'), ('@unit', 'mm')]))])",*

 * * "'sd'": "OrderedDict([('@description', 'soil water equivalent'), ('@shortName', 'scov'), "*

 * *         "('@unit', 'm'), ('Conversion', OrderedDict([('@function', 'x=1000*x'), ('@id', 'tomm'), "*

 * *         "('@unit', 'mm')]))])",*

 * * "'sf'": "OrderedDict([('@descri […]*

```diff
@@ -160,14 +160,45 @@
         "Conversion": {
             "@cutOffNegative": true,
             "@function": "x=x*1000",
             "@id": "tomm",
             "@unit": "mm"
         }
     },
+    "pev": {
+        "@description": "Potential Evaporation",
+        "@shortName": "pev",
+        "@unit": "m",
+        "Conversion": {
+            "@cutOffNegative": true,
+            "@function": "x=-x*1000",
+            "@id": "tomm",
+            "@unit": "mm"
+        }
+    },
+    "sd": {
+        "@description": "soil water equivalent",
+        "@shortName": "scov",
+        "@unit": "m",
+        "Conversion": {
+            "@function": "x=1000*x",
+            "@id": "tomm",
+            "@unit": "mm"
+        }
+    },
+    "sf": {
+        "@description": "snowmelt",
+        "@shortName": "smelt",
+        "@unit": "m",
+        "Conversion": {
+            "@function": "x=1000*x",
+            "@id": "tomm",
+            "@unit": "mm"
+        }
+    },
     "slhf": {
         "@description": "surface latent heat flux",
         "@shortName": "slhf",
         "@unit": "W/(m^2)",
         "Conversion": [
             {
                 "@cutOffNegative": true,
@@ -179,14 +210,24 @@
                 "@cutOffNegative": true,
                 "@function": "x=x*(-0.00147)",
                 "@id": "tommh",
                 "@unit": "mm/h"
             }
         ]
     },
+    "smlt": {
+        "@description": "snowmelt",
+        "@shortName": "smelt",
+        "@unit": "m",
+        "Conversion": {
+            "@function": "x=1000*x",
+            "@id": "tomm",
+            "@unit": "mm"
+        }
+    },
     "sro": {
         "@description": "Surface Runoff",
         "@shortName": "sro",
         "@unit": "m",
         "Conversion": {
             "@cutOffNegative": true,
             "@function": "x=x*1000",
@@ -195,14 +236,19 @@
         }
     },
     "ssr": {
         "@description": "Surface solar radiation",
         "@shortName": "ssr",
         "@unit": "W s/m^2"
     },
+    "ssrd": {
+        "@description": "Surface solar radiation downwards",
+        "@shortName": "ssrd",
+        "@unit": "W s/m^2"
+    },
     "ssro": {
         "@description": "Sub-Surface Runoff",
         "@shortName": "ssro",
         "@unit": "m",
         "Conversion": {
             "@cutOffNegative": true,
             "@function": "x=x*1000",
@@ -211,14 +257,19 @@
         }
     },
     "str": {
         "@description": "Surface thermal radiation",
         "@shortName": "str",
         "@unit": "W s/m^2"
     },
+    "swvl1": {
+        "@description": "Soil Moisture",
+        "@shortName": "swvl1",
+        "@unit": "percentage"
+    },
     "t_2m": {
         "@description": "2 meters Temperature",
         "@shortName": "t_2m",
         "@unit": "K",
         "Conversion": {
             "@cutOffNegative": false,
             "@function": "x=x-273.15",
```

### Comparing `pyg2p-3.2.3/setup.py` & `pyg2p-3.2.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import glob
 from shutil import rmtree
 from setuptools import setup, find_packages, Command
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(os.path.join(current_dir, './src/'))
 
-import pyg2p.util.files as fm
-
 version_file = os.path.join(current_dir, 'src/pyg2p/VERSION')
 
 with open(version_file, 'r') as f:
     version = f.read().strip()
 
 readme_file = os.path.join(current_dir, 'README.md')
 with open(readme_file, 'r') as f:
@@ -78,25 +76,49 @@
         os.system('{} setup.py sdist'.format(sys.executable))
 
         self.print_console('Uploading the package to test PyPI via Twine...')
         os.system('twine upload --repository testpypi dist/*')
 
         sys.exit()
 
+def delete_files_from_dir(dir_path, prefix_=''):
+    # Gather directory contents
+    if is_dir(dir_path):
+        contents = [os.path.join(dir_path, i) for i in os.listdir(dir_path)]
+        # Iterate and remove each item in the appropriate manner
+        [os.unlink(i) for i in contents if i.startswith(prefix_)]
+
+def create_dir(pathname, recreate=False):
+    if not os.path.exists(pathname):
+        os.makedirs(pathname)
+    elif recreate:
+        delete_files_from_dir(pathname)
+        os.rmdir(pathname)
+        os.makedirs(pathname)
+
+def is_dir(pathname):
+    return os.path.isdir(pathname) and pathname not in ('.', '..', './', '../')
+
+def exists(pathname, is_folder=False):
+    return os.path.exists(pathname) and (os.path.isdir(pathname) if is_folder else os.path.isfile(pathname))
+
+def filename(pathname):
+    return os.path.basename(pathname)
+
 def setup_data_files(setup_args_):
     user_conf_dir = f'{os.path.expanduser("~")}/.pyg2p/'
-    fm.create_dir(user_conf_dir)
+    create_dir(user_conf_dir)
     list_files = {t: [os.path.join(t, f) for f in os.listdir(t) if f.endswith('.json')]
                   for t in ('./templates',
                             './configuration',
                             './configuration/global')}
     for_user_to_copy = [f for f in list_files['./configuration'] if
-                        not fm.exists(os.path.join(user_conf_dir, fm.filename(f)))]
+                        not exists(os.path.join(user_conf_dir, filename(f)))]
     templates_to_copy = [f for f in list_files['./templates'] if
-                         not fm.exists(os.path.join(user_conf_dir, 'templates_samples', fm.filename(f)))]
+                         not exists(os.path.join(user_conf_dir, 'templates_samples', filename(f)))]
     data_files = [('pyg2p/configuration/', list_files['./configuration/global'])]
 
     if for_user_to_copy:
         data_files.append((user_conf_dir, for_user_to_copy))
     if templates_to_copy:
         data_files.append((os.path.join(user_conf_dir, 'templates_samples'), templates_to_copy))
     setup_args_.update({'data_files': data_files})
```

### Comparing `pyg2p-3.2.3/src/pyg2p/__init__.py` & `pyg2p-3.2.4/src/pyg2p/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/exceptions.py` & `pyg2p-3.2.4/src/pyg2p/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/__init__.py` & `pyg2p-3.2.4/src/pyg2p/main/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/api.py` & `pyg2p-3.2.4/src/pyg2p/main/api.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/config.py` & `pyg2p-3.2.4/src/pyg2p/main/config.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/context.py` & `pyg2p-3.2.4/src/pyg2p/main/context.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/controller.py` & `pyg2p-3.2.4/src/pyg2p/main/controller.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/interpolation/__init__.py` & `pyg2p-3.2.4/src/pyg2p/main/interpolation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/interpolation/grib_interpolation_lib.py` & `pyg2p-3.2.4/src/pyg2p/main/interpolation/grib_interpolation_lib.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/interpolation/latlong.py` & `pyg2p-3.2.4/src/pyg2p/main/interpolation/latlong.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/interpolation/scipy_interpolation_lib.py` & `pyg2p-3.2.4/src/pyg2p/main/interpolation/scipy_interpolation_lib.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/manipulation/aggregator.py` & `pyg2p-3.2.4/src/pyg2p/main/manipulation/aggregator.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/manipulation/conversion.py` & `pyg2p-3.2.4/src/pyg2p/main/manipulation/conversion.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/manipulation/correction.py` & `pyg2p-3.2.4/src/pyg2p/main/manipulation/correction.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/readers/grib.py` & `pyg2p-3.2.4/src/pyg2p/main/readers/grib.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/readers/netcdf.py` & `pyg2p-3.2.4/src/pyg2p/main/readers/netcdf.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/readers/pcr.py` & `pyg2p-3.2.4/src/pyg2p/main/readers/pcr.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/writers/__init__.py` & `pyg2p-3.2.4/src/pyg2p/main/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/writers/netcdf.py` & `pyg2p-3.2.4/src/pyg2p/main/writers/netcdf.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/main/writers/pcr.py` & `pyg2p-3.2.4/src/pyg2p/main/writers/pcr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from osgeo import gdal
 import numpy.ma as ma
+import numpy as np
 
 from pyg2p.main.writers import Writer
 
 
 class PCRasterWriter(Writer):
     FORMAT = 'PCRaster'
 
@@ -25,14 +26,15 @@
         rows = self._src_ds.RasterYSize
         rs = self._src_band.ReadAsArray(0, 0, cols, rows)
         self.mv = self._src_band.GetNoDataValue()
         rs = ma.masked_values(rs, self.mv)
         self._mask = ma.getmask(rs)
 
     def write(self, output_map_name, values):
+        values[np.isnan(values)]=self.mv
         drv = gdal.GetDriverByName(self.FORMAT)
         masked_values = self._mask_values(values)
         n = ma.count_masked(masked_values)
         self._mem_ds.GetRasterBand(1).SetNoDataValue(self.mv)
         self._mem_ds.GetRasterBand(1).WriteArray(masked_values)
         out_ds = drv.CreateCopy(output_map_name.encode('utf-8'), self._mem_ds)
         self._log(f'{output_map_name} written!', 'INFO')
```

### Comparing `pyg2p-3.2.3/src/pyg2p/util/files.py` & `pyg2p-3.2.4/src/pyg2p/util/files.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/util/generics.py` & `pyg2p-3.2.4/src/pyg2p/util/generics.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/util/numeric.py` & `pyg2p-3.2.4/src/pyg2p/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/util/profiling/profilehooks.py` & `pyg2p-3.2.4/src/pyg2p/util/profiling/profilehooks.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p/util/strings.py` & `pyg2p-3.2.4/src/pyg2p/util/strings.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/src/pyg2p.egg-info/PKG-INFO` & `pyg2p-3.2.4/src/pyg2p.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyg2p
-Version: 3.2.3
+Version: 3.2.4
 Summary: Convert GRIB files to netCDF or PCRaster
 Author: Domenico Nappo
 Author-email: domenico.nappo@gmail.com
 License: EUPL 1.2
 Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -1274,9 +1273,7 @@
         time: Unlimited dimension for time steps
 Variables:
         lon: 2D array with shape (yc, xc)
         lat: 2D array with shape (yc, xc)
         time_nc: 1D array of values representing hours/days since dataDate of first grib message (endStep)
         values_nc: a 3D array of dimensions (time, yc, xc), with coordinates set to 'lon, lat'.
 ```
-
-
```

### Comparing `pyg2p-3.2.3/src/pyg2p.egg-info/SOURCES.txt` & `pyg2p-3.2.4/src/pyg2p.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -133,8 +133,17 @@
 templates/tigge_lam_r06.json
 templates/tigge_lam_r06_rotated.json
 templates/tigge_lam_r06_scipy.json
 templates/tigge_lam_r06_scipy_rotated.json
 templates/tigge_lam_t24.json
 templates/tigge_lam_t24_rotated.json
 templates/tigge_lam_t24_scipy.json
-templates/tigge_lam_t24_scipy_rotated.json
+templates/tigge_lam_t24_scipy_rotated.json
+tests/test_aggregator.py
+tests/test_api.py
+tests/test_conversion.py
+tests/test_correction.py
+tests/test_interpolation.py
+tests/test_oracle_data.py
+tests/test_readers.py
+tests/test_strings.py
+tests/test_writers.py
```

### Comparing `pyg2p-3.2.3/templates/AFFS_cp.json` & `pyg2p-3.2.4/templates/AFFS_cp.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/AFFS_lsp.json` & `pyg2p-3.2.4/templates/AFFS_lsp.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/AFFS_rg.json` & `pyg2p-3.2.4/templates/AFFS_rg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/AFFS_rn.json` & `pyg2p-3.2.4/templates/AFFS_rn.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/AFFS_ta.json` & `pyg2p-3.2.4/templates/AFFS_ta.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/AFFS_td.json` & `pyg2p-3.2.4/templates/AFFS_td.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/AFFS_wu.json` & `pyg2p-3.2.4/templates/AFFS_wu.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/AFFS_wv.json` & `pyg2p-3.2.4/templates/AFFS_wv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_15d.json` & `pyg2p-3.2.4/templates/EUE_15d.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_15d_glob.json` & `pyg2p-3.2.4/templates/EUE_15d_glob.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim.json` & `pyg2p-3.2.4/templates/EUE_RainAnim.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim_CV.json` & `pyg2p-3.2.4/templates/EUE_RainAnim_CV.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim_CV_g.json` & `pyg2p-3.2.4/templates/EUE_RainAnim_CV_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy.json` & `pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy_inv.json` & `pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy_inv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy_nn.json` & `pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy_nn.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim_agg.json` & `pyg2p-3.2.4/templates/EUE_RainAnim_agg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim_december.json` & `pyg2p-3.2.4/templates/EUE_RainAnim_december.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim_g.json` & `pyg2p-3.2.4/templates/EUE_RainAnim_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/EUE_RainAnim_scipy.json` & `pyg2p-3.2.4/templates/EUE_RainAnim_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/UKMO_t24_LA.json` & `pyg2p-3.2.4/templates/UKMO_t24_LA.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/UKMO_t24_LA_g.json` & `pyg2p-3.2.4/templates/UKMO_t24_LA_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/UKMO_t24_LA_scipy.json` & `pyg2p-3.2.4/templates/UKMO_t24_LA_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cin.json` & `pyg2p-3.2.4/templates/cin.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cosmo_e06.json` & `pyg2p-3.2.4/templates/cosmo_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cosmo_e06_newmaps.json` & `pyg2p-3.2.4/templates/cosmo_e06_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cosmo_e06_scipy.json` & `pyg2p-3.2.4/templates/cosmo_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cosmo_r06.json` & `pyg2p-3.2.4/templates/cosmo_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cosmo_r06_newmaps.json` & `pyg2p-3.2.4/templates/cosmo_r06_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cosmo_r06_scipy.json` & `pyg2p-3.2.4/templates/cosmo_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cosmo_t24.json` & `pyg2p-3.2.4/templates/cosmo_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cosmo_t24_newmaps.json` & `pyg2p-3.2.4/templates/cosmo_t24_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/cosmo_t24_scipy.json` & `pyg2p-3.2.4/templates/cosmo_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_e06.json` & `pyg2p-3.2.4/templates/dwd_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_e06_2.json` & `pyg2p-3.2.4/templates/dwd_e06_2.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_e06_2nd.json` & `pyg2p-3.2.4/templates/dwd_e06_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_e06_3.json` & `pyg2p-3.2.4/templates/dwd_e06_3.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_e06_scipy.json` & `pyg2p-3.2.4/templates/dwd_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_r06.json` & `pyg2p-3.2.4/templates/dwd_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_r06_2nd.json` & `pyg2p-3.2.4/templates/dwd_r06_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_r06_efas.json` & `pyg2p-3.2.4/templates/dwd_r06_efas.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_r06_gmi.json` & `pyg2p-3.2.4/templates/dwd_r06_gmi.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_r06_scipy.json` & `pyg2p-3.2.4/templates/dwd_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_t24.json` & `pyg2p-3.2.4/templates/dwd_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_t24_2nd.json` & `pyg2p-3.2.4/templates/dwd_t24_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwd_t24_scipy.json` & `pyg2p-3.2.4/templates/dwd_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/dwdl_r06.json` & `pyg2p-3.2.4/templates/dwdl_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/efas_sro.json` & `pyg2p-3.2.4/templates/efas_sro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eud_e06.json` & `pyg2p-3.2.4/templates/eud_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eud_e06_scipy.json` & `pyg2p-3.2.4/templates/eud_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eud_r06.json` & `pyg2p-3.2.4/templates/eud_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eud_r06_scipy.json` & `pyg2p-3.2.4/templates/eud_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eud_r24.json` & `pyg2p-3.2.4/templates/eud_r24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eud_r24_scipy.json` & `pyg2p-3.2.4/templates/eud_r24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eud_t24.json` & `pyg2p-3.2.4/templates/eud_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eud_t24_scipy.json` & `pyg2p-3.2.4/templates/eud_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_e24.json` & `pyg2p-3.2.4/templates/eue_e24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_e24_scipy.json` & `pyg2p-3.2.4/templates/eue_e24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_r24.json` & `pyg2p-3.2.4/templates/eue_r24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_r24_15days.json` & `pyg2p-3.2.4/templates/eue_r24_15days.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_r24_15days_g.json` & `pyg2p-3.2.4/templates/eue_r24_15days_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_r24_15days_noagg.json` & `pyg2p-3.2.4/templates/eue_r24_15days_noagg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_r24_15days_scipy.json` & `pyg2p-3.2.4/templates/eue_r24_15days_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_r24_scipy.json` & `pyg2p-3.2.4/templates/eue_r24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_t24.json` & `pyg2p-3.2.4/templates/eue_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/eue_t24_scipy.json` & `pyg2p-3.2.4/templates/eue_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/glofas_sro.json` & `pyg2p-3.2.4/templates/glofas_sro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/glofas_sro_scipy.json` & `pyg2p-3.2.4/templates/glofas_sro_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/glofas_ssro.json` & `pyg2p-3.2.4/templates/glofas_ssro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/glofas_ssro_scipy.json` & `pyg2p-3.2.4/templates/glofas_ssro_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/octahedral_test.json` & `pyg2p-3.2.4/templates/octahedral_test.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/octahedral_test_global.json` & `pyg2p-3.2.4/templates/octahedral_test_global.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/octahedral_test_global_invdist.json` & `pyg2p-3.2.4/templates/octahedral_test_global_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/octahedral_test_invdist.json` & `pyg2p-3.2.4/templates/octahedral_test_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/octahedral_test_scipy.json` & `pyg2p-3.2.4/templates/octahedral_test_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/octahedral_test_scipy_global.json` & `pyg2p-3.2.4/templates/octahedral_test_scipy_global.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/octahedral_test_scipy_global_invdist.json` & `pyg2p-3.2.4/templates/octahedral_test_scipy_global_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/octahedral_test_scipy_invdist.json` & `pyg2p-3.2.4/templates/octahedral_test_scipy_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/rn_false_mv.json` & `pyg2p-3.2.4/templates/rn_false_mv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/tigge_lam_r06.json` & `pyg2p-3.2.4/templates/tigge_lam_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/tigge_lam_r06_rotated.json` & `pyg2p-3.2.4/templates/tigge_lam_r06_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/tigge_lam_r06_scipy.json` & `pyg2p-3.2.4/templates/tigge_lam_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/tigge_lam_r06_scipy_rotated.json` & `pyg2p-3.2.4/templates/tigge_lam_r06_scipy_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/tigge_lam_t24.json` & `pyg2p-3.2.4/templates/tigge_lam_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/tigge_lam_t24_rotated.json` & `pyg2p-3.2.4/templates/tigge_lam_t24_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/tigge_lam_t24_scipy.json` & `pyg2p-3.2.4/templates/tigge_lam_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.3/templates/tigge_lam_t24_scipy_rotated.json` & `pyg2p-3.2.4/templates/tigge_lam_t24_scipy_rotated.json`

 * *Files identical despite different names*

