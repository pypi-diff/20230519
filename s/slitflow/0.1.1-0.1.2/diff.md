# Comparing `tmp/slitflow-0.1.1.tar.gz` & `tmp/slitflow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slitflow-0.1.1.tar", last modified: Mon Mar  6 09:12:21 2023, max compression
+gzip compressed data, was "slitflow-0.1.2.tar", last modified: Fri May 19 07:29:17 2023, max compression
```

## Comparing `slitflow-0.1.1.tar` & `slitflow-0.1.2.tar`

### file list

```diff
@@ -1,118 +1,122 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:21.070359 slitflow-0.1.1/
--rw-rw-rw-   0        0        0     1543 2023-02-02 03:40:43.000000 slitflow-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     3419 2023-03-06 09:12:21.071359 slitflow-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2931 2023-03-06 08:58:47.000000 slitflow-0.1.1/README.md
--rw-rw-rw-   0        0        0      151 2022-07-27 10:08:19.000000 slitflow-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      780 2023-03-06 09:12:21.078354 slitflow-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-07-27 10:08:19.000000 slitflow-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.630611 slitflow-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.676584 slitflow-0.1.1/src/slitflow/
--rw-rw-rw-   0        0        0      460 2023-02-15 09:16:07.000000 slitflow-0.1.1/src/slitflow/__init__.py
--rw-rw-rw-   0        0        0     8061 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/data.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.742547 slitflow-0.1.1/src/slitflow/fig/
--rw-rw-rw-   0        0        0      225 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/fig/__init__.py
--rw-rw-rw-   0        0        0     8592 2023-03-02 07:52:33.000000 slitflow-0.1.1/src/slitflow/fig/bar.py
--rw-rw-rw-   0        0        0     5017 2023-02-28 04:20:13.000000 slitflow-0.1.1/src/slitflow/fig/figure.py
--rw-rw-rw-   0        0        0     2417 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/fig/image.py
--rw-rw-rw-   0        0        0     7882 2023-03-02 07:52:39.000000 slitflow-0.1.1/src/slitflow/fig/line.py
--rw-rw-rw-   0        0        0     2599 2023-02-28 04:20:41.000000 slitflow-0.1.1/src/slitflow/fig/scatter.py
--rw-rw-rw-   0        0        0    41578 2023-03-06 04:01:37.000000 slitflow-0.1.1/src/slitflow/fig/style.py
--rw-rw-rw-   0        0        0     4212 2023-02-28 04:21:06.000000 slitflow-0.1.1/src/slitflow/fig/trajectory.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.767532 slitflow-0.1.1/src/slitflow/fun/
--rw-rw-rw-   0        0        0      124 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/fun/__init__.py
--rw-rw-rw-   0        0        0     1228 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/fun/img.py
--rw-rw-rw-   0        0        0      541 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/fun/misc.py
--rw-rw-rw-   0        0        0     5531 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/fun/palette.py
--rw-rw-rw-   0        0        0      242 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/fun/sort.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.805510 slitflow-0.1.1/src/slitflow/img/
--rw-rw-rw-   0        0        0      263 2023-02-15 09:21:06.000000 slitflow-0.1.1/src/slitflow/img/__init__.py
--rw-rw-rw-   0        0        0     1693 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/img/calc.py
--rw-rw-rw-   0        0        0     5437 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/img/convert.py
--rw-rw-rw-   0        0        0     4289 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/img/create.py
--rw-rw-rw-   0        0        0    10820 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/img/filter.py
--rw-rw-rw-   0        0        0     7636 2023-03-06 04:01:55.000000 slitflow-0.1.1/src/slitflow/img/image.py
--rw-rw-rw-   0        0        0     5471 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/img/montage.py
--rw-rw-rw-   0        0        0     1956 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/img/noise.py
--rw-rw-rw-   0        0        0     5648 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/img/plot.py
--rw-rw-rw-   0        0        0    24652 2023-03-06 04:02:14.000000 slitflow-0.1.1/src/slitflow/info.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.815504 slitflow-0.1.1/src/slitflow/load/
--rw-rw-rw-   0        0        0       70 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/load/__init__.py
--rw-rw-rw-   0        0        0     1365 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/load/table.py
--rw-rw-rw-   0        0        0     9413 2023-02-17 12:47:03.000000 slitflow-0.1.1/src/slitflow/load/tif.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.834494 slitflow-0.1.1/src/slitflow/loc/
--rw-rw-rw-   0        0        0      128 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/loc/__init__.py
--rw-rw-rw-   0        0        0     6508 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/loc/convert.py
--rw-rw-rw-   0        0        0     9074 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/loc/fit.py
--rw-rw-rw-   0        0        0     6043 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/loc/mask.py
--rw-rw-rw-   0        0        0     3792 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/loc/random.py
--rw-rw-rw-   0        0        0    31206 2023-03-06 06:20:02.000000 slitflow-0.1.1/src/slitflow/manager.py
--rw-rw-rw-   0        0        0     6363 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/name.py
--rw-rw-rw-   0        0        0     2774 2023-02-28 08:50:49.000000 slitflow-0.1.1/src/slitflow/setindex.py
--rw-rw-rw-   0        0        0     6126 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/setreqs.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.862478 slitflow-0.1.1/src/slitflow/tbl/
--rw-rw-rw-   0        0        0      190 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/tbl/__init__.py
--rw-rw-rw-   0        0        0     6276 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/tbl/convert.py
--rw-rw-rw-   0        0        0     4279 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/tbl/create.py
--rw-rw-rw-   0        0        0     2608 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/tbl/filter.py
--rw-rw-rw-   0        0        0    10153 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/tbl/math.py
--rw-rw-rw-   0        0        0    14129 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/tbl/stat.py
--rw-rw-rw-   0        0        0     3413 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/tbl/table.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.893461 slitflow-0.1.1/src/slitflow/trj/
--rw-rw-rw-   0        0        0      204 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/trj/__init__.py
--rw-rw-rw-   0        0        0     3356 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/trj/filter.py
--rw-rw-rw-   0        0        0    24916 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/trj/msd.py
--rw-rw-rw-   0        0        0    15950 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/trj/random.py
--rw-rw-rw-   0        0        0    32263 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/trj/wfastspt.py
--rw-rw-rw-   0        0        0    12180 2023-02-17 12:47:04.000000 slitflow-0.1.1/src/slitflow/trj/wtrackpy.py
--rw-rw-rw-   0        0        0     9667 2023-02-28 08:32:50.000000 slitflow-0.1.1/src/slitflow/trj/wtramway.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.903454 slitflow-0.1.1/src/slitflow/user/
--rw-rw-rw-   0        0        0      307 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/user/__init__.py
--rw-rw-rw-   0        0        0     1728 2023-02-01 11:16:51.000000 slitflow-0.1.1/src/slitflow/user/template.py
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:20.710569 slitflow-0.1.1/src/slitflow.egg-info/
--rw-rw-rw-   0        0        0     3419 2023-03-06 09:12:20.000000 slitflow-0.1.1/src/slitflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2775 2023-03-06 09:12:20.000000 slitflow-0.1.1/src/slitflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 09:12:20.000000 slitflow-0.1.1/src/slitflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-03-06 09:12:20.000000 slitflow-0.1.1/src/slitflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-06 09:12:20.000000 slitflow-0.1.1/src/slitflow.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 09:12:21.067361 slitflow-0.1.1/src/tests/
--rw-rw-rw-   0        0        0        0 2023-03-02 07:56:26.000000 slitflow-0.1.1/src/tests/__init__.py
--rw-rw-rw-   0        0        0     2815 2023-03-02 07:56:28.000000 slitflow-0.1.1/src/tests/test_data.py
--rw-rw-rw-   0        0        0     4148 2023-03-02 07:56:30.000000 slitflow-0.1.1/src/tests/test_fig_bar.py
--rw-rw-rw-   0        0        0     1177 2023-03-02 07:56:32.000000 slitflow-0.1.1/src/tests/test_fig_figure.py
--rw-rw-rw-   0        0        0      639 2023-03-02 07:56:35.000000 slitflow-0.1.1/src/tests/test_fig_image.py
--rw-rw-rw-   0        0        0     2485 2023-03-02 07:56:37.000000 slitflow-0.1.1/src/tests/test_fig_line.py
--rw-rw-rw-   0        0        0     1204 2023-03-02 07:56:39.000000 slitflow-0.1.1/src/tests/test_fig_scatter.py
--rw-rw-rw-   0        0        0    18945 2023-03-06 04:03:32.000000 slitflow-0.1.1/src/tests/test_fig_style.py
--rw-rw-rw-   0        0        0     1517 2023-03-02 07:56:44.000000 slitflow-0.1.1/src/tests/test_fig_trajectory.py
--rw-rw-rw-   0        0        0     3499 2023-03-02 07:56:46.000000 slitflow-0.1.1/src/tests/test_fun.py
--rw-rw-rw-   0        0        0     1634 2023-03-06 04:03:36.000000 slitflow-0.1.1/src/tests/test_getting_started.py
--rw-rw-rw-   0        0        0      549 2023-03-02 07:56:48.000000 slitflow-0.1.1/src/tests/test_img_calc.py
--rw-rw-rw-   0        0        0      760 2023-03-02 07:56:51.000000 slitflow-0.1.1/src/tests/test_img_create.py
--rw-rw-rw-   0        0        0     1098 2023-03-02 07:56:53.000000 slitflow-0.1.1/src/tests/test_img_filter.py
--rw-rw-rw-   0        0        0     3252 2023-03-06 04:03:44.000000 slitflow-0.1.1/src/tests/test_img_image.py
--rw-rw-rw-   0        0        0      952 2023-03-02 07:56:58.000000 slitflow-0.1.1/src/tests/test_img_montage.py
--rw-rw-rw-   0        0        0      607 2023-03-06 04:03:46.000000 slitflow-0.1.1/src/tests/test_img_noise.py
--rw-rw-rw-   0        0        0      732 2023-03-06 04:03:51.000000 slitflow-0.1.1/src/tests/test_img_plot.py
--rw-rw-rw-   0        0        0     6763 2023-03-06 04:03:57.000000 slitflow-0.1.1/src/tests/test_info.py
--rw-rw-rw-   0        0        0      533 2023-03-02 07:57:07.000000 slitflow-0.1.1/src/tests/test_load_table.py
--rw-rw-rw-   0        0        0      976 2023-03-02 07:57:10.000000 slitflow-0.1.1/src/tests/test_load_tif.py
--rw-rw-rw-   0        0        0     2191 2023-03-02 07:57:11.000000 slitflow-0.1.1/src/tests/test_loc_convert.py
--rw-rw-rw-   0        0        0     1252 2023-03-02 07:57:13.000000 slitflow-0.1.1/src/tests/test_loc_fit.py
--rw-rw-rw-   0        0        0     1598 2023-03-02 07:57:16.000000 slitflow-0.1.1/src/tests/test_loc_mask.py
--rw-rw-rw-   0        0        0      592 2023-03-02 07:57:17.000000 slitflow-0.1.1/src/tests/test_loc_random.py
--rw-rw-rw-   0        0        0    14806 2023-03-06 04:04:03.000000 slitflow-0.1.1/src/tests/test_manager.py
--rw-rw-rw-   0        0        0     3058 2023-03-06 04:04:08.000000 slitflow-0.1.1/src/tests/test_name.py
--rw-rw-rw-   0        0        0     1659 2023-03-06 04:04:16.000000 slitflow-0.1.1/src/tests/test_setindex.py
--rw-rw-rw-   0        0        0     2533 2023-03-02 07:57:27.000000 slitflow-0.1.1/src/tests/test_setreqs.py
--rw-rw-rw-   0        0        0      668 2023-03-02 07:57:30.000000 slitflow-0.1.1/src/tests/test_tbl_convert.py
--rw-rw-rw-   0        0        0     1237 2023-03-02 07:57:32.000000 slitflow-0.1.1/src/tests/test_tbl_create.py
--rw-rw-rw-   0        0        0      541 2023-03-02 07:57:34.000000 slitflow-0.1.1/src/tests/test_tbl_filter.py
--rw-rw-rw-   0        0        0     1860 2023-03-02 07:57:36.000000 slitflow-0.1.1/src/tests/test_tbl_math.py
--rw-rw-rw-   0        0        0     1134 2023-03-02 07:57:38.000000 slitflow-0.1.1/src/tests/test_tbl_stat.py
--rw-rw-rw-   0        0        0      957 2023-03-02 07:57:40.000000 slitflow-0.1.1/src/tests/test_tbl_table.py
--rw-rw-rw-   0        0        0     1317 2023-03-02 07:57:41.000000 slitflow-0.1.1/src/tests/test_trj_filter.py
--rw-rw-rw-   0        0        0     4269 2023-03-02 07:57:43.000000 slitflow-0.1.1/src/tests/test_trj_msd.py
--rw-rw-rw-   0        0        0     1276 2023-03-06 04:04:20.000000 slitflow-0.1.1/src/tests/test_trj_random.py
--rw-rw-rw-   0        0        0     7154 2023-03-02 07:57:47.000000 slitflow-0.1.1/src/tests/test_trj_wfastspt.py
--rw-rw-rw-   0        0        0     1194 2023-03-02 07:57:48.000000 slitflow-0.1.1/src/tests/test_trj_wtrackpy.py
--rw-rw-rw-   0        0        0     1635 2023-03-02 07:53:40.000000 slitflow-0.1.1/src/tests/test_trj_wtramway.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.790159 slitflow-0.1.2/
+-rw-rw-rw-   0        0        0     1543 2023-02-02 03:40:43.000000 slitflow-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0     3462 2023-05-19 07:29:17.791159 slitflow-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-03-06 08:58:47.000000 slitflow-0.1.2/README.md
+-rw-rw-rw-   0        0        0      151 2022-07-27 10:08:19.000000 slitflow-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      974 2023-05-19 07:29:17.799158 slitflow-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-07-27 10:08:19.000000 slitflow-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.291603 slitflow-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.342930 slitflow-0.1.2/src/slitflow/
+-rw-rw-rw-   0        0        0      486 2023-05-19 04:54:58.000000 slitflow-0.1.2/src/slitflow/__init__.py
+-rw-rw-rw-   0        0        0     8061 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/data.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.417900 slitflow-0.1.2/src/slitflow/fig/
+-rw-rw-rw-   0        0        0      225 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/fig/__init__.py
+-rw-rw-rw-   0        0        0     8592 2023-03-02 07:52:33.000000 slitflow-0.1.2/src/slitflow/fig/bar.py
+-rw-rw-rw-   0        0        0     5063 2023-05-19 06:18:31.000000 slitflow-0.1.2/src/slitflow/fig/figure.py
+-rw-rw-rw-   0        0        0     2417 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/fig/image.py
+-rw-rw-rw-   0        0        0     7882 2023-03-02 07:52:39.000000 slitflow-0.1.2/src/slitflow/fig/line.py
+-rw-rw-rw-   0        0        0     2599 2023-02-28 04:20:41.000000 slitflow-0.1.2/src/slitflow/fig/scatter.py
+-rw-rw-rw-   0        0        0    41578 2023-03-06 04:01:37.000000 slitflow-0.1.2/src/slitflow/fig/style.py
+-rw-rw-rw-   0        0        0     4212 2023-02-28 04:21:06.000000 slitflow-0.1.2/src/slitflow/fig/trajectory.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.439896 slitflow-0.1.2/src/slitflow/fun/
+-rw-rw-rw-   0        0        0      124 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/fun/__init__.py
+-rw-rw-rw-   0        0        0     1228 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/fun/img.py
+-rw-rw-rw-   0        0        0      541 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/fun/misc.py
+-rw-rw-rw-   0        0        0     5531 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/fun/palette.py
+-rw-rw-rw-   0        0        0      242 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/fun/sort.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.483179 slitflow-0.1.2/src/slitflow/img/
+-rw-rw-rw-   0        0        0      290 2023-05-18 01:18:17.000000 slitflow-0.1.2/src/slitflow/img/__init__.py
+-rw-rw-rw-   0        0        0     1693 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/calc.py
+-rw-rw-rw-   0        0        0     5437 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/convert.py
+-rw-rw-rw-   0        0        0     8470 2023-05-18 02:33:03.000000 slitflow-0.1.2/src/slitflow/img/create.py
+-rw-rw-rw-   0        0        0    10820 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/filter.py
+-rw-rw-rw-   0        0        0     7959 2023-05-18 02:33:03.000000 slitflow-0.1.2/src/slitflow/img/image.py
+-rw-rw-rw-   0        0        0     5471 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/montage.py
+-rw-rw-rw-   0        0        0     1956 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/noise.py
+-rw-rw-rw-   0        0        0     5648 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/img/plot.py
+-rw-rw-rw-   0        0        0     3703 2023-05-18 01:17:03.000000 slitflow-0.1.2/src/slitflow/img/proc.py
+-rw-rw-rw-   0        0        0    25481 2023-05-18 02:33:03.000000 slitflow-0.1.2/src/slitflow/info.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.496199 slitflow-0.1.2/src/slitflow/load/
+-rw-rw-rw-   0        0        0       70 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/load/__init__.py
+-rw-rw-rw-   0        0        0     1365 2023-02-17 12:47:03.000000 slitflow-0.1.2/src/slitflow/load/table.py
+-rw-rw-rw-   0        0        0     9465 2023-05-19 04:47:43.000000 slitflow-0.1.2/src/slitflow/load/tif.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.517168 slitflow-0.1.2/src/slitflow/loc/
+-rw-rw-rw-   0        0        0      128 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/loc/__init__.py
+-rw-rw-rw-   0        0        0     6508 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/loc/convert.py
+-rw-rw-rw-   0        0        0     9074 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/loc/fit.py
+-rw-rw-rw-   0        0        0     7263 2023-05-18 02:05:33.000000 slitflow-0.1.2/src/slitflow/loc/mask.py
+-rw-rw-rw-   0        0        0     3792 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/loc/random.py
+-rw-rw-rw-   0        0        0    31206 2023-03-06 06:20:02.000000 slitflow-0.1.2/src/slitflow/manager.py
+-rw-rw-rw-   0        0        0     6363 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/name.py
+-rw-rw-rw-   0        0        0     2616 2023-05-18 01:22:50.000000 slitflow-0.1.2/src/slitflow/setindex.py
+-rw-rw-rw-   0        0        0     8668 2023-05-18 02:05:33.000000 slitflow-0.1.2/src/slitflow/setreqs.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.554173 slitflow-0.1.2/src/slitflow/tbl/
+-rw-rw-rw-   0        0        0      217 2023-05-18 01:23:36.000000 slitflow-0.1.2/src/slitflow/tbl/__init__.py
+-rw-rw-rw-   0        0        0     7528 2023-05-18 01:23:59.000000 slitflow-0.1.2/src/slitflow/tbl/convert.py
+-rw-rw-rw-   0        0        0     4279 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/tbl/create.py
+-rw-rw-rw-   0        0        0     2608 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/tbl/filter.py
+-rw-rw-rw-   0        0        0    10153 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/tbl/math.py
+-rw-rw-rw-   0        0        0     6303 2023-05-18 01:17:19.000000 slitflow-0.1.2/src/slitflow/tbl/proc.py
+-rw-rw-rw-   0        0        0    14129 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/tbl/stat.py
+-rw-rw-rw-   0        0        0     3478 2023-05-18 01:39:32.000000 slitflow-0.1.2/src/slitflow/tbl/table.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.584198 slitflow-0.1.2/src/slitflow/trj/
+-rw-rw-rw-   0        0        0      204 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/trj/__init__.py
+-rw-rw-rw-   0        0        0     3356 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/trj/filter.py
+-rw-rw-rw-   0        0        0    24916 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/trj/msd.py
+-rw-rw-rw-   0        0        0    15950 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/trj/random.py
+-rw-rw-rw-   0        0        0    32297 2023-05-18 07:08:13.000000 slitflow-0.1.2/src/slitflow/trj/wfastspt.py
+-rw-rw-rw-   0        0        0    12180 2023-02-17 12:47:04.000000 slitflow-0.1.2/src/slitflow/trj/wtrackpy.py
+-rw-rw-rw-   0        0        0     9667 2023-02-28 08:32:50.000000 slitflow-0.1.2/src/slitflow/trj/wtramway.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.592178 slitflow-0.1.2/src/slitflow/user/
+-rw-rw-rw-   0        0        0      307 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/user/__init__.py
+-rw-rw-rw-   0        0        0     1728 2023-02-01 11:16:51.000000 slitflow-0.1.2/src/slitflow/user/template.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.381929 slitflow-0.1.2/src/slitflow.egg-info/
+-rw-rw-rw-   0        0        0     3462 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2879 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      240 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-19 07:29:17.000000 slitflow-0.1.2/src/slitflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 07:29:17.786160 slitflow-0.1.2/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-02 07:56:26.000000 slitflow-0.1.2/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     2815 2023-03-02 07:56:28.000000 slitflow-0.1.2/src/tests/test_data.py
+-rw-rw-rw-   0        0        0     4148 2023-03-02 07:56:30.000000 slitflow-0.1.2/src/tests/test_fig_bar.py
+-rw-rw-rw-   0        0        0     1177 2023-03-02 07:56:32.000000 slitflow-0.1.2/src/tests/test_fig_figure.py
+-rw-rw-rw-   0        0        0      639 2023-03-02 07:56:35.000000 slitflow-0.1.2/src/tests/test_fig_image.py
+-rw-rw-rw-   0        0        0     2485 2023-03-02 07:56:37.000000 slitflow-0.1.2/src/tests/test_fig_line.py
+-rw-rw-rw-   0        0        0     1204 2023-03-02 07:56:39.000000 slitflow-0.1.2/src/tests/test_fig_scatter.py
+-rw-rw-rw-   0        0        0    18945 2023-03-06 04:03:32.000000 slitflow-0.1.2/src/tests/test_fig_style.py
+-rw-rw-rw-   0        0        0     1517 2023-03-02 07:56:44.000000 slitflow-0.1.2/src/tests/test_fig_trajectory.py
+-rw-rw-rw-   0        0        0     3499 2023-03-02 07:56:46.000000 slitflow-0.1.2/src/tests/test_fun.py
+-rw-rw-rw-   0        0        0     1634 2023-03-06 04:03:36.000000 slitflow-0.1.2/src/tests/test_getting_started.py
+-rw-rw-rw-   0        0        0      549 2023-03-02 07:56:48.000000 slitflow-0.1.2/src/tests/test_img_calc.py
+-rw-rw-rw-   0        0        0     1343 2023-05-18 02:33:03.000000 slitflow-0.1.2/src/tests/test_img_create.py
+-rw-rw-rw-   0        0        0     1098 2023-03-02 07:56:53.000000 slitflow-0.1.2/src/tests/test_img_filter.py
+-rw-rw-rw-   0        0        0     3260 2023-05-18 05:27:15.000000 slitflow-0.1.2/src/tests/test_img_image.py
+-rw-rw-rw-   0        0        0      952 2023-03-02 07:56:58.000000 slitflow-0.1.2/src/tests/test_img_montage.py
+-rw-rw-rw-   0        0        0      607 2023-03-06 04:03:46.000000 slitflow-0.1.2/src/tests/test_img_noise.py
+-rw-rw-rw-   0        0        0      732 2023-03-06 04:03:51.000000 slitflow-0.1.2/src/tests/test_img_plot.py
+-rw-rw-rw-   0        0        0     1191 2023-05-18 01:25:03.000000 slitflow-0.1.2/src/tests/test_img_proc.py
+-rw-rw-rw-   0        0        0     6763 2023-03-06 04:03:57.000000 slitflow-0.1.2/src/tests/test_info.py
+-rw-rw-rw-   0        0        0      533 2023-03-02 07:57:07.000000 slitflow-0.1.2/src/tests/test_load_table.py
+-rw-rw-rw-   0        0        0      976 2023-03-02 07:57:10.000000 slitflow-0.1.2/src/tests/test_load_tif.py
+-rw-rw-rw-   0        0        0     2191 2023-03-02 07:57:11.000000 slitflow-0.1.2/src/tests/test_loc_convert.py
+-rw-rw-rw-   0        0        0     1252 2023-03-02 07:57:13.000000 slitflow-0.1.2/src/tests/test_loc_fit.py
+-rw-rw-rw-   0        0        0     1598 2023-03-02 07:57:16.000000 slitflow-0.1.2/src/tests/test_loc_mask.py
+-rw-rw-rw-   0        0        0      592 2023-03-02 07:57:17.000000 slitflow-0.1.2/src/tests/test_loc_random.py
+-rw-rw-rw-   0        0        0    14806 2023-03-06 04:04:03.000000 slitflow-0.1.2/src/tests/test_manager.py
+-rw-rw-rw-   0        0        0     3058 2023-03-06 04:04:08.000000 slitflow-0.1.2/src/tests/test_name.py
+-rw-rw-rw-   0        0        0     1659 2023-03-06 04:04:16.000000 slitflow-0.1.2/src/tests/test_setindex.py
+-rw-rw-rw-   0        0        0     2533 2023-03-02 07:57:27.000000 slitflow-0.1.2/src/tests/test_setreqs.py
+-rw-rw-rw-   0        0        0     2620 2023-05-18 01:26:28.000000 slitflow-0.1.2/src/tests/test_tbl_convert.py
+-rw-rw-rw-   0        0        0     1237 2023-03-02 07:57:32.000000 slitflow-0.1.2/src/tests/test_tbl_create.py
+-rw-rw-rw-   0        0        0      541 2023-03-02 07:57:34.000000 slitflow-0.1.2/src/tests/test_tbl_filter.py
+-rw-rw-rw-   0        0        0     1860 2023-03-02 07:57:36.000000 slitflow-0.1.2/src/tests/test_tbl_math.py
+-rw-rw-rw-   0        0        0     1195 2023-05-18 01:26:37.000000 slitflow-0.1.2/src/tests/test_tbl_proc.py
+-rw-rw-rw-   0        0        0     1134 2023-03-02 07:57:38.000000 slitflow-0.1.2/src/tests/test_tbl_stat.py
+-rw-rw-rw-   0        0        0      957 2023-03-02 07:57:40.000000 slitflow-0.1.2/src/tests/test_tbl_table.py
+-rw-rw-rw-   0        0        0     1317 2023-03-02 07:57:41.000000 slitflow-0.1.2/src/tests/test_trj_filter.py
+-rw-rw-rw-   0        0        0     4269 2023-03-02 07:57:43.000000 slitflow-0.1.2/src/tests/test_trj_msd.py
+-rw-rw-rw-   0        0        0     1276 2023-03-06 04:04:20.000000 slitflow-0.1.2/src/tests/test_trj_random.py
+-rw-rw-rw-   0        0        0     7154 2023-03-02 07:57:47.000000 slitflow-0.1.2/src/tests/test_trj_wfastspt.py
+-rw-rw-rw-   0        0        0     1194 2023-03-02 07:57:48.000000 slitflow-0.1.2/src/tests/test_trj_wtrackpy.py
+-rw-rw-rw-   0        0        0     1635 2023-03-02 07:53:40.000000 slitflow-0.1.2/src/tests/test_trj_wtramway.py
```

### Comparing `slitflow-0.1.1/LICENCE` & `slitflow-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/PKG-INFO` & `slitflow-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: slitflow
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python framework for single-molecule dynamics and localization analysis
 Author: Yuma Ito
 Author-email: yitou@bio.titech.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: full
+Provides-Extra: dev
 License-File: LICENCE
 
 # Slitflow
 
 **Slitflow** is a Python package that aims to construct a fully reproducible and universally accessible workflow for single-molecule analysis—namely, **S**ingle-molecule **L**ocalization-**I**ntegrated **T**rajectory analysis work**FLOW**.
 
 **Slitflow** comprises a flexible Data class that executes a task and stores the resulting data. A Data object can be input to the next Data object, the network of Data objects forming the entire workflow of complex single-molecule analysis, from image pre-processing to publication-quality figure creation.
```

### Comparing `slitflow-0.1.1/README.md` & `slitflow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/setup.cfg` & `slitflow-0.1.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -30,20 +30,32 @@
 000001d0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
 000001e0: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
 000001f0: 3d20 7372 630d 0a70 6163 6b61 6765 7320  = src..packages 
 00000200: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
 00000210: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
 00000220: 2c20 3c33 2e31 310d 0a69 6e73 7461 6c6c  , <3.11..install
 00000230: 5f72 6571 7569 7265 7320 3d20 0d0a 096e  _requires = ...n
-00000240: 756d 7079 0d0a 0970 616e 6461 730d 0a09  umpy...pandas...
-00000250: 6d61 7470 6c6f 746c 6962 0d0a 0974 6966  matplotlib...tif
-00000260: 6666 696c 650d 0a09 7471 646d 0d0a 0970  ffile...tqdm...p
-00000270: 7375 7469 6c0d 0a09 6f70 656e 6376 2d70  sutil...opencv-p
-00000280: 7974 686f 6e0d 0a09 7363 6970 790d 0a09  ython...scipy...
-00000290: 7363 696b 6974 2d6c 6561 726e 0d0a 0973  scikit-learn...s
-000002a0: 6369 6b69 742d 696d 6167 650d 0a09 6e65  cikit-image...ne
-000002b0: 7467 7261 7068 0d0a 0d0a 5b6f 7074 696f  tgraph....[optio
-000002c0: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-000002d0: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
-000002e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000300: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000240: 756d 7079 0d0a 0970 616e 6461 733c 322e  umpy...pandas<2.
+00000250: 302e 300d 0a09 6d61 7470 6c6f 746c 6962  0.0...matplotlib
+00000260: 0d0a 0974 6966 6666 696c 650d 0a09 7471  ...tifffile...tq
+00000270: 646d 0d0a 0970 7375 7469 6c0d 0a09 6f70  dm...psutil...op
+00000280: 656e 6376 2d70 7974 686f 6e0d 0a09 7363  encv-python...sc
+00000290: 6970 790d 0a09 7363 696b 6974 2d6c 6561  ipy...scikit-lea
+000002a0: 726e 0d0a 0973 6369 6b69 742d 696d 6167  rn...scikit-imag
+000002b0: 650d 0a09 6e65 7467 7261 7068 0d0a 0d0a  e...netgraph....
+000002c0: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+000002d0: 7265 7175 6972 655d 0d0a 6675 6c6c 203d  require]..full =
+000002e0: 200d 0a09 7363 696b 6974 2d70 6f73 7468   ...scikit-posth
+000002f0: 6f63 730d 0a09 7472 6163 6b70 790d 0a09  ocs...trackpy...
+00000300: 7472 616d 7761 790d 0a64 6576 203d 200d  tramway..dev = .
+00000310: 0a09 666c 616b 6538 0d0a 0961 7574 6f70  ..flake8...autop
+00000320: 6570 380d 0a09 7079 7465 7374 0d0a 0970  ep8...pytest...p
+00000330: 7974 6573 742d 636f 760d 0a09 7370 6869  ytest-cov...sphi
+00000340: 6e78 0d0a 0973 7068 696e 782d 7274 642d  nx...sphinx-rtd-
+00000350: 7468 656d 650d 0a09 646f 6375 7469 6c73  theme...docutils
+00000360: 3d3d 302e 3136 0d0a 0964 6f63 380d 0a09  ==0.16...doc8...
+00000370: 6e6f 7465 626f 6f6b 0d0a 0d0a 5b6f 7074  notebook....[opt
+00000380: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+00000390: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
+000003a0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+000003b0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+000003c0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `slitflow-0.1.1/src/slitflow/data.py` & `slitflow-0.1.2/src/slitflow/data.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/fig/bar.py` & `slitflow-0.1.2/src/slitflow/fig/bar.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/fig/figure.py` & `slitflow-0.1.2/src/slitflow/fig/figure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import io
 
 import numpy as np
+import cv2
 import matplotlib
-matplotlib.use("TKAgg")
 import matplotlib.pyplot as plt
-import cv2
 
-from ..data import Pickle
 from ..img.image import RGB
+from ..data import Pickle
+from .. import MATPLOTLIB_BACKEND
+
+matplotlib.use(MATPLOTLIB_BACKEND)
 
 
 class Figure(Pickle):
     """Figure Data saved as matplotlib pickle object.
 
     """
     EXT = '.fig'
```

### Comparing `slitflow-0.1.1/src/slitflow/fig/image.py` & `slitflow-0.1.2/src/slitflow/fig/image.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/fig/line.py` & `slitflow-0.1.2/src/slitflow/fig/line.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/fig/scatter.py` & `slitflow-0.1.2/src/slitflow/fig/scatter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/fig/style.py` & `slitflow-0.1.2/src/slitflow/fig/style.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/fig/trajectory.py` & `slitflow-0.1.2/src/slitflow/fig/trajectory.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/fun/img.py` & `slitflow-0.1.2/src/slitflow/fun/img.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/fun/misc.py` & `slitflow-0.1.2/src/slitflow/fun/misc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/fun/palette.py` & `slitflow-0.1.2/src/slitflow/fun/palette.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/img/calc.py` & `slitflow-0.1.2/src/slitflow/img/calc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/img/convert.py` & `slitflow-0.1.2/src/slitflow/img/convert.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/img/filter.py` & `slitflow-0.1.2/src/slitflow/img/filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/img/image.py` & `slitflow-0.1.2/src/slitflow/img/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,16 @@
                 stack[i, :, :] = np.flipud(tif.pages[i].asarray())
             stacks.append(stack)
         return np.concatenate(stacks, axis=0)
 
     def save_data(self, stack, path):
         """Save :class:`numpy.ndarray` data into tiff file.
         """
+        if stack.size == 0:
+            return
         with tf.TiffWriter(path) as tif:
             for i in np.arange(0, stack.shape[0]):
                 tif.write(np.flipud(stack[i, :, :]),
                           photometric="minisblack",
                           contiguous=True, description="",
                           resolution=(1, 1))
 
@@ -49,19 +51,27 @@
         """
         if not any([x is not None for x in self.data]):
             return  # e.g. data.load.image.MovieFromFolder
         stack = np.concatenate(self.data, axis=0)
         col_name = self.info.get_column_name(type="col")
         col_dict = self.info.get_column_type()
         stack = stack.astype(col_dict[col_name[0]])
-        lens = self.info.file_index().groupby("_split").size().values
-        # TODO: test
+        if stack.size == 0:
+            self.data = [stack]
+            return
+        file_index = self.info.file_index()
+        if "_file" not in file_index.columns:
+            lens = file_index.groupby(
+                ["_split"]).size().values
+        else:
+            lens = file_index.groupby(
+                ["_file", "_split"]).size().values
         if len(lens) == 0 or lens[0] == 0:
             starts = [0]
-            ends = [1]
+            ends = [stack.shape[0]]
         else:
             starts = np.delete(np.append(np.zeros(1), np.cumsum(lens)), -1)
             starts = starts.astype("int32").tolist()
             ends = starts + lens
             ends = ends.astype("int32").tolist()
         stacks = []
         for start, end in zip(starts, ends):
```

### Comparing `slitflow-0.1.1/src/slitflow/img/montage.py` & `slitflow-0.1.2/src/slitflow/img/montage.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/img/noise.py` & `slitflow-0.1.2/src/slitflow/img/noise.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/img/plot.py` & `slitflow-0.1.2/src/slitflow/img/plot.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/info.py` & `slitflow-0.1.2/src/slitflow/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             if "_split" in self.index.columns:
                 self.index.drop(columns=["_split"], inplace=True)
             if "_file" in self.index.columns:
                 self.index.drop(columns=["_file"], inplace=True)
             self.index = pd.concat([self.index, df]).drop_duplicates()
             self.set_index_file_no()
 
-    def save_index(self):
+    def save_index(self, load_index=True):
         """Update index information file.
 
         The file size is reduced by excluding duplicate higher-level
         hierarchical numbers as follows:
 
         .. code-block:: python
 
@@ -135,15 +135,16 @@
         .. caution::
 
             This method updates rather than overwrites existing index files.
             This process is necessary to save the split file, but if there is
             an unrelated index file with the same name, it must be deleted.
 
         """
-        self.load_index()
+        if load_index:
+            self.load_index()
         index_path = self.path + "x"
         if "_split" in self.index.columns:
             self.index.drop(columns=["_split"], inplace=True)
         if "_file" in self.index.columns:
             self.index.drop(columns=["_file"], inplace=True)
 
         # size reducing code
@@ -163,16 +164,21 @@
 
         with open(index_path, mode="w") as f:
             f.write(idx)
 
     def set_index_file_no(self):
         """Add file number column to the index table according to split depth.
         """
+        if "_file" in self.index.columns:
+            if not self.index['_file'].isna().any():
+                return
         index_names = self.get_column_name("index")
-        if self.split_depth() > 0:
+        if len(self.index) == 0:
+            return
+        elif self.split_depth() > 0:
             grouped = self.index.groupby(rl(index_names[:self.split_depth()]))
             dfs = list(list(zip(*grouped))[1])
             for i, df in enumerate(dfs):
                 df["_file"] = i
             self.index = pd.concat(dfs)
         else:
             self.index["_file"] = 0
@@ -205,14 +211,17 @@
         """Return index table of current file number.
 
         Returns:
             pandas.DataFrame: Index table of current split file
         """
         self.set_index_file_no()
         index = self.index.copy()
+        if len(index) == 0:
+            self.file_nos = [0]
+            return index
         if not hasattr(self, "file_nos"):
             self.set_file_nos(None)
         return index[index["_file"].isin(self.file_nos)]
 
     def save(self, info_path=None):
         """Save data information as a JSON file.
 
@@ -245,19 +254,31 @@
         self.split_depth_req = split_depth
         index_names = self.get_column_name("index")
         if split_depth > 0:
             if "_split" in self.index.columns:
                 index = self.index.drop(["_split"], axis=1)
             else:
                 index = self.index
-            split = index[index_names[:split_depth]].drop_duplicates()\
-                .reset_index(drop=True)
-            split["_split"] = split.index
-            self.index = index.merge(split, on=index_names[:split_depth])
+            if "_file" not in self.index.columns:
+                index["_file"] = []
+            if len(index) == 0:
+                self.index = index
+                return  # if no data is selected.
+            grouped = index.groupby("_file")
+            dfs_split = []
+            for _, df_file in grouped:
+                df_split = df_file[index_names[:split_depth]].drop_duplicates()
+                df_split["_split"] = range(len(df_split))
+                dfs_split.append(df_split)
+            df_split = pd.concat(dfs_split)
+            self.index = index.merge(df_split, on=index_names[:split_depth])
+            self.index = self.index.reindex(
+                index_names + ["_file", "_split"], axis=1)
         else:
+            self.index["_file"] = 0
             self.index["_split"] = 0
 
     def get_dict(self):
         """Return a dictionary of all information for saving.
 
         Returns:
             dict: Dictionary of column, param and meta dictionaries
```

### Comparing `slitflow-0.1.1/src/slitflow/load/table.py` & `slitflow-0.1.2/src/slitflow/load/table.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/load/tif.py` & `slitflow-0.1.2/src/slitflow/load/tif.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """Import a tiff image as the top level of the observation data.
 
     Args:
         reqs[] (None): Input Data is not required.
         param["path"] (str): Path to a tiff file.
         param["length_unit"] (str): String of length unit such as "um",
             "nm", "pix". This string is used as column name footers and units.
-        param["pitch"] (float): Pixel size in length_unit/pix.
+        param["pitch"] (float, optional): Pixel size in length_unit/pix.
         param["interval"] (float, optional): Time interval.
         param["index_cols"] (list of list, optional): Column names of indexes.
             Each list should have [depth number, column name, description].
             Defaults to [[1, "img_no","Image number"]].
         param["img_nums"] (list of int, optional): Set if image numbers are not
             [1,2,3,...,total_images].
         param["value_type"] (str): Value type of each pixel. "uint8", "uint16"
@@ -56,17 +56,18 @@
         for index_col in param["index_cols"]:
             self.info.add_column(
                 index_col[0], index_col[1], "int32", "num", index_col[2])
         self.info.add_column(
             0, "intensity", param["value_type"], "a.u.", "Pixel intensity")
         self.info.add_param(
             "length_unit", param["length_unit"], "str", "Unit of length")
-        self.info.add_param(
-            "pitch", param["pitch"], param["length_unit"] + "/pix",
-            "Length per pixel")
+        if "pitch" in param:
+            self.info.add_param(
+                "pitch", param["pitch"], param["length_unit"] + "/pix",
+                "Length per pixel")
         self.info.add_param(
             "img_size", [int(load_param["ImgWidth"]), int(
                 load_param["ImgHeight"])], "pix", "[width, height] of image")
         if "interval" in param:
             self.info.add_param(
                 "interval", param["interval"], "float", "Time interval")
         if "img_nums" not in param:
```

### Comparing `slitflow-0.1.1/src/slitflow/loc/convert.py` & `slitflow-0.1.2/src/slitflow/loc/convert.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/loc/fit.py` & `slitflow-0.1.2/src/slitflow/loc/fit.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/loc/mask.py` & `slitflow-0.1.2/src/slitflow/loc/mask.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import pandas as pd
 
 from ..tbl.table import Table
 from .. import setreqs
 
 
 class Value(Table):
     """Create mask value column at the coordinate position of each X and Y.
@@ -17,15 +18,15 @@
         reqs[0] (Table): Table including X,Y-coordinates. Required params;
             ``length_unit``, ``pitch``.
         reqs[1] (Image): Image stack to pick up intensity.
         param["add_cols"] (list of str, optional): Additional columns to copy
             from required table. If this param is not defined, index columns
             are copied.
         param["split_depth"] (int): File split depth number.
-        
+
     Returns:
         Table: Table containing mask value column
     """
 
     def set_reqs(self, reqs, param):
         """Drop elements that exist only in one required data.
         """
@@ -71,14 +72,16 @@
                 result table.
 
         Returns:
             pandas.DataFrame: Table containing mask value column
         """
         df = reqs[0].copy()
         img = reqs[1].copy()
+        if img.shape[0] > 1:
+            raise Exception("Image must be split into single frames.")
         frm = img[0, :, :]
         x = df[param["calc_cols"][0]].values / param["pitch"]
         y = df[param["calc_cols"][1]].values / param["pitch"]
         x_pos = np.floor(x).astype("int")
         y_pos = np.floor(y).astype("int")
         vals = []
         for x, y in zip(x_pos, y_pos):
@@ -108,14 +111,19 @@
             ``pitch``, ``length_unit``.
         reqs[1] (Image): Mask image to select table.
         param["split_depth"] (int): File split depth number.
 
     Returns:
         Table: Table with rows located inside mask image
     """
+    _temp_index = []
+
+    def __init__(self, info_path=None):
+        super().__init__(info_path)
+        BinaryImage._temp_index = []
 
     def set_reqs(self, reqs, param):
         """Drop elements that exist only in one required data.
         """
         self.reqs = setreqs.and_2reqs(reqs)
 
     def set_info(self, param={}):
@@ -124,14 +132,17 @@
         self.info.copy_req(0)
         self.info.copy_req(1, "param")
         length_unit = self.info.get_param_value("length_unit")
         calc_cols = ["x_" + length_unit, "y_" + length_unit]
         self.info.add_param(
             "calc_cols", calc_cols, "list of str",
             "Columns for X,Y-coordinate")
+        index_cols = self.info.get_column_name("index")
+        self.info.add_param("index_cols", index_cols, "list of str",
+                            "Columns for index")
         self.info.set_split_depth(param["split_depth"])
 
     @staticmethod
     def process(reqs, param):
         """Select table rows that have coordinates inside the binary mask.
 
         Args:
@@ -155,9 +166,29 @@
         for x, y in zip(x_pos, y_pos):
             if (x < 0) or (frm.shape[1] <= x) or \
                     (y < 0) or (frm.shape[0] <= y):
                 vals.append(0)
             else:
                 vals.append(frm[y, x])
         df["mask_val"] = vals
+
+        df_index = df[param["index_cols"]].drop_duplicates()
+        if len(df_index) < len(df):
+            BinaryImage._temp_index.append(df_index)
+        else:
+            df_index = df[param["index_cols"] + ["mask_val"]]
+            BinaryImage._temp_index.append(df_index)
         df = df[df["mask_val"] > 0]
         return df.drop(["mask_val"], axis=1)
+
+    def set_index(self):
+        """Set the index based on the saved temporal index.
+
+        The file number should be added to the masked index not to skip the
+        file number that is not selected.
+
+        """
+        self.info.index = pd.concat(BinaryImage._temp_index)
+        self.info.set_index_file_no()
+        if "mask_val" in self.info.index.columns:
+            self.info.index = self.info.index[self.info.index["mask_val"] > 0]
+            self.info.index = self.info.index.drop(columns=["mask_val"])
```

### Comparing `slitflow-0.1.1/src/slitflow/loc/random.py` & `slitflow-0.1.2/src/slitflow/loc/random.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/manager.py` & `slitflow-0.1.2/src/slitflow/manager.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/name.py` & `slitflow-0.1.2/src/slitflow/name.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/setindex.py` & `slitflow-0.1.2/src/slitflow/setindex.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,23 +30,30 @@
     This function can only be used for
     :class:`~slitflow.tbl.table.Table` objects.
 
     Args:
         Data (Table): Table data containing result :class:`pandas.DataFrame`.
     """
     index_cols = Data.info.get_column_name("index")
-    index = pd.concat(Data.data)[index_cols].drop_duplicates()
-    Data.info.index = pd.concat([Data.info.index, index]).drop_duplicates()
-    Data.info.set_index_file_no()
+    if (len(index_cols) > 0) & (len(Data.data) > 0):
+        index = pd.concat(Data.data)[index_cols].drop_duplicates()
+        if len(Data.info.index) == 0:
+            Data.info.index = pd.DataFrame(columns=index_cols)
+        Data.info.index = pd.merge(
+            Data.info.index, index, on=index_cols, how="outer")
+        Data.info.set_index_file_no()
+    else:
+        # for split data with no data
+        Data.info.index = pd.DataFrame(columns=index_cols)
 
 
 def from_req_plus_data(Data, req_no):
     """Copy index from required data index and result pandas.DataFrame.
 
-    This function can only be used for 
+    This function can only be used for
     :class:`~slitflow.tbl.table.Table` objects. This function is not
     used in general classes.
 
     Args:
         Data (Data): Data object containing result :class:`pandas.DataFrame` to
             paste index.
         req_no (int): Indicator number of the required data list to copy index.
@@ -56,19 +63,7 @@
     index_req = Data.reqs[req_no].info.file_index()[
         index_cols_req].drop_duplicates()
     index_cols = Data.info.get_column_name("index")
     index_data = pd.concat(Data.data)[index_cols].drop_duplicates()
     and_list = list(set(index_data) & set(index_req))
     index = pd.merge(index_data, index_req, on=and_list)
     Data.info.index = pd.concat([Data.info.index, index]).drop_duplicates()
-
-# Prepared but not used.
-# def and_2reqs(Data):
-#     """Drop index rows that exist only in one required data.
-
-#     Args:
-#         Data (Data): Result Data object containing required data.
-#     """
-#     index_0 = Data.reqs[0].info.index.drop(["_file", "_split"], axis=1)
-#     index_1 = Data.reqs[1].info.index.drop(["_file", "_split"], axis=1)
-#     index = pd.concat([index_0, index_1])
-#     Data.info.index = index[index.duplicated()]
```

### Comparing `slitflow-0.1.1/src/slitflow/tbl/convert.py` & `slitflow-0.1.2/src/slitflow/tbl/convert.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,18 +20,23 @@
         Table: Sorted Table
     """
 
     def set_info(self, param={}):
         """Copy info from reqs[0] and change depths.
         """
         self.info.copy_req(0)
-        for depth, name in zip(param["new_depths"],
-                               self.info.get_column_name("index")):
+        index_cols = self.info.get_column_name("index")
+        if len(index_cols) != len(param["new_depths"]):
+            raise Exception(
+                "The number of new depths must be equal to the number\
+                    of index columns in the table.")
+        for depth, name in zip(param["new_depths"], index_cols):
             self.info.reset_depth(name, depth=depth)
         self.info.sort_column()
+        self.info.sort_index()
         self.info.add_param("new_depths", param["new_depths"], "list of int",
                             "Target depth of index")
         self.info.set_split_depth(param["split_depth"])
 
     @staticmethod
     def process(reqs, param):
         """Change column depths and sort values.
@@ -65,56 +70,77 @@
         else:
             df = df[new_cols]
         df = df.sort_values(new_cols).reset_index(drop=True)
         return df
 
 
 class AddColumn(Table):
-    """Add a new column with values.
+    """Add new columns with explicit values to a table.
 
     .. caution::
 
-        Do not split the required table.
+        Do not split the input table.
+        TODO: col_values should have the same length as the input table.
 
     Args:
-        reqs[0] (Table): Table to add column.
-        param["col_info"] (list): Information of new column. The list should be
-            [depth, name, type, unit, description]
-        param["col_values"] (array-like): Value list of new column.
-        param["split_depth"] (int): File split depth number.
+        reqs[0] (Table): The input table to add columns to.
+        param["col_info"] (list): Information about the new column. The list
+            should contain [depth, name, type, unit, description] or list of
+            it.
+        param["col_values"] (list): The values of the new column. The length of
+            the list should be equal to the length of the "col_info" list.
+        param["split_depth"] (int): The file split depth number.
 
     Returns:
-        Table: Column-added Table
+        Table: The table with the new column.
     """
 
     def set_info(self, param={}):
-        """Copy info from reqs[0] and add column.
+        """Copy info from reqs[0] and add columns.
         """
         self.info.copy_req(0)
-        self.info.add_column(*param["col_info"])
+        if self.reqs[0].info.split_depth() > 0:
+            raise Exception("Do not split the input table.")
+
+        if isinstance(param["col_info"][0], list):
+            names = []
+            for col in param["col_info"]:
+                self.info.add_column(*col)
+                names.append(col[1])
+        else:
+            self.info.add_column(*param["col_info"])
+            names = param["col_info"][1]
         self.info.add_param("col_values", param["col_values"], "list",
                             "Values of new column")
-        self.info.add_param("col_name", param["col_info"][1], "str",
+        self.info.add_param("col_name", names, "str or list",
                             "New column name")
         self.info.set_split_depth(param["split_depth"])
 
     @staticmethod
     def process(reqs, param):
-        """Add a new column with values.
+        """Add new columns with explicit values to a table.
 
         Args:
-            reqs[0] (pandas.DataFrame): Table to add column.
-            param["col_values"] (array-like): Value list of new column.
-            param["col_name"] (str): New column name.
+            reqs[0] (pandas.DataFrame): The input table to add columns to.
+            param["col_name"] (str): The names of the columns to add.
+            param["col_values"] (list): The values of the new column. The
+                length of the list should be equal to the length of the
+                "col_name" list.
 
         Returns:
-            pandas.DataFrame: Column-added table
+            pandas.DataFrame:  The table with the new column.
         """
         df = reqs[0].copy()
-        df[param["col_name"]] = param["col_values"]
+
+        if isinstance(param["col_name"], list):
+            for col_name, col_values in zip(param["col_name"],
+                                            param["col_values"]):
+                df[col_name] = col_values
+        else:
+            df[param["col_name"]] = param["col_values"]
         return df
 
 
 class Obs2Depth(Table):
     """Merge tables from different observations into a top level depth.
 
     .. caution::
```

### Comparing `slitflow-0.1.1/src/slitflow/tbl/create.py` & `slitflow-0.1.2/src/slitflow/tbl/create.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/tbl/filter.py` & `slitflow-0.1.2/src/slitflow/tbl/filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/tbl/math.py` & `slitflow-0.1.2/src/slitflow/tbl/math.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/tbl/stat.py` & `slitflow-0.1.2/src/slitflow/tbl/stat.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/tbl/table.py` & `slitflow-0.1.2/src/slitflow/tbl/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         df = pd.concat(self.data)
         df_index = self.info.index.copy()
         common_cols = list(set(df_index.columns) & set(df.columns))
         if len(common_cols) == 0:
             return
         if len(df) == 0:
             return  # see test_trj_filter
-        df = df_index.merge(df)
-        grouped = df.groupby("_split")
+        df = pd.merge(df, df_index, on=common_cols, how="left")
+        grouped = df.groupby(["_file", "_split"])
         self.data = list(list(zip(*grouped))[1])
         data = []
         for df in self.data:
             data.append(df.drop(["_file", "_split"], axis=1))
         self.data = data
 
     def set_index(self):
@@ -67,15 +67,15 @@
     required data is :class:`numpy.ndarray` that do not have ``img_no``
     information, we have to add ``img_no`` from
     :attr:`~slitflow.info.Info.index`.
 
     """
     df_index = self.reqs[req_no].info.file_index()
     dfs = []
-    for i, (_, row) in enumerate(df_index.groupby("_split")):
+    for i, (_, row) in enumerate(df_index.groupby(["_file", "_split"])):
         row_index = row.drop_duplicates()\
             .drop(["_file", "_split"], axis=1).reset_index(drop=True)
         df = self.data[i]
         df_mrg = pd.concat([row_index, df], axis=1)
         dfs.append(df_mrg.fillna(method="ffill").astype(
             self.info.get_column_type()))
     self.data = dfs
@@ -87,15 +87,15 @@
     This function is used in :meth:`~slitflow.data.Data.post_run`
     to append index information into the result data table.
     This function merge index tables that have overlapping columns.
 
     """
     df_index = self.reqs[req_no].info.file_index()
     dfs = []
-    for i, (_, row) in enumerate(df_index.groupby("_split")):
+    for i, (_, row) in enumerate(df_index.groupby(["_file", "_split"])):
         row_index = row.drop_duplicates()\
             .drop(["_file", "_split"], axis=1).reset_index(drop=True)
         df = self.data[i]
         df_mrg = row_index.merge(df, on=on_col_name)
         dfs.append(df_mrg.fillna(method="ffill").astype(
             self.info.get_column_type()).reset_index(drop=True))
     self.data = dfs
```

### Comparing `slitflow-0.1.1/src/slitflow/trj/filter.py` & `slitflow-0.1.2/src/slitflow/trj/filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/trj/msd.py` & `slitflow-0.1.2/src/slitflow/trj/msd.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/trj/random.py` & `slitflow-0.1.2/src/slitflow/trj/random.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/trj/wfastspt.py` & `slitflow-0.1.2/src/slitflow/trj/wfastspt.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,14 +703,15 @@
             fitparams, JumpProb=Prob, r=HistVec, fit2states=fit2states,
             LocError=df_fit.sigma[0], dT=param['interval'], dZ=param['dZ'],
             a=param['a'], b=param['b'], norm=True,
             useZcorr=param['useZcorr'])
 
         df = to_model_hist_df(HistVec, y)
         df["is_cdf"] = int(not param["show_pdf"])
+        df = df[df_hist.columns]
         return df
 
 
 def to_model_hist_df(HistVec, y):
     """Convert jump length distribution histogram model to
     :class:`pandas.DataFrame`.
```

### Comparing `slitflow-0.1.1/src/slitflow/trj/wtrackpy.py` & `slitflow-0.1.2/src/slitflow/trj/wtrackpy.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/trj/wtramway.py` & `slitflow-0.1.2/src/slitflow/trj/wtramway.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow/user/template.py` & `slitflow-0.1.2/src/slitflow/user/template.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/slitflow.egg-info/PKG-INFO` & `slitflow-0.1.2/src/slitflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: slitflow
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python framework for single-molecule dynamics and localization analysis
 Author: Yuma Ito
 Author-email: yitou@bio.titech.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: full
+Provides-Extra: dev
 License-File: LICENCE
 
 # Slitflow
 
 **Slitflow** is a Python package that aims to construct a fully reproducible and universally accessible workflow for single-molecule analysis—namely, **S**ingle-molecule **L**ocalization-**I**ntegrated **T**rajectory analysis work**FLOW**.
 
 **Slitflow** comprises a flexible Data class that executes a task and stores the resulting data. A Data object can be input to the next Data object, the network of Data objects forming the entire workflow of complex single-molecule analysis, from image pre-processing to publication-quality figure creation.
```

### Comparing `slitflow-0.1.1/src/slitflow.egg-info/SOURCES.txt` & `slitflow-0.1.2/src/slitflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,27 +33,29 @@
 src/slitflow/img/convert.py
 src/slitflow/img/create.py
 src/slitflow/img/filter.py
 src/slitflow/img/image.py
 src/slitflow/img/montage.py
 src/slitflow/img/noise.py
 src/slitflow/img/plot.py
+src/slitflow/img/proc.py
 src/slitflow/load/__init__.py
 src/slitflow/load/table.py
 src/slitflow/load/tif.py
 src/slitflow/loc/__init__.py
 src/slitflow/loc/convert.py
 src/slitflow/loc/fit.py
 src/slitflow/loc/mask.py
 src/slitflow/loc/random.py
 src/slitflow/tbl/__init__.py
 src/slitflow/tbl/convert.py
 src/slitflow/tbl/create.py
 src/slitflow/tbl/filter.py
 src/slitflow/tbl/math.py
+src/slitflow/tbl/proc.py
 src/slitflow/tbl/stat.py
 src/slitflow/tbl/table.py
 src/slitflow/trj/__init__.py
 src/slitflow/trj/filter.py
 src/slitflow/trj/msd.py
 src/slitflow/trj/random.py
 src/slitflow/trj/wfastspt.py
@@ -75,14 +77,15 @@
 src/tests/test_img_calc.py
 src/tests/test_img_create.py
 src/tests/test_img_filter.py
 src/tests/test_img_image.py
 src/tests/test_img_montage.py
 src/tests/test_img_noise.py
 src/tests/test_img_plot.py
+src/tests/test_img_proc.py
 src/tests/test_info.py
 src/tests/test_load_table.py
 src/tests/test_load_tif.py
 src/tests/test_loc_convert.py
 src/tests/test_loc_fit.py
 src/tests/test_loc_mask.py
 src/tests/test_loc_random.py
@@ -90,14 +93,15 @@
 src/tests/test_name.py
 src/tests/test_setindex.py
 src/tests/test_setreqs.py
 src/tests/test_tbl_convert.py
 src/tests/test_tbl_create.py
 src/tests/test_tbl_filter.py
 src/tests/test_tbl_math.py
+src/tests/test_tbl_proc.py
 src/tests/test_tbl_stat.py
 src/tests/test_tbl_table.py
 src/tests/test_trj_filter.py
 src/tests/test_trj_msd.py
 src/tests/test_trj_random.py
 src/tests/test_trj_wfastspt.py
 src/tests/test_trj_wtrackpy.py
```

### Comparing `slitflow-0.1.1/src/tests/test_data.py` & `slitflow-0.1.2/src/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_fig_bar.py` & `slitflow-0.1.2/src/tests/test_fig_bar.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_fig_figure.py` & `slitflow-0.1.2/src/tests/test_fig_figure.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_fig_image.py` & `slitflow-0.1.2/src/tests/test_fig_image.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_fig_line.py` & `slitflow-0.1.2/src/tests/test_fig_line.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_fig_scatter.py` & `slitflow-0.1.2/src/tests/test_fig_scatter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_fig_style.py` & `slitflow-0.1.2/src/tests/test_fig_style.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_fig_trajectory.py` & `slitflow-0.1.2/src/tests/test_fig_trajectory.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_fun.py` & `slitflow-0.1.2/src/tests/test_fun.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_getting_started.py` & `slitflow-0.1.2/src/tests/test_getting_started.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_img_calc.py` & `slitflow-0.1.2/src/tests/test_img_calc.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_img_create.py` & `slitflow-0.1.2/src/tests/test_img_noise.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 import pytest
+import numpy as np
 
 import slitflow as sf
 
 
 @pytest.fixture
-def Index():
-    D = sf.tbl.create.Index()
-    D.run([], {"index_counts": [1, 1], "type": "trajectory",
-               "split_depth": 0})
-    return D
+def Black():
+    D1 = sf.tbl.create.Index()
+    D1.run([], {"index_counts": [1, 1], "type": "trajectory",
+                "split_depth": 0})
+    D2 = sf.img.create.Black()
+    D2.run([D1], {"pitch": 0.1, "interval": 0.1,
+                  "img_size": [100, 100], "length_unit": "um",
+                  "split_depth": 0})
+    return D2
 
 
-def test_Black(Index):
-    D = sf.img.create.Black()
-    D.run([Index], {"pitch": 0.1, "interval": 0.1,
-                    "img_size": [100, 100], "length_unit": "um",
-                    "split_depth": 0})
-    assert D.data[0].shape == (1, 100, 100)
-
-
-def test_RandomRGB(Index):
-    D = sf.img.create.RandomRGB()
-    D.run([Index], {"pitch": 0.1, "interval": 0.1, "img_size": [100, 100],
-                    "seed": 1, "length_unit": "um",
-                    "split_depth": 0})
-    assert D.data[0].shape == (3, 100, 100)
+def test_Gauss(Black):
+    D = sf.img.noise.Gauss()
+    D.run([Black], {"sigma": 1, "baseline": 1, "seed": 1, "split_depth": 0})
+    assert np.round(np.mean(D.data[0])) == 1
```

### Comparing `slitflow-0.1.1/src/tests/test_img_filter.py` & `slitflow-0.1.2/src/tests/test_img_filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_img_image.py` & `slitflow-0.1.2/src/tests/test_img_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     D1.run([Index], {"pitch": 0.1, "img_size": [10, 10], "length_unit": "um",
                      "split_depth": 0})
 
     D2 = sf.img.image.Image()
     D2.set_reqs([D1])
     D2.set_info({"split_depth": 0})
     assert D2.info.get_param_names() ==\
-        ['calc_cols', 'index_counts', 'pitch',
+        ['calc_cols', 'index_counts', 'pitch', 'type',
          'img_size', 'length_unit', 'split_depth']
 
 
 def test_Image_memory_error(tmpdir, Index):
     path = os.path.join(tmpdir, "test.tif")
 
     D = sf.img.create.Black()
```

### Comparing `slitflow-0.1.1/src/tests/test_img_montage.py` & `slitflow-0.1.2/src/tests/test_img_montage.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_img_plot.py` & `slitflow-0.1.2/src/tests/test_img_plot.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_info.py` & `slitflow-0.1.2/src/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_load_table.py` & `slitflow-0.1.2/src/tests/test_load_table.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_load_tif.py` & `slitflow-0.1.2/src/tests/test_load_tif.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_loc_convert.py` & `slitflow-0.1.2/src/tests/test_loc_convert.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_loc_fit.py` & `slitflow-0.1.2/src/tests/test_loc_fit.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_loc_mask.py` & `slitflow-0.1.2/src/tests/test_loc_mask.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_loc_random.py` & `slitflow-0.1.2/src/tests/test_loc_random.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_manager.py` & `slitflow-0.1.2/src/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_name.py` & `slitflow-0.1.2/src/tests/test_name.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_setindex.py` & `slitflow-0.1.2/src/tests/test_setindex.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_setreqs.py` & `slitflow-0.1.2/src/tests/test_setreqs.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_tbl_create.py` & `slitflow-0.1.2/src/tests/test_tbl_create.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_tbl_filter.py` & `slitflow-0.1.2/src/tests/test_tbl_filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_tbl_math.py` & `slitflow-0.1.2/src/tests/test_tbl_math.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_tbl_stat.py` & `slitflow-0.1.2/src/tests/test_tbl_stat.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_tbl_table.py` & `slitflow-0.1.2/src/tests/test_tbl_table.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_trj_filter.py` & `slitflow-0.1.2/src/tests/test_trj_filter.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_trj_msd.py` & `slitflow-0.1.2/src/tests/test_trj_msd.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_trj_random.py` & `slitflow-0.1.2/src/tests/test_trj_random.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_trj_wfastspt.py` & `slitflow-0.1.2/src/tests/test_trj_wfastspt.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_trj_wtrackpy.py` & `slitflow-0.1.2/src/tests/test_trj_wtrackpy.py`

 * *Files identical despite different names*

### Comparing `slitflow-0.1.1/src/tests/test_trj_wtramway.py` & `slitflow-0.1.2/src/tests/test_trj_wtramway.py`

 * *Files identical despite different names*

