# Comparing `tmp/portforward-0.4.5.tar.gz` & `tmp/portforward-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portforward-0.4.5.tar", last modified: Mon Mar  6 16:18:59 2023, max compression
+gzip compressed data, was "portforward-0.5.0.tar", last modified: Fri May 19 18:42:14 2023, max compression
```

## Comparing `portforward-0.4.5.tar` & `portforward-0.5.0.tar`

### file list

```diff
@@ -1,82 +1,88 @@
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.565139 portforward-0.4.5/
--rw-rw-r--   0 corka     (1000) corka     (1000)      163 2022-12-26 21:23:31.000000 portforward-0.4.5/AUTHORS.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)     3987 2023-02-06 15:34:50.000000 portforward-0.4.5/CONTRIBUTING.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)     1939 2023-03-06 16:12:21.000000 portforward-0.4.5/HISTORY.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)     1075 2022-12-26 21:23:31.000000 portforward-0.4.5/LICENSE
--rw-rw-r--   0 corka     (1000) corka     (1000)      332 2022-12-26 21:23:31.000000 portforward-0.4.5/MANIFEST.in
--rw-rw-r--   0 corka     (1000) corka     (1000)     5720 2023-03-06 16:18:59.565139 portforward-0.4.5/PKG-INFO
--rw-rw-r--   0 corka     (1000) corka     (1000)     2946 2023-02-06 15:33:44.000000 portforward-0.4.5/README.rst
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.561139 portforward-0.4.5/docs/
--rw-rw-r--   0 corka     (1000) corka     (1000)      612 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/Makefile
--rw-rw-r--   0 corka     (1000) corka     (1000)       28 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/authors.rst
--rwxrwxr-x   0 corka     (1000) corka     (1000)     5249 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/conf.py
--rw-rw-r--   0 corka     (1000) corka     (1000)       33 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/contributing.rst
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.561139 portforward-0.4.5/docs/docs/
--rw-rw-r--   0 corka     (1000) corka     (1000)      103 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/docs/conf.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)       49 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/docs/modules.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)       28 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/history.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)      307 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/index.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)     1230 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/installation.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)      773 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/make.bat
--rw-rw-r--   0 corka     (1000) corka     (1000)       70 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/modules.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)      124 2022-12-26 21:23:31.000000 portforward-0.4.5/docs/portforward.rst
--rw-rw-r--   0 corka     (1000) corka     (1000)      186 2023-03-06 16:12:21.000000 portforward-0.4.5/go.mod
--rw-rw-r--   0 corka     (1000) corka     (1000)    47381 2023-02-28 20:50:55.000000 portforward-0.4.5/go.sum
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.561139 portforward-0.4.5/internal/
--rw-rw-r--   0 corka     (1000) corka     (1000)    10373 2023-03-06 16:12:21.000000 portforward-0.4.5/internal/portforward.go
--rw-rw-r--   0 corka     (1000) corka     (1000)     1029 2023-03-06 16:12:21.000000 portforward-0.4.5/internal/portforward_test.go
--rw-rw-r--   0 corka     (1000) corka     (1000)     2136 2022-12-26 21:23:31.000000 portforward-0.4.5/main.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     2076 2023-03-06 16:12:21.000000 portforward-0.4.5/main.go
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.561139 portforward-0.4.5/portforward.egg-info/
--rw-rw-r--   0 corka     (1000) corka     (1000)     5720 2023-03-06 16:18:59.000000 portforward-0.4.5/portforward.egg-info/PKG-INFO
--rw-rw-r--   0 corka     (1000) corka     (1000)     2266 2023-03-06 16:18:59.000000 portforward-0.4.5/portforward.egg-info/SOURCES.txt
--rw-rw-r--   0 corka     (1000) corka     (1000)        1 2023-03-06 16:18:59.000000 portforward-0.4.5/portforward.egg-info/dependency_links.txt
--rw-rw-r--   0 corka     (1000) corka     (1000)        1 2023-03-06 16:14:06.000000 portforward-0.4.5/portforward.egg-info/not-zip-safe
--rw-rw-r--   0 corka     (1000) corka     (1000)       25 2023-03-06 16:18:59.000000 portforward-0.4.5/portforward.egg-info/top_level.txt
--rw-rw-r--   0 corka     (1000) corka     (1000)     4010 2023-03-06 16:12:21.000000 portforward-0.4.5/portforward.py
--rw-rw-r--   0 corka     (1000) corka     (1000)      390 2023-03-06 16:18:59.565139 portforward-0.4.5/setup.cfg
--rw-rw-r--   0 corka     (1000) corka     (1000)     1625 2023-03-06 16:12:21.000000 portforward-0.4.5/setup.py
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.561139 portforward-0.4.5/tests/
--rw-rw-r--   0 corka     (1000) corka     (1000)      307 2022-12-26 21:23:31.000000 portforward-0.4.5/tests/conftest.py
--rw-rw-r--   0 corka     (1000) corka     (1000)     1563 2022-12-26 21:23:31.000000 portforward-0.4.5/tests/test_portforward.py
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.557139 portforward-0.4.5/venv/
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.557139 portforward-0.4.5/venv/lib/
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.557139 portforward-0.4.5/venv/lib/python3.10/
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.557139 portforward-0.4.5/venv/lib/python3.10/site-packages/
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.561139 portforward-0.4.5/venv/lib/python3.10/site-packages/markupsafe/
--rw-rw-r--   0 corka     (1000) corka     (1000)     7083 2023-01-29 13:21:17.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/markupsafe/_speedups.c
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.557139 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.561139 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/
--rw-rw-r--   0 corka     (1000) corka     (1000)     4915 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/bytes_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    12514 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/dict_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     8031 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/exc_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     1717 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/generic_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    15739 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/getargs.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    18911 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/getargsfast.c
--rw-rw-r--   0 corka     (1000) corka     (1000)      473 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/init.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    19814 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/int_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     9877 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/list_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    24894 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/misc_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)      351 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/set_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     8075 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/str_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     1985 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/tuple_ops.c
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.557139 portforward-0.4.5/venv/lib64/
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.557139 portforward-0.4.5/venv/lib64/python3.10/
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.557139 portforward-0.4.5/venv/lib64/python3.10/site-packages/
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.565139 portforward-0.4.5/venv/lib64/python3.10/site-packages/markupsafe/
--rw-rw-r--   0 corka     (1000) corka     (1000)     7083 2023-01-29 13:21:17.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/markupsafe/_speedups.c
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.557139 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/
-drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-03-06 16:18:59.565139 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/
--rw-rw-r--   0 corka     (1000) corka     (1000)     4915 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/bytes_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    12514 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/dict_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     8031 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/exc_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     1717 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/generic_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    15739 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/getargs.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    18911 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/getargsfast.c
--rw-rw-r--   0 corka     (1000) corka     (1000)      473 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/init.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    19814 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/int_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     9877 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/list_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)    24894 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/misc_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)      351 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/set_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     8075 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/str_ops.c
--rw-rw-r--   0 corka     (1000) corka     (1000)     1985 2023-01-29 13:21:18.000000 portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/tuple_ops.c
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.653746 portforward-0.5.0/
+-rw-rw-r--   0 corka     (1000) corka     (1000)      163 2023-04-12 18:49:21.000000 portforward-0.5.0/AUTHORS.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)     3987 2023-04-12 18:49:21.000000 portforward-0.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)     2094 2023-05-19 18:36:53.000000 portforward-0.5.0/HISTORY.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)     1075 2023-04-12 18:49:21.000000 portforward-0.5.0/LICENSE
+-rw-rw-r--   0 corka     (1000) corka     (1000)      332 2023-04-12 18:49:21.000000 portforward-0.5.0/MANIFEST.in
+-rw-rw-r--   0 corka     (1000) corka     (1000)     5875 2023-05-19 18:42:14.653746 portforward-0.5.0/PKG-INFO
+-rw-rw-r--   0 corka     (1000) corka     (1000)     2946 2023-04-12 18:49:21.000000 portforward-0.5.0/README.rst
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.649747 portforward-0.5.0/docs/
+-rw-rw-r--   0 corka     (1000) corka     (1000)      612 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/Makefile
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/docs/_build/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/docs/_build/html/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.649747 portforward-0.5.0/docs/_build/html/_static/
+-rw-rw-r--   0 corka     (1000) corka     (1000)      286 2023-05-10 05:30:47.000000 portforward-0.5.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 corka     (1000) corka     (1000)       90 2023-05-10 05:30:47.000000 portforward-0.5.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 corka     (1000) corka     (1000)       90 2023-05-10 05:30:47.000000 portforward-0.5.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 corka     (1000) corka     (1000)       28 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/authors.rst
+-rwxrwxr-x   0 corka     (1000) corka     (1000)     5249 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/conf.py
+-rw-rw-r--   0 corka     (1000) corka     (1000)       33 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/contributing.rst
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.649747 portforward-0.5.0/docs/docs/
+-rw-rw-r--   0 corka     (1000) corka     (1000)      103 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/docs/conf.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)       49 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/docs/modules.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)       28 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/history.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)      307 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/index.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)     1230 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/installation.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)      773 2023-04-12 18:49:22.000000 portforward-0.5.0/docs/make.bat
+-rw-rw-r--   0 corka     (1000) corka     (1000)       76 2023-05-19 18:37:09.000000 portforward-0.5.0/docs/modules.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)      121 2023-05-19 18:37:09.000000 portforward-0.5.0/docs/portforward.rst
+-rw-rw-r--   0 corka     (1000) corka     (1000)      186 2023-04-12 18:49:21.000000 portforward-0.5.0/go.mod
+-rw-rw-r--   0 corka     (1000) corka     (1000)    47381 2023-04-12 18:49:21.000000 portforward-0.5.0/go.sum
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.649747 portforward-0.5.0/internal/
+-rw-rw-r--   0 corka     (1000) corka     (1000)    11646 2023-05-19 18:34:33.000000 portforward-0.5.0/internal/portforward.go
+-rw-rw-r--   0 corka     (1000) corka     (1000)     2149 2023-05-19 18:34:33.000000 portforward-0.5.0/main.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     2135 2023-05-19 18:34:33.000000 portforward-0.5.0/main.go
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.649747 portforward-0.5.0/portforward.egg-info/
+-rw-rw-r--   0 corka     (1000) corka     (1000)     5875 2023-05-19 18:42:14.000000 portforward-0.5.0/portforward.egg-info/PKG-INFO
+-rw-rw-r--   0 corka     (1000) corka     (1000)     2361 2023-05-19 18:42:14.000000 portforward-0.5.0/portforward.egg-info/SOURCES.txt
+-rw-rw-r--   0 corka     (1000) corka     (1000)        1 2023-05-19 18:42:14.000000 portforward-0.5.0/portforward.egg-info/dependency_links.txt
+-rw-rw-r--   0 corka     (1000) corka     (1000)        1 2023-05-19 18:38:10.000000 portforward-0.5.0/portforward.egg-info/not-zip-safe
+-rw-rw-r--   0 corka     (1000) corka     (1000)       25 2023-05-19 18:42:14.000000 portforward-0.5.0/portforward.egg-info/top_level.txt
+-rw-rw-r--   0 corka     (1000) corka     (1000)     5283 2023-05-19 18:37:52.000000 portforward-0.5.0/portforward.py
+-rw-rw-r--   0 corka     (1000) corka     (1000)      345 2023-05-19 18:42:14.653746 portforward-0.5.0/setup.cfg
+-rw-rw-r--   0 corka     (1000) corka     (1000)     1625 2023-05-19 18:37:52.000000 portforward-0.5.0/setup.py
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.649747 portforward-0.5.0/tests/
+-rw-rw-r--   0 corka     (1000) corka     (1000)        0 2023-05-17 05:16:22.000000 portforward-0.5.0/tests/conftest.py
+-rw-rw-r--   0 corka     (1000) corka     (1000)     1097 2023-05-19 18:34:33.000000 portforward-0.5.0/tests/resources.yaml
+-rw-rw-r--   0 corka     (1000) corka     (1000)     5548 2023-05-19 18:34:33.000000 portforward-0.5.0/tests/test_portforward.py
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/venv/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/venv/lib/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/venv/lib/python3.10/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/venv/lib/python3.10/site-packages/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.649747 portforward-0.5.0/venv/lib/python3.10/site-packages/markupsafe/
+-rw-rw-r--   0 corka     (1000) corka     (1000)     7083 2023-05-10 05:30:45.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/markupsafe/_speedups.c
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.653746 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/
+-rw-rw-r--   0 corka     (1000) corka     (1000)     4915 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/bytes_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    12514 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/dict_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     8031 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/exc_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     1717 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/generic_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    15739 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/getargs.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    18911 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/getargsfast.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)      473 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/init.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    19814 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/int_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     9877 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/list_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    24894 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/misc_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)      351 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/set_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     8075 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/str_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     1985 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/tuple_ops.c
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/venv/lib64/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/venv/lib64/python3.10/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/venv/lib64/python3.10/site-packages/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.653746 portforward-0.5.0/venv/lib64/python3.10/site-packages/markupsafe/
+-rw-rw-r--   0 corka     (1000) corka     (1000)     7083 2023-05-10 05:30:45.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/markupsafe/_speedups.c
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.645747 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/
+drwxrwxr-x   0 corka     (1000) corka     (1000)        0 2023-05-19 18:42:14.653746 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/
+-rw-rw-r--   0 corka     (1000) corka     (1000)     4915 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/bytes_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    12514 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/dict_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     8031 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/exc_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     1717 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/generic_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    15739 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/getargs.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    18911 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/getargsfast.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)      473 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/init.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    19814 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/int_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     9877 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/list_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)    24894 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/misc_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)      351 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/set_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     8075 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/str_ops.c
+-rw-rw-r--   0 corka     (1000) corka     (1000)     1985 2023-05-10 05:30:46.000000 portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/tuple_ops.c
```

### Comparing `portforward-0.4.5/CONTRIBUTING.rst` & `portforward-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/HISTORY.rst` & `portforward-0.5.0/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 =======
 History
 =======
 
-unreleased
-----------
+0.5.0 (2023-05-19)
+------------------
 * Move pytogo Go code into portforward
+* Fix stopping portforward for services
+* Allow portforwarding without contextmanager
+* Allow multiple portforwards to same pod or service
 
 0.4.5 (2023-03-06)
 ------------------
 * Fix panic when logging an error
 * Change default log level to INFO
 
 0.4.4 (2023-02-28)
```

### Comparing `portforward-0.4.5/LICENSE` & `portforward-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/PKG-INFO` & `portforward-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portforward
-Version: 0.4.5
+Version: 0.5.0
 Summary: Kubernetes Port-Forward Go-Edition For Python 
 Home-page: https://github.com/pytogo/portforward
 Author: Sebastian Ziemann
 Author-email: corka149@mailbox.org
 License: MIT license
 Keywords: portforward
 Platform: UNKNOWN
@@ -145,17 +145,20 @@
 .. _setuptools-golang: https://github.com/asottile/setuptools-golang
 
 
 =======
 History
 =======
 
-unreleased
-----------
+0.5.0 (2023-05-19)
+------------------
 * Move pytogo Go code into portforward
+* Fix stopping portforward for services
+* Allow portforwarding without contextmanager
+* Allow multiple portforwards to same pod or service
 
 0.4.5 (2023-03-06)
 ------------------
 * Fix panic when logging an error
 * Change default log level to INFO
 
 0.4.4 (2023-02-28)
```

### Comparing `portforward-0.4.5/README.rst` & `portforward-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/docs/Makefile` & `portforward-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/docs/conf.py` & `portforward-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/docs/installation.rst` & `portforward-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/docs/make.bat` & `portforward-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/go.sum` & `portforward-0.5.0/go.sum`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/internal/portforward.go` & `portforward-0.5.0/internal/portforward.go`

 * *Files 5% similar despite different names*

```diff
@@ -41,42 +41,72 @@
 Global states are bad but should any reference to memory exists in
 the Python and Go space? Who should when free the memory?
 
 Every space should keep the ownership of its memory allocations.
 Parameters are passed from Python to Go but Go never owns them.
 */
 var (
-	activeForwards = make(map[string]chan struct{})
-	mutex          sync.Mutex
+	activeForwards  = make(map[string]chan struct{})
+	podsForServices = make(map[string]string)
+	mutex           sync.Mutex
 )
 
 // registerForwarding adds a forwarding to the active forwards.
-func registerForwarding(namespace, podOrService string, stopCh chan struct{}) {
-	key := fmt.Sprintf("%s/%s", namespace, podOrService)
+func registerForwarding(namespace, pod, podOrService string, toPort int, stopCh chan struct{}) {
+	key := fmt.Sprintf("%s/%s/%d", namespace, pod, toPort)
+	debugPortforward(fmt.Sprintf("Register pod key %s", key))
 
 	mutex.Lock()
 	defer mutex.Unlock()
 
 	if otherCh, ok := activeForwards[key]; ok {
 		close(otherCh)
 	}
 
+	// When they are not equal then we received a service name.
+	if pod != podOrService {
+		serviceKey := fmt.Sprintf("%s/%s/%d", namespace, podOrService, toPort)
+		debugPortforward(fmt.Sprintf("Register service key %s with %s", serviceKey, pod))
+		podsForServices[serviceKey] = pod
+	}
+
 	activeForwards[key] = stopCh
 }
 
 // StopForwarding closes a port forwarding.
-func StopForwarding(namespace, podOrService string) {
-	key := fmt.Sprintf("%s/%s", namespace, podOrService)
+func StopForwarding(namespace, podOrService string, toPort int) {
+	key := fmt.Sprintf("%s/%s/%d", namespace, podOrService, toPort)
+	debugPortforward(fmt.Sprintf("Look up pod key %s", key))
 
 	mutex.Lock()
 	defer mutex.Unlock()
 
-	if otherCh, ok := activeForwards[key]; ok {
-		close(otherCh)
+	if stopChannel, ok := activeForwards[key]; ok {
+		close(stopChannel)
 		delete(activeForwards, key)
+		debugPortforward(fmt.Sprintf("Stopped forward for key %s", key))
+	}
+
+	// We did not find a stopChannel. Was it maybe a service
+	// and was registered with the actual target pod name?
+
+	serviceKey := fmt.Sprintf("%s/%s/%d", namespace, podOrService, toPort)
+	debugPortforward(fmt.Sprintf("Look up service key %s", serviceKey))
+
+	if podForService, ok := podsForServices[serviceKey]; ok {
+		key = fmt.Sprintf("%s/%s/%d", namespace, podForService, toPort)
+		debugPortforward(fmt.Sprintf("Look up pod key %s", key))
+
+		if stopChannel, ok := activeForwards[key]; ok {
+			close(stopChannel)
+			delete(activeForwards, key)
+			debugPortforward(fmt.Sprintf("Stopped forward for key %s", key))
+		}
+
+		delete(podsForServices, serviceKey)
 	}
 }
 
 // ===== Port forwarding =====
 
 // Forward connects to a pod/service and tunnels traffic from a local port to this pod.
 func Forward(namespace, podOrService string, fromPort, toPort int, configPath string, logLevel int, kubeContext string) error {
@@ -122,16 +152,16 @@
 	ports := fmt.Sprintf("%d:%d", fromPort, toPort)
 
 	if err = startForward(dialer, ports, stopChan, readyChan, log); err != nil {
 		return err
 	}
 
 	// HANDLE CLOSING
-	registerForwarding(namespace, pod.Name, stopChan)
-	closeOnSigterm(namespace, pod.Name)
+	registerForwarding(namespace, pod.Name, podOrService, toPort, stopChan)
+	closeOnSigterm(namespace, pod.Name, toPort)
 
 	return nil
 }
 
 // loadConfig fetches the config from .kube config folder inside the home dir.
 // It tries to load in-cluster-config when an empty path was provided.
 func loadConfig(kubeconfigPath string, kubeContext string, log logger) (*rest.Config, error) {
@@ -337,24 +367,24 @@
 		err = nil
 	}
 
 	return err
 }
 
 // closeOnSigterm cares about closing a channel when the OS sends a SIGTERM.
-func closeOnSigterm(namespace, qualifiedName string) {
+func closeOnSigterm(namespace, qualifiedName string, toPort int) {
 	sigs := make(chan os.Signal, 1)
 
 	signal.Notify(sigs, syscall.SIGINT, syscall.SIGTERM)
 
 	go func() {
 		// Received kill signal
 		<-sigs
 
-		StopForwarding(namespace, qualifiedName)
+		StopForwarding(namespace, qualifiedName, toPort)
 	}()
 }
 
 func overwriteLog(log logger) {
 	if !log.isOff() {
 		return
 	}
```

### Comparing `portforward-0.4.5/main.c` & `portforward-0.5.0/main.c`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 > won’t have to release any memory yourself. The only
 > exceptions are es, es#, et and et#.
 */
 int PyArg_ParseTuple_ssiisis(PyObject* args, char** a, char** b, int* c, int* d, char** e, int* f, char** g) {
     return PyArg_ParseTuple(args, "ssiisis", a, b, c, d, e, f, g);
 }
 
-int PyArg_ParseTuple_ss(PyObject* args, char** a, char** b) {
-    return PyArg_ParseTuple(args, "ss", a, b);
+int PyArg_ParseTuple_ssi(PyObject* args, char** a, char** b, int* c) {
+    return PyArg_ParseTuple(args, "ssi", a, b, c);
 }
 
 static struct PyMethodDef methods[] = {
     {
     "forward",
     (PyCFunction)forward,
     METH_VARARGS,
```

### Comparing `portforward-0.4.5/main.go` & `portforward-0.5.0/main.go`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 package main
 
 // #include <Python.h>
 // int PyArg_ParseTuple_ssiisis(PyObject* args, char** a, char** b, int* c, int* d, char** e, int* f, char** g);
-// int PyArg_ParseTuple_ss(PyObject*, char**, char**);
+// int PyArg_ParseTuple_ssi(PyObject* args, char** a, char** b, int* c);
 // void raise_exception(char *msg);
 import "C"
 
 import (
 	"github.com/pytogo/portforward/internal"
 )
 
@@ -55,23 +55,24 @@
 	// Interface for C extension and only part that contains C.
 
 	// Strings should not need to be freed
 	// > A pointer to an existing string is stored in the character pointer variable whose address you pass.
 	// https://docs.python.org/3/c-api/arg.html
 	var namespace *C.char
 	var podName *C.char
+	var toPort C.int
 
-	if C.PyArg_ParseTuple_ss(args, &namespace, &podName) == 0 {
+	if C.PyArg_ParseTuple_ssi(args, &namespace, &podName, &toPort) == 0 {
 		C.raise_exception(C.CString("Could not parse args"))
 		return nil
 	}
 
 	var ns string = C.GoString(namespace)
 	var pod string = C.GoString(podName)
 
-	internal.StopForwarding(ns, pod)
+	internal.StopForwarding(ns, pod, int(toPort))
 
 	C.Py_IncRef(C.Py_None)
 	return C.Py_None
 }
 
 func main() {}
```

### Comparing `portforward-0.4.5/portforward.egg-info/PKG-INFO` & `portforward-0.5.0/portforward.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portforward
-Version: 0.4.5
+Version: 0.5.0
 Summary: Kubernetes Port-Forward Go-Edition For Python 
 Home-page: https://github.com/pytogo/portforward
 Author: Sebastian Ziemann
 Author-email: corka149@mailbox.org
 License: MIT license
 Keywords: portforward
 Platform: UNKNOWN
@@ -145,17 +145,20 @@
 .. _setuptools-golang: https://github.com/asottile/setuptools-golang
 
 
 =======
 History
 =======
 
-unreleased
-----------
+0.5.0 (2023-05-19)
+------------------
 * Move pytogo Go code into portforward
+* Fix stopping portforward for services
+* Allow portforwarding without contextmanager
+* Allow multiple portforwards to same pod or service
 
 0.4.5 (2023-03-06)
 ------------------
 * Fix panic when logging an error
 * Change default log level to INFO
 
 0.4.4 (2023-02-28)
```

### Comparing `portforward-0.4.5/portforward.egg-info/SOURCES.txt` & `portforward-0.5.0/portforward.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,27 @@
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/portforward.rst
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
 docs/docs/conf.rst
 docs/docs/modules.rst
 internal/portforward.go
-internal/portforward_test.go
 portforward.egg-info/PKG-INFO
 portforward.egg-info/SOURCES.txt
 portforward.egg-info/dependency_links.txt
 portforward.egg-info/not-zip-safe
 portforward.egg-info/top_level.txt
 tests/conftest.py
+tests/resources.yaml
 tests/test_portforward.py
 venv/lib/python3.10/site-packages/markupsafe/_speedups.c
 venv/lib/python3.10/site-packages/mypyc/lib-rt/bytes_ops.c
 venv/lib/python3.10/site-packages/mypyc/lib-rt/dict_ops.c
 venv/lib/python3.10/site-packages/mypyc/lib-rt/exc_ops.c
 venv/lib/python3.10/site-packages/mypyc/lib-rt/generic_ops.c
 venv/lib/python3.10/site-packages/mypyc/lib-rt/getargs.c
```

### Comparing `portforward-0.4.5/portforward.py` & `portforward-0.5.0/portforward.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Kubernetes Port-Forward Go-Edition For Python
 """
 
-__version__ = "0.4.5"
+__version__ = "0.5.0"
 
 import contextlib
 import os
-import time
 from enum import Enum
 from pathlib import Path
-from typing import Generator, Optional
+from typing import Iterator, Optional
 
 import _portforward
 
 
 class PortforwardError(Exception):
     """Will be raised when something went wrong while the port-forward process."""
 
@@ -22,115 +21,162 @@
     DEBUG = 0
     INFO = 1
     WARN = 2
     ERROR = 3
     OFF = 4
 
 
+class PortForwarder:
+    def __init__(
+        self,
+        namespace: str,
+        pod_or_service: str,
+        from_port: int,
+        to_port: int,
+        config_path: Optional[str] = None,
+        waiting: float = 0.1,
+        log_level: LogLevel = LogLevel.INFO,
+        kube_context: str = "",
+    ) -> None:
+        self.namespace: str = _validate_str("namespace", namespace)
+        self.pod_or_service: str = _validate_str("pod_or_service", pod_or_service)
+        self.from_port: int = _validate_port("from_port", from_port)
+        self.to_port: int = _validate_port("to_port", to_port)
+        self.log_level: LogLevel = _validate_log(log_level)
+        self.waiting: float = waiting
+
+        self.config_path: str = _config_path(config_path)
+        self.kube_context: str = kube_context if kube_context else ""
+
+        _kube_context(kube_context)
+
+        self.actual_pod_name: str = ""
+        self._is_stopped: bool = False
+
+    def forward(self):
+        _portforward.forward(
+            self.namespace,
+            self.pod_or_service,
+            self.from_port,
+            self.to_port,
+            self.config_path,
+            self.log_level.value,
+            self.kube_context,
+        )
+        self._is_stopped = False
+
+    def stop(self):
+        _portforward.stop(self.namespace, self.pod_or_service, self.to_port)
+        self._is_stopped = True
+
+    def is_stopped(self):
+        return self._is_stopped
+
+
 @contextlib.contextmanager
 def forward(
     namespace: str,
     pod_or_service: str,
     from_port: int,
     to_port: int,
     config_path: Optional[str] = None,
     waiting: float = 0.1,
     log_level: LogLevel = LogLevel.INFO,
     kube_context: str = "",
-) -> Generator[None, None, None]:
+) -> Iterator[PortForwarder]:
     """
-    Connects to a **pod or service** and tunnels traffic from a local port to this target.
-    It uses the kubectl kube config from the home dir if no path is provided.
+    Connects to a **pod or service** and tunnels traffic from a local port to
+    this target. It uses the kubectl kube config from the home dir if no path
+    is provided.
 
     The libary will figure out for you if it has to target a pod or service.
 
     It will fall back to in-cluster-config in case no kube config file exists.
 
     Caution: Go and the port-forwarding needs some ms to be ready. ``waiting``
     can be used to wait until the port-forward is ready.
 
     (Best consumed as context manager.)
 
     Example:
         >>> import portforward
         >>> with portforward.forward("test", "web-svc", 9000, 80):
         >>>     # Do work
+        >>>
+        >>> # Or without context manager
+        >>>
+        >>> forwarder = portforward.forward("test", "some-pod", 9000, 80)
+        >>> # Do work
+        >>> forwarder.stop()
 
     :param namespace: Target namespace
     :param pod_or_service: Name of target Pod or service
     :param from_port: Local port
     :param to_port: Port inside the pod
     :param config_path: Path for loading kube config
     :param waiting: Delay in seconds
     :param log_level: Level of logging
     :param kube_context: Target kubernetes context (fallback is current context)
-    :return: None
+    :return: forwarder to manual stop the forwarding
     """
 
-    _validate_str("namespace", namespace)
-    _validate_str("pod_or_service", pod_or_service)
-
-    _validate_port("from_port", from_port)
-    _validate_port("to_port", to_port)
-
-    _validate_log(log_level)
-
-    config_path = _config_path(config_path)
-
-    kube_context = kube_context if kube_context else ""
-    _kube_context(kube_context)
+    forwarder = PortForwarder(
+        namespace,
+        pod_or_service,
+        from_port,
+        to_port,
+        config_path,
+        waiting,
+        log_level,
+        kube_context,
+    )
 
     try:
-        _portforward.forward(
-            namespace,
-            pod_or_service,
-            from_port,
-            to_port,
-            config_path,
-            log_level.value,
-            kube_context,
-        )
+        forwarder.forward()
 
-        # Go and the port-forwarding needs some ms to be ready
-        time.sleep(waiting)
-
-        yield None
+        yield forwarder
 
     except RuntimeError as err:
         # Suppress extension exception
         raise PortforwardError(err) from None
 
     finally:
-        _portforward.stop(namespace, pod_or_service)
+        forwarder.stop()
 
 
 # ===== PRIVATE =====
 
 
-def _validate_str(arg_name, arg):
+def _validate_str(arg_name, arg) -> str:
     if arg is None or not isinstance(arg, str):
         raise ValueError(f"{arg_name}={arg} is not a valid str")
 
     if len(arg) == 0:
         raise ValueError(f"{arg_name} cannot be an empty str")
 
     if "/" in arg:
         raise ValueError(f"{arg_name} contains illegal character '/'")
 
+    return arg
+
 
-def _validate_port(arg_name, arg):
+def _validate_port(arg_name, arg) -> int:
     in_range = arg and 0 < arg < 65536
     if arg is None or not isinstance(arg, int) or not in_range:
         raise ValueError(f"{arg_name}={arg} is not a valid port")
 
+    return arg
+
 
 def _validate_log(log_level):
     if not isinstance(log_level, LogLevel):
         raise ValueError(f"log_level={log_level} is not a valid LogLevel")
 
+    return log_level
+
 
 def _config_path(config_path_arg) -> str:
     if config_path_arg and not isinstance(config_path_arg, str):
         raise ValueError(f"config_path={config_path_arg} is not a valid str")
 
     elif config_path_arg:
         return config_path_arg
```

### Comparing `portforward-0.4.5/setup.py` & `portforward-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     include_package_data=True,
     keywords="portforward",
     name="portforward",
     py_modules=["portforward"],
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/pytogo/portforward",
-    version="0.4.5",
+    version="0.5.0",
     zip_safe=False,
     # Go part
     setup_requires=['setuptools-golang'],
     build_golang={'root': 'github.com/pytogo/portforward'},
     ext_modules=[
         Extension(
             "_portforward", ["main.go"],
```

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/markupsafe/_speedups.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/markupsafe/_speedups.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/bytes_ops.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/bytes_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/dict_ops.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/dict_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/exc_ops.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/exc_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/generic_ops.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/generic_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/getargs.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/getargs.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/getargsfast.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/getargsfast.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/int_ops.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/int_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/list_ops.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/list_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/misc_ops.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/misc_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/str_ops.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/str_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib/python3.10/site-packages/mypyc/lib-rt/tuple_ops.c` & `portforward-0.5.0/venv/lib/python3.10/site-packages/mypyc/lib-rt/tuple_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/markupsafe/_speedups.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/markupsafe/_speedups.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/bytes_ops.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/bytes_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/dict_ops.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/dict_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/exc_ops.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/exc_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/generic_ops.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/generic_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/getargs.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/getargs.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/getargsfast.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/getargsfast.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/int_ops.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/int_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/list_ops.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/list_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/misc_ops.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/misc_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/str_ops.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/str_ops.c`

 * *Files identical despite different names*

### Comparing `portforward-0.4.5/venv/lib64/python3.10/site-packages/mypyc/lib-rt/tuple_ops.c` & `portforward-0.5.0/venv/lib64/python3.10/site-packages/mypyc/lib-rt/tuple_ops.c`

 * *Files identical despite different names*

