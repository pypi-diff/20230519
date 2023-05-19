# Comparing `tmp/timeseriesflattener-0.26.0.tar.gz` & `tmp/timeseriesflattener-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-0.26.0.tar", last modified: Thu May  4 07:54:51 2023, max compression
+gzip compressed data, was "timeseriesflattener-0.27.0.tar", last modified: Fri May 19 14:48:01 2023, max compression
```

## Comparing `timeseriesflattener-0.26.0.tar` & `timeseriesflattener-0.27.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.030712 timeseriesflattener-0.26.0/
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:50.998711 timeseriesflattener-0.26.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      896 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      994 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      252 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.006712 timeseriesflattener-0.26.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)      849 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      877 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2446 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     3056 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2871 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1286 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    54558 2023-05-04 07:54:41.000000 timeseriesflattener-0.26.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    11584 2023-05-04 07:54:51.030712 timeseriesflattener-0.26.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9185 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/README.md
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.006712 timeseriesflattener-0.26.0/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.006712 timeseriesflattener-0.26.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   811066 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)     4211 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      320 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)     5280 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/timeseriesflattener.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.010712 timeseriesflattener-0.26.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   130812 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    68248 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    77800 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.010712 timeseriesflattener-0.26.0/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      370 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)    49714 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.010712 timeseriesflattener-0.26.0/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4318 2023-05-04 07:54:41.000000 timeseriesflattener-0.26.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 07:54:51.030712 timeseriesflattener-0.26.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.010712 timeseriesflattener-0.26.0/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6145 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
--rw-r--r--   0 root         (0) root         (0)    43524 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_spec_objects.py
--rw-r--r--   0 root         (0) root         (0)    36771 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2234 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/logger.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/resolve_multiple_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     3168 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/testing/load_synth_data.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/testing/utils_for_testing.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11584 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3857 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      723 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9179 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/tests/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/tests/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1477 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/tests/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.026712 timeseriesflattener-0.26.0/tests/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      779 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1003 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   248865 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_text_data.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.026712 timeseriesflattener-0.26.0/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3490 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.026712 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     8865 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.030712 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18335 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     6598 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 root         (0) root         (0)    16795 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_resolve_multiple.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.771905 timeseriesflattener-0.27.0/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.731904 timeseriesflattener-0.27.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.719903 timeseriesflattener-0.27.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.731904 timeseriesflattener-0.27.0/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      896 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.731904 timeseriesflattener-0.27.0/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      994 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      252 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.735904 timeseriesflattener-0.27.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      877 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    54804 2023-05-19 14:47:50.000000 timeseriesflattener-0.27.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11584 2023-05-19 14:48:01.771905 timeseriesflattener-0.27.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9185 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.739904 timeseriesflattener-0.27.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.739904 timeseriesflattener-0.27.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   811066 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/timeseriesflattener.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.739904 timeseriesflattener-0.27.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   130849 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    68308 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    77800 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.743904 timeseriesflattener-0.27.0/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      370 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.743904 timeseriesflattener-0.27.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-05-19 14:47:50.000000 timeseriesflattener-0.27.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 14:48:01.771905 timeseriesflattener-0.27.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.719903 timeseriesflattener-0.27.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.743904 timeseriesflattener-0.27.0/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/column_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6145 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
+-rw-r--r--   0 root         (0) root         (0)    44130 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_spec_objects.py
+-rw-r--r--   0 root         (0) root         (0)    36771 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/logger.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/resolve_multiple_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/testing/load_synth_data.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/testing/utils_for_testing.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11584 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      723 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9179 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.723904 timeseriesflattener-0.27.0/tests/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.723904 timeseriesflattener-0.27.0/tests/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.751904 timeseriesflattener-0.27.0/tests/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.767905 timeseriesflattener-0.27.0/tests/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      779 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   248865 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_text_data.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.767905 timeseriesflattener-0.27.0/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.767905 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     9272 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.771905 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18335 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     7995 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 root         (0) root         (0)    16795 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_resolve_multiple.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_utils.py
```

### Comparing `timeseriesflattener-0.26.0/.cruft.json` & `timeseriesflattener-0.27.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/actions/test/action.yml` & `timeseriesflattener-0.27.0/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-0.27.0/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/dependabot.yml` & `timeseriesflattener-0.27.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/recommended_repo_setup.md` & `timeseriesflattener-0.27.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/workflows/check_for_rej.yml` & `timeseriesflattener-0.27.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/workflows/cruft.yml` & `timeseriesflattener-0.27.0/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-0.27.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/workflows/documentation.yml` & `timeseriesflattener-0.27.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-0.27.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-0.27.0/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/workflows/pre-commit.yml` & `timeseriesflattener-0.27.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/workflows/stalebot.yml` & `timeseriesflattener-0.27.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.github/workflows/static_type_checks.yml` & `timeseriesflattener-0.27.0/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.gitignore` & `timeseriesflattener-0.27.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.pre-commit-config.yaml` & `timeseriesflattener-0.27.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/.zenodo.json` & `timeseriesflattener-0.27.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/CHANGELOG.md` & `timeseriesflattener-0.27.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.27.0 (2023-05-19)
+### Feature
+* Add feature_name arg to group specs and make non-optional for non group specs ([`34df7a3`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/34df7a3561206d952cb17474f8c1efa097146e6f))
+
 ## v0.26.0 (2023-05-04)
 ### Feature
 * Add group spec for text predictor spec ([`75a0112`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/75a0112f7c2717d16e1996d5087d993ba7f75cc4))
 
 ### Fix
 * Update type hints ([`887bc06`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/887bc062bf970690077fea105b5ca77018049e6d))
 * Incorrect naming of resolve_multiple_fn ([`0a4607e`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/0a4607ee48e9dd6227205bca09ab123b6d30504a))
```

### Comparing `timeseriesflattener-0.26.0/CODE_OF_CONDUCT.md` & `timeseriesflattener-0.27.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/CONTRIBUTING.md` & `timeseriesflattener-0.27.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/LICENSE` & `timeseriesflattener-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/PKG-INFO` & `timeseriesflattener-0.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 0.26.0
+Version: 0.27.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.26.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.27.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-0.26.0/README.md` & `timeseriesflattener-0.27.0/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/citation.cff` & `timeseriesflattener-0.27.0/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/Makefile` & `timeseriesflattener-0.27.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/_static/favicon.ico` & `timeseriesflattener-0.27.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/_static/icon.png` & `timeseriesflattener-0.27.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/_static/icon_dark.png` & `timeseriesflattener-0.27.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/_static/terminology_figure.png` & `timeseriesflattener-0.27.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/conf.py` & `timeseriesflattener-0.27.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/faq.rst` & `timeseriesflattener-0.27.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/index.rst` & `timeseriesflattener-0.27.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-0.27.0/docs/tutorials/01_basic.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999620060790273%*

 * *Differences: {"'cells'": '{44: {\'source\': {insert: [(5, \'    feature_name="value",\\n\')]}}}'}*

```diff
@@ -1651,14 +1651,15 @@
             "outputs": [],
             "source": [
                 "pred_spec = PredictorSpec(\n",
                 "    values_name=\"value_name_1\",\n",
                 "    lookbehind_days=365,\n",
                 "    fallback=np.nan,\n",
                 "    resolve_multiple_fn=mean,\n",
+                "    feature_name=\"value\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `timeseriesflattener-0.26.0/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-0.27.0/docs/tutorials/02_advanced.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999255952380952%*

 * *Differences: {"'cells'": '{11: {\'source\': {insert: [(5, \'    feature_name="group_predictors",\\n\')]}}}'}*

```diff
@@ -265,14 +265,15 @@
             "outputs": [],
             "source": [
                 "pred_spec_batch = PredictorGroupSpec(\n",
                 "    values_loader=[\"synth_predictor_float\"],\n",
                 "    lookbehind_days=[365, 730],\n",
                 "    fallback=[np.nan],\n",
                 "    resolve_multiple_fn=[mean, maximum],\n",
+                "    feature_name=\"group_predictors\",\n",
                 ").create_combinations()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `timeseriesflattener-0.26.0/docs/tutorials/03_text.ipynb` & `timeseriesflattener-0.27.0/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/tutorials/img/term_a.png` & `timeseriesflattener-0.27.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/tutorials/img/term_b.png` & `timeseriesflattener-0.27.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/tutorials/img/term_c.png` & `timeseriesflattener-0.27.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/docs/tutorials/img/term_d.png` & `timeseriesflattener-0.27.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/icon.png` & `timeseriesflattener-0.27.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/paper/paper.bib` & `timeseriesflattener-0.27.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/paper/paper.md` & `timeseriesflattener-0.27.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/pyproject.toml` & `timeseriesflattener-0.27.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "0.26.0"
+version = "0.27.0"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
```

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/column_handler.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/feature_spec_objects.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/feature_spec_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,16 @@
 
 def resolve_from_dict_or_registry(data: Dict[str, Any]):
     """Resolve values_df from a dictionary or registry."""
 
     if "values_name" in data and data["values_name"] is not None:
         log.info(f"Resolving values_df from {data['values_name']}")
         data["values_df"] = split_dfs.get(data["values_name"])
-        data["feature_name"] = data["values_name"]
     else:
         if isinstance(data["values_loader"], str):
-            data["feature_name"] = data["values_loader"]
             data["values_loader"] = data_loaders.get(data["values_loader"])
 
         if callable(data["values_loader"]):
             if "loader_kwargs" not in data or data["loader_kwargs"] is None:
                 data["loader_kwargs"] = {}
 
             data["values_df"] = load_df_with_cache(
@@ -795,14 +793,19 @@
     )
 
     loader_kwargs: Optional[List[Dict[str, Any]]] = Field(
         default=None,
         description="""Optional kwargs for the values_loader.""",
     )
 
+    feature_name: str = Field(
+        description="""The name of the feature. Used for column name generation, e.g.
+            <prefix>_<feature_name>.""",
+    )
+
     def _check_loaders_are_valid(self):
         """Check that all loaders can be resolved from the data_loaders catalogue."""
         invalid_loaders: list = list(
             set(self.values_loader) - set(data_loaders.get_all().keys()),  # type: ignore
         )
         if len(invalid_loaders) != 0:
             # New line variable as f-string can't handle backslashes
@@ -907,14 +910,17 @@
         allowed_nan_value_prop (List[float]):
             If NaN is higher than this in the input dataframe during
             resolution, raise an error. Defaults to: [0.0].
         prefix (str):
             Prefix for column name, e,g, <prefix>_<feature_name>. Defaults to: pred.
         loader_kwargs (Optional[List[Dict[str, Any]]]):
             Optional kwargs for the values_loader.
+        feature_name (str):
+            The name of the feature. Used for column name generation, e.g.
+            <prefix>_<feature_name>.
         lookbehind_days (List[float]):
             How far behind to look for values
     """
 
     class Doc:
         short_description = """Specification for a group of predictors."""
 
@@ -935,46 +941,49 @@
         )
 
 
 class OutcomeGroupSpec(_MinGroupSpec):
     """Specification for a group of outcomes.
 
     Fields:
-    values_loader (Optional[Sequence[str]]):
-        Loader for the df. Tries to resolve from the data_loaders
-        registry, then calls the function which should return a dataframe.
-    values_name (Optional[List[str]]):
-        List of strings that corresponds to a key in a dictionary
-        of multiple dataframes that correspods to a name of a type of values.
-    values_df (Optional[DataFrame]):
-        Dataframe with the values.
-    input_col_name_override (Optional[str]):
-        Override for the column name to use as values in df.
-    output_col_name_override (Optional[str]):
-        Override for the column name to use as values in the
-        output df.
-    resolve_multiple_fn (List[Union[Callable, str]]):
-        Name of resolve multiple fn, resolved from
-        resolve_multiple_functions.py
-    fallback (Sequence[Union[Callable, str, float]]):
-        Which value to use if no values are found within interval_days.
-    allowed_nan_value_prop (List[float]):
-        If NaN is higher than this in the input dataframe during
-        resolution, raise an error. Defaults to: [0.0].
-    prefix (str):
-        Prefix for column name, e.g. <prefix>_<feature_name>. Defaults to: outc.
-    loader_kwargs (Optional[List[Dict[str,Any]]]):
-        Optional kwargs for the values_loader.
-    incident (Sequence[bool]):
-        Whether the outcome is incident or not, i.e. whether you
-        can experience it more than once. For example, type 2 diabetes is incident.
-        Incident outcomes can be handled in a vectorised way during resolution,
-         which is faster than non-incident outcomes.
-    lookahead_days (List[float]):
-        How far ahead to look for values
+        values_loader (Optional[Sequence[str]]):
+            Loader for the df. Tries to resolve from the data_loaders
+            registry, then calls the function which should return a dataframe.
+        values_name (Optional[List[str]]):
+            List of strings that corresponds to a key in a dictionary
+            of multiple dataframes that correspods to a name of a type of values.
+        values_df (Optional[DataFrame]):
+            Dataframe with the values.
+        input_col_name_override (Optional[str]):
+            Override for the column name to use as values in df.
+        output_col_name_override (Optional[str]):
+            Override for the column name to use as values in the
+            output df.
+        resolve_multiple_fn (List[Union[Callable, str]]):
+            Name of resolve multiple fn, resolved from
+            resolve_multiple_functions.py
+        fallback (Sequence[Union[Callable, str, float]]):
+            Which value to use if no values are found within interval_days.
+        allowed_nan_value_prop (List[float]):
+            If NaN is higher than this in the input dataframe during
+            resolution, raise an error. Defaults to: [0.0].
+        prefix (str):
+            Prefix for column name, e.g. <prefix>_<feature_name>. Defaults to: outc.
+        loader_kwargs (Optional[List[Dict[str, Any]]]):
+            Optional kwargs for the values_loader.
+        feature_name (str):
+            The name of the feature. Used for column name generation, e.g.
+            <prefix>_<feature_name>.
+        incident (Sequence[bool]):
+            Whether the outcome is incident or not, i.e. whether you
+            can experience it more than once. For example, type 2 diabetes is incident.
+            Incident outcomes can be handled in a vectorised way during resolution,
+             which is faster than non-incident outcomes.
+        lookahead_days (List[float]):
+            How far ahead to look for values
     """
 
     class Doc:
         short_description = """Specification for a group of outcomes."""
 
     prefix: str = Field(
         default="outc",
@@ -1024,14 +1033,17 @@
         fallback (Sequence[Union[Callable, str, float]]):
             Which value to use if no values are found within interval_days.
         allowed_nan_value_prop (List[float]):
             If NaN is higher than this in the input dataframe during
             resolution, raise an error. Defaults to: [0.0].
         prefix (str):
             Prefix for column name, e,g, <prefix>_<feature_name>. Defaults to: pred.
+        feature_name (str):
+            The name of the feature. Used for column name generation, e.g.
+            <prefix>_<feature_name>.
         loader_kwargs (Optional[List[Dict[str, Any]]]):
             Optional kwargs for the values_loader.
         lookbehind_days (List[float]):
             How far behind to look for values
         embedding_fn (List[Callable]):
             A function used for embedding the text. Should take a
         pandas series of strings and return a pandas dataframe of embeddings.
```

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/logger.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/resolve_multiple_functions.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/resolve_multiple_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener/utils.py` & `timeseriesflattener-0.27.0/src/timeseriesflattener/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 0.26.0
+Version: 0.27.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.26.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.27.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tasks.py` & `timeseriesflattener-0.27.0/tasks.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/conftest.py` & `timeseriesflattener-0.27.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-0.27.0/tests/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-0.27.0/tests/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-0.27.0/tests/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_sex.py` & `timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-0.27.0/tests/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/synth_sex.csv` & `timeseriesflattener-0.27.0/tests/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_data/raw/synth_text_data.csv` & `timeseriesflattener-0.27.0/tests/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-0.27.0/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,46 +33,52 @@
 def test_anyspec_init():
     """Test that AnySpec initialises correctly."""
     values_loader_name = "synth_predictor_float"
 
     spec = _AnySpec(
         values_loader=values_loader_name,
         prefix="test",
+        feature_name="test_feature",
     )
 
     assert isinstance(spec.values_df, pd.DataFrame)
-    assert spec.feature_name == values_loader_name
 
 
 def test_loader_kwargs():
     """Test that loader kwargs are passed correctly."""
     spec = _AnySpec(
         values_loader="synth_predictor_float",
         prefix="test",
         loader_kwargs={"n_rows": 10},
+        feature_name="test_feature",
     )
 
     assert len(spec.values_df) == 10
 
 
 def test_invalid_multiple_data_args():
     """Test that error is raised if multiple data args are passed."""
 
     with pytest.raises(ValueError, match=r".*nly one of.*"):
         _AnySpec(
             values_loader="synth_predictor_float",
             values_name="synth_data",
             prefix="test",
+            feature_name="test_feature",
         )
 
 
 def test_anyspec_incorrect_values_loader_str():
     """Raise error if values loader is not a key in registry."""
     with pytest.raises(ValueError, match=r".*in registry.*"):
-        _AnySpec(values_loader="I don't exist", prefix="test")
+        _AnySpec(
+            values_loader="I don't exist",
+            prefix="test",
+            feature_name="test_feature",
+        )
 
 
 def test_that_col_names_in_kwargs_exist_in_df():
     """Raise error if col name specified which is not in df."""
     # Create a sample dataframe
     df = pd.DataFrame({"A": [1, 2, 3], "B": [4, 5, 6], "C": [7, 8, 9]})
 
@@ -97,14 +103,15 @@
         values_name=[
             "value_name_1",
             "value_name_2",
         ],
         resolve_multiple_fn=["mean"],
         lookbehind_days=[30],
         fallback=[0],
+        feature_name="test_feature",
     ).create_combinations()
 
     assert len(group_spec) == 2
 
 
 def test_skip_all_if_no_need_to_process():
     """Test that no combinations are created if no need to process."""
@@ -113,14 +120,15 @@
             PredictorGroupSpec(
                 values_loader=["synth_predictor_float"],
                 input_col_name_override="value",
                 lookbehind_days=[1],
                 resolve_multiple_fn=["max"],
                 fallback=[0],
                 allowed_nan_value_prop=[0.5],
+                feature_name="test_feature",
             ).create_combinations(),
         )
         == 1
     )
 
 
 def test_skip_one_if_no_need_to_process():
@@ -128,38 +136,41 @@
     created_combinations = PredictorGroupSpec(
         values_loader=["synth_predictor_float"],
         input_col_name_override="value",
         lookbehind_days=[1, 2],
         resolve_multiple_fn=["max", "min"],
         fallback=[0],
         allowed_nan_value_prop=[0],
+        feature_name="test_feature",
     ).create_combinations()
 
     assert len(created_combinations) == 4
 
 
 def test_resolve_multiple_fn_to_str():
     """Test that resolve_multiple_fn is converted to str correctly."""
     pred_spec_batch = PredictorGroupSpec(
         values_loader=["synth_predictor_float"],
         lookbehind_days=[365, 730],
         fallback=[np.nan],
         resolve_multiple_fn=[maximum],
+        feature_name="test_feature",
     ).create_combinations()
 
     assert "maximum" in pred_spec_batch[0].get_col_str()
 
 
 def test_lookbehind_days_handles_floats():
     """Test that lookbheind days does not coerce floats into ints."""
     pred_spec_batch = PredictorGroupSpec(
         values_loader=["synth_predictor_float"],
         lookbehind_days=[2, 0.5],
         fallback=[np.nan],
         resolve_multiple_fn=[maximum],
+        feature_name="test_feature",
     ).create_combinations()
 
     assert pred_spec_batch[1].lookbehind_days == 0.5
 
 
 def get_lines_with_diff(text1: str, text2: str) -> List[str]:
     """Find all lines in text1 which are different from text2."""
@@ -243,14 +254,15 @@
     spec = PredictorGroupSpec(
         values_loader=("synth_predictor_binary", "synth_predictor_float"),
         loader_kwargs=[{"n_rows": 100}],
         prefix="test_",
         resolve_multiple_fn=["bool"],
         fallback=[0],
         lookbehind_days=[10],
+        feature_name="test_feature",
     )
 
     combinations = spec.create_combinations()
 
     pd.testing.assert_frame_equal(binary_100_rows, combinations[0].values_df)
     pd.testing.assert_frame_equal(float_100_rows, combinations[1].values_df)
 
@@ -269,13 +281,14 @@
         loader_kwargs=[{"n_rows": 10}, {"n_rows": 100}],
         prefix="test_",
         resolve_multiple_fn=["concatenate"],
         fallback=[0],
         lookbehind_days=[10],
         embedding_fn=[sklearn_embedding],
         embedding_fn_kwargs=[{"model": bow_model}],
+        feature_name="test_feature",
     )
 
     combinations = spec.create_combinations()
 
     pd.testing.assert_frame_equal(text_10_rows, combinations[0].values_df)
     pd.testing.assert_frame_equal(text_100_rows, combinations[1].values_df)
```

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 
 base_float_predictor_combinations = PredictorGroupSpec(
     values_loader=["synth_predictor_float"],
     lookbehind_days=[365, 730],
     resolve_multiple_fn=["mean"],
     fallback=[np.NaN],
     allowed_nan_value_prop=[0.0],
+    feature_name="test_feature",
 ).create_combinations()
 
 base_binary_predictor_combinations = PredictorGroupSpec(
     values_loader=["synth_predictor_binary"],
     lookbehind_days=[365, 730],
     resolve_multiple_fn=["max"],
     fallback=[np.NaN],
     allowed_nan_value_prop=[0.0],
+    feature_name="test_feature",
 ).create_combinations()
 
 
 @pytest.mark.parametrize(
     "predictor_specs",
     [base_float_predictor_combinations, base_binary_predictor_combinations],
 )
```

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,26 @@
 import numpy as np
 import pandas as pd
 import pytest
 from timeseriesflattener.feature_spec_objects import (
     OutcomeSpec,
     PredictorSpec,
     StaticSpec,
+    TextPredictorGroupSpec,
     TextPredictorSpec,
 )
 from timeseriesflattener.flattened_dataset import TimeseriesFlattener
 from timeseriesflattener.resolve_multiple_functions import latest, mean
-from timeseriesflattener.text_embedding_functions import sentence_transformers_embedding
+from timeseriesflattener.testing.text_embedding_functions import (
+    _load_bow_model,
+)
+from timeseriesflattener.text_embedding_functions import (
+    sentence_transformers_embedding,
+    sklearn_embedding,
+)
 
 
 def test_add_spec(synth_prediction_times: pd.DataFrame, synth_outcome: pd.DataFrame):
     # Create an instance of the class that contains the `add_spec` method
     dataset = TimeseriesFlattener(
         prediction_times_df=synth_prediction_times,
         drop_pred_times_with_insufficient_look_distance=False,
@@ -213,7 +220,50 @@
         drop_pred_times_with_insufficient_look_distance=True,
     )
     ts_flattener.add_spec([predictor_spec])
     df = ts_flattener.get_df()
     df = ts_flattener.get_df()
 
     assert df.shape[0] == 4
+
+
+def test_group_spec_feature_name(
+    synth_prediction_times: pd.DataFrame,
+    synth_outcome: pd.DataFrame,
+):
+    # Create an instance of the class that contains the `add_spec` method
+    dataset = TimeseriesFlattener(
+        prediction_times_df=synth_prediction_times,
+        drop_pred_times_with_insufficient_look_distance=False,
+    )
+
+    # Create sample specs
+    outcome_spec = OutcomeSpec(
+        values_df=synth_outcome,
+        feature_name="outcome",
+        lookahead_days=1,
+        resolve_multiple_fn=mean,
+        fallback=0,
+        incident=False,
+    )
+
+    bow_model = _load_bow_model()
+
+    predictor_spec = TextPredictorGroupSpec(
+        values_loader=("synth_text",),
+        prefix="test",
+        resolve_multiple_fn=["concatenate"],
+        fallback=[np.nan],
+        lookbehind_days=[100],
+        feature_name="bow",
+        embedding_fn=[sklearn_embedding],
+        embedding_fn_kwargs=[{"model": bow_model}],
+        input_col_name_override="text",
+    ).create_combinations()
+
+    dataset.add_spec(outcome_spec)
+    dataset.add_spec(predictor_spec)  # type: ignore
+
+    df = dataset.get_df()
+
+    # assert correct feature names
+    assert "test_bow-for_within_100_days_concatenate_fallback_nan" in df.columns
```

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_resolve_multiple.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_resolve_multiple.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_utils.py` & `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_utils.py`

 * *Files identical despite different names*

