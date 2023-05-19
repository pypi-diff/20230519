# Comparing `tmp/ingit-0.4.8.tar.gz` & `tmp/ingit-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ingit-0.4.8.tar", last modified: Sat Aug 24 08:16:38 2019, max compression
+gzip compressed data, was "ingit-0.4.9.tar", last modified: Mon Aug 15 16:25:18 2022, max compression
```

## Comparing `ingit-0.4.8.tar` & `ingit-0.4.9.tar`

### file list

```diff
@@ -1,45 +1,59 @@
-drwxr-xr-x   0 mateusz   (1000) mateusz   (1000)        0 2019-08-24 08:16:38.000000 ingit-0.4.8/
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    35147 2019-07-18 03:55:38.000000 ingit-0.4.8/LICENSE
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)      107 2019-08-12 04:49:58.000000 ingit-0.4.8/MANIFEST.in
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)      687 2019-07-18 03:55:38.000000 ingit-0.4.8/NOTICE
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    18479 2019-08-24 08:16:38.000000 ingit-0.4.8/PKG-INFO
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    13207 2019-08-24 08:14:15.000000 ingit-0.4.8/README.rst
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)       41 2019-08-12 04:49:58.000000 ingit-0.4.8/ci_requirements.txt
-drwxr-xr-x   0 mateusz   (1000) mateusz   (1000)        0 2019-08-24 08:16:38.000000 ingit-0.4.8/ingit/
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)      100 2019-08-12 05:45:54.000000 ingit-0.4.8/ingit/__init__.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)      133 2019-08-12 06:37:57.000000 ingit-0.4.8/ingit/__main__.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)      114 2019-07-18 03:55:38.000000 ingit-0.4.8/ingit/_version.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     4446 2019-07-18 03:55:38.000000 ingit-0.4.8/ingit/action_progress.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1848 2019-07-18 03:55:38.000000 ingit-0.4.8/ingit/fetch_flags.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     3533 2019-08-12 04:49:58.000000 ingit-0.4.8/ingit/json_config.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    13233 2019-08-24 08:14:15.000000 ingit-0.4.8/ingit/main.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    22121 2019-07-18 03:55:38.000000 ingit-0.4.8/ingit/project.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1289 2019-07-18 03:55:38.000000 ingit-0.4.8/ingit/push_flags.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)        0 2019-08-12 04:49:58.000000 ingit-0.4.8/ingit/py.typed
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     3195 2019-07-18 03:55:38.000000 ingit-0.4.8/ingit/repo_data.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    13233 2019-08-24 08:14:15.000000 ingit-0.4.8/ingit/runtime.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     3395 2019-07-18 03:55:38.000000 ingit-0.4.8/ingit/runtime_interface.py
-drwxr-xr-x   0 mateusz   (1000) mateusz   (1000)        0 2019-08-24 08:16:38.000000 ingit-0.4.8/ingit.egg-info/
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    18479 2019-08-24 08:16:38.000000 ingit-0.4.8/ingit.egg-info/PKG-INFO
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)      846 2019-08-24 08:16:38.000000 ingit-0.4.8/ingit.egg-info/SOURCES.txt
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)        1 2019-08-24 08:16:38.000000 ingit-0.4.8/ingit.egg-info/dependency_links.txt
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)       47 2019-08-24 08:16:38.000000 ingit-0.4.8/ingit.egg-info/entry_points.txt
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)       62 2019-08-24 08:16:38.000000 ingit-0.4.8/ingit.egg-info/requires.txt
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)        6 2019-08-24 08:16:38.000000 ingit-0.4.8/ingit.egg-info/top_level.txt
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)       64 2019-08-12 05:46:55.000000 ingit-0.4.8/requirements.txt
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)       38 2019-08-24 08:16:38.000000 ingit-0.4.8/setup.cfg
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1445 2019-08-12 04:49:58.000000 ingit-0.4.8/setup.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    12516 2019-08-12 04:49:58.000000 ingit-0.4.8/setup_boilerplate.py
-drwxr-xr-x   0 mateusz   (1000) mateusz   (1000)        0 2019-08-24 08:16:38.000000 ingit-0.4.8/test/
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     6656 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_action_progress.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     8321 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_git_commands.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     5738 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_ingit_commands.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2794 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_json_config.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1699 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_main.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     9064 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_project.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1543 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_repo_data.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     4103 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_runtime.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1252 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_runtime_interface.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)    14058 2019-08-12 04:49:58.000000 ingit-0.4.8/test/test_setup.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     3667 2019-07-18 03:55:38.000000 ingit-0.4.8/test/test_with_git_repo.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)       73 2019-07-18 03:55:38.000000 ingit-0.4.8/test_requirements.txt
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-15 16:25:18.042340 ingit-0.4.9/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    35147 2020-05-27 06:45:47.000000 ingit-0.4.9/LICENSE
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      210 2022-01-02 13:12:59.000000 ingit-0.4.9/MANIFEST.in
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      687 2022-08-15 16:22:27.000000 ingit-0.4.9/NOTICE
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    14911 2022-08-15 16:25:18.042340 ingit-0.4.9/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    13437 2022-08-15 16:22:27.000000 ingit-0.4.9/README.rst
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-15 16:25:18.039340 ingit-0.4.9/ingit/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       86 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      185 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/__main__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      218 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/_logging.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      112 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/_version.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4395 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/action_progress.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3483 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/cli_boilerplate.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1039 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/config_boilerplate.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1828 2022-01-03 10:39:01.000000 ingit-0.4.9/ingit/fetch_flags.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3137 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/json_config.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     8371 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/logging_boilerplate.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    13375 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/main.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    22526 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/project.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1280 2020-05-27 06:45:47.000000 ingit-0.4.9/ingit/push_flags.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2020-05-27 06:45:47.000000 ingit-0.4.9/ingit/py.typed
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4071 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/repo_data.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    12963 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/runtime.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3552 2022-08-15 16:22:27.000000 ingit-0.4.9/ingit/runtime_interface.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-15 16:25:18.042340 ingit-0.4.9/ingit.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    14911 2022-08-15 16:25:17.000000 ingit-0.4.9/ingit.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1560 2022-08-15 16:25:17.000000 ingit-0.4.9/ingit.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2022-08-15 16:25:17.000000 ingit-0.4.9/ingit.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       46 2022-08-15 16:25:17.000000 ingit-0.4.9/ingit.egg-info/entry_points.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       96 2022-08-15 16:25:17.000000 ingit-0.4.9/ingit.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        6 2022-08-15 16:25:17.000000 ingit-0.4.9/ingit.egg-info/top_level.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      753 2022-08-15 16:22:27.000000 ingit-0.4.9/pyproject.toml
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      108 2022-08-15 16:22:51.000000 ingit-0.4.9/requirements.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       99 2022-08-15 16:22:27.000000 ingit-0.4.9/requirements_test.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       96 2022-08-15 16:25:18.042340 ingit-0.4.9/setup.cfg
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1429 2022-08-15 16:22:27.000000 ingit-0.4.9/setup.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    15385 2022-08-15 16:22:27.000000 ingit-0.4.9/setup_boilerplate.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-15 16:25:18.040341 ingit-0.4.9/test/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      332 2022-08-15 16:22:27.000000 ingit-0.4.9/test/__init__.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-15 16:25:18.035340 ingit-0.4.9/test/examples/
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-15 16:25:18.040341 ingit-0.4.9/test/examples/repos_config/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      651 2022-01-02 13:12:59.000000 ingit-0.4.9/test/examples/repos_config/example_initial.json
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      616 2020-05-27 06:45:47.000000 ingit-0.4.9/test/examples/repos_config/example_paths.json
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-15 16:25:18.041340 ingit-0.4.9/test/examples/runtime_config/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      160 2020-05-27 06:45:47.000000 ingit-0.4.9/test/examples/runtime_config/example_bad.json
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      180 2020-05-27 06:45:47.000000 ingit-0.4.9/test/examples/runtime_config/example_initial.json
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      186 2020-05-27 06:45:47.000000 ingit-0.4.9/test/examples/runtime_config/example_names.json
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     6666 2020-05-27 06:45:47.000000 ingit-0.4.9/test/test_action_progress.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     7997 2022-08-15 16:22:27.000000 ingit-0.4.9/test/test_git_commands.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     5470 2022-01-02 13:12:59.000000 ingit-0.4.9/test/test_ingit_commands.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2794 2020-05-27 06:45:47.000000 ingit-0.4.9/test/test_json_config.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4331 2022-08-15 16:22:27.000000 ingit-0.4.9/test/test_logging.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1717 2022-08-15 16:22:27.000000 ingit-0.4.9/test/test_main.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     9096 2020-05-27 06:45:47.000000 ingit-0.4.9/test/test_project.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1543 2020-05-27 06:45:47.000000 ingit-0.4.9/test/test_repo_data.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4087 2020-05-27 06:45:47.000000 ingit-0.4.9/test/test_runtime.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1252 2020-05-27 06:45:47.000000 ingit-0.4.9/test/test_runtime_interface.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)    14195 2022-08-15 16:22:27.000000 ingit-0.4.9/test/test_setup.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3690 2022-08-15 16:22:27.000000 ingit-0.4.9/test/test_with_git_repo.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ingit-0.4.8/LICENSE` & `ingit-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ingit-0.4.8/NOTICE` & `ingit-0.4.9/NOTICE`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ingit
-Copyright (C) 2015-2018  Mateusz Bysiek  https://mbdevpl.github.io/
+Copyright (c) 2015-2022  Mateusz Bysiek  https://mbdevpl.github.io/
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `ingit-0.4.8/README.rst` & `ingit-0.4.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: ingit
+Version: 0.4.9
+Summary: git repository collection management tool
+Home-page: https://github.com/mbdevpl/ingit
+Download-URL: 
+Author: Mateusz Bysiek
+Author-email: mateusz.bysiek@gmail.com
+Maintainer: Mateusz Bysiek
+Maintainer-email: mateusz.bysiek@gmail.com
+License: GNU General Public License v3 or later (GPLv3+)
+Keywords: tools,vcs,repository management,git,submodules
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Version Control
+Classifier: Topic :: System :: Archiving :: Backup
+Classifier: Topic :: System :: Archiving :: Mirroring
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE
+License-File: NOTICE
+
 .. role:: bash(code)
     :language: bash
 
 .. role:: json(code)
     :language: json
 
 .. role:: python(code)
@@ -14,21 +49,17 @@
 
 Tool for managing a large collection of repositories in git.
 
 .. image:: https://img.shields.io/pypi/v/ingit.svg
     :target: https://pypi.org/project/ingit
     :alt: package version from PyPI
 
-.. image:: https://travis-ci.org/mbdevpl/ingit.svg?branch=master
-    :target: https://travis-ci.org/mbdevpl/ingit
-    :alt: build status from Travis CI
-
-.. image:: https://ci.appveyor.com/api/projects/status/github/mbdevpl/ingit?branch=master&svg=true
-    :target: https://ci.appveyor.com/project/mbdevpl/ingit
-    :alt: build status from AppVeyor
+.. image:: https://github.com/mbdevpl/ingit/actions/workflows/python.yml/badge.svg?branch=main
+    :target: https://github.com/mbdevpl/ingit/actions
+    :alt: build status from GitHub
 
 .. image:: https://codecov.io/gh/mbdevpl/ingit/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/mbdevpl/ingit
     :alt: test coverage from Codecov
 
 .. image:: https://img.shields.io/github/license/mbdevpl/ingit.svg
     :target: https://github.com/mbdevpl/ingit/blob/master/NOTICE
@@ -137,40 +168,40 @@
 
 .. code:: python
 
     lambda name, tags, path, remotes: (predicate)
 
 The actual implementation is here: `<ingit/main.py#L232>`_
 
-Therefore, executing ``ingit --predicate "'mytag' in tags" fetch`` results
+Therefore, executing ``ingit --predicate "'python' in tags" fetch`` results
 in the following predicate being applied:
 
 .. code:: python
 
-    lambda name, tags, path, remotes: ('mytag' in tags)
+    lambda name, tags, path, remotes: ('python' in tags)
 
-And thus only repositories that have ``'mytag'`` in their tags are fetched.
+And thus only repositories that have ``'python'`` in their tags are fetched.
 
 
 Configuration
 -------------
 
 Ingit works based on configuration in 2 JSON files:
 
 *   runtime configuration
-*   repositories configuraion
+*   repositories configuration
 
-If either of the files doesn't exist, detaults will be generated.
+If either of the files doesn't exist, defaults will be generated.
 
-The default paths to the files can be overriden via ``--config`` and ``--repos``
+The default paths to the files can be overridden via ``--config`` and ``--repos``
 command-line options.
 
 
-Runtime configuraion
-~~~~~~~~~~~~~~~~~~~~
+Runtime configuration
+~~~~~~~~~~~~~~~~~~~~~
 
 Most importantly, stores repositories root directory -- it's a directory which ingit assumes
 to contain git-versioned projects.
 
 Example:
 
 .. code:: json
@@ -188,16 +219,16 @@
           "names": ["server", "server.domain.com"],
           "repos_path": "$HOME/Projects"
         }
       ]
     }
 
 
-Repositories configuraion
-~~~~~~~~~~~~~~~~~~~~~~~~~
+Repositories configuration
+~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 It's a file that lists all registered projects and keeps their metadata.
 
 It is automatically updated when ``ingit register`` is used.
 
 Example:
 
@@ -241,51 +272,47 @@
 
     {
       "name": "name of the project",
       "path": "path doesn't have to be specified, by default it will be 'repos_path/name'",
       "paths": {
         "machine name 1": "path used only on machine 1",
         "machine name 2": "path used only on machine 2",
-        "": "if no machine name is given, the path is used in all other cases",
-        ...
-      }
+        "": "if no machine name is given, the path is used in all other cases"
+      },
       "remotes": {
         "remote name 1": "url 1",
-        "remote name 2": "url 2",
-        ...
+        "remote name 2": "url 2"
       },
       "tags": [
         "tags are completely optional",
         "but repositories are much easier to manage if they are consistently tagged"
       ]
     }
 
 
-The ``repos_path`` mentioned above is taken from the runtime configuation of ingit.
+The ``repos_path`` mentioned above is taken from the runtime configuration of ingit.
 
 At most one of ``path`` or ``paths`` is allowed for each repo.
 
 The two path specifications below are equivalent:
 
 .. code:: json
 
     {
-      ...
-      "path": "some path",
-      ...
+      "name": "name of the project",
+      "path": "some path"
     }
 
 .. code:: json
 
     {
-      ...
+      "name": "name of the project",
       "paths": {
         "": "some path"
-      },
-      ...
+      }
     }
 
 
 
 Command details
 ===============
 
@@ -293,69 +320,76 @@
 
 
 ``ingit summary``
 -----------------
 
 Show summary of registered repositories and status of configured repository root.
 
-First of all, print a list of registered repositories. By default, all registered repositories
-are listed, but, as in case of most commands, the results can be filtered via a predicate or regex.
+First of all, print a list of registered repositories. By default, all
+registered repositories are listed, but, as in case of most commands, the
+results can be filtered via a predicate or regex.
 
-Independently, print a list of all unregistered repositories and all not versioned paths present
-in the configured repositories root.
+Independently, print a list of all unregistered repositories and all not
+versioned paths present in the configured repositories root.
 
 
 ``ingit register``
 ------------------
 
 Start tracking a repository in ingit.
 
 .. code:: bash
 
-    ingit register [--tags TAG ...] [PATH]
+    ingit register [PATH] [--tags TAG ...]
 
 The initial configuration is set according to basic repository information:
-its root directory name becomes "name" and its currently configured remotes become
-"remotes". You can edit the configuration manually afterwards.
+its root directory name becomes "name" and its currently configured remotes
+become "remotes". You can edit the configuration manually afterwards.
 
 The final "path" to the repository stored in the configuration depends on the
-``repos_path`` in runtime configuation. The configured "path" will be:
+``repos_path`` in runtime configuration. The configured "path" will be:
 
-*   resolved absolute path if there is no ``repos_path`` configured or repository path
-    is outside of the ``repos_path``;
-*   resolved relative path to the ``repos_path``, if the repository path is within it;
+*   resolved absolute path if there is no ``repos_path`` configured or
+    repository path is outside of the ``repos_path``;
+*   resolved relative path to the ``repos_path``, if the repository path is
+    within it;
 *   nothing (i.e. not stored) if the if the repository is stored directly in
     ``repos_path`` (i.e. there are no intermediate directories).
 
 Behaviour of storing relative/no paths in some cases is implemented to make
-configuration file much less verbose in typical usage scenarios. To prevent this
-behaviour, and force all repository paths to be absolute, simply set the ``repos_path``
-in your runtime configuraion to JSON ``null``.
+configuration file much less verbose in typical usage scenarios. To prevent
+this behaviour, and force all repository paths to be absolute, simply set the
+``repos_path`` in your runtime configuration to JSON ``null``.
 
 Use ``PATH`` to provide the path to root directory of repository.
 If not provided, current working directory is used.
 
-Use ``--tags`` to provide tags for this repository, they will be added to the initial configuration.
-Tags have no other effect than making repository filtering easier.
+Use ``--tags`` to provide tags for this repository, they will be added to the
+initial configuration. Tags have no other effect than making repository
+filtering easier.
 
 
 ``ingit foreach``
 ------------------
 
-TODO.
+The given command is executed in a shell in working directory of each
+project.
+
+Use ``--timeout`` to set timeout of the command (in seconds).
 
 
 ``ingit clone``
 ---------------
 
-Execute ``git clone <remote-url> --recursive --orign <remote-name> <path>``,
-where values of ``<path>`` and ``<remote-...>`` are taken from default remote configuration
-of the repository.
+Execute ``git clone <remote-url> --recursive --origin <remote-name> <path>``,
+where values of ``<path>`` and ``<remote-...>`` are taken from default remote
+configuration of the repository.
 
-After cloning, add all remaining configured remotes to the repository and fetch them.
+After cloning, add all remaining configured remotes to the repository and
+fetch them.
 
 For example, if repository configuration is as follows:
 
 .. code:: json
 
   {
     "name": "Spack",
@@ -364,77 +398,85 @@
       "source": "https://github.com/spack/spack.git",
       "github": "git@github.com:mbdevpl/spack.git"
     },
     "tags": []
   }
 
 The clone command will be:
-``git clone https://github.com/spack/spack.git --recursive --orign source ~/Software/Spack``
+``git clone https://github.com/spack/spack.git --recursive --origin source ~/Software/Spack``
 because ``source`` is the first configured remote.
 The subsequent commands will be ``git remote add github git@github.com:mbdevpl/spack.git``
 and ``git fetch github``.
 
 
 ``ingit init``
 --------------
 
-Execute ``git init`` followed by ``git remote add`` for each configured remote.
+Execute ``git init`` followed by ``git remote add`` for each configured
+remote.
 
 
 ``ingit fetch``
 ---------------
 
-Execute ``git fetch <remote-name>``, where the remote name is the remote of the current
-tracking branch, or all remotes of the repository if there's no tracking branch,
-or repository is in detached head state.
+Execute ``git fetch <remote-name>``, where the remote name is the remote of
+the current tracking branch, or all remotes of the repository if there's no
+tracking branch, or repository is in detached head state.
 
 Use ``--all`` to fetch all remotes in all cases.
 
 
 ``ingit checkout``
 ------------------
 
-Interactively select revision to checkout from list of local branches,
-remote non-tracking branches and local tags.
+Interactively select revision to checkout from list of local branches, remote
+non-tracking branches and local tags.
 
-The list of branches to select from is composed by combinig:
+The list of branches to select from is composed by combining:
 
-- local branches
-- non-tracking branches on all remotes
-- local tags
+*   local branches
+*   non-tracking branches on all remotes
+*   local tags
 
-Checking out a remote branch will create a local branch with the same unless it already exists.
-If it already exists, repository will end up in detached head state.
+Checking out a remote branch will create a local branch with the same unless
+it already exists. If it already exists, repository will end up in detached
+head state.
 
-Also, checking out any tag will put repository in detached head state.
+Also, checking out any tag will put repository in a detached head state.
 
 
 ``ingit merge``
 ---------------
 
-Not yet implemented!
+**Not yet implemented!** The following functionality is intended.
 
-Interactively merge all branches to their tracking branches.
-For each ``<branch>``-``<tracking-branch>`` pair,
-execute ``git checkout <branch>`` and then if the merge can be fast-forward,
-automatically execute ``git merge <tracking-branch> --ff-only``.
-If not, then show more information about the situation of the repository, and propose:
+Interactively merge all branches to their tracking branches. For each not
+merged ``<branch>``-``<tracking-branch>`` pair, execute
+``git checkout <branch>`` and then if the merge is fast-forward,
+automatically execute ``git merge <tracking-branch> --ff-only``. If not, then
+show more information about the situation of the repository, and propose:
 
 *   ``git merge --log <tracking-branch>``,
 *   ``git rebase -i <tracking-branch>`` and
 *   ``git reset --hard <tracking-branch>``.
 
-If repository is dirty when this command is executed, the command will do nothing.
-After work is done, return to the originally checked-out branch.
+If repository is dirty when this command is executed, do nothing. After work
+is done, return to the originally checked-out branch.
 
 
 ``ingit push``
 --------------
 
-Execute ``git push <remote-name> <branch>:<tracking-branch-name>`` for the active branch.
+Execute ``git push <remote-name> <branch>:<tracking-branch-name>`` for the
+active branch.
+
+The above functionality works, but the following functionality is **not yet implemented**.
+
+Use ``--all`` to execute the push for every branch that has a remote tracking
+branch.
 
 
 ``ingit gc``
 ------------
 
 Execute ``git gc --aggressive --prune``.
 
@@ -442,27 +484,30 @@
 ``ingit status``
 ----------------
 
 Perform git status, as well as other diagnostic git commands.
 
 Execute:
 
-*   ``git status --short --branch`` to inform about any uncommited changes,
-*   ``git log tracking_branch..branch`` to inform about commits that are not yet pushed to the remote,
-*   ``git log branch..tracking_branch`` to inform about commits that are not yet merged from the remote.
+*   ``git status --short --branch`` to inform about any uncommitted changes,
+*   ``git log tracking_branch..branch`` to inform about commits that are not
+    yet pushed to the remote,
+*   ``git log branch..tracking_branch`` to inform about commits that are not
+    yet merged from the remote.
 
-Additionally, compare registered remotes with actual remotes to make sure that ingit
-configuration is in sync with the repository metadata.
+Additionally, compare registered remotes with actual remotes to make sure
+that ingit configuration is in sync with the repository metadata.
 
-Use ``--ignored`` to include ignored files in the status report, just as with ``git status``.
+Use ``--ignored`` to include ignored files in the status report, just as with
+``git status``.
 
 
 Requirements
 ============
 
-Python version 3.5 or later.
+Python version 3.8 or later.
 
-Python libraries as specified in `<requirements.txt>`_.
+Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/ingit/blob/v0.4.9/requirements.txt>`_.
 
 Building and running tests additionally requires packages listed in `<test_requirements.txt>`_.
 
-Tested on Linux, OS X and Windows.
+Tested on Linux, macOS and Windows.
```

### Comparing `ingit-0.4.8/ingit/action_progress.py` & `ingit-0.4.9/ingit/action_progress.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import shutil
 import sys
 import typing as t
 
 import git
 import git.remote
+from git.util import RemoteProgress
 
 # list used by __create_operation_strings()
 _KNOWN_OPERATIONS_STRINGS = {
     git.remote.RemoteProgress.BEGIN: 'begun',  # 1
     git.remote.RemoteProgress.END: 'ended',  # 2
     git.remote.RemoteProgress.COUNTING: 'counting objects',  # 4
     git.remote.RemoteProgress.COMPRESSING: 'compressing',  # 8
@@ -34,34 +35,33 @@
 
 def _create_operation_strings(op_code: int):
     """Create operation strings."""
     operation_strings = []
     for key, value in _KNOWN_OPERATIONS_STRINGS.items():
         if op_code & key:
             operation_strings.append(value)
-    unknown_operations = op_code & ~(_KNOWN_OPERATIONS)
+    unknown_operations = op_code & ~_KNOWN_OPERATIONS
     if unknown_operations:
         operation_strings.append(
-            'unknown operation code(s): {0} ({0:032b})'.format(unknown_operations))
+            f'unknown operation code(s): {unknown_operations} ({unknown_operations:032b})')
     return operation_strings
 
 
 class ActionProgress(git.remote.RemoteProgress):
-
     """Emulate usual git progress reports in the console when working with GitPython."""
 
     def __init__(self, inline: bool = True, f_d=None):
         """When no redirected_output_fd is given, use stdout."""
         assert isinstance(inline, bool)
 
         super().__init__()
         self.printed_lines = False
         self.line_len = 0  # type: int
         try:
-            term_size = shutil.get_terminal_size()  # type: t.Tuple[int, int]
+            term_size = shutil.get_terminal_size()
             _LOG.log(logging.WARNING if term_size.columns < 16 else logging.NOTSET,
                      'detected terminal width is %i', term_size.columns)
             self.line_width = term_size.columns if term_size.columns else 100
         except ValueError:
             self.line_width = 100
         assert self.line_width > 0
 
@@ -74,45 +74,45 @@
         else:
             self._print_with_nl(text)
 
     def _print_with_nl(self, text: str):
         print(text, file=self.f_d)
 
     def update(self, op_code: int, cur_count: t.Any, max_count: t.Any = None, message: str = ''):
-        """Override git.remote.RemoteProgress.update()."""
+        """Override git.remote.RemoteProgress.update."""
         operation_strings = _create_operation_strings(op_code)
-        description = '{}: '.format(' '.join(operation_strings)) if operation_strings else ''
+        description = f'{" ".join(operation_strings)}: ' if operation_strings else ''
         progress = ''
         if cur_count:
             progress += str(int(cur_count))
         if cur_count and max_count:
             progress += '/'
         if max_count:
             progress += str(int(max_count))
         if cur_count and max_count:
             max_c = max_count or 100
-            progress = '{:3.0%} ({})'.format(cur_count / max_c, progress)
+            progress = f'{cur_count / max_c:3.0%} ({progress})'
         if message:
             if message.startswith(', '):
                 message = message[2:]
             message = ' - ' + message
         else:
             message = ''
         if self.inline and self.line_len > 0:
             if self.line_len < self.line_width:
-                self._print_without_nl('\r{}\r'.format(' ' * self.line_len))
+                self._print_without_nl(f'\r{" " * self.line_len}\r')
             else:
-                self._print_without_nl('\r{}\r'.format(' ' * (self.line_width - 1)))
+                self._print_without_nl(f'\r{" " * (self.line_width - 1)}\r')
                 self._print_without_nl(_CARET_UP)
-                self._print_without_nl('{}\r'.format(' ' * (self.line_width - 1)))
-        line = '{}{}{}'.format(description, progress, message)
+                self._print_without_nl(f'{" " * (self.line_width - 1)}\r')
+        line = f'{description}{progress}{message}'
         self.line_len = len(line)
         self._print_without_nl(line)
         self.printed_lines = True
 
     def finalize(self):
-        """This should be ran after the last progress report."""
+        """To be ran after the last progress report."""
         if self.printed_lines:
             if self.inline:
                 self._print_with_nl('')
             self.printed_lines = False
             self.line_len = 0
```

### Comparing `ingit-0.4.8/ingit/fetch_flags.py` & `ingit-0.4.9/ingit/fetch_flags.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,26 +28,25 @@
     for key, value in known_strings.items():
         if flags & key:
             info_strings.append(value)
     return info_strings
 
 
 def info_for_unknown_flags(flags: int, known_flags: int) -> t.MutableSequence[str]:
-    """Create string sequence that represents unknown flags according to given known flags mask.s"""
+    """Create string sequence that represents unknown flags according to given known flags mask."""
     info_strings = []
     unknown_flags = flags & ~(known_flags)
     if unknown_flags:
-        info_strings.append(
-            'unknown flag(s): {0} ({0:032b})'.format(unknown_flags))
+        info_strings.append(f'unknown flag(s): {unknown_flags} ({unknown_flags:032b})')
     return info_strings
 
 
 def create_fetch_info_strings(info: git.FetchInfo):
     """Create FetchInfo strings."""
     info_strings = info_for_known_flags(info.flags, _KNOWN_STRINGS)
     prefix = '!!'
     if info.flags & info.HEAD_UPTODATE:
         prefix = '--'
     info_strings += info_for_unknown_flags(info.flags, _KNOWN_FLAGS)
     if info.note:
-        info_strings.append('note: {0}'.format(info.note.strip()))
+        info_strings.append(f'note: {info.note.strip()}')
     return (info_strings, prefix)
```

### Comparing `ingit-0.4.8/ingit/main.py` & `ingit-0.4.9/ingit/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,206 +1,224 @@
 """Command-line interface of ingit."""
 
 import argparse
 import logging
 import pathlib
-import sys
 
 import argcomplete
 
-from ._version import VERSION
+from .config_boilerplate import initialize_config_directory
+from .cli_boilerplate import \
+    ArgumentDefaultsAndRawDescriptionHelpFormatter, make_copyright_notice, add_version_option, \
+    add_verbosity_group, get_verbosity_level, dedent_except_first_line
 from .json_config import RUNTIME_CONFIG_PATH, REPOS_CONFIG_PATH
 from .runtime import Runtime
 
 _LOG = logging.getLogger(__name__)
 
 PREDICATE_EXAMPLES = ['''name.startswith('py_')''', ''' 'python' in tags''']
 
 REGEX_EXAMPLES = ['^py_.*', '^python$']
 
 SUGGESTED_TAGS = [
     'appveyor', 'archived', 'assembla', 'bash', 'bitbucket', 'c', 'c++', 'c#', 'css', 'cython',
-    'docker', 'fortran', 'gist', 'github', 'html', 'java', 'latex', 'opencl', 'php', 'python',
-    'ruby', 'travis', 'vsonline']
+    'docker', 'fortran', 'gist', 'github', 'html', 'java', 'javascript', 'latex', 'opencl', 'php',
+    'python', 'ruby', 'travis', 'vsonline']
 
 OUT = logging.getLogger('ingit.interface.print')
 
 
 def prepare_parser():
     """Prepare command-line arguments parser."""
-
     parser = argparse.ArgumentParser(
         prog='ingit',
         description='''Tool for managing a large collection of repositories in git. If you have
         100 git-versioned projects, keeping tabs on everything can be quite troublesome.''',
-        epilog='''Copyright (C) 2015-2018 by Mateusz Bysiek,
-        GNU General Public License v3 or later (GPLv3+), https://github.com/mbdevpl/ingit''',
+        epilog=make_copyright_notice(
+            2015, 2022, license_name='GNU General Public License v3 or later (GPLv3+)',
+            url='https://github.com/mbdevpl/ingit'),
         formatter_class=argparse.ArgumentDefaultsHelpFormatter, allow_abbrev=True)
-    parser.add_argument('--version', action='version',
-                        version='ingit {}, Python {}'.format(VERSION, sys.version))
+    add_version_option(parser)
 
     interactivity_group = parser.add_mutually_exclusive_group(required=False)
     interactivity_group.add_argument(
         '--batch', '--non-interactive', dest='batch', action='store_true',
         help='run ingit in non-interactive mode')
     interactivity_group.add_argument(
         '--interactive', dest='batch', action='store_false',
         help='force interactive mode even if configuration sets batch mode as default')
     parser.set_defaults(batch=None)
 
-    verbosity_group = parser.add_mutually_exclusive_group(required=False)
-    verbosity_group.add_argument(
-        '--verbose', '-v', action='count',
-        help='ingit should be more verbose than by default'
-        ' (repeat up to 2 times for stronger effect)')
-    verbosity_group.add_argument(
-        '--quiet', '-q', action='count',
-        help='ingit should be more quiet than by default'
-        ' (repeat up to 3 times for stronger effect)')
-    verbosity_group.add_argument(
-        '--verbosity', metavar='LEVEL', type=int, default=logging.CRITICAL - logging.WARNING,
-        help='set verbosity level explicitly (normally from {} to {})'
-        .format(logging.CRITICAL - logging.CRITICAL, logging.CRITICAL - logging.NOTSET))
+    add_verbosity_group(parser)
 
     parser.add_argument(
         '--config', metavar='PATH', type=str, default=str(RUNTIME_CONFIG_PATH),
         help='''path to the runtime configuration file;
         can be absolute, or relative to current woking directory''')
 
     parser.add_argument(
         '--repos', metavar='PATH', type=str, default=str(REPOS_CONFIG_PATH),
         help='''path to the projects list file;
         can be absolute, or relative to current woking directory''')
 
     parser.add_argument(
-        '--predicate', '-p', type=str, default=None, help='''a Python expression used to select
+        '--predicate', '-p', type=str, default=None, help=f'''a Python expression used to select
         repositories operated on; it is evaluated on each repository metadata;
-        examples: "{}"'''.format('", "'.join(PREDICATE_EXAMPLES)))
+        examples: "{'", "'.join(PREDICATE_EXAMPLES)}"''')
     parser.add_argument(
-        '--regex', '-r', type=str, default=None, help='''a regular expression used to select
+        '--regex', '-r', type=str, default=None, help=f'''a regular expression used to select
         repositories operated on; repository matches if any of its metadata match;
-        examples: "{}"'''.format('", "'.join(REGEX_EXAMPLES)))
+        examples: "{'", "'.join(REGEX_EXAMPLES)}"''')
 
     commands = {
         'summary': (
             'show summary of registered repositories and status of configured repository root',
-            '''First of all, print a list of registered repositories. By default, all registered
-            repositories are listed, but, as in case of most commands, the results can be filtered
-            via a predicate or regex. Independently, print a list of all unregistered repositories
-            and all not versioned paths present in the configured repositories root.'''),
+            '''First of all, print a list of registered repositories. By default, all
+            registered repositories are listed, but, as in case of most commands, the
+            results can be filtered via a predicate or regex.
+
+            Independently, print a list of all unregistered repositories and all not
+            versioned paths present in the configured repositories root.'''),
         'register': (
             'start tracking a repository in ingit',
             '''The initial configuration is set according to basic repository information:
-            its root directory name becomes "name" and its currently configured remotes become
-            "remotes". You can edit the configuration manually afterwards.
+            its root directory name becomes "name" and its currently configured remotes
+            become "remotes". You can edit the configuration manually afterwards.
 
             The final "path" to the repository stored in the configuration depends on the
-            "repos_path" in runtime configuation. The configured "path" will be:
+            "repos_path" in runtime configuration. The configured "path" will be:
 
-            (1) resolved absolute path if there is no "repos_path" configured or repository path
-                is outside of the "repos_path";
-            (2) resolved relative path to the "repos_path", if the repository path is within it;
-            (3) nothing (i.e. not stored) if the if the repository is stored directly in
+            *   resolved absolute path if there is no "repos_path" configured or
+                repository path is outside of the "repos_path";
+            *   resolved relative path to the "repos_path", if the repository path is
+                within it;
+            *   nothing (i.e. not stored) if the if the repository is stored directly in
                 "repos_path" (i.e. there are no intermediate directories).
 
             Behaviour of storing relative/no paths in some cases is implemented to make
-            configuration file much less verbose in typical usage scenarios. To prevent this
-            behaviour, and force all repository paths to be absolute, simply set the "repos_path"
-            in your runtime configuraion to JSON "null".'''),
+            configuration file much less verbose in typical usage scenarios. To prevent
+            this behaviour, and force all repository paths to be absolute, simply set the
+            "repos_path" in your runtime configuration to JSON "null".'''),
         'foreach': (
             'execute a custom command',
-            'The given command is executed in a shell in working directory of each project.'),
+            '''The given command is executed in a shell in working directory of each
+            project.'''),
         'clone': (
             'perform git clone',
-            '''Execute "git clone <remote-url> --recursive --orign <remote-name> <path>",
-            where values of <path> and <remote-...> are taken from default remote configuration
-            of the repository.
-            After cloning, add all remaining configured remotes to the repository and fetch them.
-            '''),
+            '''Execute "git clone <remote-url> --recursive --origin <remote-name> <path>",
+            where values of <path> and <remote-...> are taken from default remote
+            configuration of the repository.
+
+            After cloning, add all remaining configured remotes to the repository and
+            fetch them.'''),
         'init': (
-            'perofrm git init',
-            'Execute "git init", followed by "git remote add" for each configured remote.'),
+            'perform git init',
+            '''Execute "git init", followed by "git remote add" for each configured
+            remote.'''),
         'fetch': (
             'perform git fetch',
-            '''Execute "git fetch <remote-name>", where the remote name is the remote of the current
-            tracking branch, or all remotes of the repository if there's no tracking branch,
-            or repository is in detached head state.'''),
+            '''Execute "git fetch <remote-name>", where the remote name is the remote of
+            the current tracking branch, or all remotes of the repository if there's no
+            tracking branch, or repository is in detached head state.'''),
         'checkout': (
             'perform git checkout',
-            '''Interactively select revision to checkout from list of local branches,
-            remote non-tracking branches and local tags.'''),
+            '''Interactively select revision to checkout from list of local branches, remote
+            non-tracking branches and local tags.
+
+            The list of branches to select from is composed by combining:
+
+            *   local branches
+            *   non-tracking branches on all remotes
+            *   local tags
+
+            Checking out a remote branch will create a local branch with the same unless
+            it already exists. If it already exists, repository will end up in detached
+            head state.
+
+            Also, checking out any tag will put repository in a detached head state.'''),
         'merge': (
             'perform git merge (not yet implemented)',
-            '''Interactively merge all branches to their tracking branches.
-            For each <branch>-<tracking-branch> pair,
-            execute "git checkout <branch>" and then if the merge can be fast-forward,
-            automatically execute "git merge <tracking-branch> --ff-only".
-            If not, then show more information about the situation of the repository, and propose:
-            "git merge --log <tracking-branch>", "git rebase -i <tracking-branch>" and
-            "git reset --hard <tracking-branch>".
-            If repository is dirty when this command is executed, the command will do nothing.
-            After work is done, return to the originally checked-out branch.'''),
+            '''Not yet implemented! The following functionality is intended.
+
+            Interactively merge all branches to their tracking branches. For each not
+            merged <branch>-<tracking-branch> pair, execute
+            "git checkout <branch>" and then if the merge is fast-forward,
+            automatically execute "git merge <tracking-branch> --ff-only". If not, then
+            show more information about the situation of the repository, and propose:
+
+            *   "git merge --log <tracking-branch>",
+            *   "git rebase -i <tracking-branch>" and
+            *   "git reset --hard <tracking-branch>".
+
+            If repository is dirty when this command is executed, do nothing. After work
+            is done, return to the originally checked-out branch.'''),
         'push': (
             'perform git push (not yet fully implemented)',
-            '''Execute "git push <remote-name> <branch>:<tracking-branch-name>"
-            for the active branch.'''),
+            '''Execute "git push <remote-name> <branch>:<tracking-branch-name>" for the
+            active branch.'''),
         'gc': ('perform git gc', 'Execute "git gc --agressive --prune".'),
         'status': (
             'perform git status, as well as other diagnostic git commands',
-            '''Execute git status --short --branch to inform about any uncommited changes,
-            git log tracking_branch..branch to inform about commits that are not yet pushed
-            to the remote, and
-            git log branch..tracking_branch to inform about commits that are not yet merged
-            from the remote.
-            Additionally, compare registered remotes with actual remotes to make sure that ingit
-            configuration is in sync with the repository metadata.''')}
+            '''Perform git status, as well as other diagnostic git commands.
+
+            Execute:
+
+            *   "git status --short --branch" to inform about any uncommitted changes,
+            *   "git log tracking_branch..branch" to inform about commits that are not
+                yet pushed to the remote,
+            *   "git log branch..tracking_branch" to inform about commits that are not
+                yet merged from the remote.
+
+            Additionally, compare registered remotes with actual remotes to make sure
+            that ingit configuration is in sync with the repository metadata..''')}
 
     subparsers = parser.add_subparsers(
-        dest='command', metavar='command', help='''main command to execute; one of: "{}";
-        run "ingit command --help" to see detailed help for a given command'''
-        .format('", "'.join(commands.keys())))
+        dest='command', metavar='command', help=f'''main command to execute; one of:
+        "{'", "'.join(commands.keys())}";
+        run "ingit command --help" to see detailed help for a given command''')
 
     _prepare_command_subparsers(subparsers, commands)
     argcomplete.autocomplete(parser)
 
     return parser
 
 
 def _prepare_command_subparsers(subparsers, commands):
     for command, (help_, description) in commands.items():
-        subparser = subparsers.add_parser(command, help=help_)
-        subparser.description = description
+        subparser = subparsers.add_parser(
+            command, help=help_, formatter_class=ArgumentDefaultsAndRawDescriptionHelpFormatter)
+        subparser.description = dedent_except_first_line(description)
         if command == 'register':
             subparser.add_argument(
                 '--tags', metavar='TAG', type=str, default=None, nargs='+',
                 help='set tags for this repository, they will be added to initial configuration') \
                 .completer = argcomplete.completers.ChoicesCompleter(choices=SUGGESTED_TAGS)
             subparser.add_argument(
                 'path', metavar='PATH', type=str, nargs='?',
                 help='''path to root directory of repository, use current working directory
                 if not provided''')
         elif command == 'foreach':
             subparser.add_argument(
                 'cmd', metavar='COMMAND', type=str,
                 help='command to be executed in shell in working directory of each project')
+            # subparser.add_argument(
+            #     '--recursive', action='store_true',
+            #     help='(not yet implemented)')
             subparser.add_argument(
-                '--recursive', action='store_true',
-                help='')  # TODO: write help
-            subparser.add_argument(
-                '--timeout', metavar='SECONDS', type=int, default=None,
-                help='')  # TODO: write help
+                '--timeout', metavar='SECONDS', type=float, default=None,
+                help='timeout of the command (in seconds)')
         elif command == 'fetch':
             subparser.add_argument(
                 '--all', action='store_true',
                 help='fetch all remotes in all cases')
         elif command == 'push':
             subparser.add_argument(
                 '--all', action='store_true',
-                help='''execute the push for every branch that has a remote tracking branch
-                (not yet implemented)''')
+                help='''(not yet implemented) execute the push for every branch that has a remote
+                tracking branch''')
         elif command == 'status':
             subparser.add_argument(
                 '-i', '--ignored', action='store_true',
                 help='''include ignored files in the status report
                 (identical to "--ignored" flag on "git status")''')
 
 
@@ -208,53 +226,48 @@
     command_options = {}
     if command == 'register':
         command_options['tags'] = parsed_args.tags
         command_options['path'] = pathlib.Path(
             '.' if parsed_args.path is None else parsed_args.path)
     elif command == 'foreach':
         command_options['cmd'] = parsed_args.cmd
+        command_options['timeout'] = parsed_args.timeout
     elif command == 'fetch':
         command_options['all_remotes'] = parsed_args.all
     elif command == 'push':
         command_options['all_branches'] = parsed_args.all
     elif command == 'status':
         command_options['ignored'] = parsed_args.ignored
     return command_options
 
 
 def main(args=None):
     """Parse command line arguments and run ingit accordingly."""
-
     parser = prepare_parser()
     parsed_args = parser.parse_args(args)
     if (parsed_args.predicate is not None or parsed_args.regex is not None) \
             and parsed_args.command == 'register':
-        parser.error('project filtering is not applicable to "{}" command'
-                     ' -- it can be used only with summary command and with git-like commands'
-                     .format(parsed_args.command))
-
-    level = logging.CRITICAL
-    if parsed_args.verbose is not None:
-        level -= 10 * parsed_args.verbose
-    if parsed_args.quiet is not None:
-        level += 10 * parsed_args.quiet
-    if parsed_args.verbosity is not None:
-        level -= parsed_args.verbosity
+        parser.error(f'project filtering is not applicable to "{parsed_args.command}" command'
+                     ' -- it can be used only with summary command and with git-like commands')
+
+    level = logging.CRITICAL - 10 * get_verbosity_level(parsed_args)
     OUT.setLevel(level)
     assert level == OUT.getEffectiveLevel(), (level, OUT.getEffectiveLevel())
 
     OUT.info('parsed args: %s', parsed_args)
 
+    initialize_config_directory('ingit')
+
     runtime_config_path = pathlib.Path(parsed_args.config)
     repos_config_path = pathlib.Path(parsed_args.repos)
 
     if parsed_args.predicate is None:
         predicate = None
     else:
-        predicate_code = "lambda name, tags, path, remotes: ({})".format(parsed_args.predicate)
+        predicate_code = f"lambda name, tags, path, remotes: ({parsed_args.predicate})"
         _LOG.warning('prepared predicate lambda: %s', predicate_code)
         predicate = eval(predicate_code)
 
     if parsed_args.regex is None:
         regex = None
     else:
         regex = parsed_args.regex
```

### Comparing `ingit-0.4.8/ingit/project.py` & `ingit-0.4.9/ingit/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Single project."""
 
 import collections
+import collections.abc
 import logging
 import pathlib
 import typing as t
 
 import git
 
 from .json_config import normalize_path
@@ -22,138 +23,139 @@
 
 
 def normalize_url(url: str):
     return normalize_path(url)
 
 
 class Project:
-
     """Single project."""
 
     def __init__(self, name: str, tags: t.Iterable[str], path: pathlib.Path,
                  remotes: t.Mapping[str, str]):
         assert isinstance(name, str), type(name)
         assert isinstance(tags, collections.abc.Iterable), type(tags)
         assert isinstance(path, pathlib.Path), type(path)
         assert isinstance(remotes, collections.abc.Mapping), type(remotes)
         self.name = name
-        self.tags = {tag for tag in tags}
+        self.tags = set(tags)
         self.path = path
-        self.remotes = collections.OrderedDict([(k, v) for k, v in remotes.items()])
+        self.remotes = collections.OrderedDict(list(remotes.items()))
 
-        self.repo = None
+        self.repo: t.Optional[RepoData] = None
 
     @property
     def is_existing(self) -> bool:
-        """True if this project's working directory exists."""
+        """Return True if this project's working directory exists."""
         return self.path.is_dir()
 
     @property
     def has_git_folder(self) -> bool:
-        """True if repo has .git folder."""
+        """Return True if repo has .git folder."""
         return self.path.joinpath('.git').is_dir()
 
     @property
     def has_git_file(self) -> bool:
-        """True if repo has .git file."""
+        """Return True if repo has .git file."""
         return self.path.joinpath('.git').is_file()
 
     @property
     def has_git_folder_or_file(self) -> bool:
-        """True if repo has .git folder or it has .git file."""
+        """Return True if repo has .git folder or it has .git file."""
         return self.has_git_folder or self.has_git_file
 
     @property
     def is_initialised(self) -> bool:
-        """True if repo exists."""
+        """Return True if repo exists."""
         return self.is_existing and self.has_git_folder_or_file
 
     def link_repo(self):
+        assert self.repo is None, self.repo
         self.repo = RepoData(git.Repo(normalize_path(str(self.path))))
 
     def clone(self) -> None:
-        """Execute "git clone --recursive --orign <remote-name> <remote-url> <path>".
+        """Execute "git clone --recursive --origin <remote-name> <remote-url> <path>".
 
         All of the <...> values are taken from project configuration.
         Values of <remote-...> are taken from default remote.
 
         This is followed by "git remote add <remote-name> <remote-url>" for all additional
         configured remotes.
         """
         if self.is_initialised:
-            OUT.info('repo {} already initialised'.format(self.path))
+            OUT.info('repo %s already initialised', self.path)
             return
         if self.is_existing:
             raise ValueError('directory already exists... please check, delete it, and try again')
 
         remotes = list(self.remotes.items())
         if not remotes:
-            raise ValueError('no configured remotes in repo {}... cannot clone'.format(self.path))
+            raise ValueError(f'no configured remotes in repo {self.path}... cannot clone')
         (remote_name, remote_url), remaning_remotes = remotes[0], remotes[1:]
 
-        if ask('Execute "git clone {} --recursive --origin={} {}"?'
-               .format(remote_url, remote_name, self.path)) != 'y':
-            OUT.warning('skipping {}'.format(self.path))
+        if ask(f'Execute "git clone {remote_url} --recursive --origin={remote_name}'
+               f' {self.path}"?') != 'y':
+            OUT.warning('skipping %s', self.path)
             return
 
         try:
             progress = ActionProgress()
             self.repo = RepoData(git.Repo.clone_from(
                 normalize_url(remote_url), normalize_path(str(self.path)), recursive=True,
                 origin=remote_name, progress=progress))
             progress.finalize()
         except git.GitCommandError as err:
-            raise ValueError('error while cloning "{}" into "{}"'
-                             .format(remote_url, self.path)) from err
+            raise ValueError(f'error while cloning "{remote_url}" into "{self.path}"') from err
 
         for remote_name, remote_url in remaning_remotes:
             self.repo.git.remote('add', remote_name, normalize_url(remote_url))
             self.repo.refresh()
             self._fetch_remote(remote_name)
 
     def init(self) -> None:
         """Execute "git init".
 
         This is followed by "git remote add <remote-name> <remote-url>" for each configured remote.
         """
         if self.is_initialised:
-            OUT.error('repo {} already initialised'.format(self.path))
+            OUT.error('repo %s already initialised', self.path)
             return
         if self.is_existing:
             raise ValueError('directory already exists... please check, delete it, and try again')
 
-        if ask('Execute "git init {}"?'.format(self.path)) != 'y':
-            OUT.warning('skipping {}'.format(self.path))
+        if ask(f'Execute "git init {self.path}"?') != 'y':
+            OUT.warning('skipping %s', self.path)
             return
 
         self.repo = RepoData(git.Repo.init(normalize_path(str(self.path))))
 
         for remote_name, remote_url in self.remotes.items():
             self.repo.git.remote('add', remote_name, normalize_url(remote_url))
 
     def fetch(self, all_remotes: bool = False) -> None:
-        """Execute "git fetch --prune" on a remote of trancking branch of current branch.
+        """Execute "git fetch --prune" on a remote of tracking branch of current branch.
 
         Or execute "git fetch --prune" for all remotes.
         """
         if not self.is_existing:
             OUT.info('skipping non-existing "%s"...', self.path)
             return
         if self.repo is None:
             self.link_repo()
+        assert self.repo is not None
         self.repo.refresh()
 
         if all_remotes:
             remote_names = self.repo.remotes
         else:
             remote_names = self._determine_remotes_to_fetch()
 
         self._fetch_remotes(*remote_names)
 
     def _determine_remotes_to_fetch(self):
+        assert self.repo is not None
         if self.repo.active_branch is None:
             OUT.warning('!! "%s" is not on any branch, fetching all remotes', self.path)
             return self.repo.remotes
         try:
             remote_name, _ = self.repo.tracking_branches[self.repo.active_branch]
         except KeyError:
             _LOG.warning('branch "%s" in "%s" not configured, fetching all remotes',
@@ -162,133 +164,136 @@
         except TypeError:
             OUT.warning('!! branch "%s" in "%s" has no tracking branch, fetching all remotes',
                         self.repo.active_branch, self.path)
             return self.repo.remotes
         return [remote_name]
 
     def _fetch_remote(self, remote_name: str) -> None:
-        fetch_infos = None  # type: t.Sequence[git.FetchInfo]
+        assert self.repo is not None
+        fetch_infos: t.Sequence[git.FetchInfo]
         try:
             progress = ActionProgress()
             fetch_infos = self.repo.remotes[remote_name].fetch(prune=True, progress=progress)
             progress.finalize()
         except git.GitCommandError as err:
-            raise ValueError('error while fetching remote "{}" ("{}") in "{}"'.format(
-                remote_name, self.repo.remotes[remote_name].url, self.name)) from err
+            raise ValueError(f'error while fetching remote "{remote_name}"'
+                             f' ("{self.repo.remotes[remote_name].url}") in "{self.name}"') from err
         if not fetch_infos:
             _LOG.warning('no fetch info after fetching from remote "%s" in "%s"',
                          remote_name, self.name)
         for fetch_info in fetch_infos:
             self._print_fetch_info(fetch_info)
             if fetch_info.flags & fetch_info.FAST_FORWARD:
                 # ans = ask('The fetch was fast-forward. Do you want to merge?')
                 # if ans == 'y':
                 #    raise NotImplementedError('merging not yet implemented')
                 pass
         # return fetch_infos
 
-    def _fetch_remotes(self, *remote_names: t.Sequence[str]) -> None:
+    def _fetch_remotes(self, *remote_names: str) -> None:
         for remote_name in remote_names:
             self._fetch_remote(remote_name)
 
     def _print_fetch_info(self, fetch_info: git.FetchInfo) -> None:
         info_strings, prefix = create_fetch_info_strings(fetch_info)
         if not info_strings:
             return
         level = logging.WARNING if fetch_info.flags & git.FetchInfo.HEAD_UPTODATE \
             else logging.CRITICAL
-        OUT.log(level, '{} fetched "{}" in "{}"; {}'.format(
-            prefix, fetch_info.ref, self.name, ', '.join(info_strings)))
+        OUT.log(level, '%s fetched "%s" in "%s"; %s',
+                prefix, fetch_info.ref, self.name, ', '.join(info_strings))
 
     def checkout(self) -> None:
         """Interactively select revision and execute "git checkout <revision>" on it.
 
-        The list of branches to select from is composed by combinig:
+        The list of branches to select from is composed by combining:
         - local branches
         - non-tracking branches on all remotes
         - local tags
         """
         if not self.is_existing:
             OUT.info('skipping non-existing "%s"...', self.path)
             return
         if self.repo is None:
             self.link_repo()
+        assert self.repo is not None
         self.repo.refresh()
 
         # if self.is_on_only_branch():
         #    return
 
         keys = r'1234567890abcdefghijklmopqrstuvwxz' \
             r'ABCDEFGHIJKLMOPRSTUVWXZ' \
             r''',.!?*&^%$#@;:'"/|\()[]<>{}-_+=~`'''
         revisions = self._prepare_checkout_list(keys)
 
         print('Checkout options:')
         for key, (revision, comment) in revisions.items():
             if comment is None:
-                print('  {}: {}'.format(key, revision))
+                print(f'  {key}: {revision}')
             else:
-                print('  {}: {} ({})'.format(key, revision, comment))
+                print(f'  {key}: {revision} ({comment})')
 
         answer = ask('Which branch to checkout?', answers=list(keys[:len(revisions)] + 'n'))
         if answer == 'n':
             return
         target, _ = revisions[answer]
         if target == self.repo.active_branch:
             return
 
         self.repo.git.checkout(target)
 
     def _prepare_checkout_list(self, keys: str):
+        assert self.repo is not None
         revisions = collections.OrderedDict()
 
         local_branches = list(self.repo.branches)
         remote_tracking_branches = set(self.repo.tracking_branches.values())
         remote_nontracking_branches = [
-            (remote, branch) for remote, branch in self.repo.remote_branches
+            (remote, branch) for remote, branch in self.repo.remote_branches.items()
             if (remote, branch) not in remote_tracking_branches and branch not in _SPECIAL_REFS]
         local_tags = list(self.repo._repo.tags)
 
-        all_candidates = local_branches + remote_nontracking_branches + local_tags
-        if len(all_candidates) > len(keys):
+        all_candidates_count: int = \
+            len(local_branches) + len(remote_nontracking_branches) + len(local_tags)
+        if all_candidates_count > len(keys):
             raise RuntimeError(
                 'not enough available keys to create a single list of checkout candidates'
-                ' - there are {} keys ("{}") but {} candidates:\n- branches:{}, {}\n- tags: {}'
-                .format(len(keys), keys, len(all_candidates), local_branches,
-                        remote_nontracking_branches, local_tags))
+                f' - there are {len(keys)} keys ("{keys}") but {all_candidates_count} candidates:'
+                f'\n- branches:{local_branches}, {remote_nontracking_branches}'
+                f'\n- tags: {local_tags}')
 
         index = 0
         for branch in self.repo.branches:
             revisions[keys[index]] = (branch, None)
             index += 1
 
         for tag in self.repo._repo.tags:
             revisions[keys[index]] = (tag, 'tag')
             index += 1
 
-        for (remote, branch) in self.repo.remote_branches:
-            # remote_branch = '{}/{}'.format(remote, branch)
+        for (remote, branch) in self.repo.remote_branches.items():
             if (remote, branch) in remote_tracking_branches \
                     or branch in _SPECIAL_REFS:
                 continue
             if branch in self.repo.branches:
-                to_checkout = '{}/{}'.format(remote, branch)
+                to_checkout = f'{remote}/{branch}'
             else:
                 to_checkout = branch
-            revisions[keys[index]] = (to_checkout, 'based on {}'.format(remote))
+            revisions[keys[index]] = (to_checkout, f'based on {remote}')
             index += 1
 
         if self.repo.active_branch is None:
             revisions['n'] = ('---', 'keep no branch/tag')
         else:
             # assert revisions['1'][0] == active_branch
             for key, (revision, comment) in revisions.items():
                 if revision == self.repo.active_branch:
                     _ = 'no change'
-                    comment = '{}, {}'.format(comment, _) if comment else _
+                    comment = f'{comment}, {_}' if comment else _
                     revisions[key] = (revision, comment)
                     break
 
         return revisions
 
     def merge(self) -> None:
         """Execute "git merge" for current branch."""
@@ -305,25 +310,26 @@
         Or, push all local branches to their tracking branches.
         """
         if not self.is_existing:
             OUT.info('skipping non-existing "%s"...', self.path)
             return
         if self.repo is None:
             self.link_repo()
+        assert self.repo is not None
 
         branches_to_push = []  # type: t.List[str]
 
         if all_branches:
             raise NotImplementedError('pushing not yet implemented')
-        else:
-            if self.repo.active_branch is None:
-                OUT.warning('not pushing "%s" because there is no active branch...', self.path)
-                return
-            else:
-                branches_to_push.append(self.repo.active_branch)
+
+        if self.repo.active_branch is None:
+            OUT.warning('not pushing "%s" because there is no active branch...', self.path)
+            return
+
+        branches_to_push.append(self.repo.active_branch)
 
         pushed_branches_per_remote = {}  # type: t.Dict[str, t.Dict[str, t.Optional[str]]]
         for local_branch in branches_to_push:
             tracking_branch = self.repo.tracking_branches[local_branch]
             if tracking_branch is None:
                 remote = next(iter(self.repo.remotes.keys()))
                 OUT.warning('pushing "%s" to "%s"...', self.path, remote)
@@ -339,136 +345,150 @@
             push_infos = self._push_single_remote(remote_name, branch_mapping)
             for push_info in push_infos:
                 self._print_push_info(push_info)
 
     def _push_single_remote(
             self, remote_name: str,
             branch_mapping: t.Mapping[str, t.Optional[str]]) -> t.Sequence[git.PushInfo]:
-        push_refspec = ['{}'.format(local_branch) if remote_branch is None
-                        else '{}:{}'.format(local_branch, remote_branch)
+        assert self.repo is not None
+        push_refspec = [f'{local_branch}' if remote_branch is None
+                        else f'{local_branch}:{remote_branch}'
                         for local_branch, remote_branch in branch_mapping.items()]
         _LOG.warning('push refspec: %s', push_refspec)
         try:
             progress = ActionProgress()
             push_infos = self.repo.remotes[remote_name].push(
                 refspec=push_refspec, with_extended_output=True, progress=progress)
             progress.finalize()
         except git.GitCommandError as err:
-            raise ValueError('error while pushing branches {} to remote "{}" ("{}") in "{}"'.format(
-                branch_mapping, remote_name, self.repo.remotes[remote_name].url,
-                self.name)) from err
+            raise ValueError(
+                f'error while pushing branches {branch_mapping} to remote "{remote_name}"'
+                f' ("{self.repo.remotes[remote_name].url}") in "{self.name}"') from err
         return push_infos
 
     def _print_push_info(self, push_info: git.PushInfo) -> None:
         info_strings, prefix = create_push_info_strings(push_info)
         if not info_strings:
             return
         level = logging.WARNING if push_info.flags & git.PushInfo.UP_TO_DATE \
             else logging.CRITICAL
-        OUT.log(level, '{} pushed "{}" to "{}" in "{}"; {}'.format(
-            prefix, push_info.local_ref, push_info.remote_ref, self.name, ', '.join(info_strings)))
+        OUT.log(level, '%s pushed "%s" to "%s" in "%s"; %s', prefix, push_info.local_ref,
+                push_info.remote_ref, self.name, ', '.join(info_strings))
 
     def collect_garbage(self) -> None:
         """Execute "git gc --agressive --prune"."""
         if not self.is_existing:
             OUT.info('skipping non-existing "%s"...', self.path)
             return
         if self.repo is None:
             self.link_repo()
+        assert self.repo is not None
 
         try:
             self.repo.git.gc(aggressive=True, prune=True)
         except git.GitCommandError as err:
-            raise ValueError('error while collecting garbage in "{}"'.format(self.path)) from err
+            raise ValueError(f'error while collecting garbage in "{self.path}"') from err
 
     def status(self, ignored: bool = False) -> None:
         """Execute "git status --short" and run "git gui" if there is any output.
 
         The "ignored" flag is equivalent to adding "--ignored".
         """
         if not self.is_existing:
             OUT.info('skipping non-existing "%s"...', self.path)
             return
         if self.repo is None:
             self.link_repo()
+        assert self.repo is not None
 
         try:
             status_log = self.repo.git.status(short=True, branch=True, ignored=ignored).splitlines()
         except git.GitCommandError as err:
-            raise ValueError('error while getting status of "{}"'.format(self.path)) from err
+            raise ValueError(f'error while getting status of "{self.path}"') from err
 
         if len(status_log) > 1:
-            OUT.critical('!! unclear status in "{}":'.format(self.path))
+            OUT.critical('!! unclear status in "%s":', self.path)
             for line in status_log:
                 OUT.critical(line)
 
         self.repo.refresh()
         self._status_branch()
         self._status_remotes()
 
     def _get_log(self, start_ref: str, end_ref: str) -> str:
         """Get log as if start_ref..end_ref was used."""
-        refs = '{}..{}'.format(start_ref, end_ref)
-        # return self.repo.git.log('--pretty=oneline', refs, color='always').splitlines()
-        return self.repo.git.log('--color=always', '--pretty=oneline', refs).splitlines()
+        assert self.repo is not None
+        refs = f'{start_ref}..{end_ref}'
+        try:
+            git_log = self.repo.git.log('--color=always', '--pretty=oneline', refs)
+        except git.GitCommandError as err:
+            raise RuntimeError(f'error while getting log for "{refs}" of "{self.path}"') from err
+        return git_log.splitlines()
 
     def _print_log(self, ref_log, printed_header: str = '', head_count: int = 10,
                    tail_count: int = 10) -> None:
         if printed_header:
             OUT.critical(printed_header)
         if len(ref_log) > head_count + tail_count + 1:
             for line in ref_log[:head_count]:
                 OUT.critical(line)
             OUT.critical(
-                '... skipped {} commits'.format(len(ref_log) - head_count - tail_count))
+                '... skipped %i commits', len(ref_log) - head_count - tail_count)
             for line in ref_log[-tail_count:]:
                 OUT.critical(line)
         else:
             for line in ref_log:
                 OUT.critical(line)
 
     def _status_branch(self, branch: str = None) -> None:
         """Evaluate the status of single branch by comparing it to the remote branch.
 
         auto-answers used in this function: create_remote_branch, push, merge, forget_locally
         """
+        assert self.repo is not None
         if branch is None:
             branch = self.repo.active_branch
         if branch is None:
             OUT.warning('cannot diagnose branch status in "%s" -- not on any branch', self.path)
             return
         tracking_branch_data = self.repo.tracking_branches[branch]
         if tracking_branch_data is None:
             OUT.warning('cannot diagnose branch status in "%s"'
                         ' -- current branch has no tracking branch', self.path)
             return
         tracking_branch = '/'.join(tracking_branch_data)
+        try:
+            self.repo.git.rev_parse(tracking_branch)
+        except:
+            OUT.warning(
+                'cannot diagnose branch status in "%s"'
+                ' -- tracking branch of the current branch does not exist', self.path)
+            return
         not_pushed_log = self._get_log(tracking_branch, branch)
         if not_pushed_log:
-            self._print_log(not_pushed_log, '!! not pushed commits from "{}" to "{}" in "{}":'
-                            .format(branch, tracking_branch, self.path))
+            self._print_log(not_pushed_log, f'!! not pushed commits from "{branch}"'
+                            f' to "{tracking_branch}" in "{self.path}":')
             # self.push_single_remote(
-            #    tracking_branch_data[0], ['{0}:{0}'.format(branch, tracking_branch_data[1])])
+            #    tracking_branch_data[0], ['{0}:{0}'.for.mat(branch, tracking_branch_data[1])])
         not_merged_log = self._get_log(branch, tracking_branch)
         if not_merged_log:
-            self._print_log(not_merged_log, '!! not merged commits from "{}" to "{}" in "{}":'
-                            .format(tracking_branch, branch, self.path))
-            '''
-            answer = self.interface.get_answer('merge')
-            if answer in ['y', 'm']:
-                self.merge_single_branch(remote, branch)
-            elif answer == 'b':
-                self.rebase_single_branch(remote, branch)
-            elif answer == 'r':
-                self.hard_reset_single_branch(remote, branch)
-            elif self.interface.confirm('forget_locally'):
-                self.repo.git.update_ref('refs/remotes/{0}/{1}'.format(remote, branch), branch)
-            '''
+            self._print_log(not_merged_log, f'!! not merged commits from "{tracking_branch}"'
+                            f' to "{branch}" in "{self.path}":')
+            # answer = self.interface.get_answer('merge')
+            # if answer in ['y', 'm']:
+            #     self.merge_single_branch(remote, branch)
+            # elif answer == 'b':
+            #     self.rebase_single_branch(remote, branch)
+            # elif answer == 'r':
+            #     self.hard_reset_single_branch(remote, branch)
+            # elif self.interface.confirm('forget_locally'):
+            #     self.repo.git.update_ref(f'refs/remotes/{remote}/{branch}', branch)
 
     def _status_remotes(self):
+        assert self.repo is not None
         assert all(len(list(v.urls)) == 1 for v in self.repo.remotes.values()), self.repo.remotes
         remote_names_in_config = set(self.remotes)
         remote_names = set(self.repo.remotes)
         remotes_in_config = {k: v.replace('\\', '/') for k, v in self.remotes.items()}
         remotes = {k: tuple(v.urls)[0].replace('\\', '/') for k, v in self.repo.remotes.items()}
 
         extra_remote_names = remote_names - remote_names_in_config
@@ -479,49 +499,46 @@
             return
         OUT.critical('!! repo "%s" has different remotes than it should', self.path)
 
         for name, url in extra_remotes.items():
             if url in missing_remotes.values():
                 OUT.critical('!! renamed remote: "%s"', name)
                 new_name = [k for k, v in missing_remotes.items() if url == v][0]
-                ans = ask('Rename remote from "{}" to "{}"?'
-                          .format(name, new_name))
+                ans = ask(f'Rename remote from "{name}" to "{new_name}"?')
                 if ans == 'y':
                     self.repo.git.remote('rename', name, new_name)
                     del missing_remotes[new_name]
             elif name in missing_remotes.keys():
                 OUT.critical('!! url changed for remote: "%s"', name)
-                ans = ask('Change URL of remote "{}" from "{}" to "{}"?'
-                          .format(name, url, remotes_in_config[name]))
+                ans = ask(f'Change URL of remote "{name}" from "{url}"'
+                          f' to "{remotes_in_config[name]}"?')
                 if ans == 'y':
                     self.repo.git.remote('set-url', name, remotes_in_config[name])
                     del missing_remotes[name]
             else:
                 OUT.critical('!! extra remote: "%s"', name)
                 if name not in extra_remote_names:
                     OUT.critical('!! misconfigured remote: "%s"', name)
                     continue
-                ans = ask('Remove remote "{}" with url "{}"?'
-                          .format(name, remotes[name]))
+                ans = ask(f'Remove remote "{name}" with url "{remotes[name]}"?')
                 if ans == 'y':
                     self.repo.git.remote('remove', name)
 
         for name, url in missing_remotes.items():
             OUT.critical('!! missing remote: "%s"', name)
             if name not in missing_remote_names:
                 OUT.critical('!! misconfigured remote: "%s"', name)
                 continue
-            ans = ask('Add remote "{}" with url "{}"?'
-                      .format(name, self.remotes[name]))
+            ans = ask(f'Add remote "{name}" with url "{self.remotes[name]}"?')
             if ans == 'y':
                 self.repo.git.remote('add', name, self.remotes[name])
 
     def __str__(self):
-        fields = ['path="{}"'.format(self.path)]
+        fields = [f'path="{self.path}"']
         if not self.is_initialised:
             if not self.is_existing:
                 fields.append('not existing')
             else:
                 fields.append('not initialized')
         if self.tags:
-            fields.append('tags={}'.format(self.tags))
-        return '{} ({})'.format(self.name, ', '.join(fields))
+            fields.append(f'tags={self.tags}')
+        return f'{self.name} ({", ".join(fields)})'
```

### Comparing `ingit-0.4.8/ingit/push_flags.py` & `ingit-0.4.9/ingit/push_flags.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     """Create PushInfo strings."""
     info_strings = info_for_known_flags(info.flags, _KNOWN_STRINGS)
     prefix = '!!'
     if info.flags & info.UP_TO_DATE:
         prefix = '--'
     info_strings += info_for_unknown_flags(info.flags, _KNOWN_FLAGS)
     if info.summary:
-        info_strings.append('summary: {0}'.format(info.summary.strip()))
+        info_strings.append(f'summary: {info.summary.strip()}')
     return (info_strings, prefix)
```

### Comparing `ingit-0.4.8/ingit/repo_data.py` & `ingit-0.4.9/ingit/repo_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,75 +7,98 @@
 
 import git
 
 _LOG = logging.getLogger(__name__)
 
 
 class RepoData:
-
     """Gather and validate data of a git repository."""
 
     def __init__(self, repo: git.Repo):
         assert isinstance(repo, git.Repo), type(repo)
         self._repo = repo
-        self.remotes = {}  # type: t.Mapping[str, git.Remote]
-        self.branches = {}  # type: t.Mapping[str, git.Reference]
-        self.active_branch = None  # type: str
-        self.remote_branches = {}  # type: t.Mapping[str, git.Reference]
-        self.tracking_branches = {}  # type: t.Mapping[str, git.Reference]
+        self.remotes: t.Mapping[str, git.Remote] = {}
+        self.branches: t.Mapping[str, git.Reference] = {}
+        self._active_branch: t.Optional[str] = None
+        self._current_tracking_branch: t.Optional[str] = None
+        self.remote_branches: t.Mapping[str, git.Reference] = {}
+        self.tracking_branches: t.Mapping[str, git.Reference] = {}
 
     @property
     def git(self):
         return self._repo.git
 
+    @property
+    def active_branch(self) -> t.Optional[str]:
+        return self._active_branch
+
+    @active_branch.setter
+    def active_branch(self, branch_name: t.Optional[str]) -> None:
+        self._active_branch = branch_name
+        self._current_tracking_branch = None
+        if branch_name is None:
+            return
+        current_tracking_ref = None
+        try:
+            current_tracking_ref = self._repo.active_branch.tracking_branch()
+        except AttributeError:
+            _LOG.warning('current branch "%s" in %s has no tracking branch',
+                         self._active_branch, self._repo)
+        if current_tracking_ref is not None:
+            self._current_tracking_branch = str(current_tracking_ref)
+
+    @property
+    def current_tracking_branch(self) -> t.Optional[str]:
+        """Get the tracking branch of the current branch, if any."""
+        return self._current_tracking_branch
+
+    @property
+    def default_remote(self) -> t.Optional[str]:
+        """Get the default remote name.
+
+        Default remote name would be the remote name of the tracking branch of the current branch.
+        It's None if the current branch has no tracking branch, or if there's no current branch.
+        """
+        if self._current_tracking_branch is None:
+            return None
+        return self._current_tracking_branch.partition('/')[0]
+
     def refresh(self) -> None:
         """Refresh repository data."""
-
         self.active_branch = None
         try:
             if self._repo.branches:
                 self.active_branch = str(self._repo.active_branch)
         except TypeError:
             _LOG.warning('repository %s is not on any branch', self._repo)
 
-        current_tracking_branch = None
-        default_remote = None
-        if self.active_branch is not None:
-            try:
-                current_tracking_branch = self._repo.active_branch.tracking_branch()
-                if current_tracking_branch is not None:
-                    current_tracking_branch = str(current_tracking_branch)
-                default_remote = current_tracking_branch.partition('/')[0]
-            except AttributeError:
-                _LOG.warning('current branch "%s" in %s has no tracking branch',
-                             self.active_branch, self._repo)
-
-        self.branches = collections.OrderedDict([] if self.active_branch is None
-                                                else [(self.active_branch, None)])
+        self.branches = collections.OrderedDict([] if self._active_branch is None
+                                                else [(self._active_branch, None)])
         self.branches.update(collections.OrderedDict([(str(_), _) for _ in self._repo.branches]))
         assert all(_ is not None for name, _ in self.branches.items()), (self._repo, self.branches)
 
         self.tracking_branches = {
             name: (tuple(str(_.tracking_branch()).partition('/')[::2])
                    if _.tracking_branch() else None)
             for name, _ in self.branches.items()}
 
+        default_remote = self.default_remote
         self.remotes = collections.OrderedDict([] if default_remote is None
                                                else [(default_remote, None)])
         self.remotes.update(collections.OrderedDict([(str(_), _) for _ in self._repo.remotes]))
 
         self.remote_branches = {
-            (remote_name, str(_).replace('{}/'.format(remote_name), '')): _
+            (remote_name, str(_).replace(f'{remote_name}/', '')): _
             for remote_name, remote in self.remotes.items() for _ in remote.refs}
 
-    def generate_repo_configuration(self) -> t.Mapping[str, t.Any]:
+    def generate_repo_configuration(self) -> t.Dict[str, t.Any]:
+        assert self._repo.working_tree_dir is not None
         path = pathlib.Path(self._repo.working_tree_dir)
         return {
             'name': path.name,
             'path': str(path.resolve()),
             'remotes': collections.OrderedDict(
                 [(name, remote.url) for name, remote in self.remotes.items()]),
             'tags': []}
 
     def __str__(self):
-        return '{}:(branches={},remotes={})'.format(
-            self._repo, self.tracking_branches, self.remotes)
+        return f'{self._repo}:(branches={self.tracking_branches},remotes={self.remotes})'
```

### Comparing `ingit-0.4.8/ingit/runtime.py` & `ingit-0.4.9/ingit/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The ingit runtime."""
 
-import collections
+import collections.abc
 import functools
 import logging
 import pathlib
 import platform
 import re
 import subprocess
 import typing as t
@@ -27,46 +27,34 @@
         re.search(regex, name) is not None
         or any(re.search(regex, tag) is not None for tag in tags)
         or re.search(regex, str(path)) is not None
         or any(re.search(regex, name) for name, url in remotes.items()))
 
 
 class Runtime:
-
     """The ingit runtime."""
 
     def __init__(self, runtime_config_path: pathlib.Path, repos_config_path: pathlib.Path,
                  hostname: str = None, interactive: t.Optional[bool] = None):
         self.runtime_config_path = runtime_config_path
         self.repos_config_path = repos_config_path
         self._hostname = platform.node() if hostname is None else hostname
-
-        self.runtime_config = None
-        self.repos_config = None
-        self._machine_config = None
         self._interactive = interactive
 
-        self.projects = None
-        self.filtered_projects = []
-
         # prepare, possibly interactive
-
         self.runtime_config = acquire_configuration(self.runtime_config_path, 'runtime')
         self._machine_config = self._read_machine_config()
-        # self.repos_path = pathlib.Path(normalize_path(self._machine_config['repos_path']))
-        # self.interactive = self._machine_config['interactive']
-        # if RuntimeInterfaceConfig.interactive is None:
-        #    runtime_config['']
 
         self.repos_config = acquire_configuration(self.repos_config_path, 'repos')
         self.projects = self._read_projects()
-        self.filtered_projects = [project for project in self.projects]
+        self.filtered_projects = list(self.projects)
 
     @property
     def repos_path(self):
+        """Get path to where repositories are by default."""
         raw_path = self._machine_config['repos_path']
         if raw_path is None:
             return None
         return pathlib.Path(normalize_path(raw_path))
 
     @property
     def interactive(self):
@@ -81,19 +69,18 @@
             if 'name' in machine:
                 names.append(machine['name'])
             else:
                 names += machine['names']
             if '' in names or self._hostname in names:
                 return machine
 
-        ans = ask('No matching machine for "{}" found in configuration. Add it?'
-                  .format(self._hostname))
+        ans = ask(f'No matching machine for "{self._hostname}" found in configuration. Add it?')
         if ans != 'y':
-            raise ValueError('No matching machine for "{}" found in configuration """{}"""'
-                             .format(self._hostname, self.runtime_config))
+            raise ValueError(f'No matching machine for "{self._hostname}"'
+                             f' found in configuration """{self.runtime_config}"""')
         machine = self.register_machine(self._hostname)
         return machine
 
     def _read_projects(self) -> t.Sequence[Project]:
         """Get list of all projects in repositories configuration."""
         projects = []
         for repo in self.repos_config['repos']:
@@ -108,25 +95,24 @@
                 raw_path = repo['paths']['']
             if raw_path is None:
                 path = pathlib.Path(name)
             else:
                 path = pathlib.Path(normalize_path(raw_path))
             if not path.is_absolute():
                 if self.repos_path is None:
-                    raise ValueError('configuration of repository "{}" must contain absolute path'
-                                     ' because repos_path in runtime configuration is not set'
-                                     .format(name))
+                    raise ValueError(f'configuration of repository "{name}" must contain absolute'
+                                     ' path because repos_path in runtime configuration is not set')
                 path = self.repos_path.joinpath(path)
             project = Project(name=name, tags=repo['tags'], path=path, remotes=repo['remotes'])
             projects.append(project)
         return projects
 
-    def filter_projects(self, predicate: t.Union[collections.Callable, str]):
+    def filter_projects(self, predicate: t.Union[collections.abc.Callable, str]):
         """Select subset of all of the projects registered projects for processing."""
-        assert isinstance(predicate, (collections.Callable, str)), type(predicate)
+        assert callable(predicate) or isinstance(predicate, str), type(predicate)
         if isinstance(predicate, str):
             predicate = functools.partial(regex_predicate, predicate)
         self.filtered_projects = [
             project for project in self.projects
             if predicate(project.name, project.tags, project.path, project.remotes)]
 
     def execute(self, command: str, **command_options):
@@ -143,116 +129,118 @@
             'push': self.execute_git_command,
             'gc': self.execute_git_command,
             'status': self.execute_git_command}[command]
 
         command_executor(command, **command_options)
 
     def execute_ingit_command(self, command: str, **command_options):
+        """Execute an ingit command, as opposed to a wrapper for a git built-in command."""
         command = {
             'summary': 'repositories_summary',
             'register': 'register_repository',
             'foreach': 'execute_command'}.get(command, command)
         implementation = getattr(self, command)
         implementation(**command_options)
 
     def execute_git_command(self, command: str, **command_options):
+        """Execute a wrapper for a git built-in command."""
         command = {
             'gc': 'collect_garbage'}.get(command, command)
         for project in self.filtered_projects:
             implementation = getattr(project, command)
             implementation(**command_options)
 
     def execute_command(self, cmd: str, timeout: int = None):
+        """Execute a command in each of the projects (after filtering was applied)."""
         for project in self.filtered_projects:
             if not project.path.is_dir():
                 continue
             try:
                 result = subprocess.run(cmd, timeout=timeout, shell=True, cwd=project.path)
                 if result.returncode != 0:
                     _LOG.error('command "%s" failed in %s: %s', cmd, project, result)
             except subprocess.TimeoutExpired:
                 _LOG.error('command "%s" in %s was aborted because it took too much time')
 
     def repositories_summary(self):
         """Summarize registered repositories."""
-
         all_count = len(self.filtered_projects)
         was_filtered = all_count < len(self.repos_config['repos'])
         if was_filtered:
-            print('Registered projects matching given conditions ({}):'.format(all_count))
+            print(f'Registered projects matching given conditions ({all_count}):')
         else:
-            print('All registered projects ({}):'.format(all_count))
+            print(f'All registered projects ({all_count}):')
         initialised_count = 0
         for project in self.filtered_projects:
             if project.is_initialised:
                 initialised_count += 1
             print(' -', project)
 
         if initialised_count == all_count:
             if all_count > 0:
                 print('All of them are initialised.')
             else:
                 print('')
         else:
-            print('{} of them are initialised ({} not).'
-                  .format(initialised_count, all_count - initialised_count))
+            print(f'{initialised_count} of them are initialised'
+                  f' ({all_count - initialised_count} not).')
 
         if self.repos_path is not None:
             self._unregistered_folders_summary()
 
     def _unregistered_folders_summary(self):
         assert self.repos_path is not None
         non_repo_paths_in_root = ordered_set.OrderedSet()
         unregistered_in_root = ordered_set.OrderedSet()
 
         project_paths_in_root = ordered_set.OrderedSet()
         for project in self.projects:
             try:
                 project_paths_in_root.add(project.path.relative_to(self.repos_path))
-            except:
+            except ValueError:
                 pass
 
         for path in self.repos_path.iterdir():
             if not path.is_dir():
                 continue
             try:
                 _ = git.Repo(str(path))
-            except git.exc.InvalidGitRepositoryError:
+            except git.InvalidGitRepositoryError:
                 # TODO: recurse into non-git dir here
                 non_repo_paths_in_root.add(path)
                 continue
             relative_path = path.relative_to(self.repos_path)
             if relative_path in project_paths_in_root:
                 continue
             unregistered_in_root.add(path)
 
         if unregistered_in_root:
-            print('There are {} unregistered git repositories in configured repositories root "{}".'
-                  .format(len(unregistered_in_root), self.repos_path))
+            print(f'There are {len(unregistered_in_root)} unregistered git repositories'
+                  f' in configured repositories root "{self.repos_path}".')
             for path in unregistered_in_root:
                 print(path)
 
         if non_repo_paths_in_root:
-            print('There are {} not versioned folders in configured repositories root "{}".'
-                  .format(len(non_repo_paths_in_root), self.repos_path))
+            print(f'There are {len(non_repo_paths_in_root)} not versioned folders'
+                  f' in configured repositories root "{self.repos_path}".')
             for path in non_repo_paths_in_root:
                 print(path)
 
     def register_machine(self, name: str) -> dict:
-        """Add machine to ingit runtime configuation."""
+        """Add machine to ingit runtime configuration."""
         assert isinstance(name, str), type(name)
         assert name
         for machine in self.runtime_config['machines']:
             names = []
             if 'name' in machine:
                 names.append(machine['name'])
             if 'names' in machine:
                 names += machine['names']
             if '' in names or name in names:
-                raise ValueError('machine "{}" already in configuration'.format(name))
+                raise ValueError(f'machine "{name}" already in configuration')
         machine_config = default_machine_configuration(name)
         _LOG.warning('adding machine to configuration: %s', machine_config)
         self.runtime_config['machines'].append(machine_config)
         json_to_file(self.runtime_config, self.runtime_config_path)
         return machine_config
 
     def register_repository(self, path: pathlib.Path, tags: t.Sequence[str]):
@@ -284,24 +272,24 @@
                                      self.repos_path, repo_path)
                 except ValueError:
                     _LOG.warning(
                         'resolved repo path "%s" is not within configured repos path "%s"'
                         ' - registering absolute path', absolute_repo_path, self.repos_path)
                     repo_config['path'] = str(absolute_repo_path)
         except ValueError:
-            _LOG.info('canot resolve repo path %s', repo_config['path'])
+            _LOG.info('cannot resolve repo path %s', repo_config['path'])
         if tags is not None:
             repo_config['tags'] += tags
         _LOG.warning('adding repo to configuration: %s', repo_config)
         index = None
         lowercase_name = repo_config['name'].lower()
         for i, project in enumerate(self.projects):
             lowercase_project_name = project.name.lower()
             if index is None and lowercase_project_name > lowercase_name:
                 index = i
             if lowercase_project_name == lowercase_name:
-                raise ValueError('project named {} already exists in current configuration'
-                                 .format(project.name))
+                raise ValueError(
+                    f'project named {project.name} already exists in current configuration')
         if index is None:
             index = len(self.projects)
         self.repos_config['repos'].insert(index, repo_config)
         json_to_file(self.repos_config, self.repos_config_path)
```

### Comparing `ingit-0.4.8/ingit/runtime_interface.py` & `ingit-0.4.9/ingit/runtime_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Interactive runtime interface of ingit."""
 
-import collections
 import collections.abc
 import logging
 import sys
 import typing as t
 
 import readchar
 
@@ -16,38 +15,41 @@
 
 OUT_HANDLER = logging.StreamHandler(sys.stdout)
 OUT_HANDLER.setLevel(logging.NOTSET)
 OUT.addHandler(OUT_HANDLER)
 
 
 def default_template(question, answers, default):
+    """Print a question with candidate answers, with the default marked accordingly.
+
+    This is the default template for ask().
+    """
     case_insensitive_answers = {_.lower() for _ in answers}
     case_insensitive = len(case_insensitive_answers) == len(answers)
     if case_insensitive:
         answers_print = [(a.upper() if a == default else a) for a in answers]
-        return '{} [{}] '.format(question, '/'.join(answers_print))
-    return '{} [{}] [default={}] '.format(question, '/'.join(answers), default)
+        return f'{question} [{"/".join(answers_print)}] '
+    return f'{question} [{"/".join(answers)}] [default={default}] '
 
 
-def ask(question: str, answers: t.Sequence[str] = None, default: str = None,
+def ask(question: str, answers: t.Sequence[str] = None, default: t.Optional[str] = None,
         autoanswer: t.Union[bool, str] = None,
-        template: collections.Callable = default_template) -> str:
+        template: collections.abc.Callable = default_template) -> str:
     """Ask a question that is to be answered with a single keystroke.
 
     By default, it is asked like this: "question [y/N] ".
 
-    @param question: a proposition that is to be answered
-    @param answers: list of valid answers, list of lower-case letters; if None, use ['y', 'n']
-    @param default:
+    :param question: a proposition that is to be answered
+    :param answers: list of valid answers, list of lower-case letters; if None, use ['y', 'n']
+    :param default:
         a default answer, lower-case letter; if None, use last of the answer, 'n' by default
-    @param autoanswer:
+    :param autoanswer:
         answer to be automatically given; if True, the default answer will be given
-    @param template: a function taking question and answers and returning string
-
-    @return: a lower-case letter that is the answer to the question
+    :param template: a function taking question and answers and returning string
+    :return: a lower-case letter that is the answer to the question
     """
     assert isinstance(question, str), type(question)
     if answers is None:
         answers = ['y', 'n']
     assert isinstance(answers, collections.abc.Sequence), type(answers)
     assert answers, answers
     assert all(
@@ -66,24 +68,25 @@
     assert autoanswer is None or autoanswer in answers, (autoanswer, answers)
     assert callable(template), type(template)
     # TODO: put this function in some library
     print(template(question, answers, default), end='', flush=True)
     case_insensitive_answers = {_.lower() for _ in answers}
     case_insensitive = len(case_insensitive_answers) == len(answers)
     if case_insensitive:
-        answers = case_insensitive_answers
+        answers = list(case_insensitive_answers)
         default = default.lower()
         if autoanswer is not None:
             autoanswer = autoanswer.lower()
     answer = autoanswer
     while answer not in answers:
         if answer is not None:
             print(answer, end='', flush=True)
         answer = readchar.readchar()
+        assert answer is not None
         if case_insensitive:
             answer = answer.lower()
         if answer in _INTERRUPTS:
             raise KeyboardInterrupt()
         if answer in _NEWLINES:
             answer = default
     print(answer)
-    return answer
+    return str(answer)
```

### Comparing `ingit-0.4.8/setup.py` & `ingit-0.4.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""This is setup.py file for ingit."""
+"""Setup script for ingit package."""
 
 import setup_boilerplate
 
 
 class Package(setup_boilerplate.Package):
-
     """Package metadata."""
 
     name = 'ingit'
     description = 'git repository collection management tool'
     url = 'https://github.com/mbdevpl/ingit'
     license_str = 'GNU General Public License v3 or later (GPLv3+)'
     classifiers = [
-        'Development Status :: 1 - Planning',
+        'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
-        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: MacOS',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Software Development :: Version Control',
         'Topic :: System :: Archiving :: Backup',
         'Topic :: System :: Archiving :: Mirroring',
         'Topic :: System :: Monitoring',
         'Topic :: Utilities'
         ]
```

### Comparing `ingit-0.4.8/setup_boilerplate.py` & `ingit-0.4.9/setup_boilerplate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,300 +1,377 @@
 """Below code is generic boilerplate and normally should not be changed.
 
-To avoid setup script boilerplate, create "setup.py" file with the minimal contents as given
-in SETUP_TEMPLATE below, and modify it according to the specifics of your package.
-
-See the implementation of setup_boilerplate.Package for default metadata values and available
-options.
-"""
-
-import pathlib
-import runpy
-import sys
-import typing as t
-
-import setuptools
+See the implementation of setup_boilerplate.Package for available options.
+Also, some fields have default values. See DEFAULT_* constants below for those values.
 
-__updated__ = '2019-06-04'
+To avoid setup script boilerplate, create "setup.py" file with the minimal contents as given
+below and modify it according to the specifics of your package.
+Note: string limiters need to be adjusted.
 
-SETUP_TEMPLATE = '''"""Setup script."""
+"" "Setup script." ""
 
 import setup_boilerplate
 
 
 class Package(setup_boilerplate.Package):
-
-    """Package metadata."""
+    "" "Package metadata." ""
 
     name = ''
     description = ''
     url = 'https://github.com/mbdevpl/...'
     classifiers = [
         'Development Status :: 1 - Planning',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3 :: Only']
     keywords = []
 
 
 if __name__ == '__main__':
     Package.setup()
-'''
+"""
+
+import logging
+import pathlib
+import runpy
+import sys
+import typing as t
+
+import docutils.frontend
+import docutils.nodes
+import docutils.parsers.rst
+import docutils.utils
+import setuptools
+
+__version__ = '2022.01.03'
+
+_LOG = logging.getLogger(__name__)
 
 HERE = pathlib.Path(__file__).resolve().parent
 
+DEFAULT_URL = 'https://github.com/mbdevpl'
+DEFAULT_AUTHOR = 'Mateusz Bysiek'
+DEFAULT_AUTHOR_EMAIL = 'mateusz.bysiek@gmail.com'
+DEFAULT_LICENSE_STR = 'Apache License 2.0'
+
 
 def find_version(
         package_name: str, version_module_name: str = '_version',
         version_variable_name: str = 'VERSION') -> str:
     """Simulate behaviour of "from package_name._version import VERSION", and return VERSION.
 
     To avoid importing whole package only to read the version, just module containing the version
     is imported. Therefore relative imports in that module will break the setup.
+
+    :param package_name: name of the package
+    :param version_module_name: name of the module containing the version
+    :param version_variable_name: name of the variable containing the version
+    :return: version string
     """
-    version_module_path = '{}/{}.py'.format(package_name.replace('-', '_'), version_module_name)
+    version_module_path = f'{package_name.replace("-", "_")}/{version_module_name}.py'
     version_module_vars = runpy.run_path(version_module_path)
     return version_module_vars[version_variable_name]
 
 
 def find_packages(root_directory: str = '.') -> t.List[str]:
-    """Find packages to pack."""
+    """Find packages to pack.
+
+    :param root_directory: directory to start searching from
+    :return: list of packages
+    """
     exclude = ['test', 'test.*'] if ('bdist_wheel' in sys.argv or 'bdist' in sys.argv) else []
     packages_list = setuptools.find_packages(root_directory, exclude=exclude)
     return packages_list
 
 
 def parse_requirements(
         requirements_path: str = 'requirements.txt') -> t.List[str]:
     """Read contents of requirements.txt file and return data from its relevant lines.
 
     Only non-empty and non-comment lines are relevant.
+
+    :param requirements_path: path to the requirements file if custom one is used
+    :return: list of requirements
     """
     requirements = []
-    with HERE.joinpath(requirements_path).open() as reqs_file:
-        for requirement in [line.strip() for line in reqs_file.read().splitlines()]:
+    with HERE.joinpath(requirements_path).open(encoding='utf-8') as requirements_file:
+        for requirement in [line.strip() for line in requirements_file.read().splitlines()]:
             if not requirement or requirement.startswith('#'):
                 continue
             requirements.append(requirement)
     return requirements
 
 
 def partition_version_classifiers(
         classifiers: t.Sequence[str], version_prefix: str = 'Programming Language :: Python :: ',
-        only_suffix: str = ' :: Only') -> t.Tuple[t.List[str], t.List[str]]:
-    """Find version number classifiers in given list and partition them into 2 groups."""
-    versions_min, versions_only = [], []
+        only_suffix: str = ' :: Only'
+        ) -> t.Tuple[t.List[t.Tuple[int, ...]], t.List[t.Tuple[int, ...]]]:
+    """Find version number classifiers in given list and partition them into 2 groups.
+
+    The 2 groups being:
+    1. minimum versions, any version at least as high this is compatible
+    2. only versions, this specific version is compatible, but nothing is said about other versions
+
+    :param classifiers: sequence of trove classifiers to be analysed
+    :param version_prefix: prefix that identifies a version classifier
+    :param only_suffix: prefix that identifies an "only version" classifier
+    :return: parsed and partitioned version tuples
+    """
+    versions_min: t.List[t.Tuple[int, ...]] = []
+    versions_only: t.List[t.Tuple[int, ...]] = []
     for classifier in classifiers:
         version = classifier.replace(version_prefix, '')
         versions = versions_min
         if version.endswith(only_suffix):
             version = version.replace(only_suffix, '')
             versions = versions_only
         try:
-            versions.append(tuple([int(_) for _ in version.split('.')]))
+            versions.append(tuple(int(_) for _ in version.split('.')))
         except ValueError:
             pass
     return versions_min, versions_only
 
 
 def find_required_python_version(
         classifiers: t.Sequence[str], version_prefix: str = 'Programming Language :: Python :: ',
         only_suffix: str = ' :: Only') -> t.Optional[str]:
-    """Determine the minimum required Python version."""
+    """Determine the minimum required Python version.
+
+    :param classifiers: sequence of trove classifiers to be analysed
+    :param version_prefix: prefix that identifies a version classifier
+    :param only_suffix: prefix that identifies an "only version" classifier
+    :return: minimum required Python version string, if any
+    """
     versions_min, versions_only = partition_version_classifiers(
         classifiers, version_prefix, only_suffix)
     if len(versions_only) > 1:
-        raise ValueError(
-            'more than one "{}" version encountered in {}'.format(only_suffix, versions_only))
+        raise ValueError(f'more than one "{only_suffix}" version encountered in {versions_only}')
     only_version = None
     if len(versions_only) == 1:
         only_version = versions_only[0]
         for version in versions_min:
             if version[:len(only_version)] != only_version:
-                raise ValueError(
-                    'the "{}" version {} is inconsistent with version {}'
-                    .format(only_suffix, only_version, version))
+                raise ValueError(f'the "{only_suffix}" version {only_version}'
+                                 f' is inconsistent with version {version}')
     min_supported_version = None
     for version in versions_min:
         if min_supported_version is None or \
                 (len(version) >= len(min_supported_version) and version < min_supported_version):
             min_supported_version = version
     if min_supported_version is None:
         if only_version is not None:
             return '.'.join([str(_) for _ in only_version])
     else:
         return '>=' + '.'.join([str(_) for _ in min_supported_version])
     return None
 
 
-def resolve_relative_rst_links(text: str, base_link: str):
-    """Resolve all relative links in a given RST document.
+def parse_rst(text: str) -> docutils.nodes.document:
+    """Parse text assuming it's an RST markup."""
+    parser = docutils.parsers.rst.Parser()
+    components = (docutils.parsers.rst.Parser,)
+    settings = docutils.frontend.OptionParser(components=components).get_default_values()
+    document = docutils.utils.new_document('<rst-doc>', settings=settings)
+    parser.parse(text, document)
+    return document
+
+
+class RelativeRefFinder(docutils.nodes.NodeVisitor):
+    """Find all relative references in a given docutils document that point to existing files."""
+
+    def __init__(self, root_dir: pathlib.Path, *args, **kwargs):
+        """Initialize the RelativeRefFinder object."""
+        super().__init__(*args, **kwargs)
+        self.root_dir = root_dir
+        self.references: t.List[docutils.nodes.reference] = []
+
+    def visit_reference(self, node: docutils.nodes.reference) -> None:
+        """Call for "reference" nodes."""
+        assert isinstance(node, docutils.nodes.TextElement), type(node)
+        _LOG.debug('RelativeRefFinder: examining reference %s', node)
+        if len(node.children) != 1 or 'refuri' not in node.attributes \
+                or node.attributes['refuri'].startswith(('http://', 'https://')):
+            return
+        # _LOG.debug('  RelativeRefFinder: reference passed initial check')
+        path = pathlib.Path(node.attributes['refuri'])
+        if path.is_absolute():
+            return
+        try:
+            resolved_path = path.resolve(strict=True)
+        except FileNotFoundError:
+            return
+        try:
+            resolved_path.relative_to(self.root_dir)
+        except ValueError:
+            return
+        if not path.is_file():
+            return
+        _LOG.debug('RelativeRefFinder: reference points to existing file')
+        self.references.append(node)
+
+    def unknown_visit(self, node: docutils.nodes.Node) -> None:
+        """Call for unknown node types."""
+        return
+
 
-    All links of form `link`_ become `link <base_link/link>`_.
-    """
-    import docutils.nodes
-    import docutils.parsers.rst
-    import docutils.utils
-
-    def parse_rst(text: str) -> docutils.nodes.document:
-        """Parse text assuming it's an RST markup."""
-        parser = docutils.parsers.rst.Parser()
-        components = (docutils.parsers.rst.Parser,)
-        settings = docutils.frontend.OptionParser(components=components).get_default_values()
-        document = docutils.utils.new_document('<rst-doc>', settings=settings)
-        parser.parse(text, document)
-        return document
-
-    class SimpleRefCounter(docutils.nodes.NodeVisitor):
-        """Find all simple references in a given docutils document."""
-
-        def __init__(self, *args, **kwargs):
-            """Initialize the SimpleRefCounter object."""
-            super().__init__(*args, **kwargs)
-            self.references = []
-
-        def visit_reference(self, node: docutils.nodes.reference) -> None:
-            """Call for "reference" nodes."""
-            if len(node.children) != 1 or not isinstance(node.children[0], docutils.nodes.Text) \
-                    or not all(_ in node.attributes for _ in ('name', 'refuri')):
-                return
-            path = pathlib.Path(node.attributes['refuri'])
-            try:
-                if path.is_absolute():
-                    return
-                resolved_path = path.resolve()
-            except FileNotFoundError:  # in resolve(), prior to Python 3.6
-                return
-            except OSError:  # in is_absolute() and resolve(), on URLs in Windows
-                return
-            try:
-                resolved_path.relative_to(HERE)
-            except ValueError:
-                return
-            if not path.is_file():
-                return
-            assert node.attributes['name'] == node.children[0].astext()
-            self.references.append(node)
+def resolve_relative_rst_links(text: str, base_link: str) -> str:
+    """Resolve all relative links in a given string representing an RST document.
 
-        def unknown_visit(self, node: docutils.nodes.Node) -> None:
-            """Call for unknown node types."""
-            return
+    Links are resolved only if they point to files existing in the project's working directory.
 
+    All links of form `link`_ become `link <absolute_link>`_.
+
+    And all link of the form :target: link become :target: absolute_link.
+
+    Where absolute_link is made by concatenating base_link to link with no separator added
+    in between. So in most cases base_link should and with a slash.
+    """
     document = parse_rst(text)
-    visitor = SimpleRefCounter(document)
-    document.walk(visitor)
-    for target in visitor.references:
-        name = target.attributes['name']
-        uri = target.attributes['refuri']
-        new_link = '`{} <{}{}>`_'.format(name, base_link, uri)
-        if name == uri:
-            text = text.replace('`<{}>`_'.format(uri), new_link)
+    finder = RelativeRefFinder(HERE, document)
+    document.walk(finder)
+    for target in finder.references:
+        _LOG.info('resolve_relative_rst_links: resolving reference %s', target)
+        assert isinstance(target, docutils.nodes.TextElement), type(target)
+        refuri = target.attributes['refuri']
+        if 'name' in target.attributes:
+            name = target.attributes['name']
+            if name == refuri:
+                old_link = f'`<{refuri}>`_'
+            else:
+                old_link = f'`{name} <{refuri}>`_'
+            new_link = f'`{name} <{base_link}{refuri}>`_'
         else:
-            text = text.replace('`{} <{}>`_'.format(name, uri), new_link)
+            old_link = f' :target: {refuri}'
+            new_link = f' :target: {base_link}{refuri}'
+        text = text.replace(old_link, new_link)
+        _LOG.info('resolve_relative_rst_links: replaced "%s" with "%s"', old_link, new_link)
     return text
 
 
 class Package:
     """Default metadata and behaviour for a Python package setup script."""
 
-    root_directory = '.'  # type: str
+    root_directory: str = '.'
     """Root directory of the source code of the package, relative to the setup.py file location."""
 
-    name = None  # type: str
+    name: str
+    """Package name."""
 
-    version = None  # type: str
-    """"If None, it will be obtained from "package_name._version.VERSION" variable."""
+    version: str
+    """Package version as string.
 
-    description = None  # type: str
+    If None, it will be obtained from "package_name._version.VERSION" variable.
+    """
 
-    long_description = None  # type: str
-    """If None, it will be generated from readme."""
+    description: str
+    """One line of text that shortly describes the package."""
 
-    long_description_content_type = None  # type: str
-    """If None, it will be set accodring to readme file extension.
+    long_description: str
+    """Full description of the package, can be arbitrarily long.
 
-    For this field to be automatically set, also long_description field has to be None.
+    If not set, it will be generated from readme.
     """
 
-    url = 'https://github.com/mbdevpl'  # type: str
-    download_url = None  # type: str
-    author = 'Mateusz Bysiek'  # type: str
-    author_email = 'mateusz.bysiek@gmail.com'  # type: str
-    # maintainer = None  # type: str
-    # maintainer_email = None  # type: str
-    license_str = 'Apache License 2.0'  # type: str
+    long_description_content_type: str
+    """Content type of the long description.
+
+    Usually one of 'text/x-rst', 'text/markdown' or 'text/plain'.
+
+    If not set, it will be set according to readme file extension.
+    For this field to be automatically set, also long_description field cannot be set.
+    """
 
-    classifiers = []  # type: t.List[str]
-    """List of valid project classifiers: https://pypi.org/pypi?:action=list_classifiers"""
+    url: str = DEFAULT_URL
+    download_url: str = ''
+    author: str = DEFAULT_AUTHOR
+    author_email: str = DEFAULT_AUTHOR_EMAIL
+    maintainer: str
+    maintainer_email: str
+    license_str: str = DEFAULT_LICENSE_STR
 
-    keywords = []  # type: t.List[str]
+    classifiers: t.List[str] = []
+    """List of trove classifiers for the package.
 
-    packages = None  # type: t.List[str]
-    """If None, determined with help of setuptools."""
+    List of valid classifiers: https://pypi.org/pypi?:action=list_classifiers
+    """
+
+    keywords: t.List[str] = []
+
+    packages: t.List[str]
+    """List of Python packages to be included in the distributed file.
+
+    Usually it's just one package per distributed file, but any number is supported.
+
+    If not set, determined with help of setuptools.
+    """
 
-    package_data = {}
-    exclude_package_data = {}
+    package_data: t.Dict[str, t.List[str]] = {}
+    exclude_package_data: t.Dict[str, t.List[str]] = {}
 
-    install_requires = None  # type: t.List[str]
+    install_requires: t.Optional[t.List[str]] = None
     """If None, determined using requirements.txt."""
 
-    extras_require = {}  # type: t.Mapping[str, t.List[str]]
+    extras_require: t.Mapping[str, t.List[str]] = {}
     """A dictionary containing entries of type 'some_feature': ['requirement1', 'requirement2']."""
 
-    python_requires = None  # type: str
+    python_requires: t.Optional[str] = None
     """If None, determined from provided classifiers."""
 
-    entry_points = {}  # type: t.Mapping[str, t.List[str]]
+    entry_points: t.Mapping[str, t.List[str]] = {}
     """A dictionary used to enable automatic creation of console scripts, gui scripts and plugins.
 
     Example entry:
     'console_scripts': ['script_name = package.subpackage:function']
     """
 
-    test_suite = 'test'  # type: str
+    test_suite: str = 'test'
 
     @classmethod
     def try_fields(cls, *names) -> t.Optional[t.Any]:
         """Return first existing of given class field names."""
         for name in names:
             if hasattr(cls, name):
                 return getattr(cls, name)
         raise AttributeError((cls, names))
 
     @classmethod
-    def parse_readme(cls, readme_path: str = 'README.rst',
+    def parse_readme(cls, readme_filename: str = 'README.rst',
                      encoding: str = 'utf-8') -> t.Tuple[str, str]:
         """Parse readme and resolve relative links in it if it is feasible.
 
         Links are resolved if readme is in rst format and the package is hosted on GitHub.
         """
-        readme_path = pathlib.Path(readme_path)
-        with HERE.joinpath(readme_path).open(encoding=encoding) as readme_file:
-            long_description = readme_file.read()  # type: str
+        readme_path = HERE.joinpath(readme_filename)
+        with readme_path.open(encoding=encoding) as readme_file:
+            long_description: str = readme_file.read()
 
         if readme_path.suffix.lower() == '.rst' and cls.url.startswith('https://github.com/'):
-            base_url = '{}/blob/v{}/'.format(cls.url, cls.version)
+            base_url = f'{cls.url}/blob/v{cls.version}/'
             long_description = resolve_relative_rst_links(long_description, base_url)
 
         long_description_content_type = {'.rst': 'text/x-rst', '.md': 'text/markdown'}.get(
             readme_path.suffix.lower(), 'text/plain')
         long_description_content_type += '; charset=UTF-8'
 
         return long_description, long_description_content_type
 
     @classmethod
     def prepare(cls) -> None:
         """Fill in possibly missing package metadata."""
-        if cls.version is None:
+        if not hasattr(cls, 'version'):
             cls.version = find_version(cls.name)
-        if cls.long_description is None:
+        if not hasattr(cls, 'long_description'):
             cls.long_description, cls.long_description_content_type = cls.parse_readme()
-        if cls.packages is None:
+        if not hasattr(cls, 'maintainer'):
+            cls.maintainer = cls.author
+        if not hasattr(cls, 'maintainer_email'):
+            cls.maintainer_email = cls.author_email
+        if not hasattr(cls, 'packages'):
             cls.packages = find_packages(cls.root_directory)
         if cls.install_requires is None:
             cls.install_requires = parse_requirements()
         if cls.python_requires is None:
             cls.python_requires = find_required_python_version(cls.classifiers)
 
     @classmethod
@@ -303,16 +380,16 @@
         cls.prepare()
         setuptools.setup(
             name=cls.name, version=cls.version, description=cls.description,
             long_description=cls.long_description,
             long_description_content_type=cls.long_description_content_type,
             url=cls.url, download_url=cls.download_url,
             author=cls.author, author_email=cls.author_email,
-            maintainer=cls.try_fields('maintainer', 'author'),
-            maintainer_email=cls.try_fields('maintainer_email', 'author_email'),
+            maintainer=cls.maintainer,
+            maintainer_email=cls.maintainer_email,
             license=cls.license_str, classifiers=cls.classifiers, keywords=cls.keywords,
             packages=cls.packages, package_dir={'': cls.root_directory},
             include_package_data=True,
             package_data=cls.package_data, exclude_package_data=cls.exclude_package_data,
             install_requires=cls.install_requires, extras_require=cls.extras_require,
             python_requires=cls.python_requires,
             entry_points=cls.entry_points, test_suite=cls.test_suite)
```

### Comparing `ingit-0.4.8/test/test_action_progress.py` & `ingit-0.4.9/test/test_action_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for git operation progress reporting."""
 
-import collections
+import collections.abc
 import logging
 import sys
 import unittest
 
 from ingit.action_progress import ActionProgress, _KNOWN_OPERATIONS_STRINGS as op_codes
 
 
@@ -12,29 +12,29 @@
 
     """Clumsy converter that allows logging instances to be used as a file-like object.
 
     Given a logging_function, will convert write(text) calls to logging_function(text) calls.
     For example: StreamToLog(logging.warning) will redirect all writes to logging.warning().
     """
 
-    def __init__(self, logging_function: collections.Callable):
+    def __init__(self, logging_function: collections.abc.Callable):
         """Construct StreamToLog."""
         assert callable(logging_function)
 
         self.logging_function = logging_function
 
     def write(self, message):
         """Redirect the write to the logging function."""
         while message.endswith('\r') or message.endswith('\n'):
             message = message[:-1]
         self.logging_function(message)
 
     def flush(self):
         """Flush can be a no-op."""
-        pass
+        # pass
 
 
 class ActionProgressTests(unittest.TestCase):
 
     """Unit tests for ActionProgress."""
 
     def test_construct(self):
```

### Comparing `ingit-0.4.8/test/test_git_commands.py` & `ingit-0.4.9/test/test_git_commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,174 +19,170 @@
 TEST_RUNTIME_CONFIG_PATH = pathlib.Path(HERE, 'examples', 'runtime_config', 'example_initial.json')
 # TEST_RUNTIME_CONFIG = file_to_json(TEST_RUNTIME_CONFIG_PATH)
 
 TEST_REPOS_CONFIG_PATH = pathlib.Path(HERE, 'examples', 'repos_config', 'example_initial.json')
 # TEST_REPOS_CONFIG = file_to_json(TEST_REPOS_CONFIG_PATH)
 
 PROJECT_NAMES = ('argunparse', 'transpyle', 'typed-astunparse')
+PROJECT_NAME = PROJECT_NAMES[0]
 
 _LOG = logging.getLogger(__name__)
 
 
 def call_main(*args, answer='y'):
     with unittest.mock.patch.object(readchar, 'readchar', return_value=answer):
         main(['--config', str(TEST_RUNTIME_CONFIG_PATH), '--repos', str(TEST_REPOS_CONFIG_PATH)]
              + list(args))
 
 
 class Tests(unittest.TestCase):
 
     def setUp(self):
         assert 'INGIT_TEST_REPOS_PATH' not in os.environ
-        self._tmpdir = tempfile.TemporaryDirectory()
+        self._tmpdir = tempfile.TemporaryDirectory()  # pylint: disable=consider-using-with
         os.environ['INGIT_TEST_REPOS_PATH'] = self._tmpdir.name
         _LOG.warning('set INGIT_TEST_REPOS_PATH="%s"', self._tmpdir.name)
         self.repos_path = pathlib.Path(self._tmpdir.name)
 
     def tearDown(self):
         if platform.system() != 'Windows':
             self._tmpdir.cleanup()
         del os.environ['INGIT_TEST_REPOS_PATH']
 
     def test_clone(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
             self.assertFalse(repo_path.is_dir())
-            call_main('-p', 'name == "{}"'.format(project_name), 'clone')
+            call_main('-p', f'name == "{project_name}"', 'clone')
             self.assertTrue(repo_path.is_dir())
             self.assertTrue(repo_path.joinpath('.git').is_dir())
 
     def test_clone_no(self):
-        project_name = 'argunparse'
-        repo_path = pathlib.Path(self.repos_path, project_name)
-        call_main('-p', 'name == "{}"'.format(project_name), 'clone', answer='n')
+        repo_path = pathlib.Path(self.repos_path, PROJECT_NAME)
+        call_main('-p', f'name == "{PROJECT_NAME}"', 'clone', answer='n')
         self.assertFalse(repo_path.is_dir())
 
     def test_clone_to_repo_dir(self):
-        project_name = 'argunparse'
-        repo_path = pathlib.Path(self.repos_path, project_name)
-        call_main('-p', 'name == "{}"'.format(project_name), 'clone')
+        repo_path = pathlib.Path(self.repos_path, PROJECT_NAME)
+        call_main('-p', f'name == "{PROJECT_NAME}"', 'clone')
         self.assertTrue(repo_path.is_dir())
         self.assertTrue(repo_path.joinpath('.git').is_dir())
-        call_main('-r', '^{}$'.format(project_name), 'clone')
+        call_main('-r', f'^{PROJECT_NAME}$', 'clone')
 
     def test_clone_to_nonrepo_dir(self):
-        project_name = 'argunparse'
-        repo_path = pathlib.Path(self.repos_path, project_name)
+        repo_path = pathlib.Path(self.repos_path, PROJECT_NAME)
         repo_path.mkdir()
         with self.assertRaises(ValueError):
-            call_main('-p', 'name == "{}"'.format(project_name), 'clone')
+            call_main('-p', f'name == "{PROJECT_NAME}"', 'clone')
         self.assertTrue(repo_path.is_dir())
 
     # def test_clone_with_multiple_remotes(self):
 
     def test_init(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
             self.assertFalse(repo_path.is_dir())
-            call_main('-p', 'name == "{}"'.format(project_name), 'init')
+            call_main('-p', f'name == "{project_name}"', 'init')
             self.assertTrue(repo_path.is_dir())
             self.assertTrue(repo_path.joinpath('.git').is_dir())
 
     def test_init_in_repo_dir(self):
-        project_name = 'argunparse'
-        repo_path = pathlib.Path(self.repos_path, project_name)
-        call_main('-p', 'name == "{}"'.format(project_name), 'clone')
+        repo_path = pathlib.Path(self.repos_path, PROJECT_NAME)
+        call_main('-p', f'name == "{PROJECT_NAME}"', 'clone')
         self.assertTrue(repo_path.is_dir())
         self.assertTrue(repo_path.joinpath('.git').is_dir())
-        call_main('-p', 'name == "{}"'.format(project_name), 'init')
+        call_main('-p', f'name == "{PROJECT_NAME}"', 'init')
 
     def test_init_no(self):
-        project_name = 'argunparse'
-        call_main('-p', 'name == "{}"'.format(project_name), 'init')
-        project_name = 'ingit'
+        project_name = PROJECT_NAMES[0]
+        call_main('-p', f'name == "{project_name}"', 'init')
+        project_name = PROJECT_NAMES[1]
         repo_path = pathlib.Path(self.repos_path, project_name)
-        call_main('-p', 'name == "{}"'.format(project_name), 'init', answer='n')
+        call_main('-p', f'name == "{project_name}"', 'init', answer='n')
         self.assertFalse(repo_path.is_dir())
 
     def test_fetch(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
-            call_main('-p', 'name == "{}"'.format(project_name), 'init')
-            call_main('-p', 'name == "{}"'.format(project_name), 'fetch')
+            call_main('-p', f'name == "{project_name}"', 'init')
+            call_main('-p', f'name == "{project_name}"', 'fetch')
             self.assertTrue(repo_path.is_dir())
             self.assertTrue(repo_path.joinpath('.git').is_dir())
 
     def test_fetch_all(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
-            call_main('-p', 'name == "{}"'.format(project_name), 'init')
-            call_main('-p', 'name == "{}"'.format(project_name), 'fetch', '--all')
+            call_main('-p', f'name == "{project_name}"', 'init')
+            call_main('-p', f'name == "{project_name}"', 'fetch', '--all')
             self.assertTrue(repo_path.is_dir())
             self.assertTrue(repo_path.joinpath('.git').is_dir())
 
     def test_checkout_detached(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
             self.assertFalse(repo_path.is_dir())
-            call_main('-p', 'name == "{}"'.format(project_name), 'clone')
+            call_main('-p', f'name == "{project_name}"', 'clone')
             self.assertTrue(repo_path.is_dir())
             repo = git.Repo(str(repo_path))
             head_ref = repo.head.commit.hexsha
             initial_commit = collections.deque(repo.iter_commits(), maxlen=1).pop()
             initial_ref = initial_commit.hexsha
             repo.git.checkout(initial_ref)
-            call_main('-p', 'name == "{}"'.format(project_name), 'checkout', answer='n')
+            call_main('-p', f'name == "{project_name}"', 'checkout', answer='n')
             self.assertEqual(repo.head.commit.hexsha, initial_ref)
-            call_main('-p', 'name == "{}"'.format(project_name), 'checkout', answer='1')
+            call_main('-p', f'name == "{project_name}"', 'checkout', answer='1')
             self.assertEqual(repo.head.commit.hexsha, head_ref)
 
     def test_checkout(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
-            call_main('-p', 'name == "{}"'.format(project_name), 'clone')
+            call_main('-p', f'name == "{project_name}"', 'clone')
             self.assertTrue(repo_path.is_dir())
             self.assertTrue(repo_path.joinpath('.git').is_dir())
-            call_main('-p', 'name == "{}"'.format(project_name), 'checkout', answer='n')
+            call_main('-p', f'name == "{project_name}"', 'checkout', answer='n')
 
     @unittest.expectedFailure
     def test_checkout_conflicting(self):
         """Checkout remote branch for which there already exists local branch having a different
         tracking branch, which will result in detached head.
         """
         # project_name = 'argunparse'
         self.fail()
 
     @unittest.expectedFailure
     def test_merge(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
-            call_main('-p', 'name == "{}"'.format(project_name), 'init')
+            call_main('-p', f'name == "{project_name}"', 'init')
             self.assertTrue(repo_path.is_dir())
-            call_main('-p', 'name == "{}"'.format(project_name), 'merge')
+            call_main('-p', f'name == "{project_name}"', 'merge')
 
     def test_push(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
-            call_main('-p', 'name == "{}"'.format(project_name), 'init')
+            call_main('-p', f'name == "{project_name}"', 'init')
             self.assertTrue(repo_path.is_dir())
-            call_main('-p', 'name == "{}"'.format(project_name), 'push')
+            call_main('-p', f'name == "{project_name}"', 'push')
             self.assertTrue(repo_path.is_dir())
 
     def test_gc(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
-            call_main('-p', 'name == "{}"'.format(project_name), 'clone')
+            call_main('-p', f'name == "{project_name}"', 'clone')
             self.assertTrue(repo_path.is_dir())
             self.assertTrue(repo_path.joinpath('.git').is_dir())
-            call_main('-p', 'name == "{}"'.format(project_name), 'gc')
+            call_main('-p', f'name == "{project_name}"', 'gc')
 
     def test_status(self):
         for project_name in PROJECT_NAMES:
             repo_path = pathlib.Path(self.repos_path, project_name)
-            call_main('-p', 'name == "{}"'.format(project_name), 'clone')
+            call_main('-p', f'name == "{project_name}"', 'clone')
             self.assertTrue(repo_path.is_dir())
             self.assertTrue(repo_path.joinpath('.git').is_dir())
-            call_main('-p', 'name == "{}"'.format(project_name), 'status', answer='n')
+            call_main('-p', f'name == "{project_name}"', 'status', answer='n')
 
     def test_skip_nonexisting(self):
         for command in ('fetch', 'checkout', 'merge', 'push', 'gc', 'status'):
-            project_name = 'argunparse'
-            repo_path = pathlib.Path(self.repos_path, project_name)
+            repo_path = pathlib.Path(self.repos_path, PROJECT_NAME)
             self.assertFalse(repo_path.is_dir())
-            call_main('-p', 'name == "{}"'.format(project_name), command)
+            call_main('-p', f'name == "{PROJECT_NAME}"', command)
             self.assertFalse(repo_path.is_dir())
```

### Comparing `ingit-0.4.8/test/test_json_config.py` & `ingit-0.4.9/test/test_json_config.py`

 * *Files identical despite different names*

### Comparing `ingit-0.4.8/test/test_main.py` & `ingit-0.4.9/test/test_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def test_script(self):
         with self.assertRaises(SystemExit):
             run_module('ingit')
         run_module('ingit', run_name='not_main')
 
     def test_help(self):
-        with open(os.devnull, 'a') as devnull:
+        with open(os.devnull, 'a', encoding='utf-8') as devnull:
             for flags in (['-h'], ['--help']):
                 with self.assertRaises(SystemExit):
                     with contextlib.redirect_stdout(devnull):
                         main(flags)
 
     def test_filtered_register(self):
         with self.assertRaises(SystemExit):
```

### Comparing `ingit-0.4.8/test/test_project.py` & `ingit-0.4.9/test/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 _REMOTE = str(_HERE.parent.joinpath('.git'))
 
 _LOG = logging.getLogger(__name__)
 
 
 class Tests(GitRepoTests):
+    # pylint: disable = too-many-public-methods
 
     def test_example(self):
         project = Project('example', ['tag1', 'tag2'], self.repo_path, {})
         self.assertEqual(project.name, 'example')
         self.assertSetEqual(project.tags, {'tag1', 'tag2'})
 
     def test_clone(self):
@@ -87,15 +88,15 @@
     # def test_checkout(self):
     #    pass
 
     def test_checkout_case_sensitive_no(self):
         self.git_init()
         self.git_commit_new_file()
         for i in range(0, 88):
-            self.repo.git.branch('branch_{:02}'.format(i))
+            self.repo.git.branch(f'branch_{i:02}')
         project = Project('example', [], self.repo_path, {})
         project.link_repo()
         with unittest.mock.patch.object(readchar, 'readchar', return_value='n'):
             project.checkout()
 
         def readchar_once():
             readchar_once.called_count += 1
@@ -110,15 +111,15 @@
 
     def test_checkout_too_many_branches(self):
         self.git_init()
         self.git_commit_new_file()
         project = Project('example', [], self.repo_path, {})
         project.link_repo()
         for i in range(0, 88):
-            self.repo.git.branch('branch_{:02}'.format(i))
+            self.repo.git.branch(f'branch_{i:02}')
             project.repo.refresh()
             with unittest.mock.patch.object(readchar, 'readchar', return_value='n'):
                 with open(os.devnull, 'a') as devnull:
                     with contextlib.redirect_stdout(devnull):
                         project.checkout()
         self.repo.git.branch('devel')
         project.repo.refresh()
```

### Comparing `ingit-0.4.8/test/test_repo_data.py` & `ingit-0.4.9/test/test_repo_data.py`

 * *Files identical despite different names*

### Comparing `ingit-0.4.8/test/test_runtime.py` & `ingit-0.4.9/test/test_runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         runtime_config_path = pathlib.Path(HERE, 'examples', 'runtime_config',
                                            'example_initial.json')
         shutil.copy(str(runtime_config_path), str(self.runtime_config_path))
         repos_config_path = pathlib.Path(HERE, 'examples', 'repos_config', 'example_paths.json')
         shutil.copy(str(repos_config_path), str(self.repos_config_path))
 
         for hostname, path in [
-                ('example_machine{}'.format(i), pathlib.Path('/example_path_{}'.format(i)))
+                (f'example_machine{i}', pathlib.Path(f'/example_path_{i}'))
                 for i in range(1, 4)]:
             runtime = Runtime(self.runtime_config_path, self.repos_config_path, hostname=hostname)
             runtime.filter_projects(lambda name, *_: name == 'example1')
             self.assertEqual(len(runtime.filtered_projects), 1)
             project = runtime.filtered_projects[0]
             self.assertEqual(project.path, path)
```

### Comparing `ingit-0.4.8/test/test_runtime_interface.py` & `ingit-0.4.9/test/test_runtime_interface.py`

 * *Files identical despite different names*

### Comparing `ingit-0.4.8/test/test_setup.py` & `ingit-0.4.9/test/test_setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,35 +8,32 @@
 import subprocess
 import sys
 import tempfile
 import types
 import typing as t
 import unittest
 
-__updated__ = '2019-06-04'
+__version__ = '2022.08.15'
 
 
-def run_program(*args, glob: bool = False):
+def run_program(*args, glob: bool = False) -> None:
     """Run subprocess with given args. Use path globbing for each arg that contains an asterisk."""
     if glob:
         cwd = pathlib.Path.cwd()
         args = tuple(itertools.chain.from_iterable(
             list(str(_.relative_to(cwd)) for _ in cwd.glob(arg)) if '*' in arg else [arg]
             for arg in args))
-    process = subprocess.Popen(args)
-    process.wait()
-    if process.returncode != 0:
-        raise AssertionError('execution of {} returned {}'.format(args, process.returncode))
-    return process
+    try:
+        subprocess.run(args, check=True)
+    except subprocess.CalledProcessError as err:
+        raise AssertionError(f'execution of {args} failed') from err
 
 
-def run_pip(*args, **kwargs):
-    python_exec_name = pathlib.Path(sys.executable).name
-    pip_exec_name = python_exec_name.replace('python', 'pip')
-    run_program(pip_exec_name, *args, **kwargs)
+def run_pip(*args, **kwargs) -> None:
+    run_program(sys.executable, '-m', 'pip', *args, **kwargs)
 
 
 def run_module(name: str, *args, run_name: str = '__main__') -> None:
     backup_sys_argv = sys.argv
     sys.argv = [name + '.py'] + list(args)
     runpy.run_module(name, run_name=run_name)
     sys.argv = backup_sys_argv
@@ -55,18 +52,14 @@
 CLASSIFIERS_LICENSES = (
     'License :: OSI Approved :: Python License (CNRI Python License)',
     'License :: OSI Approved :: Python Software Foundation License',
     'License :: Other/Proprietary License',
     'License :: Public Domain')
 
 CLASSIFIERS_PYTHON_VERSIONS = tuple("""Programming Language :: Python
-Programming Language :: Python :: 2
-Programming Language :: Python :: 2.2
-Programming Language :: Python :: 2.7
-Programming Language :: Python :: 2 :: Only
 Programming Language :: Python :: 3
 Programming Language :: Python :: 3.0
 Programming Language :: Python :: 3.5
 Programming Language :: Python :: 3 :: Only""".splitlines())
 
 CLASSIFIERS_PYTHON_IMPLEMENTATIONS = tuple("""Programming Language :: Python :: Implementation
 Programming Language :: Python :: Implementation :: CPython
@@ -135,28 +128,27 @@
         parse_requirements = import_module_member('setup_boilerplate', 'parse_requirements')
         results = parse_requirements()
         self.assertIsInstance(results, list)
         self.assertTrue(all(isinstance(result, str) for result in results), msg=results)
 
     def test_requirements_empty(self):
         parse_requirements = import_module_member('setup_boilerplate', 'parse_requirements')
-        reqs_file = tempfile.NamedTemporaryFile('w', delete=False)
-        reqs_file.close()
+        with tempfile.NamedTemporaryFile('w', delete=False) as reqs_file:
+            pass
         results = parse_requirements(reqs_file.name)
         self.assertIsInstance(results, list)
         self.assertEqual(len(results), 0)
         os.remove(reqs_file.name)
 
     def test_requirements_comments(self):
         parse_requirements = import_module_member('setup_boilerplate', 'parse_requirements')
         reqs = ['# comment', 'numpy', '', '# another comment', 'scipy', '', '# one more comment']
-        reqs_file = tempfile.NamedTemporaryFile('w', delete=False)
-        for req in reqs:
-            print(req, file=reqs_file)
-        reqs_file.close()
+        with tempfile.NamedTemporaryFile('w', delete=False) as reqs_file:
+            for req in reqs:
+                print(req, file=reqs_file)
         results = parse_requirements(reqs_file.name)
         self.assertIsInstance(results, list)
         self.assertGreater(len(results), 0)
         self.assertLess(len(results), len(reqs))
         os.remove(reqs_file.name)
 
     def test_python_versions(self):
@@ -214,15 +206,14 @@
              'Programming Language :: Python :: 3.0']]
         for classifiers in classifier_variants:
             with self.assertRaises(ValueError):
                 find_required_python_version(classifiers)
 
 
 class PackageTests(unittest.TestCase):
-
     """Test methods of Package class."""
 
     def test_try_fields(self):
         package = import_module_member('setup_boilerplate', 'Package')
 
         class Package(package):  # pylint: disable=too-few-public-methods
             name = 'package name'
@@ -249,27 +240,27 @@
         os.remove(temp_file.name)
         self.assertIsInstance(result, str)
         self.assertIsInstance(content_type, str)
 
         prefix = 'https://github.com/example/blob/v1.2.3.4/'
         for name, link, done in LINK_EXAMPLES:
             name = '' if name is None else name + ' '
-            text = 'Please see `{}<{}>`_ for details.'.format(name, link)
+            text = f'Please see `{name}<{link}>`_ for details.'
             with tempfile.NamedTemporaryFile('w', suffix='.rst', delete=False) as temp_file:
                 temp_file.write(text)
             result, content_type = Package.parse_readme(temp_file.name)
             os.remove(temp_file.name)
             self.assertIsInstance(result, str)
             self.assertIsInstance(content_type, str)
             if not done:
                 self.assertEqual(result, text)
                 continue
             if name == '':
                 name = link + ' '
-            self.assertIn('`{}<{}{}>`_'.format(name, prefix, link), result)
+            self.assertIn(f'`{name}<{prefix}{link}>`_', result)
 
     def test_prepare(self):
         package = import_module_member('setup_boilerplate', 'Package')
 
         version_ = '1.2.3.4.5.6.7'
         long_description_ = 'long package description'
 
@@ -284,29 +275,28 @@
 
         self.assertEqual(Package.version, version_)
         self.assertEqual(Package.long_description, long_description_)
         Package.prepare()
         self.assertEqual(Package.version, version_)
         self.assertEqual(Package.long_description, long_description_)
 
-        Package.long_description = None
-        Package.packages = None
-        Package.install_requires = None
-        Package.python_requires = None
+        del Package.long_description
+        del Package.packages
+        del Package.install_requires
+        del Package.python_requires
         Package.prepare()
 
-        Package.version = None
+        del Package.version
         with self.assertRaises(FileNotFoundError):
             Package.prepare()
 
 
 @unittest.skipUnless(os.environ.get('TEST_PACKAGING') or os.environ.get('CI'),
                      'skipping packaging tests for actual package')
 class IntergrationTests(unittest.TestCase):
-
     """Test if the boilerplate can actually create a valid package."""
 
     pkg_name = get_package_folder_name()
 
     def test_build_binary(self):
         run_module('setup', 'bdist')
         self.assertTrue(os.path.isdir('dist'))
@@ -316,34 +306,40 @@
         self.assertTrue(os.path.isdir('dist'))
 
     def test_build_source(self):
         run_module('setup', 'sdist', '--formats=gztar,zip')
         self.assertTrue(os.path.isdir('dist'))
 
     def test_install_code(self):
-        run_pip('install', '.')
-        run_pip('uninstall', '-y', self.pkg_name)
+        with tempfile.TemporaryDirectory() as temporary_folder:
+            run_pip('install', '--prefix', temporary_folder, '.')
+        self.assertFalse(pathlib.Path(temporary_folder).exists())
 
     def test_install_source_tar(self):
         find_version = import_module_member('setup_boilerplate', 'find_version')
         version = find_version(self.pkg_name)
-        run_pip('install', 'dist/*-{}.tar.gz'.format(version), glob=True)
-        run_pip('uninstall', '-y', self.pkg_name)
+        with tempfile.TemporaryDirectory() as temporary_folder:
+            run_pip(
+                'install', '--prefix', temporary_folder, f'dist/*-{version}.tar.gz', glob=True)
+        self.assertFalse(pathlib.Path(temporary_folder).exists())
 
     def test_install_source_zip(self):
         find_version = import_module_member('setup_boilerplate', 'find_version')
         version = find_version(self.pkg_name)
-        run_pip('install', 'dist/*-{}.zip'.format(version), glob=True)
-        run_pip('uninstall', '-y', self.pkg_name)
+        with tempfile.TemporaryDirectory() as temporary_folder:
+            run_pip('install', '--prefix', temporary_folder, f'dist/*-{version}.zip', glob=True)
+        self.assertFalse(pathlib.Path(temporary_folder).exists())
 
     def test_install_wheel(self):
         find_version = import_module_member('setup_boilerplate', 'find_version')
         version = find_version(self.pkg_name)
-        run_pip('install', 'dist/*-{}-*.whl'.format(version), glob=True)
-        run_pip('uninstall', '-y', self.pkg_name)
+        with tempfile.TemporaryDirectory() as temporary_folder:
+            run_pip(
+                'install', '--prefix', temporary_folder, f'dist/*-{version}-*.whl', glob=True)
+        self.assertFalse(pathlib.Path(temporary_folder).exists())
 
     def test_pip_error(self):
         with self.assertRaises(AssertionError):
             run_pip('wrong_pip_command')
 
     def test_setup_do_nothing_or_error(self):
         run_module('setup', 'wrong_setup_command', run_name='__not_main__')
```

### Comparing `ingit-0.4.8/test/test_with_git_repo.py` & `ingit-0.4.9/test/test_with_git_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import tempfile
 import unittest
 
 import git
 
 _LOG = logging.getLogger(__name__)
 
-__updated__ = '2018-04-18'
+__version__ = '2022.02.01'
 
 
 class GitRepoTests(unittest.TestCase):
 
     """Provide several utility propertied and methods named repo_* and git_*."""
 
     repo = None  # type: git.Repo
     repo_path = None  # type: pathlib.Path
 
     def setUp(self):
-        self._tmpdir = tempfile.TemporaryDirectory()
+        self._tmpdir = tempfile.TemporaryDirectory()  # pylint: disable=consider-using-with
         self.repo_path = pathlib.Path(self._tmpdir.name)
         self.assertTrue(self.repo_path.is_dir())
         self.repo = None
         self._repo_files = []
 
     def tearDown(self):
         for path in self._repo_files:
@@ -61,30 +61,30 @@
 
     def git_commit_new_file(self) -> pathlib.Path:
         """Create a new file and commit it."""
         with tempfile.NamedTemporaryFile('w', dir=str(self.repo_path), delete=False) as repo_file:
             repo_file.write('spam spam lovely spam\n')
             path = pathlib.Path(repo_file.name)
         self.repo.index.add([path.name])
-        self.repo.index.commit('created file {}'.format(path))
+        self.repo.index.commit(f'created file {path}')
         _LOG.debug('commited file %s as %s', path, self.repo_head_hexsha)
         self._repo_files.append(path)
         return path
 
     def git_modify_file(self, path: pathlib.Path, add: bool = False, commit: bool = False) -> None:
         """Modify an existing file."""
         self.assertIsInstance(self.repo, git.Repo)
         self.assertIsInstance(path, pathlib.Path)
         self.assertTrue(path.is_file())
         with path.open('a') as repo_file:
             repo_file.write('spam eggs ham\n')
         if add or commit:
             self.repo.index.add([path.name])
         if commit:
-            self.repo.index.commit('modified file {}'.format(path))
+            self.repo.index.commit(f'modified file {path}')
 
 
 class GitRepoSelfTests(GitRepoTests):
 
     def test_typical(self):
         self.git_init()
         pth = self.git_commit_new_file()
```

