# Comparing `tmp/invenio-cli-1.0.8.tar.gz` & `tmp/invenio-cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-cli-1.0.8.tar", last modified: Thu Oct 13 09:30:56 2022, max compression
+gzip compressed data, was "dist/invenio-cli-1.0.9.tar", last modified: Fri Oct 21 16:02:27 2022, max compression
```

## Comparing `invenio-cli-1.0.8.tar` & `invenio-cli-1.0.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5101 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2525 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10043 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6991 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/cli/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4885 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/cli/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/cli/packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/cli/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5876 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     8650 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3374 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     6226 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     9122 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/services_health.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/steps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2401 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6619 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/helpers/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3572 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/helpers/cookiecutter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/helpers/docker_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/helpers/env.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/helpers/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/helpers/process.py
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/invenio_cli/helpers/rdm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5101 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/invenio_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      837 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/commands/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1727 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/commands/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     8006 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/commands/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11814 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/commands/test_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/commands/test_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/commands/test_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/tests/commands/testpkg/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/commands/testpkg/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 09:30:56.000000 invenio-cli-1.0.8/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/helpers/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/helpers/test_cookiecutter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/helpers/test_dockerhelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/helpers/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/helpers/test_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-10-13 09:30:52.000000 invenio-cli-1.0.8/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5252 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2525 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10043 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6991 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/assets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4885 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/packages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/services.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5876 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/assets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8650 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3374 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6226 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/packages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9122 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/services.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/services_health.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2401 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6619 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3572 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/cookiecutter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/docker_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/process.py
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/invenio_cli/helpers/rdm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5252 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/invenio_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-21 16:02:26.000000 invenio-cli-1.0.9/invenio_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      837 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1727 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8006 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11814 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/tests/commands/testpkg/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/commands/testpkg/package.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:02:27.000000 invenio-cli-1.0.9/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_cookiecutter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_dockerhelper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/helpers/test_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2022-10-21 16:02:21.000000 invenio-cli-1.0.9/tests/test_cli.py
```

### Comparing `invenio-cli-1.0.8/.editorconfig` & `invenio-cli-1.0.9/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/CHANGES.rst` & `invenio-cli-1.0.9/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio-Cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.0.8 (released 2022-10-13)
+
+- Fix issue when checking for services to be up
+  and running correctly.
+
 Version 1.0.7 (released 2022-10-10)
 
 - Fix compat issue with RDM versions < v10
 
 Version 1.0.6 (released 2022-10-10)
 
 - Bump default RDM version.
```

### Comparing `invenio-cli-1.0.8/CONTRIBUTING.rst` & `invenio-cli-1.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/LICENSE` & `invenio-cli-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/MANIFEST.in` & `invenio-cli-1.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/PKG-INFO` & `invenio-cli-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: "Invenio module to ease the creation and management of applications."
 Home-page: https://github.com/inveniosoftware/invenio-cli
 Author: CERN & Northwestern University
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019-2020 CERN.
@@ -108,14 +108,19 @@
         
             Invenio-Cli is free software; you can redistribute it and/or modify
             it under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.0.8 (released 2022-10-13)
+        
+        - Fix issue when checking for services to be up
+          and running correctly.
+        
         Version 1.0.7 (released 2022-10-10)
         
         - Fix compat issue with RDM versions < v10
         
         Version 1.0.6 (released 2022-10-10)
         
         - Bump default RDM version.
```

### Comparing `invenio-cli-1.0.8/README.rst` & `invenio-cli-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/docs/Makefile` & `invenio-cli-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/docs/conf.py` & `invenio-cli-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/docs/index.rst` & `invenio-cli-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/docs/make.bat` & `invenio-cli-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/cli/assets.py` & `invenio-cli-1.0.9/invenio_cli/cli/assets.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/cli/cli.py` & `invenio-cli-1.0.9/invenio_cli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/cli/containers.py` & `invenio-cli-1.0.9/invenio_cli/cli/containers.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/cli/install.py` & `invenio-cli-1.0.9/invenio_cli/cli/install.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/cli/packages.py` & `invenio-cli-1.0.9/invenio_cli/cli/packages.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/cli/services.py` & `invenio-cli-1.0.9/invenio_cli/cli/services.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/cli/utils.py` & `invenio-cli-1.0.9/invenio_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/__init__.py` & `invenio-cli-1.0.9/invenio_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/assets.py` & `invenio-cli-1.0.9/invenio_cli/commands/assets.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/commands.py` & `invenio-cli-1.0.9/invenio_cli/commands/commands.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/containers.py` & `invenio-cli-1.0.9/invenio_cli/commands/containers.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/install.py` & `invenio-cli-1.0.9/invenio_cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/local.py` & `invenio-cli-1.0.9/invenio_cli/commands/local.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/packages.py` & `invenio-cli-1.0.9/invenio_cli/commands/packages.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/requirements.py` & `invenio-cli-1.0.9/invenio_cli/commands/requirements.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/services.py` & `invenio-cli-1.0.9/invenio_cli/commands/services.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/services_health.py` & `invenio-cli-1.0.9/invenio_cli/commands/services_health.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,42 +110,47 @@
         """Wait for the given service to be up."""
         if service not in HEALTHCHECKS:
             raise RuntimeError(
                 f"{service} not recognized. Available services: {HEALTHCHECKS.keys()}"
             )
 
         exp_backoff_time = 2
-        try_ = 1
+        try_ = 0
         check = HEALTHCHECKS[service]
         check_func = check["func"]
         initial_delay = check.get("initial_delay", 0)
+        wait_initial_delay = initial_delay > 0
         ready = False
 
-        # some services might particularly slow to start up
-        if initial_delay > 0:
-            print_func(
-                f"{service} starting up, checking in {initial_delay}s...",
-            )
-            time.sleep(initial_delay)
-
         while not ready and try_ < max_retries:
             response = check_func(
                 filepath=filepath,
                 verbose=verbose,
                 project_shortname=project_shortname,
             )
             ready = response.status_code == 0
+
             if not ready:
-                print_func(
-                    f"{service} not ready at {try_} retries, waiting "
-                    + f"{exp_backoff_time}s...",
-                )
+                is_first_check = try_ == 0
+
+                # some services might be particularly slow to start up
+                if is_first_check and wait_initial_delay:
+                    print_func(
+                        f"{service} starting up, checking in {initial_delay}s...",
+                    )
+                    time.sleep(initial_delay)
+                else:
+                    print_func(
+                        f"{service} not ready at {try_+1} retries, waiting "
+                        + f"{exp_backoff_time}s...",
+                    )
+                    time.sleep(exp_backoff_time)
+                    exp_backoff_time *= 2
+
                 try_ += 1
-                time.sleep(exp_backoff_time)
-                exp_backoff_time *= 2
 
         return ready
 
 
 HEALTHCHECKS = {
     "search": {
         "func": ServicesHealthCommands.search_healthcheck,
```

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/steps.py` & `invenio-cli-1.0.9/invenio_cli/commands/steps.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/commands/upgrade.py` & `invenio-cli-1.0.9/invenio_cli/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/helpers/cli_config.py` & `invenio-cli-1.0.9/invenio_cli/helpers/cli_config.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/helpers/cookiecutter_wrapper.py` & `invenio-cli-1.0.9/invenio_cli/helpers/cookiecutter_wrapper.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/helpers/env.py` & `invenio-cli-1.0.9/invenio_cli/helpers/env.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/helpers/filesystem.py` & `invenio-cli-1.0.9/invenio_cli/helpers/filesystem.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/helpers/process.py` & `invenio-cli-1.0.9/invenio_cli/helpers/process.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli/helpers/rdm.py` & `invenio-cli-1.0.9/invenio_cli/helpers/rdm.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/invenio_cli.egg-info/PKG-INFO` & `invenio-cli-1.0.9/invenio_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: "Invenio module to ease the creation and management of applications."
 Home-page: https://github.com/inveniosoftware/invenio-cli
 Author: CERN & Northwestern University
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019-2020 CERN.
@@ -108,14 +108,19 @@
         
             Invenio-Cli is free software; you can redistribute it and/or modify
             it under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.0.8 (released 2022-10-13)
+        
+        - Fix issue when checking for services to be up
+          and running correctly.
+        
         Version 1.0.7 (released 2022-10-10)
         
         - Fix compat issue with RDM versions < v10
         
         Version 1.0.6 (released 2022-10-10)
         
         - Bump default RDM version.
```

### Comparing `invenio-cli-1.0.8/invenio_cli.egg-info/SOURCES.txt` & `invenio-cli-1.0.9/invenio_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/run-tests.sh` & `invenio-cli-1.0.9/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/setup.cfg` & `invenio-cli-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/commands/conftest.py` & `invenio-cli-1.0.9/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/commands/test_commands.py` & `invenio-cli-1.0.9/tests/commands/test_commands.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/commands/test_containers.py` & `invenio-cli-1.0.9/tests/commands/test_containers.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/commands/test_local.py` & `invenio-cli-1.0.9/tests/commands/test_local.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/commands/test_requirements.py` & `invenio-cli-1.0.9/tests/commands/test_requirements.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/commands/test_steps.py` & `invenio-cli-1.0.9/tests/commands/test_steps.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/helpers/test_cli_config.py` & `invenio-cli-1.0.9/tests/helpers/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/helpers/test_cookiecutter_wrapper.py` & `invenio-cli-1.0.9/tests/helpers/test_cookiecutter_wrapper.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/helpers/test_dockerhelper.py` & `invenio-cli-1.0.9/tests/helpers/test_dockerhelper.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/helpers/test_env.py` & `invenio-cli-1.0.9/tests/helpers/test_env.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/helpers/test_filesystem.py` & `invenio-cli-1.0.9/tests/helpers/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.0.8/tests/test_cli.py` & `invenio-cli-1.0.9/tests/test_cli.py`

 * *Files identical despite different names*

