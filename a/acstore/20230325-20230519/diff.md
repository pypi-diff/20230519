# Comparing `tmp/acstore-20230325.tar.gz` & `tmp/acstore-20230519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acstore-20230325.tar", last modified: Sat Mar 25 15:57:23 2023, max compression
+gzip compressed data, was "acstore-20230519.tar", last modified: Fri May 19 08:45:59 2023, max compression
```

## Comparing `acstore-20230325.tar` & `acstore-20230519.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.960422 acstore-20230325/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.930422 acstore-20230325/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.934422 acstore-20230325/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2515 2023-03-19 12:37:59.000000 acstore-20230325/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-03-19 12:37:59.000000 acstore-20230325/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1666 2023-03-19 12:37:59.000000 acstore-20230325/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21911 2023-03-19 06:58:19.000000 acstore-20230325/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       94 2017-10-14 04:46:14.000000 acstore-20230325/.style.yapf
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      575 2017-10-14 04:46:14.000000 acstore-20230325/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      368 2017-10-14 04:46:14.000000 acstore-20230325/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2017-10-14 04:46:14.000000 acstore-20230325/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      494 2021-10-31 11:15:56.000000 acstore-20230325/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      617 2023-03-25 15:57:23.960422 acstore-20230325/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      249 2021-11-25 16:00:25.000000 acstore-20230325/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.934422 acstore-20230325/acstore/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      215 2023-03-25 12:48:58.000000 acstore-20230325/acstore/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.955422 acstore-20230325/acstore/containers/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-10-31 12:45:06.000000 acstore-20230325/acstore/containers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6621 2023-03-13 05:41:43.000000 acstore-20230325/acstore/containers/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3815 2022-10-02 11:32:41.000000 acstore-20230325/acstore/containers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-03-19 12:37:59.000000 acstore-20230325/acstore/errors.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6468 2022-12-31 10:05:21.000000 acstore-20230325/acstore/fake_store.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.955422 acstore-20230325/acstore/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-03-19 12:37:59.000000 acstore-20230325/acstore/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2243 2023-03-25 15:56:17.000000 acstore-20230325/acstore/helpers/schema.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4600 2023-03-19 12:37:59.000000 acstore-20230325/acstore/helpers/yaml_definitions_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6488 2023-03-25 15:56:17.000000 acstore-20230325/acstore/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-03-13 05:41:43.000000 acstore-20230325/acstore/profilers.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36560 2023-03-25 15:56:17.000000 acstore-20230325/acstore/sqlite_store.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.954422 acstore-20230325/acstore.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      617 2023-03-25 15:57:23.000000 acstore-20230325/acstore.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2023-03-25 15:57:23.000000 acstore-20230325/acstore.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-03-25 15:57:23.000000 acstore-20230325/acstore.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-03-25 15:57:23.000000 acstore-20230325/acstore.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2023-03-25 15:57:23.000000 acstore-20230325/acstore.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      397 2021-10-31 13:20:13.000000 acstore-20230325/acstore.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-03-19 06:58:19.000000 acstore-20230325/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.931422 acstore-20230325/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.956422 acstore-20230325/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      758 2023-03-19 12:37:59.000000 acstore-20230325/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-03-19 06:58:19.000000 acstore-20230325/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-03-19 06:58:19.000000 acstore-20230325/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.956422 acstore-20230325/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      170 2023-03-25 12:48:58.000000 acstore-20230325/config/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       20 2022-12-30 06:35:00.000000 acstore-20230325/config/dpkg/clean
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-03-19 06:58:19.000000 acstore-20230325/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-03-19 12:37:59.000000 acstore-20230325/config/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2022-12-30 06:35:48.000000 acstore-20230325/config/dpkg/copyright
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-03-19 06:58:19.000000 acstore-20230325/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.957422 acstore-20230325/config/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2022-12-30 06:34:18.000000 acstore-20230325/config/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      151 2023-03-19 12:37:59.000000 acstore-20230325/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.957422 acstore-20230325/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5053 2023-03-19 06:58:19.000000 acstore-20230325/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      511 2021-11-01 05:25:03.000000 acstore-20230325/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-03-19 06:58:51.000000 acstore-20230325/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.931422 acstore-20230325/docs/sources/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.957422 acstore-20230325/docs/sources/api/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      540 2021-10-31 13:20:13.000000 acstore-20230325/docs/sources/api/acstore.containers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      550 2023-03-25 12:48:58.000000 acstore-20230325/docs/sources/api/acstore.helpers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2023-03-25 12:48:58.000000 acstore-20230325/docs/sources/api/acstore.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       58 2021-10-31 13:20:13.000000 acstore-20230325/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.958422 acstore-20230325/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2021-12-28 07:11:12.000000 acstore-20230325/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      286 2021-10-31 13:20:13.000000 acstore-20230325/docs/sources/user/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-03-19 12:37:59.000000 acstore-20230325/requirements.txt
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      929 2022-06-05 12:44:16.000000 acstore-20230325/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      333 2023-03-25 15:57:23.960422 acstore-20230325/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6292 2023-03-19 06:58:19.000000 acstore-20230325/setup.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.958422 acstore-20230325/test_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      171 2023-03-19 12:37:59.000000 acstore-20230325/test_data/definitions.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-21 18:11:19.000000 acstore-20230325/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-19 06:58:19.000000 acstore-20230325/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.959422 acstore-20230325/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-07-12 17:42:16.000000 acstore-20230325/tests/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.959422 acstore-20230325/tests/containers/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-10-31 12:45:06.000000 acstore-20230325/tests/containers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5824 2022-12-29 02:46:08.000000 acstore-20230325/tests/containers/interface.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3082 2021-11-25 16:00:25.000000 acstore-20230325/tests/containers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8446 2022-12-29 02:46:08.000000 acstore-20230325/tests/fake_store.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.959422 acstore-20230325/tests/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-03-19 12:37:59.000000 acstore-20230325/tests/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-03-25 15:56:17.000000 acstore-20230325/tests/helpers/schema.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3052 2023-03-19 12:37:59.000000 acstore-20230325/tests/helpers/yaml_definitions_file.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2004 2021-12-28 03:54:14.000000 acstore-20230325/tests/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-01-01 10:11:51.000000 acstore-20230325/tests/profilers.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20147 2023-03-21 19:40:47.000000 acstore-20230325/tests/sqlite_store.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2375 2023-03-19 12:37:59.000000 acstore-20230325/tests/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2023-03-19 06:58:19.000000 acstore-20230325/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-03-25 15:57:23.960422 acstore-20230325/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2017-10-14 04:46:14.000000 acstore-20230325/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-03-19 06:58:19.000000 acstore-20230325/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-03-19 06:58:19.000000 acstore-20230325/utils/dependencies.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      645 2021-12-28 07:11:12.000000 acstore-20230325/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.739173 acstore-20230519/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.673173 acstore-20230519/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.694173 acstore-20230519/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2515 2023-05-19 03:32:32.000000 acstore-20230519/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-05-19 03:32:32.000000 acstore-20230519/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4068 2023-05-19 03:32:32.000000 acstore-20230519/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22994 2023-05-19 08:45:21.000000 acstore-20230519/.pylintrc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       94 2017-10-14 04:46:14.000000 acstore-20230519/.style.yapf
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2023-04-30 06:19:09.000000 acstore-20230519/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      575 2017-10-14 04:46:14.000000 acstore-20230519/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      368 2017-10-14 04:46:14.000000 acstore-20230519/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2017-10-14 04:46:14.000000 acstore-20230519/LICENSE
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      494 2021-10-31 11:15:56.000000 acstore-20230519/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      617 2023-05-19 08:45:59.739173 acstore-20230519/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      249 2021-11-25 16:00:25.000000 acstore-20230519/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.695173 acstore-20230519/acstore/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      215 2023-05-19 08:45:21.000000 acstore-20230519/acstore/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.696173 acstore-20230519/acstore/containers/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-10-31 12:45:06.000000 acstore-20230519/acstore/containers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6615 2023-05-19 03:32:13.000000 acstore-20230519/acstore/containers/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3816 2023-05-19 03:32:13.000000 acstore-20230519/acstore/containers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-03-19 12:37:59.000000 acstore-20230519/acstore/errors.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6468 2023-04-08 08:07:41.000000 acstore-20230519/acstore/fake_store.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.697173 acstore-20230519/acstore/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-03-19 12:37:59.000000 acstore-20230519/acstore/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2242 2023-05-19 03:32:13.000000 acstore-20230519/acstore/helpers/schema.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4600 2023-03-19 12:37:59.000000 acstore-20230519/acstore/helpers/yaml_definitions_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6488 2023-04-08 08:07:41.000000 acstore-20230519/acstore/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-03-13 05:41:43.000000 acstore-20230519/acstore/profilers.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36558 2023-05-19 03:32:13.000000 acstore-20230519/acstore/sqlite_store.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.696173 acstore-20230519/acstore.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      617 2023-05-19 08:45:58.000000 acstore-20230519/acstore.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2023-05-19 08:45:59.000000 acstore-20230519/acstore.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-19 08:45:58.000000 acstore-20230519/acstore.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-05-19 08:45:58.000000 acstore-20230519/acstore.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2023-05-19 08:45:58.000000 acstore-20230519/acstore.egg-info/top_level.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      397 2021-10-31 13:20:13.000000 acstore-20230519/acstore.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-19 03:32:32.000000 acstore-20230519/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.673173 acstore-20230519/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.697173 acstore-20230519/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      834 2023-05-19 03:32:32.000000 acstore-20230519/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-19 03:32:32.000000 acstore-20230519/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-19 03:32:32.000000 acstore-20230519/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.728173 acstore-20230519/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      170 2023-05-19 08:45:21.000000 acstore-20230519/config/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       20 2022-12-30 06:35:00.000000 acstore-20230519/config/dpkg/clean
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-19 03:32:33.000000 acstore-20230519/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-19 03:32:33.000000 acstore-20230519/config/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2022-12-30 06:35:48.000000 acstore-20230519/config/dpkg/copyright
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-19 03:32:33.000000 acstore-20230519/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.728173 acstore-20230519/config/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2022-12-30 06:34:18.000000 acstore-20230519/config/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      151 2023-03-19 12:37:59.000000 acstore-20230519/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.736173 acstore-20230519/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5049 2023-05-19 03:32:49.000000 acstore-20230519/docs/conf.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      511 2021-11-01 05:25:03.000000 acstore-20230519/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-05-19 03:32:49.000000 acstore-20230519/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.674173 acstore-20230519/docs/sources/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.737173 acstore-20230519/docs/sources/api/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      540 2021-10-31 13:20:13.000000 acstore-20230519/docs/sources/api/acstore.containers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      550 2023-03-25 12:48:58.000000 acstore-20230519/docs/sources/api/acstore.helpers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2023-03-25 12:48:58.000000 acstore-20230519/docs/sources/api/acstore.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       58 2021-10-31 13:20:13.000000 acstore-20230519/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.737173 acstore-20230519/docs/sources/user/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2021-12-28 07:11:12.000000 acstore-20230519/docs/sources/user/Installation-instructions.md
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      286 2021-10-31 13:20:13.000000 acstore-20230519/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-05-19 03:32:32.000000 acstore-20230519/requirements.txt
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      929 2022-06-05 12:44:16.000000 acstore-20230519/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      333 2023-05-19 08:45:59.740173 acstore-20230519/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6292 2023-05-19 03:32:32.000000 acstore-20230519/setup.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.737173 acstore-20230519/test_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      171 2023-03-19 12:37:59.000000 acstore-20230519/test_data/definitions.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-21 18:11:19.000000 acstore-20230519/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 03:32:32.000000 acstore-20230519/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.738173 acstore-20230519/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-07-12 17:42:16.000000 acstore-20230519/tests/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.738173 acstore-20230519/tests/containers/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-10-31 12:45:06.000000 acstore-20230519/tests/containers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5868 2023-05-19 08:45:21.000000 acstore-20230519/tests/containers/interface.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3082 2021-11-25 16:00:25.000000 acstore-20230519/tests/containers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8446 2022-12-29 02:46:08.000000 acstore-20230519/tests/fake_store.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.739173 acstore-20230519/tests/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-03-19 12:37:59.000000 acstore-20230519/tests/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-03-25 15:56:17.000000 acstore-20230519/tests/helpers/schema.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3052 2023-03-19 12:37:59.000000 acstore-20230519/tests/helpers/yaml_definitions_file.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2004 2021-12-28 03:54:14.000000 acstore-20230519/tests/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2023-05-19 08:45:21.000000 acstore-20230519/tests/profilers.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20146 2023-05-19 03:32:13.000000 acstore-20230519/tests/sqlite_store.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2375 2023-03-19 12:37:59.000000 acstore-20230519/tests/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1242 2023-05-19 08:45:21.000000 acstore-20230519/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 08:45:59.739173 acstore-20230519/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2017-10-14 04:46:14.000000 acstore-20230519/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-19 03:32:33.000000 acstore-20230519/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-19 08:45:21.000000 acstore-20230519/utils/dependencies.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      645 2021-12-28 07:11:12.000000 acstore-20230519/utils/update_release.sh
```

### Comparing `acstore-20230325/.github/workflows/test_docker.yml` & `acstore-20230519/.github/workflows/test_docker.yml`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 on: [push]
 permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['37']
+        version: ['38']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
         dnf install -y @development-tools python3 python3-devel python3-pyyaml python3-setuptools
@@ -41,15 +41,15 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         version: ['22.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
```

### Comparing `acstore-20230325/.github/workflows/test_docs.yml` & `acstore-20230519/.github/workflows/test_docs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       matrix:
         include:
         - python-version: '3.8'
           toxenv: 'docs'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
```

### Comparing `acstore-20230325/.pylintrc` & `acstore-20230519/.pylintrc`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-# Pylint 2.14.x configuration file
+# Pylint 2.17.x configuration file
 #
 # This file is generated by l2tdevtools update-dependencies.py, any dependency
 # related changes should be made in dependencies.ini.
 [MAIN]
 
 # Analyse import fallback blocks. This can be used to support both Python 2 and
 # 3 compatible code, which means that the block might have code that exists
 # only in one or another interpreter, leading to false positives when analysed.
 analyse-fallback-blocks=no
 
+# Clear in-memory caches upon conclusion of linting. Useful if running pylint
+# in a server-like mode.
+clear-cache-post-run=no
+
 # Load and enable all available extensions. Use --list-extensions to see a list
 # all available extensions.
 #enable-all-extensions=
 
 # In error mode, messages with a category besides ERROR or FATAL are
 # suppressed, and no reports are done by default. Error mode is compatible with
 # disabling specific errors.
@@ -34,31 +38,33 @@
 extension-pkg-whitelist=
 
 # Return non-zero exit code if any of these messages/categories are detected,
 # even if score is above --fail-under value. Syntax same as enable. Messages
 # specified are enabled, while categories only check already-enabled messages.
 fail-on=
 
-# Specify a score threshold to be exceeded before program exits with error.
+# Specify a score threshold under which the program will exit with error.
 fail-under=10
 
 # Interpret the stdin as a python script, whose filename needs to be passed as
 # the module_or_package argument.
 #from-stdin=
 
 # Files or directories to be skipped. They should be base names, not paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the ignore-list. The
-# regex matches against paths and can be in Posix or Windows format.
+# Add files or directories matching the regular expressions patterns to the
+# ignore-list. The regex matches against paths and can be in Posix or Windows
+# format. Because '\\' represents the directory delimiter on Windows systems,
+# it can't be used as an escape character.
 ignore-paths=
 
-# Files or directories matching the regex patterns are skipped. The regex
-# matches against base names, not paths. The default value ignores Emacs file
-# locks
+# Files or directories matching the regular expression patterns are skipped.
+# The regex matches against base names, not paths. The default value ignores
+# Emacs file locks
 ignore-patterns=^\.#
 
 # List of module names for which member attributes should not be checked
 # (useful for modules/projects where namespaces are manipulated during runtime
 # and thus existing member attributes cannot be deduced by static analysis). It
 # supports qualified module names, as well as Unix pattern matching.
 ignored-modules=
@@ -89,249 +95,32 @@
 # the version used to run pylint.
 py-version=3.11
 
 # Discover python modules and packages in the file system subtree.
 # recursive=no
 recursive=yes
 
+# Add paths to the list of the source roots. Supports globbing patterns. The
+# source root is an absolute path or a path relative to the current working
+# directory used to determine a package namespace for modules located under the
+# source root.
+source-roots=
+
 # When enabled, pylint would attempt to guess common misconfiguration and emit
 # user-friendly hints instead of false-positive error messages.
 suggestion-mode=yes
 
 # Allow loading of arbitrary C extensions. Extensions are imported into the
 # active Python interpreter and may run arbitrary code.
 unsafe-load-any-extension=no
 
 # In verbose mode, extra non-checker-related info will be displayed.
 #verbose=
 
 
-[REPORTS]
-
-# Python expression which should return a score less than or equal to 10. You
-# have access to the variables 'fatal', 'error', 'warning', 'refactor',
-# 'convention', and 'info' which contain the number of messages in each
-# category, as well as 'statement' which is the total number of statements
-# analyzed. This score is used by the global evaluation report (RP0004).
-evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
-
-# Template used to display messages. This is a python new-style format string
-# used to format the message information. See doc for all details.
-msg-template=
-
-# Set the output format. Available formats are text, parseable, colorized, json
-# and msvs (visual studio). You can also give a reporter class, e.g.
-# mypackage.mymodule.MyReporterClass.
-#output-format=
-
-# Tells whether to display a full report or only the messages.
-reports=no
-
-# Activate the evaluation score.
-# score=yes
-score=no
-
-
-[MESSAGES CONTROL]
-
-# Only show warnings with the listed confidence levels. Leave empty to show
-# all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
-# UNDEFINED.
-confidence=HIGH,
-           CONTROL_FLOW,
-           INFERENCE,
-           INFERENCE_FAILURE,
-           UNDEFINED
-
-# Disable the message, report, category or checker with the given id(s). You
-# can either give multiple identifiers separated by comma (,) or put this
-# option multiple times (only on the command line, not in the configuration
-# file where it should appear only once). You can also use "--disable=all" to
-# disable everything first and then re-enable specific checks. For example, if
-# you want to run only the similarities checker, you can use "--disable=all
-# --enable=similarities". If you want to run only the classes checker, but have
-# no Warning level messages displayed, use "--disable=all --enable=classes
-# --disable=W".
-disable=assignment-from-none,
-        bad-inline-option,
-        consider-using-f-string,
-        deprecated-pragma,
-        duplicate-code,
-        file-ignored,
-        fixme,
-        locally-disabled,
-        logging-format-interpolation,
-        logging-fstring-interpolation,
-        missing-param-doc,
-        raise-missing-from,
-        raw-checker-failed,
-        super-with-arguments,
-        suppressed-message,
-        too-few-public-methods,
-        too-many-ancestors,
-        too-many-boolean-expressions,
-        too-many-branches,
-        too-many-instance-attributes,
-        too-many-lines,
-        too-many-locals,
-        too-many-nested-blocks,
-        too-many-public-methods,
-        too-many-return-statements,
-        too-many-statements,
-        unsubscriptable-object,
-        useless-object-inheritance,
-        useless-suppression
-
-# Enable the message, report, category or checker with the given id(s). You can
-# either give multiple identifier separated by comma (,) or put this option
-# multiple time (only on the command line, not in the configuration file where
-# it should appear only once). See also the "--disable" option for examples.
-enable=c-extension-no-member
-
-
-[VARIABLES]
-
-# List of additional names supposed to be defined in builtins. Remember that
-# you should avoid defining new builtins when possible.
-additional-builtins=
-
-# Tells whether unused global variables should be treated as a violation.
-allow-global-unused-variables=yes
-
-# List of names allowed to shadow builtins
-allowed-redefined-builtins=
-
-# List of strings which can identify a callback function by name. A callback
-# name must start or end with one of those strings.
-callbacks=cb_,
-          _cb
-
-# A regular expression matching the name of dummy variables (i.e. expected to
-# not be used).
-dummy-variables-rgx=_+$|(_[a-zA-Z0-9_]*[a-zA-Z0-9]+?$)|dummy|^ignored_|^unused_
-
-# Argument names that match this expression will be ignored. Default to name
-# with leading underscore.
-ignored-argument-names=_.*|^ignored_|^unused_
-
-# Tells whether we should check for unused import in __init__ files.
-init-import=no
-
-# List of qualified module names which can have objects that can redefine
-# builtins.
-redefining-builtins-modules=six.moves,past.builtins,future.builtins,builtins,io
-
-
-[TYPECHECK]
-
-# List of decorators that produce context managers, such as
-# contextlib.contextmanager. Add to this list to register other decorators that
-# produce valid context managers.
-contextmanager-decorators=contextlib.contextmanager
-
-# List of members which are set dynamically and missed by pylint inference
-# system, and so shouldn't trigger E1101 when accessed. Python regular
-# expressions are accepted.
-generated-members=
-
-# Tells whether to warn about missing members when the owner of the attribute
-# is inferred to be None.
-ignore-none=yes
-
-# This flag controls whether pylint should warn about no-member and similar
-# checks whenever an opaque object is returned when inferring. The inference
-# can return multiple potential results while evaluating a Python object, but
-# some branches might not be evaluated, which results in partial inference. In
-# that case, it might be useful to still emit no-member and other checks for
-# the rest of the inferred objects.
-ignore-on-opaque-inference=yes
-
-# List of symbolic message names to ignore for Mixin members.
-ignored-checks-for-mixins=no-member,
-                          not-async-context-manager,
-                          not-context-manager,
-                          attribute-defined-outside-init
-
-# List of class names for which member attributes should not be checked (useful
-# for classes with dynamically set attributes). This supports the use of
-# qualified names.
-ignored-classes=optparse.Values,thread._local,_thread._local,argparse.Namespace
-
-# Show a hint with possible names when a member name was not found. The aspect
-# of finding the hint is based on edit distance.
-missing-member-hint=yes
-
-# The minimum edit distance a name should have in order to be considered a
-# similar match for a missing member name.
-missing-member-hint-distance=1
-
-# The total number of similar names that should be taken in consideration when
-# showing a hint for a missing member.
-missing-member-max-choices=1
-
-# Regex pattern to define which classes are considered mixins.
-mixin-class-rgx=.*[Mm]ixin
-
-# List of decorators that change the signature of a decorated function.
-signature-mutators=
-
-
-[LOGGING]
-
-# The type of string formatting that logging methods do. `old` means using %
-# formatting, `new` is for `{}` formatting.
-logging-format-style=old
-
-# Logging modules to check that the string format arguments are in logging
-# function parameter format.
-logging-modules=logging
-
-
-[DESIGN]
-
-# List of regular expressions of class ancestor names to ignore when counting
-# public methods (see R0903)
-exclude-too-few-public-methods=
-
-# List of qualified class names to ignore when counting class parents (see
-# R0901)
-ignored-parents=
-
-# Maximum number of arguments for function / method.
-# max-args=5
-max-args=10
-
-# Maximum number of attributes for a class (see R0902).
-max-attributes=7
-
-# Maximum number of boolean expressions in an if statement (see R0916).
-max-bool-expr=5
-
-# Maximum number of branch for function / method body.
-max-branches=12
-
-# Maximum number of locals for function / method body.
-max-locals=15
-
-# Maximum number of parents for a class (see R0901).
-max-parents=7
-
-# Maximum number of public methods for a class (see R0904).
-max-public-methods=20
-
-# Maximum number of return / yield for function / method body.
-max-returns=6
-
-# Maximum number of statements in function / method body.
-max-statements=50
-
-# Minimum number of public methods for a class (see R0903).
-min-public-methods=2
-
-
 [BASIC]
 
 # Naming style matching correct argument names.
 argument-naming-style=snake_case
 
 # Regular expression matching correct argument names. Overrides argument-
 # naming-style. If left empty, argument names will be checked with the set
@@ -456,70 +245,102 @@
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 # These decorators are taken in consideration only for invalid-name.
 property-classes=abc.abstractproperty
 
+# Regular expression matching correct type alias names. If left empty, type
+# alias names will be checked with the set naming style.
+#typealias-rgx=
+
 # Regular expression matching correct type variable names. If left empty, type
 # variable names will be checked with the set naming style.
 #typevar-rgx=
 
 # Naming style matching correct variable names.
 variable-naming-style=snake_case
 
 # Regular expression matching correct variable names. Overrides variable-
 # naming-style. If left empty, variable names will be checked with the set
 # naming style.
 #variable-rgx=
 variable-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 
-[EXCEPTIONS]
-
-# Exceptions that will emit a warning when caught.
-overgeneral-exceptions=BaseException,
-                       Exception
-
-
 [CLASSES]
 
 # Warn about protected attribute access inside special methods
 check-protected-access-in-special-methods=no
 
 # List of method names used to declare (i.e. assign) instance attributes.
 defining-attr-methods=__init__,
                       __new__,
                       setUp,
+                      asyncSetUp,
                       __post_init__
 
 # List of member names, which should be excluded from the protected access
 # warning.
-exclude-protected=_asdict,
-                  _fields,
-                  _replace,
-                  _source,
-                  _make
+exclude-protected=_asdict,_fields,_replace,_source,_make,os._exit
 
 # List of valid names for the first argument in a class method.
 valid-classmethod-first-arg=cls
 
 # List of valid names for the first argument in a metaclass class method.
+# valid-metaclass-classmethod-first-arg=mcs
 valid-metaclass-classmethod-first-arg=cls
 
 
-[MISCELLANEOUS]
+[DESIGN]
 
-# List of note tags to take in consideration, separated by a comma.
-notes=FIXME,
-      XXX,
-      TODO
+# List of regular expressions of class ancestor names to ignore when counting
+# public methods (see R0903)
+exclude-too-few-public-methods=
 
-# Regular expression of note tags to take in consideration.
-notes-rgx=
+# List of qualified class names to ignore when counting class parents (see
+# R0901)
+ignored-parents=
+
+# Maximum number of arguments for function / method.
+# max-args=5
+max-args=10
+
+# Maximum number of attributes for a class (see R0902).
+max-attributes=7
+
+# Maximum number of boolean expressions in an if statement (see R0916).
+max-bool-expr=5
+
+# Maximum number of branch for function / method body.
+max-branches=12
+
+# Maximum number of locals for function / method body.
+max-locals=15
+
+# Maximum number of parents for a class (see R0901).
+max-parents=7
+
+# Maximum number of public methods for a class (see R0904).
+max-public-methods=20
+
+# Maximum number of return / yield for function / method body.
+max-returns=6
+
+# Maximum number of statements in function / method body.
+max-statements=50
+
+# Minimum number of public methods for a class (see R0903).
+min-public-methods=2
+
+
+[EXCEPTIONS]
+
+# Exceptions that will emit a warning when caught.
+overgeneral-exceptions=builtins.BaseException,builtins.Exception
 
 
 [FORMAT]
 
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 expected-line-ending-format=
 
@@ -546,14 +367,196 @@
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
 
 
+[IMPORTS]
+
+# List of modules that can be imported at any level, not just the top level
+# one.
+allow-any-import-level=
+
+# Allow explicit reexports by alias from a package __init__.
+allow-reexport-from-package=no
+
+# Allow wildcard imports from modules that define __all__.
+allow-wildcard-with-all=no
+
+# Deprecated modules which should not be used, separated by a comma.
+deprecated-modules=
+
+# Output a graph (.gv or any supported image format) of external dependencies
+# to the given file (report RP0402 must not be disabled).
+ext-import-graph=
+
+# Output a graph (.gv or any supported image format) of all (i.e. internal and
+# external) dependencies to the given file (report RP0402 must not be
+# disabled).
+import-graph=
+
+# Output a graph (.gv or any supported image format) of internal dependencies
+# to the given file (report RP0402 must not be disabled).
+int-import-graph=
+
+# Force import order to recognize a module as part of the standard
+# compatibility libraries.
+known-standard-library=
+
+# Force import order to recognize a module as part of a third party library.
+known-third-party=enchant
+
+# Couples of modules and preferred modules, separated by a comma.
+preferred-modules=
+
+
+[LOGGING]
+
+# The type of string formatting that logging methods do. `old` means using %
+# formatting, `new` is for `{}` formatting.
+logging-format-style=old
+
+# Logging modules to check that the string format arguments are in logging
+# function parameter format.
+logging-modules=logging
+
+
+[MESSAGES CONTROL]
+
+# Only show warnings with the listed confidence levels. Leave empty to show
+# all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
+# UNDEFINED.
+confidence=HIGH,
+           CONTROL_FLOW,
+           INFERENCE,
+           INFERENCE_FAILURE,
+           UNDEFINED
+
+# Disable the message, report, category or checker with the given id(s). You
+# can either give multiple identifiers separated by comma (,) or put this
+# option multiple times (only on the command line, not in the configuration
+# file where it should appear only once). You can also use "--disable=all" to
+# disable everything first and then re-enable specific checks. For example, if
+# you want to run only the similarities checker, you can use "--disable=all
+# --enable=similarities". If you want to run only the classes checker, but have
+# no Warning level messages displayed, use "--disable=all --enable=classes
+# --disable=W".
+disable=assignment-from-none,
+        bad-inline-option,
+        consider-using-f-string,
+        deprecated-pragma,
+        duplicate-code,
+        file-ignored,
+        fixme,
+        locally-disabled,
+        logging-format-interpolation,
+        logging-fstring-interpolation,
+        missing-param-doc,
+        raise-missing-from,
+        raw-checker-failed,
+        super-with-arguments,
+        suppressed-message,
+        too-few-public-methods,
+        too-many-ancestors,
+        too-many-boolean-expressions,
+        too-many-branches,
+        too-many-instance-attributes,
+        too-many-lines,
+        too-many-locals,
+        too-many-nested-blocks,
+        too-many-public-methods,
+        too-many-return-statements,
+        too-many-statements,
+        unsubscriptable-object,
+        useless-object-inheritance,
+        useless-suppression,
+        use-symbolic-message-instead
+
+# Enable the message, report, category or checker with the given id(s). You can
+# either give multiple identifier separated by comma (,) or put this option
+# multiple time (only on the command line, not in the configuration file where
+# it should appear only once). See also the "--disable" option for examples.
+enable=c-extension-no-member
+
+
+[METHOD_ARGS]
+
+# List of qualified names (i.e., library.method) which require a timeout
+# parameter e.g. 'requests.api.get,requests.api.post'
+timeout-methods=requests.api.delete,requests.api.get,requests.api.head,requests.api.options,requests.api.patch,requests.api.post,requests.api.put,requests.api.request
+
+
+[MISCELLANEOUS]
+
+# List of note tags to take in consideration, separated by a comma.
+notes=FIXME,
+      XXX,
+      TODO
+
+# Regular expression of note tags to take in consideration.
+notes-rgx=
+
+
+[REFACTORING]
+
+# Maximum number of nested blocks for function / method body
+max-nested-blocks=5
+
+# Complete name of functions that never returns. When checking for
+# inconsistent-return-statements if a never returning function is called then
+# it will be considered as an explicit return statement and no message will be
+# printed.
+never-returning-functions=sys.exit,argparse.parse_error
+
+
+[REPORTS]
+
+# Python expression which should return a score less than or equal to 10. You
+# have access to the variables 'fatal', 'error', 'warning', 'refactor',
+# 'convention', and 'info' which contain the number of messages in each
+# category, as well as 'statement' which is the total number of statements
+# analyzed. This score is used by the global evaluation report (RP0004).
+evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
+
+# Template used to display messages. This is a python new-style format string
+# used to format the message information. See doc for all details.
+msg-template=
+
+# Set the output format. Available formats are text, parseable, colorized, json
+# and msvs (visual studio). You can also give a reporter class, e.g.
+# mypackage.mymodule.MyReporterClass.
+#output-format=
+
+# Tells whether to display a full report or only the messages.
+reports=no
+
+# Activate the evaluation score.
+# score=yes
+score=no
+
+
+[SIMILARITIES]
+
+# Comments are removed from the similarity computation
+ignore-comments=yes
+
+# Docstrings are removed from the similarity computation
+ignore-docstrings=yes
+
+# Imports are removed from the similarity computation
+ignore-imports=yes
+
+# Signatures are removed from the similarity computation
+ignore-signatures=yes
+
+# Minimum lines number of a similarity.
+min-similarity-lines=4
+
+
 [SPELLING]
 
 # Limits count of emitted suggestions for spelling mistakes.
 max-spelling-suggestions=4
 
 # Spelling dictionary name. Available dictionaries: en_AG (hunspell), en_AU
 # (hunspell), en_BS (hunspell), en_BW (hunspell), en_BZ (hunspell), en_CA
@@ -575,82 +578,102 @@
 spelling-private-dict-file=
 
 # Tells whether to store unknown words to the private dictionary (see the
 # --spelling-private-dict-file option) instead of raising a message.
 spelling-store-unknown-words=no
 
 
-[SIMILARITIES]
-
-# Comments are removed from the similarity computation
-ignore-comments=yes
-
-# Docstrings are removed from the similarity computation
-ignore-docstrings=yes
-
-# Imports are removed from the similarity computation
-ignore-imports=yes
-
-# Signatures are removed from the similarity computation
-ignore-signatures=yes
-
-# Minimum lines number of a similarity.
-min-similarity-lines=4
-
-
 [STRING]
 
 # This flag controls whether inconsistent-quotes generates a warning when the
 # character used as a quote delimiter is used inconsistently within a module.
 check-quote-consistency=no
 
 # This flag controls whether the implicit-str-concat should generate a warning
 # on implicit string concatenation in sequences defined over several lines.
 check-str-concat-over-line-jumps=no
 
 
-[IMPORTS]
+[TYPECHECK]
 
-# List of modules that can be imported at any level, not just the top level
-# one.
-allow-any-import-level=
+# List of decorators that produce context managers, such as
+# contextlib.contextmanager. Add to this list to register other decorators that
+# produce valid context managers.
+contextmanager-decorators=contextlib.contextmanager
 
-# Allow wildcard imports from modules that define __all__.
-allow-wildcard-with-all=no
+# List of members which are set dynamically and missed by pylint inference
+# system, and so shouldn't trigger E1101 when accessed. Python regular
+# expressions are accepted.
+generated-members=
 
-# Deprecated modules which should not be used, separated by a comma.
-deprecated-modules=
+# Tells whether to warn about missing members when the owner of the attribute
+# is inferred to be None.
+ignore-none=yes
 
-# Output a graph (.gv or any supported image format) of external dependencies
-# to the given file (report RP0402 must not be disabled).
-ext-import-graph=
+# This flag controls whether pylint should warn about no-member and similar
+# checks whenever an opaque object is returned when inferring. The inference
+# can return multiple potential results while evaluating a Python object, but
+# some branches might not be evaluated, which results in partial inference. In
+# that case, it might be useful to still emit no-member and other checks for
+# the rest of the inferred objects.
+ignore-on-opaque-inference=yes
 
-# Output a graph (.gv or any supported image format) of all (i.e. internal and
-# external) dependencies to the given file (report RP0402 must not be
-# disabled).
-import-graph=
+# List of symbolic message names to ignore for Mixin members.
+ignored-checks-for-mixins=no-member,
+                          not-async-context-manager,
+                          not-context-manager,
+                          attribute-defined-outside-init
 
-# Output a graph (.gv or any supported image format) of internal dependencies
-# to the given file (report RP0402 must not be disabled).
-int-import-graph=
+# List of class names for which member attributes should not be checked (useful
+# for classes with dynamically set attributes). This supports the use of
+# qualified names.
+ignored-classes=optparse.Values,thread._local,_thread._local,argparse.Namespace
 
-# Force import order to recognize a module as part of the standard
-# compatibility libraries.
-known-standard-library=
+# Show a hint with possible names when a member name was not found. The aspect
+# of finding the hint is based on edit distance.
+missing-member-hint=yes
 
-# Force import order to recognize a module as part of a third party library.
-known-third-party=enchant
+# The minimum edit distance a name should have in order to be considered a
+# similar match for a missing member name.
+missing-member-hint-distance=1
 
-# Couples of modules and preferred modules, separated by a comma.
-preferred-modules=
+# The total number of similar names that should be taken in consideration when
+# showing a hint for a missing member.
+missing-member-max-choices=1
 
+# Regex pattern to define which classes are considered mixins.
+mixin-class-rgx=.*[Mm]ixin
 
-[REFACTORING]
+# List of decorators that change the signature of a decorated function.
+signature-mutators=
 
-# Maximum number of nested blocks for function / method body
-max-nested-blocks=5
 
-# Complete name of functions that never returns. When checking for
-# inconsistent-return-statements if a never returning function is called then
-# it will be considered as an explicit return statement and no message will be
-# printed.
-never-returning-functions=sys.exit,argparse.parse_error
+[VARIABLES]
+
+# List of additional names supposed to be defined in builtins. Remember that
+# you should avoid defining new builtins when possible.
+additional-builtins=
+
+# Tells whether unused global variables should be treated as a violation.
+allow-global-unused-variables=yes
+
+# List of names allowed to shadow builtins
+allowed-redefined-builtins=
+
+# List of strings which can identify a callback function by name. A callback
+# name must start or end with one of those strings.
+callbacks=cb_,
+          _cb
+
+# A regular expression matching the name of dummy variables (i.e. expected to
+# not be used).
+dummy-variables-rgx=_+$|(_[a-zA-Z0-9_]*[a-zA-Z0-9]+?$)|dummy|^ignored_|^unused_
+
+# Argument names that match this expression will be ignored.
+ignored-argument-names=_.*|^ignored_|^unused_
+
+# Tells whether we should check for unused import in __init__ files.
+init-import=no
+
+# List of qualified module names which can have objects that can redefine
+# builtins.
+redefining-builtins-modules=six.moves,past.builtins,future.builtins,builtins,io
```

### Comparing `acstore-20230325/ACKNOWLEDGEMENTS` & `acstore-20230519/ACKNOWLEDGEMENTS`

 * *Files identical despite different names*

### Comparing `acstore-20230325/LICENSE` & `acstore-20230519/LICENSE`

 * *Files identical despite different names*

### Comparing `acstore-20230325/PKG-INFO` & `acstore-20230519/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acstore
-Version: 20230325
+Version: 20230519
 Summary: Attribute Container Storage (ACStore).
 Home-page: https://github.com/log2timeline/acstore
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: 
 Classifier: Environment :: Console
```

### Comparing `acstore-20230325/acstore/containers/interface.py` & `acstore-20230519/acstore/containers/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 
     return None
 
 
 class AttributeContainer(object):
   """The attribute container interface.
 
-  This is the the base class for those object that exists primarily as
+  This is the base class for those object that exists primarily as
   a container of attributes with basic accessors and mutators.
 
   The CONTAINER_TYPE class attribute contains a string that identifies
   the container type, for example the container type "event" identifiers
   an event object.
 
-  Attributes are public class members of an serializable type. Protected and
+  Attributes are public class members of a serializable type. Protected and
   private class members are not to be serialized, with the exception of those
   defined in _SERIALIZABLE_PROTECTED_ATTRIBUTES.
   """
 
   CONTAINER_TYPE = None
 
   # Names of protected attributes, those with a leading underscore, that
@@ -154,15 +154,15 @@
 
   def GetIdentifier(self):
     """Retrieves the identifier.
 
     The identifier is a storage specific value that should not be serialized.
 
     Returns:
-      AttributeContainerIdentifier: an unique identifier for the container.
+      AttributeContainerIdentifier: a unique identifier for the container.
     """
     return self._identifier
 
   def MatchesExpression(self, expression):
     """Determines if an attribute container matches the expression.
 
     Args:
```

### Comparing `acstore-20230325/acstore/containers/manager.py` & `acstore-20230519/acstore/containers/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     if not container_class:
       raise ValueError(f'Unsupported container type: {container_type:s}')
 
     return getattr(container_class, 'SCHEMA', {})
 
   @classmethod
   def RegisterAttributeContainer(cls, attribute_container_class):
-    """Registers a attribute container class.
+    """Registers an attribute container class.
 
     The attribute container classes are identified based on their lower case
     container type.
 
     Args:
       attribute_container_class (type): attribute container class.
```

### Comparing `acstore-20230325/acstore/fake_store.py` & `acstore-20230519/acstore/fake_store.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/acstore/helpers/schema.py` & `acstore-20230519/acstore/helpers/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       'bool': None,
       'int': None,
       'str': None,
       'timestamp': None}
 
   @classmethod
   def DeregisterDataType(cls, data_type):
-    """Deregisters an data type.
+    """Deregisters a data type.
 
     Args:
       data_type (str): data type.
 
     Raises:
       KeyError: if the data type is not set.
     """
```

### Comparing `acstore-20230325/acstore/helpers/yaml_definitions_file.py` & `acstore-20230519/acstore/helpers/yaml_definitions_file.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/acstore/interface.py` & `acstore-20230519/acstore/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/acstore/profilers.py` & `acstore-20230519/acstore/profilers.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/acstore/sqlite_store.py` & `acstore-20230519/acstore/sqlite_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
   def _CacheAttributeContainerForWrite(
       self, container_type, column_names, values):
     """Caches an attribute container for writing.
 
     Args:
       container_type (str): attribute container type.
       column_names (list[str]): names of the columns.
-      values (list[str]): values for each of the colums.
+      values (list[str]): values for each of the columns.
     """
     write_cache = self._write_cache.get(container_type, [column_names])
     write_cache.append(values)
 
     if len(write_cache) >= self._MAXIMUM_WRITE_CACHE_SIZE:
       self._FlushWriteCache(container_type, write_cache)
       write_cache = [column_names]
@@ -345,15 +345,15 @@
     try:
       self._cursor.execute(query)
     except (sqlite3.InterfaceError, sqlite3.OperationalError) as exception:
       raise IOError((
           f'Unable to query attribute container store with error: '
           f'{exception!s}'))
 
-  def _CreatetAttributeContainerFromRow(
+  def _CreateAttributeContainerFromRow(
       self, container_type, column_names, row, first_column_index):
     """Creates an attribute container of a row in the database.
 
     Args:
       container_type (str): attribute container type.
       column_names (list[str]): names of the columns selected.
       row (sqlite.Row): row as a result from a SELECT query.
@@ -492,15 +492,15 @@
         row = cursor.fetchone()
 
       finally:
         if self._storage_profiler:
           self._storage_profiler.StopTiming('get_containers')
 
       while row:
-        container = self._CreatetAttributeContainerFromRow(
+        container = self._CreateAttributeContainerFromRow(
             container_type, column_names, row, 1)
 
         identifier = containers_interface.AttributeContainerIdentifier(
             name=container_type, sequence_number=row[0])
         container.SetIdentifier(identifier)
 
         yield container
@@ -919,15 +919,15 @@
     finally:
       if self._storage_profiler:
         self._storage_profiler.StopTiming('get_container_by_index')
 
     if not row:
       return None
 
-    container = self._CreatetAttributeContainerFromRow(
+    container = self._CreateAttributeContainerFromRow(
         container_type, column_names, row, 0)
 
     identifier = containers_interface.AttributeContainerIdentifier(
         name=container_type, sequence_number=row_number)
     container.SetIdentifier(identifier)
 
     self._CacheAttributeContainerByIndex(container, index)
```

### Comparing `acstore-20230325/acstore.egg-info/PKG-INFO` & `acstore-20230519/acstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acstore
-Version: 20230325
+Version: 20230519
 Summary: Attribute Container Storage (ACStore).
 Home-page: https://github.com/log2timeline/acstore
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: 
 Classifier: Environment :: Console
```

### Comparing `acstore-20230325/acstore.egg-info/SOURCES.txt` & `acstore-20230519/acstore.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .pylintrc
 .style.yapf
+.yamllint.yaml
 ACKNOWLEDGEMENTS
 AUTHORS
 LICENSE
 MANIFEST.in
 README
 acstore.ini
 appveyor.yml
```

### Comparing `acstore-20230325/appveyor.yml` & `acstore-20230519/appveyor.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 environment:
   matrix:
-  - DESCRIPTION: "Windows with 32-bit Python 3.10"
+  - DESCRIPTION: "Windows with 32-bit Python 3.11"
     MACHINE_TYPE: "x86"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
-  - DESCRIPTION: "Windows with 64-bit Python 3.10"
+  - DESCRIPTION: "Windows with 64-bit Python 3.11"
     MACHINE_TYPE: "amd64"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310-x64"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311-x64"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
   - DESCRIPTION: "Mac OS with Python 3.11"
     APPVEYOR_BUILD_WORKER_IMAGE: macos-monterey
     HOMEBREW_NO_INSTALL_CLEANUP: 1
 
 install:
 - cmd: "%PYTHON%\\python.exe -m pip install -U pip setuptools twine wheel"
```

### Comparing `acstore-20230325/config/appveyor/install.ps1` & `acstore-20230519/config/appveyor/install.ps1`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Script to set up tests on AppVeyor Windows.
 
 $Dependencies = "PyYAML"
-$Dependencies = ${Dependencies} -split " "
 
-$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1"
-Write-Host (${Output} | Out-String)
-
-If ($env:APPVEYOR_REPO_BRANCH -eq "main")
-{
-	$Track = "stable"
-}
-Else
+If ($Dependencies.Length -gt 0)
 {
-	$Track = $env:APPVEYOR_REPO_BRANCH
-}
-New-Item -ItemType "directory" -Name "dependencies"
+	$Dependencies = ${Dependencies} -split " "
 
-$env:PYTHONPATH = "..\l2tdevtools"
+	$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
 
-$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1"
-Write-Host (${Output} | Out-String)
+	If ($env:APPVEYOR_REPO_BRANCH -eq "main")
+	{
+		$Track = "stable"
+	}
+	Else
+	{
+		$Track = $env:APPVEYOR_REPO_BRANCH
+	}
+	New-Item -ItemType "directory" -Name "dependencies"
+
+	$env:PYTHONPATH = "..\l2tdevtools"
+
+	$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
+}
```

### Comparing `acstore-20230325/config/appveyor/runtests.sh` & `acstore-20230519/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `acstore-20230325/config/dpkg/control` & `acstore-20230519/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `acstore-20230325/config/dpkg/copyright` & `acstore-20230519/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `acstore-20230325/docs/conf.py` & `acstore-20230519/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 # pylint: disable=unused-argument
 def RunSphinxAPIDoc(app):
   """Runs sphinx-apidoc to auto-generate documentation.
 
   Args:
     app (sphinx.application.Sphinx): Sphinx application. Required by the
-        the Sphinx event callback API.
+        Sphinx event callback API.
   """
   current_directory = os.path.abspath(os.path.dirname(__file__))
   module_path = os.path.join(current_directory, '..', 'acstore')
   api_directory = os.path.join(current_directory, 'sources', 'api')
   apidoc.main(['-o', api_directory, module_path, '--force'])
```

### Comparing `acstore-20230325/docs/sources/api/acstore.containers.rst` & `acstore-20230519/docs/sources/api/acstore.containers.rst`

 * *Files identical despite different names*

### Comparing `acstore-20230325/docs/sources/api/acstore.helpers.rst` & `acstore-20230519/docs/sources/api/acstore.helpers.rst`

 * *Files identical despite different names*

### Comparing `acstore-20230325/docs/sources/api/acstore.rst` & `acstore-20230519/docs/sources/api/acstore.rst`

 * *Files identical despite different names*

### Comparing `acstore-20230325/docs/sources/user/Installation-instructions.md` & `acstore-20230519/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `acstore-20230325/run_tests.py` & `acstore-20230519/run_tests.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/setup.py` & `acstore-20230519/setup.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/tests/containers/interface.py` & `acstore-20230519/tests/containers/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
     expected_attribute_names = ['attribute_name', 'attribute_value']
 
     attribute_names = sorted(attribute_container.GetAttributeNames())
 
     self.assertEqual(attribute_names, expected_attribute_names)
 
-    attribute_container._SERIALIZABLE_PROTECTED_ATTRIBUTES = [
-        '_protected_attribute']
+    setattr(attribute_container, '_SERIALIZABLE_PROTECTED_ATTRIBUTES', [
+        '_protected_attribute'])
 
     expected_attribute_names = [
         '_protected_attribute', 'attribute_name', 'attribute_value']
 
     attribute_names = sorted(attribute_container.GetAttributeNames())
 
     self.assertEqual(attribute_names, expected_attribute_names)
@@ -77,16 +77,16 @@
         ('attribute_name', 'attribute_name'),
         ('attribute_value', 'attribute_value')]
 
     attributes = sorted(attribute_container.GetAttributes())
 
     self.assertEqual(attributes, expected_attributes)
 
-    attribute_container._SERIALIZABLE_PROTECTED_ATTRIBUTES = [
-        '_protected_attribute']
+    setattr(attribute_container, '_SERIALIZABLE_PROTECTED_ATTRIBUTES', [
+        '_protected_attribute'])
 
     expected_attributes = [
         ('_protected_attribute', 'protected'),
         ('attribute_name', 'attribute_name'),
         ('attribute_value', 'attribute_value')]
 
     attributes = sorted(attribute_container.GetAttributes())
@@ -106,16 +106,16 @@
 
     attribute_values_hash2 = attribute_container.GetAttributeValuesHash()
 
     self.assertNotEqual(attribute_values_hash1, attribute_values_hash2)
 
     attribute_container.attribute_value = 'attribute_value'
 
-    attribute_container._SERIALIZABLE_PROTECTED_ATTRIBUTES = [
-        '_protected_attribute']
+    setattr(attribute_container, '_SERIALIZABLE_PROTECTED_ATTRIBUTES', [
+        '_protected_attribute'])
 
     attribute_values_hash2 = attribute_container.GetAttributeValuesHash()
 
     self.assertNotEqual(attribute_values_hash1, attribute_values_hash2)
 
   def testGetAttributeValuesString(self):
     """Tests the GetAttributeValuesString function."""
@@ -130,16 +130,16 @@
 
     attribute_values_string2 = attribute_container.GetAttributeValuesString()
 
     self.assertNotEqual(attribute_values_string1, attribute_values_string2)
 
     attribute_container.attribute_value = 'attribute_value'
 
-    attribute_container._SERIALIZABLE_PROTECTED_ATTRIBUTES = [
-        '_protected_attribute']
+    setattr(attribute_container, '_SERIALIZABLE_PROTECTED_ATTRIBUTES', [
+        '_protected_attribute'])
 
     attribute_values_string2 = attribute_container.GetAttributeValuesString()
 
     self.assertNotEqual(attribute_values_string1, attribute_values_string2)
 
   def testGetIdentifier(self):
     """Tests the GetIdentifier function."""
```

### Comparing `acstore-20230325/tests/containers/manager.py` & `acstore-20230519/tests/containers/manager.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/tests/fake_store.py` & `acstore-20230519/tests/fake_store.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/tests/helpers/schema.py` & `acstore-20230519/tests/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/tests/helpers/yaml_definitions_file.py` & `acstore-20230519/tests/helpers/yaml_definitions_file.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/tests/interface.py` & `acstore-20230519/tests/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/tests/profilers.py` & `acstore-20230519/tests/profilers.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
   def testStartStop(self):
     """Tests the Start and Stop functions."""
     with test_lib.TempDirectory() as temp_directory:
       test_profiler = profilers.StorageProfiler(
           'test', temp_directory)
 
-      test_profiler._FILENAME_PREFIX = 'test'
-      test_profiler._FILE_HEADER = 'test'
+      setattr(test_profiler, '_FILENAME_PREFIX', 'test')
+      setattr(test_profiler, '_FILE_HEADER', 'test')
 
       test_profiler.Start()
 
       test_profiler.Stop()
 
   def testSample(self):
     """Tests the Sample function."""
```

### Comparing `acstore-20230325/tests/sqlite_store.py` & `acstore-20230519/tests/sqlite_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         with self.assertRaises(IOError):
           test_store._CreateAttributeContainerTable(
               attribute_container.CONTAINER_TYPE)
 
       finally:
         test_store.Close()
 
-  # TODO: add tests for _CreatetAttributeContainerFromRow
+  # TODO: add tests for _CreateAttributeContainerFromRow
   # TODO: add tests for _Flush
   # TODO: add tests for _FlushWriteCache
 
   def testGetAttributeContainersWithFilter(self):
     """Tests the _GetAttributeContainersWithFilter function."""
     attribute_container = test_lib.TestAttributeContainer()
     attribute_container.attribute = '8f0bf95a7959baad9666b21a7feed79d'
```

### Comparing `acstore-20230325/tests/test_lib.py` & `acstore-20230519/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/utils/dependencies.py` & `acstore-20230519/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `acstore-20230325/utils/update_release.sh` & `acstore-20230519/utils/update_release.sh`

 * *Files identical despite different names*

