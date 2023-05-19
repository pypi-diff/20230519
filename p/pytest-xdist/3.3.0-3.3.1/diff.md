# Comparing `tmp/pytest-xdist-3.3.0.tar.gz` & `tmp/pytest-xdist-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-xdist-3.3.0.tar", last modified: Fri May 12 20:41:30 2023, max compression
+gzip compressed data, was "pytest-xdist-3.3.1.tar", last modified: Fri May 19 10:51:51 2023, max compression
```

## Comparing `pytest-xdist-3.3.0.tar` & `pytest-xdist-3.3.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.270263 pytest-xdist-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    32910 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-12 20:41:30.270263 pytest-xdist-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/changelog/_template.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/crash.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/distribution.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/how-it-works.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/how-to.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/known-limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/remote.rst
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/subprocess.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/boxed.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/example/loadscope/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/example/loadscope/epsilon/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/epsilon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/example/loadscope/test/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/test/test_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/test/test_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/test/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/test/test_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-12 20:41:30.270263 pytest-xdist-3.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.258262 pytest-xdist-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.266263 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.266263 pytest-xdist-3.3.0/src/xdist/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/xdist/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/dsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/looponfail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/newhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.266263 pytest-xdist-3.3.0/src/xdist/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/each.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/loadfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/loadgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/loadscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/worksteal.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/workermanage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.270263 pytest-xdist-3.3.0/testing/
--rw-r--r--   0 runner    (1001) docker     (123)    51523 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/acceptance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_dsession.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_looponfail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_newhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_workermanage.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.226486 pytest-xdist-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    33497 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-19 10:51:51.226486 pytest-xdist-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.218486 pytest-xdist-3.3.1/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/changelog/_template.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.218486 pytest-xdist-3.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/crash.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/distribution.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/how-it-works.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/how-to.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/known-limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/remote.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/docs/subprocess.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.218486 pytest-xdist-3.3.1/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/example/boxed.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.218486 pytest-xdist-3.3.1/example/loadscope/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.222486 pytest-xdist-3.3.1/example/loadscope/epsilon/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/example/loadscope/epsilon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/example/loadscope/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.222486 pytest-xdist-3.3.1/example/loadscope/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/example/loadscope/test/test_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/example/loadscope/test/test_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/example/loadscope/test/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/example/loadscope/test/test_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/example/loadscope/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-19 10:51:51.226486 pytest-xdist-3.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.218486 pytest-xdist-3.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.222486 pytest-xdist-3.3.1/src/pytest_xdist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-19 10:51:51.000000 pytest-xdist-3.3.1/src/pytest_xdist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-19 10:51:51.000000 pytest-xdist-3.3.1/src/pytest_xdist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:51:51.000000 pytest-xdist-3.3.1/src/pytest_xdist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-19 10:51:51.000000 pytest-xdist-3.3.1/src/pytest_xdist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:51:51.000000 pytest-xdist-3.3.1/src/pytest_xdist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 10:51:51.000000 pytest-xdist-3.3.1/src/pytest_xdist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 10:51:51.000000 pytest-xdist-3.3.1/src/pytest_xdist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.222486 pytest-xdist-3.3.1/src/xdist/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-19 10:51:51.000000 pytest-xdist-3.3.1/src/xdist/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19973 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/dsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/looponfail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/newhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.222486 pytest-xdist-3.3.1/src/xdist/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/scheduler/each.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/scheduler/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/scheduler/loadfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/scheduler/loadgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/scheduler/loadscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/scheduler/worksteal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/src/xdist/workermanage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:51:51.226486 pytest-xdist-3.3.1/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)    51523 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/testing/acceptance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/testing/test_dsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/testing/test_looponfail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/testing/test_newhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/testing/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/testing/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/testing/test_workermanage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/testing/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-19 10:51:31.000000 pytest-xdist-3.3.1/tox.ini
```

### Comparing `pytest-xdist-3.3.0/CHANGELOG.rst` & `pytest-xdist-3.3.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+pytest-xdist 3.3.1 (2023-05-19)
+===============================
+
+Bug Fixes
+---------
+
+- `#907 <https://github.com/pytest-dev/pytest-xdist/issues/907>`_: Avoid remote calls during startup as ``execnet`` by default does not ensure remote affinity with the
+  main thread and might accidentally schedule the pytest worker into a non-main thread, which breaks numerous frameworks,
+  for example ``asyncio``, ``anyio``, ``PyQt/PySide``, etc.
+
+  A more safe correction will require thread affinity in ``execnet`` (`pytest-dev/execnet#96 <https://github.com/pytest-dev/execnet/issues/96>`__).
+
+
 pytest-xdist 3.3.0 (2023-05-12)
 ===============================
 
 Features
 --------
 
 - `#555 <https://github.com/pytest-dev/pytest-xdist/issues/555>`_: Improved progress output when collecting nodes to be less verbose.
```

### Comparing `pytest-xdist-3.3.0/LICENSE` & `pytest-xdist-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/PKG-INFO` & `pytest-xdist-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xdist
-Version: 3.3.0
+Version: 3.3.1
 Summary: pytest xdist plugin for distributed testing, most importantly across multiple CPUs
 Home-page: https://github.com/pytest-dev/pytest-xdist
 Author: holger krekel and contributors
 Author-email: pytest-dev@python.org,holger@merlinux.eu
 License: MIT
 Project-URL: Documentation, https://pytest-xdist.readthedocs.io/en/latest
 Project-URL: Changelog, https://pytest-xdist.readthedocs.io/en/latest/changelog.html
```

### Comparing `pytest-xdist-3.3.0/README.rst` & `pytest-xdist-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/RELEASING.rst` & `pytest-xdist-3.3.1/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/changelog/_template.rst` & `pytest-xdist-3.3.1/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/docs/conf.py` & `pytest-xdist-3.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/docs/distribution.rst` & `pytest-xdist-3.3.1/docs/distribution.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/docs/how-it-works.rst` & `pytest-xdist-3.3.1/docs/how-it-works.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/docs/how-to.rst` & `pytest-xdist-3.3.1/docs/how-to.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/docs/index.rst` & `pytest-xdist-3.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/docs/known-limitations.rst` & `pytest-xdist-3.3.1/docs/known-limitations.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/docs/remote.rst` & `pytest-xdist-3.3.1/docs/remote.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/docs/subprocess.rst` & `pytest-xdist-3.3.1/docs/subprocess.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/example/boxed.txt` & `pytest-xdist-3.3.1/example/boxed.txt`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/example/loadscope/test/test_alpha.py` & `pytest-xdist-3.3.1/example/loadscope/test/test_alpha.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/example/loadscope/test/test_beta.py` & `pytest-xdist-3.3.1/example/loadscope/test/test_beta.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/example/loadscope/test/test_delta.py` & `pytest-xdist-3.3.1/example/loadscope/test/test_delta.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/example/loadscope/test/test_gamma.py` & `pytest-xdist-3.3.1/example/loadscope/test/test_gamma.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/pyproject.toml` & `pytest-xdist-3.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/setup.cfg` & `pytest-xdist-3.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/pytest_xdist.egg-info/PKG-INFO` & `pytest-xdist-3.3.1/src/pytest_xdist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xdist
-Version: 3.3.0
+Version: 3.3.1
 Summary: pytest xdist plugin for distributed testing, most importantly across multiple CPUs
 Home-page: https://github.com/pytest-dev/pytest-xdist
 Author: holger krekel and contributors
 Author-email: pytest-dev@python.org,holger@merlinux.eu
 License: MIT
 Project-URL: Documentation, https://pytest-xdist.readthedocs.io/en/latest
 Project-URL: Changelog, https://pytest-xdist.readthedocs.io/en/latest/changelog.html
```

### Comparing `pytest-xdist-3.3.0/src/pytest_xdist.egg-info/SOURCES.txt` & `pytest-xdist-3.3.1/src/pytest_xdist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/_path.py` & `pytest-xdist-3.3.1/src/xdist/_path.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/dsession.py` & `pytest-xdist-3.3.1/src/xdist/dsession.py`

 * *Files 2% similar despite different names*

```diff
@@ -440,34 +440,33 @@
         for spec in specs:
             self.setstatus(spec, WorkerStatus.Created, tests_collected=0, show=False)
         self.setstatus(spec, WorkerStatus.Created, tests_collected=0, show=True)
         self.ensure_show_status()
 
     @pytest.hookimpl
     def pytest_xdist_newgateway(self, gateway) -> None:
-        rinfo = gateway._rinfo()
-        is_local = rinfo.executable == sys.executable
-        if self.config.option.verbose > 0 and not is_local:
-            version = "%s.%s.%s" % rinfo.version_info[:3]
-            self.rewrite(
-                "[%s] %s Python %s cwd: %s"
-                % (gateway.id, rinfo.platform, version, rinfo.cwd),
-                newline=True,
-            )
+        if self.config.option.verbose > 0:
+            rinfo = gateway._rinfo()
+            different_interpreter = rinfo.executable != sys.executable
+            if different_interpreter:
+                version = "%s.%s.%s" % rinfo.version_info[:3]
+                self.rewrite(
+                    f"[{gateway.id}] {rinfo.platform} Python {version} cwd: {rinfo.cwd}",
+                    newline=True,
+                )
         self.setstatus(gateway.spec, WorkerStatus.Initialized, tests_collected=0)
 
     @pytest.hookimpl
     def pytest_testnodeready(self, node) -> None:
-        d = node.workerinfo
-        is_local = d.get("executable") == sys.executable
-        if self.config.option.verbose > 0 and not is_local:
-            infoline = "[{}] Python {}".format(
-                d["id"], d["version"].replace("\n", " -- ")
-            )
-            self.rewrite(infoline, newline=True)
+        if self.config.option.verbose > 0:
+            d = node.workerinfo
+            different_interpreter = d.get("executable") != sys.executable
+            if different_interpreter:
+                version = d["version"].replace("\n", " -- ")
+                self.rewrite(f"[{d['id']}] Python {version}", newline=True)
         self.setstatus(
             node.gateway.spec, WorkerStatus.ReadyForCollection, tests_collected=0
         )
 
     @pytest.hookimpl
     def pytest_testnodedown(self, node, error) -> None:
         if not error:
```

### Comparing `pytest-xdist-3.3.0/src/xdist/looponfail.py` & `pytest-xdist-3.3.1/src/xdist/looponfail.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/newhooks.py` & `pytest-xdist-3.3.1/src/xdist/newhooks.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/plugin.py` & `pytest-xdist-3.3.1/src/xdist/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/remote.py` & `pytest-xdist-3.3.1/src/xdist/remote.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/report.py` & `pytest-xdist-3.3.1/src/xdist/report.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/scheduler/each.py` & `pytest-xdist-3.3.1/src/xdist/scheduler/each.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/scheduler/load.py` & `pytest-xdist-3.3.1/src/xdist/scheduler/load.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/scheduler/loadfile.py` & `pytest-xdist-3.3.1/src/xdist/scheduler/loadfile.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/scheduler/loadgroup.py` & `pytest-xdist-3.3.1/src/xdist/scheduler/loadgroup.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/scheduler/loadscope.py` & `pytest-xdist-3.3.1/src/xdist/scheduler/loadscope.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/scheduler/worksteal.py` & `pytest-xdist-3.3.1/src/xdist/scheduler/worksteal.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/src/xdist/workermanage.py` & `pytest-xdist-3.3.1/src/xdist/workermanage.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/testing/acceptance_test.py` & `pytest-xdist-3.3.1/testing/acceptance_test.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/testing/conftest.py` & `pytest-xdist-3.3.1/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/testing/test_dsession.py` & `pytest-xdist-3.3.1/testing/test_dsession.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/testing/test_looponfail.py` & `pytest-xdist-3.3.1/testing/test_looponfail.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/testing/test_newhooks.py` & `pytest-xdist-3.3.1/testing/test_newhooks.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/testing/test_plugin.py` & `pytest-xdist-3.3.1/testing/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/testing/test_remote.py` & `pytest-xdist-3.3.1/testing/test_remote.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/testing/test_workermanage.py` & `pytest-xdist-3.3.1/testing/test_workermanage.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.3.0/tox.ini` & `pytest-xdist-3.3.1/tox.ini`

 * *Files identical despite different names*

