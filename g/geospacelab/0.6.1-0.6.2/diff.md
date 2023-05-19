# Comparing `tmp/geospacelab-0.6.1.tar.gz` & `tmp/geospacelab-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geospacelab-0.6.1.tar", last modified: Wed Mar  1 11:43:23 2023, max compression
+gzip compressed data, was "geospacelab-0.6.2.tar", last modified: Fri May 19 07:23:19 2023, max compression
```

## Comparing `geospacelab-0.6.1.tar` & `geospacelab-0.6.2.tar`

### file list

```diff
@@ -1,362 +1,360 @@
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1515 2021-08-21 16:59:48.000000 geospacelab-0.6.1/LICENSE
--rw-rw-r--   0 lei       (1000) lei       (1000)      279 2023-03-01 11:24:55.000000 geospacelab-0.6.1/MANIFEST.in
--rw-rw-r--   0 lei       (1000) lei       (1000)    22727 2023-03-01 11:43:23.502258 geospacelab-0.6.1/PKG-INFO
--rw-rw-r--   0 lei       (1000) lei       (1000)    21702 2023-02-21 14:28:53.000000 geospacelab-0.6.1/README.md
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/
--rw-rw-r--   0 lei       (1000) lei       (1000)      502 2023-03-01 11:43:19.000000 geospacelab-0.6.1/geospacelab/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/config/
--rw-rw-r--   0 lei       (1000) lei       (1000)      638 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/config/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4726 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/config/_preferences.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/cs/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1282 2023-03-01 11:02:12.000000 geospacelab-0.6.1/geospacelab/cs/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      723 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/cs/_aacgm.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      756 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/cs/_apex.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    17124 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/cs/_cs_base.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    18253 2022-11-07 08:45:01.000000 geospacelab-0.6.1/geospacelab/cs/_geo.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      604 2021-08-21 16:59:48.000000 geospacelab-0.6.1/geospacelab/cs/geo_utilities.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/
--rw-rw-r--   0 lei       (1000) lei       (1000)    19560 2023-02-06 07:59:04.000000 geospacelab-0.6.1/geospacelab/datahub/__dataset_base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    18655 2022-11-29 09:26:23.000000 geospacelab-0.6.1/geospacelab/datahub/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2825 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/__metadata_base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    38868 2022-10-22 14:04:59.000000 geospacelab-0.6.1/geospacelab/datahub/__variable_base__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/
--rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-12-07 06:22:00.000000 geospacelab-0.6.1/geospacelab/datahub/sources/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/
--rw-rw-r--   0 lei       (1000) lei       (1000)      680 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/omni/
--rw-rw-r--   0 lei       (1000) lei       (1000)    11040 2023-02-15 11:56:02.000000 geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/omni/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4137 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/omni/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3007 2022-11-21 13:13:26.000000 geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/omni/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6666 2022-11-21 13:13:26.000000 geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/omni/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/
--rw-rw-r--   0 lei       (1000) lei       (1000)      557 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/
--rw-rw-r--   0 lei       (1000) lei       (1000)      583 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12352 2022-12-14 12:48:43.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1994 2022-12-14 12:22:24.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1499 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4888 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12468 2022-12-14 12:48:43.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1840 2022-12-14 12:45:25.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1856 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5445 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6544 2022-12-14 12:13:27.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/l1b/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/l1b/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/l2d/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/l2d/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/l2l/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/l2l/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2605 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/fmi/
--rw-rw-r--   0 lei       (1000) lei       (1000)      737 2022-11-24 09:06:45.000000 geospacelab-0.6.1/geospacelab/datahub/sources/fmi/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/fmi/image/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-11-24 08:47:10.000000 geospacelab-0.6.1/geospacelab/datahub/sources/fmi/image/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/fmi/image/ie/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5966 2022-11-24 12:19:09.000000 geospacelab-0.6.1/geospacelab/datahub/sources/fmi/image/ie/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2582 2022-11-24 12:20:08.000000 geospacelab-0.6.1/geospacelab/datahub/sources/fmi/image/ie/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2023-02-03 18:57:40.000000 geospacelab-0.6.1/geospacelab/datahub/sources/fmi/image/ie/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/
--rw-rw-r--   0 lei       (1000) lei       (1000)      496 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4095 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6386 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3896 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1590 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/nowcast/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6310 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4665 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2687 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5666 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6630 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/nowcast/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5644 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7365 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/snf107/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5707 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/snf107/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1663 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/snf107/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/gfz/snf107/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/
--rw-rw-r--   0 lei       (1000) lei       (1000)      556 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/ampere/
--rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/ampere/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/ampere/fitted/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8505 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2709 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1546 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5496 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8283 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5322 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4347 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12477 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     9531 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4686 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2034 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/tecmap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5966 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4305 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2895 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1517 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/
--rw-rw-r--   0 lei       (1000) lei       (1000)    15249 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    16084 2022-11-05 11:21:54.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      652 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    16337 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2514 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8324 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/
--rw-rw-r--   0 lei       (1000) lei       (1000)    14228 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7529 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8274 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8269 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/
--rw-rw-r--   0 lei       (1000) lei       (1000)     7925 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3753 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6371 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/
--rw-rw-r--   0 lei       (1000) lei       (1000)     7851 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3397 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8949 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)      524 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4817 2022-11-05 11:03:22.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10317 2022-09-08 10:10:13.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4902 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    10279 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/
--rw-rw-r--   0 lei       (1000) lei       (1000)    11542 2022-09-08 10:10:14.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3360 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6734 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10204 2022-09-08 10:10:14.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3229 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4054 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4717 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/utilities.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/ncei/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/ncei/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/ncei/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/ncei/dmsp/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/noaa/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/noaa/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/noaa/swpc/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/noaa/swpc/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/noaa/swpc/goesxray/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/noaa/swpc/goesxray/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.494258 geospacelab-0.6.1/geospacelab/datahub/sources/noaa/swpc/solarwind/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/noaa/swpc/solarwind/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/
--rw-rw-r--   0 lei       (1000) lei       (1000)      592 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/potmap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8795 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/potmap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5756 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/potmap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    10900 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/potmap/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1551 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/potmap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2019 2023-02-03 11:28:38.000000 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/indices/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6727 2023-02-06 06:54:34.000000 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/indices/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7842 2023-02-06 06:47:42.000000 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/indices/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1531 2023-02-06 08:02:57.000000 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/indices/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3006 2023-02-03 18:57:39.000000 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/indices/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/magnetometer/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/magnetometer/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    27422 2023-02-03 11:24:53.000000 geospacelab-0.6.1/geospacelab/datahub/sources/supermag/supermag_api.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2742 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/
--rw-rw-r--   0 lei       (1000) lei       (1000)      595 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9336 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1591 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2436 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3337 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/wnd_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9389 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1591 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2890 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5546 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5469 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/
--rw-rw-r--   0 lei       (1000) lei       (1000)      569 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9506 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1593 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3715 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6288 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/
--rw-rw-r--   0 lei       (1000) lei       (1000)      578 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12306 2022-11-28 12:45:58.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1621 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4335 2022-10-10 08:45:16.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/wnd_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10348 2023-01-27 09:29:24.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1618 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2867 2023-01-15 11:57:47.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3346 2023-01-27 09:35:38.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/
--rw-rw-r--   0 lei       (1000) lei       (1000)      578 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9615 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1739 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2731 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/
--rw-rw-r--   0 lei       (1000) lei       (1000)      583 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9240 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1622 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_pod/
--rw-rw-r--   0 lei       (1000) lei       (1000)    11754 2022-10-11 09:28:21.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1622 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1648 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/ae/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5351 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/ae/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6552 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/ae/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1585 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/ae/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/ae/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/asysym/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5383 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/asysym/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6635 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/asysym/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1610 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/asysym/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3728 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/asysym/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/dst/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5337 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/dst/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6235 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/dst/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1521 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/dst/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1516 2022-02-23 05:03:33.000000 geospacelab-0.6.1/geospacelab/datahub/sources/wdc/dst/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/express/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.6.1/geospacelab/express/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4152 2022-10-18 12:32:59.000000 geospacelab-0.6.1/geospacelab/express/dmsp_dashboard.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8218 2023-01-16 12:39:08.000000 geospacelab-0.6.1/geospacelab/express/eiscat_dashboard.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7978 2022-11-11 08:30:29.000000 geospacelab-0.6.1/geospacelab/express/millstonehill_dashboard.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3937 2022-11-21 13:16:14.000000 geospacelab-0.6.1/geospacelab/express/omni_dashboard.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.498258 geospacelab-0.6.1/geospacelab/future/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/future/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/future/empiricalmodels/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/future/empiricalmodels/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/future/empiricalmodels/ovationprime2010/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/future/empiricalmodels/ovationprime2010/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    39045 2023-03-01 11:22:40.000000 geospacelab-0.6.1/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/future/satllites/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/future/satllites/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5213 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/future/satllites/orbit_analyzer.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1151 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/future/test_sscws.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/observatory/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/observatory/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)       11 2022-09-08 09:38:55.000000 geospacelab-0.6.1/geospacelab/observatory/constants.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/observatory/earth/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/observatory/earth/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3720 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/observatory/earth/_func.py
--rw-rw-r--   0 lei       (1000) lei       (1000)       10 2022-09-08 09:37:46.000000 geospacelab-0.6.1/geospacelab/observatory/earth/constants.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1082 2022-09-08 09:57:47.000000 geospacelab-0.6.1/geospacelab/observatory/earth/geodesy.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/observatory/orbit/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-09-08 10:08:40.000000 geospacelab-0.6.1/geospacelab/observatory/orbit/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    13350 2022-11-14 20:00:31.000000 geospacelab-0.6.1/geospacelab/observatory/orbit/sc_orbit.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    23767 2023-01-27 13:25:36.000000 geospacelab-0.6.1/geospacelab/observatory/orbit/utilities.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/quantity/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-09-03 10:12:23.000000 geospacelab-0.6.1/geospacelab/quantity/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/test/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-14 05:31:49.000000 geospacelab-0.6.1/geospacelab/test/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      108 2021-07-14 05:31:49.000000 geospacelab-0.6.1/geospacelab/test/test_A.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      556 2021-07-19 06:05:42.000000 geospacelab-0.6.1/geospacelab/test/test_B.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5938 2021-08-16 12:33:21.000000 geospacelab-0.6.1/geospacelab/test/test_eiscat.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    15193 2021-08-16 10:15:09.000000 geospacelab-0.6.1/geospacelab/test/test_swarm.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/toolbox/
--rw-rw-r--   0 lei       (1000) lei       (1000)       56 2021-07-13 05:22:19.000000 geospacelab-0.6.1/geospacelab/toolbox/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/toolbox/io/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.6.1/geospacelab/toolbox/io/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2021-08-21 16:59:48.000000 geospacelab-0.6.1/geospacelab/toolbox/io/dialog.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/toolbox/unit/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.6.1/geospacelab/toolbox/unit/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/toolbox/utilities/
--rw-rw-r--   0 lei       (1000) lei       (1000)        1 2021-07-13 05:22:19.000000 geospacelab-0.6.1/geospacelab/toolbox/utilities/__init__.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     6067 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/toolbox/utilities/numpyarray.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1838 2022-10-10 13:43:05.000000 geospacelab-0.6.1/geospacelab/toolbox/utilities/numpymath.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     3310 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/toolbox/utilities/pybasic.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     2813 2021-11-29 20:45:17.000000 geospacelab-0.6.1/geospacelab/toolbox/utilities/pyclass.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)    10865 2023-02-06 11:56:22.000000 geospacelab-0.6.1/geospacelab/toolbox/utilities/pydatetime.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     1816 2021-08-21 16:59:48.000000 geospacelab-0.6.1/geospacelab/toolbox/utilities/pylogging.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      754 2021-08-21 16:59:48.000000 geospacelab-0.6.1/geospacelab/toolbox/utilities/pyos.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/visualization/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1025 2023-02-06 14:01:52.000000 geospacelab-0.6.1/geospacelab/visualization/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/visualization/mpl/
--rw-rw-r--   0 lei       (1000) lei       (1000)    31093 2023-02-06 08:03:52.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/__base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      825 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      747 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/_helpers.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-30 07:16:41.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/axes.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)    14482 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/axis_ticks.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7090 2023-02-09 07:50:05.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/colormaps.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    16867 2023-02-06 14:02:31.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/dashboards.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3335 2021-11-29 20:45:17.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/figure.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/visualization/mpl/geomap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2368 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/geomap/__base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-08-30 10:45:18.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/geomap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2847 2022-12-14 09:15:38.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/geomap/geodashboards.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    37388 2023-02-23 11:45:59.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/geomap/geopanels.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    31842 2023-02-15 12:18:56.000000 geospacelab-0.6.1/geospacelab/visualization/mpl/panels.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/visualization/plotly/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-10-20 11:58:01.000000 geospacelab-0.6.1/geospacelab/visualization/plotly/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      224 2021-10-20 11:58:01.000000 geospacelab-0.6.1/geospacelab/visualization/plotly/ipanel.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/wrapper/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.6.1/geospacelab/wrapper/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/wrapper/geopack/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2023-03-01 10:54:57.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/LICENSE
--rw-rw-r--   0 lei       (1000) lei       (1000)    16623 2023-03-01 10:54:57.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/README.md
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:52:29.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.502258 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:54:57.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/__init__.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)    48858 2023-03-01 11:38:52.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/geopack.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    40639 2023-03-01 10:54:57.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)    76431 2023-03-01 10:54:57.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/t01.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    75795 2023-03-01 10:54:57.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/t04.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    14024 2023-03-01 10:54:57.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/t89.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    65292 2023-03-01 10:54:57.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/t96.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    15324 2023-03-01 10:54:57.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/test_geopack1.md
--rw-rw-r--   0 lei       (1000) lei       (1000)     6669 2023-03-01 11:22:40.000000 geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/test_geopack1.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-03-01 11:43:23.490258 geospacelab-0.6.1/geospacelab.egg-info/
--rw-rw-r--   0 lei       (1000) lei       (1000)    22727 2023-03-01 11:43:23.000000 geospacelab-0.6.1/geospacelab.egg-info/PKG-INFO
--rw-rw-r--   0 lei       (1000) lei       (1000)    13488 2023-03-01 11:43:23.000000 geospacelab-0.6.1/geospacelab.egg-info/SOURCES.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)        1 2023-03-01 11:43:23.000000 geospacelab-0.6.1/geospacelab.egg-info/dependency_links.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)      229 2023-03-01 11:43:23.000000 geospacelab-0.6.1/geospacelab.egg-info/requires.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)       17 2023-03-01 11:43:23.000000 geospacelab-0.6.1/geospacelab.egg-info/top_level.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)      148 2023-03-01 11:43:23.502258 geospacelab-0.6.1/setup.cfg
--rw-rw-r--   0 lei       (1000) lei       (1000)     3410 2023-03-01 11:42:51.000000 geospacelab-0.6.1/setup.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.449396 geospacelab-0.6.2/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1515 2021-08-21 16:59:48.000000 geospacelab-0.6.2/LICENSE
+-rw-rw-r--   0 lei       (1000) lei       (1000)      279 2023-03-01 11:24:55.000000 geospacelab-0.6.2/MANIFEST.in
+-rw-rw-r--   0 lei       (1000) lei       (1000)    22727 2023-05-19 07:23:19.449396 geospacelab-0.6.2/PKG-INFO
+-rw-rw-r--   0 lei       (1000) lei       (1000)    21702 2023-02-21 14:28:53.000000 geospacelab-0.6.2/README.md
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      502 2023-05-19 07:20:25.000000 geospacelab-0.6.2/geospacelab/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab/config/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      638 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/config/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4726 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/config/_preferences.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab/cs/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1282 2023-03-01 11:02:12.000000 geospacelab-0.6.2/geospacelab/cs/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      723 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/cs/_aacgm.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      756 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/cs/_apex.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    17124 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/cs/_cs_base.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    18253 2022-11-07 08:45:01.000000 geospacelab-0.6.2/geospacelab/cs/_geo.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      604 2021-08-21 16:59:48.000000 geospacelab-0.6.2/geospacelab/cs/geo_utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab/datahub/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    19560 2023-02-06 07:59:04.000000 geospacelab-0.6.2/geospacelab/datahub/__dataset_base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    18655 2022-11-29 09:26:23.000000 geospacelab-0.6.2/geospacelab/datahub/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2825 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/__metadata_base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    38790 2023-05-17 11:52:59.000000 geospacelab-0.6.2/geospacelab/datahub/__variable_base__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab/datahub/sources/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-12-07 06:22:00.000000 geospacelab-0.6.2/geospacelab/datahub/sources/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      680 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-04-05 13:39:25.000000 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/dmsp/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2516 2023-04-05 13:50:32.000000 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/omni/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10896 2023-04-03 09:52:12.000000 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/omni/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4137 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/omni/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3007 2022-11-21 13:13:26.000000 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/omni/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7304 2023-04-03 09:54:51.000000 geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/omni/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      557 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      583 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12352 2022-12-14 12:48:43.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1994 2022-12-14 12:22:24.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1499 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4888 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12468 2022-12-14 12:48:43.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1840 2022-12-14 12:45:25.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1856 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5445 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6544 2022-12-14 12:13:27.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/l1b/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/l1b/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/l2d/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/l2d/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/l2l/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/l2l/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2605 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/fmi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      737 2022-11-24 09:06:45.000000 geospacelab-0.6.2/geospacelab/datahub/sources/fmi/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-11-24 08:47:10.000000 geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/ie/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5771 2023-05-11 10:38:52.000000 geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/ie/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3068 2023-05-11 10:41:52.000000 geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/ie/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2582 2022-11-24 12:20:08.000000 geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/ie/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2023-02-03 18:57:40.000000 geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/ie/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      496 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4095 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6386 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3896 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1590 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/nowcast/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6310 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4665 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2687 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5666 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6630 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/nowcast/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5644 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7365 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/snf107/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5707 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/snf107/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1663 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/snf107/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/gfz/snf107/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      556 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/ampere/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/ampere/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/ampere/fitted/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8505 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2709 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1546 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5496 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8283 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5322 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4347 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12477 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9531 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4686 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2034 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/tecmap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5966 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4305 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2895 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1517 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    15249 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16084 2022-11-05 11:21:54.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.437395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      652 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16337 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2514 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8330 2023-04-19 11:06:29.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    14228 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7529 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8274 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8269 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7925 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3753 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6371 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7851 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3397 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8949 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      524 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4817 2022-11-05 11:03:22.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10317 2022-09-08 10:10:13.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4902 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10280 2023-04-20 12:28:27.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/
+-rw-r--r--   0 lei       (1000) lei       (1000)    11542 2023-04-20 09:13:20.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3360 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6745 2023-04-19 11:05:17.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10204 2022-09-08 10:10:14.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3229 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4054 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4717 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/ncei/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/ncei/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/ncei/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/ncei/dmsp/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/noaa/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/noaa/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/noaa/swpc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/noaa/swpc/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/noaa/swpc/goesxray/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/noaa/swpc/goesxray/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/noaa/swpc/solarwind/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/noaa/swpc/solarwind/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      592 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/potmap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8795 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/potmap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5756 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/potmap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10900 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/potmap/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1551 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/potmap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2019 2023-02-03 11:28:38.000000 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/indices/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6727 2023-02-06 06:54:34.000000 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/indices/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7842 2023-02-06 06:47:42.000000 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/indices/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1531 2023-02-06 08:02:57.000000 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/indices/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3006 2023-02-03 18:57:39.000000 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/indices/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/magnetometer/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/magnetometer/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    27422 2023-02-03 11:24:53.000000 geospacelab-0.6.2/geospacelab/datahub/sources/supermag/supermag_api.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2742 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      595 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9336 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1591 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2436 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3337 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/wnd_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9389 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1591 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2890 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5546 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5469 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      569 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9506 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1593 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3715 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6288 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      578 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12306 2022-11-28 12:45:58.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1621 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4335 2022-10-10 08:45:16.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/wnd_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10348 2023-01-27 09:29:24.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1618 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2867 2023-01-15 11:57:47.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3346 2023-01-27 09:35:38.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      578 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9615 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1739 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2731 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.441395 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      583 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9240 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1622 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_pod/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    11754 2022-10-11 09:28:21.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1622 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1648 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/ae/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5351 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/ae/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6552 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/ae/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1585 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/ae/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/ae/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/asysym/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5383 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/asysym/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6635 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/asysym/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1610 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/asysym/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3728 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/asysym/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/dst/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5337 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/dst/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6235 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/dst/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1521 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/dst/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1516 2022-02-23 05:03:33.000000 geospacelab-0.6.2/geospacelab/datahub/sources/wdc/dst/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/express/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.6.2/geospacelab/express/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4152 2022-10-18 12:32:59.000000 geospacelab-0.6.2/geospacelab/express/dmsp_dashboard.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8218 2023-01-16 12:39:08.000000 geospacelab-0.6.2/geospacelab/express/eiscat_dashboard.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7978 2022-11-11 08:30:29.000000 geospacelab-0.6.2/geospacelab/express/millstonehill_dashboard.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3937 2022-11-21 13:16:14.000000 geospacelab-0.6.2/geospacelab/express/omni_dashboard.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/future/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/future/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/future/empiricalmodels/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/future/empiricalmodels/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/future/empiricalmodels/ovationprime2010/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/future/empiricalmodels/ovationprime2010/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    39045 2023-03-01 11:22:40.000000 geospacelab-0.6.2/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/future/satllites/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/future/satllites/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5213 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/future/satllites/orbit_analyzer.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1151 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/future/test_sscws.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/observatory/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/observatory/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)       11 2022-09-08 09:38:55.000000 geospacelab-0.6.2/geospacelab/observatory/constants.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/observatory/earth/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/observatory/earth/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3720 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/observatory/earth/_func.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)       10 2022-09-08 09:37:46.000000 geospacelab-0.6.2/geospacelab/observatory/earth/constants.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1082 2022-09-08 09:57:47.000000 geospacelab-0.6.2/geospacelab/observatory/earth/geodesy.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/observatory/orbit/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-09-08 10:08:40.000000 geospacelab-0.6.2/geospacelab/observatory/orbit/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    13350 2022-11-14 20:00:31.000000 geospacelab-0.6.2/geospacelab/observatory/orbit/sc_orbit.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    23767 2023-01-27 13:25:36.000000 geospacelab-0.6.2/geospacelab/observatory/orbit/utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/quantity/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-09-03 10:12:23.000000 geospacelab-0.6.2/geospacelab/quantity/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/toolbox/
+-rw-rw-r--   0 lei       (1000) lei       (1000)       56 2021-07-13 05:22:19.000000 geospacelab-0.6.2/geospacelab/toolbox/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/toolbox/io/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.6.2/geospacelab/toolbox/io/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2021-08-21 16:59:48.000000 geospacelab-0.6.2/geospacelab/toolbox/io/dialog.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/toolbox/unit/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.6.2/geospacelab/toolbox/unit/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/toolbox/utilities/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        1 2021-07-13 05:22:19.000000 geospacelab-0.6.2/geospacelab/toolbox/utilities/__init__.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     6067 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/toolbox/utilities/numpyarray.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1838 2022-10-10 13:43:05.000000 geospacelab-0.6.2/geospacelab/toolbox/utilities/numpymath.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     3310 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/toolbox/utilities/pybasic.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     2813 2021-11-29 20:45:17.000000 geospacelab-0.6.2/geospacelab/toolbox/utilities/pyclass.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)    10865 2023-02-06 11:56:22.000000 geospacelab-0.6.2/geospacelab/toolbox/utilities/pydatetime.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     1816 2021-08-21 16:59:48.000000 geospacelab-0.6.2/geospacelab/toolbox/utilities/pylogging.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      754 2021-08-21 16:59:48.000000 geospacelab-0.6.2/geospacelab/toolbox/utilities/pyos.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/visualization/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1025 2023-02-06 14:01:52.000000 geospacelab-0.6.2/geospacelab/visualization/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/visualization/mpl/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    31503 2023-04-20 12:11:24.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/__base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      825 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      747 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/_helpers.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-30 07:16:41.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/axes.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)    14484 2023-05-17 11:50:34.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/axis_ticks.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7090 2023-02-09 07:50:05.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/colormaps.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16912 2023-05-09 07:55:30.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/dashboards.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3335 2021-11-29 20:45:17.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/figure.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/visualization/mpl/geomap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2368 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/geomap/__base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-08-30 10:45:18.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/geomap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2847 2022-12-14 09:15:38.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/geomap/geodashboards.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    37492 2023-03-28 10:45:19.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/geomap/geopanels.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    32396 2023-05-19 07:17:25.000000 geospacelab-0.6.2/geospacelab/visualization/mpl/panels.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/visualization/plotly/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-10-20 11:58:01.000000 geospacelab-0.6.2/geospacelab/visualization/plotly/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      224 2021-10-20 11:58:01.000000 geospacelab-0.6.2/geospacelab/visualization/plotly/ipanel.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/wrapper/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.6.2/geospacelab/wrapper/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.445396 geospacelab-0.6.2/geospacelab/wrapper/geopack/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2023-03-01 10:54:57.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/LICENSE
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16623 2023-03-01 10:54:57.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/README.md
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:52:29.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.449396 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:54:57.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/__init__.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)    48858 2023-03-01 11:38:52.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/geopack.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    40639 2023-03-01 10:54:57.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)    76431 2023-03-01 10:54:57.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/t01.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    75795 2023-03-01 10:54:57.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/t04.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    14024 2023-03-01 10:54:57.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/t89.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    65292 2023-03-01 10:54:57.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/t96.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    15324 2023-03-01 10:54:57.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/test_geopack1.md
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6669 2023-03-01 11:22:40.000000 geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/test_geopack1.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-05-19 07:23:19.433395 geospacelab-0.6.2/geospacelab.egg-info/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    22727 2023-05-19 07:23:19.000000 geospacelab-0.6.2/geospacelab.egg-info/PKG-INFO
+-rw-rw-r--   0 lei       (1000) lei       (1000)    13498 2023-05-19 07:23:19.000000 geospacelab-0.6.2/geospacelab.egg-info/SOURCES.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)        1 2023-05-19 07:23:19.000000 geospacelab-0.6.2/geospacelab.egg-info/dependency_links.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)      229 2023-05-19 07:23:19.000000 geospacelab-0.6.2/geospacelab.egg-info/requires.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)       23 2023-05-19 07:23:19.000000 geospacelab-0.6.2/geospacelab.egg-info/top_level.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)      148 2023-05-19 07:23:19.449396 geospacelab-0.6.2/setup.cfg
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3410 2023-03-01 11:42:51.000000 geospacelab-0.6.2/setup.py
```

### Comparing `geospacelab-0.6.1/LICENSE` & `geospacelab-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/PKG-INFO` & `geospacelab-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospacelab
-Version: 0.6.1
+Version: 0.6.2
 Summary: Collect, manage, and visualize geospace data.
 Home-page: https://github.com/JouleCai/geospacelab
 Author: Lei Cai
 Author-email: lei.cai@oulu.fi
 License: BSD 3-Clause License
 Keywords: Geospace,EISCAT,DMSP,Space weather,Ionosphere,Space,Magnetosphere
 Classifier: Development Status :: 4 - Beta
```

### Comparing `geospacelab-0.6.1/README.md` & `geospacelab-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/config/__init__.py` & `geospacelab-0.6.2/geospacelab/config/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/config/_preferences.py` & `geospacelab-0.6.2/geospacelab/config/_preferences.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/cs/__init__.py` & `geospacelab-0.6.2/geospacelab/cs/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/cs/_aacgm.py` & `geospacelab-0.6.2/geospacelab/cs/_aacgm.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/cs/_apex.py` & `geospacelab-0.6.2/geospacelab/cs/_apex.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/cs/_cs_base.py` & `geospacelab-0.6.2/geospacelab/cs/_cs_base.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/cs/_geo.py` & `geospacelab-0.6.2/geospacelab/cs/_geo.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/cs/geo_utilities.py` & `geospacelab-0.6.2/geospacelab/cs/geo_utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/__dataset_base__.py` & `geospacelab-0.6.2/geospacelab/datahub/__dataset_base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/__metadata_base__.py` & `geospacelab-0.6.2/geospacelab/datahub/__metadata_base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/__variable_base__.py` & `geospacelab-0.6.2/geospacelab/datahub/__variable_base__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 
     def __init__(self):
         self.data = None
         self.data_err = None
         self.data_scale = 1.
         self.data_res = None
         self.mask_gap = None
-        self.label = ''
+        self.label = None
         self.label_style = 'double'  # or 'single
         self.label_pos = None  # label position
         self.unit = ''
         self.lim = None
         self.scale = 'linear'
         self.invert = False
         self.ticks = None
         self.tick_labels = None
         self.minor_ticks = None
-        self.major_tick_max = 6
+        self.major_tick_min = 6
+        self.major_tick_max = 12
         self.minor_tick_max = None
         self.reverse = False
         self.visible = True
 
     def config(self, logging=True, **kwargs):
         pyclass.set_object_attributes(self, append=False, logging=logging, **kwargs)
 
@@ -589,25 +590,21 @@
         if len(v.shape) == 1 and v.shape != (1,):
             v = v.reshape((v.shape[0], 1))
         self._error = v
 
     @property
     def unit_label(self):
         label = self._unit_label
-        if not str(label):
-            label = self.unit
-        return label
+        if label is None:
+            return self.unit
+        else:
+            return label
 
     @unit_label.setter
-    def unit_label(self, label):
-        if label is None:
-            self._unit_label = ''
-            return
-        if type(label) is not str:
-            raise TypeError
+    def unit_label(self, label: str or None):
         self._unit_label = label
 
     @property
     def label(self):
         lb = self._label
         if not str(lb):
             lb = self.name
```

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/omni/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/omni/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,18 +217,18 @@
         ca = np.sign(By) * (np.pi/2 - np.arcsin(Bz / Bt))
         ca = np.mod(ca, 2 * np.pi)
 
         if not to_radian:
             ca = ca / np.pi * 180
 
         var_name = 'CA_' + cs
-        var = self['B_x_GSM'].clone()
-        var.name = var_name
+        var = self.add_variable(var_name)
         var.value = ca.reshape(ca.size, 1)
         var.label = r'$\theta$'
+        var.unit = 'rad'
         self[var_name] = var
         return self[var_name]
 
     @_validate_IMF_cs
     def add_IMF_AZ(self, cs='GSM', to_radian=False,  **kwargs):
         """
         IMF azimuthal angle in the IMF Bx-By (x-y) plane in the GSE/GSM coordinate system.
@@ -240,18 +240,18 @@
         az = np.sign(Bx) * (np.pi/2 - np.arcsin(By / Bt))
         az = np.mod(az, 2 * np.pi)
 
         if not to_radian:
             az = az / np.pi * 180
 
         var_name = 'AZ_' + cs
-        var = self['B_x_GSM'].clone()
-        var.name = var_name
+        var = self.add_variable(var_name)
         var.value = az.reshape(az.size, 1)
         var.label = r'$\phi$'
+        var.unit = 'rad'
         self[var_name] = var
         return self[var_name]
 
     @_validate_IMF_cs
     def add_IMF_EL(self, cs='GSM', to_radian=False,  **kwargs):
         """
         IMF elevation angle in the IMF Bz-Bx (x-y) plane in the GSE/GSM coordinate system.
@@ -263,18 +263,18 @@
         el = np.sign(Bz) * (np.pi / 2 - np.arcsin(Bx / Bt))
         el = np.mod(el, 2 * np.pi)
 
         if not to_radian:
             el = el / np.pi * 180
 
         var_name = 'EL_' + cs
-        var = self['B_x_GSM'].clone()
-        var.name = var_name
+        var = self.add_variable(var_name)
         var.value = el.reshape(el.size, 1)
         var.label = r'$\alpha$'
+        var.unit = 'rad'
         self[var_name] = var
         return self[var_name]
 
     def add_NCF(self):
         """
         Solar wind-magnetosphere coupling function by Newell et al., JGR, 2007.
         :return:
@@ -284,22 +284,17 @@
 
         ca = self['CA_GSM'].value
         ca = ca * np.pi / 180
         v = self['v_sw'].value
         BT = self['B_T_GSM'].value
         ncf = np.abs(v)**(4/3) * np.abs(BT)**(2/3) * np.abs(np.sin(ca*0.5))**(8/3)
 
-        var = self['CA_GSM'].clone()
-        var.value = ncf
-        var.name = 'NCF'
-        var.label = r'd$\Phi_{MP}/$d$t$'
-        var.unit = ''
-        var.unit_label = ''
-        var.visual.axis[1].lim = [None, None]
-        self['NCF'] = var
+        self['NCF'] = var_config.configured_variables['NCF'].clone()
+        self['NCF'].value = ncf
+
         return self['NCF']
 
     @property
     def database(self):
         return self._database
 
     @database.setter
```

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/omni/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/omni/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/omni/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/omni/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/cdaweb/omni/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/cdaweb/omni/variable_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,8 +220,30 @@
 # set axis attrs
 axis = var.visual.axis
 axis[1].data = "@v.value"
 axis[1].lim = [None, None]
 axis[1].label = '@v.group'
 axis[1].unit = '@v.unit_label'
 
+
+####################################################################################################################
+var_name = 'NCF'
+var = Var(name=var_name, ndim=1, variable_type='scalar', visual=visual)
+# set variable attrs
+var.fullname = 'Newell Coupling Function'
+var.label = r'd$\Phi_{MP}/$d$t$'
+var.group = r'SW-M CF'
+var.unit = ''
+var.depends = {0: depend_0}
+# set plot attrs
+plot_config = var.visual.plot_config
+plot_config.config(**default_plot_config)
+plot_config.style = '1noE'
+# set axis attrs
+axis = var.visual.axis
+axis[1].data = "@v.value"
+axis[1].lim = [None, None]
+axis[1].label = '@v.label'
+axis[1].unit = '@v.unit'
+
+
 configured_variables[var_name] = var
```

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/esa_eo/swarm/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/esa_eo/swarm/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/fmi/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/fmi/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/fmi/image/ie/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/ie/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 # from geospacelab.datahub.sources.gfz.kpap.downloader import Downloader as default_Downloader
 import geospacelab.datahub.sources.fmi.image.ie.variable_config as var_config
 
 
 default_dataset_attrs = {
     'database': fmi_database,
     'product': 'IL',
-    'data_file_ext': 'txt',
-    'data_root_dir': prf.datahub_data_root_dir / 'FMI' / 'Indices',
+    'data_file_ext': 'dat',
+    'data_root_dir': prf.datahub_data_root_dir / 'FMI' / 'IMAGE' / 'IE',
     'allow_load': True,
     'allow_download': True,
     'force_download': False,
     'data_search_recursive': False,
     'label_fields': ['database', 'product', 'data_file_ext'],
     'time_clip': True,
 }
@@ -50,21 +50,21 @@
     def __init__(self, **kwargs):
         kwargs = basic.dict_set_default(kwargs, **default_dataset_attrs)
 
         super().__init__(**kwargs)
 
         self.database = kwargs.pop('database', fmi_database)
         self.product = kwargs.pop('product', 'IE')
-        self.load_mode = kwargs.pop('load_mode', 'assigned')
+        self.load_mode = kwargs.pop('load_mode', 'AUTO')
         self.allow_download = kwargs.pop('allow_download', False)
         self.force_download = kwargs.pop('force_download', False)
 
         self.metadata = None
 
-        allow_load = kwargs.pop('allow_load', False)
+        allow_load = kwargs.pop('allow_load', True)
 
         # self.config(**kwargs)
 
         if self.loader is None:
             self.loader = default_Loader
 
         if self.downloader is None:
@@ -102,58 +102,55 @@
             self.metadata = load_obj.metadata
 
             # self.select_beams(field_aligned=True)
         if self.time_clip:
             self.time_filter_by_range()
 
     def search_data_files(self, **kwargs):
-        raise NotImplementedError
-    #     dt_fr = self.dt_fr
-    #     dt_to = self.dt_to
-    #     diff_years = dt_to.year - dt_fr.year
-    #     dt0 = datetime.datetime(dt_fr.year, 1, 1)
-    #     for i in range(diff_years + 1):
-    #         thisyear = datetime.datetime(dt0.year + i, 1, 1)
-    #         if datetime.date.today().year == thisyear.year:
-    #             self.force_download = True
-    #
-    #         initial_file_dir = kwargs.pop('initial_file_dir', None)
-    #         if initial_file_dir is None:
-    #             initial_file_dir = self.data_root_dir / 'Kp_Ap'
-    #         file_patterns = [thisyear.strftime("%Y")]
-    #         # remove empty str
-    #         file_patterns = [pattern for pattern in file_patterns if str(pattern)]
-    #
-    #         search_pattern = '*' + '*'.join(file_patterns) + '*'
-    #
-    #         if not self.force_download:
-    #             done = super().search_data_files(
-    #                 initial_file_dir=initial_file_dir, search_pattern=search_pattern
-    #             )
-    #         else:
-    #             done = False
-    #
-    #         # Validate file paths
-    #
-    #         if not done and self.allow_download:
-    #             done = self.download_data()
-    #             if done:
-    #                 done = super().search_data_files(
-    #                     initial_file_dir=initial_file_dir, search_pattern=search_pattern)
-    #             else:
-    #                 print('Cannot find files from the online database!')
-    #
-    #     return done
-    #
-    # def download_data(self):
-    #     if self.data_file_ext == 'nc':
-    #         download_obj = self.downloader(self.dt_fr, self.dt_to, data_file_root_dir=self.data_root_dir, force=self.force_download)
-    #     else:
-    #         raise NotImplementedError
-    #     return download_obj.done
+        dt_fr = self.dt_fr
+        dt_to = self.dt_to
+        diff_days = dttool.get_diff_days(dt_fr, dt_to)
+        dt0 = dttool.get_start_of_the_day(dt_fr)
+        for i in range(diff_days + 1):
+            thisday = dt0 + datetime.timedelta(days=i)
+    
+            initial_file_dir = kwargs.pop('initial_file_dir', None)
+            if initial_file_dir is None:
+                initial_file_dir = self.data_root_dir / thisday.strftime('%Y')
+            file_patterns = [thisday.strftime("%Y%m%d")]
+            # remove empty str
+            file_patterns = [pattern for pattern in file_patterns if str(pattern)]
+    
+            search_pattern = '*' + '*'.join(file_patterns) + '*'
+    
+            if not self.force_download:
+                done = super().search_data_files(
+                    initial_file_dir=initial_file_dir, search_pattern=search_pattern
+                )
+            else:
+                done = False
+    
+            # Validate file paths
+    
+            if not done and self.allow_download:
+                done = self.download_data()
+                if done:
+                    done = super().search_data_files(
+                        initial_file_dir=initial_file_dir, search_pattern=search_pattern)
+                else:
+                    print('Cannot find files from the online database!')
+    
+        return done
+    
+    def download_data(self):
+        if self.data_file_ext == 'dat':
+            download_obj = self.downloader(self.dt_fr, self.dt_to, data_file_root_dir=self.data_root_dir, force=self.force_download)
+        else:
+            raise NotImplementedError
+        return download_obj.done
 
     @property
     def database(self):
         return self._database
 
     @database.setter
     def database(self, value):
```

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/fmi/image/ie/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/ie/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/fmi/image/ie/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/fmi/image/ie/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/hpo/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/hpo/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/kpap/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/kpap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/snf107/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/snf107/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/snf107/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/snf107/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/gfz/snf107/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/gfz/snf107/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         'lim':      [90, 350],
         'label':    'h',
         'unit':     'km',
     },
     2:  {
         'data':     '@v.value',
         'label':    '@v.label',
-        'unit':     '@v.unit',
+        'unit':     '@v.unit_label',
     }
 }
 
 default_plot_config = {
     'line':         {
         'linestyle':        '',
         'linewidth':        1.5,
@@ -148,15 +148,15 @@
 configured_variables[var_name] = var
 
 ####################################################################################################################
 var_name = 'v_i_los'
 var = Var(name=var_name, ndim=2, variable_type='scalar', visual=visual)
 # set variable attrs
 var.fullname = 'Line-of-sight ion velocity'
-var.label = r'$v_i^{los}$'
+var.label = r'$v_i^{LOS}$'
 var.unit = 'm/s'
 var.error = var_name + '_err'
 var.depends = {0: depend_0, 1: depend_1}
 # set plot attrs
 var.visual.plot_config.config(**default_plot_config)
 var.visual.plot_config.style = '2P'
 # set axis attrs
```

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         'linestyle':        '',
         'linewidth':        1.5,
         'marker':           '.',
         'markersize':       3,
     },
     'pcolormesh':   {
         'cmap':            default_colormap,
-    }
+    },
 }
 
 configured_variables = {}
 visual = 'on'
 
 ####################################################################################################################
 var_name = 'JE_e'
```

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 default_colormap = cm.cmap_jet_modified()
 
 default_axis_dict_1d = {
     1: {
         'data': '@v.value',
         'label': '@v.group',
-        'unit': '@v.unit',
+        'unit': '@v.unit_label',
         'label_pos': [-0.1, 0.5],
     },
     2: {
         'label': '@v.label'
     },
 }
 
@@ -53,15 +53,15 @@
         'lim':      [90, 350],
         'label':    'h',
         'unit':     'km',
     },
     2:  {
         'data':     '@v.value',
         'label':    '@v.label',
-        'unit':     '@v.unit',
+        'unit':     '@v.unit_label',
     }
 }
 
 default_plot_config = {
     'line':         {
         'linestyle':        '-',
         'linewidth':        1.5,
@@ -214,15 +214,15 @@
 var = Var(ndim=1, variable_type='scalar', visual=visual)
 # set variable attrs
 var_config = {
     'name': var_name,
     'fullname': 'Electron density',
     'label': r'$n_e$',
     'group': 'Density',
-    'unit': 'm/-3',
+    'unit': 'm-3',
     'unit_label': r'm$^{-3}$',
     'error': None,
     'depends': {0: depend_0},
 }
 var.config(**var_config)
 # set plot attrs
 var.visual.plot_config.config(**default_plot_config)
```

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/madrigal/utilities.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/madrigal/utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/potmap/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/potmap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/potmap/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/potmap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/potmap/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/potmap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/superdarn/potmap/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/superdarn/potmap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/supermag/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/supermag/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/supermag/indices/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/supermag/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/supermag/indices/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/supermag/indices/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/supermag/indices/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/supermag/indices/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/supermag/indices/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/supermag/indices/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/supermag/supermag_api.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/supermag/supermag_api.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/ae/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/ae/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/ae/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/ae/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/ae/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/ae/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/ae/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/asysym/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/asysym/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/asysym/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/asysym/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/asysym/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/asysym/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/asysym/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/asysym/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/dst/__init__.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/dst/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/dst/downloader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/dst/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/dst/loader.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/dst/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/datahub/sources/wdc/dst/variable_config.py` & `geospacelab-0.6.2/geospacelab/datahub/sources/wdc/dst/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/express/dmsp_dashboard.py` & `geospacelab-0.6.2/geospacelab/express/dmsp_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/express/eiscat_dashboard.py` & `geospacelab-0.6.2/geospacelab/express/eiscat_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/express/millstonehill_dashboard.py` & `geospacelab-0.6.2/geospacelab/express/millstonehill_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/express/omni_dashboard.py` & `geospacelab-0.6.2/geospacelab/express/omni_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py` & `geospacelab-0.6.2/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/future/satllites/orbit_analyzer.py` & `geospacelab-0.6.2/geospacelab/future/satllites/orbit_analyzer.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/future/test_sscws.py` & `geospacelab-0.6.2/geospacelab/future/test_sscws.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/observatory/earth/_func.py` & `geospacelab-0.6.2/geospacelab/observatory/earth/_func.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/observatory/earth/geodesy.py` & `geospacelab-0.6.2/geospacelab/observatory/earth/geodesy.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/observatory/orbit/sc_orbit.py` & `geospacelab-0.6.2/geospacelab/observatory/orbit/sc_orbit.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/observatory/orbit/utilities.py` & `geospacelab-0.6.2/geospacelab/observatory/orbit/utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/toolbox/io/dialog.py` & `geospacelab-0.6.2/geospacelab/toolbox/io/dialog.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/toolbox/utilities/numpyarray.py` & `geospacelab-0.6.2/geospacelab/toolbox/utilities/numpyarray.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/toolbox/utilities/numpymath.py` & `geospacelab-0.6.2/geospacelab/toolbox/utilities/numpymath.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/toolbox/utilities/pybasic.py` & `geospacelab-0.6.2/geospacelab/toolbox/utilities/pybasic.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/toolbox/utilities/pyclass.py` & `geospacelab-0.6.2/geospacelab/toolbox/utilities/pyclass.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/toolbox/utilities/pydatetime.py` & `geospacelab-0.6.2/geospacelab/toolbox/utilities/pydatetime.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/toolbox/utilities/pylogging.py` & `geospacelab-0.6.2/geospacelab/toolbox/utilities/pylogging.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/toolbox/utilities/pyos.py` & `geospacelab-0.6.2/geospacelab/toolbox/utilities/pyos.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/visualization/__init__.py` & `geospacelab-0.6.2/geospacelab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/__base__.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/__base__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     mpl_style = pref.user_config['visualization']['mpl']['style']
 except KeyError:
     uc = pref.user_config
     uc['visualization']['mpl']['style'] = 'light'
     pref.set_user_config(user_config=uc, set_as_default=True)
 
 
-plt.rcParams['font.serif'] = 'Ubuntu'
-plt.rcParams['font.monospace'] = 'Ubuntu Mono'
+# plt.rcParams['font.serif'] = 'Ubuntu'
+# plt.rcParams['font.monospace'] = 'Ubuntu Mono'
 plt.rcParams['font.size'] = 10
 plt.rcParams['axes.labelsize'] = 10
 plt.rcParams['axes.labelweight'] = 'book'
 plt.rcParams['axes.titlesize'] = 10
 plt.rcParams['xtick.labelsize'] = 10
 plt.rcParams['ytick.labelsize'] = 10
 plt.rcParams['legend.fontsize'] = 10
@@ -253,14 +253,23 @@
         self.num_rows = None
         self.num_cols = None
         self.title = kwargs.pop('title', None)
         self.label = kwargs.pop('label', None)
         self.extra_axes = {}
         self.gs = None
 
+    def clear(self):
+        keys = list(self.panels.keys())
+        for ind_p in keys:
+            self.remove_panel(ind_p)
+        for ax in self.extra_axes.values():
+            ax.remove()
+        self.extra_axes = {}
+
+
     def set_layout(self, num_rows=None, num_cols=None, **kwargs):
         """
         Set the layout of the dashboard in a canvas using matplotlib GridSpec.
 
         :param num_rows: The number of rows of the grid.
         :type num_rows: int.
         :param num_cols: The number of columns of the grid.
@@ -320,15 +329,15 @@
         """
         Remove a panel
 
         :param index: The panel index.
         :type index: int or str.
         """
 
-        self.panels[index].remove()
+        self.panels[index].clear()
         del self.panels[index]
     #
     # def replace_panel(self, index, **kwargs):
     #     position = self.panels[index].get_position()
     #     self.remove_panel(index)
     #
     #     panel = self.figure.add_subplot(**kwargs)
@@ -352,15 +361,15 @@
         if x is None:
             x = 0.5
         if y is None:
             y = 1.05
 
         self.add_text(x, y, title, **kwargs)
 
-    def add_panel_labels(self, panel_indices=None, style='alphabets', bbox_config=None, **kwargs):
+    def add_panel_labels(self, panel_indices=None, style='alphabets', bbox_config=None, labels=list(), **kwargs):
         if panel_indices is None:
             panel_indices = self.panels.keys()
 
         if style == 'alphabets':
             label_list = string.ascii_lowercase
         else:
             raise NotImplemented
@@ -376,18 +385,22 @@
         kwargs.setdefault('ha', 'left')  # horizontal alignment
         kwargs.setdefault('va', 'center')  # vertical alignment
 
         pos_0 = self.panels[0].axes['major'].get_position()  # adjust y in case of different gs_row_heights
         for ind, p_index in enumerate(panel_indices):
             panel = self.panels[p_index]
             pos_1 = panel.axes['major'].get_position()
-            if panel.label is None:
-                label = "({})".format(label_list[ind])
+            if list(labels) :
+                label = labels[ind]
+            elif panel.label is None:
+                label = "{}".format(label_list[ind])
             else:
                 label = panel.label
+                
+            label = "({})".format(label)
             kwargs.setdefault('fontsize', plt.rcParams['axes.labelsize'])
             kwargs.setdefault('fontweight', 'book')
             if bbox_config is None:
                 bbox_config = {'facecolor': 'yellow', 'alpha': 0.3, 'edgecolor': 'none'}
             kwargs.setdefault('bbox', bbox_config)
             y_new = 1 - pos_0.height / pos_1.height + y * pos_0.height / pos_1.height
             panel.add_label(x, y_new, label, **kwargs)
@@ -558,14 +571,20 @@
         if type(ax) in [str]:
             return self.axes[ax]
         elif ax in self.axes:
             return ax
         else:
             raise AttributeError
 
+    def clear(self):
+        for ax in self.axes.values():
+            ax.remove()
+
+        self.axes = {}
+
     def sca(self, ax):
         """
         Set current axes.
 
         :param ax: the ax instance belong to the attribute axes.
         """
         plt.sca(ax)
@@ -772,15 +791,14 @@
             pos_cax = [
                 pos_ax.x0 + (pos_ax.x1 - pos_ax.x0) * cax_position[0],
                 pos_ax.y0 + (pos_ax.y1 - pos_ax.y0) * cax_position[1],
                 (pos_ax.x1 - pos_ax.x0) * cax_position[2],
                 (pos_ax.y1 - pos_ax.y0) * cax_position[3],
             ]
             cax = self.add_axes(pos_cax)
-            cax_label_config = {'rotation': 270, 'va': 'bottom', 'size': 'medium'}
 
         icb = self.figure.colorbar(im, cax=cax, **kwargs)
 
         self.sca(ax)
 
         # set colorbar label
         cax_label_config = pybasic.dict_set_default(cax_label_config, rotation=270, va='bottom', size='small')
@@ -801,14 +819,15 @@
                 [l.set_visible(False) for (i, l) in enumerate(cax.yaxis.get_ticklabels()) if i % n != 0]
                 # [l.set_ha('right') for (i, l) in enumerate(cax.yaxis.get_ticklabels()) if i % n != 0]
                 minorlocator = mpl.ticker.LogLocator(base=10.0, subs=(0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9),
                                                      numticks=12)
                 cax.yaxis.set_minor_locator(minorlocator)
                 cax.yaxis.set_minor_formatter(mpl.ticker.NullFormatter())
         cax.yaxis.set_tick_params(labelsize='x-small')
+        return icb
 
     @property
     def major_ax(self):
         return self.axes['major']
 
     @major_ax.setter
     def major_ax(self, ax):
```

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/__init__.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/_helpers.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/_helpers.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/axis_ticks.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/axis_ticks.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         #    minticks = 2 * len(ax.xaxis.get_major_ticks())
         #    maxticks = 8 * len(ax.xaxis.get_major_ticks())
         super().__init__(tz=tz, minticks=minticks, maxticks=maxticks, interval_multiples=interval_multiples)
 
 
 class DatetimeMajorFormatter(mdates.AutoDateFormatter):
     def __init__(self, locator, scaled: dict or None = None, tz=None, defaultfmt='%Y-%m-%d', *, usetex=True):
-        super().__init__(locator, tz=None, defaultfmt='%Y-%m-%d', usetex=True)
+        super().__init__(locator, tz=None, defaultfmt=defaultfmt, usetex=usetex)
         self.scaled[1 / HOURS_PER_DAY] = formatter_hour_per_day
         self.scaled[1 / MINUTES_PER_DAY] = formatter_minute_per_day
         if scaled is not None:
            self.scaled.update(**scaled)
 
 
 def formatter_hour_per_day(x, pos):
```

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/colormaps.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/colormaps.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/dashboards.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/dashboards.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,19 +355,21 @@
                         value = [(v + 180.) % 360 - 180 for v in value]
                     else:
                         value = (value + 180.) % 360 - 180
                 else:
                     itpf = interp1d(x0, y0, bounds_error=False, fill_value='extrapolate')
                     y1 = itpf(x1)
             else:
-                y1 = y0[ind_1]
+                y1 = y0
             if type(value) in (int, float):
                 ind_1 = argrelmin(np.abs(y1 - value))
             elif type(value) is list:
                 ind_1 = np.where((y1 > value[0]) & (y1 < value[1]))[0]
+            else:
+                raise NotImplementedError
 
             x1 = x1[ind_1]
             y1 = y1[ind_1]
 
         results = []
         for xx in x1:
             ind_1 = argrelmin(np.abs(x0 - xx))
@@ -425,14 +427,13 @@
                 text_config.setdefault('va', 'center')
             text_config.setdefault('ha', 'center')
             text_config.setdefault('fontsize', plt.rcParams['axes.labelsize'])
             text_config.setdefault('fontweight', 'medium')
             text_config.setdefault('clip_on', False)
             ax.text(x, y, label, transform=ax.transAxes, **text_config)
 
-    def add_top_bar(self, dt_fr, dt_to, bottom=0, top=0.02, **kwargs):
+    def add_top_bar(self, dt_fr, dt_to, bottom=0, top=0.02, facecolor='orange', **kwargs):
         bottom_extend = -1. - bottom
         top_extend = top
         kwargs.setdefault('alpha', 1.)
-        kwargs.setdefault('facecolor', 'orange')
-        self.add_shading(dt_fr, dt_to, bottom_extend=bottom_extend, top_extend=top_extend, **kwargs)
+        self.add_shading(dt_fr, dt_to, bottom_extend=bottom_extend, top_extend=top_extend, facecolor=facecolor, **kwargs)
```

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/figure.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/figure.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/geomap/__base__.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/geomap/__base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/geomap/geodashboards.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/geomap/geodashboards.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/geomap/geopanels.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/geomap/geopanels.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,15 +598,16 @@
         grid_data[ind_out] = np.nan
 
         return grid_x, grid_y, grid_data
 
     def overlay_sc_trajectory(self, sc_ut=None, sc_coords=None, cs=None, *, show_trajectory=True, color='#EEEEEE',
                           time_tick=True, time_tick_res=300., time_tick_scale=0.05,
                           time_tick_label=True, time_tick_label_format="%H:%M", time_tick_label_fontsize=8,
-                          time_tick_label_rotation=45., time_tick_label_offset=0.05,
+                          time_tick_label_rotation=45., time_tick_label_offset=0.05, 
+                          time_tick_label_fontweight='normal',
                           time_minor_tick=True, time_minor_tick_res=60,
                           time_tick_width=1, **kwargs):
         kwargs.setdefault('trajectory_config', {
             'linewidth': 1,
             'linestyle': '-',
             'color': 'k',
             'zorder': max([_.zorder for _ in self.major_ax.get_children()])
@@ -671,17 +672,17 @@
                 for ind, time_tick in enumerate(time_ticks):
                     time = dt0 + datetime.timedelta(seconds=time_tick)
                     x_time_tick = x_i[ind] - offset * np.sin(slope_i[ind])
                     y_time_tick = y_i[ind] + offset * np.cos(slope_i[ind])
 
                     self.major_ax.text(
                         x_time_tick, y_time_tick, time.strftime(time_tick_label_format),
-                        fontsize=time_tick_label_fontsize,
+                        fontsize=time_tick_label_fontsize, fontweight=time_tick_label_fontweight,
                         rotation=slope[ind] * 180. / np.pi + time_tick_label_rotation,
-                        ha='center', va='center', color=color,
+                        ha='center', va='center', color=color, 
                         zorder=zorder
                     )
 
             # self.major_ax.plot(x_time_ticks, y_time_ticks, **kwargs['time_tick_config'])
 
             if time_minor_tick:
```

### Comparing `geospacelab-0.6.1/geospacelab/visualization/mpl/panels.py` & `geospacelab-0.6.2/geospacelab/visualization/mpl/panels.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import re
 import datetime
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.colors as mpl_colors
 import matplotlib.ticker as mpl_ticker
 import matplotlib.dates as mpl_dates
+from matplotlib import rcParams
 from scipy.interpolate import interp1d
 
 from geospacelab.visualization.mpl.__base__ import PanelBase
 from geospacelab.datahub.__variable_base__ import VariableBase as VariableModel
 import geospacelab.toolbox.utilities.numpyarray as arraytool
 import geospacelab.visualization.mpl.axis_ticks as ticktool
 import geospacelab.toolbox.utilities.pybasic as basic
@@ -196,16 +197,20 @@
             errorbar_config.update(var.visual.plot_config.errorbar)
             il = ax.errorbar(x.flatten(), y.flatten(), yerr=y_err.flatten(), **errorbar_config)
         if type(il) is not list:
             il = [il]
         self.axes_overview[ax]['lines'].extend(il)
         if self.axes_overview[ax]['legend'] is None:
             self.axes_overview[ax]['legend'] = 'on'
-        elif self.axes_overview[ax]['legend'] == 'off':
+        if var.visual.axis[1].label is None:
             var.visual.axis[1].label = '@v.label'
+        if var.visual.axis[1].unit is None:
+            var.visual.axis[1].unit = '@v.unit_label'
+        # elif self.axes_overview[ax]['legend'] == 'off':
+        #    var.visual.axis[1].label = '@v.label'
         return il
 
     @check_panel_ax
     def overlay_bar(self, *args, ax=None, **kwargs):
 
         var = args[0]
         il = None
@@ -307,15 +312,18 @@
         )
         ax.xaxis.set_tick_params(which='major', length=8)
         ax.xaxis.set_tick_params(which='minor', length=4)
 
         # use date locators
         # majorlocator, minorlocator, majorformatter = ticktool.set_timeline(self._xlim[0], self._xlim[1])
         from geospacelab.visualization.mpl.axis_ticks import DatetimeMajorFormatter, DatetimeMajorLocator, DatetimeMinorLocator
-        majorlocator = DatetimeMajorLocator()
+
+        maxticks = var_for_config.visual.axis[0].major_tick_max
+        minticks = var_for_config.visual.axis[0].major_tick_min
+        majorlocator = DatetimeMajorLocator(maxticks=maxticks, minticks=minticks)
         majorformatter = DatetimeMajorFormatter(majorlocator)
 
         if not self.bottom_panel:
             majorformatter = mpl_ticker.NullFormatter()
             plt.setp(ax.get_xticklabels(), visible=False)
         ax.xaxis.set_major_locator(majorlocator)
         ax.xaxis.set_major_formatter(majorformatter)
@@ -411,15 +419,15 @@
                 elif 'MLT' in xlabels[ind]:
                     text = (datetime.datetime(1970, 1, 1) + datetime.timedelta(hours=xtick)).strftime('%H:%M')
                 else:
                     text = '%.1f' % xtick
                 ax.text(
                     xy_fig[ind_pos][0], xy_fig[ind_pos][1] + yoffset * ind - 0.013,
                     text,
-                    fontsize=plt.rcParams['xtick.labelsize'],
+                    fontsize=plt.rcParams['xtick.labelsize']-2,
                     horizontalalignment='center', verticalalignment='top',
                     transform=self.figure.transFigure
                 )
         ax.xaxis.set_major_formatter(mpl_ticker.NullFormatter())
 
         # if self.major_timeline == 'MLT':
         #     for ind_pos, xtick in enumerate(ys[mlt_ind]):
@@ -542,17 +550,21 @@
         axes = [ax]
         axes.extend(ax_ov['twinx_axes'])
         for ind, pax in enumerate(axes):
 
             pax_ov = self.axes_overview[pax]
             if list(pax_ov['lines']):
                 il = pax_ov['lines'][0]
-                pax.yaxis.label.set_color(il.get_color())
-                pax.tick_params(axis='y', which='both', colors=il.get_color())
-                pax.spines['right'].set_edgecolor(il.get_color())
+                if isinstance(il, mpl.container.ErrorbarContainer):
+                    il_ = il[0]
+                else:
+                    il_ = il
+                pax.yaxis.label.set_color(il_.get_color())
+                pax.tick_params(axis='y', which='both', colors=il_.get_color())
+                pax.spines['right'].set_edgecolor(il_.get_color())
             else:
                 continue
 
     def _check_colorbar(self, ax):
         ax_ov = self.axes_overview[ax]
         var_for_config = ax_ov['variables'][0]
         colorbar_config = var_for_config.visual.plot_config.colorbar
@@ -571,15 +583,15 @@
         ntwinx = len(ax_ov['twinx_axes'])
         cax_position = [1.02 + offset * ntwinx, 0.01, 0.025, 0.85]
         colorbar_config.update(
             cax_scale=c_scale, cax_label=c_label, cax_ticks=c_ticks, cax_tick_labels=c_tick_labels,
             cax_position=cax_position
         )
 
-        self.add_colorbar(im, cax='new', **colorbar_config)
+        cb = self.add_colorbar(im, cax='new', **colorbar_config)
 
     def _retrieve_data_1d(self, var):
         x_data = var.get_visual_axis_attr(axis=0, attr_name='data')
         if type(x_data) == list:
             x_data = x_data[0]
         if x_data is None:
             depend_0 = var.get_depend(axis=0)
```

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/LICENSE` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/LICENSE`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/README.md` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/README.md`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/geopack.py` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/geopack.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/t01.py` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/t01.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/t04.py` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/t04.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/t89.py` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/t89.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/t96.py` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/t96.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/test_geopack1.md` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/test_geopack1.md`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab/wrapper/geopack/geopack/test_geopack1.py` & `geospacelab-0.6.2/geospacelab/wrapper/geopack/geopack/test_geopack1.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.1/geospacelab.egg-info/PKG-INFO` & `geospacelab-0.6.2/geospacelab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospacelab
-Version: 0.6.1
+Version: 0.6.2
 Summary: Collect, manage, and visualize geospace data.
 Home-page: https://github.com/JouleCai/geospacelab
 Author: Lei Cai
 Author-email: lei.cai@oulu.fi
 License: BSD 3-Clause License
 Keywords: Geospace,EISCAT,DMSP,Space weather,Ionosphere,Space,Magnetosphere
 Classifier: Development Status :: 4 - Beta
```

### Comparing `geospacelab-0.6.1/geospacelab.egg-info/SOURCES.txt` & `geospacelab-0.6.2/geospacelab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 geospacelab/cs/geo_utilities.py
 geospacelab/datahub/__dataset_base__.py
 geospacelab/datahub/__init__.py
 geospacelab/datahub/__metadata_base__.py
 geospacelab/datahub/__variable_base__.py
 geospacelab/datahub/sources/__init__.py
 geospacelab/datahub/sources/cdaweb/__init__.py
+geospacelab/datahub/sources/cdaweb/downloader.py
+geospacelab/datahub/sources/cdaweb/dmsp/__init__.py
 geospacelab/datahub/sources/cdaweb/omni/__init__.py
 geospacelab/datahub/sources/cdaweb/omni/downloader.py
 geospacelab/datahub/sources/cdaweb/omni/loader.py
 geospacelab/datahub/sources/cdaweb/omni/variable_config.py
 geospacelab/datahub/sources/esa_eo/__init__.py
 geospacelab/datahub/sources/esa_eo/swarm/__init__.py
 geospacelab/datahub/sources/esa_eo/swarm/downloader.py
@@ -44,14 +46,15 @@
 geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/__init__.py
 geospacelab/datahub/sources/esa_eo/swarm/l1b/__init__.py
 geospacelab/datahub/sources/esa_eo/swarm/l2d/__init__.py
 geospacelab/datahub/sources/esa_eo/swarm/l2l/__init__.py
 geospacelab/datahub/sources/fmi/__init__.py
 geospacelab/datahub/sources/fmi/image/__init__.py
 geospacelab/datahub/sources/fmi/image/ie/__init__.py
+geospacelab/datahub/sources/fmi/image/ie/downloader.py
 geospacelab/datahub/sources/fmi/image/ie/loader.py
 geospacelab/datahub/sources/fmi/image/ie/variable_config.py
 geospacelab/datahub/sources/gfz/__init__.py
 geospacelab/datahub/sources/gfz/downloader.py
 geospacelab/datahub/sources/gfz/hpo/__init__.py
 geospacelab/datahub/sources/gfz/hpo/downloader.py
 geospacelab/datahub/sources/gfz/hpo/loader.py
@@ -209,19 +212,14 @@
 geospacelab/observatory/earth/_func.py
 geospacelab/observatory/earth/constants.py
 geospacelab/observatory/earth/geodesy.py
 geospacelab/observatory/orbit/__init__.py
 geospacelab/observatory/orbit/sc_orbit.py
 geospacelab/observatory/orbit/utilities.py
 geospacelab/quantity/__init__.py
-geospacelab/test/__init__.py
-geospacelab/test/test_A.py
-geospacelab/test/test_B.py
-geospacelab/test/test_eiscat.py
-geospacelab/test/test_swarm.py
 geospacelab/toolbox/__init__.py
 geospacelab/toolbox/io/__init__.py
 geospacelab/toolbox/io/dialog.py
 geospacelab/toolbox/unit/__init__.py
 geospacelab/toolbox/utilities/__init__.py
 geospacelab/toolbox/utilities/numpyarray.py
 geospacelab/toolbox/utilities/numpymath.py
```

### Comparing `geospacelab-0.6.1/setup.py` & `geospacelab-0.6.2/setup.py`

 * *Files identical despite different names*

