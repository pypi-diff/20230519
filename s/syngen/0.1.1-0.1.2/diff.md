# Comparing `tmp/syngen-0.1.1.tar.gz` & `tmp/syngen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.1.1.tar", last modified: Tue May 16 15:17:40 2023, max compression
+gzip compressed data, was "syngen-0.1.2.tar", last modified: Fri May 19 07:30:18 2023, max compression
```

## Comparing `syngen-0.1.1.tar` & `syngen-0.1.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-16 15:16:16.000000 syngen-0.1.1/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-16 15:16:16.000000 syngen-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-16 15:16:16.000000 syngen-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-16 15:17:40.760525 syngen-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14309 2023-05-16 15:16:16.000000 syngen-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-16 15:16:16.000000 syngen-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-16 15:17:40.760525 syngen-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.748525 syngen-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.752525 syngen-0.1.1/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.752525 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15901 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    33025 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-19 07:28:40.000000 syngen-0.1.2/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-19 07:28:40.000000 syngen-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-19 07:28:40.000000 syngen-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-19 07:30:18.022168 syngen-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14309 2023-05-19 07:28:40.000000 syngen-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-19 07:28:40.000000 syngen-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-19 07:30:18.022168 syngen-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.006168 syngen-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.010168 syngen-0.1.2/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.010168 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6554 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33025 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-19 07:30:18.000000 syngen-0.1.2/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.1.1/LICENSE` & `syngen-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/PKG-INFO` & `syngen-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.1
+Version: 0.1.2
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.1 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.2 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.1.1/README.md` & `syngen-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/setup.cfg` & `syngen-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/infer.py` & `syngen-0.1.2/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/config/configurations.py` & `syngen-0.1.2/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/convertor/convertor.py` & `syngen-0.1.2/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.1.2/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/metrics/__init__.py` & `syngen-0.1.2/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.1.2/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.1.2/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.1.2/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/metrics/utils.py` & `syngen-0.1.2/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/reporters/reporters.py` & `syngen-0.1.2/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/strategies/strategies.py` & `syngen-0.1.2/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.1.2/src/syngen/ml/train_chain/train_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from tensorflow.keras.preprocessing.text import Tokenizer
 
 from syngen.ml.vae import *
 from syngen.ml.data_loaders import DataLoader
 from syngen.ml.utils import (
     slugify_parameters,
     fetch_dataset,
-    check_if_features_assigned
+    check_if_features_assigned,
+    generate_uuid,
+    generate_uuids
 )
 
 
 class AbstractHandler(ABC):
     @abstractmethod
     def set_next(self, handler):
         pass
@@ -234,24 +236,14 @@
                 if config_of_keys.get(key).get("type") == "PK" and not isinstance(df_slices[0][column][0], (str, UUID, ULID)):
                     cumm_len = 0
                     for i, frame in enumerate(df_slices):
                         frame[column] = frame[column].map(lambda pk_val: pk_val + cumm_len)
                         cumm_len += len(frame)
         return pd.concat(df_slices, ignore_index=True)
 
-    def _generate_uuids(self, version: int, size: int):
-        ulid = ULID()
-        generated_uuid_column = []
-        for i in range(size):
-            if version != "ulid":
-                generated_uuid_column.append(uuid.UUID(int=random.getrandbits(128), version=int(version)))
-            else:
-                generated_uuid_column.append(ulid.generate())
-        return generated_uuid_column
-
     def generate_vae(self, size, data, schema):
         self.vae = self.create_wrapper(
             self.wrapper_name,
             data,
             schema,
             metadata={"table_name": self.table_name},
             table_name=self.table_name,
@@ -273,19 +265,14 @@
             counts = features[col]["counts"]
             generated_column = [" ".join([self.synth_word(s, indexes, counts) for s in
                                           np.maximum(np.random.normal(i / j, 1, j).astype('int32'), 2)])
                                 for i, j in zip(*text_structures)]
             synthetic_infer[col] = generated_column
         return synthetic_infer
 
-    def generate_uuid(self, size, dataset, uuid_columns, synthetic_infer):
-        uuid_columns_types = dataset.uuid_columns_types
-        for col in uuid_columns:
-            synthetic_infer[col] = self._generate_uuids(uuid_columns_types[col], size)
-        return synthetic_infer
 
     def run_separate(self, params: Tuple):
         i, size = params
 
         if self.random_seed:
             seed(self.random_seeds_list[i])
 
@@ -302,15 +289,15 @@
             synthetic_infer = self.generate_vae(size, data, schema)
         if self.has_no_ml:
             synthetic_infer = self.generate_long_texts(size, synthetic_infer)
 
         dataset = fetch_dataset(self.paths["dataset_pickle_path"])
         uuid_columns = dataset.uuid_columns
         if uuid_columns:
-            synthetic_infer = self.generate_uuid(size, dataset, uuid_columns, synthetic_infer)
+            synthetic_infer = generate_uuid(size, dataset, uuid_columns, synthetic_infer)
 
         return synthetic_infer
 
     @staticmethod
     def split_by_batches(size, nodes):
         quote = int(size / nodes)
         data = [quote] * nodes
```

### Comparing `syngen-0.1.1/src/syngen/ml/utils/utils.py` & `syngen-0.1.2/src/syngen/ml/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,35 @@
 from datetime import datetime, timedelta
 
 import pandas as pd
 import numpy as np
 from slugify import slugify
 from loguru import logger
 import pickle as pkl
+import uuid
+from ulid import ULID
+from uuid import UUID
+import random
 
+def generate_uuids(version: int, size: int):
+    ulid = ULID()
+    generated_uuid_column = []
+    for i in range(size):
+        if version != "ulid":
+            generated_uuid_column.append(uuid.UUID(int=random.getrandbits(128), version=int(version)))
+        else:
+            generated_uuid_column.append(ulid.generate())
+    return generated_uuid_column
+
+
+def generate_uuid(size, dataset, uuid_columns, synthetic_infer):
+    uuid_columns_types = dataset.uuid_columns_types
+    for col in uuid_columns:
+        synthetic_infer[col] = generate_uuids(uuid_columns_types[col], size)
+    return synthetic_infer
 
 def get_date_columns(df: pd.DataFrame, str_columns: List[str]):
     # TODO: extend pattern to more formats
     # pattern = r'\d{2}(\.|/|\-)\d{2}(\.|/|\-)(\d{2}|\d{4})'
     # pattern = r"\s{0,1}\d+[-/\\:]\s{0,1}\d+[-/\\:]\s{0,1}\d+"
 
     def len_filter(x):
```

### Comparing `syngen-0.1.1/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.1.2/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/vae/models/dataset.py` & `syngen-0.1.2/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/vae/models/features.py` & `syngen-0.1.2/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/vae/models/model.py` & `syngen-0.1.2/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.1.2/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.1.2/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/ml/worker/worker.py` & `syngen-0.1.2/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen/train.py` & `syngen-0.1.2/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.1/src/syngen.egg-info/PKG-INFO` & `syngen-0.1.2/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.1
+Version: 0.1.2
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.1 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.2 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.1.1/src/syngen.egg-info/SOURCES.txt` & `syngen-0.1.2/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

