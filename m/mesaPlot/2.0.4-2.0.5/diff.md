# Comparing `tmp/mesaPlot-2.0.4.tar.gz` & `tmp/mesaPlot-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mesaPlot-2.0.4.tar", last modified: Fri Sep 23 10:42:10 2022, max compression
+gzip compressed data, was "mesaPlot-2.0.5.tar", last modified: Fri May 19 12:28:19 2023, max compression
```

## Comparing `mesaPlot-2.0.4.tar` & `mesaPlot-2.0.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:10.460177 mesaPlot-2.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:10.424177 mesaPlot-2.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/.github/ISSUE_TEMPLATE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:10.428177 mesaPlot-2.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)    15219 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     8873 2022-09-23 10:42:10.460177 mesaPlot-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7987 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:10.428177 mesaPlot-2.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (121)   296403 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/abun_advanced.png
--rw-r--r--   0 runner    (1001) docker     (121)    87039 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/abun_basic.png
--rw-r--r--   0 runner    (1001) docker     (121)    87902 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/abun_bya.png
--rw-r--r--   0 runner    (1001) docker     (121)    53621 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/abun_bypandn.png
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/abundances.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (121)    35113 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/dynamo1.png
--rw-r--r--   0 runner    (1001) docker     (121)    64311 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/dynamo2.png
--rw-r--r--   0 runner    (1001) docker     (121)   112872 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/kip.png
--rw-r--r--   0 runner    (1001) docker     (121)    89490 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/kip_age.png
--rw-r--r--   0 runner    (1001) docker     (121)   104555 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/kip_prof.png
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/plotKip.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/plotTRho.py
--rw-r--r--   0 runner    (1001) docker     (121)   173052 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/examples/trho.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:10.428177 mesaPlot-2.0.4/mesaPlot/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/mesaPlot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26854 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/mesaPlot/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)    29509 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/mesaPlot/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)   174902 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/mesaPlot/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/mesaPlot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:10.432177 mesaPlot-2.0.4/mesaPlot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8873 2022-09-23 10:42:10.000000 mesaPlot-2.0.4/mesaPlot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-09-23 10:42:10.000000 mesaPlot-2.0.4/mesaPlot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 10:42:10.000000 mesaPlot-2.0.4/mesaPlot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-23 10:42:10.000000 mesaPlot-2.0.4/mesaPlot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-23 10:42:10.000000 mesaPlot-2.0.4/mesaPlot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-09-23 10:42:10.460177 mesaPlot-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:10.432177 mesaPlot-2.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:10.460177 mesaPlot-2.0.4/tests/LOGS/
--rw-r--r--   0 runner    (1001) docker     (121)   370405 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/LOGS/history.data
--rw-r--r--   0 runner    (1001) docker     (121)  2168815 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/LOGS/profile1.data
--rw-r--r--   0 runner    (1001) docker     (121) 14154619 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/LOGS/profile17.data
--rw-r--r--   0 runner    (1001) docker     (121)  2161187 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/LOGS/profile2.data
--rw-r--r--   0 runner    (1001) docker     (121)  2165001 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/LOGS/profile3.data
--rw-r--r--   0 runner    (1001) docker     (121)  2153559 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/LOGS/profile4.data
--rw-r--r--   0 runner    (1001) docker     (121)  2145931 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/LOGS/profile5.data
--rw-r--r--   0 runner    (1001) docker     (121)  2145931 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/LOGS/profile6.data
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/LOGS/profiles.index
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/test_mesaplot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 10:42:10.460177 mesaPlot-2.0.4/tests/work/
--rw-r--r--   0 runner    (1001) docker     (121)    38119 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/work/history_columns.list
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/work/inlist
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/work/inlist_pgstar
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/work/inlist_project
--rw-r--r--   0 runner    (1001) docker     (121)    25903 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tests/work/profile_columns.list
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-09-23 10:42:00.000000 mesaPlot-2.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:19.779772 mesaPlot-2.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:19.747771 mesaPlot-2.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/.github/ISSUE_TEMPLATE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:19.747771 mesaPlot-2.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-19 12:28:19.779772 mesaPlot-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:19.747771 mesaPlot-2.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   296403 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/abun_advanced.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87039 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/abun_basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87902 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/abun_bya.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53621 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/abun_bypandn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/abundances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35113 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/dynamo1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64311 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/dynamo2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112872 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/kip.png
+-rw-r--r--   0 runner    (1001) docker     (123)    89490 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/kip_age.png
+-rw-r--r--   0 runner    (1001) docker     (123)   104555 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/kip_prof.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/plotKip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/plotTRho.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173052 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/examples/trho.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:19.751771 mesaPlot-2.0.5/mesaPlot/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/mesaPlot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26854 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/mesaPlot/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29509 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/mesaPlot/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   175091 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/mesaPlot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/mesaPlot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:19.751771 mesaPlot-2.0.5/mesaPlot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-19 12:28:19.000000 mesaPlot-2.0.5/mesaPlot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-19 12:28:19.000000 mesaPlot-2.0.5/mesaPlot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:28:19.000000 mesaPlot-2.0.5/mesaPlot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 12:28:19.000000 mesaPlot-2.0.5/mesaPlot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-19 12:28:19.000000 mesaPlot-2.0.5/mesaPlot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-19 12:28:19.783772 mesaPlot-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:19.751771 mesaPlot-2.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:19.779772 mesaPlot-2.0.5/tests/LOGS/
+-rw-r--r--   0 runner    (1001) docker     (123)   370405 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/LOGS/history.data
+-rw-r--r--   0 runner    (1001) docker     (123)  2168815 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/LOGS/profile1.data
+-rw-r--r--   0 runner    (1001) docker     (123) 14154619 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/LOGS/profile17.data
+-rw-r--r--   0 runner    (1001) docker     (123)  2161187 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/LOGS/profile2.data
+-rw-r--r--   0 runner    (1001) docker     (123)  2165001 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/LOGS/profile3.data
+-rw-r--r--   0 runner    (1001) docker     (123)  2153559 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/LOGS/profile4.data
+-rw-r--r--   0 runner    (1001) docker     (123)  2145931 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/LOGS/profile5.data
+-rw-r--r--   0 runner    (1001) docker     (123)  2145931 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/LOGS/profile6.data
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/LOGS/profiles.index
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/test_mesaplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:19.779772 mesaPlot-2.0.5/tests/work/
+-rw-r--r--   0 runner    (1001) docker     (123)    38119 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/work/history_columns.list
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/work/inlist
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/work/inlist_pgstar
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/work/inlist_project
+-rw-r--r--   0 runner    (1001) docker     (123)    25903 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tests/work/profile_columns.list
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-19 12:28:10.000000 mesaPlot-2.0.5/tox.ini
```

### Comparing `mesaPlot-2.0.4/.github/workflows/publish-to-test-pypi.yml` & `mesaPlot-2.0.5/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/.github/workflows/test.yml` & `mesaPlot-2.0.5/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest]
-        python-version: ['3.6', '3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10','3.11']
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `mesaPlot-2.0.4/.gitignore` & `mesaPlot-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/COPYING.txt` & `mesaPlot-2.0.5/COPYING.txt`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/PKG-INFO` & `mesaPlot-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: mesaPlot
-Version: 2.0.4
+Version: 2.0.5
 Summary: Library for reading and plotting MESA data
 Home-page: https://github.com/rjfarmer/mesaPlot
 Author: Robert Farmer
 Author-email: robert.j.farmer37@gmail.com
 License: GPLv2+
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: COPYING.txt
 
 
 
 [![DOI](https://zenodo.org/badge/30720868.svg)](https://zenodo.org/badge/latestdoi/30720868)
```

### Comparing `mesaPlot-2.0.4/README.md` & `mesaPlot-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/abun_advanced.png` & `mesaPlot-2.0.5/examples/abun_advanced.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/abun_basic.png` & `mesaPlot-2.0.5/examples/abun_basic.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/abun_bya.png` & `mesaPlot-2.0.5/examples/abun_bya.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/abun_bypandn.png` & `mesaPlot-2.0.5/examples/abun_bypandn.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/abundances.py` & `mesaPlot-2.0.5/examples/abundances.py`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/dynamo1.png` & `mesaPlot-2.0.5/examples/dynamo1.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/dynamo2.png` & `mesaPlot-2.0.5/examples/dynamo2.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/kip.png` & `mesaPlot-2.0.5/examples/kip.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/kip_age.png` & `mesaPlot-2.0.5/examples/kip_age.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/kip_prof.png` & `mesaPlot-2.0.5/examples/kip_prof.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/examples/trho.png` & `mesaPlot-2.0.5/examples/trho.png`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/mesaPlot/debug.py` & `mesaPlot-2.0.5/mesaPlot/debug.py`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/mesaPlot/file_reader.py` & `mesaPlot-2.0.5/mesaPlot/file_reader.py`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/mesaPlot/plot.py` & `mesaPlot-2.0.5/mesaPlot/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1695,14 +1695,22 @@
             mpl.rcParams["ytick.minor.size"] = 9  # minor tick size in points
 
             mpl.rcParams["xtick.major.width"] = 0.8  # major tick size in points
             mpl.rcParams["xtick.minor.width"] = 0.6  # minor tick size in points
             mpl.rcParams["ytick.major.width"] = 0.8  # major tick size in points
             mpl.rcParams["ytick.minor.width"] = 0.6  # minor tick size in points
 
+    _core_masses = {
+        "He": {"names": ["he_core_mass"], "color": "clr_Teal"},
+        "C": {"names": ["c_core_mass", "co_core_mass"], "color": "clr_LightOliveGreen"},
+        "O": {"names": ["o_core_mass", "one_core_mass"], "color": "clr_SeaGreen"},
+        "Si": {"names": ["si_core_mass"], "color": "clr_Lilac"},
+        "Fe": {"names": ["fe_core_mass"], "color": "clr_Crimson"},
+    }
+
     def set_solar(self, solar="ag89"):
         if str(solar) == "ag89":
             self.sol_comp = self._sol_comp_ag89
         else:
             raise ValueError("Must pass ag89")
 
         self.solar_is_set = True
@@ -2439,105 +2447,86 @@
                     path_effects.Normal(),
                 ]
             )
 
         ax.set_xlim(xlim)
         ax.set_ylim(ylim)
 
-    def _plotCoreLoc(
-        self, prof, ax, xaxis, x, ymin, ymax, linecol="k", coreMasses=None
-    ):
-        if coreMasses is None:
-            coreMasses = [
-                "he_core_mass",
-                "c_core_mass",
-                "o_core_mass",
-                "si_core_mass",
-                "fe_core_mass",
-            ]
+    def _plotCoreLoc(self, prof, ax, xaxis, x, ymin, ymax, linecol="k"):
 
-        for cm in coreMasses:
+        for name, value in self._core_masses.items():
+            cn = None
             # Find cell where we have core mass and use that to index the actual x axis
+            for n in value.names:
+                if n in prof.head.dtype.names:
+                    cm = n
+
             pos = bisect.bisect_right(prof.data["mass"][::-1], prof.head[cm])
             if pos < np.size(prof.data[xaxis]) and pos > 0 and prof.head[cm] > 0.0:
                 pos = np.size(prof.data["mass"]) - pos
                 ax.plot(
                     [prof.data[xaxis][pos], prof.data[xaxis][pos]],
                     [ymin, ymax],
                     "--",
                     color=linecol,
                 )
                 xp1 = prof.data[xaxis][pos]
                 yp1 = 0.95 * (ymax - ymin) + ymin
                 ax.annotate(
-                    cm.split("_")[0],
+                    name,
                     xy=(xp1, yp1),
                     xytext=(xp1, yp1),
                     color=linecol,
                     fontsize=mpl.rcParams["font.size"] - 12,
                 )
 
     def _showMassLoc(self, m, fig, ax, x, modInd):
-        coreMasses = [
-            "he_core_mass",
-            "c_core_mass",
-            "o_core_mass",
-            "si_core_mass",
-            "fe_core_mass",
-        ]
-        labels = ["He", "C", "O", "Si", "Fe"]
-        col = [
-            "clr_Teal",
-            "clr_LightOliveGreen",
-            "clr_SeaGreen",
-            "clr_Lilac",
-            "clr_Crimson",
-        ]
 
-        for i, j in zip(coreMasses, col):
-            y = m.hist.data[i][modInd]
+        l = []
+        c = []
+        for name, val in self._core_masses.items():
+            y = None
+            for n in val["names"]:
+                if n in m.hist.data.dtype.names:
+                    y = m.hist.data[n][modInd]
+            if y is None:
+                continue
+
             if np.any(y):
-                ax.plot(x, y, color=self.colors[j], linewidth=5)
+                ax.plot(x, y, color=self.colors[val["color"]], linewidth=5)
+                l.append(name)
+                c.append(self.colors[val["color"]])
 
         self._addExtraLabelsToAxis(
             fig,
-            labels,
-            [self.colors[i] for i in col],
+            l,
+            c,
             num_left=0,
-            num_right=len(labels),
+            num_right=len(l),
             right_pad=50,
         )
 
     def _showMassLocHist(self, m, fig, ax, x, y, modInd):
-        coreMasses = [
-            "he_core_mass",
-            "c_core_mass",
-            "o_core_mass",
-            "si_core_mass",
-            "fe_core_mass",
-        ]
-        labels = ["He", "C", "O", "Si", "Fe"]
-        col = [
-            "clr_Teal",
-            "clr_LightOliveGreen",
-            "clr_SeaGreen",
-            "clr_Lilac",
-            "clr_Crimson",
-        ]
-
         out = []
         outc = []
-        for i, j, l in zip(coreMasses, col, labels):
-            ind = m.hist.data[i][modInd] > 0.0
+
+        for name, val in self._core_masses.items():
+            ind = None
+            for n in val["names"]:
+                if n in m.hist.data:
+                    ind = m.hist.data[n][modInd] > 0.0
+            if ind is None:
+                continue
+
             if np.count_nonzero(ind):
                 ax.plot(
                     [x[ind][0], x[ind][0]],
                     ax.get_ylim(),
                     "--",
-                    color=self.colors[j],
+                    color=self.colors[val["color"]],
                     linewidth=2,
                 )
                 out.append(x[ind][0])
                 outc.append(l)
 
         ax2 = ax.twiny()
         ax2.plot(ax.get_xlim(), ax.get_ylim())
@@ -5921,15 +5910,15 @@
 
         return age
 
     def _getSafeCenter(self, m, radius):
         center = None
         if radius:
             if "r_center" in m.hist:
-                if np.any(m.hist.data["r_center"] > m.hist.star_radius):
+                if np.any(m.hist.data["r_center"] > 10**m.hist.log_R):
                     # r_center in cm
                     center = m.hist.data["r_center"] / self.rsun
                 else:
                     # Solar units
                     center = m.hist.data["r_center"]
         else:
             if "m_center" in m.hist:
@@ -5991,15 +5980,21 @@
 
         return modInd
 
     def _rebinKipDataX(self, data, x, lin_x, nan=False, nan_value=1):
         sorter = np.argsort(x)
         ind = np.searchsorted(x, lin_x, sorter=sorter, side="left")
 
-        data = data[sorter[ind], :]
+        s_ind = sorter[ind]
+
+        # When flipping the ages we may end up with points at the edge
+        # so just make sure we dont go out of bound (searcgsoretd returns N if no suitable match found)
+        s_ind[s_ind == len(data)] = len(data) - 1
+
+        data = data[s_ind, :]
         if nan:
             data[data < nan_value] = np.nan
         data = np.array(data)
         return data
 
     def _rebinKipDataXY(self, data_z, data_x, data_y, num_x_zones, num_y_zones):
         ymin = np.nanmin([np.nanmin(y) for y in data_y])
```

### Comparing `mesaPlot-2.0.4/mesaPlot.egg-info/PKG-INFO` & `mesaPlot-2.0.5/mesaPlot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: mesaPlot
-Version: 2.0.4
+Version: 2.0.5
 Summary: Library for reading and plotting MESA data
 Home-page: https://github.com/rjfarmer/mesaPlot
 Author: Robert Farmer
 Author-email: robert.j.farmer37@gmail.com
 License: GPLv2+
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: COPYING.txt
 
 
 
 [![DOI](https://zenodo.org/badge/30720868.svg)](https://zenodo.org/badge/latestdoi/30720868)
```

### Comparing `mesaPlot-2.0.4/mesaPlot.egg-info/SOURCES.txt` & `mesaPlot-2.0.5/mesaPlot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/setup.cfg` & `mesaPlot-2.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 author_email = robert.j.farmer37@gmail.com
 license = GPLv2+
 platforms = unix, linux, osx, cygwin, win32
 url = https://github.com/rjfarmer/mesaPlot
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Astronomy
 	Intended Audience :: Science/Research
 
 [options]
-python_requires = >=3.6
+python_requires = >=3.7
 packages = find:
 install_requires = 
 	numpy
 	matplotlib
 	scipy
 	pandas
 	pytest
```

### Comparing `mesaPlot-2.0.4/setup.py` & `mesaPlot-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/LOGS/history.data` & `mesaPlot-2.0.5/tests/LOGS/history.data`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/LOGS/profile1.data` & `mesaPlot-2.0.5/tests/LOGS/profile1.data`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/LOGS/profile17.data` & `mesaPlot-2.0.5/tests/LOGS/profile17.data`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/LOGS/profile2.data` & `mesaPlot-2.0.5/tests/LOGS/profile2.data`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/LOGS/profile3.data` & `mesaPlot-2.0.5/tests/LOGS/profile3.data`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/LOGS/profile4.data` & `mesaPlot-2.0.5/tests/LOGS/profile4.data`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/LOGS/profile5.data` & `mesaPlot-2.0.5/tests/LOGS/profile5.data`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/LOGS/profile6.data` & `mesaPlot-2.0.5/tests/LOGS/profile6.data`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/test_mesaplot.py` & `mesaPlot-2.0.5/tests/test_mesaplot.py`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/work/history_columns.list` & `mesaPlot-2.0.5/tests/work/history_columns.list`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/work/inlist` & `mesaPlot-2.0.5/tests/work/inlist`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/work/inlist_pgstar` & `mesaPlot-2.0.5/tests/work/inlist_pgstar`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/work/inlist_project` & `mesaPlot-2.0.5/tests/work/inlist_project`

 * *Files identical despite different names*

### Comparing `mesaPlot-2.0.4/tests/work/profile_columns.list` & `mesaPlot-2.0.5/tests/work/profile_columns.list`

 * *Files identical despite different names*

