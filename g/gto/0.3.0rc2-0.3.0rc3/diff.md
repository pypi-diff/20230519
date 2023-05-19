# Comparing `tmp/gto-0.3.0rc2.tar.gz` & `tmp/gto-0.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gto-0.3.0rc2.tar", last modified: Thu Apr  6 16:35:45 2023, max compression
+gzip compressed data, was "gto-0.3.0rc3.tar", last modified: Fri May 19 15:51:14 2023, max compression
```

## Comparing `gto-0.3.0rc2.tar` & `gto-0.3.0rc3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:35:45.196151 gto-0.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-06 16:35:27.000000 gto-0.3.0rc2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:35:45.184150 gto-0.3.0rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:35:45.188151 gto-0.3.0rc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-06 16:35:27.000000 gto-0.3.0rc2/.github/ISSUE_TEMPLATE/epic-or-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:35:45.188151 gto-0.3.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-06 16:35:27.000000 gto-0.3.0rc2/.github/workflows/check-test-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-06 16:35:27.000000 gto-0.3.0rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-06 16:35:27.000000 gto-0.3.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-04-06 16:35:27.000000 gto-0.3.0rc2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-06 16:35:27.000000 gto-0.3.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-06 16:35:45.196151 gto-0.3.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-06 16:35:27.000000 gto-0.3.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:35:45.192151 gto-0.3.0rc2/gto/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-06 16:35:44.000000 gto-0.3.0rc2/gto/_gto_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29313 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/commit_message_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/ext_dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/ext_mlem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    20840 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-06 16:35:27.000000 gto-0.3.0rc2/gto/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:35:45.192151 gto-0.3.0rc2/gto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-06 16:35:45.000000 gto-0.3.0rc2/gto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-06 16:35:45.000000 gto-0.3.0rc2/gto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 16:35:45.000000 gto-0.3.0rc2/gto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-06 16:35:45.000000 gto-0.3.0rc2/gto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 16:35:45.000000 gto-0.3.0rc2/gto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-06 16:35:45.000000 gto-0.3.0rc2/gto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 16:35:45.000000 gto-0.3.0rc2/gto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-06 16:35:27.000000 gto-0.3.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-06 16:35:27.000000 gto-0.3.0rc2/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-06 16:35:45.196151 gto-0.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-06 16:35:27.000000 gto-0.3.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:35:45.196151 gto-0.3.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:35:45.196151 gto-0.3.0rc2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/resources/sample_remote_repo_expected_history_churn.json
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/resources/sample_remote_repo_expected_registry.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/skip_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    28593 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_showcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-06 16:35:27.000000 gto-0.3.0rc2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.533838 gto-0.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.521838 gto-0.3.0rc3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.525838 gto-0.3.0rc3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.github/ISSUE_TEMPLATE/epic-or-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.525838 gto-0.3.0rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.github/workflows/check-test-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-19 15:50:58.000000 gto-0.3.0rc3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-19 15:50:58.000000 gto-0.3.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-19 15:51:14.533838 gto-0.3.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-19 15:50:58.000000 gto-0.3.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.529838 gto-0.3.0rc3/gto/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto/_gto_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29313 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/commit_message_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/ext_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/ext_mlem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-19 15:50:58.000000 gto-0.3.0rc3/gto/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.529838 gto-0.3.0rc3/gto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 15:51:14.000000 gto-0.3.0rc3/gto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 15:50:58.000000 gto-0.3.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 15:50:58.000000 gto-0.3.0rc3/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-19 15:51:14.533838 gto-0.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-19 15:50:58.000000 gto-0.3.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.533838 gto-0.3.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:51:14.533838 gto-0.3.0rc3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/resources/sample_remote_repo_expected_history_churn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/resources/sample_remote_repo_expected_registry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/skip_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28593 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-19 15:50:58.000000 gto-0.3.0rc3/tests/utils.py
```

### Comparing `gto-0.3.0rc2/.github/ISSUE_TEMPLATE/epic-or-story.md` & `gto-0.3.0rc3/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/.github/workflows/check-test-release.yml` & `gto-0.3.0rc3/.github/workflows/check-test-release.yml`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/.gitignore` & `gto-0.3.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/.pre-commit-config.yaml` & `gto-0.3.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/.pylintrc` & `gto-0.3.0rc3/.pylintrc`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/LICENSE` & `gto-0.3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/PKG-INFO` & `gto-0.3.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.0rc2
+Version: 0.3.0rc3
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.0rc2/README.md` & `gto-0.3.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/api.py` & `gto-0.3.0rc3/gto/api.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/base.py` & `gto-0.3.0rc3/gto/base.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/cli.py` & `gto-0.3.0rc3/gto/cli.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/config.py` & `gto-0.3.0rc3/gto/config.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/constants.py` & `gto-0.3.0rc3/gto/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 
 
 def tag_to_name(value):
     return value.replace(SEPARATOR_IN_TAG, SEPARATOR_IN_NAME)
 
 
 dirname = "[a-z0-9-_./]+"  # improve?
-name = r"[a-z]([a-z0-9-/]*[a-z0-9])?"  # just like in DVC now + "/"
+name = r"[a-z0-9]([a-z0-9-/]*[a-z0-9])?"
 semver = r"(?P<major>0|[1-9]\d*)\.(?P<minor>0|[1-9]\d*)\.(?P<patch>0|[1-9]\d*)(?:-(?P<prerelease>(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+(?P<buildmetadata>[0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?"
 counter = "?P<counter>[0-9]+"
 name_re = re.compile(f"^{name}$")
-fullname = f"(?P<dirname>{dirname}{SEPARATOR_IN_NAME})?{name}"  # add test to check ":" is here only once?
+fullname = f"(?P<dirname>{dirname}{SEPARATOR_IN_NAME})?(?P<name>{name})"  # add test to check ":" is here only once?
 fullname_in_tag = name_to_tag(fullname)
 fullname_re = re.compile(f"^{fullname}$")
 fullname_in_tag_re = re.compile(f"^{fullname_in_tag}$")
 
 tag_re = re.compile(
     f"^(?P<artifact>{fullname_in_tag})(((#(?P<stage>{name})|@(?P<version>v{semver}))(?P<cancel>!?))|@((?P<deprecated>deprecated)|(?P<created>created)))(#({counter}))?$"
 )
@@ -77,15 +77,15 @@
 
 
 def assert_fullname_is_valid(value):
     if not check_string_is_valid(value, regex=fullname_re):
         # fix error message to be regex-specific
         raise ValidationError(
             f"Invalid value '{value}'. Only lowercase english letters, , '-', '/' are allowed."
-            "Value must be of len >= 2, must with a letter and end with a letter or a number."
+            "Value must be of len >= 2, must start with a letter and end with a letter or a number."
         )
 
 
 class Shortcut(BaseModel):
     name: str
     stage: Optional[str] = None
     version: Optional[str] = None
```

### Comparing `gto-0.3.0rc2/gto/exceptions.py` & `gto-0.3.0rc3/gto/exceptions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/ext.py` & `gto-0.3.0rc3/gto/ext.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/ext_dvc.py` & `gto-0.3.0rc3/gto/ext_dvc.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/ext_mlem.py` & `gto-0.3.0rc3/gto/ext_mlem.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/git_utils.py` & `gto-0.3.0rc3/gto/git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/index.py` & `gto-0.3.0rc3/gto/index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/log.py` & `gto-0.3.0rc3/gto/log.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/registry.py` & `gto-0.3.0rc3/gto/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,17 +473,17 @@
         event = self.check_ref(tag)
         if len(event) > 1:
             raise NotImplementedInGTO("Can't process a tag that caused multiple events")
         event = event[0]
         return event
 
     @staticmethod
-    def _echo_git_suggestion(tag):
+    def _echo_git_suggestion(tag, delete=False):
         echo("To push the changes upstream, run:")
-        echo(f"    git push origin {tag}")
+        echo(f"    git push{' --delete ' if delete else ' '}origin {tag}")
 
     def _delete_tags(self, tags, stdout, push: bool):
         tags = list(tags)
         for tag in tags:
             delete_tag(self.repo, tag)
             if stdout:
                 echo(f"Deleted git tag '{tag}'")
@@ -585,8 +585,8 @@
                 delete=delete,
             )
             if stdout:
                 echo(
                     f"Successfully {'deleted' if delete else 'pushed'} git tag {tag_name} on remote."
                 )
         elif stdout:
-            self._echo_git_suggestion(tag_name)
+            self._echo_git_suggestion(tag_name, delete=delete)
```

### Comparing `gto-0.3.0rc2/gto/tag.py` & `gto-0.3.0rc3/gto/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 def parse_name(name: str, raise_on_fail: bool = True):
 
     match = re.search(tag_re, name)
     if raise_on_fail and not match:
         raise InvalidTagName(name)
     if match:
-        parsed = {tag_to_name(NAME): match["artifact"]}
+        parsed = {NAME: tag_to_name(match["artifact"])}
         if match["deprecated"]:
             parsed[ACTION] = Action.DEPRECATE
         if match[VERSION]:
             parsed[VERSION] = match[VERSION]
             parsed[ACTION] = (
                 Action.DEREGISTER if match["cancel"] == "!" else Action.REGISTER
             )
```

### Comparing `gto-0.3.0rc2/gto/ui.py` & `gto-0.3.0rc3/gto/ui.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/utils.py` & `gto-0.3.0rc3/gto/utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto/versions.py` & `gto-0.3.0rc3/gto/versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/gto.egg-info/PKG-INFO` & `gto-0.3.0rc3/gto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.0rc2
+Version: 0.3.0rc3
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.0rc2/gto.egg-info/SOURCES.txt` & `gto-0.3.0rc3/gto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/setup.cfg` & `gto-0.3.0rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/setup.py` & `gto-0.3.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/conftest.py` & `gto-0.3.0rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/resources/__init__.py` & `gto-0.3.0rc3/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/resources/sample_remote_repo_expected_history_churn.json` & `gto-0.3.0rc3/tests/resources/sample_remote_repo_expected_history_churn.json`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/resources/sample_remote_repo_expected_registry.json` & `gto-0.3.0rc3/tests/resources/sample_remote_repo_expected_registry.json`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/skip_presets.py` & `gto-0.3.0rc3/tests/skip_presets.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/test_api.py` & `gto-0.3.0rc3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/test_cli.py` & `gto-0.3.0rc3/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,20 @@
     # TODO: make unsuccessful
     _check_successful_cmd(
         "check-ref",
         ["-r", path, "this-tag-does-not-exist"],
         "",
     )
     _check_successful_cmd(
+        "parse-tag",
+        ["dvclive/dsd=nn@v0.0.1"],
+        "dvclive/dsd:nn",
+        _check_output_contains,
+    )
+    _check_successful_cmd(
         "doctor",
         ["-r", path],
         None,
     )
 
 
 EXPECTED_DESCRIBE_OUTPUT_2 = """{
@@ -322,14 +328,22 @@
         ["-r", repo.working_dir, "a1"],
         "Created git tag 'a1@v0.0.1' that registers version\n"
         "To push the changes upstream, run:\n"
         "    git push origin a1@v0.0.1\n",
     )
 
     _check_successful_cmd(
+        "deprecate",
+        ["-r", repo.working_dir, "a1", "v0.0.1", "--delete"],
+        "Deleted git tag 'a1@v0.0.1'\n"
+        "To push the changes upstream, run:\n"
+        "    git push --delete origin a1@v0.0.1\n",
+    )
+
+    _check_successful_cmd(
         "register",
         ["-r", repo.working_dir, "a2", "--version", "v1.2.3"],
         "Created git tag 'a2@v1.2.3' that registers version\n"
         "To push the changes upstream, run:\n"
         "    git push origin a2@v1.2.3\n",
     )
```

### Comparing `gto-0.3.0rc2/tests/test_config.py` & `gto-0.3.0rc3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/test_constants.py` & `gto-0.3.0rc3/tests/test_constants.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,34 +6,34 @@
     fullname_re,
 )
 
 
 @pytest.mark.parametrize(
     "name",
     [
+        "1",
         "m",
         "nn",
         "m1",
+        "1nn",
         "model-prod",
         "model-prod-v1",
         "dvclive/model",
     ],
 )
 def test_check_name_is_valid(name):
     assert check_string_is_valid(name)
 
 
 @pytest.mark.parametrize(
     "name",
     [
         "",
-        "1",
         "m/",
         "/m",
-        "1nn",
         "###",
         "@@@",
         "a model",
         "a_model",
         "-model",
         "model-",
         "model@1",
```

### Comparing `gto-0.3.0rc2/tests/test_git_utils.py` & `gto-0.3.0rc3/tests/test_git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/test_index.py` & `gto-0.3.0rc3/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/test_registry.py` & `gto-0.3.0rc3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/test_showcase.py` & `gto-0.3.0rc3/tests/test_showcase.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/test_tag.py` & `gto-0.3.0rc3/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/test_versions.py` & `gto-0.3.0rc3/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.0rc2/tests/utils.py` & `gto-0.3.0rc3/tests/utils.py`

 * *Files identical despite different names*

