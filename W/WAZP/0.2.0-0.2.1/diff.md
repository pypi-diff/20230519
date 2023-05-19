# Comparing `tmp/WAZP-0.2.0.tar.gz` & `tmp/WAZP-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WAZP-0.2.0.tar", last modified: Mon Apr 17 17:55:26 2023, max compression
+gzip compressed data, was "WAZP-0.2.1.tar", last modified: Fri May 19 10:21:55 2023, max compression
```

## Comparing `WAZP-0.2.0.tar` & `WAZP-0.2.1.tar`

### file list

```diff
@@ -1,93 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 17:55:09.000000 WAZP-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.824925 WAZP-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.824925 WAZP-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-17 17:55:09.000000 WAZP-0.2.0/.github/workflows/docs_build_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-17 17:55:09.000000 WAZP-0.2.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-17 17:55:09.000000 WAZP-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-17 17:55:09.000000 WAZP-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-17 17:55:09.000000 WAZP-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-17 17:55:09.000000 WAZP-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-17 17:55:09.000000 WAZP-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-17 17:55:26.832925 WAZP-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-17 17:55:09.000000 WAZP-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.828925 WAZP-0.2.0/WAZP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-17 17:55:26.000000 WAZP-0.2.0/WAZP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 17:55:24.000000 WAZP-0.2.0/WAZP.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-17 17:55:09.000000 WAZP-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.828925 WAZP-0.2.0/sample_project/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 17:55:09.000000 WAZP-0.2.0/sample_project/input_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-17 17:55:09.000000 WAZP-0.2.0/sample_project/metadata_fields.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/sample_project/videos/
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_control.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_nectar1.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_nectar2.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-17 17:55:12.000000 WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_wateronly_s.metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:55:26.832925 WAZP-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_integration/test_smoke.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_unit/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-17 17:55:12.000000 WAZP-0.2.0/tests/test_unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-17 17:55:12.000000 WAZP-0.2.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/wazp/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/wazp/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/home.py
--rw-r--r--   0 runner    (1001) docker     (123)    25843 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    28552 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/callbacks/roi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:55:26.832925 WAZP-0.2.0/wazp/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/01_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/02_ROI.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/03_pose_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/04_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/pages/home.py
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-04-17 17:55:12.000000 WAZP-0.2.0/wazp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.126507 WAZP-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.102507 WAZP-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.110507 WAZP-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-19 10:21:39.000000 WAZP-0.2.1/.github/workflows/docs_build_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-19 10:21:39.000000 WAZP-0.2.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-19 10:21:39.000000 WAZP-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-19 10:21:39.000000 WAZP-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-05-19 10:21:39.000000 WAZP-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-19 10:21:39.000000 WAZP-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-19 10:21:39.000000 WAZP-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-19 10:21:55.126507 WAZP-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-19 10:21:39.000000 WAZP-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.110507 WAZP-0.2.1/WAZP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-19 10:21:52.000000 WAZP-0.2.1/WAZP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-19 10:21:55.000000 WAZP-0.2.1/WAZP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:21:52.000000 WAZP-0.2.1/WAZP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 10:21:52.000000 WAZP-0.2.1/WAZP.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-19 10:21:52.000000 WAZP-0.2.1/WAZP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 10:21:52.000000 WAZP-0.2.1/WAZP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-19 10:21:39.000000 WAZP-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.110507 WAZP-0.2.1/sample_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-19 10:21:39.000000 WAZP-0.2.1/sample_project/input_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-19 10:21:39.000000 WAZP-0.2.1/sample_project/metadata_fields.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.126507 WAZP-0.2.1/sample_project/videos/
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspE_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspE_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspE_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspE_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspG_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspG_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspG_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspG_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspH_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspH_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspH_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspH_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspI_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspI_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspI_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspI_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspJ_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspJ_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspJ_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspJ_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspK_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspK_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspK_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspK_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspL_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspL_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspL_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspL_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspM_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspM_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspM_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspM_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspN_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspN_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspN_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspN_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspO_nectar-open-close_control.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspO_nectar-open-close_nectar1.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspO_nectar-open-close_nectar2.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-19 10:21:41.000000 WAZP-0.2.1/sample_project/videos/jwaspO_nectar-open-close_wateronly_s.metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:21:55.126507 WAZP-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.126507 WAZP-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:41.000000 WAZP-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.126507 WAZP-0.2.1/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:41.000000 WAZP-0.2.1/tests/test_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-19 10:21:41.000000 WAZP-0.2.1/tests/test_integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-19 10:21:41.000000 WAZP-0.2.1/tests/test_integration/test_smoke.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.126507 WAZP-0.2.1/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:41.000000 WAZP-0.2.1/tests/test_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 10:21:41.000000 WAZP-0.2.1/tests/test_unit/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-19 10:21:41.000000 WAZP-0.2.1/tests/test_unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-19 10:21:41.000000 WAZP-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.126507 WAZP-0.2.1/wazp/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.126507 WAZP-0.2.1/wazp/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/callbacks/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/callbacks/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26744 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/callbacks/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29882 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/callbacks/roi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:21:55.126507 WAZP-0.2.1/wazp/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/pages/01_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/pages/02_ROI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/pages/03_pose_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/pages/04_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/pages/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-05-19 10:21:41.000000 WAZP-0.2.1/wazp/utils.py
```

### Comparing `WAZP-0.2.0/.github/workflows/docs_build_and_deploy.yml` & `WAZP-0.2.1/.github/workflows/docs_build_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/.github/workflows/test_and_deploy.yml` & `WAZP-0.2.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/.gitignore` & `WAZP-0.2.1/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *,cover
 .hypothesis/
 .pytest_cache/
+.test_helper_screenshots/
 
 # mypy
 .mypy_cache/
 
 # Translations
 *.mo
 *.pot
```

### Comparing `WAZP-0.2.0/CONTRIBUTING.md` & `WAZP-0.2.1/CONTRIBUTING.md`

 * *Files 15% similar despite different names*

```diff
@@ -41,41 +41,86 @@
 - Ask for a review from someone specific if you think they would be a particularly suited reviewer
 
 ## Development guidelines
 
 ### Formatting and pre-commit hooks
 
 Running `pre-commit install` will set up [pre-commit hooks](https://pre-commit.com/) to ensure a consistent formatting style. Currently, these are:
-* [isort](https://pycqa.github.io/isort/) for sorting import statements
-* [flake8](https://flake8.pycqa.org/en/latest/) for linting
+* [ruff](https://github.com/charliermarsh/ruff) does a number of jobs, including enforcing PEP8 and sorting imports
 * [black](https://black.readthedocs.io/en/stable/) for auto-formatting
 * [mypy](https://mypy.readthedocs.io/en/stable/index.html) as a static type checker
 
 These will prevent code from being committed if any of these hooks fail. To run them individually (from the root of the repository), you can use:
 ```sh
-isort .
-flake8
+ruff .
 black ./
 mypy -p wazp
 ```
 
 To run all the hooks before committing:
 
 ```sh
 pre-commit run  # for staged files
 pre-commit run -a  # for all files in the repository
 ```
 
 ### Testing
 
-We use [pytest](https://docs.pytest.org/en/latest/) for testing. Please try to ensure that all functions
-are tested, including both unit and integration tests.
+We use [pytest](https://docs.pytest.org/en/latest/) for testing, and our integration tests require Google chrome or chromium and a compatible `chromedriver`.
+Please try to ensure that all functions are tested, including both unit and integration tests.
 Write your test methods and classes in the `test` folder.
 
-Remember to test locally, before pushing, via running `pytest` in the root of the repository. This will run all tests and also report test coverage.
+#### Integration tests with chrome
+
+The integration tests start a server and browse with chrome(ium),
+so you will need to download and install Google chrome or chromium (if you don't already use one of them).
+You will then need to download a [compatible version of `chromedriver`](https://chromedriver.chromium.org/downloads).
+Depending on your OS you may also need to ***trust*** the executable.
+
+<details>
+<summary>Ubuntu</summary>
+
+Installing chromium and chromedriver is a one-liner (tested in Ubuntu 20.04 and 22.04).
+
+```sh
+sudo apt install chromium-chromedriver
+pytest # in the root of the repository
+```
+
+</details>
+
+<details>
+<summary>MacOS</summary>
+There is also a [homebrew cask](https://formulae.brew.sh/cask/chromedriver) for `chromedriver` so instead of going to the web and downloading you should be able to:
+
+```sh
+brew install chromedriver
+brew info chromedriver
+```
+And take note of the installation path.
+(It's probably something like `/opt/homebrew/Caskroom/chromedriver/<version>`).
+
+However you obtained `chomedriver`, you can trust the executable via the security settings and/or keychain GUI or just:
+
+```sh
+cd /place/where/your/chromedriver/is
+xattr -d com.apple.quarantine chromedriver
+```
+
+Once downloaded, make sure the `chromedriver` binary in your `PATH` and check that you can run the integration tests.
+
+```sh
+export PATH=$PATH:/place/where/your/chromedriver/is/chromedriver
+pytest # in the root of the repository
+```
+
+</details>
+
+
+It's a good idea to test locally before pushing. Pytest will run all tests and also report test coverage.
 
 ### Continuous integration
 All pushes and pull requests will be built by [GitHub actions](https://docs.github.com/en/actions). This will usually include linting, testing and deployment.
 
 A GitHub actions workflow (`.github/workflows/test_and_deploy.yml`) has been set up to run (on each commit/PR):
 * Linting checks (pre-commit).
 * Testing (only if linting checks pass)
```

### Comparing `WAZP-0.2.0/LICENSE` & `WAZP-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/PKG-INFO` & `WAZP-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WAZP
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wasp Animal-tracking Zoo project with Pose estimation
 Author-email: Sofia Miñano <s.minano@ucl.ac.uk>, Nikoloz Sirmpilatze <niko.sirbiladze@gmail.com>, Sam Cunliffe <s.cunliffe@ucl.ac.uk>, Adam Tyson <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/SainsburyWellcomeCentre/WAZP
 Project-URL: Bug tracker, https://github.com/SainsburyWellcomeCentre/WAZP/issues
 Project-URL: Documentation, https://SainsburyWellcomeCentre.github.io/WAZP
 Project-URL: Source code, https://github.com/SainsburyWellcomeCentre/WAZP
@@ -19,16 +19,17 @@
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause)
 ![CI](https://img.shields.io/github/actions/workflow/status/SainsburyWellcomeCentre/WAZP/test_and_deploy.yml?label=CI)
+[![codecov](https://codecov.io/gh/SainsburyWellcomeCentre/WAZP/branch/main/graph/badge.svg?token=DYQB8EHTJB)](https://codecov.io/gh/SainsburyWellcomeCentre/WAZP)
 [![docs](https://img.shields.io/website?down_color=red&down_message=down&label=docs&up_color=brightgreen&up_message=up&url=https%3A%2F%2Fsainsburywellcomecentre.github.io%2FWAZP%2F)](https://sainsburywellcomecentre.github.io/WAZP/)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 # WAZP 🐝
 **W**asp **A**nimal-tracking **Z**oo project with **P**ose estimation
 (name is subject to refinement)
```

### Comparing `WAZP-0.2.0/README.md` & `WAZP-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause)
 ![CI](https://img.shields.io/github/actions/workflow/status/SainsburyWellcomeCentre/WAZP/test_and_deploy.yml?label=CI)
+[![codecov](https://codecov.io/gh/SainsburyWellcomeCentre/WAZP/branch/main/graph/badge.svg?token=DYQB8EHTJB)](https://codecov.io/gh/SainsburyWellcomeCentre/WAZP)
 [![docs](https://img.shields.io/website?down_color=red&down_message=down&label=docs&up_color=brightgreen&up_message=up&url=https%3A%2F%2Fsainsburywellcomecentre.github.io%2FWAZP%2F)](https://sainsburywellcomecentre.github.io/WAZP/)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 # WAZP 🐝
 **W**asp **A**nimal-tracking **Z**oo project with **P**ose estimation
 (name is subject to refinement)
```

### Comparing `WAZP-0.2.0/WAZP.egg-info/PKG-INFO` & `WAZP-0.2.1/WAZP.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WAZP
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wasp Animal-tracking Zoo project with Pose estimation
 Author-email: Sofia Miñano <s.minano@ucl.ac.uk>, Nikoloz Sirmpilatze <niko.sirbiladze@gmail.com>, Sam Cunliffe <s.cunliffe@ucl.ac.uk>, Adam Tyson <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/SainsburyWellcomeCentre/WAZP
 Project-URL: Bug tracker, https://github.com/SainsburyWellcomeCentre/WAZP/issues
 Project-URL: Documentation, https://SainsburyWellcomeCentre.github.io/WAZP
 Project-URL: Source code, https://github.com/SainsburyWellcomeCentre/WAZP
@@ -19,16 +19,17 @@
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause)
 ![CI](https://img.shields.io/github/actions/workflow/status/SainsburyWellcomeCentre/WAZP/test_and_deploy.yml?label=CI)
+[![codecov](https://codecov.io/gh/SainsburyWellcomeCentre/WAZP/branch/main/graph/badge.svg?token=DYQB8EHTJB)](https://codecov.io/gh/SainsburyWellcomeCentre/WAZP)
 [![docs](https://img.shields.io/website?down_color=red&down_message=down&label=docs&up_color=brightgreen&up_message=up&url=https%3A%2F%2Fsainsburywellcomecentre.github.io%2FWAZP%2F)](https://sainsburywellcomecentre.github.io/WAZP/)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 # WAZP 🐝
 **W**asp **A**nimal-tracking **Z**oo project with **P**ose estimation
 (name is subject to refinement)
```

### Comparing `WAZP-0.2.0/WAZP.egg-info/SOURCES.txt` & `WAZP-0.2.1/WAZP.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.flake8
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
```

### Comparing `WAZP-0.2.0/pyproject.toml` & `WAZP-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -52,18 +52,17 @@
 dev = [
     "pytest",
     "pytest-cov",
     "coverage",
     "dash[testing]",
     "tox",
     "black",
-    "isort",
+    "ruff",
     "mypy",
     "pre-commit",
-    "flake8",
     "setuptools-scm",
     "types-PyYAML",
     "pandas-stubs",
     "types-Pillow",
 ]
 
 
@@ -104,30 +103,31 @@
     | build
     | dist
     | examples
   )/
 )
 '''
 
-[tool.isort]
-profile = "black"
-line_length = 79
+[tool.ruff]
+line-length = 79
+exclude = ["__init__.py","build",".eggs"]
+select = ["I", "E", "F"]
+fix = true
 
 [tool.setuptools_scm]
 
 [tool.check-manifest]
 ignore = [
     "*.yaml",
     "tox.ini",
     "tests/*",
     "tests/test_unit/*",
     "tests/test_integration/*",
     "docs/",
     "docs/source/",
-    ".flake8"
 ]
 
 [[tool.mypy.overrides]]
 module = [
   "dash.*",
   "dash_bootstrap_components.*",
   "h5py.*",
```

### Comparing `WAZP-0.2.0/sample_project/input_config.yaml` & `WAZP-0.2.1/sample_project/input_config.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/metadata_fields.yaml` & `WAZP-0.2.1/sample_project/metadata_fields.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspE_nectar-open-close_control.metadata.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   path: M484.23300516875133,565.133184774723L483.3063124386091,605.9076649009826L487.01308335917815,624.4415195038279L489.7931615496049,634.6351395353927L495.3533179304585,639.268603186104L532.4210271361491,639.268603186104L558.3684235801323,635.5618322655349L562.0751945007014,628.1482904243968L560.2218090404169,604.054279440698L557.4417308499901,570.6933411555766L557.4417308499901,563.2797993144385Z
 - drawn_on_frame: 38000
   line_color: '#1CA71C'
   name: control_box
   path: M756.6806678305767,278.34419881335197L761.314131481288,311.7051370984735L767.8009805922838,337.6525335424568L770.5810587827106,343.2126899233104L800.235226147263,337.6525335424568L832.6694717022423,336.7258408123146L834.5228571625267,322.8254498601806L826.1826225912464,286.68443338463237L825.2559298611042,267.22388605164485L826.1826225912464,275.5641206229252Z
 - drawn_on_frame: 38000
   line_color: '#FB0D0D'
-  name: water-only_box
+  name: water_only_box
   path: M1061.562576047381,566.5456378875958L1071.756196078946,619.3671235057049L1078.2430451899418,633.2675144578387L1104.190441633925,630.487436267412L1143.1115362999,628.6340508071274L1145.891614490327,623.0738944262739L1143.1115362999,602.6866543631442L1136.6246871889043,573.0324869985917L1131.991223538193,554.4986323957464Z
 - drawn_on_frame: 38000
   line_color: '#DA16FF'
   name: nectar2_box
   path: M812.2822316391125,845.4801496604169L809.5021534486857,922.3956462622248L859.5435608763679,920.5422608019403L881.7841863997821,911.2753335005176L884.564264590209,894.5948643579569L885.4909573203512,861.2339260728354L882.7108791299245,835.2865296288521Z
 - drawn_on_frame: 38000
   line_color: '#222A2A'
```

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspE_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspE_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspE_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspE_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspG_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspG_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspG_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspG_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspG_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspH_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspH_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspH_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspH_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspH_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspI_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspI_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspI_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspI_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspI_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspJ_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspJ_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspJ_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspJ_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspJ_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspK_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspK_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspK_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspK_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspK_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspL_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspL_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspL_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspL_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspL_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspM_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspM_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspM_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspM_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspM_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspN_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspN_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspN_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspN_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspN_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_control.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspO_nectar-open-close_control.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_nectar1.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspO_nectar-open-close_nectar1.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_nectar2.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspO_nectar-open-close_nectar2.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/sample_project/videos/jwaspO_nectar-open-close_wateronly_s.metadata.yaml` & `WAZP-0.2.1/sample_project/videos/jwaspO_nectar-open-close_wateronly_s.metadata.yaml`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/tests/test_integration/test_smoke.py` & `WAZP-0.2.1/tests/test_integration/test_smoke.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/tests/test_unit/test_utils.py` & `WAZP-0.2.1/tests/test_unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/wazp/app.py` & `WAZP-0.2.1/wazp/app.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/wazp/callbacks/dashboard.py` & `WAZP-0.2.1/wazp/callbacks/dashboard.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/wazp/callbacks/home.py` & `WAZP-0.2.1/wazp/callbacks/home.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/wazp/callbacks/metadata.py` & `WAZP-0.2.1/wazp/callbacks/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -240,15 +240,14 @@
         -------
         html.Div
             html component holding the metadata dash_table and
             the auxiliary buttons for common table manipulations
         """
 
         if not metadata_output_children:
-
             metadata_table = create_metadata_table_component_from_df(
                 utils.df_from_metadata_yaml_files(
                     app_storage["config"]["videos_dir_path"],
                     app_storage["metadata_fields"],
                 ),
                 app_storage["config"],
             )
@@ -342,26 +341,39 @@
                     id="import-message",
                     dismissable=True,
                     fade=False,
                     is_open=False,
                 ),
             )
 
+            # check for missing metadata files
+            check_missing_files_tooltip = dbc.Tooltip(
+                "Check which videos in the "
+                "video directory are metadata "
+                "and add a row for each of them. Note "
+                "this won't save the metadata.",
+                target="add-rows-for-missing-button",
+            )
+
             generate_yaml_tooltip = dbc.Tooltip(
-                "Generate YAML files for each row in the selected spreadsheet "
-                "and save them in the videos directory",
+                "Generate metadata files from a selected spreadsheet. "
+                "Rows in the spreadsheet that do not correspond to a "
+                "video will be ignored."
+                "WARNING! This will overwrite any existing metadata "
+                "files with the same name!",
                 target="generate-yaml-files-button",
             )
 
             return html.Div(
                 [
                     metadata_table,
                     auxiliary_buttons_row,
                     alert_message_row,
                     import_message_row,
+                    check_missing_files_tooltip,
                     generate_yaml_tooltip,
                 ]
             )
 
     @app.callback(
         Output("metadata-table", "data"),
         Output("add-row-manually-button", "n_clicks"),
@@ -542,15 +554,14 @@
                 data,
                 list_selected_rows,
             )
 
         # If the export button is clicked: export selected rows and unselect
         # TODO: add if not list_selected_rows: message--no data to export
         if (n_clicks_export > 0) and list_selected_rows:
-
             # export yaml files
             utils.export_selected_rows_as_yaml(
                 data, list_selected_rows, app_storage["config"]
             )
 
             # display alert if successful import
             # TODO: what is a better way to check if export was successful?
@@ -658,41 +669,51 @@
                 import_message_text = (
                     "There was an error reading" f" this file ({e})."
                 )
                 import_message_color = "danger"
 
             # convert all fields in dataframe to strings
             # (otherwise datetime fields are not encoded correctly in the YAML)
-            # TODO: is it better to use to_json instead?
-            # if so I think date encodes in
-            # epoch milliseconds
-            # list_dict_per_row = df.to_json('records')
             df = df.applymap(str)
 
-            # check if columns match metadata file: if not
-            # add missing columns
+            # check if columns in spreadsheet match metadata file:
+            # if not, add missing columns
             list_columns = df.columns.tolist()
             list_metadata_fields = list(app_storage["metadata_fields"].keys())
             list_columns_to_add = [
                 f for f in list_metadata_fields if f not in list_columns
             ]
-            # TODO: use sets instead? (more efficient?
-            # not symmetric diff though)
             # TODO: warn/break if columns only in spreadsheet?
             for col in list_columns_to_add:
                 df[col] = ""
 
             # convert to list of dictionaries, one per row
             list_dict_per_row = df.to_dict("records")
 
-            # dump each row as a yaml
+            # exclude rows that do not exist as a video file or a symlink
+            # in the video dir
+            # TODO: select whether to overwrite existing YAML?
             video_dir = app_storage["config"]["videos_dir_path"]
             field_to_use_as_filename = app_storage["config"][
                 "metadata_key_field_str"
             ]
+
+            list_filepaths_to_check = [
+                pl.Path(video_dir, row[field_to_use_as_filename])
+                for row in list_dict_per_row
+            ]
+            list_dict_per_row = [
+                row
+                for row, fpath in zip(
+                    list_dict_per_row, list_filepaths_to_check
+                )
+                if pl.Path(fpath).is_file() or pl.Path(fpath).is_symlink()
+            ]
+
+            # dump as yaml files
             for row in list_dict_per_row:
                 yaml_filename = (
                     pl.Path(row[field_to_use_as_filename]).stem
                     + ".metadata.yaml"
                 )
 
                 with open(pl.Path(video_dir) / yaml_filename, "w") as yamlf:
```

### Comparing `WAZP-0.2.0/wazp/callbacks/roi.py` & `WAZP-0.2.1/wazp/callbacks/roi.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,25 +80,35 @@
 
     @app.callback(
         [
             Output("roi-select", "options"),
             Output("roi-select", "value"),
             Output("roi-colors-storage", "data"),
         ],
-        Input("session-storage", "data"),
+        [
+            Input("session-storage", "data"),
+            Input("roi-storage", "data"),
+            Input("video-select", "value"),
+        ],
     )
     def update_roi_select_options(
         app_storage: dict,
+        roi_storage: dict,
+        video_path: str,
     ) -> Optional[tuple[list[dict], str, dict]]:
         """Update the options of the ROI select dropdown.
         Parameters
         ----------
         app_storage : dict
             data held in temporary memory storage,
             accessible to all tabs in the app
+        roi_storage : dict
+            Dictionary storing ROI data for each video.
+        video_path : str
+            Path to the video file.
         Returns
         -------
         list[dict]
             list of dictionaries with keys 'label' and 'value'
         str
             value of the first ROI in the list
         dict
@@ -107,22 +117,45 @@
                 - color2roi: dict mapping colors to ROI names
         """
         if "config" in app_storage.keys():
             # Get ROI names from stored config
             config = app_storage["config"]
             roi_names = config["ROI_tags"]
             options = [{"label": r, "value": r} for r in roi_names]
-            value = roi_names[0]
 
             # Get ROI-to-color mapping
             roi_color_mapping = utils.assign_roi_colors(
                 roi_names, cmap=ROI_CMAP
             )
 
+            video_name = pl.Path(video_path).name
+            # restrict ROI options to the ones not already stored
+            if video_name in roi_storage.keys():
+                stored_roi_names = [
+                    shape["roi_name"]
+                    for shape in roi_storage[video_name]["shapes"]
+                ]
+                options = [
+                    opt
+                    for opt in options
+                    if opt["value"] not in stored_roi_names
+                ]
+
+            # If there are no ROIs to draw
+            if len(options) == 0:
+                # Display a message in the ROI dropdown
+                options = [
+                    {"label": "All ROIs have been drawn.", "value": "none"}
+                ]
+
+            # Set the value to the first ROI in the list
+            value = options[0]["value"]
+
             return options, value, roi_color_mapping
+
         else:
             return dash.no_update, dash.no_update, dash.no_update
 
     @app.callback(
         [
             Output("frame-slider", "max"),
             Output("frame-slider", "step"),
@@ -521,31 +554,35 @@
         if video_name in roi_storage.keys():
             stored_shapes = roi_storage[video_name]["shapes"]
             # Get rid of the custom keys that we added
             graph_shapes = [
                 utils.shape_drop_custom_keys(shape) for shape in stored_shapes
             ]
         # Get the color for the next ROI
-        next_shape_color = roi_color_mapping["roi2color"][roi_name]
+        if roi_name == "none":
+            # if it's none, don't allow drawing
+            # and set the color to transparent
+            next_shape_color = "rgba(0,0,0,0)"
+            drag_mode = False  # type: ignore
+        else:
+            next_shape_color = roi_color_mapping["roi2color"][roi_name]
+            drag_mode = "drawclosedpath"  # type: ignore
+
+        current_fig["layout"]["newshape"]["line"]["color"] = next_shape_color
+        current_fig["layout"]["dragmode"] = drag_mode
+        current_fig["layout"]["shapes"] = graph_shapes
 
         trigger = dash.callback_context.triggered[0]["prop_id"]
-        # If triggered by an update of the roi-storage
-        # maintain the current figure and only update the shapes
-        if trigger == "roi-storage.data":
+        # If triggered by an update of the roi-storage or of the
+        # roi-dropdown, maintain the current figure with updated
+        # shapes, next shape color and drag mode
+        if (trigger == "roi-storage.data") or (trigger == "roi-select.value"):
             current_fig["layout"]["shapes"] = graph_shapes
             return current_fig, dash.no_update, dash.no_update, dash.no_update
 
-        # If triggered by a change in the ROI dropdown
-        # maintain the current figure and only update the new shape color
-        elif trigger == "roi-select.value":
-            current_fig["layout"]["newshape"]["line"][
-                "color"
-            ] = next_shape_color
-            return current_fig, dash.no_update, dash.no_update, dash.no_update
-
         # If triggered by a change in the video or frame
         # Load the frame into a new figure
         else:
             try:
                 frame_filepath = utils.cache_frame(
                     video_path_pl, shown_frame_idx
                 )
@@ -554,15 +591,15 @@
 
             new_frame = Image.open(frame_filepath)
             new_fig = px.imshow(new_frame)
             # Add the stored shapes and set the nextROI color
             new_fig.update_layout(
                 shapes=graph_shapes,
                 newshape_line_color=next_shape_color,
-                dragmode="drawclosedpath",
+                dragmode=drag_mode,
                 margin=dict(l=0, r=0, t=0, b=0),
                 yaxis={"visible": False, "showticklabels": False},
                 xaxis={"visible": False, "showticklabels": False},
             )
             alert_msg = f"Showing frame {shown_frame_idx}/{max_frame_idx}"
             return new_fig, alert_msg, "light", True
```

### Comparing `WAZP-0.2.0/wazp/pages/02_ROI.py` & `WAZP-0.2.1/wazp/pages/02_ROI.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/wazp/pages/04_dashboard.py` & `WAZP-0.2.1/wazp/pages/04_dashboard.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/wazp/pages/home.py` & `WAZP-0.2.1/wazp/pages/home.py`

 * *Files identical despite different names*

### Comparing `WAZP-0.2.0/wazp/utils.py` & `WAZP-0.2.1/wazp/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -769,24 +769,23 @@
                 raise KeyError(f"Could not find key 'ROIs' in {yaml_path}")
     else:
         raise FileNotFoundError(f"Could not find {yaml_path}")
 
     return shapes_to_store
 
 
-def are_same_shape(shape0: dict, shape1: dict) -> bool:
-    """Checks if two shapes are the same"""
-    same_coords = shape0["path"] == shape1["path"]
+def shapes_same_color(shape0: dict, shape1: dict) -> bool:
+    """Checks if two shapes have the same color"""
     same_color = shape0["line"]["color"] == shape1["line"]["color"]
-    return same_coords and same_color
+    return same_color
 
 
 def shape_in_list(shape_list: list) -> Callable[[dict], bool]:
     """Checks if a shape is already in a list of shapes"""
-    return lambda s: any(are_same_shape(s, s_) for s_ in shape_list)
+    return lambda s: any(shapes_same_color(s, s_) for s_ in shape_list)
 
 
 def shape_drop_custom_keys(shape: dict) -> dict:
     """
     plotly.graph_objects.Figure complains if we include custom
     keys in the shape dictionary, so we remove them here
     """
```

