# Comparing `tmp/sphinx-versioned-docs-1.0.tar.gz` & `tmp/sphinx-versioned-docs-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-versioned-docs-1.0.tar", last modified: Wed May  3 13:26:56 2023, max compression
+gzip compressed data, was "sphinx-versioned-docs-1.1.tar", last modified: Fri May 19 09:00:55 2023, max compression
```

## Comparing `sphinx-versioned-docs-1.0.tar` & `sphinx-versioned-docs-1.1.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.634432 sphinx-versioned-docs-1.0/
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.574432 sphinx-versioned-docs-1.0/.github/
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.604432 sphinx-versioned-docs-1.0/.github/workflows/
--rw-r--r--   0 devansh   (1000) devansh   (1000)     1042 2023-05-03 12:31:35.000000 sphinx-versioned-docs-1.0/.github/workflows/CI-themes.yml
--rw-r--r--   0 devansh   (1000) devansh   (1000)     2168 2023-05-03 12:38:09.000000 sphinx-versioned-docs-1.0/.github/workflows/main.yml
--rw-r--r--   0 devansh   (1000) devansh   (1000)      888 2023-05-03 05:13:32.000000 sphinx-versioned-docs-1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 devansh   (1000) devansh   (1000)      647 2023-05-01 07:49:35.000000 sphinx-versioned-docs-1.0/.gitignore
--rw-r--r--   0 devansh   (1000) devansh   (1000)      381 2023-05-03 05:13:32.000000 sphinx-versioned-docs-1.0/.readthedocs.yaml
--rw-r--r--   0 devansh   (1000) devansh   (1000)     1075 2023-05-01 06:12:37.000000 sphinx-versioned-docs-1.0/LICENSE
--rw-r--r--   0 devansh   (1000) devansh   (1000)     4281 2023-05-03 13:26:56.634432 sphinx-versioned-docs-1.0/PKG-INFO
--rw-r--r--   0 devansh   (1000) devansh   (1000)     3344 2023-05-03 13:26:14.000000 sphinx-versioned-docs-1.0/README.rst
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.614432 sphinx-versioned-docs-1.0/docs/
--rw-r--r--   0 devansh   (1000) devansh   (1000)      580 2023-05-01 06:12:37.000000 sphinx-versioned-docs-1.0/docs/Makefile
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.614432 sphinx-versioned-docs-1.0/docs/_static/
--rw-r--r--   0 devansh   (1000) devansh   (1000)     9433 2023-05-01 06:12:37.000000 sphinx-versioned-docs-1.0/docs/_static/Favicon_logo_Smile.png
--rw-r--r--   0 devansh   (1000) devansh   (1000)      599 2023-05-03 13:26:14.000000 sphinx-versioned-docs-1.0/docs/api.rst
--rw-r--r--   0 devansh   (1000) devansh   (1000)       46 2023-05-03 05:45:18.000000 sphinx-versioned-docs-1.0/docs/changelog.rst
--rw-r--r--   0 devansh   (1000) devansh   (1000)     7601 2023-05-03 05:45:18.000000 sphinx-versioned-docs-1.0/docs/conf.py
--rw-r--r--   0 devansh   (1000) devansh   (1000)     1001 2023-05-03 13:26:14.000000 sphinx-versioned-docs-1.0/docs/contributing.rst
--rw-r--r--   0 devansh   (1000) devansh   (1000)      507 2023-05-03 13:26:14.000000 sphinx-versioned-docs-1.0/docs/index.rst
--rw-r--r--   0 devansh   (1000) devansh   (1000)      504 2023-05-03 13:26:14.000000 sphinx-versioned-docs-1.0/docs/install.rst
--rw-r--r--   0 devansh   (1000) devansh   (1000)      370 2023-05-03 13:26:14.000000 sphinx-versioned-docs-1.0/docs/themes.rst
--rw-r--r--   0 devansh   (1000) devansh   (1000)     1697 2023-05-03 13:26:14.000000 sphinx-versioned-docs-1.0/docs/tutorial.rst
--rw-r--r--   0 devansh   (1000) devansh   (1000)     1432 2023-05-02 18:55:05.000000 sphinx-versioned-docs-1.0/pyproject.toml
--rw-r--r--   0 devansh   (1000) devansh   (1000)       96 2023-05-03 05:13:32.000000 sphinx-versioned-docs-1.0/requirements.txt
--rw-r--r--   0 devansh   (1000) devansh   (1000)     1546 2023-05-03 13:26:56.634432 sphinx-versioned-docs-1.0/setup.cfg
--rwxr-xr-x   0 devansh   (1000) devansh   (1000)      127 2023-05-01 07:49:35.000000 sphinx-versioned-docs-1.0/setup.py
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.614432 sphinx-versioned-docs-1.0/sphinx_versioned/
--rw-r--r--   0 devansh   (1000) devansh   (1000)       50 2023-05-03 05:45:18.000000 sphinx-versioned-docs-1.0/sphinx_versioned/__init__.py
--rwxr-xr-x   0 devansh   (1000) devansh   (1000)     7297 2023-05-03 10:15:38.000000 sphinx-versioned-docs-1.0/sphinx_versioned/__main__.py
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.614432 sphinx-versioned-docs-1.0/sphinx_versioned/_static/
--rw-r--r--   0 devansh   (1000) devansh   (1000)      315 2023-05-03 09:10:38.000000 sphinx-versioned-docs-1.0/sphinx_versioned/_static/_rtd_versions.js
--rw-r--r--   0 devansh   (1000) devansh   (1000)     4153 2023-05-03 06:48:24.000000 sphinx-versioned-docs-1.0/sphinx_versioned/_static/badge_only.css
--rw-r--r--   0 devansh   (1000) devansh   (1000)      710 2023-05-02 18:55:05.000000 sphinx-versioned-docs-1.0/sphinx_versioned/_static/banner.css
--rw-r--r--   0 devansh   (1000) devansh   (1000)    98024 2023-05-03 06:48:24.000000 sphinx-versioned-docs-1.0/sphinx_versioned/_static/fontawesome-webfont.woff
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.614432 sphinx-versioned-docs-1.0/sphinx_versioned/_templates/
--rw-r--r--   0 devansh   (1000) devansh   (1000)     1369 2023-05-02 18:55:05.000000 sphinx-versioned-docs-1.0/sphinx_versioned/_templates/banner.html
--rw-r--r--   0 devansh   (1000) devansh   (1000)     2934 2023-05-03 06:48:24.000000 sphinx-versioned-docs-1.0/sphinx_versioned/_templates/versions.html
--rw-r--r--   0 devansh   (1000) devansh   (1000)      155 2023-05-03 13:26:56.000000 sphinx-versioned-docs-1.0/sphinx_versioned/_version.py
--rw-r--r--   0 devansh   (1000) devansh   (1000)     1624 2023-05-02 18:55:05.000000 sphinx-versioned-docs-1.0/sphinx_versioned/lib.py
--rw-r--r--   0 devansh   (1000) devansh   (1000)     6220 2023-05-03 10:15:38.000000 sphinx-versioned-docs-1.0/sphinx_versioned/sphinx_.py
--rw-r--r--   0 devansh   (1000) devansh   (1000)     2973 2023-05-03 09:10:46.000000 sphinx-versioned-docs-1.0/sphinx_versioned/versions.py
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.624432 sphinx-versioned-docs-1.0/sphinx_versioned_docs.egg-info/
--rw-r--r--   0 devansh   (1000) devansh   (1000)     4281 2023-05-03 13:26:56.000000 sphinx-versioned-docs-1.0/sphinx_versioned_docs.egg-info/PKG-INFO
--rw-r--r--   0 devansh   (1000) devansh   (1000)     1187 2023-05-03 13:26:56.000000 sphinx-versioned-docs-1.0/sphinx_versioned_docs.egg-info/SOURCES.txt
--rw-r--r--   0 devansh   (1000) devansh   (1000)        1 2023-05-03 13:26:56.000000 sphinx-versioned-docs-1.0/sphinx_versioned_docs.egg-info/dependency_links.txt
--rw-r--r--   0 devansh   (1000) devansh   (1000)       67 2023-05-03 13:26:56.000000 sphinx-versioned-docs-1.0/sphinx_versioned_docs.egg-info/entry_points.txt
--rw-r--r--   0 devansh   (1000) devansh   (1000)        1 2023-05-03 13:26:56.000000 sphinx-versioned-docs-1.0/sphinx_versioned_docs.egg-info/not-zip-safe
--rw-r--r--   0 devansh   (1000) devansh   (1000)      132 2023-05-03 13:26:56.000000 sphinx-versioned-docs-1.0/sphinx_versioned_docs.egg-info/requires.txt
--rw-r--r--   0 devansh   (1000) devansh   (1000)       17 2023-05-03 13:26:56.000000 sphinx-versioned-docs-1.0/sphinx_versioned_docs.egg-info/top_level.txt
-drwxr-xr-x   0 devansh   (1000) devansh   (1000)        0 2023-05-03 13:26:56.634432 sphinx-versioned-docs-1.0/tests/
--rw-r--r--   0 devansh   (1000) devansh   (1000)        0 2023-05-02 18:55:05.000000 sphinx-versioned-docs-1.0/tests/__init__.py
--rw-r--r--   0 devansh   (1000) devansh   (1000)       30 2023-05-02 18:55:05.000000 sphinx-versioned-docs-1.0/tests/conftest.py
--rw-r--r--   0 devansh   (1000) devansh   (1000)      587 2023-05-03 10:15:38.000000 sphinx-versioned-docs-1.0/tests/prepare_tox_build_docs.py
--rw-r--r--   0 devansh   (1000) devansh   (1000)     2140 2023-05-03 10:15:38.000000 sphinx-versioned-docs-1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.160697 sphinx-versioned-docs-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.152697 sphinx-versioned-docs-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.152697 sphinx-versioned-docs-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/.github/workflows/CI-themes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/.github/workflows/check-changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-19 09:00:55.160697 sphinx-versioned-docs-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.156697 sphinx-versioned-docs-1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.156697 sphinx-versioned-docs-1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/_static/Favicon_logo_Smile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/themes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-19 09:00:55.160697 sphinx-versioned-docs-1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.156697 sphinx-versioned-docs-1.1/sphinx_versioned/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7671 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.156697 sphinx-versioned-docs-1.1/sphinx_versioned/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/_static/_rtd_versions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/_static/badge_only.css
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/_static/banner.css
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/_static/fontawesome-webfont.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.156697 sphinx-versioned-docs-1.1/sphinx_versioned/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/_templates/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-19 09:00:54.000000 sphinx-versioned-docs-1.1/sphinx_versioned/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/sphinx_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/sphinx_versioned/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.156697 sphinx-versioned-docs-1.1/sphinx_versioned_docs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-19 09:00:54.000000 sphinx-versioned-docs-1.1/sphinx_versioned_docs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-19 09:00:55.000000 sphinx-versioned-docs-1.1/sphinx_versioned_docs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:00:54.000000 sphinx-versioned-docs-1.1/sphinx_versioned_docs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-19 09:00:54.000000 sphinx-versioned-docs-1.1/sphinx_versioned_docs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:00:54.000000 sphinx-versioned-docs-1.1/sphinx_versioned_docs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-19 09:00:54.000000 sphinx-versioned-docs-1.1/sphinx_versioned_docs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 09:00:54.000000 sphinx-versioned-docs-1.1/sphinx_versioned_docs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:55.156697 sphinx-versioned-docs-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/tests/prepare_tox_build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-19 09:00:37.000000 sphinx-versioned-docs-1.1/tox.ini
```

### Comparing `sphinx-versioned-docs-1.0/.github/workflows/CI-themes.yml` & `sphinx-versioned-docs-1.1/.github/workflows/CI-themes.yml`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/.github/workflows/main.yml` & `sphinx-versioned-docs-1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/.github/workflows/python-publish.yml` & `sphinx-versioned-docs-1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/.gitignore` & `sphinx-versioned-docs-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/LICENSE` & `sphinx-versioned-docs-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/README.rst` & `sphinx-versioned-docs-1.1/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 =====================
 sphinx-versioned-docs
 =====================
 
-|build| |CI themes| |docs| |codestyle|
+|versions| |license|
+
+|build| |CI themes| |docs| |status| |codestyle|
 
 Sphinx extension that allows building versioned docs for self-hosting.
 Supported on Linux and macOS.
 
 It works by producing docs for all(specified) branches in separate folders and injects a readthedocs-like version selector menu/badge.
 
 This project is a fork of `Smile-SA/sphinx-versions <https://github.com/Smile-SA/sphinx-versions>`_ with significant changes.
@@ -15,32 +17,43 @@
 
 How to use
 ==========
 
 .. code:: bash
 
     sphinx-versioned --help
-    sphinx-versioned build --help
 
 .. code::
 
-     Usage: sphinx-versioned build [OPTIONS]
+     Usage: sphinx-versioned [OPTIONS]
 
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ --chdir                            TEXT  Make this the current working directory before running. [default: None]             │
     │ --output      -O                   TEXT  Output directory [default: docs/_build]                                             │
     │ --git-root                         TEXT  Path to directory in the local repo. Default is CWD.                                │
     │ --local-conf                       TEXT  Path to conf.py for sphinx-versions to read config from. [default: docs/conf.py]    │
     │ --root-ref    -r                   TEXT  The branch/tag at the root of DESTINATION. Will also be in subdir. [default: main]  │
     │ --prebuild        --no-prebuild          Disables the pre-builds; halves the runtime [default: prebuild]                     │
     │ --branches    -b                   TEXT  Build docs for specific branches and tags [default: None]                           │
     │ --quite           --no-quite             No output from `sphinx` [default: quite]                                            │
     │ --help                                   Show this message and exit.                                                         │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
+.. |versions| image:: https://img.shields.io/pypi/pyversions/sphinx-versioned-docs.svg?logo=python&logoColor=FBE072
+    :target: https://pypi.org/project/sphinx-versioned-docs/
+    :alt: Python versions supported
+
+.. |status| image:: https://img.shields.io/pypi/status/sphinx-versioned-docs.svg
+    :target: https://pypi.org/project/sphinx-versioned-docs/
+    :alt: Package stability
+
+.. |license| image:: https://img.shields.io/pypi/l/sphinx-versioned-docs 
+    :target: https://pypi.org/project/sphinx-versioned-docs/
+    :alt: License
+
 .. |build| image:: https://github.com/devanshshukla99/sphinx-versioned-docs/actions/workflows/main.yml/badge.svg
     :alt: CI
 
 .. |codestyle| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |docs| image:: https://readthedocs.org/projects/sphinx-versioned-docs/badge/?version=latest
```

### Comparing `sphinx-versioned-docs-1.0/docs/Makefile` & `sphinx-versioned-docs-1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/docs/_static/Favicon_logo_Smile.png` & `sphinx-versioned-docs-1.1/docs/_static/Favicon_logo_Smile.png`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/docs/api.rst` & `sphinx-versioned-docs-1.1/docs/api.rst`

 * *Files 14% similar despite different names*

```diff
@@ -18,26 +18,25 @@
 .. automodule:: sphinx_versioned.sphinx_
     :members:
     :undoc-members:
     :show-inheritance:
 
 ----------
 
-Versions container
+versions container
 ------------------
 
 .. automodule:: sphinx_versioned.versions
     :members:
     :undoc-members:
     :show-inheritance:
 
 ----------
 
-Util
+util
 ----
 
 .. automodule:: sphinx_versioned.lib
     :members:
     :undoc-members:
     :show-inheritance:
 
-----------
```

### Comparing `sphinx-versioned-docs-1.0/docs/conf.py` & `sphinx-versioned-docs-1.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = []
+exclude_patterns = ["changes"]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
```

### Comparing `sphinx-versioned-docs-1.0/docs/contributing.rst` & `sphinx-versioned-docs-1.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/docs/tutorial.rst` & `sphinx-versioned-docs-1.1/docs/tutorial.rst`

 * *Files 8% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 Building versioned docs
 =======================
 
 By default, ``sphinx-versioned-docs`` will try to build all tags and branches present in the git repo, using the command:
 
 .. code-block:: bash
 
-    sphinx-versioned build
+    sphinx-versioned
 
 However, to build some particular branch(s) and tag(s), they can be specified in the ``--branches`` argument as:
 
 .. code-block:: bash
 
-    sphinx-versioned build --branches "main, docs"
+    sphinx-versioned --branches "main, docs"
 
 This command will build the ``main`` and ``docs`` branches.
 
 After the build has succeded, your docs should be available in `docs/_build/<branch>/index.html` with a "Versions" section in the sidebar.
 
 .. note::
```

### Comparing `sphinx-versioned-docs-1.0/pyproject.toml` & `sphinx-versioned-docs-1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 [tool.setuptools_scm]
 write_to = "sphinx_versioned/_version.py"
 
 [tool.black]
 line-length = 110
 
 [tool.towncrier]
-    package = "sphinx_versioned_docs"
+    package = "sphinx_versioned"
     filename = "CHANGELOG.rst"
-    directory = "changelog/"
+    directory = "docs/changes/"
     issue_format = "`#{issue} <https://github.com/devanshshukla99/sphinx-versioned-docs/pull/{issue}>`__"
     title_format = "{version} ({project_date})"
 
     [[tool.towncrier.type]]
         directory = "breaking"
         name = "Backwards Incompatible Changes"
         showcontent = true
```

### Comparing `sphinx-versioned-docs-1.0/setup.cfg` & `sphinx-versioned-docs-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned/__main__.py` & `sphinx-versioned-docs-1.1/sphinx_versioned/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import re
 import os
+import sys
 import typer
 import shutil
 import pathlib
 from sphinx import application
 from sphinx.config import Config as SphinxConfig
 from sphinx.cmd.build import build_main
 from sphinx.errors import SphinxError
 from sphinx_versioned.versions import GitVersions, BuiltVersions
 
 from loguru import logger as log
 
 from sphinx_versioned.lib import TempDir
 from sphinx_versioned.sphinx_ import EventHandlers
 
+logger_format = (
+    "| <level>{level: <8}</level> | <cyan>{name}</cyan>:<cyan>{line}</cyan> | - <level>{message}</level>"
+)
+log.remove()
+log.add(sys.stderr, format=logger_format)
 
 app = typer.Typer()
 
 
-@app.callback()
-def cli(
-    verbose: bool = typer.Option(
-        False, "--verbose", "-v", help="Debug logging. Specify more than once for more logging."
-    ),
-):
-    pass
-
-
 class ConfigInject(SphinxConfig):
     """Inject this extension info self.extensions. Append after user's extensions."""
 
     def __init__(self, *args):
         super(ConfigInject, self).__init__(*args)
         self.extensions.append("sphinx_versioned.sphinx_")
 
@@ -42,14 +39,18 @@
         self._handle_paths()
 
         self._versions_to_pre_build = []
         self._versions_to_build = []
         self._failed_build = []
         self._quite = "-Q" if self.quite else None
 
+        if self.list_branches:
+            self._get_all_versions()
+            return
+
         # selectively build branches / build all branches
         self._versions_to_pre_build = (
             self._select_specific_branches() if self.select_branches else self._get_all_versions()
         )
         self._pre_build_versions()
 
         # Adds our extension to the sphinx-config
@@ -180,15 +181,15 @@
                 log.error(f"build failed for {tag}")
                 exit(-1)
             finally:
                 # restore to active branch
                 self.versions.checkout(self._active_branch)
 
 
-@app.command("build")
+@app.command()
 def main(
     chdir: str = typer.Option(
         None, "--chdir", help="Make this the current working directory before running."
     ),
     output_dir: str = typer.Option("docs/_build", "--output", "-O", help="Output directory"),
     git_root: str = typer.Option(
         None, "--git-root", help="Path to directory in the local repo. Default is CWD.", show_default=False
@@ -202,15 +203,21 @@
         "--root-ref",
         help="The branch/tag at the root of DESTINATION. Will also be in subdir.",
     ),
     prebuild: bool = typer.Option(True, help="Disables the pre-builds; halves the runtime"),
     select_branches: str = typer.Option(
         None, "-b", "--branches", help="Build docs for specific branches and tags"
     ),
+    list_branches: bool = typer.Option(
+        False, "--list-branches", "-l", help="List all branches/tags detected via GitPython"
+    ),
     quite: bool = typer.Option(True, help="No output from `sphinx`"),
+    verbose: bool = typer.Option(
+        False, "--verbose", "-v", help="Debug logging. Specify more than once for more logging."
+    ),
 ) -> None:
     if select_branches:
         select_branches = re.split(",|\ ", select_branches)
     return VersionedDocs(locals())
 
 
 if __name__ == "__main__":
```

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned/_static/badge_only.css` & `sphinx-versioned-docs-1.1/sphinx_versioned/_static/badge_only.css`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned/_static/banner.css` & `sphinx-versioned-docs-1.1/sphinx_versioned/_static/banner.css`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned/_static/fontawesome-webfont.woff` & `sphinx-versioned-docs-1.1/sphinx_versioned/_static/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned/_templates/banner.html` & `sphinx-versioned-docs-1.1/sphinx_versioned/_templates/banner.html`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned/_templates/versions.html` & `sphinx-versioned-docs-1.1/sphinx_versioned/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned/lib.py` & `sphinx-versioned-docs-1.1/sphinx_versioned/lib.py`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned/sphinx_.py` & `sphinx-versioned-docs-1.1/sphinx_versioned/sphinx_.py`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned/versions.py` & `sphinx-versioned-docs-1.1/sphinx_versioned/versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Collect and sort version strings."""
 
 import os
-import pathlib
+
+os.environ["GIT_PYTHON_REFRESH"] = "quiet"
+
 import git
+import pathlib
 from loguru import logger as log
 
 
 class GitVersions(object):
     def __init__(self, git_root, build_directory) -> None:
         self.git_root = git_root
         self.build_directory = pathlib.Path(build_directory)
```

### Comparing `sphinx-versioned-docs-1.0/sphinx_versioned_docs.egg-info/SOURCES.txt` & `sphinx-versioned-docs-1.1/sphinx_versioned_docs.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 .gitignore
 .readthedocs.yaml
+CHANGELOG.rst
 LICENSE
 README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/CI-themes.yml
+.github/workflows/check-changelog.yml
 .github/workflows/main.yml
 .github/workflows/python-publish.yml
 docs/Makefile
 docs/api.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
```

### Comparing `sphinx-versioned-docs-1.0/tests/prepare_tox_build_docs.py` & `sphinx-versioned-docs-1.1/tests/prepare_tox_build_docs.py`

 * *Files identical despite different names*

### Comparing `sphinx-versioned-docs-1.0/tox.ini` & `sphinx-versioned-docs-1.1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 changedir = .tmp/{envname}
 description = build sphinx_rtd_theme with prebuild
 deps =
     sphinx_rtd_theme
 commands =
     - sphinx-quickstart docs -p test-sphinx -a devanshshukla99 -v v1.0 --makefile --no-sep -r v1.0 -l en -q
     python {toxinidir}/tests/prepare_tox_build_docs.py sphinx_rtd_theme
-    sphinx-versioned build --no-quite
+    sphinx-versioned --no-quite
 
 # test codestyle
 [testenv:codestyle]
 changedir =
 skip_install = true
 description = check code style
 deps = 
@@ -44,26 +44,26 @@
 # test themes
 [testenv:sphinx_rtd_theme]
 changedir = .tmp/{envname}
 description = test sphinx_rtd_theme with --no-prebuild and main branch
 commands =
     - sphinx-quickstart docs -p test-sphinx -a devanshshukla99 -v v1.0 --makefile --no-sep -r v1.0 -l en -q
     python {toxinidir}/tests/prepare_tox_build_docs.py sphinx_rtd_theme
-    sphinx-versioned build --no-quite --no-prebuild --branches main
+    sphinx-versioned --no-quite --no-prebuild --branches main
 
 [testenv:astropy_sphinx_theme]
 changedir = .tmp/{envname}
 description = test astropy_sphinx_theme with --no-prebuild and main branch
 deps =
     astropy_sphinx_theme
 commands =
     - sphinx-quickstart docs -p test-sphinx -a devanshshukla99 -v v1.0 --makefile --no-sep -r v1.0 -l en -q
     python {toxinidir}/tests/prepare_tox_build_docs.py bootstrap-astropy
-    sphinx-versioned build --no-quite --no-prebuild --branches main
+    sphinx-versioned --no-quite --no-prebuild --branches main
 
 [testenv:alabaster]
 changedir = .tmp/{envname}
 description = test alabaster with --no-prebuild and main branch
 commands =
     - sphinx-quickstart docs -p test-sphinx -a devanshshukla99 -v v1.0 --makefile --no-sep -r v1.0 -l en -q
     python {toxinidir}/tests/prepare_tox_build_docs.py alabaster
-    sphinx-versioned build --no-quite --no-prebuild --branches main
+    sphinx-versioned --no-quite --no-prebuild --branches main
```

