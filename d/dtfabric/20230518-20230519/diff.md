# Comparing `tmp/dtfabric-20230518.tar.gz` & `tmp/dtfabric-20230519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfabric-20230518.tar", last modified: Thu May 18 16:25:30 2023, max compression
+gzip compressed data, was "dtfabric-20230519.tar", last modified: Fri May 19 02:58:48 2023, max compression
```

## Comparing `dtfabric-20230518.tar` & `dtfabric-20230519.tar`

### file list

```diff
@@ -1,133 +1,132 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.548572 dtfabric-20230518/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.209572 dtfabric-20230518/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.310572 dtfabric-20230518/.github/workflows/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2541 2023-05-12 04:16:07.000000 dtfabric-20230518/.github/workflows/test_docker.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-05-12 04:16:07.000000 dtfabric-20230518/.github/workflows/test_docs.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4107 2023-05-12 04:16:07.000000 dtfabric-20230518/.github/workflows/test_tox.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    22994 2023-05-12 04:16:07.000000 dtfabric-20230518/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-07-10 04:44:41.000000 dtfabric-20230518/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2022-01-24 07:36:34.000000 dtfabric-20230518/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      265 2018-07-03 18:38:13.000000 dtfabric-20230518/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-09-25 06:41:25.000000 dtfabric-20230518/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      592 2021-08-22 05:30:09.000000 dtfabric-20230518/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-18 16:25:30.548572 dtfabric-20230518/PKG-INFO
--rw-r-----   0 lordyesta  (1000) lordyesta  (1000)      195 2020-06-21 05:38:03.000000 dtfabric-20230518/README
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-12 04:16:07.000000 dtfabric-20230518/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.210572 dtfabric-20230518/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.312572 dtfabric-20230518/config/appveyor/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      839 2023-05-12 04:16:07.000000 dtfabric-20230518/config/appveyor/install.ps1
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-12 04:16:07.000000 dtfabric-20230518/config/appveyor/install.sh
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-12 04:16:07.000000 dtfabric-20230518/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.364572 dtfabric-20230518/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-05-18 11:05:37.000000 dtfabric-20230518/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       38 2017-05-26 07:25:10.000000 dtfabric-20230518/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-12 04:16:07.000000 dtfabric-20230518/config/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      786 2023-05-12 04:16:07.000000 dtfabric-20230518/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2017-04-14 13:14:48.000000 dtfabric-20230518/config/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       20 2017-04-14 13:31:35.000000 dtfabric-20230518/config/dpkg/dtfabric-data.dirs
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       26 2017-04-14 13:32:40.000000 dtfabric-20230518/config/dpkg/dtfabric-data.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:20.000000 dtfabric-20230518/config/dpkg/python-dtfabric.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:27.000000 dtfabric-20230518/config/dpkg/python3-dtfabric.install
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-12 04:16:07.000000 dtfabric-20230518/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.378572 dtfabric-20230518/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-04-14 13:14:48.000000 dtfabric-20230518/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.379572 dtfabric-20230518/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      362 2020-06-21 09:14:13.000000 dtfabric-20230518/config/pylint/spelling-private-dict
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2020-01-19 18:45:05.000000 dtfabric-20230518/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.397572 dtfabric-20230518/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2023-05-12 04:16:07.000000 dtfabric-20230518/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2021-07-30 06:46:25.000000 dtfabric-20230518/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-05-12 04:16:16.000000 dtfabric-20230518/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.408572 dtfabric-20230518/docs/sources/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15554 2022-07-10 05:53:49.000000 dtfabric-20230518/docs/sources/Format-specification.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.447572 dtfabric-20230518/docs/sources/api/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2022-02-19 13:55:33.000000 dtfabric-20230518/docs/sources/api/dtfabric.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      869 2021-07-30 06:46:25.000000 dtfabric-20230518/docs/sources/api/dtfabric.runtime.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       61 2021-07-30 06:37:51.000000 dtfabric-20230518/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.454572 dtfabric-20230518/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2021-12-28 03:59:54.000000 dtfabric-20230518/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      288 2021-07-30 06:37:51.000000 dtfabric-20230518/docs/sources/user/index.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.473572 dtfabric-20230518/dtfabric/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       74 2023-05-18 11:04:17.000000 dtfabric-20230518/dtfabric/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31346 2023-05-14 14:27:49.000000 dtfabric-20230518/dtfabric/data_types.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-09-18 09:38:10.000000 dtfabric-20230518/dtfabric/decorators.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2021-07-30 10:44:15.000000 dtfabric-20230518/dtfabric/definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1016 2021-07-30 06:46:25.000000 dtfabric-20230518/dtfabric/errors.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    52825 2023-05-18 03:12:53.000000 dtfabric-20230518/dtfabric/reader.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3192 2022-09-18 09:35:13.000000 dtfabric-20230518/dtfabric/registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.512572 dtfabric-20230518/dtfabric/runtime/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230518/dtfabric/runtime/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2523 2022-09-18 09:36:04.000000 dtfabric-20230518/dtfabric/runtime/byte_operations.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76230 2023-05-18 16:17:58.000000 dtfabric-20230518/dtfabric/runtime/data_maps.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2022-01-27 14:27:48.000000 dtfabric-20230518/dtfabric/runtime/fabric.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6233 2022-09-18 09:46:53.000000 dtfabric-20230518/dtfabric/runtime/runtime.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.483572 dtfabric-20230518/dtfabric.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-18 16:25:28.000000 dtfabric-20230518/dtfabric.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2877 2023-05-18 16:25:29.000000 dtfabric-20230518/dtfabric.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-18 16:25:28.000000 dtfabric-20230518/dtfabric.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-05-18 16:25:28.000000 dtfabric-20230518/dtfabric.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        9 2023-05-18 16:25:28.000000 dtfabric-20230518/dtfabric.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      395 2019-02-03 12:58:57.000000 dtfabric-20230518/dtfabric.ini
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-05-12 04:16:07.000000 dtfabric-20230518/requirements.txt
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      777 2022-09-18 09:32:38.000000 dtfabric-20230518/run_tests.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.534572 dtfabric-20230518/scripts/
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3218 2022-09-18 08:56:58.000000 dtfabric-20230518/scripts/validate-definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      302 2023-05-18 16:25:30.549572 dtfabric-20230518/setup.cfg
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     6782 2023-05-12 04:16:07.000000 dtfabric-20230518/setup.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.543572 dtfabric-20230518/test_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12288 2023-05-18 15:47:17.000000 dtfabric-20230518/test_data/.structure_with_string.yaml.swp
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2017-05-01 13:58:49.000000 dtfabric-20230518/test_data/Notepad.lnk
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2022-07-10 05:55:10.000000 dtfabric-20230518/test_data/boolean.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      101 2022-07-10 05:55:12.000000 dtfabric-20230518/test_data/character.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      284 2022-07-10 05:55:13.000000 dtfabric-20230518/test_data/constant.yaml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.544572 dtfabric-20230518/test_data/definitions/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      524 2022-07-10 05:54:56.000000 dtfabric-20230518/test_data/definitions/booleans.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      453 2022-07-10 05:54:58.000000 dtfabric-20230518/test_data/definitions/characters.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      405 2022-07-10 05:55:00.000000 dtfabric-20230518/test_data/definitions/floating-points.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2022-07-10 05:55:01.000000 dtfabric-20230518/test_data/definitions/integers.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-07-10 05:55:15.000000 dtfabric-20230518/test_data/enumeration.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-07-10 05:55:16.000000 dtfabric-20230518/test_data/floating-point.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-07-10 05:55:18.000000 dtfabric-20230518/test_data/format.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2022-07-10 05:55:19.000000 dtfabric-20230518/test_data/integer.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       83 2022-07-10 05:55:23.000000 dtfabric-20230518/test_data/padding.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      457 2022-07-10 05:55:28.000000 dtfabric-20230518/test_data/sequence.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      572 2022-07-10 05:55:25.000000 dtfabric-20230518/test_data/sequence_with_context.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      433 2023-05-18 05:56:24.000000 dtfabric-20230518/test_data/sequence_with_structure.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      657 2022-07-10 05:55:29.000000 dtfabric-20230518/test_data/stream.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      707 2022-07-10 05:55:32.000000 dtfabric-20230518/test_data/string.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      818 2022-07-10 05:55:30.000000 dtfabric-20230518/test_data/string_array.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1059 2022-07-10 05:55:50.000000 dtfabric-20230518/test_data/structure.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2022-07-10 05:55:34.000000 dtfabric-20230518/test_data/structure_family.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1576 2022-07-10 05:55:35.000000 dtfabric-20230518/test_data/structure_group.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      651 2022-07-10 05:55:36.000000 dtfabric-20230518/test_data/structure_with_condition.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      496 2022-07-10 05:55:38.000000 dtfabric-20230518/test_data/structure_with_context.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      712 2022-07-10 05:57:13.000000 dtfabric-20230518/test_data/structure_with_padding.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      322 2022-07-10 05:55:41.000000 dtfabric-20230518/test_data/structure_with_section.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      468 2022-07-10 05:55:43.000000 dtfabric-20230518/test_data/structure_with_sequence.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      466 2022-07-10 05:55:44.000000 dtfabric-20230518/test_data/structure_with_stream.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      446 2022-07-10 05:55:45.000000 dtfabric-20230518/test_data/structure_with_string.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      370 2022-07-10 05:55:47.000000 dtfabric-20230518/test_data/structure_with_union.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      700 2022-07-10 05:55:49.000000 dtfabric-20230518/test_data/structure_with_values.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      383 2022-07-10 05:55:53.000000 dtfabric-20230518/test_data/union.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      380 2022-07-10 05:55:51.000000 dtfabric-20230518/test_data/union_with_condition.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      200 2022-07-10 05:55:54.000000 dtfabric-20230518/test_data/uuid.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      107 2022-12-18 07:46:44.000000 dtfabric-20230518/test_dependencies.ini
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       14 2023-05-12 04:16:07.000000 dtfabric-20230518/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.545572 dtfabric-20230518/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230518/tests/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19685 2022-02-13 10:09:16.000000 dtfabric-20230518/tests/data_types.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    62234 2023-05-18 03:22:07.000000 dtfabric-20230518/tests/reader.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2021-07-30 06:46:25.000000 dtfabric-20230518/tests/registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.547572 dtfabric-20230518/tests/runtime/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230518/tests/runtime/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2021-07-30 09:04:50.000000 dtfabric-20230518/tests/runtime/byte_operations.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84696 2023-05-18 15:50:47.000000 dtfabric-20230518/tests/runtime/data_maps.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      662 2021-07-30 06:46:25.000000 dtfabric-20230518/tests/runtime/fabric.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2494 2021-07-30 06:46:25.000000 dtfabric-20230518/tests/runtime/runtime.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2022-09-18 09:32:59.000000 dtfabric-20230518/tests/test_lib.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2023-05-12 04:16:07.000000 dtfabric-20230518/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.548572 dtfabric-20230518/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       70 2018-03-18 06:58:04.000000 dtfabric-20230518/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-12 04:16:07.000000 dtfabric-20230518/utils/check_dependencies.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-12 04:16:07.000000 dtfabric-20230518/utils/dependencies.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      616 2021-12-28 04:01:20.000000 dtfabric-20230518/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.302414 dtfabric-20230519/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:47.998414 dtfabric-20230519/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.076414 dtfabric-20230519/.github/workflows/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2541 2023-05-12 04:16:07.000000 dtfabric-20230519/.github/workflows/test_docker.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-05-12 04:16:07.000000 dtfabric-20230519/.github/workflows/test_docs.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4107 2023-05-12 04:16:07.000000 dtfabric-20230519/.github/workflows/test_tox.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    22994 2023-05-12 04:16:07.000000 dtfabric-20230519/.pylintrc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-07-10 04:44:41.000000 dtfabric-20230519/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2022-01-24 07:36:34.000000 dtfabric-20230519/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      265 2018-07-03 18:38:13.000000 dtfabric-20230519/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-09-25 06:41:25.000000 dtfabric-20230519/LICENSE
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      592 2021-08-22 05:30:09.000000 dtfabric-20230519/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-19 02:58:48.302414 dtfabric-20230519/PKG-INFO
+-rw-r-----   0 lordyesta  (1000) lordyesta  (1000)      195 2020-06-21 05:38:03.000000 dtfabric-20230519/README
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-12 04:16:07.000000 dtfabric-20230519/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:47.998414 dtfabric-20230519/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.078414 dtfabric-20230519/config/appveyor/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      839 2023-05-12 04:16:07.000000 dtfabric-20230519/config/appveyor/install.ps1
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-12 04:16:07.000000 dtfabric-20230519/config/appveyor/install.sh
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-12 04:16:07.000000 dtfabric-20230519/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.138414 dtfabric-20230519/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-05-19 02:56:42.000000 dtfabric-20230519/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       38 2017-05-26 07:25:10.000000 dtfabric-20230519/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-12 04:16:07.000000 dtfabric-20230519/config/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      786 2023-05-12 04:16:07.000000 dtfabric-20230519/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2017-04-14 13:14:48.000000 dtfabric-20230519/config/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       20 2017-04-14 13:31:35.000000 dtfabric-20230519/config/dpkg/dtfabric-data.dirs
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       26 2017-04-14 13:32:40.000000 dtfabric-20230519/config/dpkg/dtfabric-data.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:20.000000 dtfabric-20230519/config/dpkg/python-dtfabric.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:27.000000 dtfabric-20230519/config/dpkg/python3-dtfabric.install
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-12 04:16:07.000000 dtfabric-20230519/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.138414 dtfabric-20230519/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-04-14 13:14:48.000000 dtfabric-20230519/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.139414 dtfabric-20230519/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      362 2020-06-21 09:14:13.000000 dtfabric-20230519/config/pylint/spelling-private-dict
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2020-01-19 18:45:05.000000 dtfabric-20230519/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.155414 dtfabric-20230519/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2023-05-12 04:16:07.000000 dtfabric-20230519/docs/conf.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2021-07-30 06:46:25.000000 dtfabric-20230519/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-05-12 04:16:16.000000 dtfabric-20230519/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.155414 dtfabric-20230519/docs/sources/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15554 2022-07-10 05:53:49.000000 dtfabric-20230519/docs/sources/Format-specification.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.156414 dtfabric-20230519/docs/sources/api/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2022-02-19 13:55:33.000000 dtfabric-20230519/docs/sources/api/dtfabric.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      869 2021-07-30 06:46:25.000000 dtfabric-20230519/docs/sources/api/dtfabric.runtime.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       61 2021-07-30 06:37:51.000000 dtfabric-20230519/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.156414 dtfabric-20230519/docs/sources/user/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2021-12-28 03:59:54.000000 dtfabric-20230519/docs/sources/user/Installation-instructions.md
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      288 2021-07-30 06:37:51.000000 dtfabric-20230519/docs/sources/user/index.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.158414 dtfabric-20230519/dtfabric/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       74 2023-05-19 02:56:42.000000 dtfabric-20230519/dtfabric/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31346 2023-05-14 14:27:49.000000 dtfabric-20230519/dtfabric/data_types.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-09-18 09:38:10.000000 dtfabric-20230519/dtfabric/decorators.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2021-07-30 10:44:15.000000 dtfabric-20230519/dtfabric/definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1016 2021-07-30 06:46:25.000000 dtfabric-20230519/dtfabric/errors.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    52825 2023-05-18 03:12:53.000000 dtfabric-20230519/dtfabric/reader.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3192 2022-09-18 09:35:13.000000 dtfabric-20230519/dtfabric/registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.161414 dtfabric-20230519/dtfabric/runtime/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230519/dtfabric/runtime/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2523 2022-09-18 09:36:04.000000 dtfabric-20230519/dtfabric/runtime/byte_operations.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76538 2023-05-18 17:48:42.000000 dtfabric-20230519/dtfabric/runtime/data_maps.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2022-01-27 14:27:48.000000 dtfabric-20230519/dtfabric/runtime/fabric.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6233 2022-09-18 09:46:53.000000 dtfabric-20230519/dtfabric/runtime/runtime.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.160414 dtfabric-20230519/dtfabric.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-19 02:58:46.000000 dtfabric-20230519/dtfabric.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2835 2023-05-19 02:58:47.000000 dtfabric-20230519/dtfabric.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-19 02:58:46.000000 dtfabric-20230519/dtfabric.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-05-19 02:58:46.000000 dtfabric-20230519/dtfabric.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        9 2023-05-19 02:58:46.000000 dtfabric-20230519/dtfabric.egg-info/top_level.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      395 2019-02-03 12:58:57.000000 dtfabric-20230519/dtfabric.ini
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-05-12 04:16:07.000000 dtfabric-20230519/requirements.txt
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      777 2022-09-18 09:32:38.000000 dtfabric-20230519/run_tests.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.161414 dtfabric-20230519/scripts/
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3218 2022-09-18 08:56:58.000000 dtfabric-20230519/scripts/validate-definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      302 2023-05-19 02:58:48.303414 dtfabric-20230519/setup.cfg
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     6782 2023-05-12 04:16:07.000000 dtfabric-20230519/setup.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.187414 dtfabric-20230519/test_data/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2017-05-01 13:58:49.000000 dtfabric-20230519/test_data/Notepad.lnk
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2022-07-10 05:55:10.000000 dtfabric-20230519/test_data/boolean.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      101 2022-07-10 05:55:12.000000 dtfabric-20230519/test_data/character.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      284 2022-07-10 05:55:13.000000 dtfabric-20230519/test_data/constant.yaml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.188414 dtfabric-20230519/test_data/definitions/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      524 2022-07-10 05:54:56.000000 dtfabric-20230519/test_data/definitions/booleans.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      453 2022-07-10 05:54:58.000000 dtfabric-20230519/test_data/definitions/characters.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      405 2022-07-10 05:55:00.000000 dtfabric-20230519/test_data/definitions/floating-points.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2022-07-10 05:55:01.000000 dtfabric-20230519/test_data/definitions/integers.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-07-10 05:55:15.000000 dtfabric-20230519/test_data/enumeration.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-07-10 05:55:16.000000 dtfabric-20230519/test_data/floating-point.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-07-10 05:55:18.000000 dtfabric-20230519/test_data/format.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2022-07-10 05:55:19.000000 dtfabric-20230519/test_data/integer.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       83 2022-07-10 05:55:23.000000 dtfabric-20230519/test_data/padding.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      457 2022-07-10 05:55:28.000000 dtfabric-20230519/test_data/sequence.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      572 2022-07-10 05:55:25.000000 dtfabric-20230519/test_data/sequence_with_context.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      433 2023-05-18 05:56:24.000000 dtfabric-20230519/test_data/sequence_with_structure.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      657 2022-07-10 05:55:29.000000 dtfabric-20230519/test_data/stream.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      707 2022-07-10 05:55:32.000000 dtfabric-20230519/test_data/string.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      818 2022-07-10 05:55:30.000000 dtfabric-20230519/test_data/string_array.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1059 2022-07-10 05:55:50.000000 dtfabric-20230519/test_data/structure.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2022-07-10 05:55:34.000000 dtfabric-20230519/test_data/structure_family.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1576 2022-07-10 05:55:35.000000 dtfabric-20230519/test_data/structure_group.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      651 2022-07-10 05:55:36.000000 dtfabric-20230519/test_data/structure_with_condition.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      496 2022-07-10 05:55:38.000000 dtfabric-20230519/test_data/structure_with_context.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      712 2022-07-10 05:57:13.000000 dtfabric-20230519/test_data/structure_with_padding.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      322 2022-07-10 05:55:41.000000 dtfabric-20230519/test_data/structure_with_section.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      468 2022-07-10 05:55:43.000000 dtfabric-20230519/test_data/structure_with_sequence.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      466 2022-07-10 05:55:44.000000 dtfabric-20230519/test_data/structure_with_stream.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      446 2022-07-10 05:55:45.000000 dtfabric-20230519/test_data/structure_with_string.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      370 2022-07-10 05:55:47.000000 dtfabric-20230519/test_data/structure_with_union.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      700 2022-07-10 05:55:49.000000 dtfabric-20230519/test_data/structure_with_values.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      383 2022-07-10 05:55:53.000000 dtfabric-20230519/test_data/union.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      380 2022-07-10 05:55:51.000000 dtfabric-20230519/test_data/union_with_condition.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      200 2022-07-10 05:55:54.000000 dtfabric-20230519/test_data/uuid.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      107 2022-12-18 07:46:44.000000 dtfabric-20230519/test_dependencies.ini
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       14 2023-05-12 04:16:07.000000 dtfabric-20230519/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.241414 dtfabric-20230519/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230519/tests/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19685 2022-02-13 10:09:16.000000 dtfabric-20230519/tests/data_types.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    62234 2023-05-18 03:22:07.000000 dtfabric-20230519/tests/reader.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2021-07-30 06:46:25.000000 dtfabric-20230519/tests/registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.295414 dtfabric-20230519/tests/runtime/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230519/tests/runtime/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2021-07-30 09:04:50.000000 dtfabric-20230519/tests/runtime/byte_operations.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84696 2023-05-18 15:50:47.000000 dtfabric-20230519/tests/runtime/data_maps.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      662 2021-07-30 06:46:25.000000 dtfabric-20230519/tests/runtime/fabric.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2494 2021-07-30 06:46:25.000000 dtfabric-20230519/tests/runtime/runtime.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2022-09-18 09:32:59.000000 dtfabric-20230519/tests/test_lib.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2023-05-12 04:16:07.000000 dtfabric-20230519/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.302414 dtfabric-20230519/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       70 2018-03-18 06:58:04.000000 dtfabric-20230519/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-12 04:16:07.000000 dtfabric-20230519/utils/check_dependencies.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-12 04:16:07.000000 dtfabric-20230519/utils/dependencies.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      616 2021-12-28 04:01:20.000000 dtfabric-20230519/utils/update_release.sh
```

### Comparing `dtfabric-20230518/.github/workflows/test_docker.yml` & `dtfabric-20230519/.github/workflows/test_docker.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/.github/workflows/test_docs.yml` & `dtfabric-20230519/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/.github/workflows/test_tox.yml` & `dtfabric-20230519/.github/workflows/test_tox.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/.pylintrc` & `dtfabric-20230519/.pylintrc`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/LICENSE` & `dtfabric-20230519/LICENSE`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/MANIFEST.in` & `dtfabric-20230519/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/PKG-INFO` & `dtfabric-20230519/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfabric
-Version: 20230518
+Version: 20230519
 Summary: Data type fabric (dtfabric)
 Home-page: https://github.com/libyal/dtfabric
 Maintainer: Joachim Metz
 Maintainer-email: joachim.metz@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dtfabric-20230518/appveyor.yml` & `dtfabric-20230519/appveyor.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/config/appveyor/install.ps1` & `dtfabric-20230519/config/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/config/appveyor/runtests.sh` & `dtfabric-20230519/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/config/dpkg/control` & `dtfabric-20230519/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/config/dpkg/copyright` & `dtfabric-20230519/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/docs/conf.py` & `dtfabric-20230519/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/docs/index.rst` & `dtfabric-20230519/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/docs/sources/Format-specification.md` & `dtfabric-20230519/docs/sources/Format-specification.md`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/docs/sources/api/dtfabric.rst` & `dtfabric-20230519/docs/sources/api/dtfabric.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/docs/sources/api/dtfabric.runtime.rst` & `dtfabric-20230519/docs/sources/api/dtfabric.runtime.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/docs/sources/user/Installation-instructions.md` & `dtfabric-20230519/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric/data_types.py` & `dtfabric-20230519/dtfabric/data_types.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric/decorators.py` & `dtfabric-20230519/dtfabric/decorators.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric/definitions.py` & `dtfabric-20230519/dtfabric/definitions.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric/errors.py` & `dtfabric-20230519/dtfabric/errors.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric/reader.py` & `dtfabric-20230519/dtfabric/reader.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric/registry.py` & `dtfabric-20230519/dtfabric/registry.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric/runtime/byte_operations.py` & `dtfabric-20230519/dtfabric/runtime/byte_operations.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric/runtime/data_maps.py` & `dtfabric-20230519/dtfabric/runtime/data_maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2316,17 +2316,28 @@
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
     context_state = getattr(context, 'state', {})
 
     member_identifier = context_state.get('member_identifier', None)
     if member_identifier is None:
-      subcontext = DataTypeMapContext()
-      mapped_base_value = self._base_data_type_map.MapByteStream(
-          byte_stream, context=subcontext, **kwargs)
+      subcontext = context_state.get('context', None)
+      if not subcontext:
+        subcontext = DataTypeMapContext()
+
+      try:
+        mapped_base_value = self._base_data_type_map.MapByteStream(
+            byte_stream, context=subcontext, **kwargs)
+
+      except errors.ByteStreamTooSmallError as exception:
+        context_state['context'] = subcontext
+        raise exception
+
+      except Exception as exception:
+        raise errors.MappingError(exception)
 
       member_identifier = getattr(
           mapped_base_value, self._data_type_definition.identifier, None)
       if member_identifier is None:
         raise errors.MappingError(
             f'Unable to determine value of '
             f'{self._data_type_definition.identifier:s}')
@@ -2337,15 +2348,14 @@
     if member_data_type_map is None:
       raise errors.MappingError(
           f'Missing member data type map for '
           f'{self._data_type_definition.identifier:s}: '
           f'{member_identifier!s}')
 
     subcontext = context_state.get('context', None)
-
     if not subcontext:
       subcontext = DataTypeMapContext()
 
     if context:
       context.byte_size = None
 
     try:
```

### Comparing `dtfabric-20230518/dtfabric/runtime/fabric.py` & `dtfabric-20230519/dtfabric/runtime/fabric.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric/runtime/runtime.py` & `dtfabric-20230519/dtfabric/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/dtfabric.egg-info/PKG-INFO` & `dtfabric-20230519/dtfabric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfabric
-Version: 20230518
+Version: 20230519
 Summary: Data type fabric (dtfabric)
 Home-page: https://github.com/libyal/dtfabric
 Maintainer: Joachim Metz
 Maintainer-email: joachim.metz@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dtfabric-20230518/dtfabric.egg-info/SOURCES.txt` & `dtfabric-20230519/dtfabric.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 dtfabric.egg-info/top_level.txt
 dtfabric/runtime/__init__.py
 dtfabric/runtime/byte_operations.py
 dtfabric/runtime/data_maps.py
 dtfabric/runtime/fabric.py
 dtfabric/runtime/runtime.py
 scripts/validate-definitions.py
-test_data/.structure_with_string.yaml.swp
 test_data/Notepad.lnk
 test_data/boolean.yaml
 test_data/character.yaml
 test_data/constant.yaml
 test_data/enumeration.yaml
 test_data/floating-point.yaml
 test_data/format.yaml
```

### Comparing `dtfabric-20230518/run_tests.py` & `dtfabric-20230519/run_tests.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/scripts/validate-definitions.py` & `dtfabric-20230519/scripts/validate-definitions.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/setup.py` & `dtfabric-20230519/setup.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/Notepad.lnk` & `dtfabric-20230519/test_data/Notepad.lnk`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/definitions/booleans.yaml` & `dtfabric-20230519/test_data/definitions/booleans.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/definitions/integers.yaml` & `dtfabric-20230519/test_data/definitions/integers.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/enumeration.yaml` & `dtfabric-20230519/test_data/enumeration.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/format.yaml` & `dtfabric-20230519/test_data/format.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/sequence_with_context.yaml` & `dtfabric-20230519/test_data/sequence_with_context.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/stream.yaml` & `dtfabric-20230519/test_data/stream.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/string.yaml` & `dtfabric-20230519/test_data/string.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/string_array.yaml` & `dtfabric-20230519/test_data/string_array.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/structure.yaml` & `dtfabric-20230519/test_data/structure.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/structure_family.yaml` & `dtfabric-20230519/test_data/structure_family.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/structure_group.yaml` & `dtfabric-20230519/test_data/structure_group.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/structure_with_condition.yaml` & `dtfabric-20230519/test_data/structure_with_condition.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/structure_with_padding.yaml` & `dtfabric-20230519/test_data/structure_with_padding.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/test_data/structure_with_values.yaml` & `dtfabric-20230519/test_data/structure_with_values.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/tests/data_types.py` & `dtfabric-20230519/tests/data_types.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/tests/reader.py` & `dtfabric-20230519/tests/reader.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/tests/registry.py` & `dtfabric-20230519/tests/registry.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/tests/runtime/byte_operations.py` & `dtfabric-20230519/tests/runtime/byte_operations.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/tests/runtime/data_maps.py` & `dtfabric-20230519/tests/runtime/data_maps.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/tests/runtime/fabric.py` & `dtfabric-20230519/tests/runtime/fabric.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/tests/runtime/runtime.py` & `dtfabric-20230519/tests/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/tests/test_lib.py` & `dtfabric-20230519/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/tox.ini` & `dtfabric-20230519/tox.ini`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/utils/dependencies.py` & `dtfabric-20230519/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230518/utils/update_release.sh` & `dtfabric-20230519/utils/update_release.sh`

 * *Files identical despite different names*

