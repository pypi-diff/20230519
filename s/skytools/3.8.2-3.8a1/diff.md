# Comparing `tmp/skytools-3.8.2.tar.gz` & `tmp/skytools-3.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytools-3.8.2.tar", last modified: Fri May 19 13:22:59 2023, max compression
+gzip compressed data, was "skytools-3.8a1.tar", last modified: Mon Jul 11 13:39:18 2022, max compression
```

## Comparing `skytools-3.8.2.tar` & `skytools-3.8a1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:22:59.290588 skytools-3.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-19 13:22:56.000000 skytools-3.8.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)    15738 2023-05-19 13:22:56.000000 skytools-3.8.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-19 13:22:56.000000 skytools-3.8.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-19 13:22:56.000000 skytools-3.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-19 13:22:56.000000 skytools-3.8.2/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-19 13:22:59.290588 skytools-3.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-19 13:22:56.000000 skytools-3.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:22:59.282588 skytools-3.8.2/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-05-19 13:22:56.000000 skytools-3.8.2/modules/cquoting.c
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-19 13:22:56.000000 skytools-3.8.2/modules/get_buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-05-19 13:22:56.000000 skytools-3.8.2/modules/hashtext.c
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-19 13:22:59.290588 skytools-3.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-19 13:22:56.000000 skytools-3.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:22:59.286588 skytools-3.8.2/skytools/
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/_chashtext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/_cquoting.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/_pyquoting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/adminscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/apipkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/dbservice.py
--rw-r--r--   0 runner    (1001) docker     (123)    24085 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/dbstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/fileutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/gzlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/hashtext.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/installer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/natsort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/plpy_applyrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/psycopgwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/querybuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/quoting.py
--rw-r--r--   0 runner    (1001) docker     (123)    41583 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10928 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/skylog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/sockutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    20037 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/sqltools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/timeutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/tnetstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-19 13:22:56.000000 skytools-3.8.2/skytools/utf8.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:22:59.286588 skytools-3.8.2/skytools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-19 13:22:59.000000 skytools-3.8.2/skytools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-19 13:22:59.000000 skytools-3.8.2/skytools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:22:59.000000 skytools-3.8.2/skytools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:22:59.000000 skytools-3.8.2/skytools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 13:22:59.000000 skytools-3.8.2/skytools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:22:59.290588 skytools-3.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/config2.ini
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_dbservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_fileutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_gzlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_hashtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_kwcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_natsort.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_querybuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_quoting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_skylog.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_sockutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_sqltools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_timeutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_tnetstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 13:22:56.000000 skytools-3.8.2/tests/test_utf8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-19 13:22:56.000000 skytools-3.8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:39:18.065624 skytools-3.8a1/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-07-11 13:39:14.000000 skytools-3.8a1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)    15688 2022-07-11 13:39:14.000000 skytools-3.8a1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-07-11 13:39:14.000000 skytools-3.8a1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-07-11 13:39:14.000000 skytools-3.8a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3269 2022-07-11 13:39:14.000000 skytools-3.8a1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-07-11 13:39:18.065624 skytools-3.8a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-07-11 13:39:14.000000 skytools-3.8a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:39:18.057623 skytools-3.8a1/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)    16418 2022-07-11 13:39:14.000000 skytools-3.8a1/modules/cquoting.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-07-11 13:39:14.000000 skytools-3.8a1/modules/get_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8198 2022-07-11 13:39:14.000000 skytools-3.8a1/modules/hashtext.c
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-11 13:39:18.069624 skytools-3.8a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-07-11 13:39:14.000000 skytools-3.8a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:39:18.061623 skytools-3.8a1/skytools/
+-rw-r--r--   0 runner    (1001) docker     (121)     8009 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/_chashtext.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/_cquoting.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4938 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/_pyquoting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/adminscript.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6723 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/apipkg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22316 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/checker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12653 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23959 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/dbservice.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24085 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/dbstruct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4536 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/fileutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/gzlog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3634 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/hashtext.py
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/installer_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/natsort.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14604 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6603 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/plpy_applyrow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/psycopgwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    12676 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/querybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5797 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/quoting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41563 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10928 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/skylog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3832 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/sockutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20022 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/sqltools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3711 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/timeutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/tnetstrings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-07-11 13:39:14.000000 skytools-3.8a1/skytools/utf8.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:39:18.065624 skytools-3.8a1/skytools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-07-11 13:39:17.000000 skytools-3.8a1/skytools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-07-11 13:39:18.000000 skytools-3.8a1/skytools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 13:39:17.000000 skytools-3.8a1/skytools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 13:39:17.000000 skytools-3.8a1/skytools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-11 13:39:17.000000 skytools-3.8a1/skytools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 13:39:18.065624 skytools-3.8a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/config.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/config2.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5835 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_dbservice.py
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_fileutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_gzlog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2449 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_hashtext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_kwcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_natsort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7298 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_querybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8047 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_quoting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_skylog.py
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_sockutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_sqltools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_timeutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_tnetstrings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-07-11 13:39:14.000000 skytools-3.8a1/tests/test_utf8.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-07-11 13:39:14.000000 skytools-3.8a1/tox.ini
```

### Comparing `skytools-3.8.2/.pylintrc` & `skytools-3.8a1/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 	unused-argument,
 	unused-variable,
 	using-constant-test,
 	useless-object-inheritance,
 	duplicate-code,
         singleton-comparison,
         consider-using-f-string,
-        broad-exception-raised,
 
 	arguments-differ,
 	multiple-statements,
 	len-as-condition,
 	chained-comparison,
 	unnecessary-pass,
 	cyclic-import,
@@ -511,9 +510,9 @@
 known-third-party=enchant
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "BaseException, Exception".
-overgeneral-exceptions=builtins.BaseException,
-                       builtins.Exception
+overgeneral-exceptions=BaseException,
+                       Exception
```

### Comparing `skytools-3.8.2/AUTHORS` & `skytools-3.8a1/AUTHORS`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/NEWS.rst` & `skytools-3.8a1/NEWS.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,14 @@
 
 NEWS
 ====
 
-Skytools 3.8.2 (2023-05-19)
+Skytools 3.8a1 (2022-07-11)
 ---------------------------
 
-Fixes:
-
-* scripting: restore tracking of failed work() state
-
-Skytools 3.8.1 (2022-11-21)
----------------------------
-
-Fixes:
-
-* full_copy: use ``ONLY`` when using filter query
-* test_scripting: support Python 3.11
-
-Skytools 3.8 (2022-07-11)
--------------------------
-
 Cleanups:
 
 * Lots of typing improvements
 * Refresh CI setup
 * Work around PyPy3.9 bug
 
 Skytools 3.7.3 (2021-08-03)
```

### Comparing `skytools-3.8.2/PKG-INFO` & `skytools-3.8a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytools
-Version: 3.8.2
+Version: 3.8a1
 Summary: Utilities for database scripts
 Home-page: https://github.com/pgq/python-skytools
 Maintainer: Marko Kreen
 Maintainer-email: markokr@gmail.com
 License: ISC
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `skytools-3.8.2/README.rst` & `skytools-3.8a1/README.rst`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/modules/cquoting.c` & `skytools-3.8a1/modules/cquoting.c`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/modules/get_buffer.h` & `skytools-3.8a1/modules/get_buffer.h`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/modules/hashtext.c` & `skytools-3.8a1/modules/hashtext.c`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/setup.py` & `skytools-3.8a1/setup.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/__init__.py` & `skytools-3.8a1/skytools/__init__.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/_pyquoting.py` & `skytools-3.8a1/skytools/_pyquoting.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/adminscript.py` & `skytools-3.8a1/skytools/adminscript.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/apipkg.py` & `skytools-3.8a1/skytools/apipkg.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/basetypes.py` & `skytools-3.8a1/skytools/basetypes.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/checker.py` & `skytools-3.8a1/skytools/checker.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/config.py` & `skytools-3.8a1/skytools/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,35 +129,35 @@
         if not self.cf.has_option(self.main_section, key):
             if default is None:
                 raise NoOptionError(key, self.main_section)
             return default
 
         return self.cf.getint(self.main_section, key)
 
-    def getboolean(self, key: str, default: Optional[bool] = None) -> bool:
+    def getboolean(self, key: str, default: bool = None) -> bool:
         """Reads boolean value, if not set then default."""
 
         if not self.cf.has_option(self.main_section, key):
             if default is None:
                 raise NoOptionError(key, self.main_section)
             return default
 
         return self.cf.getboolean(self.main_section, key)
 
-    def getfloat(self, key: str, default: Optional[float] = None) -> float:
+    def getfloat(self, key: str, default: float = None) -> float:
         """Reads float value, if not set then default."""
 
         if not self.cf.has_option(self.main_section, key):
             if default is None:
                 raise NoOptionError(key, self.main_section)
             return default
 
         return self.cf.getfloat(self.main_section, key)
 
-    def getlist(self, key: str, default: Optional[Sequence[str]] = None) -> Sequence[str]:
+    def getlist(self, key: str, default: Sequence[str] = None) -> Sequence[str]:
         """Reads comma-separated list from key."""
 
         if not self.cf.has_option(self.main_section, key):
             if default is None:
                 raise NoOptionError(key, self.main_section)
             return default
```

### Comparing `skytools-3.8.2/skytools/dbservice.py` & `skytools-3.8a1/skytools/dbservice.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/dbstruct.py` & `skytools-3.8a1/skytools/dbstruct.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/fileutil.py` & `skytools-3.8a1/skytools/fileutil.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/gzlog.py` & `skytools-3.8a1/skytools/gzlog.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/hashtext.py` & `skytools-3.8a1/skytools/hashtext.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/natsort.py` & `skytools-3.8a1/skytools/natsort.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/parsing.py` & `skytools-3.8a1/skytools/parsing.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/plpy_applyrow.py` & `skytools-3.8a1/skytools/plpy_applyrow.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/psycopgwrapper.py` & `skytools-3.8a1/skytools/psycopgwrapper.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/querybuilder.py` & `skytools-3.8a1/skytools/querybuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         args = self._params
         curs.execute(q, args)
 
 
 class PLPyQueryBuilder(QueryBuilderCore):
 
     def __init__(self, sqlexpr: str, params: Optional[Mapping[str, Any]],
-                 plan_cache: Optional[Dict[str, Any]] = None,
+                 plan_cache: Dict[str, Any] = None,
                  sqls: Optional[List[Dict[str, str]]] = None):
         """Init the object.
 
         @param sqlexpr:     Partial sql fragment.
         @param params:      Dict of parameter values.
         @param plan_cache:  (PL/Python) A dict object where to store the plan cache, under the key C{"plan_cache"}.
                             If not given, plan will not be cached and values will be inserted directly
```

### Comparing `skytools-3.8.2/skytools/quoting.py` & `skytools-3.8a1/skytools/quoting.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/scripting.py` & `skytools-3.8a1/skytools/scripting.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,15 @@
             work = self.run_once()
 
             if not self.looping or self.loop_delay < 0:
                 break
 
             # remember work state
             if work:
-                self.work_state = 1 if work > 0 else -1
+                self.work_state = 1
             else:
                 self.work_state = 0
             # should sleep?
             if not work:
                 if self.loop_delay > 0:
                     self.sleep(self.loop_delay)
                     if not self.looping:
```

### Comparing `skytools-3.8.2/skytools/skylog.py` & `skytools-3.8a1/skytools/skylog.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/sockutil.py` & `skytools-3.8a1/skytools/sockutil.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/sqltools.py` & `skytools-3.8a1/skytools/sqltools.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
             qfields = build_qfields(cols)
             return "%s (%s)" % (qtable, qfields)
         else:
             return qtable
 
     dst = build_statement(dst_tablename, dst_column_list)
     if condition:
-        src = "(SELECT %s FROM ONLY %s WHERE %s)" % (build_qfields(column_list),
+        src = "(SELECT %s FROM %s WHERE %s)" % (build_qfields(column_list),
                                                 skytools.quote_fqident(tablename),
                                                 condition)
     else:
         src = build_statement(tablename, column_list)
 
     sql_to = "COPY %s TO stdout" % src
     sql_from = "COPY %s FROM stdin" % dst
@@ -634,15 +634,15 @@
                 col = skytools.quote_ident(col)
                 val = skytools.quote_literal(val)
                 set_list.append("%s = %s" % (col, val))
     return "update only %s set %s where %s;" % (skytools.quote_fqident(tbl),
                                                 ", ".join(set_list), " and ".join(whe_list))
 
 
-def mk_delete_sql(row: DictRow, tbl: str, pkey_list: Sequence[str], field_map: Optional[Mapping[str, str]] = None):
+def mk_delete_sql(row: DictRow, tbl: str, pkey_list: Sequence[str], field_map: Mapping[str, str] = None):
     """Generate DELETE statement from dict data.
     """
     if len(pkey_list) < 1:
         raise Exception("delete needs pkeys")
     whe_list = []
     for k in pkey_list:
         new_k = field_map and field_map[k] or k
```

### Comparing `skytools-3.8.2/skytools/timeutil.py` & `skytools-3.8a1/skytools/timeutil.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/tnetstrings.py` & `skytools-3.8a1/skytools/tnetstrings.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools/utf8.py` & `skytools-3.8a1/skytools/utf8.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/skytools.egg-info/PKG-INFO` & `skytools-3.8a1/skytools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytools
-Version: 3.8.2
+Version: 3.8a1
 Summary: Utilities for database scripts
 Home-page: https://github.com/pgq/python-skytools
 Maintainer: Marko Kreen
 Maintainer-email: markokr@gmail.com
 License: ISC
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `skytools-3.8.2/skytools.egg-info/SOURCES.txt` & `skytools-3.8a1/skytools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_config.py` & `skytools-3.8a1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_dbservice.py` & `skytools-3.8a1/tests/test_dbservice.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_gzlog.py` & `skytools-3.8a1/tests/test_gzlog.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_hashtext.py` & `skytools-3.8a1/tests/test_hashtext.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_kwcheck.py` & `skytools-3.8a1/tests/test_kwcheck.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_natsort.py` & `skytools-3.8a1/tests/test_natsort.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_parsing.py` & `skytools-3.8a1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_querybuilder.py` & `skytools-3.8a1/tests/test_querybuilder.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_quoting.py` & `skytools-3.8a1/tests/test_quoting.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_scripting.py` & `skytools-3.8a1/tests/test_scripting.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,43 +88,43 @@
 
 
 @pytest.mark.skipif(WIN32, reason="use signals on win32")
 def test_optparse_signals(capsys):
     with pytest.raises(SystemExit):
         OptScript("testscript", ["-s", CONF])
     res = capsys.readouterr()
-    assert "SIGINT" in res.out or f"signal: {signal.SIGINT}" in res.out
+    assert "SIGINT" in res.out
 
     with pytest.raises(SystemExit):
         OptScript("testscript", ["-r", CONF])
     res = capsys.readouterr()
-    assert "SIGHUP" in res.out or f"signal: {signal.SIGHUP}" in res.out
+    assert "SIGHUP" in res.out
 
     with pytest.raises(SystemExit):
         OptScript("testscript", ["-k", CONF])
     res = capsys.readouterr()
-    assert "SIGTERM" in res.out or f"signal: {signal.SIGTERM}" in res.out
+    assert "SIGTERM" in res.out
 
 
 @pytest.mark.skipif(WIN32, reason="need to use signals")
 def test_argparse_signals(capsys):
     with pytest.raises(SystemExit):
         ArgScript("testscript", ["-s", CONF])
     res = capsys.readouterr()
-    assert "SIGINT" in res.out or f"signal: {signal.SIGINT}" in res.out
+    assert "SIGINT" in res.out
 
     with pytest.raises(SystemExit):
         ArgScript("testscript", ["-r", CONF])
     res = capsys.readouterr()
-    assert "SIGHUP" in res.out or f"signal: {signal.SIGHUP}" in res.out
+    assert "SIGHUP" in res.out
 
     with pytest.raises(SystemExit):
         ArgScript("testscript", ["-k", CONF])
     res = capsys.readouterr()
-    assert "SIGTERM" in res.out or f"signal: {signal.SIGTERM}" in res.out
+    assert "SIGTERM" in res.out
 
 
 def test_optparse_confopt(capsys):
     s = ArgScript("testscript", [CONF])
     s.start()
     res = capsys.readouterr()
     assert "opt=test" in res.out
```

### Comparing `skytools-3.8.2/tests/test_sockutil.py` & `skytools-3.8a1/tests/test_sockutil.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_sqltools.py` & `skytools-3.8a1/tests/test_sqltools.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_timeutil.py` & `skytools-3.8a1/tests/test_timeutil.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_tnetstrings.py` & `skytools-3.8a1/tests/test_tnetstrings.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tests/test_utf8.py` & `skytools-3.8a1/tests/test_utf8.py`

 * *Files identical despite different names*

### Comparing `skytools-3.8.2/tox.ini` & `skytools-3.8a1/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 [tox]
 envlist = lint,xlint,py3
 
 [package]
 name = skytools
 deps =
-    psycopg2-binary==2.9.6
+    psycopg2-binary==2.9.3
 test_deps =
-    coverage==7.2.5
-    pytest==7.3.1
-    pytest-cov==4.0.0
+    coverage==6.4.1
+    pytest==7.1.2
+    pytest-cov==3.0.0
 lint_deps =
-    mypy==1.3.0
-    pylint==2.17.4
-    flake8==6.0.0
-    types-setuptools==65.6.0.0
+    mypy==0.961
+    pylint==2.14.4
+    flake8==4.0.1
+    types-setuptools==57.4.18
 doc_deps =
-    sphinx==7.0.1
-    docutils==0.20.1
+    sphinx==5.0.2
+    docutils==0.18.1
 
 [testenv]
 changedir = {toxinidir}
 deps =
     {[package]deps}
     {[package]test_deps}
 setenv =
```

