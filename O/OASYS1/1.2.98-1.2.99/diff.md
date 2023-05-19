# Comparing `tmp/OASYS1-1.2.98.tar.gz` & `tmp/OASYS1-1.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OASYS1-1.2.98.tar", last modified: Wed Feb  9 22:31:30 2022, max compression
+gzip compressed data, was "dist/OASYS1-1.2.99.tar", last modified: Wed Feb  9 23:56:30 2022, max compression
```

## Comparing `OASYS1-1.2.98.tar` & `OASYS1-1.2.99.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/
--rwxrwxrwx   0 bishop    (1601)      907    35147 2018-10-03 22:11:26.000000 OASYS1-1.2.98/LICENSE
--rwxrwxrwx   0 bishop    (1601)      907      231 2020-09-17 21:31:42.000000 OASYS1-1.2.98/MANIFEST.in
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:29.000000 OASYS1-1.2.98/OASYS1.egg-info/
--rw-rw-rw-   0 bishop    (1601)      907     1382 2022-02-09 22:31:28.000000 OASYS1-1.2.98/OASYS1.egg-info/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907     5322 2022-02-09 22:31:28.000000 OASYS1-1.2.98/OASYS1.egg-info/SOURCES.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2022-02-09 22:31:28.000000 OASYS1-1.2.98/OASYS1.egg-info/dependency_links.txt
--rw-rw-rw-   0 bishop    (1601)      907      147 2022-02-09 22:31:28.000000 OASYS1-1.2.98/OASYS1.egg-info/entry_points.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2018-10-04 14:33:31.000000 OASYS1-1.2.98/OASYS1.egg-info/not-zip-safe
--rw-rw-rw-   0 bishop    (1601)      907      199 2022-02-09 22:31:28.000000 OASYS1-1.2.98/OASYS1.egg-info/requires.txt
--rw-rw-rw-   0 bishop    (1601)      907        6 2022-02-09 22:31:28.000000 OASYS1-1.2.98/OASYS1.egg-info/top_level.txt
--rw-r--r--   0 bishop    (1601)      907     1382 2022-02-09 22:31:30.000000 OASYS1-1.2.98/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907      198 2020-01-07 20:38:05.000000 OASYS1-1.2.98/README.md
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:29.000000 OASYS1-1.2.98/oasys/
--rwxrwxrwx   0 bishop    (1601)      907      245 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:29.000000 OASYS1-1.2.98/oasys/application/
--rw-rw-rw-   0 bishop    (1601)      907        0 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/application/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    35989 2021-05-05 21:17:35.000000 OASYS1-1.2.98/oasys/application/addons.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:29.000000 OASYS1-1.2.98/oasys/application/data/
--rw-rw-rw-   0 bishop    (1601)      907       68 2021-08-04 18:25:01.000000 OASYS1-1.2.98/oasys/application/data/INTERNAL_LIBRARIES_PY37.txt
--rw-rw-rw-   0 bishop    (1601)      907       96 2021-08-04 18:51:17.000000 OASYS1-1.2.98/oasys/application/data/INTERNAL_LIBRARIES_PY38.txt
--rw-rw-rw-   0 bishop    (1601)      907      117 2021-08-04 18:41:13.000000 OASYS1-1.2.98/oasys/application/data/OFFICIAL_ADDONS.txt
--rw-rw-rw-   0 bishop    (1601)      907    22419 2021-08-04 18:51:17.000000 OASYS1-1.2.98/oasys/application/internal_libraries.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:29.000000 OASYS1-1.2.98/oasys/canvas/
--rwxrwxrwx   0 bishop    (1601)      907      379 2020-07-12 22:05:28.000000 OASYS1-1.2.98/oasys/canvas/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    17470 2021-06-16 16:17:25.000000 OASYS1-1.2.98/oasys/canvas/__main__.py
--rw-rw-rw-   0 bishop    (1601)      907     3707 2021-08-04 18:43:53.000000 OASYS1-1.2.98/oasys/canvas/conf.py
--rw-rw-rw-   0 bishop    (1601)      907     1375 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/discovery.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/canvas/icons/
--rwxrwxrwx   0 bishop    (1601)      907      585 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Arrow.svg
--rwxrwxrwx   0 bishop    (1601)      907      663 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Back.svg
--rwxrwxrwx   0 bishop    (1601)      907     1174 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Document Info.svg
--rwxrwxrwx   0 bishop    (1601)      907     1975 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Documentation.svg
--rwxrwxrwx   0 bishop    (1601)      907      532 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Dropdown.svg
--rwxrwxrwx   0 bishop    (1601)      907    11459 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Get Started.svg
--rwxrwxrwx   0 bishop    (1601)      907     1336 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Grid.svg
--rwxrwxrwx   0 bishop    (1601)      907     1422 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Info.svg
--rw-rw-rw-   0 bishop    (1601)      907      813 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Install.svg
--rwxrwxrwx   0 bishop    (1601)      907      591 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Maximize Toolbar.svg
--rwxrwxrwx   0 bishop    (1601)      907      590 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Minimize Toolbar.svg
--rwxrwxrwx   0 bishop    (1601)      907     1120 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/New.svg
--rwxrwxrwx   0 bishop    (1601)      907     1414 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Open.svg
--rwxrwxrwx   0 bishop    (1601)      907      570 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Pause.svg
--rwxrwxrwx   0 bishop    (1601)      907     1165 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Recent.svg
--rwxrwxrwx   0 bishop    (1601)      907     1288 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Search.svg
--rwxrwxrwx   0 bishop    (1601)      907      861 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Text Size.svg
--rwxrwxrwx   0 bishop    (1601)      907     1364 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Tutorials.svg
--rw-rw-rw-   0 bishop    (1601)      907     1265 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/Update.svg
--rwxrwxrwx   0 bishop    (1601)      907      441 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/application.png
--rwxrwxrwx   0 bishop    (1601)      907      405 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/arrow-right.svg
--rwxrwxrwx   0 bishop    (1601)      907     1163 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/categories.png
--rwxrwxrwx   0 bishop    (1601)      907      845 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/default-category.svg
--rwxrwxrwx   0 bishop    (1601)      907      964 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/default-widget.svg
--rwxrwxrwx   0 bishop    (1601)      907      777 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/delete.png
--rwxrwxrwx   0 bishop    (1601)      907     1507 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/delete_gray.png
--rwxrwxrwx   0 bishop    (1601)      907      402 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/doc.png
--rwxrwxrwx   0 bishop    (1601)      907      659 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/error.png
--rwxrwxrwx   0 bishop    (1601)      907      692 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/exit.png
--rwxrwxrwx   0 bishop    (1601)      907     3436 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/folders.png
--rwxrwxrwx   0 bishop    (1601)      907      841 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/folders2.png
--rwxrwxrwx   0 bishop    (1601)      907      456 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/frame.png
--rwxrwxrwx   0 bishop    (1601)      907      444 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/frame2.png
--rwxrwxrwx   0 bishop    (1601)      907      691 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/information.png
--rwxrwxrwx   0 bishop    (1601)      907      380 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/leftEdge.png
--rwxrwxrwx   0 bishop    (1601)      907      380 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/leftEdgeG.png
--rwxrwxrwx   0 bishop    (1601)      907      316 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/leftEdgeR.png
--rwxrwxrwx   0 bishop    (1601)      907      662 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/moveleft.png
--rwxrwxrwx   0 bishop    (1601)      907      654 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/moveright.png
--rwxrwxrwx   0 bishop    (1601)      907   115281 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/oasys-splash-screen.png
--rw-rw-rw-   0 bishop    (1601)      907     4294 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/oasys.png
--rwxrwxrwx   0 bishop    (1601)      907      772 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/open.png
--rwxrwxrwx   0 bishop    (1601)      907     1741 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/options.png
--rwxrwxrwx   0 bishop    (1601)      907     9893 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/icons/orange-canvas.svg
--rwxrwxrwx   0 bishop    (1601)      907      561 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/output.png
--rwxrwxrwx   0 bishop    (1601)      907      652 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/print.png
--rwxrwxrwx   0 bishop    (1601)      907      380 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/rightEdge.png
--rwxrwxrwx   0 bishop    (1601)      907      380 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/rightEdgeG.png
--rwxrwxrwx   0 bishop    (1601)      907      316 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/rightEdgeR.png
--rwxrwxrwx   0 bishop    (1601)      907      590 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/save.png
--rwxrwxrwx   0 bishop    (1601)      907    19984 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/splash.png
--rwxrwxrwx   0 bishop    (1601)      907      716 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/text.png
--rwxrwxrwx   0 bishop    (1601)      907      604 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/triangle-blue.png
--rwxrwxrwx   0 bishop    (1601)      907      542 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/triangle-orange.png
--rwxrwxrwx   0 bishop    (1601)      907      626 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/triangle-red.png
--rwxrwxrwx   0 bishop    (1601)      907     1620 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/update.png
--rwxrwxrwx   0 bishop    (1601)      907     2017 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/update1.png
--rwxrwxrwx   0 bishop    (1601)      907      664 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/canvas/icons/warning.png
--rw-rw-rw-   0 bishop    (1601)      907    46060 2021-02-24 18:48:57.000000 OASYS1-1.2.98/oasys/canvas/mainwindow.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/canvas/styles/
--rwxrwxrwx   0 bishop    (1601)      907       27 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/canvas/styles/orange/
--rwxrwxrwx   0 bishop    (1601)      907      610 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/orange/Arrow.svg
--rwxrwxrwx   0 bishop    (1601)      907     1187 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/orange/Document Info.svg
--rwxrwxrwx   0 bishop    (1601)      907      545 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/orange/Dropdown.svg
--rwxrwxrwx   0 bishop    (1601)      907     1349 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/orange/Grid.svg
--rwxrwxrwx   0 bishop    (1601)      907     1435 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/orange/Info.svg
--rwxrwxrwx   0 bishop    (1601)      907      583 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/orange/Pause.svg
--rwxrwxrwx   0 bishop    (1601)      907     1301 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/orange/Search.svg
--rwxrwxrwx   0 bishop    (1601)      907      874 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/orange/Text Size.svg
--rwxrwxrwx   0 bishop    (1601)      907     8410 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/canvas/styles/orange.qss
--rw-rw-rw-   0 bishop    (1601)      907     5514 2020-07-10 00:07:35.000000 OASYS1-1.2.98/oasys/canvas/widgetsscheme.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/menus/
--rwxrwxrwx   0 bishop    (1601)      907       20 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/menus/__init__.py
--rwxrwxrwx   0 bishop    (1601)      907     1094 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/menus/menu.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/tests/
--rw-rw-rw-   0 bishop    (1601)      907        0 2019-04-22 20:00:45.000000 OASYS1-1.2.98/oasys/tests/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907      805 2019-04-22 20:00:45.000000 OASYS1-1.2.98/oasys/tests/test_addons.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/util/
--rw-rw-rw-   0 bishop    (1601)      907        0 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/util/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     2281 2019-01-10 16:01:05.000000 OASYS1-1.2.98/oasys/util/custom_distribution.py
--rwxrwxrwx   0 bishop    (1601)      907    34824 2019-01-09 22:24:45.000000 OASYS1-1.2.98/oasys/util/enhanced_grid.py
--rw-r--r--   0 bishop    (1601)      907    30174 2021-12-23 02:41:30.000000 OASYS1-1.2.98/oasys/util/error_profile_util.py
--rw-rw-rw-   0 bishop    (1601)      907     2690 2020-07-12 16:02:54.000000 OASYS1-1.2.98/oasys/util/external_command.py
--rw-rw-rw-   0 bishop    (1601)      907    31532 2018-11-15 21:52:56.000000 OASYS1-1.2.98/oasys/util/hdf5_viewer.py
--rw-rw-rw-   0 bishop    (1601)      907     1459 2022-02-03 14:55:06.000000 OASYS1-1.2.98/oasys/util/oasys_objects.py
--rw-rw-rw-   0 bishop    (1601)      907    16257 2021-10-01 20:03:40.000000 OASYS1-1.2.98/oasys/util/oasys_util.py
--rwxrwxrwx   0 bishop    (1601)      907    10660 2020-06-10 19:25:33.000000 OASYS1-1.2.98/oasys/util/random_distributions.py
--rw-rw-rw-   0 bishop    (1601)      907    12714 2021-10-01 19:58:45.000000 OASYS1-1.2.98/oasys/util/scanning_gui.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/util/script/
--rw-rw-rw-   0 bishop    (1601)      907        0 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/util/script/__init__.py
--rwxrwxrwx   0 bishop    (1601)      907    15331 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/util/script/itemmodels.py
--rwxrwxrwx   0 bishop    (1601)      907     4432 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/util/script/value.py
--rwxrwxrwx   0 bishop    (1601)      907    18561 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/util/script/variable.py
--rw-rw-rw-   0 bishop    (1601)      907      259 2022-02-09 22:31:28.000000 OASYS1-1.2.98/oasys/version.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/
--rwxrwxrwx   0 bishop    (1601)      907        8 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/widgets/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/abstract/
--rw-rw-rw-   0 bishop    (1601)      907        0 2020-06-11 02:11:38.000000 OASYS1-1.2.98/oasys/widgets/abstract/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/abstract/beamline_rendering/
--rw-r--r--   0 bishop    (1601)      907     3390 2022-02-03 14:37:45.000000 OASYS1-1.2.98/oasys/widgets/abstract/beamline_rendering/__init__.py
--rw-r--r--   0 bishop    (1601)      907    33141 2022-02-09 22:21:25.000000 OASYS1-1.2.98/oasys/widgets/abstract/beamline_rendering/ow_abstract_beamline_renderer.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/abstract/error_profile/
--rw-rw-rw-   0 bishop    (1601)      907        0 2018-11-14 21:14:18.000000 OASYS1-1.2.98/oasys/widgets/abstract/error_profile/__init__.py
--rwxrwxrwx   0 bishop    (1601)      907    44196 2022-02-03 15:01:12.000000 OASYS1-1.2.98/oasys/widgets/abstract/error_profile/abstract_dabam_height_profile.py
--rwxrwxrwx   0 bishop    (1601)      907    31855 2022-02-03 18:59:00.000000 OASYS1-1.2.98/oasys/widgets/abstract/error_profile/abstract_height_profile_simulator.py
--rwxrwxrwx   0 bishop    (1601)      907    38247 2022-02-03 15:17:05.000000 OASYS1-1.2.98/oasys/widgets/abstract/error_profile/abstract_multiple_height_profile_simulator_S.py
--rwxrwxrwx   0 bishop    (1601)      907    38252 2022-02-03 15:17:05.000000 OASYS1-1.2.98/oasys/widgets/abstract/error_profile/abstract_multiple_height_profile_simulator_T.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/abstract/scanning/
--rw-rw-rw-   0 bishop    (1601)      907        0 2020-06-11 02:11:52.000000 OASYS1-1.2.98/oasys/widgets/abstract/scanning/__init__.py
--rwxrwxrwx   0 bishop    (1601)      907     6088 2020-06-11 22:02:53.000000 OASYS1-1.2.98/oasys/widgets/abstract/scanning/abstract_scan_file_node_point.py
--rw-rw-rw-   0 bishop    (1601)      907    13397 2021-07-21 15:38:33.000000 OASYS1-1.2.98/oasys/widgets/abstract/scanning/abstract_scan_node_point.py
--rwxrwxrwx   0 bishop    (1601)      907     8296 2021-07-21 15:38:13.000000 OASYS1-1.2.98/oasys/widgets/abstract/scanning/abstract_scan_variable_node_point.py
--rw-rw-rw-   0 bishop    (1601)      907     3581 2021-06-15 23:32:53.000000 OASYS1-1.2.98/oasys/widgets/congruence.py
--rw-rw-rw-   0 bishop    (1601)      907     1331 2020-06-30 15:56:03.000000 OASYS1-1.2.98/oasys/widgets/exchange.py
--rw-rw-rw-   0 bishop    (1601)      907    12688 2022-02-04 20:01:32.000000 OASYS1-1.2.98/oasys/widgets/gui.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/loop_management/
--rw-rw-rw-   0 bishop    (1601)      907      285 2020-06-10 20:20:30.000000 OASYS1-1.2.98/oasys/widgets/loop_management/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/loop_management/icons/
--rwxrwxrwx   0 bishop    (1601)      907    87776 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/loop_management/icons/cycle.png
--rwxrwxrwx   0 bishop    (1601)      907    10231 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/loop_management/icons/loop_management.png
--rwxrwxrwx   0 bishop    (1601)      907    46217 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/loop_management/icons/pin.png
--rwxrwxrwx   0 bishop    (1601)      907     7335 2022-02-03 14:40:32.000000 OASYS1-1.2.98/oasys/widgets/loop_management/ow_node_point.py
--rwxrwxrwx   0 bishop    (1601)      907     1162 2022-02-03 14:40:32.000000 OASYS1-1.2.98/oasys/widgets/loop_management/ow_pin.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/scanning/
--rw-rw-rw-   0 bishop    (1601)      907      292 2020-06-10 20:20:30.000000 OASYS1-1.2.98/oasys/widgets/scanning/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/scanning/icons/
--rwxrwxrwx   0 bishop    (1601)      907   286710 2020-06-11 22:12:13.000000 OASYS1-1.2.98/oasys/widgets/scanning/icons/cycle_file.png
--rwxrwxrwx   0 bishop    (1601)      907   307537 2020-06-11 22:12:52.000000 OASYS1-1.2.98/oasys/widgets/scanning/icons/cycle_variable.png
--rw-rw-rw-   0 bishop    (1601)      907    17681 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/scanning/icons/scanning.png
--rwxrwxrwx   0 bishop    (1601)      907     4094 2020-06-11 22:11:00.000000 OASYS1-1.2.98/oasys/widgets/scanning/ow_scan_file_node_point.py
--rwxrwxrwx   0 bishop    (1601)      907     4126 2020-06-11 22:11:00.000000 OASYS1-1.2.98/oasys/widgets/scanning/ow_scan_variable_node_point.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/tools/
--rw-rw-rw-   0 bishop    (1601)      907      254 2018-10-03 22:11:26.000000 OASYS1-1.2.98/oasys/widgets/tools/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 22:31:30.000000 OASYS1-1.2.98/oasys/widgets/tools/icons/
--rw-rw-rw-   0 bishop    (1601)      907     3954 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/tools/icons/hdf5.png
--rwxrwxrwx   0 bishop    (1601)      907      514 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/tools/icons/histogram.png
--rw-rw-rw-   0 bishop    (1601)      907     9813 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/tools/icons/python_script.png
--rw-rw-rw-   0 bishop    (1601)      907    23757 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/tools/icons/surface_merger.png
--rw-rw-rw-   0 bishop    (1601)      907    10360 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/tools/icons/surface_reader.png
--rw-rw-rw-   0 bishop    (1601)      907    61924 2020-06-11 18:47:08.000000 OASYS1-1.2.98/oasys/widgets/tools/icons/tools.png
--rw-rw-rw-   0 bishop    (1601)      907     4686 2019-05-31 16:30:19.000000 OASYS1-1.2.98/oasys/widgets/tools/ow_hdf5_file_reader.py
--rwxrwxrwx   0 bishop    (1601)      907    24324 2020-09-02 19:23:21.000000 OASYS1-1.2.98/oasys/widgets/tools/ow_python_script.py
--rw-rw-rw-   0 bishop    (1601)      907     8735 2022-02-03 15:17:05.000000 OASYS1-1.2.98/oasys/widgets/tools/ow_surface_file_merger.py
--rw-rw-rw-   0 bishop    (1601)      907     5473 2022-02-03 15:17:05.000000 OASYS1-1.2.98/oasys/widgets/tools/ow_surface_file_reader.py
--rwxrwxrwx   0 bishop    (1601)      907     5229 2020-07-16 22:33:55.000000 OASYS1-1.2.98/oasys/widgets/widget.py
--rw-r--r--   0 bishop    (1601)      907       38 2022-02-09 22:31:30.000000 OASYS1-1.2.98/setup.cfg
--rwxrwxrwx   0 bishop    (1601)      907     5489 2022-02-09 22:31:12.000000 OASYS1-1.2.98/setup.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/
+-rwxrwxrwx   0 bishop    (1601)      907    35147 2018-10-03 22:11:26.000000 OASYS1-1.2.99/LICENSE
+-rwxrwxrwx   0 bishop    (1601)      907      231 2020-09-17 21:31:42.000000 OASYS1-1.2.99/MANIFEST.in
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/OASYS1.egg-info/
+-rw-rw-rw-   0 bishop    (1601)      907     1382 2022-02-09 23:56:30.000000 OASYS1-1.2.99/OASYS1.egg-info/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907     5322 2022-02-09 23:56:30.000000 OASYS1-1.2.99/OASYS1.egg-info/SOURCES.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2022-02-09 23:56:30.000000 OASYS1-1.2.99/OASYS1.egg-info/dependency_links.txt
+-rw-rw-rw-   0 bishop    (1601)      907      147 2022-02-09 23:56:30.000000 OASYS1-1.2.99/OASYS1.egg-info/entry_points.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2018-10-04 14:33:31.000000 OASYS1-1.2.99/OASYS1.egg-info/not-zip-safe
+-rw-rw-rw-   0 bishop    (1601)      907      199 2022-02-09 23:56:30.000000 OASYS1-1.2.99/OASYS1.egg-info/requires.txt
+-rw-rw-rw-   0 bishop    (1601)      907        6 2022-02-09 23:56:30.000000 OASYS1-1.2.99/OASYS1.egg-info/top_level.txt
+-rw-r--r--   0 bishop    (1601)      907     1382 2022-02-09 23:56:30.000000 OASYS1-1.2.99/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907      198 2020-01-07 20:38:05.000000 OASYS1-1.2.99/README.md
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/
+-rwxrwxrwx   0 bishop    (1601)      907      245 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/application/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/application/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    35989 2021-05-05 21:17:35.000000 OASYS1-1.2.99/oasys/application/addons.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/application/data/
+-rw-rw-rw-   0 bishop    (1601)      907       68 2021-08-04 18:25:01.000000 OASYS1-1.2.99/oasys/application/data/INTERNAL_LIBRARIES_PY37.txt
+-rw-rw-rw-   0 bishop    (1601)      907       96 2021-08-04 18:51:17.000000 OASYS1-1.2.99/oasys/application/data/INTERNAL_LIBRARIES_PY38.txt
+-rw-rw-rw-   0 bishop    (1601)      907      117 2021-08-04 18:41:13.000000 OASYS1-1.2.99/oasys/application/data/OFFICIAL_ADDONS.txt
+-rw-rw-rw-   0 bishop    (1601)      907    22419 2021-08-04 18:51:17.000000 OASYS1-1.2.99/oasys/application/internal_libraries.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/canvas/
+-rwxrwxrwx   0 bishop    (1601)      907      379 2020-07-12 22:05:28.000000 OASYS1-1.2.99/oasys/canvas/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    17470 2021-06-16 16:17:25.000000 OASYS1-1.2.99/oasys/canvas/__main__.py
+-rw-rw-rw-   0 bishop    (1601)      907     3707 2021-08-04 18:43:53.000000 OASYS1-1.2.99/oasys/canvas/conf.py
+-rw-rw-rw-   0 bishop    (1601)      907     1375 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/discovery.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/canvas/icons/
+-rwxrwxrwx   0 bishop    (1601)      907      585 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Arrow.svg
+-rwxrwxrwx   0 bishop    (1601)      907      663 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Back.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1174 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Document Info.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1975 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Documentation.svg
+-rwxrwxrwx   0 bishop    (1601)      907      532 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Dropdown.svg
+-rwxrwxrwx   0 bishop    (1601)      907    11459 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Get Started.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1336 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Grid.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1422 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Info.svg
+-rw-rw-rw-   0 bishop    (1601)      907      813 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Install.svg
+-rwxrwxrwx   0 bishop    (1601)      907      591 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Maximize Toolbar.svg
+-rwxrwxrwx   0 bishop    (1601)      907      590 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Minimize Toolbar.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1120 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/New.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1414 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Open.svg
+-rwxrwxrwx   0 bishop    (1601)      907      570 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Pause.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1165 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Recent.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1288 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Search.svg
+-rwxrwxrwx   0 bishop    (1601)      907      861 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Text Size.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1364 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Tutorials.svg
+-rw-rw-rw-   0 bishop    (1601)      907     1265 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/Update.svg
+-rwxrwxrwx   0 bishop    (1601)      907      441 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/application.png
+-rwxrwxrwx   0 bishop    (1601)      907      405 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/arrow-right.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1163 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/categories.png
+-rwxrwxrwx   0 bishop    (1601)      907      845 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/default-category.svg
+-rwxrwxrwx   0 bishop    (1601)      907      964 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/default-widget.svg
+-rwxrwxrwx   0 bishop    (1601)      907      777 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/delete.png
+-rwxrwxrwx   0 bishop    (1601)      907     1507 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/delete_gray.png
+-rwxrwxrwx   0 bishop    (1601)      907      402 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/doc.png
+-rwxrwxrwx   0 bishop    (1601)      907      659 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/error.png
+-rwxrwxrwx   0 bishop    (1601)      907      692 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/exit.png
+-rwxrwxrwx   0 bishop    (1601)      907     3436 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/folders.png
+-rwxrwxrwx   0 bishop    (1601)      907      841 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/folders2.png
+-rwxrwxrwx   0 bishop    (1601)      907      456 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/frame.png
+-rwxrwxrwx   0 bishop    (1601)      907      444 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/frame2.png
+-rwxrwxrwx   0 bishop    (1601)      907      691 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/information.png
+-rwxrwxrwx   0 bishop    (1601)      907      380 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/leftEdge.png
+-rwxrwxrwx   0 bishop    (1601)      907      380 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/leftEdgeG.png
+-rwxrwxrwx   0 bishop    (1601)      907      316 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/leftEdgeR.png
+-rwxrwxrwx   0 bishop    (1601)      907      662 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/moveleft.png
+-rwxrwxrwx   0 bishop    (1601)      907      654 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/moveright.png
+-rwxrwxrwx   0 bishop    (1601)      907   115281 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/oasys-splash-screen.png
+-rw-rw-rw-   0 bishop    (1601)      907     4294 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/oasys.png
+-rwxrwxrwx   0 bishop    (1601)      907      772 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/open.png
+-rwxrwxrwx   0 bishop    (1601)      907     1741 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/options.png
+-rwxrwxrwx   0 bishop    (1601)      907     9893 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/icons/orange-canvas.svg
+-rwxrwxrwx   0 bishop    (1601)      907      561 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/output.png
+-rwxrwxrwx   0 bishop    (1601)      907      652 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/print.png
+-rwxrwxrwx   0 bishop    (1601)      907      380 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/rightEdge.png
+-rwxrwxrwx   0 bishop    (1601)      907      380 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/rightEdgeG.png
+-rwxrwxrwx   0 bishop    (1601)      907      316 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/rightEdgeR.png
+-rwxrwxrwx   0 bishop    (1601)      907      590 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/save.png
+-rwxrwxrwx   0 bishop    (1601)      907    19984 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/splash.png
+-rwxrwxrwx   0 bishop    (1601)      907      716 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/text.png
+-rwxrwxrwx   0 bishop    (1601)      907      604 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/triangle-blue.png
+-rwxrwxrwx   0 bishop    (1601)      907      542 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/triangle-orange.png
+-rwxrwxrwx   0 bishop    (1601)      907      626 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/triangle-red.png
+-rwxrwxrwx   0 bishop    (1601)      907     1620 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/update.png
+-rwxrwxrwx   0 bishop    (1601)      907     2017 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/update1.png
+-rwxrwxrwx   0 bishop    (1601)      907      664 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/canvas/icons/warning.png
+-rw-rw-rw-   0 bishop    (1601)      907    46060 2021-02-24 18:48:57.000000 OASYS1-1.2.99/oasys/canvas/mainwindow.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/canvas/styles/
+-rwxrwxrwx   0 bishop    (1601)      907       27 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/canvas/styles/orange/
+-rwxrwxrwx   0 bishop    (1601)      907      610 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/orange/Arrow.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1187 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/orange/Document Info.svg
+-rwxrwxrwx   0 bishop    (1601)      907      545 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/orange/Dropdown.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1349 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/orange/Grid.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1435 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/orange/Info.svg
+-rwxrwxrwx   0 bishop    (1601)      907      583 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/orange/Pause.svg
+-rwxrwxrwx   0 bishop    (1601)      907     1301 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/orange/Search.svg
+-rwxrwxrwx   0 bishop    (1601)      907      874 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/orange/Text Size.svg
+-rwxrwxrwx   0 bishop    (1601)      907     8410 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/canvas/styles/orange.qss
+-rw-rw-rw-   0 bishop    (1601)      907     5514 2020-07-10 00:07:35.000000 OASYS1-1.2.99/oasys/canvas/widgetsscheme.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/menus/
+-rwxrwxrwx   0 bishop    (1601)      907       20 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/menus/__init__.py
+-rwxrwxrwx   0 bishop    (1601)      907     1094 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/menus/menu.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/tests/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2019-04-22 20:00:45.000000 OASYS1-1.2.99/oasys/tests/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907      805 2019-04-22 20:00:45.000000 OASYS1-1.2.99/oasys/tests/test_addons.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/util/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/util/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     2281 2019-01-10 16:01:05.000000 OASYS1-1.2.99/oasys/util/custom_distribution.py
+-rwxrwxrwx   0 bishop    (1601)      907    34824 2019-01-09 22:24:45.000000 OASYS1-1.2.99/oasys/util/enhanced_grid.py
+-rw-r--r--   0 bishop    (1601)      907    30174 2021-12-23 02:41:30.000000 OASYS1-1.2.99/oasys/util/error_profile_util.py
+-rw-rw-rw-   0 bishop    (1601)      907     2690 2020-07-12 16:02:54.000000 OASYS1-1.2.99/oasys/util/external_command.py
+-rw-rw-rw-   0 bishop    (1601)      907    31532 2018-11-15 21:52:56.000000 OASYS1-1.2.99/oasys/util/hdf5_viewer.py
+-rw-rw-rw-   0 bishop    (1601)      907     1459 2022-02-03 14:55:06.000000 OASYS1-1.2.99/oasys/util/oasys_objects.py
+-rw-rw-rw-   0 bishop    (1601)      907    16257 2021-10-01 20:03:40.000000 OASYS1-1.2.99/oasys/util/oasys_util.py
+-rwxrwxrwx   0 bishop    (1601)      907    10660 2020-06-10 19:25:33.000000 OASYS1-1.2.99/oasys/util/random_distributions.py
+-rw-rw-rw-   0 bishop    (1601)      907    12714 2021-10-01 19:58:45.000000 OASYS1-1.2.99/oasys/util/scanning_gui.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/util/script/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/util/script/__init__.py
+-rwxrwxrwx   0 bishop    (1601)      907    15331 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/util/script/itemmodels.py
+-rwxrwxrwx   0 bishop    (1601)      907     4432 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/util/script/value.py
+-rwxrwxrwx   0 bishop    (1601)      907    18561 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/util/script/variable.py
+-rw-rw-rw-   0 bishop    (1601)      907      259 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/version.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/
+-rwxrwxrwx   0 bishop    (1601)      907        8 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/widgets/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/abstract/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2020-06-11 02:11:38.000000 OASYS1-1.2.99/oasys/widgets/abstract/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/abstract/beamline_rendering/
+-rw-r--r--   0 bishop    (1601)      907     3390 2022-02-03 14:37:45.000000 OASYS1-1.2.99/oasys/widgets/abstract/beamline_rendering/__init__.py
+-rw-r--r--   0 bishop    (1601)      907    32740 2022-02-09 23:54:14.000000 OASYS1-1.2.99/oasys/widgets/abstract/beamline_rendering/ow_abstract_beamline_renderer.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/abstract/error_profile/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2018-11-14 21:14:18.000000 OASYS1-1.2.99/oasys/widgets/abstract/error_profile/__init__.py
+-rwxrwxrwx   0 bishop    (1601)      907    44196 2022-02-03 15:01:12.000000 OASYS1-1.2.99/oasys/widgets/abstract/error_profile/abstract_dabam_height_profile.py
+-rwxrwxrwx   0 bishop    (1601)      907    31855 2022-02-03 18:59:00.000000 OASYS1-1.2.99/oasys/widgets/abstract/error_profile/abstract_height_profile_simulator.py
+-rwxrwxrwx   0 bishop    (1601)      907    38247 2022-02-03 15:17:05.000000 OASYS1-1.2.99/oasys/widgets/abstract/error_profile/abstract_multiple_height_profile_simulator_S.py
+-rwxrwxrwx   0 bishop    (1601)      907    38252 2022-02-03 15:17:05.000000 OASYS1-1.2.99/oasys/widgets/abstract/error_profile/abstract_multiple_height_profile_simulator_T.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/abstract/scanning/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2020-06-11 02:11:52.000000 OASYS1-1.2.99/oasys/widgets/abstract/scanning/__init__.py
+-rwxrwxrwx   0 bishop    (1601)      907     6088 2020-06-11 22:02:53.000000 OASYS1-1.2.99/oasys/widgets/abstract/scanning/abstract_scan_file_node_point.py
+-rw-rw-rw-   0 bishop    (1601)      907    13397 2021-07-21 15:38:33.000000 OASYS1-1.2.99/oasys/widgets/abstract/scanning/abstract_scan_node_point.py
+-rwxrwxrwx   0 bishop    (1601)      907     8296 2021-07-21 15:38:13.000000 OASYS1-1.2.99/oasys/widgets/abstract/scanning/abstract_scan_variable_node_point.py
+-rw-rw-rw-   0 bishop    (1601)      907     3581 2021-06-15 23:32:53.000000 OASYS1-1.2.99/oasys/widgets/congruence.py
+-rw-rw-rw-   0 bishop    (1601)      907     1331 2020-06-30 15:56:03.000000 OASYS1-1.2.99/oasys/widgets/exchange.py
+-rw-r--r--   0 bishop    (1601)      907    13476 2022-02-09 23:54:14.000000 OASYS1-1.2.99/oasys/widgets/gui.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/loop_management/
+-rw-rw-rw-   0 bishop    (1601)      907      285 2020-06-10 20:20:30.000000 OASYS1-1.2.99/oasys/widgets/loop_management/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/loop_management/icons/
+-rwxrwxrwx   0 bishop    (1601)      907    87776 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/loop_management/icons/cycle.png
+-rwxrwxrwx   0 bishop    (1601)      907    10231 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/loop_management/icons/loop_management.png
+-rwxrwxrwx   0 bishop    (1601)      907    46217 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/loop_management/icons/pin.png
+-rwxrwxrwx   0 bishop    (1601)      907     7335 2022-02-03 14:40:32.000000 OASYS1-1.2.99/oasys/widgets/loop_management/ow_node_point.py
+-rwxrwxrwx   0 bishop    (1601)      907     1162 2022-02-03 14:40:32.000000 OASYS1-1.2.99/oasys/widgets/loop_management/ow_pin.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/scanning/
+-rw-rw-rw-   0 bishop    (1601)      907      292 2020-06-10 20:20:30.000000 OASYS1-1.2.99/oasys/widgets/scanning/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/scanning/icons/
+-rwxrwxrwx   0 bishop    (1601)      907   286710 2020-06-11 22:12:13.000000 OASYS1-1.2.99/oasys/widgets/scanning/icons/cycle_file.png
+-rwxrwxrwx   0 bishop    (1601)      907   307537 2020-06-11 22:12:52.000000 OASYS1-1.2.99/oasys/widgets/scanning/icons/cycle_variable.png
+-rw-rw-rw-   0 bishop    (1601)      907    17681 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/scanning/icons/scanning.png
+-rwxrwxrwx   0 bishop    (1601)      907     4094 2020-06-11 22:11:00.000000 OASYS1-1.2.99/oasys/widgets/scanning/ow_scan_file_node_point.py
+-rwxrwxrwx   0 bishop    (1601)      907     4126 2020-06-11 22:11:00.000000 OASYS1-1.2.99/oasys/widgets/scanning/ow_scan_variable_node_point.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/tools/
+-rw-rw-rw-   0 bishop    (1601)      907      254 2018-10-03 22:11:26.000000 OASYS1-1.2.99/oasys/widgets/tools/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-09 23:56:30.000000 OASYS1-1.2.99/oasys/widgets/tools/icons/
+-rw-rw-rw-   0 bishop    (1601)      907     3954 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/tools/icons/hdf5.png
+-rwxrwxrwx   0 bishop    (1601)      907      514 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/tools/icons/histogram.png
+-rw-rw-rw-   0 bishop    (1601)      907     9813 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/tools/icons/python_script.png
+-rw-rw-rw-   0 bishop    (1601)      907    23757 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/tools/icons/surface_merger.png
+-rw-rw-rw-   0 bishop    (1601)      907    10360 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/tools/icons/surface_reader.png
+-rw-rw-rw-   0 bishop    (1601)      907    61924 2020-06-11 18:47:08.000000 OASYS1-1.2.99/oasys/widgets/tools/icons/tools.png
+-rw-rw-rw-   0 bishop    (1601)      907     4686 2019-05-31 16:30:19.000000 OASYS1-1.2.99/oasys/widgets/tools/ow_hdf5_file_reader.py
+-rwxrwxrwx   0 bishop    (1601)      907    24324 2020-09-02 19:23:21.000000 OASYS1-1.2.99/oasys/widgets/tools/ow_python_script.py
+-rw-rw-rw-   0 bishop    (1601)      907     8735 2022-02-03 15:17:05.000000 OASYS1-1.2.99/oasys/widgets/tools/ow_surface_file_merger.py
+-rw-rw-rw-   0 bishop    (1601)      907     5473 2022-02-03 15:17:05.000000 OASYS1-1.2.99/oasys/widgets/tools/ow_surface_file_reader.py
+-rwxrwxrwx   0 bishop    (1601)      907     5229 2020-07-16 22:33:55.000000 OASYS1-1.2.99/oasys/widgets/widget.py
+-rw-r--r--   0 bishop    (1601)      907       38 2022-02-09 23:56:30.000000 OASYS1-1.2.99/setup.cfg
+-rwxrwxrwx   0 bishop    (1601)      907     5489 2022-02-09 23:56:21.000000 OASYS1-1.2.99/setup.py
```

### Comparing `OASYS1-1.2.98/LICENSE` & `OASYS1-1.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/OASYS1.egg-info/PKG-INFO` & `OASYS1-1.2.99/OASYS1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: OASYS1
-Version: 1.2.98
+Version: 1.2.99
 Summary: OrAnge SYnchrotron Suite
 Home-page: https://github.com/oasys-kit/OASYS1
 Author: Luca Rebuffi, Manuel Sanchez del Rio and Bioinformatics Laboratory, FRI UL
 Author-email: lrebuffi@anl.gov
 Maintainer: Luca Rebuffi, Argonne National Lab, USA
 Maintainer-email: lrebuffi@anl.gov
 License: GPLv3
```

### Comparing `OASYS1-1.2.98/OASYS1.egg-info/SOURCES.txt` & `OASYS1-1.2.99/OASYS1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/PKG-INFO` & `OASYS1-1.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: OASYS1
-Version: 1.2.98
+Version: 1.2.99
 Summary: OrAnge SYnchrotron Suite
 Home-page: https://github.com/oasys-kit/OASYS1
 Author: Luca Rebuffi, Manuel Sanchez del Rio and Bioinformatics Laboratory, FRI UL
 Author-email: lrebuffi@anl.gov
 Maintainer: Luca Rebuffi, Argonne National Lab, USA
 Maintainer-email: lrebuffi@anl.gov
 License: GPLv3
```

### Comparing `OASYS1-1.2.98/oasys/application/addons.py` & `OASYS1-1.2.99/oasys/application/addons.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/application/internal_libraries.py` & `OASYS1-1.2.99/oasys/application/internal_libraries.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/__main__.py` & `OASYS1-1.2.99/oasys/canvas/__main__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/conf.py` & `OASYS1-1.2.99/oasys/canvas/conf.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/discovery.py` & `OASYS1-1.2.99/oasys/canvas/discovery.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Arrow.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Arrow.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Back.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Back.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Document Info.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Document Info.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Documentation.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Documentation.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Dropdown.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Dropdown.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Get Started.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Get Started.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Grid.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Grid.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Info.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Info.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Install.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Install.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Maximize Toolbar.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Maximize Toolbar.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Minimize Toolbar.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Minimize Toolbar.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/New.svg` & `OASYS1-1.2.99/oasys/canvas/icons/New.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Open.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Open.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Pause.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Pause.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Recent.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Recent.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Search.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Search.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Text Size.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Text Size.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Tutorials.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Tutorials.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/Update.svg` & `OASYS1-1.2.99/oasys/canvas/icons/Update.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/categories.png` & `OASYS1-1.2.99/oasys/canvas/icons/categories.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/default-category.svg` & `OASYS1-1.2.99/oasys/canvas/icons/default-category.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/default-widget.svg` & `OASYS1-1.2.99/oasys/canvas/icons/default-widget.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/delete.png` & `OASYS1-1.2.99/oasys/canvas/icons/delete.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/delete_gray.png` & `OASYS1-1.2.99/oasys/canvas/icons/delete_gray.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/error.png` & `OASYS1-1.2.99/oasys/canvas/icons/error.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/exit.png` & `OASYS1-1.2.99/oasys/canvas/icons/exit.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/folders.png` & `OASYS1-1.2.99/oasys/canvas/icons/folders.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/folders2.png` & `OASYS1-1.2.99/oasys/canvas/icons/folders2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/information.png` & `OASYS1-1.2.99/oasys/canvas/icons/information.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/moveleft.png` & `OASYS1-1.2.99/oasys/canvas/icons/moveleft.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/moveright.png` & `OASYS1-1.2.99/oasys/canvas/icons/moveright.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/oasys-splash-screen.png` & `OASYS1-1.2.99/oasys/canvas/icons/oasys-splash-screen.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/oasys.png` & `OASYS1-1.2.99/oasys/canvas/icons/oasys.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/open.png` & `OASYS1-1.2.99/oasys/canvas/icons/open.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/options.png` & `OASYS1-1.2.99/oasys/canvas/icons/options.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/orange-canvas.svg` & `OASYS1-1.2.99/oasys/canvas/icons/orange-canvas.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/output.png` & `OASYS1-1.2.99/oasys/canvas/icons/output.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/print.png` & `OASYS1-1.2.99/oasys/canvas/icons/print.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/save.png` & `OASYS1-1.2.99/oasys/canvas/icons/save.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/splash.png` & `OASYS1-1.2.99/oasys/canvas/icons/splash.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/text.png` & `OASYS1-1.2.99/oasys/canvas/icons/text.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/triangle-blue.png` & `OASYS1-1.2.99/oasys/canvas/icons/triangle-blue.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/triangle-orange.png` & `OASYS1-1.2.99/oasys/canvas/icons/triangle-orange.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/triangle-red.png` & `OASYS1-1.2.99/oasys/canvas/icons/triangle-red.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/update.png` & `OASYS1-1.2.99/oasys/canvas/icons/update.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/update1.png` & `OASYS1-1.2.99/oasys/canvas/icons/update1.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/icons/warning.png` & `OASYS1-1.2.99/oasys/canvas/icons/warning.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/mainwindow.py` & `OASYS1-1.2.99/oasys/canvas/mainwindow.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/styles/orange/Arrow.svg` & `OASYS1-1.2.99/oasys/canvas/styles/orange/Arrow.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/styles/orange/Document Info.svg` & `OASYS1-1.2.99/oasys/canvas/styles/orange/Document Info.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/styles/orange/Dropdown.svg` & `OASYS1-1.2.99/oasys/canvas/styles/orange/Dropdown.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/styles/orange/Grid.svg` & `OASYS1-1.2.99/oasys/canvas/styles/orange/Grid.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/styles/orange/Info.svg` & `OASYS1-1.2.99/oasys/canvas/styles/orange/Info.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/styles/orange/Pause.svg` & `OASYS1-1.2.99/oasys/canvas/styles/orange/Pause.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/styles/orange/Search.svg` & `OASYS1-1.2.99/oasys/canvas/styles/orange/Search.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/styles/orange/Text Size.svg` & `OASYS1-1.2.99/oasys/canvas/styles/orange/Text Size.svg`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/styles/orange.qss` & `OASYS1-1.2.99/oasys/canvas/styles/orange.qss`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/canvas/widgetsscheme.py` & `OASYS1-1.2.99/oasys/canvas/widgetsscheme.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/menus/menu.py` & `OASYS1-1.2.99/oasys/menus/menu.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/tests/test_addons.py` & `OASYS1-1.2.99/oasys/tests/test_addons.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/custom_distribution.py` & `OASYS1-1.2.99/oasys/util/custom_distribution.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/enhanced_grid.py` & `OASYS1-1.2.99/oasys/util/enhanced_grid.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/error_profile_util.py` & `OASYS1-1.2.99/oasys/util/error_profile_util.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/external_command.py` & `OASYS1-1.2.99/oasys/util/external_command.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/hdf5_viewer.py` & `OASYS1-1.2.99/oasys/util/hdf5_viewer.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/oasys_objects.py` & `OASYS1-1.2.99/oasys/util/oasys_objects.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/oasys_util.py` & `OASYS1-1.2.99/oasys/util/oasys_util.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/random_distributions.py` & `OASYS1-1.2.99/oasys/util/random_distributions.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/scanning_gui.py` & `OASYS1-1.2.99/oasys/util/scanning_gui.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/script/itemmodels.py` & `OASYS1-1.2.99/oasys/util/script/itemmodels.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/script/value.py` & `OASYS1-1.2.99/oasys/util/script/value.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/util/script/variable.py` & `OASYS1-1.2.99/oasys/util/script/variable.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/abstract/beamline_rendering/__init__.py` & `OASYS1-1.2.99/oasys/widgets/abstract/beamline_rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/abstract/beamline_rendering/ow_abstract_beamline_renderer.py` & `OASYS1-1.2.99/oasys/widgets/abstract/beamline_rendering/ow_abstract_beamline_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,14 @@
 
 class AbstractBeamlineRenderer(widget.OWWidget):
     want_main_area = 1
 
     WIDGET_WIDTH = 1900
     WIDGET_HEIGHT = 1000
 
-    is_interactive = Setting(1)
-
     initial_height = Setting(0.0)
     use_axis = Setting(1)
     use_labels = Setting(1)
     draw_source = Setting(1)
     draw_optical_axis = Setting(1)
 
     element_expansion_factor =  Setting(1.0)
@@ -136,23 +134,16 @@
         self.setMaximumHeight(self.geometry().height())
         self.setMaximumWidth(self.geometry().width())
 
         button_box = oasysgui.widgetBox(self.controlArea, "", addSpace=False, orientation="horizontal", width=control_area_width)
 
         gui.button(button_box, self, "Restore Default View and Values", callback=self.reset_default, height=45)
 
-        button_box = oasysgui.widgetBox(self.controlArea, "", addSpace=False, orientation="horizontal", width=control_area_width)
-
-        gui.button(button_box, self, "Reset Zoom/Shift", callback=self.reset_zoom_shift, height=25)
-        gui.button(button_box, self, "Reset Rotation", callback=self.reset_rotation, height=25)
-
         gen_box = oasysgui.widgetBox(self.controlArea, "Options", addSpace=False, orientation="vertical", width=control_area_width)
 
-        gui.checkBox(gen_box, self, "is_interactive", "Real time refresh active", labelWidth=200)
-
         beamline_box = oasysgui.widgetBox(gen_box, "Beamline", addSpace=False, orientation="vertical", height=170)
 
         gui.checkBox(beamline_box, self, "use_axis", "Show axis", labelWidth=200, callback=self.refresh)
         gui.checkBox(beamline_box, self, "use_labels", "Show labels", labelWidth=200, callback=self.refresh)
         gui.checkBox(beamline_box, self, "draw_source", "Draw source", labelWidth=200, callback=self.refresh)
         gui.checkBox(beamline_box, self, "draw_optical_axis", "Draw optical axis", labelWidth=200, callback=self.refresh)
         self.le_initial_height = oasysgui.lineEdit(beamline_box, self, "initial_height", "Beam vertical baseline ", labelWidth=230, valueType=float, orientation="horizontal", callback=self.refresh)
@@ -259,65 +250,65 @@
         label = self.le_range_max.parent().layout().itemAt(0).widget()
         label.setText(label.text() + " [" + units_label + "]")
 
         self.set_units_attributes(units_label, units_to_mm)
         self.set_range(do_refresh=False)
 
     def refresh(self):
-        if self.is_interactive: self.reset_all()
+        self.render(reset_rotation=False)
+        self.figure_canvas.draw()
 
     def set_range(self, do_refresh=True):
         if self.use_range == 1:
             self.range_box_1.setVisible(True)
             self.distance_compression_factor = 1.0
         else:
             self.range_box_1.setVisible(False)
+
         if do_refresh: self.refresh()
 
     def reset_default(self):
         self.element_expansion_factor = 1.0
         self.distance_compression_factor = 1.0
         self.use_range = 0
         self.set_range(do_refresh=False)
         self.reset_all()
 
-    def reset_zoom_shift(self):
-        self.render(reset_rotation=False)
+    def reset_all(self):
+        self.render(reset_rotation=True)
         self.figure_canvas.draw()
 
     def reset_rotation(self):
         self.axis.view_init(azim=DEFAULT_AZIM, elev=DEFAULT_ELEV)
         self.figure_canvas.draw()
-
-    def reset_all(self):
-        self.render(reset_rotation=True)
+        self.figure_canvas.mark_default_view()
 
     def check_fields(self):
         congruence.checkNumber(self.initial_height, "Beam vertical baseline")
         congruence.checkStrictlyPositiveNumber(self.element_expansion_factor, "O.E. Expansion Factor")
         congruence.checkStrictlyPositiveNumber(self.distance_compression_factor, "Layout compression factor")
         if self.use_range:
             if self.range_max <= self.range_min:
                 self.range_max = self.range_min + self.tick_interval
                 self.slider_max.setValue(self.range_max*self.units_to_mm)
 
-    def render(self, reset_rotation=True, init_range=False):
+    def render(self, reset_rotation=True, on_receiving_input=False):
         try:
             self.check_fields()
 
-            render_result = self.render_beamline(reset_rotation)
+            render_result = self.render_beamline()
 
             if not render_result is None:
                 number_of_elements, centers, limits = render_result
 
                 limits[:, 0, :] *= 10.0/self.element_expansion_factor # aestetic
 
                 # sliders are integers, so they must be always in mm
 
-                if init_range:
+                if on_receiving_input:
                     self.slider_min.setMinimum(numpy.min(limits[:, 1, :])*self.units_to_mm - self.tick_interval) # for visibility
                     self.slider_min.setMaximum(numpy.max(limits[:, 1, :])*self.units_to_mm - self.tick_interval) # for consistency
                     if self.range_min*self.units_to_mm == self.slider_min.minimum() + self.tick_interval:
                         self.range_min = self.slider_min.minimum()/self.units_to_mm
                         self.slider_min.setValue(self.slider_min.minimum())
                     else:
                         self.slider_min.setValue(max(self.range_min*self.units_to_mm, numpy.min(limits[:, 1, :])*self.units_to_mm))
@@ -338,21 +329,22 @@
                 if self.draw_optical_axis:
                     if self.use_range == 1: self.draw_central_radiation_line(centers=centers, rng=numpy.array([self.range_min, self.range_max]))
                     else:                   self.draw_central_radiation_line(centers=centers)
 
                 self.format_axis(limits)
 
                 if reset_rotation: self.reset_rotation()
+                if on_receiving_input: self.figure_canvas.mark_default_view()
 
         except Exception as e:
             QMessageBox.critical(self, "Error", str(e), QMessageBox.Ok)
 
             if self.IS_DEVELOP: raise e
 
-    def render_beamline(self, reset_rotation=True):
+    def render_beamline(self):
         raise NotImplementedError()
 
     def format_axis(self, limits):
         if self.use_axis:
             self.axis.set_axis_on()
             self.axis.set_ylabel("\n\n\n\n\nDistance along beam direction [" + self.units_label + "]")
             self.axis.axes.xaxis.set_ticklabels([])
```

### Comparing `OASYS1-1.2.98/oasys/widgets/abstract/error_profile/abstract_dabam_height_profile.py` & `OASYS1-1.2.99/oasys/widgets/abstract/error_profile/abstract_dabam_height_profile.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/abstract/error_profile/abstract_height_profile_simulator.py` & `OASYS1-1.2.99/oasys/widgets/abstract/error_profile/abstract_height_profile_simulator.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/abstract/error_profile/abstract_multiple_height_profile_simulator_S.py` & `OASYS1-1.2.99/oasys/widgets/abstract/error_profile/abstract_multiple_height_profile_simulator_S.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/abstract/error_profile/abstract_multiple_height_profile_simulator_T.py` & `OASYS1-1.2.99/oasys/widgets/abstract/error_profile/abstract_multiple_height_profile_simulator_T.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/abstract/scanning/abstract_scan_file_node_point.py` & `OASYS1-1.2.99/oasys/widgets/abstract/scanning/abstract_scan_file_node_point.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/abstract/scanning/abstract_scan_node_point.py` & `OASYS1-1.2.99/oasys/widgets/abstract/scanning/abstract_scan_node_point.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/abstract/scanning/abstract_scan_variable_node_point.py` & `OASYS1-1.2.99/oasys/widgets/abstract/scanning/abstract_scan_variable_node_point.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/congruence.py` & `OASYS1-1.2.99/oasys/widgets/congruence.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/exchange.py` & `OASYS1-1.2.99/oasys/widgets/exchange.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/gui.py` & `OASYS1-1.2.99/oasys/widgets/gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -168,40 +168,58 @@
 
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 
 class FigureCanvas3D(FigureCanvas):
 
     def __init__(self, fig, ax, show_legend=True):
         super().__init__(fig)
+
+        box = widgetBox(self, "", orientation="vertical")
+        orange_gui.button(box, self, "Default View", width=100, height=35, callback=self.__default_view)
+        orange_gui.button(box, self, "Top View", width=100, height=35, callback=self.__top_view)
+        orange_gui.button(box, self, "Lateral View", width=100, height=35, callback=self.__lateral_view)
+
         self.ax = ax
         self.size_x, self.size_y = fig.get_size_inches() * fig.dpi
         self.x_c = int(self.size_x / 2)
         self.y_c = int(self.size_y / 2)
 
         self.last_pos_x = self.x_c
         self.last_pos_y = self.y_c
 
         self.__show_legend = show_legend
         self.__add_legend()
 
+        self.mark_default_view()
+
+    def mark_default_view(self):
+        self.__initial_azim = self.ax.azim
+        self.__initial_elev = self.ax.elev
+
+    def __default_view(self):
+        self.ax.view_init(azim=self.__initial_azim, elev=self.__initial_elev)
+        self.draw()
+
+    def __top_view(self):
+        self.ax.view_init(azim=0.0, elev=90.0)
+        self.draw()
+
+    def __lateral_view(self):
+        self.ax.view_init(azim=0.0, elev=0.0)
+        self.draw()
+
     def __add_legend(self):
         if self.__show_legend:
             self.ax.text2D(0.05, 0.95,
                            "Mouse Left Button -> Click and Hold: Rotate\n" +  #, Double Click: Recenter\n" + \
                            "Mouse Right Button -> Click and Hold: Zoom\n" +
                            "Mouse Left & Right Buttons or Central Button -> Click and Hold: Shift",
                            transform=self.ax.transAxes,
                            color='blue')
 
-    def __recenter(self, posx, posy):
-        pass #
-
-    def __reset_view(self):
-        pass
-
     def __pan(self, dx, dy):
         # convert dx dy -> dxx dyy dzz
         minx, maxx, miny, maxy, minz, maxz = self.ax.get_w_lims()
         elev, azim = numpy.deg2rad(self.ax.elev), numpy.deg2rad(self.ax.azim)
         dxe = (dy / self.size_y) * numpy.sin(elev)
         dye = - (dx / self.size_x)
         dze = - (dy / self.size_y) * numpy.cos(elev)
@@ -226,14 +244,16 @@
         self.ax.get_proj()
 
     def __rotate(self, dx, dy):
         self.ax.view_init(azim=art3d._norm_angle(self.ax.azim - (dx / self.size_x) * 180),
                           elev=art3d._norm_angle(self.ax.elev - (dy / self.size_y) * 180))
 
     def mouseMoveEvent(self, event):
+        print(self.ax.azim, self.ax.elev)
+
         pos_x = event.pos().x() - self.x_c
         pos_y = -(event.pos().y() - self.y_c)
 
         dx = pos_x - self.last_pos_x
         dy = pos_y - self.last_pos_y
 
         if dx == 0 and dy == 0: return
```

### Comparing `OASYS1-1.2.98/oasys/widgets/loop_management/icons/cycle.png` & `OASYS1-1.2.99/oasys/widgets/loop_management/icons/cycle.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/loop_management/icons/loop_management.png` & `OASYS1-1.2.99/oasys/widgets/loop_management/icons/loop_management.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/loop_management/icons/pin.png` & `OASYS1-1.2.99/oasys/widgets/loop_management/icons/pin.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/loop_management/ow_node_point.py` & `OASYS1-1.2.99/oasys/widgets/loop_management/ow_node_point.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/loop_management/ow_pin.py` & `OASYS1-1.2.99/oasys/widgets/loop_management/ow_pin.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/scanning/icons/cycle_file.png` & `OASYS1-1.2.99/oasys/widgets/scanning/icons/cycle_file.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/scanning/icons/cycle_variable.png` & `OASYS1-1.2.99/oasys/widgets/scanning/icons/cycle_variable.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/scanning/icons/scanning.png` & `OASYS1-1.2.99/oasys/widgets/scanning/icons/scanning.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/scanning/ow_scan_file_node_point.py` & `OASYS1-1.2.99/oasys/widgets/scanning/ow_scan_file_node_point.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/scanning/ow_scan_variable_node_point.py` & `OASYS1-1.2.99/oasys/widgets/scanning/ow_scan_variable_node_point.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/icons/hdf5.png` & `OASYS1-1.2.99/oasys/widgets/tools/icons/hdf5.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/icons/histogram.png` & `OASYS1-1.2.99/oasys/widgets/tools/icons/histogram.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/icons/python_script.png` & `OASYS1-1.2.99/oasys/widgets/tools/icons/python_script.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/icons/surface_merger.png` & `OASYS1-1.2.99/oasys/widgets/tools/icons/surface_merger.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/icons/surface_reader.png` & `OASYS1-1.2.99/oasys/widgets/tools/icons/surface_reader.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/icons/tools.png` & `OASYS1-1.2.99/oasys/widgets/tools/icons/tools.png`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/ow_hdf5_file_reader.py` & `OASYS1-1.2.99/oasys/widgets/tools/ow_hdf5_file_reader.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/ow_python_script.py` & `OASYS1-1.2.99/oasys/widgets/tools/ow_python_script.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/ow_surface_file_merger.py` & `OASYS1-1.2.99/oasys/widgets/tools/ow_surface_file_merger.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/tools/ow_surface_file_reader.py` & `OASYS1-1.2.99/oasys/widgets/tools/ow_surface_file_reader.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/oasys/widgets/widget.py` & `OASYS1-1.2.99/oasys/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `OASYS1-1.2.98/setup.py` & `OASYS1-1.2.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import platform
 
 from setuptools import setup
 
 NAME = 'OASYS1'
 
-VERSION = '1.2.98'
+VERSION = '1.2.99'
 
 ISRELEASED = True
 
 DESCRIPTION = 'OrAnge SYnchrotron Suite'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi, Manuel Sanchez del Rio and Bioinformatics Laboratory, FRI UL'
```

