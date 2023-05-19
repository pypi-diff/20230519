# Comparing `tmp/metaindex-2.0.0.tar.gz` & `tmp/metaindex-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaindex-2.0.0.tar", last modified: Thu May 11 18:12:32 2023, max compression
+gzip compressed data, was "metaindex-2.1.0.tar", last modified: Thu May 18 15:26:53 2023, max compression
```

## Comparing `metaindex-2.0.0.tar` & `metaindex-2.1.0.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/
--rw-r--r--   0 robert    (1000) robert    (1000)     4488 2023-05-11 18:10:58.000000 metaindex-2.0.0/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-2.0.0/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-2.0.0/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     5107 2023-05-11 18:12:32.776761 metaindex-2.0.0/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     4284 2023-05-11 18:09:52.000000 metaindex-2.0.0/README.md
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.763427 metaindex-2.0.0/doc/
--rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-2.0.0/doc/Makefile
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.763427 metaindex-2.0.0/doc/build/
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.766761 metaindex-2.0.0/doc/build/doctrees/
--rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/addons.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/changelog.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/cmdoptions.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/cmdusage.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/configuration.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/description.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/environment.pickle
--rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/examples.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/extrametadata.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/index.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/indexers.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/install.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/license.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/reference.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/searchsyntax.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/synopsis.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/usage.doctree
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.766761 metaindex-2.0.0/doc/build/html/
--rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/.buildinfo
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.770094 metaindex-2.0.0/doc/build/html/_sources/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.0.0/doc/build/html/_sources/addons.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.0.0/doc/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-2.0.0/doc/build/html/_sources/cmdoptions.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-2.0.0/doc/build/html/_sources/cmdusage.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-2.0.0/doc/build/html/_sources/configuration.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.0.0/doc/build/html/_sources/description.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.0.0/doc/build/html/_sources/examples.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.0.0/doc/build/html/_sources/extrametadata.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.0.0/doc/build/html/_sources/index.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.0.0/doc/build/html/_sources/indexers.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.0.0/doc/build/html/_sources/install.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.0.0/doc/build/html/_sources/license.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.0.0/doc/build/html/_sources/reference.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.0.0/doc/build/html/_sources/searchsyntax.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.0.0/doc/build/html/_sources/synopsis.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.0.0/doc/build/html/_sources/usage.rst.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.770094 metaindex-2.0.0/doc/build/html/_static/
--rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/basic.css
--rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/doctools.js
--rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/documentation_options.js
--rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/file.png
--rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/jquery.js
--rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/language_data.js
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/minus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/nature.css
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/plus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/pygments.css
--rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/searchtools.js
--rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/underscore.js
--rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/addons.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/changelog.html
--rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/cmdusage.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/configuration.html
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/description.html
--rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/examples.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/extrametadata.html
--rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/genindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/index.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/indexers.html
--rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/install.html
--rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/license.html
--rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/objects.inv
--rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/reference.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/search.html
--rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/searchindex.js
--rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/searchsyntax.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/synopsis.html
--rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/usage.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-2.0.0/doc/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-2.0.0/doc/make.bat
--rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-2.0.0/doc/metaindex.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-2.0.0/doc/requirements.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.770094 metaindex-2.0.0/doc/source/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.0.0/doc/source/addons.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.0.0/doc/source/changelog.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     5130 2023-05-11 18:09:52.000000 metaindex-2.0.0/doc/source/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      653 2023-05-11 18:09:52.000000 metaindex-2.0.0/doc/source/cmdusage.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-2.0.0/doc/source/conf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     7739 2023-05-11 18:09:52.000000 metaindex-2.0.0/doc/source/configuration.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.0.0/doc/source/description.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.0.0/doc/source/examples.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.0.0/doc/source/extrametadata.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.0.0/doc/source/index.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.0.0/doc/source/indexers.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.0.0/doc/source/install.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.0.0/doc/source/license.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.0.0/doc/source/reference.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.0.0/doc/source/searchsyntax.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.0.0/doc/source/synopsis.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.0.0/doc/source/usage.rst
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/examples/
--rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-2.0.0/examples/indexing.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/man/
--rw-r--r--   0 robert    (1000) robert    (1000)    34927 2023-05-11 18:12:32.000000 metaindex-2.0.0/man/metaindex.1
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)      247 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)    15817 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)    12235 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/cacheentry.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1968 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/client.py
--rw-r--r--   0 robert    (1000) robert    (1000)    23509 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/configuration.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/metaindex/docs/
--rw-r--r--   0 robert    (1000) robert    (1000)    13555 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex/docs/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)    52404 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex/docs/metaindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     2859 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/find.py
--rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-2.0.0/metaindex/fuse.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-2.0.0/metaindex/humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)    15257 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/indexer.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/metaindex/indexers/
--rw-r--r--   0 robert    (1000) robert    (1000)      472 2022-06-28 21:59:17.000000 metaindex-2.0.0/metaindex/indexers/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1972 2022-08-21 19:12:49.000000 metaindex-2.0.0/metaindex/indexers/abc.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-2.0.0/metaindex/indexers/audio.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4953 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/indexers/collections.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6003 2022-06-27 12:23:21.000000 metaindex-2.0.0/metaindex/indexers/comicbook.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-2.0.0/metaindex/indexers/epub.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3810 2022-04-30 12:58:34.000000 metaindex-2.0.0/metaindex/indexers/filetags.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4354 2022-06-27 12:21:13.000000 metaindex-2.0.0/metaindex/indexers/gpx.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1686 2022-05-04 19:09:52.000000 metaindex-2.0.0/metaindex/indexers/html.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3238 2022-05-29 12:11:11.000000 metaindex-2.0.0/metaindex/indexers/images.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2711 2022-06-28 22:04:20.000000 metaindex-2.0.0/metaindex/indexers/ooxml.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2799 2022-06-28 22:03:27.000000 metaindex-2.0.0/metaindex/indexers/opendocument.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6824 2022-05-11 17:43:40.000000 metaindex-2.0.0/metaindex/indexers/pdf.py
--rw-r--r--   0 robert    (1000) robert    (1000)    10686 2022-03-15 20:14:03.000000 metaindex-2.0.0/metaindex/indexers/ruleindexer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4560 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1566 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/logger.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8767 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3407 2022-05-10 20:51:51.000000 metaindex-2.0.0/metaindex/ocr.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2017 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/opf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8167 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/proto.py
--rw-r--r--   0 robert    (1000) robert    (1000)    25764 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/server.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4214 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/shared.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3198 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/stores.py
--rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-05-11 18:10:04.000000 metaindex-2.0.0/metaindex/version.py
--rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-2.0.0/metaindex/xmlproxy.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3920 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/yaml.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/metaindex.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     5107 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     4390 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       88 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      241 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       29 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/top_level.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/misc/
--rw-r--r--   0 robert    (1000) robert    (1000)     2161 2023-05-11 18:09:52.000000 metaindex-2.0.0/misc/metaindex.conf
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/misc/ranger_metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-2.0.0/misc/ranger_metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)      737 2023-05-11 18:09:16.000000 metaindex-2.0.0/misc/ranger_metaindex/linemode.py
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-05-11 18:12:32.776761 metaindex-2.0.0/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     3667 2023-05-11 18:09:52.000000 metaindex-2.0.0/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     1072 2022-08-21 19:09:08.000000 metaindex-2.0.0/tests/test_abc.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4343 2023-05-11 18:09:52.000000 metaindex-2.0.0/tests/test_cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-2.0.0/tests/test_cacheentry.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-2.0.0/tests/test_cleanup.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-2.0.0/tests/test_collect.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-2.0.0/tests/test_humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-2.0.0/tests/test_indexers.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-2.0.0/tests/test_json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-2.0.0/tests/test_ruleindexer.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.610476 metaindex-2.1.0/
+-rw-r--r--   0 robert    (1000) robert    (1000)     4571 2023-05-18 15:07:33.000000 metaindex-2.1.0/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-2.1.0/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-2.1.0/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     5107 2023-05-18 15:26:53.610476 metaindex-2.1.0/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4284 2023-05-11 18:09:52.000000 metaindex-2.1.0/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.597143 metaindex-2.1.0/doc/
+-rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-2.1.0/doc/Makefile
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.597143 metaindex-2.1.0/doc/build/
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.600476 metaindex-2.1.0/doc/build/doctrees/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/addons.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/changelog.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/cmdoptions.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/cmdusage.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/configuration.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/description.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/doctrees/environment.pickle
+-rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/examples.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/extrametadata.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/index.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/indexers.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/install.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-2.1.0/doc/build/doctrees/license.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/doctrees/reference.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/doctrees/searchsyntax.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/doctrees/synopsis.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/doctrees/usage.doctree
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.603809 metaindex-2.1.0/doc/build/html/
+-rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/.buildinfo
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.603809 metaindex-2.1.0/doc/build/html/_sources/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.1.0/doc/build/html/_sources/addons.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.1.0/doc/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-2.1.0/doc/build/html/_sources/cmdoptions.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-2.1.0/doc/build/html/_sources/cmdusage.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-2.1.0/doc/build/html/_sources/configuration.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.1.0/doc/build/html/_sources/description.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.1.0/doc/build/html/_sources/examples.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.1.0/doc/build/html/_sources/extrametadata.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.1.0/doc/build/html/_sources/index.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.1.0/doc/build/html/_sources/indexers.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.1.0/doc/build/html/_sources/install.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.1.0/doc/build/html/_sources/license.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.1.0/doc/build/html/_sources/reference.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.1.0/doc/build/html/_sources/searchsyntax.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.1.0/doc/build/html/_sources/synopsis.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.1.0/doc/build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.603809 metaindex-2.1.0/doc/build/html/_static/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/_static/basic.css
+-rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-2.1.0/doc/build/html/_static/doctools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/_static/documentation_options.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-2.1.0/doc/build/html/_static/file.png
+-rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-2.1.0/doc/build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-2.1.0/doc/build/html/_static/jquery.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/_static/language_data.js
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.1.0/doc/build/html/_static/minus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/_static/nature.css
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.1.0/doc/build/html/_static/plus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/_static/pygments.css
+-rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-2.1.0/doc/build/html/_static/searchtools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-2.1.0/doc/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-2.1.0/doc/build/html/_static/underscore.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/addons.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/changelog.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/cmdusage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/configuration.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/description.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/examples.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/extrametadata.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/genindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/index.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/indexers.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/install.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/license.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/objects.inv
+-rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/reference.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/search.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/searchindex.js
+-rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/searchsyntax.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/synopsis.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-2.1.0/doc/build/html/usage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-2.1.0/doc/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-2.1.0/doc/make.bat
+-rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-2.1.0/doc/metaindex.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-2.1.0/doc/requirements.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.607143 metaindex-2.1.0/doc/source/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.1.0/doc/source/addons.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.1.0/doc/source/changelog.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     5130 2023-05-11 18:09:52.000000 metaindex-2.1.0/doc/source/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      653 2023-05-11 18:09:52.000000 metaindex-2.1.0/doc/source/cmdusage.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-2.1.0/doc/source/conf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8069 2023-05-18 15:06:36.000000 metaindex-2.1.0/doc/source/configuration.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.1.0/doc/source/description.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.1.0/doc/source/examples.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.1.0/doc/source/extrametadata.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.1.0/doc/source/index.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.1.0/doc/source/indexers.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.1.0/doc/source/install.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.1.0/doc/source/license.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.1.0/doc/source/reference.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.1.0/doc/source/searchsyntax.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.1.0/doc/source/synopsis.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.1.0/doc/source/usage.rst
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.607143 metaindex-2.1.0/examples/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-2.1.0/examples/indexing.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.607143 metaindex-2.1.0/man/
+-rw-r--r--   0 robert    (1000) robert    (1000)    35328 2023-05-18 15:26:53.000000 metaindex-2.1.0/man/metaindex.1
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.607143 metaindex-2.1.0/metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)      274 2023-05-16 17:26:33.000000 metaindex-2.1.0/metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    15817 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    12235 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1968 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/client.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    23595 2023-05-18 15:06:53.000000 metaindex-2.1.0/metaindex/configuration.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.607143 metaindex-2.1.0/metaindex/docs/
+-rw-r--r--   0 robert    (1000) robert    (1000)    13555 2023-05-18 15:26:53.000000 metaindex-2.1.0/metaindex/docs/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    53112 2023-05-18 15:26:53.000000 metaindex-2.1.0/metaindex/docs/metaindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     2859 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/find.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-2.1.0/metaindex/fuse.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-2.1.0/metaindex/humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    15257 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/indexer.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.610476 metaindex-2.1.0/metaindex/indexers/
+-rw-r--r--   0 robert    (1000) robert    (1000)      472 2022-06-28 21:59:17.000000 metaindex-2.1.0/metaindex/indexers/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1972 2022-08-21 19:12:49.000000 metaindex-2.1.0/metaindex/indexers/abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-2.1.0/metaindex/indexers/audio.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4953 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/indexers/collections.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6003 2022-06-27 12:23:21.000000 metaindex-2.1.0/metaindex/indexers/comicbook.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-2.1.0/metaindex/indexers/epub.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3810 2022-04-30 12:58:34.000000 metaindex-2.1.0/metaindex/indexers/filetags.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4354 2022-06-27 12:21:13.000000 metaindex-2.1.0/metaindex/indexers/gpx.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1686 2022-05-04 19:09:52.000000 metaindex-2.1.0/metaindex/indexers/html.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3238 2022-05-29 12:11:11.000000 metaindex-2.1.0/metaindex/indexers/images.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2711 2022-06-28 22:04:20.000000 metaindex-2.1.0/metaindex/indexers/ooxml.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2799 2022-06-28 22:03:27.000000 metaindex-2.1.0/metaindex/indexers/opendocument.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6824 2022-05-11 17:43:40.000000 metaindex-2.1.0/metaindex/indexers/pdf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    10686 2022-03-15 20:14:03.000000 metaindex-2.1.0/metaindex/indexers/ruleindexer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4560 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1566 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/logger.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8767 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3407 2022-05-10 20:51:51.000000 metaindex-2.1.0/metaindex/ocr.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2017 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/opf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8167 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/proto.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    27228 2023-05-18 15:17:05.000000 metaindex-2.1.0/metaindex/server.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4214 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/shared.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3198 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/stores.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-05-18 15:25:34.000000 metaindex-2.1.0/metaindex/version.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-2.1.0/metaindex/xmlproxy.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3920 2023-05-11 18:09:52.000000 metaindex-2.1.0/metaindex/yaml.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.607143 metaindex-2.1.0/metaindex.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     5107 2023-05-18 15:26:53.000000 metaindex-2.1.0/metaindex.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4390 2023-05-18 15:26:53.000000 metaindex-2.1.0/metaindex.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-05-18 15:26:53.000000 metaindex-2.1.0/metaindex.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       88 2023-05-18 15:26:53.000000 metaindex-2.1.0/metaindex.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      241 2023-05-18 15:26:53.000000 metaindex-2.1.0/metaindex.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       29 2023-05-18 15:26:53.000000 metaindex-2.1.0/metaindex.egg-info/top_level.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.610476 metaindex-2.1.0/misc/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2161 2023-05-11 18:09:52.000000 metaindex-2.1.0/misc/metaindex.conf
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.610476 metaindex-2.1.0/misc/ranger_metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-2.1.0/misc/ranger_metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      737 2023-05-11 18:09:16.000000 metaindex-2.1.0/misc/ranger_metaindex/linemode.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-05-18 15:26:53.610476 metaindex-2.1.0/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     3667 2023-05-11 18:09:52.000000 metaindex-2.1.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-18 15:26:53.610476 metaindex-2.1.0/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1072 2022-08-21 19:09:08.000000 metaindex-2.1.0/tests/test_abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4343 2023-05-11 18:09:52.000000 metaindex-2.1.0/tests/test_cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-2.1.0/tests/test_cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-2.1.0/tests/test_cleanup.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-2.1.0/tests/test_collect.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-2.1.0/tests/test_humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-2.1.0/tests/test_indexers.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-2.1.0/tests/test_json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-2.1.0/tests/test_ruleindexer.py
```

### Comparing `metaindex-2.0.0/CHANGELOG.md` & `metaindex-2.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 This file contains the changes made between released versions.
 
 The format is based on [Keep a changelog](https://keepachangelog.com/) and the versioning tries to follow
 [Semantic Versioning](https://semver.org).
 
+## Not released yet
+### Added
+- Configuration option for server, `index-new-tags`
+
 
 ## 2.0.0
 ### Changed
 - Drastic refactoring, back-end changed to xapian
 
 ## 1.5.0
 ### Changed
```

### Comparing `metaindex-2.0.0/LICENSE` & `metaindex-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/PKG-INFO` & `metaindex-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 2.0.0
+Version: 2.1.0
 Summary: Utilities to tag files
 Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `metaindex-2.0.0/README.md` & `metaindex-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/Makefile` & `metaindex-2.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/addons.doctree` & `metaindex-2.1.0/doc/build/doctrees/addons.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/changelog.doctree` & `metaindex-2.1.0/doc/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/cmdoptions.doctree` & `metaindex-2.1.0/doc/build/doctrees/cmdoptions.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/cmdusage.doctree` & `metaindex-2.1.0/doc/build/doctrees/cmdusage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/configuration.doctree` & `metaindex-2.1.0/doc/build/doctrees/configuration.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/description.doctree` & `metaindex-2.1.0/doc/build/doctrees/description.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/environment.pickle` & `metaindex-2.1.0/doc/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/examples.doctree` & `metaindex-2.1.0/doc/build/doctrees/examples.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/extrametadata.doctree` & `metaindex-2.1.0/doc/build/doctrees/extrametadata.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/index.doctree` & `metaindex-2.1.0/doc/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/indexers.doctree` & `metaindex-2.1.0/doc/build/doctrees/indexers.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/install.doctree` & `metaindex-2.1.0/doc/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/license.doctree` & `metaindex-2.1.0/doc/build/doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/reference.doctree` & `metaindex-2.1.0/doc/build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/searchsyntax.doctree` & `metaindex-2.1.0/doc/build/doctrees/searchsyntax.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/synopsis.doctree` & `metaindex-2.1.0/doc/build/doctrees/synopsis.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/doctrees/usage.doctree` & `metaindex-2.1.0/doc/build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/addons.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/addons.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/cmdoptions.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/cmdoptions.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/cmdusage.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/cmdusage.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/configuration.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/configuration.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/description.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/description.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/examples.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/examples.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/extrametadata.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/extrametadata.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/indexers.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/indexers.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/install.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/reference.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/reference.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_sources/searchsyntax.rst.txt` & `metaindex-2.1.0/doc/build/html/_sources/searchsyntax.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/basic.css` & `metaindex-2.1.0/doc/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/doctools.js` & `metaindex-2.1.0/doc/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/jquery-3.5.1.js` & `metaindex-2.1.0/doc/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/jquery.js` & `metaindex-2.1.0/doc/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/language_data.js` & `metaindex-2.1.0/doc/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/nature.css` & `metaindex-2.1.0/doc/build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/pygments.css` & `metaindex-2.1.0/doc/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/searchtools.js` & `metaindex-2.1.0/doc/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/underscore-1.13.1.js` & `metaindex-2.1.0/doc/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/_static/underscore.js` & `metaindex-2.1.0/doc/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/addons.html` & `metaindex-2.1.0/doc/build/html/addons.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/changelog.html` & `metaindex-2.1.0/doc/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/cmdoptions.html` & `metaindex-2.1.0/doc/build/html/cmdoptions.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/cmdusage.html` & `metaindex-2.1.0/doc/build/html/cmdusage.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/configuration.html` & `metaindex-2.1.0/doc/build/html/configuration.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/description.html` & `metaindex-2.1.0/doc/build/html/description.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/examples.html` & `metaindex-2.1.0/doc/build/html/examples.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/extrametadata.html` & `metaindex-2.1.0/doc/build/html/extrametadata.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/genindex.html` & `metaindex-2.1.0/doc/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/index.html` & `metaindex-2.1.0/doc/build/html/index.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/indexers.html` & `metaindex-2.1.0/doc/build/html/indexers.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/install.html` & `metaindex-2.1.0/doc/build/html/install.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/license.html` & `metaindex-2.1.0/doc/build/html/license.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/objects.inv` & `metaindex-2.1.0/doc/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/reference.html` & `metaindex-2.1.0/doc/build/html/reference.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/search.html` & `metaindex-2.1.0/doc/build/html/search.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/searchindex.js` & `metaindex-2.1.0/doc/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/searchsyntax.html` & `metaindex-2.1.0/doc/build/html/searchsyntax.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/synopsis.html` & `metaindex-2.1.0/doc/build/html/synopsis.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/build/html/usage.html` & `metaindex-2.1.0/doc/build/html/usage.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/cmdoptions.rst` & `metaindex-2.1.0/doc/cmdoptions.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/make.bat` & `metaindex-2.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/metaindex.rst` & `metaindex-2.1.0/doc/metaindex.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/addons.rst` & `metaindex-2.1.0/doc/source/addons.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/cmdoptions.rst` & `metaindex-2.1.0/doc/source/cmdoptions.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/cmdusage.rst` & `metaindex-2.1.0/doc/source/cmdusage.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/conf.py` & `metaindex-2.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/configuration.rst` & `metaindex-2.1.0/doc/source/configuration.rst`

 * *Files 4% similar despite different names*

```diff
@@ -130,14 +130,31 @@
     same way as the ``ocr`` option. For example, if you wanted to only do
     fulltext extraction of PDFs and images, you would use ``ocr = .pdf,
     image/``.
 
     The default is ``no``, so no fulltext will be extracted.
 
 
+Server
+~~~~~~
+
+
+  ``index-new-tags``
+    Whether or not the server backend should allow the creation and indexing
+    of tags that are not listed in `Synonyms`_.
+
+    Defaults to ``no``.
+
+  ``autostart``
+    Whether or not to automatically start the server when a client attempts to
+    connect to it.
+
+    Defaults to ``yes``.
+
+
 Synonyms
 ~~~~~~~~
 
 Some metadata fields have less convenient names than others, but might
 semantically be the same. For example, ``Xmp.xmp.CreatorTool`` and
 ``pdf.Creator`` both mean "The program that was used to create this file".
```

### Comparing `metaindex-2.0.0/doc/source/description.rst` & `metaindex-2.1.0/doc/source/description.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/examples.rst` & `metaindex-2.1.0/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/extrametadata.rst` & `metaindex-2.1.0/doc/source/extrametadata.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/indexers.rst` & `metaindex-2.1.0/doc/source/indexers.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/install.rst` & `metaindex-2.1.0/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/reference.rst` & `metaindex-2.1.0/doc/source/reference.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/doc/source/searchsyntax.rst` & `metaindex-2.1.0/doc/source/searchsyntax.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/examples/indexing.py` & `metaindex-2.1.0/examples/indexing.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/man/metaindex.1` & `metaindex-2.1.0/man/metaindex.1`

 * *Files 1% similar despite different names*

```diff
@@ -441,14 +441,33 @@
 fulltext extraction of PDFs and images, you would use \fBocr = .pdf,
 image/\fP\&.
 .sp
 The default is \fBno\fP, so no fulltext will be extracted.
 .UNINDENT
 .UNINDENT
 .UNINDENT
+.SS Server
+.INDENT 0.0
+.INDENT 3.5
+.INDENT 0.0
+.TP
+.B \fBindex\-new\-tags\fP
+Whether or not the server backend should allow the creation and indexing
+of tags that are not listed in \fI\%Synonyms\fP\&.
+.sp
+Defaults to \fBno\fP\&.
+.TP
+.B \fBautostart\fP
+Whether or not to automatically start the server when a client attempts to
+connect to it.
+.sp
+Defaults to \fByes\fP\&.
+.UNINDENT
+.UNINDENT
+.UNINDENT
 .SS Synonyms
 .sp
 Some metadata fields have less convenient names than others, but might
 semantically be the same. For example, \fBXmp.xmp.CreatorTool\fP and
 \fBpdf.Creator\fP both mean \(dqThe program that was used to create this file\(dq.
 .sp
 To simplify the search it is possible to define synonyms for these metadata fields.
```

### Comparing `metaindex-2.0.0/metaindex/cache.py` & `metaindex-2.1.0/metaindex/cache.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/cacheentry.py` & `metaindex-2.1.0/metaindex/cacheentry.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/client.py` & `metaindex-2.1.0/metaindex/client.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/configuration.py` & `metaindex-2.1.0/metaindex/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 CONFIG_OCR = 'ocr'
 CONFIG_FULLTEXT = 'fulltext'
 CONFIG_MIMETYPES = 'mimetypes'
 CONFIG_IMPLICIT_TAGS = 'implicit-tags'
 CONFIG_LOGFILE = 'logfile'
 CONFIG_LOGLEVEL = 'loglevel'
 CONFIG_AUTOSTART = 'autostart'
+CONFIG_DYNAMIC_TAGS = 'index-new-tags'
 
 CONF_DEFAULTS = {SECTION_GENERAL: {
                     CONFIG_CACHE: str(CACHEPATH),
                     CONFIG_SOCKET: str(SOCKETPATH),
                     CONFIG_RECURSIVE_EXTRA_METADATA: "yes",
                     CONFIG_COLLECTION_METADATA: ".metadata, metadata",
                     CONFIG_IGNORE_DIRS: "\n".join(IGNORE_DIRS),
@@ -175,14 +176,15 @@
                     CONFIG_FULLTEXT: 'no',
                     CONFIG_IMPLICIT_TAGS: ', '.join(IMPLICIT_TAGS),
                  },
                  SECTION_SERVER: {
                     CONFIG_LOGFILE: str(LOGFILEPATH),
                     CONFIG_LOGLEVEL: str(LOGLEVEL),
                     CONFIG_AUTOSTART: 'yes',
+                    CONFIG_DYNAMIC_TAGS: 'no',
                  },
                  SECTION_SYNONYMS: {k: ', '.join(v)
                                     for k, v in SYNONYMS.items()},
                  SECTION_INCLUDE: {
                  },
                 }
```

### Comparing `metaindex-2.0.0/metaindex/docs/cmdoptions.html` & `metaindex-2.1.0/metaindex/docs/cmdoptions.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/docs/metaindex.html` & `metaindex-2.1.0/metaindex/docs/metaindex.html`

 * *Files 1% similar despite different names*

#### Comparing `metaindex-2.0.0/metaindex/docs/metaindex.html` & `metaindex-2.1.0/metaindex/docs/metaindex.html`

```diff
@@ -1071,14 +1071,51 @@
                     <tt class="docutils literal">no</tt>
                     , so no fulltext will be extracted.
                   </p>
                 </dd>
               </dl>
             </blockquote>
           </div>
+          <div class="section" id="server-1">
+            <h3>Server</h3>
+            <blockquote>
+              <dl class="docutils">
+                <dt>
+                  <tt class="docutils literal">
+                    <span class="pre">index-new-tags</span>
+                  </tt>
+                </dt>
+                <dd>
+                  <p class="first">
+                    Whether or not the server backend should allow the creation and indexing
+of tags that are not listed in
+                    <a class="reference internal" href="#synonyms">Synonyms</a>
+                    .
+                  </p>
+                  <p class="last">
+                    Defaults to
+                    <tt class="docutils literal">no</tt>
+                    .
+                  </p>
+                </dd>
+                <dt>
+                  <tt class="docutils literal">autostart</tt>
+                </dt>
+                <dd>
+                  <p class="first">Whether or not to automatically start the server when a client attempts to
+connect to it.</p>
+                  <p class="last">
+                    Defaults to
+                    <tt class="docutils literal">yes</tt>
+                    .
+                  </p>
+                </dd>
+              </dl>
+            </blockquote>
+          </div>
           <div class="section" id="synonyms">
             <h3>Synonyms</h3>
             <p>
               Some metadata fields have less convenient names than others, but might
 semantically be the same. For example,
               <tt class="docutils literal">Xmp.xmp.CreatorTool</tt>
               and
```

### Comparing `metaindex-2.0.0/metaindex/find.py` & `metaindex-2.1.0/metaindex/find.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/fuse.py` & `metaindex-2.1.0/metaindex/fuse.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/humanizer.py` & `metaindex-2.1.0/metaindex/humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexer.py` & `metaindex-2.1.0/metaindex/indexer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/abc.py` & `metaindex-2.1.0/metaindex/indexers/abc.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/audio.py` & `metaindex-2.1.0/metaindex/indexers/audio.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/collections.py` & `metaindex-2.1.0/metaindex/indexers/collections.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/comicbook.py` & `metaindex-2.1.0/metaindex/indexers/comicbook.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/epub.py` & `metaindex-2.1.0/metaindex/indexers/epub.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/filetags.py` & `metaindex-2.1.0/metaindex/indexers/filetags.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/gpx.py` & `metaindex-2.1.0/metaindex/indexers/gpx.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/html.py` & `metaindex-2.1.0/metaindex/indexers/html.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/images.py` & `metaindex-2.1.0/metaindex/indexers/images.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/ooxml.py` & `metaindex-2.1.0/metaindex/indexers/ooxml.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/opendocument.py` & `metaindex-2.1.0/metaindex/indexers/opendocument.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/pdf.py` & `metaindex-2.1.0/metaindex/indexers/pdf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/indexers/ruleindexer.py` & `metaindex-2.1.0/metaindex/indexers/ruleindexer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/json.py` & `metaindex-2.1.0/metaindex/json.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/logger.py` & `metaindex-2.1.0/metaindex/logger.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/main.py` & `metaindex-2.1.0/metaindex/main.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/ocr.py` & `metaindex-2.1.0/metaindex/ocr.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/opf.py` & `metaindex-2.1.0/metaindex/opf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/proto.py` & `metaindex-2.1.0/metaindex/proto.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/server.py` & `metaindex-2.1.0/metaindex/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,16 @@
         self.send(proto.OkayResponse())
 
 
 class Server(socketserver.ThreadingMixIn, socketserver.UnixStreamServer):
     def __init__(self, manager):
         socketpath = manager.config.path(configuration.SECTION_GENERAL,
                                          configuration.CONFIG_SOCKET)
+        if socketpath.is_socket():
+            socketpath.unlink()
         super().__init__(str(socketpath), ConnectionHandler)
         self.path = socketpath
         self.manager = manager
         self.manager.server_process = self
 
     def cleanup(self):
         try:
@@ -131,21 +133,25 @@
         self._qparser = None
 
         self.server_process = None
 
         # xapian prefixes are upper-case strings consisting only of letters
         # and starting with X for user-defined prefixes
         # the mapping of human-readable to xapian prefixes is here:
-        self.prefixpath = configuration.CACHEPATH / "prefixes.csv"
+        self.prefixpath = self.dbpath.parent / "prefixes.csv"
         self.human_to_prefix = {}
         self.prefix_to_human = {}
         # indexers produce their own tags (e.g. 'epub.writer'), but for
         # indexing they need to map to one of the base-level tags (e.g. 'author')
         self.tag_mapping = {}
 
+        self.create_tags_dynamically = self.config.bool(configuration.SECTION_SERVER,
+                                                        configuration.CONFIG_DYNAMIC_TAGS,
+                                                        "no")
+
         self.load_prefix_translations()
         self.load_tag_mapping()
 
         self.requests = queue.Queue(20)
         self.thread = None
 
         self.stemmers = {lang: xapian.Stem(lang)
@@ -157,26 +163,42 @@
 
         for tag in self.config[configuration.SECTION_SYNONYMS]:
             self.tag_mapping.update({s: tag
                                      for s in self.config.list(configuration.SECTION_SYNONYMS,
                                                                tag)})
 
         for tag in self.config[configuration.SECTION_SYNONYMS]:
-            if tag in self.human_to_prefix or tag in BASE_TAGS:
+            prefix, is_new = self.add_tag(tag)
+            if not is_new:
                 continue
-            prefix = next_prefix(self.prefix_to_human.keys())
-
-            self.human_to_prefix[tag] = prefix
-            self.prefix_to_human[prefix] = tag
             logger.debug("Added %s -> %s mapping", tag, prefix)
             updated = True
 
         if updated:
             self.save_prefix_translations()
 
+    def add_tag(self, tag):
+        """Ensure this tag is in the translation tables and return the prefix and whether it is new
+
+        Returns a tuple ``(prefix, is_new)`` with ``is_new`` indicating whether the prefix has just
+        been created newly.
+        """
+        if tag in self.human_to_prefix:
+            return self.human_to_prefix[tag], False
+        if tag in BASE_TAGS:
+            return BASE_TAGS[tag], False
+
+        prefix = next_prefix(self.prefix_to_human.keys())
+        self.human_to_prefix[tag] = prefix
+        self.prefix_to_human[prefix] = tag
+
+        self._qparser = None
+
+        return prefix, True
+
     def load_prefix_translations(self):
         """Load the translations of tag->xapian prefix from disk"""
         if not self.prefixpath.is_file():
             return
 
         with open(self.prefixpath, 'rt', newline='', encoding='utf-8') as prefixfile:
             reader = csv.reader(prefixfile)
@@ -307,14 +329,16 @@
         Returns 'True' on success, otherwise 'False'
         """
         db_exists = self.ensure_connection()
 
         dbconn = xapian.WritableDatabase(str(self.dbpath))
         indexer = xapian.TermGenerator()
 
+        updated_prefix_table = False
+
         dbconn.begin_transaction()
         for entry in entries:
             # build a unique identifier for the given entry
             strpath = str(entry.path)
             pathid = self.unique(entry.path)
 
             # attempt to find the document to see if it needs to be replaced instead of added
@@ -349,15 +373,19 @@
             # all indexable keys, their prefix, and whether any humanizable values exist
             for key, values in entry.metadata.items():
                 key = self.config.synonymized.get(key, key)
                 key = self.tag_mapping.get(key, key)
                 prefix = BASE_TAGS.get(key, self.human_to_prefix.get(key, None))
 
                 if prefix is None:
-                    continue
+                    if not self.create_tags_dynamically:
+                        continue
+                    prefix, is_new = self.add_tag(key)
+                    if is_new:
+                        updated_prefix_table = True
 
                 if key not in keys:
                     keys[key] = (prefix, [])
                 keys[key][1].extend(values)
 
             # first index the raw values, but already collect humanized values
             humanized = []
@@ -416,14 +444,21 @@
             if docid is None:
                 dbconn.add_document(doc)
             else:
                 dbconn.replace_document(docid, doc)
 
         dbconn.commit_transaction()
         dbconn.close()
+
+        if updated_prefix_table:
+            try:
+                self.save_prefix_translations()
+            except OSError as exc:
+                logger.error(f"Failed to save prefix table: {exc}")
+
         return True
 
     def clear(self):
         """Clear the databasee"""
         if not self.ensure_connection():
             raise RuntimeError("Could not connect to database")
         logger.info("Flushing database")
@@ -690,15 +725,22 @@
     client.recv()
 
 
 def launch(config):
     manager = Manager(config)
     manager.start()
 
-    with Server(manager) as server:
+    try:
+        server = Server(manager)
+    except OSError as exc:
+        logger.error(f"Could not start server: {exc}")
+        manager.stop()
+        return
+
+    with server:
         try:
             server.serve_forever()
         except (KeyboardInterrupt, EOFError):
             pass
 
     manager.stop()
     manager.save_prefix_translations()
@@ -735,15 +777,18 @@
     launch(config)
 
 
 def run():
     args = parse_args()
 
     config = configuration.load(args.config)
-    if not args.stop and is_server_running(config):
+    another_server = False
+    if not args.stop:
+        another_server = is_server_running(config)
+    if not args.stop and another_server:
         logger.info("Another server is already running")
         return 1
 
     loglevel = args.log_level or config.get(configuration.SECTION_SERVER, configuration.CONFIG_LOGLEVEL)
     logfile = args.log_file or config.get(configuration.SECTION_SERVER, configuration.CONFIG_LOGFILE)
 
     logger.setup(level=loglevel.upper(), filename=logfile)
```

### Comparing `metaindex-2.0.0/metaindex/shared.py` & `metaindex-2.1.0/metaindex/shared.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/stores.py` & `metaindex-2.1.0/metaindex/stores.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/xmlproxy.py` & `metaindex-2.1.0/metaindex/xmlproxy.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex/yaml.py` & `metaindex-2.1.0/metaindex/yaml.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/metaindex.egg-info/PKG-INFO` & `metaindex-2.1.0/metaindex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 2.0.0
+Version: 2.1.0
 Summary: Utilities to tag files
 Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `metaindex-2.0.0/metaindex.egg-info/SOURCES.txt` & `metaindex-2.1.0/metaindex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/misc/metaindex.conf` & `metaindex-2.1.0/misc/metaindex.conf`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/misc/ranger_metaindex/linemode.py` & `metaindex-2.1.0/misc/ranger_metaindex/linemode.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/setup.py` & `metaindex-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/tests/test_abc.py` & `metaindex-2.1.0/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/tests/test_cache.py` & `metaindex-2.1.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/tests/test_cacheentry.py` & `metaindex-2.1.0/tests/test_cacheentry.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/tests/test_cleanup.py` & `metaindex-2.1.0/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/tests/test_collect.py` & `metaindex-2.1.0/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/tests/test_humanizer.py` & `metaindex-2.1.0/tests/test_humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/tests/test_indexers.py` & `metaindex-2.1.0/tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/tests/test_json.py` & `metaindex-2.1.0/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.0.0/tests/test_ruleindexer.py` & `metaindex-2.1.0/tests/test_ruleindexer.py`

 * *Files identical despite different names*

