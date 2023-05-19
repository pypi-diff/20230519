# Comparing `tmp/dkist-1.0.0b8.tar.gz` & `tmp/dkist-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-1.0.0b8.tar", last modified: Mon Jul 18 22:10:52 2022, max compression
+gzip compressed data, was "dkist-1.0.0b9.tar", last modified: Fri Sep 30 13:51:45 2022, max compression
```

## Comparing `dkist-1.0.0b8.tar` & `dkist-1.0.0b9.tar`

### file list

```diff
@@ -1,183 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.278501 dkist-1.0.0b8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.258501 dkist-1.0.0b8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.266501 dkist-1.0.0b8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-07-18 22:10:36.000000 dkist-1.0.0b8/.github/ISSUE_TEMPLATE/BUG_REPORT.md
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-07-18 22:10:36.000000 dkist-1.0.0b8/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-07-18 22:10:36.000000 dkist-1.0.0b8/.github/ISSUE_TEMPLATE/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.266501 dkist-1.0.0b8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-07-18 22:10:36.000000 dkist-1.0.0b8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-07-18 22:10:36.000000 dkist-1.0.0b8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:36.000000 dkist-1.0.0b8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-07-18 22:10:36.000000 dkist-1.0.0b8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-07-18 22:10:36.000000 dkist-1.0.0b8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11611 2022-07-18 22:10:36.000000 dkist-1.0.0b8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-07-18 22:10:36.000000 dkist-1.0.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-07-18 22:10:52.278501 dkist-1.0.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-07-18 22:10:36.000000 dkist-1.0.0b8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-07-18 22:10:36.000000 dkist-1.0.0b8/azure-pipelines.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.266501 dkist-1.0.0b8/changelog/
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-07-18 22:10:36.000000 dkist-1.0.0b8/changelog/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-18 22:10:36.000000 dkist-1.0.0b8/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-18 22:10:36.000000 dkist-1.0.0b8/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.266501 dkist-1.0.0b8/dkist/
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.266501 dkist-1.0.0b8/dkist/config/
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9961 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.266501 dkist-1.0.0b8/dkist/data/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.266501 dkist-1.0.0b8/dkist/data/test/
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/5d_gwcs.asdf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.270501 dkist-1.0.0b8/dkist/data/test/EIT/
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.000010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.020010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.030011_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.040010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.050010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.060010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.080010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.090010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.100010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.110010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.120010_s.fits
--rw-r--r--   0 runner    (1001) docker     (121)   100114 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/EIT/eit_test_dataset.asdf
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    96835 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/eit_dataset_0.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (121)    96980 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/eit_dataset_0.2.0.asdf
--rw-r--r--   0 runner    (1001) docker     (121)    97623 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/eit_dataset_0.3.0.asdf
--rw-r--r--   0 runner    (1001) docker     (121)   100114 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/eit_dataset_1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (121)     3812 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/globus_operation_ls_response.json
--rw-r--r--   0 runner    (1001) docker     (121)    42219 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/data/test/globus_search_response.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.270501 dkist-1.0.0b8/dkist/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7576 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.270501 dkist-1.0.0b8/dkist/dataset/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/dataset/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3325 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/dataset/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/dataset/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/dataset/tests/test_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4491 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/dataset/tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4017 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/dataset/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/dkist.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.270501 dkist-1.0.0b8/dkist/extern/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.270501 dkist-1.0.0b8/dkist/io/
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.270501 dkist-1.0.0b8/dkist/io/asdf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.270501 dkist-1.0.0b8/dkist/io/asdf/converters/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/converters/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/converters/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4926 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/converters/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/converters/tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/entry_points.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.270501 dkist-1.0.0b8/dkist/io/asdf/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.270501 dkist-1.0.0b8/dkist/io/asdf/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     3049 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/io/asdf/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4567 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5471 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/asdf/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14191 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/level_1_dataset_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/io/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8581 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/tests/test_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/io/tests/test_fits.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/net/
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6082 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (121)    11073 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8869 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/net/globus/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6240 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/globus/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     5370 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/globus/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/net/globus/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/globus/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4156 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/globus/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/globus/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     8902 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/globus/tests/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (121)    12581 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/globus/transfer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4184 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/net/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4066 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (121)     7115 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/tests/test_attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (121)     8299 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/net/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/tests/coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)     7508 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/tests/generate_aia_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4986 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/tests/generate_eit_test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/tests/setup_package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/utils/inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/utils/sysinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/utils/tests/test_inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/wcs/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28887 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/wcs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.274501 dkist-1.0.0b8/dkist/wcs/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5936 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/wcs/tests/test_coupled_compound_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    15353 2022-07-18 22:10:36.000000 dkist-1.0.0b8/dkist/wcs/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.266501 dkist-1.0.0b8/dkist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-07-18 22:10:52.000000 dkist-1.0.0b8/dkist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4458 2022-07-18 22:10:52.000000 dkist-1.0.0b8/dkist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 22:10:52.000000 dkist-1.0.0b8/dkist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-07-18 22:10:52.000000 dkist-1.0.0b8/dkist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-07-18 22:10:52.000000 dkist-1.0.0b8/dkist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-18 22:10:52.000000 dkist-1.0.0b8/dkist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.278501 dkist-1.0.0b8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6340 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3753 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/developer.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.278501 dkist-1.0.0b8/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/guide/level1data.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6376 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/guide/loading.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8545 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/guide/net.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/guide/usertools.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.278501 dkist-1.0.0b8/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (121)    72150 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/logo/icon_square.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.278501 dkist-1.0.0b8/docs/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/whatsnew/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-07-18 22:10:36.000000 dkist-1.0.0b8/docs/whatsnew/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.278501 dkist-1.0.0b8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-07-18 22:10:36.000000 dkist-1.0.0b8/examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-07-18 22:10:36.000000 dkist-1.0.0b8/examples/create_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 22:10:52.278501 dkist-1.0.0b8/licenses/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-18 22:10:36.000000 dkist-1.0.0b8/licenses/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-07-18 22:10:36.000000 dkist-1.0.0b8/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-07-18 22:10:36.000000 dkist-1.0.0b8/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-07-18 22:10:36.000000 dkist-1.0.0b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4173 2022-07-18 22:10:52.282501 dkist-1.0.0b8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       58 2022-07-18 22:10:36.000000 dkist-1.0.0b8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-07-18 22:10:36.000000 dkist-1.0.0b8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.192241 dkist-1.0.0b9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.172242 dkist-1.0.0b9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.176242 dkist-1.0.0b9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-09-30 13:51:30.000000 dkist-1.0.0b9/.github/ISSUE_TEMPLATE/BUG_REPORT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-30 13:51:30.000000 dkist-1.0.0b9/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-30 13:51:30.000000 dkist-1.0.0b9/.github/ISSUE_TEMPLATE/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.176242 dkist-1.0.0b9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-09-30 13:51:30.000000 dkist-1.0.0b9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-09-30 13:51:30.000000 dkist-1.0.0b9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:30.000000 dkist-1.0.0b9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-09-30 13:51:30.000000 dkist-1.0.0b9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-09-30 13:51:30.000000 dkist-1.0.0b9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    12871 2022-09-30 13:51:30.000000 dkist-1.0.0b9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-30 13:51:30.000000 dkist-1.0.0b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-09-30 13:51:45.192241 dkist-1.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-30 13:51:30.000000 dkist-1.0.0b9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-09-30 13:51:30.000000 dkist-1.0.0b9/azure-pipelines.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.176242 dkist-1.0.0b9/changelog/
+-rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-09-30 13:51:30.000000 dkist-1.0.0b9/changelog/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-30 13:51:30.000000 dkist-1.0.0b9/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-30 13:51:30.000000 dkist-1.0.0b9/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.176242 dkist-1.0.0b9/dkist/
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.176242 dkist-1.0.0b9/dkist/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10803 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.176242 dkist-1.0.0b9/dkist/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.176242 dkist-1.0.0b9/dkist/data/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/5d_gwcs.asdf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.180241 dkist-1.0.0b9/dkist/data/test/EIT/
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.000010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.020010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.030011_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.040010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.050010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.060010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.080010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.090010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.100010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.110010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.120010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   100114 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/EIT/eit_test_dataset.asdf
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    96835 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/eit_dataset_0.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (121)    96980 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/eit_dataset_0.2.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (121)    97623 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/eit_dataset_0.3.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (121)   100114 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/eit_dataset_1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (121)     3812 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/globus_operation_ls_response.json
+-rw-r--r--   0 runner    (1001) docker     (121)    42219 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/globus_search_response.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.180241 dkist-1.0.0b9/dkist/data/test/small_visp/
+-rw-r--r--   0 runner    (1001) docker     (121)    25920 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/small_visp/0.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    25920 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/small_visp/1.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    25920 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/small_visp/2.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   107103 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/data/test/small_visp/test_visp.asdf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.180241 dkist-1.0.0b9/dkist/dataset/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7576 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.180241 dkist-1.0.0b9/dkist/dataset/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/dataset/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3374 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/dataset/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/dataset/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/dataset/tests/test_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4491 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/dataset/tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4017 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/dkist.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.180241 dkist-1.0.0b9/dkist/extern/
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.180241 dkist-1.0.0b9/dkist/io/
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.180241 dkist-1.0.0b9/dkist/io/asdf/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.184241 dkist-1.0.0b9/dkist/io/asdf/converters/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/converters/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/converters/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4926 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/converters/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/converters/tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/entry_points.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.184241 dkist-1.0.0b9/dkist/io/asdf/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.184241 dkist-1.0.0b9/dkist/io/asdf/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.184241 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)     3049 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.184241 dkist-1.0.0b9/dkist/io/asdf/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4567 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5471 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/asdf/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14565 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/level_1_dataset_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.184241 dkist-1.0.0b9/dkist/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9302 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/tests/test_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/io/tests/test_fits.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.188241 dkist-1.0.0b9/dkist/net/
+-rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6082 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11150 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8913 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.188241 dkist-1.0.0b9/dkist/net/globus/
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6240 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/globus/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5370 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/globus/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.188241 dkist-1.0.0b9/dkist/net/globus/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/globus/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/globus/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/globus/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8881 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/globus/tests/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12542 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/globus/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4689 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.188241 dkist-1.0.0b9/dkist/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4066 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7115 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/tests/test_attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8382 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4670 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/net/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.188241 dkist-1.0.0b9/dkist/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/tests/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)     7508 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/tests/generate_aia_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4986 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/tests/generate_eit_test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/tests/setup_package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.188241 dkist-1.0.0b9/dkist/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/utils/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/utils/sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.188241 dkist-1.0.0b9/dkist/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/utils/tests/test_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.188241 dkist-1.0.0b9/dkist/wcs/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28887 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/wcs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.188241 dkist-1.0.0b9/dkist/wcs/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     5936 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/wcs/tests/test_coupled_compound_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15353 2022-09-30 13:51:30.000000 dkist-1.0.0b9/dkist/wcs/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.176242 dkist-1.0.0b9/dkist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-09-30 13:51:45.000000 dkist-1.0.0b9/dkist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4602 2022-09-30 13:51:45.000000 dkist-1.0.0b9/dkist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 13:51:45.000000 dkist-1.0.0b9/dkist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-09-30 13:51:45.000000 dkist-1.0.0b9/dkist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-09-30 13:51:45.000000 dkist-1.0.0b9/dkist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-30 13:51:45.000000 dkist-1.0.0b9/dkist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.192241 dkist-1.0.0b9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     6340 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3753 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/developer.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.192241 dkist-1.0.0b9/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/guide/level1data.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6376 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/guide/loading.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8545 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/guide/net.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/guide/usertools.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.192241 dkist-1.0.0b9/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (121)    72150 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/logo/icon_square.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.192241 dkist-1.0.0b9/docs/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/whatsnew/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-09-30 13:51:30.000000 dkist-1.0.0b9/docs/whatsnew/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.192241 dkist-1.0.0b9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-09-30 13:51:30.000000 dkist-1.0.0b9/examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-09-30 13:51:30.000000 dkist-1.0.0b9/examples/create_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:51:45.192241 dkist-1.0.0b9/licenses/
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-09-30 13:51:30.000000 dkist-1.0.0b9/licenses/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-30 13:51:30.000000 dkist-1.0.0b9/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-09-30 13:51:30.000000 dkist-1.0.0b9/licenses/TEMPLATE_LICENCE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-09-30 13:51:30.000000 dkist-1.0.0b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     4266 2022-09-30 13:51:45.192241 dkist-1.0.0b9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)       58 2022-09-30 13:51:30.000000 dkist-1.0.0b9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2176 2022-09-30 13:51:30.000000 dkist-1.0.0b9/tox.ini
```

### Comparing `dkist-1.0.0b8/.github/ISSUE_TEMPLATE/BUG_REPORT.md` & `dkist-1.0.0b9/.github/ISSUE_TEMPLATE/BUG_REPORT.md`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md` & `dkist-1.0.0b9/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/.github/workflows/main.yml` & `dkist-1.0.0b9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/.gitignore` & `dkist-1.0.0b9/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/.pre-commit-config.yaml` & `dkist-1.0.0b9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/CHANGELOG.rst` & `dkist-1.0.0b9/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+1.0.0b9 (2022-09-30)
+====================
+
+Features
+--------
+
+- Add a ``label=`` kwarg to `.FileManager.download` and
+  `.transfer_complete_datasets` allowing the user to completely customise the
+  Globus transfer task label. (`#193 <https://github.com/DKISTDC/dkist/pull/193>`_)
+
+
+Bug Fixes
+---------
+
+- Successfully ask for re-authentication when Globus token is stale. (`#197 <https://github.com/DKISTDC/dkist/pull/197>`_)
+- Fix a bug where ``FileManager.download`` would fail if there was not an
+  asdf file or quality report PDF in inventory. (`#199 <https://github.com/DKISTDC/dkist/pull/199>`_)
+- Fix an issue with slicing a dataset where the slicing wouldn't work correctly
+  if the first axis of the data array has length one. (`#199 <https://github.com/DKISTDC/dkist/pull/199>`_)
+- No more invalid characters in default Globus label name. (`#200 <https://github.com/DKISTDC/dkist/pull/200>`_)
+- Hide extraneous names in `dkist.net.attrs` with underscores so they don't get imported when using that module. (`#201 <https://github.com/DKISTDC/dkist/pull/201>`_)
+- Catch empty return value from data search in `transfer_complete_datasets` and raise a ValueError telling the user what's happening. (`#204 <https://github.com/DKISTDC/dkist/pull/204>`_)
+
+
 v1.0.0b8 (2022-07-18)
 =====================
 
 Features
 --------
 
 - Support passing a whole `~sunpy.net.fido_factory.UnifiedResponse` to
```

### Comparing `dkist-1.0.0b8/PKG-INFO` & `dkist-1.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: DKIST User Tools
 Home-page: http://dkist.nso.edu
 Author: NSO / AURA
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-1.0.0b8/README.rst` & `dkist-1.0.0b9/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/azure-pipelines.yml` & `dkist-1.0.0b9/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/changelog/README.rst` & `dkist-1.0.0b9/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/__init__.py` & `dkist-1.0.0b9/dkist/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/conftest.py` & `dkist-1.0.0b9/dkist/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -259,7 +259,31 @@
 @pytest.fixture
 def simple_tiled_dataset(dataset):
     datasets = [copy.deepcopy(dataset) for i in range(4)]
     for ds in datasets:
         ds.meta['inventory'] = dataset.meta['inventory']
     dataset_array = np.array(datasets).reshape((2,2))
     return TiledDataset(dataset_array, dataset.meta['inventory'])
+
+
+@pytest.fixture
+def small_visp_dataset():
+    """
+    This fixture is used to test when the array in the FITS file has a length
+    one NAXIS 3.
+    """
+    # This asdf file wont work with sunpy less than 4
+    pytest.importorskip("sunpy", "4.0.0")
+
+    # This dataset was generated by the following code:
+    # from dkist_data_simulator.spec214.visp import SimpleVISPDataset
+    # from dkist_inventory.asdf_generator import dataset_from_fits
+    # import astropy.units as u
+
+    # ds = SimpleVISPDataset(n_maps=1, n_steps=3, n_stokes=1, time_delta=10,
+    #                        linewave=500*u.nm, detector_shape=(10, 25))
+    # ds.generate_files(vispdir)
+    # dataset_from_fits(vispdir, "test_visp.asdf")
+
+    vispdir = Path(rootdir) / "small_visp"
+    with asdf.open(vispdir / "test_visp.asdf") as f:
+        return f.tree['dataset']
```

### Comparing `dkist-1.0.0b8/dkist/data/test/5d_gwcs.asdf` & `dkist-1.0.0b9/dkist/data/test/5d_gwcs.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.000010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.000010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.020010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.020010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.030011_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.030011_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.040010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.040010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.050010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.050010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.060010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.060010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.080010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.080010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.090010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.090010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.100010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.100010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.110010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.110010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/efz20040301.120010_s.fits` & `dkist-1.0.0b9/dkist/data/test/EIT/efz20040301.120010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/EIT/eit_test_dataset.asdf` & `dkist-1.0.0b9/dkist/data/test/EIT/eit_test_dataset.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/eit_dataset_0.1.0.asdf` & `dkist-1.0.0b9/dkist/data/test/eit_dataset_0.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/eit_dataset_0.2.0.asdf` & `dkist-1.0.0b9/dkist/data/test/eit_dataset_0.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/eit_dataset_0.3.0.asdf` & `dkist-1.0.0b9/dkist/data/test/eit_dataset_0.3.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/eit_dataset_1.0.0.asdf` & `dkist-1.0.0b9/dkist/data/test/eit_dataset_1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/globus_operation_ls_response.json` & `dkist-1.0.0b9/dkist/data/test/globus_operation_ls_response.json`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/data/test/globus_search_response.json` & `dkist-1.0.0b9/dkist/data/test/globus_search_response.json`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/dataset/dataset.py` & `dkist-1.0.0b9/dkist/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/dataset/tests/test_dataset.py` & `dkist-1.0.0b9/dkist/dataset/tests/test_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,12 +106,13 @@
     with pytest.raises(AttributeError):
         dataset.files = 10
 
     assert len(dataset.files.filenames) == 11
     assert len(dataset.files.filenames) == 11
 
     assert isinstance(dataset[5]._file_manager, FileManager)
-    assert len(dataset[..., 5].files.filenames) == 1
+    assert len(dataset[..., 5].files.filenames) == 11
+    assert len(dataset[5].files.filenames) == 1
 
 
 def test_no_file_manager(dataset_3d):
     assert dataset_3d.files is None
```

### Comparing `dkist-1.0.0b8/dkist/dataset/tests/test_plotting.py` & `dkist-1.0.0b9/dkist/dataset/tests/test_plotting.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 from astropy.visualization.wcsaxes import WCSAxes
 
 
 @pytest.mark.parametrize("aslice", (np.s_[0, :, :], np.s_[:, 0, :], np.s_[:, :, 0]))
 def test_dataset_projection(dataset_3d, aslice):
     pytest.importorskip("ndcube", "2.0.2")  # https://github.com/sunpy/ndcube/pull/509
     ds = dataset_3d[aslice]
+    fig = plt.figure()
     ax = plt.subplot(projection=ds)
     assert isinstance(ax, WCSAxes)
+    return fig
 
 
 # @pytest.mark.mpl_image_compare
 @pytest.mark.parametrize("aslice", (np.s_[0, :, :], np.s_[:, 0, :], np.s_[:, :, 0]))
 def test_2d_plot(dataset_3d, aslice):
+    fig = plt.figure()
     dataset_3d[aslice].plot()
-    return plt.gcf()
+    return fig
 
 
 # @pytest.mark.mpl_image_compare
 def test_2d_plot2(dataset_3d):
+    fig = plt.figure()
     dataset_3d[:, :, 0].plot(axes_units=["Angstrom", "deg", "deg"])
-    return plt.gcf()
+    return fig
```

### Comparing `dkist-1.0.0b8/dkist/dataset/tests/test_tiled_dataset.py` & `dkist-1.0.0b9/dkist/dataset/tests/test_tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/dataset/tiled_dataset.py` & `dkist-1.0.0b9/dkist/dataset/tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/dataset/utils.py` & `dkist-1.0.0b9/dkist/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/converters/dataset.py` & `dkist-1.0.0b9/dkist/io/asdf/converters/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/converters/file_manager.py` & `dkist-1.0.0b9/dkist/io/asdf/converters/file_manager.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/converters/models.py` & `dkist-1.0.0b9/dkist/io/asdf/converters/models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/converters/tiled_dataset.py` & `dkist-1.0.0b9/dkist/io/asdf/converters/tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/entry_points.py` & `dkist-1.0.0b9/dkist/io/asdf/entry_points.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml` & `dkist-1.0.0b9/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/tests/test_dataset.py` & `dkist-1.0.0b9/dkist/io/asdf/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/asdf/tests/test_models.py` & `dkist-1.0.0b9/dkist/io/asdf/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/dask_utils.py` & `dkist-1.0.0b9/dkist/io/dask_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/file_manager.py` & `dkist-1.0.0b9/dkist/io/file_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -221,33 +221,34 @@
     def __eq__(self, other):
         return self._striped_external_array == other._striped_external_array
 
     def __len__(self):
         return len(self._striped_external_array)
 
     def __str__(self) -> str:
-        return f"FileManager containing {len(self)} files with shape {self.shape}"
+        return f"FileManager containing {len(self)} files with each array having shape {self.shape}"
 
     def __repr__(self) -> str:
         return f"{object.__repr__(self)}\n{self}"
 
     def __getitem__(self, item):
         item = sanitize_slices(item, self._striped_external_array.reference_array.ndim)
         return type(self)(StripedExternalArrayView(self._striped_external_array, item))
 
     def _array_slice_to_reference_slice(self, aslice):
         """
         Convert a slice for the reconstructed array to a slice for the reference_array.
         """
-        shape = self._striped_external_array.shape
+        fits_array_shape = self._striped_external_array.shape
         aslice = list(sanitize_slices(aslice, len(self.output_shape)))
-        if shape[0] == 1:
-            # Insert a blank slice for the removed dimension
-            aslice.insert(len(shape) - 1, slice(None))
-        aslice = aslice[len(shape) :]
+        if fits_array_shape[0] == 1:
+            # Insert a blank slice for the dummy dimension
+            aslice.insert(len(fits_array_shape) - 1, slice(None))
+        # Now only use the dimensions of the slice not covered by the array axes
+        aslice = aslice[:-1*len(fits_array_shape)]
         return tuple(aslice)
 
     def _slice_by_cube(self, item):
         item = self._array_slice_to_reference_slice(item)
         loader_view = StripedExternalArrayView(self._striped_external_array, item)
         return type(self)(loader_view)
 
@@ -309,15 +310,15 @@
 
     def __init__(self, fits_loader: StripedExternalArray):
         super().__init__(fits_loader)
         # When this object is attached to a Dataset object this attribute will
         # be populated with a reference to that Dataset instance.
         self._ndcube = None
 
-    def download(self, path=None, destination_endpoint=None, progress=True, wait=True):
+    def download(self, path=None, destination_endpoint=None, progress=True, wait=True, label=None):
         """
         Start a Globus file transfer for all files in this Dataset.
 
         Parameters
         ----------
         path : `pathlib.Path` or `str`, optional
             The path to save the data in, must be accessible by the Globus
@@ -347,14 +348,17 @@
            If ``progress="verbose"`` then all globus events generated during
            the transfer will be shown (by default only error messages are
            shown.)
 
         wait : `bool`, optional
             If `False` then the function will return while the Globus transfer task
             is still running. Setting ``wait=False`` implies ``progress=False``.
+
+        label : `str`
+            Label for the Globus transfer. If `None` then a default will be used.
         """
         if self._ndcube is None:
             raise ValueError(
                 "This file manager has no associated Dataset object, so the data can not be downloaded."
             )
 
         inv = self._ndcube.meta["inventory"]
@@ -365,27 +369,30 @@
         destination_path = Path(destination_path).as_posix()
         destination_path = Path(destination_path.format(**human_inv))
 
         # TODO: If we are transferring the whole dataset then we should use the
         # directory not the list of all the files in it.
         file_list = [base_path / fn for fn in self.filenames]
         file_list.append(Path("/") / inv["bucket"] / inv["asdfObjectKey"])
-        file_list.append(Path("/") / inv["bucket"] / inv["browseMovieObjectKey"])
-        file_list.append(Path("/") / inv["bucket"] / inv["qualityReportObjectKey"])
+        if inv["browseMovieObjectKey"]:
+            file_list.append(Path("/") / inv["bucket"] / inv["browseMovieObjectKey"])
+        if inv["qualityReportObjectKey"]:
+            file_list.append(Path("/") / inv["bucket"] / inv["qualityReportObjectKey"])
 
         # TODO: Ascertain if the destination path is local better than this
         is_local = not destination_endpoint
 
         _orchestrate_transfer_task(
             file_list,
             recursive=False,
             destination_path=destination_path,
             destination_endpoint=destination_endpoint,
             progress=progress,
             wait=wait,
+            label=label
         )
 
         if is_local:
             if str(destination_path).startswith("/~/"):
                 local_destination = Path(str(destination_path)[1:])
             local_destination = destination_path.expanduser()
             self.basepath = local_destination
```

### Comparing `dkist-1.0.0b8/dkist/io/level_1_dataset_schema.yaml` & `dkist-1.0.0b9/dkist/io/level_1_dataset_schema.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/loaders.py` & `dkist-1.0.0b9/dkist/io/loaders.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/io/tests/test_file_manager.py` & `dkist-1.0.0b9/dkist/io/tests/test_file_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,22 @@
 
     # Check that we haven't made a copy
     assert ds.files is not sds.files
 
     # Assert that we have copied the value of basepath
     assert ds.files.basepath == sds.files.basepath
 
+    sds = ds[0]
+
+    # Check that we haven't made a copy
+    assert ds.files is not sds.files
+
+    # Assert that we have copied the value of basepath
+    assert ds.files.basepath == sds.files.basepath
+
     # TODO: Decide on the desired behaviour here.
     ## Running sds.download() here would affect the parent cubes data, because
     ## the base paths are the same.
 
     # If we set a new basepath on the parent cube the sub-cube shouldn't update
     # ds.files.basepath = "test1"
     # assert ds.files.basepath != sds.files.basepath
@@ -183,22 +191,24 @@
     orchestrate_transfer_mock.assert_called_once_with(
         file_list,
         recursive=False,
         destination_path=Path('/~'),
         destination_endpoint=None,
         progress=True,
         wait=True,
+        label=None,
     )
 
 
 @pytest.mark.parametrize("keywords", [
-    {"progress": True, "wait": True, "destination_endpoint": None},
-    {"progress": True, "wait": False, "destination_endpoint": None},
-    {"progress": False, "wait": True, "destination_endpoint": None},
-    {"progress": False, "wait": True, "destination_endpoint": "wibble"},
+    {"progress": True, "wait": True, "destination_endpoint": None, "label": None},
+    {"progress": True, "wait": False, "destination_endpoint": None, "label": None},
+    {"progress": False, "wait": True, "destination_endpoint": None, "label": None},
+    {"progress": False, "wait": True, "destination_endpoint": "wibble", "label": None},
+    {"progress": False, "wait": True, "destination_endpoint": None, "label": "fibble"},
 ])
 def test_download_keywords(dataset, orchestrate_transfer_mock, keywords):
     """
     Assert that keywords are passed through as expected
     """
     base_path = Path(net.conf.dataset_path.format(**dataset.meta["inventory"]))
 
@@ -234,10 +244,23 @@
     orchestrate_transfer_mock.assert_called_once_with(
         file_list,
         recursive=False,
         destination_path=Path('~/test_dataset/'),
         destination_endpoint=None,
         progress=True,
         wait=True,
+        label=None,
     )
 
     assert dataset.files.basepath == Path("~/test_dataset").expanduser()
+
+
+def test_length_one_first_array_axis(small_visp_dataset):
+    all_files = small_visp_dataset.files.filenames
+
+    assert len(all_files) == 3
+
+    assert len(small_visp_dataset[0:2].files.filenames) == 2
+
+    assert len(small_visp_dataset[0].files.filenames) == 1
+
+    assert len(small_visp_dataset[:, 5, 5].files.filenames) == 3
```

### Comparing `dkist-1.0.0b8/dkist/io/tests/test_fits.py` & `dkist-1.0.0b9/dkist/io/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/net/__init__.py` & `dkist-1.0.0b9/dkist/net/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/net/attr_walker.py` & `dkist-1.0.0b9/dkist/net/attr_walker.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/net/attrs.py` & `dkist-1.0.0b9/dkist/net/attrs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Search attributes which are specific to the `dkist.net.DKISTClient`.
 
 Other attributes provided by `sunpy.net.attrs` are supported by the client.
 """
-import astropy.units as u
+import astropy.units as _u
 import sunpy.net._attrs as _sunpy_attrs
-from sunpy.coordinates.frames import Helioprojective
-from sunpy.coordinates.utils import get_rectangle_coordinates
+from sunpy.coordinates.frames import Helioprojective as _Helioprojective
+from sunpy.coordinates.utils import get_rectangle_coordinates as _get_rectangle_coordinates
 from sunpy.net.attr import DataAttr as _DataAttr
 from sunpy.net.attr import Range as _Range
 from sunpy.net.attr import SimpleAttr as _SimpleAttr
 
 __all__ = ['Dataset', 'WavelengthBand', 'Embargoed', 'Observable',
            'Experiment', 'Proposal', 'TargetType', 'Recipe',
            'FriedParameter', 'PolarimetricAccuracy', 'ExposureTime',
@@ -148,15 +148,15 @@
     ----------
     friedmin : `u.Quantity`
         The minimum value of the average fried parameter to search between.
 
     friedmax : `u.Quantity`
         The maximum value of the average fried parameter to search between.
     """
-    def __init__(self, friedmin: u.cm, friedmax: u.cm):
+    def __init__(self, friedmin: _u.cm, friedmax: _u.cm):
         super().__init__(friedmin, friedmax)
 
     def collides(self, other):
         return isinstance(other, self.__class__)
 
 
 # qualityAveragePolarimetricAccuracyMin, qualityAverageFriedParameterMax
@@ -170,16 +170,16 @@
 
 
 # exposureTimeMin, exposureTimeMax
 class ExposureTime(_Range):
     """
     Most common exposure time of the calibrated data frames within the dataset.
     """
-    @u.quantity_input
-    def __init__(self, expmin: u.s, expmax: u.s):
+    @_u.quantity_input
+    def __init__(self, expmin: _u.s, expmax: _u.s):
         super().__init__(expmin, expmax)
 
     def collides(self, other):
         return isinstance(other, self.__class__)
 
 
 # embargoEndDateMin, embargoEndDateMax
@@ -253,26 +253,26 @@
     the time specified when passed to this function. This means that if you for
     instance pass a heliographic coordinate to this attribute for Jan 1st
     2020, but you search for a dataset on Jan 1st 2025, it will use the
     helioprojective coordinate equivalent to the heliographic coordinate passed
     as seen by an observer on Earth **on Jan 1st 2020**.
     """
 
-    def __init__(self, bottom_left, *, top_right=None, width: u.deg = None,
-                 height: u.deg = None, search="containing"):
-        bottom_left, top_right = get_rectangle_coordinates(bottom_left,
-                                                           top_right=top_right,
-                                                           width=width, height=height)
-        bottom_left = bottom_left.transform_to(Helioprojective(observer="earth"))
-        top_right = top_right.transform_to(Helioprojective(observer="earth"))
-
-        self.hpc_bounding_box_arcsec = ((bottom_left.Tx.to_value(u.arcsec),
-                                         bottom_left.Ty.to_value(u.arcsec)),
-                                        (top_right.Tx.to_value(u.arcsec),
-                                         top_right.Ty.to_value(u.arcsec)))
+    def __init__(self, bottom_left, *, top_right=None, width: _u.deg = None,
+                 height: _u.deg = None, search="containing"):
+        bottom_left, top_right = _get_rectangle_coordinates(bottom_left,
+                                                            top_right=top_right,
+                                                            width=width, height=height)
+        bottom_left = bottom_left.transform_to(_Helioprojective(observer="earth"))
+        top_right = top_right.transform_to(_Helioprojective(observer="earth"))
+
+        self.hpc_bounding_box_arcsec = ((bottom_left.Tx.to_value(_u.arcsec),
+                                         bottom_left.Ty.to_value(_u.arcsec)),
+                                        (top_right.Tx.to_value(_u.arcsec),
+                                         top_right.Ty.to_value(_u.arcsec)))
 
         self.search_type = search
 
     def collides(self, other):
         return isinstance(other, self.__class__)
 
 # averageDatasetSpectralSamplingMin, averageDatasetSpectralSamplingMax
@@ -284,16 +284,16 @@
     ----------
     spectralmin : `u.Quantity`
         The minimum value of the average spectral sampling to search between.
 
     spectralmax : `u.Quantity`
         The maximum value of the average spectral sampling to search between.
     """
-    u.quantity_input(equivalencies=u.spectral())
-    def __init__(self, spectralmin: u.nm, spectralmax: u.nm):
+    _u.quantity_input(equivalencies=_u.spectral())
+    def __init__(self, spectralmin: _u.nm, spectralmax: _u.nm):
         super().__init__(spectralmin, spectralmax)
 
     def collides(self, other):
         return isinstance(other, self.__class__)
 
 # averageDatasetSpatialSamplingMin, averageDatasetSpatialSamplingMax
 class SpatialSampling(_Range):
@@ -304,15 +304,15 @@
     ----------
     spatialmin :
         The minimum value of the average spatial sampling to search between.
 
     spatialmax :
         The maximum value of the average spatial sampling to search between.
     """
-    def __init__(self, spatialmin: u.arcsec/u.pix, spatialmax: u.arcsec/u.pix):
+    def __init__(self, spatialmin: _u.arcsec/_u.pix, spatialmax: _u.arcsec/_u.pix):
         super().__init__(spatialmin, spatialmax)
 
     def collides(self, other):
         return isinstance(other, self.__class__)
 
 # averageDatasetTemporalSamplingMin, averageDatasetTemporalSamplingMax
 class TemporalSampling(_Range):
@@ -323,12 +323,12 @@
     ----------
     temporalmin : `u.Quantity`
         The minimum value of the average temporal sampling to search between.
 
     temporalmax : `u.Quantity`
         The maximum value of the average temporal sampling to search between.
     """
-    def __init__(self, temporalmin: u.s, temporalmax: u.s):
+    def __init__(self, temporalmin: _u.s, temporalmax: _u.s):
         super().__init__(temporalmin, temporalmax)
 
     def collides(self, other):
         return isinstance(other, self.__class__)
```

### Comparing `dkist-1.0.0b8/dkist/net/client.py` & `dkist-1.0.0b9/dkist/net/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 import urllib.request
 from typing import Any, List, Mapping, Iterable
 from functools import partial
 from collections import defaultdict
 
 import aiohttp
+import numpy as np
 import parfive
 
 import astropy.units as u
 from astropy.table import TableAttribute
 from astropy.time import Time
 from sunpy.net import attr
 from sunpy.net import attrs as sattrs
@@ -56,14 +57,17 @@
                 continue  # pragma: no cover
             if not any([v is None for v in results[colname]]):
                 results[colname] = Time(results[colname])
 
         for colname, unit in units.items():
             if colname not in results.colnames:
                 continue  # pragma: no cover
+            none_values = results[colname] == None
+            if any(none_values):
+                results[colname][none_values] = np.nan
             results[colname] = u.Quantity(results[colname], unit=unit)
 
         if results:
             results["Wavelength"] = u.Quantity([results["Wavelength Min"], results["Wavelength Max"]]).T
             results.remove_columns(("Wavelength Min", "Wavelength Max"))
 
         return results
@@ -159,16 +163,15 @@
             The download manager to use.
         """
         if not len(query_results):
             return
 
         for row in query_results:
             url = f"{self._metadata_streamer_url}/asdf?datasetId={row['Dataset ID']}"
-            # Set max_splits here as the metadata streamer doesn't like accept-range at the moment.
-            downloader.enqueue_file(url, filename=partial(self._make_filename, path, row), max_splits=1)
+            downloader.enqueue_file(url, filename=partial(self._make_filename, path, row))
 
     @classmethod
     def _can_handle_query(cls, *query) -> bool:
         # This enables the client to register what kind of searches it can
         # handle, to prevent Fido using the incorrect client.
         from sunpy.net import attrs as a
```

### Comparing `dkist-1.0.0b8/dkist/net/globus/auth.py` & `dkist-1.0.0b9/dkist/net/globus/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,13 +204,13 @@
     login.
     """
     @functools.wraps(func)
     def do_reauth(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except globus_sdk.AuthAPIError as e:
-            if e.http_status == 400 and e.message == "invalid_grant":
+            if e.http_status == 400 and "invalid_grant" in e.message:
                 print("Globus login has expired.")
                 get_refresh_token_authorizer(force_reauth=True)
                 return func(*args, **kwargs)
 
     return do_reauth
```

### Comparing `dkist-1.0.0b8/dkist/net/globus/endpoints.py` & `dkist-1.0.0b9/dkist/net/globus/endpoints.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/net/globus/tests/conftest.py` & `dkist-1.0.0b9/dkist/net/globus/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/net/globus/tests/test_auth.py` & `dkist-1.0.0b9/dkist/net/globus/tests/test_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     assert isinstance(auth, globus_sdk.RefreshTokenAuthorizer)
     assert auth.access_token == cache["transfer.api.globus.org"]["access_token"]
 
 
 def test_ensure_auth_decorator(mocker):
     error = globus_sdk.AuthAPIError(mocker.MagicMock())
     mocker.patch.object(error, "http_status", 400)
-    mocker.patch.object(error, "message", "invalid_grant")
+    mocker.patch.object(error, "message", '{"error":"invalid_grant"}')
     reauth = mocker.patch("dkist.net.globus.auth.get_refresh_token_authorizer")
 
     called = [False]
     @ensure_globus_authorized
     def test_func():
         if not called[0]:
             called[0] = True
```

### Comparing `dkist-1.0.0b8/dkist/net/globus/tests/test_endpoints.py` & `dkist-1.0.0b9/dkist/net/globus/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/net/globus/tests/test_transfer.py` & `dkist-1.0.0b9/dkist/net/globus/tests/test_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,30 +191,30 @@
 
     orchestrate_mocks.start_transfer_from_file_list.assert_called_once_with(
         "patched-datacenter-endpoint-id",
         "mysecretendpoint",
         Path("/~/"),
         tfr_file_list,
         recursive=False,
-        label_suffix=None,
+        label=None,
     )
 
 
 def test_orchestrate_transfer_no_progress(tfr_file_list, mocker, orchestrate_mocks):
     _orchestrate_transfer_task(tfr_file_list, recursive=False,
                                destination_path=Path("/~/"),
                                progress=False)
 
     orchestrate_mocks.start_transfer_from_file_list.assert_called_once_with(
         "patched-datacenter-endpoint-id",
         "mysecretendpoint",
         Path("/~/"),
         tfr_file_list,
         recursive=False,
-        label_suffix=None,
+        label=None,
     )
 
     orchestrate_mocks.watch_transfer_progress.assert_not_called()
     orchestrate_mocks.get_transfer_client.return_value.task_wait.assert_called_once_with(
         "1234",
         timeout=1e6
     )
@@ -227,12 +227,12 @@
 
     orchestrate_mocks.start_transfer_from_file_list.assert_called_once_with(
         "patched-datacenter-endpoint-id",
         "mysecretendpoint",
         Path("/~/"),
         tfr_file_list,
         recursive=False,
-        label_suffix=None,
+        label=None,
     )
 
     orchestrate_mocks.watch_transfer_progress.assert_not_called()
     orchestrate_mocks.get_transfer_client.return_value.task_wait.assert_not_called()
```

### Comparing `dkist-1.0.0b8/dkist/net/globus/transfer.py` & `dkist-1.0.0b9/dkist/net/globus/transfer.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .endpoints import (auto_activate_endpoint, get_data_center_endpoint_id,
                         get_endpoint_id, get_local_endpoint_id, get_transfer_client)
 
 __all__ = ['watch_transfer_progress', 'start_transfer_from_file_list']
 
 
 def start_transfer_from_file_list(src_endpoint, dst_endpoint, dst_base_path, file_list,
-                                  src_base_path=None, recursive=False, label_suffix=None):
+                                  src_base_path=None, recursive=False, label=None):
     """
     Start a new transfer task for a list of files.
 
     Parameters
     ----------
     src_endpoint : `str`
         The endpoint to copy file from. Can be any identifier accepted by
@@ -51,16 +51,16 @@
     recursive : `bool` or `list` of `bool`, optional
        Controls if the path in ``file_list`` is added to the Globus task with
        the recursive flag or not.
        This should be `True` if the element of ``file_list`` is a directory.
        If you need to set this per-item in ``file_list`` it should be a `list`
        of `bool` of equal length as ``file_list``.
 
-    label_suffix : `str`
-       String to append to the transfer task label.
+    label : `str`
+       Label for the Globus transfer. If None then a default will be used.
 
     Returns
     -------
     `str`
         Task ID.
     """
     if isinstance(recursive, bool):
@@ -76,18 +76,18 @@
     # Resolve to IDs and activate endpoints
     src_endpoint = get_endpoint_id(src_endpoint, tc)
     auto_activate_endpoint(src_endpoint, tc)
 
     dst_endpoint = get_endpoint_id(dst_endpoint, tc)
     auto_activate_endpoint(dst_endpoint, tc)
 
-    now = datetime.datetime.now().strftime("%Y-%m-%dT%H-%M-%S")
-    label_suffix = f" {label_suffix}" if label_suffix is not None else ""
+    now = datetime.datetime.now().strftime("%Y-%m-%dT%H-%M")
+    label = f"DKIST Python Tools - {now}" if label is None else label
     transfer_manifest = globus_sdk.TransferData(tc, src_endpoint, dst_endpoint,
-                                                label=f"DKIST Python Tools - {now}{label_suffix}",
+                                                label=label,
                                                 sync_level="checksum",
                                                 verify_checksum=True)
 
     dst_base_path = pathlib.Path(dst_base_path)
     src_file_list = copy.copy(file_list)
     dst_file_list = []
     for src_file in src_file_list:
@@ -267,15 +267,15 @@
 def _orchestrate_transfer_task(file_list: List[PathLike],
                                recursive: List[bool],
                                destination_path: PathLike = "/~/",
                                destination_endpoint: str = None,
                                *,
                                progress: Union[bool, Literal["verbose"]] = True,
                                wait: bool = True,
-                               label_suffix=None):
+                               label=None):
     """
     Transfer the files given in file_list to the path on ``destination_endpoint``.
 
     Parameters
     ----------
     file_list
         The list of file paths on the source endpoint to transfer to the
@@ -302,16 +302,16 @@
         transfer will be shown (by default only error messages are shown.)
         This keyword is only used if ``wait=True``.
 
     wait
        If `False` then the function will return while the Globus transfer task
        is still running. Setting ``wait=False`` implies ``progress=False``.
 
-    label_suffix : `str`
-       String to append to the transfer task label.
+    label : `str`
+       Label for the Globus transfer. If `None` then a default will be used.
 
     Returns
     -------
     destination_path
         The path to the directory containing the dataset on the destination
         endpoint.
 
@@ -321,15 +321,15 @@
         destination_endpoint = get_local_endpoint_id()
 
     task_id = start_transfer_from_file_list(get_data_center_endpoint_id(),
                                             destination_endpoint,
                                             destination_path,
                                             file_list,
                                             recursive=recursive,
-                                            label_suffix=label_suffix)
+                                            label=label)
 
     tc = get_transfer_client()
 
     if wait:
         if progress:
             watch_transfer_progress(task_id,
                                     tc,
```

### Comparing `dkist-1.0.0b8/dkist/net/helpers.py` & `dkist-1.0.0b9/dkist/net/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Functions and classes for searching and downloading from the data center.
 """
+import datetime
 from os import PathLike
-from typing import List, Union, Literal
+from typing import List, Union, Literal, Optional
 from pathlib import Path
 
 from astropy import table
 from sunpy.net.base_client import QueryResponseRow
 from sunpy.net.fido_factory import UnifiedResponse
 
 from dkist.net.attrs import Dataset
@@ -16,22 +17,27 @@
 __all__ = ["transfer_complete_datasets"]
 
 
 def _get_dataset_inventory(dataset_id: str):  # pragma: no cover
     """
     Do a search for a single dataset id
     """
-    return DKISTClient().search(Dataset(dataset_id))
+    results = DKISTClient().search(Dataset(dataset_id))
+    if len(results) == 0:
+        raise ValueError(f"No results available for dataset {dataset_id}")
+
+    return results
 
 
 def transfer_complete_datasets(datasets: Union[str, QueryResponseRow, DKISTQueryResponseTable, UnifiedResponse],
                                path: PathLike = "/~/",
                                destination_endpoint: str = None,
                                progress: Union[bool, Literal["verbose"]] = True,
-                               wait: bool = True) -> Union[List[str], str]:
+                               wait: bool = True,
+                               label: Optional[str] = None) -> Union[List[str], str]:
     """
     Transfer one or more complete datasets to a path on a globus endpoint.
 
     Parameters
     ----------
     dataset
         The dataset to transfer. This can either be a string dataset id, or it
@@ -52,14 +58,17 @@
 
     wait
        If `True` (the default) the function will wait for the Globus transfer
        task to complete before processing the next dataset or returning from the
        function. To run multiple dataset transfer tasks in parallel (one task per
        dataset) specify ``wait=False``.
 
+    label : `str`
+        Label for the Globus transfer. If `None` then a default will be used.
+
     Returns
     -------
     The path to the directories containing the dataset(s) on the destination endpoint.
 
     """
     # Avoid circular import
     from dkist.net import conf
@@ -77,15 +86,16 @@
     if isinstance(datasets, DKISTQueryResponseTable) and len(datasets) > 1:
         paths = []
         for record in datasets:
             paths.append(transfer_complete_datasets(record,
                                                     path=path,
                                                     destination_endpoint=destination_endpoint,
                                                     progress=progress,
-                                                    wait=wait))
+                                                    wait=wait,
+                                                    label=label))
         return paths
 
     # At this point we only have one dataset
     dataset = datasets
     dataset_id = dataset["Dataset ID"]
     proposal_id = dataset["Primary Proposal ID"]
     bucket = dataset["Storage Bucket"]
@@ -94,16 +104,19 @@
 
     file_list = [Path(conf.dataset_path.format(
         datasetId=dataset_id,
         primaryProposalId=proposal_id,
         bucket=bucket
     ))]
 
+    now = datetime.datetime.now().strftime("%Y-%m-%dT%H-%M")
+    label = f"DKIST Python Tools - {now} {dataset_id}" if label is None else label
+
     _orchestrate_transfer_task(file_list,
                                recursive=True,
                                destination_path=destination_path,
                                destination_endpoint=destination_endpoint,
                                progress=progress,
                                wait=wait,
-                               label_suffix=dataset_id)
+                               label=label)
 
     return destination_path / dataset_id
```

### Comparing `dkist-1.0.0b8/dkist/net/tests/conftest.py` & `dkist-1.0.0b9/dkist/net/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/net/tests/strategies.py` & `dkist-1.0.0b9/dkist/net/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/net/tests/test_attr_walker.py` & `dkist-1.0.0b9/dkist/net/tests/test_attr_walker.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/net/tests/test_client.py` & `dkist-1.0.0b9/dkist/net/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
                 "createDate": "2020-02-28T17:05:53.330Z",
                 "experimentDescription": "string",
                 "isEmbargoed": True,
                 "updateDate": "2020-02-28T17:05:53.330Z",
                 "embargoEndDate": "2020-02-28T17:05:53.330Z",
                 "browseMovieUrl": "string",
                 "isDownloadable": True,
+                "averageDatasetSpectralSampling": None  # Some fields are optional
             }
         ],
     }
 
 
 @pytest.fixture
 def expected_table_keys():
```

### Comparing `dkist-1.0.0b8/dkist/net/tests/test_helpers.py` & `dkist-1.0.0b9/dkist/net/tests/test_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from pathlib import Path
 
 import pytest
 
 from sunpy.net.fido_factory import UnifiedResponse
 
 from dkist.net.client import DKISTClient, DKISTQueryResponseTable
@@ -12,39 +13,52 @@
 def orchestrate_transfer_mock(mocker):
     yield mocker.patch("dkist.net.helpers._orchestrate_transfer_task", autospec=True)
 
 
 @pytest.mark.parametrize(
     "keywords",
     [
-        {"progress": True, "wait": True, "destination_endpoint": None},
-        {"progress": True, "wait": False, "destination_endpoint": None},
-        {"progress": False, "wait": True, "destination_endpoint": None},
-        {"progress": False, "wait": True, "destination_endpoint": "wibble"},
+        {"progress": True, "wait": True, "destination_endpoint": None, "label": None},
+        {"progress": True, "wait": False, "destination_endpoint": None, "label": None},
+        {"progress": False, "wait": True, "destination_endpoint": None, "label": None},
+        {"progress": False, "wait": True, "destination_endpoint": "wibble", "label": None},
+        {"progress": False, "wait": True, "destination_endpoint": None, "label": "fibble"},
     ],
 )
 def test_download_default_keywords(orchestrate_transfer_mock, keywords):
     transfer_complete_datasets(
         {
             "Dataset ID": "AAAA",
             "Primary Proposal ID": "pm_1_10",
             "Storage Bucket": "data",
         },
         **keywords
     )
 
+    if keywords["label"] is None:
+        keywords["label"] = f"DKIST Python Tools - {datetime.datetime.now().strftime('%Y-%m-%dT%H-%M')} AAAA"
     orchestrate_transfer_mock.assert_called_once_with(
         [Path("/data/pm_1_10/AAAA")],
         recursive=True,
         destination_path=Path("/~/pm_1_10"),
-        label_suffix="AAAA",
         **keywords
     )
 
 
+def test_transfer_unavailable_data(mocker):
+    get_inv_mock = mocker.patch(
+        "dkist.net.client.DKISTClient.search",
+        autospec=True,
+        return_value=[],
+    )
+
+    with pytest.raises(ValueError, match="No results available for dataset"):
+        transfer_complete_datasets("null")
+
+
 def test_transfer_from_dataset_id(mocker, orchestrate_transfer_mock):
     get_inv_mock = mocker.patch(
         "dkist.net.helpers._get_dataset_inventory",
         autospec=True,
         return_value=[
             {
                 "Dataset ID": "AAAA",
@@ -59,46 +73,44 @@
     orchestrate_transfer_mock.assert_called_once_with(
         [Path("/data/pm_1_10/AAAA")],
         recursive=True,
         destination_path=Path("/~/pm_1_10"),
         destination_endpoint=None,
         progress=True,
         wait=True,
-        label_suffix="AAAA",
+        label=f"DKIST Python Tools - {datetime.datetime.now().strftime('%Y-%m-%dT%H-%M')} AAAA"
     )
 
     get_inv_mock.assert_called_once_with("AAAA")
 
 
 def test_transfer_from_table(orchestrate_transfer_mock, mocker):
     res = DKISTQueryResponseTable(
         {
             "Dataset ID": ["A", "B"],
             "Primary Proposal ID": ["pm_1_10", "pm_2_20"],
             "Storage Bucket": ["data", "data"],
         },
     )
 
-    transfer_complete_datasets(res)
+    transfer_complete_datasets(res, label="fibble")
 
-    kwargs = {"progress": True, "wait": True, "destination_endpoint": None}
+    kwargs = {"progress": True, "wait": True, "destination_endpoint": None, "label": "fibble"}
     orchestrate_transfer_mock.assert_has_calls(
         [
             mocker.call(
                 [Path("/data/pm_1_10/A")],
                 recursive=True,
                 destination_path=Path("/~/pm_1_10"),
-                label_suffix="A",
                 **kwargs
             ),
             mocker.call(
                 [Path("/data/pm_2_20/B")],
                 recursive=True,
                 destination_path=Path("/~/pm_2_20"),
-                label_suffix="B",
                 **kwargs
             ),
         ]
     )
 
 
 def test_transfer_from_UnifiedResponse(orchestrate_transfer_mock, mocker):
@@ -116,28 +128,26 @@
                 "Primary Proposal ID": ["pm_2_20"],
                 "Storage Bucket": ["data"],
             },
         ),
     )
     res._list[0].client = res._list[1].client = DKISTClient()
 
-    transfer_complete_datasets(res)
+    transfer_complete_datasets(res, label="fibble")
 
-    kwargs = {"progress": True, "wait": True, "destination_endpoint": None}
+    kwargs = {"progress": True, "wait": True, "destination_endpoint": None, "label": "fibble"}
     orchestrate_transfer_mock.assert_has_calls(
         [
             mocker.call(
                 [Path("/data/pm_1_10/A")],
                 recursive=True,
                 destination_path=Path("/~/pm_1_10"),
-                label_suffix="A",
                 **kwargs
             ),
             mocker.call(
                 [Path("/data/pm_2_20/B")],
                 recursive=True,
                 destination_path=Path("/~/pm_2_20"),
-                label_suffix="B",
                 **kwargs
             ),
         ]
     )
```

### Comparing `dkist-1.0.0b8/dkist/tests/coveragerc` & `dkist-1.0.0b9/dkist/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/tests/generate_aia_dataset.py` & `dkist-1.0.0b9/dkist/tests/generate_aia_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/tests/generate_eit_test_dataset.py` & `dkist-1.0.0b9/dkist/tests/generate_eit_test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/utils/inventory.py` & `dkist-1.0.0b9/dkist/utils/inventory.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/utils/sysinfo.py` & `dkist-1.0.0b9/dkist/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/utils/tests/test_inventory.py` & `dkist-1.0.0b9/dkist/utils/tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/wcs/models.py` & `dkist-1.0.0b9/dkist/wcs/models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/wcs/tests/test_coupled_compound_model.py` & `dkist-1.0.0b9/dkist/wcs/tests/test_coupled_compound_model.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist/wcs/tests/test_models.py` & `dkist-1.0.0b9/dkist/wcs/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/dkist.egg-info/PKG-INFO` & `dkist-1.0.0b9/dkist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: DKIST User Tools
 Home-page: http://dkist.nso.edu
 Author: NSO / AURA
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-1.0.0b8/dkist.egg-info/SOURCES.txt` & `dkist-1.0.0b9/dkist.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 dkist/data/test/EIT/efz20040301.060010_s.fits
 dkist/data/test/EIT/efz20040301.080010_s.fits
 dkist/data/test/EIT/efz20040301.090010_s.fits
 dkist/data/test/EIT/efz20040301.100010_s.fits
 dkist/data/test/EIT/efz20040301.110010_s.fits
 dkist/data/test/EIT/efz20040301.120010_s.fits
 dkist/data/test/EIT/eit_test_dataset.asdf
+dkist/data/test/small_visp/0.fits
+dkist/data/test/small_visp/1.fits
+dkist/data/test/small_visp/2.fits
+dkist/data/test/small_visp/test_visp.asdf
 dkist/dataset/__init__.py
 dkist/dataset/dataset.py
 dkist/dataset/tiled_dataset.py
 dkist/dataset/utils.py
 dkist/dataset/tests/__init__.py
 dkist/dataset/tests/test_dataset.py
 dkist/dataset/tests/test_plotting.py
```

### Comparing `dkist-1.0.0b8/docs/Makefile` & `dkist-1.0.0b9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/conf.py` & `dkist-1.0.0b9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/developer.rst` & `dkist-1.0.0b9/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/guide/install.rst` & `dkist-1.0.0b9/docs/guide/install.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/guide/level1data.rst` & `dkist-1.0.0b9/docs/guide/level1data.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/guide/loading.rst` & `dkist-1.0.0b9/docs/guide/loading.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/guide/net.rst` & `dkist-1.0.0b9/docs/guide/net.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/guide/usertools.rst` & `dkist-1.0.0b9/docs/guide/usertools.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/index.rst` & `dkist-1.0.0b9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/logo/icon_square.jpg` & `dkist-1.0.0b9/docs/logo/icon_square.jpg`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/make.bat` & `dkist-1.0.0b9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/docs/reference.rst` & `dkist-1.0.0b9/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/examples/create_dataset.py` & `dkist-1.0.0b9/examples/create_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/licenses/LICENSE.rst` & `dkist-1.0.0b9/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/licenses/TEMPLATE_LICENCE.rst` & `dkist-1.0.0b9/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/pyproject.toml` & `dkist-1.0.0b9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-1.0.0b8/setup.cfg` & `dkist-1.0.0b9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 	dask[array]>=2
 	globus-sdk>=3.0
 	gwcs>=0.18.0
 	matplotlib>=3.1
 	ndcube[plotting,reproject]>=2.0
 	numpy>=1.17
 	parfive[ftp]>=1.3
-	sunpy[net,asdf]>=3.0.2
+	sunpy[net,asdf]>=4
 setup_requires = setuptools_scm
 
 [options.extras_require]
 tests = 
 	pytest-astropy
 	pytest-cov
 	pytest-mock
@@ -92,21 +92,22 @@
 	ignore:ERFA function "taiutc"*
 	ignore:defusedxml.lxml is no longer supported and will be removed in a future release.
 	ignore:numpy.ufunc size changed:RuntimeWarning
 	ignore:numpy.ndarray size changed:RuntimeWarning
 	ignore:the imp module is deprecated in favour of importlib:DeprecationWarning:ipykernel.iostream
 	ignore:File.*asdf.extension.BuiltinExtension.*:asdf.exceptions.AsdfWarning
 	ignore:The .* argument to AsdfSchemaFile is deprecated
-	ignore:leap-second auto-update failed due to the following exception
 	ignore:File.*from package gwcs\=\=0\.18\.0\), but older package \(gwcs.*\) is installed.
-	ignore: File.*eit_test_dataset.asdf.* was created with extension class.*but older package.*is installed.
+	ignore: File.* was created with extension.*but older package.*is installed.
 	ignore:The distutils.sysconfig module is deprecated, use sysconfig instead:DeprecationWarning
 	ignore:ASDF functionality for astropy is being moved out of the astropy package to the new asdf-astropy package
 	ignore:FLIP_TOP_BOTTOM is deprecated and will be removed in Pillow.*
 	ignore::ResourceWarning
+	ignore:`np.float` is a deprecated alias for the builtin `float`. To silence this warning, use `float` by itself.::dask.array
+	ignore:leap-second auto-update failed due to the following exception
 
 [flake8]
 exclude = extern,sphinx,*parsetab.py,conftest.py,docs/conf.py,setup.py,__init__.py
 max-line-length = 100
 ignore = I1,D1,D200
 docstring-convention = numpy
```

### Comparing `dkist-1.0.0b8/tox.ini` & `dkist-1.0.0b9/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -8,28 +8,33 @@
 
 [testenv]
 passenv = CC
 setenv =
     MPLBACKEND = agg
     COLUMNS = 180
     PYTEST_COMMAND = pytest --cov=dkist --cov-config={toxinidir}/setup.cfg --verbose --timeout=120
+    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/astropy/simple https://pypi.anaconda.org/scipy-wheels-nightly/simple
 extras = tests
-commands = {env:PYTEST_COMMAND} {posargs}
+commands =
+    pip freeze --all --no-input
+    {env:PYTEST_COMMAND} {posargs}
 description =
     run tests
     devdeps: with the latest developer version of key dependencies
     oldestdeps: with the oldest supported version of all dependencies
 deps =
     # We currently require a development version of astropy for this to all work
     pytest-timeout
 
     # Devdeps installs our key dependancies from git to ensure we catch future
     # breaking changes before they make it to release
-    # Astropy is installed from nightly wheels
-    devdeps: astropy>=5.1.dev0
+    devdeps: astropy>=0.0.dev0
+    devdeps: numpy>=0.0.dev0
+    devdeps: scipy>=0.0.dev0
+    devdeps: matplotlib>=0.0.dev0
     devdeps: git+https://github.com/sunpy/sunpy
     devdeps: git+https://github.com/sunpy/ndcube
     devdeps: git+https://github.com/spacetelescope/gwcs
     devdeps: git+https://github.com/asdf-format/asdf
 
     # The oldest deps build runs all our tests against the oldest supported
     # versions
@@ -39,18 +44,16 @@
     oldestdeps: dask[array]<2.1
     oldestdeps: globus-sdk<1.8
     oldestdeps: gwcs<0.19
     oldestdeps: matplotlib<3.2
     oldestdeps: ndcube<2.1
     oldestdeps: numpy<1.19
     oldestdeps: parfive[ftp]<1.3
-    oldestdeps: sunpy[net,asdf]<3.0.3
+    oldestdeps: sunpy[net,asdf]<4.0.1
     oldestdeps: setuptools<60  # Use older setuptools to prevent distutils warning
-install_command =
-  devdeps: pip install --extra-index-url=https://pkgs.dev.azure.com/astropy-project/astropy/_packaging/nightly/pypi/simple/ {opts} {packages}
 
 [testenv:build_docs]
 extras = docs
 description = invoke sphinx-build to build the HTML docs
 commands = sphinx-build docs docs/_build/html -W -b html
 
 [testenv:codestyle]
```

