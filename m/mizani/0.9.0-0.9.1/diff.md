# Comparing `tmp/mizani-0.9.0.tar.gz` & `tmp/mizani-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizani-0.9.0.tar", last modified: Sat Apr 15 15:00:08 2023, max compression
+gzip compressed data, was "mizani-0.9.1.tar", last modified: Fri May 19 16:40:47 2023, max compression
```

## Comparing `mizani-0.9.0.tar` & `mizani-0.9.1.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.802698 mizani-0.9.0/
--rw-r--r--   0 hassan     (503) staff       (20)       32 2016-06-28 12:36:41.000000 mizani-0.9.0/.gitattributes
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.738633 mizani-0.9.0/.github/
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.747629 mizani-0.9.0/.github/workflows/
--rw-r--r--   0 hassan     (503) staff       (20)     2869 2023-03-18 11:25:34.000000 mizani-0.9.0/.github/workflows/testing.yml
--rw-r--r--   0 hassan     (503) staff       (20)      751 2022-07-06 06:38:46.000000 mizani-0.9.0/.gitignore
--rw-r--r--   0 hassan     (503) staff       (20)      271 2023-04-05 12:30:47.000000 mizani-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 hassan     (503) staff       (20)      528 2023-03-18 11:25:34.000000 mizani-0.9.0/.readthedocs.yaml
--rw-r--r--   0 hassan     (503) staff       (20)     1478 2016-06-28 12:36:41.000000 mizani-0.9.0/LICENSE
--rw-r--r--   0 hassan     (503) staff       (20)     1565 2023-04-15 14:59:50.000000 mizani-0.9.0/Makefile
--rw-r--r--   0 hassan     (503) staff       (20)     3753 2023-04-15 15:00:08.801986 mizani-0.9.0/PKG-INFO
--rw-r--r--   0 hassan     (503) staff       (20)     1043 2023-04-15 14:59:50.000000 mizani-0.9.0/README.md
--rw-r--r--   0 hassan     (503) staff       (20)      375 2023-02-27 19:00:09.000000 mizani-0.9.0/codecov.yml
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.752917 mizani-0.9.0/doc/
--rw-r--r--   0 hassan     (503) staff       (20)     1134 2023-02-27 19:00:09.000000 mizani-0.9.0/doc/Makefile
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.753629 mizani-0.9.0/doc/_static/
--rw-r--r--   0 hassan     (503) staff       (20)     3143 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/_static/copybutton.js
--rw-r--r--   0 hassan     (503) staff       (20)     2494 2022-06-23 11:43:31.000000 mizani-0.9.0/doc/_static/custom.css
--rw-r--r--   0 hassan     (503) staff       (20)      148 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/bounds.rst
--rw-r--r--   0 hassan     (503) staff       (20)      182 2022-04-01 15:37:12.000000 mizani-0.9.0/doc/breaks.rst
--rw-r--r--   0 hassan     (503) staff       (20)    12437 2023-04-15 14:59:50.000000 mizani-0.9.0/doc/changelog.rst
--rw-r--r--   0 hassan     (503) staff       (20)    11659 2023-03-18 11:25:34.000000 mizani-0.9.0/doc/conf.py
--rw-r--r--   0 hassan     (503) staff       (20)      118 2022-06-23 11:43:31.000000 mizani-0.9.0/doc/docutils.conf
--rw-r--r--   0 hassan     (503) staff       (20)      158 2020-06-03 18:30:42.000000 mizani-0.9.0/doc/formatters.rst
--rw-r--r--   0 hassan     (503) staff       (20)      362 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/index.rst
--rw-r--r--   0 hassan     (503) staff       (20)      967 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/installation.rst
--rw-r--r--   0 hassan     (503) staff       (20)      170 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/palettes.rst
--rw-r--r--   0 hassan     (503) staff       (20)      116 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/scale.rst
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.754597 mizani-0.9.0/doc/sphinxext/
--rw-r--r--   0 hassan     (503) staff       (20)        0 2016-06-28 12:36:41.000000 mizani-0.9.0/doc/sphinxext/__init__.py
--rw-r--r--   0 hassan     (503) staff       (20)      368 2023-03-18 11:25:34.000000 mizani-0.9.0/doc/sphinxext/inline_code_highlight.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.764599 mizani-0.9.0/doc/theme/
--rw-r--r--   0 hassan     (503) staff       (20)      455 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/globaltoc.html
--rw-r--r--   0 hassan     (503) staff       (20)     3664 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/layout.html
--rw-r--r--   0 hassan     (503) staff       (20)       10 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/localtoc.html
--rw-r--r--   0 hassan     (503) staff       (20)     2002 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/navbar-2.html
--rw-r--r--   0 hassan     (503) staff       (20)     2072 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/navbar.html
--rw-r--r--   0 hassan     (503) staff       (20)      360 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/navbarsearchbox.html
--rw-r--r--   0 hassan     (503) staff       (20)      305 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/navbartoc.html
--rw-r--r--   0 hassan     (503) staff       (20)     1111 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/relations.html
--rw-r--r--   0 hassan     (503) staff       (20)     2614 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/search.html
--rw-r--r--   0 hassan     (503) staff       (20)      327 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/searchbox.html
--rw-r--r--   0 hassan     (503) staff       (20)     1120 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/searchresults.html
--rw-r--r--   0 hassan     (503) staff       (20)      195 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/sourcelink.html
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.766241 mizani-0.9.0/doc/theme/static/
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.739888 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.766967 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/css/
--rw-r--r--   0 hassan     (503) staff       (20)   124135 2023-02-27 19:00:09.000000 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.768253 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/js/
--rw-r--r--   0 hassan     (503) staff       (20)    40021 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js
--rw-r--r--   0 hassan     (503) staff       (20)     5924 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/bootstrap-sphinx.css_t
--rw-r--r--   0 hassan     (503) staff       (20)     5162 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/bootstrap-sphinx.js_t
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.770288 mizani-0.9.0/doc/theme/static/js/
--rw-r--r--   0 hassan     (503) staff       (20)    97163 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/js/jquery-1.12.4.min.js
--rw-r--r--   0 hassan     (503) staff       (20)       90 2023-02-27 18:48:05.000000 mizani-0.9.0/doc/theme/static/js/jquery-fix.js
--rw-r--r--   0 hassan     (503) staff       (20)     1895 2023-02-27 19:00:09.000000 mizani-0.9.0/doc/theme/theme.conf
--rw-r--r--   0 hassan     (503) staff       (20)      188 2018-10-03 08:09:15.000000 mizani-0.9.0/doc/transforms.rst
--rw-r--r--   0 hassan     (503) staff       (20)     1344 2022-06-23 11:43:31.000000 mizani-0.9.0/how-to-release.rst
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.773038 mizani-0.9.0/licences/
--rw-r--r--   0 hassan     (503) staff       (20)     1059 2016-06-28 12:36:41.000000 mizani-0.9.0/licences/HUSL_LICENSE
--rw-r--r--   0 hassan     (503) staff       (20)       77 2016-06-28 12:36:41.000000 mizani-0.9.0/licences/SCALES_LICENSE
--rw-r--r--   0 hassan     (503) staff       (20)     1498 2016-06-28 12:36:41.000000 mizani-0.9.0/licences/SEABORN_LICENSE
--rw-r--r--   0 hassan     (503) staff       (20)     1066 2016-06-28 12:36:41.000000 mizani-0.9.0/licences/SIX_LICENSE
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.781426 mizani-0.9.0/mizani/
--rw-r--r--   0 hassan     (503) staff       (20)      172 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/__init__.py
--rw-r--r--   0 hassan     (503) staff       (20)    15042 2023-03-18 11:55:22.000000 mizani-0.9.0/mizani/bounds.py
--rw-r--r--   0 hassan     (503) staff       (20)    26005 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/breaks.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.786220 mizani-0.9.0/mizani/colors/
--rw-r--r--   0 hassan     (503) staff       (20)        0 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/__init__.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.789042 mizani-0.9.0/mizani/colors/brewer/
--rw-r--r--   0 hassan     (503) staff       (20)     1717 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/brewer/__init__.py
--rw-r--r--   0 hassan     (503) staff       (20)    17728 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/brewer/diverging.py
--rw-r--r--   0 hassan     (503) staff       (20)    11725 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/brewer/qualitative.py
--rw-r--r--   0 hassan     (503) staff       (20)    24032 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/brewer/sequential.py
--rw-r--r--   0 hassan     (503) staff       (20)     1942 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/colors/color_palette.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.792109 mizani-0.9.0/mizani/external/
--rw-r--r--   0 hassan     (503) staff       (20)      104 2018-10-03 08:09:15.000000 mizani-0.9.0/mizani/external/__init__.py
--rw-r--r--   0 hassan     (503) staff       (20)     5055 2018-10-03 08:09:15.000000 mizani-0.9.0/mizani/external/crayon_rgb.py
--rw-r--r--   0 hassan     (503) staff       (20)     6488 2017-01-28 08:50:04.000000 mizani-0.9.0/mizani/external/husl.py
--rw-r--r--   0 hassan     (503) staff       (20)    28029 2018-10-03 08:09:15.000000 mizani-0.9.0/mizani/external/xkcd_rgb.py
--rw-r--r--   0 hassan     (503) staff       (20)    23347 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/formatters.py
--rw-r--r--   0 hassan     (503) staff       (20)    22690 2023-04-05 12:44:26.000000 mizani-0.9.0/mizani/palettes.py
--rw-r--r--   0 hassan     (503) staff       (20)     7476 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/scale.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.799531 mizani-0.9.0/mizani/tests/
--rw-r--r--   0 hassan     (503) staff       (20)        0 2022-06-23 11:43:31.000000 mizani-0.9.0/mizani/tests/__init__.py
--rw-r--r--   0 hassan     (503) staff       (20)    13788 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_bounds.py
--rw-r--r--   0 hassan     (503) staff       (20)     8245 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_breaks.py
--rw-r--r--   0 hassan     (503) staff       (20)     7749 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_formatters.py
--rw-r--r--   0 hassan     (503) staff       (20)     6085 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/tests/test_palettes.py
--rw-r--r--   0 hassan     (503) staff       (20)     3719 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_scale.py
--rw-r--r--   0 hassan     (503) staff       (20)     7102 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_transforms.py
--rw-r--r--   0 hassan     (503) staff       (20)     4229 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/tests/test_utils.py
--rw-r--r--   0 hassan     (503) staff       (20)    21685 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/transforms.py
--rw-r--r--   0 hassan     (503) staff       (20)      698 2023-04-05 12:30:47.000000 mizani-0.9.0/mizani/typing.py
--rw-r--r--   0 hassan     (503) staff       (20)     6684 2023-03-18 11:25:34.000000 mizani-0.9.0/mizani/utils.py
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.785058 mizani-0.9.0/mizani.egg-info/
--rw-r--r--   0 hassan     (503) staff       (20)     3753 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/PKG-INFO
--rw-r--r--   0 hassan     (503) staff       (20)     2038 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/SOURCES.txt
--rw-r--r--   0 hassan     (503) staff       (20)        1 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/dependency_links.txt
--rw-r--r--   0 hassan     (503) staff       (20)      377 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/requires.txt
--rw-r--r--   0 hassan     (503) staff       (20)        7 2023-04-15 15:00:08.000000 mizani-0.9.0/mizani.egg-info/top_level.txt
--rw-r--r--   0 hassan     (503) staff       (20)     3412 2023-04-15 14:59:50.000000 mizani-0.9.0/pyproject.toml
--rw-r--r--   0 hassan     (503) staff       (20)       38 2023-04-15 15:00:08.802884 mizani-0.9.0/setup.cfg
-drwxr-xr-x   0 hassan     (503) staff       (20)        0 2023-04-15 15:00:08.800991 mizani-0.9.0/tools/
--rwxr-xr-x   0 hassan     (503) staff       (20)      862 2022-06-23 11:43:31.000000 mizani-0.9.0/tools/build_theme.sh
--rw-r--r--   0 hassan     (503) staff       (20)     2116 2023-04-15 14:59:50.000000 mizani-0.9.0/tools/release.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.737091 mizani-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 16:40:38.000000 mizani-0.9.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.725091 mizani-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-19 16:40:38.000000 mizani-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-19 16:40:38.000000 mizani-0.9.1/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-19 16:40:38.000000 mizani-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-19 16:40:38.000000 mizani-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-19 16:40:38.000000 mizani-0.9.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-19 16:40:38.000000 mizani-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-19 16:40:38.000000 mizani-0.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-19 16:40:47.737091 mizani-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-19 16:40:38.000000 mizani-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 16:40:38.000000 mizani-0.9.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/bounds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/breaks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/formatters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/palettes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/scale.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/sphinxext/inline_code_highlight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/navbar-2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/navbarsearchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/navbartoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/relations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/searchresults.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/sourcelink.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.725091 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   124135 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/bootstrap-sphinx.css_t
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/bootstrap-sphinx.js_t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/doc/theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/js/jquery-1.12.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/js/jquery-fix.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/transforms.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/licences/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-19 16:40:38.000000 mizani-0.9.1/licences/HUSL_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 16:40:38.000000 mizani-0.9.1/licences/SCALES_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-19 16:40:38.000000 mizani-0.9.1/licences/SEABORN_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 16:40:38.000000 mizani-0.9.1/licences/SIX_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/breaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani/colors/brewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/brewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/brewer/diverging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/brewer/qualitative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/brewer/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/color_palette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/external/crayon_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/external/husl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28029 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/external/xkcd_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22688 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.737091 mizani-0.9.1/mizani/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_breaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_palettes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21685 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-19 16:40:38.000000 mizani-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:40:47.737091 mizani-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.737091 mizani-0.9.1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-05-19 16:40:38.000000 mizani-0.9.1/tools/build_theme.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-19 16:40:38.000000 mizani-0.9.1/tools/gha_check_semver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-19 16:40:38.000000 mizani-0.9.1/tools/release-checklist.md
```

### Comparing `mizani-0.9.0/.github/workflows/testing.yml` & `mizani-0.9.1/.github/workflows/testing.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
-name: build
+name: Test
 
-on: [push, pull_request]
+on:
+  push:
+    branches:
+      - '*'
+    tags-ignore:
+      - 'v[0-9]*'
+  pull_request:
+  workflow_call:
 
 jobs:
   unittests:
     runs-on: ubuntu-latest
 
     # We want to run on external PRs, but not on our own internal PRs as they'll be run
     # by the push to the branch.
```

### Comparing `mizani-0.9.0/.gitignore` & `mizani-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/.readthedocs.yaml` & `mizani-0.9.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/LICENSE` & `mizani-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/Makefile` & `mizani-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/PKG-INFO` & `mizani-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizani
-Version: 0.9.0
+Version: 0.9.1
 Summary: Scales for Python
 Author-email: Hassan Kibirige <has2k1@gmail.com>
 License: Copyright (c) 2016, Hassan Kibirige
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `mizani-0.9.0/README.md` & `mizani-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/Makefile` & `mizani-0.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/_static/copybutton.js` & `mizani-0.9.1/doc/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/_static/custom.css` & `mizani-0.9.1/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/changelog.rst` & `mizani-0.9.1/doc/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changelog
 =========
 
+v0.9.1
+------
+
+*2023-05-19*
+
+Bug Fixes
+*********
+
+- Fixed but in :class:`~mizani.formatters.date_format` to handle datetime
+  sequences within the same timezone but a mixed daylight saving state.
+  `(plotnine #687) <https://github.com/has2k1/plotnine/issues/687>`_
+
 v0.9.0
 ------
 
 *2023-04-15*
 
 API Changes
 ************
```

### Comparing `mizani-0.9.0/doc/conf.py` & `mizani-0.9.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/installation.rst` & `mizani-0.9.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/layout.html` & `mizani-0.9.1/doc/theme/layout.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/navbar-2.html` & `mizani-0.9.1/doc/theme/navbar-2.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/navbar.html` & `mizani-0.9.1/doc/theme/navbar.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/relations.html` & `mizani-0.9.1/doc/theme/relations.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/search.html` & `mizani-0.9.1/doc/theme/search.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/searchresults.html` & `mizani-0.9.1/doc/theme/searchresults.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css` & `mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js` & `mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/static/bootstrap-sphinx.css_t` & `mizani-0.9.1/doc/theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/static/bootstrap-sphinx.js_t` & `mizani-0.9.1/doc/theme/static/bootstrap-sphinx.js_t`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/static/js/jquery-1.12.4.min.js` & `mizani-0.9.1/doc/theme/static/js/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/doc/theme/theme.conf` & `mizani-0.9.1/doc/theme/theme.conf`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/licences/HUSL_LICENSE` & `mizani-0.9.1/licences/HUSL_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/licences/SEABORN_LICENSE` & `mizani-0.9.1/licences/SEABORN_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/licences/SIX_LICENSE` & `mizani-0.9.1/licences/SIX_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/bounds.py` & `mizani-0.9.1/mizani/bounds.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/breaks.py` & `mizani-0.9.1/mizani/breaks.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/colors/brewer/__init__.py` & `mizani-0.9.1/mizani/colors/brewer/__init__.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/colors/brewer/diverging.py` & `mizani-0.9.1/mizani/colors/brewer/diverging.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/colors/brewer/qualitative.py` & `mizani-0.9.1/mizani/colors/brewer/qualitative.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/colors/brewer/sequential.py` & `mizani-0.9.1/mizani/colors/brewer/sequential.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/colors/color_palette.py` & `mizani-0.9.1/mizani/colors/color_palette.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/external/crayon_rgb.py` & `mizani-0.9.1/mizani/external/crayon_rgb.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/external/husl.py` & `mizani-0.9.1/mizani/external/husl.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/external/xkcd_rgb.py` & `mizani-0.9.1/mizani/external/xkcd_rgb.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/formatters.py` & `mizani-0.9.1/mizani/formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,26 +7,31 @@
 The `*_format` functions below create functions that convert data
 values as understood by a specific scale and return string
 representations of those values. Manipulating the string
 representation of a value helps improve readability of the guide.
 """
 import re
 from bisect import bisect_right
-from warnings import warn
 
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     # python < 3.9
     from backports.zoneinfo import ZoneInfo
 
 import numpy as np
 
 from .breaks import timedelta_helper
-from .utils import match, precision, round_any, same_log10_order_of_magnitude
+from .utils import (
+    get_timezone,
+    match,
+    precision,
+    round_any,
+    same_log10_order_of_magnitude,
+)
 
 __all__ = [
     "comma_format",
     "custom_format",
     "currency_format",
     "dollar_format",
     "percent_format",
@@ -597,24 +602,15 @@
         out : list
             List of strings.
         """
         from matplotlib.dates import date2num
 
         # Formatter timezone
         if self.tz is None and len(x):
-            tz = self.formatter.tz = x[0].tzinfo
-
-            if not all(value.tzinfo == tz for value in x):
-                msg = (
-                    "Dates have different time zones. "
-                    "Choosen `{}` the time zone of the first date. "
-                    "To use a different time zone, create a "
-                    "formatter and pass the time zone."
-                )
-                warn(msg.format(tz.key))
+            self.formatter.tz = get_timezone(x)
 
         # The formatter is tied to axes and takes
         # breaks in ordinal format.
         x = [date2num(val) for val in x]
         return _format(self.formatter, x)
```

### Comparing `mizani-0.9.0/mizani/palettes.py` & `mizani-0.9.1/mizani/palettes.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
     >>> hue_pal()(5)
     ['#db5f57', '#b9db57', '#57db94', '#5784db', '#c957db']
     >>> hue_pal(color_space='husl')(5)
     ['#e0697e', '#9b9054', '#569d79', '#5b98ab', '#b675d7']
     """
     import matplotlib.colors as mcolors
 
-    if not all([0 <= val <= 1 for val in (h, l, s)]):
+    if not all(0 <= val <= 1 for val in (h, l, s)):
         msg = (
             "hue_pal expects values to be between 0 and 1. "
             " I got h={}, l={}, s={}".format(h, l, s)
         )
         raise ValueError(msg)
 
     if color_space not in ("hls", "husl"):
```

### Comparing `mizani-0.9.0/mizani/scale.py` & `mizani-0.9.1/mizani/scale.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/tests/test_bounds.py` & `mizani-0.9.1/mizani/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/tests/test_breaks.py` & `mizani-0.9.1/mizani/tests/test_breaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     breaks = log_breaks()((float("-inf"), float("inf")))
     assert len(breaks) == 0
 
     # When the limits are in the same order of magnitude
     breaks = log_breaks()([35, 60])
     assert len(breaks) > 0
-    assert all([1 < b < 100 for b in breaks])
+    assert all(1 < b < 100 for b in breaks)
 
     breaks = log_breaks()([200, 800])
     npt.assert_array_equal(breaks, [100, 200, 300, 500, 1000])
 
     breaks = log_breaks()((1664, 14008))
     npt.assert_array_equal(breaks, [1000, 3000, 5000, 10000, 30000])
```

### Comparing `mizani-0.9.0/mizani/tests/test_formatters.py` & `mizani-0.9.1/mizani/tests/test_formatters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 import warnings
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, tzinfo
 
 import numpy as np
 import pandas as pd
 import pytest
+import pytz
 
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     # python < 3.9
     from backports.zoneinfo import ZoneInfo
 
@@ -159,14 +160,36 @@
     # Different timezones
     PCT = ZoneInfo("US/Pacific")
     UG = ZoneInfo("Africa/Kampala")
     x = [datetime(2010, 1, 1, tzinfo=UG), datetime(2010, 1, 1, tzinfo=PCT)]
     with pytest.warns(UserWarning, match=r"different time zones"):
         date_format()(x)
 
+    # Timezone with Daylight time
+    NY = ZoneInfo("America/New_York")
+    x = [datetime(2023, 10, 1, tzinfo=NY), datetime(2023, 11, 1, tzinfo=NY)]
+    result = date_format()(x)
+    assert result == ["2023-10-01", "2023-11-01"]
+
+    # Same as above, but different tz library
+    NY = pytz.timezone("America/New_York")
+    x = [datetime(2023, 10, 1, tzinfo=NY), datetime(2023, 11, 1, tzinfo=NY)]
+    result = date_format()(x)
+    assert result == ["2023-10-01", "2023-11-01"]
+
+    # Unknown Timezone
+    class myTzInfo(tzinfo):
+        def __str__(self):
+            return "None"
+
+    TZ = myTzInfo()
+    x = [datetime(2023, 10, 1, tzinfo=TZ), datetime(2023, 11, 1, tzinfo=TZ)]
+    with pytest.raises(ValueError, match=r"^Unrecognised timezone class"):
+        date_format()(x)
+
 
 def test_timedelta_format():
     x = [timedelta(days=7 * i) for i in range(5)]
     labels = timedelta_format()(x)
     assert labels == ["0", "1 week", "2 weeks", "3 weeks", "4 weeks"]
 
     x = [pd.Timedelta(seconds=600 * i) for i in range(5)]
```

### Comparing `mizani-0.9.0/mizani/tests/test_palettes.py` & `mizani-0.9.1/mizani/tests/test_palettes.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/tests/test_scale.py` & `mizani-0.9.1/mizani/tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/tests/test_transforms.py` & `mizani-0.9.1/mizani/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/tests/test_utils.py` & `mizani-0.9.1/mizani/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/transforms.py` & `mizani-0.9.1/mizani/transforms.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/typing.py` & `mizani-0.9.1/mizani/typing.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/mizani/utils.py` & `mizani-0.9.1/mizani/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,39 @@
+from __future__ import annotations
+
+import typing
 from collections import OrderedDict, defaultdict
 from collections.abc import Iterator
 from itertools import chain
+from warnings import warn
+
+try:
+    from zoneinfo import ZoneInfo
+except ImportError:
+    # python < 3.9
+    from backports.zoneinfo import ZoneInfo
 
 import numpy as np
 
+if typing.TYPE_CHECKING:
+    from datetime import datetime
+    from typing import Sequence
+
+
 __all__ = [
     "round_any",
     "min_max",
     "match",
     "precision",
     "first_element",
     "multitype_sort",
     "same_log10_order_of_magnitude",
     "identity",
     "get_categories",
+    "get_timezone",
 ]
 
 DISCRETE_KINDS = "ObUS"
 CONTINUOUS_KINDS = "ifuc"
 
 SECONDS = OrderedDict(
     [
@@ -308,7 +324,50 @@
     elif base == 2:
         res = np.log2(x)
     elif base == np.e:
         res = np.log(x)
     else:
         res = np.log(x) / np.log(base)
     return res
+
+
+def get_timezone(x: Sequence[datetime]) -> ZoneInfo:
+    """
+    Return a single timezone for the sequence of datetimes
+
+    Returns the timezone of first item and warns if any other item
+    has a different timezone
+    """
+
+    from pytz.tzinfo import BaseTzInfo
+
+    # Ref: https://en.wikipedia.org/wiki/List_of_tz_database_time_zones
+
+    info = x[0].tzinfo
+    if info is None:
+        return ZoneInfo("UTC")
+
+    # We recognise two sources of timezone info:
+    #   1. zoneinfo
+    #   2. pytz
+    # These are all subclasses of datetime.tzinfo but they store the
+    # timezone identifier e.g. (Africa/Uganda) in different properties
+    # We assume that all items in the sequence do not mix
+    if isinstance(info, ZoneInfo):
+        prop = "key"
+    elif isinstance(info, BaseTzInfo):
+        prop = "zone"
+    else:
+        raise ValueError(f"Unrecognised timezone class {info.__class__}")
+
+    # Consistency check
+    tz = ZoneInfo(getattr(info, prop))
+    tz_ids = (getattr(value.tzinfo, prop) for value in x)
+    if any(id != tz.key for id in tz_ids):
+        msg = (
+            "Dates in column have different time zones. "
+            "Choosen `{}` the time zone of the first date. "
+            "To use a different time zone, create a "
+            "formatter and pass the time zone."
+        )
+        warn(msg.format(tz.key))
+    return tz
```

### Comparing `mizani-0.9.0/mizani.egg-info/PKG-INFO` & `mizani-0.9.1/mizani.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizani
-Version: 0.9.0
+Version: 0.9.1
 Summary: Scales for Python
 Author-email: Hassan Kibirige <has2k1@gmail.com>
 License: Copyright (c) 2016, Hassan Kibirige
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `mizani-0.9.0/mizani.egg-info/SOURCES.txt` & `mizani-0.9.1/mizani.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 Makefile
 README.md
 codecov.yml
-how-to-release.rst
 pyproject.toml
+.github/workflows/release.yml
 .github/workflows/testing.yml
 doc/Makefile
 doc/bounds.rst
 doc/breaks.rst
 doc/changelog.rst
 doc/conf.py
 doc/docutils.conf
@@ -77,8 +77,9 @@
 mizani/tests/test_breaks.py
 mizani/tests/test_formatters.py
 mizani/tests/test_palettes.py
 mizani/tests/test_scale.py
 mizani/tests/test_transforms.py
 mizani/tests/test_utils.py
 tools/build_theme.sh
-tools/release.sh
+tools/gha_check_semver.py
+tools/release-checklist.md
```

### Comparing `mizani-0.9.0/pyproject.toml` & `mizani-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.0/tools/build_theme.sh` & `mizani-0.9.1/tools/build_theme.sh`

 * *Files identical despite different names*

